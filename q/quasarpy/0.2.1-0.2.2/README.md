# Comparing `tmp/quasarpy-0.2.1.tar.gz` & `tmp/quasarpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasarpy-0.2.1.tar", max compression
+gzip compressed data, was "quasarpy-0.2.2.tar", max compression
```

## Comparing `quasarpy-0.2.1.tar` & `quasarpy-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    31941 2024-05-02 04:34:16.754901 quasarpy-0.2.1/LICENSE
--rw-r--r--   0        0        0     1843 2024-05-02 04:34:16.754901 quasarpy-0.2.1/README.md
--rw-r--r--   0        0        0  1387623 2024-05-02 04:34:16.754901 quasarpy-0.2.1/assets/logo_complete.png
--rw-r--r--   0        0        0   127970 2024-05-02 04:34:16.758901 quasarpy-0.2.1/assets/logo_complete_svg.svg
--rw-r--r--   0        0        0   182267 2024-05-02 04:34:16.758901 quasarpy-0.2.1/assets/logo_complete_tbg.png
--rw-r--r--   0        0        0   418415 2024-05-02 04:34:16.758901 quasarpy-0.2.1/assets/logo_icon.png
--rw-r--r--   0        0        0   166944 2024-05-02 04:34:16.758901 quasarpy-0.2.1/assets/logo_text.png
--rw-r--r--   0        0        0     1170 2024-05-02 04:34:16.762901 quasarpy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      670 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/__init__.py
--rw-r--r--   0        0        0       86 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/__main__.py
--rw-r--r--   0        0        0       17 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/_version.py
--rw-r--r--   0        0        0      177 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/algorithm/__init__.py
--rw-r--r--   0        0        0     5249 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/algorithm/detector.py
--rw-r--r--   0        0        0     2857 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/algorithm/llm.py
--rw-r--r--   0        0        0     7703 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/algorithm/model/class_model.json
--rw-r--r--   0        0        0     7703 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/algorithm/model/method_model.json
--rw-r--r--   0        0        0     4170 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/cli/__init__.py
--rw-r--r--   0        0        0       79 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/handler/__init__.py
--rw-r--r--   0        0        0     2708 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/handler/issue.py
--rw-r--r--   0        0        0        0 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/tests/__init__.py
--rw-r--r--   0        0        0      389 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/tests/conftest.py
--rw-r--r--   0        0        0        1 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/tests/test_algorithm.py
--rw-r--r--   0        0        0        0 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/tests/test_cli.py
--rw-r--r--   0        0        0      545 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/tests/test_handler.py
--rw-r--r--   0        0        0      645 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/tests/test_utils.py
--rw-r--r--   0        0        0      508 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/utils/__init__.py
--rw-r--r--   0        0        0     1864 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/utils/analyser.py
--rw-r--r--   0        0        0     1322 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/utils/ascii.py
--rw-r--r--   0        0        0      195 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/utils/errors.py
--rw-r--r--   0        0        0      187 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/utils/logger.py
--rw-r--r--   0        0        0     1030 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/utils/prompt_template.py
--rw-r--r--   0        0        0     4524 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/utils/redis_server.py
--rw-r--r--   0        0        0     2978 2024-05-02 04:34:16.762901 quasarpy-0.2.1/quasarpy/utils/templates/report_template.html
--rw-r--r--   0        0        0     3304 1970-01-01 00:00:00.000000 quasarpy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    31941 2024-05-02 16:51:21.018555 quasarpy-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1843 2024-05-02 16:51:21.018555 quasarpy-0.2.2/README.md
+-rw-r--r--   0        0        0  1387623 2024-05-02 16:51:21.018555 quasarpy-0.2.2/assets/logo_complete.png
+-rw-r--r--   0        0        0   127970 2024-05-02 16:51:21.022555 quasarpy-0.2.2/assets/logo_complete_svg.svg
+-rw-r--r--   0        0        0   182267 2024-05-02 16:51:21.022555 quasarpy-0.2.2/assets/logo_complete_tbg.png
+-rw-r--r--   0        0        0   418415 2024-05-02 16:51:21.022555 quasarpy-0.2.2/assets/logo_icon.png
+-rw-r--r--   0        0        0   166944 2024-05-02 16:51:21.022555 quasarpy-0.2.2/assets/logo_text.png
+-rw-r--r--   0        0        0     1153 2024-05-02 16:51:34.870668 quasarpy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      670 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/__main__.py
+-rw-r--r--   0        0        0       17 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/_version.py
+-rw-r--r--   0        0        0      177 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/algorithm/__init__.py
+-rw-r--r--   0        0        0     5249 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/algorithm/detector.py
+-rw-r--r--   0        0        0     2857 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/algorithm/llm.py
+-rw-r--r--   0        0        0     7703 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/algorithm/model/class_model.json
+-rw-r--r--   0        0        0     7703 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/algorithm/model/method_model.json
+-rw-r--r--   0        0        0     4170 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/cli/__init__.py
+-rw-r--r--   0        0        0       79 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/handler/__init__.py
+-rw-r--r--   0        0        0     2708 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/handler/issue.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/tests/__init__.py
+-rw-r--r--   0        0        0      389 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/tests/conftest.py
+-rw-r--r--   0        0        0        1 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/tests/test_algorithm.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/tests/test_cli.py
+-rw-r--r--   0        0        0      545 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/tests/test_handler.py
+-rw-r--r--   0        0        0      645 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/tests/test_utils.py
+-rw-r--r--   0        0        0      508 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/utils/__init__.py
+-rw-r--r--   0        0        0     1864 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/utils/analyser.py
+-rw-r--r--   0        0        0     1322 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/utils/ascii.py
+-rw-r--r--   0        0        0      195 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/utils/errors.py
+-rw-r--r--   0        0        0      187 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/utils/logger.py
+-rw-r--r--   0        0        0     1030 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/utils/prompt_template.py
+-rw-r--r--   0        0        0     4524 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/utils/redis_server.py
+-rw-r--r--   0        0        0     2978 2024-05-02 16:51:21.026555 quasarpy-0.2.2/quasarpy/utils/templates/report_template.html
+-rw-r--r--   0        0        0     3189 1970-01-01 00:00:00.000000 quasarpy-0.2.2/PKG-INFO
```

### Comparing `quasarpy-0.2.1/LICENSE` & `quasarpy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/README.md` & `quasarpy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/assets/logo_complete.png` & `quasarpy-0.2.2/assets/logo_complete.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/assets/logo_complete_svg.svg` & `quasarpy-0.2.2/assets/logo_complete_svg.svg`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/assets/logo_complete_tbg.png` & `quasarpy-0.2.2/assets/logo_complete_tbg.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/assets/logo_icon.png` & `quasarpy-0.2.2/assets/logo_icon.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/assets/logo_text.png` & `quasarpy-0.2.2/assets/logo_text.png`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/pyproject.toml` & `quasarpy-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 [tool.poetry]
 name = "quasarpy"
