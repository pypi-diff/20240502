# Comparing `tmp/arz_api-1.7.tar.gz` & `tmp/arz_api-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arz_api-1.7.tar", last modified: Wed Nov  8 20:16:11 2023, max compression
+gzip compressed data, was "arz_api-1.8.tar", last modified: Wed May  1 21:16:16 2024, max compression
```

## Comparing `arz_api-1.7.tar` & `arz_api-1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-11-08 20:16:11.953698 arz_api-1.7/
--rw-rw-rw-   0        0        0     1089 2023-11-08 20:12:48.000000 arz_api-1.7/LICENSE
--rw-rw-rw-   0        0        0     1648 2023-11-08 20:16:11.954723 arz_api-1.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-11-08 20:15:07.000000 arz_api-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-11-08 20:16:11.886936 arz_api-1.7/arz_api/
--rw-rw-rw-   0        0        0     3604 2023-08-04 21:34:31.000000 arz_api-1.7/arz_api/__init__.py
--rw-rw-rw-   0        0        0    28631 2023-11-08 19:34:11.000000 arz_api-1.7/arz_api/api.py
-drwxrwxrwx   0        0        0        0 2023-11-08 20:16:11.934755 arz_api-1.7/arz_api/bypass_antibot/
--rw-rw-rw-   0        0        0       21 2023-05-31 18:16:38.000000 arz_api-1.7/arz_api/bypass_antibot/__init__.py
--rw-rw-rw-   0        0        0    35306 2023-05-31 19:17:18.000000 arz_api-1.7/arz_api/bypass_antibot/script.py
--rw-rw-rw-   0        0        0      247 2023-06-03 18:57:22.000000 arz_api-1.7/arz_api/consts.py
--rw-rw-rw-   0        0        0      563 2023-07-08 19:21:59.000000 arz_api-1.7/arz_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-11-08 20:16:11.952701 arz_api-1.7/arz_api/models/
--rw-rw-rw-   0        0        0      112 2023-05-31 18:48:38.000000 arz_api-1.7/arz_api/models/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-11-08 19:23:07.000000 arz_api-1.7/arz_api/models/category_object.py
--rw-rw-rw-   0        0        0     4745 2023-11-08 19:17:06.000000 arz_api-1.7/arz_api/models/member_object.py
--rw-rw-rw-   0        0        0      512 2023-07-08 10:56:45.000000 arz_api-1.7/arz_api/models/other.py
--rw-rw-rw-   0        0        0     5106 2023-11-08 19:16:43.000000 arz_api-1.7/arz_api/models/post_object.py
--rw-rw-rw-   0        0        0     5483 2023-11-08 19:21:52.000000 arz_api-1.7/arz_api/models/thread_object.py
-drwxrwxrwx   0        0        0        0 2023-11-08 20:16:11.930364 arz_api-1.7/arz_api.egg-info/
--rw-rw-rw-   0        0        0     1648 2023-11-08 20:16:11.000000 arz_api-1.7/arz_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-11-08 20:16:11.000000 arz_api-1.7/arz_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-08 20:16:11.000000 arz_api-1.7/arz_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-11-08 20:16:11.000000 arz_api-1.7/arz_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-11-08 20:16:11.000000 arz_api-1.7/arz_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-08 20:16:11.957686 arz_api-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1847 2023-11-08 20:15:48.000000 arz_api-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:16:16.409235 arz_api-1.8/
+-rw-rw-rw-   0        0        0     1089 2023-11-08 20:12:48.000000 arz_api-1.8/LICENSE
+-rw-rw-rw-   0        0        0     1737 2024-05-01 21:16:16.407972 arz_api-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-11-08 20:15:07.000000 arz_api-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 21:16:16.357942 arz_api-1.8/arz_api/
+-rw-rw-rw-   0        0        0     3604 2023-08-04 21:34:31.000000 arz_api-1.8/arz_api/__init__.py
+-rw-rw-rw-   0        0        0    30037 2024-05-01 21:05:52.000000 arz_api-1.8/arz_api/api.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:16:16.389893 arz_api-1.8/arz_api/bypass_antibot/
+-rw-rw-rw-   0        0        0       21 2023-05-31 18:16:38.000000 arz_api-1.8/arz_api/bypass_antibot/__init__.py
+-rw-rw-rw-   0        0        0    35306 2023-05-31 19:17:18.000000 arz_api-1.8/arz_api/bypass_antibot/script.py
+-rw-rw-rw-   0        0        0      247 2023-06-03 18:57:22.000000 arz_api-1.8/arz_api/consts.py
+-rw-rw-rw-   0        0        0      563 2023-07-08 19:21:59.000000 arz_api-1.8/arz_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:16:16.402957 arz_api-1.8/arz_api/models/
+-rw-rw-rw-   0        0        0      112 2023-05-31 18:48:38.000000 arz_api-1.8/arz_api/models/__init__.py
+-rw-rw-rw-   0        0        0     4093 2024-05-01 21:05:18.000000 arz_api-1.8/arz_api/models/category_object.py
+-rw-rw-rw-   0        0        0     5180 2024-05-01 20:44:42.000000 arz_api-1.8/arz_api/models/member_object.py
+-rw-rw-rw-   0        0        0      512 2023-07-08 10:56:45.000000 arz_api-1.8/arz_api/models/other.py
+-rw-rw-rw-   0        0        0     5943 2024-05-01 21:08:21.000000 arz_api-1.8/arz_api/models/post_object.py
+-rw-rw-rw-   0        0        0     5774 2024-05-01 20:46:57.000000 arz_api-1.8/arz_api/models/thread_object.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:16:16.404948 arz_api-1.8/arz_api.egg-info/
+-rw-rw-rw-   0        0        0     1737 2024-05-01 21:16:16.000000 arz_api-1.8/arz_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-01 21:16:16.000000 arz_api-1.8/arz_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 21:16:16.000000 arz_api-1.8/arz_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-01 21:16:16.000000 arz_api-1.8/arz_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-01 21:16:16.000000 arz_api-1.8/arz_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 21:16:16.411232 arz_api-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1847 2024-05-01 21:15:05.000000 arz_api-1.8/setup.py
```

### Comparing `arz_api-1.7/LICENSE` & `arz_api-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `arz_api-1.7/PKG-INFO` & `arz_api-1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: arz_api
-Version: 1.7
+Version: 1.8
 Summary: Модуль для взаимодействия с форумом без Xenforo ключей
 Home-page: https://github.com/TastyBread123/Arizona-API/
 Author: TastyBread123
 Author-email: ermakovglebyt@gmail.com
 Project-URL: Documentation, https://tastybread123.github.io/Arizona-API/arz_api.html
 Keywords: python xenforo arizona roleplay samp gta
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.25.1
+Requires-Dist: bs4>=0.0.1
+Requires-Dist: dukpy>=0.3.0
 
 # Arizona-API
 API для взаимодействия с ресурсами Arizona без необходимости в получении API ключа xenforo у администраторов форума. Вы можете просто найти ваши куки (рекомендую для этого отдельные расширения) и начинать разработку!
 
 # Описание проекта
 API поддерживает около 35 методов, которые помогают в решении 90% задач. API легко масштабируется, а также имеет удобную [документацию](https://tastybread123.github.io/Arizona-API/arz_api.html).  
 Также рекомендую ознакомиться с [примерами](https://github.com/TastyBread123/Arizona-API/tree/main/examples), дабы возникало меньше вопросов по использованию API.
```

