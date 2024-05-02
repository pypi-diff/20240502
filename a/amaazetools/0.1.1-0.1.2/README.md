# Comparing `tmp/amaazetools-0.1.1.tar.gz` & `tmp/amaazetools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amaazetools-0.1.1.tar", last modified: Wed Dec 20 04:35:15 2023, max compression
+gzip compressed data, was "amaazetools-0.1.2.tar", last modified: Thu May  2 00:22:08 2024, max compression
```

## Comparing `amaazetools-0.1.1.tar` & `amaazetools-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 04:35:15.567490 amaazetools-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-20 04:34:55.000000 amaazetools-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-20 04:34:55.000000 amaazetools-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-12-20 04:35:15.563490 amaazetools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-12-20 04:34:55.000000 amaazetools-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 04:35:15.563490 amaazetools-0.1.1/amaazetools/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 04:34:55.000000 amaazetools-0.1.1/amaazetools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25709 2023-12-20 04:34:55.000000 amaazetools-0.1.1/amaazetools/dicom.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6860 2023-12-20 04:34:55.000000 amaazetools-0.1.1/amaazetools/edge_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2023-12-20 04:34:55.000000 amaazetools-0.1.1/amaazetools/mesh_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2023-12-20 04:34:55.000000 amaazetools-0.1.1/amaazetools/svi.py
--rw-r--r--   0 runner    (1001) docker     (127)    41172 2023-12-20 04:34:55.000000 amaazetools-0.1.1/amaazetools/trimesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 04:35:15.563490 amaazetools-0.1.1/amaazetools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-12-20 04:35:15.000000 amaazetools-0.1.1/amaazetools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-12-20 04:35:15.000000 amaazetools-0.1.1/amaazetools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 04:35:15.000000 amaazetools-0.1.1/amaazetools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-20 04:35:15.000000 amaazetools-0.1.1/amaazetools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-20 04:35:15.000000 amaazetools-0.1.1/amaazetools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-12-20 04:34:55.000000 amaazetools-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 04:35:15.567490 amaazetools-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-20 04:34:55.000000 amaazetools-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 04:35:15.563490 amaazetools-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2023-12-20 04:34:55.000000 amaazetools-0.1.1/src/cextensions.c
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2023-12-20 04:34:55.000000 amaazetools-0.1.1/src/memory_allocation.c
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-20 04:34:55.000000 amaazetools-0.1.1/src/memory_allocation.h
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2023-12-20 04:34:55.000000 amaazetools-0.1.1/src/mesh_operations.c
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-12-20 04:34:55.000000 amaazetools-0.1.1/src/mesh_operations.h
--rw-r--r--   0 runner    (1001) docker     (127)    18102 2023-12-20 04:34:55.000000 amaazetools-0.1.1/src/svi_computations.c
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2023-12-20 04:34:55.000000 amaazetools-0.1.1/src/svi_computations.h
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2023-12-20 04:34:55.000000 amaazetools-0.1.1/src/vector_operations.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-02 00:22:08.988533 amaazetools-0.1.2/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-02 00:22:01.000000 amaazetools-0.1.2/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       10 2024-05-02 00:22:01.000000 amaazetools-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     1707 2024-05-02 00:22:08.988358 amaazetools-0.1.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      935 2024-05-02 00:22:01.000000 amaazetools-0.1.2/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-02 00:22:08.986239 amaazetools-0.1.2/amaazetools/
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-02 00:22:01.000000 amaazetools-0.1.2/amaazetools/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    28162 2024-05-02 00:22:01.000000 amaazetools-0.1.2/amaazetools/dicom.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6860 2024-05-02 00:22:01.000000 amaazetools-0.1.2/amaazetools/edge_detection.py
+-rw-r--r--   0 runner     (501) staff       (20)     9073 2024-05-02 00:22:01.000000 amaazetools-0.1.2/amaazetools/mesh_segmentation.py
+-rw-r--r--   0 runner     (501) staff       (20)     9193 2024-05-02 00:22:01.000000 amaazetools-0.1.2/amaazetools/svi.py
+-rw-r--r--   0 runner     (501) staff       (20)    41172 2024-05-02 00:22:01.000000 amaazetools-0.1.2/amaazetools/trimesh.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-02 00:22:08.988096 amaazetools-0.1.2/amaazetools.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1707 2024-05-02 00:22:08.000000 amaazetools-0.1.2/amaazetools.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      557 2024-05-02 00:22:08.000000 amaazetools-0.1.2/amaazetools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-02 00:22:08.000000 amaazetools-0.1.2/amaazetools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       86 2024-05-02 00:22:08.000000 amaazetools-0.1.2/amaazetools.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       12 2024-05-02 00:22:08.000000 amaazetools-0.1.2/amaazetools.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      942 2024-05-02 00:22:01.000000 amaazetools-0.1.2/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-02 00:22:08.988565 amaazetools-0.1.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      581 2024-05-02 00:22:01.000000 amaazetools-0.1.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-02 00:22:08.987941 amaazetools-0.1.2/src/
+-rw-r--r--   0 runner     (501) staff       (20)     3003 2024-05-02 00:22:01.000000 amaazetools-0.1.2/src/cextensions.c
+-rw-r--r--   0 runner     (501) staff       (20)     1602 2024-05-02 00:22:01.000000 amaazetools-0.1.2/src/memory_allocation.c
+-rw-r--r--   0 runner     (501) staff       (20)      336 2024-05-02 00:22:01.000000 amaazetools-0.1.2/src/memory_allocation.h
+-rw-r--r--   0 runner     (501) staff       (20)    14431 2024-05-02 00:22:01.000000 amaazetools-0.1.2/src/mesh_operations.c
+-rw-r--r--   0 runner     (501) staff       (20)     1268 2024-05-02 00:22:01.000000 amaazetools-0.1.2/src/mesh_operations.h
+-rw-r--r--   0 runner     (501) staff       (20)    18102 2024-05-02 00:22:01.000000 amaazetools-0.1.2/src/svi_computations.c
+-rw-r--r--   0 runner     (501) staff       (20)     1375 2024-05-02 00:22:01.000000 amaazetools-0.1.2/src/svi_computations.h
+-rw-r--r--   0 runner     (501) staff       (20)     1385 2024-05-02 00:22:01.000000 amaazetools-0.1.2/src/vector_operations.h
```

### Comparing `amaazetools-0.1.1/LICENSE` & `amaazetools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/PKG-INFO` & `amaazetools-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amaazetools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for mesh processing tools developed by AMAAZE
 Author-email: Jeff Calder <jwcalder@umn.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcalder/AMAAZETools
 Project-URL: Bug Tracker, https://github.com/jwcalder/AMAAZETools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `amaazetools-0.1.1/README.md` & `amaazetools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/amaazetools/dicom.py` & `amaazetools-0.1.2/amaazetools/dicom.py`

 * *Files 5% similar despite different names*

