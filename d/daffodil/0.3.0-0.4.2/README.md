# Comparing `tmp/daffodil-0.3.0.tar.gz` & `tmp/daffodil-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daffodil-0.3.0.tar", last modified: Sun Apr 14 21:33:25 2024, max compression
+gzip compressed data, was "daffodil-0.4.2.tar", last modified: Thu May  2 03:52:56 2024, max compression
```

## Comparing `daffodil-0.3.0.tar` & `daffodil-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 21:33:25.799924 daffodil-0.3.0/
-drwxrwxrwx   0        0        0        0 2024-04-14 21:33:25.791931 daffodil-0.3.0/Daffodil.egg-info/
--rw-rw-rw-   0        0        0    50162 2024-04-14 21:33:25.000000 daffodil-0.3.0/Daffodil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2024-04-14 21:33:25.000000 daffodil-0.3.0/Daffodil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 21:33:25.000000 daffodil-0.3.0/Daffodil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-14 21:33:25.000000 daffodil-0.3.0/Daffodil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-14 21:33:25.000000 daffodil-0.3.0/Daffodil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.3.0/LICENSE
--rw-rw-rw-   0        0        0    50162 2024-04-14 21:33:25.796925 daffodil-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    49512 2024-04-12 21:24:34.000000 daffodil-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 21:33:25.785425 daffodil-0.3.0/lib/
--rw-rw-rw-   0        0        0        4 2024-03-01 21:59:22.000000 daffodil-0.3.0/lib/__init__.py
--rw-rw-rw-   0        0        0    43076 2024-03-01 21:59:22.000000 daffodil-0.3.0/lib/daf_indexing.py
--rw-rw-rw-   0        0        0    31511 2024-03-13 19:29:45.000000 daffodil-0.3.0/lib/daf_md.py
--rw-rw-rw-   0        0        0     7580 2024-03-13 19:01:32.000000 daffodil-0.3.0/lib/daf_pandas.py
--rw-rw-rw-   0        0        0     5327 2024-03-23 00:09:19.000000 daffodil-0.3.0/lib/daf_types.py
--rw-rw-rw-   0        0        0    46595 2024-03-23 00:31:44.000000 daffodil-0.3.0/lib/daf_utils.py
--rw-rw-rw-   0        0        0     5796 2024-03-01 21:59:22.000000 daffodil-0.3.0/lib/md_demo.py
--rw-rw-rw-   0        0        0       86 2024-04-14 21:25:39.000000 daffodil-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 21:33:25.799924 daffodil-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      895 2024-04-14 21:25:39.000000 daffodil-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 21:33:25.788394 daffodil-0.3.0/tests/
--rw-rw-rw-   0        0        0   164370 2024-04-14 19:08:24.000000 daffodil-0.3.0/tests/test_daf.py
+drwxrwxrwx   0        0        0        0 2024-05-02 03:52:56.530249 daffodil-0.4.2/
+-rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0    54014 2024-05-02 03:52:56.527255 daffodil-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0    53364 2024-05-01 01:35:13.000000 daffodil-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 03:52:56.524249 daffodil-0.4.2/daffodil.egg-info/
+-rw-rw-rw-   0        0        0    54014 2024-05-02 03:52:56.000000 daffodil-0.4.2/daffodil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-02 03:52:56.000000 daffodil-0.4.2/daffodil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 03:52:56.000000 daffodil-0.4.2/daffodil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-02 03:52:56.000000 daffodil-0.4.2/daffodil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 03:52:56.000000 daffodil-0.4.2/daffodil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      766 2024-05-02 03:32:58.000000 daffodil-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 03:52:56.530249 daffodil-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      903 2024-05-02 03:32:58.000000 daffodil-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 03:52:56.521252 daffodil-0.4.2/tests/
+-rw-rw-rw-   0        0        0   164640 2024-05-02 03:32:58.000000 daffodil-0.4.2/tests/test_daf.py
```

### Comparing `daffodil-0.3.0/Daffodil.egg-info/PKG-INFO` & `daffodil-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daffodil
-Version: 0.3.0
+Version: 0.4.2
 Summary: Daffodil provides lightweight and fast 2-D dataframes
 Home-page: https://github.com/raylutz/daffodil
 Author: Ray Lutz
 Author-email: raylutz@cognisys.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
