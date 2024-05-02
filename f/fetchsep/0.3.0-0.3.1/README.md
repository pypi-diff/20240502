# Comparing `tmp/fetchsep-0.3.0.tar.gz` & `tmp/fetchsep-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetchsep-0.3.0.tar", last modified: Thu Nov  2 16:54:04 2023, max compression
+gzip compressed data, was "fetchsep-0.3.1.tar", last modified: Thu May  2 20:27:43 2024, max compression
```

## Comparing `fetchsep-0.3.0.tar` & `fetchsep-0.3.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.335835 fetchsep-0.3.0/
--rw-r--r--   0 regeland   (502) staff       (20)      165 2023-06-01 16:48:43.000000 fetchsep-0.3.0/AUTHORS.rst
--rw-r--r--   0 regeland   (502) staff       (20)     3550 2023-06-01 16:48:43.000000 fetchsep-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 regeland   (502) staff       (20)     1890 2023-11-02 16:08:57.000000 fetchsep-0.3.0/HISTORY.rst
--rw-r--r--   0 regeland   (502) staff       (20)     1074 2023-06-01 16:48:43.000000 fetchsep-0.3.0/LICENSE
--rw-r--r--   0 regeland   (502) staff       (20)      337 2023-09-22 19:46:29.000000 fetchsep-0.3.0/MANIFEST.in
--rw-r--r--   0 regeland   (502) staff       (20)     8544 2023-11-02 16:54:04.335328 fetchsep-0.3.0/PKG-INFO
--rw-r--r--   0 regeland   (502) staff       (20)     5575 2023-09-22 19:00:30.000000 fetchsep-0.3.0/README.rst
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.269296 fetchsep-0.3.0/bin/
--rwxr-xr-x   0 regeland   (502) staff       (20)    13879 2023-11-01 17:17:56.000000 fetchsep-0.3.0/bin/fetchsep_prepare_obs
--rwxr-xr-x   0 regeland   (502) staff       (20)     4515 2023-09-22 18:28:54.000000 fetchsep-0.3.0/bin/idsep
--rwxr-xr-x   0 regeland   (502) staff       (20)     2332 2023-09-21 21:05:22.000000 fetchsep-0.3.0/bin/make_opsep_event_list
--rwxr-xr-x   0 regeland   (502) staff       (20)     7296 2023-09-22 18:31:34.000000 fetchsep-0.3.0/bin/opsep
--rwxr-xr-x   0 regeland   (502) staff       (20)     5779 2023-09-21 21:05:22.000000 fetchsep-0.3.0/bin/opsep_batch
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.285444 fetchsep-0.3.0/docs/
--rw-r--r--   0 regeland   (502) staff       (20)      609 2023-06-01 16:47:59.000000 fetchsep-0.3.0/docs/Makefile
--rw-r--r--   0 regeland   (502) staff       (20)       28 2023-06-01 16:47:59.000000 fetchsep-0.3.0/docs/authors.rst
--rwxr-xr-x   0 regeland   (502) staff       (20)     4804 2023-06-01 16:47:59.000000 fetchsep-0.3.0/docs/conf.py
--rw-r--r--   0 regeland   (502) staff       (20)       33 2023-06-01 16:47:59.000000 fetchsep-0.3.0/docs/contributing.rst
--rw-r--r--   0 regeland   (502) staff       (20)       28 2023-06-01 16:47:59.000000 fetchsep-0.3.0/docs/history.rst
--rw-r--r--   0 regeland   (502) staff       (20)      306 2023-06-01 16:47:59.000000 fetchsep-0.3.0/docs/index.rst
--rw-r--r--   0 regeland   (502) staff       (20)     1141 2023-06-01 16:47:59.000000 fetchsep-0.3.0/docs/installation.rst
--rw-r--r--   0 regeland   (502) staff       (20)      806 2023-06-01 16:47:59.000000 fetchsep-0.3.0/docs/make.bat
--rw-r--r--   0 regeland   (502) staff       (20)       27 2023-06-01 16:47:59.000000 fetchsep-0.3.0/docs/readme.rst
--rw-r--r--   0 regeland   (502) staff       (20)       72 2023-06-01 16:47:59.000000 fetchsep-0.3.0/docs/usage.rst
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.287584 fetchsep-0.3.0/fetchsep/
--rw-r--r--   0 regeland   (502) staff       (20)       96 2023-11-02 16:27:08.000000 fetchsep-0.3.0/fetchsep/__init__.py
--rw-r--r--   0 regeland   (502) staff       (20)      439 2023-06-01 18:20:32.000000 fetchsep-0.3.0/fetchsep/cli.py
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.296080 fetchsep-0.3.0/fetchsep/idsep/
--rw-r--r--   0 regeland   (502) staff       (20)       21 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/idsep/__init__.py
--rw-r--r--   0 regeland   (502) staff       (20)    41817 2023-11-01 17:17:56.000000 fetchsep-0.3.0/fetchsep/idsep/idsep.py
--rw-r--r--   0 regeland   (502) staff       (20)     7698 2023-11-01 17:17:56.000000 fetchsep-0.3.0/fetchsep/idsep/make_event_list.py
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.301684 fetchsep-0.3.0/fetchsep/json/
--rw-r--r--   0 regeland   (502) staff       (20)        0 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/json/__init__.py
--rw-r--r--   0 regeland   (502) staff       (20)    66114 2023-11-01 17:17:56.000000 fetchsep-0.3.0/fetchsep/json/ccmc_json_handler.py
--rw-r--r--   0 regeland   (502) staff       (20)    24084 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/json/keys.py
--rwxr-xr-x   0 regeland   (502) staff       (20)     5662 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/json/read_json_example.py
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.309242 fetchsep-0.3.0/fetchsep/json/templates/
--rw-r--r--   0 regeland   (502) staff       (20)        0 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/json/templates/__init__.py
--rw-r--r--   0 regeland   (502) staff       (20)     2987 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/json/templates/model_example.json
--rw-r--r--   0 regeland   (502) staff       (20)     2531 2023-06-01 16:31:11.000000 fetchsep-0.3.0/fetchsep/json/templates/model_template.json
--rw-r--r--   0 regeland   (502) staff       (20)     2106 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/json/templates/observations_example.json
--rw-r--r--   0 regeland   (502) staff       (20)     2546 2023-06-01 16:31:11.000000 fetchsep-0.3.0/fetchsep/json/templates/observations_template.json
--rw-r--r--   0 regeland   (502) staff       (20)     2511 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/json/templates/triggers_template.json
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.312465 fetchsep-0.3.0/fetchsep/opsep/
--rw-r--r--   0 regeland   (502) staff       (20)       21 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/opsep/__init__.py
--rwxr-xr-x   0 regeland   (502) staff       (20)    22389 2023-11-01 17:17:56.000000 fetchsep-0.3.0/fetchsep/opsep/batch_run_opsep.py
--rwxr-xr-x   0 regeland   (502) staff       (20)   185514 2023-11-01 19:44:36.000000 fetchsep-0.3.0/fetchsep/opsep/opsep.py
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.328053 fetchsep-0.3.0/fetchsep/utils/
--rw-r--r--   0 regeland   (502) staff       (20)        0 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/utils/__init__.py
--rw-r--r--   0 regeland   (502) staff       (20)     2326 2023-09-22 17:34:40.000000 fetchsep-0.3.0/fetchsep/utils/config.py
--rw-r--r--   0 regeland   (502) staff       (20)     1139 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/utils/date_handler.py
--rw-r--r--   0 regeland   (502) staff       (20)    25669 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/utils/define_background_idsep.py
--rw-r--r--   0 regeland   (502) staff       (20)    26850 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/utils/derive_background_opsep.py
--rw-r--r--   0 regeland   (502) staff       (20)     9358 2023-11-01 17:17:56.000000 fetchsep-0.3.0/fetchsep/utils/fetchsep.cfg
--rw-r--r--   0 regeland   (502) staff       (20)    13813 2023-11-01 17:17:56.000000 fetchsep-0.3.0/fetchsep/utils/move_output.py
--rw-r--r--   0 regeland   (502) staff       (20)    23068 2023-06-01 16:15:44.000000 fetchsep-0.3.0/fetchsep/utils/plotting_tools.py
--rw-r--r--   0 regeland   (502) staff       (20)   120974 2023-09-27 19:32:16.000000 fetchsep-0.3.0/fetchsep/utils/read_datasets.py
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.292675 fetchsep-0.3.0/fetchsep.egg-info/
--rw-r--r--   0 regeland   (502) staff       (20)     8544 2023-11-02 16:54:04.000000 fetchsep-0.3.0/fetchsep.egg-info/PKG-INFO
--rw-r--r--   0 regeland   (502) staff       (20)     1480 2023-11-02 16:54:04.000000 fetchsep-0.3.0/fetchsep.egg-info/SOURCES.txt
--rw-r--r--   0 regeland   (502) staff       (20)        1 2023-11-02 16:54:04.000000 fetchsep-0.3.0/fetchsep.egg-info/dependency_links.txt
--rw-r--r--   0 regeland   (502) staff       (20)        1 2023-11-02 16:54:04.000000 fetchsep-0.3.0/fetchsep.egg-info/not-zip-safe
--rw-r--r--   0 regeland   (502) staff       (20)      106 2023-11-02 16:54:04.000000 fetchsep-0.3.0/fetchsep.egg-info/requires.txt
--rw-r--r--   0 regeland   (502) staff       (20)        9 2023-11-02 16:54:04.000000 fetchsep-0.3.0/fetchsep.egg-info/top_level.txt
--rw-r--r--   0 regeland   (502) staff       (20)      380 2023-11-02 16:54:04.337239 fetchsep-0.3.0/setup.cfg
--rw-r--r--   0 regeland   (502) staff       (20)     1866 2023-11-02 16:26:48.000000 fetchsep-0.3.0/setup.py
-drwxr-xr-x   0 regeland   (502) staff       (20)        0 2023-11-02 16:54:04.333447 fetchsep-0.3.0/tests/
--rw-r--r--   0 regeland   (502) staff       (20)       38 2023-06-01 16:46:50.000000 fetchsep-0.3.0/tests/__init__.py
--rw-r--r--   0 regeland   (502) staff       (20)      475 2023-09-22 16:34:48.000000 fetchsep-0.3.0/tests/test_config.py
--rw-r--r--   0 regeland   (502) staff       (20)      439 2023-09-22 16:31:04.000000 fetchsep-0.3.0/tests/test_fetchsep.py
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.598262 fetchsep-0.3.1/
+-rw-r--r--   0 regeland   (502) staff       (20)      165 2023-06-01 16:48:43.000000 fetchsep-0.3.1/AUTHORS.rst
+-rw-r--r--   0 regeland   (502) staff       (20)     3541 2024-05-02 19:36:51.000000 fetchsep-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 regeland   (502) staff       (20)     2315 2024-05-02 20:09:09.000000 fetchsep-0.3.1/HISTORY.rst
+-rw-r--r--   0 regeland   (502) staff       (20)     1074 2023-06-01 16:48:43.000000 fetchsep-0.3.1/LICENSE
+-rw-r--r--   0 regeland   (502) staff       (20)      337 2023-09-22 19:46:29.000000 fetchsep-0.3.1/MANIFEST.in
+-rw-r--r--   0 regeland   (502) staff       (20)     8960 2024-05-02 20:27:43.597327 fetchsep-0.3.1/PKG-INFO
+-rw-r--r--   0 regeland   (502) staff       (20)     5569 2024-05-02 19:35:27.000000 fetchsep-0.3.1/README.rst
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.527441 fetchsep-0.3.1/bin/
+-rwxr-xr-x   0 regeland   (502) staff       (20)    13887 2024-05-02 19:40:00.000000 fetchsep-0.3.1/bin/fetchsep_prepare_obs
+-rwxr-xr-x   0 regeland   (502) staff       (20)     4515 2023-09-22 18:28:54.000000 fetchsep-0.3.1/bin/idsep
+-rwxr-xr-x   0 regeland   (502) staff       (20)     2332 2023-09-21 21:05:22.000000 fetchsep-0.3.1/bin/make_opsep_event_list
+-rwxr-xr-x   0 regeland   (502) staff       (20)     7296 2023-09-22 18:31:34.000000 fetchsep-0.3.1/bin/opsep
+-rwxr-xr-x   0 regeland   (502) staff       (20)     5779 2023-09-21 21:05:22.000000 fetchsep-0.3.1/bin/opsep_batch
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.539058 fetchsep-0.3.1/docs/
+-rw-r--r--   0 regeland   (502) staff       (20)      609 2023-06-01 16:47:59.000000 fetchsep-0.3.1/docs/Makefile
+-rw-r--r--   0 regeland   (502) staff       (20)       28 2023-06-01 16:47:59.000000 fetchsep-0.3.1/docs/authors.rst
+-rwxr-xr-x   0 regeland   (502) staff       (20)     4804 2023-06-01 16:47:59.000000 fetchsep-0.3.1/docs/conf.py
+-rw-r--r--   0 regeland   (502) staff       (20)       33 2023-06-01 16:47:59.000000 fetchsep-0.3.1/docs/contributing.rst
+-rw-r--r--   0 regeland   (502) staff       (20)       28 2023-06-01 16:47:59.000000 fetchsep-0.3.1/docs/history.rst
+-rw-r--r--   0 regeland   (502) staff       (20)      306 2023-06-01 16:47:59.000000 fetchsep-0.3.1/docs/index.rst
+-rw-r--r--   0 regeland   (502) staff       (20)     1129 2024-05-02 19:37:23.000000 fetchsep-0.3.1/docs/installation.rst
+-rw-r--r--   0 regeland   (502) staff       (20)      806 2023-06-01 16:47:59.000000 fetchsep-0.3.1/docs/make.bat
+-rw-r--r--   0 regeland   (502) staff       (20)       27 2023-06-01 16:47:59.000000 fetchsep-0.3.1/docs/readme.rst
+-rw-r--r--   0 regeland   (502) staff       (20)       72 2023-06-01 16:47:59.000000 fetchsep-0.3.1/docs/usage.rst
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.540949 fetchsep-0.3.1/fetchsep/
+-rw-r--r--   0 regeland   (502) staff       (20)       96 2024-05-02 20:20:23.000000 fetchsep-0.3.1/fetchsep/__init__.py
+-rw-r--r--   0 regeland   (502) staff       (20)      439 2023-06-01 18:20:32.000000 fetchsep-0.3.1/fetchsep/cli.py
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.549708 fetchsep-0.3.1/fetchsep/idsep/
+-rw-r--r--   0 regeland   (502) staff       (20)       21 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/idsep/__init__.py
+-rw-r--r--   0 regeland   (502) staff       (20)    42289 2024-05-02 19:40:00.000000 fetchsep-0.3.1/fetchsep/idsep/idsep.py
+-rw-r--r--   0 regeland   (502) staff       (20)     7698 2023-11-01 17:17:56.000000 fetchsep-0.3.1/fetchsep/idsep/make_event_list.py
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.556351 fetchsep-0.3.1/fetchsep/json/
+-rw-r--r--   0 regeland   (502) staff       (20)        0 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/json/__init__.py
+-rw-r--r--   0 regeland   (502) staff       (20)    66632 2024-05-02 19:40:00.000000 fetchsep-0.3.1/fetchsep/json/ccmc_json_handler.py
+-rw-r--r--   0 regeland   (502) staff       (20)    24214 2024-05-02 19:40:00.000000 fetchsep-0.3.1/fetchsep/json/keys.py
+-rwxr-xr-x   0 regeland   (502) staff       (20)     5662 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/json/read_json_example.py
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.563921 fetchsep-0.3.1/fetchsep/json/templates/
+-rw-r--r--   0 regeland   (502) staff       (20)        0 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/json/templates/__init__.py
+-rw-r--r--   0 regeland   (502) staff       (20)     2987 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/json/templates/model_example.json
+-rw-r--r--   0 regeland   (502) staff       (20)     2588 2024-05-02 19:40:00.000000 fetchsep-0.3.1/fetchsep/json/templates/model_template.json
+-rw-r--r--   0 regeland   (502) staff       (20)     2106 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/json/templates/observations_example.json
+-rw-r--r--   0 regeland   (502) staff       (20)     2603 2024-05-02 19:40:00.000000 fetchsep-0.3.1/fetchsep/json/templates/observations_template.json
+-rw-r--r--   0 regeland   (502) staff       (20)     2511 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/json/templates/triggers_template.json
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.569541 fetchsep-0.3.1/fetchsep/opsep/
+-rw-r--r--   0 regeland   (502) staff       (20)       21 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/opsep/__init__.py
+-rwxr-xr-x   0 regeland   (502) staff       (20)    22389 2023-11-01 17:17:56.000000 fetchsep-0.3.1/fetchsep/opsep/batch_run_opsep.py
+-rwxr-xr-x   0 regeland   (502) staff       (20)   190662 2024-05-02 19:40:00.000000 fetchsep-0.3.1/fetchsep/opsep/opsep.py
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.589557 fetchsep-0.3.1/fetchsep/utils/
+-rw-r--r--   0 regeland   (502) staff       (20)        0 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/utils/__init__.py
+-rw-r--r--   0 regeland   (502) staff       (20)     2326 2023-09-22 17:34:40.000000 fetchsep-0.3.1/fetchsep/utils/config.py
+-rw-r--r--   0 regeland   (502) staff       (20)     1139 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/utils/date_handler.py
+-rw-r--r--   0 regeland   (502) staff       (20)    25669 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/utils/define_background_idsep.py
+-rw-r--r--   0 regeland   (502) staff       (20)    26850 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/utils/derive_background_opsep.py
+-rw-r--r--   0 regeland   (502) staff       (20)     9358 2023-11-01 17:17:56.000000 fetchsep-0.3.1/fetchsep/utils/fetchsep.cfg
+-rw-r--r--   0 regeland   (502) staff       (20)    13813 2023-11-01 17:17:56.000000 fetchsep-0.3.1/fetchsep/utils/move_output.py
+-rw-r--r--   0 regeland   (502) staff       (20)    23068 2023-06-01 16:15:44.000000 fetchsep-0.3.1/fetchsep/utils/plotting_tools.py
+-rw-r--r--   0 regeland   (502) staff       (20)   120992 2024-05-02 19:40:00.000000 fetchsep-0.3.1/fetchsep/utils/read_datasets.py
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.546106 fetchsep-0.3.1/fetchsep.egg-info/
+-rw-r--r--   0 regeland   (502) staff       (20)     8960 2024-05-02 20:27:43.000000 fetchsep-0.3.1/fetchsep.egg-info/PKG-INFO
+-rw-r--r--   0 regeland   (502) staff       (20)     1480 2024-05-02 20:27:43.000000 fetchsep-0.3.1/fetchsep.egg-info/SOURCES.txt
+-rw-r--r--   0 regeland   (502) staff       (20)        1 2024-05-02 20:27:43.000000 fetchsep-0.3.1/fetchsep.egg-info/dependency_links.txt
+-rw-r--r--   0 regeland   (502) staff       (20)        1 2024-05-02 20:27:43.000000 fetchsep-0.3.1/fetchsep.egg-info/not-zip-safe
+-rw-r--r--   0 regeland   (502) staff       (20)      106 2024-05-02 20:27:43.000000 fetchsep-0.3.1/fetchsep.egg-info/requires.txt
+-rw-r--r--   0 regeland   (502) staff       (20)        9 2024-05-02 20:27:43.000000 fetchsep-0.3.1/fetchsep.egg-info/top_level.txt
+-rw-r--r--   0 regeland   (502) staff       (20)      380 2024-05-02 20:27:43.599557 fetchsep-0.3.1/setup.cfg
+-rw-r--r--   0 regeland   (502) staff       (20)     1863 2024-05-02 20:20:23.000000 fetchsep-0.3.1/setup.py
+drwxr-xr-x   0 regeland   (502) staff       (20)        0 2024-05-02 20:27:43.594484 fetchsep-0.3.1/tests/
+-rw-r--r--   0 regeland   (502) staff       (20)       38 2023-06-01 16:46:50.000000 fetchsep-0.3.1/tests/__init__.py
+-rw-r--r--   0 regeland   (502) staff       (20)      475 2023-09-22 16:34:48.000000 fetchsep-0.3.1/tests/test_config.py
+-rw-r--r--   0 regeland   (502) staff       (20)      439 2023-09-22 16:31:04.000000 fetchsep-0.3.1/tests/test_fetchsep.py
```

### Comparing `fetchsep-0.3.0/CONTRIBUTING.rst` & `fetchsep-0.3.1/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at https://github.com/rickyegeland/fetchsep/issues.
+Report bugs at https://github.com/ktindiana/fetchsep/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
@@ -41,15 +41,15 @@
 Fetch SEP could always use more documentation, whether as part of the
 official Fetch SEP docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/rickyegeland/fetchsep/issues.
