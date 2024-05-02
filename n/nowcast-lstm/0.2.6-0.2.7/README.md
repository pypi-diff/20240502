# Comparing `tmp/nowcast_lstm-0.2.6.tar.gz` & `tmp/nowcast_lstm-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcast_lstm-0.2.6.tar", last modified: Fri Nov 24 10:15:34 2023, max compression
+gzip compressed data, was "nowcast_lstm-0.2.7.tar", last modified: Thu May  2 12:46:42 2024, max compression
```

## Comparing `nowcast_lstm-0.2.6.tar` & `nowcast_lstm-0.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2023-11-24 10:15:34.994566 nowcast_lstm-0.2.6/
--rw-r--r--   0 danielhopp   (501) staff       (20)     1068 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.6/LICENSE
--rw-r--r--   0 danielhopp   (501) staff       (20)    12811 2023-11-24 10:15:34.994394 nowcast_lstm-0.2.6/PKG-INFO
--rw-r--r--   0 danielhopp   (501) staff       (20)    12340 2023-11-24 10:13:57.000000 nowcast_lstm-0.2.6/README.md
-drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2023-11-24 10:15:34.993134 nowcast_lstm-0.2.6/nowcast_lstm/
--rw-r--r--   0 danielhopp   (501) staff       (20)    26068 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.6/nowcast_lstm/LSTM.py
--rw-r--r--   0 danielhopp   (501) staff       (20)        0 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.6/nowcast_lstm/__init__.py
--rw-r--r--   0 danielhopp   (501) staff       (20)    17474 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.6/nowcast_lstm/data_setup.py
--rw-r--r--   0 danielhopp   (501) staff       (20)     4457 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.6/nowcast_lstm/interval_prediction.py
--rw-r--r--   0 danielhopp   (501) staff       (20)    45719 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.6/nowcast_lstm/model_selection.py
--rw-r--r--   0 danielhopp   (501) staff       (20)    11174 2023-11-24 10:13:57.000000 nowcast_lstm-0.2.6/nowcast_lstm/modelling.py
--rw-r--r--   0 danielhopp   (501) staff       (20)     1895 2023-11-24 10:13:57.000000 nowcast_lstm-0.2.6/nowcast_lstm/mv_lstm.py
-drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2023-11-24 10:15:34.993569 nowcast_lstm-0.2.6/nowcast_lstm.egg-info/
--rw-r--r--   0 danielhopp   (501) staff       (20)    12811 2023-11-24 10:15:34.000000 nowcast_lstm-0.2.6/nowcast_lstm.egg-info/PKG-INFO
--rw-r--r--   0 danielhopp   (501) staff       (20)      447 2023-11-24 10:15:34.000000 nowcast_lstm-0.2.6/nowcast_lstm.egg-info/SOURCES.txt
--rw-r--r--   0 danielhopp   (501) staff       (20)        1 2023-11-24 10:15:34.000000 nowcast_lstm-0.2.6/nowcast_lstm.egg-info/dependency_links.txt
--rw-r--r--   0 danielhopp   (501) staff       (20)       19 2023-11-24 10:15:34.000000 nowcast_lstm-0.2.6/nowcast_lstm.egg-info/top_level.txt
--rw-r--r--   0 danielhopp   (501) staff       (20)       38 2023-11-24 10:15:34.994605 nowcast_lstm-0.2.6/setup.cfg
--rw-r--r--   0 danielhopp   (501) staff       (20)      686 2023-11-24 10:13:57.000000 nowcast_lstm-0.2.6/setup.py
-drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2023-11-24 10:15:34.994194 nowcast_lstm-0.2.6/tests/
--rw-r--r--   0 danielhopp   (501) staff       (20)        0 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.6/tests/__init__.py
--rw-r--r--   0 danielhopp   (501) staff       (20)     5571 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.6/tests/test_LSTM.py
--rw-r--r--   0 danielhopp   (501) staff       (20)     6100 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.6/tests/test_data_setup.py
--rw-r--r--   0 danielhopp   (501) staff       (20)     3470 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.6/tests/test_modelling.py
+drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2024-05-02 12:46:42.620288 nowcast_lstm-0.2.7/
+-rw-r--r--   0 danielhopp   (501) staff       (20)     1068 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.7/LICENSE
+-rw-r--r--   0 danielhopp   (501) staff       (20)    13196 2024-05-02 12:46:42.620048 nowcast_lstm-0.2.7/PKG-INFO
+-rw-r--r--   0 danielhopp   (501) staff       (20)    12725 2024-05-02 12:45:45.000000 nowcast_lstm-0.2.7/README.md
+drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2024-05-02 12:46:42.619011 nowcast_lstm-0.2.7/nowcast_lstm/
+-rw-r--r--   0 danielhopp   (501) staff       (20)    26899 2024-05-02 12:45:45.000000 nowcast_lstm-0.2.7/nowcast_lstm/LSTM.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)        0 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.7/nowcast_lstm/__init__.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)    17474 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.7/nowcast_lstm/data_setup.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)     4457 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.7/nowcast_lstm/interval_prediction.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)    45801 2024-05-02 12:45:45.000000 nowcast_lstm-0.2.7/nowcast_lstm/model_selection.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)    11766 2024-05-02 12:45:45.000000 nowcast_lstm-0.2.7/nowcast_lstm/modelling.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)     2283 2024-05-02 12:45:45.000000 nowcast_lstm-0.2.7/nowcast_lstm/mv_lstm.py
+drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2024-05-02 12:46:42.619428 nowcast_lstm-0.2.7/nowcast_lstm.egg-info/
+-rw-r--r--   0 danielhopp   (501) staff       (20)    13196 2024-05-02 12:46:42.000000 nowcast_lstm-0.2.7/nowcast_lstm.egg-info/PKG-INFO
+-rw-r--r--   0 danielhopp   (501) staff       (20)      447 2024-05-02 12:46:42.000000 nowcast_lstm-0.2.7/nowcast_lstm.egg-info/SOURCES.txt
+-rw-r--r--   0 danielhopp   (501) staff       (20)        1 2024-05-02 12:46:42.000000 nowcast_lstm-0.2.7/nowcast_lstm.egg-info/dependency_links.txt
+-rw-r--r--   0 danielhopp   (501) staff       (20)       19 2024-05-02 12:46:42.000000 nowcast_lstm-0.2.7/nowcast_lstm.egg-info/top_level.txt
+-rw-r--r--   0 danielhopp   (501) staff       (20)       38 2024-05-02 12:46:42.620321 nowcast_lstm-0.2.7/setup.cfg
+-rw-r--r--   0 danielhopp   (501) staff       (20)      686 2024-05-02 12:45:45.000000 nowcast_lstm-0.2.7/setup.py
+drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2024-05-02 12:46:42.619829 nowcast_lstm-0.2.7/tests/
+-rw-r--r--   0 danielhopp   (501) staff       (20)        0 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.7/tests/__init__.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)     5571 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.7/tests/test_LSTM.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)     6100 2023-11-24 09:43:27.000000 nowcast_lstm-0.2.7/tests/test_data_setup.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)     3484 2024-05-02 12:45:45.000000 nowcast_lstm-0.2.7/tests/test_modelling.py
```

### Comparing `nowcast_lstm-0.2.6/LICENSE` & `nowcast_lstm-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nowcast_lstm-0.2.6/PKG-INFO` & `nowcast_lstm-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcast_lstm
-Version: 0.2.6
+Version: 0.2.7
 Summary: Code for running LSTM neural networks on economic data for nowcasting
 Home-page: https://github.com/dhopp1/nowcast_lstm
 Author: Daniel Hopp
 Author-email: daniel.hopp@un.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,26 +43,27 @@
 [LSTM neural networks](https://en.wikipedia.org/wiki/Long_short-term_memory) have been used for nowcasting [before](https://papers.nips.cc/paper/2015/file/07563a3fe3bbe7e3ba84431ad9d055af-Paper.pdf), combining the strengths of artificial neural networks with a temporal aspect. However their use in nowcasting economic indicators remains limited, no doubt in part due to the difficulty of obtaining results in existing deep learning frameworks. This library seeks to streamline the process of obtaining results in the hopes of expanding the domains to which LSTM can be applied.
 
 While neural networks are flexible and this framework may be able to get sensible results on levels, the model architecture was developed to nowcast growth rates of economic indicators. As such training inputs should ideally be stationary and seasonally adjusted.
 
 Further explanation of the background problem can be found in [this paper](https://unctad.org/system/files/official-document/ser-rp-2018d9_en.pdf). Further explanation and results can be found in [this](https://www.researchgate.net/publication/363509881_Economic_Nowcasting_with_Long_Short-Term_Memory_Artificial_Neural_Networks_LSTM) paper in the Journal of Official Statistics.
 
 ## R, MATLAB, and Julia wrappers 
-[R](https://github.com/dhopp1/nowcastLSTM),  [MATLAB](https://github.com/dhopp1/nowcast_lstm_matlab), and [Julia](https://github.com/dhopp1/NowcastLSTM.jl) wrappers exist for this Python library. Python and some Python libraries still need to be installed on your system, but full functionality from R, MATLAB, and Julia can be obtained with the wrappers without any Python knowledge.
+[R](https://github.com/dhopp1/nowcastLSTM),  [MATLAB](https://github.com/dhopp1/nowcast_lstm_matlab), and [Julia](https://github.com/dhopp1/NowcastLSTM.jl) wrappers exist for this Python library. Python and some Python libraries still need to be installed on your system, but full functionality from R can be obtained with the wrappers without any Python knowledge. The MATLAB and Julia wrappers work with older versions of the library but are no longer being mantained and updated to work with the newest features.
 
 
 ## Quick usage
 The main object and functionality of the library comes from the `LSTM` object. Given `data` = a pandas DataFrame of a date column + monthly data + a quarterly target series to run the model on, usage is as follows:
 
 ```python
 from nowcast_lstm.LSTM import LSTM
 
 # note that if a column has no data in it, i.e., is all NAs, its values will be replaced with 0. This won't affect model performance and will ensure that the model can still be trained
 # a list of columns with no data in them can be accessed with `model.no_data_cols`
 model = LSTM(data, "target_col_name", n_timesteps=12) # default parameters with 12 timestep history
+#model = LSTM(data, "target_col_name", n_timesteps=12, n_models=10, seeds=list(range(10)) # For reproducibility on a single machine/system, give a list of manual seeds as long as the n_models parameter. Reproducibility across machines is not guaranteed.
 
 model.X # array of the transformed training dataset
 model.y # array of the target values
 
 model.mv_lstm # list of trained PyTorch network(s)
 model.train_loss # list of training losses for the network(s)
```

### Comparing `nowcast_lstm-0.2.6/README.md` & `nowcast_lstm-0.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,27 @@
 [LSTM neural networks](https://en.wikipedia.org/wiki/Long_short-term_memory) have been used for nowcasting [before](https://papers.nips.cc/paper/2015/file/07563a3fe3bbe7e3ba84431ad9d055af-Paper.pdf), combining the strengths of artificial neural networks with a temporal aspect. However their use in nowcasting economic indicators remains limited, no doubt in part due to the difficulty of obtaining results in existing deep learning frameworks. This library seeks to streamline the process of obtaining results in the hopes of expanding the domains to which LSTM can be applied.
 
 While neural networks are flexible and this framework may be able to get sensible results on levels, the model architecture was developed to nowcast growth rates of economic indicators. As such training inputs should ideally be stationary and seasonally adjusted.
 
 Further explanation of the background problem can be found in [this paper](https://unctad.org/system/files/official-document/ser-rp-2018d9_en.pdf). Further explanation and results can be found in [this](https://www.researchgate.net/publication/363509881_Economic_Nowcasting_with_Long_Short-Term_Memory_Artificial_Neural_Networks_LSTM) paper in the Journal of Official Statistics.
 
 ## R, MATLAB, and Julia wrappers 
-[R](https://github.com/dhopp1/nowcastLSTM),  [MATLAB](https://github.com/dhopp1/nowcast_lstm_matlab), and [Julia](https://github.com/dhopp1/NowcastLSTM.jl) wrappers exist for this Python library. Python and some Python libraries still need to be installed on your system, but full functionality from R, MATLAB, and Julia can be obtained with the wrappers without any Python knowledge.
+[R](https://github.com/dhopp1/nowcastLSTM),  [MATLAB](https://github.com/dhopp1/nowcast_lstm_matlab), and [Julia](https://github.com/dhopp1/NowcastLSTM.jl) wrappers exist for this Python library. Python and some Python libraries still need to be installed on your system, but full functionality from R can be obtained with the wrappers without any Python knowledge. The MATLAB and Julia wrappers work with older versions of the library but are no longer being mantained and updated to work with the newest features.
 
 
 ## Quick usage
 The main object and functionality of the library comes from the `LSTM` object. Given `data` = a pandas DataFrame of a date column + monthly data + a quarterly target series to run the model on, usage is as follows:
 
 ```python
 from nowcast_lstm.LSTM import LSTM
 
 # note that if a column has no data in it, i.e., is all NAs, its values will be replaced with 0. This won't affect model performance and will ensure that the model can still be trained
 # a list of columns with no data in them can be accessed with `model.no_data_cols`
 model = LSTM(data, "target_col_name", n_timesteps=12) # default parameters with 12 timestep history
+#model = LSTM(data, "target_col_name", n_timesteps=12, n_models=10, seeds=list(range(10)) # For reproducibility on a single machine/system, give a list of manual seeds as long as the n_models parameter. Reproducibility across machines is not guaranteed.
 
 model.X # array of the transformed training dataset
 model.y # array of the target values
 
 model.mv_lstm # list of trained PyTorch network(s)
 model.train_loss # list of training losses for the network(s)
```

### Comparing `nowcast_lstm-0.2.6/nowcast_lstm/LSTM.py` & `nowcast_lstm-0.2.7/nowcast_lstm/LSTM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from importlib import import_module
 import numpy as np
 import pandas as pd
+import torch
 import datetime
 
 import nowcast_lstm.data_setup
 import nowcast_lstm.modelling
 import nowcast_lstm.interval_prediction as ip
 
 
@@ -33,14 +34,15 @@
         :decay: float: learning rate decay
         :n_hidden: int: number of hidden states in the network
         :n_layers: int: number of LSTM layers in the network
         :dropout: float: dropout rate between the LSTM layers
         :criterion: torch loss criterion, defaults to MAE
         :optimizer: torch optimizer, defaults to Adam
         :optimizer_parameters: dictionary: list of parameters for optimizer, including learning rate. E.g. {"lr": 1e-2}
+        :seeds: List[int]: what to seed the initial weights for reproducibility. Must be list of same length as n_models parameter
     """
 
     def __init__(
         self,
         data,
         target_variable,
         n_timesteps,
@@ -52,34 +54,44 @@
         decay=0.98,
         n_hidden=20,
         n_layers=2,
         dropout=0,
         criterion="",
         optimizer="",
         optimizer_parameters={"lr": 1e-2},
+        seeds=[],
     ):
         self.data_setup = import_module("nowcast_lstm.data_setup")
         self.modelling = import_module("nowcast_lstm.modelling")
 
         self.data = data.reset_index(drop=True)
         # check for columns with no data in them
-        self.no_data_cols = [col for col in self.data.columns if self.data[col].isnull().sum() / len(self.data) == 1.0]
-        if (len(self.no_data_cols) > 0):
+        self.no_data_cols = [
+            col
+            for col in self.data.columns
+            if self.data[col].isnull().sum() / len(self.data) == 1.0
+        ]
+        if len(self.no_data_cols) > 0:
             for col in self.no_data_cols:
                 self.data[col] = 0.0
-        
+
         self.target_variable = target_variable
         self.n_timesteps = n_timesteps
 
         self.fill_na_func = fill_na_func
         self.fill_ragged_edges_func = fill_ragged_edges_func
 
         self.train_episodes = train_episodes
         self.n_models = n_models
 
+        if seeds == []:
+            self.seeds = [np.random.randint(0, 1e9) for i in range(self.n_models)]
+        else:
+            self.seeds = seeds
+
         self.batch_size = batch_size
         self.decay = decay
         self.n_hidden = n_hidden
         self.n_layers = n_layers
         self.dropout = dropout
         self.criterion = criterion
         self.optimizer = optimizer
@@ -112,14 +124,21 @@
         self.ragged_X = self.ragged_input[0]
 
         self.mv_lstm = []
         self.train_loss = []
 
         self.feature_contribution_values = None
 
+        if torch.cuda.is_available():
+            self.device = f"cuda:{torch.cuda.current_device()}"
+        elif torch.backends.mps.is_available() and torch.backends.mps.is_built():
+            self.device = "cpu"  # "mps" mps slower than cpu
+        else:
+            self.device = "cpu"
+
     def train(self, num_workers=0, shuffle=False, quiet=False):
         """train the model
 
         :num_workers: int: number of workers for multi-process data loading
         :shuffle: boolean: whether to shuffle data at every epoch
         :quiet: boolean: whether or not to print the losses in the epoch loop
         """
@@ -132,14 +151,16 @@
                 n_timesteps=self.n_timesteps,
                 n_hidden=self.n_hidden,
                 n_layers=self.n_layers,
                 dropout=self.dropout,
                 criterion=self.criterion,
                 optimizer=self.optimizer,
                 optimizer_parameters=self.optimizer_parameters,
+                seed=self.seeds[i],
+                device=self.device,
             )
             mv_lstm = instantiated["mv_lstm"]
             criterion = instantiated["criterion"]
             optimizer = instantiated["optimizer"]
             # train the model
             trained = self.modelling.train_model(
                 self.X,
@@ -149,14 +170,15 @@
                 optimizer,
                 train_episodes=self.train_episodes,
                 batch_size=self.batch_size,
                 decay=self.decay,
                 num_workers=num_workers,
                 shuffle=shuffle,
                 quiet=quiet,
+                device=self.device,
             )
             self.mv_lstm.append(trained["mv_lstm"])
             self.train_loss.append(trained["train_loss"])
 
     def predict(self, data, only_actuals_obs=False):
         """Make predictions on a dataframe with same columns and order as the model was trained on, including the target variable.
 
@@ -182,15 +204,15 @@
         )
         X = model_input[0]
         y = model_input[1]
 
         # predictions on every model
         preds = []
         for i in range(self.n_models):
-            preds.append(self.modelling.predict(X, self.mv_lstm[i]))
+            preds.append(self.modelling.predict(X, self.mv_lstm[i], device=self.device))
         preds = list(np.mean(preds, axis=0))
 
         prediction_df = pd.DataFrame(
             {
                 "date": date_series[
                     (len(date_series) - len(preds)) :
                 ].values.flatten(),  # may lose some observations at the beginning depending on n_timeperiods, account for that
@@ -284,15 +306,15 @@
         output:
             :return: pandas DataFrame of actuals, predictions, and dates
         """
         X, y, dates = self.gen_ragged_X(pub_lags, lag, data, start_date, end_date)
         # predictions on every model
         preds = []
         for i in range(self.n_models):
-            preds.append(self.modelling.predict(X, self.mv_lstm[i]))
+            preds.append(self.modelling.predict(X, self.mv_lstm[i], device=self.device))
         preds = list(np.mean(preds, axis=0))
         pred_df = pd.DataFrame(
             {
                 "date": dates,
                 "actuals": y,
                 "predictions": preds,
             }
@@ -390,15 +412,15 @@
         )
         X = model_input[0]
         y = model_input[1]
 
         # predictions on every model
         preds = []
         for i in range(self.n_models):
-            preds.append(self.modelling.predict(X, self.mv_lstm[i]))
+            preds.append(self.modelling.predict(X, self.mv_lstm[i], device=self.device))
 
         point_preds = list(np.mean(preds, axis=0))
 
         prediction_df = pd.DataFrame(
             {
                 "date": date_series[
                     (len(date_series) - len(point_preds)) :
@@ -516,15 +538,15 @@
             end_date=end_date,
         )
         date_series = pd.Series(date_series)
 
         # predictions on every model
         preds = []
         for i in range(self.n_models):
-            preds.append(self.modelling.predict(X, self.mv_lstm[i]))
+            preds.append(self.modelling.predict(X, self.mv_lstm[i], device=self.device))
 
         point_preds = list(np.mean(preds, axis=0))
 
         prediction_df = pd.DataFrame(
             {
                 "date": date_series[
                     (len(date_series) - len(point_preds)) :
```

### Comparing `nowcast_lstm-0.2.6/nowcast_lstm/data_setup.py` & `nowcast_lstm-0.2.7/nowcast_lstm/data_setup.py`

 * *Files identical despite different names*

### Comparing `nowcast_lstm-0.2.6/nowcast_lstm/interval_prediction.py` & `nowcast_lstm-0.2.7/nowcast_lstm/interval_prediction.py`

 * *Files identical despite different names*

### Comparing `nowcast_lstm-0.2.6/nowcast_lstm/model_selection.py` & `nowcast_lstm-0.2.7/nowcast_lstm/model_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,37 +72,42 @@
     lags=[],
     performance_metric="RMSE",
     quiet=False,
 ):
     "univariate runs to determine order for additive variable selection"
 
     data = data.copy()
-    
+
     # first valid index of target variable
     start_index = data.loc[lambda x: ~pd.isna(x[target_variable]), :].index[0]
-    start_index = np.max([0, start_index - n_timesteps + 1]) # where to start the data considering n_timesteps
-    data = data.loc[start_index:, :].reset_index(drop = True)
-    
+    start_index = np.max(
+        [0, start_index - n_timesteps + 1]
+    )  # where to start the data considering n_timesteps
+    data = data.loc[start_index:, :].reset_index(drop=True)
+
     # fold train indices
     end_train_indices = gen_folds(data, n_folds=n_folds, init_test_size=init_test_size)
-    
+
     # check for columns with not enough data for the train set
     shortest_train = data.loc[: end_train_indices[0], :]
-    no_data_cols = [col for col in shortest_train.columns if shortest_train[col].isnull().sum() / len(shortest_train) == 1.0]
-    if (len(no_data_cols) > 0):
+    no_data_cols = [
+        col
+        for col in shortest_train.columns
+        if shortest_train[col].isnull().sum() / len(shortest_train) == 1.0
+    ]
+    if len(no_data_cols) > 0:
         for col in no_data_cols:
             data[col] = 0.0
-    
+
     # columns to assess, excluding date column and target variable
     columns = list(data.columns[data.columns != target_variable][1:])
 
     # initializing performance dictionary
     performance = dict.fromkeys(columns, [])
 
-
     # defining RMSE and MAE
     if performance_metric == "RMSE":
 
         def performance_metric(preds, actuals):
             return np.sqrt(np.nanmean((preds - actuals) ** 2))
 
     elif performance_metric == "MAE":
@@ -233,27 +238,33 @@
     output:
         :return: tuple
             list[str]: list of best-performing column names
             float: performance metric of these variables (i.e. best performing)
     """
 
     data = data.copy()
-    
+
     # first valid index of target variable
     start_index = data.loc[lambda x: ~pd.isna(x[target_variable]), :].index[0]
-    start_index = np.max([0, start_index - n_timesteps + 1]) # where to start the data considering n_timesteps
-    data = data.loc[start_index:, :].reset_index(drop = True)
-    
+    start_index = np.max(
+        [0, start_index - n_timesteps + 1]
+    )  # where to start the data considering n_timesteps
+    data = data.loc[start_index:, :].reset_index(drop=True)
+
     # fold train indices
     end_train_indices = gen_folds(data, n_folds=n_folds, init_test_size=init_test_size)
-    
+
     # check for columns with not enough data for the train set
     shortest_train = data.loc[: end_train_indices[0], :]
-    no_data_cols = [col for col in shortest_train.columns if shortest_train[col].isnull().sum() / len(shortest_train) == 1.0]
-    if (len(no_data_cols) > 0):
+    no_data_cols = [
+        col
+        for col in shortest_train.columns
+        if shortest_train[col].isnull().sum() / len(shortest_train) == 1.0
+    ]
+    if len(no_data_cols) > 0:
         for col in no_data_cols:
             data[col] = 0.0
 
     if initial_ordering == "univariate":
         column_order = univariate_order(
             data,
             target_variable,
@@ -435,15 +446,15 @@
 
         # add this column to final list of performance improved over previous minimum
         if col != column_order[0]:  # only relevant if not first column
             if performance[-1] < np.min(performance[:-1]):
                 end_variables = end_variables + [col]
 
     # ensure can't pick a column with no data
-    end_variables = [col for col in end_variables if col not in no_data_cols]    
+    end_variables = [col for col in end_variables if col not in no_data_cols]
 
     return end_variables, np.min(performance)
 
 
 def hyperparameter_tuning(
     data,
     target_variable,
@@ -478,29 +489,35 @@
         :performance_metric: performance metric to use for variable selection. Pass "RMSE" for root mean square error or "MAE" for mean absolute error, "AICc" for corrected Akaike Information Criterion. Alternatively can pass a function that takes arguments of a pandas Series of predictions and actuals and returns a scalar. E.g. custom_function(preds, actuals).
         :quiet: bool: whether or not to print progress
     output:
         :return: Pandas DataFrame: hyperparameters sorted by best-performing model to least
     """
 
     data = data.copy()
-    
+
     # first valid index of target variable
     start_index = data.loc[lambda x: ~pd.isna(x[target_variable]), :].index[0]
-    start_index = np.max([0, start_index - np.max(n_timesteps_grid) + 1]) # where to start the data considering n_timesteps
-    data = data.loc[start_index:, :].reset_index(drop = True)
+    start_index = np.max(
+        [0, start_index - np.max(n_timesteps_grid) + 1]
+    )  # where to start the data considering n_timesteps
+    data = data.loc[start_index:, :].reset_index(drop=True)
 
     alpha = 0.0  # legacy to work with same variable selection code
 
     # fold train indices
     end_train_indices = gen_folds(data, n_folds=n_folds, init_test_size=init_test_size)
-    
+
     # check for columns with not enough data for the train set
     shortest_train = data.loc[: end_train_indices[0], :]
-    no_data_cols = [col for col in shortest_train.columns if shortest_train[col].isnull().sum() / len(shortest_train) == 1.0]
-    if (len(no_data_cols) > 0):
+    no_data_cols = [
+        col
+        for col in shortest_train.columns
+        if shortest_train[col].isnull().sum() / len(shortest_train) == 1.0
+    ]
+    if len(no_data_cols) > 0:
         for col in no_data_cols:
             data[col] = 0.0
 
     # defining RMSE and MAE
     if performance_metric == "RMSE":
 
         def performance_metric(preds, actuals):
```

### Comparing `nowcast_lstm-0.2.6/nowcast_lstm/modelling.py` & `nowcast_lstm-0.2.7/nowcast_lstm/modelling.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,43 +11,55 @@
     n_timesteps,
     n_hidden=20,
     n_layers=2,
     dropout=0,
     criterion="",
     optimizer="",
     optimizer_parameters={"lr": 1e-2},
+    seed=np.random.randint(0, 1e9),
+    device="cpu",
 ):
     """Create the network, criterion, and optimizer objects necessary for training a model
 
     parameters:
         :model_input: numpy array: output of `gen_model_input` function, first entry in tuple (X)
         :n_timesteps: how many historical periods to consider when training the model. For example if the original data is monthly, n_steps=12 would consider data for the last year.
         :n_hidden: int: number of hidden states in the network
         :n_layers: int: number of LSTM layers in the network
         :dropout: float: dropout rate between the LSTM layers
         :lr: float: learning rate
         :criterion: torch loss criterion, defaults to MAE
         :optimizer: torch optimizer, defaults to Adam
+        :seed: int: torch manual seed for reproducibility
+        :device: str: ["mps", "cuda:0", "cpu"] which device to instantiate the model on
 
     output: Dict
         :mv_lstm: torch network
         :criterion: torch criterion
         :optimizer: torch optimizer
     """
 
     n_features = model_x_input.shape[
         2
     ]  # 3rd axis of the matrix is the number of features
-    
+
     if criterion == "":
         criterion = torch.nn.L1Loss()
-    
+
     mv_lstm = nowcast_lstm.mv_lstm.MV_LSTM(
-        n_features, n_timesteps, n_hidden, n_layers, dropout, criterion
+        n_features,
+        n_timesteps,
+        n_hidden,
+        n_layers,
+        dropout,
+        criterion,
+        seed,
+        device=device,
     )
+    mv_lstm.to(device)
 
     # for generating the optimizer
     def generate_optimizer(model, opt_fn=None, opt_kwargs=optimizer_parameters):
         optimizer = opt_fn(model.parameters(), **opt_kwargs)
         return optimizer
 
     if optimizer == "":
@@ -85,14 +97,15 @@
     optimizer,
     train_episodes=200,
     batch_size=30,
     decay=0.98,
     num_workers=0,
     shuffle=False,
     quiet=False,
+    device="cpu",
 ):
     """Train the network
 
     parameters:
         :X: numpy array: output of `gen_model_input` function, first entry in tuple (X), input variables
         :y: numpy array: output of `gen_model_input` function, second entry in tuple (y), targets
         :mv_lstm: torch network: output of `instantiate_model` function, "mv_lstm" entry
@@ -100,45 +113,44 @@
         :optimizer: torch optimizer: output of `instantiate_model` function, "optimizer" entry, Adam is default
         :train_episodes: int: number of epochs/episodes to train the model
         :batch_size: int: number of observations per training batch
         :decay: float: learning rate decay
         :num_workers: int: number of workers for multi-process data loading
         :shuffle: boolean: whether to shuffle data at every epoch
         :quiet: boolean: whether or not to print the losses in the epoch loop
+        :device: str: ["mps", "cuda:0", "cpu"] which device to instantiate the model on
 
     output:
         :return: Dict
             :mv_lstm: trained network
             :train_loss: list of losses per epoch, for informational purposes
     """
+    torch.manual_seed(mv_lstm.seed)
+    torch.cuda.manual_seed_all(mv_lstm.seed)
+    torch.mps.manual_seed(mv_lstm.seed)
 
-    # CUDA if available
-    use_cuda = torch.cuda.is_available()
-    device = torch.device("cuda:0" if use_cuda else "cpu")
     params = {"batch_size": batch_size, "shuffle": shuffle, "num_workers": num_workers}
 
     # PyTorch dataset
     data_generator = torch.utils.data.DataLoader(
         Dataset(
-            torch.tensor(X, dtype=torch.float32), torch.tensor(y, dtype=torch.float32)
+            torch.tensor(X, dtype=torch.float32, device=device),
+            torch.tensor(y, dtype=torch.float32, device=device),
         ),
         **params
     )
 
     train_loss = []  # for plotting train loss
     my_lr_scheduler = torch.optim.lr_scheduler.ExponentialLR(
         optimizer=optimizer, gamma=decay
     )  # for learning rate decay
 
     mv_lstm.train()
     for t in range(train_episodes):
         for batch_X, batch_y in data_generator:
-            # to GPU
-            batch_X, batch_y = batch_X.to(device), batch_y.to(device)
-
             mv_lstm.init_hidden(batch_X.size(0))
             output = mv_lstm(batch_X)
             loss = criterion(output.view(-1), batch_y)
 
             loss.backward()
             optimizer.step()
             optimizer.zero_grad()
@@ -152,28 +164,33 @@
 
     return {
         "mv_lstm": mv_lstm,
         "train_loss": train_loss,
     }
 
 
-def predict(X, mv_lstm):
+def predict(X, mv_lstm, device="cpu"):
     """Make predictions on a trained network
 
     parameters:
         :X: numpy array: output of `gen_model_input` function, first entry in tuple (X), input variables
         :mv_lstm: torch network: output of `train_model` function, "mv_lstm" entry, trained network
+        :device: str: ["mps", "cuda:0", "cpu"] which device to instantiate the model on
 
     output:
         :return: np array: array of predictions
     """
+    torch.manual_seed(mv_lstm.seed)
+    torch.cuda.manual_seed_all(mv_lstm.seed)
+    torch.mps.manual_seed(mv_lstm.seed)
+
     with torch.no_grad():
-        inpt = torch.tensor(X, dtype=torch.float32)
+        inpt = torch.tensor(X, dtype=torch.float32, device=device)
     mv_lstm.init_hidden(inpt.size(0))
-    preds = mv_lstm(inpt).view(-1).detach().numpy()
+    preds = mv_lstm(inpt).cpu().view(-1).detach().numpy()
 
     return preds
 
 
 def gen_news(model, target_period, old_data, new_data):
     """Generate the news between two data releases using the method of holding out new data feature by feature and recording the differences in model output
     Make sure both the old and new dataset have the target period in them to allow for predictions and news generation.
```

### Comparing `nowcast_lstm-0.2.6/nowcast_lstm/mv_lstm.py` & `nowcast_lstm-0.2.7/nowcast_lstm/mv_lstm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,76 @@
 import torch
 
 
 class MV_LSTM(torch.nn.Module):
-    def __init__(self, n_features, n_timesteps, n_hidden, n_layers, dropout, criterion):
+    def __init__(
+        self,
+        n_features,
+        n_timesteps,
+        n_hidden,
+        n_layers,
+        dropout,
+        criterion,
+        seed,
+        device,
+    ):
         super(MV_LSTM, self).__init__()
         self.n_features = n_features
         self.n_timesteps = n_timesteps
         self.n_hidden = n_hidden
         self.n_layers = n_layers
         self.criterion = criterion
+        self.seed = seed
+        torch.manual_seed(seed)
+        torch.cuda.manual_seed_all(seed)
+        torch.mps.manual_seed(seed)
+        self.device = device
 
         # model layers
         # n_layers stacked LSTM layers + one linear dense layer to get final prediction
         self.l_lstm = torch.nn.LSTM(
             input_size=n_features,
             hidden_size=self.n_hidden,
             num_layers=self.n_layers,
             batch_first=True,
             dropout=dropout,
+            device=self.device,
         )
-        self.l_linear = torch.nn.Linear(self.n_hidden * self.n_timesteps, 1)
-        
+        self.l_linear = torch.nn.Linear(
+            self.n_hidden * self.n_timesteps, 1, device=self.device
+        )
+
         # if binary classifcation, add sigmoid layer and edit forward
         def binary_forward(x):
             batch_size, n_timesteps, _ = x.size()
 
             # model layers
             x, self.hidden = self.l_lstm(x, self.hidden)
             x = x.contiguous().view(batch_size, -1)  # make tensor of right dimensions
             x = self.l_linear(x)
-            
+
             x = torch.sigmoid(x)
             return x
+
         if type(self.criterion) == type(torch.nn.BCELoss()):
             self.forward = binary_forward
 
     # model layers
 
     def init_hidden(self, batch_size):  # initializing hidden layers
-        hidden_state = torch.zeros(self.n_layers, batch_size, self.n_hidden)
-        cell_state = torch.zeros(self.n_layers, batch_size, self.n_hidden)
+        hidden_state = torch.zeros(
+            self.n_layers, batch_size, self.n_hidden, device=self.device
+        )
+        cell_state = torch.zeros(
+            self.n_layers, batch_size, self.n_hidden, device=self.device
+        )
         self.hidden = (hidden_state, cell_state)
-        
+
     def forward(self, x):
         batch_size, n_timesteps, _ = x.size()
 
         # model layers
         x, self.hidden = self.l_lstm(x, self.hidden)
         x = x.contiguous().view(batch_size, -1)  # make tensor of right dimensions
         x = self.l_linear(x)
         # model layers
-        return x
+        return x
```

### Comparing `nowcast_lstm-0.2.6/nowcast_lstm.egg-info/PKG-INFO` & `nowcast_lstm-0.2.7/nowcast_lstm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcast-lstm
-Version: 0.2.6
+Version: 0.2.7
 Summary: Code for running LSTM neural networks on economic data for nowcasting
 Home-page: https://github.com/dhopp1/nowcast_lstm
 Author: Daniel Hopp
 Author-email: daniel.hopp@un.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,26 +43,27 @@
 [LSTM neural networks](https://en.wikipedia.org/wiki/Long_short-term_memory) have been used for nowcasting [before](https://papers.nips.cc/paper/2015/file/07563a3fe3bbe7e3ba84431ad9d055af-Paper.pdf), combining the strengths of artificial neural networks with a temporal aspect. However their use in nowcasting economic indicators remains limited, no doubt in part due to the difficulty of obtaining results in existing deep learning frameworks. This library seeks to streamline the process of obtaining results in the hopes of expanding the domains to which LSTM can be applied.
 
 While neural networks are flexible and this framework may be able to get sensible results on levels, the model architecture was developed to nowcast growth rates of economic indicators. As such training inputs should ideally be stationary and seasonally adjusted.
 
 Further explanation of the background problem can be found in [this paper](https://unctad.org/system/files/official-document/ser-rp-2018d9_en.pdf). Further explanation and results can be found in [this](https://www.researchgate.net/publication/363509881_Economic_Nowcasting_with_Long_Short-Term_Memory_Artificial_Neural_Networks_LSTM) paper in the Journal of Official Statistics.
 
 ## R, MATLAB, and Julia wrappers 
-[R](https://github.com/dhopp1/nowcastLSTM),  [MATLAB](https://github.com/dhopp1/nowcast_lstm_matlab), and [Julia](https://github.com/dhopp1/NowcastLSTM.jl) wrappers exist for this Python library. Python and some Python libraries still need to be installed on your system, but full functionality from R, MATLAB, and Julia can be obtained with the wrappers without any Python knowledge.
+[R](https://github.com/dhopp1/nowcastLSTM),  [MATLAB](https://github.com/dhopp1/nowcast_lstm_matlab), and [Julia](https://github.com/dhopp1/NowcastLSTM.jl) wrappers exist for this Python library. Python and some Python libraries still need to be installed on your system, but full functionality from R can be obtained with the wrappers without any Python knowledge. The MATLAB and Julia wrappers work with older versions of the library but are no longer being mantained and updated to work with the newest features.
 
 
 ## Quick usage
 The main object and functionality of the library comes from the `LSTM` object. Given `data` = a pandas DataFrame of a date column + monthly data + a quarterly target series to run the model on, usage is as follows:
 
 ```python
 from nowcast_lstm.LSTM import LSTM
 
 # note that if a column has no data in it, i.e., is all NAs, its values will be replaced with 0. This won't affect model performance and will ensure that the model can still be trained
 # a list of columns with no data in them can be accessed with `model.no_data_cols`
 model = LSTM(data, "target_col_name", n_timesteps=12) # default parameters with 12 timestep history
+#model = LSTM(data, "target_col_name", n_timesteps=12, n_models=10, seeds=list(range(10)) # For reproducibility on a single machine/system, give a list of manual seeds as long as the n_models parameter. Reproducibility across machines is not guaranteed.
 
 model.X # array of the transformed training dataset
 model.y # array of the target values
 
 model.mv_lstm # list of trained PyTorch network(s)
 model.train_loss # list of training losses for the network(s)
```

### Comparing `nowcast_lstm-0.2.6/setup.py` & `nowcast_lstm-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nowcast_lstm",
-    version="0.2.6",
+    version="0.2.7",
     author="Daniel Hopp",
     author_email="daniel.hopp@un.org",
     description="Code for running LSTM neural networks on economic data for nowcasting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dhopp1/nowcast_lstm",
     packages=setuptools.find_packages(),
```

### Comparing `nowcast_lstm-0.2.6/tests/test_LSTM.py` & `nowcast_lstm-0.2.7/tests/test_LSTM.py`

 * *Files identical despite different names*

### Comparing `nowcast_lstm-0.2.6/tests/test_data_setup.py` & `nowcast_lstm-0.2.7/tests/test_data_setup.py`

 * *Files identical despite different names*

### Comparing `nowcast_lstm-0.2.6/tests/test_modelling.py` & `nowcast_lstm-0.2.7/tests/test_modelling.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,14 @@
         model = result["mv_lstm"]
         crit = result["criterion"]
         opt = result["optimizer"]
         model_result = modelling.train_model(
             model_input[0], model_input[1], model, crit, opt, quiet=True
         )
         model = model_result["mv_lstm"]
-        preds = modelling.predict(model_input[0], model)
+        preds = modelling.predict(model_input[0], model, model.device)
 
         self.assertEqual(len(preds), 2)
 
 
 if __name__ == "__main__":
     unittest.main()
```

