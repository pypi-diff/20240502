# Comparing `tmp/fftrack-0.1.0.tar.gz` & `tmp/fftrack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fftrack-0.1.0.tar", last modified: Thu May  2 10:12:45 2024, max compression
+gzip compressed data, was "fftrack-0.1.1.tar", last modified: Thu May  2 10:30:14 2024, max compression
```

## Comparing `fftrack-0.1.0.tar` & `fftrack-0.1.1.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.869667 fftrack-0.1.0/
--rw-r--r--   0 nicolas    (501) staff       (20)      123 2024-05-02 09:53:34.000000 fftrack-0.1.0/MANIFEST.in
--rw-r--r--   0 nicolas    (501) staff       (20)     2560 2024-05-02 10:12:45.869382 fftrack-0.1.0/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)     1487 2024-05-02 09:53:22.000000 fftrack-0.1.0/README.md
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.851283 fftrack-0.1.0/fftrack/
--rw-r--r--   0 nicolas    (501) staff       (20)      475 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)       59 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/__main__.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.854059 fftrack-0.1.0/fftrack/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)      562 2024-04-29 16:25:05.000000 fftrack-0.1.0/fftrack/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      562 2024-04-29 16:26:08.000000 fftrack-0.1.0/fftrack/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      243 2024-04-18 10:03:05.000000 fftrack-0.1.0/fftrack/__pycache__/__main__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      243 2024-04-23 08:20:35.000000 fftrack-0.1.0/fftrack/__pycache__/__main__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     1219 2024-04-18 16:45:54.000000 fftrack-0.1.0/fftrack/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     1254 2024-05-02 10:10:11.000000 fftrack-0.1.0/fftrack/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     3061 2024-04-23 07:32:24.000000 fftrack-0.1.0/fftrack/__pycache__/main.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     2999 2024-05-02 10:00:43.000000 fftrack-0.1.0/fftrack/__pycache__/main.cpython-39.pyc
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.856046 fftrack-0.1.0/fftrack/audio/
--rw-r--r--   0 nicolas    (501) staff       (20)     9160 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/audio/AudioProcessing.py
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-04-10 15:51:20.000000 fftrack-0.1.0/fftrack/audio/__init__.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.859714 fftrack-0.1.0/fftrack/audio/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)     7618 2024-04-29 16:25:06.000000 fftrack-0.1.0/fftrack/audio/__pycache__/AudioProcessing.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     7600 2024-04-29 16:26:09.000000 fftrack-0.1.0/fftrack/audio/__pycache__/AudioProcessing.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      179 2024-04-10 15:51:24.000000 fftrack-0.1.0/fftrack/audio/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      179 2024-04-23 08:06:43.000000 fftrack-0.1.0/fftrack/audio/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     6310 2024-04-10 11:03:17.000000 fftrack-0.1.0/fftrack/audio/__pycache__/audio_compare.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     3613 2024-04-18 08:38:22.000000 fftrack-0.1.0/fftrack/audio/__pycache__/audio_reader.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     3613 2024-04-29 16:26:24.000000 fftrack-0.1.0/fftrack/audio/__pycache__/audio_reader.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     9345 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/audio/audio_compare.py
--rw-r--r--   0 nicolas    (501) staff       (20)     3700 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/audio/audio_reader.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1203 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/audio/main_audio.py
--rw-r--r--   0 nicolas    (501) staff       (20)      465 2024-04-18 16:39:51.000000 fftrack-0.1.0/fftrack/config.json
--rw-r--r--   0 nicolas    (501) staff       (20)     1077 2024-05-02 10:09:46.000000 fftrack-0.1.0/fftrack/config.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.861698 fftrack-0.1.0/fftrack/database/
--rw-r--r--   0 nicolas    (501) staff       (20)       78 2024-03-31 21:16:40.000000 fftrack-0.1.0/fftrack/database/__init__.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.863355 fftrack-0.1.0/fftrack/database/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)      289 2024-03-31 21:19:52.000000 fftrack-0.1.0/fftrack/database/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      289 2024-04-23 08:06:41.000000 fftrack-0.1.0/fftrack/database/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4825 2024-04-29 16:25:05.000000 fftrack-0.1.0/fftrack/database/__pycache__/db_manager.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4817 2024-04-29 16:26:08.000000 fftrack-0.1.0/fftrack/database/__pycache__/db_manager.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     2313 2024-04-29 16:25:05.000000 fftrack-0.1.0/fftrack/database/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     2313 2024-04-29 16:26:09.000000 fftrack-0.1.0/fftrack/database/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4819 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/database/db_manager.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1652 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/database/main_db.py
--rw-r--r--   0 nicolas    (501) staff       (20)     2032 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/database/models.py
--rw-r--r--   0 nicolas    (501) staff       (20)     3275 2024-05-02 09:53:22.000000 fftrack-0.1.0/fftrack/main.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.863890 fftrack-0.1.0/fftrack/matching/
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.865226 fftrack-0.1.0/fftrack/matching/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)      221 2024-04-09 09:17:26.000000 fftrack-0.1.0/fftrack/matching/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      221 2024-04-23 08:20:35.000000 fftrack-0.1.0/fftrack/matching/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     1926 2024-04-09 09:49:28.000000 fftrack-0.1.0/fftrack/matching/__pycache__/main_matching.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4728 2024-04-18 10:02:12.000000 fftrack-0.1.0/fftrack/matching/__pycache__/matcher.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4736 2024-04-29 16:26:24.000000 fftrack-0.1.0/fftrack/matching/__pycache__/matcher.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     6334 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/matching/main_matching.py
--rw-r--r--   0 nicolas    (501) staff       (20)     7345 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/matching/matcher.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.866080 fftrack-0.1.0/fftrack/scripts/
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-05-02 09:54:41.000000 fftrack-0.1.0/fftrack/scripts/__init__.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.866575 fftrack-0.1.0/fftrack/scripts/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)      181 2024-04-23 08:42:12.000000 fftrack-0.1.0/fftrack/scripts/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4171 2024-04-23 08:45:30.000000 fftrack-0.1.0/fftrack/scripts/__pycache__/populate_database.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4926 2024-05-02 09:54:41.000000 fftrack-0.1.0/fftrack/scripts/populate_database.py
--rw-r--r--   0 nicolas    (501) staff       (20)      261 2024-05-02 09:54:41.000000 fftrack-0.1.0/fftrack/scripts/songs_to_download.csv
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.867620 fftrack-0.1.0/fftrack/ui/
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.867730 fftrack-0.1.0/fftrack/ui/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)     2323 2024-04-18 08:54:51.000000 fftrack-0.1.0/fftrack/ui/__pycache__/main_cli_nicolas.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     2533 2024-04-18 09:05:36.000000 fftrack-0.1.0/fftrack/ui/cli.py
--rw-r--r--   0 nicolas    (501) staff       (20)     4525 2024-04-18 09:05:36.000000 fftrack-0.1.0/fftrack/ui/main_cli.py
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-04-29 16:19:29.000000 fftrack-0.1.0/fftrack/ui/main_cli_nicolas.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:12:45.852269 fftrack-0.1.0/fftrack.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)     2560 2024-05-02 10:12:45.000000 fftrack-0.1.0/fftrack.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)     2315 2024-05-02 10:12:45.000000 fftrack-0.1.0/fftrack.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2024-05-02 10:12:45.000000 fftrack-0.1.0/fftrack.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas    (501) staff       (20)      104 2024-05-02 10:12:45.000000 fftrack-0.1.0/fftrack.egg-info/entry_points.txt
--rw-r--r--   0 nicolas    (501) staff       (20)     1232 2024-05-02 10:12:45.000000 fftrack-0.1.0/fftrack.egg-info/requires.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        8 2024-05-02 10:12:45.000000 fftrack-0.1.0/fftrack.egg-info/top_level.txt
--rw-r--r--   0 nicolas    (501) staff       (20)     2012 2024-04-29 16:19:29.000000 fftrack-0.1.0/pyproject.toml
--rw-r--r--   0 nicolas    (501) staff       (20)     1239 2024-04-29 16:19:29.000000 fftrack-0.1.0/requirements.txt
--rw-r--r--   0 nicolas    (501) staff       (20)       38 2024-05-02 10:12:45.869726 fftrack-0.1.0/setup.cfg
--rw-r--r--   0 nicolas    (501) staff       (20)     2626 2024-05-02 10:04:11.000000 fftrack-0.1.0/setup.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.778650 fftrack-0.1.1/
+-rw-r--r--   0 nicolas    (501) staff       (20)      123 2024-05-02 09:53:34.000000 fftrack-0.1.1/MANIFEST.in
+-rw-r--r--   0 nicolas    (501) staff       (20)      299 2024-05-02 10:30:14.778447 fftrack-0.1.1/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)     1487 2024-05-02 09:53:22.000000 fftrack-0.1.1/README.md
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.762442 fftrack-0.1.1/fftrack/
+-rw-r--r--   0 nicolas    (501) staff       (20)      475 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)       59 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/__main__.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.766212 fftrack-0.1.1/fftrack/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)      562 2024-04-29 16:25:05.000000 fftrack-0.1.1/fftrack/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      562 2024-04-29 16:26:08.000000 fftrack-0.1.1/fftrack/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      243 2024-04-18 10:03:05.000000 fftrack-0.1.1/fftrack/__pycache__/__main__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      243 2024-04-23 08:20:35.000000 fftrack-0.1.1/fftrack/__pycache__/__main__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     1213 2024-05-02 10:19:16.000000 fftrack-0.1.1/fftrack/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     1254 2024-05-02 10:10:11.000000 fftrack-0.1.1/fftrack/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     3011 2024-05-02 10:19:16.000000 fftrack-0.1.1/fftrack/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     2999 2024-05-02 10:00:43.000000 fftrack-0.1.1/fftrack/__pycache__/main.cpython-39.pyc
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.768126 fftrack-0.1.1/fftrack/audio/
+-rw-r--r--   0 nicolas    (501) staff       (20)     9160 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/audio/AudioProcessing.py
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-04-10 15:51:20.000000 fftrack-0.1.1/fftrack/audio/__init__.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.770466 fftrack-0.1.1/fftrack/audio/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)     7618 2024-04-29 16:25:06.000000 fftrack-0.1.1/fftrack/audio/__pycache__/AudioProcessing.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     7600 2024-04-29 16:26:09.000000 fftrack-0.1.1/fftrack/audio/__pycache__/AudioProcessing.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      179 2024-04-10 15:51:24.000000 fftrack-0.1.1/fftrack/audio/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      179 2024-04-23 08:06:43.000000 fftrack-0.1.1/fftrack/audio/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     6310 2024-04-10 11:03:17.000000 fftrack-0.1.1/fftrack/audio/__pycache__/audio_compare.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     3613 2024-05-02 10:19:15.000000 fftrack-0.1.1/fftrack/audio/__pycache__/audio_reader.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     3613 2024-04-29 16:26:24.000000 fftrack-0.1.1/fftrack/audio/__pycache__/audio_reader.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     9345 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/audio/audio_compare.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     3700 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/audio/audio_reader.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1203 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/audio/main_audio.py
+-rw-r--r--   0 nicolas    (501) staff       (20)      465 2024-04-18 16:39:51.000000 fftrack-0.1.1/fftrack/config.json
+-rw-r--r--   0 nicolas    (501) staff       (20)     1077 2024-05-02 10:09:46.000000 fftrack-0.1.1/fftrack/config.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.771432 fftrack-0.1.1/fftrack/database/
+-rw-r--r--   0 nicolas    (501) staff       (20)       78 2024-03-31 21:16:40.000000 fftrack-0.1.1/fftrack/database/__init__.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.773086 fftrack-0.1.1/fftrack/database/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)      289 2024-03-31 21:19:52.000000 fftrack-0.1.1/fftrack/database/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      289 2024-04-23 08:06:41.000000 fftrack-0.1.1/fftrack/database/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4825 2024-04-29 16:25:05.000000 fftrack-0.1.1/fftrack/database/__pycache__/db_manager.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4817 2024-04-29 16:26:08.000000 fftrack-0.1.1/fftrack/database/__pycache__/db_manager.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     2313 2024-04-29 16:25:05.000000 fftrack-0.1.1/fftrack/database/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     2313 2024-04-29 16:26:09.000000 fftrack-0.1.1/fftrack/database/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4819 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/database/db_manager.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1652 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/database/main_db.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2032 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/database/models.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     3275 2024-05-02 09:53:22.000000 fftrack-0.1.1/fftrack/main.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.773717 fftrack-0.1.1/fftrack/matching/
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-05-02 10:28:07.000000 fftrack-0.1.1/fftrack/matching/__init__.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.775041 fftrack-0.1.1/fftrack/matching/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)      221 2024-04-09 09:17:26.000000 fftrack-0.1.1/fftrack/matching/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      221 2024-04-23 08:20:35.000000 fftrack-0.1.1/fftrack/matching/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     1926 2024-04-09 09:49:28.000000 fftrack-0.1.1/fftrack/matching/__pycache__/main_matching.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4728 2024-05-02 10:19:16.000000 fftrack-0.1.1/fftrack/matching/__pycache__/matcher.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4736 2024-04-29 16:26:24.000000 fftrack-0.1.1/fftrack/matching/__pycache__/matcher.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     6334 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/matching/main_matching.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     7345 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/matching/matcher.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.775659 fftrack-0.1.1/fftrack/scripts/
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-05-02 09:54:41.000000 fftrack-0.1.1/fftrack/scripts/__init__.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.776286 fftrack-0.1.1/fftrack/scripts/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)      181 2024-04-23 08:42:12.000000 fftrack-0.1.1/fftrack/scripts/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4171 2024-04-23 08:45:30.000000 fftrack-0.1.1/fftrack/scripts/__pycache__/populate_database.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4926 2024-05-02 09:54:41.000000 fftrack-0.1.1/fftrack/scripts/populate_database.py
+-rw-r--r--   0 nicolas    (501) staff       (20)      261 2024-05-02 09:54:41.000000 fftrack-0.1.1/fftrack/scripts/songs_to_download.csv
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.777421 fftrack-0.1.1/fftrack/ui/
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.777530 fftrack-0.1.1/fftrack/ui/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)     2323 2024-04-18 08:54:51.000000 fftrack-0.1.1/fftrack/ui/__pycache__/main_cli_nicolas.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     2533 2024-04-18 09:05:36.000000 fftrack-0.1.1/fftrack/ui/cli.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     4525 2024-04-18 09:05:36.000000 fftrack-0.1.1/fftrack/ui/main_cli.py
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-04-29 16:19:29.000000 fftrack-0.1.1/fftrack/ui/main_cli_nicolas.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 10:30:14.763429 fftrack-0.1.1/fftrack.egg-info/
+-rw-r--r--   0 nicolas    (501) staff       (20)      299 2024-05-02 10:30:14.000000 fftrack-0.1.1/fftrack.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)     2344 2024-05-02 10:30:14.000000 fftrack-0.1.1/fftrack.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2024-05-02 10:30:14.000000 fftrack-0.1.1/fftrack.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)      105 2024-05-02 10:30:14.000000 fftrack-0.1.1/fftrack.egg-info/entry_points.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)     1232 2024-05-02 10:30:14.000000 fftrack-0.1.1/fftrack.egg-info/requires.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        8 2024-05-02 10:30:14.000000 fftrack-0.1.1/fftrack.egg-info/top_level.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)     2012 2024-04-29 16:19:29.000000 fftrack-0.1.1/pyproject.toml
+-rw-r--r--   0 nicolas    (501) staff       (20)     1239 2024-04-29 16:19:29.000000 fftrack-0.1.1/requirements.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)       38 2024-05-02 10:30:14.778818 fftrack-0.1.1/setup.cfg
+-rw-r--r--   0 nicolas    (501) staff       (20)     2626 2024-05-02 10:29:56.000000 fftrack-0.1.1/setup.py
```

### Comparing `fftrack-0.1.0/README.md` & `fftrack-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/__pycache__/__init__.cpython-38.pyc` & `fftrack-0.1.1/fftrack/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/__pycache__/__init__.cpython-39.pyc` & `fftrack-0.1.1/fftrack/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/__pycache__/config.cpython-38.pyc` & `fftrack-0.1.1/fftrack/__pycache__/config.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr 18 16:43:53 2024 UTC, .py size: 1083 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,76 @@
-00000000: 550d 0d0a 0000 0000 c94d 2166 3b04 0000  U........M!f;...
+00000000: 550d 0d0a 0000 0000 6a66 3366 3504 0000  U.......jf3f5...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
+00000020: 0005 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c00 5a00 6501 6a02 a003 6501 6a02  d.l.Z.e.j...e.j.
-00000050: a004 6505 a101 6402 6403 a103 5a06 6506  ..e...d.d...Z.e.
-00000060: 6601 6404 6405 8401 5a07 6506 6601 6406  f.d.d...Z.e.f.d.
-00000070: 6407 8401 5a08 6401 5300 2908 e900 0000  d...Z.d.S.).....
-00000080: 004e 7a02 2e2e 7a0b 636f 6e66 6967 2e6a  .Nz...z.config.j
-00000090: 736f 6e63 0100 0000 0000 0000 0000 0000  sonc............
-000000a0: 0300 0000 0900 0000 4300 0000 733e 0000  ........C...s>..
-000000b0: 0074 006a 01a0 027c 00a1 0173 1a74 0364  .t.j...|...s.t.d
-000000c0: 017c 009b 009d 0283 0182 0174 047c 0064  .|.........t.|.d
-000000d0: 0283 028f 107d 0174 05a0 067c 01a1 017d  .....}.t...|...}
-000000e0: 0257 0035 0051 0052 0058 007c 0253 0029  .W.5.Q.R.X.|.S.)
-000000f0: 037a ac0a 2020 2020 4c6f 6164 2063 6f6e  .z..    Load con
-00000100: 6669 6775 7261 7469 6f6e 2064 6174 6120  figuration data 
-00000110: 6672 6f6d 2061 204a 534f 4e20 6669 6c65  from a JSON file
-00000120: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00000130: 2020 2020 2063 6f6e 6669 675f 6669 6c65       config_file
-00000140: 5f70 6174 6820 2873 7472 293a 2050 6174  _path (str): Pat
-00000150: 6820 746f 2074 6865 204a 534f 4e20 636f  h to the JSON co
-00000160: 6e66 6967 2066 696c 652e 0a0a 2020 2020  nfig file...    
-00000170: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00000180: 2064 6963 743a 2043 6f6e 6669 6775 7261   dict: Configura
-00000190: 7469 6f6e 2064 6174 612e 0a20 2020 207a  tion data..    z
-000001a0: 1743 6f6e 6669 6720 6669 6c65 206e 6f74  .Config file not
-000001b0: 2066 6f75 6e64 3a20 da01 7229 07da 026f   found: ..r)...o
-000001c0: 73da 0470 6174 68da 0665 7869 7374 73da  s..path..exists.
-000001d0: 1146 696c 654e 6f74 466f 756e 6445 7272  .FileNotFoundErr
-000001e0: 6f72 da04 6f70 656e da04 6a73 6f6e da04  or..open..json..
-000001f0: 6c6f 6164 2903 da10 636f 6e66 6967 5f66  load)...config_f
-00000200: 696c 655f 7061 7468 da01 66da 0b63 6f6e  ile_path..f..con
-00000210: 6669 675f 6461 7461 a900 720d 0000 00fa  fig_data..r.....
-00000220: 502f 5573 6572 732f 6e69 636f 6c61 732f  P/Users/nicolas/
-00000230: 4465 7665 6c6f 7065 722f 776f 726b 7370  Developer/worksp
-00000240: 6163 652f 556e 692f 4c32 2f53 342f 5072  ace/Uni/L2/S4/Pr
-00000250: 6f6a 6574 2f64 6f73 7369 6572 5356 4e2f  ojet/dossierSVN/
-00000260: 6666 7472 6163 6b2f 636f 6e66 6967 2e70  fftrack/config.p
-00000270: 79da 0b6c 6f61 645f 636f 6e66 6967 0900  y..load_config..
-00000280: 0000 730a 0000 0000 0a0c 010e 010c 0114  ..s.............
-00000290: 0172 0f00 0000 6302 0000 0000 0000 0000  .r....c.........
-000002a0: 0000 0003 0000 0009 0000 0043 0000 0073  ...........C...s
-000002b0: 3600 0000 7c01 6401 6b08 720c 7400 7d01  6...|.d.k.r.t.}.
-000002c0: 7401 7c01 6402 8302 8f16 7d02 7402 6a03  t.|.d.....}.t.j.
-000002d0: 7c00 7c02 6403 6404 8d03 0100 5700 3500  |.|.d.d.....W.5.
-000002e0: 5100 5200 5800 6401 5300 2905 7aec 0a20  Q.R.X.d.S.).z.. 
-000002f0: 2020 2053 6176 6520 636f 6e66 6967 7572     Save configur
-00000300: 6174 696f 6e20 6461 7461 2074 6f20 6120  ation data to a 
-00000310: 4a53 4f4e 2066 696c 652e 0a0a 2020 2020  JSON file...    
-00000320: 4172 6773 3a0a 2020 2020 2020 2020 636f  Args:.        co
-00000330: 6e66 6967 5f64 6174 6120 2864 6963 7429  nfig_data (dict)
-00000340: 3a20 436f 6e66 6967 7572 6174 696f 6e20  : Configuration 
-00000350: 6461 7461 2074 6f20 7361 7665 2e0a 2020  data to save..  
-00000360: 2020 2020 2020 636f 6e66 6967 5f66 696c        config_fil
-00000370: 655f 7061 7468 2028 7374 7229 3a20 5061  e_path (str): Pa
-00000380: 7468 2074 6f20 7468 6520 4a53 4f4e 2063  th to the JSON c
-00000390: 6f6e 6669 6720 6669 6c65 2e20 4966 204e  onfig file. If N
-000003a0: 6f6e 652c 2075 7365 2074 6865 2064 6566  one, use the def
-000003b0: 6175 6c74 2070 6174 682e 0a0a 2020 2020  ault path...    
-000003c0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-000003d0: 204e 6f6e 650a 2020 2020 4eda 0177 e904   None.    N..w..
-000003e0: 0000 0029 01da 0669 6e64 656e 7429 04da  ...)...indent)..
-000003f0: 1344 4546 4155 4c54 5f43 4f4e 4649 475f  .DEFAULT_CONFIG_
-00000400: 5041 5448 7207 0000 0072 0800 0000 da04  PATHr....r......
-00000410: 6475 6d70 2903 720c 0000 0072 0a00 0000  dump).r....r....
-00000420: 720b 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00000430: 0e00 0000 da0b 7361 7665 5f63 6f6e 6669  ......save_confi
-00000440: 671a 0000 0073 0a00 0000 000b 0801 0401  g....s..........
-00000450: 0c01 1a01 7215 0000 0029 0972 0800 0000  ....r....).r....
-00000460: 7203 0000 0072 0400 0000 da04 6a6f 696e  r....r......join
-00000470: da07 6469 726e 616d 65da 085f 5f66 696c  ..dirname..__fil
-00000480: 655f 5f72 1300 0000 720f 0000 0072 1500  e__r....r....r..
-00000490: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-000004a0: 0072 0e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000004b0: 0100 0000 730a 0000 0008 0208 0108 0218  ....s...........
-000004c0: 030c 11                                  ...
+00000050: a004 6505 a101 6402 a102 5a06 6506 6601  ..e...d...Z.e.f.
+00000060: 6403 6404 8401 5a07 6506 6601 6405 6406  d.d...Z.e.f.d.d.
+00000070: 8401 5a08 6401 5300 2907 e900 0000 004e  ..Z.d.S.)......N
+00000080: 7a0b 636f 6e66 6967 2e6a 736f 6e63 0100  z.config.jsonc..
+00000090: 0000 0000 0000 0000 0000 0300 0000 0900  ................
+000000a0: 0000 4300 0000 733e 0000 0074 006a 01a0  ..C...s>...t.j..
+000000b0: 027c 00a1 0173 1a74 0364 017c 009b 009d  .|...s.t.d.|....
+000000c0: 0283 0182 0174 047c 0064 0283 028f 107d  .....t.|.d.....}
+000000d0: 0174 05a0 067c 01a1 017d 0257 0035 0051  .t...|...}.W.5.Q
+000000e0: 0052 0058 007c 0253 0029 037a ac0a 2020  .R.X.|.S.).z..  
+000000f0: 2020 4c6f 6164 2063 6f6e 6669 6775 7261    Load configura
+00000100: 7469 6f6e 2064 6174 6120 6672 6f6d 2061  tion data from a
+00000110: 204a 534f 4e20 6669 6c65 2e0a 0a20 2020   JSON file...   
+00000120: 2041 7267 733a 0a20 2020 2020 2020 2063   Args:.        c
+00000130: 6f6e 6669 675f 6669 6c65 5f70 6174 6820  onfig_file_path 
+00000140: 2873 7472 293a 2050 6174 6820 746f 2074  (str): Path to t
+00000150: 6865 204a 534f 4e20 636f 6e66 6967 2066  he JSON config f
+00000160: 696c 652e 0a0a 2020 2020 5265 7475 726e  ile...    Return
+00000170: 733a 0a20 2020 2020 2020 2064 6963 743a  s:.        dict:
+00000180: 2043 6f6e 6669 6775 7261 7469 6f6e 2064   Configuration d
+00000190: 6174 612e 0a20 2020 207a 1743 6f6e 6669  ata..    z.Confi
+000001a0: 6720 6669 6c65 206e 6f74 2066 6f75 6e64  g file not found
+000001b0: 3a20 da01 7229 07da 026f 73da 0470 6174  : ..r)...os..pat
+000001c0: 68da 0665 7869 7374 73da 1146 696c 654e  h..exists..FileN
+000001d0: 6f74 466f 756e 6445 7272 6f72 da04 6f70  otFoundError..op
+000001e0: 656e da04 6a73 6f6e da04 6c6f 6164 2903  en..json..load).
+000001f0: da10 636f 6e66 6967 5f66 696c 655f 7061  ..config_file_pa
+00000200: 7468 da01 66da 0b63 6f6e 6669 675f 6461  th..f..config_da
+00000210: 7461 a900 720d 0000 00fa 502f 5573 6572  ta..r.....P/User
+00000220: 732f 6e69 636f 6c61 732f 4465 7665 6c6f  s/nicolas/Develo
+00000230: 7065 722f 776f 726b 7370 6163 652f 556e  per/workspace/Un
+00000240: 692f 4c32 2f53 342f 5072 6f6a 6574 2f64  i/L2/S4/Projet/d
+00000250: 6f73 7369 6572 5356 4e2f 6666 7472 6163  ossierSVN/fftrac
+00000260: 6b2f 636f 6e66 6967 2e70 79da 0b6c 6f61  k/config.py..loa
+00000270: 645f 636f 6e66 6967 0900 0000 730a 0000  d_config....s...
+00000280: 0000 0a0c 010e 010c 0114 0172 0f00 0000  ...........r....
+00000290: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+000002a0: 0009 0000 0043 0000 0073 3600 0000 7c01  .....C...s6...|.
+000002b0: 6401 6b08 720c 7400 7d01 7401 7c01 6402  d.k.r.t.}.t.|.d.
+000002c0: 8302 8f16 7d02 7402 6a03 7c00 7c02 6403  ....}.t.j.|.|.d.
+000002d0: 6404 8d03 0100 5700 3500 5100 5200 5800  d.....W.5.Q.R.X.
+000002e0: 6401 5300 2905 7aec 0a20 2020 2053 6176  d.S.).z..    Sav
+000002f0: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00000300: 6461 7461 2074 6f20 6120 4a53 4f4e 2066  data to a JSON f
+00000310: 696c 652e 0a0a 2020 2020 4172 6773 3a0a  ile...    Args:.
+00000320: 2020 2020 2020 2020 636f 6e66 6967 5f64          config_d
+00000330: 6174 6120 2864 6963 7429 3a20 436f 6e66  ata (dict): Conf
+00000340: 6967 7572 6174 696f 6e20 6461 7461 2074  iguration data t
+00000350: 6f20 7361 7665 2e0a 2020 2020 2020 2020  o save..        
+00000360: 636f 6e66 6967 5f66 696c 655f 7061 7468  config_file_path
+00000370: 2028 7374 7229 3a20 5061 7468 2074 6f20   (str): Path to 
+00000380: 7468 6520 4a53 4f4e 2063 6f6e 6669 6720  the JSON config 
+00000390: 6669 6c65 2e20 4966 204e 6f6e 652c 2075  file. If None, u
+000003a0: 7365 2074 6865 2064 6566 6175 6c74 2070  se the default p
+000003b0: 6174 682e 0a0a 2020 2020 5265 7475 726e  ath...    Return
+000003c0: 733a 0a20 2020 2020 2020 204e 6f6e 650a  s:.        None.
+000003d0: 2020 2020 4eda 0177 e904 0000 0029 01da      N..w.....)..
+000003e0: 0669 6e64 656e 7429 04da 1344 4546 4155  .indent)...DEFAU
+000003f0: 4c54 5f43 4f4e 4649 475f 5041 5448 7207  LT_CONFIG_PATHr.
+00000400: 0000 0072 0800 0000 da04 6475 6d70 2903  ...r......dump).
+00000410: 720c 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+00000420: 0d00 0000 720d 0000 0072 0e00 0000 da0b  ....r....r......
+00000430: 7361 7665 5f63 6f6e 6669 671a 0000 0073  save_config....s
+00000440: 0a00 0000 000b 0801 0401 0c01 1a01 7215  ..............r.
+00000450: 0000 0029 0972 0800 0000 7203 0000 0072  ...).r....r....r
+00000460: 0400 0000 da04 6a6f 696e da07 6469 726e  ......join..dirn
+00000470: 616d 65da 085f 5f66 696c 655f 5f72 1300  ame..__file__r..
+00000480: 0000 720f 0000 0072 1500 0000 720d 0000  ..r....r....r...
+00000490: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+000004a0: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+000004b0: 0000 0008 0208 0108 0216 030c 11         .............
```

### Comparing `fftrack-0.1.0/fftrack/__pycache__/config.cpython-39.pyc` & `fftrack-0.1.1/fftrack/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/__pycache__/main.cpython-38.pyc` & `fftrack-0.1.1/fftrack/ui/__pycache__/main_cli_nicolas.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 23 07:28:18 2024 UTC, .py size: 3318 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,192 +1,146 @@
-00000000: 550d 0d0a 0000 0000 1263 2766 f60c 0000  U........c'f....
+00000000: 550d 0d0a 0000 0000 cadb 2066 a20a 0000  U......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
-00000050: 6402 6c04 6d05 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6406 6c0d 6d0e 5a0e 0100 6500 a00f a100  d.l.m.Z...e.....
-00000090: 5a10 650c 8300 5a11 650a 6407 6408 8d01  Z.e...Z.e.d.d...
-000000a0: 5a12 6508 8300 5a13 650e 6513 8301 5a14  Z.e...Z.e.e...Z.
-000000b0: 6506 a015 a100 5a05 6516 6505 6409 1900  e.....Z.e.e.d...
-000000c0: 8301 5a17 6510 a018 a100 640a 640b 8400  ..Z.e.....d.d...
-000000d0: 8301 5a19 6510 a018 a100 640c 640d 8400  ..Z.e.....d.d...
-000000e0: 8301 5a1a 6510 a018 a100 651b 640e 9c01  ..Z.e.....e.d...
-000000f0: 640f 6410 8404 8301 5a1c 6510 a018 a100  d.d.....Z.e.....
-00000100: 6411 6412 8400 8301 5a1d 6510 a018 a100  d.d.....Z.e.....
-00000110: 651b 6413 9c01 6414 6415 8404 8301 5a1e  e.d...d.d.....Z.
-00000120: 651f 6416 6b02 9001 7202 6510 8300 0100  e.d.k...r.e.....
-00000130: 6401 5300 2917 e900 0000 004e 2901 da06  d.S.)......N)...
-00000140: 636f 6e66 6967 2901 da0f 4461 7461 6261  config)...Databa
-00000150: 7365 4d61 6e61 6765 7229 01da 0f41 7564  seManager)...Aud
-00000160: 696f 5072 6f63 6573 7369 6e67 2901 da0b  ioProcessing)...
-00000170: 4175 6469 6f52 6561 6465 7229 01da 074d  AudioReader)...M
-00000180: 6174 6368 6572 4629 01da 0470 6c6f 745a  atcherF)...plotZ
-00000190: 0b6c 6973 7465 6e5f 7469 6d65 6300 0000  .listen_timec...
-000001a0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-000001b0: 0043 0000 0073 1800 0000 7400 a001 6401  .C...s....t...d.
-000001c0: a101 0100 7400 a001 6402 a101 0100 6400  ....t...d.....d.
-000001d0: 5300 2903 4e7a 1357 656c 636f 6d65 2074  S.).Nz.Welcome t
-000001e0: 6f20 4646 5472 6163 6b21 7a2e 5573 6520  o FFTrack!z.Use 
-000001f0: 7468 6520 2d2d 6865 6c70 2066 6c61 6720  the --help flag 
-00000200: 746f 2073 6565 2061 7661 696c 6162 6c65  to see available
-00000210: 2063 6f6d 6d61 6e64 732e 2902 da05 7479   commands.)...ty
-00000220: 7065 72da 0465 6368 6fa9 0072 0a00 0000  per..echo..r....
-00000230: 720a 0000 00fa 4e2f 5573 6572 732f 6e69  r.....N/Users/ni
-00000240: 636f 6c61 732f 4465 7665 6c6f 7065 722f  colas/Developer/
-00000250: 776f 726b 7370 6163 652f 556e 692f 4c32  workspace/Uni/L2
-00000260: 2f53 342f 5072 6f6a 6574 2f64 6f73 7369  /S4/Projet/dossi
-00000270: 6572 5356 4e2f 6666 7472 6163 6b2f 6d61  erSVN/fftrack/ma
-00000280: 696e 2e70 79da 046d 6169 6e19 0000 0073  in.py..main....s
-00000290: 0400 0000 0002 0a01 720c 0000 0063 0000  ........r....c..
-000002a0: 0000 0000 0000 0000 0000 0500 0000 0a00  ................
-000002b0: 0000 4300 0000 7366 0100 007a 3a74 00a0  ..C...sf...z:t..
-000002c0: 0164 0174 029b 0064 029d 03a1 0101 0074  .d.t...d.......t
-000002d0: 03a0 04a1 0001 0074 05a0 0674 02a1 0101  .......t...t....
-000002e0: 0074 03a0 07a1 0001 0074 00a0 0164 03a1  .t.......t...d..
-000002f0: 0101 0057 006e 3804 0074 086b 0a72 7201  ...W.n8..t.k.rr.
-00000300: 007d 0001 007a 1a74 00a0 0164 047c 009b  .}...z.t...d.|..
-00000310: 009d 02a1 0101 0057 0059 00a2 0464 0053  .......W.Y...d.S
-00000320: 0064 007d 007e 0058 0059 006e 0258 007a  .d.}.~.X.Y.n.X.z
-00000330: 3074 00a0 0164 05a1 0101 0074 09a0 0a74  0t...d.....t...t
-00000340: 036a 0ba1 017d 0174 00a0 0164 0674 0c7c  .j...}.t...d.t.|
-00000350: 0183 019b 0064 079d 03a1 0101 0057 006e  .....d.......W.n
-00000360: 3804 0074 086b 0a72 dc01 007d 0001 007a  8..t.k.r...}...z
-00000370: 1a74 00a0 0164 087c 009b 009d 02a1 0101  .t...d.|........
-00000380: 0057 0059 00a2 0464 0053 0064 007d 007e  .W.Y...d.S.d.}.~
-00000390: 0058 0059 006e 0258 007a 4874 00a0 0164  .X.Y.n.X.zHt...d
-000003a0: 09a1 0101 0074 0da0 0e7c 01a1 017d 027c  .....t...|...}.|
-000003b0: 0290 0172 1a7c 025c 027d 037d 0474 00a0  ...r.|.\.}.}.t..
-000003c0: 0164 0a7c 039b 0064 0b7c 049b 009d 04a1  .d.|...d.|......
-000003d0: 0101 006e 0a74 00a0 0164 0ca1 0101 0057  ...n.t...d.....W
-000003e0: 006e 3a04 0074 086b 0a90 0172 6001 007d  .n:..t.k...r`..}
-000003f0: 0001 007a 1a74 00a0 0164 0d7c 009b 009d  ...z.t...d.|....
-00000400: 02a1 0101 0057 0059 00a2 0464 0053 0064  .....W.Y...d.S.d
-00000410: 007d 007e 0058 0059 006e 0258 0064 0053  .}.~.X.Y.n.X.d.S
-00000420: 0029 0e4e 7a0e 4c69 7374 656e 696e 6720  .).Nz.Listening 
-00000430: 666f 7220 7a04 732e 2e2e 7a19 4175 6469  for z.s...z.Audi
-00000440: 6f20 7265 636f 7264 696e 6720 636f 6d70  o recording comp
-00000450: 6c65 7465 2e7a 1745 7272 6f72 2072 6563  lete.z.Error rec
-00000460: 6f72 6469 6e67 2061 7564 696f 3a20 fa13  ording audio: ..
-00000470: 5072 6f63 6573 7369 6e67 2061 7564 696f  Processing audio
-00000480: 2e2e 2efa 0a47 656e 6572 6174 6564 20fa  .....Generated .
-00000490: 1b20 6669 6e67 6572 7072 696e 7473 2073  . fingerprints s
-000004a0: 7563 6365 7373 6675 6c6c 792e fa18 4572  uccessfully...Er
-000004b0: 726f 7220 7072 6f63 6573 7369 6e67 2061  ror processing a
-000004c0: 7564 696f 3a20 fa11 4d61 7463 6869 6e67  udio: ..Matching
-000004d0: 2061 7564 696f 2e2e 2efa 1442 6573 7420   audio.....Best 
-000004e0: 6d61 7463 683a 2053 6f6e 6720 4944 20fa  match: Song ID .
-000004f0: 112c 204d 6174 6368 2064 6574 6169 6c73  ., Match details
-00000500: 3a20 fa0f 4e6f 206d 6174 6368 2066 6f75  : ..No match fou
-00000510: 6e64 2efa 1645 7272 6f72 206d 6174 6368  nd...Error match
-00000520: 696e 6720 6175 6469 6f3a 2029 0f72 0800  ing audio: ).r..
-00000530: 0000 7209 0000 00da 0b4c 4953 5445 4e5f  ..r......LISTEN_
-00000540: 5449 4d45 da0c 6175 6469 6f5f 7265 6164  TIME..audio_read
-00000550: 6572 da0f 7374 6172 745f 7265 636f 7264  er..start_record
-00000560: 696e 67da 0474 696d 65da 0573 6c65 6570  ing..time..sleep
-00000570: da0e 7374 6f70 5f72 6563 6f72 6469 6e67  ..stop_recording
-00000580: da09 4578 6365 7074 696f 6eda 0f61 7564  ..Exception..aud
-00000590: 696f 5f70 726f 6365 7373 6f72 da1f 6765  io_processor..ge
-000005a0: 6e65 7261 7465 5f66 696e 6765 7270 7269  nerate_fingerpri
-000005b0: 6e74 735f 6672 6f6d 5f66 696c 65da 0f6f  nts_from_file..o
-000005c0: 7574 7075 745f 6669 6c65 6e61 6d65 da03  utput_filename..
-000005d0: 6c65 6eda 076d 6174 6368 6572 da0e 6765  len..matcher..ge
-000005e0: 745f 6265 7374 5f6d 6174 6368 2905 da01  t_best_match)...
-000005f0: 65da 0c66 696e 6765 7270 7269 6e74 73da  e..fingerprints.
-00000600: 0a62 6573 745f 6d61 7463 68da 0773 6f6e  .best_match..son
-00000610: 675f 6964 da0d 6d61 7463 685f 6465 7461  g_id..match_deta
-00000620: 696c 7372 0a00 0000 720a 0000 0072 0b00  ilsr....r....r..
-00000630: 0000 da06 6c69 7374 656e 1f00 0000 7334  ....listen....s4
-00000640: 0000 0000 0302 0112 0108 010a 0108 010e  ................
-00000650: 0110 0110 0218 0302 010a 010c 011a 0110  ................
-00000660: 0110 0118 0202 020a 010a 0106 0108 0118  ................
-00000670: 020e 0112 0110 0172 2800 0000 2901 da09  .......r(...)...
-00000680: 6669 6c65 5f70 6174 6863 0100 0000 0000  file_pathc......
-00000690: 0000 0000 0000 0700 0000 0a00 0000 4300  ..............C.
-000006a0: 0000 735e 0100 007a 1874 00a0 0164 01a1  ..s^...z.t...d..
-000006b0: 0101 0074 02a0 037c 00a1 0101 0057 006e  ...t...|.....W.n
-000006c0: 3804 0074 046b 0a72 5001 007d 0101 007a  8..t.k.rP..}...z
-000006d0: 1a74 00a0 0164 027c 019b 009d 02a1 0101  .t...d.|........
-000006e0: 0057 0059 00a2 0464 0053 0064 007d 017e  .W.Y...d.S.d.}.~
-000006f0: 0158 0059 006e 0258 007a 3074 00a0 0164  .X.Y.n.X.z0t...d
-00000700: 03a1 0101 0074 05a0 0674 026a 07a1 017d  .....t...t.j...}
-00000710: 0274 00a0 0164 0474 087c 0283 019b 0064  .t...d.t.|.....d
-00000720: 059d 03a1 0101 0057 006e 3804 0074 046b  .......W.n8..t.k
-00000730: 0a72 ba01 007d 0101 007a 1a74 00a0 0164  .r...}...z.t...d
-00000740: 067c 019b 009d 02a1 0101 0057 0059 00a2  .|.........W.Y..
-00000750: 0464 0053 0064 007d 017e 0158 0059 006e  .d.S.d.}.~.X.Y.n
-00000760: 0258 007a 6274 00a0 0164 07a1 0101 0074  .X.zbt...d.....t
-00000770: 09a0 0a7c 02a1 017d 037c 0390 0172 127c  ...|...}.|...r.|
-00000780: 035c 027d 047d 0574 00a0 0164 087c 049b  .\.}.}.t...d.|..
-00000790: 0064 097c 059b 009d 04a1 0101 0074 0ba0  .d.|.........t..
-000007a0: 0c7c 04a1 017d 0674 00a0 0164 0a7c 069b  .|...}.t...d.|..
-000007b0: 009d 02a1 0101 006e 0a74 00a0 0164 0ba1  .......n.t...d..
-000007c0: 0101 0057 006e 3a04 0074 046b 0a90 0172  ...W.n:..t.k...r
-000007d0: 5801 007d 0101 007a 1a74 00a0 0164 0c7c  X..}...z.t...d.|
-000007e0: 019b 009d 02a1 0101 0057 0059 00a2 0464  .........W.Y...d
-000007f0: 0053 0064 007d 017e 0158 0059 006e 0258  .S.d.}.~.X.Y.n.X
-00000800: 0064 0053 0029 0d4e 7a15 4c6f 6164 696e  .d.S.).Nz.Loadin
-00000810: 6720 6175 6469 6f20 6669 6c65 2e2e 2e7a  g audio file...z
-00000820: 1a45 7272 6f72 206c 6f61 6469 6e67 2061  .Error loading a
-00000830: 7564 696f 2066 696c 653a 2072 0d00 0000  udio file: r....
-00000840: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000850: 1100 0000 7212 0000 0072 1300 0000 7a0e  ....r....r....z.
-00000860: 536f 6e67 2064 6574 6169 6c73 3a20 7214  Song details: r.
-00000870: 0000 0072 1500 0000 290d 7208 0000 0072  ...r....).r....r
-00000880: 0900 0000 7217 0000 00da 0c61 7564 696f  ....r......audio
-00000890: 5f74 6f5f 7761 7672 1c00 0000 721d 0000  _to_wavr....r...
-000008a0: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-000008b0: 7221 0000 0072 2200 0000 da02 6462 da0e  r!...r".....db..
-000008c0: 6765 745f 736f 6e67 5f62 795f 6964 2907  get_song_by_id).
-000008d0: 7229 0000 0072 2300 0000 7224 0000 0072  r)...r#...r$...r
-000008e0: 2500 0000 7226 0000 0072 2700 0000 da04  %...r&...r'.....
-000008f0: 736f 6e67 720a 0000 0072 0a00 0000 720b  songr....r....r.
-00000900: 0000 00da 0869 6465 6e74 6966 7944 0000  .....identifyD..
-00000910: 0073 3200 0000 0003 0201 0a01 0e01 1001  .s2.............
-00000920: 1001 1803 0201 0a01 0c01 1a01 1001 1001  ................
-00000930: 1802 0202 0a01 0a01 0601 0801 1602 0a01  ................
-00000940: 1202 0e01 1201 1001 722e 0000 0063 0000  ........r....c..
-00000950: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000960: 0000 4300 0000 7318 0000 0074 00a0 0164  ..C...s....t...d
-00000970: 01a1 0101 0074 00a0 0174 02a1 0101 0064  .....t...t.....d
-00000980: 0053 0029 024e 7a16 4375 7272 656e 7420  .S.).Nz.Current 
-00000990: 636f 6e66 6967 7572 6174 696f 6e3a a903  configuration:..
-000009a0: 7208 0000 0072 0900 0000 7202 0000 0072  r....r....r....r
-000009b0: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
-000009c0: 0000 00da 0a67 6574 5f63 6f6e 6669 6768  .....get_configh
-000009d0: 0000 0073 0400 0000 0002 0a01 7230 0000  ...s........r0..
-000009e0: 00a9 01da 0773 6574 7469 6e67 6301 0000  .....settingc...
-000009f0: 0000 0000 0000 0000 0001 0000 0007 0000  ................
-00000a00: 0043 0000 0073 1e00 0000 7400 a001 6401  .C...s....t...d.
-00000a10: 7c00 9b00 6402 7402 7c00 1900 9b00 9d04  |...d.t.|.......
-00000a20: a101 0100 6400 5300 2903 4e7a 1143 7572  ....d.S.).Nz.Cur
-00000a30: 7265 6e74 2076 616c 7565 206f 6620 7a02  rent value of z.
-00000a40: 3a20 722f 0000 0072 3100 0000 720a 0000  : r/...r1...r...
-00000a50: 0072 0a00 0000 720b 0000 00da 0b67 6574  .r....r......get
-00000a60: 5f73 6574 7469 6e67 6e00 0000 7302 0000  _settingn...s...
-00000a70: 0000 0272 3300 0000 da08 5f5f 6d61 696e  ...r3.....__main
-00000a80: 5f5f 2920 7208 0000 00da 026f 73da 046a  __) r......os..j
-00000a90: 736f 6e72 1900 0000 da07 6666 7472 6163  sonr......fftrac
-00000aa0: 6b72 0200 0000 da02 6366 5a1b 6666 7472  kr......cfZ.fftr
-00000ab0: 6163 6b2e 6461 7461 6261 7365 2e64 625f  ack.database.db_
-00000ac0: 6d61 6e61 6765 7272 0300 0000 5a1d 6666  managerr....Z.ff
-00000ad0: 7472 6163 6b2e 6175 6469 6f2e 4175 6469  track.audio.Audi
-00000ae0: 6f50 726f 6365 7373 696e 6772 0400 0000  oProcessingr....
-00000af0: 5a1a 6666 7472 6163 6b2e 6175 6469 6f2e  Z.fftrack.audio.
-00000b00: 6175 6469 6f5f 7265 6164 6572 7205 0000  audio_readerr...
-00000b10: 005a 1866 6674 7261 636b 2e6d 6174 6368  .Z.fftrack.match
-00000b20: 696e 672e 6d61 7463 6865 7272 0600 0000  ing.matcherr....
-00000b30: 5a05 5479 7065 72da 0361 7070 7217 0000  Z.Typer..appr...
-00000b40: 0072 1d00 0000 722b 0000 0072 2100 0000  .r....r+...r!...
-00000b50: da0b 6c6f 6164 5f63 6f6e 6669 67da 0369  ..load_config..i
-00000b60: 6e74 7216 0000 00da 0763 6f6d 6d61 6e64  ntr......command
-00000b70: 720c 0000 0072 2800 0000 da03 7374 7272  r....r(.....strr
-00000b80: 2e00 0000 7230 0000 0072 3300 0000 da08  ....r0...r3.....
-00000b90: 5f5f 6e61 6d65 5f5f 720a 0000 0072 0a00  __name__r....r..
-00000ba0: 0000 720a 0000 0072 0b00 0000 da08 3c6d  ..r....r......<m
-00000bb0: 6f64 756c 653e 0100 0000 7336 0000 0008  odule>....s6....
-00000bc0: 0108 0108 0108 020c 020c 010c 010c 010c  ................
-00000bd0: 0208 0106 010a 0106 0108 0308 010c 0406  ................
-00000be0: 010a 0506 010a 2406 0110 2306 010a 0506  ......$...#.....
-00000bf0: 0110 040a 01                             .....
+00000020: 0004 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6400 6401 6c09 5a09 6500  m.Z...d.d.l.Z.e.
+00000070: a00a a100 5a0b 6506 8300 5a0c 6504 6406  ....Z.e...Z.e.d.
+00000080: 6407 8d01 5a0d 6502 8300 5a0e 6508 650e  d...Z.e...Z.e.e.
+00000090: 8301 5a0f 6408 5a10 650b a011 a100 6409  ..Z.d.Z.e.....d.
+000000a0: 640a 8400 8301 5a12 650b a011 a100 6513  d.....Z.e.....e.
+000000b0: 640b 9c01 640c 640d 8404 8301 5a14 6515  d...d.d.....Z.e.
+000000c0: 640e 6b02 729e 650b 8300 0100 6401 5300  d.k.r.e.....d.S.
+000000d0: 290f e900 0000 004e 2901 da0f 4461 7461  )......N)...Data
+000000e0: 6261 7365 4d61 6e61 6765 7229 01da 0f41  baseManager)...A
+000000f0: 7564 696f 5072 6f63 6573 7369 6e67 2901  udioProcessing).
+00000100: da0b 4175 6469 6f52 6561 6465 7229 01da  ..AudioReader)..
+00000110: 074d 6174 6368 6572 4629 01da 0470 6c6f  .MatcherF)...plo
+00000120: 74e9 0500 0000 6300 0000 0000 0000 0000  t.....c.........
+00000130: 0000 0005 0000 000a 0000 0043 0000 0073  ...........C...s
+00000140: 6601 0000 7a3a 7400 a001 6401 7402 9b00  f...z:t...d.t...
+00000150: 6402 9d03 a101 0100 7403 a004 a100 0100  d.......t.......
+00000160: 7405 a006 7402 a101 0100 7403 a007 a100  t...t.....t.....
+00000170: 0100 7400 a001 6403 a101 0100 5700 6e38  ..t...d.....W.n8
+00000180: 0400 7408 6b0a 7272 0100 7d00 0100 7a1a  ..t.k.rr..}...z.
+00000190: 7400 a001 6404 7c00 9b00 9d02 a101 0100  t...d.|.........
+000001a0: 5700 5900 a204 6400 5300 6400 7d00 7e00  W.Y...d.S.d.}.~.
+000001b0: 5800 5900 6e02 5800 7a30 7400 a001 6405  X.Y.n.X.z0t...d.
+000001c0: a101 0100 7409 a00a 7403 6a0b a101 7d01  ....t...t.j...}.
+000001d0: 7400 a001 6406 740c 7c01 8301 9b00 6407  t...d.t.|.....d.
+000001e0: 9d03 a101 0100 5700 6e38 0400 7408 6b0a  ......W.n8..t.k.
+000001f0: 72dc 0100 7d00 0100 7a1a 7400 a001 6408  r...}...z.t...d.
+00000200: 7c00 9b00 9d02 a101 0100 5700 5900 a204  |.........W.Y...
+00000210: 6400 5300 6400 7d00 7e00 5800 5900 6e02  d.S.d.}.~.X.Y.n.
+00000220: 5800 7a48 7400 a001 6409 a101 0100 740d  X.zHt...d.....t.
+00000230: a00e 7c01 a101 7d02 7c02 9001 721a 7c02  ..|...}.|...r.|.
+00000240: 5c02 7d03 7d04 7400 a001 640a 7c03 9b00  \.}.}.t...d.|...
+00000250: 640b 7c04 9b00 9d04 a101 0100 6e0a 7400  d.|.........n.t.
+00000260: a001 640c a101 0100 5700 6e3a 0400 7408  ..d.....W.n:..t.
+00000270: 6b0a 9001 7260 0100 7d00 0100 7a1a 7400  k...r`..}...z.t.
+00000280: a001 640d 7c00 9b00 9d02 a101 0100 5700  ..d.|.........W.
+00000290: 5900 a204 6400 5300 6400 7d00 7e00 5800  Y...d.S.d.}.~.X.
+000002a0: 5900 6e02 5800 6400 5300 290e 4e7a 0e4c  Y.n.X.d.S.).Nz.L
+000002b0: 6973 7465 6e69 6e67 2066 6f72 207a 0473  istening for z.s
+000002c0: 2e2e 2e7a 1941 7564 696f 2072 6563 6f72  ...z.Audio recor
+000002d0: 6469 6e67 2063 6f6d 706c 6574 652e 7a17  ding complete.z.
+000002e0: 4572 726f 7220 7265 636f 7264 696e 6720  Error recording 
+000002f0: 6175 6469 6f3a 20fa 1350 726f 6365 7373  audio: ..Process
+00000300: 696e 6720 6175 6469 6f2e 2e2e fa0a 4765  ing audio.....Ge
+00000310: 6e65 7261 7465 6420 fa1b 2066 696e 6765  nerated .. finge
+00000320: 7270 7269 6e74 7320 7375 6363 6573 7366  rprints successf
+00000330: 756c 6c79 2efa 1845 7272 6f72 2070 726f  ully...Error pro
+00000340: 6365 7373 696e 6720 6175 6469 6f3a 20fa  cessing audio: .
+00000350: 114d 6174 6368 696e 6720 6175 6469 6f2e  .Matching audio.
+00000360: 2e2e fa14 4265 7374 206d 6174 6368 3a20  ....Best match: 
+00000370: 536f 6e67 2049 4420 fa11 2c20 4d61 7463  Song ID .., Matc
+00000380: 6820 6465 7461 696c 733a 20fa 0f4e 6f20  h details: ..No 
+00000390: 6d61 7463 6820 666f 756e 642e fa16 4572  match found...Er
+000003a0: 726f 7220 6d61 7463 6869 6e67 2061 7564  ror matching aud
+000003b0: 696f 3a20 290f da05 7479 7065 72da 0465  io: )...typer..e
+000003c0: 6368 6fda 0b4c 4953 5445 4e5f 5449 4d45  cho..LISTEN_TIME
+000003d0: da0c 6175 6469 6f5f 7265 6164 6572 da0f  ..audio_reader..
+000003e0: 7374 6172 745f 7265 636f 7264 696e 67da  start_recording.
+000003f0: 0474 696d 65da 0573 6c65 6570 da0e 7374  .time..sleep..st
+00000400: 6f70 5f72 6563 6f72 6469 6e67 da09 4578  op_recording..Ex
+00000410: 6365 7074 696f 6eda 0f61 7564 696f 5f70  ception..audio_p
+00000420: 726f 6365 7373 6f72 da1f 6765 6e65 7261  rocessor..genera
+00000430: 7465 5f66 696e 6765 7270 7269 6e74 735f  te_fingerprints_
+00000440: 6672 6f6d 5f66 696c 65da 0f6f 7574 7075  from_file..outpu
+00000450: 745f 6669 6c65 6e61 6d65 da03 6c65 6eda  t_filename..len.
+00000460: 076d 6174 6368 6572 da0e 6765 745f 6265  .matcher..get_be
+00000470: 7374 5f6d 6174 6368 2905 da01 65da 0c66  st_match)...e..f
+00000480: 696e 6765 7270 7269 6e74 73da 0a62 6573  ingerprints..bes
+00000490: 745f 6d61 7463 68da 0773 6f6e 675f 6964  t_match..song_id
+000004a0: da0d 6d61 7463 685f 6465 7461 696c 73a9  ..match_details.
+000004b0: 0072 2500 0000 fa5d 2f55 7365 7273 2f6e  .r%....]/Users/n
+000004c0: 6963 6f6c 6173 2f44 6576 656c 6f70 6572  icolas/Developer
+000004d0: 2f77 6f72 6b73 7061 6365 2f55 6e69 2f4c  /workspace/Uni/L
+000004e0: 322f 5334 2f50 726f 6a65 742f 646f 7373  2/S4/Projet/doss
+000004f0: 6965 7253 564e 2f66 6674 7261 636b 2f75  ierSVN/fftrack/u
+00000500: 692f 6d61 696e 5f63 6c69 5f6e 6963 6f6c  i/main_cli_nicol
+00000510: 6173 2e70 79da 066c 6973 7465 6e10 0000  as.py..listen...
+00000520: 0073 3400 0000 0003 0201 1201 0801 0a01  .s4.............
+00000530: 0801 0e01 1001 1001 1803 0201 0a01 0c01  ................
+00000540: 1a01 1001 1001 1802 0202 0a01 0a01 0601  ................
+00000550: 0801 1802 0e01 1201 1001 7227 0000 0029  ..........r'...)
+00000560: 01da 0966 696c 655f 7061 7468 6301 0000  ...file_pathc...
+00000570: 0000 0000 0000 0000 0006 0000 000a 0000  ................
+00000580: 0043 0000 0073 4201 0000 7a18 7400 a001  .C...sB...z.t...
+00000590: 6401 a101 0100 7402 a003 7c00 a101 0100  d.....t...|.....
+000005a0: 5700 6e38 0400 7404 6b0a 7250 0100 7d01  W.n8..t.k.rP..}.
+000005b0: 0100 7a1a 7400 a001 6402 7c01 9b00 9d02  ..z.t...d.|.....
+000005c0: a101 0100 5700 5900 a204 6400 5300 6400  ....W.Y...d.S.d.
+000005d0: 7d01 7e01 5800 5900 6e02 5800 7a30 7400  }.~.X.Y.n.X.z0t.
+000005e0: a001 6403 a101 0100 7405 a006 7402 6a07  ..d.....t...t.j.
+000005f0: a101 7d02 7400 a001 6404 7408 7c02 8301  ..}.t...d.t.|...
+00000600: 9b00 6405 9d03 a101 0100 5700 6e38 0400  ..d.......W.n8..
+00000610: 7404 6b0a 72ba 0100 7d01 0100 7a1a 7400  t.k.r...}...z.t.
+00000620: a001 6406 7c01 9b00 9d02 a101 0100 5700  ..d.|.........W.
+00000630: 5900 a204 6400 5300 6400 7d01 7e01 5800  Y...d.S.d.}.~.X.
+00000640: 5900 6e02 5800 7a46 7400 a001 6407 a101  Y.n.X.zFt...d...
+00000650: 0100 7409 a00a 7c02 a101 7d03 7c03 72f6  ..t...|...}.|.r.
+00000660: 7c03 5c02 7d04 7d05 7400 a001 6408 7c04  |.\.}.}.t...d.|.
+00000670: 9b00 6409 7c05 9b00 9d04 a101 0100 6e0a  ..d.|.........n.
+00000680: 7400 a001 640a a101 0100 5700 6e3a 0400  t...d.....W.n:..
+00000690: 7404 6b0a 9001 723c 0100 7d01 0100 7a1a  t.k...r<..}...z.
+000006a0: 7400 a001 640b 7c01 9b00 9d02 a101 0100  t...d.|.........
+000006b0: 5700 5900 a204 6400 5300 6400 7d01 7e01  W.Y...d.S.d.}.~.
+000006c0: 5800 5900 6e02 5800 6400 5300 290c 4e7a  X.Y.n.X.d.S.).Nz
+000006d0: 154c 6f61 6469 6e67 2061 7564 696f 2066  .Loading audio f
+000006e0: 696c 652e 2e2e 7a1a 4572 726f 7220 6c6f  ile...z.Error lo
+000006f0: 6164 696e 6720 6175 6469 6f20 6669 6c65  ading audio file
+00000700: 3a20 7208 0000 0072 0900 0000 720a 0000  : r....r....r...
+00000710: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000720: 720e 0000 0072 0f00 0000 7210 0000 0029  r....r....r....)
+00000730: 0b72 1100 0000 7212 0000 0072 1400 0000  .r....r....r....
+00000740: da0c 6175 6469 6f5f 746f 5f77 6176 7219  ..audio_to_wavr.
+00000750: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000760: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000770: 0029 0672 2800 0000 7220 0000 0072 2100  .).r(...r ...r!.
+00000780: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
+00000790: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+000007a0: da0a 6d61 7463 685f 6669 6c65 3300 0000  ..match_file3...
+000007b0: 732e 0000 0000 0302 010a 010e 0110 0110  s...............
+000007c0: 0118 0302 010a 010c 011a 0110 0110 0118  ................
+000007d0: 0202 020a 010a 0104 0108 0118 020e 0112  ................
+000007e0: 0110 0172 2a00 0000 da08 5f5f 6d61 696e  ...r*.....__main
+000007f0: 5f5f 2916 7211 0000 005a 1b66 6674 7261  __).r....Z.fftra
+00000800: 636b 2e64 6174 6162 6173 652e 6462 5f6d  ck.database.db_m
+00000810: 616e 6167 6572 7202 0000 005a 1d66 6674  anagerr....Z.fft
+00000820: 7261 636b 2e61 7564 696f 2e41 7564 696f  rack.audio.Audio
+00000830: 5072 6f63 6573 7369 6e67 7203 0000 005a  Processingr....Z
+00000840: 1a66 6674 7261 636b 2e61 7564 696f 2e61  .fftrack.audio.a
+00000850: 7564 696f 5f72 6561 6465 7272 0400 0000  udio_readerr....
+00000860: 5a18 6666 7472 6163 6b2e 6d61 7463 6869  Z.fftrack.matchi
+00000870: 6e67 2e6d 6174 6368 6572 7205 0000 0072  ng.matcherr....r
+00000880: 1600 0000 5a05 5479 7065 72da 0361 7070  ....Z.Typer..app
+00000890: 7214 0000 0072 1a00 0000 da02 6462 721e  r....r......dbr.
+000008a0: 0000 0072 1300 0000 da07 636f 6d6d 616e  ...r......comman
+000008b0: 6472 2700 0000 da03 7374 7272 2a00 0000  dr'.....strr*...
+000008c0: da08 5f5f 6e61 6d65 5f5f 7225 0000 0072  ..__name__r%...r
+000008d0: 2500 0000 7225 0000 0072 2600 0000 da08  %...r%...r&.....
+000008e0: 3c6d 6f64 756c 653e 0100 0000 7322 0000  <module>....s"..
+000008f0: 0008 020c 010c 010c 010c 0108 0208 0106  ................
+00000900: 010a 0106 0108 0104 0206 010a 2206 0110  ............"...
+00000910: 1f08 01                                  ...
```

### Comparing `fftrack-0.1.0/fftrack/__pycache__/main.cpython-39.pyc` & `fftrack-0.1.1/fftrack/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/audio/AudioProcessing.py` & `fftrack-0.1.1/fftrack/audio/AudioProcessing.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/audio/__pycache__/AudioProcessing.cpython-38.pyc` & `fftrack-0.1.1/fftrack/audio/__pycache__/AudioProcessing.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/audio/__pycache__/AudioProcessing.cpython-39.pyc` & `fftrack-0.1.1/fftrack/audio/__pycache__/AudioProcessing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/audio/__pycache__/audio_compare.cpython-38.pyc` & `fftrack-0.1.1/fftrack/audio/__pycache__/audio_compare.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/audio/__pycache__/audio_reader.cpython-38.pyc` & `fftrack-0.1.1/fftrack/audio/__pycache__/audio_reader.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr 11 11:55:51 2024 UTC, .py size: 3700 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c7cf 1766 740e 0000  U..........ft...
+00000000: 550d 0d0a 0000 0000 91c8 2f66 740e 0000  U........./ft...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 4700 6403 6404 8400 6404 8302 5a05  ..G.d.d...d...Z.
 00000060: 6401 5300 2905 e900 0000 004e 2901 da06  d.S.)......N)...
 00000070: 5468 7265 6164 6300 0000 0000 0000 0000  Threadc.........
