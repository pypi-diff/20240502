# Comparing `tmp/mama-0.9.5.tar.gz` & `tmp/mama-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mama-0.9.5.tar", last modified: Wed May  1 11:07:00 2024, max compression
+gzip compressed data, was "mama-0.9.6.tar", last modified: Wed May  1 12:05:01 2024, max compression
```

## Comparing `mama-0.9.5.tar` & `mama-0.9.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2022-10-15 13:42:02.000000 mama-0.9.5/LICENSE
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-01 11:07:00.778757 mama-0.9.5/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11351 2024-02-02 11:55:24.000000 mama-0.9.5/README.md
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/mama/
--rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2022-10-15 12:52:32.000000 mama-0.9.5/mama/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11805 2024-03-24 12:54:08.000000 mama-0.9.5/mama/artifactory.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    40005 2024-05-01 11:06:08.000000 mama-0.9.5/mama/build_config.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    24912 2024-03-24 13:57:15.000000 mama-0.9.5/mama/build_dependency.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    55602 2024-05-01 11:06:10.000000 mama-0.9.5/mama/build_target.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11779 2024-03-26 11:44:52.000000 mama-0.9.5/mama/cmake_configure.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    16670 2024-05-01 11:06:08.000000 mama-0.9.5/mama/dependency_chain.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2022-10-14 21:28:27.000000 mama-0.9.5/mama/init_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12378 2024-02-20 10:18:01.000000 mama-0.9.5/mama/main.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2022-10-14 21:35:20.000000 mama-0.9.5/mama/msbuild.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     9665 2024-05-01 11:06:08.000000 mama-0.9.5/mama/package.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     7757 2024-03-24 13:37:47.000000 mama-0.9.5/mama/papa_deploy.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3778 2024-03-24 22:17:15.000000 mama-0.9.5/mama/papa_upload.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1763 2024-03-24 13:50:55.000000 mama-0.9.5/mama/parse_mamafile.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/mama/platforms/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-10 12:13:25.000000 mama-0.9.5/mama/platforms/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     8558 2023-08-24 17:06:29.000000 mama-0.9.5/mama/platforms/android.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5376 2023-10-05 15:21:24.000000 mama-0.9.5/mama/platforms/mips.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5644 2024-01-24 19:36:51.000000 mama-0.9.5/mama/platforms/oclea.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/mama/types/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:55.000000 mama-0.9.5/mama/types/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-31 19:23:36.000000 mama-0.9.5/mama/types/artifactory_pkg.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2024-03-24 13:38:20.000000 mama-0.9.5/mama/types/asset.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-31 19:23:36.000000 mama-0.9.5/mama/types/dep_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    15161 2024-04-01 21:45:25.000000 mama-0.9.5/mama/types/git.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2022-10-13 16:33:15.000000 mama-0.9.5/mama/types/local_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    17510 2024-03-24 21:19:55.000000 mama-0.9.5/mama/util.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/mama/utils/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:54.000000 mama-0.9.5/mama/utils/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1637 2023-10-14 09:10:27.000000 mama-0.9.5/mama/utils/gdb.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    17034 2024-03-24 13:15:53.000000 mama-0.9.5/mama/utils/gnu_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      923 2023-10-14 09:10:17.000000 mama-0.9.5/mama/utils/gtest.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2022-10-14 18:37:11.000000 mama-0.9.5/mama/utils/nonblocking_io.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3789 2024-05-01 11:06:08.000000 mama-0.9.5/mama/utils/run.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    10345 2024-03-26 12:29:05.000000 mama-0.9.5/mama/utils/sub_process.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1245 2024-05-01 11:06:08.000000 mama-0.9.5/mama/utils/system.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/mama.egg-info/
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)      921 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/SOURCES.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/dependency_links.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/entry_points.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/requires.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/top_level.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2024-05-01 11:06:15.000000 mama-0.9.5/pyproject.toml
--rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2024-05-01 11:07:00.778757 mama-0.9.5/setup.cfg
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 12:05:01.607053 mama-0.9.6/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2022-10-15 13:42:02.000000 mama-0.9.6/LICENSE
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-01 12:05:01.607053 mama-0.9.6/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11351 2024-02-02 11:55:24.000000 mama-0.9.6/README.md
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 12:05:01.597053 mama-0.9.6/mama/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2022-10-15 12:52:32.000000 mama-0.9.6/mama/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11805 2024-03-24 12:54:08.000000 mama-0.9.6/mama/artifactory.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    40004 2024-05-01 12:04:54.000000 mama-0.9.6/mama/build_config.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    24912 2024-03-24 13:57:15.000000 mama-0.9.6/mama/build_dependency.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    55602 2024-05-01 11:06:10.000000 mama-0.9.6/mama/build_target.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11779 2024-03-26 11:44:52.000000 mama-0.9.6/mama/cmake_configure.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    16670 2024-05-01 11:06:08.000000 mama-0.9.6/mama/dependency_chain.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2022-10-14 21:28:27.000000 mama-0.9.6/mama/init_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12378 2024-02-20 10:18:01.000000 mama-0.9.6/mama/main.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2022-10-14 21:35:20.000000 mama-0.9.6/mama/msbuild.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     9665 2024-05-01 11:06:08.000000 mama-0.9.6/mama/package.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     7757 2024-03-24 13:37:47.000000 mama-0.9.6/mama/papa_deploy.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3778 2024-03-24 22:17:15.000000 mama-0.9.6/mama/papa_upload.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1763 2024-03-24 13:50:55.000000 mama-0.9.6/mama/parse_mamafile.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 12:05:01.597053 mama-0.9.6/mama/platforms/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-10 12:13:25.000000 mama-0.9.6/mama/platforms/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     8558 2023-08-24 17:06:29.000000 mama-0.9.6/mama/platforms/android.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5376 2023-10-05 15:21:24.000000 mama-0.9.6/mama/platforms/mips.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5644 2024-01-24 19:36:51.000000 mama-0.9.6/mama/platforms/oclea.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 12:05:01.597053 mama-0.9.6/mama/types/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:55.000000 mama-0.9.6/mama/types/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-31 19:23:36.000000 mama-0.9.6/mama/types/artifactory_pkg.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2024-03-24 13:38:20.000000 mama-0.9.6/mama/types/asset.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-31 19:23:36.000000 mama-0.9.6/mama/types/dep_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    15161 2024-04-01 21:45:25.000000 mama-0.9.6/mama/types/git.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2022-10-13 16:33:15.000000 mama-0.9.6/mama/types/local_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    17510 2024-03-24 21:19:55.000000 mama-0.9.6/mama/util.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 12:05:01.607053 mama-0.9.6/mama/utils/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:54.000000 mama-0.9.6/mama/utils/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1637 2023-10-14 09:10:27.000000 mama-0.9.6/mama/utils/gdb.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    17034 2024-03-24 13:15:53.000000 mama-0.9.6/mama/utils/gnu_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      923 2023-10-14 09:10:17.000000 mama-0.9.6/mama/utils/gtest.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2022-10-14 18:37:11.000000 mama-0.9.6/mama/utils/nonblocking_io.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3789 2024-05-01 11:06:08.000000 mama-0.9.6/mama/utils/run.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    10345 2024-03-26 12:29:05.000000 mama-0.9.6/mama/utils/sub_process.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1288 2024-05-01 12:04:54.000000 mama-0.9.6/mama/utils/system.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 12:05:01.607053 mama-0.9.6/mama.egg-info/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-01 12:05:01.000000 mama-0.9.6/mama.egg-info/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      921 2024-05-01 12:05:01.000000 mama-0.9.6/mama.egg-info/SOURCES.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2024-05-01 12:05:01.000000 mama-0.9.6/mama.egg-info/dependency_links.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2024-05-01 12:05:01.000000 mama-0.9.6/mama.egg-info/entry_points.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2024-05-01 12:05:01.000000 mama-0.9.6/mama.egg-info/requires.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2024-05-01 12:05:01.000000 mama-0.9.6/mama.egg-info/top_level.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2024-05-01 12:04:54.000000 mama-0.9.6/pyproject.toml
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2024-05-01 12:05:01.607053 mama-0.9.6/setup.cfg
```

### Comparing `mama-0.9.5/LICENSE` & `mama-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/PKG-INFO` & `mama-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.9.5
+Version: 0.9.6
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.9.5/README.md` & `mama-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/artifactory.py` & `mama-0.9.6/mama/artifactory.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/build_config.py` & `mama-0.9.6/mama/build_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
             elif self.oclea:      self.set_arch('arm64')
             elif self.mips:       self.set_arch(self.mips.mips_arch)
             else:
                 if System.aarch64:  self.set_arch('arm64')
                 elif System.x86_64: self.set_arch('x64')
                 else:               self.set_arch('x86')
 
