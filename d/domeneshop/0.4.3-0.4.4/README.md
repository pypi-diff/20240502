# Comparing `tmp/domeneshop-0.4.3.tar.gz` & `tmp/domeneshop-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domeneshop-0.4.3.tar", last modified: Thu Nov 17 10:20:45 2022, max compression
+gzip compressed data, was "domeneshop-0.4.4.tar", last modified: Thu May  2 09:22:57 2024, max compression
```

## Comparing `domeneshop-0.4.3.tar` & `domeneshop-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rye        (501) staff       (20)        0 2022-11-17 10:20:45.212622 domeneshop-0.4.3/
--rw-r--r--   0 rye        (501) staff       (20)     1069 2022-10-20 07:27:38.000000 domeneshop-0.4.3/LICENSE
--rw-r--r--   0 rye        (501) staff       (20)       15 2022-10-20 07:27:38.000000 domeneshop-0.4.3/MANIFEST.in
--rw-r--r--   0 rye        (501) staff       (20)     2249 2022-11-17 10:20:45.212719 domeneshop-0.4.3/PKG-INFO
--rw-r--r--   0 rye        (501) staff       (20)     1090 2022-11-17 10:14:26.000000 domeneshop-0.4.3/README.rst
-drwxr-xr-x   0 rye        (501) staff       (20)        0 2022-11-17 10:20:45.211005 domeneshop-0.4.3/domeneshop/
--rw-r--r--   0 rye        (501) staff       (20)       49 2022-10-20 07:27:38.000000 domeneshop-0.4.3/domeneshop/__init__.py
--rw-r--r--   0 rye        (501) staff       (20)     8764 2022-11-17 10:12:48.000000 domeneshop-0.4.3/domeneshop/client.py
-drwxr-xr-x   0 rye        (501) staff       (20)        0 2022-11-17 10:20:45.212415 domeneshop-0.4.3/domeneshop.egg-info/
--rw-r--r--   0 rye        (501) staff       (20)     2249 2022-11-17 10:20:45.000000 domeneshop-0.4.3/domeneshop.egg-info/PKG-INFO
--rw-r--r--   0 rye        (501) staff       (20)      262 2022-11-17 10:20:45.000000 domeneshop-0.4.3/domeneshop.egg-info/SOURCES.txt
--rw-r--r--   0 rye        (501) staff       (20)        1 2022-11-17 10:20:45.000000 domeneshop-0.4.3/domeneshop.egg-info/dependency_links.txt
--rw-r--r--   0 rye        (501) staff       (20)       51 2022-11-17 10:20:45.000000 domeneshop-0.4.3/domeneshop.egg-info/requires.txt
--rw-r--r--   0 rye        (501) staff       (20)       11 2022-11-17 10:20:45.000000 domeneshop-0.4.3/domeneshop.egg-info/top_level.txt
--rw-r--r--   0 rye        (501) staff       (20)       67 2022-11-17 10:20:45.213056 domeneshop-0.4.3/setup.cfg
--rw-r--r--   0 rye        (501) staff       (20)     1564 2022-11-17 10:17:05.000000 domeneshop-0.4.3/setup.py
+drwxr-xr-x   0 rye        (501) staff       (20)        0 2024-05-02 09:22:57.035572 domeneshop-0.4.4/
+-rw-r--r--   0 rye        (501) staff       (20)     1070 2024-05-02 09:09:28.000000 domeneshop-0.4.4/LICENSE
+-rw-r--r--   0 rye        (501) staff       (20)       15 2024-05-02 08:57:54.000000 domeneshop-0.4.4/MANIFEST.in
+-rw-r--r--   0 rye        (501) staff       (20)     2362 2024-05-02 09:22:57.035501 domeneshop-0.4.4/PKG-INFO
+-rw-r--r--   0 rye        (501) staff       (20)     1059 2024-05-02 09:20:49.000000 domeneshop-0.4.4/README.rst
+drwxr-xr-x   0 rye        (501) staff       (20)        0 2024-05-02 09:22:57.034422 domeneshop-0.4.4/domeneshop/
+-rw-r--r--   0 rye        (501) staff       (20)       49 2024-05-02 09:09:07.000000 domeneshop-0.4.4/domeneshop/__init__.py
+-rw-r--r--   0 rye        (501) staff       (20)     8734 2024-05-02 09:16:02.000000 domeneshop-0.4.4/domeneshop/client.py
+drwxr-xr-x   0 rye        (501) staff       (20)        0 2024-05-02 09:22:57.035254 domeneshop-0.4.4/domeneshop.egg-info/
+-rw-r--r--   0 rye        (501) staff       (20)     2362 2024-05-02 09:22:57.000000 domeneshop-0.4.4/domeneshop.egg-info/PKG-INFO
+-rw-r--r--   0 rye        (501) staff       (20)      262 2024-05-02 09:22:57.000000 domeneshop-0.4.4/domeneshop.egg-info/SOURCES.txt
+-rw-r--r--   0 rye        (501) staff       (20)        1 2024-05-02 09:22:57.000000 domeneshop-0.4.4/domeneshop.egg-info/dependency_links.txt
+-rw-r--r--   0 rye        (501) staff       (20)       29 2024-05-02 09:22:57.000000 domeneshop-0.4.4/domeneshop.egg-info/requires.txt
+-rw-r--r--   0 rye        (501) staff       (20)       11 2024-05-02 09:22:57.000000 domeneshop-0.4.4/domeneshop.egg-info/top_level.txt
+-rw-r--r--   0 rye        (501) staff       (20)       67 2024-05-02 09:22:57.035758 domeneshop-0.4.4/setup.cfg
+-rw-r--r--   0 rye        (501) staff       (20)     1592 2024-05-02 09:10:18.000000 domeneshop-0.4.4/setup.py
```

### Comparing `domeneshop-0.4.3/LICENSE` & `domeneshop-0.4.4/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Domeneshop AS
+Copyright (c) 2024 Domeneshop AS
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `domeneshop-0.4.3/PKG-INFO` & `domeneshop-0.4.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: domeneshop
-Version: 0.4.3
+Version: 0.4.4
 Summary: Domeneshop API library
 Home-page: https://github.com/domeneshop/python-domeneshop
 Author: Domeneshop AS
 Author-email: kundeservice@domeneshop.no
 License: MIT License
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
-Requires-Python: !=2.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
-Provides-Extra: dev
+Requires-Python: !=2.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 License-File: LICENSE
+Requires-Dist: urllib3
+Requires-Dist: certifi
+Provides-Extra: dev
+Requires-Dist: wheel; extra == "dev"
 
 domeneshop
 ==========
 
 Python 3 library for working with the Domeneshop_ API.
 
 **Note:** This library does *not* support Python 2.x.
@@ -70,10 +74,8 @@
             print(record["id"], record["host"], record["type"], record["data"])
 
 More examples can be found in the `examples <examples/>`_ folder.
 
 Documentation
 -------------
 
-Coming soon.
-
-In the meantime, see the docstrings for `domeneshop.client.Client <src/domeneshop/client.py>`_.
+See the docstrings for `domeneshop.client.Client <src/domeneshop/client.py>`_.
```

