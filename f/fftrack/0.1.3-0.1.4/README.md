# Comparing `tmp/fftrack-0.1.3.tar.gz` & `tmp/fftrack-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fftrack-0.1.3.tar", last modified: Thu May  2 11:04:57 2024, max compression
+gzip compressed data, was "fftrack-0.1.4.tar", last modified: Thu May  2 11:15:58 2024, max compression
```

## Comparing `fftrack-0.1.3.tar` & `fftrack-0.1.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.336799 fftrack-0.1.3/
--rw-r--r--   0 nicolas    (501) staff       (20)      123 2024-05-02 09:53:34.000000 fftrack-0.1.3/MANIFEST.in
--rw-r--r--   0 nicolas    (501) staff       (20)      299 2024-05-02 11:04:57.336634 fftrack-0.1.3/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)     1487 2024-05-02 09:53:22.000000 fftrack-0.1.3/README.md
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.320771 fftrack-0.1.3/fftrack/
--rw-r--r--   0 nicolas    (501) staff       (20)      475 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)       59 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/__main__.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.324525 fftrack-0.1.3/fftrack/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)      562 2024-04-29 16:25:05.000000 fftrack-0.1.3/fftrack/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      562 2024-04-29 16:26:08.000000 fftrack-0.1.3/fftrack/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      243 2024-04-18 10:03:05.000000 fftrack-0.1.3/fftrack/__pycache__/__main__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      243 2024-04-23 08:20:35.000000 fftrack-0.1.3/fftrack/__pycache__/__main__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     1213 2024-05-02 10:19:16.000000 fftrack-0.1.3/fftrack/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     1254 2024-05-02 10:10:11.000000 fftrack-0.1.3/fftrack/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     3011 2024-05-02 10:19:16.000000 fftrack-0.1.3/fftrack/__pycache__/main.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     2999 2024-05-02 10:00:43.000000 fftrack-0.1.3/fftrack/__pycache__/main.cpython-39.pyc
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.326088 fftrack-0.1.3/fftrack/audio/
--rw-r--r--   0 nicolas    (501) staff       (20)     9160 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/audio/AudioProcessing.py
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-04-10 15:51:20.000000 fftrack-0.1.3/fftrack/audio/__init__.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.328507 fftrack-0.1.3/fftrack/audio/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)     7618 2024-04-29 16:25:06.000000 fftrack-0.1.3/fftrack/audio/__pycache__/AudioProcessing.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     7600 2024-04-29 16:26:09.000000 fftrack-0.1.3/fftrack/audio/__pycache__/AudioProcessing.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      179 2024-04-10 15:51:24.000000 fftrack-0.1.3/fftrack/audio/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      179 2024-04-23 08:06:43.000000 fftrack-0.1.3/fftrack/audio/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     6310 2024-04-10 11:03:17.000000 fftrack-0.1.3/fftrack/audio/__pycache__/audio_compare.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     3613 2024-05-02 10:19:15.000000 fftrack-0.1.3/fftrack/audio/__pycache__/audio_reader.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     3613 2024-04-29 16:26:24.000000 fftrack-0.1.3/fftrack/audio/__pycache__/audio_reader.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     9345 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/audio/audio_compare.py
--rw-r--r--   0 nicolas    (501) staff       (20)     3700 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/audio/audio_reader.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1203 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/audio/main_audio.py
--rw-r--r--   0 nicolas    (501) staff       (20)      465 2024-04-18 16:39:51.000000 fftrack-0.1.3/fftrack/config.json
--rw-r--r--   0 nicolas    (501) staff       (20)     1077 2024-05-02 10:09:46.000000 fftrack-0.1.3/fftrack/config.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.329416 fftrack-0.1.3/fftrack/database/
--rw-r--r--   0 nicolas    (501) staff       (20)       78 2024-03-31 21:16:40.000000 fftrack-0.1.3/fftrack/database/__init__.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.330977 fftrack-0.1.3/fftrack/database/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)      289 2024-03-31 21:19:52.000000 fftrack-0.1.3/fftrack/database/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      289 2024-04-23 08:06:41.000000 fftrack-0.1.3/fftrack/database/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4825 2024-04-29 16:25:05.000000 fftrack-0.1.3/fftrack/database/__pycache__/db_manager.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4817 2024-04-29 16:26:08.000000 fftrack-0.1.3/fftrack/database/__pycache__/db_manager.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     2313 2024-04-29 16:25:05.000000 fftrack-0.1.3/fftrack/database/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     2313 2024-04-29 16:26:09.000000 fftrack-0.1.3/fftrack/database/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4819 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/database/db_manager.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1652 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/database/main_db.py
--rw-r--r--   0 nicolas    (501) staff       (20)     2032 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/database/models.py
--rw-r--r--   0 nicolas    (501) staff       (20)     3275 2024-05-02 09:53:22.000000 fftrack-0.1.3/fftrack/main.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.331562 fftrack-0.1.3/fftrack/matching/
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-05-02 10:28:07.000000 fftrack-0.1.3/fftrack/matching/__init__.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.332937 fftrack-0.1.3/fftrack/matching/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)      182 2024-05-02 10:42:51.000000 fftrack-0.1.3/fftrack/matching/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      221 2024-04-23 08:20:35.000000 fftrack-0.1.3/fftrack/matching/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     1926 2024-04-09 09:49:28.000000 fftrack-0.1.3/fftrack/matching/__pycache__/main_matching.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4728 2024-05-02 10:19:16.000000 fftrack-0.1.3/fftrack/matching/__pycache__/matcher.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4736 2024-04-29 16:26:24.000000 fftrack-0.1.3/fftrack/matching/__pycache__/matcher.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     6334 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/matching/main_matching.py
--rw-r--r--   0 nicolas    (501) staff       (20)     7345 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/matching/matcher.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.333615 fftrack-0.1.3/fftrack/scripts/
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-05-02 09:54:41.000000 fftrack-0.1.3/fftrack/scripts/__init__.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.334807 fftrack-0.1.3/fftrack/scripts/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)      181 2024-05-02 10:42:51.000000 fftrack-0.1.3/fftrack/scripts/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)      181 2024-04-23 08:42:12.000000 fftrack-0.1.3/fftrack/scripts/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4156 2024-05-02 10:42:51.000000 fftrack-0.1.3/fftrack/scripts/__pycache__/populate_database.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4171 2024-04-23 08:45:30.000000 fftrack-0.1.3/fftrack/scripts/__pycache__/populate_database.cpython-39.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     4926 2024-05-02 09:54:41.000000 fftrack-0.1.3/fftrack/scripts/populate_database.py
--rw-r--r--   0 nicolas    (501) staff       (20)      261 2024-05-02 09:54:41.000000 fftrack-0.1.3/fftrack/scripts/songs_to_download.csv
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.335734 fftrack-0.1.3/fftrack/ui/
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.335840 fftrack-0.1.3/fftrack/ui/__pycache__/
--rw-r--r--   0 nicolas    (501) staff       (20)     2323 2024-04-18 08:54:51.000000 fftrack-0.1.3/fftrack/ui/__pycache__/main_cli_nicolas.cpython-38.pyc
--rw-r--r--   0 nicolas    (501) staff       (20)     2533 2024-04-18 09:05:36.000000 fftrack-0.1.3/fftrack/ui/cli.py
--rw-r--r--   0 nicolas    (501) staff       (20)     4525 2024-04-18 09:05:36.000000 fftrack-0.1.3/fftrack/ui/main_cli.py
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-04-29 16:19:29.000000 fftrack-0.1.3/fftrack/ui/main_cli_nicolas.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:04:57.321879 fftrack-0.1.3/fftrack.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)      299 2024-05-02 11:04:57.000000 fftrack-0.1.3/fftrack.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)     2457 2024-05-02 11:04:57.000000 fftrack-0.1.3/fftrack.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2024-05-02 11:04:57.000000 fftrack-0.1.3/fftrack.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas    (501) staff       (20)      105 2024-05-02 11:04:57.000000 fftrack-0.1.3/fftrack.egg-info/entry_points.txt
--rw-r--r--   0 nicolas    (501) staff       (20)     1232 2024-05-02 11:04:57.000000 fftrack-0.1.3/fftrack.egg-info/requires.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        8 2024-05-02 11:04:57.000000 fftrack-0.1.3/fftrack.egg-info/top_level.txt
--rw-r--r--   0 nicolas    (501) staff       (20)     2012 2024-04-29 16:19:29.000000 fftrack-0.1.3/pyproject.toml
--rw-r--r--   0 nicolas    (501) staff       (20)     1239 2024-04-29 16:19:29.000000 fftrack-0.1.3/requirements.txt
--rw-r--r--   0 nicolas    (501) staff       (20)       38 2024-05-02 11:04:57.336858 fftrack-0.1.3/setup.cfg
--rw-r--r--   0 nicolas    (501) staff       (20)     2643 2024-05-02 11:03:38.000000 fftrack-0.1.3/setup.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.709363 fftrack-0.1.4/
+-rw-r--r--   0 nicolas    (501) staff       (20)      123 2024-05-02 09:53:34.000000 fftrack-0.1.4/MANIFEST.in
+-rw-r--r--   0 nicolas    (501) staff       (20)      299 2024-05-02 11:15:58.709186 fftrack-0.1.4/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)     1487 2024-05-02 09:53:22.000000 fftrack-0.1.4/README.md
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.693836 fftrack-0.1.4/fftrack/
+-rw-r--r--   0 nicolas    (501) staff       (20)      475 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)       59 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/__main__.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.696957 fftrack-0.1.4/fftrack/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)      562 2024-04-29 16:25:05.000000 fftrack-0.1.4/fftrack/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      562 2024-04-29 16:26:08.000000 fftrack-0.1.4/fftrack/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      243 2024-04-18 10:03:05.000000 fftrack-0.1.4/fftrack/__pycache__/__main__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      243 2024-04-23 08:20:35.000000 fftrack-0.1.4/fftrack/__pycache__/__main__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     1213 2024-05-02 10:19:16.000000 fftrack-0.1.4/fftrack/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     1254 2024-05-02 10:10:11.000000 fftrack-0.1.4/fftrack/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     3011 2024-05-02 10:19:16.000000 fftrack-0.1.4/fftrack/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     2999 2024-05-02 10:00:43.000000 fftrack-0.1.4/fftrack/__pycache__/main.cpython-39.pyc
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.698819 fftrack-0.1.4/fftrack/audio/
+-rw-r--r--   0 nicolas    (501) staff       (20)     9160 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/audio/AudioProcessing.py
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-04-10 15:51:20.000000 fftrack-0.1.4/fftrack/audio/__init__.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.701100 fftrack-0.1.4/fftrack/audio/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)     7618 2024-04-29 16:25:06.000000 fftrack-0.1.4/fftrack/audio/__pycache__/AudioProcessing.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     7600 2024-04-29 16:26:09.000000 fftrack-0.1.4/fftrack/audio/__pycache__/AudioProcessing.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      179 2024-04-10 15:51:24.000000 fftrack-0.1.4/fftrack/audio/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      179 2024-04-23 08:06:43.000000 fftrack-0.1.4/fftrack/audio/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     6310 2024-04-10 11:03:17.000000 fftrack-0.1.4/fftrack/audio/__pycache__/audio_compare.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     3613 2024-05-02 10:19:15.000000 fftrack-0.1.4/fftrack/audio/__pycache__/audio_reader.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     3613 2024-04-29 16:26:24.000000 fftrack-0.1.4/fftrack/audio/__pycache__/audio_reader.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     9345 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/audio/audio_compare.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     3700 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/audio/audio_reader.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1203 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/audio/main_audio.py
+-rw-r--r--   0 nicolas    (501) staff       (20)      465 2024-04-18 16:39:51.000000 fftrack-0.1.4/fftrack/config.json
+-rw-r--r--   0 nicolas    (501) staff       (20)     1077 2024-05-02 10:09:46.000000 fftrack-0.1.4/fftrack/config.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.702028 fftrack-0.1.4/fftrack/database/
+-rw-r--r--   0 nicolas    (501) staff       (20)       78 2024-03-31 21:16:40.000000 fftrack-0.1.4/fftrack/database/__init__.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.703740 fftrack-0.1.4/fftrack/database/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)      289 2024-03-31 21:19:52.000000 fftrack-0.1.4/fftrack/database/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      289 2024-04-23 08:06:41.000000 fftrack-0.1.4/fftrack/database/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4825 2024-04-29 16:25:05.000000 fftrack-0.1.4/fftrack/database/__pycache__/db_manager.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4817 2024-04-29 16:26:08.000000 fftrack-0.1.4/fftrack/database/__pycache__/db_manager.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     2313 2024-04-29 16:25:05.000000 fftrack-0.1.4/fftrack/database/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     2313 2024-04-29 16:26:09.000000 fftrack-0.1.4/fftrack/database/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4819 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/database/db_manager.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1652 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/database/main_db.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2032 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/database/models.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     3275 2024-05-02 09:53:22.000000 fftrack-0.1.4/fftrack/main.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.704358 fftrack-0.1.4/fftrack/matching/
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-05-02 10:28:07.000000 fftrack-0.1.4/fftrack/matching/__init__.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.705761 fftrack-0.1.4/fftrack/matching/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)      182 2024-05-02 10:42:51.000000 fftrack-0.1.4/fftrack/matching/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      221 2024-04-23 08:20:35.000000 fftrack-0.1.4/fftrack/matching/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     1926 2024-04-09 09:49:28.000000 fftrack-0.1.4/fftrack/matching/__pycache__/main_matching.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4728 2024-05-02 10:19:16.000000 fftrack-0.1.4/fftrack/matching/__pycache__/matcher.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4736 2024-04-29 16:26:24.000000 fftrack-0.1.4/fftrack/matching/__pycache__/matcher.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     6334 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/matching/main_matching.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     7345 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/matching/matcher.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.706389 fftrack-0.1.4/fftrack/scripts/
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-05-02 09:54:41.000000 fftrack-0.1.4/fftrack/scripts/__init__.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.707337 fftrack-0.1.4/fftrack/scripts/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)      181 2024-05-02 10:42:51.000000 fftrack-0.1.4/fftrack/scripts/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)      181 2024-04-23 08:42:12.000000 fftrack-0.1.4/fftrack/scripts/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4156 2024-05-02 10:42:51.000000 fftrack-0.1.4/fftrack/scripts/__pycache__/populate_database.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4171 2024-04-23 08:45:30.000000 fftrack-0.1.4/fftrack/scripts/__pycache__/populate_database.cpython-39.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     4992 2024-05-02 11:12:04.000000 fftrack-0.1.4/fftrack/scripts/populate_database.py
+-rw-r--r--   0 nicolas    (501) staff       (20)      261 2024-05-02 09:54:41.000000 fftrack-0.1.4/fftrack/scripts/songs_to_download.csv
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.708255 fftrack-0.1.4/fftrack/ui/
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.708351 fftrack-0.1.4/fftrack/ui/__pycache__/
+-rw-r--r--   0 nicolas    (501) staff       (20)     2323 2024-04-18 08:54:51.000000 fftrack-0.1.4/fftrack/ui/__pycache__/main_cli_nicolas.cpython-38.pyc
+-rw-r--r--   0 nicolas    (501) staff       (20)     2533 2024-04-18 09:05:36.000000 fftrack-0.1.4/fftrack/ui/cli.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     4525 2024-04-18 09:05:36.000000 fftrack-0.1.4/fftrack/ui/main_cli.py
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2024-04-29 16:19:29.000000 fftrack-0.1.4/fftrack/ui/main_cli_nicolas.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-05-02 11:15:58.694760 fftrack-0.1.4/fftrack.egg-info/
+-rw-r--r--   0 nicolas    (501) staff       (20)      299 2024-05-02 11:15:58.000000 fftrack-0.1.4/fftrack.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)     2457 2024-05-02 11:15:58.000000 fftrack-0.1.4/fftrack.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2024-05-02 11:15:58.000000 fftrack-0.1.4/fftrack.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)      105 2024-05-02 11:15:58.000000 fftrack-0.1.4/fftrack.egg-info/entry_points.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)     1232 2024-05-02 11:15:58.000000 fftrack-0.1.4/fftrack.egg-info/requires.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        8 2024-05-02 11:15:58.000000 fftrack-0.1.4/fftrack.egg-info/top_level.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)     2012 2024-04-29 16:19:29.000000 fftrack-0.1.4/pyproject.toml
+-rw-r--r--   0 nicolas    (501) staff       (20)     1239 2024-04-29 16:19:29.000000 fftrack-0.1.4/requirements.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)       38 2024-05-02 11:15:58.709421 fftrack-0.1.4/setup.cfg
+-rw-r--r--   0 nicolas    (501) staff       (20)     2643 2024-05-02 11:15:46.000000 fftrack-0.1.4/setup.py
```

### Comparing `fftrack-0.1.3/README.md` & `fftrack-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/__pycache__/__init__.cpython-38.pyc` & `fftrack-0.1.4/fftrack/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/__pycache__/__init__.cpython-39.pyc` & `fftrack-0.1.4/fftrack/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/__pycache__/config.cpython-38.pyc` & `fftrack-0.1.4/fftrack/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/__pycache__/config.cpython-39.pyc` & `fftrack-0.1.4/fftrack/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/__pycache__/main.cpython-38.pyc` & `fftrack-0.1.4/fftrack/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/__pycache__/main.cpython-39.pyc` & `fftrack-0.1.4/fftrack/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/audio/AudioProcessing.py` & `fftrack-0.1.4/fftrack/audio/AudioProcessing.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/audio/__pycache__/AudioProcessing.cpython-38.pyc` & `fftrack-0.1.4/fftrack/audio/__pycache__/AudioProcessing.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/audio/__pycache__/AudioProcessing.cpython-39.pyc` & `fftrack-0.1.4/fftrack/audio/__pycache__/AudioProcessing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/audio/__pycache__/audio_compare.cpython-38.pyc` & `fftrack-0.1.4/fftrack/audio/__pycache__/audio_compare.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/audio/__pycache__/audio_reader.cpython-38.pyc` & `fftrack-0.1.4/fftrack/audio/__pycache__/audio_reader.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/audio/__pycache__/audio_reader.cpython-39.pyc` & `fftrack-0.1.4/fftrack/audio/__pycache__/audio_reader.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/audio/audio_compare.py` & `fftrack-0.1.4/fftrack/audio/audio_compare.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/audio/audio_reader.py` & `fftrack-0.1.4/fftrack/audio/audio_reader.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/audio/main_audio.py` & `fftrack-0.1.4/fftrack/audio/main_audio.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/config.py` & `fftrack-0.1.4/fftrack/config.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/database/__pycache__/db_manager.cpython-38.pyc` & `fftrack-0.1.4/fftrack/database/__pycache__/db_manager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/database/__pycache__/db_manager.cpython-39.pyc` & `fftrack-0.1.4/fftrack/database/__pycache__/db_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/database/__pycache__/models.cpython-38.pyc` & `fftrack-0.1.4/fftrack/database/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/database/__pycache__/models.cpython-39.pyc` & `fftrack-0.1.4/fftrack/database/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/database/db_manager.py` & `fftrack-0.1.4/fftrack/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/database/main_db.py` & `fftrack-0.1.4/fftrack/database/main_db.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/database/models.py` & `fftrack-0.1.4/fftrack/database/models.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/main.py` & `fftrack-0.1.4/fftrack/main.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/matching/__pycache__/main_matching.cpython-38.pyc` & `fftrack-0.1.4/fftrack/matching/__pycache__/main_matching.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/matching/__pycache__/matcher.cpython-38.pyc` & `fftrack-0.1.4/fftrack/matching/__pycache__/matcher.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/matching/__pycache__/matcher.cpython-39.pyc` & `fftrack-0.1.4/fftrack/matching/__pycache__/matcher.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/matching/main_matching.py` & `fftrack-0.1.4/fftrack/matching/main_matching.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/matching/matcher.py` & `fftrack-0.1.4/fftrack/matching/matcher.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/scripts/__pycache__/populate_database.cpython-38.pyc` & `fftrack-0.1.4/fftrack/scripts/__pycache__/populate_database.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/scripts/__pycache__/populate_database.cpython-39.pyc` & `fftrack-0.1.4/fftrack/scripts/__pycache__/populate_database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/scripts/populate_database.py` & `fftrack-0.1.4/fftrack/scripts/populate_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 import logging
 import pandas as pd
 from pydub import AudioSegment
 from sqlalchemy.orm import sessionmaker
 from fftrack.database.models import Base, Song, create_database, engine
 from fftrack.database import DatabaseManager
 from fftrack.audio.AudioProcessing import AudioProcessing
