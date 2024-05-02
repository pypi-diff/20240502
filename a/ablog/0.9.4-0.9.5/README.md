# Comparing `tmp/ablog-0.9.4.tar.gz` & `tmp/ablog-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ablog-0.9.4.tar", last modified: Sun Feb 10 21:07:17 2019, max compression
+gzip compressed data, was "dist/ablog-0.9.5.tar", last modified: Mon Aug 19 21:18:29 2019, max compression
```

## Comparing `ablog-0.9.4.tar` & `ablog-0.9.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/
--rw-r--r--   0 nabil     (1000) users      (985)     1113 2018-06-29 13:37:24.000000 ablog-0.9.4/LICENSE.rst
--rw-r--r--   0 nabil     (1000) users      (985)      183 2018-06-29 13:37:24.000000 ablog-0.9.4/MANIFEST.in
--rw-r--r--   0 nabil     (1000) users      (985)     1401 2019-02-10 21:07:17.000000 ablog-0.9.4/PKG-INFO
--rw-r--r--   0 nabil     (1000) users      (985)     4112 2019-02-10 20:55:34.000000 ablog-0.9.4/README.rst
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/
--rwxr-xr-x   0 nabil     (1000) users      (985)     2884 2019-02-10 21:02:26.000000 ablog-0.9.4/ablog/__init__.py
--rw-r--r--   0 nabil     (1000) users      (985)    17965 2018-12-06 11:38:56.000000 ablog-0.9.4/ablog/blog.py
--rw-r--r--   0 nabil     (1000) users      (985)    14605 2019-02-10 20:55:34.000000 ablog-0.9.4/ablog/commands.py
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/de/
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/de/LC_MESSAGES/
--rw-r--r--   0 nabil     (1000) users      (985)     1297 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/de/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 nabil     (1000) users      (985)     2539 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/de/LC_MESSAGES/sphinx.po
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/es/
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/es/LC_MESSAGES/
--rw-r--r--   0 nabil     (1000) users      (985)     1331 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/es/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 nabil     (1000) users      (985)     2578 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/es/LC_MESSAGES/sphinx.po
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/et/
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/et/LC_MESSAGES/
--rw-r--r--   0 nabil     (1000) users      (985)     1302 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/et/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 nabil     (1000) users      (985)     2528 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/et/LC_MESSAGES/sphinx.po
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/ru/
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/ru/LC_MESSAGES/
--rw-r--r--   0 nabil     (1000) users      (985)     1662 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/ru/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 nabil     (1000) users      (985)     2786 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/ru/LC_MESSAGES/sphinx.po
--rw-r--r--   0 nabil     (1000) users      (985)     2264 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/sphinx.pot
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/tr/
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/locale/tr/LC_MESSAGES/
--rw-r--r--   0 nabil     (1000) users      (985)     1239 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/tr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 nabil     (1000) users      (985)     2482 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/locale/tr/LC_MESSAGES/sphinx.po
--rw-r--r--   0 nabil     (1000) users      (985)    23810 2018-12-06 11:22:20.000000 ablog-0.9.4/ablog/post.py
--rw-r--r--   0 nabil     (1000) users      (985)    21517 2018-10-27 10:15:52.000000 ablog-0.9.4/ablog/start.py
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog/templates/
--rw-r--r--   0 nabil     (1000) users      (985)      305 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/templates/archives.html
--rw-r--r--   0 nabil     (1000) users      (985)      298 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/templates/authors.html
--rw-r--r--   0 nabil     (1000) users      (985)      760 2019-02-10 20:55:34.000000 ablog-0.9.4/ablog/templates/catalog.html
--rw-r--r--   0 nabil     (1000) users      (985)      307 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/templates/categories.html
--rw-r--r--   0 nabil     (1000) users      (985)     1755 2019-02-10 20:55:34.000000 ablog-0.9.4/ablog/templates/collection.html
--rw-r--r--   0 nabil     (1000) users      (985)      306 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/templates/languages.html
--rw-r--r--   0 nabil     (1000) users      (985)      306 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/templates/locations.html
--rw-r--r--   0 nabil     (1000) users      (985)     2302 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/templates/page.html
--rw-r--r--   0 nabil     (1000) users      (985)      495 2019-02-10 20:55:34.000000 ablog-0.9.4/ablog/templates/postcard.html
--rw-r--r--   0 nabil     (1000) users      (985)     3607 2019-02-10 20:55:34.000000 ablog-0.9.4/ablog/templates/postcard2.html
--rw-r--r--   0 nabil     (1000) users      (985)      813 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/templates/postnavy.html
--rw-r--r--   0 nabil     (1000) users      (985)      377 2019-02-10 20:55:34.000000 ablog-0.9.4/ablog/templates/recentposts.html
--rw-r--r--   0 nabil     (1000) users      (985)      351 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/templates/redirect.html
--rw-r--r--   0 nabil     (1000) users      (985)      809 2018-06-29 13:37:24.000000 ablog-0.9.4/ablog/templates/tagcloud.html
-drwxr-xr-x   0 nabil     (1000) users      (985)        0 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog.egg-info/
--rw-r--r--   0 nabil     (1000) users      (985)     1401 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog.egg-info/PKG-INFO
--rw-r--r--   0 nabil     (1000) users      (985)     1126 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog.egg-info/SOURCES.txt
--rw-r--r--   0 nabil     (1000) users      (985)        1 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog.egg-info/dependency_links.txt
--rw-r--r--   0 nabil     (1000) users      (985)       53 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog.egg-info/entry_points.txt
--rw-r--r--   0 nabil     (1000) users      (985)       72 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog.egg-info/requires.txt
--rw-r--r--   0 nabil     (1000) users      (985)        6 2019-02-10 21:07:17.000000 ablog-0.9.4/ablog.egg-info/top_level.txt
--rw-r--r--   0 nabil     (1000) users      (985)       38 2019-02-10 21:07:17.000000 ablog-0.9.4/setup.cfg
--rw-r--r--   0 nabil     (1000) users      (985)     2232 2018-10-28 16:14:21.000000 ablog-0.9.4/setup.py
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     1113 2019-08-19 20:43:41.000000 ablog-0.9.5/LICENSE.rst
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      183 2019-08-19 20:43:41.000000 ablog-0.9.5/MANIFEST.in
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     1401 2019-08-19 21:18:29.000000 ablog-0.9.5/PKG-INFO
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     4112 2019-08-19 20:43:41.000000 ablog-0.9.5/README.rst
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/
+-rwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)     2884 2019-08-19 20:59:23.000000 ablog-0.9.5/ablog/__init__.py
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)    18003 2019-08-19 20:59:12.000000 ablog-0.9.5/ablog/blog.py
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)    14605 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/commands.py
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/de/
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     1297 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/de/LC_MESSAGES/sphinx.mo
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     2539 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/de/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/es/
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     1331 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/es/LC_MESSAGES/sphinx.mo
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     2578 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/es/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/et/
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/et/LC_MESSAGES/
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     1302 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/et/LC_MESSAGES/sphinx.mo
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     2528 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/et/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/ru/
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     1662 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/ru/LC_MESSAGES/sphinx.mo
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     2786 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/ru/LC_MESSAGES/sphinx.po
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     2264 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/sphinx.pot
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/tr/
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     1239 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/tr/LC_MESSAGES/sphinx.mo
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     2482 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/locale/tr/LC_MESSAGES/sphinx.po
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)    23684 2019-08-19 20:59:12.000000 ablog-0.9.5/ablog/post.py
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)    21862 2019-08-19 20:59:12.000000 ablog-0.9.5/ablog/start.py
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog/templates/
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      305 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/archives.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      298 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/authors.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      760 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/catalog.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      307 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/categories.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     1755 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/collection.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      306 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/languages.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      306 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/locations.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     2302 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/page.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      495 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/postcard.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     3607 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/postcard2.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      813 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/postnavy.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      377 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/recentposts.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      351 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/redirect.html
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)      809 2019-08-19 20:43:41.000000 ablog-0.9.5/ablog/templates/tagcloud.html
+drwxrwxr-x   0 nabobalis  (1000) nabobalis  (1000)        0 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog.egg-info/
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     1401 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog.egg-info/PKG-INFO
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     1126 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog.egg-info/SOURCES.txt
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)        1 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog.egg-info/dependency_links.txt
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)       53 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog.egg-info/entry_points.txt
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)       72 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog.egg-info/requires.txt
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)        6 2019-08-19 21:18:29.000000 ablog-0.9.5/ablog.egg-info/top_level.txt
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)       38 2019-08-19 21:18:29.000000 ablog-0.9.5/setup.cfg
+-rw-rw-r--   0 nabobalis  (1000) nabobalis  (1000)     2221 2019-08-19 20:59:23.000000 ablog-0.9.5/setup.py
```

### Comparing `ablog-0.9.4/LICENSE.rst` & `ablog-0.9.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/PKG-INFO` & `ablog-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ablog
-Version: 0.9.4
+Version: 0.9.5
 Summary: ABlog allows you to blog with Sphinx
 Home-page: http://ablog.readthedocs.org/
 Author: SunPy Developers
 Author-email: nabil.freij@gmail.com
 License: MIT License
 Description: 
         ABlog for Sphinx