### Comparing `domeneshop-0.4.3/README.rst` & `domeneshop-0.4.4/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -40,10 +40,8 @@
             print(record["id"], record["host"], record["type"], record["data"])
 
 More examples can be found in the `examples <examples/>`_ folder.
 
 Documentation
 -------------
 
-Coming soon.
-
-In the meantime, see the docstrings for `domeneshop.client.Client <src/domeneshop/client.py>`_.
+See the docstrings for `domeneshop.client.Client <src/domeneshop/client.py>`_.
```

### Comparing `domeneshop-0.4.3/domeneshop/client.py` & `domeneshop-0.4.4/domeneshop/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Domeneshop API client implementation."""
 
+import base64
 import json
 import logging
 from typing import List
 
-import urllib3
 import certifi
-import base64
+import urllib3
 
 logger = logging.getLogger(__name__)
 
 VALID_TYPES = [
     "A",
     "AAAA",
     "CNAME",
@@ -50,97 +50,104 @@
 
         self._headers = {
             "Authorization": "Basic {}".format(
                 base64.b64encode("{}:{}".format(token, secret).encode()).decode()
             ),
             "Accept": "application/json",
             "Content-Type": "application/json",
-            "User-Agent": "domeneshop-python/0.4.3",
+            "User-Agent": "domeneshop-python/0.4.4",
         }
         self._http = urllib3.HTTPSConnectionPool(
-            "api.domeneshop.no", 443, maxsize=5, block=True, headers=self._headers, cert_reqs='CERT_REQUIRED', ca_certs=certifi.where()
+            "api.domeneshop.no",
+            443,
+            maxsize=5,
+            block=True,
+            headers=self._headers,
+            cert_reqs="CERT_REQUIRED",
+            ca_certs=certifi.where(),
         )
 
     # Domains
 
     def get_domains(self) -> List[dict]:
         """
         Retrieve a list of all domains.
 
         :return: A list of domain dictionaries
 
         """
         resp = self._request("GET", "/domains")
-        domains = json.loads(resp.data.decode('utf-8'))
+        domains = json.loads(resp.data.decode("utf-8"))
         return domains
 
     def get_domain(self, domain_id: int) -> dict:
         """
         Retrieve a domain.
