# Comparing `tmp/neurocaps-0.8.8.post4.tar.gz` & `tmp/neurocaps-0.8.8.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.8.8.post4.tar", last modified: Wed Apr 24 02:00:18 2024, max compression
+gzip compressed data, was "neurocaps-0.8.8.post5.tar", last modified: Thu May  2 16:14:20 2024, max compression
```

## Comparing `neurocaps-0.8.8.post4.tar` & `neurocaps-0.8.8.post5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/LICENSE.md
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    12235 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    11310 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/README.md
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps/_utils/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_cap_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_cap_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2227 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_check_confound_names.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2901 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6126 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2405 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/neurocaps/analysis/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       85 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/analysis/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    44374 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/analysis/cap.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4697 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/analysis/merge.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/neurocaps/extraction/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/extraction/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    20113 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/extraction/timeseriesextractor.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    12235 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      956 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/SOURCES.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/dependency_links.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       94 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/requires.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/top_level.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1240 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/pyproject.toml
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/setup.cfg
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/tests/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-04-24 01:37:41.000000 neurocaps-0.8.8.post4/tests/test_CAP.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1005 2024-04-24 01:37:41.000000 neurocaps-0.8.8.post4/tests/test_TimeseriesExtractor.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-04-24 01:37:41.000000 neurocaps-0.8.8.post4/tests/test_merge_dicts.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/LICENSE.md
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    12235 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    11310 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/README.md
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/_utils/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_cap_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_cap_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2227 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_check_confound_names.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2901 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6324 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2405 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/analysis/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       85 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/analysis/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    44374 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/analysis/cap.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4697 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/analysis/merge.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps/extraction/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/extraction/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    22479 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/neurocaps/extraction/timeseriesextractor.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    12235 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1001 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/SOURCES.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/dependency_links.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       94 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/requires.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/neurocaps.egg-info/top_level.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1240 2024-05-02 16:12:49.000000 neurocaps-0.8.8.post5/pyproject.toml
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/setup.cfg
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-02 16:14:20.000000 neurocaps-0.8.8.post5/tests/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-02 16:12:50.000000 neurocaps-0.8.8.post5/tests/test_CAP.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1864 2024-05-02 16:12:50.000000 neurocaps-0.8.8.post5/tests/test_TimeseriesExtractor.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1045 2024-05-02 16:12:50.000000 neurocaps-0.8.8.post5/tests/test_TimeseriesExtractor_additional.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-02 16:12:50.000000 neurocaps-0.8.8.post5/tests/test_merge_dicts.py
```

### Comparing `neurocaps-0.8.8.post4/LICENSE.md` & `neurocaps-0.8.8.post5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post4/PKG-INFO` & `neurocaps-0.8.8.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.8.8.post4
+Version: 0.8.8.post5
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `neurocaps-0.8.8.post4/README.md` & `neurocaps-0.8.8.post5/README.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post4/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.8.8.post5/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post4/neurocaps/_utils/_check_confound_names.py` & `neurocaps-0.8.8.post5/neurocaps/_utils/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 def _extract_timeseries(subj_id, nifti_files, mask_files, event_files, confound_files, confound_metadata_files, run_list, tr, condition, parcel_approach, signal_clean_info, verbose, flush_print):
 
     from nilearn.maskers import NiftiLabelsMasker
     from nilearn.image import index_img, load_img
-    import pandas as pd, json, math, copy, warnings
+    import pandas as pd, json, math, numpy as np, copy, warnings
 
     # Intitialize subject dictionary
     subject_timeseries = {subj_id: {}}
     
     for run in run_list:
 
+        run_id = "run-1" if run == None else run
+        run = run if run != None else ""
+
         # Get files from specific run
-        nifti_file = [nifti_file for nifti_file in nifti_files if run in nifti_file]
-        mask_file = [mask_file for mask_file in mask_files if run in mask_file]
-        confound_file = [confound_file for confound_file in confound_files if run in confound_file] if signal_clean_info["use_confounds"] else None
-        confound_metadata_file = [confound_metadata_file for confound_metadata_file in confound_metadata_files if run in confound_metadata_file] if signal_clean_info["use_confounds"] and signal_clean_info["n_acompcor_separate"] else None
+        nifti_file = [nifti_file for nifti_file in nifti_files if run in nifti_file.split("/")[-1]]
+        mask_file = [mask_file for mask_file in mask_files if run in mask_file.split("/")[-1]]
+        confound_file = [confound_file for confound_file in confound_files if run in confound_file.split("/")[-1]] if signal_clean_info["use_confounds"] else None
+        confound_metadata_file = [confound_metadata_file for confound_metadata_file in confound_metadata_files if run in confound_metadata_file.split("/")[-1]] if signal_clean_info["use_confounds"] and signal_clean_info["n_acompcor_separate"] else None
 
-        if verbose: print(f"Running subject: {subj_id}; {run}; \n {nifti_file}", flush=flush_print)
+        if verbose: print(f"Running subject: {subj_id}; run: {run_id}; \n {nifti_file}", flush=flush_print)
 
         confound_df = pd.read_csv(confound_file[0], sep="\t") if signal_clean_info["use_confounds"] else None
 
-        event_file = None if len(event_files) == 0 else [event_file for event_file in event_files if run in event_file]
+        event_file = None if len(event_files) == 0 else [event_file for event_file in event_files if run in event_file.split("/")[-1]]
 
         # Extract confound information of interest and ensure confound file does not contain NAs
         if signal_clean_info["use_confounds"]:
             # Extract first "n" numbers of specified WM and CSF components
             confound_names = copy.deepcopy(signal_clean_info["confound_names"])
             if confound_metadata_file:
                 with open(confound_metadata_file[0]) as foo:
@@ -49,15 +52,15 @@
                 else: invalid_confounds.extend([confound_name])
 
             if len(invalid_confounds) > 0: 
                 if verbose: print(f"Subject {subj_id} did not have the following confounds: {invalid_confounds}", flush=flush_print)
 
             confounds = confound_df[valid_confounds]
             confounds = confounds.fillna(0)
-            if verbose: print(f"Confounds used for subject: {subj_id}; {run} - {confounds.columns}", flush=flush_print)
+            if verbose: print(f"Confounds used for subject: {subj_id}; run: {run_id} - {confounds.columns}", flush=flush_print)
 
         # Create the masker for extracting time series
         masker = NiftiLabelsMasker(
             mask_img=mask_file[0],
             labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
             labels=parcel_approach[list(parcel_approach.keys())[0]]["labels"], 
             resampling_target='data',
@@ -95,13 +98,13 @@
 
             # Timeseries with the extracted scans corresponding to condition; set is used to remove overlapping TRs    
             timeseries = timeseries[sorted(list(set(scan_list))),:]
 
         if timeseries.shape[0] == 0:
             warnings.warn(f"Subject {subj_id} timeseries is empty for {run}. Most likely due to condition not existing or TRs correspoonding to the condition being removed by `dummy_scans`.")
         else:
-            subject_timeseries[subj_id].update({run: timeseries})
+            subject_timeseries[subj_id].update({run_id: timeseries})
     
     if len(subject_timeseries[subj_id].keys()) == 0:
         subject_timeseries = None
 
     return subject_timeseries
```

