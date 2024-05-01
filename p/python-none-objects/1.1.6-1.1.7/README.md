# Comparing `tmp/python_none_objects-1.1.6.tar.gz` & `tmp/python_none_objects-1.1.7.tar.gz`

## Comparing `python_none_objects-1.1.6.tar` & `python_none_objects-1.1.7.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/README_printable.md
--rwxr-xr-x   0        0        0     1664 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/build_and_checks.sh
--rwxr-xr-x   0        0        0      993 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/build_readme.sh
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/src/python_none_objects/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/src/python_none_objects/py.typed
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/typing_test/__init__.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/COPYING.LESSER
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/README.md
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/pyproject.toml
--rw-r--r--   0        0        0    14616 2020-02-02 00:00:00.000000 python_none_objects-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/README_printable.md
+-rwxr-xr-x   0        0        0     2345 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/build_and_checks.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/wget_sha512.sh
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/src/python_none_objects/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/src/python_none_objects/py.typed
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/typing_test/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/COPYING.LESSER
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/README.md
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0    14879 2020-02-02 00:00:00.000000 python_none_objects-1.1.7/PKG-INFO
```

### Comparing `python_none_objects-1.1.6/README_printable.md` & `python_none_objects-1.1.7/README_printable.md`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.6/src/python_none_objects/__init__.py` & `python_none_objects-1.1.7/src/python_none_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.6/typing_test/__init__.py` & `python_none_objects-1.1.7/typing_test/__init__.py`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.6/COPYING` & `python_none_objects-1.1.7/COPYING`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.6/COPYING.LESSER` & `python_none_objects-1.1.7/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.6/README.md` & `python_none_objects-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `python_none_objects-1.1.6/pyproject.toml` & `python_none_objects-1.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,32 +2,39 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-none-objects"
-version = "1.1.6"
+version = "1.1.7"
 description = """\
 Add more constant \"None\" objects to Python \
 to avoid boilerplate code\
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
 keywords = ["Python", "None", "Immutable", "Default values"]
 dependencies = [
 ]
 requires-python = ">=3.11"
 
 [project.optional-dependencies]
```

### Comparing `python_none_objects-1.1.6/PKG-INFO` & `python_none_objects-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.3
 Name: python-none-objects
-Version: 1.1.6
+Version: 1.1.7
 Summary: Add more constant "None" objects to Python to avoid boilerplate code
 Project-URL: Homepage, https://github.com/LLyaudet/python-none-objects
 Project-URL: Bug Tracker, https://github.com/LLyaudet/python-none-objects/issues
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
 Keywords: Default values,Immutable,None,Python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Description-Content-Type: text/markdown
```

