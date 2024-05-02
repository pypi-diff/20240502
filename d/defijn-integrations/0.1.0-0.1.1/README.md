# Comparing `tmp/defijn_integrations-0.1.0.tar.gz` & `tmp/defijn_integrations-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defijn_integrations-0.1.0.tar", max compression
+gzip compressed data, was "defijn_integrations-0.1.1.tar", max compression
```

## Comparing `defijn_integrations-0.1.0.tar` & `defijn_integrations-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1690 2024-05-02 08:59:38.233300 defijn_integrations-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-30 11:08:47.502417 defijn_integrations-0.1.0/defijn_integrations/__init__.py
--rw-r--r--   0        0        0       28 2024-04-30 10:07:20.166946 defijn_integrations-0.1.0/defijn_integrations/clickupint.py
--rw-r--r--   0        0        0     4480 2024-04-25 11:18:06.965981 defijn_integrations-0.1.0/defijn_integrations/everhourint.py
--rw-r--r--   0        0        0     6450 2024-04-26 10:21:17.823550 defijn_integrations-0.1.0/defijn_integrations/gitlabint.py
--rw-r--r--   0        0        0      740 2024-04-30 10:08:33.800355 defijn_integrations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 defijn_integrations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1966 2024-05-02 13:52:23.222060 defijn_integrations-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 11:08:47.502417 defijn_integrations-0.1.1/defijn_integrations/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-30 10:07:20.166946 defijn_integrations-0.1.1/defijn_integrations/clickupint.py
+-rw-r--r--   0        0        0     4480 2024-04-25 11:18:06.965981 defijn_integrations-0.1.1/defijn_integrations/everhourint.py
+-rw-r--r--   0        0        0     6450 2024-04-26 10:21:17.823550 defijn_integrations-0.1.1/defijn_integrations/gitlabint.py
+-rw-r--r--   0        0        0      757 2024-05-02 13:54:19.519977 defijn_integrations-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2783 1970-01-01 00:00:00.000000 defijn_integrations-0.1.1/PKG-INFO
```

### Comparing `defijn_integrations-0.1.0/README.md` & `defijn_integrations-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -43,16 +43,31 @@
     poetry build
     ```
 
     This command will generate the distribution package in the `dist` directory.
 
 ### Publishing the Package
 
-Before publishing, ensure you have an account on [PyPI](https://pypi.org/) and have set up the necessary authentication (API token recommended).
+1. Setting up Authentication for PyPI
 
-1. Run the following command to publish your package to PyPI:
+   Before you can publish packages to PyPI, you need to authenticate your package upload requests. You can do this by creating a .pypirc file in your home directory with the following content:
+    
+   ```ini
+   [distutils]
+   index-servers =
+     pypi
+   
+   [pypi]
+   repository = https://upload.pypi.org/legacy/
+   username = __token__
+   password = <your-token>
+   ```
+    
+   Replace `<your-token>` with your PyPI token.
+
+2. Run the following command to publish your package:
+
+   ```bash
+    twine upload dist/*
+   ```
 
-    ```bash
-    poetry publish
-    ```
-
-    You will be prompted to enter your PyPI username and password (or use an API token).
+    This command will publish your package to PyPI.
```

### Comparing `defijn_integrations-0.1.0/defijn_integrations/everhourint.py` & `defijn_integrations-0.1.1/defijn_integrations/everhourint.py`

 * *Files identical despite different names*

### Comparing `defijn_integrations-0.1.0/defijn_integrations/gitlabint.py` & `defijn_integrations-0.1.1/defijn_integrations/gitlabint.py`

 * *Files identical despite different names*

### Comparing `defijn_integrations-0.1.0/pyproject.toml` & `defijn_integrations-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "defijn-integrations"
-version = "0.1.0"
+version = "0.1.1"
 description = "Defijn's package providing integrations for various third-party APIs such as Everhour, GitLab and Clickup."
 authors = ["Jonathan <jonathan@defijn.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/defijn-io/defijn-integrations"
 homepage = "https://defijn.io"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
 rich = "^13.7.0"
 python-gitlab = "^4.4.0"
 questionary = "^2.0.1"
 textual = "^0.58.0"
+twine = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 # If your package includes a CLI, specify the entry point here
```

### Comparing `defijn_integrations-0.1.0/PKG-INFO` & `defijn_integrations-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: defijn-integrations
-Version: 0.1.0
+Version: 0.1.1
 Summary: Defijn's package providing integrations for various third-party APIs such as Everhour, GitLab and Clickup.
 Home-page: https://defijn.io
 License: MIT
 Author: Jonathan
 Author-email: jonathan@defijn.io
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: python-gitlab (>=4.4.0,<5.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: textual (>=0.58.0,<0.59.0)
+Requires-Dist: twine (>=5.0.0,<6.0.0)
 Project-URL: Repository, https://github.com/defijn-io/defijn-integrations
 Description-Content-Type: text/markdown
 
 # defijn-integrations
 
 `defijn-integrations` is a Python package providing convenient integrations with several third-party services including GitLab, Everhour, and ClickUp. This package simplifies the process of interacting with these services by wrapping their APIs into easy-to-use Python functions.
 
@@ -63,17 +64,31 @@
     poetry build
     ```
 
     This command will generate the distribution package in the `dist` directory.
 
 ### Publishing the Package
 
-Before publishing, ensure you have an account on [PyPI](https://pypi.org/) and have set up the necessary authentication (API token recommended).
+1. Setting up Authentication for PyPI
 
-1. Run the following command to publish your package to PyPI:
+   Before you can publish packages to PyPI, you need to authenticate your package upload requests. You can do this by creating a .pypirc file in your home directory with the following content:
+    
+   ```ini
+   [distutils]
+   index-servers =
+     pypi
+   
+   [pypi]
+   repository = https://upload.pypi.org/legacy/
+   username = __token__
+   password = <your-token>
+   ```
+    
+   Replace `<your-token>` with your PyPI token.
 
-    ```bash
-    poetry publish
-    ```
+2. Run the following command to publish your package:
 
-    You will be prompted to enter your PyPI username and password (or use an API token).
+   ```bash
+    twine upload dist/*
+   ```
 
+    This command will publish your package to PyPI.
```

