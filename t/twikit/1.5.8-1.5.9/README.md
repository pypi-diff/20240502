# Comparing `tmp/twikit-1.5.8.tar.gz` & `tmp/twikit-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.5.8.tar", last modified: Thu Apr 25 06:59:23 2024, max compression
+gzip compressed data, was "twikit-1.5.9.tar", last modified: Sun Apr 28 13:04:44 2024, max compression
```

## Comparing `twikit-1.5.8.tar` & `twikit-1.5.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 06:59:23.013476 twikit-1.5.8/
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.8/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-25 06:59:23.010478 twikit-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 06:59:23.013476 twikit-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:59:22.933684 twikit-1.5.8/twikit/
--rw-rw-rw-   0        0        0      658 2024-04-25 06:57:47.000000 twikit-1.5.8/twikit/__init__.py
--rw-rw-rw-   0        0        0     1686 2024-04-23 16:10:15.000000 twikit-1.5.8/twikit/bookmark.py
--rw-rw-rw-   0        0        0   139609 2024-04-25 06:49:11.000000 twikit-1.5.8/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.8/twikit/community.py
--rw-rw-rw-   0        0        0     2666 2024-04-22 14:20:57.000000 twikit-1.5.8/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.8/twikit/group.py
--rw-rw-rw-   0        0        0     2095 2024-04-23 16:02:50.000000 twikit-1.5.8/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.8/twikit/notification.py
--rw-rw-rw-   0        0        0        0 2024-04-23 16:07:38.000000 twikit-1.5.8/twikit/py.typed
--rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/trend.py
--rw-rw-rw-   0        0        0    23612 2024-04-25 06:54:59.000000 twikit-1.5.8/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:59:23.008484 twikit-1.5.8/twikit/twikit_async/
--rw-rw-rw-   0        0        0      610 2024-04-23 16:10:47.000000 twikit-1.5.8/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0     1758 2024-04-23 16:10:22.000000 twikit-1.5.8/twikit/twikit_async/bookmark.py
--rw-rw-rw-   0        0        0   141857 2024-04-25 06:47:26.000000 twikit-1.5.8/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.8/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.8/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    23493 2024-04-25 06:55:20.000000 twikit-1.5.8/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-04-25 06:56:56.000000 twikit-1.5.8/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.8/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.8/twikit/user.py
--rw-rw-rw-   0        0        0    30253 2024-04-25 02:12:28.000000 twikit-1.5.8/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:59:22.951638 twikit-1.5.8/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-25 06:59:22.000000 twikit-1.5.8/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      857 2024-04-25 06:59:22.000000 twikit-1.5.8/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 06:59:22.000000 twikit-1.5.8/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-25 06:59:22.000000 twikit-1.5.8/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-25 06:59:22.000000 twikit-1.5.8/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 13:04:44.979653 twikit-1.5.9/
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.9/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-28 13:04:44.977661 twikit-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 13:04:44.979653 twikit-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-26 14:47:36.000000 twikit-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:04:44.909846 twikit-1.5.9/twikit/
+-rw-rw-rw-   0        0        0      658 2024-04-28 13:04:06.000000 twikit-1.5.9/twikit/__init__.py
+-rw-rw-rw-   0        0        0     1686 2024-04-23 16:10:15.000000 twikit-1.5.9/twikit/bookmark.py
+-rw-rw-rw-   0        0        0   139609 2024-04-25 17:33:46.000000 twikit-1.5.9/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.9/twikit/community.py
+-rw-rw-rw-   0        0        0     2666 2024-04-22 14:20:57.000000 twikit-1.5.9/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.9/twikit/group.py
+-rw-rw-rw-   0        0        0     2095 2024-04-23 16:02:50.000000 twikit-1.5.9/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-25 14:48:07.000000 twikit-1.5.9/twikit/notification.py
+-rw-rw-rw-   0        0        0        0 2024-04-23 16:07:38.000000 twikit-1.5.9/twikit/py.typed
+-rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/trend.py
+-rw-rw-rw-   0        0        0    23812 2024-04-28 13:02:12.000000 twikit-1.5.9/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:04:44.974668 twikit-1.5.9/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      610 2024-04-25 17:56:33.000000 twikit-1.5.9/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0     1758 2024-04-23 16:10:22.000000 twikit-1.5.9/twikit/twikit_async/bookmark.py
+-rw-rw-rw-   0        0        0   141857 2024-04-26 13:42:52.000000 twikit-1.5.9/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-04-26 13:28:49.000000 twikit-1.5.9/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.9/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    23693 2024-04-28 13:01:46.000000 twikit-1.5.9/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-04-26 13:32:10.000000 twikit-1.5.9/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.9/twikit/user.py
+-rw-rw-rw-   0        0        0    30253 2024-04-25 02:12:28.000000 twikit-1.5.9/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 13:04:44.927796 twikit-1.5.9/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-28 13:04:44.000000 twikit-1.5.9/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      857 2024-04-28 13:04:44.000000 twikit-1.5.9/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 13:04:44.000000 twikit-1.5.9/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-28 13:04:44.000000 twikit-1.5.9/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 13:04:44.000000 twikit-1.5.9/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.5.8/LICENSE` & `twikit-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/PKG-INFO` & `twikit-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.8
+Version: 1.5.9
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.8/README.md` & `twikit-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/setup.py` & `twikit-1.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/__init__.py` & `twikit-1.5.9/twikit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========================
 Twikit Twitter API Wrapper
 ==========================
 
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.5.8'
+__version__ = '1.5.9'
 
 from .bookmark import BookmarkFolder
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
 from .group import Group, GroupMessage
