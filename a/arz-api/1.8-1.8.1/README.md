# Comparing `tmp/arz_api-1.8.tar.gz` & `tmp/arz_api-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arz_api-1.8.tar", last modified: Wed May  1 21:16:16 2024, max compression
+gzip compressed data, was "arz_api-1.8.1.tar", last modified: Thu May  2 04:28:53 2024, max compression
```

## Comparing `arz_api-1.8.tar` & `arz_api-1.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 21:16:16.409235 arz_api-1.8/
--rw-rw-rw-   0        0        0     1089 2023-11-08 20:12:48.000000 arz_api-1.8/LICENSE
--rw-rw-rw-   0        0        0     1737 2024-05-01 21:16:16.407972 arz_api-1.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-11-08 20:15:07.000000 arz_api-1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 21:16:16.357942 arz_api-1.8/arz_api/
--rw-rw-rw-   0        0        0     3604 2023-08-04 21:34:31.000000 arz_api-1.8/arz_api/__init__.py
--rw-rw-rw-   0        0        0    30037 2024-05-01 21:05:52.000000 arz_api-1.8/arz_api/api.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:16:16.389893 arz_api-1.8/arz_api/bypass_antibot/
--rw-rw-rw-   0        0        0       21 2023-05-31 18:16:38.000000 arz_api-1.8/arz_api/bypass_antibot/__init__.py
--rw-rw-rw-   0        0        0    35306 2023-05-31 19:17:18.000000 arz_api-1.8/arz_api/bypass_antibot/script.py
--rw-rw-rw-   0        0        0      247 2023-06-03 18:57:22.000000 arz_api-1.8/arz_api/consts.py
--rw-rw-rw-   0        0        0      563 2023-07-08 19:21:59.000000 arz_api-1.8/arz_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:16:16.402957 arz_api-1.8/arz_api/models/
--rw-rw-rw-   0        0        0      112 2023-05-31 18:48:38.000000 arz_api-1.8/arz_api/models/__init__.py
--rw-rw-rw-   0        0        0     4093 2024-05-01 21:05:18.000000 arz_api-1.8/arz_api/models/category_object.py
--rw-rw-rw-   0        0        0     5180 2024-05-01 20:44:42.000000 arz_api-1.8/arz_api/models/member_object.py
--rw-rw-rw-   0        0        0      512 2023-07-08 10:56:45.000000 arz_api-1.8/arz_api/models/other.py
--rw-rw-rw-   0        0        0     5943 2024-05-01 21:08:21.000000 arz_api-1.8/arz_api/models/post_object.py
--rw-rw-rw-   0        0        0     5774 2024-05-01 20:46:57.000000 arz_api-1.8/arz_api/models/thread_object.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:16:16.404948 arz_api-1.8/arz_api.egg-info/
--rw-rw-rw-   0        0        0     1737 2024-05-01 21:16:16.000000 arz_api-1.8/arz_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-05-01 21:16:16.000000 arz_api-1.8/arz_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 21:16:16.000000 arz_api-1.8/arz_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-01 21:16:16.000000 arz_api-1.8/arz_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-01 21:16:16.000000 arz_api-1.8/arz_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 21:16:16.411232 arz_api-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1847 2024-05-01 21:15:05.000000 arz_api-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 04:28:53.707129 arz_api-1.8.1/
+-rw-rw-rw-   0        0        0     1089 2023-11-08 20:12:48.000000 arz_api-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0     1739 2024-05-02 04:28:53.707129 arz_api-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-11-08 20:15:07.000000 arz_api-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 04:28:53.644630 arz_api-1.8.1/arz_api/
+-rw-rw-rw-   0        0        0     3604 2023-08-04 21:34:31.000000 arz_api-1.8.1/arz_api/__init__.py
+-rw-rw-rw-   0        0        0    30043 2024-05-02 04:25:13.000000 arz_api-1.8.1/arz_api/api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 04:28:53.691502 arz_api-1.8.1/arz_api/bypass_antibot/
+-rw-rw-rw-   0        0        0       21 2023-05-31 18:16:38.000000 arz_api-1.8.1/arz_api/bypass_antibot/__init__.py
+-rw-rw-rw-   0        0        0    35306 2023-05-31 19:17:18.000000 arz_api-1.8.1/arz_api/bypass_antibot/script.py
+-rw-rw-rw-   0        0        0      247 2023-06-03 18:57:22.000000 arz_api-1.8.1/arz_api/consts.py
+-rw-rw-rw-   0        0        0      563 2023-07-08 19:21:59.000000 arz_api-1.8.1/arz_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-02 04:28:53.707129 arz_api-1.8.1/arz_api/models/
+-rw-rw-rw-   0        0        0      112 2023-05-31 18:48:38.000000 arz_api-1.8.1/arz_api/models/__init__.py
+-rw-rw-rw-   0        0        0     4093 2024-05-01 21:05:18.000000 arz_api-1.8.1/arz_api/models/category_object.py
+-rw-rw-rw-   0        0        0     5180 2024-05-01 20:44:42.000000 arz_api-1.8.1/arz_api/models/member_object.py
+-rw-rw-rw-   0        0        0      512 2023-07-08 10:56:45.000000 arz_api-1.8.1/arz_api/models/other.py
+-rw-rw-rw-   0        0        0     5943 2024-05-01 21:08:21.000000 arz_api-1.8.1/arz_api/models/post_object.py
+-rw-rw-rw-   0        0        0     5774 2024-05-01 20:46:57.000000 arz_api-1.8.1/arz_api/models/thread_object.py
+drwxrwxrwx   0        0        0        0 2024-05-02 04:28:53.707129 arz_api-1.8.1/arz_api.egg-info/
+-rw-rw-rw-   0        0        0     1739 2024-05-02 04:28:53.000000 arz_api-1.8.1/arz_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-02 04:28:53.000000 arz_api-1.8.1/arz_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 04:28:53.000000 arz_api-1.8.1/arz_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-02 04:28:53.000000 arz_api-1.8.1/arz_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 04:28:53.000000 arz_api-1.8.1/arz_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 04:28:53.707129 arz_api-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1849 2024-05-02 04:28:23.000000 arz_api-1.8.1/setup.py
```

### Comparing `arz_api-1.8/LICENSE` & `arz_api-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arz_api-1.8/PKG-INFO` & `arz_api-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arz_api
-Version: 1.8
+Version: 1.8.1
 Summary: Модуль для взаимодействия с форумом без Xenforo ключей
 Home-page: https://github.com/TastyBread123/Arizona-API/
 Author: TastyBread123
 Author-email: ermakovglebyt@gmail.com
 Project-URL: Documentation, https://tastybread123.github.io/Arizona-API/arz_api.html
 Keywords: python xenforo arizona roleplay samp gta
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `arz_api-1.8/arz_api/__init__.py` & `arz_api-1.8.1/arz_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8/arz_api/api.py` & `arz_api-1.8.1/arz_api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         post = content.find('article', {'id': f'js-post-{post_id}'})
         if post is None:
             return None
 
         try: creator = self.get_member(int(post.find('a', {'data-xf-init': 'member-tooltip'})['data-user-id']))
         except:
             user_info = post.find('a', {'data-xf-init': 'member-tooltip'})
-            creator = Member(self, int(user_info['data-user-id']), user_info.text, None, None, None, None, None)
+            creator = Member(self, int(user_info['data-user-id']), user_info.text, None, None, None, None, None, None)
 
         thread = self.get_thread(int(content.find('html')['data-content-key'].strip('thread-')))
         create_date = int(post.find('time', {'class': 'u-dt'})['data-time'])
         bb_content = post.find('div', {'class': 'bbWrapper'})
         text_content = bb_content.text
         return Post(self, post_id, creator, thread, create_date, bb_content, text_content)
```

