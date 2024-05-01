# Comparing `tmp/chrono24-0.2.7.tar.gz` & `tmp/chrono24-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrono24-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "chrono24-0.2.8.tar", last modified: Wed May  1 22:37:40 2024, max compression
```

## Comparing `chrono24-0.2.7.tar` & `chrono24-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       83 2023-12-31 20:29:04.122838 chrono24-0.2.7/.flake8
--rw-r--r--   0        0        0      170 2022-12-31 19:48:44.859641 chrono24-0.2.7/.github/dependabot.yaml
--rw-r--r--   0        0        0      997 2024-02-18 04:27:00.536961 chrono24-0.2.7/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     1799 2023-01-02 19:05:24.745258 chrono24-0.2.7/.gitignore
--rw-r--r--   0        0        0     1068 2023-01-02 19:05:24.745422 chrono24-0.2.7/LICENSE
--rw-r--r--   0        0        0      847 2023-12-31 22:56:54.196916 chrono24-0.2.7/Makefile
--rw-r--r--   0        0        0     5589 2024-01-23 21:11:24.534767 chrono24-0.2.7/README.md
--rw-r--r--   0        0        0      156 2024-02-18 04:40:54.915484 chrono24-0.2.7/chrono24/__init__.py
--rw-r--r--   0        0        0    18367 2024-02-18 04:39:14.993682 chrono24-0.2.7/chrono24/api.py
--rw-r--r--   0        0        0      239 2023-12-31 22:45:10.167411 chrono24-0.2.7/chrono24/exceptions.py
--rw-r--r--   0        0        0     4509 2024-01-01 01:40:19.692191 chrono24-0.2.7/chrono24/session.py
--rw-r--r--   0        0        0        0 2023-12-31 22:43:03.061191 chrono24-0.2.7/conftest.py
--rw-r--r--   0        0        0      887 2023-12-31 18:18:22.048837 chrono24-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       32 2023-12-31 22:50:57.346272 chrono24-0.2.7/requirements-dev.txt
--rw-r--r--   0        0        0       33 2023-12-31 18:16:11.713712 chrono24-0.2.7/requirements.txt
--rw-r--r--   0        0        0     1255 2023-12-31 18:19:07.082258 chrono24-0.2.7/setup.cfg
--rw-r--r--   0        0        0     2974 2024-01-02 03:17:17.072335 chrono24-0.2.7/tests/test_api.py
--rw-r--r--   0        0        0      647 2024-01-01 18:55:58.188389 chrono24-0.2.7/tests/test_exceptions.py
--rw-r--r--   0        0        0     6457 1970-01-01 00:00:00.000000 chrono24-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       83 2023-12-31 20:29:04.122838 chrono24-0.2.8/.flake8
+-rw-r--r--   0        0        0      170 2022-12-31 19:48:44.859641 chrono24-0.2.8/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1087 2024-05-01 22:16:45.525774 chrono24-0.2.8/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     1799 2023-01-02 19:05:24.745258 chrono24-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1068 2023-01-02 19:05:24.745422 chrono24-0.2.8/LICENSE
+-rw-r--r--   0        0        0      847 2023-12-31 22:56:54.196916 chrono24-0.2.8/Makefile
+-rw-r--r--   0        0        0     5717 2024-05-01 22:16:45.526242 chrono24-0.2.8/README.md
+-rw-r--r--   0        0        0      156 2024-05-01 22:37:10.249426 chrono24-0.2.8/chrono24/__init__.py
+-rw-r--r--   0        0        0    18621 2024-05-01 22:35:42.518925 chrono24-0.2.8/chrono24/api.py
+-rw-r--r--   0        0        0      239 2023-12-31 22:45:10.167411 chrono24-0.2.8/chrono24/exceptions.py
+-rw-r--r--   0        0        0     4509 2024-01-01 01:40:19.692191 chrono24-0.2.8/chrono24/session.py
+-rw-r--r--   0        0        0        0 2023-12-31 22:43:03.061191 chrono24-0.2.8/conftest.py
+-rw-r--r--   0        0        0      887 2023-12-31 18:18:22.048837 chrono24-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-12-31 22:50:57.346272 chrono24-0.2.8/requirements-dev.txt
+-rw-r--r--   0        0        0       33 2023-12-31 18:16:11.713712 chrono24-0.2.8/requirements.txt
+-rw-r--r--   0        0        0     1255 2023-12-31 18:19:07.082258 chrono24-0.2.8/setup.cfg
+-rw-r--r--   0        0        0     2974 2024-01-02 03:17:17.072335 chrono24-0.2.8/tests/test_api.py
+-rw-r--r--   0        0        0      647 2024-01-01 18:55:58.188389 chrono24-0.2.8/tests/test_exceptions.py
+-rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 chrono24-0.2.8/PKG-INFO
```

### Comparing `chrono24-0.2.7/.github/workflows/ci.yaml` & `chrono24-0.2.8/.github/workflows/ci.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 name: continuous-integration
 
 on:
   push:
   workflow_dispatch:
+  schedule:
+    # Schedule for the workflow to run at 00:00 every Sunday
+    - cron: '0 0 * * 0'
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
     - uses: actions/checkout@v2
     
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `chrono24-0.2.7/.gitignore` & `chrono24-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.7/LICENSE` & `chrono24-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.7/Makefile` & `chrono24-0.2.8/Makefile`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.7/README.md` & `chrono24-0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # chrono24
 
+<p align="center">
+  <img src="https://static.chrono24.com/images/default/logo-positive-reduced.svg" width="50%" />
+</p>
+
+<br>
+
 [Chrono24](https://www.chrono24.com/) API wrapper
 
 [![pypiv](https://img.shields.io/pypi/v/chrono24.svg)](https://pypi.python.org/pypi/chrono24)
-[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![continuous-integration](https://github.com/irahorecka/chrono24/workflows/continuous-integration/badge.svg)](https://github.com/irahorecka/chrono24/actions)
 [![Licence](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/irahorecka/chrono24/main/LICENSE)
 
 ## Installation
 
 ```bash
 pip install chrono24
```

### Comparing `chrono24-0.2.7/chrono24/api.py` & `chrono24-0.2.8/chrono24/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 chrono24/api
 ~~~~~~~~~~~~
 """
 
+import json
 import re
 from functools import lru_cache
 
 from bs4 import BeautifulSoup
 
 from chrono24.exceptions import NoListingsFoundException
 from chrono24.session import get_html, get_response
@@ -215,23 +216,29 @@
 
         Returns:
             int: The total count of listings as an integer.
 
         Raises:
             NoListingsFoundException: Raised if the query is invalid or no listing count is found.
         """
-        try:
-            listing_count_text = get_text_html_tag(
-                html.find("div", {"class": "result-page-top"}).find("strong")
-            )
-            match = re.search(RE_PATTERN_COMMA_SEPARATED_NUM, listing_count_text)
-            # Return total listing count as integer, otherwise 0
-            return int(match.group().replace(",", ""))
-        except AttributeError as e:
-            raise NoListingsFoundException("No listings found.") from e
+        # Find the script tag that contains `window.metaData`
+        script = html.find("script", text=re.compile("window.metaData"))
+        # Use regex to extract the JSON string
+        pattern = re.compile(r"window.metaData = ({.*?});", re.DOTALL)
+        script_text = script.text
+        match = pattern.search(script_text)
+        if match:
+            metadata_json_str = match[1]
+            metadata = json.loads(metadata_json_str)
+            # Only return total count if listings are found
+            total_count = int(metadata["data"]["searchResult"]["numResult"])
+            if total_count > 0:
+                return total_count
+
+        raise NoListingsFoundException("No listings found.")
 
 
 class StandardListing:
     """Represents a standard listing extracted from HTML content."""
 
     def __init__(self, html):
         """Initialize a StandardListing object with HTML content.
```

### Comparing `chrono24-0.2.7/chrono24/session.py` & `chrono24-0.2.8/chrono24/session.py`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.7/pyproject.toml` & `chrono24-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.7/setup.cfg` & `chrono24-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.7/tests/test_api.py` & `chrono24-0.2.8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.7/tests/test_exceptions.py` & `chrono24-0.2.8/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.7/PKG-INFO` & `chrono24-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrono24
-Version: 0.2.7
+Version: 0.2.8
 Summary: chrono24
 Home-page: https://github.com/irahorecka/chrono24
 Author: Ira Horecka
 Author-email: ira89@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
@@ -20,18 +20,24 @@
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4>=4.11.0
 Requires-Dist: requests>=2.28.0
 Requires-Dist: tenacity>=8.2.0
 
 # chrono24
 
+<p align="center">
+  <img src="https://static.chrono24.com/images/default/logo-positive-reduced.svg" width="50%" />
+</p>
+
+<br>
+
 [Chrono24](https://www.chrono24.com/) API wrapper
 
 [![pypiv](https://img.shields.io/pypi/v/chrono24.svg)](https://pypi.python.org/pypi/chrono24)
-[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![continuous-integration](https://github.com/irahorecka/chrono24/workflows/continuous-integration/badge.svg)](https://github.com/irahorecka/chrono24/actions)
 [![Licence](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/irahorecka/chrono24/main/LICENSE)
 
 ## Installation
 
 ```bash
 pip install chrono24
```

