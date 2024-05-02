# Comparing `tmp/musicnotes-1.0.tar.gz` & `tmp/musicnotes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicnotes-1.0.tar", last modified: Thu May  2 00:35:28 2024, max compression
+gzip compressed data, was "musicnotes-1.0.1.tar", last modified: Thu May  2 00:47:47 2024, max compression
```

## Comparing `musicnotes-1.0.tar` & `musicnotes-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 00:35:28.086004 musicnotes-1.0/
--rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0/LICENSE
--rw-rw-rw-   0        0        0     1434 2024-05-02 00:35:28.082931 musicnotes-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2902 2024-05-01 23:44:11.000000 musicnotes-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 00:35:28.080923 musicnotes-1.0/musicnotes.egg-info/
--rw-rw-rw-   0        0        0     1434 2024-05-02 00:35:28.000000 musicnotes-1.0/musicnotes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-05-02 00:35:28.000000 musicnotes-1.0/musicnotes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 00:35:28.000000 musicnotes-1.0/musicnotes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 00:35:28.000000 musicnotes-1.0/musicnotes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1210 2024-05-02 00:00:06.000000 musicnotes-1.0/musicnotes.py
--rw-rw-rw-   0        0        0       42 2024-05-02 00:35:28.086004 musicnotes-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1567 2024-05-02 00:34:49.000000 musicnotes-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:47:47.363648 musicnotes-1.0.1/
+-rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4437 2024-05-02 00:47:47.361635 musicnotes-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2902 2024-05-01 23:44:11.000000 musicnotes-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 00:47:47.359587 musicnotes-1.0.1/musicnotes.egg-info/
+-rw-rw-rw-   0        0        0     4437 2024-05-02 00:47:47.000000 musicnotes-1.0.1/musicnotes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-05-02 00:47:47.000000 musicnotes-1.0.1/musicnotes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 00:47:47.000000 musicnotes-1.0.1/musicnotes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 00:47:47.000000 musicnotes-1.0.1/musicnotes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1210 2024-05-02 00:00:06.000000 musicnotes-1.0.1/musicnotes.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 00:47:47.364647 musicnotes-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1887 2024-05-02 00:45:59.000000 musicnotes-1.0.1/setup.py
```

### Comparing `musicnotes-1.0/LICENSE` & `musicnotes-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0/README.md` & `musicnotes-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0/musicnotes.py` & `musicnotes-1.0.1/musicnotes.py`

 * *Files identical despite different names*

