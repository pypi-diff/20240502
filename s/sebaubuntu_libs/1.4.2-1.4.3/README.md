# Comparing `tmp/sebaubuntu_libs-1.4.2.tar.gz` & `tmp/sebaubuntu_libs-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sebaubuntu_libs-1.4.2.tar", max compression
+gzip compressed data, was "sebaubuntu_libs-1.4.3.tar", max compression
```

## Comparing `sebaubuntu_libs-1.4.2.tar` & `sebaubuntu_libs-1.4.3.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0      891 2024-02-09 22:48:50.706982 sebaubuntu_libs-1.4.2/README.md
--rw-r--r--   0        0        0      688 2024-02-11 04:35:52.765224 sebaubuntu_libs-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      196 2024-02-11 04:35:55.738571 sebaubuntu_libs-1.4.2/sebaubuntu_libs/__init__.py
--rw-r--r--   0        0        0     6035 2024-02-11 04:33:41.381281 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libaik/__init__.py
--rw-r--r--   0        0        0      105 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/__init__.py
--rw-r--r--   0        0        0     7010 2024-02-10 04:07:48.496895 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/device_info.py
--rw-r--r--   0        0        0      106 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/elf/__init__.py
--rw-r--r--   0        0        0      828 2024-02-07 03:12:58.691914 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/elf/elf.py
--rw-r--r--   0        0        0     1790 2024-02-07 03:13:29.788597 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/elf/shared_library.py
--rw-r--r--   0        0        0     4156 2024-02-10 04:09:38.911471 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/fstab/__init__.py
--rw-r--r--   0        0        0      115 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/partitions/__init__.py
--rw-r--r--   0        0        0     2102 2024-02-07 02:39:13.511273 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/partitions/partition.py
--rw-r--r--   0        0        0     2310 2024-02-07 03:13:39.378603 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/partitions/partition_model.py
--rw-r--r--   0        0        0     2466 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/partitions/partitions.py
--rw-r--r--   0        0        0     2289 2024-02-07 02:36:25.643377 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/props/__init__.py
--rw-r--r--   0        0        0     1361 2024-02-07 02:47:09.521468 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/props/utils.py
--rw-r--r--   0        0        0     2992 2024-02-07 03:12:22.731907 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/versions.py
--rw-r--r--   0        0        0      132 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/vintf/__init__.py
--rw-r--r--   0        0        0     1924 2024-02-07 03:15:32.548731 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/vintf/aidl.py
--rw-r--r--   0        0        0      451 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/vintf/common.py
--rw-r--r--   0        0        0     4508 2024-02-10 02:42:10.410105 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/vintf/hidl.py
--rw-r--r--   0        0        0     2382 2024-02-07 03:10:14.118651 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/vintf/manifest.py
--rw-r--r--   0        0        0      395 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libexception/__init__.py
--rw-r--r--   0        0        0      131 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/__init__.py
--rw-r--r--   0        0        0     1260 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/account.py
--rw-r--r--   0        0        0     4151 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/contents.py
--rw-r--r--   0        0        0     2959 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/raw_api/__init__.py
--rw-r--r--   0        0        0     1344 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/raw_api/rest.py
--rw-r--r--   0        0        0      437 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/session.py
--rw-r--r--   0        0        0     2553 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/utils.py
--rw-r--r--   0        0        0      187 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/liblocale/__init__.py
--rw-r--r--   0        0        0      517 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/liblogging/__init__.py
--rw-r--r--   0        0        0      443 2024-02-07 03:20:02.006003 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libnekobin/__init__.py
--rw-r--r--   0        0        0      323 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libpath/__init__.py
--rw-r--r--   0        0        0     1755 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libreorder/__init__.py
--rw-r--r--   0        0        0      435 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libsed/__init__.py
--rw-r--r--   0        0        0      436 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libstring/__init__.py
--rw-r--r--   0        0        0      301 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.2/sebaubuntu_libs/libtyping/__init__.py
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 sebaubuntu_libs-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0      838 2024-04-30 08:05:08.346788 sebaubuntu_libs-1.4.3/README.md
+-rw-r--r--   0        0        0      688 2024-05-02 14:02:06.347460 sebaubuntu_libs-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      196 2024-05-02 14:02:11.067521 sebaubuntu_libs-1.4.3/sebaubuntu_libs/__init__.py
+-rw-r--r--   0        0        0     6035 2024-02-11 04:33:41.381281 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libaik/__init__.py
+-rw-r--r--   0        0        0      105 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/__init__.py
+-rw-r--r--   0        0        0     7036 2024-05-02 13:57:43.487707 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/device_info.py
+-rw-r--r--   0        0        0      106 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/elf/__init__.py
+-rw-r--r--   0        0        0      828 2024-02-07 03:12:58.691914 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/elf/elf.py
+-rw-r--r--   0        0        0     1790 2024-02-07 03:13:29.788597 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/elf/shared_library.py
+-rw-r--r--   0        0        0     4156 2024-02-10 04:09:38.911471 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/fstab/__init__.py
+-rw-r--r--   0        0        0      115 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/partitions/__init__.py
+-rw-r--r--   0        0        0     2102 2024-02-07 02:39:13.511273 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/partitions/partition.py
+-rw-r--r--   0        0        0     2310 2024-02-07 03:13:39.378603 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/partitions/partition_model.py
+-rw-r--r--   0        0        0     2466 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/partitions/partitions.py
+-rw-r--r--   0        0        0     2316 2024-05-02 13:57:34.874294 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/props/__init__.py
+-rw-r--r--   0        0        0     1361 2024-02-07 02:47:09.521468 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/props/utils.py
+-rw-r--r--   0        0        0     2992 2024-02-07 03:12:22.731907 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/versions.py
+-rw-r--r--   0        0        0      132 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/vintf/__init__.py
+-rw-r--r--   0        0        0     1924 2024-02-07 03:15:32.548731 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/vintf/aidl.py
+-rw-r--r--   0        0        0      451 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/vintf/common.py
+-rw-r--r--   0        0        0     4508 2024-02-10 02:42:10.410105 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/vintf/hidl.py
+-rw-r--r--   0        0        0     2382 2024-02-07 03:10:14.118651 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/vintf/manifest.py
+-rw-r--r--   0        0        0      154 2024-05-02 13:57:13.277438 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libcompat/__init__.py
+-rw-r--r--   0        0        0      168 2024-05-02 13:57:05.577376 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libcompat/distutils/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-02 13:56:41.103859 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libcompat/distutils/util.py
+-rw-r--r--   0        0        0      395 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libexception/__init__.py
+-rw-r--r--   0        0        0      131 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/__init__.py
+-rw-r--r--   0        0        0     1260 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/account.py
+-rw-r--r--   0        0        0     4151 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/contents.py
+-rw-r--r--   0        0        0     2959 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/raw_api/__init__.py
+-rw-r--r--   0        0        0     1344 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/raw_api/rest.py
+-rw-r--r--   0        0        0      437 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/session.py
+-rw-r--r--   0        0        0     2553 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/utils.py
+-rw-r--r--   0        0        0      187 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/liblocale/__init__.py
+-rw-r--r--   0        0        0      517 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/liblogging/__init__.py
+-rw-r--r--   0        0        0      443 2024-02-07 03:20:02.006003 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libnekobin/__init__.py
+-rw-r--r--   0        0        0      323 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libpath/__init__.py
+-rw-r--r--   0        0        0     1755 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libreorder/__init__.py
+-rw-r--r--   0        0        0      435 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libsed/__init__.py
+-rw-r--r--   0        0        0      436 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libstring/__init__.py
+-rw-r--r--   0        0        0      301 2023-12-30 22:26:10.671296 sebaubuntu_libs-1.4.3/sebaubuntu_libs/libtyping/__init__.py
+-rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 sebaubuntu_libs-1.4.3/PKG-INFO
```

### Comparing `sebaubuntu_libs-1.4.2/README.md` & `sebaubuntu_libs-1.4.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # sebaubuntu_libs
 
 [![PyPI version](https://img.shields.io/pypi/v/sebaubuntu_libs)](https://pypi.org/project/sebaubuntu_libs/)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/8c14dd62f48043fdadbc5a31361310f5)](https://www.codacy.com/gh/sebaubuntu-python/sebaubuntu_libs/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=sebaubuntu-python/sebaubuntu_libs&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/8c14dd62f48043fdadbc5a31361310f5)](https://app.codacy.com/gh/sebaubuntu-python/sebaubuntu_libs/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Documentation Status](https://readthedocs.org/projects/sebaubuntu_libs/badge/?version=latest)](https://sebaubuntu_libs.readthedocs.io/en/latest/?badge=latest)
 
 A collection of code shared between my projects
 
 ## Installation
 
 ```sh
```

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libaik/__init__.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libaik/__init__.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/device_info.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/device_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #
 # Copyright (C) 2022 Sebastiano Barezzi
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
-from distutils.util import strtobool
 from enum import Enum
 from typing import Any, Callable, List
 
 from sebaubuntu_libs.libandroid.props import BuildProp
 from sebaubuntu_libs.libandroid.props.utils import fingerprint_to_description, get_partition_props
+from sebaubuntu_libs.libcompat.distutils.util import strtobool
 
 def get_product_props(value: str):
 	return get_partition_props("ro.product.{}" + value, add_empty=True)
 
 DEVICE_CODENAME = get_product_props("device")
 DEVICE_MANUFACTURER = get_product_props("manufacturer")
 DEVICE_BRAND = get_product_props("brand")
```

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/elf/elf.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/elf/elf.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/elf/shared_library.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/elf/shared_library.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/fstab/__init__.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/fstab/__init__.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/partitions/partition.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/partitions/partition.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/partitions/partition_model.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/partitions/partition_model.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/partitions/partitions.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/partitions/partitions.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/props/__init__.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/props/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # Copyright (C) 2022 Sebastiano Barezzi
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 """Android build prop library."""
 
 from __future__ import annotations
-from distutils.util import strtobool
 from pathlib import Path
 from typing import Any, Callable, List, Optional, Union
 
+from sebaubuntu_libs.libcompat.distutils.util import strtobool
+
 class BuildProp(dict):
 	"""
 	A class representing a build prop.
 	This class basically mimics Android props system, with both getprop and setprop commands
 	"""
 	@classmethod
 	def from_file(cls, file: Path):
```

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/props/utils.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/props/utils.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/versions.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/versions.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/vintf/aidl.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/vintf/aidl.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/vintf/hidl.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/vintf/hidl.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libandroid/vintf/manifest.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libandroid/vintf/manifest.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/account.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/account.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/contents.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/contents.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/raw_api/__init__.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/raw_api/__init__.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/raw_api/rest.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/raw_api/rest.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libgofile/utils.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libgofile/utils.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/liblogging/__init__.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/liblogging/__init__.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/sebaubuntu_libs/libreorder/__init__.py` & `sebaubuntu_libs-1.4.3/sebaubuntu_libs/libreorder/__init__.py`

 * *Files identical despite different names*

### Comparing `sebaubuntu_libs-1.4.2/PKG-INFO` & `sebaubuntu_libs-1.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sebaubuntu_libs
-Version: 1.4.2
+Version: 1.4.3
 Summary: SebaUbuntu's shared libs
 Home-page: https://github.com/sebaubuntu-python/sebaubuntu_libs
 License: Apache-2.0
 Author: Sebastiano Barezzi
 Author-email: barezzisebastiano@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,25 +12,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
-Requires-Dist: pyelftools (>=0.29,<0.31)
+Requires-Dist: pyelftools (>=0.29,<0.32)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sphinx (>=5.0.1,<8.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1,<3) ; extra == "docs"
 Project-URL: Repository, https://github.com/sebaubuntu-python/sebaubuntu_libs
 Description-Content-Type: text/markdown
 
 # sebaubuntu_libs
 
 [![PyPI version](https://img.shields.io/pypi/v/sebaubuntu_libs)](https://pypi.org/project/sebaubuntu_libs/)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/8c14dd62f48043fdadbc5a31361310f5)](https://www.codacy.com/gh/sebaubuntu-python/sebaubuntu_libs/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=sebaubuntu-python/sebaubuntu_libs&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/8c14dd62f48043fdadbc5a31361310f5)](https://app.codacy.com/gh/sebaubuntu-python/sebaubuntu_libs/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Documentation Status](https://readthedocs.org/projects/sebaubuntu_libs/badge/?version=latest)](https://sebaubuntu_libs.readthedocs.io/en/latest/?badge=latest)
 
 A collection of code shared between my projects
 
 ## Installation
 
 ```sh
```

