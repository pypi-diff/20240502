# Comparing `tmp/regression_graph-0.1.tar.gz` & `tmp/regression_graph-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regression_graph-0.1.tar", last modified: Tue Mar  5 16:46:07 2024, max compression
+gzip compressed data, was "regression_graph-2.tar", last modified: Thu May  2 14:26:50 2024, max compression
```

## Comparing `regression_graph-0.1.tar` & `regression_graph-2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 16:46:07.067840 regression_graph-0.1/
--rw-rw-rw-   0        0        0     1092 2024-03-04 18:41:50.000000 regression_graph-0.1/LICENSE
--rw-rw-rw-   0        0        0     3309 2024-03-05 16:46:07.067840 regression_graph-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-05 16:46:07.050338 regression_graph-0.1/regression_graph/
--rw-rw-rw-   0        0        0      229 2024-03-05 15:29:42.000000 regression_graph-0.1/regression_graph/__init__.py
--rw-rw-rw-   0        0        0     6855 2024-03-05 15:48:59.000000 regression_graph-0.1/regression_graph/regression_graph.py
-drwxrwxrwx   0        0        0        0 2024-03-05 16:46:07.066808 regression_graph-0.1/regression_graph.egg-info/
--rw-rw-rw-   0        0        0     3309 2024-03-05 16:46:06.000000 regression_graph-0.1/regression_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-03-05 16:46:06.000000 regression_graph-0.1/regression_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 16:46:06.000000 regression_graph-0.1/regression_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-03-05 16:46:06.000000 regression_graph-0.1/regression_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-05 16:46:06.000000 regression_graph-0.1/regression_graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-05 16:46:07.067840 regression_graph-0.1/setup.cfg
--rw-rw-rw-   0        0        0      695 2024-03-05 16:45:14.000000 regression_graph-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 14:26:50.422362 regression_graph-2/
+-rw-rw-rw-   0        0        0     1092 2024-05-02 11:05:37.000000 regression_graph-2/LICENSE
+-rw-rw-rw-   0        0        0     4592 2024-05-02 14:26:50.422362 regression_graph-2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 14:26:50.397904 regression_graph-2/regression_graph/
+-rw-rw-rw-   0        0        0      299 2024-05-02 11:08:55.000000 regression_graph-2/regression_graph/__init__.py
+-rw-rw-rw-   0        0        0    16299 2024-05-02 14:23:40.000000 regression_graph-2/regression_graph/regression_graph.py
+drwxrwxrwx   0        0        0        0 2024-05-02 14:26:50.422362 regression_graph-2/regression_graph.egg-info/
+-rw-rw-rw-   0        0        0     4592 2024-05-02 14:26:50.000000 regression_graph-2/regression_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-02 14:26:50.000000 regression_graph-2/regression_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 14:26:50.000000 regression_graph-2/regression_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-02 14:26:50.000000 regression_graph-2/regression_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-02 14:26:50.000000 regression_graph-2/regression_graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 14:26:50.422362 regression_graph-2/setup.cfg
+-rw-rw-rw-   0        0        0      787 2024-05-02 14:26:35.000000 regression_graph-2/setup.py
```

### Comparing `regression_graph-0.1/LICENSE` & `regression_graph-2/LICENSE`

 * *Files identical despite different names*

### Comparing `regression_graph-0.1/PKG-INFO` & `regression_graph-2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: regression_graph
-Version: 0.1
-Summary: Python library to create regression graphs
+Version: 2
+Summary: Python library for regression graphs using coefficents, confidence intervals and p-values
 Author: Saema Khanom
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **README.md:**
 ```markdown
 # Regression Graph
 
@@ -17,23 +18,25 @@
 
 This Python library was designed to create regression graphs for datasets. Instead of using p-values, this library will use the coefficients and confidence interval to plot bars for each variable in the given dataset. The bars will be plotted with their upper and lower confidence interval and will use the p-value for the saturation of the bars. There's optional arguments to standardize the dataset. A table can be created to display the variable, mean and standard deviation of the dataset. 
 
 ## Features 
 
 plot_graph: plot the regression graph with manual data or with statsmodel regression
 
+coefficient_distribution_plots: plot any scipy distrabutions
+
 create_table: create a table for the variables, mean and standard deviation
 
 extract_data: use the statsmodel library to pass a fitted regression model which will extact the coefficents, confidence interval and p-value from the model and pass it onto plot_graph to produce the graph. 
 
 regression_plot, call this function and either inpur manaul dataset or statsmodels regression model to produce the graph. This function will either call extract_model if a regression is passed or plot_graph if manual data is passed. Call create_table to produce a table with the variable name, mean and standard devisation of the values. 
 
 ## Installation
 
-Install the package using pip install regression graph
+Install the package using pip install regression_graph
 
 ## Example usage 
 
 ```python
 from regression_graph import regression_plot
 ```
 
@@ -57,14 +60,60 @@
 3. Optional table
 create_table(ax2=position, dataframe, loc=none, font_size=none, col_widths=none,
              label_cell_loc=none, label_bbox=mandatory)
 
 Both options allow the values to be standardize by doing standardize=True in the regression_plot argument. 
 If standardize=True then user is required to give an input_X value (this is the indepdenat variable, can be a column from the dataset) for the function to work. 
 
+# Coefficent distrabution
+1. Read file path file
+2. Remove rows with missing values
+3. select the dependent variable (y) and independent variables (X)
+4. Fit the regression model
+5. Give variable names for the y-axis eg x
+6. Give manual values for coefficents, p-values, std_errs or pass a model to get the values. 
+7. Use scipy to pass a distrabution 
+8. Call regression_plot
+(ax1, coefficients=coefficients, distribution=distribution, p_values=p_values)
+9. Optional Paramter for Table
+10. Show graph
+
+# Create Table
+1. Call create_table
+2. Provide a paramter for data (independant variable)
+3. Optional paramter to change table size and text.
+
+# Customisable options 
+Plot_graph
+1. xlabel
+2. title
+3. show_yticks
+4. custom_levels
+5. positive_colour, negstive_colour
+
+coefficient_distribution_plots
+1. same as plot_graph with these additional optiond
+2. distribution
+3. num_std
+4. lower_percentile, upper_percentile
+
+create_table 
+1. data
+2. dependent_variable
+3. loc
+4. cell_loc
+5. font_size
+6. bbox
+7. col_widths
+8. label_cell_loc
+9. labels_bbox
+
+regression_plot
+table_kwargs
+
 ## Requirements
 Python 3.6 and above
 Numpy
 Matplotlib
 Pandas
 Statsmodels (optional)
```

