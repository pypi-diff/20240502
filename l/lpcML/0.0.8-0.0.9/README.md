# Comparing `tmp/lpcML-0.0.8.tar.gz` & `tmp/lpcML-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpcML-0.0.8.tar", last modified: Tue Apr 30 10:59:04 2024, max compression
+gzip compressed data, was "lpcML-0.0.9.tar", last modified: Thu May  2 08:03:54 2024, max compression
```

## Comparing `lpcML-0.0.8.tar` & `lpcML-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:59:04.256729 lpcML-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)    35165 2024-04-30 10:58:51.000000 lpcML-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1624 2024-04-30 10:59:04.256729 lpcML-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      879 2024-04-30 10:58:51.000000 lpcML-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 10:59:04.256729 lpcML-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-30 10:58:51.000000 lpcML-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:59:04.256729 lpcML-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:59:04.256729 lpcML-0.0.8/src/lpcML/
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-30 10:58:51.000000 lpcML-0.0.8/src/lpcML/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6817 2024-04-30 10:58:51.000000 lpcML-0.0.8/src/lpcML/data_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2024-04-30 10:58:51.000000 lpcML-0.0.8/src/lpcML/model.py
--rw-rw-rw-   0 root         (0) root         (0)     4175 2024-04-30 10:58:51.000000 lpcML-0.0.8/src/lpcML/model_fitting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:59:04.256729 lpcML-0.0.8/src/lpcML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1624 2024-04-30 10:59:04.000000 lpcML-0.0.8/src/lpcML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      287 2024-04-30 10:59:04.000000 lpcML-0.0.8/src/lpcML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 10:59:04.000000 lpcML-0.0.8/src/lpcML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-30 10:59:04.000000 lpcML-0.0.8/src/lpcML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-30 10:59:04.000000 lpcML-0.0.8/src/lpcML.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:03:54.549474 lpcML-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    35165 2024-05-02 08:03:42.000000 lpcML-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-05-02 08:03:54.549474 lpcML-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      879 2024-05-02 08:03:42.000000 lpcML-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 08:03:54.549474 lpcML-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2024-05-02 08:03:42.000000 lpcML-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:03:54.549474 lpcML-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:03:54.549474 lpcML-0.0.9/src/lpcML/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-02 08:03:42.000000 lpcML-0.0.9/src/lpcML/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7463 2024-05-02 08:03:42.000000 lpcML-0.0.9/src/lpcML/data_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2024-05-02 08:03:42.000000 lpcML-0.0.9/src/lpcML/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4210 2024-05-02 08:03:42.000000 lpcML-0.0.9/src/lpcML/model_fitting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:03:54.549474 lpcML-0.0.9/src/lpcML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-05-02 08:03:54.000000 lpcML-0.0.9/src/lpcML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      287 2024-05-02 08:03:54.000000 lpcML-0.0.9/src/lpcML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 08:03:54.000000 lpcML-0.0.9/src/lpcML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-02 08:03:54.000000 lpcML-0.0.9/src/lpcML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-02 08:03:54.000000 lpcML-0.0.9/src/lpcML.egg-info/top_level.txt
```

### Comparing `lpcML-0.0.8/LICENSE` & `lpcML-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.8/PKG-INFO` & `lpcML-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpcML
-Version: 0.0.8
+Version: 0.0.9
 Summary: LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `lpcML-0.0.8/README.md` & `lpcML-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.8/setup.py` & `lpcML-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     long_description=''
     with open(Path(Path(__file__).parent,'README.md'), 'r') as fh:
         long_description=fh.read()
     return long_description
 
 setuptools.setup(
     name='lpcML',
-    version='0.0.8',
+    version='0.0.9',
     description='LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='Julian Garcia Fernandez ',
     author_email='julian.garcia.fernandez2@usc.es',
     url='https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML',
     setup_requires=['setuptools'],
-    install_requires=['torch','pytorch_lightning','wandb','numpy','pandas','scikit-learn','pathlib'],
+    install_requires=['torch','pytorch_lightning','wandb','numpy','pandas','scikit-learn','torcheval','pathlib'],
     package_dir={"":"src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     classifiers=[
         'Topic :: Utilities',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
```

### Comparing `lpcML-0.0.8/src/lpcML/data_processing.py` & `lpcML-0.0.9/src/lpcML/data_processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pathlib import Path
 from pickle import dump
+import os
 
 import pandas as pd 
 import matplotlib.pyplot as plt
 import torch
 from torcheval.metrics.functional import mean_squared_error
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import  StandardScaler, MinMaxScaler
@@ -23,32 +24,40 @@
     -------
     data: pandas dataframe 
         dataframe with data
     '''
     data = pd.read_csv(path, delimiter=delimiter)
     return data
 
-def data_to_input_output_tensors(data, verbosity=False):
+def data_to_input_output_tensors(data, input_param=None, output_param=None, verbosity=False):
     '''Preprocessing function that creates the input and output tensors
     ---------
     Input:
     -----
     data: pd.Dataframe
         hLPC optimization data