### Comparing `arz_api-1.7/arz_api/__init__.py` & `arz_api-1.8/arz_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.7/arz_api/api.py` & `arz_api-1.8/arz_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,60 +40,74 @@
     def current_member(self) -> CurrentMember:
         """Объект текущего пользователя"""
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/account").content, 'lxml')
         user_id = int(content.find('span', {'class': 'avatar--xxs'})['data-user-id'])
         member_info = self.get_member(user_id)
 
-        return CurrentMember(self, user_id, member_info.username, member_info.user_title, member_info.avatar, member_info.messages_count, member_info.reactions_count, member_info.trophies_count)
+        return CurrentMember(self, user_id, member_info.username, member_info.user_title, member_info.avatar, member_info.roles, member_info.messages_count, member_info.reactions_count, member_info.trophies_count)
 
     
     def get_category(self, category_id: int) -> Category:
         """Найти раздел по ID"""
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/forums/{category_id}").content, 'lxml')
         title = content.find('h1', {'class': 'p-title-value'}).text
+        if "Упс! Мы столкнулись с некоторыми проблемами." in title:
+            return None
 
         try: pages_count = int(content.find_all('li', {'class': 'pageNav-page'})[-1].text)
         except IndexError: pages_count = 1
         try: parent_category_id = int(content.find('html')['data-container-key'].strip('node-'))
         except: parent_category_id = None
 
         temp_url = ''
         if parent_category_id is not None: temp_url = f'forums/{parent_category_id}/'
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/{temp_url}").content, 'lxml')
         