```

### Comparing `ablog-0.9.4/README.rst` & `ablog-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/__init__.py` & `ablog-0.9.5/ablog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .blog import Blog, CONFIG
 from .post import (PostDirective, PostListDirective, UpdateDirective,
                    UpdateNode, process_posts, process_postlist, purge_posts,
                    generate_archive_pages, generate_atom_feeds,
                    missing_reference)
 
-__version__ = '0.9.4'
+__version__ = '0.9.5'
 
 __all__ = ['setup']
 
 
 def anchor(post):
     """Return anchor string for posts that arepage sections."""
```

### Comparing `ablog-0.9.4/ablog/blog.py` & `ablog-0.9.5/ablog/blog.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     ('fontawesome_included', False, True),
     ('fontawesome_css_file', '', True),
 
     ('post_date_format', '%d %B %Y', True),
     ('post_date_format_short', '%d %B', True),
     ('post_auto_image', 0, True),
     ('post_auto_excerpt', 1, True),
+    ('post_auto_orphan', True, True),
     ('post_redirect_refresh', 5, True),
     ('post_always_section', False, True),
 
     ('disqus_shortname', None, True),
     ('disqus_drafts', False, True),
     ('disqus_pages', False, True),
 ]
```

### Comparing `ablog-0.9.4/ablog/commands.py` & `ablog-0.9.5/ablog/commands.py`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/de/LC_MESSAGES/sphinx.mo` & `ablog-0.9.5/ablog/locale/de/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/de/LC_MESSAGES/sphinx.po` & `ablog-0.9.5/ablog/locale/de/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/es/LC_MESSAGES/sphinx.mo` & `ablog-0.9.5/ablog/locale/es/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/es/LC_MESSAGES/sphinx.po` & `ablog-0.9.5/ablog/locale/es/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/et/LC_MESSAGES/sphinx.mo` & `ablog-0.9.5/ablog/locale/et/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/et/LC_MESSAGES/sphinx.po` & `ablog-0.9.5/ablog/locale/et/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/ru/LC_MESSAGES/sphinx.mo` & `ablog-0.9.5/ablog/locale/ru/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/ru/LC_MESSAGES/sphinx.po` & `ablog-0.9.5/ablog/locale/ru/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/sphinx.pot` & `ablog-0.9.5/ablog/locale/sphinx.pot`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/tr/LC_MESSAGES/sphinx.mo` & `ablog-0.9.5/ablog/locale/tr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/locale/tr/LC_MESSAGES/sphinx.po` & `ablog-0.9.5/ablog/locale/tr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/post.py` & `ablog-0.9.5/ablog/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,21 +96,16 @@
 
 
 class UpdateDirective(BaseAdmonition):
     required_arguments = 1
     node_class = UpdateNode
 
     def run(self):
