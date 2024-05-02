# Comparing `tmp/ssm-svg-0.0.1.tar.gz` & `tmp/ssm_svg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-svg-0.0.1.tar", last modified: Thu May  2 07:00:41 2024, max compression
+gzip compressed data, was "ssm_svg-0.0.2.tar", last modified: Thu May  2 08:57:57 2024, max compression
```

## Comparing `ssm-svg-0.0.1.tar` & `ssm_svg-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 obeezzy   (1000) users      (984)        0 2024-05-02 07:00:41.344089 ssm-svg-0.0.1/
--rw-r--r--   0 obeezzy   (1000) users      (984)     1070 2024-05-02 03:01:06.000000 ssm-svg-0.0.1/LICENSE
--rw-r--r--   0 obeezzy   (1000) users      (984)     2840 2024-05-02 07:00:41.344089 ssm-svg-0.0.1/PKG-INFO
--rw-r--r--   0 obeezzy   (1000) users      (984)     2406 2024-05-02 06:44:53.000000 ssm-svg-0.0.1/README.md
--rw-r--r--   0 obeezzy   (1000) users      (984)       38 2024-05-02 07:00:41.344089 ssm-svg-0.0.1/setup.cfg
--rw-r--r--   0 obeezzy   (1000) users      (984)      847 2024-05-02 03:10:14.000000 ssm-svg-0.0.1/setup.py
-drwxr-xr-x   0 obeezzy   (1000) users      (984)        0 2024-05-02 07:00:41.344089 ssm-svg-0.0.1/ssm_svg.egg-info/
--rw-r--r--   0 obeezzy   (1000) users      (984)     2840 2024-05-02 07:00:41.000000 ssm-svg-0.0.1/ssm_svg.egg-info/PKG-INFO
--rw-r--r--   0 obeezzy   (1000) users      (984)      198 2024-05-02 07:00:41.000000 ssm-svg-0.0.1/ssm_svg.egg-info/SOURCES.txt
--rw-r--r--   0 obeezzy   (1000) users      (984)        1 2024-05-02 07:00:41.000000 ssm-svg-0.0.1/ssm_svg.egg-info/dependency_links.txt
--rw-r--r--   0 obeezzy   (1000) users      (984)        5 2024-05-02 07:00:41.000000 ssm-svg-0.0.1/ssm_svg.egg-info/requires.txt
--rw-r--r--   0 obeezzy   (1000) users      (984)        1 2024-05-02 07:00:41.000000 ssm-svg-0.0.1/ssm_svg.egg-info/top_level.txt
-drwxr-xr-x   0 obeezzy   (1000) users      (984)        0 2024-05-02 07:00:41.344089 ssm-svg-0.0.1/tests/
--rw-r--r--   0 obeezzy   (1000) users      (984)     6353 2024-05-02 05:59:47.000000 ssm-svg-0.0.1/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:57:57.364526 ssm_svg-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 08:57:49.000000 ssm_svg-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-02 08:57:57.364526 ssm_svg-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-02 08:57:49.000000 ssm_svg-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:57:57.364526 ssm_svg-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 08:57:49.000000 ssm_svg-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:57:57.364526 ssm_svg-0.0.2/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:57:49.000000 ssm_svg-0.0.2/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 08:57:49.000000 ssm_svg-0.0.2/ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 08:57:49.000000 ssm_svg-0.0.2/ssm/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15531 2024-05-02 08:57:49.000000 ssm_svg-0.0.2/ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:57:57.364526 ssm_svg-0.0.2/ssm_svg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-02 08:57:57.000000 ssm_svg-0.0.2/ssm_svg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 08:57:57.000000 ssm_svg-0.0.2/ssm_svg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:57:57.000000 ssm_svg-0.0.2/ssm_svg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 08:57:57.000000 ssm_svg-0.0.2/ssm_svg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 08:57:57.000000 ssm_svg-0.0.2/ssm_svg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 08:57:57.000000 ssm_svg-0.0.2/ssm_svg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:57:57.364526 ssm_svg-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-02 08:57:49.000000 ssm_svg-0.0.2/tests/test_ssm.py
```

### Comparing `ssm-svg-0.0.1/LICENSE` & `ssm_svg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssm-svg-0.0.1/PKG-INFO` & `ssm_svg-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-svg
-Version: 0.0.1
+Version: 0.0.2
 Summary: SVG spritesheet maker
 Home-page: https://github.com/obeezzy/ssm
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ssm-svg-0.0.1/README.md` & `ssm_svg-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ssm-svg-0.0.1/setup.py` & `ssm_svg-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (ROOT_DIR / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="ssm-svg",
-    version="0.0.1",
+    version="0.0.2",
     description="SVG spritesheet maker",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/obeezzy/ssm",
     author="Chronic Coder",
     author_email="efeoghene.obebeduo@gmail.com",
     license="MIT",
@@ -22,8 +22,11 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     packages=find_packages(exclude=("tests",)),
     include_package_data=True,
     install_requires=["lxml"],
+    entry_points={
+        "console_scripts": ["ssm=ssm.ssm:main"]
+    },
 )
```

### Comparing `ssm-svg-0.0.1/ssm_svg.egg-info/PKG-INFO` & `ssm_svg-0.0.2/ssm_svg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-svg
-Version: 0.0.1
+Version: 0.0.2
 Summary: SVG spritesheet maker
 Home-page: https://github.com/obeezzy/ssm
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ssm-svg-0.0.1/tests/test_ssm.py` & `ssm_svg-0.0.2/tests/test_ssm.py`

 * *Files identical despite different names*

