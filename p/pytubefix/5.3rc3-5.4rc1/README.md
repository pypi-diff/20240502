# Comparing `tmp/pytubefix-5.3rc3.tar.gz` & `tmp/pytubefix-5.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubefix-5.3rc3.tar", last modified: Tue Apr 30 00:45:26 2024, max compression
+gzip compressed data, was "pytubefix-5.4rc1.tar", last modified: Wed May  1 19:35:22 2024, max compression
```

## Comparing `pytubefix-5.3rc3.tar` & `pytubefix-5.4rc1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:45:26.140663 pytubefix-5.3rc3/
--rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/LICENSE
--rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/MANIFEST.in
--rw-r--r--   0 juan      (1000) juan      (1000)     4342 2024-04-30 00:45:26.136663 pytubefix-5.3rc3/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     3010 2024-04-30 00:39:00.000000 pytubefix-5.3rc3/README.md
--rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-04-30 00:41:41.000000 pytubefix-5.3rc3/pyproject.toml
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:45:26.124663 pytubefix-5.3rc3/pytubefix/
--rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    20118 2024-04-30 00:31:55.000000 pytubefix-5.3rc3/pytubefix/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6595 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/chapters.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    17032 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      786 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/colors.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:45:26.132663 pytubefix-5.3rc3/pytubefix/contrib/
--rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/contrib/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/contrib/channel.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/contrib/playlist.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/contrib/search.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4115 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18319 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     9944 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    17902 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/innertube.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4311 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/jsinterp.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/monostate.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5960 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14289 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     8817 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14818 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/streams.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-04-30 00:42:00.000000 pytubefix-5.3rc3/pytubefix/version.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:45:26.136663 pytubefix-5.3rc3/pytubefix.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     4342 2024-04-30 00:45:26.000000 pytubefix-5.3rc3/pytubefix.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     1029 2024-04-30 00:45:26.000000 pytubefix-5.3rc3/pytubefix.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-30 00:45:26.000000 pytubefix-5.3rc3/pytubefix.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-04-30 00:45:26.000000 pytubefix-5.3rc3/pytubefix.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-04-30 00:45:26.000000 pytubefix-5.3rc3/pytubefix.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-30 00:45:26.140663 pytubefix-5.3rc3/setup.cfg
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:45:26.136663 pytubefix-5.3rc3/tests/
--rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_main.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_streams.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-01 19:35:22.278043 pytubefix-5.4rc1/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/LICENSE
+-rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/MANIFEST.in
+-rw-r--r--   0 juan      (1000) juan      (1000)     4342 2024-05-01 19:35:22.274043 pytubefix-5.4rc1/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3010 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-05-01 19:22:11.000000 pytubefix-5.4rc1/pyproject.toml
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-01 19:35:22.270043 pytubefix-5.4rc1/pytubefix/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/pytubefix/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    20063 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6593 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/pytubefix/chapters.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/pytubefix/cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    16972 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      781 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/colors.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-01 19:35:22.270043 pytubefix-5.4rc1/pytubefix/contrib/
+-rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/pytubefix/contrib/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/pytubefix/contrib/channel.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/pytubefix/contrib/playlist.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/pytubefix/contrib/search.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4099 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18315 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     9943 2024-05-01 19:28:41.000000 pytubefix-5.4rc1/pytubefix/helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17742 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/innertube.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4276 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/pytubefix/jsinterp.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/pytubefix/metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/pytubefix/monostate.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5948 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14359 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     8736 2024-05-01 19:15:47.000000 pytubefix-5.4rc1/pytubefix/request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    16049 2024-05-01 19:25:51.000000 pytubefix-5.4rc1/pytubefix/streams.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-05-01 19:29:15.000000 pytubefix-5.4rc1/pytubefix/version.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-01 19:35:22.274043 pytubefix-5.4rc1/pytubefix.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     4342 2024-05-01 19:35:22.000000 pytubefix-5.4rc1/pytubefix.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1029 2024-05-01 19:35:22.000000 pytubefix-5.4rc1/pytubefix.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-01 19:35:22.000000 pytubefix-5.4rc1/pytubefix.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-05-01 19:35:22.000000 pytubefix-5.4rc1/pytubefix.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-05-01 19:35:22.000000 pytubefix-5.4rc1/pytubefix.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-01 19:35:22.278043 pytubefix-5.4rc1/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-01 19:35:22.274043 pytubefix-5.4rc1/tests/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_main.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-05-01 19:14:26.000000 pytubefix-5.4rc1/tests/test_streams.py
```

### Comparing `pytubefix-5.3rc3/LICENSE` & `pytubefix-5.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/PKG-INFO` & `pytubefix-5.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.3rc3
+Version: 5.4rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.3rc3 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.4rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.3rc3/README.md` & `pytubefix-5.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/pyproject.toml` & `pytubefix-5.4rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubefix"
-version = "5.3-rc3"
+version = "5.4-rc1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python3 library for downloading YouTube Videos."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT license"}
```

### Comparing `pytubefix-5.3rc3/pytubefix/__init__.py` & `pytubefix-5.4rc1/pytubefix/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/pytubefix/__main__.py` & `pytubefix-5.4rc1/pytubefix/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,22 +80,29 @@
         :param bool use_oauth:
             (Optional) Prompt the user to authenticate to YouTube.
             If allow_oauth_cache is set to True, the user should only be prompted once.
         :param bool allow_oauth_cache:
             (Optional) Cache OAuth tokens locally on the machine. Defaults to True.
             These tokens are only generated if use_oauth is set to True as well.
         """
-        self._js: Optional[str] = None  # js fetched by js_url
-        self._js_url: Optional[str] = None  # the url to the js, parsed from watch html
+        # js fetched by js_url
+        self._js: Optional[str] = None
 
-        self._vid_info: Optional[Dict] = None  # content fetched from innertube/player
+        # the url to the js, parsed from watch html
+        self._js_url: Optional[str] = None
 
-        self._watch_html: Optional[str] = None  # the html of /watch?v=<video_id>
+        # content fetched from innertube/player
+        self._vid_info: Optional[Dict] = None
+
+        # the html of /watch?v=<video_id>
+        self._watch_html: Optional[str] = None
         self._embed_html: Optional[str] = None
-        self._player_config_args: Optional[Dict] = None  # inline js in the html containing
+
+        # inline js in the html containing
+        self._player_config_args: Optional[Dict] = None
         self._age_restricted: Optional[bool] = None
 
         self._fmt_streams: Optional[List[Stream]] = None
 
         self._initial_data = None
         self._metadata: Optional[YouTubeMetadata] = None
 
@@ -188,15 +195,16 @@
         return self._initial_data
 
     @property
     def streaming_data(self):
         """Return streamingData from video info."""
         if 'streamingData' in self.vid_info:
 
-            invalid_id_list = ['aQvGIIdgFDM']  # List of YouTube error video IDs
+            # List of YouTube error video IDs
+            invalid_id_list = ['aQvGIIdgFDM']
             video_id = self.vid_info['videoDetails']['videoId']
 
             if video_id in invalid_id_list:
                 logger.warning(
                     f'The {self.client} client did not get a valid response, trying to use the WEB client.'
                 )
                 logger.warning(
@@ -205,19 +213,18 @@
                 logger.warning(
                     'Please open an issue at '
                     'https://github.com/JuanBindez/pytubefix/issues '
                     'and provide this log output.'
                 )
 
                 self.try_another_client()
-
-            return self.vid_info['streamingData']
         else:
             self.try_another_client()
-            return self.vid_info['streamingData']
+
+        return self.vid_info['streamingData']
 
     @property
     def fmt_streams(self):
         """Returns a list of streams if they have been initialized.
 
         If the streams have not been initialized, finds all relevant
         streams and initializes them.
