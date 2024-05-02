# Comparing `tmp/featuring-data-0.2.2.tar.gz` & `tmp/featuring_data-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featuring-data-0.2.2.tar", last modified: Fri Apr 12 14:38:08 2024, max compression
+gzip compressed data, was "featuring_data-0.2.4.tar", last modified: Thu May  2 02:24:10 2024, max compression
```

## Comparing `featuring-data-0.2.2.tar` & `featuring_data-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:38:08.449623 featuring-data-0.2.2/
--rw-r--r--   0 dancapellupo   (501) staff       (20)     1079 2024-02-15 19:01:48.000000 featuring-data-0.2.2/LICENSE
--rw-r--r--   0 dancapellupo   (501) staff       (20)      832 2024-04-12 14:38:08.449434 featuring-data-0.2.2/PKG-INFO
--rw-r--r--   0 dancapellupo   (501) staff       (20)      172 2024-02-15 18:59:58.000000 featuring-data-0.2.2/README.md
--rw-r--r--   0 dancapellupo   (501) staff       (20)      719 2024-04-12 14:37:51.000000 featuring-data-0.2.2/pyproject.toml
--rw-r--r--   0 dancapellupo   (501) staff       (20)       38 2024-04-12 14:38:08.449663 featuring-data-0.2.2/setup.cfg
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:38:08.442997 featuring-data-0.2.2/src/
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:38:08.449237 featuring-data-0.2.2/src/featuring_data.egg-info/
--rw-r--r--   0 dancapellupo   (501) staff       (20)      832 2024-04-12 14:38:08.000000 featuring-data-0.2.2/src/featuring_data.egg-info/PKG-INFO
--rw-r--r--   0 dancapellupo   (501) staff       (20)      824 2024-04-12 14:38:08.000000 featuring-data-0.2.2/src/featuring_data.egg-info/SOURCES.txt
--rw-r--r--   0 dancapellupo   (501) staff       (20)        1 2024-04-12 14:38:08.000000 featuring-data-0.2.2/src/featuring_data.egg-info/dependency_links.txt
--rw-r--r--   0 dancapellupo   (501) staff       (20)       18 2024-04-12 14:38:08.000000 featuring-data-0.2.2/src/featuring_data.egg-info/requires.txt
--rw-r--r--   0 dancapellupo   (501) staff       (20)       14 2024-04-12 14:38:08.000000 featuring-data-0.2.2/src/featuring_data.egg-info/top_level.txt
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:38:08.444368 featuring-data-0.2.2/src/featuringdata/
--rw-r--r--   0 dancapellupo   (501) staff       (20)        0 2024-02-19 19:41:13.000000 featuring-data-0.2.2/src/featuringdata/__init__.py
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:38:08.445978 featuring-data-0.2.2/src/featuringdata/featureSelector/
--rw-r--r--   0 dancapellupo   (501) staff       (20)       79 2024-03-26 00:18:12.000000 featuring-data-0.2.2/src/featuringdata/featureSelector/__init__.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)      819 2024-03-15 01:12:03.000000 featuring-data-0.2.2/src/featuringdata/featureSelector/_create_pdf_report.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    24269 2024-03-25 22:49:10.000000 featuring-data-0.2.2/src/featuringdata/featureSelector/_features_select.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)     4018 2024-03-18 02:12:33.000000 featuring-data-0.2.2/src/featuringdata/featureSelector/_generate_plots.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    11861 2024-03-26 12:16:29.000000 featuring-data-0.2.2/src/featuringdata/featureSelector/_recursive_fit.py
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:38:08.448722 featuring-data-0.2.2/src/featuringdata/featuresEDA/
--rw-r--r--   0 dancapellupo   (501) staff       (20)       68 2024-02-19 23:39:34.000000 featuring-data-0.2.2/src/featuringdata/featuresEDA/__init__.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    13809 2024-04-11 22:48:40.000000 featuring-data-0.2.2/src/featuringdata/featuresEDA/_correlation.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    16529 2024-04-12 02:28:29.000000 featuring-data-0.2.2/src/featuringdata/featuresEDA/_create_pdf_report.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    21667 2024-04-12 02:32:28.000000 featuring-data-0.2.2/src/featuringdata/featuresEDA/_features_eda.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    10430 2024-04-12 02:14:19.000000 featuring-data-0.2.2/src/featuringdata/featuresEDA/_generate_plots.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)     5258 2024-03-28 02:40:38.000000 featuring-data-0.2.2/src/featuringdata/featuresEDA/_initial_eda_functions.py
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 02:24:10.290197 featuring_data-0.2.4/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     1079 2024-02-15 19:01:48.000000 featuring_data-0.2.4/LICENSE
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     8561 2024-05-02 02:24:10.289945 featuring_data-0.2.4/PKG-INFO
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     7775 2024-05-01 19:56:47.000000 featuring_data-0.2.4/README.md
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      794 2024-05-02 02:09:06.000000 featuring_data-0.2.4/pyproject.toml
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       38 2024-05-02 02:24:10.290275 featuring_data-0.2.4/setup.cfg
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 02:24:10.283110 featuring_data-0.2.4/src/
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 02:24:10.289706 featuring_data-0.2.4/src/featuring_data.egg-info/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     8561 2024-05-02 02:24:10.000000 featuring_data-0.2.4/src/featuring_data.egg-info/PKG-INFO
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      824 2024-05-02 02:24:10.000000 featuring_data-0.2.4/src/featuring_data.egg-info/SOURCES.txt
+-rw-r--r--   0 dancapellupo   (501) staff       (20)        1 2024-05-02 02:24:10.000000 featuring_data-0.2.4/src/featuring_data.egg-info/dependency_links.txt
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       69 2024-05-02 02:24:10.000000 featuring_data-0.2.4/src/featuring_data.egg-info/requires.txt
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       14 2024-05-02 02:24:10.000000 featuring_data-0.2.4/src/featuring_data.egg-info/top_level.txt
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 02:24:10.284450 featuring_data-0.2.4/src/featuringdata/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)        0 2024-02-19 19:41:13.000000 featuring_data-0.2.4/src/featuringdata/__init__.py
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 02:24:10.286314 featuring_data-0.2.4/src/featuringdata/featureSelector/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       79 2024-03-26 00:18:12.000000 featuring_data-0.2.4/src/featuringdata/featureSelector/__init__.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      819 2024-03-15 01:12:03.000000 featuring_data-0.2.4/src/featuringdata/featureSelector/_create_pdf_report.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    25391 2024-04-26 03:01:02.000000 featuring_data-0.2.4/src/featuringdata/featureSelector/_features_select.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     4018 2024-03-18 02:12:33.000000 featuring_data-0.2.4/src/featuringdata/featureSelector/_generate_plots.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    13670 2024-04-19 04:06:25.000000 featuring_data-0.2.4/src/featuringdata/featureSelector/_recursive_fit.py
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 02:24:10.289233 featuring_data-0.2.4/src/featuringdata/featuresEDA/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       68 2024-02-19 23:39:34.000000 featuring_data-0.2.4/src/featuringdata/featuresEDA/__init__.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    17018 2024-04-26 21:01:09.000000 featuring_data-0.2.4/src/featuringdata/featuresEDA/_correlation.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    21188 2024-04-26 21:05:20.000000 featuring_data-0.2.4/src/featuringdata/featuresEDA/_create_pdf_report.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    22295 2024-04-28 02:43:24.000000 featuring_data-0.2.4/src/featuringdata/featuresEDA/_features_eda.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    13544 2024-04-26 21:21:04.000000 featuring_data-0.2.4/src/featuringdata/featuresEDA/_generate_plots.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     6793 2024-04-22 02:30:06.000000 featuring_data-0.2.4/src/featuringdata/featuresEDA/_initial_eda_functions.py
```

### Comparing `featuring-data-0.2.2/LICENSE` & `featuring_data-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `featuring-data-0.2.2/src/featuring_data.egg-info/SOURCES.txt` & `featuring_data-0.2.4/src/featuring_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featuring-data-0.2.2/src/featuringdata/featureSelector/_create_pdf_report.py` & `featuring_data-0.2.4/src/featuringdata/featureSelector/_create_pdf_report.py`

 * *Files identical despite different names*

### Comparing `featuring-data-0.2.2/src/featuringdata/featureSelector/_features_select.py` & `featuring_data-0.2.4/src/featuringdata/featureSelector/_features_select.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from sklearn.model_selection import train_test_split, ParameterGrid
 from sklearn.metrics import mean_squared_error, mean_absolute_error
-
-from xgboost.sklearn import XGBRegressor
+from sklearn.preprocessing import LabelEncoder
+from xgboost.sklearn import XGBRegressor, XGBClassifier
 
 from ._create_pdf_report import (
     initialize_pdf_doc,
     add_text_pdf,
     add_plot_pdf,
     save_pdf_doc
 )
 
-from ._recursive_fit import recursive_fit
+from ._recursive_fit import recursive_fit, calc_model_metric
 
 from ._generate_plots import plot_inline_scatter, plot_xy, plot_horizontal_line, plot_vertical_line, save_fig, plot_xy_splitaxis
 
 
 class FeatureSelector:
     """
     This class implements an iterative machine learning model training
@@ -133,21 +133,22 @@
         - "num_iters": The number of iterations each feature appeared in,
             before being removed.
 
 
     """
 
     def __init__(self, numeric_cols, non_numeric_cols, report_prefix='FeatureSelection', target_col=None,
-                 target_log=False, test_size=0.15, parameter_dict=None):
+                 target_log=False, target_type='regression', test_size=0.15, parameter_dict=None):
 
         self.numeric_cols = numeric_cols
         self.non_numeric_cols = non_numeric_cols
         self.report_prefix = report_prefix
         self.target_col = target_col
         self.target_log = target_log
+        self.target_type = target_type
 
         self.test_size = test_size
 
         if parameter_dict is None:
             self.parameter_dict = {'max_depth': [3, 4, 5, 6], 'gamma': [0, 1, 5],
                                    'min_child_weight': [0, 1, 5], 'max_delta_step': [0, 1, 5]}
         else:
@@ -158,15 +159,15 @@
         self.X = None
         self.y = None
 
         self.hyperparams_df = pd.DataFrame()
         self.feature_importance_dict_list = list()
         self.feat_import_bycol_df = pd.DataFrame()
 
