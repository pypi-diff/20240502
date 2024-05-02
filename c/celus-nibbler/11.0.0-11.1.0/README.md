# Comparing `tmp/celus_nibbler-11.0.0.tar.gz` & `tmp/celus_nibbler-11.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celus_nibbler-11.0.0.tar", max compression
+gzip compressed data, was "celus_nibbler-11.1.0.tar", max compression
```

## Comparing `celus_nibbler-11.0.0.tar` & `celus_nibbler-11.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1057 2022-06-17 07:35:22.867507 celus_nibbler-11.0.0/LICENSE
--rw-r--r--   0        0        0      644 2024-03-13 08:47:12.478670 celus_nibbler-11.0.0/celus_nibbler/__init__.py
--rw-r--r--   0        0        0     8253 2024-03-25 08:56:47.282003 celus_nibbler-11.0.0/celus_nibbler/__main__.py
--rw-r--r--   0        0        0     5480 2023-11-22 12:21:31.240892 celus_nibbler-11.0.0/celus_nibbler/aggregator.py
--rw-r--r--   0        0        0     6946 2024-03-13 08:47:12.478670 celus_nibbler-11.0.0/celus_nibbler/conditions.py
--rw-r--r--   0        0        0     6096 2024-03-13 08:47:12.478670 celus_nibbler-11.0.0/celus_nibbler/coordinates.py
--rw-r--r--   0        0        0    14359 2024-03-13 08:47:12.478670 celus_nibbler-11.0.0/celus_nibbler/data_headers.py
--rw-r--r--   0        0        0     2117 2024-03-25 08:56:47.282003 celus_nibbler-11.0.0/celus_nibbler/definitions/__init__.py
--rw-r--r--   0        0        0     1717 2024-03-13 08:47:12.478670 celus_nibbler-11.0.0/celus_nibbler/definitions/base.py
--rw-r--r--   0        0        0     4238 2023-10-27 12:46:00.516284 celus_nibbler-11.0.0/celus_nibbler/definitions/celus_format.py
--rw-r--r--   0        0        0    15825 2024-03-25 08:56:47.282003 celus_nibbler-11.0.0/celus_nibbler/definitions/counter.py
--rw-r--r--   0        0        0     4561 2023-10-27 12:46:00.520284 celus_nibbler-11.0.0/celus_nibbler/definitions/date_based.py
--rw-r--r--   0        0        0     4472 2023-10-27 12:46:00.520284 celus_nibbler-11.0.0/celus_nibbler/definitions/date_metric_based.py
--rw-r--r--   0        0        0     4726 2023-10-27 12:46:00.520284 celus_nibbler-11.0.0/celus_nibbler/definitions/generic.py
--rw-r--r--   0        0        0     4381 2023-10-27 12:46:00.520284 celus_nibbler-11.0.0/celus_nibbler/definitions/metric_based.py
--rw-r--r--   0        0        0    14563 2024-03-25 08:56:47.282003 celus_nibbler-11.0.0/celus_nibbler/eat_and_poop.py
--rw-r--r--   0        0        0     5880 2024-03-13 08:47:12.478670 celus_nibbler-11.0.0/celus_nibbler/errors.py
--rw-r--r--   0        0        0     2785 2022-11-01 15:22:27.669687 celus_nibbler-11.0.0/celus_nibbler/parsers/__init__.py
--rw-r--r--   0        0        0    15074 2024-03-25 08:56:47.282003 celus_nibbler-11.0.0/celus_nibbler/parsers/base.py
--rw-r--r--   0        0        0    13122 2024-03-25 08:56:47.282003 celus_nibbler-11.0.0/celus_nibbler/parsers/counter/__init__.py
--rw-r--r--   0        0        0    11529 2024-03-13 08:47:12.478670 celus_nibbler-11.0.0/celus_nibbler/parsers/counter/c4.py
--rw-r--r--   0        0        0    10618 2024-03-25 08:56:47.282003 celus_nibbler-11.0.0/celus_nibbler/parsers/counter/c5.py
--rw-r--r--   0        0        0     3803 2024-03-25 08:56:47.282003 celus_nibbler-11.0.0/celus_nibbler/parsers/counter/c5json.py
--rw-r--r--   0        0        0      156 2023-08-15 12:26:51.461995 celus_nibbler-11.0.0/celus_nibbler/parsers/dynamic.py
--rw-r--r--   0        0        0        0 2022-10-21 20:55:53.099727 celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/__init__.py
--rw-r--r--   0        0        0      194 2022-11-04 15:01:01.540828 celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/base.py
--rw-r--r--   0        0        0     5683 2023-07-29 08:57:05.293613 celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/celus_format.py
--rw-r--r--   0        0        0      322 2023-07-19 09:21:05.347414 celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/date_based.py
--rw-r--r--   0        0        0     2547 2023-07-19 09:21:05.347414 celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/date_metric_based.py
--rw-r--r--   0        0        0      774 2023-07-19 09:21:05.347414 celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/generic.py
--rw-r--r--   0        0        0     2478 2023-07-19 09:21:05.347414 celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/metric_based.py
--rw-r--r--   0        0        0    14705 2024-03-13 08:47:12.482670 celus_nibbler-11.0.0/celus_nibbler/reader.py
--rw-r--r--   0        0        0    15482 2024-03-25 08:56:47.286003 celus_nibbler-11.0.0/celus_nibbler/sources.py
--rw-r--r--   0        0        0     1624 2023-10-27 12:46:00.524284 celus_nibbler-11.0.0/celus_nibbler/utils.py
--rw-r--r--   0        0        0     9468 2024-03-13 08:47:12.482670 celus_nibbler-11.0.0/celus_nibbler/validators.py
--rw-r--r--   0        0        0     3311 2024-03-25 09:04:45.769202 celus_nibbler-11.0.0/pyproject.toml
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 celus_nibbler-11.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-06-17 07:35:22.867507 celus_nibbler-11.1.0/LICENSE
+-rw-r--r--   0        0        0      644 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/__init__.py
+-rw-r--r--   0        0        0     8253 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/__main__.py
+-rw-r--r--   0        0        0     5480 2023-11-22 12:21:31.240892 celus_nibbler-11.1.0/celus_nibbler/aggregator.py
+-rw-r--r--   0        0        0     6946 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/conditions.py
+-rw-r--r--   0        0        0     6096 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/coordinates.py
+-rw-r--r--   0        0        0    14359 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/data_headers.py
+-rw-r--r--   0        0        0     2117 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/definitions/__init__.py
+-rw-r--r--   0        0        0     1717 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/definitions/base.py
+-rw-r--r--   0        0        0     4238 2023-10-27 12:46:00.516284 celus_nibbler-11.1.0/celus_nibbler/definitions/celus_format.py
+-rw-r--r--   0        0        0    15825 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/definitions/counter.py
+-rw-r--r--   0        0        0     4561 2023-10-27 12:46:00.520284 celus_nibbler-11.1.0/celus_nibbler/definitions/date_based.py
+-rw-r--r--   0        0        0     4472 2023-10-27 12:46:00.520284 celus_nibbler-11.1.0/celus_nibbler/definitions/date_metric_based.py
+-rw-r--r--   0        0        0     4726 2023-10-27 12:46:00.520284 celus_nibbler-11.1.0/celus_nibbler/definitions/generic.py
+-rw-r--r--   0        0        0     4381 2023-10-27 12:46:00.520284 celus_nibbler-11.1.0/celus_nibbler/definitions/metric_based.py
+-rw-r--r--   0        0        0    14563 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/eat_and_poop.py
+-rw-r--r--   0        0        0     6074 2024-03-27 09:28:05.075344 celus_nibbler-11.1.0/celus_nibbler/errors.py
+-rw-r--r--   0        0        0     2785 2022-11-01 15:22:27.669687 celus_nibbler-11.1.0/celus_nibbler/parsers/__init__.py
+-rw-r--r--   0        0        0    15074 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/parsers/base.py
+-rw-r--r--   0        0        0    13122 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/parsers/counter/__init__.py
+-rw-r--r--   0        0        0    11529 2024-03-13 08:47:12.478670 celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c4.py
+-rw-r--r--   0        0        0    10694 2024-04-16 09:33:13.184343 celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c5.py
+-rw-r--r--   0        0        0     3803 2024-03-25 08:56:47.282003 celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c5json.py
+-rw-r--r--   0        0        0      156 2023-08-15 12:26:51.461995 celus_nibbler-11.1.0/celus_nibbler/parsers/dynamic.py
+-rw-r--r--   0        0        0        0 2022-10-21 20:55:53.099727 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/__init__.py
+-rw-r--r--   0        0        0      194 2022-11-04 15:01:01.540828 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/base.py
+-rw-r--r--   0        0        0     5683 2023-07-29 08:57:05.293613 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/celus_format.py
+-rw-r--r--   0        0        0      322 2023-07-19 09:21:05.347414 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/date_based.py
+-rw-r--r--   0        0        0     2547 2023-07-19 09:21:05.347414 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/date_metric_based.py
+-rw-r--r--   0        0        0      774 2023-07-19 09:21:05.347414 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/generic.py
+-rw-r--r--   0        0        0     2478 2023-07-19 09:21:05.347414 celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/metric_based.py
+-rw-r--r--   0        0        0    14940 2024-03-27 09:04:12.880873 celus_nibbler-11.1.0/celus_nibbler/reader.py
+-rw-r--r--   0        0        0    15482 2024-03-25 08:56:47.286003 celus_nibbler-11.1.0/celus_nibbler/sources.py
+-rw-r--r--   0        0        0     1624 2023-10-27 12:46:00.524284 celus_nibbler-11.1.0/celus_nibbler/utils.py
+-rw-r--r--   0        0        0     9468 2024-03-13 08:47:12.482670 celus_nibbler-11.1.0/celus_nibbler/validators.py
+-rw-r--r--   0        0        0     3311 2024-04-16 09:36:42.696448 celus_nibbler-11.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 celus_nibbler-11.1.0/PKG-INFO
```

### Comparing `celus_nibbler-11.0.0/LICENSE` & `celus_nibbler-11.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/__init__.py` & `celus_nibbler-11.1.0/celus_nibbler/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/__main__.py` & `celus_nibbler-11.1.0/celus_nibbler/__main__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/aggregator.py` & `celus_nibbler-11.1.0/celus_nibbler/aggregator.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/conditions.py` & `celus_nibbler-11.1.0/celus_nibbler/conditions.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/coordinates.py` & `celus_nibbler-11.1.0/celus_nibbler/coordinates.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/data_headers.py` & `celus_nibbler-11.1.0/celus_nibbler/data_headers.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/definitions/__init__.py` & `celus_nibbler-11.1.0/celus_nibbler/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/definitions/base.py` & `celus_nibbler-11.1.0/celus_nibbler/definitions/base.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/definitions/celus_format.py` & `celus_nibbler-11.1.0/celus_nibbler/definitions/celus_format.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/definitions/counter.py` & `celus_nibbler-11.1.0/celus_nibbler/definitions/counter.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/definitions/date_based.py` & `celus_nibbler-11.1.0/celus_nibbler/definitions/date_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/definitions/date_metric_based.py` & `celus_nibbler-11.1.0/celus_nibbler/definitions/date_metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/definitions/generic.py` & `celus_nibbler-11.1.0/celus_nibbler/definitions/generic.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/definitions/metric_based.py` & `celus_nibbler-11.1.0/celus_nibbler/definitions/metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/eat_and_poop.py` & `celus_nibbler-11.1.0/celus_nibbler/eat_and_poop.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/errors.py` & `celus_nibbler-11.1.0/celus_nibbler/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,22 @@
             return False
         return all(
             getattr(self, attr, None) == getattr(other, attr, None)
             for attr in ["file", "file_suffix"]
         )
 
 
