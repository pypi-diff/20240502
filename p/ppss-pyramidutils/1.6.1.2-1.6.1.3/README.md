# Comparing `tmp/ppss_pyramidutils-1.6.1.2.tar.gz` & `tmp/ppss_pyramidutils-1.6.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppss_pyramidutils-1.6.1.2.tar", last modified: Wed Feb  7 14:10:22 2024, max compression
+gzip compressed data, was "ppss_pyramidutils-1.6.1.3.tar", last modified: Thu May  2 09:20:13 2024, max compression
```

## Comparing `ppss_pyramidutils-1.6.1.2.tar` & `ppss_pyramidutils-1.6.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-02-07 14:10:22.303177 ppss_pyramidutils-1.6.1.2/
--rw-r--r--   0 dan       (1000) dan       (1000)      152 2024-01-26 17:51:06.000000 ppss_pyramidutils-1.6.1.2/MANIFEST.in
--rw-r--r--   0 dan       (1000) dan       (1000)     8370 2024-02-07 14:10:22.303177 ppss_pyramidutils-1.6.1.2/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     6999 2024-01-26 17:51:06.000000 ppss_pyramidutils-1.6.1.2/README.md
--rw-r--r--   0 dan       (1000) dan       (1000)      836 2024-02-02 13:15:07.000000 ppss_pyramidutils-1.6.1.2/change.log
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-02-07 14:10:22.303177 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/
--rw-r--r--   0 dan       (1000) dan       (1000)      445 2024-01-26 17:51:06.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)      363 2024-01-26 17:51:06.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/appsettings.py
--rw-r--r--   0 dan       (1000) dan       (1000)     3628 2024-01-26 17:51:06.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/backgroundjobs.py
--rw-r--r--   0 dan       (1000) dan       (1000)     4020 2024-02-06 09:22:00.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/cryptoutils.py
--rw-r--r--   0 dan       (1000) dan       (1000)     3190 2024-01-26 17:51:06.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/filemanager.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1108 2024-02-02 13:13:20.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/jsonutils.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1963 2024-01-26 17:51:06.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/modelbase.py
--rw-r--r--   0 dan       (1000) dan       (1000)      890 2024-01-26 17:51:06.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/scriptbase.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1111 2024-01-26 17:51:06.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/sessionhandling.py
--rw-r--r--   0 dan       (1000) dan       (1000)     6136 2024-01-26 17:51:06.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/utf8csv.py
--rw-r--r--   0 dan       (1000) dan       (1000)     4500 2024-02-07 11:44:53.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/utils.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-02-07 14:10:22.303177 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils.egg-info/
--rw-r--r--   0 dan       (1000) dan       (1000)     8370 2024-02-07 14:10:22.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils.egg-info/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)      597 2024-02-07 14:10:22.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils.egg-info/SOURCES.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2024-02-07 14:10:22.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils.egg-info/dependency_links.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       34 2024-02-07 14:10:22.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils.egg-info/requires.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       18 2024-02-07 14:10:22.000000 ppss_pyramidutils-1.6.1.2/ppss_pyramidutils.egg-info/top_level.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2024-02-07 14:10:22.303177 ppss_pyramidutils-1.6.1.2/setup.cfg
--rw-r--r--   0 dan       (1000) dan       (1000)     1147 2024-02-07 11:58:18.000000 ppss_pyramidutils-1.6.1.2/setup.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-05-02 09:20:13.360809 ppss_pyramidutils-1.6.1.3/
+-rw-r--r--   0 dan       (1000) dan       (1000)      152 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/MANIFEST.in
+-rw-r--r--   0 dan       (1000) dan       (1000)     8410 2024-05-02 09:20:13.360809 ppss_pyramidutils-1.6.1.3/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     6999 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/README.md
+-rw-r--r--   0 dan       (1000) dan       (1000)      876 2024-05-02 09:19:00.000000 ppss_pyramidutils-1.6.1.3/change.log
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-05-02 09:20:13.360809 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/
+-rw-r--r--   0 dan       (1000) dan       (1000)      445 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      363 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/appsettings.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     3628 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/backgroundjobs.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     4020 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/cryptoutils.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     3190 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/filemanager.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1108 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/jsonutils.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1963 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/modelbase.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      890 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/scriptbase.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1111 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/sessionhandling.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     6158 2024-05-02 08:46:00.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/utf8csv.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     4500 2024-05-02 08:42:47.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/utils.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-05-02 09:20:13.360809 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils.egg-info/
+-rw-r--r--   0 dan       (1000) dan       (1000)     8410 2024-05-02 09:20:13.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils.egg-info/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)      597 2024-05-02 09:20:13.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils.egg-info/SOURCES.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2024-05-02 09:20:13.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils.egg-info/dependency_links.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       34 2024-05-02 09:20:13.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils.egg-info/requires.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       18 2024-05-02 09:20:13.000000 ppss_pyramidutils-1.6.1.3/ppss_pyramidutils.egg-info/top_level.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2024-05-02 09:20:13.360809 ppss_pyramidutils-1.6.1.3/setup.cfg
+-rw-r--r--   0 dan       (1000) dan       (1000)     1147 2024-05-02 09:18:34.000000 ppss_pyramidutils-1.6.1.3/setup.py
```

### Comparing `ppss_pyramidutils-1.6.1.2/PKG-INFO` & `ppss_pyramidutils-1.6.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppss_pyramidutils
-Version: 1.6.1.2
+Version: 1.6.1.3
 Summary: Simple utils to handle data from ini files in Pyramid for python 2.7 & 3
 Home-page: UNKNOWN
 Author: pdepmcp
 Author-email: pdepmcp@gmail.com
 License: UNKNOWN
 Keywords: pyramid module utils accelerator
 Platform: UNKNOWN
