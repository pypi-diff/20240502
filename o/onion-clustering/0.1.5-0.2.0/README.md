# Comparing `tmp/onion_clustering-0.1.5.tar.gz` & `tmp/onion_clustering-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_clustering-0.1.5.tar", last modified: Mon Apr 29 14:35:36 2024, max compression
+gzip compressed data, was "onion_clustering-0.2.0.tar", last modified: Thu May  2 13:06:17 2024, max compression
```

## Comparing `onion_clustering-0.1.5.tar` & `onion_clustering-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.540272 onion_clustering-0.1.5/
--rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/.coverage
--rw-r--r--   0 mattebecchi   (501) staff       (20)       50 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/.gitignore
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.1.5/LICENSE
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-04-29 14:35:36.539260 onion_clustering-0.1.5/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/README.md
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.523382 onion_clustering-0.1.5/examples/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3664 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/examples/example_script.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3669 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/examples/example_script_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      635 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/justfile
--rw-r--r--   0 mattebecchi   (501) staff       (20)      942 2024-04-29 14:35:03.000000 onion_clustering-0.1.5/pyproject.toml
--rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.1.5/pytest.ini
--rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-04-29 14:35:36.540594 onion_clustering-0.1.5/setup.cfg
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.517796 onion_clustering-0.1.5/src/
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.528542 onion_clustering-0.1.5/src/onion_clustering/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/__init__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      465 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/__version__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    34309 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    19431 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/first_classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    23244 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/functions.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    17172 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/main.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    23148 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/main_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/utilities.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.538152 onion_clustering-0.1.5/src/onion_clustering.egg-info/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-04-29 14:35:36.000000 onion_clustering-0.1.5/src/onion_clustering.egg-info/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)      878 2024-04-29 14:35:36.000000 onion_clustering-0.1.5/src/onion_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-04-29 14:35:36.000000 onion_clustering-0.1.5/src/onion_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-04-29 14:35:36.000000 onion_clustering-0.1.5/src/onion_clustering.egg-info/requires.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-04-29 14:35:36.000000 onion_clustering-0.1.5/src/onion_clustering.egg-info/top_level.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.533722 onion_clustering-0.1.5/test/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.1.5/test/__init__.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.535537 onion_clustering-0.1.5/test/output_multi/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      409 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_multi/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_multi/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_multi/number_of_states.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.537357 onion_clustering-0.1.5/test/output_uni/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      265 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_uni/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_uni/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_uni/number_of_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3361 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/test_multi.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3271 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/test_uni.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.948502 onion_clustering-0.2.0/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-05-02 13:04:24.000000 onion_clustering-0.2.0/.coverage
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       50 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/.gitignore
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.0/LICENSE
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-02 13:06:17.947605 onion_clustering-0.2.0/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/README.md
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.932442 onion_clustering-0.2.0/examples/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3664 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/examples/example_script.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3669 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/examples/example_script_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/justfile
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-02 13:05:25.000000 onion_clustering-0.2.0/pyproject.toml
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.0/pytest.ini
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-02 13:06:17.948680 onion_clustering-0.2.0/setup.cfg
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.927333 onion_clustering-0.2.0/src/
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.936821 onion_clustering-0.2.0/src/onion_clustering/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/src/onion_clustering/__init__.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    35963 2024-05-02 12:59:06.000000 onion_clustering-0.2.0/src/onion_clustering/classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    19800 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/src/onion_clustering/first_classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    22934 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/src/onion_clustering/functions.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    18526 2024-05-02 12:59:27.000000 onion_clustering-0.2.0/src/onion_clustering/main.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    23334 2024-05-02 13:01:37.000000 onion_clustering-0.2.0/src/onion_clustering/main_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/src/onion_clustering/utilities.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.946642 onion_clustering-0.2.0/src/onion_clustering.egg-info/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-05-02 13:06:17.000000 onion_clustering-0.2.0/src/onion_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      842 2024-05-02 13:06:17.000000 onion_clustering-0.2.0/src/onion_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-02 13:06:17.000000 onion_clustering-0.2.0/src/onion_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-02 13:06:17.000000 onion_clustering-0.2.0/src/onion_clustering.egg-info/requires.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-02 13:06:17.000000 onion_clustering-0.2.0/src/onion_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.941621 onion_clustering-0.2.0/test/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.0/test/__init__.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.944046 onion_clustering-0.2.0/test/output_multi/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      409 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/test/output_multi/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/test/output_multi/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/test/output_multi/number_of_states.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-02 13:06:17.945993 onion_clustering-0.2.0/test/output_uni/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1668 2024-05-02 07:31:53.000000 onion_clustering-0.2.0/test/output_uni/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-02 07:28:27.000000 onion_clustering-0.2.0/test/output_uni/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/test/output_uni/number_of_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3375 2024-05-02 07:25:21.000000 onion_clustering-0.2.0/test/test_multi.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3275 2024-05-02 08:15:07.000000 onion_clustering-0.2.0/test/test_uni.py
```

### Comparing `onion_clustering-0.1.5/LICENSE` & `onion_clustering-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.5/PKG-INFO` & `onion_clustering-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.1.5
+Version: 0.2.0
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.1.5/README.md` & `onion_clustering-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.5/examples/example_script.py` & `onion_clustering-0.2.0/examples/example_script.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.5/examples/example_script_2d.py` & `onion_clustering-0.2.0/examples/example_script_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.5/justfile` & `onion_clustering-0.2.0/justfile`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 check:
   #!/usr/bin/env bash
 
   error=0
   trap error=1 ERR
 
   echo
-  (set -x; ruff . )
+  (set -x; ruff check . )
 
   echo
   ( set -x; ruff format --check . )
 
   echo
   ( set -x; mypy . )
```

