# Comparing `tmp/aiotgbot-0.9.5.tar.gz` & `tmp/aiotgbot-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotgbot-0.9.5.tar", last modified: Thu May 27 08:27:09 2021, max compression
+gzip compressed data, was "aiotgbot-0.9.6.tar", last modified: Sat Jun 19 12:48:37 2021, max compression
```

## Comparing `aiotgbot-0.9.5.tar` & `aiotgbot-0.9.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 gleb      (1000) gleb      (1000)        0 2021-05-27 08:27:09.701280 aiotgbot-0.9.5/
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     1073 2021-02-13 14:27:57.000000 aiotgbot-0.9.5/LICENSE
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     2991 2021-05-27 08:27:09.701280 aiotgbot-0.9.5/PKG-INFO
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     2143 2021-02-22 09:23:33.000000 aiotgbot-0.9.5/README.rst
-drwxrwxr-x   0 gleb      (1000) gleb      (1000)        0 2021-05-27 08:27:09.697280 aiotgbot-0.9.5/aiotgbot/
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     2204 2021-05-27 08:25:06.000000 aiotgbot-0.9.5/aiotgbot/__init__.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)    57818 2021-05-08 17:57:10.000000 aiotgbot-0.9.5/aiotgbot/api_methods.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)    43446 2021-05-24 17:28:34.000000 aiotgbot-0.9.5/aiotgbot/api_types.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)    16941 2021-05-08 08:41:17.000000 aiotgbot-0.9.5/aiotgbot/bot.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     3454 2021-05-07 19:18:44.000000 aiotgbot-0.9.5/aiotgbot/bot_update.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     4273 2021-05-07 19:32:32.000000 aiotgbot-0.9.5/aiotgbot/constants.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     1455 2021-02-06 13:24:00.000000 aiotgbot-0.9.5/aiotgbot/exceptions.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     3864 2021-02-20 14:42:48.000000 aiotgbot-0.9.5/aiotgbot/filters.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)    14810 2021-05-07 19:34:36.000000 aiotgbot-0.9.5/aiotgbot/handler_table.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)      975 2021-02-20 14:11:40.000000 aiotgbot-0.9.5/aiotgbot/helpers.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     3824 2021-03-12 15:47:10.000000 aiotgbot-0.9.5/aiotgbot/listen_bot.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)       14 2020-11-12 16:48:25.000000 aiotgbot-0.9.5/aiotgbot/py.typed
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     2527 2021-03-11 09:13:16.000000 aiotgbot-0.9.5/aiotgbot/runner.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)      819 2021-02-06 13:24:00.000000 aiotgbot-0.9.5/aiotgbot/storage.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)      870 2021-02-06 13:25:09.000000 aiotgbot-0.9.5/aiotgbot/storage_memory.py
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     3117 2021-02-06 13:25:09.000000 aiotgbot-0.9.5/aiotgbot/storage_sqlite.py
-drwxrwxr-x   0 gleb      (1000) gleb      (1000)        0 2021-05-27 08:27:09.701280 aiotgbot-0.9.5/aiotgbot.egg-info/
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     2991 2021-05-27 08:27:09.000000 aiotgbot-0.9.5/aiotgbot.egg-info/PKG-INFO
--rw-rw-r--   0 gleb      (1000) gleb      (1000)      537 2021-05-27 08:27:09.000000 aiotgbot-0.9.5/aiotgbot.egg-info/SOURCES.txt
--rw-rw-r--   0 gleb      (1000) gleb      (1000)        1 2021-05-27 08:27:09.000000 aiotgbot-0.9.5/aiotgbot.egg-info/dependency_links.txt
--rw-rw-r--   0 gleb      (1000) gleb      (1000)      106 2021-05-27 08:27:09.000000 aiotgbot-0.9.5/aiotgbot.egg-info/requires.txt
--rw-rw-r--   0 gleb      (1000) gleb      (1000)        9 2021-05-27 08:27:09.000000 aiotgbot-0.9.5/aiotgbot.egg-info/top_level.txt
--rw-rw-r--   0 gleb      (1000) gleb      (1000)       38 2021-05-27 08:27:09.701280 aiotgbot-0.9.5/setup.cfg
--rw-rw-r--   0 gleb      (1000) gleb      (1000)     1532 2021-04-30 18:08:09.000000 aiotgbot-0.9.5/setup.py
+drwxrwxr-x   0 gleb      (1000) gleb      (1000)        0 2021-06-19 12:48:37.907233 aiotgbot-0.9.6/
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     1073 2021-02-13 14:27:57.000000 aiotgbot-0.9.6/LICENSE
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     2991 2021-06-19 12:48:37.907233 aiotgbot-0.9.6/PKG-INFO
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     2143 2021-02-22 09:23:33.000000 aiotgbot-0.9.6/README.rst
+drwxrwxr-x   0 gleb      (1000) gleb      (1000)        0 2021-06-19 12:48:37.903233 aiotgbot-0.9.6/aiotgbot/
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     2204 2021-06-19 12:45:28.000000 aiotgbot-0.9.6/aiotgbot/__init__.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)    57818 2021-05-08 17:57:10.000000 aiotgbot-0.9.6/aiotgbot/api_methods.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)    43635 2021-06-19 12:36:38.000000 aiotgbot-0.9.6/aiotgbot/api_types.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)    16941 2021-05-08 08:41:17.000000 aiotgbot-0.9.6/aiotgbot/bot.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     3454 2021-05-07 19:18:44.000000 aiotgbot-0.9.6/aiotgbot/bot_update.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     4273 2021-05-07 19:32:32.000000 aiotgbot-0.9.6/aiotgbot/constants.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     1455 2021-02-06 13:24:00.000000 aiotgbot-0.9.6/aiotgbot/exceptions.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     3864 2021-02-20 14:42:48.000000 aiotgbot-0.9.6/aiotgbot/filters.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)    14810 2021-05-07 19:34:36.000000 aiotgbot-0.9.6/aiotgbot/handler_table.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)      975 2021-02-20 14:11:40.000000 aiotgbot-0.9.6/aiotgbot/helpers.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     3824 2021-03-12 15:47:10.000000 aiotgbot-0.9.6/aiotgbot/listen_bot.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)       14 2020-11-12 16:48:25.000000 aiotgbot-0.9.6/aiotgbot/py.typed
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     2527 2021-03-11 09:13:16.000000 aiotgbot-0.9.6/aiotgbot/runner.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)      819 2021-02-06 13:24:00.000000 aiotgbot-0.9.6/aiotgbot/storage.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)      870 2021-02-06 13:25:09.000000 aiotgbot-0.9.6/aiotgbot/storage_memory.py
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     3117 2021-02-06 13:25:09.000000 aiotgbot-0.9.6/aiotgbot/storage_sqlite.py
+drwxrwxr-x   0 gleb      (1000) gleb      (1000)        0 2021-06-19 12:48:37.907233 aiotgbot-0.9.6/aiotgbot.egg-info/
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     2991 2021-06-19 12:48:37.000000 aiotgbot-0.9.6/aiotgbot.egg-info/PKG-INFO
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)      537 2021-06-19 12:48:37.000000 aiotgbot-0.9.6/aiotgbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)        1 2021-06-19 12:48:37.000000 aiotgbot-0.9.6/aiotgbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)      106 2021-06-19 12:48:37.000000 aiotgbot-0.9.6/aiotgbot.egg-info/requires.txt
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)        9 2021-06-19 12:48:37.000000 aiotgbot-0.9.6/aiotgbot.egg-info/top_level.txt
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)       38 2021-06-19 12:48:37.907233 aiotgbot-0.9.6/setup.cfg
+-rw-rw-r--   0 gleb      (1000) gleb      (1000)     1532 2021-04-30 18:08:09.000000 aiotgbot-0.9.6/setup.py
```

### Comparing `aiotgbot-0.9.5/LICENSE` & `aiotgbot-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/PKG-INFO` & `aiotgbot-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgbot
-Version: 0.9.5
+Version: 0.9.6
 Summary: Asynchronous library for Telegram bot API
 Home-page: https://github.com/gleb-chipiga/aiotgbot
 Author: Gleb Chipiga
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `aiotgbot-0.9.5/README.rst` & `aiotgbot-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/__init__.py` & `aiotgbot-0.9.6/aiotgbot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.9.5'
+__version__ = '0.9.6'
 
 from .api_types import (BaseTelegram, CallbackQuery, Chat, ChosenInlineResult,
                         Contact, File, InlineKeyboardButton,
                         InlineKeyboardMarkup, InlineQuery, KeyboardButton,
                         LocalFile, Message, PreCheckoutQuery,
                         ReplyKeyboardMarkup, ReplyKeyboardRemove,
                         ShippingQuery, StreamFile, User)
```

