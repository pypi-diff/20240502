# Comparing `tmp/emmett_crypto-0.5.1.tar.gz` & `tmp/emmett_crypto-0.6.0-cp312-cp312-macosx_10_12_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

