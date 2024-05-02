# Comparing `tmp/dicomthings-0.7.1.tar.gz` & `tmp/dicomthings-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomthings-0.7.1.tar", last modified: Tue Apr 30 09:47:13 2024, max compression
+gzip compressed data, was "dicomthings-0.8.0.tar", last modified: Thu May  2 13:39:44 2024, max compression
```

## Comparing `dicomthings-0.7.1.tar` & `dicomthings-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2024-04-30 09:47:13.424729 dicomthings-0.7.1/
--rw-r--r--   0 jeroenbertels   (501) staff       (20)    11357 2023-11-03 13:41:14.000000 dicomthings-0.7.1/LICENSE
--rw-r--r--   0 jeroenbertels   (501) staff       (20)      567 2024-04-30 09:47:13.424547 dicomthings-0.7.1/PKG-INFO
--rw-r--r--   0 jeroenbertels   (501) staff       (20)       61 2023-11-06 08:08:03.000000 dicomthings-0.7.1/README.md
-drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2024-04-30 09:47:13.423462 dicomthings-0.7.1/dicomthings/
--rw-r--r--   0 jeroenbertels   (501) staff       (20)        0 2023-11-13 11:07:07.000000 dicomthings-0.7.1/dicomthings/__init__.py
--rw-r--r--   0 jeroenbertels   (501) staff       (20)     8650 2023-12-11 12:28:36.000000 dicomthings-0.7.1/dicomthings/array.py
--rw-r--r--   0 jeroenbertels   (501) staff       (20)    15233 2023-11-14 12:59:40.000000 dicomthings-0.7.1/dicomthings/dicom.py
--rw-r--r--   0 jeroenbertels   (501) staff       (20)     4954 2024-04-30 09:44:56.000000 dicomthings-0.7.1/dicomthings/nifti.py
--rw-r--r--   0 jeroenbertels   (501) staff       (20)     2265 2023-11-22 10:02:41.000000 dicomthings-0.7.1/dicomthings/utils.py
-drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2024-04-30 09:47:13.424344 dicomthings-0.7.1/dicomthings.egg-info/
--rw-r--r--   0 jeroenbertels   (501) staff       (20)      567 2024-04-30 09:47:13.000000 dicomthings-0.7.1/dicomthings.egg-info/PKG-INFO
--rw-r--r--   0 jeroenbertels   (501) staff       (20)      314 2024-04-30 09:47:13.000000 dicomthings-0.7.1/dicomthings.egg-info/SOURCES.txt
--rw-r--r--   0 jeroenbertels   (501) staff       (20)        1 2024-04-30 09:47:13.000000 dicomthings-0.7.1/dicomthings.egg-info/dependency_links.txt
--rw-r--r--   0 jeroenbertels   (501) staff       (20)       12 2024-04-30 09:47:13.000000 dicomthings-0.7.1/dicomthings.egg-info/requires.txt
--rw-r--r--   0 jeroenbertels   (501) staff       (20)       12 2024-04-30 09:47:13.000000 dicomthings-0.7.1/dicomthings.egg-info/top_level.txt
--rw-r--r--   0 jeroenbertels   (501) staff       (20)      665 2024-04-30 09:45:16.000000 dicomthings-0.7.1/pyproject.toml
--rw-r--r--   0 jeroenbertels   (501) staff       (20)       38 2024-04-30 09:47:13.424772 dicomthings-0.7.1/setup.cfg
+drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2024-05-02 13:39:44.454201 dicomthings-0.8.0/
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)    11357 2023-11-03 13:41:14.000000 dicomthings-0.8.0/LICENSE
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)      567 2024-05-02 13:39:44.454019 dicomthings-0.8.0/PKG-INFO
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)       61 2023-11-06 08:08:03.000000 dicomthings-0.8.0/README.md
+drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2024-05-02 13:39:44.452932 dicomthings-0.8.0/dicomthings/
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)        0 2023-11-13 11:07:07.000000 dicomthings-0.8.0/dicomthings/__init__.py
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)     8650 2023-12-11 12:28:36.000000 dicomthings-0.8.0/dicomthings/array.py
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)    15395 2024-05-02 13:38:47.000000 dicomthings-0.8.0/dicomthings/dicom.py
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)     4954 2024-04-30 09:44:56.000000 dicomthings-0.8.0/dicomthings/nifti.py
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)     2265 2023-11-22 10:02:41.000000 dicomthings-0.8.0/dicomthings/utils.py
+drwxr-xr-x   0 jeroenbertels   (501) staff       (20)        0 2024-05-02 13:39:44.453810 dicomthings-0.8.0/dicomthings.egg-info/
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)      567 2024-05-02 13:39:44.000000 dicomthings-0.8.0/dicomthings.egg-info/PKG-INFO
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)      314 2024-05-02 13:39:44.000000 dicomthings-0.8.0/dicomthings.egg-info/SOURCES.txt
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)        1 2024-05-02 13:39:44.000000 dicomthings-0.8.0/dicomthings.egg-info/dependency_links.txt
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)       12 2024-05-02 13:39:44.000000 dicomthings-0.8.0/dicomthings.egg-info/requires.txt
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)       12 2024-05-02 13:39:44.000000 dicomthings-0.8.0/dicomthings.egg-info/top_level.txt
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)      665 2024-04-30 09:45:16.000000 dicomthings-0.8.0/pyproject.toml
+-rw-r--r--   0 jeroenbertels   (501) staff       (20)       38 2024-05-02 13:39:44.454248 dicomthings-0.8.0/setup.cfg
```

### Comparing `dicomthings-0.7.1/LICENSE` & `dicomthings-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dicomthings-0.7.1/PKG-INFO` & `dicomthings-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicomthings
-Version: 0.7.1
+Version: 0.8.0
 Summary: A Python library for working with DICOM files.
 Author-email: Jeroen Bertels <jeroen.bertels@gmail.com>
 Project-URL: Homepage, https://github.com/JeroenBertels/dicomthings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `dicomthings-0.7.1/dicomthings/array.py` & `dicomthings-0.8.0/dicomthings/array.py`

 * *Files identical despite different names*

