# Comparing `tmp/pynpdc-0.13.1.tar.gz` & `tmp/pynpdc-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynpdc-0.13.1.tar", last modified: Tue Apr 30 10:57:59 2024, max compression
+gzip compressed data, was "pynpdc-0.13.2.tar", last modified: Thu May  2 12:05:05 2024, max compression
```

## Comparing `pynpdc-0.13.1.tar` & `pynpdc-0.13.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-30 10:57:59.805313 pynpdc-0.13.1/
--rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-04-30 10:57:59.805313 pynpdc-0.13.1/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     6577 2024-04-11 12:20:53.000000 pynpdc-0.13.1/README.md
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-30 10:57:59.805313 pynpdc-0.13.1/pynpdc/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      911 2024-04-26 08:39:05.000000 pynpdc-0.13.1/pynpdc/__init__.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    10243 2024-04-30 10:50:07.000000 pynpdc-0.13.1/pynpdc/auth.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    39423 2024-04-26 08:29:11.000000 pynpdc-0.13.1/pynpdc/dataset.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      443 2024-04-11 09:18:52.000000 pynpdc-0.13.1/pynpdc/exception.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        0 2024-04-26 08:07:44.000000 pynpdc-0.13.1/pynpdc/py.typed
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1504 2024-04-11 09:18:52.000000 pynpdc-0.13.1/pynpdc/types.py
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-30 10:57:59.805313 pynpdc-0.13.1/pynpdc.egg-info/
--rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-04-30 10:57:59.000000 pynpdc-0.13.1/pynpdc.egg-info/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      318 2024-04-30 10:57:59.000000 pynpdc-0.13.1/pynpdc.egg-info/SOURCES.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-04-30 10:57:59.000000 pynpdc-0.13.1/pynpdc.egg-info/dependency_links.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       54 2024-04-30 10:57:59.000000 pynpdc-0.13.1/pynpdc.egg-info/requires.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        7 2024-04-30 10:57:59.000000 pynpdc-0.13.1/pynpdc.egg-info/top_level.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      932 2024-04-30 10:55:29.000000 pynpdc-0.13.1/pyproject.toml
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-04-30 10:57:59.805313 pynpdc-0.13.1/setup.cfg
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-30 10:57:59.805313 pynpdc-0.13.1/tests/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     7253 2024-04-11 09:18:52.000000 pynpdc-0.13.1/tests/test_auth.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    27966 2024-04-26 11:20:41.000000 pynpdc-0.13.1/tests/test_dataset.py
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-02 12:05:05.985391 pynpdc-0.13.2/
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-05-02 12:05:05.985391 pynpdc-0.13.2/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     6577 2024-04-11 12:20:53.000000 pynpdc-0.13.2/README.md
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-02 12:05:05.985391 pynpdc-0.13.2/pynpdc/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1019 2024-05-02 12:01:47.000000 pynpdc-0.13.2/pynpdc/__init__.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    10243 2024-04-30 10:50:07.000000 pynpdc-0.13.2/pynpdc/auth.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    39396 2024-05-02 12:03:42.000000 pynpdc-0.13.2/pynpdc/dataset.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      443 2024-04-11 09:18:52.000000 pynpdc-0.13.2/pynpdc/exception.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        0 2024-04-26 08:07:44.000000 pynpdc-0.13.2/pynpdc/py.typed
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1504 2024-04-11 09:18:52.000000 pynpdc-0.13.2/pynpdc/types.py
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-02 12:05:05.985391 pynpdc-0.13.2/pynpdc.egg-info/
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-05-02 12:05:05.000000 pynpdc-0.13.2/pynpdc.egg-info/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      318 2024-05-02 12:05:05.000000 pynpdc-0.13.2/pynpdc.egg-info/SOURCES.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-05-02 12:05:05.000000 pynpdc-0.13.2/pynpdc.egg-info/dependency_links.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       54 2024-05-02 12:05:05.000000 pynpdc-0.13.2/pynpdc.egg-info/requires.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        7 2024-05-02 12:05:05.000000 pynpdc-0.13.2/pynpdc.egg-info/top_level.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      932 2024-05-02 12:01:10.000000 pynpdc-0.13.2/pyproject.toml
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-05-02 12:05:05.985391 pynpdc-0.13.2/setup.cfg
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-02 12:05:05.985391 pynpdc-0.13.2/tests/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     7253 2024-04-11 09:18:52.000000 pynpdc-0.13.2/tests/test_auth.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    27966 2024-04-26 11:20:41.000000 pynpdc-0.13.2/tests/test_dataset.py
```

### Comparing `pynpdc-0.13.1/PKG-INFO` & `pynpdc-0.13.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynpdc
-Version: 0.13.1
+Version: 0.13.2
 Summary: Python lib to interact with the NPDC stack
 Author-email: Olaf Schneider <olaf.schneider@npolar.no>, Mikhail Itkin <mikhail.itkin@npolar.no>
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pynpdc-0.13.1/README.md` & `pynpdc-0.13.2/README.md`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.1/pynpdc/__init__.py` & `pynpdc-0.13.2/pynpdc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # flake8: noqa
 
 from pynpdc.auth import (
     AUTH_LIFE_ENTRYPOINT as AUTH_LIFE_ENTRYPOINT,
     AUTH_STAGING_ENTRYPOINT as AUTH_STAGING_ENTRYPOINT,
     Account as Account,
+    AccountWithCleartextPassword as AccountWithCleartextPassword,
+    AccountWithToken as AccountWithToken,
     AuthClient as AuthClient,
 )
 
 from pynpdc.dataset import (
     DATASET_LIFE_ENTRYPOINT as DATASET_LIFE_ENTRYPOINT,
     DATASET_STAGING_ENTRYPOINT as DATASET_STAGING_ENTRYPOINT,
     DEFAULT_CHUNK_SIZE as DEFAULT_CHUNK_SIZE,
```

