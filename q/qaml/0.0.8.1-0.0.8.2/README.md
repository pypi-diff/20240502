# Comparing `tmp/qaml-0.0.8.1.tar.gz` & `tmp/qaml-0.0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.8.1.tar", last modified: Tue Apr 30 19:51:43 2024, max compression
+gzip compressed data, was "qaml-0.0.8.2.tar", last modified: Thu May  2 19:42:14 2024, max compression
```

## Comparing `qaml-0.0.8.1.tar` & `qaml-0.0.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-30 19:51:43.733349 qaml-0.0.8.1/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.8.1/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-30 19:51:43.733204 qaml-0.0.8.1/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.8.1/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      770 2024-04-30 19:51:31.000000 qaml-0.0.8.1/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-30 19:51:43.732309 qaml-0.0.8.1/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.8.1/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.8.1/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      981 2024-04-29 18:11:49.000000 qaml-0.0.8.1/qaml/cli_agent.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    16669 2024-04-30 19:46:20.000000 qaml-0.0.8.1/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-30 19:51:43.733063 qaml-0.0.8.1/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      269 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       77 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-30 19:51:43.000000 qaml-0.0.8.1/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-30 19:51:43.733378 qaml-0.0.8.1/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-05-02 19:42:14.238920 qaml-0.0.8.2/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.8.2/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-05-02 19:42:14.238774 qaml-0.0.8.2/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.8.2/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      770 2024-05-02 19:39:37.000000 qaml-0.0.8.2/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-05-02 19:42:14.237911 qaml-0.0.8.2/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.8.2/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.8.2/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      981 2024-04-29 18:11:49.000000 qaml-0.0.8.2/qaml/cli_agent.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    16834 2024-05-02 19:37:05.000000 qaml-0.0.8.2/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-05-02 19:42:14.238636 qaml-0.0.8.2/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-05-02 19:42:14.000000 qaml-0.0.8.2/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      269 2024-05-02 19:42:14.000000 qaml-0.0.8.2/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-05-02 19:42:14.000000 qaml-0.0.8.2/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       77 2024-05-02 19:42:14.000000 qaml-0.0.8.2/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-05-02 19:42:14.000000 qaml-0.0.8.2/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-05-02 19:42:14.000000 qaml-0.0.8.2/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-05-02 19:42:14.238949 qaml-0.0.8.2/setup.cfg
```

### Comparing `qaml-0.0.8.1/LICENSE` & `qaml-0.0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.8.1/PKG-INFO` & `qaml-0.0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.8.1
+Version: 0.0.8.2
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.8.1/README.md` & `qaml-0.0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.8.1/pyproject.toml` & `qaml-0.0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.8.1"
+version = "0.0.8.2"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.8.1/qaml/__main__.py` & `qaml-0.0.8.2/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.8.1/qaml/cli_agent.py` & `qaml-0.0.8.2/qaml/cli_agent.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.8.1/qaml/client.py` & `qaml-0.0.8.2/qaml/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         accessibility_elements = [element for element in accessibility_elements if element.tag != "XCUIElementTypeStaticText" and element.tag != "android.widget.TextView" and element.tag != "XCUIElementTypeKey"]
         accessibility_elements = [{"left": int(element.attrib["x"]), "top": int(element.attrib["y"]), "width": int(element.attrib["width"]), "height": int(element.attrib["height"]), "type": element.attrib["type"], "label": element.attrib.get("label", "")} for element in accessibility_elements]
         # remove elements with no label
         accessibility_elements = [element for element in accessibility_elements if element["label"] and element["label"].strip()]
         return accessibility_elements
 
     def execute(self, script):
+        if not script.strip():
+            return
         screenshot = self.get_screenshot()
         accessibility_elements = self.get_accessibility_elements()
         payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.system_prompt, "accessibility_elements": accessibility_elements}
         response = self.req_session.post(f"{self.api_base_url}/v1/execute", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
         print(f"Action: {script} - Response: {response.text}")
         try:
             actions = response.json()
@@ -210,23 +212,26 @@
         direction_map = {"up": "down", "down": "up", "left": "right", "right": "left"}
         self.swipe(direction_map[direction])
 
     def type_text(self, text):
         self.driver.execute_script("mobile: shell", {"command": f"input text '{text}'"})
 
 class IOSClient(BaseClient):
-    def __init__(self, api_key, driver=None, use_mjpeg=True):
+    def __init__(self, api_key, driver=None, use_mjpeg=True, udid=None):
         super().__init__(api_key)
         self.available_functions["switch_to_app"] = self.switch_to_app
         self.platform = "iOS"
         self.use_mjpeg = use_mjpeg
+        self.udid = udid
         if driver:
             self.driver = driver
         else:
             def get_ios_udid():
+                if udid:
+                    return udid
                 system_profiler_output = subprocess.run(["system_profiler", "SPUSBDataType"], capture_output=True, text=True).stdout
                 serial_numbers = re.findall(r'(iPhone|iPad).*?Serial Number: *([^\n]+)', system_profiler_output, re.DOTALL)
 
                 if serial_numbers:
                     first_serial_number = serial_numbers[0][1].strip()
                     modified_serial_number = first_serial_number[:8] + '-' + first_serial_number[8:]
                     return modified_serial_number
@@ -331,15 +336,15 @@
 
             self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": usage, "durationSeconds": 0.005})  # Key down
             self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": 0x00, "durationSeconds": 0.005})  # Key up
 
     def switch_to_app(self, bundle_id):
         self.driver.activate_app(bundle_id)
 
-def Client(api_key, driver=None, use_mjpeg=True, use_hid_typing=False, use_accessibility_elements=False):
+def Client(api_key, driver=None, use_mjpeg=True, use_hid_typing=False, use_accessibility_elements=False, udid=None):
 
     def get_connected_android_devices():
         try:
             result = subprocess.run(["adb", "devices"], capture_output=True, text=True)
             devices = result.stdout.splitlines()[1:]  # Skip the first line, which is a header
             connected_devices = [line.split('\t')[0] for line in devices if "device" in line]
             return connected_devices
@@ -365,14 +370,14 @@
     android_devices = get_connected_android_devices()
     if android_devices:
         client = AndroidClient(api_key)
         client.use_accessibility_elements = use_accessibility_elements
         return client
 
     try:
-        client = IOSClient(api_key, use_mjpeg=use_mjpeg)
+        client = IOSClient(api_key, use_mjpeg=use_mjpeg, udid=udid)
         client.use_accessibility_elements = use_accessibility_elements
         client.use_hid_typing = use_hid_typing
         return client
     except:
         raise Exception("No connected devices found or driver provided.")
```

### Comparing `qaml-0.0.8.1/qaml.egg-info/PKG-INFO` & `qaml-0.0.8.2/qaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.8.1
+Version: 0.0.8.2
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

