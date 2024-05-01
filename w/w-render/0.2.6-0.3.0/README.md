# Comparing `tmp/w_render-0.2.6.tar.gz` & `tmp/w_render-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w_render-0.2.6.tar", last modified: Mon Apr 15 13:41:06 2024, max compression
+gzip compressed data, was "w_render-0.3.0.tar", last modified: Wed May  1 21:43:54 2024, max compression
```

## Comparing `w_render-0.2.6.tar` & `w_render-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,20 @@
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:41:06.357049 w_render-0.2.6/
--rw-r--r--   0 repente   (1000) repente   (1000)      993 2024-04-15 13:41:06.353049 w_render-0.2.6/PKG-INFO
--rw-rw-r--   0 repente   (1000) repente   (1000)      605 2023-08-31 19:42:54.000000 w_render-0.2.6/README.md
--rw-rw-r--   0 repente   (1000) repente   (1000)       38 2024-04-15 13:41:06.357049 w_render-0.2.6/setup.cfg
--rw-rw-r--   0 repente   (1000) repente   (1000)     3297 2024-04-15 13:40:45.000000 w_render-0.2.6/setup.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:41:06.353049 w_render-0.2.6/w_render.egg-info/
--rw-r--r--   0 repente   (1000) repente   (1000)      993 2024-04-15 13:41:06.000000 w_render-0.2.6/w_render.egg-info/PKG-INFO
--rw-rw-r--   0 repente   (1000) repente   (1000)      790 2024-04-15 13:41:06.000000 w_render-0.2.6/w_render.egg-info/SOURCES.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)        1 2024-04-15 13:41:06.000000 w_render-0.2.6/w_render.egg-info/dependency_links.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)      158 2024-04-15 13:41:06.000000 w_render-0.2.6/w_render.egg-info/entry_points.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)       80 2024-04-15 13:41:06.000000 w_render-0.2.6/w_render.egg-info/requires.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)       11 2024-04-15 13:41:06.000000 w_render-0.2.6/w_render.egg-info/top_level.txt
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:41:06.353049 w_render-0.2.6/web_render/
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:41:06.353049 w_render-0.2.6/web_render/base/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:27:26.000000 w_render-0.2.6/web_render/base/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     2337 2023-09-03 20:30:16.000000 w_render-0.2.6/web_render/base/__main__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     8874 2024-04-15 13:40:45.000000 w_render-0.2.6/web_render/base/abstract.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1125 2023-08-24 07:40:40.000000 w_render-0.2.6/web_render/base/client.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1730 2024-04-15 13:30:29.000000 w_render-0.2.6/web_render/base/extends.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     4320 2023-08-24 21:59:25.000000 w_render-0.2.6/web_render/base/server.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     4107 2024-04-15 13:40:45.000000 w_render-0.2.6/web_render/base/test_webrender.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1508 2023-08-24 07:24:47.000000 w_render-0.2.6/web_render/config.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:41:06.353049 w_render-0.2.6/web_render/flask/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-07-28 09:55:28.000000 w_render-0.2.6/web_render/flask/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1817 2023-08-28 08:31:02.000000 w_render-0.2.6/web_render/flask/__main__.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:41:06.353049 w_render-0.2.6/web_render/flask/core/
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:41:06.353049 w_render-0.2.6/web_render/flask/core/main/
--rw-rw-r--   0 repente   (1000) repente   (1000)      837 2023-08-24 07:40:41.000000 w_render-0.2.6/web_render/flask/core/main/view.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:41:06.353049 w_render-0.2.6/web_render/flask/core/render_api/
--rw-rw-r--   0 repente   (1000) repente   (1000)     1372 2023-08-24 07:40:41.000000 w_render-0.2.6/web_render/flask/core/render_api/logic.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1075 2023-08-24 07:24:47.000000 w_render-0.2.6/web_render/flask/core/render_api/view.py
--rw-rw-r--   0 repente   (1000) repente   (1000)      207 2023-08-24 07:24:47.000000 w_render-0.2.6/web_render/flask/core/routing.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:41:06.353049 w_render-0.2.6/web_render/flask/core/service/
--rw-rw-r--   0 repente   (1000) repente   (1000)      389 2023-08-24 07:24:47.000000 w_render-0.2.6/web_render/flask/core/service/interface.py
--rw-rw-r--   0 repente   (1000) repente   (1000)      377 2023-08-24 07:24:47.000000 w_render-0.2.6/web_render/interface.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:41:06.353049 w_render-0.2.6/web_render/script/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:28:05.000000 w_render-0.2.6/web_render/script/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1507 2023-08-24 08:38:56.000000 w_render-0.2.6/web_render/script/render_server.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1498 2023-08-24 12:59:54.000000 w_render-0.2.6/web_render/tool.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-05-01 21:43:54.893122 w_render-0.3.0/
+-rw-r--r--   0 repente   (1000) repente   (1000)     1294 2024-05-01 21:43:54.893122 w_render-0.3.0/PKG-INFO
+-rw-rw-r--   0 repente   (1000) repente   (1000)      951 2024-05-01 21:28:50.000000 w_render-0.3.0/README.md
+-rw-rw-r--   0 repente   (1000) repente   (1000)       38 2024-05-01 21:43:54.893122 w_render-0.3.0/setup.cfg
+-rw-rw-r--   0 repente   (1000) repente   (1000)     2861 2024-05-01 21:43:49.000000 w_render-0.3.0/setup.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-05-01 21:43:54.893122 w_render-0.3.0/w_render.egg-info/
+-rw-r--r--   0 repente   (1000) repente   (1000)     1294 2024-05-01 21:43:54.000000 w_render-0.3.0/w_render.egg-info/PKG-INFO
+-rw-rw-r--   0 repente   (1000) repente   (1000)      354 2024-05-01 21:43:54.000000 w_render-0.3.0/w_render.egg-info/SOURCES.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)        1 2024-05-01 21:43:54.000000 w_render-0.3.0/w_render.egg-info/dependency_links.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)       65 2024-05-01 21:43:54.000000 w_render-0.3.0/w_render.egg-info/requires.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)       11 2024-05-01 21:43:54.000000 w_render-0.3.0/w_render.egg-info/top_level.txt
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-05-01 21:43:54.893122 w_render-0.3.0/web_render/
+-rw-rw-r--   0 repente   (1000) repente   (1000)       66 2024-05-01 20:48:45.000000 w_render-0.3.0/web_render/__init__.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-05-01 21:43:54.893122 w_render-0.3.0/web_render/base/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:27:26.000000 w_render-0.3.0/web_render/base/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)       90 2024-05-01 20:18:10.000000 w_render-0.3.0/web_render/base/__main__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     8694 2024-05-01 21:15:35.000000 w_render-0.3.0/web_render/base/abstract.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1821 2024-05-01 21:30:19.000000 w_render-0.3.0/web_render/base/extends.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      377 2024-05-01 21:30:48.000000 w_render-0.3.0/web_render/interface.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      981 2024-05-01 21:09:05.000000 w_render-0.3.0/web_render/tool.py
```

### Comparing `w_render-0.2.6/setup.py` & `w_render-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,49 +14,38 @@
     long_description = fh.read()
 
 # Функция, которая принимает несколько аргументов. Она присваивает эти значения пакету.
 setup(
     # Имя дистрибутива пакета. Оно должно быть уникальным, поэтому добавление вашего имени пользователя в конце является обычным делом.
     name="w-render",
     # Номер версии вашего пакета. Обычно используется семантическое управление версиями.
-    version="0.2.6",
+    version="0.3.0",
     # Имя автора.
     author="Andrey Plugin",
     # Его почта.
     author_email="9keepa@gmail.com",
     # Краткое описание, которое будет показано на странице PyPi.
     description="Render a dynamical sites.",
     # Длинное описание, которое будет отображаться на странице PyPi. Использует README.md репозитория для заполнения.
     long_description=long_description,
     # Определяет тип контента, используемый в long_description.
     long_description_content_type="text/markdown",
     # URL-адрес, представляющий домашнюю страницу проекта. Большинство проектов ссылаются на репозиторий.
     # Находит все пакеты внутри проекта и объединяет их в дистрибутив.
     packages=[
         "web_render",
-        "web_render.flask",
-        "web_render.flask.core",
-        "web_render.flask.core.main",
-        "web_render.flask.core.render_api",
-        "web_render.flask.core.service",
         "web_render.base",
-        "web_render.script",
     ],
     entry_points={
-        'console_scripts': [
-            'web-render = web_render.base.__main__:cli',
-            'flask-backend = web_render.flask.__main__:cli',
-            'render-server = web_render.script.render_server:cli',
-        ]
+        'console_scripts': []
     },
     # requirements или dependencies, которые будут установлены вместе с пакетом, когда пользователь установит его через pip.
     install_requires=[
-        "requests", "flask",
+        "selenium",
         "webdriver-manager",
-        "waitress",
         "undetected-chromedriver",
         "python-dotenv"
     ],
     # Требуемая версия Python.
     python_requires='>=3.8',
     # лицензия
     license='MIT',
```

### Comparing `w_render-0.2.6/web_render/base/abstract.py` & `w_render-0.3.0/web_render/base/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-Copyright (c) 2023 Plugin Andrey (9keepa@gmail.com)
+Copyright (c) 2024 Plugin Andrey (9keepa@gmail.com)
 Licensed under the MIT License
 """
 from abc import ABCMeta, abstractmethod
-from typing import Dict, Union, List, TypedDict
+from typing import Dict, Union, List, TypedDict, Callable
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.chrome.service import Service
 from web_render.tool import log
 from selenium.webdriver.common.by import By
@@ -96,26 +96,20 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.quit()
 
     def _web_wait(self, items: Union[IWebWait, List[IWebWait]]):
         if isinstance(items, list):
             for item in items:
-                target: Union[
-                    CheckElementInDOM,
-                    CheckNumberElementsInPage
-                ] = web_wait_class[item['name']]
-                self._web_driver_wait.until(target(**item['params']))
+                target: Callable = web_wait_class[item['name']](**item['params'])
+                self._web_driver_wait.until(target)
 
         if isinstance(items, dict):
-            target: Union[
-                CheckElementInDOM,
-                CheckNumberElementsInPage
-            ] = web_wait_class[items['name']]
-            self._web_driver_wait.until(target(**items['params']))
+            target: Callable = web_wait_class[items['name']](**items['params'])
+            self._web_driver_wait.until(target)
 
     def web_wait(self, items: Union[IWebWait, List[IWebWait]]):
         self._web_wait(items)
 
     def set_url(self, url, web_wait: Union[IWebWait, List[IWebWait], None]=None,
                 execute_script=None, execute_async_script=None):
         self.browser.get(url)
```

### Comparing `w_render-0.2.6/web_render/base/extends.py` & `w_render-0.3.0/web_render/base/extends.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Copyright (c) 2024 Plugin Andrey (9keepa@gmail.com)
+Licensed under the MIT License
+"""
 import base64
 import io
 import zipfile
 
 
 def get_extension(manifest_json, background_js):
     zip_buffer = io.BytesIO()
```