@@ -455,25 +462,25 @@
         )
 
         if self._title:
             return self._title.replace('/', '\\')
 
         try:
             self._title = self.vid_info['videoDetails']['title']
-        except KeyError:
+        except KeyError as e:
             # Check_availability will raise the correct exception in most cases
             #  if it doesn't, ask for a report.
             self.check_availability()
             raise exceptions.PytubeFixError(
                 (
                     f'Exception while accessing title of {self.watch_url}. '
                     'Please file a bug report at https://github.com/JuanBindez/pytubefix'
                 )
-            )
-        # print(self.vid_info['videoDetails'])
+            ) from e
+
         return self._title.replace('/', '\\')
 
     @title.setter
     def title(self, value):
         """Sets the title value."""
         self._title = value
 
@@ -553,19 +560,18 @@
 
     @property
     def metadata(self) -> Optional[YouTubeMetadata]:
         """Get the metadata for the video.
 
         :rtype: YouTubeMetadata
         """
-        if self._metadata:
-            return self._metadata
-        else:
-            self._metadata = extract.metadata(self.initial_data)
-            return self._metadata
+        if not self._metadata:
+            self._metadata = extract.metadata(
+                self.initial_data)  # Creating the metadata
+        return self._metadata
 
     def register_on_progress_callback(self, func: Callable[[Any, bytes, int], None]):
         """Register a download progress callback function post initialization.
 
         :param callable func:
             A callback function that takes ``stream``, ``chunk``,
              and ``bytes_remaining`` as parameters.
@@ -590,10 +596,9 @@
     def from_id(video_id: str) -> "YouTube":
         """Construct a :class:`YouTube <YouTube>` object from a video id.
 
         :param str video_id:
             The video id of the YouTube video.
 
         :rtype: :class:`YouTube <YouTube>`
-        
         """
         return YouTube(f"https://www.youtube.com/watch?v={video_id}")
```

### Comparing `pytubefix-5.3rc3/pytubefix/captions.py` & `pytubefix-5.4rc1/pytubefix/captions.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,38 +42,38 @@
     def xml_captions(self) -> str:
         """Download the xml caption tracks."""
         return request.get(self.url)
 
     @property
     def json_captions(self) -> dict:
         """Download and parse the json caption tracks."""
-        json_captions_url = self.url.replace('fmt=srv3','fmt=json3')
+        json_captions_url = self.url.replace('fmt=srv3', 'fmt=json3')
         text = request.get(json_captions_url)
         parsed = json.loads(text)
         assert parsed['wireMagic'] == 'pb3', 'Unexpected captions format'
         return parsed
 
     def generate_srt_captions(self) -> str:
         """Generate "SubRip Subtitle" captions.
 
         Takes the xml captions from :meth:`~pytube.Caption.xml_captions` and
         recompiles them into the "SubRip Subtitle" format.
         """
         return self.xml_caption_to_srt(self.xml_captions)
-    
+
     def save_captions(self, filename: str):
         """Generate and save "SubRip Subtitle" captions to a text file.
 
         Takes the xml captions from :meth:`~pytubefix.Caption.xml_captions` and
         recompiles them into the "SubRip Subtitle" format and saves it to a text file.
