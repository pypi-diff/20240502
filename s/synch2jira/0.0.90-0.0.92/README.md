# Comparing `tmp/synch2jira-0.0.90.tar.gz` & `tmp/synch2jira-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synch2jira-0.0.90.tar", last modified: Mon Mar 11 10:36:28 2024, max compression
+gzip compressed data, was "synch2jira-0.0.92.tar", last modified: Mon Mar 11 10:40:30 2024, max compression
```

## Comparing `synch2jira-0.0.90.tar` & `synch2jira-0.0.92.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 ibtihell  (1000) ibtihell  (1000)        0 2024-03-11 10:36:28.032629 synch2jira-0.0.90/
--rw-r--r--   0 ibtihell  (1000) ibtihell  (1000)     1776 2024-03-11 10:36:28.032629 synch2jira-0.0.90/PKG-INFO
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     1456 2024-03-06 15:15:55.000000 synch2jira-0.0.90/README.md
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)       38 2024-03-11 10:36:28.032629 synch2jira-0.0.90/setup.cfg
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     1490 2024-03-11 10:36:07.000000 synch2jira-0.0.90/setup.py
-drwxrwxr-x   0 ibtihell  (1000) ibtihell  (1000)        0 2024-03-11 10:36:28.032629 synch2jira-0.0.90/synch2jira/
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)        0 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/__init__.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     3015 2024-03-11 10:36:06.000000 synch2jira-0.0.90/synch2jira/config_handler.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      792 2024-03-11 10:36:06.000000 synch2jira-0.0.90/synch2jira/config_package.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      174 2024-03-11 10:36:06.000000 synch2jira-0.0.90/synch2jira/historique.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      495 2024-03-11 10:36:06.000000 synch2jira-0.0.90/synch2jira/implementation_historique.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     2920 2024-03-11 10:36:06.000000 synch2jira-0.0.90/synch2jira/implementation_issue_S1.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)    14925 2024-03-11 10:36:06.000000 synch2jira-0.0.90/synch2jira/implementation_issue_S2.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     2606 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/implementation_issue_S3.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     8419 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/implementation_issue_wokflow.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)       79 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/implementation_status.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      584 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/implementation_synchronisation_S1.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      584 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/implementation_synchronisation_S2.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     2642 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/implementation_table_correpondance_key_id.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     4974 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/issue.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     3476 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/issue_workflow.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      306 2024-03-06 09:47:24.000000 synch2jira-0.0.90/synch2jira/setup_files.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)       55 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/status.py
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     4519 2024-03-11 10:36:07.000000 synch2jira-0.0.90/synch2jira/synchronisation.py
-drwxrwxr-x   0 ibtihell  (1000) ibtihell  (1000)        0 2024-03-11 10:36:28.032629 synch2jira-0.0.90/synch2jira.egg-info/
--rw-r--r--   0 ibtihell  (1000) ibtihell  (1000)     1776 2024-03-11 10:36:28.000000 synch2jira-0.0.90/synch2jira.egg-info/PKG-INFO
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      771 2024-03-11 10:36:28.000000 synch2jira-0.0.90/synch2jira.egg-info/SOURCES.txt
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)        1 2024-03-11 10:36:28.000000 synch2jira-0.0.90/synch2jira.egg-info/dependency_links.txt
--rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)       11 2024-03-11 10:36:28.000000 synch2jira-0.0.90/synch2jira.egg-info/top_level.txt
+drwxrwxr-x   0 ibtihell  (1000) ibtihell  (1000)        0 2024-03-11 10:40:30.906701 synch2jira-0.0.92/
+-rw-r--r--   0 ibtihell  (1000) ibtihell  (1000)     1776 2024-03-11 10:40:30.906701 synch2jira-0.0.92/PKG-INFO
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     1456 2024-03-06 15:15:55.000000 synch2jira-0.0.92/README.md
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)       38 2024-03-11 10:40:30.906701 synch2jira-0.0.92/setup.cfg
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     1490 2024-03-11 10:40:15.000000 synch2jira-0.0.92/setup.py
+drwxrwxr-x   0 ibtihell  (1000) ibtihell  (1000)        0 2024-03-11 10:40:30.906701 synch2jira-0.0.92/synch2jira/
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)        0 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/__init__.py
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     3015 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/config_handler.py
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      792 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/config_package.py
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      174 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/historique.py
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      495 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/historique.pyi
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     4974 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/issue.py
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     2920 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/issue_S1.pyi
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)    14925 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/issue_S2.pyi
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     2606 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/issue_S3.pyi
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     8419 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/issue_wokflow.pyi
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     3476 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/issue_workflow.py
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      306 2024-03-06 09:47:24.000000 synch2jira-0.0.92/synch2jira/setup_files.py
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)       55 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/status.py
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)       79 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/status.pyi
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     4519 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/synch.py
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      584 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/synchronisation_S1.pyi
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      584 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/synchronisation_S2.pyi
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)     2642 2024-03-11 10:40:15.000000 synch2jira-0.0.92/synch2jira/table_correpondance_key_id.pyi
+drwxrwxr-x   0 ibtihell  (1000) ibtihell  (1000)        0 2024-03-11 10:40:30.906701 synch2jira-0.0.92/synch2jira.egg-info/
+-rw-r--r--   0 ibtihell  (1000) ibtihell  (1000)     1776 2024-03-11 10:40:30.000000 synch2jira-0.0.92/synch2jira.egg-info/PKG-INFO
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)      635 2024-03-11 10:40:30.000000 synch2jira-0.0.92/synch2jira.egg-info/SOURCES.txt
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)        1 2024-03-11 10:40:30.000000 synch2jira-0.0.92/synch2jira.egg-info/dependency_links.txt
+-rw-rw-r--   0 ibtihell  (1000) ibtihell  (1000)       11 2024-03-11 10:40:30.000000 synch2jira-0.0.92/synch2jira.egg-info/top_level.txt
```

### Comparing `synch2jira-0.0.90/PKG-INFO` & `synch2jira-0.0.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synch2jira
-Version: 0.0.90
+Version: 0.0.92
 Summary: Lib
 Author: wefine
 Author-email: wefine2529@ebuthor.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `synch2jira-0.0.90/README.md` & `synch2jira-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/setup.py` & `synch2jira-0.0.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="synch2jira",
     # version of the module
-    version="0.0.90",
+    version="0.0.92",
     # Name of Author
     author="wefine",
     # your Email address
     author_email="wefine2529@ebuthor.com",
     # #Small Description about module
     description="Lib",
     # long_description=long_description,
```

