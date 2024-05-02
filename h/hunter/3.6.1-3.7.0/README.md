# Comparing `tmp/hunter-3.6.1.tar.gz` & `tmp/hunter-3.7.0-pp310.pp38.pp39-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hunter-3.6.1.tar", last modified: Wed Apr 26 09:56:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

