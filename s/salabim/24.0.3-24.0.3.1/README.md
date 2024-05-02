# Comparing `tmp/salabim-24.0.3.tar.gz` & `tmp/salabim-24.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salabim-24.0.3.tar", last modified: Wed May  1 16:03:34 2024, max compression
+gzip compressed data, was "salabim-24.0.3.1.tar", last modified: Thu May  2 13:48:13 2024, max compression
```

## Comparing `salabim-24.0.3.tar` & `salabim-24.0.3.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 16:03:34.317685 salabim-24.0.3/
--rw-rw-rw-   0        0        0     3045 2024-05-01 16:03:34.317685 salabim-24.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2522 2024-04-28 16:58:56.000000 salabim-24.0.3/README.md
--rw-rw-rw-   0        0        0      729 2024-05-01 16:03:29.000000 salabim-24.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-01 16:03:34.284834 salabim-24.0.3/salabim/
--rw-rw-rw-   0        0        0   335068 2018-11-08 08:44:44.000000 salabim-24.0.3/salabim/DejaVuSansMono.ttf
--rw-rw-rw-   0        0        0  1330156 2023-05-08 05:21:17.000000 salabim-24.0.3/salabim/calibri.ttf
--rw-rw-rw-   0        0        0   289812 2018-11-08 08:44:33.000000 salabim-24.0.3/salabim/mplus-1m-regular.ttf
--rw-rw-rw-   0        0        0  1093612 2024-05-01 16:03:16.000000 salabim-24.0.3/salabim/salabim.py
-drwxrwxrwx   0        0        0        0 2024-05-01 16:03:34.317685 salabim-24.0.3/salabim.egg-info/
--rw-rw-rw-   0        0        0     3045 2024-05-01 16:03:34.000000 salabim-24.0.3/salabim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2024-05-01 16:03:34.000000 salabim-24.0.3/salabim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 16:03:34.000000 salabim-24.0.3/salabim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-01 16:03:34.000000 salabim-24.0.3/salabim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 16:03:34.317685 salabim-24.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 16:03:34.316282 salabim-24.0.3/tests/
--rw-rw-rw-   0        0        0      677 2023-10-05 13:11:47.000000 salabim-24.0.3/tests/test_cap_now.py
--rw-rw-rw-   0        0        0     6228 2023-05-14 06:16:09.000000 salabim-24.0.3/tests/test_componentgenerator.py
--rw-rw-rw-   0        0        0     2993 2023-08-16 15:40:02.000000 salabim-24.0.3/tests/test_datetime.py
--rw-rw-rw-   0        0        0     6295 2023-03-08 18:04:01.000000 salabim-24.0.3/tests/test_distributions.py
--rw-rw-rw-   0        0        0     1693 2023-07-02 09:23:01.000000 salabim-24.0.3/tests/test_misc.py
--rw-rw-rw-   0        0        0    21231 2023-10-05 13:15:36.000000 salabim-24.0.3/tests/test_monitor.py
--rw-rw-rw-   0        0        0      654 2020-10-22 20:12:03.000000 salabim-24.0.3/tests/test_process.py
--rw-rw-rw-   0        0        0     5060 2021-11-17 08:19:40.000000 salabim-24.0.3/tests/test_queue.py
--rw-rw-rw-   0        0        0       74 2023-07-02 10:54:17.000000 salabim-24.0.3/tests/test_salabim.py
--rw-rw-rw-   0        0        0     2677 2023-08-14 09:14:44.000000 salabim-24.0.3/tests/test_state.py
--rw-rw-rw-   0        0        0      344 2023-11-29 17:46:13.000000 salabim-24.0.3/tests/test_store.py
--rw-rw-rw-   0        0        0     4517 2022-04-30 07:30:12.000000 salabim-24.0.3/tests/test_timeunit.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:48:13.879714 salabim-24.0.3.1/
+-rw-rw-rw-   0        0        0     3047 2024-05-02 13:48:13.878715 salabim-24.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2522 2024-04-28 16:58:56.000000 salabim-24.0.3.1/README.md
+-rw-rw-rw-   0        0        0      740 2024-05-02 13:48:08.000000 salabim-24.0.3.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-02 13:48:13.848389 salabim-24.0.3.1/salabim/
+-rw-rw-rw-   0        0        0   335068 2018-11-08 08:44:44.000000 salabim-24.0.3.1/salabim/DejaVuSansMono.ttf
+-rw-rw-rw-   0        0        0     1105 2024-03-23 13:29:56.000000 salabim-24.0.3.1/salabim/LICENSE.txt
+-rw-rw-rw-   0        0        0  1330156 2023-05-08 05:21:17.000000 salabim-24.0.3.1/salabim/calibri.ttf
+-rw-rw-rw-   0        0        0   294265 2024-05-01 15:58:03.000000 salabim-24.0.3.1/salabim/changelog.txt
+-rw-rw-rw-   0        0        0   289812 2018-11-08 08:44:33.000000 salabim-24.0.3.1/salabim/mplus-1m-regular.ttf
+-rw-rw-rw-   0        0        0  1093612 2024-05-01 16:03:16.000000 salabim-24.0.3.1/salabim/salabim.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:48:13.877714 salabim-24.0.3.1/salabim.egg-info/
+-rw-rw-rw-   0        0        0     3047 2024-05-02 13:48:13.000000 salabim-24.0.3.1/salabim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2024-05-02 13:48:13.000000 salabim-24.0.3.1/salabim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 13:48:13.000000 salabim-24.0.3.1/salabim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 13:48:13.000000 salabim-24.0.3.1/salabim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 13:48:13.880820 salabim-24.0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 13:48:13.875429 salabim-24.0.3.1/tests/
+-rw-rw-rw-   0        0        0      677 2023-10-05 13:11:47.000000 salabim-24.0.3.1/tests/test_cap_now.py
+-rw-rw-rw-   0        0        0     6228 2023-05-14 06:16:09.000000 salabim-24.0.3.1/tests/test_componentgenerator.py
+-rw-rw-rw-   0        0        0     2993 2023-08-16 15:40:02.000000 salabim-24.0.3.1/tests/test_datetime.py
+-rw-rw-rw-   0        0        0     6295 2023-03-08 18:04:01.000000 salabim-24.0.3.1/tests/test_distributions.py
+-rw-rw-rw-   0        0        0     1693 2023-07-02 09:23:01.000000 salabim-24.0.3.1/tests/test_misc.py
+-rw-rw-rw-   0        0        0    21231 2023-10-05 13:15:36.000000 salabim-24.0.3.1/tests/test_monitor.py
+-rw-rw-rw-   0        0        0      654 2020-10-22 20:12:03.000000 salabim-24.0.3.1/tests/test_process.py
+-rw-rw-rw-   0        0        0     5060 2021-11-17 08:19:40.000000 salabim-24.0.3.1/tests/test_queue.py
+-rw-rw-rw-   0        0        0       74 2023-07-02 10:54:17.000000 salabim-24.0.3.1/tests/test_salabim.py
+-rw-rw-rw-   0        0        0     2677 2023-08-14 09:14:44.000000 salabim-24.0.3.1/tests/test_state.py
+-rw-rw-rw-   0        0        0      344 2023-11-29 17:46:13.000000 salabim-24.0.3.1/tests/test_store.py
+-rw-rw-rw-   0        0        0     4517 2022-04-30 07:30:12.000000 salabim-24.0.3.1/tests/test_timeunit.py
```

### Comparing `salabim-24.0.3/PKG-INFO` & `salabim-24.0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salabim
-Version: 24.0.3
+Version: 24.0.3.1
 Summary: salabim - discrete event simulation in Python
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/salabim
 Project-URL: Repository, https://github.com/salabim/salabim
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `salabim-24.0.3/README.md` & `salabim-24.0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/pyproject.toml` & `salabim-24.0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "salabim"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "salabim - discrete event simulation in Python"
-version = "24.0.3"
+version = "24.0.3.1"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
@@ -23,8 +23,8 @@
 Repository = "https://github.com/salabim/salabim"
 
 
 [tool.setuptools]
 packages = ["salabim"]
 
 [tool.setuptools.package-data]
-"*" = ["*.ttf"]
+"*" = ["*.ttf", "*.txt"]
```

