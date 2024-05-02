# Comparing `tmp/openav-1.0.0a7.tar.gz` & `tmp/openav-1.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openav-1.0.0a7.tar", last modified: Sat Apr 27 19:00:20 2024, max compression
+gzip compressed data, was "openav-1.0.0a8.tar", last modified: Thu May  2 18:33:25 2024, max compression
```

## Comparing `openav-1.0.0a7.tar` & `openav-1.0.0a8.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.836671 openav-1.0.0a7/
--rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a7/LICENSE
--rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a7/MANIFEST.in
--rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 19:00:20.837754 openav-1.0.0a7/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a7/README.md
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.725899 openav-1.0.0a7/openav/
--rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a7/openav/__garbage__.py
--rw-r--r--   0 dl         (501) staff       (20)     1077 2024-04-27 19:00:14.000000 openav-1.0.0a7/openav/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.776563 openav-1.0.0a7/openav/api/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a7/openav/api/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a7/openav/api/augmentation.py
--rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a7/openav/api/download.py
--rw-r--r--   0 dl         (501) staff       (20)    21181 2024-04-27 12:48:45.000000 openav-1.0.0a7/openav/api/preprocess_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    19835 2024-04-27 12:48:33.000000 openav-1.0.0a7/openav/api/preprocess_video.py
--rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a7/openav/api/test_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a7/openav/api/test_video.py
--rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a7/openav/api/testing.py
--rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a7/openav/api/train_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    22373 2024-04-27 18:53:38.000000 openav-1.0.0a7/openav/api/train_audiovisual.py
--rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a7/openav/api/train_video.py
--rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a7/openav/api/vad.py
--rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a7/openav/api/vad_gui.py
--rw-r--r--   0 dl         (501) staff       (20)    23001 2024-04-27 12:49:02.000000 openav-1.0.0a7/openav/api/vosk_sr.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.778232 openav-1.0.0a7/openav/modules/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a7/openav/modules/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.791692 openav-1.0.0a7/openav/modules/core/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a7/openav/modules/core/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    31017 2024-04-26 16:59:06.000000 openav-1.0.0a7/openav/modules/core/core.py
--rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a7/openav/modules/core/exceptions.py
--rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a7/openav/modules/core/language.py
--rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a7/openav/modules/core/logging.py
--rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a7/openav/modules/core/messages.py
--rw-r--r--   0 dl         (501) staff       (20)    14550 2024-04-21 20:40:49.000000 openav-1.0.0a7/openav/modules/core/settings.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.794779 openav-1.0.0a7/openav/modules/dataset_recording/
--rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a7/openav/modules/dataset_recording/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     4518 2024-04-26 09:47:40.000000 openav-1.0.0a7/openav/modules/dataset_recording/app.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.806812 openav-1.0.0a7/openav/modules/file_manager/
--rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a7/openav/modules/file_manager/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a7/openav/modules/file_manager/download.py
--rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a7/openav/modules/file_manager/file_manager.py
--rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a7/openav/modules/file_manager/json_manager.py
--rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a7/openav/modules/file_manager/unzip.py
--rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a7/openav/modules/file_manager/yaml_manager.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.817998 openav-1.0.0a7/openav/modules/lab/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a7/openav/modules/lab/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)   120642 2024-04-24 09:54:17.000000 openav-1.0.0a7/openav/modules/lab/audio.py
--rw-r--r--   0 dl         (501) staff       (20)    27211 2024-04-27 18:57:37.000000 openav-1.0.0a7/openav/modules/lab/audiovisual.py
--rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a7/openav/modules/lab/build.py
--rw-r--r--   0 dl         (501) staff       (20)    24427 2024-04-24 13:03:57.000000 openav-1.0.0a7/openav/modules/lab/video.py
--rw-r--r--   0 dl         (501) staff       (20)      202 2024-04-23 19:00:17.000000 openav-1.0.0a7/openav/modules/lab/video_converter.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.713322 openav-1.0.0a7/openav/modules/locales/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.712764 openav-1.0.0a7/openav/modules/locales/en/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.821237 openav-1.0.0a7/openav/modules/locales/en/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a7/openav/modules/locales/en/LC_MESSAGES/argparse.mo
--rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a7/openav/modules/locales/en/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.714169 openav-1.0.0a7/openav/modules/locales/ru/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.824168 openav-1.0.0a7/openav/modules/locales/ru/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a7/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
--rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a7/openav/modules/locales/ru/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.830474 openav-1.0.0a7/openav/modules/nn/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a7/openav/modules/nn/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    11245 2024-04-26 16:34:46.000000 openav-1.0.0a7/openav/modules/nn/av_dataset.py
--rw-r--r--   0 dl         (501) staff       (20)    10390 2024-04-27 13:08:42.000000 openav-1.0.0a7/openav/modules/nn/models.py
--rw-r--r--   0 dl         (501) staff       (20)     2727 2024-04-26 17:11:00.000000 openav-1.0.0a7/openav/modules/nn/utils.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.832424 openav-1.0.0a7/openav/modules/trml/
--rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a7/openav/modules/trml/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a7/openav/modules/trml/shell.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.834222 openav-1.0.0a7/openav/rsrs/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a7/openav/rsrs/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.835492 openav-1.0.0a7/openav/rsrs/favicon/
--rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a7/openav/rsrs/favicon/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-27 19:00:20.733670 openav-1.0.0a7/openav.egg-info/
--rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-27 19:00:20.000000 openav-1.0.0a7/openav.egg-info/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1834 2024-04-27 19:00:20.000000 openav-1.0.0a7/openav.egg-info/SOURCES.txt
--rw-r--r--   0 dl         (501) staff       (20)        1 2024-04-27 19:00:20.000000 openav-1.0.0a7/openav.egg-info/dependency_links.txt
--rw-r--r--   0 dl         (501) staff       (20)      271 2024-04-27 19:00:20.000000 openav-1.0.0a7/openav.egg-info/entry_points.txt
--rw-r--r--   0 dl         (501) staff       (20)      459 2024-04-27 19:00:20.000000 openav-1.0.0a7/openav.egg-info/requires.txt
--rw-r--r--   0 dl         (501) staff       (20)        7 2024-04-27 19:00:20.000000 openav-1.0.0a7/openav.egg-info/top_level.txt
--rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a7/pyproject.toml
--rw-r--r--   0 dl         (501) staff       (20)       79 2024-04-27 19:00:20.839425 openav-1.0.0a7/setup.cfg
--rw-r--r--   0 dl         (501) staff       (20)     4489 2024-04-26 16:55:19.000000 openav-1.0.0a7/setup.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.302820 openav-1.0.0a8/
+-rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a8/LICENSE
+-rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a8/MANIFEST.in
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-05-02 18:33:25.303416 openav-1.0.0a8/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a8/README.md
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.242962 openav-1.0.0a8/openav/
+-rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a8/openav/__garbage__.py
+-rw-r--r--   0 dl         (501) staff       (20)     1077 2024-05-02 18:33:11.000000 openav-1.0.0a8/openav/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.265587 openav-1.0.0a8/openav/api/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a8/openav/api/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a8/openav/api/augmentation.py
+-rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a8/openav/api/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    21181 2024-04-27 12:48:45.000000 openav-1.0.0a8/openav/api/preprocess_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    19835 2024-04-27 12:48:33.000000 openav-1.0.0a8/openav/api/preprocess_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a8/openav/api/test_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    19855 2024-05-02 17:42:44.000000 openav-1.0.0a8/openav/api/test_audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a8/openav/api/test_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a8/openav/api/testing.py
+-rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a8/openav/api/train_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    22373 2024-04-27 18:53:38.000000 openav-1.0.0a8/openav/api/train_audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a8/openav/api/train_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a8/openav/api/vad.py
+-rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a8/openav/api/vad_gui.py
+-rw-r--r--   0 dl         (501) staff       (20)    23001 2024-04-27 12:49:02.000000 openav-1.0.0a8/openav/api/vosk_sr.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.266863 openav-1.0.0a8/openav/modules/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a8/openav/modules/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.274727 openav-1.0.0a8/openav/modules/core/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a8/openav/modules/core/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    31017 2024-04-26 16:59:06.000000 openav-1.0.0a8/openav/modules/core/core.py
+-rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a8/openav/modules/core/exceptions.py
+-rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/core/language.py
+-rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/core/logging.py
+-rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/core/messages.py
+-rw-r--r--   0 dl         (501) staff       (20)    14550 2024-04-21 20:40:49.000000 openav-1.0.0a8/openav/modules/core/settings.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.276617 openav-1.0.0a8/openav/modules/dataset_recording/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a8/openav/modules/dataset_recording/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     4518 2024-04-26 09:47:40.000000 openav-1.0.0a8/openav/modules/dataset_recording/app.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.282422 openav-1.0.0a8/openav/modules/file_manager/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a8/openav/modules/file_manager/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a8/openav/modules/file_manager/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a8/openav/modules/file_manager/file_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/file_manager/json_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a8/openav/modules/file_manager/unzip.py
+-rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/file_manager/yaml_manager.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.290877 openav-1.0.0a8/openav/modules/lab/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a8/openav/modules/lab/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)   120642 2024-04-24 09:54:17.000000 openav-1.0.0a8/openav/modules/lab/audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    35524 2024-05-02 18:05:21.000000 openav-1.0.0a8/openav/modules/lab/audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/lab/build.py
+-rw-r--r--   0 dl         (501) staff       (20)    24427 2024-04-24 13:03:57.000000 openav-1.0.0a8/openav/modules/lab/video.py
+-rw-r--r--   0 dl         (501) staff       (20)      202 2024-04-23 19:00:17.000000 openav-1.0.0a8/openav/modules/lab/video_converter.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.238180 openav-1.0.0a8/openav/modules/locales/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.237995 openav-1.0.0a8/openav/modules/locales/en/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.292937 openav-1.0.0a8/openav/modules/locales/en/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a8/openav/modules/locales/en/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a8/openav/modules/locales/en/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.238299 openav-1.0.0a8/openav/modules/locales/ru/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.294624 openav-1.0.0a8/openav/modules/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a8/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a8/openav/modules/locales/ru/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.298117 openav-1.0.0a8/openav/modules/nn/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a8/openav/modules/nn/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    11245 2024-04-26 16:34:46.000000 openav-1.0.0a8/openav/modules/nn/av_dataset.py
+-rw-r--r--   0 dl         (501) staff       (20)    11719 2024-05-02 18:32:54.000000 openav-1.0.0a8/openav/modules/nn/models.py
+-rw-r--r--   0 dl         (501) staff       (20)     2727 2024-04-26 17:11:00.000000 openav-1.0.0a8/openav/modules/nn/utils.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.300133 openav-1.0.0a8/openav/modules/trml/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a8/openav/modules/trml/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/trml/shell.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.301706 openav-1.0.0a8/openav/rsrs/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a8/openav/rsrs/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.302290 openav-1.0.0a8/openav/rsrs/favicon/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/rsrs/favicon/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.245826 openav-1.0.0a8/openav.egg-info/
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1865 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/SOURCES.txt
+-rw-r--r--   0 dl         (501) staff       (20)        1 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/dependency_links.txt
+-rw-r--r--   0 dl         (501) staff       (20)      330 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/entry_points.txt
+-rw-r--r--   0 dl         (501) staff       (20)      459 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/requires.txt
+-rw-r--r--   0 dl         (501) staff       (20)        7 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/top_level.txt
+-rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a8/pyproject.toml
+-rw-r--r--   0 dl         (501) staff       (20)       79 2024-05-02 18:33:25.304658 openav-1.0.0a8/setup.cfg
+-rw-r--r--   0 dl         (501) staff       (20)     4567 2024-05-02 18:32:33.000000 openav-1.0.0a8/setup.py
```

### Comparing `openav-1.0.0a7/LICENSE` & `openav-1.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/PKG-INFO` & `openav-1.0.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
```

### Comparing `openav-1.0.0a7/README.md` & `openav-1.0.0a8/README.md`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/__garbage__.py` & `openav-1.0.0a8/openav/__garbage__.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/__init__.py` & `openav-1.0.0a8/openav/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 __title__ = "OpenAV"
 __summary__ = "OpenAV"
 __uri__ = "https://github.com/DmitryRyumin/openav"
 
 __version__ = "1.0"
-__release__ = __version__ + ".0-a7"
+__release__ = __version__ + ".0-a8"
 
 __author__ru__ = "Рюмин Дмитрий, Иванько Денис, Шилов Николай, Маркитантов Максим, Карпов Алексей"
 __author__en__ = "Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov"
 __email__ = (
     "dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, " "karpov@iias.spb.su"
 )
```

