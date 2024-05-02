# Comparing `tmp/bent-0.0.55.tar.gz` & `tmp/bent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bent-0.0.55.tar", last modified: Thu May  2 09:46:04 2024, max compression
+gzip compressed data, was "dist/bent-0.0.9.tar", last modified: Fri Feb  3 19:10:35 2023, max compression
```

## Comparing `bent-0.0.55.tar` & `bent-0.0.9.tar`

### file list

```diff
@@ -1,60 +1,57 @@
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.014741 bent-0.0.55/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    11340 2024-04-29 10:21:28.000000 bent-0.0.55/LICENSE.txt
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)      202 2024-04-29 10:21:28.000000 bent-0.0.55/MANIFEST.in
--rw-r--r--   0 pruas     (1000) pruas     (1000)    18902 2024-05-02 09:46:04.014741 bent-0.0.55/PKG-INFO
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     4055 2024-04-29 10:21:28.000000 bent-0.0.55/README.rst
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.002741 bent-0.0.55/bent/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-04-29 10:21:28.000000 bent-0.0.55/bent/__init__.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    13748 2024-04-30 12:54:08.000000 bent-0.0.55/bent/annotate.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1756 2024-04-29 18:24:03.000000 bent-0.0.55/bent/get_data.sh
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1889 2024-04-30 12:28:07.000000 bent-0.0.55/bent/get_kb_dicts.sh
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1138 2024-04-30 12:31:20.000000 bent-0.0.55/bent/get_kbs.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)      444 2024-04-29 10:21:28.000000 bent-0.0.55/bent/requirements.txt
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     3341 2024-05-02 09:45:41.000000 bent-0.0.55/bent/setup_package.sh
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)      179 2024-04-29 10:21:28.000000 bent-0.0.55/bent/setup_package_wrapper.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.006741 bent-0.0.55/bent/src/
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.006741 bent-0.0.55/bent/src/NILINKER/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/NILINKER/__init__.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    10004 2024-04-29 19:24:25.000000 bent-0.0.55/bent/src/NILINKER/nilinker.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)      986 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/NILINKER/predict_nilinker.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    12838 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/NILINKER/utils.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.010741 bent-0.0.55/bent/src/REEL/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/REEL/__init__.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    15205 2024-04-30 12:53:08.000000 bent-0.0.55/bent/src/REEL/candidates.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2745 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/REEL/information_content.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2707 2024-04-30 11:23:40.000000 bent-0.0.55/bent/src/REEL/post_process.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    20290 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/REEL/ppr_for_ned_all.class
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    39492 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/REEL/ppr_for_ned_all.java
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    15077 2024-04-30 11:24:06.000000 bent-0.0.55/bent/src/REEL/pre_process.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2928 2024-04-30 11:23:38.000000 bent-0.0.55/bent/src/REEL/run.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1450 2024-04-30 11:03:55.000000 bent-0.0.55/bent/src/REEL/utils.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/__init__.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.010741 bent-0.0.55/bent/src/abbreviation_detector/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/abbreviation_detector/__init__.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)     2404 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/abbreviation_detector/run.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)      296 2024-04-29 14:35:38.000000 bent-0.0.55/bent/src/cfg.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     5643 2024-04-30 10:02:18.000000 bent-0.0.55/bent/src/classes.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.010741 bent-0.0.55/bent/src/dicts/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/dicts/__init__.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.010741 bent-0.0.55/bent/src/dicts/annotations/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/dicts/annotations/__init__.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)    12350 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/dicts/annotations/dataset_entities.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.010741 bent-0.0.55/bent/src/dicts/kb/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/dicts/kb/__init__.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)     3702 2024-04-29 14:07:52.000000 bent-0.0.55/bent/src/dicts/kb/generate_dicts.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)    23898 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/dicts/kb/kb.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.010741 bent-0.0.55/bent/src/dicts/relation_extraction/
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/dicts/relation_extraction/__init__.py
--rw-rw-r--   0 pruas     (1000) pruas     (1000)     8394 2024-04-29 10:21:28.000000 bent-0.0.55/bent/src/dicts/relation_extraction/dicts.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2654 2024-04-30 12:32:03.000000 bent-0.0.55/bent/src/nel.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    20071 2024-04-29 18:40:09.000000 bent-0.0.55/bent/src/ner.py
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)    19487 2024-04-30 12:53:52.000000 bent-0.0.55/bent/src/utils.py
-drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2024-05-02 09:46:04.010741 bent-0.0.55/bent.egg-info/
--rw-r--r--   0 pruas     (1000) pruas     (1000)    18902 2024-05-02 09:46:03.000000 bent-0.0.55/bent.egg-info/PKG-INFO
--rw-rw-r--   0 pruas     (1000) pruas     (1000)     1247 2024-05-02 09:46:03.000000 bent-0.0.55/bent.egg-info/SOURCES.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)        1 2024-05-02 09:46:03.000000 bent-0.0.55/bent.egg-info/dependency_links.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)       63 2024-05-02 09:46:03.000000 bent-0.0.55/bent.egg-info/entry_points.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)      296 2024-05-02 09:46:03.000000 bent-0.0.55/bent.egg-info/requires.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)        5 2024-05-02 09:46:03.000000 bent-0.0.55/bent.egg-info/top_level.txt
--rw-rw-r--   0 pruas     (1000) pruas     (1000)       38 2024-05-02 09:46:04.014741 bent-0.0.55/setup.cfg
--rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1978 2024-05-02 09:45:55.000000 bent-0.0.55/setup.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)    11340 2023-02-03 16:59:19.000000 bent-0.0.9/LICENSE.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)    17578 2023-02-03 19:10:35.000000 bent-0.0.9/PKG-INFO
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     3426 2023-02-03 16:59:19.000000 bent-0.0.9/README.rst
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/__init__.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    13167 2023-02-03 16:59:19.000000 bent-0.0.9/bent/annotate.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     1699 2023-02-03 16:59:19.000000 bent-0.0.9/bent/get_data.sh
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     1718 2023-02-03 16:59:19.000000 bent-0.0.9/bent/get_kb_dicts.sh
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)      203 2023-02-03 16:59:19.000000 bent-0.0.9/bent/requirements.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     2351 2023-02-03 16:59:19.000000 bent-0.0.9/bent/setup_package.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1909 2023-02-03 16:59:19.000000 bent-0.0.9/bent/setup_package.sh
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/NILINKER/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/NILINKER/__init__.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    10851 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/NILINKER/nilinker.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     1003 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/NILINKER/predict_nilinker.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    13194 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/NILINKER/utils.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/REEL/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/__init__.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    14863 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/candidates.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2866 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/information_content.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2903 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/post_process.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    20290 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/ppr_for_ned_all.class
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    39492 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/ppr_for_ned_all.java
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    15702 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/pre_process.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     3314 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/run.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     4303 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/REEL/utils.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/__init__.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/abbreviation_detector/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/abbreviation_detector/__init__.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     2541 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/abbreviation_detector/run.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)      284 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/cfg.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     5803 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/classes.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)     2453 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/nel.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    19947 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/ner.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/setup/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/__init__.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/setup/annotations/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/annotations/__init__.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)    12270 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/annotations/dataset_entities.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/setup/kb/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/kb/__init__.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     3719 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/kb/generate_dicts.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)    24028 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/kb/kb.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent/src/setup/relation_extraction/
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/relation_extraction/__init__.py
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     8085 2023-02-03 16:59:19.000000 bent-0.0.9/bent/src/setup/relation_extraction/dicts.py
+-rwxrwxr-x   0 pruas     (1000) pruas     (1000)    20061 2023-02-03 19:05:11.000000 bent-0.0.9/bent/src/utils.py
+drwxrwxr-x   0 pruas     (1000) pruas     (1000)        0 2023-02-03 19:10:35.000000 bent-0.0.9/bent.egg-info/
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)    17578 2023-02-03 19:10:34.000000 bent-0.0.9/bent.egg-info/PKG-INFO
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     1180 2023-02-03 19:10:35.000000 bent-0.0.9/bent.egg-info/SOURCES.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)        1 2023-02-03 19:10:34.000000 bent-0.0.9/bent.egg-info/dependency_links.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)      203 2023-02-03 19:10:34.000000 bent-0.0.9/bent.egg-info/requires.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)        5 2023-02-03 19:10:34.000000 bent-0.0.9/bent.egg-info/top_level.txt
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)       38 2023-02-03 19:10:35.000000 bent-0.0.9/setup.cfg
+-rw-rw-r--   0 pruas     (1000) pruas     (1000)     2172 2023-02-03 19:10:23.000000 bent-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `bent-0.0.55/LICENSE.txt` & `bent-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bent-0.0.55/PKG-INFO` & `bent-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bent
-Version: 0.0.55
+Version: 0.0.9
 Summary: BENT: Biomedical Entity Annotator
 Home-page: https://github.com/lasigeBioTM/bent
 Author: Pedro Ruas
 Author-email: pedrosimruas@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -219,168 +219,124 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Unix Shell
 Classifier: Programming Language :: Java
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7, <=3.10.13
+Requires-Python: >=3.7
 License-File: LICENSE.txt
-Requires-Dist: obonet==0.3.0
-Requires-Dist: tensorflow-gpu==2.5.1; python_version < "3.10"
-Requires-Dist: tensorflow==2.13.1; python_version == "3.10"
-Requires-Dist: transformers==4.9.0; python_version < "3.10"
-Requires-Dist: transformers==4.35.2; python_version == "3.10"
-Requires-Dist: torch==1.9.1; python_version < "3.10"
-Requires-Dist: torch==2.0; python_version == "3.10"
-Requires-Dist: networkx==2.5.1
-Requires-Dist: gdown==4.6.0
-Requires-Dist: rapidfuzz==2.0.2
-Requires-Dist: tqdm==4.66
-Requires-Dist: spacy==3.0.1; python_version < "3.10"
-Requires-Dist: spacy==3.7.2; python_version == "3.10"
-Requires-Dist: seqeval==1.2.2
-Requires-Dist: orjson==3.8.5
-Requires-Dist: psutil
 
 
 
 BENT: Biomedical Entity Annotator
 ---------------------------------
 
 Python Library for Named Entity Recognition (NER) and Linking (NEL) in the biomedical domain.
 
+NER models are based on `PubMedBERT <https://arxiv.org/pdf/2007.15779.pdf>`__ and a post-processing rule-based module.
+the NEL model is a graph-based approach based on the Personalized PageRank algorithm and Information content.
+
 BENT can be used for: 
 
 * Named Entity Recogniton (NER)
 * Named Entity Linking (NEL) 
 * Named Entity Recognition and Linking (NER+NEL)
 
-Access the full `documentation <https://bent.readthedocs.io/en/latest/>`__.
+Access the full documentation `here <https://bent.readthedocs.io/en/latest/>`__.
 
-Citation::
+Citation:
 
-  Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking. 
-  Journal of Biomedical Informatics, 132:104137, 2022. 
-  doi: https://doi.org/10.1016/j.jbi.2022.104137.
+* Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking <https://www.sciencedirect.com/science/article/pii/S1532046422001526>`__. Journal of Biomedical Informatics, 132:104137, 2022. doi: https://doi.org/10.1016/j.jbi.2022.104137.
 
 Installation
-~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~
 
 To use the current version of BENT it is required: 
 
-*  OS: Debian>=11/Ubuntu>=20.04
-
-*  Python >=3.7, <=3.10.13
+* OS based on Ubuntu/Debian 
+* `Conda <https://docs.conda.io/en/latest/>`__ environment 
+* Python>=3.7
+* Between 11 and 15 GB free space (5 GB Anaconda + 2.5 GB to install dependencies + 3.0 GB data or 7.5 GB if you use all available knowlegde bases for NEL)
 
-*  Required space between 5.5 GB - 10 GB 
-   * Dependencies: 2.5 GB 
-   * Data: between 3.0 GB (base) or 7.5 GB (if you use all available knowledge bases for Named Entity Linking)
+.. note::
 
-**NOTE**: Python Docker images (3.7 to 3.9) in `Docker Hub <https://hub.docker.com/_/python>`__ have Debian 11 as the base OS.
+   Please ensure that you have the appropriate version of Conda installed.
 
 
-Install the BENT package using pip:
+Create a Conda environment (adapt for the name of your project):
 
 ::
 
-   pip install bent
+   conda create --name annotation_project python=3.7
 
 
-The following knowledge bases can be configured:
+Activate the environment:
 
-* 'medic' (`MEDIC <http://ctdbase.org/>`__)
+::
 
-* 'do' (`Disease ontology <https://disease-ontology.org/>`__)
+   conda activate annotation_project
 
