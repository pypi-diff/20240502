# Comparing `tmp/dagster-managed-elements-0.23.3.tar.gz` & `tmp/dagster-managed-elements-0.23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-managed-elements-0.23.3.tar", last modified: Thu Apr 25 20:21:30 2024, max compression
+gzip compressed data, was "dagster-managed-elements-0.23.4.tar", last modified: Thu May  2 20:43:52 2024, max compression
```

## Comparing `dagster-managed-elements-0.23.3.tar` & `dagster-managed-elements-0.23.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:30.665511 dagster-managed-elements-0.23.3/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-managed-elements-0.23.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-25 20:08:31.000000 dagster-managed-elements-0.23.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      723 2024-04-25 20:21:30.665511 dagster-managed-elements-0.23.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-25 20:08:31.000000 dagster-managed-elements-0.23.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:30.661511 dagster-managed-elements-0.23.3/dagster_managed_elements/
--rw-r--r--   0 root         (0) root         (0)      202 2024-04-25 20:08:31.000000 dagster-managed-elements-0.23.3/dagster_managed_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6241 2024-04-25 20:08:31.000000 dagster-managed-elements-0.23.3/dagster_managed_elements/cli.py
--rw-r--r--   0 root         (0) root         (0)     9608 2024-04-25 20:08:31.000000 dagster-managed-elements-0.23.3/dagster_managed_elements/types.py
--rw-r--r--   0 root         (0) root         (0)     3357 2024-04-25 20:08:31.000000 dagster-managed-elements-0.23.3/dagster_managed_elements/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-25 20:08:31.000000 dagster-managed-elements-0.23.3/dagster_managed_elements/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:30.665511 dagster-managed-elements-0.23.3/dagster_managed_elements.egg-info/
--rw-r--r--   0 root         (0) root         (0)      723 2024-04-25 20:21:30.000000 dagster-managed-elements-0.23.3/dagster_managed_elements.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      558 2024-04-25 20:21:30.000000 dagster-managed-elements-0.23.3/dagster_managed_elements.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:21:30.000000 dagster-managed-elements-0.23.3/dagster_managed_elements.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      126 2024-04-25 20:21:30.000000 dagster-managed-elements-0.23.3/dagster_managed_elements.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:21:30.000000 dagster-managed-elements-0.23.3/dagster_managed_elements.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 20:21:30.000000 dagster-managed-elements-0.23.3/dagster_managed_elements.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 20:21:30.000000 dagster-managed-elements-0.23.3/dagster_managed_elements.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2024-04-25 20:21:30.665511 dagster-managed-elements-0.23.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1561 2024-04-25 20:08:31.000000 dagster-managed-elements-0.23.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:52.082811 dagster-managed-elements-0.23.4/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:41.000000 dagster-managed-elements-0.23.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-02 20:31:41.000000 dagster-managed-elements-0.23.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      723 2024-05-02 20:43:52.082811 dagster-managed-elements-0.23.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2024-05-02 20:31:41.000000 dagster-managed-elements-0.23.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:52.082811 dagster-managed-elements-0.23.4/dagster_managed_elements/
+-rw-r--r--   0 root         (0) root         (0)      202 2024-05-02 20:31:41.000000 dagster-managed-elements-0.23.4/dagster_managed_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6241 2024-05-02 20:31:41.000000 dagster-managed-elements-0.23.4/dagster_managed_elements/cli.py
+-rw-r--r--   0 root         (0) root         (0)     9608 2024-05-02 20:31:41.000000 dagster-managed-elements-0.23.4/dagster_managed_elements/types.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2024-05-02 20:31:41.000000 dagster-managed-elements-0.23.4/dagster_managed_elements/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-managed-elements-0.23.4/dagster_managed_elements/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:43:52.082811 dagster-managed-elements-0.23.4/dagster_managed_elements.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      723 2024-05-02 20:43:51.000000 dagster-managed-elements-0.23.4/dagster_managed_elements.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-02 20:43:51.000000 dagster-managed-elements-0.23.4/dagster_managed_elements.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:43:51.000000 dagster-managed-elements-0.23.4/dagster_managed_elements.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2024-05-02 20:43:51.000000 dagster-managed-elements-0.23.4/dagster_managed_elements.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:43:51.000000 dagster-managed-elements-0.23.4/dagster_managed_elements.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 20:43:51.000000 dagster-managed-elements-0.23.4/dagster_managed_elements.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-02 20:43:51.000000 dagster-managed-elements-0.23.4/dagster_managed_elements.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-02 20:43:52.086811 dagster-managed-elements-0.23.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1561 2024-05-02 20:31:41.000000 dagster-managed-elements-0.23.4/setup.py
```

### Comparing `dagster-managed-elements-0.23.3/LICENSE` & `dagster-managed-elements-0.23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.23.3/PKG-INFO` & `dagster-managed-elements-0.23.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.23.3
+Version: 0.23.4
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-managed-elements-0.23.3/dagster_managed_elements/cli.py` & `dagster-managed-elements-0.23.4/dagster_managed_elements/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.23.3/dagster_managed_elements/types.py` & `dagster-managed-elements-0.23.4/dagster_managed_elements/types.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.23.3/dagster_managed_elements/utils.py` & `dagster-managed-elements-0.23.4/dagster_managed_elements/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.23.3/dagster_managed_elements.egg-info/PKG-INFO` & `dagster-managed-elements-0.23.4/dagster_managed_elements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.23.3
+Version: 0.23.4
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-managed-elements-0.23.3/dagster_managed_elements.egg-info/SOURCES.txt` & `dagster-managed-elements-0.23.4/dagster_managed_elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.23.3/setup.py` & `dagster-managed-elements-0.23.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_managed_elements_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.3", "requests", "click_spinner"],
+    install_requires=["dagster==1.7.4", "requests", "click_spinner"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-managed-elements = dagster_managed_elements.cli:main",
             "dagster-me = dagster_managed_elements.cli:main",
         ]
     },
```