-    def run(self, data_df, numeric_df=None, non_numeric_df=None):
+    def run(self, data_df, master_columns_df=None, numeric_df=None, non_numeric_df=None):
         """
         Run an iterative model training on a given dataset:
 
         This function runs the following steps:
         - Data preparation tasks
         - Iterative / recursive model training
         - Generate plots and a PDF report
@@ -226,41 +227,43 @@
         # Perform onehot encoding on any categorical features:
         if len(self.non_numeric_cols) > 0:
             X_onehot = pd.get_dummies(data_df[self.non_numeric_cols], dtype=int)
 
             self.X = self.X.merge(X_onehot, left_index=True, right_index=True)
 
         # Take the log of the target variable, if user chooses:
-        if self.target_log:
+        if self.target_type == 'classification':
+            enc = LabelEncoder()
+            self.y = enc.fit_transform(data_df[self.target_col].values)
+        elif self.target_log:
             self.y = np.log1p(data_df[self.target_col].values)
         else:
             self.y = data_df[self.target_col].values
 
         # TODO: Update this code for more than 2 splits
         # Perform random data splits:
         X_train_42, X_test_42, y_train_42, y_test_42 = train_test_split(self.X, self.y, test_size=self.test_size,
                                                                         random_state=42)
         X_train_46, X_test_46, y_train_46, y_test_46 = train_test_split(self.X, self.y, test_size=self.test_size,
                                                                         random_state=46)
-
         # TODO Allow user to set max/min values of the hyperparam ranges, as well as number of total iterations,
         #  which would define how many values to consider per hyperparam
 
         X_train_comb = [X_train_42, X_train_46]
         X_test_comb = [X_test_42, X_test_46]
 
         y_train_comb = [y_train_42, y_train_46]
         y_test_comb = [y_test_42, y_test_46]
 
         # --------------------------------------------------------------------
         # Run Recursive Training
 
         training_results_df, self.hyperparams_df, self.feature_importance_dict_list = recursive_fit(
             X_train_comb, y_train_comb, X_test_comb, y_test_comb, target_log=self.target_log,
-            parameter_dict=self.parameter_dict)
+            target_type=self.target_type, parameter_dict=self.parameter_dict)
 
         # --------------------------------------------------------------------
         # Identify Best Results
 
         # TODO: Identify best run based on metric out to certain number [3?] of decimal points
         best_result_ind_1 = np.argmin(training_results_df["RMSE_test_1"].values)
         best_result_ind_2 = np.argmin(training_results_df["RMSE_test_2"].values)
@@ -289,23 +292,28 @@
 
         hyperparams_dict = self.hyperparams_df.loc[hyperparam_iter].to_dict()
         print('Using Iter {} from data split {} with {}'.format(best_ind, data_ind+1, hyperparams_dict))
 
         # --------------------------------------------------------------------
         # XGBoost Training with "Best" Feature Selection
 
-        xgb_reg = XGBRegressor(n_estimators=1000, early_stopping_rounds=20, random_state=42, **hyperparams_dict)
+        if self.target_type == 'regression':
+            xgb_reg = XGBRegressor(n_estimators=1000, early_stopping_rounds=20, random_state=42, **hyperparams_dict)
+        else:
+            xgb_reg = XGBClassifier(n_estimators=1000, early_stopping_rounds=20, random_state=42, **hyperparams_dict)
         xgb_reg.fit(X_train_best, y_train_comb[data_ind], eval_set=[(X_test_best, y_test_comb[data_ind])], verbose=True)
 
         y_test_pred = xgb_reg.predict(X_test_best)
-
+        
         if self.target_log:
-            mae_final = mean_absolute_error(np.expm1(y_test_comb[data_ind]), np.expm1(y_test_pred))
+            mae_final = calc_model_metric(np.expm1(y_test_comb[data_ind]), np.expm1(y_test_pred),
+                                          target_type=self.target_type, metric_type='easy')
         else:
-            mae_final = mean_absolute_error(y_test_comb[data_ind], y_test_pred)
+            mae_final = calc_model_metric(y_test_comb[data_ind], y_test_pred, target_type=self.target_type,
+                                          metric_type='easy')
         print('\nFinal MAE: {}\n'.format(mae_final))
 
         # --------------------
         # Save results to CSV:
         training_results_df.to_csv('{}_training_results_full_{}.csv'.format(self.report_prefix, timestamp))
         self.hyperparams_df.to_csv('{}_best_hyperparameters_{}.csv'.format(self.report_prefix, timestamp))
 
@@ -383,28 +391,30 @@
         # PLOT #2 - Generate plots showing how the feature importance of the
         #  top features changes depending on the number of total features used
 
         num_features = training_results_df["num_features_{}".format(data_ind+1)].values
         # Set the number of features to show on each plot:
         num_feat_per_plot = 5
         # Set the total number of features to plot:
-        tot_feat_to_plot = 20
+        tot_feat_to_plot = min(20, len(self.feat_import_bycol_df) - len(self.feat_import_bycol_df) % num_feat_per_plot)
         # Each loop corresponds to one plot:
         for jj in range(0, tot_feat_to_plot, num_feat_per_plot):
             cols_to_plot = self.feat_import_bycol_df.index[jj:jj+num_feat_per_plot]
 
             # Within each plot, loop over each feature to plot:
             for jjj, col in enumerate(cols_to_plot):
                 # Find all the feature importance values for this feature
                 #  (this will vary per feature depending on when that feature
                 #   was removed during the iterative training):
                 num_iters = int(self.feat_import_bycol_df.loc[col, "num_iters"])
                 x = num_features[start_ii:num_iters]
                 y = self.feature_importance_dict_list[data_ind][col][start_ii:]
 
+                print(jj, jjj, col)
+
                 # If this is the first feature for this plot panel:
                 if jjj == 0:
                     f, ax = plot_xy(x, y, xlabel='num_features_{}'.format(data_ind+1), ylabel='feature importance',
                                     leg_label=col, overplot=False, outfile=False)
                 elif jjj < num_feat_per_plot-1:
                     f, ax = plot_xy(x, y, f=f, ax=ax, leg_label=col, overplot=True, outfile=False)
                 # If this is the last feature for this plot panel, save the
@@ -422,30 +432,33 @@
         # --------------------------------------------------------------------
         # PLOT #3 - Generate plot of feature importance versus correlation
         #  with target variable
 
         cols_best_iter = self.feat_import_bycol_df.dropna().index
         # This plot can only be generated if a dataframe with feature
         #  correlations is passed to the function:
-        if numeric_df is not None:
+        if master_columns_df is not None:
             # Get a list of features that are both numeric and are part of the
             #  "best" training iteration:
-            numeric_best_feat = set(cols_best_iter).intersection(set(numeric_df.index))
-            print('Number of numeric features in best iteration: {}'.format(len(numeric_best_feat)))
+            numeric_df = master_columns_df.loc[master_columns_df["Column Type"] == 'numeric']
+            if len(numeric_df) > 0:
+                numeric_best_feat = set(cols_best_iter).intersection(set(numeric_df.index))
+                print('Number of numeric features in best iteration: {}'.format(len(numeric_best_feat)))
 
-            x, y = [], []
-            for feat in numeric_best_feat:
-                x.append(numeric_df.loc[feat, "Random Forest"])
-                y.append(self.feat_import_bycol_df.loc[feat, "best_feat_imp"])
-
-            f, ax = plot_xy(x, y, xlabel='RF Correlation between Feature and Target', ylabel='Feature Importance',
-                            leg_label='Numeric Feature', overplot=False, outfile=False, plots_folder=plots_folder,
-                            title='target_correlation_vs_feature_importance')
+                x, y = [], []
+                for feat in numeric_best_feat:
+                    x.append(numeric_df.loc[feat, "Random Forest"])
+                    y.append(self.feat_import_bycol_df.loc[feat, "best_feat_imp"])
+
+                f, ax = plot_xy(x, y, xlabel='RF Correlation between Feature and Target', ylabel='Feature Importance',
+                                leg_label='Numeric Feature', overplot=False, outfile=False, plots_folder=plots_folder,
+                                title='target_correlation_vs_feature_importance')
 
-            if non_numeric_df is not None:
+            non_numeric_df = master_columns_df.loc[master_columns_df["Column Type"] == 'non-numeric']
+            if len(non_numeric_df) > 0:
                 feat_import_bycol_df_best = self.feat_import_bycol_df.dropna()
                 # non_numeric_best_feat = set(cols_best_iter).difference()
 
                 x, y = [], []
                 for feat in non_numeric_df.index:
                     # For categorical features, the name may appear more than
                     #  once due to one-hot encoding:
```

### Comparing `featuring-data-0.2.2/src/featuringdata/featureSelector/_generate_plots.py` & `featuring_data-0.2.4/src/featuringdata/featureSelector/_generate_plots.py`

 * *Files identical despite different names*

### Comparing `featuring-data-0.2.2/src/featuringdata/featureSelector/_recursive_fit.py` & `featuring_data-0.2.4/src/featuringdata/featureSelector/_recursive_fit.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 
 from tqdm.auto import tqdm
 
 import numpy as np
 import pandas as pd
 
 from sklearn.model_selection import GridSearchCV, ParameterGrid
-from sklearn.metrics import mean_squared_error, mean_absolute_error
+from sklearn.metrics import (
+    mean_squared_error,
+    mean_absolute_error,
+    accuracy_score,
+    log_loss,
+    cohen_kappa_score,
+)
 
-from xgboost.sklearn import XGBRegressor
+from xgboost.sklearn import XGBRegressor, XGBClassifier
 
 
 def round_to_n_sigfig(x, n=3):
     """
     Round a number to 'n' significant digits.
 
     Parameters
@@ -49,16 +55,29 @@
     # If rounding creates a number with no digits beyond the decimal point,
     #  then make it an integer:
     if x_round > 10 ** (n - 1):
         x_round = int(x_round)
     return x_round
 
 
-def recursive_fit(X_train_comb, y_train_comb, X_test_comb, y_test_comb, parameter_dict, use_gridsearchcv=False,
-                  target_log=False):
+def calc_model_metric(y, y_pred, target_type='regression', metric_type='regular'):
+        if target_type == 'regression':
+            if metric_type == 'regular':
+                return mean_squared_error(y, y_pred, squared=False)
+            else:
+                return mean_absolute_error(y, y_pred)
+        else:
+            if metric_type == 'regular':
+                return log_loss(y, y_pred)
+            else:
+                return cohen_kappa_score(y, y_pred)
+
+
+def recursive_fit(X_train_comb, y_train_comb, X_test_comb, y_test_comb, parameter_dict, target_type='regression',
+                  use_gridsearchcv=False, target_log=False):
     """
     This is the core function that performs the iterative model training.
 
     Parameters
     ----------
     X_train_comb : list
         A list of X_train training sets.
@@ -160,15 +179,18 @@
             # Hyperparameter Search
             best_score = None
 
             for data_jj in range(2):
 
                 if use_gridsearchcv:
                     # Hyperparameter search using GridSearchCV:
-                    xgb_reg = XGBRegressor(n_estimators=1000, early_stopping_rounds=20, random_state=42)
+                    if target_type == 'regression':
+                        xgb_reg = XGBRegressor(n_estimators=1000, early_stopping_rounds=20, random_state=42)
+                    else:
+                        xgb_reg = XGBClassifier(n_estimators=1000, early_stopping_rounds=20, random_state=42)
 
                     grid_search = GridSearchCV(xgb_reg, param_grid=parameter_dict, cv=2)
 
                     grid_search.fit(X_train_comb[data_jj][feature_columns[data_jj]], y_train_comb[data_jj],
                                     eval_set=[(X_test_comb[data_jj][feature_columns[data_jj]], y_test_comb[data_jj])],
                                     verbose=False)
 
@@ -180,17 +202,21 @@
                         best_params_dict = grid_search.best_params_
                         best_score = grid_search.best_score_
 
                 else:
                     # Hyperparameter search using the train and validation sets already defined:
                     print('Running grid search at Iteration {} on data split {}...'.format(jj, data_jj+1))
                     for parameter_dict_tmp in iter(tqdm(ParameterGrid(parameter_dict))):
-
-                        xgb_reg = XGBRegressor(n_estimators=1000, early_stopping_rounds=20, random_state=42,
-                                               **parameter_dict_tmp)
+                        
+                        if target_type == 'regression':
+                            xgb_reg = XGBRegressor(n_estimators=1000, early_stopping_rounds=20, random_state=42,
+                                                   **parameter_dict_tmp)
+                        else:
+                            xgb_reg = XGBClassifier(n_estimators=1000, early_stopping_rounds=20, random_state=42,
+                                                    **parameter_dict_tmp)
                         xgb_reg.fit(X_train_comb[data_jj][feature_columns[data_jj]], y_train_comb[data_jj],
                                     eval_set=[(X_test_comb[data_jj][feature_columns[data_jj]], y_test_comb[data_jj])],
                                     verbose=False)
 
                         if (best_score is None) or (xgb_reg.best_score < best_score):
                             best_score = xgb_reg.best_score
                             best_params_dict = parameter_dict_tmp
@@ -206,34 +232,43 @@
 
         out_row = []
 
         # Loop over the two random data splits:
         for data_jj in range(2):
 
             # XGBoost Training:
-            xgb_reg = XGBRegressor(n_estimators=1000, early_stopping_rounds=20, random_state=42, **best_params_dict)
+            if target_type == 'regression':
+                xgb_reg = XGBRegressor(n_estimators=1000, early_stopping_rounds=20, random_state=42, **best_params_dict)
+            else:
+                xgb_reg = XGBClassifier(n_estimators=1000, early_stopping_rounds=20, random_state=42, **best_params_dict)
 
             xgb_reg.fit(X_train_comb[data_jj][feature_columns[data_jj]], y_train_comb[data_jj],
                         eval_set=[(X_test_comb[data_jj][feature_columns[data_jj]], y_test_comb[data_jj])], verbose=False)
 
-            y_train_pred = xgb_reg.predict(X_train_comb[data_jj][feature_columns[data_jj]])
-            y_test_pred = xgb_reg.predict(X_test_comb[data_jj][feature_columns[data_jj]])
+            if target_type == 'regression':
+                y_train_pred = xgb_reg.predict(X_train_comb[data_jj][feature_columns[data_jj]])
+                y_test_pred = xgb_reg.predict(X_test_comb[data_jj][feature_columns[data_jj]])
+            else:
+                y_train_pred = xgb_reg.predict_proba(X_train_comb[data_jj][feature_columns[data_jj]])
+                y_test_pred = xgb_reg.predict_proba(X_test_comb[data_jj][feature_columns[data_jj]])
 
             # TODO: Instead of rounding, go by significant digits [# of digits to be user-configurable]
-            train_err = round_to_n_sigfig(mean_squared_error(y_train_comb[data_jj], y_train_pred, squared=False), 5)
-            test_err = round_to_n_sigfig(mean_squared_error(y_test_comb[data_jj], y_test_pred, squared=False), 5)
+            train_err = round_to_n_sigfig(calc_model_metric(y_train_comb[data_jj], y_train_pred, target_type=target_type), 5)
+            test_err = round_to_n_sigfig(calc_model_metric(y_test_comb[data_jj], y_test_pred, target_type=target_type), 5)
 
             # If the log of the training data was taken, then reverse the log
             #  to save an easier-to-follow MAE value for the user:
             if target_log:
                 test_mae = round_to_n_sigfig(
-                    mean_absolute_error(np.expm1(y_test_comb[data_jj]), np.expm1(y_test_pred)), 5)
+                    calc_model_metric(np.expm1(y_test_comb[data_jj]), np.expm1(y_test_pred), target_type=target_type, metric_type='easy'), 5)
             else:
-                test_mae = round_to_n_sigfig(mean_absolute_error(y_test_comb[data_jj], y_test_pred), 5)
-
+                if target_type == 'classification':
+                    y_test_pred = xgb_reg.predict(X_test_comb[data_jj][feature_columns[data_jj]])
+                test_mae = round_to_n_sigfig(calc_model_metric(y_test_comb[data_jj], y_test_pred, target_type=target_type, metric_type='easy'), 5)
+            
             # ----------------------------------------------------------------
             # Save information from this iteration to dataframe
             out_row.extend(
                 [train_err, test_err, test_mae, len(feature_columns[data_jj]), ', '.join(feature_columns[data_jj])])
 
             max_feat_import_ind = np.argmax(xgb_reg.feature_importances_)
             out_row.extend([feature_columns[data_jj][max_feat_import_ind],
```

### Comparing `featuring-data-0.2.2/src/featuringdata/featuresEDA/_correlation.py` & `featuring_data-0.2.4/src/featuringdata/featuresEDA/_correlation.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 from tqdm.auto import tqdm
 
 import numpy as np
 import pandas as pd
 
 from scipy.stats import pearsonr
-from sklearn.feature_selection import mutual_info_regression
+from sklearn.preprocessing import LabelEncoder
+from sklearn.feature_selection import mutual_info_regression, mutual_info_classif
+from sklearn.metrics import cohen_kappa_score
 
-from sklearn.ensemble import RandomForestRegressor
+from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
 
 
 def get_random_forest_hyperparams(n_samples, rf_n_estimators='auto', numeric=True):
 
     # For 3000 samples or less, use 50 trees. Otherwise, stick to 10:
     if rf_n_estimators == 'auto':
         rf_n_estimators = 10 if n_samples >= 3000 else 50
@@ -29,15 +31,16 @@
 
     else:
         min_samples_leaf = np.ceil(0.0025 * n_samples).astype(int)
 
     return rf_n_estimators, min_samples_leaf
 
 
-def calc_numeric_features_target_corr(data_df, numeric_cols, target_col, rf_n_estimators='auto'):
+def calc_numeric_features_target_corr(data_df, numeric_cols, master_columns_df, target_col, target_type='regression',
+                                      rf_n_estimators='auto'):
     """
     Calculate the correlation between numeric features and the target
     variable.
 
     If the target variable is numeric (i.e., a regression problem), the
     Pearson correlation is calculated first.
 
