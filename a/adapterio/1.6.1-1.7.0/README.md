# Comparing `tmp/adapterio-1.6.1.tar.gz` & `tmp/adapterio-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapterio-1.6.1.tar", last modified: Tue Jun 27 02:03:53 2023, max compression
+gzip compressed data, was "adapterio-1.7.0.tar", last modified: Thu May  2 20:33:55 2024, max compression
```

## Comparing `adapterio-1.6.1.tar` & `adapterio-1.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-06-27 02:03:53.711484 adapterio-1.6.1/
--rw-r--r--   0 mgrahovac   (502) staff       (20)     1653 2023-06-27 02:03:53.711042 adapterio-1.6.1/PKG-INFO
--rw-r--r--   0 mgrahovac   (502) staff       (20)     7012 2023-05-05 11:27:35.000000 adapterio-1.6.1/README.md
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-06-27 02:03:53.705217 adapterio-1.6.1/adapter/
--rw-r--r--   0 mgrahovac   (502) staff       (20)      120 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/Secret_example.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)      168 2023-06-27 02:03:37.000000 adapterio-1.6.1/adapter/__init__.py
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-06-27 02:03:53.707908 adapterio-1.6.1/adapter/comm/
--rw-r--r--   0 mgrahovac   (502) staff       (20)        0 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/comm/__init__.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)    25380 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/comm/excel.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)     5015 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/comm/sql.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)     6547 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/comm/tools.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)    29220 2023-06-27 02:03:37.000000 adapterio-1.6.1/adapter/i_o.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)      632 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/label_map.py
--rw-r--r--   0 mgrahovac   (502) staff       (20)    14700 2023-05-05 11:27:35.000000 adapterio-1.6.1/adapter/to_python.py
-drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2023-06-27 02:03:53.710295 adapterio-1.6.1/adapterio.egg-info/
--rw-r--r--   0 mgrahovac   (502) staff       (20)     1653 2023-06-27 02:03:53.000000 adapterio-1.6.1/adapterio.egg-info/PKG-INFO
--rw-r--r--   0 mgrahovac   (502) staff       (20)      389 2023-06-27 02:03:53.000000 adapterio-1.6.1/adapterio.egg-info/SOURCES.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)        1 2023-06-27 02:03:53.000000 adapterio-1.6.1/adapterio.egg-info/dependency_links.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)       88 2023-06-27 02:03:53.000000 adapterio-1.6.1/adapterio.egg-info/requires.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)        8 2023-06-27 02:03:53.000000 adapterio-1.6.1/adapterio.egg-info/top_level.txt
--rw-r--r--   0 mgrahovac   (502) staff       (20)      103 2023-05-05 11:27:35.000000 adapterio-1.6.1/pyproject.toml
--rw-r--r--   0 mgrahovac   (502) staff       (20)       38 2023-06-27 02:03:53.711663 adapterio-1.6.1/setup.cfg
--rw-r--r--   0 mgrahovac   (502) staff       (20)     2779 2023-05-05 11:27:35.000000 adapterio-1.6.1/setup.py
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2024-05-02 20:33:55.443742 adapterio-1.7.0/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     1815 2024-05-02 20:33:55.443110 adapterio-1.7.0/PKG-INFO
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     7012 2023-05-05 11:27:35.000000 adapterio-1.7.0/README.md
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2024-05-02 20:33:55.437013 adapterio-1.7.0/adapter/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      120 2023-05-05 11:27:35.000000 adapterio-1.7.0/adapter/Secret_example.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      168 2024-05-02 20:31:35.000000 adapterio-1.7.0/adapter/__init__.py
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2024-05-02 20:33:55.439741 adapterio-1.7.0/adapter/comm/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)        0 2023-05-05 11:27:35.000000 adapterio-1.7.0/adapter/comm/__init__.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)    25380 2023-05-05 11:27:35.000000 adapterio-1.7.0/adapter/comm/excel.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     5015 2023-05-05 11:27:35.000000 adapterio-1.7.0/adapter/comm/sql.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     5894 2024-05-02 20:31:35.000000 adapterio-1.7.0/adapter/comm/tools.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)    29220 2023-06-27 02:03:37.000000 adapterio-1.7.0/adapter/i_o.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      632 2023-05-05 11:27:35.000000 adapterio-1.7.0/adapter/label_map.py
+-rw-r--r--   0 mgrahovac   (502) staff       (20)    14664 2024-05-02 20:31:35.000000 adapterio-1.7.0/adapter/to_python.py
+drwxr-xr-x   0 mgrahovac   (502) staff       (20)        0 2024-05-02 20:33:55.442463 adapterio-1.7.0/adapterio.egg-info/
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     1815 2024-05-02 20:33:55.000000 adapterio-1.7.0/adapterio.egg-info/PKG-INFO
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      389 2024-05-02 20:33:55.000000 adapterio-1.7.0/adapterio.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)        1 2024-05-02 20:33:55.000000 adapterio-1.7.0/adapterio.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)       87 2024-05-02 20:33:55.000000 adapterio-1.7.0/adapterio.egg-info/requires.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)        8 2024-05-02 20:33:55.000000 adapterio-1.7.0/adapterio.egg-info/top_level.txt
+-rw-r--r--   0 mgrahovac   (502) staff       (20)      103 2023-05-05 11:27:35.000000 adapterio-1.7.0/pyproject.toml
+-rw-r--r--   0 mgrahovac   (502) staff       (20)       38 2024-05-02 20:33:55.443879 adapterio-1.7.0/setup.cfg
+-rw-r--r--   0 mgrahovac   (502) staff       (20)     2778 2024-05-02 20:31:35.000000 adapterio-1.7.0/setup.py
```

### Comparing `adapterio-1.6.1/PKG-INFO` & `adapterio-1.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 Metadata-Version: 2.1
 Name: adapterio
