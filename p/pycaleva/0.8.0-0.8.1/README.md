# Comparing `tmp/pycaleva-0.8.0.tar.gz` & `tmp/pycaleva-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycaleva-0.8.0.tar", last modified: Wed May  1 19:26:30 2024, max compression
+gzip compressed data, was "pycaleva-0.8.1.tar", last modified: Thu May  2 20:21:41 2024, max compression
```

## Comparing `pycaleva-0.8.0.tar` & `pycaleva-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-01 19:26:30.187409 pycaleva-0.8.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1520 2024-05-01 18:08:29.000000 pycaleva-0.8.0/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     7394 2024-05-01 19:26:30.187409 pycaleva-0.8.0/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     6571 2024-05-01 18:30:48.000000 pycaleva-0.8.0/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)       79 2024-05-01 19:26:30.191409 pycaleva-0.8.0/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     1321 2024-05-01 18:46:24.000000 pycaleva-0.8.0/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-01 19:26:30.187409 pycaleva-0.8.0/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-01 19:26:30.187409 pycaleva-0.8.0/src/pycaleva/
--rw-rw-r--   0 martin    (1000) martin    (1000)       80 2024-05-01 18:08:29.000000 pycaleva-0.8.0/src/pycaleva/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    36030 2024-05-01 19:21:29.000000 pycaleva-0.8.0/src/pycaleva/_basecalib.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6056 2024-05-01 18:48:50.000000 pycaleva-0.8.0/src/pycaleva/_report.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      556 2024-05-01 18:08:29.000000 pycaleva-0.8.0/src/pycaleva/_result_types.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    20495 2024-05-01 18:08:29.000000 pycaleva-0.8.0/src/pycaleva/calbelt.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      925 2024-05-01 18:08:29.000000 pycaleva-0.8.0/src/pycaleva/calibeval.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1751 2024-05-01 18:08:29.000000 pycaleva-0.8.0/src/pycaleva/metrics.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-01 19:26:30.187409 pycaleva-0.8.0/src/pycaleva.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     7394 2024-05-01 19:26:30.000000 pycaleva-0.8.0/src/pycaleva.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      395 2024-05-01 19:26:30.000000 pycaleva-0.8.0/src/pycaleva.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-05-01 19:26:30.000000 pycaleva-0.8.0/src/pycaleva.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      124 2024-05-01 19:26:30.000000 pycaleva-0.8.0/src/pycaleva.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        9 2024-05-01 19:26:30.000000 pycaleva-0.8.0/src/pycaleva.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-02 20:21:41.858516 pycaleva-0.8.1/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1520 2024-05-01 18:08:29.000000 pycaleva-0.8.1/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7394 2024-05-02 20:21:41.858516 pycaleva-0.8.1/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6571 2024-05-01 18:30:48.000000 pycaleva-0.8.1/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)       79 2024-05-02 20:21:41.862516 pycaleva-0.8.1/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1321 2024-05-02 20:20:37.000000 pycaleva-0.8.1/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-02 20:21:41.858516 pycaleva-0.8.1/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-02 20:21:41.858516 pycaleva-0.8.1/src/pycaleva/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       80 2024-05-01 18:08:29.000000 pycaleva-0.8.1/src/pycaleva/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    36175 2024-05-02 20:18:11.000000 pycaleva-0.8.1/src/pycaleva/_basecalib.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6056 2024-05-01 18:48:50.000000 pycaleva-0.8.1/src/pycaleva/_report.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      556 2024-05-01 18:08:29.000000 pycaleva-0.8.1/src/pycaleva/_result_types.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    20495 2024-05-01 18:08:29.000000 pycaleva-0.8.1/src/pycaleva/calbelt.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      925 2024-05-01 18:08:29.000000 pycaleva-0.8.1/src/pycaleva/calibeval.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1751 2024-05-01 18:08:29.000000 pycaleva-0.8.1/src/pycaleva/metrics.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-02 20:21:41.858516 pycaleva-0.8.1/src/pycaleva.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7394 2024-05-02 20:21:41.000000 pycaleva-0.8.1/src/pycaleva.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      395 2024-05-02 20:21:41.000000 pycaleva-0.8.1/src/pycaleva.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-05-02 20:21:41.000000 pycaleva-0.8.1/src/pycaleva.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      124 2024-05-02 20:21:41.000000 pycaleva-0.8.1/src/pycaleva.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        9 2024-05-02 20:21:41.000000 pycaleva-0.8.1/src/pycaleva.egg-info/top_level.txt
```

### Comparing `pycaleva-0.8.0/LICENSE` & `pycaleva-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycaleva-0.8.0/PKG-INFO` & `pycaleva-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaleva
-Version: 0.8.0
+Version: 0.8.1
 Summary: A framework for calibration evaluation of binary classification models
 Home-page: https://github.com/MartinWeigl/pycaleva
 Author: Martin Weigl
 Author-email: martinweigl48@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/MartinWeigl/pycaleva
 Project-URL: Documentation, https://martinweigl.github.io/pycaleva/
