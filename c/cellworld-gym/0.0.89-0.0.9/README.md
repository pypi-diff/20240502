# Comparing `tmp/cellworld_gym-0.0.89.tar.gz` & `tmp/cellworld_gym-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_gym-0.0.89.tar", last modified: Wed May  1 14:55:50 2024, max compression
+gzip compressed data, was "cellworld_gym-0.0.9.tar", last modified: Thu Apr 18 15:03:36 2024, max compression
```

## Comparing `cellworld_gym-0.0.89.tar` & `cellworld_gym-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 14:55:50.889116 cellworld_gym-0.0.89/
--rw-rw-rw-   0        0        0       35 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/MANIFEST.in
--rw-rw-rw-   0        0        0      455 2024-05-01 14:55:50.888116 cellworld_gym-0.0.89/PKG-INFO
--rw-rw-rw-   0        0        0       40 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 14:55:50.861124 cellworld_gym-0.0.89/cellworld_gym/
--rw-rw-rw-   0        0        0       40 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/cellworld_gym/README.md
--rw-rw-rw-   0        0        0       73 2024-05-01 14:24:56.000000 cellworld_gym-0.0.89/cellworld_gym/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 14:55:50.875125 cellworld_gym-0.0.89/cellworld_gym/__pycache__/
--rw-rw-rw-   0        0        0      253 2024-04-25 16:59:59.000000 cellworld_gym-0.0.89/cellworld_gym/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     4221 2024-04-25 16:59:59.000000 cellworld_gym-0.0.89/cellworld_gym/__pycache__/core.cpython-312.pyc
--rw-rw-rw-   0        0        0     2221 2024-04-25 16:59:42.000000 cellworld_gym-0.0.89/cellworld_gym/core.py
-drwxrwxrwx   0        0        0        0 2024-05-01 14:55:50.881124 cellworld_gym-0.0.89/cellworld_gym/envs/
--rw-rw-rw-   0        0        0      504 2024-05-01 14:24:32.000000 cellworld_gym-0.0.89/cellworld_gym/envs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 14:55:50.886116 cellworld_gym-0.0.89/cellworld_gym/envs/__pycache__/
--rw-rw-rw-   0        0        0      751 2024-04-29 16:12:25.000000 cellworld_gym-0.0.89/cellworld_gym/envs/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     8411 2024-04-29 16:12:25.000000 cellworld_gym-0.0.89/cellworld_gym/envs/__pycache__/bot_evade.cpython-312.pyc
--rw-rw-rw-   0        0        0    11111 2024-04-29 16:12:26.000000 cellworld_gym-0.0.89/cellworld_gym/envs/__pycache__/dual_evade.cpython-312.pyc
--rw-rw-rw-   0        0        0     9383 2024-04-25 20:13:13.000000 cellworld_gym-0.0.89/cellworld_gym/envs/__pycache__/oasis.cpython-312.pyc
--rw-rw-rw-   0        0        0     5725 2024-05-01 14:55:00.000000 cellworld_gym-0.0.89/cellworld_gym/envs/bot_evade.py
--rw-rw-rw-   0        0        0     7313 2024-05-01 14:23:50.000000 cellworld_gym-0.0.89/cellworld_gym/envs/dual_evade.py
--rw-rw-rw-   0        0        0     5957 2024-05-01 14:20:28.000000 cellworld_gym-0.0.89/cellworld_gym/envs/oasis.py
--rw-rw-rw-   0        0        0     1636 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/cellworld_gym/license.txt
--rw-rw-rw-   0        0        0      180 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/cellworld_gym/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 14:55:50.887126 cellworld_gym-0.0.89/cellworld_gym.egg-info/
--rw-rw-rw-   0        0        0      455 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/cellworld_gym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/cellworld_gym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/cellworld_gym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/cellworld_gym.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/cellworld_gym.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/cellworld_gym.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 14:55:50.889116 cellworld_gym-0.0.89/setup.cfg
--rw-rw-rw-   0        0        0      652 2024-05-01 14:55:50.000000 cellworld_gym-0.0.89/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:03:36.908794 cellworld_gym-0.0.9/
+-rw-rw-rw-   0        0        0       35 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      415 2024-04-18 15:03:36.907727 cellworld_gym-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 15:03:36.873624 cellworld_gym-0.0.9/cellworld_gym/
+-rw-rw-rw-   0        0        0       40 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym/README.md
+-rw-rw-rw-   0        0        0       72 2024-04-18 15:03:01.000000 cellworld_gym-0.0.9/cellworld_gym/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:03:36.904706 cellworld_gym-0.0.9/cellworld_gym/envs/
+-rw-rw-rw-   0        0        0      141 2024-04-18 14:54:55.000000 cellworld_gym-0.0.9/cellworld_gym/envs/__init__.py
+-rw-rw-rw-   0        0        0     5839 2024-04-17 20:14:13.000000 cellworld_gym-0.0.9/cellworld_gym/envs/bot_evade.py
+-rw-rw-rw-   0        0        0     1636 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym/license.txt
+-rw-rw-rw-   0        0        0      192 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 15:03:36.906775 cellworld_gym-0.0.9/cellworld_gym.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 15:03:36.908794 cellworld_gym-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      605 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/setup.py
```

### Comparing `cellworld_gym-0.0.89/cellworld_gym/license.txt` & `cellworld_gym-0.0.9/cellworld_gym/license.txt`

 * *Files identical despite different names*

