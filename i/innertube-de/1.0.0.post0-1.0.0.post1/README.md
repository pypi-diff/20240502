# Comparing `tmp/innertube_de-1.0.0.post0.tar.gz` & `tmp/innertube-de-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innertube_de-1.0.0.post0.tar", last modified: Fri Apr 26 15:56:42 2024, max compression
+gzip compressed data, was "innertube-de-1.0.0.post1.tar", last modified: Thu May  2 11:29:06 2024, max compression
```

## Comparing `innertube_de-1.0.0.post0.tar` & `innertube-de-1.0.0.post1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-04-26 15:56:42.373049 innertube_de-1.0.0.post0/
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1058 2024-04-14 16:38:01.000000 innertube_de-1.0.0.post0/LICENSE
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3100 2024-04-26 15:56:42.369716 innertube_de-1.0.0.post0/PKG-INFO
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2708 2024-04-26 15:56:27.000000 innertube_de-1.0.0.post0/README.md
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-04-26 15:56:42.369716 innertube_de-1.0.0.post0/innertube_de/
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1703 2024-04-24 09:49:38.000000 innertube_de-1.0.0.post0/innertube_de/__init__.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     5262 2024-04-23 12:08:36.000000 innertube_de-1.0.0.post0/innertube_de/containers.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8158 2024-04-24 10:16:58.000000 innertube_de-1.0.0.post0/innertube_de/endpoints.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     1098 2024-04-24 09:55:56.000000 innertube_de-1.0.0.post0/innertube_de/errors.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    58257 2024-04-24 18:38:45.000000 innertube_de-1.0.0.post0/innertube_de/extractor.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4223 2024-04-21 09:08:19.000000 innertube_de-1.0.0.post0/innertube_de/itags.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    26279 2024-04-24 15:29:38.000000 innertube_de-1.0.0.post0/innertube_de/items.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3970 2024-04-23 16:24:08.000000 innertube_de-1.0.0.post0/innertube_de/stream.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     4742 2024-04-24 16:22:19.000000 innertube_de-1.0.0.post0/innertube_de/types.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8555 2024-04-24 14:48:45.000000 innertube_de-1.0.0.post0/innertube_de/utils.py
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-04-26 15:56:42.369716 innertube_de-1.0.0.post0/innertube_de.egg-info/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3100 2024-04-26 15:56:42.000000 innertube_de-1.0.0.post0/innertube_de.egg-info/PKG-INFO
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)      424 2024-04-26 15:56:42.000000 innertube_de-1.0.0.post0/innertube_de.egg-info/SOURCES.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)        1 2024-04-26 15:56:42.000000 innertube_de-1.0.0.post0/innertube_de.egg-info/dependency_links.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       13 2024-04-26 15:56:42.000000 innertube_de-1.0.0.post0/innertube_de.egg-info/top_level.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       38 2024-04-26 15:56:42.373049 innertube_de-1.0.0.post0/setup.cfg
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)      785 2024-04-26 15:56:06.000000 innertube_de-1.0.0.post0/setup.py
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-04-26 15:56:42.369716 innertube_de-1.0.0.post0/tests/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)    13336 2024-04-24 21:49:23.000000 innertube_de-1.0.0.post0/tests/tester.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/PKG-INFO
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2708 2024-05-02 11:24:00.000000 innertube-de-1.0.0.post1/README.md
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/innertube_de/
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1703 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/__init__.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     5262 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/containers.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8158 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/endpoints.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     1098 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/errors.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    58862 2024-05-02 11:22:37.000000 innertube-de-1.0.0.post1/innertube_de/extractor.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4223 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/itags.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    26289 2024-05-02 11:22:37.000000 innertube-de-1.0.0.post1/innertube_de/items.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3970 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/stream.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     4742 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/types.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8543 2024-05-02 10:48:08.000000 innertube-de-1.0.0.post1/innertube_de/utils.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/innertube_de.egg-info/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-02 11:29:06.000000 innertube-de-1.0.0.post1/innertube_de.egg-info/PKG-INFO
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)      416 2024-05-02 11:29:06.000000 innertube-de-1.0.0.post1/innertube_de.egg-info/SOURCES.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)        1 2024-05-02 11:29:06.000000 innertube-de-1.0.0.post1/innertube_de.egg-info/dependency_links.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       13 2024-05-02 11:29:06.000000 innertube-de-1.0.0.post1/innertube_de.egg-info/top_level.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       38 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/setup.cfg
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)      785 2024-05-02 11:23:51.000000 innertube-de-1.0.0.post1/setup.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/tests/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)    13806 2024-05-02 11:22:31.000000 innertube-de-1.0.0.post1/tests/tester.py
```

### Comparing `innertube_de-1.0.0.post0/PKG-INFO` & `innertube-de-1.0.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: innertube-de
-Version: 1.0.0.post0
+Version: 1.0.0.post1
 Summary: InnerTube Data Extractor
 Home-page: https://github.com/g3nsy/innertube-de
 Author: g3nsy
 Author-email: g3nsydev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-0-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-1-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube_de-1.0.0.post0/README.md` & `innertube-de-1.0.0.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-0-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-1-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube_de-1.0.0.post0/innertube_de/__init__.py` & `innertube-de-1.0.0.post1/innertube_de/__init__.py`

 * *Files identical despite different names*

### Comparing `innertube_de-1.0.0.post0/innertube_de/containers.py` & `innertube-de-1.0.0.post1/innertube_de/containers.py`

 * *Files identical despite different names*

### Comparing `innertube_de-1.0.0.post0/innertube_de/endpoints.py` & `innertube-de-1.0.0.post1/innertube_de/endpoints.py`

 * *Files identical despite different names*

### Comparing `innertube_de-1.0.0.post0/innertube_de/errors.py` & `innertube-de-1.0.0.post1/innertube_de/errors.py`

 * *Files identical despite different names*

### Comparing `innertube_de-1.0.0.post0/innertube_de/extractor.py` & `innertube-de-1.0.0.post1/innertube_de/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,14 +625,16 @@
             if item_type is None:
                 item_type = get_item_type(
                     self._get(
                         ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer", 
                         "text", "runs", 0, "text", opt=True
                     )
                 )
