# Comparing `tmp/xlextract-0.1.4.tar.gz` & `tmp/xlextract-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlextract-0.1.4.tar", max compression
+gzip compressed data, was "xlextract-0.1.5.tar", max compression
```

## Comparing `xlextract-0.1.4.tar` & `xlextract-0.1.5.tar`

### file list

```diff
@@ -1,104 +1,5 @@
--rw-r--r--   0        0        0     3952 2024-05-02 00:24:36.472717 xlextract-0.1.4/README.md
--rw-r--r--   0        0        0      392 2024-05-02 00:24:52.072839 xlextract-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       34 2024-05-01 18:05:47.773922 xlextract-0.1.4/xlextract/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2024-05-01 18:06:56.104470 xlextract-0.1.4/xlextract/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180414 2024-05-01 18:05:47.673921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1647 2024-05-01 18:05:47.673921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    57974 2024-05-01 18:05:47.663921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1686 2024-05-01 18:05:47.663921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    24760 2024-05-01 18:05:47.663921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1643 2024-05-01 18:05:47.663921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0   113635 2024-05-01 18:05:47.663921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1711 2024-05-01 18:05:47.663921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    28418 2024-05-01 18:05:47.653921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1653 2024-05-01 18:05:47.653921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0  1711103 2024-05-01 18:05:47.743922 xlextract-0.1.4/xlextract/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1724 2024-05-01 18:05:47.743922 xlextract-0.1.4/xlextract/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   131375 2024-05-01 18:05:47.653921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1673 2024-05-01 18:05:47.653921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   801174 2024-05-01 18:05:47.653921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1713 2024-05-01 18:05:47.653921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3736 2024-05-01 18:05:47.623921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1624 2024-05-01 18:05:47.623921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   129375 2024-05-01 18:05:47.623921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1686 2024-05-01 18:05:47.623921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    83381 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1691 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0     7812 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1701 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    26274 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/_policybase.data.json
--rw-r--r--   0        0        0     1722 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/_policybase.meta.json
--rw-r--r--   0        0        0    16650 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1653 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7512 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1666 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25164 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1638 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9460 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1651 2024-05-01 18:05:47.613921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0   123702 2024-05-01 18:05:47.603921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1798 2024-05-01 18:05:47.603921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    12130 2024-05-01 18:05:47.603921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1702 2024-05-01 18:05:47.603921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0   116099 2024-05-01 18:05:47.603921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1667 2024-05-01 18:05:47.603921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    30801 2024-05-01 18:05:47.593921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1677 2024-05-01 18:05:47.593921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     6457 2024-05-01 18:05:47.593921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1703 2024-05-01 18:05:47.593921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0     5392 2024-05-01 18:05:47.593921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/_abc.data.json
--rw-r--r--   0        0        0     1666 2024-05-01 18:05:47.593921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/_abc.meta.json
--rw-r--r--   0        0        0    58770 2024-05-01 18:05:47.593921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1763 2024-05-01 18:05:47.593921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    77929 2024-05-01 18:05:47.593921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1808 2024-05-01 18:05:47.593921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0   117718 2024-05-01 18:05:47.583921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1833 2024-05-01 18:05:47.583921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    19857 2024-05-01 18:05:47.583921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1683 2024-05-01 18:05:47.583921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    22958 2024-05-01 18:05:47.583921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/readers.data.json
--rw-r--r--   0        0        0     1843 2024-05-01 18:05:47.583921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/readers.meta.json
--rw-r--r--   0        0        0    10874 2024-05-01 18:05:47.573921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/resources/__init__.data.json
--rw-r--r--   0        0        0     1767 2024-05-01 18:05:47.583921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/resources/__init__.meta.json
--rw-r--r--   0        0        0     1809 2024-05-01 18:05:47.573921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/resources/abc.data.json
--rw-r--r--   0        0        0     1666 2024-05-01 18:05:47.573921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/importlib/resources/abc.meta.json
--rw-r--r--   0        0        0   108464 2024-05-01 18:05:47.573921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1686 2024-05-01 18:05:47.573921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   405124 2024-05-01 18:05:47.573921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1755 2024-05-01 18:05:47.573921 xlextract-0.1.4/xlextract/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4913 2024-05-01 18:05:47.553920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1613 2024-05-01 18:05:47.553920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0   104515 2024-05-01 18:05:47.543920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1695 2024-05-01 18:05:47.543920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0   125881 2024-05-01 18:05:47.543920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1693 2024-05-01 18:05:47.543920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   246513 2024-05-01 18:05:47.543920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1714 2024-05-01 18:05:47.543920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    45119 2024-05-01 18:05:47.533920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/resource.data.json
--rw-r--r--   0        0        0     1628 2024-05-01 18:05:47.533920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/resource.meta.json
--rw-r--r--   0        0        0    14507 2024-05-01 18:05:47.533920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1638 2024-05-01 18:05:47.533920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28949 2024-05-01 18:05:47.533920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1663 2024-05-01 18:05:47.533920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    52302 2024-05-01 18:05:47.533920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1706 2024-05-01 18:05:47.533920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   224781 2024-05-01 18:05:47.523920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1688 2024-05-01 18:05:47.523920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   157649 2024-05-01 18:05:47.513920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/sys/__init__.data.json
--rw-r--r--   0        0        0     1735 2024-05-01 18:05:47.513920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/sys/__init__.meta.json
--rw-r--r--   0        0        0   310173 2024-05-01 18:05:47.513920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1704 2024-05-01 18:05:47.513920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   600170 2024-05-01 18:05:47.503920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1706 2024-05-01 18:05:47.503920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0   121173 2024-05-01 18:05:47.473920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1670 2024-05-01 18:05:47.473920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0     9572 2024-05-01 18:06:56.104470 xlextract-0.1.4/xlextract/.mypy_cache/3.11/xlextract/__init__.data.json
--rw-r--r--   0        0        0     1525 2024-05-01 18:06:56.104470 xlextract-0.1.4/xlextract/.mypy_cache/3.11/xlextract/__init__.meta.json
--rw-r--r--   0        0        0    12521 2024-05-01 18:06:19.624179 xlextract-0.1.4/xlextract/.mypy_cache/3.11/xlextract/xlextract.data.json
--rw-r--r--   0        0        0     1570 2024-05-01 18:06:19.624179 xlextract-0.1.4/xlextract/.mypy_cache/3.11/xlextract/xlextract.meta.json
--rw-r--r--   0        0        0    98226 2024-05-01 18:05:47.473920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/zipfile/__init__.data.json
--rw-r--r--   0        0        0     1699 2024-05-01 18:05:47.473920 xlextract-0.1.4/xlextract/.mypy_cache/3.11/zipfile/__init__.meta.json
--rw-r--r--   0        0        0      190 2024-05-01 18:05:47.773922 xlextract-0.1.4/xlextract/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     4424 2024-05-02 00:23:15.412088 xlextract-0.1.4/xlextract/__init__.py
--rw-r--r--   0        0        0     1884 2024-05-01 18:06:16.984157 xlextract-0.1.4/xlextract/classes.py
--rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 xlextract-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3945 2024-05-02 00:47:30.904698 xlextract-0.1.5/README.md
+-rw-r--r--   0        0        0      392 2024-05-02 00:49:51.815971 xlextract-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4424 2024-05-02 00:23:15.412088 xlextract-0.1.5/xlextract/__init__.py
+-rw-r--r--   0        0        0     1884 2024-05-01 18:06:16.984157 xlextract-0.1.5/xlextract/classes.py
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 xlextract-0.1.5/PKG-INFO
```

### Comparing `xlextract-0.1.4/README.md` & `xlextract-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 or via pip with: ```pip install xlextract```
 
 ## What does it do?
 xlextract searches a spreadsheet for a keyword you provide and extracts nearby data.  
 It provides three operations:
 1. Right Lookup: Extract cell value to the immediate right of the keyword
 2. Left Lookup: Extract cell value to the immediate left of the keyword
