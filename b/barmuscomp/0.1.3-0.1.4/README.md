# Comparing `tmp/barmuscomp-0.1.3.tar.gz` & `tmp/barmuscomp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barmuscomp-0.1.3.tar", last modified: Thu Apr 25 15:14:22 2024, max compression
+gzip compressed data, was "barmuscomp-0.1.4.tar", last modified: Thu May  2 15:59:36 2024, max compression
```

## Comparing `barmuscomp-0.1.3.tar` & `barmuscomp-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       88 2023-10-26 01:08:08.000000 barmuscomp-0.1.3/AUTHORS
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1503 2024-01-10 11:57:04.000000 barmuscomp-0.1.3/LICENSE.md
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3711 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/PKG-INFO
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     2985 2023-10-26 01:08:08.000000 barmuscomp-0.1.3/README.md
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/barmuscomp/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      305 2024-01-10 11:57:01.000000 barmuscomp-0.1.3/barmuscomp/__init__.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    36646 2024-01-10 11:57:01.000000 barmuscomp-0.1.3/barmuscomp/ae.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    19648 2024-01-10 11:57:02.000000 barmuscomp-0.1.3/barmuscomp/ae_ntd.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    13589 2024-01-10 11:57:02.000000 barmuscomp-0.1.3/barmuscomp/ae_utils.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    13546 2024-01-10 11:57:02.000000 barmuscomp-0.1.3/barmuscomp/lra.py
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/barmuscomp/model/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        0 2023-10-26 01:08:08.000000 barmuscomp-0.1.3/barmuscomp/model/__init__.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     7339 2024-01-31 09:55:24.000000 barmuscomp-0.1.3/barmuscomp/model/current_plot.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3039 2023-10-26 01:08:08.000000 barmuscomp-0.1.3/barmuscomp/model/early_stopping.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      201 2024-01-10 11:57:03.000000 barmuscomp-0.1.3/barmuscomp/model/errors.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4388 2024-01-10 11:57:03.000000 barmuscomp-0.1.3/barmuscomp/model/features.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    19983 2024-01-10 11:57:03.000000 barmuscomp-0.1.3/barmuscomp/model/pattern_study.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4910 2024-01-10 11:57:03.000000 barmuscomp-0.1.3/barmuscomp/model/plot_comparison_ae_ntd.py
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/barmuscomp/scripts/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        0 2023-10-26 01:08:08.000000 barmuscomp-0.1.3/barmuscomp/scripts/__init__.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1790 2024-01-10 11:57:03.000000 barmuscomp-0.1.3/barmuscomp/scripts/default_path.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     7444 2024-01-10 11:57:04.000000 barmuscomp-0.1.3/barmuscomp/scripts/overall_scripts.py
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/barmuscomp.egg-info/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3711 2024-04-25 15:14:22.000000 barmuscomp-0.1.3/barmuscomp.egg-info/PKG-INFO
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      642 2024-04-25 15:14:22.000000 barmuscomp-0.1.3/barmuscomp.egg-info/SOURCES.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        1 2024-04-25 15:14:22.000000 barmuscomp-0.1.3/barmuscomp.egg-info/dependency_links.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      172 2024-04-25 15:14:22.000000 barmuscomp-0.1.3/barmuscomp.egg-info/requires.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       11 2024-04-25 15:14:22.000000 barmuscomp-0.1.3/barmuscomp.egg-info/top_level.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       38 2024-04-25 15:14:22.971230 barmuscomp-0.1.3/setup.cfg
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1329 2024-04-25 15:14:06.000000 barmuscomp-0.1.3/setup.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       88 2023-10-26 01:08:08.000000 barmuscomp-0.1.4/AUTHORS
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1503 2024-01-10 11:57:04.000000 barmuscomp-0.1.4/LICENSE.md
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3689 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/PKG-INFO
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     2985 2023-10-26 01:08:08.000000 barmuscomp-0.1.4/README.md
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/barmuscomp/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      305 2024-01-10 11:57:01.000000 barmuscomp-0.1.4/barmuscomp/__init__.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    36646 2024-01-10 11:57:01.000000 barmuscomp-0.1.4/barmuscomp/ae.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    19648 2024-01-10 11:57:02.000000 barmuscomp-0.1.4/barmuscomp/ae_ntd.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    13589 2024-01-10 11:57:02.000000 barmuscomp-0.1.4/barmuscomp/ae_utils.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    13546 2024-01-10 11:57:02.000000 barmuscomp-0.1.4/barmuscomp/lra.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/barmuscomp/model/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        0 2023-10-26 01:08:08.000000 barmuscomp-0.1.4/barmuscomp/model/__init__.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     7339 2024-01-31 09:55:24.000000 barmuscomp-0.1.4/barmuscomp/model/current_plot.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3039 2023-10-26 01:08:08.000000 barmuscomp-0.1.4/barmuscomp/model/early_stopping.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      201 2024-01-10 11:57:03.000000 barmuscomp-0.1.4/barmuscomp/model/errors.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4388 2024-01-10 11:57:03.000000 barmuscomp-0.1.4/barmuscomp/model/features.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    19983 2024-01-10 11:57:03.000000 barmuscomp-0.1.4/barmuscomp/model/pattern_study.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4910 2024-01-10 11:57:03.000000 barmuscomp-0.1.4/barmuscomp/model/plot_comparison_ae_ntd.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/barmuscomp/scripts/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        0 2023-10-26 01:08:08.000000 barmuscomp-0.1.4/barmuscomp/scripts/__init__.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1790 2024-01-10 11:57:03.000000 barmuscomp-0.1.4/barmuscomp/scripts/default_path.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     7444 2024-01-10 11:57:04.000000 barmuscomp-0.1.4/barmuscomp/scripts/overall_scripts.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/barmuscomp.egg-info/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3689 2024-05-02 15:59:36.000000 barmuscomp-0.1.4/barmuscomp.egg-info/PKG-INFO
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      642 2024-05-02 15:59:36.000000 barmuscomp-0.1.4/barmuscomp.egg-info/SOURCES.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        1 2024-05-02 15:59:36.000000 barmuscomp-0.1.4/barmuscomp.egg-info/dependency_links.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      177 2024-05-02 15:59:36.000000 barmuscomp-0.1.4/barmuscomp.egg-info/requires.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       11 2024-05-02 15:59:36.000000 barmuscomp-0.1.4/barmuscomp.egg-info/top_level.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       38 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/setup.cfg
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1305 2024-05-02 15:57:42.000000 barmuscomp-0.1.4/setup.py
```

### Comparing `barmuscomp-0.1.3/LICENSE.md` & `barmuscomp-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/PKG-INFO` & `barmuscomp-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: barmuscomp
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for barwise compression applied on musical segmentation.
 Home-page: https://gitlab.inria.fr/amarmore/barmuscomp
 Author: Marmoret Axel
 Author-email: axel.marmoret@irisa.fr
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS
 
 # BarMusComp: Encoding songs with linear and nonlinear compression methods to reveal structure #
 
 Hello, and welcome on this repository!
