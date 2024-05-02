# Comparing `tmp/nonebot_plugin_chikari_yinpa-1.4.0.tar.gz` & `tmp/nonebot_plugin_chikari_yinpa-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chikari_yinpa-1.4.0.tar", last modified: Tue Apr 30 10:05:47 2024, max compression
+gzip compressed data, was "nonebot_plugin_chikari_yinpa-1.4.1.tar", last modified: Thu May  2 07:38:40 2024, max compression
```

## Comparing `nonebot_plugin_chikari_yinpa-1.4.0.tar` & `nonebot_plugin_chikari_yinpa-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 10:05:47.306381 nonebot_plugin_chikari_yinpa-1.4.0/
--rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_yinpa-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     4734 2024-04-30 10:05:47.305405 nonebot_plugin_chikari_yinpa-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4033 2024-03-16 14:39:20.000000 nonebot_plugin_chikari_yinpa-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 10:05:47.297597 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/
--rw-rw-rw-   0        0        0     2835 2024-04-30 10:05:25.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/__init__.py
--rw-rw-rw-   0        0        0      684 2024-02-17 04:46:31.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/config.py
--rw-rw-rw-   0        0        0     6161 2024-04-30 09:36:41.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/data_handles.py
--rw-rw-rw-   0        0        0    15078 2024-04-30 09:40:40.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/dicts.py
--rw-rw-rw-   0        0        0    36824 2024-04-30 10:05:10.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/handles.py
--rw-rw-rw-   0        0        0    27358 2024-04-30 09:41:35.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 10:05:47.304429 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/
--rw-rw-rw-   0        0        0     4734 2024-04-30 10:05:47.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2024-04-30 10:05:47.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 10:05:47.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-30 10:05:47.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-30 10:05:47.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-30 10:05:47.307357 nonebot_plugin_chikari_yinpa-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      783 2024-04-30 10:05:28.000000 nonebot_plugin_chikari_yinpa-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:38:40.070546 nonebot_plugin_chikari_yinpa-1.4.1/
+-rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_yinpa-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     4734 2024-05-02 07:38:40.070546 nonebot_plugin_chikari_yinpa-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4033 2024-03-16 14:39:20.000000 nonebot_plugin_chikari_yinpa-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 07:38:40.063565 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/
+-rw-rw-rw-   0        0        0     2835 2024-05-02 07:37:12.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-02-17 04:46:31.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/config.py
+-rw-rw-rw-   0        0        0     6161 2024-04-30 09:36:41.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/data_handles.py
+-rw-rw-rw-   0        0        0    15078 2024-04-30 09:40:40.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/dicts.py
+-rw-rw-rw-   0        0        0    36831 2024-05-02 07:36:50.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/handles.py
+-rw-rw-rw-   0        0        0    27358 2024-04-30 09:41:35.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:38:40.069549 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa.egg-info/
+-rw-rw-rw-   0        0        0     4734 2024-05-02 07:38:40.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2024-05-02 07:38:40.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 07:38:40.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-02 07:38:40.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-02 07:38:40.000000 nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-02 07:38:40.071544 nonebot_plugin_chikari_yinpa-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      783 2024-05-02 07:37:13.000000 nonebot_plugin_chikari_yinpa-1.4.1/setup.py
```

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/LICENSE` & `nonebot_plugin_chikari_yinpa-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/PKG-INFO` & `nonebot_plugin_chikari_yinpa-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_yinpa
-Version: 1.4.0
+Version: 1.4.1
 Summary: A plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.4.0
+Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.4.1
 Summary: A plugin for nonebot 2 Home-page: https://github.com/mrqx0195/
 nonebot_plugin_chikari_yinpa Author: mrqx0195 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pillow Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
```

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/README.md` & `nonebot_plugin_chikari_yinpa-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/__init__.py` & `nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     usage="",
     config=Config,
     type="application",
     homepage="https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa",
     supported_adapters={"~onebot.v11"}
 )
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 on_yinpa_control = on_command(
     "yinpa_control",
     aliases={"银趴控制"},
     permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
     priority=10,
     block=False,
```

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/config.py` & `nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/data_handles.py` & `nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/data_handles.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/dicts.py` & `nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/dicts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/handles.py` & `nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/handles.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             await matcher.finish("本群银趴已禁用，你不准参加银趴！")
         if Utils.yinpa_user_presence_check(event.get_user_id()):
             await matcher.finish("您已加入银趴！\n如果想要重置银趴数据，请使用 /leave_yinpa 或 /离开银趴 离开银趴后再加入")
         uid: str = event.get_user_id()
         command: str = args.extract_plain_text()
         arg_list: list = command.split()
         if not len(arg_list) == 2:
-            bot = get_bots()[event.self_id]
+            bot = get_bots()[(str)(event.self_id)]
             name: str = bot.call_api("get_group_member_info",group_id = event.group_id,user_id = uid)["nickname"]
         else:
             name: str = arg_list[0]
         if (int)(arg_list[1]) <= 0:
             species: int = Utils.dice(7,event.get_user_id())
         else:
             if not arg_list[1].isdigit():
```

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/utils.py` & `nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO` & `nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_yinpa
-Version: 1.4.0
+Version: 1.4.1
 Summary: A plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.4.0
+Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.4.1
 Summary: A plugin for nonebot 2 Home-page: https://github.com/mrqx0195/
 nonebot_plugin_chikari_yinpa Author: mrqx0195 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pillow Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
```

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt` & `nonebot_plugin_chikari_yinpa-1.4.1/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.4.0/setup.py` & `nonebot_plugin_chikari_yinpa-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_chikari_yinpa",
-    version="1.4.0",
+    version="1.4.1",
     author="mrqx0195",
     author_email="2317249571@qq.com",
     description="A plugin for nonebot 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa",
     packages=setuptools.find_packages(),
```

