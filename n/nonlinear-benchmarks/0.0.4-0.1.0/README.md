# Comparing `tmp/nonlinear_benchmarks-0.0.4.tar.gz` & `tmp/nonlinear_benchmarks-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonlinear_benchmarks-0.0.4.tar", last modified: Mon Feb 19 11:11:10 2024, max compression
+gzip compressed data, was "nonlinear_benchmarks-0.1.0.tar", last modified: Thu May  2 14:27:09 2024, max compression
```

## Comparing `nonlinear_benchmarks-0.0.4.tar` & `nonlinear_benchmarks-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-19 11:11:10.362000 nonlinear_benchmarks-0.0.4/
--rw-rw-rw-   0        0        0     1505 2023-10-17 14:32:40.000000 nonlinear_benchmarks-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3817 2024-02-19 11:11:10.339000 nonlinear_benchmarks-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2927 2024-02-19 10:36:32.000000 nonlinear_benchmarks-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-19 11:11:10.082000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks/
--rw-rw-rw-   0        0        0      265 2024-02-19 10:30:03.000000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks/__init__.py
--rw-rw-rw-   0        0        0    10457 2023-10-27 07:56:07.000000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks/benchmarks.py
--rw-rw-rw-   0        0        0     5550 2024-02-19 10:29:13.000000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks/error_metrics.py
--rw-rw-rw-   0        0        0    11755 2023-10-20 15:27:18.000000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks/not_splitted_benchmarks.py
--rw-rw-rw-   0        0        0     7823 2023-10-18 10:54:20.000000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks/utilities.py
-drwxrwxrwx   0        0        0        0 2024-02-19 11:11:10.292000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks.egg-info/
--rw-rw-rw-   0        0        0     3817 2024-02-19 11:11:09.000000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2024-02-19 11:11:09.000000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-19 11:11:09.000000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-02-19 11:11:09.000000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-02-19 11:11:09.000000 nonlinear_benchmarks-0.0.4/nonlinear_benchmarks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      807 2024-02-19 11:11:10.360000 nonlinear_benchmarks-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      810 2024-02-19 11:08:56.000000 nonlinear_benchmarks-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 14:27:09.096000 nonlinear_benchmarks-0.1.0/
+-rw-rw-rw-   0        0        0     1505 2023-10-17 14:32:40.000000 nonlinear_benchmarks-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5291 2024-05-02 14:27:09.029000 nonlinear_benchmarks-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4403 2024-05-02 14:26:00.000000 nonlinear_benchmarks-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 14:27:08.800000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks/
+-rw-rw-rw-   0        0        0      891 2024-05-01 15:03:51.000000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks/__init__.py
+-rw-rw-rw-   0        0        0    12266 2024-05-02 13:21:11.000000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks/benchmarks.py
+-rw-rw-rw-   0        0        0     5603 2024-02-19 11:29:22.000000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks/error_metrics.py
+-rw-rw-rw-   0        0        0    12335 2024-05-01 15:29:12.000000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks/not_splitted_benchmarks.py
+-rw-rw-rw-   0        0        0     9138 2024-05-02 13:33:59.000000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-02 14:27:09.001000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks.egg-info/
+-rw-rw-rw-   0        0        0     5291 2024-05-02 14:27:08.000000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2024-05-02 14:27:08.000000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 14:27:08.000000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-02 14:27:08.000000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-02 14:27:08.000000 nonlinear_benchmarks-0.1.0/nonlinear_benchmarks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      807 2024-05-02 14:27:09.093000 nonlinear_benchmarks-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      810 2024-05-02 14:25:59.000000 nonlinear_benchmarks-0.1.0/setup.py
```

### Comparing `nonlinear_benchmarks-0.0.4/LICENSE` & `nonlinear_benchmarks-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonlinear_benchmarks-0.0.4/PKG-INFO` & `nonlinear_benchmarks-0.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,115 @@
-Metadata-Version: 2.1
-Name: nonlinear_benchmarks
-Version: 0.0.4
-Summary: The official dataload for http://www.nonlinearbenchmark.org/
-Home-page: https://github.com/GerbenBeintema/nonlinear_benchmarks
-Author: Gerben Beintema
-Author-email: g.i.beintema@tue.nl
-License: BSD 3-Clause License
-Project-URL: Bug Tracker, https://github.com/GerbenBeintema/nonlinear_benchmarks/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: tqdm
-Requires-Dist: progressbar
-Requires-Dist: scipy
-Requires-Dist: requests
-Requires-Dist: rarfile
-Provides-Extra: docs
-Requires-Dist: sphinx>=1.6; extra == "docs"
-Requires-Dist: sphinx-rtd-theme>=0.5; extra == "docs"
-
 
 # nonlinear_benchmarks
  
