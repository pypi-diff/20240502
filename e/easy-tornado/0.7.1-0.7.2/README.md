# Comparing `tmp/easy_tornado-0.7.1.tar.gz` & `tmp/easy_tornado-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_tornado-0.7.1.tar", last modified: Thu Jan 18 11:56:38 2024, max compression
+gzip compressed data, was "easy_tornado-0.7.2.tar", last modified: Thu May  2 09:14:01 2024, max compression
```

## Comparing `easy_tornado-0.7.1.tar` & `easy_tornado-0.7.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 wangshugen5   (502) staff       (20)        0 2024-01-18 11:56:38.716416 easy_tornado-0.7.1/
--rw-r--r--   0 wangshugen5   (502) staff       (20)      343 2024-01-18 11:56:38.716216 easy_tornado-0.7.1/PKG-INFO
--rw-r--r--   0 wangshugen5   (502) staff       (20)      315 2023-10-10 08:01:52.000000 easy_tornado-0.7.1/README.md
-drwxr-xr-x   0 wangshugen5   (502) staff       (20)        0 2024-01-18 11:56:38.712334 easy_tornado-0.7.1/easy_tornado/
--rw-r--r--   0 wangshugen5   (502) staff       (20)      634 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/__init__.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     2406 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/compat.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     1444 2023-10-10 08:01:52.000000 easy_tornado-0.7.1/easy_tornado/filtering.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     2009 2023-10-10 08:01:52.000000 easy_tornado-0.7.1/easy_tornado/functional.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     4734 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/invoking.py
-drwxr-xr-x   0 wangshugen5   (502) staff       (20)        0 2024-01-18 11:56:38.715373 easy_tornado-0.7.1/easy_tornado/utility/
--rw-r--r--   0 wangshugen5   (502) staff       (20)     2472 2024-01-18 09:10:46.000000 easy_tornado-0.7.1/easy_tornado/utility/__init__.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)      339 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/utility/collection.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     7336 2024-01-18 09:10:46.000000 easy_tornado-0.7.1/easy_tornado/utility/datetime.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)      925 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/utility/exception.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     8519 2024-01-18 09:10:46.000000 easy_tornado-0.7.1/easy_tornado/utility/filesystem.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     2494 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/utility/httpclient.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     3352 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/utility/printext.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     1351 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/utility/runtime.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     1853 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/utility/stringext.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)      862 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/utility/validation.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     3701 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/utility/webext.py
-drwxr-xr-x   0 wangshugen5   (502) staff       (20)        0 2024-01-18 11:56:38.715701 easy_tornado-0.7.1/easy_tornado/web/
--rw-r--r--   0 wangshugen5   (502) staff       (20)       59 2023-10-10 08:01:52.000000 easy_tornado-0.7.1/easy_tornado/web/__init__.py
--rw-r--r--   0 wangshugen5   (502) staff       (20)     8055 2024-01-18 09:09:35.000000 easy_tornado-0.7.1/easy_tornado/web/web_application_handler.py
-drwxr-xr-x   0 wangshugen5   (502) staff       (20)        0 2024-01-18 11:56:38.716003 easy_tornado-0.7.1/easy_tornado.egg-info/
--rw-r--r--   0 wangshugen5   (502) staff       (20)      343 2024-01-18 11:56:38.000000 easy_tornado-0.7.1/easy_tornado.egg-info/PKG-INFO
--rw-r--r--   0 wangshugen5   (502) staff       (20)      766 2024-01-18 11:56:38.000000 easy_tornado-0.7.1/easy_tornado.egg-info/SOURCES.txt
--rw-r--r--   0 wangshugen5   (502) staff       (20)        1 2024-01-18 11:56:38.000000 easy_tornado-0.7.1/easy_tornado.egg-info/dependency_links.txt
--rw-r--r--   0 wangshugen5   (502) staff       (20)       37 2024-01-18 11:56:38.000000 easy_tornado-0.7.1/easy_tornado.egg-info/requires.txt
--rw-r--r--   0 wangshugen5   (502) staff       (20)       13 2024-01-18 11:56:38.000000 easy_tornado-0.7.1/easy_tornado.egg-info/top_level.txt
--rw-r--r--   0 wangshugen5   (502) staff       (20)       38 2024-01-18 11:56:38.716472 easy_tornado-0.7.1/setup.cfg
--rw-r--r--   0 wangshugen5   (502) staff       (20)      607 2024-01-18 09:10:46.000000 easy_tornado-0.7.1/setup.py
+drwxr-xr-x   0 empire     (501) staff       (20)        0 2024-05-02 09:14:01.233053 easy_tornado-0.7.2/
+-rw-r--r--   0 empire     (501) staff       (20)      343 2024-05-02 09:14:01.232835 easy_tornado-0.7.2/PKG-INFO
+-rw-r--r--   0 empire     (501) staff       (20)      315 2021-02-08 17:07:53.000000 easy_tornado-0.7.2/README.md
+drwxr-xr-x   0 empire     (501) staff       (20)        0 2024-05-02 09:14:01.229708 easy_tornado-0.7.2/easy_tornado/
+-rw-r--r--   0 empire     (501) staff       (20)      634 2024-05-02 05:00:12.000000 easy_tornado-0.7.2/easy_tornado/__init__.py
+-rw-r--r--   0 empire     (501) staff       (20)     2406 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/compat.py
+-rw-r--r--   0 empire     (501) staff       (20)     1444 2021-01-16 15:07:01.000000 easy_tornado-0.7.2/easy_tornado/filtering.py
+-rw-r--r--   0 empire     (501) staff       (20)     2009 2021-01-16 15:07:06.000000 easy_tornado-0.7.2/easy_tornado/functional.py
+-rw-r--r--   0 empire     (501) staff       (20)     4770 2024-05-02 09:08:37.000000 easy_tornado-0.7.2/easy_tornado/invoking.py
+drwxr-xr-x   0 empire     (501) staff       (20)        0 2024-05-02 09:14:01.232080 easy_tornado-0.7.2/easy_tornado/utility/
+-rw-r--r--   0 empire     (501) staff       (20)     2472 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/utility/__init__.py
+-rw-r--r--   0 empire     (501) staff       (20)      339 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/utility/collection.py
+-rw-r--r--   0 empire     (501) staff       (20)     7336 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/utility/datetime.py
+-rw-r--r--   0 empire     (501) staff       (20)      925 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/utility/exception.py
+-rw-r--r--   0 empire     (501) staff       (20)     8519 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/utility/filesystem.py
+-rw-r--r--   0 empire     (501) staff       (20)     2494 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/utility/httpclient.py
+-rw-r--r--   0 empire     (501) staff       (20)     3362 2024-05-02 08:11:11.000000 easy_tornado-0.7.2/easy_tornado/utility/printext.py
+-rw-r--r--   0 empire     (501) staff       (20)     1351 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/utility/runtime.py
+-rw-r--r--   0 empire     (501) staff       (20)     1853 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/utility/stringext.py
+-rw-r--r--   0 empire     (501) staff       (20)      862 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/utility/validation.py
+-rw-r--r--   0 empire     (501) staff       (20)     3701 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/utility/webext.py
+drwxr-xr-x   0 empire     (501) staff       (20)        0 2024-05-02 09:14:01.232403 easy_tornado-0.7.2/easy_tornado/web/
+-rw-r--r--   0 empire     (501) staff       (20)       59 2019-11-07 09:59:48.000000 easy_tornado-0.7.2/easy_tornado/web/__init__.py
+-rw-r--r--   0 empire     (501) staff       (20)     8055 2024-01-18 13:27:45.000000 easy_tornado-0.7.2/easy_tornado/web/web_application_handler.py
+drwxr-xr-x   0 empire     (501) staff       (20)        0 2024-05-02 09:14:01.232596 easy_tornado-0.7.2/easy_tornado.egg-info/
+-rw-r--r--   0 empire     (501) staff       (20)      343 2024-05-02 09:14:01.000000 easy_tornado-0.7.2/easy_tornado.egg-info/PKG-INFO
+-rw-r--r--   0 empire     (501) staff       (20)      766 2024-05-02 09:14:01.000000 easy_tornado-0.7.2/easy_tornado.egg-info/SOURCES.txt
+-rw-r--r--   0 empire     (501) staff       (20)        1 2024-05-02 09:14:01.000000 easy_tornado-0.7.2/easy_tornado.egg-info/dependency_links.txt
+-rw-r--r--   0 empire     (501) staff       (20)       37 2024-05-02 09:14:01.000000 easy_tornado-0.7.2/easy_tornado.egg-info/requires.txt
+-rw-r--r--   0 empire     (501) staff       (20)       13 2024-05-02 09:14:01.000000 easy_tornado-0.7.2/easy_tornado.egg-info/top_level.txt
+-rw-r--r--   0 empire     (501) staff       (20)       38 2024-05-02 09:14:01.233097 easy_tornado-0.7.2/setup.cfg
+-rw-r--r--   0 empire     (501) staff       (20)      607 2024-05-02 09:10:22.000000 easy_tornado-0.7.2/setup.py
```

### Comparing `easy_tornado-0.7.1/easy_tornado/__init__.py` & `easy_tornado-0.7.2/easy_tornado/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/compat.py` & `easy_tornado-0.7.2/easy_tornado/compat.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/filtering.py` & `easy_tornado-0.7.2/easy_tornado/filtering.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/functional.py` & `easy_tornado-0.7.2/easy_tornado/functional.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/invoking.py` & `easy_tornado-0.7.2/easy_tornado/invoking.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # email: wangshugen@ict.ac.cn
 # date: 2018/11/14 16:30
 import codecs
 import subprocess
 import warnings
 
 from .compat import python2
