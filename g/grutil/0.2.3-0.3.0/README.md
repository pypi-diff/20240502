# Comparing `tmp/grutil-0.2.3.tar.gz` & `tmp/grutil-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grutil-0.2.3.tar", max compression
+gzip compressed data, was "grutil-0.3.0.tar", max compression
```

## Comparing `grutil-0.2.3.tar` & `grutil-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-23 19:55:13.376022 grutil-0.2.3/grutil/__init__.py
--rw-r--r--   0        0        0      388 2024-04-23 17:34:27.834727 grutil-0.2.3/grutil/afm.py
--rw-r--r--   0        0        0      596 2024-04-23 17:40:10.985103 grutil-0.2.3/grutil/amka.py
--rw-r--r--   0        0        0     5448 2024-04-23 21:12:14.495687 grutil-0.2.3/grutil/dates.py
--rw-r--r--   0        0        0      695 2024-04-23 20:39:27.875522 grutil-0.2.3/grutil/numbers.py
--rw-r--r--   0        0        0      383 2024-04-23 19:06:07.821075 grutil-0.2.3/grutil/text.py
--rw-r--r--   0        0        0      276 2024-04-23 21:12:18.956473 grutil-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-23 18:22:42.049682 grutil-0.2.3/README.md
--rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 grutil-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-23 19:55:13.376022 grutil-0.3.0/grutil/__init__.py
+-rw-r--r--   0        0        0      388 2024-04-23 17:34:27.834727 grutil-0.3.0/grutil/afm.py
+-rw-r--r--   0        0        0      596 2024-04-23 17:40:10.985103 grutil-0.3.0/grutil/amka.py
+-rw-r--r--   0        0        0     5448 2024-04-23 21:12:14.495687 grutil-0.3.0/grutil/dates.py
+-rw-r--r--   0        0        0     1392 2024-05-02 20:08:11.141966 grutil-0.3.0/grutil/money.py
+-rw-r--r--   0        0        0      695 2024-04-23 20:39:27.875522 grutil-0.3.0/grutil/numbers.py
+-rw-r--r--   0        0        0      383 2024-04-23 19:06:07.821075 grutil-0.3.0/grutil/text.py
+-rw-r--r--   0        0        0      276 2024-05-02 21:15:43.312493 grutil-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-23 18:22:42.049682 grutil-0.3.0/README.md
+-rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 grutil-0.3.0/PKG-INFO
```

### Comparing `grutil-0.2.3/grutil/amka.py` & `grutil-0.3.0/grutil/amka.py`

 * *Files identical despite different names*

### Comparing `grutil-0.2.3/grutil/dates.py` & `grutil-0.3.0/grutil/dates.py`

 * *Files identical despite different names*

### Comparing `grutil-0.2.3/grutil/numbers.py` & `grutil-0.3.0/grutil/numbers.py`

 * *Files identical despite different names*

