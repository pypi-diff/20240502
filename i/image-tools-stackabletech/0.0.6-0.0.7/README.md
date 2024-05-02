# Comparing `tmp/image_tools_stackabletech-0.0.6.tar.gz` & `tmp/image_tools_stackabletech-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_tools_stackabletech-0.0.6.tar", last modified: Wed Apr 24 15:45:04 2024, max compression
+gzip compressed data, was "image_tools_stackabletech-0.0.7.tar", last modified: Thu May  2 10:41:11 2024, max compression
```

## Comparing `image_tools_stackabletech-0.0.6.tar` & `image_tools_stackabletech-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2024-04-24 15:45:04.290118 image_tools_stackabletech-0.0.6/
--rw-rw-r--   0 razvan    (1000) razvan    (1000)     1069 2023-12-01 16:23:46.000000 image_tools_stackabletech-0.0.6/LICENSE
--rw-r--r--   0 razvan    (1000) razvan    (1000)     2171 2024-04-24 15:45:04.290118 image_tools_stackabletech-0.0.6/PKG-INFO
--rw-rw-r--   0 razvan    (1000) razvan    (1000)     1445 2024-04-24 15:35:44.000000 image_tools_stackabletech-0.0.6/README.md
--rw-rw-r--   0 razvan    (1000) razvan    (1000)      898 2024-04-24 15:35:44.000000 image_tools_stackabletech-0.0.6/pyproject.toml
--rw-rw-r--   0 razvan    (1000) razvan    (1000)       38 2024-04-24 15:45:04.290118 image_tools_stackabletech-0.0.6/setup.cfg
-drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2024-04-24 15:45:04.282118 image_tools_stackabletech-0.0.6/src/
-drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2024-04-24 15:45:04.286118 image_tools_stackabletech-0.0.6/src/image_tools/
--rw-rw-r--   0 razvan    (1000) razvan    (1000)       34 2023-12-01 16:23:46.000000 image_tools_stackabletech-0.0.6/src/image_tools/__init__.py
--rw-rw-r--   0 razvan    (1000) razvan    (1000)     6230 2024-04-24 15:35:44.000000 image_tools_stackabletech-0.0.6/src/image_tools/args.py
--rw-rw-r--   0 razvan    (1000) razvan    (1000)     5996 2023-12-01 16:23:46.000000 image_tools_stackabletech-0.0.6/src/image_tools/bake.py
--rw-rw-r--   0 razvan    (1000) razvan    (1000)      711 2023-12-01 16:23:46.000000 image_tools_stackabletech-0.0.6/src/image_tools/lib.py
--rw-rw-r--   0 razvan    (1000) razvan    (1000)     4524 2024-04-24 15:35:44.000000 image_tools_stackabletech-0.0.6/src/image_tools/preflight.py
-drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2024-04-24 15:45:04.286118 image_tools_stackabletech-0.0.6/src/image_tools/test/
--rw-rw-r--   0 razvan    (1000) razvan    (1000)    14577 2023-12-01 16:23:46.000000 image_tools_stackabletech-0.0.6/src/image_tools/test/conf.py
-drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2024-04-24 15:45:04.290118 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/
--rw-r--r--   0 razvan    (1000) razvan    (1000)     2171 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/PKG-INFO
--rw-rw-r--   0 razvan    (1000) razvan    (1000)      509 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/SOURCES.txt
--rw-rw-r--   0 razvan    (1000) razvan    (1000)        1 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/dependency_links.txt
--rw-rw-r--   0 razvan    (1000) razvan    (1000)       92 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/entry_points.txt
--rw-rw-r--   0 razvan    (1000) razvan    (1000)       60 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/requires.txt
--rw-rw-r--   0 razvan    (1000) razvan    (1000)       12 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/top_level.txt
+drwxr-xr-x   0 razvan    (1000) razvan    (1000)        0 2024-05-02 10:41:11.729666 image_tools_stackabletech-0.0.7/
+-rw-r--r--   0 razvan    (1000) razvan    (1000)     1069 2024-04-26 19:44:29.000000 image_tools_stackabletech-0.0.7/LICENSE
+-rw-r--r--   0 razvan    (1000) razvan    (1000)     2171 2024-05-02 10:41:11.729666 image_tools_stackabletech-0.0.7/PKG-INFO
+-rw-r--r--   0 razvan    (1000) razvan    (1000)     1445 2024-05-02 10:39:50.000000 image_tools_stackabletech-0.0.7/README.md
+-rw-r--r--   0 razvan    (1000) razvan    (1000)      876 2024-05-02 10:39:50.000000 image_tools_stackabletech-0.0.7/pyproject.toml
+-rw-r--r--   0 razvan    (1000) razvan    (1000)       38 2024-05-02 10:41:11.729666 image_tools_stackabletech-0.0.7/setup.cfg
+drwxr-xr-x   0 razvan    (1000) razvan    (1000)        0 2024-05-02 10:41:11.727666 image_tools_stackabletech-0.0.7/src/
+drwxr-xr-x   0 razvan    (1000) razvan    (1000)        0 2024-05-02 10:41:11.728665 image_tools_stackabletech-0.0.7/src/image_tools/
+-rw-r--r--   0 razvan    (1000) razvan    (1000)       34 2024-04-26 19:44:29.000000 image_tools_stackabletech-0.0.7/src/image_tools/__init__.py
+-rw-r--r--   0 razvan    (1000) razvan    (1000)     6211 2024-05-02 10:34:46.000000 image_tools_stackabletech-0.0.7/src/image_tools/args.py
+-rw-r--r--   0 razvan    (1000) razvan    (1000)     5961 2024-05-02 10:34:46.000000 image_tools_stackabletech-0.0.7/src/image_tools/bake.py
+-rw-r--r--   0 razvan    (1000) razvan    (1000)      711 2024-04-26 19:44:29.000000 image_tools_stackabletech-0.0.7/src/image_tools/lib.py
+-rw-r--r--   0 razvan    (1000) razvan    (1000)     4524 2024-04-26 19:44:29.000000 image_tools_stackabletech-0.0.7/src/image_tools/preflight.py
+drwxr-xr-x   0 razvan    (1000) razvan    (1000)        0 2024-05-02 10:41:11.728665 image_tools_stackabletech-0.0.7/src/image_tools/test/
+-rw-r--r--   0 razvan    (1000) razvan    (1000)    14577 2024-04-26 19:44:29.000000 image_tools_stackabletech-0.0.7/src/image_tools/test/conf.py
+drwxr-xr-x   0 razvan    (1000) razvan    (1000)        0 2024-05-02 10:41:11.729666 image_tools_stackabletech-0.0.7/src/image_tools_stackabletech.egg-info/
+-rw-r--r--   0 razvan    (1000) razvan    (1000)     2171 2024-05-02 10:41:11.000000 image_tools_stackabletech-0.0.7/src/image_tools_stackabletech.egg-info/PKG-INFO
+-rw-r--r--   0 razvan    (1000) razvan    (1000)      509 2024-05-02 10:41:11.000000 image_tools_stackabletech-0.0.7/src/image_tools_stackabletech.egg-info/SOURCES.txt
+-rw-r--r--   0 razvan    (1000) razvan    (1000)        1 2024-05-02 10:41:11.000000 image_tools_stackabletech-0.0.7/src/image_tools_stackabletech.egg-info/dependency_links.txt
+-rw-r--r--   0 razvan    (1000) razvan    (1000)       92 2024-05-02 10:41:11.000000 image_tools_stackabletech-0.0.7/src/image_tools_stackabletech.egg-info/entry_points.txt
+-rw-r--r--   0 razvan    (1000) razvan    (1000)       60 2024-05-02 10:41:11.000000 image_tools_stackabletech-0.0.7/src/image_tools_stackabletech.egg-info/requires.txt
+-rw-r--r--   0 razvan    (1000) razvan    (1000)       12 2024-05-02 10:41:11.000000 image_tools_stackabletech-0.0.7/src/image_tools_stackabletech.egg-info/top_level.txt
```

### Comparing `image_tools_stackabletech-0.0.6/LICENSE` & `image_tools_stackabletech-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `image_tools_stackabletech-0.0.6/PKG-INFO` & `image_tools_stackabletech-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-tools-stackabletech
-Version: 0.0.6
+Version: 0.0.7
 Summary: Image tools for the Stackable Data Platform.
 Author-email: Razvan Mihai <razvan.mihai@stackable.tech>
 Project-URL: Homepage, https://github.com/stackabletech/image-tools
 Project-URL: Bug Tracker, https://github.com/stackabletech/image-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 License-File: LICENSE
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: PyYAML>=6.0
 Provides-Extra: lint
 Requires-Dist: ruff==0.0.275; extra == "lint"
 Requires-Dist: mypy==1.4.0; extra == "lint"
 
-# image-tools v0.0.6
+# image-tools v0.0.7
 
 Commandline tools to manage Stackable container images available at https://github.com/stackabletech/docker-images
 
 This repository (and the installable package) contain two tools:
 
 * `bake` : build and publish product images.
 * `check-container` : run RedHat preflight checks on container images.
```

