# Comparing `tmp/pyiotown-0.5.1-py3-none-any.whl.zip` & `tmp/pyiotown-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 7775 bytes, number of entries: 11
+Zip file size: 8371 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-05 08:55 pyiotown/__init__.py
+-rw-r--r--  2.0 unx      795 b- defN 24-Apr-30 13:17 pyiotown/command.py
 -rw-r--r--  2.0 unx      925 b- defN 23-Sep-04 05:59 pyiotown/delete.py
--rw-r--r--  2.0 unx     3948 b- defN 23-Oct-26 01:24 pyiotown/get.py
+-rw-r--r--  2.0 unx     4313 b- defN 24-Mar-21 23:18 pyiotown/get.py
 -rw-r--r--  2.0 unx     5058 b- defN 23-Sep-04 06:00 pyiotown/post.py
--rw-r--r--  2.0 unx     8413 b- defN 24-Mar-11 22:49 pyiotown/post_process.py
--rw-r--r--  2.0 unx     1053 b- defN 24-Mar-11 22:50 pyiotown-0.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      696 b- defN 24-Mar-11 22:50 pyiotown-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-11 22:50 pyiotown-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 24-Mar-11 22:50 pyiotown-0.5.1.dist-info/pbr.json
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-11 22:50 pyiotown-0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      851 b- defN 24-Mar-11 22:50 pyiotown-0.5.1.dist-info/RECORD
-11 files, 21092 bytes uncompressed, 6337 bytes compressed:  70.0%
+-rw-r--r--  2.0 unx     8447 b- defN 24-Apr-22 22:44 pyiotown/post_process.py
+-rw-r--r--  2.0 unx     1053 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      696 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/pbr.json
+-rw-r--r--  2.0 unx        9 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      926 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/RECORD
+12 files, 22361 bytes uncompressed, 6819 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,34 +1,37 @@
 Filename: pyiotown/__init__.py
 Comment: 
 
+Filename: pyiotown/command.py
+Comment: 
+
 Filename: pyiotown/delete.py
 Comment: 
 
 Filename: pyiotown/get.py
 Comment: 
 
 Filename: pyiotown/post.py
 Comment: 
 
 Filename: pyiotown/post_process.py
 Comment: 
 
-Filename: pyiotown-0.5.1.dist-info/LICENSE
+Filename: pyiotown-0.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: pyiotown-0.5.1.dist-info/METADATA
+Filename: pyiotown-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: pyiotown-0.5.1.dist-info/WHEEL
+Filename: pyiotown-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyiotown-0.5.1.dist-info/pbr.json
+Filename: pyiotown-0.5.2.dist-info/pbr.json
 Comment: 
 
-Filename: pyiotown-0.5.1.dist-info/top_level.txt
+Filename: pyiotown-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyiotown-0.5.1.dist-info/RECORD
+Filename: pyiotown-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyiotown/get.py

```diff
@@ -18,15 +18,15 @@
     
     if r.status_code == 200:
         return r.json()
     else:
         print(r)
         return None
     
-def storage(url, token, nid=None, date_from=None, date_to=None, count=None, sort=None, lastKey="", group_id=None, verify=True, timeout=60):
+def storage(url, token, nid=None, date_from=None, date_to=None, count=None, sort=None, lastKey=None, consolidate=True, group_id=None, verify=True, timeout=60):
     '''
     url : IoT.own Server Address
     token : IoT.own API Token
     nid : Node ID
     '''
                     
     header = {'Accept':'application/json','token':token}
@@ -35,52 +35,60 @@
     if group_id is not None:
         header['grpid'] = group_id
 
     uri_prefix = url + "/api/v1.0/storage"
 
     params = []
     
-    if nid != None:
+    if nid is not None:
         params.append(f"nid={nid}")
         
-    if date_from != None:
+    if date_from is not None:
         params.append(f"from={date_from}")
 
-    if date_to != None:
+    if date_to is not None:
         params.append(f"to={date_to}")
 
-    if count != None:
+    if count is not None:
         params.append(f"count={count}")
 
-    if sort != None:
+    if sort is not None:
         params.append(f"sort={sort}")
 
     if len(params) > 0:
         uri_prefix += '?' + '&'.join(params)
         
     result = None
     
     while True:
         try:
-            uri = uri_prefix if lastKey == "" else uri_prefix + "&lastKey=" + lastKey
+            uri = uri_prefix if lastKey is None else uri_prefix + "&lastKey=" + lastKey
+            print(uri)
             r = requests.get(uri, headers=header, verify=verify, timeout=timeout)
         except Exception as e:
             print(e)
             return None
     
         if r.status_code == 200:
+            data_obj = r.json()
             if result is None:
-                result = r.json()
-                if 'lastKey' in result.keys():
-                    del result['lastKey']
+                # at first
+                result = data_obj
+                
+                # if 'lastKey' in result.keys():
+                #     del result['lastKey']
             else:
-                result['data'] += r.json()['data']
+                result['data'] += data_obj['data']
+                if 'lastKey' in data_obj.keys():
+                    result['lastKey'] = data_obj['lastKey']
+                elif 'lastKey' in result.keys():
+                    del result['lastKey']
 
-            if 'lastKey' in r.json().keys():
-                lastKey = r.json()['lastKey']
+            if consolidate == True and 'lastKey' in result.keys():
+                lastKey = result['lastKey']
             else:
                 return result
         else:
             print(r)
             return None
 
 def command(url, token, nid, group_id=None, verify=True, timeout=60):
```

## pyiotown/post_process.py

```diff
@@ -1,17 +1,19 @@
 from .post import post_files
 import json
 from urllib.parse import urlparse
 import paho.mqtt.client as mqtt
 import sys
 import ssl
+import requests
+import threading
 
 def on_connect(client, userdata, flags, reason_code, properties):
     if reason_code.is_failure:
-        print(f"Bad connection (reason: {reason_code.getName()}", file=sys.stderr)
+        print(f"Bad connection (reason: {reason_code.getName()})", file=sys.stderr)
         sys.exit(3)
     else:
         name = userdata['name']
         print(f"Post process '{name}' Connect OK! Subscribe Start")
 
 def on_disconnect(client, userdata, flags, reason_code, properties):
     if reason_code.is_failure:
```

## Comparing `pyiotown-0.5.1.dist-info/LICENSE` & `pyiotown-0.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyiotown-0.5.1.dist-info/METADATA` & `pyiotown-0.5.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiotown
-Version: 0.5.1
+Version: 0.5.2
 Summary: IoT.own Library
 Home-page: https://github.com/CoXlabInc/pyiotow
 Author: CoXlab Inc.
 Author-email: support@coxlab.kr
 Maintainer: Jongsoo Jeong
 Maintainer-email: jsjeong@coxlab.k
 License: MIT
```

