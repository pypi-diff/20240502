# Comparing `tmp/agxclick-0.3.1.tar.gz` & `tmp/agxclick-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agxclick-0.3.1.tar", max compression
+gzip compressed data, was "agxclick-0.3.2.tar", max compression
```

## Comparing `agxclick-0.3.1.tar` & `agxclick-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1417 2024-03-22 14:00:24.674986 agxclick-0.3.1/README-pypi.md
--rw-r--r--   0        0        0      574 2024-03-22 14:14:51.936331 agxclick-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      649 2023-06-07 20:19:13.570644 agxclick-0.3.1/src/agxclick/__init__.py
--rw-r--r--   0        0        0     2450 2023-12-18 18:14:18.912567 agxclick-0.3.1/src/agxclick/agx_application.py
--rw-r--r--   0        0        0      264 2023-06-07 20:19:13.570644 agxclick-0.3.1/src/agxclick/application_step_listener.py
--rw-r--r--   0        0        0     1647 2023-06-07 20:19:13.570644 agxclick-0.3.1/src/agxclick/brick_reader.py
--rw-r--r--   0        0        0     2379 2023-06-07 20:19:13.570644 agxclick-0.3.1/src/agxclick/brick_utils.py
--rw-r--r--   0        0        0    10592 2023-11-01 08:36:26.627930 agxclick-0.3.1/src/agxclick/click_application.py
--rw-r--r--   0        0        0     9767 2023-11-10 09:56:26.356202 agxclick-0.3.1/src/agxclick/click_event_listener.py
--rw-r--r--   0        0        0    10192 2023-06-07 20:19:13.570644 agxclick-0.3.1/src/agxclick/click_robot.py
--rw-r--r--   0        0        0      736 2023-06-07 20:19:13.570644 agxclick-0.3.1/src/agxclick/graphics_throttler.py
--rw-r--r--   0        0        0     1319 2023-06-07 20:19:13.570644 agxclick-0.3.1/src/agxclick/keyboard_listener.py
--rw-r--r--   0        0        0    10274 2023-11-09 16:05:31.994357 agxclick-0.3.1/src/agxclick/message_factory.py
--rw-r--r--   0        0        0     1230 2023-06-07 20:19:13.570644 agxclick-0.3.1/src/agxclick/reset_batch_listener.py
--rw-r--r--   0        0        0      348 2023-06-07 20:19:13.570644 agxclick-0.3.1/src/agxclick/wallclock.py
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 agxclick-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1417 2024-05-02 07:39:28.500352 agxclick-0.3.2/README-pypi.md
+-rw-r--r--   0        0        0      574 2024-05-02 07:39:28.500352 agxclick-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      649 2023-06-07 20:19:13.570644 agxclick-0.3.2/src/agxclick/__init__.py
+-rw-r--r--   0        0        0     2450 2023-12-18 18:14:18.912567 agxclick-0.3.2/src/agxclick/agx_application.py
+-rw-r--r--   0        0        0      264 2023-06-07 20:19:13.570644 agxclick-0.3.2/src/agxclick/application_step_listener.py
+-rw-r--r--   0        0        0     1647 2023-06-07 20:19:13.570644 agxclick-0.3.2/src/agxclick/brick_reader.py
+-rw-r--r--   0        0        0     2379 2023-06-07 20:19:13.570644 agxclick-0.3.2/src/agxclick/brick_utils.py
+-rw-r--r--   0        0        0    10592 2023-11-01 08:36:26.627930 agxclick-0.3.2/src/agxclick/click_application.py
+-rw-r--r--   0        0        0     9767 2023-11-10 09:56:26.356202 agxclick-0.3.2/src/agxclick/click_event_listener.py
+-rw-r--r--   0        0        0    10192 2023-06-07 20:19:13.570644 agxclick-0.3.2/src/agxclick/click_robot.py
+-rw-r--r--   0        0        0      736 2023-06-07 20:19:13.570644 agxclick-0.3.2/src/agxclick/graphics_throttler.py
+-rw-r--r--   0        0        0     1319 2023-06-07 20:19:13.570644 agxclick-0.3.2/src/agxclick/keyboard_listener.py
+-rw-r--r--   0        0        0    10274 2023-11-09 16:05:31.994357 agxclick-0.3.2/src/agxclick/message_factory.py
+-rw-r--r--   0        0        0     1230 2023-06-07 20:19:13.570644 agxclick-0.3.2/src/agxclick/reset_batch_listener.py
+-rw-r--r--   0        0        0      348 2023-06-07 20:19:13.570644 agxclick-0.3.2/src/agxclick/wallclock.py
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 agxclick-0.3.2/PKG-INFO
```

### Comparing `agxclick-0.3.1/README-pypi.md` & `agxclick-0.3.2/README-pypi.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 Prerequisites: AGX and agxBrick
 
 ```bash
 # Latest version
 pip install agxclick -U
 # Specific version
-pip install agxclick==0.3.1
+pip install agxclick==0.3.2
 ```
 
 ## Usage Examples
 
 Visit the [GitHub repo](https://github.com/algoryx/click-mirror/agxClick/README.md) for usage examples.
 
 ## License
```

### Comparing `agxclick-0.3.1/pyproject.toml` & `agxclick-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "agxclick"
-version = "0.3.1"
+version = "0.3.2"
 description = "Controller to AGX Dynamics communication using pclick messaging"
 authors = ["Algoryx Simulation <contact@algoryx.se>"]
 license = "Apache-2.0"
 repository = "https://github.com/algoryx/click-mirror"
 readme = "README-pypi.md"
 packages = [
     { include = "agxclick", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-pclick = ">=0.3.1"
+pclick = ">=0.3.2"
 agxBrick = ">=0.6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `agxclick-0.3.1/src/agxclick/__init__.py` & `agxclick-0.3.2/src/agxclick/__init__.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/src/agxclick/agx_application.py` & `agxclick-0.3.2/src/agxclick/agx_application.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/src/agxclick/brick_reader.py` & `agxclick-0.3.2/src/agxclick/brick_reader.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/src/agxclick/brick_utils.py` & `agxclick-0.3.2/src/agxclick/brick_utils.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/src/agxclick/click_application.py` & `agxclick-0.3.2/src/agxclick/click_application.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/src/agxclick/click_event_listener.py` & `agxclick-0.3.2/src/agxclick/click_event_listener.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/src/agxclick/click_robot.py` & `agxclick-0.3.2/src/agxclick/click_robot.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/src/agxclick/graphics_throttler.py` & `agxclick-0.3.2/src/agxclick/graphics_throttler.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/src/agxclick/keyboard_listener.py` & `agxclick-0.3.2/src/agxclick/keyboard_listener.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/src/agxclick/message_factory.py` & `agxclick-0.3.2/src/agxclick/message_factory.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/src/agxclick/reset_batch_listener.py` & `agxclick-0.3.2/src/agxclick/reset_batch_listener.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.3.1/PKG-INFO` & `agxclick-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: agxclick
-Version: 0.3.1
+Version: 0.3.2
 Summary: Controller to AGX Dynamics communication using pclick messaging
 Home-page: https://github.com/algoryx/click-mirror
 License: Apache-2.0
 Author: Algoryx Simulation
 Author-email: contact@algoryx.se
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: agxBrick (>=0.6.0)
-Requires-Dist: pclick (>=0.3.1)
+Requires-Dist: pclick (>=0.3.2)
 Project-URL: Repository, https://github.com/algoryx/click-mirror
 Description-Content-Type: text/markdown
 
 # agxclick
 
 agxclick uses [pclick](https://pypi.org/project/pclick/), [AGX Dynamics](https://www.algoryx.se/agx-dynamics/) and [agxBrick](https://pypi.org/project/agxBrick/) to a implement a simulation application that implements Click out of the box for a provided Brick model.
 
@@ -42,15 +42,15 @@
 
 Prerequisites: AGX and agxBrick
 
 ```bash
 # Latest version
 pip install agxclick -U
 # Specific version
-pip install agxclick==0.3.1
+pip install agxclick==0.3.2
 ```
 
 ## Usage Examples
 
 Visit the [GitHub repo](https://github.com/algoryx/click-mirror/agxClick/README.md) for usage examples.
 
 ## License
```

