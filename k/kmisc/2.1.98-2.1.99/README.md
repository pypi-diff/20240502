# Comparing `tmp/kmisc-2.1.98.tar.gz` & `tmp/kmisc-2.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmisc-2.1.98.tar", last modified: Thu Dec  7 16:00:32 2023, max compression
+gzip compressed data, was "kmisc-2.1.99.tar", last modified: Wed Dec 20 17:12:01 2023, max compression
```

## Comparing `kmisc-2.1.98.tar` & `kmisc-2.1.99.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2023-12-07 16:00:32.977311 kmisc-2.1.98/
--rw-rw-r--   0 kage      (1000) kage      (1000)     1066 2021-12-15 17:55:20.000000 kmisc-2.1.98/LICENSE
--rw-r--r--   0 kage      (1000) kage      (1000)     5502 2023-12-07 16:00:32.977311 kmisc-2.1.98/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)     5084 2022-02-08 03:10:22.000000 kmisc-2.1.98/README.md
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2023-12-07 16:00:32.976311 kmisc-2.1.98/kmisc/
--rw-r--r--   0 kage      (1000) kage      (1000)   133273 2023-12-07 15:59:33.000000 kmisc-2.1.98/kmisc/__init__.py
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2023-12-07 16:00:32.977311 kmisc-2.1.98/kmisc.egg-info/
--rw-rw-r--   0 kage      (1000) kage      (1000)     5502 2023-12-07 16:00:32.000000 kmisc-2.1.98/kmisc.egg-info/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)      175 2023-12-07 16:00:32.000000 kmisc-2.1.98/kmisc.egg-info/SOURCES.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        1 2023-12-07 16:00:32.000000 kmisc-2.1.98/kmisc.egg-info/dependency_links.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        6 2023-12-07 16:00:32.000000 kmisc-2.1.98/kmisc.egg-info/top_level.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)      104 2021-12-15 17:55:20.000000 kmisc-2.1.98/pyproject.toml
--rw-r--r--   0 kage      (1000) kage      (1000)       38 2023-12-07 16:00:32.977311 kmisc-2.1.98/setup.cfg
--rw-rw-r--   0 kage      (1000) kage      (1000)     1974 2021-12-16 01:37:50.000000 kmisc-2.1.98/setup.py
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2023-12-20 17:12:01.414912 kmisc-2.1.99/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1066 2021-12-15 17:55:20.000000 kmisc-2.1.99/LICENSE
+-rw-r--r--   0 kage      (1000) kage      (1000)     5502 2023-12-20 17:12:01.414912 kmisc-2.1.99/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)     5084 2022-02-08 03:10:22.000000 kmisc-2.1.99/README.md
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2023-12-20 17:12:01.413912 kmisc-2.1.99/kmisc/
+-rw-r--r--   0 kage      (1000) kage      (1000)   133266 2023-12-20 17:11:10.000000 kmisc-2.1.99/kmisc/__init__.py
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2023-12-20 17:12:01.413912 kmisc-2.1.99/kmisc.egg-info/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     5502 2023-12-20 17:12:01.000000 kmisc-2.1.99/kmisc.egg-info/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)      175 2023-12-20 17:12:01.000000 kmisc-2.1.99/kmisc.egg-info/SOURCES.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        1 2023-12-20 17:12:01.000000 kmisc-2.1.99/kmisc.egg-info/dependency_links.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        6 2023-12-20 17:12:01.000000 kmisc-2.1.99/kmisc.egg-info/top_level.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)      104 2021-12-15 17:55:20.000000 kmisc-2.1.99/pyproject.toml
+-rw-r--r--   0 kage      (1000) kage      (1000)       38 2023-12-20 17:12:01.414912 kmisc-2.1.99/setup.cfg
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1974 2021-12-16 01:37:50.000000 kmisc-2.1.99/setup.py
```

### Comparing `kmisc-2.1.98/LICENSE` & `kmisc-2.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `kmisc-2.1.98/PKG-INFO` & `kmisc-2.1.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmisc
-Version: 2.1.98
+Version: 2.1.99
 Summary: Enginering useful library
 Home-page: https://github.com/kagepark/kmisc
 Author: Kage Park
 License: MIT
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kmisc-2.1.98/README.md` & `kmisc-2.1.99/README.md`

 * *Files identical despite different names*

### Comparing `kmisc-2.1.98/kmisc/__init__.py` & `kmisc-2.1.99/kmisc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1693,15 +1693,15 @@
             print('no title')
             return False
         scr_id=self.Id(title)
         if scr_id:
             print('Already has the title at {}'.format(scr_id))
             return False
         
-        if not IP(ip).IsBmcIp(port=(623,664,443)):
+        if not IpV4(ip,port=(623,664,443)):
             print('{} is not ipmi ip'.format(ip))
             return False
 
         # if Not support SOL 
         if self.Info(ip,ipmi_user,ipmi_pass)[0] is False:
             print('The BMC is not support SOL function')
             return False
```

### Comparing `kmisc-2.1.98/kmisc.egg-info/PKG-INFO` & `kmisc-2.1.99/kmisc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmisc
-Version: 2.1.98
+Version: 2.1.99
 Summary: Enginering useful library
 Home-page: https://github.com/kagepark/kmisc
 Author: Kage Park
 License: MIT
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kmisc-2.1.98/setup.py` & `kmisc-2.1.99/setup.py`

 * *Files identical despite different names*

