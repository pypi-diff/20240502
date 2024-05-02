# Comparing `tmp/vfo-0.0.8.tar.gz` & `tmp/vfo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vfo-0.0.8.tar", last modified: Sat Oct  8 07:44:23 2022, max compression
+gzip compressed data, was "dist\vfo-0.0.9.tar", last modified: Thu Oct 13 05:40:19 2022, max compression
```

## Comparing `vfo-0.0.8.tar` & `vfo-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-10-08 07:44:23.000000 vfo-0.0.8/
--rw-rw-rw-   0        0        0     1457 2022-10-08 07:44:23.000000 vfo-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      753 2021-11-29 18:41:45.000000 vfo-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2022-10-08 07:44:23.000000 vfo-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      815 2022-10-08 07:39:47.000000 vfo-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-08 07:44:23.000000 vfo-0.0.8/vfo/
--rw-rw-rw-   0        0        0    59006 2021-11-29 18:56:39.000000 vfo-0.0.8/vfo/Get_Rendering.py
--rw-rw-rw-   0        0        0        0 2021-11-29 18:56:39.000000 vfo-0.0.8/vfo/__init__.py
--rw-rw-rw-   0        0        0      796 2022-09-02 15:17:05.000000 vfo-0.0.8/vfo/classTags.py
--rw-rw-rw-   0        0        0    22338 2022-10-08 07:34:55.000000 vfo-0.0.8/vfo/internal_database_functions.py
--rw-rw-rw-   0        0        0    22582 2022-06-14 06:05:25.000000 vfo-0.0.8/vfo/internal_plotting_functions.py
--rw-rw-rw-   0        0        0     6410 2021-11-29 18:56:39.000000 vfo-0.0.8/vfo/live_model_view.py
--rw-rw-rw-   0        0        0    56086 2022-10-07 15:06:26.000000 vfo-0.0.8/vfo/vfo.py
-drwxrwxrwx   0        0        0        0 2022-10-08 07:44:23.000000 vfo-0.0.8/vfo.egg-info/
--rw-rw-rw-   0        0        0     1457 2022-10-08 07:44:22.000000 vfo-0.0.8/vfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2022-10-08 07:44:22.000000 vfo-0.0.8/vfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-08 07:44:22.000000 vfo-0.0.8/vfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2022-10-08 07:44:22.000000 vfo-0.0.8/vfo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-10-08 07:44:22.000000 vfo-0.0.8/vfo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-10-13 05:40:19.000000 vfo-0.0.9/
+-rw-rw-rw-   0        0        0     1457 2022-10-13 05:40:19.000000 vfo-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2021-11-29 18:41:45.000000 vfo-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-10-13 05:40:19.000000 vfo-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      815 2022-10-13 05:38:21.000000 vfo-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-13 05:40:19.000000 vfo-0.0.9/vfo/
+-rw-rw-rw-   0        0        0    59006 2021-11-29 18:56:39.000000 vfo-0.0.9/vfo/Get_Rendering.py
+-rw-rw-rw-   0        0        0        0 2021-11-29 18:56:39.000000 vfo-0.0.9/vfo/__init__.py
+-rw-rw-rw-   0        0        0      796 2022-09-02 15:17:05.000000 vfo-0.0.9/vfo/classTags.py
+-rw-rw-rw-   0        0        0    22338 2022-10-08 07:34:55.000000 vfo-0.0.9/vfo/internal_database_functions.py
+-rw-rw-rw-   0        0        0    22582 2022-06-14 06:05:25.000000 vfo-0.0.9/vfo/internal_plotting_functions.py
+-rw-rw-rw-   0        0        0     6410 2021-11-29 18:56:39.000000 vfo-0.0.9/vfo/live_model_view.py
+-rw-rw-rw-   0        0        0    56083 2022-10-13 05:37:39.000000 vfo-0.0.9/vfo/vfo.py
+drwxrwxrwx   0        0        0        0 2022-10-13 05:40:19.000000 vfo-0.0.9/vfo.egg-info/
+-rw-rw-rw-   0        0        0     1457 2022-10-13 05:40:19.000000 vfo-0.0.9/vfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2022-10-13 05:40:19.000000 vfo-0.0.9/vfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-13 05:40:19.000000 vfo-0.0.9/vfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2022-10-13 05:40:19.000000 vfo-0.0.9/vfo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2022-10-13 05:40:19.000000 vfo-0.0.9/vfo.egg-info/top_level.txt
```

### Comparing `vfo-0.0.8/PKG-INFO` & `vfo-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfo
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for visualization of OpenSees models.
 Home-page: https://github.com/u-anurag/vfo
 Author: anurag upadhyay
 Author-email: iitg.anurag@gmail.com
 License: UNKNOWN
 Description: # vfo (Visualization For OpenSees)
         Python Commands to visualize OpenSees models and components.