-3. Table Lookup: Extract an entire Excel table of data adjacent to the keyword. The table is modeled as a list of dictionaries where each list item represents a row in the table and the item is a dictionary (key/value pair) where each item in the dictionary represents a column of the row and the key is the column header. An example will be provided below.
+3. Table Lookup: Extract an entire Excel table of data adjacent to the keyword. The table is modeled as a list of dictionaries where each list item represents a row in the table and the list item is a dictionary (key/value pairs) where each item in the dictionary represents a column of the row and where the key is the column header. An example will be provided below.
 
 ## How do I use it in my project?
 You need four bits of information to use xlextract:
 1. The name of the Excel file
 2. The name of the sheet in the Excel file
 3. The keyword you want to search for
 4. The type of lookup you want to do (Right, Left, or Table)
@@ -40,15 +40,15 @@
 from xlextract import XLExtract
 
 vrf_table = XLExtract("design_document.xlsx", "Tenants", "VRF NAME")
 ```
 
 # Table Lookup Example
 Assuming we have an Excel spreadsheet with a "Tenants" tab that contains a table that looks like this:  
-image  
+![Sample Excel Table](./art/ACI_VRF_Table.jpg?raw=true)
 If we then do this in our Python code:
 ```python
 vrf_table.TLookup()
 
 print(json.dumps(vrf_table.value, indent = 4))
 ```
 
@@ -64,28 +64,20 @@
         "TENANT": "Prod-tn",
         "VRF NAME": "Dev-VRF",
         "ENABLE PREFERRED GROUP": "enabled"
     }
 ]
 ```
 