-        
+
         :param domain_id: The domain ID to retrieve
 
         :return: A domain dictionary
         """
 
         resp = self._request("GET", "/domains/{0}".format(domain_id))
-        domain = json.loads(resp.data.decode('utf-8'))
+        domain = json.loads(resp.data.decode("utf-8"))
         return domain
 
     # DNS records
 
     def get_records(self, domain_id: int) -> List[dict]:
         """
         Retrieve DNS records for a domain, or raises an error.
-        
+
         :param domain_id: The domain ID to operate on
 
         :return: A list of record dictionaries
         """
         resp = self._request("GET", "/domains/{0}/dns".format(domain_id))
-        records = json.loads(resp.data.decode('utf-8'))
+        records = json.loads(resp.data.decode("utf-8"))
         return records
 
     def get_record(self, domain_id: int, record_id: int) -> dict:
         """
         Retrieve a specific DNS record for a domain, or raises an error.
-        
+
         :param domain_id: The domain ID to operate on
         :param record_id: The DNS record ID to retrieve
 
         :return: A record dictionary
         """
         resp = self._request("GET", "/domains/{0}/dns/{1}".format(domain_id, record_id))
-        record = json.loads(resp.data.decode('utf-8'))
+        record = json.loads(resp.data.decode("utf-8"))
         return record
 
-    def create_record(self, domain_id: int, record: int) -> int:
+    def create_record(self, domain_id: int, record: dict) -> int:
         """
         Create a DNS record for a domain, or raises an error. The record is validated
         primitively before being passed on to the API.
-        
+
         :param domain_id: The domain ID to operate on
         :param record: A dict
 
         :return: The Record ID of the created record.
 
         Raises:
             TypeError: If the record appears to be invalid
         """
         _validate_record(record)
         resp = self._request("POST", "/domains/{0}/dns".format(domain_id), data=record)
 
-        record_id = resp.headers.get("location").split("/")[-1]
+        record_id = resp.headers.get("location").split("/")[-1]  # type: ignore
+
         return int(record_id)
 
     def modify_record(self, domain_id: int, record_id: int, record: dict) -> None:
         """
         Modify a DNS record for a domain, or raises an error. The record is validated
         primitively before being passed on to the API.
-        
+
         :param domain_id:  The domain ID to operate on
         :param record: A dict
 
         :return: A list of record dictionaries
 
         Raises:
             TypeError if the record appears to be invalid.
@@ -149,103 +156,99 @@
         self._request(
             "PUT", "/domains/{0}/dns/{1}".format(domain_id, record_id), data=record
         )
 
     def delete_record(self, domain_id: int, record_id: int) -> None:
         """
         Delete a DNS record for a domain, or raises an error.
-        
+
         :param domain_id:  The domain ID to operate on
         :param record_id: The record ID to delete
         """
         self._request("DELETE", "/domains/{0}/dns/{1}".format(domain_id, record_id))
 
     # Forwards
 
     def get_forwards(self, domain_id: int) -> List[dict]:
         """
         Retrieve forwardings for a domain, or raises an error.
-        
+
         :param domain_id: The domain ID to operate on
 
         :return: A list of forwarding dictionaries
         """
         resp = self._request("GET", "/domains/{0}/forwards".format(domain_id))
-        records = json.loads(resp.data.decode('utf-8'))
+        records = json.loads(resp.data.decode("utf-8"))
         return records
 
     def get_forward(self, domain_id: int, host: str) -> List[dict]:
         """
         Retrieve forwardings for a domain, or raises an error.
-        
+
         :param domain_id: The domain ID to operate on
 
         :return: A list of forwarding dictionaries
         """
         resp = self._request("GET", "/domains/{0}/forwards/{1}".format(domain_id, host))
-        records = json.loads(resp.data.decode('utf-8'))
+        records = json.loads(resp.data.decode("utf-8"))
         return records
 
     def create_forward(
         self, domain_id: int, host: str, target: str, frame=False
     ) -> None:
         """
         Create a forwarding for a domain, or raises an error.
-        
+
         :param domain_id:  The domain ID to operate on
         :param host:  The host (subdomain) to modify
         :param forward: A dict
 
         :return: A list of record dictionaries
 
         """
 
         forward = {"frame": frame, "host": host, "url": target}
 