+                if item_type is None:
+                    item_type = ItemType.SONG
 
             match item_type:
                 case ItemType.ARTIST:
                     subscribers = self._clc_int(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer",
                             "text", "runs", -1, "text", opt=True
@@ -652,15 +654,14 @@
                     )
                     item = AlbumItem(
                         name=name, endpoint=endpoint, thumbnail_url=thumbnail_url,
                         release_year=release_year, artist_items=None
                     )
 
                 case ItemType.YOUTUBE_MUSIC_VIDEO:
-                    # _clc_int IndexError in some cases
                     length = self._clc_length(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer", "text",
                             "runs", -1, "text"
                         )
                     )
 
@@ -678,15 +679,14 @@
                     tracks_num = to_int(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer", "text",
                             "runs", -1, "text", opt=True
                         )
                     )
 
-                    # _clc_int IndexError in some cases
                     views = self._clc_int(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer", "text",
                             "runs", -1, "text", opt=True
                         ),
                         opt=True
                     )
@@ -711,14 +711,21 @@
                     length = self._clc_length(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer", 
                             "text", "runs", -1, "text", opt=True
                         ),
                         opt=True
                     )
+                    if length is None:
+                        length = self._clc_length(
+                            self._get(
+                                ds, "fixedColumns", 0, "musicResponsiveListItemFixedColumnRenderer",
+                                "text", "runs", 0, "text", opt=True
+                            )
+                        )
 
                     attempt1 = self._clc_int(
                         self._get(
                             ds, "flexColumns", -1, "musicResponsiveListItemFlexColumnRenderer",
                             "text", "runs", -1, "text", opt=True
                         ),
                         opt=True
@@ -751,17 +758,19 @@
                         ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer",
                         "text", "runs", -1, "text"
                     )
                     item = ProfileItem(name=name, thumbnail_url=thumbnail_url, handle=item_handle)
 
                 case ItemType.EP:
                     item = EPItem(name=name, endpoint=endpoint, thumbnail_url=thumbnail_url)
+
                 case _:
                     return None
 
+
         # YouTube Music
         elif ItemStructType.MUSIC_TWO_ROW_ITEM.value in entry_item:
             ds = self._get(entry_item, ItemStructType.MUSIC_TWO_ROW_ITEM.value)
             thumbnail_url = self._extract_urls(
                 self._get(ds, "thumbnailRenderer", "musicThumbnailRenderer", "thumbnail", "thumbnails")
             )
             name = self._get(ds, "title", "runs", 0, "text")
