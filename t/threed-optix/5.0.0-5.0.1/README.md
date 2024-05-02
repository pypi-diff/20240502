# Comparing `tmp/threed_optix-5.0.0.tar.gz` & `tmp/threed_optix-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threed_optix-5.0.0.tar", last modified: Wed May  1 11:16:46 2024, max compression
+gzip compressed data, was "threed_optix-5.0.1.tar", last modified: Wed May  1 13:31:40 2024, max compression
```

## Comparing `threed_optix-5.0.0.tar` & `threed_optix-5.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.0/.gitignore
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.0/LICENSE.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-01 11:16:46.290742 threed_optix-5.0.0/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.0/README.md
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/help/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    46819 2024-05-01 11:13:46.000000 threed_optix-5.0.0/help/SDK help text.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    46929 2024-05-01 11:13:46.000000 threed_optix-5.0.0/help/SDK help.md
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-01 11:16:46.290742 threed_optix-5.0.0/setup.cfg
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1242 2024-05-01 11:13:46.000000 threed_optix-5.0.0/setup.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/src/
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/src/threed_optix/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      832 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23682 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/analyses.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.0/src/threed_optix/beams.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43188 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/client.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.0/src/threed_optix/optimize.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/src/threed_optix/package_utils/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.0/src/threed_optix/package_utils/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15563 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/package_utils/api.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3247 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/package_utils/general.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/package_utils/math.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.0/src/threed_optix/package_utils/matlab.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19082 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/package_utils/vars.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    59842 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/parts.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    14858 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/simulations.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4718 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/utils.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/src/threed_optix.egg-info/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-01 11:16:46.000000 threed_optix-5.0.0/src/threed_optix.egg-info/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-01 11:16:46.000000 threed_optix-5.0.0/src/threed_optix.egg-info/SOURCES.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-01 11:16:46.000000 threed_optix-5.0.0/src/threed_optix.egg-info/dependency_links.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      116 2024-05-01 11:16:46.000000 threed_optix-5.0.0/src/threed_optix.egg-info/requires.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-01 11:16:46.000000 threed_optix-5.0.0/src/threed_optix.egg-info/top_level.txt
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 13:31:40.738132 threed_optix-5.0.1/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.1/.gitignore
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.1/LICENSE.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-01 13:31:40.738132 threed_optix-5.0.1/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.1/README.md
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 13:31:40.738132 threed_optix-5.0.1/help/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    46819 2024-05-01 11:13:46.000000 threed_optix-5.0.1/help/SDK help text.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    46929 2024-05-01 11:13:46.000000 threed_optix-5.0.1/help/SDK help.md
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-01 13:31:40.738132 threed_optix-5.0.1/setup.cfg
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1242 2024-05-01 11:13:46.000000 threed_optix-5.0.1/setup.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 13:31:40.728132 threed_optix-5.0.1/src/
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 13:31:40.738132 threed_optix-5.0.1/src/threed_optix/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      832 2024-05-01 11:13:46.000000 threed_optix-5.0.1/src/threed_optix/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23682 2024-05-01 11:13:46.000000 threed_optix-5.0.1/src/threed_optix/analyses.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.1/src/threed_optix/beams.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43188 2024-05-01 11:13:46.000000 threed_optix-5.0.1/src/threed_optix/client.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.1/src/threed_optix/optimize.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 13:31:40.738132 threed_optix-5.0.1/src/threed_optix/package_utils/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.1/src/threed_optix/package_utils/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15563 2024-05-01 11:13:46.000000 threed_optix-5.0.1/src/threed_optix/package_utils/api.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3247 2024-05-01 11:13:46.000000 threed_optix-5.0.1/src/threed_optix/package_utils/general.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.1/src/threed_optix/package_utils/math.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.1/src/threed_optix/package_utils/matlab.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19082 2024-05-01 13:30:57.000000 threed_optix-5.0.1/src/threed_optix/package_utils/vars.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    59842 2024-05-01 11:13:46.000000 threed_optix-5.0.1/src/threed_optix/parts.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15018 2024-05-01 13:31:16.000000 threed_optix-5.0.1/src/threed_optix/simulations.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4718 2024-05-01 11:13:46.000000 threed_optix-5.0.1/src/threed_optix/utils.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 13:31:40.738132 threed_optix-5.0.1/src/threed_optix.egg-info/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-01 13:31:40.000000 threed_optix-5.0.1/src/threed_optix.egg-info/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-01 13:31:40.000000 threed_optix-5.0.1/src/threed_optix.egg-info/SOURCES.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-01 13:31:40.000000 threed_optix-5.0.1/src/threed_optix.egg-info/dependency_links.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      116 2024-05-01 13:31:40.000000 threed_optix-5.0.1/src/threed_optix.egg-info/requires.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-01 13:31:40.000000 threed_optix-5.0.1/src/threed_optix.egg-info/top_level.txt
```

### Comparing `threed_optix-5.0.0/LICENSE.txt` & `threed_optix-5.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/PKG-INFO` & `threed_optix-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed_optix
-Version: 5.0.0
+Version: 5.0.1
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-5.0.0/README.md` & `threed_optix-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/help/SDK help text.txt` & `threed_optix-5.0.1/help/SDK help text.txt`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/help/SDK help.md` & `threed_optix-5.0.1/help/SDK help.md`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/setup.py` & `threed_optix-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/src/threed_optix/__init__.py` & `threed_optix-5.0.1/src/threed_optix/__init__.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/src/threed_optix/analyses.py` & `threed_optix-5.0.1/src/threed_optix/analyses.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/src/threed_optix/beams.py` & `threed_optix-5.0.1/src/threed_optix/beams.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/src/threed_optix/client.py` & `threed_optix-5.0.1/src/threed_optix/client.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/src/threed_optix/package_utils/api.py` & `threed_optix-5.0.1/src/threed_optix/package_utils/api.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/src/threed_optix/package_utils/general.py` & `threed_optix-5.0.1/src/threed_optix/package_utils/general.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/src/threed_optix/package_utils/math.py` & `threed_optix-5.0.1/src/threed_optix/package_utils/math.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/src/threed_optix/package_utils/vars.py` & `threed_optix-5.0.1/src/threed_optix/package_utils/vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import re
 
 DEBUG = False
 BASE_BACKUP = 'DEFAULT'
 VALID_RESPONSE_CODES = [200, 201, 202, 204]
 # Take the version of the package
