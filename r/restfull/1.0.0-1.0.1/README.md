# Comparing `tmp/restfull-1.0.0.tar.gz` & `tmp/restfull-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restfull-1.0.0.tar", last modified: Wed May  1 23:07:13 2024, max compression
+gzip compressed data, was "restfull-1.0.1.tar", last modified: Thu May  2 16:24:13 2024, max compression
```

## Comparing `restfull-1.0.0.tar` & `restfull-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-01 23:07:13.093825 restfull-1.0.0/
--rw-r--r--   0 michael    (501) staff       (20)      294 2024-05-01 23:01:08.000000 restfull-1.0.0/.bumpversion.cfg
--rw-r--r--   0 michael    (501) staff       (20)     3125 2024-05-01 21:50:19.000000 restfull-1.0.0/.gitignore
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-01 23:07:13.086540 restfull-1.0.0/.idea/
--rw-r--r--   0 michael    (501) staff       (20)      176 2024-05-01 15:13:54.000000 restfull-1.0.0/.idea/.gitignore
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-01 23:07:13.087151 restfull-1.0.0/.idea/inspectionProfiles/
--rw-r--r--   0 michael    (501) staff       (20)     4768 2024-05-01 15:13:54.000000 restfull-1.0.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 michael    (501) staff       (20)      174 2024-05-01 15:13:55.000000 restfull-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 michael    (501) staff       (20)      298 2024-05-01 15:21:37.000000 restfull-1.0.0/.idea/misc.xml
--rw-r--r--   0 michael    (501) staff       (20)      268 2024-05-01 15:13:55.000000 restfull-1.0.0/.idea/modules.xml
--rw-r--r--   0 michael    (501) staff       (20)      353 2024-05-01 15:13:55.000000 restfull-1.0.0/.idea/restfull.iml
--rw-r--r--   0 michael    (501) staff       (20)      180 2024-05-01 15:13:55.000000 restfull-1.0.0/.idea/vcs.xml
--rw-r--r--   0 michael    (501) staff       (20)     1074 2024-05-01 21:53:55.000000 restfull-1.0.0/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)      571 2024-05-01 21:46:50.000000 restfull-1.0.0/Makefile
--rw-r--r--   0 michael    (501) staff       (20)      988 2024-05-01 23:07:13.091302 restfull-1.0.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)       67 2024-05-01 21:48:49.000000 restfull-1.0.0/README.md
--rw-r--r--   0 michael    (501) staff       (20)        6 2024-05-01 21:47:32.000000 restfull-1.0.0/VERSION
--rw-r--r--   0 michael    (501) staff       (20)      133 2024-05-01 21:34:39.000000 restfull-1.0.0/requirements.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-01 23:07:13.088853 restfull-1.0.0/restfull/
--rw-r--r--   0 michael    (501) staff       (20)      161 2024-05-01 21:47:14.000000 restfull-1.0.0/restfull/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      256 2024-05-01 19:04:43.000000 restfull-1.0.0/restfull/base_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      632 2024-05-01 19:04:43.000000 restfull-1.0.0/restfull/basic_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      417 2024-05-01 19:04:43.000000 restfull-1.0.0/restfull/bearer_auth.py
--rw-r--r--   0 michael    (501) staff       (20)      689 2024-05-01 19:56:28.000000 restfull-1.0.0/restfull/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)     8123 2024-05-01 22:52:39.000000 restfull-1.0.0/restfull/restapi.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-01 23:07:13.089903 restfull-1.0.0/restfull.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)      988 2024-05-01 23:07:13.000000 restfull-1.0.0/restfull.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      628 2024-05-01 23:07:13.000000 restfull-1.0.0/restfull.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2024-05-01 23:07:13.000000 restfull-1.0.0/restfull.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       96 2024-05-01 23:07:13.000000 restfull-1.0.0/restfull.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2024-05-01 23:07:13.000000 restfull-1.0.0/restfull.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2024-05-01 23:07:13.093869 restfull-1.0.0/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1274 2024-05-01 22:59:33.000000 restfull-1.0.0/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-01 23:07:13.090944 restfull-1.0.0/tests/
--rw-r--r--   0 michael    (501) staff       (20)        0 2024-05-01 21:30:18.000000 restfull-1.0.0/tests/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      535 2024-05-01 21:30:54.000000 restfull-1.0.0/tests/conftest.py
--rw-r--r--   0 michael    (501) staff       (20)      101 2024-05-01 21:31:14.000000 restfull-1.0.0/tests/pytest.ini
--rw-r--r--   0 michael    (501) staff       (20)     4087 2024-05-01 22:56:21.000000 restfull-1.0.0/tests/test_1.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.782671 restfull-1.0.1/
+-rw-r--r--   0 michael    (501) staff       (20)      293 2024-05-02 16:23:20.000000 restfull-1.0.1/.bumpversion.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     3125 2024-05-01 21:50:19.000000 restfull-1.0.1/.gitignore
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.776410 restfull-1.0.1/.idea/
+-rw-r--r--   0 michael    (501) staff       (20)      176 2024-05-01 15:13:54.000000 restfull-1.0.1/.idea/.gitignore
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.777125 restfull-1.0.1/.idea/inspectionProfiles/
+-rw-r--r--   0 michael    (501) staff       (20)     4768 2024-05-01 15:13:54.000000 restfull-1.0.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 michael    (501) staff       (20)      174 2024-05-01 15:13:55.000000 restfull-1.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 michael    (501) staff       (20)      298 2024-05-01 15:21:37.000000 restfull-1.0.1/.idea/misc.xml
+-rw-r--r--   0 michael    (501) staff       (20)      268 2024-05-01 15:13:55.000000 restfull-1.0.1/.idea/modules.xml
+-rw-r--r--   0 michael    (501) staff       (20)      353 2024-05-01 15:13:55.000000 restfull-1.0.1/.idea/restfull.iml
+-rw-r--r--   0 michael    (501) staff       (20)      180 2024-05-01 15:13:55.000000 restfull-1.0.1/.idea/vcs.xml
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2024-05-01 21:53:55.000000 restfull-1.0.1/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)      571 2024-05-01 21:46:50.000000 restfull-1.0.1/Makefile
+-rw-r--r--   0 michael    (501) staff       (20)      988 2024-05-02 16:24:13.781903 restfull-1.0.1/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)       67 2024-05-02 16:23:20.000000 restfull-1.0.1/README.md
+-rw-r--r--   0 michael    (501) staff       (20)        6 2024-05-02 16:23:20.000000 restfull-1.0.1/VERSION
+-rw-r--r--   0 michael    (501) staff       (20)      133 2024-05-01 21:34:39.000000 restfull-1.0.1/requirements.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.779194 restfull-1.0.1/restfull/
+-rw-r--r--   0 michael    (501) staff       (20)      161 2024-05-02 16:23:20.000000 restfull-1.0.1/restfull/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      256 2024-05-01 19:04:43.000000 restfull-1.0.1/restfull/base_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      632 2024-05-01 19:04:43.000000 restfull-1.0.1/restfull/basic_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      416 2024-05-02 16:18:39.000000 restfull-1.0.1/restfull/bearer_auth.py
+-rw-r--r--   0 michael    (501) staff       (20)      689 2024-05-01 19:56:28.000000 restfull-1.0.1/restfull/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)     8123 2024-05-01 22:52:39.000000 restfull-1.0.1/restfull/restapi.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.780223 restfull-1.0.1/restfull.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)      988 2024-05-02 16:24:13.000000 restfull-1.0.1/restfull.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      628 2024-05-02 16:24:13.000000 restfull-1.0.1/restfull.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2024-05-02 16:24:13.000000 restfull-1.0.1/restfull.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       96 2024-05-02 16:24:13.000000 restfull-1.0.1/restfull.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2024-05-02 16:24:13.000000 restfull-1.0.1/restfull.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2024-05-02 16:24:13.782734 restfull-1.0.1/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1274 2024-05-01 22:59:33.000000 restfull-1.0.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-02 16:24:13.781484 restfull-1.0.1/tests/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2024-05-01 21:30:18.000000 restfull-1.0.1/tests/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      535 2024-05-01 21:30:54.000000 restfull-1.0.1/tests/conftest.py
+-rw-r--r--   0 michael    (501) staff       (20)      101 2024-05-01 21:31:14.000000 restfull-1.0.1/tests/pytest.ini
+-rw-r--r--   0 michael    (501) staff       (20)     4087 2024-05-01 22:56:21.000000 restfull-1.0.1/tests/test_1.py
```

### Comparing `restfull-1.0.0/.gitignore` & `restfull-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `restfull-1.0.0/.idea/inspectionProfiles/Project_Default.xml` & `restfull-1.0.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `restfull-1.0.0/LICENSE.txt` & `restfull-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restfull-1.0.0/Makefile` & `restfull-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `restfull-1.0.0/PKG-INFO` & `restfull-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restfull
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python REST API Frontend
 Home-page: https://github.com/mminichino/restfull
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: utilities,rest,api
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,13 +20,13 @@
 License-File: LICENSE.txt
 Requires-Dist: requests>=2.31.0
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: pytoolbase>=1.0.1
 Requires-Dist: python-certifi-win32>=1.6.1
 Requires-Dist: certifi>=2023.5.7
 
-# pytoolbase 1.0.0
+# pytoolbase 1.0.1
 
 ## Installing
 ```
 $ pip install pytoolbase
 ```
```

