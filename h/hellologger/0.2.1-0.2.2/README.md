# Comparing `tmp/hellologger-0.2.1.tar.gz` & `tmp/hellologger-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hellologger-0.2.1.tar", max compression
+gzip compressed data, was "hellologger-0.2.2.tar", max compression
```

## Comparing `hellologger-0.2.1.tar` & `hellologger-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2024-03-22 13:18:42.471202 hellologger-0.2.1/LICENSE
--rw-r--r--   0        0        0      596 2024-03-31 14:29:17.041876 hellologger-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3847 2024-03-31 13:14:58.314070 hellologger-0.2.1/README.md
--rw-r--r--   0        0        0     4531 2024-03-31 14:28:44.465255 hellologger-0.2.1/src/hellologger/__init__.py
--rw-r--r--   0        0        0      308 2024-03-23 15:31:02.983633 hellologger-0.2.1/src/hellologger/const.py
--rw-r--r--   0        0        0     4434 1970-01-01 00:00:00.000000 hellologger-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-03-22 13:18:42.471202 hellologger-0.2.2/LICENSE
+-rw-r--r--   0        0        0      596 2024-05-02 16:57:50.292853 hellologger-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4354 2024-03-31 15:04:10.183295 hellologger-0.2.2/README.md
+-rw-r--r--   0        0        0     4860 2024-05-02 16:56:56.465688 hellologger-0.2.2/src/hellologger/__init__.py
+-rw-r--r--   0        0        0      308 2024-03-23 15:31:02.983633 hellologger-0.2.2/src/hellologger/const.py
+-rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 hellologger-0.2.2/PKG-INFO
```

### Comparing `hellologger-0.2.1/LICENSE` & `hellologger-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hellologger-0.2.1/pyproject.toml` & `hellologger-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hellologger"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["快乐的老鼠宝宝 <laoshubaby@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/OSMChina/Yuheng"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `hellologger-0.2.1/README.md` & `hellologger-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -118,7 +118,13 @@
 hellologger.log(level:str,message:str,device:str)
 ```
 
 并可指定logging或者loguru来完成任务，避免有部分平台loguru就是打不上去的也能用本项目打上去。
 
 引用hellologger从此一身轻！
 
+## 杂谈
+
+Q：为什么要叫这个名字？
+
+A：因为当时想了很多，包括什么logcat、magiclog等。然后在路过的招牌的塑料袋上看到一个hello，干脆就叫hellologger了，因为无论如何都要体现出log嘛。之后就去搜有没有撞车知名项目，然后只发现了[soongoo/HelloLogger](https://github.com/soongoo/HelloLogger)和[larse514/HelloLogger](https://github.com/larse514/HelloLogger)两个项目，都已经看起来停止维护了，就开工了！
+
```

