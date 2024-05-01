# Comparing `tmp/mdpsolver-0.9.1.tar.gz` & `tmp/mdpsolver-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdpsolver-0.9.1.tar", last modified: Sun Apr 28 23:20:11 2024, max compression
+gzip compressed data, was "mdpsolver-0.9.2.tar", last modified: Wed May  1 23:25:11 2024, max compression
```

## Comparing `mdpsolver-0.9.1.tar` & `mdpsolver-0.9.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-04-28 23:20:11.651060 mdpsolver-0.9.1/
--rw-r--r--   0 anders    (1000) anders    (1000)     1127 2024-04-24 21:40:55.000000 mdpsolver-0.9.1/LICENSE
--rw-rw-r--   0 anders    (1000) anders    (1000)       37 2024-04-28 23:19:52.000000 mdpsolver-0.9.1/MANIFEST.in
--rw-r--r--   0 anders    (1000) anders    (1000)     4197 2024-04-28 23:20:11.651060 mdpsolver-0.9.1/PKG-INFO
--rw-rw-r--   0 anders    (1000) anders    (1000)     3584 2024-04-25 22:46:57.000000 mdpsolver-0.9.1/README.md
--rw-rw-r--   0 anders    (1000) anders    (1000)      795 2024-04-28 23:20:03.000000 mdpsolver-0.9.1/pyproject.toml
--rw-rw-r--   0 anders    (1000) anders    (1000)       38 2024-04-28 23:20:11.651060 mdpsolver-0.9.1/setup.cfg
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-04-28 23:20:11.647060 mdpsolver-0.9.1/src/
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-04-28 23:20:11.651060 mdpsolver-0.9.1/src/mdpsolver/
--rw-rw-r--   0 anders    (1000) anders    (1000)       33 2024-04-24 21:40:19.000000 mdpsolver-0.9.1/src/mdpsolver/__init__.py
--rw-rw-r--   0 anders    (1000) anders    (1000)     4524 2024-04-27 19:29:45.000000 mdpsolver-0.9.1/src/mdpsolver/model.py
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-04-28 23:20:11.651060 mdpsolver-0.9.1/src/mdpsolver/problems/
--rw-rw-r--   0 anders    (1000) anders    (1000)     1371 2024-04-24 21:22:58.000000 mdpsolver-0.9.1/src/mdpsolver/problems/cbmaux.py
--rw-rw-r--   0 anders    (1000) anders    (1000)     1366 2024-04-24 21:22:58.000000 mdpsolver-0.9.1/src/mdpsolver/problems/tbmaux.py
--rw-r--r--   0 anders    (1000) anders    (1000)   242688 2024-04-28 22:35:40.000000 mdpsolver-0.9.1/src/mdpsolver/solvermodule.cp310-win_amd64.pyd
--rwxrwxr-x   0 anders    (1000) anders    (1000)   432424 2024-04-28 21:55:45.000000 mdpsolver-0.9.1/src/mdpsolver/solvermodule.cpython-310-x86_64-linux-gnu.so
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-04-28 23:20:11.651060 mdpsolver-0.9.1/src/mdpsolver.egg-info/
--rw-r--r--   0 anders    (1000) anders    (1000)     4197 2024-04-28 23:20:11.000000 mdpsolver-0.9.1/src/mdpsolver.egg-info/PKG-INFO
--rw-rw-r--   0 anders    (1000) anders    (1000)      413 2024-04-28 23:20:11.000000 mdpsolver-0.9.1/src/mdpsolver.egg-info/SOURCES.txt
--rw-rw-r--   0 anders    (1000) anders    (1000)        1 2024-04-28 23:20:11.000000 mdpsolver-0.9.1/src/mdpsolver.egg-info/dependency_links.txt
--rw-rw-r--   0 anders    (1000) anders    (1000)       10 2024-04-28 23:20:11.000000 mdpsolver-0.9.1/src/mdpsolver.egg-info/top_level.txt
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-01 23:25:11.074892 mdpsolver-0.9.2/
+-rw-rw-r--   0 anders    (1000) anders    (1000)     1106 2024-04-28 23:39:54.000000 mdpsolver-0.9.2/LICENSE
+-rw-rw-r--   0 anders    (1000) anders    (1000)       37 2024-04-28 23:19:52.000000 mdpsolver-0.9.2/MANIFEST.in
+-rw-r--r--   0 anders    (1000) anders    (1000)     4164 2024-05-01 23:25:11.074892 mdpsolver-0.9.2/PKG-INFO
+-rw-r--r--   0 anders    (1000) anders    (1000)     3681 2024-05-01 12:42:21.000000 mdpsolver-0.9.2/README.md
+-rw-rw-r--   0 anders    (1000) anders    (1000)      795 2024-05-01 23:21:11.000000 mdpsolver-0.9.2/pyproject.toml
+-rw-rw-r--   0 anders    (1000) anders    (1000)       38 2024-05-01 23:25:11.074892 mdpsolver-0.9.2/setup.cfg
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-01 23:25:11.070891 mdpsolver-0.9.2/src/
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-01 23:25:11.074892 mdpsolver-0.9.2/src/mdpsolver/
+-rw-rw-r--   0 anders    (1000) anders    (1000)       33 2024-04-28 23:39:54.000000 mdpsolver-0.9.2/src/mdpsolver/__init__.py
+-rw-rw-r--   0 anders    (1000) anders    (1000)     4532 2024-05-01 22:22:15.000000 mdpsolver-0.9.2/src/mdpsolver/model.py
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-01 23:25:11.074892 mdpsolver-0.9.2/src/mdpsolver/problems/
+-rw-rw-r--   0 anders    (1000) anders    (1000)     1371 2024-04-28 23:39:54.000000 mdpsolver-0.9.2/src/mdpsolver/problems/cbmaux.py
+-rw-rw-r--   0 anders    (1000) anders    (1000)     1366 2024-04-28 23:39:54.000000 mdpsolver-0.9.2/src/mdpsolver/problems/tbmaux.py
+-rw-rw-r--   0 anders    (1000) anders    (1000)   242688 2024-04-28 23:39:54.000000 mdpsolver-0.9.2/src/mdpsolver/solvermodule.cp310-win_amd64.pyd
+-rw-r--r--   0 anders    (1000) anders    (1000)   244736 2024-05-01 23:14:53.000000 mdpsolver-0.9.2/src/mdpsolver/solvermodule.cp311-win_amd64.pyd
+-rw-r--r--   0 anders    (1000) anders    (1000)   247296 2024-05-01 19:38:54.000000 mdpsolver-0.9.2/src/mdpsolver/solvermodule.cp312-win_amd64.pyd
+-rwxrwxr-x   0 anders    (1000) anders    (1000)   432424 2024-05-01 21:34:50.000000 mdpsolver-0.9.2/src/mdpsolver/solvermodule.cpython-310-x86_64-linux-gnu.so
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-01 23:25:11.074892 mdpsolver-0.9.2/src/mdpsolver.egg-info/
+-rw-r--r--   0 anders    (1000) anders    (1000)     4164 2024-05-01 23:25:11.000000 mdpsolver-0.9.2/src/mdpsolver.egg-info/PKG-INFO
+-rw-rw-r--   0 anders    (1000) anders    (1000)      507 2024-05-01 23:25:11.000000 mdpsolver-0.9.2/src/mdpsolver.egg-info/SOURCES.txt
+-rw-rw-r--   0 anders    (1000) anders    (1000)        1 2024-05-01 23:25:11.000000 mdpsolver-0.9.2/src/mdpsolver.egg-info/dependency_links.txt
+-rw-rw-r--   0 anders    (1000) anders    (1000)       10 2024-05-01 23:25:11.000000 mdpsolver-0.9.2/src/mdpsolver.egg-info/top_level.txt
```

### Comparing `mdpsolver-0.9.1/LICENSE` & `mdpsolver-0.9.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Anders Reenberg Andersen and Jesper Fink Andersen
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Anders Reenberg Andersen and Jesper Fink Andersen
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mdpsolver-0.9.1/PKG-INFO` & `mdpsolver-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdpsolver
-Version: 0.9.1
+Version: 0.9.2
 Summary: An efficient solver for Markov Decision Processes
 Author-email: Anders Reenberg Andersen <andersra@live.dk>, Jesper Fink Andersen <jfan@dtu.dk>
 Project-URL: Homepage, https://github.com/areenberg/MDPSolver
 Project-URL: Issues, https://github.com/areenberg/MDPSolver/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 `mdpsolver` is the Python package for deriving the policies of Markov Decision Processes (MDPs) with infinite-horizon and the expected total discounted reward optimality criterion. 
 
 ## Features
 
 * Available on PyPI.
 * Solver-engine developed in C++.
 * Available optimization algorithms: *Value iteration*, *Policy iteration*, and *Modified policy iteration*.  