@@ -80,87 +83,104 @@
     """
 
     rf_n_estimators, min_samples_leaf = get_random_forest_hyperparams(len(data_df), rf_n_estimators=rf_n_estimators)
 
     print('For random forest (RF) correlation measure, using {} trees and min_samples_leaf={}.\n'.format(
         rf_n_estimators, min_samples_leaf))
 
-    numeric_df = pd.DataFrame(columns=["Count not-Null", "Pearson", "Mutual Info", "Random Forest"])
+    if target_type == 'regression':
+        numeric_df = pd.DataFrame(columns=["Count not-Null", "Pearson", "Mutual Info", "Random Forest"])
+    else:
+        numeric_df = pd.DataFrame(columns=["Count not-Null", "Mutual Info", "Random Forest"])
 
     # Loop over each numeric feature:
     print('Running correlations of numeric features to target variable...')
     for col in tqdm(numeric_cols):
         # Keep only rows that do not have NULL for that feature:
         data_df_col_notnull = data_df[[col, target_col]].dropna()
 
-        # Calculate Pearson correlation between feature and target:
-        pcorr = pearsonr(data_df_col_notnull[col].values, data_df_col_notnull[target_col].values)[0]
-        # Calculate the Mutual Information for feature and target:
-        minfo = mutual_info_regression(
-            data_df_col_notnull[col].values.reshape(-1, 1), data_df_col_notnull[target_col].values)[0]
-
-        # Train a random forest model with just that feature and the target variable:
-        rf_reg = RandomForestRegressor(n_estimators=rf_n_estimators, min_samples_leaf=min_samples_leaf)
-        rf_reg.fit(data_df_col_notnull[col].values.reshape(-1, 1), data_df_col_notnull[target_col].values)
-        rfscore = rf_reg.score(data_df_col_notnull[col].values.reshape(-1, 1), data_df_col_notnull[target_col])
+        if target_type == 'regression':
+            # Calculate Pearson correlation between feature and target:
+            pcorr = pearsonr(data_df_col_notnull[col].values, data_df_col_notnull[target_col].values)[0]
+            # Calculate the Mutual Information for feature and target:
+            minfo = mutual_info_regression(
+                data_df_col_notnull[col].values.reshape(-1, 1), data_df_col_notnull[target_col].values)[0]
+
+            # Train a random forest model with just that feature and the target variable:
+            rf_reg = RandomForestRegressor(n_estimators=rf_n_estimators, min_samples_leaf=min_samples_leaf)
+            rf_reg.fit(data_df_col_notnull[col].values.reshape(-1, 1), data_df_col_notnull[target_col].values)
+            rfscore = rf_reg.score(data_df_col_notnull[col].values.reshape(-1, 1), data_df_col_notnull[target_col])
+
+            # Save the results as a new row in the dataframe for output:
+            numeric_df.loc[col] = len(data_df_col_notnull), round(pcorr, 2), round(minfo, 2), round(max(rfscore, 0), 2)
+
+        else:
+            # Calculate the Mutual Information for feature and target:
+            minfo = mutual_info_classif(
+                data_df_col_notnull[col].values.reshape(-1, 1), data_df_col_notnull[target_col].values)[0]
+
+            # Train a random forest model with just that feature and the target variable:
+            rf_class = RandomForestClassifier(n_estimators=rf_n_estimators, min_samples_leaf=min_samples_leaf)
+            rf_class.fit(data_df_col_notnull[col].values.reshape(-1, 1), data_df_col_notnull[target_col].values)
+            y_train_pred = rf_class.predict(data_df_col_notnull[col].values.reshape(-1, 1))
+            rf_ck = max(cohen_kappa_score(data_df_col_notnull[target_col].values, y_train_pred), 0)
+
+            # Save the results as a new row in the dataframe for output:
+            numeric_df.loc[col] = len(data_df_col_notnull), round(minfo, 2), round(rf_ck, 2)
 
-        # Save the results as a new row in the dataframe for output:
-        numeric_df.loc[col] = len(data_df_col_notnull), round(pcorr, 2), round(minfo, 2), round(rfscore, 2)
+    master_columns_df.loc[numeric_df.index, numeric_df.columns] = numeric_df
 
     # The counts of NULL values should be integers:
-    numeric_df["Count not-Null"] = numeric_df["Count not-Null"].astype(int)
+    # numeric_df["Count not-Null"] = numeric_df["Count not-Null"].astype(int)
 
     # Sort the dataframe by the Random Forest R^2 for each feature, in
     # descending order:
-    numeric_df = numeric_df.sort_values(by=["Random Forest"], ascending=False)
+    # numeric_df = numeric_df.sort_values(by=["Random Forest"], ascending=False)
 
-    return numeric_df
+    return master_columns_df
 
 
-def calc_corr_numeric_features(data_df, numeric_cols):
+def calc_corr_numeric_features(data_df, numeric_cols, master_columns_df):
     """
 
     :param data_df:
     :param numeric_cols:
     :return:
     """
 
     rf_n_estimators, min_samples_leaf = get_random_forest_hyperparams(len(data_df))
 
-    start = time.time()
     numeric_collinear_df = pd.DataFrame(columns=["Feature1", "Feature2", "Count not-Null", "Pearson", "Random Forest"])
 
     jj = 0
     total_iters = len(list(it.combinations(numeric_cols, 2)))
     for pair in tqdm(it.combinations(numeric_cols, 2), total=total_iters):
         col1, col2 = pair[0], pair[1]
 
         data_df_cols_notnull = data_df[[col1, col2]].dropna()
 
         pcorr = pearsonr(data_df_cols_notnull[col1].values, data_df_cols_notnull[col2].values)[0]
 
         rf_reg = RandomForestRegressor(n_estimators=10, min_samples_leaf=min_samples_leaf)
         rf_reg.fit(data_df_cols_notnull[col1].values.reshape(-1, 1), data_df_cols_notnull[col2].values)
-        rfscore1 = rf_reg.score(data_df_cols_notnull[col1].values.reshape(-1, 1), data_df_cols_notnull[col2])
+        rfscore1 = max(rf_reg.score(data_df_cols_notnull[col1].values.reshape(-1, 1), data_df_cols_notnull[col2]), 0)
 
         rf_reg = RandomForestRegressor(n_estimators=10, min_samples_leaf=min_samples_leaf)
         rf_reg.fit(data_df_cols_notnull[col2].values.reshape(-1, 1), data_df_cols_notnull[col1].values)
-        rfscore2 = rf_reg.score(data_df_cols_notnull[col2].values.reshape(-1, 1), data_df_cols_notnull[col1])
+        rfscore2 = max(rf_reg.score(data_df_cols_notnull[col2].values.reshape(-1, 1), data_df_cols_notnull[col1]), 0)
 
         numeric_collinear_df.loc[jj] = col1, col2, len(data_df_cols_notnull), round(pcorr, 2), round((rfscore1+rfscore2)/2, 2)
 
         jj += 1
 
     numeric_collinear_df = numeric_collinear_df.sort_values(by=["Random Forest"], ascending=False)
-    print(time.time() - start)
 
-    start = time.time()
     numeric_collinear_summary_df = pd.DataFrame(
-        columns=["Avg Pearson Corr", "Avg RF Corr", "Max Pear Corr Feature", "Max Pear", "Max RF Corr Feature",
-                 "Max RF Corr"])
+        columns=["COLLIN Avg Pearson Corr", "COLLIN Avg RF Corr", "COLLIN Max Pear Corr Feature", "COLLIN Max Pear",
+                 "COLLIN Max RF Corr Feature", "COLLIN Max RF Corr"])
 
     for col in numeric_cols:
         numeric_collinear_df_col = numeric_collinear_df.loc[
             (numeric_collinear_df["Feature1"] == col) | (numeric_collinear_df["Feature2"] == col)]
 
         pn_xx = np.argmax(np.abs(numeric_collinear_df_col["Pearson"].values))
         max_corr_feat1, max_corr_feat2 = numeric_collinear_df_col[["Feature1", "Feature2"]].iloc[pn_xx]
@@ -171,19 +191,21 @@
         max_rf_corr_feat = max_corr_feat1 if max_corr_feat1 != col else max_corr_feat2
 
         numeric_collinear_summary_df.loc[col] = (
             round(np.mean(np.abs(numeric_collinear_df_col["Pearson"].values)), 2),
             round(numeric_collinear_df_col["Random Forest"].mean(), 2), max_pn_corr_feat,
             numeric_collinear_df_col["Pearson"].iloc[pn_xx], max_rf_corr_feat,
             numeric_collinear_df_col["Random Forest"].iloc[rf_xx])
+    
+    master_columns_df.loc[
+        numeric_collinear_summary_df.index, numeric_collinear_summary_df.columns] = numeric_collinear_summary_df
 
-    numeric_collinear_summary_df = numeric_collinear_summary_df.sort_values(by=["Max RF Corr"], ascending=False)
-    print(time.time() - start)
+    # numeric_collinear_summary_df = numeric_collinear_summary_df.sort_values(by=["Max RF Corr"], ascending=False)
 
-    return numeric_collinear_df, numeric_collinear_summary_df
+    return numeric_collinear_df, master_columns_df
 
 
 def calc_max_rfscore(num=2):
     """
     Calculate the theoretical maximum R^2 score one could expect for a given
     number of unique values for a categorical feature.
 
@@ -227,15 +249,16 @@
             y_pred[int(jj*split*1000):] = split_mid + jj*split
 
     r2 = (1 - ((y - y_pred)**2).sum() / ((y - 0.5)**2).sum())
 
     return r2
 
 
