# Comparing `tmp/pre5g-3.9.tar.gz` & `tmp/pre5g-4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-3.9.tar", last modified: Tue Apr 16 06:31:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

