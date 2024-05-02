# Comparing `tmp/aic_tools_alpaca-0.0.3.tar.gz` & `tmp/aic_tools_alpaca-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aic_tools_alpaca-0.0.3.tar", last modified: Thu Apr  4 04:09:58 2024, max compression
+gzip compressed data, was "aic_tools_alpaca-1.0.0.tar", last modified: Thu May  2 04:08:12 2024, max compression
```

## Comparing `aic_tools_alpaca-0.0.3.tar` & `aic_tools_alpaca-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-04 04:09:58.505378 aic_tools_alpaca-0.0.3/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      272 2024-04-04 04:09:58.505253 aic_tools_alpaca-0.0.3/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      584 2024-04-02 01:02:37.000000 aic_tools_alpaca-0.0.3/README.md
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-04 04:09:58.504459 aic_tools_alpaca-0.0.3/aic_tools_alpaca/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-04 04:09:50.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca/__init__.py
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      716 2024-04-04 04:09:41.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca/account_info.py
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-04 04:09:58.505083 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      272 2024-04-04 04:09:58.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      279 2024-04-04 04:09:58.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/SOURCES.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-04 04:09:58.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/dependency_links.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       18 2024-04-04 04:09:58.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/requires.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       17 2024-04-04 04:09:58.000000 aic_tools_alpaca-0.0.3/aic_tools_alpaca.egg-info/top_level.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-04 04:09:58.505421 aic_tools_alpaca-0.0.3/setup.cfg
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      734 2024-04-04 04:09:55.000000 aic_tools_alpaca-0.0.3/setup.py
+drwxrwxr-x   0 serhii    (1000) serhii    (1000)        0 2024-05-02 04:08:12.569329 aic_tools_alpaca-1.0.0/
+-rw-r--r--   0 serhii    (1000) serhii    (1000)      605 2024-05-02 04:08:12.569329 aic_tools_alpaca-1.0.0/PKG-INFO
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)      311 2024-04-22 11:29:53.000000 aic_tools_alpaca-1.0.0/README.md
+drwxrwxr-x   0 serhii    (1000) serhii    (1000)        0 2024-05-02 04:08:12.567329 aic_tools_alpaca-1.0.0/aic_tools_alpaca/
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)        0 2024-04-21 15:47:15.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca/__init__.py
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)     1889 2024-05-01 10:51:28.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca/account_info.py
+drwxrwxr-x   0 serhii    (1000) serhii    (1000)        0 2024-05-02 04:08:12.568329 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/
+-rw-r--r--   0 serhii    (1000) serhii    (1000)      605 2024-05-02 04:08:11.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/PKG-INFO
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)      344 2024-05-02 04:08:11.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/SOURCES.txt
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)        1 2024-05-02 04:08:11.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/dependency_links.txt
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)       38 2024-05-02 04:08:11.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/requires.txt
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)       23 2024-05-02 04:08:11.000000 aic_tools_alpaca-1.0.0/aic_tools_alpaca.egg-info/top_level.txt
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)       38 2024-05-02 04:08:12.569329 aic_tools_alpaca-1.0.0/setup.cfg
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)      784 2024-05-02 03:48:52.000000 aic_tools_alpaca-1.0.0/setup.py
+drwxrwxr-x   0 serhii    (1000) serhii    (1000)        0 2024-05-02 04:08:12.568329 aic_tools_alpaca-1.0.0/tests/
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)        0 2024-04-21 16:42:01.000000 aic_tools_alpaca-1.0.0/tests/__init__.py
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)      438 2024-05-01 10:51:28.000000 aic_tools_alpaca-1.0.0/tests/handy_test.py
+-rw-rw-r--   0 serhii    (1000) serhii    (1000)     1771 2024-05-01 10:51:28.000000 aic_tools_alpaca-1.0.0/tests/test_account_info.py
```

### Comparing `aic_tools_alpaca-0.0.3/setup.py` & `aic_tools_alpaca-1.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from setuptools import setup, find_packages
 
+
 # Function to read the contents of the requirements file
 def read_requirements():
     with open('requirements.txt', 'r') as req:
         # Exclude any comments or empty lines
         return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
+
 # Call the function and store the requirements list
 install_requires = read_requirements()
 
 setup(
     name='aic_tools_alpaca',
-    version='0.0.3',
+    version='1.0.0',
     packages=find_packages(),
     description='Alpaca tools for AI Characters',
     long_description_content_type='text/markdown',
+    long_description=open('README.md').read(),
     author='Viacheslav Kovalevskyi',
     author_email='viacheslav@kovalevskyi.com',
     license='MIT',
     install_requires=install_requires
-)
+)
```

