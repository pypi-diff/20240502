# Comparing `tmp/oso-cloud-1.4.0.dev0.tar.gz` & `tmp/oso_cloud-1.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oso-cloud-1.4.0.dev0.tar", last modified: Wed Apr 10 03:31:43 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