@@ -40,28 +40,28 @@
 ![pydf_table](https://github.com/raylutz/daffodil/assets/14955977/05c54a27-8d8e-47b6-ae73-957709a5d398)
 
 Daffodil uses standard python data types, and can mix data types in rows and columns, and can store any type 
 within a cell, even another Daffodil instance. 
 
 It works well in traditional Pythonic processing paradigms, such as in loops, allowing fast row appends, 
 insertions and other operations that column-oriented packages like Pandas handle poorly or don't offer at all.
-Selecting, inserting, appending rows does not make a copy of the data but uses references and works the way 
+Selecting, inserting, appending rows does not make a copy of the data but uses references the way 
 Python normally does, leveraging the inherent power of Python without replacing it.
 
 Daffodil offers row-based apply and reduce functions, including support for chunked large data sets that can be described 
 by a Daffodil table which operates as a manifest to chunks, and useful for delegations for parallel processing, 
 where each delegation can handle a number of chunks.
 
 Daffodil is a very simple 'bare metal' class that is well suited for those situations where pure number crunching is not 
 the main objective. But it is also very compatible with other dataframe packages and can provide great way 
 to build and clean the data before providing the data to other packages for number crunching.
 
 Tabular data is commonly built
 record-by-record, while popular analysis and manipulation tools are oriented to work on data columns once
-it is fully assembled. If only a very few data operations are performed on columns (such as a sums, stdev, etc.)
+it is fully assembled. If only a very few data operations are performed (say < 30) on columns (such as a sums, stdev, etc.)
 then it is frequently more performant to leave it in row format rather than reforming it into columns and enduring
 the delays of porting and converting the data to those other packages.
 
 Spreadsheet-like operations are also provided, which are useful for processing the entire array with the same formula template,
 and can avoid glue code for many transformations. Python equations in the formula pane operate on the data
 pane and calculations from spreadsheet programs can be easily ported in, to avoid random glue code.
 
@@ -145,22 +145,25 @@
 Column names must be hashable and unique, and other than that, there are no firm restrictions.  
 (However, to use the interface with SQLite, avoid using the double underscore "__" in the names, which is used to 
 allow arbitrary names in SQLite.)
     
 When reading CSV files, the header is normally taken from the first (non-comment) line. If "user_format" is 
 specified on reading csv files, the csv data will be pre-processed and "comment" lines starting with # are removed.
 
+<!--
 Daffodil supports CSVJ, which is a mix of CSV with JSON metadata in comment fields in the first few lines of the file, 
 to provide data type, formatting, and other information. Using CSVJ speeds importing CSV data into a Daffodil instance 
 because the data can be converted to the appropriate type as it is read, and therefore avoids a second pass to convert 
 data from str type, which is the default. This also may unflatten objects. (CSVJ not supported yet).
+-->
 
 In some cases, you may be working with CSV files without a header line providing of column names. This is common
 in xlsx spreadsheets which have column names set by position. Setting noheader=True avoids 
-capturing the column names from the header line from csv input, and then column names will not be defined.
+capturing the column names from the header line from csv input, and then column names will not be defined, but can
+be defined in code.
 
 If columns repeated or are missing, this will be detected when first read, and the header row will be adjusted
 so it can be used. If any column name is blank, then these are named "colN" (or any other prefix you may prefer) 
 where N is the column number staring at 0. If there
 are duplicates, then the duplicate name is named "duplicatename_N", where 'duplicatename' is the original name
 and N is the column number. If you don't want this behavior, then use noheader=True and handle definition of the 
 'cols' parameter yourself.
@@ -234,56 +237,145 @@
 Other column operations such as statistics are not as performant as column-based packages but in those cases when
 many operations are required, the appropriate portion of the array can be ported to NumPy, Pandas, or any other dataframe package.
 
 Also, rows can be conceptually treated as if they are columns, because the structure of a Daffodil array is transposition symmetrical. Simply
 place column data in each row and name the row with the column name. To sum values in a column, then the values in each row, which is a 
 list, can be summed with the sum() operator.
 
+## Datatypes and conversion
+
+### data typing and conversion
+        
+Since we are using Python data objects, each cell in the array can have a different data type. However, it is useful to 
+convert data when it is first read from a csv file to make sure it is handled correctly. CSV files, by default, provide
+character data and therefore, without conversion, will provide `str` data. 
+        
+Data which is missing is provided as null strings, which will be ignored in apply or reduce operations. When converted to 
+other forms, such as a NumPy array, these values will be expressed as missing data using NAN or other indicators. 
+Daffodil uses null strings because they will print correctly when viewed, rather than seeing the distracting NAN indicators.
+
+Data type conversion is mainly an issue when converting from/to .csv file formats. In many cases, type conversions of the entire
+file may be avoided, so it is handled explicitly. `dtypes` is a dictionary where each column can have a Python type expressed, such as
+`str`, `int`, `float`, `dict`, `list`. 
+
+### .apply_dtypes(dtypes, unflatten, from_str)
+
+When data is read from a `.csv` file, it is parsed into `str` objects, as this is the fastest possible way to load data from such a file.
+The `.apply_dtypes()` method is used to convert all or some of the columns to the appropriate type. This conversion is done "in place"
+and a new array is not created. Thus, if only a limited number of columns is converted, it will not disturb the other columns for 
+best performance.
+
+If `from_str` is True (the default), only non-`str` columns are converted. Otherwise, columns specified as `str` will 
+also be scanned to ensure that they are expressed as `str` types.
+
+If `unflatten` is True (the default), columns with `list` or `dict` types will be unflattened from JSON if possible to create 
+accurate internal object types. (Tuples are not directly supported due to the use of JSON and will be imported as lists).
+
+If the `.apply_dtypes()` method is called with a `dtypes` argument, then if the Daf object does not have any dtypes defined, 
+the `dtypes` parameter will be used to initiallize the internal `dtypes` attribute and 
+the columns will be defined accordingly. However, if the `dtypes` attribute is already defined as non-empty, 
+then the `dtypes` dictionary argument is used to define which columns will be included in the operation.
+
+To apply dtypes to a .csv file, then the following syntax can be used:
+
+    my_daf = Daf.from_csv('filename.csv').apply_dtypes(dtypes=my_daf_dtypes)
+    
+which will convert all non-`str` types and unflatten JSON encoded `dict` and `list` values. Here, any `str` data is left alone.
+
+The explicit nature of the `.apply_dtypes()` method makes it feasible to avoid any conversion if say only `str` formatted columns
+are needed, and improve performance, and the operation of conversion of types is easy to understand.
+
+### .flatten()
+
+Prior to writing a file, if the Daf array has any `list` or `dict` objects, then the `.flatten()` method should be used prior to
+writing it. Also, this converts `bool` data to `1` and `0` to avoid the overhead of `True` and `False` in the `.csv` file. 
+
+    my_daf.flatten().to_csv('filename.csv')
+    
+or alternatively:
+
+    my_daf.to_csv('filename.csv', flatten=True)
+    
+### .to_list(), .to_dict(), .to_value()
+
+When selecting a single row or column in a Daf array, it will be returned normally as another Daf object.
+However, you can use `.to_list()` to convert it to a single list of values, or `.to_dict()` to get a dictionary,
+with keys set as the column names. If a single cell is selected, use .to_value() to obtain that single value.
+
+### .retmode
+
+A Daf object also has the attribute `.retmode` which can be either 'obj' (default) or 'val'
+If set to 'obj', then Daffodil objects are always produced from a selection operation. If set to 'val',
+then it will return a single value if a single cell is selected, or a list if a single row or column
+is selected.
+
+### example1
+
+For example, to sum all the values in a specific column, converting to a list will allow the python sum()
+operator to correctly sum the values. Caution: if the values must be numeric types.
+
+    `total = sum(my_daf[:, 'this_column'].to_list())`
+    
+Note: for performance, use `reduce()` and process all columns at the same time if multiple columns are to be
+summed, for example, as this is much more peformant and is scalable to multiple `.csv` files.
+
+### example2
+
+In this example, we set the retmode to 'val' so individual or list values will result
+
+    my_daf.retmode = 'val'
+    
+    `total_one = my_daf[3,4] + my_daf[5,6] * 10`
+
+    `total_two = sum(my_daf[:, 'this_column'])
+
+       
 ## Common Usage Pattern
        
-One common usage pattern allows iteration over the rows and appending to another instance. For example:
+One common usage pattern allows iteration over the rows and appending to another Daf instance. For example:
     
-        # read csv file into 2-D array, handling column headers and unflattening
-        my_daf = Daf.from_csv(file_path, unflatten=True)  
+        # read csv file into 2-D array, handling column headers, respecting data types and unflattening
+        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
     
         # create a new (empty) table to be built as we scan the input.
         new_daf = Daf()
         
         # scan the input my_daf row by row and construct the output. Pandas can't do this efficiently.
         for original_row in my_daf:  
             new_row = transform_row(original_row)
             new_daf.append(new_row)                
             # appending is no problem in Daffodil. Pandas will emit a future warning that appending is deprecated.
+            # here the column names are initialized as the first dictionary is appended.
             
         # create a flat csv file with any python objects flattened using JSON.
-        new_daf.to_csv(file_path, flatten=True)        
+        new_daf.flatten().to_csv(file_path)        
 
 This common pattern can be abbreviated using the apply() method:
 
-        my_daf = Daf.from_csv(file_path, unflatten=True)
+        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
         
         new_daf = my_daf.apply(transform_row)
         
-        new_daf.to_csv(file_path, flatten=True)
+        new_daf.flatten().to_csv(file_path)
 
 Or
 
-        Daf.from_csv(file_path).apply(transform_row).to_csv(file_path)
+        Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes).apply(transform_row).flatten().to_csv(file_path)
 
 And further extension of this pattern can apply the transformation to a set of csv files described by a chunk_manifest.
 The chunk manifest essentially provides metadata and instructions for accessing the source data, which may be many 1000s
 of chunks, each of which will fit in memory.
 
         chunk_manifest_daf = Daf.from_csv(file_path)  
         result_manifest_daf = chunk_manifest_daf.manifest_apply(transform_row)
 
 Similarly, a set of csv_files can be reduced to a single record using a reduction method. For example, 
 for determining valuecounts of columns in a set of files:
 
-        chunk_manifest_daf = Daf.from_csv(file_path, unflatten=True)
+        chunk_manifest_daf = Daf.from_csv(file_path)
         result_record = chunk_manifest_daf.manifest_reduce(count_values)
         
 Daffodil actually extends to chunks very elegantly because the apply() or reduce() operators can be applied to the
 rows and to chunks just as well. In contrast, column-based schemes require many passes through the data or delayed
 "lazy" operations that are difficult to comprehend.        
         
     
@@ -337,32 +429,14 @@
     len(daf)
         Provide the number of rows currently used by the data array.
 
     bool(my_daf)   # True only if my_daf exists and is not empty.
     
     (rows, cols) = daf.shape()   # Provide the current size of the data array.
     
-### data typing and conversion
-        
-Since we are using Python data objects, each cell in the array can have a different data type. However, it is useful to 
-convert data when it is first read from a csv file to make sure it is handled correctly. CSV files, by default, provide
-character data and therefore, without conversion, will provide `str` data. 
-        
-`dtypes` is a dict that specifies the datatype for each column, and if provided, will convert the data as it is initially read
-from the source. Other sources of data will normally provide the data type when it is imported.
-    
-When reading flat csv files, if `unflatten` is specified and `dtypes` specifies a list or a dict, then the data in those columns 
-will be converted from JSON to produce the list or dict object.
-
-Data which is missing is provided as null strings, which will be ignored in apply or reduce operations, and when converted to 
-other forms, like NumPy, will be expressed as missing data using NAN or other indicators. We use null strings because they will
-print correctly when viewed, rather than seeing the distracting NAN indicators.
-
-Daffodil supports the CSVJ file format, which includes a set of initial comments that are valid JSON to describe metdata and 
-data types. A CSVJ file is generally also a valid CSV file with # comment lines.
 
 
 ### creation and conversion
 
     Daf() -- Create a new daffodil instance.
         parameters:
             lol:        Optional[T_lola]        = None,     # Optional List[List[Any]] to initialize the data array. 
@@ -377,15 +451,18 @@
 
 #### create empty daf with nothing specified.
     
     my_daf = Daf()
 
 #### create empty daf with specified cols and keyfield, and with dtypes defined.
     
-    my_daf = Daf(cols=list_of_colnames, keyfield=fieldname, dtypes=dtype_dict) 
+    my_daf = Daf(cols=list_of_colnames, keyfield=fieldname, dtypes=dtype_dict)
+    
+Note that although dtypes may be defined, conversion of types can be an expensive
+operation and so it is done explicitly, using the `apply_dtypes()' method.    
     
 #### create empty daf with only keyfield specified.
     
     my_daf = Daf(keyfield=fieldname)
 
 #### create an empty daf object with same cols and keyfield.
     
@@ -460,53 +537,53 @@
 - If only one row is selected, return a list.
 - if only one col is selected, return a list.
 - if multiple columns are specified, they will be returned in the original orientation in a consistent daf instance copied from the original, and with the data specified.
 
 Please note: operations on columns is relatively inefficient. Try to avoid working on one column at a time.
 Instead, use .apply() or .reduce() and handle any manipulations of all columns at the same time, and select them with the cols parameter at that time.
 
-      my_daf[2, 3]     -- select cell at row 2, col 3 and return value.
-      my_daf[2]        -- select row 2, including all columns, return a list.
-      my_daf[2, :]     -- same as above
-      my_daf[-1, :]    -- select the last row
-      my_daf[:5]       -- select first 5 rows; like `head()` in other dataframe packages.
-      my_daf[:-5]      -- select last 5 rows; like `tail()` in other dataframe packages.
-      my_daf[:, 3]     -- select only column 3, including all rows. Return a list.
-      my_daf[:, 'C']   -- select only column named 'C', including all rows, return a list.
-      my_daf[2:4]      -- select rows 2 and 3, including all columns, return as daf.
-      my_daf[2:4, :]   -- same as above
-      my_daf[:, 3:5]   -- select columns 3 and 4, including all rows, return as daf.
-      my_daf[[2,4,6]]  -- return rows with indices 2,4,6 as daf array.
-      my_daf[:, [1,3,5]] -- return columns with indices 1,3,5 as daf array.
-      my_daf[['row5','row6','row7']] -- return rows with keyfield values 'row5','row6','row7'
-      my_daf[:, ['col1', 'col3', 'col5']] -- return columns with column names 'col1', 'col3', 'col5'
-      my_daf[('row5','row49'), :]] -- return rows with keyfield values 'row5' through 'row49' inclusive (note: column idx is required)
-      my_daf[('row5',), :]] -- return rows with keyfield values 'row5' through the end (note: column idx is required)
-      my_daf[(,'row49'), :]] -- return rows with keyfield values from the first row through 'row49' inclusive (note: column idx is required)
-      my_daf[:, ('col5', 'col23')]] -- return columns with column names from 'col5', through 'col23' inclusive
-      my_daf[:, (, 'col23')]] -- return columns with column names from the first column through 'col23' inclusive
-      my_daf[:, ('col23',)]] -- return columns with column names from 'col23', through the end
+      `my_daf[2, 3]`     -- select cell at row 2, col 3 and return value.
+      `my_daf[2]`        -- select row 2, including all columns, return a list.
+      `my_daf[2, :]`     -- same as above
+      `my_daf[-1, :]`    -- select the last row
+      `my_daf[:5]`       -- select first 5 rows; like `head()` in other dataframe packages.
+      `my_daf[:-5]`      -- select last 5 rows; like `tail()` in other dataframe packages.
+      `my_daf[:, 3]`     -- select only column 3, including all rows. Return a list.
+      `my_daf[:, 'C']`   -- select only column named 'C', including all rows, return a list.
+      `my_daf[2:4]`      -- select rows 2 and 3, including all columns, return as daf.
+      `my_daf[2:4, :]`   -- same as above
+      `my_daf[:, 3:5]`   -- select columns 3 and 4, including all rows, return as daf.
+      `my_daf[[2,4,6]]`  -- return rows with indices 2,4,6 as daf array.
+      `my_daf[:, [1,3,5]]` -- return columns with indices 1,3,5 as daf array.
+      `my_daf[['row5','row6','row7']]` -- return rows with keyfield values 'row5','row6','row7'
+      `my_daf[:, ['col1', 'col3', 'col5']]` -- return columns with column names 'col1', 'col3', 'col5'
+      `my_daf[('row5','row49'), :]]` -- return rows with keyfield values 'row5' through 'row49' inclusive (note: column idx is required)
+      `my_daf[('row5',), :]]` -- return rows with keyfield values 'row5' through the end (note: column idx is required)
+      `my_daf[(,'row49'), :]]` -- return rows with keyfield values from the first row through 'row49' inclusive (note: column idx is required)
+      `my_daf[:, ('col5', 'col23')]]` -- return columns with column names from 'col5', through 'col23' inclusive
+      `my_daf[:, (, 'col23')]]` -- return columns with column names from the first column through 'col23' inclusive
+      `my_daf[:, ('col23',)]]` -- return columns with column names from 'col23', through the end
 
 
 Please note that if you want to index rows by a keyfield or index columns using column names that are integers, 
 then you must use method calls. The square-bracket indexing will assume any integers are indices, not names.
 The integer values shown in the examples below do not index the array directly, but choose the row or columns by name.
 To choose by row keys (krows), then keyfield must be set. To choose by column keys (kcols), cols must be set.
 
