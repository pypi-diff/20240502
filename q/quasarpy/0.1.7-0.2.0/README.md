# Comparing `tmp/quasarpy-0.1.7.tar.gz` & `tmp/quasarpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasarpy-0.1.7.tar", max compression
+gzip compressed data, was "quasarpy-0.2.0.tar", max compression
```

## Comparing `quasarpy-0.1.7.tar` & `quasarpy-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    31941 2024-05-02 03:39:56.441356 quasarpy-0.1.7/LICENSE
--rw-r--r--   0        0        0     1843 2024-05-02 03:39:56.441356 quasarpy-0.1.7/README.md
--rw-r--r--   0        0        0  1387623 2024-05-02 03:39:56.441356 quasarpy-0.1.7/assets/logo_complete.png
--rw-r--r--   0        0        0   127970 2024-05-02 03:39:56.441356 quasarpy-0.1.7/assets/logo_complete_svg.svg
--rw-r--r--   0        0        0   182267 2024-05-02 03:39:56.445356 quasarpy-0.1.7/assets/logo_complete_tbg.png
--rw-r--r--   0        0        0   418415 2024-05-02 03:39:56.445356 quasarpy-0.1.7/assets/logo_icon.png
--rw-r--r--   0        0        0   166944 2024-05-02 03:39:56.445356 quasarpy-0.1.7/assets/logo_text.png
--rw-r--r--   0        0        0     1170 2024-05-02 03:39:56.449356 quasarpy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      673 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/__init__.py
--rw-r--r--   0        0        0       86 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/__main__.py
--rw-r--r--   0        0        0       21 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/_version.py
--rw-r--r--   0        0        0      177 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/algorithm/__init__.py
--rw-r--r--   0        0        0     5249 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/algorithm/detector.py
--rw-r--r--   0        0        0     2857 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/algorithm/llm.py
--rw-r--r--   0        0        0     7703 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/algorithm/model/class_model.json
--rw-r--r--   0        0        0     7703 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/algorithm/model/method_model.json
--rw-r--r--   0        0        0     4172 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/cli/__init__.py
--rw-r--r--   0        0        0       79 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/handler/__init__.py
--rw-r--r--   0        0        0     2586 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/handler/issue.py
--rw-r--r--   0        0        0        0 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/__init__.py
--rw-r--r--   0        0        0      389 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/conftest.py
--rw-r--r--   0        0        0        1 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/test_algorithm.py
--rw-r--r--   0        0        0        0 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/test_cli.py
--rw-r--r--   0        0        0      545 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/test_handler.py
--rw-r--r--   0        0        0      645 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/tests/test_utils.py
--rw-r--r--   0        0        0      508 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/__init__.py
--rw-r--r--   0        0        0     1864 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/analyser.py
--rw-r--r--   0        0        0     1322 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/ascii.py
--rw-r--r--   0        0        0      195 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/errors.py
--rw-r--r--   0        0        0      187 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/logger.py
--rw-r--r--   0        0        0     1030 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/prompt_template.py
--rw-r--r--   0        0        0     4524 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/redis_server.py
--rw-r--r--   0        0        0     2978 2024-05-02 03:39:56.449356 quasarpy-0.1.7/quasarpy/utils/templates/report_template.html
--rw-r--r--   0        0        0     3304 1970-01-01 00:00:00.000000 quasarpy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    31941 2024-05-02 04:19:26.209349 quasarpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1843 2024-05-02 04:19:26.209349 quasarpy-0.2.0/README.md
+-rw-r--r--   0        0        0  1387623 2024-05-02 04:19:26.213349 quasarpy-0.2.0/assets/logo_complete.png
+-rw-r--r--   0        0        0   127970 2024-05-02 04:19:26.213349 quasarpy-0.2.0/assets/logo_complete_svg.svg
+-rw-r--r--   0        0        0   182267 2024-05-02 04:19:26.213349 quasarpy-0.2.0/assets/logo_complete_tbg.png
+-rw-r--r--   0        0        0   418415 2024-05-02 04:19:26.217349 quasarpy-0.2.0/assets/logo_icon.png
+-rw-r--r--   0        0        0   166944 2024-05-02 04:19:26.217349 quasarpy-0.2.0/assets/logo_text.png
+-rw-r--r--   0        0        0     1170 2024-05-02 04:19:26.221349 quasarpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      673 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/__main__.py
+-rw-r--r--   0        0        0       21 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/_version.py
+-rw-r--r--   0        0        0      177 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/algorithm/__init__.py
+-rw-r--r--   0        0        0     5249 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/algorithm/detector.py
+-rw-r--r--   0        0        0     2857 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/algorithm/llm.py
+-rw-r--r--   0        0        0     7703 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/algorithm/model/class_model.json
+-rw-r--r--   0        0        0     7703 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/algorithm/model/method_model.json
+-rw-r--r--   0        0        0     4172 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/cli/__init__.py
+-rw-r--r--   0        0        0       79 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/handler/__init__.py
+-rw-r--r--   0        0        0     2708 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/handler/issue.py
+-rw-r--r--   0        0        0        0 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/tests/__init__.py
+-rw-r--r--   0        0        0      389 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/tests/conftest.py
+-rw-r--r--   0        0        0        1 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/tests/test_algorithm.py
+-rw-r--r--   0        0        0        0 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/tests/test_cli.py
+-rw-r--r--   0        0        0      545 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/tests/test_handler.py
+-rw-r--r--   0        0        0      645 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/tests/test_utils.py
+-rw-r--r--   0        0        0      508 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/utils/__init__.py
+-rw-r--r--   0        0        0     1864 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/utils/analyser.py
+-rw-r--r--   0        0        0     1322 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/utils/ascii.py
+-rw-r--r--   0        0        0      195 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/utils/errors.py
+-rw-r--r--   0        0        0      187 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/utils/logger.py
+-rw-r--r--   0        0        0     1030 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/utils/prompt_template.py
+-rw-r--r--   0        0        0     4524 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/utils/redis_server.py
+-rw-r--r--   0        0        0     2978 2024-05-02 04:19:26.221349 quasarpy-0.2.0/quasarpy/utils/templates/report_template.html
+-rw-r--r--   0        0        0     3304 1970-01-01 00:00:00.000000 quasarpy-0.2.0/PKG-INFO
```

### Comparing `quasarpy-0.1.7/LICENSE` & `quasarpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/README.md` & `quasarpy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/assets/logo_complete.png` & `quasarpy-0.2.0/assets/logo_complete.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/assets/logo_complete_svg.svg` & `quasarpy-0.2.0/assets/logo_complete_svg.svg`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/assets/logo_complete_tbg.png` & `quasarpy-0.2.0/assets/logo_complete_tbg.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/assets/logo_icon.png` & `quasarpy-0.2.0/assets/logo_icon.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/assets/logo_text.png` & `quasarpy-0.2.0/assets/logo_text.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/pyproject.toml` & `quasarpy-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quasarpy"
-version = "0.1.7"
+version = "0.2.0"
 description = "Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc."
 authors = ["Khushiyant <khushiyant2002@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 include = ["assets", 'LICENSE']
 
 [tool.poetry.scripts]
```