```

### Comparing `pycaleva-0.8.0/README.md` & `pycaleva-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pycaleva-0.8.0/setup.py` & `pycaleva-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name="pycaleva",
-    version="0.8.0",
+    version="0.8.1",
     author="Martin Weigl",
     author_email="martinweigl48@gmail.com",
     description="A framework for calibration evaluation of binary classification models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MartinWeigl/pycaleva",
```

### Comparing `pycaleva-0.8.0/src/pycaleva/_basecalib.py` & `pycaleva-0.8.1/src/pycaleva/_basecalib.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         df = df.sort_values('prob')
         df.reset_index(inplace=True)
         
         # Group data using deciles of risks
         try:
             df['dcl'] = pd.qcut(df['prob'], self.__ngroups)
         except ValueError:
-            # Most likely low variance in probabilities results in non unique bin edges
+            # Most likely low variance in probabilities results in non unique bin e
             try:
                 # FIX -> Put some probabilities into the same group
                 df['dcl'] = pd.qcut(df['prob'].rank(method='first'), self.__ngroups)
 
                 # Get propper interval labels after applied fix
                 new_categories = {}
                 df['rank'] = df['prob'].rank(method='first')
@@ -858,31 +858,31 @@
 
         # Get nonparametric curve based on y and p using lowess
         x_nonparametric,y_nonparametric = self.__nonparametric_fit(update_awlc=False)
 
         # Add calibration line for model
         plt.scatter(p_grouped,y_grouped, marker="^", facecolors='none', edgecolors='r', label=f'Grouped observations g={self.__ngroups}')
 
-        # Add histogram on second axis
-        h, e = np.histogram(self.__p, bins=50)
-        h = h.astype('float')
-        h /= h.max()                # Get relative frequencies
-        ax2 = ax1.twinx()
-        ax2.set_ylim(-0.1,5)        # Scale down histogram
-        ax2.axis('off')             # Hide labels and ticks
-        ax2.stem(e[:-1],h, linefmt="grey", markerfmt=" ", basefmt=" ")
-
         # Add line for nonparametric fit using lowess
         ax1.plot(x_nonparametric, y_nonparametric, label="Nonparametric")
 
         # Add line for perfect calibration
         ax1.plot([0, 1], [0, 1], "k:", label="Perfectly calibrated")
 
+        # Add stem plot for distribution of observations
+        h, e = np.histogram(self.__p, bins=50, density=False)
+        bin_center_points = 0.5 * (e[1:] + e[:-1])
+        h = h.astype('float')
+        h /= h.sum()                   # normalize stem height to sum to 1
+        ax2 = ax1.twinx()
+        ax2.set_ylim([-0.01, 1.05])    # y-domain for the stem plot goes from 0 to 1, with slight offsets for visibility reasons
+        ax2.stem(bin_center_points, h, linefmt="grey", markerfmt=" ", basefmt=" ")
+
         ax1.set_xlabel('Predicted Probability')
         ax1.set_ylabel('Actual Probability')
         
-        props = dict(boxstyle='round', facecolor='white', alpha=0.4)
-        ax1.text(0.00, 0.75, self.__metrics_to_string(), fontsize=10, family='monospace', bbox=props)
+        props = dict(boxstyle='round', facecolor='white', alpha=0.5)
+        ax1.text(0.02, 0.78, self.__metrics_to_string(), fontsize=10, family='monospace', bbox=props)
 
-        ax1.legend(loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5))
+        ax1.legend(loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5), fancybox=True, framealpha=0.5)
 
         return fig
```

### Comparing `pycaleva-0.8.0/src/pycaleva/_report.py` & `pycaleva-0.8.1/src/pycaleva/_report.py`

 * *Files identical despite different names*

### Comparing `pycaleva-0.8.0/src/pycaleva/_result_types.py` & `pycaleva-0.8.1/src/pycaleva/_result_types.py`

 * *Files identical despite different names*

### Comparing `pycaleva-0.8.0/src/pycaleva/calbelt.py` & `pycaleva-0.8.1/src/pycaleva/calbelt.py`

 * *Files identical despite different names*

### Comparing `pycaleva-0.8.0/src/pycaleva/calibeval.py` & `pycaleva-0.8.1/src/pycaleva/calibeval.py`

 * *Files identical despite different names*

### Comparing `pycaleva-0.8.0/src/pycaleva/metrics.py` & `pycaleva-0.8.1/src/pycaleva/metrics.py`

 * *Files identical despite different names*

### Comparing `pycaleva-0.8.0/src/pycaleva.egg-info/PKG-INFO` & `pycaleva-0.8.1/src/pycaleva.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaleva
-Version: 0.8.0
+Version: 0.8.1
 Summary: A framework for calibration evaluation of binary classification models
 Home-page: https://github.com/MartinWeigl/pycaleva
 Author: Martin Weigl
 Author-email: martinweigl48@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/MartinWeigl/pycaleva
 Project-URL: Documentation, https://martinweigl.github.io/pycaleva/
```

