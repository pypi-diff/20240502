# Comparing `tmp/komoutils-0.0.224.tar.gz` & `tmp/komoutils-0.0.225.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komoutils-0.0.224.tar", max compression
+gzip compressed data, was "komoutils-0.0.225.tar", max compression
```

## Comparing `komoutils-0.0.224.tar` & `komoutils-0.0.225.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2024-02-22 16:30:36.997703 komoutils-0.0.224/README.md
--rw-r--r--   0        0        0      294 2024-02-23 05:43:36.448362 komoutils-0.0.224/komoutils/__init__.py
--rw-r--r--   0        0        0     1822 2024-04-02 07:42:20.814589 komoutils-0.0.224/komoutils/core/__init__.py
--rw-r--r--   0        0        0        1 2024-02-25 11:24:54.905290 komoutils-0.0.224/komoutils/core/base/__init__.py
--rw-r--r--   0        0        0      579 2024-02-25 11:24:54.909290 komoutils-0.0.224/komoutils/core/base/komo_base.py
--rw-r--r--   0        0        0      973 2024-01-07 07:39:27.992568 komoutils-0.0.224/komoutils/core/base/publish_queue.py
--rw-r--r--   0        0        0     3820 2024-04-15 14:01:45.573648 komoutils-0.0.224/komoutils/core/encodings/__init__.py
--rw-r--r--   0        0        0     2289 2024-02-22 16:53:53.243852 komoutils-0.0.224/komoutils/core/time/__init__.py
--rw-r--r--   0        0        0        0 2024-02-22 16:55:04.304573 komoutils-0.0.224/komoutils/db/__init__.py
--rw-r--r--   0        0        0     1996 2024-03-11 04:12:22.829593 komoutils-0.0.224/komoutils/db/mongodb_reader_writer.py
--rw-r--r--   0        0        0      577 2024-02-23 05:43:36.436362 komoutils-0.0.224/komoutils/logger/__init__.py
--rw-r--r--   0        0        0      743 2023-03-16 15:19:40.459000 komoutils-0.0.224/komoutils/logger/logger.py
--rw-r--r--   0        0        0     1254 2024-02-23 05:43:36.400362 komoutils-0.0.224/komoutils/logger/struct_logger.py
--rw-r--r--   0        0        0      380 2024-04-15 15:06:34.442250 komoutils-0.0.224/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 komoutils-0.0.224/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-22 16:30:36.997703 komoutils-0.0.225/README.md
+-rw-r--r--   0        0        0      294 2024-02-23 05:43:36.448362 komoutils-0.0.225/komoutils/__init__.py
+-rw-r--r--   0        0        0     1822 2024-04-02 07:42:20.814589 komoutils-0.0.225/komoutils/core/__init__.py
+-rw-r--r--   0        0        0        1 2024-02-25 11:24:54.905290 komoutils-0.0.225/komoutils/core/base/__init__.py
+-rw-r--r--   0        0        0      579 2024-02-25 11:24:54.909290 komoutils-0.0.225/komoutils/core/base/komo_base.py
+-rw-r--r--   0        0        0      973 2024-01-07 07:39:27.992568 komoutils-0.0.225/komoutils/core/base/publish_queue.py
+-rw-r--r--   0        0        0     3820 2024-04-15 14:01:45.573648 komoutils-0.0.225/komoutils/core/encodings/__init__.py
+-rw-r--r--   0        0        0     2289 2024-02-22 16:53:53.243852 komoutils-0.0.225/komoutils/core/time/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-22 16:55:04.304573 komoutils-0.0.225/komoutils/db/__init__.py
+-rw-r--r--   0        0        0     4821 2024-05-01 10:59:48.559383 komoutils-0.0.225/komoutils/db/mongodb_reader_writer.py
+-rw-r--r--   0        0        0      577 2024-02-23 05:43:36.436362 komoutils-0.0.225/komoutils/logger/__init__.py
+-rw-r--r--   0        0        0      743 2023-03-16 15:19:40.459000 komoutils-0.0.225/komoutils/logger/logger.py
+-rw-r--r--   0        0        0     1254 2024-02-23 05:43:36.400362 komoutils-0.0.225/komoutils/logger/struct_logger.py
+-rw-r--r--   0        0        0      361 2024-05-01 10:59:53.367419 komoutils-0.0.225/pyproject.toml
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 komoutils-0.0.225/PKG-INFO
```

### Comparing `komoutils-0.0.224/komoutils/core/__init__.py` & `komoutils-0.0.225/komoutils/core/__init__.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.224/komoutils/core/base/komo_base.py` & `komoutils-0.0.225/komoutils/core/base/komo_base.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.224/komoutils/core/base/publish_queue.py` & `komoutils-0.0.225/komoutils/core/base/publish_queue.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.224/komoutils/core/encodings/__init__.py` & `komoutils-0.0.225/komoutils/core/encodings/__init__.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.224/komoutils/core/time/__init__.py` & `komoutils-0.0.225/komoutils/core/time/__init__.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.224/komoutils/logger/__init__.py` & `komoutils-0.0.225/komoutils/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.224/komoutils/logger/logger.py` & `komoutils-0.0.225/komoutils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.224/komoutils/logger/struct_logger.py` & `komoutils-0.0.225/komoutils/logger/struct_logger.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.224/PKG-INFO` & `komoutils-0.0.225/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: komoutils
-Version: 0.0.224
+Version: 0.0.225
 Summary: 
 Author: Makhosonke Morafo
 Author-email: makhosonke@komokun.org
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: pendulum (==3.0.0)
-Requires-Dist: prefect (==2.10.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pymongo (>=4.6.2,<5.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Description-Content-Type: text/markdown
```

