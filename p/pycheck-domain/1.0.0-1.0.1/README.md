# Comparing `tmp/pycheck_domain-1.0.0.tar.gz` & `tmp/pycheck_domain-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycheck_domain-1.0.0.tar", last modified: Fri Mar 15 14:42:26 2024, max compression
+gzip compressed data, was "pycheck_domain-1.0.1.tar", last modified: Thu May  2 14:36:36 2024, max compression
```

## Comparing `pycheck_domain-1.0.0.tar` & `pycheck_domain-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:42:26.542470 pycheck_domain-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-15 14:42:15.000000 pycheck_domain-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-15 14:42:26.542470 pycheck_domain-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-15 14:42:15.000000 pycheck_domain-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:42:26.542470 pycheck_domain-1.0.0/pycheck_domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:42:15.000000 pycheck_domain-1.0.0/pycheck_domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-15 14:42:15.000000 pycheck_domain-1.0.0/pycheck_domain/check_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:42:26.542470 pycheck_domain-1.0.0/pycheck_domain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-15 14:42:26.000000 pycheck_domain-1.0.0/pycheck_domain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-15 14:42:26.000000 pycheck_domain-1.0.0/pycheck_domain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:42:26.000000 pycheck_domain-1.0.0/pycheck_domain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-15 14:42:26.000000 pycheck_domain-1.0.0/pycheck_domain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-15 14:42:26.000000 pycheck_domain-1.0.0/pycheck_domain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:42:26.000000 pycheck_domain-1.0.0/pycheck_domain.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 14:42:26.542470 pycheck_domain-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-15 14:42:15.000000 pycheck_domain-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:36:36.876247 pycheck_domain-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-02 14:36:28.000000 pycheck_domain-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-02 14:36:36.876247 pycheck_domain-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-02 14:36:28.000000 pycheck_domain-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:36:36.872247 pycheck_domain-1.0.1/pycheck_domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:36:28.000000 pycheck_domain-1.0.1/pycheck_domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-02 14:36:28.000000 pycheck_domain-1.0.1/pycheck_domain/check_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:36:36.876247 pycheck_domain-1.0.1/pycheck_domain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-02 14:36:36.000000 pycheck_domain-1.0.1/pycheck_domain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-02 14:36:36.000000 pycheck_domain-1.0.1/pycheck_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:36:36.000000 pycheck_domain-1.0.1/pycheck_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 14:36:36.000000 pycheck_domain-1.0.1/pycheck_domain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 14:36:36.000000 pycheck_domain-1.0.1/pycheck_domain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:36:36.000000 pycheck_domain-1.0.1/pycheck_domain.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:36:36.876247 pycheck_domain-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-02 14:36:28.000000 pycheck_domain-1.0.1/setup.py
```

### Comparing `pycheck_domain-1.0.0/LICENSE` & `pycheck_domain-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycheck_domain-1.0.0/setup.py` & `pycheck_domain-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with io.open("requirements.txt", 'r') as f:
     install_requires = f.read().split(os.sep)
 
 
 setup(
     name='pycheck_domain',
-    version='1.0.0',
+    version='1.0.1',
     description='域名助手',
     author='buyfakett',
     author_email='buyfakett@vip.qq.com',
     license='MIT',
     url="https://github.com/buyfakett",
     packages=find_packages(),  # packages=["pytest"],
     long_description=long_description,
```