-* 'chebi' (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
-* 'ctd_chem' (`CTD-Chemicals <http://ctdbase.org/>`__)
+Install the BENT package using pip:
 
-* 'ncbi_gene' (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
+::
 
-* 'ctd_gene' (`CTD-GENES <http://ctdbase.org/>`__)
+   pip install bent
 
-* 'ncbi_taxon' (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
-* 'go_bp' (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
+After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Specify the knowledge bases that will be used:
 
-* 'ctd_anat' (`CTD-Anatomy <http://ctdbase.org/>`__)
+::
 
-* 'fma' (`Foundation model of Anatomy <http://sig.biostr.washington.edu/projects/fm/AboutFM.html>`__)
+   python -c "from bent.setup_package import setup_package;setup_package([<kb1>, <kb2>, <kb3>])"
 
-* 'uberon' (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
+Available knowledge bases:
 
-* 'go_cc' (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
+* ‘medic’ (`MEDIC <http://ctdbase.org/>`__)
 
-* 'cell_ontology' (`Cell Ontology <https://cell-ontology.github.io/>`__)
+* ‘do’ (`Disease ontology <https://disease-ontology.org/>`__)
 
-* 'cellosaurus' (`Cellosaurus <https://www.cellosaurus.org/>`__)
+* 'chebi’ (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
+* ‘ctd_chem’ (`CTD-Chemicals <http://ctdbase.org/>`__)
 
-After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Run in the command line:
+* ‘ncbi_gene’ (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
 
-::
+* ‘ctd_gene’ (`CTD-GENES <http://ctdbase.org/>`__)
 
-   bent_setup
+* ‘ncbi_taxon’ (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
+* ‘go_bp’ (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
 
-Only the default knowledge bases 'medic' and 'chebi' will be available at this point.
+* ‘ctd_anat’ (`CTD-Anatomy <http://ctdbase.org/>`__)
 
-To disable annoyng messages in the terminal run:
+* ‘uberon’ (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
 
-::
+* ‘go_cc’ (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
 
-   export TF_CPP_MIN_LOG_LEVEL='3'
+* ‘cell_ontology’ (`Cell Ontology <https://cell-ontology.github.io/>`__)
 
+* cellosaurus’ (`Cellosaurus <https://www.cellosaurus.org/>`__)
 
-You can download more knowledge bases later by specifying the desired knowledge bases among the ones that are available:
+Example to download only the MEDIC vocabulary:
 
 ::
 
-   python -c "from bent.get_kbs import get_additional_kbs;get_additional_kbs([<kb1>, <kb2>])"
-
-
-Example: to download the NCBI Taxonomy and the NCBI Gene run: 
-
-::    
+   python -c "from bent.setup_package import setup_package;setup_package(['medic'])"
 
-    python -c "from bent.get_kbs import get_additional_kbs;get_additional_kbs(['ncbi_taxon', 'ncbi_gene'])"
 
+If you want to download all knowledge bases, choose the option 'all':
 
-Get started
-~~~~~~~~~~~
-
-To apply the complete pipeline of entity extraction (NER+NEL) set the arguments:
+::
 
-* **recognize**: indicate that the NER module will be applied ('True')
-* **link**: indicate that the NEL module will be applied ('True')
-* **types**: entity types to recognize and the respective target knowledge bases.
-* **in_dir**: directory path containing the text files to be annotated (the directory must contain text files exclusively)
-* **out_dir**: the output directory that will contain the annotation files
+   python -c "from bent.setup_package import setup_package;setup_package(['all'])"
 
 
-Example:
+You can download more knowledge bases later by running the same command and specifying the desired knolwedge bases among the ones that are available and setting the argument ' only_kb_dicts' to True:
 
 ::
 
-   import bent.annotate as bt
-
-   bt.annotate(
-           recognize=True,
-           link=True,
-           types={
-            'disease': 'medic'
-            'chemical': 'chebi',
-            'gene': 'ncbi_gene',
-            'anatomical': 'uberon',
-            'cell_line': 'cellosaurus',
-            'bioprocess': 'go_bp'
-            },
-           in_dir='input/txt/',
-           out_dir='output/nel/'
-   )
-
+   python -c "from bent.setup_package import setup_package;setup_package([<kb>],  only_kb_dicts=True)"
 
-It is also possible to apply the pipeline (NER+NEL) to a string or a list or strings instantiated in the execution script.
 
-To see more usage examples, access the `documentation <https://bent.readthedocs.io/en/latest/usage.html>`__.
+Reinitiate the conda environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bent-0.0.55/README.rst` & `bent-0.0.9/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,114 @@
 
 
 BENT: Biomedical Entity Annotator
 ---------------------------------
 
 Python Library for Named Entity Recognition (NER) and Linking (NEL) in the biomedical domain.
 
+NER models are based on `PubMedBERT <https://arxiv.org/pdf/2007.15779.pdf>`__ and a post-processing rule-based module.
+the NEL model is a graph-based approach based on the Personalized PageRank algorithm and Information content.
+
 BENT can be used for: 
 
 * Named Entity Recogniton (NER)
 * Named Entity Linking (NEL) 
 * Named Entity Recognition and Linking (NER+NEL)
 
-Access the full `documentation <https://bent.readthedocs.io/en/latest/>`__.
+Access the full documentation `here <https://bent.readthedocs.io/en/latest/>`__.
 
-Citation::
+Citation:
 
-  Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking. 
-  Journal of Biomedical Informatics, 132:104137, 2022. 
-  doi: https://doi.org/10.1016/j.jbi.2022.104137.
+* Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking <https://www.sciencedirect.com/science/article/pii/S1532046422001526>`__. Journal of Biomedical Informatics, 132:104137, 2022. doi: https://doi.org/10.1016/j.jbi.2022.104137.
 
 Installation
-~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~
 
 To use the current version of BENT it is required: 
 
-*  OS: Debian>=11/Ubuntu>=20.04
-
-*  Python >=3.7, <=3.10.13
+* OS based on Ubuntu/Debian 
+* `Conda <https://docs.conda.io/en/latest/>`__ environment 
+* Python>=3.7
+* Between 11 and 15 GB free space (5 GB Anaconda + 2.5 GB to install dependencies + 3.0 GB data or 7.5 GB if you use all available knowlegde bases for NEL)
 
-*  Required space between 5.5 GB - 10 GB 
-   * Dependencies: 2.5 GB 
-   * Data: between 3.0 GB (base) or 7.5 GB (if you use all available knowledge bases for Named Entity Linking)
+.. note::
 
-**NOTE**: Python Docker images (3.7 to 3.9) in `Docker Hub <https://hub.docker.com/_/python>`__ have Debian 11 as the base OS.
+   Please ensure that you have the appropriate version of Conda installed.
 
 
-Install the BENT package using pip:
+Create a Conda environment (adapt for the name of your project):
 
 ::
 
-   pip install bent
+   conda create --name annotation_project python=3.7
 
 
-The following knowledge bases can be configured:
+Activate the environment:
 
-* 'medic' (`MEDIC <http://ctdbase.org/>`__)
+::
 
-* 'do' (`Disease ontology <https://disease-ontology.org/>`__)
+   conda activate annotation_project
 
-* 'chebi' (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
-* 'ctd_chem' (`CTD-Chemicals <http://ctdbase.org/>`__)
+Install the BENT package using pip:
 
-* 'ncbi_gene' (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
+::
 
-* 'ctd_gene' (`CTD-GENES <http://ctdbase.org/>`__)
+   pip install bent
 
-* 'ncbi_taxon' (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
-* 'go_bp' (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
+After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Specify the knowledge bases that will be used:
 
-* 'ctd_anat' (`CTD-Anatomy <http://ctdbase.org/>`__)
+::
 
-* 'fma' (`Foundation model of Anatomy <http://sig.biostr.washington.edu/projects/fm/AboutFM.html>`__)
+   python -c "from bent.setup_package import setup_package;setup_package([<kb1>, <kb2>, <kb3>])"
 
-* 'uberon' (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
+Available knowledge bases:
 
-* 'go_cc' (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
+* ‘medic’ (`MEDIC <http://ctdbase.org/>`__)
 
-* 'cell_ontology' (`Cell Ontology <https://cell-ontology.github.io/>`__)
+* ‘do’ (`Disease ontology <https://disease-ontology.org/>`__)
 
-* 'cellosaurus' (`Cellosaurus <https://www.cellosaurus.org/>`__)
+* 'chebi’ (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
+* ‘ctd_chem’ (`CTD-Chemicals <http://ctdbase.org/>`__)
 
-After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Run in the command line:
+* ‘ncbi_gene’ (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
 
-::
+* ‘ctd_gene’ (`CTD-GENES <http://ctdbase.org/>`__)
 
-   bent_setup
+* ‘ncbi_taxon’ (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
+* ‘go_bp’ (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
 
-Only the default knowledge bases 'medic' and 'chebi' will be available at this point.
+* ‘ctd_anat’ (`CTD-Anatomy <http://ctdbase.org/>`__)
 
-To disable annoyng messages in the terminal run:
+* ‘uberon’ (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
 
-::
+* ‘go_cc’ (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
 
-   export TF_CPP_MIN_LOG_LEVEL='3'
+* ‘cell_ontology’ (`Cell Ontology <https://cell-ontology.github.io/>`__)
 
+* cellosaurus’ (`Cellosaurus <https://www.cellosaurus.org/>`__)
 
-You can download more knowledge bases later by specifying the desired knowledge bases among the ones that are available:
+Example to download only the MEDIC vocabulary:
 
 ::
 
-   python -c "from bent.get_kbs import get_additional_kbs;get_additional_kbs([<kb1>, <kb2>])"
-
-
-Example: to download the NCBI Taxonomy and the NCBI Gene run: 
-
-::    
+   python -c "from bent.setup_package import setup_package;setup_package(['medic'])"
 
-    python -c "from bent.get_kbs import get_additional_kbs;get_additional_kbs(['ncbi_taxon', 'ncbi_gene'])"
 
+If you want to download all knowledge bases, choose the option 'all':
 
-Get started
-~~~~~~~~~~~
-
-To apply the complete pipeline of entity extraction (NER+NEL) set the arguments:
+::
 
-* **recognize**: indicate that the NER module will be applied ('True')
-* **link**: indicate that the NEL module will be applied ('True')
-* **types**: entity types to recognize and the respective target knowledge bases.
-* **in_dir**: directory path containing the text files to be annotated (the directory must contain text files exclusively)
-* **out_dir**: the output directory that will contain the annotation files
+   python -c "from bent.setup_package import setup_package;setup_package(['all'])"
 
 
-Example:
+You can download more knowledge bases later by running the same command and specifying the desired knolwedge bases among the ones that are available and setting the argument ' only_kb_dicts' to True:
 
 ::
 
-   import bent.annotate as bt
-
-   bt.annotate(
-           recognize=True,
-           link=True,
-           types={
-            'disease': 'medic'
-            'chemical': 'chebi',
-            'gene': 'ncbi_gene',
-            'anatomical': 'uberon',
-            'cell_line': 'cellosaurus',
-            'bioprocess': 'go_bp'
-            },
-           in_dir='input/txt/',
-           out_dir='output/nel/'
-   )
-
+   python -c "from bent.setup_package import setup_package;setup_package([<kb>],  only_kb_dicts=True)"
 
-It is also possible to apply the pipeline (NER+NEL) to a string or a list or strings instantiated in the execution script.
 
-To see more usage examples, access the `documentation <https://bent.readthedocs.io/en/latest/usage.html>`__.
+Reinitiate the conda environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bent-0.0.55/bent/annotate.py` & `bent-0.0.9/bent/annotate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,398 +1,338 @@
 #!/usr/bin/env python
 import os
 import random
 import string
-from pathlib import Path
 import spacy
 from tqdm import tqdm
 import bent.src.utils as utils
 from bent.src.ner import ner
 from bent.src.nel import nel
 from bent.src.classes import Dataset
-import bent.src.cfg as cfg
-import warnings
 
-warnings.simplefilter(action='ignore', category=FutureWarning)
-warnings.showwarning = utils.ignore_spacy_warning
 
-def _recognize(
-    in_dir,
-    entity_types,
-    out_dir,
-    ner_model,
-    return_dataset=False,
-    input_tmp=False,
-):
-    """Pipeline to perform Named Entity Recognition. For each input
-    document/text it outputs either an annotations file (BRAT format) or a
+def recognizer(in_dir, input_text, entity_types, out_dir, ner_model, run_id):
+    """Pipeline to perform Named Entity Recognition. For each input 
+    document/text it outputs either an annotations file (BRAT format) or a 
     Dataset object including all documents and respective annotations.
 
-    :param in_dir: path to directory containing text files to be annotated,
+    :param in_dir: path to directory containing text files to be annotated, 
         defaults to None
     :type in_dir: _type_, optional
-    :param types: the entity types that will be recognized
+    :param input_text: text string or list of text strings (each element 
+        represinting a different document) to be annotated, defaults to None
+    :type input_text: str or list, optional
+    :param types: the entity types that will be recognized 
         :type types: list
     :param out_dir: path to directory where the output of the pipeline will be
-        located, optional. If 'out_dir' == None (deafult) a Dataset object
-        including all documents and respective annotations will be returned
+        located, optional. If 'out_dir' == None (deafult) a Dataset object 
+        including all documents and respective annotations will be returned  
     :type out_dir: str, defaults to None
-    :param ner_model: the Named Entity Recognition model that will be used,
+    :param ner_model: the Named Entity Recognition model that will be used, 
         defaults to 'pubmedbert'
     :type ner_model: str, optional
-    :param input_tmp: indicates if the input is composed of temporary text files.
-    :type input_tmp: bool
-    :return: dataset (an object including all the input texts along with the
+    :return: dataset (an object including all the input texts along with the 
         annotations) if 'out_dir' is None; an annotation file for each inputed
         text if 'out_dir' is different that None
     :rtype: Dataset object, text file(s)
     """
-
+    
     # Disable printing of annoying messages
     os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
-    # Spacy language model to segment the inputed texts into sentences
-    lang_model = spacy.load("en_core_sci_lg")
+    # Spacy language model to segment the inputed texts into sentences 
+    lang_model = spacy.load('en_core_sci_lg')
     stopwords = lang_model.Defaults.stop_words
-
+    
     # Load the NER models that will be used
     recognizer = ner(ner_model, entity_types, stopwords)
 
-    # Whether the input is a directory with text files or not
-    dataset = Dataset()
+    # Wether the input is a directory with text files or not
+    filename_mode = False 
 
-    assert in_dir is not None, 'Invalid "in_dir"!'
+    dataset = Dataset()
 
-    if recognizer.model_type == "bert":
-        input_files = [
-            f"{in_dir}{filename}" for filename in os.listdir(in_dir)
-        ]
+    if out_dir == None:
+        # In this case a dataset object will be outputted and the 
+        # temporary annotation files will be stored in 'tmp/NER/' directory
+        tmp_out_dir = '.tmp/{}/'.format(run_id)
+        os.mkdir(tmp_out_dir)
+
+    if recognizer.model_type == "bert":  
+        input_files = None
+
+        if in_dir != None:
+            filename_mode = True
+            input_files = [
+                in_dir + filename for filename in os.listdir(in_dir)]
+            
+        elif input_text != None:
+            
+            if type(input_text) == str:
+                input_files = [input_text]
+            
+            elif type(input_text) == list:
+                input_files = input_text
 
         # Recognize entities in each document
-        pbar = tqdm(
-            total=len(input_files),
-            colour="green",
-            desc="Recognizing entities (documents)",
-        )
-
-        for i, filename in enumerate(input_files, start=1):
-            doc_id = ""
-
-            if input_tmp:
-                doc_id = f"doc_{str(i)}"
-
+        pbar = tqdm(total=len(input_files), colour= 'green', 
+            desc='Recognizing entities (documents)')
+        
+        for i, filename in enumerate(input_files):
+            doc_id = ''
+            text = ''
+            
+            if filename_mode:
+                doc_id = filename.strip(in_dir).strip('.txt')
+               
+                with open(filename, 'r') as input_file:
+                    text = input_file.read()
+                    input_file.close()
+            
             else:
-                doc_id = filename.strip(in_dir).strip(".txt")
-
-            text = ""
-
-            with open(filename, "r", encoding="utf-8") as input_file:
-                text = input_file.read()
-                input_file.close()
-
+                text = filename
+                doc_id = str(i)
+            
             # Sentence segmentation
-            doc_sentences = utils._sentence_splitter(text, lang_model)
-
+            doc_sentences = utils.sentence_splitter(text, lang_model)
+            
             # Objectify input
-            doc_obj = utils._objectify_ner_input(doc_id, text, doc_sentences)
-
+            doc_obj = utils.objectify_ner_input(
+                doc_id, text, doc_sentences)
+            
             # Apply NER models to input text
             doc_entities = recognizer.apply(doc_obj)
 
             # Output recognized entities to a file
             # Prepare output string with annotations
-            doc_annots = utils._prepare_output_from_objects(doc_entities, only_ner=True)
+            doc_annots = utils.prepare_output_from_objects(
+                doc_entities, only_ner=True)
+
+            out_filename = ''
 
-            out_filename = f"{out_dir}{doc_id}.ann"
+            if out_dir == None:
+                out_filename = '{}{}.ann'.format(tmp_out_dir, doc_id)                
+                # Add Document object to Dataset object
+                dataset.add_doc(doc_entities)
 
-            with open(out_filename, "w", encoding="utf-8") as out_file:
+            else:
+                out_filename = out_dir + doc_id + '.ann'
+
+            with open(out_filename, 'w') as out_file:
                 out_file.write(doc_annots[:-1])
                 out_file.close()
-
+            
             del doc_annots
             del text
             del doc_sentences
             del doc_obj
             del doc_entities
+            
+            utils.garbage_collect()
 
             pbar.update(1)
-
+            
         pbar.close()
 
     del recognizer
     del lang_model
     del stopwords
+    utils.garbage_collect()
 
-    if return_dataset:
+    if out_dir == None:
         return dataset
 
 
-def _link(
-    recognize,
-    types,
-    nel_model,
-    run_id,
-    ner_dir=None,
-    out_dir=None,
-    dataset=None,
-    return_dataset=False,
-):
-    """Pipeline to perform Named Entity Linking. For each input
-    annotation files with recognized entities it outputs an updated
+def linker(
+            recognize, types, nel_model, run_id, out_format=None, 
+            ner_dir=None, out_dir=None, dataset=None):
+    """Pipeline to perform Named Entity Linking. For each input 
+    annotation files with recognized entities it outputs an updated 
     annotations file (BRAT format) with knowledge base identifiers for each
     entity.
 
-    :param recognize: specifies wether the pipeline performs Named Entity
+    :param recognize: specifies wether the pipeline performs Named Entity 
         Recognition, defaults to False
     :type recognize: bool, optional
     :param types: types of entities to be recognized along with the respective
-        target knowledge bases, defaults to {}. Options:
-        {'disease': 'medic'}, {'disease': 'do'},
+        target knowledge bases, defaults to {}. Options: 
+        {'disease': 'medic'}, {'disease': 'do'}, 
         {'chemical': 'chebi'}, {'chemical': 'ctd_chem'},
         {'gene': 'ncbi_gene'},
         {'bioprocess': 'go_bp'},
         {'organism': 'ncbi_taxon'},
         {'anatomical': 'uberon'}, {'anatomical', 'ctd_anat'},
         {'cell_component': 'go_cc'},
         {'cell_line': 'cellosaurus'},
         {'cell_type': 'cell_ontology'},
         {'variant': ''}
         {<entity_type>: <custom_knowledge_base>}
     :type types: dict, optional
-    :param nel_model: the Named Entity Linking model that will be used,
+    :param nel_model: the Named Entity Linking model that will be used, 
         defaults to 'reel_nilinker'
-    :param ner_dir: directory where the output of the NER stage is located.
+    :param ner_dir: directory where the output of the NER stage is located. 
         Only applicable when there is already an output from the NER stage.
-        Defaults to 'None'.
+        Defaults to 'None'. 
     :type ner_dir: str, optional
     :param out_dir: path to directory where the output of the pipeline will be
-        located, optional. If 'out_dir' == None (deafult) a Dataset object
-        including all documents and respective annotations will be returned
+        located, optional. If 'out_dir' == None (deafult) a Dataset object 
+        including all documents and respective annotations will be returned  
     :type out_dir: str, defaults to None
-    :param dataset: dataset (an object including all the input texts along with
+    :param dataset: dataset (an object including all the input texts along with 
         the annotations from the NER stage), defaults to None
     :type dataset: Dataset, optional
     :raises ValueError: if 'ner_dir'==None and recognize==False, which means
         that if the NER stage was not performed it is necessary nevertheless
-        indicate the directory containing annotation files corresponding to
+        indicate the directory containing annotation files corresponding to 
         the NER output
     """
-
+    
     # Link the recognized/inputted entities to the specified KBs
-    linker = nel(nel_model, run_id)
+    linker = nel(nel_model)
     target_kbs = {}
-
+    
     for ent_type in types.keys():
-
-        if types[ent_type] != "":
+        
+        if types[ent_type] != '':
             target_kbs[ent_type] = types[ent_type]
-
+    
     if recognize:
-        ner_dir = out_dir
-
+        
+        if out_dir == None:
+            ner_dir = '.tmp/{}/'.format(run_id)
+        
+        else:
+            # The output of the previous NER step is locacted in the out_dir
+            ner_dir = out_dir
+    
     else:
 
-        if ner_dir is None and run_id is None:
-            raise ValueError(
-                'It is necessary to specify the directory \
-                containing the NER output ("ner_dir")'
-            )
-
+        if ner_dir == None and run_id==None:
+            raise ValueError('It is necessary to specify the directory \
+                containing the NER output ("ner_dir")')
+    
     nel_run_ids = linker.apply(target_kbs, ner_dir=ner_dir)
-
+    
     del linker
-
-    if return_dataset:
-        return utils._update_dataset_with_nel_output(dataset, nel_run_ids)
-
+    
+    if out_dir == None:
+        return utils.update_dataset_with_nel_output(dataset, nel_run_ids)
+    
     else:
-        utils._update_ner_file_with_nel_output(ner_dir, nel_run_ids, out_dir=out_dir)
+        utils.update_ner_file_with_nel_output(ner_dir, nel_run_ids, out_dir=out_dir)  
 
 
-def annotate(
-    recognize=False,
-    link=False,
-    types={},
-    input_text=None,
-    in_dir=None,
-    ner_dir=None,
-    input_format="brat",
-    out_format="brat",
-    out_dir=None,
-    ner_model="pubmedbert",
-    nel_model="reel_nilinker",
-):
+def annotate(recognize=False, link=False, types={}, input_text=None,
+        in_dir=None, ner_dir=None, input_format='brat', out_format='brat',
+        out_dir=None, ner_model='pubmedbert', nel_model='reel_nilinker'):
     """Pipeline to annotate text(s) with recognized entities (Named Entity and
     Recognition) to link them to knowledge base concepts (Named Entity Linking).
 
-    :param recognize: specifies wether the pipeline performs Named Entity
+    :param recognize: specifies wether the pipeline performs Named Entity 
         Recognition, defaults to False
     :type recognize: bool, optional
-    :param link: specifies wether the pipeline performs Named Entity
+    :param link: specifies wether the pipeline performs Named Entity 
         Linking, defaults to False
     :type link: bool, optional
     :param types: types of entities to be recognized along with the respective
-        target knowledge bases, defaults to {}. Options:
-        {'disease': 'medic'}, {'disease': 'do'},
+        target knowledge bases, defaults to {}. Options: 
+        {'disease': 'medic'}, {'disease': 'do'}, 
         {'chemical': 'chebi'}, {'chemical': 'ctd_chem'},
         {'gene': 'ncbi_gene'},
         {'bioprocess': 'go_bp'},
         {'organism': 'ncbi_taxon'},
         {'anatomical': 'uberon'}, {'anatomical', 'ctd_anat'},
         {'cell_component': 'go_cc'},
         {'cell_line': 'cellosaurus'},
         {'cell_type': 'cell_ontology'},
         {'variant': ''}
         {<entity_type>: <custom_knowledge_base>}
     :type types: dict, optional
-    :param input_text: text string or list of text strings (each element
+    :param input_text: text string or list of text strings (each element 
         represinting a different document) to be annotated, defaults to None
     :type input_text: str or list, optional
     :param in_dir: path to directory containing text files to be annotated (NER
-        and optionally NEL),
+        and optionally NEL), 
         defaults to None
     :type in_dir: _type_, optional
-    :param ner_dir: directory where the output of the NER stage is located.
+    :param ner_dir: directory where the output of the NER stage is located. 
         Only applicable when there is already an output from the NER stage.
-        Defaults to 'None'.
+        Defaults to 'None'. 
     :type ner_dir: str, optional
-    :param in_format: the format of the input files. Options: 'brat',
+    :param in_format: the format of the input files. Options: 'brat', 
         'bioc_xml', 'bioc_json', 'pubtator'
     :type input_format: str, optional, defaults to 'brat'
     :param out_dir: path to directory where the output of the pipeline will be
         located, optional. To choose current directory set out_dir==''.
-        If 'out_dir' == None (deafult) a Dataset object
-        including all documents and respective annotations will be returned
+        If 'out_dir' == None (deafult) a Dataset object 
+        including all documents and respective annotations will be returned  
     :type out_dir: str, defaults to None
     :param out_format: the format of the ouput ('brat', None), defaults to None
     :type out_format: str, optional
-    :param ner_model: the Named Entity Recognition model that will be used,
+    :param ner_model: the Named Entity Recognition model that will be used, 
         defaults to 'pubmedbert'
     :type ner_model: str, optional
-    :param nel_model: the Named Entity Linking model that will be used,
+    :param nel_model: the Named Entity Linking model that will be used, 
         defaults to 'reel_nilinker'
     :type nel_model: str, optional
     :raises ValueError: if both 'input_text' and 'in_dir' are None
     :raises ValueError: if both 'recognize' and 'link' are None
-    :return: dataset (an object including all the input texts along with the
+    :return: dataset (an object including all the input texts along with the 
         annotations) if 'out_dir' is None; an annotation file for each inputed
         text if 'out_dir' is different that None
     :rtype: Dataset object, text file(s)
     """
-    run_id = "".join(random.choices(string.ascii_uppercase + string.digits, k=15))
-
-    os.makedirs(cfg.tmp_dir + run_id, exist_ok=True)
+    run_id = ''.join(random.choices(string.ascii_uppercase + string.digits, 
+        k=15)) 
 
     # Check if input arguments are valid
-    utils._check_input_args(
-        recognize,
-        link,
-        types,
-        input_format,
-        input_text,
-        in_dir,
-        ner_dir,
-        out_dir
-    )
+    utils.check_input_args(recognize, link, types, input_format,
+        input_text, in_dir, ner_dir, out_dir, ner_model, nel_model)
 
-    if ner_dir is not None:
-        # There are already files with NER annotations in the 'ner_dir'
+    if ner_dir != None:
         in_dir = ner_dir
-
-    if out_dir is not None:
-
+    
+    if out_dir != None:
+        
         if not os.path.exists(out_dir):
-            os.makedirs(out_dir, exist_ok=True)
-
-    # --------------------------------------------------------------------------
+            os.mkdir(out_dir)
+    
+    #--------------------------------------------------------------------------
     #                   CONVERT INPUT TO THE BRAT FORMAT
-    # --------------------------------------------------------------------------
-    input_tmp = False
-
-    if input_text is not None:
-        # The input is either a string or a list of strings, so there is no
-        # 'in_dir'.
-        # A temporary directory to store the text files will be created
-        in_dir = ".tmp/"
-
-        if not os.path.exists(in_dir):
-            os.makedirs(in_dir, exist_ok=True)
-
-        in_dir = f".tmp/{run_id}/"
-
-        if not os.path.exists(in_dir):
-            os.makedirs(in_dir, exist_ok=True)
-
-        in_dir = f"{in_dir}txt/"
-
-        if not os.path.exists(in_dir):
-            os.makedirs(in_dir, exist_ok=True)
-
-        utils._convert_input_files(
-            in_dir=in_dir, input_text=input_text
-        )
-
-        input_tmp = True
-
-    # --------------------------------------------------------------------------
+    #-------------------------------------------------------------------------- 
+    if input_text!= None:
+        
+        utils.convert_input_files(input_format, input_text=input_text, 
+            in_dir=in_dir, recognize=recognize)
+        
+        in_dir += 'brat/'
+        
+    #--------------------------------------------------------------------------
     #                           NER
-    # --------------------------------------------------------------------------
+    #--------------------------------------------------------------------------
     if recognize:
         entity_types = types.keys()
 
-        if out_dir is not None:
-            _recognize(
-                in_dir, entity_types, out_dir, ner_model, run_id, input_tmp=input_tmp
-            )
-
-        elif out_dir is not None:
-            # In this case a dataset object will be outputted and the
-            # temporary annotation files will be stored in 'tmp/NER/' directory
-            tmp_out_dir = f"{in_dir}ann/"
-
-            if not os.path.exists(tmp_out_dir):
-                os.makedirs(tmp_out_dir, exist_ok=True)
-
-            dataset = _recognize(
-                in_dir,
-                entity_types,
-                tmp_out_dir,
-                ner_model,
-                return_dataset=True,
-                input_tmp=input_tmp,
-            )
-
-            if link:
-                # The input dir for the NEL module now is the directory
-                # containing the annotation files outputted by the NER module
-                in_dir = tmp_out_dir
-
-    # --------------------------------------------------------------------------
+        if out_dir != None:
+            recognizer(
+                in_dir, input_text, entity_types, out_dir, ner_model, run_id)
+        
+        else:
+            dataset = recognizer(
+                in_dir, input_text, entity_types, out_dir, ner_model, run_id)
+    #--------------------------------------------------------------------------
     #                           NEL
-    # --------------------------------------------------------------------------
+    #--------------------------------------------------------------------------
     if link:
 
-        if out_dir is not None:
-            # Annotation files with NER+NEL output will be created in 'out_dir'
-            _link(
-                recognize,
-                types,
-                nel_model,
-                run_id,
-                ner_dir=in_dir,
-                out_dir=out_dir,
-            )
+        if out_dir != None:
+            linker(
+                recognize, types, nel_model, run_id, out_format=out_format,
+                    ner_dir=in_dir, 
+                out_dir=out_dir)
 
         else:
-            # A Dataset object will be returned containing NER+NEL output
-            dataset = _link(
-                recognize,
-                types,
-                nel_model,
-                run_id,
-                ner_dir=in_dir,
-                dataset=dataset,
-                out_dir=tmp_out_dir,
-                return_dataset=True,
-            )
-
+            dataset = linker(
+                recognize, types, nel_model, run_id, out_format=out_format, 
+                ner_dir=in_dir, dataset=dataset, out_dir=out_dir)
+            
             return dataset
```

### Comparing `bent-0.0.55/bent/get_data.sh` & `bent-0.0.9/bent/get_data.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/bin/bash
-package_path=$1
 
 # ---------------------------------------------------------------------------
 #                    Create directories for later use
 # ---------------------------------------------------------------------------
-cwd=$(pwd)
-data_dir="${package_path}/data"
-cd $data_dir
-mkdir -p "datasets/"
-mkdir -p "NILINKER/"
+mkdir ../data
+cd ../data/
+
+mkdir datasets/
+mkdir NILINKER/
+
 
 #-------------------------------------------------------------------------
 #   Download entity frequency dicts (to resolve overlapping entities)
 #-------------------------------------------------------------------------
 gdown https://drive.google.com/uc?id=1PYk84F_eCRYgbZ1c8VMCH9srKqulF0AV
 tar -xvf overlapping_entities.tar.gz
 rm overlapping_entities.tar.gz
@@ -23,15 +23,15 @@
 gdown https://drive.google.com/uc?id=1wDfQkyF526d6FBAbjZlmbrcWsMrUzfdL
 tar -xvf relations.tar.gz
 rm relations.tar.gz
 
 #-------------------------------------------------------------------------
 #                       Download NILINKER data
 #-------------------------------------------------------------------------
-cd "NILINKER/"
+cd NILINKER/
 # Word-concept dictionaries
 wget https://zenodo.org/record/6561477/files/word_concept.tar.gz?download=1
 tar -xvf 'word_concept.tar.gz?download=1'
 rm 'word_concept.tar.gz?download=1'
 
 # Trained models files
 wget https://zenodo.org/record/6561477/files/nilinker_files.tar.gz?download=1
@@ -39,8 +39,8 @@
 rm 'nilinker_files.tar.gz?download=1'
 
 # Embeddings
 wget https://zenodo.org/record/6561477/files/embeddings.tar.gz?download=1
 tar -xvf 'embeddings.tar.gz?download=1'
 rm 'embeddings.tar.gz?download=1'
 
-cd $cwd
+cd ../
```

### Comparing `bent-0.0.55/bent/src/NILINKER/nilinker.py` & `bent-0.0.9/bent/src/NILINKER/nilinker.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,308 +2,285 @@
 
 import numpy as np
 import tensorflow as tf
 from bent.src.NILINKER.utils import get_candidates_4_word, get_words_ids_4_entity
 
 
 class Words2embed(tf.keras.layers.Layer):
-    """First layer of the model, encodes entities and
-    candidates with embeddings."""
-
+    """First layer of the model, encodes entities and 
+       candidates with embeddings."""
+    
     def __init__(self, wc, word_embeds, candidate_embeds):
         super(Words2embed, self).__init__()
         self.word_embeds = word_embeds
         self.candidate_embeds = candidate_embeds
         self.wc_word2id = wc.word2id
         self.id2word = wc.id2word
         self.word2candidates = wc.word2candidates
         self.root_concept_int = wc.root_concept_int
-
+    
     def call(self, entity):
 
         # To get candidates for word l and r, we use the WC word_ids
         wc_word_l_id = entity.numpy()[0]
         wc_word_r_id = entity.numpy()[1]
 
         input_candidates_l = get_candidates_4_word(
-            self.id2word, self.word2candidates, wc_word_id=wc_word_l_id
-        )
-
+                                self.id2word, 
+                                self.word2candidates,
+                                wc_word_id=wc_word_l_id)
+        
         input_candidates_r = get_candidates_4_word(
-            self.id2word, self.word2candidates, wc_word_id=wc_word_r_id
-        )
-
+                                self.id2word, 
+                                self.word2candidates,
+                                wc_word_id=wc_word_r_id)
+        
         embed_candidates_r = tf.nn.embedding_lookup(
-            params=self.candidate_embeds, ids=input_candidates_r
-        )
+            params=self.candidate_embeds, ids=input_candidates_r)
         embed_candidates_l = tf.nn.embedding_lookup(
-            params=self.candidate_embeds, ids=input_candidates_l
-        )
+            params=self.candidate_embeds, ids=input_candidates_l)
 
         # To get the embeddings for word l and r, we use the embeds word ids
         embeds_word_l_id = entity.numpy()[2]
         embeds_word_r_id = entity.numpy()[3]
 
-        input_l = np.array(
-            [
-                embeds_word_l_id,
-            ]
-        )
-        input_r = np.array(
-            [
-                embeds_word_r_id,
-            ]
-        )
-
-        try:
-            embed_word_l = tf.nn.embedding_lookup(params=self.word_embeds, ids=input_l)
-        except:
-            input_l = np.array([0])
-            embed_word_l = tf.nn.embedding_lookup(params=self.word_embeds, ids=input_l)
-
-        try:
-            embed_word_r = tf.nn.embedding_lookup(params=self.word_embeds, ids=input_r)
-        except:
-            input_r = np.array([0])
-            embed_word_r = tf.nn.embedding_lookup(params=self.word_embeds, ids=input_r)
-
-        return embed_word_l, embed_word_r, embed_candidates_l, embed_candidates_r
+        input_l = np.array([embeds_word_l_id, ])
+        input_r = np.array([embeds_word_r_id, ])
+        
+        embed_word_l = tf.nn.embedding_lookup(
+            params=self.word_embeds, ids=input_l)
+        embed_word_r = tf.nn.embedding_lookup(
+            params=self.word_embeds, ids=input_r)
+       
+        return embed_word_l, embed_word_r, \
+               embed_candidates_l, embed_candidates_r 
 
 
 class Attention(tf.keras.layers.Layer):
     """Attention layer of the model."""
 
     def __init__(self, params):
         super(Attention, self).__init__()
-
+        
         self.W_a = tf.Variable(
-            tf.random.truncated_normal([params[0], params[0]], stddev=0.5),
-            tf.float32,
-            name="W_a",
-        )
-
-        self.b_a = tf.Variable(tf.zeros([1, params[0]]), tf.float32, name="b_a")
+            tf.random.truncated_normal([params[0], params[0]], \
+            stddev=0.5), 
+            tf.float32, name='W_a')
+        
+        self.b_a = tf.Variable(
+            tf.zeros([1, params[0]]), tf.float32, name='b_a')
 
     @staticmethod
-    def determine_attention(direction, embed_word, embed_opposite_candidates, W_a, b_a):
-
+    def determine_attention(
+            direction, embed_word, embed_opposite_candidates, W_a, b_a):
+        
         direction_dict = {"l": "r", "r": "l"}
-        name1 = "embed_align_" + direction_dict[direction]
+        name1 = "embed_align_" + direction_dict[direction]  
         name2 = "embed_aggre_word_" + direction + "_pure"
 
         embed_word_align = tf.nn.tanh(
-            tf.matmul(embed_word, W_a) + b_a, name=name1
-        )  # 1 * dim
+            tf.matmul(embed_word, W_a) + b_a, name=name1)  # 1 * dim
         attention = tf.nn.softmax(
-            tf.matmul(embed_opposite_candidates, tf.transpose(embed_word_align)), axis=0
-        )
-
+            tf.matmul(embed_opposite_candidates, \
+            tf.transpose(embed_word_align)), axis=0)
+        
         embed_candidates = attention * embed_opposite_candidates
-
-        attention = tf.reduce_sum(embed_candidates, axis=0, keepdims=True, name=name2)
-
+        
+        attention = tf.reduce_sum(
+            embed_candidates, axis=0, keepdims=True, name=name2)
+                                  
         return attention
 
-    def call(self, embed_word_l, embed_word_r, embed_candidates_l, embed_candidates_r):
-
-        embed_aggre_word_l = Attention.determine_attention(
-            "l", embed_word_l, embed_candidates_r, self.W_a, self.b_a
-        )
-
-        embed_aggre_word_r = Attention.determine_attention(
-            "r", embed_word_r, embed_candidates_l, self.W_a, self.b_a
-        )
-
+    def call(self, embed_word_l, embed_word_r, 
+            embed_candidates_l, embed_candidates_r):
+        
+        embed_aggre_word_l = Attention.determine_attention("l", embed_word_l, 
+            embed_candidates_r, self.W_a, self.b_a)
+
+        embed_aggre_word_r = Attention.determine_attention("r", embed_word_r, 
+            embed_candidates_l, self.W_a, self.b_a)
+        
         return embed_aggre_word_l, embed_aggre_word_r
 
 
 class PhraseVec(tf.keras.layers.Layer):
     """It concatenates candidate and word embeddings after attention values
-    are calculated."""
+       are calculated."""
 
     def __init__(self, params):
         super(PhraseVec, self).__init__()
-
-        self.W_c = tf.Variable(
-            tf.random.truncated_normal([2 * params[0], params[0]], stddev=1.0),
-            tf.float32,
-            name="W_c",
-        )
-        self.b_c = tf.Variable(tf.zeros([1, params[0]]), tf.float32, name="b_c")
+        
+        self.W_c = tf.Variable(tf.random.truncated_normal(
+            [2 * params[0], params[0]], stddev=1.0), tf.float32, name='W_c')
+        self.b_c = tf.Variable(
+            tf.zeros([1, params[0]]), tf.float32, name='b_c')
+        
 
     def call(
-        self,
-        embed_word_r,
-        embed_word_l,
-        embed_aggre_word_r_pure,
-        embed_aggre_word_l_pure,
-    ):
+            self, embed_word_r, embed_word_l, embed_aggre_word_r_pure, 
+            embed_aggre_word_l_pure):
 
         embed_words_whole = embed_word_r + embed_word_l
-
-        embed_candidates_whole = embed_aggre_word_r_pure + embed_aggre_word_l_pure
-
+        
+        embed_candidates_whole = embed_aggre_word_r_pure \
+                                 + embed_aggre_word_l_pure
+        
         phrase_vec = tf.math.tanh(
             tf.matmul(
-                tf.concat([embed_words_whole, embed_candidates_whole], 1), self.W_c
-            )
-            + self.b_c,
-            name="phrase_vec",
-        )
-
+            tf.concat([embed_words_whole, embed_candidates_whole], 1), \
+                       self.W_c) + self.b_c, name="phrase_vec")
+        
         return phrase_vec
 
 
 class Output(tf.keras.layers.Layer):
     """Logits layer with raw predictions for the classes."""
-
+    
     def __init__(self, candidate_embeds, name=None):
         super(Output, self).__init__()
         self.candidate_embeds = candidate_embeds
 
     def call(self, phrase_vec):
         output = tf.matmul(phrase_vec, tf.transpose(self.candidate_embeds))
-
+        
         return output
 
 
 class Nilinker(tf.keras.Model):
     """Instantiates the NILINKER model integrating all the layers
-    as well methods for training, evaluation, and prediction."""
-
-    def __init__(
-        self, word_embeds, candidate_embeds, params, wc, kb_id_to_name, embeds_words2id
-    ):
+       as well methods for training, evaluation, and prediction."""
 
+    def __init__(self, word_embeds, candidate_embeds, 
+            params, wc, kb_id_to_name, embeds_words2id):
+        
         super(Nilinker, self).__init__()
         self.word_embeds = tf.Variable(
-            tf.constant(
-                word_embeds,
-                shape=[word_embeds.shape[0], word_embeds.shape[1]],
-                dtype=tf.float32,
-            ),
-            trainable=False,
-            name="word_embeds",
-        )
+                                tf.constant(
+                                    word_embeds, shape=[word_embeds.shape[0], 
+                                    word_embeds.shape[1]], dtype=tf.float32), 
+                                    trainable=False, 
+                                    name='word_embeds')
         self.candidate_embeds = tf.Variable(
-            tf.constant(
-                candidate_embeds, shape=[params[1], params[0]], dtype=tf.float32
-            ),
-            trainable=True,
-            name="candidate_embeds",
-        )
-        self.first_layer = Words2embed(wc, self.word_embeds, self.candidate_embeds)  # ,
-        # kb_id_to_name)
+                                    tf.constant(
+                                        candidate_embeds, 
+                                        shape=[params[1], params[0]], 
+                                        dtype=tf.float32), 
+                                        trainable=True, 
+                                        name='candidate_embeds')
+        self.first_layer = Words2embed(
+                                wc, self.word_embeds, self.candidate_embeds)#, 
+                                #kb_id_to_name)
         self.attention_layer = Attention(params)
         self.phrase_layer = PhraseVec(params)
         self.output_layer = Output(self.candidate_embeds)
         self.optimizer = None
         self.candidate_num = wc.candidate_num
         self.id2candidate = wc.id2candidate
         self.wc_word2id = wc.word2id
         self.embeds_word2id = embeds_words2id
         self.id_to_name = kb_id_to_name
-        self.top_k = params[2]
+        self.top_k= params[2]
 
     def call(self, input):
-
+       
         top_candidates_list = list()
         y_pred_list = list()
-
+        
         for entity in input:
-            embed_word_l, embed_word_r, embed_candidates_l, embed_candidates_r = (
-                self.first_layer(entity)
-            )
+            embed_word_l, embed_word_r, \
+                embed_candidates_l, embed_candidates_r = self.first_layer(
+                                                           entity)  
 
             # 2nd layer: attention
             embed_aggre_word_l, embed_aggre_word_r = self.attention_layer(
-                embed_word_l, embed_word_r, embed_candidates_l, embed_candidates_r
-            )
-
+                                                        embed_word_l, 
+                                                        embed_word_r,
+                                                        embed_candidates_l, 
+                                                        embed_candidates_r)
+            
             # 3rd layer: concatenation of word + candidate embeddings
             phrase_vec = self.phrase_layer(
-                embed_word_r, embed_word_l, embed_aggre_word_r, embed_aggre_word_l
-            )
-
+                embed_word_r, embed_word_l, embed_aggre_word_r, 
+                embed_aggre_word_l)
+            
             # 4th layer: logits output layer
             output = self.output_layer(phrase_vec)
-
+            
             # 5th layer: Activation (final layer)
             y_pred_ent = tf.nn.softmax(output)
             y_pred_list.append(y_pred_ent)
 
+            
             candidates_rank = tf.nn.top_k(
-                y_pred_ent, k=self.candidate_num
-            )  # sorted=True)
-
+                y_pred_ent, k=self.candidate_num)#sorted=True)
+            
             ent_candidates = list()
 
             for i in range(0, self.top_k):
                 cand = int(candidates_rank[1][0][i])
                 ent_candidates.append(cand)
 
             top_candidates_list.append(ent_candidates)
-
-        y_pred_tensor = tf.reshape(y_pred_list, [len(input), self.candidate_num])
-
+        
+        y_pred_tensor = tf.reshape(
+            y_pred_list, [len(input), self.candidate_num])
+        
         return y_pred_tensor, top_candidates_list
 
     def predict_step(self, input):
-
+        
         # Input is a batch, even if it only contains 1 entity:
         # To ensure compatibility with train and test modes
         y_pred, top_candidates = self(input)
-
+        
         top_candidates_kb_ids = [
-            self.id2candidate[candidate] for candidate in top_candidates[0]
-        ]
+            self.id2candidate[candidate] for candidate in top_candidates[0]]
         top_candidates_names = [
-            self.id_to_name[kb_id]
-            for kb_id in top_candidates_kb_ids
-            if kb_id in self.id_to_name.keys()
-        ]
-
-        output = [
-            (top_candidates_kb_ids[i], top_candidates_names[i])
-            for i in range(len(top_candidates_names))
-        ]
-
+            self.id_to_name[kb_id] for kb_id in top_candidates_kb_ids if kb_id in self.id_to_name.keys()]
+  
+        output = [(top_candidates_kb_ids[i], top_candidates_names[i]) 
+            for i in range(len(top_candidates_names))]
+        
         output = tf.expand_dims(output, axis=0)
-
+        
         return output
-
+    
     def prediction(self, entity_str):
         """Wrapper function to preprocess the given entity and to input it to
         the NILINKER model. It returns the top k KB candidates (names and KB
-        ids).
+        ids).  
         """
-
+        
         # The first stept is the pre-processing of the inputed entity.
         # The string has to be converted into the following format:
-        #
+        # 
         #              [wc_word_l_id, wc_word_r_id,
         #               embeds_word_l_id, embeds_word_r_id,
         #               gold_label_id]
 
         wc_word_l_id, wc_word_r_id = get_words_ids_4_entity(
-            entity_str, wc_word2id=self.wc_word2id, mode="wc"
-        )
-
-        embeds_word_l_id, embeds_word_r_id = get_words_ids_4_entity(
-            entity_str, embeds_word2id=self.embeds_word2id, mode="embeds"
-        )
-
-        input_entity = (wc_word_l_id, wc_word_r_id, embeds_word_l_id, embeds_word_r_id)
-
-        # Now apply NILINKER to predict relevant KB concepts
-        top_candidates = self.predict([input_entity], verbose=0)
-
-        output = []
-
+                                    entity_str, 
+                                    wc_word2id=self.wc_word2id,
+                                    mode='wc')
+        
+        embeds_word_l_id, \
+           embeds_word_r_id = get_words_ids_4_entity(
+                                   entity_str, 
+                                   embeds_word2id=self.embeds_word2id,
+                                   mode='embeds')
+                               
+        input_entity = (wc_word_l_id, wc_word_r_id,
+                        embeds_word_l_id, embeds_word_r_id)
+        
+        # Now apply NILINKER to predict relevant KB concepts  
+        top_candidates = self.predict([input_entity])
+        
+        output = list()
+        
         for tmp in top_candidates:
-
+            
             for cand in tmp:
-                kb_id = cand[0].decode("utf-8")
-                cand_name = cand[1].decode("utf-8")
+                kb_id = cand[0].decode('utf-8')
+                cand_name = cand[1].decode('utf-8')
                 output.append((kb_id, cand_name))
-
-        return output
+   
+        return output
```

### Comparing `bent-0.0.55/bent/src/NILINKER/predict_nilinker.py` & `bent-0.0.9/bent/src/NILINKER/predict_nilinker.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 from bent.src.NILINKER.nilinker import Nilinker
 from bent.src.NILINKER.utils import get_wc_embeds, get_kb_data
 
 
 def load_model(partition, top_k=1):
     """Prepare the model for later prediction when requested.
 
-    :param partition: has value 'medic', 'ctd_chem', 'hp', 'chebi',
+    :param partition: has value 'medic', 'ctd_chem', 'hp', 'chebi', 
         "go_bp", "ctd_anatomy"
     :type partition: str
-    :return: loaded and compiled NILINKER model for the specified partition
-    :rtype: tf.keras.Model() object
+    :return: loaded and compiled NILINKER model for the specified partition 
+    :rtype: tf.keras.Model() object 
     """
 
     word_embeds, candidate_embeds, wc, embeds_word2id = get_wc_embeds(partition)
     params = [200, wc.candidate_num, top_k]
     id_to_name = get_kb_data(partition)
-
-    model_dir = f"{cfg.root_path}/data/NILINKER/nilinker_files/{partition}/train/"
-
+    
+    model_dir = "{}data/NILINKER/nilinker_files/{}/train/".format(cfg.root_path, partition)
+    
     model = Nilinker(
-        word_embeds, candidate_embeds, params, wc, id_to_name, embeds_word2id
-    )
-    model.compile(run_eagerly=True)
+        word_embeds, candidate_embeds, params, wc, id_to_name, embeds_word2id)
+    model.compile(run_eagerly = True)
     model.built = True
     model.load_weights(model_dir + "best.h5")
 
     return model
```

### Comparing `bent-0.0.55/bent/src/NILINKER/utils.py` & `bent-0.0.9/bent/src/NILINKER/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,208 +3,197 @@
 import bent.src.cfg as cfg
 import orjson as json
 import numpy as np
 from rapidfuzz import process, fuzz
 
 
 class WordConcept:
-    """Class representing a word-concept (WC) dictionary object associated with
-    a given KB. It includes mappings between words and WC int ids, words and
+    """Class representing a word-concept (WC) dictionary object associated with 
+    a given KB. It includes mappings between words and WC int ids, words and 
     candidates, etc.
     """
-
-    __slots__ = [
-        "partition",
-        "filepath",
-        "word2candidates",
-        "word2id",
-        "id2word",
-        "candidate_num",
-        "candidate2id",
-        "id2candidate",
-        "root_concept_int",
-    ]
-
+    
+    __slots__ = ['partition', 'filepath', 'word2candidates', 'word2id',
+        'id2word', 'candidate_num', 'candidate2id', 'id2candidate', 
+        'root_concept_int' ]
     def __init__(self, partition):
-
+    
         self.partition = partition
-        self.filepath = (
-            f"{cfg.root_path}/data/NILINKER/word_concept/wc_{partition}.json"
-        )
+        self.filepath = "{}data/NILINKER/word_concept/wc_{}.json".format(cfg.root_path, partition)
         self.word2candidates = None
         self.word2id = None
         self.id2word = None
         self.candidate_num = None
         self.candidate2id = None
         self.id2candidate = None
         self.root_concept_int = None
-
+        
     def build(self):
-        """Fill a WordConcept object with info about words belonging to
-        the considered Word-Concept (WC) dict, and candidates and respectives
-        int ids. (*note: Candidate int ids are distinct from WC words ids).
+        """Fill a WordConcept object with info about words belonging to 
+        the considered Word-Concept (WC) dict, and candidates and respectives 
+        int ids. (*note: Candidate int ids are distinct from WC words ids). 
         """
 
         # Load node_id_to_int
         with open(
-            f"{cfg.root_path}/data/NILINKER/embeddings/{self.partition}/node_id_to_int_{self.partition}.json"
-        ) as in_file:
+                "{}data/NILINKER/embeddings/{}/node_id_to_int_{}.json"\
+                .format(cfg.root_path, self.partition, self.partition)) as in_file:
             node_id_to_int = json.loads(in_file.read())
 
         # Create candidate2id and id2candidate
         id2candidate, candidate2id = {}, {}
-
+        
         for concept in node_id_to_int.keys():
             candidate_int = node_id_to_int[concept]
-            candidate2id[concept] = candidate_int
+            candidate2id[concept] = candidate_int 
             id2candidate[candidate_int] = concept
 
         # Add int for the root concept to wc
-        root_dict = {
-            "go_bp": ("GO:0008150", "biological_process"),
-            "chebi": ("CHEBI:00", "root"),
-            "hp": ("HP:0000001", "All"),
-            "medic": ("MESH:C", "Diseases"),
-            "ctd_anat": ("MESH:A", "Anatomy"),
-            "ctd_chem": ("MESH:D", "Chemicals"),
-        }
-        root_concept_kb_id = root_dict[self.partition][0]
+        root_dict = {"go_bp": ("GO:0008150", "biological_process"), 
+                    "chebi": ("CHEBI:00", "root"), 
+                    "hp": ("HP:0000001", "All"), 
+                    "medic": ("MESH:C", "Diseases"), 
+                    "ctd_anat": ("MESH:A", "Anatomy"), 
+                    "ctd_chem": ("MESH:D", "Chemicals")}
+        root_concept_kb_id= root_dict[self.partition][0]
         root_concept_int = candidate2id[root_concept_kb_id]
         self.root_concept_int = root_concept_int
 
         word2candidates = {}
-
+        
         # Load word-concept file into dict
-        with open(self.filepath, "r", encoding="utf-8") as wc:
+        with open(self.filepath, 'r', encoding='utf-8') as wc: 
             word2candidates = json.loads(wc.read())
-
+        
         # Create word2candidates with candidates int
         vocab_size = len(node_id_to_int.keys())
-
+        
         word2candidates_up, wc_word2id, id2word = {}, {}, {}
         word_count = 0
 
         for word in word2candidates.keys():
             word_count += 1
             wc_word2id[word] = word_count
             id2word[word_count] = word
 
             candidates = word2candidates[word]
             candidates_int = []
-
+            
             for candidate in candidates:
                 # Convert concept ID in int
                 candidate_int = node_id_to_int[candidate]
                 candidate_int_up = 0
 
                 if candidate_int == vocab_size:
                     candidate_int_up = root_concept_int
 
                 else:
                     candidate_int_up = candidate_int
-
+                
                 candidates_int.append(candidate_int_up)
 
             word2candidates_up[word] = candidates_int
-
+            
         self.word2candidates = word2candidates_up
-        self.word2id = wc_word2id
+        self.word2id = wc_word2id 
         self.id2word = id2word
         self.candidate2id = candidate2id
         self.id2candidate = id2candidate
         self.candidate_num = len(candidate2id.keys())
-        root_concept_kb_id = root_dict[self.partition][0]
+        root_concept_kb_id= root_dict[self.partition][0]
         root_concept_int = candidate2id[root_concept_kb_id]
         self.root_concept_int = root_concept_int
-
-
+        
+    
 def load_word_embeds(embeds_dir):
-    """Load word embeddings from file into a Numpy array and generate dicts
+    """Load word embeddings from file into a Numpy array and generate dicts 
     with information about each word and respective int ID.
 
     :param embeds_filepath: path for the file containing word embeddings
     :type embeds_filepath: str
     :return: embeds, word2id, id2word
     :rtype: Numpy array, dict, dict
     """
 
     embeds, vocabulary = [], []
 
-    with open(f"{embeds_dir}word_embeddings.txt", "r", encoding="utf-8") as embed_file:
-
+    with open(embeds_dir + 'word_embeddings.txt', 'r', encoding='utf-8') \
+            as embed_file:
+        
         for line in embed_file.readlines():
             word = line.split()[0]
             embed = [float(item) for item in line.split()[1:]]
             embeds.append(embed)
             vocabulary.append(word)
-
+        
         embed_file.close()
-
-    assert len(embeds) == len(vocabulary)
+    
+    assert (len(embeds) == len(vocabulary))
 
     embeds_word2id = {}
-
-    with open(f"{embeds_dir}word2id.json", "r") as word2id_file:
+    
+    with open(embeds_dir + 'word2id.json', 'r') as word2id_file:
         embeds_word2id = json.loads(word2id_file.read())
         word2id_file.close()
-
-    embeds = np.array(embeds)  # s.astype('float32')
+ 
+    embeds = np.array(embeds)#s.astype('float32')
     embeds = embeds / np.sqrt(np.sum(embeds * embeds, axis=1, keepdims=True))
-
+   
     return embeds, embeds_word2id
 
 
 def load_candidate_embeds(embeds_filepath, candidate2id):
     """Load candidate embeddings from file into a Numpy array.
 
-    :param embeds_filepath: path for the file containing candidate
+    :param embeds_filepath: path for the file containing candidate 
         (i.e. KB concepts) embeddings
     :type embeds_filepath: str
     :param candidate2id: info about candidates and respective internal ID
     :type candidate2id: dict
     :return: embeds
     :rtype: Numpy array
     """
 
     embed_dict = {}
-
-    with open(embeds_filepath, "r", encoding="utf-8") as embed_file:
-
+    
+    with open(embeds_filepath, 'r', encoding='utf-8') as embed_file:
+        
         for line in embed_file.readlines():
             word = line.split()[0]
             embedding = [float(item) for item in line.split()[1:]]
             embed_dict[word] = embedding
 
     embeds = []
-
-    for candidate in candidate2id.keys():
+    
+    for candidate in candidate2id.keys(): 
         candidate_id = candidate2id[candidate]
         embeds.append(embed_dict[str(candidate_id)])
-
+    
     embeds = np.array(embeds)
     embeds = embeds / np.sqrt(np.sum(embeds * embeds, axis=1, keepdims=True))
-
+    
     return embeds
 
 
-def get_candidates_4_word(wc_2idword, word2candidates, word_str="", wc_word_id=-1):
-    """Retrieve KB candidate concepts for given word (either WC word id or
-    string) or for the most similar word in the WC if the word is not present
+def get_candidates_4_word(
+        wc_2idword, word2candidates, word_str='', wc_word_id=-1):
+    """Retrieve KB candidate concepts for given word (either WC word id or 
+    string) or for the most similar word in the WC if the word is not present 
     in the WC.
 
     :param wc_2idword: mappings between WC word ids and WC words
     :type wc_2idword: dict
-    :param word2candidates: mappings between WC words and KB
+    :param word2candidates: mappings between WC words and KB 
         candidate concepts
     :type word2candidates: dict
     :param word_str: string of the target word
     :type word_str = str
-    :param wc_word_id: the WC word id for the target word
+    :param wc_word_id: the WC word id for the target word 
     :type wc_word_id: int or numpy.int64
-    :raises ValueError: if given input is invalid, input must be either a
+    :raises ValueError: if given input is invalid, input must be either a 
         string or a valid WC word id
     :return: candidates_ids
     :rtype: Numpy array
 
     >>> wc_word_id = 444
     >>> wc_2idword = {444: 'gene'}
     >>> word2candidates = {'gene': [1, 2, 3]}
@@ -214,100 +203,102 @@
     >>> get_candidates_4_wordid(wc_2idword,word2candidates,word_str=word)
     [1, 2, 3]
     >>> word_id = 3.5
     >>> get_candidates_4_wordid(wc_2idword,word2candidates,word_id=word_id)
     ValuError: 'Input not valid! Must be either a word string or a WC word id'
     """
 
-    word = ""
-
-    if wc_word_id != -1 and (isinstance(wc_word_id, np.int64) or isinstance(wc_word_id, int)):
-
+    word = ''
+    
+    if wc_word_id != -1 and \
+            (type(wc_word_id) == np.int64 or type(wc_word_id) == int):
+        
         word = wc_2idword[wc_word_id]
-
+        
     else:
 
-        if word_str != "":
+        if word_str != '':
             word = word_str
-
+        
         else:
             raise ValueError(
-                "Input not valid! Must be either a word string or a WC word id"
-            )
-
+               'Input not valid! Must be either a word string or a WC word id')
+    
     candidates = []
 
     if word in word2candidates.keys():
         candidates = word2candidates[word]
 
     else:
         top_match = process.extract(
-            word, word2candidates.keys(), scorer=fuzz.token_sort_ratio, limit=1
-        )
+                        word, word2candidates.keys(), 
+                        scorer=fuzz.token_sort_ratio, 
+                        limit=1)
         most_similar_word = top_match[0][0]
         candidates = word2candidates[most_similar_word]
 
     candidates_ids = np.array(candidates)
-
+    
     return candidates_ids
 
-
+   
 def get_wc_embeds(partition):
-    """Create and populate WordConcept object and get Numpy arrays with
+    """Create and populate WordConcept object and get Numpy arrays with 
     candidate and word embeddings.
 
-    :param partition: has value 'medic', 'ctd_chem', 'hp', 'chebi', 'go_bp',
+    :param partition: has value 'medic', 'ctd_chem', 'hp', 'chebi', 'go_bp', 
         'ctd_anat'
     :type partition: str
     :return: word_embeds, candidate_embeds, wc
     :rtype: Numpy array, Numpy array, WordConcept object
     """
 
-    embeds_dir = f"{cfg.root_path}/data/NILINKER/embeddings/{partition}/"
-    word_embeds_filepath = embeds_dir
+    embeds_dir = "{}data/NILINKER/embeddings/{}/".format(cfg.root_path, partition)
+    word_embeds_filepath = embeds_dir 
     candidates_embeds_filepath = embeds_dir + partition + ".emb"
 
     wc = WordConcept(partition)
     wc.build()
 
     word_embeds, embeds_word2id = load_word_embeds(word_embeds_filepath)
-
+    
     candidate_embeds = load_candidate_embeds(
-        candidates_embeds_filepath, wc.candidate2id
-    )
+                            candidates_embeds_filepath, 
+                            wc.candidate2id)
 
     return word_embeds, candidate_embeds, wc, embeds_word2id
 
 
 def get_tokens_4_entity(entity_str):
-
+    
     tokens = []
-
-    if isinstance(entity_str, str):
+    
+    if type(entity_str) == str: 
         tokens = entity_str.split(" ")
-
+    
     else:
-        raise TypeError("Entity type is not <str>")
+        raise TypeError('Entity type is not <str>')
 
     if len(tokens) == 1:
-        # If the entity has only 1 word, we assume that
+        # If the entity has only 1 word, we assume that 
         # it has two repeated words
         tokens = [tokens[0], tokens[0]]
 
     return tokens
 
 
-def get_words_ids_4_entity(entity_str, wc_word2id={}, embeds_word2id={}, mode=""):
+def get_words_ids_4_entity(
+        entity_str, wc_word2id={}, embeds_word2id={}, mode=''):
     """Tokenize given entity string and, according with the selected mode,
-    return the ids of the words that are part of the entity. If mode 'wc' it
-    returns the WC word ids for left and right words, if mode 'embeds' it
-    returns the embeddings word ids for left and right words. If a given word
-    is not present in the given dictionary, it finds the most similar word in
+    return the ids of the words that are part of the entity. If mode 'wc' it 
+    returns the WC word ids for left and right words, if mode 'embeds' it 
+    returns the embeddings word ids for left and right words. If a given word 
+    is not present in the given dictionary, it finds the most similar word in 
     the dict according with the Levenshtein distance.
-
+    
     :param entity_str: the target entity string
     :type entity_str: str
     :param wc_word2id: mappings between each word in the WC and the
         respective int ids
     :type wc_word2id: dict
     :param embeds_word2id: mappings between each word in the embeddings
         vocabulary and the respective int ids
@@ -318,93 +309,89 @@
         right words of the given entity.
     :rtype: tuple with 2 ints
 
     >>> entity = 'arrythmic palpitation'
     >>> wc_word2id = {'palpitation':1663,'arrythmic':1629,'hematoma':1353}
     >>> get_words_ids_4_entity(entity, wc_word2id=wc_word2id, mode='wc')
     1629, 1663
-
+    
     >>> entity = 'arrythmic palpitations'
     >>> embeds_word2id = {'palpitation':1,'arrythmic':2,'hematoma':3}
     >>> mode = 'embeds'
     >>> get_words_ids_4_entity(entity,embeds_word2id=embeds_word2id,mode=mode)
     2, 1
     """
-
+    
     ids = {}
 
-    if mode == "wc":
+    if mode == 'wc':
         ids = wc_word2id
-
-    elif mode == "embeds":
+    
+    elif mode == 'embeds':
         ids = embeds_word2id
 
     else:
-        raise ValueError(
-            'Invalid mode! Choose either "wc" (to get the \
+        raise ValueError('Invalid mode! Choose either "wc" (to get the \
                           word ids from Word-Concept) or "embeds" mode \
-                         (to get words ids from the embeddings vocabulary)'
-        )
+                         (to get words ids from the embeddings vocabulary)')
 
     tokens = get_tokens_4_entity(entity_str)
 
     word_l_id, word_r_id, token_count = 0, 0, 1
-
+    
     for token in tokens[:2]:
         # Only consider the first two words of the entity
-
+        
         if token in ids.keys():
 
             if token_count == 1:
                 word_l_id = ids[token]
 
             elif token_count == 2:
                 word_r_id = ids[token]
 
         else:
             top_match = process.extract(
-                token, ids.keys(), scorer=fuzz.token_sort_ratio, limit=1
-            )
-
+                token, ids.keys(), scorer=fuzz.token_sort_ratio, 
+                limit=1)
+           
             most_similar_word = ids[top_match[0][0]]
-
+            
             if token_count == 1:
                 word_l_id = most_similar_word
 
             elif token_count == 2:
                 word_r_id = most_similar_word
-
+        
         token_count += 1
-
+    
     return word_l_id, word_r_id
 
 
 def get_kb_data(partition):
-    """Load KB data (concept names, synonyms, IDs, etc) associated with given
+    """Load KB data (concept names, synonyms, IDs, etc) associated with given 
     partition into a KnowledgeBase object.
 
-    :param partition: has value 'medic', 'ctd_chem', 'hp', 'chebi',
+    :param partition: has value 'medic', 'ctd_chem', 'hp', 'chebi', 
         'go_bp' or 'ctd_anat'
     :type partition: str
     :return: kb_data representing the given KB
     :rtype: KnowledgeBase object
     """
 
-    source_filename = f"{cfg.root_path}/data/kbs/dicts/{partition}/id_to_name.json"
+    source_filename = '{}data/dicts/{}/id_to_name.json'.format(cfg.root_path, partition)
 
-    if partition == "chebi":
-        source_filename = (
-            f"{cfg.root_path}/data/kbs/dicts/chebi/id_to_name_nilinker.json"
-        )
+    if partition == 'chebi':
+        source_filename = '{}data/dicts/chebi/id_to_name_nilinker.json'.format(cfg.root_path)
 
-    with open(source_filename, "r") as in_file:
-        id_to_name = json.loads(in_file.read())
+    with open(source_filename, 'r') as in_file:
+        id_to_name = json.loads(in_file.read()) 
         in_file.close()
 
     # Format the KB identifiers (MESH:D019967 passa a MESH_D019967)
     id_to_name_up = {}
 
     for kb_id in id_to_name.keys():
-        kb_id_up = kb_id.replace("_", ":")
+        kb_id_up = kb_id.replace('_', ':')
         id_to_name_up[kb_id_up] = id_to_name[kb_id]
 
     return id_to_name_up
```

### Comparing `bent-0.0.55/bent/src/REEL/candidates.py` & `bent-0.0.9/bent/src/REEL/candidates.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,455 +1,390 @@
 #!/usr/bin/env python
 
 import random
 from rapidfuzz import process, fuzz
-from bent.src.REEL.utils import CANDIDATE_STR
+from bent.src.REEL.utils import candidate_string
 
 
 def map_to_kb(
-    entity_text,
-    names,
-    synonyms,
-    name_to_id,
-    synonym_to_id,
-    kb,
-    kb_cache,
-    doc_abbreviations,
-):
+        entity_text, names, synonyms, name_to_id, synonym_to_id, kb, kb_cache, 
+        doc_abbreviations):
     """
-    Retrieve best knowledge base matches for entity text according to
+    Retrieve best knowledge base matches for entity text according to 
     lexical similarity (edit distance).
 
-    :param entity_text: the surface form of given entity
+    :param entity_text: the surface form of given entity 
     :type entity_text: str
-    :param names: the strings of all the concepts included in the given
+    :param names: the strings of all the concepts included in the given 
         knowledge base
     :type names: set
-    :synonyms: the strings of all the synonyms of the concepts included in the
+    :synonyms: the strings of all the synonyms of the concepts included in the 
         given knowledge base
     :type synonyms: set
-    :param name_to_id: mappings between each KB concept name and
+    :param name_to_id: mappings between each KB concept name and 
         respective KB id
     :type name_to_id: dict
-    :param synonym_to_id: mappings between each synonym for a
+    :param synonym_to_id: mappings between each synonym for a 
         given KB concept and respective KB id
     :type synonym_to_id: dict
     :param kb: target knowledge base
     :type kb: str
     :param kb_cache: candidates cache for the given kb
     :type kb_cache: dict
-
-    :return: matches (list) with format
+    
+    :return: matches (list) with format 
         [{'kb_id': <kb_id>, 'name': <name>, 'match_score': (...)}],
         changed_cache indicating wether the candidates cache was updated
-        in the performed mapping or if it remains inaltered, kb_cache_up
+        in the performed mapping or if it remains inaltered, kb_cache_up 
         corresponding to the updated candidates cache (if there was any change)
         or to the same candidates cache
     :rtype: tuple (list, bool, dict)
     """
-
-    changed_cache = False
+    
+    changed_cache = False 
     top_concepts = []
 
     if entity_text in doc_abbreviations:
         entity_text = doc_abbreviations[entity_text]
 
-    if entity_text in kb_cache:
+    if entity_text in kb_cache: 
         # There is already a candidate list stored in cache file
         top_concepts = kb_cache[entity_text]
 
     else:
-
-        if entity_text in names:
+    
+        if entity_text in names: 
             # There is an exact match for this entity
             top_concepts = [(entity_text, 100, 1)]
             kb_cache[entity_text] = top_concepts
             changed_cache = True
 
-        elif entity_text in synonyms:
+        elif entity_text in synonyms: 
             # There is an exact match for this entity
-            top_concepts = [(entity_text, 100, 1, "syn")]
+            top_concepts = [(entity_text, 100, 1, 'syn')]
             kb_cache[entity_text] = top_concepts
             changed_cache = True
-
+            
         else:
-            # Get first ten KB candidates according to lexical similarity
+            # Get first ten KB candidates according to lexical similarity 
             # with entity_text
             top_concepts = None
 
-            if kb == "ncbi_gene":
+            if kb == 'ncbi_gene':
                 top_concept = process.extractOne(
-                    entity_text, names, scorer=fuzz.token_sort_ratio
-                )
-
+                    entity_text, names ,scorer=fuzz.token_sort_ratio)
+                
                 top_concepts = [top_concept]
-
+                
             else:
                 top_concepts = process.extract(
-                    entity_text, names, limit=5, scorer=fuzz.token_sort_ratio
-                )
-
-            if top_concepts[0][1] == 100:
+                    entity_text, names, limit=10,
+                    scorer=fuzz.token_sort_ratio)
+                
+            if top_concepts[0][1] == 100: 
                 # There is an exact match for this entity
                 top_concepts = [top_concepts[0]]
 
-            elif top_concepts[0][1] < 100:
+            elif top_concepts[0][1] < 100: 
                 # Check for synonyms to this entity
                 top_synonyms = None
 
-                if kb == "ncbi_gene":
+                if kb == 'ncbi_gene':
                     top_synonym = process.extractOne(
-                        entity_text, synonyms, scorer=fuzz.token_sort_ratio
-                    )
+                        entity_text, synonyms,scorer=fuzz.token_sort_ratio)
 
                     top_synonyms = [top_synonym]
 
                 else:
                     top_synonyms = process.extract(
-                        entity_text, synonyms, limit=5, scorer=fuzz.token_sort_ratio
-                    )
+                        entity_text, synonyms, limit=10, 
+                        scorer=fuzz.token_sort_ratio)
 
                 for synonym in top_synonyms:
 
                     if synonym[1] == 100:
-                        synoynm_up = (synonym[0], synonym[1], synonym[2], "syn")
+                        synoynm_up = (
+                            synonym[0], synonym[1], synonym[2], 'syn')
                         top_concepts = [synoynm_up]
-
+                    
                     else:
 
                         if synonym[1] >= top_concepts[-1][1]:
-                            synoynm_up = (synonym[0], synonym[1], synonym[2], "syn")
+                            synoynm_up = (
+                                synonym[0], synonym[1], synonym[2], 'syn')
                             top_concepts.append(synoynm_up)
-
+            
             kb_cache[entity_text] = top_concepts
             changed_cache = True
-
-    # Build the candidates list with match id, name and matching score
+       
+    # Build the candidates list with match id, name and matching score 
     # with entity_text
     matches = []
 
     for concept in top_concepts:
         term_name = concept[0]
-        term_id = ""
+        term_id = ''
 
-        if len(concept) == 4 and concept[3] == "syn":
+        if len(concept) == 4 and concept[3] == 'syn':
             term_id = synonym_to_id[term_name]
 
         elif len(concept) == 3:
             term_id = name_to_id[term_name]
-
+        
         else:
             term_id = "NIL"
 
-        match = {"kb_id": term_id, "name": term_name, "match_score": concept[1] / 100}
-
+        match = {"kb_id": term_id,
+                 "name": term_name,
+                 "match_score": concept[1]/100}
+    
         matches.append(match)
