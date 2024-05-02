# Comparing `tmp/simple_spykes-0.0.3.tar.gz` & `tmp/simple_spykes-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_spykes-0.0.3.tar", last modified: Tue Aug  1 23:27:51 2023, max compression
+gzip compressed data, was "simple_spykes-0.1.0.tar", last modified: Thu May  2 00:04:02 2024, max compression
```

## Comparing `simple_spykes-0.0.3.tar` & `simple_spykes-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 23:27:51.838266 simple_spykes-0.0.3/
--rw-rw-rw-   0        0        0    35819 2023-08-01 21:31:04.000000 simple_spykes-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      509 2023-08-01 23:27:51.838266 simple_spykes-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-08-01 21:30:37.000000 simple_spykes-0.0.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-01 23:27:51.839265 simple_spykes-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-08-01 23:27:31.000000 simple_spykes-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 23:27:51.827266 simple_spykes-0.0.3/simple_spykes/
--rw-rw-rw-   0        0        0      139 2023-08-01 23:23:10.000000 simple_spykes-0.0.3/simple_spykes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 23:27:51.836264 simple_spykes-0.0.3/simple_spykes/util/
--rw-rw-rw-   0        0        0        0 2023-08-01 23:21:48.000000 simple_spykes-0.0.3/simple_spykes/util/__init__.py
--rw-rw-rw-   0        0        0     2643 2023-08-01 23:27:20.000000 simple_spykes-0.0.3/simple_spykes/util/ecephys.py
-drwxrwxrwx   0        0        0        0 2023-08-01 23:27:51.834265 simple_spykes-0.0.3/simple_spykes.egg-info/
--rw-rw-rw-   0        0        0      509 2023-08-01 23:27:51.000000 simple_spykes-0.0.3/simple_spykes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-08-01 23:27:51.000000 simple_spykes-0.0.3/simple_spykes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 23:27:51.000000 simple_spykes-0.0.3/simple_spykes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-08-01 23:27:51.000000 simple_spykes-0.0.3/simple_spykes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-01 23:27:51.000000 simple_spykes-0.0.3/simple_spykes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 00:04:02.092541 simple_spykes-0.1.0/
+-rw-rw-rw-   0        0        0    35819 2023-08-01 21:31:04.000000 simple_spykes-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      509 2024-05-02 00:04:02.091541 simple_spykes-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-08-01 21:30:37.000000 simple_spykes-0.1.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-02 00:04:02.092541 simple_spykes-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      695 2024-05-01 00:01:45.000000 simple_spykes-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:04:02.062542 simple_spykes-0.1.0/simple_spykes/
+-rw-rw-rw-   0        0        0      139 2023-08-01 23:23:10.000000 simple_spykes-0.1.0/simple_spykes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:04:02.076542 simple_spykes-0.1.0/simple_spykes/graphing/
+-rw-rw-rw-   0        0        0        0 2023-10-13 16:01:47.000000 simple_spykes-0.1.0/simple_spykes/graphing/__init__.py
+-rw-rw-rw-   0        0        0     6584 2023-12-13 20:19:00.000000 simple_spykes-0.1.0/simple_spykes/graphing/basic.py
+-rw-rw-rw-   0        0        0     8544 2023-12-13 20:19:00.000000 simple_spykes-0.1.0/simple_spykes/graphing/multi.py
+-rw-rw-rw-   0        0        0     7380 2023-12-13 19:28:30.000000 simple_spykes-0.1.0/simple_spykes/graphing/raw.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:04:02.082541 simple_spykes-0.1.0/simple_spykes/graphing/util/
+-rw-rw-rw-   0        0        0        0 2023-12-13 14:19:28.000000 simple_spykes-0.1.0/simple_spykes/graphing/util/__init__.py
+-rw-rw-rw-   0        0        0     2943 2023-12-13 19:34:54.000000 simple_spykes-0.1.0/simple_spykes/graphing/util/graphdata.py
+-rw-rw-rw-   0        0        0      952 2023-12-13 16:49:04.000000 simple_spykes-0.1.0/simple_spykes/graphing/util/grapher.py
+-rw-rw-rw-   0        0        0     2794 2023-12-13 19:46:05.000000 simple_spykes-0.1.0/simple_spykes/graphing/util/io.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:04:02.088542 simple_spykes-0.1.0/simple_spykes/metric_packages/
+-rw-rw-rw-   0        0        0      188 2023-12-01 02:56:54.000000 simple_spykes-0.1.0/simple_spykes/metric_packages/__init__.py
+-rw-rw-rw-   0        0        0     5883 2023-12-13 00:38:47.000000 simple_spykes-0.1.0/simple_spykes/metric_packages/bombcell_metrics.py
+-rw-rw-rw-   0        0        0     4339 2024-05-02 00:04:00.000000 simple_spykes-0.1.0/simple_spykes/metric_packages/ecephys_metrics.py
+-rw-rw-rw-   0        0        0    13121 2023-12-01 02:56:26.000000 simple_spykes-0.1.0/simple_spykes/metric_packages/spikeinterface_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:04:02.089540 simple_spykes-0.1.0/simple_spykes/util/
+-rw-rw-rw-   0        0        0      548 2023-12-01 02:17:18.000000 simple_spykes-0.1.0/simple_spykes/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:04:02.070541 simple_spykes-0.1.0/simple_spykes.egg-info/
+-rw-rw-rw-   0        0        0      509 2024-05-02 00:04:01.000000 simple_spykes-0.1.0/simple_spykes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2024-05-02 00:04:01.000000 simple_spykes-0.1.0/simple_spykes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 00:04:01.000000 simple_spykes-0.1.0/simple_spykes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-05-02 00:04:01.000000 simple_spykes-0.1.0/simple_spykes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-02 00:04:01.000000 simple_spykes-0.1.0/simple_spykes.egg-info/top_level.txt
```

### Comparing `simple_spykes-0.0.3/LICENSE` & `simple_spykes-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_spykes-0.0.3/setup.py` & `simple_spykes-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.3"
+VERSION = "0.1.0"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

