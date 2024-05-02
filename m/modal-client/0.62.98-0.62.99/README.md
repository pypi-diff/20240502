# Comparing `tmp/modal_client-0.62.98-py3-none-any.whl.zip` & `tmp/modal_client-0.62.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1270 bytes, number of entries: 4
--rw-r--r--  2.0 unx      527 b- defN 24-Apr-21 19:40 modal_client-0.62.98.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 19:40 modal_client-0.62.98.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-21 19:40 modal_client-0.62.98.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      324 b- defN 24-Apr-21 19:40 modal_client-0.62.98.dist-info/RECORD
-4 files, 944 bytes uncompressed, 632 bytes compressed:  33.1%
+Zip file size: 1272 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      527 b- defN 24-Apr-22 08:13 modal_client-0.62.99.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 08:13 modal_client-0.62.99.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-22 08:13 modal_client-0.62.99.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      324 b- defN 24-Apr-22 08:13 modal_client-0.62.99.dist-info/RECORD
+4 files, 944 bytes uncompressed, 634 bytes compressed:  32.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: modal_client-0.62.98.dist-info/METADATA
+Filename: modal_client-0.62.99.dist-info/METADATA
 Comment: 
 
-Filename: modal_client-0.62.98.dist-info/WHEEL
+Filename: modal_client-0.62.99.dist-info/WHEEL
 Comment: 
 
-Filename: modal_client-0.62.98.dist-info/top_level.txt
+Filename: modal_client-0.62.99.dist-info/top_level.txt
 Comment: 
 
-Filename: modal_client-0.62.98.dist-info/RECORD
+Filename: modal_client-0.62.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `modal_client-0.62.98.dist-info/METADATA` & `modal_client-0.62.99.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: modal-client
-Version: 0.62.98
+Version: 0.62.99
 Summary: Legacy name for the Modal client
 Author: Modal Labs
 Author-email: support@modal.com
 Project-URL: Homepage, https://modal.com
 Description-Content-Type: text/markdown
-Requires-Dist: modal (==0.62.98)
+Requires-Dist: modal (==0.62.99)
 
 This is a legacy compatibility package that just requires the `modal` client library.
 In versions before 0.51, the official name of the client library was called `modal-client`.
 We have renamed it to `modal`, but this library is kept updated for compatibility.
```

