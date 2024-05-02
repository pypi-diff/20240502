# Comparing `tmp/layeutils-0.2.8.tar.gz` & `tmp/layeutils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layeutils-0.2.8.tar", last modified: Fri Mar 15 05:32:17 2024, max compression
+gzip compressed data, was "layeutils-0.2.9.tar", last modified: Fri Mar 15 05:35:06 2024, max compression
```

## Comparing `layeutils-0.2.8.tar` & `layeutils-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 05:32:17.066104 layeutils-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-15 05:32:16.000000 layeutils-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-15 05:32:17.066104 layeutils-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 05:32:16.000000 layeutils-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 05:32:17.062104 layeutils-0.2.8/layeutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 05:32:16.000000 layeutils-0.2.8/layeutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-15 05:32:16.000000 layeutils-0.2.8/layeutils/dataprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-15 05:32:16.000000 layeutils-0.2.8/layeutils/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-15 05:32:16.000000 layeutils-0.2.8/layeutils/dtale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-03-15 05:32:16.000000 layeutils-0.2.8/layeutils/googlesheets.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 05:32:16.000000 layeutils-0.2.8/layeutils/homeproxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-15 05:32:16.000000 layeutils-0.2.8/layeutils/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-15 05:32:16.000000 layeutils-0.2.8/layeutils/plotly.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-15 05:32:16.000000 layeutils-0.2.8/layeutils/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 05:32:17.066104 layeutils-0.2.8/layeutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-15 05:32:17.000000 layeutils-0.2.8/layeutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-15 05:32:17.000000 layeutils-0.2.8/layeutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 05:32:17.000000 layeutils-0.2.8/layeutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-15 05:32:17.000000 layeutils-0.2.8/layeutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 05:32:17.066104 layeutils-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-15 05:32:16.000000 layeutils-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 05:35:06.120958 layeutils-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-15 05:35:05.000000 layeutils-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-15 05:35:06.120958 layeutils-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 05:35:05.000000 layeutils-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 05:35:06.116958 layeutils-0.2.9/layeutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 05:35:05.000000 layeutils-0.2.9/layeutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-15 05:35:05.000000 layeutils-0.2.9/layeutils/dataprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-15 05:35:05.000000 layeutils-0.2.9/layeutils/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-15 05:35:05.000000 layeutils-0.2.9/layeutils/dtale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-15 05:35:05.000000 layeutils-0.2.9/layeutils/googlesheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 05:35:05.000000 layeutils-0.2.9/layeutils/homeproxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-15 05:35:05.000000 layeutils-0.2.9/layeutils/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-15 05:35:05.000000 layeutils-0.2.9/layeutils/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-15 05:35:05.000000 layeutils-0.2.9/layeutils/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 05:35:06.120958 layeutils-0.2.9/layeutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-15 05:35:06.000000 layeutils-0.2.9/layeutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-15 05:35:06.000000 layeutils-0.2.9/layeutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 05:35:06.000000 layeutils-0.2.9/layeutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-15 05:35:06.000000 layeutils-0.2.9/layeutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 05:35:06.120958 layeutils-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-15 05:35:05.000000 layeutils-0.2.9/setup.py
```

### Comparing `layeutils-0.2.8/LICENSE` & `layeutils-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `layeutils-0.2.8/layeutils/dataprocess.py` & `layeutils-0.2.9/layeutils/dataprocess.py`

 * *Files identical despite different names*

### Comparing `layeutils-0.2.8/layeutils/date.py` & `layeutils-0.2.9/layeutils/date.py`

 * *Files identical despite different names*

### Comparing `layeutils-0.2.8/layeutils/googlesheets.py` & `layeutils-0.2.9/layeutils/googlesheets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 """使用gspread库，需要首先安装配置：
     https://docs.gspread.org/en/latest/oauth2.html#service-account
 """
 import gspread
-import homeproxy
 import pandas as pd
 
 
 def get_spreadsheet(file_title: str, folder_id: str = None) -> gspread.Spreadsheet:
     """根据给定的文件名，Sheet名称，返回gspread.Worksheet对象; 如果要获得gspread.Spreadsheet对象，使用get_spreadsheet()方法
 
     Args:
         file_title (str): _description_
         folder_id (str, optional): 如果有重名文件，则默认返回第一个，否则需要指定folder_id. Defaults to None.. Defaults to None.
 
     Returns:
         gspread.Worksheet: _description_
     """
-    homeproxy.using_home_server_proxy()
     return gspread.service_account().open(title=file_title, folder_id=folder_id)
 
 
 def get_worksheet(file_title: str, sheet_name: str, folder_id: str = None) -> gspread.Worksheet:
     """根据给定的文件名，Sheet名称，返回gspread.Worksheet对象; 如果要获得gspread.Spreadsheet对象，使用get_spreadsheet()方法
 
     Args:
         file_title (str): _description_
         sheet_name (str): _description_
         folder_id (str, optional): 如果有重名文件，则默认返回第一个，否则需要指定folder_id. Defaults to None.. Defaults to None.
 
     Returns:
         gspread.Worksheet: _description_
     """
-    homeproxy.using_home_server_proxy()
     spreadsheet = gspread.service_account().open(title=file_title, folder_id=folder_id)
     return spreadsheet.worksheet(title=sheet_name)
 
 
 def worksheet2df(worksheet: gspread.Worksheet) -> pd.DataFrame:
     """将gspread.Worksheet对象内容提取成为pd.DataFrame
 
@@ -51,17 +48,15 @@
 def update_worksheet_by_df(worksheet: gspread.Worksheet, content_df: pd.DataFrame) -> None:
     """更新worksheet文件，这里的更新不是追加，而是全量更新
 
     Args:
         worksheet (gspread.Worksheet): _description_
         content_df (pd.DataFrame): _description_
     """
-    homeproxy.using_home_server_proxy()
     worksheet.update(
         [content_df.columns.values.tolist()] + content_df.values.tolist(),
         value_input_option='USER_ENTERED')
 
 
 def add_worksheet(spreadsheet: gspread.Spreadsheet, worksheet_title: str, rows: int, cols: int):
-    homeproxy.using_home_server_proxy()
     added = spreadsheet.add_worksheet(title=worksheet_title, rows=rows, cols=cols)
     return added
```

### Comparing `layeutils-0.2.8/layeutils/mongodb.py` & `layeutils-0.2.9/layeutils/mongodb.py`

 * *Files identical despite different names*

### Comparing `layeutils-0.2.8/layeutils/plotly.py` & `layeutils-0.2.9/layeutils/plotly.py`

 * *Files identical despite different names*

### Comparing `layeutils-0.2.8/layeutils/request.py` & `layeutils-0.2.9/layeutils/request.py`

 * *Files identical despite different names*

