# Comparing `tmp/simic-1.5.tar.gz` & `tmp/simic-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simic-1.5.tar", last modified: Thu May  2 17:02:58 2024, max compression
+gzip compressed data, was "simic-1.5.1.tar", last modified: Thu May  2 17:27:24 2024, max compression
```

## Comparing `simic-1.5.tar` & `simic-1.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 17:02:58.208000 simic-1.5/
--rw-rw-rw-   0        0        0       50 2024-05-02 17:02:58.164000 simic-1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-02 17:02:58.200000 simic-1.5/setup.cfg
--rw-rw-rw-   0        0        0      169 2024-05-02 17:02:49.000000 simic-1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:02:57.526000 simic-1.5/simic/
--rw-rw-rw-   0        0        0       20 2024-04-25 14:59:26.000000 simic-1.5/simic/__init__.py
--rw-rw-rw-   0        0        0     4383 2024-05-02 16:48:28.000000 simic-1.5/simic/xpath.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:02:58.055000 simic-1.5/simic.egg-info/
--rw-rw-rw-   0        0        0       50 2024-05-02 17:02:56.000000 simic-1.5/simic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-02 17:02:57.000000 simic-1.5/simic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 17:02:56.000000 simic-1.5/simic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 17:02:56.000000 simic-1.5/simic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-02 17:02:56.000000 simic-1.5/simic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 17:27:24.056000 simic-1.5.1/
+-rw-rw-rw-   0        0        0       52 2024-05-02 17:27:24.014000 simic-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-02 17:27:24.043000 simic-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      171 2024-05-02 17:27:17.000000 simic-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:27:23.618000 simic-1.5.1/simic/
+-rw-rw-rw-   0        0        0       20 2024-04-25 14:59:26.000000 simic-1.5.1/simic/__init__.py
+-rw-rw-rw-   0        0        0     4383 2024-05-02 16:48:28.000000 simic-1.5.1/simic/xpath.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:27:23.945000 simic-1.5.1/simic.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-02 17:27:23.000000 simic-1.5.1/simic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-02 17:27:23.000000 simic-1.5.1/simic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 17:27:23.000000 simic-1.5.1/simic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 17:27:23.000000 simic-1.5.1/simic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 17:27:23.000000 simic-1.5.1/simic.egg-info/top_level.txt
```

### Comparing `simic-1.5/simic/xpath.py` & `simic-1.5.1/simic/xpath.py`

 * *Files identical despite different names*