### Comparing `openav-1.0.0a7/openav/api/augmentation.py` & `openav-1.0.0a8/openav/api/augmentation.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/download.py` & `openav-1.0.0a8/openav/api/download.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/preprocess_audio.py` & `openav-1.0.0a8/openav/api/preprocess_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/preprocess_video.py` & `openav-1.0.0a8/openav/api/preprocess_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/test_audio.py` & `openav-1.0.0a8/openav/api/test_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/test_video.py` & `openav-1.0.0a8/openav/api/test_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/testing.py` & `openav-1.0.0a8/openav/api/testing.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/train_audio.py` & `openav-1.0.0a8/openav/api/train_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/train_audiovisual.py` & `openav-1.0.0a8/openav/api/train_audiovisual.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/train_video.py` & `openav-1.0.0a8/openav/api/train_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/vad.py` & `openav-1.0.0a8/openav/api/vad.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/vad_gui.py` & `openav-1.0.0a8/openav/api/vad_gui.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/api/vosk_sr.py` & `openav-1.0.0a8/openav/api/vosk_sr.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/core/core.py` & `openav-1.0.0a8/openav/modules/core/core.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/core/exceptions.py` & `openav-1.0.0a8/openav/modules/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/core/language.py` & `openav-1.0.0a8/openav/modules/core/language.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/core/logging.py` & `openav-1.0.0a8/openav/modules/core/logging.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/core/messages.py` & `openav-1.0.0a8/openav/modules/core/messages.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/core/settings.py` & `openav-1.0.0a8/openav/modules/core/settings.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/dataset_recording/app.py` & `openav-1.0.0a8/openav/modules/dataset_recording/app.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/file_manager/download.py` & `openav-1.0.0a8/openav/modules/file_manager/download.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/file_manager/file_manager.py` & `openav-1.0.0a8/openav/modules/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/file_manager/json_manager.py` & `openav-1.0.0a8/openav/modules/file_manager/json_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/file_manager/unzip.py` & `openav-1.0.0a8/openav/modules/file_manager/unzip.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/file_manager/yaml_manager.py` & `openav-1.0.0a8/openav/modules/file_manager/yaml_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/lab/audio.py` & `openav-1.0.0a8/openav/modules/lab/audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/lab/audiovisual.py` & `openav-1.0.0a8/openav/modules/lab/audiovisual.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,18 +43,20 @@
 from openav.modules.nn.models import AVModel
 
 # ######################################################################################################################
 # Константы
 # ######################################################################################################################
 
 SUBFOLDERS: List[str] = ["train", "val", "test"]