-Version: 1.6.1
+Version: 1.7.0
 Summary: I/O module
 Home-page: https://github.com/LBNL-ETA/Adapter
 Author: Milica Grahovac, Youness Bennani, Thomas Burke, Katie Coughlin, Mohan Ganeshalingam, Akhil Mathur, Evan Neill, Akshay Sharma, Zheng He and Lyra Lan
 License: BSD-3-Clause-LBNL
 Keywords: data,tables,IO for research computation,sql,excel,csv,dataframe,connection
 Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: pandas>=2.2.0
+Requires-Dist: xlwings>=0.19.4
+Requires-Dist: psycopg2-binary>=2.8.6
+Requires-Dist: SQLAlchemy>=2.0.0
+Requires-Dist: openpyxl>=3.1.2
 
 The `Adapter Python IO` software provides a convenient data table loader from various formats such as `xlsx`, `csv`, `db (sqlite database)`, and `sqlalchemy`. Its main feature is the ability to convert data tables identified in one main and optionally one or more additional input files into `database tables` and `Pandas DataFrames` for downstream usage in any compatible software. `Adapter` builds upon the existing Python packages that allow for the communication between `Python` and `MS Excel`, as well as `databases` and `csv` files. It provides inbuilt capabilities to specify the output location path, as well as a version identifier for a research code run.  In addition to the loading capability, an instance of the `Adapter` `IO` object has the write capability. If invoked, all loaded tables are written as either a single `database` or a set of `csv` files, or both. The purpose of this software is to support the development of research and analytical software through allowing for a simple multi-format IO with versioning and output path specification in the input data itself. The package is supported on `Windows` and `macOS`, as well as for `Linux` for the utilization without any `xlsx` inputs.
```

### Comparing `adapterio-1.6.1/README.md` & `adapterio-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.1/adapter/comm/excel.py` & `adapterio-1.7.0/adapter/comm/excel.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.1/adapter/comm/sql.py` & `adapterio-1.7.0/adapter/comm/sql.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.1/adapter/comm/tools.py` & `adapterio-1.7.0/adapter/comm/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import re
 import sys
 from datetime import datetime
 from pathlib import PureWindowsPath, PurePosixPath
+import tkinter as tk
+from tkinter import filedialog as fd
 
 
 def process_column_labels(list_of_labels):
     """Removes undesired spaces.
 
     Parameters:
 
@@ -131,57 +133,31 @@
     Returns:
 
         fpath: string
             Fullpath to the selected input file, or,
             in case of multiple file selection,
             the selected input folder path holding the files.
     """
+    root = tk.Tk()
+    root.withdraw()
 
-    # case for Windows
-    if sys.platform.lower().startswith("win"):
+    print(
+        user_message
+        + " (You may have to search for the file prompt window)"
+    )
 
-        print(user_message)
-        import win32ui, win32con
+    if mul_fls:
+        fpath = fd.askdirectory(title=user_message)
 
