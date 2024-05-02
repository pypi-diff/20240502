# Comparing `tmp/pygrnd-0.1.6.tar.gz` & `tmp/pygrnd-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrnd-0.1.6.tar", last modified: Tue Jun 13 10:07:43 2023, max compression
+gzip compressed data, was "pygrnd-0.1.7.tar", last modified: Thu May  2 15:07:47 2024, max compression
```

## Comparing `pygrnd-0.1.6.tar` & `pygrnd-0.1.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:43.850313 pygrnd-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-13 10:07:33.000000 pygrnd-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14431 2023-06-13 10:07:43.850313 pygrnd-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-06-13 10:07:33.000000 pygrnd-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:43.842313 pygrnd-0.1.6/pygrnd/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:43.846313 pygrnd-0.1.6/pygrnd/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/MonteCarloSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    56649 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/UCPquboFunctionLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/bruteforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/meritorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/qaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)    27666 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/qmco.py
--rw-r--r--   0 runner    (1001) docker     (123)    39791 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/sat_ucp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:43.850313 pygrnd-0.1.6/pygrnd/qc/
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/QAE.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24444 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/brm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/brm_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/brm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/circuitConstructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/circuitConstructor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/lowDepthQAEgradientDescent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/parallelQAE.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/patternGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21171 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/patternReducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/probabilisticNetworks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/qml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:43.846313 pygrnd-0.1.6/pygrnd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14431 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 10:07:43.850313 pygrnd-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-13 10:07:33.000000 pygrnd-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:07:47.299236 pygrnd-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-02 15:07:43.000000 pygrnd-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14808 2024-05-02 15:07:47.299236 pygrnd-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-05-02 15:07:43.000000 pygrnd-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:07:47.295236 pygrnd-0.1.7/pygrnd/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:07:47.295236 pygrnd-0.1.7/pygrnd/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/optimize/MonteCarloSolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61157 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/optimize/UCPquboFunctionLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/optimize/bruteforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/optimize/meritorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15853 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/optimize/qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27449 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/optimize/qmco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39791 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/optimize/sat_ucp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:07:47.299236 pygrnd-0.1.7/pygrnd/qc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/QAE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/brm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/brm_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/brm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/circuitConstructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/circuitConstructor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/lowDepthQAEgradientDescent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18631 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/parallelQAE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/patternGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21171 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/patternReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/probabilisticNetworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-05-02 15:07:43.000000 pygrnd-0.1.7/pygrnd/qc/qml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:07:47.299236 pygrnd-0.1.7/pygrnd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14808 2024-05-02 15:07:47.000000 pygrnd-0.1.7/pygrnd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-02 15:07:47.000000 pygrnd-0.1.7/pygrnd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:07:47.000000 pygrnd-0.1.7/pygrnd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:07:47.000000 pygrnd-0.1.7/pygrnd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 15:07:47.000000 pygrnd-0.1.7/pygrnd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 15:07:47.000000 pygrnd-0.1.7/pygrnd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:07:47.299236 pygrnd-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-02 15:07:43.000000 pygrnd-0.1.7/setup.py
```

### Comparing `pygrnd-0.1.6/LICENSE` & `pygrnd-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/PKG-INFO` & `pygrnd-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: pygrnd
-Version: 0.1.6
-Summary: A python library for quantum algorithms and software
-Home-page: https://github.com/JoSQUANTUM/pygrnd
-Author: JoS QUANTUM
-Author-email: contact@jos-quantum.de
-License: Apache 2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![](https://github.com/JoSQUANTUM/pygrnd/actions/workflows/publish-to-pypi.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 
 # pygrnd 
 is a library of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
```

### Comparing `pygrnd-0.1.6/README.md` & `pygrnd-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: pygrnd
+Version: 0.1.7
+Summary: A python library for quantum algorithms and software
+Home-page: https://github.com/JoSQUANTUM/pygrnd
+Author: JoS QUANTUM
+Author-email: contact@jos-quantum.de
+License: Apache 2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: qiskit
+Requires-Dist: numpy
+Requires-Dist: dimod
+Requires-Dist: dwave-greedy
+Requires-Dist: dwave-neal
+Requires-Dist: pennylane
+Requires-Dist: pandas
+Requires-Dist: seaborn
+Requires-Dist: tqdm
+Requires-Dist: pylatexenc
+Requires-Dist: scikit-learn
+Requires-Dist: DateTime
+Requires-Dist: shap
+Requires-Dist: xgboost
+Requires-Dist: holidays
+Requires-Dist: imblearn
+
 ![](https://github.com/JoSQUANTUM/pygrnd/actions/workflows/publish-to-pypi.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 
 # pygrnd 
 is a library of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
```

### Comparing `pygrnd-0.1.6/pygrnd/__init__.py` & `pygrnd-0.1.7/pygrnd/__init__.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/optimize/MonteCarloSolver.py` & `pygrnd-0.1.7/pygrnd/optimize/MonteCarloSolver.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/optimize/UCPquboFunctionLibrary.py` & `pygrnd-0.1.7/pygrnd/optimize/UCPquboFunctionLibrary.py`

 * *Files 4% similar despite different names*

```diff
@@ -971,16 +971,57 @@
 
 def buildUCPqubo(autoset,n,pres,T,d,dgen,Clist,varcost,startcost,minup,mindown,mingen,maxgen):
 
     """
     Build the QUBO for the unit commitment problem as outlined in the following paper:
     M.C. Braun, T. Decker, N. Hegemann, S.F. Kerstan, F. Lorenz, "Towards optimization under uncertainty for fundamental models in energy markets using quantum computers", arXiv:2301.01108
     
-    Input:
-    List of power unit parameters, precision, time steps, demand, costs, min up/down min/max supply parameters
+    Parameters
+    ----------
+    autoset : bool
+        Whether the penalty factor should be set automatically or not.
+    n : int
+        Number of conventional power units (non-renewables).
+    pres : int
+        Resolution (number of bits) for discretizing the power supply range of units.
+    T : int
+        Number of time steps.
+    d : list of numbers
+        List of effective demands for every time step (= actual demands minus renewables).
+    dgen : list of lists of floats
+        Helper vector in the following format:
+        The i-th sublist is for the i-th conventional power unit.
+        The r-th element in the i-th sublist corresponds to `[(ppart * 2**r) * (maxgen[i]-mingen[i])`,
+        where `ppart` is `1 / ((2**(pres) - 1))`.
+    Clist : list of numpy vectors
+        (Not used) auxiliary variable for cost of unit i per timestep.
+        `Clist = [np.array(dgen[i])*varcost[i] for i in range(n)]`
+    varcost : list of numbers
+        List of costs for every conventional energy unit to produce 1 MWh.
+    startcost : list of numbers
+        List of costs for turning on every conventional energy unit.
+    minup : list of numbers
+        List of "minimal up-times" for every conventional energy unit
+        (whenever the i-th conventional energy unit is turned on,
+        it must remain "turned on" for at least `minup[i]` time steps).
+    mindown : list of numbers
+        List of "minimal down-times" for every conventional energy unit
+        (whenever the i-th conventional energy unit is turned off,
+        it must remain "turned off" for at least `minfown[i]` time steps).
+    mingen : list of numbers
+        List of minimal amount of power generation (in MWh) in each time step
+        for every conventional energy unit.
+    maxgen : list of numbers
+        List of maximal amount of power generation (in MWh) in each time step
+        for every conventional energy unit.
+    
+    Returns
+    ----------
+    Q : numpy matrix
+    Qcost : numpy matrix
     """
 
     print("Start building UCP QUBO")
 
     qubostart = time.process_time()
 
 
@@ -1109,14 +1150,59 @@
     Build the relaxed QUBO for the unit commitment problem including uncertainty as outlined in the following paper:
     M.C. Braun, T. Decker, N. Hegemann, S.F. Kerstan, F. Lorenz, "Towards optimization under uncertainty for fundamental models in energy markets using quantum computers", arXiv:2301.01108
     
     Input:
     List of power unit parameters, precision, time steps, demand, costs, min up/down min/max supply parameters, list of demand and supply including probabilities from renewables
     """
 
+    print("Preparation")
+
+    #initializing variables & setting variables with parameters / units
+    T=len(demand)                          # number of time steps
+    n = len(minup)                         # number of conventional power units
+    ppart = 1 / ((2**(pres) - 1))          # step size of logarithmic resolution
+
+    dgen0=[maxgen[i]-mingen[i] for i in range(len(mingen))]                     #power supply range of individual units
+    Clist = [dgen0[i]*varcost[i] for i in range(n)]                              #defining auxiliary variable for cost of unit i per timestep
+    dgen=[[ppart*dgen0[i]* 2**r for r in range(pres)] for i in range(n)]         #preparing power stage resolved "dgen"-vector
+
+    d=[]                                                                         #computing effective demans
+    for k in range(len(demand)):
+        if len(suppren)!=0:
+            if len(suppren)!=len(demand):
+                print('Mismatch of timesteps in demand and suppren')
+            d.append(demand[k] - np.sum(suppren[k]))
+        else:
+            d.append(demand[k])
+
+    #calculating expectation values
+    expD=[ sum(pdD[t][l]*probsD[t][l] for l in range(len(pdD[t]))) for t in range(T)]
+    if graphicsout==True:
+        print('expectation value of demand: ', expD)
+    expRE=[ sum(sum(pdRE[t][j][s]*probsRE[t][j][s] for s in range(len(pdRE[t][j]))) for j in range(len(pdRE[t]))) for t in range(T)]
+    if graphicsout==True:
+        print('expectation values of renewable supply: ', expRE)
+
+    from math import prod
+    comb=[list(itertools.product(*pdRE[i])) for i in range(len(pdRE))]
+    allcombinds_pdRE=[[[pdRE[l][list(np.array(m)).index(k)].index(k) for k in m] for m in comb[l]]for l in range(len(comb))]
+    allcombs_pdRE=[[[pdRE[l][m][allcombinds_pdRE[l][j][m]] for m in range(len(allcombinds_pdRE[l][j]))] for j in range(len(allcombinds_pdRE[l]))] for l in range(len(allcombinds_pdRE))]
+    expd=[sum(np.prod([probsRE[t][allcombinds_pdRE[t][m].index(allcombinds_pdRE[t][m][n])][allcombinds_pdRE[t][m][n]] for n in range(len(allcombs_pdRE[t][m]))])*probsD[t][r]*(pdD[t][r]-(sum(allcombs_pdRE[t][m][n] for n in range(len(allcombs_pdRE[t][m]))))) for m in range(len(allcombs_pdRE[t])) for r in range(len(pdD[t]))) for t in range(T)]
+    if graphicsout==True:
+        print('expected eff. demand: ', expd)
+
+    if A==0 and B==0 and C==0 and C2==0 and D==0 and E==0 and F==0 and G==0 and H==0:                                                                 # set penalty strengths before passing to buildQUBO
+        autoset=[1,0,0,0,0,0,0,0,0,0]
+    else:
+        autoset=[0,A,B,C,C2,D,E,F,G,H]
+
+
+
+
+
     print("Start building relaxed UCP QUBO")
 
     qubostart = time.process_time()
 
 
     #calculating auxiliary variables
     REres=len(pdRE[0][0])
```

### Comparing `pygrnd-0.1.6/pygrnd/optimize/bruteforce.py` & `pygrnd-0.1.7/pygrnd/optimize/bruteforce.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/optimize/meritorder.py` & `pygrnd-0.1.7/pygrnd/optimize/meritorder.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/optimize/qaoa.py` & `pygrnd-0.1.7/pygrnd/optimize/qaoa.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from qiskit import QuantumCircuit, ClassicalRegister, QuantumRegister
-from qiskit import execute
-from qiskit import Aer
-from qiskit import IBMQ
+from qiskit.providers.basic_provider import BasicProvider
+from qiskit import transpile
 from qiskit.visualization import plot_histogram
-from math import pi
-
 
+import itertools
 import math
+from math import pi
 import cmath
 import random
 import numpy as np
 
 from scipy.optimize import minimize
 
 import matplotlib.pyplot as plt
 from scipy.stats import norm
 
+
 def num2bin(x,r):
     res=""
     buffer=x
     for i in range(r):
         m=buffer%2
         res=res+str(m)
         buffer=(buffer-m)//2
@@ -62,25 +62,23 @@
 def maxString(counts):
     bits=len(list(counts.keys())[0])
     probList=counts2probs(counts)
     stringList=allCombinations(bits)
     maxi=np.argmax(probList)
     return stringList[maxi]
 
-
+# Return objective to x^t Q x value
 def eval_solution(x,m):
-
     obj=np.matmul(np.matmul(x,m),np.transpose(x))
-
     return obj
 
-import itertools
 
-def bruteForceSolver(m):
 
+# Brute force QUBO solver
+def bruteForceSolver(m):
     menge=[p for p in itertools.product([0,1], repeat=len(m))]
     #bestCost=-math.inf # maximize
     bestCost=math.inf # minimize
     bestVector=0
     for x in menge:
         v=np.zeros((1,len(m)))
         for i in range(len(m)):
@@ -88,17 +86,15 @@
         value=np.matmul(v,np.matmul(m,np.transpose(v)))
         if value<bestCost: #value>bestCost: <-- maximize
             bestCost=value
             bestVector=x
     return bestVector,bestCost
 
 
-
-
-
+# Convert matrix
 def matrixConvertInv(m):
     buffer=np.zeros((len(m),len(m)))
     for i in range(len(m)):
         for j in range(len(m)):
             if i==j:
                 buffer[i][i]=buffer[i][i]+m[i][i]/2
             else:
@@ -121,29 +117,36 @@
                 #qc.barrier()
     #qc.barrier()
     return qc
 
 
 ## Single layer QAOA
 
-def qaoaExp(m0,beta,gamma,Nshots,backend = Aer.get_backend('qasm_simulator')):
+def qaoaExp(m0,beta,gamma,Nshots,backend = BasicProvider().get_backend("basic_simulator")):
+    
     m=matrixConvertInv(m0)
     
     qr=QuantumRegister(len(m),'q')
     cr=ClassicalRegister(len(m),'c')
     qc=QuantumCircuit(qr,cr)
     for i in range(len(m)):
         qc.h(qr[i])
     addGates(qr,qc,m,gamma)
     for i in range(len(m)):
         qc.ry(beta,qr[i])
     qc.measure(qr,cr)
 
     #backend=Aer.get_backend("qasm_simulator")
-    job = execute(qc, backend,shots=Nshots)
+    #job = execute(qc, backend,shots=Nshots)
+    #counts=job.result().get_counts()
+
+    #backend = BasicProvider().get_backend("basic_simulator")
+    
+    qcNew=transpile(qc, backend)
+    job=backend.run(qcNew,shots=Nshots)
     counts=job.result().get_counts()
 
     # pull result with highest count
     maxValue=-math.inf
     for c in counts:
         if counts[c]>maxValue:
             maxValue=counts[c]
@@ -169,15 +172,15 @@
 #- use minimize with a function that has a single parameter (can be a vector)
 #- define appropriate function based on multyLayerqaoaExp
 #- use first half as $\beta$ parameters and second half as $\gamma$ parameters
 #- try one, two or six layers (2, 4 or 12 total parameters)
 
 # calculate expectation value through multi layer qaoa
 
-def multiLayerqaoaExp(m,betas,gammas,Nshots,backend = Aer.get_backend('qasm_simulator')):
+def multiLayerqaoaExp(m,betas,gammas,Nshots,backend = BasicProvider().get_backend("basic_simulator")):
     
     mPauli=matrixConvertInv(m)
     
     qr=QuantumRegister(len(mPauli),'q')
     cr=ClassicalRegister(len(mPauli),'c')
     qc=QuantumCircuit(qr,cr)
 
@@ -193,15 +196,19 @@
         for k in range(len(mPauli)):
             qc.ry(betas[j],qr[k])
             #qc.barrier()
         qc.barrier()
     qc.measure(qr,cr)
 
     #backend=Aer.get_backend("qasm_simulator")
-    job = execute(qc, backend,shots=Nshots)
+    #job = execute(qc, backend,shots=Nshots)
+    #counts=job.result().get_counts()
+
+    qcNew=transpile(qc, backend)
+    job=backend.run(qcNew,shots=Nshots)
     counts=job.result().get_counts()
 
     # pull result with highest count
     maxValue=-math.inf
     for c in counts:
         if counts[c]>maxValue:
             maxValue=counts[c]
@@ -220,15 +227,15 @@
 
     #return vec, sol, counts, obj, prob, qc
     return obj
 
 
 # calculate expectation value through multi layer qaoa
 
-def multiLayerqaoa(m,betas,gammas,Nshots,backend = Aer.get_backend('qasm_simulator')):
+def multiLayerqaoa(m,betas,gammas,Nshots,backend = BasicProvider().get_backend("basic_simulator")):
     
     mPauli=matrixConvertInv(m)
     
     qr=QuantumRegister(len(mPauli),'q')
     cr=ClassicalRegister(len(mPauli),'c')
     qc=QuantumCircuit(qr,cr)
 
@@ -244,15 +251,19 @@
         for k in range(len(mPauli)):
             qc.ry(betas[j],qr[k])
             #qc.barrier()
         qc.barrier()
     qc.measure(qr,cr)
 
     #backend=Aer.get_backend("qasm_simulator")
-    job = execute(qc, backend,shots=Nshots)
+    #job = execute(qc, backend,shots=Nshots)
+    #counts=job.result().get_counts()
+
+    qcNew=transpile(qc, backend)
+    job=backend.run(qcNew,shots=Nshots)
     counts=job.result().get_counts()
 
     # pull result with highest count
     maxValue=-math.inf
     for c in counts:
         if counts[c]>maxValue:
             maxValue=counts[c]
@@ -274,15 +285,15 @@
 
     
     
 ## functions using scipy minimize Nelder-Mead optimizer for multi layer QAOA
 ## Random init of beta, gamma
 ## returns circuit, parameters and found results
     
-def QAOAoptimizeMaxCount(m,layer,Nshots,backend = Aer.get_backend('qasm_simulator')):
+def QAOAoptimizeMaxCount(m,layer,Nshots,backend = BasicProvider().get_backend("basic_simulator")):
 
     def QAOAobjectiveFunction(x):
         size=len(x)
         size2=size//2
         return multiLayerqaoaExp(m,x[:size2],x[size2:],Nshots,backend)
 
     
@@ -354,15 +365,15 @@
     plt.colorbar()
 
 
 
 
 ## method by approximating the expectation value with the overall average of counts evaluated with the cost function
 
-def multiLayerqaoaExpectation(m,betas,gammas,Nshots,backend = Aer.get_backend('qasm_simulator')):
+def multiLayerqaoaExpectation(m,betas,gammas,Nshots,backend = BasicProvider().get_backend("basic_simulator")):
     
     mPauli=matrixConvertInv(m)
     
     qr=QuantumRegister(len(mPauli),'q')
     cr=ClassicalRegister(len(mPauli),'c')
     qc=QuantumCircuit(qr,cr)
 
@@ -378,15 +389,19 @@
         for k in range(len(mPauli)):
             qc.ry(betas[j],qr[k])
             #qc.barrier()
         qc.barrier()
     qc.measure(qr,cr)
 
     #backend=Aer.get_backend("qasm_simulator")
-    job = execute(qc, backend,shots=Nshots)
+    #job = execute(qc, backend,shots=Nshots)
+    #counts=job.result().get_counts()
+
+    qcNew=transpile(qc, backend)
+    job=backend.run(qcNew,shots=Nshots)
     counts=job.result().get_counts()
 
     avg = 0
     sum_count = 0
 
     for c in counts:
         #print(c,counts[c])
@@ -405,15 +420,15 @@
     #print(expectationValue)
     #print(avg/sum_count)
     return expectationValue
 
 
 # calculate expectation value through multi layer qaoa
 
-def multiLayerqaoaExpectation1(m,betas,gammas,Nshots,backend = Aer.get_backend('qasm_simulator')):
+def multiLayerqaoaExpectation1(m,betas,gammas,Nshots,backend = BasicProvider().get_backend("basic_simulator")):
     
     mPauli=matrixConvertInv(m)
     
     qr=QuantumRegister(len(mPauli),'q')
     cr=ClassicalRegister(len(mPauli),'c')
     qc=QuantumCircuit(qr,cr)
 
@@ -429,17 +444,20 @@
         for k in range(len(mPauli)):
             qc.ry(betas[j],qr[k])
             #qc.barrier()
         qc.barrier()
     qc.measure(qr,cr)
 
     #backend=Aer.get_backend("qasm_simulator")
-    job = execute(qc, backend,shots=Nshots)
-    counts=job.result().get_counts()
+    #job = execute(qc, backend,shots=Nshots)
+    #counts=job.result().get_counts()
 
+    qcNew=transpile(qc, backend)
+    job=backend.run(qcNew,shots=Nshots)
+    counts=job.result().get_counts()
     
     avg = 0
     sum_count = 0
 
     for c in counts:
         #print(c,counts[c])
         y=counts[c]
@@ -483,15 +501,15 @@
     
 ## functions using scipy minimize Nelder-Mead optimizer for multi layer QAOA
 ## Random init of beta, gamma
 ## returns circuit, parameters and found results
 ## optional backend: can be executed on simulator (default) or real harware
 ## optonal optimizer: "Nelder-Mead" (default), "COBYLA", "SLSQP"
     
-def QAOAoptimizeExpectation(m,layer,Nshots,backend = Aer.get_backend('qasm_simulator'),method="Nelder-Mead"):
+def QAOAoptimizeExpectation(m,layer,Nshots,backend = BasicProvider().get_backend("basic_simulator"),method="Nelder-Mead"):
 
     def QAOAobjectiveFunctionExpectation(x):
         size=len(x)
         size2=size//2
         return multiLayerqaoaExpectation(m,x[:size2],x[size2:],Nshots,backend)
```

### Comparing `pygrnd-0.1.6/pygrnd/optimize/qmco.py` & `pygrnd-0.1.7/pygrnd/optimize/qmco.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,22 +239,14 @@
         Difference from `annealingSamples`: a high number of annealingSamples
         only gives a higher
     DWtoken : None / str, optional
         If given a string: use it as the token for accessing D-Wave quantum hardware;
         If None: use D-Wave's simulated annealing algorithm.
     DWregion : str, optional
         Choose to use D-Wave's compute resources in a particular region. Default is "eu-central-1".
-    
-    
-    Returns
-    -------
-    mat_objs : list of numpy matrices
-        list of matrices coding the objective functions.
-    mat_cstrs : list of numpy matrices
-        list of matrices coding the constraints.
 
     Examples for `objs` and `cstrs`
     -------------------------------
     *Problem 1:*  we want 6 resolution bits for solving
         min  wᵀAw + bᵀw + c
                           w ∈ [0,1]ⁿ
     `qubo_resolution([('min',[A,b,c])], [], m=6)`
```

### Comparing `pygrnd-0.1.6/pygrnd/optimize/sat_ucp.py` & `pygrnd-0.1.7/pygrnd/optimize/sat_ucp.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py` & `pygrnd-0.1.7/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/qc/QAE.py` & `pygrnd-0.1.7/pygrnd/qc/QAE.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/qc/brm.py` & `pygrnd-0.1.7/pygrnd/qc/brm.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.'''
 
 import math
 import numpy as np
 import qiskit
-from qiskit import Aer, execute
 import random
 from qiskit import QuantumCircuit, QuantumRegister, ClassicalRegister
 from qiskit.circuit.library.standard_gates import U3Gate, XGate, ZGate
 from pygrnd.qc.helper import allCombinations, addValue, addPower2, subtractValue, subtractPower2,getMinusMarkerGate
 from pygrnd.qc.parallelQAE import getBitStringsForClosestBin
 from qiskit.extensions import UnitaryGate
 from qiskit.circuit.library import QFT
+from qiskit.providers.basic_provider import BasicProvider
+from qiskit import transpile
 
 def brm(nodes, edges, probsNodes, probsEdges, model2gate=False):
     """input:
          Risk item list e.g.  nodes = ['0','1']
          Correlation risk e.g. edges=[('0','1')] # correlations
          probsNodes={'0':0.1,'1':0.1} # intrinsic probs
          probsEdges={('0','1'):0.2} # transition probs
```

### Comparing `pygrnd-0.1.6/pygrnd/qc/brm_oracle.py` & `pygrnd-0.1.7/pygrnd/qc/brm_oracle.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 import math
 import numpy as np
 import qiskit
 import networkx as nx
 from qiskit import QuantumCircuit, QuantumRegister
 from qiskit.circuit.library.standard_gates import ZGate
-
+from qiskit.providers.basic_provider import BasicProvider
+from qiskit import transpile
 
 
 def brmoracle(name,PDFgenerator,pdfqubits,pdfancillas,LISTOFcontrolstrings):
 
    ##input:
    # PDFgenerator = underlying risk model
    # pdfqubits = QAE bit resolution
```

### Comparing `pygrnd-0.1.6/pygrnd/qc/brm_test.py` & `pygrnd-0.1.7/pygrnd/qc/brm_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.'''
 
 import random
 import pygrnd
-from qiskit import execute
-from qiskit import Aer
 from qiskit.quantum_info import hellinger_fidelity
 from pygrnd.qc.helper import *
 from pygrnd.qc.brm import *
 from pygrnd.qc.brm_oracle import *
 from pygrnd.qc.QAE import *
+from qiskit.providers.basic_provider import BasicProvider
+from qiskit import transpile
+
 
 def calculateDiffProbabilities(probsClassical, probsStatevector):
     '''Given are two dictionaries of probabilities. Calculate the difference
        of the probabilities.
     '''
     diffProbabilities=0
     for p in probsClassical:
```

### Comparing `pygrnd-0.1.6/pygrnd/qc/circuitConstructor.py` & `pygrnd-0.1.7/pygrnd/qc/circuitConstructor.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/qc/circuitConstructor_test.py` & `pygrnd-0.1.7/pygrnd/qc/circuitConstructor_test.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/qc/helper.py` & `pygrnd-0.1.7/pygrnd/qc/helper.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/qc/lowDepthQAEgradientDescent.py` & `pygrnd-0.1.7/pygrnd/qc/lowDepthQAEgradientDescent.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/qc/optimize.py` & `pygrnd-0.1.7/pygrnd/qc/optimize.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/qc/parallelQAE.py` & `pygrnd-0.1.7/pygrnd/qc/parallelQAE.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,22 @@
 # 
 # See "Error Resilient Quantum Amplitude Estimation from Parallel Quantum Phase Estimation"
 # https://arxiv.org/pdf/2204.01337.pdf
 
 import math, cmath, random
 import numpy as np
 from math import pi
-from qiskit import QuantumCircuit, ClassicalRegister, QuantumRegister, execute, Aer
+
+from qiskit import QuantumCircuit, ClassicalRegister, QuantumRegister, transpile
 from qiskit.circuit.library import QFT, HGate, XGate, UGate, SGate, ZGate, IGate
 from qiskit.circuit.random import random_circuit
+from qiskit.quantum_info import Statevector, Operator
+from qiskit.providers.basic_provider import BasicProvider
+
+
 import itertools
 from pygrnd.qc.helper import *
 #
 # Turn a number into binary string representation with b bits.
 #
 def num2bin(n, b):
     if b==0:
@@ -152,32 +157,39 @@
     numberQubits=model.num_qubits
 
     # Sum up the probabilities from the model operator.
     qr=QuantumRegister(numberQubits,'q')
     qc=QuantumCircuit(qr)
     qc.append(model,qr)
 
-    backend = Aer.get_backend('statevector_simulator')
-    job = execute(qc, backend)
-    v=np.asarray(job.result().get_statevector())
+    #backend = Aer.get_backend('statevector_simulator')
+    #job = execute(qc, backend)
+    #v=np.asarray(job.result().get_statevector())
+    v = Statevector(qc)
+    
+    
     sumProbs=0
     for i in range(len(v)):
         if num2bin(i,numberQubits) in targets:
             sumProbs=sumProbs+abs(v[i])**2
     # This is the resulting probability from the statevector simulation of the model.
     print("sum of probabilities of good states=",sumProbs)
 
     # Create the Grover operator and check the non-trivial eigenvalues.
     qr=QuantumRegister(numberQubits,'q')
     qc=QuantumCircuit(qr)
     qc.append(constructGroverOperator(model, targets),qr)
 
-    backend = Aer.get_backend('unitary_simulator')
-    job = execute(qc, backend)
-    u=job.result().get_unitary()
+    #backend = Aer.get_backend('unitary_simulator')
+    #job = execute(qc, backend)
+    #u=job.result().get_unitary()
+
+    #backend = UnitarySimulator(precision='single')
+    u = Operator(qc).data
+
     ev,ev2=np.linalg.eig(u)
     for x in ev:
         angle=np.angle(x)
         prob=math.sin(angle/2)**2
         if abs(prob-1)>0.01 and abs(prob-0)>0.01:
             print("probabilty from non-trivial eigenvalue of Grover operator:",prob)
 
@@ -226,32 +238,40 @@
 def getGoodEigenvaluesGroverOperator(modelGate, goodStates):
     numberQubits=modelGate.num_qubits
 
     qr=QuantumRegister(numberQubits,'q')
     qc=QuantumCircuit(qr)
     qc.append(constructGroverOperator(modelGate, goodStates),qr)
 
-    backend = Aer.get_backend('unitary_simulator')
-    job = execute(qc, backend)
-    u=job.result().get_unitary()
+    #backend = Aer.get_backend('unitary_simulator')
+    #job = execute(qc, backend)
+    #u=job.result().get_unitary()
+
+    u = Operator(qc).data
+
     return getGoodEigenvaluesUnitary(u)
 
 #
 # Add a qubit on top to get the eigenvector in the form can be compared
 # directly to the approximation. Note that the approximation circuit
 # has an extra qubit for creating the superposition.
 #
 def getEmbeddedVector(v):
     numberQubits=int(math.log(len(v))/math.log(2))
     qr=QuantumRegister(numberQubits+1,'q')
     qc=QuantumCircuit(qr)
     qc.initialize(v,qr[1:])
-    backend = Aer.get_backend('statevector_simulator')
-    job = execute(qc, backend)
-    return np.asarray(job.result().get_statevector())
+    
+    #backend = Aer.get_backend('statevector_simulator')
+    #job = execute(qc, backend)
+    v = Statevector(qc)
+
+    
+    
+    return v
 
 def getAllEmbeddedVectors(modelGate, goodStates):
     eigenvectors=getGoodEigenvaluesGroverOperator(modelGate,goodStates)
 
     embeddedEigenvectors=[]
     for v in eigenvectors:
         w=getEmbeddedVector(v)
@@ -504,19 +524,24 @@
         modelGate.label='m'
 
         qr=QuantumRegister(qubits,'q')
         cr=ClassicalRegister(qubits,'c')
         qc=QuantumCircuit(qr,cr)
         qc.append(modelGate,qr)
         qc.measure(qr,cr)
-        backend = Aer.get_backend('qasm_simulator')
+        
+        #backend = Aer.get_backend('qasm_simulator')
+        #job = execute(qc, backend, shots=numberShots)
+        #result=job.result()
+        #counts=result.get_counts()
+        backend = BasicProvider().get_backend("basic_simulator")
+        qcNew=transpile(qc, backend)
+        job=backend.run(qcNew,shots=numberShots)
+        counts=job.result().get_counts()
 
-        job = execute(qc, backend, shots=numberShots)
-        result=job.result()
-        counts=result.get_counts()
         
         # Check all subsets of size numberStates of possible combinations of results
         # if we land in the desired region. Each relevant state should have at least 1
         # hit to be relevant.
         binaryWords=allBits(qubits)
         
         for combi in itertools.combinations(binaryWords, numberStates):
```

### Comparing `pygrnd-0.1.6/pygrnd/qc/patternGenerator.py` & `pygrnd-0.1.7/pygrnd/qc/patternGenerator.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/qc/patternReducer.py` & `pygrnd-0.1.7/pygrnd/qc/patternReducer.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd/qc/probabilisticNetworks.py` & `pygrnd-0.1.7/pygrnd/qc/probabilisticNetworks.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,16 +267,17 @@
     return qc
 
 def evaluateQuantum(timesteps, nodes, probFail, probRecovery, edges):
     """ Evaluate a probabilistic network with a simulation of the corresponding quantum circuit.
     """
     qc,qr,cr=createCircuit(timesteps, nodes, probFail, probRecovery, edges)
     backend_qiskit = Aer.get_backend(name='statevector_simulator')
-    job = execute(qc, backend_qiskit)
-    v = np.asarray(job.result().get_statevector())
+    #job = execute(qc, backend_qiskit)
+    #v = np.asarray(job.result().get_statevector())
+    v = Statevector(qc)
 
     res={}
     for c in allCombinations(len(nodes)):
         res[c]=0
 
     for i in range(len(v)):
         binValue=num2bin(i,len(nodes)*timesteps)
```

### Comparing `pygrnd-0.1.6/pygrnd/qc/qml.py` & `pygrnd-0.1.7/pygrnd/qc/qml.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/pygrnd.egg-info/PKG-INFO` & `pygrnd-0.1.7/pygrnd.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 Metadata-Version: 2.1
 Name: pygrnd
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python library for quantum algorithms and software
 Home-page: https://github.com/JoSQUANTUM/pygrnd
 Author: JoS QUANTUM
 Author-email: contact@jos-quantum.de
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: qiskit
+Requires-Dist: numpy
+Requires-Dist: dimod
+Requires-Dist: dwave-greedy
+Requires-Dist: dwave-neal
+Requires-Dist: pennylane
+Requires-Dist: pandas
+Requires-Dist: seaborn
+Requires-Dist: tqdm
+Requires-Dist: pylatexenc
+Requires-Dist: scikit-learn
+Requires-Dist: DateTime
+Requires-Dist: shap
+Requires-Dist: xgboost
+Requires-Dist: holidays
+Requires-Dist: imblearn
 
 ![](https://github.com/JoSQUANTUM/pygrnd/actions/workflows/publish-to-pypi.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 
 # pygrnd 
 is a library of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
```

### Comparing `pygrnd-0.1.6/pygrnd.egg-info/SOURCES.txt` & `pygrnd-0.1.7/pygrnd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.6/setup.py` & `pygrnd-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,40 +15,41 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='pygrnd',
-    version='0.1.6',
+    version='0.1.7',
     description='A python library for quantum algorithms and software',
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='https://github.com/JoSQUANTUM/pygrnd',
     author='JoS QUANTUM',
     author_email='contact@jos-quantum.de',
     license='Apache 2.0',
     zip_safe=False,
     include_package_data=True,
     packages= find_packages(),
-    install_requires=['qiskit>=0.32.1',
+    install_requires=['qiskit',
                       'numpy',
                       'dimod',
                       'dwave-greedy',
                       'dwave-neal',
-                      'pennylane>=0.27.0',
+                      'pennylane',
                       'pandas',
                       'seaborn',
                       'tqdm',
                       'pylatexenc',
                       'scikit-learn',
                       'DateTime',
                       'shap',
                       'xgboost',
-                      'holidays'
+                      'holidays',
+                      'imblearn'
                       ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
     ],
 )
```