+SUBFOLDERS_TEST: List[str] = ["test"]
 SHAPE_AUDIO: List[str] = ["channels", "n_mels", "samples"]
 SHAPE_VIDEO: List[str] = ["frames", "channels", "width", "height"]
 EXT_AV_VIDEO: List[str] = ["mov", "mp4", "webm"]  # Расширения искомых файлов
 EXT_MODELS: str = "pt"
+EXTH_MODELS: str = "pth"
 OPTIMIZERS: List[str] = ["adam", "adamw", "sgd", "lion"]
 REQUIRED_GRAD: List[str] = ["none", "a", "v", "av"]
 
 
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
@@ -70,18 +72,23 @@
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
         super().__post_init__()  # Выполнение конструктора из суперкласса
 
+        self._subfolder_search: str = (
+            self._('Поиск вложенной директории "{}" в директории "{}" (глубина вложенности: {})') + self._em
+        )
         self._subfolders_search: str = (
             self._('Поиск вложенных директорий в директории "{}" (глубина вложенности: {})') + self._em
         )
 
+        self._subfolder_not_found: str = self._("В указанной директории вложенная директория не найдена") + self._em
+
         self._files_audiovisual_find: str = (
             self._('Поиск файлов с расширениями "{}" в директории "{}" (глубина вложенности: {})') + self._em
         )
 
         self._files_audiovisual_find: str = (
             self._('Поиск файлов с расширениями "{}" в директории "{}" (глубина вложенности: {})') + self._em
         )
