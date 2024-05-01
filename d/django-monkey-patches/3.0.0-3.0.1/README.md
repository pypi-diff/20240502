# Comparing `tmp/django_monkey_patches-3.0.0.tar.gz` & `tmp/django_monkey_patches-3.0.1.tar.gz`

## Comparing `django_monkey_patches-3.0.0.tar` & `django_monkey_patches-3.0.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/README_printable.md
--rwxr-xr-x   0        0        0     1646 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/build_and_checks.sh
--rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/build_readme.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/__init__.py
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__base_cache__make_cache_key.py
--rw-r--r--   0        0        0    15568 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__orm__prefetch.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set__get.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set__get_or_create.py
--rw-r--r--   0        0        0    37274 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_wrapper.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__test_case__tear_down.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django_rest_framework__field__get_request.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/PKG-INFO
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/requires.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/top_level.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/COPYING.LESSER
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    13519 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/README_printable.md
+-rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/build_and_checks.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/wget_sha512.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/__init__.py
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/django__base_cache__make_cache_key.py
+-rw-r--r--   0        0        0    15568 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/django__orm__prefetch.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/django__query_set.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/django__query_set__get.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/django__query_set__get_or_create.py
+-rw-r--r--   0        0        0    37274 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/django__query_wrapper.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/django__test_case__tear_down.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/django_rest_framework__field__get_request.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches.egg-info/requires.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/src/django_monkey_patches.egg-info/top_level.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/COPYING.LESSER
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/README.md
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.1/PKG-INFO
```

### Comparing `django_monkey_patches-3.0.0/README_printable.md` & `django_monkey_patches-3.0.1/README_printable.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/django__base_cache__make_cache_key.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/django__base_cache__make_cache_key.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/django__orm__prefetch.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/django__orm__prefetch.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/django__query_set.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set__get.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/django__query_set__get.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set__get_or_create.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/django__query_set__get_or_create.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_wrapper.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/django__query_wrapper.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/django__test_case__tear_down.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/django__test_case__tear_down.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/django_rest_framework__field__get_request.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/django_rest_framework__field__get_request.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py` & `django_monkey_patches-3.0.1/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/PKG-INFO` & `django_monkey_patches-3.0.1/src/django_monkey_patches.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/SOURCES.txt` & `django_monkey_patches-3.0.1/src/django_monkey_patches.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/COPYING` & `django_monkey_patches-3.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/COPYING.LESSER` & `django_monkey_patches-3.0.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/README.md` & `django_monkey_patches-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.0/pyproject.toml` & `django_monkey_patches-3.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,31 +2,41 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-monkey-patches"
-version = "3.0.0"
+version = "3.0.1"
 description = """\
 Add monkey-patches to correct and enhance your favorite framework\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
+maintainers = [
+    { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
+]
 license = { file = "COPYING.LESSER" }
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Framework :: Django",
+    "Intended Audience :: Developers",
     """\
 License :: OSI Approved :: \
 GNU Lesser General Public License v3 or later (LGPLv3+)\
 """,
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    """\
+Topic :: Software Development :: Libraries :: Application Frameworks\
+""",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["Django", "monkey-patch"]
 dependencies = [
 ]
 requires-python = ">=3.0"
 
 [project.optional-dependencies]
```

### Comparing `django_monkey_patches-3.0.0/PKG-INFO` & `django_monkey_patches-3.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.3
 Name: django-monkey-patches
-Version: 3.0.0
+Version: 3.0.1
 Summary: Add monkey-patches to correct and enhance your favorite framework
 Project-URL: Homepage, https://github.com/LLyaudet/django-monkey-patches
 Project-URL: Bug Tracker, https://github.com/LLyaudet/django-monkey-patches/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
+Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -169,18 +170,23 @@
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 License-File: COPYING
 License-File: COPYING.LESSER
 Keywords: Django,monkey-patch
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.0
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Description-Content-Type: text/markdown
```