### Comparing `salabim-24.0.3/salabim/DejaVuSansMono.ttf` & `salabim-24.0.3.1/salabim/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/salabim/calibri.ttf` & `salabim-24.0.3.1/salabim/calibri.ttf`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/salabim/mplus-1m-regular.ttf` & `salabim-24.0.3.1/salabim/mplus-1m-regular.ttf`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/salabim/salabim.py` & `salabim-24.0.3.1/salabim/salabim.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/salabim.egg-info/PKG-INFO` & `salabim-24.0.3.1/salabim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salabim
-Version: 24.0.3
+Version: 24.0.3.1
 Summary: salabim - discrete event simulation in Python
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/salabim
 Project-URL: Repository, https://github.com/salabim/salabim
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `salabim-24.0.3/salabim.egg-info/SOURCES.txt` & `salabim-24.0.3.1/salabim.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 README.md
 pyproject.toml
 salabim/DejaVuSansMono.ttf
+salabim/LICENSE.txt
 salabim/calibri.ttf
+salabim/changelog.txt
 salabim/mplus-1m-regular.ttf
 salabim/salabim.py
 salabim.egg-info/PKG-INFO
 salabim.egg-info/SOURCES.txt
 salabim.egg-info/dependency_links.txt
 salabim.egg-info/top_level.txt
 tests/test_cap_now.py
```

### Comparing `salabim-24.0.3/tests/test_cap_now.py` & `salabim-24.0.3.1/tests/test_cap_now.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/tests/test_componentgenerator.py` & `salabim-24.0.3.1/tests/test_componentgenerator.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/tests/test_datetime.py` & `salabim-24.0.3.1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/tests/test_distributions.py` & `salabim-24.0.3.1/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/tests/test_misc.py` & `salabim-24.0.3.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/tests/test_monitor.py` & `salabim-24.0.3.1/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/tests/test_process.py` & `salabim-24.0.3.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/tests/test_queue.py` & `salabim-24.0.3.1/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/tests/test_state.py` & `salabim-24.0.3.1/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.3/tests/test_timeunit.py` & `salabim-24.0.3.1/tests/test_timeunit.py`

 * *Files identical despite different names*