-
+    
     return matches, changed_cache, kb_cache
 
 
-def get_candidate_properties(
-        candidate, 
-        min_match_score, 
-        id_to_info,
-        kb,
-        kb_id_2_id,
-        candidates_list):
-
-    if candidate["match_score"] > min_match_score and candidate["kb_id"] != "NIL":
-
-        if kb != "ncbi_gene":
-
-            try:
-                outcount = id_to_info[candidate["kb_id"]][0]
-                incount = id_to_info[candidate["kb_id"]][1]
-
-            except KeyError:
-                incount = 0
-                outcount = 0
-
-        else:
-            outcount = 0
-            incount = 0
-
-        candidate_id = 0
-
-        if candidate["kb_id"] in kb_id_2_id.keys():
-            candidate_id = kb_id_2_id[candidate["kb_id"]]
-
-        else:
-            # generate random id for current candidate
-            candidate_id = random.randint(0, 1000000)
-            kb_id_2_id[candidate["kb_id"]] = candidate_id
-
-        # The first candidate in candidate_names
-        # should be the correct disambiguation for entity
-        candidates_list.append(
-            {
-                "url": candidate["kb_id"],
-                "name": candidate["name"],
-                "outcount": outcount,
-                "incount": incount,
-                "id": candidate_id,
-                "links": [],
-                "score": candidate["match_score"],
-            }
-        )
-
-    return candidates_list
-
-
 def generate_candidates_list(
-    entity_text,
-    kb,
-    id_to_info,
-    names,
-    synonyms,
-    name_to_id,
-    synonym_to_id,
-    kb_cache,
-    min_match_score,
-    doc_abbreviations,
-    kb_id_2_id,
-    nil_candidates=None,
-):
+        entity_text, kb, id_to_info, names, synonyms, name_to_id, synonym_to_id, 
+        kb_cache, min_match_score, doc_abbreviations, kb_id_2_id, 
+        nil_candidates=None):
     """
     Build a structured candidates list for given entity text.
 
     :param entity_text: string of the considered entity
     :type entity_text: str
     :param kb: target knowledge base
     :type kb: str
-    :param id_to_info:
+    :param id_to_info: 
     :type id_to_info: dict
-    :param names: the strings of all the concepts included in the given
+    :param names: the strings of all the concepts included in the given 
         knowledge base
     :type names: set
-    :synonyms: the strings of all the synonyms of the concepts included in the
+    :synonyms: the strings of all the synonyms of the concepts included in the 
         given knowledge base
     :type synonyms: set
-    :param name_to_id: mappings between each ontology concept name and
+    :param name_to_id: mappings between each ontology concept name and 
         the respective id
     :type name_to_id: dict
-    :param synonym_to_id: mappings between each synonym for a given ontology
+    :param synonym_to_id: mappings between each synonym for a given ontology 
         concept and the respective id
     :type synonym_to_id: dict
     :param kb_cache: candidates cache for the given kb
     :type kb_cache: dict
-    :param min_match_score: minimum edit distance between the mention text
-        and candidate string, candidates below this threshold are excluded
+    :param min_match_score: minimum edit distance between the mention text 
+        and candidate string, candidates below this threshold are excluded 
         from candidates list
     :type min_match_score: float
     :param doc_abbreviations: abbreviations identified in the given document
     :type doc_abbreviations: dict
-    :param nil_candidates: in cases where the candidates outputed from the
+    :param nil_candidates: in cases where the candidates outputed from the 
         'NILINKER' model need to be structured
     :type nil_candidates: list
     :return: candidates_list including all the structured candidates for given
         entity, changed_cache indicating weter the candidates cache was updated
-        in the performed mapping or if it remains inaltered, kb_cache_up
+        in the performed mapping or if it remains inaltered, kb_cache_up 
         corresponding to the updated candidates cache (if there was any change)
         or to the same candidates cache
     :rtype: tuple (list, bool, dict)
     """
-
-    candidates_list = []
-
+    
+    candidates_list  = []
+    less_than_min_score = 0
+    
     # Retrieve best KB candidates names and respective ids
     candidate_names = []
     changed_cache = False
     kb_cache_up = {}
-    
-    if nil_candidates is None:
-        candidate_names, changed_cache, kb_cache_up = map_to_kb(
-            entity_text,
-            names,
-            synonyms,
-            name_to_id,
-            synonym_to_id,
-            kb,
-            kb_cache,
-            doc_abbreviations,
-        )
-        changed_cache = True
 
+    if nil_candidates == None:
+        candidate_names, changed_cache, kb_cache_up = map_to_kb(
+            entity_text, names, synonyms, name_to_id, synonym_to_id, 
+            kb, kb_cache, doc_abbreviations)
+     
     else:
         candidate_names = nil_candidates
-    
-    # Get properties for each retrieved candidate
-    if candidate_names is not None and candidate_names != []:
-        for candidate in candidate_names:
-            candidates_list = get_candidate_properties(
-                                candidate,
-                                min_match_score,
-                                id_to_info,
-                                kb,
-                                kb_id_2_id,
-                                candidates_list)
-    
+
+    # Get properties for each retrieved candidate 
+    for candidate in candidate_names: 
+        
+        if candidate["match_score"] > min_match_score \
+                and candidate["kb_id"] != "NIL":
+            
+            if kb != 'ncbi_gene':
+
+                try:
+                    outcount = id_to_info[candidate["kb_id"]][0]
+                    incount = id_to_info[candidate["kb_id"]][1]
+
+                except KeyError:
+                    incount = 0
+                    outcount = 0
+                    
+            else:
+                outcount = 0
+                incount = 0
+            
+            candidate_id = 0
+
+            if candidate["kb_id"] in kb_id_2_id.keys():
+                candidate_id = kb_id_2_id[candidate["kb_id"]]
+            
+            else:
+                # generate random id for current candidate
+                candidate_id = random.randint(0, 1000000)
+                kb_id_2_id[candidate["kb_id"]] = candidate_id
+                
+            # The first candidate in candidate_names 
+            # should be the correct disambiguation for entity
+            candidates_list.append(
+                {"url": candidate["kb_id"], "name": candidate["name"],
+                "outcount": outcount, "incount": incount, "id": candidate_id, 
+                "links": [], "score": candidate["match_score"]})
+            
+        else:
+            less_than_min_score += 1
+   
     return candidates_list, changed_cache, kb_cache_up, kb_id_2_id
 
 
 def check_if_related(c1_url, link_mode, extracted_relations, kb_edges, c2_url):
     """
-    Check if two given knowledge base concepts/candidates are linked according
+    Check if two given knowledge base concepts/candidates are linked according 
     to the criterium defined by link_mode.
 
     :param c1: KB concept/candidate 1
     :type c1: str
     :param c2: KB concept/candidate 2
     :type c2: str
     :param link_mode: how the edges are added to the disambiguation graph ('kb',
     'corpus', 'kb_corpus')
     :type link_mode: str
     :param extracted_relations: relations extracted from target corpus
     :type extracted_relations: list
     :param kb_edges: relations described in the knowledge base
     :type kb_edges: list
-
-    :return: related, is True if the two candidates are related, False
+    
+    :return: related, is True if the two candidates are related, False 
              otherwise
     :rtype: bool
 
     :Example:
     >>> c1 = "ID:01"
     >>> c2 = "ID:02"
     >>> link_mode = "corpus"
-    >>> extracted_relations = {"ID:01": ["ID:02"], "ID:03": ["ID:02"]}
+    >>> extracted_relations = {"ID:01": ["ID:02"], "ID:03": ["ID:02"]} 
     >>> kb_edges = ["ID:04_ID:O5", "ID:06_ID:07"]
     >>> check_if_related(c1, c2, link_mode, extracted_relations, kb_edges)
     True
     """
-
+   
     related = False
 
     if link_mode == "corpus":
         # Check if there is an extracted relation between the two candidates
         if c1_url in extracted_relations:
             relations_with_c1 = extracted_relations[c1_url]
-
-            if c2_url in relations_with_c1:
+                            
+            if c2_url in relations_with_c1: 
                 # Found an extracted relation
                 related = True
 
     else:
-
+        
         if c1_url == c2_url:
             # There is a KB link between the two candidates
             related = True
-
+                        
         else:
-
+            
             if c1_url in kb_edges and c2_url in kb_edges[c1_url]:
                 related = True
 
             else:
 
                 if c2_url in kb_edges and c1_url in kb_edges[c2_url]:
                     related = True
-
+                    
                 else:
                     # There is no KB link between the two candidates
                     # Search in the extracted relations dataset
-
-                    if link_mode == "kb_corpus":
-                        # Maybe there is an extracted relation
+                                                            
+                    if link_mode == "kb_corpus": 
+                        # Maybe there is an extracted relation 
                         # between the two candidates
-
+                                        
                         if c1_url in extracted_relations:
                             relations_with_c1 = extracted_relations[c1_url]
-
-                            if c2_url in relations_with_c1:
+                                    
+                            if c2_url in relations_with_c1: 
                                 # Found an extracted relation
                                 related = True
-
+    
     return related
 
 
 def write_candidates_file(
-    kb,
-    doc_entities_candidates,
-    candidates_dir,
-    entity_type,
-    kb_edges,
-    link_mode,
-    extracted_relations,
-    doc_id,
-):
-    """Generate the candidates file associated with given document according to
+        kb, doc_entities_candidates, candidates_dir, entity_type, kb_edges, 
+        link_mode, extracted_relations, doc_id):
+    """Generate the candidates file associated with given document according to 
     the given entities_candidates dictionary that was previously built.
 
     :param kb: target knowledge base
     :type kb: str
-    :param entities_candidates: includes entities of the given document and
+    :param entities_candidates: includes entities of the given document and 
         respective candidates to output
     :type entities_candidates: dict
-    :param candidates_dir: path to the directory where the candidates file
+    :param candidates_dir: path to the directory where the candidates file 
         will be located
     :type candidates_dir: str
      :param entity_type: the type of the entities that will be linked
     :type entity_type: str
     :param kb_edges: includes the edges between knowledge base concepts in the
         format: (concept_1_id, concept_2_id)
     :type kb_edges: list
