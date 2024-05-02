# Comparing `tmp/osu_py-2.0.1.tar.gz` & `tmp/osu_py-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osu_py-2.0.1.tar", last modified: Sun Apr 21 08:58:11 2024, max compression
+gzip compressed data, was "osu_py-2.0.2.tar", last modified: Thu May  2 00:49:30 2024, max compression
```

## Comparing `osu_py-2.0.1.tar` & `osu_py-2.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 08:58:11.331484 osu_py-2.0.1/
--rw-rw-rw-   0        0        0     1094 2022-06-04 07:49:48.000000 osu_py-2.0.1/LICENSE
--rw-rw-rw-   0        0        0       24 2023-10-21 06:55:23.000000 osu_py-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4150 2024-04-21 08:58:11.329983 osu_py-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2984 2024-04-21 06:50:20.000000 osu_py-2.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-21 08:58:11.247487 osu_py-2.0.1/osu/
--rw-rw-rw-   0        0        0      391 2024-04-21 08:53:02.000000 osu_py-2.0.1/osu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 08:58:11.282984 osu_py-2.0.1/osu/asyncio/
--rw-rw-rw-   0        0        0       40 2022-02-10 01:20:57.000000 osu_py-2.0.1/osu/asyncio/__init__.py
--rw-rw-rw-   0        0        0    58757 2024-04-21 06:44:56.000000 osu_py-2.0.1/osu/asyncio/client.py
--rw-rw-rw-   0        0        0     5413 2024-04-21 06:44:55.000000 osu_py-2.0.1/osu/asyncio/http.py
--rw-rw-rw-   0        0        0    12111 2024-04-21 06:44:55.000000 osu_py-2.0.1/osu/auth.py
--rw-rw-rw-   0        0        0    58021 2024-04-21 06:44:56.000000 osu_py-2.0.1/osu/client.py
--rw-rw-rw-   0        0        0     1041 2024-04-12 20:15:58.000000 osu_py-2.0.1/osu/constants.py
--rw-rw-rw-   0        0        0    31492 2023-08-02 22:55:27.000000 osu_py-2.0.1/osu/enums.py
--rw-rw-rw-   0        0        0       97 2021-06-15 19:50:18.000000 osu_py-2.0.1/osu/exceptions.py
--rw-rw-rw-   0        0        0     4412 2024-04-21 06:44:55.000000 osu_py-2.0.1/osu/http.py
--rw-rw-rw-   0        0        0     7878 2024-04-21 06:44:55.000000 osu_py-2.0.1/osu/notification.py
-drwxrwxrwx   0        0        0        0 2024-04-21 08:58:11.325986 osu_py-2.0.1/osu/objects/
--rw-rw-rw-   0        0        0      554 2023-07-31 18:42:39.000000 osu_py-2.0.1/osu/objects/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-07-09 07:14:02.000000 osu_py-2.0.1/osu/objects/achievement.py
--rw-rw-rw-   0        0        0    26137 2023-10-21 06:16:49.000000 osu_py-2.0.1/osu/objects/beatmap.py
--rw-rw-rw-   0        0        0     9870 2023-07-09 07:36:16.000000 osu_py-2.0.1/osu/objects/beatmapset_event.py
--rw-rw-rw-   0        0        0     6006 2023-07-09 07:36:16.000000 osu_py-2.0.1/osu/objects/build.py
--rw-rw-rw-   0        0        0     4966 2023-07-31 18:23:23.000000 osu_py-2.0.1/osu/objects/chat.py
--rw-rw-rw-   0        0        0     7460 2023-07-09 07:36:16.000000 osu_py-2.0.1/osu/objects/comment.py
--rw-rw-rw-   0        0        0     4826 2023-07-09 07:36:16.000000 osu_py-2.0.1/osu/objects/current_user_attributes.py
--rw-rw-rw-   0        0        0     8463 2023-07-31 18:23:24.000000 osu_py-2.0.1/osu/objects/discussion.py
--rw-rw-rw-   0        0        0     8203 2023-07-31 18:44:40.000000 osu_py-2.0.1/osu/objects/event.py
--rw-rw-rw-   0        0        0     5810 2023-07-31 23:59:49.000000 osu_py-2.0.1/osu/objects/forum.py
--rw-rw-rw-   0        0        0     2416 2023-07-09 07:40:37.000000 osu_py-2.0.1/osu/objects/group.py
--rw-rw-rw-   0        0        0     2138 2023-07-09 07:41:54.000000 osu_py-2.0.1/osu/objects/kudosu.py
--rw-rw-rw-   0        0        0     5432 2023-08-01 00:00:54.000000 osu_py-2.0.1/osu/objects/match.py
--rw-rw-rw-   0        0        0    12031 2023-07-31 18:23:24.000000 osu_py-2.0.1/osu/objects/multiplayer.py
--rw-rw-rw-   0        0        0     2427 2023-07-09 08:22:08.000000 osu_py-2.0.1/osu/objects/news.py
--rw-rw-rw-   0        0        0    17563 2023-07-09 08:22:51.000000 osu_py-2.0.1/osu/objects/notification.py
--rw-rw-rw-   0        0        0     3165 2023-07-09 08:23:43.000000 osu_py-2.0.1/osu/objects/ranking.py
--rw-rw-rw-   0        0        0     1691 2023-07-09 07:36:16.000000 osu_py-2.0.1/osu/objects/scope.py
--rw-rw-rw-   0        0        0    13178 2024-04-20 05:34:50.000000 osu_py-2.0.1/osu/objects/score.py
--rw-rw-rw-   0        0        0     1327 2023-07-09 07:36:16.000000 osu_py-2.0.1/osu/objects/seasonal_background.py
--rw-rw-rw-   0        0        0    29585 2024-04-20 05:16:20.000000 osu_py-2.0.1/osu/objects/user.py
--rw-rw-rw-   0        0        0     2001 2023-07-09 07:36:16.000000 osu_py-2.0.1/osu/objects/wiki.py
--rw-rw-rw-   0        0        0     6612 2024-04-20 05:44:23.000000 osu_py-2.0.1/osu/path.py
--rw-rw-rw-   0        0        0     9104 2024-04-21 08:54:44.000000 osu_py-2.0.1/osu/results.py
--rw-rw-rw-   0        0        0    12080 2023-10-21 06:16:48.000000 osu_py-2.0.1/osu/util.py
-drwxrwxrwx   0        0        0        0 2024-04-21 08:58:11.327984 osu_py-2.0.1/osu.py.egg-info/
--rw-rw-rw-   0        0        0     4150 2024-04-21 08:58:11.000000 osu_py-2.0.1/osu.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1003 2024-04-21 08:58:11.000000 osu_py-2.0.1/osu.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 08:58:11.000000 osu_py-2.0.1/osu.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2024-04-21 08:58:11.000000 osu_py-2.0.1/osu.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-21 08:58:11.000000 osu_py-2.0.1/osu.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      204 2024-04-21 05:59:15.000000 osu_py-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       65 2024-04-21 05:30:36.000000 osu_py-2.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 08:58:11.331484 osu_py-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1630 2024-04-21 06:43:24.000000 osu_py-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:49:30.929842 osu_py-2.0.2/
+-rw-rw-rw-   0        0        0     1094 2022-06-04 07:49:48.000000 osu_py-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-10-21 06:55:23.000000 osu_py-2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4035 2024-05-02 00:49:30.920843 osu_py-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2869 2024-04-29 06:28:38.000000 osu_py-2.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-02 00:49:30.101345 osu_py-2.0.2/osu/
+-rw-rw-rw-   0        0        0      391 2024-05-02 00:47:43.000000 osu_py-2.0.2/osu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:49:30.250841 osu_py-2.0.2/osu/asyncio/
+-rw-rw-rw-   0        0        0       40 2022-02-10 01:20:57.000000 osu_py-2.0.2/osu/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    58757 2024-04-21 06:44:56.000000 osu_py-2.0.2/osu/asyncio/client.py
+-rw-rw-rw-   0        0        0     5413 2024-04-21 06:44:55.000000 osu_py-2.0.2/osu/asyncio/http.py
+-rw-rw-rw-   0        0        0    12078 2024-05-02 00:14:03.000000 osu_py-2.0.2/osu/auth.py
+-rw-rw-rw-   0        0        0    58021 2024-04-21 06:44:56.000000 osu_py-2.0.2/osu/client.py
+-rw-rw-rw-   0        0        0     1041 2024-04-12 20:15:58.000000 osu_py-2.0.2/osu/constants.py
+-rw-rw-rw-   0        0        0    31492 2023-08-02 22:55:27.000000 osu_py-2.0.2/osu/enums.py
+-rw-rw-rw-   0        0        0       97 2021-06-15 19:50:18.000000 osu_py-2.0.2/osu/exceptions.py
+-rw-rw-rw-   0        0        0     4412 2024-04-21 06:44:55.000000 osu_py-2.0.2/osu/http.py
+-rw-rw-rw-   0        0        0     7878 2024-04-21 06:44:55.000000 osu_py-2.0.2/osu/notification.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:49:30.894843 osu_py-2.0.2/osu/objects/
+-rw-rw-rw-   0        0        0      554 2023-07-31 18:42:39.000000 osu_py-2.0.2/osu/objects/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-07-09 07:14:02.000000 osu_py-2.0.2/osu/objects/achievement.py
+-rw-rw-rw-   0        0        0    26137 2023-10-21 06:16:49.000000 osu_py-2.0.2/osu/objects/beatmap.py
+-rw-rw-rw-   0        0        0     9870 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/beatmapset_event.py
+-rw-rw-rw-   0        0        0     6006 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/build.py
+-rw-rw-rw-   0        0        0     4966 2023-07-31 18:23:23.000000 osu_py-2.0.2/osu/objects/chat.py
+-rw-rw-rw-   0        0        0     7460 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/comment.py
+-rw-rw-rw-   0        0        0     4860 2024-05-01 23:50:50.000000 osu_py-2.0.2/osu/objects/current_user_attributes.py
+-rw-rw-rw-   0        0        0     8463 2023-07-31 18:23:24.000000 osu_py-2.0.2/osu/objects/discussion.py
+-rw-rw-rw-   0        0        0     8203 2023-07-31 18:44:40.000000 osu_py-2.0.2/osu/objects/event.py
+-rw-rw-rw-   0        0        0     5810 2023-07-31 23:59:49.000000 osu_py-2.0.2/osu/objects/forum.py
+-rw-rw-rw-   0        0        0     2416 2023-07-09 07:40:37.000000 osu_py-2.0.2/osu/objects/group.py
+-rw-rw-rw-   0        0        0     2138 2023-07-09 07:41:54.000000 osu_py-2.0.2/osu/objects/kudosu.py
+-rw-rw-rw-   0        0        0     5432 2023-08-01 00:00:54.000000 osu_py-2.0.2/osu/objects/match.py
+-rw-rw-rw-   0        0        0    12031 2023-07-31 18:23:24.000000 osu_py-2.0.2/osu/objects/multiplayer.py
+-rw-rw-rw-   0        0        0     2427 2023-07-09 08:22:08.000000 osu_py-2.0.2/osu/objects/news.py
+-rw-rw-rw-   0        0        0    17563 2023-07-09 08:22:51.000000 osu_py-2.0.2/osu/objects/notification.py
+-rw-rw-rw-   0        0        0     3165 2023-07-09 08:23:43.000000 osu_py-2.0.2/osu/objects/ranking.py
+-rw-rw-rw-   0        0        0     1691 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/scope.py
+-rw-rw-rw-   0        0        0    13178 2024-04-20 05:34:50.000000 osu_py-2.0.2/osu/objects/score.py
+-rw-rw-rw-   0        0        0     1327 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/seasonal_background.py
+-rw-rw-rw-   0        0        0    29585 2024-04-20 05:16:20.000000 osu_py-2.0.2/osu/objects/user.py
+-rw-rw-rw-   0        0        0     2001 2023-07-09 07:36:16.000000 osu_py-2.0.2/osu/objects/wiki.py
+-rw-rw-rw-   0        0        0     6612 2024-04-20 05:44:23.000000 osu_py-2.0.2/osu/path.py
+-rw-rw-rw-   0        0        0     9104 2024-04-21 08:54:44.000000 osu_py-2.0.2/osu/results.py
+-rw-rw-rw-   0        0        0    12080 2023-10-21 06:16:48.000000 osu_py-2.0.2/osu/util.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:49:30.901342 osu_py-2.0.2/osu.py.egg-info/
+-rw-rw-rw-   0        0        0     4035 2024-05-02 00:49:29.000000 osu_py-2.0.2/osu.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1003 2024-05-02 00:49:29.000000 osu_py-2.0.2/osu.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 00:49:29.000000 osu_py-2.0.2/osu.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2024-05-02 00:49:29.000000 osu_py-2.0.2/osu.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-02 00:49:29.000000 osu_py-2.0.2/osu.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      204 2024-04-21 05:59:15.000000 osu_py-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       65 2024-04-21 05:30:36.000000 osu_py-2.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 00:49:30.930842 osu_py-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2024-04-21 06:43:24.000000 osu_py-2.0.2/setup.py
```

### Comparing `osu_py-2.0.1/LICENSE` & `osu_py-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/PKG-INFO` & `osu_py-2.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osu.py
-Version: 2.0.1
+Version: 2.0.2
 Summary: API Wrapper for osu!api v2 written in Python.
 Home-page: https://github.com/Sheepposu/osu.py
 Author: Sheepposu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sheepposu/osu.py/issues
 Project-URL: osu.py documentation, https://osupy.readthedocs.io/
 Project-URL: osu!api v2 documentation, https://osu.ppy.sh/docs/index.html