### Comparing `onion_clustering-0.1.5/pyproject.toml` & `onion_clustering-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onion_clustering"
-version = "0.1.5"
+version = "0.2.0"
 description = "Code for unsupervised clustering of time-correlated data."
 # license = "MIT"
 maintainers = [
   { name = "Matteo Becchi", email = "bechmath@gmail.com" },
 ]
 dependencies = [
   "matplotlib",
@@ -26,15 +26,15 @@
 #write_to = "src/onion_clustering/__version__.py"
 
 [tool.black]
 line-length = 79
 
 [tool.ruff]
 line-length = 79
-extend-select = ["I"]
+lint.extend-select = ["I"]
 
 [tool.mypy]
 show_error_codes = true
 implicit_optional = false
 warn_no_return = true
 strict_optional = true
```

### Comparing `onion_clustering-0.1.5/src/onion_clustering/classes.py` & `onion_clustering-0.2.0/src/onion_clustering/classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,20 +24,29 @@
 
 COLORMAP = "viridis"
 
 
 class ClusteringObject:
     """This class contains input, output and methods for plotting."""
 
-    def __init__(self, par: Parameters, data: Union[UniData, MultiData]):
+    def __init__(
+        self,
+        par: Parameters,
+        data: Union[UniData, MultiData],
+        number_of_sigmas: float,
+    ):
         self.par = par
+        self.number_of_sigmas = number_of_sigmas
         self.data = data
         self.iterations = -1
+        self.tau_window_list: np.ndarray
+        self.t_smooth_list: np.ndarray
         self.number_of_states: np.ndarray
         self.fraction_0: np.ndarray
+        self.list_of_pop: List[List[List[float]]]
 
     def plot_input_data(self, filename: str):
         """Plots input data for visualization."""
         raise NotImplementedError
 
     def preparing_the_data(self):
         """Processes raw data for analysis."""
@@ -322,14 +331,57 @@
             fig.savefig(
                 "output_figures/Time_resolution_analysis_"
                 + str(t_smooth)
                 + ".png",
                 dpi=600,
             )
 
+    def plot_pop_fractions(self):
+        """
+        Plot, for every time resolution, the populations of the ENVs.
+
+        The bottom state is the ENV0.
+        """
+        print("* Print populations fractions...")
+
+        t_conv, units = self.par.t_conv, self.par.t_units
+        time = self.tau_window_list * t_conv
+
+        for i, t_smooth in enumerate(self.t_smooth_list):
+            pop_array = self.list_of_pop[i]
+
+            max_num_of_states = np.max(
+                [len(pop_list) for pop_list in pop_array]
+            )
+            for j, pop_list in enumerate(pop_array):
+                while len(pop_list) < max_num_of_states:
+                    pop_array[j].append(0.0)
+
+            pop_array = np.array(pop_array)
+
+            fig, axes = plt.subplots()
+            width = time[1:] - time[:-1]
+            width = np.insert(width, 0, width[0] / 2)
+
+            bottom = np.zeros(len(pop_array))
+            for j, state in enumerate(pop_array.T):
+                _ = axes.bar(
+                    time, state, width, bottom=bottom, edgecolor="black"
+                )
+                bottom += state
+
+            axes.set_xlabel(rf"Time resolution $\Delta t$ {units}")
+            axes.set_ylabel(r"Population's fractions")
+            axes.set_xscale("log")
+
+            fig.savefig(
+                f"output_figures/Populations_{t_smooth}.png",
+                dpi=600,
+            )
+
 
 class ClusteringObject1D(ClusteringObject):
     """This class contains input, output and methods for plotting."""
 
     states: List[StateUni] = []
 
     def plot_input_data(self, filename: str):
```

### Comparing `onion_clustering-0.1.5/src/onion_clustering/first_classes.py` & `onion_clustering-0.2.0/src/onion_clustering/first_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,15 @@
         - Saves the figure as a PNG file in the 'output_figures' directory.
         """
         tau_window = int(self.num_of_steps / self.labels.shape[1])
         all_the_labels = self.labels
         # Initialize lists to store cluster means and standard deviations
         center_list = []
         std_list = []
+        env0 = []
 
         # If there are no assigned window, we still need the "0" state
         # for consistency:
         missing_zero = 0
         list_of_labels = np.unique(all_the_labels)
         if 0 not in list_of_labels:
             list_of_labels = np.insert(list_of_labels, 0, 0)
@@ -230,17 +231,19 @@
                     time_1 = (window + 1) * tau_window
                     # If the label matches the current cluster,
                     # append the corresponding data to tmp
                     if label == ref_label:
                         tmp.append(self.matrix[i][time_0:time_1])
 
             # Calculate mean and standard deviation for the current cluster
-            if len(tmp) > 0:
+            if len(tmp) > 0 and ref_label > 0:
                 center_list.append(np.mean(tmp, axis=0))
                 std_list.append(np.std(tmp, axis=0))
+            elif len(tmp) > 0:
+                env0 = tmp
 
         center_arr = np.array(center_list)
         std_arr = np.array(std_list)
         np.savetxt(
             "medoid_center.txt",
             center_arr,
             header="Signal average for each ENV",
@@ -266,28 +269,40 @@
             err_inf = center - std_list[center_id]
             err_sup = center + std_list[center_id]
             axes.fill_between(
                 time_seq,
                 err_inf,
                 err_sup,
                 alpha=0.25,
-                color=palette[center_id + missing_zero],
+                color=palette[center_id + missing_zero + 1],
             )
             axes.plot(
                 time_seq,
                 center,
                 label="ENV" + str(center_id + missing_zero),
                 marker="o",
-                c=palette[center_id + missing_zero],
+                c=palette[center_id + missing_zero + 1],
+                zorder=1,
             )
+
+        for window in env0:
+            axes.plot(
+                time_seq,
+                window,
+                lw=0.1,
+                c=palette[0],
+                zorder=0,
+                alpha=0.25,
+            )
+
         fig.suptitle("Average time sequence inside each environments")
         axes.set_xlabel(r"Time $t$ [frames]")
         axes.set_ylabel(r"Signal")
         axes.xaxis.set_major_locator(MaxNLocator(integer=True))
-        axes.legend()
+        axes.legend(loc="lower left")
 
         fig.savefig("output_figures/Fig4.png", dpi=600)
 
 
 class MultiData:
     """
     The input signals of the analysis.
```

### Comparing `onion_clustering-0.1.5/src/onion_clustering/functions.py` & `onion_clustering-0.2.0/src/onion_clustering/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -475,15 +475,14 @@
     # Compute the fraction of data points in each state
     for st_id, state in enumerate(updated_states):
         num_of_points = np.sum(all_the_labels == st_id + 1)
         state.perc = num_of_points / all_the_labels.size
 
     # Step 2: Calculate the final threshold values
     # and their types based on the intercept between neighboring states.
-
     updated_states[0].th_inf[0] = m_range[0]
     updated_states[0].th_inf[1] = 0
 
     for i in range(len(updated_states) - 1):
         th_val, th_type = find_intersection(
             updated_states[i], updated_states[i + 1]
         )
@@ -491,34 +490,24 @@
         updated_states[i].th_sup[1] = th_type
         updated_states[i + 1].th_inf[0] = th_val
         updated_states[i + 1].th_inf[1] = th_type
 
     updated_states[-1].th_sup[0] = m_range[1]
     updated_states[-1].th_sup[1] = 0
 
-    # if updated_states[0].th_sup[0] < m_range[0]:
-    #     updated_states.pop(0)
-    #     updated_states[0].th_inf[0] = m_range[0]
-    #     mask = all_the_labels > 1
-    #     all_the_labels[mask] -= 1
-
-    # if updated_states[-1].th_inf[0] > m_range[1]:
-    #     updated_states.pop(-1)
-    #     updated_states[-1].th_inf[1] = m_range[1]
-    #     mask = all_the_labels == np.max(all_the_labels)
-    #     all_the_labels[mask] -= 1
-
     # Step 3: Write the final states and final thresholds to text files.
     # The data is saved in two separate files:
     # 'final_states.txt' and 'final_thresholds.txt'.
-    with open("final_states.txt", "w", encoding="utf-8") as file:
+    with open("final_states.txt", "a", encoding="utf-8") as file:
+        print("####################################", file=file)
         print("# Mu \t Sigma \t A \t state_fraction", file=file)
         for state in updated_states:
             print(state.mean, state.sigma, state.area, state.perc, file=file)
-    with open("final_thresholds.txt", "w", encoding="utf-8") as file:
+    with open("final_thresholds.txt", "a", encoding="utf-8") as file:
+        print("####################################", file=file)
         for state in updated_states:
             print(state.th_inf[0], state.th_inf[1], file=file)
         print(
             updated_states[-1].th_sup[0],
             updated_states[-1].th_sup[1],
             file=file,
         )
```

### Comparing `onion_clustering-0.1.5/src/onion_clustering/main.py` & `onion_clustering-0.2.0/src/onion_clustering/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,18 @@
     param_grid,
     plot_histo,
     read_input_data,
     relabel_states,
     set_final_states,
 )
 