-The official dataloader of [nonlinearbenchmark.org](http://www.nonlinearbenchmark.org/). This toolbox can automatically download, load and split many of the datasets which can be found on the website. 
+The official dataloader of [nonlinearbenchmark.org](http://www.nonlinearbenchmark.org/). This toolbox simplifies the process of downloading, loading, and splitting various datasets available on the website.
+
+## Usage Example
 
-For intance, https://www.nonlinearbenchmark.org/benchmarks/wiener-hammerstein.
+https://www.nonlinearbenchmark.org/benchmarks/wiener-hammerstein is loaded as:
 
 ```python
 import nonlinear_benchmarks
 train_val, test = nonlinear_benchmarks.WienerHammerBenchMark()
-sampling_time = train_val.sampling_time #in seconds
-u_train, y_train = train_val #or train_val.u, train_val.y
-u_test, y_test = test        #or test.u,      test.y
-```
 
-In the `WienerHammerBenchMark` multiple options are provided. You can find the data files by using `raw_data=True` and obtain the entire, not train-test splitted, dataset by using `train_test_split=False`.
+print(train_val) 
+# prints : Input_output_data "train WH" u.shape=(100000,) y.shape=(100000,)
+#          sampling_time=1.953e-05
+print(test)
+# prints: Input_output_data "test WH" u.shape=(78800,) y.shape=(78800,) 
+#         sampling_time=1.953e-05 n_initialization_samples=50
+
+sampling_time = train_val.sampling_time #in seconds
+u_train, y_train = train_val  #or train_val.u, train_val.y
+u_test, y_test = test         #or test.u,      test.y
+print(test.n_initialization_samples) 
+#n_initialization_samples = The number of samples that can be used at the 
+#                           start of the test set to initialize the model state.
+```
+
+## Useful Options
+
+When using the `WienerHammerBenchMark` (or any other benchmark function), you can customize the behavior with the following options:
+
+ * `data_file_locations=True`: Returns the raw data file locations.
+ * `train_test_split=False`: Retrieves the entire dataset without splitting.
+ * `force_download=True`: Forces (re-)downloading of benchmark files.
+ * `url=` : Allows manual override of the download link (contact maintainers if the default link is broken).
+ * `atleast_2d=True`: Converts input/output arrays to at least 2D shape (e.g., `u.shape = (250,)` becomes `u.shape = (250, 1)`).
 
 # Install
 
 ```
 pip install nonlinear-benchmarks
 ```
 
 # Datasets
 
-Multiple datasets have been implemented with an official train test split which are given below. (p.s. datasets without a official train test split can be found in `nonlinear_benchmarks.not_splitted_benchmarks`)
+Multiple datasets have been implemented with an official train test split which are given below. 
+
+(p.s. datasets without an official train test split can be found in `nonlinear_benchmarks.not_splitted_benchmarks`)
 
 ## EMPS
 
 ![image](figures/EMPS.jpg)
 
 ```python
 train_val, test = nonlinear_benchmarks.EMPS()
+print(test.n_initialization_samples) # = 20
 train_val_u, train_val_y = train_val
 test_u, test_y = test
 ```
 
 ## CED
 
 ![image](figures/CED.jpg)
 
 ```python
 train_val, test = nonlinear_benchmarks.CED()
+print(test[0].n_initialization_samples) # = 4
 (train_val_u_1, train_val_y_1), (train_val_u_2, train_val_y_2) = train_val
 (test_u_1, test_y_1), (test_u_2, test_y_2) = test
 ```
 
+This dataset consists of two time series where the first has a low input amplitude (`train_val_1` and `test_1`) and the second a high input amplitude (`train_val_2` and `test_2`).  
+
+You can use both training sets in your training, and please report the RMSE values on both test sets separately. 
+
 ## Cascaded_Tanks
 
 ![image](figures/Cascaded_Tanks.jpg)
 
 ```python
 train_val, test = nonlinear_benchmarks.Cascaded_Tanks()
+print(test.n_initialization_samples) # = 4
 train_val_u, train_val_y = train_val
 test_u, test_y = test
 ```
 
 
 ## WienerHammerBenchMark
 
 ![image](figures/WienerHammerBenchMark.jpg)
 
 ```python
 train_val, test = nonlinear_benchmarks.WienerHammerBenchMark()
+print(test.n_initialization_samples) # = 50
 train_val_u, train_val_y = train_val
 test_u, test_y = test
 ```
 
 
 ## Silverbox
 
 ![image](figures/Silverbox.jpg)
 
 ```python
 train_val, test = nonlinear_benchmarks.Silverbox()
 multisine_train_val = train_val
+print(test[0].n_initialization_samples) # = 50 (for all test sets)
 test_multisine, test_arrow_full, test_arrow_no_extrapolation = test
 ```
 
 Note that the test arrow full and the test arrow no extrapolation have some overlap.
 
 # Error Metrics
```

### Comparing `nonlinear_benchmarks-0.0.4/nonlinear_benchmarks/benchmarks.py` & `nonlinear_benchmarks-0.1.0/nonlinear_benchmarks/benchmarks.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from scipy.io import loadmat
 import tempfile
 import os.path
 from pathlib import Path
 from nonlinear_benchmarks.utilities import *
 import numpy as np
 
-def EMPS(train_test_split=True, raw_data=False, dir_placement=None, force_download=False, url=None):
+def EMPS(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, atleast_2d=False):
     '''The Electro-Mechanical Positioning System is a standard configuration of a drive system for prismatic joint of robots or machine tools. The main source of nonlinearity is caused by friction effects that are present in the setup. Due to the presence of a pure integrator in the system, the measurements are obtained in a closed-loop setting.
 
     The provided data is described in this link. The provided Electro-Mechanical Positioning System datasets are available for download here. This zip-file contains the system description and available data sets .mat file format.
 
     Please refer to the Electro-Mechanical Positioning System as:
 
     A. Janot, M. Gautier and M. Brunot, Data Set and Reference Models of EMPS, 2019 Workshop on Nonlinear System Identification Benchmarks, Eindhoven, The Netherlands, April 10-12, 2019.
@@ -29,32 +29,33 @@
     #vir applied the vector of motor force expressed in the load side i.e. in N;
 
     # url = 'http://www.nonlinearbenchmark.org/FILES/BENCHMARKS/EMPS/EMPS.zip'
     url = 'https://drive.google.com/file/d/1zwoXYa9-3f8NQ0ohzmjpF7UxbNgRTHkS/view' if url is None else url
     download_size = 1949929
     save_dir = cashed_download(url,'EMPS',zip_name='EMPS.zip', dir_placement=dir_placement,download_size=download_size,force_download=force_download)
 
-    if raw_data:
+    if data_file_locations:
         return [os.path.join(save_dir,name) for name in ['DATA_EMPS.mat','DATA_EMPS_PULSES.mat']]
 
     datasets = []
-    for name in ['DATA_EMPS.mat','DATA_EMPS_PULSES.mat']:
-        matfile = loadmat(os.path.join(save_dir,name))
+    for name, file_name in [('train (DATA_EMPS)','DATA_EMPS.mat'),('test (DATA_EMPS_PULSES)','DATA_EMPS_PULSES.mat')]:
+        matfile = loadmat(os.path.join(save_dir,file_name))
         q_cur, q_ref, t, vir = [matfile[a][:,0] for a in ['qm','qg','t','vir']] #qg is reference, either, q_ref is input or vir is input
-        out_data = Input_output_data(u=vir, y=q_cur, sampling_time=t[1]-t[0])
+        out_data = Input_output_data(u=vir, y=q_cur, sampling_time=t[1]-t[0], name=name)
         datasets.append(out_data)
 
     if train_test_split:
         train_val = datasets[0]
         test = datasets[1]
-        return train_val, test
+        test.n_initialization_samples = 20
+        return atleast_2d_fun(train_val, test, apply=atleast_2d)
     else:
-        return datasets
+        return atleast_2d_fun(datasets, apply=atleast_2d)
 
-def CED(train_test_split=True, raw_data=False, dir_placement=None, force_download=False, url=None):
+def CED(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, atleast_2d=False):
     '''The coupled electric drives consists of two electric motors that drive a pulley using a flexible belt. 
     The pulley is held by a spring, resulting in a lightly damped dynamic mode. The electric drives can
     be individually controlled allowing the tension and the speed of the belt to be simultaneously controlled. 
     The drive control is symmetric around zero, hence both clockwise and counter clockwise movement is possible.
     The focus is only on the speed control system. The angular speed of the pulley is measured as an output with
     a pulse counter and this sensor is insensitive to the sign of the velocity. The available data sets are short,
     which constitute a challenge when performing identification.
@@ -81,68 +82,82 @@
 
     #http://www.it.uu.se/research/publications/reports/2017-024/2017-024-nc.pdf
     url = 'http://www.it.uu.se/research/publications/reports/2017-024/CoupledElectricDrivesDataSetAndReferenceModels.zip' if url is None else url
     download_size= 278528
     save_dir = cashed_download(url,'CED',dir_placement=dir_placement,download_size=download_size,force_download=force_download)
 
     d = os.path.join(save_dir,'DATAUNIF.MAT')
-    if raw_data:
+    if data_file_locations:
         return d
 
     matfile = loadmat(d)
     u11, u12, z11, z12 = [matfile[a][:,0] for a in ['u11','u12','z11','z12']]
-    datasets = [Input_output_data(u=u11, y=z11, sampling_time=0.02), Input_output_data(u=u12,y=z12, sampling_time=0.02)]
+    datasets = [Input_output_data(u=u11, y=z11, sampling_time=0.02, name='CED low input amplitude'), \
+                Input_output_data(u=u12,y=z12, sampling_time=0.02, name='CED high input amplitude')]
 
     if train_test_split:
         train_val = datasets[0][:400], datasets[1][:400]
+        train_val[0].name = 'train CED low input amplitude'
+        train_val[1].name = 'train CED high input amplitude'
         test = datasets[0][400:], datasets[1][400:]
-        return train_val, test
+        test[0].name = 'test CED low input amplitude'
+        test[1].name = 'test CED high input amplitude'
+        test[0].n_initialization_samples = 4
+        test[1].n_initialization_samples = 4
+        return atleast_2d_fun(train_val, test, apply=atleast_2d)
     else:
-        return datasets
+        return atleast_2d_fun(datasets, apply=atleast_2d)
 
-def Cascaded_Tanks(train_test_split=True, raw_data=False, dir_placement=None, force_download=False, url=None):
+def Cascaded_Tanks(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, atleast_2d=False):
     #does not work anymore?
     # url = 'https://data.4tu.nl/file/d4810b78-6cdd-48fe-8950-9bd601e5f47f/3b697e42-01a4-4979-a370-813a456c36f5' if url is None else url
     url = 'https://drive.google.com/file/d/1HnQf_gu0g_UlggoBqy2s34l9YJiFdN01/view' if url is None else url
     download_size = 7520592
-    save_dir = cashed_download(url,'Cascaded_Tanks',zip_name='CascadedTanksFiles.zip',dir_placement=dir_placement,download_size=download_size,force_download=force_download)
+    save_dir = cashed_download(url, 'Cascaded_Tanks', zip_name='CascadedTanksFiles.zip',dir_placement=dir_placement,download_size=download_size,force_download=force_download)
     save_dir = os.path.join(save_dir,'CascadedTanksFiles')
 
     d = os.path.join(save_dir,'dataBenchmark.mat')
-    if raw_data:
+    if data_file_locations:
         return d
     out = loadmat(d)
 
     uEst, uVal, yEst, yVal, Ts = out['uEst'][:,0],out['uVal'][:,0],out['yEst'][:,0],out['yVal'][:,0],out['Ts'][0,0]
-    datasets = [Input_output_data(u=uEst,y=yEst, sampling_time=Ts),Input_output_data(u=uVal,y=yVal, sampling_time=Ts)]
+    datasets = [Input_output_data(u=uEst,y=yEst, sampling_time=Ts, name='train Cascaded_Tanks'),\
+                Input_output_data(u=uVal,y=yVal, sampling_time=Ts, name='test Cascaded_Tanks')]
     if train_test_split:
         train_val = datasets[0]
         test = datasets[1]
-        return train_val, test
+        test.n_initialization_samples = 5
+        return atleast_2d_fun(train_val, test, apply=atleast_2d)
     else:
-        return datasets
+        datasets[0].name, datasets[1].name = 'Cascaded_Tanks first dataset', 'Cascaded_Tanks second dataset'
+        return atleast_2d_fun(datasets, apply=atleast_2d)
 
-def WienerHammerBenchMark(train_test_split=True, raw_data=False, dir_placement=None, force_download=False, url=None):
+def WienerHammerBenchMark(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, atleast_2d=False):
     url = 'http://www.ee.kth.se/~hjalmars/ifac_tc11_benchmarks/2009_wienerhammerstein/WienerHammerBenchMark.mat' if url is None else url
     download_size=1707601
     save_dir = cashed_download(url,'WienerHammerBenchMark',dir_placement=dir_placement,download_size=download_size,force_download=force_download,zipped=False)
 
-    if raw_data:
+    if data_file_locations:
         return os.path.join(save_dir,'WienerHammerBenchMark.mat')
 
     out = loadmat(os.path.join(save_dir,'WienerHammerBenchMark.mat'))
     u,y,fs = out['uBenchMark'][:,0], out['yBenchMark'][:,0], out['fs'][0,0]
-    full_data = Input_output_data(u=u,y=y, sampling_time=1/fs)
+    full_data = Input_output_data(u=u,y=y, sampling_time=1/fs, name='WH benchmark full')
     if train_test_split==False:
-        return full_data
+        return atleast_2d_fun(full_data, apply=atleast_2d)
     
     sys_data = full_data[5200:184000] 
-    return (sys_data[:100000], sys_data[100000:]) if train_test_split else sys_data
+    train, test = sys_data[:100000], sys_data[100000:]
+    train.name = 'train WH'
+    test.name = 'test WH'
+    test.n_initialization_samples = 50
+    return atleast_2d_fun(train, test, apply=atleast_2d)
 
-def Silverbox(train_test_split=True, raw_data=False, dir_placement=None, force_download=False, url=None):
+def Silverbox(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None, atleast_2d=False):
     '''The Silverbox system can be seen as an electronic implementation of the Duffing oscillator. It is build as a 
     2nd order linear time-invariant system with a 3rd degree polynomial static nonlinearity around it in feedback. 
     This type of dynamics are, for instance, often encountered in mechanical systems.
 
     The provided data is part of a previously published ECC paper available online. A technical note describing the 
     Silverbox benchmark can be found here. All the provided data (.mat file format) on the Silverbox system is available
     for download here. This .zip file contains the Silverbox dataset as specified in the benchmark document (V1 is the
@@ -162,29 +177,34 @@
     url = 'https://drive.google.com/file/d/17iS-6oBUUgrmiAcrZoG9S5sOaljZnDSy/view' if url is None else url
     download_size=5793999
     save_dir = cashed_download(url, 'Silverbox', zip_name='SilverboxFiles.zip',\
         dir_placement=dir_placement, download_size=download_size, force_download=force_download)
     save_dir = os.path.join(save_dir,'SilverboxFiles') #matfiles location
 
     d1, d2 = os.path.join(save_dir,'Schroeder80mV.mat'), os.path.join(save_dir,'SNLS80mV.mat')
-    if raw_data:
+    if data_file_locations:
         return d1, d2
 
     out = loadmat(d2) #train test
     u,y = out['V1'][0], out['V2'][0]
-    data2 = Input_output_data(u=u,y=y, sampling_time=1/610.35)
+    data2 = Input_output_data(u=u,y=y, sampling_time=1/610.35, name='Silverbox Data All')
 
     if train_test_split:
         test_arrow_full = data2[100:40575]
+        test_arrow_full.name = 'test SB multisine'
         test_arrow_no_extrapolation = test_arrow_full[:32000] #keep init=50
-
+        test_arrow_no_extrapolation.name = 'test SB arrow no extrapolation'
 
         multisine = data2[40650:127400]
         s = int(len(multisine)*0.75)
         multisine_train_val, test_multisine = multisine[:s], multisine[s:]
+        multisine_train_val.name = 'train SB multisine'
+        test_multisine.name = 'test SB multisine'
+        for v in [test_multisine, test_arrow_full, test_arrow_no_extrapolation]:
+            v.n_initialization_samples = 50
 
         from collections import namedtuple
-        m = namedtuple('Silverbox_data_splits', ['test_multisine', 'test_arrow_full', 'test_arrow_no_extrapolation'])
-        return multisine_train_val, m(test_multisine, test_arrow_full, test_arrow_no_extrapolation)
+        # m = namedtuple('Silverbox_data_splits', ['test_multisine', 'test_arrow_full', 'test_arrow_no_extrapolation'])
+        return atleast_2d_fun(multisine_train_val, (test_multisine, test_arrow_full, test_arrow_no_extrapolation), apply=atleast_2d)
     else:
-        return data2
+        return atleast_2d_fun(data2, apply=atleast_2d)
```

### Comparing `nonlinear_benchmarks-0.0.4/nonlinear_benchmarks/error_metrics.py` & `nonlinear_benchmarks-0.1.0/nonlinear_benchmarks/error_metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-#error_mean does not seem useful
+#adapted from https://github.com/forgi86/pytorch-ident/blob/master/torchid/metrics.py
 
 def RMSE(y_true, y_pred, time_axis=0):
     """ Computes the Root Mean Square Error (RMSE) (also called RMS).
 
     The RMSE index is computed separately on each channel as:
     RMSE = np.sqrt(np.mean((y_pred - y_true)**2, axis=time_axis))
```

### Comparing `nonlinear_benchmarks-0.0.4/nonlinear_benchmarks/not_splitted_benchmarks.py` & `nonlinear_benchmarks-0.1.0/nonlinear_benchmarks/not_splitted_benchmarks.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import tempfile
 import os.path
 from pathlib import Path
 from nonlinear_benchmarks.utilities import *
 import numpy as np
 
 
-def BoucWen(train_test_split=True, raw_data=False, dir_placement=None, force_download=False, url=None):
+def BoucWen(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None):
 
     #todo: dot p file integration as system for training data
     #generate more data
     # url = 'http://www.nonlinearbenchmark.org/FILES/BENCHMARKS/BOUCWEN/BoucWenFiles.zip'
-    url = 'https://data.4tu.nl/ndownloader/files/24703124'
-    download_size = 5284363
-    save_dir = cashed_download(url,'BoucWen',zip_name='BoucWenFiles.zip',dir_placement=dir_placement,download_size=download_size,force_download=force_download)
+    # url = 'https://data.4tu.nl/ndownloader/items/7060f9bc-8289-411e-8d32-57bef2740d32/versions/1'
+    url = 'https://data.4tu.nl/file/7060f9bc-8289-411e-8d32-57bef2740d32/cd40469c-5064-4968-ae59-88cbb850264b' if url is None else url
+    download_size = 5649141
+    save_dir = cashed_download(url,'BoucWen',zip_name='Hysteretic Benchmark with a Dynamic Nonlinearity_1_all.zip',dir_placement=dir_placement,download_size=download_size,force_download=force_download)
     save_dir = os.path.join(save_dir,'BoucWenFiles/Test signals/Validation signals') #matfiles location
-    if raw_data:
+    if data_file_locations:
         return save_dir
 
     if train_test_split==True:
         print('Warning no offical train and test split has been determined for this dataset')
     
     datafiles = []
 
@@ -36,27 +37,27 @@
     u_sinesweep = out['uval_sinesweep'][0]
     out = loadmat(os.path.join(save_dir,'yval_sinesweep.mat'))
     y_sinesweep = out['yval_sinesweep'][0]
     datafiles.append(Input_output_data(u=u_sinesweep,y=y_sinesweep))
     return datafiles
 
 
-def WienerHammerstein_Process_Noise(train_test_split=True, raw_data=False, dir_placement=None, force_download=False, url=None):
+def WienerHammerstein_Process_Noise(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None):
     '''Warning this is a quite a bit of data'''
     # url = 'http://www.nonlinearbenchmark.org/FILES/BENCHMARKS/WIENERHAMMERSTEINPROCESS/WienerHammersteinFiles.zip'
-    url = 'https://data.4tu.nl/ndownloader/files/24671987'
+    url = 'https://data.4tu.nl/file/1f194001-affa-4459-870a-ad9e9d9146f9/2dbbc046-1ac2-43b2-bf4e-53b5a4be8b96' if url is None else url
     download_size=423134764
     save_dir = cashed_download(url,'WienHammer',zip_name='WienerHammersteinFiles.zip',dir_placement=dir_placement,download_size=download_size,force_download=force_download)
     save_dir = os.path.join(save_dir,'WienerHammersteinFiles') #matfiles location
     matfiles = [os.path.join(save_dir,a).replace('\\','/') for a in os.listdir(save_dir) if a.split('.')[-1]=='mat']
 
     if train_test_split==True:
         print('Warning no offical train and test split has been determined for this dataset')
 
-    if raw_data:
+    if data_file_locations:
         return matfiles
     
     dataset = []
     dataset_test = []
 
     #file = 'WH_CombinedZeroMultisineSinesweep.mat' #'WH_Triangle_meas.mat'
     for file in matfiles:
@@ -68,23 +69,23 @@
             dataset_test.extend(data)
         else:
             dataset.extend(data)
     return dataset, dataset_test
 
 
 
-def ParWHF(train_test_split=True, raw_data=False, dir_placement=None, force_download=False, url=None):
+def ParWHF(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None):
     '''Parallel Wienner-Hammerstein'''
     # url = 'http://www.nonlinearbenchmark.org/FILES/BENCHMARKS/PARWH/ParWHFiles.zip'
-    url = 'https://data.4tu.nl/ndownloader/files/24666227' if url is None else url
+    url = 'https://data.4tu.nl/file/5edca002-b132-4985-b8b9-2353c6e85292/2aaf0790-9ade-43d5-a718-39062524fc93' if url is None else url
     download_size=58203304
     save_dir = cashed_download(url,'ParWHF',zip_name='ParWHFiles.zip',dir_placement=dir_placement,download_size=download_size,force_download=force_download)
     save_dir = os.path.join(save_dir,'ParWHFiles') #matfiles location
     d = os.path.join(save_dir,'ParWHData.mat')
-    if raw_data:
+    if data_file_locations:
         return d
 
     out = loadmat(d)
     # print(out.keys())
     # print(out['amp'][0]) #5 values 
     # print(out['fs'][0,0])
     # print(out['lines'][0]) #range 2:4096
@@ -115,15 +116,15 @@
     yValArr = out['yValArr'].reshape((16384,-1))
     data = [Input_output_data(u=ui,y=yi, sampling_time=1/fs) for ui,yi in zip(uValArr.T,yValArr.T)]
     datafiles_test.extend(data) if train_test_split else datafiles.extend(data)
 
     return datafiles, datafiles_test
 
     
-def F16(train_test_split=True, output_index=0, raw_data=False, dir_placement=None, force_download=False, url=None):
+def F16(train_test_split=True, output_index=0, data_file_locations=False, dir_placement=None, force_download=False, url=None):
     '''The F-16 Ground Vibration Test benchmark features a high order system with clearance and friction nonlinearities at the mounting interface of the payloads.
 
     The experimental data made available to the Workshop participants were acquired on a full-scale F-16 aircraft on the occasion of the Siemens LMS Ground Vibration Testing Master Class, held in September 2014 at the Saffraanberg military basis, Sint-Truiden, Belgium.
 
     During the test campaign, two dummy payloads were mounted at the wing tips to simulate the mass and inertia properties of real devices typically equipping an F-16 in ﬂight. The aircraft structure was instrumented with accelerometers. One shaker was attached underneath the right wing to apply input signals. The dominant source of nonlinearity in the structural dynamics was expected to originate from the mounting interfaces of the two payloads. These interfaces consist of T-shaped connecting elements on the payload side, slid through a rail attached to the wing side. A preliminary investigation showed that the back connection of the right-wing-to-payload interface was the predominant source of nonlinear distortions in the aircraft dynamics, and is therefore the focus of this benchmark study.
 
     A detailed formulation of the identification problem can be found here. All the provided files and information on the F-16 aircraft benchmark system are available for download here. This zip-file contains a detailed system description, the estimation and test data sets, and some pictures of the setup. The data is available in the .csv and .mat file format.
@@ -138,34 +139,35 @@
     #todo this is still broken for some mat files
     # assert False, 'this is still broken for some files where y has many more dimensions than expected'
     # url = 'http://www.nonlinearbenchmark.org/FILES/BENCHMARKS/F16/F16GVT_Files.zip'
 
     if train_test_split==True:
         print('Warning no offical train and test split has been determined for this dataset')
 
-    url = 'https://data.4tu.nl/ndownloader/files/24675560' if url is None else url
+    if url is None:
+        url = 'https://data.4tu.nl/file/b6dc643b-ecc6-437c-8a8a-1681650ec3fe/5414dfdc-6e8d-4208-be6e-fa553de9866f'
     download_size=148455295
     save_dir = cashed_download(url,'F16',zip_name='F16GVT_Files.zip',dir_placement=dir_placement,download_size=download_size,force_download=force_download)
     save_dir = os.path.join(save_dir,'F16GVT_Files/BenchmarkData') #matfiles location
     matfiles = [os.path.join(save_dir,a).replace('\\','/') for a in os.listdir(save_dir) if a.split('.')[-1]=='mat']
-    if raw_data:
+    if data_file_locations:
         return matfiles
     datasets = []
     for file in sorted(matfiles):
         out = loadmat(file)
         Force, Voltage, (y1,y2,y3),Fs = out['Force'][0], out['Voltage'][0], out['Acceleration'], out['Fs'][0,0]
         #u = Force
         #y = one of the ys, multi objective regression?
         name = file.split('/')[-1]
         if 'SpecialOddMSine' not in name:
             datasets.append(Input_output_data(u=Force,y=[y1,y2,y3][output_index], sampling_time=1/Fs))
     return datasets
 
 
-def Industrial_robot(train_test_split=True, raw_data=False, dir_placement=None, force_download=False, url=None):
+def Industrial_robot(train_test_split=True, data_file_locations=False, dir_placement=None, force_download=False, url=None):
     '''An identification benchmark dataset for a full robot movement with a KUKA KR300 R2500 
     ultra SE industrial robot is presented. It is a robot with a nominal payload capacity of
     300 kg, a weight of 1120 kg, and a reach of 2500mm. It exhibits 12 states accounting for
     position and velocity for each of the 6 joints. The robot encounters backlash in all 
     joints, pose-dependent inertia, pose-dependent gravitational loads, pose-dependent
     hydraulic forces, pose- and velocity-dependent centripetal and Coriolis forces as well 
     as nonlinear friction, which is temperature-dependent and therefore potentially 
@@ -177,28 +179,28 @@
     A detailed formulation of the identification problem can be found here. All the provided 
     files and information on the industrial robot dataset can be found here. 
 
     https://kluedo.ub.uni-kl.de/frontdoor/index/index/docId/6731
 
     https://fdm-fallback.uni-kl.de/TUK/FB/MV/WSKL/0001/
 
-    https://fdm-fallback.uni-kl.de/TUK/FB/MV/WSKL/0001/Robot_Identification_Benchmark_Without_Raw_Data.rar
+    https://fdm-fallback.uni-kl.de/TUK/FB/MV/WSKL/0001/Robot_Identification_Benchmark_Without_data_file_locations.rar
 
     Special thanks to Jonas Weigand and co-authors for creating and sharing this benchmark!'''
     url = 'https://fdm-fallback.uni-kl.de/TUK/FB/MV/WSKL/0001/Robot_Identification_Benchmark_Without_Raw_Data.rar'  if url is None else url
 
 
 
 
-    download_size=12717003 
+    download_size = 12717003 
     save_dir = cashed_download(url, 'Industrial_robot', zip_name='Robot_Identification_Benchmark_Without_Raw_Data.rar',\
         dir_placement=dir_placement, download_size=download_size, force_download=force_download)
-    # save_dir = os.path.join(save_dir,'forward_identification_without_raw_data') #matfiles location
+    # save_dir = os.path.join(save_dir,'forward_identification_without_data_file_locations') #matfiles location
     d = os.path.join(save_dir,'forward_identification_without_raw_data.mat')
-    if raw_data:
+    if data_file_locations:
         return d
 
 
     if train_test_split==True:
         print('Warning no offical train and test split has been determined for this dataset')
 
 
@@ -209,7 +211,10 @@
             for n in range(out['y_train'].shape[1]//K)]
     train = trains
     tests = [Input_output_data(y=out['y_test'][:,n*K:(n+1)*K].T,u = out['u_test'][:,n*K:(n+1)*K].T) \
             for n in range(out['y_test'].shape[1]//K)]
     test = tests
 
     return train, test
+
+if __name__=='__main__':
+    data = F16()
```

### Comparing `nonlinear_benchmarks-0.0.4/nonlinear_benchmarks/utilities.py` & `nonlinear_benchmarks-0.1.0/nonlinear_benchmarks/utilities.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,486 +4,569 @@
 00000030: 7175 6573 740d 0a69 6d70 6f72 7420 6f73  quest..import os
 00000040: 0d0a 696d 706f 7274 206f 732e 7061 7468  ..import os.path
 00000050: 0d0a 6672 6f6d 2070 6174 686c 6962 2069  ..from pathlib i
 00000060: 6d70 6f72 7420 5061 7468 0d0a 6672 6f6d  mport Path..from
 00000070: 2073 7973 2069 6d70 6f72 7420 706c 6174   sys import plat
 00000080: 666f 726d 0d0a 696d 706f 7274 2073 6875  form..import shu
 00000090: 7469 6c0d 0a69 6d70 6f72 7420 7072 6f67  til..import prog
-000000a0: 7265 7373 6261 720d 0a0d 0a69 6d70 6f72  ressbar....impor
-000000b0: 7420 7265 7175 6573 7473 0d0a 0d0a 0d0a  t requests......
-000000c0: 0d0a 636c 6173 7320 496e 7075 745f 6f75  ..class Input_ou
-000000d0: 7470 7574 5f64 6174 613a 0d0a 2020 2020  tput_data:..    
-000000e0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-000000f0: 662c 2075 2c20 792c 2073 616d 706c 696e  f, u, y, samplin
-00000100: 675f 7469 6d65 3d4e 6f6e 6529 3a0d 0a20  g_time=None):.. 
-00000110: 2020 2020 2020 2073 656c 662e 7520 3d20         self.u = 
-00000120: 750d 0a20 2020 2020 2020 2073 656c 662e  u..        self.
-00000130: 7920 3d20 790d 0a20 2020 2020 2020 2073  y = y..        s
-00000140: 656c 662e 7361 6d70 6c69 6e67 5f74 696d  elf.sampling_tim
-00000150: 6520 3d20 7361 6d70 6c69 6e67 5f74 696d  e = sampling_tim
-00000160: 650d 0a20 2020 200d 0a20 2020 2064 6566  e..    ..    def
-00000170: 205f 5f72 6570 725f 5f28 7365 6c66 293a   __repr__(self):
-00000180: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000190: 2066 2749 6e70 7574 5f6f 7574 7075 745f   f'Input_output_
-000001a0: 6461 7461 206f 6620 6c65 6e67 7468 3a20  data of length: 
-000001b0: 7b6c 656e 2873 656c 662e 7529 7d20 616e  {len(self.u)} an
-000001c0: 6420 7361 6d70 6c69 6e67 5f74 696d 653d  d sampling_time=
-000001d0: 7b73 656c 662e 7361 6d70 6c69 6e67 5f74  {self.sampling_t
-000001e0: 696d 653a 2e34 667d 270d 0a20 2020 200d  ime:.4f}'..    .
-000001f0: 0a20 2020 2064 6566 205f 5f69 7465 725f  .    def __iter_
-00000200: 5f28 7365 6c66 293a 0d0a 2020 2020 2020  _(self):..      
-00000210: 2020 7969 656c 6420 7365 6c66 2e75 0d0a    yield self.u..
-00000220: 2020 2020 2020 2020 7969 656c 6420 7365          yield se
-00000230: 6c66 2e79 0d0a 0d0a 2020 2020 6465 6620  lf.y....    def 
-00000240: 5f5f 6c65 6e5f 5f28 7365 6c66 293a 0d0a  __len__(self):..
-00000250: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-00000260: 656e 2873 656c 662e 7929 0d0a 2020 2020  en(self.y)..    
-00000270: 0d0a 2020 2020 6465 6620 5f5f 6765 7469  ..    def __geti
-00000280: 7465 6d5f 5f28 7365 6c66 2c61 7267 293a  tem__(self,arg):
-00000290: 0d0a 2020 2020 2020 2020 2727 2753 6c69  ..        '''Sli
-000002a0: 6365 2074 6865 2053 7973 7465 6d5f 6461  ce the System_da
-000002b0: 7461 2069 6e20 7469 6d65 2069 6e64 6578  ta in time index
-000002c0: 2727 270d 0a20 2020 2020 2020 2069 6620  '''..        if 
-000002d0: 6973 696e 7374 616e 6365 2861 7267 2c20  isinstance(arg, 
-000002e0: 696e 7429 3a0d 0a20 2020 2020 2020 2020  int):..         
-000002f0: 2020 2069 6620 6172 673d 3d30 3a0d 0a20     if arg==0:.. 
-00000300: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00000310: 6574 7572 6e20 7365 6c66 2e75 0d0a 2020  eturn self.u..  
-00000320: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
-00000330: 7267 3d3d 313a 0d0a 2020 2020 2020 2020  rg==1:..        
-00000340: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000350: 656c 662e 790d 0a20 2020 2020 2020 2020  elf.y..         
-00000360: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00000370: 726f 7228 6627 6966 2061 7267 756d 656e  ror(f'if argumen
-00000380: 7420 7b61 7267 7d20 6973 2061 2069 6e74  t {arg} is a int
-00000390: 2074 6861 6e20 6f6e 6c79 2030 2066 6f72   than only 0 for
-000003a0: 2075 2061 6e64 2031 2066 6f72 2079 2063   u and 1 for y c
-000003b0: 616e 2062 6520 7573 6564 2729 0d0a 2020  an be used')..  
-000003c0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-000003d0: 7461 6e63 6528 6172 672c 736c 6963 6529  tance(arg,slice)
-000003e0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000003f0: 7461 7274 2c20 7374 6f70 2c20 7374 6570  tart, stop, step
-00000400: 203d 2061 7267 2e69 6e64 6963 6573 286c   = arg.indices(l
-00000410: 656e 2873 656c 662e 7529 290d 0a20 2020  en(self.u))..   
-00000420: 2020 2020 2020 2020 2075 6e65 7720 3d20           unew = 
-00000430: 7365 6c66 2e75 5b61 7267 5d0d 0a20 2020  self.u[arg]..   
-00000440: 2020 2020 2020 2020 2079 6e65 7720 3d20           ynew = 
-00000450: 7365 6c66 2e79 5b61 7267 5d0d 0a20 2020  self.y[arg]..   
-00000460: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000470: 496e 7075 745f 6f75 7470 7574 5f64 6174  Input_output_dat
-00000480: 6128 753d 756e 6577 2c20 793d 796e 6577  a(u=unew, y=ynew
-00000490: 2c20 7361 6d70 6c69 6e67 5f74 696d 653d  , sampling_time=
-000004a0: 7365 6c66 2e73 616d 706c 696e 675f 7469  self.sampling_ti
-000004b0: 6d65 290d 0a20 2020 2020 2020 2065 6c73  me)..        els
-000004c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000004d0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-000004e0: 2866 2761 7267 756d 656e 7420 7769 7468  (f'argument with
-000004f0: 2076 616c 7565 2022 7b61 7267 7d22 206f   value "{arg}" o
-00000500: 6620 5f5f 6765 7469 7465 6d5f 5f20 6f66  f __getitem__ of
-00000510: 2074 7970 6520 227b 7479 7065 2861 7267   type "{type(arg
-00000520: 297d 2220 6973 206e 6f74 2061 6c6c 6f77  )}" is not allow
-00000530: 6564 2729 0d0a 0d0a 0d0a 6465 6620 6765  ed')......def ge
-00000540: 745f 746d 705f 6265 6e63 686d 6172 6b5f  t_tmp_benchmark_
-00000550: 6469 7265 6374 6f72 7928 293a 0d0a 2020  directory():..  
-00000560: 2020 2727 2741 2075 7469 6c69 7479 2066    '''A utility f
-00000570: 756e 6374 696f 6e20 7768 6963 6820 6765  unction which ge
-00000580: 7473 2074 6865 2075 7469 6c69 7479 2064  ts the utility d
-00000590: 6972 6563 746f 7269 6573 2066 6f72 2065  irectories for e
-000005a0: 6163 6820 4f53 0d0a 0d0a 2020 2020 4974  ach OS....    It
-000005b0: 2063 7265 6174 6573 2061 2077 6f72 6b69   creates a worki
-000005c0: 6e67 2064 6972 6563 746f 7279 2063 616c  ng directory cal
-000005d0: 6c65 6420 6e6f 6e6c 696e 6561 725f 6265  led nonlinear_be
-000005e0: 6e63 686d 6172 6b73 200d 0a0d 0a20 2020  nchmarks ....   
-000005f0: 2020 2020 2069 6e20 4c4f 4341 4c41 5050       in LOCALAPP
-00000600: 4441 5441 2066 6f72 2077 696e 646f 7773  DATA for windows
-00000610: 0d0a 0d0a 2020 2020 2020 2020 696e 207e  ....        in ~
-00000620: 2f2e 6e6f 6e6c 696e 6561 725f 6265 6e63  /.nonlinear_benc
-00000630: 686d 6172 6b73 2f20 666f 7220 756e 6978  hmarks/ for unix
-00000640: 206c 696b 650d 0a0d 0a20 2020 2020 2020   like....       
-00000650: 2069 6e20 7e2f 4c69 6272 6172 792f 4170   in ~/Library/Ap
-00000660: 706c 6963 6174 696f 6e20 5375 7070 6f72  plication Suppor
-00000670: 742f 6e6f 6e6c 696e 6561 725f 6265 6e63  t/nonlinear_benc
-00000680: 686d 6172 6b73 2f20 666f 7220 6461 7277  hmarks/ for darw
-00000690: 696e 0d0a 0d0a 2020 2020 6974 2063 7265  in....    it cre
-000006a0: 6174 6573 2074 776f 2064 6972 6563 746f  ates two directo
-000006b0: 7269 6573 2069 6e73 6964 6520 6f66 2074  ries inside of t
-000006c0: 6865 206e 6f6e 6c69 6e65 6172 5f62 656e  he nonlinear_ben
-000006d0: 6368 6d61 726b 7320 6469 7265 6374 6f72  chmarks director
-000006e0: 790d 0a0d 0a20 2020 2020 2020 2064 6174  y....        dat
-000006f0: 615f 7365 7473 203a 2063 6163 6865 206c  a_sets : cache l
-00000700: 6f63 6174 696f 6e20 6f66 2074 6865 2064  ocation of the d
-00000710: 6f77 6e6c 6f61 6465 6420 6461 7461 2073  ownloaded data s
-00000720: 6574 730d 0a0d 0a20 2020 2020 2020 2063  ets....        c
-00000730: 6865 636b 706f 696e 7473 203a 2075 7365  heckpoints : use
-00000740: 6420 6475 7269 6e67 2074 7261 696e 696e  d during trainin
-00000750: 6720 6f66 2074 6f72 6368 206d 6f64 656c  g of torch model
-00000760: 730d 0a0d 0a20 2020 2052 6574 7572 6e73  s....    Returns
-00000770: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20  ..    -------.. 
-00000780: 2020 2064 6963 7428 6261 7365 3d62 6173     dict(base=bas
-00000790: 655f 6469 722c 2064 6174 615f 7365 7473  e_dir, data_sets
-000007a0: 3d64 6174 615f 7365 7473 5f64 6972 2c20  =data_sets_dir, 
-000007b0: 6368 6563 6b70 6f69 6e74 733d 6368 6563  checkpoints=chec
-000007c0: 6b70 6f69 6e74 735f 6469 7229 0d0a 2020  kpoints_dir)..  
-000007d0: 2020 2727 270d 0a0d 0a20 2020 2064 6566    '''....    def
-000007e0: 206d 6b64 6972 2864 6972 6563 746f 7279   mkdir(directory
-000007f0: 293a 0d0a 2020 2020 2020 2020 6966 206f  ):..        if o
-00000800: 732e 7061 7468 2e69 7364 6972 2864 6972  s.path.isdir(dir
-00000810: 6563 746f 7279 2920 6973 2046 616c 7365  ectory) is False
-00000820: 3a0d 0a20 2020 2020 2020 2020 2020 206f  :..            o
-00000830: 732e 6d6b 6469 7228 6469 7265 6374 6f72  s.mkdir(director
-00000840: 7929 0d0a 0d0a 2020 2020 6672 6f6d 2073  y)....    from s
-00000850: 7973 2069 6d70 6f72 7420 706c 6174 666f  ys import platfo
-00000860: 726d 0d0a 2020 2020 6966 2070 6c61 7466  rm..    if platf
-00000870: 6f72 6d20 3d3d 2022 6461 7277 696e 223a  orm == "darwin":
-00000880: 2023 6e6f 7420 7465 7374 6564 2062 7574   #not tested but
-00000890: 2068 6572 6520 6974 2067 6f65 730d 0a20   here it goes.. 
-000008a0: 2020 2020 2020 2062 6173 655f 6469 7220         base_dir 
-000008b0: 3d20 6f73 2e70 6174 682e 6578 7061 6e64  = os.path.expand
-000008c0: 7573 6572 2827 7e2f 4c69 6272 6172 792f  user('~/Library/
-000008d0: 4170 706c 6963 6174 696f 6e20 5375 7070  Application Supp
-000008e0: 6f72 742f 6e6f 6e6c 696e 6561 725f 6265  ort/nonlinear_be
-000008f0: 6e63 686d 6172 6b73 2f27 290d 0a20 2020  nchmarks/')..   
-00000900: 2065 6c69 6620 706c 6174 666f 726d 203d   elif platform =
-00000910: 3d20 2277 696e 3332 223a 0d0a 2020 2020  = "win32":..    
-00000920: 2020 2020 6261 7365 5f64 6972 203d 206f      base_dir = o
-00000930: 732e 7061 7468 2e6a 6f69 6e28 6f73 2e67  s.path.join(os.g
-00000940: 6574 656e 7628 274c 4f43 414c 4150 5044  etenv('LOCALAPPD
-00000950: 4154 4127 292c 276e 6f6e 6c69 6e65 6172  ATA'),'nonlinear
-00000960: 5f62 656e 6368 6d61 726b 732f 2729 0d0a  _benchmarks/')..
-00000970: 2020 2020 656c 7365 3a20 2375 6e69 7820      else: #unix 
-00000980: 6c69 6b65 2c20 6d69 6768 7420 6265 2070  like, might be p
-00000990: 726f 626c 656d 6174 6963 2066 6f72 2073  roblematic for s
-000009a0: 6f6d 6520 7765 6972 6420 6f70 6572 6174  ome weird operat
-000009b0: 696e 6720 7379 7374 656d 732e 0d0a 2020  ing systems...  
-000009c0: 2020 2020 2020 6261 7365 5f64 6972 203d        base_dir =
-000009d0: 206f 732e 7061 7468 2e65 7870 616e 6475   os.path.expandu
-000009e0: 7365 7228 277e 2f2e 6e6f 6e6c 696e 6561  ser('~/.nonlinea
-000009f0: 725f 6265 6e63 686d 6172 6b73 2f27 2923  r_benchmarks/')#
-00000a00: 5061 7468 2827 7e2f 2e6e 6f6e 6c69 6e65  Path('~/.nonline
-00000a10: 6172 5f62 656e 6368 6d61 726b 732f 2729  ar_benchmarks/')
-00000a20: 0d0a 2020 2020 6d6b 6469 7228 6261 7365  ..    mkdir(base
-00000a30: 5f64 6972 290d 0a20 2020 2072 6574 7572  _dir)..    retur
-00000a40: 6e20 6261 7365 5f64 6972 0d0a 0d0a 6465  n base_dir....de
-00000a50: 6620 636c 6561 725f 6361 6368 6528 293a  f clear_cache():
-00000a60: 0d0a 2020 2020 2727 2744 656c 6574 6520  ..    '''Delete 
-00000a70: 616c 6c20 6361 6368 6564 2064 6f77 6e6c  all cached downl
-00000a80: 6f61 6473 2727 270d 0a20 2020 200d 0a20  oads'''..    .. 
-00000a90: 2020 2074 656d 705f 6469 7220 3d20 6765     temp_dir = ge
-00000aa0: 745f 746d 705f 6265 6e63 686d 6172 6b5f  t_tmp_benchmark_
-00000ab0: 6469 7265 6374 6f72 7928 290d 0a20 2020  directory()..   
-00000ac0: 2066 6f72 206c 2069 6e20 5b27 454d 5053   for l in ['EMPS
-00000ad0: 272c 2743 4544 272c 2746 3136 272c 2757  ','CED','F16','W
-00000ae0: 6965 6e48 616d 6d65 7227 2c27 426f 7563  ienHammer','Bouc
-00000af0: 5765 6e27 2c27 5061 7257 4846 272c 2757  Wen','ParWHF','W
-00000b00: 6965 6e65 7248 616d 6d65 7242 656e 6368  ienerHammerBench
-00000b10: 4d61 726b 272c 2753 696c 7665 7262 6f78  Mark','Silverbox
-00000b20: 272c 2743 6173 6361 6465 645f 5461 6e6b  ','Cascaded_Tank
-00000b30: 7327 5d3a 0d0a 2020 2020 2020 2020 7472  s']:..        tr
-00000b40: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00000b50: 7368 7574 696c 2e72 6d74 7265 6528 6f73  shutil.rmtree(os
-00000b60: 2e70 6174 682e 6a6f 696e 2874 656d 705f  .path.join(temp_
-00000b70: 6469 722c 6c29 290d 0a20 2020 2020 2020  dir,l))..       
-00000b80: 2065 7863 6570 7420 4669 6c65 4e6f 7446   except FileNotF
-00000b90: 6f75 6e64 4572 726f 723a 0d0a 2020 2020  oundError:..    
-00000ba0: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
-00000bb0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00000bc0: 7368 7574 696c 2e72 6d74 7265 6528 6f73  shutil.rmtree(os
-00000bd0: 2e70 6174 682e 6a6f 696e 2874 656d 705f  .path.join(temp_
-00000be0: 6469 722c 2744 6149 5379 5f64 6174 6127  dir,'DaISy_data'
-00000bf0: 2929 0d0a 2020 2020 6578 6365 7074 2046  ))..    except F
-00000c00: 696c 654e 6f74 466f 756e 6445 7272 6f72  ileNotFoundError
-00000c10: 3a0d 0a20 2020 2020 2020 2070 6173 730d  :..        pass.
-00000c20: 0a0d 0a0d 0a63 6c61 7373 204d 7950 726f  .....class MyPro
-00000c30: 6772 6573 7342 6172 2829 3a0d 0a20 2020  gressBar():..   
-00000c40: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00000c50: 6c66 2c64 6f77 6e6c 6f61 645f 7369 7a65  lf,download_size
-00000c60: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-00000c70: 2e70 6261 7220 3d20 4e6f 6e65 0d0a 2020  .pbar = None..  
-00000c80: 2020 2020 2020 7365 6c66 2e64 6f77 6e6c        self.downl
-00000c90: 6f61 645f 7369 7a65 203d 2064 6f77 6e6c  oad_size = downl
-00000ca0: 6f61 645f 7369 7a65 0d0a 0d0a 2020 2020  oad_size....    
-00000cb0: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
-00000cc0: 662c 2062 6c6f 636b 5f6e 756d 2c20 626c  f, block_num, bl
-00000cd0: 6f63 6b5f 7369 7a65 2c20 746f 7461 6c5f  ock_size, total_
-00000ce0: 7369 7a65 293a 0d0a 2020 2020 2020 2020  size):..        
-00000cf0: 746f 7461 6c5f 7369 7a65 203d 2073 656c  total_size = sel
-00000d00: 662e 646f 776e 6c6f 6164 5f73 697a 650d  f.download_size.
-00000d10: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00000d20: 7365 6c66 2e70 6261 723a 0d0a 2020 2020  self.pbar:..    
-00000d30: 2020 2020 2020 2020 7365 6c66 2e70 6261          self.pba
-00000d40: 723d 7072 6f67 7265 7373 6261 722e 5072  r=progressbar.Pr
-00000d50: 6f67 7265 7373 4261 7228 6d61 7876 616c  ogressBar(maxval
-00000d60: 3d74 6f74 616c 5f73 697a 6529 0d0a 2020  =total_size)..  
-00000d70: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00000d80: 6261 722e 7374 6172 7428 290d 0a0d 0a20  bar.start().... 
-00000d90: 2020 2020 2020 2064 6f77 6e6c 6f61 6465         downloade
-00000da0: 6420 3d20 626c 6f63 6b5f 6e75 6d20 2a20  d = block_num * 
-00000db0: 626c 6f63 6b5f 7369 7a65 0d0a 2020 2020  block_size..    
-00000dc0: 2020 2020 6966 2064 6f77 6e6c 6f61 6465      if downloade
-00000dd0: 6420 3c20 746f 7461 6c5f 7369 7a65 3a0d  d < total_size:.
-00000de0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00000df0: 662e 7062 6172 2e75 7064 6174 6528 646f  f.pbar.update(do
-00000e00: 776e 6c6f 6164 6564 290d 0a20 2020 2020  wnloaded)..     
-00000e10: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000e20: 2020 2020 2020 7365 6c66 2e70 6261 722e        self.pbar.
-00000e30: 6669 6e69 7368 2829 0d0a 0d0a 0d0a 6465  finish()......de
-00000e40: 6620 6361 7368 6564 5f64 6f77 6e6c 6f61  f cashed_downloa
-00000e50: 6428 7572 6c2c 6e61 6d65 5f64 6972 2c7a  d(url,name_dir,z
-00000e60: 6970 5f6e 616d 653d 4e6f 6e65 2c64 6972  ip_name=None,dir
-00000e70: 5f70 6c61 6365 6d65 6e74 3d4e 6f6e 652c  _placement=None,
-00000e80: 646f 776e 6c6f 6164 5f73 697a 653d 4e6f  download_size=No
-00000e90: 6e65 2c66 6f72 6365 5f64 6f77 6e6c 6f61  ne,force_downloa
-00000ea0: 643d 4661 6c73 652c 7a69 7070 6564 3d54  d=False,zipped=T
-00000eb0: 7275 6529 3a0d 0a20 2020 2027 2727 7572  rue):..    '''ur
-00000ec0: 6c20 6973 2074 6865 2066 696c 6520 746f  l is the file to
-00000ed0: 2062 6520 646f 776e 6c6f 6164 6564 0d0a   be downloaded..
-00000ee0: 2020 2020 6e61 6d65 5f64 6972 2069 7320      name_dir is 
-00000ef0: 7468 6520 6469 7265 6374 6f72 7920 6e61  the directory na
-00000f00: 6d65 2077 6865 7265 2074 6865 2066 696c  me where the fil
-00000f10: 6520 616e 6420 7468 6520 636f 6e74 656e  e and the conten
-00000f20: 7473 206f 6620 7468 6520 6669 6c65 2077  ts of the file w
-00000f30: 696c 6c20 6265 2073 6176 6564 0d0a 2020  ill be saved..  
-00000f40: 2020 6469 725f 706c 6163 656d 656e 7420    dir_placement 
-00000f50: 6973 2061 6e20 6f70 7469 6f6e 616c 2061  is an optional a
-00000f60: 7267 756d 656e 7420 7468 6174 2067 6976  rgument that giv
-00000f70: 6573 2074 6865 206c 6f63 6174 696f 6e20  es the location 
-00000f80: 6f66 2074 6865 2064 6f77 6e6c 6f61 6465  of the downloade
-00000f90: 6420 6669 6c65 200d 0a20 2020 2069 6620  d file ..    if 
-00000fa0: 6974 2069 7320 6e6f 6e65 2069 7420 7769  it is none it wi
-00000fb0: 6c6c 2064 6f77 6e6c 6f61 6420 746f 2074  ll download to t
-00000fc0: 6865 2074 656d 7020 6469 720d 0a20 2020  he temp dir..   
-00000fd0: 2069 6620 6469 725f 6e61 6d65 2069 7320   if dir_name is 
-00000fe0: 4e6f 6e65 2069 7420 7769 6c6c 2062 6520  None it will be 
-00000ff0: 7361 7665 6420 696e 2074 6865 2074 656d  saved in the tem
-00001000: 7020 6469 7265 6374 6f72 7920 6f66 2074  p directory of t
-00001010: 6865 2073 7973 7465 6d27 2727 0d0a 0d0a  he system'''....
-00001020: 2020 2020 2366 696e 6469 6e67 2f6d 616b      #finding/mak
-00001030: 696e 6720 6469 7265 6374 6f72 6965 730d  ing directories.
-00001040: 0a20 2020 2069 6620 6469 725f 706c 6163  .    if dir_plac
-00001050: 656d 656e 7420 6973 204e 6f6e 653a 0d0a  ement is None:..
-00001060: 2020 2020 2020 2020 7020 3d20 6765 745f          p = get_
-00001070: 746d 705f 6265 6e63 686d 6172 6b5f 6469  tmp_benchmark_di
-00001080: 7265 6374 6f72 7928 2920 2375 7365 2074  rectory() #use t
-00001090: 656d 7020 6469 720d 0a20 2020 2065 6c73  emp dir..    els
-000010a0: 653a 0d0a 2020 2020 2020 2020 7020 3d20  e:..        p = 
-000010b0: 5061 7468 2864 6972 5f70 6c61 6365 6d65  Path(dir_placeme
-000010c0: 6e74 2920 2375 7365 2067 6976 656e 2064  nt) #use given d
-000010d0: 6972 0d0a 2020 2020 7361 7665 5f64 6972  ir..    save_dir
-000010e0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-000010f0: 702c 5061 7468 286e 616d 655f 6469 7229  p,Path(name_dir)
-00001100: 290d 0a20 2020 2069 6620 6f73 2e70 6174  )..    if os.pat
-00001110: 682e 6973 6469 7228 7361 7665 5f64 6972  h.isdir(save_dir
-00001120: 2920 6973 2046 616c 7365 3a0d 0a20 2020  ) is False:..   
-00001130: 2020 2020 206f 732e 6d6b 6469 7228 7361       os.mkdir(sa
-00001140: 7665 5f64 6972 290d 0a20 2020 2066 696c  ve_dir)..    fil
-00001150: 655f 6e61 6d65 203d 2075 726c 2e73 706c  e_name = url.spl
-00001160: 6974 2827 2f27 295b 2d31 5d20 6966 207a  it('/')[-1] if z
-00001170: 6970 5f6e 616d 653d 3d4e 6f6e 6520 656c  ip_name==None el
-00001180: 7365 207a 6970 5f6e 616d 650d 0a20 2020  se zip_name..   
-00001190: 2073 6176 655f 6c6f 6320 3d20 6f73 2e70   save_loc = os.p
-000011a0: 6174 682e 6a6f 696e 2873 6176 655f 6469  ath.join(save_di
-000011b0: 722c 6669 6c65 5f6e 616d 6529 200d 0a0d  r,file_name) ...
-000011c0: 0a20 2020 2069 6620 6f73 2e70 6174 682e  .    if os.path.
-000011d0: 6973 6669 6c65 2873 6176 655f 6c6f 6329  isfile(save_loc)
-000011e0: 2061 6e64 206e 6f74 2066 6f72 6365 5f64   and not force_d
-000011f0: 6f77 6e6c 6f61 643a 0d0a 2020 2020 2020  ownload:..      
-00001200: 2020 7265 7475 726e 2073 6176 655f 6469    return save_di
-00001210: 720d 0a0d 0a20 2020 2069 6620 666f 7263  r....    if forc
-00001220: 655f 646f 776e 6c6f 6164 3a0d 0a20 2020  e_download:..   
-00001230: 2020 2020 2070 7269 6e74 2866 2728 7265       print(f'(re
-00001240: 2d29 646f 776e 6c6f 6164 696e 6720 6461  -)downloading da
-00001250: 7461 7365 7420 6672 6f6d 207b 7572 6c7d  taset from {url}
-00001260: 205c 6e20 696e 207b 7361 7665 5f6c 6f63   \n in {save_loc
-00001270: 7d27 290d 0a20 2020 2065 6c73 653a 0d0a  }')..    else:..
-00001280: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-00001290: 6461 7461 7365 7420 6e6f 7420 666f 756e  dataset not foun
-000012a0: 6420 646f 776e 6c6f 6164 696e 6720 6672  d downloading fr
-000012b0: 6f6d 207b 7572 6c7d 205c 6e20 696e 207b  om {url} \n in {
-000012c0: 7361 7665 5f6c 6f63 7d27 290d 0a0d 0a20  save_loc}').... 
-000012d0: 2020 2069 6620 2764 7269 7665 2e67 6f6f     if 'drive.goo
-000012e0: 676c 6527 2069 6e20 7572 6c3a 0d0a 2020  gle' in url:..  
-000012f0: 2020 2020 2020 646f 776e 6c6f 6164 5f66        download_f
-00001300: 696c 655f 6672 6f6d 5f67 6f6f 676c 655f  ile_from_google_
-00001310: 6472 6976 6528 7572 6c2c 2073 6176 655f  drive(url, save_
-00001320: 6c6f 6329 0d0a 2020 2020 656c 7365 3a0d  loc)..    else:.
-00001330: 0a20 2020 2020 2020 2066 726f 6d20 6874  .        from ht
-00001340: 7470 2e63 6c69 656e 7420 696d 706f 7274  tp.client import
-00001350: 2049 6e63 6f6d 706c 6574 6552 6561 640d   IncompleteRead.
-00001360: 0a20 2020 2020 2020 2074 7269 6573 203d  .        tries =
-00001370: 2030 0d0a 2020 2020 2020 2020 7768 696c   0..        whil
-00001380: 6520 5472 7565 3a0d 0a20 2020 2020 2020  e True:..       
-00001390: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-000013a0: 2020 2020 2020 2020 2020 2069 6620 646f             if do
-000013b0: 776e 6c6f 6164 5f73 697a 6520 6973 204e  wnload_size is N
-000013c0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000013d0: 2020 2020 2020 2020 2020 7572 6c6c 6962            urllib
-000013e0: 2e72 6571 7565 7374 2e75 726c 7265 7472  .request.urlretr
-000013f0: 6965 7665 2875 726c 2c20 7361 7665 5f6c  ieve(url, save_l
-00001400: 6f63 2923 204d 7950 726f 6772 6573 7342  oc)# MyProgressB
-00001410: 6172 2829 2069 7320 6120 7374 6561 6d20  ar() is a steam 
-00001420: 736f 206e 6f20 6c65 6e67 7468 2069 7320  so no length is 
-00001430: 6769 7665 6e0d 0a20 2020 2020 2020 2020  given..         
-00001440: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00001450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001460: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00001470: 2020 2020 2020 2020 2020 2020 2075 726c               url
-00001480: 6c69 622e 7265 7175 6573 742e 7572 6c72  lib.request.urlr
-00001490: 6574 7269 6576 6528 7572 6c2c 2073 6176  etrieve(url, sav
-000014a0: 655f 6c6f 632c 204d 7950 726f 6772 6573  e_loc, MyProgres
-000014b0: 7342 6172 2864 6f77 6e6c 6f61 645f 7369  sBar(download_si
-000014c0: 7a65 3d69 6e74 2864 6f77 6e6c 6f61 645f  ze=int(download_
-000014d0: 7369 7a65 2929 290d 0a20 2020 2020 2020  size)))..       
-000014e0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-000014f0: 616b 0d0a 2020 2020 2020 2020 2020 2020  ak..            
-00001500: 6578 6365 7074 2049 6e63 6f6d 706c 6574  except Incomplet
-00001510: 6552 6561 643a 0d0a 2020 2020 2020 2020  eRead:..        
-00001520: 2020 2020 2020 2020 7472 6965 7320 2b3d          tries +=
-00001530: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00001540: 2020 2020 7072 696e 7428 2749 6e63 6f6d      print('Incom
-00001550: 706c 6574 6552 6561 6420 646f 776e 6c6f  pleteRead downlo
-00001560: 6164 2066 6169 6c65 642c 2072 652d 646f  ad failed, re-do
-00001570: 776e 6c6f 6164 696e 6720 6669 6c65 2729  wnloading file')
-00001580: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001590: 2020 646f 776e 6c6f 6164 5f73 697a 6520    download_size 
-000015a0: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-000015b0: 2020 2020 2020 2020 6966 2074 7269 6573          if tries
-000015c0: 3d3d 353a 0d0a 2020 2020 2020 2020 2020  ==5:..          
-000015d0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-000015e0: 2046 616c 7365 2c20 2744 6f77 6e6c 6f61   False, 'Downloa
-000015f0: 6420 4661 696c 2035 2074 696d 6573 2065  d Fail 5 times e
-00001600: 7869 7469 6e67 2e27 0d0a 0d0a 0d0a 2020  xiting.'......  
-00001610: 2020 6966 206e 6f74 207a 6970 7065 643a    if not zipped:
-00001620: 2072 6574 7572 6e20 7361 7665 5f64 6972   return save_dir
-00001630: 0d0a 2020 2020 7072 696e 7428 2765 7874  ..    print('ext
-00001640: 7261 6374 696e 6720 6669 6c65 2e2e 2e27  racting file...'
-00001650: 290d 0a20 2020 200d 0a20 2020 2065 6e64  )..    ..    end
-00001660: 696e 6720 3d20 6669 6c65 5f6e 616d 652e  ing = file_name.
-00001670: 7370 6c69 7428 272e 2729 5b2d 315d 0d0a  split('.')[-1]..
-00001680: 2020 2020 6966 2065 6e64 696e 673d 3d27      if ending=='
-00001690: 677a 273a 0d0a 2020 2020 2020 2020 696d  gz':..        im
-000016a0: 706f 7274 2073 6875 7469 6c0d 0a20 2020  port shutil..   
-000016b0: 2020 2020 2069 6d70 6f72 7420 677a 6970       import gzip
-000016c0: 0d0a 2020 2020 2020 2020 7769 7468 206f  ..        with o
-000016d0: 7065 6e28 6f73 2e70 6174 682e 6a6f 696e  pen(os.path.join
-000016e0: 2873 6176 655f 6469 722c 6669 6c65 5f6e  (save_dir,file_n
-000016f0: 616d 655b 3a2d 335d 292c 2027 7762 2729  ame[:-3]), 'wb')
-00001700: 2061 7320 665f 6f75 743a 0d0a 2020 2020   as f_out:..    
-00001710: 2020 2020 2020 2020 7769 7468 2067 7a69          with gzi
-00001720: 702e 6f70 656e 2873 6176 655f 6c6f 632c  p.open(save_loc,
-00001730: 2027 7262 2729 2061 7320 665f 696e 3a0d   'rb') as f_in:.
-00001740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001750: 2073 6875 7469 6c2e 636f 7079 6669 6c65   shutil.copyfile
-00001760: 6f62 6a28 665f 696e 2c20 665f 6f75 7429  obj(f_in, f_out)
-00001770: 0d0a 2020 2020 656c 6966 2065 6e64 696e  ..    elif endin
-00001780: 673d 3d27 7a69 7027 3a0d 0a20 2020 2020  g=='zip':..     
-00001790: 2020 2066 726f 6d20 7a69 7066 696c 6520     from zipfile 
-000017a0: 696d 706f 7274 205a 6970 4669 6c65 2061  import ZipFile a
-000017b0: 7320 4669 6c65 0d0a 2020 2020 2020 2020  s File..        
-000017c0: 7769 7468 2046 696c 6528 7361 7665 5f6c  with File(save_l
-000017d0: 6f63 2920 6173 204f 626a 3a0d 0a20 2020  oc) as Obj:..   
-000017e0: 2020 2020 2020 2020 204f 626a 2e65 7874           Obj.ext
-000017f0: 7261 6374 616c 6c28 7361 7665 5f64 6972  ractall(save_dir
-00001800: 290d 0a20 2020 2065 6c69 6620 656e 6469  )..    elif endi
-00001810: 6e67 3d3d 2772 6172 273a 0d0a 2020 2020  ng=='rar':..    
-00001820: 2020 2020 6672 6f6d 2072 6172 6669 6c65      from rarfile
-00001830: 2069 6d70 6f72 7420 5261 7246 696c 6520   import RarFile 
-00001840: 6173 2046 696c 650d 0a20 2020 2020 2020  as File..       
-00001850: 2077 6974 6820 4669 6c65 2873 6176 655f   with File(save_
-00001860: 6c6f 6329 2061 7320 4f62 6a3a 0d0a 2020  loc) as Obj:..  
-00001870: 2020 2020 2020 2020 2020 4f62 6a2e 6578            Obj.ex
-00001880: 7472 6163 7461 6c6c 2873 6176 655f 6469  tractall(save_di
-00001890: 7229 0d0a 2020 2020 656c 7365 3a0d 0a20  r)..    else:.. 
-000018a0: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-000018b0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-000018c0: 2866 2766 696c 6520 7b66 696c 655f 6e61  (f'file {file_na
-000018d0: 6d65 7d20 7479 7065 206e 6f74 2069 6d70  me} type not imp
-000018e0: 6c65 6d65 6e74 6564 2729 0d0a 2020 2020  lemented')..    
-000018f0: 7265 7475 726e 2073 6176 655f 6469 720d  return save_dir.
-00001900: 0a0d 0a0d 0a64 6566 2064 6f77 6e6c 6f61  .....def downloa
-00001910: 645f 6669 6c65 5f66 726f 6d5f 676f 6f67  d_file_from_goog
-00001920: 6c65 5f64 7269 7665 2875 726c 2c20 6465  le_drive(url, de
-00001930: 7374 696e 6174 696f 6e29 3a0d 0a20 2020  stination):..   
-00001940: 2069 6420 3d20 7572 6c2e 7370 6c69 7428   id = url.split(
-00001950: 272f 2729 5b2d 325d 0d0a 2020 2020 5552  '/')[-2]..    UR
-00001960: 4c20 3d20 2268 7474 7073 3a2f 2f64 6f63  L = "https://doc
-00001970: 732e 676f 6f67 6c65 2e63 6f6d 2f75 633f  s.google.com/uc?
-00001980: 6578 706f 7274 3d64 6f77 6e6c 6f61 6422  export=download"
-00001990: 0d0a 0d0a 2020 2020 7365 7373 696f 6e20  ....    session 
-000019a0: 3d20 7265 7175 6573 7473 2e53 6573 7369  = requests.Sessi
-000019b0: 6f6e 2829 0d0a 0d0a 2020 2020 7265 7370  on()....    resp
-000019c0: 6f6e 7365 203d 2073 6573 7369 6f6e 2e67  onse = session.g
-000019d0: 6574 2855 524c 2c20 7061 7261 6d73 203d  et(URL, params =
-000019e0: 207b 2027 6964 2720 3a20 6964 207d 2c20   { 'id' : id }, 
-000019f0: 7374 7265 616d 203d 2054 7275 6529 0d0a  stream = True)..
-00001a00: 2020 2020 746f 6b65 6e20 3d20 6765 745f      token = get_
-00001a10: 636f 6e66 6972 6d5f 746f 6b65 6e28 7265  confirm_token(re
-00001a20: 7370 6f6e 7365 290d 0a0d 0a20 2020 2069  sponse)....    i
-00001a30: 6620 746f 6b65 6e3a 0d0a 2020 2020 2020  f token:..      
-00001a40: 2020 7061 7261 6d73 203d 207b 2027 6964    params = { 'id
-00001a50: 2720 3a20 6964 2c20 2763 6f6e 6669 726d  ' : id, 'confirm
-00001a60: 2720 3a20 746f 6b65 6e20 7d0d 0a20 2020  ' : token }..   
-00001a70: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-00001a80: 7365 7373 696f 6e2e 6765 7428 5552 4c2c  session.get(URL,
-00001a90: 2070 6172 616d 7320 3d20 7061 7261 6d73   params = params
-00001aa0: 2c20 7374 7265 616d 203d 2054 7275 6529  , stream = True)
-00001ab0: 0d0a 0d0a 2020 2020 7361 7665 5f72 6573  ....    save_res
-00001ac0: 706f 6e73 655f 636f 6e74 656e 7428 7265  ponse_content(re
-00001ad0: 7370 6f6e 7365 2c20 6465 7374 696e 6174  sponse, destinat
-00001ae0: 696f 6e29 2020 2020 0d0a 0d0a 6465 6620  ion)    ....def 
-00001af0: 6765 745f 636f 6e66 6972 6d5f 746f 6b65  get_confirm_toke
-00001b00: 6e28 7265 7370 6f6e 7365 293a 0d0a 2020  n(response):..  
-00001b10: 2020 666f 7220 6b65 792c 2076 616c 7565    for key, value
-00001b20: 2069 6e20 7265 7370 6f6e 7365 2e63 6f6f   in response.coo
-00001b30: 6b69 6573 2e69 7465 6d73 2829 3a0d 0a20  kies.items():.. 
-00001b40: 2020 2020 2020 2069 6620 6b65 792e 7374         if key.st
-00001b50: 6172 7473 7769 7468 2827 646f 776e 6c6f  artswith('downlo
-00001b60: 6164 5f77 6172 6e69 6e67 2729 3a0d 0a20  ad_warning'):.. 
-00001b70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001b80: 6e20 7661 6c75 650d 0a0d 0a20 2020 2072  n value....    r
-00001b90: 6574 7572 6e20 4e6f 6e65 0d0a 0d0a 6465  eturn None....de
-00001ba0: 6620 7361 7665 5f72 6573 706f 6e73 655f  f save_response_
-00001bb0: 636f 6e74 656e 7428 7265 7370 6f6e 7365  content(response
-00001bc0: 2c20 6465 7374 696e 6174 696f 6e29 3a0d  , destination):.
-00001bd0: 0a20 2020 2043 4855 4e4b 5f53 495a 4520  .    CHUNK_SIZE 
-00001be0: 3d20 3332 3736 380d 0a0d 0a20 2020 2077  = 32768....    w
-00001bf0: 6974 6820 6f70 656e 2864 6573 7469 6e61  ith open(destina
-00001c00: 7469 6f6e 2c20 2277 6222 2920 6173 2066  tion, "wb") as f
-00001c10: 3a0d 0a20 2020 2020 2020 2066 6f72 2063  :..        for c
-00001c20: 6875 6e6b 2069 6e20 7265 7370 6f6e 7365  hunk in response
-00001c30: 2e69 7465 725f 636f 6e74 656e 7428 4348  .iter_content(CH
-00001c40: 554e 4b5f 5349 5a45 293a 0d0a 2020 2020  UNK_SIZE):..    
-00001c50: 2020 2020 2020 2020 6966 2063 6875 6e6b          if chunk
-00001c60: 3a20 2320 6669 6c74 6572 206f 7574 206b  : # filter out k
-00001c70: 6565 702d 616c 6976 6520 6e65 7720 6368  eep-alive new ch
-00001c80: 756e 6b73 0d0a 2020 2020 2020 2020 2020  unks..          
-00001c90: 2020 2020 2020 662e 7772 6974 6528 6368        f.write(ch
-00001ca0: 756e 6b29 0d0a 0d0a 2320 6966 205f 5f6e  unk)....# if __n
-00001cb0: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
-00001cc0: 5f5f 273a 0d0a 2320 2020 2020 696d 706f  __':..#     impo
-00001cd0: 7274 206e 6f6e 6c69 6e65 6172 5f62 656e  rt nonlinear_ben
-00001ce0: 6368 6d61 726b 730d 0a23 2020 2020 2075  chmarks..#     u
-00001cf0: 2c79 203d 206e 6f6e 6c69 6e65 6172 5f62  ,y = nonlinear_b
-00001d00: 656e 6368 6d61 726b 732e 4345 4428 7370  enchmarks.CED(sp
-00001d10: 6c69 745f 6461 7461 3d46 616c 7365 290d  lit_data=False).
-00001d20: 0a23 2020 2020 2073 7973 5f64 6174 612e  .#     sys_data.
-00001d30: 706c 6f74 2873 686f 773d 5472 7565 290d  plot(show=True).
-00001d40: 0a0d 0a20 2020 2023 2066 696c 656e 616d  ...    # filenam
-00001d50: 6520 3d20 272e 2f66 696c 652e 7a69 7027  e = './file.zip'
-00001d60: 0d0a 2020 2020 2320 7572 6c20 3d20 2768  ..    # url = 'h
-00001d70: 7474 703a 2f2f 7777 772e 6e6f 6e6c 696e  ttp://www.nonlin
-00001d80: 6561 7262 656e 6368 6d61 726b 2e6f 7267  earbenchmark.org
-00001d90: 2f46 494c 4553 2f42 454e 4348 4d41 524b  /FILES/BENCHMARK
-00001da0: 532f 454d 5053 2f45 4d50 532e 7a69 7027  S/EMPS/EMPS.zip'
-00001db0: 0d0a 2020 2020 2320 7572 6c6c 6962 2e72  ..    # urllib.r
-00001dc0: 6571 7565 7374 2e75 726c 7265 7472 6965  equest.urlretrie
-00001dd0: 7665 2875 726c 2c20 6669 6c65 6e61 6d65  ve(url, filename
-00001de0: 290d 0a0d 0a20 2020 2023 2072 6573 7020  )....    # resp 
-00001df0: 3d20 7572 6c6c 6962 2e72 6571 7565 7374  = urllib.request
-00001e00: 2e75 726c 6f70 656e 2875 726c 290d 0a20  .urlopen(url).. 
-00001e10: 2020 2023 2072 6573 7048 746d 6c20 3d20     # respHtml = 
-00001e20: 7265 7370 2e72 6561 6428 290d 0a20 2020  resp.read()..   
-00001e30: 2023 2062 696e 6669 6c65 203d 206f 7065   # binfile = ope
-00001e40: 6e28 6669 6c65 6e61 6d65 2c20 2277 6222  n(filename, "wb"
-00001e50: 290d 0a20 2020 2023 2062 696e 6669 6c65  )..    # binfile
-00001e60: 2e77 7269 7465 2872 6573 7048 746d 6c29  .write(respHtml)
-00001e70: 0d0a 2020 2020 2320 6269 6e66 696c 652e  ..    # binfile.
-00001e80: 636c 6f73 6528 290d 0a0d 0a20 2020 20    close()....    
+000000a0: 7265 7373 6261 720d 0a69 6d70 6f72 7420  ressbar..import 
+000000b0: 6e75 6d70 7920 6173 206e 700d 0a66 726f  numpy as np..fro
+000000c0: 6d20 6e75 6d62 6572 7320 696d 706f 7274  m numbers import
+000000d0: 204e 756d 6265 720d 0a0d 0a69 6d70 6f72   Number....impor
+000000e0: 7420 7265 7175 6573 7473 0d0a 0d0a 636c  t requests....cl
+000000f0: 6173 7320 496e 7075 745f 6f75 7470 7574  ass Input_output
+00000100: 5f64 6174 613a 0d0a 2020 2020 6465 6620  _data:..    def 
+00000110: 5f5f 696e 6974 5f5f 2873 656c 662c 2075  __init__(self, u
+00000120: 2c20 792c 2073 616d 706c 696e 675f 7469  , y, sampling_ti
+00000130: 6d65 3d4e 6f6e 652c 206e 616d 653d 4e6f  me=None, name=No
+00000140: 6e65 2c20 6e5f 696e 6974 6961 6c69 7a61  ne, n_initializa
+00000150: 7469 6f6e 5f73 616d 706c 6573 3d4e 6f6e  tion_samples=Non
+00000160: 6529 3a0d 0a20 2020 2020 2020 2061 7373  e):..        ass
+00000170: 6572 7420 6c65 6e28 7529 3d3d 6c65 6e28  ert len(u)==len(
+00000180: 7929 2c20 6627 696e 7075 7420 7365 7175  y), f'input sequ
+00000190: 656e 6365 2075 206e 6565 6420 746f 2068  ence u need to h
+000001a0: 6176 6520 7468 6520 7361 6d65 206c 656e  ave the same len
+000001b0: 6774 6820 6173 2079 3a20 6375 7272 656e  gth as y: curren
+000001c0: 746c 7920 7b75 2e73 6861 7065 3d7d 2c20  tly {u.shape=}, 
+000001d0: 7b79 2e73 6861 7065 3d7d 270d 0a20 2020  {y.shape=}'..   
+000001e0: 2020 2020 2073 656c 662e 7520 3d20 750d       self.u = u.
+000001f0: 0a20 2020 2020 2020 2073 656c 662e 7920  .        self.y 
+00000200: 3d20 790d 0a20 2020 2020 2020 2073 656c  = y..        sel
+00000210: 662e 7361 6d70 6c69 6e67 5f74 696d 6520  f.sampling_time 
+00000220: 3d20 7361 6d70 6c69 6e67 5f74 696d 650d  = sampling_time.
+00000230: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
+00000240: 6d65 203d 2027 2720 6966 206e 616d 6520  me = '' if name 
+00000250: 6973 204e 6f6e 6520 656c 7365 206e 616d  is None else nam
+00000260: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00000270: 6e5f 696e 6974 6961 6c69 7a61 7469 6f6e  n_initialization
+00000280: 5f73 616d 706c 6573 203d 206e 5f69 6e69  _samples = n_ini
+00000290: 7469 616c 697a 6174 696f 6e5f 7361 6d70  tialization_samp
+000002a0: 6c65 730d 0a20 2020 200d 0a20 2020 2064  les..    ..    d
+000002b0: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
+000002c0: 293a 0d0a 2020 2020 2020 2020 7a20 3d20  ):..        z = 
+000002d0: 2727 2069 6620 2873 656c 662e 6e61 6d65  '' if (self.name
+000002e0: 3d3d 4e6f 6e65 206f 7220 7365 6c66 2e6e  ==None or self.n
+000002f0: 616d 653d 3d27 2729 2065 6c73 6520 6627  ame=='') else f'
+00000300: 2022 7b73 656c 662e 6e61 6d65 7d22 2720   "{self.name}"' 
+00000310: 0d0a 2020 2020 2020 2020 752c 2079 203d  ..        u, y =
+00000320: 2073 656c 662e 752c 2073 656c 662e 790d   self.u, self.y.
+00000330: 0a20 2020 2020 2020 2041 203d 2066 2773  .        A = f's
+00000340: 616d 706c 696e 675f 7469 6d65 3d7b 666c  ampling_time={fl
+00000350: 6f61 7428 7365 6c66 2e73 616d 706c 696e  oat(self.samplin
+00000360: 675f 7469 6d65 293a 2e34 7d27 2069 6620  g_time):.4}' if 
+00000370: 6973 696e 7374 616e 6365 2873 656c 662e  isinstance(self.
+00000380: 7361 6d70 6c69 6e67 5f74 696d 652c 204e  sampling_time, N
+00000390: 756d 6265 7229 2065 6c73 6520 2773 616d  umber) else 'sam
+000003a0: 706c 696e 675f 7469 6d65 3d44 6973 6372  pling_time=Discr
+000003b0: 6574 6520 7469 6d65 270d 0a20 2020 2020  ete time'..     
+000003c0: 2020 205a 203d 2066 2720 6e5f 696e 6974     Z = f' n_init
+000003d0: 6961 6c69 7a61 7469 6f6e 5f73 616d 706c  ialization_sampl
+000003e0: 6573 3d7b 7365 6c66 2e6e 5f69 6e69 7469  es={self.n_initi
+000003f0: 616c 697a 6174 696f 6e5f 7361 6d70 6c65  alization_sample
+00000400: 737d 2720 6966 2073 656c 662e 6e5f 696e  s}' if self.n_in
+00000410: 6974 6961 6c69 7a61 7469 6f6e 5f73 616d  itialization_sam
+00000420: 706c 6573 213d 4e6f 6e65 2065 6c73 6520  ples!=None else 
+00000430: 2727 0d0a 2020 2020 2020 2020 7265 7475  ''..        retu
+00000440: 726e 2066 2749 6e70 7574 5f6f 7574 7075  rn f'Input_outpu
+00000450: 745f 6461 7461 7b7a 7d20 7b75 2e73 6861  t_data{z} {u.sha
+00000460: 7065 3d7d 207b 792e 7368 6170 653d 7d20  pe=} {y.shape=} 
+00000470: 7b41 7d7b 5a7d 270d 0a20 2020 200d 0a20  {A}{Z}'..    .. 
+00000480: 2020 2064 6566 205f 5f69 7465 725f 5f28     def __iter__(
+00000490: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000004a0: 7969 656c 6420 7365 6c66 2e75 0d0a 2020  yield self.u..  
+000004b0: 2020 2020 2020 7969 656c 6420 7365 6c66        yield self
+000004c0: 2e79 0d0a 0d0a 2020 2020 6465 6620 5f5f  .y....    def __
+000004d0: 6c65 6e5f 5f28 7365 6c66 293a 0d0a 2020  len__(self):..  
+000004e0: 2020 2020 2020 7265 7475 726e 206c 656e        return len
+000004f0: 2873 656c 662e 7929 0d0a 2020 2020 0d0a  (self.y)..    ..
+00000500: 2020 2020 6465 6620 5f5f 6765 7469 7465      def __getite
+00000510: 6d5f 5f28 7365 6c66 2c61 7267 293a 0d0a  m__(self,arg):..
+00000520: 2020 2020 2020 2020 2727 2753 6c69 6365          '''Slice
+00000530: 2074 6865 2053 7973 7465 6d5f 6461 7461   the System_data
+00000540: 2069 6e20 7469 6d65 2069 6e64 6578 2727   in time index''
+00000550: 270d 0a20 2020 2020 2020 2069 6620 6973  '..        if is
+00000560: 696e 7374 616e 6365 2861 7267 2c20 696e  instance(arg, in
+00000570: 7429 3a0d 0a20 2020 2020 2020 2020 2020  t):..           
+00000580: 2069 6620 6172 673d 3d30 3a0d 0a20 2020   if arg==0:..   
+00000590: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000005a0: 7572 6e20 7365 6c66 2e75 0d0a 2020 2020  urn self.u..    
+000005b0: 2020 2020 2020 2020 656c 6966 2061 7267          elif arg
+000005c0: 3d3d 313a 0d0a 2020 2020 2020 2020 2020  ==1:..          
+000005d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000005e0: 662e 790d 0a20 2020 2020 2020 2020 2020  f.y..           
+000005f0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00000600: 7228 6627 6966 2061 7267 756d 656e 7420  r(f'if argument 
+00000610: 7b61 7267 7d20 6973 2061 2069 6e74 2074  {arg} is a int t
+00000620: 6861 6e20 6f6e 6c79 2030 2066 6f72 2075  han only 0 for u
+00000630: 2061 6e64 2031 2066 6f72 2079 2063 616e   and 1 for y can
+00000640: 2062 6520 7573 6564 2729 0d0a 2020 2020   be used')..    
+00000650: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+00000660: 6e63 6528 6172 672c 736c 6963 6529 3a0d  nce(arg,slice):.
+00000670: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00000680: 7274 2c20 7374 6f70 2c20 7374 6570 203d  rt, stop, step =
+00000690: 2061 7267 2e69 6e64 6963 6573 286c 656e   arg.indices(len
+000006a0: 2873 656c 662e 7529 290d 0a20 2020 2020  (self.u))..     
+000006b0: 2020 2020 2020 2075 6e65 7720 3d20 7365         unew = se
+000006c0: 6c66 2e75 5b61 7267 5d0d 0a20 2020 2020  lf.u[arg]..     
+000006d0: 2020 2020 2020 2079 6e65 7720 3d20 7365         ynew = se
+000006e0: 6c66 2e79 5b61 7267 5d0d 0a20 2020 2020  lf.y[arg]..     
+000006f0: 2020 2020 2020 2072 6574 7572 6e20 496e         return In
+00000700: 7075 745f 6f75 7470 7574 5f64 6174 6128  put_output_data(
+00000710: 753d 756e 6577 2c20 793d 796e 6577 2c20  u=unew, y=ynew, 
+00000720: 7361 6d70 6c69 6e67 5f74 696d 653d 7365  sampling_time=se
+00000730: 6c66 2e73 616d 706c 696e 675f 7469 6d65  lf.sampling_time
+00000740: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+00000750: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00000760: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+00000770: 2761 7267 756d 656e 7420 7769 7468 2076  'argument with v
+00000780: 616c 7565 2022 7b61 7267 7d22 206f 6620  alue "{arg}" of 
+00000790: 5f5f 6765 7469 7465 6d5f 5f20 6f66 2074  __getitem__ of t
+000007a0: 7970 6520 227b 7479 7065 2861 7267 297d  ype "{type(arg)}
+000007b0: 2220 6973 206e 6f74 2061 6c6c 6f77 6564  " is not allowed
+000007c0: 2729 0d0a 2020 2020 0d0a 2020 2020 6465  ')..    ..    de
+000007d0: 6620 6174 6c65 6173 745f 3264 2873 656c  f atleast_2d(sel
+000007e0: 6629 3a0d 0a20 2020 2020 2020 2076 203d  f):..        v =
+000007f0: 206c 616d 6264 6120 783a 2078 2069 6620   lambda x: x if 
+00000800: 782e 6e64 696d 3e31 2065 6c73 6520 785b  x.ndim>1 else x[
+00000810: 3a2c 4e6f 6e65 5d0d 0a20 2020 2020 2020  :,None]..       
+00000820: 2072 6574 7572 6e20 496e 7075 745f 6f75   return Input_ou
+00000830: 7470 7574 5f64 6174 6128 753d 7628 7365  tput_data(u=v(se
+00000840: 6c66 2e75 292c 2079 3d76 2873 656c 662e  lf.u), y=v(self.
+00000850: 7929 2c20 5c0d 0a20 2020 2020 2020 2020  y), \..         
+00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000870: 2020 2020 2020 2073 616d 706c 696e 675f         sampling_
+00000880: 7469 6d65 3d73 656c 662e 7361 6d70 6c69  time=self.sampli
+00000890: 6e67 5f74 696d 652c 205c 0d0a 2020 2020  ng_time, \..    
+000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000008c0: 3d73 656c 662e 6e61 6d65 2c20 5c0d 0a20  =self.name, \.. 
+000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000008f0: 5f69 6e69 7469 616c 697a 6174 696f 6e5f  _initialization_
+00000900: 7361 6d70 6c65 733d 7365 6c66 2e6e 5f69  samples=self.n_i
+00000910: 6e69 7469 616c 697a 6174 696f 6e5f 7361  nitialization_sa
+00000920: 6d70 6c65 7329 0d0a 0d0a 6465 6620 6174  mples)....def at
+00000930: 6c65 6173 745f 3264 5f66 756e 282a 6461  least_2d_fun(*da
+00000940: 7461 2c20 6170 706c 793d 5472 7565 293a  ta, apply=True):
+00000950: 0d0a 2020 2020 6966 206c 656e 2864 6174  ..    if len(dat
+00000960: 6129 3d3d 313a 0d0a 2020 2020 2020 2020  a)==1:..        
+00000970: 6461 7461 203d 2064 6174 615b 305d 0d0a  data = data[0]..
+00000980: 2020 2020 6966 2061 7070 6c79 3d3d 4661      if apply==Fa
+00000990: 6c73 653a 0d0a 2020 2020 2020 2020 7265  lse:..        re
+000009a0: 7475 726e 2064 6174 610d 0a20 2020 2069  turn data..    i
+000009b0: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
+000009c0: 612c 2049 6e70 7574 5f6f 7574 7075 745f  a, Input_output_
+000009d0: 6461 7461 293a 0d0a 2020 2020 2020 2020  data):..        
+000009e0: 7265 7475 726e 2064 6174 612e 6174 6c65  return data.atle
+000009f0: 6173 745f 3264 2829 0d0a 2020 2020 656c  ast_2d()..    el
+00000a00: 7365 3a0d 0a20 2020 2020 2020 2072 6574  se:..        ret
+00000a10: 7572 6e20 5b61 746c 6561 7374 5f32 645f  urn [atleast_2d_
+00000a20: 6675 6e28 642c 2061 7070 6c79 3d61 7070  fun(d, apply=app
+00000a30: 6c79 2920 666f 7220 6420 696e 2064 6174  ly) for d in dat
+00000a40: 615d 0d0a 0d0a 0d0a 6465 6620 6765 745f  a]......def get_
+00000a50: 746d 705f 6265 6e63 686d 6172 6b5f 6469  tmp_benchmark_di
+00000a60: 7265 6374 6f72 7928 293a 0d0a 2020 2020  rectory():..    
+00000a70: 2727 2741 2075 7469 6c69 7479 2066 756e  '''A utility fun
+00000a80: 6374 696f 6e20 7768 6963 6820 6765 7473  ction which gets
+00000a90: 2074 6865 2075 7469 6c69 7479 2064 6972   the utility dir
+00000aa0: 6563 746f 7269 6573 2066 6f72 2065 6163  ectories for eac
+00000ab0: 6820 4f53 0d0a 0d0a 2020 2020 4974 2063  h OS....    It c
+00000ac0: 7265 6174 6573 2061 2077 6f72 6b69 6e67  reates a working
+00000ad0: 2064 6972 6563 746f 7279 2063 616c 6c65   directory calle
+00000ae0: 6420 6e6f 6e6c 696e 6561 725f 6265 6e63  d nonlinear_benc
+00000af0: 686d 6172 6b73 200d 0a0d 0a20 2020 2020  hmarks ....     
+00000b00: 2020 2069 6e20 4c4f 4341 4c41 5050 4441     in LOCALAPPDA
+00000b10: 5441 2066 6f72 2077 696e 646f 7773 0d0a  TA for windows..
+00000b20: 0d0a 2020 2020 2020 2020 696e 207e 2f2e  ..        in ~/.
+00000b30: 6e6f 6e6c 696e 6561 725f 6265 6e63 686d  nonlinear_benchm
+00000b40: 6172 6b73 2f20 666f 7220 756e 6978 206c  arks/ for unix l
+00000b50: 696b 650d 0a0d 0a20 2020 2020 2020 2069  ike....        i
+00000b60: 6e20 7e2f 4c69 6272 6172 792f 4170 706c  n ~/Library/Appl
+00000b70: 6963 6174 696f 6e20 5375 7070 6f72 742f  ication Support/
+00000b80: 6e6f 6e6c 696e 6561 725f 6265 6e63 686d  nonlinear_benchm
+00000b90: 6172 6b73 2f20 666f 7220 6461 7277 696e  arks/ for darwin
+00000ba0: 0d0a 0d0a 2020 2020 6974 2063 7265 6174  ....    it creat
+00000bb0: 6573 2074 776f 2064 6972 6563 746f 7269  es two directori
+00000bc0: 6573 2069 6e73 6964 6520 6f66 2074 6865  es inside of the
+00000bd0: 206e 6f6e 6c69 6e65 6172 5f62 656e 6368   nonlinear_bench
+00000be0: 6d61 726b 7320 6469 7265 6374 6f72 790d  marks directory.
+00000bf0: 0a0d 0a20 2020 2020 2020 2064 6174 615f  ...        data_
+00000c00: 7365 7473 203a 2063 6163 6865 206c 6f63  sets : cache loc
+00000c10: 6174 696f 6e20 6f66 2074 6865 2064 6f77  ation of the dow
+00000c20: 6e6c 6f61 6465 6420 6461 7461 2073 6574  nloaded data set
+00000c30: 730d 0a0d 0a20 2020 2020 2020 2063 6865  s....        che
+00000c40: 636b 706f 696e 7473 203a 2075 7365 6420  ckpoints : used 
+00000c50: 6475 7269 6e67 2074 7261 696e 696e 6720  during training 
+00000c60: 6f66 2074 6f72 6368 206d 6f64 656c 730d  of torch models.
+00000c70: 0a0d 0a20 2020 2052 6574 7572 6e73 0d0a  ...    Returns..
+00000c80: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+00000c90: 2064 6963 7428 6261 7365 3d62 6173 655f   dict(base=base_
+00000ca0: 6469 722c 2064 6174 615f 7365 7473 3d64  dir, data_sets=d
+00000cb0: 6174 615f 7365 7473 5f64 6972 2c20 6368  ata_sets_dir, ch
+00000cc0: 6563 6b70 6f69 6e74 733d 6368 6563 6b70  eckpoints=checkp
+00000cd0: 6f69 6e74 735f 6469 7229 0d0a 2020 2020  oints_dir)..    
+00000ce0: 2727 270d 0a0d 0a20 2020 2064 6566 206d  '''....    def m
+00000cf0: 6b64 6972 2864 6972 6563 746f 7279 293a  kdir(directory):
+00000d00: 0d0a 2020 2020 2020 2020 6966 206f 732e  ..        if os.
+00000d10: 7061 7468 2e69 7364 6972 2864 6972 6563  path.isdir(direc
+00000d20: 746f 7279 2920 6973 2046 616c 7365 3a0d  tory) is False:.
+00000d30: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
+00000d40: 6d6b 6469 7228 6469 7265 6374 6f72 7929  mkdir(directory)
+00000d50: 0d0a 0d0a 2020 2020 6672 6f6d 2073 7973  ....    from sys
+00000d60: 2069 6d70 6f72 7420 706c 6174 666f 726d   import platform
+00000d70: 0d0a 2020 2020 6966 2070 6c61 7466 6f72  ..    if platfor
+00000d80: 6d20 3d3d 2022 6461 7277 696e 223a 2023  m == "darwin": #
+00000d90: 6e6f 7420 7465 7374 6564 2062 7574 2068  not tested but h
+00000da0: 6572 6520 6974 2067 6f65 730d 0a20 2020  ere it goes..   
+00000db0: 2020 2020 2062 6173 655f 6469 7220 3d20       base_dir = 
+00000dc0: 6f73 2e70 6174 682e 6578 7061 6e64 7573  os.path.expandus
+00000dd0: 6572 2827 7e2f 4c69 6272 6172 792f 4170  er('~/Library/Ap
+00000de0: 706c 6963 6174 696f 6e20 5375 7070 6f72  plication Suppor
+00000df0: 742f 6e6f 6e6c 696e 6561 725f 6265 6e63  t/nonlinear_benc
+00000e00: 686d 6172 6b73 2f27 290d 0a20 2020 2065  hmarks/')..    e
+00000e10: 6c69 6620 706c 6174 666f 726d 203d 3d20  lif platform == 
+00000e20: 2277 696e 3332 223a 0d0a 2020 2020 2020  "win32":..      
+00000e30: 2020 6261 7365 5f64 6972 203d 206f 732e    base_dir = os.
+00000e40: 7061 7468 2e6a 6f69 6e28 6f73 2e67 6574  path.join(os.get
+00000e50: 656e 7628 274c 4f43 414c 4150 5044 4154  env('LOCALAPPDAT
+00000e60: 4127 292c 276e 6f6e 6c69 6e65 6172 5f62  A'),'nonlinear_b
+00000e70: 656e 6368 6d61 726b 732f 2729 0d0a 2020  enchmarks/')..  
+00000e80: 2020 656c 7365 3a20 2375 6e69 7820 6c69    else: #unix li
+00000e90: 6b65 2c20 6d69 6768 7420 6265 2070 726f  ke, might be pro
+00000ea0: 626c 656d 6174 6963 2066 6f72 2073 6f6d  blematic for som
+00000eb0: 6520 7765 6972 6420 6f70 6572 6174 696e  e weird operatin
+00000ec0: 6720 7379 7374 656d 732e 0d0a 2020 2020  g systems...    
+00000ed0: 2020 2020 6261 7365 5f64 6972 203d 206f      base_dir = o
+00000ee0: 732e 7061 7468 2e65 7870 616e 6475 7365  s.path.expanduse
+00000ef0: 7228 277e 2f2e 6e6f 6e6c 696e 6561 725f  r('~/.nonlinear_
+00000f00: 6265 6e63 686d 6172 6b73 2f27 2923 5061  benchmarks/')#Pa
+00000f10: 7468 2827 7e2f 2e6e 6f6e 6c69 6e65 6172  th('~/.nonlinear
+00000f20: 5f62 656e 6368 6d61 726b 732f 2729 0d0a  _benchmarks/')..
+00000f30: 2020 2020 6d6b 6469 7228 6261 7365 5f64      mkdir(base_d
+00000f40: 6972 290d 0a20 2020 2072 6574 7572 6e20  ir)..    return 
+00000f50: 6261 7365 5f64 6972 0d0a 0d0a 6465 6620  base_dir....def 
+00000f60: 636c 6561 725f 6361 6368 6528 293a 0d0a  clear_cache():..
+00000f70: 2020 2020 2727 2744 656c 6574 6520 616c      '''Delete al
+00000f80: 6c20 6361 6368 6564 2064 6f77 6e6c 6f61  l cached downloa
+00000f90: 6473 2727 270d 0a20 2020 200d 0a20 2020  ds'''..    ..   
+00000fa0: 2074 656d 705f 6469 7220 3d20 6765 745f   temp_dir = get_
+00000fb0: 746d 705f 6265 6e63 686d 6172 6b5f 6469  tmp_benchmark_di
+00000fc0: 7265 6374 6f72 7928 290d 0a20 2020 2066  rectory()..    f
+00000fd0: 6f72 206c 2069 6e20 5b27 454d 5053 272c  or l in ['EMPS',
+00000fe0: 2743 4544 272c 2746 3136 272c 2757 6965  'CED','F16','Wie
+00000ff0: 6e48 616d 6d65 7227 2c27 426f 7563 5765  nHammer','BoucWe
+00001000: 6e27 2c27 5061 7257 4846 272c 2757 6965  n','ParWHF','Wie
+00001010: 6e65 7248 616d 6d65 7242 656e 6368 4d61  nerHammerBenchMa
+00001020: 726b 272c 2753 696c 7665 7262 6f78 272c  rk','Silverbox',
+00001030: 2743 6173 6361 6465 645f 5461 6e6b 7327  'Cascaded_Tanks'
+00001040: 5d3a 0d0a 2020 2020 2020 2020 7472 793a  ]:..        try:
+00001050: 0d0a 2020 2020 2020 2020 2020 2020 7368  ..            sh
+00001060: 7574 696c 2e72 6d74 7265 6528 6f73 2e70  util.rmtree(os.p
+00001070: 6174 682e 6a6f 696e 2874 656d 705f 6469  ath.join(temp_di
+00001080: 722c 6c29 290d 0a20 2020 2020 2020 2065  r,l))..        e
+00001090: 7863 6570 7420 4669 6c65 4e6f 7446 6f75  xcept FileNotFou
+000010a0: 6e64 4572 726f 723a 0d0a 2020 2020 2020  ndError:..      
+000010b0: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
+000010c0: 7472 793a 0d0a 2020 2020 2020 2020 7368  try:..        sh
+000010d0: 7574 696c 2e72 6d74 7265 6528 6f73 2e70  util.rmtree(os.p
+000010e0: 6174 682e 6a6f 696e 2874 656d 705f 6469  ath.join(temp_di
+000010f0: 722c 2744 6149 5379 5f64 6174 6127 2929  r,'DaISy_data'))
+00001100: 0d0a 2020 2020 6578 6365 7074 2046 696c  ..    except Fil
+00001110: 654e 6f74 466f 756e 6445 7272 6f72 3a0d  eNotFoundError:.
+00001120: 0a20 2020 2020 2020 2070 6173 730d 0a0d  .        pass...
+00001130: 0a0d 0a63 6c61 7373 204d 7950 726f 6772  ...class MyProgr
+00001140: 6573 7342 6172 2829 3a0d 0a20 2020 2064  essBar():..    d
+00001150: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00001160: 2c64 6f77 6e6c 6f61 645f 7369 7a65 293a  ,download_size):
+00001170: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00001180: 6261 7220 3d20 4e6f 6e65 0d0a 2020 2020  bar = None..    
+00001190: 2020 2020 7365 6c66 2e64 6f77 6e6c 6f61      self.downloa
+000011a0: 645f 7369 7a65 203d 2064 6f77 6e6c 6f61  d_size = downloa
+000011b0: 645f 7369 7a65 0d0a 0d0a 2020 2020 6465  d_size....    de
+000011c0: 6620 5f5f 6361 6c6c 5f5f 2873 656c 662c  f __call__(self,
+000011d0: 2062 6c6f 636b 5f6e 756d 2c20 626c 6f63   block_num, bloc
+000011e0: 6b5f 7369 7a65 2c20 746f 7461 6c5f 7369  k_size, total_si
+000011f0: 7a65 293a 0d0a 2020 2020 2020 2020 746f  ze):..        to
+00001200: 7461 6c5f 7369 7a65 203d 2073 656c 662e  tal_size = self.
+00001210: 646f 776e 6c6f 6164 5f73 697a 650d 0a20  download_size.. 
+00001220: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00001230: 6c66 2e70 6261 723a 0d0a 2020 2020 2020  lf.pbar:..      
+00001240: 2020 2020 2020 7365 6c66 2e70 6261 723d        self.pbar=
+00001250: 7072 6f67 7265 7373 6261 722e 5072 6f67  progressbar.Prog
+00001260: 7265 7373 4261 7228 6d61 7876 616c 3d74  ressBar(maxval=t
+00001270: 6f74 616c 5f73 697a 6529 0d0a 2020 2020  otal_size)..    
+00001280: 2020 2020 2020 2020 7365 6c66 2e70 6261          self.pba
+00001290: 722e 7374 6172 7428 290d 0a0d 0a20 2020  r.start()....   
+000012a0: 2020 2020 2064 6f77 6e6c 6f61 6465 6420       downloaded 
+000012b0: 3d20 626c 6f63 6b5f 6e75 6d20 2a20 626c  = block_num * bl
+000012c0: 6f63 6b5f 7369 7a65 0d0a 2020 2020 2020  ock_size..      
+000012d0: 2020 6966 2064 6f77 6e6c 6f61 6465 6420    if downloaded 
+000012e0: 3c20 746f 7461 6c5f 7369 7a65 3a0d 0a20  < total_size:.. 
+000012f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001300: 7062 6172 2e75 7064 6174 6528 646f 776e  pbar.update(down
+00001310: 6c6f 6164 6564 290d 0a20 2020 2020 2020  loaded)..       
+00001320: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00001330: 2020 2020 7365 6c66 2e70 6261 722e 6669      self.pbar.fi
+00001340: 6e69 7368 2829 0d0a 0d0a 0d0a 6465 6620  nish()......def 
+00001350: 6361 7368 6564 5f64 6f77 6e6c 6f61 6428  cashed_download(
+00001360: 7572 6c2c 6e61 6d65 5f64 6972 2c7a 6970  url,name_dir,zip
+00001370: 5f6e 616d 653d 4e6f 6e65 2c64 6972 5f70  _name=None,dir_p
+00001380: 6c61 6365 6d65 6e74 3d4e 6f6e 652c 646f  lacement=None,do
+00001390: 776e 6c6f 6164 5f73 697a 653d 4e6f 6e65  wnload_size=None
+000013a0: 2c66 6f72 6365 5f64 6f77 6e6c 6f61 643d  ,force_download=
+000013b0: 4661 6c73 652c 7a69 7070 6564 3d54 7275  False,zipped=Tru
+000013c0: 6529 3a0d 0a20 2020 2027 2727 7572 6c20  e):..    '''url 
+000013d0: 6973 2074 6865 2066 696c 6520 746f 2062  is the file to b
+000013e0: 6520 646f 776e 6c6f 6164 6564 0d0a 2020  e downloaded..  
+000013f0: 2020 6e61 6d65 5f64 6972 2069 7320 7468    name_dir is th
+00001400: 6520 6469 7265 6374 6f72 7920 6e61 6d65  e directory name
+00001410: 2077 6865 7265 2074 6865 2066 696c 6520   where the file 
+00001420: 616e 6420 7468 6520 636f 6e74 656e 7473  and the contents
+00001430: 206f 6620 7468 6520 6669 6c65 2077 696c   of the file wil
+00001440: 6c20 6265 2073 6176 6564 0d0a 2020 2020  l be saved..    
+00001450: 6469 725f 706c 6163 656d 656e 7420 6973  dir_placement is
+00001460: 2061 6e20 6f70 7469 6f6e 616c 2061 7267   an optional arg
+00001470: 756d 656e 7420 7468 6174 2067 6976 6573  ument that gives
+00001480: 2074 6865 206c 6f63 6174 696f 6e20 6f66   the location of
+00001490: 2074 6865 2064 6f77 6e6c 6f61 6465 6420   the downloaded 
+000014a0: 6669 6c65 200d 0a20 2020 2069 6620 6974  file ..    if it
+000014b0: 2069 7320 6e6f 6e65 2069 7420 7769 6c6c   is none it will
+000014c0: 2064 6f77 6e6c 6f61 6420 746f 2074 6865   download to the
+000014d0: 2074 656d 7020 6469 720d 0a20 2020 2069   temp dir..    i
+000014e0: 6620 6469 725f 6e61 6d65 2069 7320 4e6f  f dir_name is No
+000014f0: 6e65 2069 7420 7769 6c6c 2062 6520 7361  ne it will be sa
+00001500: 7665 6420 696e 2074 6865 2074 656d 7020  ved in the temp 
+00001510: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
+00001520: 2073 7973 7465 6d27 2727 0d0a 0d0a 2020   system'''....  
+00001530: 2020 2366 696e 6469 6e67 2f6d 616b 696e    #finding/makin
+00001540: 6720 6469 7265 6374 6f72 6965 730d 0a20  g directories.. 
+00001550: 2020 2069 6620 6469 725f 706c 6163 656d     if dir_placem
+00001560: 656e 7420 6973 204e 6f6e 653a 0d0a 2020  ent is None:..  
+00001570: 2020 2020 2020 7020 3d20 6765 745f 746d        p = get_tm
+00001580: 705f 6265 6e63 686d 6172 6b5f 6469 7265  p_benchmark_dire
+00001590: 6374 6f72 7928 2920 2375 7365 2074 656d  ctory() #use tem
+000015a0: 7020 6469 720d 0a20 2020 2065 6c73 653a  p dir..    else:
+000015b0: 0d0a 2020 2020 2020 2020 7020 3d20 5061  ..        p = Pa
+000015c0: 7468 2864 6972 5f70 6c61 6365 6d65 6e74  th(dir_placement
+000015d0: 2920 2375 7365 2067 6976 656e 2064 6972  ) #use given dir
+000015e0: 0d0a 2020 2020 7361 7665 5f64 6972 203d  ..    save_dir =
+000015f0: 206f 732e 7061 7468 2e6a 6f69 6e28 702c   os.path.join(p,
+00001600: 5061 7468 286e 616d 655f 6469 7229 290d  Path(name_dir)).
+00001610: 0a20 2020 2069 6620 6f73 2e70 6174 682e  .    if os.path.
+00001620: 6973 6469 7228 7361 7665 5f64 6972 2920  isdir(save_dir) 
+00001630: 6973 2046 616c 7365 3a0d 0a20 2020 2020  is False:..     
+00001640: 2020 206f 732e 6d6b 6469 7228 7361 7665     os.mkdir(save
+00001650: 5f64 6972 290d 0a20 2020 2066 696c 655f  _dir)..    file_
+00001660: 6e61 6d65 203d 2075 726c 2e73 706c 6974  name = url.split
+00001670: 2827 2f27 295b 2d31 5d20 6966 207a 6970  ('/')[-1] if zip
+00001680: 5f6e 616d 653d 3d4e 6f6e 6520 656c 7365  _name==None else
+00001690: 207a 6970 5f6e 616d 650d 0a20 2020 2073   zip_name..    s
+000016a0: 6176 655f 6c6f 6320 3d20 6f73 2e70 6174  ave_loc = os.pat
+000016b0: 682e 6a6f 696e 2873 6176 655f 6469 722c  h.join(save_dir,
+000016c0: 6669 6c65 5f6e 616d 6529 200d 0a0d 0a20  file_name) .... 
+000016d0: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
+000016e0: 6669 6c65 2873 6176 655f 6c6f 6329 2061  file(save_loc) a
+000016f0: 6e64 206e 6f74 2066 6f72 6365 5f64 6f77  nd not force_dow
+00001700: 6e6c 6f61 643a 0d0a 2020 2020 2020 2020  nload:..        
+00001710: 7265 7475 726e 2073 6176 655f 6469 720d  return save_dir.
+00001720: 0a0d 0a20 2020 2069 6620 666f 7263 655f  ...    if force_
+00001730: 646f 776e 6c6f 6164 3a0d 0a20 2020 2020  download:..     
+00001740: 2020 2070 7269 6e74 2866 2728 7265 2d29     print(f'(re-)
+00001750: 646f 776e 6c6f 6164 696e 6720 6461 7461  downloading data
+00001760: 7365 7420 6672 6f6d 207b 7572 6c7d 205c  set from {url} \
+00001770: 6e20 696e 207b 7361 7665 5f6c 6f63 7d27  n in {save_loc}'
+00001780: 290d 0a20 2020 2065 6c73 653a 0d0a 2020  )..    else:..  
+00001790: 2020 2020 2020 7072 696e 7428 6627 6461        print(f'da
+000017a0: 7461 7365 7420 6e6f 7420 666f 756e 6420  taset not found 
+000017b0: 646f 776e 6c6f 6164 696e 6720 6672 6f6d  downloading from
+000017c0: 207b 7572 6c7d 205c 6e20 696e 207b 7361   {url} \n in {sa
+000017d0: 7665 5f6c 6f63 7d27 290d 0a0d 0a20 2020  ve_loc}')....   
+000017e0: 2069 6620 2764 7269 7665 2e67 6f6f 676c   if 'drive.googl
+000017f0: 6527 2069 6e20 7572 6c3a 0d0a 2020 2020  e' in url:..    
+00001800: 2020 2020 646f 776e 6c6f 6164 5f66 696c      download_fil
+00001810: 655f 6672 6f6d 5f67 6f6f 676c 655f 6472  e_from_google_dr
+00001820: 6976 6528 7572 6c2c 2073 6176 655f 6c6f  ive(url, save_lo
+00001830: 6329 0d0a 2020 2020 656c 7365 3a0d 0a20  c)..    else:.. 
+00001840: 2020 2020 2020 2066 726f 6d20 6874 7470         from http
+00001850: 2e63 6c69 656e 7420 696d 706f 7274 2049  .client import I
+00001860: 6e63 6f6d 706c 6574 6552 6561 640d 0a20  ncompleteRead.. 
+00001870: 2020 2020 2020 2074 7269 6573 203d 2030         tries = 0
+00001880: 0d0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
+00001890: 5472 7565 3a0d 0a20 2020 2020 2020 2020  True:..         
+000018a0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+000018b0: 2020 2020 2020 2020 2069 6620 646f 776e           if down
+000018c0: 6c6f 6164 5f73 697a 6520 6973 204e 6f6e  load_size is Non
+000018d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000018e0: 2020 2020 2020 2020 7572 6c6c 6962 2e72          urllib.r
+000018f0: 6571 7565 7374 2e75 726c 7265 7472 6965  equest.urlretrie
+00001900: 7665 2875 726c 2c20 7361 7665 5f6c 6f63  ve(url, save_loc
+00001910: 2923 204d 7950 726f 6772 6573 7342 6172  )# MyProgressBar
+00001920: 2829 2069 7320 6120 7374 6561 6d20 736f  () is a steam so
+00001930: 206e 6f20 6c65 6e67 7468 2069 7320 6769   no length is gi
+00001940: 7665 6e0d 0a20 2020 2020 2020 2020 2020  ven..           
+00001950: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00001980: 2020 2020 2020 2020 2020 2075 726c 6c69             urlli
+00001990: 622e 7265 7175 6573 742e 7572 6c72 6574  b.request.urlret
+000019a0: 7269 6576 6528 7572 6c2c 2073 6176 655f  rieve(url, save_
+000019b0: 6c6f 632c 204d 7950 726f 6772 6573 7342  loc, MyProgressB
+000019c0: 6172 2864 6f77 6e6c 6f61 645f 7369 7a65  ar(download_size
+000019d0: 3d69 6e74 2864 6f77 6e6c 6f61 645f 7369  =int(download_si
+000019e0: 7a65 2929 290d 0a20 2020 2020 2020 2020  ze)))..         
+000019f0: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00001a00: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+00001a10: 6365 7074 2049 6e63 6f6d 706c 6574 6552  cept IncompleteR
+00001a20: 6561 643a 0d0a 2020 2020 2020 2020 2020  ead:..          
+00001a30: 2020 2020 2020 7472 6965 7320 2b3d 2031        tries += 1
+00001a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001a50: 2020 7072 696e 7428 2749 6e63 6f6d 706c    print('Incompl
+00001a60: 6574 6552 6561 6420 646f 776e 6c6f 6164  eteRead download
+00001a70: 2066 6169 6c65 642c 2072 652d 646f 776e   failed, re-down
+00001a80: 6c6f 6164 696e 6720 6669 6c65 2729 0d0a  loading file')..
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 646f 776e 6c6f 6164 5f73 697a 6520 3d20  download_size = 
+00001ab0: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+00001ac0: 2020 2020 2020 6966 2074 7269 6573 3d3d        if tries==
+00001ad0: 353a 0d0a 2020 2020 2020 2020 2020 2020  5:..            
+00001ae0: 2020 2020 2020 2020 6173 7365 7274 2046          assert F
+00001af0: 616c 7365 2c20 2744 6f77 6e6c 6f61 6420  alse, 'Download 
+00001b00: 4661 696c 2035 2074 696d 6573 2065 7869  Fail 5 times exi
+00001b10: 7469 6e67 2e27 0d0a 0d0a 0d0a 2020 2020  ting.'......    
+00001b20: 6966 206e 6f74 207a 6970 7065 643a 2072  if not zipped: r
+00001b30: 6574 7572 6e20 7361 7665 5f64 6972 0d0a  eturn save_dir..
+00001b40: 2020 2020 7072 696e 7428 2765 7874 7261      print('extra
+00001b50: 6374 696e 6720 6669 6c65 2e2e 2e27 290d  cting file...').
+00001b60: 0a20 2020 2070 7269 6e74 2866 277b 7361  .    print(f'{sa
+00001b70: 7665 5f6c 6f63 3d7d 2729 0d0a 2020 2020  ve_loc=}')..    
+00001b80: 656e 6469 6e67 203d 2066 696c 655f 6e61  ending = file_na
+00001b90: 6d65 2e73 706c 6974 2827 2e27 295b 2d31  me.split('.')[-1
+00001ba0: 5d0d 0a20 2020 2069 6620 656e 6469 6e67  ]..    if ending
+00001bb0: 3d3d 2767 7a27 3a0d 0a20 2020 2020 2020  =='gz':..       
+00001bc0: 2069 6d70 6f72 7420 7368 7574 696c 0d0a   import shutil..
+00001bd0: 2020 2020 2020 2020 696d 706f 7274 2067          import g
+00001be0: 7a69 700d 0a20 2020 2020 2020 2077 6974  zip..        wit
+00001bf0: 6820 6f70 656e 286f 732e 7061 7468 2e6a  h open(os.path.j
+00001c00: 6f69 6e28 7361 7665 5f64 6972 2c66 696c  oin(save_dir,fil
+00001c10: 655f 6e61 6d65 5b3a 2d33 5d29 2c20 2777  e_name[:-3]), 'w
+00001c20: 6227 2920 6173 2066 5f6f 7574 3a0d 0a20  b') as f_out:.. 
+00001c30: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00001c40: 677a 6970 2e6f 7065 6e28 7361 7665 5f6c  gzip.open(save_l
+00001c50: 6f63 2c20 2772 6227 2920 6173 2066 5f69  oc, 'rb') as f_i
+00001c60: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
+00001c70: 2020 2020 7368 7574 696c 2e63 6f70 7966      shutil.copyf
+00001c80: 696c 656f 626a 2866 5f69 6e2c 2066 5f6f  ileobj(f_in, f_o
+00001c90: 7574 290d 0a20 2020 2065 6c69 6620 656e  ut)..    elif en
+00001ca0: 6469 6e67 3d3d 277a 6970 273a 0d0a 2020  ding=='zip':..  
+00001cb0: 2020 2020 2020 6672 6f6d 207a 6970 6669        from zipfi
+00001cc0: 6c65 2069 6d70 6f72 7420 5a69 7046 696c  le import ZipFil
+00001cd0: 6520 6173 2046 696c 650d 0a20 2020 2020  e as File..     
+00001ce0: 2020 2077 6974 6820 4669 6c65 2873 6176     with File(sav
+00001cf0: 655f 6c6f 6329 2061 7320 4f62 6a3a 0d0a  e_loc) as Obj:..
+00001d00: 2020 2020 2020 2020 2020 2020 4f62 6a2e              Obj.
+00001d10: 6578 7472 6163 7461 6c6c 2873 6176 655f  extractall(save_
+00001d20: 6469 7229 0d0a 2020 2020 656c 6966 2065  dir)..    elif e
+00001d30: 6e64 696e 673d 3d27 7261 7227 3a0d 0a20  nding=='rar':.. 
+00001d40: 2020 2020 2020 2066 726f 6d20 7261 7266         from rarf
+00001d50: 696c 6520 696d 706f 7274 2052 6172 4669  ile import RarFi
+00001d60: 6c65 2061 7320 4669 6c65 0d0a 2020 2020  le as File..    
+00001d70: 2020 2020 7769 7468 2046 696c 6528 7361      with File(sa
+00001d80: 7665 5f6c 6f63 2920 6173 204f 626a 3a0d  ve_loc) as Obj:.
+00001d90: 0a20 2020 2020 2020 2020 2020 204f 626a  .            Obj
+00001da0: 2e65 7874 7261 6374 616c 6c28 7361 7665  .extractall(save
+00001db0: 5f64 6972 290d 0a20 2020 2065 6c73 653a  _dir)..    else:
+00001dc0: 0d0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
+00001dd0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00001de0: 726f 7228 6627 6669 6c65 207b 6669 6c65  ror(f'file {file
+00001df0: 5f6e 616d 657d 2074 7970 6520 6e6f 7420  _name} type not 
+00001e00: 696d 706c 656d 656e 7465 6427 290d 0a20  implemented').. 
+00001e10: 2020 2072 6574 7572 6e20 7361 7665 5f64     return save_d
+00001e20: 6972 0d0a 0d0a 0d0a 6465 6620 646f 776e  ir......def down
+00001e30: 6c6f 6164 5f66 696c 655f 6672 6f6d 5f67  load_file_from_g
+00001e40: 6f6f 676c 655f 6472 6976 6528 7572 6c2c  oogle_drive(url,
+00001e50: 2064 6573 7469 6e61 7469 6f6e 293a 0d0a   destination):..
+00001e60: 2020 2020 6964 203d 2075 726c 2e73 706c      id = url.spl
+00001e70: 6974 2827 2f27 295b 2d32 5d0d 0a20 2020  it('/')[-2]..   
+00001e80: 2055 524c 203d 2022 6874 7470 733a 2f2f   URL = "https://
+00001e90: 646f 6373 2e67 6f6f 676c 652e 636f 6d2f  docs.google.com/
+00001ea0: 7563 3f65 7870 6f72 743d 646f 776e 6c6f  uc?export=downlo
+00001eb0: 6164 220d 0a0d 0a20 2020 2073 6573 7369  ad"....    sessi
+00001ec0: 6f6e 203d 2072 6571 7565 7374 732e 5365  on = requests.Se
+00001ed0: 7373 696f 6e28 290d 0a0d 0a20 2020 2072  ssion()....    r
+00001ee0: 6573 706f 6e73 6520 3d20 7365 7373 696f  esponse = sessio
+00001ef0: 6e2e 6765 7428 5552 4c2c 2070 6172 616d  n.get(URL, param
+00001f00: 7320 3d20 7b20 2769 6427 203a 2069 6420  s = { 'id' : id 
+00001f10: 7d2c 2073 7472 6561 6d20 3d20 5472 7565  }, stream = True
+00001f20: 290d 0a20 2020 2074 6f6b 656e 203d 2067  )..    token = g
+00001f30: 6574 5f63 6f6e 6669 726d 5f74 6f6b 656e  et_confirm_token
+00001f40: 2872 6573 706f 6e73 6529 0d0a 0d0a 2020  (response)....  
+00001f50: 2020 6966 2074 6f6b 656e 3a0d 0a20 2020    if token:..   
+00001f60: 2020 2020 2070 6172 616d 7320 3d20 7b20       params = { 
+00001f70: 2769 6427 203a 2069 642c 2027 636f 6e66  'id' : id, 'conf
+00001f80: 6972 6d27 203a 2074 6f6b 656e 207d 0d0a  irm' : token }..
+00001f90: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00001fa0: 203d 2073 6573 7369 6f6e 2e67 6574 2855   = session.get(U
+00001fb0: 524c 2c20 7061 7261 6d73 203d 2070 6172  RL, params = par
+00001fc0: 616d 732c 2073 7472 6561 6d20 3d20 5472  ams, stream = Tr
+00001fd0: 7565 290d 0a0d 0a20 2020 2073 6176 655f  ue)....    save_
+00001fe0: 7265 7370 6f6e 7365 5f63 6f6e 7465 6e74  response_content
+00001ff0: 2872 6573 706f 6e73 652c 2064 6573 7469  (response, desti
+00002000: 6e61 7469 6f6e 2920 2020 200d 0a0d 0a64  nation)    ....d
+00002010: 6566 2067 6574 5f63 6f6e 6669 726d 5f74  ef get_confirm_t
+00002020: 6f6b 656e 2872 6573 706f 6e73 6529 3a0d  oken(response):.
+00002030: 0a20 2020 2066 6f72 206b 6579 2c20 7661  .    for key, va
+00002040: 6c75 6520 696e 2072 6573 706f 6e73 652e  lue in response.
+00002050: 636f 6f6b 6965 732e 6974 656d 7328 293a  cookies.items():
+00002060: 0d0a 2020 2020 2020 2020 6966 206b 6579  ..        if key
+00002070: 2e73 7461 7274 7377 6974 6828 2764 6f77  .startswith('dow
+00002080: 6e6c 6f61 645f 7761 726e 696e 6727 293a  nload_warning'):
+00002090: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000020a0: 7475 726e 2076 616c 7565 0d0a 0d0a 2020  turn value....  
+000020b0: 2020 7265 7475 726e 204e 6f6e 650d 0a0d    return None...
+000020c0: 0a64 6566 2073 6176 655f 7265 7370 6f6e  .def save_respon
+000020d0: 7365 5f63 6f6e 7465 6e74 2872 6573 706f  se_content(respo
+000020e0: 6e73 652c 2064 6573 7469 6e61 7469 6f6e  nse, destination
+000020f0: 293a 0d0a 2020 2020 4348 554e 4b5f 5349  ):..    CHUNK_SI
+00002100: 5a45 203d 2033 3237 3638 0d0a 0d0a 2020  ZE = 32768....  
+00002110: 2020 7769 7468 206f 7065 6e28 6465 7374    with open(dest
+00002120: 696e 6174 696f 6e2c 2022 7762 2229 2061  ination, "wb") a
+00002130: 7320 663a 0d0a 2020 2020 2020 2020 666f  s f:..        fo
+00002140: 7220 6368 756e 6b20 696e 2072 6573 706f  r chunk in respo
+00002150: 6e73 652e 6974 6572 5f63 6f6e 7465 6e74  nse.iter_content
+00002160: 2843 4855 4e4b 5f53 495a 4529 3a0d 0a20  (CHUNK_SIZE):.. 
+00002170: 2020 2020 2020 2020 2020 2069 6620 6368             if ch
+00002180: 756e 6b3a 2023 2066 696c 7465 7220 6f75  unk: # filter ou
+00002190: 7420 6b65 6570 2d61 6c69 7665 206e 6577  t keep-alive new
+000021a0: 2063 6875 6e6b 730d 0a20 2020 2020 2020   chunks..       
+000021b0: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
+000021c0: 2863 6875 6e6b 290d 0a0d 0a23 2069 6620  (chunk)....# if 
+000021d0: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+000021e0: 6169 6e5f 5f27 3a0d 0a23 2020 2020 2069  ain__':..#     i
+000021f0: 6d70 6f72 7420 6e6f 6e6c 696e 6561 725f  mport nonlinear_
+00002200: 6265 6e63 686d 6172 6b73 0d0a 2320 2020  benchmarks..#   
+00002210: 2020 752c 7920 3d20 6e6f 6e6c 696e 6561    u,y = nonlinea
+00002220: 725f 6265 6e63 686d 6172 6b73 2e43 4544  r_benchmarks.CED
+00002230: 2873 706c 6974 5f64 6174 613d 4661 6c73  (split_data=Fals
+00002240: 6529 0d0a 2320 2020 2020 7379 735f 6461  e)..#     sys_da
+00002250: 7461 2e70 6c6f 7428 7368 6f77 3d54 7275  ta.plot(show=Tru
+00002260: 6529 0d0a 0d0a 2020 2020 2320 6669 6c65  e)....    # file
+00002270: 6e61 6d65 203d 2027 2e2f 6669 6c65 2e7a  name = './file.z
+00002280: 6970 270d 0a20 2020 2023 2075 726c 203d  ip'..    # url =
+00002290: 2027 6874 7470 3a2f 2f77 7777 2e6e 6f6e   'http://www.non
+000022a0: 6c69 6e65 6172 6265 6e63 686d 6172 6b2e  linearbenchmark.
+000022b0: 6f72 672f 4649 4c45 532f 4245 4e43 484d  org/FILES/BENCHM
+000022c0: 4152 4b53 2f45 4d50 532f 454d 5053 2e7a  ARKS/EMPS/EMPS.z
+000022d0: 6970 270d 0a20 2020 2023 2075 726c 6c69  ip'..    # urlli
+000022e0: 622e 7265 7175 6573 742e 7572 6c72 6574  b.request.urlret
+000022f0: 7269 6576 6528 7572 6c2c 2066 696c 656e  rieve(url, filen
+00002300: 616d 6529 0d0a 0d0a 2020 2020 2320 7265  ame)....    # re
+00002310: 7370 203d 2075 726c 6c69 622e 7265 7175  sp = urllib.requ
+00002320: 6573 742e 7572 6c6f 7065 6e28 7572 6c29  est.urlopen(url)
+00002330: 0d0a 2020 2020 2320 7265 7370 4874 6d6c  ..    # respHtml
+00002340: 203d 2072 6573 702e 7265 6164 2829 0d0a   = resp.read()..
+00002350: 2020 2020 2320 6269 6e66 696c 6520 3d20      # binfile = 
+00002360: 6f70 656e 2866 696c 656e 616d 652c 2022  open(filename, "
+00002370: 7762 2229 0d0a 2020 2020 2320 6269 6e66  wb")..    # binf
+00002380: 696c 652e 7772 6974 6528 7265 7370 4874  ile.write(respHt
+00002390: 6d6c 290d 0a20 2020 2023 2062 696e 6669  ml)..    # binfi
+000023a0: 6c65 2e63 6c6f 7365 2829 0d0a 0d0a 2020  le.close()....  
+000023b0: 2020
```

### Comparing `nonlinear_benchmarks-0.0.4/setup.cfg` & `nonlinear_benchmarks-0.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6f6e 6c69 6e65 6172 5f62 656e   = nonlinear_ben
 00000020: 6368 6d61 726b 730d 0a76 6572 7369 6f6e  chmarks..version
-00000030: 203d 2030 2e30 2e34 0d0a 6175 7468 6f72   = 0.0.4..author
+00000030: 203d 2030 2e31 2e30 0d0a 6175 7468 6f72   = 0.1.0..author
 00000040: 203d 2047 6572 6265 6e20 4265 696e 7465   = Gerben Beinte
 00000050: 6d61 0d0a 6175 7468 6f72 5f65 6d61 696c  ma..author_email
 00000060: 203d 2067 2e69 2e62 6569 6e74 656d 6140   = g.i.beintema@
 00000070: 7475 652e 6e6c 0d0a 6465 7363 7269 7074  tue.nl..descript
 00000080: 696f 6e20 3d20 5468 6520 6f66 6669 6369  ion = The offici
 00000090: 616c 2064 6174 616c 6f61 6420 666f 7220  al dataload for 
 000000a0: 6874 7470 3a2f 2f77 7777 2e6e 6f6e 6c69  http://www.nonli
```

### Comparing `nonlinear_benchmarks-0.0.4/setup.py` & `nonlinear_benchmarks-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 'scipy',
 'requests',
 'rarfile']
 
 packages = [a for a in find_namespace_packages(where='.') if a[:6]=='nonlinear_benchmarks']
 
 setup(name = 'nonlinear_benchmarks',
-      version = '0.0.4',
+      version = '0.1.0',
       description = 'The official dataload for http://www.nonlinearbenchmark.org/',
       author = 'Gerben Beintema',
       author_email = 'g.i.beintema@tue.nl',
       license = 'BSD 3-Clause License',
       python_requires = '>=3.6',
       packages=packages,
       install_requires = install_requires,
```

