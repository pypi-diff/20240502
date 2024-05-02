# Comparing `tmp/report_creator-1.0.8.tar.gz` & `tmp/report_creator-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report_creator-1.0.8.tar", last modified: Mon Apr 22 00:01:39 2024, max compression
+gzip compressed data, was "report_creator-1.0.9.tar", last modified: Mon Apr 22 00:09:10 2024, max compression
```

## Comparing `report_creator-1.0.8.tar` & `report_creator-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:01:39.161110 report_creator-1.0.8/
--rw-r--r--   0 drace      (501) staff       (20)     1066 2024-04-20 05:46:16.000000 report_creator-1.0.8/LICENSE
--rw-r--r--   0 drace      (501) staff       (20)       69 2024-04-19 02:06:16.000000 report_creator-1.0.8/MANIFEST.in
--rw-r--r--   0 drace      (501) staff       (20)     4406 2024-04-22 00:01:39.161050 report_creator-1.0.8/PKG-INFO
--rw-r--r--   0 drace      (501) staff       (20)     3300 2024-04-20 05:46:16.000000 report_creator-1.0.8/README.md
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:01:39.159828 report_creator-1.0.8/report_creator/
--rw-r--r--   0 drace      (501) staff       (20)      478 2024-04-19 02:06:16.000000 report_creator-1.0.8/report_creator/__init__.py
--rw-r--r--   0 drace      (501) staff       (20)      174 2024-04-22 00:01:33.000000 report_creator-1.0.8/report_creator/__meta__.py
--rw-r--r--   0 drace      (501) staff       (20)    45428 2024-04-19 02:06:16.000000 report_creator-1.0.8/report_creator/report_creator.py
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:01:39.160540 report_creator-1.0.8/report_creator/templates/
--rw-r--r--   0 drace      (501) staff       (20)    10528 2024-04-19 02:06:16.000000 report_creator-1.0.8/report_creator/templates/default.html
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:01:39.160850 report_creator-1.0.8/report_creator.egg-info/
--rw-r--r--   0 drace      (501) staff       (20)     4406 2024-04-22 00:01:39.000000 report_creator-1.0.8/report_creator.egg-info/PKG-INFO
--rw-r--r--   0 drace      (501) staff       (20)      362 2024-04-22 00:01:39.000000 report_creator-1.0.8/report_creator.egg-info/SOURCES.txt
--rw-r--r--   0 drace      (501) staff       (20)        1 2024-04-22 00:01:39.000000 report_creator-1.0.8/report_creator.egg-info/dependency_links.txt
--rw-r--r--   0 drace      (501) staff       (20)      102 2024-04-22 00:01:39.000000 report_creator-1.0.8/report_creator.egg-info/requires.txt
--rw-r--r--   0 drace      (501) staff       (20)       15 2024-04-22 00:01:39.000000 report_creator-1.0.8/report_creator.egg-info/top_level.txt
--rw-r--r--   0 drace      (501) staff       (20)     1079 2024-04-22 00:01:39.161353 report_creator-1.0.8/setup.cfg
--rw-r--r--   0 drace      (501) staff       (20)     2113 2024-04-22 00:01:13.000000 report_creator-1.0.8/setup.py
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:09:10.284682 report_creator-1.0.9/
+-rw-r--r--   0 drace      (501) staff       (20)     1066 2024-04-20 05:46:16.000000 report_creator-1.0.9/LICENSE
+-rw-r--r--   0 drace      (501) staff       (20)       69 2024-04-19 02:06:16.000000 report_creator-1.0.9/MANIFEST.in
+-rw-r--r--   0 drace      (501) staff       (20)     4406 2024-04-22 00:09:10.284620 report_creator-1.0.9/PKG-INFO
+-rw-r--r--   0 drace      (501) staff       (20)     3300 2024-04-20 05:46:16.000000 report_creator-1.0.9/README.md
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:09:10.283413 report_creator-1.0.9/report_creator/
+-rw-r--r--   0 drace      (501) staff       (20)      478 2024-04-19 02:06:16.000000 report_creator-1.0.9/report_creator/__init__.py
+-rw-r--r--   0 drace      (501) staff       (20)      174 2024-04-22 00:09:06.000000 report_creator-1.0.9/report_creator/__meta__.py
+-rw-r--r--   0 drace      (501) staff       (20)    45428 2024-04-19 02:06:16.000000 report_creator-1.0.9/report_creator/report_creator.py
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:09:10.284230 report_creator-1.0.9/report_creator/templates/
+-rw-r--r--   0 drace      (501) staff       (20)    10528 2024-04-19 02:06:16.000000 report_creator-1.0.9/report_creator/templates/default.html
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:09:10.284424 report_creator-1.0.9/report_creator.egg-info/
+-rw-r--r--   0 drace      (501) staff       (20)     4406 2024-04-22 00:09:10.000000 report_creator-1.0.9/report_creator.egg-info/PKG-INFO
+-rw-r--r--   0 drace      (501) staff       (20)      362 2024-04-22 00:09:10.000000 report_creator-1.0.9/report_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 drace      (501) staff       (20)        1 2024-04-22 00:09:10.000000 report_creator-1.0.9/report_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 drace      (501) staff       (20)      102 2024-04-22 00:09:10.000000 report_creator-1.0.9/report_creator.egg-info/requires.txt
+-rw-r--r--   0 drace      (501) staff       (20)       15 2024-04-22 00:09:10.000000 report_creator-1.0.9/report_creator.egg-info/top_level.txt
+-rw-r--r--   0 drace      (501) staff       (20)     1079 2024-04-22 00:09:10.284918 report_creator-1.0.9/setup.cfg
+-rw-r--r--   0 drace      (501) staff       (20)     2114 2024-04-22 00:08:40.000000 report_creator-1.0.9/setup.py
```

### Comparing `report_creator-1.0.8/LICENSE` & `report_creator-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.8/PKG-INFO` & `report_creator-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report_creator
-Version: 1.0.8
+Version: 1.0.9
 Summary: Produce self-contained HTML reports from Python
 Home-page: https://github.com/darenr/report_creator
 Author: Daren Race
 Author-email: daren.race@gmail.com
 License: MIT
 Keywords: python,html,reports,report,creator,generator,markdown,yaml,plot,chart,table
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `report_creator-1.0.8/README.md` & `report_creator-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.8/report_creator/report_creator.py` & `report_creator-1.0.9/report_creator/report_creator.py`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.8/report_creator/templates/default.html` & `report_creator-1.0.9/report_creator/templates/default.html`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.8/report_creator.egg-info/PKG-INFO` & `report_creator-1.0.9/report_creator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report_creator
-Version: 1.0.8
+Version: 1.0.9
 Summary: Produce self-contained HTML reports from Python
 Home-page: https://github.com/darenr/report_creator
 Author: Daren Race
 Author-email: daren.race@gmail.com
 License: MIT
 Keywords: python,html,reports,report,creator,generator,markdown,yaml,plot,chart,table
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `report_creator-1.0.8/setup.cfg` & `report_creator-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.8/setup.py` & `report_creator-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 def get_install_requires() -> List[str]:
     """Returns requirements.txt parsed to a list"""
     fname = Path(__file__).parent / "requirements.txt"
     targets = []
     if fname.exists():
         with open(fname) as f:
             targets = f.read().splitlines()
+
     return targets
 
 
 # get package metadata by parsing __meta__ module
 with open("report_creator/__meta__.py") as source:
     content = source.read().strip()
     metadata = {
```