@@ -94,14 +101,18 @@
             self._(
                 "Минимум одна выборка пустая (обучающая - {}, валидационная - {}, тестовая - {}) или количество меток "
                 + "не совпадает с количеством файлов"
             )
             + self._em
         )
 
+        self._sampling_nn_test_error: str = (
+            self._("Тестовая выборка пустая или количество меток не совпадает с количеством файлов") + self._em
+        )
+
         self._sampling_nn_true: str = self._("Обучающая - {} {}, валидационная - {} {}, тестовая - {} {}") + self._em
         self._format_percentage = lambda x: "({}%)".format(x)
 
         self._run_train: str = self._("Запуск процесса обучения") + self._em
         self._epoch: str = self._("Эпоха: {} из {}") + self._em
         self._loss: str = self._("Значения ошибки: обучение - {}, валидация - {}, тест - {}")
         self._acc_valid_and_test: str = self._("Валидация: точность {} | Тест: точность {}")
@@ -569,7 +580,177 @@
                     else:
                         stop_flag_training += 1
 
                     if stop_flag_training > patience:
                         self.message_info(self._end_train, out=out)
 
                         return True
+
+    def test_audiovisual(
+        self,
+        subfolders: Dict[str, str],
+        n_classes: int,
+        classes: List[str],
+        encoder_decoder: int,
+        max_segment: int,
+        hidden_units: int,
+        hidden_features: int,
+        input_dim: int,
+        shape_audio: Dict[str, int],
+        shape_video: Dict[str, int],
+        path_to_model: str,
+        out: bool = True,
+    ) -> bool:
+        """Автоматическое тестирование на аудиовизуальных данных
+
+        Args:
+            subfolders (Dict[str, str]): Словарь с подкаталогами с данными
+            n_classes (int): Количество классов
+            classes (List[str]): Список классов
+            encoder_decoder (int): Количество энкодеров и декодеров
+            max_segment (int): Максимальная длительность сегмента видео
+            hidden_units (int): Количество скрытых нейронов
+            hidden_features (int): Количество скрытых признаков
+            input_dim (int): Количество входных признаков
+            shape_audio (Dict[str, int]): Входная размерность аудио лог-мел спектрограммы
+            shape_video (Dict[str, int]): Входная размерность видеокадров
+            path_to_model (str): Путь к нейросетевой аудиовизуальной модели
+            out (bool) Отображение
+
+        Returns:
+            bool: **True** если автоматическое тестирование на аудиовизуальных данных произведено, в обратном случае
+            **False**
+        """
+
+        try:
+            # Проверка аргументов
+            if (
+                type(subfolders) is not dict
+                or len(subfolders) == 0
+                or not all(subfolder in subfolders for subfolder in SUBFOLDERS_TEST)
+                or type(n_classes) is not int
+                or not (0 < n_classes)
+                or type(classes) is not list
+                or len(classes) == 0
+                or type(encoder_decoder) is not int
+                or not (1 <= encoder_decoder <= 50)
+                or type(max_segment) is not int
+                or not (1 <= max_segment <= 10)
+                or not (0 < hidden_units)
+                or type(hidden_features) is not int
+                or not (0 < hidden_features)
+                or type(input_dim) is not int
+                or not (0 < input_dim)
+                or type(shape_audio) is not dict
+                or len(shape_audio) == 0
+                or not all(shape in shape_audio for shape in SHAPE_AUDIO)
+                or type(shape_video) is not dict
+                or len(shape_video) == 0
+                or not all(shape in shape_video for shape in SHAPE_VIDEO)
+                or type(path_to_model) is not str
+                or not path_to_model
+                or type(out) is not bool
+            ):
+                raise TypeError
+        except TypeError:
+            self.inv_args(__class__.__name__, self.test_audiovisual.__name__, out=out)
+            return False
+        else:
+            depth = 3
+            classes = [cls.lower() for cls in classes]
+
+            shape_audio = (
+                None,
+                max_segment,
+                shape_audio[SHAPE_AUDIO[0]],
+                shape_audio[SHAPE_AUDIO[1]],
+                shape_audio[SHAPE_AUDIO[2]],
+            )
+            shape_video = (
+                None,
+                max_segment,
+                shape_video[SHAPE_VIDEO[0]],
+                shape_video[SHAPE_VIDEO[1]],
+                shape_video[SHAPE_VIDEO[3]],
+                shape_video[SHAPE_VIDEO[2]],
+            )
+
+            # Информационное сообщение
+            self.message_info(
+                self._subfolder_search.format(
+                    self.message_line(subfolders[SUBFOLDERS_TEST[0]]),
+                    self.message_line(self.path_to_dataset),
+                    self.message_line(str(depth)),
+                ),
+                out=out,
+            )
+
+            nested_paths = self.get_paths(self.path_to_dataset, depth=depth, out=False)
+
+            # Вложенные директории не найдены
+            try:
+                if len(nested_paths) == 0:
+                    raise IsNestedCatalogsNotFoundError
+            except IsNestedCatalogsNotFoundError:
+                self.message_error(self._subfolder_not_found, space=self._space, out=out)
+                return False
+
+            # Информационное сообщение
+            self.message_info(
+                self._files_audiovisual_find.format(
+                    self.message_line(", ".join(x.replace(".", "") for x in EXT_AV_VIDEO)),
+                    self.message_line(self.path_to_dataset),
+                    self.message_line(str(depth)),
+                ),
+                out=out,
+            )
+
+            hierarchy_from_paths = self.__get_hierarchy_from_paths(nested_paths, depth)
+
+            path_test, lb_test = [], []
+
+            # Проход по всем вложенным директориям
+            for nested_path in hierarchy_from_paths:
+                if nested_path[0].lower() in classes:
+                    # Формирование списка с видеофайлами
+                    for p in Path(os.path.join(self.path_to_dataset, *reversed(nested_path))).glob("*"):
+                        # Добавление текущего пути к видеофайлу в список
+                        if p.suffix.lower().replace(".", "") in EXT_AV_VIDEO:
+                            [index for index, cls in enumerate(classes) if cls.lower() == nested_path[0].lower()]
+
+                            if nested_path[-1] == subfolders[SUBFOLDERS_TEST[0]]:
+                                path_test.append(p.resolve())
+                                lb_test.append(classes.index(nested_path[0].lower()))
+                            else:
+                                pass
+
+            # Директории с поднаборами данных не содержат визуальных файлов с необходимыми расширениями
+            try:
+                len_path_test = len(path_test)
+                len_lb_test = len(lb_test)
+
+                if len_path_test == 0 or len_lb_test == 0 or len_path_test != len_lb_test:
+                    raise ValueError
+            except ValueError:
+                self.message_error(
+                    self._sampling_nn_test_error,
+                    space=self._space,
+                    out=out,
+                )
+                return False
+            except Exception:
+                self.message_error(self._unknown_err, space=self._space, out=out)
+                return False
+            else:
+                model = AVModel(
+                    shape_audio=shape_audio,
+                    shape_video=shape_video,
+                    input_dim=input_dim,
+                    h_u=hidden_units,
+                    h_f=hidden_features,
+                    n_class=n_classes,
+                    encoder_decoder=encoder_decoder,
+                ).to(self.__device)
+
+                e = model.load_state_dict(torch.load(path_to_model, map_location=torch.device(self.__device)))
+
+                print(e)
```

### Comparing `openav-1.0.0a7/openav/modules/lab/build.py` & `openav-1.0.0a8/openav/modules/lab/build.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/lab/video.py` & `openav-1.0.0a8/openav/modules/lab/video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/locales/en/LC_MESSAGES/base.mo` & `openav-1.0.0a8/openav/modules/locales/en/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/locales/ru/LC_MESSAGES/argparse.mo` & `openav-1.0.0a8/openav/modules/locales/ru/LC_MESSAGES/argparse.mo`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/nn/av_dataset.py` & `openav-1.0.0a8/openav/modules/nn/av_dataset.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/nn/models.py` & `openav-1.0.0a8/openav/modules/nn/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -244,14 +244,27 @@
         for _ in range(encoder_decoder - 1):
             self.encoders.append(SecondEncoder(input_dim=input_dim))
 
         # Создание декодеров
         for _ in range(encoder_decoder):
             self.decoders.append(Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class))
 
+        # self.enc0 = InitialEncoder(input_dim=input_dim)
+        # self.enc1 = SecondEncoder(input_dim=input_dim)
+        # self.enc2 = SecondEncoder(input_dim=input_dim)
+        # self.enc3 = SecondEncoder(input_dim=input_dim)
+        # self.enc4 = SecondEncoder(input_dim=input_dim)
+        # self.enc5 = SecondEncoder(input_dim=input_dim)
+        # self.dec0 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
+        # self.dec1 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
+        # self.dec2 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
+        # self.dec3 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
+        # self.dec4 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
+        # self.dec5 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
+
     def forward(self, x):
         x_w = [x]
 
         x_w.append(self.encoders[0](x))
 
         for encoder in self.encoders[1:]:
             x_w.append(encoder(x, x_w[-1]))
@@ -261,14 +274,32 @@
             y_all.append(decoder(x_w[i]))
 
         y_all = torch.stack(y_all)
         y_mean = torch.mean(y_all, dim=0)
 
         return y_mean
 
+        # x_w0 = self.enc0(x)
+        # x_w1 = self.enc1(x, x_w0)
+        # x_w2 = self.enc2(x, x_w1)
+        # x_w3 = self.enc3(x, x_w2)
+        # x_w4 = self.enc4(x, x_w3)
+        # x_w5 = self.enc4(x, x_w4)
+        # y0 = self.dec0(x_w0)
+        # y1 = self.dec1(x_w1)
+        # y2 = self.dec2(x_w2)
+        # y3 = self.dec3(x_w3)
+        # y4 = self.dec4(x_w4)
+        # y5 = self.dec4(x_w5)
+
+        # y_all = torch.stack([y0, y1, y2, y3, y4, y5])
+        # y_mean = torch.mean(y_all, dim=0)
+
+        # return y_mean
+
 
 class AVModel(nn.Module):
     def __init__(self, shape_audio, shape_video, input_dim=512, h_u=512, h_f=64, n_class=500, encoder_decoder=5):
         super(AVModel, self).__init__()
         self.feature_audio = ResNet18(channels=shape_audio[2])
         self.fc_audio = nn.Linear(shape_audio[1], h_f)
         self.feature_video = CNNLSTMPyTorch()
```