-      my_daf.select_krows(krows = 123)  -- return daf with one row with integer 123 in keyfield column.
-      my_daf.select_krows(krows = [123, 456])  -- return daf with two rows selected by with integers in the keyfield column.
-      my_daf.select_krows(krows = [123, 456], inverse=True)   -- return daf dropping two rows selected by with integers in the keyfield column.
-      my_daf.select_krows(krows = (123, ), inverse=True)   -- drop all rows starting with row named 123 to the end.
-      my_daf.select_krows(krows = (, 123), inverse=True)   -- drop all rows from the first through row named 123.
+    `my_daf.select_krows(krows = 123)`  -- return daf with one row with integer 123 in keyfield column.
+    `my_daf.select_krows(krows = [123, 456])`  -- return daf with two rows selected by with integers in the keyfield column.
+    `my_daf.select_krows(krows = [123, 456], inverse=True)`   -- return daf dropping two rows selected by with integers in the keyfield column.
+    `my_daf.select_krows(krows = (123, ), inverse=True)`   -- drop all rows starting with row named 123 to the end.
+    `my_daf.select_krows(krows = (, 123), inverse=True)`   -- drop all rows from the first through row named 123.
      
-      my_daf.select_kcols(kcols = 123)  -- return daf of column named 123 (integer), placed in col 0
-      my_daf.select_kcols(kcols = 123).to_list()  -- return list of column named 123 (integer).
-      my_daf.select_kcols(kcols = 123).to_list(unique=True)  -- return list with one column with integer 123 colname, and remove duplicates.
-      my_daf.select_kcols(kcols = 123, inverse=True)   -- drop column with name 123
-      my_daf.select_kcols(kcols = 123, inverse=True, flip=True)   -- drop column with name 123 and transpose columns to rows.
+    `my_daf.select_kcols(kcols = 123)`  -- return daf of column named 123 (integer), placed in col 0
+    `my_daf.select_kcols(kcols = 123).to_list()`  -- return list of column named 123 (integer).
+    `my_daf.select_kcols(kcols = 123).to_list(unique=True)`  -- return list with one column with integer 123 colname, and remove duplicates.
+    `my_daf.select_kcols(kcols = 123, inverse=True)`   -- drop column with name 123
+    `my_daf.select_kcols(kcols = 123, inverse=True, flip=True)`   -- drop column with name 123 and transpose columns to rows.
 
 There are also similar methods for selecting rows and cols by indexes. Selecting rows using select_irows(rows_spec) is the same as my_daf[row_spec],
 except the parameter inverse is available to drop rows rather than keeping them.
 
     my_daf.select_irows(irows=10)                  -- select single row 10. Same as my_daf[10].
     my_daf.select_irows(irows=10, inverse=True)    -- drop single row 10. Same as my_daf[10].
     my_daf.select_irows(irows=[1,2,3,45])          -- select rows 1,2,3, and 45 using indices. Same as my_daf[[1,2,3,45]].
