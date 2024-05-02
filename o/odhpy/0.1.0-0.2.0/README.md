# Comparing `tmp/odhpy-0.1.0.tar.gz` & `tmp/odhpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odhpy-0.1.0.tar", last modified: Fri Apr 26 05:33:50 2024, max compression
+gzip compressed data, was "odhpy-0.2.0.tar", last modified: Thu May  2 00:18:35 2024, max compression
```

## Comparing `odhpy-0.1.0.tar` & `odhpy-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.543233 odhpy-0.1.0/
--rw-rw-rw-   0        0        0     2793 2024-04-26 05:33:50.542233 odhpy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2175 2024-04-03 03:37:24.000000 odhpy-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 05:33:50.544233 odhpy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      960 2024-03-19 03:03:09.000000 odhpy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.502233 odhpy-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.511232 odhpy-0.1.0/src/odhpy/
--rw-rw-rw-   0        0        0       76 2024-03-14 03:25:23.000000 odhpy-0.1.0/src/odhpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.517233 odhpy-0.1.0/src/odhpy/clim/
--rw-rw-rw-   0        0        0       21 2024-03-14 03:25:23.000000 odhpy-0.1.0/src/odhpy/clim/__init__.py
--rw-rw-rw-   0        0        0     6756 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/clim/clim.py
--rw-rw-rw-   0        0        0      128 2024-03-14 03:25:23.000000 odhpy-0.1.0/src/odhpy/demo.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.523245 odhpy-0.1.0/src/odhpy/io/
--rw-rw-rw-   0        0        0      128 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/io/__init__.py
--rw-rw-rw-   0        0        0     4256 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/io/csv_io.py
--rw-rw-rw-   0        0        0     2868 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/io/idx_io.py
--rw-rw-rw-   0        0        0     6065 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/io/iqqm_out_reader.py
--rw-rw-rw-   0        0        0     1705 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/io/lqn_io.py
--rw-rw-rw-   0        0        0     3059 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/io/res_csv_io.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.525233 odhpy-0.1.0/src/odhpy/maps/
--rw-rw-rw-   0        0        0       29 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/maps/__init__.py
--rw-rw-rw-   0        0        0     5090 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/maps/station_maps.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.529233 odhpy-0.1.0/src/odhpy/plots/
--rw-rw-rw-   0        0        0      121 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/plots/__init__.py
--rw-rw-rw-   0        0        0    23149 2024-04-26 05:19:03.000000 odhpy-0.1.0/src/odhpy/plots/altair_plots.py
--rw-rw-rw-   0        0        0      274 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/plots/node_diagrams.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/plots/plot_functions.py
--rw-rw-rw-   0        0        0        0 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/plots/plotly_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.532233 odhpy-0.1.0/src/odhpy/stats/
--rw-rw-rw-   0        0        0      111 2024-03-18 23:58:54.000000 odhpy-0.1.0/src/odhpy/stats/__init__.py
--rw-rw-rw-   0        0        0     2498 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/stats/aggregate_stats.py
--rw-rw-rw-   0        0        0    12092 2024-04-03 03:37:24.000000 odhpy-0.1.0/src/odhpy/stats/reliability_stats_class.py
--rw-rw-rw-   0        0        0     9163 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/stats/storage_level_assessment.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.534233 odhpy-0.1.0/src/odhpy/stats/swflo2s/
--rw-rw-rw-   0        0        0       22 2024-04-03 03:37:24.000000 odhpy-0.1.0/src/odhpy/stats/swflo2s/__init__.py
--rw-rw-rw-   0        0        0     6755 2024-04-03 03:37:24.000000 odhpy-0.1.0/src/odhpy/stats/swflo2s/swflo2s.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.536233 odhpy-0.1.0/src/odhpy/stoch/
--rw-rw-rw-   0        0        0       23 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/stoch/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/stoch/analyse.py
--rw-rw-rw-   0        0        0     2867 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/stoch/generate.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.538233 odhpy-0.1.0/src/odhpy/trans/
--rw-rw-rw-   0        0        0       27 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/trans/__init__.py
--rw-rw-rw-   0        0        0     2953 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/trans/transformers.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.542233 odhpy-0.1.0/src/odhpy/utils/
--rw-rw-rw-   0        0        0       99 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/utils/__init__.py
--rw-rw-rw-   0        0        0    11382 2024-04-03 03:37:24.000000 odhpy-0.1.0/src/odhpy/utils/dataframe_functions.py
--rw-rw-rw-   0        0        0    10157 2024-03-19 03:03:09.000000 odhpy-0.1.0/src/odhpy/utils/datetime_functions.py
--rw-rw-rw-   0        0        0      753 2024-03-14 03:25:24.000000 odhpy-0.1.0/src/odhpy/utils/interpolation.py
--rw-rw-rw-   0        0        0      210 2024-04-26 05:24:30.000000 odhpy-0.1.0/src/odhpy/version.py
-drwxrwxrwx   0        0        0        0 2024-04-26 05:33:50.516232 odhpy-0.1.0/src/odhpy.egg-info/
--rw-rw-rw-   0        0        0     2793 2024-04-26 05:33:50.000000 odhpy-0.1.0/src/odhpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2024-04-26 05:33:50.000000 odhpy-0.1.0/src/odhpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 05:33:50.000000 odhpy-0.1.0/src/odhpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-26 05:33:50.000000 odhpy-0.1.0/src/odhpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 05:33:50.000000 odhpy-0.1.0/src/odhpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:35.004766 odhpy-0.2.0/
+-rw-rw-rw-   0        0        0     2793 2024-05-02 00:18:35.002847 odhpy-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2024-04-03 03:37:24.000000 odhpy-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 00:18:35.004766 odhpy-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      960 2024-03-19 03:03:09.000000 odhpy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.877772 odhpy-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.910731 odhpy-0.2.0/src/odhpy/
+-rw-rw-rw-   0        0        0       76 2024-03-14 03:25:23.000000 odhpy-0.2.0/src/odhpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.931285 odhpy-0.2.0/src/odhpy/clim/
+-rw-rw-rw-   0        0        0       21 2024-03-14 03:25:23.000000 odhpy-0.2.0/src/odhpy/clim/__init__.py
+-rw-rw-rw-   0        0        0     6756 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/clim/clim.py
+-rw-rw-rw-   0        0        0      128 2024-03-14 03:25:23.000000 odhpy-0.2.0/src/odhpy/demo.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.945030 odhpy-0.2.0/src/odhpy/io/
+-rw-rw-rw-   0        0        0      128 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/io/__init__.py
+-rw-rw-rw-   0        0        0     4256 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/io/csv_io.py
+-rw-rw-rw-   0        0        0     2868 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/io/idx_io.py
+-rw-rw-rw-   0        0        0     6065 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/io/iqqm_out_reader.py
+-rw-rw-rw-   0        0        0     1705 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/io/lqn_io.py
+-rw-rw-rw-   0        0        0     3059 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/io/res_csv_io.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.951034 odhpy-0.2.0/src/odhpy/maps/
+-rw-rw-rw-   0        0        0       29 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/maps/__init__.py
+-rw-rw-rw-   0        0        0     5090 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/maps/station_maps.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.963617 odhpy-0.2.0/src/odhpy/plots/
+-rw-rw-rw-   0        0        0      121 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/plots/__init__.py
+-rw-rw-rw-   0        0        0    31099 2024-05-02 00:09:23.000000 odhpy-0.2.0/src/odhpy/plots/altair_plots.py
+-rw-rw-rw-   0        0        0      274 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/plots/node_diagrams.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/plots/plot_functions.py
+-rw-rw-rw-   0        0        0        0 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/plots/plotly_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.975605 odhpy-0.2.0/src/odhpy/stats/
+-rw-rw-rw-   0        0        0      111 2024-03-18 23:58:54.000000 odhpy-0.2.0/src/odhpy/stats/__init__.py
+-rw-rw-rw-   0        0        0     2498 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/stats/aggregate_stats.py
+-rw-rw-rw-   0        0        0    12092 2024-04-03 03:37:24.000000 odhpy-0.2.0/src/odhpy/stats/reliability_stats_class.py
+-rw-rw-rw-   0        0        0     9163 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/stats/storage_level_assessment.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.979770 odhpy-0.2.0/src/odhpy/stats/swflo2s/
+-rw-rw-rw-   0        0        0       22 2024-04-03 03:37:24.000000 odhpy-0.2.0/src/odhpy/stats/swflo2s/__init__.py
+-rw-rw-rw-   0        0        0     6755 2024-04-03 03:37:24.000000 odhpy-0.2.0/src/odhpy/stats/swflo2s/swflo2s.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.987831 odhpy-0.2.0/src/odhpy/stoch/
+-rw-rw-rw-   0        0        0       23 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/stoch/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/stoch/analyse.py
+-rw-rw-rw-   0        0        0     2867 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/stoch/generate.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.991895 odhpy-0.2.0/src/odhpy/trans/
+-rw-rw-rw-   0        0        0       27 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/trans/__init__.py
+-rw-rw-rw-   0        0        0     2953 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/trans/transformers.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.999782 odhpy-0.2.0/src/odhpy/utils/
+-rw-rw-rw-   0        0        0       99 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    11382 2024-04-03 03:37:24.000000 odhpy-0.2.0/src/odhpy/utils/dataframe_functions.py
+-rw-rw-rw-   0        0        0    10157 2024-03-19 03:03:09.000000 odhpy-0.2.0/src/odhpy/utils/datetime_functions.py
+-rw-rw-rw-   0        0        0      753 2024-03-14 03:25:24.000000 odhpy-0.2.0/src/odhpy/utils/interpolation.py
+-rw-rw-rw-   0        0        0      210 2024-05-02 00:10:39.000000 odhpy-0.2.0/src/odhpy/version.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:18:34.927333 odhpy-0.2.0/src/odhpy.egg-info/
+-rw-rw-rw-   0        0        0     2793 2024-05-02 00:18:34.000000 odhpy-0.2.0/src/odhpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2024-05-02 00:18:34.000000 odhpy-0.2.0/src/odhpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 00:18:34.000000 odhpy-0.2.0/src/odhpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-02 00:18:34.000000 odhpy-0.2.0/src/odhpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 00:18:34.000000 odhpy-0.2.0/src/odhpy.egg-info/top_level.txt
```

### Comparing `odhpy-0.1.0/PKG-INFO` & `odhpy-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odhpy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A collection of splashings to master that which has no form and count that which is uncountable.
 Home-page: https://bitbucket.org/odhydrology/odhpy.git
 Author: Chas Egan
 Author-email: chas@odhydrology.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `odhpy-0.1.0/README.md` & `odhpy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/setup.py` & `odhpy-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/clim/clim.py` & `odhpy-0.2.0/src/odhpy/clim/clim.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/io/csv_io.py` & `odhpy-0.2.0/src/odhpy/io/csv_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/io/idx_io.py` & `odhpy-0.2.0/src/odhpy/io/idx_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/io/iqqm_out_reader.py` & `odhpy-0.2.0/src/odhpy/io/iqqm_out_reader.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/io/lqn_io.py` & `odhpy-0.2.0/src/odhpy/io/lqn_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/io/res_csv_io.py` & `odhpy-0.2.0/src/odhpy/io/res_csv_io.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/maps/station_maps.py` & `odhpy-0.2.0/src/odhpy/maps/station_maps.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/plots/altair_plots.py` & `odhpy-0.2.0/src/odhpy/plots/altair_plots.py`

 * *Files 16% similar despite different names*