+The best way to send feedback is to file an issue at https://github.com/ktindiana/fetchsep/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
@@ -99,15 +99,15 @@
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
 3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
-   https://travis-ci.com/rickyegeland/fetchsep/pull_requests
+   https://travis-ci.com/ktindiana/fetchsep/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `fetchsep-0.3.0/HISTORY.rst` & `fetchsep-0.3.1/HISTORY.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 History
 =======
 
+0.3.1 (2024-05-02)
+------------------
+
+* opsep: modified onset peak fitting and estimate
+* opsep: onset peak changed to max flux if automated algorithm
+  identifies onset after max
+* opsep: better workflow for fetchsep_prepare_obs when starting from
+  BATCH
+* opsep: updates to json output to comply with CCMC schema
+* Bugfix: Fix crash in opsep and idsep on certain python installations
+  when reading in GOES-R data files
+
 0.3.0 (2023-11-02)
 ------------------
 
 * Fixed bug preventing fluence calculation for differential fluxes
 * Improved plots for differential energy channels
 * Added capability to move output produced by `opsep` to a target dir
 * Updated filenames for plots to contain full zulu string
```

### Comparing `fetchsep-0.3.0/LICENSE` & `fetchsep-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/PKG-INFO` & `fetchsep-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fetchsep
-Version: 0.3.0
+Version: 0.3.1
 Summary: Identify SEP elevations above background in a time series (idsep) and analyze events individually (opsep)
