# Comparing `tmp/ratio_delta-1.0.0.tar.gz` & `tmp/ratio_delta-1.0.1.tar.gz`

## Comparing `ratio_delta-1.0.0.tar` & `ratio_delta-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 ratio_delta-1.0.0/src/ratio_delta/__init__.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ratio_delta-1.0.0/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 ratio_delta-1.0.0/COPYING.LESSER
--rw-r--r--   0        0        0    13711 2020-02-02 00:00:00.000000 ratio_delta-1.0.0/README.md
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 ratio_delta-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    23664 2020-02-02 00:00:00.000000 ratio_delta-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    14448 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/README_printable.md
+-rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/src/ratio_delta/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/COPYING.LESSER
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/README.md
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    24610 2020-02-02 00:00:00.000000 ratio_delta-1.0.1/PKG-INFO
```

### Comparing `ratio_delta-1.0.0/src/ratio_delta/__init__.py` & `ratio_delta-1.0.1/src/ratio_delta/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """
 This file is part of RatioDelta library.
 
-RatioDelta is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-RatioDelta is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
-
-You should have received a copy of the GNU Lesser General Public License
-along with RatioDelta.    If not, see <http://www.gnu.org/licenses/>.
+RatioDelta is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
+
+RatioDelta is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
+
+You should have received a copy of
+the GNU Lesser General Public License
+along with RatioDelta.
+If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
 """
 
 from typing import Optional
 
 