```diff
@@ -516,8 +516,205 @@
           axis=alt.Axis(title='Date')),
         alt.Y(yLabel + ':Q',
           axis=alt.Axis(title=yLabel)),
         color=legendTitle,
         tooltip=[alt.Tooltip(legendTitle),alt.Tooltip('Date',title='Date'),alt.Tooltip(yLabel,format=',.0f')]
     ).properties(width=plotWidth,height=plotHeight).interactive(bind_y=False)
     
-    return residMassPlot
+    return residMassPlot
+
+def storage_plot(df:pd.DataFrame, triggers=None, data_labels=None, colours=None, ylabel="Volume (ML)", xlabel="Date", legend="Key", caption=None, lineWidth=2, plotWidth=800, plotHeight=300, plot2Height=None, show_tooltip=True):
+    """Daily storage plot of timeseries data.
+
+    Args:
+        df (pd.DataFrame): pd.Dataframe of daily timeseries to plot.
+        triggers (dict, optional): Optional horizontal lines to mark on chart e.g. DSV, FSV. Dictionary where {key: value} = {'Trigger name':  Y value}. Defaults to None.
+        data_label (str, optional): Optional string to assign to supplied timeseries. Defaults to df column names.
+        colours (list, optional): Optional list of colours to apply to data. Defaults to Altair default.
+        ylabel (str, optional): Optional label for y axis. Defaults to "Volume (ML)".
+        xlabel (str, optional): Optional label for x axis. Defaults to "Date".
+        legend (str, optional): Optional label for legend. Defaults to "Key".
+        caption (str, optional): Optional caption for figure. Defaults to None.
+        lineWidth (float, optional): Optional width of figure lines. Defaults to 2.
+        plotWidth (float, optional): Optional overall width of figure. Defaults to 800.
+        plotHeight (float, optional): Optional overall height of main figure. Defaults to 300.
+        plot2Height (float, optional): Optional height of secondary figure. Defaults to 10% of main figure height.
+        show_tooltip (bool, optional): Optionally show tooltip. Defaults to True.
+
+    Returns:
+        altair.Chart: Returns an Altair chart object
+    """
+    #In case of pd.Series
+    df=pd.DataFrame(df)
+
+    #Get column names of input
+    cols_df=df.columns.values
+
+    #Set figure labels to column names (or data_labels input)
+    if data_labels is None:
+        labels=cols_df
+    else:
+        if data_labels.__len__() != cols_df.__len__():
+            print("Warning: Length of data_labels should equal number of columns in input df. Reverting labels to df column names.")
+            labels=cols_df            
+        else:
+            labels=data_labels
+    df.columns=labels
+
+    if plot2Height is None:
+        plot2Height=plotHeight/10
+
+    if triggers is None:
+        trigger_flag=False
+    else:
+        trigger_flag=True   
+
+    if caption is None:
+        caption=''
+
+    if show_tooltip:
+        tooltip = ['Date:T',alt.Tooltip('column:N',title=legend),alt.Tooltip('value:Q',title=ylabel, format=',.1f')]
+    else:
+        tooltip = []
+
+    #Default altair colours
+    if colours is None:
+        colours = ["#4c78a8", "#f58518", "#e45756", "#72b7b2", "#54a24b", "#eeca3b", "#b279a2", "#ff9da6", "#9d755d", "#bab0ac"]
+
+    interval = alt.selection_interval(encodings=['x'])   
+
+    #Base settings for main figure
+    base = alt.Chart(df.reset_index()).mark_line(
+        strokeWidth=lineWidth
+    ).transform_fold(
+        labels,
+        as_=['column','value']
+    ).transform_calculate(
+        value='round(datum.value * 10)/10'
+    ).encode(
+            x=alt.X('Date:T'),
+            y=alt.Y('value:Q',axis=alt.Axis(title=ylabel)),
+            color=alt.Color('column:N',sort=None, title=legend, scale=alt.Scale(range=colours))
+    )
+
+    #Main figure
+    chart = base.encode(
+        x=alt.X('Date:T', scale=alt.Scale(domain=interval), title=""),
+        tooltip=tooltip
+    ).properties(
+        width=plotWidth,
+        height=plotHeight,
+        title=caption
+    )
+
+    #Selection figure
+    view = alt.Chart(df.reset_index()).mark_line(
+        strokeWidth=1.5
+    ).transform_fold(
+        labels,
+        as_=['column','value']
+    ).transform_calculate(
+        value='round(datum.value * 10)/10'
+        #value='datum.value'
+    ).encode(
+        x=alt.X('Date:T', title=xlabel),
+        y=alt.Y('value:Q', axis=alt.Axis(title="")),
+        color=alt.Color('column:N',sort=None, title="", scale=alt.Scale(range=colours))
+    ).add_params(
+        interval
+    ).properties(
+        width=plotWidth,
+        height=plot2Height
+    )
+
+    #If triggers provided, rules figure
+    if trigger_flag:
+        df_trig=pd.DataFrame.from_dict({"value": triggers}).reset_index()
+        
+        rule=alt.Chart(df_trig).mark_rule(
+            strokeWidth=lineWidth,
+            opacity=0.9
+        ).encode(
+            y='value:Q',
+            color=alt.Color('index:O', sort=None),
+            strokeDash=alt.value([5,5])
+        )
+
+        combined=chart+rule
+
+    else:
+        combined=chart
+
+    return (combined.interactive(bind_x=False) & view)
+
+def annual_demand_supply_plot(demand: pd.DataFrame, supply: pd.DataFrame, wy_month=7, colours=None, plotWidth=1400, plotHeight=500, show_tooltip=True, label_freq=5, caption=None, legend="Key", xlabel="WY", ylabel="ML/a", sup_opacity = 1):
+    """Annual plot of demand and supply from daily timeseries input.
+
+    Args:
+        demand (pd.DataFrame): pd.Dataframe of daily demand timeseries to plot.
+        supply (pd.DataFrame): pd.Dataframe of daily supply timeseries to plot.
+        wy_month (int, optional): Water year start month. Defaults to 7.
+        colours (list, optional): Optional list of colours to apply to data. Defaults to selection from "muted rainbow" colour scheme.
+        plotWidth (float, optional): Optional overall width of figure. Defaults to 1400.
+        plotHeight (float, optional): Optional overall height of figure. Defaults to 500.
+        show_tooltip (bool, optional): Optionally show tooltip. Defaults to True.
+        label_freq (int, optional): Optional frequency to display year label. Defaults to 5 (years).
+        caption (str, optional): Optional figure caption. Defaults to None.
+        legend (str, optional): Optional legend label. Defaults to "Key".
+        xlabel (str, optional): Optional x axis label. Defaults to "WY".
+        ylabel (str, optional): Optional y axis label. Defaults to "ML/a".
+        sup_opacity (float, optional): Optional opacity of supply series. Defaults to 1.
+
+    Returns:
+        altair.Chart: Returns an Altair chart object
+    """        
+
+    if colours is None:
+        colours = ["#72AC57", "#639188", "#5C77B0", "#765EA4", "#98467A", "#BA3438", "#CF512B", "#E18433"]
+
+    if caption is None:
+        caption=''
+
+    if show_tooltip:
+        tooltip=[alt.Tooltip('index:O', title=xlabel), alt.Tooltip('column:O',title=legend), alt.Tooltip('value:Q',format=',.1f', title='Value (ML/a)')]
+    else:
+        tooltip=[]
+
+    demand=pd.DataFrame(demand)
+    supply=pd.DataFrame(supply)
+
+    dem_cols = demand.columns.values
+    sup_cols = supply.columns.values
+
+    df=pd.concat([demand,supply],axis=1)
+    df_annual=df.groupby(utils.get_wy(df.index, wy_month)).sum()
+
+    cht_dem=alt.Chart(df_annual.reset_index()).mark_bar(width=alt.RelativeBandSize(1)
+    ).transform_fold(
+        dem_cols,
+        as_=['column', 'value']
+    ).encode(
+        x=alt.X('index:O', title=xlabel, axis=alt.Axis(labelExpr="datum.value % " + str(label_freq) + " ? null : datum.label")),
+        y=alt.Y('value:Q', stack='zero', title=ylabel),
+        color=alt.Color('column:O', title=legend, scale=alt.Scale(range=colours), sort=None),
+        tooltip=tooltip
+    ).properties(
+        width=plotWidth,
+        height=plotHeight,
+        title=caption
+    )
+
+    cht_sup=alt.Chart(df_annual.reset_index()).mark_bar(width=alt.RelativeBandSize(1), opacity=sup_opacity
+    ).transform_fold(
+        sup_cols,
+        as_=['column', 'value']
+    ).encode(
+        x=alt.X('index:O', title=xlabel),
+        y=alt.Y('value:Q', stack='zero'),
+        color=alt.Color('column:O', title=legend, scale=alt.Scale(range=colours), sort=None),
+        tooltip=tooltip
+    ).properties(
+        width=plotWidth,
+        height=plotHeight,
+    )
+
+    return (cht_dem+cht_sup)
```

