# Comparing `tmp/lume-base-0.3.2.tar.gz` & `tmp/lume-base-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/lume-base/lume-base/dist/.tmp-bi9ehuwa/lume-base-0.3.2.tar", last modified: Thu Mar 16 21:19:50 2023, max compression
+gzip compressed data, was "/home/runner/work/lume-base/lume-base/dist/.tmp-vcja5quc/lume-base-0.3.3.tar", last modified: Thu May  2 15:24:15 2024, max compression
```

## Comparing `lume-base-0.3.2.tar` & `lume-base-0.3.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:50.000000 lume-base-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-16 21:19:40.000000 lume-base-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-16 21:19:40.000000 lume-base-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-16 21:19:50.000000 lume-base-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-16 21:19:40.000000 lume-base-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/parsers/namelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/parsers/numbers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/serializers/hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/tests/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/tests/files/test_command_wrapper_subclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/tests/serializers/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-03-16 21:19:40.000000 lume-base-0.3.2/lume/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-16 21:19:50.000000 lume-base-0.3.2/lume_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 21:19:40.000000 lume-base-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-16 21:19:50.000000 lume-base-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-16 21:19:40.000000 lume-base-0.3.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-03-16 21:19:40.000000 lume-base-0.3.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:15.000000 lume-base-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 15:24:11.000000 lume-base-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-02 15:24:11.000000 lume-base-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-02 15:24:15.000000 lume-base-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 15:24:11.000000 lume-base-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18071 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/parsers/namelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/parsers/numbers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/serializers/hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/tests/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/tests/files/test_command_wrapper_subclass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/tests/serializers/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-02 15:24:11.000000 lume-base-0.3.3/lume/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 15:24:15.000000 lume-base-0.3.3/lume_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:24:11.000000 lume-base-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 15:24:15.000000 lume-base-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-02 15:24:11.000000 lume-base-0.3.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78254 2024-05-02 15:24:11.000000 lume-base-0.3.3/versioneer.py
```

### Comparing `lume-base-0.3.2/LICENSE` & `lume-base-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/lume/base.py` & `lume-base-0.3.3/lume/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,15 @@
         """
         Get or set the working directory
         """
         return self._workdir
 
     @workdir.setter
     def workdir(self, workdir):
-        workdir = full_path(workdir)
+        workdir = tools.full_path(workdir)
         self.setup_workdir(workdir)
 
 
     def setup_workdir(self, workdir, cleanup=True):
         """
         Set up the work directory if `use_temp_dir` is set.
```

### Comparing `lume-base-0.3.2/lume/parsers/namelist.py` & `lume-base-0.3.3/lume/parsers/namelist.py`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/lume/parsers/numbers.py` & `lume-base-0.3.3/lume/parsers/numbers.py`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/lume/serializers/base.py` & `lume-base-0.3.3/lume/serializers/base.py`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/lume/serializers/hdf5.py` & `lume-base-0.3.3/lume/serializers/hdf5.py`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/lume/tests/conftest.py` & `lume-base-0.3.3/lume/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/lume/tests/files/test_command_wrapper_subclass.py` & `lume-base-0.3.3/lume/tests/files/test_command_wrapper_subclass.py`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/lume/tests/serializers/test_hdf5.py` & `lume-base-0.3.3/lume/tests/serializers/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/lume/tests/test_base.py` & `lume-base-0.3.3/lume/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/lume/tools.py` & `lume-base-0.3.3/lume/tools.py`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/lume_base.egg-info/SOURCES.txt` & `lume-base-0.3.3/lume_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/setup.py` & `lume-base-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `lume-base-0.3.2/versioneer.py` & `lume-base-0.3.3/versioneer.py`

 * *Files identical despite different names*

