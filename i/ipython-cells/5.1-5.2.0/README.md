# Comparing `tmp/ipython_cells-5.1.tar.gz` & `tmp/ipython_cells-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ipython_cells-5.1.tar", last modified: Tue Apr 28 23:31:35 2020, max compression
+gzip compressed data, was "ipython_cells-5.2.0.tar", last modified: Thu May  2 20:49:33 2024, max compression
```

## Comparing `ipython_cells-5.1.tar` & `ipython_cells-5.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 evan      (1000) evan      (1000)        0 2020-04-28 23:31:35.000000 ipython_cells-5.1/
--rw-rw-r--   0 evan      (1000) evan      (1000)     3151 2020-04-28 23:31:35.000000 ipython_cells-5.1/PKG-INFO
--rw-rw-r--   0 evan      (1000) evan      (1000)     1940 2020-04-28 23:29:43.000000 ipython_cells-5.1/README.md
-drwxrwxr-x   0 evan      (1000) evan      (1000)        0 2020-04-28 23:31:35.000000 ipython_cells-5.1/ipython_cells/
--rw-rw-r--   0 evan      (1000) evan      (1000)       50 2019-02-23 07:48:22.000000 ipython_cells-5.1/ipython_cells/__init__.py
--rw-rw-r--   0 evan      (1000) evan      (1000)     4194 2020-04-28 23:29:20.000000 ipython_cells-5.1/ipython_cells/ipython_cells.py
--rw-rw-r--   0 evan      (1000) evan      (1000)       20 2020-04-28 23:30:55.000000 ipython_cells-5.1/ipython_cells/version.py
-drwxrwxr-x   0 evan      (1000) evan      (1000)        0 2020-04-28 23:31:35.000000 ipython_cells-5.1/ipython_cells.egg-info/
--rw-rw-r--   0 evan      (1000) evan      (1000)     3151 2020-04-28 23:31:34.000000 ipython_cells-5.1/ipython_cells.egg-info/PKG-INFO
--rw-rw-r--   0 evan      (1000) evan      (1000)      284 2020-04-28 23:31:34.000000 ipython_cells-5.1/ipython_cells.egg-info/SOURCES.txt
--rw-rw-r--   0 evan      (1000) evan      (1000)        1 2020-04-28 23:31:34.000000 ipython_cells-5.1/ipython_cells.egg-info/dependency_links.txt
--rw-rw-r--   0 evan      (1000) evan      (1000)        8 2020-04-28 23:31:34.000000 ipython_cells-5.1/ipython_cells.egg-info/requires.txt
--rw-rw-r--   0 evan      (1000) evan      (1000)       14 2020-04-28 23:31:34.000000 ipython_cells-5.1/ipython_cells.egg-info/top_level.txt
--rw-rw-r--   0 evan      (1000) evan      (1000)       38 2020-04-28 23:31:35.000000 ipython_cells-5.1/setup.cfg
--rw-rw-r--   0 evan      (1000) evan      (1000)      667 2019-05-16 19:20:15.000000 ipython_cells-5.1/setup.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-05-02 20:49:33.173953 ipython_cells-5.2.0/
+-rw-r--r--   0 evan      (1000) evan      (1000)     2976 2024-05-02 20:49:33.173953 ipython_cells-5.2.0/PKG-INFO
+-rw-r--r--   0 evan      (1000) evan      (1000)     2555 2022-11-09 23:32:11.000000 ipython_cells-5.2.0/README.md
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-05-02 20:49:33.173953 ipython_cells-5.2.0/ipython_cells/
+-rw-r--r--   0 evan      (1000) evan      (1000)       50 2021-02-03 01:51:20.000000 ipython_cells-5.2.0/ipython_cells/__init__.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     8217 2024-05-02 20:39:45.000000 ipython_cells-5.2.0/ipython_cells/ipython_cells.py
+-rw-r--r--   0 evan      (1000) evan      (1000)       22 2024-05-02 20:48:27.000000 ipython_cells-5.2.0/ipython_cells/version.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-05-02 20:49:33.173953 ipython_cells-5.2.0/ipython_cells.egg-info/
+-rw-r--r--   0 evan      (1000) evan      (1000)     2976 2024-05-02 20:49:33.000000 ipython_cells-5.2.0/ipython_cells.egg-info/PKG-INFO
+-rw-r--r--   0 evan      (1000) evan      (1000)      299 2024-05-02 20:49:33.000000 ipython_cells-5.2.0/ipython_cells.egg-info/SOURCES.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)        1 2024-05-02 20:49:33.000000 ipython_cells-5.2.0/ipython_cells.egg-info/dependency_links.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)        8 2024-05-02 20:49:33.000000 ipython_cells-5.2.0/ipython_cells.egg-info/requires.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       14 2024-05-02 20:49:33.000000 ipython_cells-5.2.0/ipython_cells.egg-info/top_level.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       38 2024-05-02 20:49:33.173953 ipython_cells-5.2.0/setup.cfg
+-rw-r--r--   0 evan      (1000) evan      (1000)      667 2021-02-03 01:51:20.000000 ipython_cells-5.2.0/setup.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-05-02 20:49:33.173953 ipython_cells-5.2.0/tests/
+-rw-r--r--   0 evan      (1000) evan      (1000)     1761 2024-05-02 20:43:31.000000 ipython_cells-5.2.0/tests/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ipython_cells-5.1/README.md` & `ipython_cells-5.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,100 @@
+Metadata-Version: 2.1
+Name: ipython_cells
+Version: 5.2.0
+Summary: Jupyter-like cell running in ipython
+Home-page: https://github.com/uiuc-sine/ipython-cells
+Author: Evan Widloski, Ulaş Kamacι
+Author-email: evan@evanw.org, ukamaci2@illinois.edu
+License: GPLv3
+Keywords: jupyter ipython cells magic extension
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+Requires-Dist: IPython
+
 # ipython-cells
 
