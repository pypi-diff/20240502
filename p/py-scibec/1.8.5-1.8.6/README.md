# Comparing `tmp/py_scibec-1.8.5.tar.gz` & `tmp/py_scibec-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_scibec-1.8.5.tar", last modified: Tue Jan 16 13:19:48 2024, max compression
+gzip compressed data, was "py_scibec-1.8.6.tar", last modified: Tue Jan 16 13:23:15 2024, max compression
```

## Comparing `py_scibec-1.8.5.tar` & `py_scibec-1.8.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.166332 py_scibec-1.8.5/
--rw-r--r--   0 root         (0) root         (0)      471 2024-01-16 13:19:48.166332 py_scibec-1.8.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.165332 py_scibec-1.8.5/py_scibec/
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-12-01 16:51:18.000000 py_scibec-1.8.5/py_scibec/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-01-16 13:19:34.000000 py_scibec-1.8.5/py_scibec/bec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.165332 py_scibec-1.8.5/py_scibec.egg-info/
--rw-r--r--   0 root         (0) root         (0)      471 2024-01-16 13:19:48.000000 py_scibec-1.8.5/py_scibec.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      225 2024-01-16 13:19:48.000000 py_scibec-1.8.5/py_scibec.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-16 13:19:48.000000 py_scibec-1.8.5/py_scibec.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2024-01-16 13:19:48.000000 py_scibec-1.8.5/py_scibec.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-01-16 13:19:48.000000 py_scibec-1.8.5/py_scibec.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-01-16 13:19:48.166332 py_scibec-1.8.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1699 2024-01-16 13:19:35.000000 py_scibec-1.8.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.607773 py_scibec-1.8.6/
+-rw-r--r--   0 root         (0) root         (0)      471 2024-01-16 13:23:15.607773 py_scibec-1.8.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.606773 py_scibec-1.8.6/py_scibec/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-12-01 16:51:18.000000 py_scibec-1.8.6/py_scibec/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2024-01-16 13:23:02.000000 py_scibec-1.8.6/py_scibec/bec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.607773 py_scibec-1.8.6/py_scibec.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      471 2024-01-16 13:23:15.000000 py_scibec-1.8.6/py_scibec.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      225 2024-01-16 13:23:15.000000 py_scibec-1.8.6/py_scibec.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-16 13:23:15.000000 py_scibec-1.8.6/py_scibec.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2024-01-16 13:23:15.000000 py_scibec-1.8.6/py_scibec.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-01-16 13:23:15.000000 py_scibec-1.8.6/py_scibec.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-01-16 13:23:15.608773 py_scibec-1.8.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2024-01-16 13:23:03.000000 py_scibec-1.8.6/setup.py
```

### Comparing `py_scibec-1.8.5/py_scibec/bec.py` & `py_scibec-1.8.6/py_scibec/bec.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,31 +40,49 @@
     def wrapper(*args, **kwargs):
         if not args[0].client:
             raise SciBecError("Not logged in.")
         return func(*args, **kwargs)
 
     return wrapper
 
+class SciBecModelsMixin:
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.AccessAccount = AccessAccount
+        self.AccessConfig = AccessConfig
+        self.Beamline = Beamline
+        self.Dataset = Dataset
+        self.Device = Device
+        self.Event = Event
+        self.Experiment = Experiment
+        self.ExperimentAccount = ExperimentAccount
+        self.FunctionalAccount = FunctionalAccount
+        self.Scan = Scan
+        self.Session = Session
+        self.User = User
 
-class SciBecCore:
+
+class SciBecCore():
     def __init__(self, host: str = "https://bec.development.psi.ch/api/v1") -> None:
         self.client = None
         self.configuration = py_scibec_openapi_client.Configuration(host=host)
+        self.models = SciBecModelsMixin()
         self._access_account = None
         self._access_config = None
         self._beamline = None
         self._dataset = None
         self._device = None
         self._event = None
         self._experiment = None
         self._experiment_account = None
         self._functional_account = None
         self._scan = None
         self._session = None
         self._user = None
+        
 
     @property
     @login_required
     def access_account(self):
         return self._access_account
 
     @property
```

### Comparing `py_scibec-1.8.5/setup.cfg` & `py_scibec-1.8.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `py_scibec-1.8.5/setup.py` & `py_scibec-1.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 openapi_client = f"{current_path}/../py_scibec_openapi_client/"
 
-__version__ = "1.8.5"
+__version__ = "1.8.6"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

