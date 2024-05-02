# Comparing `tmp/t_bug_catcher-0.4.8.tar.gz` & `tmp/t_bug_catcher-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-ovp05d25/t_bug_catcher-0.4.8.tar", last modified: Wed May  1 07:10:25 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-_re2n7q4/t_bug_catcher-0.4.9.tar", last modified: Wed May  1 14:01:50 2024, max compression
```

## Comparing `t_bug_catcher-0.4.8.tar` & `t_bug_catcher-0.4.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1451 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/t_bug_catcher/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12348 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/bug_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/bug_snag.py
--rw-rw-rw-   0 root         (0) root         (0)     1537 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    50197 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/jira.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/t_bug_catcher/resources/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/resources/whispers_config.yml
--rw-rw-rw-   0 root         (0) root         (0)     5219 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/stack_saver.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/t_bug_catcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2633 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     4063 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/validation.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/t_bug_catcher/workitems.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1451 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-01 07:10:25.000000 t_bug_catcher-0.4.8/t_bug_catcher.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 07:10:25.473927 t_bug_catcher-0.4.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-05-01 07:09:58.000000 t_bug_catcher-0.4.8/tests/test_t_bug_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 14:01:50.575104 t_bug_catcher-0.4.9/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-01 14:01:50.575104 t_bug_catcher-0.4.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-05-01 14:01:50.575104 t_bug_catcher-0.4.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 14:01:50.571104 t_bug_catcher-0.4.9/t_bug_catcher/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12348 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/bug_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/bug_snag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    50197 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/jira.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 14:01:50.571104 t_bug_catcher-0.4.9/t_bug_catcher/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/resources/whispers_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5219 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/stack_saver.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 14:01:50.571104 t_bug_catcher-0.4.9/t_bug_catcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/t_bug_catcher/workitems.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 14:01:50.571104 t_bug_catcher-0.4.9/t_bug_catcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-01 14:01:50.000000 t_bug_catcher-0.4.9/t_bug_catcher.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-01 14:01:50.000000 t_bug_catcher-0.4.9/t_bug_catcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-01 14:01:50.000000 t_bug_catcher-0.4.9/t_bug_catcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-01 14:01:50.000000 t_bug_catcher-0.4.9/t_bug_catcher.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-01 14:01:50.000000 t_bug_catcher-0.4.9/t_bug_catcher.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-01 14:01:50.000000 t_bug_catcher-0.4.9/t_bug_catcher.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 14:01:50.571104 t_bug_catcher-0.4.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2024-05-01 14:01:17.000000 t_bug_catcher-0.4.9/tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.4.8/PKG-INFO` & `t_bug_catcher-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.8
+Version: 0.4.9
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.8/README.rst` & `t_bug_catcher-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.8/setup.py` & `t_bug_catcher-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     description="Bug catcher",
     long_description=readme,
     keywords="t_bug_catcher",
     name="t_bug_catcher",
     packages=find_packages(include=["t_bug_catcher", "t_bug_catcher.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.4.8",
+    version="0.4.9",
     zip_safe=False,
     install_requires=install_requirements,
     include_package_data=True,
     package_data={"": ["resources/*.yml"]},
 )
```

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher/bug_catcher.py` & `t_bug_catcher-0.4.9/t_bug_catcher/bug_catcher.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher/bug_snag.py` & `t_bug_catcher-0.4.9/t_bug_catcher/bug_snag.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher/config.py` & `t_bug_catcher-0.4.9/t_bug_catcher/config.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher/jira.py` & `t_bug_catcher-0.4.9/t_bug_catcher/jira.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher/resources/whispers_config.yml` & `t_bug_catcher-0.4.9/t_bug_catcher/resources/whispers_config.yml`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher/stack_saver.py` & `t_bug_catcher-0.4.9/t_bug_catcher/stack_saver.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher/utils/common.py` & `t_bug_catcher-0.4.9/t_bug_catcher/utils/common.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher/utils/logger.py` & `t_bug_catcher-0.4.9/t_bug_catcher/utils/logger.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher/validation.py` & `t_bug_catcher-0.4.9/t_bug_catcher/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 import logging
 import os
 
 from t_bug_catcher.utils.common import strip_path
 
 validation_logger = logging.getLogger("t_bug_catcher")
 
+validation_logger.setLevel(logging.DEBUG)
+console_handler = logging.StreamHandler()
+console_handler.setLevel(logging.DEBUG)
+
+formatter = logging.Formatter("%(levelname)s - %(name)s - %(message)s")
+validation_logger.addHandler(console_handler)
+
 EXCLUDED_DIRS = [".venv", "venv", "site-packages"]
 
 
 class IncorrectTryBlockVisitor(ast.NodeVisitor):
     """A visitor that checks for incorrect try-except blocks."""
 
     def __init__(self):
@@ -83,15 +90,21 @@
 
                     self.check_broad_exceptions(file_path)
 
     def check_broad_exceptions(self, filename):
         """Checks for broad exception warnings in the specified file."""
         with open(filename, "r", encoding="utf8") as source:
             source_code = source.read()
-            tree = ast.parse(source_code, filename=filename)
+            try:
+                tree = ast.parse(source_code, filename=filename)
+            except SyntaxError:
+                return
+            except Exception as ex:
+                validation_logger.error(f"Unable to validate: {filename} - {ex}")
+                return
 
         visitor = IncorrectTryBlockVisitor()
         visitor.visit(tree)
 
         for line, message in visitor.get_errors().items():
             be_warn = BroadExceptionWarning(filename, line, message, source_code=source_code)
             self.broad_exception_warnings.append(be_warn)
```

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher.egg-info/PKG-INFO` & `t_bug_catcher-0.4.9/t_bug_catcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.8
+Version: 0.4.9
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.8/t_bug_catcher.egg-info/SOURCES.txt` & `t_bug_catcher-0.4.9/t_bug_catcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.8/tests/test_t_bug_catcher.py` & `t_bug_catcher-0.4.9/tests/test_t_bug_catcher.py`

 * *Files identical despite different names*