### Comparing `arz_api-1.8/arz_api/bypass_antibot/script.py` & `arz_api-1.8.1/arz_api/bypass_antibot/script.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8/arz_api/exceptions.py` & `arz_api-1.8.1/arz_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8/arz_api/models/category_object.py` & `arz_api-1.8.1/arz_api/models/category_object.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8/arz_api/models/member_object.py` & `arz_api-1.8.1/arz_api/models/member_object.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8/arz_api/models/other.py` & `arz_api-1.8.1/arz_api/models/other.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8/arz_api/models/post_object.py` & `arz_api-1.8.1/arz_api/models/post_object.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8/arz_api/models/thread_object.py` & `arz_api-1.8.1/arz_api/models/thread_object.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.8/arz_api.egg-info/PKG-INFO` & `arz_api-1.8.1/arz_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arz_api
-Version: 1.8
+Version: 1.8.1
 Summary: Модуль для взаимодействия с форумом без Xenforo ключей
 Home-page: https://github.com/TastyBread123/Arizona-API/
 Author: TastyBread123
 Author-email: ermakovglebyt@gmail.com
 Project-URL: Documentation, https://tastybread123.github.io/Arizona-API/arz_api.html
 Keywords: python xenforo arizona roleplay samp gta
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `arz_api-1.8/arz_api.egg-info/SOURCES.txt` & `arz_api-1.8.1/arz_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arz_api-1.8/setup.py` & `arz_api-1.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name='arz_api',
-  version='1.8',
+  version='1.8.1',
   author='TastyBread123',
   author_email='ermakovglebyt@gmail.com',
   description='Модуль для взаимодействия с форумом без Xenforo ключей',
   long_description="""# Arizona-API
 API для взаимодействия с ресурсами Arizona без необходимости в получении API ключа xenforo у администраторов форума. Вы можете просто найти ваши куки (рекомендую для этого отдельные расширения) и начинать разработку!
 
 # Описание проекта
```