```

### Comparing `barmuscomp-0.1.3/README.md` & `barmuscomp-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/ae.py` & `barmuscomp-0.1.4/barmuscomp/ae.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/ae_ntd.py` & `barmuscomp-0.1.4/barmuscomp/ae_ntd.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/ae_utils.py` & `barmuscomp-0.1.4/barmuscomp/ae_utils.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/lra.py` & `barmuscomp-0.1.4/barmuscomp/lra.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/model/current_plot.py` & `barmuscomp-0.1.4/barmuscomp/model/current_plot.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/model/early_stopping.py` & `barmuscomp-0.1.4/barmuscomp/model/early_stopping.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/model/features.py` & `barmuscomp-0.1.4/barmuscomp/model/features.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/model/pattern_study.py` & `barmuscomp-0.1.4/barmuscomp/model/pattern_study.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/model/plot_comparison_ae_ntd.py` & `barmuscomp-0.1.4/barmuscomp/model/plot_comparison_ae_ntd.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/scripts/default_path.py` & `barmuscomp-0.1.4/barmuscomp/scripts/default_path.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp/scripts/overall_scripts.py` & `barmuscomp-0.1.4/barmuscomp/scripts/overall_scripts.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/barmuscomp.egg-info/PKG-INFO` & `barmuscomp-0.1.4/barmuscomp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: barmuscomp
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for barwise compression applied on musical segmentation.
 Home-page: https://gitlab.inria.fr/amarmore/barmuscomp
 Author: Marmoret Axel
 Author-email: axel.marmoret@irisa.fr
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS
 
 # BarMusComp: Encoding songs with linear and nonlinear compression methods to reveal structure #
 
 Hello, and welcome on this repository!
```

### Comparing `barmuscomp-0.1.3/barmuscomp.egg-info/SOURCES.txt` & `barmuscomp-0.1.4/barmuscomp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.3/setup.py` & `barmuscomp-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="barmuscomp",
-    version="0.1.3",
+    version="0.1.4",
     author="Marmoret Axel",
     author_email="axel.marmoret@irisa.fr",
     description="Package for barwise compression applied on musical segmentation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.inria.fr/amarmore/barmuscomp",
     packages=setuptools.find_packages(),
@@ -23,22 +23,21 @@
         "Programming Language :: Python :: 3.8"
     ],
     license='BSD',
     install_requires=[
         'as_seg',
         'librosa >= 0.8.0',
         #'madmom @ git+https://github.com/CPJKU/madmom',
-        'madmom >= 0.16.1' ,
+        'madmom >= 0.16.1',
         'matplotlib',
         'mir_eval >= 0.6',
         'mirdata >= 0.3.3',
         'nn-fac >= 0.2.0',
         'numpy >= 1.18.2',
         'pandas',
         'scipy >= 1.4.1',
-        'sklearn',
+        'scikit-learn',
         'soundfile',
         'tensorly >= 0.5.1',
         'torch >= 1.8.0'
     ],
-    python_requires='>3.7',
 )
```

