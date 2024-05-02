# Comparing `tmp/mira_omf-3.2.0rc1.tar.gz` & `tmp/mira_omf-3.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mira_omf-3.2.0rc1.tar", max compression
+gzip compressed data, was "mira_omf-3.2.0rc2.tar", max compression
```

## Comparing `mira_omf-3.2.0rc1.tar` & `mira_omf-3.2.0rc2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1122 2024-04-23 21:18:33.429696 mira_omf-3.2.0rc1/LICENSE
--rw-r--r--   0        0        0     1684 2024-04-27 21:37:48.543607 mira_omf-3.2.0rc1/omf/__init__.py
--rw-r--r--   0        0        0     6754 2024-04-23 21:18:33.550153 mira_omf-3.2.0rc1/omf/base.py
--rw-r--r--   0        0        0     8561 2024-04-23 21:18:33.550153 mira_omf-3.2.0rc1/omf/data.py
--rw-r--r--   0        0        0      111 2024-04-23 21:18:33.551152 mira_omf-3.2.0rc1/omf/fileio/__init__.py
--rw-r--r--   0        0        0     6049 2024-04-23 21:18:33.551152 mira_omf-3.2.0rc1/omf/fileio/fileio.py
--rw-r--r--   0        0        0    43690 2024-04-23 21:18:33.552162 mira_omf-3.2.0rc1/omf/fileio/geoh5.py
--rw-r--r--   0        0        0     1123 2024-04-23 21:18:33.552162 mira_omf-3.2.0rc1/omf/fileio/utils.py
--rw-r--r--   0        0        0     1760 2024-04-23 21:18:33.553151 mira_omf-3.2.0rc1/omf/lineset.py
--rw-r--r--   0        0        0     1411 2024-04-23 21:18:33.553151 mira_omf-3.2.0rc1/omf/pointset.py
--rw-r--r--   0        0        0        0 2024-04-23 21:18:33.553151 mira_omf-3.2.0rc1/omf/scripts/__init__.py
--rw-r--r--   0        0        0     1221 2024-04-23 21:18:33.554151 mira_omf-3.2.0rc1/omf/scripts/geoh5_to_omf.py
--rw-r--r--   0        0        0     1729 2024-04-23 21:18:33.554151 mira_omf-3.2.0rc1/omf/scripts/omf_to_geoh5.py
--rw-r--r--   0        0        0     3682 2024-04-23 21:18:33.554151 mira_omf-3.2.0rc1/omf/serializers.py
--rw-r--r--   0        0        0     3736 2024-04-23 21:18:33.555150 mira_omf-3.2.0rc1/omf/surface.py
--rw-r--r--   0        0        0      675 2024-04-23 21:18:33.555150 mira_omf-3.2.0rc1/omf/texture.py
--rw-r--r--   0        0        0     2409 2024-04-23 21:18:33.555150 mira_omf-3.2.0rc1/omf/volume.py
--rw-r--r--   0        0        0     2255 2024-04-27 21:37:54.011682 mira_omf-3.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2467 2024-04-27 21:36:29.725597 mira_omf-3.2.0rc1/README.rst
--rw-r--r--   0        0        0     3673 1970-01-01 00:00:00.000000 mira_omf-3.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1122 2024-04-23 21:18:33.429696 mira_omf-3.2.0rc2/LICENSE
+-rw-r--r--   0        0        0     1684 2024-05-02 20:13:02.910648 mira_omf-3.2.0rc2/omf/__init__.py
+-rw-r--r--   0        0        0     6756 2024-04-27 23:07:13.495353 mira_omf-3.2.0rc2/omf/base.py
+-rw-r--r--   0        0        0     8561 2024-04-23 21:18:33.550153 mira_omf-3.2.0rc2/omf/data.py
+-rw-r--r--   0        0        0      111 2024-04-29 03:17:19.916176 mira_omf-3.2.0rc2/omf/fileio/__init__.py
+-rw-r--r--   0        0        0     6049 2024-04-23 21:18:33.551152 mira_omf-3.2.0rc2/omf/fileio/fileio.py
+-rw-r--r--   0        0        0    43718 2024-04-27 23:29:12.042916 mira_omf-3.2.0rc2/omf/fileio/geoh5.py
+-rw-r--r--   0        0        0     1123 2024-04-23 21:18:33.552162 mira_omf-3.2.0rc2/omf/fileio/utils.py
+-rw-r--r--   0        0        0     1760 2024-04-23 21:18:33.553151 mira_omf-3.2.0rc2/omf/lineset.py
+-rw-r--r--   0        0        0     1411 2024-04-23 21:18:33.553151 mira_omf-3.2.0rc2/omf/pointset.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:18:33.553151 mira_omf-3.2.0rc2/omf/scripts/__init__.py
+-rw-r--r--   0        0        0     1221 2024-04-23 21:18:33.554151 mira_omf-3.2.0rc2/omf/scripts/geoh5_to_omf.py
+-rw-r--r--   0        0        0     1729 2024-04-23 21:18:33.554151 mira_omf-3.2.0rc2/omf/scripts/omf_to_geoh5.py
+-rw-r--r--   0        0        0     3557 2024-04-27 23:28:28.346635 mira_omf-3.2.0rc2/omf/serializers.py
+-rw-r--r--   0        0        0     3736 2024-04-23 21:18:33.555150 mira_omf-3.2.0rc2/omf/surface.py
+-rw-r--r--   0        0        0      675 2024-04-23 21:18:33.555150 mira_omf-3.2.0rc2/omf/texture.py
+-rw-r--r--   0        0        0     2409 2024-04-23 21:18:33.555150 mira_omf-3.2.0rc2/omf/volume.py
+-rw-r--r--   0        0        0     2503 2024-05-02 20:13:02.916643 mira_omf-3.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4108 2024-05-02 04:12:41.741367 mira_omf-3.2.0rc2/README.rst
+-rw-r--r--   0        0        0      929 2024-05-02 04:12:41.741367 mira_omf-3.2.0rc2/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     5406 1970-01-01 00:00:00.000000 mira_omf-3.2.0rc2/PKG-INFO
```

### Comparing `mira_omf-3.2.0rc1/LICENSE` & `mira_omf-3.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/omf/__init__.py` & `mira_omf-3.2.0rc2/omf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from .fileio import GeoH5Writer, OMFReader, OMFWriter
 from .lineset import LineSetElement, LineSetGeometry
 from .pointset import PointSetElement, PointSetGeometry
 from .surface import SurfaceElement, SurfaceGeometry, SurfaceGridGeometry
 from .texture import ImageTexture
 from .volume import VolumeElement, VolumeGridGeometry
 