### Comparing `openav-1.0.0a7/openav/modules/nn/utils.py` & `openav-1.0.0a8/openav/modules/nn/utils.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav/modules/trml/shell.py` & `openav-1.0.0a8/openav/modules/trml/shell.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a7/openav.egg-info/PKG-INFO` & `openav-1.0.0a8/openav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
```

### Comparing `openav-1.0.0a7/openav.egg-info/SOURCES.txt` & `openav-1.0.0a8/openav.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 openav.egg-info/top_level.txt
 openav/api/__init__.py
 openav/api/augmentation.py
 openav/api/download.py
 openav/api/preprocess_audio.py
 openav/api/preprocess_video.py
 openav/api/test_audio.py
+openav/api/test_audiovisual.py
 openav/api/test_video.py
 openav/api/testing.py
 openav/api/train_audio.py
 openav/api/train_audiovisual.py
 openav/api/train_video.py
 openav/api/vad.py
 openav/api/vad_gui.py
```

### Comparing `openav-1.0.0a7/setup.py` & `openav-1.0.0a8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,16 @@
         python_requires=">=3.9, <4",
         entry_points={
             "console_scripts": [
                 "openav_vad = openav.api.vad:main",
                 "openav_vosk_sr = openav.api.vosk_sr:main",
                 "openav_preprocess_audio = openav.api.preprocess_audio:main",
                 "openav_preprocess_video = openav.api.preprocess_video:main",
-                "openav_train_audiovisual = openav.api_train_audiovisual:main",
+                "openav_train_audiovisual = openav.api.train_audiovisual:main",
+                "openav_test_audiovisual = openav.api.test_audiovisual:main",
             ],
         },
         project_urls={
             "Bug Reports": "https://github.com/DmitryRyumin/openav/issues",
             "Documentation": "https://openav.readthedocs.io",
             "Source Code": "https://github.com/DmitryRyumin/openav/tree/main/openav",
             "Download": "https://github.com/DmitryRyumin/openav/tags",
```

