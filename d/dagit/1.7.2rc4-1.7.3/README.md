# Comparing `tmp/dagit-1.7.2rc4.tar.gz` & `tmp/dagit-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagit-1.7.2rc4.tar", last modified: Fri Apr 19 18:02:36 2024, max compression
+gzip compressed data, was "dagit-1.7.3.tar", last modified: Thu Apr 25 20:09:12 2024, max compression
```

## Comparing `dagit-1.7.2rc4.tar` & `dagit-1.7.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:36.173881 dagit-1.7.2rc4/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-19 18:01:50.000000 dagit-1.7.2rc4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-19 18:01:50.000000 dagit-1.7.2rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      920 2024-04-19 18:02:36.173881 dagit-1.7.2rc4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2024-04-19 18:01:50.000000 dagit-1.7.2rc4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:36.169881 dagit-1.7.2rc4/dagit/
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-19 18:01:50.000000 dagit-1.7.2rc4/dagit/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-19 18:01:50.000000 dagit-1.7.2rc4/dagit/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:36.173881 dagit-1.7.2rc4/dagit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      920 2024-04-19 18:02:35.000000 dagit-1.7.2rc4/dagit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      260 2024-04-19 18:02:36.000000 dagit-1.7.2rc4/dagit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:02:35.000000 dagit-1.7.2rc4/dagit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-19 18:02:35.000000 dagit-1.7.2rc4/dagit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      120 2024-04-19 18:02:35.000000 dagit-1.7.2rc4/dagit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-19 18:02:35.000000 dagit-1.7.2rc4/dagit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      153 2024-04-19 18:02:36.173881 dagit-1.7.2rc4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1822 2024-04-19 18:01:50.000000 dagit-1.7.2rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:12.764123 dagit-1.7.3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagit-1.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-25 20:08:31.000000 dagit-1.7.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      917 2024-04-25 20:09:12.764123 dagit-1.7.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2024-04-25 20:08:31.000000 dagit-1.7.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:12.764123 dagit-1.7.3/dagit/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-25 20:08:31.000000 dagit-1.7.3/dagit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-25 20:08:31.000000 dagit-1.7.3/dagit/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:09:12.764123 dagit-1.7.3/dagit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      917 2024-04-25 20:09:12.000000 dagit-1.7.3/dagit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      260 2024-04-25 20:09:12.000000 dagit-1.7.3/dagit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:09:12.000000 dagit-1.7.3/dagit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-25 20:09:12.000000 dagit-1.7.3/dagit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-25 20:09:12.000000 dagit-1.7.3/dagit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-25 20:09:12.000000 dagit-1.7.3/dagit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      153 2024-04-25 20:09:12.768123 dagit-1.7.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1819 2024-04-25 20:08:31.000000 dagit-1.7.3/setup.py
```

### Comparing `dagit-1.7.2rc4/LICENSE` & `dagit-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagit-1.7.2rc4/PKG-INFO` & `dagit-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagit
-Version: 1.7.2rc4
+Version: 1.7.3
 Summary: Web UI for dagster.
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagit-1.7.2rc4/dagit.egg-info/PKG-INFO` & `dagit-1.7.3/dagit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagit
-Version: 1.7.2rc4
+Version: 1.7.3
 Summary: Web UI for dagster.
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagit-1.7.2rc4/setup.py` & `dagit-1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagit_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster-webserver==1.7.2rc4",
+        "dagster-webserver==1.7.3",
     ],
     extras_require={
         "notebook": [f"dagster-webserver[notebook]{pin}"],  # notebooks support
         "test": [f"dagster-webserver[test]{pin}"],  # TestClient deps in full
     },
     entry_points={
         "console_scripts": [
```