-Home-page: https://github.com/rickyegeland/fetchsep
+Home-page: https://github.com/ktindiana/fetchsep
 Author: Kathryn Whitman
 Author-email: kathryn.whitman@nasa.gov
 License: MIT license
 Keywords: fetchsep
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -36,16 +36,16 @@
 FetchSEP
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/fetchsep.svg
         :target: https://pypi.python.org/pypi/fetchsep
 
-.. image:: https://img.shields.io/travis/rickyegeland/fetchsep.svg
-        :target: https://travis-ci.com/rickyegeland/fetchsep
+.. image:: https://img.shields.io/travis/ktindiana/fetchsep.svg
+        :target: https://travis-ci.com/ktindiana/fetchsep
 
 .. image:: https://readthedocs.org/projects/fetchsep/badge/?version=latest
         :target: https://fetchsep.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 
@@ -162,14 +162,26 @@
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 History
 =======
 
+0.3.1 (2024-05-02)
+------------------
+
+* opsep: modified onset peak fitting and estimate
+* opsep: onset peak changed to max flux if automated algorithm
+  identifies onset after max
+* opsep: better workflow for fetchsep_prepare_obs when starting from
+  BATCH
+* opsep: updates to json output to comply with CCMC schema
+* Bugfix: Fix crash in opsep and idsep on certain python installations
+  when reading in GOES-R data files
+
 0.3.0 (2023-11-02)
 ------------------
 
 * Fixed bug preventing fluence calculation for differential fluxes
 * Improved plots for differential energy channels
 * Added capability to move output produced by `opsep` to a target dir
 * Updated filenames for plots to contain full zulu string
```

### Comparing `fetchsep-0.3.0/README.rst` & `fetchsep-0.3.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 FetchSEP
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/fetchsep.svg
         :target: https://pypi.python.org/pypi/fetchsep
 
-.. image:: https://img.shields.io/travis/rickyegeland/fetchsep.svg
-        :target: https://travis-ci.com/rickyegeland/fetchsep
+.. image:: https://img.shields.io/travis/ktindiana/fetchsep.svg
+        :target: https://travis-ci.com/ktindiana/fetchsep
 
 .. image:: https://readthedocs.org/projects/fetchsep/badge/?version=latest
         :target: https://fetchsep.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
```

### Comparing `fetchsep-0.3.0/bin/fetchsep_prepare_obs` & `fetchsep-0.3.1/bin/fetchsep_prepare_obs`

 * *Files 0% similar despite different names*

```diff
@@ -216,19 +216,19 @@
 
 #SECOND ########################
 #Parse the output file created in the previous step. This will
 #rewrite in the correct format to batch run quiet and elevated
 #time periods in OpSEP.
 ################################
 energy_bin = cfg.ref_energy_bin
-septimes_file = septimes_fname(experiment, flux_type, options, energy_bin)
-detector_list = goesfname
 batchfile = 'batch_event_list.txt'
 
 if startpoint == "MAKEFILE" or startpoint == "IDSEP":
+    septimes_file = septimes_fname(experiment, flux_type, options, energy_bin)
+    detector_list = goesfname
     revise = True #add time padding in front of each SEP event
     event_list.make_event_list(str_startdate, str_enddate,
         septimes_file, detector_list,experiment, flux_type,options,
         batchfile, revise)
```

### Comparing `fetchsep-0.3.0/bin/idsep` & `fetchsep-0.3.1/bin/idsep`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/bin/make_opsep_event_list` & `fetchsep-0.3.1/bin/make_opsep_event_list`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/bin/opsep` & `fetchsep-0.3.1/bin/opsep`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/bin/opsep_batch` & `fetchsep-0.3.1/bin/opsep_batch`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/docs/Makefile` & `fetchsep-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/docs/conf.py` & `fetchsep-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/docs/make.bat` & `fetchsep-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/idsep/idsep.py` & `fetchsep-0.3.1/fetchsep/idsep/idsep.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,15 +339,23 @@
     global allow_miss
     allow_miss = max(math.ceil(nconsec/4),1)
     if nconsec == 2 or nconsec == 3: allow_miss = 0
     global dwell_pts
     dwell_pts = max(math.ceil(nconsec/2),2)
     #Rosetta? needs --> dwell_pts = max(math.ceil(nconsec),2)
     
-    print("Requiring " + str(nconsec) + " points (" + str(time_increase/(60.*60.)) + " hours) to define an onset.")
+#    #TO USE THE VALUES IN THE CONFIG FILE
+#    global nconsec
+#    nconsec = cfg.nconsec
+#    global allow_miss
+#    allow_miss = cfg.allow_miss
+#    global dwell_pts
+#    dwell_pts = cfg.dwell_pts
+    
+    print("Requiring " + str(nconsec) + " points (" + str(nconsec*time_res_sec/(60.*60.)) + " hours) to define an onset.")
     print("Allowing " + str(allow_miss) + " points to be missed in onset definition.")
     print("Event ends after " + str(dwell_pts) + " points are below threshold (dwell time).")
                 
     npts = len(dates)
     IsSPE = False
     SPEflag = False
     
@@ -437,15 +445,15 @@
     
     fig = plt.figure(figname,figsize=(12,8))
     plt.rcParams.update({'font.size': 16})
     ax = plt.subplot(111)
     nbins = len(energy_bins)
     ifig = 0
     for i in range(nbins):
