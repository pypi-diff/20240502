# Comparing `tmp/search_buddy-1.1.3.tar.gz` & `tmp/search_buddy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search_buddy-1.1.3.tar", last modified: Mon Sep  5 05:41:46 2022, max compression
+gzip compressed data, was "search_buddy-1.1.4.tar", last modified: Thu May  2 15:47:28 2024, max compression
```

## Comparing `search_buddy-1.1.3.tar` & `search_buddy-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ajlinux   (1000) ajlinux   (1000)        0 2022-09-05 05:41:46.413699 search_buddy-1.1.3/
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)     1076 2022-08-01 13:12:11.000000 search_buddy-1.1.3/LICENSE.txt
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)      557 2022-09-05 05:41:46.413699 search_buddy-1.1.3/PKG-INFO
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)     1521 2022-08-02 04:18:15.000000 search_buddy-1.1.3/README.md
-drwxrwxr-x   0 ajlinux   (1000) ajlinux   (1000)        0 2022-09-05 05:41:46.413699 search_buddy-1.1.3/search_buddy/
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)        0 2022-08-01 13:13:29.000000 search_buddy-1.1.3/search_buddy/__init__.py
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)       55 2022-08-03 02:13:11.000000 search_buddy-1.1.3/search_buddy/command_line.py
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)     5064 2022-09-05 05:40:37.000000 search_buddy-1.1.3/search_buddy/search_buddy.py
-drwxrwxr-x   0 ajlinux   (1000) ajlinux   (1000)        0 2022-09-05 05:41:46.413699 search_buddy-1.1.3/search_buddy.egg-info/
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)      557 2022-09-05 05:41:46.000000 search_buddy-1.1.3/search_buddy.egg-info/PKG-INFO
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)      331 2022-09-05 05:41:46.000000 search_buddy-1.1.3/search_buddy.egg-info/SOURCES.txt
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)        1 2022-09-05 05:41:46.000000 search_buddy-1.1.3/search_buddy.egg-info/dependency_links.txt
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)       74 2022-09-05 05:41:46.000000 search_buddy-1.1.3/search_buddy.egg-info/entry_points.txt
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)       34 2022-09-05 05:41:46.000000 search_buddy-1.1.3/search_buddy.egg-info/requires.txt
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)       13 2022-09-05 05:41:46.000000 search_buddy-1.1.3/search_buddy.egg-info/top_level.txt
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)       38 2022-09-05 05:41:46.413699 search_buddy-1.1.3/setup.cfg
--rw-rw-r--   0 ajlinux   (1000) ajlinux   (1000)     1058 2022-09-05 05:40:44.000000 search_buddy-1.1.3/setup.py
+drwxrwxr-x   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)        0 2024-05-02 15:47:28.250547 search_buddy-1.1.4/
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)     1076 2022-08-01 13:12:11.000000 search_buddy-1.1.4/LICENSE.txt
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)      557 2024-05-02 15:47:28.250547 search_buddy-1.1.4/PKG-INFO
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)     1521 2022-08-02 04:18:15.000000 search_buddy-1.1.4/README.md
+drwxrwxr-x   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)        0 2024-05-02 15:47:28.250547 search_buddy-1.1.4/search_buddy/
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)        0 2022-08-01 13:13:29.000000 search_buddy-1.1.4/search_buddy/__init__.py
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)       55 2022-08-03 02:13:11.000000 search_buddy-1.1.4/search_buddy/command_line.py
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)     5742 2024-05-02 15:41:04.000000 search_buddy-1.1.4/search_buddy/search_buddy.py
+drwxrwxr-x   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)        0 2024-05-02 15:47:28.250547 search_buddy-1.1.4/search_buddy.egg-info/
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)      557 2024-05-02 15:47:28.000000 search_buddy-1.1.4/search_buddy.egg-info/PKG-INFO
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)      331 2024-05-02 15:47:28.000000 search_buddy-1.1.4/search_buddy.egg-info/SOURCES.txt
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)        1 2024-05-02 15:47:28.000000 search_buddy-1.1.4/search_buddy.egg-info/dependency_links.txt
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)       75 2024-05-02 15:47:28.000000 search_buddy-1.1.4/search_buddy.egg-info/entry_points.txt
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)       34 2024-05-02 15:47:28.000000 search_buddy-1.1.4/search_buddy.egg-info/requires.txt
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)        1 2024-05-02 15:47:28.000000 search_buddy-1.1.4/search_buddy.egg-info/top_level.txt
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)       38 2024-05-02 15:47:28.250547 search_buddy-1.1.4/setup.cfg
+-rw-rw-r--   0 aspiring-aardvark  (1000) aspiring-aardvark  (1000)     1058 2024-05-02 15:41:25.000000 search_buddy-1.1.4/setup.py
```

### Comparing `search_buddy-1.1.3/LICENSE.txt` & `search_buddy-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `search_buddy-1.1.3/PKG-INFO` & `search_buddy-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: search_buddy
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool to simplify initial literature searches
 Home-page: https://github.com/soapGame34/lib-search-buddy
 Author: Alexander J. Calder
 Author-email: alexcalder91@gmail.com
 License: MIT
 Keywords: research literature-search
 Platform: UNKNOWN
```

### Comparing `search_buddy-1.1.3/README.md` & `search_buddy-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `search_buddy-1.1.3/search_buddy.egg-info/PKG-INFO` & `search_buddy-1.1.4/search_buddy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: search-buddy
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool to simplify initial literature searches
 Home-page: https://github.com/soapGame34/lib-search-buddy
 Author: Alexander J. Calder
 Author-email: alexcalder91@gmail.com
 License: MIT
 Keywords: research literature-search
 Platform: UNKNOWN
```

### Comparing `search_buddy-1.1.3/setup.py` & `search_buddy-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'Topic :: Terminals',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     ]
   
 # calling the setup function 
 setup(name='search_buddy',
-      version='1.1.3',
+      version='1.1.4',
       description='A tool to simplify initial literature searches',
       #long_description=long_description,
       url='https://github.com/soapGame34/lib-search-buddy',
       author='Alexander J. Calder',
       author_email='alexcalder91@gmail.com',
       license='MIT',
       entry_points = { 'console_scripts' : ['litsearch = search_buddy.search_buddy.command_line:main']},
```

