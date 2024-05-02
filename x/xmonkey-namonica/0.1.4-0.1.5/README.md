# Comparing `tmp/xmonkey_namonica-0.1.4.tar.gz` & `tmp/xmonkey_namonica-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmonkey_namonica-0.1.4.tar", last modified: Mon Apr 29 21:43:04 2024, max compression
+gzip compressed data, was "xmonkey_namonica-0.1.5.tar", last modified: Thu May  2 01:23:40 2024, max compression
```

## Comparing `xmonkey_namonica-0.1.4.tar` & `xmonkey_namonica-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-29 21:43:04.682138 xmonkey_namonica-0.1.4/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.4/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-04-29 21:43:04.681952 xmonkey_namonica-0.1.4/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1966 2024-04-29 20:51:13.000000 xmonkey_namonica-0.1.4/README.md
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-04-29 21:43:04.682174 xmonkey_namonica-0.1.4/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      343 2024-04-29 21:42:49.000000 xmonkey_namonica-0.1.4/setup.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-29 21:43:04.679287 xmonkey_namonica-0.1.4/xmonkey_namonica/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2135 2024-04-28 18:13:38.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/cli.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3716 2024-04-26 18:36:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/common.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-29 21:43:04.681467 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/base_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 22:27:16.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/cargo_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4011 2024-04-29 20:48:00.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/gen_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3696 2024-04-28 18:23:26.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/github_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2200 2024-04-26 22:48:11.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/npm_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 17:48:03.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/nuget_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2218 2024-04-26 17:49:28.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/pypi_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1609 2024-04-26 18:40:38.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/utils.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-29 21:43:04.681756 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      708 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/entry_points.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/requires.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/top_level.txt
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 01:23:40.678223 xmonkey_namonica-0.1.5/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.5/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-05-02 01:23:40.678062 xmonkey_namonica-0.1.5/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1966 2024-04-29 20:51:13.000000 xmonkey_namonica-0.1.5/README.md
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-05-02 01:23:40.678255 xmonkey_namonica-0.1.5/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      343 2024-05-02 01:22:54.000000 xmonkey_namonica-0.1.5/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 01:23:40.674326 xmonkey_namonica-0.1.5/xmonkey_namonica/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2265 2024-05-01 21:38:26.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/cli.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3953 2024-05-02 01:18:35.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/common.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 01:23:40.677564 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/base_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 22:27:16.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/cargo_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4011 2024-04-29 20:48:00.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/gen_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3696 2024-04-28 18:23:26.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/github_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5113 2024-05-02 01:21:48.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/golang_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2200 2024-04-26 22:48:11.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/npm_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 17:48:03.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/nuget_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2218 2024-04-26 17:49:28.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/pypi_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1609 2024-04-26 18:40:38.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/utils.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 01:23:40.677899 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      752 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/entry_points.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/requires.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/top_level.txt
```

### Comparing `xmonkey_namonica-0.1.4/LICENSE` & `xmonkey_namonica-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.4/README.md` & `xmonkey_namonica-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica/cli.py` & `xmonkey_namonica-0.1.5/xmonkey_namonica/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 from .handlers.npm_handler import NpmHandler
 from .handlers.cargo_handler import CargoHandler
 from .handlers.pypi_handler import PypiHandler
 from .handlers.nuget_handler import NugetHandler
 from .handlers.gen_handler import GenericHandler
 from .handlers.github_handler import GithubHandler
+from .handlers.golang_handler import GolangHandler
 
 
 def main():
     parser = argparse.ArgumentParser(description="Package Analyzer Tool")
     parser.add_argument("purl", type=str, help="Package URL to process")
     parser.add_argument(
         "--export", type=str,
@@ -26,14 +27,16 @@
         handler = NpmHandler(args.purl)
     elif "pkg:cargo" in args.purl:
         handler = CargoHandler(args.purl)
     elif "pkg:pypi" in args.purl:
         handler = PypiHandler(args.purl)
     elif "pkg:nuget" in args.purl:
         handler = NugetHandler(args.purl)
+    elif "pkg:golang" in args.purl:
+        handler = GolangHandler(args.purl)
     elif "pkg:generic" in args.purl:
         handler = GenericHandler(args.purl)
     elif "pkg:github" in args.purl:
         handler = GithubHandler(args.purl)
     else:
         raise ValueError("Unsupported PURL type")
     handler.fetch()
```

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica/common.py` & `xmonkey_namonica-0.1.5/xmonkey_namonica/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,32 @@
         path_parts = url.path.strip('/').split('/')
         if len(path_parts) < 2:
             raise ValueError(
                 "Invalid PURL format. Expected at least pkg:type/name@version"
             )
         result['type'] = path_parts[0]
         name_with_version = path_parts[-1]
-        if len(path_parts) == 3:
+        if len(path_parts) >= 3:
             result['namespace'] = unquote(path_parts[1])
         else:
             result['namespace'] = None
         name_version = name_with_version.split('@', 1)
         result['name'] = unquote(name_version[0])
         if len(name_version) > 1:
             result['version'] = name_version[1]
         else:
             result['version'] = None
+        # Small ugly hack for Go
+        if 'golang' in result['type']:
+            if len(path_parts) == 5:
+                result['name'] = path_parts[3]
+                result['version'] = None
         result['qualifiers'] = parse_qs(url.query)
         result['subpath'] = unquote(url.fragment) if url.fragment else None
-
+        result['fullparts'] = path_parts
         return result
 
     @staticmethod
     def unpack_package(file_path):
         with temp_directory() as temp_dir:
             if file_path.endswith('.zip'):
                 extract_zip(file_path, temp_dir)
```

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/base_handler.py` & `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/cargo_handler.py` & `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/cargo_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/gen_handler.py` & `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/gen_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/github_handler.py` & `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/github_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/npm_handler.py` & `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/npm_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/nuget_handler.py` & `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/nuget_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/pypi_handler.py` & `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/pypi_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica/utils.py` & `xmonkey_namonica-0.1.5/xmonkey_namonica/utils.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/SOURCES.txt` & `xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 xmonkey_namonica.egg-info/requires.txt
 xmonkey_namonica.egg-info/top_level.txt
 xmonkey_namonica/handlers/__init__.py
 xmonkey_namonica/handlers/base_handler.py
 xmonkey_namonica/handlers/cargo_handler.py
 xmonkey_namonica/handlers/gen_handler.py
 xmonkey_namonica/handlers/github_handler.py
+xmonkey_namonica/handlers/golang_handler.py
 xmonkey_namonica/handlers/npm_handler.py
 xmonkey_namonica/handlers/nuget_handler.py
 xmonkey_namonica/handlers/pypi_handler.py
```