### Comparing `dicomthings-0.7.1/dicomthings/dicom.py` & `dicomthings-0.8.0/dicomthings/dicom.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,17 @@
         else:
             self.dicom.save_as(file_path)
 
         new_dicom_file = DicomFile(self)  
         new_dicom_file.file_path = file_path          
         return new_dicom_file
 
+    def get(self, tag):
+        return getattr(self, tag, self.dicom.get(tag, None))
+
     def get_datetime_file(self, tags=["Series", "Acquisition", "InstanceCreation", "Content"]):
         for tag in tags:
             try:
                 date = str(self.dicom[tag + "Date"].value)
                 time = str(self.dicom[tag + "Time"].value)
                 format = "%Y%m%d_%H%M%S.%f" if "." in time else "%Y%m%d_%H%M%S"
                 return datetime.strptime(f"{date}_{time}", format)
@@ -119,15 +122,19 @@
             self.dicom.PatientName = new_patient_id
 
         if remove_private_tags:
             self.dicom.remove_private_tags()
 
         if file_path is not None:
             self.write_dicom_file(file_path)
-
+    
+    @property
+    def orientation(self):
+        return self.get_orientation()
+    
     def get_orientation(self):  # https://stackoverflow.com/questions/70645577/translate-image-orientation-into-axial-sagittal-or-coronal-plane
         return DicomFile.image_ori_to_str(self.dicom.ImageOrientationPatient)
 
     @staticmethod
     def image_ori_to_str(image_ori):
         if image_ori is None:
             return 
@@ -268,15 +275,15 @@
         if not self.is_sorted_into_series():
             print("WARNING: This dicom directory is not sorted into series!")
 
     def sort(self, tags, remove_duplicates=False):
         sorted_directory = DicomDirectory()
         for subdir in self:
             for dicom_file in self[subdir]:
-                sorted_subdir = os.sep.join([str(dicom_file.dicom.get(tag, None)) for tag in tags])
+                sorted_subdir = os.sep.join([str(dicom_file.get(tag)) for tag in tags])
                 sorted_directory[sorted_subdir] = sorted_directory.get(sorted_subdir, []) + [dicom_file]
         
         if remove_duplicates:
             for subdir in sorted_directory:
                 filtered_subdir = []
                 for dicom_file in sorted_directory[subdir]:
                     if not any([filecmp.cmp(dicom_file.file_path, dicom_file_.file_path, shallow=False) for dicom_file_ in filtered_subdir]):
```

### Comparing `dicomthings-0.7.1/dicomthings/nifti.py` & `dicomthings-0.8.0/dicomthings/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomthings-0.7.1/dicomthings/utils.py` & `dicomthings-0.8.0/dicomthings/utils.py`

 * *Files identical despite different names*

### Comparing `dicomthings-0.7.1/dicomthings.egg-info/PKG-INFO` & `dicomthings-0.8.0/dicomthings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicomthings
-Version: 0.7.1
+Version: 0.8.0
 Summary: A Python library for working with DICOM files.
 Author-email: Jeroen Bertels <jeroen.bertels@gmail.com>
 Project-URL: Homepage, https://github.com/JeroenBertels/dicomthings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `dicomthings-0.7.1/pyproject.toml` & `dicomthings-0.8.0/pyproject.toml`

 * *Files identical despite different names*