-* Includes a variety of input formats available for users to choose from.
+* Includes support for sparse matrices.
 
 # Quick start guide
 
 The following shows how to get quickly started with `mdpsolver`.
 
 ## Installation
 
@@ -78,15 +78,15 @@
 The optimized policy can be returned in a variety of ways. Here, we return the policy as a list and print directly in the terminal. 
 
 ```python
 print(mdl.getPolicy())
 #[1, 1, 0]
 ```
 
-## Large transition matrix?
+## Sparse transition matrix?
 
 `mdpsolver` has three alternative formats for large and highly sparse transition probability matrices.
 
 **(1) Elementwise representation (excluding elements containing zeros):**
 
 ```python
 #[from_state,action,to_state,probability]
```

### Comparing `mdpsolver-0.9.1/README.md` & `mdpsolver-0.9.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-# `mdpsolver`: An efficient solver for Markov Decision Processes
- 
-`mdpsolver` is the Python package for deriving the policies of Markov Decision Processes (MDPs) with infinite-horizon and the expected total discounted reward optimality criterion. 
-
-## Features
-
-* Available on PyPI.
-* Solver-engine developed in C++.
-* Available optimization algorithms: *Value iteration*, *Policy iteration*, and *Modified policy iteration*.  
-* Includes a variety of input formats available for users to choose from.
-
-# Quick start guide
-
-The following shows how to get quickly started with `mdpsolver`.
-
-## Installation
-
-Download and install `mdpsolver` directly from PyPI. 
-
-```
-pip install mdpsolver
-```
-
-## Usage
-
-Start by specifying the reward function and transition probabilities as lists. The following is an example of a simple MDP containing **three states** and **two actions in each state**.
-
-```python
-#Import packages
-import mdpsolver
-
-#Rewards (3 states x 2 actions)
-#e.g. choosing second action in first state gives reward=-1
-rewards = [[5,-1],
-           [1,-2],
-           [50,0]]
-
-#Transition probabilities (3 from_states x 2 actions x 3 to_states)
-#e.g. choosing first action in third state gives a probability of 0.6 of staying in third state
-tranMatWithZeros = [[[0.9,0.1,0.0],[0.1,0.9,0.0]],
-                    [[0.4,0.5,0.1],[0.3,0.5,0.2]],
-                    [[0.2,0.2,0.6],[0.5,0.5,0.0]]]
-```
-
-Now, create the model object and insert the problem parameters.
-
-```python
-#Create model object
-mdl = mdpsolver.model()
-
-#Insert the problem parameters
-mdl.mdp(discount=0.8,
-        rewards=rewards,
-        tranMatWithZeros=tranMatWithZeros)
-```
-
-We can now optimize the policy.
-
-```python
-mdl.solve()
-```
-
-The optimized policy can be returned in a variety of ways. Here, we return the policy as a list and print directly in the terminal. 
-
-```python
-print(mdl.getPolicy())
-#[1, 1, 0]
-```
-
-## Large transition matrix?
-
-`mdpsolver` has three alternative formats for large and highly sparse transition probability matrices.
-
-**(1) Elementwise representation (excluding elements containing zeros):**
-
-```python
-#[from_state,action,to_state,probability]
-tranMatElementwise = [[0,0,0,0.9],
-                      [0,0,1,0.1],
-                      [0,1,0,0.1],
-                      [0,1,1,0.9],
-                      [1,0,0,0.4],
-                      [1,0,1,0.5],
-                      [1,0,2,0.1],
-                      [1,1,0,0.3],
-                      [1,1,1,0.5],
-                      [1,1,2,0.2],
-                      [2,0,0,0.2],
-                      [2,0,1,0.2],
-                      [2,0,2,0.6],
-                      [2,1,0,0.5],
-                      [2,1,1,0.5]]
-
-mdl.mdp(discount=0.8,
-        rewards=rewards,
-        tranMatElementwise=tranMatElementwise)
-```
-
-**(2) Probabilities and column (to_state) indices in separate lists:**
-
-```python
-tranMatProbs = [[[0.9,0.1],[0.1,0.9]],
-                [[0.4,0.5,0.1],[0.3,0.5,0.2]],
-                [[0.2,0.2,0.6],[0.5,0.5]]]
-
-tranMatColumns = [[[0,1],[0,1]],
-                [[0,1,2],[0,1,2]],
-                [[0,1,2],[0,1]]]
-
-mdl.mdp(discount=0.8,
-        rewards=rewards,
-        tranMatProbs=tranMatProbs,
-        tranMatColumns=tranMatColumns)
-
-```
-
-**(3) Load the elementwise representation from a file:**
-
-```python
-mdl.mdp(discount=0.8,
-        rewards=rewards,
-        tranMatFromFile="transitions.csv")
-```
-
-# User manual
-
-Further information can be found in the wiki for `mdpsolver` on Github.
-
-# How to cite
-
+# `mdpsolver`: An efficient solver for Markov Decision Processes
+ 
+`mdpsolver` is the Python package for deriving the policies of Markov Decision Processes (MDPs) with infinite-horizon and the expected total discounted reward optimality criterion. 
+
+## Features
+
+* Available on PyPI.
+* Solver-engine developed in C++.
+* Available optimization algorithms: *Value iteration*, *Policy iteration*, and *Modified policy iteration*.  
+* Includes support for sparse matrices.
+
+# Quick start guide
+
+The following shows how to get quickly started with `mdpsolver`.
+
+## Installation
+
+Download and install `mdpsolver` directly from PyPI. 
+
+```
+pip install mdpsolver
+```
+
+## Usage
+
+Start by specifying the reward function and transition probabilities as lists. The following is an example of a simple MDP containing **three states** and **two actions in each state**.
+
+```python
+#Import packages
+import mdpsolver
+
+#Rewards (3 states x 2 actions)
+#e.g. choosing second action in first state gives reward=-1
+rewards = [[5,-1],
+           [1,-2],
+           [50,0]]
+
+#Transition probabilities (3 from_states x 2 actions x 3 to_states)
+#e.g. choosing first action in third state gives a probability of 0.6 of staying in third state
+tranMatWithZeros = [[[0.9,0.1,0.0],[0.1,0.9,0.0]],
+                    [[0.4,0.5,0.1],[0.3,0.5,0.2]],
+                    [[0.2,0.2,0.6],[0.5,0.5,0.0]]]
+```
+
+Now, create the model object and insert the problem parameters.
+
+```python
+#Create model object
+mdl = mdpsolver.model()
+
+#Insert the problem parameters
+mdl.mdp(discount=0.8,
+        rewards=rewards,
+        tranMatWithZeros=tranMatWithZeros)
+```
+
+We can now optimize the policy.
+
+```python
+mdl.solve()
+```
+
+The optimized policy can be returned in a variety of ways. Here, we return the policy as a list and print directly in the terminal. 
+
+```python
+print(mdl.getPolicy())
+#[1, 1, 0]
+```
+
+## Sparse transition matrix?
+
+`mdpsolver` has three alternative formats for large and highly sparse transition probability matrices.
+
+**(1) Elementwise representation (excluding elements containing zeros):**
+
+```python
+#[from_state,action,to_state,probability]
+tranMatElementwise = [[0,0,0,0.9],
+                      [0,0,1,0.1],
+                      [0,1,0,0.1],
+                      [0,1,1,0.9],
+                      [1,0,0,0.4],
+                      [1,0,1,0.5],
+                      [1,0,2,0.1],
+                      [1,1,0,0.3],
+                      [1,1,1,0.5],
+                      [1,1,2,0.2],
+                      [2,0,0,0.2],
+                      [2,0,1,0.2],
+                      [2,0,2,0.6],
+                      [2,1,0,0.5],
+                      [2,1,1,0.5]]
+
+mdl.mdp(discount=0.8,
+        rewards=rewards,
+        tranMatElementwise=tranMatElementwise)
+```
+
+**(2) Probabilities and column (to_state) indices in separate lists:**
+
+```python
+tranMatProbs = [[[0.9,0.1],[0.1,0.9]],
+                [[0.4,0.5,0.1],[0.3,0.5,0.2]],
+                [[0.2,0.2,0.6],[0.5,0.5]]]
+
+tranMatColumns = [[[0,1],[0,1]],
+                [[0,1,2],[0,1,2]],
+                [[0,1,2],[0,1]]]
+
+mdl.mdp(discount=0.8,
+        rewards=rewards,
+        tranMatProbs=tranMatProbs,
+        tranMatColumns=tranMatColumns)
+
+```
+
+**(3) Load the elementwise representation from a file:**
+
+```python
+mdl.mdp(discount=0.8,
+        rewards=rewards,
+        tranMatFromFile="transitions.csv")
+```
+
+# User manual
+
+Further information can be found in the wiki for `mdpsolver` on Github.
+
+# How to cite
+
 [![DOI](https://zenodo.org/badge/294063917.svg)](https://zenodo.org/badge/latestdoi/294063917)
```

### Comparing `mdpsolver-0.9.1/pyproject.toml` & `mdpsolver-0.9.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "mdpsolver"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="Anders Reenberg Andersen", email="andersra@live.dk" },
   { name="Jesper Fink Andersen", email="jfan@dtu.dk" },
 ]
 description = "An efficient solver for Markov Decision Processes"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mdpsolver-0.9.1/src/mdpsolver/model.py` & `mdpsolver-0.9.2/src/mdpsolver/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from mdpsolver.problems.cbmaux import cbmaux
 
 class model:
     
     def __init__(self):
         self.initialize()            
         