-NUMBER_OF_SIGMAS = 2.0
 OUTPUT_FILE = "states_output.txt"
 
 
-def all_the_input_stuff() -> ClusteringObject1D:
+def all_the_input_stuff(number_of_sigmas: float) -> ClusteringObject1D:
     """
     Reads input parameters and raw data from specified files and directories,
     processes the raw data, and creates output files.
     """
     # Read input parameters from files.
     data_directory = read_input_data()
     par = Parameters("input_parameters.txt")
@@ -59,21 +58,23 @@
             if os.path.isfile(file_path):
                 os.remove(file_path)
             elif os.path.isdir(file_path):
                 shutil.rmtree(file_path)
         except OSError as ex_msg:
             print(f"Failed to delete {file_path}. Reason: {ex_msg}")
 
-    clustering_object = ClusteringObject1D(par, data)
+    clustering_object = ClusteringObject1D(par, data, number_of_sigmas)
 
     return clustering_object
 
 
 def perform_gauss_fit(
-    param: List[int], data: List[np.ndarray], int_type: str
+    param: List[int],
+    data: List[np.ndarray],
+    int_type: str,
 ) -> Tuple[bool, int, np.ndarray]:
     """
     Perform Gaussian fit on given data.
 
     Args:
     - id0 (int): Index representing the lower limit for data selection.
     - id1 (int): Index representing the upper limit for data selection.
@@ -93,27 +94,27 @@
     id0, id1, max_ind, n_data, gap = param
     bins, counts = data
 
     goodness = 5
     selected_bins = bins[id0:id1]
     selected_counts = counts[id0:id1]
     mu0 = bins[max_ind]
-    sigma0 = (bins[id0] - bins[id1]) / 6
+    sigma0 = (bins[id1] - bins[id0]) / 6
     area0 = counts[max_ind] * np.sqrt(np.pi) * sigma0
     try:
         popt, pcov, _, _, _ = scipy.optimize.curve_fit(
             gaussian,
             selected_bins,
             selected_counts,
             p0=[mu0, sigma0, area0],
             full_output=True,
         )
         if popt[1] < 0:
-            popt[1] = -popt[1]
-            popt[2] = -popt[2]
+            popt[1] *= -1
+            popt[2] *= -1
         gauss_max = popt[2] * np.sqrt(np.pi) * popt[1]
         if gauss_max < area0 / 2:
             goodness -= 1
         popt[2] *= n_data
         if popt[0] < selected_bins[0] or popt[0] > selected_bins[-1]:
             goodness -= 1
         if popt[1] > selected_bins[-1] - selected_bins[0]:
@@ -151,15 +152,19 @@
             np.empty(
                 3,
             ),
         )
 
 
 def gauss_fit_max(
-    m_clean: np.ndarray, par: Parameters, filename: str, full_out: bool
+    m_clean: np.ndarray,
+    par: Parameters,
+    number_of_sigmas: float,
+    filename: str,
+    full_out: bool,
 ) -> Union[StateUni, None]:
     """
     Performs Gaussian fitting on input data.
 
     Args:
     - m_clean (np.ndarray): Input data for Gaussian fitting.
     - par (Parameters): Object containing parameters for fitting.