-        return Category(self, category_id, title, pages_count)
+        return Category(self, category_id, title, pages_count, parent_category_id)
     
     
     def get_member(self, user_id: int) -> Member:
-        """Найти пользователя по ID"""
+        """Найти пользователя по ID (возвращает либо Member, либо None (если профиль закрыт / не существует))"""
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/members/{user_id}").content, 'lxml')
-        username = content.find('span', {'class': 'username'}).text
-        
+
+        username = content.find('span', {'class': 'username'})
+        if username is None:
+            return None
+        username = username.text
+
+        roles = []
+        for i in content.find('div', {'class': 'memberHeader-banners'}).children:
+            if i.text != '\n': roles.append(i.text)
+
         try: user_title = content.find('span', {'class': 'userTitle'}).text
         except AttributeError: user_title = None
         try: avatar = MAIN_URL + content.find('a', {'class': 'avatar avatar--l'})['href']
         except TypeError: avatar = None
 
         messages_count = int(content.find('a', {'href': f'/search/member?user_id={user_id}'}).text.strip().replace(',', ''))
         reactions_count = int(content.find('dl', {'class': 'pairs pairs--rows pairs--rows--centered'}).find('dd').text.strip().replace(',', ''))
         trophies_count = int(content.find('a', {'href': f'/members/{user_id}/trophies'}).text.strip().replace(',', ''))
         
-        return Member(self, user_id, username, user_title, avatar, messages_count, reactions_count, trophies_count)
+        return Member(self, user_id, username, user_title, avatar, roles, messages_count, reactions_count, trophies_count)
 
     
     def get_thread(self, thread_id: int) -> Thread:
-        """Найти тему по ID"""
+        """Найти тему по ID (Thread если тема существует, None если недоступна / не существует)"""
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-1").content, 'lxml')
         
-        try: creator = self.get_member(int(content.find('a', {'class': 'username'})['data-user-id']))
-        except: creator = Member(self, int(content.find('a', {'class': 'username'})['data-user-id']), content.find('a', {'class': 'username'}).text, None, None, None, None, None)
+        creator_id = content.find('a', {'class': 'username'})
+        if creator_id is None:
+            return None
+
+        try: creator = self.get_member(int(creator_id['data-user-id']))
+        except: creator = Member(self, int(creator_id['data-user-id']), content.find('a', {'class': 'username'}).text, None, None, None, None, None, None)
         
         category = self.get_category(int(content.find('html')['data-container-key'].strip('node-')))
         create_date = int(content.find('time')['data-time'])
         
         try: title = [i for i in content.find('h1', {'class': 'p-title-value'}).strings][-1]
         except: title = ""
         try: prefix = content.find('h1', {'class': 'p-title-value'}).find('span', {'class': 'label'}).text
