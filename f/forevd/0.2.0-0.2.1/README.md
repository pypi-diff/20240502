# Comparing `tmp/forevd-0.2.0.tar.gz` & `tmp/forevd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forevd-0.2.0.tar", max compression
+gzip compressed data, was "forevd-0.2.1.tar", max compression
```

## Comparing `forevd-0.2.0.tar` & `forevd-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-15 11:21:15.919592 forevd-0.2.0/LICENSE
--rw-r--r--   0        0        0     5628 2023-06-15 11:21:15.919592 forevd-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/__init__.py
--rw-r--r--   0        0        0     6589 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/__main__.py
--rw-r--r--   0        0        0     1543 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/apache/__init__.py
--rw-r--r--   0        0        0     4840 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/apache/httpd.conf
--rw-r--r--   0        0        0      216 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/app.py
--rw-r--r--   0        0        0        0 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/resources/logging/__init__.py
--rw-r--r--   0        0        0      387 2023-06-15 11:21:15.919592 forevd-0.2.0/forevd/resources/logging/cli.conf
--rw-r--r--   0        0        0      884 2023-06-15 11:21:15.919592 forevd-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6333 1970-01-01 00:00:00.000000 forevd-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 01:22:51.177572 forevd-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5628 2024-05-02 01:22:51.177572 forevd-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/__init__.py
+-rw-r--r--   0        0        0     6590 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/__main__.py
+-rw-r--r--   0        0        0     1544 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/apache/__init__.py
+-rw-r--r--   0        0        0     4840 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/apache/httpd.conf
+-rw-r--r--   0        0        0      216 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/app.py
+-rw-r--r--   0        0        0        0 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/resources/logging/__init__.py
+-rw-r--r--   0        0        0      387 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/resources/logging/cli.conf
+-rw-r--r--   0        0        0      910 2024-05-02 01:22:51.177572 forevd-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6347 1970-01-01 00:00:00.000000 forevd-0.2.1/PKG-INFO
```

### Comparing `forevd-0.2.0/LICENSE` & `forevd-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `forevd-0.2.0/README.md` & `forevd-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `forevd-0.2.0/forevd/__main__.py` & `forevd-0.2.1/forevd/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The main entry point for forevd.
 """
+
 import importlib
 import logging
 import os
 import tempfile
 
 import click
```

### Comparing `forevd-0.2.0/forevd/apache/__init__.py` & `forevd-0.2.1/forevd/apache/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Resources module ot help load templates in
 """
+
 import io
 import logging
 import os
 import shlex
 import shutil
 
 import jinja2
```

### Comparing `forevd-0.2.0/forevd/apache/httpd.conf` & `forevd-0.2.1/forevd/apache/httpd.conf`

 * *Files identical despite different names*

### Comparing `forevd-0.2.0/pyproject.toml` & `forevd-0.2.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [tool.poetry]
 name = "forevd"
-version = "0.2.0"
+version = "0.2.1"
 description = "Forward and reverse proxy using apache or nginx"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
-Jinja2 = "^3.1.2"
-requests = "^2.28.1"
-firestone-lib = "^0.1.8"
-fastapi = "^0.95.2"
-uvicorn = "^0.22.0"
+python = ">=3.9,<4.0"
+Jinja2 = ">=3.1.2"
+requests = ">=2.28.1"
+firestone-lib = ">=0.1.8"
+fastapi = ">=0.95.2"
+uvicorn = ">=0.22.0"
 
 [tool.poetry.group.build.dependencies]
-black = "^22.10.0"
-pytest = "^7.2.0"
-pylint = "^2.15.5"
-pytest-mock = "^3.10.0"
-mock = "^4.0.3"
-pycodestyle = "^2.9.1"
-pytest-cov = "^4.0.0"
+black = ">=22.10.0"
+pytest = ">=7.2.0"
+pylint = ">=2.15.5"
+pytest-mock = ">=3.10.0"
+mock = ">=4.0.3"
+pycodestyle = ">=2.9.1"
+pytest-cov = ">=4.0.0"
 
 [tool.poetry.scripts]
 forevd = 'forevd.__main__:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
-target-version = ["py310"]
+target-version = ["py39", "py310"]
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 150
 good-names = [
     "fh"
 ]
 max-args = 8
```

### Comparing `forevd-0.2.0/PKG-INFO` & `forevd-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: forevd
-Version: 0.2.0
+Version: 0.2.1
 Summary: Forward and reverse proxy using apache or nginx
 License: LICENSE
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: fastapi (>=0.95.2,<0.96.0)
-Requires-Dist: firestone-lib (>=0.1.8,<0.2.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Jinja2 (>=3.1.2)
+Requires-Dist: fastapi (>=0.95.2)
+Requires-Dist: firestone-lib (>=0.1.8)
+Requires-Dist: requests (>=2.28.1)
+Requires-Dist: uvicorn (>=0.22.0)
 Description-Content-Type: text/markdown
 
 # Table of contents
 1. [Intro](#intro)
 1. [Dependencies](#dependencies)
 1. [Running `forevd`](#running-forevd)
 1. [Config Files](#config-files)
```