-        if (i != 0 and not i%3) or nbins < 3:
+        if (i != 0 and not i%3) or nbins <= 3:
             if saveplot:
                 fig.savefig(plotpath + '/' +figname + '.png')
             figname_plt = figname + str(i)
             fig = plt.figure(figname_plt,figsize=(12,8))
             ax = plt.subplot(111)
             ifig = 0
 
@@ -816,42 +824,43 @@
         prename = 'SEPTimes_' + exp_name + '_' + flux_type + modifier
     
     #####WRITE SEP DATES OUT TO FILE INSTEAD OF PRINTING##########
     for j in range(len(SEPstart)):
         fname = outpath + "/" + prename + '_' + str(energy_bins[j][0]) + '_to_'\
                 + str(energy_bins[j][1]) + '.txt'
         outfile = open(fname,"w")
-        outfile.write("#SEP times calculated by SEPAutoID\n")
+        outfile.write("#SEP times calculated by idsep\n")
         if experiment == "user" and exp_name != '':
             outfile.write("#Experiment: " + exp_name + "\n")
         else:
             outfile.write("#Experiment: " + experiment + "\n")
         outfile.write("#Flux type: " + flux_type + "\n")
         outfile.write("#Energy channel: " + str(energy_bins[j][0]) \
                     + " - " + str(energy_bins[j][1]) + "\n")
         outfile.write("#Selected options: " + str(options) + "\n")
         outfile.write("#Searched date range: " + str_stdate + " to "\
                     + str_enddate + "\n")
         outfile.write("#User applied an initial cut of " + str(remove_above)
                 + ", initial averaging window of " + str(init_win) + " days"
                 + ", final threshold with a sliding window of "
                 + str(sliding_win) + " days\n")
+        outfile.write("#The percentage of points in the sliding window that must be "
+                "background was " + str(cfg.percent_points) + "\n")
         outfile.write("#Threshold defined as mean background + " + str(nsigma)
                 + " x sigma\n")
         outfile.write("#SEPs were identified when " + str(nconsec) + " points "
                 + " exceeded threshold, allowing up to " + str(allow_miss)
                 + " points to be missed. The SEP event ended after " +
                 str(dwell_pts) + " were below threshold (dwell time).\n")
         outfile.write("#Start Time    End Time\n")
         
         for k in range(len(SEPstart[j])):
             SEPst = SEPstart[j][k]
             SEPed = SEPend[j][k]
             if for_inclusive:
-                SEPst = SEPst - one_sec
                 SEPed = SEPed - one_sec
             outfile.write(str(SEPst) + " " + str(SEPed) + "\n")
             
         outfile.close()
 
     
     
@@ -914,29 +923,31 @@
         prename = 'HighPoints_' + exp_name + '_' + flux_type + modifier
     
     #####WRITE SEP DATES OUT TO FILE INSTEAD OF PRINTING##########
     for j in range(len(fluxes_high)):
         fname = outpath + "/" + prename + '_' + str(energy_bins[j][0]) + '_to_'\
                 + str(energy_bins[j][1]) + '.txt'
         outfile = open(fname,"w")
-        outfile.write("#All high points above mean background + 3*sigma calculated by SEPAutoID\n")
+        outfile.write("#All high points above mean background + 3*sigma calculated by idsep\n")
         if experiment == "user" and exp_name != '':
             outfile.write("#Experiment: " + exp_name + "\n")
         else:
             outfile.write("#Experiment: " + experiment + "\n")
         outfile.write("#Flux type: " + flux_type + "\n")
         outfile.write("#Energy channel: " + str(energy_bins[j][0]) \
                     + " - " + str(energy_bins[j][1]) + "\n")
         outfile.write("#Selected options: " + str(options) + "\n")
         outfile.write("#Searched date range: " + str_stdate + " to "\
                     + str_enddate + "\n")
         outfile.write("#User applied an initial cut of " + str(remove_above)
                 + ", initial averaging window of " + str(init_win) + " days"
                 + ", final threshold with a sliding window of "
                 + str(sliding_win) + " days\n")
+        outfile.write("#The percentage of points in the sliding window that must be "
+                "background was " + str(cfg.percent_points) + "\n")
         outfile.write("#Threshold defined as mean background + " + str(nsigma)
                 + " x sigma\n")
         outfile.write("#High flux points were identified when flux values "
                     "exceeded mean background flux + 3*sigma "
                     "by applying a " + str(sliding_win) + " days "
                     "backward sliding window to estimate the background levels.\n")
         outfile.write("#Start Time    End Time\n")
```

### Comparing `fetchsep-0.3.0/fetchsep/idsep/make_event_list.py` & `fetchsep-0.3.1/fetchsep/idsep/make_event_list.py`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/json/ccmc_json_handler.py` & `fetchsep-0.3.1/fetchsep/json/ccmc_json_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from datetime import timedelta
 import copy
 import zulu
 from astropy import units as u
 import os
 import sys
 
-__version__ = "1.9"
+__version__ = "2.0"
 __author__ = "Katie Whitman"
 __maintainer__ = "Katie Whitman"
 __email__ = "kathryn.whitman@nasa.gov"
 
 
 #2021-01-12 changes in v0.2: Added fluence to json file. Added threshold
 #   crossing entry for end of event.
@@ -91,14 +91,19 @@
 #   the json. In the context of this code, may be most useful to add
 #   the trigger information and change the issue time.
 #2023-7-06, changes in 1.8: cast max flux as float in fill_json
 #   because found that models with 0 flux resulted in an error
 #   when dumping json.
 #2023-10-01, changes in 1.9: Added subroutines to transform
 #   threshold and energy channels to string keys.
+#2024-04-24, changes in 2.0: Made changes to accomodate new fields
+#   from CCMC. "model": {"flux_type": } --> "source_info": {"native_flux_type":}
+#   Modified clean_json to remove the options field if nothing added.
+#   Changed event_lengths threshold field to threshold_start and added
+#   threshold_end.
 
 def about_ccmc_json_handler():
     """ ABOUT ccmc_json_handler.py
     
         This module places all derived information into json and supporting
         files that follow the format specified for CCMC's SEP Scoreboard.
         https://ccmc.gsfc.nasa.gov/challenges/sep.php#format
@@ -324,25 +329,25 @@
     #For now, assume a user-input file is model output
     #This is not generic and should be modified in the future
     if experiment == "user" and json_type == "model":
         key = keys.model_main
         type_key = keys.model_type
         win_key = keys.model_win
         template[key]['model']['short_name'] = model_name
-        template[key]['model']['flux_type'] = flux_type
+        template[key]['source_info']['native_flux_type'] = flux_type
         template[key]['model']['spase_id'] = spase_id
                         
     else:
         key = keys.obs_main
         type_key = keys.obs_type
         win_key = keys.obs_win
         template[key][keys.obs_exp]['short_name'] = experiment
         if experiment == "user" and model_name != "":
                 template[key][keys.obs_exp]['short_name'] = model_name
-        template[key][keys.obs_exp]['flux_type'] = flux_type
+        template[key]['source_info']['native_flux_type'] = flux_type
         if spase_id != "":
             template[key]['observatory']['spase_id'] = spase_id
 
     template[key]['options'] = options
     template[key]['issue_time'] = issue_time
 
     template[key]['notes'].append({'note':"opsep v" + str(opsep_version)})
@@ -444,15 +449,16 @@
             #Maximum Flux
             max_dict = {"intensity":float(peak_flux[i]),"time": zpdate,
                             "units":flux_units}
             template[key][type_key][tidx]['peak_intensity_max'].update(max_dict)
             
             #Start and End Times
             length_dict = { "start_time": zct,  "end_time": zeet,
-                            "threshold": flux_thresholds[i],
+                            "threshold_start": flux_thresholds[i],
+                            "threshold_end": flux_thresholds[i]*cfg.endfac,
                             "threshold_units": flux_units }
             if template[key][type_key][tidx]['event_lengths'][0]['start_time']\
                 == "":
                 template[key][type_key][tidx]['event_lengths'][0].update(length_dict)
             else:
                 template[key][type_key][tidx]['event_lengths'].append(length_dict)
             
@@ -599,14 +605,18 @@
         type_key = keys.obs_type
         win_key = keys.obs_win
 
         spase_id = template[key]['observatory']['spase_id']
         if spase_id != "":
             template[key]['observatory'].pop('spase_id', None)
 
+    options = template[key]['options']
+    if options == [""]:
+        template[key].pop('options', None)
+
     nent = len(template[key][type_key])
     for i in range(nent-1,-1,-1):
         #Onset Peak Flux
         if template[key][type_key][i]['peak_intensity']['intensity'] == "":
             template[key][type_key][i].pop('peak_intensity', None)
         
         #Maximum Flux
```

### Comparing `fetchsep-0.3.0/fetchsep/json/keys.py` & `fetchsep-0.3.1/fetchsep/json/keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..utils import config as cfg
 
-__version__ = "0.4"
+__version__ = "0.5"
 __author__ = "Katie Whitman"
 __maintainer__ = "Katie Whitman"
 __email__ = "kathryn.whitman@nasa.gov"
 
 #2021-07-23, Changes in 0.2: Remove the contacts fields due to
 #   NASA privacy rules.
 #   Updating to follow updated CCMC JSON format. This version
