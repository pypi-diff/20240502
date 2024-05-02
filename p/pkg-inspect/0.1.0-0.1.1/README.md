# Comparing `tmp/pkg_inspect-0.1.0.tar.gz` & `tmp/pkg_inspect-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_inspect-0.1.0.tar", last modified: Thu May  2 01:55:16 2024, max compression
+gzip compressed data, was "pkg_inspect-0.1.1.tar", last modified: Thu May  2 01:59:21 2024, max compression
```

## Comparing `pkg_inspect-0.1.0.tar` & `pkg_inspect-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:55:16.225755 pkg_inspect-0.1.0/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.1.0/LICENSE.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.1.0/MANIFEST.in
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-02 01:55:16.225463 pkg_inspect-0.1.0/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.1.0/README.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      956 2024-05-02 01:55:16.226626 pkg_inspect-0.1.0/setup.cfg
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.1.0/setup.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:55:16.215730 pkg_inspect-0.1.0/src/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      129 2024-05-02 01:20:19.000000 pkg_inspect-0.1.0/src/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:55:16.216034 pkg_inspect-0.1.0/src/pkg_inspect/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       66 2024-04-29 03:13:14.000000 pkg_inspect-0.1.0/src/pkg_inspect/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:55:16.218955 pkg_inspect-0.1.0/src/pkg_inspect/pkg_functions/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       25 2024-04-24 00:55:56.000000 pkg_inspect-0.1.0/src/pkg_inspect/pkg_functions/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13184 2024-05-02 01:11:40.000000 pkg_inspect-0.1.0/src/pkg_inspect/pkg_functions/functions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:55:16.221195 pkg_inspect-0.1.0/src/pkg_inspect/pkg_modules/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      148 2024-04-29 03:13:14.000000 pkg_inspect-0.1.0/src/pkg_inspect/pkg_modules/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    48812 2024-05-02 01:11:40.000000 pkg_inspect-0.1.0/src/pkg_inspect/pkg_modules/pkg_inspect.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10121 2024-05-01 23:52:03.000000 pkg_inspect-0.1.0/src/pkg_inspect/pkg_modules/pkg_metrics.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    43685 2024-05-02 00:20:34.000000 pkg_inspect-0.1.0/src/pkg_inspect/pkg_modules/pkg_versions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:55:16.223573 pkg_inspect-0.1.0/src/pkg_inspect/pkg_utils/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       21 2024-04-22 02:40:00.000000 pkg_inspect-0.1.0/src/pkg_inspect/pkg_utils/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4523 2024-05-02 01:11:40.000000 pkg_inspect-0.1.0/src/pkg_inspect/pkg_utils/exception.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1588 2024-04-29 03:16:50.000000 pkg_inspect-0.1.0/src/pkg_inspect/pkg_utils/util_types.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    48422 2024-05-01 04:36:26.000000 pkg_inspect-0.1.0/src/pkg_inspect/pkg_utils/utils.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:55:16.217949 pkg_inspect-0.1.0/src/pkg_inspect.egg-info/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-02 01:55:16.000000 pkg_inspect-0.1.0/src/pkg_inspect.egg-info/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      701 2024-05-02 01:55:16.000000 pkg_inspect-0.1.0/src/pkg_inspect.egg-info/SOURCES.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-02 01:55:16.000000 pkg_inspect-0.1.0/src/pkg_inspect.egg-info/dependency_links.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-02 01:55:16.000000 pkg_inspect-0.1.0/src/pkg_inspect.egg-info/top_level.txt
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:55:16.224569 pkg_inspect-0.1.0/tests/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.1.0/tests/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-04-29 03:16:50.000000 pkg_inspect-0.1.0/tests/test_pipinspect.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:59:21.345986 pkg_inspect-0.1.1/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.1.1/LICENSE.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.1.1/MANIFEST.in
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-02 01:59:21.345698 pkg_inspect-0.1.1/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.1.1/README.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      956 2024-05-02 01:59:21.346982 pkg_inspect-0.1.1/setup.cfg
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.1.1/setup.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:59:21.331996 pkg_inspect-0.1.1/src/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      129 2024-05-02 01:58:59.000000 pkg_inspect-0.1.1/src/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:59:21.332358 pkg_inspect-0.1.1/src/pkg_inspect/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       66 2024-04-29 03:13:14.000000 pkg_inspect-0.1.1/src/pkg_inspect/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:59:21.335236 pkg_inspect-0.1.1/src/pkg_inspect/pkg_functions/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       25 2024-04-24 00:55:56.000000 pkg_inspect-0.1.1/src/pkg_inspect/pkg_functions/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13184 2024-05-02 01:11:40.000000 pkg_inspect-0.1.1/src/pkg_inspect/pkg_functions/functions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:59:21.338828 pkg_inspect-0.1.1/src/pkg_inspect/pkg_modules/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      165 2024-05-02 01:58:47.000000 pkg_inspect-0.1.1/src/pkg_inspect/pkg_modules/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    48812 2024-05-02 01:11:40.000000 pkg_inspect-0.1.1/src/pkg_inspect/pkg_modules/pkg_inspect.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10121 2024-05-01 23:52:03.000000 pkg_inspect-0.1.1/src/pkg_inspect/pkg_modules/pkg_metrics.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    43685 2024-05-02 00:20:34.000000 pkg_inspect-0.1.1/src/pkg_inspect/pkg_modules/pkg_versions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:59:21.342723 pkg_inspect-0.1.1/src/pkg_inspect/pkg_utils/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       21 2024-04-22 02:40:00.000000 pkg_inspect-0.1.1/src/pkg_inspect/pkg_utils/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4523 2024-05-02 01:11:40.000000 pkg_inspect-0.1.1/src/pkg_inspect/pkg_utils/exception.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1588 2024-04-29 03:16:50.000000 pkg_inspect-0.1.1/src/pkg_inspect/pkg_utils/util_types.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    48422 2024-05-01 04:36:26.000000 pkg_inspect-0.1.1/src/pkg_inspect/pkg_utils/utils.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:59:21.334103 pkg_inspect-0.1.1/src/pkg_inspect.egg-info/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-02 01:59:21.000000 pkg_inspect-0.1.1/src/pkg_inspect.egg-info/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      701 2024-05-02 01:59:21.000000 pkg_inspect-0.1.1/src/pkg_inspect.egg-info/SOURCES.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-02 01:59:21.000000 pkg_inspect-0.1.1/src/pkg_inspect.egg-info/dependency_links.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-02 01:59:21.000000 pkg_inspect-0.1.1/src/pkg_inspect.egg-info/top_level.txt
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 01:59:21.344507 pkg_inspect-0.1.1/tests/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.1.1/tests/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-04-29 03:16:50.000000 pkg_inspect-0.1.1/tests/test_pipinspect.py
```

### Comparing `pkg_inspect-0.1.0/LICENSE.md` & `pkg_inspect-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.0/PKG-INFO` & `pkg_inspect-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg_inspect
-Version: 0.1.0
+Version: 0.1.1
 Summary: A comprehensive tools to inspect Python packages and Python installations.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.1.0/README.md` & `pkg_inspect-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.0/setup.cfg` & `pkg_inspect-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pkg_inspect
