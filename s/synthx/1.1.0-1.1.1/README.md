# Comparing `tmp/synthx-1.1.0.tar.gz` & `tmp/synthx-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthx-1.1.0.tar", max compression
+gzip compressed data, was "synthx-1.1.1.tar", max compression
```

## Comparing `synthx-1.1.0.tar` & `synthx-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7544 2024-04-30 07:29:11.374218 synthx-1.1.0/README.md
--rw-r--r--   0        0        0     1270 2024-04-30 09:13:02.339012 synthx-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.1.0/synthx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.1.0/synthx/core/__init__.py
--rw-r--r--   0        0        0    12286 2024-04-30 09:13:02.339283 synthx-1.1.0/synthx/core/dataset.py
--rw-r--r--   0        0        0     8907 2024-04-30 09:13:02.339542 synthx-1.1.0/synthx/core/result.py
--rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.1.0/synthx/core/sample.py
--rw-r--r--   0        0        0      923 2024-04-30 09:13:02.339718 synthx-1.1.0/synthx/errors/__init__.py
--rw-r--r--   0        0        0    11221 2024-04-24 16:13:54.752232 synthx-1.1.0/synthx/method.py
--rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.1.0/synthx/stats/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.1.0/synthx/stats/norm.py
--rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.1.0/synthx/stats/p.py
--rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 synthx-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7544 2024-04-30 07:29:11.374218 synthx-1.1.1/README.md
+-rw-r--r--   0        0        0     1270 2024-05-02 15:33:38.187018 synthx-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.1.1/synthx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.1.1/synthx/core/__init__.py
+-rw-r--r--   0        0        0    12500 2024-05-02 15:33:38.187244 synthx-1.1.1/synthx/core/dataset.py
+-rw-r--r--   0        0        0     8907 2024-04-30 09:13:02.339542 synthx-1.1.1/synthx/core/result.py
+-rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.1.1/synthx/core/sample.py
+-rw-r--r--   0        0        0      923 2024-04-30 09:13:40.939358 synthx-1.1.1/synthx/errors/__init__.py
+-rw-r--r--   0        0        0    11370 2024-05-02 15:33:38.187471 synthx-1.1.1/synthx/method.py
+-rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.1.1/synthx/stats/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.1.1/synthx/stats/norm.py
+-rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.1.1/synthx/stats/p.py
+-rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 synthx-1.1.1/PKG-INFO
```

### Comparing `synthx-1.1.0/README.md` & `synthx-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `synthx-1.1.0/pyproject.toml` & `synthx-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synthx"
-version = "1.1.0"
+version = "1.1.1"
 description = "A Python Library for Advanced Synthetic Control Analysis"
 authors = ["kenki931128 <kenki.nkmr@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `synthx-1.1.0/synthx/core/dataset.py` & `synthx-1.1.1/synthx/core/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,27 +60,37 @@
         )
         self.intervention_time = intervention_time
         self.validation_time = validation_time
         self.norm = norm
         self.__validate()
         self.__normalization()
 
-    def plot(self, units: Optional[list[str]] = None, save: Optional[str] = None) -> None:
+    def plot(
+        self,
+        units: Optional[list[str]] = None,
+        save: Optional[str] = None,
+        show_label: bool = False,
+    ) -> None:
         """Plot the dataset and display its characteristics.
 
         Args:
             units (Optional[list[str]]): only plot data of this variable if specified.
             save (Optional[str]): file path to save the plot. If None, the plot will be displayed.
+            show_label (bool): show label on the plot or not.
         """
         # Plot the target variable over time for each unit
         units = units if units is not None else self.data[self.unit_column].unique().to_list()
         plt.figure(figsize=(10, 6))
         for unit in units:
             unit_data = self.data.filter(pl.col(self.unit_column) == unit)
-            plt.plot(unit_data[self.time_column], unit_data[self.y_column], label=f'Unit {unit}')
+            plt.plot(
+                unit_data[self.time_column],
+                unit_data[self.y_column],
+                label=f'Unit {unit}' if show_label else None,
+            )
 
         # Add vertical line for validation time and intervention time
         if self.validation_time is not None:
             plt.axvline(
                 self.validation_time, color='orange', linestyle='--', label='Validation Time'  # type: ignore
             )
         plt.axvline(
```

### Comparing `synthx-1.1.0/synthx/core/result.py` & `synthx-1.1.1/synthx/core/result.py`

 * *Files identical despite different names*

### Comparing `synthx-1.1.0/synthx/core/sample.py` & `synthx-1.1.1/synthx/core/sample.py`

 * *Files identical despite different names*

### Comparing `synthx-1.1.0/synthx/errors/__init__.py` & `synthx-1.1.1/synthx/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `synthx-1.1.0/synthx/method.py` & `synthx-1.1.1/synthx/method.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,22 +210,24 @@
 
 def sensitivity_check(
     dataset: sx.Dataset,
     effects_placebo: list[float],
     p_value_target: float = 0.03,
     l: float = 1.0,
     r: float = 10.0,
+    write_progress: bool = False,
 ) -> Optional[float]:
     """Perform a sensitivity check on the synthetic control results.
 
     Args:
         dataset (sx.Dataset): The dataset for the synthetic control analysis.
         effects_placebo (list[float]): The list of placebo effects estimated.
         p_value_target (float, optional): The target p-value threshold for statistical significance.
         l (float), r (float): the range of uplift. If you have assumption, narrow down to be faster.
+        write_progress (bool): Whether to write progress information to stderr.
 
     Returns:
         float or None: The uplift which becomes statistically significant.
     """
     df = dataset.data
 
     if l < 1.0:
@@ -266,14 +268,15 @@
             r = uplift  # highly likely uplift was too big. TODO: think better algorithm.
             continue
 
         p_value = sx.stats.calc_p_value(sc.estimate_effects(), effects_placebo)
         if p_value <= p_value_target:
             r = uplift
         else:
-            tqdm.write(f'uplift: {uplift:.4f}, p value: {p_value}.', file=sys.stderr)
+            if write_progress:
+                tqdm.write(f'uplift: {uplift:.4f}, p value: {p_value}.', file=sys.stderr)
             l = uplift
 
     # even 1000% uplift cannot be captured / singnificant difference without actual uplift.
     if r == 10 or l == 1:
         return None
     return r
```

### Comparing `synthx-1.1.0/synthx/stats/norm.py` & `synthx-1.1.1/synthx/stats/norm.py`

 * *Files identical despite different names*

### Comparing `synthx-1.1.0/synthx/stats/p.py` & `synthx-1.1.1/synthx/stats/p.py`

 * *Files identical despite different names*

### Comparing `synthx-1.1.0/PKG-INFO` & `synthx-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthx
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python Library for Advanced Synthetic Control Analysis
 License: MIT
 Author: kenki931128
 Author-email: kenki.nkmr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

