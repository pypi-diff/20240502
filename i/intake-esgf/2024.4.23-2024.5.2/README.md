# Comparing `tmp/intake_esgf-2024.4.23.tar.gz` & `tmp/intake_esgf-2024.5.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake_esgf-2024.4.23.tar", last modified: Tue Apr 23 13:46:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

