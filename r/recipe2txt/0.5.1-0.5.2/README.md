# Comparing `tmp/recipe2txt-0.5.1.tar.gz` & `tmp/recipe2txt-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recipe2txt-0.5.1.tar", last modified: Mon Apr  1 20:30:48 2024, max compression
+gzip compressed data, was "recipe2txt-0.5.2.tar", last modified: Thu May  2 15:01:20 2024, max compression
```

## Comparing `recipe2txt-0.5.1.tar` & `recipe2txt-0.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-04-01 20:30:48.742472 recipe2txt-0.5.1/
--rw-rw-r--   0 pc        (1000) pc        (1000)    35149 2023-07-25 13:15:25.000000 recipe2txt-0.5.1/LICENSE
--rw-r--r--   0 pc        (1000) pc        (1000)     9818 2024-04-01 20:30:48.742472 recipe2txt-0.5.1/PKG-INFO
--rw-rw-r--   0 pc        (1000) pc        (1000)     8295 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/README.md
--rw-rw-r--   0 pc        (1000) pc        (1000)     3541 2024-04-01 20:29:15.000000 recipe2txt-0.5.1/pyproject.toml
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-04-01 20:30:48.734472 recipe2txt-0.5.1/recipe2txt/
--rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-07-11 12:26:00.000000 recipe2txt-0.5.1/recipe2txt/__init__.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     7243 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/fetcher.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3380 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/fetcher_async.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    10409 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/file_setup.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    15310 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/html2recipe.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     9424 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/parsing_error.py
--rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-03-10 13:56:18.000000 recipe2txt-0.5.1/recipe2txt/py.typed
--rw-rw-r--   0 pc        (1000) pc        (1000)     2796 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/re2txt.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     4044 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/recipes2out.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    15720 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/sql.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    10197 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/user_interface.py
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-04-01 20:30:48.738472 recipe2txt-0.5.1/recipe2txt/utils/
--rw-rw-r--   0 pc        (1000) pc        (1000)    18860 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/utils/ArgConfig.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    11731 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/utils/ContextLogger.py
--rw-rw-r--   0 pc        (1000) pc        (1000)        0 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/utils/__init__.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     1259 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/utils/conditional_imports.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    11029 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/recipe2txt/utils/filesystem.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     4320 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/utils/markdown.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     6242 2024-04-01 18:59:04.000000 recipe2txt-0.5.1/recipe2txt/utils/misc.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3158 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/recipe2txt/utils/traceback_utils.py
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-04-01 20:30:48.738472 recipe2txt-0.5.1/recipe2txt.egg-info/
--rw-r--r--   0 pc        (1000) pc        (1000)     9818 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/PKG-INFO
--rw-rw-r--   0 pc        (1000) pc        (1000)     1037 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/SOURCES.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)        1 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/dependency_links.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       86 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/entry_points.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)      219 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/requires.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       11 2024-04-01 20:30:48.000000 recipe2txt-0.5.1/recipe2txt.egg-info/top_level.txt
--rw-rw-r--   0 pc        (1000) pc        (1000)       38 2024-04-01 20:30:48.742472 recipe2txt-0.5.1/setup.cfg
-drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-04-01 20:30:48.738472 recipe2txt-0.5.1/test/
--rw-rw-r--   0 pc        (1000) pc        (1000)     8844 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test4recipe2txt.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    17183 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_argconfig.py
--rw-rw-r--   0 pc        (1000) pc        (1000)    15340 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_contextlogger.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3042 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_fetcher.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     5203 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_file_setup.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     6434 2024-04-01 20:25:12.000000 recipe2txt-0.5.1/test/test_filestystem.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     6174 2024-04-01 20:25:12.000000 recipe2txt-0.5.1/test/test_helpers.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     4635 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/test/test_html2recipe.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     2958 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_misc.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3094 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_recipes2out.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     9851 2024-04-01 12:26:24.000000 recipe2txt-0.5.1/test/test_sql.py
--rw-rw-r--   0 pc        (1000) pc        (1000)     3389 2024-02-12 10:23:25.000000 recipe2txt-0.5.1/test/test_traceback_utils.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-05-02 15:01:20.231512 recipe2txt-0.5.2/
+-rw-rw-r--   0 pc        (1000) pc        (1000)    35149 2023-07-25 13:15:25.000000 recipe2txt-0.5.2/LICENSE
+-rw-r--r--   0 pc        (1000) pc        (1000)     9818 2024-05-02 15:01:20.227512 recipe2txt-0.5.2/PKG-INFO
+-rw-rw-r--   0 pc        (1000) pc        (1000)     8295 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/README.md
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3541 2024-05-02 13:56:36.000000 recipe2txt-0.5.2/pyproject.toml
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-05-02 15:01:20.219512 recipe2txt-0.5.2/recipe2txt/
+-rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-07-11 12:26:00.000000 recipe2txt-0.5.2/recipe2txt/__init__.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     7243 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/recipe2txt/fetcher.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3380 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/recipe2txt/fetcher_async.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    10409 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/recipe2txt/file_setup.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    15310 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/recipe2txt/html2recipe.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     9424 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/recipe2txt/parsing_error.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)        0 2023-03-10 13:56:18.000000 recipe2txt-0.5.2/recipe2txt/py.typed
+-rw-rw-r--   0 pc        (1000) pc        (1000)     2796 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/recipe2txt/re2txt.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4044 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/recipe2txt/recipes2out.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    15720 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/recipe2txt/sql.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    10197 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/recipe2txt/user_interface.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-05-02 15:01:20.223513 recipe2txt-0.5.2/recipe2txt/utils/
+-rw-rw-r--   0 pc        (1000) pc        (1000)    18860 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/recipe2txt/utils/ArgConfig.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    11731 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/recipe2txt/utils/ContextLogger.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)        0 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/recipe2txt/utils/__init__.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1259 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/recipe2txt/utils/conditional_imports.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    11029 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/recipe2txt/utils/filesystem.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4320 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/recipe2txt/utils/markdown.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     6242 2024-04-01 18:59:04.000000 recipe2txt-0.5.2/recipe2txt/utils/misc.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3158 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/recipe2txt/utils/traceback_utils.py
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-05-02 15:01:20.227512 recipe2txt-0.5.2/recipe2txt.egg-info/
+-rw-r--r--   0 pc        (1000) pc        (1000)     9818 2024-05-02 15:01:20.000000 recipe2txt-0.5.2/recipe2txt.egg-info/PKG-INFO
+-rw-rw-r--   0 pc        (1000) pc        (1000)     1037 2024-05-02 15:01:20.000000 recipe2txt-0.5.2/recipe2txt.egg-info/SOURCES.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)        1 2024-05-02 15:01:20.000000 recipe2txt-0.5.2/recipe2txt.egg-info/dependency_links.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       86 2024-05-02 15:01:20.000000 recipe2txt-0.5.2/recipe2txt.egg-info/entry_points.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)      219 2024-05-02 15:01:20.000000 recipe2txt-0.5.2/recipe2txt.egg-info/requires.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       11 2024-05-02 15:01:20.000000 recipe2txt-0.5.2/recipe2txt.egg-info/top_level.txt
+-rw-rw-r--   0 pc        (1000) pc        (1000)       38 2024-05-02 15:01:20.231512 recipe2txt-0.5.2/setup.cfg
+drwxrwxr-x   0 pc        (1000) pc        (1000)        0 2024-05-02 15:01:20.227512 recipe2txt-0.5.2/test/
+-rw-rw-r--   0 pc        (1000) pc        (1000)     8844 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/test/test4recipe2txt.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    17183 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/test/test_argconfig.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)    15340 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/test/test_contextlogger.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3042 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/test/test_fetcher.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     5203 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/test/test_file_setup.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     6434 2024-04-01 20:25:12.000000 recipe2txt-0.5.2/test/test_filestystem.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     6174 2024-04-01 20:25:12.000000 recipe2txt-0.5.2/test/test_helpers.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     4635 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/test/test_html2recipe.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     2958 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/test/test_misc.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3094 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/test/test_recipes2out.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     9851 2024-04-01 12:26:24.000000 recipe2txt-0.5.2/test/test_sql.py
+-rw-rw-r--   0 pc        (1000) pc        (1000)     3389 2024-02-12 10:23:25.000000 recipe2txt-0.5.2/test/test_traceback_utils.py
```

### Comparing `recipe2txt-0.5.1/LICENSE` & `recipe2txt-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/PKG-INFO` & `recipe2txt-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe2txt
-Version: 0.5.1
+Version: 0.5.2
 Summary: Scrapes recipes and converts them to txt or markdown
 Author-email: Jan Philipp Berg <git.7ksst@aleeas.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/jp-berg/recipe2txt
 Project-URL: Bug Tracker, https://github.com/jp-berg/recipe2txt/issues
 Keywords: recipes,cooking,scraping,website
 Classifier: Programming Language :: Python :: 3
