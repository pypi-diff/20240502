# Comparing `tmp/cc.udp-2024.1.23.tar.gz` & `tmp/cc.udp-2024.5.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc.udp-2024.1.23.tar", last modified: Tue Jan 23 22:20:06 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