@@ -40,17 +40,15 @@
    :target: https://pepy.tech/project/osu-py
    :alt: Download metric
 .. image:: https://readthedocs.org/projects/osupy/badge/?version=v1.0.0&style=flat
    :target: https://osupy.readthedocs.io
    :alt: Documentation
 
 Easy to use API wrapper for osu!api v2 written in Python.
-This uses osu!api v2, which is still under development. 
-So some code that was originally working may break overnight. 
-However, I'll do my best to fix any issues I find as quick as possible. 
+Has a high-level interface while still allowing ways to do more complex things.
 
 Major features/capabilties
 --------------------------
 - Client class which carries out all api requests.
 - AsynchronousClient class which is the same as Client but all api request functions are asynchronous.
 - NotificationWebsocket class for using the notification websocket feature of osu api v2.
 - Support for Authorization Code Grant and Client Credentials Grant.
```

### Comparing `osu_py-2.0.1/README.rst` & `osu_py-2.0.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,15 @@
    :target: https://pepy.tech/project/osu-py
    :alt: Download metric
 .. image:: https://readthedocs.org/projects/osupy/badge/?version=v1.0.0&style=flat
    :target: https://osupy.readthedocs.io
    :alt: Documentation
 
 Easy to use API wrapper for osu!api v2 written in Python.
