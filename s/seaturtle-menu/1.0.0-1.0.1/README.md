# Comparing `tmp/seaturtle_menu-1.0.0.tar.gz` & `tmp/seaturtle_menu-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaturtle_menu-1.0.0.tar", last modified: Thu May  2 18:57:52 2024, max compression
+gzip compressed data, was "seaturtle_menu-1.0.1.tar", last modified: Thu May  2 19:40:18 2024, max compression
```

## Comparing `seaturtle_menu-1.0.0.tar` & `seaturtle_menu-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 18:57:52.087288 seaturtle_menu-1.0.0/
--rw-rw-r--   0 tathya    (1000) tathya    (1000)     1058 2024-05-02 16:30:48.000000 seaturtle_menu-1.0.0/LICENSE
--rw-r--r--   0 tathya    (1000) tathya    (1000)     2143 2024-05-02 18:57:52.087288 seaturtle_menu-1.0.0/PKG-INFO
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      377 2024-05-02 17:28:04.000000 seaturtle_menu-1.0.0/README.md
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      756 2024-05-02 18:56:39.000000 seaturtle_menu-1.0.0/pyproject.toml
-drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 18:57:52.083288 seaturtle_menu-1.0.0/seaturtle_menu/
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      331 2024-05-02 18:57:12.000000 seaturtle_menu-1.0.0/seaturtle_menu/__init__.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)     2575 2024-05-02 18:51:21.000000 seaturtle_menu-1.0.0/seaturtle_menu/bullets.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)       81 2024-05-02 16:19:13.000000 seaturtle_menu-1.0.0/seaturtle_menu/consts.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)     3167 2024-05-02 18:54:47.000000 seaturtle_menu-1.0.0/seaturtle_menu/menu.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      229 2024-05-02 13:25:08.000000 seaturtle_menu-1.0.0/seaturtle_menu/utils.py
-drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 18:57:52.083288 seaturtle_menu-1.0.0/seaturtle_menu.egg-info/
--rw-r--r--   0 tathya    (1000) tathya    (1000)     2143 2024-05-02 18:57:52.000000 seaturtle_menu-1.0.0/seaturtle_menu.egg-info/PKG-INFO
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      318 2024-05-02 18:57:52.000000 seaturtle_menu-1.0.0/seaturtle_menu.egg-info/SOURCES.txt
--rw-rw-r--   0 tathya    (1000) tathya    (1000)        1 2024-05-02 18:57:52.000000 seaturtle_menu-1.0.0/seaturtle_menu.egg-info/dependency_links.txt
--rw-rw-r--   0 tathya    (1000) tathya    (1000)       15 2024-05-02 18:57:52.000000 seaturtle_menu-1.0.0/seaturtle_menu.egg-info/top_level.txt
--rw-rw-r--   0 tathya    (1000) tathya    (1000)       38 2024-05-02 18:57:52.087288 seaturtle_menu-1.0.0/setup.cfg
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      666 2024-05-02 18:56:55.000000 seaturtle_menu-1.0.0/setup.py
+drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 19:40:18.406342 seaturtle_menu-1.0.1/
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)     1058 2024-05-02 16:30:48.000000 seaturtle_menu-1.0.1/LICENSE
+-rw-r--r--   0 tathya    (1000) tathya    (1000)     2143 2024-05-02 19:40:18.406342 seaturtle_menu-1.0.1/PKG-INFO
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      377 2024-05-02 17:28:04.000000 seaturtle_menu-1.0.1/README.md
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      756 2024-05-02 19:39:27.000000 seaturtle_menu-1.0.1/pyproject.toml
+drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 19:40:18.406342 seaturtle_menu-1.0.1/seaturtle_menu/
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      331 2024-05-02 19:39:32.000000 seaturtle_menu-1.0.1/seaturtle_menu/__init__.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)     2575 2024-05-02 18:51:21.000000 seaturtle_menu-1.0.1/seaturtle_menu/bullets.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)       81 2024-05-02 16:19:13.000000 seaturtle_menu-1.0.1/seaturtle_menu/consts.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)     3101 2024-05-02 19:38:23.000000 seaturtle_menu-1.0.1/seaturtle_menu/menu.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      229 2024-05-02 13:25:08.000000 seaturtle_menu-1.0.1/seaturtle_menu/utils.py
+drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 19:40:18.406342 seaturtle_menu-1.0.1/seaturtle_menu.egg-info/
+-rw-r--r--   0 tathya    (1000) tathya    (1000)     2143 2024-05-02 19:40:18.000000 seaturtle_menu-1.0.1/seaturtle_menu.egg-info/PKG-INFO
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      318 2024-05-02 19:40:18.000000 seaturtle_menu-1.0.1/seaturtle_menu.egg-info/SOURCES.txt
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)        1 2024-05-02 19:40:18.000000 seaturtle_menu-1.0.1/seaturtle_menu.egg-info/dependency_links.txt
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)       15 2024-05-02 19:40:18.000000 seaturtle_menu-1.0.1/seaturtle_menu.egg-info/top_level.txt
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)       38 2024-05-02 19:40:18.406342 seaturtle_menu-1.0.1/setup.cfg
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      666 2024-05-02 19:39:22.000000 seaturtle_menu-1.0.1/setup.py
```

### Comparing `seaturtle_menu-1.0.0/LICENSE` & `seaturtle_menu-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seaturtle_menu-1.0.0/PKG-INFO` & `seaturtle_menu-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaturtle_menu
-Version: 1.0.0
+Version: 1.0.1
 Summary: Make effective terminal menus quickly and concisely.
 Author: Tathya Garg
 Author-email: Tathya Garg <tathya.garg@gmail.com>
 Maintainer-email: Tathya Garg <tathya.garg@gmail.com>
 License: Copyright 2024 Tathya Garg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `seaturtle_menu-1.0.0/pyproject.toml` & `seaturtle_menu-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "seaturtle_menu"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = []
 requires-python = ">=3.12"
 authors = [
   {name = "Tathya Garg", email = "tathya.garg@gmail.com"},
 ]
 maintainers = [
   {name = "Tathya Garg", email = "tathya.garg@gmail.com"},
```