@@ -171,16 +176,17 @@
     """
     print("* Gaussian fit...")
     flat_m = m_clean.flatten()
 
     ### 1. Histogram ###
     counts, bins = np.histogram(flat_m, bins=par.bins, density=True)
     gap = 1
-    if bins.size > 50:
-        gap = 3
+    if bins.size > 99:
+        gap = int(bins.size * 0.02)
+    print(f"\tNumber of bins = {bins.size}, gap = {gap}")
 
     ### 2. Smoothing with tau = 3 ###
     counts = moving_average(counts, gap)
     bins = moving_average(bins, gap)
     if (counts == 0.0).any():
         print(
             "\tWARNING: there are empty bins. "
@@ -217,14 +223,23 @@
     ### 7. Try the fit between the minima and check its goodness ###
     fit_param = [half_id0, half_id1, max_ind, flat_m.size, gap]
     fit_data = [bins, counts]
     flag_half, goodness_half, popt_half = perform_gauss_fit(
         fit_param, fit_data, "Half"
     )
 
+    ### 7.bis Avoid that the ENV0 is hidden in a very large Gaussian ###
+    data_range = np.max(m_clean) - np.min(m_clean)
+    if popt_min[1] > data_range / 4:
+        print("\tWARNING: sigma is too large, fit discarded.")
+        flag_min = False
+    if popt_half[1] > data_range / 4:
+        print("\tWARNING: sigma is too large, fit discarded.")
+        flag_half = False
+
     ### 8. Choose the best fit ###
     goodness = goodness_min
     if flag_min == 1 and flag_half == 0:
         popt = popt_min
     elif flag_min == 0 and flag_half == 1:
         popt = popt_half
         goodness = goodness_half
@@ -235,15 +250,15 @@
             popt = popt_half
             goodness = goodness_half
     else:
         print("\tWARNING: this fit is not converging.")
         return None
 
     state = StateUni(popt[0], popt[1], popt[2])
-    state.build_boundaries(NUMBER_OF_SIGMAS)
+    state.build_boundaries(number_of_sigmas)
 
     with open(OUTPUT_FILE, "a", encoding="utf-8") as file:
         print("\n", file=file)
         print(
             f"\tmu = {state.mean:.4f}, sigma = {state.sigma:.4f},"
             f" area = {state.area:.4f}"
         )
@@ -344,15 +359,17 @@
 
     # Return the array of non-stable windows, the fraction of stable windows,
     # and the updated list_of_states
     return m2_array, window_fraction, one_last_state
 
 
 def iterative_search(
-    cl_ob: ClusteringObject1D, name: str, full_out: bool
+    cl_ob: ClusteringObject1D,
+    name: str,
+    full_out: bool,
 ) -> Tuple[ClusteringObject1D, np.ndarray, bool]:
     """
     Performs an iterative search for stable states in a trajectory.
 
     Args:
     - cl_ob (ClusteringObject1D).
     - name (str): Name for identifying output figures.
