# Comparing `tmp/fps_kernels-0.5.1.tar.gz` & `tmp/fps_kernels-0.5.2.tar.gz`

## Comparing `fps_kernels-0.5.1.tar` & `fps_kernels-0.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/main.py
--rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/COPYING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fps_kernels-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/main.py
+-rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/COPYING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fps_kernels-0.5.2/PKG-INFO
```

### Comparing `fps_kernels-0.5.1/fps_kernels/main.py` & `fps_kernels-0.5.2/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/fps_kernels/routes.py` & `fps_kernels-0.5.2/fps_kernels/routes.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/fps_kernels/kernel_driver/connect.py` & `fps_kernels-0.5.2/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/fps_kernels/kernel_driver/driver.py` & `fps_kernels-0.5.2/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/fps_kernels/kernel_driver/kernelspec.py` & `fps_kernels-0.5.2/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/fps_kernels/kernel_driver/message.py` & `fps_kernels-0.5.2/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/fps_kernels/kernel_driver/paths.py` & `fps_kernels-0.5.2/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/fps_kernels/kernel_server/message.py` & `fps_kernels-0.5.2/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/fps_kernels/kernel_server/server.py` & `fps_kernels-0.5.2/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/.gitignore` & `fps_kernels-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/COPYING.md` & `fps_kernels-0.5.2/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/pyproject.toml` & `fps_kernels-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.5.1/PKG-INFO` & `fps_kernels-0.5.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fps_kernels
-Version: 0.5.1
+Version: 0.5.2
 Summary: An FPS plugin for the kernels API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

