# Comparing `tmp/qceltis-0.1.1-py3-none-any.whl.zip` & `tmp/qceltis-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 41183 bytes, number of entries: 13
+Zip file size: 41190 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-11 21:56 qceltis/__init__.py
 -rw-rw-rw-  2.0 fat    25014 b- defN 24-Apr-30 18:10 qceltis/main.py
 -rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-11 21:56 qceltis/mod/__init__.py
 -rw-rw-rw-  2.0 fat    18150 b- defN 24-Apr-11 18:46 qceltis/mod/general_functions.py
 -rw-rw-rw-  2.0 fat    67355 b- defN 24-Apr-29 07:56 qceltis/mod/idbased_metrics.py
 -rw-rw-rw-  2.0 fat    33089 b- defN 24-Apr-29 07:56 qceltis/mod/mzml_extract.py
 -rw-rw-rw-  2.0 fat    26499 b- defN 24-Apr-11 18:46 qceltis/templates/report_template.html
--rw-rw-rw-  2.0 fat     1069 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    31127 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       46 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1069 b- defN 24-Apr-30 18:28 qceltis-0.1.1.dist-info/RECORD
-13 files, 203552 bytes uncompressed, 39399 bytes compressed:  80.6%
+-rw-rw-rw-  2.0 fat     1069 b- defN 24-May-01 22:50 qceltis-0.1.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    31127 b- defN 24-May-01 22:50 qceltis-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-01 22:50 qceltis-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       46 b- defN 24-May-01 22:50 qceltis-0.1.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-01 22:50 qceltis-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1069 b- defN 24-May-01 22:50 qceltis-0.1.2.dist-info/RECORD
+13 files, 203552 bytes uncompressed, 39406 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: qceltis/mod/mzml_extract.py
 Comment: 
 
 Filename: qceltis/templates/report_template.html
 Comment: 
 
-Filename: qceltis-0.1.1.dist-info/LICENSE.txt
+Filename: qceltis-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: qceltis-0.1.1.dist-info/METADATA
+Filename: qceltis-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: qceltis-0.1.1.dist-info/WHEEL
+Filename: qceltis-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: qceltis-0.1.1.dist-info/entry_points.txt
+Filename: qceltis-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: qceltis-0.1.1.dist-info/top_level.txt
+Filename: qceltis-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: qceltis-0.1.1.dist-info/RECORD
+Filename: qceltis-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `qceltis-0.1.1.dist-info/LICENSE.txt` & `qceltis-0.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `qceltis-0.1.1.dist-info/METADATA` & `qceltis-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qceltis
-Version: 0.1.1
+Version: 0.1.2
 Summary: Quality Control Package for DIA Proteomics
 Home-page: https://github.com/csmc-vaneykjlab/QCeltis
 Author: Manasa Vegesna
 Author-email: vmanasa1129@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: pandas >=2.0.1
+Requires-Dist: pandas ==2.0.1
 Requires-Dist: numpy >=1.24.3
 Requires-Dist: xlsxwriter >=3.2.0
 Requires-Dist: plotly >=5.13.0
 Requires-Dist: jinja2 >=3.1.3
 Requires-Dist: scipy >=1.10.1
 Requires-Dist: scikit-learn >=1.2.2
 Requires-Dist: pymzml >=2.5.9
```

## Comparing `qceltis-0.1.1.dist-info/RECORD` & `qceltis-0.1.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 qceltis/__init__.py,sha256=aOtkInm-Zzu1IDz5k1kt59tFbqSITr7WE9q0x0BQezg,17
 qceltis/main.py,sha256=PYrtjQsCR2v7Mh2aOs_9oXefIKRI_z10lWUfrFU9XgI,25014
 qceltis/mod/__init__.py,sha256=aOtkInm-Zzu1IDz5k1kt59tFbqSITr7WE9q0x0BQezg,17
 qceltis/mod/general_functions.py,sha256=DIhUINDNVORqBclvAmrNVVZCzMJO0FkUo47hdZ1xrX0,18150
 qceltis/mod/idbased_metrics.py,sha256=D9pPIkV4-UCMAPs5BY0iF3dgBdNV8UZiy-Pd_YbImK8,67355
 qceltis/mod/mzml_extract.py,sha256=itlU0mgCWJOxhlbSVWUcYjXghToKLeqVzMCFpuXcQto,33089
 qceltis/templates/report_template.html,sha256=X87BwMY_dd8JtWBTTStgDQAa5_kodEIAlC71QW5XUAg,26499
-qceltis-0.1.1.dist-info/LICENSE.txt,sha256=KRE8-Cn8i6Zzmawykhw-z-DiQVznNGV1T7HTTJCDE14,1069
-qceltis-0.1.1.dist-info/METADATA,sha256=x0lY2kWBqy7B6VJGXerjPx1M07BFnzghfl_2KQJAJcw,31127
-qceltis-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-qceltis-0.1.1.dist-info/entry_points.txt,sha256=7OGUACvioZACakR5HIEQ5PDJvsXz5FFGqe7gjNFaHwg,46
-qceltis-0.1.1.dist-info/top_level.txt,sha256=aKJhPLleA6JhwhvihRVD4gR-ZjadhBouFxeAR980S00,8
-qceltis-0.1.1.dist-info/RECORD,,
+qceltis-0.1.2.dist-info/LICENSE.txt,sha256=KRE8-Cn8i6Zzmawykhw-z-DiQVznNGV1T7HTTJCDE14,1069
+qceltis-0.1.2.dist-info/METADATA,sha256=qivwJfxWGyHncxCPey4azw1PgHPUOMaE4_pH1Bkzv-I,31127
+qceltis-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+qceltis-0.1.2.dist-info/entry_points.txt,sha256=7OGUACvioZACakR5HIEQ5PDJvsXz5FFGqe7gjNFaHwg,46
+qceltis-0.1.2.dist-info/top_level.txt,sha256=aKJhPLleA6JhwhvihRVD4gR-ZjadhBouFxeAR980S00,8
+qceltis-0.1.2.dist-info/RECORD,,
```

