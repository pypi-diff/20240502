# Comparing `tmp/conda-libmamba-solver-0.0.1.tar.gz` & `tmp/conda-libmamba-solver-24.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda-libmamba-solver-0.0.1.tar", last modified: Thu May  2 16:31:04 2024, max compression
+gzip compressed data, was "conda-libmamba-solver-24.1.0.tar", last modified: Thu May  2 17:30:49 2024, max compression
```

## Comparing `conda-libmamba-solver-0.0.1.tar` & `conda-libmamba-solver-24.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:31:04.717297 conda-libmamba-solver-0.0.1/
--rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 conda-libmamba-solver-0.0.1/LICENSE.txt
--rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 conda-libmamba-solver-0.0.1/MANIFEST.in
--rw-r--r--   0 kotko      (501) staff       (20)      450 2024-05-02 16:31:04.717204 conda-libmamba-solver-0.0.1/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)       15 2023-05-10 17:51:27.000000 conda-libmamba-solver-0.0.1/README.md
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:31:04.716910 conda-libmamba-solver-0.0.1/conda_libmamba_solver.egg-info/
--rw-r--r--   0 kotko      (501) staff       (20)      450 2024-05-02 16:31:04.000000 conda-libmamba-solver-0.0.1/conda_libmamba_solver.egg-info/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)      345 2024-05-02 16:31:04.000000 conda-libmamba-solver-0.0.1/conda_libmamba_solver.egg-info/SOURCES.txt
--rw-r--r--   0 kotko      (501) staff       (20)        1 2024-05-02 16:31:04.000000 conda-libmamba-solver-0.0.1/conda_libmamba_solver.egg-info/dependency_links.txt
--rw-r--r--   0 kotko      (501) staff       (20)        9 2024-05-02 16:31:04.000000 conda-libmamba-solver-0.0.1/conda_libmamba_solver.egg-info/requires.txt
--rw-r--r--   0 kotko      (501) staff       (20)        6 2024-05-02 16:31:04.000000 conda-libmamba-solver-0.0.1/conda_libmamba_solver.egg-info/top_level.txt
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:31:04.715789 conda-libmamba-solver-0.0.1/data/
--rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 conda-libmamba-solver-0.0.1/data/data_file
--rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 conda-libmamba-solver-0.0.1/pyproject.toml
--rw-r--r--   0 kotko      (501) staff       (20)       78 2024-05-02 16:31:04.717819 conda-libmamba-solver-0.0.1/setup.cfg
--rw-r--r--   0 kotko      (501) staff       (20)      715 2024-05-02 16:31:00.000000 conda-libmamba-solver-0.0.1/setup.py
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 16:31:04.716435 conda-libmamba-solver-0.0.1/tests/
--rw-r--r--   0 kotko      (501) staff       (20)      208 2021-02-11 13:14:03.000000 conda-libmamba-solver-0.0.1/tests/__init__.py
--rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 conda-libmamba-solver-0.0.1/tests/test_simple.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:30:49.538301 conda-libmamba-solver-24.1.0/
+-rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 conda-libmamba-solver-24.1.0/LICENSE.txt
+-rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 conda-libmamba-solver-24.1.0/MANIFEST.in
+-rw-r--r--   0 kotko      (501) staff       (20)     1108 2024-05-02 17:30:49.538205 conda-libmamba-solver-24.1.0/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)       15 2023-05-10 17:51:27.000000 conda-libmamba-solver-24.1.0/README.md
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:30:49.536610 conda-libmamba-solver-24.1.0/data/
+-rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 conda-libmamba-solver-24.1.0/data/data_file
+-rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 conda-libmamba-solver-24.1.0/pyproject.toml
+-rw-r--r--   0 kotko      (501) staff       (20)       78 2024-05-02 17:30:49.538533 conda-libmamba-solver-24.1.0/setup.cfg
+-rw-r--r--   0 kotko      (501) staff       (20)     2514 2024-05-02 17:30:46.000000 conda-libmamba-solver-24.1.0/setup.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:30:49.535549 conda-libmamba-solver-24.1.0/src/
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:30:49.537694 conda-libmamba-solver-24.1.0/src/conda_libmamba_solver.egg-info/
+-rw-r--r--   0 kotko      (501) staff       (20)     1108 2024-05-02 17:30:49.000000 conda-libmamba-solver-24.1.0/src/conda_libmamba_solver.egg-info/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)      399 2024-05-02 17:30:49.000000 conda-libmamba-solver-24.1.0/src/conda_libmamba_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        1 2024-05-02 17:30:49.000000 conda-libmamba-solver-24.1.0/src/conda_libmamba_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 kotko      (501) staff       (20)       39 2024-05-02 17:30:49.000000 conda-libmamba-solver-24.1.0/src/conda_libmamba_solver.egg-info/entry_points.txt
+-rw-r--r--   0 kotko      (501) staff       (20)       80 2024-05-02 17:30:49.000000 conda-libmamba-solver-24.1.0/src/conda_libmamba_solver.egg-info/requires.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        1 2024-05-02 17:30:49.000000 conda-libmamba-solver-24.1.0/src/conda_libmamba_solver.egg-info/top_level.txt
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2024-05-02 17:30:49.537497 conda-libmamba-solver-24.1.0/tests/
+-rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 conda-libmamba-solver-24.1.0/tests/test_simple.py
```

### Comparing `conda-libmamba-solver-0.0.1/LICENSE.txt` & `conda-libmamba-solver-24.1.0/LICENSE.txt`

 * *Files identical despite different names*

