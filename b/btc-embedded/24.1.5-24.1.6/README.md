# Comparing `tmp/btc_embedded-24.1.5.tar.gz` & `tmp/btc_embedded-24.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btc_embedded-24.1.5.tar", last modified: Mon Apr  8 13:49:02 2024, max compression
+gzip compressed data, was "btc_embedded-24.1.6.tar", last modified: Mon Apr  8 13:55:12 2024, max compression
```

## Comparing `btc_embedded-24.1.5.tar` & `btc_embedded-24.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 13:49:02.947741 btc_embedded-24.1.5/
--rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.5/LICENSE.txt
--rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.5/MANIFEST.in
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-08 13:49:02.947854 btc_embedded-24.1.5/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.5/README.md
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 13:49:02.946785 btc_embedded-24.1.5/btc_embedded/
--rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.5/btc_embedded/__init__.py
--rw-r--r--   0 thabok     (501) staff       (20)    22308 2024-04-08 13:48:36.000000 btc_embedded-24.1.5/btc_embedded/api.py
--rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.5/btc_embedded/btc_config.yml
--rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.5/btc_embedded/btc_summary_report.template
--rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.5/btc_embedded/config.py
--rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.5/btc_embedded/reporting.py
--rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.5/btc_embedded/util.py
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 13:49:02.947607 btc_embedded-24.1.5/btc_embedded.egg-info/
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-08 13:49:02.000000 btc_embedded-24.1.5/btc_embedded.egg-info/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-08 13:49:02.000000 btc_embedded-24.1.5/btc_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-08 13:49:02.000000 btc_embedded-24.1.5/btc_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-08 13:49:02.000000 btc_embedded-24.1.5/btc_embedded.egg-info/requires.txt
--rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-08 13:49:02.000000 btc_embedded-24.1.5/btc_embedded.egg-info/top_level.txt
--rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-08 13:49:02.948106 btc_embedded-24.1.5/setup.cfg
--rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-08 13:48:26.000000 btc_embedded-24.1.5/setup.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 13:55:12.504053 btc_embedded-24.1.6/
+-rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/LICENSE.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/MANIFEST.in
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-08 13:55:12.504139 btc_embedded-24.1.6/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/README.md
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 13:55:12.503228 btc_embedded-24.1.6/btc_embedded/
+-rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/btc_embedded/__init__.py
+-rw-r--r--   0 thabok     (501) staff       (20)    22323 2024-04-08 13:55:04.000000 btc_embedded-24.1.6/btc_embedded/api.py
+-rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/btc_embedded/btc_config.yml
+-rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/btc_embedded/btc_summary_report.template
+-rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.6/btc_embedded/config.py
+-rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/btc_embedded/reporting.py
+-rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/btc_embedded/util.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 13:55:12.503928 btc_embedded-24.1.6/btc_embedded.egg-info/
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-08 13:55:12.000000 btc_embedded-24.1.6/btc_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-08 13:55:12.000000 btc_embedded-24.1.6/btc_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-08 13:55:12.000000 btc_embedded-24.1.6/btc_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-08 13:55:12.000000 btc_embedded-24.1.6/btc_embedded.egg-info/requires.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-08 13:55:12.000000 btc_embedded-24.1.6/btc_embedded.egg-info/top_level.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-08 13:55:12.504368 btc_embedded-24.1.6/setup.cfg
+-rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-08 13:55:09.000000 btc_embedded-24.1.6/setup.py
```

### Comparing `btc_embedded-24.1.5/LICENSE.txt` & `btc_embedded-24.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.5/PKG-INFO` & `btc_embedded-24.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc_embedded
-Version: 24.1.5
+Version: 24.1.6
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-24.1.5/README.md` & `btc_embedded-24.1.6/README.md`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.5/btc_embedded/api.py` & `btc_embedded-24.1.6/btc_embedded/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,14 +361,15 @@
         self.log_file_path = os.environ['LOG_DIR'] + '/current.log'
         self.actively_started = True
         
         # if container has matlab -> assume that this shall be started as well
         if shutil.which('matlab') and not skip_matlab_start: subprocess.Popen('matlab')
 
     def check_for_ep_start_keyword(self, start_time, timeout):
+        return
         while True:
             if (time.time() - start_time) > timeout:
                 print(f"\n\nCould not connect to EP within the specified timeout of {timeout} seconds. \n\n")
                 raise Exception("Application didn't respond within the defined timeout.")
             elif (not self._is_ep_process_still_alive()):
                 print(f"\n\nApplication failed to start. Please check the log file for further information:\n{self.log_file_path}\n\n")
                 raise Exception("Application failed to start.")
```

### Comparing `btc_embedded-24.1.5/btc_embedded/btc_config.yml` & `btc_embedded-24.1.6/btc_embedded/btc_config.yml`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.5/btc_embedded/btc_summary_report.template` & `btc_embedded-24.1.6/btc_embedded/btc_summary_report.template`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.5/btc_embedded/config.py` & `btc_embedded-24.1.6/btc_embedded/config.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.5/btc_embedded/reporting.py` & `btc_embedded-24.1.6/btc_embedded/reporting.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.5/btc_embedded/util.py` & `btc_embedded-24.1.6/btc_embedded/util.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.5/btc_embedded.egg-info/PKG-INFO` & `btc_embedded-24.1.6/btc_embedded.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc-embedded
-Version: 24.1.5
+Version: 24.1.6
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-24.1.5/setup.py` & `btc_embedded-24.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='btc_embedded',
-    version='24.1.5',
+    version='24.1.6',
     packages=['btc_embedded'],
     include_package_data=True,
     license='MIT',
     description='API wrapper for BTC EmbeddedPlatform 23.3p0 REST API',
     author='Thabo Krick',
     author_email='thabo.krick@btc-embedded.com',
     url='https://github.com/btc-embedded/btc-embedded',
```