+    input_param: list
+        list of input parameters used to tain de neural network, ['C1_up2_thick','C1_up2_dop','C1_down1_thick','C1_down1_dop','wavelength'] by default
+    output_param: list
+        list of output parameter(s) used to tain de neural network, ['Eff'] by default
     verbosity: bool
         Print information about the final scaled tensors
     Output:
     ------
     X_list: torch.tensor
         Input tensor
     Y_list: torch.tensor
         Output tensor
     '''
-    df_inputs = pd.DataFrame(data, columns=['C1_up2_thick','C1_up2_dop','C1_down1_thick','C1_down1_dop','wavelength'])
-    df_outputs = pd.DataFrame(data, columns=['Eff'])
+    if not input_param:
+        input_param = ['C1_up2_thick','C1_up2_dop','C1_down1_thick','C1_down1_dop','wavelength']
+    if not output_param:
+        output_param = ['Eff']
+    df_inputs = pd.DataFrame(data, columns=input_param)
+    df_outputs = pd.DataFrame(data, columns=output_param)
     X_list, Y_list = df_inputs.to_numpy(), df_outputs.to_numpy()
     if verbosity:
         print("Total size\n","\tInput:", torch.tensor(X_list, dtype=torch.float32).shape,"\tOutput:",torch.tensor(Y_list, dtype=torch.float32).shape)
     return torch.tensor(X_list, dtype=torch.float32), torch.tensor(Y_list, dtype=torch.float32)
 
 
 def split_data(X, Y, test_split = 0.2, verbosity=False):
@@ -105,15 +114,18 @@
     if scaler == 'standard':
         scaler_inputs = StandardScaler()
     elif scaler == 'minmax':
         scaler_inputs = MinMaxScaler()
     X_train_scaled = scaler_inputs.fit_transform(X_train)
     X_val_scaled = scaler_inputs.transform(X_val)
     X_test_scaled = scaler_inputs.transform(X_test)
-    dump(scaler_inputs, open('scaler_objects/scaler_inputs.pkl', 'wb'))
+    directory =  'scaler_objects/'
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+    dump(scaler_inputs, open(directory+'scaler_inputs.pkl', 'wb'))
     return torch.tensor(X_train_scaled, dtype=torch.float32), torch.tensor(X_val_scaled, dtype=torch.float32), torch.tensor(X_test_scaled, dtype=torch.float32), scale_input
 
 
 def scale_output(Y_train, Y_val, Y_test, scaler='standard'):
     '''Preprocessing function that normalize the input and output of the neural network and store the scalers
     ---------
     Input:
@@ -136,15 +148,18 @@
     if scaler == 'standard':
         scaler_output = StandardScaler()
     elif scaler == 'minmax':
         scaler_output = MinMaxScaler()
     Y_train_scaled = scaler_output.fit_transform(Y_train)
     Y_val_scaled = scaler_output.transform(Y_val)
     Y_test_scaled = scaler_output.transform(Y_test)
-    dump(scaler_output, open('scaler_objects/scaler_output.pkl', 'wb'))
+    directory =  'scaler_objects/'
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+    dump(scale_output, open(directory+'scaler_output.pkl', 'wb'))
     return torch.tensor(Y_train_scaled, dtype=torch.float32), torch.tensor(Y_val_scaled, dtype=torch.float32), torch.tensor(Y_test_scaled, dtype=torch.float32), scaler_output
 
 
 def prediction_versus_simulation_plot(simulation, prediction, r2, xlabel = None, ylabel = None, rms = None, storepath = None):
     '''Plot for the comparison of the simulated versus predicted data with machine learning
     --------------------
     Parameters:
```

### Comparing `lpcML-0.0.8/src/lpcML/model.py` & `lpcML-0.0.9/src/lpcML/model.py`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.8/src/lpcML/model_fitting.py` & `lpcML-0.0.9/src/lpcML/model_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         trainer = pl.Trainer(accelerator="cpu",max_epochs=self.num_epochs, log_every_n_steps = math.floor(len(X_train)/self.config["batch_size"]), callbacks=[early_stopping]) # Init Lightning trainer callbacks=[early_stopping]
         trainer.fit(self.model, train_loader, val_loader)
         if wandb.run is not None:
             wandb.finish()
         elapsed_time = round(time() - start_time,2)
         if self.verbosity == True:
             print('Trainer time:', elapsed_time)
-            print(self.config)
+            print('The defined hyperparmaters are:', self.config)
 
 
     def test(self, X_test, Y_test, scaler_output):
         with torch.no_grad():
             y_hat = self.model(X_test)
         pred = scaler_output.inverse_transform(y_hat)
         sim = scaler_output.inverse_transform(Y_test)
```

### Comparing `lpcML-0.0.8/src/lpcML.egg-info/PKG-INFO` & `lpcML-0.0.9/src/lpcML.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpcML
-Version: 0.0.8
+Version: 0.0.9
 Summary: LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

