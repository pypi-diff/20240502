# Comparing `tmp/innertube-de-1.0.0.post1.tar.gz` & `tmp/innertube-de-1.0.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innertube-de-1.0.0.post1.tar", last modified: Thu May  2 11:29:06 2024, max compression
+gzip compressed data, was "innertube-de-1.0.0.post2.tar", last modified: Thu May  2 13:05:03 2024, max compression
```

## Comparing `innertube-de-1.0.0.post1.tar` & `innertube-de-1.0.0.post2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/PKG-INFO
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2708 2024-05-02 11:24:00.000000 innertube-de-1.0.0.post1/README.md
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/innertube_de/
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1703 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/__init__.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     5262 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/containers.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8158 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/endpoints.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     1098 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/errors.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    58862 2024-05-02 11:22:37.000000 innertube-de-1.0.0.post1/innertube_de/extractor.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4223 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/itags.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    26289 2024-05-02 11:22:37.000000 innertube-de-1.0.0.post1/innertube_de/items.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3970 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/stream.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     4742 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post1/innertube_de/types.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8543 2024-05-02 10:48:08.000000 innertube-de-1.0.0.post1/innertube_de/utils.py
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/innertube_de.egg-info/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-02 11:29:06.000000 innertube-de-1.0.0.post1/innertube_de.egg-info/PKG-INFO
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)      416 2024-05-02 11:29:06.000000 innertube-de-1.0.0.post1/innertube_de.egg-info/SOURCES.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)        1 2024-05-02 11:29:06.000000 innertube-de-1.0.0.post1/innertube_de.egg-info/dependency_links.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       13 2024-05-02 11:29:06.000000 innertube-de-1.0.0.post1/innertube_de.egg-info/top_level.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       38 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/setup.cfg
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)      785 2024-05-02 11:23:51.000000 innertube-de-1.0.0.post1/setup.py
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 11:29:06.219979 innertube-de-1.0.0.post1/tests/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)    13806 2024-05-02 11:22:31.000000 innertube-de-1.0.0.post1/tests/tester.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 13:05:03.738231 innertube-de-1.0.0.post2/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-02 13:05:03.738231 innertube-de-1.0.0.post2/PKG-INFO
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2708 2024-05-02 13:02:55.000000 innertube-de-1.0.0.post2/README.md
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 13:05:03.738231 innertube-de-1.0.0.post2/innertube_de/
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1703 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post2/innertube_de/__init__.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     5262 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post2/innertube_de/containers.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8158 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post2/innertube_de/endpoints.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     1098 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post2/innertube_de/errors.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    60151 2024-05-02 13:02:55.000000 innertube-de-1.0.0.post2/innertube_de/extractor.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4223 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post2/innertube_de/itags.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    26289 2024-05-02 11:22:37.000000 innertube-de-1.0.0.post2/innertube_de/items.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3970 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post2/innertube_de/stream.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     4796 2024-05-02 13:02:55.000000 innertube-de-1.0.0.post2/innertube_de/types.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8543 2024-05-02 10:48:08.000000 innertube-de-1.0.0.post2/innertube_de/utils.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 13:05:03.738231 innertube-de-1.0.0.post2/innertube_de.egg-info/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-02 13:05:03.000000 innertube-de-1.0.0.post2/innertube_de.egg-info/PKG-INFO
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)      416 2024-05-02 13:05:03.000000 innertube-de-1.0.0.post2/innertube_de.egg-info/SOURCES.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)        1 2024-05-02 13:05:03.000000 innertube-de-1.0.0.post2/innertube_de.egg-info/dependency_links.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       13 2024-05-02 13:05:03.000000 innertube-de-1.0.0.post2/innertube_de.egg-info/top_level.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       38 2024-05-02 13:05:03.738231 innertube-de-1.0.0.post2/setup.cfg
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)      785 2024-05-02 13:02:55.000000 innertube-de-1.0.0.post2/setup.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 13:05:03.738231 innertube-de-1.0.0.post2/tests/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)    13806 2024-05-02 11:22:31.000000 innertube-de-1.0.0.post2/tests/tester.py
```

### Comparing `innertube-de-1.0.0.post1/PKG-INFO` & `innertube-de-1.0.0.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: innertube-de
-Version: 1.0.0.post1
+Version: 1.0.0.post2
 Summary: InnerTube Data Extractor
 Home-page: https://github.com/g3nsy/innertube-de
 Author: g3nsy
 Author-email: g3nsydev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-1-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-2-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube-de-1.0.0.post1/README.md` & `innertube-de-1.0.0.post2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-1-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-2-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube-de-1.0.0.post1/innertube_de/__init__.py` & `innertube-de-1.0.0.post2/innertube_de/__init__.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post1/innertube_de/containers.py` & `innertube-de-1.0.0.post2/innertube_de/containers.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post1/innertube_de/endpoints.py` & `innertube-de-1.0.0.post2/innertube_de/endpoints.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post1/innertube_de/errors.py` & `innertube-de-1.0.0.post2/innertube_de/errors.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post1/innertube_de/extractor.py` & `innertube-de-1.0.0.post2/innertube_de/extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,27 @@
 
             # YouTube Music
             if "secondaryContents" in ds:
                 return self._get(ds, "secondaryContents", "sectionListRenderer", "contents")
 
             # YouTube
             elif "tabs" in ds:
-                return self._get(ds, "tabs", 0, "tabRenderer", "content", "sectionListRenderer", "contents")
+                tmp = self._get(
+                    ds, "tabs", 0, "tabRenderer", "content", "sectionListRenderer", "contents"
+                )
+                shelves: List[Dict] = []
+                for entry in tmp:
+                    if ItemStructType.CONTINUATION_ITEM.value in entry:
+                        continue
+                    tmp1 = self._get(entry, ShelfStructType.ITEM_SECTION.value, "contents", 0)
+                    if ItemStructType.CHANNEL_VIDEO_PLAYER.value in tmp1:
+                        shelves.append({ShelfStructType.CHANNEL_SHELF.value: {"contents": [tmp1]}})
+                    else:
+                        shelves.append(tmp1)
+                return shelves
             else:
                 raise AccessError(data=ds)
 
         # YouTube Music
         elif ResultStructType.SINGLE_COLUMN_BROWSE_RESULTS.value in data:
             tmp1 = self._get(
                 data, ResultStructType.SINGLE_COLUMN_BROWSE_RESULTS.value, "tabs", 0,
@@ -306,15 +318,15 @@
 
             if tmp1 is not None:
                 tmp2 = self._get(tmp1, "contents", 0, opt=True)
                 if tmp2 is not None:
                     if ShelfStructType.GRID.value in tmp2:
                         return self._get(tmp1, "contents")
                     elif ShelfStructType.MUSIC_PLAYLIST_SHELF.value in tmp2:
-                        return self._get(tmp1, "contents", 0, "musicPlaylistShelfRenderer", "contents")
+                        return [tmp2]
                     elif ShelfStructType.MUSIC_CAROUSEL_SHELF.value in tmp2:
                         return self._get(tmp1, "contents")
                     elif ShelfStructType.MUSIC_SHELF.value in tmp2:
                         return self._get(tmp1, "contents")
                     else:
                         raise AccessError(data=tmp2)
                 else:
@@ -417,14 +429,19 @@
             ds = self._get(entry, ShelfStructType.MUSIC_SHELF.value)
             name = self._get(ds, "title", "runs", 0, "text", opt=True)
             contents = self._get(ds, "contents")
             endpoint = self._extract_endpoint(self._get(ds, "bottomEndpoint", opt=True))
             shelf = Shelf(name=name, endpoint=endpoint)
             item_type = get_item_type(name)
 
+        elif ShelfStructType.MUSIC_PLAYLIST_SHELF.value in entry:
+            ds = self._get(entry, ShelfStructType.MUSIC_PLAYLIST_SHELF.value)
+            contents = self._get(ds, "contents")
+            shelf = Shelf()
+
         # YouTube Music
         elif ShelfStructType.MUSIC_CAROUSEL_SHELF.value in entry:
             ds = self._get(entry, ShelfStructType.MUSIC_CAROUSEL_SHELF.value)
             contents = self._get(ds, "contents")
             name = self._get(
                 ds, "header", "musicCarouselShelfBasicHeaderRenderer", "title", "runs", 0, "text"
             )
@@ -490,14 +507,19 @@
 
         # YouTube
         elif ShelfStructType.PLAYLIST_VIDEO_LIST_CONTINUATION.value in entry:
             contents = self._get(entry, ShelfStructType.PLAYLIST_VIDEO_LIST_CONTINUATION.value, "contents")
             shelf = Shelf()
 
         # YouTube
+        elif ShelfStructType.PLAYLIST_VIDEO_LIST.value in entry:
+            contents = self._get(entry, ShelfStructType.PLAYLIST_VIDEO_LIST.value, "contents")
+            shelf = Shelf()
+
+        # YouTube
         elif ShelfStructType.CHANNEL_SHELF.value in entry:
             contents = self._get(entry, ShelfStructType.CHANNEL_SHELF.value, "contents")
             shelf = Shelf()
 
         elif ShelfStructType.REEL_SHELF.value in entry:
             ds = self._get(entry, ShelfStructType.REEL_SHELF.value)
             name = self._get(ds, "title", "runs", 0, "text", opt=True)
@@ -1180,23 +1202,26 @@
             if canonical_base_url is None:
                 endpoint = BrowseEndpoint(browse_id=browse_id, params=params)
             else:
                 endpoint = YouTubeBrowseEndpoint(
                     browse_id=browse_id, params=params, canonical_base_url=canonical_base_url
                 )
 
-        elif (
-            EndpointType.WATCH.value in data
-            or EndpointType.REEL_WATCH.value in data
-        ):
+        elif EndpointType.WATCH.value in data:
             video_id = self._get(data, EndpointType.WATCH.value, "videoId")
             playlist_id = self._get(data, EndpointType.WATCH.value, "playlistId", opt=True)
             params = self._get(data, EndpointType.WATCH.value, "params", opt=True)
             endpoint = WatchEndpoint(video_id=video_id, playlist_id=playlist_id, params=params)
 
+        elif EndpointType.REEL_WATCH.value in data:
+            video_id = self._get(data, EndpointType.REEL_WATCH.value, "videoId")
+            playlist_id = self._get(data, EndpointType.REEL_WATCH.value, "playlistId", opt=True)
+            params = self._get(data, EndpointType.REEL_WATCH.value, "params", opt=True)
+            endpoint = WatchEndpoint(video_id=video_id, playlist_id=playlist_id, params=params)
+
         elif EndpointType.SEARCH.value in data:
             query = self._get(data, EndpointType.SEARCH.value, "query")
             params = self._get(data, EndpointType.SEARCH.value, "params", opt=True)
             endpoint = SearchEndpoint(query=query, params=params)
 
         elif EndpointType.URL.value in data:
             url = self._get(data, EndpointType.URL.value, "url")
```

### Comparing `innertube-de-1.0.0.post1/innertube_de/itags.py` & `innertube-de-1.0.0.post2/innertube_de/itags.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post1/innertube_de/items.py` & `innertube-de-1.0.0.post2/innertube_de/items.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post1/innertube_de/stream.py` & `innertube-de-1.0.0.post2/innertube_de/stream.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post1/innertube_de/types.py` & `innertube-de-1.0.0.post2/innertube_de/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     PLAYLIST_PANEL = "playlistPanelRenderer"
     SHOWING_RESULTS_FOR = "showingResultsForRenderer"
 
     # YouTube
     SHELF = "shelfRenderer"
     SECONDARY_RESULTS = "secondaryResults"
     PLAYLIST_VIDEO_LIST_CONTINUATION = "playlistVideoListContinuation"
+    PLAYLIST_VIDEO_LIST = "playlistVideoListRenderer"
     REEL_SHELF = "reelShelfRenderer"
     VERTICAL_WATCH_CARD_LIST = "verticalWatchCardListRenderer"
     HORIZONTAL_CARD_LIST_RENDERER = "horizontalCardListRenderer"
 
     # YouTube - custom
     NEXT_PRIMARY_SHELF = "nextPrimaryShelf"
     CHANNEL_SHELF = "channelShelf"
```

### Comparing `innertube-de-1.0.0.post1/innertube_de/utils.py` & `innertube-de-1.0.0.post2/innertube_de/utils.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post1/innertube_de.egg-info/PKG-INFO` & `innertube-de-1.0.0.post2/innertube_de.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: innertube-de
-Version: 1.0.0.post1
+Version: 1.0.0.post2
 Summary: InnerTube Data Extractor
 Home-page: https://github.com/g3nsy/innertube-de
 Author: g3nsy
 Author-email: g3nsydev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-1-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-2-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube-de-1.0.0.post1/setup.py` & `innertube-de-1.0.0.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 here = Path(__file__).parent
 long_description = (here / "README.md").read_text()
 
 
 setup(
     name="innertube-de",
-    version="1.0.0-1",
+    version="1.0.0-2",
     description="InnerTube Data Extractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="g3nsy",
     author_email="g3nsydev@gmail.com",
     python_requires=">=3.6.0",
     url="https://github.com/g3nsy/innertube-de",
```

### Comparing `innertube-de-1.0.0.post1/tests/tester.py` & `innertube-de-1.0.0.post2/tests/tester.py`

 * *Files identical despite different names*

