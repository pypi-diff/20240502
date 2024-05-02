# Comparing `tmp/softpy-0.0.2.tar.gz` & `tmp/softpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "softpy-0.0.2.tar", last modified: Mon Mar 11 09:07:43 2024, max compression
+gzip compressed data, was "softpy-0.0.3.tar", last modified: Thu May  2 10:43:02 2024, max compression
```

## Comparing `softpy-0.0.2.tar` & `softpy-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-03-11 09:07:43.073115 softpy-0.0.2/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      280 2023-03-06 10:54:52.000000 softpy-0.0.2/LICENSE
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-03-11 09:07:43.073115 softpy-0.0.2/PKG-INFO
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      715 2024-03-08 13:07:13.000000 softpy-0.0.2/README.md
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      162 2024-03-11 09:07:43.078115 softpy-0.0.2/setup.cfg
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      571 2024-03-11 09:07:33.000000 softpy-0.0.2/setup.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-03-11 09:07:42.656508 softpy-0.0.2/softpy/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)       49 2023-05-12 17:24:06.000000 softpy-0.0.2/softpy/__init__.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-03-11 09:07:42.911121 softpy-0.0.2/softpy/evolutionary/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      637 2023-06-14 11:31:54.000000 softpy-0.0.2/softpy/evolutionary/__init__.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)    12572 2023-06-21 10:17:14.000000 softpy-0.0.2/softpy/evolutionary/candidate.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     7558 2024-03-08 14:08:59.000000 softpy-0.0.2/softpy/evolutionary/genetic.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1285 2023-06-21 10:13:20.000000 softpy-0.0.2/softpy/evolutionary/selection.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3238 2023-06-21 10:16:53.000000 softpy-0.0.2/softpy/evolutionary/singlestate.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-03-11 09:07:43.046546 softpy-0.0.2/softpy/fuzzy/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1336 2024-03-08 14:09:52.000000 softpy-0.0.2/softpy/fuzzy/__init__.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3254 2024-03-08 14:08:45.000000 softpy-0.0.2/softpy/fuzzy/clustering.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     9634 2024-03-08 14:08:37.000000 softpy-0.0.2/softpy/fuzzy/control.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)    18190 2024-03-11 09:05:48.000000 softpy-0.0.2/softpy/fuzzy/fuzzyset.py
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)    14578 2024-03-08 14:08:32.000000 softpy-0.0.2/softpy/fuzzy/operations.py
-drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-03-11 09:07:42.791022 softpy-0.0.2/softpy.egg-info/
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-03-11 09:07:42.000000 softpy-0.0.2/softpy.egg-info/PKG-INFO
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)      496 2024-03-11 09:07:42.000000 softpy-0.0.2/softpy.egg-info/SOURCES.txt
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)        1 2024-03-11 09:07:42.000000 softpy-0.0.2/softpy.egg-info/dependency_links.txt
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)       28 2024-03-11 09:07:42.000000 softpy-0.0.2/softpy.egg-info/requires.txt
--rwxrwxrwx   0 andrea    (1000) andrea    (1000)        7 2024-03-11 09:07:42.000000 softpy-0.0.2/softpy.egg-info/top_level.txt
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:43:02.355692 softpy-0.0.3/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      280 2023-03-06 10:54:52.000000 softpy-0.0.3/LICENSE
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-05-02 10:43:02.356693 softpy-0.0.3/PKG-INFO
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      715 2024-03-08 13:07:13.000000 softpy-0.0.3/README.md
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      162 2024-05-02 10:43:02.362820 softpy-0.0.3/setup.cfg
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      571 2024-05-02 10:41:23.000000 softpy-0.0.3/setup.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:43:01.936905 softpy-0.0.3/softpy/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)       49 2023-05-12 17:24:06.000000 softpy-0.0.3/softpy/__init__.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:43:02.160914 softpy-0.0.3/softpy/evolutionary/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      708 2024-05-02 10:40:30.000000 softpy-0.0.3/softpy/evolutionary/__init__.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)    12572 2023-06-21 10:17:14.000000 softpy-0.0.3/softpy/evolutionary/candidate.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     7558 2024-03-08 14:08:59.000000 softpy-0.0.3/softpy/evolutionary/genetic.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1285 2023-06-21 10:13:20.000000 softpy-0.0.3/softpy/evolutionary/selection.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3238 2023-06-21 10:16:53.000000 softpy-0.0.3/softpy/evolutionary/singlestate.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:43:02.336680 softpy-0.0.3/softpy/fuzzy/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1336 2024-03-08 14:09:52.000000 softpy-0.0.3/softpy/fuzzy/__init__.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     3254 2024-03-08 14:08:45.000000 softpy-0.0.3/softpy/fuzzy/clustering.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     9634 2024-03-08 14:08:37.000000 softpy-0.0.3/softpy/fuzzy/control.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)    20235 2024-03-22 11:48:08.000000 softpy-0.0.3/softpy/fuzzy/fuzzyset.py
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)    14578 2024-03-22 11:52:40.000000 softpy-0.0.3/softpy/fuzzy/operations.py
+drwxrwxrwx   0 andrea    (1000) andrea    (1000)        0 2024-05-02 10:43:02.036371 softpy-0.0.3/softpy.egg-info/
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)     1019 2024-05-02 10:43:01.000000 softpy-0.0.3/softpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)      496 2024-05-02 10:43:01.000000 softpy-0.0.3/softpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)        1 2024-05-02 10:43:01.000000 softpy-0.0.3/softpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)       28 2024-05-02 10:43:01.000000 softpy-0.0.3/softpy.egg-info/requires.txt
+-rwxrwxrwx   0 andrea    (1000) andrea    (1000)        7 2024-05-02 10:43:01.000000 softpy-0.0.3/softpy.egg-info/top_level.txt
```

### Comparing `softpy-0.0.2/PKG-INFO` & `softpy-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for soft computing in Python.
 Home-page: https://pypi.org/project/scikit-weak/
 Author: Andrea Campagner
 Author-email: onyris93@gmail.com
 License: LICENSE.txt
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `softpy-0.0.2/README.md` & `softpy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `softpy-0.0.2/setup.py` & `softpy-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
    name='softpy',
