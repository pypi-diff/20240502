# Comparing `tmp/sts_lib-0.30.0.tar.gz` & `tmp/sts_lib-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.30.0.tar", last modified: Tue Apr 30 13:22:29 2024, max compression
+gzip compressed data, was "sts_lib-0.30.1.tar", last modified: Thu May  2 00:54:30 2024, max compression
```

## Comparing `sts_lib-0.30.0.tar` & `sts_lib-0.30.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.275998 sts_lib-0.30.0/
--rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.30.0/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.30.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6916 2024-04-30 13:22:29.275998 sts_lib-0.30.0/PKG-INFO
--rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.30.0/README.md
--rw-rw-rw-   0        0        0     1728 2024-04-30 13:22:29.277996 sts_lib-0.30.0/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.30.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.234227 sts_lib-0.30.0/sts/
--rw-rw-rw-   0        0        0    52950 2024-04-30 13:22:07.000000 sts_lib-0.30.0/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.30.0/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-04-30 13:21:35.000000 sts_lib-0.30.0/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.235226 sts_lib-0.30.0/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.247209 sts_lib-0.30.0/sts/data/config/
--rw-rw-rw-   0        0        0      915 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      608 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      346 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      410 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      419 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      267 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      417 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      607 2024-04-30 13:22:07.000000 sts_lib-0.30.0/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      247 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      261 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      267 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      245 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      606 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      670 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      344 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.263198 sts_lib-0.30.0/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    22625 2024-04-30 13:22:07.000000 sts_lib-0.30.0/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.266180 sts_lib-0.30.0/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-04-30 13:22:01.000000 sts_lib-0.30.0/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 13:22:29.273998 sts_lib-0.30.0/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     6916 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-30 13:22:29.000000 sts_lib-0.30.0/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 00:54:30.930103 sts_lib-0.30.1/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.30.1/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.30.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6916 2024-05-02 00:54:30.930103 sts_lib-0.30.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.30.1/README.md
+-rw-rw-rw-   0        0        0     1728 2024-05-02 00:54:30.930103 sts_lib-0.30.1/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.30.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:54:30.876692 sts_lib-0.30.1/sts/
+-rw-rw-rw-   0        0        0    52950 2024-05-02 00:53:14.000000 sts_lib-0.30.1/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.30.1/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:54:30.892336 sts_lib-0.30.1/sts/data/
+drwxrwxrwx   0        0        0        0 2024-05-02 00:54:30.892336 sts_lib-0.30.1/sts/data/config/
+-rw-rw-rw-   0        0        0      915 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      608 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      346 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      410 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      419 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      267 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      417 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      607 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      247 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      261 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      267 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      245 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      606 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      670 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      344 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-05-02 00:54:30.914465 sts_lib-0.30.1/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-05-02 00:53:33.000000 sts_lib-0.30.1/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    22659 2024-05-02 00:54:15.000000 sts_lib-0.30.1/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-05-02 00:54:30.914465 sts_lib-0.30.1/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-05-02 00:54:03.000000 sts_lib-0.30.1/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-05-02 00:53:09.000000 sts_lib-0.30.1/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 00:54:30.930103 sts_lib-0.30.1/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     6916 2024-05-02 00:54:30.000000 sts_lib-0.30.1/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-05-02 00:54:30.000000 sts_lib-0.30.1/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 00:54:30.000000 sts_lib-0.30.1/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-02 00:54:30.000000 sts_lib-0.30.1/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-05-02 00:54:30.000000 sts_lib-0.30.1/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-02 00:54:30.000000 sts_lib-0.30.1/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.30.0/LICENSE` & `sts_lib-0.30.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/PKG-INFO` & `sts_lib-0.30.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.30.0
+Version: 0.30.1
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.30.0/README.md` & `sts_lib-0.30.1/README.md`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/setup.cfg` & `sts_lib-0.30.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/__init__.py` & `sts_lib-0.30.1/sts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.30.0'
+__version__ = '0.30.1'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 StsConvExclude = namedtuple('StsConvExclude', ['text'])
 
 
 class StreamList(list):
```

### Comparing `sts_lib-0.30.0/sts/cli.py` & `sts_lib-0.30.1/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/config/_default.json` & `sts_lib-0.30.1/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/config/hk2s.json` & `sts_lib-0.30.1/sts/data/config/hk2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/config/s2twp.json` & `sts_lib-0.30.1/sts/data/config/s2twp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/config/tw2s.json` & `sts_lib-0.30.1/sts/data/config/tw2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/config/tw2sp.json` & `sts_lib-0.30.1/sts/data/config/tw2sp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.30.1/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.30.1/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.30.1/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.30.1/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.30.1/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.30.1/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.30.1/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.30.1/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.30.1/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.30.1/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.30.1/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.30.1/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/htmlpage.tpl.html` & `sts_lib-0.30.1/sts/data/htmlpage.tpl.html`

 * *Files 0% similar despite different names*

```diff
@@ -438,14 +438,15 @@
       cmd = await new Promise((resolve, reject) => {
         function onClose(event) {
           dialog.removeEventListener('close', onClose);
           const rv = dialog.returnValue ? dialog.querySelector('form').cmd.value : null;
           resolve(rv);
         }
         dialog.addEventListener('close', onClose);
+        dialog.returnValue = '';
         dialog.showModal();
       });
     } else {
       const idxMap = Array.from(Object.keys(cmds));
       const options = idxMap.map((cmd, i) => `${i + 1}.${cmds[cmd]}`);
       const msg = "請輸入要執行的指令：\n" + options.join('\n');
       const idx = parseInt(prompt(msg), 10);
```

### Comparing `sts_lib-0.30.0/sts/data/scheme/st_multi.txt` & `sts_lib-0.30.1/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts/data/scheme/variant.txt` & `sts_lib-0.30.1/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.0/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.30.1/sts_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.30.0
+Version: 0.30.1
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.30.0/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.30.1/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