```

### Comparing `fftrack-0.1.0/fftrack/audio/__pycache__/audio_reader.cpython-39.pyc` & `fftrack-0.1.1/fftrack/audio/__pycache__/audio_reader.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/audio/audio_compare.py` & `fftrack-0.1.1/fftrack/audio/audio_compare.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/audio/audio_reader.py` & `fftrack-0.1.1/fftrack/audio/audio_reader.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/audio/main_audio.py` & `fftrack-0.1.1/fftrack/audio/main_audio.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/config.py` & `fftrack-0.1.1/fftrack/config.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/database/__pycache__/db_manager.cpython-38.pyc` & `fftrack-0.1.1/fftrack/database/__pycache__/db_manager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/database/__pycache__/db_manager.cpython-39.pyc` & `fftrack-0.1.1/fftrack/database/__pycache__/db_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/database/__pycache__/models.cpython-38.pyc` & `fftrack-0.1.1/fftrack/database/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/database/__pycache__/models.cpython-39.pyc` & `fftrack-0.1.1/fftrack/database/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/database/db_manager.py` & `fftrack-0.1.1/fftrack/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/database/main_db.py` & `fftrack-0.1.1/fftrack/database/main_db.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/database/models.py` & `fftrack-0.1.1/fftrack/database/models.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/main.py` & `fftrack-0.1.1/fftrack/main.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/matching/__pycache__/main_matching.cpython-38.pyc` & `fftrack-0.1.1/fftrack/matching/__pycache__/main_matching.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/matching/__pycache__/matcher.cpython-38.pyc` & `fftrack-0.1.1/fftrack/matching/__pycache__/matcher.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr 18 09:05:35 2024 UTC, .py size: 7345 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5fe2 2066 b11c 0000  U......._. f....
+00000000: 550d 0d0a 0000 0000 91c8 2f66 b11c 0000  U........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 6d05 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6403 5a07 6404 5a08 6405 5a09 6406  ..d.Z.d.Z.d.Z.d.
 00000060: 5a0a 6406 5a0b 6405 5a0c 4700 6407 6408  Z.d.Z.d.Z.G.d.d.
 00000070: 8400 6408 8302 5a0d 6401 5300 2909 e900  ..d...Z.d.S.)...