-version = "0.2.1"
+version = "0.2.2"
 description = "Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc."
 authors = ["Khushiyant <khushiyant2002@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 include = ["assets", 'LICENSE']
 
 [tool.poetry.scripts]
 quasar = "quasarpy:main"
 
-[tool.poetry-dynamic-versioning]
-enable = true
-
 [tool.poetry.dependencies]
 python = "^3.10"
-sphinx = "^7.2.6"
 click = "^8.1.7"
-pytest = "^8.0.0"
 python-dotenv = "^1.0.1"
 radon = "^6.0.1"
 redis = "^5.0.1"
 requests = "^2.31.0"
 pygithub = "^2.2.0"
-ruff = "^0.2.1"
 termcolor = "^2.4.0"
 pandas = "^2.2.0"
 transformers = "^4.38.1"
 torch = "^2.2.1"
 pydantic = "^2.6.3"
 xgboost = "^2.0.3"
 scikit-learn = "^1.4.1.post1"
 jinja2 = "^3.1.3"
 xhtml2pdf = "^0.2.15"
 huggingface-hub = "^0.22.2"
 twine = "^5.0.0"
 
+[tool.poetry.dev-dependencies]
+pytest = "^8.0.0"
+ruff = "^0.2.1"
+sphinx = "^7.2.6"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `quasarpy-0.2.1/quasarpy/__init__.py` & `quasarpy-0.2.2/quasarpy/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/algorithm/detector.py` & `quasarpy-0.2.2/quasarpy/algorithm/detector.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/algorithm/llm.py` & `quasarpy-0.2.2/quasarpy/algorithm/llm.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/algorithm/model/class_model.json` & `quasarpy-0.2.2/quasarpy/algorithm/model/class_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/algorithm/model/method_model.json` & `quasarpy-0.2.2/quasarpy/algorithm/model/method_model.json`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/cli/__init__.py` & `quasarpy-0.2.2/quasarpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/handler/issue.py` & `quasarpy-0.2.2/quasarpy/handler/issue.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/tests/test_handler.py` & `quasarpy-0.2.2/quasarpy/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/tests/test_utils.py` & `quasarpy-0.2.2/quasarpy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/utils/analyser.py` & `quasarpy-0.2.2/quasarpy/utils/analyser.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/utils/ascii.py` & `quasarpy-0.2.2/quasarpy/utils/ascii.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/utils/prompt_template.py` & `quasarpy-0.2.2/quasarpy/utils/prompt_template.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/utils/redis_server.py` & `quasarpy-0.2.2/quasarpy/utils/redis_server.py`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/quasarpy/utils/templates/report_template.html` & `quasarpy-0.2.2/quasarpy/utils/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `quasarpy-0.2.1/PKG-INFO` & `quasarpy-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasarpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quasar is python package that can be used for smell detection along with detailed report in various formats such as html, pdf, etc.
 License: GPL-3.0-or-later
 Author: Khushiyant
 Author-email: khushiyant2002@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -13,22 +13,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: huggingface-hub (>=0.22.2,<0.23.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pygithub (>=2.2.0,<3.0.0)
-Requires-Dist: pytest (>=8.0.0,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: radon (>=6.0.1,<7.0.0)
 Requires-Dist: redis (>=5.0.1,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: ruff (>=0.2.1,<0.3.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
-Requires-Dist: sphinx (>=7.2.6,<8.0.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Requires-Dist: torch (>=2.2.1,<3.0.0)
 Requires-Dist: transformers (>=4.38.1,<5.0.0)
 Requires-Dist: twine (>=5.0.0,<6.0.0)
 Requires-Dist: xgboost (>=2.0.3,<3.0.0)
 Requires-Dist: xhtml2pdf (>=0.2.15,<0.3.0)
 Description-Content-Type: text/markdown
```