-    :param link_mode: specifies the way the edges are built in the
-        disambiguation graphs that are the input of the PPR algorithm
-        ('corpus' - extracted relations from an external corpus,
-        'kb' - relations described in the knowledge base,
+    :param link_mode: specifies the way the edges are built in the 
+        disambiguation graphs that are the input of the PPR algorithm 
+        ('corpus' - extracted relations from an external corpus, 
+        'kb' - relations described in the knowledge base, 
         'kb_corpus' - extracted relations from an external corpus and relations
-        described in the knowledge base,
+        described in the knowledge base, 
     :type link_mode: str
-    :param extracted_relations: includes extracted relations from external
+    :param extracted_relations: includes extracted relations from external 
         dictionary or is empty if link_mode=kb
     :type extracted_relations: list
     """
-
-    candidates_filename = f"{candidates_dir}{doc_id}"
-    candidates_file = open(candidates_filename, "w", encoding="utf-8")
+    
+    candidates_filename = candidates_dir + doc_id
+    candidates_file = open(candidates_filename, 'w')
 
     for annotation1 in doc_entities_candidates:
         entity_str = annotation1[0]
         candidates_file.write(entity_str)
-
+    
         for c1 in annotation1[1]:
-            c1["links"] = ""
+            c1["links"] = ''
 
-            if kb != "ncbi_gene":
+            if kb != 'ncbi_gene':
                 # Find links between the candidates in the current document
-
-                # Get all the candidates for the remaining entities in the
+            
+                # Get all the candidates for the remaining entities in the 
                 # same document
-                other_candidates = [
-                    (c2["url"], c2["id"])
-                    for annotation2 in doc_entities_candidates
-                    if annotation1[0] != annotation2[0]
-                    for c2 in annotation2[1]
-                ]
+                other_candidates = [(c2['url'], c2['id']) for annotation2 in 
+                    doc_entities_candidates if annotation1[0] != annotation2[0] 
+                    for c2 in annotation2[1]]
 
                 # Check if there is a relation between current candidate and each
                 # of the candidates for the remaining entities
-                id_links = [
-                    str(c2[1])
-                    for c2 in other_candidates
-                    if check_if_related(
-                        c1["url"], link_mode, extracted_relations, kb_edges, c2[0]
-                    )
-                ]
+                id_links = [str(c2[1]) for c2 in other_candidates 
+                                if check_if_related( 
+                                    c1['url'], link_mode, 
+                                    extracted_relations, 
+                                    kb_edges, c2[0])]
 
                 # The ids of the candidates are needed instead of the KB ids
                 c1["links"] = ";".join(set(id_links))
 
             candidates_file.write(
-                CANDIDATE_STR.format(
-                    c1["id"],
-                    c1["incount"],
-                    c1["outcount"],
-                    c1["links"],
-                    c1["url"],
-                    c1["name"],
-                    c1["name"].lower(),
-                    c1["name"].lower(),
-                    entity_type,
-                )
-            )
-
+                candidate_string.format(c1["id"], c1["incount"], c1["outcount"], 
+                c1["links"], c1["url"], c1["name"], c1["name"].lower(), 
+                c1["name"].lower(), entity_type))
+                
     candidates_file.close()
```

### Comparing `bent-0.0.55/bent/src/REEL/information_content.py` & `bent-0.0.9/bent/src/REEL/information_content.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,100 @@
 #!/usr/bin/env python
 
 import os
 from math import log
 
 
 def build_term_counts(candidates_dir):
-    """Build a dict containing the frequency of each candidate entity that
+    """Build a dict containing the frequency of each candidate entity that 
     appears in the candidates files generated during the pre-processing stage.
     """
 
     term_counts = {}
 
     candidates_files = os.listdir(candidates_dir)
-
+    
     # Get the term frequency in the corpus
-    for filename in candidates_files:
-
-        lines = open(f"{candidates_dir}{filename}", "r", encoding="utf-8").readlines()
+    for filename in candidates_files: 
 
+        lines = open(candidates_dir + filename, 'r').readlines()
+        
         for line in lines:
 
-            if line[:9] == "CANDIDATE":
-                url = line.split("\t")[5].split("url:")[1]
+            if line[:9] == 'CANDIDATE':
+                url = line.split('\t')[5].split('url:')[1]
 
-                if url not in term_counts:
+                if url not in term_counts.keys():
                     term_counts[url] = 1
-
+                
                 else:
                     term_counts[url] += 1
 
     return term_counts
 
 
 def build_information_content_dict(candidates_dir, id_to_info, mode=None):
-    """Generate dictionary with the information content for each candidate
+    """Generate dictionary with the information content for each candidate 
     term. For more info about the definition of information content see
-    https://www.sciencedirect.com/science/article/pii/B9780128096338204019?via%3Dihub"""
+    https://www.sciencedirect.com/science/article/pii/B9780128096338204019?via%3Dihub""" 
 
     term_counts = build_term_counts(candidates_dir)
-
+    
     ic = {}
     total_terms = 0
 
-    if mode == "intrinsic":
+    if mode == 'intrinsic':
         total_terms = len(id_to_info.keys())
 
-    for term_id in term_counts:
-
+    for term_id in term_counts:        
+        
         term_probability = float()
 
-        if mode == "extrinsic":
+        if mode == 'extrinsic':
             # Frequency of the most frequent term in dataset
-            max_freq = max(term_counts.values())
-            term_frequency = term_counts[term_id]
-            term_probability = (term_frequency + 1) / (max_freq + 1)
-
-        elif mode == "intrinsic":
-
+            max_freq = max(term_counts.values()) 
+            term_frequency = term_counts[term_id] 
+            term_probability = (term_frequency + 1)/(max_freq + 1)
+        
+        elif mode == 'intrinsic':
+            
             try:
                 num_descendants = id_to_info[term_id][2]
                 term_probability = (num_descendants + 1) / total_terms
-
+                
             except:
                 term_probability = 0.000001
 
         else:
-            raise ValueError("Invalid mode!")
-
+            raise ValueError('Invalid mode!')
+        
         information_content = -log(term_probability) + 1
         ic[term_id] = information_content + 1
-
+    
     return ic
 
 
 def generate_ic_file(run_id, candidates_dir, id_to_info):
-    """Generate file with information content of all entities present in the
+    """Generate file with information content of all entities present in the 
     candidates files."""
 
-    ic = build_information_content_dict(candidates_dir, id_to_info, mode="intrinsic")
+    ic = build_information_content_dict(
+        candidates_dir, id_to_info, mode='intrinsic') 
 
     # Build output string
     out_string = str()
 
-    for term in ic:
-        out_string += f"{term}\t{str(ic[term])}\n"
+    for term in ic.keys():
+        out_string += term +'\t' + str(ic[term]) + '\n'
 
-    # Create file ontology_pop with information content for all entities
+    # Create file ontology_pop with information content for all entities 
     # in candidates file
-    out_dir = f".tmp/{run_id}/REEL/"
+    out_dir = ".tmp/{}/REEL/".format(run_id)
 
-    os.makedirs(out_dir, exist_ok=True)
+    if not os.path.exists(out_dir):
+        os.mkdir(out_dir)
 
-    output_file_name = f"{out_dir}ic"
+    output_file_name = out_dir + "ic" 
 
-    with open(output_file_name, "w", encoding="utf-8") as ic_file:
+    with open(output_file_name, 'w') as ic_file:
         ic_file.write(out_string)
-        ic_file.close()
+        ic_file.close()
```

### Comparing `bent-0.0.55/bent/src/REEL/post_process.py` & `bent-0.0.9/bent/src/REEL/post_process.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,81 +5,81 @@
 import os
 
 
 def process_results(run_id, entity_type, kb):
     """Process the results after the application of the PPR-IC model and
     output a JSON file in the directory 'tmp/REEL/results/<run_id>/."""
 
-    if kb != "ncbi_gene":
-        results_filepath = f"{cfg.tmp_dir}{run_id}/REEL/results/candidate_scores"
+    if kb != 'ncbi_gene':
+        results_filepath = '{}{}/REEL/results/candidate_scores'.format(
+            cfg.tmp_dir, run_id)
 
         # Import PPR output
-        with open(results_filepath, "r", encoding="utf-8") as results:
+        with open(results_filepath, 'r') as results:
             data = results.readlines()
-
+            results.close
+    
         linked_entities = {}
-        doc_id = ""
-
+        doc_id = ''
+        
         for line in data:
-
-            if line != "\n":
-
-                if line[0] == "=":
-                    doc_id = line.strip("\n").split(" ")[1]
-
+            
+            if line != '\n':
+                
+                if line[0] == '=':
+                    doc_id = line.strip('\n').split(' ')[1]
+                    
                 else:
-                    entity = line.split("\t")[1].split("=")[1]
-                    answer = (
-                        line.split("\t")[3]
-                        .split("ANS=")[1]
-                        .strip("\n")
-                        .replace("_", ":")
-                    )
-
-                    if doc_id in linked_entities:
+                    entity = line.split('\t')[1].split('=')[1]           
+                    answer = line.split('\t')[3].split('ANS=')[1].strip('\n').\
+                        replace('_', ':')
+            
+                    if doc_id in linked_entities.keys():
                         linked_entities[doc_id][entity] = (answer, entity_type)
-
+                    
                     else:
                         linked_entities[doc_id] = {entity: (answer, entity_type)}
-
-    elif kb == "ncbi_gene":
-        results_filepath = f"{cfg.tmp_dir}{run_id}/REEL/candidates/"
+    
+    elif kb == 'ncbi_gene':
+        results_filepath = cfg.tmp_dir + run_id + '/REEL/candidates/'
         results_files = os.listdir(results_filepath)
         linked_entities = {}
         found_entity = False
 
         for file in results_files:
 
-            with open(results_filepath + file, "r", encoding="utf-8") as results:
+            with open(results_filepath + file, 'r') as results:
                 data = results.readlines()
                 results.close()
-                entity = ""
+                entity = ''
 
                 for line in data:
-
+                    
                     if found_entity:
                         # This is the top candidate
-                        answer = line.split("url:")[1].split("\t")[0].replace("_", ":")
-
+                        answer = line.split('url:')[1].split('\t')[0].\
+                            replace('_', ':')
+                        
                         if file in linked_entities:
-                            linked_entities[file][entity] = (answer, "gene")
-
+                            linked_entities[file][entity] = (answer, 'gene')
+                        
                         else:
-                            linked_entities[file] = {entity: (answer, "gene")}
+                            linked_entities[file] = {entity: (answer, 'gene')}
 
                         found_entity = False
-                        entity = ""
-
+                        entity = ''
+                    
                     else:
 
-                        if line[0] == "E":
-                            entity = line.split("\t")[1].strip("text:")
+                        if line[0] == 'E':
+                            entity = line.split('\t')[1].strip('text:')
                             found_entity = True
-
-    out_dir = f"{cfg.tmp_dir}{run_id}/REEL/results/"
-
-    for doc, doc_results in linked_entities.items():
+    
+    out_dir = '{}{}/REEL/results/'.format(cfg.tmp_dir, run_id)
+    
+    for doc in linked_entities.keys():
+        doc_results = linked_entities[doc]
         out_json = json.dumps(doc_results)
 
-        with open(f"{out_dir}{doc}.json", "wb") as out_file:
+        with open(out_dir + doc + '.json', 'wb') as out_file:
             out_file.write(out_json)
-            out_file.close()
+            out_file.close()
```

### Comparing `bent-0.0.55/bent/src/REEL/ppr_for_ned_all.class` & `bent-0.0.9/bent/src/REEL/ppr_for_ned_all.class`

 * *Files identical despite different names*

### Comparing `bent-0.0.55/bent/src/REEL/ppr_for_ned_all.java` & `bent-0.0.9/bent/src/REEL/ppr_for_ned_all.java`

 * *Files identical despite different names*

### Comparing `bent-0.0.55/bent/src/REEL/pre_process.py` & `bent-0.0.9/bent/src/REEL/pre_process.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,415 +3,386 @@
 import bent.src.cfg as cfg
 import orjson as json
 import os
 import sys
 from bent.src.REEL.candidates import write_candidates_file, generate_candidates_list
 from bent.src.REEL.information_content import generate_ic_file
 from bent.src.NILINKER.predict_nilinker import load_model
-from bent.src.REEL.utils import ENTITY_STR, check_if_candidates_dir
+from bent.src.REEL.utils import entity_string, check_if_candidates_dir
 from bent.src.utils import garbage_collect
 
 sys.path.append("./")
 
 
 def build_entity_candidate_dict(
-    ner_dir,
-    candidates_dir,
-    kb,
-    id_to_info,
-    name_to_id,
-    synonym_to_id,
-    kb_edges,
-    link_mode,
-    extracted_relations,
-    kb_cache,
-    entity_type,
-    abbreviations,
-    min_match_score,
-    nil_mode=None,
-    nilinker=None,
-):
-    """Build a dictionary including the candidates for all entity mentions in
+        ner_dir, candidates_dir, kb, id_to_info, name_to_id, synonym_to_id, 
+        kb_edges, link_mode, extracted_relations, kb_cache, entity_type, 
+        abbreviations, min_match_score, nil_model_name='none', nilinker=None):
+    """Build a dictionary including the candidates for all entity mentions in 
         all the input documents.
 
     :param ner_dir: path to directory where the recognized entities are
         stored in the annotations files
     :type ner_dir: str
     :param kb: target knowledge base
     :type kb: str
     :param id_to_info: mappings between KB identifiers and information
     :type id_to_info: dict
-    :param name_to_id: mappings between each kb concept name and
+    :param name_to_id: mappings between each kb concept name and 
         the respective id
     :type name_to_id: dict
-    :param synonym_to_id: mappings between each synonym for a given kb concept
+    :param synonym_to_id: mappings between each synonym for a given kb concept 
         and the respective id
     :type synonym_to_id: dict
     :param kb_cache: candidates cache for the given kb
     :type kb_cache: dict
     :param entity_type: the type of the entities that will be linked
     :type entity_type: str
-    :param abbreviations: abbreviations with format
+    :param abbreviations: abbreviations with format 
         {'doc_id'':' {'abbv1': 'long_form'}]
     :type abbreviations: dict
-    :param min_match_score: minimum lexical similarity between entity text and
-        candidate text-exclude candidates with a lexical similarity below
+    :param min_match_score: minimum lexical similarity between entity text and 
+        candidate text-exclude candidates with a lexical similarity below 
         min_match_score
     :type min_match_score: float
     :param nil_mode: model to deal with the NIL entities ('none' or 'NILINKER)
     :type nil_mode: str
-    :param nilinker: the loaded NILINKER model if 'nil_mode'='NILINKER,
+    :param nilinker: the loaded NILINKER model if 'nil_mode'='NILINKER, 
         defaults to None
     :type nilinker: _type_, optional
 
-    :return: entities_candidates (dict) with format
-        {doc_id':' {mention:[candidate1, ...]} }, changed_cache_final (bool)
+    :return: entities_candidates (dict) with format 
+        {doc_id':' {mention:[candidate1, ...]} }, changed_cache_final (bool) 
         indicating wether the candidates cache has been updated comparing with
-        preivous execution of the script, and kb_cache_up (dict), which
-        corresponds to the candidates cache for given KB, updated or not
+        preivous execution of the script, and kb_cache_up (dict), which 
+        corresponds to the candidates cache for given KB, updated or not 
         according to the value of changed_cache
     :rtype: tuple with dict, bool, dict
     """
-
+    
     doc_count = 0
     changed_cache_final = False
     kb_cache_up = None
     names = set(name_to_id.keys())
     synonyms = set(synonym_to_id.keys())
-    ner_out_docs = os.listdir(ner_dir)
 
+    ner_out_docs = os.listdir(ner_dir)
+    
     for doc in ner_out_docs:
         ner_annots = None
-        doc_id = doc.strip(".ann")
+        doc_id = doc.strip('.ann')
 
-        with open(f"{ner_dir}{doc}", "r", encoding="utf-8") as ner_doc:
+        with open(ner_dir + doc, 'r') as ner_doc:
             ner_annots = ner_doc.readlines()
             ner_doc.close()
-
-        doc_count += 1
+        
+        doc_count += 1 
         check_entity = []
         doc_entities_final = []
         doc_abbrvs = {}
-
+        
         if doc_id in abbreviations:
             doc_abbrvs = abbreviations[doc_id]
 
         kb_id_2_id = {}
-
+        
         for line in ner_annots:
-            annot_type = ""
-            entity_text = ""
+            annot_type = ''
+            entity_text = ''
 
-            if line != "\n":
-                line_data = line.split("\t")
-                annot_type = line_data[1].split(" ")[0]
-                entity_text = line_data[2].strip("\n")
-
-            if (
-                annot_type.lower() == entity_type.lower()
-                and entity_text not in check_entity
-            ):
+            if line != '\n':
+                line_data = line.split('\t')
+                annot_type = line_data[1].split(' ')[0]
+                entity_text = line_data[2].strip('\n')
+            
+            if annot_type.lower() == entity_type.lower() \
+                    and entity_text not in check_entity:
                 # Only disambiguate entities belonging to the same given
                 # entity type
-                # Repeated instances of the same entity in a document
+                # Repeated instances of the same entity in a document 
                 # are not considered
                 check_entity.append(entity_text)
                 
                 # Get candidates list for entity
-                candidates_list, changed_cache, kb_cache_up, kb_id_2_id = (
-                    generate_candidates_list(
-                        entity_text,
-                        kb,
-                        id_to_info,
-                        names,
-                        synonyms,
-                        name_to_id,
-                        synonym_to_id,
-                        kb_cache,
-                        min_match_score,
-                        doc_abbrvs,
-                        kb_id_2_id,
-                    )
-                )
-
+                candidates_list, \
+                    changed_cache, \
+                    kb_cache_up, \
+                    kb_id_2_id = generate_candidates_list(
+                                                    entity_text, 
+                                                    kb, 
+                                                    id_to_info, 
+                                                    names,
+                                                    synonyms,
+                                                    name_to_id, 
+                                                    synonym_to_id,  
+                                                    kb_cache,  
+                                                    min_match_score,
+                                                    doc_abbrvs,
+                                                    kb_id_2_id)
+                
                 if changed_cache:
-                    # There is at least 1 change in the cache file
+                    #There is at least 1 change in the cache file
                     changed_cache_final = True
 
-                if len(candidates_list) == 0:
-
-                    if nil_mode is not None:
+                if len(candidates_list) == 0: 
+                    
+                    if nil_model_name != 'none':
                         # The model will try to disambiguate the NIL entity
                         top_candidates_up = []
 
-                        if nil_mode == "NILINKER":
+                        if nil_model_name == 'NILINKER':
                             # Find top-k candidates with NILINKER and include
                             # them in the candidates file
-                            top_candidates = nilinker.prediction(entity_text)
-
+                            top_candidates = nilinker.prediction(
+                                                entity_text)
+                                    
                         for cand in top_candidates:
                             kb_id = cand[0]
 
-                            if nil_mode == "NILINKER":
+                            if nil_model_name == 'NILINKER':
                                 kb_id = cand[0].replace(":", "_")
-
-                            cand_up = {
-                                "kb_id": kb_id,
-                                "name": cand[1],
-                                "match_score": 1.0,
-                            }
-
+                        
+                            cand_up = {'kb_id': kb_id , 
+                                        'name': cand[1],
+                                        'match_score': 1.0}
+                            
                             top_candidates_up.append(cand_up)
-
-                        candidates_list, changed_cache, kb_cache_up, kb_id_2_id = (
-                            generate_candidates_list(
-                                entity_text,
-                                kb,
-                                id_to_info,
-                                names,
-                                synonyms,
-                                name_to_id,
-                                synonym_to_id,
-                                kb_cache,
-                                min_match_score,
-                                doc_abbrvs,
-                                kb_id_2_id,
-                                nil_candidates=top_candidates_up,
-                            )
-                        )
-
-                    elif nil_mode is None:
+                        
+                        candidates_list, \
+                            changed_cache, \
+                            kb_cache_up, \
+                            kb_id_2_id = generate_candidates_list(
+                                            entity_text, 
+                                            kb, 
+                                            id_to_info, 
+                                            names, 
+                                            synonyms,
+                                            name_to_id, 
+                                            synonym_to_id, 
+                                            kb_cache, 
+                                            min_match_score, 
+                                            doc_abbrvs, 
+                                            kb_id_2_id,
+                                            nil_candidates=top_candidates_up)
+                    
+                    elif nil_model_name == 'none':
                         # Since nil entities are not disambiguated,
                         # create a dummy candidate
                         candidates_list = [
-                            {
-                                "url": "NIL",
-                                "name": "none",
-                                "outcount": 0,
-                                "incount": 0,
-                                "id": -1,
-                                "links": [],
-                                "score": 0,
-                            }
-                        ]
-
-                entity_str = ENTITY_STR.format(
-                    entity_text,
-                    entity_text.lower(),
-                    entity_type,
-                    doc_count,
-                    doc_id,
-                    "unknown",
-                )
-
+                            {'url': 'NIL', 
+                            'name': 'none', 
+                            'outcount': 0, 
+                            'incount': 0, 
+                            'id': -1, 'links': [], 
+                            'score': 0}]
+                        
+                entity_str = entity_string.format(
+                    entity_text, entity_text.lower(), entity_type, 
+                    doc_count, doc_id, 'unknown')
+                
                 add_entity = [entity_str, candidates_list]
 
                 doc_entities_final.append(add_entity)
 
                 del candidates_list
 
         if doc_entities_final != []:
-            # In this document there is at least 1 entity
-            # ------------------------------------------------------------------
+            #In this document there is at least 1 entity
+            #------------------------------------------------------------------
             #                        Generate candidates files
-            # ------------------------------------------------------------------
+            #------------------------------------------------------------------
             write_candidates_file(
-                kb,
-                doc_entities_final,
-                candidates_dir,
-                entity_type,
-                kb_edges,
-                link_mode,
-                extracted_relations,
-                doc_id,
-            )
-
+                kb, doc_entities_final, candidates_dir, entity_type, kb_edges, 
+                link_mode, extracted_relations, doc_id)
+        
         del doc_abbrvs
         del doc_entities_final
         del kb_id_2_id
-
+     
     del names
     del synonyms
-
+   
     return changed_cache_final, kb_cache_up
+    
 
-
-def pre_process(run_id, ner_dir, kb, entity_type, link_mode, nil_mode, abbreviations):
-    """Execute all pre-processing steps that are necessary to create the
-        candidate files, which will be the input for the PPR algorithm. The
-        candidate files will be located in the directory
+def pre_process(
+        run_id, ner_dir, kb, entity_type, link_mode, nil_mode, abbreviations):
+    """Execute all pre-processing steps that are necessary to create the 
+        candidate files, which will be the input for the PPR algorithm. The 
+        candidate files will be located in the directory 
         'tmp/REEL/candidates/<run_id>'.
 
     :param run_id: representing the identifier of the current run of REEL
     :type run_id: str
     :param ner_dir: path to directory where the recognized entities are
         stored in the annotations files
     :type ner_dir: str
     :param kb: target knowledge base
     :type kb: str
     :param entity_type: the type of the entities that will be linked
     :type entity_type: str
-    :param link_mode: specifies the way the edges are built in the
-        disambiguation graphs that are the input of the PPR algorithm
-        ('corpus' - extracted relations from an external corpus,
-        'kb' - relations described in the knowledge base,
+    :param link_mode: specifies the way the edges are built in the 
+        disambiguation graphs that are the input of the PPR algorithm 
+        ('corpus' - extracted relations from an external corpus, 
+        'kb' - relations described in the knowledge base, 
         'kb_corpus' - extracted relations from an external corpus and relations
-        described in the knowledge base,
+        described in the knowledge base, 
     :type link_mode: str
     :param nil_mode: model to deal with the NIL entities ('none' or 'NILINKER)
     :type nil_mode: str
-    param abbreviations: abbreviations with format:
+    param abbreviations: abbreviations with format: 
         {'doc_id': {'abbv1': 'long_form'}]
     :type abbreviations: dict
     """
 
-    # -------------------------------------------------------------------------
+    #-------------------------------------------------------------------------
     #                          Create directories
-    # -------------------------------------------------------------------------
-    os.makedirs(cfg.tmp_dir, exist_ok=True)
-    os.makedirs(f"{cfg.tmp_dir}{run_id}", exist_ok=True)
-    os.makedirs(f"{cfg.tmp_dir}REEL/", exist_ok=True)
-    os.makedirs(f"{cfg.tmp_dir}REEL/cache/", exist_ok=True)
-    os.makedirs(f"{cfg.tmp_dir}{run_id}/REEL/", exist_ok=True)
-    os.makedirs(f"{cfg.tmp_dir}{run_id}/REEL/candidates", exist_ok=True)
-    os.makedirs(f"{cfg.tmp_dir}{run_id}/REEL/results/", exist_ok=True)
-
-    # -------------------------------------------------------------------------
+    #-------------------------------------------------------------------------
+    if not os.path.exists(cfg.tmp_dir):
+        os.mkdir(cfg.tmp_dir)
+
+    if not os.path.exists(cfg.tmp_dir + run_id):
+        os.mkdir(cfg.tmp_dir + run_id)
+
+    if not os.path.exists(cfg.tmp_dir + 'REEL/'):
+        os.mkdir(cfg.tmp_dir + 'REEL/')
+
+    if not os.path.exists(cfg.tmp_dir + 'REEL/cache/'):
+        os.mkdir(cfg.tmp_dir + 'REEL/cache/')
+
+    os.mkdir('{}{}/REEL/'.format(cfg.tmp_dir, run_id))
+    os.mkdir('{}{}/REEL/candidates'.format(cfg.tmp_dir, run_id))
+    os.mkdir('{}{}/REEL/results/'.format(cfg.tmp_dir, run_id))
+    
+    #-------------------------------------------------------------------------
     #                            Import KB info
-    # -------------------------------------------------------------------------
+    #-------------------------------------------------------------------------
 
     # Load preprocessed dicts
     name_to_id = {}
     synonym_to_id = {}
-    kb_dicts_dir = f"{cfg.root_path}/data/kbs/dicts/{kb}/"
-
-    with open(f"{kb_dicts_dir}name_to_id.json", "r", encoding="utf-8") as dict_file:
+    kb_dicts_dir = '{}data/dicts/{}/'.format(cfg.root_path, kb) 
+    
+    with open(kb_dicts_dir + 'name_to_id.json', 'r') as dict_file:
         name_to_id = json.loads(dict_file.read())
         dict_file.close()
 
-    synonyms_filepath = f"{kb_dicts_dir}synonym_to_id_full.json"
+    synonyms_filepath = kb_dicts_dir + 'synonym_to_id_full.json'
 
-    if "synonym_to_id_full.json" not in os.listdir(kb_dicts_dir):
-        synonyms_filepath = f"{kb_dicts_dir}synonym_to_id.json"
-
-    with open(synonyms_filepath, "r", encoding="utf-8") as dict_file2:
+    if 'synonym_to_id_full.json' not in os.listdir(kb_dicts_dir):
+        synonyms_filepath = kb_dicts_dir + 'synonym_to_id.json'
+    
+    with open(synonyms_filepath, 'r') as dict_file2:
         synonym_to_id = json.loads(dict_file2.read())
-        dict_file2.close()
+        dict_file2.close()    
 
     id_to_info = None
+    
+    if kb != 'ncbi_gene':
+        id_to_info_filepath = kb_dicts_dir + 'id_to_info.json'
 
-    if kb != "ncbi_gene":
-        id_to_info_filepath = f"{kb_dicts_dir}id_to_info.json"
-
-        with open(id_to_info_filepath, "r", encoding="utf-8") as dict_file3:
+        with open(id_to_info_filepath, 'r') as dict_file3:
             id_to_info = json.loads(dict_file3.read())
-            dict_file3.close()
+            dict_file3.close()  
 
-    # -------------------------------------------------------------------------
+    #-------------------------------------------------------------------------
     #                  Import cache file (if available)
-    # -------------------------------------------------------------------------
-    kb_cache_filename = f"{cfg.tmp_dir}/REEL/cache/{kb}.json"
+    #-------------------------------------------------------------------------
+    kb_cache_filename = '{}/REEL/cache/{}.json'.format(cfg.tmp_dir, kb)
     kb_cache = {}
 
     if os.path.exists(kb_cache_filename):
-        cache_file = open(kb_cache_filename, "r", encoding="utf-8")
+        cache_file = open(kb_cache_filename, 'r')
         kb_cache = json.loads(cache_file.read())
         cache_file.close()
 
     changed_cache_final = False
-
-    # -------------------------------------------------------------------------
+    
+    #-------------------------------------------------------------------------
     #                            Load NILINKER
-    # -------------------------------------------------------------------------
-    if nil_mode == "NILINKER":
+    #-------------------------------------------------------------------------
+    if nil_mode == 'NILINKER':
         # Prepare NILINKER and get compiled model ready to predict
         # top_k defines the number of candidates that NILINKER wil return
         # for each given entity
         top_k = 1
         nilinker = load_model(kb, top_k=int(top_k))
-
+      
     else:
         nilinker = None
-
-    # -------------------------------------------------------------------------
+    
+    #-------------------------------------------------------------------------
     #            Import relations to add to the disambiguation graphs
-    # -------------------------------------------------------------------------
+    #-------------------------------------------------------------------------
     extracted_relations = {}
-
-    if link_mode == "corpus" or link_mode == "kb_corpus":
-        relations_dir = f"{cfg.root_path}/data/relations/"
-        rel_filenames = os.listdir(relations_dir)
-        rel_filename = f"{entity_type}_{kb}_relations.json"
+    
+    if link_mode == 'corpus' or link_mode == 'kb_corpus': 
+        relations_dir = '{}data/relations/'.format(cfg.root_path)
+        rel_filenames = os.listdir(relations_dir)    
+        rel_filename = '{}_{}_relations.json'.format(entity_type, kb)
 
         if rel_filename in rel_filenames:
 
-            with open(f"{relations_dir}{rel_filename}", "r", encoding="utf-8") as rel_file:
+            with open(relations_dir + rel_filename, 'r') as rel_file:
                 extracted_relations = json.loads(rel_file.read())
                 rel_file.close()
-
+  
     candidates_dir = check_if_candidates_dir(run_id)
 
     kb_edges = []
-
-    if kb != "ncbi_gene":
-        edges_filepath = f"{kb_dicts_dir}node_to_node.json"
-
-        with open(edges_filepath, "r", encoding="utf-8") as dict_file4:
+    
+    if kb != 'ncbi_gene':
+        edges_filepath = kb_dicts_dir + 'node_to_node.json'
+        
+        with open(edges_filepath, 'r') as dict_file4:
             kb_edges = json.loads(dict_file4.read())
-            dict_file4.close()
+            dict_file4.close() 
 
-    # -------------------------------------------------------------------------
+    #-------------------------------------------------------------------------
     #                   Build candidates lists for the entities
-    # -------------------------------------------------------------------------
-
-    # Min lexical similarity between entity text and candidate text:
+    #-------------------------------------------------------------------------
+    
+    # Min lexical similarity between entity text and candidate text: 
     # exclude candidates with a lexical similarity below min_match_score
-    min_match_score = 0.0
-
+    min_match_score = 0.0 
+    
     # Prepare dataset for candidate generation
-    changed_cache_final, kb_cache_up = build_entity_candidate_dict(
-        ner_dir,
-        candidates_dir,
-        kb,
-        id_to_info,
-        name_to_id,
-        synonym_to_id,
-        kb_edges,
-        link_mode,
-        extracted_relations,
-        kb_cache,
-        entity_type,
-        abbreviations,
-        min_match_score,
-        nil_mode=nil_mode,
-        nilinker=nilinker,
-    )
-
+    changed_cache_final, \
+            kb_cache_up = build_entity_candidate_dict(
+                            ner_dir, candidates_dir, 
+                            kb, id_to_info, name_to_id, 
+                            synonym_to_id, 
+                            kb_edges, link_mode, extracted_relations,
+                            kb_cache, entity_type, abbreviations, 
+                            min_match_score, nil_model_name=nil_mode,
+                            nilinker=nilinker)
+    
     del nilinker
     del name_to_id
     del synonym_to_id
 
     if changed_cache_final:
         cache_out = json.dumps(kb_cache_up)
-
-        with open(kb_cache_filename, "wb") as cache_out_file:
+    
+        with open(kb_cache_filename, 'wb') as cache_out_file:
             cache_out_file.write(cache_out)
             cache_out_file.close()
 
         del cache_out
-
+    
     del kb_cache_up
     del kb_cache
     del extracted_relations
     del kb_edges
-    # -------------------------------------------------------------------------
+    #-------------------------------------------------------------------------
     #                  Generate Information content file
-    # -------------------------------------------------------------------------
-
+    #-------------------------------------------------------------------------
+        
     # INTRINSIC INFORMATION CONTENT:
-    # Create information content file including every KB concept appearing
-    # in candidates files
-    if kb != "ncbi_gene":
+    # Create information content file including every KB concept appearing 
+    # in candidates files 
+    if kb != 'ncbi_gene':
         generate_ic_file(run_id, candidates_dir, id_to_info)
 
     # Free up memory usage
-    del id_to_info
+    del id_to_info
+    garbage_collect()
```

### Comparing `bent-0.0.55/bent/src/REEL/run.py` & `bent-0.0.9/bent/src/REEL/run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,74 @@
 #!/usr/bin/env python
-import os
+
 import bent.src.cfg as cfg
+import os
+import random
+import string
 from bent.src.REEL.pre_process import pre_process
 from bent.src.REEL.post_process import process_results
 
 
-def run(run_id, ner_dir, kb, entity_type, abbreviations, nil_mode=None):
-    """Apply the REEL model (preprocess, candidate scoring with PPR,
+def run(ner_dir, kb, entity_type, abbreviations):
+    """Apply the REEL model (preprocess, candidate scoring with PPR, 
     postprocess) to the entities present in files in ner_dir.
 
     :param ner_dir: path to directory where the recognized entities are
         stored in the annotations files
     :type ner_dir: str
     :param kb: target knowledge base
     :type kb: str
     :param entity_type: the type of the entities that will be linked
     :type entity_type: str
-    :param abbreviations: abbreviations with format:
+    :param abbreviations: abbreviations with format: 
         {'doc_id': {'abbv1': 'long_form'}]
     :type abbreviations: dict
     :return: nel_run_id representing the identifier of the current run of REEL.
-        The results of the run will be located in the directory
+        The results of the run will be located in the directory 
         'tmp/REEL/results/<run_id/>'.
     :rtype: str
     """
 
-    nel_run_name = f"{run_id}/{entity_type}"
+    nel_run_id = ''.join(random.choices(string.ascii_uppercase + string.digits, 
+        k=15))
+    nel_run_name = nel_run_id + '_' + entity_type
 
-    # Use relations extracted from external corpora and relations described in
+    # Use relations extracted from external corpora and relations described in 
     # the targer knowledge base
-    link_mode = "kb_corpus"
+    link_mode='kb_corpus' 
 
     # Use NILINKER model if available
-    if nil_mode:
-        #TODO: implement efficient NILINKER-ctd_chem model
-        available_kbs_nilinker = ["chebi", "medic", "go_bp", "hp"]
-        
-        if kb in available_kbs_nilinker:
-            nil_mode = "NILINKER"
-    # -------------------------------------------------------------------------#
-    #                        REEL: PRE_PROCESSING
-    #        Pre-processes the corpus to create a candidates file for each
-    #        document in dataset to allow further building of the
-    #        disambiguation graph.
-    # -------------------------------------------------------------------------#
-    pre_process(
-        nel_run_name, ner_dir, kb, entity_type, link_mode, nil_mode, abbreviations
-    )
-
-    # ------------------------------------------------------------------------#
-    #                          REEL: PPR
-    #         Builds a disambiguation graph from each candidates file:
-    #         the nodes are the candidates and relations are added
-    #         according to candidate link_mode. After the disambiguation
-    #         graph is built, it runs the PPR algorithm over the graph
-    #         and ranks each candidate.
-    # ------------------------------------------------------------------------#
-    if kb != "ncbi_gene":
-        ppr_dir = f"{cfg.root_path}/src/REEL/"
-        comm = f"java -classpath :{ppr_dir} ppr_for_ned_all {nel_run_name} ppr_ic"
+    nil_mode = 'none'
+    available_kbs_nilinker = [
+        'chebi', 'ctd_chem', 'medic', 'go_bp', 'hp']
+
+    if kb in available_kbs_nilinker:
+        nil_mode = 'NILINKER'
+    #-------------------------------------------------------------------------#
+    #                        REEL: PRE_PROCESSING                             
+    #        Pre-processes the corpus to create a candidates file for each     
+    #        document in dataset to allow further building of the              
+    #        disambiguation graph.                                             
+    #-------------------------------------------------------------------------#
+    pre_process(nel_run_name, ner_dir, kb, entity_type, link_mode, nil_mode, 
+        abbreviations)
+   
+    #------------------------------------------------------------------------#
+    #                          REEL: PPR                                     
+    #         Builds a disambiguation graph from each candidates file:            
+    #         the nodes are the candidates and relations are added                
+    #         according to candidate link_mode. After the disambiguation          
+    #         graph is built, it runs the PPR algorithm over the graph            
+    #         and ranks each candidate.                                           
+    #------------------------------------------------------------------------#
+    if kb != 'ncbi_gene':
+        ppr_filepath = '{}scripts/'.format(cfg.root_path)
+        comm = 'java -classpath :{} ppr_for_ned_all {} ppr_ic'.\
+            format(ppr_filepath, nel_run_name)
         os.system(comm)
 
-    # ------------------------------------------------------------------------#
-    #                         REEL: Post-processing
-    # ------------------------------------------------------------------------#
+    #------------------------------------------------------------------------#
+    #                         REEL: Post-processing                                                                      
+    #------------------------------------------------------------------------# 
     process_results(nel_run_name, entity_type, kb)
-
-    return nel_run_name
+    
+    return nel_run_name
```

### Comparing `bent-0.0.55/bent/src/abbreviation_detector/run.py` & `bent-0.0.9/bent/src/abbreviation_detector/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,81 +11,84 @@
     :param filepaths: paths of the files that were outputted by Ab3P
     :type filepaths: list
     :return: abbreviations with format: {'doc_id': {'abbv1': 'long_form'}]
     :rtype: dict
     """
 
     abbreviations = {}
-    doc_id = ""
-
+    doc_id = ''
+    
     for filepath in filepaths:
         doc_abbrvs = {}
-
-        if ".txt" in filepath or ".ann" in filepath:
+       
+        if '.txt' in filepath or '.ann' in filepath:
             doc_id = filepath[:-4]
-
+        
         else:
             doc_id = filepath
 
-        filepath_up = f"tmp/{doc_id}_abbrvs"
-
-        with open(filepath_up, "r", encoding="utf-8") as out_file:
+        filepath_up = 'tmp/{}_abbrvs'.format(doc_id)
+        
+        with open(filepath_up, 'r') as out_file:
             data = out_file.readlines()
             out_file.close()
-
+            
             for line in data:
 
-                if line[0] == " ":
-                    line_data = line.split("|")
-
+                if line[0] == ' ': 
+                    line_data = line.split('|')
+                    
                     if len(line_data) == 3:
                         score = float(line_data[2])
 
                         if score >= 0.90:
-                            doc_abbrvs[line_data[0].strip(" ")] = line_data[1]
+                            doc_abbrvs[line_data[0].strip(' ')] = line_data[1]
 
         # Remove the generated txt files
-        comm1 = f"rm {filepath_up}"
+        comm1 = 'rm {}'.format(filepath_up)
         os.system(comm1)
-
+        
         abbreviations[doc_id] = doc_abbrvs
-
+    
     # Return to the original dir
     os.chdir(initial_dir)
 
     return abbreviations
 
 
 def run_Ab3P(input_dir):
-    """Apply the abbreviation detector Ab3P in the texts located in input_dir.
+    """Apply the abbreviation detector Ab3P in the texts located in input_dir. 
 
-    :param input_dir: path to the directory including the texts of the
+    :param input_dir: path to the directory including the texts of the 
         documents where the entities were recognized
     :type input_dir: str
     :return: abbreviations with format: {'doc_id': {'abbv1': 'long_form'}]
     :rtype: dict
     """
 
     filepaths = [file for file in os.listdir(input_dir)]
 
     # change to Ab3P directory
     cwd = os.getcwd()
-    os.chdir(cfg.root_path + "/abbreviation_detector/Ab3P/")
-    os.makedirs("tmp/", exist_ok=True)
+    os.chdir(cfg.root_path + 'scripts/abbreviation_detector/Ab3P/')
+
+    if not os.path.exists('tmp/'):
+        os.mkdir('tmp/')
 
     # Run Ab3P for each text file
     for filepath in filepaths:
-        doc_id = ""
+        doc_id = ''
 
-        if ".txt" in filepath or ".ann" in filepath:
+        if '.txt' in filepath or '.ann' in filepath:
             doc_id = filepath[:-4]
-
+        
         else:
             doc_id = filepath
 
-        comm = f"./identify_abbr ../../../{input_dir}{filepath} 2> /dev/null >> tmp/{doc_id}_abbrvs"
+        comm = './identify_abbr ../../../{}{} 2> /dev/null >> tmp/{}_abbrvs'.format(
+            input_dir, filepath, doc_id)
         os.system(comm)
-
+    
     # Return to the original dir
-    # os.chdir('../../../')
+    #os.chdir('../../../')
 
-    return parse_Ab3P_output(filepaths, cwd)
+    return parse_Ab3P_output(filepaths, cwd)
```

### Comparing `bent-0.0.55/bent/src/dicts/annotations/dataset_entities.py` & `bent-0.0.9/bent/src/setup/annotations/dataset_entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     return pubtator_annots
 
 
 def get_annotations_from_brat(filename, ent_type):
 
     brat_annots = {}
 
-    with open(filename, 'r', encoding="utf-8") as ann_file:
+    with open(filename, 'r') as ann_file:
         annotations = ann_file.readlines()
         entity_tmp = ''
         found_entity = False
         kb_id = ''
 
         for line in annotations:
 
@@ -67,22 +67,22 @@
                 else:
                     found_entity = False
 
         ann_file.close()
 
     found_entity = False
 
-    return brat_annots
+    return brat_annots 
 
 
 def get_annotations_from_craft(filename):
 
     craft_annots = {}
 
-    with open(filename, 'r', encoding="utf-8") as ann_file:
+    with open(filename, 'r') as ann_file:
         annotations = ann_file.readlines()
 
         for line in annotations:
             
             try:
                 line_data = line.split('\t')
                 kb_id = line_data[1].split(' ')[0].replace(':', '_')
@@ -102,14 +102,15 @@
 def build_annotations_dict(corpora_dir, dicts_dir, kb):
 
     entity_2_kb_id = {}
 
     # ------------------------------------------------------------------------
     #                       Import useful data from corpora
     # ------------------------------------------------------------------------
+    
     #-------------------------- NCBI TAXON -----------------------------------
     if kb == 'ncbi_taxon':
 
         # CRAFT-NCBITaxon
         corpora_dir += 'CRAFT-4.0.1/concept-annotation/NCBITaxon/NCBITaxon/brat/'
         craft_files = os.listdir(corpora_dir)
 
@@ -279,80 +280,80 @@
             if filename[-3:] == 'ann':
                 file_annots = get_annotations_from_craft(corpora_dir + filename)
                 entity_2_kb_id = {**entity_2_kb_id, **file_annots}
 
     # ------------------------------------------------------------------------
     # Filter out the annotations that have an exact match in the target KB
     # ------------------------------------------------------------------------
-    with open(f"{dicts_dir}{kb}/name_to_id.json", 'r', encoding="utf-8") as dictfile1:
+    with open(dicts_dir + '{}/name_to_id.json'.format(kb), 'r') as dictfile1:
         name_to_id = json.load(dictfile1)
         dictfile1.close()
     
-    with open(f"{dicts_dir}{kb}/synonym_to_id.json", 'r', encoding="utf-8") as dictfile2:
+    with open(dicts_dir + '{}/synonym_to_id.json'.format(kb), 'r') as dictfile2:
         synonym_to_id = json.load(dictfile2)
         dictfile2.close()
 
     alt_id_to_id = {}
 
     if os.path.exists(dicts_dir + '{}/alt_id_to_id.json'):
-        with open(f"{dicts_dir}{kb}/alt_id_to_id.json", 'r', encoding="utf-8") as dictfile3:
+        with open(dicts_dir + '{}/alt_id_to_id.json'.format(kb), 'r') as dictfile3:
             alt_id_to_id = json.load(dictfile3)
             dictfile3.close()
         
     #with open(dicts_dir + '{}/id_to_name.json'.format(kb), 'r') as dictfile4:
     #    id_to_name = json.load(dictfile4)
     #    dictfile4.close()
-    with open(f"{dicts_dir}{kb}/id_to_info.json", 'r', encoding="utf-8") as dictfile4:
+    with open(dicts_dir + '{}/id_to_info.json'.format(kb), 'r') as dictfile4:
         id_to_info = json.load(dictfile4)
         dictfile4.close()
 
     to_delete = []
 
     for entity in entity_2_kb_id.keys():
 
         if entity in name_to_id or entity in synonym_to_id:
-            to_delete.append(entity)
-            
+            to_delete.append(entity) 
+
         kb_id = entity_2_kb_id[entity]
         
         if kb_id in alt_id_to_id.keys():
             kb_id = alt_id_to_id[kb_id]
             entity_2_kb_id[entity] = kb_id
        
         if kb_id not in id_to_info.keys() and kb != 'ncbi_taxon':
             to_delete.append(entity)
     
-    to_delete_up = list(set(to_delete))
+    to_delete_up = [entity for entity in set(to_delete)]
     
     for entity in to_delete_up:
         del entity_2_kb_id[entity]
 
     # ------------------------------------------------------------------------
     #     Concatenate the generated dict with the respective synonym_to_id
     # ------------------------------------------------------------------------
 
-    synonyms_filepath = f"{dicts_dir}{kb}/synonym_to_id.json"
+    synonyms_filepath = dicts_dir + '{}/synonym_to_id.json'.format(kb)
     
-    with open(synonyms_filepath, "r", encoding="utf-8") as synonyms_file:
+    with open(synonyms_filepath, 'r') as synonyms_file:
         synonym_to_id = json.load(synonyms_file)
         synonyms_file.close()
    
     output_dict = {**synonym_to_id, **entity_2_kb_id}
     
     output = json.dumps(output_dict, indent=4, ensure_ascii=False)
-    out_filename = f"{dicts_dir}{kb}/synonym_to_id_full.json"
+    out_filename = dicts_dir + '{}/synonym_to_id_full.json'.format(kb)
 
-    with open(out_filename, "w", encoding="utf-8") as out_file:
+    with open(out_filename, 'w') as out_file:
         out_file.write(output)
         out_file.close()
 
 
 def generate_annotation_dicts():
-    corpora_dir = cfg.root_path + '/data/datasets/'
-    dicts_dir = cfg.root_path + '/data/kbs/dicts/'
+    corpora_dir = cfg.root_path + 'data/datasets/'
+    dicts_dir = cfg.root_path + 'data/kbs/dicts/'
 
     kbs = ['ncbi_taxon', 'medic', 'ctd_chem', 'chebi', 'go_bp', 'ncbi_gene',
         'go_cc', 'cl', 'uberon']
     #kbs = ['medic']
 
     for kb in kbs:
         build_annotations_dict(corpora_dir, dicts_dir, kb)
```

### Comparing `bent-0.0.55/bent/src/dicts/kb/generate_dicts.py` & `bent-0.0.9/bent/src/setup/kb/generate_dicts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python
 
 import bent.src.cfg as cfg
 import orjson as json
 import os
-from bent.src.dicts.kb.kb import KnowledgeBase
+from bent.src.setup.kb.kb import KnowledgeBase
 
-dict_dir = cfg.root_path + '/data/kbs/dicts/'
+dict_dir = cfg.root_path + 'data/dicts/'
 
 
 def generate_dicts_4_kb(kb=None, mode='reel', terms_filename=None, 
         edges_filename=None, kb_filename=None, input_format=None):
     
     out_dir = dict_dir + kb 
 
-    os.makedirs(out_dir, exist_ok=True)
+    if not os.path.exists(out_dir):
+        os.mkdir(out_dir)
 
     kb_obj = KnowledgeBase(kb, mode, terms_filename=terms_filename, 
         edges_filename=edges_filename, input_format=input_format)
     
     if mode == 'reel':
         name_to_id = json.dumps(kb_obj.name_to_id)
```

### Comparing `bent-0.0.55/bent/src/dicts/kb/kb.py` & `bent-0.0.9/bent/src/setup/kb/kb.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 objects (dictionaries and Networkx graph)."""
 
 import csv
 import networkx as nx
 import obonet
 import bent.src.cfg as cfg
 
-data_dir = cfg.root_path + '/data/kbs/original_files/'
+data_dir = cfg.root_path + 'data/kbs/original_files/'
 
 
 class KnowledgeBase:
     """Represents a knowledge base that is loaded from a given local file."""
 
     def __init__(self, kb, mode, terms_filename=None, edges_filename=None, 
             kb_filename=None, input_format=None):
@@ -67,15 +67,17 @@
                 self.load_obo()
                 
             elif self.kb in self.tsv_file or self.input_format == 'tsv':
                 self.load_tsv()
                     
             elif self.kb == 'ncbi_taxon':
                 self.load_ncbi_taxon()
-     
+            #elif self.kb in self.csv_file or self.input_format == 'csv':
+            #    self.load_csv()
+            
             elif self.kb == 'ncbi_gene':
                 self.load_ncbi_gene()
             
             else:
                  
                 if self.input_format == 'txt':
                     self.load_txt()
@@ -96,19 +98,19 @@
         filepaths = {'medic': 'CTD_diseases', 'chebi': 'chebi', 
                         'go_bp': 'go-basic', 'go_cc': 'go-basic', 
                         'do': 'doid', 'hp': 'hp',
                         'cellosaurus': 'cellosaurus', 'cl': 'cl-basic',
                         'uberon': 'uberon-basic'
                         }
 
-        if self.kb in filepaths:
+        if self.kb in filepaths.keys():
             filepath += filepaths[self.kb] + '.obo' 
        
         else:
-            filepath += self.kb_filename
+            filepath += + self.kb_filename
         
         name_to_id = {}
         id_to_name = {}
         id_to_info = {}
         synonym_to_id = {}
         child_to_parent = {}
         alt_id_to_id = {}
@@ -116,21 +118,21 @@
 
         graph = obonet.read_obo(filepath)
         edges = []
         
         for node in  graph.nodes(data=True):
             add_node = False
             
-            if "name" in node[1]:
+            if "name" in node[1].keys():
                 node_id, node_name = node[0], node[1]["name"]
 
                 if self.mode == 'reel':
                     node_id = node_id.replace(':', '_')
                 
-                if self.kb == "go_bp":
+                if self.kb == "go_bp": 
                     # For go_bp, ensure that only Biological Process 
                     # concepts are considered
                     
                     if node[1]['namespace'] == 'biological_process':
                         name_to_id[node_name] = node_id
                         id_to_name[node_id] = node_name
                         #id_to_info[node_id] = node_name
@@ -159,22 +161,22 @@
 
                 if 'alt_id' in node[1].keys():
                 
                     for alt_id in node[1]['alt_id']:
                         alt_id_to_id[alt_id.replace(':', '_')] = node_id
 
                 if 'is_obsolete' in node[1].keys() and \
-                        node[1]['is_obsolete'] is True:
+                        node[1]['is_obsolete'] == True:
                     add_node = False
                     del name_to_id[node_name]
                     del id_to_name[node_id]
                 
                 # Check parents for this node
-                if 'is_a' in node[1].keys() and add_node:
-                    # The root node of the ontology does not
+                if 'is_a' in node[1].keys() and add_node: 
+                    # The root node of the ontology does not 
                     # have is_a relationships
 
                     if len(node[1]['is_a']) == 1: 
                         # Only consider concepts with 1 direct ancestor
                         child_to_parent[node_id] = node[1]['is_a'][0]
 
                     for parent in node[1]['is_a']: 
@@ -199,26 +201,26 @@
                         
                     for synonym in node[1]["synonym"]:
                         synonym_name = synonym.split("\"")[1]
                         synonym_to_id[synonym_name] = node_id
 
                 if "xref" in node[1].keys() and add_node:
 
-                    if self.kb == "hp":
+                    if self.kb == "hp": 
                         # Map UMLS concepts to HPO concepts
                         for xref in node[1]['xref']:
                             if xref[:4] == "UMLS":
                                 umls_id = xref.strip("UMLS:")
                                 umls_to_hp[umls_id] =  node_id 
         
-        if self.kb in self.root_dict:
+        if self.kb in self.root_dict.keys():
             root_concept_name = self.root_dict[self.kb][1]
-            root_id = ""
+            root_id = str()
         
-            if root_concept_name not in name_to_id:
+            if root_concept_name not in name_to_id.keys():
                 root_id = self.root_dict[self.kb][0]
                 name_to_id[root_concept_name] = root_id
                 id_to_name[root_id] = root_concept_name
         
         #----------------------------------------------------------------------
         # Add misssing edges between the ontology root and 
         # sub-ontology root concepts
@@ -235,15 +237,15 @@
         kb_graph = nx.DiGraph([edge for edge in edges])
         
         # Build id_to_info (KB-ID: (outdegree, indegree, num_descendants))
         for node in kb_graph.nodes:
             num_descendants = len(nx.descendants(kb_graph, node))
 
             id_to_info[node] = (
-                kb_graph.out_degree(node), kb_graph.in_degree(node),
+                kb_graph.out_degree(node), kb_graph.in_degree(node), 
                 num_descendants)
 
         node_to_node = {}
 
         for edge in edges:
             
             if edge[0] in node_to_node:
@@ -488,15 +490,15 @@
         name_to_id = {}
         id_to_name = {}
         id_to_info = {}
         synonym_to_id = {}
         edges = []
 
         # import concept names
-        with open(self.terms_filename, 'r', encoding="utf-8") as in_file:
+        with open(self.terms_filename, 'r') as in_file:
             data = in_file.readlines()
 
             for line in data:
                 
                 if line != '\n':
                     line_ = line.strip('\n').split('\t')
                     kb_id = line_[0]
@@ -509,15 +511,15 @@
                         
                         for synonym in synonyms:
                             synonym_to_id[synonym] = kb_id
 
         # import relations between concepts
         edges = []
 
-        with open(self.edges_filename, 'r', encoding="utf-8") as in_file:
+        with open(self.edges_filename, 'r') as in_file:
             data = in_file.readlines()
 
             for line in data:
                 
                 if line != '\n':
                     line_ = line.strip('\n').split('\t')
                     term1 = line_[0]
@@ -568,15 +570,15 @@
         name_to_id = {}
         id_to_name = {}
         synonym_to_id = {}
         child_to_parent = {}
         ancestors_count = {}
 
         edges = [] 
-        terms_to_include = []
+        terms_to_include = [],
 
         # Import relations between ChEBI concepts
         with open(kb_dir + 'relation_3star.tsv') as relations_file:
             reader = csv.reader(relations_file, delimiter='\t')
             
             for row in reader:
                 
@@ -588,15 +590,15 @@
     
                     if term1 not in terms_to_include:
                         terms_to_include.append(term1)
 
                     if term2 not in terms_to_include:
                         terms_to_include.append(term2)
 
-                    if term1 in ancestors_count:
+                    if term1 in ancestors_count.keys():
                         added = ancestors_count[term1]
                         added += 1
                         ancestors_count[term1] = added
                     
                     else:
                         ancestors_count[term1] = 1
 
@@ -646,15 +648,15 @@
         edges.append((application, root_id))
 
         # Find child-parent links
         for edge in edges:
             child = edge[0]
             parent = edge[1]
 
-            if child in ancestors_count and ancestors_count[child] == 1:
+            if child in ancestors_count.keys() and ancestors_count[child] == 1:
                 # The term has only 1 direct ancestor
                 child_to_parent[child] = parent
 
         self.name_to_id = name_to_id
         self.id_to_name = id_to_name
         self.synonym_to_id = synonym_to_id
         self.child_to_parent = child_to_parent
```

### Comparing `bent-0.0.55/bent/src/dicts/relation_extraction/dicts.py` & `bent-0.0.9/bent/src/setup/relation_extraction/dicts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 
 # Build dictionaries of extracted relations to further inclusion in the NEL module
 import bent.src.cfg as cfg
 import json
-#import pandas as pd
+import pandas as pd
 
-datasets_dir = cfg.root_path + '/data/datasets/'
-relations_dir = cfg.root_path + '/data/relations/'
+datasets_dir = cfg.root_path + 'data/datasets/'
+relations_dir = cfg.root_path + 'data/relations/'
 
 
 def update_dict(id1, id2, relations):
 
     if id1 not in relations:
         relations[id1] = [id2]
                     
@@ -106,15 +106,15 @@
         if line_count > 1:
             hp_id = line.split("\t")[0].replace(":","_")
             gene_id = line.split("\t")[2]
 
             if entity_type == 'phenotype':
                 relations_temp = update_dict(gene_id, hp_id, relations_temp)
 
-            elif entity_type == 'gene' or entity_type == 'NILGene':
+            elif entity_type == 'gene':
                 relations_temp = update_dict(hp_id, gene_id, relations_temp)
 
         line_count += 1
     
     relations = dict()
     
     for key in relations_temp:
@@ -175,20 +175,20 @@
                 line_data = line.split("\t")
                 
                 if len(line_data) == 4 and line_data[1] == "CID":
                     # Chemical-disease Relation 
                     chemical_id = 'MESH_' + line_data[2]
                     disease_id = 'MESH_' + line_data[3].strip("\n")
 
-                    if entity_type == "disease" or entity_type == "NILDis":
+                    if entity_type == "disease":
                         # Get the disease-disease relations
                         relations_temp = update_dict(
                             chemical_id, disease_id, relations_temp)
                     
-                    elif entity_type == "chemical" or entity_type == "NILChem":
+                    elif entity_type == "chemical":
                         # Get the chemical-chemical relations
                         
                         relations_temp = update_dict(
                             disease_id, chemical_id, relations_temp)
 
     # Two disease terms are related if associated with the same chemical
     # Two chemical terms are related if associated with the same disease
@@ -206,31 +206,31 @@
     return relations
  
 
 def buid_dict(entity_type, kb):
 
     filenames = []
     
-    if entity_type == 'chemical' or entity_type == 'NILChem':
+    if entity_type == 'chemical':
 
         if kb == 'chebi':
             filenames = ['CHR']
         
         elif kb == 'ctd_chem':
             filenames = ['BC5CDR_train', 'BC5CDR_dev']
 
-    elif entity_type == 'disease' or entity_type == 'NILDis':
+    elif entity_type == 'disease':
         
         if kb == 'medic':
             filenames = ['BC5CDR_train', 'BC5CDR_dev']
 
     elif entity_type == 'bioprocess':
         pass
 
-    elif entity_type == 'gene' or entity_type == 'NILGene':
+    elif entity_type == 'gene':
         
         if kb == 'ncbi_gene':
             filenames = ['phenotype_to_genes.txt']
 
     elif entity_type == 'phenotype':
 
         if kb == 'hp':
@@ -260,15 +260,12 @@
     with open(relations_dir + outfilename, 'w') as outfile:
         outfile.write(output)
         outfile.close()
     
 
 def build_relations_dicts():
       
-    pairs = [('disease', 'medic'), ('NILDis', 'medic'), 
-             ('chemical', 'chebi'), ('NILChem', 'chebi'), 
-             ('bioprocess', 'go_bp'), ('gene', 'ncbi_gene'), 
-             ('NILGene', 'ncbi_gene'), ('chemical', 'ctd_chem'),
-             ('NILChem', 'ctd_chem')]
+    pairs = [('disease', 'medic'), ('chemical', 'chebi'), 
+        ('bioprocess', 'go_bp'), ('gene', 'ncbi_gene'), ('chemical', 'ctd_chem')]
    
     for pair in pairs:
         buid_dict(pair[0], pair[1])
```

### Comparing `bent-0.0.55/bent/src/ner.py` & `bent-0.0.9/bent/src/ner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,426 +1,371 @@
 #!/usr/bin/env python
-import os
-import orjson as json
-from transformers import (
-    AutoModelForTokenClassification,
-    AutoTokenizer,
-    TokenClassificationPipeline,
-)
-import bent.src.utils as utils
 import bent.src.cfg as cfg
+import gc
+import orjson as json
+import os
+import bent.src.utils  as utils
+from transformers import AutoModelForTokenClassification, AutoTokenizer, TokenClassificationPipeline
 
 
-class ner:
+class ner():
     """Represent a Named Entity Recognition (NER) pipeline"""
-
-    __slots__ = [
-        "name",
-        "stopwords",
-        "module_root_path",
-        "model_type",
-        "models",
-        "disease_prob",
-        "chemical_prob",
-        "gene_prob",
-        "organism_prob",
-        "bioprocess_prob",
-        "anatomical_prob",
-        "cell_component_prob",
-        "cell_line_prob",
-        "variant_prob",
-    ]
-
+    
+    __slots__= ['name', 'stopwords', 'module_root_path', 'model_type', 'models', 
+        'disease_prob', 'chemical_prob', 'gene_prob', 'organism_prob',
+        'bioprocess_prob', 'anatomical_prob', 'cell_component_prob',
+        'cell_line_prob', 'variant_prob']
     def __init__(self, name, types, stopwords):
         """_summary_
 
         :param name: the name of the model that will be loaded
         :type name: str
-        :param types: the entity types that will be recognized
+        :param types: the entity types that will be recognized 
         :type types: list
-        :param stopwords: frequent words ('the', 'and', 'of) that will not be
+        :param stopwords: frequent words ('the', 'and', 'of) that will not be 
             considered as an entity
         :type stopwords: str
         :raises ValueError: if the inputted model name is not 'pubmedbert'
         """
-        self.name = name
+        self.name = name    
         self.stopwords = stopwords
 
         module_root_path = cfg.root_path
         self.module_root_path = module_root_path
-        # --------------------------------------------------------------------
-        # Load NER models and dictionaries with entities probabilities to
+        #--------------------------------------------------------------------
+        # Load NER models and dictionaries with entities probabilities to 
         # resolve overlapping entities
-        # --------------------------------------------------------------------
+        #--------------------------------------------------------------------
         self.model_type = None
         self.models = {}
-
-        if self.name == "pubmedbert":
-            self.model_type = "bert"
-
-            if "disease" in types:
+      
+        if self.name == 'pubmedbert':
+            self.model_type = 'bert'
+            
+            if 'disease' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Disease"
-                self.models["disease"] = ner.load_transformer_model(model_name)
-                dict_filename = f"{module_root_path}data/overlapping_entities/disease.json"
-
+                self.models['disease'] = ner.load_transformer_model(model_name)
+                dict_filename = '{}data/overlapping_entities/disease.json'.format(module_root_path)
                 if len(types) > 1:
                     self.disease_prob = ner.load_probabilities_file(dict_filename)
-
-            if "NILDis" in types:
-                model_name = "pruas/BENT-PubMedBERT-NER-Disease"
-                self.models["NILDis"] = ner.load_transformer_model(model_name)
-
-            if "chemical" in types:
+                
+            if 'chemical' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Chemical"
-                self.models["chemical"] = ner.load_transformer_model(model_name)
-                dict_filename = f"{module_root_path}data/overlapping_entities/chemical.json"
-                    
+                self.models['chemical'] = ner.load_transformer_model(model_name)
+                dict_filename = '{}data/overlapping_entities/chemical.json'.format(module_root_path)
                 if len(types) > 1:
                     self.chemical_prob = ner.load_probabilities_file(dict_filename)
-
-            if "NILChem" in types:
-                model_name = "pruas/BENT-PubMedBERT-NER-Chemical"
-                self.models["NILChem"] = ner.load_transformer_model(model_name)
-
-            if "gene" in types:
+           
+            if 'gene' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Gene"
-                self.models["gene"] = ner.load_transformer_model(model_name)
-                dict_filename = f"{module_root_path}/data/overlapping_entities/gene.json"
-
+                self.models['gene'] = ner.load_transformer_model(model_name)
+                dict_filename = '{}/data/overlapping_entities/gene.json'.format(module_root_path)
                 if len(types) > 1:
                     self.gene_prob = ner.load_probabilities_file(dict_filename)
 
-            if "NILGene" in types:
-                model_name = "pruas/BENT-PubMedBERT-NER-Gene"
-                self.models["NILGene"] = ner.load_transformer_model(model_name)
-
-            if "organism" in types:
+            if 'organism' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Organism"
-                self.models["organism"] = ner.load_transformer_model(model_name)
-                dict_filename = f"{module_root_path}data/overlapping_entities/organism.json"
-
-                if len(types) > 1:
+                self.models['organism'] = ner.load_transformer_model(model_name)
+                dict_filename = '{}data/overlapping_entities/organism.json'.format(module_root_path)
+                if len(types) > 1:    
                     self.organism_prob = ner.load_probabilities_file(dict_filename)
 
-            if "bioprocess" in types:
+            if 'bioprocess' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Bioprocess"
-                self.models["bioprocess"] = ner.load_transformer_model(model_name)
-                dict_filename = f"{module_root_path}data/overlapping_entities/bioprocess.json"
-
-                if len(types) > 1:
+                self.models['bioprocess'] = ner.load_transformer_model(model_name)   
+                dict_filename = '{}data/overlapping_entities/bioprocess.json'.format(module_root_path)
+                if len(types) > 1:    
                     self.bioprocess_prob = ner.load_probabilities_file(dict_filename)
 
-            if "anatomical" in types:
+            if 'anatomical' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Anatomical"
-                self.models["anatomical"] = ner.load_transformer_model(model_name)
-                dict_filename = f"{module_root_path}data/overlapping_entities/anatomical.json"
-
-                if len(types) > 1:
+                self.models['anatomical'] = ner.load_transformer_model(model_name)   
+                dict_filename = '{}data/overlapping_entities/anatomical.json'.format(module_root_path)
+                if len(types) > 1:    
                     self.anatomical_prob = ner.load_probabilities_file(dict_filename)
-
-            if "cell_component" in types:
+            
+            if 'cell_component' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Cell-Component"
-                self.models["cell_component"] = ner.load_transformer_model(model_name)
-                dict_filename = f"{module_root_path}data/overlapping_entities/cell_component.json"
-
-                if len(types) > 1:
-                    self.cell_component_prob = ner.load_probabilities_file(
-                        dict_filename
-                    )
-
-            if "cell_line" in types:
+                self.models['cell_component'] = ner.load_transformer_model(model_name)   
+                dict_filename = '{}data/overlapping_entities/cell_component.json'.format(module_root_path)
+                if len(types) > 1:    
+                    self.cell_component_prob = ner.load_probabilities_file(dict_filename)
+            
+            if 'cell_line' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Cell-Line"
-                self.models["cell_line"] = ner.load_transformer_model(model_name)
-                dict_filename = f"{module_root_path}data/overlapping_entities/cell_line.json"
-
-                if len(types) > 1:
+                self.models['cell_line'] = ner.load_transformer_model(model_name)   
+                dict_filename = '{}data/overlapping_entities/cell_line.json'.format(module_root_path)
+                if len(types) > 1:    
                     self.cell_line_prob = ner.load_probabilities_file(dict_filename)
-
-            if "cell_type" in types:
+            
+            if 'cell_type' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Cell-Type"
-                self.models["cell_type"] = ner.load_transformer_model(model_name)
-                dict_filename = f"{module_root_path}data/overlapping_entities/cell_type.json"
-
-                if len(types) > 1:
+                self.models['cell_type'] = ner.load_transformer_model(model_name)   
+                dict_filename = '{}data/overlapping_entities/cell_type.json'.format(module_root_path)
+                if len(types) > 1:    
                     self.cell_type_prob = ner.load_probabilities_file(dict_filename)
 
-            if "variant" in types:
+            if 'variant' in types:
                 model_name = "pruas/BENT-PubMedBERT-NER-Variant"
-                self.models["variant"] = ner.load_transformer_model(model_name)
-                dict_filename = f"{module_root_path}data/overlapping_entities/variant.json"
-
-                if len(types) > 1:
-                    self.variant_prob = ner.load_probabilities_file(dict_filename)
-
+                self.models['variant'] = ner.load_transformer_model(model_name)   
+                dict_filename = '{}data/overlapping_entities/variant.json'.format(module_root_path)
+                if len(types) > 1:    
+                    self.variant_prob = ner.load_probabilities_file(dict_filename)  
+        
         else:
-            raise ValueError("Model not implemented!")
+            raise ValueError('Model not implemented!')
 
     @staticmethod
     def load_transformer_model(model_filepath):
-        """Load NER model from given filepath into a
-        'TokenClassificationPipeline' object (Hugging Face library) ready to
+        """Load NER model from given filepath into a 
+        'TokenClassificationPipeline' object (Hugging Face library) ready to 
         annotate texts.
 
         :param model_filepath: local or online path for the model
         :type model_filepath: str
         :return: loaded_model
         :rtype: 'TokenClassificationPipeline' object
         """
-
+        
+        
         model = AutoModelForTokenClassification.from_pretrained(model_filepath)
         tokenizer_1 = AutoTokenizer.from_pretrained(
-            model_filepath, model_max_length=512
-        )
-        loaded_model = TokenClassificationPipeline(
-            task="ner",
-            model=model,
-            tokenizer=tokenizer_1,
-            aggregation_strategy="simple",
-        )
-
+            model_filepath, model_max_length=512)
+        loaded_model = TokenClassificationPipeline(task='ner', 
+                        model=model, 
+                        tokenizer=tokenizer_1,
+                        aggregation_strategy='simple')#, 
+                        #grouped_entities=True)#,
+                        #aggregation_strategy='simple')
+        
         return loaded_model
-
+    
     @staticmethod
     def load_probabilities_file(dict_filename):
-
+        
         type_dict = {}
 
         if os.path.exists(dict_filename):
-            with open(dict_filename, "r") as dict_file:
+            with open(dict_filename, 'r') as dict_file:
                 type_dict = json.loads(dict_file.read())
                 dict_file.close()
-
+        
         return type_dict
-
+ 
     @staticmethod
     def correct_tokens(sent, raw_annots, entity_type, stopwords):
-        """Correct the output of BERT-based models by grouping tokens
+        """Correct the output of BERT-based models by grouping tokens 
         associated with the same entity. For example, the entities
-        'Am' and '##minoacids' are considered independent, but they are
+        'Am' and '##minoacids' are considered independent, but they are 
         the same entity.
 
-        :param sent: specific sentence where the model was applied
+        :param sent: specific sentence where the model was applied 
         :type sent: 'Sentence' object
         :param raw_annots: recognized entities in given sentence
         :type raw_anots: list
-        :param entity_type: the type of the entities that were recognized in
+        :param entity_type: the type of the entities that were recognized in 
             this sentence
         :type entity_type: str
-        :param stopwords: frequent words ('the', 'and', 'of) that will not be
+        :param stopwords: frequent words ('the', 'and', 'of) that will not be 
             considered as an entity
         :type stopwords: str
-        :return: corrected_annots including the recognized entities with text
+        :return: corrected_annots including the recognized entities with text 
             and span corrected
         :rtype: list
         """
-
+        
         annots_up = []
         token_count = 0
-
+        
         for i, annot in enumerate(raw_annots):
-            current_start = sent.start + annot["start"]
-            current_end = sent.start + annot["end"]
-            current_token_score = annot["score"]
-
+            current_start = sent.start + annot['start']
+            current_end =  sent.start + annot['end']
+            current_token_score = annot['score']
+            
             if i > 0:
                 previous_annot = annots_up[-1]
                 previous_start = previous_annot[0]
                 previous_end = previous_annot[1]
                 previous_token_score = previous_annot[4]
                 previous_token_count = previous_annot[5]
-
-                if previous_end == (current_start - 1) or previous_end == (
-                    current_start
-                ):
-
-                    # Entity spans are defined in the context of the sentence
+                   
+                if previous_end == (current_start - 1) \
+                        or previous_end == (current_start):
+                   
+                    # Entity spans are defined in the context of the sentence 
                     # and not of the entire document
                     start_tmp = previous_start - sent.start
                     end_tmp = current_end - sent.start
                     entity_text_up = sent.text[start_tmp:end_tmp]
-
+                    
                     # Calculate averaget of previous token scores with current
                     # one. Formula: ( n * a + v ) / (n + 1);
                     current_token_count_update = previous_token_count + 1
-                    current_token_score_updated = (
-                        previous_token_count * previous_token_score
-                        + current_token_score
-                    ) / (current_token_count_update)
-
+                    current_token_score_updated = (previous_token_count * \
+                        previous_token_score + current_token_score) / \
+                        (current_token_count_update)
+                    
                     annot_up = [
-                        previous_start,
-                        current_end,
-                        entity_text_up,
-                        entity_type,
-                        current_token_score_updated,
-                        current_token_count_update,
-                    ]
-
+                        previous_start, current_end, 
+                        entity_text_up, entity_type, \
+                        current_token_score_updated, current_token_count_update]
+                    
                     annots_up.append(annot_up)
 
-                    # Delete previous incomplete annotation and replace it
+                    # Delete previous incomplete annotation and replace it 
                     # by the updated entity
                     del annots_up[-2]
-
+                    
                 else:
                     # Current entity is a new entity
                     start_tmp = current_start - sent.start
                     end_tmp = current_end - sent.start
                     entity_text = sent.text[start_tmp:end_tmp]
                     current_token_count = 1
-
+                    
                     annot_up = [
-                        current_start,
-                        current_end,
-                        entity_text,
-                        entity_type,
-                        current_token_score,
-                        current_token_count,
-                    ]
-
+                        current_start, current_end, 
+                        entity_text, entity_type, 
+                        current_token_score, current_token_count]
+                    
                     annots_up.append(annot_up)
-
+                
             else:
                 # Current entity is the first entity in given sentence
                 start_tmp = current_start - sent.start
                 end_tmp = current_end - sent.start
                 entity_text = sent.text[start_tmp:end_tmp]
                 token_count += 1
-
+                            
                 annot_up = [
-                    current_start,
-                    current_end,
-                    entity_text,
-                    entity_type,
-                    current_token_score,
-                    token_count,
-                ]
+                    current_start, current_end,
+                    entity_text, entity_type, current_token_score, token_count]
 
                 annots_up.append(annot_up)
