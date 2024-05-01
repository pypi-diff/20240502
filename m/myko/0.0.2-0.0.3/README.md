# Comparing `tmp/myko-0.0.2.tar.gz` & `tmp/myko-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myko-0.0.2.tar", last modified: Mon Mar 25 23:20:38 2024, max compression
+gzip compressed data, was "myko-0.0.3.tar", last modified: Wed May  1 21:58:31 2024, max compression
```

## Comparing `myko-0.0.2.tar` & `myko-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:20:38.898938 myko-0.0.2/
--rw-r--r--   0 max        (501) staff       (20)     1074 2024-03-25 22:29:02.000000 myko-0.0.2/LICENSE
--rw-r--r--   0 max        (501) staff       (20)      378 2024-03-25 23:20:38.898720 myko-0.0.2/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)       14 2024-03-25 22:28:39.000000 myko-0.0.2/README.md
-drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:20:38.897624 myko-0.0.2/myko/
--rw-r--r--   0 max        (501) staff       (20)      151 2024-03-25 23:19:28.000000 myko-0.0.2/myko/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     2458 2024-03-25 20:17:37.000000 myko-0.0.2/myko/myko.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:20:38.898500 myko-0.0.2/myko.egg-info/
--rw-r--r--   0 max        (501) staff       (20)      378 2024-03-25 23:20:38.000000 myko-0.0.2/myko.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      174 2024-03-25 23:20:38.000000 myko-0.0.2/myko.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2024-03-25 23:20:38.000000 myko-0.0.2/myko.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)        5 2024-03-25 23:20:38.000000 myko-0.0.2/myko.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)      437 2024-03-25 23:20:35.000000 myko-0.0.2/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)       38 2024-03-25 23:20:38.898978 myko-0.0.2/setup.cfg
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-05-01 21:58:31.085050 myko-0.0.3/
+-rw-r--r--   0 max        (501) staff       (20)     1074 2024-04-30 22:08:25.000000 myko-0.0.3/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)      378 2024-05-01 21:58:31.079288 myko-0.0.3/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)       14 2024-04-30 22:08:25.000000 myko-0.0.3/README.md
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-05-01 21:58:31.065669 myko-0.0.3/myko/
+-rw-r--r--   0 max        (501) staff       (20)      151 2024-04-30 22:08:25.000000 myko-0.0.3/myko/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     2009 2024-05-01 21:57:30.000000 myko-0.0.3/myko/myko.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-05-01 21:58:31.078692 myko-0.0.3/myko.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)      378 2024-05-01 21:58:31.000000 myko-0.0.3/myko.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      174 2024-05-01 21:58:31.000000 myko-0.0.3/myko.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2024-05-01 21:58:31.000000 myko-0.0.3/myko.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)        5 2024-05-01 21:58:31.000000 myko-0.0.3/myko.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)      437 2024-05-01 21:58:21.000000 myko-0.0.3/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)       38 2024-05-01 21:58:31.085278 myko-0.0.3/setup.cfg
```

### Comparing `myko-0.0.2/LICENSE` & `myko-0.0.3/LICENSE`

 * *Files identical despite different names*