```

### Comparing `vfo-0.0.8/README.md` & `vfo-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vfo-0.0.8/setup.py` & `vfo-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vfo", # Replace with your own username
-    version="0.0.8",
+    version="0.0.9",
     author="anurag upadhyay",
     author_email="iitg.anurag@gmail.com",
     description="A package for visualization of OpenSees models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/u-anurag/vfo",
     packages=setuptools.find_packages(),
```

### Comparing `vfo-0.0.8/vfo/Get_Rendering.py` & `vfo-0.0.9/vfo/Get_Rendering.py`

 * *Files identical despite different names*

### Comparing `vfo-0.0.8/vfo/classTags.py` & `vfo-0.0.9/vfo/classTags.py`

 * *Files identical despite different names*

### Comparing `vfo-0.0.8/vfo/internal_database_functions.py` & `vfo-0.0.9/vfo/internal_database_functions.py`

 * *Files identical despite different names*

### Comparing `vfo-0.0.8/vfo/internal_plotting_functions.py` & `vfo-0.0.9/vfo/internal_plotting_functions.py`

 * *Files identical despite different names*

### Comparing `vfo-0.0.8/vfo/live_model_view.py` & `vfo-0.0.9/vfo/live_model_view.py`

 * *Files identical despite different names*

### Comparing `vfo-0.0.8/vfo/vfo.py` & `vfo-0.0.9/vfo/vfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 import math
 
 from math import asin
 import matplotlib.pyplot as plt
 import numpy as np
 import pyvista as pv
 
-
 for line in range(0,len(sys.argv)):
     if "ipykernel_launcher.py" in sys.argv[line]:
         # matplotlib.use('nbagg')
         pv.set_jupyter_backend('panel')
         break
     else:
         pass
@@ -761,15 +760,15 @@
 	if ndm == 2:
 		for ii in range(0,len(this_nodeArray[:,0])):
 			nodeArray[ii,0:3] = this_nodeArray[ii,:]
 	else:
 		nodeArray = this_nodeArray
 		
 	pl = pv.Plotter()		
-	# pl.show(interactive_update=True)
+	pl.show(interactive_update=True)
 	
 	
 	# DeflectedNodeCoordArray = nodeArray[:,1:]+ scale*displacement_nodeArray[jj,:,:]
 	DeflectedNodeCoordArray = nodeArray[:,1:]+ scale*Mode_nodeArray[:,1:]
 	
 	DeflectedNodeArray = np.hstack((nodeArray[:,0].reshape(len(nodeArray[:,0]),1),DeflectedNodeCoordArray[:,0:]))
 	# DeflectedNodeArray = Mode_nodeArray
```

### Comparing `vfo-0.0.8/vfo.egg-info/PKG-INFO` & `vfo-0.0.9/vfo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfo
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for visualization of OpenSees models.
 Home-page: https://github.com/u-anurag/vfo
 Author: anurag upadhyay
 Author-email: iitg.anurag@gmail.com
 License: UNKNOWN
 Description: # vfo (Visualization For OpenSees)
         Python Commands to visualize OpenSees models and components.
```