### Comparing `quasarpy-0.1.7/quasarpy/__init__.py` & `quasarpy-0.2.0/quasarpy/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/algorithm/detector.py` & `quasarpy-0.2.0/quasarpy/algorithm/detector.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/algorithm/llm.py` & `quasarpy-0.2.0/quasarpy/algorithm/llm.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/algorithm/model/class_model.json` & `quasarpy-0.2.0/quasarpy/algorithm/model/class_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/algorithm/model/method_model.json` & `quasarpy-0.2.0/quasarpy/algorithm/model/method_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/cli/__init__.py` & `quasarpy-0.2.0/quasarpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/handler/issue.py` & `quasarpy-0.2.0/quasarpy/handler/issue.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,10 +85,13 @@
 
         Raises:
             click.UsageError: If the token or repository is invalid.
 
         Returns:
             None
         """
-        repo = Github.get_repo(self.repo.name)
-        repo.create_issue(title=issue.title, body=issue.body, labels=issue.labels)
-        self.logger.info('Issue successfully created.')
+        try:
+            repo = Github.get_repo(self.repo.name)
+            repo.create_issue(title=issue.title, body=issue.body, labels=issue.labels)
+            self.logger.info('Issue successfully created.')
+        except GithubException as e:
+            self.logger.error(f'Error creating issue: {e}')
```

### Comparing `quasarpy-0.1.7/quasarpy/tests/test_handler.py` & `quasarpy-0.2.0/quasarpy/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/tests/test_utils.py` & `quasarpy-0.2.0/quasarpy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/utils/analyser.py` & `quasarpy-0.2.0/quasarpy/utils/analyser.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/utils/ascii.py` & `quasarpy-0.2.0/quasarpy/utils/ascii.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/utils/prompt_template.py` & `quasarpy-0.2.0/quasarpy/utils/prompt_template.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/utils/redis_server.py` & `quasarpy-0.2.0/quasarpy/utils/redis_server.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/quasarpy/utils/templates/report_template.html` & `quasarpy-0.2.0/quasarpy/utils/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `quasarpy-0.1.7/PKG-INFO` & `quasarpy-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasarpy
-Version: 0.1.7
+Version: 0.2.0
 Summary: Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc.
 License: GPL-3.0-or-later
 Author: Khushiyant
 Author-email: khushiyant2002@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

