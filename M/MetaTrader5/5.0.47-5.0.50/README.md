# Comparing `tmp/MetaTrader5-5.0.47-cp39-cp39-win_amd64.whl.zip` & `tmp/MetaTrader5-5.0.50-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 57338 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    17680 b- defN 24-Feb-02 17:50 MetaTrader5/__init__.py
--rw-rw-rw-  2.0 fat   140800 b- defN 24-Feb-02 17:50 MetaTrader5/_core.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1065 b- defN 24-Feb-02 17:50 MetaTrader5-5.0.47.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2386 b- defN 24-Feb-02 17:50 MetaTrader5-5.0.47.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Feb-02 17:50 MetaTrader5-5.0.47.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Feb-02 17:50 MetaTrader5-5.0.47.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      592 b- defN 24-Feb-02 17:50 MetaTrader5-5.0.47.dist-info/RECORD
-7 files, 162635 bytes uncompressed, 56290 bytes compressed:  65.4%
+Zip file size: 57339 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    17680 b- defN 24-Feb-02 18:04 MetaTrader5/__init__.py
+-rw-rw-rw-  2.0 fat   140800 b- defN 24-Feb-02 18:04 MetaTrader5/_core.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1065 b- defN 24-Feb-02 18:04 MetaTrader5-5.0.50.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2386 b- defN 24-Feb-02 18:04 MetaTrader5-5.0.50.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Feb-02 18:04 MetaTrader5-5.0.50.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Feb-02 18:04 MetaTrader5-5.0.50.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      592 b- defN 24-Feb-02 18:04 MetaTrader5-5.0.50.dist-info/RECORD
+7 files, 162635 bytes uncompressed, 56291 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: MetaTrader5/__init__.py
 Comment: 
 
 Filename: MetaTrader5/_core.cp39-win_amd64.pyd
 Comment: 
 
-Filename: MetaTrader5-5.0.47.dist-info/LICENSE.txt
+Filename: MetaTrader5-5.0.50.dist-info/LICENSE.txt
 Comment: 
 
-Filename: MetaTrader5-5.0.47.dist-info/METADATA
+Filename: MetaTrader5-5.0.50.dist-info/METADATA
 Comment: 
 
-Filename: MetaTrader5-5.0.47.dist-info/WHEEL
+Filename: MetaTrader5-5.0.50.dist-info/WHEEL
 Comment: 
 
-Filename: MetaTrader5-5.0.47.dist-info/top_level.txt
+Filename: MetaTrader5-5.0.50.dist-info/top_level.txt
 Comment: 
 
-Filename: MetaTrader5-5.0.47.dist-info/RECORD
+Filename: MetaTrader5-5.0.50.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## MetaTrader5/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '5.0.47'
+__version__ = '5.0.50'
 __author__  = 'MetaQuotes Ltd.'
 
 # timeframes
 TIMEFRAME_M1                        = 1
 TIMEFRAME_M2                        = 2
 TIMEFRAME_M3                        = 3
 TIMEFRAME_M4                        = 4
```

## Comparing `MetaTrader5-5.0.47.dist-info/LICENSE.txt` & `MetaTrader5-5.0.50.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `MetaTrader5-5.0.47.dist-info/METADATA` & `MetaTrader5-5.0.50.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetaTrader5
-Version: 5.0.47
+Version: 5.0.50
 Summary: API Connector to MetaTrader 5 Terminal
 Home-page: https://www.metatrader5.com
 Author: MetaQuotes Ltd.
 Author-email: plugins@metaquotes.net
 Maintainer: MetaQuotes Ltd.
 Maintainer-email: plugins@metaquotes.net
 License: MIT
```

## Comparing `MetaTrader5-5.0.47.dist-info/RECORD` & `MetaTrader5-5.0.50.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-MetaTrader5/__init__.py,sha256=xZhM4xAJq6ONq9RcvntK3ad7Znj7El-vKDxSIiDNEoo,17680
-MetaTrader5/_core.cp39-win_amd64.pyd,sha256=gB2ZoVPvltgbgAx6Q2ZNK1yU1d725AfI8gSXc34KveA,140800
-MetaTrader5-5.0.47.dist-info/LICENSE.txt,sha256=Uudx9j4rjki_WlFSLM-qMBT5cM8nYiTTr3xHnX93o6k,1065
-MetaTrader5-5.0.47.dist-info/METADATA,sha256=jUZceIM0wSmkB8L-7Fa3kYrTJMy--uCRhImU0QMsH_0,2386
-MetaTrader5-5.0.47.dist-info/WHEEL,sha256=GZFS91_ufm4WrNPBaFVPB9MvOXR6bMZQhPcZRRTN5YM,100
-MetaTrader5-5.0.47.dist-info/top_level.txt,sha256=FxZl8Gt0jwFY0ZY4D-Zyv9Y56ACVnOUOUDZbGZRyaWA,12
-MetaTrader5-5.0.47.dist-info/RECORD,,
+MetaTrader5/__init__.py,sha256=hl2uCXdozgeHjjYEqbLCms2rUbeh0ZIQwQJnazy71YU,17680
+MetaTrader5/_core.cp39-win_amd64.pyd,sha256=TDMBQTqF1XsQw0jMONt8aTle8l5ypVBJ_9GiSHxqYck,140800
+MetaTrader5-5.0.50.dist-info/LICENSE.txt,sha256=Uudx9j4rjki_WlFSLM-qMBT5cM8nYiTTr3xHnX93o6k,1065
+MetaTrader5-5.0.50.dist-info/METADATA,sha256=TJiYhSqb6A9emiTfqrU22CQSOi6OAI9rXg91c5AWi-w,2386
+MetaTrader5-5.0.50.dist-info/WHEEL,sha256=GZFS91_ufm4WrNPBaFVPB9MvOXR6bMZQhPcZRRTN5YM,100
+MetaTrader5-5.0.50.dist-info/top_level.txt,sha256=FxZl8Gt0jwFY0ZY4D-Zyv9Y56ACVnOUOUDZbGZRyaWA,12
+MetaTrader5-5.0.50.dist-info/RECORD,,
```

