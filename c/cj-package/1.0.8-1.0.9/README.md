# Comparing `tmp/cj_package-1.0.8.tar.gz` & `tmp/cj_package-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cj_package-1.0.8.tar", last modified: Wed Mar 27 02:47:57 2024, max compression
+gzip compressed data, was "cj_package-1.0.9.tar", last modified: Wed Mar 27 07:00:50 2024, max compression
```

## Comparing `cj_package-1.0.8.tar` & `cj_package-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 02:47:57.040786 cj_package-1.0.8/
--rw-r--r--   0 caojie     (501) staff       (20)     1068 2024-03-15 01:36:01.000000 cj_package-1.0.8/LICENSE
--rw-r--r--   0 caojie     (501) staff       (20)     1374 2024-03-27 02:47:57.040311 cj_package-1.0.8/PKG-INFO
--rw-r--r--   0 caojie     (501) staff       (20)      803 2024-03-27 02:46:58.000000 cj_package-1.0.8/README.md
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 02:47:57.026280 cj_package-1.0.8/cj_package/
--rw-r--r--   0 caojie     (501) staff       (20)      141 2024-03-26 10:05:44.000000 cj_package-1.0.8/cj_package/__init__.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 02:47:57.029822 cj_package-1.0.8/cj_package/aliyun/
--rw-r--r--   0 caojie     (501) staff       (20)       48 2024-03-15 06:21:59.000000 cj_package-1.0.8/cj_package/aliyun/__init__.py
--rw-r--r--   0 caojie     (501) staff       (20)     4979 2024-03-27 02:46:58.000000 cj_package-1.0.8/cj_package/aliyun/sls.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 02:47:57.031285 cj_package-1.0.8/cj_package/command/
--rw-r--r--   0 caojie     (501) staff       (20)       60 2024-03-21 00:51:11.000000 cj_package-1.0.8/cj_package/command/__init__.py
--rw-r--r--   0 caojie     (501) staff       (20)     2110 2024-03-26 09:31:08.000000 cj_package-1.0.8/cj_package/command/base.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 02:47:57.033940 cj_package-1.0.8/cj_package/domain/
--rw-r--r--   0 caojie     (501) staff       (20)       70 2024-03-26 07:16:36.000000 cj_package-1.0.8/cj_package/domain/__init__.py
--rw-r--r--   0 caojie     (501) staff       (20)     3057 2024-03-26 09:25:43.000000 cj_package-1.0.8/cj_package/domain/cert.py
--rw-r--r--   0 caojie     (501) staff       (20)      776 2024-03-26 07:23:25.000000 cj_package-1.0.8/cj_package/domain/resolve_ip.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 02:47:57.035472 cj_package-1.0.8/cj_package/excel/
--rw-r--r--   0 caojie     (501) staff       (20)       35 2024-03-15 06:50:33.000000 cj_package-1.0.8/cj_package/excel/__init__.py
--rw-r--r--   0 caojie     (501) staff       (20)      748 2024-03-18 01:24:09.000000 cj_package-1.0.8/cj_package/excel/base.py
--rw-r--r--   0 caojie     (501) staff       (20)      222 2024-03-26 12:41:37.000000 cj_package-1.0.8/cj_package/info.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 02:47:57.036977 cj_package-1.0.8/cj_package/qw/
--rw-r--r--   0 caojie     (501) staff       (20)       46 2024-03-15 07:32:48.000000 cj_package-1.0.8/cj_package/qw/__init__.py
--rw-r--r--   0 caojie     (501) staff       (20)      869 2024-03-21 00:51:11.000000 cj_package-1.0.8/cj_package/qw/sendMessage.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 02:47:57.038470 cj_package-1.0.8/cj_package/sql/
--rw-r--r--   0 caojie     (501) staff       (20)       29 2024-03-26 10:17:53.000000 cj_package-1.0.8/cj_package/sql/__init__.py
--rw-r--r--   0 caojie     (501) staff       (20)      921 2024-03-26 10:27:31.000000 cj_package-1.0.8/cj_package/sql/mysql.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 02:47:57.039419 cj_package-1.0.8/cj_package.egg-info/
--rw-r--r--   0 caojie     (501) staff       (20)     1374 2024-03-27 02:47:56.000000 cj_package-1.0.8/cj_package.egg-info/PKG-INFO
--rw-r--r--   0 caojie     (501) staff       (20)      598 2024-03-27 02:47:56.000000 cj_package-1.0.8/cj_package.egg-info/SOURCES.txt
--rw-r--r--   0 caojie     (501) staff       (20)        1 2024-03-27 02:47:56.000000 cj_package-1.0.8/cj_package.egg-info/dependency_links.txt
--rw-r--r--   0 caojie     (501) staff       (20)      109 2024-03-27 02:47:56.000000 cj_package-1.0.8/cj_package.egg-info/requires.txt
--rw-r--r--   0 caojie     (501) staff       (20)       11 2024-03-27 02:47:56.000000 cj_package-1.0.8/cj_package.egg-info/top_level.txt
--rw-r--r--   0 caojie     (501) staff       (20)       38 2024-03-27 02:47:57.040885 cj_package-1.0.8/setup.cfg
--rw-r--r--   0 caojie     (501) staff       (20)     1534 2024-03-27 02:47:53.000000 cj_package-1.0.8/setup.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 07:00:50.504509 cj_package-1.0.9/
+-rw-r--r--   0 caojie     (501) staff       (20)     1068 2024-03-15 01:36:01.000000 cj_package-1.0.9/LICENSE
+-rw-r--r--   0 caojie     (501) staff       (20)     1377 2024-03-27 07:00:50.504031 cj_package-1.0.9/PKG-INFO
+-rw-r--r--   0 caojie     (501) staff       (20)      806 2024-03-27 05:37:16.000000 cj_package-1.0.9/README.md
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 07:00:50.490483 cj_package-1.0.9/cj_package/
+-rw-r--r--   0 caojie     (501) staff       (20)      141 2024-03-26 10:05:44.000000 cj_package-1.0.9/cj_package/__init__.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 07:00:50.493971 cj_package-1.0.9/cj_package/aliyun/
+-rw-r--r--   0 caojie     (501) staff       (20)       81 2024-03-27 02:51:10.000000 cj_package-1.0.9/cj_package/aliyun/__init__.py
+-rw-r--r--   0 caojie     (501) staff       (20)     4979 2024-03-27 02:46:58.000000 cj_package-1.0.9/cj_package/aliyun/sls.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 07:00:50.495532 cj_package-1.0.9/cj_package/command/
+-rw-r--r--   0 caojie     (501) staff       (20)       60 2024-03-21 00:51:11.000000 cj_package-1.0.9/cj_package/command/__init__.py
+-rw-r--r--   0 caojie     (501) staff       (20)     2110 2024-03-26 09:31:08.000000 cj_package-1.0.9/cj_package/command/base.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 07:00:50.497924 cj_package-1.0.9/cj_package/domain/
+-rw-r--r--   0 caojie     (501) staff       (20)       70 2024-03-26 07:16:36.000000 cj_package-1.0.9/cj_package/domain/__init__.py
+-rw-r--r--   0 caojie     (501) staff       (20)     3057 2024-03-26 09:25:43.000000 cj_package-1.0.9/cj_package/domain/cert.py
+-rw-r--r--   0 caojie     (501) staff       (20)      776 2024-03-26 07:23:25.000000 cj_package-1.0.9/cj_package/domain/resolve_ip.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 07:00:50.499258 cj_package-1.0.9/cj_package/excel/
+-rw-r--r--   0 caojie     (501) staff       (20)       35 2024-03-15 06:50:33.000000 cj_package-1.0.9/cj_package/excel/__init__.py
+-rw-r--r--   0 caojie     (501) staff       (20)      779 2024-03-27 05:47:02.000000 cj_package-1.0.9/cj_package/excel/base.py
+-rw-r--r--   0 caojie     (501) staff       (20)      222 2024-03-26 12:41:37.000000 cj_package-1.0.9/cj_package/info.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 07:00:50.499987 cj_package-1.0.9/cj_package/k8s/
+-rw-r--r--   0 caojie     (501) staff       (20)        0 2024-03-27 02:54:52.000000 cj_package-1.0.9/cj_package/k8s/__init__.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 07:00:50.500978 cj_package-1.0.9/cj_package/qw/
+-rw-r--r--   0 caojie     (501) staff       (20)       46 2024-03-15 07:32:48.000000 cj_package-1.0.9/cj_package/qw/__init__.py
+-rw-r--r--   0 caojie     (501) staff       (20)      869 2024-03-21 00:51:11.000000 cj_package-1.0.9/cj_package/qw/sendMessage.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 07:00:50.502372 cj_package-1.0.9/cj_package/sql/
+-rw-r--r--   0 caojie     (501) staff       (20)       29 2024-03-26 10:17:53.000000 cj_package-1.0.9/cj_package/sql/__init__.py
+-rw-r--r--   0 caojie     (501) staff       (20)     1265 2024-03-27 06:03:08.000000 cj_package-1.0.9/cj_package/sql/mysql.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-03-27 07:00:50.503214 cj_package-1.0.9/cj_package.egg-info/
+-rw-r--r--   0 caojie     (501) staff       (20)     1377 2024-03-27 07:00:50.000000 cj_package-1.0.9/cj_package.egg-info/PKG-INFO
+-rw-r--r--   0 caojie     (501) staff       (20)      625 2024-03-27 07:00:50.000000 cj_package-1.0.9/cj_package.egg-info/SOURCES.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        1 2024-03-27 07:00:50.000000 cj_package-1.0.9/cj_package.egg-info/dependency_links.txt
+-rw-r--r--   0 caojie     (501) staff       (20)      109 2024-03-27 07:00:50.000000 cj_package-1.0.9/cj_package.egg-info/requires.txt
+-rw-r--r--   0 caojie     (501) staff       (20)       11 2024-03-27 07:00:50.000000 cj_package-1.0.9/cj_package.egg-info/top_level.txt
+-rw-r--r--   0 caojie     (501) staff       (20)       38 2024-03-27 07:00:50.504608 cj_package-1.0.9/setup.cfg
+-rw-r--r--   0 caojie     (501) staff       (20)     1534 2024-03-27 07:00:29.000000 cj_package-1.0.9/setup.py
```

### Comparing `cj_package-1.0.8/LICENSE` & `cj_package-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cj_package-1.0.8/PKG-INFO` & `cj_package-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cj_package
-Version: 1.0.8
+Version: 1.0.9
 Summary: cj package
 Author: cj
 Author-email: chenxing@cjdropshipping.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