-version = 0.1.0
+version = 0.1.1
 author = Yousef Abuzahrieh
 author_email = yousefzahrieh17@gmail.com
 description = A comprehensive tools to inspect Python packages and Python installations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yousefabuz17/PkgInspect
 download_url = https://github.com/yousefabuz17/PkgInspect.git
```

### Comparing `pkg_inspect-0.1.0/src/pkg_inspect/pkg_functions/functions.py` & `pkg_inspect-0.1.1/src/pkg_inspect/pkg_functions/functions.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.0/src/pkg_inspect/pkg_modules/pkg_inspect.py` & `pkg_inspect-0.1.1/src/pkg_inspect/pkg_modules/pkg_inspect.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.0/src/pkg_inspect/pkg_modules/pkg_metrics.py` & `pkg_inspect-0.1.1/src/pkg_inspect/pkg_modules/pkg_metrics.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.0/src/pkg_inspect/pkg_modules/pkg_versions.py` & `pkg_inspect-0.1.1/src/pkg_inspect/pkg_modules/pkg_versions.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.0/src/pkg_inspect/pkg_utils/exception.py` & `pkg_inspect-0.1.1/src/pkg_inspect/pkg_utils/exception.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.0/src/pkg_inspect/pkg_utils/util_types.py` & `pkg_inspect-0.1.1/src/pkg_inspect/pkg_utils/util_types.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.0/src/pkg_inspect/pkg_utils/utils.py` & `pkg_inspect-0.1.1/src/pkg_inspect/pkg_utils/utils.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.0/src/pkg_inspect.egg-info/PKG-INFO` & `pkg_inspect-0.1.1/src/pkg_inspect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-inspect
-Version: 0.1.0
+Version: 0.1.1
 Summary: A comprehensive tools to inspect Python packages and Python installations.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.1.0/src/pkg_inspect.egg-info/SOURCES.txt` & `pkg_inspect-0.1.1/src/pkg_inspect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.0/tests/test_pipinspect.py` & `pkg_inspect-0.1.1/tests/test_pipinspect.py`

 * *Files identical despite different names*