@@ -108,19 +122,21 @@
         if content.find('dl', {'class': 'blockStatus'}): is_closed = True
         thread_post_id = content.find('article', {'id': compile('js-post-*')})['id'].strip('js-post-')
 
         return Thread(self, thread_id, creator, category, create_date, title, prefix, thread_content, thread_content_html, pages_count, thread_post_id, is_closed)
     
 
     def get_post(self, post_id: int) -> Post:
-        """Найти пост по ID"""
+        """Найти пост по ID (Post если существует, None - удален / нет доступа)"""
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/posts/{post_id}").content, 'lxml')
         post = content.find('article', {'id': f'js-post-{post_id}'})
-        
+        if post is None:
+            return None
+
         try: creator = self.get_member(int(post.find('a', {'data-xf-init': 'member-tooltip'})['data-user-id']))
         except:
             user_info = post.find('a', {'data-xf-init': 'member-tooltip'})
             creator = Member(self, int(user_info['data-user-id']), user_info.text, None, None, None, None, None)
 
         thread = self.get_thread(int(content.find('html')['data-content-key'].strip('thread-')))
         create_date = int(post.find('time', {'class': 'u-dt'})['data-time'])
@@ -130,14 +146,17 @@
 
 
     def get_profile_post(self, post_id: int) -> ProfilePost:
         """Найти сообщение профиля по ID"""
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/profile-posts/{post_id}").content, 'lxml')
         post = content.find('article', {'id': f'js-profilePost-{post_id}'})
+        if post is None:
+            return None
+
         creator = self.get_member(int(post.find('a', {'class': 'username'})['data-user-id']))
         profile = self.get_member(int(content.find('span', {'class': 'username'})['data-user-id']))
         create_date = int(post.find('time')['data-time'])
         bb_content = post.find('div', {'class': 'bbWrapper'})
         text_content = bb_content.text
 
         return ProfilePost(self, post_id, creator, profile, create_date, bb_content, text_content)
@@ -356,14 +375,28 @@
             Объект Response модуля requests
         """
 
         token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
         return self.session.post(f"{MAIN_URL}/posts/{post_id}/delete", {"reason": reason, "hard_delete": int(hard_delete), "_xfToken": token})
     
 
+    def bookmark_post(self, post_id: int) -> Response:
+        """Добавить сообщение в закладки
+
+        Attributes:
+            post_id (int): ID сообщения
+        
+        Returns:
+            Объект Response модуля requests
+        """
+
+        token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
+        return self.session.post(f"{MAIN_URL}/posts/{post_id}/bookmark", {"_xfToken": token})
+
+
     # PROFILE POST
     def react_profile_post(self, post_id: int, reaction_id: int = 1) -> Response:
         """Поставить реакцию на сообщение профиля
 
         Attributes:
             post_id (int): ID сообщения профиля
             reaction_id (int): ID реакции. По умолчанию 1 (необяз.)
@@ -527,15 +560,15 @@
             Объект Response модуля requests
         """
 
         token = BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
         data = {"_xfToken": token}
 
         if title is not None: data.update({'title': title})
-        if prefix_id is not None: data.update({'prefix_id[]', prefix_id})
+        if prefix_id is not None: data.update({'prefix_id[]': prefix_id})
 
         return self.session.post(f"{MAIN_URL}/threads/{thread_id}/edit", data)
     
 
     def get_thread_posts(self, thread_id: int, page: int = 1) -> list:
         """Получить все сообщения из темы на странице
```

### Comparing `arz_api-1.7/arz_api/bypass_antibot/script.py` & `arz_api-1.8/arz_api/bypass_antibot/script.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.7/arz_api/exceptions.py` & `arz_api-1.8/arz_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.7/arz_api/models/category_object.py` & `arz_api-1.8/arz_api/models/category_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from arz_api import ArizonaAPI
 
 
 class Category:
-    def __init__(self, API: 'ArizonaAPI', id: int, title: str, pages_count: int) -> None:
+    def __init__(self, API: 'ArizonaAPI', id: int, title: str, pages_count: int, parent_category_id: int) -> None:
         self.API = API
         self.id = id
         """**ID категории**"""
         self.title = title
         """**Название категории**"""
         self.pages_count = pages_count
         """**Количество страниц в категории**"""
+        self.parent_category_id = parent_category_id
+        """**ID предыдуще категории (родительская). Если нет - None**"""
 
 
     def create_thread(self, title: str, message_html: str, discussion_type: str = 'discussion', watch_thread: int = 1) -> Response:
         """Создать тему в категории
 
         Attributes:
             title (str): Название темы
@@ -78,7 +80,16 @@
         """Получить дочерние категории из раздела
         
         Returns:
             Список (list), состоящий из ID дочерних категорий раздела
         """
 
         return self.API.get_categories(self.id)
+    
+
+    def get_url(self) -> str:
+        """Получить ссылку на объект
+        
+        Returns:
+            Ссылку в формате https://forum.arizona-rp.com/forums/x/"""
+        
+        return f"https://forum.arizona-rp.com/forums/{self.id}/"
```

### Comparing `arz_api-1.7/arz_api/models/member_object.py` & `arz_api-1.8/arz_api/models/member_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,32 @@
 class Member:
     API: 'ArizonaAPI'  # Объект ArizonaAPI
 
     id: int
     username: str
     user_title: str
     avatar: str
+    roles: list
     
     messages_count: int
     reactions_count: int
     trophies_count: int
 
-    def __init__(self, API, id: int, username: str, user_title: str, avatar: str, messages_count: int, reactions_count: int, trophies_count: int) -> None:
+    def __init__(self, API, id: int, username: str, user_title: str, avatar: str, roles: list, messages_count: int, reactions_count: int, trophies_count: int) -> None:
         self.API = API
         self.id = id
         """**ID пользователя**"""
         self.username = username
         """**Имя пользователя**"""
         self.user_title = user_title
         """**Звание пользователя**"""
         self.avatar = avatar
         """**Ссылка на аватарку пользователя**"""
+        self.roles = roles
+        """Роль пользователя на форуме ('покраска')"""
 
         self.messages_count = messages_count
         """**Количество сообщений в счетчике**"""
         self.reactions_count = reactions_count
         """**Количество реакций в счетчике**"""
         self.trophies_count = trophies_count
         """**Количество баллов в счетчике**"""
@@ -76,14 +79,22 @@
             page (int): Страница для поиска. По умолчанию 1 (необяз.)
             
         Returns:
             Cписок (list) с ID всех сообщений профиля
         """
 
         return self.API.get_profile_messages(self.id, page)
+    
+    def get_url(self) -> str:
+        """Получить ссылку на объект
+        
+        Returns:
+            Ссылку в формате https://forum.arizona-rp.com/members/x/"""
+        
+        return f"https://forum.arizona-rp.com/members/{self.id}/"
 
 
 class CurrentMember(Member):
     follow = property(doc='Forbidden method for Current Member object')
     ignore = property(doc='Forbidden method for Current Member object')
 
     def edit_avatar(self, upload_photo: str) -> Response:
