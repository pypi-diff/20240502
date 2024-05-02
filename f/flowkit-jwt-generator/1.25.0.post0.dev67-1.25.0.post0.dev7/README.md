# Comparing `tmp/flowkit_jwt_generator-1.25.0.post0.dev67-py3-none-any.whl.zip` & `tmp/flowkit_jwt_generator-1.25.0.post0.dev7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8543 bytes, number of entries: 10
--rw-r--r--  2.0 unx      507 b- defN 24-May-02 04:52 flowkit_jwt_generator/__init__.py
--rw-r--r--  2.0 unx      510 b- defN 24-May-02 04:52 flowkit_jwt_generator/_version.py
--rw-r--r--  2.0 unx     1591 b- defN 24-May-02 04:52 flowkit_jwt_generator/cli.py
--rw-r--r--  2.0 unx     3405 b- defN 24-May-02 04:52 flowkit_jwt_generator/fixtures.py
--rw-r--r--  2.0 unx     9215 b- defN 24-May-02 04:52 flowkit_jwt_generator/jwt.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-02 04:52 flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 04:52 flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/WHEEL
--rw-r--r--  2.0 unx      138 b- defN 24-May-02 04:52 flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 24-May-02 04:52 flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 24-May-02 04:52 flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/RECORD
-10 files, 17781 bytes uncompressed, 6845 bytes compressed:  61.5%
+Zip file size: 8527 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-30 15:22 flowkit_jwt_generator/__init__.py
+-rw-r--r--  2.0 unx      509 b- defN 24-Apr-30 15:22 flowkit_jwt_generator/_version.py
+-rw-r--r--  2.0 unx     1591 b- defN 24-Apr-30 15:22 flowkit_jwt_generator/cli.py
+-rw-r--r--  2.0 unx     3405 b- defN 24-Apr-30 15:22 flowkit_jwt_generator/fixtures.py
+-rw-r--r--  2.0 unx     9215 b- defN 24-Apr-30 15:22 flowkit_jwt_generator/jwt.py
+-rw-r--r--  2.0 unx     1333 b- defN 24-Apr-30 15:22 flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 15:22 flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      138 b- defN 24-Apr-30 15:22 flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-30 15:22 flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      962 b- defN 24-Apr-30 15:22 flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/RECORD
+10 files, 17774 bytes uncompressed, 6839 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: flowkit_jwt_generator/fixtures.py
 Comment: 
 
 Filename: flowkit_jwt_generator/jwt.py
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/METADATA
+Filename: flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/METADATA
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/WHEEL
+Filename: flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/WHEEL
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/entry_points.txt
+Filename: flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/entry_points.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/top_level.txt
+Filename: flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/top_level.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/RECORD
+Filename: flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flowkit_jwt_generator/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-05-02T04:49:08+0000",
+ "date": "2024-04-30T15:19:50+0000",
  "dirty": false,
  "error": null,
- "full-revisionid": "f74639f5e61f1d5ba95b54322f025bf78f578fc8",
- "version": "1.25.0.post0.dev67"
+ "full-revisionid": "113017f48374b8816efda23673d0476e6fd81674",
+ "version": "1.25.0.post0.dev7"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/METADATA` & `flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowkit_jwt_generator
-Version: 1.25.0.post0.dev67
+Version: 1.25.0.post0.dev7
 Summary: Common test JWT generator for FlowKit.
 Home-page: https://github.com/Flowminder/FlowKit
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
```

## Comparing `flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/RECORD` & `flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 flowkit_jwt_generator/__init__.py,sha256=Vqa2vcGLH7wfO7GXFiSQX2QXctRgwUuM-QG9DJ0HQqk,507
-flowkit_jwt_generator/_version.py,sha256=HhIitYNFtGjuNfloUsRdsepR0gRrNDBENhJPOSzbdik,510
+flowkit_jwt_generator/_version.py,sha256=_6rVRgEXjrqESm3FvLiNv9y1tdKZE4n7ZCyKOb2XG54,509
 flowkit_jwt_generator/cli.py,sha256=hx88rA2O7sqhQ0EHQTCVrZpcdBLW-qssaaodnpXV1DQ,1591
 flowkit_jwt_generator/fixtures.py,sha256=jVDYkagDNtu_m94ns2F6sDtqMmq1kBygS6DBaMqBGoo,3405
 flowkit_jwt_generator/jwt.py,sha256=R_IjXQwtq3eYOmEVcHp7bOCtBgoGUyUpmrJRKsp1MMc,9215
-flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/METADATA,sha256=SKox5p8sPRuNIBDHpopzgrlhR3RWs2JmBKaI9pEFD6M,1334
-flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/entry_points.txt,sha256=dn2fWa3YIICO8NuUzecgAhZjHJqa_hCnJkRPdwdYW5I,138
-flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/top_level.txt,sha256=qNfUi5RerckeRiSkJOlGGv5098vruKE2Ck_3TbYyci4,22
-flowkit_jwt_generator-1.25.0.post0.dev67.dist-info/RECORD,,
+flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/METADATA,sha256=wRcdNMt0yGsCzlx4DxGZCVMkiMUgpfxGN5TBKQvup_s,1333
+flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/entry_points.txt,sha256=dn2fWa3YIICO8NuUzecgAhZjHJqa_hCnJkRPdwdYW5I,138
+flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/top_level.txt,sha256=qNfUi5RerckeRiSkJOlGGv5098vruKE2Ck_3TbYyci4,22
+flowkit_jwt_generator-1.25.0.post0.dev7.dist-info/RECORD,,
```