```diff
@@ -865,7 +865,80 @@
     M = M[u>0,:]
     M = M[:,u>0]
     X = X[u>0]
     Y = Y[u>0]
 
     return M,X,Y
 
+
+def surfacing_subproc(filename,directory,iso_level,write_gif=False):
+    
+    print('Loading '+filename+'...')
+    M = np.load(os.path.join(directory,filename))
+    I = M['I']; dx = M['dx']; dz = M['dz']
+    
+    #Rescale image to account for different dx/dz dimensions
+    J = rescale(I.astype(float),(dz/dx,1,1),mode='constant')
+    
+    try: 
+        verts,faces,normals,values = measure.marching_cubes(J,iso_level)
+        mesh = tm.mesh(dx*verts,faces) #Multiplication by dx fixes units
+    
+        #Reverse orientation of triangles (marching_cubes returns inward normals)
+        mesh.flip_normals()
+    
+        #Write to ply file
+        mesh_filename = os.path.join(directory,filename[:-4]+'_iso%d'%iso_level)
+        print('Saving mesh to '+mesh_filename+'...')
+        mesh.to_ply(mesh_filename+'.ply')
+    
+        if write_gif:
+            mesh.to_gif(mesh_filename+'.gif')
+        return '0'
+    except Exception as error:
+        print('surfacing error with ', filename, ': ', error)
+        return filename
+
+
+
+def surface_bones_parallel(directory, iso=2500, write_gif=False,error_fname='./surfacing_errors.csv',ncores='all'):
+    """ parallelized implementation of surface_bones with also surfacing error support.
+        Processes all npz files in directory creating surface and saving to a ply file.
+
+        Parameters
+        ----------
+        directory : str
+            Directory to work within.
+        iso : float (optional), default is 2500
+            Iso level to be used for surfacing.
+        write_gif : bool (optional), default=False
+            Whether to output rotating gifs for each object. Requires mayavi, which can be hard to install.
+        error_fname
+
+        Returns
+        -------
+        None
+    """
+    
+    ddd = os.listdir(directory)
+    
+    fnames = []
+    for f in ddd:
+        if f.endswith('.npz'):
+            fnames.append(f)
+    
+        
+    if isinstance(ncores,int):
+        num_cores = ncores
+    else: 
+        num_cores =multiprocessing.cpu_count()
+        
+    errs = Parallel(n_jobs=num_cores)(delayed(surfacing_subproc)(f,directory,iso,write_gif) for f in fnames)
+    
+    errs = np.array(errs)
+    errs = errs[errs!='0']
+    
+    if len(errs)==0:
+        print('no errors, not saving an error csv.')
+    else:
+        print('there were ' + str(len(errs)) +' errors. saving CSV to ',error_fname)              
+        pd.DataFrame(errs).to_csv(error_fname,header=False, index=False)
```