@@ -25,18 +25,18 @@
 License-File: LICENSE
 Requires-Dist: aiodns~=3.2
 Requires-Dist: aiohttp~=3.9
 Requires-Dist: backports.strenum~=1.2; python_version < "3.11"
 Requires-Dist: importlib-metadata~=7.1
 Requires-Dist: jinja2~=3.1
 Requires-Dist: lxml==5.0.2
-Requires-Dist: recipe-scrapers~=14.55
+Requires-Dist: recipe-scrapers~=14.56
 Requires-Dist: tomli~=2.0; python_version < "3.11"
 Requires-Dist: typing_extensions~=4.6.2; python_version < "3.11"
-Requires-Dist: validators~=0.24
+Requires-Dist: validators~=0.28
 Requires-Dist: xdg-base-dirs~=6.0
 
 # Introduction
 
 `recipe2txt` is a CLI-program that you can feed your urls of recipes and it spits out formatted cookbooks containing those recipes. Highlights include:
 
 * asynchronous fetching of recipes
```

### Comparing `recipe2txt-0.5.1/README.md` & `recipe2txt-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/pyproject.toml` & `recipe2txt-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "recipe2txt"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Jan Philipp Berg", email="git.7ksst@aleeas.com" },
 ]
 description = "Scrapes recipes and converts them to txt or markdown"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