```

### Comparing `daffodil-0.3.0/LICENSE` & `daffodil-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `daffodil-0.3.0/PKG-INFO` & `daffodil-0.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: daffodil
-Version: 0.3.0
-Summary: Daffodil provides lightweight and fast 2-D dataframes
-Home-page: https://github.com/raylutz/daffodil
-Author: Ray Lutz
-Author-email: raylutz@cognisys.com
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: xlsx2csv==0.8.2
-Requires-Dist: Markdown==3.4.1
-Provides-Extra: numpy
-Requires-Dist: numpy; extra == "numpy"
-
 ![daffodil_logo](https://github.com/raylutz/daffodil/assets/14955977/5e141583-0216-429d-9ba8-be938aa13017)
 
 # Python Daffodil
 
 The Python Daffodil (DAtaFrames For Optimized Data Inspection and Logical processing) package provides
 lightweight, simple and flexible 2-d dataframes built on 
 python data types, including a list-of-list array as the core datatype. Daffodil is similar to other data frame
@@ -40,28 +20,28 @@
 ![pydf_table](https://github.com/raylutz/daffodil/assets/14955977/05c54a27-8d8e-47b6-ae73-957709a5d398)
 
 Daffodil uses standard python data types, and can mix data types in rows and columns, and can store any type 
 within a cell, even another Daffodil instance. 
 
 It works well in traditional Pythonic processing paradigms, such as in loops, allowing fast row appends, 
 insertions and other operations that column-oriented packages like Pandas handle poorly or don't offer at all.
-Selecting, inserting, appending rows does not make a copy of the data but uses references and works the way 
+Selecting, inserting, appending rows does not make a copy of the data but uses references the way 
 Python normally does, leveraging the inherent power of Python without replacing it.
 
 Daffodil offers row-based apply and reduce functions, including support for chunked large data sets that can be described 
 by a Daffodil table which operates as a manifest to chunks, and useful for delegations for parallel processing, 
 where each delegation can handle a number of chunks.
 
 Daffodil is a very simple 'bare metal' class that is well suited for those situations where pure number crunching is not 
 the main objective. But it is also very compatible with other dataframe packages and can provide great way 
 to build and clean the data before providing the data to other packages for number crunching.
 
 Tabular data is commonly built
 record-by-record, while popular analysis and manipulation tools are oriented to work on data columns once
-it is fully assembled. If only a very few data operations are performed on columns (such as a sums, stdev, etc.)
+it is fully assembled. If only a very few data operations are performed (say < 30) on columns (such as a sums, stdev, etc.)
 then it is frequently more performant to leave it in row format rather than reforming it into columns and enduring
 the delays of porting and converting the data to those other packages.
 
 Spreadsheet-like operations are also provided, which are useful for processing the entire array with the same formula template,
 and can avoid glue code for many transformations. Python equations in the formula pane operate on the data
 pane and calculations from spreadsheet programs can be easily ported in, to avoid random glue code.
 
@@ -145,22 +125,25 @@
 Column names must be hashable and unique, and other than that, there are no firm restrictions.  
 (However, to use the interface with SQLite, avoid using the double underscore "__" in the names, which is used to 
 allow arbitrary names in SQLite.)
     
 When reading CSV files, the header is normally taken from the first (non-comment) line. If "user_format" is 
 specified on reading csv files, the csv data will be pre-processed and "comment" lines starting with # are removed.
 
+<!--
 Daffodil supports CSVJ, which is a mix of CSV with JSON metadata in comment fields in the first few lines of the file, 
 to provide data type, formatting, and other information. Using CSVJ speeds importing CSV data into a Daffodil instance 
 because the data can be converted to the appropriate type as it is read, and therefore avoids a second pass to convert 
 data from str type, which is the default. This also may unflatten objects. (CSVJ not supported yet).
+-->
 
 In some cases, you may be working with CSV files without a header line providing of column names. This is common
 in xlsx spreadsheets which have column names set by position. Setting noheader=True avoids 
-capturing the column names from the header line from csv input, and then column names will not be defined.
+capturing the column names from the header line from csv input, and then column names will not be defined, but can
+be defined in code.
 
 If columns repeated or are missing, this will be detected when first read, and the header row will be adjusted
 so it can be used. If any column name is blank, then these are named "colN" (or any other prefix you may prefer) 
 where N is the column number staring at 0. If there
 are duplicates, then the duplicate name is named "duplicatename_N", where 'duplicatename' is the original name
 and N is the column number. If you don't want this behavior, then use noheader=True and handle definition of the 
 'cols' parameter yourself.
@@ -234,56 +217,145 @@
 Other column operations such as statistics are not as performant as column-based packages but in those cases when
 many operations are required, the appropriate portion of the array can be ported to NumPy, Pandas, or any other dataframe package.
 
 Also, rows can be conceptually treated as if they are columns, because the structure of a Daffodil array is transposition symmetrical. Simply
 place column data in each row and name the row with the column name. To sum values in a column, then the values in each row, which is a 
 list, can be summed with the sum() operator.
 
+## Datatypes and conversion
+
+### data typing and conversion
+        
+Since we are using Python data objects, each cell in the array can have a different data type. However, it is useful to 
+convert data when it is first read from a csv file to make sure it is handled correctly. CSV files, by default, provide
+character data and therefore, without conversion, will provide `str` data. 
+        
+Data which is missing is provided as null strings, which will be ignored in apply or reduce operations. When converted to 
+other forms, such as a NumPy array, these values will be expressed as missing data using NAN or other indicators. 
+Daffodil uses null strings because they will print correctly when viewed, rather than seeing the distracting NAN indicators.
+
+Data type conversion is mainly an issue when converting from/to .csv file formats. In many cases, type conversions of the entire
+file may be avoided, so it is handled explicitly. `dtypes` is a dictionary where each column can have a Python type expressed, such as
+`str`, `int`, `float`, `dict`, `list`. 
+
+### .apply_dtypes(dtypes, unflatten, from_str)
+
+When data is read from a `.csv` file, it is parsed into `str` objects, as this is the fastest possible way to load data from such a file.
+The `.apply_dtypes()` method is used to convert all or some of the columns to the appropriate type. This conversion is done "in place"
+and a new array is not created. Thus, if only a limited number of columns is converted, it will not disturb the other columns for 
+best performance.
+
+If `from_str` is True (the default), only non-`str` columns are converted. Otherwise, columns specified as `str` will 
+also be scanned to ensure that they are expressed as `str` types.
+
+If `unflatten` is True (the default), columns with `list` or `dict` types will be unflattened from JSON if possible to create 
+accurate internal object types. (Tuples are not directly supported due to the use of JSON and will be imported as lists).
+
+If the `.apply_dtypes()` method is called with a `dtypes` argument, then if the Daf object does not have any dtypes defined, 
+the `dtypes` parameter will be used to initiallize the internal `dtypes` attribute and 
+the columns will be defined accordingly. However, if the `dtypes` attribute is already defined as non-empty, 
+then the `dtypes` dictionary argument is used to define which columns will be included in the operation.
+
+To apply dtypes to a .csv file, then the following syntax can be used:
+
+    my_daf = Daf.from_csv('filename.csv').apply_dtypes(dtypes=my_daf_dtypes)
+    
+which will convert all non-`str` types and unflatten JSON encoded `dict` and `list` values. Here, any `str` data is left alone.
+
+The explicit nature of the `.apply_dtypes()` method makes it feasible to avoid any conversion if say only `str` formatted columns
+are needed, and improve performance, and the operation of conversion of types is easy to understand.
+
+### .flatten()
+
+Prior to writing a file, if the Daf array has any `list` or `dict` objects, then the `.flatten()` method should be used prior to
+writing it. Also, this converts `bool` data to `1` and `0` to avoid the overhead of `True` and `False` in the `.csv` file. 
+
+    my_daf.flatten().to_csv('filename.csv')
+    
+or alternatively:
+
+    my_daf.to_csv('filename.csv', flatten=True)
+    
+### .to_list(), .to_dict(), .to_value()
+
+When selecting a single row or column in a Daf array, it will be returned normally as another Daf object.
+However, you can use `.to_list()` to convert it to a single list of values, or `.to_dict()` to get a dictionary,
+with keys set as the column names. If a single cell is selected, use .to_value() to obtain that single value.
+
+### .retmode
+
+A Daf object also has the attribute `.retmode` which can be either 'obj' (default) or 'val'
+If set to 'obj', then Daffodil objects are always produced from a selection operation. If set to 'val',
+then it will return a single value if a single cell is selected, or a list if a single row or column
+is selected.
+
+### example1
+
+For example, to sum all the values in a specific column, converting to a list will allow the python sum()
+operator to correctly sum the values. Caution: if the values must be numeric types.
+
+    `total = sum(my_daf[:, 'this_column'].to_list())`
+    
+Note: for performance, use `reduce()` and process all columns at the same time if multiple columns are to be
+summed, for example, as this is much more peformant and is scalable to multiple `.csv` files.
+
+### example2
+
+In this example, we set the retmode to 'val' so individual or list values will result
+
+    my_daf.retmode = 'val'
+    
+    `total_one = my_daf[3,4] + my_daf[5,6] * 10`
+
+    `total_two = sum(my_daf[:, 'this_column'])
+
+       
 ## Common Usage Pattern
        
-One common usage pattern allows iteration over the rows and appending to another instance. For example:
+One common usage pattern allows iteration over the rows and appending to another Daf instance. For example:
     
-        # read csv file into 2-D array, handling column headers and unflattening
-        my_daf = Daf.from_csv(file_path, unflatten=True)  
+        # read csv file into 2-D array, handling column headers, respecting data types and unflattening
+        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
     
         # create a new (empty) table to be built as we scan the input.
         new_daf = Daf()
         
         # scan the input my_daf row by row and construct the output. Pandas can't do this efficiently.
         for original_row in my_daf:  
             new_row = transform_row(original_row)
             new_daf.append(new_row)                
             # appending is no problem in Daffodil. Pandas will emit a future warning that appending is deprecated.
+            # here the column names are initialized as the first dictionary is appended.
             
         # create a flat csv file with any python objects flattened using JSON.
-        new_daf.to_csv(file_path, flatten=True)        
+        new_daf.flatten().to_csv(file_path)        
 
 This common pattern can be abbreviated using the apply() method:
 
-        my_daf = Daf.from_csv(file_path, unflatten=True)
+        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
         
         new_daf = my_daf.apply(transform_row)
         
-        new_daf.to_csv(file_path, flatten=True)
+        new_daf.flatten().to_csv(file_path)
 
 Or
 
-        Daf.from_csv(file_path).apply(transform_row).to_csv(file_path)
+        Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes).apply(transform_row).flatten().to_csv(file_path)
 
 And further extension of this pattern can apply the transformation to a set of csv files described by a chunk_manifest.
 The chunk manifest essentially provides metadata and instructions for accessing the source data, which may be many 1000s
 of chunks, each of which will fit in memory.
 
         chunk_manifest_daf = Daf.from_csv(file_path)  
         result_manifest_daf = chunk_manifest_daf.manifest_apply(transform_row)
 
 Similarly, a set of csv_files can be reduced to a single record using a reduction method. For example, 
 for determining valuecounts of columns in a set of files:
 
-        chunk_manifest_daf = Daf.from_csv(file_path, unflatten=True)
+        chunk_manifest_daf = Daf.from_csv(file_path)
         result_record = chunk_manifest_daf.manifest_reduce(count_values)
         
 Daffodil actually extends to chunks very elegantly because the apply() or reduce() operators can be applied to the
 rows and to chunks just as well. In contrast, column-based schemes require many passes through the data or delayed
 "lazy" operations that are difficult to comprehend.        
         
     
@@ -337,32 +409,14 @@
     len(daf)
         Provide the number of rows currently used by the data array.
 
     bool(my_daf)   # True only if my_daf exists and is not empty.
     
     (rows, cols) = daf.shape()   # Provide the current size of the data array.
     
-### data typing and conversion
-        
-Since we are using Python data objects, each cell in the array can have a different data type. However, it is useful to 
-convert data when it is first read from a csv file to make sure it is handled correctly. CSV files, by default, provide
-character data and therefore, without conversion, will provide `str` data. 
-        
-`dtypes` is a dict that specifies the datatype for each column, and if provided, will convert the data as it is initially read
-from the source. Other sources of data will normally provide the data type when it is imported.
-    
-When reading flat csv files, if `unflatten` is specified and `dtypes` specifies a list or a dict, then the data in those columns 
-will be converted from JSON to produce the list or dict object.
-
-Data which is missing is provided as null strings, which will be ignored in apply or reduce operations, and when converted to 
-other forms, like NumPy, will be expressed as missing data using NAN or other indicators. We use null strings because they will
-print correctly when viewed, rather than seeing the distracting NAN indicators.
-
-Daffodil supports the CSVJ file format, which includes a set of initial comments that are valid JSON to describe metdata and 
-data types. A CSVJ file is generally also a valid CSV file with # comment lines.
 
 
 ### creation and conversion
 
     Daf() -- Create a new daffodil instance.
         parameters:
             lol:        Optional[T_lola]        = None,     # Optional List[List[Any]] to initialize the data array. 