-__version__ = "3.2.0-rc.1"
+__version__ = "3.2.0-rc.2"
 __author__ = "Global Mining Standards and Guidelines Group"
 __license__ = "MIT License"
 __copyright__ = "Copyright 2017 Global Mining Standards and Guidelines Group"
 
 
 def _create_logger():
     error_handler = logging.StreamHandler(sys.stderr)
```

### Comparing `mira_omf-3.2.0rc1/omf/base.py` & `mira_omf-3.2.0rc2/omf/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """base.py: OMF Project and base classes for its components"""
+
 from __future__ import annotations
 
 import datetime
 
 import properties
```

### Comparing `mira_omf-3.2.0rc1/omf/data.py` & `mira_omf-3.2.0rc2/omf/data.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/omf/fileio/fileio.py` & `mira_omf-3.2.0rc2/omf/fileio/fileio.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/omf/fileio/geoh5.py` & `mira_omf-3.2.0rc2/omf/fileio/geoh5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # pylint: disable=too-many-lines
 
 from __future__ import annotations
 
 import inspect
 import logging
 from abc import ABC, abstractmethod
+from collections.abc import Generator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Generator
+from typing import Any
 
 import numpy as np
 from geoh5py.data import Data, FloatData, IntegerData, ReferencedData
 from geoh5py.groups import PropertyGroup, RootGroup
 from geoh5py.objects import BlockModel, Curve, Grid2D, ObjectBase, Points, Surface
 from geoh5py.shared import FLOAT_NDV, INTEGER_NDV, Entity
 from geoh5py.workspace import Workspace
```

### Comparing `mira_omf-3.2.0rc1/omf/fileio/utils.py` & `mira_omf-3.2.0rc2/omf/fileio/utils.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/omf/lineset.py` & `mira_omf-3.2.0rc2/omf/lineset.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/omf/pointset.py` & `mira_omf-3.2.0rc2/omf/pointset.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/omf/scripts/geoh5_to_omf.py` & `mira_omf-3.2.0rc2/omf/scripts/geoh5_to_omf.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/omf/scripts/omf_to_geoh5.py` & `mira_omf-3.2.0rc2/omf/scripts/omf_to_geoh5.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/omf/serializers.py` & `mira_omf-3.2.0rc2/omf/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 
 import zlib
 from io import BytesIO
 
 import numpy as np
 from six import PY2
 
