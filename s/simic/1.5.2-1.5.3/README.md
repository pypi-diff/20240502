# Comparing `tmp/simic-1.5.2.tar.gz` & `tmp/simic-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simic-1.5.2.tar", last modified: Thu May  2 17:35:45 2024, max compression
+gzip compressed data, was "simic-1.5.3.tar", last modified: Thu May  2 17:39:31 2024, max compression
```

## Comparing `simic-1.5.2.tar` & `simic-1.5.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 17:35:45.623000 simic-1.5.2/
--rw-rw-rw-   0        0        0       52 2024-05-02 17:35:45.568000 simic-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-02 17:35:45.609000 simic-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      171 2024-05-02 17:35:35.000000 simic-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:35:45.002000 simic-1.5.2/simic/
--rw-rw-rw-   0        0        0      304 2024-05-02 17:35:03.000000 simic-1.5.2/simic/__init__.py
--rw-rw-rw-   0        0        0     4103 2024-05-02 17:34:57.000000 simic-1.5.2/simic/xpath.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:35:45.508000 simic-1.5.2/simic.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-02 17:35:44.000000 simic-1.5.2/simic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-02 17:35:44.000000 simic-1.5.2/simic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 17:35:44.000000 simic-1.5.2/simic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 17:35:44.000000 simic-1.5.2/simic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-02 17:35:44.000000 simic-1.5.2/simic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 17:39:31.238000 simic-1.5.3/
+-rw-rw-rw-   0        0        0       52 2024-05-02 17:39:31.194000 simic-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-02 17:39:31.223000 simic-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      171 2024-05-02 17:39:24.000000 simic-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:39:30.591000 simic-1.5.3/simic/
+-rw-rw-rw-   0        0        0      360 2024-05-02 17:39:19.000000 simic-1.5.3/simic/__init__.py
+-rw-rw-rw-   0        0        0     4103 2024-05-02 17:34:57.000000 simic-1.5.3/simic/xpath.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:39:31.122000 simic-1.5.3/simic.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-02 17:39:29.000000 simic-1.5.3/simic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-02 17:39:30.000000 simic-1.5.3/simic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 17:39:29.000000 simic-1.5.3/simic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 17:39:29.000000 simic-1.5.3/simic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 17:39:29.000000 simic-1.5.3/simic.egg-info/top_level.txt
```

### Comparing `simic-1.5.2/simic/xpath.py` & `simic-1.5.3/simic/xpath.py`

 * *Files identical despite different names*