-        date_arg = self.arguments[0] if self.arguments else ''
-        self.arguments = [_('Updated on ' + date_arg), ]
-        # The following line is needed to trick the BaseAdmonition class into thinking we have a title.
-        # There almost certainly has to be a better way, but I don't see it naturally from the docutils source
-        self.node_class = nodes.admonition
-        ad = super(UpdateDirective, self).run()  # For Python3, it is run(), not run(self)
-        del self.node_class  # Undo our tricksy hack from a few lines ago
+        ad = super(UpdateDirective, self).run()
+        ad[0]['date'] = self.arguments[0] if self.arguments else ''
         return ad
 
 
 class PostListDirective(Directive):
     """Handle ``postlist`` directives."""
 
     def _split(a): return set(s.strip() for s in a.split(','))
@@ -189,19 +184,20 @@
                     update = date_parser(update_node['date'])
                 except ValueError:
                     raise ValueError('invalid post date in: ' + docname)
             else:
                 raise ValueError('invalid post date (%s) in ' % (date) +
                                  docname +
                                  ". Expected format: %s" % post_date_format)
+        # Insert a new title element which contains the `Updated on {date}` logic.
         substitute = nodes.title(u'',
-                                 update_node[0][0].astext() + u' ' +
-                                 update.strftime(post_date_format))
-        update_node[0].replace_self(substitute)
-        # for now, let updates look like note
+                                 'Updated on '
+                                 + update.strftime(post_date_format)
+                                )
+        update_node.insert(0, substitute)
         update_node['classes'] = ['note', 'update']
 
         update_dates.append(update)
     return update_dates
 
 
 def process_posts(app, doctree):