### Comparing `aiotgbot-0.9.5/aiotgbot/api_methods.py` & `aiotgbot-0.9.6/aiotgbot/api_methods.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/api_types.py` & `aiotgbot-0.9.6/aiotgbot/api_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from enum import Enum
 from io import BufferedReader
 from pathlib import Path
 from typing import (Any, AsyncIterator, Dict, Final, Generator, Iterable, List,
                     Optional, Set, Tuple, Type, TypeVar, Union, cast, get_args,
                     get_origin, get_type_hints)
 
 import attr
@@ -129,14 +130,16 @@
             key = _attr.name.rstrip('_')
             if isinstance(value, BaseTelegram):
                 _dict[key] = value.to_dict()
             elif isinstance(value, (tuple, list)):
                 _dict[key] = BaseTelegram._to_list(value)
             elif isinstance(value, (int, str, bool, float)):
                 _dict[key] = value
+            elif isinstance(value, Enum):
+                _dict[key] = value.value
             elif value is None:
                 continue
             else:
                 raise TypeError(f'"{value}" has unsupported type')
 
         return _dict
 
@@ -150,14 +153,16 @@
         for item in value:
             if isinstance(item, (int, str, bool, float)):
                 _list.append(item)
             elif isinstance(item, (tuple, list)):
                 _list.append(BaseTelegram._to_list(item))
             elif isinstance(item, BaseTelegram):
                 _list.append(item.to_dict())