-   version='0.0.2',
+   version='0.0.3',
    author='Andrea Campagner',
    python_requires=">3.8.0",
    author_email='onyris93@gmail.com',
    packages=find_packages(include=['softpy', 'softpy.*']),
    url='https://pypi.org/project/scikit-weak/',
    license='LICENSE.txt',
    description='A package for soft computing in Python.',
```

### Comparing `softpy-0.0.2/softpy/evolutionary/__init__.py` & `softpy-0.0.3/softpy/evolutionary/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from .genetic import GeneticAlgorithm, SteadyStateGeneticAlgorithm
 from .singlestate import HillClimbing, RandomSearch
-from .selection import tournament_selection, fitness_prop_selection
+from .selection import tournament_selection, fitness_prop_selection, stochastic_universal_selection
 from .candidate import Candidate, BitVectorCandidate, FloatVectorCandidate, PathCandidate, TreeCandidate, DictionaryCandidate
 
 all = [
     "GeneticAlgorithm",
     "SteadyStateGeneticAlgorithm",
     "HillClimbing",
     "RandomSearch",
     "tournament_selection",
     "fitness_prop_selection",
+    "stochastic_universal_selection",
     "Candidate",
     "BitVectorCandidate",
     "FloatVectorCandidate",
     "PathCandidate",
     "TreeCandidate",
     "DictionaryCandidate"
 ]
