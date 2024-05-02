# Comparing `tmp/pyshared-1.5.7-py3-none-any.whl.zip` & `tmp/pyshared-1.5.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 12623 bytes, number of entries: 16
--rw-r--r--  2.0 unx      921 b- defN 24-Apr-30 16:46 pyshared/__init__.py
+Zip file size: 12547 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      759 b- defN 24-May-02 17:09 pyshared/__init__.py
 -rw-r--r--  2.0 unx      124 b- defN 24-Jan-11 01:53 pyshared/consts.py
 -rw-r--r--  2.0 unx     1293 b- defN 24-Jan-12 03:28 pyshared/crypto.py
 -rw-r--r--  2.0 unx     2029 b- defN 24-Apr-03 16:31 pyshared/env.py
 -rw-r--r--  2.0 unx      943 b- defN 24-Mar-31 21:02 pyshared/exceptions.py
 -rw-r--r--  2.0 unx      936 b- defN 24-Apr-12 00:40 pyshared/pytest.py
 -rw-r--r--  2.0 unx     5650 b- defN 24-Apr-21 08:20 pyshared/python.py
 -rw-r--r--  2.0 unx      790 b- defN 24-Jan-11 05:57 pyshared/shell.py
 -rw-r--r--  2.0 unx     2083 b- defN 24-Jan-12 03:45 pyshared/terminal.py
 -rw-r--r--  2.0 unx     2792 b- defN 24-Apr-18 06:32 pyshared/test.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-30 16:44 pyshared/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-30 16:46 pyshared-1.5.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     6929 b- defN 24-Apr-30 16:46 pyshared-1.5.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 16:46 pyshared-1.5.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-30 16:46 pyshared-1.5.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1211 b- defN 24-Apr-30 16:46 pyshared-1.5.7.dist-info/RECORD
-16 files, 26892 bytes uncompressed, 10655 bytes compressed:  60.4%
+-rw-r--r--  2.0 unx       22 b- defN 24-May-02 17:09 pyshared/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-02 17:09 pyshared-1.5.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6929 b- defN 24-May-02 17:09 pyshared-1.5.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 17:09 pyshared-1.5.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-02 17:09 pyshared-1.5.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1211 b- defN 24-May-02 17:09 pyshared-1.5.8.dist-info/RECORD
+16 files, 26730 bytes uncompressed, 10579 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: pyshared/test.py
 Comment: 
 
 Filename: pyshared/version.py
 Comment: 
 
-Filename: pyshared-1.5.7.dist-info/LICENSE
+Filename: pyshared-1.5.8.dist-info/LICENSE
 Comment: 
 
-Filename: pyshared-1.5.7.dist-info/METADATA
+Filename: pyshared-1.5.8.dist-info/METADATA
 Comment: 
 
-Filename: pyshared-1.5.7.dist-info/WHEEL
+Filename: pyshared-1.5.8.dist-info/WHEEL
 Comment: 
 
-Filename: pyshared-1.5.7.dist-info/top_level.txt
+Filename: pyshared-1.5.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pyshared-1.5.7.dist-info/RECORD
+Filename: pyshared-1.5.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyshared/__init__.py

```diff
@@ -27,12 +27,7 @@
 from .crypto import is_jwt
 from .env import typed_evar
 from .exceptions import NotPrintableError
 from .python import default_repr, ranstr, safe_repr, truncstr, tmp_pythonpath
 from .shell import runcmd
 from .terminal import get_terminal_width, print_columns, print_middle
 from .test import RanData
-
-try:
-    from .pytest import multiscope_fixture
-except (ImportError, ModuleNotFoundError):
-    print("pytest not installed, skipping multiscope_fixture import")
```

## pyshared/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.5.7'
+__version__ = '1.5.8'
```

## Comparing `pyshared-1.5.7.dist-info/LICENSE` & `pyshared-1.5.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyshared-1.5.7.dist-info/METADATA` & `pyshared-1.5.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshared
-Version: 1.5.7
+Version: 1.5.8
 Summary: A Python library containing common utility functions for use across multiple codebases, filling gaps not covered by the standard Python libraries.
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Cary Carter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `pyshared-1.5.7.dist-info/RECORD` & `pyshared-1.5.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-pyshared/__init__.py,sha256=AQ6jfkVz0ti59hIna15DhjdCTN6quoEuCVzDJDXedj4,921
+pyshared/__init__.py,sha256=cmZKKnA-UShXuIcBToW-zwVTlUOLQZFgBKRaU_8-ekQ,759
 pyshared/consts.py,sha256=vfUhhaxsFGp-DnTP_iJ-ZFT_w_be6frq9VabkLzejuA,124
 pyshared/crypto.py,sha256=Ww3uT2xa7g0ewgZzvJthJQ_BRPeHM0sLZPc5c3tad2E,1293
 pyshared/env.py,sha256=sJM9SVUIKVq9n7ugpC81zRhvAlNPur_Q8qUiCasglXQ,2029
 pyshared/exceptions.py,sha256=j7alpB6QyzZcCt9quCWPIKXmSsUw7dZPvs7fdqbYbO4,943
 pyshared/pytest.py,sha256=3coYUTNfSHB7-pQIPlIOWwOjbtjgBoX5uEc90DfH188,936
 pyshared/python.py,sha256=k8rBcjZpMYDmvwBydM7AGHwhYIBHLlYeF5RL4TulWRk,5650
 pyshared/shell.py,sha256=F2EJdaImnnlxeiONPlzdXcE_JZ1HUAdBWR5_i-WLfSA,790
 pyshared/terminal.py,sha256=6BjoRuUoqU7iKuXhEqU091aOiQWJUcVWXTMeUlNE3MA,2083
 pyshared/test.py,sha256=Ta4nNuYckDAtay4mltFCrXSHicQyuQvwGrkM0ypvPHQ,2792
-pyshared/version.py,sha256=1EQtBGa2dlHmCdA46_Q8GSrMI6pq3EXQ8KTx-m_h-LY,22
-pyshared-1.5.7.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
-pyshared-1.5.7.dist-info/METADATA,sha256=P5Fs-mGBtVTpri5G1xxaI_ZZpIN0PCctSrdgnk0TuRw,6929
-pyshared-1.5.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyshared-1.5.7.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
-pyshared-1.5.7.dist-info/RECORD,,
+pyshared/version.py,sha256=3cQJSv3T_SakRn0lVbTbIfYChgmmC7jm8CAfs40aiic,22
+pyshared-1.5.8.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
+pyshared-1.5.8.dist-info/METADATA,sha256=gKoHGrLyVBahTc-QAjCWtLwSHz_-_D1pn_2z0KD-KCM,6929
+pyshared-1.5.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyshared-1.5.8.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
+pyshared-1.5.8.dist-info/RECORD,,
```

