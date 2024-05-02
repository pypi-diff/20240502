# Comparing `tmp/pyeasee-0.8.0.tar.gz` & `tmp/pyeasee-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasee-0.8.0.tar", last modified: Mon Mar 11 20:58:22 2024, max compression
+gzip compressed data, was "pyeasee-0.8.1.tar", last modified: Thu May  2 18:32:14 2024, max compression
```

## Comparing `pyeasee-0.8.0.tar` & `pyeasee-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2024-03-11 20:58:22.807043 pyeasee-0.8.0/
--rw-rw-r--   0 olal      (1000) olal      (1000)     3294 2024-03-11 20:58:22.807043 pyeasee-0.8.0/PKG-INFO
--rw-rw-r--   0 olal      (1000) olal      (1000)     2274 2024-03-04 19:18:42.000000 pyeasee-0.8.0/README.md
-drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2024-03-11 20:58:22.807043 pyeasee-0.8.0/pyeasee/
--rw-rw-r--   0 olal      (1000) olal      (1000)      185 2022-12-18 22:29:13.000000 pyeasee-0.8.0/pyeasee/__init__.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    14016 2023-11-07 19:40:02.000000 pyeasee-0.8.0/pyeasee/__main__.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    22952 2023-11-07 19:40:02.000000 pyeasee-0.8.0/pyeasee/charger.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    29600 2024-03-11 20:47:22.000000 pyeasee-0.8.0/pyeasee/const.py
--rw-rw-r--   0 olal      (1000) olal      (1000)    15515 2024-03-11 20:49:12.000000 pyeasee-0.8.0/pyeasee/easee.py
--rw-rw-r--   0 olal      (1000) olal      (1000)      776 2022-12-17 23:49:14.000000 pyeasee-0.8.0/pyeasee/exceptions.py
--rw-rw-r--   0 olal      (1000) olal      (1000)     8691 2023-06-10 20:31:11.000000 pyeasee-0.8.0/pyeasee/site.py
--rw-rw-r--   0 olal      (1000) olal      (1000)     2130 2022-12-18 22:29:13.000000 pyeasee-0.8.0/pyeasee/utils.py
-drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2024-03-11 20:58:22.807043 pyeasee-0.8.0/pyeasee.egg-info/
--rw-rw-r--   0 olal      (1000) olal      (1000)     3294 2024-03-11 20:58:22.000000 pyeasee-0.8.0/pyeasee.egg-info/PKG-INFO
--rw-rw-r--   0 olal      (1000) olal      (1000)      364 2024-03-11 20:58:22.000000 pyeasee-0.8.0/pyeasee.egg-info/SOURCES.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)        1 2024-03-11 20:58:22.000000 pyeasee-0.8.0/pyeasee.egg-info/dependency_links.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)       51 2024-03-11 20:58:22.000000 pyeasee-0.8.0/pyeasee.egg-info/entry_points.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)       25 2024-03-11 20:58:22.000000 pyeasee-0.8.0/pyeasee.egg-info/requires.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)        8 2024-03-11 20:58:22.000000 pyeasee-0.8.0/pyeasee.egg-info/top_level.txt
--rw-rw-r--   0 olal      (1000) olal      (1000)      168 2024-03-11 20:58:22.807043 pyeasee-0.8.0/setup.cfg
--rw-rw-r--   0 olal      (1000) olal      (1000)      787 2024-03-11 20:49:12.000000 pyeasee-0.8.0/setup.py
+drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2024-05-02 18:32:13.976436 pyeasee-0.8.1/
+-rw-rw-r--   0 olal      (1000) olal      (1000)     3204 2024-05-02 18:32:13.976436 pyeasee-0.8.1/PKG-INFO
+-rw-rw-r--   0 olal      (1000) olal      (1000)     2184 2024-04-01 15:36:52.000000 pyeasee-0.8.1/README.md
+drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2024-05-02 18:32:13.968437 pyeasee-0.8.1/pyeasee/
+-rw-rw-r--   0 olal      (1000) olal      (1000)      185 2022-12-18 22:29:13.000000 pyeasee-0.8.1/pyeasee/__init__.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    14016 2023-11-07 19:40:02.000000 pyeasee-0.8.1/pyeasee/__main__.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    22952 2023-11-07 19:40:02.000000 pyeasee-0.8.1/pyeasee/charger.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    29684 2024-05-02 18:28:34.000000 pyeasee-0.8.1/pyeasee/const.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)    15521 2024-05-02 18:30:33.000000 pyeasee-0.8.1/pyeasee/easee.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)      776 2022-12-17 23:49:14.000000 pyeasee-0.8.1/pyeasee/exceptions.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)     8691 2023-06-10 20:31:11.000000 pyeasee-0.8.1/pyeasee/site.py
+-rw-rw-r--   0 olal      (1000) olal      (1000)     2130 2022-12-18 22:29:13.000000 pyeasee-0.8.1/pyeasee/utils.py
+drwxrwxr-x   0 olal      (1000) olal      (1000)        0 2024-05-02 18:32:13.976436 pyeasee-0.8.1/pyeasee.egg-info/
+-rw-rw-r--   0 olal      (1000) olal      (1000)     3204 2024-05-02 18:32:12.000000 pyeasee-0.8.1/pyeasee.egg-info/PKG-INFO
+-rw-rw-r--   0 olal      (1000) olal      (1000)      364 2024-05-02 18:32:12.000000 pyeasee-0.8.1/pyeasee.egg-info/SOURCES.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)        1 2024-05-02 18:32:12.000000 pyeasee-0.8.1/pyeasee.egg-info/dependency_links.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)       51 2024-05-02 18:32:12.000000 pyeasee-0.8.1/pyeasee.egg-info/entry_points.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)       25 2024-05-02 18:32:12.000000 pyeasee-0.8.1/pyeasee.egg-info/requires.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)        8 2024-05-02 18:32:12.000000 pyeasee-0.8.1/pyeasee.egg-info/top_level.txt
+-rw-rw-r--   0 olal      (1000) olal      (1000)      168 2024-05-02 18:32:13.976436 pyeasee-0.8.1/setup.cfg
+-rw-rw-r--   0 olal      (1000) olal      (1000)      787 2024-05-02 18:30:33.000000 pyeasee-0.8.1/setup.py
```

### Comparing `pyeasee-0.8.0/PKG-INFO` & `pyeasee-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyeasee
-Version: 0.8.0
+Version: 0.8.1
 Summary: Easee EV charger API library
 Home-page: https://github.com/nordicopen/pyeasee
 Author: Ola Lidholm
 Author-email: olal@plea.se
 License: MIT