```

### Comparing `softpy-0.0.2/softpy/evolutionary/candidate.py` & `softpy-0.0.3/softpy/evolutionary/candidate.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.2/softpy/evolutionary/genetic.py` & `softpy-0.0.3/softpy/evolutionary/genetic.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.2/softpy/evolutionary/selection.py` & `softpy-0.0.3/softpy/evolutionary/selection.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.2/softpy/evolutionary/singlestate.py` & `softpy-0.0.3/softpy/evolutionary/singlestate.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.2/softpy/fuzzy/__init__.py` & `softpy-0.0.3/softpy/fuzzy/__init__.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.2/softpy/fuzzy/clustering.py` & `softpy-0.0.3/softpy/fuzzy/clustering.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.2/softpy/fuzzy/control.py` & `softpy-0.0.3/softpy/fuzzy/control.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.2/softpy/fuzzy/fuzzyset.py` & `softpy-0.0.3/softpy/fuzzy/fuzzyset.py`

 * *Files 3% similar despite different names*

```diff
@@ -465,8 +465,62 @@
         except AttributeError:
             left = lambda x: (x - self.lower)/(self.middle1 - self.lower)
             right = lambda x: (self.upper - x)/(self.upper - self.middle2)
             left_int = lambda x: left(x)*np.log(1/left(x)) + (1 - left(x))*np.log2(1/(1-left(x)))
             right_int = lambda x: right(x)*np.log(1/right(x)) + (1 - right(x))*np.log2(1/(1-right(x)))
             self.f : np.number = sp.integrate.quad(left_int, self.lower, self.middle1)[0]
             self.f += sp.integrate.quad(right_int, self.middle2, self.upper)[0]
+            return self.f
+        
+
+
+
+class GaussianFuzzyNumber(FuzzyNumber):
+    '''
+    Implements a Gaussian fuzzy number
+    '''
+    def __init__(self, mean: np.number, std: np.number):
+        if not np.issubdtype(type(mean), np.number):
+            raise TypeError("Mean should be float, is %s" % type(mean))
+        
+        if not np.issubdtype(type(std), np.number):
+            raise TypeError("Middle should be floats, is %s" % type(std))
+        
+        if std < 0:
+            raise ValueError("std should be positive")
+        
+        self.mean = mean
+        self.std = std
+
+        self.min = self.mean - np.sqrt(2*self.std**2 * np.log(1/0.001))
+        self.max = self.mean + np.sqrt(2*self.std**2 * np.log(1/0.001))
+
+    def __call__(self, arg: np.number) -> np.number:
+        if not np.issubdtype(type(arg), np.number):
+            raise TypeError("Arg should be float, is %s" % type(arg))
+        
+        return np.exp(-(arg - self.mean)**2/(2*self.std**2))
+        
+    def __getitem__(self, alpha: np.number) -> tuple[np.number, np.number]:
+        if not np.issubdtype(type(alpha), np.number):
+            raise TypeError("Alpha should be a float in [0,1], is %s" % type(alpha))
+        
+        if alpha < 0 or alpha > 1:
+            raise ValueError("Alpha should be in [0,1], is %s" % alpha)
+        
+        low = self.mean - np.sqrt(2*self.std**2 * np.log(1/alpha))
+        upp = self.mean + np.sqrt(2*self.std**2 * np.log(1/alpha))
+        
+        return low, upp
+    
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, GaussianFuzzyNumber):
+            return NotImplemented
+        return self.mean == other.mean and self.std == other.std
+    
+    def fuzziness(self) -> np.number:
+        try:
+            return self.f
+        except AttributeError:
+            intgr = lambda x: self(x)*np.log(1/self(x)) + (1 - self(x))*np.log2(1/(1-self(x)))
+            self.f : np.number = sp.integrate.quad(intgr, self.min, self.max)[0]
             return self.f
```

### Comparing `softpy-0.0.2/softpy/fuzzy/operations.py` & `softpy-0.0.3/softpy/fuzzy/operations.py`

 * *Files identical despite different names*

### Comparing `softpy-0.0.2/softpy.egg-info/PKG-INFO` & `softpy-0.0.3/softpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for soft computing in Python.
 Home-page: https://pypi.org/project/scikit-weak/
 Author: Andrea Campagner
 Author-email: onyris93@gmail.com
 License: LICENSE.txt
 Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
```

