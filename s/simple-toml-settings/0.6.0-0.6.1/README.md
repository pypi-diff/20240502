# Comparing `tmp/simple_toml_settings-0.6.0.tar.gz` & `tmp/simple_toml_settings-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_toml_settings-0.6.0.tar", max compression
+gzip compressed data, was "simple_toml_settings-0.6.1.tar", max compression
```

## Comparing `simple_toml_settings-0.6.0.tar` & `simple_toml_settings-0.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2024-02-14 10:03:09.008101 simple_toml_settings-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     4037 2024-03-11 15:27:17.695115 simple_toml_settings-0.6.0/README.md
--rw-r--r--   0        0        0     5105 2024-03-11 16:57:07.323802 simple_toml_settings-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      110 2024-03-07 09:16:51.689416 simple_toml_settings-0.6.0/simple_toml_settings/__init__.py
--rw-r--r--   0        0        0      858 2024-02-14 09:47:27.566464 simple_toml_settings-0.6.0/simple_toml_settings/exceptions.py
--rw-r--r--   0        0        0        0 2023-10-12 12:17:59.335044 simple_toml_settings-0.6.0/simple_toml_settings/py.typed
--rw-r--r--   0        0        0     5625 2024-03-11 14:59:54.144875 simple_toml_settings-0.6.0/simple_toml_settings/settings.py
--rw-r--r--   0        0        0     5356 1970-01-01 00:00:00.000000 simple_toml_settings-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-02-14 10:03:09.008101 simple_toml_settings-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     4037 2024-03-11 15:27:17.695115 simple_toml_settings-0.6.1/README.md
+-rw-r--r--   0        0        0     5115 2024-05-02 10:36:59.762896 simple_toml_settings-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-03-07 09:16:51.689416 simple_toml_settings-0.6.1/simple_toml_settings/__init__.py
+-rw-r--r--   0        0        0      858 2024-02-14 09:47:27.566464 simple_toml_settings-0.6.1/simple_toml_settings/exceptions.py
+-rw-r--r--   0        0        0        0 2023-10-12 12:17:59.335044 simple_toml_settings-0.6.1/simple_toml_settings/py.typed
+-rw-r--r--   0        0        0     5625 2024-03-11 14:59:54.144875 simple_toml_settings-0.6.1/simple_toml_settings/settings.py
+-rw-r--r--   0        0        0     5355 1970-01-01 00:00:00.000000 simple_toml_settings-0.6.1/PKG-INFO
```

### Comparing `simple_toml_settings-0.6.0/LICENSE.txt` & `simple_toml_settings-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_toml_settings-0.6.0/README.md` & `simple_toml_settings-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `simple_toml_settings-0.6.0/pyproject.toml` & `simple_toml_settings-0.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple-toml-settings"
-version = "0.6.0"
+version = "0.6.1"
 description = "A Python library to save your settings in a TOML file."
 authors = ["Grant Ramsay <seapagan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 packages = [{ include = "simple_toml_settings" }]
 
@@ -29,35 +29,35 @@
 # shown on [Pypi.org](https://pypi.org/) if you are creating a public package.
 "Pull Requests" = "https://github.com/seapagan/simple-toml-settings/pulls"
 "Bug Tracker" = "https://github.com/seapagan/simple-toml-settings/issues"
 "Changelog" = "https://github.com/seapagan/simple-toml-settings/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-rtoml = "^0.9.0"
-github-changelog-md = "0.9.2"
+rtoml = ">=0.9.0,<1.0.0"
+github-changelog-md = ">=0.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Configure dev dependencies you can add or remove as needed
 [tool.poetry.group.dev.dependencies]
 # linting, type-checking and security checks
 mypy = "^1.4.1"
 pre-commit = "^3.3.3"
 pymarkdownlnt = "^0.9.12"
-ruff = ">=0.1.3,<0.4.0"
+ruff = ">=0.1.3,<0.5.0"
 
 # task runner
-poethepoet = ">=0.24.1,<0.26.0"
+poethepoet = ">=0.24.1,<0.27.0"
 
 # testing
 pytest = ">=7.4,<9.0"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 pytest-xdist = "^3.2.1"
 pytest-sugar = ">=0.9.7,<1.1.0"
 pytest-randomly = "^3.13.0"
 pytest-reverse = "^1.7.0"
 pytest-mock = "^3.11.1"
 mock = "^5.1.0"
 faker = ">=19.2,<25.0"
```

### Comparing `simple_toml_settings-0.6.0/simple_toml_settings/exceptions.py` & `simple_toml_settings-0.6.1/simple_toml_settings/exceptions.py`

 * *Files identical despite different names*

### Comparing `simple_toml_settings-0.6.0/simple_toml_settings/settings.py` & `simple_toml_settings-0.6.1/simple_toml_settings/settings.py`

 * *Files identical despite different names*

### Comparing `simple_toml_settings-0.6.0/PKG-INFO` & `simple_toml_settings-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-toml-settings
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python library to save your settings in a TOML file.
 Home-page: https://github.com/seapagan/simple-toml-settings
 License: MIT
 Author: Grant Ramsay
 Author-email: seapagan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,16 +13,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: github-changelog-md (==0.9.2)
-Requires-Dist: rtoml (>=0.9.0,<0.10.0)
+Requires-Dist: github-changelog-md (>=0.9.0)
+Requires-Dist: rtoml (>=0.9.0,<1.0.0)
 Project-URL: Bug Tracker, https://github.com/seapagan/simple-toml-settings/issues
 Project-URL: Changelog, https://github.com/seapagan/simple-toml-settings/blob/main/CHANGELOG.md
 Project-URL: Documentation, http://toml-settings.grantramsay.dev/
 Project-URL: Pull Requests, https://github.com/seapagan/simple-toml-settings/pulls
 Project-URL: Repository, https://github.com/seapagan/simple-toml-settings
 Description-Content-Type: text/markdown
```

