# Comparing `tmp/dfddnsclient-1.1.tar.gz` & `tmp/dfddnsclient-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfddnsclient-1.1.tar", last modified: Wed May  1 21:47:42 2024, max compression
+gzip compressed data, was "dfddnsclient-1.2.tar", last modified: Wed May  1 22:09:19 2024, max compression
```

## Comparing `dfddnsclient-1.1.tar` & `dfddnsclient-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 21:47:42.204145 dfddnsclient-1.1/
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 17:51:39.000000 dfddnsclient-1.1/LICENSE
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      263 2024-05-01 21:47:42.204017 dfddnsclient-1.1/PKG-INFO
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      248 2024-05-01 20:43:16.000000 dfddnsclient-1.1/README.md
-drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 21:47:42.203028 dfddnsclient-1.1/dfddnsclient/
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 17:50:48.000000 dfddnsclient-1.1/dfddnsclient/__init__.py
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)     2247 2024-05-01 20:44:31.000000 dfddnsclient-1.1/dfddnsclient/app.py
-drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 21:47:42.203802 dfddnsclient-1.1/dfddnsclient.egg-info/
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      263 2024-05-01 21:47:42.000000 dfddnsclient-1.1/dfddnsclient.egg-info/PKG-INFO
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      250 2024-05-01 21:47:42.000000 dfddnsclient-1.1/dfddnsclient.egg-info/SOURCES.txt
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        1 2024-05-01 21:47:42.000000 dfddnsclient-1.1/dfddnsclient.egg-info/dependency_links.txt
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       24 2024-05-01 21:47:42.000000 dfddnsclient-1.1/dfddnsclient.egg-info/requires.txt
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       13 2024-05-01 21:47:42.000000 dfddnsclient-1.1/dfddnsclient.egg-info/top_level.txt
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       38 2024-05-01 21:47:42.204202 dfddnsclient-1.1/setup.cfg
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      423 2024-05-01 21:45:20.000000 dfddnsclient-1.1/setup.py
+drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 22:09:19.682163 dfddnsclient-1.2/
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 17:51:39.000000 dfddnsclient-1.2/LICENSE
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      263 2024-05-01 22:09:19.682024 dfddnsclient-1.2/PKG-INFO
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      248 2024-05-01 22:07:55.000000 dfddnsclient-1.2/README.md
+drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 22:09:19.680983 dfddnsclient-1.2/dfddnsclient/
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 17:50:48.000000 dfddnsclient-1.2/dfddnsclient/__init__.py
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)     2247 2024-05-01 20:44:31.000000 dfddnsclient-1.2/dfddnsclient/app.py
+drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 22:09:19.681824 dfddnsclient-1.2/dfddnsclient.egg-info/
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      263 2024-05-01 22:09:19.000000 dfddnsclient-1.2/dfddnsclient.egg-info/PKG-INFO
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      250 2024-05-01 22:09:19.000000 dfddnsclient-1.2/dfddnsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        1 2024-05-01 22:09:19.000000 dfddnsclient-1.2/dfddnsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       24 2024-05-01 22:09:19.000000 dfddnsclient-1.2/dfddnsclient.egg-info/requires.txt
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       13 2024-05-01 22:09:19.000000 dfddnsclient-1.2/dfddnsclient.egg-info/top_level.txt
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       38 2024-05-01 22:09:19.682228 dfddnsclient-1.2/setup.cfg
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      436 2024-05-01 22:07:59.000000 dfddnsclient-1.2/setup.py
```

### Comparing `dfddnsclient-1.1/dfddnsclient/app.py` & `dfddnsclient-1.2/dfddnsclient/app.py`

 * *Files identical despite different names*

