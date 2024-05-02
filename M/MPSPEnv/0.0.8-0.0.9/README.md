# Comparing `tmp/MPSPEnv-0.0.8.tar.gz` & `tmp/MPSPEnv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MPSPEnv-0.0.8.tar", last modified: Fri Feb 23 21:30:00 2024, max compression
+gzip compressed data, was "MPSPEnv-0.0.9.tar", last modified: Sat Feb 24 11:20:35 2024, max compression
```

## Comparing `MPSPEnv-0.0.8.tar` & `MPSPEnv-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-23 21:30:00.781487 MPSPEnv-0.0.8/
--rw-r--r--   0 axelhojmark   (501) staff       (20)       19 2024-01-16 19:28:34.000000 MPSPEnv-0.0.8/MANIFEST.in
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-23 21:30:00.776658 MPSPEnv-0.0.8/MPSPEnv/
--rw-r--r--   0 axelhojmark   (501) staff       (20)       27 2024-01-16 19:28:34.000000 MPSPEnv-0.0.8/MPSPEnv/__init__.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-23 21:30:00.775186 MPSPEnv-0.0.8/MPSPEnv/c/
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-23 21:30:00.780774 MPSPEnv-0.0.8/MPSPEnv/c/src/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     2833 2024-01-17 21:40:27.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/array.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      589 2024-01-17 21:40:30.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/array.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     7131 2024-01-18 09:17:31.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/bay.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      533 2024-01-18 09:12:54.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/bay.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     4379 2024-02-05 17:19:30.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/env.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      541 2024-01-16 19:28:34.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/env.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1522 2024-01-18 09:19:11.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/random.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      229 2024-01-16 19:28:34.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/random.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)      660 2024-01-16 19:28:34.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/sort.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      132 2024-01-16 19:28:34.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/sort.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     5893 2024-01-30 22:33:00.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/transportation_matrix.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      934 2024-01-16 19:28:34.000000 MPSPEnv-0.0.8/MPSPEnv/c/src/transportation_matrix.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1653 2024-02-05 17:20:47.000000 MPSPEnv-0.0.8/MPSPEnv/c_interface.py
--rw-r--r--   0 axelhojmark   (501) staff       (20)     8434 2024-02-23 21:29:25.000000 MPSPEnv-0.0.8/MPSPEnv/env.py
--rw-r--r--   0 axelhojmark   (501) staff       (20)     4922 2024-02-04 21:34:43.000000 MPSPEnv-0.0.8/MPSPEnv/visualizer.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-23 21:30:00.780986 MPSPEnv-0.0.8/MPSPEnv.egg-info/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3800 2024-02-23 21:30:00.000000 MPSPEnv-0.0.8/MPSPEnv.egg-info/PKG-INFO
--rw-r--r--   0 axelhojmark   (501) staff       (20)      552 2024-02-23 21:30:00.000000 MPSPEnv-0.0.8/MPSPEnv.egg-info/SOURCES.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)        1 2024-02-23 21:30:00.000000 MPSPEnv-0.0.8/MPSPEnv.egg-info/dependency_links.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)       31 2024-02-23 21:30:00.000000 MPSPEnv-0.0.8/MPSPEnv.egg-info/requires.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)        8 2024-02-23 21:30:00.000000 MPSPEnv-0.0.8/MPSPEnv.egg-info/top_level.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3800 2024-02-23 21:30:00.781248 MPSPEnv-0.0.8/PKG-INFO
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3410 2024-02-14 10:07:42.000000 MPSPEnv-0.0.8/README.md
--rw-r--r--   0 axelhojmark   (501) staff       (20)       38 2024-02-23 21:30:00.781536 MPSPEnv-0.0.8/setup.cfg
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1065 2024-02-23 21:28:33.000000 MPSPEnv-0.0.8/setup.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-24 11:20:35.134986 MPSPEnv-0.0.9/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       19 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MANIFEST.in
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-24 11:20:35.132253 MPSPEnv-0.0.9/MPSPEnv/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       27 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/__init__.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-24 11:20:35.131425 MPSPEnv-0.0.9/MPSPEnv/c/
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-24 11:20:35.134432 MPSPEnv-0.0.9/MPSPEnv/c/src/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     2833 2024-01-17 21:40:27.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/array.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      589 2024-01-17 21:40:30.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/array.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     7131 2024-01-18 09:17:31.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/bay.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      533 2024-01-18 09:12:54.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/bay.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     4379 2024-02-05 17:19:30.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/env.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      541 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/env.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1522 2024-01-18 09:19:11.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/random.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      229 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/random.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      660 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/sort.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      132 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/sort.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     5893 2024-01-30 22:33:00.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/transportation_matrix.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      934 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/transportation_matrix.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1653 2024-02-05 17:20:47.000000 MPSPEnv-0.0.9/MPSPEnv/c_interface.py
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     8690 2024-02-24 11:18:57.000000 MPSPEnv-0.0.9/MPSPEnv/env.py
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     4922 2024-02-04 21:34:43.000000 MPSPEnv-0.0.9/MPSPEnv/visualizer.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-24 11:20:35.134604 MPSPEnv-0.0.9/MPSPEnv.egg-info/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3800 2024-02-24 11:20:35.000000 MPSPEnv-0.0.9/MPSPEnv.egg-info/PKG-INFO
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      552 2024-02-24 11:20:35.000000 MPSPEnv-0.0.9/MPSPEnv.egg-info/SOURCES.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)        1 2024-02-24 11:20:35.000000 MPSPEnv-0.0.9/MPSPEnv.egg-info/dependency_links.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       31 2024-02-24 11:20:35.000000 MPSPEnv-0.0.9/MPSPEnv.egg-info/requires.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)        8 2024-02-24 11:20:35.000000 MPSPEnv-0.0.9/MPSPEnv.egg-info/top_level.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3800 2024-02-24 11:20:35.134803 MPSPEnv-0.0.9/PKG-INFO
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3410 2024-02-14 10:07:42.000000 MPSPEnv-0.0.9/README.md
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       38 2024-02-24 11:20:35.135032 MPSPEnv-0.0.9/setup.cfg
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1065 2024-02-24 11:20:28.000000 MPSPEnv-0.0.9/setup.py
```

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c/src/array.c` & `MPSPEnv-0.0.9/MPSPEnv/c/src/array.c`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c/src/array.h` & `MPSPEnv-0.0.9/MPSPEnv/c/src/array.h`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c/src/bay.c` & `MPSPEnv-0.0.9/MPSPEnv/c/src/bay.c`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c/src/bay.h` & `MPSPEnv-0.0.9/MPSPEnv/c/src/bay.h`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c/src/env.c` & `MPSPEnv-0.0.9/MPSPEnv/c/src/env.c`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c/src/env.h` & `MPSPEnv-0.0.9/MPSPEnv/c/src/env.h`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c/src/random.c` & `MPSPEnv-0.0.9/MPSPEnv/c/src/random.c`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c/src/sort.c` & `MPSPEnv-0.0.9/MPSPEnv/c/src/sort.c`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c/src/transportation_matrix.c` & `MPSPEnv-0.0.9/MPSPEnv/c/src/transportation_matrix.c`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c/src/transportation_matrix.h` & `MPSPEnv-0.0.9/MPSPEnv/c/src/transportation_matrix.h`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/c_interface.py` & `MPSPEnv-0.0.9/MPSPEnv/c_interface.py`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv/env.py` & `MPSPEnv-0.0.9/MPSPEnv/env.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,15 +178,18 @@
 
         if self.take_first_action:
             self.step(0)
 
         return self._get_observation(), {}
 
     def _get_observation(self):