### Comparing `restfull-1.0.0/restfull/basic_auth.py` & `restfull-1.0.1/restfull/basic_auth.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.0/restfull/exceptions.py` & `restfull-1.0.1/restfull/exceptions.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.0/restfull/restapi.py` & `restfull-1.0.1/restfull/restapi.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.0/restfull.egg-info/PKG-INFO` & `restfull-1.0.1/restfull.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restfull
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python REST API Frontend
 Home-page: https://github.com/mminichino/restfull
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: utilities,rest,api
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,13 +20,13 @@
 License-File: LICENSE.txt
 Requires-Dist: requests>=2.31.0
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: pytoolbase>=1.0.1
 Requires-Dist: python-certifi-win32>=1.6.1
 Requires-Dist: certifi>=2023.5.7
 
-# pytoolbase 1.0.0
+# pytoolbase 1.0.1
 
 ## Installing
 ```
 $ pip install pytoolbase
 ```
```

### Comparing `restfull-1.0.0/restfull.egg-info/SOURCES.txt` & `restfull-1.0.1/restfull.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `restfull-1.0.0/setup.py` & `restfull-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.0/tests/conftest.py` & `restfull-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `restfull-1.0.0/tests/test_1.py` & `restfull-1.0.1/tests/test_1.py`

 * *Files identical despite different names*

