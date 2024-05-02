# Comparing `tmp/brisque-0.0.15.tar.gz` & `tmp/brisque-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brisque-0.0.15.tar", last modified: Tue Oct 18 19:09:38 2022, max compression
+gzip compressed data, was "brisque-0.0.16.tar", last modified: Thu May  2 13:10:32 2024, max compression
```

## Comparing `brisque-0.0.15.tar` & `brisque-0.0.16.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:09:38.197635 brisque-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-18 19:08:58.000000 brisque-0.0.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-10-18 19:09:38.197635 brisque-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-18 19:08:58.000000 brisque-0.0.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:09:38.197635 brisque-0.0.15/brisque/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-18 19:08:58.000000 brisque-0.0.15/brisque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7723 2022-10-18 19:08:58.000000 brisque-0.0.15/brisque/brisque.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:09:38.197635 brisque-0.0.15/brisque/models/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-10-18 19:08:58.000000 brisque-0.0.15/brisque/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-10-18 19:08:58.000000 brisque-0.0.15/brisque/models/normalize.pickle
--rw-r--r--   0 runner    (1001) docker     (121)   351414 2022-10-18 19:08:58.000000 brisque-0.0.15/brisque/models/svm.txt
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-18 19:08:58.000000 brisque-0.0.15/brisque/test_brisque.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 19:09:38.197635 brisque-0.0.15/brisque.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-10-18 19:09:38.000000 brisque-0.0.15/brisque.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-10-18 19:09:38.000000 brisque-0.0.15/brisque.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 19:09:38.000000 brisque-0.0.15/brisque.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-18 19:09:38.000000 brisque-0.0.15/brisque.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-18 19:09:38.000000 brisque-0.0.15/brisque.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-18 19:08:58.000000 brisque-0.0.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-18 19:08:58.000000 brisque-0.0.15/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-18 19:09:38.197635 brisque-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-10-18 19:08:58.000000 brisque-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:10:32.804065 brisque-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 13:10:11.000000 brisque-0.0.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 13:10:11.000000 brisque-0.0.16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-02 13:10:32.804065 brisque-0.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-02 13:10:11.000000 brisque-0.0.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:10:32.800065 brisque-0.0.16/brisque/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 13:10:11.000000 brisque-0.0.16/brisque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-02 13:10:11.000000 brisque-0.0.16/brisque/brisque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:10:32.804065 brisque-0.0.16/brisque/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 13:10:11.000000 brisque-0.0.16/brisque/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-02 13:10:11.000000 brisque-0.0.16/brisque/models/normalize.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)   351414 2024-05-02 13:10:11.000000 brisque-0.0.16/brisque/models/svm.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:10:32.804065 brisque-0.0.16/brisque/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:10:11.000000 brisque-0.0.16/brisque/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-02 13:10:11.000000 brisque-0.0.16/brisque/tests/test_brisque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:10:32.804065 brisque-0.0.16/brisque.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-02 13:10:32.000000 brisque-0.0.16/brisque.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 13:10:32.000000 brisque-0.0.16/brisque.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:10:32.000000 brisque-0.0.16/brisque.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 13:10:32.000000 brisque-0.0.16/brisque.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 13:10:32.000000 brisque-0.0.16/brisque.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-02 13:10:11.000000 brisque-0.0.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-02 13:10:11.000000 brisque-0.0.16/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 13:10:32.804065 brisque-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 13:10:11.000000 brisque-0.0.16/setup.py
```

### Comparing `brisque-0.0.15/PKG-INFO` & `brisque-0.0.16/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brisque
-Version: 0.0.15
+Version: 0.0.16
 Summary: Image Quality
 Home-page: https://github.com/rehanguha/brisque
 Author: Rehan Guha
 Author-email: rehanguha29@gmail.com
 License: mit
 Keywords: quality,svm,image,maths
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,20 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Developers
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scikit-image
+Requires-Dist: scipy
+Requires-Dist: opencv-python
+Requires-Dist: libsvm-official
 
 # Blind/Referenceless Image Spatial Quality Evaluator (BRISQUE) 
 
 BRISQUE is a no-reference image quality score.
 
 A good place to know how BRISQUE works : [LearnOpenCV](https://learnopencv.com/image-quality-assessment-brisque/)
 
@@ -46,19 +52,44 @@
 
 obj = BRISQUE(url=True)
 obj.score("<URL for the Image>")
 ```
 
 ### Example
 
+#### Local Image
+
 - Input
 ```python
 from brisque import BRISQUE
+import numpy as np
+from PIL import Image
+
+img_path = "brisque/tests/sample-image.jpg"
+img = Image.open(img_path)
+ndarray = np.asarray(img)
 
-obj = BRISQUE("https://www.mathworks.com/help/examples/images/win64/CalculateBRISQUEScoreUsingCustomFeatureModelExample_01.png", 
-        url=True)
-obj.score()
+obj = BRISQUE(url=False)
+obj.score(img=ndarray)
 ```
 - Output
 ```
-74.41910327611319
+34.84883848208594
 ```
+
+#### URL
+
+- Input
+```python
+from brisque import BRISQUE
+
+URL = "https://www.mathworks.com/help/examples/images/win64/CalculateBRISQUEScoreUsingCustomFeatureModelExample_01.png"
+
+obj = BRISQUE(url=True)
+obj.score(URL)
+```
+- Output
+```
+71.73427549219988
+```
+
+
```

### Comparing `brisque-0.0.15/README.md` & `brisque-0.0.16/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -27,19 +27,44 @@
 
 obj = BRISQUE(url=True)
 obj.score("<URL for the Image>")
 ```
 
 ### Example
 
+#### Local Image
+
+- Input
+```python
+from brisque import BRISQUE
+import numpy as np
+from PIL import Image
+
+img_path = "brisque/tests/sample-image.jpg"
+img = Image.open(img_path)
+ndarray = np.asarray(img)
+
+obj = BRISQUE(url=False)
+obj.score(img=ndarray)
+```
+- Output
+```
+34.84883848208594
+```
+
+#### URL
+
 - Input
 ```python
 from brisque import BRISQUE
 
-obj = BRISQUE("https://www.mathworks.com/help/examples/images/win64/CalculateBRISQUEScoreUsingCustomFeatureModelExample_01.png", 
-        url=True)
-obj.score()
+URL = "https://www.mathworks.com/help/examples/images/win64/CalculateBRISQUEScoreUsingCustomFeatureModelExample_01.png"
+
+obj = BRISQUE(url=True)
+obj.score(URL)
 ```
 - Output
 ```
-74.41910327611319
+71.73427549219988
 ```
+
+
```

### Comparing `brisque-0.0.15/brisque/brisque.py` & `brisque-0.0.16/brisque/brisque.py`

 * *Files identical despite different names*

### Comparing `brisque-0.0.15/brisque/models/normalize.pickle` & `brisque-0.0.16/brisque/models/normalize.pickle`

 * *Files identical despite different names*

### Comparing `brisque-0.0.15/brisque/models/svm.txt` & `brisque-0.0.16/brisque/models/svm.txt`

 * *Files identical despite different names*

### Comparing `brisque-0.0.15/brisque.egg-info/PKG-INFO` & `brisque-0.0.16/brisque.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brisque
-Version: 0.0.15
+Version: 0.0.16
 Summary: Image Quality
 Home-page: https://github.com/rehanguha/brisque
 Author: Rehan Guha
 Author-email: rehanguha29@gmail.com
 License: mit
 Keywords: quality,svm,image,maths
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,20 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Developers
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scikit-image
+Requires-Dist: scipy
+Requires-Dist: opencv-python
+Requires-Dist: libsvm-official
 
 # Blind/Referenceless Image Spatial Quality Evaluator (BRISQUE) 
 
 BRISQUE is a no-reference image quality score.
 
 A good place to know how BRISQUE works : [LearnOpenCV](https://learnopencv.com/image-quality-assessment-brisque/)
 
@@ -46,19 +52,44 @@
 
 obj = BRISQUE(url=True)
 obj.score("<URL for the Image>")
 ```
 
 ### Example
 
+#### Local Image
+
 - Input
 ```python
 from brisque import BRISQUE
+import numpy as np
+from PIL import Image
+
+img_path = "brisque/tests/sample-image.jpg"
+img = Image.open(img_path)
+ndarray = np.asarray(img)
 
-obj = BRISQUE("https://www.mathworks.com/help/examples/images/win64/CalculateBRISQUEScoreUsingCustomFeatureModelExample_01.png", 
-        url=True)
-obj.score()
+obj = BRISQUE(url=False)
+obj.score(img=ndarray)
 ```
 - Output
 ```
-74.41910327611319
+34.84883848208594
 ```
+
+#### URL
+
+- Input
+```python
+from brisque import BRISQUE
+
+URL = "https://www.mathworks.com/help/examples/images/win64/CalculateBRISQUEScoreUsingCustomFeatureModelExample_01.png"
+
+obj = BRISQUE(url=True)
+obj.score(URL)
+```
+- Output
+```
+71.73427549219988
+```
+
+
```

### Comparing `brisque-0.0.15/setup.py` & `brisque-0.0.16/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,9 +24,9 @@
         "Natural Language :: English",
         "Programming Language :: Python",
         'Topic :: Software Development :: Libraries :: Python Modules',
         "Topic :: Scientific/Engineering",
         'Intended Audience :: Developers',
     ],
     python_requires='>=2.7',
-    install_requires=['numpy', 'scikit-image', 'scipy', 'opencv-python', 'libsvm'],
+    install_requires=['numpy', 'scikit-image', 'scipy', 'opencv-python', 'libsvm-official'],
 )
```