### Comparing `image_tools_stackabletech-0.0.6/README.md` & `image_tools_stackabletech-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# image-tools v0.0.6
+# image-tools v0.0.7
 
 Commandline tools to manage Stackable container images available at https://github.com/stackabletech/docker-images
 
 This repository (and the installable package) contain two tools:
 
 * `bake` : build and publish product images.
 * `check-container` : run RedHat preflight checks on container images.
```

### Comparing `image_tools_stackabletech-0.0.6/pyproject.toml` & `image_tools_stackabletech-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 [project]
 name = "image-tools-stackabletech"
-version = "0.0.6"
-authors = [
-    { name = "Razvan Mihai", email = "razvan.mihai@stackable.tech" }
-]
+version = "0.0.7"
+authors = [{ name = "Razvan Mihai", email = "razvan.mihai@stackable.tech" }]
 description = "Image tools for the Stackable Data Platform."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "Jinja2>=3.1.2",
-    "PyYAML>=6.0"
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
+dependencies = ["Jinja2>=3.1.2", "PyYAML>=6.0"]
 [project.optional-dependencies]
 lint = ['ruff==0.0.275', 'mypy==1.4.0']
 
 [project.scripts]
 bake = "image_tools.bake:main"
 check-container = "image_tools.preflight:main"