-        # Arch itself is validated in set_arch(), 
+        # Arch itself is validated in set_arch(),
         # however we need to validate if arch is allowed on platform
         if self.arch:
             if self.linux and self.arch == 'arm':
                 raise RuntimeError(f'Unsupported arch={self.arch} on linux platform! Build with android instead')
             if self.raspi and self.arch != 'arm':
                 raise RuntimeError(f'Unsupported arch={self.arch} on raspi platform! Supported=arm')
             if self.oclea and self.arch != 'arm64':
```

### Comparing `mama-0.9.5/mama/build_dependency.py` & `mama-0.9.6/mama/build_dependency.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/build_target.py` & `mama-0.9.6/mama/build_target.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/cmake_configure.py` & `mama-0.9.6/mama/cmake_configure.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/dependency_chain.py` & `mama-0.9.6/mama/dependency_chain.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/init_project.py` & `mama-0.9.6/mama/init_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/main.py` & `mama-0.9.6/mama/main.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/msbuild.py` & `mama-0.9.6/mama/msbuild.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/package.py` & `mama-0.9.6/mama/package.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/papa_deploy.py` & `mama-0.9.6/mama/papa_deploy.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/papa_upload.py` & `mama-0.9.6/mama/papa_upload.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/parse_mamafile.py` & `mama-0.9.6/mama/parse_mamafile.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/platforms/android.py` & `mama-0.9.6/mama/platforms/android.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/platforms/mips.py` & `mama-0.9.6/mama/platforms/mips.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/platforms/oclea.py` & `mama-0.9.6/mama/platforms/oclea.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/types/artifactory_pkg.py` & `mama-0.9.6/mama/types/artifactory_pkg.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/types/asset.py` & `mama-0.9.6/mama/types/asset.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/types/dep_source.py` & `mama-0.9.6/mama/types/dep_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/types/git.py` & `mama-0.9.6/mama/types/git.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/types/local_source.py` & `mama-0.9.6/mama/types/local_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/util.py` & `mama-0.9.6/mama/util.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/utils/gdb.py` & `mama-0.9.6/mama/utils/gdb.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/utils/gnu_project.py` & `mama-0.9.6/mama/utils/gnu_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/utils/gtest.py` & `mama-0.9.6/mama/utils/gtest.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/utils/nonblocking_io.py` & `mama-0.9.6/mama/utils/nonblocking_io.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/utils/run.py` & `mama-0.9.6/mama/utils/run.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/utils/sub_process.py` & `mama-0.9.6/mama/utils/sub_process.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/mama/utils/system.py` & `mama-0.9.6/mama/utils/system.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 is_linux   = sys.platform.startswith('linux')
 is_macos   = sys.platform == 'darwin'
 if not (is_windows or is_linux or is_macos):
     raise RuntimeError(f'MamaBuild unsupported platform {sys.platform}')
 
 machine = platform.machine()
 is_aarch64 = machine == 'aarch64'
-is_x86_64 = machine == 'x86_64'
-is_x86 = machine == 'x86'
+is_x86_64 = machine == 'x86_64' or machine == 'AMD64'
+is_x86 = machine == 'x86' or machine == 'i386'
 
 class System:
     windows = is_windows
     linux   = is_linux
     macos   = is_macos
     aarch64 = is_aarch64
     x86_64  = is_x86_64
```

### Comparing `mama-0.9.5/mama.egg-info/PKG-INFO` & `mama-0.9.6/mama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.9.5
+Version: 0.9.6
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.9.5/mama.egg-info/SOURCES.txt` & `mama-0.9.6/mama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mama-0.9.5/pyproject.toml` & `mama-0.9.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mama"
-version = "0.9.5"
+version = "0.9.6"
 description = "A modular C++ build tool even your mama can use"
 license = { text = "MIT" }
 authors = [
     { name="Jorma Rebane", email="jorma.rebane@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
```

