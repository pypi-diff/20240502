# Comparing `tmp/nightingalejsonadapter-1.2.0.tar.gz` & `tmp/nightingalejsonadapter-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nightingalejsonadapter-1.2.0.tar", last modified: Mon Apr 10 14:33:10 2023, max compression
+gzip compressed data, was "nightingalejsonadapter-2.1.0.tar", last modified: Thu May  2 15:31:34 2024, max compression
```

## Comparing `nightingalejsonadapter-1.2.0.tar` & `nightingalejsonadapter-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-10 14:33:10.436648 nightingalejsonadapter-1.2.0/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      246 2023-04-10 14:33:10.436648 nightingalejsonadapter-1.2.0/PKG-INFO
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-10 14:33:10.436648 nightingalejsonadapter-1.2.0/nightingalejsonadapter/
--rw-r--r--   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:22:01.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/__init__.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      452 2023-04-05 17:04:25.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/intervention_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      560 2023-04-03 16:31:02.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/patient_info_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      516 2023-03-15 15:22:55.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/uuid_generator.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      622 2023-04-05 17:04:56.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/vital_kafka_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      601 2023-04-05 17:04:40.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/vitals_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)     1180 2023-04-05 17:05:24.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/vitals_response.py
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-10 14:33:10.436648 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      246 2023-04-10 14:33:10.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/PKG-INFO
--rw-r--r--   0 nuno      (1000) nuno      (1000)      536 2023-04-10 14:33:10.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/SOURCES.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        1 2023-04-10 14:33:10.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/dependency_links.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        9 2023-04-10 14:33:10.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/requires.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       23 2023-04-10 14:33:10.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/top_level.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       38 2023-04-10 14:33:10.436648 nightingalejsonadapter-1.2.0/setup.cfg
--rw-r--r--   0 nuno      (1000) nuno      (1000)      715 2023-04-05 17:01:48.000000 nightingalejsonadapter-1.2.0/setup.py
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-02 15:31:34.713131 nightingalejsonadapter-2.1.0/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-02 15:31:34.713131 nightingalejsonadapter-2.1.0/PKG-INFO
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-02 15:31:34.709797 nightingalejsonadapter-2.1.0/nightingalejsonadapter/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:22:01.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/__init__.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      452 2023-04-05 17:04:25.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/intervention_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      560 2023-04-03 16:31:02.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/patient_info_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      434 2024-05-02 14:49:08.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/trigger_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      516 2023-03-15 15:22:55.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/uuid_generator.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      622 2023-04-05 17:04:56.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/vital_kafka_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      601 2023-04-05 17:04:40.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/vitals_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)     1180 2023-04-05 17:05:24.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/vitals_response.py
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-02 15:31:34.713131 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-02 15:31:34.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/PKG-INFO
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      578 2024-05-02 15:31:34.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/SOURCES.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        1 2024-05-02 15:31:34.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/dependency_links.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        9 2024-05-02 15:31:34.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/requires.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)       23 2024-05-02 15:31:34.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/top_level.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)       38 2024-05-02 15:31:34.713131 nightingalejsonadapter-2.1.0/setup.cfg
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      774 2024-05-02 14:50:05.000000 nightingalejsonadapter-2.1.0/setup.py
```

### Comparing `nightingalejsonadapter-1.2.0/nightingalejsonadapter/patient_info_adapter.py` & `nightingalejsonadapter-2.1.0/nightingalejsonadapter/patient_info_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-1.2.0/nightingalejsonadapter/uuid_generator.py` & `nightingalejsonadapter-2.1.0/nightingalejsonadapter/uuid_generator.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-1.2.0/nightingalejsonadapter/vital_kafka_adapter.py` & `nightingalejsonadapter-2.1.0/nightingalejsonadapter/vital_kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-1.2.0/nightingalejsonadapter/vitals_adapter.py` & `nightingalejsonadapter-2.1.0/nightingalejsonadapter/vitals_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-1.2.0/nightingalejsonadapter/vitals_response.py` & `nightingalejsonadapter-2.1.0/nightingalejsonadapter/vitals_response.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/SOURCES.txt` & `nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 setup.py
 nightingalejsonadapter/__init__.py
 nightingalejsonadapter/intervention_adapter.py
 nightingalejsonadapter/patient_info_adapter.py
+nightingalejsonadapter/trigger_adapter.py
 nightingalejsonadapter/uuid_generator.py
 nightingalejsonadapter/vital_kafka_adapter.py
 nightingalejsonadapter/vitals_adapter.py
 nightingalejsonadapter/vitals_response.py
 nightingalejsonadapter.egg-info/PKG-INFO
 nightingalejsonadapter.egg-info/SOURCES.txt
 nightingalejsonadapter.egg-info/dependency_links.txt
```

### Comparing `nightingalejsonadapter-1.2.0/setup.py` & `nightingalejsonadapter-2.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.0' 
+VERSION = '2.1.0' 
 DESCRIPTION = 'JSON adapter'
 LONG_DESCRIPTION = 'JSON adapters and validators for Nightingale Communication and Integration'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="nightingalejsonadapter", 
@@ -14,8 +14,11 @@
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         install_requires=['pydantic'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
         keywords=['jsonadapter']
-)
+)
+
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
```