@@ -365,24 +382,28 @@
 
     # Initialize an array to store labels for each window.
     num_windows = int(cl_ob.data.num_of_steps / cl_ob.par.tau_w)
     tmp_labels = np.zeros((cl_ob.data.num_of_particles, num_windows)).astype(
         int
     )
 
+    with open(OUTPUT_FILE, "a", encoding="utf-8") as file:
+        print(f"tau_window = {cl_ob.par.tau_w}", file=file)
+
     states_list = []
     m_copy = cl_ob.data.matrix
     iteration_id = 1
     states_counter = 0
     one_last_state = False
     while True:
         ### Locate and fit maximum in the signal distribution
         state = gauss_fit_max(
             m_copy,
             cl_ob.par,
+            cl_ob.number_of_sigmas,
             "output_figures/" + name + "Fig1_" + str(iteration_id),
             full_out,
         )
         if state is None:
             print("Iterations interrupted because fit does not converge. ")
             break
 
@@ -395,36 +416,44 @@
         states_list.append(state)
         states_counter += 1
         iteration_id += 1
         ### Exit the loop if no new stable windows are found
         if counter <= 0.0:
             print("Iterations interrupted because last state is empty. ")
             break
+        if m_next.size == 0:
+            print("Iterations interrupted because all points are classififed.")
+            break
         m_copy = m_next
 
     cl_ob.iterations = len(states_list)
     atl, lis = relabel_states(tmp_labels, states_list)
     cl_ob.states = lis
     return cl_ob, atl, one_last_state
 
 
 def timeseries_analysis(
-    cl_ob: ClusteringObject1D, tau_w: int, t_smooth: int, full_out: bool
-) -> Tuple[int, float]:
+    cl_ob: ClusteringObject1D,
+    tau_w: int,
+    t_smooth: int,
+    full_out: bool,
+) -> Tuple[int, float, List[float]]:
     """
     Performs an analysis pipeline on time series data.
 
     Args:
     - cl_ob (ClusteringObject1D)
     - tau_w (int): the time window for the analysis
     - t_smooth (int): the width of the moving average for the analysis
 
     Returns:
     - num_states (int): Number of identified states.
     - fraction_0 (float): Fraction of unclassified data points.
+    - list_of_pop (List[float]): List of the populations of the different
+        states.
     """
 
     print("* New analysis: ", tau_w, t_smooth)
     name = str(t_smooth) + "_" + str(tau_w) + "_"
 
     tmp_cl_ob = copy.deepcopy(cl_ob)
     tmp_cl_ob.par.tau_w = tau_w
@@ -437,37 +466,37 @@
         tmp_cl_ob, name, full_out
     )
 
     if len(tmp_cl_ob.states) == 0:
         print("* No possible classification was found. ")
         # We need to free the memory otherwise it accumulates
         del tmp_cl_ob
-        return 1, 1.0
+        return 0, 1.0, [1.0]
 
     tmp_cl_ob.states, tmp_cl_ob.data.labels = set_final_states(
         tmp_cl_ob.states, tmp_labels, tmp_cl_ob.data.range
     )
 
-    fraction_0 = 1 - np.sum([state.perc for state in tmp_cl_ob.states])
+    list_of_pop = [state.perc for state in tmp_cl_ob.states]
+    fraction_0 = 1 - np.sum(list_of_pop)
+    list_of_pop.insert(0, fraction_0)
     n_states = len(tmp_cl_ob.states)
 
-    if one_last_state:
-        n_states += 1
-
     # We need to free the memory otherwise it accumulates
     del tmp_cl_ob
 
     print(
         "Number of states identified:", n_states, "[" + str(fraction_0) + "]\n"
     )