-## Class Attributes
-- filename (str)
-- sheet (sheet object)
-- sheetname (str)
-- keyword (str)
-- keycoords (str)
-- value (list[dict] or str)
-
 ## How does it do the table lookup?
 The table lookup assumes the keyword you provide resides in the table header.  
 It first searches cells left of the keyword, then right of the keyword to establish table width.  
 When it encounters the first empty cell it assumes the edge of the table.  
 Then it moves down from the keyword cell, if data is present it captures the row.  
 When it encounters the first empty cell it assumes the bottom of the table, completing the extraction.
 
 ## CAVEATS
 The source Excel spreadsheet content should be planned ahead of time to account for these operational caveats:
 - Keywords on a given sheet must be unique
 - Keywords for a table should be one of the column headers
 - All cells in a table header should be populated for the table lookup to determine the correct table width
-- All data cells in the keyword column should be populated for the table lookup to determine the correct table height. Because of this you should not use columns with optional data for the keyword, or populated the cells with something like "N/A"
+- All data cells in the keyword column should be populated for the table lookup to determine the correct table height. Because of this you should not use columns with optional data for the keyword, or if you must, populate all the cells in the column with something ("N/A" or "empty" if a cell has no value for example).
```

### Comparing `xlextract-0.1.4/xlextract/__init__.py` & `xlextract-0.1.5/xlextract/__init__.py`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.4/xlextract/classes.py` & `xlextract-0.1.5/xlextract/classes.py`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.4/PKG-INFO` & `xlextract-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlextract
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extract data from Excel files
 Author: AJ Cruz
 Author-email: aj.cruz@computacenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -27,15 +27,15 @@
 or via pip with: ```pip install xlextract```
 
 ## What does it do?
 xlextract searches a spreadsheet for a keyword you provide and extracts nearby data.  
 It provides three operations:
 1. Right Lookup: Extract cell value to the immediate right of the keyword
 2. Left Lookup: Extract cell value to the immediate left of the keyword
-3. Table Lookup: Extract an entire Excel table of data adjacent to the keyword. The table is modeled as a list of dictionaries where each list item represents a row in the table and the item is a dictionary (key/value pair) where each item in the dictionary represents a column of the row and the key is the column header. An example will be provided below.
+3. Table Lookup: Extract an entire Excel table of data adjacent to the keyword. The table is modeled as a list of dictionaries where each list item represents a row in the table and the list item is a dictionary (key/value pairs) where each item in the dictionary represents a column of the row and where the key is the column header. An example will be provided below.
 
 ## How do I use it in my project?
 You need four bits of information to use xlextract:
 1. The name of the Excel file
 2. The name of the sheet in the Excel file
 3. The keyword you want to search for
 4. The type of lookup you want to do (Right, Left, or Table)
@@ -53,15 +53,15 @@
 from xlextract import XLExtract
 
 vrf_table = XLExtract("design_document.xlsx", "Tenants", "VRF NAME")
 ```
 
 # Table Lookup Example
 Assuming we have an Excel spreadsheet with a "Tenants" tab that contains a table that looks like this:  
-image  
+![Sample Excel Table](./art/ACI_VRF_Table.jpg?raw=true)
 If we then do this in our Python code:
 ```python
 vrf_table.TLookup()
 
 print(json.dumps(vrf_table.value, indent = 4))
 ```
 
@@ -77,28 +77,20 @@
         "TENANT": "Prod-tn",
         "VRF NAME": "Dev-VRF",
         "ENABLE PREFERRED GROUP": "enabled"
     }
 ]
 ```
 
-## Class Attributes
-- filename (str)
-- sheet (sheet object)
-- sheetname (str)
-- keyword (str)
-- keycoords (str)
-- value (list[dict] or str)
-
 ## How does it do the table lookup?
 The table lookup assumes the keyword you provide resides in the table header.  
 It first searches cells left of the keyword, then right of the keyword to establish table width.  
 When it encounters the first empty cell it assumes the edge of the table.  
 Then it moves down from the keyword cell, if data is present it captures the row.  
 When it encounters the first empty cell it assumes the bottom of the table, completing the extraction.
 
 ## CAVEATS
 The source Excel spreadsheet content should be planned ahead of time to account for these operational caveats:
 - Keywords on a given sheet must be unique
 - Keywords for a table should be one of the column headers
 - All cells in a table header should be populated for the table lookup to determine the correct table width
-- All data cells in the keyword column should be populated for the table lookup to determine the correct table height. Because of this you should not use columns with optional data for the keyword, or populated the cells with something like "N/A"
+- All data cells in the keyword column should be populated for the table lookup to determine the correct table height. Because of this you should not use columns with optional data for the keyword, or if you must, populate all the cells in the column with something ("N/A" or "empty" if a cell has no value for example).
```