-IPython extension for executing cells Jupyter-style in .py files.  Supports Jupyter and Spyder cell syntax.
+This is an IPython extension for those who prefer to work in a terminal but still need the cell-by-cell execution provided by a Jupyter notebook.
+
+Example Jupyter notebook:
+
+![](notebook.png)
+
+Running exported notebook with ipython-cells:
+
+![](commandline.png)
 
-Brings the advantages of linear, selective-execution during development to IPython without the bloat of Jupyter.
 
-#### Quickstart
+## Quickstart
 
-Install the extension
+Install the extension:
 
     pip install ipython-cells
+    
+Convert an existing notebook to a Python file (In Jupyter):
 
-In IPython:
+    Cell > Run All
+    File > Download As > python (.py)
+
+Execute cells in iPython:
 
 ``` python
 >>> %load_ext ipython_cells
->>> %load_file example.py
+>>> %load_file my_notebook.py
 >>> %cell_run 1
-hello
 >>> %cell_run 2
-world
+array([1.+0.j, 1.+0.j, 1.+0.j, 1.+0.j, 1.+0.j, 1.+0.j, 1.+0.j, 1.+0.j])
 ```
 
-`example.py`
+You can freely add/delete/rename cells in the downloaded `my_notebook.py`.  `my_notebook.py` is automatically reloaded when changes are made.
+   
+Alternatively, you can create a new .py file from scratch without starting from a Jupyter notebook.  See the [cell delimiter syntax](#cell-delimiter-syntax).
+
+## Other Features
+
+Spyder cell delimiter syntax is also supported:
 
 ``` python
 # %% cell1
 print('hello')
 
 # %% cell2
 print('world')
 ```
 
-#### Other Features
+Other commands:
 
 ``` python
-%load_file example.py
+# cell ranges - run all cells from beginning of file to cell2 (inclusive)
+>>> %cell_run ^cell2
+hello
+world
+
+# cell ranges - run all cells from cell1 (inclusive) to end of file
+>>> %cell_run cell1$
+hello
+world
 
 # list available cells for running
-%list_cells
+>>> %list_cells
 ['__first', 'cell1', 'cell2']
-
-# run all cells from beginning of file to cell2 (inclusive)
-%cell_run ^cell2
-10
-11
-
-# run all cells from cell1 (inclusive) to end of file
-%cell_run cell1$
-12
-13
 ```
 
-#### Automatically Load Extension
+
+## Automatically Load Extension
 
 To load extension on IPython start, add this to `~/.ipython/profile_default/ipython_config.py`
 
 ``` python
 c.InteractiveShellApp.extensions = [
     'ipython_cells'
 ]
 ```
 
-#### Autoreloading
+## Autoreloading
 ``` python
 # load example.py with autoreloading
 %load_file example.py
 
 %cell_run cell1
 10
 # example.py is modified by an external editor (e.g. `a = 10`  ->  `a = 20`)
@@ -73,26 +102,26 @@
 %cell_run cell1
 20
 
 ```
 
 Auto reloading can be disabled with `%load_file example.py --noreload`
 
-#### Cell Delimiter Syntax
+## Cell Delimiter Syntax
 
 Cells are delimited by special comments.  Both Jupyter and Spyder style cells are supported.  Below are different variations of a cell called `foobar_cell`.
 
 - `# %% foobar_cell`
 - `# In[foobar_cell]`
 - `# %% foobar_cell some extra text`
 - `# In[foobar_cell] some extra text`
 
-#### Running Exported Jupyter Notebooks
+## Running Exported Jupyter Notebooks
 
 This extension can run exported Jupyter notebooks. (`File > Download As > python (.py)`).
 
 Be sure to run all cells before exporting so they are assigned an index. (`Cell > Run All`).
 
-#### Tests
+## Tests
 
     cd tests
     ipython3 tests.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ipython_cells-5.1/setup.py` & `ipython_cells-5.2.0/setup.py`

 * *Files identical despite different names*

