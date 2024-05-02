# Comparing `tmp/qc_parser-0.0.8.tar.gz` & `tmp/qc_parser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qc_parser-0.0.8.tar", max compression
+gzip compressed data, was "qc_parser-0.0.9.tar", max compression
```

## Comparing `qc_parser-0.0.8.tar` & `qc_parser-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1083 2023-10-17 16:44:02.877270 qc_parser-0.0.8/LICENSE
--rw-r--r--   0        0        0     1884 2023-12-06 14:39:59.326425 qc_parser-0.0.8/README.md
--rw-r--r--   0        0        0     1221 2024-01-11 19:58:56.214198 qc_parser-0.0.8/pyproject.toml
--rwxr-xr-x   0        0        0     6832 2023-12-13 15:39:53.992898 qc_parser-0.0.8/src/MetricsParser.py
--rwxr-xr-x   0        0        0     1688 2023-12-06 14:39:50.750645 qc_parser-0.0.8/src/QMGeneric.py
--rw-r--r--   0        0        0        0 2023-10-17 19:48:48.025273 qc_parser-0.0.8/src/__init__.py
--rwxr-xr-x   0        0        0    26523 2024-01-11 19:58:56.215749 qc_parser-0.0.8/src/metrics_to_extract.py
--rw-r--r--   0        0        0     2687 2023-12-06 14:39:50.752394 qc_parser-0.0.8/src/parse_qc.py
--rw-r--r--   0        0        0     2963 1970-01-01 00:00:00.000000 qc_parser-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-10-17 16:44:02.877270 qc_parser-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1884 2023-12-06 14:39:59.326425 qc_parser-0.0.9/README.md
+-rw-r--r--   0        0        0     1220 2024-01-25 19:17:06.216255 qc_parser-0.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0     7163 2024-01-25 19:17:06.217354 qc_parser-0.0.9/src/MetricsParser.py
+-rwxr-xr-x   0        0        0     1688 2023-12-06 14:39:50.750645 qc_parser-0.0.9/src/QMGeneric.py
+-rw-r--r--   0        0        0        0 2023-10-17 19:48:48.025273 qc_parser-0.0.9/src/__init__.py
+-rwxr-xr-x   0        0        0    26523 2024-01-11 19:58:56.215749 qc_parser-0.0.9/src/metrics_to_extract.py
+-rw-r--r--   0        0        0     2687 2023-12-06 14:39:50.752394 qc_parser-0.0.9/src/parse_qc.py
+-rw-r--r--   0        0        0     2963 1970-01-01 00:00:00.000000 qc_parser-0.0.9/PKG-INFO
```

### Comparing `qc_parser-0.0.8/LICENSE` & `qc_parser-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qc_parser-0.0.8/README.md` & `qc_parser-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `qc_parser-0.0.8/pyproject.toml` & `qc_parser-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qc-parser"
-version = "0.0.8"
+version = "0.0.9"
 description = "Parses outputs of different QC tools and unifies them for the SMaHT portal"
 authors = ["Alexander Veit <alexander_veit@hms.harvard.edu>", "Michele Berselli <berselli.michele@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/smaht-dac/qc-parser"
 repository = "https://github.com/smaht-dac/qc-parser"
 packages = [
@@ -35,8 +35,7 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 parse-qc = "src.parse_qc:parse_qc"
-
```

### Comparing `qc_parser-0.0.8/src/MetricsParser.py` & `qc_parser-0.0.9/src/MetricsParser.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,21 +84,30 @@
 
     def parse_rnaseqqc(self) -> List[QMValue]:
         # TODO
         return
 
     def parse_picard_CollectAlignmentSummaryMetrics(self) -> List[QMValue]:
         qm_values = []
-        header, pair = [], []
+        header, pair, unpair = [], [], []
         with open(self.path) as fi:
             for line in fi:
                 if line.startswith('CATEGORY'):
                     header = line.rstrip().split('\t')
                 elif line.startswith('PAIR'):
                     pair = line.rstrip().split('\t')
+                elif line.startswith('UNPAIRED'):
+                    unpair = line.rstrip().split('\t')
+
+        # Check for both PAIR and UNPAIRED -> ERROR
+        if pair and unpair:
+            sys.exit(
+                f"Paired-end BAM file contains unpaired reads")
+        elif unpair:
+            pair = unpair
 
         for i, field in enumerate(header):
             if field in metrics[PICARD_COLLECT_ALIGNMENT_SUMMARY_METRICS]:
                 m = metrics[PICARD_COLLECT_ALIGNMENT_SUMMARY_METRICS][field]
                 value_cast = self.safe_cast(pair[i], m["type"])
                 if value_cast == None:
                     continue
```

### Comparing `qc_parser-0.0.8/src/QMGeneric.py` & `qc_parser-0.0.9/src/QMGeneric.py`

 * *Files identical despite different names*

### Comparing `qc_parser-0.0.8/src/metrics_to_extract.py` & `qc_parser-0.0.9/src/metrics_to_extract.py`

 * *Files identical despite different names*

### Comparing `qc_parser-0.0.8/src/parse_qc.py` & `qc_parser-0.0.9/src/parse_qc.py`

 * *Files identical despite different names*

### Comparing `qc_parser-0.0.8/PKG-INFO` & `qc_parser-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qc-parser
-Version: 0.0.8
+Version: 0.0.9
 Summary: Parses outputs of different QC tools and unifies them for the SMaHT portal
 Home-page: https://github.com/smaht-dac/qc-parser
 License: MIT
 Author: Alexander Veit
 Author-email: alexander_veit@hms.harvard.edu
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

