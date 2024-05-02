# Comparing `tmp/sigmond_scripts-1.0.1.tar.gz` & `tmp/sigmond_scripts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmond_scripts-1.0.1.tar", last modified: Sun Apr 28 00:42:12 2024, max compression
+gzip compressed data, was "sigmond_scripts-1.0.2.tar", last modified: Thu May  2 13:46:26 2024, max compression
```

## Comparing `sigmond_scripts-1.0.1.tar` & `sigmond_scripts-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 00:42:12.473420 sigmond_scripts-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    35141 2024-04-24 16:22:10.000000 sigmond_scripts-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-28 00:42:12.473420 sigmond_scripts-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1307 2024-04-25 03:29:22.000000 sigmond_scripts-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      104 2024-04-24 16:34:39.000000 sigmond_scripts-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      628 2024-04-28 00:42:12.473420 sigmond_scripts-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 00:42:12.453420 sigmond_scripts-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 00:42:12.473420 sigmond_scripts-1.0.1/src/sigmond_scripts/
--rw-r--r--   0 root         (0) root         (0)        2 2024-04-25 03:37:53.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8422 2024-04-25 04:07:58.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/channel.py
--rw-r--r--   0 root         (0) root         (0)     5860 2024-04-25 03:53:23.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/correlator_data.py
--rw-r--r--   0 root         (0) root         (0)     5572 2024-04-25 03:54:45.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/data_files.py
--rw-r--r--   0 root         (0) root         (0)    18225 2024-04-26 15:02:28.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/data_handler.py
--rw-r--r--   0 root         (0) root         (0)    22391 2024-04-25 04:11:05.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/fit_info.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-24 16:34:39.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/isospin.py
--rw-r--r--   0 root         (0) root         (0)    13785 2024-04-25 04:08:30.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/operator.py
--rw-r--r--   0 root         (0) root         (0)     9681 2024-04-25 04:09:04.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/operator_set.py
--rw-r--r--   0 root         (0) root         (0)     9948 2024-04-25 04:10:28.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/sigmond_info.py
--rw-r--r--   0 root         (0) root         (0)    70514 2024-04-25 04:10:11.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/sigmond_input.py
--rw-r--r--   0 root         (0) root         (0)    38929 2024-04-27 18:43:48.000000 sigmond_scripts-1.0.1/src/sigmond_scripts/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 00:42:12.473420 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-28 00:42:12.000000 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      660 2024-04-28 00:42:12.000000 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 00:42:12.000000 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-28 00:42:12.000000 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-28 00:42:12.000000 sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/top_level.txt
+drwxr-xr-x   0 sarahski  (1140) lattice   (2100)        0 2024-05-02 13:46:26.586976 sigmond_scripts-1.0.2/
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)    35141 2023-11-12 18:14:19.000000 sigmond_scripts-1.0.2/LICENSE
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)     1902 2024-05-02 13:46:26.586976 sigmond_scripts-1.0.2/PKG-INFO
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)     1307 2024-04-25 03:28:41.000000 sigmond_scripts-1.0.2/README.md
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)      104 2024-03-06 15:19:28.000000 sigmond_scripts-1.0.2/pyproject.toml
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)      628 2024-05-02 13:46:26.588976 sigmond_scripts-1.0.2/setup.cfg
+drwxr-xr-x   0 sarahski  (1140) lattice   (2100)        0 2024-05-02 13:46:26.536975 sigmond_scripts-1.0.2/src/
+drwxr-xr-x   0 sarahski  (1140) lattice   (2100)        0 2024-05-02 13:46:26.561976 sigmond_scripts-1.0.2/src/sigmond_scripts/
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)        2 2024-04-29 12:55:42.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/__init__.py
+drwxr-xr-x   0 sarahski  (1140) lattice   (2100)        0 2024-05-02 13:46:26.574976 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)      277 2024-03-07 19:43:07.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/__init__.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)    15030 2023-11-12 18:14:19.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/launcher.py
+drwxr-xr-x   0 sarahski  (1140) lattice   (2100)        0 2024-05-02 13:46:26.575976 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/operator_info/
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)      277 2024-03-07 19:52:36.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/operator_info/__init__.py
+-rwxr-xr-x   0 sarahski  (1140) lattice   (2100)     1325 2023-11-12 18:14:19.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/run_sigmond.py
+drwxr-xr-x   0 sarahski  (1140) lattice   (2100)        0 2024-05-02 13:46:26.577976 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/sigmond_info/
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)      277 2024-03-07 19:53:16.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/sigmond_info/__init__.py
+drwxr-xr-x   0 sarahski  (1140) lattice   (2100)        0 2024-05-02 13:46:26.582976 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/utils/
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)      277 2024-03-07 19:47:53.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/utils/__init__.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)     1841 2023-11-12 18:14:19.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/utils/menu.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)    11219 2023-11-12 18:14:19.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/analysis/utils/plotting.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)     8422 2024-04-29 12:55:42.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/channel.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)     5860 2024-04-29 12:55:42.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/correlator_data.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)     5572 2024-04-29 12:55:42.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/data_files.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)    17418 2024-04-30 19:08:51.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/data_handler.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)    22391 2024-04-29 12:55:42.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/fit_info.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)      428 2024-04-29 12:55:42.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/isospin.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)    13785 2024-04-29 12:55:42.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/operator.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)     9681 2024-04-29 12:55:42.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/operator_set.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)     9948 2024-04-29 12:55:42.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/sigmond_info.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)    70514 2024-04-29 12:55:42.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/sigmond_input.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)    16504 2024-05-02 02:52:27.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/sigmond_log.py
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)    38929 2024-04-29 13:38:10.000000 sigmond_scripts-1.0.2/src/sigmond_scripts/util.py
+drwxr-xr-x   0 sarahski  (1140) lattice   (2100)        0 2024-05-02 13:46:26.584976 sigmond_scripts-1.0.2/src/sigmond_scripts.egg-info/
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)     1902 2024-05-02 13:46:26.000000 sigmond_scripts-1.0.2/src/sigmond_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)     1067 2024-05-02 13:46:26.000000 sigmond_scripts-1.0.2/src/sigmond_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)        1 2024-05-02 13:46:26.000000 sigmond_scripts-1.0.2/src/sigmond_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)       67 2024-05-02 13:46:26.000000 sigmond_scripts-1.0.2/src/sigmond_scripts.egg-info/requires.txt
+-rw-r--r--   0 sarahski  (1140) lattice   (2100)       16 2024-05-02 13:46:26.000000 sigmond_scripts-1.0.2/src/sigmond_scripts.egg-info/top_level.txt
```

### Comparing `sigmond_scripts-1.0.1/LICENSE` & `sigmond_scripts-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.1/PKG-INFO` & `sigmond_scripts-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmond_scripts
-Version: 1.0.1
+Version: 1.0.2
 Summary: Supporting functions for handling the c++ library sigmond
 Author: Drew Hanlon
 Author-email: ahanlon@bnl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `sigmond_scripts-1.0.1/README.md` & `sigmond_scripts-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.1/setup.cfg` & `sigmond_scripts-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sigmond_scripts
-version = 1.0.1
+version = 1.0.2
 author = Drew Hanlon
 author_email = ahanlon@bnl.gov
 description = Supporting functions for handling the c++ library sigmond
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts/channel.py` & `sigmond_scripts-1.0.2/src/sigmond_scripts/channel.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts/correlator_data.py` & `sigmond_scripts-1.0.2/src/sigmond_scripts/correlator_data.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts/data_files.py` & `sigmond_scripts-1.0.2/src/sigmond_scripts/data_files.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts/data_handler.py` & `sigmond_scripts-1.0.2/src/sigmond_scripts/data_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import h5py
 
-from typing import NamedTuple
 import logging
 from sortedcontainers import SortedSet
 import tqdm
+# import multiprocessing
+# import dill
 
 import sigmond_scripts.util as util
 from sigmond_scripts.data_files import DataFiles, FileInfo
 from sigmond_scripts.correlator_data import CorrelatorData
-from sigmond_scripts.operator import Operator
 
 import sigmond
 
 class DataHandler(metaclass=util.Singleton):
   """ The all important Data Handler!  """
 
   def __init__(self, project_info, shared_node = True, nodes=os.cpu_count()):
@@ -273,66 +273,59 @@
 
     logging.info("Searching through found raw data files...")
     self._raw_data += self._findLaphData(data_files)
 
     if data_files.bin_files:
       logging.info("Reading bin data")
       
-      # files = list(data_files.bin_files)
-      # if len(data_files.bin_files)>self.nodes:
-      #   nblock = int(len(data_files.bin_files)/self.nodes)+1
-      # else:
-      #   nblock = 1
-
-      # processes = []
-      # results = []
-      # for i in range(0,len(data_files.bin_files),nblock):
-      #   results.append(CorrelatorData())
-      #   if i>(len(data_files.bin_files)-nblock):
-      #     processes.append(threading.Thread(target=self._findSigmondDataSeries, args=(files[i:], sigmond.FileType.Bins, results[-1])))
-      #     processes[-1].start()
-      #     # self._raw_data += self._findSigmondDataSeries(files[i:], sigmond.FileType.Bins)
-      #   else:
-      #     processes.append(threading.Thread(target=self._findSigmondDataSeries, args=(files[i:i+nblock], sigmond.FileType.Bins, results[-1])))
-      #     processes[-1].start()
-      #     # self._raw_data += self._findSigmondDataSeries(files[i:i+nblock], sigmond.FileType.Bins)
-
-      # for process in tqdm.tqdm(processes):
-      #   process.join()
-      # args = []
-      # files = list(data_files.bin_files)
-      # if len(data_files.bin_files)>self.nodes:
-      #   nblock = int(len(data_files.bin_files)/self.nodes)+1
-      # else:
-      #   nblock = 1
-      # for i in tqdm.tqdm(range(0,len(data_files.bin_files),nblock)):
-      #   if i>(len(data_files.bin_files)-nblock):
-      #     args.append(files[i:])
-      #   else:
-      #     args.append(files[i:i+nblock])
-      # results = pqdm(args, self._findSigmondDataSeriesBins, n_jobs=self.nodes)
-      # # results = pqdm([[file, sigmond.FileType.Bins] for file in data_files.bin_files], self._findSigmondData, n_jobs=self.nodes, argument_type='args')
-      # print(results)
-      # for i in range(len(results)):
-      #   self._raw_data += results[i]
+    #   if self.nodes:
+    #     files = list(data_files.bin_files)
+    #     nblock = int(len(data_files.bin_files)/self.nodes)+1
+    #     blocked_files = [files[i:i+nblock] for i in range(0,len(data_files.bin_files),nblock)]
+    #     processes = []
+    #     results = []
+    #     q = multiprocessing.SimpleQueue()
+    #     dill.detect.trace(True)
+    #     dill.detect.errors(CorrelatorData())
+    #     for files in blocked_files:
+    #         results.append(CorrelatorData())
+    #         processes.append(multiprocessing.Process(target=self._findSigmondDataSeries,args=(files, sigmond.FileType.Bins,q)))
+    #         processes[-1].start()
+    #     print("processes started")
+
+    #     for process in processes:
+    #         print("\t getting")
+    #         self._raw_data += q.get()
+
+    #     for process in processes:
+    #         process.join()
+
+    #     q.close()
+
+    #     print("processes joined")
+
+    #   else:
       for bin_file in tqdm.tqdm(data_files.bin_files):
         self._raw_data += self._findSigmondData(bin_file, sigmond.FileType.Bins)
 
     if data_files.sampling_files:
       logging.info("Reading sampling data")
       for smp_file in tqdm.tqdm(data_files.sampling_files):
         self._raw_data += self._findSigmondData(smp_file, sigmond.FileType.Samplings)
 
     self.raw_data_files = data_files
     logging.info("done")
   
-  def _findSigmondDataSeries(self, files, filetype, data):
-    # data = CorrelatorData()
+  def _findSigmondDataSeries(self, files, filetype, q):
+    data = CorrelatorData()
     for file in files:
       data += self._findSigmondData(file, filetype)
+    print("done getting data")
+    q.put(data)
+    print("done putting data")
     # return data
   
   def _findSigmondDataRaw(self, files, filetype):
     # data = CorrelatorData()
     for file in files:
       self._raw_data += self._findSigmondData(file, filetype)
     # return data
```

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts/fit_info.py` & `sigmond_scripts-1.0.2/src/sigmond_scripts/fit_info.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts/operator.py` & `sigmond_scripts-1.0.2/src/sigmond_scripts/operator.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts/operator_set.py` & `sigmond_scripts-1.0.2/src/sigmond_scripts/operator_set.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts/sigmond_info.py` & `sigmond_scripts-1.0.2/src/sigmond_scripts/sigmond_info.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts/sigmond_input.py` & `sigmond_scripts-1.0.2/src/sigmond_scripts/sigmond_input.py`

 * *Files identical despite different names*

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts/util.py` & `sigmond_scripts-1.0.2/src/sigmond_scripts/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 
   return result_obs
 
 #########################################################################################
 # PDF documents
 def create_doc(title, with_tikz=False):
   logging.info("Creating PDF...")
-  doc = pylatex.Document(geometry_options={'margin': '1.5cm'},imputenc=None)
+  doc = pylatex.Document(geometry_options={'margin': '1.5cm'},inputenc=None)
   doc.packages.append(pylatex.Package('hyperref'))
   doc.packages.append(pylatex.Package('amssymb'))
   doc.packages.append(pylatex.Package('amsmath'))
   doc.packages.append(pylatex.Package('float'))
   doc.packages.append(pylatex.Package('xcolor'))
   doc.packages.append(pylatex.Package('caption', {'labelformat': 'empty', 'justification': 'centering'}))
 #   doc.packages.append(pylatex.Package('todonotes'))
```

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/PKG-INFO` & `sigmond_scripts-1.0.2/src/sigmond_scripts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmond_scripts
-Version: 1.0.1
+Version: 1.0.2
 Summary: Supporting functions for handling the c++ library sigmond
 Author: Drew Hanlon
 Author-email: ahanlon@bnl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `sigmond_scripts-1.0.1/src/sigmond_scripts.egg-info/SOURCES.txt` & `sigmond_scripts-1.0.2/src/sigmond_scripts.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,13 +9,22 @@
 src/sigmond_scripts/data_handler.py
 src/sigmond_scripts/fit_info.py
 src/sigmond_scripts/isospin.py
 src/sigmond_scripts/operator.py
 src/sigmond_scripts/operator_set.py
 src/sigmond_scripts/sigmond_info.py
 src/sigmond_scripts/sigmond_input.py
+src/sigmond_scripts/sigmond_log.py
 src/sigmond_scripts/util.py
 src/sigmond_scripts.egg-info/PKG-INFO
 src/sigmond_scripts.egg-info/SOURCES.txt
 src/sigmond_scripts.egg-info/dependency_links.txt
 src/sigmond_scripts.egg-info/requires.txt
-src/sigmond_scripts.egg-info/top_level.txt
+src/sigmond_scripts.egg-info/top_level.txt
+src/sigmond_scripts/analysis/__init__.py
+src/sigmond_scripts/analysis/launcher.py
+src/sigmond_scripts/analysis/run_sigmond.py
+src/sigmond_scripts/analysis/operator_info/__init__.py
+src/sigmond_scripts/analysis/sigmond_info/__init__.py
+src/sigmond_scripts/analysis/utils/__init__.py
+src/sigmond_scripts/analysis/utils/menu.py
+src/sigmond_scripts/analysis/utils/plotting.py
```