-
+        
         # Further post_processing of the entities
         corrected_annots = []
 
         for annot in annots_up:
             text = annot[2]
-            words = text.split(" ")
+            words = text.split(' ')
 
-            if text[0] != ":":
+            if text[0] != ':':
 
                 # Do not consider entities with length=1 except of chemical type
                 if len(text) == 1:
 
                     if entity_type == "ChemicalEntity":
-                        # Chemical entities can have length 1 (e.g. chemical
+                        # Chemical entities can have length 1 (e.g. chemical 
                         # elements) but there can be errors (e.g. "-"")
-
+                        
                         if text.isalpha() and text not in stopwords:
-                            # The only char is not a letter, so it cannot be a
+                            # The only char is not a letter, so it cannot be a 
                             # chemical element
                             corrected_annots.append(annot)
-
+                        
                 elif len(text) > 1:
-
+                    
                     if len(words) > 1:
                         corrected_annots.append(annot)
-
+                    
                     elif len(words) == 1:
-
-                        # If the entity has only 1 word and that word is a stop
+                        
+                        # If the entity has only 1 word and that word is a stop 
                         # word, the entity won't be considered
                         if text not in stopwords:
                             corrected_annots.append(annot)
-
-                if "\n" in text:
+                
+                if '\n' in text:
                     # Correct error such as 'fenofibrate\nFenofibrate'
