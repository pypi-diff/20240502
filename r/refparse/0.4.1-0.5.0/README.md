# Comparing `tmp/refparse-0.4.1.tar.gz` & `tmp/refparse-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refparse-0.4.1.tar", last modified: Mon Apr 29 14:50:01 2024, max compression
+gzip compressed data, was "refparse-0.5.0.tar", last modified: Thu May  2 16:19:06 2024, max compression
```

## Comparing `refparse-0.4.1.tar` & `refparse-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:50:01.497932 refparse-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 14:49:57.000000 refparse-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-29 14:50:01.497932 refparse-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-29 14:49:57.000000 refparse-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-29 14:49:57.000000 refparse-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:50:01.497932 refparse-0.4.1/refparse/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-29 14:49:57.000000 refparse-0.4.1/refparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-29 14:49:57.000000 refparse-0.4.1/refparse/cssci.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-29 14:49:57.000000 refparse-0.4.1/refparse/scopus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-29 14:49:57.000000 refparse-0.4.1/refparse/wos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:50:01.497932 refparse-0.4.1/refparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-29 14:50:01.000000 refparse-0.4.1/refparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 14:50:01.000000 refparse-0.4.1/refparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:50:01.000000 refparse-0.4.1/refparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 14:50:01.000000 refparse-0.4.1/refparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:50:01.497932 refparse-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:50:01.497932 refparse-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-04-29 14:49:57.000000 refparse-0.4.1/tests/test_cssci.py
--rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-04-29 14:49:57.000000 refparse-0.4.1/tests/test_scopus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-29 14:49:57.000000 refparse-0.4.1/tests/test_wos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:19:06.601207 refparse-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 16:19:02.000000 refparse-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-02 16:19:06.601207 refparse-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-02 16:19:02.000000 refparse-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-02 16:19:02.000000 refparse-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:19:06.597207 refparse-0.5.0/refparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-02 16:19:02.000000 refparse-0.5.0/refparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-02 16:19:02.000000 refparse-0.5.0/refparse/cssci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-05-02 16:19:02.000000 refparse-0.5.0/refparse/scopus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-02 16:19:02.000000 refparse-0.5.0/refparse/wos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:19:06.601207 refparse-0.5.0/refparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-02 16:19:06.000000 refparse-0.5.0/refparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-02 16:19:06.000000 refparse-0.5.0/refparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:19:06.000000 refparse-0.5.0/refparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 16:19:06.000000 refparse-0.5.0/refparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:19:06.601207 refparse-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:19:06.601207 refparse-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-05-02 16:19:02.000000 refparse-0.5.0/tests/test_cssci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-05-02 16:19:02.000000 refparse-0.5.0/tests/test_scopus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-05-02 16:19:02.000000 refparse-0.5.0/tests/test_wos.py
```

### Comparing `refparse-0.4.1/LICENSE` & `refparse-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `refparse-0.4.1/PKG-INFO` & `refparse-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refparse
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Python library to parse bibliographic references
 Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/doublessay/refparse
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -46,20 +46,17 @@
  'issue': None,
  'page': '436-444',
  'year': '2015'}
 ```
 
 ## Return Fields
 
-|        | Web of Science | Scopus  | CSSCI*  |
+|        | Web of Science | Scopus  | CSSCI   |
 | :---:  | :---:          | :---:   | :---:   |
-| author | &check;        | &check; |         |
-| title  |                | &check; |         |
-| source | &check;        | &check; |         |
-| volume | &check;        | &check; |         |
-| issue  |                | &check; |         |
-| page   | &check;        | &check; |         |
-| year   | &check;        | &check; |         |
+| author | &check;        | &check; | &check; |
+| title  |                | &check; | &check; |
+| source | &check;        | &check; | &check; |
+| volume | &check;        | &check; | &check; |
+| issue  |                | &check; | &check; |
+| page   | &check;        | &check; | &check; |
+| year   | &check;        | &check; | &check; |
 | doi    | &check;        |         |         |