### Comparing `hellologger-0.2.1/src/hellologger/__init__.py` & `hellologger-0.2.2/src/hellologger/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,61 +26,66 @@
     log_target: 是否启用不同的数据源
     不同数据源会使用对应的数据驱动
     代号可见如下：
     * local
     * aliyun
     * aws
     """
-    logging_config = {
-        "version": 1,
-        "formatters": {
-            "rawformatter": {
-                "class": "logging.Formatter",
-                "format": "%(message)s",
-            }
-        },
-        "handlers": {
-            "aliyun_sls_python_sdk": {
-                "()": "aliyun.log.QueuedLogHandler",
-                "level": log_level.get("aliyun", "INFO"),
-                "formatter": "rawformatter",
-                "end_point": get_variable(
-                    key=log_config.get("LOG_CONFIG_ALIYUN_ENDPOINT", None),
-                    default=LOG_CONFIG_ALIYUN_ENDPOINT,
-                ),
-                "access_key_id": get_variable(
-                    key="ALIYUN_ACCESSKEY_ID",
-                    default=LOG_CONFIG_ALIYUN_ACCESSKEY_ID,
-                ),
-                "access_key": get_variable(
-                    key="ALIYUN_ACCESSKEY_SECRET",
-                    default=LOG_CONFIG_ALIYUN_ACCESSKEY_SECRET,
-                ),
-                "project": get_variable(
-                    key=log_config.get("LOG_CONFIG_ALIYUN_PROJECT", None),
-                    default=LOG_CONFIG_ALIYUN_PROJECT,
-                ),
-                "log_store": get_variable(
-                    key=log_config.get("LOG_CONFIG_ALIYUN_LOGSTORE", None),
-                    default=LOG_CONFIG_ALIYUN_LOGSTORE,
-                ),
-            }
-        },
-        "loggers": {
-            "aliyun_sls": {
-                "handlers": [
-                    "aliyun_sls_python_sdk",
-                ],
-                "level": log_level.get("aliyun", "INFO"),
-                "propagate": False,
-            }
-        },
-    }
-    logging.config.dictConfig(logging_config)
-    logging_handler_aliyun = logging.getLogger("aliyun_sls").handlers[0]
+    if (
+        log_target.get("aliyun", True)
+        or log_target.get("aws", True)
+        or log_target.get("webhook", True)
+    ):
+        logging_config = {
+            "version": 1,
+            "formatters": {
+                "rawformatter": {
+                    "class": "logging.Formatter",
+                    "format": "%(message)s",
+                }
+            },
+            "handlers": {
+                "aliyun_sls_python_sdk": {
+                    "()": "aliyun.log.QueuedLogHandler",
+                    "level": log_level.get("aliyun", "INFO"),
+                    "formatter": "rawformatter",
+                    "end_point": get_variable(
+                        key=log_config.get("LOG_CONFIG_ALIYUN_ENDPOINT", None),
+                        default=LOG_CONFIG_ALIYUN_ENDPOINT,
+                    ),
+                    "access_key_id": get_variable(
+                        key="ALIYUN_ACCESSKEY_ID",
+                        default=LOG_CONFIG_ALIYUN_ACCESSKEY_ID,
+                    ),
+                    "access_key": get_variable(
+                        key="ALIYUN_ACCESSKEY_SECRET",
+                        default=LOG_CONFIG_ALIYUN_ACCESSKEY_SECRET,
+                    ),
+                    "project": get_variable(
+                        key=log_config.get("LOG_CONFIG_ALIYUN_PROJECT", None),
+                        default=LOG_CONFIG_ALIYUN_PROJECT,
+                    ),
+                    "log_store": get_variable(
+                        key=log_config.get("LOG_CONFIG_ALIYUN_LOGSTORE", None),
+                        default=LOG_CONFIG_ALIYUN_LOGSTORE,
+                    ),
+                }
+            },
+            "loggers": {
+                "aliyun_sls": {
+                    "handlers": [
+                        "aliyun_sls_python_sdk",
+                    ],
+                    "level": log_level.get("aliyun", "INFO"),
+                    "propagate": False,
+                }
+            },
+        }
+        logging.config.dictConfig(logging_config)
+        logging_handler_aliyun = logging.getLogger("aliyun_sls").handlers[0]
 
     loguru_config = {}
     loguru_format = "{time:YYYY-MM-DD HH:mm:ss.SSS} | {level: <8} | {name}:{function}:{line} - {message}"
     logger = loguru.logger
 
     # for pytest project may need to record logs write by framework
     # pytest-loguru
@@ -92,15 +97,15 @@
     logger.add(
         sink=os.path.join(log_path, log_file),
         format=loguru_format,
         level="TRACE",
         **loguru_config,
     )
     # saas_aliyun_sls
-    if log_target.get("aliyun", False):
+    if log_target.get("aliyun", True):
         logger.add(
             sink=logging_handler_aliyun,
             format=loguru_format,
             level=log_level.get("aliyun", "INFO"),
             **loguru_config,
         )
     # saas_aws_cloudwatch
```

### Comparing `hellologger-0.2.1/PKG-INFO` & `hellologger-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: hellologger
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Home-page: https://github.com/OSMChina/Yuheng
 License: MIT
 Author: 快乐的老鼠宝宝
 Author-email: laoshubaby@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Project-URL: Repository, https://github.com/OSMChina/Yuheng
 Description-Content-Type: text/markdown
 
 # HelloLogger
 
 Push your log to everywhere!
@@ -138,8 +139,14 @@
 hellologger.log(level:str,message:str,device:str)
 ```
 
 并可指定logging或者loguru来完成任务，避免有部分平台loguru就是打不上去的也能用本项目打上去。
 
 引用hellologger从此一身轻！
 
+## 杂谈
+
+Q：为什么要叫这个名字？
+
+A：因为当时想了很多，包括什么logcat、magiclog等。然后在路过的招牌的塑料袋上看到一个hello，干脆就叫hellologger了，因为无论如何都要体现出log嘛。之后就去搜有没有撞车知名项目，然后只发现了[soongoo/HelloLogger](https://github.com/soongoo/HelloLogger)和[larse514/HelloLogger](https://github.com/larse514/HelloLogger)两个项目，都已经看起来停止维护了，就开工了！
+
```

