# Comparing `tmp/fancylog-0.4.1.tar.gz` & `tmp/fancylog-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fancylog-0.4.1.tar", last modified: Tue Apr 30 16:34:57 2024, max compression
+gzip compressed data, was "fancylog-0.4.2.tar", last modified: Thu May  2 12:51:35 2024, max compression
```

## Comparing `fancylog-0.4.1.tar` & `fancylog-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.224138 fancylog-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.224138 fancylog-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-30 16:34:51.000000 fancylog-0.4.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-30 16:34:51.000000 fancylog-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-30 16:34:51.000000 fancylog-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-30 16:34:51.000000 fancylog-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 16:34:51.000000 fancylog-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-30 16:34:57.228139 fancylog-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-30 16:34:51.000000 fancylog-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/fancylog/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 16:34:51.000000 fancylog-0.4.1/fancylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-30 16:34:51.000000 fancylog-0.4.1/fancylog/fancylog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/fancylog/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:51.000000 fancylog-0.4.1/fancylog/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-30 16:34:51.000000 fancylog-0.4.1/fancylog/tools/git.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/fancylog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-30 16:34:57.000000 fancylog-0.4.1/fancylog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 16:34:57.000000 fancylog-0.4.1/fancylog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:34:57.000000 fancylog-0.4.1/fancylog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 16:34:57.000000 fancylog-0.4.1/fancylog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 16:34:57.000000 fancylog-0.4.1/fancylog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-30 16:34:51.000000 fancylog-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:34:57.228139 fancylog-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:51.000000 fancylog-0.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:57.228139 fancylog-0.4.1/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:34:51.000000 fancylog-0.4.1/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-30 16:34:51.000000 fancylog-0.4.1/tests/tests/test_general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:35.064711 fancylog-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:35.060711 fancylog-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:35.060711 fancylog-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-02 12:51:28.000000 fancylog-0.4.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-02 12:51:28.000000 fancylog-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-02 12:51:28.000000 fancylog-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-02 12:51:28.000000 fancylog-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-02 12:51:28.000000 fancylog-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-02 12:51:35.064711 fancylog-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-02 12:51:28.000000 fancylog-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:35.060711 fancylog-0.4.2/fancylog/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 12:51:28.000000 fancylog-0.4.2/fancylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-02 12:51:28.000000 fancylog-0.4.2/fancylog/fancylog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:35.060711 fancylog-0.4.2/fancylog/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:28.000000 fancylog-0.4.2/fancylog/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-02 12:51:28.000000 fancylog-0.4.2/fancylog/tools/git.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:35.064711 fancylog-0.4.2/fancylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-02 12:51:35.000000 fancylog-0.4.2/fancylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-02 12:51:35.000000 fancylog-0.4.2/fancylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:51:35.000000 fancylog-0.4.2/fancylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 12:51:35.000000 fancylog-0.4.2/fancylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 12:51:35.000000 fancylog-0.4.2/fancylog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-02 12:51:28.000000 fancylog-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:51:35.064711 fancylog-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:35.060711 fancylog-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:28.000000 fancylog-0.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:35.064711 fancylog-0.4.2/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:51:28.000000 fancylog-0.4.2/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-02 12:51:28.000000 fancylog-0.4.2/tests/tests/test_general.py
```

### Comparing `fancylog-0.4.1/.github/workflows/test_and_deploy.yml` & `fancylog-0.4.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `fancylog-0.4.1/.gitignore` & `fancylog-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fancylog-0.4.1/.pre-commit-config.yaml` & `fancylog-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fancylog-0.4.1/LICENSE` & `fancylog-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fancylog-0.4.1/PKG-INFO` & `fancylog-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fancylog
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fancier logging in Python
 Author-email: Adam Tyson <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/neuroinformatics-unit/fancylog
 Project-URL: bug_tracker, https://github.com/neuroinformatics-unit/fancylog/issues
 Project-URL: documentation, https://github.com/neuroinformatics-unit/fancylog
 Project-URL: source_code, https://github.com/neuroinformatics-unit/fancylog
```

### Comparing `fancylog-0.4.1/README.md` & `fancylog-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `fancylog-0.4.1/fancylog/fancylog.py` & `fancylog-0.4.2/fancylog/fancylog.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,14 +239,16 @@
     Default: 'DEBUG'
     :param log_to_console: Print logs to the console or not
     :param logger_name: If None, logger uses default logger. Otherwise,
     logger name is set to `logger_name`.
     """
     if logger_name:
         logger = logging.getLogger(logger_name)
+        logger.handlers = []
+        logger.propagate = False
     else:
         logger = logging.getLogger()
 
     logger.setLevel(getattr(logging, file_level))
 
     formatter = logging.Formatter(
         "%(asctime)s - %(levelname)s"
@@ -286,22 +288,29 @@
     Default: 'DEBUG'
     :param multiprocessing_aware: Default: True
     :param log_to_console: Print logs to the console or no.
     Default: True
     :param logger_name: If None, logger uses default logger. Otherwise,
         logger name is set to `logger_name`.
     """
-    initialise_logger(
+    logger = initialise_logger(
         filename,
         print_level=print_level,
         file_level=file_level,
         log_to_console=log_to_console,
         logger_name=logger_name,
     )
     if multiprocessing_aware:
+        if logger_name:
+            raise ValueError(
+                "`multiprocessing_aware` is not supported"
+                "with `logger_name`. Multiprocess logging"
+                "must be performed with the root logger."
+            )
+
         try:
             import multiprocessing_logging
 
             multiprocessing_logging.install_mp_handler()
             logging.info("Starting logging")
             logging.info(
                 "Multiprocessing-logging module found. Logging from all"
@@ -310,16 +319,16 @@
         except ModuleNotFoundError:
             logging.info("Starting logging")
             logging.info(
                 "Multiprocessing-logging module not found, not logging "
                 "multiple processes."
             )
     else:
-        logging.info("Starting logging")
-        logging.info("Not logging multiple processes")
+        logger.info("Starting logging")
+        logger.info("Not logging multiple processes")
 
 
 def disable_logging():
     """Prevents any more logging. Saves remembering that logging.disable() with
     no argument doesn't work.
     :return:
     """
```

### Comparing `fancylog-0.4.1/fancylog/tools/git.py` & `fancylog-0.4.2/fancylog/tools/git.py`

 * *Files identical despite different names*

### Comparing `fancylog-0.4.1/fancylog.egg-info/PKG-INFO` & `fancylog-0.4.2/fancylog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fancylog
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fancier logging in Python
 Author-email: Adam Tyson <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/neuroinformatics-unit/fancylog
 Project-URL: bug_tracker, https://github.com/neuroinformatics-unit/fancylog/issues
 Project-URL: documentation, https://github.com/neuroinformatics-unit/fancylog
 Project-URL: source_code, https://github.com/neuroinformatics-unit/fancylog
```

### Comparing `fancylog-0.4.1/pyproject.toml` & `fancylog-0.4.2/pyproject.toml`

 * *Files identical despite different names*

