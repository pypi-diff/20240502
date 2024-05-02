# Comparing `tmp/aprofs-0.0.1.tar.gz` & `tmp/aprofs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprofs-0.0.1.tar", max compression
+gzip compressed data, was "aprofs-0.0.2.tar", max compression
```

## Comparing `aprofs-0.0.1.tar` & `aprofs-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1215 2024-04-25 14:17:12.562406 aprofs-0.0.1/README.md
--rw-r--r--   0        0        0     2521 2024-04-25 14:18:25.856539 aprofs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-09 20:55:21.340320 aprofs-0.0.1/src/aprofs/__init__.py
--rw-r--r--   0        0        0    11058 2024-04-25 10:10:35.776954 aprofs-0.0.1/src/aprofs/code.py
--rw-r--r--   0        0        0     4931 2024-04-02 20:02:08.522909 aprofs-0.0.1/src/aprofs/example.json
--rw-r--r--   0        0        0    23242 2024-04-25 10:08:45.329819 aprofs-0.0.1/src/aprofs/utils.py
--rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 aprofs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1215 2024-04-25 14:17:12.562406 aprofs-0.0.2/README.md
+-rw-r--r--   0        0        0     2521 2024-05-02 14:50:35.530323 aprofs-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-09 20:55:21.340320 aprofs-0.0.2/src/aprofs/__init__.py
+-rw-r--r--   0        0        0    13076 2024-05-02 16:10:00.407480 aprofs-0.0.2/src/aprofs/code.py
+-rw-r--r--   0        0        0    27676 2024-05-02 16:11:30.750548 aprofs-0.0.2/src/aprofs/utils.py
+-rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 aprofs-0.0.2/PKG-INFO
```

### Comparing `aprofs-0.0.1/README.md` & `aprofs-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aprofs-0.0.1/pyproject.toml` & `aprofs-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 #[tool.setuptools.dynamic]
 #version = { file = "version.txt" }
 
 
 [tool.poetry]
 name = "aprofs"
-version = "0.0.1"
+version = "0.0.2"
 description = "\"Package aprofs serves the purpose of streaming the feature selection using aproximate preditions\""
 authors = ["Filipe Santos"]
 license = "MIT"
 readme = "README.md"
 keywords = ["one", "two"]
 classifiers = ["Programming Language :: Python :: 3"]
 #package-mode = false
```

### Comparing `aprofs-0.0.1/src/aprofs/code.py` & `aprofs-0.0.2/src/aprofs/code.py`

 * *Files 8% similar despite different names*

```diff
@@ -269,7 +269,57 @@
         utils.plot_data_compare(
             temp_data,
             feature,
             nbins=nbins,
             type_bins=type_bins,
             type_plot=type_plot,
         )
+
+    def visualize_neutralized_feature(  # pylint: disable=too-many-arguments
+        self,
+        main_feature: str,
+        neutralize_features: List[str] = None,
+        nbins: int = 20,
+        type_bins: str = "qcut",
+        type_plot: str = "prob",
+    ) -> None:
+        """
+        Visualize the marginal effect of a feature on the target variable after neutralizing the effect of other features.
+
+        Parameters:
+            main_feature (str): The main feature for which to visualize the marginal effect.
+            neutralize_features (List[str]): The list of other features to be neutralized.
+            nbins (int): The number of bins to use for the visualization. Default is 20.
+            type_bins (str): The type of binning to use. Default is "qcut".
+            type_plot (str): The type of plot to generate. Default is "prob".
+
+        Returns:
+            None
+
+        Raises:
+            ValueError: If an any feature is missing in the SHAP values dataframe.
+        """
+        # generate data to plot marginal effect shapley values
+        if neutralize_features is None:
+            neutralize_features = []
+        features = []
+        if not isinstance(neutralize_features, list):
+            neutralize_features = [neutralize_features]
+
+        features.append(main_feature)
+        features.extend(neutralize_features)
+        features = list(set(features))  # remove duplicates
+
+        missing_features = [feature for feature in features if feature not in self.shap_values.columns]
+        if missing_features:
+            raise ValueError(f"The following features are missing in the SHAP values: {missing_features}")
+
+        temp_data = utils.temp_neutral_plot_data(self, neutralize_features)
+        temp_data[main_feature] = self.current_data[main_feature]
+        # call plotting function
+        utils.plot_data_neutral(
+            temp_data,
+            main_feature,
+            nbins=nbins,
+            type_bins=type_bins,
+            type_plot=type_plot,
+        )
```

### Comparing `aprofs-0.0.1/src/aprofs/utils.py` & `aprofs-0.0.2/src/aprofs/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -631,7 +631,134 @@
     temp[f"{feature}_shap_prob_compare"] = 1 / (1 + np.exp(-temp[f"{feature}_shap_compare"]))
 
     # model probabilities data
     temp["shap_model"] = aprofs_obj.shap_mean + aprofs_obj.shap_values.sum(axis=1)
     temp["shap_prob_model"] = 1 / (1 + np.exp(-temp["shap_model"]))
 
     return temp
