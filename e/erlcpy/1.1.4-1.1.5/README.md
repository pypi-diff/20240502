# Comparing `tmp/erlcpy-1.1.4.tar.gz` & `tmp/erlcpy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlcpy-1.1.4.tar", last modified: Mon Apr 15 20:41:41 2024, max compression
+gzip compressed data, was "erlcpy-1.1.5.tar", last modified: Thu May  2 19:23:42 2024, max compression
```

## Comparing `erlcpy-1.1.4.tar` & `erlcpy-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 20:41:41.312086 erlcpy-1.1.4/
--rw-rw-rw-   0        0        0     1085 2024-02-25 08:54:13.000000 erlcpy-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      363 2024-04-15 20:41:41.312086 erlcpy-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      666 2024-02-25 08:21:47.000000 erlcpy-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 20:41:41.296085 erlcpy-1.1.4/erlcpy/
--rw-rw-rw-   0        0        0       46 2024-04-15 20:39:04.000000 erlcpy-1.1.4/erlcpy/__init__.py
--rw-rw-rw-   0        0        0     2204 2024-04-15 20:38:09.000000 erlcpy-1.1.4/erlcpy/main.py
-drwxrwxrwx   0        0        0        0 2024-04-15 20:41:41.311088 erlcpy-1.1.4/erlcpy.egg-info/
--rw-rw-rw-   0        0        0      363 2024-04-15 20:41:41.000000 erlcpy-1.1.4/erlcpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-15 20:41:41.000000 erlcpy-1.1.4/erlcpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 20:41:41.000000 erlcpy-1.1.4/erlcpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 20:41:41.000000 erlcpy-1.1.4/erlcpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 20:41:41.000000 erlcpy-1.1.4/erlcpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 20:41:41.313085 erlcpy-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      469 2024-04-15 20:41:31.000000 erlcpy-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:23:42.424074 erlcpy-1.1.5/
+-rw-rw-rw-   0        0        0     1085 2024-02-25 08:54:13.000000 erlcpy-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      363 2024-05-02 19:23:42.423066 erlcpy-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2024-02-25 08:21:47.000000 erlcpy-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 19:23:42.406626 erlcpy-1.1.5/erlcpy/
+-rw-rw-rw-   0        0        0       46 2024-04-15 20:39:04.000000 erlcpy-1.1.5/erlcpy/__init__.py
+-rw-rw-rw-   0        0        0     2972 2024-05-02 19:21:27.000000 erlcpy-1.1.5/erlcpy/main.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:23:42.421986 erlcpy-1.1.5/erlcpy.egg-info/
+-rw-rw-rw-   0        0        0      363 2024-05-02 19:23:42.000000 erlcpy-1.1.5/erlcpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-02 19:23:42.000000 erlcpy-1.1.5/erlcpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 19:23:42.000000 erlcpy-1.1.5/erlcpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 19:23:42.000000 erlcpy-1.1.5/erlcpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-02 19:23:42.000000 erlcpy-1.1.5/erlcpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 19:23:42.424074 erlcpy-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      469 2024-05-02 19:23:40.000000 erlcpy-1.1.5/setup.py
```

### Comparing `erlcpy-1.1.4/LICENSE` & `erlcpy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `erlcpy-1.1.4/README.md` & `erlcpy-1.1.5/README.md`

 * *Files identical despite different names*