-from .utility import current_datetime_r_str
+from .utility import current_datetime_str_r
 from .utility import write_file_contents
 
 NOHUP = 'nohup'
 BG_MARK = '&'
 
 
 def _get_log_paths(log_prefix):
-  time_suffix = current_datetime_r_str()
+  time_suffix = current_datetime_str_r()
 
   def refine_path(prefix, suffix):
     return '{}-{}.{}'.format(prefix, time_suffix, suffix)
 
   cmd_path = refine_path(log_prefix, 'cmd')
   out_path = refine_path(log_prefix, 'out')
   err_path = refine_path(log_prefix, 'err')
@@ -82,14 +82,15 @@
     return subprocess.check_call(
       command, shell=True, stdout=stdout, stderr=stderr
     )
   except subprocess.CalledProcessError as e:
     if on_error:
       on_error(e)
     else:
+      ret_buffer['errno'] = e.errno
       raise
 
 
 def executable_exists(executable):
   """
   检测可执行文件是否存在
   :param executable: 可执行文件
```

### Comparing `easy_tornado-0.7.1/easy_tornado/utility/__init__.py` & `easy_tornado-0.7.2/easy_tornado/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/utility/datetime.py` & `easy_tornado-0.7.2/easy_tornado/utility/datetime.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/utility/exception.py` & `easy_tornado-0.7.2/easy_tornado/utility/exception.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/utility/filesystem.py` & `easy_tornado-0.7.2/easy_tornado/utility/filesystem.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/utility/httpclient.py` & `easy_tornado-0.7.2/easy_tornado/utility/httpclient.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/utility/printext.py` & `easy_tornado-0.7.2/easy_tornado/utility/printext.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 """
 Whether enable message out or not
 """
 _enable = True
 
 
-def it_print(message='', indent=None, device=1, newline=True, json_fmt=False):
+def it_print(message='', indent=None, device=1, newline=True, json_fmt=False, **kwargs):
   """
   in time print: print one line to console immediately
 
   :param message: the message to be printed
   :type message: object
 
   :param indent: number of blank to be indented, default 0
```

### Comparing `easy_tornado-0.7.1/easy_tornado/utility/runtime.py` & `easy_tornado-0.7.2/easy_tornado/utility/runtime.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/utility/stringext.py` & `easy_tornado-0.7.2/easy_tornado/utility/stringext.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/utility/validation.py` & `easy_tornado-0.7.2/easy_tornado/utility/validation.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/utility/webext.py` & `easy_tornado-0.7.2/easy_tornado/utility/webext.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado/web/web_application_handler.py` & `easy_tornado-0.7.2/easy_tornado/web/web_application_handler.py`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/easy_tornado.egg-info/SOURCES.txt` & `easy_tornado-0.7.2/easy_tornado.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easy_tornado-0.7.1/setup.py` & `easy_tornado-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 ssl._create_default_https_context = ssl._create_unverified_context
 
 setup(
   name='easy_tornado',
-  version='0.7.1',
+  version='0.7.2',
   description='A tornado based web framework and toolkit package',
   author='Wang Shugen',
   author_email='wsg1107556314@163.com',
   url='https://artifacts.wshugen.cn/python/easy_tornado',
   packages=find_packages(),
   install_requires=['tornado', 'decorator', 'six', 'urllib3', 'psutil']
 )
```

