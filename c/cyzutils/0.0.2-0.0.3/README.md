# Comparing `tmp/cyzutils-0.0.2.tar.gz` & `tmp/cyzutils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyzutils-0.0.2.tar", last modified: Tue Apr 30 11:38:53 2024, max compression
+gzip compressed data, was "cyzutils-0.0.3.tar", last modified: Thu May  2 16:13:08 2024, max compression
```

## Comparing `cyzutils-0.0.2.tar` & `cyzutils-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 11:38:53.751339 cyzutils-0.0.2/
--rw-rw-rw-   0        0        0      653 2024-04-30 11:38:53.742921 cyzutils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-04-15 06:35:04.000000 cyzutils-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 11:38:53.714508 cyzutils-0.0.2/cyzutils/
--rw-rw-rw-   0        0        0       19 2024-04-08 07:21:05.000000 cyzutils-0.0.2/cyzutils/__init__.py
--rw-rw-rw-   0        0        0     2082 2024-04-30 11:34:25.000000 cyzutils-0.0.2/cyzutils/mail.py
-drwxrwxrwx   0        0        0        0 2024-04-30 11:38:53.740924 cyzutils-0.0.2/cyzutils.egg-info/
--rw-rw-rw-   0        0        0      653 2024-04-30 11:38:53.000000 cyzutils-0.0.2/cyzutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-04-30 11:38:53.000000 cyzutils-0.0.2/cyzutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 11:38:53.000000 cyzutils-0.0.2/cyzutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 11:38:53.000000 cyzutils-0.0.2/cyzutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 11:38:53.752335 cyzutils-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1116 2024-04-15 06:33:21.000000 cyzutils-0.0.2/setup.py
+drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-05-02 16:13:08.455174 cyzutils-0.0.3/
+-rw-r--r--   0 cyz        (501) staff       (20)     1024 2024-05-02 16:13:08.455001 cyzutils-0.0.3/PKG-INFO
+-rw-rw-rw-   0 cyz        (501) staff       (20)      835 2024-05-02 16:12:29.000000 cyzutils-0.0.3/README.md
+drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-05-02 16:13:08.453287 cyzutils-0.0.3/cyzutils/
+-rw-rw-rw-   0 cyz        (501) staff       (20)       19 2024-04-08 07:21:05.000000 cyzutils-0.0.3/cyzutils/__init__.py
+-rw-rw-rw-   0 cyz        (501) staff       (20)     2082 2024-04-30 11:34:25.000000 cyzutils-0.0.3/cyzutils/mail.py
+-rw-r--r--   0 cyz        (501) staff       (20)     1468 2024-05-02 16:09:18.000000 cyzutils-0.0.3/cyzutils/run_py.py
+drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-05-02 16:13:08.454824 cyzutils-0.0.3/cyzutils.egg-info/
+-rw-r--r--   0 cyz        (501) staff       (20)     1024 2024-05-02 16:13:08.000000 cyzutils-0.0.3/cyzutils.egg-info/PKG-INFO
+-rw-r--r--   0 cyz        (501) staff       (20)      203 2024-05-02 16:13:08.000000 cyzutils-0.0.3/cyzutils.egg-info/SOURCES.txt
+-rw-r--r--   0 cyz        (501) staff       (20)        1 2024-05-02 16:13:08.000000 cyzutils-0.0.3/cyzutils.egg-info/dependency_links.txt
+-rw-r--r--   0 cyz        (501) staff       (20)        9 2024-05-02 16:13:08.000000 cyzutils-0.0.3/cyzutils.egg-info/top_level.txt
+-rw-r--r--   0 cyz        (501) staff       (20)       38 2024-05-02 16:13:08.455211 cyzutils-0.0.3/setup.cfg
+-rw-rw-rw-   0 cyz        (501) staff       (20)     1116 2024-05-02 14:55:34.000000 cyzutils-0.0.3/setup.py
```

### Comparing `cyzutils-0.0.2/cyzutils/mail.py` & `cyzutils-0.0.3/cyzutils/mail.py`

 * *Files identical despite different names*

### Comparing `cyzutils-0.0.2/setup.py` & `cyzutils-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(here, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='cyzutils',  # 必填，项目的名字，用户根据这个名字安装，pip install SpiderKeeper-new
-    version='0.0.2',  # 必填，项目的版本，建议遵循语义化版本规范
+    version='0.0.3',  # 必填，项目的版本，建议遵循语义化版本规范
     author='cyz020403',  # 项目的作者
     description='my utils',  # 项目的一个简短描述
     long_description=long_description,  # 项目的详细说明，通常读取 README.md 文件的内容
     long_description_content_type='text/markdown',  # 描述的格式，可选的值： text/plain, text/x-rst, and text/markdown
     author_email='cyz020403@gmail.com',  # 作者的有效邮箱地址
     url='https://github.com/cyz020403',  # 项目的源码地址
     license='MIT',
```