@@ -25,194 +31,210 @@
     b: float,
     c: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return a / b + c
 
 
 def fused_divide_subtract(
     a: float,
     b: float,
     c: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return a / b - c
 
 
 def fused_absolute_divide_add(
     a: float,
     b: float,
     c: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return abs(a / b + c)
 
 
 def fused_absolute_divide_subtract(
     a: float,
     b: float,
     c: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return abs(a / b - c)
 
 
 def scaled_fused_divide_add(
     a: float,
     b: float,
     c: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return (a / b + c) * scale
 
 
 def scaled_fused_divide_subtract(
     a: float,
     b: float,
     c: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return (a / b - c) * scale
 
 
 def scaled_fused_absolute_divide_add(
     a: float,
     b: float,
     c: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return abs(a / b + c) * scale
 
 
 def scaled_fused_absolute_divide_subtract(
     a: float,
     b: float,
     c: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return abs(a / b - c) * scale
 
 
 def fused_divide_increment(
     a: float,
     b: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return a / b + 1
 
 
 def fused_divide_decrement(
     a: float,
     b: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return a / b - 1
 
 
 def fused_absolute_divide_increment(
     a: float,
     b: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return abs(a / b + 1)
 
 
 def fused_absolute_divide_decrement(
     a: float,
     b: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return abs(a / b - 1)
 
 
 def scaled_fused_divide_increment(
     a: float,
     b: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return (a / b + 1) * scale
 
 
 def scaled_fused_divide_decrement(
     a: float,
     b: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return (a / b - 1) * scale
 
 
 def scaled_fused_absolute_divide_increment(
     a: float,
     b: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return abs(a / b + 1) * scale
 
 
 def scaled_fused_absolute_divide_decrement(
     a: float,
     b: float,
     scale: float,
 ) -> float:
     """
     It should be inlined.
     Maybe one day it will be a single assembly operation.
     """
+
     return abs(a / b - 1) * scale
 
 
 # pylint: disable-next=too-many-arguments,too-many-return-statements
 def ratio_iota(
     a: Optional[float],
     b: Optional[float],
@@ -223,14 +245,15 @@
     a_null: Optional[float] = None,
     b_null: Optional[float] = None,
     b_zero: Optional[float] = None,
 ) -> Optional[float]:
     """
     Divide and increment, and more if affinity.
     """
+
     if a is None:
         if b is None:
             return both_null
         return a_null
     if b is None:
         return b_null
     if b == 0:
@@ -255,14 +278,15 @@
     a_null: Optional[float] = None,
     b_null: Optional[float] = None,
     b_zero: Optional[float] = None,
 ) -> Optional[float]:
     """
     Divide and decrement, and more if affinity.
     """
+
     if a is None:
         if b is None:
             return both_null
         return a_null
     if b is None:
         return b_null
     if b == 0:
@@ -292,14 +316,15 @@
     b_null: Optional[float] = None,
     c_null: Optional[float] = None,
     b_zero: Optional[float] = None,
 ) -> Optional[float]:
     """
     Divide and add, and more if affinity.
     """
+
     if a is None:
         if b is None:
             if c is None:
                 return all_null
             return a_b_null
         if c is None:
             return a_c_null
@@ -337,14 +362,15 @@
     b_null: Optional[float] = None,
     c_null: Optional[float] = None,
     b_zero: Optional[float] = None,
 ) -> Optional[float]:
     """
     Divide and subtract, and more if affinity.
     """
+
     if a is None:
         if b is None:
             if c is None:
                 return all_null
             return a_b_null
         if c is None:
             return a_c_null
```

### Comparing `ratio_delta-1.0.0/COPYING` & `ratio_delta-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `ratio_delta-1.0.0/COPYING.LESSER` & `ratio_delta-1.0.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `ratio_delta-1.0.0/README.md` & `ratio_delta-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # RatioDelta
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ratio-delta)
-[![pypi-version](https://img.shields.io/pypi/v/ratio-delta.svg)](https://pypi.org/project/ratio-delta/)
-[![Downloads](https://img.shields.io/pypi/dm/ratio-delta)](https://pypistats.org/packages/ratio-delta)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
-[![CodeFactor](https://www.codefactor.io/repository/github/llyaudet/RatioDelta/badge/main)](https://www.codefactor.io/repository/github/llyaudet/RatioDelta/overview/main)
-[![CodeClimateMaintainability](https://api.codeclimate.com/v1/badges/23218bfc6b7b7dd5c2aa/maintainability)](https://codeclimate.com/github/LLyaudet/RatioDelta/maintainability)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/d4c03e8e52194c1fb3fb51bb58c4f54c)](https://app.codacy.com/gh/LLyaudet/RatioDelta/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-![GitHub top language](https://img.shields.io/github/languages/top/llyaudet/RatioDelta)
-![GitHub License](https://img.shields.io/github/license/llyaudet/RatioDelta)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/llyaudet/RatioDelta)
-[![GitHub Sponsors](https://img.shields.io/github/sponsors/LLyaudet)](https://github.com/sponsors/LLyaudet)
+[![PyPI-version-badge]][PyPI-package-page]
+[![Downloads-badge]][PyPIStats-package-page]
+[![Code-style:black:badge]][Black-GitHub.com]
+[![Imports:isort:badge]][Isort-GitHub.io]
+[![Typecheck:mypy:badge]][Typecheck-mypy-lang.org]
+[![Linting:pylint:badge]][Pylint-GitHub.com]
+[![CodeFactor-badge]][CodeFactor-package-page]
+[![CodeClimateMaintainability-badge]][CodeClimateM13y-package-page]
+[![Codacy-badge]][Codacy-package-page]
+![GitHub-top-language-badge]
+![GitHub-license-badge]
+![PyPI-python-version-badge]
+![GitHub-code-size-in-bytes-badge]
 
 |     **An unknown? but somewhat common arithmetic operation**     |
 
 In accounting, it is common to compute (a/b - 1),
 or (a/b - 1) * 100 if you want percents.
 Following Knuth's advice "Name and conquer",
 we give the name ratio-delta to the binary operation a/b - 1.
@@ -213,14 +212,15 @@
 $$ LANGUAGE SQL;
 ```
 
 This detour from accounting to relative error via a new name
 was the opportunity to give you SQL functions for it,
 and see that no major database has a function
 for (signed) relative error:
+
 - <https://www.postgresql.org/docs/current/functions-math.html>
 - <https://mariadb.com/kb/en/numeric-functions/>
 - <https://dev.mysql.com/doc/refman/8.0/en/numeric-functions.html>
 - <https://docs.oracle.com/cd/E49933_01/server.770/es_eql/src/ceql_functions_numeric.html>
 - <https://learn.microsoft.com/en-us/sql/odbc/reference/appendixes/numeric-functions?view=sql-server-ver16>
 
 There also does not seem to have any CPU architecture
@@ -297,19 +297,21 @@
 by using "increment" when the second operand is 1
 and "add" when the second operand is variable.
 I'm not the first to use this trick,
 and will probably not be the last ;).
 
 For hardware, the topic of ratio-alpha and ratio-sigma
 has been addressed in academic papers on fused divide-add:
+
 - <https://ieeexplore.ieee.org/abstract/document/5451057>
 - <https://ieeexplore.ieee.org/document/5349981>
 - <https://ieeexplore.ieee.org/abstract/document/7280029>
 
 It was already envisionned in 1994:
+
 - <https://www.researchgate.net/profile/Michael-Flynn-7/publication/3043776_Design_issues_in_division_and_other_floating-point_operations/links/5467be1a0cf2f5eb18036e1e/Design-issues-in-division-and-other-floating-point-operations.pdf>
 
 But we could not check if someone linked explicitely
 relative error with fused divide-add.
 (A paper about fused divide-add/subtract can talk about relative error
 as a tool to analyze the fused divide-add/subtract method,
 without noting that the relative error can be computed
@@ -323,15 +325,16 @@
 
 With dedicated function in software,
 it may be easier to use dedicated hardware if it exists one day.
 
 ## Voltage divider, and beyond?
 
 If we look at ratio-iota (a/b) + 1,
-when you have a voltage divider (<https://en.wikipedia.org/wiki/Voltage_divider>)
+when you have a voltage divider
+(<https://en.wikipedia.org/wiki/Voltage_divider>)
 with two resistors,
 the coefficient applied to tension is (Z2/(Z1+Z2)) = 1 / (Z1/Z2 + 1).
 Thus, we could, but probably should not, add:
 
 - inverted... when you take the inverse of it.
 
 And the coefficient in a voltage divider
@@ -353,11 +356,54 @@
 with differential and operational amplifiers,
 see
 <https://www.electronique-et-informatique.fr/anglais/Amplificateur_differentiel.php>
 for example.
 
 ## Source code
 
-The source code is available for SQL, Python, and PHP currently.
+The source code is available for many languages.
 It is quite verbose and repetitive because we wanted to explicit
 what could be assembly operation in our point of view.
 
+[PyPI-python-version-badge]: https://img.shields.io/pypi/pyversions/ratio-delta
+
+[PyPI-version-badge]: https://img.shields.io/pypi/v/ratio-delta.svg
+
+[PyPI-package-page]: https://pypi.org/project/ratio-delta/
+
+[Downloads-badge]: https://img.shields.io/pypi/dm/ratio-delta
+
+[PyPIStats-package-page]: https://pypistats.org/packages/ratio-delta
+
+[Code-style:black:badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+
+[Black-GitHub.com]: https://github.com/psf/black
+
+[Imports:isort:badge]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+
+[Isort-GitHub.io]: https://pycqa.github.io/isort/
+
+[Typecheck:mypy:badge]: https://www.mypy-lang.org/static/mypy_badge.svg
+
+[Typecheck-mypy-lang.org]: https://mypy-lang.org/
+
+[Linting:pylint:badge]: https://img.shields.io/badge/linting-pylint-yellowgreen
+
+[Pylint-GitHub.com]: https://github.com/pylint-dev/pylint
+
+[CodeFactor-badge]: https://www.codefactor.io/repository/github/llyaudet/RatioDelta/badge/main
+
+[CodeFactor-package-page]: https://www.codefactor.io/repository/github/llyaudet/RatioDelta/overview/main
+
+[CodeClimateMaintainability-badge]: https://api.codeclimate.com/v1/badges/23218bfc6b7b7dd5c2aa/maintainability
+
+[CodeClimateM13y-package-page]: https://codeclimate.com/github/LLyaudet/RatioDelta/maintainability
+
+[Codacy-badge]: https://app.codacy.com/project/badge/Grade/d4c03e8e52194c1fb3fb51bb58c4f54c
+
+[Codacy-package-page]: https://app.codacy.com/gh/LLyaudet/RatioDelta/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+
+[GitHub-top-language-badge]: https://img.shields.io/github/languages/top/llyaudet/RatioDelta
+
+[GitHub-license-badge]: https://img.shields.io/github/license/llyaudet/RatioDelta
+
+[GitHub-code-size-in-bytes-badge]: https://img.shields.io/github/languages/code-size/llyaudet/RatioDelta
```

### Comparing `ratio_delta-1.0.0/pyproject.toml` & `ratio_delta-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,26 +2,38 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ratio-delta"
-version = "1.0.0"
-description = "Add functions for variants of a common arithmetic operation"
+version = "1.0.1"
+description = """\
+Add functions for variants of a common arithmetic operation\
+"""
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
+maintainers = [
+    { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
+]
 license = { file = "COPYING.LESSER" }
 classifiers = [
-    "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    """\
+License :: OSI Approved :: \
+GNU Lesser General Public License v3 or later (LGPLv3+)\
+""",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Typing :: Typed",
 ]
 keywords = [
     "Python",
     "fused-divide-add",
     "fused-divide-subract",
     "fused-divide-increment",
     "fused-divide-decrement",
@@ -47,8 +59,7 @@
 
 [tool.black]
 line-length = 70
 
 [tool.isort]
 profile = "black"
 line_length = 70
-
```

### Comparing `ratio_delta-1.0.0/PKG-INFO` & `ratio_delta-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.3
 Name: ratio-delta
-Version: 1.0.0
+Version: 1.0.1
 Summary: Add functions for variants of a common arithmetic operation
 Project-URL: Homepage, https://github.com/LLyaudet/RatioDelta
 Project-URL: Bug Tracker, https://github.com/LLyaudet/RatioDelta/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
+Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -169,42 +170,45 @@
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 License-File: COPYING
 License-File: COPYING.LESSER
 Keywords: Python,fused-divide-add,fused-divide-decrement,fused-divide-increment,fused-divide-subract,ratio-alpha,ratio-delta,ratio-iota,ratio-sigma
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Python: >=3.5
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # RatioDelta
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ratio-delta)
-[![pypi-version](https://img.shields.io/pypi/v/ratio-delta.svg)](https://pypi.org/project/ratio-delta/)
-[![Downloads](https://img.shields.io/pypi/dm/ratio-delta)](https://pypistats.org/packages/ratio-delta)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
-[![CodeFactor](https://www.codefactor.io/repository/github/llyaudet/RatioDelta/badge/main)](https://www.codefactor.io/repository/github/llyaudet/RatioDelta/overview/main)
-[![CodeClimateMaintainability](https://api.codeclimate.com/v1/badges/23218bfc6b7b7dd5c2aa/maintainability)](https://codeclimate.com/github/LLyaudet/RatioDelta/maintainability)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/d4c03e8e52194c1fb3fb51bb58c4f54c)](https://app.codacy.com/gh/LLyaudet/RatioDelta/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-![GitHub top language](https://img.shields.io/github/languages/top/llyaudet/RatioDelta)
-![GitHub License](https://img.shields.io/github/license/llyaudet/RatioDelta)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/llyaudet/RatioDelta)
-[![GitHub Sponsors](https://img.shields.io/github/sponsors/LLyaudet)](https://github.com/sponsors/LLyaudet)
+[![PyPI-version-badge]][PyPI-package-page]
+[![Downloads-badge]][PyPIStats-package-page]
+[![Code-style:black:badge]][Black-GitHub.com]
+[![Imports:isort:badge]][Isort-GitHub.io]
+[![Typecheck:mypy:badge]][Typecheck-mypy-lang.org]
+[![Linting:pylint:badge]][Pylint-GitHub.com]
+[![CodeFactor-badge]][CodeFactor-package-page]
+[![CodeClimateMaintainability-badge]][CodeClimateM13y-package-page]
+[![Codacy-badge]][Codacy-package-page]
+![GitHub-top-language-badge]
+![GitHub-license-badge]
+![PyPI-python-version-badge]
+![GitHub-code-size-in-bytes-badge]
 
 |     **An unknown? but somewhat common arithmetic operation**     |
 
 In accounting, it is common to compute (a/b - 1),
 or (a/b - 1) * 100 if you want percents.
 Following Knuth's advice "Name and conquer",
 we give the name ratio-delta to the binary operation a/b - 1.
@@ -400,14 +404,15 @@
 $$ LANGUAGE SQL;
 ```
 
 This detour from accounting to relative error via a new name
 was the opportunity to give you SQL functions for it,
 and see that no major database has a function
 for (signed) relative error:
+
 - <https://www.postgresql.org/docs/current/functions-math.html>
 - <https://mariadb.com/kb/en/numeric-functions/>
 - <https://dev.mysql.com/doc/refman/8.0/en/numeric-functions.html>
 - <https://docs.oracle.com/cd/E49933_01/server.770/es_eql/src/ceql_functions_numeric.html>
 - <https://learn.microsoft.com/en-us/sql/odbc/reference/appendixes/numeric-functions?view=sql-server-ver16>
 
 There also does not seem to have any CPU architecture
@@ -484,19 +489,21 @@
 by using "increment" when the second operand is 1
 and "add" when the second operand is variable.
 I'm not the first to use this trick,
 and will probably not be the last ;).
 
 For hardware, the topic of ratio-alpha and ratio-sigma
 has been addressed in academic papers on fused divide-add:
+
 - <https://ieeexplore.ieee.org/abstract/document/5451057>
 - <https://ieeexplore.ieee.org/document/5349981>
 - <https://ieeexplore.ieee.org/abstract/document/7280029>
 
 It was already envisionned in 1994:
+
 - <https://www.researchgate.net/profile/Michael-Flynn-7/publication/3043776_Design_issues_in_division_and_other_floating-point_operations/links/5467be1a0cf2f5eb18036e1e/Design-issues-in-division-and-other-floating-point-operations.pdf>
 
 But we could not check if someone linked explicitely
 relative error with fused divide-add.
 (A paper about fused divide-add/subtract can talk about relative error
 as a tool to analyze the fused divide-add/subtract method,
 without noting that the relative error can be computed
@@ -510,15 +517,16 @@
 
 With dedicated function in software,
 it may be easier to use dedicated hardware if it exists one day.
 
 ## Voltage divider, and beyond?
 
 If we look at ratio-iota (a/b) + 1,
-when you have a voltage divider (<https://en.wikipedia.org/wiki/Voltage_divider>)
+when you have a voltage divider
+(<https://en.wikipedia.org/wiki/Voltage_divider>)
 with two resistors,
 the coefficient applied to tension is (Z2/(Z1+Z2)) = 1 / (Z1/Z2 + 1).
 Thus, we could, but probably should not, add:
 
 - inverted... when you take the inverse of it.
 
 And the coefficient in a voltage divider
@@ -540,11 +548,54 @@
 with differential and operational amplifiers,
 see
 <https://www.electronique-et-informatique.fr/anglais/Amplificateur_differentiel.php>
 for example.
 
 ## Source code
 
-The source code is available for SQL, Python, and PHP currently.
+The source code is available for many languages.
 It is quite verbose and repetitive because we wanted to explicit
 what could be assembly operation in our point of view.
 
+[PyPI-python-version-badge]: https://img.shields.io/pypi/pyversions/ratio-delta
+
+[PyPI-version-badge]: https://img.shields.io/pypi/v/ratio-delta.svg
+
+[PyPI-package-page]: https://pypi.org/project/ratio-delta/
+
+[Downloads-badge]: https://img.shields.io/pypi/dm/ratio-delta
+
+[PyPIStats-package-page]: https://pypistats.org/packages/ratio-delta
+
+[Code-style:black:badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+
+[Black-GitHub.com]: https://github.com/psf/black
+
+[Imports:isort:badge]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+
+[Isort-GitHub.io]: https://pycqa.github.io/isort/
+
+[Typecheck:mypy:badge]: https://www.mypy-lang.org/static/mypy_badge.svg
+
+[Typecheck-mypy-lang.org]: https://mypy-lang.org/
+
+[Linting:pylint:badge]: https://img.shields.io/badge/linting-pylint-yellowgreen
+
+[Pylint-GitHub.com]: https://github.com/pylint-dev/pylint
+
+[CodeFactor-badge]: https://www.codefactor.io/repository/github/llyaudet/RatioDelta/badge/main
+
+[CodeFactor-package-page]: https://www.codefactor.io/repository/github/llyaudet/RatioDelta/overview/main
+
+[CodeClimateMaintainability-badge]: https://api.codeclimate.com/v1/badges/23218bfc6b7b7dd5c2aa/maintainability
+
+[CodeClimateM13y-package-page]: https://codeclimate.com/github/LLyaudet/RatioDelta/maintainability
+
+[Codacy-badge]: https://app.codacy.com/project/badge/Grade/d4c03e8e52194c1fb3fb51bb58c4f54c
+
+[Codacy-package-page]: https://app.codacy.com/gh/LLyaudet/RatioDelta/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+
+[GitHub-top-language-badge]: https://img.shields.io/github/languages/top/llyaudet/RatioDelta
+
+[GitHub-license-badge]: https://img.shields.io/github/license/llyaudet/RatioDelta
+
+[GitHub-code-size-in-bytes-badge]: https://img.shields.io/github/languages/code-size/llyaudet/RatioDelta
```