@@ -774,15 +783,14 @@
                             "text", "runs", 0, "text", opt=True
                         )
                     )
                 except ValueError:
                     item_type = None
 
             match item_type:
-
                 case ItemType.ARTIST:
                     subscribers = self._clc_int(self._get(ds, "subtitle", "runs", 0, "text"))
                     item = ArtistItem(
                         name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, subscribers=subscribers
                     )
 
                 case ItemType.ALBUM:
@@ -864,48 +872,54 @@
             ds = self._get(entry_item, ItemStructType.MUSIC_DETAIL_HEADER.value)
             try:
                 item_type = ItemType(self._get(ds, "subtitle", "runs", 0, "text"))
             except ValueError:
                 return None
 
             name = self._get(ds, "title", "runs", 0, "text")
+
             thumbnail_url = self._extract_urls(
                 self._get(ds, "thumbnail", "croppedSquareThumbnailRenderer", "thumbnail", "thumbnails")
             )
 
             release_year = to_int(self._get(ds, "subtitle", "runs", -1, "text", opt=True))
+
             if item_type is ItemType.YOUTUBE_MUSIC_PLAYLIST:
-                tracks_num = to_int(self._get(ds, "secondSubtitle", "runs", 2, "text"))
+                tracks_num = clc_int(self._get(ds, "secondSubtitle", "runs", 2, "text"))
             else:
-                tracks_num = to_int(self._get(ds, "secondSubtitle", "runs", 0, "text"))
+                tracks_num = clc_int(self._get(ds, "secondSubtitle", "runs", 0, "text"))
+
+            description = self._extract_description(self._get(ds, "description", "runs", opt=True))
+
+            # TODO extract length: X minutes, N hour (?), K seconds (?)
 
             match item_type:
                 case ItemType.ALBUM:
                     item = AlbumItem(
                         name=name, endpoint=None, thumbnail_url=thumbnail_url, tracks_num=tracks_num,
-                        release_year=release_year
+                        release_year=release_year, description=description
                     )
 
                 case ItemType.EP:
                     item = EPItem(
-                        name=name, endpoint=None, thumbnail_url=thumbnail_url, 
-                        tracks_num=tracks_num, release_year=release_year
+                        name=name, endpoint=None, thumbnail_url=thumbnail_url, tracks_num=tracks_num, 
+                        release_year=release_year, description=description
                     )
 
                 case ItemType.SINGLE:
                     item = SingleItem(
-                        name=name, endpoint=None, thumbnail_url=thumbnail_url, 
-                        tracks_num=tracks_num, release_year=release_year
+                        name=name, endpoint=None, thumbnail_url=thumbnail_url, tracks_num=tracks_num, 
+                        release_year=release_year, description=description
                     )
 
                 case ItemType.YOUTUBE_MUSIC_PLAYLIST:
                     views = self._clc_int(self._get(ds, "secondSubtitle", "runs", 0, "text"))
                     item = YouTubeMusicPlaylistItem(
                         name=name, endpoint=None, thumbnail_url=thumbnail_url, tracks_num=tracks_num,
-                        release_year=release_year, views=views
+                        release_year=release_year, description=description, views=views
                     )
 
                 case _:
                     return None
 
         # YouTube Music
         elif ItemStructType.MUSIC_VISUAL_HEADER.value in entry_item:
```

### Comparing `innertube_de-1.0.0.post0/innertube_de/itags.py` & `innertube-de-1.0.0.post1/innertube_de/itags.py`

 * *Files identical despite different names*

### Comparing `innertube_de-1.0.0.post0/innertube_de/items.py` & `innertube-de-1.0.0.post1/innertube_de/items.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Base class of items. Contains data common to all other defined Item types.
     """
     def __init__(
             self,
             name: Optional[str] = None,
             thumbnail_url: Optional[List[Dict]] = None,
             endpoint: Optional[Endpoint] = None,
-            description: Optional[List[Tuple[str, Endpoint]]] = None,
+            description: Optional[List[Tuple[str, Optional[Endpoint]]]] = None,
     ) -> None:
         """
         Initialize this object with the specified parameters.
         @param name: The name of the item.
         @param thumbnail_url: The URL of the cover of this item.
         @param endpoint: The associated Endpoint object.
         @param description: A description of this item.