-Description: ![Maintenance](https://img.shields.io/maintenance/yes/2024.svg) ![Easee library](https://github.com/nordicopen/easee/workflows/Easee%20library/badge.svg)
+Description: ![Maintenance](https://img.shields.io/maintenance/yes/2024.svg)
         
         # Easee EV Charger library
         
         This library is an async thin wrapper around [Easee's Rest API](https://developer.easee.com/reference/post_api-accounts-login)
         
         ## Installation
```

### Comparing `pyeasee-0.8.0/README.md` & `pyeasee-0.8.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Maintenance](https://img.shields.io/maintenance/yes/2024.svg) ![Easee library](https://github.com/nordicopen/easee/workflows/Easee%20library/badge.svg)
+![Maintenance](https://img.shields.io/maintenance/yes/2024.svg)
 
 # Easee EV Charger library
 
 This library is an async thin wrapper around [Easee's Rest API](https://developer.easee.com/reference/post_api-accounts-login)
 
 ## Installation
```

### Comparing `pyeasee-0.8.0/pyeasee/__main__.py` & `pyeasee-0.8.1/pyeasee/__main__.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.8.0/pyeasee/charger.py` & `pyeasee-0.8.1/pyeasee/charger.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.8.0/pyeasee/const.py` & `pyeasee-0.8.1/pyeasee/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,44 +75,44 @@
     )
     state_circuitTotalAllocatedPhaseConductorCurrentL1 = 70  # Total current allocated to L1 by all chargers on the circuit. Sent in by master only [Double] ['Admin', 'Partner', 'User']
     state_circuitTotalAllocatedPhaseConductorCurrentL2 = 71  # Total current allocated to L2 by all chargers on the circuit. Sent in by master only [Double] ['Admin', 'Partner', 'User']
     state_circuitTotalAllocatedPhaseConductorCurrentL3 = 72  # Total current allocated to L3 by all chargers on the circuit. Sent in by master only [Double] ['Admin', 'Partner', 'User']
     state_circuitTotalPhaseConductorCurrentL1 = 73  # Total current in L1 (sum of all chargers on the circuit) Sent in by master only [Double] ['Admin', 'Partner', 'User']
     state_circuitTotalPhaseConductorCurrentL2 = 74  # Total current in L2 (sum of all chargers on the circuit) Sent in by master only [Double] ['Admin', 'Partner', 'User']
     state_circuitTotalPhaseConductorCurrentL3 = 75  # Total current in L3 (sum of all chargers on the circuit) Sent in by master only [Double] ['Admin', 'Partner', 'User']
-    NumberOfCarsConnected = 76  # Number of cars connected to this circuit [Integer] ['Admin', 'Partner']
-    NumberOfCarsCharging = 77  # Number of cars currently charging [Integer] ['Admin', 'Partner']
-    NumberOfCarsInQueue = (
+    state_numberOfCarsConnected = 76  # Number of cars connected to this circuit [Integer] ['Admin', 'Partner']
+    state_numberOfCarsCharging = 77  # Number of cars currently charging [Integer] ['Admin', 'Partner']
+    state_numberOfCarsInQueue = (
         78  # Number of cars currently in queue, waiting to be allocated power [Integer] ['Admin', 'Partner']
     )
-    NumberOfCarsFullyCharged = 79  # Number of cars that appear to be fully charged [Integer] ['Admin', 'Partner']
+    state_numberOfCarsFullyCharged = 79  # Number of cars that appear to be fully charged [Integer] ['Admin', 'Partner']
     state_chargerFirmware = 80  # Embedded software package release id [boot] [Integer] ['Admin', 'Partner', 'User']
-    ICCID = 81  # SIM integrated circuit card identifier [String] ['Admin', 'Partner']
+    state_ICCID = 81  # SIM integrated circuit card identifier [String] ['Admin', 'Partner']
     ModemFwId = 82  # Modem firmware version [String] ['Admin', 'Partner']
     OTAErrorCode = 83  # OTA error code, see table [event] [Integer] ['Admin', 'Partner']
     MobileNetworkOperator = 84  # Current mobile network operator [pollable] [String] ['Admin', 'Partner']
     RebootReason = 89  # Reason of reboot. Bitmask of flags. [Integer] ['Admin', 'Partner']
     PowerPCBVersion = 90  # Power PCB hardware version [Integer] ['Admin', 'Partner']
     ComPCBVersion = 91  # Communication PCB hardware version [Integer] ['Admin', 'Partner']
     state_reasonForNoCurrent = 96  # Enum describing why a charger with a car connected is not offering current to the car [Integer] ['Admin', 'Partner', 'User']
     LoadBalancingNumberOfConnectedChargers = 97  # Number of connected chargers in the load balancin. Including the master. Sent from Master only. [Integer] ['Admin', 'Partner']
-    UDPNumOfConnectedNodes = (
+    state_UDPNumOfConnectedNodes = (
         98  # Number of chargers connected to master through UDP / WIFI [Integer] ['Admin', 'Partner']
     )
-    LocalConnection = 99  # Slaves only. Current connection to master, 0 = None, 1= Radio, 2 = WIFI UDP, 3 = Radio and WIFI UDP [Integer] ['Admin', 'Partner']
-    PilotMode = 100  # Pilot Mode Letter (A-F) [event] [String] ['Admin', 'Partner']
+    state_localConnection = 99  # Slaves only. Current connection to master, 0 = None, 1= Radio, 2 = WIFI UDP, 3 = Radio and WIFI UDP [Integer] ['Admin', 'Partner']
+    state_pilotMode = 100  # Pilot Mode Letter (A-F) [event] [String] ['Admin', 'Partner']
     CarConnectedDEPRECATED = 101  # Car connection state [Boolean] ['Admin', 'Partner']
     state_smartCharging = (
         102  # Smart charging state enabled by capacitive touch button [event] [Boolean] ['Admin', 'Partner', 'User']
     )
     state_cableLocked = 103  # Cable lock state [event] [Boolean] ['Admin', 'Partner', 'User']
     state_cableRating = 104  # Cable rating read [Amperes][event] [Integer] ['Admin', 'Partner', 'User']
     PilotHigh = 105  # Pilot signal high [Volt][debug] [Integer] ['Admin', 'Partner']
     PilotLow = 106  # Pilot signal low [Volt][debug] [Integer] ['Admin', 'Partner']
-    BackPlateID = 107  # Back Plate RFID of charger [boot] [String] ['Admin', 'Partner']
+    state_backPlateID = 107  # Back Plate RFID of charger [boot] [String] ['Admin', 'Partner']
     state_userIDTokenReversed = 108  # User ID token string from RFID reading [event](NB! Must reverse these strings) [String] ['Admin', 'Partner']
     state_chargerOpMode = (
         109  # Charger operation mode according to charger mode table [event] [Integer] ['Admin', 'Partner', 'User']
     )
     state_outputPhase = 110  # Active output phase(s) to EV according to output phase type table. [event] [Integer] ['Admin', 'Partner', 'User']
     state_dynamicCircuitCurrentP1 = 111  # Dynamically set circuit maximum current for phase 1 [Amperes][event] [Double] ['Admin', 'Partner', 'User']
     state_dynamicCircuitCurrentP2 = 112  # Dynamically set circuit maximum current for phase 2 [Amperes][event] [Double] ['Admin', 'Partner', 'User']
@@ -126,21 +126,21 @@
     state_totalPower = 120  # Total power [kW][telemetry] [Double] ['Admin', 'Partner', 'User']
     state_sessionEnergy = 121  # Session accumulated energy [kWh][telemetry] [Double] ['Admin', 'Partner', 'User']
     state_energyPerHour = 122  # Accumulated energy per hour [kWh][event] [Double] ['Admin', 'Partner', 'User']
     LegacyEvStatus = 123  # 0 = not legacy ev, 1 = legacy ev detected, 2 = reviving ev [Integer] ['Admin', 'Partner']
     state_lifetimeEnergy = (
         124  # Accumulated energy in the lifetime of the charger [kWh] [Double] ['Admin', 'Partner', 'User']
     )
-    LifetimeRelaySwitches = 125  # Total number of relay switches in the lifetime of the charger (irrespective of the number of phases used) [Integer] ['Admin', 'Partner']
-    LifetimeHours = 126  # Total number of hours in operation [Integer] ['Admin', 'Partner']
+    state_lifetimeRelaySwitches = 125  # Total number of relay switches in the lifetime of the charger (irrespective of the number of phases used) [Integer] ['Admin', 'Partner']
+    state_lifetimeHours = 126  # Total number of hours in operation [Integer] ['Admin', 'Partner']
     DynamicCurrentOfflineFallbackDEPRICATED = (
         127  # Maximum circuit current when offline [event] [Integer] ['Admin', 'Partner']
     )
     state_userIDToken = 128  # User ID token string from RFID reading [event] [String] ['Admin', 'Partner']
-    ChargingSession = 129  # Charging sessions [json][event] [String] ['Admin', 'Partner']
+    state_ChargingSession = 129  # Charging sessions [json][event] [String] ['Admin', 'Partner']
     state_cellRSSI = 130  # Cellular signal strength [dBm][telemetry] [Integer] ['Admin', 'Partner', 'User']
     CellRAT = 131  # Cellular radio access technology according to RAT table [event] [Integer] ['Admin', 'Partner']
     state_wiFiRSSI = 132  # WiFi signal strength [dBm][telemetry] [Integer] ['Admin', 'Partner', 'User']
     CellAddress = 133  # IP address assigned by cellular network [debug] [String] ['Admin', 'Partner']
     WiFiAddress = 134  # IP address assigned by WiFi network [debug] [String] ['Admin', 'Partner']
     WiFiType = 135  # WiFi network type letters (G, N, AC, etc) [debug] [String] ['Admin', 'Partner']
     state_localRSSI = 136  # Local radio signal strength [dBm][telemetry] [Integer] ['Admin', 'Partner', 'User']
@@ -340,16 +340,16 @@
     state_phaseMappingReport = 81  # Charger vs Meter phase correlation report [String] ['Admin', 'Partner']
     state_phaseLearningStatus = 82  # Status of the phaselearning/loadbalancing [String] ['Admin', 'Partner']
     config_modbusConfiguration = 85  # Complete Modbus Configuration [String] ['Admin', 'Partner', 'User']
     state_loadbalanceThrottle = 86  # Throttle level [percent] [Integer] ['Admin', 'Partner']
     state_availableCurrentL1 = 87  # Available Current for Balancing in Amps [Double] ['Admin', 'Partner', 'User']
     state_availableCurrentL2 = 88  # Available Current for Balancing in Amps [Double] ['Admin', 'Partner', 'User']
     state_availableCurrentL3 = 89  # Available Current for Balancing in Amps [Double] ['Admin', 'Partner', 'User']
-    MeterErrors = 90  # Meter Errors [Integer] ['Admin', 'Partner']
-    APMacAddress = 91  # Mac Address of the Wifi access point [String] ['Admin', 'Partner']
+    state_meterErrors = 90  # Meter Errors [Integer] ['Admin', 'Partner']
+    state_APMacAddress = 91  # Mac Address of the Wifi access point [String] ['Admin', 'Partner']
     state_wifiReconnects = 92  # Number of sucessful reconnects to AP [Integer] ['Admin', 'Partner']
     state_ledMode = 100  # Current LED pattern [Integer] ['Admin', 'Partner', 'User']
     state_equalizedChargeCurrentL1 = (
         105  # Charge current controlled by Equalizer in Amps [Double] ['Admin', 'Partner', 'User']
     )
     state_equalizedChargeCurrentL2 = (
         106  # Charge current controlled by Equalizer in Amps [Double] ['Admin', 'Partner', 'User']
```

### Comparing `pyeasee-0.8.0/pyeasee/easee.py` & `pyeasee-0.8.1/pyeasee/easee.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     NotFoundException,
     ServerFailureException,
     TooManyRequestsException,
 )
 from .site import Site, SiteState
 from .utils import convert_stream_data
 
-__VERSION__ = "0.8.0"
+__VERSION__ = "0.8.1"
 
 _LOGGER = logging.getLogger(__name__)
 
 SR_MIN_BACKOFF = 0
 SR_MAX_BACKOFF = 300
 SR_INC_BACKOFF = 30
 
@@ -240,15 +240,15 @@
     async def _sr_close_cb(self) -> None:
         """
         Signalr disconnected callback - called from signalr thread, internal use only
         """
         _LOGGER.debug("SignalR stream disconnected")
         self.sr_connection = None
         self.sr_connected = False
-        self._sr_connect(SR_INC_BACKOFF)
+        await self._sr_connect(SR_INC_BACKOFF)
 
     async def _sr_error_cb(self, message: CompletionMessage) -> None:
         _LOGGER.debug("SignalR error recevied {message.error}")
 
     async def _sr_product_update_cb(self, stuff: List[Dict[str, Any]]) -> None:
         """
         Signalr new data recieved callback - called from signalr thread, internal use only
```

### Comparing `pyeasee-0.8.0/pyeasee/exceptions.py` & `pyeasee-0.8.1/pyeasee/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.8.0/pyeasee/site.py` & `pyeasee-0.8.1/pyeasee/site.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.8.0/pyeasee/utils.py` & `pyeasee-0.8.1/pyeasee/utils.py`

 * *Files identical despite different names*

### Comparing `pyeasee-0.8.0/pyeasee.egg-info/PKG-INFO` & `pyeasee-0.8.1/pyeasee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyeasee
-Version: 0.8.0
+Version: 0.8.1
 Summary: Easee EV charger API library
 Home-page: https://github.com/nordicopen/pyeasee
 Author: Ola Lidholm
 Author-email: olal@plea.se
 License: MIT
-Description: ![Maintenance](https://img.shields.io/maintenance/yes/2024.svg) ![Easee library](https://github.com/nordicopen/easee/workflows/Easee%20library/badge.svg)
+Description: ![Maintenance](https://img.shields.io/maintenance/yes/2024.svg)
         
         # Easee EV Charger library
         
         This library is an async thin wrapper around [Easee's Rest API](https://developer.easee.com/reference/post_api-accounts-login)
         
         ## Installation
```

### Comparing `pyeasee-0.8.0/setup.py` & `pyeasee-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os.path
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="pyeasee",
-    version="0.8.0",
+    version="0.8.1",
     description="Easee EV charger API library",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nordicopen/pyeasee",
     author="Ola Lidholm",
     author_email="olal@plea.se",
     license="MIT",
```

