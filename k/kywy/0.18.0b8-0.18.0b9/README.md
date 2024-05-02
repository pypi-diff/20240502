# Comparing `tmp/kywy-0.18.0b8-py3-none-any.whl.zip` & `tmp/kywy-0.18.0b9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 61494 bytes, number of entries: 50
+Zip file size: 61496 bytes, number of entries: 50
 -rw-r--r--  2.0 unx     6148 b- defN 24-Jan-12 10:00 .DS_Store
 -rw-r--r--  2.0 unx     6148 b- defN 24-Jan-12 10:00 kywy/.DS_Store
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 09:57 kywy/client/__init__.py
 -rw-r--r--  2.0 unx     7834 b- defN 24-Feb-21 00:35 kywy/client/benchmark.py
 -rw-r--r--  2.0 unx     7033 b- defN 23-Dec-06 17:20 kywy/client/benchmark_v2.py
 -rw-r--r--  2.0 unx     1024 b- defN 24-Mar-29 16:17 kywy/client/chat.py
 -rw-r--r--  2.0 unx    28964 b- defN 24-Mar-29 16:17 kywy/client/commands.py
@@ -41,12 +41,12 @@
 -rw-r--r--  2.0 unx     2549 b- defN 23-Dec-06 17:20 kywy/server/kawa_directory_manager.py
 -rw-r--r--  2.0 unx     1114 b- defN 23-Nov-24 14:24 kywy/server/kawa_error_manager.py
 -rw-r--r--  2.0 unx     7047 b- defN 24-Jan-22 02:43 kywy/server/kawa_flight_server.py
 -rw-r--r--  2.0 unx     2940 b- defN 23-Nov-24 14:24 kywy/server/kawa_jobs_manager.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Mar-07 22:07 kywy/server/kawa_script_manager.py
 -rw-r--r--  2.0 unx       93 b- defN 23-Jun-26 16:14 kywy/server/server.py
 -rw-r--r--  2.0 unx     2302 b- defN 23-Dec-06 17:20 kywy/server/start_flight_server.py
--rw-r--r--  2.0 unx     1117 b- defN 24-Mar-29 17:27 kywy-0.18.0b8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-29 17:27 kywy-0.18.0b8.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Mar-29 17:27 kywy-0.18.0b8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4162 b- defN 24-Mar-29 17:27 kywy-0.18.0b8.dist-info/RECORD
-50 files, 226583 bytes uncompressed, 54888 bytes compressed:  75.8%
+-rw-r--r--  2.0 unx     1117 b- defN 24-Mar-30 15:02 kywy-0.18.0b9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-30 15:02 kywy-0.18.0b9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Mar-30 15:02 kywy-0.18.0b9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4162 b- defN 24-Mar-30 15:02 kywy-0.18.0b9.dist-info/RECORD
+50 files, 226583 bytes uncompressed, 54890 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -132,20 +132,20 @@
 
 Filename: kywy/server/server.py
 Comment: 
 
 Filename: kywy/server/start_flight_server.py
 Comment: 
 
-Filename: kywy-0.18.0b8.dist-info/METADATA
+Filename: kywy-0.18.0b9.dist-info/METADATA
 Comment: 
 
-Filename: kywy-0.18.0b8.dist-info/WHEEL
+Filename: kywy-0.18.0b9.dist-info/WHEEL
 Comment: 
 
-Filename: kywy-0.18.0b8.dist-info/top_level.txt
+Filename: kywy-0.18.0b9.dist-info/top_level.txt
 Comment: 
 
-Filename: kywy-0.18.0b8.dist-info/RECORD
+Filename: kywy-0.18.0b9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `kywy-0.18.0b8.dist-info/METADATA` & `kywy-0.18.0b9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kywy
-Version: 0.18.0b8
+Version: 0.18.0b9
 Summary: Python client for Kawa - https://docs.kawa.ai
 Home-page: UNKNOWN
 Author: Kawa Analytics
 Author-email: emmmanuel@kawa.ai
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `kywy-0.18.0b8.dist-info/RECORD` & `kywy-0.18.0b9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -40,11 +40,11 @@
 kywy/server/kawa_directory_manager.py,sha256=jSQFpK-b2I2zzm9ihQ2JiEDKCxfpp6BUc7FDXNwcrG4,2549
 kywy/server/kawa_error_manager.py,sha256=7iNl_fQ3uovSNbnD5q-DA1RdOKqsinejhdq-I7eUpDc,1114
 kywy/server/kawa_flight_server.py,sha256=khEUuXRGkzYzmX8L8blralyLwHeiATcgj09fsAZ8uQI,7047
 kywy/server/kawa_jobs_manager.py,sha256=AbOGxkGcUnfobeyIaZL1-aWi4ahpuHhw6FPIC7yUxio,2940
 kywy/server/kawa_script_manager.py,sha256=3cqy2AXGrWWkFWp8YF4h3nspZAKwTDzMu-_cDMzGTvU,4195
 kywy/server/server.py,sha256=BUsmqvFYHA26IHX2HTJ3mg9_XPLLNRfBCUmeLgN5OyA,93
 kywy/server/start_flight_server.py,sha256=KSDJ36B_kH183V4LGLV1yV58DvSCbPap4h_fCvnycvY,2302
-kywy-0.18.0b8.dist-info/METADATA,sha256=vbpES9sEQO9YrznP_dJ82GhF_YaDbLKCbjyc6lfLDZg,1117
-kywy-0.18.0b8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-kywy-0.18.0b8.dist-info/top_level.txt,sha256=l2OblXFizKIUlLW71gnkiR2oTqdGosiS303jGGQmgNE,5
-kywy-0.18.0b8.dist-info/RECORD,,
+kywy-0.18.0b9.dist-info/METADATA,sha256=7o8NclkDByzu-m1yyiYGAKntlcyJh5wRW3d3OXMc6bQ,1117
+kywy-0.18.0b9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+kywy-0.18.0b9.dist-info/top_level.txt,sha256=l2OblXFizKIUlLW71gnkiR2oTqdGosiS303jGGQmgNE,5
+kywy-0.18.0b9.dist-info/RECORD,,
```

