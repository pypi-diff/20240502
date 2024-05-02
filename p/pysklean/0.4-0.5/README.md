# Comparing `tmp/pysklean-0.4.tar.gz` & `tmp/pysklean-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysklean-0.4.tar", last modified: Wed Apr 24 16:10:02 2024, max compression
+gzip compressed data, was "pysklean-0.5.tar", last modified: Thu May  2 16:21:19 2024, max compression
```

## Comparing `pysklean-0.4.tar` & `pysklean-0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 16:10:02.918526 pysklean-0.4/
--rw-rw-rw-   0        0        0      113 2024-04-24 16:10:02.915521 pysklean-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 16:10:02.883517 pysklean-0.4/pysklean/
--rw-rw-rw-   0        0        0       46 2024-04-24 16:09:07.000000 pysklean-0.4/pysklean/__init__.py
--rw-rw-rw-   0        0        0    27139 2024-04-24 16:09:40.000000 pysklean-0.4/pysklean/main.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:10:02.912527 pysklean-0.4/pysklean.egg-info/
--rw-rw-rw-   0        0        0      113 2024-04-24 16:10:02.000000 pysklean-0.4/pysklean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-04-24 16:10:02.000000 pysklean-0.4/pysklean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 16:10:02.000000 pysklean-0.4/pysklean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 16:10:02.000000 pysklean-0.4/pysklean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 16:10:02.919528 pysklean-0.4/setup.cfg
--rw-rw-rw-   0        0        0      225 2024-04-24 16:09:47.000000 pysklean-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:21:19.539848 pysklean-0.5/
+-rw-rw-rw-   0        0        0      113 2024-05-02 16:21:19.525075 pysklean-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 16:21:19.419758 pysklean-0.5/pysklean/
+-rw-rw-rw-   0        0        0       42 2024-05-02 16:19:33.000000 pysklean-0.5/pysklean/__init__.py
+-rw-rw-rw-   0        0        0    59692 2024-05-02 16:19:22.000000 pysklean-0.5/pysklean/main.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:21:19.521073 pysklean-0.5/pysklean.egg-info/
+-rw-rw-rw-   0        0        0      113 2024-05-02 16:21:18.000000 pysklean-0.5/pysklean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-05-02 16:21:19.000000 pysklean-0.5/pysklean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 16:21:18.000000 pysklean-0.5/pysklean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 16:21:18.000000 pysklean-0.5/pysklean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 16:21:19.540849 pysklean-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      225 2024-05-02 16:19:39.000000 pysklean-0.5/setup.py
```