### Comparing `pynpdc-0.13.1/pynpdc/auth.py` & `pynpdc-0.13.2/pynpdc/auth.py`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.1/pynpdc/dataset.py` & `pynpdc-0.13.2/pynpdc/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from requests_toolbelt.multipart.encoder import MultipartEncoder  # type: ignore
 import requests
 import shutil
 from typing import (
     Any,
     BinaryIO,
     Dict,
-    Generator,
     Generic,
+    Iterator,
     Optional,
     Tuple,
     TypeVar,
     cast,
 )
 from typing_extensions import Self
 from urllib.parse import urlencode
@@ -432,15 +432,15 @@
 class LazyCollection(Generic[T], ABC):
     chunk_size: int
     client: DatasetClient
     model_class: type[Attachment | Dataset]
     query: dict[str, Any]
     skip: int
     take: int | None
-    _generator: Generator[T, None, None]
+    _generator: Iterator[T]
 
     def __init__(
         self,
         *,
         client: DatasetClient,
         chunk_size: int = DEFAULT_CHUNK_SIZE,
         **query: Any,
@@ -461,15 +461,15 @@
     def _endpoint(self) -> str:
         return ""
 
     def _request(self, query: Dict[str, Any]) -> requests.Response:
         url = self._endpoint + "?" + urlencode(query)
         return self.client._exec_request("GET", url)
 
-    def _generate(self) -> Generator[T, None, None]:
+    def _generate(self) -> Iterator[T]:
         chunk_size = self.chunk_size
         if self.take is not None and self.take < chunk_size:
             chunk_size = self.take
 
         query = {
             **self.query,
             "take": chunk_size,
```

### Comparing `pynpdc-0.13.1/pynpdc/types.py` & `pynpdc-0.13.2/pynpdc/types.py`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.1/pynpdc.egg-info/PKG-INFO` & `pynpdc-0.13.2/pynpdc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynpdc
-Version: 0.13.1
+Version: 0.13.2
 Summary: Python lib to interact with the NPDC stack
 Author-email: Olaf Schneider <olaf.schneider@npolar.no>, Mikhail Itkin <mikhail.itkin@npolar.no>
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pynpdc-0.13.1/pyproject.toml` & `pynpdc-0.13.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pynpdc"
-version = "0.13.1"
+version = "0.13.2"
 dependencies = [
     "requests",
     "requests-toolbelt",
     "typing-extensions",
     "werkzeug",
 ]
 requires-python = ">= 3.8"
```

### Comparing `pynpdc-0.13.1/tests/test_auth.py` & `pynpdc-0.13.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.1/tests/test_dataset.py` & `pynpdc-0.13.2/tests/test_dataset.py`

 * *Files identical despite different names*