@@ -377,15 +431,18 @@
 
 #### create empty daf with nothing specified.
     
     my_daf = Daf()
 
 #### create empty daf with specified cols and keyfield, and with dtypes defined.
     
-    my_daf = Daf(cols=list_of_colnames, keyfield=fieldname, dtypes=dtype_dict) 
+    my_daf = Daf(cols=list_of_colnames, keyfield=fieldname, dtypes=dtype_dict)
+    
+Note that although dtypes may be defined, conversion of types can be an expensive
+operation and so it is done explicitly, using the `apply_dtypes()' method.    
     
 #### create empty daf with only keyfield specified.
     
     my_daf = Daf(keyfield=fieldname)
 
 #### create an empty daf object with same cols and keyfield.
     
@@ -460,53 +517,53 @@
 - If only one row is selected, return a list.
 - if only one col is selected, return a list.
 - if multiple columns are specified, they will be returned in the original orientation in a consistent daf instance copied from the original, and with the data specified.
 
 Please note: operations on columns is relatively inefficient. Try to avoid working on one column at a time.
 Instead, use .apply() or .reduce() and handle any manipulations of all columns at the same time, and select them with the cols parameter at that time.
 
-      my_daf[2, 3]     -- select cell at row 2, col 3 and return value.
-      my_daf[2]        -- select row 2, including all columns, return a list.
-      my_daf[2, :]     -- same as above
-      my_daf[-1, :]    -- select the last row
-      my_daf[:5]       -- select first 5 rows; like `head()` in other dataframe packages.
-      my_daf[:-5]      -- select last 5 rows; like `tail()` in other dataframe packages.
-      my_daf[:, 3]     -- select only column 3, including all rows. Return a list.
-      my_daf[:, 'C']   -- select only column named 'C', including all rows, return a list.
-      my_daf[2:4]      -- select rows 2 and 3, including all columns, return as daf.
-      my_daf[2:4, :]   -- same as above
-      my_daf[:, 3:5]   -- select columns 3 and 4, including all rows, return as daf.
-      my_daf[[2,4,6]]  -- return rows with indices 2,4,6 as daf array.
-      my_daf[:, [1,3,5]] -- return columns with indices 1,3,5 as daf array.
-      my_daf[['row5','row6','row7']] -- return rows with keyfield values 'row5','row6','row7'
-      my_daf[:, ['col1', 'col3', 'col5']] -- return columns with column names 'col1', 'col3', 'col5'
-      my_daf[('row5','row49'), :]] -- return rows with keyfield values 'row5' through 'row49' inclusive (note: column idx is required)
-      my_daf[('row5',), :]] -- return rows with keyfield values 'row5' through the end (note: column idx is required)
-      my_daf[(,'row49'), :]] -- return rows with keyfield values from the first row through 'row49' inclusive (note: column idx is required)
-      my_daf[:, ('col5', 'col23')]] -- return columns with column names from 'col5', through 'col23' inclusive
-      my_daf[:, (, 'col23')]] -- return columns with column names from the first column through 'col23' inclusive
-      my_daf[:, ('col23',)]] -- return columns with column names from 'col23', through the end
+      `my_daf[2, 3]`     -- select cell at row 2, col 3 and return value.
+      `my_daf[2]`        -- select row 2, including all columns, return a list.
+      `my_daf[2, :]`     -- same as above
+      `my_daf[-1, :]`    -- select the last row
+      `my_daf[:5]`       -- select first 5 rows; like `head()` in other dataframe packages.
+      `my_daf[:-5]`      -- select last 5 rows; like `tail()` in other dataframe packages.
+      `my_daf[:, 3]`     -- select only column 3, including all rows. Return a list.
+      `my_daf[:, 'C']`   -- select only column named 'C', including all rows, return a list.
+      `my_daf[2:4]`      -- select rows 2 and 3, including all columns, return as daf.
+      `my_daf[2:4, :]`   -- same as above
+      `my_daf[:, 3:5]`   -- select columns 3 and 4, including all rows, return as daf.
+      `my_daf[[2,4,6]]`  -- return rows with indices 2,4,6 as daf array.
+      `my_daf[:, [1,3,5]]` -- return columns with indices 1,3,5 as daf array.
+      `my_daf[['row5','row6','row7']]` -- return rows with keyfield values 'row5','row6','row7'
+      `my_daf[:, ['col1', 'col3', 'col5']]` -- return columns with column names 'col1', 'col3', 'col5'
+      `my_daf[('row5','row49'), :]]` -- return rows with keyfield values 'row5' through 'row49' inclusive (note: column idx is required)
+      `my_daf[('row5',), :]]` -- return rows with keyfield values 'row5' through the end (note: column idx is required)
+      `my_daf[(,'row49'), :]]` -- return rows with keyfield values from the first row through 'row49' inclusive (note: column idx is required)
+      `my_daf[:, ('col5', 'col23')]]` -- return columns with column names from 'col5', through 'col23' inclusive
+      `my_daf[:, (, 'col23')]]` -- return columns with column names from the first column through 'col23' inclusive
+      `my_daf[:, ('col23',)]]` -- return columns with column names from 'col23', through the end
 
 
 Please note that if you want to index rows by a keyfield or index columns using column names that are integers, 
 then you must use method calls. The square-bracket indexing will assume any integers are indices, not names.
 The integer values shown in the examples below do not index the array directly, but choose the row or columns by name.
 To choose by row keys (krows), then keyfield must be set. To choose by column keys (kcols), cols must be set.
 
-      my_daf.select_krows(krows = 123)  -- return daf with one row with integer 123 in keyfield column.
-      my_daf.select_krows(krows = [123, 456])  -- return daf with two rows selected by with integers in the keyfield column.
-      my_daf.select_krows(krows = [123, 456], inverse=True)   -- return daf dropping two rows selected by with integers in the keyfield column.
-      my_daf.select_krows(krows = (123, ), inverse=True)   -- drop all rows starting with row named 123 to the end.
-      my_daf.select_krows(krows = (, 123), inverse=True)   -- drop all rows from the first through row named 123.
+    `my_daf.select_krows(krows = 123)`  -- return daf with one row with integer 123 in keyfield column.
+    `my_daf.select_krows(krows = [123, 456])`  -- return daf with two rows selected by with integers in the keyfield column.
+    `my_daf.select_krows(krows = [123, 456], inverse=True)`   -- return daf dropping two rows selected by with integers in the keyfield column.
+    `my_daf.select_krows(krows = (123, ), inverse=True)`   -- drop all rows starting with row named 123 to the end.
+    `my_daf.select_krows(krows = (, 123), inverse=True)`   -- drop all rows from the first through row named 123.
      
-      my_daf.select_kcols(kcols = 123)  -- return daf of column named 123 (integer), placed in col 0
-      my_daf.select_kcols(kcols = 123).to_list()  -- return list of column named 123 (integer).
-      my_daf.select_kcols(kcols = 123).to_list(unique=True)  -- return list with one column with integer 123 colname, and remove duplicates.
-      my_daf.select_kcols(kcols = 123, inverse=True)   -- drop column with name 123
-      my_daf.select_kcols(kcols = 123, inverse=True, flip=True)   -- drop column with name 123 and transpose columns to rows.
+    `my_daf.select_kcols(kcols = 123)`  -- return daf of column named 123 (integer), placed in col 0
+    `my_daf.select_kcols(kcols = 123).to_list()`  -- return list of column named 123 (integer).
+    `my_daf.select_kcols(kcols = 123).to_list(unique=True)`  -- return list with one column with integer 123 colname, and remove duplicates.
+    `my_daf.select_kcols(kcols = 123, inverse=True)`   -- drop column with name 123
+    `my_daf.select_kcols(kcols = 123, inverse=True, flip=True)`   -- drop column with name 123 and transpose columns to rows.
 
 There are also similar methods for selecting rows and cols by indexes. Selecting rows using select_irows(rows_spec) is the same as my_daf[row_spec],
 except the parameter inverse is available to drop rows rather than keeping them.
 
     my_daf.select_irows(irows=10)                  -- select single row 10. Same as my_daf[10].
     my_daf.select_irows(irows=10, inverse=True)    -- drop single row 10. Same as my_daf[10].
     my_daf.select_irows(irows=[1,2,3,45])          -- select rows 1,2,3, and 45 using indices. Same as my_daf[[1,2,3,45]].
```