+class XlsError(NibblerError):
+    def __init__(self, xls_exception):
+        self.xls_exception = xls_exception
+
+    def __str__(self):
+        return f'XLS Exception: "{self.xls_exception}"'
+
+
 class JsonException(NibblerError):
     """
     Error while parsing JSON format
     """
 
     def __init__(self, reason: str):
         self.reason = reason
```

### Comparing `celus_nibbler-11.0.0/celus_nibbler/parsers/__init__.py` & `celus_nibbler-11.1.0/celus_nibbler/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/parsers/base.py` & `celus_nibbler-11.1.0/celus_nibbler/parsers/base.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/parsers/counter/__init__.py` & `celus_nibbler-11.1.0/celus_nibbler/parsers/counter/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/parsers/counter/c4.py` & `celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c4.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/parsers/counter/c5.py` & `celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c5.py`

 * *Files 5% similar despite different names*

```diff
@@ -343,14 +343,15 @@
 
     class Area(Counter5HeaderArea):
         DIMENSION_NAMES_MAP = [
             ("Article_Version", {"Article Version", "Article_Version"}),
             ("Access_Type", {"Access Type", "Access_Type"}),
             ("Access_Method", {"Access_Method", "Access Method"}),
             ("Data_Type", {"Data Type", "Data_Type"}),
+            ("Parent_Data_Type", {"Parent Data Type", "Parent_Data_Type"}),
             ("YOP", {"YOP", "Year of Publication", "Year_of_Publication"}),
             ("Platform", {"Platform"}),
             ("Publisher", {"Publisher"}),
         ]
         TITLE_COLUMN_NAMES = ["Parent_Title"]
         ITEM_COLUMN_NAMES = ["Title", "Item"]