-| identifier except doi | |         | &check; |
-
-\* CSSCI will return differently depending on reference type.
```

### Comparing `refparse-0.4.1/README.md` & `refparse-0.5.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -23,20 +23,17 @@
  'issue': None,
  'page': '436-444',
  'year': '2015'}
 ```
 
 ## Return Fields
 
-|        | Web of Science | Scopus  | CSSCI*  |
+|        | Web of Science | Scopus  | CSSCI   |
 | :---:  | :---:          | :---:   | :---:   |
-| author | &check;        | &check; |         |
-| title  |                | &check; |         |
-| source | &check;        | &check; |         |
-| volume | &check;        | &check; |         |
-| issue  |                | &check; |         |
-| page   | &check;        | &check; |         |
-| year   | &check;        | &check; |         |
+| author | &check;        | &check; | &check; |
+| title  |                | &check; | &check; |
+| source | &check;        | &check; | &check; |
+| volume | &check;        | &check; | &check; |
+| issue  |                | &check; | &check; |
+| page   | &check;        | &check; | &check; |
+| year   | &check;        | &check; | &check; |
 | doi    | &check;        |         |         |
-| identifier except doi | |         | &check; |
-
-\* CSSCI will return differently depending on reference type.
```

### Comparing `refparse-0.4.1/pyproject.toml` & `refparse-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `refparse-0.4.1/refparse/__init__.py` & `refparse-0.5.0/refparse/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.1"
+__version__ = "0.5.0"
 
 from typing import Literal, Optional
 from .wos import ParseWos
 from .scopus import ParseScopus
 from .cssci import ParseCssci
```

### Comparing `refparse-0.4.1/refparse/scopus.py` & `refparse-0.5.0/refparse/scopus.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         # Remove volume symbol
         ref = re.sub(r"\bvol\.? ([^,]+)", r"\1", ref, flags=re.I)
 
         # Add page symbol
         if re.search(r", \d+-\d+, \(", ref):
             if not re.search(r", \d{4}-\d{4}, ", ref):
-                match = re.search(r", (\d+-\d+), ", ref).group(1)
+                match = re.search(r", (\d+-\d+), ", ref).group(1) # type: ignore
                 if re.search(r"\d, \d+-", ref):
                     a, b = (int(i) for i in match.split("-"))
                     # Exclude possible issue
                     if b - a != 1:
                         ref = ref.replace(match, f"pp. {match}", 1)
                 else:
                     ref = ref.replace(match, f"pp. {match}", 1)
@@ -197,15 +197,15 @@
                 else:
                     title = None
 
         # Extract title info
         if title == "unknown":
             # Remove other fields info
             if source:
-                repr_str = re.match(r"([A-Za-z\d\. ]{,20})", source)[1]
+                repr_str = re.match(r"([A-Za-z\d\. ]{,20})", source).group(1) # type: ignore
                 ref_left = re.sub(f", {repr_str}.*$", "", self.ref)
             elif volume:
                 ref_left = re.sub(f", {volume}.*$", "", self.ref)
             elif page:
                 ref_left = re.sub(f", pp.*$", "", self.ref)
             else:
                 ref_left = self.ref[:-8]
```

### Comparing `refparse-0.4.1/refparse/wos.py` & `refparse-0.5.0/refparse/wos.py`

 * *Files identical despite different names*

### Comparing `refparse-0.4.1/refparse.egg-info/PKG-INFO` & `refparse-0.5.0/refparse.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refparse
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Python library to parse bibliographic references
 Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/doublessay/refparse
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -46,20 +46,17 @@
  'issue': None,
  'page': '436-444',
  'year': '2015'}
 ```
 
 ## Return Fields
 
-|        | Web of Science | Scopus  | CSSCI*  |
+|        | Web of Science | Scopus  | CSSCI   |
 | :---:  | :---:          | :---:   | :---:   |
-| author | &check;        | &check; |         |
-| title  |                | &check; |         |
-| source | &check;        | &check; |         |
-| volume | &check;        | &check; |         |
-| issue  |                | &check; |         |
-| page   | &check;        | &check; |         |
-| year   | &check;        | &check; |         |
+| author | &check;        | &check; | &check; |
+| title  |                | &check; | &check; |
+| source | &check;        | &check; | &check; |
+| volume | &check;        | &check; | &check; |
+| issue  |                | &check; | &check; |
+| page   | &check;        | &check; | &check; |
+| year   | &check;        | &check; | &check; |
 | doi    | &check;        |         |         |
-| identifier except doi | |         | &check; |
-
-\* CSSCI will return differently depending on reference type.
```

### Comparing `refparse-0.4.1/tests/test_scopus.py` & `refparse-0.5.0/tests/test_scopus.py`

 * *Files identical despite different names*

### Comparing `refparse-0.4.1/tests/test_wos.py` & `refparse-0.5.0/tests/test_wos.py`

 * *Files identical despite different names*