### Comparing `synch2jira-0.0.90/synch2jira/config_handler.py` & `synch2jira-0.0.92/synch2jira/config_handler.py`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/config_package.py` & `synch2jira-0.0.92/synch2jira/config_package.py`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/implementation_issue_S1.py` & `synch2jira-0.0.92/synch2jira/issue_S1.pyi`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/implementation_issue_S2.py` & `synch2jira-0.0.92/synch2jira/issue_S2.pyi`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/implementation_issue_S3.py` & `synch2jira-0.0.92/synch2jira/issue_S3.pyi`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/implementation_issue_wokflow.py` & `synch2jira-0.0.92/synch2jira/issue_wokflow.pyi`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/implementation_synchronisation_S1.py` & `synch2jira-0.0.92/synch2jira/synchronisation_S1.pyi`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/implementation_synchronisation_S2.py` & `synch2jira-0.0.92/synch2jira/synchronisation_S2.pyi`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/implementation_table_correpondance_key_id.py` & `synch2jira-0.0.92/synch2jira/table_correpondance_key_id.pyi`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/issue.py` & `synch2jira-0.0.92/synch2jira/issue.py`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/issue_workflow.py` & `synch2jira-0.0.92/synch2jira/issue_workflow.py`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira/synchronisation.py` & `synch2jira-0.0.92/synch2jira/synch.py`

 * *Files identical despite different names*

### Comparing `synch2jira-0.0.90/synch2jira.egg-info/PKG-INFO` & `synch2jira-0.0.92/synch2jira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synch2jira
-Version: 0.0.90
+Version: 0.0.92
 Summary: Lib
 Author: wefine
 Author-email: wefine2529@ebuthor.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