-        print(forward)
-
-        self._request(
-            "POST", "/domains/{0}/forwards".format(domain_id, host), data=forward
-        )
+        self._request("POST", "/domains/{0}/forwards".format(domain_id), data=forward)
 
     def modify_forward(
         self, domain_id: int, host: str, target: str, frame=False
     ) -> None:
         """
         Modify a forwarding for a domain, or raises an error.
-        
+
         :param domain_id:  The domain ID to operate on
         :param host:  The host (subdomain) to modify
         :param forward: A dict
         """
 
         forward = {"frame": frame, "host": host, "url": target}
 
         self._request(
             "PUT", "/domains/{0}/forwards/{1}".format(domain_id, host), data=forward
         )
 
     def delete_forward(self, domain_id: int, host: str) -> None:
         """
         Deletes a forwarding for a domain, or raises an error.
-        
+
         :param domain_id:  The domain ID to operate on
         :param host:  The host (subdomain) to delete
         """
 
         self._request("DELETE", "/domains/{0}/forwards/{1}".format(domain_id, host))
 
     def _request(self, method="GET", endpoint="/", data=None):
         if data is not None:
             data = json.dumps(data).encode("utf-8")
         try:
             resp = self._http.request(method, "/v0" + endpoint, body=data)
             if resp.status >= 400:
                 try:
-                    data = json.loads(resp.data.decode('utf-8'))
+                    data = json.loads(resp.data.decode("utf-8"))
                 except json.JSONDecodeError:
                     data = {"error": resp.status, "help": "A server error occurred."}
                 raise DomeneshopError(resp.status, data) from None
         except urllib3.exceptions.HTTPError as e:
             raise e
         else:
             return resp
@@ -272,15 +275,15 @@
         super().__init__(error_message)
 
 
 def _validate_record(record: dict):
     record_keys = set(record.keys())
     record_type = record.get("type")
 
-    if record_type not in VALID_TYPES:
+    if not record_type or record_type not in VALID_TYPES:
         raise TypeError("Record has invalid type. Valid types: {0}".format(VALID_TYPES))
 
     required_keys = COMMON_KEYS | VALID_KEYS.get(record_type, set())
 
     if record_keys != required_keys:
         raise TypeError(
             "Record is missing or has invalid keys. Required keys: {0}".format(
```

### Comparing `domeneshop-0.4.3/domeneshop.egg-info/PKG-INFO` & `domeneshop-0.4.4/domeneshop.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: domeneshop
-Version: 0.4.3
+Version: 0.4.4
 Summary: Domeneshop API library
 Home-page: https://github.com/domeneshop/python-domeneshop
 Author: Domeneshop AS
 Author-email: kundeservice@domeneshop.no
 License: MIT License
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
-Requires-Python: !=2.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
-Provides-Extra: dev
+Requires-Python: !=2.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 License-File: LICENSE
+Requires-Dist: urllib3
+Requires-Dist: certifi
+Provides-Extra: dev
+Requires-Dist: wheel; extra == "dev"
 
 domeneshop
 ==========
 
 Python 3 library for working with the Domeneshop_ API.
 
 **Note:** This library does *not* support Python 2.x.
@@ -70,10 +74,8 @@
             print(record["id"], record["host"], record["type"], record["data"])
 
 More examples can be found in the `examples <examples/>`_ folder.
 
 Documentation
 -------------
 
-Coming soon.
-
-In the meantime, see the docstrings for `domeneshop.client.Client <src/domeneshop/client.py>`_.
+See the docstrings for `domeneshop.client.Client <src/domeneshop/client.py>`_.
```

### Comparing `domeneshop-0.4.3/setup.py` & `domeneshop-0.4.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from setuptools import find_packages, setup
 
-
 INSTALL_REQUIRES = ["urllib3", "certifi"]
 
-DEV_EXTRAS = ["black", "mypy", "prospector", "wheel"]
+DEV_EXTRAS = ["wheel"]
 
 with open("README.rst", "rb") as f:
     LONG_DESCRIPTION = f.read().decode("utf-8")
 
 setup(
     name="domeneshop",
-    version="0.4.3",
+    version="0.4.4",
     description="Domeneshop API library",
     author="Domeneshop AS",
     url="https://github.com/domeneshop/python-domeneshop",
     license="MIT License",
     long_description=LONG_DESCRIPTION,
-    python_requires="!=2.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*",
+    python_requires="!=2.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*",
     classifiers=[
         "Environment :: Plugins",
         "Intended Audience :: System Administrators",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Security",
         "Topic :: System :: Installation/Setup",
         "Topic :: System :: Networking",
         "Topic :: System :: Systems Administration",
         "Topic :: Utilities",
     ],
```