@@ -14,15 +14,15 @@
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: requests>=2.31.0
 Requires-Dist: loguru>=0.6.0
 Requires-Dist: dnspython>=2.6.1
 Requires-Dist: pendulum
 Requires-Dist: pymysql
 
-# 功能
+# 工具集
 
 ## aliyun
 阿里云相关功能方法
 > 1.杭州ingress日志查询方法  hz_ingress_log
 > 1.杭州service日志查询方法  hz_service_log
 > 2.硅谷ingress日志查询方法  usa_ingress_log
 > 2.硅谷service日志查询方法  usa_service_log
```

### Comparing `cj_package-1.0.8/README.md` & `cj_package-1.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 功能
+# 工具集
 
 ## aliyun
 阿里云相关功能方法
 > 1.杭州ingress日志查询方法  hz_ingress_log
 > 1.杭州service日志查询方法  hz_service_log
 > 2.硅谷ingress日志查询方法  usa_ingress_log
 > 2.硅谷service日志查询方法  usa_service_log
```

### Comparing `cj_package-1.0.8/cj_package/aliyun/sls.py` & `cj_package-1.0.9/cj_package/aliyun/sls.py`

 * *Files identical despite different names*

### Comparing `cj_package-1.0.8/cj_package/command/base.py` & `cj_package-1.0.9/cj_package/command/base.py`

 * *Files identical despite different names*

### Comparing `cj_package-1.0.8/cj_package/domain/cert.py` & `cj_package-1.0.9/cj_package/domain/cert.py`

 * *Files identical despite different names*

### Comparing `cj_package-1.0.8/cj_package/domain/resolve_ip.py` & `cj_package-1.0.9/cj_package/domain/resolve_ip.py`

 * *Files identical despite different names*

### Comparing `cj_package-1.0.8/cj_package/excel/base.py` & `cj_package-1.0.9/cj_package/excel/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import pandas as pd
 
 def list_write_excel(data: list, filename=None):
     """
-    将列表字典写入excel中
+    将列表字典写入excel中,默认保存文件名data.xlsx
     @param data: 数据,列表字典
     @param filename: 文件名[可选]
     """
     # 判断data是否为list类型
     if not isinstance(data, list):
         raise Exception('传入data必须为list类型')
     if filename and not str(filename).endswith('.xlsx'):