-        # For multiple files replace 0 with win32con.OFN_ALLOWMULTISELECT below
-        if mul_fls:
-            dial_flg = win32con.OFN_ALLOWMULTISELECT
-        else:
-            dial_flg = 0
-
-        fd = win32ui.CreateFileDialog(1, None, None, dial_flg)
-
-        fd.SetOFNTitle(user_message)
-        if fd.DoModal() == win32con.IDCANCEL:
-            sys.exit(1)
-
-        # file_name = fd.GetFileName()
-        fpath = fd.GetPathName()
-
-        return fpath
-
-    # case for OSX
-    elif sys.platform.lower() == "darwin":
-
-        print(
-            user_message
-            + " (You may have to search for the file prompt window)"
+    else:
+        fpath = fd.askopenfilename(
+            title=user_message,
+            filetypes=[("Excel", "*.xlsx *.xls"), ("Database", "*.db")],
         )
-        from tkinter import filedialog as fd
-
-        if mul_fls:
-            fpath = fd.askdirectory(title=user_message)
-
-        else:
-            fpath = fd.askopenfilename(
-                title=user_message,
-                filetypes=[("Excel", "*.xlsx *.xls"), ("Database", "*.db")],
-            )
-
-        return fpath
+    return fpath
 
 
 def mark_time(prefix: str = "", ts_format: str = "short") -> str:
     """This method creates a string using prefix string and a timestamp.
 
     Parameters
     ----------
```

### Comparing `adapterio-1.6.1/adapter/i_o.py` & `adapterio-1.7.0/adapter/i_o.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.1/adapter/label_map.py` & `adapterio-1.7.0/adapter/label_map.py`

 * *Files identical despite different names*

### Comparing `adapterio-1.6.1/adapter/to_python.py` & `adapterio-1.7.0/adapter/to_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             dict_of_dfs: dictionary of dataframes
                 Python dictionary with table name/
                 named range as keys and contents of
                 the corresponding named data object
                 values
         """
         # check if any name in data_object_names not in excel file
-        all_input_ranges = {object_range.name for object_range in self.wb.defined_names.definedName}
+        all_input_ranges = set(self.wb.defined_names.keys())    
         all_input_tables = {object_table for ws in self.wb.worksheets for object_table in ws.tables.keys()}
         all_input_objects = all_input_ranges | all_input_tables
 
         if isinstance(data_object_names, list):
             data_object_names = set(data_object_names)
             missings = data_object_names - all_input_objects
             if len(missings) > 0:
```

### Comparing `adapterio-1.6.1/adapterio.egg-info/PKG-INFO` & `adapterio-1.7.0/adapterio.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 Metadata-Version: 2.1
 Name: adapterio
-Version: 1.6.1
+Version: 1.7.0
 Summary: I/O module
 Home-page: https://github.com/LBNL-ETA/Adapter
 Author: Milica Grahovac, Youness Bennani, Thomas Burke, Katie Coughlin, Mohan Ganeshalingam, Akhil Mathur, Evan Neill, Akshay Sharma, Zheng He and Lyra Lan
 License: BSD-3-Clause-LBNL
 Keywords: data,tables,IO for research computation,sql,excel,csv,dataframe,connection
 Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: pandas>=2.2.0
+Requires-Dist: xlwings>=0.19.4
+Requires-Dist: psycopg2-binary>=2.8.6
+Requires-Dist: SQLAlchemy>=2.0.0
+Requires-Dist: openpyxl>=3.1.2
 
 The `Adapter Python IO` software provides a convenient data table loader from various formats such as `xlsx`, `csv`, `db (sqlite database)`, and `sqlalchemy`. Its main feature is the ability to convert data tables identified in one main and optionally one or more additional input files into `database tables` and `Pandas DataFrames` for downstream usage in any compatible software. `Adapter` builds upon the existing Python packages that allow for the communication between `Python` and `MS Excel`, as well as `databases` and `csv` files. It provides inbuilt capabilities to specify the output location path, as well as a version identifier for a research code run.  In addition to the loading capability, an instance of the `Adapter` `IO` object has the write capability. If invoked, all loaded tables are written as either a single `database` or a set of `csv` files, or both. The purpose of this software is to support the development of research and analytical software through allowing for a simple multi-format IO with versioning and output path specification in the input data itself. The package is supported on `Windows` and `macOS`, as well as for `Linux` for the utilization without any `xlsx` inputs.
```

### Comparing `adapterio-1.6.1/setup.py` & `adapterio-1.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,14 @@
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Programming Language :: Python :: 3.8",
     ],
     keywords="data, tables, IO for research computation, sql, excel, csv, dataframe, connection",
     packages=find_packages(exclude=["*.tests", "*.tests"]),
     install_requires=[
-        "pandas>=1.0.4",
+        "pandas>=2.2.0",
         "xlwings>=0.19.4",
         "psycopg2-binary>=2.8.6",
-        "SQLAlchemy==1.4.29",
-        "openpyxl==3.0.9",
+        "SQLAlchemy>=2.0.0",
+        "openpyxl>=3.1.2",
     ],
 )
```