### Comparing `daffodil-0.3.0/README.md` & `daffodil-0.4.2/daffodil.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: daffodil
+Version: 0.4.2
+Summary: Daffodil provides lightweight and fast 2-D dataframes
+Home-page: https://github.com/raylutz/daffodil
+Author: Ray Lutz
+Author-email: raylutz@cognisys.com
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: xlsx2csv==0.8.2
+Requires-Dist: Markdown==3.4.1
+Provides-Extra: numpy
+Requires-Dist: numpy; extra == "numpy"
+
 ![daffodil_logo](https://github.com/raylutz/daffodil/assets/14955977/5e141583-0216-429d-9ba8-be938aa13017)
 
 # Python Daffodil
 
 The Python Daffodil (DAtaFrames For Optimized Data Inspection and Logical processing) package provides
 lightweight, simple and flexible 2-d dataframes built on 
 python data types, including a list-of-list array as the core datatype. Daffodil is similar to other data frame
@@ -20,28 +40,28 @@
 ![pydf_table](https://github.com/raylutz/daffodil/assets/14955977/05c54a27-8d8e-47b6-ae73-957709a5d398)
 
 Daffodil uses standard python data types, and can mix data types in rows and columns, and can store any type 
 within a cell, even another Daffodil instance. 
 
 It works well in traditional Pythonic processing paradigms, such as in loops, allowing fast row appends, 
 insertions and other operations that column-oriented packages like Pandas handle poorly or don't offer at all.
-Selecting, inserting, appending rows does not make a copy of the data but uses references and works the way 
+Selecting, inserting, appending rows does not make a copy of the data but uses references the way 
 Python normally does, leveraging the inherent power of Python without replacing it.
 
 Daffodil offers row-based apply and reduce functions, including support for chunked large data sets that can be described 
 by a Daffodil table which operates as a manifest to chunks, and useful for delegations for parallel processing, 
 where each delegation can handle a number of chunks.
 
 Daffodil is a very simple 'bare metal' class that is well suited for those situations where pure number crunching is not 
 the main objective. But it is also very compatible with other dataframe packages and can provide great way 
 to build and clean the data before providing the data to other packages for number crunching.
 
 Tabular data is commonly built
 record-by-record, while popular analysis and manipulation tools are oriented to work on data columns once
-it is fully assembled. If only a very few data operations are performed on columns (such as a sums, stdev, etc.)
+it is fully assembled. If only a very few data operations are performed (say < 30) on columns (such as a sums, stdev, etc.)
 then it is frequently more performant to leave it in row format rather than reforming it into columns and enduring
 the delays of porting and converting the data to those other packages.
 
 Spreadsheet-like operations are also provided, which are useful for processing the entire array with the same formula template,
 and can avoid glue code for many transformations. Python equations in the formula pane operate on the data
 pane and calculations from spreadsheet programs can be easily ported in, to avoid random glue code.
 
@@ -125,22 +145,25 @@
 Column names must be hashable and unique, and other than that, there are no firm restrictions.  
 (However, to use the interface with SQLite, avoid using the double underscore "__" in the names, which is used to 
 allow arbitrary names in SQLite.)
     
 When reading CSV files, the header is normally taken from the first (non-comment) line. If "user_format" is 
 specified on reading csv files, the csv data will be pre-processed and "comment" lines starting with # are removed.
 
+<!--
 Daffodil supports CSVJ, which is a mix of CSV with JSON metadata in comment fields in the first few lines of the file, 
 to provide data type, formatting, and other information. Using CSVJ speeds importing CSV data into a Daffodil instance 
 because the data can be converted to the appropriate type as it is read, and therefore avoids a second pass to convert 
 data from str type, which is the default. This also may unflatten objects. (CSVJ not supported yet).
+-->
 
 In some cases, you may be working with CSV files without a header line providing of column names. This is common
 in xlsx spreadsheets which have column names set by position. Setting noheader=True avoids 
-capturing the column names from the header line from csv input, and then column names will not be defined.
+capturing the column names from the header line from csv input, and then column names will not be defined, but can
+be defined in code.
 
 If columns repeated or are missing, this will be detected when first read, and the header row will be adjusted
 so it can be used. If any column name is blank, then these are named "colN" (or any other prefix you may prefer) 
 where N is the column number staring at 0. If there
 are duplicates, then the duplicate name is named "duplicatename_N", where 'duplicatename' is the original name
 and N is the column number. If you don't want this behavior, then use noheader=True and handle definition of the 
 'cols' parameter yourself.
@@ -214,56 +237,145 @@
 Other column operations such as statistics are not as performant as column-based packages but in those cases when
 many operations are required, the appropriate portion of the array can be ported to NumPy, Pandas, or any other dataframe package.
 
 Also, rows can be conceptually treated as if they are columns, because the structure of a Daffodil array is transposition symmetrical. Simply
 place column data in each row and name the row with the column name. To sum values in a column, then the values in each row, which is a 
 list, can be summed with the sum() operator.
 
+## Datatypes and conversion
+
+### data typing and conversion
+        
+Since we are using Python data objects, each cell in the array can have a different data type. However, it is useful to 
+convert data when it is first read from a csv file to make sure it is handled correctly. CSV files, by default, provide
+character data and therefore, without conversion, will provide `str` data. 
+        
+Data which is missing is provided as null strings, which will be ignored in apply or reduce operations. When converted to 
+other forms, such as a NumPy array, these values will be expressed as missing data using NAN or other indicators. 
+Daffodil uses null strings because they will print correctly when viewed, rather than seeing the distracting NAN indicators.
+
+Data type conversion is mainly an issue when converting from/to .csv file formats. In many cases, type conversions of the entire
+file may be avoided, so it is handled explicitly. `dtypes` is a dictionary where each column can have a Python type expressed, such as
+`str`, `int`, `float`, `dict`, `list`. 
+
+### .apply_dtypes(dtypes, unflatten, from_str)
+
+When data is read from a `.csv` file, it is parsed into `str` objects, as this is the fastest possible way to load data from such a file.
+The `.apply_dtypes()` method is used to convert all or some of the columns to the appropriate type. This conversion is done "in place"
+and a new array is not created. Thus, if only a limited number of columns is converted, it will not disturb the other columns for 
+best performance.
+
+If `from_str` is True (the default), only non-`str` columns are converted. Otherwise, columns specified as `str` will 
+also be scanned to ensure that they are expressed as `str` types.
+
+If `unflatten` is True (the default), columns with `list` or `dict` types will be unflattened from JSON if possible to create 
+accurate internal object types. (Tuples are not directly supported due to the use of JSON and will be imported as lists).
+
+If the `.apply_dtypes()` method is called with a `dtypes` argument, then if the Daf object does not have any dtypes defined, 
+the `dtypes` parameter will be used to initiallize the internal `dtypes` attribute and 
+the columns will be defined accordingly. However, if the `dtypes` attribute is already defined as non-empty, 
+then the `dtypes` dictionary argument is used to define which columns will be included in the operation.
+
+To apply dtypes to a .csv file, then the following syntax can be used:
+
+    my_daf = Daf.from_csv('filename.csv').apply_dtypes(dtypes=my_daf_dtypes)
+    
+which will convert all non-`str` types and unflatten JSON encoded `dict` and `list` values. Here, any `str` data is left alone.
+
+The explicit nature of the `.apply_dtypes()` method makes it feasible to avoid any conversion if say only `str` formatted columns
+are needed, and improve performance, and the operation of conversion of types is easy to understand.
+
+### .flatten()
+
+Prior to writing a file, if the Daf array has any `list` or `dict` objects, then the `.flatten()` method should be used prior to
+writing it. Also, this converts `bool` data to `1` and `0` to avoid the overhead of `True` and `False` in the `.csv` file. 
+
+    my_daf.flatten().to_csv('filename.csv')
+    
+or alternatively:
+
+    my_daf.to_csv('filename.csv', flatten=True)
+    
+### .to_list(), .to_dict(), .to_value()
+
+When selecting a single row or column in a Daf array, it will be returned normally as another Daf object.
+However, you can use `.to_list()` to convert it to a single list of values, or `.to_dict()` to get a dictionary,
+with keys set as the column names. If a single cell is selected, use .to_value() to obtain that single value.
+
+### .retmode
+
+A Daf object also has the attribute `.retmode` which can be either 'obj' (default) or 'val'
+If set to 'obj', then Daffodil objects are always produced from a selection operation. If set to 'val',
+then it will return a single value if a single cell is selected, or a list if a single row or column
+is selected.
+
+### example1
+
+For example, to sum all the values in a specific column, converting to a list will allow the python sum()
+operator to correctly sum the values. Caution: if the values must be numeric types.
+
+    `total = sum(my_daf[:, 'this_column'].to_list())`
+    
+Note: for performance, use `reduce()` and process all columns at the same time if multiple columns are to be
+summed, for example, as this is much more peformant and is scalable to multiple `.csv` files.
+
+### example2
+
+In this example, we set the retmode to 'val' so individual or list values will result
+
+    my_daf.retmode = 'val'
+    
+    `total_one = my_daf[3,4] + my_daf[5,6] * 10`
+
+    `total_two = sum(my_daf[:, 'this_column'])
+
+       
 ## Common Usage Pattern
        
-One common usage pattern allows iteration over the rows and appending to another instance. For example:
+One common usage pattern allows iteration over the rows and appending to another Daf instance. For example:
     
-        # read csv file into 2-D array, handling column headers and unflattening
-        my_daf = Daf.from_csv(file_path, unflatten=True)  
+        # read csv file into 2-D array, handling column headers, respecting data types and unflattening
+        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
     
         # create a new (empty) table to be built as we scan the input.
         new_daf = Daf()
         
         # scan the input my_daf row by row and construct the output. Pandas can't do this efficiently.
         for original_row in my_daf:  
             new_row = transform_row(original_row)
             new_daf.append(new_row)                
             # appending is no problem in Daffodil. Pandas will emit a future warning that appending is deprecated.
+            # here the column names are initialized as the first dictionary is appended.
             
         # create a flat csv file with any python objects flattened using JSON.
-        new_daf.to_csv(file_path, flatten=True)        
+        new_daf.flatten().to_csv(file_path)        
 
 This common pattern can be abbreviated using the apply() method:
 
-        my_daf = Daf.from_csv(file_path, unflatten=True)
+        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
         
         new_daf = my_daf.apply(transform_row)
         
-        new_daf.to_csv(file_path, flatten=True)
+        new_daf.flatten().to_csv(file_path)
 
 Or
 
-        Daf.from_csv(file_path).apply(transform_row).to_csv(file_path)
+        Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes).apply(transform_row).flatten().to_csv(file_path)
 
 And further extension of this pattern can apply the transformation to a set of csv files described by a chunk_manifest.
 The chunk manifest essentially provides metadata and instructions for accessing the source data, which may be many 1000s
 of chunks, each of which will fit in memory.
 
         chunk_manifest_daf = Daf.from_csv(file_path)  
         result_manifest_daf = chunk_manifest_daf.manifest_apply(transform_row)
 
 Similarly, a set of csv_files can be reduced to a single record using a reduction method. For example, 
 for determining valuecounts of columns in a set of files:
 
-        chunk_manifest_daf = Daf.from_csv(file_path, unflatten=True)
+        chunk_manifest_daf = Daf.from_csv(file_path)
         result_record = chunk_manifest_daf.manifest_reduce(count_values)
         
 Daffodil actually extends to chunks very elegantly because the apply() or reduce() operators can be applied to the
 rows and to chunks just as well. In contrast, column-based schemes require many passes through the data or delayed
 "lazy" operations that are difficult to comprehend.        
         
     
@@ -317,32 +429,14 @@
     len(daf)
         Provide the number of rows currently used by the data array.
 
     bool(my_daf)   # True only if my_daf exists and is not empty.
     
     (rows, cols) = daf.shape()   # Provide the current size of the data array.
     
-### data typing and conversion
-        
-Since we are using Python data objects, each cell in the array can have a different data type. However, it is useful to 
-convert data when it is first read from a csv file to make sure it is handled correctly. CSV files, by default, provide
-character data and therefore, without conversion, will provide `str` data. 
-        
-`dtypes` is a dict that specifies the datatype for each column, and if provided, will convert the data as it is initially read
-from the source. Other sources of data will normally provide the data type when it is imported.
-    
-When reading flat csv files, if `unflatten` is specified and `dtypes` specifies a list or a dict, then the data in those columns 
-will be converted from JSON to produce the list or dict object.
-
-Data which is missing is provided as null strings, which will be ignored in apply or reduce operations, and when converted to 
-other forms, like NumPy, will be expressed as missing data using NAN or other indicators. We use null strings because they will
-print correctly when viewed, rather than seeing the distracting NAN indicators.
-
-Daffodil supports the CSVJ file format, which includes a set of initial comments that are valid JSON to describe metdata and 
-data types. A CSVJ file is generally also a valid CSV file with # comment lines.
 
 
 ### creation and conversion
 
     Daf() -- Create a new daffodil instance.
         parameters:
             lol:        Optional[T_lola]        = None,     # Optional List[List[Any]] to initialize the data array. 
@@ -357,15 +451,18 @@
 
 #### create empty daf with nothing specified.
     
     my_daf = Daf()
 
 #### create empty daf with specified cols and keyfield, and with dtypes defined.
     
-    my_daf = Daf(cols=list_of_colnames, keyfield=fieldname, dtypes=dtype_dict) 
+    my_daf = Daf(cols=list_of_colnames, keyfield=fieldname, dtypes=dtype_dict)
+    
+Note that although dtypes may be defined, conversion of types can be an expensive
+operation and so it is done explicitly, using the `apply_dtypes()' method.    
     
 #### create empty daf with only keyfield specified.
     
     my_daf = Daf(keyfield=fieldname)
 
 #### create an empty daf object with same cols and keyfield.
     
@@ -440,53 +537,53 @@
 - If only one row is selected, return a list.
 - if only one col is selected, return a list.
 - if multiple columns are specified, they will be returned in the original orientation in a consistent daf instance copied from the original, and with the data specified.
 
 Please note: operations on columns is relatively inefficient. Try to avoid working on one column at a time.
 Instead, use .apply() or .reduce() and handle any manipulations of all columns at the same time, and select them with the cols parameter at that time.
 
-      my_daf[2, 3]     -- select cell at row 2, col 3 and return value.
-      my_daf[2]        -- select row 2, including all columns, return a list.
-      my_daf[2, :]     -- same as above
-      my_daf[-1, :]    -- select the last row
-      my_daf[:5]       -- select first 5 rows; like `head()` in other dataframe packages.
-      my_daf[:-5]      -- select last 5 rows; like `tail()` in other dataframe packages.
-      my_daf[:, 3]     -- select only column 3, including all rows. Return a list.
-      my_daf[:, 'C']   -- select only column named 'C', including all rows, return a list.
-      my_daf[2:4]      -- select rows 2 and 3, including all columns, return as daf.
-      my_daf[2:4, :]   -- same as above
-      my_daf[:, 3:5]   -- select columns 3 and 4, including all rows, return as daf.
-      my_daf[[2,4,6]]  -- return rows with indices 2,4,6 as daf array.
-      my_daf[:, [1,3,5]] -- return columns with indices 1,3,5 as daf array.
-      my_daf[['row5','row6','row7']] -- return rows with keyfield values 'row5','row6','row7'
-      my_daf[:, ['col1', 'col3', 'col5']] -- return columns with column names 'col1', 'col3', 'col5'
-      my_daf[('row5','row49'), :]] -- return rows with keyfield values 'row5' through 'row49' inclusive (note: column idx is required)
-      my_daf[('row5',), :]] -- return rows with keyfield values 'row5' through the end (note: column idx is required)
-      my_daf[(,'row49'), :]] -- return rows with keyfield values from the first row through 'row49' inclusive (note: column idx is required)
-      my_daf[:, ('col5', 'col23')]] -- return columns with column names from 'col5', through 'col23' inclusive
-      my_daf[:, (, 'col23')]] -- return columns with column names from the first column through 'col23' inclusive
-      my_daf[:, ('col23',)]] -- return columns with column names from 'col23', through the end
+      `my_daf[2, 3]`     -- select cell at row 2, col 3 and return value.
+      `my_daf[2]`        -- select row 2, including all columns, return a list.
+      `my_daf[2, :]`     -- same as above
+      `my_daf[-1, :]`    -- select the last row
+      `my_daf[:5]`       -- select first 5 rows; like `head()` in other dataframe packages.
+      `my_daf[:-5]`      -- select last 5 rows; like `tail()` in other dataframe packages.
+      `my_daf[:, 3]`     -- select only column 3, including all rows. Return a list.
+      `my_daf[:, 'C']`   -- select only column named 'C', including all rows, return a list.
+      `my_daf[2:4]`      -- select rows 2 and 3, including all columns, return as daf.
+      `my_daf[2:4, :]`   -- same as above
+      `my_daf[:, 3:5]`   -- select columns 3 and 4, including all rows, return as daf.
+      `my_daf[[2,4,6]]`  -- return rows with indices 2,4,6 as daf array.
+      `my_daf[:, [1,3,5]]` -- return columns with indices 1,3,5 as daf array.
+      `my_daf[['row5','row6','row7']]` -- return rows with keyfield values 'row5','row6','row7'
+      `my_daf[:, ['col1', 'col3', 'col5']]` -- return columns with column names 'col1', 'col3', 'col5'
+      `my_daf[('row5','row49'), :]]` -- return rows with keyfield values 'row5' through 'row49' inclusive (note: column idx is required)
+      `my_daf[('row5',), :]]` -- return rows with keyfield values 'row5' through the end (note: column idx is required)
+      `my_daf[(,'row49'), :]]` -- return rows with keyfield values from the first row through 'row49' inclusive (note: column idx is required)
+      `my_daf[:, ('col5', 'col23')]]` -- return columns with column names from 'col5', through 'col23' inclusive
+      `my_daf[:, (, 'col23')]]` -- return columns with column names from the first column through 'col23' inclusive
+      `my_daf[:, ('col23',)]]` -- return columns with column names from 'col23', through the end
 
 
 Please note that if you want to index rows by a keyfield or index columns using column names that are integers, 
 then you must use method calls. The square-bracket indexing will assume any integers are indices, not names.
 The integer values shown in the examples below do not index the array directly, but choose the row or columns by name.
 To choose by row keys (krows), then keyfield must be set. To choose by column keys (kcols), cols must be set.
 