-This uses osu!api v2, which is still under development. 
-So some code that was originally working may break overnight. 
-However, I'll do my best to fix any issues I find as quick as possible. 
+Has a high-level interface while still allowing ways to do more complex things.
 
 Major features/capabilties
 --------------------------
 - Client class which carries out all api requests.
 - AsynchronousClient class which is the same as Client but all api request functions are asynchronous.
 - NotificationWebsocket class for using the notification websocket feature of osu api v2.
 - Support for Authorization Code Grant and Client Credentials Grant.
```

### Comparing `osu_py-2.0.1/osu/asyncio/client.py` & `osu_py-2.0.2/osu/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/asyncio/http.py` & `osu_py-2.0.2/osu/asyncio/http.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/auth.py` & `osu_py-2.0.2/osu/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,14 @@
 class AsynchronousAuthHandler(FunctionalAuthHandler):
     async def _request(self, data, is_refresh=False):
         async with aiohttp.ClientSession() as session:
             async with session.request("POST", token_url, json=data) as resp:
                 try:
                     resp.raise_for_status()
                 except Exception as e:
-                    print(data)
                     raise e
                 json = await resp.json()
                 self._handle_response(json)
 
                 if is_refresh and self._refresh_callback:
                     self._refresh_callback(self)
```

### Comparing `osu_py-2.0.1/osu/client.py` & `osu_py-2.0.2/osu/client.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/constants.py` & `osu_py-2.0.2/osu/constants.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/enums.py` & `osu_py-2.0.2/osu/enums.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/http.py` & `osu_py-2.0.2/osu/http.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/notification.py` & `osu_py-2.0.2/osu/notification.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/__init__.py` & `osu_py-2.0.2/osu/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/achievement.py` & `osu_py-2.0.2/osu/objects/achievement.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/beatmap.py` & `osu_py-2.0.2/osu/objects/beatmap.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/beatmapset_event.py` & `osu_py-2.0.2/osu/objects/beatmapset_event.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/build.py` & `osu_py-2.0.2/osu/objects/build.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/chat.py` & `osu_py-2.0.2/osu/objects/chat.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/comment.py` & `osu_py-2.0.2/osu/objects/comment.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/current_user_attributes.py` & `osu_py-2.0.2/osu/objects/current_user_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,23 +155,23 @@
 
     **Attributes**
 
     is_pinned: :class:`bool`
 
     score_id: :class:`int`
 
