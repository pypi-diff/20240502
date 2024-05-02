# Comparing `tmp/dagster-embedded-elt-0.23.3.tar.gz` & `tmp/dagster-embedded-elt-0.23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-embedded-elt-0.23.3.tar", last modified: Thu Apr 25 20:20:52 2024, max compression
+gzip compressed data, was "dagster-embedded-elt-0.23.4.tar", last modified: Thu May  2 20:38:04 2024, max compression
```

## Comparing `dagster-embedded-elt-0.23.3.tar` & `dagster-embedded-elt-0.23.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:52.501854 dagster-embedded-elt-0.23.3/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-25 20:20:52.501854 dagster-embedded-elt-0.23.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:52.497854 dagster-embedded-elt-0.23.3/dagster_embedded_elt/
--rw-r--r--   0 root         (0) root         (0)      163 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:52.501854 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/
--rw-r--r--   0 root         (0) root         (0)      270 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3875 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/constants.py
--rw-r--r--   0 root         (0) root         (0)     7033 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/resource.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:52.501854 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4954 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)     8087 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/dagster_sling_translator.py
--rw-r--r--   0 root         (0) root         (0)    17560 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/resources.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/sling_replication.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:52.497854 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      886 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/integration.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2024-04-25 20:20:52.505854 dagster-embedded-elt-0.23.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:38:04.845964 dagster-embedded-elt-0.23.4/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-02 20:38:04.845964 dagster-embedded-elt-0.23.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:38:04.837964 dagster-embedded-elt-0.23.4/dagster_embedded_elt/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:38:04.841964 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:38:04.845964 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4954 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/dagster_sling_translator.py
+-rw-r--r--   0 root         (0) root         (0)    17560 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/sling_replication.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:38:04.837964 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/integration.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2024-05-02 20:38:04.849964 dagster-embedded-elt-0.23.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/setup.py
```

### Comparing `dagster-embedded-elt-0.23.3/LICENSE` & `dagster-embedded-elt-0.23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/asset_decorator.py` & `dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/resource.py` & `dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/translator.py` & `dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/__init__.py` & `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/asset_decorator.py` & `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/asset_defs.py` & `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/dagster_sling_translator.py` & `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/dagster_sling_translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/resources.py` & `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/sling_replication.py` & `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/sling_replication.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/SOURCES.txt` & `dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.3/setup.py` & `dagster-embedded-elt-0.23.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_embedded_elt_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.3", "sling>=1.1.5", "dlt>=0.4"],
+    install_requires=["dagster==1.7.4", "sling>=1.1.5", "dlt>=0.4"],
     zip_safe=False,
     extras_require={
         "test": [
             "duckdb",
         ]
     },
 )
```