-      my_daf.select_krows(krows = 123)  -- return daf with one row with integer 123 in keyfield column.
-      my_daf.select_krows(krows = [123, 456])  -- return daf with two rows selected by with integers in the keyfield column.
-      my_daf.select_krows(krows = [123, 456], inverse=True)   -- return daf dropping two rows selected by with integers in the keyfield column.
-      my_daf.select_krows(krows = (123, ), inverse=True)   -- drop all rows starting with row named 123 to the end.
-      my_daf.select_krows(krows = (, 123), inverse=True)   -- drop all rows from the first through row named 123.
+    `my_daf.select_krows(krows = 123)`  -- return daf with one row with integer 123 in keyfield column.
+    `my_daf.select_krows(krows = [123, 456])`  -- return daf with two rows selected by with integers in the keyfield column.
+    `my_daf.select_krows(krows = [123, 456], inverse=True)`   -- return daf dropping two rows selected by with integers in the keyfield column.
+    `my_daf.select_krows(krows = (123, ), inverse=True)`   -- drop all rows starting with row named 123 to the end.
+    `my_daf.select_krows(krows = (, 123), inverse=True)`   -- drop all rows from the first through row named 123.
      
-      my_daf.select_kcols(kcols = 123)  -- return daf of column named 123 (integer), placed in col 0
-      my_daf.select_kcols(kcols = 123).to_list()  -- return list of column named 123 (integer).
-      my_daf.select_kcols(kcols = 123).to_list(unique=True)  -- return list with one column with integer 123 colname, and remove duplicates.
-      my_daf.select_kcols(kcols = 123, inverse=True)   -- drop column with name 123
-      my_daf.select_kcols(kcols = 123, inverse=True, flip=True)   -- drop column with name 123 and transpose columns to rows.
+    `my_daf.select_kcols(kcols = 123)`  -- return daf of column named 123 (integer), placed in col 0
+    `my_daf.select_kcols(kcols = 123).to_list()`  -- return list of column named 123 (integer).
+    `my_daf.select_kcols(kcols = 123).to_list(unique=True)`  -- return list with one column with integer 123 colname, and remove duplicates.
+    `my_daf.select_kcols(kcols = 123, inverse=True)`   -- drop column with name 123
+    `my_daf.select_kcols(kcols = 123, inverse=True, flip=True)`   -- drop column with name 123 and transpose columns to rows.
 
 There are also similar methods for selecting rows and cols by indexes. Selecting rows using select_irows(rows_spec) is the same as my_daf[row_spec],
 except the parameter inverse is available to drop rows rather than keeping them.
 
     my_daf.select_irows(irows=10)                  -- select single row 10. Same as my_daf[10].
     my_daf.select_irows(irows=10, inverse=True)    -- drop single row 10. Same as my_daf[10].
     my_daf.select_irows(irows=[1,2,3,45])          -- select rows 1,2,3, and 45 using indices. Same as my_daf[[1,2,3,45]].
