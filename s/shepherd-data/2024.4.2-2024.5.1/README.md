# Comparing `tmp/shepherd_data-2024.4.2.tar.gz` & `tmp/shepherd_data-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_data-2024.4.2.tar", last modified: Wed Apr 24 19:39:07 2024, max compression
+gzip compressed data, was "shepherd_data-2024.5.1.tar", last modified: Thu May  2 10:00:47 2024, max compression
```

## Comparing `shepherd_data-2024.4.2.tar` & `shepherd_data-2024.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:39:07.061107 shepherd_data-2024.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-24 19:39:07.061107 shepherd_data-2024.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:39:07.061107 shepherd_data-2024.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:39:07.057107 shepherd_data-2024.4.2/shepherd_data/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/shepherd_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14981 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/shepherd_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/shepherd_data/ivonne.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/shepherd_data/mppt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/shepherd_data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:39:07.057107 shepherd_data-2024.4.2/shepherd_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 19:39:07.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:39:06.000000 shepherd_data-2024.4.2/shepherd_data.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:39:07.057107 shepherd_data-2024.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_cli_downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_cli_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_cli_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_cli_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_ivonne.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 19:38:51.000000 shepherd_data-2024.4.2/tests/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:47.858806 shepherd_data-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-02 10:00:47.858806 shepherd_data-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:00:47.858806 shepherd_data-2024.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:47.854806 shepherd_data-2024.5.1/shepherd_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/shepherd_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14992 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/shepherd_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/shepherd_data/ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/shepherd_data/mppt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/shepherd_data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:47.858806 shepherd_data-2024.5.1/shepherd_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-02 10:00:47.000000 shepherd_data-2024.5.1/shepherd_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-02 10:00:47.000000 shepherd_data-2024.5.1/shepherd_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:00:47.000000 shepherd_data-2024.5.1/shepherd_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 10:00:47.000000 shepherd_data-2024.5.1/shepherd_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 10:00:47.000000 shepherd_data-2024.5.1/shepherd_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 10:00:47.000000 shepherd_data-2024.5.1/shepherd_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:00:47.000000 shepherd_data-2024.5.1/shepherd_data.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:00:47.858806 shepherd_data-2024.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/tests/test_cli_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/tests/test_cli_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/tests/test_cli_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/tests/test_cli_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/tests/test_ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 10:00:29.000000 shepherd_data-2024.5.1/tests/test_reader.py
```

### Comparing `shepherd_data-2024.4.2/PKG-INFO` & `shepherd_data-2024.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_data
-Version: 2024.4.2
+Version: 2024.5.1
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Author-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Maintainer-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Project-URL: Documentation, https://github.com/orgua/shepherd-datalib/blob/main/README.md
 Project-URL: Issues, https://pypi.org/project/shepherd-data/issues
 Project-URL: Source, https://pypi.org/project/shepherd-data/
 Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
@@ -31,15 +31,15 @@
 Requires-Dist: click
 Requires-Dist: h5py
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: pyYAML
 Requires-Dist: scipy
-Requires-Dist: shepherd-core[inventory]>=2024.4.2
+Requires-Dist: shepherd-core[inventory]>=2024.5.1
 Requires-Dist: tqdm
 Provides-Extra: elf
 Requires-Dist: shepherd-core[elf]; extra == "elf"
 Provides-Extra: dev
 Requires-Dist: shepherd-core[dev]; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Provides-Extra: test
```

### Comparing `shepherd_data-2024.4.2/README.md` & `shepherd_data-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.2/pyproject.toml` & `shepherd_data-2024.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "click",
     "h5py",
     "matplotlib",  # full-version
     "numpy",
     "pandas>=2.0.0",  # full-version, v2 is OK
     "pyYAML",
     "scipy",   # full-version
-    "shepherd-core[inventory]>=2024.4.2",
+    "shepherd-core[inventory]>=2024.5.1",
     "tqdm",    # full-version
 ]
 
 [project.optional-dependencies]
 elf = [
     "shepherd-core[elf]"
 ]
```

### Comparing `shepherd_data-2024.4.2/shepherd_data/cli.py` & `shepherd_data-2024.5.1/shepherd_data/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,19 +164,20 @@
     """Extract metadata and logs from file or directory containing shepherd-recordings."""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     for file in files:
         logger.info("Extracting metadata & logs from '%s' ...", file.name)
         # TODO: add default exports (user-centric) and allow specifying --all or specific ones
         # TODO: could also be combined with other extractors (just have one)
-        # TODO: remove deprecated timesync; "shepherd-log", "dmesg", "exceptions"
         try:
             with Reader(file, verbose=verbose_level > 2) as shpr:
                 shpr.save_metadata()
-                for element in ["ptp", "sysutil", "timesync"]:
+                csvs_depr = ["sysutil", "timesync"]
+                csvs = ["ptp", "sys_util", "pru_util"]
+                for element in csvs + csvs_depr:
                     if element in shpr.h5file:
                         shpr.save_csv(shpr[element], separator)
                 logs_depr = ["shepherd-log", "dmesg", "exceptions"]
                 logs = ["sheep", "kernel", "phc2sys", "uart"]
                 for element in logs + logs_depr:
                     if element in shpr.h5file:
                         shpr.save_log(shpr[element])
```

### Comparing `shepherd_data-2024.4.2/shepherd_data/ivonne.py` & `shepherd_data-2024.5.1/shepherd_data/ivonne.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.2/shepherd_data/mppt.py` & `shepherd_data-2024.5.1/shepherd_data/mppt.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.2/shepherd_data/reader.py` & `shepherd_data-2024.5.1/shepherd_data/reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.2/shepherd_data.egg-info/PKG-INFO` & `shepherd_data-2024.5.1/shepherd_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_data
-Version: 2024.4.2
+Version: 2024.5.1
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Author-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Maintainer-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Project-URL: Documentation, https://github.com/orgua/shepherd-datalib/blob/main/README.md
 Project-URL: Issues, https://pypi.org/project/shepherd-data/issues
 Project-URL: Source, https://pypi.org/project/shepherd-data/
 Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
@@ -31,15 +31,15 @@
 Requires-Dist: click
 Requires-Dist: h5py
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: pyYAML
 Requires-Dist: scipy
-Requires-Dist: shepherd-core[inventory]>=2024.4.2
+Requires-Dist: shepherd-core[inventory]>=2024.5.1
 Requires-Dist: tqdm
 Provides-Extra: elf
 Requires-Dist: shepherd-core[elf]; extra == "elf"
 Provides-Extra: dev
 Requires-Dist: shepherd-core[dev]; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Provides-Extra: test
```

### Comparing `shepherd_data-2024.4.2/shepherd_data.egg-info/SOURCES.txt` & `shepherd_data-2024.5.1/shepherd_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.2/tests/test_cli_downsample.py` & `shepherd_data-2024.5.1/tests/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.2/tests/test_cli_extract.py` & `shepherd_data-2024.5.1/tests/test_cli_extract.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.2/tests/test_cli_plot.py` & `shepherd_data-2024.5.1/tests/test_cli_plot.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.2/tests/test_examples.py` & `shepherd_data-2024.5.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2024.4.2/tests/test_ivonne.py` & `shepherd_data-2024.5.1/tests/test_ivonne.py`

 * *Files identical despite different names*

