# Comparing `tmp/python_repeatable_iterable-2.1.3.tar.gz` & `tmp/python_repeatable_iterable-2.1.4.tar.gz`

## Comparing `python_repeatable_iterable-2.1.3.tar` & `python_repeatable_iterable-2.1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/CONTRIBUTORS.md
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/README_printable.md
--rwxr-xr-x   0        0        0     1699 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/build_and_checks.sh
--rwxr-xr-x   0        0        0     1021 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/build_readme.sh
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/src/python_repeatable_iterable/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/src/python_repeatable_iterable/py.typed
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/typing_test/__init__.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/COPYING.LESSER
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/README.md
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/pyproject.toml
--rw-r--r--   0        0        0    14323 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/README_printable.md
+-rwxr-xr-x   0        0        0     2380 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/build_and_checks.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/wget_sha512.sh
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/src/python_repeatable_iterable/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/src/python_repeatable_iterable/py.typed
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/typing_test/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/COPYING.LESSER
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/README.md
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 python_repeatable_iterable-2.1.4/PKG-INFO
```

### Comparing `python_repeatable_iterable-2.1.3/README_printable.md` & `python_repeatable_iterable-2.1.4/README_printable.md`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.3/src/python_repeatable_iterable/__init__.py` & `python_repeatable_iterable-2.1.4/src/python_repeatable_iterable/__init__.py`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.3/typing_test/__init__.py` & `python_repeatable_iterable-2.1.4/typing_test/__init__.py`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.3/COPYING` & `python_repeatable_iterable-2.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.3/COPYING.LESSER` & `python_repeatable_iterable-2.1.4/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.3/README.md` & `python_repeatable_iterable-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `python_repeatable_iterable-2.1.3/pyproject.toml` & `python_repeatable_iterable-2.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-repeatable-iterable"
-version = "2.1.3"
+version = "2.1.4"
 description = """\
 Add a RepeatableIterable type and a function to obtain it\
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
+    "Intended Audience :: Developers",
     """\
 License :: OSI Approved :: \
 GNU Lesser General Public License v3 or later (LGPLv3+)\
 """,
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Typing :: Typed",
 ]
 keywords = ["Python", "Iterable", "Repeatable", "RepeatableIterable"]
 dependencies = [
    "python-none-objects==1.1.5",
 ]
 requires-python = ">=3.11"
```

### Comparing `python_repeatable_iterable-2.1.3/PKG-INFO` & `python_repeatable_iterable-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.3
 Name: python-repeatable-iterable
-Version: 2.1.3
+Version: 2.1.4
 Summary: Add a RepeatableIterable type and a function to obtain it
 Project-URL: Homepage, https://github.com/LLyaudet/python-repeatable-iterable
 Project-URL: Bug Tracker, https://github.com/LLyaudet/python-repeatable-iterable/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
+Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -169,18 +170,22 @@
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 License-File: COPYING
 License-File: COPYING.LESSER
 Keywords: Iterable,Python,Repeatable,RepeatableIterable
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Requires-Dist: python-none-objects==1.1.5
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
```

