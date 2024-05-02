# Comparing `tmp/libgunshotmatch-0.9.0.tar.gz` & `tmp/libgunshotmatch-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libgunshotmatch-0.9.0.tar", last modified: Thu Feb 29 08:25:41 2024, max compression
+gzip compressed data, was "libgunshotmatch-0.9.1.tar", last modified: Tue Mar  5 16:54:14 2024, max compression
```

## Comparing `libgunshotmatch-0.9.0.tar` & `libgunshotmatch-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-29 08:25:41.155012 libgunshotmatch-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-02-29 08:25:41.163011 libgunshotmatch-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-02-29 08:25:41.159011 libgunshotmatch-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-29 08:25:41.159011 libgunshotmatch-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-02-29 08:25:41.163011 libgunshotmatch-0.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/datafile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/gzip_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/peak.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-02-29 08:25:18.167210 libgunshotmatch-0.9.0/libgunshotmatch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-02-29 08:25:18.167210 libgunshotmatch-0.9.0/libgunshotmatch/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/project.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/comparison/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/comparison/unknowns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/comparison/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/method/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/consolidate/_spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/consolidate/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    22736 2024-02-29 08:25:18.163210 libgunshotmatch-0.9.0/libgunshotmatch/consolidate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-05 16:54:14.239271 libgunshotmatch-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-03-05 16:54:14.243271 libgunshotmatch-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-05 16:54:14.243271 libgunshotmatch-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-05 16:54:14.243271 libgunshotmatch-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-03-05 16:54:14.243271 libgunshotmatch-0.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-03-05 16:53:48.579376 libgunshotmatch-0.9.1/libgunshotmatch/datafile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-05 16:53:48.575376 libgunshotmatch-0.9.1/libgunshotmatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-05 16:53:48.579376 libgunshotmatch-0.9.1/libgunshotmatch/gzip_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-03-05 16:53:48.579376 libgunshotmatch-0.9.1/libgunshotmatch/peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-03-05 16:53:48.579376 libgunshotmatch-0.9.1/libgunshotmatch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-03-05 16:53:48.579376 libgunshotmatch-0.9.1/libgunshotmatch/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-03-05 16:53:48.579376 libgunshotmatch-0.9.1/libgunshotmatch/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 16:53:48.579376 libgunshotmatch-0.9.1/libgunshotmatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-05 16:53:48.575376 libgunshotmatch-0.9.1/libgunshotmatch/comparison/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-03-05 16:53:48.575376 libgunshotmatch-0.9.1/libgunshotmatch/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-05 16:53:48.575376 libgunshotmatch-0.9.1/libgunshotmatch/comparison/unknowns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-05 16:53:48.575376 libgunshotmatch-0.9.1/libgunshotmatch/comparison/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-03-05 16:53:48.579376 libgunshotmatch-0.9.1/libgunshotmatch/method/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-03-05 16:53:48.579376 libgunshotmatch-0.9.1/libgunshotmatch/method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-05 16:53:48.575376 libgunshotmatch-0.9.1/libgunshotmatch/consolidate/_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-05 16:53:48.575376 libgunshotmatch-0.9.1/libgunshotmatch/consolidate/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22736 2024-03-05 16:53:48.575376 libgunshotmatch-0.9.1/libgunshotmatch/consolidate/__init__.py
```

### Comparing `libgunshotmatch-0.9.0/LICENSE` & `libgunshotmatch-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/PKG-INFO` & `libgunshotmatch-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libgunshotmatch
-Version: 0.9.0
+Version: 0.9.1
 Summary: Base library for GunShotMatch.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Home-page: https://github.com/GunShotMatch/libgunshotmatch
 Project-URL: Issue Tracker, https://github.com/GunShotMatch/libgunshotmatch/issues
 Project-URL: Source Code, https://github.com/GunShotMatch/libgunshotmatch
 Project-URL: Documentation, https://libgunshotmatch.readthedocs.io/en/latest
@@ -131,15 +131,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/libgunshotmatch
 	:target: https://github.com/GunShotMatch/libgunshotmatch/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/libgunshotmatch
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/libgunshotmatch/v0.9.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/libgunshotmatch/v0.9.1
 	:target: https://github.com/GunShotMatch/libgunshotmatch/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/libgunshotmatch
 	:target: https://github.com/GunShotMatch/libgunshotmatch/commit/master
 	:alt: GitHub last commit