@@ -212,19 +208,23 @@
     if not hasattr(env, 'ablog_posts'):
         env.ablog_posts = {}
 
     post_nodes = list(doctree.traverse(PostNode))
     if not post_nodes:
         return
     post_date_format = app.config['post_date_format']
+    should_auto_orphan = app.config['post_auto_orphan']
     docname = env.docname
 
-    # mark the post as 'orphan' so that
-    #   "document isn't included in any toctree" warning is not issued
-    app.env.metadata[docname]['orphan'] = True
+    if should_auto_orphan:
+        # mark the post as 'orphan' so that
+        #   "document isn't included in any toctree" warning is not issued
+        # We do not simply assign to should_auto_orphan because if auto-orphan
+        # is false, we still want to respect the per-post :rst:dir`orphan` setting
+        app.env.metadata[docname]['orphan'] = True
 
     blog = Blog(app)
     auto_excerpt = blog.post_auto_excerpt
     multi_post = len(post_nodes) > 1 or blog.post_always_section
 
     for order, node in enumerate(post_nodes, start=1):
         if node['excerpt'] is None:
```

### Comparing `ablog-0.9.4/ablog/start.py` & `ablog-0.9.5/ablog/start.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,20 @@
 
 # When ``True``, post title and excerpt is always taken from the section that
 # contains the :rst:dir:`post` directive, instead of the document. This is the
 # behavior when :rst:dir:`post` is used multiple times in a document. Default
 # is ``False``.
 #post_always_section = False
 
+# When ``False``, the :rst:dir:`orphan` directive is not automatically set
+# for each post. Without this directive, Sphinx will warn about posts that
+# are not explicitly referenced via another document. :rst:dir:`orphan` can
+# be set on a per-post basis as well if this is false. Default is ``True``.
+#post_auto_orphan = True
+
 # -- ABlog Sidebars -------------------------------------------------------
 
 # There are seven sidebars you can include in your HTML output.
 # postcard.html provides information regarding the current post.
 # recentposts.html lists most recent five posts. Others provide
 # a link to a archive pages generated for each tag, category, and year.
 # In addition, there are authors.html, languages.html, and locations.html
@@ -325,17 +331,14 @@
 # using the given strftime format.
 #html_last_updated_fmt = '%%b %%d, %%Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
 #html_use_smartypants = True
 
-# Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
-
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
 #html_additional_pages = {}
 
 # If false, no module index is generated.
 #html_domain_indices = True
 
@@ -619,17 +622,18 @@
 
     if 'blog_baseurl' not in d:
         print('')
         print(w('Please enter the base URL for your project. Blog feeds will '
                 'be generated relative to this URL. If you don\'t have one yet, '
                 'you can set it in configuration file later.'))
         if SPHINX_LT_17:
+            # APR: Not sure how do_prompt() worked prior to Sphinx 1.7; likely to be `lambda x: x` here too
             do_prompt(d, 'blog_baseurl', 'Base URL for your project', None, lambda x: True)
         else:
-            d['blog_baseurl'] = do_prompt('Base URL for your project', None, lambda x: True)
+            d['blog_baseurl'] = do_prompt('Base URL for your project', None, lambda x: x)
 
     print('')
 
 
 def ablog_start(**kwargs):
     if not color_terminal():
         nocolor()
```

### Comparing `ablog-0.9.4/ablog/templates/catalog.html` & `ablog-0.9.5/ablog/templates/catalog.html`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/templates/collection.html` & `ablog-0.9.5/ablog/templates/collection.html`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/templates/page.html` & `ablog-0.9.5/ablog/templates/page.html`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/templates/postcard2.html` & `ablog-0.9.5/ablog/templates/postcard2.html`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/templates/postnavy.html` & `ablog-0.9.5/ablog/templates/postnavy.html`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog/templates/tagcloud.html` & `ablog-0.9.5/ablog/templates/tagcloud.html`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/ablog.egg-info/PKG-INFO` & `ablog-0.9.5/ablog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ablog
-Version: 0.9.4
+Version: 0.9.5
 Summary: ABlog allows you to blog with Sphinx
 Home-page: http://ablog.readthedocs.org/
 Author: SunPy Developers
 Author-email: nabil.freij@gmail.com
 License: MIT License
 Description: 
         ABlog for Sphinx
```

### Comparing `ablog-0.9.4/ablog.egg-info/SOURCES.txt` & `ablog-0.9.5/ablog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ablog-0.9.4/setup.py` & `ablog-0.9.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from setuptools import setup
 
 __version__ = ''
 with open('ablog/__init__.py') as inp:
     for line in inp:
         if (line.startswith('__version__')):
             exec(line.strip())
```