@@ -12,14 +12,16 @@
 #2021-08-18, Changes in 0.3: added identifiers for all of the possible
 #   fields in the json files produced by operational_sep_quantities.py
 #   or that may be produced by models for the CCMC SEP Scoreboard.
 #   This code matches the same version of the code in the validation
 #   project library. Must keep both of these version matched and
 #   up-to-date with each other.
 #2023-04-18, changes in 0.4: Adding keys for triggers.
+#2024-04-24, changes in 0.5: changed event_lengths threshold to
+#   threshold_start to reflect CCMC's SEP Scoreboard format
 
 def about_keys():
     """ About keys.py
     
         This version of keys.py is maintained in the operational-sep
         project.
     
@@ -435,15 +437,15 @@
     if value == id_event_lengths:
         key_chain = ['event_lengths']                    #--> array of dictionaries
     if value == id_event_length_start_time:
         key_chain = ['event_lengths',index,'start_time']#--> string zulu time
     if value == id_event_length_end_time:
         key_chain = ['event_lengths',index,'end_time']  #--> string zulu time
     if value == id_event_length_threshold:
-        key_chain = ['event_lengths',index,'threshold'] #--> float
+        key_chain = ['event_lengths',index,'threshold_start'] #--> float
     if value == id_event_length_threshold_units:
         key_chain = ['event_lengths',index,'threshold_units'] #--> string
         
     if value == id_threshold_crossings:
         key_chain = ['threshold_crossings']              #--> array of dictionaries
     if value == id_thresh_crossing_time:
         key_chain = ['threshold_crossings',index,'crossing_time'] #--> string zulu time
```

### Comparing `fetchsep-0.3.0/fetchsep/json/read_json_example.py` & `fetchsep-0.3.1/fetchsep/json/read_json_example.py`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/json/templates/model_example.json` & `fetchsep-0.3.1/fetchsep/json/templates/model_example.json`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/json/templates/model_template.json` & `fetchsep-0.3.1/fetchsep/json/templates/observations_template.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('sep_observation_submission', OrderedDict([('notes', "*

 * *            "[OrderedDict([('note', 'produced by fetchsep/opsep.py')])]), ('observatory', "*

 * *            "OrderedDict([('short_name', ''), ('spase_id', '')])), ('source_info', "*

 * *            "OrderedDict([('native_flux_type', '')])), ('options', ''), ('issue_time', ''), "*

 * *            "('mode', 'measurement'), ('observations', [OrderedDict([('energy_channel', "*

 * *            "OrderedDict([('min', 10), ('max', -1), ('units', 'MeV')] […]*

```diff
@@ -1,10 +1,17 @@
 {
-    "sep_forecast_submission": {
-        "forecasts": [
+    "sep_observation_submission": {
+        "issue_time": "",
+        "mode": "measurement",
+        "notes": [
+            {
+                "note": "produced by fetchsep/opsep.py"
+            }
+        ],
+        "observations": [
             {
                 "all_clear": {
                     "all_clear_boolean": "",
                     "threshold": "",
                     "threshold_units": ""
                 },
                 "energy_channel": {
@@ -12,15 +19,16 @@
                     "min": 10,
                     "units": "MeV"
                 },
                 "event_lengths": [
                     {
                         "end_time": "",
                         "start_time": "",
-                        "threshold": "",
+                        "threshold_end": "",
+                        "threshold_start": "",
                         "threshold_units": ""
                     }
                 ],
                 "fluence_spectra": [
                     {
                         "end_time": "",
                         "fluence_spectrum": [
@@ -40,28 +48,28 @@
                 "fluences": [
                     {
                         "fluence": "",
                         "units": ""
                     }
                 ],
                 "location": "earth",
+                "observation_window": {
+                    "end_time": "",
+                    "start_time": ""
+                },
                 "peak_intensity": {
                     "intensity": "",
                     "time": "",
                     "units": ""
                 },
                 "peak_intensity_max": {
                     "intensity": "",
                     "time": "",
                     "units": ""
                 },
-                "prediction_window": {
-                    "end_time": "",
-                    "start_time": ""
-                },
                 "sep_profile": "",
                 "species": "proton",
                 "threshold_crossings": [
                     {
                         "crossing_time": "",
                         "threshold": "",
                         "threshold_units": ""
@@ -107,47 +115,42 @@
                 "fluences": [
                     {
                         "fluence": "",
                         "units": ""
                     }
                 ],
                 "location": "earth",
+                "observation_window": {
+                    "end_time": "",
+                    "start_time": ""
+                },
                 "peak_intensity": {
                     "intensity": "",
                     "time": "",
                     "units": ""
                 },
                 "peak_intensity_max": {
                     "intensity": "",
                     "time": "",
                     "units": ""
                 },
-                "prediction_window": {
-                    "end_time": "",
-                    "start_time": ""
-                },
                 "sep_profile": "",
                 "species": "proton",
                 "threshold_crossings": [
                     {
                         "crossing_time": "",
                         "threshold": "",
                         "threshold_units": ""
                     }
                 ]
             }
         ],
-        "issue_time": "",
-        "mode": "historical",
-        "model": {
-            "flux_type": "",
+        "observatory": {
             "short_name": "",
             "spase_id": ""
         },
-        "notes": [
-            {
-                "note": "produced by fetchsep/opsep.py"
-            }
-        ],
-        "options": ""
+        "options": "",
+        "source_info": {
+            "native_flux_type": ""
+        }
     }
 }
```

### Comparing `fetchsep-0.3.0/fetchsep/json/templates/observations_example.json` & `fetchsep-0.3.1/fetchsep/json/templates/observations_example.json`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/json/templates/observations_template.json` & `fetchsep-0.3.1/fetchsep/json/templates/model_template.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('sep_forecast_submission', OrderedDict([('notes', "*

 * *            "[OrderedDict([('note', 'produced by fetchsep/opsep.py')])]), ('model', "*

 * *            "OrderedDict([('short_name', ''), ('spase_id', '')])), ('source_info', "*

 * *            "OrderedDict([('native_flux_type', '')])), ('options', ''), ('issue_time', ''), "*

 * *            "('mode', 'historical'), ('forecasts', [OrderedDict([('energy_channel', "*

 * *            "OrderedDict([('min', 10), ('max', -1), ('units', 'MeV')])), ('species […]*

```diff
@@ -1,17 +1,10 @@
 {
-    "sep_observation_submission": {
-        "issue_time": "",
-        "mode": "measurement",
-        "notes": [
-            {
-                "note": "produced by fetchsep/opsep.py"
-            }
-        ],
-        "observations": [
+    "sep_forecast_submission": {
+        "forecasts": [
             {
                 "all_clear": {
                     "all_clear_boolean": "",
                     "threshold": "",
                     "threshold_units": ""
                 },
                 "energy_channel": {
@@ -19,15 +12,16 @@
                     "min": 10,
                     "units": "MeV"
                 },
                 "event_lengths": [
                     {
                         "end_time": "",
                         "start_time": "",
-                        "threshold": "",
+                        "threshold_end": "",
+                        "threshold_start": "",
                         "threshold_units": ""
                     }
                 ],
                 "fluence_spectra": [
                     {
                         "end_time": "",
                         "fluence_spectrum": [
@@ -47,28 +41,28 @@
                 "fluences": [
                     {
                         "fluence": "",
                         "units": ""
                     }
                 ],
                 "location": "earth",
-                "observation_window": {
-                    "end_time": "",
-                    "start_time": ""
-                },
                 "peak_intensity": {
                     "intensity": "",
                     "time": "",
                     "units": ""
                 },
                 "peak_intensity_max": {
                     "intensity": "",
                     "time": "",
                     "units": ""
                 },
+                "prediction_window": {
+                    "end_time": "",
+                    "start_time": ""
+                },
                 "sep_profile": "",
                 "species": "proton",
                 "threshold_crossings": [
                     {
                         "crossing_time": "",
                         "threshold": "",
                         "threshold_units": ""
@@ -114,40 +108,49 @@
                 "fluences": [
                     {
                         "fluence": "",
                         "units": ""
                     }
                 ],
                 "location": "earth",
-                "observation_window": {
-                    "end_time": "",
-                    "start_time": ""
-                },
                 "peak_intensity": {
                     "intensity": "",
                     "time": "",
                     "units": ""
                 },
                 "peak_intensity_max": {
                     "intensity": "",
                     "time": "",
                     "units": ""
                 },
+                "prediction_window": {
+                    "end_time": "",
+                    "start_time": ""
+                },
                 "sep_profile": "",
                 "species": "proton",
                 "threshold_crossings": [
                     {
                         "crossing_time": "",
                         "threshold": "",
                         "threshold_units": ""
                     }
                 ]
             }
         ],
-        "observatory": {
-            "flux_type": "",
+        "issue_time": "",
+        "mode": "historical",
+        "model": {
             "short_name": "",
             "spase_id": ""
         },
-        "options": ""
+        "notes": [
+            {
+                "note": "produced by fetchsep/opsep.py"
+            }
+        ],
+        "options": "",
+        "source_info": {
+            "native_flux_type": ""
+        }
     }
 }
```

### Comparing `fetchsep-0.3.0/fetchsep/json/templates/triggers_template.json` & `fetchsep-0.3.1/fetchsep/json/templates/triggers_template.json`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/opsep/batch_run_opsep.py` & `fetchsep-0.3.1/fetchsep/opsep/batch_run_opsep.py`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/opsep/opsep.py` & `fetchsep-0.3.1/fetchsep/opsep/opsep.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import pandas as pd
 import scipy
 from scipy import signal
 from statistics import mode
 from lmfit import minimize, Parameters
 import array
 
-__version__ = "3.4"
+__version__ = "3.7"
 __author__ = "Katie Whitman"
 __maintainer__ = "Katie Whitman"
 __email__ = "kathryn.whitman@nasa.gov"
 
 ################ CHANGE LOG ####################
 #CHANGES in 0.4: allows users to specify user model or experiment name for
 #output files
@@ -301,14 +301,28 @@
 #   has dropped below threshold for longer than the dwell time, then choose the
 #   end time as the first below below threshold. endfac should be set to 1.0 in
 #   config.py to ensure the end of the event applies the same threshold as the
 #   start of the event.
 #2023-09-30, changes in v3.4: Changed filenames of plots to contain zulu
 #   time for starting window or threshold crossing time so that they
 #   are unique.
+#2024-02-09, changes in v3.5: Changed onset peak fitting algorithm. Added
+#   logic that identifies large and small events and handles them a little
+#   differently as far as the time range for applying the fit. For lower
+#   intensity events, added logic that attempts to identify when the first
+#   increase above background occurred (defined as a set flux threshold,
+#   currently will only be useful for integral fluxes) and extends the fit
+#   time range closer to that initial increase to capture more of the onset.
+#2024-03-11, changes in v3.6: If onset peak time is calculated to be after the
+#   maximum flux time, then choose to set the onset peak to the same point
+#   as the max flux.
+#2024-04-24, changes in v3.7: The json templates and ccmc_json_handler
+#   were changed to reflect CCMC's schema.
+#   "model":{"flux_type":} --> "source_info":{"native_flux_type":}
+#   "event_lengths": [{"threshold":}] --> "event_lengths": [{"threshold_start":}]
 ########################################################################
 
 #See full program description in all_program_info() below
 datapath = cfg.datapath
 outpath = cfg.outpath + "/opsep"
 plotpath = cfg.plotpath + "/opsep"
 badval = cfg.badval #bad data points will be set to this value; must be negative
@@ -1866,66 +1880,77 @@
             ax2.set_ylabel("Derivative")
             plt.show()
 
     return onset_date, onset_peak
 
 
 
+def residual(fit, data):
+    """ Calculate difference between fit and data.
+    
+    """
+    
+    resid = []
+    for i in range(len(fit)):
+        resid.append(data[i] - fit[i])
+    
+    return resid
+
+
 def modified_weibull(times, Ip, a, b):
     """ Create a Weibull for times in seconds since first
         date with params a and b.
         
     """
     
     weibull = []
     for t in times:
         W = Ip*(-a/b)*(t/b)**(a-1)*math.exp(-(t/b)**a)
         weibull.append(W)
         
     return weibull
 
 
-
-def residual(fit, data):
-    """ Calculate difference between fit and data.
-    
+def lognormal(times, Ip, a, b):
+    """ Create a lognormal fit for times in seconds since first
+        date with params a and b. (a=sigma and b=mu)
+        
     """
     
