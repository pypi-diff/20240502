# Comparing `tmp/camel-kenlm-2023.3.17.2.tar.gz` & `tmp/camel-kenlm-2024.5.2.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camel-kenlm-2023.3.17.2.tar", last modified: Fri Mar 17 11:38:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