+            elif isinstance(value, Enum):
+                _list.append(value.value)
             else:
                 raise TypeError(f'"{item}" has unsupported type')
 
         return _list
 
     @staticmethod
     def _get_type_hints(_type: Any) -> Tuple[Tuple[str, str, Any], ...]:
```

### Comparing `aiotgbot-0.9.5/aiotgbot/bot.py` & `aiotgbot-0.9.6/aiotgbot/bot.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/bot_update.py` & `aiotgbot-0.9.6/aiotgbot/bot_update.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/constants.py` & `aiotgbot-0.9.6/aiotgbot/constants.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/exceptions.py` & `aiotgbot-0.9.6/aiotgbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/filters.py` & `aiotgbot-0.9.6/aiotgbot/filters.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/handler_table.py` & `aiotgbot-0.9.6/aiotgbot/handler_table.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/helpers.py` & `aiotgbot-0.9.6/aiotgbot/helpers.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/listen_bot.py` & `aiotgbot-0.9.6/aiotgbot/listen_bot.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/runner.py` & `aiotgbot-0.9.6/aiotgbot/runner.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/storage.py` & `aiotgbot-0.9.6/aiotgbot/storage.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/storage_memory.py` & `aiotgbot-0.9.6/aiotgbot/storage_memory.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot/storage_sqlite.py` & `aiotgbot-0.9.6/aiotgbot/storage_sqlite.py`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/aiotgbot.egg-info/PKG-INFO` & `aiotgbot-0.9.6/aiotgbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgbot
-Version: 0.9.5
+Version: 0.9.6
 Summary: Asynchronous library for Telegram bot API
 Home-page: https://github.com/gleb-chipiga/aiotgbot
 Author: Gleb Chipiga
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `aiotgbot-0.9.5/aiotgbot.egg-info/SOURCES.txt` & `aiotgbot-0.9.6/aiotgbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotgbot-0.9.5/setup.py` & `aiotgbot-0.9.6/setup.py`

 * *Files identical despite different names*