@@ -145,14 +145,17 @@
 
 
 
 
 
 
 
+__v1.6.1.3
+fix "quote all" in exporter
+
 __v1.6.1
 added skip rows to jsonwalker
 
 __v1.6.0
 added cryptoutils and jsonutils
 
 __v1.5.4.0
```

### Comparing `ppss_pyramidutils-1.6.1.2/README.md` & `ppss_pyramidutils-1.6.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ppss_pyramidutils-1.6.1.2/change.log` & `ppss_pyramidutils-1.6.1.3/change.log`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__v1.6.1.3
+fix "quote all" in exporter
+
 __v1.6.1
 added skip rows to jsonwalker
 
 __v1.6.0
 added cryptoutils and jsonutils
 
 __v1.5.4.0
```

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/backgroundjobs.py` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/backgroundjobs.py`

 * *Files identical despite different names*

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/cryptoutils.py` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/cryptoutils.py`

 * *Files identical despite different names*

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/filemanager.py` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/filemanager.py`

 * *Files identical despite different names*

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/jsonutils.py` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/jsonutils.py`

 * *Files identical despite different names*

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/modelbase.py` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/modelbase.py`

 * *Files identical despite different names*

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/scriptbase.py` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/scriptbase.py`

 * *Files identical despite different names*

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/sessionhandling.py` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/sessionhandling.py`

 * *Files identical despite different names*

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/utf8csv.py` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/utf8csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 
     def writeAll(self, delimiter = None):
         d = delimiter if delimiter else self.delimiter if self.delimiter else ','
         if PY2:
             w = UnicodeWriter(self.retfile, delimiter=d, quoting=csv.QUOTE_ALL)
         else:
-            w = csv.writer(self.retfile, dialect=csv.excel, delimiter = d)
+            w = csv.writer(self.retfile, dialect=csv.excel, delimiter = d,quoting=csv.QUOTE_ALL)
         w.writerow(self.titles)
         for maprow in self.evl:
             l.info("*******{row}".format(row=maprow) )
             w.writerow(maprow)
         self.retfile.seek(0, 0)
         return self.retfile
```

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils/utils.py` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils/utils.py`

 * *Files identical despite different names*

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils.egg-info/PKG-INFO` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppss-pyramidutils
-Version: 1.6.1.2
+Version: 1.6.1.3
 Summary: Simple utils to handle data from ini files in Pyramid for python 2.7 & 3
 Home-page: UNKNOWN
 Author: pdepmcp
 Author-email: pdepmcp@gmail.com
 License: UNKNOWN
 Keywords: pyramid module utils accelerator
 Platform: UNKNOWN
@@ -145,14 +145,17 @@
 
 
 
 
 
 
 
+__v1.6.1.3
+fix "quote all" in exporter
+
 __v1.6.1
 added skip rows to jsonwalker
 
 __v1.6.0
 added cryptoutils and jsonutils
 
 __v1.5.4.0
```

### Comparing `ppss_pyramidutils-1.6.1.2/ppss_pyramidutils.egg-info/SOURCES.txt` & `ppss_pyramidutils-1.6.1.3/ppss_pyramidutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ppss_pyramidutils-1.6.1.2/setup.py` & `ppss_pyramidutils-1.6.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 here = os.path.abspath(os.path.dirname(__file__))
 readme = open(os.path.join(here, 'README.md'), 'r').read()
 changelog = open(os.path.join(here, 'change.log'), 'r').read()
 
 
 setup(name='ppss_pyramidutils',
-      version='1.6.1.2',
+      version='1.6.1.3',
       description='Simple utils to handle data from ini files in Pyramid for python 2.7 & 3',
       long_description=readme + "\n\n\n" + changelog,
       long_description_content_type="text/markdown",
       author='pdepmcp',
       author_email='pdepmcp@gmail.com',
       install_requires=[
         'six',
```

