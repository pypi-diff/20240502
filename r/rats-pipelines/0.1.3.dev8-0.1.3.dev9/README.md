# Comparing `tmp/rats_pipelines-0.1.3.dev8-py3-none-any.whl.zip` & `tmp/rats_pipelines-0.1.3.dev9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 48750 bytes, number of entries: 81
+Zip file size: 48749 bytes, number of entries: 81
 -rw-r--r--  2.0 unx      679 b- defN 80-Jan-01 00:00 rats/app/__init__.py
 -rw-r--r--  2.0 unx      832 b- defN 80-Jan-01 00:00 rats/app/_building_di_container.py
 -rw-r--r--  2.0 unx      475 b- defN 80-Jan-01 00:00 rats/app/_building_services.py
 -rw-r--r--  2.0 unx      714 b- defN 80-Jan-01 00:00 rats/app/_dag_di_container.py
 -rw-r--r--  2.0 unx     3867 b- defN 80-Jan-01 00:00 rats/app/_io2_di_container.py
 -rw-r--r--  2.0 unx     3067 b- defN 80-Jan-01 00:00 rats/app/_io_di_container.py
 -rw-r--r--  2.0 unx     5986 b- defN 80-Jan-01 00:00 rats/app/_rats_app.py
@@ -72,12 +72,12 @@
 -rw-r--r--  2.0 unx     2350 b- defN 80-Jan-01 00:00 rats/services/_scopes.py
 -rw-r--r--  2.0 unx     3798 b- defN 80-Jan-01 00:00 rats/services/_service_container.py
 -rw-r--r--  2.0 unx     2587 b- defN 80-Jan-01 00:00 rats/services/_service_factory.py
 -rw-r--r--  2.0 unx     3289 b- defN 80-Jan-01 00:00 rats/services/_service_managers.py
 -rw-r--r--  2.0 unx      598 b- defN 80-Jan-01 00:00 rats/services/_services.py
 -rw-r--r--  2.0 unx     1409 b- defN 80-Jan-01 00:00 rats/services/_typed_containers.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 rats/services/py.typed
--rw-r--r--  2.0 unx      774 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.3.dev8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.3.dev8.dist-info/WHEEL
--rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.3.dev8.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     6861 b- defN 16-Jan-01 00:00 rats_pipelines-0.1.3.dev8.dist-info/RECORD
-81 files, 124877 bytes uncompressed, 37868 bytes compressed:  69.7%
+-rw-r--r--  2.0 unx      774 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.3.dev9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.3.dev9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       85 b- defN 80-Jan-01 00:00 rats_pipelines-0.1.3.dev9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     6861 b- defN 16-Jan-01 00:00 rats_pipelines-0.1.3.dev9.dist-info/RECORD
+81 files, 124877 bytes uncompressed, 37867 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -225,20 +225,20 @@
 
 Filename: rats/services/_typed_containers.py
 Comment: 
 
 Filename: rats/services/py.typed
 Comment: 
 
-Filename: rats_pipelines-0.1.3.dev8.dist-info/METADATA
+Filename: rats_pipelines-0.1.3.dev9.dist-info/METADATA
 Comment: 
 
-Filename: rats_pipelines-0.1.3.dev8.dist-info/WHEEL
+Filename: rats_pipelines-0.1.3.dev9.dist-info/WHEEL
 Comment: 
 
-Filename: rats_pipelines-0.1.3.dev8.dist-info/entry_points.txt
+Filename: rats_pipelines-0.1.3.dev9.dist-info/entry_points.txt
 Comment: 
 
-Filename: rats_pipelines-0.1.3.dev8.dist-info/RECORD
+Filename: rats_pipelines-0.1.3.dev9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rats_pipelines-0.1.3.dev8.dist-info/METADATA` & `rats_pipelines-0.1.3.dev9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rats-pipelines
-Version: 0.1.3.dev8
+Version: 0.1.3.dev9
 Summary: Rats Pipelines
 Home-page: https://github.com/microsoft/rats/
 License: MIT
 Keywords: pipelines,machine learning,research
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `rats_pipelines-0.1.3.dev8.dist-info/RECORD` & `rats_pipelines-0.1.3.dev9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -71,11 +71,11 @@
 rats/services/_scopes.py,sha256=UJKK6XZsuQN0ukTKmpFNjoXsGKNS2eaZ6SUu09HLdOU,2350
 rats/services/_service_container.py,sha256=WeaXkbWRn7rbJTUeI8asTJr57oR-f_WJxitLxgZzZyY,3798
 rats/services/_service_factory.py,sha256=T2-Egvl1WLVrLpH9qxWesFV0uzQj242MPZCGq9u4Ynk,2587
 rats/services/_service_managers.py,sha256=EvyTyX6_OwN9eBoeb9FD7JHOyHHIe0il-bbx8d_l_6U,3289
 rats/services/_services.py,sha256=jQctaj9nqes1_S42PcnJzRRcNhigoyqpTmO_mquq1Uc,598
 rats/services/_typed_containers.py,sha256=xRBlJ5vgeeoJGa1wiYDj3uUdxVmal_3cNzYMcIyrpOA,1409
 rats/services/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rats_pipelines-0.1.3.dev8.dist-info/METADATA,sha256=Gq2VstMzkogMWMhsxi9QAyaU1mv4xr7NLMNRX0GlixI,774
-rats_pipelines-0.1.3.dev8.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-rats_pipelines-0.1.3.dev8.dist-info/entry_points.txt,sha256=NY28IUb7dnNl0HFwzCGV2o9Uivyh278m0NpQRVDIgRQ,85
-rats_pipelines-0.1.3.dev8.dist-info/RECORD,,
+rats_pipelines-0.1.3.dev9.dist-info/METADATA,sha256=X6Yw9OpW0guZGHa8lRZZA1VaABLcfg8kjEygaRX8pnU,774
+rats_pipelines-0.1.3.dev9.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+rats_pipelines-0.1.3.dev9.dist-info/entry_points.txt,sha256=NY28IUb7dnNl0HFwzCGV2o9Uivyh278m0NpQRVDIgRQ,85
+rats_pipelines-0.1.3.dev9.dist-info/RECORD,,
```