-def calc_nonnumeric_features_target_corr(data_df, non_numeric_cols, target_col):
+def calc_nonnumeric_features_target_corr(data_df, non_numeric_cols, master_columns_df, target_col,
+                                         target_type='regression'):
     """
     Calculate the correlation between non-numeric features and the target
     variable.
 
     To do this, a random forest model is run for each feature, with just that
     feature and the target variable. And the R^2 is reported as a proxy for
     correlation.
@@ -278,44 +301,69 @@
 
     rf_n_estimators, min_samples_leaf = get_random_forest_hyperparams(len(data_df), rf_n_estimators='auto',
                                                                       numeric=False)
 
     print('For random forest (RF) correlation measure, using {} trees and min_samples_leaf={}.\n'.format(
         rf_n_estimators, min_samples_leaf))
 
-    non_numeric_df = pd.DataFrame(columns=["Count not-Null", "Num Unique", "Random Forest", "RF_norm"])
+    if target_type == 'regression':
+        non_numeric_df = pd.DataFrame(columns=["Count not-Null", "Mutual Info", "Random Forest", "RF_norm"])
+    else:
+        non_numeric_df = pd.DataFrame(columns=["Count not-Null", "Mutual Info", "Random Forest", "RF_norm"])
 
     # Loop over each categorical feature:
     print('Running correlations of non-numeric features to target variable...')
     for col in tqdm(non_numeric_cols):
         # Keep only rows that do not have NULL for that feature:
         train_col_notnull = data_df[[col, target_col]].dropna()
 
         # Split the feature into multiple features for the random forest
         # training using one-hot encoding:
         X_col = pd.get_dummies(train_col_notnull[col], dtype=int)
 
-        # Train a random forest model:
-        rf_reg = RandomForestRegressor(n_estimators=rf_n_estimators, min_samples_leaf=min_samples_leaf)
-        rf_reg.fit(X_col, train_col_notnull[target_col].values)
-        rfscore = rf_reg.score(X_col, train_col_notnull[target_col])
-
-        # The number of unique values is calculated for the purpose of
-        # adjusting the Random Forest R^2:
-        num_uniq = train_col_notnull[col].nunique()
-        # Adjust the R^2 based on the number of unique values affecting a
-        # feature's maximum theoretical R^2:
-        rfscore_norm = rfscore * (1 / calc_max_rfscore(num_uniq))
+        if target_type == 'regression':
+            # Calculate the Mutual Information for feature and target:
+            minfo = mutual_info_regression(
+                LabelEncoder().fit_transform(train_col_notnull[col]).reshape(-1, 1),
+                train_col_notnull[target_col].values, discrete_features=True)[0]
+
+            # Train a random forest model:
+            rf_reg = RandomForestRegressor(n_estimators=rf_n_estimators, min_samples_leaf=min_samples_leaf)
+            rf_reg.fit(X_col, train_col_notnull[target_col].values)
+            rfscore = max(rf_reg.score(X_col, train_col_notnull[target_col]), 0)
+
+            # The number of unique values is calculated for the purpose of
+            # adjusting the Random Forest R^2:
+            num_uniq = master_columns_df.loc[col, "Num Unique Values"]
+            # Adjust the R^2 based on the number of unique values affecting a
+            # feature's maximum theoretical R^2:
+            rfscore_norm = rfscore * (1 / calc_max_rfscore(num_uniq))
+
+            # Save the results as a new row in the dataframe for output:
+            non_numeric_df.loc[col] = len(train_col_notnull), round(minfo, 2), round(rfscore, 2), round(rfscore_norm, 2)
+
+        else:
+            minfo = mutual_info_classif(LabelEncoder().fit_transform(train_col_notnull[col]).reshape(-1, 1),
+                                        train_col_notnull[target_col].values, discrete_features=True)[0]
+
+            # Train a random forest model with just that feature and the target variable:
+            rf_class = RandomForestClassifier(n_estimators=rf_n_estimators, min_samples_leaf=min_samples_leaf)
+            rf_class.fit(X_col, train_col_notnull[target_col].values)
+            y_train_pred = rf_class.predict(X_col)
+            rf_ck = max(cohen_kappa_score(train_col_notnull[target_col].values, y_train_pred), 0)
+
+            # Save the results as a new row in the dataframe for output:
+            num_uniq = master_columns_df.loc[col, "Num Unique Values"]
+            non_numeric_df.loc[col] = len(train_col_notnull), round(minfo, 2), round(rf_ck, 2), round(rf_ck, 2)
 
-        # Save the results as a new row in the dataframe for output:
-        non_numeric_df.loc[col] = len(train_col_notnull), num_uniq, round(rfscore, 2), round(rfscore_norm, 2)
+    master_columns_df.loc[non_numeric_df.index, non_numeric_df.columns] = non_numeric_df
 
     # The counts of NULL values and unique values should be integers:
-    non_numeric_df["Count not-Null"] = non_numeric_df["Count not-Null"].astype(int)
-    non_numeric_df["Num Unique"] = non_numeric_df["Num Unique"].astype(int)
+    # non_numeric_df["Count not-Null"] = non_numeric_df["Count not-Null"].astype(int)
+    # non_numeric_df["Num Unique"] = non_numeric_df["Num Unique"].astype(int)
 
     # Sort the dataframe by the adjusted Random Forest R^2 for each feature,
     # in descending order:
-    non_numeric_df = non_numeric_df.sort_values(by=["RF_norm"], ascending=False)
+    # non_numeric_df = non_numeric_df.sort_values(by=["RF_norm"], ascending=False)
 
-    return non_numeric_df
+    return master_columns_df
```

### Comparing `featuring-data-0.2.2/src/featuringdata/featuresEDA/_create_pdf_report.py` & `featuring_data-0.2.4/src/featuringdata/featuresEDA/_create_pdf_report.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     pdf.ln(2)
 
     return pdf
 
 
 def save_pdf_doc(pdf, custom_filename='FeatureSelection', timestamp=''):
     pdf.output('./{}_EDA_Report_{}.pdf'.format(custom_filename, timestamp), 'F')
+    print("File '{}_EDA_Report_{}.pdf' has been saved in current working directory.".format(custom_filename, timestamp))
 
 
 def adjust_fontsize_for_feature_names(pdf, feature, box_width=60, start_fontsize=12):
 
     # sum(i.isupper() for i in a)
     feat_len_adj = len(feature) + np.floor(sum(map(str.isupper, feature)) / 2).astype(int)
 
@@ -48,45 +49,49 @@
         pdf.set_font('Arial', '', font_size)
     pdf.cell(w=box_width, h=10, txt=feature, border=1, ln=0, align='L')
     pdf.set_font('Arial', '', start_fontsize)
 
     return pdf
 
 
-def section_on_null_columns(pdf, num_features, null_cols_df, null_count_by_row_series):
+def section_on_null_columns(pdf, num_features, master_columns_df, null_count_by_row_series):
+
+    null_cols_df = master_columns_df.loc[
+        master_columns_df["Num of Nulls"] > 0, ["Num of Nulls", "Frac Null"]].sort_values(
+            by=["Num of Nulls"], ascending=False)
+
     pdf.set_font('Arial', 'B', 13)
     pdf.cell(w=0, h=10, txt="Null Values", ln=1)
 
     pdf.ln(2)
 
     pdf.set_font('Arial', 'B', 12)
     pdf.cell(w=0, h=10, txt="Null Values by Columns/Features", ln=1)
 
     pdf.set_font('Arial', '', 12)
-    # TODO: Indicate also if target_col has nulls
-    output_txt = "Out of {} total feature columns, there are {} columns with at least 1 null value.".format(
+    output_txt = "Out of {} total data columns, there are {} columns with at least 1 null value.".format(
         num_features, len(null_cols_df))
     print(output_txt + '\n')
     pdf.cell(w=0, h=10, txt=output_txt, ln=1)
 
     pdf.ln(3)
 
     if len(null_cols_df) == 0:
         return pdf
 
     # Table Header
     pdf.set_font('Arial', 'B', 12)
-    pdf.cell(w=60, h=10, txt=null_cols_df.columns[0], border=1, ln=0, align='C')
-    pdf.cell(w=35, h=10, txt=null_cols_df.columns[1], border=1, ln=0, align='C')
-    pdf.cell(w=35, h=10, txt=null_cols_df.columns[2], border=1, ln=1, align='C')
+    pdf.cell(w=60, h=10, txt="Feature", border=1, ln=0, align='C')
+    pdf.cell(w=35, h=10, txt=null_cols_df.columns[0], border=1, ln=0, align='C')
+    pdf.cell(w=35, h=10, txt=null_cols_df.columns[1], border=1, ln=1, align='C')
 
     # Table contents
     pdf.set_font('Arial', '', 12)
     for ii in range(0, min(8, len(null_cols_df))):
-        pdf = adjust_fontsize_for_feature_names(pdf, null_cols_df["Feature"].iloc[ii])
+        pdf = adjust_fontsize_for_feature_names(pdf, null_cols_df.index[ii])
         pdf.cell(w=35, h=10, txt=null_cols_df["Num of Nulls"].iloc[ii].astype(str), border=1, ln=0, align='R')
         pdf.cell(w=35, h=10, txt=null_cols_df["Frac Null"].iloc[ii].astype(str), border=1, ln=1, align='R')
 
     pdf.ln(6)
     pdf.set_font('Arial', 'B', 12)
     pdf.cell(w=0, h=10, txt="Null Values by Rows/Data Samples", ln=1)
 
@@ -111,114 +116,179 @@
     output_txt = 'The row with the most NULL values has {} NULLs.'.format(np.max(null_count_by_row))
     print(output_txt)
     pdf.cell(w=0, h=10, txt=output_txt, ln=1)
 
     return pdf
 
 
-def section_on_unique_values(pdf, numeric_cols, non_numeric_cols, numeric_uniq_vals_df, non_numeric_uniq_vals_df,
-                             single_value_cols_numeric_df=None, numeric_cols_to_cat_df=None,
-                             single_value_cols_nonnumeric_df=None, nonnumeric_uniq_vals_thresh=5):
+def section_on_unique_values(pdf, master_columns_df, nonnumeric_uniq_vals_thresh=5):
     pdf.add_page()
     pdf.set_font('Arial', 'B', 13)
     pdf.cell(w=0, h=10, txt="Numeric vs Non-Numeric Features and Unique Values Count", ln=1)
 
+    num_numeric_cols = len(master_columns_df.loc[master_columns_df["Column Type (orig)"] == 'numeric'])
+    num_nonnumeric_cols = len(master_columns_df.loc[master_columns_df["Column Type (orig)"] == 'non-numeric'])
+
     pdf.set_font('Arial', '', 12)
     pdf.cell(w=0, h=10,
              txt="Out of {} total feature columns, there are {} numeric columns and {} non-numeric columns.".format(
-                 len(numeric_cols)+len(non_numeric_cols), len(numeric_cols), len(non_numeric_cols)),
+                 num_numeric_cols+num_nonnumeric_cols, num_numeric_cols, num_nonnumeric_cols),
              ln=1)
 
     pdf.ln(3)
 
-    if ((single_value_cols_numeric_df is not None and len(single_value_cols_numeric_df) > 0) or
-            (numeric_cols_to_cat_df is not None and len(numeric_cols_to_cat_df) > 0)):
+    # Table Header
+    max_table_len = 8
+    numeric_uniq_vals_df = master_columns_df.loc[
+        (master_columns_df["Column Type (orig)"] == 'numeric') & (master_columns_df["Num Unique Values"] <= 10),
+        ["Num Unique Values"]].sort_values(by=["Num Unique Values"])
+    pdf.set_font('Arial', 'B', 12)
+    pdf.cell(w=60, h=10, txt='Numeric Feature', border=1, ln=0, align='C')
+    pdf.cell(w=42, h=10, txt=numeric_uniq_vals_df.columns[0], border=1, ln=1, align='C')
+
+    pdf.set_font('Arial', '', 12)
+    if len(numeric_uniq_vals_df) == 0:
+        output_txt = 'There are no numeric columns with 10 or fewer unique values.'
+        print(output_txt)
+        pdf.cell(w=0, h=10, txt=output_txt, ln=1)
+    
+    else:
+        # Table Contents
+        for ii in range(0, min(max_table_len, len(numeric_uniq_vals_df))):
+            pdf = adjust_fontsize_for_feature_names(pdf, numeric_uniq_vals_df.index[ii])
+            pdf.cell(w=42, h=10,
+                    txt=numeric_uniq_vals_df["Num Unique Values"].iloc[ii].astype(str),
+                    border=1, ln=1, align='R')
+
+    if len(numeric_uniq_vals_df) > max_table_len:
+        pdf.cell(w=0, h=10,
+                 txt="There are an additional {} numeric feature columns with 10 or fewer unique values.".format(
+                     len(numeric_uniq_vals_df) - max_table_len),
+                 ln=1)
+
+    pdf.ln(4)
 
-        if single_value_cols_numeric_df is not None and len(single_value_cols_numeric_df) > 0:
+    if len(master_columns_df.loc[master_columns_df["Column Type (orig)"] == 'numeric', "Column Note"].dropna()) > 0:
+        num_single_val = len(master_columns_df.loc[
+            (master_columns_df["Column Type (orig)"] == 'numeric') & (master_columns_df["Column Note"] == 'remove')])
+        
+        if num_single_val > 0:
             pdf.set_font('Arial', 'B', 12)
-            pdf.cell(w=0, h=10,
-                     txt="There are {} numeric columns with just a single value and will be removed.".format(
-                         len(single_value_cols_numeric_df)), ln=1)
-            pdf.ln(4)
+            output_txt = "There are {} numeric columns with just a single value and will be removed.".format(
+                num_single_val)
+            print(output_txt)
+            pdf.cell(w=0, h=10, txt=output_txt, ln=1)
+            pdf.ln(6)
 
-        if numeric_cols_to_cat_df is not None and len(numeric_cols_to_cat_df) > 0:
+        num_switch = len(master_columns_df.loc[master_columns_df["Column Note"] == 'switch to non-numeric'])
+        
+        if num_switch > 0:
             pdf.set_font('Arial', 'B', 12)
             output_txt = 'There are {} numeric columns that will be switched to categorical.'.format(
-                len(numeric_cols_to_cat_df))
+                num_switch)
             print(output_txt)
             pdf.cell(w=0, h=10, txt=output_txt, ln=1)
-            pdf.ln(4)
+            pdf.ln(6)
 
-    else:
-        # Table Header
-        pdf.set_font('Arial', 'B', 12)
-        pdf.cell(w=60, h=10, txt='Numeric Feature', border=1, ln=0, align='C')
-        pdf.cell(w=42, h=10, txt=numeric_uniq_vals_df.columns[1], border=1, ln=1, align='C')
+    # Table Header
+    non_numeric_uniq_vals_df_tmp = master_columns_df.loc[
+        (master_columns_df["Column Type (orig)"] == 'non-numeric') & (master_columns_df["Num Unique Values"] > nonnumeric_uniq_vals_thresh),
+        ["Num Unique Values"]].sort_values(by=["Num Unique Values"], ascending=False)
 
-        # Table Contents
-        pdf.set_font('Arial', '', 12)
-        for ii in range(0, min(8, len(numeric_uniq_vals_df))):
-            pdf = adjust_fontsize_for_feature_names(pdf, numeric_uniq_vals_df["Feature"].iloc[ii])
+    pdf.set_font('Arial', 'B', 12)
+    pdf.cell(w=60, h=10, txt='Non-Numeric Feature', border=1, ln=0, align='C')
+    pdf.cell(w=42, h=10, txt=non_numeric_uniq_vals_df_tmp.columns[0], border=1, ln=1, align='C')
+
+    pdf.set_font('Arial', '', 12)
+    if len(non_numeric_uniq_vals_df_tmp) == 0:
+        output_txt = 'There are no non-numeric columns with more than {} unique values.'.format(nonnumeric_uniq_vals_thresh)
+        print(output_txt)
+        pdf.cell(w=0, h=10, txt=output_txt, ln=1)
+
+    else:
+        # Table contents
+        for ii in range(0, min(max_table_len, len(non_numeric_uniq_vals_df_tmp))):
+            pdf = adjust_fontsize_for_feature_names(pdf, non_numeric_uniq_vals_df_tmp.index[ii])
             pdf.cell(w=42, h=10,
-                     txt=numeric_uniq_vals_df["Num Unique Values"].iloc[ii].astype(str),
-                     border=1, ln=1, align='R')
+                    txt=non_numeric_uniq_vals_df_tmp["Num Unique Values"].iloc[ii].astype(str),
+                    border=1, ln=1, align='R')
 
-        if len(numeric_uniq_vals_df) > 5:
-            pdf.cell(w=0, h=10,
-                     txt="There are an additional {} numeric feature columns with 10 or fewer unique values.".format(
-                         len(numeric_uniq_vals_df) - 5),
-                     ln=1)
+    if len(non_numeric_uniq_vals_df_tmp) > max_table_len:
+        pdf.cell(w=0, h=10,
+                 txt="There are an additional {} non-numeric feature columns with more than {} unique values.".format(
+                     len(non_numeric_uniq_vals_df_tmp) - max_table_len, nonnumeric_uniq_vals_thresh), ln=1)
 
     pdf.ln(4)
 
-    if single_value_cols_nonnumeric_df is not None and len(single_value_cols_nonnumeric_df) > 0:
+    num_issues = len(master_columns_df.loc[master_columns_df["Column Type (orig)"] == 'non-numeric', "Column Note"].dropna())
+    if num_issues > 0:
+        num_single = len(master_columns_df.loc[
+            (master_columns_df["Column Type (orig)"] == 'non-numeric') & (master_columns_df["Num Unique Values"] == 1)])
         pdf.set_font('Arial', 'B', 12)
-        pdf.cell(w=0, h=10,
-                 txt="There are {} non-numeric columns with just a single value and will be removed.".format(
-                     len(single_value_cols_nonnumeric_df)), ln=1)
+        output_txt = "There are {} non-numeric columns with just a single value and will be removed.".format(
+            num_single)
+        print(output_txt)
+        pdf.cell(w=0, h=10, txt=output_txt, ln=1)
+        output_txt = "There are {} non-numeric columns with a very large number of unique values and will be removed.".format(
+            num_issues-num_single)
+        print(output_txt)
+        pdf.cell(w=0, h=10, txt=output_txt, ln=1)
         pdf.ln(4)
+    
+    if len(master_columns_df["Column Note"].dropna()) > 0:
+        pdf.ln(8)
+        num_numeric_cols = len(master_columns_df.loc[master_columns_df["Column Type"] == 'numeric'])
+        num_nonnumeric_cols = len(master_columns_df.loc[master_columns_df["Column Type"] == 'non-numeric'])
+        pdf.set_font('Arial', '', 12)
+        output_txt = ("After the above adjustments, there are now {} data columns, with {} numeric columns and {} "
+                      "non-numeric/categorical columns.").format(
+                          num_numeric_cols+num_nonnumeric_cols, num_numeric_cols, num_nonnumeric_cols)
+        print(output_txt)
+        pdf.write(5, output_txt)
 
-    # Table Header
-    non_numeric_uniq_vals_df_tmp = non_numeric_uniq_vals_df.loc[
-        non_numeric_uniq_vals_df["Num Unique Values"] > nonnumeric_uniq_vals_thresh]
+    return pdf
 
-    pdf.set_font('Arial', 'B', 12)
-    pdf.cell(w=60, h=10, txt='Non-Numeric Feature', border=1, ln=0, align='C')
-    pdf.cell(w=42, h=10, txt=non_numeric_uniq_vals_df_tmp.columns[1], border=1, ln=1, align='C')
 
-    # Table contents
+def section_on_target_column(pdf, target_col, target_type, target_num_null, target_num_uniq):
+
+    pdf.add_page()
+
+    pdf.set_font('Arial', 'B', 13)
+    pdf.cell(w=0, h=10, txt="Target Column", ln=1)
+
+    pdf.ln(2)
     pdf.set_font('Arial', '', 12)
-    for ii in range(0, min(8, len(non_numeric_uniq_vals_df_tmp))):
-        pdf = adjust_fontsize_for_feature_names(pdf, non_numeric_uniq_vals_df_tmp["Feature"].iloc[ii])
-        pdf.cell(w=42, h=10,
-                 txt=non_numeric_uniq_vals_df_tmp["Num Unique Values"].iloc[ii].astype(str),
-                 border=1, ln=1, align='R')
+    output_txt = "For the chosen target column ('{}'), this appears to be a {} problem.".format(
+        target_col, target_type)
+    print(output_txt)
+    pdf.write(5, output_txt)
 
-    if len(non_numeric_uniq_vals_df_tmp) > 5:
-        pdf.cell(w=0, h=10,
-                 txt="There are an additional {} non-numeric feature columns with more than {} unique values.".format(
-                     len(non_numeric_uniq_vals_df_tmp) - 5, nonnumeric_uniq_vals_thresh), ln=1)
+    pdf.ln(6)
+    output_txt = "The target column has {} null values and {} unique values.".format(
+        target_num_null, target_num_uniq)
+    print(output_txt)
+    pdf.write(5, output_txt)
+
+    pdf.ln(12)
 
     return pdf
 
 
-def section_on_unique_values_p2(pdf, numeric_cols, non_numeric_cols):
+def section_on_target_column_plot(pdf, plots_folder='./'):
 
-    pdf.ln(3)
-    pdf.set_font('Arial', '', 12)
-    output_txt = ("After the above adjustments, there are now {} feature columns, with {} numeric columns and {} "
-                  "non-numeric/categorical columns.").format(
-        len(numeric_cols)+len(non_numeric_cols), len(numeric_cols), len(non_numeric_cols))
-    print(output_txt)
+    pdf.image('{}/target_data_distribution.png'.format(plots_folder), x=10, y=None, w=160, h=0, type='PNG')
+    pdf.ln(2)
+
+    output_txt = "The above plot shows the distribution of values in the target column."
     pdf.write(5, output_txt)
 
     return pdf
 
 
-def section_on_feature_corr(pdf, numeric_df, numeric_collinear_summary_df, non_numeric_df, plots_folder='./'):
+def section_on_feature_corr(pdf, master_columns_df, target_type='regression', plots_folder='./'):
 
     pdf.add_page()
 
     pdf.set_font('Arial', 'B', 13)
     pdf.cell(w=0, h=10, txt="Feature Correlations", ln=1)
 
     # ------------------------------------------------------------------------
@@ -226,47 +296,55 @@
 
     pdf.ln(2)
     pdf.set_font('Arial', 'B', 12)
     pdf.cell(w=0, h=10, txt="Correlations of Numeric Features with Target Variable", ln=1)
 
     pdf.ln(2)
 
+    numeric_df = master_columns_df.loc[
+        master_columns_df["Column Type"] == 'numeric'].sort_values(by=["Random Forest"], ascending=False)
+
     if len(numeric_df) == 0:
         pdf.cell(w=0, h=10, txt="** No numeric features in this dataset. **", align='C')
 
     else:
         # Table Header
         pdf.set_font('Arial', 'B', 12)
         pdf.cell(w=60, h=10, txt='Numeric Feature', border=1, ln=0, align='C')
         pdf.cell(w=35, h=10, txt='Count non-Null', border=1, ln=0, align='C')
-        pdf.cell(w=35, h=10, txt='Pearson Corr', border=1, ln=0, align='C')
+        txt = 'Pearson Corr' if target_type == 'regression' else 'Mutual Info'
+        pdf.cell(w=35, h=10, txt=txt, border=1, ln=0, align='C')
         pdf.cell(w=35, h=10, txt='RF Corr', border=1, ln=1, align='C')
 
         # Table contents
         pdf.set_font('Arial', '', 12)
         for ii in range(0, min(8, len(numeric_df))):
             pdf = adjust_fontsize_for_feature_names(pdf, numeric_df.index[ii])
             pdf.cell(w=35, h=10, txt=numeric_df["Count not-Null"].iloc[ii].astype(str), border=1, ln=0, align='R')
-            pdf.cell(w=35, h=10, txt=numeric_df["Pearson"].iloc[ii].astype(str), border=1, ln=0, align='R')
+            cell = "Pearson" if target_type == 'regression' else "Mutual Info"
+            pdf.cell(w=35, h=10, txt=numeric_df[cell].iloc[ii].astype(str), border=1, ln=0, align='R')
             pdf.cell(w=35, h=10, txt=numeric_df["Random Forest"].iloc[ii].astype(str), border=1, ln=1, align='R')
-
+        
         pdf.ln(6)
         pdf.image('{}/numeric_columns_target_correlation_hist.png'.format(plots_folder),
                   x=10, y=None, w=160, h=0, type='PNG')
         pdf.ln(2)
 
         output_txt = ('The above plot shows a histogram of all numeric features and their correlation value with the '
                       'target variable.')
         pdf.write(5, output_txt)
         pdf.ln(7)
 
     # ------------------------------------------------------------------------
     # Correlations Between Numeric Features
 
-    if len(numeric_collinear_summary_df) > 0:
+    if "COLLIN Max RF Corr" in master_columns_df.columns:
+        numeric_collinear_summary_df = master_columns_df.loc[
+            master_columns_df["Column Type"] == 'numeric'].sort_values(by=["COLLIN Max RF Corr"], ascending=False)
+
         pdf.add_page()
         pdf.set_font('Arial', 'B', 12)
         pdf.cell(w=0, h=10, txt="Correlations between Numeric Features", ln=1)
 
         pdf.ln(2)
 
         # Table Header
@@ -288,27 +366,27 @@
         pdf.cell(w=17, h=6, txt='Corr', border='LBR', ln=1, align='C')
 
         # Table contents
         pdf.set_font('Arial', '', 10)
         for ii in range(0, min(8, len(numeric_collinear_summary_df))):
             pdf = adjust_fontsize_for_feature_names(
                 pdf, numeric_collinear_summary_df.index[ii], box_width=44, start_fontsize=10)
-            pdf.cell(w=23, h=10, txt=numeric_collinear_summary_df["Avg Pearson Corr"].iloc[ii].astype(str), border=1,
+            pdf.cell(w=23, h=10, txt=numeric_collinear_summary_df["COLLIN Avg Pearson Corr"].iloc[ii].astype(str), border=1,
                      ln=0, align='R')
-            pdf.cell(w=22, h=10, txt=numeric_collinear_summary_df["Avg RF Corr"].iloc[ii].astype(str), border=1,
+            pdf.cell(w=22, h=10, txt=numeric_collinear_summary_df["COLLIN Avg RF Corr"].iloc[ii].astype(str), border=1,
                      ln=0, align='R')
             pdf.set_font('Arial', '', 8)
             pdf = adjust_fontsize_for_feature_names(
-                pdf, numeric_collinear_summary_df["Max Pear Corr Feature"].iloc[ii], box_width=33, start_fontsize=10)
-            pdf.cell(w=18, h=10, txt=numeric_collinear_summary_df["Max Pear"].iloc[ii].astype(str), border=1,
+                pdf, numeric_collinear_summary_df["COLLIN Max Pear Corr Feature"].iloc[ii], box_width=33, start_fontsize=10)
+            pdf.cell(w=18, h=10, txt=numeric_collinear_summary_df["COLLIN Max Pear"].iloc[ii].astype(str), border=1,
                      ln=0, align='R')
             pdf.set_font('Arial', '', 8)
             pdf = adjust_fontsize_for_feature_names(
-                pdf, numeric_collinear_summary_df["Max RF Corr Feature"].iloc[ii], box_width=33, start_fontsize=10)
-            pdf.cell(w=17, h=10, txt=numeric_collinear_summary_df["Max RF Corr"].iloc[ii].astype(str), border=1,
+                pdf, numeric_collinear_summary_df["COLLIN Max RF Corr Feature"].iloc[ii], box_width=33, start_fontsize=10)
+            pdf.cell(w=17, h=10, txt=numeric_collinear_summary_df["COLLIN Max RF Corr"].iloc[ii].astype(str), border=1,
                      ln=1, align='R')
 
         pdf.ln(6)
         pdf.image('{}/numeric_columns_collinear_correlation_hist.png'.format(plots_folder),
                   x=15, y=None, w=160, h=0, type='PNG')
         pdf.ln(2)
 
@@ -323,42 +401,54 @@
     pdf.add_page()
 
     pdf.set_font('Arial', 'B', 12)
     pdf.cell(w=0, h=10, txt="Correlations of Non-Numeric Features with Target Variable", ln=1)
 
     pdf.ln(2)
 
+    sort_col = "RF_norm" if "RF_norm" in master_columns_df.columns else "Random Forest"
+    non_numeric_df = master_columns_df.loc[
+        master_columns_df["Column Type"] == 'non-numeric'].sort_values(by=[sort_col], ascending=False)
+
     if len(non_numeric_df) == 0:
         pdf.cell(w=0, h=10, txt="** No non-numeric features in this dataset. **", align='C')
         return pdf
 
     # Table Header
     pdf.set_font('Arial', 'B', 12)
-    pdf.cell(w=60, h=10, txt='Non-Numeric Feature', border=1, ln=0, align='C')
-    pdf.cell(w=32, h=10, txt='Count non-Null', border=1, ln=0, align='C')
-    pdf.cell(w=28, h=10, txt='Num Unique', border=1, ln=0, align='C')
-    pdf.cell(w=30, h=10, txt='RF Corr', border=1, ln=0, align='C')
-    pdf.cell(w=30, h=10, txt='RF Corr (norm)', border=1, ln=1, align='C')
+    pdf.cell(w=60, h=6, txt='Non-Numeric Feature', border='LTR', ln=0, align='C')
+    pdf.cell(w=24, h=6, txt='Count', border='LTR', ln=0, align='C')
+    pdf.cell(w=24, h=6, txt='Num', border='LTR', ln=0, align='C')
+    pdf.cell(w=26, h=6, txt='Mutual', border='LTR', ln=0, align='C')
+    if target_type == 'regression':
+        pdf.cell(w=26, h=6, txt='RF Corr', border='LTR', ln=0, align='C')
+    pdf.cell(w=26, h=6, txt='RF Corr', border='LTR', ln=1, align='C')
+
+    pdf.cell(w=60, h=6, txt='', border='LBR', ln=0, align='C')
+    pdf.cell(w=24, h=6, txt='non-Null', border='LBR', ln=0, align='C')
+    pdf.cell(w=24, h=6, txt='Unique', border='LBR', ln=0, align='C')
+    pdf.cell(w=26, h=6, txt='Info', border='LBR', ln=0, align='C')
+    if target_type == 'regression':
+        pdf.cell(w=26, h=6, txt='', border='LBR', ln=0, align='C')
+        pdf.cell(w=26, h=6, txt='(norm)', border='LBR', ln=1, align='C')
+    else:
+        pdf.cell(w=26, h=6, txt='', border='LBR', ln=1, align='C')
 
     # Table contents
     pdf.set_font('Arial', '', 12)
     for ii in range(0, min(8, len(non_numeric_df))):
         pdf = adjust_fontsize_for_feature_names(pdf, non_numeric_df.index[ii])
-        pdf.cell(w=32, h=10,
-                 txt=non_numeric_df["Count not-Null"].iloc[ii].astype(str),
-                 border=1, ln=0, align='R')
-        pdf.cell(w=28, h=10,
-                 txt=non_numeric_df["Num Unique"].iloc[ii].astype(str),
-                 border=1, ln=0, align='R')
-        pdf.cell(w=30, h=10,
-                 txt=non_numeric_df["Random Forest"].iloc[ii].astype(str),
-                 border=1, ln=0, align='R')
-        pdf.cell(w=30, h=10,
-                 txt=non_numeric_df["RF_norm"].iloc[ii].astype(str),
-                 border=1, ln=1, align='R')
+        pdf.cell(w=24, h=10, txt=non_numeric_df["Count not-Null"].iloc[ii].astype(str), border=1, ln=0, align='R')
+        pdf.cell(w=24, h=10, txt=non_numeric_df["Num Unique Values"].iloc[ii].astype(str), border=1, ln=0, align='R')
+        pdf.cell(w=26, h=10, txt=non_numeric_df["Mutual Info"].iloc[ii].astype(str), border=1, ln=0, align='R')
+        if target_type == 'regression':
+            pdf.cell(w=26, h=10, txt=non_numeric_df["Random Forest"].iloc[ii].astype(str), border=1, ln=0, align='R')
+            pdf.cell(w=26, h=10, txt=non_numeric_df["RF_norm"].iloc[ii].astype(str), border=1, ln=1, align='R')
+        else:
+            pdf.cell(w=26, h=10, txt=non_numeric_df["Random Forest"].iloc[ii].astype(str), border=1, ln=1, align='R')
 
     pdf.ln(6)
     pdf.image('{}/non_numeric_columns_target_correlation_hist.png'.format(plots_folder),
               x=15, y=None, w=160, h=0, type='PNG')
     pdf.ln(2)
 
     output_txt = ('The above plot shows a histogram of all non-numeric features and their correlation value with the '
@@ -383,10 +473,16 @@
             pdf.add_page()
         else:
             pdf.ln(4)
 
         # TODO: Double-check that file exists
         pdf.image('{}/{}_vs_{}.png'.format(plots_folder, column, target_col),
                   x=10, y=None, w=0, h=130, type='PNG')
+        
+        if jj == 150:
+            pdf.ln(2)
+            pdf.set_font('Arial', 'B', 12)
+            pdf.cell(w=0, h=20, txt="Any additional plots are located in '{}'.".format(plots_folder), align='C')
+            break
 
     return pdf
```

### Comparing `featuring-data-0.2.2/src/featuringdata/featuresEDA/_features_eda.py` & `featuring_data-0.2.4/src/featuringdata/featuresEDA/_features_eda.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,34 +5,37 @@
 import numpy as np
 import pandas as pd
 
 from ._create_pdf_report import (
     initialize_pdf_doc,
     section_on_null_columns,
     section_on_unique_values,
-    section_on_unique_values_p2,
+    section_on_target_column,
+    section_on_target_column_plot,
     section_on_feature_corr,
     section_of_plots,
     save_pdf_doc
 )
 
 from ._initial_eda_functions import (
     count_null_values,
     sort_numeric_nonnumeric_columns,
-    count_numeric_unique_values,
-    count_nonnumeric_unique_values
 )
 
 from ._correlation import (
     calc_numeric_features_target_corr,
     calc_corr_numeric_features,
     calc_nonnumeric_features_target_corr
 )
 
-from ._generate_plots import plot_ecdf, plot_hist, plot_feature_values
+from ._generate_plots import (
+    plot_hist,
+    plot_hist_target_col,
+    plot_feature_values
+)
 
 
 class FeaturesEDA:
     """
     This class implements Exploratory Data Analysis (EDA) on an input dataset.
 
     The results of the EDA are available within your Jupyter Notebook