```

### Comparing `twikit-1.5.8/twikit/bookmark.py` & `twikit-1.5.9/twikit/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/client.py` & `twikit-1.5.9/twikit/client.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/community.py` & `twikit-1.5.9/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/errors.py` & `twikit-1.5.9/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/group.py` & `twikit-1.5.9/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/http.py` & `twikit-1.5.9/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/list.py` & `twikit-1.5.9/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/message.py` & `twikit-1.5.9/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/notification.py` & `twikit-1.5.9/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/trend.py` & `twikit-1.5.9/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/tweet.py` & `twikit-1.5.9/twikit/tweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,18 @@
         Poll attached to the tweet.
     has_card : :class:`bool`
         Indicates if the tweet contains a card.
     thumbnail_title : :class:`str` | None
         The title of the webpage displayed inside tweet's card.
     thumbnail_url : :class:`str` | None
         Link to the image displayed in the tweet's card.
+    urls : :class:`list`
+        Information about URLs contained in the tweet.
+    full_text : :class:`str` | None
+        The full text of the tweet.
     """
 
     def __init__(self, client: Client, data: dict, user: User = None) -> None:
         self._client = client
         self._data = data
         self.user = user
 
@@ -158,22 +162,22 @@
         self.is_edit_eligible: bool = data['edit_control'].get(
             'is_edit_eligible')
         self.edits_remaining: int = data['edit_control'].get('edits_remaining')
         self.state: str = (data['views'].get('state')
                            if 'views' in data else None)
         self.has_community_notes: bool = data.get('has_birdwatch_notes')
 
+        self.community_note = None
         if 'birdwatch_pivot' in data:
             community_note_data = data['birdwatch_pivot']
-            self.community_note = {
-                'id': community_note_data['note']['rest_id'],
-                'text': community_note_data['subtitle']['text']
-            }
-        else:
-            self.community_note = None
+            if 'note' in community_note_data:
+                self.community_note = {
+                    'id': community_note_data['note']['rest_id'],
+                    'text': community_note_data['subtitle']['text']
+                }
 
         if note_tweet_results:
             hashtags_ = find_dict(note_tweet_results, 'hashtags')
             if hashtags_:
                 hashtags = hashtags_[0]
             else:
                 hashtags = []
```

### Comparing `twikit-1.5.8/twikit/twikit_async/__init__.py` & `twikit-1.5.9/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/bookmark.py` & `twikit-1.5.9/twikit/twikit_async/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/client.py` & `twikit-1.5.9/twikit/twikit_async/client.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/community.py` & `twikit-1.5.9/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/errors.py` & `twikit-1.5.9/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/group.py` & `twikit-1.5.9/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/http.py` & `twikit-1.5.9/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/list.py` & `twikit-1.5.9/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/message.py` & `twikit-1.5.9/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/notification.py` & `twikit-1.5.9/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/trend.py` & `twikit-1.5.9/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/tweet.py` & `twikit-1.5.9/twikit/twikit_async/tweet.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,18 @@
         Hashtags included in the tweet text.
     has_card : :class:`bool`
         Indicates if the tweet contains a card.
     thumbnail_title : :class:`str` | None
         The title of the webpage displayed inside tweet's card.
     thumbnail_url : :class:`str` | None
         Link to the image displayed in the tweet's card.
+    urls : :class:`list`
+        Information about URLs contained in the tweet.
+    full_text : :class:`str` | None
+        The full text of the tweet.
     """
 
     def __init__(self, client: Client, data: dict, user: User = None) -> None:
         self._client = client
         self._data = data
         self.user = user
 
@@ -155,22 +159,22 @@
         self.is_edit_eligible: bool = data['edit_control'].get(
             'is_edit_eligible')
         self.edits_remaining: int = data['edit_control'].get('edits_remaining')
         self.state: str = (data['views'].get('state')
                            if 'views' in data else None)
         self.has_community_notes: bool = data.get('has_birdwatch_notes')
 
+        self.community_note = None
         if 'birdwatch_pivot' in data:
             community_note_data = data['birdwatch_pivot']
-            self.community_note = {
-                'id': community_note_data['note']['rest_id'],
-                'text': community_note_data['subtitle']['text']
-            }
-        else:
-            self.community_note = None
+            if 'note' in community_note_data:
+                self.community_note = {
+                    'id': community_note_data['note']['rest_id'],
+                    'text': community_note_data['subtitle']['text']
+                }
 
         if note_tweet_results:
             hashtags_ = find_dict(note_tweet_results, 'hashtags')
             if hashtags_:
                 hashtags = hashtags_[0]
             else:
                 hashtags = []
```

### Comparing `twikit-1.5.8/twikit/twikit_async/user.py` & `twikit-1.5.9/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/twikit_async/utils.py` & `twikit-1.5.9/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/user.py` & `twikit-1.5.9/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit/utils.py` & `twikit-1.5.9/twikit/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.8/twikit.egg-info/PKG-INFO` & `twikit-1.5.9/twikit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.8
+Version: 1.5.9
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.8/twikit.egg-info/SOURCES.txt` & `twikit-1.5.9/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

