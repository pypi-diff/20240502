# Comparing `tmp/TikTokLive-6.0.5.tar.gz` & `tmp/tiktoklive-6.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/isaackogan/PycharmProjects/TikTokLive/dist/.tmp-7z108tdr/TikTokLive-6.0.5.tar", last modified: Wed Apr 10 04:51:42 2024, max compression
+gzip compressed data, was "/Users/isaackogan/PycharmProjects/TikTokLive/dist/.tmp-0llw1zn2/tiktoklive-6.0.6.tar", last modified: Thu May  2 19:49:22 2024, max compression
```

## Comparing `TikTokLive-6.0.5.tar` & `tiktoklive-6.0.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.188356 TikTokLive-6.0.5/
--rw-r--r--   0 isaackogan   (501) staff       (20)     1068 2024-02-22 06:19:06.000000 TikTokLive-6.0.5/LICENSE
--rw-r--r--   0 isaackogan   (501) staff       (20)    17683 2024-04-10 04:51:42.188045 TikTokLive-6.0.5/PKG-INFO
--rw-r--r--   0 isaackogan   (501) staff       (20)    16551 2024-04-08 20:25:06.000000 TikTokLive-6.0.5/README.md
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.173507 TikTokLive-6.0.5/TikTokLive/
--rw-r--r--   0 isaackogan   (501) staff       (20)       43 2024-02-22 03:47:28.000000 TikTokLive-6.0.5/TikTokLive/__init__.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.175511 TikTokLive-6.0.5/TikTokLive/client/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-11 08:02:27.000000 TikTokLive-6.0.5/TikTokLive/client/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    16401 2024-04-10 00:48:55.000000 TikTokLive-6.0.5/TikTokLive/client/client.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      659 2024-04-08 20:08:19.000000 TikTokLive-6.0.5/TikTokLive/client/errors.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     4209 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/client/logger.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.176403 TikTokLive-6.0.5/TikTokLive/client/web/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-20 23:59:08.000000 TikTokLive-6.0.5/TikTokLive/client/web/__init__.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.179626 TikTokLive-6.0.5/TikTokLive/client/web/routes/
--rw-r--r--   0 isaackogan   (501) staff       (20)      303 2024-04-08 19:26:24.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      925 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_gift_list.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      619 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_image.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2355 2024-04-08 19:57:30.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_is_live.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2803 2024-04-08 19:57:30.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_id_api.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1889 2024-04-08 19:26:01.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_id_html.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1424 2024-04-08 19:50:54.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_info.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     5209 2024-04-03 17:28:04.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_sign.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     6065 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_video.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     4918 2024-04-08 19:22:45.000000 TikTokLive-6.0.5/TikTokLive/client/web/web_base.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1532 2024-04-08 19:57:30.000000 TikTokLive-6.0.5/TikTokLive/client/web/web_client.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2607 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/client/web/web_settings.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.179890 TikTokLive-6.0.5/TikTokLive/client/ws/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2024-02-03 19:50:49.000000 TikTokLive-6.0.5/TikTokLive/client/ws/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     7748 2024-03-22 01:02:42.000000 TikTokLive-6.0.5/TikTokLive/client/ws/ws_client.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.180814 TikTokLive-6.0.5/TikTokLive/events/
--rw-r--r--   0 isaackogan   (501) staff       (20)      567 2024-02-22 06:22:04.000000 TikTokLive-6.0.5/TikTokLive/events/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)      439 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/events/base_event.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2316 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLive/events/custom_events.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     7061 2024-02-28 19:23:41.000000 TikTokLive-6.0.5/TikTokLive/events/proto_events.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.181971 TikTokLive-6.0.5/TikTokLive/proto/
--rw-r--r--   0 isaackogan   (501) staff       (20)       55 2024-02-04 07:15:00.000000 TikTokLive-6.0.5/TikTokLive/proto/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     5166 2024-04-10 04:48:50.000000 TikTokLive-6.0.5/TikTokLive/proto/custom_proto.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2603 2024-04-10 04:24:02.000000 TikTokLive-6.0.5/TikTokLive/proto/proto_utils.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    98737 2024-02-04 08:14:43.000000 TikTokLive-6.0.5/TikTokLive/proto/tiktok_proto.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.187739 TikTokLive-6.0.5/TikTokLive.egg-info/
--rw-r--r--   0 isaackogan   (501) staff       (20)    17683 2024-04-10 04:51:42.000000 TikTokLive-6.0.5/TikTokLive.egg-info/PKG-INFO
--rw-r--r--   0 isaackogan   (501) staff       (20)     1764 2024-04-10 04:51:42.000000 TikTokLive-6.0.5/TikTokLive.egg-info/SOURCES.txt
--rw-r--r--   0 isaackogan   (501) staff       (20)        1 2024-04-10 04:51:42.000000 TikTokLive-6.0.5/TikTokLive.egg-info/dependency_links.txt
--rw-r--r--   0 isaackogan   (501) staff       (20)      162 2024-04-10 04:51:42.000000 TikTokLive-6.0.5/TikTokLive.egg-info/requires.txt
--rw-r--r--   0 isaackogan   (501) staff       (20)       28 2024-04-10 04:51:42.000000 TikTokLive-6.0.5/TikTokLive.egg-info/top_level.txt
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.183157 TikTokLive-6.0.5/TikTokLiveLegacy/
--rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/__init__.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.185074 TikTokLive-6.0.5/TikTokLiveLegacy/client/
--rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    22144 2024-03-22 00:18:26.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/base.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     7425 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/client.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     2032 2024-02-17 18:22:43.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/config.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    10349 2024-02-22 06:31:30.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/httpx.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     4736 2024-02-22 06:29:21.000000 TikTokLive-6.0.5/TikTokLiveLegacy/client/wsclient.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.186145 TikTokLive-6.0.5/TikTokLiveLegacy/proto/
--rw-r--r--   0 isaackogan   (501) staff       (20)       50 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/proto/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    46393 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/proto/tiktok_schema_pb2.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     3003 2024-02-22 06:29:21.000000 TikTokLive-6.0.5/TikTokLiveLegacy/proto/utilities.py
-drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-04-10 04:51:42.187389 TikTokLive-6.0.5/TikTokLiveLegacy/types/
--rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/types/__init__.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     3362 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/types/errors.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    16175 2024-02-22 06:29:21.000000 TikTokLive-6.0.5/TikTokLiveLegacy/types/events.py
--rw-r--r--   0 isaackogan   (501) staff       (20)    15122 2024-02-22 06:29:21.000000 TikTokLive-6.0.5/TikTokLiveLegacy/types/objects.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1023 2023-06-16 17:56:57.000000 TikTokLive-6.0.5/TikTokLiveLegacy/types/utilities.py
--rw-r--r--   0 isaackogan   (501) staff       (20)     1350 2024-02-24 20:23:34.000000 TikTokLive-6.0.5/TikTokLiveLegacy/utilities.py
--rw-r--r--   0 isaackogan   (501) staff       (20)       38 2024-04-10 04:51:42.188403 TikTokLive-6.0.5/setup.cfg
--rw-r--r--   0 isaackogan   (501) staff       (20)     1937 2024-04-10 04:51:36.000000 TikTokLive-6.0.5/setup.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.320767 tiktoklive-6.0.6/
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1068 2024-02-22 06:19:06.000000 tiktoklive-6.0.6/LICENSE
+-rw-r--r--   0 isaackogan   (501) staff       (20)    17521 2024-05-02 19:49:22.320473 tiktoklive-6.0.6/PKG-INFO
+-rw-r--r--   0 isaackogan   (501) staff       (20)    16389 2024-04-10 21:18:05.000000 tiktoklive-6.0.6/README.md
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.304362 tiktoklive-6.0.6/TikTokLive/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       43 2024-02-22 03:47:28.000000 tiktoklive-6.0.6/TikTokLive/__init__.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.306430 tiktoklive-6.0.6/TikTokLive/client/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-11 08:02:27.000000 tiktoklive-6.0.6/TikTokLive/client/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    16401 2024-04-10 00:48:55.000000 tiktoklive-6.0.6/TikTokLive/client/client.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      659 2024-04-08 20:08:19.000000 tiktoklive-6.0.6/TikTokLive/client/errors.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     4209 2024-02-24 20:23:34.000000 tiktoklive-6.0.6/TikTokLive/client/logger.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.307350 tiktoklive-6.0.6/TikTokLive/client/web/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-12-20 23:59:08.000000 tiktoklive-6.0.6/TikTokLive/client/web/__init__.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.309891 tiktoklive-6.0.6/TikTokLive/client/web/routes/
+-rw-r--r--   0 isaackogan   (501) staff       (20)      303 2024-04-08 19:26:24.000000 tiktoklive-6.0.6/TikTokLive/client/web/routes/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      925 2024-05-01 20:32:50.000000 tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_gift_list.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      619 2024-02-24 20:23:34.000000 tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_image.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2355 2024-04-08 19:57:30.000000 tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_is_live.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2803 2024-04-08 19:57:30.000000 tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_room_id_api.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1889 2024-04-08 19:26:01.000000 tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_room_id_html.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1424 2024-04-08 19:50:54.000000 tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_room_info.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     5209 2024-04-03 17:28:04.000000 tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_sign.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     6065 2024-02-24 20:23:34.000000 tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_video.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     4918 2024-04-08 19:22:45.000000 tiktoklive-6.0.6/TikTokLive/client/web/web_base.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1532 2024-04-08 19:57:30.000000 tiktoklive-6.0.6/TikTokLive/client/web/web_client.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2607 2024-02-24 20:23:34.000000 tiktoklive-6.0.6/TikTokLive/client/web/web_settings.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.310252 tiktoklive-6.0.6/TikTokLive/client/ws/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2024-02-03 19:50:49.000000 tiktoklive-6.0.6/TikTokLive/client/ws/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     7748 2024-03-22 01:02:42.000000 tiktoklive-6.0.6/TikTokLive/client/ws/ws_client.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.311257 tiktoklive-6.0.6/TikTokLive/events/
+-rw-r--r--   0 isaackogan   (501) staff       (20)      567 2024-02-22 06:22:04.000000 tiktoklive-6.0.6/TikTokLive/events/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)      439 2024-02-24 20:23:34.000000 tiktoklive-6.0.6/TikTokLive/events/base_event.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2316 2024-02-24 20:23:34.000000 tiktoklive-6.0.6/TikTokLive/events/custom_events.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     7482 2024-05-01 20:57:21.000000 tiktoklive-6.0.6/TikTokLive/events/proto_events.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.312490 tiktoklive-6.0.6/TikTokLive/proto/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       55 2024-02-04 07:15:00.000000 tiktoklive-6.0.6/TikTokLive/proto/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     5166 2024-04-10 21:17:48.000000 tiktoklive-6.0.6/TikTokLive/proto/custom_proto.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2603 2024-04-10 04:24:02.000000 tiktoklive-6.0.6/TikTokLive/proto/proto_utils.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    98737 2024-02-04 08:14:43.000000 tiktoklive-6.0.6/TikTokLive/proto/tiktok_proto.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.320179 tiktoklive-6.0.6/TikTokLive.egg-info/
+-rw-r--r--   0 isaackogan   (501) staff       (20)    17521 2024-05-02 19:49:22.000000 tiktoklive-6.0.6/TikTokLive.egg-info/PKG-INFO
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1764 2024-05-02 19:49:22.000000 tiktoklive-6.0.6/TikTokLive.egg-info/SOURCES.txt
+-rw-r--r--   0 isaackogan   (501) staff       (20)        1 2024-05-02 19:49:22.000000 tiktoklive-6.0.6/TikTokLive.egg-info/dependency_links.txt
+-rw-r--r--   0 isaackogan   (501) staff       (20)      162 2024-05-02 19:49:22.000000 tiktoklive-6.0.6/TikTokLive.egg-info/requires.txt
+-rw-r--r--   0 isaackogan   (501) staff       (20)       28 2024-05-02 19:49:22.000000 tiktoklive-6.0.6/TikTokLive.egg-info/top_level.txt
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.315117 tiktoklive-6.0.6/TikTokLiveLegacy/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 tiktoklive-6.0.6/TikTokLiveLegacy/__init__.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.317518 tiktoklive-6.0.6/TikTokLiveLegacy/client/
+-rw-r--r--   0 isaackogan   (501) staff       (20)        0 2023-06-16 17:56:57.000000 tiktoklive-6.0.6/TikTokLiveLegacy/client/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    22144 2024-03-22 00:18:26.000000 tiktoklive-6.0.6/TikTokLiveLegacy/client/base.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     7425 2023-06-16 17:56:57.000000 tiktoklive-6.0.6/TikTokLiveLegacy/client/client.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     2032 2024-02-17 18:22:43.000000 tiktoklive-6.0.6/TikTokLiveLegacy/client/config.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    10349 2024-02-22 06:31:30.000000 tiktoklive-6.0.6/TikTokLiveLegacy/client/httpx.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     4736 2024-02-22 06:29:21.000000 tiktoklive-6.0.6/TikTokLiveLegacy/client/wsclient.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.318446 tiktoklive-6.0.6/TikTokLiveLegacy/proto/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       50 2023-06-16 17:56:57.000000 tiktoklive-6.0.6/TikTokLiveLegacy/proto/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    46393 2023-06-16 17:56:57.000000 tiktoklive-6.0.6/TikTokLiveLegacy/proto/tiktok_schema_pb2.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     3003 2024-02-22 06:29:21.000000 tiktoklive-6.0.6/TikTokLiveLegacy/proto/utilities.py
+drwxr-xr-x   0 isaackogan   (501) staff       (20)        0 2024-05-02 19:49:22.319825 tiktoklive-6.0.6/TikTokLiveLegacy/types/
+-rw-r--r--   0 isaackogan   (501) staff       (20)       44 2023-06-16 17:56:57.000000 tiktoklive-6.0.6/TikTokLiveLegacy/types/__init__.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     3362 2023-06-16 17:56:57.000000 tiktoklive-6.0.6/TikTokLiveLegacy/types/errors.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    16175 2024-02-22 06:29:21.000000 tiktoklive-6.0.6/TikTokLiveLegacy/types/events.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)    15122 2024-02-22 06:29:21.000000 tiktoklive-6.0.6/TikTokLiveLegacy/types/objects.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1023 2023-06-16 17:56:57.000000 tiktoklive-6.0.6/TikTokLiveLegacy/types/utilities.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1350 2024-02-24 20:23:34.000000 tiktoklive-6.0.6/TikTokLiveLegacy/utilities.py
+-rw-r--r--   0 isaackogan   (501) staff       (20)       38 2024-05-02 19:49:22.320809 tiktoklive-6.0.6/setup.cfg
+-rw-r--r--   0 isaackogan   (501) staff       (20)     1937 2024-05-02 19:49:15.000000 tiktoklive-6.0.6/setup.py
```

### Comparing `TikTokLive-6.0.5/LICENSE` & `tiktoklive-6.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/PKG-INFO` & `tiktoklive-6.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TikTokLive
-Version: 6.0.5
+Version: 6.0.6
 Summary: TikTok Live Python Client
 Home-page: https://github.com/isaackogan/TikTokLive
-Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.5
+Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.6
 Author: Isaac Kogan
 Author-email: info@isaackogan.com
 License: MIT
 Keywords: tiktok,tiktok live,python3,api,unofficial
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -48,17 +48,14 @@
 
 Join the [TikTokLive discord](https://discord.gg/e2XwPNTBBr) and visit
 the [`#py-support`](https://discord.gg/uja6SajDxd)
 channel for questions, contributions and ideas.
 
 ### Enterprise Access
 
-- Tokens to scrape ANY TikTok URL (i.e. fetch profiles,  videos, comments, etc.)
-- Increased TikTok LIVE rate limits (i.e. ability to 1000s of clients per hour)
-
 <div align="left">
     <a href="https://eulerstream.com" target="_blank">
         <div>
             <b>Eulerstream</b> offers paid plans for enterprises for increased TikTokLive access & TikTok API tokens for data collection
         </div>
         <br/>
         <img src="https://github.com/isaackogan/TikTokLive/assets/65869106/b56cef89-5d87-4f2f-ac3e-0685af21b28d)" width="100" alt="Eulerstream">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: TikTokLive Version: 6.0.5 Summary: TikTok Live
+Metadata-Version: 2.1 Name: TikTokLive Version: 6.0.6 Summary: TikTok Live
 Python Client Home-page: https://github.com/isaackogan/TikTokLive Download-URL:
-https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.5 Author: Isaac
+https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.6 Author: Isaac
 Kogan Author-email: info@isaackogan.com License: MIT Keywords: tiktok,tiktok
 live,python3,api,unofficial Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Build Tools Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -23,17 +23,15 @@
 library designed to connect to [TikTok LIVE](https://tiktok.com/live) and
 receive realtime events such as comments, gifts, and likes through a websocket
 connection to TikTok's internal Webcast service. This library allows you to
 connect directly to TikTok with just a username (`@unique_id`). No credentials
 are required to use TikTokLive. Join the [TikTokLive discord](https://
 discord.gg/e2XwPNTBBr) and visit the [`#py-support`](https://discord.gg/
 uja6SajDxd) channel for questions, contributions and ideas. ### Enterprise
-Access - Tokens to scrape ANY TikTok URL (i.e. fetch profiles, videos,
-comments, etc.) - Increased TikTok LIVE rate limits (i.e. ability to 1000s of
-clients per hour)
+Access
 _EE_uu_ll_ee_rr_ss_tt_rr_ee_aa_mm_ _o_f_f_e_r_s_ _p_a_i_d_ _p_l_a_n_s_ _f_o_r_ _e_n_t_e_r_p_r_i_s_e_s_ _f_o_r_ _i_n_c_r_e_a_s_e_d_ _T_i_k_T_o_k_L_i_v_e_ _a_c_c_e_s_s_ _&
 _T_i_k_T_o_k_ _A_P_I_ _t_o_k_e_n_s_ _f_o_r_ _d_a_t_a_ _c_o_l_l_e_c_t_i_o_n
 
 _[_E_u_l_e_r_s_t_r_e_a_m_]
 ### Consider Donating <3 I'm a 2nd-year Biology student in university who likes
 to program for fun. Please consider supporting development through a small
 donation at [https://www.buymeacoffee.com/isaackogan](https://
```

### Comparing `TikTokLive-6.0.5/README.md` & `tiktoklive-6.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 
 Join the [TikTokLive discord](https://discord.gg/e2XwPNTBBr) and visit
 the [`#py-support`](https://discord.gg/uja6SajDxd)
 channel for questions, contributions and ideas.
 
 ### Enterprise Access
 
-- Tokens to scrape ANY TikTok URL (i.e. fetch profiles,  videos, comments, etc.)
-- Increased TikTok LIVE rate limits (i.e. ability to 1000s of clients per hour)
-
 <div align="left">
     <a href="https://eulerstream.com" target="_blank">
         <div>
             <b>Eulerstream</b> offers paid plans for enterprises for increased TikTokLive access & TikTok API tokens for data collection
         </div>
         <br/>
         <img src="https://github.com/isaackogan/TikTokLive/assets/65869106/b56cef89-5d87-4f2f-ac3e-0685af21b28d)" width="100" alt="Eulerstream">
```

### Comparing `TikTokLive-6.0.5/TikTokLive/client/client.py` & `tiktoklive-6.0.6/TikTokLive/client/client.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/errors.py` & `tiktoklive-6.0.6/TikTokLive/client/errors.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/logger.py` & `tiktoklive-6.0.6/TikTokLive/client/logger.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_gift_list.py` & `tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_gift_list.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_image.py` & `tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_image.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_is_live.py` & `tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_is_live.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_id_api.py` & `tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_room_id_api.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_id_html.py` & `tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_room_id_html.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_room_info.py` & `tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_room_info.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_sign.py` & `tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_sign.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/routes/fetch_video.py` & `tiktoklive-6.0.6/TikTokLive/client/web/routes/fetch_video.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/web_base.py` & `tiktoklive-6.0.6/TikTokLive/client/web/web_base.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/web_client.py` & `tiktoklive-6.0.6/TikTokLive/client/web/web_client.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/web/web_settings.py` & `tiktoklive-6.0.6/TikTokLive/client/web/web_settings.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/client/ws/ws_client.py` & `tiktoklive-6.0.6/TikTokLive/client/ws/ws_client.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/events/__init__.py` & `tiktoklive-6.0.6/TikTokLive/events/__init__.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/events/custom_events.py` & `tiktoklive-6.0.6/TikTokLive/events/custom_events.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/events/proto_events.py` & `tiktoklive-6.0.6/TikTokLive/events/proto_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Generated by the TikTokLive compiler.
 # DO NOT EDIT!
 # SERIOUSLY!
 # I MEAN IT!
+from typing import Union
 
 from TikTokLive.proto.tiktok_proto import *
 from TikTokLive.proto.custom_proto import *
 from .base_event import BaseEvent
-from typing import Type, Union, Dict
-from typing import Union
 
 
 class JoinEvent(BaseEvent, WebcastMemberMessage):
     """
     JoinEvent
     """
 
@@ -97,14 +96,29 @@
         """
 
         if not self.gift.streakable:
             return False
 
         return not bool(self.repeat_end)
 
+    @property
+    def value(self) -> Optional[float]:
+        """
+        Get the USD value of a GiftEvent. If the gift is streakable, this will return None until the streak is over
+
+        :return: The value of the gift
+
+        """
+
+        # Prevent double-count by only calculating for non-streaking gifts
+        if self.streaking:
+            return None
+
+        return self.repeat_count * self.gift.diamond_count * 0.005  # 0.005 is the conversion
+
 
 class GoalUpdateEvent(BaseEvent, WebcastGoalUpdateMessage):
     """
     GoalUpdateEvent
 
     """
```

### Comparing `TikTokLive-6.0.5/TikTokLive/proto/custom_proto.py` & `tiktoklive-6.0.6/TikTokLive/proto/custom_proto.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/proto/proto_utils.py` & `tiktoklive-6.0.6/TikTokLive/proto/proto_utils.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive/proto/tiktok_proto.py` & `tiktoklive-6.0.6/TikTokLive/proto/tiktok_proto.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLive.egg-info/PKG-INFO` & `tiktoklive-6.0.6/TikTokLive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TikTokLive
-Version: 6.0.5
+Version: 6.0.6
 Summary: TikTok Live Python Client
 Home-page: https://github.com/isaackogan/TikTokLive
-Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.5
+Download-URL: https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.6
 Author: Isaac Kogan
 Author-email: info@isaackogan.com
 License: MIT
 Keywords: tiktok,tiktok live,python3,api,unofficial
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -48,17 +48,14 @@
 
 Join the [TikTokLive discord](https://discord.gg/e2XwPNTBBr) and visit
 the [`#py-support`](https://discord.gg/uja6SajDxd)
 channel for questions, contributions and ideas.
 
 ### Enterprise Access
 
-- Tokens to scrape ANY TikTok URL (i.e. fetch profiles,  videos, comments, etc.)
-- Increased TikTok LIVE rate limits (i.e. ability to 1000s of clients per hour)
-
 <div align="left">
     <a href="https://eulerstream.com" target="_blank">
         <div>
             <b>Eulerstream</b> offers paid plans for enterprises for increased TikTokLive access & TikTok API tokens for data collection
         </div>
         <br/>
         <img src="https://github.com/isaackogan/TikTokLive/assets/65869106/b56cef89-5d87-4f2f-ac3e-0685af21b28d)" width="100" alt="Eulerstream">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: TikTokLive Version: 6.0.5 Summary: TikTok Live
+Metadata-Version: 2.1 Name: TikTokLive Version: 6.0.6 Summary: TikTok Live
 Python Client Home-page: https://github.com/isaackogan/TikTokLive Download-URL:
-https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.5 Author: Isaac
+https://github.com/isaackogan/TikTokLive/releases/tag/v6.0.6 Author: Isaac
 Kogan Author-email: info@isaackogan.com License: MIT Keywords: tiktok,tiktok
 live,python3,api,unofficial Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Build Tools Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -23,17 +23,15 @@
 library designed to connect to [TikTok LIVE](https://tiktok.com/live) and
 receive realtime events such as comments, gifts, and likes through a websocket
 connection to TikTok's internal Webcast service. This library allows you to
 connect directly to TikTok with just a username (`@unique_id`). No credentials
 are required to use TikTokLive. Join the [TikTokLive discord](https://
 discord.gg/e2XwPNTBBr) and visit the [`#py-support`](https://discord.gg/
 uja6SajDxd) channel for questions, contributions and ideas. ### Enterprise
-Access - Tokens to scrape ANY TikTok URL (i.e. fetch profiles, videos,
-comments, etc.) - Increased TikTok LIVE rate limits (i.e. ability to 1000s of
-clients per hour)
+Access
 _EE_uu_ll_ee_rr_ss_tt_rr_ee_aa_mm_ _o_f_f_e_r_s_ _p_a_i_d_ _p_l_a_n_s_ _f_o_r_ _e_n_t_e_r_p_r_i_s_e_s_ _f_o_r_ _i_n_c_r_e_a_s_e_d_ _T_i_k_T_o_k_L_i_v_e_ _a_c_c_e_s_s_ _&
 _T_i_k_T_o_k_ _A_P_I_ _t_o_k_e_n_s_ _f_o_r_ _d_a_t_a_ _c_o_l_l_e_c_t_i_o_n
 
 _[_E_u_l_e_r_s_t_r_e_a_m_]
 ### Consider Donating <3 I'm a 2nd-year Biology student in university who likes
 to program for fun. Please consider supporting development through a small
 donation at [https://www.buymeacoffee.com/isaackogan](https://
```

### Comparing `TikTokLive-6.0.5/TikTokLive.egg-info/SOURCES.txt` & `tiktoklive-6.0.6/TikTokLive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/client/base.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/client/base.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/client/client.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/client/client.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/client/config.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/client/config.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/client/httpx.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/client/httpx.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/client/wsclient.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/client/wsclient.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/proto/tiktok_schema_pb2.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/proto/tiktok_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/proto/utilities.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/proto/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/types/errors.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/types/errors.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/types/events.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/types/events.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/types/objects.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/types/objects.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/types/utilities.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/types/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/TikTokLiveLegacy/utilities.py` & `tiktoklive-6.0.6/TikTokLiveLegacy/utilities.py`

 * *Files identical despite different names*

### Comparing `TikTokLive-6.0.5/setup.py` & `tiktoklive-6.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # PyPi upload Command
 # rm -r dist ; python setup.py sdist ; python -m twine upload dist/*
 
 manifest: dict = {
     "name": "TikTokLive",
     "license": "MIT",
     "author": "Isaac Kogan",
-    "version": "6.0.5",
+    "version": "6.0.6",
     "email": "info@isaackogan.com"
 }
 
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
```

