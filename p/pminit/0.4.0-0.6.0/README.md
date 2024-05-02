# Comparing `tmp/pminit-0.4.0.tar.gz` & `tmp/pminit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pminit-0.4.0.tar", max compression
+gzip compressed data, was "pminit-0.6.0.tar", max compression
```

## Comparing `pminit-0.4.0.tar` & `pminit-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       55 2024-04-04 20:50:40.973190 pminit-0.4.0/pminit/__init__.py
--rw-r--r--   0        0        0     1176 2024-04-04 20:50:40.973304 pminit-0.4.0/pminit/cli.py
--rw-r--r--   0        0        0     1192 2024-04-04 20:50:40.974188 pminit-0.4.0/post-install-hook.py
--rw-r--r--   0        0        0     1005 2024-04-04 20:51:24.489678 pminit-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    19961 2024-04-04 20:50:40.974439 pminit-0.4.0/pythonmonkey/package-lock.json
--rw-r--r--   0        0        0      679 2024-04-04 20:50:40.974539 pminit-0.4.0/pythonmonkey/package.json
--rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 pminit-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       55 2024-05-02 19:35:06.896936 pminit-0.6.0/pminit/__init__.py
+-rw-r--r--   0        0        0     1176 2024-05-02 19:35:06.897026 pminit-0.6.0/pminit/cli.py
+-rw-r--r--   0        0        0     1192 2024-05-02 19:35:06.897101 pminit-0.6.0/post-install-hook.py
+-rw-r--r--   0        0        0     1005 2024-05-02 19:35:51.713289 pminit-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    19961 2024-05-02 19:35:06.897336 pminit-0.6.0/pythonmonkey/package-lock.json
+-rw-r--r--   0        0        0      679 2024-05-02 19:35:06.897431 pminit-0.6.0/pythonmonkey/package.json
+-rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 pminit-0.6.0/PKG-INFO
```

### Comparing `pminit-0.4.0/pminit/cli.py` & `pminit-0.6.0/pminit/cli.py`

 * *Files identical despite different names*

### Comparing `pminit-0.4.0/post-install-hook.py` & `pminit-0.6.0/post-install-hook.py`

 * *Files identical despite different names*

### Comparing `pminit-0.4.0/pyproject.toml` & `pminit-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pminit"
-version = "0.4.0"
+version = "0.6.0"
 description = "Post-install hook for PythonMonkey"
 authors = [
   "Tom Tang <xmader@distributive.network>",
   "Caleb Aikens <caleb@distributive.network>",
   "Wes Garland <wes@distributive.network>",
   "Hamada Gasmallah <hamada@distributive.network>"
 ]
```

### Comparing `pminit-0.4.0/pythonmonkey/package-lock.json` & `pminit-0.6.0/pythonmonkey/package-lock.json`

 * *Files identical despite different names*

### Comparing `pminit-0.4.0/pythonmonkey/package.json` & `pminit-0.6.0/pythonmonkey/package.json`

 * *Files identical despite different names*

