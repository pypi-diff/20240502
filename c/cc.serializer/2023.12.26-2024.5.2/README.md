# Comparing `tmp/cc.serializer-2023.12.26.tar.gz` & `tmp/cc.serializer-2024.5.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc.serializer-2023.12.26.tar", last modified: Fri Dec 29 08:36:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

