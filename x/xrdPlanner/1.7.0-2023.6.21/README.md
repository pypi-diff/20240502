# Comparing `tmp/xrdplanner-1.7.0.tar.gz` & `tmp/xrdPlanner-2023.6.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrdplanner-1.7.0.tar", last modified: Thu May  2 08:59:22 2024, max compression
+gzip compressed data, was "xrdPlanner-2023.6.21.tar", last modified: Wed Jun 21 08:08:53 2023, max compression
```

## Comparing `xrdplanner-1.7.0.tar` & `xrdPlanner-2023.6.21.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2024-05-02 08:59:22.657878 xrdplanner-1.7.0/
--rw-rw-r--   0 au577597 (1644281986) staff       (20)    35149 2023-06-21 09:32:27.000000 xrdplanner-1.7.0/LICENSE
--rw-r--r--   0 au577597 (1644281986) staff       (20)    26257 2024-05-02 08:59:22.657631 xrdplanner-1.7.0/PKG-INFO
--rw-r--r--   0 au577597 (1644281986) staff       (20)    25360 2024-05-02 08:58:33.000000 xrdplanner-1.7.0/README.md
--rw-r--r--   0 au577597 (1644281986) staff       (20)     1042 2023-11-28 15:46:59.000000 xrdplanner-1.7.0/pyproject.toml
--rw-r--r--   0 au577597 (1644281986) staff       (20)       38 2024-05-02 08:59:22.657928 xrdplanner-1.7.0/setup.cfg
-drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2024-05-02 08:59:22.656253 xrdplanner-1.7.0/xrdPlanner/
--rw-r--r--   0 au577597 (1644281986) staff       (20)      207 2024-05-02 08:43:22.000000 xrdplanner-1.7.0/xrdPlanner/__init__.py
--rw-r--r--   0 au577597 (1644281986) staff       (20)   153461 2024-05-02 08:41:19.000000 xrdplanner-1.7.0/xrdPlanner/classes.py
--rw-r--r--   0 au577597 (1644281986) staff       (20)   525436 2024-04-25 09:32:52.000000 xrdplanner-1.7.0/xrdPlanner/resources.py
--rw-r--r--   0 au577597 (1644281986) staff       (20)      256 2024-02-17 13:45:50.000000 xrdplanner-1.7.0/xrdPlanner/run_xrdPlanner.py
-drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2024-05-02 08:59:22.657390 xrdplanner-1.7.0/xrdPlanner.egg-info/
--rw-r--r--   0 au577597 (1644281986) staff       (20)    26257 2024-05-02 08:59:22.000000 xrdplanner-1.7.0/xrdPlanner.egg-info/PKG-INFO
--rw-r--r--   0 au577597 (1644281986) staff       (20)      336 2024-05-02 08:59:22.000000 xrdplanner-1.7.0/xrdPlanner.egg-info/SOURCES.txt
--rw-r--r--   0 au577597 (1644281986) staff       (20)        1 2024-05-02 08:59:22.000000 xrdplanner-1.7.0/xrdPlanner.egg-info/dependency_links.txt
--rw-r--r--   0 au577597 (1644281986) staff       (20)       62 2024-05-02 08:59:22.000000 xrdplanner-1.7.0/xrdPlanner.egg-info/entry_points.txt
--rw-r--r--   0 au577597 (1644281986) staff       (20)       77 2024-05-02 08:59:22.000000 xrdplanner-1.7.0/xrdPlanner.egg-info/requires.txt
--rw-r--r--   0 au577597 (1644281986) staff       (20)       11 2024-05-02 08:59:22.000000 xrdplanner-1.7.0/xrdPlanner.egg-info/top_level.txt
+drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2023-06-21 08:08:53.647622 xrdPlanner-2023.6.21/
+-rw-rw-r--   0 au577597 (1644281986) staff       (20)    18092 2023-06-16 09:45:06.000000 xrdPlanner-2023.6.21/LICENSE
+-rw-r--r--   0 au577597 (1644281986) staff       (20)     4640 2023-06-21 08:08:53.647515 xrdPlanner-2023.6.21/PKG-INFO
+-rw-rw-r--   0 au577597 (1644281986) staff       (20)     3930 2023-06-21 08:06:37.000000 xrdPlanner-2023.6.21/README.md
+-rw-r--r--   0 au577597 (1644281986) staff       (20)       38 2023-06-21 08:08:53.647656 xrdPlanner-2023.6.21/setup.cfg
+-rw-r--r--   0 au577597 (1644281986) staff       (20)     1257 2023-06-21 08:06:42.000000 xrdPlanner-2023.6.21/setup.py
+drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2023-06-21 08:08:53.646614 xrdPlanner-2023.6.21/xrdPlanner/
+-rw-r--r--   0 au577597 (1644281986) staff       (20)       80 2023-06-21 08:07:18.000000 xrdPlanner-2023.6.21/xrdPlanner/__init__.py
+-rw-rw-r--   0 au577597 (1644281986) staff       (20)    50103 2023-06-21 07:56:07.000000 xrdPlanner-2023.6.21/xrdPlanner/classes.py
+-rw-r--r--   0 au577597 (1644281986) staff       (20)    93475 2023-06-21 07:00:20.000000 xrdPlanner-2023.6.21/xrdPlanner/resources.py
+-rw-rw-r--   0 au577597 (1644281986) staff       (20)      256 2023-06-21 06:49:34.000000 xrdPlanner-2023.6.21/xrdPlanner/run_xrdPlanner.py
+drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2023-06-21 08:08:53.647364 xrdPlanner-2023.6.21/xrdPlanner.egg-info/
+-rw-r--r--   0 au577597 (1644281986) staff       (20)     4640 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/PKG-INFO
+-rw-r--r--   0 au577597 (1644281986) staff       (20)      330 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/SOURCES.txt
+-rw-r--r--   0 au577597 (1644281986) staff       (20)        1 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/dependency_links.txt
+-rw-r--r--   0 au577597 (1644281986) staff       (20)       62 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/entry_points.txt
+-rw-r--r--   0 au577597 (1644281986) staff       (20)       77 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/requires.txt
+-rw-r--r--   0 au577597 (1644281986) staff       (20)       11 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/top_level.txt
```