-        return {"one_hot_bay": self.one_hot_bay, "flat_T": self.flat_T}
+        return {
+            "one_hot_bay": self.one_hot_bay,
+            "flat_T": self.flat_T / (self.R * self.C),  # Normalize to [0, 1]
+        }
 
     def action_masks(self):
         return self._mask.copy()
 
     @property
     def bay(self):
         return self._bay.copy()
@@ -220,14 +223,22 @@
     def __del__(self):
         if self._env is not None:
             warnings.warn(
                 "Env was not closed properly. Please call .close() to avoid memory leaks."
             )
             self.close()
 
+    def __hash__(self):
+        return hash(self.bay.tobytes() + self.flat_T.tobytes())
+
+    def __eq__(self, other):
+        return np.array_equal(self.bay, other.bay) and np.array_equal(
+            self.flat_T, other.flat_T
+        )
+
     def _set_numpy_views(self):
         # The following numpy arrays are views of the underlying C arrays
         # You should always .copy() them before using them
         self._bay = np.ctypeslib.as_array(
             self._env.bay.matrix.values, shape=(self.R, self.C)
         )
         self._T = np.ctypeslib.as_array(
@@ -239,17 +250,14 @@
         self._flat_T = np.ctypeslib.as_array(
             self._env.flat_T_matrix.values, shape=((self.N - 1) * self.N // 2,)
         )
         self._one_hot_bay = np.ctypeslib.as_array(
             self._env.one_hot_bay.values, shape=(self.N - 1, self.R, self.C)
         )
 
-    def _overwride(self, old, new):
-        old[...] = new
-
     def copy(self):
         new_env = Env(
             self.R,
             self.C,
             self.N,
             self.skip_last_port,
             self.take_first_action,
```

### Comparing `MPSPEnv-0.0.8/MPSPEnv/visualizer.py` & `MPSPEnv-0.0.9/MPSPEnv/visualizer.py`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/MPSPEnv.egg-info/PKG-INFO` & `MPSPEnv-0.0.9/MPSPEnv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MPSPEnv
-Version: 0.0.8
+Version: 0.0.9
 Summary: A reinforcement learning environment for the Multi Port Stowage Planning problem
 Author: Axel Højmark
 Author-email: axelhojmark@gmail.com
 Project-URL: Repository, https://github.com/hojmax/MPSPEnv
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: gymnasium
```

### Comparing `MPSPEnv-0.0.8/MPSPEnv.egg-info/SOURCES.txt` & `MPSPEnv-0.0.9/MPSPEnv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/PKG-INFO` & `MPSPEnv-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MPSPEnv
-Version: 0.0.8
+Version: 0.0.9
 Summary: A reinforcement learning environment for the Multi Port Stowage Planning problem
 Author: Axel Højmark
 Author-email: axelhojmark@gmail.com
 Project-URL: Repository, https://github.com/hojmax/MPSPEnv
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: gymnasium
```

### Comparing `MPSPEnv-0.0.8/README.md` & `MPSPEnv-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `MPSPEnv-0.0.8/setup.py` & `MPSPEnv-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MPSPEnv",
-    version="0.0.8",
+    version="0.0.9",
     author="Axel Højmark",
     author_email="axelhojmark@gmail.com",
     description="A reinforcement learning environment for the Multi Port Stowage Planning problem",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[ext_modules],
     packages=["MPSPEnv"],
```

