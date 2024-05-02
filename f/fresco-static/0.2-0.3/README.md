# Comparing `tmp/fresco-static-0.2.tar.gz` & `tmp/fresco_static-0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fresco-static-0.2.tar", last modified: Wed Aug  1 11:32:28 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

