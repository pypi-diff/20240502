# Comparing `tmp/zoltraak-0.1.8.tar.gz` & `tmp/zoltraak-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoltraak-0.1.8.tar", last modified: Wed Apr 24 07:27:13 2024, max compression
+gzip compressed data, was "zoltraak-0.1.9.tar", last modified: Wed Apr 24 07:32:45 2024, max compression
```

## Comparing `zoltraak-0.1.8.tar` & `zoltraak-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.763677 zoltraak-0.1.8/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 07:27:13.763539 zoltraak-0.1.8/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    50235 2024-04-24 03:41:33.000000 zoltraak-0.1.8/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-04-24 07:27:13.763714 zoltraak-0.1.8/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      522 2024-04-24 07:27:12.000000 zoltraak-0.1.8/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.757951 zoltraak-0.1.8/zoltraak/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-15 18:33:00.000000 zoltraak-0.1.8/zoltraak/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5713 2024-04-24 06:17:03.000000 zoltraak-0.1.8/zoltraak/cli.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    17101 2024-04-24 03:11:27.000000 zoltraak-0.1.8/zoltraak/converter.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.758321 zoltraak-0.1.8/zoltraak/llms/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1065 2024-04-21 23:52:43.000000 zoltraak-0.1.8/zoltraak/llms/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      946 2024-04-16 05:55:37.000000 zoltraak-0.1.8/zoltraak/llms/claude.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    10617 2024-04-24 06:37:12.000000 zoltraak-0.1.8/zoltraak/md_generator.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.757023 zoltraak-0.1.8/zoltraak/setting/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.758496 zoltraak-0.1.8/zoltraak/setting/architect/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      183 2024-04-24 03:01:15.000000 zoltraak-0.1.8/zoltraak/setting/architect/architect.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.760528 zoltraak-0.1.8/zoltraak/setting/compiler/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     7114 2024-04-22 10:16:30.000000 zoltraak-0.1.8/zoltraak/setting/compiler/biz_consult copy.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3766 2024-04-22 10:21:52.000000 zoltraak-0.1.8/zoltraak/setting/compiler/biz_consult.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1093 2024-04-22 00:24:25.000000 zoltraak-0.1.8/zoltraak/setting/compiler/dev_akirapp.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       69 2024-04-22 23:55:14.000000 zoltraak-0.1.8/zoltraak/setting/compiler/dev_front.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1463 2024-04-22 00:24:12.000000 zoltraak-0.1.8/zoltraak/setting/compiler/dev_func.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2302 2024-04-22 10:10:26.000000 zoltraak-0.1.8/zoltraak/setting/compiler/dev_obj.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1413 2024-04-22 00:43:30.000000 zoltraak-0.1.8/zoltraak/setting/compiler/dev_obj_lisp.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2759 2024-04-22 00:47:40.000000 zoltraak-0.1.8/zoltraak/setting/compiler/dev_obj_lisp_g.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2221 2024-04-22 00:56:55.000000 zoltraak-0.1.8/zoltraak/setting/compiler/dev_obj_lisp_g_base64.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      100 2024-04-21 22:59:42.000000 zoltraak-0.1.8/zoltraak/setting/compiler/encode_lisp.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      447 2024-04-22 16:38:24.000000 zoltraak-0.1.8/zoltraak/setting/compiler/general_def.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3832 2024-04-21 23:02:20.000000 zoltraak-0.1.8/zoltraak/setting/compiler/general_reqdef.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      772 2024-04-24 02:39:26.000000 zoltraak-0.1.8/zoltraak/setting/compiler/ref_create_directory.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.760650 zoltraak-0.1.8/zoltraak/setting/developer/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 03:16:20.000000 zoltraak-0.1.8/zoltraak/setting/developer/dev_python.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.760965 zoltraak-0.1.8/zoltraak/setting/encryption/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      432 2024-04-21 18:24:02.000000 zoltraak-0.1.8/zoltraak/setting/encryption/emoji.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.761523 zoltraak-0.1.8/zoltraak/setting/formatter/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      118 2024-04-21 18:10:10.000000 zoltraak-0.1.8/zoltraak/setting/formatter/md_comment.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      193 2024-04-21 18:04:36.000000 zoltraak-0.1.8/zoltraak/setting/formatter/py_comment.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.761643 zoltraak-0.1.8/zoltraak/setting/interpretspec/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4799 2024-04-21 18:35:46.000000 zoltraak-0.1.8/zoltraak/setting/interpretspec/hirokichi.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:27:13.762439 zoltraak-0.1.8/zoltraak.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 07:27:13.000000 zoltraak-0.1.8/zoltraak.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2126 2024-04-24 07:27:13.000000 zoltraak-0.1.8/zoltraak.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-04-24 07:27:13.000000 zoltraak-0.1.8/zoltraak.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-04-24 07:27:13.000000 zoltraak-0.1.8/zoltraak.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       17 2024-04-24 07:27:13.000000 zoltraak-0.1.8/zoltraak.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        9 2024-04-24 07:27:13.000000 zoltraak-0.1.8/zoltraak.egg-info/top_level.txt
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.248842 zoltraak-0.1.9/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 07:32:45.248698 zoltraak-0.1.9/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    50235 2024-04-24 03:41:33.000000 zoltraak-0.1.9/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-04-24 07:32:45.248876 zoltraak-0.1.9/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      861 2024-04-24 07:32:44.000000 zoltraak-0.1.9/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.241591 zoltraak-0.1.9/zoltraak/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-15 18:33:00.000000 zoltraak-0.1.9/zoltraak/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5713 2024-04-24 06:17:03.000000 zoltraak-0.1.9/zoltraak/cli.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    17101 2024-04-24 03:11:27.000000 zoltraak-0.1.9/zoltraak/converter.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.242059 zoltraak-0.1.9/zoltraak/llms/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1065 2024-04-21 23:52:43.000000 zoltraak-0.1.9/zoltraak/llms/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      946 2024-04-16 05:55:37.000000 zoltraak-0.1.9/zoltraak/llms/claude.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    10617 2024-04-24 07:31:57.000000 zoltraak-0.1.9/zoltraak/md_generator.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.240169 zoltraak-0.1.9/zoltraak/setting/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.242347 zoltraak-0.1.9/zoltraak/setting/architect/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      183 2024-04-24 03:01:15.000000 zoltraak-0.1.9/zoltraak/setting/architect/architect.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.246224 zoltraak-0.1.9/zoltraak/setting/compiler/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     7114 2024-04-22 10:16:30.000000 zoltraak-0.1.9/zoltraak/setting/compiler/biz_consult copy.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3766 2024-04-22 10:21:52.000000 zoltraak-0.1.9/zoltraak/setting/compiler/biz_consult.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1093 2024-04-22 00:24:25.000000 zoltraak-0.1.9/zoltraak/setting/compiler/dev_akirapp.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       69 2024-04-22 23:55:14.000000 zoltraak-0.1.9/zoltraak/setting/compiler/dev_front.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1463 2024-04-22 00:24:12.000000 zoltraak-0.1.9/zoltraak/setting/compiler/dev_func.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2302 2024-04-22 10:10:26.000000 zoltraak-0.1.9/zoltraak/setting/compiler/dev_obj.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1413 2024-04-22 00:43:30.000000 zoltraak-0.1.9/zoltraak/setting/compiler/dev_obj_lisp.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2759 2024-04-22 00:47:40.000000 zoltraak-0.1.9/zoltraak/setting/compiler/dev_obj_lisp_g.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2221 2024-04-22 00:56:55.000000 zoltraak-0.1.9/zoltraak/setting/compiler/dev_obj_lisp_g_base64.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      100 2024-04-21 22:59:42.000000 zoltraak-0.1.9/zoltraak/setting/compiler/encode_lisp.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      447 2024-04-22 16:38:24.000000 zoltraak-0.1.9/zoltraak/setting/compiler/general_def.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3832 2024-04-21 23:02:20.000000 zoltraak-0.1.9/zoltraak/setting/compiler/general_reqdef.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      772 2024-04-24 02:39:26.000000 zoltraak-0.1.9/zoltraak/setting/compiler/ref_create_directory.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.246324 zoltraak-0.1.9/zoltraak/setting/developer/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 03:16:20.000000 zoltraak-0.1.9/zoltraak/setting/developer/dev_python.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.246410 zoltraak-0.1.9/zoltraak/setting/encryption/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      432 2024-04-21 18:24:02.000000 zoltraak-0.1.9/zoltraak/setting/encryption/emoji.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.246901 zoltraak-0.1.9/zoltraak/setting/formatter/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      118 2024-04-21 18:10:10.000000 zoltraak-0.1.9/zoltraak/setting/formatter/md_comment.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      193 2024-04-21 18:04:36.000000 zoltraak-0.1.9/zoltraak/setting/formatter/py_comment.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.247105 zoltraak-0.1.9/zoltraak/setting/interpretspec/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4799 2024-04-21 18:35:46.000000 zoltraak-0.1.9/zoltraak/setting/interpretspec/hirokichi.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:32:45.248023 zoltraak-0.1.9/zoltraak.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 07:32:45.000000 zoltraak-0.1.9/zoltraak.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2126 2024-04-24 07:32:45.000000 zoltraak-0.1.9/zoltraak.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-04-24 07:32:45.000000 zoltraak-0.1.9/zoltraak.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-04-24 07:32:45.000000 zoltraak-0.1.9/zoltraak.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       17 2024-04-24 07:32:45.000000 zoltraak-0.1.9/zoltraak.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        9 2024-04-24 07:32:45.000000 zoltraak-0.1.9/zoltraak.egg-info/top_level.txt
```

### Comparing `zoltraak-0.1.8/README.md` & `zoltraak-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/cli.py` & `zoltraak-0.1.9/zoltraak/cli.py`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/converter.py` & `zoltraak-0.1.9/zoltraak/converter.py`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/llms/claude.py` & `zoltraak-0.1.9/zoltraak/llms/claude.py`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/llms/claude.txt` & `zoltraak-0.1.9/zoltraak/llms/claude.txt`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/md_generator.py` & `zoltraak-0.1.9/zoltraak/md_generator.py`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/compiler/biz_consult copy.md` & `zoltraak-0.1.9/zoltraak/setting/compiler/biz_consult copy.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/compiler/biz_consult.md` & `zoltraak-0.1.9/zoltraak/setting/compiler/biz_consult.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/compiler/dev_akirapp.md` & `zoltraak-0.1.9/zoltraak/setting/compiler/dev_akirapp.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/compiler/dev_func.md` & `zoltraak-0.1.9/zoltraak/setting/compiler/dev_func.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/compiler/dev_obj.md` & `zoltraak-0.1.9/zoltraak/setting/compiler/dev_obj.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/compiler/dev_obj_lisp.md` & `zoltraak-0.1.9/zoltraak/setting/compiler/dev_obj_lisp.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/compiler/dev_obj_lisp_g.md` & `zoltraak-0.1.9/zoltraak/setting/compiler/dev_obj_lisp_g.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/compiler/dev_obj_lisp_g_base64.md` & `zoltraak-0.1.9/zoltraak/setting/compiler/dev_obj_lisp_g_base64.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/compiler/general_reqdef.md` & `zoltraak-0.1.9/zoltraak/setting/compiler/general_reqdef.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/compiler/ref_create_directory.py` & `zoltraak-0.1.9/zoltraak/setting/compiler/ref_create_directory.py`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak/setting/interpretspec/hirokichi.md` & `zoltraak-0.1.9/zoltraak/setting/interpretspec/hirokichi.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.8/zoltraak.egg-info/SOURCES.txt` & `zoltraak-0.1.9/zoltraak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