-        
+
         :param filename: The name of the file to save the captions.
         """
         srt_captions = self.xml_caption_to_srt(self.xml_captions)
-        
+
         with open(filename, 'w', encoding='utf-8') as file:
             file.write(srt_captions)
 
     @staticmethod
     def float_to_srt_time_format(d: float) -> str:
         """Convert decimal durations into proper srt format.
 
@@ -92,25 +92,27 @@
         """Convert xml caption tracks to "SubRip Subtitle (srt)".
 
         :param str xml_captions:
             XML formatted caption tracks.
         """
         segments = []
         root = ElementTree.fromstring(xml_captions)
-        
-        i=0
+
+        i = 0
         for child in list(root.iter("body"))[0]:
             if child.tag == 'p':
                 caption = ''
-                if len(list(child))==0:
+
+                # I think it will be faster than `len(list(child)) == 0`
+                if not list(child):
                     # instead of 'continue'
                     caption = child.text
                 for s in list(child):
                     if s.tag == 's':
-                        caption += ' ' + s.text
+                        caption += f' {s.text}'
                 caption = unescape(caption.replace("\n", " ").replace("  ", " "),)
                 try:
                     duration = float(child.attrib["d"])/1000.0
                 except KeyError:
                     duration = 0.0
                 start = float(child.attrib["t"])/1000.0
                 end = start + duration
@@ -162,19 +164,15 @@
 
         if filename_prefix:
             filename = f"{safe_filename(filename_prefix)}{filename}"
 
         filename = safe_filename(filename)
 
         filename += f" ({self.code})"
-
-        if srt:
-            filename += ".srt"
-        else:
-            filename += ".xml"
+        filename += ".srt" if srt else ".xml"
 
         file_path = os.path.join(target_directory(output_path), filename)
 
         with open(file_path, "w", encoding="utf-8") as file_handle:
             if srt:
                 file_handle.write(self.generate_srt_captions())
             else:
```

### Comparing `pytubefix-5.3rc3/pytubefix/chapters.py` & `pytubefix-5.4rc1/pytubefix/chapters.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/pytubefix/cipher.py` & `pytubefix-5.4rc1/pytubefix/cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/pytubefix/cli.py` & `pytubefix-5.4rc1/pytubefix/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 
 TODO: REFACTOR THIS FILE
 
 """
 
 
-
 #!/usr/bin/env python3
 """A simple command line application to download youtube videos."""
 
+
 import random
 import argparse
 import gzip
 import json
 import logging
 import os
 import shutil
@@ -21,59 +21,56 @@
 import subprocess  # nosec
 from typing import List, Optional
 import pytubefix.exceptions as exceptions
 from pytubefix import __version__
 from pytubefix import CaptionQuery, Playlist, Stream
 from pytubefix.helpers import safe_filename, setup_logger
 from pytubefix import YouTube
-
-
 logger = logging.getLogger(__name__)
 
+
 def main():
     # TODO: Refactor cli.py to OOP
     # temporary fix
     from pytubefix import YouTube
     # noinspection PyTypeChecker
     parser = argparse.ArgumentParser(description=main.__doc__)
     args = _parse_args(parser)
     if args.verbose:
-        log_filename = None
-        if args.logfile:
-            log_filename = args.logfile
+        log_filename = args.logfile or None
         setup_logger(logging.DEBUG, log_filename=log_filename)
         logger.debug(f'Pytube version: {__version__}')
 
     if not args.url or "youtu" not in args.url:
         parser.print_help()
         sys.exit(1)
 
     if "/playlist" in args.url:
         print("Loading playlist...")
         playlist = Playlist(args.url)
         if not args.target:
             args.target = safe_filename(playlist.title)
+
         for youtube_video in playlist.videos:
             try:
                 _perform_args_on_youtube(youtube_video, args)
             except exceptions.PytubeFixError as e:
                 print(f"There was an error with video: {youtube_video}")
                 print(e)
     else:
         print("Loading video...")
 
         youtube = YouTube(args.url)
         _perform_args_on_youtube(youtube, args)
 
 
-
 def _perform_args_on_youtube(
     youtube: YouTube, args: argparse.Namespace
 ) -> None:
-    if len(sys.argv) == 2 :  # no arguments parsed
+    if len(sys.argv) == 2:  # no arguments parsed
         download_highest_resolution_progressive(
             youtube=youtube, resolution="highest", target=args.target
         )
     if args.list_captions:
         _print_available_captions(youtube.captions)
     if args.list:
         display_streams(youtube)
@@ -104,15 +101,15 @@
 def _parse_args(
     parser: argparse.ArgumentParser, args: Optional[List] = None
 ) -> argparse.Namespace:
     parser.add_argument(
         "url", help="The YouTube /watch or /playlist url", nargs="?"
     )
     parser.add_argument(
-        "--version", action="version", version="%(prog)s " + __version__,
+        "--version", action="version", version=f"%(prog)s {__version__}"
     )
     parser.add_argument(
         "--itag", type=int, help="The itag for the desired stream",
     )
     parser.add_argument(
         "-r",
         "--resolution",
@@ -216,14 +213,15 @@
                     "js": js,
                     "watch_html": watch_html,
                     "video_info": vid_info,
                 }
             ).encode("utf8"),
         )
 
+
 def display_progress_bar(
     bytes_received: int, filesize: int, ch: str = "█", scale: float = 0.55
 ) -> None:
     """Display a simple, pretty progress bar.
 
     Example:
     ~~~~~~~~