@@ -196,28 +199,19 @@
         self.report_prefix = report_prefix
         self.target_col = target_col
         self.cols_to_drop = cols_to_drop
         self.numeric_uniq_vals_thresh = numeric_uniq_vals_thresh
         self.nonnumeric_uniq_vals_thresh = nonnumeric_uniq_vals_thresh
 
         self.pdf = None
-        self.null_cols_df = None
         self.null_count_by_row_series = None
         # TODO: Combine unique values and corr info into one DF
         self.numeric_cols = None
         self.non_numeric_cols = None
-        self.numeric_uniq_vals_df = None
-        self.non_numeric_uniq_vals_df = None
-        self.numeric_df = pd.DataFrame()
         self.numeric_collinear_df = pd.DataFrame()
-        self.numeric_collinear_summary_df = pd.DataFrame()
-        self.non_numeric_df = pd.DataFrame()
-
-    # TODO Create function that does up to correlation
-    # TODO For full EDA, make collinear correlation optional
 
     def run_initial_eda(self, data_df, output=True):
         """
         Run an initial exploratory data analysis (EDA) on a given dataset.
 
         This function runs the following steps:
         - Null values analysis
@@ -247,79 +241,58 @@
         if self.cols_to_drop is not None:
             data_df = data_df.drop(columns=self.cols_to_drop)
 
         # --------------------------------------------------------------------
         # Generating PDF Document
         self.pdf = initialize_pdf_doc()
 
+        # Initialize dataframe for column/feature statistics
+        self.master_columns_df = pd.DataFrame(index=data_df.columns)
+
         # --------------------------------------------------------------------
         # Null Values Analysis
         print('--- Null Values Analysis ---')
 
-        self.null_cols_df, self.null_count_by_row_series = count_null_values(data_df)
+        self.master_columns_df, self.null_count_by_row_series = count_null_values(data_df, self.master_columns_df)
 
         # PDF Page 1: Summary of Null values information and unique values for numeric and non-numeric feature columns
-        self.pdf = section_on_null_columns(self.pdf, data_df.shape[1], self.null_cols_df, self.null_count_by_row_series)
+        self.pdf = section_on_null_columns(self.pdf, data_df.shape[1], self.master_columns_df, self.null_count_by_row_series)
         print()
 
         # --------------------------------------------------------------------
         # Sort Numeric and Non-numeric/Categorical Columns
         print('--- Sorting Numeric and Non-numeric Columns / Unique Values ---')
 
-        self.numeric_cols, self.non_numeric_cols = sort_numeric_nonnumeric_columns(data_df, self.target_col)
+        self.master_columns_df = sort_numeric_nonnumeric_columns(data_df, self.master_columns_df, self.target_col)
+
+        self.pdf = section_on_unique_values(self.pdf, self.master_columns_df)
+
+        # # Removing any columns with only a single unique value.
+
+
+        # --------------------------------------------------------------------
+        # Target Column
+
+        if self.target_col is not None:
+            print('\n--- Target Column ---')
 
-        # Count the number of unique values for each feature
-        self.numeric_uniq_vals_df = count_numeric_unique_values(
-            data_df, self.numeric_cols, uniq_vals_thresh=self.numeric_uniq_vals_thresh)
-
-        self.non_numeric_uniq_vals_df = count_nonnumeric_unique_values(
-            data_df, self.non_numeric_cols, uniq_vals_thresh=self.nonnumeric_uniq_vals_thresh)
-
-        # Identify any numeric columns with just a single unique value:
-        single_value_cols_numeric_df = self.numeric_uniq_vals_df.loc[
-            self.numeric_uniq_vals_df["Num Unique Values"] == 1]
-
-        # Identify any numeric columns with only two unique values:
-        numeric_cols_to_cat_df = self.numeric_uniq_vals_df.loc[
-            self.numeric_uniq_vals_df["Num Unique Values"].between(2, 2, inclusive='both')]
-
-        # Identify any non-numeric columns with just a single unique value:
-        single_value_cols_nonnumeric_df = self.non_numeric_uniq_vals_df.loc[
-            self.non_numeric_uniq_vals_df["Num Unique Values"] == 1]
-
-        print('There are {} numeric and {} non-numeric columns with only a single value.'.format(
-            len(single_value_cols_numeric_df), len(single_value_cols_nonnumeric_df)))
-
-        self.pdf = section_on_unique_values(self.pdf, self.numeric_cols, self.non_numeric_cols,
-                                            self.numeric_uniq_vals_df, self.non_numeric_uniq_vals_df,
-                                            single_value_cols_numeric_df=single_value_cols_numeric_df,
-                                            single_value_cols_nonnumeric_df=single_value_cols_nonnumeric_df,
-                                            numeric_cols_to_cat_df=numeric_cols_to_cat_df)
-
-        # Removing any columns with only a single unique value. Any columns
-        # that are numeric, but were determined to be categorical are
-        # removed from the 'numeric_cols' list and added to the
-        # 'non_numeric_cols' list:
-        if ((len(single_value_cols_numeric_df) > 0) or (len(single_value_cols_nonnumeric_df) > 0) or
-                (len(numeric_cols_to_cat_df) > 0)):
-
-            if len(single_value_cols_numeric_df) > 0:
-                for col in single_value_cols_numeric_df["Feature"].values:
-                    self.numeric_cols.remove(col)
-
-            if len(single_value_cols_nonnumeric_df) > 0:
-                for col in single_value_cols_nonnumeric_df["Feature"].values:
-                    self.non_numeric_cols.remove(col)
-
-            if len(numeric_cols_to_cat_df) > 0:
-                for col in numeric_cols_to_cat_df["Feature"]:
-                    self.numeric_cols.remove(col)
-                    self.non_numeric_cols.append(col)
+            # Insert code / function here for target column nulls, unique values, distribution
+            target_col_notnull = data_df[self.target_col].dropna()
+            target_num_null = len(data_df) - len(target_col_notnull)
+            target_num_uniq = target_col_notnull.nunique()
+
+            if pd.api.types.is_string_dtype(target_col_notnull):
+                self.target_type = 'classification'
+            elif target_num_uniq <= 10:
+                self.target_type = 'classification'
+            else:
+                self.target_type = 'regression'
 
-            self.pdf = section_on_unique_values_p2(self.pdf, self.numeric_cols, self.non_numeric_cols)
+            self.pdf = section_on_target_column(self.pdf, self.target_col, self.target_type, target_num_null,
+                                                target_num_uniq)
 
         # Save PDF document to current working directory:
         if output:
             custom_filename = self.report_prefix + '_Initial'
             save_pdf_doc(self.pdf, custom_filename=custom_filename, timestamp=timestamp)
 
     def run_full_eda(self, data_df, run_collinear=True, generate_plots=True):
@@ -354,105 +327,144 @@
         Path(plots_folder).mkdir()
 
         # if self.cols_to_drop is not None:
         #     data_df = data_df.drop(columns=self.cols_to_drop)
 
         # Run the initial EDA steps:
         self.run_initial_eda(data_df, output=False)
+
+        plot_hist_target_col(data_df[self.target_col].dropna(), target_type=self.target_type, plots_folder=plots_folder)
+        self.pdf = section_on_target_column_plot(self.pdf, plots_folder)
+
         print()
 
         # --------------------------------------------------------------------
         # Calculate feature correlations
 
+        print('--- Feature Correlations ---')
+
+        self.numeric_cols = self.master_columns_df.loc[
+            self.master_columns_df["Column Type"] == 'numeric'].index.to_list()
+        self.non_numeric_cols = self.master_columns_df.loc[
+            self.master_columns_df["Column Type"] == 'non-numeric'].index.to_list()
+
         # Calculate correlations between each numeric feature and the target
         # variable:
         if len(self.numeric_cols) > 0:
-            self.numeric_df = calc_numeric_features_target_corr(data_df, self.numeric_cols, self.target_col,
-                                                                rf_n_estimators='auto')
+            self.master_columns_df = calc_numeric_features_target_corr(data_df, self.numeric_cols, self.master_columns_df,
+                                                                       self.target_col, self.target_type, rf_n_estimators='auto')
         else:
             run_collinear = False
 
         # Calculate correlations between numeric features:
         if run_collinear:
-            self.numeric_collinear_df, self.numeric_collinear_summary_df = calc_corr_numeric_features(data_df,
-                                                                                                      self.numeric_cols)
+            self.numeric_collinear_df, self.master_columns_df = calc_corr_numeric_features(
+                data_df, self.numeric_cols, self.master_columns_df)
 
         # Calculate correlations between each categorical feature and the
         # target variable:
         if len(self.non_numeric_cols) > 0:
-            self.non_numeric_df = calc_nonnumeric_features_target_corr(data_df, self.non_numeric_cols, self.target_col)
-
+            self.master_columns_df = calc_nonnumeric_features_target_corr(data_df, self.non_numeric_cols, self.master_columns_df,
+                                                                          self.target_col, self.target_type)
+        
+        # The counts of NULL values should be integers:
+        if self.target_col is not None:
+            self.master_columns_df.loc[self.target_col, "Count not-Null"] = data_df[self.target_col].notna().sum()
+        self.master_columns_df["Count not-Null"] = self.master_columns_df["Count not-Null"].astype('Int64')
+        
         # --------------------------------------------------------------------
         # Generating PDF Document
 
         # PDF Page 1: Generated during the 'run_initial_eda' function
 
         # PDF Pages 2-3: Summary of numeric and non-numeric feature
         # correlations:
 
         # plot_ecdf(np.abs(self.numeric_df["Pearson"].values), data_label="Pearson", outfile=False)
         # plot_ecdf(
         #     self.numeric_df["Random Forest"], data_label="Random Forest", xlabel='Correlation Value',
         #     filename='numeric_columns_target_correlation_ecdf', overplot=True, outfile=True, plots_folder=plots_folder)
 
-        if len(self.numeric_df) > 0:
-            plot_hist(data_for_bins=np.abs(self.numeric_df["Pearson"].values), label_bins='Pearson (abs)',
-                      data_for_line=self.numeric_df["Random Forest"].values, label_line="RF_corr",
-                      xlabel='Correlation Value', ylabel='Feature Count',
-                      filename='numeric_columns_target_correlation_hist', plots_folder=plots_folder)
+        if len(self.numeric_cols) > 0:
+            rf_vals = self.master_columns_df.loc[
+                self.master_columns_df["Column Type"] == 'numeric', "Random Forest"].values
+            if self.target_type == 'regression':
+                pearson_vals = self.master_columns_df.loc[
+                    self.master_columns_df["Column Type"] == 'numeric', "Pearson"].values
+                plot_hist(data_for_bins=np.abs(pearson_vals), label_bins='Pearson (abs)', data_for_line=rf_vals,
+                          label_line="RF_corr", xlabel='Correlation Value', ylabel='Feature Count',
+                          filename='numeric_columns_target_correlation_hist', plots_folder=plots_folder)
+            else:
+                plot_hist(data_for_bins=rf_vals, label_bins='RF Cohen-Kappa', xlabel='Correlation Value',
+                          ylabel='Feature Count', filename='numeric_columns_target_correlation_hist',
+                          plots_folder=plots_folder)
 
         if run_collinear:
             plot_hist(data_for_bins=np.abs(self.numeric_collinear_df["Pearson"].values), label_bins='Pearson (abs)',
                       data_for_line=self.numeric_collinear_df["Random Forest"].values, label_line="RF_corr",
                       xlabel='Correlation Value', ylabel='Count of Numeric Feature Pairs',
                       filename='numeric_columns_collinear_correlation_hist', plots_folder=plots_folder)
 
-        if len(self.non_numeric_df) > 0:
-            plot_hist(data_for_bins=self.non_numeric_df["Random Forest"].values, label_bins='RF_corr',
-                      data_for_line=self.non_numeric_df["RF_norm"].values, label_line="RF_corr (norm)",
-                      xlabel='Correlation Value', ylabel='Feature Count',
-                      filename='non_numeric_columns_target_correlation_hist', plots_folder=plots_folder)
-
-        self.pdf = section_on_feature_corr(self.pdf, self.numeric_df, self.numeric_collinear_summary_df,
-                                           self.non_numeric_df, plots_folder=plots_folder)
+        if len(self.non_numeric_cols) > 0:
+            rf_vals = self.master_columns_df.loc[
+                self.master_columns_df["Column Type"] == 'non-numeric', "Random Forest"].values
+            rf_corr_vals = self.master_columns_df.loc[
+                self.master_columns_df["Column Type"] == 'non-numeric', "RF_norm"].values
+            if self.target_type == 'regression':
+                plot_hist(data_for_bins=rf_vals, label_bins='RF_corr', data_for_line=rf_corr_vals,
+                          label_line="RF_corr (norm)", xlabel='Correlation Value', ylabel='Feature Count',
+                          filename='non_numeric_columns_target_correlation_hist', plots_folder=plots_folder)
+            else:
+                plot_hist(data_for_bins=rf_vals, label_bins='RF_corr', xlabel='Correlation Value',
+                          ylabel='Feature Count', filename='non_numeric_columns_target_correlation_hist',
+                          plots_folder=plots_folder)
+        
+        self.pdf = section_on_feature_corr(self.pdf, self.master_columns_df, self.target_type,
+                                           plots_folder=plots_folder)
 
         # --------------------------------------------------------------------
         # Generate EDA plots
 
         if generate_plots:
             # ----------------------------------
             # Generate plots of numeric features
 
-            if len(self.numeric_df) > 0:
+            if len(self.numeric_cols) > 0:
                 # Order the features by correlation with target variable, in
                 # descending order:
-                columns_list_ordered = self.numeric_df.index
+                columns_list_ordered = self.master_columns_df.loc[
+                    self.master_columns_df["Column Type"] == 'numeric'].sort_values(
+                        by=["Random Forest"], ascending=False).index.to_list()
 
                 # Generate plots of numeric features, and save them to the
                 # timestamped directory defined above:
-                plot_feature_values(data_df, columns_list_ordered, self.numeric_df, target_col=self.target_col,
-                                    numeric=True, plots_folder=plots_folder)
+                plot_feature_values(data_df, columns_list_ordered, self.master_columns_df, target_col=self.target_col,
+                                    numeric=True, target_type=self.target_type, plots_folder=plots_folder)
 
                 # Add the plots to the PDF:
                 self.pdf = section_of_plots(self.pdf, columns_list_ordered, target_col=self.target_col, numeric=True,
                                             plots_folder=plots_folder)
 
             # ----------------------------------
             # Generate plots of non-numeric features
 
-            if len(self.non_numeric_df) > 0:
+            if len(self.non_numeric_cols) > 0:
                 # Order the features by correlation with target variable, in
                 # descending order:
-                columns_list_ordered = self.non_numeric_df.index
+                columns_list_ordered = self.master_columns_df.loc[
+                    self.master_columns_df["Column Type"] == 'non-numeric'].sort_values(
+                        by=["RF_norm"], ascending=False).index.to_list()
 
                 # Generate plots of non-numeric features, and save them to the
                 # timestamped directory defined above:
-                plot_feature_values(data_df, columns_list_ordered, self.non_numeric_df, target_col=self.target_col,
-                                    numeric=False, plots_folder=plots_folder)
-
+                plot_feature_values(data_df, columns_list_ordered, self.master_columns_df, target_col=self.target_col,
+                                    numeric=False, target_type=self.target_type, plots_folder=plots_folder)
+                
                 # Add the plots to the PDF:
                 self.pdf = section_of_plots(self.pdf, columns_list_ordered, target_col=self.target_col, numeric=False,
                                             plots_folder=plots_folder)
 
+        print('\n--- Files Output ---')
         # Save PDF document to current working directory:
         save_pdf_doc(self.pdf, custom_filename=self.report_prefix, timestamp=timestamp)
+        print('All PNG files can be found in {}.'.format(plots_folder))
```

### Comparing `featuring-data-0.2.2/src/featuringdata/featuresEDA/_generate_plots.py` & `featuring_data-0.2.4/src/featuringdata/featuresEDA/_generate_plots.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,14 +47,32 @@
     plt.xlim(0, 1)
     plt.legend()
 
     plt.savefig('{}/{}.png'.format(plots_folder, filename), bbox_inches='tight')
     plt.close()
 
 
+def plot_hist_target_col(target_col_vals, target_type='regression', plots_folder='./'):
+
+    sns.set_theme(style="ticks", font_scale=1.2)
+    f, ax = plt.subplots(figsize=(9, 6))
+
+    if target_type == 'regression':
+        sns.histplot(data=target_col_vals)
+        plt.grid()
+        plt.xlim(target_col_vals.min(), target_col_vals.max())
+    else:
+        sns.histplot(data=target_col_vals, discrete=True, shrink=0.6)
+        ax.set_xticks(target_col_vals.unique())
+        plt.grid(axis='y')
+
+    plt.savefig('{}/target_data_distribution.png'.format(plots_folder), bbox_inches='tight')
+    plt.close()
+
+
 def plot_scatter_density(x, y, fig=None, ax=None, sort=True, bins=20, **kwargs):
     """
     Scatter plot colored by 2d histogram
     """
     if ax is None:
         fig, ax = plt.subplots()
 
@@ -83,16 +101,16 @@
     # norm = mpl.colors.Normalize(vmin=np.min(z), vmax=np.max(z))
     # cbar = fig.colorbar(mpl.cm.ScalarMappable(norm=norm), ax=ax, cmap='viridis')
     # cbar.ax.set_ylabel('Density')
 
     return ax
 
 
-def plot_feature_values(data_df, columns_list, correlation_df, target_col, numeric=True, catplot_style='scatterdense',
-                        plots_folder='./plots'):
+def plot_feature_values(data_df, columns_list, correlation_df, target_col, numeric=True, target_type='regression',
+                        catplot_style='scatterdense', plots_folder='./plots'):
     """
     Generate EDA plots that show each feature versus the target variable.
 
     The code automatically adjusts based on certain properties of the feature:
     - For categorical features, as well as numeric features with up to 10
       unique values, a box plot with a swarm plot is generated. If there are
       more than 1,000 data points, then only a random selection of 1,000