-    resid = []
-    for i in range(len(fit)):
-        resid.append(data[i] - fit[i])
-    
-    return resid
-    
+    func = []
+    for t in times:
+        LN = Ip/(t*a*(2.*math.pi)**0.5) * math.exp(-((math.log(t)-b)**2)/(2*a**2))
+        func.append(LN)
+        
+    return func
 
 
-def weibull_residual(params, *args):
+def func_residual(params, *args):
     """ Caluate the residual of the Weibull fit
         compared to data.
         
     """
     
     pars = params.valuesdict()
     a = pars['alpha']
     b = pars['beta']
     Ip = pars['peak_intensity']
     
-    #print('Generating Weibull Ip: ' + str(Ip) + ', a: ' + str(a) + ', b: ' + str(b))
     times = args[0]
     data = args[1]
     
     fit = modified_weibull(times, Ip, a, b)
+#    fit = lognormal(times, Ip, a, b)
     
     resid = residual(fit, data)
 
     return resid
     
 
 
-
 def find_max_curvature(x, y, energy_threshold, crossing_time,
         experiment, showplot, saveplot):
     """ Calculate the curvature along a curve
         and find the maximum curvature location.
         
         https://undergroundmathematics.org/glossary/curvature
         
@@ -1951,16 +1976,16 @@
     if showplot or saveplot:
         tzulu = ccmc_json.make_ccmc_zulu_time(crossing_time)
         tzulu = tzulu.replace(":","")
         figname = tzulu + "_" + "SecondDerivative_" + experiment + "_"\
                 + str(energy_threshold) + "MeV"
         fig = plt.figure(figname,figsize=(9,5))
         plt.plot(xarr,yarr,label="orig")
-        plt.plot(xarr[max_k_idx+2], yarr[max_k_idx+2],"o",label="Min 2nd Derivative on Weibull")
-        plt.plot(xarr[max_y_idx], yarr[max_y_idx],"o",label="max Weibull")
+        plt.plot(xarr[max_k_idx+2], yarr[max_k_idx+2],"o",label="Min 2nd Derivative on Fit")
+        plt.plot(xarr[max_y_idx], yarr[max_y_idx],"o",label="max Fit")
         plt.plot(xarr[2:],k_x,label="2nd Derivative")
         plt.plot(xarr[max_k_idx+2],k_x[max_k_idx],"o",label="Min 2nd Derivative")
         plt.legend(loc='lower left')
         plt.xlabel("Hours")
         plt.ylabel("Y")
         #plt.yscale("log")
         #plt.ylim(1e-4,1e6)
@@ -1970,17 +1995,40 @@
             plt.close(fig)
 
         
     return max_k_idx+2
 
 
 
+def get_thresh_cross_time(dates,fluxes,thresh):
+    """ For a given threshold value, find the first time that
+        the flux exceeds (or is equal to) that value;
+        
+        INPUT:
+        
+            :dates: (datetime array)
+            :fluxes: (float array 1xn)
+            :thresh: (float) threshold value
+            
+        OUTPUT:
+        
+            (datetime) time that threshold was crossed
+            
+    """
+
+    for i in range(len(fluxes)):
+        if fluxes[i] >= thresh:
+            return dates[i]
+            
+    return 0
+
 
-def calculate_onset_peak_from_fit(experiment, energy_thresholds, dates, integral_fluxes,
-                crossing_time, event_end_time, showplot, saveplot):
+def calculate_onset_peak_from_fit(experiment, energy_thresholds,
+    flux_thresholds, dates, integral_fluxes, crossing_time, event_end_time,
+    showplot, saveplot):
     """ Calculate the peak associated with the initial SEP onset. This subroutine
         searches for the rollover that typically occurs after the SEP onset.
         The peak value will be specified as the flux value at the rollover
         location.
         The onset peak may provide a more physically appropriate comparison
         with models.
         If code cannot identify onset peak, it will return a value of 0 on
@@ -1998,16 +2046,18 @@
         A least 6 hours of flux measurements are required to fit the Weibull.
         If the duration of the time profile is shorter, then the onset peak
         will not be calcualated.
         
         INPUTS:
         
         :experiment: (string) e.g. GOES-13
-        :energy_thresholds: (float 1xn array) - energy channels for which thresholds
-            are applied
+        :energy_thresholds: (float 1xn array) - energy channels for which
+            thresholds are applied
+        :flux_thresholds: (float 1xn array) - flux threshold applied to
+            associated energy channel
         :dates: (datetime 1xm array) - dates associated with flux time profile
         :integral_fluxes: (float nxm array) - fluxes for each energy channel for
             which a threshold is applied; each is the same length as dates
         :crossing_time: (datetime 1xn array) - threshold crossing times for each energy
             channel for which a threshold is applied
         :event_end_time: (datetime 1xn array) - end times for each energy channel for which
             a threshold is applied
@@ -2036,57 +2086,102 @@
     onset_date = [[]]*nthresh
     onset_peak = [[]]*nthresh
     
     #Convert dates into a series of times in hours for fitting
     times = [((t - dates[0]).total_seconds() + 60)/(60*60) for t in dates]
     
     #Do a fit of the Weibull function for each time profile
-    params_weib = Parameters()
-    params_weib.add('alpha', value = -3, min = -5, max = -0.1)
-    params_weib.add('beta', value = 10, min = 1, max =100)
-    params_weib.add('peak_intensity', value = 100, min = 1e-3, max =1e6)
+    params_fit = Parameters()
+    params_fit.add('alpha', value = -3, min = -5, max = -0.1)
+    params_fit.add('beta', value = 10, min = 1, max =100)
+    params_fit.add('peak_intensity', value = 100, min = 1e-3, max =1e6)
+    
+    #Lognormal Parameters
+#    params_fit = Parameters()
+#    params_fit.add('alpha', value = 1, min = 0.1, max = 5)
+#    params_fit.add('beta', value = 2, min = 0.1, max = 10)
+#    params_fit.add('peak_intensity', value = 100, min = 1e-3, max =1e6)
     
     for i in range(nthresh):
         if crossing_time[i] == 0: continue
         