-VERSION = "5.0.0"
+VERSION = "5.0.1"
 
 
 #Base API URL
 API_URL = "https://api.3doptix.com/v1"
 
 class Analyses:
     DEFAULT_NUM_RAYS = 30
```

### Comparing `threed_optix-5.0.0/src/threed_optix/parts.py` & `threed_optix-5.0.1/src/threed_optix/parts.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/src/threed_optix/simulations.py` & `threed_optix-5.0.1/src/threed_optix/simulations.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,17 +351,26 @@
 
     def delete_part(self, part: tdo_parts.Part):
         '''
         Deletes the part from the setup.
         '''
         self._api._delete_part(self.id, part.id)
         self._parts = [p for p in self.parts if p.id != part.id]
+
         if isinstance(part, tdo_parts.LightSource):
             for part in self:
+
+                if part._surfaces is None:
+                    continue
+
                 for surface in part.surfaces:
+
+                    if surface._analyses is None:
+                        continue
+
                     for analysis in surface.analyses:
                         # if the laser id in the analysis rays attribute as key, delete the entry
                         if part.id in analysis.rays:
                             del analysis.rays[part.id]
 
         return
```

### Comparing `threed_optix-5.0.0/src/threed_optix/utils.py` & `threed_optix-5.0.1/src/threed_optix/utils.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.0/src/threed_optix.egg-info/PKG-INFO` & `threed_optix-5.0.1/src/threed_optix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed-optix
-Version: 5.0.0
+Version: 5.0.1
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-5.0.0/src/threed_optix.egg-info/SOURCES.txt` & `threed_optix-5.0.1/src/threed_optix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

