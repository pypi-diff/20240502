# Comparing `tmp/automvs-0.0.7.post1.tar.gz` & `tmp/automvs-0.0.7.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automvs-0.0.7.post1.tar", last modified: Wed May  1 17:16:44 2024, max compression
+gzip compressed data, was "automvs-0.0.7.post2.tar", last modified: Wed May  1 20:24:20 2024, max compression
```

## Comparing `automvs-0.0.7.post1.tar` & `automvs-0.0.7.post2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 17:16:44.638017 automvs-0.0.7.post1/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.7.post1/LICENSE
--rw-r--r--   0 phil      (1000) phil      (1000)     1436 2024-05-01 17:16:44.638017 automvs-0.0.7.post1/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.7.post1/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 17:16:44.634017 automvs-0.0.7.post1/automvs/
--rw-rw-r--   0 phil      (1000) phil      (1000)    19910 2024-05-01 17:16:36.000000 automvs-0.0.7.post1/automvs/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 17:16:44.634017 automvs-0.0.7.post1/automvs.egg-info/
--rw-r--r--   0 phil      (1000) phil      (1000)     1436 2024-05-01 17:16:44.000000 automvs-0.0.7.post1/automvs.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-01 17:16:44.000000 automvs-0.0.7.post1/automvs.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-01 17:16:44.000000 automvs-0.0.7.post1/automvs.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-01 17:16:44.000000 automvs-0.0.7.post1/automvs.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-01 17:16:44.638017 automvs-0.0.7.post1/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      783 2024-05-01 17:16:20.000000 automvs-0.0.7.post1/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 20:24:20.378388 automvs-0.0.7.post2/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.7.post2/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     1436 2024-05-01 20:24:20.378388 automvs-0.0.7.post2/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.7.post2/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 20:24:20.378388 automvs-0.0.7.post2/automvs/
+-rw-rw-r--   0 phil      (1000) phil      (1000)    19900 2024-05-01 20:24:12.000000 automvs-0.0.7.post2/automvs/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 20:24:20.378388 automvs-0.0.7.post2/automvs.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1436 2024-05-01 20:24:20.000000 automvs-0.0.7.post2/automvs.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-01 20:24:20.000000 automvs-0.0.7.post2/automvs.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-01 20:24:20.000000 automvs-0.0.7.post2/automvs.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-01 20:24:20.000000 automvs-0.0.7.post2/automvs.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-01 20:24:20.378388 automvs-0.0.7.post2/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)      783 2024-05-01 20:24:12.000000 automvs-0.0.7.post2/setup.py
```

### Comparing `automvs-0.0.7.post1/LICENSE` & `automvs-0.0.7.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `automvs-0.0.7.post1/PKG-INFO` & `automvs-0.0.7.post2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.7.post1
+Version: 0.0.7.post2
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.7.post1/README.md` & `automvs-0.0.7.post2/README.md`

 * *Files identical despite different names*

### Comparing `automvs-0.0.7.post1/automvs/__init__.py` & `automvs-0.0.7.post2/automvs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     This library allows the use of MVS/CE in an automated fashion. This can
     be used for deploying XMI files, pushing out updates, building software,
     creating custom MVS deployments.
 
     Using this library requires a recent version of hercules SDL and MVS/CE.
 """
 
-__version__ = '0.0.7-1'
+__version__ = '0.0.7-2'
 __author__ = 'Philip Young'
 __license__ = "GPL"
 
 # Copyright (c) 2021, Philip Young
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
@@ -350,16 +350,16 @@
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
                     universal_newlines=True)
         reset_herc_event.clear()
         quit_herc_event.clear()
         self.start_threads()
 
-        self.rc = self.hercproc.poll()
-        if self.rc is not None:
+        rc = self.hercproc.poll()
+        if rc is not None:
             raise("[AUTOMATION] Unable to start hercules")
         self.logger.debug("[AUTOMATION] Hercules launched")
         #self.write_logs()
         self.logger.debug("[AUTOMATION] Hercules Re-initialization Complete")
 
 
     def quit_hercules(self, msg=True):
```

### Comparing `automvs-0.0.7.post1/automvs.egg-info/PKG-INFO` & `automvs-0.0.7.post2/automvs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.7.post1
+Version: 0.0.7.post2
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.7.post1/setup.py` & `automvs-0.0.7.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
     name='automvs',
-    version='0.0.7-1',    
+    version='0.0.7-2',    
     description='Python library for MVS/CE automation',
     url='https://github.com/MVS-sysgen/automvs',
     author='Philip Young',
     author_email='mainframed767@gmail.com',
     license='MIT',
     packages=['automvs'],
     install_requires=[],
```

