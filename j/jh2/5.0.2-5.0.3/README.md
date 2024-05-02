# Comparing `tmp/jh2-5.0.2.tar.gz` & `tmp/jh2-5.0.3-pp37-pypy37_pp73-manylinux_2_17_ppc64.manylinux2014_ppc64.whl.zip`

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