-    return n_states, fraction_0
+    return n_states, fraction_0, list_of_pop
 
 
 def full_output_analysis(
-    cl_ob: ClusteringObject1D, full_out: bool
+    cl_ob: ClusteringObject1D,
+    full_out: bool,
 ) -> ClusteringObject1D:
     """Perform a comprehensive analysis on the input data."""
 
     cl_ob.preparing_the_data()
 
     cl_ob, tmp_labels, _ = iterative_search(cl_ob, "", full_out)
     if len(cl_ob.states) == 0:
@@ -487,26 +516,34 @@
 
     Args:
     - cl_ob (ClusteringObject1D): Conteining now only the raw input data.
     """
     tau_window_list, t_smooth_list = param_grid(
         cl_ob.par, cl_ob.data.num_of_steps
     )
+    cl_ob.tau_window_list = np.array(tau_window_list)
+    cl_ob.t_smooth_list = np.array(t_smooth_list)
 
     number_of_states = []
     fraction_0 = []
-    for tau_w in tau_window_list:
+    list_of_pop: List[List[List[float]]] = [
+        [[] for _ in tau_window_list] for _ in t_smooth_list
+    ]
+
+    for i, tau_w in enumerate(tau_window_list):
         tmp = [tau_w]
         tmp1 = [tau_w]
-        for t_s in t_smooth_list:
-            n_s, f_0 = timeseries_analysis(cl_ob, tau_w, t_s, full_out)
+        for j, t_s in enumerate(t_smooth_list):
+            n_s, f_0, l_pop = timeseries_analysis(cl_ob, tau_w, t_s, full_out)
             tmp.append(n_s)
             tmp1.append(f_0)
+            list_of_pop[j][i] = l_pop
         number_of_states.append(tmp)
         fraction_0.append(tmp1)
+
     number_of_states_arr = np.array(number_of_states)
     fraction_0_arr = np.array(fraction_0)
 
     np.savetxt(
         "number_of_states.txt",
         number_of_states,
         fmt="%i",
@@ -518,32 +555,36 @@
         fraction_0,
         delimiter=" ",
         header="tau_window\t fraction in ENV0 for different t_smooth",
     )
 
     cl_ob.number_of_states = number_of_states_arr
     cl_ob.fraction_0 = fraction_0_arr
+    cl_ob.list_of_pop = list_of_pop
 
 
-def main(full_output: bool = True) -> ClusteringObject1D:
+def main(
+    full_output: bool = True,
+    number_of_sigmas: float = 1.5,
+) -> ClusteringObject1D:
     """
     Returns the clustering object with the analysi.
 
     all_the_input_stuff() reads the data and the parameters
     time_resolution_analysis() explore the parameter
         (tau_window, t_smooth) space.
     full_output_analysis() performs a detailed analysis
         with the chosen parameters.
     """
     print("##############################################################")
     print("# If you publish results using onion-clustering, please cite #")
     print("# this work: https://doi.org/10.48550/arXiv.2402.07786.      #")
     print("##############################################################")
 
-    clustering_object = all_the_input_stuff()
+    clustering_object = all_the_input_stuff(number_of_sigmas)
     time_resolution_analysis(clustering_object, full_output)
     clustering_object = full_output_analysis(clustering_object, full_output)
 
     return clustering_object
 
 
 if __name__ == "__main__":
```

### Comparing `onion_clustering-0.1.5/src/onion_clustering/main_2d.py` & `onion_clustering-0.2.0/src/onion_clustering/main_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     relabel_states_2d,
 )
 
 NUMBER_OF_SIGMAS = 2.0
 OUTPUT_FILE = "states_output.txt"
 
 
-def all_the_input_stuff() -> ClusteringObject2D:
+def all_the_input_stuff(number_of_sigmas: float) -> ClusteringObject2D:
     """
     Reads input parameters and raw data from specified files and directories,
     processes the raw data, and creates output files.
     """
     # Read input parameters from files.
     data_directory = read_input_data()
     par = Parameters("input_parameters.txt")
@@ -52,23 +52,24 @@
             if os.path.isfile(file_path):
                 os.remove(file_path)
             elif os.path.isdir(file_path):
                 shutil.rmtree(file_path)
         except OSError as exc_msg:
             print(f"Failed to delete {file_path}. Reason: {exc_msg}")
 
-    clustering_object = ClusteringObject2D(par, data)
+    clustering_object = ClusteringObject2D(par, data, number_of_sigmas)
 
     return clustering_object
 
 
 def gauss_fit_max(
     m_clean: np.ndarray,
     m_limits: np.ndarray,
     bins: Union[int, str],
+    number_of_sigmas: float,
     filename: str,
     full_out: bool,
 ) -> Union[StateMulti, None]:
     """
     Perform Gaussian fit and generate plots based on the provided data.
 
     Args:
@@ -281,15 +282,15 @@
     ### Find the tresholds for state identification
     mean, sigma, area = [], [], []
     for dim in range(m_clean.shape[2]):
         mean.append(popt[3 * dim])
         sigma.append(popt[3 * dim + 1])
         area.append(popt[3 * dim + 2])
     state = StateMulti(np.array(mean), np.array(sigma), np.array(area))
-    state.build_boundaries(NUMBER_OF_SIGMAS)
+    state.build_boundaries(number_of_sigmas)
 
     ### Plot the distribution and the fitted Gaussians
     if m_clean.shape[2] == 2:
         with open(OUTPUT_FILE, "a", encoding="utf-8") as file:
             print("\n", file=file)
             print(
                 f"\tmu = [{popt[0]:.4f}, {popt[3]:.4f}],"
@@ -497,15 +498,17 @@
 
     # Return the array of non-stable windows, the fraction of stable windows,
     # and the updated list_of_states
     return m_new_arr, fraction_of_points, one_last_state
 
 
 def iterative_search(
-    cl_ob: ClusteringObject2D, name: str, full_out: bool
+    cl_ob: ClusteringObject2D,
+    name: str,
+    full_out: bool,
 ) -> Tuple[ClusteringObject2D, bool]:
     """
     Perform an iterative search to identify stable windows in trajectory data.
 
     Args:
     - name (str): Name for the output figures.
 
@@ -528,14 +531,15 @@
     one_last_state = False
     while True:
         ### Locate and fit maximum in the signal distribution
         state = gauss_fit_max(
             m_copy,
             np.array(cl_ob.data.range),
             bins,
+            cl_ob.number_of_sigmas,
             "output_figures/" + name + "Fig1_" + str(iteration_id),
             full_out,
         )
         if state is None:
             print("Iterations interrupted because fit does not converge. ")
             break
 
@@ -563,15 +567,18 @@
     all_the_labels, list_of_states = relabel_states_2d(tmp_labels, states_list)
     cl_ob.data.labels = all_the_labels
     cl_ob.states = list_of_states
     return cl_ob, one_last_state
 
 
 def timeseries_analysis(
-    cl_ob: ClusteringObject2D, tau_w: int, t_smooth: int, full_out: bool
+    cl_ob: ClusteringObject2D,
+    tau_w: int,
+    t_smooth: int,
+    full_out: bool,
 ) -> Tuple[int, float]:
     """
     Perform time series analysis on the input data.
 
     Args:
     - cl_ob (ClusteringObject)
     - tau_w (int): the time window for the analysis
@@ -612,15 +619,16 @@
     print(
         "Number of states identified:", n_states, "[" + str(fraction_0) + "]\n"
     )
     return n_states, fraction_0
 
 
 def full_output_analysis(
-    cl_ob: ClusteringObject2D, full_out: bool
+    cl_ob: ClusteringObject2D,
+    full_out: bool,
 ) -> ClusteringObject2D:
     """Perform a comprehensive analysis on the input data."""
 
     cl_ob.preparing_the_data()
 
     cl_ob, _ = iterative_search(cl_ob, "", full_out)
     if len(cl_ob.states) == 0:
@@ -673,30 +681,32 @@
 
     cl_ob.number_of_states = number_of_states_arr
     cl_ob.fraction_0 = fraction_0_arr
 
     cl_ob.plot_tra_figure()
 
 
-def main(full_output: bool = True) -> ClusteringObject2D:
+def main(
+    full_output: bool = True, number_of_sigmas: float = 2.0
+) -> ClusteringObject2D:
     """
     Returns the clustering object with the analysi.
 
     all_the_input_stuff() reads the data and the parameters
     time_resolution_analysis() explore the parameter
         (tau_window, t_smooth) space.
     full_output_analysis() performs a detailed analysis
         with the chosen parameters.
     """
     print("##############################################################")
     print("# If you publish results using onion-clustering, please cite #")
     print("# this work: https://doi.org/10.48550/arXiv.2402.07786.      #")
     print("##############################################################")
 
-    clustering_object = all_the_input_stuff()
+    clustering_object = all_the_input_stuff(number_of_sigmas)
     time_resolution_analysis(clustering_object, full_output)
     clustering_object = full_output_analysis(clustering_object, full_output)
 
     return clustering_object
 
 
 if __name__ == "__main__":
```

### Comparing `onion_clustering-0.1.5/src/onion_clustering/utilities.py` & `onion_clustering-0.2.0/src/onion_clustering/utilities.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.5/src/onion_clustering.egg-info/PKG-INFO` & `onion_clustering-0.2.0/src/onion_clustering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.1.5
+Version: 0.2.0
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.1.5/src/onion_clustering.egg-info/SOURCES.txt` & `onion_clustering-0.2.0/src/onion_clustering.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 README.md
 justfile
 pyproject.toml
 pytest.ini
 examples/example_script.py
 examples/example_script_2d.py
 src/onion_clustering/__init__.py
-src/onion_clustering/__version__.py
 src/onion_clustering/classes.py
 src/onion_clustering/first_classes.py
 src/onion_clustering/functions.py
 src/onion_clustering/main.py
 src/onion_clustering/main_2d.py
 src/onion_clustering/utilities.py
 src/onion_clustering.egg-info/PKG-INFO
```

### Comparing `onion_clustering-0.1.5/test/test_multi.py` & `onion_clustering-0.2.0/test/test_multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,18 @@
         original_dir
     )  # Restore the original working directory after the test
 
 
 # Define the actual test
 def test_output_files(setup_test_environment):
     ### Set all the analysis parameters ###