### Comparing `odhpy-0.1.0/src/odhpy/plots/plot_functions.py` & `odhpy-0.2.0/src/odhpy/plots/plot_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/stats/aggregate_stats.py` & `odhpy-0.2.0/src/odhpy/stats/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/stats/reliability_stats_class.py` & `odhpy-0.2.0/src/odhpy/stats/reliability_stats_class.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/stats/storage_level_assessment.py` & `odhpy-0.2.0/src/odhpy/stats/storage_level_assessment.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/stats/swflo2s/swflo2s.py` & `odhpy-0.2.0/src/odhpy/stats/swflo2s/swflo2s.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/stoch/generate.py` & `odhpy-0.2.0/src/odhpy/stoch/generate.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/trans/transformers.py` & `odhpy-0.2.0/src/odhpy/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/utils/dataframe_functions.py` & `odhpy-0.2.0/src/odhpy/utils/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/utils/datetime_functions.py` & `odhpy-0.2.0/src/odhpy/utils/datetime_functions.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy/utils/interpolation.py` & `odhpy-0.2.0/src/odhpy/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `odhpy-0.1.0/src/odhpy.egg-info/PKG-INFO` & `odhpy-0.2.0/src/odhpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odhpy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A collection of splashings to master that which has no form and count that which is uncountable.
 Home-page: https://bitbucket.org/odhydrology/odhpy.git
 Author: Chas Egan
 Author-email: chas@odhydrology.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `odhpy-0.1.0/src/odhpy.egg-info/SOURCES.txt` & `odhpy-0.2.0/src/odhpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