```

### Comparing `libgunshotmatch-0.9.0/pyproject.toml` & `libgunshotmatch-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "libgunshotmatch"
-version = "0.9.0"
+version = "0.9.1"
 description = "Base library for GunShotMatch."
 readme = "README.rst"
 keywords = []
 dynamic = []
 dependencies = [
     "attrs>=23.1.0",
     "chemistry-tools>=v1.0.0b2",
```

### Comparing `libgunshotmatch-0.9.0/README.rst` & `libgunshotmatch-0.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/libgunshotmatch
 	:target: https://github.com/GunShotMatch/libgunshotmatch/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/libgunshotmatch
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/libgunshotmatch/v0.9.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/libgunshotmatch/v0.9.1
 	:target: https://github.com/GunShotMatch/libgunshotmatch/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/libgunshotmatch
 	:target: https://github.com/GunShotMatch/libgunshotmatch/commit/master
 	:alt: GitHub last commit
```

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/datafile.py` & `libgunshotmatch-0.9.1/libgunshotmatch/datafile.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/__init__.py` & `libgunshotmatch-0.9.1/libgunshotmatch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2023 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.9.0"
+__version__: str = "0.9.1"
 __email__: str = "dominic@davis-foster.co.uk"
```

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/gzip_util.py` & `libgunshotmatch-0.9.1/libgunshotmatch/gzip_util.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/peak.py` & `libgunshotmatch-0.9.1/libgunshotmatch/peak.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/utils.py` & `libgunshotmatch-0.9.1/libgunshotmatch/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 # stdlib
 from decimal import Decimal
 from typing import TYPE_CHECKING, Any, Iterable, List, Optional, Sequence, Tuple, Type, TypeVar, Union
 
 # 3rd party
 import numpy
+from attr import AttrsInstance
 from chemistry_tools.spectrum_similarity import SpectrumSimilarity
 from mathematical.utils import rounders
 from pyms.DPA.Alignment import Alignment
 from pyms.Peak.Class import Peak
 from pyms.Spectrum import MassSpectrum
 from scipy.stats import truncnorm  # type: ignore[import-untyped]
 
@@ -110,18 +111,18 @@
 			xlim=(45, 500),  # TODO: configurable or taken from spectra
 			)
 
 	match, rmatch = sim.score()
 	return match * 1000
 
 
-_O = TypeVar("_O", bound=object)
+_AI = TypeVar("_AI", bound=AttrsInstance)
 
 
-def _fix_init_annotations(method: Type[_O]) -> Type[_O]:
+def _fix_init_annotations(method: Type[_AI]) -> Type[_AI]:
 	init_annotations = method.__init__.__annotations__
 	cls_annotations = method.__annotations__
 
 	for k, v in cls_annotations.items():
 		if k in init_annotations:
 			if init_annotations[k] is Any:
 				init_annotations[k] = v
```

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/search.py` & `libgunshotmatch-0.9.1/libgunshotmatch/search.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/project.py` & `libgunshotmatch-0.9.1/libgunshotmatch/project.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/comparison/_utils.py` & `libgunshotmatch-0.9.1/libgunshotmatch/comparison/_utils.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/comparison/__init__.py` & `libgunshotmatch-0.9.1/libgunshotmatch/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/comparison/unknowns.py` & `libgunshotmatch-0.9.1/libgunshotmatch/comparison/unknowns.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/comparison/projects.py` & `libgunshotmatch-0.9.1/libgunshotmatch/comparison/projects.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/method/_fields.py` & `libgunshotmatch-0.9.1/libgunshotmatch/method/_fields.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/method/__init__.py` & `libgunshotmatch-0.9.1/libgunshotmatch/method/__init__.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/consolidate/_spectra.py` & `libgunshotmatch-0.9.1/libgunshotmatch/consolidate/_spectra.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/consolidate/_fields.py` & `libgunshotmatch-0.9.1/libgunshotmatch/consolidate/_fields.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch-0.9.0/libgunshotmatch/consolidate/__init__.py` & `libgunshotmatch-0.9.1/libgunshotmatch/consolidate/__init__.py`

 * *Files identical despite different names*

