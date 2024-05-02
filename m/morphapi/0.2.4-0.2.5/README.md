# Comparing `tmp/morphapi-0.2.4.tar.gz` & `tmp/morphapi-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphapi-0.2.4.tar", last modified: Fri Apr 26 13:57:18 2024, max compression
+gzip compressed data, was "morphapi-0.2.5.tar", last modified: Thu May  2 16:27:03 2024, max compression
```

## Comparing `morphapi-0.2.4.tar` & `morphapi-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.499450 morphapi-0.2.4/
-drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.460327 morphapi-0.2.4/.github/
-drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.462115 morphapi-0.2.4/.github/workflows/
--rw-r--r--   0 adamtyson   (501) staff       (20)     1444 2024-02-09 14:31:34.000000 morphapi-0.2.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 adamtyson   (501) staff       (20)      978 2024-02-09 14:31:34.000000 morphapi-0.2.4/.gitignore
--rw-r--r--   0 adamtyson   (501) staff       (20)      624 2024-04-26 10:23:07.000000 morphapi-0.2.4/CITATION.cff
--rw-r--r--   0 adamtyson   (501) staff       (20)     1082 2024-02-09 14:31:34.000000 morphapi-0.2.4/LICENSE
--rw-r--r--   0 adamtyson   (501) staff       (20)      229 2024-04-26 10:23:07.000000 morphapi-0.2.4/MANIFEST.in
--rw-r--r--   0 adamtyson   (501) staff       (20)     2277 2024-04-26 13:57:18.499110 morphapi-0.2.4/PKG-INFO
--rw-r--r--   0 adamtyson   (501) staff       (20)      402 2024-02-09 14:31:34.000000 morphapi-0.2.4/README.md
-drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.473334 morphapi-0.2.4/morphapi/
--rw-r--r--   0 adamtyson   (501) staff       (20)      174 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/__init__.py
-drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.475788 morphapi-0.2.4/morphapi/api/
--rw-r--r--   0 adamtyson   (501) staff       (20)        0 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/api/__init__.py
--rw-r--r--   0 adamtyson   (501) staff       (20)     3651 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/api/allenmorphology.py
--rw-r--r--   0 adamtyson   (501) staff       (20)    16887 2024-04-26 10:23:07.000000 morphapi-0.2.4/morphapi/api/mouselight.py
--rw-r--r--   0 adamtyson   (501) staff       (20)     5706 2024-04-26 10:23:07.000000 morphapi-0.2.4/morphapi/api/mpin_celldb.py
--rw-r--r--   0 adamtyson   (501) staff       (20)     8449 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/api/neuromorphorg.py
-drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.495376 morphapi-0.2.4/morphapi/morphology/
--rw-r--r--   0 adamtyson   (501) staff       (20)        0 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/morphology/__init__.py
--rw-r--r--   0 adamtyson   (501) staff       (20)     4531 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/morphology/cache.py
--rw-r--r--   0 adamtyson   (501) staff       (20)     8850 2024-04-26 13:56:19.000000 morphapi-0.2.4/morphapi/morphology/morphology.py
--rw-r--r--   0 adamtyson   (501) staff       (20)     1627 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/paths_manager.py
-drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.496680 morphapi-0.2.4/morphapi/utils/
--rw-r--r--   0 adamtyson   (501) staff       (20)        0 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/utils/__init__.py
--rw-r--r--   0 adamtyson   (501) staff       (20)     3086 2024-02-09 14:31:34.000000 morphapi-0.2.4/morphapi/utils/data_io.py
--rw-r--r--   0 adamtyson   (501) staff       (20)     4072 2024-04-26 10:23:07.000000 morphapi-0.2.4/morphapi/utils/webqueries.py
-drwxr-xr-x   0 adamtyson   (501) staff       (20)        0 2024-04-26 13:57:18.497116 morphapi-0.2.4/morphapi.egg-info/
--rw-r--r--   0 adamtyson   (501) staff       (20)     2277 2024-04-26 13:57:18.000000 morphapi-0.2.4/morphapi.egg-info/PKG-INFO
--rw-r--r--   0 adamtyson   (501) staff       (20)      631 2024-04-26 13:57:18.000000 morphapi-0.2.4/morphapi.egg-info/SOURCES.txt
--rw-r--r--   0 adamtyson   (501) staff       (20)        1 2024-04-26 13:57:18.000000 morphapi-0.2.4/morphapi.egg-info/dependency_links.txt
--rw-r--r--   0 adamtyson   (501) staff       (20)      279 2024-04-26 13:57:18.000000 morphapi-0.2.4/morphapi.egg-info/requires.txt
--rw-r--r--   0 adamtyson   (501) staff       (20)        9 2024-04-26 13:57:18.000000 morphapi-0.2.4/morphapi.egg-info/top_level.txt
--rw-r--r--   0 adamtyson   (501) staff       (20)     2421 2024-04-26 10:23:07.000000 morphapi-0.2.4/pyproject.toml
--rw-r--r--   0 adamtyson   (501) staff       (20)       38 2024-04-26 13:57:18.499523 morphapi-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:27:03.791275 morphapi-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:27:03.787275 morphapi-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:27:03.787275 morphapi-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-02 16:26:59.000000 morphapi-0.2.5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-02 16:26:59.000000 morphapi-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-02 16:26:59.000000 morphapi-0.2.5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-02 16:26:59.000000 morphapi-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 16:26:59.000000 morphapi-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-02 16:27:03.791275 morphapi-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-02 16:26:59.000000 morphapi-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:27:03.787275 morphapi-0.2.5/morphapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:27:03.787275 morphapi-0.2.5/morphapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/api/allenmorphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16887 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/api/mouselight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/api/mpin_celldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/api/neuromorphorg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:27:03.791275 morphapi-0.2.5/morphapi/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/morphology/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/morphology/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/paths_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:27:03.791275 morphapi-0.2.5/morphapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/utils/data_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-02 16:26:59.000000 morphapi-0.2.5/morphapi/utils/webqueries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:27:03.791275 morphapi-0.2.5/morphapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-02 16:27:03.000000 morphapi-0.2.5/morphapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-02 16:27:03.000000 morphapi-0.2.5/morphapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:27:03.000000 morphapi-0.2.5/morphapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 16:27:03.000000 morphapi-0.2.5/morphapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 16:27:03.000000 morphapi-0.2.5/morphapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-02 16:26:59.000000 morphapi-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:27:03.791275 morphapi-0.2.5/setup.cfg
```

### Comparing `morphapi-0.2.4/.github/workflows/test_and_deploy.yml` & `morphapi-0.2.5/.github/workflows/test_and_deploy.yml`

 * *Files 12% similar despite different names*

```diff
@@ -25,23 +25,28 @@
     name: ${{ matrix.os }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         # Run all supported Python versions on linux
         python-version: ["3.9", "3.10", "3.11"]
         os: [ubuntu-latest]
-        # Include one windows and macos run
+        # Include one windows and ARM/Intel macos run
         include:
-        - os: macos-latest
+        - os: macos-13 # Intel Mac
+          python-version: "3.10"
+        - os: macos-latest # ARM Mac
           python-version: "3.10"
         - os: windows-latest
           python-version: "3.10"
 
     steps:
       # Run tests
+      - name: install HDF5 libs on ARM Mac
+        if: matrix.os == 'macos-latest'
+        run: brew install hdf5
       - uses: neuroinformatics-unit/actions/test@v2
         with:
           python-version: ${{ matrix.python-version }}
 
   build_sdist_wheels:
     name: Build source distribution
     needs: [test]
```

### Comparing `morphapi-0.2.4/.gitignore` & `morphapi-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/CITATION.cff` & `morphapi-0.2.5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/LICENSE` & `morphapi-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/PKG-INFO` & `morphapi-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphapi
-Version: 0.2.4
+Version: 0.2.5
 Summary: A lightweight python package to download neuronal morphologies
 Author-email: Federico Claudi <hello@brainglobe.info>
 License: MIT
 Project-URL: Homepage, https://github.com/brainglobe/morphapi
 Project-URL: Bug Tracker, https://github.com/brainglobe/morphapi/issues
 Project-URL: Documentation, https://github.com/brainglobe/morphapi
 Project-URL: Source Code, https://github.com/brainglobe/morphapi
```

### Comparing `morphapi-0.2.4/morphapi/api/allenmorphology.py` & `morphapi-0.2.5/morphapi/api/allenmorphology.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/morphapi/api/mouselight.py` & `morphapi-0.2.5/morphapi/api/mouselight.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/morphapi/api/mpin_celldb.py` & `morphapi-0.2.5/morphapi/api/mpin_celldb.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/morphapi/api/neuromorphorg.py` & `morphapi-0.2.5/morphapi/api/neuromorphorg.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/morphapi/morphology/cache.py` & `morphapi-0.2.5/morphapi/morphology/cache.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/morphapi/morphology/morphology.py` & `morphapi-0.2.5/morphapi/morphology/morphology.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,31 +74,38 @@
             self.load_from_swc()
 
     def load_from_swc(self):
         if self.neuron_name is None:
             self.neuron_name = self.data_file.name
 
         nrn = nm.load_morphology(self.data_file)
-
-        # Get position and radius of some
-        soma_pos = nrn.soma.points[0, :3]
-        soma_radius = nrn.soma.points[0, -1]
-
-        # Get the rest of the data and store it
         self.morphology = nrn
-        self.points = dict(
-            soma=component(
-                soma_pos[0],
-                soma_pos[1],
-                soma_pos[2],
-                soma_pos,
-                soma_radius,
-                nrn.soma,
-            ),
-        )
+
+        try:
+            # Get position and radius of soma
+            soma_pos = nrn.soma.points[0, :3]
+            soma_radius = nrn.soma.points[0, -1]
+
+            # Get the rest of the data and store it
+            self.points = dict(
+                soma=component(
+                    soma_pos[0],
+                    soma_pos[1],
+                    soma_pos[2],
+                    soma_pos,
+                    soma_radius,
+                    nrn.soma,
+                ),
+            )
+        except IndexError:
+            logger.warning(
+                f"Neuron {self.neuron_name} has no soma, "
+                "only neurites will be loaded"
+            )
+            self.points = dict(soma=None)
 
         for ntype, nclass in self._neurite_types.items():
             self.points[ntype] = [
                 component(
                     n.points[:, 0],
                     n.points[:, 1],
                     n.points[:, 2],
@@ -203,24 +210,25 @@
         # Render
         if neurites is not None:
             whole_neuron = neurites.pop("whole_neuron")
             neurites["soma"].c(soma_color)
         else:
             # Create soma actor
             neurites = {}
-            coords = self.points["soma"].coords
-            if self.invert_dims:
-                coords = coords[[2, 1, 0]]
-
-            soma = Sphere(
-                pos=coords,
-                r=self.points["soma"].radius * soma_radius,
-                c=soma_color,
-            ).compute_normals()
-            neurites["soma"] = soma.clone().c(soma_color)
+            if self.points["soma"] is not None:
+                coords = self.points["soma"].coords
+                if self.invert_dims:
+                    coords = coords[[2, 1, 0]]
+
+                soma = Sphere(
+                    pos=coords,
+                    r=self.points["soma"].radius * soma_radius,
+                    c=soma_color,
+                ).compute_normals()
+                neurites["soma"] = soma.clone().c(soma_color)
 
             # Create neurites actors
             for ntype in self._neurite_types:
                 actors = []
                 for neurite in self.points[ntype]:
                     for section in iter_sections(neurite.component):
                         for child in section.children:
```

### Comparing `morphapi-0.2.4/morphapi/paths_manager.py` & `morphapi-0.2.5/morphapi/paths_manager.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/morphapi/utils/data_io.py` & `morphapi-0.2.5/morphapi/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/morphapi/utils/webqueries.py` & `morphapi-0.2.5/morphapi/utils/webqueries.py`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/morphapi.egg-info/PKG-INFO` & `morphapi-0.2.5/morphapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphapi
-Version: 0.2.4
+Version: 0.2.5
 Summary: A lightweight python package to download neuronal morphologies
 Author-email: Federico Claudi <hello@brainglobe.info>
 License: MIT
 Project-URL: Homepage, https://github.com/brainglobe/morphapi
 Project-URL: Bug Tracker, https://github.com/brainglobe/morphapi/issues
 Project-URL: Documentation, https://github.com/brainglobe/morphapi
 Project-URL: Source Code, https://github.com/brainglobe/morphapi
```

### Comparing `morphapi-0.2.4/morphapi.egg-info/SOURCES.txt` & `morphapi-0.2.5/morphapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morphapi-0.2.4/pyproject.toml` & `morphapi-0.2.5/pyproject.toml`

 * *Files identical despite different names*

