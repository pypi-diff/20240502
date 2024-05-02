# Comparing `tmp/pygorpho-1.0.0.tar.gz` & `tmp/pygorpho-1.0.1.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pygorpho-1.0.0.tar", last modified: Sun Dec 20 20:28:35 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