@@ -131,102 +149,111 @@
     """
 
     # backend_ = mpl.get_backend()
     # print('*** {} ***'.format(backend_))
     # mpl.use("Agg")
     # print('*** {} ***'.format(mpl.get_backend()))
 
-    start = time.time()
-    time1, time2 = 0., 0.
-
     # Set box plot display parameters:
     if catplot_style != 'scatterdense':
         box_params = {'whis': [0, 100], 'width': 0.6}
     else:
         box_params = {'whis': [0, 100], 'width': 0.6, 'fill': False, 'color': 'black'}
 
-    # Check for strong outliers in target column:
-    med = data_df[target_col].median()
-    std = data_df[target_col].std()
-    xx = np.where(data_df[target_col].values > med + 10*std)[0]
-    xx = np.append(xx, np.where(data_df[target_col].values < med - 10*std)[0])
     set_ylim = False
-    if xx.size > 0:
-        print('Target outlier points:', data_df[target_col].values[xx])
-
-        target_col_vals = data_df.reset_index().drop(xx)[target_col].values
-        target_min, target_max = np.min(target_col_vals), np.max(target_col_vals)
-        max_minus_min = target_max - target_min
-        ymin = target_min - 0.025*max_minus_min
-        ymax = target_max + 0.025*max_minus_min
-        print('New target min/max values:', target_min, target_max)
-        print('Set y-axis limits (for display only):', ymin, ymax)
-        set_ylim = True
+    if target_type == 'regression':
+        # Check for strong outliers in target column:
+        med = data_df[target_col].median()
+        std = data_df[target_col].std()
+        xx = np.where(data_df[target_col].values > med + 10*std)[0]
+        xx = np.append(xx, np.where(data_df[target_col].values < med - 10*std)[0])
+        if xx.size > 0:
+            print('Target outlier points:', data_df[target_col].values[xx])
+
+            target_col_vals = data_df.reset_index().drop(xx)[target_col].values
+            target_min, target_max = np.min(target_col_vals), np.max(target_col_vals)
+            max_minus_min = target_max - target_min
+            ymin = target_min - 0.025*max_minus_min
+            ymax = target_max + 0.025*max_minus_min
+            print('New target min/max values:', target_min, target_max)
+            print('Set y-axis limits (for display only): {:.2f} {:.2f}.\n'.format(ymin, ymax))
+            set_ylim = True
 
     sns.set_theme(style="ticks")
 
     print('Generating plots of {} features...'.format('numeric' if numeric else 'non-numeric/categorical'))
     for jj, column in enumerate(tqdm(columns_list)):
 
         f, ax = plt.subplots(figsize=(9, 6))
 
         data_df_col_notnull = data_df[[column, target_col]].dropna().reset_index()
 
-        # TODO: Use already calculated DF of unique values:
         # TODO: User can define this value:
-        if (not numeric) or (np.unique(data_df_col_notnull[column]).size <= 10):
+        num_uniq = correlation_df.loc[column, "Num Unique Values"]
+        if (not numeric) or (num_uniq <= 10):
 
-            if not numeric:
-                # Standard Box Plot with X-axis ordered by median value in each category
-                xaxis_order = data_df_col_notnull.groupby(
-                    by=[column]).median().sort_values(by=[target_col]).index.tolist()
-
-                start1 = time.time()
-                sns.boxplot(data_df_col_notnull, x=column, y=target_col, order=xaxis_order, **box_params)
-                time1 += (time.time() - start1)
+            if num_uniq > 20:
+                orig_len = len(data_df_col_notnull)
+                value_counts_index = data_df_col_notnull[column].value_counts().index[0:20]
+                data_df_col_notnull = data_df_col_notnull.loc[data_df_col_notnull[column].isin(value_counts_index)]
+                print("For '{}', more than 20 unique values: Only plotting top 20, which is {} out of {} total data"
+                      "points.".format(column, len(data_df_col_notnull), orig_len))
+                anc = AnchoredText('Plotting top 20 out of {} total uniq vals'.format(num_uniq), loc="upper left",
+                                   frameon=False)
+                ax.add_artist(anc)
+            
+            if target_type == 'regression':
+                if not numeric:
+                    # Standard Box Plot with X-axis ordered by median value in each category
+                    xaxis_order = data_df_col_notnull.groupby(
+                        by=[column]).median().sort_values(by=[target_col]).index.tolist()
+
+                    sns.boxplot(data_df_col_notnull, x=column, y=target_col, order=xaxis_order, **box_params)
+
+                else:
+                    # Standard Box Plot
+                    sns.boxplot(data_df_col_notnull, x=column, y=target_col, **box_params)  # hue="method", palette="vlag"
+
+                # Add in points to show each observation
+                if (catplot_style != 'scatterdense') and (len(data_df_col_notnull) > 1000):
+                    data_df_col_notnull = data_df_col_notnull.sample(n=1000, replace=False)
+
+                if catplot_style == 'swarm':
+                    sns.swarmplot(data_df_col_notnull, x=column, y=target_col, size=2, color=".3", warn_thresh=0.4)
+
+                elif catplot_style == 'strip':
+                    sns.stripplot(data_df_col_notnull, x=column, y=target_col, jitter=0.25, size=2, color=".3")
+
+                elif catplot_style == 'scatterdense':
+                    x_all, y_all = np.array([]), np.array([])
+
+                    for cat in ax.get_xticklabels():
+                        # print(cat, cat.get_text(), cat.get_position(), cat.get_position()[0])
+
+                        try:
+                            data_df_cat = data_df_col_notnull.loc[
+                                (data_df_col_notnull[column] == cat.get_text()) | (data_df_col_notnull[column] == float(cat.get_text()))]
+                        except ValueError:
+                            data_df_cat = data_df_col_notnull.loc[data_df_col_notnull[column] == cat.get_text()]
+                        # print(len(data_df_cat))
+
+                        x = (np.zeros(len(data_df_cat)) + cat.get_position()[0] +
+                            np.random.normal(scale=0.06, size=len(data_df_cat)))  # 0.005
+                        y = data_df_cat[target_col].values
+                        x_all, y_all = np.append(x_all, x), np.append(y_all, y)
 
+                    ax = plot_scatter_density(x_all, y_all, fig=f, ax=ax, bins=100, s=3, cmap='viridis')
+                
             else:
-                # Standard Box Plot
-                sns.boxplot(data_df_col_notnull, x=column, y=target_col, **box_params)  # hue="method", palette="vlag"
-
-            # Add in points to show each observation
-            start2 = time.time()
-            if (catplot_style != 'scatterdense') and (len(data_df_col_notnull) > 1000):
-                data_df_col_notnull = data_df_col_notnull.sample(n=1000, replace=False)
+                sns.histplot(data_df_col_notnull, x=column, hue=target_col, discrete=True, shrink=0.6, multiple="dodge")  # "stack"
+                ax.set_xticks(data_df_col_notnull[column].unique())
 
-            if catplot_style == 'swarm':
-                sns.swarmplot(data_df_col_notnull, x=column, y=target_col, size=2, color=".3", warn_thresh=0.4)
-
-            elif catplot_style == 'strip':
-                sns.stripplot(data_df_col_notnull, x=column, y=target_col, jitter=0.25, size=2, color=".3")
-
-            elif catplot_style == 'scatterdense':
-                x_all, y_all = np.array([]), np.array([])
-
-                for cat in ax.get_xticklabels():
-                    # print(cat, cat.get_text(), cat.get_position(), cat.get_position()[0])
-
-                    try:
-                        data_df_cat = data_df_col_notnull.loc[
-                            (data_df_col_notnull[column] == cat.get_text()) | (data_df_col_notnull[column] == float(cat.get_text()))]
-                    except ValueError:
-                        data_df_cat = data_df_col_notnull.loc[data_df_col_notnull[column] == cat.get_text()]
-                    # print(len(data_df_cat))
-
-                    x = (np.zeros(len(data_df_cat)) + cat.get_position()[0] +
-                         np.random.normal(scale=0.06, size=len(data_df_cat)))  # 0.005
-                    y = data_df_cat[target_col].values
-                    x_all, y_all = np.append(x_all, x), np.append(y_all, y)
-
-                ax = plot_scatter_density(x_all, y_all, fig=f, ax=ax, bins=100, s=3, cmap='viridis')
-
-            time2 += (time.time() - start2)
-
-            if (not numeric) and data_df_col_notnull[column].nunique() >= 10:
+            if (not numeric) and num_uniq >= 10:
                 plt.xticks(rotation=45)
+                plt.grid(axis='x')
 
             plt.grid(axis='y')
 
         else:
 
             med = data_df_col_notnull[column].median()
             std = data_df_col_notnull[column].std()
@@ -235,48 +262,73 @@
 
             if xx.size > 0:
                 data_df_col_notnull = data_df_col_notnull.drop(xx)
 
                 anc = AnchoredText('Not Shown: {} Outliers'.format(xx.size), loc="upper left", frameon=False)
                 ax.add_artist(anc)
 
-            # sns.scatterplot(train_data_mod, x=column, y=target_col, hue="OverallQual")
-            # sns.scatterplot(data_df, x=column, y=target_col, size=2, legend=False)
+            if target_type == 'regression':
+                # sns.scatterplot(train_data_mod, x=column, y=target_col, hue="OverallQual")
+                # sns.scatterplot(data_df, x=column, y=target_col, size=2, legend=False)
+
+                ax = plot_scatter_density(data_df_col_notnull[column].values, data_df_col_notnull[target_col].values,
+                                        fig=f, ax=ax, bins=100, s=3, cmap='viridis')
+
+                # plt.hist2d(data_df_col_notnull[column], data_df_col_notnull[target_col], bins=(100, 100),
+                #            cmap='viridis', cmin=1)  # BuPu
+                # plt.colorbar()
+
+                # ax.scatter(x, y, c=z, s=100, edgecolor='')
+                # ax.scatter(x, y, c=z, s=50)
+            
+            else:
+                sns.boxplot(data_df_col_notnull, x=column, y=target_col, orient='y', **box_params)
+
+                x_all, y_all = np.array([]), np.array([])
+
+                for cat in ax.get_yticklabels():
+                    # print(cat, cat.get_text(), cat.get_position(), cat.get_position()[0])
 
-            ax = plot_scatter_density(data_df_col_notnull[column].values, data_df_col_notnull[target_col].values,
-                                      fig=f, ax=ax, bins=100, s=3, cmap='viridis')
+                    try:
+                        data_df_cat = data_df_col_notnull.loc[
+                            (data_df_col_notnull[target_col] == cat.get_text()) | (
+                                        data_df_col_notnull[target_col] == float(cat.get_text()))]
+                    except ValueError:
+                        data_df_cat = data_df_col_notnull.loc[data_df_col_notnull[target_col] == cat.get_text()]
+                    # print(len(data_df_cat))
 
-            # plt.hist2d(data_df_col_notnull[column], data_df_col_notnull[target_col], bins=(100, 100),
-            #            cmap='viridis', cmin=1)  # BuPu
-            # plt.colorbar()
+                    y = (np.zeros(len(data_df_cat)) + cat.get_position()[1] +
+                        np.random.normal(scale=0.06, size=len(data_df_cat)))
+                    x = data_df_cat[column].values
+                    x_all, y_all = np.append(x_all, x), np.append(y_all, y)
 
-            # ax.scatter(x, y, c=z, s=100, edgecolor='')
-            # ax.scatter(x, y, c=z, s=50)
+                ax = plot_scatter_density(x_all, y_all, fig=f, ax=ax, bins=100, s=3, cmap='viridis')
 
             plt.grid()
 
             plt.xlabel(column)
             plt.ylabel(target_col)
 
-            # DONE Need to check index for using xx here
-
         if set_ylim:
             plt.ylim(ymin, ymax)
 
         if numeric:
-            ax.set_title('{} vs {} : P={}, MI={}, RF={}'.format(
-                column, target_col, correlation_df.loc[column, "Pearson"],
-                correlation_df.loc[column, "Mutual Info"], correlation_df.loc[column, "Random Forest"]))
+            if target_type == 'regression':
+                ax.set_title('{} vs {} : P={}, MI={}, RF={}'.format(
+                    column, target_col, correlation_df.loc[column, "Pearson"],
+                    correlation_df.loc[column, "Mutual Info"], correlation_df.loc[column, "Random Forest"]))
+            else:
+                ax.set_title('{} vs {} : MI={}, RF={}'.format(
+                    column, target_col, correlation_df.loc[column, "Mutual Info"],
+                    correlation_df.loc[column, "Random Forest"]))
         else:
-            ax.set_title('{} vs {} : RF={}, RF_norm={}'.format(
-                column, target_col, correlation_df.loc[column, "Random Forest"],
-                correlation_df.loc[column, "RF_norm"]))
+            ax.set_title('{} vs {} : MI={}, RF={}, RF_norm={}'.format(
+                column, target_col, correlation_df.loc[column, "Mutual Info"],
+                correlation_df.loc[column, "Random Forest"], correlation_df.loc[column, "RF_norm"]))
 
         plt.savefig('{}/{}_vs_{}.png'.format(plots_folder, column, target_col), bbox_inches='tight')
 
         plt.close()
 
     # mpl.use(backend_)  # Reset backend
     # print('*** {} ***'.format(mpl.get_backend()))
 
-    # print(time.time() - start, time1, time2)
-
```

