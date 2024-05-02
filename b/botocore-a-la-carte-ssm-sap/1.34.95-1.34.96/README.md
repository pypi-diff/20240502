# Comparing `tmp/botocore-a-la-carte-ssm-sap-1.34.95.tar.gz` & `tmp/botocore_a_la_carte_ssm_sap-1.34.96-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ssm-sap-1.34.95.tar", last modified: Wed May  1 01:06:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
