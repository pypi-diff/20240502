# Comparing `tmp/skillcorner-2.2.8.tar.gz` & `tmp/skillcorner-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillcorner-2.2.8.tar", max compression
+gzip compressed data, was "skillcorner-2.2.9.tar", max compression
```

## Comparing `skillcorner-2.2.8.tar` & `skillcorner-2.2.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2024-03-18 16:29:05.103165 skillcorner-2.2.8/LICENSE.md
--rw-r--r--   0        0        0     3824 2024-03-18 16:29:05.103165 skillcorner-2.2.8/README.md
--rw-r--r--   0        0        0     1078 2024-03-18 16:29:05.107165 skillcorner-2.2.8/pyproject.toml
--rw-r--r--   0        0        0     5030 2024-03-18 16:29:05.107165 skillcorner-2.2.8/skillcorner/client.py
--rw-r--r--   0        0        0     4590 1970-01-01 00:00:00.000000 skillcorner-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-02 12:30:00.181266 skillcorner-2.2.9/LICENSE.md
+-rw-r--r--   0        0        0     3824 2024-04-02 12:30:00.181266 skillcorner-2.2.9/README.md
+-rw-r--r--   0        0        0     1078 2024-04-02 12:30:00.181266 skillcorner-2.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5030 2024-04-02 12:30:00.181266 skillcorner-2.2.9/skillcorner/client.py
+-rw-r--r--   0        0        0     4590 1970-01-01 00:00:00.000000 skillcorner-2.2.9/PKG-INFO
```

### Comparing `skillcorner-2.2.8/LICENSE.md` & `skillcorner-2.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `skillcorner-2.2.8/README.md` & `skillcorner-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `skillcorner-2.2.8/pyproject.toml` & `skillcorner-2.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skillcorner"
-version = "2.2.8"
+version = "2.2.9"
 description = "Python client for interact with SkillCorner API"
 homepage = "https://skillcorner.com/"
 repository = "https://gitlab.com/public-corner/skillcorner"
 documentation = "https://skillcorner.readthedocs.io/en/latest/"
 authors = ["Skillcorner"]
 readme = "README.md"
```

### Comparing `skillcorner-2.2.8/skillcorner/client.py` & `skillcorner-2.2.9/skillcorner/client.py`

 * *Files identical despite different names*

### Comparing `skillcorner-2.2.8/PKG-INFO` & `skillcorner-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillcorner
-Version: 2.2.8
+Version: 2.2.9
 Summary: Python client for interact with SkillCorner API
 Home-page: https://skillcorner.com/
 Author: Skillcorner
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