```

### Comparing `fftrack-0.1.0/fftrack/matching/__pycache__/matcher.cpython-39.pyc` & `fftrack-0.1.1/fftrack/matching/__pycache__/matcher.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/matching/main_matching.py` & `fftrack-0.1.1/fftrack/matching/main_matching.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/matching/matcher.py` & `fftrack-0.1.1/fftrack/matching/matcher.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/scripts/__pycache__/populate_database.cpython-39.pyc` & `fftrack-0.1.1/fftrack/scripts/__pycache__/populate_database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/scripts/populate_database.py` & `fftrack-0.1.1/fftrack/scripts/populate_database.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/ui/__pycache__/main_cli_nicolas.cpython-38.pyc` & `fftrack-0.1.1/fftrack/__pycache__/main.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr 18 08:37:30 2024 UTC, .py size: 2722 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,146 +1,189 @@
-00000000: 550d 0d0a 0000 0000 cadb 2066 a20a 0000  U......... f....
+00000000: 550d 0d0a 0000 0000 9262 3366 cb0c 0000  U........b3f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6400 6401 6c09 5a09 6500  m.Z...d.d.l.Z.e.
-00000070: a00a a100 5a0b 6506 8300 5a0c 6504 6406  ....Z.e...Z.e.d.
-00000080: 6407 8d01 5a0d 6502 8300 5a0e 6508 650e  d...Z.e...Z.e.e.
-00000090: 8301 5a0f 6408 5a10 650b a011 a100 6409  ..Z.d.Z.e.....d.
-000000a0: 640a 8400 8301 5a12 650b a011 a100 6513  d.....Z.e.....e.
-000000b0: 640b 9c01 640c 640d 8404 8301 5a14 6515  d...d.d.....Z.e.
-000000c0: 640e 6b02 729e 650b 8300 0100 6401 5300  d.k.r.e.....d.S.
-000000d0: 290f e900 0000 004e 2901 da0f 4461 7461  )......N)...Data
-000000e0: 6261 7365 4d61 6e61 6765 7229 01da 0f41  baseManager)...A
-000000f0: 7564 696f 5072 6f63 6573 7369 6e67 2901  udioProcessing).
-00000100: da0b 4175 6469 6f52 6561 6465 7229 01da  ..AudioReader)..
-00000110: 074d 6174 6368 6572 4629 01da 0470 6c6f  .MatcherF)...plo
-00000120: 74e9 0500 0000 6300 0000 0000 0000 0000  t.....c.........
-00000130: 0000 0005 0000 000a 0000 0043 0000 0073  ...........C...s
-00000140: 6601 0000 7a3a 7400 a001 6401 7402 9b00  f...z:t...d.t...
-00000150: 6402 9d03 a101 0100 7403 a004 a100 0100  d.......t.......
-00000160: 7405 a006 7402 a101 0100 7403 a007 a100  t...t.....t.....
-00000170: 0100 7400 a001 6403 a101 0100 5700 6e38  ..t...d.....W.n8
-00000180: 0400 7408 6b0a 7272 0100 7d00 0100 7a1a  ..t.k.rr..}...z.
-00000190: 7400 a001 6404 7c00 9b00 9d02 a101 0100  t...d.|.........
-000001a0: 5700 5900 a204 6400 5300 6400 7d00 7e00  W.Y...d.S.d.}.~.
-000001b0: 5800 5900 6e02 5800 7a30 7400 a001 6405  X.Y.n.X.z0t...d.
-000001c0: a101 0100 7409 a00a 7403 6a0b a101 7d01  ....t...t.j...}.
-000001d0: 7400 a001 6406 740c 7c01 8301 9b00 6407  t...d.t.|.....d.
-000001e0: 9d03 a101 0100 5700 6e38 0400 7408 6b0a  ......W.n8..t.k.
-000001f0: 72dc 0100 7d00 0100 7a1a 7400 a001 6408  r...}...z.t...d.
-00000200: 7c00 9b00 9d02 a101 0100 5700 5900 a204  |.........W.Y...
-00000210: 6400 5300 6400 7d00 7e00 5800 5900 6e02  d.S.d.}.~.X.Y.n.
-00000220: 5800 7a48 7400 a001 6409 a101 0100 740d  X.zHt...d.....t.
-00000230: a00e 7c01 a101 7d02 7c02 9001 721a 7c02  ..|...}.|...r.|.
-00000240: 5c02 7d03 7d04 7400 a001 640a 7c03 9b00  \.}.}.t...d.|...
-00000250: 640b 7c04 9b00 9d04 a101 0100 6e0a 7400  d.|.........n.t.
-00000260: a001 640c a101 0100 5700 6e3a 0400 7408  ..d.....W.n:..t.
-00000270: 6b0a 9001 7260 0100 7d00 0100 7a1a 7400  k...r`..}...z.t.
-00000280: a001 640d 7c00 9b00 9d02 a101 0100 5700  ..d.|.........W.
-00000290: 5900 a204 6400 5300 6400 7d00 7e00 5800  Y...d.S.d.}.~.X.
-000002a0: 5900 6e02 5800 6400 5300 290e 4e7a 0e4c  Y.n.X.d.S.).Nz.L
-000002b0: 6973 7465 6e69 6e67 2066 6f72 207a 0473  istening for z.s
-000002c0: 2e2e 2e7a 1941 7564 696f 2072 6563 6f72  ...z.Audio recor
-000002d0: 6469 6e67 2063 6f6d 706c 6574 652e 7a17  ding complete.z.
-000002e0: 4572 726f 7220 7265 636f 7264 696e 6720  Error recording 
-000002f0: 6175 6469 6f3a 20fa 1350 726f 6365 7373  audio: ..Process
-00000300: 696e 6720 6175 6469 6f2e 2e2e fa0a 4765  ing audio.....Ge
-00000310: 6e65 7261 7465 6420 fa1b 2066 696e 6765  nerated .. finge
-00000320: 7270 7269 6e74 7320 7375 6363 6573 7366  rprints successf
-00000330: 756c 6c79 2efa 1845 7272 6f72 2070 726f  ully...Error pro
-00000340: 6365 7373 696e 6720 6175 6469 6f3a 20fa  cessing audio: .
-00000350: 114d 6174 6368 696e 6720 6175 6469 6f2e  .Matching audio.
-00000360: 2e2e fa14 4265 7374 206d 6174 6368 3a20  ....Best match: 
-00000370: 536f 6e67 2049 4420 fa11 2c20 4d61 7463  Song ID .., Matc
-00000380: 6820 6465 7461 696c 733a 20fa 0f4e 6f20  h details: ..No 
-00000390: 6d61 7463 6820 666f 756e 642e fa16 4572  match found...Er
-000003a0: 726f 7220 6d61 7463 6869 6e67 2061 7564  ror matching aud
-000003b0: 696f 3a20 290f da05 7479 7065 72da 0465  io: )...typer..e
-000003c0: 6368 6fda 0b4c 4953 5445 4e5f 5449 4d45  cho..LISTEN_TIME
-000003d0: da0c 6175 6469 6f5f 7265 6164 6572 da0f  ..audio_reader..
-000003e0: 7374 6172 745f 7265 636f 7264 696e 67da  start_recording.
-000003f0: 0474 696d 65da 0573 6c65 6570 da0e 7374  .time..sleep..st
-00000400: 6f70 5f72 6563 6f72 6469 6e67 da09 4578  op_recording..Ex
-00000410: 6365 7074 696f 6eda 0f61 7564 696f 5f70  ception..audio_p
-00000420: 726f 6365 7373 6f72 da1f 6765 6e65 7261  rocessor..genera
-00000430: 7465 5f66 696e 6765 7270 7269 6e74 735f  te_fingerprints_
-00000440: 6672 6f6d 5f66 696c 65da 0f6f 7574 7075  from_file..outpu
-00000450: 745f 6669 6c65 6e61 6d65 da03 6c65 6eda  t_filename..len.
-00000460: 076d 6174 6368 6572 da0e 6765 745f 6265  .matcher..get_be
-00000470: 7374 5f6d 6174 6368 2905 da01 65da 0c66  st_match)...e..f
-00000480: 696e 6765 7270 7269 6e74 73da 0a62 6573  ingerprints..bes
-00000490: 745f 6d61 7463 68da 0773 6f6e 675f 6964  t_match..song_id
-000004a0: da0d 6d61 7463 685f 6465 7461 696c 73a9  ..match_details.
-000004b0: 0072 2500 0000 fa5d 2f55 7365 7273 2f6e  .r%....]/Users/n
-000004c0: 6963 6f6c 6173 2f44 6576 656c 6f70 6572  icolas/Developer
-000004d0: 2f77 6f72 6b73 7061 6365 2f55 6e69 2f4c  /workspace/Uni/L
-000004e0: 322f 5334 2f50 726f 6a65 742f 646f 7373  2/S4/Projet/doss
-000004f0: 6965 7253 564e 2f66 6674 7261 636b 2f75  ierSVN/fftrack/u
-00000500: 692f 6d61 696e 5f63 6c69 5f6e 6963 6f6c  i/main_cli_nicol
-00000510: 6173 2e70 79da 066c 6973 7465 6e10 0000  as.py..listen...
-00000520: 0073 3400 0000 0003 0201 1201 0801 0a01  .s4.............
-00000530: 0801 0e01 1001 1001 1803 0201 0a01 0c01  ................
-00000540: 1a01 1001 1001 1802 0202 0a01 0a01 0601  ................
-00000550: 0801 1802 0e01 1201 1001 7227 0000 0029  ..........r'...)
-00000560: 01da 0966 696c 655f 7061 7468 6301 0000  ...file_pathc...
-00000570: 0000 0000 0000 0000 0006 0000 000a 0000  ................
-00000580: 0043 0000 0073 4201 0000 7a18 7400 a001  .C...sB...z.t...
-00000590: 6401 a101 0100 7402 a003 7c00 a101 0100  d.....t...|.....
-000005a0: 5700 6e38 0400 7404 6b0a 7250 0100 7d01  W.n8..t.k.rP..}.
-000005b0: 0100 7a1a 7400 a001 6402 7c01 9b00 9d02  ..z.t...d.|.....
-000005c0: a101 0100 5700 5900 a204 6400 5300 6400  ....W.Y...d.S.d.
-000005d0: 7d01 7e01 5800 5900 6e02 5800 7a30 7400  }.~.X.Y.n.X.z0t.
-000005e0: a001 6403 a101 0100 7405 a006 7402 6a07  ..d.....t...t.j.
-000005f0: a101 7d02 7400 a001 6404 7408 7c02 8301  ..}.t...d.t.|...
-00000600: 9b00 6405 9d03 a101 0100 5700 6e38 0400  ..d.......W.n8..
-00000610: 7404 6b0a 72ba 0100 7d01 0100 7a1a 7400  t.k.r...}...z.t.
-00000620: a001 6406 7c01 9b00 9d02 a101 0100 5700  ..d.|.........W.
-00000630: 5900 a204 6400 5300 6400 7d01 7e01 5800  Y...d.S.d.}.~.X.
-00000640: 5900 6e02 5800 7a46 7400 a001 6407 a101  Y.n.X.zFt...d...
-00000650: 0100 7409 a00a 7c02 a101 7d03 7c03 72f6  ..t...|...}.|.r.
-00000660: 7c03 5c02 7d04 7d05 7400 a001 6408 7c04  |.\.}.}.t...d.|.
-00000670: 9b00 6409 7c05 9b00 9d04 a101 0100 6e0a  ..d.|.........n.
-00000680: 7400 a001 640a a101 0100 5700 6e3a 0400  t...d.....W.n:..
-00000690: 7404 6b0a 9001 723c 0100 7d01 0100 7a1a  t.k...r<..}...z.
-000006a0: 7400 a001 640b 7c01 9b00 9d02 a101 0100  t...d.|.........
-000006b0: 5700 5900 a204 6400 5300 6400 7d01 7e01  W.Y...d.S.d.}.~.
-000006c0: 5800 5900 6e02 5800 6400 5300 290c 4e7a  X.Y.n.X.d.S.).Nz
-000006d0: 154c 6f61 6469 6e67 2061 7564 696f 2066  .Loading audio f
-000006e0: 696c 652e 2e2e 7a1a 4572 726f 7220 6c6f  ile...z.Error lo
-000006f0: 6164 696e 6720 6175 6469 6f20 6669 6c65  ading audio file
-00000700: 3a20 7208 0000 0072 0900 0000 720a 0000  : r....r....r...
-00000710: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000720: 720e 0000 0072 0f00 0000 7210 0000 0029  r....r....r....)
-00000730: 0b72 1100 0000 7212 0000 0072 1400 0000  .r....r....r....
-00000740: da0c 6175 6469 6f5f 746f 5f77 6176 7219  ..audio_to_wavr.
-00000750: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000760: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00000770: 0029 0672 2800 0000 7220 0000 0072 2100  .).r(...r ...r!.
-00000780: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
-00000790: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-000007a0: da0a 6d61 7463 685f 6669 6c65 3300 0000  ..match_file3...
-000007b0: 732e 0000 0000 0302 010a 010e 0110 0110  s...............
-000007c0: 0118 0302 010a 010c 011a 0110 0110 0118  ................
-000007d0: 0202 020a 010a 0104 0108 0118 020e 0112  ................
-000007e0: 0110 0172 2a00 0000 da08 5f5f 6d61 696e  ...r*.....__main
-000007f0: 5f5f 2916 7211 0000 005a 1b66 6674 7261  __).r....Z.fftra
-00000800: 636b 2e64 6174 6162 6173 652e 6462 5f6d  ck.database.db_m
-00000810: 616e 6167 6572 7202 0000 005a 1d66 6674  anagerr....Z.fft
-00000820: 7261 636b 2e61 7564 696f 2e41 7564 696f  rack.audio.Audio
-00000830: 5072 6f63 6573 7369 6e67 7203 0000 005a  Processingr....Z
-00000840: 1a66 6674 7261 636b 2e61 7564 696f 2e61  .fftrack.audio.a
-00000850: 7564 696f 5f72 6561 6465 7272 0400 0000  udio_readerr....
-00000860: 5a18 6666 7472 6163 6b2e 6d61 7463 6869  Z.fftrack.matchi
-00000870: 6e67 2e6d 6174 6368 6572 7205 0000 0072  ng.matcherr....r
-00000880: 1600 0000 5a05 5479 7065 72da 0361 7070  ....Z.Typer..app
-00000890: 7214 0000 0072 1a00 0000 da02 6462 721e  r....r......dbr.
-000008a0: 0000 0072 1300 0000 da07 636f 6d6d 616e  ...r......comman
-000008b0: 6472 2700 0000 da03 7374 7272 2a00 0000  dr'.....strr*...
-000008c0: da08 5f5f 6e61 6d65 5f5f 7225 0000 0072  ..__name__r%...r
-000008d0: 2500 0000 7225 0000 0072 2600 0000 da08  %...r%...r&.....
-000008e0: 3c6d 6f64 756c 653e 0100 0000 7322 0000  <module>....s"..
-000008f0: 0008 020c 010c 010c 010c 0108 0208 0106  ................
-00000900: 010a 0106 0108 0104 0206 010a 2206 0110  ............"...
-00000910: 1f08 01                                  ...
+00000020: 0004 0000 0040 0000 0073 fe00 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
+00000050: 6403 6c04 5400 6402 6404 6c05 6d06 5a06  d.l.T.d.d.l.m.Z.
+00000060: 0100 6402 6405 6c07 6d08 5a08 0100 6402  ..d.d.l.m.Z...d.
+00000070: 6406 6c09 6d0a 5a0a 0100 6402 6407 6c0b  d.l.m.Z...d.d.l.
+00000080: 6d0c 5a0c 0100 6500 a00d a100 5a0e 650a  m.Z...e.....Z.e.
+00000090: 8300 5a0f 6508 6408 6409 8d01 5a10 6506  ..Z.e.d.d...Z.e.
+000000a0: 8300 5a11 650c 6511 8301 5a12 6513 8300  ..Z.e.e...Z.e...
+000000b0: 5a04 6514 6504 640a 1900 8301 5a15 650e  Z.e.e.d.....Z.e.
+000000c0: a016 a100 640b 640c 8400 8301 5a17 650e  ....d.d.....Z.e.
+000000d0: a016 a100 640d 640e 8400 8301 5a18 650e  ....d.d.....Z.e.
+000000e0: a016 a100 6519 640f 9c01 6410 6411 8404  ....e.d...d.d...
+000000f0: 8301 5a1a 650e a016 a100 6412 6413 8400  ..Z.e.....d.d...
+00000100: 8301 5a1b 650e a016 a100 6519 6414 9c01  ..Z.e.....e.d...
+00000110: 6415 6416 8404 8301 5a1c 651d 6417 6b02  d.d.....Z.e.d.k.
+00000120: 72fa 650e 8300 0100 6401 5300 2918 e900  r.e.....d.S.)...
+00000130: 0000 004e e901 0000 0029 01da 012a 2901  ...N.....)...*).
+00000140: da0f 4461 7461 6261 7365 4d61 6e61 6765  ..DatabaseManage
+00000150: 7229 01da 0f41 7564 696f 5072 6f63 6573  r)...AudioProces
+00000160: 7369 6e67 2901 da0b 4175 6469 6f52 6561  sing)...AudioRea
+00000170: 6465 7229 01da 074d 6174 6368 6572 4629  der)...MatcherF)
+00000180: 01da 0470 6c6f 745a 0b6c 6973 7465 6e5f  ...plotZ.listen_
+00000190: 7469 6d65 6300 0000 0000 0000 0000 0000  timec...........
+000001a0: 0000 0000 0003 0000 0043 0000 0073 1800  .........C...s..
+000001b0: 0000 7400 a001 6401 a101 0100 7400 a001  ..t...d.....t...
+000001c0: 6402 a101 0100 6400 5300 2903 4e7a 1357  d.....d.S.).Nz.W
+000001d0: 656c 636f 6d65 2074 6f20 4646 5472 6163  elcome to FFTrac
+000001e0: 6b21 7a2e 5573 6520 7468 6520 2d2d 6865  k!z.Use the --he
+000001f0: 6c70 2066 6c61 6720 746f 2073 6565 2061  lp flag to see a
+00000200: 7661 696c 6162 6c65 2063 6f6d 6d61 6e64  vailable command
+00000210: 732e 2902 da05 7479 7065 72da 0465 6368  s.)...typer..ech
+00000220: 6fa9 0072 0b00 0000 720b 0000 00fa 4e2f  o..r....r.....N/
+00000230: 5573 6572 732f 6e69 636f 6c61 732f 4465  Users/nicolas/De
+00000240: 7665 6c6f 7065 722f 776f 726b 7370 6163  veloper/workspac
+00000250: 652f 556e 692f 4c32 2f53 342f 5072 6f6a  e/Uni/L2/S4/Proj
+00000260: 6574 2f64 6f73 7369 6572 5356 4e2f 6666  et/dossierSVN/ff
+00000270: 7472 6163 6b2f 6d61 696e 2e70 79da 046d  track/main.py..m
+00000280: 6169 6e18 0000 0073 0400 0000 0002 0a01  ain....s........
+00000290: 720d 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000002a0: 0000 0500 0000 0a00 0000 4300 0000 7366  ..........C...sf
+000002b0: 0100 007a 3a74 00a0 0164 0174 029b 0064  ...z:t...d.t...d
+000002c0: 029d 03a1 0101 0074 03a0 04a1 0001 0074  .......t.......t
+000002d0: 05a0 0674 02a1 0101 0074 03a0 07a1 0001  ...t.....t......
+000002e0: 0074 00a0 0164 03a1 0101 0057 006e 3804  .t...d.....W.n8.
+000002f0: 0074 086b 0a72 7201 007d 0001 007a 1a74  .t.k.rr..}...z.t
+00000300: 00a0 0164 047c 009b 009d 02a1 0101 0057  ...d.|.........W
+00000310: 0059 00a2 0464 0053 0064 007d 007e 0058  .Y...d.S.d.}.~.X
+00000320: 0059 006e 0258 007a 3074 00a0 0164 05a1  .Y.n.X.z0t...d..
+00000330: 0101 0074 09a0 0a74 036a 0ba1 017d 0174  ...t...t.j...}.t
+00000340: 00a0 0164 0674 0c7c 0183 019b 0064 079d  ...d.t.|.....d..
+00000350: 03a1 0101 0057 006e 3804 0074 086b 0a72  .....W.n8..t.k.r
+00000360: dc01 007d 0001 007a 1a74 00a0 0164 087c  ...}...z.t...d.|
+00000370: 009b 009d 02a1 0101 0057 0059 00a2 0464  .........W.Y...d
+00000380: 0053 0064 007d 007e 0058 0059 006e 0258  .S.d.}.~.X.Y.n.X
+00000390: 007a 4874 00a0 0164 09a1 0101 0074 0da0  .zHt...d.....t..
+000003a0: 0e7c 01a1 017d 027c 0290 0172 1a7c 025c  .|...}.|...r.|.\
+000003b0: 027d 037d 0474 00a0 0164 0a7c 039b 0064  .}.}.t...d.|...d
+000003c0: 0b7c 049b 009d 04a1 0101 006e 0a74 00a0  .|.........n.t..
+000003d0: 0164 0ca1 0101 0057 006e 3a04 0074 086b  .d.....W.n:..t.k
+000003e0: 0a90 0172 6001 007d 0001 007a 1a74 00a0  ...r`..}...z.t..
+000003f0: 0164 0d7c 009b 009d 02a1 0101 0057 0059  .d.|.........W.Y
+00000400: 00a2 0464 0053 0064 007d 007e 0058 0059  ...d.S.d.}.~.X.Y
+00000410: 006e 0258 0064 0053 0029 0e4e 7a0e 4c69  .n.X.d.S.).Nz.Li
+00000420: 7374 656e 696e 6720 666f 7220 7a04 732e  stening for z.s.
+00000430: 2e2e 7a19 4175 6469 6f20 7265 636f 7264  ..z.Audio record
+00000440: 696e 6720 636f 6d70 6c65 7465 2e7a 1745  ing complete.z.E
+00000450: 7272 6f72 2072 6563 6f72 6469 6e67 2061  rror recording a
+00000460: 7564 696f 3a20 fa13 5072 6f63 6573 7369  udio: ..Processi
+00000470: 6e67 2061 7564 696f 2e2e 2efa 0a47 656e  ng audio.....Gen
+00000480: 6572 6174 6564 20fa 1b20 6669 6e67 6572  erated .. finger
+00000490: 7072 696e 7473 2073 7563 6365 7373 6675  prints successfu
+000004a0: 6c6c 792e fa18 4572 726f 7220 7072 6f63  lly...Error proc
+000004b0: 6573 7369 6e67 2061 7564 696f 3a20 fa11  essing audio: ..
+000004c0: 4d61 7463 6869 6e67 2061 7564 696f 2e2e  Matching audio..
+000004d0: 2efa 1442 6573 7420 6d61 7463 683a 2053  ...Best match: S
+000004e0: 6f6e 6720 4944 20fa 112c 204d 6174 6368  ong ID .., Match
+000004f0: 2064 6574 6169 6c73 3a20 fa0f 4e6f 206d   details: ..No m
+00000500: 6174 6368 2066 6f75 6e64 2efa 1645 7272  atch found...Err
+00000510: 6f72 206d 6174 6368 696e 6720 6175 6469  or matching audi
+00000520: 6f3a 2029 0f72 0900 0000 720a 0000 00da  o: ).r....r.....
+00000530: 0b4c 4953 5445 4e5f 5449 4d45 da0c 6175  .LISTEN_TIME..au
+00000540: 6469 6f5f 7265 6164 6572 da0f 7374 6172  dio_reader..star
+00000550: 745f 7265 636f 7264 696e 67da 0474 696d  t_recording..tim
+00000560: 65da 0573 6c65 6570 da0e 7374 6f70 5f72  e..sleep..stop_r
+00000570: 6563 6f72 6469 6e67 da09 4578 6365 7074  ecording..Except
+00000580: 696f 6eda 0f61 7564 696f 5f70 726f 6365  ion..audio_proce
+00000590: 7373 6f72 da1f 6765 6e65 7261 7465 5f66  ssor..generate_f
+000005a0: 696e 6765 7270 7269 6e74 735f 6672 6f6d  ingerprints_from
+000005b0: 5f66 696c 65da 0f6f 7574 7075 745f 6669  _file..output_fi
+000005c0: 6c65 6e61 6d65 da03 6c65 6eda 076d 6174  lename..len..mat
+000005d0: 6368 6572 da0e 6765 745f 6265 7374 5f6d  cher..get_best_m
+000005e0: 6174 6368 2905 da01 65da 0c66 696e 6765  atch)...e..finge
+000005f0: 7270 7269 6e74 73da 0a62 6573 745f 6d61  rprints..best_ma
+00000600: 7463 68da 0773 6f6e 675f 6964 da0d 6d61  tch..song_id..ma
+00000610: 7463 685f 6465 7461 696c 7372 0b00 0000  tch_detailsr....
+00000620: 720b 0000 0072 0c00 0000 da06 6c69 7374  r....r......list
+00000630: 656e 1e00 0000 7334 0000 0000 0302 0112  en....s4........
+00000640: 0108 010a 0108 010e 0110 0110 0218 0302  ................
+00000650: 010a 010c 011a 0110 0110 0118 0202 020a  ................
+00000660: 010a 0106 0108 0118 020e 0112 0110 0172  ...............r
+00000670: 2900 0000 2901 da09 6669 6c65 5f70 6174  )...)...file_pat
+00000680: 6863 0100 0000 0000 0000 0000 0000 0700  hc..............
+00000690: 0000 0a00 0000 4300 0000 735e 0100 007a  ......C...s^...z
+000006a0: 1874 00a0 0164 01a1 0101 0074 02a0 037c  .t...d.....t...|
+000006b0: 00a1 0101 0057 006e 3804 0074 046b 0a72  .....W.n8..t.k.r
+000006c0: 5001 007d 0101 007a 1a74 00a0 0164 027c  P..}...z.t...d.|
+000006d0: 019b 009d 02a1 0101 0057 0059 00a2 0464  .........W.Y...d
+000006e0: 0053 0064 007d 017e 0158 0059 006e 0258  .S.d.}.~.X.Y.n.X
+000006f0: 007a 3074 00a0 0164 03a1 0101 0074 05a0  .z0t...d.....t..
+00000700: 0674 026a 07a1 017d 0274 00a0 0164 0474  .t.j...}.t...d.t
+00000710: 087c 0283 019b 0064 059d 03a1 0101 0057  .|.....d.......W
+00000720: 006e 3804 0074 046b 0a72 ba01 007d 0101  .n8..t.k.r...}..
+00000730: 007a 1a74 00a0 0164 067c 019b 009d 02a1  .z.t...d.|......
+00000740: 0101 0057 0059 00a2 0464 0053 0064 007d  ...W.Y...d.S.d.}
+00000750: 017e 0158 0059 006e 0258 007a 6274 00a0  .~.X.Y.n.X.zbt..
+00000760: 0164 07a1 0101 0074 09a0 0a7c 02a1 017d  .d.....t...|...}
+00000770: 037c 0390 0172 127c 035c 027d 047d 0574  .|...r.|.\.}.}.t
+00000780: 00a0 0164 087c 049b 0064 097c 059b 009d  ...d.|...d.|....
+00000790: 04a1 0101 0074 0ba0 0c7c 04a1 017d 0674  .....t...|...}.t
+000007a0: 00a0 0164 0a7c 069b 009d 02a1 0101 006e  ...d.|.........n
+000007b0: 0a74 00a0 0164 0ba1 0101 0057 006e 3a04  .t...d.....W.n:.
+000007c0: 0074 046b 0a90 0172 5801 007d 0101 007a  .t.k...rX..}...z
+000007d0: 1a74 00a0 0164 0c7c 019b 009d 02a1 0101  .t...d.|........
+000007e0: 0057 0059 00a2 0464 0053 0064 007d 017e  .W.Y...d.S.d.}.~
+000007f0: 0158 0059 006e 0258 0064 0053 0029 0d4e  .X.Y.n.X.d.S.).N
+00000800: 7a15 4c6f 6164 696e 6720 6175 6469 6f20  z.Loading audio 
+00000810: 6669 6c65 2e2e 2e7a 1a45 7272 6f72 206c  file...z.Error l
+00000820: 6f61 6469 6e67 2061 7564 696f 2066 696c  oading audio fil
+00000830: 653a 2072 0e00 0000 720f 0000 0072 1000  e: r....r....r..
+00000840: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000850: 0072 1400 0000 7a0e 536f 6e67 2064 6574  .r....z.Song det
+00000860: 6169 6c73 3a20 7215 0000 0072 1600 0000  ails: r....r....
+00000870: 290d 7209 0000 0072 0a00 0000 7218 0000  ).r....r....r...
+00000880: 00da 0c61 7564 696f 5f74 6f5f 7761 7672  ...audio_to_wavr
+00000890: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+000008a0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
+000008b0: 0000 da02 6462 da0e 6765 745f 736f 6e67  ....db..get_song
+000008c0: 5f62 795f 6964 2907 722a 0000 0072 2400  _by_id).r*...r$.
+000008d0: 0000 7225 0000 0072 2600 0000 7227 0000  ..r%...r&...r'..
+000008e0: 0072 2800 0000 da04 736f 6e67 720b 0000  .r(.....songr...
+000008f0: 0072 0b00 0000 720c 0000 00da 0869 6465  .r....r......ide
+00000900: 6e74 6966 7943 0000 0073 3200 0000 0003  ntifyC...s2.....
+00000910: 0201 0a01 0e01 1001 1001 1803 0201 0a01  ................
+00000920: 0c01 1a01 1001 1001 1802 0202 0a01 0a01  ................
+00000930: 0601 0801 1602 0a01 1202 0e01 1201 1001  ................
+00000940: 722f 0000 0063 0000 0000 0000 0000 0000  r/...c..........
+00000950: 0000 0000 0000 0300 0000 4300 0000 7318  ..........C...s.
+00000960: 0000 0074 00a0 0164 01a1 0101 0074 00a0  ...t...d.....t..
+00000970: 0174 02a1 0101 0064 0053 0029 024e 7a16  .t.....d.S.).Nz.
+00000980: 4375 7272 656e 7420 636f 6e66 6967 7572  Current configur
+00000990: 6174 696f 6e3a a903 7209 0000 0072 0a00  ation:..r....r..
+000009a0: 0000 da06 636f 6e66 6967 720b 0000 0072  ....configr....r
+000009b0: 0b00 0000 720b 0000 0072 0c00 0000 da0a  ....r....r......
+000009c0: 6765 745f 636f 6e66 6967 6700 0000 7304  get_configg...s.
+000009d0: 0000 0000 020a 0172 3200 0000 a901 da07  .......r2.......
+000009e0: 7365 7474 696e 6763 0100 0000 0000 0000  settingc........
+000009f0: 0000 0000 0100 0000 0700 0000 4300 0000  ............C...
+00000a00: 731e 0000 0074 00a0 0164 017c 009b 0064  s....t...d.|...d
+00000a10: 0274 027c 0019 009b 009d 04a1 0101 0064  .t.|...........d
+00000a20: 0053 0029 034e 7a11 4375 7272 656e 7420  .S.).Nz.Current 
+00000a30: 7661 6c75 6520 6f66 207a 023a 2072 3000  value of z.: r0.
+00000a40: 0000 7233 0000 0072 0b00 0000 720b 0000  ..r3...r....r...
+00000a50: 0072 0c00 0000 da0b 6765 745f 7365 7474  .r......get_sett
+00000a60: 696e 676d 0000 0073 0200 0000 0002 7235  ingm...s......r5
+00000a70: 0000 00da 085f 5f6d 6169 6e5f 5f29 1e72  .....__main__).r
+00000a80: 0900 0000 da02 6f73 da04 6a73 6f6e 721a  ......os..jsonr.
+00000a90: 0000 0072 3100 0000 5a13 6461 7461 6261  ...r1...Z.databa
+00000aa0: 7365 2e64 625f 6d61 6e61 6765 7272 0400  se.db_managerr..
+00000ab0: 0000 5a15 6175 6469 6f2e 4175 6469 6f50  ..Z.audio.AudioP
+00000ac0: 726f 6365 7373 696e 6772 0500 0000 5a12  rocessingr....Z.
+00000ad0: 6175 6469 6f2e 6175 6469 6f5f 7265 6164  audio.audio_read
+00000ae0: 6572 7206 0000 005a 106d 6174 6368 696e  err....Z.matchin
+00000af0: 672e 6d61 7463 6865 7272 0700 0000 5a05  g.matcherr....Z.
+00000b00: 5479 7065 72da 0361 7070 7218 0000 0072  Typer..appr....r
+00000b10: 1e00 0000 722c 0000 0072 2200 0000 da0b  ....r,...r".....
+00000b20: 6c6f 6164 5f63 6f6e 6669 67da 0369 6e74  load_config..int
+00000b30: 7217 0000 00da 0763 6f6d 6d61 6e64 720d  r......commandr.
+00000b40: 0000 0072 2900 0000 da03 7374 7272 2f00  ...r).....strr/.
+00000b50: 0000 7232 0000 0072 3500 0000 da08 5f5f  ..r2...r5.....__
+00000b60: 6e61 6d65 5f5f 720b 0000 0072 0b00 0000  name__r....r....
+00000b70: 720b 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
+00000b80: 756c 653e 0100 0000 7336 0000 0008 0108  ule>....s6......
+00000b90: 0108 0108 0208 010c 010c 010c 010c 0208  ................
+00000ba0: 0106 010a 0106 0108 0306 010c 0406 010a  ................
+00000bb0: 0506 010a 2406 0110 2306 010a 0506 0110  ....$...#.......
+00000bc0: 0408 01                                  ...
```

### Comparing `fftrack-0.1.0/fftrack/ui/cli.py` & `fftrack-0.1.1/fftrack/ui/cli.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack/ui/main_cli.py` & `fftrack-0.1.1/fftrack/ui/main_cli.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/fftrack.egg-info/SOURCES.txt` & `fftrack-0.1.1/fftrack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 fftrack/database/models.py
 fftrack/database/__pycache__/__init__.cpython-38.pyc
 fftrack/database/__pycache__/__init__.cpython-39.pyc
 fftrack/database/__pycache__/db_manager.cpython-38.pyc
 fftrack/database/__pycache__/db_manager.cpython-39.pyc
 fftrack/database/__pycache__/models.cpython-38.pyc
 fftrack/database/__pycache__/models.cpython-39.pyc
+fftrack/matching/__init__.py
 fftrack/matching/main_matching.py
 fftrack/matching/matcher.py
 fftrack/matching/__pycache__/__init__.cpython-38.pyc
 fftrack/matching/__pycache__/__init__.cpython-39.pyc
 fftrack/matching/__pycache__/main_matching.cpython-38.pyc
 fftrack/matching/__pycache__/matcher.cpython-38.pyc
 fftrack/matching/__pycache__/matcher.cpython-39.pyc
```

### Comparing `fftrack-0.1.0/fftrack.egg-info/requires.txt` & `fftrack-0.1.1/fftrack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/pyproject.toml` & `fftrack-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/requirements.txt` & `fftrack-0.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.0/setup.py` & `fftrack-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fftrack',
-    version='0.1.0',
+    version='0.1.1',
     description='FFTrack is a Python-based music recognition tool that allows users to identify songs from audio input.',
     author='schuldt-ogre <nschuldt@ogre.run>',
     packages=find_packages(),
     package_data={
         'fftrack': ['config.json'],
     },
     install_requires=[
```

