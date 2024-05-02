# Comparing `tmp/dig_ass_ocr_protos-0.0.4.tar.gz` & `tmp/dig_ass_ocr_protos-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ocr_protos-0.0.4.tar", last modified: Wed Apr 17 15:45:58 2024, max compression
+gzip compressed data, was "dig_ass_ocr_protos-0.0.5.tar", last modified: Thu May  2 11:12:53 2024, max compression
```

## Comparing `dig_ass_ocr_protos-0.0.4.tar` & `dig_ass_ocr_protos-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 15:45:58.129968 dig_ass_ocr_protos-0.0.4/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.4/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-17 15:45:58.129968 dig_ass_ocr_protos-0.0.4/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.4/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 15:45:58.129968 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1686 2024-04-17 15:45:56.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      692 2024-04-17 15:45:56.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2914 2024-04-17 15:45:56.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-17 15:45:14.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      648 2024-04-12 21:06:32.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 15:45:58.129968 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-17 15:45:58.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      498 2024-04-17 15:45:58.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-17 15:45:58.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-17 15:45:58.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-04-17 15:45:58.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.4/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-17 15:45:58.129968 dig_ass_ocr_protos-0.0.4/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      800 2024-04-11 10:26:57.000000 dig_ass_ocr_protos-0.0.4/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:53.894706 dig_ass_ocr_protos-0.0.5/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.5/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-05-02 11:12:53.894706 dig_ass_ocr_protos-0.0.5/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.5/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:53.894706 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1686 2024-05-02 11:12:52.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      692 2024-05-02 11:12:52.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2914 2024-05-02 11:12:52.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 11:11:21.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      662 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:53.894706 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-05-02 11:12:53.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      498 2024-05-02 11:12:53.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 11:12:53.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 11:12:53.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-02 11:12:53.000000 dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.5/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 11:12:53.894706 dig_ass_ocr_protos-0.0.5/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      800 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.5/setup.py
```

### Comparing `dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py` & `dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi` & `dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py` & `dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/client.py` & `dig_ass_ocr_protos-0.0.5/dig_ass_ocr_protos/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from dig_ass_ocr_protos.DigitalAssistantOCR_pb2_grpc import DigitalAssistantOCRStub
-from dig_ass_ocr_protos.DigitalAssistantOCR_pb2 import DigitalAssistantOCRRequest, DigitalAssistantOCRResponse
+from dig_ass_ocr_protos.DigitalAssistantOCR_pb2 import (
+    DigitalAssistantOCRRequest,
+    DigitalAssistantOCRResponse,
+)
 
 from .abstract_client import AbstractClient
 
+
 class OCRClient(AbstractClient):
     def __init__(self, address) -> None:
         super().__init__(address)
         self._stub = DigitalAssistantOCRStub(self._channel)
 
     def __call__(self, image: bytearray, pdf: bytearray):
         request = DigitalAssistantOCRRequest(Image=image, PDF=pdf)
```

### Comparing `dig_ass_ocr_protos-0.0.4/setup.py` & `dig_ass_ocr_protos-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 import re
 from setuptools import setup, find_packages
 
 from dig_ass_ocr_protos import __version__
 
 
 def read(file_path):
-    with io.open(file_path, "r", encoding="utf-8") as f:
+    with io.open(file_path, 'r', encoding='utf-8') as f:
         return f.read()
 
 
-readme = read("README.md")
+readme = read('README.md')
 # вычищаем локальные версии из файла requirements (согласно PEP440)
-requirements = "\n".join(
+requirements = '\n'.join(
     re.findall(
-        r"^([^\s^+]+).*$",
-        read("requirements.txt"),
+        r'^([^\s^+]+).*$',
+        read('requirements.txt'),
         flags=re.MULTILINE,
     )
 )
 
 setup(
     # metadata
-    name="dig_ass_ocr_protos",
+    name='dig_ass_ocr_protos',
     version=__version__,
-    author="AGI-MED-TEAM",
-    description="Proto files for dig_ass_ocr_protos",
+    author='AGI-MED-TEAM',
+    description='Proto files for dig_ass_ocr_protos',
     long_description=readme,
     # options
     packages=find_packages(),
-    install_requires="\n".join([requirements]),
+    install_requires='\n'.join([requirements]),
     include_package_data=True,
 )
```