-    score_type: :class:`ObjectType`
+    score_type: Optional[:class:`ObjectType`]
     """
 
     __slots__ = ("is_pinned", "score_id", "score_type")
 
     def __init__(self, data):
         self.is_pinned: bool = data["is_pinned"]
         self.score_id: int = data["score_id"]
-        self.score_type: ObjectType = ObjectType(data["score_type"])
+        self.score_type: Optional[ObjectType] = get_optional(data, "score_type", ObjectType)
 
 
 class CommentableMetaAttributes:
     """
     User attributes for a :class:`CommentableMeta` object
 
     **Attributes**
```

### Comparing `osu_py-2.0.1/osu/objects/discussion.py` & `osu_py-2.0.2/osu/objects/discussion.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/event.py` & `osu_py-2.0.2/osu/objects/event.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/forum.py` & `osu_py-2.0.2/osu/objects/forum.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/group.py` & `osu_py-2.0.2/osu/objects/group.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/kudosu.py` & `osu_py-2.0.2/osu/objects/kudosu.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/match.py` & `osu_py-2.0.2/osu/objects/match.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/multiplayer.py` & `osu_py-2.0.2/osu/objects/multiplayer.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/news.py` & `osu_py-2.0.2/osu/objects/news.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/notification.py` & `osu_py-2.0.2/osu/objects/notification.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/ranking.py` & `osu_py-2.0.2/osu/objects/ranking.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/scope.py` & `osu_py-2.0.2/osu/objects/scope.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/score.py` & `osu_py-2.0.2/osu/objects/score.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/seasonal_background.py` & `osu_py-2.0.2/osu/objects/seasonal_background.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/user.py` & `osu_py-2.0.2/osu/objects/user.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/objects/wiki.py` & `osu_py-2.0.2/osu/objects/wiki.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/path.py` & `osu_py-2.0.2/osu/path.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/results.py` & `osu_py-2.0.2/osu/results.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu/util.py` & `osu_py-2.0.2/osu/util.py`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/osu.py.egg-info/PKG-INFO` & `osu_py-2.0.2/osu.py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osu.py
-Version: 2.0.1
+Version: 2.0.2
 Summary: API Wrapper for osu!api v2 written in Python.
 Home-page: https://github.com/Sheepposu/osu.py
 Author: Sheepposu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sheepposu/osu.py/issues
 Project-URL: osu.py documentation, https://osupy.readthedocs.io/
 Project-URL: osu!api v2 documentation, https://osu.ppy.sh/docs/index.html
@@ -40,17 +40,15 @@
    :target: https://pepy.tech/project/osu-py
    :alt: Download metric
 .. image:: https://readthedocs.org/projects/osupy/badge/?version=v1.0.0&style=flat
    :target: https://osupy.readthedocs.io
    :alt: Documentation
 
 Easy to use API wrapper for osu!api v2 written in Python.
-This uses osu!api v2, which is still under development. 
-So some code that was originally working may break overnight. 
-However, I'll do my best to fix any issues I find as quick as possible. 
+Has a high-level interface while still allowing ways to do more complex things.
 
 Major features/capabilties
 --------------------------
 - Client class which carries out all api requests.
 - AsynchronousClient class which is the same as Client but all api request functions are asynchronous.
 - NotificationWebsocket class for using the notification websocket feature of osu api v2.
 - Support for Authorization Code Grant and Client Credentials Grant.
```

### Comparing `osu_py-2.0.1/osu.py.egg-info/SOURCES.txt` & `osu_py-2.0.2/osu.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osu_py-2.0.1/setup.py` & `osu_py-2.0.2/setup.py`

 * *Files identical despite different names*