-    PATH_TO_INPUT_DATA = ("/Users/mattebecchi/00_signal_analysis/data/"
-        "synthetic_2D/3D_synthetic_data.npy")
+    PATH_TO_INPUT_DATA = (
+        "/Users/mattebecchi/00_signal_analysis/data/"
+        "synthetic_2D/3D_synthetic_data.npy"
+    )
     TAU_WINDOW = 10  # time resolution of the analysis
     T_CONV = 200  # convert frames in time units (default 1)
     T_UNITS = "dt"  # the time units (default 'frames')
     NUM_TAU_W = 2  # number of tau_window tested (default 20)
     MAX_TAU_W = 10  # max value of tau_window tested (default auto)
     MAX_T_SMOOTH = 2  # max value of t_smooth tested (default 5)
     BINS = 50  # number of histogram bins (default auto)
```

### Comparing `onion_clustering-0.1.5/test/test_uni.py` & `onion_clustering-0.2.0/test/test_uni.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 import os
 
 import pytest
-from onion_clustering import main
+from onion_clustering import main as onion
+
+### Set all the analysis parameters ###
+FILE = "water_coex_100ps_1nm_LENS.npy"
+PATH_TO_INPUT_DATA = "/Users/mattebecchi/00_signal_analysis/data/" + FILE
+TAU_WINDOW = 10  # time resolution of the analysis
+T_DELAY = 1  # remove the first t_delay frames (default 0)
+T_CONV = 0.1  # convert frames in time units (default 1)
+T_UNITS = "ns"  # the time units (default 'frames')
+NUM_TAU_W = 2
+MAX_TAU_W = 10
+MAX_T_SMOOTH = 2  # max value of t_smooth tested (default 5)
 
 
 # Define a fixture to set up the test environment
 @pytest.fixture
 def setup_test_environment(tmpdir):
     # tmpdir is a built-in pytest fixture providing a temporary directory
     original_dir = os.getcwd()  # Save the current working directory
@@ -14,25 +25,14 @@
     os.chdir(
         original_dir
     )  # Restore the original working directory after the test
 
 
 # Define the actual test
 def test_output_files(setup_test_environment):
-    ### Set all the analysis parameters ###
-    FILE = "water_coex_100ps_1nm_LENS.npy"
-    PATH_TO_INPUT_DATA = "/Users/mattebecchi/00_signal_analysis/data/" + FILE
-    TAU_WINDOW = 10  # time resolution of the analysis
-    T_DELAY = 1  # remove the first t_delay frames (default 0)
-    T_CONV = 0.1  # convert frames in time units (default 1)
-    T_UNITS = "ns"  # the time units (default 'frames')
-    NUM_TAU_W = 2
-    MAX_TAU_W = 10
-    MAX_T_SMOOTH = 2  # max value of t_smooth tested (default 5)
-
     ### Create the 'data_directory.txt' file ###
     with open("data_directory.txt", "w+", encoding="utf-8") as file:
         print(PATH_TO_INPUT_DATA, file=file)
 
     ### Create the 'input_parameter.txt' file ###
     with open("input_parameters.txt", "w+", encoding="utf-8") as file:
         print("tau_window\t" + str(TAU_WINDOW), file=file)
@@ -40,25 +40,26 @@
         print("t_conv\t" + str(T_CONV), file=file)
         print("t_units\t" + T_UNITS, file=file)
         print("num_tau_w\t" + str(NUM_TAU_W), file=file)
         print("max_tau_w\t" + str(MAX_TAU_W), file=file)
         print("max_t_smooth\t" + str(MAX_T_SMOOTH), file=file)
 
     # Call your code to generate the output files
-    tmp = main.main()
+    tmp = onion.main(False)
 
     # Test the output
     tmp.plot_tra_figure()
     tmp.plot_input_data("Fig0")
     tmp.plot_cumulative_figure()
     tmp.plot_one_trajectory()
     tmp.data.plot_medoids()
     tmp.plot_state_populations()
     tmp.sankey([0, 10, 20, 30, 40])
     tmp.print_labels()
+    tmp.plot_pop_fractions()
 
     # Define the paths to the expected and actual output files
     original_dir = (
         "/Users/mattebecchi/00_signal_analysis/timeseries_analysis/test/"
     )
     expected_output_path_1 = original_dir + "output_uni/final_states.txt"
     expected_output_path_2 = original_dir + "output_uni/number_of_states.txt"
```