-                    # Current annotation will origin two distinct annotations
-                    text1 = text.split("\n")[0]
+                    # Current annotation will origin two distinct annotations 
+                    text1 = text.split('\n')[0]
                     start1 = annot[0]
                     end1 = start1 + len(text1)
                     annot1 = [start1, end1, text1, annot[3], annot[4], annot[5]]
-
-                    text2 = text.split("\n")[1]
+                    
+                    text2 = text.split('\n')[1]
                     start2 = end1 + 1
-                    end2 = start2 + len(text2)
+                    end2 = start2 + len(text2) 
                     annot2 = [start2, end2, text2, annot[3], annot[4], annot[5]]
 
                     # Replace current annotation with annotation 1
                     current_index = corrected_annots.index(annot)
                     corrected_annots[current_index] = annot1
 
                     # Insert annotation 2 after annotation 1
                     index_2 = current_index + 1
                     corrected_annots.insert(index_2, annot2)
 
         return corrected_annots
 
     def get_entity_prob(self, ent_text, ent_type):
-
+    
         target_dict = {}
 
-        if ent_type == "disease":
+        if ent_type == 'disease':
             target_dict = self.disease_prob
 
-        if ent_type == "chemical":
+        if ent_type == 'chemical':
             target_dict = self.chemical_prob
 
-        if ent_type == "gene":
+        if ent_type == 'gene':
             target_dict = self.gene_prob
 
-        if ent_type == "organism":
+        if ent_type == 'organism':
             target_dict = self.organism_prob
 
-        if ent_type == "bioprocess":
+        if ent_type == 'bioprocess':
             target_dict = self.bioprocess_prob
 
-        if ent_type == "anatomical":
+        if ent_type == 'anatomical':
             target_dict = self.anatomical_prob
 
-        if ent_type == "cell_component":
+        if ent_type == 'cell_component':
             target_dict = self.cell_component_prob
 
-        if ent_type == "cell_line":
+        if ent_type == 'cell_line':
             target_dict = self.cell_line_prob
 
-        if ent_type == "cell_type":
+        if ent_type == 'cell_type':
             target_dict = self.cell_type_prob
 
-        if ent_type == "variant":
+        if ent_type == 'variant':
             target_dict = self.variant_prob
 
         prob = 0.0
 
         if ent_text.lower() in target_dict.keys():
             prob = target_dict[ent_text.lower()]
-
+        
         return prob
-
+    
     def compare_entities_w_same_text(self, annot, annot2, entity_frequency):
 
-        # Retrieve probabilities from external dicts
+        # Retrieve probabilities from external dicts         
         annot_prob = ner.get_entity_prob(self, annot.text, annot.type)
         annot2_prob = ner.get_entity_prob(self, annot2.text, annot2.type)
 
-        # --------------------------------------------------------------------
+        #--------------------------------------------------------------------
         # Remove the entity with lower probability
         entity2keep = None
         entity2remove = None
 
         if annot_prob > annot2_prob:
             entity2remove = annot2
             entity2keep = annot
-
+        
         elif annot_prob < annot2_prob:
             entity2remove = annot
             entity2keep = annot2
-
+        
         elif annot_prob == annot2_prob:
-            annot_key = annot.text + "_" + annot.type
+            annot_key = annot.text + '_' + annot.type
             freq1 = entity_frequency[annot_key]
-            annot2_key = annot2.text + "_" + annot2.type
+            annot2_key = annot2.text + '_' + annot2.type
             freq2 = entity_frequency[annot2_key]
 
             if freq1 > freq2:
                 entity2remove = annot2
                 entity2keep = annot
 
             elif freq1 < freq2:
@@ -431,109 +376,107 @@
 
     @staticmethod
     def get_entity_frequency_in_doc(entities):
 
         entity_frequency = {}
 
         for entity in entities:
-            entity_key = entity.text + "_" + entity.type
+            entity_key = entity.text + '_' + entity.type
 
             if entity.text in entity_frequency.keys():
                 entity_frequency[entity_key] += 1
-
+        
             else:
                 entity_frequency[entity_key] = 1
-
+        
         return entity_frequency
 
     def correct_overlapping_annotations(self, doc):
         """Correct overlapping entities in a given document. The overlapping
-        is both at the level of span (two entities share either the start or
-        the end position in a given sentence) and at the level of the string
-        (two entities with the same string classified according different
+        is both at the level of span (two entities share either the start or 
+        the end position in a given sentence) and at the level of the string 
+        (two entities with the same string classified according different 
         entities types)
 
         :param doc:
         :type doc: Document object
         :return: doc
-        :rtype:
+        :rtype: 
         """
 
-        # ---------------------------------------------------------------------
+        #---------------------------------------------------------------------
         # Resolve overlapping pairs of entities in each sentence of given doc
-        # ---------------------------------------------------------------------
+        #---------------------------------------------------------------------
 
         # Get frequency of each entity
         entity_frequency = ner.get_entity_frequency_in_doc(doc.entities)
 
-        # ---------------------------------------------------------------------
+        #---------------------------------------------------------------------  
         # Resolve entities that have the same text, different entity type and
         # that are located in DIFFERENT SENTENCES of the document
-        # ---------------------------------------------------------------------
+        #---------------------------------------------------------------------     
         doc_entities = doc.entities
 
         for annot in doc_entities:
-
+            
             for annot2 in doc_entities:
 
-                if annot.text == annot2.text and annot.type != annot2.type:
+                if annot.text == annot2.text and \
+                    annot.type != annot2.type:
 
                     entity2keep, entity2remove = ner.compare_entities_w_same_text(
-                        self, annot, annot2, entity_frequency
-                    )
+                        self, annot, annot2, entity_frequency)
 
                     if entity2keep != None and entity2remove != None:
                         sent = doc.get_sentence(entity2remove.sent_num)
                         sent.remove_entity(entity2remove)
                         doc.remove_entities([entity2remove])
 
                         # Change the type of the deleted entity and add it again
                         entity2add = entity2remove
                         entity2add.type = entity2keep.type
                         sent.add_entity(entity2add)
                         doc.update_sentence(sent, sent.num)
 
         return doc
-
+        
     def apply(self, document):
         """Annotate the texts belonging to given collection with the previously
         loaded model(s).
 
-        :param document: doc_obj including all the information about the input
-            text, such as its identifier and its sentences
+        :param document: doc_obj including all the information about the input 
+            text, such as its identifier and its sentences 
         :type document: Document object
         :raises ValueError: if the loaded model has different type that 'bert'
         :return: doc_entities including the inputted information updated with
             the recognized entities
         :rtype: Document object
         """
 
-        if self.model_type == "bert":
+        if self.model_type == 'bert':
             doc_sentences = document.sentences
-
+            
             for i, sent in enumerate(doc_sentences):
-
+                
                 for model in self.models:
                     raw_annots = self.models[model](
-                        sent.text
-                    )  # truncation=True, padding=True)
+                        sent.text, padding=True, truncation=True)
                     annots_up = ner.correct_tokens(
-                        sent, raw_annots, model, self.stopwords
-                    )
-
-                    annots_obj = utils._objectify_entities(annots_up, i)
+                        sent, raw_annots, model, self.stopwords)
 
+                    annots_obj = utils.objectify_entities(annots_up, i)
+                    
                     sent.add_multi_entities(annots_obj)
                     document.update_sentence(sent, i)
-
+                        
             doc_entities = ner.correct_overlapping_annotations(self, document)
 
             del doc_sentences
             del raw_annots
-            del annots_up
+            del annots_up 
             del annots_obj
             utils.garbage_collect()
 
         else:
-            raise ValueError("Model not implemented!")
+            raise ValueError('Model not implemented!')
 
         return doc_entities
```

### Comparing `bent-0.0.55/bent/src/utils.py` & `bent-0.0.9/bent/src/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,584 +1,580 @@
 #!/usr/bin/env python
-from copy import deepcopy
+import bent.src.cfg as cfg
+import orjson as json 
 import os
-import gc
 import psutil
 import shutil
-import orjson as json
-import bent.src.cfg as cfg
+import gc
 from bent.src.classes import Document, Sentence, Entity
+from copy import deepcopy
 
-# ------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #                       INPUT ARGUMENTS VERIFICATION
-# ------------------------------------------------------------------------------
-
+#------------------------------------------------------------------------------
 
-def _check_input_types(types):
-    """Check if the inputted entity types are valid, as well the selected
+def check_input_types(types):
+    """Check if the inputted entity types are valid, as well the selected 
     target knowledge bases.
 
     :param types: a dictionary with the format {'entity_type: 'target_kb'}
     :type types: dict
-    :raises ValueError: if types is an empty dictionary
+    :raises ValueError: if types is an empty dictionary 
     """
-
+    
     if types == {}:
-        raise ValueError("No specified entity types!")
-
+        raise ValueError('No specified entity types!')
+    
     else:
         available_types = [
-            "disease",
-            "chemical",
-            "gene",
-            "organism",
-            "bioprocess",
-            "anatomical",
-            "cell_component",
-            "cell_line",
-            "cell_type",
-            "variant",
-            "NILDis",
-            "NILChem",
-            "NILGene",
-        ]
-
+            'disease', 'chemical', 'gene', 'organism', 'bioprocess', 
+            'anatomical', 'cell_component', 'cell_line', 'cell_type', 
+            'variant']
+       
         for ent_type in types:
+            
+            if ent_type != '':
+                assert ent_type in available_types, \
+                    '{} is an invalid entity type! Options:\
+                    "disease", "chemical", "gene", "organism", "bioprocess", \
+                    "bioprocess", "anatomical", "cell_component", "cell_line",\
+                    "cell_type", "variant"'.format(ent_type)
+                        
+
+def check_input_args(recognize, link, types, input_format, input_text, 
+        in_dir, ner_dir, out_dir, ner_model, nel_model):
+    """Verify if the input arguments are valid"""
 
-            if ent_type != "":
-                assert (
-                    ent_type in available_types
-                ), f"{ent_type} is an invalid entity type to recognize! Options:\
-                    'disease', 'chemical', 'gene', 'organism', 'bioprocess', \
-                    'bioprocess', 'anatomical', 'cell_component', 'cell_line',\
-                    'cell_type', 'variant', 'NILDis', 'NILChem', 'NILGene'"               
-
-
-def _check_input_args(
-    recognize,
-    link,
-    types,
-    input_format,
-    input_text,
-    in_dir,
-    ner_dir,
-    out_dir,
-):
-    """Verify if the input arguments are valid."""
-
-    available_formats = ["brat", "bioc_xml", "bioc_json", "pubtator"]
+    available_formats = ['brat', 'bioc_xml', 'bioc_json', 'pubtator'] 
 
     # Verify selected task(s)
-    assert (
-        recognize is True or link is True
-    ), "It is available Named Entity Recognition (NER) and/or Named Entity ensure that either recognize == True and/or link == True"
+    assert recognize == True or link == True, \
+        'It is available Named Entity Recognition (NER) and/or Named Entity \
+        ensure that either recognize == True and/or link == True'
 
     # Verify the inputed entity types and respective target KBs
-    _check_input_types(types)
+    check_input_types(types)
 
-    # Verify input format and directory arguments
+    # Verify input format and dir
     if recognize:
 
-        if input_text is None and in_dir is None:
-            raise ValueError(
-                'It is necessary to input either a text or a list of texts (by setting the argument "input_text") OR a directory containing file(s) with texts to annotate (by setting the argument "text_dir").'
-            )
-
-        if (
-            input_format == "bioc_json"
-            or input_format == "bioc_xml"
-            or input_format == "pubtator"
-        ):
-
-            assert (
-                in_dir is not None or ner_dir is not None
-            ), 'For input formats "bioc_json", "bioc_xml"and "pubtator" it is necessary to specify the input directory by setting the argument "in_dir"'
+        if input_text == None and in_dir == None:
+            raise ValueError('It is necessary to input either a text \
+                ("input_text") OR a directory containing file(s) with text \
+                to annotate ("text_dir").') 
+        
+        if input_format == 'bioc_json' or input_format == 'bioc_xml' \
+                or input_format == 'pubtator':
+
+                assert in_dir != None or ner_dir != None, \
+                    'For input formats "bioc_json"\
+                    , "bioc_xml"and "pubtator" it is necessary to specify\
+                    the input directory "in_dir"'
 
     if link:
 
         if not recognize:
 
-            assert (
-                ner_dir is not None
-            ), 'No NER will be performed, only NEL: it is necessary to specfiy the directory containing NER annotations (by setting the argument "ner_dir").'
-
-    # Check directory paths
-
-    if in_dir is not None:
-        assert (
-            in_dir[-1:] == "/"
-        ), 'Invalid argument "in_dir": the last character in the directory path must be "/"\n. Examples: "dataset/txt" -> INVALID directory path "dataset/txt/" -> VALID directory path'
-
-    if ner_dir is not None:
-        assert (
-            ner_dir[-1:] == "/"
-        ), 'Invalid argument "ner_dir": the last character in the directory path must be "/"\n. Examples: "dataset/ann" -> INVALID directory path "dataset/ann/" -> VALID directory path'
-
-    if out_dir is not None:
-        assert (
-            out_dir[-1:] == "/"
-        ), 'Invalid argument "out_dir": the last character in the directory path must be "/"\n. Examples: "dataset/ann" -> INVALID directory path "dataset/ann/" -> VALID directory path'
+            assert ner_dir != None, 'It is necessary to specfiy the directory \
+                containing the ouput from the NER stage ("ner_dir").' 
 
+    #Check directories paths
+    if in_dir != None:
+        assert in_dir[-1:] == '/', 'Invalid "in_dir". Last character in \
+            directory name must be "/"'
+
+    if ner_dir != None:
+        assert ner_dir[-1:] == '/', 'Invalid "ner_dir". Last character in \
+            directory name must be "/"'
+
+    if out_dir != None:
+        assert out_dir[-1:] == '/', 'Invalid "out_dir". Last character in \
+            directory name must be "/"'
+        
 
-# ------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #                       INPUT FILE FORMAT CONVERSION
-# ------------------------------------------------------------------------------
-def _parse_bioc_json_file(filename, include_text=True):
+#------------------------------------------------------------------------------
+
+def parse_bioc_json_file(filename, include_text=True):
+    
 
-    with open(filename, "r", encoding="utf-8") as infile:
+    with open(filename, 'r') as infile:
         parsed_data = json.loads(infile.read())
         infile.close()
 
     parsed_data_up = {}
 
-    for doc in parsed_data["documents"]:
-        title = ""
-        abstract = ""
+    for doc in parsed_data['documents']:
+        title = ''
+        abstract = ''
         annotations = []
-        parsed_data_up[doc["id"]] = ["", []]
-
-        for passage in doc["passages"]:
+        parsed_data_up[doc['id']] = ['', []]
 
-            if passage["infons"]["type"] == "title":
-                title = passage["text"]
+        for passage in doc['passages']:
+            
+            if passage['infons']['type'] == 'title':
+                title = passage['text']
 
-            if passage["infons"]["type"] == "abstract":
-                abstract = passage["text"]
+            if passage['infons']['type'] == 'abstract':
+                abstract = passage['text']
 
-                for annot in passage["annotations"]:
-                    ent_type = annot["infons"]["type"]
-                    text = annot["text"]
+                for annot in passage['annotations']:
+                    ent_type = annot['infons']['type']
+                    #kb_id = annot['infons']['identifier']
+                    text = annot['text']
 
-                    begin = annot["locations"][0]["offset"]
-                    end = str(int(begin) + int(annot["locations"][0]["length"]))
+                    begin = annot['locations'][0]['offset']
+                    end = str(int(begin) + int(annot['locations'][0]['length']))
 
                     annotation = (ent_type, begin, end, text)
                     annotations.append(annotation)
-
-        text = title + "\n" + abstract
-
-        parsed_data_up[doc["id"]][0] = ""
+        
+        text = title + '\n' + abstract
+        
+        parsed_data_up[doc['id']][0] = ''
 
         if include_text:
-            parsed_data_up[doc["id"]][0] = text
-
-        parsed_data_up[doc["id"]][1] = annotations
+            parsed_data_up[doc['id']][0] = text
+        
+        parsed_data_up[doc['id']][1] = annotations
 
     return parsed_data_up
 
 
 def output_parsed_docs(parsed_data, out_dir, recognize=False):
 
     # Output parsed documents to out_dir in the BRAT format
-    os.makedirs(f"{out_dir}txt/", exist_ok=True)
-    os.makedirs(f"{out_dir}ann/", exist_ok=True)
+    if not os.path.exists(out_dir + 'txt/'):
+        os.mkdir(out_dir + 'txt/')
+    
+    if not os.path.exists(out_dir + 'ann/'):
+        os.mkdir(out_dir + 'ann/')
 
     for doc_id in parsed_data:
         doc_text = parsed_data[doc_id][0]
-
-        with open(f"{out_dir}txt/{doc_id}.txt", "w", encoding="utf-8") as txt_file:
+        
+        with open(out_dir + 'txt/' + doc_id + '.txt', 'w') as txt_file:
             txt_file.write(doc_text)
             txt_file.close()
-
+       
         if not recognize:
             # In this case only the NEL step will be performed
             # Make annotations file
+        
             annotations = parsed_data[doc_id][1]
-            annot_str = ""
+            annot_str = ''
 
             for i, annot in enumerate(annotations):
-                annot_str += f"T{str(i + 1)}\t{annot[0]} {annot[1]} {annot[2]}\t{annot[3]}\n"
-
-            with open(f"{out_dir}ann/{doc_id}.ann", "w", encoding="utf-8") as ann_file:
+                annot_str += 'T{}\t{} {} {}\t{}\n'.format(
+                    str(i+1), annot[0], annot[1], annot[2], annot[3]) 
+        
+            with open(out_dir + 'ann/' + doc_id + '.ann', 'w') as ann_file:
                 ann_file.write(annot_str)
                 ann_file.close()
+        
 
+def convert_input_files(format, input_text=None, in_dir=None, recognize=False):
+    """Convert input file(s) into brat/standoof format"""
+    
+    if input_text != None:
 
-def _convert_input_files(in_dir=None, input_text=None):
-    """Convert input file(s) into brat/standoff format"""
-
-    if input_text is not None:
-
-        if isinstance(input_text, str):
+        if type(input_text) == str:
             input_files = [input_text]
-
-        elif isinstance(input_text, list):
+            
+        elif type(input_text) == list:
             input_files = input_text
 
         # Create a txt file for later use in the NEL module.
-        for i, text in enumerate(input_files, start=1):
-            doc_id = f"doc_{str(i)}"
-
-            with open(f"{in_dir}{doc_id}.txt", "w", encoding="utf-8") as txt_file:
+        for i, text in enumerate(input_files):
+            doc_id = str(i)
+            
+            with open(out_dir + doc_id + '.txt', 'w') as txt_file:
                 txt_file.write(text)
                 txt_file.close()
+    
+    else:
 
+        assert format == 'bioc_xml' or format == 'bioc_json' \
+            or format == 'pubtator',  'Invalid format. Options: "brat", \
+            "bioc_xml", "bioc_json", "pubtator"'
+        
+        
+        filenames = [in_dir + filename for filename in os.listdir(in_dir)]
+        out_dir = in_dir + 'brat/'
+            
+        for filename in filenames:
+            output = False
+            
+            if format == 'bioc_xml' and filename[-3:] == 'xml':
+                parsed_data = parse_bioc_xml_file(filename)
+                output = True
+            
+            elif format == 'bioc_json' and filename[-4:] == 'json':
+                parsed_data = parse_bioc_json_file(filename)
+                output = True
+           
+            elif format == 'pubtator' and filename[-3:] == 'txt':
+                parsed_data = parse_pubtator_file(filename)
+                output = True
 
-# ------------------------------------------------------------------------------
-#                       TEXT PARSING AND OBJECTIFICATION
-# ------------------------------------------------------------------------------
+            if output:
 
+                if not os.path.exists(out_dir):
+                    os.mkdir(out_dir)
+                
+                output_parsed_docs(parsed_data, out_dir, recognize=recognize)
+        
 
-def _sentence_splitter(doc_text, lang_model):
-    """Split given text into sentences using SpaCy and the ScispaCy model
+#------------------------------------------------------------------------------
+#                       TEXT PARSING AND OBJECTIFICATION 
+#------------------------------------------------------------------------------
+
+def sentence_splitter(doc_text, lang_model):
+    """Split given text into sentences using SpaCy and the ScispaCy model 
     'en_core_sci_lg' (https://allenai.github.io/scispacy/).
 
     :param doc_text: the input text to be splitted into sentences
     :type doc_text: str
     :param lang_model: Spacy sentence splitter model
     :type lang_model:
-    :return: doc_sentences including input text splitted in sentences
+    :return: doc_sentences including input text splitted in sentences 
     :rtype: list
     """
-
+  
     processed_doc = lang_model(doc_text)
     doc_sentences = [sent.text for sent in processed_doc.sents]
-
+    
     return doc_sentences
 
 
-def _objectify_ner_input(doc_id, doc_text, doc_sentences):
+def objectify_ner_input(doc_id, doc_text, doc_sentences):
     """Convert a given input text into a Document object.
 
     :param doc_id: the idenfitifer of the input text
     :type doc_id: str
     :param doc_text: the input text
     :type doc_text: str
     :param doc_sentences: the sentences of the input text
     :type doc_sentences: list
-    :return: doc_obj including all the information about the input text, such
-        as its identifier and its sentences
+    :return: doc_obj including all the information about the input text, such 
+        as its identifier and its sentences 
     :rtype: Document objcet
     """
-
+    
     # Hierarchy: Collection -> Document -> Sentence -> Entity
     doc_obj = Document(doc_text)
     doc_obj.set_id(doc_id)
     current_pos = 0
-    last_sent_index = len(doc_sentences) - 1
-    doc_text_len = len(doc_text)
-
+    last_sent_index = len(doc_sentences) -1
+    doc_text_len = len(doc_text) 
+   
     for i, sent_text in enumerate(doc_sentences):
-        # ---------------------------------------------------------------------
+        #---------------------------------------------------------------------
         # Solve mismatches produced by the sentence splitter when current
         # sentence and previous sentence are not separated by ' '.
         # This allows the correction of the span of the recognized entities
-
+        
         if sent_text.isalnum():
-
+                    
             try:
                 if i == last_sent_index:
-                    original_char = doc_text[current_pos - 1]
-
+                    original_char = (doc_text[current_pos-1])
+                
                 elif i < last_sent_index:
-                    original_char = doc_text[current_pos]
-
-                if original_char == " ":
+                    original_char = (doc_text[current_pos])
+                
+                if original_char == ' ':
                     i = 0
                     proceed = True
-
+                    
                     while proceed:
                         current_pos += 1
-
+                        
                         if current_pos < (doc_text_len):
-                            original_char = doc_text[current_pos]
-
-                            if original_char != " ":
+                            original_char = (doc_text[current_pos])
+                            
+                            if original_char != ' ':
                                 proceed = False
-
+                        
                         else:
                             proceed = False
 
                         i += 1
-
+                    
                 else:
                     sent_first_char = sent_text[0]
 
                     if original_char != sent_first_char:
                         i = 0
-
+                        
                         while original_char != sent_first_char:
                             current_pos -= 1
-                            original_char = doc_text[current_pos]
-                            i += 1
+                            original_char = (doc_text[current_pos])
+                            i += 1      
 
             except IndexError:
-                continue
-        # ---------------------------------------------------------------------
-        sent_start = current_pos
+                continue  
+        #---------------------------------------------------------------------
+        sent_start = current_pos 
         sent_end = current_pos + len(sent_text)
         sent_obj = Sentence(sent_start, sent_end, sent_text)
         sent_obj.set_num(i)
-
-        doc_obj.add_sentence(sent_obj)
-
-        # Usually sentences are separated by ' ', so it is added 1 to the
-        # current position but in some cases this is not true
-        current_pos += len(sent_text)
         
-        if i > 0:
-            current_pos += 1
+        doc_obj.add_sentence(sent_obj) 
 
+        # Usually sentences are separated by ' ', so it is added 1 to the 
+        # current position but in some cases this is not true
+        current_pos += len(sent_text) + 1
+    
     return doc_obj
 
 
-def _objectify_entities(entities, sent_pos, includes_links=False):
+def objectify_entities(entities, sent_pos, includes_links=False):
     """Convert inputted recognized entities into Entity objects.
 
     :param entities: entities to be objectified
     :type entities: list
-    :param sent_pos: the position of the sentence where the input entities
-        were recognized relative to the source document
+    :param sent_pos: the position of the sentence where the input entities 
+        were recognized relative to the source document 
     :type sent_pos: int
-    :param includes_links: specifies if there are knowledge based identifiers
+    :param includes_links: specifies if there are knowledge based identifiers 
         associated with the input entities, defaults to False
     :type includes_links: bool, optional
-    :return: entities_obj including the Entity objects relative to the input
-        entities
+    :return: entities_obj including the Entity objects relative to the input 
+        entities 
     :rtype: list
     """
 
     entities_obj = []
 
     for entity in entities:
         kb_id = None
 
         if len(entity) == 2:
-            entity_obj = Entity(None, None, entity[0], entity[1], None, None, None)
+            entity_obj = Entity(None, None, entity[0], entity[1], None, None, 
+                None)
 
         elif len(entity) > 2:
 
             if includes_links:
                 kb_id = entity[4]
                 entity_obj = Entity(
-                    entity[0],
-                    entity[1],
-                    entity[2],
-                    entity[3],
-                    kb_id,
-                    entity[5],
-                    sent_pos,
-                )
-
+                    entity[0], entity[1], entity[2], entity[3], kb_id, 
+                    entity[5], sent_pos)
+            
             else:
                 kb_id = None
                 entity_obj = Entity(
-                    entity[0],
-                    entity[1],
-                    entity[2],
-                    entity[3],
-                    kb_id,
-                    entity[4],
-                    sent_pos,
-                )
-
+                    entity[0], entity[1], entity[2], entity[3], kb_id, 
+                    entity[4], sent_pos)
+            
         entities_obj.append(entity_obj)
 
     return entities_obj
 
 
