# Comparing `tmp/pipemake_utils-0.1.6.tar.gz` & `tmp/pipemake_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pipemake_utils-0.1.6.tar", last modified: Fri Mar  1 21:31:19 2024, max compression
+gzip compressed data, was "dist/pipemake_utils-0.1.7.tar", last modified: Fri Mar  8 00:40:07 2024, max compression
```

## Comparing `pipemake_utils-0.1.6.tar` & `pipemake_utils-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/pipemake_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/pipemake_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/pipemake_utils/filter_gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/pipemake_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/pipemake_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14031 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/pipemake_utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/pipemake_utils/model_category_inds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/pipemake_utils/ped_phenotype_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/pipemake_utils/process_braker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/pipemake_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/pipemake_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/pipemake_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/pipemake_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/pipemake_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/pipemake_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/pipemake_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 21:31:19.000000 pipemake_utils-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-01 21:31:14.000000 pipemake_utils-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/pipemake_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/pipemake_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/pipemake_utils/filter_gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/pipemake_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/pipemake_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14049 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/pipemake_utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/pipemake_utils/model_category_inds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/pipemake_utils/model_pop_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/pipemake_utils/ped_phenotype_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/pipemake_utils/process_braker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/pipemake_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/pipemake_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/pipemake_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/pipemake_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/pipemake_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/pipemake_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/pipemake_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 00:40:07.000000 pipemake_utils-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-08 00:40:01.000000 pipemake_utils-0.1.7/setup.py
```

### Comparing `pipemake_utils-0.1.6/pipemake_utils/filter_gemma.py` & `pipemake_utils-0.1.7/pipemake_utils/filter_gemma.py`

 * *Files identical despite different names*

### Comparing `pipemake_utils-0.1.6/pipemake_utils/logger.py` & `pipemake_utils-0.1.7/pipemake_utils/logger.py`

 * *Files identical despite different names*

### Comparing `pipemake_utils-0.1.6/pipemake_utils/model.py` & `pipemake_utils-0.1.7/pipemake_utils/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,16 +277,17 @@
             sampled_inds = np.random.choice(self.ind_dict[pop], sample_size, replace = with_replacements)
 
             # Save the sampled inds as a list
             self.ind_dict[pop] = list(sampled_inds)
 
     def create_pop_files (self, file_ext = '', file_path = '', overwrite = False):
         for pop in self.pop_list:
+            
             # Assign the filename for the population file
-            pop_filename = pop + file_ext
+            pop_filename = f'{pop}.{file_ext}'
 
             # If a path is assigned, create the file at the specified location
             if file_path:
                 pop_filename = os.path.join(file_path, pop_filename)
 
             # Check if previous files should be overwriten
             if not overwrite:
```

### Comparing `pipemake_utils-0.1.6/pipemake_utils/model_category_inds.py` & `pipemake_utils-0.1.7/pipemake_utils/model_category_inds.py`

 * *Files identical despite different names*

### Comparing `pipemake_utils-0.1.6/pipemake_utils/ped_phenotype_file.py` & `pipemake_utils-0.1.7/pipemake_utils/ped_phenotype_file.py`

 * *Files identical despite different names*

### Comparing `pipemake_utils-0.1.6/pipemake_utils/process_braker.py` & `pipemake_utils-0.1.7/pipemake_utils/process_braker.py`

 * *Files identical despite different names*

### Comparing `pipemake_utils-0.1.6/pipemake_utils.egg-info/SOURCES.txt` & `pipemake_utils-0.1.7/pipemake_utils.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 pipemake_utils/__init__.py
 pipemake_utils/filter_gemma.py
 pipemake_utils/logger.py
 pipemake_utils/misc.py
 pipemake_utils/model.py
 pipemake_utils/model_category_inds.py
+pipemake_utils/model_pop_files.py
 pipemake_utils/ped_phenotype_file.py
 pipemake_utils/process_braker.py
 pipemake_utils.egg-info/PKG-INFO
 pipemake_utils.egg-info/SOURCES.txt
 pipemake_utils.egg-info/dependency_links.txt
 pipemake_utils.egg-info/entry_points.txt
 pipemake_utils.egg-info/requires.txt
```

### Comparing `pipemake_utils-0.1.6/setup.py` & `pipemake_utils-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,12 +32,13 @@
     packages=["pipemake_utils"],
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "process-braker=pipemake_utils.process_braker:main",
             "ped-phenotype-file=pipemake_utils.ped_phenotype_file:main",
             "model-category-inds = pipemake_utils.model_category_inds:main",
-            "filter-gemma = pipemake_utils.filter_gemma:main"
+            "filter-gemma = pipemake_utils.filter_gemma:main",
+            "model-pop-files = pipemake_utils.model_pop_files:main"
         ],
     },
     python_requires=">=3.7",
 )
```