```

### Comparing `innertube_de-1.0.0.post0/innertube_de/stream.py` & `innertube-de-1.0.0.post1/innertube_de/stream.py`

 * *Files identical despite different names*

### Comparing `innertube_de-1.0.0.post0/innertube_de/types.py` & `innertube-de-1.0.0.post1/innertube_de/types.py`

 * *Files identical despite different names*

### Comparing `innertube_de-1.0.0.post0/innertube_de/utils.py` & `innertube-de-1.0.0.post1/innertube_de/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import re
 
-from datetime import (
-    time,
-    date
-)
+from datetime import time, date
 
 from typing import (
     Optional,
     Callable,
     List,
     Any,
     Dict,
```

### Comparing `innertube_de-1.0.0.post0/innertube_de.egg-info/PKG-INFO` & `innertube-de-1.0.0.post1/innertube_de.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: innertube-de
-Version: 1.0.0.post0
+Version: 1.0.0.post1
 Summary: InnerTube Data Extractor
 Home-page: https://github.com/g3nsy/innertube-de
 Author: g3nsy
 Author-email: g3nsydev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-0-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-1-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube_de-1.0.0.post0/setup.py` & `innertube-de-1.0.0.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 here = Path(__file__).parent
 long_description = (here / "README.md").read_text()
 
 
 setup(
     name="innertube-de",
-    version="1.0.0-0",
+    version="1.0.0-1",
     description="InnerTube Data Extractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="g3nsy",
     author_email="g3nsydev@gmail.com",
     python_requires=">=3.6.0",
     url="https://github.com/g3nsy/innertube-de",
```

### Comparing `innertube_de-1.0.0.post0/tests/tester.py` & `innertube-de-1.0.0.post1/tests/tester.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import json
-import traceback
 import argparse
 import logging
 import paths
 from rich import console
 from httpx import ConnectError
 from innertube.clients import InnerTube
 from innertube.errors import RequestError
@@ -146,70 +145,90 @@
 
                     if self.save_data:
                         with open(os.path.join(self.dump_path, f"{name}.json"), mode="w") as file:
                             json.dump(dump, file, indent=4)
                     self.ser_log.append(f"{name} [green][OK][/green]")
 
                 except Exception:
-                    traceback.print_exc()
+                    log.exception(f"{name}: serialization error")
                     self.ser_log.append(f"{name} [red][ER][/red]")
+                    self.ser_containers[name] = None
 
             else:
                 self.ser_containers[name] = None
                 self.ser_log.append(f"{name} [yellow][NE][/yellow]")
 
     def test_deserialization(self) -> None:
         for name, container_data in self.ser_containers.items():
             if container_data is not None:
+
                 container = Container()
-                container.load(container_data)
-                self.des_containers[name] = container
-                self.des_log.append(f"{name} [green][OK][/green]")
+
+                try:
+                    container.load(container_data)  
+
+                except Exception:
+                    log.exception(f"{name}: deserialization error")
+                    self.des_log.append(f"{name} [red][ER][/red]")
+                    self.des_containers[name] = None
+
+                else:
+                    self.des_containers[name] = container
+                    self.des_log.append(f"{name} [green][OK][/green]")
+
             else:
-                self.des_containers[name] = None
                 self.des_log.append(f"{name} [yellow][NE][/yellow]")
+                self.des_containers[name] = None
 
     def test_data_integrity(self) -> None:
         for name, container in self.des_containers.items():
-            if container is None and self.ext_containers[name] is None:
+            
+            if container is None:
                 self.dat_log.append(f"{name} [yellow][NE][/yellow]")
+
             else:
                 try:
                     compare_container(container, self.ext_containers[name])
                     check_container(container)                  # type: ignore
                     check_container(self.ext_containers[name])  # type: ignore
                         
                     if self.ext_containers[name] == container:
                         self.dat_log.append(f"{name} [green][OK][/green]")
                     else:
                         self.dat_log.append(f"{name} [red][ER][/red]")
 
                 except AssertionError:
-                    cs.print(f"[blue]{name}[/blue]")
-                    log.exception("data integrity error")
+                    log.exception(f"{name}: data integrity error")
                     self.dat_log.append(f"{name} [red][ER][/red]")
 
     def _do_extraction_test(self, func: Callable, test_type: str, test_name: str) -> None:
         name = f"{test_type}_{test_name}"
         cs.print()
         cs.print(f"[blue]{name}[/blue]")
         try:
             innertube_data = get_innertube_data(func)
             ext_container = self.extractor.extract(innertube_data)
 
-        except (ExtractionError, RequestError, ConnectError) as error:
-            traceback.print_exc()
+        except (RequestError, ConnectError):
+            log.exception(f"{name}: innertube error")
+            self.ext_log.append(f"{name} [yellow][NE][/yellow]")
+            self.ext_containers[name] = None
+
+        except ExtractionError:
+            log.exception(f"{name}: extraction error")
             self.ext_log.append(f"{name} [red][ER][/red]")
             self.ext_containers[name] = None
 
-            if isinstance(error, ExtractionError) and self.save_data:
+            if self.save_data is True:
                 with open(os.path.join(self.errs_path, f"{name}.json"), mode="w") as file:
                     json.dump(innertube_data, file, indent=4)  # noqa # type: ignore
-        except Exception as error:
-            traceback.print_exc()
+
+        except Exception:
+            log.exception("tester error")
+
         else:
             self.ext_log.append(f"{name} [green][OK][/green]")
             self.ext_containers[name] = ext_container
             if self.verbose:
                 print_container(ext_container)
             if self.save_data:
                 with open(os.path.join(self.inne_path, f"{name}.json"), mode="w") as file:
@@ -227,33 +246,34 @@
         return
 
     def rstring(string: str) -> str:
         return (" " * distance).join([string for _ in range(len(testers))])
 
     def get_table_line(tester: Tester, index: int) -> str:
         table_line = f"| {tester.ext_log[index]} "
-        table_line += f"| {tester.des_log[index]} "
         table_line += f"| {tester.ser_log[index]} "
+        table_line += f"| {tester.des_log[index]} "
         table_line += f"| {tester.dat_log[index]} |"
         return table_line
 
+    LENGTH = 77
     def get_table_name(tester: Tester) -> str:
-        ns = 0 if center is False else 77 // 2 - len(tester.target.value) // 2
-        sxs = " " * (77 + distance - len(tester.target.value) - ns)
+        ns = 0 if center is False else LENGTH // 2 - len(tester.target.value) // 2
+        sxs = " " * (LENGTH + distance - len(tester.target.value) - ns)
         return f"{' ' * ns}{tester.target.value.upper()}{sxs}"
 
     table_horizontal = "+------------------" * 4 + "+"
     ext_col = "| [blue]EXTRACTION[/blue]       "
     ser_col = "| [blue]SERIALIZATION[/blue]    "
     des_col = "| [blue]DESERIALIZATION[/blue]  "
     dat_col = "| [blue]DATA INTEGRITY[/blue]   |"
     table_header = f"{ext_col}{ser_col}{des_col}{dat_col}"
 
     td = get_terminal_dimensions()
-    max_width = len(testers) * 77 + (distance * len(testers))
+    max_width = len(testers) * LENGTH + (distance * len(testers))
     vertical_view = (td[1] < max_width or vertical_view) if td is not None else True
 
     cs.print()
     if vertical_view:
         for tester in testers:
             cs.print(f"[blue]{get_table_name(tester)}[/blue]")
             cs.print(table_horizontal)
@@ -268,23 +288,23 @@
         for i, tester in enumerate(testers):
             table_names += get_table_name(tester)
             closed[tester] = False
 
         cs.print(f"[blue]{table_names}[/blue]")
         cs.print(rstring(table_horizontal))
         cs.print(rstring(table_header))
-        for i in range(max(map(len, [tester.ext_log for tester in testers]))):
+        for i in range(max(map(len, [tester.ext_log for tester in testers])) + 1):
             table_line = ""
             for j, tester in enumerate(testers):
-                if i >= len(tester.ext_log) - 1:
+                if i >= len(tester.ext_log):
                     if closed[tester] is False:
                         table_line += f"{' ' * distance if j > 0 else ''}{table_horizontal}"
                         closed[tester] = True
                     else:
-                        table_line += " " * 77
+                        table_line += " " * LENGTH
                 else:
                     if j > 0:
                         table_line += " " * distance
                     table_line += get_table_line(tester, i)
             cs.print(table_line)
```