### Comparing `amaazetools-0.1.1/amaazetools/edge_detection.py` & `amaazetools-0.1.2/amaazetools/edge_detection.py`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/amaazetools/mesh_segmentation.py` & `amaazetools-0.1.2/amaazetools/mesh_segmentation.py`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/amaazetools/svi.py` & `amaazetools-0.1.2/amaazetools/svi.py`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/amaazetools/trimesh.py` & `amaazetools-0.1.2/amaazetools/trimesh.py`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/amaazetools.egg-info/PKG-INFO` & `amaazetools-0.1.2/amaazetools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amaazetools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for mesh processing tools developed by AMAAZE
 Author-email: Jeff Calder <jwcalder@umn.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcalder/AMAAZETools
 Project-URL: Bug Tracker, https://github.com/jwcalder/AMAAZETools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `amaazetools-0.1.1/amaazetools.egg-info/SOURCES.txt` & `amaazetools-0.1.2/amaazetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/pyproject.toml` & `amaazetools-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [tool.setuptools]
 packages = ['amaazetools']
 
 
 [project]
 name = "amaazetools"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Jeff Calder", email="jwcalder@umn.edu" },
 ]
 description = "Python package for mesh processing tools developed by AMAAZE"
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.6"
```

### Comparing `amaazetools-0.1.1/setup.py` & `amaazetools-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/src/cextensions.c` & `amaazetools-0.1.2/src/cextensions.c`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/src/memory_allocation.c` & `amaazetools-0.1.2/src/memory_allocation.c`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/src/mesh_operations.c` & `amaazetools-0.1.2/src/mesh_operations.c`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/src/mesh_operations.h` & `amaazetools-0.1.2/src/mesh_operations.h`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/src/svi_computations.c` & `amaazetools-0.1.2/src/svi_computations.c`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/src/svi_computations.h` & `amaazetools-0.1.2/src/svi_computations.h`

 * *Files identical despite different names*

### Comparing `amaazetools-0.1.1/src/vector_operations.h` & `amaazetools-0.1.2/src/vector_operations.h`

 * *Files identical despite different names*

