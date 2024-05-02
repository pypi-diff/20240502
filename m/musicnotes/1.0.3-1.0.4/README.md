# Comparing `tmp/musicnotes-1.0.3.tar.gz` & `tmp/musicnotes-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicnotes-1.0.3.tar", last modified: Thu May  2 01:48:37 2024, max compression
+gzip compressed data, was "musicnotes-1.0.4.tar", last modified: Thu May  2 02:02:51 2024, max compression
```

## Comparing `musicnotes-1.0.3.tar` & `musicnotes-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 01:48:37.614380 musicnotes-1.0.3/
--rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     4686 2024-05-02 01:48:36.976807 musicnotes-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3091 2024-05-02 00:50:49.000000 musicnotes-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 01:48:36.975808 musicnotes-1.0.3/musicnotes.egg-info/
--rw-rw-rw-   0        0        0     4686 2024-05-02 01:48:36.000000 musicnotes-1.0.3/musicnotes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-05-02 01:48:36.000000 musicnotes-1.0.3/musicnotes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 01:48:36.000000 musicnotes-1.0.3/musicnotes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 01:48:36.000000 musicnotes-1.0.3/musicnotes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1210 2024-05-02 00:00:06.000000 musicnotes-1.0.3/musicnotes.py
--rw-rw-rw-   0        0        0       42 2024-05-02 01:48:37.615383 musicnotes-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1939 2024-05-02 01:48:31.000000 musicnotes-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:02:51.744910 musicnotes-1.0.4/
+-rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4161 2024-05-02 02:02:51.742456 musicnotes-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3091 2024-05-02 00:50:49.000000 musicnotes-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 02:02:51.732633 musicnotes-1.0.4/musicnotes/
+-rw-rw-rw-   0        0        0        0 2024-05-02 01:47:17.000000 musicnotes-1.0.4/musicnotes/__init__.py
+-rw-rw-rw-   0        0        0     1210 2024-05-02 02:01:09.000000 musicnotes-1.0.4/musicnotes/musicnotes.py
+-rw-rw-rw-   0        0        0     7194 2024-05-02 02:01:15.000000 musicnotes-1.0.4/musicnotes/sound.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:02:51.740815 musicnotes-1.0.4/musicnotes.egg-info/
+-rw-rw-rw-   0        0        0     4161 2024-05-02 02:02:51.000000 musicnotes-1.0.4/musicnotes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-05-02 02:02:51.000000 musicnotes-1.0.4/musicnotes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 02:02:51.000000 musicnotes-1.0.4/musicnotes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 02:02:51.000000 musicnotes-1.0.4/musicnotes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 02:02:51.744910 musicnotes-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1351 2024-05-02 02:02:06.000000 musicnotes-1.0.4/setup.py
```

### Comparing `musicnotes-1.0.3/LICENSE` & `musicnotes-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.3/README.md` & `musicnotes-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.3/musicnotes.py` & `musicnotes-1.0.4/musicnotes/musicnotes.py`

 * *Files identical despite different names*