-    def initialize(self):
+    def initialize(self):        
         #create the solver object
         self.mdl = solvermodule.Model()
     
     def solve(self,
               algorithm="mpi",
               tolerance=1e-3,
               update="standard",
```

### Comparing `mdpsolver-0.9.1/src/mdpsolver/problems/cbmaux.py` & `mdpsolver-0.9.2/src/mdpsolver/problems/cbmaux.py`

 * *Files identical despite different names*

### Comparing `mdpsolver-0.9.1/src/mdpsolver/problems/tbmaux.py` & `mdpsolver-0.9.2/src/mdpsolver/problems/tbmaux.py`

 * *Files identical despite different names*

### Comparing `mdpsolver-0.9.1/src/mdpsolver/solvermodule.cpython-310-x86_64-linux-gnu.so` & `mdpsolver-0.9.2/src/mdpsolver/solvermodule.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `mdpsolver-0.9.1/src/mdpsolver.egg-info/PKG-INFO` & `mdpsolver-0.9.2/src/mdpsolver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdpsolver
-Version: 0.9.1
+Version: 0.9.2
 Summary: An efficient solver for Markov Decision Processes
 Author-email: Anders Reenberg Andersen <andersra@live.dk>, Jesper Fink Andersen <jfan@dtu.dk>
 Project-URL: Homepage, https://github.com/areenberg/MDPSolver
 Project-URL: Issues, https://github.com/areenberg/MDPSolver/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 `mdpsolver` is the Python package for deriving the policies of Markov Decision Processes (MDPs) with infinite-horizon and the expected total discounted reward optimality criterion. 
 
 ## Features
 
 * Available on PyPI.
 * Solver-engine developed in C++.
 * Available optimization algorithms: *Value iteration*, *Policy iteration*, and *Modified policy iteration*.  
-* Includes a variety of input formats available for users to choose from.
+* Includes support for sparse matrices.
 
 # Quick start guide
 
 The following shows how to get quickly started with `mdpsolver`.
 
 ## Installation
 
@@ -78,15 +78,15 @@
 The optimized policy can be returned in a variety of ways. Here, we return the policy as a list and print directly in the terminal. 
 
 ```python
 print(mdl.getPolicy())
 #[1, 1, 0]
 ```
 
-## Large transition matrix?
+## Sparse transition matrix?
 
 `mdpsolver` has three alternative formats for large and highly sparse transition probability matrices.
 
 **(1) Elementwise representation (excluding elements containing zeros):**
 
 ```python
 #[from_state,action,to_state,probability]
```

