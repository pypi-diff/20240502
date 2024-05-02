# Comparing `tmp/nonebot_plugin_kawaii_status-0.1.4.tar.gz` & `tmp/nonebot_plugin_kawaii_status-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kawaii_status-0.1.4.tar", last modified: Sat Apr 20 08:43:36 2024, max compression
+gzip compressed data, was "nonebot_plugin_kawaii_status-0.1.5.tar", last modified: Thu May  2 14:34:09 2024, max compression
```

## Comparing `nonebot_plugin_kawaii_status-0.1.4.tar` & `nonebot_plugin_kawaii_status-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/LICENSE
--rw-r--r--   0        0        0     2326 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/README.md
--rw-r--r--   0        0        0     1511 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/__init__.py
--rw-r--r--   0        0        0      669 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/color.py
--rw-r--r--   0        0        0      369 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/config.py
--rw-r--r--   0        0        0     3965 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/drawer.py
--rw-r--r--   0        0        0     2029 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/model.py
--rw-r--r--   0        0        0      427 2024-04-20 08:43:11.718305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/path.py
--rw-r--r--   0        0        0    96904 2024-04-20 08:43:11.722305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/ADLaMDisplay-Regular.ttf
--rw-r--r--   0        0        0    65816 2024-04-20 08:43:11.722305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/SpicyRice-Regular.ttf
--rw-r--r--   0        0        0  6227568 2024-04-20 08:43:11.758305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/baotu.ttf
--rw-r--r--   0        0        0   603174 2024-04-20 08:43:11.762305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/images/background.png
--rw-r--r--   0        0        0     4863 2024-04-20 08:43:11.762305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/images/marker.png
--rw-r--r--   0        0        0      385 2024-04-20 08:43:11.762305 nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/utils.py
--rw-r--r--   0        0        0     1456 2024-04-20 08:43:36.594742 nonebot_plugin_kawaii_status-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 nonebot_plugin_kawaii_status-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-02 14:33:42.528258 nonebot_plugin_kawaii_status-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2326 2024-05-02 14:33:42.528258 nonebot_plugin_kawaii_status-0.1.5/README.md
+-rw-r--r--   0        0        0     1511 2024-05-02 14:33:42.532258 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-02 14:33:42.532258 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/color.py
+-rw-r--r--   0        0        0      369 2024-05-02 14:33:42.532258 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/config.py
+-rw-r--r--   0        0        0     3988 2024-05-02 14:33:42.532258 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/drawer.py
+-rw-r--r--   0        0        0     2029 2024-05-02 14:33:42.532258 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/model.py
+-rw-r--r--   0        0        0      427 2024-05-02 14:33:42.532258 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/path.py
+-rw-r--r--   0        0        0    96904 2024-05-02 14:33:42.532258 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/resources/fonts/ADLaMDisplay-Regular.ttf
+-rw-r--r--   0        0        0    65816 2024-05-02 14:33:42.532258 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/resources/fonts/SpicyRice-Regular.ttf
+-rw-r--r--   0        0        0  6227568 2024-05-02 14:33:42.572259 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/resources/fonts/baotu.ttf
+-rw-r--r--   0        0        0   603174 2024-05-02 14:33:42.572259 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/resources/images/background.png
+-rw-r--r--   0        0        0     4863 2024-05-02 14:33:42.572259 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/resources/images/marker.png
+-rw-r--r--   0        0        0      385 2024-05-02 14:33:42.572259 nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/utils.py
+-rw-r--r--   0        0        0     1456 2024-05-02 14:34:09.132528 nonebot_plugin_kawaii_status-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 nonebot_plugin_kawaii_status-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_kawaii_status-0.1.4/LICENSE` & `nonebot_plugin_kawaii_status-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.4/README.md` & `nonebot_plugin_kawaii_status-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/__init__.py` & `nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 require("nonebot_plugin_alconna")
 from nonebot_plugin_alconna import Command
 from nonebot_plugin_alconna.uniseg import UniMessage
 
 from .config import Config, ScopedConfig
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 __plugin_meta__ = PluginMetadata(
     name="运行状态",
     description="NoneBot2 服务器状态查看插件",
     usage="/status",
     type="application",
     homepage="https://github.com/KomoriDev/nonebot-plugin-kawaii-status",
     config=Config,
```

### Comparing `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/color.py` & `nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/color.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/drawer.py` & `nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             (352, 1378),
             f"{truncate_string(cpuinfo.get_cpu_info()['brand_raw'])}",
             font=adlam_fnt,
             fill=details_color,
         )
         content.text(
             (352, 1431),
-            f"{system.system} {system.release}",
+            f"{truncate_string(system.system + ' ' + system.release)}",
             font=adlam_fnt,
             fill=details_color,
         )
         content.text(
             (352, 1484),
             f"NoneBot {__nb_version__} x Plugin {__status_version__}",
             font=adlam_fnt,
```

### Comparing `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/model.py` & `nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/ADLaMDisplay-Regular.ttf` & `nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/resources/fonts/ADLaMDisplay-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/SpicyRice-Regular.ttf` & `nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/resources/fonts/SpicyRice-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/fonts/baotu.ttf` & `nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/resources/fonts/baotu.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/images/background.png` & `nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/resources/images/background.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.4/nonebot_plugin_kawaii_status/resources/images/marker.png` & `nonebot_plugin_kawaii_status-0.1.5/nonebot_plugin_kawaii_status/resources/images/marker.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_status-0.1.4/pyproject.toml` & `nonebot_plugin_kawaii_status-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-kawaii-status"
-version = "0.1.4"
+version = "0.1.5"
 description = "NoneBot2 服务器状态查看插件 / View server status for NoneBot2"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
     { name = "KomoriDev", email = "mute231010@gmail.com" },
 ]
 dependencies = [
```

### Comparing `nonebot_plugin_kawaii_status-0.1.4/PKG-INFO` & `nonebot_plugin_kawaii_status-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-kawaii-status
-Version: 0.1.4
+Version: 0.1.5
 Summary: NoneBot2 服务器状态查看插件 / View server status for NoneBot2
 Home-page: https://github.com/KomoriDev/nonebot-plugin-kawaii-status
 Author-Email: KomoriDev <mute231010@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/KomoriDev/nonebot-plugin-kawaii-status
 Project-URL: Repository, https://github.com/KomoriDev/nonebot-plugin-kawaii-status
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-kawaii-status Version: 0.1.4
+Metadata-Version: 2.1 Name: nonebot-plugin-kawaii-status Version: 0.1.5
 Summary: NoneBot2 æå¡å¨ç¶ææ¥çæä»¶ / View server status for NoneBot2
 Home-page: https://github.com/KomoriDev/nonebot-plugin-kawaii-status Author-
 Email: KomoriDev
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/KomoriDev/
 nonebot-plugin-kawaii-status Project-URL: Repository, https://github.com/
 KomoriDev/nonebot-plugin-kawaii-status Requires-Python: >=3.8 Requires-Dist:
 nonebot-plugin-alconna>=0.37.0 Requires-Dist: psutil>=5.9.8 Requires-Dist:
```

