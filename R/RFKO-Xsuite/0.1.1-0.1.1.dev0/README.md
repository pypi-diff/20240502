# Comparing `tmp/rfko_xsuite-0.1.1.tar.gz` & `tmp/rfko_xsuite-0.1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfko_xsuite-0.1.1.tar", last modified: Wed May  1 15:53:35 2024, max compression
+gzip compressed data, was "rfko_xsuite-0.1.1.dev0.tar", last modified: Thu May  2 18:16:03 2024, max compression
```

## Comparing `rfko_xsuite-0.1.1.tar` & `rfko_xsuite-0.1.1.dev0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 15:53:35.393930 rfko_xsuite-0.1.1/
--rw-rw-rw-   0        0        0      548 2024-05-01 15:53:35.391772 rfko_xsuite-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-03-27 10:33:56.000000 rfko_xsuite-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 15:53:35.375902 rfko_xsuite-0.1.1/RFKO_Xsuite/
--rw-rw-rw-   0        0        0    30632 2024-04-12 09:43:59.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/Rfko.py
--rw-rw-rw-   0        0        0      724 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/__init__.py
--rw-rw-rw-   0        0        0    14307 2024-01-15 14:53:41.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/bare_mach_setup.py
--rw-rw-rw-   0        0        0     9841 2024-03-05 17:58:46.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/check_functions.py
--rw-rw-rw-   0        0        0    32863 2024-03-05 17:58:47.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/line_setup.py
--rw-rw-rw-   0        0        0    29653 2024-01-15 16:29:04.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/macro.py
--rw-rw-rw-   0        0        0     8087 2024-04-08 14:11:35.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/phy_helper.py
--rw-rw-rw-   0        0        0    28736 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/plotting1.py
--rw-rw-rw-   0        0        0    28440 2024-02-15 16:37:06.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/plotting2.py
--rw-rw-rw-   0        0        0    16009 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/quad_ripples.py
--rw-rw-rw-   0        0        0     2293 2024-04-25 15:13:09.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/saving.py
--rw-rw-rw-   0        0        0    19516 2024-04-12 09:38:07.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/slowex_actions.py
--rw-rw-rw-   0        0        0    12126 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/slowex_helper.py
--rw-rw-rw-   0        0        0     5017 2024-04-25 15:04:10.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/utility.py
--rw-rw-rw-   0        0        0     6564 2024-02-26 15:04:56.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/xsuite_actions.py
--rw-rw-rw-   0        0        0    23120 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1/RFKO_Xsuite/xsuite_helper.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:53:35.390769 rfko_xsuite-0.1.1/RFKO_Xsuite.egg-info/
--rw-rw-rw-   0        0        0      548 2024-05-01 15:53:35.000000 rfko_xsuite-0.1.1/RFKO_Xsuite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2024-05-01 15:53:35.000000 rfko_xsuite-0.1.1/RFKO_Xsuite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 15:53:35.000000 rfko_xsuite-0.1.1/RFKO_Xsuite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-01 15:53:35.000000 rfko_xsuite-0.1.1/RFKO_Xsuite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-01 15:53:35.000000 rfko_xsuite-0.1.1/RFKO_Xsuite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 15:53:35.393930 rfko_xsuite-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      772 2024-05-01 15:52:41.000000 rfko_xsuite-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:53:35.388259 rfko_xsuite-0.1.1/tests/
--rw-rw-rw-   0        0        0      559 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1/tests/test1.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:16:03.937286 rfko_xsuite-0.1.1.dev0/
+-rw-rw-rw-   0        0        0     1443 2024-05-02 18:16:03.934148 rfko_xsuite-0.1.1.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-03-27 10:33:56.000000 rfko_xsuite-0.1.1.dev0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 18:16:03.899741 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/
+-rw-rw-rw-   0        0        0    30632 2024-04-12 09:43:59.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/Rfko.py
+-rw-rw-rw-   0        0        0      724 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/__init__.py
+-rw-rw-rw-   0        0        0    14307 2024-01-15 14:53:41.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/bare_mach_setup.py
+-rw-rw-rw-   0        0        0     9841 2024-03-05 17:58:46.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/check_functions.py
+-rw-rw-rw-   0        0        0    32863 2024-03-05 17:58:47.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/line_setup.py
+-rw-rw-rw-   0        0        0    29653 2024-01-15 16:29:04.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/macro.py
+-rw-rw-rw-   0        0        0     8087 2024-04-08 14:11:35.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/phy_helper.py
+-rw-rw-rw-   0        0        0    28736 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/plotting1.py
+-rw-rw-rw-   0        0        0    28440 2024-02-15 16:37:06.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/plotting2.py
+-rw-rw-rw-   0        0        0    16009 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/quad_ripples.py
+-rw-rw-rw-   0        0        0     2293 2024-04-25 15:13:09.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/saving.py
+-rw-rw-rw-   0        0        0    19516 2024-04-12 09:38:07.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/slowex_actions.py
+-rw-rw-rw-   0        0        0    12126 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/slowex_helper.py
+-rw-rw-rw-   0        0        0     5017 2024-04-25 15:04:10.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/utility.py
+-rw-rw-rw-   0        0        0     6564 2024-02-26 15:04:56.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/xsuite_actions.py
+-rw-rw-rw-   0        0        0    23120 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/xsuite_helper.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:16:03.931687 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite.egg-info/
+-rw-rw-rw-   0        0        0     1443 2024-05-02 18:16:03.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      652 2024-05-02 18:16:03.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 18:16:03.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      540 2024-05-02 18:16:03.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-02 18:16:03.000000 rfko_xsuite-0.1.1.dev0/RFKO_Xsuite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 18:16:03.937286 rfko_xsuite-0.1.1.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-05-02 18:15:53.000000 rfko_xsuite-0.1.1.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:16:03.927340 rfko_xsuite-0.1.1.dev0/tests/
+-rw-rw-rw-   0        0        0      294 2024-05-02 15:51:38.000000 rfko_xsuite-0.1.1.dev0/tests/test_basic.py
+-rw-rw-rw-   0        0        0      559 2024-05-01 15:50:01.000000 rfko_xsuite-0.1.1.dev0/tests/test_class.py
```

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/Rfko.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/Rfko.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/__init__.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/bare_mach_setup.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/bare_mach_setup.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/check_functions.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/check_functions.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/line_setup.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/line_setup.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/macro.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/macro.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/phy_helper.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/phy_helper.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/plotting1.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/plotting1.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/plotting2.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/plotting2.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/quad_ripples.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/quad_ripples.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/saving.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/saving.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/slowex_actions.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/slowex_actions.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/slowex_helper.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/slowex_helper.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/utility.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/utility.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/xsuite_actions.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/xsuite_actions.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite/xsuite_helper.py` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite/xsuite_helper.py`

 * *Files identical despite different names*

### Comparing `rfko_xsuite-0.1.1/RFKO_Xsuite.egg-info/SOURCES.txt` & `rfko_xsuite-0.1.1.dev0/RFKO_Xsuite.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 RFKO_Xsuite/xsuite_actions.py
 RFKO_Xsuite/xsuite_helper.py
 RFKO_Xsuite.egg-info/PKG-INFO
 RFKO_Xsuite.egg-info/SOURCES.txt
 RFKO_Xsuite.egg-info/dependency_links.txt
 RFKO_Xsuite.egg-info/requires.txt
 RFKO_Xsuite.egg-info/top_level.txt
