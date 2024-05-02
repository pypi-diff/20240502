# Comparing `tmp/szkgraph-0.0.2.tar.gz` & `tmp/szkgraph-0.0.3.tar.gz`

## Comparing `szkgraph-0.0.2.tar` & `szkgraph-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 szkgraph-0.0.2/examples/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 szkgraph-0.0.2/src/szkGraph/__init__.py
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 szkgraph-0.0.2/src/szkGraph/szkGraph.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 szkgraph-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 szkgraph-0.0.2/LICENSE
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 szkgraph-0.0.2/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 szkgraph-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 szkgraph-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 szkgraph-0.0.3/examples/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 szkgraph-0.0.3/src/szkGraph/__init__.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 szkgraph-0.0.3/src/szkGraph/formatter.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 szkgraph-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 szkgraph-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 szkgraph-0.0.3/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 szkgraph-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 szkgraph-0.0.3/PKG-INFO
```

### Comparing `szkgraph-0.0.2/examples/example.py` & `szkgraph-0.0.3/examples/example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import szkGraph
+import szkGraph.formatter as gformat
 
 
 # example 1: plot a simple graph
 def example1():
     # preparation
-    fig, ax = szkGraph.prepare(
+    fig, ax = gformat.prepare(
         xtitle="This is x-axis",
         ytitle="This is y-axis",
         w=6,
         h=5,
         font="arial",
     )
 
     # plotting scatter
     x = [0, 1, 2, 3, 4, 5]
     y = [0, 1, 4, 9, 16, 25]
     ax.scatter(x, y)
 
     # output the graph
     fn_out = "example1.png"
-    szkGraph.finalize(fig, ax, fn_out)
+    gformat.finalize(fig, ax, fn_out)
 
 
 # example 2: modify figure size
 def example2():
     # figure size can be set with width and height, or width and ratio
     # width can be float value in inches, or portion of paper width, or portion of powerpoint page width
     # number of pixels are determined by inches*dpi. default dpi is 300, which is common value for printing.
 
     # preparation
-    fig, ax = szkGraph.prepare(
+    fig, ax = gformat.prepare(
         xtitle="This is x-axis",
         ytitle="This is y-axis",
         w="pp0.3",  # 0.3 of the powerpoint page width
         r=0.7,  # ratio of height to width
         font="arial",
     )
 
     # plotting scatter
     x = [0, 1, 2, 3, 4, 5]
     y = [0, 1, 4, 9, 16, 25]
     ax.scatter(x, y)
 
     # output the graph
     fn_out = "example2.png"
-    szkGraph.finalize(fig, ax, fn_out)
+    gformat.finalize(fig, ax, fn_out)
 
 
 # example 3: modify axis range and tick interval
 def example3():
     # preparation
-    fig, ax = szkGraph.prepare(
+    fig, ax = gformat.prepare(
         xtitle="This is x-axis",
         ytitle="This is y-axis",
         w=6,
         h=5,
         font="arial",
     )
 
@@ -64,15 +64,15 @@
     ax.scatter(x, y)
 
     # axis range can bw set with lims, where [xmin, xmax, ymin, ymax]
     # tick interval can be set with xspace and yspace, where float for spacing and tuple for (spacing, offset)
 
     # output the graph
     fn_out = "example3.png"
-    szkGraph.finalize(
+    gformat.finalize(
         fig, ax, fn_out, lims=[-0.5, 5.5, -1, 26], xspace=(1, 0), yspace=(5, 0)
     )
 
 
 ### EXECUTION ###
 example1()
 example2()
```

### Comparing `szkgraph-0.0.2/src/szkGraph/szkGraph.py` & `szkgraph-0.0.3/src/szkGraph/formatter.py`

 * *Files identical despite different names*

### Comparing `szkgraph-0.0.2/.gitignore` & `szkgraph-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `szkgraph-0.0.2/LICENSE` & `szkgraph-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `szkgraph-0.0.2/README.md` & `szkgraph-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # szkGraph - simple style formatter for matplotlib
 This is a useful Python codes to simply modify the style of matplotlib for your presentation and academic papers.
 Any type of suggestions, feedbacks, and upgrades are welcome.
 
 # How to install?
 Install using pip.
+
 `python -m pip install -U szkGraph`
 
+Then, import as follows.
+
+`import szkGraph.formatter`
+
 # How to use?
-Call `szkGraph.prepare()` to initialize the figure. Use the returned `fig, ax` for plotting.
-After plotting and modifying your figure, export the figure with `szkGraph.finalize()`. 
+Call `formatter.prepare()` to initialize the figure. Use the returned `fig, ax` for plotting.
+After plotting and modifying your figure, export the figure with `formatter.finalize()`. 
 
-## `szkGraph.prepare(xtitle=None, ytitle=None, w=None, h=None, r=0.7, font="arial", fontsize=20)`
+## `formatter.prepare(xtitle=None, ytitle=None, w=None, h=None, r=0.7, font="arial", fontsize=20)`
 ### Paramters
 * **xtitle**: _str, optional_
     Title of x-axis.
 * **ytitle**: _str, optional_
     Title of y-axis.
 * **w**: _float or str, optional_
     Float for specifying the width in inches, str for specifying the width relative to powerpoint slide or academic paper.
@@ -29,15 +34,15 @@
     Fontsize in pt.
 
 ### Returns
 * **fig**: _matplotlib.figure_
 * **ax**: _matplotlib.axes_
 
 
-## `finalize(fig, ax, fn_figout, lims=[None, None, None, None], dpi=300, comp={}, tight=True, pad=0.2, xspace=None, yspace=None)`
+## `formatter.finalize(fig, ax, fn_figout, lims=[None, None, None, None], dpi=300, comp={}, tight=True, pad=0.2, xspace=None, yspace=None)`
 ### Paramters
 * **fig**: _matplotlib.figure_
 * **ax**: _matplotlib.axes_
 * **fn_figout**: _str_
     Name of the output figure file. It could also be in absolute or relative path.
 * **lims**: _list of floats, optional_
     Range of axis in one list as `[xmin, xmax, ymin, ymax]`.
```

### Comparing `szkgraph-0.0.2/pyproject.toml` & `szkgraph-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "szkGraph"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Mahiro Sawada", email="sawada.mahiro@gmail.com" },
 ]
 description = "An easy graph formatting tool for matplotlib"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `szkgraph-0.0.2/PKG-INFO` & `szkgraph-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: szkGraph
-Version: 0.0.2
+Version: 0.0.3
 Summary: An easy graph formatting tool for matplotlib
 Project-URL: Homepage, https://github.com/MP931/szkGraph
 Project-URL: Issues, https://github.com/MP931/szkGraph/issues
 Author-email: Mahiro Sawada <sawada.mahiro@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,21 +15,26 @@
 
 # szkGraph - simple style formatter for matplotlib
 This is a useful Python codes to simply modify the style of matplotlib for your presentation and academic papers.
 Any type of suggestions, feedbacks, and upgrades are welcome.
 
 # How to install?
 Install using pip.
+
 `python -m pip install -U szkGraph`
 
+Then, import as follows.
+
+`import szkGraph.formatter`
+
 # How to use?
-Call `szkGraph.prepare()` to initialize the figure. Use the returned `fig, ax` for plotting.
-After plotting and modifying your figure, export the figure with `szkGraph.finalize()`. 
+Call `formatter.prepare()` to initialize the figure. Use the returned `fig, ax` for plotting.
+After plotting and modifying your figure, export the figure with `formatter.finalize()`. 
 
-## `szkGraph.prepare(xtitle=None, ytitle=None, w=None, h=None, r=0.7, font="arial", fontsize=20)`
+## `formatter.prepare(xtitle=None, ytitle=None, w=None, h=None, r=0.7, font="arial", fontsize=20)`
 ### Paramters
 * **xtitle**: _str, optional_
     Title of x-axis.
 * **ytitle**: _str, optional_
     Title of y-axis.
 * **w**: _float or str, optional_
     Float for specifying the width in inches, str for specifying the width relative to powerpoint slide or academic paper.
@@ -44,15 +49,15 @@
     Fontsize in pt.
 
 ### Returns
 * **fig**: _matplotlib.figure_
 * **ax**: _matplotlib.axes_
 
 
-## `finalize(fig, ax, fn_figout, lims=[None, None, None, None], dpi=300, comp={}, tight=True, pad=0.2, xspace=None, yspace=None)`
+## `formatter.finalize(fig, ax, fn_figout, lims=[None, None, None, None], dpi=300, comp={}, tight=True, pad=0.2, xspace=None, yspace=None)`
 ### Paramters
 * **fig**: _matplotlib.figure_
 * **ax**: _matplotlib.axes_
 * **fn_figout**: _str_
     Name of the output figure file. It could also be in absolute or relative path.
 * **lims**: _list of floats, optional_
     Range of axis in one list as `[xmin, xmax, ymin, ymax]`.
```

