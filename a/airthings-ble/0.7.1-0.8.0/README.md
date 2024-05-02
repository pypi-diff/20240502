# Comparing `tmp/airthings_ble-0.7.1.tar.gz` & `tmp/airthings_ble-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airthings_ble-0.7.1.tar", max compression
+gzip compressed data, was "airthings_ble-0.8.0.tar", max compression
```

## Comparing `airthings_ble-0.7.1.tar` & `airthings_ble-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-03-12 22:05:45.411091 airthings_ble-0.7.1/LICENSE
--rw-r--r--   0        0        0      985 2024-03-12 22:05:45.411091 airthings_ble-0.7.1/README.md
--rw-r--r--   0        0        0      304 2024-03-12 22:05:46.839092 airthings_ble-0.7.1/airthings_ble/__init__.py
--rw-r--r--   0        0        0     2132 2024-03-12 22:05:45.411091 airthings_ble-0.7.1/airthings_ble/const.py
--rw-r--r--   0        0        0     4048 2024-03-12 22:05:45.411091 airthings_ble-0.7.1/airthings_ble/device_type.py
--rw-r--r--   0        0        0    24097 2024-03-12 22:05:45.411091 airthings_ble-0.7.1/airthings_ble/parser.py
--rw-r--r--   0        0        0        0 2024-03-12 22:05:45.411091 airthings_ble-0.7.1/airthings_ble/py.typed
--rw-r--r--   0        0        0     2182 2024-03-12 22:05:46.815092 airthings_ble-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 airthings_ble-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/LICENSE
+-rw-r--r--   0        0        0      985 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/README.md
+-rw-r--r--   0        0        0      304 2024-05-02 09:40:11.482850 airthings_ble-0.8.0/airthings_ble/__init__.py
+-rw-r--r--   0        0        0     2157 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/airthings_ble/const.py
+-rw-r--r--   0        0        0     4048 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/airthings_ble/device_type.py
+-rw-r--r--   0        0        0    25217 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/airthings_ble/parser.py
+-rw-r--r--   0        0        0        0 2024-05-02 09:40:09.242837 airthings_ble-0.8.0/airthings_ble/py.typed
+-rw-r--r--   0        0        0     2182 2024-05-02 09:40:11.458850 airthings_ble-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 airthings_ble-0.8.0/PKG-INFO
```

### Comparing `airthings_ble-0.7.1/LICENSE` & `airthings_ble-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.7.1/README.md` & `airthings_ble-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.7.1/airthings_ble/const.py` & `airthings_ble-0.8.0/airthings_ble/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,7 +48,9 @@
 BQ_TO_PCI_MULTIPLIER = 0.027
 
 CO2_MAX = 65534
 VOC_MAX = 65534
 PERCENTAGE_MAX = 100
 RADON_MAX = 16383
 TEMPERATURE_MAX = 100