+
+
+def plot_data_neutral(  # pylint: disable=too-many-arguments
+    data: pd.DataFrame,
+    feature: str,
+    nbins: int = 20,
+    type_bins: str = "qcut",
+    type_plot: str = "prob",
+) -> None:
+    """
+    Plot data based on the provided neutralized DataFrame and features.
+
+    Args:
+        data (pd.DataFrame): The DataFrame containing the neutralize shap data.
+        feature (str): The main feature to plot on the x-axis.
+        nbins (int, optional): The number of bins. Defaults to 20.
+        type_bins (str, optional): The type of binning. Defaults to "qcut".
+        type_plot (str, optional): The type of plot. Defaults to "prob".
+
+    Returns:
+        None
+
+    Examples:
+        >>> temp = pd.DataFrame(...)
+        >>> plot_data_neutral(temp, "main_feature", other_features=["feature_1", "feature_2"], nbins=10, type_bins="cut", type_plot="raw")
+    """
+
+    if data[feature].unique().shape[0] < 25:
+        data["bins"] = data[feature].astype(str)
+    elif type_bins == "cut":
+        data["bins"] = pd.cut(data[feature], bins=nbins)
+    elif type_bins == "qcut":
+        data["bins"] = pd.qcut(data[feature], q=nbins)
+    else:
+        print("Invalid type_bins value")
+
+    # Calculate the means for each bin
+    means = data.groupby("bins", observed=True)["target"].mean()
+
+    if type_plot == "raw":
+        means_shap_others = data.groupby("bins", observed=True)["shap_other"].mean()
+        means_shap_model = data.groupby("bins", observed=True)["shap_model"].mean()
+    else:
+        means_shap_others = data.groupby("bins", observed=True)["shap_prob_other"].mean()
+        means_shap_model = data.groupby("bins", observed=True)["shap_prob_model"].mean()
+
+    # Calculate the counts for each bin
+    counts = data["bins"].value_counts(normalize=True).sort_index()
+
+    # Create a figure
+    fig = go.Figure()
+
+    # Add bar plot for counts on the primary y-axis
+    fig.add_trace(go.Bar(x=counts.index.astype(str), y=counts, name="Data", yaxis="y", marker_color="lightgray"))
+
+    # Add line plots on the secondary y-axis
+    fig.add_trace(go.Scatter(x=means.index.astype(str), y=means, mode="lines", name="Observed", yaxis="y2"))
+
+    fig.add_trace(
+        go.Scatter(
+            x=means_shap_others.index.astype(str),
+            y=means_shap_others,
+            mode="lines",
+            name="Neutralized shaps",
+            yaxis="y2",
+        )
+    )
+    fig.add_trace(
+        go.Scatter(
+            x=means_shap_model.index.astype(str),
+            y=means_shap_model,
+            mode="lines",
+            name="Original Model shaps",
+            yaxis="y2",
+        )
+    )
+
+    # Update layout to include a secondary y-axis
+    fig.update_layout(
+        yaxis={"title": "Counts", "side": "left", "tickformat": ".0%"},
+        yaxis2={"title": "Avg.", "side": "right", "overlaying": "y"},
+    )
+
+    fig.show()
+
+
+def temp_neutral_plot_data(aprofs_obj, features: List[str]) -> pd.DataFrame:
+    """
+    Generate a temporary DataFrame for plotting purposes.
+
+    Args:
+        aprofs_obj (Aprofs Object): An instance of the Aprofs class.
+        features (List[str]): A list of feature names that will be neutralized. The shapley values for this will be just the average values. This way the break the segmentation of the feature, maintaining the global effect of all the others.
+
+    Returns:
+        pd.DataFrame: The temporary DataFrame.
+
+    Examples:
+        >>> aprofs_obj = Aprofs Object(...)
+        >>> features = ['feature_1', 'feature_2']
+        >>> temp = temp_neutral_plot_data(aprofs_obj, features)
+        >>> print(temp.head())
+    """
+    if not isinstance(features, list):
+        features = [features]
+
+    temp = pd.DataFrame(
+        {
+            "target": aprofs_obj.target_column,
+        }
+    )
+
+    for feat in features:
+        temp[feat] = aprofs_obj.current_data[feat].values  # adding features to data
+
+    temp["shap_other"] = (
+        aprofs_obj.shap_mean
+        + aprofs_obj.shap_values[[col for col in aprofs_obj.shap_values.columns if col not in features]].sum(axis=1)
+        + aprofs_obj.shap_values[features]
+        .sum(axis=1)
+        .mean()  # sums the columns of the features and calculate the average value
+    )
+    temp["shap_prob_other"] = 1 / (1 + np.exp(-temp["shap_other"]))
+    temp["shap_model"] = aprofs_obj.shap_mean + aprofs_obj.shap_values.sum(axis=1)
+    temp["shap_prob_model"] = 1 / (1 + np.exp(-temp["shap_model"]))
+
+    return temp
```

### Comparing `aprofs-0.0.1/PKG-INFO` & `aprofs-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprofs
-Version: 0.0.1
+Version: 0.0.2
 Summary: "Package aprofs serves the purpose of streaming the feature selection using aproximate preditions"
 License: MIT
 Keywords: one,two
 Author: Filipe Santos
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