+from pkg_resources import resource_filename
 
 # Constant values
 DATABASE_URL = "sqlite:///fftrack.db"
-csv_file_path = "./fftrack/scripts/songs_to_download.csv"
-download_dir = "./fftrack/scripts/downloaded_songs"
+csv_file_path = resource_filename(__name__, "songs_to_download.csv")
+download_dir = resource_filename(__name__, "downloaded_songs")
 delete_existing = False
 delete_downloaded = True
 
 # logging
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
```

### Comparing `fftrack-0.1.3/fftrack/ui/__pycache__/main_cli_nicolas.cpython-38.pyc` & `fftrack-0.1.4/fftrack/ui/__pycache__/main_cli_nicolas.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/ui/cli.py` & `fftrack-0.1.4/fftrack/ui/cli.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack/ui/main_cli.py` & `fftrack-0.1.4/fftrack/ui/main_cli.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack.egg-info/SOURCES.txt` & `fftrack-0.1.4/fftrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/fftrack.egg-info/requires.txt` & `fftrack-0.1.4/fftrack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/pyproject.toml` & `fftrack-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/requirements.txt` & `fftrack-0.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.3/setup.py` & `fftrack-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fftrack',
-    version='0.1.3',
+    version='0.1.4',
     description='FFTrack is a Python-based music recognition tool that allows users to identify songs from audio input.',
     author='schuldt-ogre <nschuldt@ogre.run>',
     packages=find_packages(),
     package_data={
         'fftrack': ['config.json', 'scripts/*.csv'],
     },
     install_requires=[
```