+        #Attempt to refine the fit start point, particularly in the cases
+        #where the event was very gradual and just barely crossed threshold.
+        #The initial increase above background may have started many hours
+        #prior to the official threshold crossing and the onset peak
+        #may be many hours prior to the threshold crossing in that case.
+        #If an event has low fluxes, then apply a threshold closer to the
+        #background and extend the fit to try to better capture the onset.
+        #If an event has very high fluxes, then there is plenty of values
+        #above threshold to fit and don't need to extend back so far.
+        flxratio = max(integral_fluxes[i])/flux_thresholds[i]
+        print("Ratio of max flux " + str(max(integral_fluxes[i])) + " to threshold " + str(flux_thresholds[i]) + " is " + str(flxratio))
+        #For mid to strong SEP events, time according to prompt onset and the
+        #possibility of a CME arriving around 24 hours later (set timing
+        #to approximately exclude CME arrival)
+        start_fit_time = crossing_time[i] - datetime.timedelta(hours=3)
+        end_fit_time = crossing_time[i] + datetime.timedelta(hours=24)
+
+        #For lower intensity events, extend back to initial elevation to
+        #capture more of the event and also capture more time
+        #after threshold crossing as likely a slower CME or CME that
+        #will not arrive at Earth (for very gradual rises)
+        if flxratio < 10:
+            low_thresh = 0.5 #integral flux, > GOES bg
+            low_cross_time =\
+                get_thresh_cross_time(dates,integral_fluxes[i],low_thresh)
+            print("Crossing Time above thresh: " + str(low_thresh) + " is " + str(low_cross_time))
+            
+            start_fit_time = crossing_time[i] - datetime.timedelta(hours=3)
+            end_fit_time = min(event_end_time[i],crossing_time[i] + datetime.timedelta(hours=36))
+            if low_cross_time != 0:
+                #Try options for fit times
+                td = [6, 8, 12, 16, 20, 24, 28]
+                for tm in td:
+                    delta = datetime.timedelta(hours=tm)
+                    if low_cross_time < (crossing_time[i] - delta):
+                        start_fit_time = crossing_time[i] - delta
+
         #Fit only to fluxes starting at crossing time up to 24
         #hours afterwards
-        fit_st = crossing_time[i] - datetime.timedelta(hours=6)
+        fit_st = start_fit_time
         fit_end = crossing_time[i] + datetime.timedelta(hours=24)
+        print("FITTING BETWEEN " + str(fit_st) + " to " + str(fit_end))
         trim_fluxes = []
         trim_times = []
         trim_dates = []
         for j in range(len(dates)):
             if dates[j] >= fit_st and dates[j] <= fit_end:
                 trim_fluxes.append(integral_fluxes[i][j])
                 trim_times.append(times[j])
                 trim_dates.append(dates[j])
         
         #log_fluxes = [math.log10(f) for f in integral_fluxes[i]]