```

### Comparing `image_tools_stackabletech-0.0.6/src/image_tools/args.py` & `image_tools_stackabletech-0.0.7/src/image_tools/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     parser.add_argument("-u", "--push", help="Push images",
                         action="store_true")
     parser.add_argument("-d", "--dry", help="Dry run.", action="store_true")
     parser.add_argument(
         "-a",
         "--architecture",
         help="Target platform for image. Default: linux/amd64.",
-        nargs="+",
         default="linux/amd64",
         type=check_architecture_input,
     )
     parser.add_argument(
         "-o",
         "--organization",
         help="Organization name within the given registry. Default: stackable",
```

### Comparing `image_tools_stackabletech-0.0.6/src/image_tools/bake.py` & `image_tools_stackabletech-0.0.7/src/image_tools/bake.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     build_args = build_image_args(versions, args.image_version)
 
     return {
         bakefile_target_name_for_product_version(product_name, versions["product"]): {
             "dockerfile": f"{product_name}/Dockerfile",
             "tags": tags,
             "args": build_args,
-            "platforms": args.architecture,
+            "platforms": [args.architecture],
             "context": ".",
             "contexts": {
                 f"stackable/image/{name}": f"target:{bakefile_target_name_for_product_version(name, version)}"
                 for name, version in versions.items()
                 if name in product_names
             },
         },
@@ -138,23 +138,22 @@
     """
     Returns a list of commands that need to be run in order to build and
     publish product images.
 
     For local building, builder instances are supported.
     """
 
-    if args.push:
-        target_mode = ["--push"]
-    elif len(args.architecture) == 1:
-        target_mode = ["--load"]
-    else:
-        target_mode = []
-
     if args.dry:
         target_mode = ["--print"]
+    else:
+        if args.push:
+            target_mode = ["--push"]
+        else:
+            target_mode = ["--load"]
+
 
     return Command(
         args=[
             "docker",
             "buildx",
             "bake",
             "--file",
```

### Comparing `image_tools_stackabletech-0.0.6/src/image_tools/lib.py` & `image_tools_stackabletech-0.0.7/src/image_tools/lib.py`

 * *Files identical despite different names*

### Comparing `image_tools_stackabletech-0.0.6/src/image_tools/preflight.py` & `image_tools_stackabletech-0.0.7/src/image_tools/preflight.py`

 * *Files identical despite different names*

### Comparing `image_tools_stackabletech-0.0.6/src/image_tools/test/conf.py` & `image_tools_stackabletech-0.0.7/src/image_tools/test/conf.py`

 * *Files identical despite different names*

### Comparing `image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/PKG-INFO` & `image_tools_stackabletech-0.0.7/src/image_tools_stackabletech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-tools-stackabletech
-Version: 0.0.6
+Version: 0.0.7
 Summary: Image tools for the Stackable Data Platform.
 Author-email: Razvan Mihai <razvan.mihai@stackable.tech>
 Project-URL: Homepage, https://github.com/stackabletech/image-tools
 Project-URL: Bug Tracker, https://github.com/stackabletech/image-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 License-File: LICENSE
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: PyYAML>=6.0
 Provides-Extra: lint
 Requires-Dist: ruff==0.0.275; extra == "lint"
 Requires-Dist: mypy==1.4.0; extra == "lint"
 
-# image-tools v0.0.6
+# image-tools v0.0.7
 
 Commandline tools to manage Stackable container images available at https://github.com/stackabletech/docker-images
 
 This repository (and the installable package) contain two tools:
 
 * `bake` : build and publish product images.
 * `check-container` : run RedHat preflight checks on container images.
```