### Comparing `neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.8.8.post5/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post4/neurocaps/analysis/cap.py` & `neurocaps-0.8.8.post5/neurocaps/analysis/cap.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post4/neurocaps/analysis/merge.py` & `neurocaps-0.8.8.post5/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post4/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.8.8.post5/neurocaps/extraction/timeseriesextractor.py`

 * *Files 8% similar despite different names*

```diff
@@ -160,22 +160,46 @@
             
                 # Aggregate new timeseries
                 if isinstance(subject_timeseries, dict): self._subject_timeseries.update(subject_timeseries)
         
     # Get valid subjects to iterate through
     def _setup_extraction(self, layout, subj_id_list):
        for subj_id in subj_id_list:
-            nifti_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, session=self._task_info["session"],extension = "nii.gz", subject=subj_id))
-            bold_metadata_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, session=self._task_info["session"], extension = "json", subject=subj_id))
-            event_files = sorted([file for file in sorted(layout.get(return_type="filename",suffix="events", task=self._task_info["task"], session=self._task_info["session"],extension = "tsv", subject = subj_id))]) if self._task_info["condition"] else []
-            confound_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], session=self._task_info["session"],extension = "tsv", subject=subj_id))
-            confound_metadata_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], session=self._task_info["session"],extension = "json", subject=subj_id))
-            mask_files = sorted(layout.get(scope='derivatives', return_type='file', suffix='mask', task=self._task_info["task"], space=self._space, session=self._task_info["session"], extension = "nii.gz", subject=subj_id))
+            if self._task_info["session"]:
+                nifti_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, session=self._task_info["session"],extension = "nii.gz", subject=subj_id))
+                bold_metadata_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, session=self._task_info["session"], extension = "json", subject=subj_id))
+                event_files = sorted([file for file in sorted(layout.get(return_type="filename",suffix="events", task=self._task_info["task"], session=self._task_info["session"],extension = "tsv", subject = subj_id))]) if self._task_info["condition"] else []
+                confound_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], session=self._task_info["session"],extension = "tsv", subject=subj_id))
+                confound_metadata_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], session=self._task_info["session"],extension = "json", subject=subj_id))
+                mask_files = sorted(layout.get(scope='derivatives', return_type='file', suffix='mask', task=self._task_info["task"], space=self._space, session=self._task_info["session"], extension = "nii.gz", subject=subj_id))
+            else:
+                nifti_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, extension = "nii.gz", subject=subj_id))
+                bold_metadata_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, extension = "json", subject=subj_id))
+                event_files = sorted([file for file in sorted(layout.get(return_type="filename",suffix="events", task=self._task_info["task"], extension = "tsv", subject = subj_id))]) if self._task_info["condition"] else []
+                confound_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], extension = "tsv", subject=subj_id))
+                confound_metadata_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], extension = "json", subject=subj_id))
+                mask_files = sorted(layout.get(scope='derivatives', return_type='file', suffix='mask', task=self._task_info["task"], space=self._space, extension = "nii.gz", subject=subj_id))
+
+            # Generate a list of runs to iterate through based on runs in nifti_files
+            if self._task_info["runs"]:
+                check_runs = [f"run-{run}" for run in self._task_info["runs"]] 
+            elif len(nifti_files) != 0:
+                if "run-" in nifti_files[0].split("/")[-1]:
+                    check_runs = [re.search("run-(\\S+?)[-_]",x.split("/")[-1])[0][:-1] for x in nifti_files]
+                else:
+                   check_runs = [] 
+            else:
+                check_runs = []
+
             # Generate a list of runs to iterate through based on runs in nifti_files
-            check_runs = [f"run-{run}" for run in self._task_info["runs"]] if self._task_info["runs"] else [re.search("run-(\\d+)",x)[0] for x in nifti_files]
+            if not self._task_info["session"] and len(nifti_files) != 0:
+                if "ses-" in nifti_files[0].split("/")[-1]:
+                    check_sessions = [re.search("ses-(\\S+?)[-_]",x.split("/")[-1])[0][:-1] for x in nifti_files]
+                    if len(list(set(check_sessions))) > 1:
+                        raise ValueError(f"`session` not specified but subject {subj_id} has more than one session : {sorted(list(set(check_sessions)))}. In order to continue timeseries extraction, the specific session to extract must be specified")
 
             if len(nifti_files) == 0 or len(mask_files) == 0:
                 warnings.warn(f"Skipping subject: {subj_id} due to missing nifti or mask files.")
                 continue
 
             if self._signal_clean_info["use_confounds"]:
                 if len(confound_files) == 0:
@@ -184,37 +208,39 @@
                 if len(confound_metadata_files) == 0 and self._signal_clean_info["n_acompcor_separate"]:
                     warnings.warn(f"Skipping subject: {subj_id} due to missing confound metadata to locate the first six components of the white-matter and cerobrospinal fluid masks seperately.")
                     continue
             
             if self._task_info["condition"] and len(event_files) == 0:
                 warnings.warn(f"Skipping subject: {subj_id} due to having no event files.")
                 continue
-
-            run_list = []
-            # Check if at least one run has all files present
-            for run in check_runs:
-                curr_list = []
-                # Assess is any of these returns True
-                curr_list.append(any([run in file for file in nifti_files]))
-                if self._task_info["condition"]: curr_list.append(any([run in file for file in event_files]))
-                if self._signal_clean_info["use_confounds"]:
-                    curr_list.append(any([run in file for file in confound_files]))
-                    if self._signal_clean_info["n_acompcor_separate"]: curr_list.append(any([run in file for file in confound_metadata_files]))
-                curr_list.append(any([run in file for file in mask_files]))
-                # Append runs that contain all needed files
-                if all(curr_list): run_list.append(run)
-            
-            # Skip subject if no run has all needed files present
-            if len(run_list) != len(check_runs) or len(run_list) == 0:
-                if len(run_list) == 0:
-                    if self._task_info["condition"]: warnings.warn(f"Skipping subject: {subj_id} due to no nifti file, mask file, confound tsv file, confound json file being from the same run.")
-                    else: warnings.warn(f"Skipping subject: {subj_id} due to no nifti file, mask file, event file, confound tsv file, confound json file being from the same run.")
-                    continue
-                else: warnings.warn(f"Subject: {subj_id} only has the following runs available: {', '.join(run_list)}")
-
+                
+            if len(check_runs) != 0:
+                run_list = []
+                # Check if at least one run has all files present
+                for run in check_runs:
+                    curr_list = []
+                    # Assess is any of these returns True
+                    curr_list.append(any([run in file for file in nifti_files]))
+                    if self._task_info["condition"]: curr_list.append(any([run in file for file in event_files]))
+                    if self._signal_clean_info["use_confounds"]:
+                        curr_list.append(any([run in file for file in confound_files]))
+                        if self._signal_clean_info["n_acompcor_separate"]: curr_list.append(any([run in file for file in confound_metadata_files]))
+                    curr_list.append(any([run in file for file in mask_files]))
+                    # Append runs that contain all needed files
+                    if all(curr_list): run_list.append(run)
+                
+                # Skip subject if no run has all needed files present
+                if len(run_list) != len(check_runs) or len(run_list) == 0:
+                    if len(run_list) == 0:
+                        if self._task_info["condition"]: warnings.warn(f"Skipping subject: {subj_id} due to no nifti file, mask file, confound tsv file, confound json file being from the same run.")
+                        else: warnings.warn(f"Skipping subject: {subj_id} due to no nifti file, mask file, event file, confound tsv file, confound json file being from the same run.")
+                        continue
+                    else: warnings.warn(f"Subject: {subj_id} only has the following runs available: {', '.join(run_list)}")
+            else:
+                run_list = [None]
             # Add subject list to subject attribute. These are subjects that will be ran
             self._subject_ids.append(subj_id)
 
             # Get repetition time for the subject
             tr = self._task_info["tr"] if self._task_info["tr"] else json.load(open(bold_metadata_files[0]))["RepetitionTime"]
 
             # Store subject specific information
```

