# Comparing `tmp/cpi_tools-0.3.19.tar.gz` & `tmp/cpi_tools-0.3.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpi_tools-0.3.19.tar", last modified: Mon Apr  8 22:14:53 2024, max compression
+gzip compressed data, was "cpi_tools-0.3.24.tar", last modified: Thu May  2 18:38:23 2024, max compression
```

## Comparing `cpi_tools-0.3.19.tar` & `cpi_tools-0.3.24.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 22:14:53.849841 cpi_tools-0.3.19/
--rw-rw-rw-   0        0        0     1074 2023-01-26 16:53:27.000000 cpi_tools-0.3.19/LICENSE
--rw-rw-rw-   0        0        0        0 2023-01-27 16:40:16.000000 cpi_tools-0.3.19/MANIFEST.in
--rw-rw-rw-   0        0        0      957 2024-04-08 22:14:53.841828 cpi_tools-0.3.19/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-01-27 16:58:15.000000 cpi_tools-0.3.19/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 22:14:53.809827 cpi_tools-0.3.19/cpi_tools/
--rw-rw-rw-   0        0        0        0 2023-01-26 16:53:26.000000 cpi_tools-0.3.19/cpi_tools/__init__.py
--rw-rw-rw-   0        0        0     2375 2023-01-27 16:56:14.000000 cpi_tools-0.3.19/cpi_tools/aws_tools.py
--rw-rw-rw-   0        0        0     5403 2023-09-18 18:36:57.000000 cpi_tools-0.3.19/cpi_tools/cpi_validation.py
--rw-rw-rw-   0        0        0     9747 2024-04-08 21:06:40.000000 cpi_tools-0.3.19/cpi_tools/fuzzy_matching_cpi.py
--rw-rw-rw-   0        0        0    16524 2024-04-08 21:06:40.000000 cpi_tools-0.3.19/cpi_tools/tracking_processing_tools.py
--rw-rw-rw-   0        0        0    15367 2024-04-08 22:14:01.000000 cpi_tools-0.3.19/cpi_tools/tracking_processing_tools_v2.py
-drwxrwxrwx   0        0        0        0 2024-04-08 22:14:53.833839 cpi_tools-0.3.19/cpi_tools.egg-info/
--rw-rw-rw-   0        0        0      957 2024-04-08 22:14:53.000000 cpi_tools-0.3.19/cpi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-04-08 22:14:53.000000 cpi_tools-0.3.19/cpi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 22:14:53.000000 cpi_tools-0.3.19/cpi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-08 22:14:53.000000 cpi_tools-0.3.19/cpi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-01-27 16:46:45.000000 cpi_tools-0.3.19/pyproject.toml
--rw-rw-rw-   0        0        0      582 2024-04-08 22:14:53.849841 cpi_tools-0.3.19/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 18:38:23.015372 cpi_tools-0.3.24/
+-rw-rw-rw-   0        0        0     1074 2023-01-26 16:53:27.000000 cpi_tools-0.3.24/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-01-27 16:40:16.000000 cpi_tools-0.3.24/MANIFEST.in
+-rw-rw-rw-   0        0        0      957 2024-05-02 18:38:23.015372 cpi_tools-0.3.24/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-01-27 16:58:15.000000 cpi_tools-0.3.24/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 18:38:22.983370 cpi_tools-0.3.24/cpi_tools/
+-rw-rw-rw-   0        0        0        0 2023-01-26 16:53:26.000000 cpi_tools-0.3.24/cpi_tools/__init__.py
+-rw-rw-rw-   0        0        0     3418 2024-05-02 18:36:58.000000 cpi_tools-0.3.24/cpi_tools/aws_tools.py
+-rw-rw-rw-   0        0        0     5403 2023-09-18 18:36:57.000000 cpi_tools-0.3.24/cpi_tools/cpi_validation.py
+-rw-rw-rw-   0        0        0     9747 2024-04-08 21:06:40.000000 cpi_tools-0.3.24/cpi_tools/fuzzy_matching_cpi.py
+-rw-rw-rw-   0        0        0    16524 2024-04-08 21:06:40.000000 cpi_tools-0.3.24/cpi_tools/tracking_processing_tools.py
+-rw-rw-rw-   0        0        0    15367 2024-04-08 22:14:01.000000 cpi_tools-0.3.24/cpi_tools/tracking_processing_tools_v2.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:38:23.007376 cpi_tools-0.3.24/cpi_tools.egg-info/
+-rw-rw-rw-   0        0        0      957 2024-05-02 18:38:22.000000 cpi_tools-0.3.24/cpi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-05-02 18:38:22.000000 cpi_tools-0.3.24/cpi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 18:38:22.000000 cpi_tools-0.3.24/cpi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-02 18:38:22.000000 cpi_tools-0.3.24/cpi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-01-27 16:46:45.000000 cpi_tools-0.3.24/pyproject.toml
+-rw-rw-rw-   0        0        0      582 2024-05-02 18:38:23.023375 cpi_tools-0.3.24/setup.cfg
```

### Comparing `cpi_tools-0.3.19/LICENSE` & `cpi_tools-0.3.24/LICENSE`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.3.19/PKG-INFO` & `cpi_tools-0.3.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpi_tools
-Version: 0.3.19
+Version: 0.3.24
 Summary: Repository of functions used across CPI
 Home-page: https://github.com/climatepolicydata/cpi_tools
 Author: Jake Connolly, Nikita Marini
 Author-email: datascience@cpiglobal.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cpi_tools-0.3.19/cpi_tools/cpi_validation.py` & `cpi_tools-0.3.24/cpi_tools/cpi_validation.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.3.19/cpi_tools/fuzzy_matching_cpi.py` & `cpi_tools-0.3.24/cpi_tools/fuzzy_matching_cpi.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.3.19/cpi_tools/tracking_processing_tools.py` & `cpi_tools-0.3.24/cpi_tools/tracking_processing_tools.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.3.19/cpi_tools/tracking_processing_tools_v2.py` & `cpi_tools-0.3.24/cpi_tools/tracking_processing_tools_v2.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.3.19/cpi_tools.egg-info/PKG-INFO` & `cpi_tools-0.3.24/cpi_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpi_tools
-Version: 0.3.19
+Version: 0.3.24
 Summary: Repository of functions used across CPI
 Home-page: https://github.com/climatepolicydata/cpi_tools
 Author: Jake Connolly, Nikita Marini
 Author-email: datascience@cpiglobal.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cpi_tools-0.3.19/setup.cfg` & `cpi_tools-0.3.24/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 7069 5f74 6f6f 6c73 0d0a 7665   = cpi_tools..ve
-00000020: 7273 696f 6e20 3d20 302e 332e 3139 0d0a  rsion = 0.3.19..
+00000020: 7273 696f 6e20 3d20 302e 332e 3234 0d0a  rsion = 0.3.24..
 00000030: 6175 7468 6f72 203d 204a 616b 6520 436f  author = Jake Co
 00000040: 6e6e 6f6c 6c79 2c20 4e69 6b69 7461 204d  nnolly, Nikita M
 00000050: 6172 696e 690d 0a61 7574 686f 725f 656d  arini..author_em
 00000060: 6169 6c20 3d20 6461 7461 7363 6965 6e63  ail = datascienc
 00000070: 6540 6370 6967 6c6f 6261 6c2e 6f72 670d  e@cpiglobal.org.
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2052  .description = R
 00000090: 6570 6f73 6974 6f72 7920 6f66 2066 756e  epository of fun
```

