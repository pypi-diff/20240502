# Comparing `tmp/powershap-0.0.8rc2.tar.gz` & `tmp/powershap-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powershap-0.0.8rc2.tar", max compression
+gzip compressed data, was "powershap-0.0.9.tar", max compression
```

## Comparing `powershap-0.0.8rc2.tar` & `powershap-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1142 2022-05-31 13:08:11.960840 powershap-0.0.8rc2/LICENSE
--rw-r--r--   0        0        0     1695 2022-05-31 13:08:11.960840 powershap-0.0.8rc2/LICENSE.txt
--rw-r--r--   0        0        0     5541 2022-06-30 09:58:52.956037 powershap-0.0.8rc2/README.md
--rw-r--r--   0        0        0      143 2022-07-09 06:57:13.874965 powershap-0.0.8rc2/powershap/__init__.py
--rw-r--r--   0        0        0    22775 2022-07-09 06:56:50.626765 powershap-0.0.8rc2/powershap/powershap.py
--rw-r--r--   0        0        0       56 2022-03-30 18:10:04.342631 powershap-0.0.8rc2/powershap/shap_wrappers/__init__.py
--rw-r--r--   0        0        0    12258 2022-06-18 16:44:59.436115 powershap-0.0.8rc2/powershap/shap_wrappers/shap_explainer.py
--rw-r--r--   0        0        0     1259 2022-07-09 06:57:13.878965 powershap-0.0.8rc2/powershap/shap_wrappers/shap_explainer_factory.py
--rw-r--r--   0        0        0     3123 2022-04-06 09:49:45.846484 powershap-0.0.8rc2/powershap/utils.py
--rw-r--r--   0        0        0      723 2022-07-20 08:39:50.307418 powershap-0.0.8rc2/pyproject.toml
--rw-r--r--   0        0        0     6481 2022-07-20 08:40:03.338548 powershap-0.0.8rc2/setup.py
--rw-r--r--   0        0        0     6402 2022-07-20 08:40:03.339586 powershap-0.0.8rc2/PKG-INFO
+-rw-r--r--   0        0        0     1142 2022-11-29 10:21:13.082294 powershap-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1695 2022-11-29 10:21:13.082294 powershap-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     5391 2023-01-12 09:58:56.830199 powershap-0.0.9/README.md
+-rw-r--r--   0        0        0      166 2023-01-12 15:55:50.233316 powershap-0.0.9/powershap/__init__.py
+-rw-r--r--   0        0        0    22387 2023-01-12 15:52:11.875451 powershap-0.0.9/powershap/powershap.py
+-rw-r--r--   0        0        0       93 2023-01-12 15:52:11.875451 powershap-0.0.9/powershap/shap_wrappers/__init__.py
+-rw-r--r--   0        0        0    12964 2023-01-12 15:52:11.875451 powershap-0.0.9/powershap/shap_wrappers/shap_explainer.py
+-rw-r--r--   0        0        0     1295 2023-01-12 15:52:11.875451 powershap-0.0.9/powershap/shap_wrappers/shap_explainer_factory.py
+-rw-r--r--   0        0        0     3002 2023-01-12 15:52:11.875451 powershap-0.0.9/powershap/utils.py
+-rw-r--r--   0        0        0     1284 2023-01-12 15:56:09.908769 powershap-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6336 1970-01-01 00:00:00.000000 powershap-0.0.9/setup.py
+-rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 powershap-0.0.9/PKG-INFO
```

### Comparing `powershap-0.0.8rc2/LICENSE` & `powershap-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `powershap-0.0.8rc2/LICENSE.txt` & `powershap-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `powershap-0.0.8rc2/README.md` & `powershap-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,29 @@
         <img alt="PowerShap logo" src="https://raw.githubusercontent.com/predict-idlab/powershap/main/powershap_full_scaled.png" width=70%>
     </a>
 </p>
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/powershap.svg)](https://pypi.org/project/powershap/)
 [![support-version](https://img.shields.io/pypi/pyversions/powershap)](https://img.shields.io/pypi/pyversions/powershap)
 [![codecov](https://img.shields.io/codecov/c/github/predict-idlab/powershap?logo=codecov)](https://codecov.io/gh/predict-idlab/powershap)
-[![Code quality](https://img.shields.io/lgtm/grade/python/github/predict-idlab/powershap?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-idlab/powershap/context:python)
 [![Downloads](https://pepy.tech/badge/powershap)](https://pepy.tech/project/powershap)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)
 [![Testing](https://github.com/predict-idlab/powershap/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/powershap/actions/workflows/test.yml)
 [![DOI](https://zenodo.org/badge/470633431.svg)](https://zenodo.org/badge/latestdoi/470633431)
 
 > *powershap* is a **feature selection method** that uses statistical hypothesis testing and power calculations on **Shapley values**, enabling fast and intuitive wrapper-based feature selection.  
 
 ## Installation ⚙️
 
 | [**pip**](https://pypi.org/project/powershap/) | `pip install powershap` | 
 | ---| ----|
 
 ## Usage 🛠
 
-*powershap* is built to be intuitive, it supports various models including linear, tree-based, and even deep learning models.  
+*powershap* is built to be intuitive, it supports various models including linear, tree-based, and even deep learning models for classification and regression tasks.  
 <!-- It is also implented as sklearn `Transformer` component, allowing convenient integration in `sklearn` pipelines. -->
 
 ```py
 from powershap import PowerShap
 from catboost import CatBoostClassifier
 
 X, y = ...  # your classification dataset
```

#### html2text {}

```diff
@@ -1,70 +1,67 @@
                                _[_P_o_w_e_r_S_h_a_p_ _l_o_g_o_]
 [![PyPI Latest Release](https://img.shields.io/pypi/v/powershap.svg)](https://
 pypi.org/project/powershap/) [![support-version](https://img.shields.io/pypi/
 pyversions/powershap)](https://img.shields.io/pypi/pyversions/powershap) [!
 [codecov](https://img.shields.io/codecov/c/github/predict-idlab/
-powershap?logo=codecov)](https://codecov.io/gh/predict-idlab/powershap) [![Code
-quality](https://img.shields.io/lgtm/grade/python/github/predict-idlab/
-powershap?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-
-idlab/powershap/context:python) [![Downloads](https://pepy.tech/badge/
-powershap)](https://pepy.tech/project/powershap) [![PRs Welcome](https://
-img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
-makeapullrequest.com) [![Testing](https://github.com/predict-idlab/powershap/
-actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/
-powershap/actions/workflows/test.yml) [![DOI](https://zenodo.org/badge/
-470633431.svg)](https://zenodo.org/badge/latestdoi/470633431) > *powershap* is
-a **feature selection method** that uses statistical hypothesis testing and
-power calculations on **Shapley values**, enabling fast and intuitive wrapper-
-based feature selection. ## Installation âï¸ | [**pip**](https://pypi.org/
-project/powershap/) | `pip install powershap` | | ---| ----| ## Usage ð 
-*powershap* is built to be intuitive, it supports various models including
-linear, tree-based, and even deep learning models. ```py from powershap import
-PowerShap from catboost import CatBoostClassifier X, y = ... # your
-classification dataset selector = PowerShap( model=CatBoostClassifier
-(n_estimators=250, verbose=0, use_best_model=True) ) selector.fit(X, y) # Fit
-the PowerShap feature selector selector.transform(X) # Reduce the dataset to
-the selected features ``` ## Features â¨ * default automatic mode * `scikit-
-learn` compatible * supports various models * insights into the feature
-selection method: call the `._processed_shaps_df` on a fitted `PowerSHAP`
-feature selector. * tested code! ## Benchmarks â± Check out our benchmark
-results [here](examples/results/). ## How does it work âï¸ Powershap is
-built on the core assumption that *an informative feature will have a larger
-impact on the prediction compared to a known random feature.* * Powershap
-trains multiple models with different random seeds on different subsets of the
-data. Each iteration it adds a random uniform feature to the dataset for
-training. * In a single iteration after training a model, powershap calculates
-the absolute Shapley values of all features, including the random feature. If
-there are multiple outputs or multiple classes, powershap uses the maximum
-across these multiple outputs. These values are then averaged for each feature,
-symbolising the impact of the feature in this iteration. * After performing all
-iterations, each feature then has an array of impacts. The impact array of each
-feature is then compared to the average of the random feature impact array
-using the percentile formula to provide a p-value. This tests whether the
-feature has a larger impact than the random feature and outputs a low p-value
-if true. * Powershap then outputs all features with a p-value below the
-provided threshold. The threshold is by default 0.01. ### Automatic mode ð¤
-The required number of iterations and the threshold values are hyperparameters
-of powershap. However, to *avoid manually optimizing the hyperparameters*
-powershap by default uses an automatic mode that automatically determines these
-hyperparameters. * The automatic mode first starts with executing powershap
-using ten iterations. * Then, for each feature powershap calculates the effect
-size and the statistical power of the test using a student-t power test. *
-Using the calculated effect size, powershap then calculates the required
-iterations to achieve a predefined power requirement. By default this is 0.99,
-which represents a false positive probability of 0.01. * If the required
-iterations are larger than the already performed iterations, powershap then
-further executes for the extra required iterations. * Afterward, powershap re-
-calculates the required iterations and it keeps re-executing until the required
-iterations are met. ## Referencing our package :memo: If you use *powershap* in
-a scientific publication, we would highly appreciate citing us as: ```bibtex
-@misc{https://doi.org/10.48550/arxiv.2206.08394, doi = {10.48550/
-ARXIV.2206.08394}, url = {https://arxiv.org/abs/2206.08394}, author =
-{Verhaeghe, Jarne and Van Der Donckt, Jeroen and Ongenae, Femke and Van Hoecke,
-Sofie}, keywords = {Machine Learning (cs.LG), Machine Learning (stat.ML), FOS:
-Computer and information sciences, FOS: Computer and information sciences},
-title = {Powershap: A Power-full Shapley Feature Selection Method}, publisher =
-{arXiv}, year = {2022} copyright = {arXiv.org perpetual, non-exclusive license}
-} ``` Paper is accepted at ECML PKDD 2022 and will be presented there. The
-preprint can be found on arXiv ([link](https://arxiv.org/abs/2206.08394)) and
-on the github. ---
+powershap?logo=codecov)](https://codecov.io/gh/predict-idlab/powershap) [!
+[Downloads](https://pepy.tech/badge/powershap)](https://pepy.tech/project/
+powershap) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-
+brightgreen.svg?)](http://makeapullrequest.com) [![Testing](https://github.com/
+predict-idlab/powershap/actions/workflows/test.yml/badge.svg)](https://
+github.com/predict-idlab/powershap/actions/workflows/test.yml) [![DOI](https://
+zenodo.org/badge/470633431.svg)](https://zenodo.org/badge/latestdoi/470633431)
+> *powershap* is a **feature selection method** that uses statistical
+hypothesis testing and power calculations on **Shapley values**, enabling fast
+and intuitive wrapper-based feature selection. ## Installation âï¸ |
+[**pip**](https://pypi.org/project/powershap/) | `pip install powershap` | | --
+-| ----| ## Usage ð  *powershap* is built to be intuitive, it supports
+various models including linear, tree-based, and even deep learning models for
+classification and regression tasks. ```py from powershap import PowerShap from
+catboost import CatBoostClassifier X, y = ... # your classification dataset
+selector = PowerShap( model=CatBoostClassifier(n_estimators=250, verbose=0,
+use_best_model=True) ) selector.fit(X, y) # Fit the PowerShap feature selector
+selector.transform(X) # Reduce the dataset to the selected features ``` ##
+Features â¨ * default automatic mode * `scikit-learn` compatible * supports
+various models * insights into the feature selection method: call the
+`._processed_shaps_df` on a fitted `PowerSHAP` feature selector. * tested code!
+## Benchmarks â± Check out our benchmark results [here](examples/results/). ##
+How does it work âï¸ Powershap is built on the core assumption that *an
+informative feature will have a larger impact on the prediction compared to a
+known random feature.* * Powershap trains multiple models with different random
+seeds on different subsets of the data. Each iteration it adds a random uniform
+feature to the dataset for training. * In a single iteration after training a
+model, powershap calculates the absolute Shapley values of all features,
+including the random feature. If there are multiple outputs or multiple
+classes, powershap uses the maximum across these multiple outputs. These values
+are then averaged for each feature, symbolising the impact of the feature in
+this iteration. * After performing all iterations, each feature then has an
+array of impacts. The impact array of each feature is then compared to the
+average of the random feature impact array using the percentile formula to
+provide a p-value. This tests whether the feature has a larger impact than the
+random feature and outputs a low p-value if true. * Powershap then outputs all
+features with a p-value below the provided threshold. The threshold is by
+default 0.01. ### Automatic mode ð¤ The required number of iterations and the
+threshold values are hyperparameters of powershap. However, to *avoid manually
+optimizing the hyperparameters* powershap by default uses an automatic mode
+that automatically determines these hyperparameters. * The automatic mode first
+starts with executing powershap using ten iterations. * Then, for each feature
+powershap calculates the effect size and the statistical power of the test
+using a student-t power test. * Using the calculated effect size, powershap
+then calculates the required iterations to achieve a predefined power
+requirement. By default this is 0.99, which represents a false positive
+probability of 0.01. * If the required iterations are larger than the already
+performed iterations, powershap then further executes for the extra required
+iterations. * Afterward, powershap re-calculates the required iterations and it
+keeps re-executing until the required iterations are met. ## Referencing our
+package :memo: If you use *powershap* in a scientific publication, we would
+highly appreciate citing us as: ```bibtex @misc{https://doi.org/10.48550/
+arxiv.2206.08394, doi = {10.48550/ARXIV.2206.08394}, url = {https://arxiv.org/
+abs/2206.08394}, author = {Verhaeghe, Jarne and Van Der Donckt, Jeroen and
+Ongenae, Femke and Van Hoecke, Sofie}, keywords = {Machine Learning (cs.LG),
+Machine Learning (stat.ML), FOS: Computer and information sciences, FOS:
+Computer and information sciences}, title = {Powershap: A Power-full Shapley
+Feature Selection Method}, publisher = {arXiv}, year = {2022} copyright =
+{arXiv.org perpetual, non-exclusive license} } ``` Paper is accepted at ECML
+PKDD 2022 and will be presented there. The preprint can be found on arXiv (
+[link](https://arxiv.org/abs/2206.08394)) and on the github. ---
                   ð¤ Jarne Verhaeghe, Jeroen Van Der Donckt
```

### Comparing `powershap-0.0.8rc2/powershap/powershap.py` & `powershap-0.0.9/powershap/powershap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 __author__ = "Jarne Verhaeghe, Jeroen Van Der Donckt"
 
 import warnings
-import sklearn
+
 import numpy as np
 import pandas as pd
-
+import sklearn
 from sklearn.base import BaseEstimator
 from sklearn.feature_selection import SelectorMixin
-from sklearn.utils.validation import check_is_fitted
 from sklearn.model_selection import BaseCrossValidator
+from sklearn.utils.validation import check_is_fitted
 
 from .shap_wrappers import ShapExplainerFactory
-
 from .utils import powerSHAP_statistical_analysis
 
 
 class PowerShap(SelectorMixin, BaseEstimator):
     """
     Feature selection based on significance of shap values.
 
@@ -79,17 +78,17 @@
             `power_iterations`. By default False.
         force_convergence: bool, optional
             Only used for automatic mode. If True, powershap will continue delete
             the found relevant features and rerun until no more relevant features are found.
             This is especially useful in high-dimensional datasets
         limit_convergence_its: int, optional
             The number of maximum allowed recursions when `force_convergence` is True. By
-            default 0, meaning that no limit is applied. A limit_convergence_its of 1 suggests 
-            only executing one convergence recursion 
-            after a single full automatic PowerShap execution. 
+            default 0, meaning that no limit is applied. A limit_convergence_its of 1 suggests
+            only executing one convergence recursion
+            after a single full automatic PowerShap execution.
         limit_automatic: int, optional
             The number of maximum allowed iterations when `automatic` is True. By
             default None, meaning that no limit is applied.
         limit_incremental_iterations: int, optional
             If the required iterations exceed `limit_automatic` in automatic mode, add
             `limit_incremental_iterations` iterations and re-evaluate. By default 10.
         limit_recursive_automatic: int, optional
@@ -143,17 +142,19 @@
         self.fit_kwargs = fit_kwargs
 
         def _infinite_splitter(cv):
             """Infinite yields for the given splitter.
             If the splitter is exhausted, it will be reset and restarted.
             """
             from copy import deepcopy
+
             cv = deepcopy(cv)
-            splitter = None 
+            splitter = None
             random_state = 0
+
             def split(X, y=None, groups=None):
                 nonlocal splitter, random_state
                 if splitter is None:
                     if hasattr(cv, "random_state"):  # Update random state
                         cv.__setattr__("random_state", random_state)
                         random_state += 1
                     splitter = cv.split(X, y=y, groups=groups)
@@ -162,16 +163,17 @@
                         yield next(splitter)
                     except StopIteration:
                         if hasattr(cv, "random_state"):  # Update random state
                             cv.__setattr__("random_state", random_state)
                             random_state += 1
                         splitter = cv.split(X, y=y, groups=groups)
                         yield next(splitter)
+
             return split
-     
+
         if cv is not None:
             self.cv = _infinite_splitter(cv)
         else:
             self.cv = None
 
         if model is not None:
             self._explainer = ShapExplainerFactory.get_explainer(model=model)
@@ -180,42 +182,34 @@
     def _get_default_model(y: np.ndarray):
         from catboost import CatBoostClassifier, CatBoostRegressor
 
         assert isinstance(y, np.ndarray)
         dtype = y.dtype
         if np.issubdtype(dtype, np.number) and not np.issubdtype(dtype, np.integer):
             return CatBoostRegressor(
-                n_estimators=250,
-                od_type="Iter",
-                od_wait=25,
-                use_best_model=True,
-                verbose=0,
+                n_estimators=250, od_type="Iter", od_wait=25, use_best_model=True, verbose=0
             )
         if np.issubdtype(dtype, np.integer) and len(np.unique(y.ravel())) >= 5:
             warnings.warn(
-                "Classifying although there are >= 5 integers in the labels.",
-                UserWarning,
+                "Classifying although there are >= 5 integers in the labels.", UserWarning
             )
         return CatBoostClassifier(
             n_estimators=250, od_type="Iter", od_wait=25, use_best_model=True, verbose=0
         )
 
     def _log_feature_names_sklean_v0(self, X):
         """Log the feature names if we have sklearn 0.x"""
         assert sklearn.__version__.startswith("0.")
         feature_names = np.asarray(X.columns) if hasattr(X, "columns") else None
         if feature_names is not None and len(feature_names) > 0:
             # Check if all feature names of type string
             types = sorted(t.__qualname__ for t in set(type(v) for v in feature_names))
             if len(types) > 1 or types[0] != "str":
                 feature_names = None
-                warnings.warn(
-                    "Feature names only support names that are all strings.",
-                    UserWarning,
-                )
+                warnings.warn("Feature names only support names that are all strings.", UserWarning)
 
         if feature_names is not None and len(feature_names) > 0:
             self.feature_names_in_ = feature_names
         elif hasattr(self, "feature_names_in_"):
             # Delete the attribute when the estimator is fitted on a new dataset that
             # has no feature names.
             delattr(self, "feature_names_in_")
@@ -278,17 +272,15 @@
                     groups=groups,
                     cv_split=self.cv,  # pass the wrapped cv split function
                     random_seed_start=max_iterations_old,
                     show_progress=self.show_progress,
                     **kwargs,
                 )
 
-                max_iterations_old = (
-                    max_iterations_old + self.limit_incremental_iterations
-                )
+                max_iterations_old = max_iterations_old + self.limit_incremental_iterations
 
             else:
                 self._print(
                     f"Automatic mode: Powershap requires {max_iterations} "
                     f"iterations; Adding {max_iterations-max_iterations_old} ",
                     "powershap iterations.",
                 )
@@ -307,18 +299,15 @@
                 )
 
                 max_iterations_old = max_iterations
 
             shaps_df = pd.concat([shaps_df, shaps_df_recursive])
 
             processed_shaps_df = powerSHAP_statistical_analysis(
-                shaps_df,
-                self.power_alpha,
-                self.power_req_iterations,
-                include_all=self.include_all,
+                shaps_df, self.power_alpha, self.power_req_iterations, include_all=self.include_all
             )
 
             if not any(processed_shaps_df.p_value < self.power_alpha):
                 # There is no feature found yet...
                 self._print("No features selected after 10 automatic iterations!")
                 # Return already as more iterations will only result in including less
                 # features
@@ -355,32 +344,30 @@
             Group labels for the samples used while splitting the dataset into
             train/test set. By default None.
 
         """
         if stratify is None and self.stratify:
             # Set stratify to y, if no stratify is given and self.stratify is True
             stratify = y
-        
+
         # kwargs take precedence over fit_kwargs
         kwargs = {**self.fit_kwargs, **kwargs}
 
         if self.model is None:
             # If no model is passed to the constructor -> select the default catboost
             # model
             self.model = PowerShap._get_default_model(np.asarray(y))
             self._explainer = ShapExplainerFactory.get_explainer(self.model)
 
         if sklearn.__version__.startswith("0."):
             # Log the feature names if we have sklearn 0.x
             self._log_feature_names_sklean_v0(X)
         # Perform the necessary sklearn checks -> X and y are both ndarray
         # Logs the feature names as well (in self.feature_names_in_ in sklearn 1.x)
-        X, y = self._explainer._validate_data(
-            self._validate_data, X, y, multi_output=True
-        )
+        X, y = self._explainer._validate_data(self._validate_data, X, y, multi_output=True)
 
         self._print("Starting powershap")
 
         X = pd.DataFrame(data=X, columns=list(range(X.shape[1])))
 
         loop_its = self.power_iterations
         if self.automatic:
@@ -399,18 +386,15 @@
             groups=groups,
             cv_split=self.cv,  # pass the wrapped cv split function
             show_progress=self.show_progress,
             **kwargs,
         )
 
         processed_shaps_df = powerSHAP_statistical_analysis(
-            shaps_df,
-            self.power_alpha,
-            self.power_req_iterations,
-            include_all=self.include_all,
+            shaps_df, self.power_alpha, self.power_req_iterations, include_all=self.include_all
         )
 
         if self.automatic:
 
             processed_shaps_df = self._automatic_fit(
                 X=X,
                 y=y,
@@ -428,28 +412,30 @@
 
                 converge_df = processed_shaps_df.copy()
 
                 significant_cols = np.array(
                     converge_df[converge_df.p_value < self.power_alpha].index.values
                 )
 
-                # If limit_convergence_its is zero, the convergence mode does not have a limit. If not, the 
-                # While loop condition is recalculated every while loop iteration.
+                # If limit_convergence_its is zero, the convergence mode does not have a limit.
+                # If not, the while loop condition is recalculated every while loop iteration.
                 if self.limit_convergence_its > 0:
                     current_converge_recursions = 0
-                    while_convergence_bool = current_converge_recursions < self.limit_convergence_its
+                    while_convergence_bool = (
+                        current_converge_recursions < self.limit_convergence_its
+                    )
                 else:
                     while_convergence_bool = True
 
-                while((len(converge_df[converge_df.p_value < self.power_alpha]) > 0) & (while_convergence_bool)):
+                while (len(converge_df[converge_df.p_value < self.power_alpha]) > 0) & (
+                    while_convergence_bool
+                ):
                     self._print("Rerunning powershap for convergence. ")
                     converge_shaps_df = self._explainer.explain(
-                        X=X.drop(
-                            columns=X.columns.values[significant_cols.astype(np.int32)]
-                        ),
+                        X=X.drop(columns=X.columns.values[significant_cols.astype(np.int32)]),
                         y=y,
                         loop_its=loop_its,
                         val_size=self.val_size,
                         stratify=stratify,
                         groups=groups,
                         cv_split=self.cv,  # pass the wrapped cv split function
                         show_progress=self.show_progress,
@@ -460,58 +446,51 @@
                         converge_shaps_df,
                         self.power_alpha,
                         self.power_req_iterations,
                         include_all=self.include_all,
                     )
 
                     converge_df = self._automatic_fit(
-                        X=X.drop(
-                            columns=X.columns.values[significant_cols.astype(np.int32)]
-                        ),
+                        X=X.drop(columns=X.columns.values[significant_cols.astype(np.int32)]),
                         y=y,
                         processed_shaps_df=converge_df,
                         loop_its=loop_its,
                         stratify=stratify,
                         groups=groups,
                         converge_shaps_df=converge_shaps_df,
                         shaps_df=converge_shaps_df,
                         **kwargs,
                     )
 
                     significant_cols = np.append(
                         significant_cols,
-                        converge_df[
-                            converge_df.p_value < self.power_alpha
-                        ].index.values,
+                        converge_df[converge_df.p_value < self.power_alpha].index.values,
                     )
 
                     processed_shaps_df.loc[
                         converge_df[converge_df.p_value < self.power_alpha].index.values
                     ] = converge_df[converge_df.p_value < self.power_alpha]
 
-                    
                     if self.limit_convergence_its > 0:
                         current_converge_recursions += 1
                         print(current_converge_recursions)
-                        while_convergence_bool = current_converge_recursions < self.limit_convergence_its
+                        while_convergence_bool = (
+                            current_converge_recursions < self.limit_convergence_its
+                        )
 
                         if not while_convergence_bool:
                             self._print("Convergence limit reached: Stopping convergence mode.")
 
-
                 processed_shaps_df.loc[converge_df.index.values] = converge_df
 
-
         self._print("Done!")
 
         ## Set the p-values property (used in the transform function)
         # Remove the random feature (legit features have int index)
-        sub_df = processed_shaps_df[
-            processed_shaps_df.index.map(lambda x: isinstance(x, int))
-        ]
+        sub_df = processed_shaps_df[processed_shaps_df.index.map(lambda x: isinstance(x, int))]
         # Sort to have original order again
         sub_df = sub_df.sort_index()
         self._p_values = sub_df.p_value.values
 
         ## Store the processed_shaps_df in the object
         self._processed_shaps_df = processed_shaps_df
         if hasattr(self, "feature_names_in_"):
@@ -530,14 +509,13 @@
         return self._p_values < self.power_alpha
 
     def transform(self, X):
         check_is_fitted(self, ["_processed_shaps_df", "_p_values", "_explainer"])
         if hasattr(self, "feature_names_in_") and isinstance(X, pd.DataFrame):
             assert np.all(X.columns.values == self.feature_names_in_)
             return pd.DataFrame(
-                super().transform(X),
-                columns=self.feature_names_in_[self._get_support_mask()],
+                super().transform(X), columns=self.feature_names_in_[self._get_support_mask()]
             )
         return super().transform(X)
 
     def _more_tags(self):
         return self._explainer._get_more_tags()
```

### Comparing `powershap-0.0.8rc2/powershap/shap_wrappers/shap_explainer.py` & `powershap-0.0.9/powershap/shap_wrappers/shap_explainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 __author__ = "Jarne Verhaeghe, Jeroen Van Der Donckt"
 
 import warnings
-import shap
-import pandas as pd
-import numpy as np
+from abc import ABC
+from copy import copy
+from typing import Any, Callable
 
-from tqdm.auto import tqdm
+import numpy as np
+import pandas as pd
+import shap
 from numpy.random import RandomState
 from sklearn.model_selection import train_test_split
-from abc import ABC
-
-from typing import Any, Callable
+from tqdm.auto import tqdm
 
 
 class ShapExplainer(ABC):
     """Interface class for a (POWERshap explainer class."""
 
-    def __init__(
-        self,
-        model: Any,
-    ):
+    def __init__(self, model: Any):
         """Create a POWERshap explainer instance.
 
         Parameters
         ----------
         model: Any
             The  model from which powershap will use its shap values to perform feature
             selection.
 
         """
         assert self.supports_model(model)
         self.model = model
 
     # Should be implemented by subclass
-    def _fit_get_shap(
-        self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs
-    ) -> np.array:
+    def _fit_get_shap(self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs) -> np.array:
         raise NotImplementedError
 
     def _validate_data(self, validate_data: Callable, X, y, **kwargs):
         return validate_data(X, y, **kwargs)
 
     # Should be implemented by subclass
     @staticmethod
@@ -77,16 +72,15 @@
         Parameters
         ----------
         X: pd.DataFrame
             The features.
         y: np.array
             The labels.
         loop_its: int
-            The number of iterations to fit the model with random state and random
-            feature.
+            The number of iterations to fit the model with random state and random feature.
         val_size: float
             The fractional size of the validation set. Should be a float between ]0,1[.
         stratify: np.array, optional
             The array used to create a stratified train_test_split. By default None.
         groups: np.array, optional
             The group labels for the samples used while splitting the dataset into
             train/test set. By default None.
@@ -96,15 +90,15 @@
             infinite amount of splits. The arguments of this function are X, y, groups.
         random_seed_start: int, optional
             The random seed to start the iterations with. By default 0.
         **kwargs: dict
             The keyword arguments for the fit method.
         """
         random_col_name = "random_uniform_feature"
-        assert not random_col_name in X.columns
+        assert random_col_name not in X.columns
 
         X = X.copy(deep=True)
 
         shaps = []  # TODO: pre-allocate for efficiency
 
         cv_splitter = None
         if cv_split is not None:
@@ -123,53 +117,43 @@
             ### A) Split using the wrapped cross-validation splitter
             if cv_splitter is not None:
                 train_idx, val_idx = next(cv_splitter)
             ### B) Perform train-test split when no cross-validation splitter is passed
             elif groups is None:
                 # stratify may be None or not None
                 train_idx, val_idx = train_test_split(
-                    np.arange(len(X)),
-                    test_size=val_size,
-                    random_state=i,
-                    stratify=stratify,
+                    np.arange(len(X)), test_size=val_size, random_state=i, stratify=stratify
                 )
             elif stratify is None:
                 # groups may be None or not None
                 from sklearn.model_selection import GroupShuffleSplit
 
                 train_idx, val_idx = next(
-                    GroupShuffleSplit(
-                        random_state=i,
-                        n_splits=1,
-                        test_size=val_size,
-                    ).split(X, y, groups=groups)
+                    GroupShuffleSplit(random_state=i, n_splits=1, test_size=val_size).split(
+                        X, y, groups=groups
+                    )
                 )
             else:
                 # stratify and groups are both not None
                 try:
                     from sklearn.model_selection import StratifiedGroupKFold
 
                     train_idx, val_idx = next(
                         StratifiedGroupKFold(
-                            shuffle=True,
-                            random_state=i,
-                            n_splits=int(1 / val_size),
+                            shuffle=True, random_state=i, n_splits=int(1 / val_size)
                         ).split(X, y, groups=groups)
                     )
-                except:
+                except Exception:
                     warnings.warn(
                         "Did not find StratifiedGroupKFold in sklearn install, "
                         + "this is only supported in sklearn 1.x.",
                         UserWarning,
                     )
                     train_idx, val_idx = train_test_split(
-                        np.arange(len(X)),
-                        test_size=val_size,
-                        random_state=i,
-                        stratify=stratify,
+                        np.arange(len(X)), test_size=val_size, random_state=i, stratify=stratify
                     )
 
             X_train = X.iloc[np.sort(train_idx)]
             X_val = X.iloc[np.sort(val_idx)]
             Y_train = y[np.sort(train_idx)]
             Y_val = y[np.sort(val_idx)]
 
@@ -196,92 +180,115 @@
 
     def _get_more_tags(self):
         return {}
 
 
 ### CATBOOST
 
-from catboost import CatBoostRegressor, CatBoostClassifier
+from catboost import CatBoostClassifier, CatBoostRegressor
 
 
 class CatboostExplainer(ShapExplainer):
     @staticmethod
     def supports_model(model) -> bool:
         supported_models = [CatBoostRegressor, CatBoostClassifier]
         return isinstance(model, tuple(supported_models))
 
     def _validate_data(self, validate_data: Callable, X, y, **kwargs):
         kwargs["force_all_finite"] = False  # catboost allows NaNs and infs in X
         kwargs["dtype"] = None  # allow non-numeric data
         return super()._validate_data(validate_data, X, y, **kwargs)
 
-    def _fit_get_shap(
-        self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs
-    ) -> np.array:
+    def _fit_get_shap(self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs) -> np.array:
         # Fit the model
         PowerShap_model = self.model.copy().set_params(random_seed=random_seed)
         PowerShap_model.fit(X_train, Y_train, eval_set=(X_val, Y_val))
         # Calculate the shap values
         C_explainer = shap.TreeExplainer(PowerShap_model)
         return C_explainer.shap_values(X_val)
 
     def _get_more_tags(self):
         return {"allow_nan": True}
 
 
+### LGBM
+
+
 class LGBMExplainer(ShapExplainer):
     @staticmethod
     def supports_model(model) -> bool:
         from lightgbm import LGBMClassifier, LGBMRegressor
+
         supported_models = [LGBMClassifier, LGBMRegressor]
         return isinstance(model, tuple(supported_models))
 
     def _validate_data(self, validate_data: Callable, X, y, **kwargs):
         kwargs["force_all_finite"] = False  # lgbm allows NaNs and infs in X
         return super()._validate_data(validate_data, X, y, **kwargs)
 
-    def _fit_get_shap(
-        self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs
-    ) -> np.array:
+    def _fit_get_shap(self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs) -> np.array:
         # Fit the model
-
         # Why we need to use deepcopy and delete LGBM __deepcopy__
         # https://github.com/microsoft/LightGBM/issues/4085
-        from copy import copy
-
         PowerShap_model = copy(self.model).set_params(random_seed=random_seed)
         PowerShap_model.fit(X_train, Y_train, eval_set=(X_val, Y_val))
         # Calculate the shap values
         C_explainer = shap.TreeExplainer(PowerShap_model)
         return C_explainer.shap_values(X_val)
 
     def _get_more_tags(self):
         return {"allow_nan": True}
 
 
+### XGBOOST
+
+
+class XGBoostExplainer(ShapExplainer):
+    @staticmethod
+    def supports_model(model) -> bool:
+        from xgboost import XGBClassifier, XGBRegressor
+
+        supported_models = [XGBClassifier, XGBRegressor]
+        return isinstance(model, tuple(supported_models))
+
+    def _validate_data(self, validate_data: Callable, X, y, **kwargs):
+        kwargs["force_all_finite"] = False  # xgboost allows NaNs and infs in X
+        kwargs["dtype"] = None  # allow non-numeric data
+        return super()._validate_data(validate_data, X, y, **kwargs)
+
+    def _fit_get_shap(self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs) -> np.array:
+        # Fit the model
+        PowerShap_model = copy(self.model).set_params(random_seed=random_seed)
+        PowerShap_model.fit(X_train, Y_train)  # , eval_set=(X_val, Y_val))
+        # Calculate the shap values
+        C_explainer = shap.TreeExplainer(PowerShap_model)
+        return C_explainer.shap_values(X_val)
+
+    def _get_more_tags(self):
+        return {"allow_nan": True}
+
 
 ### RANDOMFOREST
 
 
 class EnsembleExplainer(ShapExplainer):
     @staticmethod
     def supports_model(model) -> bool:
         # TODO: these first 2 require extra checks on the base_estimator
         # from sklearn.ensemble._weight_boosting import BaseWeightBoosting
         # from sklearn.ensemble._bagging import BaseBagging
-        from sklearn.ensemble._forest import ForestRegressor, ForestClassifier
+        from sklearn.ensemble._forest import ForestClassifier, ForestRegressor
         from sklearn.ensemble._gb import BaseGradientBoosting
+
         # from sklearn.ensemble._hist_gradient_boosting import BaseHistGradientBoosting
 
         supported_models = [ForestRegressor, ForestClassifier, BaseGradientBoosting]
         return issubclass(type(model), tuple(supported_models))
 
-    def _fit_get_shap(
-        self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs
-    ) -> np.array:
+    def _fit_get_shap(self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs) -> np.array:
         from sklearn.base import clone
 
         # Fit the model
         PowerShap_model = clone(self.model).set_params(random_state=random_seed)
         PowerShap_model.fit(X_train, Y_train)
         # Calculate the shap values
         C_explainer = shap.TreeExplainer(PowerShap_model)
@@ -296,23 +303,21 @@
     def supports_model(model) -> bool:
         from sklearn.linear_model._base import LinearClassifierMixin, LinearModel
         from sklearn.linear_model._stochastic_gradient import BaseSGD
 
         supported_models = [LinearClassifierMixin, LinearModel, BaseSGD]
         return issubclass(type(model), tuple(supported_models))
 
-    def _fit_get_shap(
-        self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs
-    ) -> np.array:
+    def _fit_get_shap(self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs) -> np.array:
         from sklearn.base import clone
 
         # Fit the model
         try:
             PowerShap_model = clone(self.model).set_params(random_state=random_seed)
-        except:
+        except Exception:
             PowerShap_model = clone(self.model)
         PowerShap_model.fit(X_train, Y_train)
 
         # Calculate the shap values
         C_explainer = shap.explainers.Linear(PowerShap_model, X_train)
         return C_explainer.shap_values(X_val)
 
@@ -326,17 +331,15 @@
         import tensorflow as tf  # ; import torch
 
         # import torch  ## TODO: do we support pytorch??
 
         supported_models = [tf.keras.Model]  # , torch.nn.Module]
         return isinstance(model, tuple(supported_models))
 
-    def _fit_get_shap(
-        self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs
-    ) -> np.array:
+    def _fit_get_shap(self, X_train, Y_train, X_val, Y_val, random_seed, **kwargs) -> np.array:
         import tensorflow as tf
 
         tf.compat.v1.disable_v2_behavior()  # https://github.com/slundberg/shap/issues/2189
 
         # Fit the model
         PowerShap_model = tf.keras.models.clone_model(self.model)
         metrics = kwargs.get("nn_metric")
```

### Comparing `powershap-0.0.8rc2/powershap/shap_wrappers/shap_explainer_factory.py` & `powershap-0.0.9/powershap/shap_wrappers/shap_explainer_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 __author__ = "Jarne Verhaeghe, Jeroen Van Der Donckt"
 
+from typing import Any
+
 from .shap_explainer import (
-    ShapExplainer,
     CatboostExplainer,
-    LGBMExplainer,
+    DeepLearningExplainer,
     EnsembleExplainer,
+    LGBMExplainer,
     LinearExplainer,
-    DeepLearningExplainer,
+    ShapExplainer,
+    XGBoostExplainer,
 )
 
-from typing import Any
-
 
 class ShapExplainerFactory:
     """Factory class for creating the appropriate ShapExplainer."""
 
     _explainer_models = [
         CatboostExplainer,
         LGBMExplainer,
+        XGBoostExplainer,
         EnsembleExplainer,
         LinearExplainer,
         DeepLearningExplainer,
     ]
 
     @classmethod
     def get_explainer(cls, model: Any) -> ShapExplainer:
@@ -38,12 +40,10 @@
             The shap explainer for the given model.
 
         """
         for explainer_class in cls._explainer_models:
             try:  # To avoid errors when the library is not installed
                 if explainer_class.supports_model(model):
                     return explainer_class(model)
-            except:
+            except Exception:
                 pass
-        raise ValueError(
-            f"Given model ({model}) is not yet supported by our explainer models"
-        )
+        raise ValueError(f"Given model ({model}) is not yet supported by our explainer models")
```

### Comparing `powershap-0.0.8rc2/powershap/utils.py` & `powershap-0.0.9/powershap/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 __author__ = "Jarne Verhaeghe"
 
-import pandas as pd
 import numpy as np
-
+import pandas as pd
 from scipy import stats
 from statsmodels.stats.power import TTestPower
 
+
 def p_values_arg_coef(coefficients, arg):
     return stats.percentileofscore(coefficients, arg)
 
 
 def powerSHAP_statistical_analysis(
-    shaps_df: pd.DataFrame,
-    power_alpha: float,
-    power_req_iterations: float,
-    include_all: bool,
+    shaps_df: pd.DataFrame, power_alpha: float, power_req_iterations: float, include_all: bool
 ):
     p_values = []
     effect_size = []
     power_list = []
     required_iterations = []
     n_samples = len(shaps_df["random_uniform_feature"].values)
     mean_random_uniform = shaps_df["random_uniform_feature"].mean()
     for i in range(len(shaps_df.columns)):
-        p_value = (
-            p_values_arg_coef(
-                np.array(shaps_df.values[:, i]), mean_random_uniform)
-            / 100
-        )
+        p_value = p_values_arg_coef(np.array(shaps_df.values[:, i]), mean_random_uniform) / 100
 
         p_values.append(p_value)
 
         if include_all or p_value < power_alpha:
             pooled_standard_deviation = np.sqrt(
                 (
-                    (shaps_df.std().values[i] ** 2) 
+                    (shaps_df.std().values[i] ** 2)
                     + (shaps_df["random_uniform_feature"].values.std() ** 2)
                 )
                 / (2)
             )
             effect_size.append(
-                (mean_random_uniform - shaps_df.mean().values[i])
-                / pooled_standard_deviation
+                (mean_random_uniform - shaps_df.mean().values[i]) / pooled_standard_deviation
             )
             power_list.append(
                 TTestPower().power(
                     effect_size=effect_size[-1],
                     nobs=n_samples,
                     alpha=power_alpha,
                     df=None,
@@ -73,17 +65,15 @@
     processed_shaps_df = pd.DataFrame(
         data=np.hstack(
             [
                 np.reshape(shaps_df.mean().values, (-1, 1)),
                 np.reshape(np.array(p_values), (len(p_values), 1)),
                 np.reshape(np.array(effect_size), (len(effect_size), 1)),
                 np.reshape(np.array(power_list), (len(power_list), 1)),
-                np.reshape(
-                    np.array(required_iterations), (len(required_iterations), 1)
-                ),
+                np.reshape(np.array(required_iterations), (len(required_iterations), 1)),
             ]
         ),
         columns=[
             "impact",
             "p_value",
             "effect_size",
             "power_" + str(power_alpha) + "_alpha",
```

### Comparing `powershap-0.0.8rc2/setup.py` & `powershap-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['catboost>=1.0.5,<2.0.0',
  'numpy>=1.21,<2.0',
  'pandas>=1.3,<2.0',
+ 'scikit-learn',
  'shap>=0.40,<0.41',
- 'sklearn',
  'statsmodels>=0.13.2,<0.14.0']
 
 setup_kwargs = {
     'name': 'powershap',
-    'version': '0.0.8rc2',
+    'version': '0.0.9',
     'description': 'Feature selection using statistical significance of shap values',
-    'long_description': '\t\n<p align="center">\n    <a href="#readme">\n        <img alt="PowerShap logo" src="https://raw.githubusercontent.com/predict-idlab/powershap/main/powershap_full_scaled.png" width=70%>\n    </a>\n</p>\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/powershap.svg)](https://pypi.org/project/powershap/)\n[![support-version](https://img.shields.io/pypi/pyversions/powershap)](https://img.shields.io/pypi/pyversions/powershap)\n[![codecov](https://img.shields.io/codecov/c/github/predict-idlab/powershap?logo=codecov)](https://codecov.io/gh/predict-idlab/powershap)\n[![Code quality](https://img.shields.io/lgtm/grade/python/github/predict-idlab/powershap?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-idlab/powershap/context:python)\n[![Downloads](https://pepy.tech/badge/powershap)](https://pepy.tech/project/powershap)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)\n[![Testing](https://github.com/predict-idlab/powershap/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/powershap/actions/workflows/test.yml)\n[![DOI](https://zenodo.org/badge/470633431.svg)](https://zenodo.org/badge/latestdoi/470633431)\n\n> *powershap* is a **feature selection method** that uses statistical hypothesis testing and power calculations on **Shapley values**, enabling fast and intuitive wrapper-based feature selection.  \n\n## Installation ⚙️\n\n| [**pip**](https://pypi.org/project/powershap/) | `pip install powershap` | \n| ---| ----|\n\n## Usage 🛠\n\n*powershap* is built to be intuitive, it supports various models including linear, tree-based, and even deep learning models.  \n<!-- It is also implented as sklearn `Transformer` component, allowing convenient integration in `sklearn` pipelines. -->\n\n```py\nfrom powershap import PowerShap\nfrom catboost import CatBoostClassifier\n\nX, y = ...  # your classification dataset\n\nselector = PowerShap(\n    model=CatBoostClassifier(n_estimators=250, verbose=0, use_best_model=True)\n)\n\nselector.fit(X, y)  # Fit the PowerShap feature selector\nselector.transform(X)  # Reduce the dataset to the selected features\n\n```\n\n## Features ✨\n\n* default automatic mode\n* `scikit-learn` compatible\n* supports various models\n* insights into the feature selection method: call the `._processed_shaps_df` on a fitted `PowerSHAP` feature selector.\n* tested code!\n\n## Benchmarks ⏱\n\nCheck out our benchmark results [here](examples/results/).  \n\n## How does it work ⁉️\n\nPowershap is built on the core assumption that *an informative feature will have a larger impact on the prediction compared to a known random feature.*\n\n* Powershap trains multiple models with different random seeds on different subsets of the data. Each iteration it adds a random uniform feature to the dataset for training.\n* In a single iteration after training a model, powershap calculates the absolute Shapley values of all features, including the random feature. If there are multiple outputs or multiple classes, powershap uses the maximum across these multiple outputs. These values are then averaged for each feature, symbolising the impact of the feature in this iteration.\n* After performing all iterations, each feature then has an array of impacts. The impact array of each feature is then compared to the average of the random feature impact array using the percentile formula to provide a p-value. This tests whether the feature has a larger impact than the random feature and outputs a low p-value if true. \n* Powershap then outputs all features with a p-value below the provided threshold. The threshold is by default 0.01.\n\n\n### Automatic mode 🤖\n\nThe required number of iterations and the threshold values are hyperparameters of powershap. However, to *avoid manually optimizing the hyperparameters* powershap by default uses an automatic mode that automatically determines these hyperparameters. \n\n* The automatic mode first starts with executing powershap using ten iterations.\n* Then, for each feature powershap calculates the effect size and the statistical power of the test using a student-t power test. \n* Using the calculated effect size, powershap then calculates the required iterations to achieve a predefined power requirement. By default this is 0.99, which represents a false positive probability of 0.01.\n* If the required iterations are larger than the already performed iterations, powershap then further executes for the extra required iterations. \n* Afterward, powershap re-calculates the required iterations and it keeps re-executing until the required iterations are met.\n\n## Referencing our package :memo:\n\nIf you use *powershap* in a scientific publication, we would highly appreciate citing us as:\n\n```bibtex\n@misc{https://doi.org/10.48550/arxiv.2206.08394,\n  doi = {10.48550/ARXIV.2206.08394},\n  url = {https://arxiv.org/abs/2206.08394},\n  author = {Verhaeghe, Jarne and Van Der Donckt, Jeroen and Ongenae, Femke and Van Hoecke, Sofie},\n  keywords = {Machine Learning (cs.LG), Machine Learning (stat.ML), FOS: Computer and information sciences, FOS: Computer and information sciences},\n  title = {Powershap: A Power-full Shapley Feature Selection Method},\n  publisher = {arXiv},\n  year = {2022}\n  copyright = {arXiv.org perpetual, non-exclusive license}\n}\n\n```\n\nPaper is accepted at ECML PKDD 2022 and will be presented there. The preprint can be found on arXiv ([link](https://arxiv.org/abs/2206.08394)) and on the github.\n\n---\n\n<p align="center">\n👤 <i>Jarne Verhaeghe, Jeroen Van Der Donckt</i>\n</p>\n',
+    'long_description': '\t\n<p align="center">\n    <a href="#readme">\n        <img alt="PowerShap logo" src="https://raw.githubusercontent.com/predict-idlab/powershap/main/powershap_full_scaled.png" width=70%>\n    </a>\n</p>\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/powershap.svg)](https://pypi.org/project/powershap/)\n[![support-version](https://img.shields.io/pypi/pyversions/powershap)](https://img.shields.io/pypi/pyversions/powershap)\n[![codecov](https://img.shields.io/codecov/c/github/predict-idlab/powershap?logo=codecov)](https://codecov.io/gh/predict-idlab/powershap)\n[![Downloads](https://pepy.tech/badge/powershap)](https://pepy.tech/project/powershap)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)\n[![Testing](https://github.com/predict-idlab/powershap/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/powershap/actions/workflows/test.yml)\n[![DOI](https://zenodo.org/badge/470633431.svg)](https://zenodo.org/badge/latestdoi/470633431)\n\n> *powershap* is a **feature selection method** that uses statistical hypothesis testing and power calculations on **Shapley values**, enabling fast and intuitive wrapper-based feature selection.  \n\n## Installation ⚙️\n\n| [**pip**](https://pypi.org/project/powershap/) | `pip install powershap` | \n| ---| ----|\n\n## Usage 🛠\n\n*powershap* is built to be intuitive, it supports various models including linear, tree-based, and even deep learning models for classification and regression tasks.  \n<!-- It is also implented as sklearn `Transformer` component, allowing convenient integration in `sklearn` pipelines. -->\n\n```py\nfrom powershap import PowerShap\nfrom catboost import CatBoostClassifier\n\nX, y = ...  # your classification dataset\n\nselector = PowerShap(\n    model=CatBoostClassifier(n_estimators=250, verbose=0, use_best_model=True)\n)\n\nselector.fit(X, y)  # Fit the PowerShap feature selector\nselector.transform(X)  # Reduce the dataset to the selected features\n\n```\n\n## Features ✨\n\n* default automatic mode\n* `scikit-learn` compatible\n* supports various models\n* insights into the feature selection method: call the `._processed_shaps_df` on a fitted `PowerSHAP` feature selector.\n* tested code!\n\n## Benchmarks ⏱\n\nCheck out our benchmark results [here](examples/results/).  \n\n## How does it work ⁉️\n\nPowershap is built on the core assumption that *an informative feature will have a larger impact on the prediction compared to a known random feature.*\n\n* Powershap trains multiple models with different random seeds on different subsets of the data. Each iteration it adds a random uniform feature to the dataset for training.\n* In a single iteration after training a model, powershap calculates the absolute Shapley values of all features, including the random feature. If there are multiple outputs or multiple classes, powershap uses the maximum across these multiple outputs. These values are then averaged for each feature, symbolising the impact of the feature in this iteration.\n* After performing all iterations, each feature then has an array of impacts. The impact array of each feature is then compared to the average of the random feature impact array using the percentile formula to provide a p-value. This tests whether the feature has a larger impact than the random feature and outputs a low p-value if true. \n* Powershap then outputs all features with a p-value below the provided threshold. The threshold is by default 0.01.\n\n\n### Automatic mode 🤖\n\nThe required number of iterations and the threshold values are hyperparameters of powershap. However, to *avoid manually optimizing the hyperparameters* powershap by default uses an automatic mode that automatically determines these hyperparameters. \n\n* The automatic mode first starts with executing powershap using ten iterations.\n* Then, for each feature powershap calculates the effect size and the statistical power of the test using a student-t power test. \n* Using the calculated effect size, powershap then calculates the required iterations to achieve a predefined power requirement. By default this is 0.99, which represents a false positive probability of 0.01.\n* If the required iterations are larger than the already performed iterations, powershap then further executes for the extra required iterations. \n* Afterward, powershap re-calculates the required iterations and it keeps re-executing until the required iterations are met.\n\n## Referencing our package :memo:\n\nIf you use *powershap* in a scientific publication, we would highly appreciate citing us as:\n\n```bibtex\n@misc{https://doi.org/10.48550/arxiv.2206.08394,\n  doi = {10.48550/ARXIV.2206.08394},\n  url = {https://arxiv.org/abs/2206.08394},\n  author = {Verhaeghe, Jarne and Van Der Donckt, Jeroen and Ongenae, Femke and Van Hoecke, Sofie},\n  keywords = {Machine Learning (cs.LG), Machine Learning (stat.ML), FOS: Computer and information sciences, FOS: Computer and information sciences},\n  title = {Powershap: A Power-full Shapley Feature Selection Method},\n  publisher = {arXiv},\n  year = {2022}\n  copyright = {arXiv.org perpetual, non-exclusive license}\n}\n\n```\n\nPaper is accepted at ECML PKDD 2022 and will be presented there. The preprint can be found on arXiv ([link](https://arxiv.org/abs/2206.08394)) and on the github.\n\n---\n\n<p align="center">\n👤 <i>Jarne Verhaeghe, Jeroen Van Der Donckt</i>\n</p>\n',
     'author': 'Jarne Verhaeghe, Jeroen Van Der Donckt',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/predict-idlab/powershap',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<3.10',
+    'python_requires': '>=3.7,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,34 +1,32 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['powershap',
 'powershap.shap_wrappers'] package_data = \ {'': ['*']} install_requires = \
-['catboost>=1.0.5,<2.0.0', 'numpy>=1.21,<2.0', 'pandas>=1.3,<2.0',
-'shap>=0.40,<0.41', 'sklearn', 'statsmodels>=0.13.2,<0.14.0'] setup_kwargs =
-{ 'name': 'powershap', 'version': '0.0.8rc2', 'description': 'Feature selection
+['catboost>=1.0.5,<2.0.0', 'numpy>=1.21,<2.0', 'pandas>=1.3,<2.0', 'scikit-
+learn', 'shap>=0.40,<0.41', 'statsmodels>=0.13.2,<0.14.0'] setup_kwargs =
+{ 'name': 'powershap', 'version': '0.0.9', 'description': 'Feature selection
 using statistical significance of shap values', 'long_description': '\t\n
                           \n _\_n_ _[_P_o_w_e_r_S_h_a_p_ _l_o_g_o_]_\_n_ \n
 \n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/powershap.svg)]
 (https://pypi.org/project/powershap/)\n[![support-version](https://
 img.shields.io/pypi/pyversions/powershap)](https://img.shields.io/pypi/
 pyversions/powershap)\n[![codecov](https://img.shields.io/codecov/c/github/
 predict-idlab/powershap?logo=codecov)](https://codecov.io/gh/predict-idlab/
-powershap)\n[![Code quality](https://img.shields.io/lgtm/grade/python/github/
-predict-idlab/powershap?label=code%20quality&logo=lgtm)](https://lgtm.com/
-projects/g/predict-idlab/powershap/context:python)\n[![Downloads](https://
-pepy.tech/badge/powershap)](https://pepy.tech/project/powershap)\n[![PRs
-Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
-makeapullrequest.com)\n[![Testing](https://github.com/predict-idlab/powershap/
-actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/
-powershap/actions/workflows/test.yml)\n[![DOI](https://zenodo.org/badge/
-470633431.svg)](https://zenodo.org/badge/latestdoi/470633431)\n\n> *powershap*
-is a **feature selection method** that uses statistical hypothesis testing and
-power calculations on **Shapley values**, enabling fast and intuitive wrapper-
-based feature selection. \n\n## Installation âï¸\n\n| [**pip**](https://
-pypi.org/project/powershap/) | `pip install powershap` | \n| ---| ----|\n\n##
-Usage ð \n\n*powershap* is built to be intuitive, it supports various models
-including linear, tree-based, and even deep learning models. \n\n\n```py\nfrom
+powershap)\n[![Downloads](https://pepy.tech/badge/powershap)](https://
+pepy.tech/project/powershap)\n[![PRs Welcome](https://img.shields.io/badge/PRs-
+welcome-brightgreen.svg?)](http://makeapullrequest.com)\n[![Testing](https://
+github.com/predict-idlab/powershap/actions/workflows/test.yml/badge.svg)]
+(https://github.com/predict-idlab/powershap/actions/workflows/test.yml)\n[!
+[DOI](https://zenodo.org/badge/470633431.svg)](https://zenodo.org/badge/
+latestdoi/470633431)\n\n> *powershap* is a **feature selection method** that
+uses statistical hypothesis testing and power calculations on **Shapley
+values**, enabling fast and intuitive wrapper-based feature selection. \n\n##
+Installation âï¸\n\n| [**pip**](https://pypi.org/project/powershap/) | `pip
+install powershap` | \n| ---| ----|\n\n## Usage ð \n\n*powershap* is built to
+be intuitive, it supports various models including linear, tree-based, and even
+deep learning models for classification and regression tasks. \n\n\n```py\nfrom
 powershap import PowerShap\nfrom catboost import CatBoostClassifier\n\nX, y =
 ... # your classification dataset\n\nselector = PowerShap(\n
 model=CatBoostClassifier(n_estimators=250, verbose=0,
 use_best_model=True)\n)\n\nselector.fit(X, y) # Fit the PowerShap feature
 selector\nselector.transform(X) # Reduce the dataset to the selected
 features\n\n```\n\n## Features â¨\n\n* default automatic mode\n* `scikit-
 learn` compatible\n* supports various models\n* insights into the feature
@@ -72,12 +70,12 @@
 sciences, FOS: Computer and information sciences},\n title = {Powershap: A
 Power-full Shapley Feature Selection Method},\n publisher = {arXiv},\n year =
 {2022}\n copyright = {arXiv.org perpetual, non-exclusive
 license}\n}\n\n```\n\nPaper is accepted at ECML PKDD 2022 and will be presented
 there. The preprint can be found on arXiv ([link](https://arxiv.org/abs/
 2206.08394)) and on the github.\n\n---\n\n
                 \nð¤ Jarne Verhaeghe, Jeroen Van Der Donckt\n
-\n', 'author': 'Jarne Verhaeghe, Jeroen Van Der Donckt', 'author_email': None,
-'maintainer': None, 'maintainer_email': None, 'url': 'https://github.com/
-predict-idlab/powershap', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.7.1,<3.10', }
-setup(**setup_kwargs)
+\n', 'author': 'Jarne Verhaeghe, Jeroen Van Der Donckt', 'author_email':
+'None', 'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://
+github.com/predict-idlab/powershap', 'packages': packages, 'package_data':
+package_data, 'install_requires': install_requires, 'python_requires':
+'>=3.7,<3.11', } setup(**setup_kwargs)
```

### Comparing `powershap-0.0.8rc2/PKG-INFO` & `powershap-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 Metadata-Version: 2.1
 Name: powershap
-Version: 0.0.8rc2
+Version: 0.0.9
 Summary: Feature selection using statistical significance of shap values
 Home-page: https://github.com/predict-idlab/powershap
 License: MIT
 Keywords: feature selection,shap,data-science,machine learning
 Author: Jarne Verhaeghe, Jeroen Van Der Donckt
-Requires-Python: >=3.7.1,<3.10
+Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: catboost (>=1.0.5,<2.0.0)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: scikit-learn
 Requires-Dist: shap (>=0.40,<0.41)
-Requires-Dist: sklearn
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Project-URL: Repository, https://github.com/predict-idlab/powershap
 Description-Content-Type: text/markdown
 
 	
 <p align="center">
     <a href="#readme">
         <img alt="PowerShap logo" src="https://raw.githubusercontent.com/predict-idlab/powershap/main/powershap_full_scaled.png" width=70%>
     </a>
 </p>
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/powershap.svg)](https://pypi.org/project/powershap/)
 [![support-version](https://img.shields.io/pypi/pyversions/powershap)](https://img.shields.io/pypi/pyversions/powershap)
 [![codecov](https://img.shields.io/codecov/c/github/predict-idlab/powershap?logo=codecov)](https://codecov.io/gh/predict-idlab/powershap)
-[![Code quality](https://img.shields.io/lgtm/grade/python/github/predict-idlab/powershap?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-idlab/powershap/context:python)
 [![Downloads](https://pepy.tech/badge/powershap)](https://pepy.tech/project/powershap)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)
 [![Testing](https://github.com/predict-idlab/powershap/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/powershap/actions/workflows/test.yml)
 [![DOI](https://zenodo.org/badge/470633431.svg)](https://zenodo.org/badge/latestdoi/470633431)
 
 > *powershap* is a **feature selection method** that uses statistical hypothesis testing and power calculations on **Shapley values**, enabling fast and intuitive wrapper-based feature selection.  
 
 ## Installation ⚙️
 
 | [**pip**](https://pypi.org/project/powershap/) | `pip install powershap` | 
 | ---| ----|
 
 ## Usage 🛠
 
-*powershap* is built to be intuitive, it supports various models including linear, tree-based, and even deep learning models.  
+*powershap* is built to be intuitive, it supports various models including linear, tree-based, and even deep learning models for classification and regression tasks.  
 <!-- It is also implented as sklearn `Transformer` component, allowing convenient integration in `sklearn` pipelines. -->
 
 ```py
 from powershap import PowerShap
 from catboost import CatBoostClassifier
 
 X, y = ...  # your classification dataset
```

#### html2text {}

```diff
@@ -1,82 +1,80 @@
-Metadata-Version: 2.1 Name: powershap Version: 0.0.8rc2 Summary: Feature
-selection using statistical significance of shap values Home-page: https://
-github.com/predict-idlab/powershap License: MIT Keywords: feature
-selection,shap,data-science,machine learning Author: Jarne Verhaeghe, Jeroen
-Van Der Donckt Requires-Python: >=3.7.1,<3.10 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Requires-Dist: catboost (>=1.0.5,<2.0.0) Requires-
+Metadata-Version: 2.1 Name: powershap Version: 0.0.9 Summary: Feature selection
+using statistical significance of shap values Home-page: https://github.com/
+predict-idlab/powershap License: MIT Keywords: feature selection,shap,data-
+science,machine learning Author: Jarne Verhaeghe, Jeroen Van Der Donckt
+Requires-Python: >=3.7,<3.11 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Requires-Dist: catboost (>=1.0.5,<2.0.0) Requires-
 Dist: numpy (>=1.21,<2.0) Requires-Dist: pandas (>=1.3,<2.0) Requires-Dist:
-shap (>=0.40,<0.41) Requires-Dist: sklearn Requires-Dist: statsmodels
+scikit-learn Requires-Dist: shap (>=0.40,<0.41) Requires-Dist: statsmodels
 (>=0.13.2,<0.14.0) Project-URL: Repository, https://github.com/predict-idlab/
 powershap Description-Content-Type: text/markdown
                                _[_P_o_w_e_r_S_h_a_p_ _l_o_g_o_]
 [![PyPI Latest Release](https://img.shields.io/pypi/v/powershap.svg)](https://
 pypi.org/project/powershap/) [![support-version](https://img.shields.io/pypi/
 pyversions/powershap)](https://img.shields.io/pypi/pyversions/powershap) [!
 [codecov](https://img.shields.io/codecov/c/github/predict-idlab/
-powershap?logo=codecov)](https://codecov.io/gh/predict-idlab/powershap) [![Code
-quality](https://img.shields.io/lgtm/grade/python/github/predict-idlab/
-powershap?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-
-idlab/powershap/context:python) [![Downloads](https://pepy.tech/badge/
-powershap)](https://pepy.tech/project/powershap) [![PRs Welcome](https://
-img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
-makeapullrequest.com) [![Testing](https://github.com/predict-idlab/powershap/
-actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/
-powershap/actions/workflows/test.yml) [![DOI](https://zenodo.org/badge/
-470633431.svg)](https://zenodo.org/badge/latestdoi/470633431) > *powershap* is
-a **feature selection method** that uses statistical hypothesis testing and
-power calculations on **Shapley values**, enabling fast and intuitive wrapper-
-based feature selection. ## Installation âï¸ | [**pip**](https://pypi.org/
-project/powershap/) | `pip install powershap` | | ---| ----| ## Usage ð 
-*powershap* is built to be intuitive, it supports various models including
-linear, tree-based, and even deep learning models. ```py from powershap import
-PowerShap from catboost import CatBoostClassifier X, y = ... # your
-classification dataset selector = PowerShap( model=CatBoostClassifier
-(n_estimators=250, verbose=0, use_best_model=True) ) selector.fit(X, y) # Fit
-the PowerShap feature selector selector.transform(X) # Reduce the dataset to
-the selected features ``` ## Features â¨ * default automatic mode * `scikit-
-learn` compatible * supports various models * insights into the feature
-selection method: call the `._processed_shaps_df` on a fitted `PowerSHAP`
-feature selector. * tested code! ## Benchmarks â± Check out our benchmark
-results [here](examples/results/). ## How does it work âï¸ Powershap is
-built on the core assumption that *an informative feature will have a larger
-impact on the prediction compared to a known random feature.* * Powershap
-trains multiple models with different random seeds on different subsets of the
-data. Each iteration it adds a random uniform feature to the dataset for
-training. * In a single iteration after training a model, powershap calculates
-the absolute Shapley values of all features, including the random feature. If
-there are multiple outputs or multiple classes, powershap uses the maximum
-across these multiple outputs. These values are then averaged for each feature,
-symbolising the impact of the feature in this iteration. * After performing all
-iterations, each feature then has an array of impacts. The impact array of each
-feature is then compared to the average of the random feature impact array
-using the percentile formula to provide a p-value. This tests whether the
-feature has a larger impact than the random feature and outputs a low p-value
-if true. * Powershap then outputs all features with a p-value below the
-provided threshold. The threshold is by default 0.01. ### Automatic mode ð¤
-The required number of iterations and the threshold values are hyperparameters
-of powershap. However, to *avoid manually optimizing the hyperparameters*
-powershap by default uses an automatic mode that automatically determines these
-hyperparameters. * The automatic mode first starts with executing powershap
-using ten iterations. * Then, for each feature powershap calculates the effect
-size and the statistical power of the test using a student-t power test. *
-Using the calculated effect size, powershap then calculates the required
-iterations to achieve a predefined power requirement. By default this is 0.99,
-which represents a false positive probability of 0.01. * If the required
-iterations are larger than the already performed iterations, powershap then
-further executes for the extra required iterations. * Afterward, powershap re-
-calculates the required iterations and it keeps re-executing until the required
-iterations are met. ## Referencing our package :memo: If you use *powershap* in
-a scientific publication, we would highly appreciate citing us as: ```bibtex
-@misc{https://doi.org/10.48550/arxiv.2206.08394, doi = {10.48550/
-ARXIV.2206.08394}, url = {https://arxiv.org/abs/2206.08394}, author =
-{Verhaeghe, Jarne and Van Der Donckt, Jeroen and Ongenae, Femke and Van Hoecke,
-Sofie}, keywords = {Machine Learning (cs.LG), Machine Learning (stat.ML), FOS:
-Computer and information sciences, FOS: Computer and information sciences},
-title = {Powershap: A Power-full Shapley Feature Selection Method}, publisher =
-{arXiv}, year = {2022} copyright = {arXiv.org perpetual, non-exclusive license}
-} ``` Paper is accepted at ECML PKDD 2022 and will be presented there. The
-preprint can be found on arXiv ([link](https://arxiv.org/abs/2206.08394)) and
-on the github. ---
+powershap?logo=codecov)](https://codecov.io/gh/predict-idlab/powershap) [!
+[Downloads](https://pepy.tech/badge/powershap)](https://pepy.tech/project/
+powershap) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-
+brightgreen.svg?)](http://makeapullrequest.com) [![Testing](https://github.com/
+predict-idlab/powershap/actions/workflows/test.yml/badge.svg)](https://
+github.com/predict-idlab/powershap/actions/workflows/test.yml) [![DOI](https://
+zenodo.org/badge/470633431.svg)](https://zenodo.org/badge/latestdoi/470633431)
+> *powershap* is a **feature selection method** that uses statistical
+hypothesis testing and power calculations on **Shapley values**, enabling fast
+and intuitive wrapper-based feature selection. ## Installation âï¸ |
+[**pip**](https://pypi.org/project/powershap/) | `pip install powershap` | | --
+-| ----| ## Usage ð  *powershap* is built to be intuitive, it supports
+various models including linear, tree-based, and even deep learning models for
+classification and regression tasks. ```py from powershap import PowerShap from
+catboost import CatBoostClassifier X, y = ... # your classification dataset
+selector = PowerShap( model=CatBoostClassifier(n_estimators=250, verbose=0,
+use_best_model=True) ) selector.fit(X, y) # Fit the PowerShap feature selector
+selector.transform(X) # Reduce the dataset to the selected features ``` ##
+Features â¨ * default automatic mode * `scikit-learn` compatible * supports
+various models * insights into the feature selection method: call the
+`._processed_shaps_df` on a fitted `PowerSHAP` feature selector. * tested code!
+## Benchmarks â± Check out our benchmark results [here](examples/results/). ##
+How does it work âï¸ Powershap is built on the core assumption that *an
+informative feature will have a larger impact on the prediction compared to a
+known random feature.* * Powershap trains multiple models with different random
+seeds on different subsets of the data. Each iteration it adds a random uniform
+feature to the dataset for training. * In a single iteration after training a
+model, powershap calculates the absolute Shapley values of all features,
+including the random feature. If there are multiple outputs or multiple
+classes, powershap uses the maximum across these multiple outputs. These values
+are then averaged for each feature, symbolising the impact of the feature in
+this iteration. * After performing all iterations, each feature then has an
+array of impacts. The impact array of each feature is then compared to the
+average of the random feature impact array using the percentile formula to
+provide a p-value. This tests whether the feature has a larger impact than the
+random feature and outputs a low p-value if true. * Powershap then outputs all
+features with a p-value below the provided threshold. The threshold is by
+default 0.01. ### Automatic mode ð¤ The required number of iterations and the
+threshold values are hyperparameters of powershap. However, to *avoid manually
+optimizing the hyperparameters* powershap by default uses an automatic mode
+that automatically determines these hyperparameters. * The automatic mode first
+starts with executing powershap using ten iterations. * Then, for each feature
+powershap calculates the effect size and the statistical power of the test
+using a student-t power test. * Using the calculated effect size, powershap
+then calculates the required iterations to achieve a predefined power
+requirement. By default this is 0.99, which represents a false positive
+probability of 0.01. * If the required iterations are larger than the already
+performed iterations, powershap then further executes for the extra required
+iterations. * Afterward, powershap re-calculates the required iterations and it
+keeps re-executing until the required iterations are met. ## Referencing our
+package :memo: If you use *powershap* in a scientific publication, we would
+highly appreciate citing us as: ```bibtex @misc{https://doi.org/10.48550/
+arxiv.2206.08394, doi = {10.48550/ARXIV.2206.08394}, url = {https://arxiv.org/
+abs/2206.08394}, author = {Verhaeghe, Jarne and Van Der Donckt, Jeroen and
+Ongenae, Femke and Van Hoecke, Sofie}, keywords = {Machine Learning (cs.LG),
+Machine Learning (stat.ML), FOS: Computer and information sciences, FOS:
+Computer and information sciences}, title = {Powershap: A Power-full Shapley
+Feature Selection Method}, publisher = {arXiv}, year = {2022} copyright =
+{arXiv.org perpetual, non-exclusive license} } ``` Paper is accepted at ECML
+PKDD 2022 and will be presented there. The preprint can be found on arXiv (
+[link](https://arxiv.org/abs/2206.08394)) and on the github. ---
                   ð¤ Jarne Verhaeghe, Jeroen Van Der Donckt
```

