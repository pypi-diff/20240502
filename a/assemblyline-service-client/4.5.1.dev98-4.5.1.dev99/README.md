# Comparing `tmp/assemblyline_service_client-4.5.1.dev98-py3-none-any.whl.zip` & `tmp/assemblyline_service_client-4.5.1.dev99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9729 bytes, number of entries: 8
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-22 20:02 assemblyline_service_client/VERSION
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 20:02 assemblyline_service_client/__init__.py
--rw-r--r--  2.0 unx    23233 b- defN 24-Apr-22 20:02 assemblyline_service_client/task_handler.py
--rw-r--r--  2.0 unx     1396 b- defN 24-Apr-22 20:02 assemblyline_service_client-4.5.1.dev98.dist-info/LICENCE.md
--rw-r--r--  2.0 unx     1577 b- defN 24-Apr-22 20:02 assemblyline_service_client-4.5.1.dev98.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 20:02 assemblyline_service_client-4.5.1.dev98.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 24-Apr-22 20:02 assemblyline_service_client-4.5.1.dev98.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      803 b- defN 24-Apr-22 20:02 assemblyline_service_client-4.5.1.dev98.dist-info/RECORD
-8 files, 27141 bytes uncompressed, 8281 bytes compressed:  69.5%
+Zip file size: 9740 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-22 20:21 assemblyline_service_client/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 20:21 assemblyline_service_client/__init__.py
+-rw-r--r--  2.0 unx    23242 b- defN 24-Apr-22 20:21 assemblyline_service_client/task_handler.py
+-rw-r--r--  2.0 unx     1396 b- defN 24-Apr-22 20:21 assemblyline_service_client-4.5.1.dev99.dist-info/LICENCE.md
+-rw-r--r--  2.0 unx     1577 b- defN 24-Apr-22 20:21 assemblyline_service_client-4.5.1.dev99.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 20:21 assemblyline_service_client-4.5.1.dev99.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-22 20:21 assemblyline_service_client-4.5.1.dev99.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      803 b- defN 24-Apr-22 20:21 assemblyline_service_client-4.5.1.dev99.dist-info/RECORD
+8 files, 27150 bytes uncompressed, 8292 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: assemblyline_service_client/__init__.py
 Comment: 
 
 Filename: assemblyline_service_client/task_handler.py
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev98.dist-info/LICENCE.md
+Filename: assemblyline_service_client-4.5.1.dev99.dist-info/LICENCE.md
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev98.dist-info/METADATA
+Filename: assemblyline_service_client-4.5.1.dev99.dist-info/METADATA
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev98.dist-info/WHEEL
+Filename: assemblyline_service_client-4.5.1.dev99.dist-info/WHEEL
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev98.dist-info/top_level.txt
+Filename: assemblyline_service_client-4.5.1.dev99.dist-info/top_level.txt
 Comment: 
 
-Filename: assemblyline_service_client-4.5.1.dev98.dist-info/RECORD
+Filename: assemblyline_service_client-4.5.1.dev99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## assemblyline_service_client/VERSION

```diff
@@ -1 +1 @@
-4.5.1.dev98
+4.5.1.dev99
```

## assemblyline_service_client/task_handler.py

```diff
@@ -429,16 +429,16 @@
                 while not r['success'] and r['missing_files']:
                     for f_sha256 in r['missing_files']:
                         file_info = result_files[f_sha256]
                         headers = dict(
                             sha256=file_info['sha256'],
                             classification=file_info['classification'],
                             ttl=str(task.ttl),
-                            is_section_image=str(file_info.get('is_section_image', False))
                         )
+                        headers["Is-Section-Image"] = str(file_info.get('is_section_image', False))
 
                         with open(file_info['path'], 'rb') as fh:
                             # Upload the file requested by service server
                             self.log.info(f"[{task.sid}] Uploading file {file_info['path']} [{file_info['sha256']}]")
                             try:
                                 self.request_with_retries('put', self._path('file'), files=dict(file=fh),
                                                           headers=headers,timeout=FILE_REQUEST_TIMEOUT)
```

## Comparing `assemblyline_service_client-4.5.1.dev98.dist-info/LICENCE.md` & `assemblyline_service_client-4.5.1.dev99.dist-info/LICENCE.md`

 * *Files identical despite different names*

## Comparing `assemblyline_service_client-4.5.1.dev98.dist-info/METADATA` & `assemblyline_service_client-4.5.1.dev99.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-service-client
-Version: 4.5.1.dev98
+Version: 4.5.1.dev99
 Summary: Assemblyline 4 - Service client
 Home-page: https://github.com/CybercentreCanada/assemblyline-service-client/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `assemblyline_service_client-4.5.1.dev98.dist-info/RECORD` & `assemblyline_service_client-4.5.1.dev99.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-assemblyline_service_client/VERSION,sha256=NxTYIb4TeI-fwiSdZ6FGC9h7rpr9cCfPxWcXtCxv7gU,12
+assemblyline_service_client/VERSION,sha256=0WpTt07sdsYDEyZ2ujT1Jv9yTsDp7oYK3rBVi1Bcfv4,12
 assemblyline_service_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-assemblyline_service_client/task_handler.py,sha256=U6OmqDSbBY9p-JccwdFImZ436McK_PK-A5Pl6d54Kko,23233
-assemblyline_service_client-4.5.1.dev98.dist-info/LICENCE.md,sha256=NSkYo9EH8h5oOkzg4VhjAHF4339MqPP2cQ8msTPgl-c,1396
-assemblyline_service_client-4.5.1.dev98.dist-info/METADATA,sha256=bk3CtKSK_zIE3ieUYl3Snv3Swc8iYd7AXOyF1Dd2He8,1577
-assemblyline_service_client-4.5.1.dev98.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-assemblyline_service_client-4.5.1.dev98.dist-info/top_level.txt,sha256=clNWHvn8nw0kR15l5TASxWxIQvKGKe5Pso3kVPMiJv0,28
-assemblyline_service_client-4.5.1.dev98.dist-info/RECORD,,
+assemblyline_service_client/task_handler.py,sha256=oNSpF2pNBX8CMETpMP5S0gcqLUQwx6j8gt-fxj2mufo,23242
+assemblyline_service_client-4.5.1.dev99.dist-info/LICENCE.md,sha256=NSkYo9EH8h5oOkzg4VhjAHF4339MqPP2cQ8msTPgl-c,1396
+assemblyline_service_client-4.5.1.dev99.dist-info/METADATA,sha256=bGcHL_k-vWRJA0fJkWIXCiikHSEkMOhsRJihshNFyvw,1577
+assemblyline_service_client-4.5.1.dev99.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+assemblyline_service_client-4.5.1.dev99.dist-info/top_level.txt,sha256=clNWHvn8nw0kR15l5TASxWxIQvKGKe5Pso3kVPMiJv0,28
+assemblyline_service_client-4.5.1.dev99.dist-info/RECORD,,
```