-if PY2:
-    memoryview = (
-        buffer  # pylint: disable=redefined-builtin, invalid-name, undefined-variable
-    )
-
 
 def array_serializer(arr, open_file, **kwargs):  # pylint: disable=unused-argument
     """Convert array data to a serialized binary format"""
     if arr is None:
         return None
     if open_file.mode != "wb":
         raise ValueError("file mode must be wb")
```

### Comparing `mira_omf-3.2.0rc1/omf/surface.py` & `mira_omf-3.2.0rc2/omf/surface.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/omf/texture.py` & `mira_omf-3.2.0rc2/omf/texture.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/omf/volume.py` & `mira_omf-3.2.0rc2/omf/volume.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.2.0rc1/pyproject.toml` & `mira_omf-3.2.0rc2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tool.poetry]
 name = "mira-omf"
-version = "3.2.0-rc.1"
+version = "3.2.0-rc.2"
 description = "API Library for Open Mining Format"
+license = "MIT"
 authors = [
-    "Mira Geoscience <dominiquef@mirageoscience.com>",
-    "Global Mining Standards and Guidelines Group <it@seequent.com>",
+    "Mira Geoscience <support@mirageoscience.com>",
+    "Global Mining Guidelines Group <info@gmggroup.org>",
 ]
+maintainers = ["Dominique Fournier <dominiquef@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/omf"
-homepage = "http://www.globalminingstandards.org/"
+#documentation  = "https://mirageoscience-omf.readthedocs-hosted.com/"
+homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
+
 readme = "README.rst"
 keywords = ["geology", "geophysics", "earth sciences"]
 classifiers = [
     'Development Status :: 4 - Beta',
     'Programming Language :: Python',
     'Topic :: Scientific/Engineering',
     'Topic :: Scientific/Engineering :: Mathematics',
@@ -36,15 +40,15 @@
 ]
 
 [tool.poetry.scripts]
 geoh5_to_omf = 'omf.scripts.geoh5_to_omf:main'
 omf_to_geoh5 = 'omf.scripts.omf_to_geoh5:main'
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.11"
+python = "^3.9,<3.11"
 
 numpy = "~1.23.5"  # also in geoh5py
 properties = "~0.6.0"
 pypng = "^0.20220715"
 six = "^1.16"
 vectormath = "~0.2.0"
 
@@ -60,20 +64,27 @@
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
 sphinx = "^5.3"
 tomli = "*"  # for tests only
 
 [tool.isort]
-# settings for compatibility between ``isort`` and ``black`` formatting
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-line_length = 88
+profile = "black"
 
 [tool.black]
 # defaults are just fine
 
+[tool.mypy]
+warn_unused_configs = true
+ignore_missing_imports = true
+scripts_are_modules = true
+show_error_context = true
+show_column_numbers = true
+check_untyped_defs = true
+
+plugins = [
+#    "numpy.typing.mypy_plugin"
+]
+
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mira_omf-3.2.0rc1/PKG-INFO` & `mira_omf-3.2.0rc2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: mira-omf
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: API Library for Open Mining Format
-Home-page: http://www.globalminingstandards.org/
+Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
+License: MIT
 Keywords: geology,geophysics,earth sciences
 Author: Mira Geoscience
-Author-email: dominiquef@mirageoscience.com
-Requires-Python: >=3.8,<3.11
+Author-email: support@mirageoscience.com
+Maintainer: Dominique Fournier
+Maintainer-email: dominiquef@mirageoscience.com
+Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
@@ -112,7 +115,43 @@
 
 .. code:: bash
 
     git clone https://github.com/GMSGDataExchange/omf.git
     cd omf
     pip install -e .
 
+
+License
+^^^^^^^
+MIT License
+
+Copyright (c) 2024 Mira Geoscience
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+Third Party Software
+^^^^^^^^^^^^^^^^^^^^
+The mira-omf Software may provide links to third party libraries or code (collectively “Third Party Software”)
+to implement various functions. Third Party Software does not comprise part of the Software.
+The use of Third Party Software is governed by the terms of such software license(s).
+Third Party Software notices and/or additional terms and conditions are located in the
+`THIRD_PARTY_SOFTWARE.rst`_ file.
+
+.. _THIRD_PARTY_SOFTWARE.rst: THIRD_PARTY_SOFTWARE.rst
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