-        minimize_weib = minimize(weibull_residual, params_weib,
+        minimize_func = minimize(func_residual, params_fit,
                     args = [trim_times, trim_fluxes],
                     nan_policy= 'propagate', max_nfev=np.inf)
         
-        best_pars = minimize_weib.params.valuesdict()
+        best_pars = minimize_func.params.valuesdict()
         best_a = best_pars['alpha']
         best_b = best_pars['beta']
         best_Ip = best_pars['peak_intensity']
-        best_weibull = modified_weibull(trim_times, best_Ip, best_a, best_b)
+        best_fit = modified_weibull(trim_times, best_Ip, best_a, best_b)
+#        best_fit = lognormal(trim_times, best_Ip, best_a, best_b)
         print("calculate_onset_peak_from_fit ==== "
                 + str(energy_thresholds[i]) + " MeV =====")
-        print('Best Fit Weibull Ip: ' + str(best_Ip) + ', a: ' + str(best_a) + ', b: ' + str(best_b))
+        print('Best Fit Ip: ' + str(best_Ip) + ', a: ' + str(best_a) + ', b: ' + str(best_b))
         
         ####FIND ONSET PEAK USING MAXIMUM CURVATURE ON WEIBULL FIT
-        max_curve_idx = find_max_curvature(trim_times, best_weibull,
+        max_curve_idx = find_max_curvature(trim_times, best_fit,
                             energy_thresholds[i], crossing_time[i],
                             experiment, showplot, saveplot)
 
         max_curve_model_time = trim_times[max_curve_idx]
         max_curve_model_date = trim_dates[max_curve_idx]
-        max_curve_model_peak = best_weibull[max_curve_idx]
+        max_curve_model_peak = best_fit[max_curve_idx]
         
         #Pull out max measured value around the maximum of curvature
         max_curve_meas_peak = 0
         max_curve_meas_time = 0
         max_curve_meas_date = 0
         dt = datetime.timedelta(hours=1)
         for k in range(len(trim_dates)):
@@ -2098,16 +2193,16 @@
                     max_curve_meas_date = trim_dates[k]
 
         
         onset_date[i] = max_curve_meas_date
         onset_peak[i] = max_curve_meas_peak
         
         ####FIND PEAK BY JUST TAKING MAXIMUM OF WEIBULL
-        max_val = np.max(best_weibull)
-        max_idx = np.where(best_weibull == max_val)
+        max_val = np.max(best_fit)
+        max_idx = np.where(best_fit == max_val)
         max_time = trim_times[max_idx[0][0]]
         
         #Pull out max measured value around this identified maximum in the fit
         model_max_date = datetime.timedelta(seconds=(max_time*60*60 - 60)) + dates[0]
         max_meas = 0
         max_meas_time = 0
         max_date = 0
@@ -2116,38 +2211,33 @@
             if trim_dates[k] >= model_max_date - dt and trim_dates[k] <= model_max_date + dt:
                 if trim_fluxes[k] > max_meas:
                     max_meas = trim_fluxes[k]
                     max_meas_time = trim_times[k]
                     max_date = trim_dates[k]
         
         
-        #onset_date[i] = max_date
-        #onset_peak[i] = max_meas
-        
-        
-        
         if showplot or saveplot:
             tzulu = ccmc_json.make_ccmc_zulu_time(crossing_time[i])
             tzulu = tzulu.replace(":","")
-            figname = tzulu + "_Weibull_fit_"+ experiment + "_" \
+            figname = tzulu + "_profile_fit_"+ experiment + "_" \
                     + str(energy_thresholds[i]) + "MeV"
             fig = plt.figure(figname,figsize=(9,5))
             label = ">" + str(energy_thresholds[i]) + " MeV"
             plt.plot(trim_times,trim_fluxes,label=label)
-            label_weib = "Weibull\n Ip: " + str(best_Ip) \
+            label_fit = "Fit\n Ip: " + str(best_Ip) \
                         + "\n alpha: " + str(best_a) \
                         +"\n beta: " + str(best_b)
-            plt.plot(trim_times,best_weibull,label=label_weib)
-            plt.plot(max_time, max_val,"o",label="max Weibull")
-            plt.plot(max_meas_time, max_meas,">",label="measured peak near Weibull max")
+            plt.plot(trim_times,best_fit,label=label_fit)
+            plt.plot(max_time, max_val,"o",label="max fit")
+            plt.plot(max_meas_time, max_meas,">",label="measured peak near fit max")
             plt.plot(max_curve_model_time, max_curve_model_peak,"D",label="Min 2nd Derivative")
             plt.plot(max_curve_meas_time, max_curve_meas_peak,"^",label="measured peak near min 2nd Derivative")
             #plt.plot(onset_time, onset_peak[i],">",label="onset Weibull")
             plt.legend(loc='lower right')
-            plt.title("Weibull Fit to Find Onset Peak for " + experiment
+            plt.title("Fit to Find Onset Peak for " + experiment
                         +"\n " + str(crossing_time[i]))
             plt.xlabel("Hours")
             plt.ylabel("Intensity")
             plt.yscale("log")
             plt.ylim(1e-4,1e6)
             
             if saveplot:
@@ -3262,16 +3352,22 @@
                                  options, doBGSub,
                                  model_name, input_threshold[i][0],
                                  input_threshold[i][1], sep_d, sep_f,
                                  energy_bins, is_diff_thresh[i], True) #savefile
                 bin_fl = fl[svbin] #fluence for bin associated with threshold
                 
                 od,op=calculate_onset_peak_from_fit(experiment, energy_thresh,
-                            dates, in_flx, ct, eet, showplot, saveplot)
-
+                        flux_thresh, dates, in_flx, ct, eet, showplot, saveplot)
+                #If the onset peak is after the maximum flux, set the onset peak
+                #to the same point as the maximum flux
+                if isinstance(od[0],datetime.date) and isinstance(pt[0], datetime.date):
+                    if od[0] > pt[0]:
+                        od = pt
+                        op = pf
+                    
                 if umasep:
                     umasep_t, umasep_f = calculate_umasep_info(\
                                 [input_threshold[i][0]],[input_threshold[i][1]],
                                 dates, [fluxes[svbin]], ct)
                     umasep_times.append(umasep_t[0]) #One channel at a time
                     umasep_fluxes.append(umasep_f[0]) #so only one element in array
 
@@ -3564,16 +3660,25 @@
     #integral fluxes are used to define event start and stop
     crossing_time,peak_flux,peak_time,rise_time,event_end_time,duration=\
         calculate_event_info(energy_thresholds,flux_thresholds, dates,
                     integral_fluxes, detect_prev_event, two_peaks, False)
                     #Always integral fluxes here, so False
 
     #Calculate onset peak for all thresholds
-    onset_date, onset_peak = calculate_onset_peak_from_fit(experiment, energy_thresholds,
-                dates, integral_fluxes, crossing_time, event_end_time, showplot, saveplot)
+    onset_date, onset_peak = calculate_onset_peak_from_fit(experiment,
+        energy_thresholds, flux_thresholds, dates, integral_fluxes, crossing_time,
+        event_end_time, showplot, saveplot)
+        
+        
+    #If onset_date is after peak_time, then set the onset peak to the max flux point
+    for ii in range(len(peak_time)):
+        if isinstance(onset_date[ii], datetime.date) and isinstance(peak_time[ii],datetime.date):
+            if onset_date[ii] > peak_time[ii]:
+                onset_date[ii] = peak_time[ii]
+                onset_peak[ii] = peak_flux[ii]
 
     #Calculate times used in UMASEP
     umasep_times =[]
     umasep_fluxes=[]
     if umasep:
         umasep_times, umasep_fluxes = calculate_umasep_info(energy_thresholds,
                         flux_thresholds, dates, integral_fluxes, crossing_time)
```

### Comparing `fetchsep-0.3.0/fetchsep/utils/config.py` & `fetchsep-0.3.1/fetchsep/utils/config.py`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/utils/date_handler.py` & `fetchsep-0.3.1/fetchsep/utils/date_handler.py`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/utils/define_background_idsep.py` & `fetchsep-0.3.1/fetchsep/utils/define_background_idsep.py`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/utils/derive_background_opsep.py` & `fetchsep-0.3.1/fetchsep/utils/derive_background_opsep.py`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/utils/fetchsep.cfg` & `fetchsep-0.3.1/fetchsep/utils/fetchsep.cfg`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/utils/move_output.py` & `fetchsep-0.3.1/fetchsep/utils/move_output.py`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/utils/plotting_tools.py` & `fetchsep-0.3.1/fetchsep/utils/plotting_tools.py`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/fetchsep/utils/read_datasets.py` & `fetchsep-0.3.1/fetchsep/utils/read_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1593,15 +1593,15 @@
                     if flux < 0:
                         flux = badval
                     fluxes[ncol+j][count] = flux
                 count = count + 1
         csvfile.close()
 
         #If reading in multiple files, then combine all data into one array
-        if all_fluxes == []:
+        if len(all_fluxes) == 0:
             all_fluxes = fluxes
             all_dates = dates
         else:
             all_fluxes = np.concatenate((all_fluxes,fluxes),axis=1)
             all_dates = all_dates + dates
     
     if all_dates == []:
@@ -1710,15 +1710,15 @@
             
 
             flux = data.variables["AvgIntProtonFlux"][j][idx]
             if flux < 0:
                 flux = badval
             fluxes[-1][j] = flux
                 
-        if all_fluxes == []:
+        if len(all_fluxes) == 0:
             all_fluxes = fluxes
         else:
             all_fluxes = np.concatenate((all_fluxes,fluxes),axis=1)
 
 
     return all_dates, all_fluxes, west_detector
 
@@ -1832,16 +1832,16 @@
                 for k in range(n_chan):
                     flux = float(row[1+k])
                     if flux < 0:
                         flux = badval
                     fluxes[k][j] = flux
                 
                 j = j+1 #count dates
-                    
-        if all_fluxes == []:
+        
+        if len(all_fluxes) == 0:
             all_fluxes = fluxes
         else:
             all_fluxes = np.concatenate((all_fluxes,fluxes[:,0:len(all_dates)]),axis=1)
 
     return all_dates, all_fluxes, west_detector
 
 
@@ -2774,43 +2774,43 @@
     nbins = len(energy_bins)
 
     for j in range(ndates):  #flux at each time
         for i in range(nbins):
             if fluxes[i,j] == None: #bad data
                 #estimate flux with interpolation in time
                 if dointerp:
-                    print('There is a data gap for time ' + str(dates[j])
-                            + ' and energy bin ' + str(energy_bins[i][0]) + ' - '
-                            + str(energy_bins[i][1]) + '.'
-                            + ' Filling in missing value with linear '
-                            + 'interpolation in time.')
+#                    print('There is a data gap for time ' + str(dates[j])
+#                            + ' and energy bin ' + str(energy_bins[i][0]) + ' - '
+#                            + str(energy_bins[i][1]) + '.'
+#                            + ' Filling in missing value with linear '
+#                            + 'interpolation in time.')
                     interp_flux = do_interpolation(j,dates,fluxes[i,:])
                     fluxes[i,j] = interp_flux
                 else:
-                    print('There is a data gap for time ' + str(dates[j])
-                            + ' and energy bin ' + str(energy_bins[i][0]) + ' - '
-                            + str(energy_bins[i][1]) + '.'
-                            + ' Filling in missing value with None ')
+#                    print('There is a data gap for time ' + str(dates[j])
+#                            + ' and energy bin ' + str(energy_bins[i][0]) + ' - '
+#                            + str(energy_bins[i][1]) + '.'
+#                            + ' Filling in missing value with None ')
                     fluxes[i,j] = None
 
             elif fluxes[i,j] < 0:
                 #estimate flux with interpolation in time
                 if dointerp:
-                    print('There is a data gap for time ' + str(dates[j])
-                            + ' and energy bin ' + str(energy_bins[i][0]) + ' - '
-                            + str(energy_bins[i][1]) + '.'
-                            + ' Filling in missing value with linear '
-                            + 'interpolation in time.')
+#                    print('There is a data gap for time ' + str(dates[j])
+#                            + ' and energy bin ' + str(energy_bins[i][0]) + ' - '
+#                            + str(energy_bins[i][1]) + '.'
+#                            + ' Filling in missing value with linear '
+#                            + 'interpolation in time.')
                     interp_flux = do_interpolation(j,dates,fluxes[i,:])
                     fluxes[i,j] = interp_flux
                 else:
-                    print('There is a data gap for time ' + str(dates[j])
-                            + ' and energy bin ' + str(energy_bins[i][0]) + ' - '
-                            + str(energy_bins[i][1]) + '.'
-                            + ' Filling in missing value with None ')
+#                    print('There is a data gap for time ' + str(dates[j])
+#                            + ' and energy bin ' + str(energy_bins[i][0]) + ' - '
+#                            + str(energy_bins[i][1]) + '.'
+#                            + ' Filling in missing value with None ')
                     fluxes[i,j] = None #results in NaN value in np array
 
     
     print('Finished checking for bad data.')
     print()
     return fluxes
```

### Comparing `fetchsep-0.3.0/fetchsep.egg-info/PKG-INFO` & `fetchsep-0.3.1/fetchsep.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fetchsep
-Version: 0.3.0
+Version: 0.3.1
 Summary: Identify SEP elevations above background in a time series (idsep) and analyze events individually (opsep)
-Home-page: https://github.com/rickyegeland/fetchsep
+Home-page: https://github.com/ktindiana/fetchsep
 Author: Kathryn Whitman
 Author-email: kathryn.whitman@nasa.gov
 License: MIT license
 Keywords: fetchsep
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -36,16 +36,16 @@
 FetchSEP
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/fetchsep.svg
         :target: https://pypi.python.org/pypi/fetchsep
 
-.. image:: https://img.shields.io/travis/rickyegeland/fetchsep.svg
-        :target: https://travis-ci.com/rickyegeland/fetchsep
+.. image:: https://img.shields.io/travis/ktindiana/fetchsep.svg
+        :target: https://travis-ci.com/ktindiana/fetchsep
 
 .. image:: https://readthedocs.org/projects/fetchsep/badge/?version=latest
         :target: https://fetchsep.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 
@@ -162,14 +162,26 @@
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 History
 =======
 
+0.3.1 (2024-05-02)
+------------------
+
+* opsep: modified onset peak fitting and estimate
+* opsep: onset peak changed to max flux if automated algorithm
+  identifies onset after max
+* opsep: better workflow for fetchsep_prepare_obs when starting from
+  BATCH
+* opsep: updates to json output to comply with CCMC schema
+* Bugfix: Fix crash in opsep and idsep on certain python installations
+  when reading in GOES-R data files
+
 0.3.0 (2023-11-02)
 ------------------
 
 * Fixed bug preventing fluence calculation for differential fluxes
 * Improved plots for differential energy channels
 * Added capability to move output produced by `opsep` to a target dir
 * Updated filenames for plots to contain full zulu string
```

### Comparing `fetchsep-0.3.0/fetchsep.egg-info/SOURCES.txt` & `fetchsep-0.3.1/fetchsep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fetchsep-0.3.0/setup.py` & `fetchsep-0.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,11 +60,11 @@
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='fetchsep',
     name='fetchsep',
     packages=find_packages(include=['fetchsep', 'fetchsep.*']),
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/rickyegeland/fetchsep',
-    version='0.3.0',
+    url='https://github.com/ktindiana/fetchsep',
+    version='0.3.1',
     zip_safe=False,
 )
```

