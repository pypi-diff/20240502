# Comparing `tmp/SparkleLogging-1.0.2.tar.gz` & `tmp/SparkleLogging-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleLogging-1.0.2.tar", last modified: Wed May  1 12:15:56 2024, max compression
+gzip compressed data, was "SparkleLogging-1.0.3.tar", last modified: Thu May  2 12:12:19 2024, max compression
```

## Comparing `SparkleLogging-1.0.2.tar` & `SparkleLogging-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 12:15:56.673143 SparkleLogging-1.0.2/
--rw-rw-rw-   0        0        0     2136 2024-05-01 12:15:56.672172 SparkleLogging-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 12:15:56.647211 SparkleLogging-1.0.2/SparkleLogging/
--rw-rw-rw-   0        0        0       21 2024-04-17 12:31:27.000000 SparkleLogging-1.0.2/SparkleLogging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 12:15:56.664165 SparkleLogging-1.0.2/SparkleLogging/plugins/
--rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.2/SparkleLogging/plugins/DecoratorsTools.py
--rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.2/SparkleLogging/plugins/HttpHander.py
--rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.2/SparkleLogging/plugins/__init__.py
--rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.2/SparkleLogging/plugins/websocketHander.py
-drwxrwxrwx   0        0        0        0 2024-05-01 12:15:56.669155 SparkleLogging-1.0.2/SparkleLogging/utils/
--rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.2/SparkleLogging/utils/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-01 05:44:49.000000 SparkleLogging-1.0.2/SparkleLogging/utils/core.py
--rw-rw-rw-   0        0        0     4761 2024-05-01 05:44:46.000000 SparkleLogging-1.0.2/SparkleLogging/utils/getLog.py
--rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.2/SparkleLogging/utils/plugins_for_core.py
-drwxrwxrwx   0        0        0        0 2024-05-01 12:15:56.670151 SparkleLogging-1.0.2/SparkleLogging.egg-info/
--rw-rw-rw-   0        0        0     2136 2024-05-01 12:15:56.000000 SparkleLogging-1.0.2/SparkleLogging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-05-01 12:15:56.000000 SparkleLogging-1.0.2/SparkleLogging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 12:15:56.000000 SparkleLogging-1.0.2/SparkleLogging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-01 12:15:56.000000 SparkleLogging-1.0.2/SparkleLogging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-01 12:15:56.000000 SparkleLogging-1.0.2/SparkleLogging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 12:15:56.673143 SparkleLogging-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      724 2024-05-01 12:15:53.000000 SparkleLogging-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:12:18.920859 SparkleLogging-1.0.3/
+-rw-rw-rw-   0        0        0     2838 2024-05-02 12:12:18.918864 SparkleLogging-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 12:12:18.817911 SparkleLogging-1.0.3/SparkleLogging/
+-rw-rw-rw-   0        0        0        0 2024-05-01 12:32:10.000000 SparkleLogging-1.0.3/SparkleLogging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:12:18.907894 SparkleLogging-1.0.3/SparkleLogging/plugins/
+-rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.3/SparkleLogging/plugins/DecoratorsTools.py
+-rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.3/SparkleLogging/plugins/HttpHander.py
+-rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.3/SparkleLogging/plugins/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.3/SparkleLogging/plugins/websocketHander.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:12:18.914875 SparkleLogging-1.0.3/SparkleLogging/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.3/SparkleLogging/utils/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-05-01 05:44:49.000000 SparkleLogging-1.0.3/SparkleLogging/utils/core.py
+-rw-rw-rw-   0        0        0     4991 2024-05-02 12:07:21.000000 SparkleLogging-1.0.3/SparkleLogging/utils/getLog.py
+-rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.3/SparkleLogging/utils/plugins_for_core.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:12:18.916869 SparkleLogging-1.0.3/SparkleLogging.egg-info/
+-rw-rw-rw-   0        0        0     2838 2024-05-02 12:12:16.000000 SparkleLogging-1.0.3/SparkleLogging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-05-02 12:12:16.000000 SparkleLogging-1.0.3/SparkleLogging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 12:12:16.000000 SparkleLogging-1.0.3/SparkleLogging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-02 12:12:16.000000 SparkleLogging-1.0.3/SparkleLogging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-02 12:12:16.000000 SparkleLogging-1.0.3/SparkleLogging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 12:12:18.920859 SparkleLogging-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-05-02 12:10:40.000000 SparkleLogging-1.0.3/setup.py
```

### Comparing `SparkleLogging-1.0.2/SparkleLogging/plugins/HttpHander.py` & `SparkleLogging-1.0.3/SparkleLogging/plugins/HttpHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.2/SparkleLogging/plugins/websocketHander.py` & `SparkleLogging-1.0.3/SparkleLogging/plugins/websocketHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.2/SparkleLogging/utils/getLog.py` & `SparkleLogging-1.0.3/SparkleLogging/utils/getLog.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,18 @@
     def __init__(self) -> None:
         self.public_formatter = logging.Formatter(
             fmt='[%(asctime)s.%(msecs)d| %(levelname)-8s |%(threadName)s|%(name)s.%(funcName)s|%(filename)s:%(lineno)d]: %(message)s',
             datefmt='%Y-%m-%d %H:%M:%S'
         )
 
     def GetLogger(self, log_name: str = "default",
+                  setConsoleLevel: int = logging.DEBUG,
+                  setFileLevel: int = logging.INFO,
+                  setWebsocketLevel: int = logging.INFO,
+                  setHTTPLevel: int = logging.INFO,
                   out_to_console: bool = True,
                   web_log_mode: bool = False,
                   WSpost_url: str = "",
                   HTTPpost_url: str = "",
                   http_mode: bool = False,
                   custom_formatter: logging.Formatter = logging.Formatter(
             fmt='[%(asctime)s.%(msecs)d| %(levelname)-8s |%(threadName)s|%(name)s.%(funcName)s|%(filename)s:%(lineno)d]: %(message)s',
@@ -36,33 +40,33 @@
             'DEBUG': 'bold_blue', 'INFO': 'bold_cyan',
             'WARNING': 'bold_yellow', 'ERROR': 'red',
             'CRITICAL': 'bold_red', 'RESET': 'reset',
             'asctime': 'green'
         }
         if out_to_console:
             console_handler = logging.StreamHandler()
-            console_handler.setLevel(logging.DEBUG)
+            console_handler.setLevel(setConsoleLevel)
             console_formatter = colorlog.ColoredFormatter(
                 fmt='%(log_color)s [%(asctime)s.%(msecs)d| %(levelname)-8s |%(threadName)s|%(name)s.%(funcName)s|%(fileName)s:%(lineno)d]: %(message)s %(reset)s',
                 datefmt='%H:%M:%S',
                 log_colors=log_color_config
             )
             if custom_formatter:
                 console_formatter = custom_formatter
 
             if isinstance(console_handler, logging.StreamHandler):
                 console_formatter = colorlog.ColoredFormatter(fmt=f"%(log_color)s {console_formatter._fmt} %(reset)s",datefmt=console_formatter.datefmt, log_colors=log_color_config)
                 console_handler.setFormatter(console_formatter)
 
-            logger.setLevel(logging.DEBUG)
+            logger.setLevel(setConsoleLevel)
             logger.addHandler(console_handler)
 
         
         file_handler = TimedRotatingFileHandler(f'./logs/{log_name}/{log_name}.log',encoding="utf-8", when='midnight', interval=1, backupCount=7)
-        file_handler.setLevel(logging.INFO)
+        file_handler.setLevel(setFileLevel)
         file_handler.setFormatter(self.public_formatter)
 
         if custom_formatter:
             file_handler.setFormatter(custom_formatter)
 
         # 检查代码是否在异步环境中运行
         if asyncio.iscoroutinefunction(logging.Handler.emit):
@@ -72,33 +76,33 @@
             logger.addHandler(queue_handler)
             asyncio.ensure_future(queue_listener.start())
         else:
             logger.addHandler(file_handler)
 
         if web_log_mode and WSpost_url:
             websocket_handler = WebsocketHandler(WSpost_url)
-            websocket_handler.setLevel(logging.INFO)
+            websocket_handler.setLevel(setWebsocketLevel)
             formatter = self.public_formatter
             if custom_formatter:
                 formatter = custom_formatter
             websocket_handler.setFormatter(formatter)
             logger.addHandler(websocket_handler)
 
         if http_mode and HTTPpost_url:
             # 检查代码是否在异步环境中运行
             if asyncio.iscoroutinefunction(logging.Handler.emit):
                 async_http_hander = AsyncHTTPhandler(HTTPpost_url)
-                async_http_hander.setLevel(logging.INFO)
+                async_http_hander.setLevel(setHTTPLevel)
                 formatter = self.public_formatter
                 if custom_formatter:
                     formatter = custom_formatter
                 async_http_hander.setFormatter(formatter)
                 logger.addHandler(async_http_hander)
             http_handler = HTTPhandler(HTTPpost_url)
-            http_handler.setLevel(logging.INFO)
+            http_handler.setLevel(setHTTPLevel)
             formatter = self.public_formatter
             if custom_formatter:
                 formatter = custom_formatter
             http_handler.setFormatter(formatter)
             logger.addHandler(http_handler)
 
         return logger
```

### Comparing `SparkleLogging-1.0.2/SparkleLogging.egg-info/SOURCES.txt` & `SparkleLogging-1.0.3/SparkleLogging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.2/setup.py` & `SparkleLogging-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SparkleLogging',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(),
     author='花火official',
     author_email='3072252442@qq.com',
     description='A logging library for Python',
     long_description=open('Readme.md','r',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KOKOMI12345/SparkleLogging',
```

