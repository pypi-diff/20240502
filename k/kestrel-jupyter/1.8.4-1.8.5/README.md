# Comparing `tmp/kestrel_jupyter-1.8.4.tar.gz` & `tmp/kestrel_jupyter-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel_jupyter-1.8.4.tar", last modified: Tue Apr 23 15:57:00 2024, max compression
+gzip compressed data, was "kestrel_jupyter-1.8.5.tar", last modified: Wed May  1 23:18:21 2024, max compression
```

## Comparing `kestrel_jupyter-1.8.4.tar` & `kestrel_jupyter-1.8.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:57:00.205812 kestrel_jupyter-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-04-23 15:57:00.205812 kestrel_jupyter-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:57:00.205812 kestrel_jupyter-1.8.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:57:00.201812 kestrel_jupyter-1.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:57:00.201812 kestrel_jupyter-1.8.4/src/kestrel_ipython/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_ipython/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:57:00.205812 kestrel_jupyter-1.8.4/src/kestrel_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-04-23 15:57:00.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-23 15:57:00.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:57:00.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 15:57:00.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-23 15:57:00.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 15:57:00.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:57:00.205812 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:57:00.205812 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/codemirror/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/codemirror/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/codemirror/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:57:00.205812 kestrel_jupyter-1.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/tests/test_kernel_install.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-23 15:56:47.000000 kestrel_jupyter-1.8.4/tests/test_notebook_syntax_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:21.623758 kestrel_jupyter-1.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-01 23:18:21.623758 kestrel_jupyter-1.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 23:18:21.623758 kestrel_jupyter-1.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:21.619758 kestrel_jupyter-1.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:21.619758 kestrel_jupyter-1.8.5/src/kestrel_ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_ipython/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:21.623758 kestrel_jupyter-1.8.5/src/kestrel_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-01 23:18:21.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-01 23:18:21.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:18:21.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 23:18:21.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-01 23:18:21.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 23:18:21.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:21.623758 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:21.623758 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/codemirror/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/codemirror/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/codemirror/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:21.623758 kestrel_jupyter-1.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/tests/test_kernel_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-01 23:18:05.000000 kestrel_jupyter-1.8.5/tests/test_notebook_syntax_gen.py
```

### Comparing `kestrel_jupyter-1.8.4/PKG-INFO` & `kestrel_jupyter-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel_jupyter
-Version: 1.8.4
+Version: 1.8.5
 Summary: Kestrel Jupyter Kernel
 Maintainer-email: Xiaokui Shu <xiaokui.shu@ibm.com>, Paul Coccoli <pcoccoli@us.ibm.com>
 License: Apache 2.0 License
 Project-URL: Homepage, https://github.com/opencybersecurityalliance/kestrel-lang
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Project-URL: Repository, https://github.com/opencybersecurityalliance/kestrel-lang.git
 Keywords: kestrel,Jupyter,kernel
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: kestrel_core==1.8.2
 Requires-Dist: kestrel_datasource_stixbundle==1.8.0
-Requires-Dist: kestrel_datasource_stixshifter==1.8.2
+Requires-Dist: kestrel_datasource_stixshifter==1.8.3
 Requires-Dist: kestrel_analytics_python==1.8.0
 Requires-Dist: kestrel_analytics_docker==1.8.1
 Requires-Dist: jupyterlab-server
 Requires-Dist: jupyterlab
 Requires-Dist: jupyter_client
 Requires-Dist: nbclassic
 Provides-Extra: test
```

### Comparing `kestrel_jupyter-1.8.4/README.rst` & `kestrel_jupyter-1.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.4/pyproject.toml` & `kestrel_jupyter-1.8.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.2.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kestrel_jupyter"
-version = "1.8.4"
+version = "1.8.5"
 description = "Kestrel Jupyter Kernel"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "Apache 2.0 License"}
 maintainers = [
     {name = "Xiaokui Shu", email = "xiaokui.shu@ibm.com"},
     {name = "Paul Coccoli", email = "pcoccoli@us.ibm.com"},
@@ -24,15 +24,15 @@
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
 ]
 
 dependencies = [
     "kestrel_core==1.8.2",
     "kestrel_datasource_stixbundle==1.8.0",
-    "kestrel_datasource_stixshifter==1.8.2",
+    "kestrel_datasource_stixshifter==1.8.3",
     "kestrel_analytics_python==1.8.0",
     "kestrel_analytics_docker==1.8.1",
     "jupyterlab-server",
     "jupyterlab",
     "jupyter_client",
     "nbclassic",
 ]
```

### Comparing `kestrel_jupyter-1.8.4/src/kestrel_ipython/magic.py` & `kestrel_jupyter-1.8.5/src/kestrel_ipython/magic.py`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.4/src/kestrel_jupyter.egg-info/PKG-INFO` & `kestrel_jupyter-1.8.5/src/kestrel_jupyter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel_jupyter
-Version: 1.8.4
+Version: 1.8.5
 Summary: Kestrel Jupyter Kernel
 Maintainer-email: Xiaokui Shu <xiaokui.shu@ibm.com>, Paul Coccoli <pcoccoli@us.ibm.com>
 License: Apache 2.0 License
 Project-URL: Homepage, https://github.com/opencybersecurityalliance/kestrel-lang
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Project-URL: Repository, https://github.com/opencybersecurityalliance/kestrel-lang.git
 Keywords: kestrel,Jupyter,kernel
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: kestrel_core==1.8.2
 Requires-Dist: kestrel_datasource_stixbundle==1.8.0
-Requires-Dist: kestrel_datasource_stixshifter==1.8.2
+Requires-Dist: kestrel_datasource_stixshifter==1.8.3
 Requires-Dist: kestrel_analytics_python==1.8.0
 Requires-Dist: kestrel_analytics_docker==1.8.1
 Requires-Dist: jupyterlab-server
 Requires-Dist: jupyterlab
 Requires-Dist: jupyter_client
 Requires-Dist: nbclassic
 Provides-Extra: test
```

### Comparing `kestrel_jupyter-1.8.4/src/kestrel_jupyter.egg-info/SOURCES.txt` & `kestrel_jupyter-1.8.5/src/kestrel_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js` & `kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/codemirror/setup.py` & `kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/codemirror/setup.py`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/kernel.py` & `kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/logo-64x64.png` & `kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `kestrel_jupyter-1.8.4/src/kestrel_jupyter_kernel/setup.py` & `kestrel_jupyter-1.8.5/src/kestrel_jupyter_kernel/setup.py`

 * *Files identical despite different names*