```

### Comparing `cj_package-1.0.8/cj_package/qw/sendMessage.py` & `cj_package-1.0.9/cj_package/qw/sendMessage.py`

 * *Files identical despite different names*

### Comparing `cj_package-1.0.8/cj_package.egg-info/PKG-INFO` & `cj_package-1.0.9/cj_package.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cj_package
-Version: 1.0.8
+Version: 1.0.9
 Summary: cj package
 Author: cj
 Author-email: chenxing@cjdropshipping.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
@@ -14,15 +14,15 @@
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: requests>=2.31.0
 Requires-Dist: loguru>=0.6.0
 Requires-Dist: dnspython>=2.6.1
 Requires-Dist: pendulum
 Requires-Dist: pymysql
 
-# 功能
+# 工具集
 
 ## aliyun
 阿里云相关功能方法
 > 1.杭州ingress日志查询方法  hz_ingress_log
 > 1.杭州service日志查询方法  hz_service_log
 > 2.硅谷ingress日志查询方法  usa_ingress_log
 > 2.硅谷service日志查询方法  usa_service_log
```

### Comparing `cj_package-1.0.8/cj_package.egg-info/SOURCES.txt` & `cj_package-1.0.9/cj_package.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 cj_package/command/__init__.py
 cj_package/command/base.py
 cj_package/domain/__init__.py
 cj_package/domain/cert.py
 cj_package/domain/resolve_ip.py
 cj_package/excel/__init__.py
 cj_package/excel/base.py
+cj_package/k8s/__init__.py
 cj_package/qw/__init__.py
 cj_package/qw/sendMessage.py
 cj_package/sql/__init__.py
 cj_package/sql/mysql.py
```

### Comparing `cj_package-1.0.8/setup.py` & `cj_package-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="cj_package",
      # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="1.0.8",
+    version="1.0.9",
     # 作者名
     author="cj",
      # 作者邮箱
     author_email="chenxing@cjdropshipping.co",
     # 包的简介描述
     description="cj package",
     # 包的详细介绍(一般通过加载README.md)
```