@@ -37,18 +37,18 @@
 dependencies = [
   "aiodns ~= 3.2",
   "aiohttp ~= 3.9",
   "backports.strenum ~= 1.2; python_version < '3.11'",
   "importlib-metadata ~= 7.1",
   "jinja2 ~= 3.1",
   "lxml == 5.0.2",
-  "recipe-scrapers ~= 14.55",
+  "recipe-scrapers ~= 14.56",
   "tomli ~= 2.0; python_version < '3.11'",
   "typing_extensions ~= 4.6.2; python_version < '3.11'",
-  "validators ~= 0.24",
+  "validators ~= 0.28",
   "xdg-base-dirs ~= 6.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jp-berg/recipe2txt"
 "Bug Tracker" = "https://github.com/jp-berg/recipe2txt/issues"
```

### Comparing `recipe2txt-0.5.1/recipe2txt/fetcher.py` & `recipe2txt-0.5.2/recipe2txt/fetcher.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/fetcher_async.py` & `recipe2txt-0.5.2/recipe2txt/fetcher_async.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/file_setup.py` & `recipe2txt-0.5.2/recipe2txt/file_setup.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/html2recipe.py` & `recipe2txt-0.5.2/recipe2txt/html2recipe.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/parsing_error.py` & `recipe2txt-0.5.2/recipe2txt/parsing_error.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/re2txt.py` & `recipe2txt-0.5.2/recipe2txt/re2txt.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/recipes2out.py` & `recipe2txt-0.5.2/recipe2txt/recipes2out.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/sql.py` & `recipe2txt-0.5.2/recipe2txt/sql.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/user_interface.py` & `recipe2txt-0.5.2/recipe2txt/user_interface.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/utils/ArgConfig.py` & `recipe2txt-0.5.2/recipe2txt/utils/ArgConfig.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/utils/ContextLogger.py` & `recipe2txt-0.5.2/recipe2txt/utils/ContextLogger.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/utils/conditional_imports.py` & `recipe2txt-0.5.2/recipe2txt/utils/conditional_imports.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/utils/filesystem.py` & `recipe2txt-0.5.2/recipe2txt/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/utils/markdown.py` & `recipe2txt-0.5.2/recipe2txt/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/utils/misc.py` & `recipe2txt-0.5.2/recipe2txt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt/utils/traceback_utils.py` & `recipe2txt-0.5.2/recipe2txt/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/recipe2txt.egg-info/PKG-INFO` & `recipe2txt-0.5.2/recipe2txt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe2txt
-Version: 0.5.1
+Version: 0.5.2
 Summary: Scrapes recipes and converts them to txt or markdown
 Author-email: Jan Philipp Berg <git.7ksst@aleeas.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/jp-berg/recipe2txt
 Project-URL: Bug Tracker, https://github.com/jp-berg/recipe2txt/issues
 Keywords: recipes,cooking,scraping,website
 Classifier: Programming Language :: Python :: 3
@@ -25,18 +25,18 @@
 License-File: LICENSE
 Requires-Dist: aiodns~=3.2
 Requires-Dist: aiohttp~=3.9
 Requires-Dist: backports.strenum~=1.2; python_version < "3.11"
 Requires-Dist: importlib-metadata~=7.1
 Requires-Dist: jinja2~=3.1
 Requires-Dist: lxml==5.0.2
-Requires-Dist: recipe-scrapers~=14.55
+Requires-Dist: recipe-scrapers~=14.56
 Requires-Dist: tomli~=2.0; python_version < "3.11"
 Requires-Dist: typing_extensions~=4.6.2; python_version < "3.11"
-Requires-Dist: validators~=0.24
+Requires-Dist: validators~=0.28
 Requires-Dist: xdg-base-dirs~=6.0
 
 # Introduction
 
 `recipe2txt` is a CLI-program that you can feed your urls of recipes and it spits out formatted cookbooks containing those recipes. Highlights include:
 
 * asynchronous fetching of recipes
```

### Comparing `recipe2txt-0.5.1/recipe2txt.egg-info/SOURCES.txt` & `recipe2txt-0.5.2/recipe2txt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test4recipe2txt.py` & `recipe2txt-0.5.2/test/test4recipe2txt.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_argconfig.py` & `recipe2txt-0.5.2/test/test_argconfig.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_contextlogger.py` & `recipe2txt-0.5.2/test/test_contextlogger.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_fetcher.py` & `recipe2txt-0.5.2/test/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_file_setup.py` & `recipe2txt-0.5.2/test/test_file_setup.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_filestystem.py` & `recipe2txt-0.5.2/test/test_filestystem.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_helpers.py` & `recipe2txt-0.5.2/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_html2recipe.py` & `recipe2txt-0.5.2/test/test_html2recipe.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_misc.py` & `recipe2txt-0.5.2/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_recipes2out.py` & `recipe2txt-0.5.2/test/test_recipes2out.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_sql.py` & `recipe2txt-0.5.2/test/test_sql.py`

 * *Files identical despite different names*

### Comparing `recipe2txt-0.5.1/test/test_traceback_utils.py` & `recipe2txt-0.5.2/test/test_traceback_utils.py`

 * *Files identical despite different names*

