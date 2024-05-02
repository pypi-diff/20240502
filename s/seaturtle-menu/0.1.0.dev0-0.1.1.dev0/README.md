# Comparing `tmp/seaturtle_menu-0.1.0.dev0.tar.gz` & `tmp/seaturtle_menu-0.1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaturtle_menu-0.1.0.dev0.tar", last modified: Thu May  2 17:40:35 2024, max compression
+gzip compressed data, was "seaturtle_menu-0.1.1.dev0.tar", last modified: Thu May  2 18:12:00 2024, max compression
```

## Comparing `seaturtle_menu-0.1.0.dev0.tar` & `seaturtle_menu-0.1.1.dev0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 17:40:35.250038 seaturtle_menu-0.1.0.dev0/
--rw-rw-r--   0 tathya    (1000) tathya    (1000)     1058 2024-05-02 16:30:48.000000 seaturtle_menu-0.1.0.dev0/LICENSE
--rw-r--r--   0 tathya    (1000) tathya    (1000)      218 2024-05-02 17:40:35.250038 seaturtle_menu-0.1.0.dev0/PKG-INFO
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      377 2024-05-02 17:28:04.000000 seaturtle_menu-0.1.0.dev0/README.md
-drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 17:40:35.246039 seaturtle_menu-0.1.0.dev0/seaturtle_menu/
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      340 2024-05-02 16:30:10.000000 seaturtle_menu-0.1.0.dev0/seaturtle_menu/__init__.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)     2575 2024-05-02 16:27:02.000000 seaturtle_menu-0.1.0.dev0/seaturtle_menu/bullets.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)       81 2024-05-02 16:19:13.000000 seaturtle_menu-0.1.0.dev0/seaturtle_menu/consts.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)     3073 2024-05-02 16:38:29.000000 seaturtle_menu-0.1.0.dev0/seaturtle_menu/menu.py
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      229 2024-05-02 13:25:08.000000 seaturtle_menu-0.1.0.dev0/seaturtle_menu/utils.py
-drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 17:40:35.246039 seaturtle_menu-0.1.0.dev0/seaturtle_menu.egg-info/
--rw-r--r--   0 tathya    (1000) tathya    (1000)      218 2024-05-02 17:40:35.000000 seaturtle_menu-0.1.0.dev0/seaturtle_menu.egg-info/PKG-INFO
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      303 2024-05-02 17:40:35.000000 seaturtle_menu-0.1.0.dev0/seaturtle_menu.egg-info/SOURCES.txt
--rw-rw-r--   0 tathya    (1000) tathya    (1000)        1 2024-05-02 17:40:35.000000 seaturtle_menu-0.1.0.dev0/seaturtle_menu.egg-info/dependency_links.txt
--rw-rw-r--   0 tathya    (1000) tathya    (1000)       15 2024-05-02 17:40:35.000000 seaturtle_menu-0.1.0.dev0/seaturtle_menu.egg-info/top_level.txt
--rw-rw-r--   0 tathya    (1000) tathya    (1000)       38 2024-05-02 17:40:35.250038 seaturtle_menu-0.1.0.dev0/setup.cfg
--rw-rw-r--   0 tathya    (1000) tathya    (1000)      344 2024-05-02 17:38:04.000000 seaturtle_menu-0.1.0.dev0/setup.py
+drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 18:12:00.563394 seaturtle_menu-0.1.1.dev0/
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)     1058 2024-05-02 16:30:48.000000 seaturtle_menu-0.1.1.dev0/LICENSE
+-rw-r--r--   0 tathya    (1000) tathya    (1000)     2148 2024-05-02 18:12:00.563394 seaturtle_menu-0.1.1.dev0/PKG-INFO
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      377 2024-05-02 17:28:04.000000 seaturtle_menu-0.1.1.dev0/README.md
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      761 2024-05-02 18:07:14.000000 seaturtle_menu-0.1.1.dev0/pyproject.toml
+drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 18:12:00.559394 seaturtle_menu-0.1.1.dev0/seaturtle_menu/
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      341 2024-05-02 18:07:26.000000 seaturtle_menu-0.1.1.dev0/seaturtle_menu/__init__.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)     2575 2024-05-02 16:27:02.000000 seaturtle_menu-0.1.1.dev0/seaturtle_menu/bullets.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)       81 2024-05-02 16:19:13.000000 seaturtle_menu-0.1.1.dev0/seaturtle_menu/consts.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)     3073 2024-05-02 16:38:29.000000 seaturtle_menu-0.1.1.dev0/seaturtle_menu/menu.py
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      229 2024-05-02 13:25:08.000000 seaturtle_menu-0.1.1.dev0/seaturtle_menu/utils.py
+drwxrwxr-x   0 tathya    (1000) tathya    (1000)        0 2024-05-02 18:12:00.563394 seaturtle_menu-0.1.1.dev0/seaturtle_menu.egg-info/
+-rw-r--r--   0 tathya    (1000) tathya    (1000)     2148 2024-05-02 18:12:00.000000 seaturtle_menu-0.1.1.dev0/seaturtle_menu.egg-info/PKG-INFO
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      318 2024-05-02 18:12:00.000000 seaturtle_menu-0.1.1.dev0/seaturtle_menu.egg-info/SOURCES.txt
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)        1 2024-05-02 18:12:00.000000 seaturtle_menu-0.1.1.dev0/seaturtle_menu.egg-info/dependency_links.txt
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)       15 2024-05-02 18:12:00.000000 seaturtle_menu-0.1.1.dev0/seaturtle_menu.egg-info/top_level.txt
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)       38 2024-05-02 18:12:00.563394 seaturtle_menu-0.1.1.dev0/setup.cfg
+-rw-rw-r--   0 tathya    (1000) tathya    (1000)      671 2024-05-02 18:07:09.000000 seaturtle_menu-0.1.1.dev0/setup.py
```

### Comparing `seaturtle_menu-0.1.0.dev0/LICENSE` & `seaturtle_menu-0.1.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `seaturtle_menu-0.1.0.dev0/seaturtle_menu/bullets.py` & `seaturtle_menu-0.1.1.dev0/seaturtle_menu/bullets.py`

 * *Files identical despite different names*

### Comparing `seaturtle_menu-0.1.0.dev0/seaturtle_menu/menu.py` & `seaturtle_menu-0.1.1.dev0/seaturtle_menu/menu.py`

 * *Files identical despite different names*