@@ -252,15 +250,15 @@
     text = f" ↳ |{progress_bar}| {percent}%\r"
     sys.stdout.write(text)
     sys.stdout.flush()
 
 
 # noinspection PyUnusedLocal
 def on_progress(stream: Stream,
-                chunk: bytes, 
+                chunk: bytes,
                 bytes_remaining: int
                 ) -> None:  # pylint: disable=W0613
 
     filesize = stream.filesize
     bytes_received = filesize - bytes_remaining
     display_progress_bar(bytes_received, filesize)
 
@@ -277,20 +275,19 @@
         print(f"Already downloaded at:\n{file_path}")
         return
 
     stream.download(output_path=target, filename=filename)
     sys.stdout.write("\n")
 
 
-def _unique_name(base: str, 
-                 subtype: str, 
-                 media_type: str, 
+def _unique_name(base: str,
+                 subtype: str,
+                 media_type: str,
                  target: str
                  ) -> str:
-
     """
     Given a base name, the file format, and the target directory, will generate
     a filename unique for that directory and file format.
     :param str base:
         The given base-name.
     :param str subtype:
         The filetype of the video which will be downloaded.
@@ -305,16 +302,16 @@
         file_name = f"{base}_{media_type}_{counter}"
         file_path = os.path.join(target, f"{file_name}.{subtype}")
         if not os.path.exists(file_path):
             return file_name
         counter += 1
 
 
-def ffmpeg_process(youtube: YouTube, 
-                   resolution: str, 
+def ffmpeg_process(youtube: YouTube,
+                   resolution: str,
                    target: Optional[str] = None
                    ) -> None:
     """
     Decides the correct video stream to download, then calls _ffmpeg_downloader.
 
     :param YouTube youtube:
         A valid YouTube object.
@@ -366,16 +363,16 @@
         print("Could not find an audio only stream")
         sys.exit()
     _ffmpeg_downloader(
         audio_stream=audio_stream, video_stream=video_stream, target=target
     )
 
 
-def _ffmpeg_downloader(audio_stream: Stream, 
-                       video_stream: Stream, 
+def _ffmpeg_downloader(audio_stream: Stream,
+                       video_stream: Stream,
                        target: str) -> None:
     """
     Given a YouTube Stream object, finds the correct audio stream, downloads them both
     giving them a unique name, them uses ffmpeg to create a new file with the audio
     and video from the previously downloaded files. Then deletes the original adaptive
     streams, leaving the combination.
```

### Comparing `pytubefix-5.3rc3/pytubefix/colors.py` & `pytubefix-5.4rc1/pytubefix/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Colors to be used in cli"""
 
 
 class Color:
     GREEN = '\033[92m'
-    LIGTH_GREEN = '\033[1;92m'
+    LIGHT_GREEN = '\033[1;92m'
     RED = '\033[91m'
     YELLOW = '\033[93m'
     BLUE = '\033[1;34m'
     MAGENTA = '\033[1;35m'
     BOLD = '\033[;1m'
     CYAN = '\033[1;36m'
     LIGHT_CYAN = '\033[1;96m'
-    LIGTH_GREY = '\033[1;37m'
+    LIGHT_GREY = '\033[1;37m'
     DARK_GREY = '\033[1;90m'
     BLACK = '\033[1;30m'
     WHITE = '\033[1;97m'
-    INVERTE = '\033[;7m'
+    INVERT = '\033[;7m'
     RESET = '\033[0m'
-    
+
 
 GREEN = '\033[92m'
-LIGTH_GREEN = '\033[1;92m'
+LIGHT_GREEN = '\033[1;92m'
 RED = '\033[91m'
 YELLOW = '\033[93m'
 BLUE = '\033[1;34m'
 MAGENTA = '\033[1;35m'
 BOLD = '\033[;1m'
 CYAN = '\033[1;36m'
 LIGHT_CYAN = '\033[1;96m'
-LIGTH_GREY = '\033[1;37m'
+LIGHT_GREY = '\033[1;37m'
 DARK_GREY = '\033[1;90m'
 BLACK = '\033[1;30m'
 WHITE = '\033[1;97m'
 INVERTE = '\033[;7m'
 RESET = '\033[0m'
 
 colors_list = [
```

### Comparing `pytubefix-5.3rc3/pytubefix/contrib/channel.py` & `pytubefix-5.4rc1/pytubefix/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/pytubefix/contrib/playlist.py` & `pytubefix-5.4rc1/pytubefix/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/pytubefix/contrib/search.py` & `pytubefix-5.4rc1/pytubefix/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/pytubefix/exceptions.py` & `pytubefix-5.4rc1/pytubefix/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def __init__(self, caller: str, pattern: Union[str, Pattern]):
         """
         :param str caller:
             Calling function
         :param str pattern:
             Pattern that failed to match
         """
-        super().__init__(c.RED + f"{caller}: could not find match for {pattern}" + c.RESET)
+        super().__init__(f"{c.RED}{caller}: could not find match for {pattern}{c.RESET}")
         self.caller = caller
         self.pattern = pattern
 
 
 class VideoUnavailable(PytubeFixError):
     """Base video unavailable error."""
     def __init__(self, video_id: str):
@@ -47,73 +47,73 @@
             A YouTube video identifier.
         """
         self.video_id = video_id
         super().__init__(self.error_string)
 
     @property
     def error_string(self):
-        return c.RED + f'{self.video_id} is unavailable' + c.RESET
+        return f'{c.RED}{self.video_id} is unavailable{c.RESET}'
 
 
 class AgeRestrictedError(VideoUnavailable):
     """Video is age restricted, and cannot be accessed without OAuth."""
     def __init__(self, video_id: str):
         """
         :param str video_id:
             A YouTube video identifier.
         """
         self.video_id = video_id
         super().__init__(self.video_id)
 
     @property
     def error_string(self):
-        return c.RED + f"Video ID = {self.video_id}: is age restricted, and can't be accessed without logging in." + c.RESET
+        return f"{c.RED}Video ID = {self.video_id}: is age restricted, and can't be accessed without logging in.{c.RESET}"
 
 
 class LiveStreamError(VideoUnavailable):
     """Video is a live stream."""
     def __init__(self, video_id: str):
         """
         :param str video_id:
             A YouTube video identifier.
         """
         self.video_id = video_id
         super().__init__(self.video_id)
 
     @property
     def error_string(self):
-        return c.RED + f'{self.video_id} is streaming live and cannot be loaded' + c.RESET
+        return f'{c.RED}{self.video_id} is streaming live and cannot be loaded{c.RESET}'
 
 
 class VideoPrivate(VideoUnavailable):
     def __init__(self, video_id: str):
         """
         :param str video_id:
             A YouTube video identifier.
         """
         self.video_id = video_id
         super().__init__(self.video_id)
 
     @property
     def error_string(self):
-        return c.RED + f'{self.video_id} is a private video' + c.RESET
+        return f'{c.RED}{self.video_id} is a private video{c.RESET}'
 
 
 class RecordingUnavailable(VideoUnavailable):
     def __init__(self, video_id: str):
         """
         :param str video_id:
             A YouTube video identifier.
         """
         self.video_id = video_id
         super().__init__(self.video_id)
 
     @property
     def error_string(self):
-        return c.RED + f'{self.video_id} does not have a live stream recording available' + c.RESET
+        return f'{c.RED}{self.video_id} does not have a live stream recording available{c.RESET}'
 
 
 class MembersOnly(VideoUnavailable):
     """Video is members-only.
 
     YouTube has special videos that are only viewable to users who have
     subscribed to a content creator.
@@ -125,22 +125,22 @@
             A YouTube video identifier.
         """
         self.video_id = video_id
         super().__init__(self.video_id)
 
     @property
     def error_string(self):
-        return c.RED + f'{self.video_id} is a members-only video' + c.RESET
+        return f'{c.RED}{self.video_id} is a members-only video{c.RESET}'
 
 
 class VideoRegionBlocked(VideoUnavailable):
     def __init__(self, video_id: str):
         """
         :param str video_id:
             A YouTube video identifier.
         """
         self.video_id = video_id
         super().__init__(self.video_id)
 
     @property
     def error_string(self):
-        return c.RED + f'{self.video_id} is not available in your region' + c.RESET
+        return f'{c.RED}{self.video_id} is not available in your region{c.RESET}'
```

### Comparing `pytubefix-5.3rc3/pytubefix/extract.py` & `pytubefix-5.4rc1/pytubefix/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
             ("cver", "7.20201028"),
         ]
     )
     return _video_info_url(params)
 
 
 def _video_info_url(params: OrderedDict) -> str:
-    return "https://www.youtube.com/get_video_info?" + urlencode(params)
+    return f"https://www.youtube.com/get_video_info?{urlencode(params)}"
 
 
 def js_url(html: str) -> str:
     """Get the base JavaScript url.
 
     Construct the base JavaScript url, which contains the decipher
     "transforms".
@@ -264,15 +264,15 @@
     :param str html:
         The html contents of the watch page.
     """
     try:
         base_js = get_ytplayer_config(html)['assets']['js']
     except (KeyError, RegexMatchError):
         base_js = get_ytplayer_js(html)
-    return "https://youtube.com" + base_js
+    return f"https://youtube.com{base_js}"
 
 
 def mime_type_codec(mime_type_codec: str) -> Tuple[str, List[str]]:
     """Parse the type data.
 
     Breaks up the data in the ``type`` key of the manifest, which contains the
     mime type and codecs serialized together, and splits them into separate
@@ -391,15 +391,15 @@
         try:
             found_objects = parse_for_all_objects(html, pattern)
             for obj in found_objects:
                 ytcfg.update(obj)
         except HTMLParseError:
             continue
 
-    if len(ytcfg) > 0:
+    if ytcfg: # there is at least one item
         return ytcfg
 
     raise RegexMatchError(
         caller="get_ytcfg", pattern="ytcfg_pattenrs"
     )
 
 
@@ -490,19 +490,18 @@
     if 'formats' in stream_data.keys():
         formats.extend(stream_data['formats'])
     if 'adaptiveFormats' in stream_data.keys():
         formats.extend(stream_data['adaptiveFormats'])
 
     # Extract url and s from signatureCiphers as necessary
     for data in formats:
-        if 'url' not in data:
-            if 'signatureCipher' in data:
-                cipher_url = parse_qs(data['signatureCipher'])
-                data['url'] = cipher_url['url'][0]
-                data['s'] = cipher_url['s'][0]
+        if 'url' not in data and 'signatureCipher' in data:
+            cipher_url = parse_qs(data['signatureCipher'])
+            data['url'] = cipher_url['url'][0]
+            data['s'] = cipher_url['s'][0]
         data['is_otf'] = data.get('type') == 'FORMAT_STREAM_TYPE_OTF'
 
     logger.debug("applying descrambler")
     return formats
 
 
 def initial_data(watch_html: str) -> dict:
```

### Comparing `pytubefix-5.3rc3/pytubefix/helpers.py` & `pytubefix-5.4rc1/pytubefix/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class DeferredGeneratorList:
     """A wrapper class for deferring list generation.
 
-    Pytube has some continuation generators that create web calls, which means
+    Pytubefix has some continuation generators that create web calls, which means
     that any time a full list is requested, all of those web calls must be
     made at once, which could lead to slowdowns. This will allow individual
     elements to be queried, so that slowdowns only happen as necessary. For
     example, you can iterate over elements in the list without accessing them
     all simultaneously. This should allow for speed improvements for playlist
     and channel interactions.
     """
@@ -144,15 +144,15 @@
     :param int max_length:
         The maximum filename character length.
     :rtype: str
     :returns:
         A sanitized string.
     """
     # Characters in range 0-31 (0x00-0x1F) are not allowed in ntfs filenames.
-    ntfs_characters = [chr(i) for i in range(0, 31)]
+    ntfs_characters = [chr(i) for i in range(31)]
     characters = [
         r'"',
         r"\#",
         r"\$",
         r"\%",
         r"'",
         r"\*",
@@ -301,15 +301,15 @@
     :param str vid_id
         YouTube video id
 
     :return dict data
         Dict used to generate the json.gz file
     """
     from pytubefix import YouTube
-    gzip_filename = 'yt-video-%s-html.json.gz' % vid_id
+    gzip_filename = f'yt-video-{vid_id}-html.json.gz'
 
     # Get the pytube directory in order to navigate to /tests/mocks
     pytube_dir_path = os.path.abspath(
         os.path.join(
             os.path.dirname(__file__),
             os.path.pardir
         )
@@ -328,11 +328,12 @@
 
     logger.info(f'Outputing json.gz file to {gzip_filepath}')
     with gzip.open(gzip_filepath, 'wb') as f:
         f.write(json.dumps(html_data).encode('utf-8'))
 
     return html_data
 
+
 # Remove ANSI color codes from a colored string
 def strip_color_codes(input_str):
     ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
     return ansi_escape.sub('', input_str)
```

### Comparing `pytubefix-5.3rc3/pytubefix/innertube.py` & `pytubefix-5.4rc1/pytubefix/innertube.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,23 +299,21 @@
         self.use_oauth = use_oauth
         self.allow_cache = allow_cache
 
         # Stored as epoch time
         self.expires = None
 
         # Try to load from file if specified
-        if self.use_oauth and self.allow_cache:
-            # Try to load from file if possible
-            if os.path.exists(_token_file):
-                with open(_token_file) as f:
-                    data = json.load(f)
-                    self.access_token = data['access_token']
-                    self.refresh_token = data['refresh_token']
-                    self.expires = data['expires']
-                    self.refresh_bearer_token()
+        if self.use_oauth and self.allow_cache and os.path.exists(_token_file):
+            with open(_token_file) as f:
+                data = json.load(f)
+                self.access_token = data['access_token']
+                self.refresh_token = data['refresh_token']
+                self.expires = data['expires']
+                self.refresh_bearer_token()
 
     def cache_tokens(self):
         """Cache tokens to file if allowed."""
         if not self.allow_cache:
             return
 
         data = {
@@ -434,18 +432,18 @@
         headers = {
             'Content-Type': 'application/json',
         }
         # Add the bearer token if applicable
         if self.use_oauth:
             if self.access_token:
                 self.refresh_bearer_token()
-                headers['Authorization'] = f'Bearer {self.access_token}'
             else:
                 self.fetch_bearer_token()
-                headers['Authorization'] = f'Bearer {self.access_token}'
+
+            headers['Authorization'] = f'Bearer {self.access_token}'
 
         headers.update(self.header)
 
         response = request._execute_request(
             endpoint_url,
             'POST',
             headers=headers,
```

### Comparing `pytubefix-5.3rc3/pytubefix/itags.py` & `pytubefix-5.4rc1/pytubefix/itags.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,25 +125,22 @@
 }
 
 HDR = [330, 331, 332, 333, 334, 335, 336, 337]
 _3D = [82, 83, 84, 85, 100, 101, 102]
 LIVE = [91, 92, 93, 94, 95, 96, 132, 151]
 
 
-def get_format_profile(itag: int) -> Dict:
+def get_format_profile(itag: str) -> Dict:
     """Get additional format information for a given itag.
 
     :param str itag:
         YouTube format identifier code.
     """
     itag = int(itag)
-    if itag in ITAGS:
-        res, bitrate = ITAGS[itag]
-    else:
-        res, bitrate = None, None
+    res, bitrate = ITAGS[itag] if itag in ITAGS else (None, None)
     return {
         "resolution": res,
         "abr": bitrate,
         "is_live": itag in LIVE,
         "is_3d": itag in _3D,
         "is_hdr": itag in HDR,
         "is_dash": (
```

### Comparing `pytubefix-5.3rc3/pytubefix/jsinterp.py` & `pytubefix-5.4rc1/pytubefix/jsinterp.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/pytubefix/metadata.py` & `pytubefix-5.4rc1/pytubefix/metadata.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/pytubefix/parser.py` & `pytubefix-5.4rc1/pytubefix/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 # Some of the instances might fail because set is technically
                 # a method of the ytcfg object. We'll skip these since they
                 # don't seem relevant at the moment.
                 continue
             else:
                 result.append(obj)
 
-    if len(result) == 0:
+    if not result:
         raise HTMLParseError(f'No matches for regex {preceding_regex}')
 
     return result
 
 
 def parse_for_object(html, preceding_regex):
     """Parses input html to find the end of a JavaScript object.
@@ -84,15 +84,15 @@
         '[': ']',
         '"': '"',
         '\'': '\'',
         '/': '/' # javascript regex
     }
 
     while i < len(html):
-        if len(stack) == 0:
+        if not stack:
             break
         if curr_char not in [' ', '\n']:
             last_char = curr_char
         curr_char = html[i]
         curr_context = stack[-1]
 
         # If we've reached a context closer, we can remove an element off the stack
```

### Comparing `pytubefix-5.3rc3/pytubefix/query.py` & `pytubefix-5.4rc1/pytubefix/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,15 @@
             YouTube format identifier code.
         :rtype: :class:`Stream <Stream>` or None
         :returns:
             The :class:`Stream <Stream>` matching the given itag or None if
             not found.
 
         """
+        # TODO: You need to make sure itag is an int or str, if it is a int remove casting.
         return self.itag_index.get(int(itag))
 
     def get_by_resolution(self, resolution: str) -> Optional[Stream]:
         """Get the corresponding :class:`Stream <Stream>` for a given resolution.
 
         Stream must be a progressive mp4.
 
@@ -376,23 +377,20 @@
         """
         try:
             return self.fmt_streams[-1]
         except IndexError:
             pass
 
     @deprecated("Get the size of this list directly using len()")
-    def count(self, value: Optional[str] = None) -> int:  # pragma: no cover
+    def count(self, value: Optional[str] = None) -> int:    # pragma: no cover
         """Get the count of items in the list.
 
         :rtype: int
         """
-        if value:
-            return self.fmt_streams.count(value)
-
-        return len(self)
+        return self.fmt_streams.count(value) if value else len(self)
 
     @deprecated("This object can be treated as a list, all() is useless")
     def all(self) -> List[Stream]:  # pragma: no cover
         """Get all the results represented by this query as a list.
 
         :rtype: list
```

### Comparing `pytubefix-5.3rc3/pytubefix/request.py` & `pytubefix-5.4rc1/pytubefix/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,15 @@
     headers=None,
     data=None,
     timeout=socket._GLOBAL_DEFAULT_TIMEOUT
 ):
     base_headers = {"User-Agent": "Mozilla/5.0", "accept-language": "en-US,en"}
     if headers:
         base_headers.update(headers)
-    if data:
-        # encode data for request
-        if not isinstance(data, bytes):
+    if data and not isinstance(data, bytes): # encode data for request
             data = bytes(json.dumps(data), encoding="utf-8")
     if url.lower().startswith("http"):
         request = Request(url, headers=base_headers, method=method, data=data)
     else:
         raise ValueError("Invalid URL")
     return urlopen(request, timeout=timeout)  # nosec
 
@@ -92,15 +90,15 @@
 
     """Read the response in sequence.
     :param str url: The URL to perform the GET request for.
     :rtype: Iterable[bytes]
     """
     # YouTube expects a request sequence number as part of the parameters.
     split_url = parse.urlsplit(url)
-    base_url = '%s://%s/%s?' % (split_url.scheme, split_url.netloc, split_url.path)
+    base_url = f'{split_url.scheme}://{split_url.netloc}/{split_url.path}?'
 
     querys = dict(parse.parse_qsl(split_url.query))
 
     # The 0th sequential request provides the file headers, which tell us
     #  information about how the file is segmented.
     querys['sq'] = 0
     url = base_url + parse.urlencode(querys)
@@ -150,37 +148,35 @@
             # If the max retries is exceeded, raise an exception
             if tries >= 1 + max_retries:
                 raise MaxRetriesExceeded()
 
             # Try to execute the request, ignoring socket timeouts
             try:
                 response = _execute_request(
-                    url + f"&range={downloaded}-{stop_pos}",
+                    f"{url}&range={downloaded}-{stop_pos}",
                     method="GET",
                     timeout=timeout
                 )
             except URLError as e:
                 # We only want to skip over timeout errors, and
                 # raise any other URLError exceptions
-                if isinstance(e.reason, socket.timeout):
-                    pass
-                else:
+                if not isinstance(e.reason, socket.timeout):
                     raise
             except http.client.IncompleteRead:
                 # Allow retries on IncompleteRead errors for unreliable connections
                 pass
             else:
                 # On a successful request, break from loop
                 break
             tries += 1
 
         if file_size == default_range_size:
             try:
                 resp = _execute_request(
-                    url + f"&range={0}-{99999999999}",
+                    f"{url}&range=0-99999999999",
                     method="GET",
                     timeout=timeout
                 )
                 content_range = resp.info()["Content-Length"]
                 file_size = int(content_range)
             except (KeyError, IndexError, ValueError) as e:
                 logger.error(e)
@@ -214,15 +210,15 @@
 
     :param str url: The URL to get the size of
     :returns: int: size in bytes of remote file
     """
     total_filesize = 0
     # YouTube expects a request sequence number as part of the parameters.
     split_url = parse.urlsplit(url)
-    base_url = '%s://%s/%s?' % (split_url.scheme, split_url.netloc, split_url.path)
+    base_url = f'{split_url.scheme}://{split_url.netloc}/{split_url.path}?'
     querys = dict(parse.parse_qsl(split_url.query))
 
     # The 0th sequential request provides the file headers, which tell us
     #  information about how the file is segmented.
     querys['sq'] = 0
     url = base_url + parse.urlencode(querys)
     response = _execute_request(
```

### Comparing `pytubefix-5.3rc3/pytubefix/streams.py` & `pytubefix-5.4rc1/pytubefix/streams.py`

 * *Files 9% similar despite different names*

```diff
@@ -270,23 +270,45 @@
                 filename: Optional[str] = None,
                 filename_prefix: Optional[str] = None,
                 skip_existing: bool = True,
                 timeout: Optional[int] = None,
                 max_retries: Optional[int] = 0,
                 mp3: bool = False) -> str:
         
-        if mp3:
-            filename = self.title + ".mp3"
+        """
+        Download the file from the URL provided by `self.url`.
 
-            file_path = self.get_file_path(
-                filename=filename,
-                output_path=output_path,
-                filename_prefix=filename_prefix,
-            )
-    
+        Args:
+            output_path (Optional[str]): Path where the downloaded file will be saved.
+            filename (Optional[str]): Name of the downloaded file.
+            filename_prefix (Optional[str]): Prefix to be added to the filename.
+            skip_existing (bool): Whether to skip the download if the file already exists.
+            timeout (Optional[int]): Timeout for the download request.
+            max_retries (Optional[int]): Maximum number of retries for the download.
+            mp3 (bool): Whether the file to be downloaded is an MP3 audio file.
+
+        Returns:
+            str: File path of the downloaded file.
+
+        Raises:
+            HTTPError: If an HTTP error occurs during the download.
+
+        Note:
+            If `mp3` is set to True, the downloaded file will be assumed to be an MP3 audio file.
+            If `filename` is not provided and `mp3` is True, the title of the resource will be used as the filename with '.mp3' extension.
+            If `filename` is provided and `mp3` is True, '.mp3' extension will be appended to the filename.
+            The progress of the download is tracked using the `on_progress` callback.
+            The `on_complete` callback is triggered after the download is completed.
+        """
+        
+        if mp3:
+            if filename is None:
+                filename = self.title + ".mp3"
+            else:
+                filename = filename + ".mp3"
 
         file_path = self.get_file_path(
             filename=filename,
             output_path=output_path,
             filename_prefix=filename_prefix,
         )
 
@@ -309,29 +331,27 @@
                     bytes_remaining -= len(chunk)
                     # send to the on_progress callback.
                     self.on_progress(chunk, fh, bytes_remaining)
             except HTTPError as e:
                 if e.code != 404:
                     raise
             except StopIteration:
-                pass
                 # Some adaptive streams need to be requested with sequence numbers
                 for chunk in request.seq_stream(
                     self.url,
                     timeout=timeout,
                     max_retries=max_retries
                 ):
                     # reduce the (bytes) remainder by the length of the chunk.
                     bytes_remaining -= len(chunk)
                     # send to the on_progress callback.
                     self.on_progress(chunk, fh, bytes_remaining)
-            
+
         self.on_complete(file_path)
         return file_path
-    
 
     def get_file_path(
         self,
         filename: Optional[str] = None,
         output_path: Optional[str] = None,
         filename_prefix: Optional[str] = None,
     ) -> str:
```

### Comparing `pytubefix-5.3rc3/pytubefix.egg-info/PKG-INFO` & `pytubefix-5.4rc1/pytubefix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.3rc3
+Version: 5.4rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.3rc3 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.4rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.3rc3/pytubefix.egg-info/SOURCES.txt` & `pytubefix-5.4rc1/pytubefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_captions.py` & `pytubefix-5.4rc1/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_cipher.py` & `pytubefix-5.4rc1/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_cli.py` & `pytubefix-5.4rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_exceptions.py` & `pytubefix-5.4rc1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_extract.py` & `pytubefix-5.4rc1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_helpers.py` & `pytubefix-5.4rc1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_main.py` & `pytubefix-5.4rc1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_parser.py` & `pytubefix-5.4rc1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_query.py` & `pytubefix-5.4rc1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_request.py` & `pytubefix-5.4rc1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc3/tests/test_streams.py` & `pytubefix-5.4rc1/tests/test_streams.py`

 * *Files identical despite different names*

