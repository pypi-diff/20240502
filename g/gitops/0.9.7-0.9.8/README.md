# Comparing `tmp/gitops-0.9.7.tar.gz` & `tmp/gitops-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitops-0.9.7.tar", max compression
+gzip compressed data, was "gitops-0.9.8.tar", max compression
```

## Comparing `gitops-0.9.7.tar` & `gitops-0.9.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1315 2022-11-24 00:59:09.568700 gitops-0.9.7/LICENSE
--rw-r--r--   0        0        0      961 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/__init__.py
--rw-r--r--   0        0        0        0 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/common/__init__.py
--rw-r--r--   0        0        0     5300 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/common/app.py
--rw-r--r--   0        0        0     1058 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/common/utils.py
--rw-r--r--   0        0        0    12506 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/core.py
--rw-r--r--   0        0        0     8052 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/db.py
--rw-r--r--   0        0        0      520 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/main.py
--rw-r--r--   0        0        0     1855 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/shorthands.py
--rw-r--r--   0        0        0     1223 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/utils/__init__.py
--rw-r--r--   0        0        0     5038 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/utils/apps.py
--rw-r--r--   0        0        0     2639 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/utils/async_runner.py
--rw-r--r--   0        0        0     1209 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/utils/cli.py
--rw-r--r--   0        0        0      507 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/utils/exceptions.py
--rw-r--r--   0        0        0     1663 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/utils/images.py
--rw-r--r--   0        0        0    11011 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/utils/kube.py
--rw-r--r--   0        0        0     1360 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/utils/tags.py
--rw-r--r--   0        0        0     1467 2022-11-24 00:59:09.572700 gitops-0.9.7/gitops/utils/yaml.py
--rw-r--r--   0        0        0     1519 2022-11-24 00:59:09.576701 gitops-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 gitops-0.9.7/setup.py
--rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 gitops-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1315 2022-12-06 00:08:25.943154 gitops-0.9.8/LICENSE
+-rw-r--r--   0        0        0      961 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/common/__init__.py
+-rw-r--r--   0        0        0     5300 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/common/app.py
+-rw-r--r--   0        0        0     1058 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/common/utils.py
+-rw-r--r--   0        0        0    12506 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/core.py
+-rw-r--r--   0        0        0     8052 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/db.py
+-rw-r--r--   0        0        0      520 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/main.py
+-rw-r--r--   0        0        0     1855 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/shorthands.py
+-rw-r--r--   0        0        0     1223 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/utils/__init__.py
+-rw-r--r--   0        0        0     5038 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/utils/apps.py
+-rw-r--r--   0        0        0     2639 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/utils/async_runner.py
+-rw-r--r--   0        0        0     1209 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/utils/cli.py
+-rw-r--r--   0        0        0      507 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/utils/exceptions.py
+-rw-r--r--   0        0        0     1663 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/utils/images.py
+-rw-r--r--   0        0        0    11011 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/utils/kube.py
+-rw-r--r--   0        0        0     1360 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/utils/tags.py
+-rw-r--r--   0        0        0     1467 2022-12-06 00:08:25.947155 gitops-0.9.8/gitops/utils/yaml.py
+-rw-r--r--   0        0        0     1519 2022-12-06 00:08:25.947155 gitops-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 gitops-0.9.8/setup.py
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 gitops-0.9.8/PKG-INFO
```

### Comparing `gitops-0.9.7/LICENSE` & `gitops-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/__init__.py` & `gitops-0.9.8/gitops/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 from pathlib import Path
 
 from .utils.cli import success, warning
 
-__version__ = "0.9.6"
+__version__ = "0.9.8"
 
 
 # Checking gitops version matches cluster repo version.
 versions_path = (
     Path(os.environ.get("GITOPS_APPS_DIRECTORY", "apps")).parent.absolute() / "setup.cfg"
 )
 if versions_path.exists():
```

### Comparing `gitops-0.9.7/gitops/common/app.py` & `gitops-0.9.8/gitops/common/app.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/common/utils.py` & `gitops-0.9.8/gitops/common/utils.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/core.py` & `gitops-0.9.8/gitops/core.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/db.py` & `gitops-0.9.8/gitops/db.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/main.py` & `gitops-0.9.8/gitops/main.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/shorthands.py` & `gitops-0.9.8/gitops/shorthands.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/utils/__init__.py` & `gitops-0.9.8/gitops/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/utils/apps.py` & `gitops-0.9.8/gitops/utils/apps.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/utils/async_runner.py` & `gitops-0.9.8/gitops/utils/async_runner.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/utils/cli.py` & `gitops-0.9.8/gitops/utils/cli.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/utils/images.py` & `gitops-0.9.8/gitops/utils/images.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/utils/kube.py` & `gitops-0.9.8/gitops/utils/kube.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/utils/tags.py` & `gitops-0.9.8/gitops/utils/tags.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/gitops/utils/yaml.py` & `gitops-0.9.8/gitops/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `gitops-0.9.7/pyproject.toml` & `gitops-0.9.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitops"
-version = "0.9.7"
+version = "0.9.8"
 description = "Manage multiple apps across one or more k8s clusters."
 authors = ["Jarek Głowacki <jarekwg@gmail.com>"]
 license = "BSD"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 # CLI requirements
```

### Comparing `gitops-0.9.7/setup.py` & `gitops-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             'kubernetes_asyncio>=12.1.2,<13.0.0']}
 
 entry_points = \
 {'console_scripts': ['gitops = gitops.main:program.run']}
 
 setup_kwargs = {
     'name': 'gitops',
-    'version': '0.9.7',
+    'version': '0.9.8',
     'description': 'Manage multiple apps across one or more k8s clusters.',
     'long_description': 'None',
     'author': 'Jarek Głowacki',
     'author_email': 'jarekwg@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `gitops-0.9.7/PKG-INFO` & `gitops-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitops
-Version: 0.9.7
+Version: 0.9.8
 Summary: Manage multiple apps across one or more k8s clusters.
 License: BSD
 Author: Jarek Głowacki
 Author-email: jarekwg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