### Comparing `seaturtle_menu-1.0.0/seaturtle_menu/bullets.py` & `seaturtle_menu-1.0.1/seaturtle_menu/bullets.py`

 * *Files identical despite different names*

### Comparing `seaturtle_menu-1.0.0/seaturtle_menu/menu.py` & `seaturtle_menu-1.0.1/seaturtle_menu/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
             size: int = len(self.prompts)
             width = 0
             while size:
                 width += 1
                 size //= _bullets.charset_len + 1
 
             self.width = width
-            print(width, len(self.prompts), _bullets.charset_len)
 
             self.bullets = _bullets.from_width(self.width)
         else:
             self.width = _bullets.width
             self.bullets = _bullets
 
         self.bullets_as_list = list(self.bullets)[:len(self.prompts)]
```

### Comparing `seaturtle_menu-1.0.0/seaturtle_menu.egg-info/PKG-INFO` & `seaturtle_menu-1.0.1/seaturtle_menu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaturtle_menu
-Version: 1.0.0
+Version: 1.0.1
 Summary: Make effective terminal menus quickly and concisely.
 Author: Tathya Garg
 Author-email: Tathya Garg <tathya.garg@gmail.com>
 Maintainer-email: Tathya Garg <tathya.garg@gmail.com>
 License: Copyright 2024 Tathya Garg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `seaturtle_menu-1.0.0/setup.py` & `seaturtle_menu-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Make effective terminal menus quickly and concisely.'
 
 setup(
     name='seaturtle_menu',
     version=VERSION,
     author='Tathya Garg',
     author_email='tathya.garg@gmail.com',
```