```

### Comparing `arz_api-1.7/arz_api/models/other.py` & `arz_api-1.8/arz_api/models/other.py`

 * *Files identical despite different names*

### Comparing `arz_api-1.7/arz_api/models/post_object.py` & `arz_api-1.8/arz_api/models/post_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,31 @@
             hard_delete (bool): Полное удаление сообщения. По умолчанию False (необяз.)
             
         Returns:
             Объект Response модуля requests
         """
 
         return self.API.delete_post(self.id, reason, hard_delete)
+    
+    
+    def bookmark(self) -> Response:
+        """Добавить сообщение в закладки
+        
+        Returns:
+            Объект Response модуля requests"""
+        return self.API.bookmark_post(self.id)
+    
+
+    def get_url(self) -> str:
+        """Получить ссылку на объект
+        
+        Returns:
+            Ссылку в формате https://forum.arizona-rp.com/posts/x/"""
+        
+        return f"https://forum.arizona-rp.com/posts/{self.id}/"
 
 
 class ProfilePost:
     def __init__(self, API: 'ArizonaAPI', id: int, creator: 'Member', profile: 'Member', create_date: int, bb_content: str, text_content: str) -> None:
         self.API = API
         self.id = id
         """**ID сообщения профиля**"""
@@ -127,7 +144,16 @@
             message_html (str): Новое содержание сообщения профиля. Рекомендуется использование HTML
         
         Returns:
             Объект Response модуля requests
         """
 
         return self.API.edit_profile_post(self.id, message_html)
+
+
+    def get_url(self) -> str:
+        """Получить ссылку на объект
+        
+        Returns:
+            Ссылку в формате https://forum.arizona-rp.com/profile-posts/x/"""
+        
+        return f"https://forum.arizona-rp.com/profile-posts/{self.id}/"
```

### Comparing `arz_api-1.7/arz_api/models/thread_object.py` & `arz_api-1.8/arz_api/models/thread_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,7 +142,16 @@
             reaction_id (int): ID реакции. По умолчанию 1 (необяз.)
             
         Returns:
             Объект Response модуля requests
         """
 
         return self.API.react_thread(self.id, reaction_id)
+    
+
+    def get_url(self) -> str:
+        """Получить ссылку на объект
+        
+        Returns:
+            Ссылку в формате https://forum.arizona-rp.com/threads/x/"""
+        
+        return f"https://forum.arizona-rp.com/threads/{self.id}/"
```

### Comparing `arz_api-1.7/arz_api.egg-info/PKG-INFO` & `arz_api-1.8/arz_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
-Name: arz-api
-Version: 1.7
+Name: arz_api
+Version: 1.8
 Summary: Модуль для взаимодействия с форумом без Xenforo ключей
 Home-page: https://github.com/TastyBread123/Arizona-API/
 Author: TastyBread123
 Author-email: ermakovglebyt@gmail.com
 Project-URL: Documentation, https://tastybread123.github.io/Arizona-API/arz_api.html
 Keywords: python xenforo arizona roleplay samp gta
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.25.1
+Requires-Dist: bs4>=0.0.1
+Requires-Dist: dukpy>=0.3.0
 
 # Arizona-API
 API для взаимодействия с ресурсами Arizona без необходимости в получении API ключа xenforo у администраторов форума. Вы можете просто найти ваши куки (рекомендую для этого отдельные расширения) и начинать разработку!
 
 # Описание проекта
 API поддерживает около 35 методов, которые помогают в решении 90% задач. API легко масштабируется, а также имеет удобную [документацию](https://tastybread123.github.io/Arizona-API/arz_api.html).  
 Также рекомендую ознакомиться с [примерами](https://github.com/TastyBread123/Arizona-API/tree/main/examples), дабы возникало меньше вопросов по использованию API.
```

### Comparing `arz_api-1.7/arz_api.egg-info/SOURCES.txt` & `arz_api-1.8/arz_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arz_api-1.7/setup.py` & `arz_api-1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name='arz_api',
-  version='1.7',
+  version='1.8',
   author='TastyBread123',
   author_email='ermakovglebyt@gmail.com',
   description='Модуль для взаимодействия с форумом без Xenforo ключей',
   long_description="""# Arizona-API
 API для взаимодействия с ресурсами Arizona без необходимости в получении API ключа xenforo у администраторов форума. Вы можете просто найти ваши куки (рекомендую для этого отдельные расширения) и начинать разработку!
 
 # Описание проекта
```

