# Comparing `tmp/p4cmd-2.4.8.tar.gz` & `tmp/p4cmd-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p4cmd-2.4.8.tar", last modified: Wed Mar 13 08:55:10 2024, max compression
+gzip compressed data, was "p4cmd-2.4.9.tar", last modified: Thu May  2 12:07:23 2024, max compression
```

## Comparing `p4cmd-2.4.8.tar` & `p4cmd-2.4.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:55:10.338529 p4cmd-2.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-13 08:55:06.000000 p4cmd-2.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-03-13 08:55:10.338529 p4cmd-2.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-03-13 08:55:06.000000 p4cmd-2.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:55:10.334529 p4cmd-2.4.8/p4cmd/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42460 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/p4cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/p4errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/p4file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:55:10.338529 p4cmd-2.4.8/p4cmd/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/resources/perforce_DEPOT_ONLY.png
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/resources/perforce_MOVED.png
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/resources/perforce_NEED_SYNC.png
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/resources/perforce_OPEN_FOR_ADD.png
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/resources/perforce_OPEN_FOR_DELETE.png
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/resources/perforce_OPEN_FOR_EDIT.png
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/resources/perforce_UNKNOWN.png
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/resources/perforce_UNTRACKED.png
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-03-13 08:55:06.000000 p4cmd-2.4.8/p4cmd/resources/perforce_UP_TO_DATE.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:55:10.338529 p4cmd-2.4.8/p4cmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-03-13 08:55:10.000000 p4cmd-2.4.8/p4cmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-13 08:55:10.000000 p4cmd-2.4.8/p4cmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 08:55:10.000000 p4cmd-2.4.8/p4cmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 08:55:10.000000 p4cmd-2.4.8/p4cmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 08:55:10.338529 p4cmd-2.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-13 08:55:06.000000 p4cmd-2.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:23.187324 p4cmd-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 12:07:19.000000 p4cmd-2.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-02 12:07:23.187324 p4cmd-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-02 12:07:19.000000 p4cmd-2.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:23.183324 p4cmd-2.4.9/p4cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42460 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/p4cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/p4errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/p4file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:23.187324 p4cmd-2.4.9/p4cmd/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/resources/perforce_DEPOT_ONLY.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/resources/perforce_MOVED.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/resources/perforce_NEED_SYNC.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/resources/perforce_OPEN_FOR_ADD.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/resources/perforce_OPEN_FOR_DELETE.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/resources/perforce_OPEN_FOR_EDIT.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/resources/perforce_UNKNOWN.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/resources/perforce_UNTRACKED.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-02 12:07:19.000000 p4cmd-2.4.9/p4cmd/resources/perforce_UP_TO_DATE.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:23.187324 p4cmd-2.4.9/p4cmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-02 12:07:23.000000 p4cmd-2.4.9/p4cmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-02 12:07:23.000000 p4cmd-2.4.9/p4cmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:07:23.000000 p4cmd-2.4.9/p4cmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 12:07:23.000000 p4cmd-2.4.9/p4cmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:07:23.187324 p4cmd-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-02 12:07:19.000000 p4cmd-2.4.9/setup.py
```

### Comparing `p4cmd-2.4.8/LICENSE` & `p4cmd-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/PKG-INFO` & `p4cmd-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4cmd
-Version: 2.4.8
+Version: 2.4.9
 Summary: Simple P4 python module
 Home-page: https://github.com/nielsvaes/p4cmd
 Author: Niels Vaes
 Author-email: nielsvaes@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `p4cmd-2.4.8/README.md` & `p4cmd-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/p4cmd.py` & `p4cmd-2.4.9/p4cmd/p4cmd.py`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/p4file.py` & `p4cmd-2.4.9/p4cmd/p4file.py`

 * *Files 9% similar despite different names*

```diff
@@ -207,8 +207,23 @@
             value = None
         self.__have_revision = value
 
     def get_last_submitted_by(self):
         return self.__last_submitted_by
 
     def set_last_submitted_by(self, value):
-        self.__last_submitted_by = value
+        self.__last_submitted_by = value
+
+    def __eq__(self, other):
+        if not isinstance(other, P4File):
+            return NotImplemented
+
+        private_attributes = [
+            '_P4File__local_file_path', '_P4File__depot_file_path', '_P4File__last_submitted_by',
+            '_P4File__have_revision', '_P4File__head_revision', '_P4File__checked_out_by',
+            '_P4File__last_submit_time', '_P4File__action', '_P4File__raw_data', '_P4File__head_action'
+        ]
+
+        for attr in private_attributes:
+            if getattr(self, attr) != getattr(other, attr):
+                return False
+        return True
```

### Comparing `p4cmd-2.4.8/p4cmd/resources/__init__.py` & `p4cmd-2.4.9/p4cmd/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/resources/perforce_DEPOT_ONLY.png` & `p4cmd-2.4.9/p4cmd/resources/perforce_DEPOT_ONLY.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/resources/perforce_MOVED.png` & `p4cmd-2.4.9/p4cmd/resources/perforce_MOVED.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/resources/perforce_NEED_SYNC.png` & `p4cmd-2.4.9/p4cmd/resources/perforce_NEED_SYNC.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/resources/perforce_OPEN_FOR_ADD.png` & `p4cmd-2.4.9/p4cmd/resources/perforce_OPEN_FOR_ADD.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/resources/perforce_OPEN_FOR_DELETE.png` & `p4cmd-2.4.9/p4cmd/resources/perforce_OPEN_FOR_DELETE.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/resources/perforce_OPEN_FOR_EDIT.png` & `p4cmd-2.4.9/p4cmd/resources/perforce_OPEN_FOR_EDIT.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/resources/perforce_UNKNOWN.png` & `p4cmd-2.4.9/p4cmd/resources/perforce_UNKNOWN.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/resources/perforce_UNTRACKED.png` & `p4cmd-2.4.9/p4cmd/resources/perforce_UNTRACKED.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd/resources/perforce_UP_TO_DATE.png` & `p4cmd-2.4.9/p4cmd/resources/perforce_UP_TO_DATE.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/p4cmd.egg-info/PKG-INFO` & `p4cmd-2.4.9/p4cmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4cmd
-Version: 2.4.8
+Version: 2.4.9
 Summary: Simple P4 python module
 Home-page: https://github.com/nielsvaes/p4cmd
 Author: Niels Vaes
 Author-email: nielsvaes@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `p4cmd-2.4.8/p4cmd.egg-info/SOURCES.txt` & `p4cmd-2.4.9/p4cmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p4cmd-2.4.8/setup.py` & `p4cmd-2.4.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 data_files_to_include = ["*.png"]
 
 setuptools.setup(
     name="p4cmd",
-    version="2.4.8",
+    version="2.4.9",
     author="Niels Vaes",
     license='MIT',
     author_email="nielsvaes@gmail.com",
     description="Simple P4 python module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nielsvaes/p4cmd",
```

