# Comparing `tmp/xlextract-0.1.5.tar.gz` & `tmp/xlextract-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlextract-0.1.5.tar", max compression
+gzip compressed data, was "xlextract-0.1.6.tar", max compression
```

## Comparing `xlextract-0.1.5.tar` & `xlextract-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3945 2024-05-02 00:47:30.904698 xlextract-0.1.5/README.md
--rw-r--r--   0        0        0      392 2024-05-02 00:49:51.815971 xlextract-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4424 2024-05-02 00:23:15.412088 xlextract-0.1.5/xlextract/__init__.py
--rw-r--r--   0        0        0     1884 2024-05-01 18:06:16.984157 xlextract-0.1.5/xlextract/classes.py
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 xlextract-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3990 2024-05-02 00:54:15.458342 xlextract-0.1.6/README.md
+-rw-r--r--   0        0        0      392 2024-05-02 00:55:03.108750 xlextract-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4424 2024-05-02 00:23:15.412088 xlextract-0.1.6/xlextract/__init__.py
+-rw-r--r--   0        0        0     1884 2024-05-01 18:06:16.984157 xlextract-0.1.6/xlextract/classes.py
+-rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 xlextract-0.1.6/PKG-INFO
```

### Comparing `xlextract-0.1.5/README.md` & `xlextract-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from xlextract import XLExtract
 
 vrf_table = XLExtract("design_document.xlsx", "Tenants", "VRF NAME")
 ```
 
 # Table Lookup Example
 Assuming we have an Excel spreadsheet with a "Tenants" tab that contains a table that looks like this:  
-![Sample Excel Table](./art/ACI_VRF_Table.jpg?raw=true)
+![Sample Excel Table](https://github.com/aj-cruz/xlextract/blob/main/art/ACI_VRF_Table.jpg?raw=true)
 If we then do this in our Python code:
 ```python
 vrf_table.TLookup()
 
 print(json.dumps(vrf_table.value, indent = 4))
 ```
```

### Comparing `xlextract-0.1.5/xlextract/__init__.py` & `xlextract-0.1.6/xlextract/__init__.py`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.5/xlextract/classes.py` & `xlextract-0.1.6/xlextract/classes.py`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.5/PKG-INFO` & `xlextract-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlextract
-Version: 0.1.5
+Version: 0.1.6
 Summary: Extract data from Excel files
 Author: AJ Cruz
 Author-email: aj.cruz@computacenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -53,15 +53,15 @@
 from xlextract import XLExtract
 
 vrf_table = XLExtract("design_document.xlsx", "Tenants", "VRF NAME")
 ```
 
 # Table Lookup Example
 Assuming we have an Excel spreadsheet with a "Tenants" tab that contains a table that looks like this:  
-![Sample Excel Table](./art/ACI_VRF_Table.jpg?raw=true)
+![Sample Excel Table](https://github.com/aj-cruz/xlextract/blob/main/art/ACI_VRF_Table.jpg?raw=true)
 If we then do this in our Python code:
 ```python
 vrf_table.TLookup()
 
 print(json.dumps(vrf_table.value, indent = 4))
 ```
```