### Comparing `regression_graph-0.1/regression_graph.egg-info/PKG-INFO` & `regression_graph-2/regression_graph.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: regression-graph
-Version: 0.1
-Summary: Python library to create regression graphs
+Version: 2
+Summary: Python library for regression graphs using coefficents, confidence intervals and p-values
 Author: Saema Khanom
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **README.md:**
 ```markdown
 # Regression Graph
 
@@ -17,23 +18,25 @@
 
 This Python library was designed to create regression graphs for datasets. Instead of using p-values, this library will use the coefficients and confidence interval to plot bars for each variable in the given dataset. The bars will be plotted with their upper and lower confidence interval and will use the p-value for the saturation of the bars. There's optional arguments to standardize the dataset. A table can be created to display the variable, mean and standard deviation of the dataset. 
 
 ## Features 
 
 plot_graph: plot the regression graph with manual data or with statsmodel regression
 
+coefficient_distribution_plots: plot any scipy distrabutions
+
 create_table: create a table for the variables, mean and standard deviation
 
 extract_data: use the statsmodel library to pass a fitted regression model which will extact the coefficents, confidence interval and p-value from the model and pass it onto plot_graph to produce the graph. 
 
 regression_plot, call this function and either inpur manaul dataset or statsmodels regression model to produce the graph. This function will either call extract_model if a regression is passed or plot_graph if manual data is passed. Call create_table to produce a table with the variable name, mean and standard devisation of the values. 
 
 ## Installation
 
-Install the package using pip install regression graph
+Install the package using pip install regression_graph
 
 ## Example usage 
 
 ```python
 from regression_graph import regression_plot
 ```
 
@@ -57,14 +60,60 @@
 3. Optional table
 create_table(ax2=position, dataframe, loc=none, font_size=none, col_widths=none,
              label_cell_loc=none, label_bbox=mandatory)
 
 Both options allow the values to be standardize by doing standardize=True in the regression_plot argument. 
 If standardize=True then user is required to give an input_X value (this is the indepdenat variable, can be a column from the dataset) for the function to work. 
 
+# Coefficent distrabution
+1. Read file path file
+2. Remove rows with missing values
+3. select the dependent variable (y) and independent variables (X)
+4. Fit the regression model
+5. Give variable names for the y-axis eg x
+6. Give manual values for coefficents, p-values, std_errs or pass a model to get the values. 
+7. Use scipy to pass a distrabution 
+8. Call regression_plot
+(ax1, coefficients=coefficients, distribution=distribution, p_values=p_values)
+9. Optional Paramter for Table
+10. Show graph
+
+# Create Table
+1. Call create_table
+2. Provide a paramter for data (independant variable)
+3. Optional paramter to change table size and text.
+
+# Customisable options 
+Plot_graph
+1. xlabel
+2. title
+3. show_yticks
+4. custom_levels
+5. positive_colour, negstive_colour
+
+coefficient_distribution_plots
+1. same as plot_graph with these additional optiond
+2. distribution
+3. num_std
+4. lower_percentile, upper_percentile
+
+create_table 
+1. data
+2. dependent_variable
+3. loc
+4. cell_loc
+5. font_size
+6. bbox
+7. col_widths
+8. label_cell_loc
+9. labels_bbox
+
+regression_plot
+table_kwargs
+
 ## Requirements
 Python 3.6 and above
 Numpy
 Matplotlib
 Pandas
 Statsmodels (optional)
```

### Comparing `regression_graph-0.1/setup.py` & `regression_graph-2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import find_namespace_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='regression_graph',
-    version='0.1',
-    description="Python library to create regression graphs",
+    version='2',
+    description="Python library for regression graphs using coefficents, confidence intervals and p-values",
     packages=find_namespace_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown", 
     author="Saema Khanom",
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
     ],
     install_requires=[
         'numpy',
         'matplotlib',
         'statsmodels',
         'pandas',
     ],
```