```

### Comparing `celus_nibbler-11.0.0/celus_nibbler/parsers/counter/c5json.py` & `celus_nibbler-11.1.0/celus_nibbler/parsers/counter/c5json.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/celus_format.py` & `celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/celus_format.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/date_metric_based.py` & `celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/date_metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/generic.py` & `celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/generic.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/parsers/non_counter/metric_based.py` & `celus_nibbler-11.1.0/celus_nibbler/parsers/non_counter/metric_based.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/reader.py` & `celus_nibbler-11.1.0/celus_nibbler/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from io import BufferedIOBase, BytesIO, RawIOBase, StringIO, TextIOBase, TextIOWrapper
 from typing import IO, Any, Dict, List, Optional, Sequence, Union
 
 import openpyxl
 from celus_nigiri.counter5 import Counter5ReportBase
 from celus_nigiri.csv_detect import detect_csv_dialect, detect_file_encoding
 
+from .errors import XlsError
+
 logger = logging.getLogger(__name__)
 
 
 class _TextIOWrapperNoClose(TextIOWrapper):
     """Wrapper around TextIOWrapper which can't be closed
 
     Usually TextIOWrapper closes the opened file when it is discarded in `__del__` method.
@@ -390,45 +392,48 @@
 
     class XlsReader(TableReader):  # noqa
         """
         Reads XLS file it probably loads entire file into memory
         """
 
         def __init__(self, source: Union[str, pathlib.Path, RawIOBase, BufferedIOBase]):
-            if isinstance(source, (RawIOBase, BufferedIOBase)):
-                workbook = xlrd.open_workbook(file_contents=source.read())
-            else:
-                workbook = xlrd.open_workbook(filename=source)
-
-            self.sheets = []
-
-            # Store each sheet as temporary CSV file
-            for idx in range(workbook.nsheets):
-                sheet = workbook.sheet_by_index(idx)
-
-                # write data to csv
-                f = tempfile.TemporaryFile("w+")
-                # unix dialect escapes all by default
-                dialect = csv.get_dialect("unix")
-                writer = csv.writer(f, dialect=dialect)
-                row_length = sheet.ncols
-                for rx in range(sheet.nrows):
-                    row = sheet.row(rx)
-
-                    # Make sure that length of the row is extending
-                    current_length = len(row)
-                    extra_cells = [""] * (row_length - current_length)
-
-                    writer.writerow([self._cell_to_str(cell) for cell in row] + extra_cells)
-                f.seek(0)
-
-                self.sheets.append(CsvSheetReader(idx, sheet.name, f, dialect="unix"))
-                workbook.unload_sheet(idx)
-
-            workbook.release_resources()
+            try:
+                if isinstance(source, (RawIOBase, BufferedIOBase)):
+                    workbook = xlrd.open_workbook(file_contents=source.read())
+                else:
+                    workbook = xlrd.open_workbook(filename=source)
+
+                self.sheets = []
+
+                # Store each sheet as temporary CSV file
+                for idx in range(workbook.nsheets):
+                    sheet = workbook.sheet_by_index(idx)
+
+                    # write data to csv
+                    f = tempfile.TemporaryFile("w+")
+                    # unix dialect escapes all by default
+                    dialect = csv.get_dialect("unix")
+                    writer = csv.writer(f, dialect=dialect)
+                    row_length = sheet.ncols
+                    for rx in range(sheet.nrows):
+                        row = sheet.row(rx)
+
+                        # Make sure that length of the row is extending
+                        current_length = len(row)
+                        extra_cells = [""] * (row_length - current_length)
+
+                        writer.writerow([self._cell_to_str(cell) for cell in row] + extra_cells)
+                    f.seek(0)
+
+                    self.sheets.append(CsvSheetReader(idx, sheet.name, f, dialect="unix"))
+                    workbook.unload_sheet(idx)
+
+                workbook.release_resources()
+            except xlrd.compdoc.CompDocError as e:
+                raise XlsError(e) from e
 
         def _cell_to_str(self, cell: xlrd.sheet.Cell) -> str:
             if cell.ctype in [xlrd.XL_CELL_EMPTY, xlrd.XL_CELL_BLANK, xlrd.XL_CELL_ERROR]:
                 return ""
 
             elif cell.ctype == xlrd.XL_CELL_TEXT:
                 return cell.value
```

### Comparing `celus_nibbler-11.0.0/celus_nibbler/sources.py` & `celus_nibbler-11.1.0/celus_nibbler/sources.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/utils.py` & `celus_nibbler-11.1.0/celus_nibbler/utils.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/celus_nibbler/validators.py` & `celus_nibbler-11.1.0/celus_nibbler/validators.py`

 * *Files identical despite different names*

### Comparing `celus_nibbler-11.0.0/pyproject.toml` & `celus_nibbler-11.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 plugins = "pydantic.mypy"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 
 [tool.poetry]
 name = "celus-nibbler"
-version = "11.0.0"
+version = "11.1.0"
 description = "Counter-like data reader and processor."
 authors = ["Stepan Henek <stepan@bigdigdata.com>", "Zbynek Vyhlas <zbyneksmail@gmail.com>"]
 license = "MIT"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"Topic :: Software Development :: Libraries"
 ]
@@ -44,15 +44,15 @@
 
 [tool.poetry.scripts]
 nibbler-eat = 'celus_nibbler.__main__:main'
 
 [tool.poetry.dependencies]
 python = "^3.8.9"
 
-celus-nigiri = "~2.0.0"
+celus-nigiri = "~2.1.0"
 diskcache = "~5.6.0"
 nltk = "~3.8.1"
 pydantic = "~2.6.4"
 python-dateutil = "~2.9.0"
 openpyxl = "~3.1.2"
 unidecode = "~1.3.7"
 isbnlib = "~3.10.14"
```

### Comparing `celus_nibbler-11.0.0/PKG-INFO` & `celus_nibbler-11.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: celus-nibbler
-Version: 11.0.0
+Version: 11.1.0
 Summary: Counter-like data reader and processor.
 License: MIT
 Keywords: parsing,counter5
 Author: Stepan Henek
 Author-email: stepan@bigdigdata.com
 Requires-Python: >=3.8.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: xls
-Requires-Dist: celus-nigiri (>=2.0.0,<2.1.0)
+Requires-Dist: celus-nigiri (>=2.1.0,<2.2.0)
 Requires-Dist: diskcache (>=5.6.0,<5.7.0)
 Requires-Dist: isbnlib (>=3.10.14,<3.11.0)
 Requires-Dist: nltk (>=3.8.1,<3.9.0)
 Requires-Dist: openpyxl (>=3.1.2,<3.2.0)
 Requires-Dist: pydantic (>=2.6.4,<2.7.0)
 Requires-Dist: python-dateutil (>=2.9.0,<2.10.0)
 Requires-Dist: typing-extensions (>=4.10.0,<4.11.0)
```