-# ------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #                        FORMAT OUTPUT
-# ------------------------------------------------------------------------------
-def _prepare_output_from_objects(doc, only_ner=True):
-    """Output given dataset in BRAT format to the given directory"""
+#------------------------------------------------------------------------------
 
-    doc_annots = ""
-    normalizations = ""
+def prepare_output_from_objects(doc, only_ner=True):
+    """Output given dataset in BRAT format to the given directory"""
 
+    doc_annots = ''
+    normalizations = ''
+    
     for i, entity in enumerate(doc.entities):
-        annot_id = str(i + 1)
-        doc_annots += f"T{annot_id}\t{entity.type} {entity.start} {entity.end}\t{entity.text}\n"
+        doc_annots += 'T{}\t{} {} {}\t{}\n'.format(
+            str(i+1), entity.type, entity.start, entity.end, entity.text) 
 
         if not only_ner:
-            normalizations += f"N{annot_id}\tReference T{annot_id} {entity.kb_id}\t{entity.text}\n"
+            normalizations += 'N{}\tReference T{} {}\t{}\n'.format(
+                str(i+1), str(i+1), entity.kb_id, entity.text)
 
     if not only_ner:
         doc_annots += normalizations
-
-    return doc_annots
+    
+    return doc_annots   
 
 
-def _merge_dicts(dict1, dict2):
-
+def merge_dicts(dict1, dict2):
+    
     dict3 = {}
     overlapping_keys = dict1.keys() & dict2.keys()
 
     for key in overlapping_keys:
-        dict3[key] = _merge_dicts(dict1[key], dict2[key])
+        dict3[key] = merge_dicts(dict1[key], dict2[key])
 
     for key in dict1.keys() - overlapping_keys:
         dict3[key] = deepcopy(dict1[key])
 
     for key in dict2.keys() - overlapping_keys:
         dict3[key] = deepcopy(dict2[key])
 
     return dict3
 
 
-def _import_reel_results(doc_id, nel_run_ids):
-    """Parse the results outputted by REEL-NILINKER for given document from
+def import_reel_results(doc_id, nel_run_ids):
+    """Parse the results outputted by REEL-NILINKER for given document from 
     file into a dictionary.
 
-    :param doc_id: the identifier of the document where the entities were
-        recognized
+    :param doc_id: the identifier of the document where the entities were 
+        recognized 
     :type doc_id: str
-    :param nel_run_ids: identifiers that allow the parsing of the output of the
+    :param nel_run_ids: identifiers that allow the parsing of the output of the 
         Named Entity Linking step from files
     :type nel_run_ids: list
     :return: linked_entities with format: {'entity_text': 'kb_id'}
     :rtype: dict
     """
-
+    
     linked_entities = {}
 
     for run_id in nel_run_ids:
-        results_dir = f"{cfg.tmp_dir}{run_id}/REEL/results/"
+        results_dir = '{}{}/REEL/results/'.format(cfg.tmp_dir, run_id)
         results_files = os.listdir(results_dir)
-        linked_entities_type = {}
-        ent_type = run_id.split("/")[1]
-        target_filename = f"{doc_id}.json"
+        linked_entities_type = {}       
+        ent_type = run_id.split('_')[1] 
+        target_filename = doc_id + '.json'
 
         if target_filename in results_files:
             filepath = results_dir + target_filename
-
-            with open(filepath, "r", encoding="utf-8") as infile:
+            
+            with open(filepath, 'r') as infile:
                 linked_entities_type = json.loads(infile.read())
                 infile.close()
 
         if linked_entities_type != {}:
             # Transform the keys of linked_entities_type
             linked_entities_type_up = {}
 
             for key in linked_entities_type.keys():
-                key_name = key + "_" + ent_type
+                key_name = key + '_' + ent_type
                 linked_entities_type_up[key_name] = linked_entities_type[key]
-
-            linked_entities = _merge_dicts(linked_entities, linked_entities_type_up)
-
+    
+            linked_entities = merge_dicts(
+                linked_entities, linked_entities_type_up)
+   
     return linked_entities
 
 
-def _update_dataset_with_nel_output(dataset, nel_run_ids):
-    """Update Dataset object containing recognized entities (Named Entity
-    Recognition step) with the output of the Named Entity Linking pipeline,
+def update_dataset_with_nel_output(dataset, nel_run_ids):
+    """Update Dataset object containing recognized entities (Named Entity 
+    Recognition step) with the output of the Named Entity Linking pipeline, 
     i.e. knowledge base identifiers for each recognized entity.
 
-    :param dataset: includes the output of the Named Entity Recognition
+    :param dataset: includes the output of the Named Entity Recognition 
         pipeline
     :type dataset: Dataset object
-    :param nel_run_ids: identifiers that allow the parsing of the output of the
+    :param nel_run_ids: identifiers that allow the parsing of the output of the 
         Named Entity Linking step from files
     :type nel_run_ids: list
     :return: updated dataset combining Named Entity Recognition + Linking
         outputs
     :rtype: Dataset object
     """
-
-    dataset_docs = dataset.documents
+    
+    dataset_docs = dataset.documents   
 
     for doc in dataset_docs:
-        linked_entities = _import_reel_results(doc.id, nel_run_ids)
-
+        linked_entities = import_reel_results(doc.id, nel_run_ids)
+        
         for i, sent in enumerate(doc.sentences):
             sent_entities = sent.entities
 
             for entity in sent_entities:
-                key_name = entity.text + "_" + entity.type
-
-                if key_name in linked_entities:
+                key_name = entity.text + '_' + entity.type
+                
+                if key_name in linked_entities.keys():
                     kb_id = linked_entities[key_name][0]
-                    entity.set_kb_id(kb_id)
+                    entity.set_kb_id(kb_id)        
                     sent.update_entity(entity)
-
+            
             doc.update_sentence(sent, i)
 
-    dataset.update_doc(doc, doc.id)
+    dataset.update_doc(doc, doc.id) 
 
-    return dataset
+    return dataset 
 
 
-def _update_ner_file_with_nel_output(ner_dir, nel_run_ids, out_dir=None):
+def update_ner_file_with_nel_output(ner_dir, nel_run_ids, out_dir=None):
     """Update annotations file generated in the Named Entity Recognition step
-    with the output of the Named Entity Linking pipeline, i.e. knowledge base
-    identifiers for each recognized entity. The generated annotations files
+    with the output of the Named Entity Linking pipeline, i.e. knowledge base 
+    identifiers for each recognized entity. The generated annotations files 
     will be located in the directory 'ner_dir'.
 
     :param ner_dir: path to directory where the recognized entities are
         stored in the annotations files
     :type ner_dir: str
-    :param nel_run_ids: identifiers that allow the parsing of the output of the
+    :param nel_run_ids: identifiers that allow the parsing of the output of the 
         Named Entity Linking step from files
     :type nel_run_ids: list
     :param out_format: the format of the ouput, defaults to 'brat'
     :type out_format: str, optional
     """
-
+        
     ner_filenames = os.listdir(ner_dir)
 
     for filename in ner_filenames:
-        doc_id = filename.strip(".ann")
-        linked_entities = _import_reel_results(doc_id, nel_run_ids)
-        complete_filepath = f"{ner_dir}{filename}"
-
-        with open(complete_filepath, "r", encoding="utf-8") as ner_file:
+        doc_id = filename.strip('.ann')
+        linked_entities = import_reel_results(doc_id, nel_run_ids)
+        complete_filepath = ner_dir + filename
+        
+        with open(complete_filepath, 'r') as ner_file:
             ner_output = ner_file.readlines()
             ner_file.close()
-
+   
         # Add the normalization lines to the annotations file
-        final_output = ""
-        
-        for line in ner_output:
+        final_output = ''
 
-            if line != "\n":
-                entity_text = line.split("\t")[2].strip("\n")
-                term_id = line.split("\t")[0]
-                entity_type = line.split("\t")[1].split(" ")[0]
+        for line in ner_output:
+            
+            if line != '\n':
+                entity_text = line.split('\t')[2].strip('\n')
+                term_id = line.split('\t')[0]
+                entity_type = line.split('\t')[1].split(' ')[0]
                 final_output += line
 
-                if final_output[-1:] != "\n":
-                    final_output += "\n"
-
-                key_name = f"{entity_text}"
+                if final_output[-1:] != '\n':
+                    final_output += '\n'
                 
-                if key_name in linked_entities and term_id[0] == "T":
+                key_name = entity_text + '_' + entity_type
+                
+                if key_name in linked_entities.keys() and term_id[0] == 'T':
                     kb_id = linked_entities[key_name][0]
-                    annot_id = term_id.split("T")[1]
-                    final_output += f"N{annot_id}\tReference {term_id} {kb_id}\t{entity_text}\n"
-            
-        if final_output[-1:] == "\n":
+                    final_output += 'N{}\tReference {} {}\t{}\n'.format(
+                        term_id.split('T')[1], term_id, kb_id, entity_text)
+        
+        if final_output[-1:] == '\n':
             final_output = final_output[:-1]
 
-        if out_dir is not None:
-            out_filepath = f"{out_dir}{filename}"
-            os.makedirs(out_dir, exist_ok=True)
-
-            with open(out_filepath, "w", encoding="utf-8") as out_file:
-                out_file.write(final_output)
-                out_file.close()
+        if out_dir != None:
+            out_filepath = out_dir + filename
+
+            if not os.path.exists(out_dir):
+                os.mkdir(out_dir)
+
+        with open(out_filepath, 'w' ) as out_file:
+            out_file.write(final_output)   
+            out_file.close()   
 
     # Delete temporary files associated with given run_ids
-    #for run_id in nel_run_ids:
-    #    dir_to_delete = cfg.tmp_dir + run_id
-    #    shutil.rmtree(dir_to_delete, ignore_errors=True)
+    for run_id in nel_run_ids:
+        dir_to_delete = cfg.tmp_dir + run_id
+        shutil.rmtree(dir_to_delete, ignore_errors=True)
 
 
-# ------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #                           OTHER
-# ------------------------------------------------------------------------------
-
+#------------------------------------------------------------------------------
 
 def garbage_collect(threshold=50.0):
     """Call the garbage collection if memory usage is greater than threshold.
 
-    :param threshold: amount of memory usage that triggers the garbage
+    :param threshold: amount of memory usage that triggers the garbage 
         collection, defaults to 50.0
     :type threshold: float, optional
     """
 
     if psutil.virtual_memory().percent >= threshold:
-        gc.collect()
-
-
-# Function to filter out the specific warning message
-def ignore_spacy_warning(message, category, filename, lineno, file=None, line=None):
-    return "Model 'en_core_sci_lg' (0.5.3) was trained with spaCy v3.6.1" in str(message)
+        gc.collect()
```

### Comparing `bent-0.0.55/bent.egg-info/PKG-INFO` & `bent-0.0.9/bent.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bent
-Version: 0.0.55
+Version: 0.0.9
 Summary: BENT: Biomedical Entity Annotator
 Home-page: https://github.com/lasigeBioTM/bent
 Author: Pedro Ruas
 Author-email: pedrosimruas@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -219,168 +219,124 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Unix Shell
 Classifier: Programming Language :: Java
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7, <=3.10.13
+Requires-Python: >=3.7
 License-File: LICENSE.txt
-Requires-Dist: obonet==0.3.0
-Requires-Dist: tensorflow-gpu==2.5.1; python_version < "3.10"
-Requires-Dist: tensorflow==2.13.1; python_version == "3.10"
-Requires-Dist: transformers==4.9.0; python_version < "3.10"
-Requires-Dist: transformers==4.35.2; python_version == "3.10"
-Requires-Dist: torch==1.9.1; python_version < "3.10"
-Requires-Dist: torch==2.0; python_version == "3.10"
-Requires-Dist: networkx==2.5.1
-Requires-Dist: gdown==4.6.0
-Requires-Dist: rapidfuzz==2.0.2
-Requires-Dist: tqdm==4.66
-Requires-Dist: spacy==3.0.1; python_version < "3.10"
-Requires-Dist: spacy==3.7.2; python_version == "3.10"
-Requires-Dist: seqeval==1.2.2
-Requires-Dist: orjson==3.8.5
-Requires-Dist: psutil
 
 
 
 BENT: Biomedical Entity Annotator
 ---------------------------------
 
 Python Library for Named Entity Recognition (NER) and Linking (NEL) in the biomedical domain.
 
+NER models are based on `PubMedBERT <https://arxiv.org/pdf/2007.15779.pdf>`__ and a post-processing rule-based module.
+the NEL model is a graph-based approach based on the Personalized PageRank algorithm and Information content.
+
 BENT can be used for: 
 
 * Named Entity Recogniton (NER)
 * Named Entity Linking (NEL) 
 * Named Entity Recognition and Linking (NER+NEL)
 
-Access the full `documentation <https://bent.readthedocs.io/en/latest/>`__.
+Access the full documentation `here <https://bent.readthedocs.io/en/latest/>`__.
 
-Citation::
+Citation:
 
-  Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking. 
-  Journal of Biomedical Informatics, 132:104137, 2022. 
-  doi: https://doi.org/10.1016/j.jbi.2022.104137.
+* Pedro Ruas and Francisco M. Couto. `Nilinker: attention-based approach to nil entity linking <https://www.sciencedirect.com/science/article/pii/S1532046422001526>`__. Journal of Biomedical Informatics, 132:104137, 2022. doi: https://doi.org/10.1016/j.jbi.2022.104137.
 
 Installation
-~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~
 
 To use the current version of BENT it is required: 
 
-*  OS: Debian>=11/Ubuntu>=20.04
-
-*  Python >=3.7, <=3.10.13
+* OS based on Ubuntu/Debian 
+* `Conda <https://docs.conda.io/en/latest/>`__ environment 
+* Python>=3.7
+* Between 11 and 15 GB free space (5 GB Anaconda + 2.5 GB to install dependencies + 3.0 GB data or 7.5 GB if you use all available knowlegde bases for NEL)
 
-*  Required space between 5.5 GB - 10 GB 
-   * Dependencies: 2.5 GB 
-   * Data: between 3.0 GB (base) or 7.5 GB (if you use all available knowledge bases for Named Entity Linking)
+.. note::
 
-**NOTE**: Python Docker images (3.7 to 3.9) in `Docker Hub <https://hub.docker.com/_/python>`__ have Debian 11 as the base OS.
+   Please ensure that you have the appropriate version of Conda installed.
 
 
-Install the BENT package using pip:
+Create a Conda environment (adapt for the name of your project):
 
 ::
 
-   pip install bent
+   conda create --name annotation_project python=3.7
 
 
-The following knowledge bases can be configured:
+Activate the environment:
 
-* 'medic' (`MEDIC <http://ctdbase.org/>`__)
+::
 
-* 'do' (`Disease ontology <https://disease-ontology.org/>`__)
+   conda activate annotation_project
 
-* 'chebi' (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
-* 'ctd_chem' (`CTD-Chemicals <http://ctdbase.org/>`__)
+Install the BENT package using pip:
 
-* 'ncbi_gene' (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
+::
 
-* 'ctd_gene' (`CTD-GENES <http://ctdbase.org/>`__)
+   pip install bent
 
-* 'ncbi_taxon' (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
-* 'go_bp' (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
+After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Specify the knowledge bases that will be used:
 
-* 'ctd_anat' (`CTD-Anatomy <http://ctdbase.org/>`__)
+::
 
-* 'fma' (`Foundation model of Anatomy <http://sig.biostr.washington.edu/projects/fm/AboutFM.html>`__)
+   python -c "from bent.setup_package import setup_package;setup_package([<kb1>, <kb2>, <kb3>])"
 
-* 'uberon' (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
+Available knowledge bases:
 
-* 'go_cc' (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
+* ‘medic’ (`MEDIC <http://ctdbase.org/>`__)
 
-* 'cell_ontology' (`Cell Ontology <https://cell-ontology.github.io/>`__)
+* ‘do’ (`Disease ontology <https://disease-ontology.org/>`__)
 
-* 'cellosaurus' (`Cellosaurus <https://www.cellosaurus.org/>`__)
+* 'chebi’ (`ChEBI ontology <https://www.ebi.ac.uk/chebi/>`__) 
 
+* ‘ctd_chem’ (`CTD-Chemicals <http://ctdbase.org/>`__)
 
-After the pip installation, it is required a further step to install non-Python dependencies and to download the necessary data. Run in the command line:
+* ‘ncbi_gene’ (`NCBI Gene <https://www.ncbi.nlm.nih.gov/gene/>`__)
 
-::
+* ‘ctd_gene’ (`CTD-GENES <http://ctdbase.org/>`__)
 
-   bent_setup
+* ‘ncbi_taxon’ (`NCBI Taxonomy <https://www.ncbi.nlm.nih.gov/taxonomy>`__)
 
+* ‘go_bp’ (`Gene Ontology-Biological Process <http://geneontology.org/>`__)
 
-Only the default knowledge bases 'medic' and 'chebi' will be available at this point.
+* ‘ctd_anat’ (`CTD-Anatomy <http://ctdbase.org/>`__)
 
-To disable annoyng messages in the terminal run:
+* ‘uberon’ (`UBERON ontology <http://obophenotype.github.io/uberon/>`__)
 
-::
+* ‘go_cc’ (`Gene Ontology-Cellular Component <http://geneontology.org/>`__)
 
-   export TF_CPP_MIN_LOG_LEVEL='3'
+* ‘cell_ontology’ (`Cell Ontology <https://cell-ontology.github.io/>`__)
 
+* cellosaurus’ (`Cellosaurus <https://www.cellosaurus.org/>`__)
 
-You can download more knowledge bases later by specifying the desired knowledge bases among the ones that are available:
+Example to download only the MEDIC vocabulary:
 
 ::
 
-   python -c "from bent.get_kbs import get_additional_kbs;get_additional_kbs([<kb1>, <kb2>])"
-
-
-Example: to download the NCBI Taxonomy and the NCBI Gene run: 
-
-::    
+   python -c "from bent.setup_package import setup_package;setup_package(['medic'])"
 
-    python -c "from bent.get_kbs import get_additional_kbs;get_additional_kbs(['ncbi_taxon', 'ncbi_gene'])"
 
+If you want to download all knowledge bases, choose the option 'all':
 
-Get started
-~~~~~~~~~~~
-
-To apply the complete pipeline of entity extraction (NER+NEL) set the arguments:
+::
 
-* **recognize**: indicate that the NER module will be applied ('True')
-* **link**: indicate that the NEL module will be applied ('True')
-* **types**: entity types to recognize and the respective target knowledge bases.
-* **in_dir**: directory path containing the text files to be annotated (the directory must contain text files exclusively)
-* **out_dir**: the output directory that will contain the annotation files
+   python -c "from bent.setup_package import setup_package;setup_package(['all'])"
 
 
-Example:
+You can download more knowledge bases later by running the same command and specifying the desired knolwedge bases among the ones that are available and setting the argument ' only_kb_dicts' to True:
 
 ::
 
-   import bent.annotate as bt
-
-   bt.annotate(
-           recognize=True,
-           link=True,
-           types={
-            'disease': 'medic'
-            'chemical': 'chebi',
-            'gene': 'ncbi_gene',
-            'anatomical': 'uberon',
-            'cell_line': 'cellosaurus',
-            'bioprocess': 'go_bp'
-            },
-           in_dir='input/txt/',
-           out_dir='output/nel/'
-   )
-
+   python -c "from bent.setup_package import setup_package;setup_package([<kb>],  only_kb_dicts=True)"
 
-It is also possible to apply the pipeline (NER+NEL) to a string or a list or strings instantiated in the execution script.
 
-To see more usage examples, access the `documentation <https://bent.readthedocs.io/en/latest/usage.html>`__.
+Reinitiate the conda environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bent-0.0.55/bent.egg-info/SOURCES.txt` & `bent-0.0.9/bent.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 LICENSE.txt
-MANIFEST.in
 README.rst
 setup.py
 bent/__init__.py
 bent/annotate.py
 bent/get_data.sh
 bent/get_kb_dicts.sh
-bent/get_kbs.py
 bent/requirements.txt
+bent/setup_package.py
 bent/setup_package.sh
-bent/setup_package_wrapper.py
 bent.egg-info/PKG-INFO
 bent.egg-info/SOURCES.txt
 bent.egg-info/dependency_links.txt
-bent.egg-info/entry_points.txt
 bent.egg-info/requires.txt
 bent.egg-info/top_level.txt
 bent/src/__init__.py
 bent/src/cfg.py
 bent/src/classes.py
 bent/src/nel.py
 bent/src/ner.py
@@ -33,15 +30,15 @@
 bent/src/REEL/ppr_for_ned_all.class
 bent/src/REEL/ppr_for_ned_all.java
 bent/src/REEL/pre_process.py
 bent/src/REEL/run.py
 bent/src/REEL/utils.py
 bent/src/abbreviation_detector/__init__.py
 bent/src/abbreviation_detector/run.py
-bent/src/dicts/__init__.py
-bent/src/dicts/annotations/__init__.py
-bent/src/dicts/annotations/dataset_entities.py
-bent/src/dicts/kb/__init__.py
-bent/src/dicts/kb/generate_dicts.py
-bent/src/dicts/kb/kb.py
-bent/src/dicts/relation_extraction/__init__.py
-bent/src/dicts/relation_extraction/dicts.py
+bent/src/setup/__init__.py
+bent/src/setup/annotations/__init__.py
+bent/src/setup/annotations/dataset_entities.py
+bent/src/setup/kb/__init__.py
+bent/src/setup/kb/generate_dicts.py
+bent/src/setup/kb/kb.py
+bent/src/setup/relation_extraction/__init__.py
+bent/src/setup/relation_extraction/dicts.py
```