-tests/test1.py
+tests/test_basic.py
+tests/test_class.py
```

### Comparing `rfko_xsuite-0.1.1/setup.py` & `rfko_xsuite-0.1.1.dev0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md",
           "r", encoding="utf-8") as file:
     long_description = file.read()
 
+# Read requirements.txt
+with open('requirements.txt', 'r', encoding='utf-16') as f:
+    required = f.read().splitlines()
 ### xcoll not considered for now
 
 setup(
     name='RFKO_Xsuite',
-    version='0.1.1',
-    packages=find_packages(exclude=['tests*']),
+    version='0.1.1dev',
+    packages=['RFKO_Xsuite'],#find_packages(exclude=['tests*']),
     license='MIT',
     description='A package for wrapping up some funcitonalities from Xsuite',
     long_description=long_description,
-    install_requires=['xsuite','xpart','xobjects','xtrack','xcoll','cpymad','matplotlib'
-        ,'numpy', 'pandas'],  # add any additional packages you want to include here
+    install_requires=required,  # add any additional packages you want to include here
     url='https://gitlab.cern.ch/wscarpa/rfko_xsuite.git',  # replace with your package's url
     author='Wesley',
     author_email='wesley.scarpa@cern.ch'
 )
```

### Comparing `rfko_xsuite-0.1.1/tests/test1.py` & `rfko_xsuite-0.1.1.dev0/tests/test_class.py`

 * *Files identical despite different names*