### Comparing `neurocaps-0.8.8.post4/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.8.8.post5/neurocaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.8.8.post4
+Version: 0.8.8.post5
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `neurocaps-0.8.8.post4/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.8.8.post5/neurocaps.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 neurocaps/analysis/__init__.py
 neurocaps/analysis/cap.py
 neurocaps/analysis/merge.py
 neurocaps/extraction/__init__.py
 neurocaps/extraction/timeseriesextractor.py
 tests/test_CAP.py
 tests/test_TimeseriesExtractor.py
+tests/test_TimeseriesExtractor_additional.py
 tests/test_merge_dicts.py
```

### Comparing `neurocaps-0.8.8.post4/pyproject.toml` & `neurocaps-0.8.8.post5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neurocaps"
-version = "0.8.8post4"
+version = "0.8.8post5"
 authors = [{name = "Donisha Smith", email = "donishasmith@outlook.com"}]
 description = "Co-activation patterns Python package"
 readme = "README.md"
 requires-python = ">=3.9.0"
 keywords = ["python", "Co-Activation Patterns", "CAPs", "neuroimaging", "fmri", "dfc", "dynamic functional connectivity", "fMRIPrep"]
 classifiers = [
     "Intended Audience :: Education",
```

### Comparing `neurocaps-0.8.8.post4/tests/test_CAP.py` & `neurocaps-0.8.8.post5/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post4/tests/test_TimeseriesExtractor.py` & `neurocaps-0.8.8.post5/tests/test_TimeseriesExtractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import os, pytest
 from neurocaps.extraction import TimeseriesExtractor
-from neurocaps.analysis import CAP
-
 
 def test_TimeseriesExtractor_no_parallel():
     dir = os.path.dirname(__file__)
 
     confounds=["Cosine*", "aComp*", "Rot*"]
 
     parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
@@ -18,8 +16,30 @@
 
     pipeline_name = "fmriprep_1.0.0/fmriprep"
     extractor.get_bold(bids_dir=bids_dir, session='002', task="rest", pipeline_name=pipeline_name, tr=1.2)
     
     print(extractor.subject_timeseries, flush=True)
 
     assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 100
-    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 34
+    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 40
+
+def test_TimeseriesExtractor_no_parallel_no_session():
+    dir = os.path.dirname(__file__)
+
+    confounds=["Cosine*", "aComp*", "Rot*"]
+
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
+                                    confound_names=confounds)
+
+    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
+
+    pipeline_name = "fmriprep_1.0.0/fmriprep"
+    extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
+    
+    print(extractor.subject_timeseries, flush=True)
+
+    assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 100
+    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 40
+
```

### Comparing `neurocaps-0.8.8.post4/tests/test_merge_dicts.py` & `neurocaps-0.8.8.post5/tests/test_merge_dicts.py`

 * *Files identical despite different names*

