# Comparing `tmp/anipie-0.0.8.tar.gz` & `tmp/anipie-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipie-0.0.8.tar", last modified: Wed Jan  3 19:25:53 2024, max compression
+gzip compressed data, was "anipie-0.0.9.tar", last modified: Thu May  2 11:31:11 2024, max compression
```

## Comparing `anipie-0.0.8.tar` & `anipie-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 19:25:53.329768 anipie-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-03 19:25:45.000000 anipie-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-03 19:25:53.329768 anipie-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 19:25:53.329768 anipie-0.0.8/anipie/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-03 19:25:45.000000 anipie-0.0.8/anipie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-01-03 19:25:45.000000 anipie-0.0.8/anipie/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-01-03 19:25:45.000000 anipie-0.0.8/anipie/search_by_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 19:25:53.329768 anipie-0.0.8/anipie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-03 19:25:53.000000 anipie-0.0.8/anipie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-03 19:25:53.000000 anipie-0.0.8/anipie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 19:25:53.000000 anipie-0.0.8/anipie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-03 19:25:53.000000 anipie-0.0.8/anipie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-03 19:25:53.000000 anipie-0.0.8/anipie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 19:25:53.329768 anipie-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-03 19:25:47.000000 anipie-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:31:11.793190 anipie-0.0.9/
+-rw-rw-rw-   0        0        0     1089 2023-07-12 10:40:29.000000 anipie-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      493 2024-05-02 11:31:11.792189 anipie-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1360 2024-01-03 19:07:16.000000 anipie-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 11:31:11.770189 anipie-0.0.9/anipie/
+-rw-rw-rw-   0        0        0      124 2024-01-03 17:37:53.000000 anipie-0.0.9/anipie/__init__.py
+-rw-rw-rw-   0        0        0     1429 2024-02-27 03:41:48.000000 anipie-0.0.9/anipie/queries.py
+-rw-rw-rw-   0        0        0     5599 2024-05-02 11:14:29.000000 anipie-0.0.9/anipie/search_by_query.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:31:11.791189 anipie-0.0.9/anipie.egg-info/
+-rw-rw-rw-   0        0        0      493 2024-05-02 11:31:11.000000 anipie-0.0.9/anipie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-02 11:31:11.000000 anipie-0.0.9/anipie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 11:31:11.000000 anipie-0.0.9/anipie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 11:31:11.000000 anipie-0.0.9/anipie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-02 11:31:11.000000 anipie-0.0.9/anipie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 11:31:11.793190 anipie-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      955 2024-05-02 11:29:45.000000 anipie-0.0.9/setup.py
```

### Comparing `anipie-0.0.8/LICENSE` & `anipie-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Lynniswaifu
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Lynniswaifu
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `anipie-0.0.8/anipie/queries.py` & `anipie-0.0.9/anipie/queries.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-ANIME_API_URL = 'https://graphql.anilist.co'
-
-
-ANIME_QUERY = '''
-query ($search: String! $type: MediaType!) { 
-            Media (search: $search type: $type) { 
-                id
-                title {
-                    romaji
-                    english
-                }
-                status
-                description
-                averageScore
-                startDate {
-                    year
-                    month
-                    day
-                }
-                endDate {
-                    year
-                    month
-                    day
-                }
-                coverImage {
-                    large  
-                }
-                genres
-                siteUrl
-                episodes
-                season
-                format
-            }
-        }
-'''
-
-MANGA_QUERY = '''
-query ($search: String! $type: MediaType!) { 
-    Media (search: $search type: $type) { 
-        id
-        title {
-            romaji
-            english
-        }
-        status
-        description
-        averageScore
-        startDate {
-            year
-            month
-            day
-        }
-        endDate {
-            year
-            month
-            day
-        }
-        coverImage {
-            large  
-        }
-        genres
-        siteUrl
-        chapters
-        volumes
-        format
-    }
-}
-'''
+ANIME_API_URL = "https://graphql.anilist.co"
+
+
+ANIME_QUERY = """
+query ($search: String! $type: MediaType!) { 
+            Media (search: $search type: $type) { 
+                id
+                title {
+                    romaji
+                    english
+                }
+                status
+                description
+                averageScore
+                startDate {
+                    year
+                    month
+                    day
+                }
+                endDate {
+                    year
+                    month
+                    day
+                }
+                coverImage {
+                    large  
+                }
+                genres
+                siteUrl
+                episodes
+                season
+                format
+            }
+        }
+"""
+
+MANGA_QUERY = """
+query ($search: String! $type: MediaType!) { 
+    Media (search: $search type: $type) { 
+        id
+        title {
+            romaji
+            english
+        }
+        status
+        description
+        averageScore
+        startDate {
+            year
+            month
+            day
+        }
+        endDate {
+            year
+            month
+            day
+        }
+        coverImage {
+            large  
+        }
+        genres
+        siteUrl
+        chapters
+        volumes
+        format
+    }
+}
+"""
```

