# Comparing `tmp/ls_cred_storage-0.1.1.tar.gz` & `tmp/ls_cred_storage-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls_cred_storage-0.1.1.tar", last modified: Thu May  2 09:36:42 2024, max compression
+gzip compressed data, was "ls_cred_storage-0.1.12.tar", last modified: Mon Apr 29 20:19:18 2024, max compression
```

## Comparing `ls_cred_storage-0.1.1.tar` & `ls_cred_storage-0.1.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:36:42.141761 ls_cred_storage-0.1.1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1103 2024-05-02 09:33:45.000000 ls_cred_storage-0.1.1/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      560 2024-05-02 09:36:42.141761 ls_cred_storage-0.1.1/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2024-05-02 09:33:45.000000 ls_cred_storage-0.1.1/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:36:42.137761 ls_cred_storage-0.1.1/ls_cred_storage/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-02 09:33:45.000000 ls_cred_storage-0.1.1/ls_cred_storage/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1983 2024-05-02 09:33:45.000000 ls_cred_storage-0.1.1/ls_cred_storage/ls_cred_storage.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:36:42.141761 ls_cred_storage-0.1.1/ls_cred_storage.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      560 2024-05-02 09:36:42.000000 ls_cred_storage-0.1.1/ls_cred_storage.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      289 2024-05-02 09:36:42.000000 ls_cred_storage-0.1.1/ls_cred_storage.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-02 09:36:42.000000 ls_cred_storage-0.1.1/ls_cred_storage.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-02 09:36:42.000000 ls_cred_storage-0.1.1/ls_cred_storage.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-02 09:36:42.000000 ls_cred_storage-0.1.1/ls_cred_storage.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      616 2024-05-02 09:36:38.000000 ls_cred_storage-0.1.1/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-02 09:36:42.141761 ls_cred_storage-0.1.1/setup.cfg
+drwxr-xr-x   0 Sargis_Hayrapetyan   (501) staff       (20)        0 2024-04-29 20:19:18.568089 ls_cred_storage-0.1.12/
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)     1103 2024-04-29 20:17:05.000000 ls_cred_storage-0.1.12/LICENSE
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)      532 2024-04-29 20:19:18.567303 ls_cred_storage-0.1.12/PKG-INFO
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)       79 2024-04-29 20:17:05.000000 ls_cred_storage-0.1.12/README.md
+drwxr-xr-x   0 Sargis_Hayrapetyan   (501) staff       (20)        0 2024-04-29 20:19:18.564282 ls_cred_storage-0.1.12/ls_cred_storage/
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)       57 2024-04-29 20:17:05.000000 ls_cred_storage-0.1.12/ls_cred_storage/__init__.py
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)     1983 2024-04-29 20:17:05.000000 ls_cred_storage-0.1.12/ls_cred_storage/ls_cred_storage.py
+drwxr-xr-x   0 Sargis_Hayrapetyan   (501) staff       (20)        0 2024-04-29 20:19:18.566667 ls_cred_storage-0.1.12/ls_cred_storage.egg-info/
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)      532 2024-04-29 20:19:18.000000 ls_cred_storage-0.1.12/ls_cred_storage.egg-info/PKG-INFO
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)      283 2024-04-29 20:19:18.000000 ls_cred_storage-0.1.12/ls_cred_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)        1 2024-04-29 20:19:18.000000 ls_cred_storage-0.1.12/ls_cred_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)       16 2024-04-29 20:19:18.000000 ls_cred_storage-0.1.12/ls_cred_storage.egg-info/requires.txt
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)       16 2024-04-29 20:19:18.000000 ls_cred_storage-0.1.12/ls_cred_storage.egg-info/top_level.txt
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)       38 2024-04-29 20:19:18.568275 ls_cred_storage-0.1.12/setup.cfg
+-rw-r--r--   0 Sargis_Hayrapetyan   (501) staff       (20)      805 2024-04-29 20:17:05.000000 ls_cred_storage-0.1.12/setup.py
```

### Comparing `ls_cred_storage-0.1.1/LICENSE` & `ls_cred_storage-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `ls_cred_storage-0.1.1/ls_cred_storage/ls_cred_storage.py` & `ls_cred_storage-0.1.12/ls_cred_storage/ls_cred_storage.py`

 * *Files identical despite different names*