```

### Comparing `daffodil-0.3.0/setup.py` & `daffodil-0.4.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from setuptools import setup, find_packages
-from pathlib import Path
 
 setup(
-    name='daffodil',
-    version='0.3.0',
-    packages=find_packages(),
+    name="daffodil",
+    version="0.4.2",
+    packages=find_packages(),  # Automatically discover packages
+    author="Ray Lutz",
+    author_email="raylutz@cognisys.com",
+    description="Daffodil provides lightweight and fast 2-D dataframes",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/raylutz/daffodil",
+    #packages=["daffodil"],
+    python_requires=">=3.6",
     install_requires=[
-        'xlsx2csv==0.8.2',
-        'Markdown==3.4.1',
+        "xlsx2csv==0.8.2",
+        "Markdown==3.4.1",
     ],
     extras_require={
-        'numpy': ['numpy'],
+        "numpy": ["numpy"],
     },
-    author='Ray Lutz',
-    author_email='raylutz@cognisys.com',
-    description='Daffodil provides lightweight and fast 2-D dataframes',
-    long_description=Path('README.md').read_text(),
-    long_description_content_type='text/markdown',
-    url='https://github.com/raylutz/daffodil',
-    python_requires='>=3.6',
-    readme="READMD.md",
-    license='MIT',
+    license="MIT",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
+        "Development Status :: 2 - Pre-Alpha",
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
     ],
 )
```

### Comparing `daffodil-0.3.0/tests/test_daf.py` & `daffodil-0.4.2/tests/test_daf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import pandas as pd
 #from io import BytesIO
 from pathlib import Path
 sys.path.append('..')
 
 from daffodil.daf import Daf
-from lib import daf_utils as utils
+from daffodil.lib import daf_utils as utils
 
 class TestDaf(unittest.TestCase):
 
     maxDiff = None
     
     # initialization
     def test_init_default_values(self):
@@ -31,15 +31,15 @@
     def test_init_custom_values(self):
         cols = ['col1', 'col2']
         hd = {'col1': 0, 'col2': 1}
         lol = [[1, 2], [3, 4]]
         kd = {1: 0, 3: 1}
         dtypes = {'col1': int, 'col2': str}
         expected_lol = [[1, '2'], [3, '4']]
-        daf = Daf(cols=cols, lol=lol, dtypes=dtypes, name='TestDaf', keyfield='col1')
+        daf = Daf(cols=cols, lol=lol, dtypes=dtypes, name='TestDaf', keyfield='col1').apply_dtypes(from_str=False)
         self.assertEqual(daf.name, 'TestDaf')
         self.assertEqual(daf.keyfield, 'col1')
         self.assertEqual(daf.hd, hd)
         self.assertEqual(daf.lol, expected_lol)
         self.assertEqual(daf.kd, kd)
         self.assertEqual(daf.dtypes, dtypes)
         self.assertEqual(daf._iter_index, 0)
@@ -47,15 +47,15 @@
     def test_init_no_cols_but_dtypes(self):
         #cols = ['col1', 'col2']
         hd = {'col1': 0, 'col2': 1}
         lol = [[1, 2], [3, 4]]
         kd = {1: 0, 3: 1}
         dtypes = {'col1': int, 'col2': str}
         expected_lol = [[1, '2'], [3, '4']]
-        daf = Daf(lol=lol, dtypes=dtypes, name='TestDaf', keyfield='col1')
+        daf = Daf(lol=lol, dtypes=dtypes, name='TestDaf', keyfield='col1').apply_dtypes(from_str=False)
         self.assertEqual(daf.name, 'TestDaf')
         self.assertEqual(daf.keyfield, 'col1')
         self.assertEqual(daf.hd, hd)
         self.assertEqual(daf.lol, expected_lol)
         self.assertEqual(daf.kd, kd)
         self.assertEqual(daf.dtypes, dtypes)
         self.assertEqual(daf._iter_index, 0)
@@ -826,15 +826,15 @@
         df_mock = pd.DataFrame([
             {'ID': 1, 'Name': 'John', 'Age': 30},
             {'ID': 2, 'Name': 'Alice', 'Age': 25},
             {'ID': 3, 'Name': 'Bob', 'Age': 35}
         ])
 
         # Call the method under test
-        daf = Daf.from_pandas_df(df_mock, use_csv=True)
+        daf = Daf.from_pandas_df(df_mock, use_csv=True).apply_dtypes(dtypes={'ID': int, 'Name': str, 'Age': int})
 
         # Assert that the Daf object is created with the correct properties
         self.assertEqual(daf.len(), 3)
         self.assertEqual(daf.num_cols(), 3)
         self.assertEqual(daf.columns(), ['ID', 'Name', 'Age'])
         self.assertEqual(daf.lol, [[1, 'John', 30], [2, 'Alice', 25], [3, 'Bob', 35]])
 
@@ -1176,16 +1176,16 @@
         daf1 = Daf()
         daf2 = Daf()
 
         cols = ['col1', 'col2']
         hd = {'col1': 0, 'col2': 1}
         lol1 = [[1, 'a'], [2, 'b']]
         lol2 = [['x', 'y'], ['z', 'w']]
-        daf1 = Daf(cols=cols, lol=lol1, keyfield='', dtypes={'col1': str, 'col2': str})
-        daf2 = Daf(cols=cols, lol=lol2, keyfield='', dtypes={'col1': str, 'col2': str})
+        daf1 = Daf(cols=cols, lol=lol1, keyfield='', dtypes={'col1': str, 'col2': str}).apply_dtypes(from_str=False)
+        daf2 = Daf(cols=cols, lol=lol2, keyfield='', dtypes={'col1': str, 'col2': str}).apply_dtypes(from_str=False)
 
         daf1.concat(daf2)
 
         self.assertEqual(daf1.name, '')
         self.assertEqual(daf1.keyfield, '')
         self.assertEqual(daf1.hd, hd)
         self.assertEqual(daf1.lol, [['1', 'a'], ['2', 'b'], ['x', 'y'], ['z', 'w']])
@@ -1220,16 +1220,16 @@
 
         cols = ['col1', 'col2']
         hd = {'col1': 0, 'col2': 1}
         lol1 = [[1, 'a'], [2, 'b']]
         lol2 = [['x', 'y'], ['z', 'w']]
         
         # import pdb; pdb.set_trace() #temp
-        daf1 = Daf(cols=cols, lol=lol1, keyfield='', dtypes={'col1': str, 'col2': str})
-        daf2 = Daf(cols=cols, lol=lol2, keyfield='', dtypes={'col1': str, 'col2': str})
+        daf1 = Daf(cols=cols, lol=lol1, keyfield='', dtypes={'col1': str, 'col2': str}).apply_dtypes(from_str=False)
+        daf2 = Daf(cols=cols, lol=lol2, keyfield='', dtypes={'col1': str, 'col2': str}).apply_dtypes(from_str=False)
 
         daf1.append(daf2)
 
         self.assertEqual(daf1.name, '')
         self.assertEqual(daf1.keyfield, '')
         self.assertEqual(daf1.hd, hd)
         self.assertEqual(daf1.lol, [['1', 'a'], ['2', 'b'], ['x', 'y'], ['z', 'w']])
@@ -3522,15 +3522,15 @@
         expected_daf = Daf(cols=['A', 'B', 'C'], lol=[[1, 4, 7], [2, 5, 8], [3, 6, 9]], keyfield='A')
         self.assertEqual(result_daf, expected_daf)
 
     def test_from_cols_dol_with_dtypes(self):
         # Test creating Daf instance from cols_dol with specified dtype
         cols_dol = {'A': [1, 2, 3], 'B': [4, 5, 6], 'C': [7, 8, 9]}
         dtypes = {'A': int, 'B': float, 'C': str}
-        result_daf = Daf.from_cols_dol(cols_dol, dtypes=dtypes)
+        result_daf = Daf.from_cols_dol(cols_dol).apply_dtypes(dtypes=dtypes, from_str=False)
         expected_daf = Daf(cols=['A', 'B', 'C'], lol=[[1, 4.0, '7'], [2, 5.0, '8'], [3, 6.0, '9']], dtypes=dtypes)
         self.assertEqual(result_daf, expected_daf)
 
     # # to_dict
     # def test_to_dict_empty_daf(self):
         # # Test to_dict() on an empty Daf instance
         # daf = Daf()
```