+
+MAX_UPDATE_ATTEMPTS = 3
```

### Comparing `airthings_ble-0.7.1/airthings_ble/device_type.py` & `airthings_ble-0.8.0/airthings_ble/device_type.py`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.7.1/airthings_ble/parser.py` & `airthings_ble-0.8.0/airthings_ble/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from async_interrupt import interrupt
 from bleak import BleakClient, BleakError
 from bleak.backends.device import BLEDevice
 from bleak_retry_connector import BleakClientWithServiceCache, establish_connection
 
 from .const import (
+    MAX_UPDATE_ATTEMPTS,
     BQ_TO_PCI_MULTIPLIER,
     CHAR_UUID_DATETIME,
     CHAR_UUID_DEVICE_NAME,
     CHAR_UUID_FIRMWARE_REV,
     CHAR_UUID_HARDWARE_REV,
     CHAR_UUID_HUMIDITY,
     CHAR_UUID_ILLUMINANCE_ACCELEROMETER,
@@ -338,34 +339,45 @@
     """
 
     message: bytearray | None
 
     def __init__(self, message_size: int):
         self.message = None
         self._message_size = message_size
-        self._event = asyncio.Event()
+        self._loop = asyncio.get_running_loop()
+        self._future: asyncio.Future[None] = self._loop.create_future()
 
     def _full_message_received(self) -> bool:
         return self.message is not None and len(self.message) >= self._message_size
 
     def __call__(self, _: Any, data: bytearray) -> None:
         if self.message is None:
             self.message = data
         elif not self._full_message_received():
             self.message += data
         if self._full_message_received():
-            self._event.set()
+            self._future.set_result(None)
 
-    async def wait_for_message(self) -> None:
+    def _on_timeout(self) -> None:
+        if not self._future.done():
+            self._future.set_exception(
+                asyncio.TimeoutError("Timeout waiting for message")
+            )
+
+    async def wait_for_message(self, timeout: float) -> None:
         """Waits until the full message is received.
 
         If the full message has already been received, this method returns immediately.
         """
         if not self._full_message_received():
-            await self._event.wait()
+            timer_handle = self._loop.call_later(timeout, self._on_timeout)
+            try:
+                await self._future
+            finally:
+                timer_handle.cancel()
 
 
 def get_radon_level(data: float) -> str:
     """Returns the applicable radon level"""
     if data <= VERY_LOW[1]:
         radon_level = VERY_LOW[2]
     elif data <= LOW[1]:
@@ -599,16 +611,15 @@
 
                     # Set up the notification handlers
                     await client.start_notify(characteristic, command_data_receiver)
                     # send command to this 'indicate' characteristic
                     await client.write_gatt_char(characteristic, bytearray(decoder.cmd))
                     # Wait for up to one second to see if a callback comes in.
                     try:
-                        async with asyncio_timeout(1):
-                            await command_data_receiver.wait_for_message()
+                        await command_data_receiver.wait_for_message(5)
                     except asyncio.TimeoutError:
                         self.logger.warning("Timeout getting command data.")
 
                     command_sensor_data = decoder.decode_data(
                         self.logger, command_data_receiver.message
                     )
                     if command_sensor_data is not None:
@@ -633,14 +644,32 @@
         """Handle disconnect from device."""
         self.logger.debug("Disconnected from %s", client.address)
         if not disconnect_future.done():
             disconnect_future.set_result(True)
 
     async def update_device(self, ble_device: BLEDevice) -> AirthingsDevice:
         """Connects to the device through BLE and retrieves relevant data"""
+        for attempt in range(MAX_UPDATE_ATTEMPTS):
+            is_final_attempt = attempt == MAX_UPDATE_ATTEMPTS - 1
+            try:
+                return await self._update_device(ble_device)
+            except DisconnectedError:
+                if is_final_attempt:
+                    raise
+                self.logger.debug(
+                    "Unexpectedly disconnected from %s", ble_device.address
+                )
+            except BleakError as err:
+                if is_final_attempt:
+                    raise
+                self.logger.debug("Bleak error: %s", err)
+        raise RuntimeError("Should not reach this point")
+
+    async def _update_device(self, ble_device: BLEDevice) -> AirthingsDevice:
+        """Connects to the device through BLE and retrieves relevant data"""
         device = AirthingsDevice()
         loop = asyncio.get_running_loop()
         disconnect_future = loop.create_future()
         client: BleakClientWithServiceCache = (
             await establish_connection(  # pylint: disable=line-too-long
                 BleakClientWithServiceCache,  # type: ignore
                 ble_device,
@@ -659,13 +688,12 @@
                 await self._get_device_characteristics(client, device)
                 await self._get_service_characteristics(client, device)
         except BleakError as err:
             if "not found" in str(err):  # In future bleak this is a named exception
                 # Clear the char cache since a char is likely
                 # missing from the cache
                 await client.clear_cache()
-        except DisconnectedError:
-            self.logger.debug("Unexpectedly disconnected from %s", client.address)
+            raise
         finally:
             await client.disconnect()
 
         return device
```

### Comparing `airthings_ble-0.7.1/pyproject.toml` & `airthings_ble-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airthings-ble"
-version = "0.7.1"
+version = "0.8.0"
 description = "Manage Airthings BLE devices"
 authors = ["Vincent Giorgi", "Ståle Storø Hauknes"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/Airthings/airthings-ble"
 documentation = "https://airthings-ble.readthedocs.io"
 classifiers = [
```

### Comparing `airthings_ble-0.7.1/PKG-INFO` & `airthings_ble-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airthings-ble
-Version: 0.7.1
+Version: 0.8.0
 Summary: Manage Airthings BLE devices
 Home-page: https://github.com/Airthings/airthings-ble
 License: Apache Software License 2.0
 Author: Vincent Giorgi
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

