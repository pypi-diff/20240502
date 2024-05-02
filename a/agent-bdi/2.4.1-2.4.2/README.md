# Comparing `tmp/agent-bdi-2.4.1.tar.gz` & `tmp/agent-bdi-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent-bdi-2.4.1.tar", last modified: Sat Apr 27 18:04:20 2024, max compression
+gzip compressed data, was "agent-bdi-2.4.2.tar", last modified: Thu May  2 07:23:23 2024, max compression
```

## Comparing `agent-bdi-2.4.1.tar` & `agent-bdi-2.4.2.tar`

### file list

```diff
@@ -1,52 +1,84 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.592495 agent-bdi-2.4.1/
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/LICENSE.md
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3202 2024-04-27 18:04:20.591492 agent-bdi-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 18:04:20.592495 agent-bdi-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-04-27 18:03:56.000000 agent-bdi-2.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.540646 agent-bdi-2.4.1/src/
--rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/__init__.py
--rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/abdi_config.py
-drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.555645 agent-bdi-2.4.1/src/agent_bdi.egg-info/
--rw-rw-rw-   0        0        0     3202 2024-04-27 18:04:20.000000 agent-bdi-2.4.1/src/agent_bdi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-04-27 18:04:20.000000 agent-bdi-2.4.1/src/agent_bdi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 18:04:20.000000 agent-bdi-2.4.1/src/agent_bdi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-27 18:04:20.000000 agent-bdi-2.4.1/src/agent_bdi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.568148 agent-bdi-2.4.1/src/broker/
--rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.4.1/src/broker/__init__.py
--rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.4.1/src/broker/broker_maker.py
--rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/broker/empty_broker.py
--rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.4.1/src/broker/message_broker.py
--rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.4.1/src/broker/mqtt_broker.py
--rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.4.1/src/broker/notifier.py
--rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/broker/redis_broker.py
--rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/broker/ros_broker.py
--rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.4.1/src/broker/ros_noetic_broker.py
-drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.572152 agent-bdi-2.4.1/src/core/
--rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.4.1/src/core/Agent.py
--rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/core/Belief.py
--rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/core/Desire.py
--rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/core/Intention.py
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.579152 agent-bdi-2.4.1/src/holon/
--rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/holon/Blackboard.py
--rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.4.1/src/holon/Heart.py
--rw-rw-rw-   0        0        0     9850 2024-04-27 15:00:13.000000 agent-bdi-2.4.1/src/holon/HolonicAgent.py
--rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/holon/HolonicDesire.py
--rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.4.1/src/holon/HolonicIntention.py
--rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.4.1/src/holon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.585478 agent-bdi-2.4.1/src/holon/logistics/
--rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.4.1/src/holon/logistics/__init__.py
--rw-rw-rw-   0        0        0      722 2024-04-27 17:02:10.000000 agent-bdi-2.4.1/src/holon/logistics/base_logistic.py
--rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.4.1/src/holon/logistics/broker_logistic.py
--rw-rw-rw-   0        0        0     5299 2024-02-26 10:20:43.000000 agent-bdi-2.4.1/src/holon/logistics/loading_coordinator.py
--rw-rw-rw-   0        0        0     6333 2024-04-04 18:40:47.000000 agent-bdi-2.4.1/src/holon/logistics/payload_wrapper.py
--rw-rw-rw-   0        0        0     3709 2024-04-17 17:18:06.000000 agent-bdi-2.4.1/src/holon/logistics/request_logistic.py
--rw-rw-rw-   0        0        0     3312 2024-04-27 17:02:22.000000 agent-bdi-2.4.1/src/holon/logistics/response_logistic.py
--rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.4.1/src/holon/payload.py
-drwxrwxrwx   0        0        0        0 2024-04-27 18:04:20.590493 agent-bdi-2.4.1/tests/
--rw-rw-rw-   0        0        0      404 2024-04-27 15:27:38.000000 agent-bdi-2.4.1/tests/test01.py
--rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.4.1/tests/test_loadingbal.py
--rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.4.1/tests/test_request.py
--rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.4.1/tests/test_send.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.710671 agent-bdi-2.4.2/
+-rw-r--r--   0 xumingfang   (501) staff       (20)     1943 2023-10-09 06:47:42.000000 agent-bdi-2.4.2/.gitignore
+-rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:56:07.000000 agent-bdi-2.4.2/CHANGES.md
+-rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:55:55.000000 agent-bdi-2.4.2/LICENSE.md
+-rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:56:20.000000 agent-bdi-2.4.2/MANIFEST.in
+-rw-r--r--   0 xumingfang   (501) staff       (20)     3149 2024-05-02 07:23:23.710427 agent-bdi-2.4.2/PKG-INFO
+-rw-r--r--   0 xumingfang   (501) staff       (20)     2612 2023-01-10 11:54:29.000000 agent-bdi-2.4.2/README.md
+-rw-r--r--   0 xumingfang   (501) staff       (20)       60 2023-01-10 18:24:03.000000 agent-bdi-2.4.2/agent-bdi.code-workspace
+-rw-r--r--   0 xumingfang   (501) staff       (20)     1364 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/requirements.txt
+-rw-r--r--   0 xumingfang   (501) staff       (20)       38 2024-05-02 07:23:23.710726 agent-bdi-2.4.2/setup.cfg
+-rw-r--r--   0 xumingfang   (501) staff       (20)      860 2024-05-02 07:22:37.000000 agent-bdi-2.4.2/setup.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.698594 agent-bdi-2.4.2/src/
+-rw-r--r--   0 xumingfang   (501) staff       (20)        0 2024-01-04 05:54:31.000000 agent-bdi-2.4.2/src/__init__.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.699696 agent-bdi-2.4.2/src/_bak/
+-rw-r--r--   0 xumingfang   (501) staff       (20)     1114 2023-10-09 06:48:00.000000 agent-bdi-2.4.2/src/_bak/helper-20231009.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     4469 2024-02-25 08:13:49.000000 agent-bdi-2.4.2/src/_bak/loading_coordinator-20240225.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     3618 2024-05-01 17:08:04.000000 agent-bdi-2.4.2/src/_bak/request_logistic-20240502.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     3232 2024-05-01 17:08:04.000000 agent-bdi-2.4.2/src/_bak/response_logistic-20240502.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      627 2024-01-04 05:54:31.000000 agent-bdi-2.4.2/src/abdi_config.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.700405 agent-bdi-2.4.2/src/agent_bdi.egg-info/
+-rw-r--r--   0 xumingfang   (501) staff       (20)     3149 2024-05-02 07:23:23.000000 agent-bdi-2.4.2/src/agent_bdi.egg-info/PKG-INFO
+-rw-r--r--   0 xumingfang   (501) staff       (20)     1804 2024-05-02 07:23:23.000000 agent-bdi-2.4.2/src/agent_bdi.egg-info/SOURCES.txt
+-rw-r--r--   0 xumingfang   (501) staff       (20)        1 2024-05-02 07:23:23.000000 agent-bdi-2.4.2/src/agent_bdi.egg-info/dependency_links.txt
+-rw-r--r--   0 xumingfang   (501) staff       (20)       44 2024-05-02 07:23:23.000000 agent-bdi-2.4.2/src/agent_bdi.egg-info/top_level.txt
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.701668 agent-bdi-2.4.2/src/broker/
+-rw-r--r--   0 xumingfang   (501) staff       (20)      126 2023-10-09 02:21:29.000000 agent-bdi-2.4.2/src/broker/__init__.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      941 2023-11-01 06:52:28.000000 agent-bdi-2.4.2/src/broker/broker_maker.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      906 2024-01-04 05:54:31.000000 agent-bdi-2.4.2/src/broker/empty_broker.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      618 2023-11-01 06:52:28.000000 agent-bdi-2.4.2/src/broker/message_broker.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     2116 2024-01-04 05:54:31.000000 agent-bdi-2.4.2/src/broker/mqtt_broker.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      366 2023-11-01 07:34:22.000000 agent-bdi-2.4.2/src/broker/notifier.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      866 2024-01-04 05:54:31.000000 agent-bdi-2.4.2/src/broker/redis_broker.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      860 2024-01-04 05:54:31.000000 agent-bdi-2.4.2/src/broker/ros_broker.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     2570 2024-01-04 05:54:31.000000 agent-bdi-2.4.2/src/broker/ros_noetic_broker.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.702685 agent-bdi-2.4.2/src/core/
+-rw-r--r--   0 xumingfang   (501) staff       (20)      302 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/src/core/Agent.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)       56 2023-01-10 11:54:29.000000 agent-bdi-2.4.2/src/core/Belief.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)       50 2023-01-10 11:54:29.000000 agent-bdi-2.4.2/src/core/Desire.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)       53 2023-01-10 11:54:29.000000 agent-bdi-2.4.2/src/core/Intention.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:54:43.000000 agent-bdi-2.4.2/src/core/__init__.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.703785 agent-bdi-2.4.2/src/holon/
+-rw-r--r--   0 xumingfang   (501) staff       (20)      111 2023-01-10 11:54:29.000000 agent-bdi-2.4.2/src/holon/Blackboard.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      436 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/src/holon/Heart.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     9531 2024-05-01 18:44:19.000000 agent-bdi-2.4.2/src/holon/HolonicAgent.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)       69 2023-01-10 11:54:29.000000 agent-bdi-2.4.2/src/holon/HolonicDesire.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)       81 2023-01-10 11:54:29.000000 agent-bdi-2.4.2/src/holon/HolonicIntention.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-10-09 02:21:29.000000 agent-bdi-2.4.2/src/holon/__init__.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.705379 agent-bdi-2.4.2/src/holon/logistics/
+-rw-r--r--   0 xumingfang   (501) staff       (20)        0 2024-02-12 08:17:17.000000 agent-bdi-2.4.2/src/holon/logistics/__init__.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      688 2024-04-29 17:47:01.000000 agent-bdi-2.4.2/src/holon/logistics/base_logistic.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      335 2024-02-12 08:10:44.000000 agent-bdi-2.4.2/src/holon/logistics/broker_logistic.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     5145 2024-02-29 06:15:18.000000 agent-bdi-2.4.2/src/holon/logistics/loading_coordinator.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     6588 2024-05-01 21:14:17.000000 agent-bdi-2.4.2/src/holon/logistics/payload_wrapper.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     3294 2024-05-01 21:18:24.000000 agent-bdi-2.4.2/src/holon/logistics/request_logistic.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     4904 2024-05-01 23:04:22.000000 agent-bdi-2.4.2/src/holon/logistics/response_logistic.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)       76 2024-01-14 06:25:33.000000 agent-bdi-2.4.2/src/holon/payload.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.706185 agent-bdi-2.4.2/tests/
+-rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:55:02.000000 agent-bdi-2.4.2/tests/__init__.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.706627 agent-bdi-2.4.2/tests/guide/
+-rw-r--r--   0 xumingfang   (501) staff       (20)     2112 2024-01-04 05:54:31.000000 agent-bdi-2.4.2/tests/guide/__init__.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.707242 agent-bdi-2.4.2/tests/guide/dialog/
+-rw-r--r--   0 xumingfang   (501) staff       (20)     3009 2024-01-04 05:54:31.000000 agent-bdi-2.4.2/tests/guide/dialog/AudioInput.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      137 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/tests/guide/dialog/AudioOutput.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.707528 agent-bdi-2.4.2/tests/guide/hearing/
+-rw-r--r--   0 xumingfang   (501) staff       (20)     7519 2024-01-04 05:54:31.000000 agent-bdi-2.4.2/tests/guide/hearing/Microphone.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.707991 agent-bdi-2.4.2/tests/guide/navi/
+-rw-r--r--   0 xumingfang   (501) staff       (20)      179 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/tests/guide/navi/RouteFind.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      144 2023-06-05 10:21:03.000000 agent-bdi-2.4.2/tests/guide/navi/VisualInput.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.708697 agent-bdi-2.4.2/tests/guide/navi/walk/
+-rw-r--r--   0 xumingfang   (501) staff       (20)      140 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/tests/guide/navi/walk/KanbanDetect.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      138 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/tests/guide/navi/walk/RoadDetect.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      610 2023-06-05 16:50:06.000000 agent-bdi-2.4.2/tests/guide/navi/walk/WalkGuide.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      532 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/tests/guide/start.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.709318 agent-bdi-2.4.2/tests/guide/visual/
+-rw-r--r--   0 xumingfang   (501) staff       (20)      132 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/tests/guide/visual/Camera.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      144 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/tests/guide/visual/ImagePreprocessing.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      324 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/tests/guide/visual/Visual.py
+drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2024-05-02 07:23:23.709994 agent-bdi-2.4.2/tests/guide/voice/
+-rw-r--r--   0 xumingfang   (501) staff       (20)      869 2023-07-06 19:38:24.000000 agent-bdi-2.4.2/tests/guide/voice/Speaker.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      140 2023-06-05 08:29:29.000000 agent-bdi-2.4.2/tests/guide/voice/ToneProcessing.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)      324 2023-07-03 17:04:36.000000 agent-bdi-2.4.2/tests/guide/voice/Voice.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     1773 2024-02-17 07:42:25.000000 agent-bdi-2.4.2/tests/test_loadingbal.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     2234 2024-01-14 06:25:33.000000 agent-bdi-2.4.2/tests/test_request.py
+-rw-r--r--   0 xumingfang   (501) staff       (20)     2654 2024-01-14 06:25:33.000000 agent-bdi-2.4.2/tests/test_send.py
```

### Comparing `agent-bdi-2.4.1/PKG-INFO` & `agent-bdi-2.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-Metadata-Version: 2.1
-Name: agent-bdi
-Version: 2.4.1
-Summary: Agent BDI framework
-Home-page: https://github.com/mfshiu/abdi.git
-Author: Ming Fang Shiu
-Author-email: avatar.xu@gmail.com
-Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Physiologically Inspired Framework for Complex System Integration
-
-
-## Introduction
-In this study, inspired by the physiological operation of the human body, an efficient and resilient software framework was developed to aid in the integration of mature AI technologies, allowing them to coordinate with one another to accomplish more advanced goals. A navigation system for the visually impaired was then developed to validate the framework, with promising experimental results. This framework can be applied to other types of AI systems.
-
-
-## Instruction
-1. Install the required packages.
-````
-pip install -r requirements.txt
-````
-2. Create config.py, rewite the MQTT settings. 
-````
-cp config.sample.py config.py
-````
-3. Start the framework.
-````
-python start.py
-````
-
-
-## Class Diagram
-The class diagram of the integration of agents and coordination. HolonicAgent represents the core, and HeadAgents and BodyAgents represent the collection of head agents and subagents, respectively. MQTT is the fundamental communication protocol for agents in the global circulation system, and MqttClient is a private member of HolonicAgent, which allows the agent to have built-in MQTT connection and reception capabilities.
-
-All agents inherit from HolonicAgent to form a hierarchical structure, and they use the DDS to achieve neural message transmission depending on their specific behavior. Each super-agent is a DDS domain that publishes or subscribes to related topics with the required QoS, such as the DEADLINE policy to confirm the date of the data or the TRANSPORT_PRIORITY policy to define the transmission priority order, in order to achieve the purpose of a specific agent.
-<figure>
-    <img src="https://i.imgur.com/9vIa7JH.png" height=500>
-    <figcaption>Class diagram of integration</figcaption>
-</figure>
-
-
-## Sequence Diagram
-According to the sequence diagram depicted in below, the DDS and MQTT serve to transmit messages for the agents. Action 1 entails generating an independent process immediately after the root agent is initialized. Action 2 entails subscribing to or publishing relevant topics within the QoS constraints. Action 3 entails recursively calling all the subagents to initiate the action. The agent main action is performed in a separate process of Action 2 until it is notified of its termination. Finally, Action 4 entails generating a global broadcast with MQTT, with a system termination notification serving as an example in this study.
-<figure>
-    <img src="https://i.imgur.com/6lA3w1X.png" height=500>
-    <figcaption>Sequence Diagram of Integration</figcaption>
-</figure>
+Metadata-Version: 2.1
+Name: agent-bdi
+Version: 2.4.2
+Summary: Agent BDI framework
+Home-page: https://github.com/mfshiu/abdi.git
+Author: Ming Fang Shiu
+Author-email: avatar.xu@gmail.com
+Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Physiologically Inspired Framework for Complex System Integration
+
+
+## Introduction
+In this study, inspired by the physiological operation of the human body, an efficient and resilient software framework was developed to aid in the integration of mature AI technologies, allowing them to coordinate with one another to accomplish more advanced goals. A navigation system for the visually impaired was then developed to validate the framework, with promising experimental results. This framework can be applied to other types of AI systems.
+
+
+## Instruction
+1. Install the required packages.
+````
+pip install -r requirements.txt
+````
+2. Create config.py, rewite the MQTT settings. 
+````
+cp config.sample.py config.py
+````
+3. Start the framework.
+````
+python start.py
+````
+
+
+## Class Diagram
+The class diagram of the integration of agents and coordination. HolonicAgent represents the core, and HeadAgents and BodyAgents represent the collection of head agents and subagents, respectively. MQTT is the fundamental communication protocol for agents in the global circulation system, and MqttClient is a private member of HolonicAgent, which allows the agent to have built-in MQTT connection and reception capabilities.
+
+All agents inherit from HolonicAgent to form a hierarchical structure, and they use the DDS to achieve neural message transmission depending on their specific behavior. Each super-agent is a DDS domain that publishes or subscribes to related topics with the required QoS, such as the DEADLINE policy to confirm the date of the data or the TRANSPORT_PRIORITY policy to define the transmission priority order, in order to achieve the purpose of a specific agent.
+<figure>
+    <img src="https://i.imgur.com/9vIa7JH.png" height=500>
+    <figcaption>Class diagram of integration</figcaption>
+</figure>
+
+
+## Sequence Diagram
+According to the sequence diagram depicted in below, the DDS and MQTT serve to transmit messages for the agents. Action 1 entails generating an independent process immediately after the root agent is initialized. Action 2 entails subscribing to or publishing relevant topics within the QoS constraints. Action 3 entails recursively calling all the subagents to initiate the action. The agent main action is performed in a separate process of Action 2 until it is notified of its termination. Finally, Action 4 entails generating a global broadcast with MQTT, with a system termination notification serving as an example in this study.
+<figure>
+    <img src="https://i.imgur.com/6lA3w1X.png" height=500>
+    <figcaption>Sequence Diagram of Integration</figcaption>
+</figure>
```

### Comparing `agent-bdi-2.4.1/README.md` & `agent-bdi-2.4.2/src/agent_bdi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,53 @@
-# Physiologically Inspired Framework for Complex System Integration
-
-
-## Introduction
-In this study, inspired by the physiological operation of the human body, an efficient and resilient software framework was developed to aid in the integration of mature AI technologies, allowing them to coordinate with one another to accomplish more advanced goals. A navigation system for the visually impaired was then developed to validate the framework, with promising experimental results. This framework can be applied to other types of AI systems.
-
-
-## Instruction
-1. Install the required packages.
-````
-pip install -r requirements.txt
-````
-2. Create config.py, rewite the MQTT settings. 
-````
-cp config.sample.py config.py
-````
-3. Start the framework.
-````
-python start.py
-````
-
-
-## Class Diagram
-The class diagram of the integration of agents and coordination. HolonicAgent represents the core, and HeadAgents and BodyAgents represent the collection of head agents and subagents, respectively. MQTT is the fundamental communication protocol for agents in the global circulation system, and MqttClient is a private member of HolonicAgent, which allows the agent to have built-in MQTT connection and reception capabilities.
-
-All agents inherit from HolonicAgent to form a hierarchical structure, and they use the DDS to achieve neural message transmission depending on their specific behavior. Each super-agent is a DDS domain that publishes or subscribes to related topics with the required QoS, such as the DEADLINE policy to confirm the date of the data or the TRANSPORT_PRIORITY policy to define the transmission priority order, in order to achieve the purpose of a specific agent.
-<figure>
-    <img src="https://i.imgur.com/9vIa7JH.png" height=500>
-    <figcaption>Class diagram of integration</figcaption>
-</figure>
-
-
-## Sequence Diagram
-According to the sequence diagram depicted in below, the DDS and MQTT serve to transmit messages for the agents. Action 1 entails generating an independent process immediately after the root agent is initialized. Action 2 entails subscribing to or publishing relevant topics within the QoS constraints. Action 3 entails recursively calling all the subagents to initiate the action. The agent main action is performed in a separate process of Action 2 until it is notified of its termination. Finally, Action 4 entails generating a global broadcast with MQTT, with a system termination notification serving as an example in this study.
-<figure>
-    <img src="https://i.imgur.com/6lA3w1X.png" height=500>
-    <figcaption>Sequence Diagram of Integration</figcaption>
-</figure>
+Metadata-Version: 2.1
+Name: agent-bdi
+Version: 2.4.2
+Summary: Agent BDI framework
+Home-page: https://github.com/mfshiu/abdi.git
+Author: Ming Fang Shiu
+Author-email: avatar.xu@gmail.com
+Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Physiologically Inspired Framework for Complex System Integration
+
+
+## Introduction
+In this study, inspired by the physiological operation of the human body, an efficient and resilient software framework was developed to aid in the integration of mature AI technologies, allowing them to coordinate with one another to accomplish more advanced goals. A navigation system for the visually impaired was then developed to validate the framework, with promising experimental results. This framework can be applied to other types of AI systems.
+
+
+## Instruction
+1. Install the required packages.
+````
+pip install -r requirements.txt
+````
+2. Create config.py, rewite the MQTT settings. 
+````
+cp config.sample.py config.py
+````
+3. Start the framework.
+````
+python start.py
+````
+
+
+## Class Diagram
+The class diagram of the integration of agents and coordination. HolonicAgent represents the core, and HeadAgents and BodyAgents represent the collection of head agents and subagents, respectively. MQTT is the fundamental communication protocol for agents in the global circulation system, and MqttClient is a private member of HolonicAgent, which allows the agent to have built-in MQTT connection and reception capabilities.
+
+All agents inherit from HolonicAgent to form a hierarchical structure, and they use the DDS to achieve neural message transmission depending on their specific behavior. Each super-agent is a DDS domain that publishes or subscribes to related topics with the required QoS, such as the DEADLINE policy to confirm the date of the data or the TRANSPORT_PRIORITY policy to define the transmission priority order, in order to achieve the purpose of a specific agent.
+<figure>
+    <img src="https://i.imgur.com/9vIa7JH.png" height=500>
+    <figcaption>Class diagram of integration</figcaption>
+</figure>
+
+
+## Sequence Diagram
+According to the sequence diagram depicted in below, the DDS and MQTT serve to transmit messages for the agents. Action 1 entails generating an independent process immediately after the root agent is initialized. Action 2 entails subscribing to or publishing relevant topics within the QoS constraints. Action 3 entails recursively calling all the subagents to initiate the action. The agent main action is performed in a separate process of Action 2 until it is notified of its termination. Finally, Action 4 entails generating a global broadcast with MQTT, with a system termination notification serving as an example in this study.
+<figure>
+    <img src="https://i.imgur.com/6lA3w1X.png" height=500>
+    <figcaption>Sequence Diagram of Integration</figcaption>
+</figure>
```

### Comparing `agent-bdi-2.4.1/src/abdi_config.py` & `agent-bdi-2.4.2/src/abdi_config.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import logging
-
-from broker import BrokerType
-
-
-LOGGER_NAME = "ABDI"
-
-
-
-class AbdiConfig:
-    def __init__(self, options=None):
-        self.options = options if options else {}
-
-        self.log_level = logging.DEBUG
-        self.log_dir = "./_log"
-        
-        
-    def get_broker_type(self) -> BrokerType:
-        if broker_type := self.get("broker_type"):
-            return BrokerType(broker_type.lower())
-        else:
-            return BrokerType.Empty
-        
-    
-    def get(self, key:str):
-        return self.options.get(key)
-        
-    
-    def set(self, key:str, value):
-        self.options[key] = value
+import logging
+
+from broker import BrokerType
+
+
+LOGGER_NAME = "ABDI"
+
+
+
+class AbdiConfig:
+    def __init__(self, options=None):
+        self.options = options if options else {}
+
+        self.log_level = logging.DEBUG
+        self.log_dir = "./_log"
+        
+        
+    def get_broker_type(self) -> BrokerType:
+        if broker_type := self.get("broker_type"):
+            return BrokerType(broker_type.lower())
+        else:
+            return BrokerType.Empty
+        
+    
+    def get(self, key:str):
+        return self.options.get(key)
+        
+    
+    def set(self, key:str, value):
+        self.options[key] = value
```

### Comparing `agent-bdi-2.4.1/src/agent_bdi.egg-info/PKG-INFO` & `agent-bdi-2.4.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,38 @@
-Metadata-Version: 2.1
-Name: agent-bdi
-Version: 2.4.1
-Summary: Agent BDI framework
-Home-page: https://github.com/mfshiu/abdi.git
-Author: Ming Fang Shiu
-Author-email: avatar.xu@gmail.com
-Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Physiologically Inspired Framework for Complex System Integration
-
-
-## Introduction
-In this study, inspired by the physiological operation of the human body, an efficient and resilient software framework was developed to aid in the integration of mature AI technologies, allowing them to coordinate with one another to accomplish more advanced goals. A navigation system for the visually impaired was then developed to validate the framework, with promising experimental results. This framework can be applied to other types of AI systems.
-
-
-## Instruction
-1. Install the required packages.
-````
-pip install -r requirements.txt
-````
-2. Create config.py, rewite the MQTT settings. 
-````
-cp config.sample.py config.py
-````
-3. Start the framework.
-````
-python start.py
-````
-
-
-## Class Diagram
-The class diagram of the integration of agents and coordination. HolonicAgent represents the core, and HeadAgents and BodyAgents represent the collection of head agents and subagents, respectively. MQTT is the fundamental communication protocol for agents in the global circulation system, and MqttClient is a private member of HolonicAgent, which allows the agent to have built-in MQTT connection and reception capabilities.
-
-All agents inherit from HolonicAgent to form a hierarchical structure, and they use the DDS to achieve neural message transmission depending on their specific behavior. Each super-agent is a DDS domain that publishes or subscribes to related topics with the required QoS, such as the DEADLINE policy to confirm the date of the data or the TRANSPORT_PRIORITY policy to define the transmission priority order, in order to achieve the purpose of a specific agent.
-<figure>
-    <img src="https://i.imgur.com/9vIa7JH.png" height=500>
-    <figcaption>Class diagram of integration</figcaption>
-</figure>
-
-
-## Sequence Diagram
-According to the sequence diagram depicted in below, the DDS and MQTT serve to transmit messages for the agents. Action 1 entails generating an independent process immediately after the root agent is initialized. Action 2 entails subscribing to or publishing relevant topics within the QoS constraints. Action 3 entails recursively calling all the subagents to initiate the action. The agent main action is performed in a separate process of Action 2 until it is notified of its termination. Finally, Action 4 entails generating a global broadcast with MQTT, with a system termination notification serving as an example in this study.
-<figure>
-    <img src="https://i.imgur.com/6lA3w1X.png" height=500>
-    <figcaption>Sequence Diagram of Integration</figcaption>
-</figure>
+# Physiologically Inspired Framework for Complex System Integration
+
+
+## Introduction
+In this study, inspired by the physiological operation of the human body, an efficient and resilient software framework was developed to aid in the integration of mature AI technologies, allowing them to coordinate with one another to accomplish more advanced goals. A navigation system for the visually impaired was then developed to validate the framework, with promising experimental results. This framework can be applied to other types of AI systems.
+
+
+## Instruction
+1. Install the required packages.
+````
+pip install -r requirements.txt
+````
+2. Create config.py, rewite the MQTT settings. 
+````
+cp config.sample.py config.py
+````
+3. Start the framework.
+````
+python start.py
+````
+
+
+## Class Diagram
+The class diagram of the integration of agents and coordination. HolonicAgent represents the core, and HeadAgents and BodyAgents represent the collection of head agents and subagents, respectively. MQTT is the fundamental communication protocol for agents in the global circulation system, and MqttClient is a private member of HolonicAgent, which allows the agent to have built-in MQTT connection and reception capabilities.
+
+All agents inherit from HolonicAgent to form a hierarchical structure, and they use the DDS to achieve neural message transmission depending on their specific behavior. Each super-agent is a DDS domain that publishes or subscribes to related topics with the required QoS, such as the DEADLINE policy to confirm the date of the data or the TRANSPORT_PRIORITY policy to define the transmission priority order, in order to achieve the purpose of a specific agent.
+<figure>
+    <img src="https://i.imgur.com/9vIa7JH.png" height=500>
+    <figcaption>Class diagram of integration</figcaption>
+</figure>
+
+
+## Sequence Diagram
+According to the sequence diagram depicted in below, the DDS and MQTT serve to transmit messages for the agents. Action 1 entails generating an independent process immediately after the root agent is initialized. Action 2 entails subscribing to or publishing relevant topics within the QoS constraints. Action 3 entails recursively calling all the subagents to initiate the action. The agent main action is performed in a separate process of Action 2 until it is notified of its termination. Finally, Action 4 entails generating a global broadcast with MQTT, with a system termination notification serving as an example in this study.
+<figure>
+    <img src="https://i.imgur.com/6lA3w1X.png" height=500>
+    <figcaption>Sequence Diagram of Integration</figcaption>
+</figure>
```

### Comparing `agent-bdi-2.4.1/src/broker/broker_maker.py` & `agent-bdi-2.4.2/src/broker/broker_maker.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from broker import BrokerType
-from broker.empty_broker import EmptyBroker
-from broker.mqtt_broker import MqttBroker
-from broker.redis_broker import RedisBroker
-from broker.ros_broker import RosBroker
-# from broker.ros_noetic_broker import RosNoeticBroker
-from broker.notifier import BrokerNotifier
-
-
-class BrokerMaker():
-    def create_broker(self, broker_type:BrokerType, notifier:BrokerNotifier):
-        if broker_type is BrokerType.Redis:
-            return RedisBroker(notifier)
-        elif broker_type is BrokerType.MQTT:
-            return MqttBroker(notifier)
-        elif broker_type is BrokerType.ROS:
-            return RosBroker(notifier)
-        # elif broker_type is BrokerType.ROS:
-        #     return RosNoeticBroker(notifier)
-        elif broker_type is BrokerType.Empty:
-            return EmptyBroker(notifier)
-        else:
-           raise TypeError(f"Unsupported broker type: {type(broker_type).__name__}.") 
+from broker import BrokerType
+from broker.empty_broker import EmptyBroker
+from broker.mqtt_broker import MqttBroker
+from broker.redis_broker import RedisBroker
+from broker.ros_broker import RosBroker
+# from broker.ros_noetic_broker import RosNoeticBroker
+from broker.notifier import BrokerNotifier
+
+
+class BrokerMaker():
+    def create_broker(self, broker_type:BrokerType, notifier:BrokerNotifier):
+        if broker_type is BrokerType.Redis:
+            return RedisBroker(notifier)
+        elif broker_type is BrokerType.MQTT:
+            return MqttBroker(notifier)
+        elif broker_type is BrokerType.ROS:
+            return RosBroker(notifier)
+        # elif broker_type is BrokerType.ROS:
+        #     return RosNoeticBroker(notifier)
+        elif broker_type is BrokerType.Empty:
+            return EmptyBroker(notifier)
+        else:
+           raise TypeError(f"Unsupported broker type: {type(broker_type).__name__}.")
```

### Comparing `agent-bdi-2.4.1/src/broker/empty_broker.py` & `agent-bdi-2.4.2/src/broker/ros_broker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import logging
-
-from broker.message_broker import MessageBroker
-from broker.notifier import BrokerNotifier
-from abdi_config import LOGGER_NAME
-
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class EmptyBroker(MessageBroker):
-    def __init__(self, notifier:BrokerNotifier):
-        logger.info(f"Initialize...")
-        
-        super().__init__(notifier=notifier)
-
-
-
-    ###################################
-    # Implementation of MessageBroker #
-    ###################################
-    
-    
-    def start(self, options:dict):
-        logger.info(f"Empty broker is starting. options:{options}")
-       
-
-    def stop(self):
-        logger.info(f"Empty broker is stopping...")
-
-
-    def publish(self, topic:str, payload):
-        logger.info(f"topic: {topic}, payload: {payload}")
-        
-    
-    def subscribe(self, topic:str, data_type):
-        logger.info(f"topic: {topic}, data_type: {data_type}")
+import logging
+
+from broker.message_broker import MessageBroker
+from broker.notifier import BrokerNotifier
+from abdi_config import LOGGER_NAME
+
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class RosBroker(MessageBroker):
+    def __init__(self, notifier:BrokerNotifier):
+        logger.info(f"Initialize...")
+        
+        super().__init__(notifier=notifier)
+
+
+
+    ###################################
+    # Implementation of MessageBroker #
+    ###################################
+    
+    
+    def start(self, options:dict):
+        logger.info(f"Ros broker is starting...")
+       
+
+    def stop(self):
+        logger.info(f"Ros broker is stopping...")
+
+
+    def publish(self, topic:str, payload):
+        logger.info(f"topic: {topic}, payload: {payload}")
+        
+    
+    def subscribe(self, topic:str, data_type):
+        logger.info(f"topic: {topic}")
```

### Comparing `agent-bdi-2.4.1/src/broker/message_broker.py` & `agent-bdi-2.4.2/src/broker/message_broker.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from abc import ABC, abstractmethod
-from broker.notifier import BrokerNotifier
-
-
-class MessageBroker(ABC):
-    def __init__(self, notifier:BrokerNotifier):
-        self._notifier = notifier
-        
-    
-    @abstractmethod
-    def start(self, options:dict):
-        """Start the message broker."""
-        
-    
-    @abstractmethod
-    def stop(self):
-        """Stop the message broker."""
-        
-    
-    @abstractmethod
-    def publish(self, topic:str, payload):
-        """Publish the topic."""
-        
-    
-    @abstractmethod
-    def subscribe(self, topic:str, data_type):
-        """Subscribe the topic."""
+from abc import ABC, abstractmethod
+from broker.notifier import BrokerNotifier
+
+
+class MessageBroker(ABC):
+    def __init__(self, notifier:BrokerNotifier):
+        self._notifier = notifier
+        
+    
+    @abstractmethod
+    def start(self, options:dict):
+        """Start the message broker."""
+        
+    
+    @abstractmethod
+    def stop(self):
+        """Stop the message broker."""
+        
+    
+    @abstractmethod
+    def publish(self, topic:str, payload):
+        """Publish the topic."""
+        
+    
+    @abstractmethod
+    def subscribe(self, topic:str, data_type):
+        """Subscribe the topic."""
```

### Comparing `agent-bdi-2.4.1/src/broker/mqtt_broker.py` & `agent-bdi-2.4.2/src/broker/mqtt_broker.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from paho.mqtt.client import Client
-
-from broker.message_broker import MessageBroker
-from broker.notifier import BrokerNotifier
-import logging
-from abdi_config import LOGGER_NAME
-
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class MqttBroker(MessageBroker):
-    def __init__(self, notifier:BrokerNotifier):
-        self._client = Client()
-        self.host = ""
-        self.port = 0
-        self.keepalive = 0
-        
-        super().__init__(notifier=notifier)
-
-
-    def _on_connect(self, client:Client, userdata, flags, rc):
-        logger.info(f"MQTT broker connected. url: {self.host}, port: {self.port}, keepalive: {self.keepalive}")
-        # logger.debug(f"Client: {client}\nuserdata:{userdata}\nflags: {flags}\nrc: {rc}")
-        self._notifier._on_connect()
-
-
-    def _on_message(self, client:Client, db, message):
-        try:
-            self._notifier._on_message(message.topic, message.payload)
-        except Exception as ex:
-            logger.exception(ex)
-
-
-
-    ###################################
-    # Implementation of MessageBroker #
-    ###################################
-    
-    
-    def start(self, options:dict):
-        logger.info(f"MQTT broker is starting...")
-        
-        self._client.on_connect = self._on_connect
-        self._client.on_message = self._on_message
-        if username := options.get("username"):
-            self._client.username_pw_set(username, options.get("password"))
-        
-        self.host = options.get("host")
-        self.port = options.get("port")
-        self.keepalive = options.get("keepalive")
-        # logger.debug(f"host:{host} port:{port} keep:{keepalive}")
-        self._client.connect(self.host, self.port, self.keepalive)
-        
-        self._client.loop_start()
-
-
-    def stop(self):
-        logger.info(f"MQTT broker is stopping...")
-        
-        self._client.disconnect()
-        self._client.loop_stop()
-
-
-    def publish(self, topic:str, payload):
-        return self._client.publish(topic=topic, payload=payload)
-        
-    
-    def subscribe(self, topic:str, data_type):
-        return self._client.subscribe(topic=topic)
+from paho.mqtt.client import Client
+
+from broker.message_broker import MessageBroker
+from broker.notifier import BrokerNotifier
+import logging
+from abdi_config import LOGGER_NAME
+
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class MqttBroker(MessageBroker):
+    def __init__(self, notifier:BrokerNotifier):
+        self._client = Client()
+        self.host = ""
+        self.port = 0
+        self.keepalive = 0
+        
+        super().__init__(notifier=notifier)
+
+
+    def _on_connect(self, client:Client, userdata, flags, rc):
+        logger.info(f"MQTT broker connected. url: {self.host}, port: {self.port}, keepalive: {self.keepalive}")
+        # logger.debug(f"Client: {client}\nuserdata:{userdata}\nflags: {flags}\nrc: {rc}")
+        self._notifier._on_connect()
+
+
+    def _on_message(self, client:Client, db, message):
+        try:
+            self._notifier._on_message(message.topic, message.payload)
+        except Exception as ex:
+            logger.exception(ex)
+
+
+
+    ###################################
+    # Implementation of MessageBroker #
+    ###################################
+    
+    
+    def start(self, options:dict):
+        logger.info(f"MQTT broker is starting...")
+        
+        self._client.on_connect = self._on_connect
+        self._client.on_message = self._on_message
+        if username := options.get("username"):
+            self._client.username_pw_set(username, options.get("password"))
+        
+        self.host = options.get("host")
+        self.port = options.get("port")
+        self.keepalive = options.get("keepalive")
+        # logger.debug(f"host:{host} port:{port} keep:{keepalive}")
+        self._client.connect(self.host, self.port, self.keepalive)
+        
+        self._client.loop_start()
+
+
+    def stop(self):
+        logger.info(f"MQTT broker is stopping...")
+        
+        self._client.disconnect()
+        self._client.loop_stop()
+
+
+    def publish(self, topic:str, payload):
+        return self._client.publish(topic=topic, payload=payload)
+        
+    
+    def subscribe(self, topic:str, data_type):
+        return self._client.subscribe(topic=topic)
```

### Comparing `agent-bdi-2.4.1/src/broker/redis_broker.py` & `agent-bdi-2.4.2/src/broker/empty_broker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import logging
-
-from broker.message_broker import MessageBroker
-from broker.notifier import BrokerNotifier
-from abdi_config import LOGGER_NAME
-
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class RedisBroker(MessageBroker):
-    def __init__(self, notifier:BrokerNotifier):
-        logger.info(f"Initialize...")
-        
-        super().__init__(notifier=notifier)
-
-
-
-    ###################################
-    # Implementation of MessageBroker #
-    ###################################
-    
-    
-    def start(self, options:dict):
-        logger.info(f"Redis broker is starting...")
-       
-
-    def stop(self):
-        logger.info(f"Redis broker is stopping...")
-
-
-    def publish(self, topic:str, payload):
-        logger.info(f"topic: {topic}, payload: {payload}")
-        
-    
-    def subscribe(self, topic:str, data_type):
-        logger.info(f"topic: {topic}")
+import logging
+
+from broker.message_broker import MessageBroker
+from broker.notifier import BrokerNotifier
+from abdi_config import LOGGER_NAME
+
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class EmptyBroker(MessageBroker):
+    def __init__(self, notifier:BrokerNotifier):
+        logger.info(f"Initialize...")
+        
+        super().__init__(notifier=notifier)
+
+
+
+    ###################################
+    # Implementation of MessageBroker #
+    ###################################
+    
+    
+    def start(self, options:dict):
+        logger.info(f"Empty broker is starting. options:{options}")
+       
+
+    def stop(self):
+        logger.info(f"Empty broker is stopping...")
+
+
+    def publish(self, topic:str, payload):
+        logger.info(f"topic: {topic}, payload: {payload}")
+        
+    
+    def subscribe(self, topic:str, data_type):
+        logger.info(f"topic: {topic}, data_type: {data_type}")
```

### Comparing `agent-bdi-2.4.1/src/broker/ros_broker.py` & `agent-bdi-2.4.2/src/broker/redis_broker.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import logging
-
-from broker.message_broker import MessageBroker
-from broker.notifier import BrokerNotifier
-from abdi_config import LOGGER_NAME
-
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class RosBroker(MessageBroker):
-    def __init__(self, notifier:BrokerNotifier):
-        logger.info(f"Initialize...")
-        
-        super().__init__(notifier=notifier)
-
-
-
-    ###################################
-    # Implementation of MessageBroker #
-    ###################################
-    
-    
-    def start(self, options:dict):
-        logger.info(f"Ros broker is starting...")
-       
-
-    def stop(self):
-        logger.info(f"Ros broker is stopping...")
-
-
-    def publish(self, topic:str, payload):
-        logger.info(f"topic: {topic}, payload: {payload}")
-        
-    
-    def subscribe(self, topic:str, data_type):
-        logger.info(f"topic: {topic}")
+import logging
+
+from broker.message_broker import MessageBroker
+from broker.notifier import BrokerNotifier
+from abdi_config import LOGGER_NAME
+
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class RedisBroker(MessageBroker):
+    def __init__(self, notifier:BrokerNotifier):
+        logger.info(f"Initialize...")
+        
+        super().__init__(notifier=notifier)
+
+
+
+    ###################################
+    # Implementation of MessageBroker #
+    ###################################
+    
+    
+    def start(self, options:dict):
+        logger.info(f"Redis broker is starting...")
+       
+
+    def stop(self):
+        logger.info(f"Redis broker is stopping...")
+
+
+    def publish(self, topic:str, payload):
+        logger.info(f"topic: {topic}, payload: {payload}")
+        
+    
+    def subscribe(self, topic:str, data_type):
+        logger.info(f"topic: {topic}")
```

### Comparing `agent-bdi-2.4.1/src/broker/ros_noetic_broker.py` & `agent-bdi-2.4.2/src/broker/ros_noetic_broker.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import logging
-
-import rospy
-from std_msgs.msg import String, Int32, UInt8MultiArray
-
-from broker.message_broker import MessageBroker
-from broker.notifier import BrokerNotifier
-from abdi_config import LOGGER_NAME
-
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class RosNoeticBroker(MessageBroker):
-    def __init__(self, notifier:BrokerNotifier):
-        self.pub = rospy.Publisher('chatter', String, queue_size=10)
-        self.publishers = {}
-        
-        super().__init__(notifier=notifier)
-
-
-
-    ###################################
-    # Implementation of MessageBroker #
-    ###################################
-    
-    
-    def start(self, options:dict):
-        rospy.init_node(self._notifier.name, anonymous=True)
-       
-
-    def stop(self):
-        logger.info(f"Ros broker is stopping...")
-        
-        
-    def _get_publisher(self, topic, data):
-        type_name = type(data).__name__
-        topic_key = f"{topic}_{type_name}"
-        publisher = self.publishers.get(topic_key)
-        if not publisher:
-            if "str" == type_name:
-                publisher = rospy.Publisher(topic, String, queue_size=10)
-            elif "int" == type_name:
-                publisher = rospy.Publisher(topic, Int32, queue_size=10)
-            elif "bytes" == type_name:
-                publisher = rospy.Publisher(topic, UInt8MultiArray, queue_size=10)
-            else:
-                raise TypeError(f"Unsupported data type: {type_name}")
-            
-            self.publishers[topic_key] = publisher
-            
-        return publisher
-
-
-    def publish(self, topic:str, payload):
-        logger.info(f"topic: {topic}, payload: {payload}")
-        
-        publisher = self._get_publisher(topic, payload)
-        rospy.loginfo(payload)
-        publisher.publish(payload)
-        
-    
-    def _callback_with_topic(self, topic):
-        def callback(data):
-            self._notifier._on_message(topic, data)
-            rospy.loginfo(f"Received on topic {topic}, data.data: {data.data}")
-
-        return callback
-
-
-    def subscribe(self, topic:str, data_type):
-        logger.info(f"topic: {topic}, , data_type: {data_type}")
-
-        if "str" == data_type:
-            rospy.Subscriber(topic, String, self._callback_with_topic(topic))
-        elif "int" == data_type:
-            rospy.Subscriber(topic, Int32, self._callback_with_topic(topic))
-        elif "bytes" == data_type:
-            rospy.Subscriber(topic, UInt8MultiArray, self._callback_with_topic(topic))
-        else:
-            raise TypeError(f"Unsupported data type: {data_type}")
+import logging
+
+import rospy
+from std_msgs.msg import String, Int32, UInt8MultiArray
+
+from broker.message_broker import MessageBroker
+from broker.notifier import BrokerNotifier
+from abdi_config import LOGGER_NAME
+
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class RosNoeticBroker(MessageBroker):
+    def __init__(self, notifier:BrokerNotifier):
+        self.pub = rospy.Publisher('chatter', String, queue_size=10)
+        self.publishers = {}
+        
+        super().__init__(notifier=notifier)
+
+
+
+    ###################################
+    # Implementation of MessageBroker #
+    ###################################
+    
+    
+    def start(self, options:dict):
+        rospy.init_node(self._notifier.name, anonymous=True)
+       
+
+    def stop(self):
+        logger.info(f"Ros broker is stopping...")
+        
+        
+    def _get_publisher(self, topic, data):
+        type_name = type(data).__name__
+        topic_key = f"{topic}_{type_name}"
+        publisher = self.publishers.get(topic_key)
+        if not publisher:
+            if "str" == type_name:
+                publisher = rospy.Publisher(topic, String, queue_size=10)
+            elif "int" == type_name:
+                publisher = rospy.Publisher(topic, Int32, queue_size=10)
+            elif "bytes" == type_name:
+                publisher = rospy.Publisher(topic, UInt8MultiArray, queue_size=10)
+            else:
+                raise TypeError(f"Unsupported data type: {type_name}")
+            
+            self.publishers[topic_key] = publisher
+            
+        return publisher
+
+
+    def publish(self, topic:str, payload):
+        logger.info(f"topic: {topic}, payload: {payload}")
+        
+        publisher = self._get_publisher(topic, payload)
+        rospy.loginfo(payload)
+        publisher.publish(payload)
+        
+    
+    def _callback_with_topic(self, topic):
+        def callback(data):
+            self._notifier._on_message(topic, data)
+            rospy.loginfo(f"Received on topic {topic}, data.data: {data.data}")
+
+        return callback
+
+
+    def subscribe(self, topic:str, data_type):
+        logger.info(f"topic: {topic}, , data_type: {data_type}")
+
+        if "str" == data_type:
+            rospy.Subscriber(topic, String, self._callback_with_topic(topic))
+        elif "int" == data_type:
+            rospy.Subscriber(topic, Int32, self._callback_with_topic(topic))
+        elif "bytes" == data_type:
+            rospy.Subscriber(topic, UInt8MultiArray, self._callback_with_topic(topic))
+        else:
+            raise TypeError(f"Unsupported data type: {data_type}")
```

### Comparing `agent-bdi-2.4.1/src/holon/logistics/loading_coordinator.py` & `agent-bdi-2.4.2/src/holon/logistics/loading_coordinator.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-import json
-import logging
-from queue import Queue
-import random
-import threading
-import time
-
-from abdi_config import LOGGER_NAME
-from holon.HolonicAgent import HolonicAgent
-from holon.logistics.base_logistic import BaseLogistic
-
-
-logger = logging.getLogger(LOGGER_NAME)
-HEADER_RANKING = "@ranking"
-HEADER_ELECTED = "@elected"
-
-
-class LoadingCoordinator(BaseLogistic):
-    def __init__(self, agent:HolonicAgent, loading_evaluator, datatype="str"):
-        self.agent = agent
-        self.topic_handler = None
-        self.loading_evaluator = loading_evaluator
-        self.loading_rate = 0
-        self.candidates = None
-        self.electing = False
-        self.topic_payloads = Queue()
-
-        
-    def publish(self, topic, payload):
-        self.agent.publish(topic, payload)
-
-
-    def subscribe(self, topic, topic_handler=None, datatype="str"):
-        self.topic_handler = topic_handler
-        self.agent.subscribe(topic, datatype, self.start)
-        self.agent.subscribe(f"{HEADER_RANKING}.{topic}", datatype, self.rank)
-        self.agent.subscribe(f"{HEADER_ELECTED}.{topic}", datatype, self.elected)
-        
-        
-    def reset(self):
-        self._set_electing(False)
-        self.candidates = []
-        self.determine_delay = ThreadSafeCounter()
-        
-        
-    def _set_electing(self, is_electing):
-        self.electing = is_electing
-        logger.debug(f"{self.agent.short_id}> set electing to {self.electing}")
-        
-        
-    def start(self, topic:str, payload):
-        logger.debug(f"{self.agent.short_id}> topic: {topic}, payload: {payload}")
-        if self.electing:
-            logger.warning(f"{self.agent.short_id}> electing")
-            self.topic_payloads.put((topic, payload))
-            return
-        self.reset()
-        self._set_electing(True)
-        
-        self.loading_rate = self.loading_evaluator(topic, payload)
-        self.rank_number = self.loading_rate * 10000 + random.randint(0, 9999)
-
-        rank_payload = {
-            "agent_id": self.agent.agent_id,
-            "rank_number": self.rank_number
-        }
-        self.candidates.append(rank_payload)
-        self.agent.publish(f"{HEADER_RANKING}.{topic}", json.dumps(rank_payload))
-        
-        threading.Timer(.1, self.determine, args=(topic, payload)).start()
-
-
-    def rank(self, topic:str, payload):
-        if not self.electing:
-            logger.warning(f"{self.agent.short_id}> NOT electing")
-            return
-            
-        rank_payload = json.loads(payload.decode())
-        if rank_payload['agent_id'] != self.agent.agent_id:
-            self.candidates.append(rank_payload)
-            
-        self.determine_delay.add(0.01)
-        
-        
-    def determine(self, topic:str, payload):
-        if not self.electing:
-            logger.warning(f"{self.agent.short_id}> NOT electing")
-            return
-        
-        determine_delay = self.determine_delay.get_value()
-        while determine_delay > 0:
-            self.determine_delay.substract(determine_delay)
-            time.sleep(determine_delay)
-            determine_delay = self.determine_delay.get_value()
-        
-        logger.debug(f"{self.agent.short_id}> Candidates: {self.candidates}")
-        # logger.debug(f"{self.agent.short_id}> candidates size: {len(self.candidates)}")
-        if len(self.candidates):
-            min_agent = min(self.candidates, key=lambda x: (x['rank_number'], x['agent_id']))
-            if self.agent.agent_id == min_agent['agent_id']:
-                logger.info(f"{self.agent.short_id}> Elected for topic: {topic}, payload: {payload}")
-                self.agent.publish(f"{HEADER_ELECTED}.{topic}", self.agent.agent_id)
-                
-                if self.topic_handler:
-                    self.topic_handler(topic, payload)
-                else:
-                    self.agent.on_message(topic, payload)
-        
-        
-    def elected(self, topic:str, payload):
-        self.reset()
-        
-        elected_agent_id = payload.decode()
-        if not self.topic_payloads.empty():
-            work = self.topic_payloads.get()
-            if self.agent.agent_id == elected_agent_id:
-                next_topic, next_payload = work
-                logger.info(f"{self.agent.short_id}> Next work, topic: {next_topic}, payload: {next_payload}")
-                self.agent.publish(next_topic, next_payload)
-            # self.start(topic=work[0], payload=work[1])
-
-
-    def pack(self, topic:str, payload):
-        return topic, payload
-
-
-    def unpack(self, payload):
-        return payload
-            
-            
-            
-class ThreadSafeCounter:
-    def __init__(self, initial=0):
-        self.value = initial
-        self.lock = threading.Lock()
-    
-    def add(self, number):
-        with self.lock:
-            self.value += number
-    
-    def substract(self, number):
-        with self.lock:
-            self.value -= number
-    
-    def increment(self):
-        with self.lock:
-            self.value += 1
-    
-    def decrement(self):
-        with self.lock:
-            self.value -= 1
-    
-    def get_value(self):
-        with self.lock:
+import json
+import logging
+from queue import Queue
+import random
+import threading
+import time
+
+from abdi_config import LOGGER_NAME
+from holon.HolonicAgent import HolonicAgent
+from holon.logistics.base_logistic import BaseLogistic
+
+
+logger = logging.getLogger(LOGGER_NAME)
+HEADER_RANKING = "@ranking"
+HEADER_ELECTED = "@elected"
+
+
+class LoadingCoordinator(BaseLogistic):
+    def __init__(self, agent:HolonicAgent, loading_evaluator, datatype="str"):
+        self.agent = agent
+        self.topic_handler = None
+        self.loading_evaluator = loading_evaluator
+        self.loading_rate = 0
+        self.candidates = None
+        self.electing = False
+        self.topic_payloads = Queue()
+
+        
+    def publish(self, topic, payload):
+        self.agent.publish(topic, payload)
+
+
+    def subscribe(self, topic, topic_handler=None, datatype="str"):
+        self.topic_handler = topic_handler
+        self.agent.subscribe(topic, datatype, self.start)
+        self.agent.subscribe(f"{HEADER_RANKING}.{topic}", datatype, self.rank)
+        self.agent.subscribe(f"{HEADER_ELECTED}.{topic}", datatype, self.elected)
+        
+        
+    def reset(self):
+        self._set_electing(False)
+        self.candidates = []
+        self.determine_delay = ThreadSafeCounter()
+        
+        
+    def _set_electing(self, is_electing):
+        self.electing = is_electing
+        logger.debug(f"{self.agent.short_id}> set electing to {self.electing}")
+        
+        
+    def start(self, topic:str, payload):
+        logger.debug(f"{self.agent.short_id}> topic: {topic}, payload: {payload}")
+        if self.electing:
+            logger.warning(f"{self.agent.short_id}> electing")
+            self.topic_payloads.put((topic, payload))
+            return
+        self.reset()
+        self._set_electing(True)
+        
+        self.loading_rate = self.loading_evaluator(topic, payload)
+        self.rank_number = self.loading_rate * 10000 + random.randint(0, 9999)
+
+        rank_payload = {
+            "agent_id": self.agent.agent_id,
+            "rank_number": self.rank_number
+        }
+        self.candidates.append(rank_payload)
+        self.agent.publish(f"{HEADER_RANKING}.{topic}", json.dumps(rank_payload))
+        
+        threading.Timer(.1, self.determine, args=(topic, payload)).start()
+
+
+    def rank(self, topic:str, payload):
+        if not self.electing:
+            logger.warning(f"{self.agent.short_id}> NOT electing")
+            return
+            
+        rank_payload = json.loads(payload.decode())
+        if rank_payload['agent_id'] != self.agent.agent_id:
+            self.candidates.append(rank_payload)
+            
+        self.determine_delay.add(0.01)
+        
+        
+    def determine(self, topic:str, payload):
+        if not self.electing:
+            logger.warning(f"{self.agent.short_id}> NOT electing")
+            return
+        
+        determine_delay = self.determine_delay.get_value()
+        while determine_delay > 0:
+            self.determine_delay.substract(determine_delay)
+            time.sleep(determine_delay)
+            determine_delay = self.determine_delay.get_value()
+        
+        logger.debug(f"{self.agent.short_id}> Candidates: {self.candidates}")
+        # logger.debug(f"{self.agent.short_id}> candidates size: {len(self.candidates)}")
+        if len(self.candidates):
+            min_agent = min(self.candidates, key=lambda x: (x['rank_number'], x['agent_id']))
+            if self.agent.agent_id == min_agent['agent_id']:
+                logger.info(f"{self.agent.short_id}> Elected for topic: {topic}, payload: {payload}")
+                self.agent.publish(f"{HEADER_ELECTED}.{topic}", self.agent.agent_id)
+                
+                if self.topic_handler:
+                    self.topic_handler(topic, payload)
+                else:
+                    self.agent.on_message(topic, payload)
+        
+        
+    def elected(self, topic:str, payload):
+        self.reset()
+        
+        elected_agent_id = payload.decode()
+        if not self.topic_payloads.empty():
+            work = self.topic_payloads.get()
+            if self.agent.agent_id == elected_agent_id:
+                next_topic, next_payload = work
+                logger.info(f"{self.agent.short_id}> Next work, topic: {next_topic}, payload: {next_payload}")
+                self.agent.publish(next_topic, next_payload)
+            # self.start(topic=work[0], payload=work[1])
+
+
+    def pack(self, topic:str, payload):
+        return topic, payload
+
+
+    def unpack(self, payload):
+        return payload
+            
+            
+            
+class ThreadSafeCounter:
+    def __init__(self, initial=0):
+        self.value = initial
+        self.lock = threading.Lock()
+    
+    def add(self, number):
+        with self.lock:
+            self.value += number
+    
+    def substract(self, number):
+        with self.lock:
+            self.value -= number
+    
+    def increment(self):
+        with self.lock:
+            self.value += 1
+    
+    def decrement(self):
+        with self.lock:
+            self.value -= 1
+    
+    def get_value(self):
+        with self.lock:
             return self.value
```

### Comparing `agent-bdi-2.4.1/src/holon/logistics/payload_wrapper.py` & `agent-bdi-2.4.2/src/holon/logistics/payload_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,185 +1,193 @@
-import json
-import logging
-import pickle
-import uuid
-
-from abdi_config import LOGGER_NAME
-
-logger = logging.getLogger(LOGGER_NAME)
-VERSION = "0001"
-VERSION_BYTES = VERSION.encode('utf-8')
-# WRAPPER_HEAD = "950f7f7ba7c111eea5c4ff9ca9F3fcfd"
-# WRAPPER_HEAD = "950f7f7ba7c111ee"
-WRAPPER_REQUEST_HEAD = "950f7f7ba7c111ee"
-WRAPPER_RESPONSE_HEAD = "a5c4ff9ca9F3fcfd"
-WRAPPER_REQUEST_HEAD_BYTES = WRAPPER_REQUEST_HEAD.encode("utf-8")
-WRAPPER_RESPONSE_HEAD_BYTES = WRAPPER_RESPONSE_HEAD.encode("utf-8")
-
-
-class PayloadWrapper:
-    def __init__(self, agent_id:str):
-        self.binary_wrapper = BinaryWrapper(self)
-        self.text_wrapper = TextWrapper(self)
-        self.agent_id = agent_id
-        
-        
-    def create_response_json(self, response_payload, request_payload):
-        response_json = {
-            "version": VERSION,
-            "request_id": request_payload["request_id"],
-            "receiver": request_payload["sender"],
-            "request_token": request_payload["request_token"]
-        }
-        response_json["content"] = response_payload
-        
-        return response_json
-        
-        
-    def create_request_json(self, payload, request_id):
-        request_json = {
-            "version": VERSION,
-            "request_id": request_id,
-            "sender": self.agent_id,
-            "request_token": str(uuid.uuid4()).replace("-", "")
-        }
-        request_json["content"] = payload
-        
-        return request_json
-        
-
-    def get_payload_wrapper(self, payload):
-        # logger.debug(f"get_payload_wrapper, payload: {payload}, type: {type(payload)}")
-        if payload:
-            if self.text_wrapper.is_acceptable(payload):
-                return self.text_wrapper
-            elif self.binary_wrapper.is_acceptable(payload):
-                return self.binary_wrapper
-            else:
-                return None
-        else:
-            return payload
-        
-        
-    def is_request(self, payload:bytes):
-        return self.__check_head(payload, WRAPPER_REQUEST_HEAD_BYTES)
-        
-        
-    def is_response(self, payload:bytes):
-        return self.__check_head(payload, WRAPPER_RESPONSE_HEAD_BYTES)
-    
-    
-    def __check_head(self, payload:bytes, head_to_check):
-        managed = False
-
-        if payload:
-            head_bytes = payload[:len(head_to_check)]
-            # logger.debug(f"head_bytes: {head_bytes}, head_to_check: {head_to_check}")
-            managed = head_bytes == head_to_check
-
-        return managed
-
-
-    def unpack(self, payload):
-        wrapper = self.get_payload_wrapper(payload)
-        if wrapper:
-            unpacked = wrapper.unpack(payload)
-        else:
-            raise Exception("Not managed payload.")
-            
-        return unpacked
-
-
-    def wrap_for_response(self, payload:str, managed_request_payload:str) -> str:
-        wrapper = self.get_payload_wrapper(payload)
-        if wrapper:
-            payload_resp = wrapper.wrap_for_response(payload, managed_request_payload)
-        else:
-            raise Exception(f"Unsupported payload type: {type(payload)}")
-
-        return payload_resp
-
-
-    def wrap_for_request(self, payload, request_id) -> str:
-        wrapper = self.get_payload_wrapper(payload)
-        if wrapper:
-            payload_request, request_token = wrapper.wrap_for_request(payload, request_id)
-        else:
-            raise Exception("Unsupported payload type.")
-
-        return payload_request, request_token
-
-
-
-class BinaryWrapper:
-    def __init__(self, payload_wrapper:PayloadWrapper):
-        self.payload_wrapper = payload_wrapper
-        
-        
-    def is_acceptable(self, payload):
-        return isinstance(payload, bytes) or isinstance(payload, bytearray)
-
-        
-    def unpack(self, payload:bytes):
-        payload_body = payload[len(WRAPPER_REQUEST_HEAD_BYTES):]
-        payload_json = pickle.loads(payload_body)
-
-        if VERSION != payload_json["version"]:
-            raise Exception("Invalid payload version.")
-
-        return payload_json
-
-
-    def wrap_for_request(self, payload, request_id) -> bytes:
-        request_json = self.payload_wrapper.create_request_json(payload, request_id)
-        request_payload = WRAPPER_REQUEST_HEAD_BYTES + pickle.dumps(request_json)
-        
-        return request_payload, request_json['request_token']
-     
-        
-    def wrap_for_response(self, response_payload:bytes, managed_request_payload) -> bytes:
-        response_json = self.payload_wrapper.create_response_json(response_payload, managed_request_payload)
-        response_payload = WRAPPER_RESPONSE_HEAD_BYTES + pickle.dumps(response_json)
-        
-        return response_payload
-
-
-            
-class TextWrapper:
-    def __init__(self, payload_wrapper:PayloadWrapper):
-        self.payload_wrapper = payload_wrapper
-        
-        
-    def is_acceptable(self, payload):
-        if isinstance(payload, str):
-            acceptable = True
-        else:
-            try:
-                _ = payload.decode('utf-8')
-                acceptable = True
-            except UnicodeDecodeError:
-                acceptable = False
-            
-        return acceptable
-
-        
-    def unpack(self, payload:str):
-        payload_text = payload.decode('utf-8')
-        payload_json = json.loads(payload_text[len(WRAPPER_REQUEST_HEAD):])
-        logger.debug(f"payload_json: {str(payload_json)[:300]}...")
-        if VERSION != payload_json["version"]:
-            raise Exception("Invalid payload version.")
-        return payload_json
-
-
-    def wrap_for_request(self, payload, request_id) -> str:
-        request_json = self.payload_wrapper.create_request_json(payload, request_id)
-        request_payload = f"{WRAPPER_REQUEST_HEAD}{json.dumps(request_json)}"
-        
-        return request_payload, request_json['request_token']
-                
-        
-    def wrap_for_response(self, response_payload:str, managed_request_payload) -> str:
-        response_json = self.payload_wrapper.create_response_json(response_payload, managed_request_payload)
-        response_payload = f"{WRAPPER_RESPONSE_HEAD}{json.dumps(response_json)}"
-        
-        return response_payload
+import copy
+import json
+import logging
+import pickle
+import uuid
+
+from abdi_config import LOGGER_NAME
+
+logger = logging.getLogger(LOGGER_NAME)
+VERSION = "0001"
+VERSION_BYTES = VERSION.encode('utf-8')
+# WRAPPER_HEAD = "950f7f7ba7c111eea5c4ff9ca9F3fcfd"
+# WRAPPER_HEAD = "950f7f7ba7c111ee"
+WRAPPER_REQUEST_HEAD = "950f7f7ba7c111ee"
+WRAPPER_RESPONSE_HEAD = "a5c4ff9ca9F3fcfd"
+WRAPPER_REQUEST_HEAD_BYTES = WRAPPER_REQUEST_HEAD.encode("utf-8")
+WRAPPER_RESPONSE_HEAD_BYTES = WRAPPER_RESPONSE_HEAD.encode("utf-8")
+
+
+class PayloadWrapper:
+    def __init__(self, agent_id:str):
+        self.binary_wrapper = BinaryWrapper(self)
+        self.text_wrapper = TextWrapper(self)
+        self.agent_id = agent_id
+        
+        
+    def create_response_json(self, response_payload, request_payload):
+        response_json = copy.deepcopy(request_payload)
+        # response_json = {
+        #     "version": VERSION,
+        #     "request_id": request_payload["request_id"],
+        #     "receiver": request_payload["sender"],
+        #     "request_token": request_payload["request_token"]
+        # }
+        response_json["version"] = VERSION
+        response_json["content"] = response_payload
+
+        # if 'source_payload' in request_payload:
+        #     response_json["source_payload"] = request_payload["source_payload"]
+        
+        return response_json
+        
+        
+    def create_request_json(self, payload, request_id, source_payload):
+        request_json = {
+            "version": VERSION,
+            "request_id": request_id,
+            "sender": self.agent_id,
+            "request_token": str(uuid.uuid4()).replace("-", "")
+        }
+        request_json["content"] = payload
+
+        if source_payload:
+            request_json["source_payload"] = source_payload
+        
+        return request_json
+        
+
+    def get_payload_wrapper(self, payload):
+        # logger.debug(f"get_payload_wrapper, payload: {payload}, type: {type(payload)}")
+        if payload:
+            if self.text_wrapper.is_acceptable(payload):
+                return self.text_wrapper
+            elif self.binary_wrapper.is_acceptable(payload):
+                return self.binary_wrapper
+            else:
+                return None
+        else:
+            return payload
+        
+        
+    def is_request(self, payload:bytes):
+        return self.__check_head(payload, WRAPPER_REQUEST_HEAD_BYTES)
+        
+        
+    def is_response(self, payload:bytes):
+        return self.__check_head(payload, WRAPPER_RESPONSE_HEAD_BYTES)
+    
+    
+    def __check_head(self, payload:bytes, head_to_check):
+        managed = False
+
+        if payload:
+            head_bytes = payload[:len(head_to_check)]
+            # logger.debug(f"head_bytes: {head_bytes}, head_to_check: {head_to_check}")
+            managed = head_bytes == head_to_check
+
+        return managed
+
+
+    def unpack(self, payload):
+        wrapper = self.get_payload_wrapper(payload)
+        if wrapper:
+            unpacked = wrapper.unpack(payload)
+        else:
+            raise Exception("Not managed payload.")
+            
+        return unpacked
+
+
+    def wrap_for_response(self, payload:str, managed_request_payload:str) -> str:
+        wrapper = self.get_payload_wrapper(payload)
+        if wrapper:
+            payload_resp = wrapper.wrap_for_response(payload, managed_request_payload)
+        else:
+            raise Exception(f"Unsupported payload type: {type(payload)}")
+
+        return payload_resp
+
+
+    def wrap_for_request(self, payload, request_id, source_payload) -> str:
+        if wrapper := self.get_payload_wrapper(payload):
+            payload_request, request_token = wrapper.wrap_for_request(payload, request_id, source_payload)
+        else:
+            raise Exception("Unsupported payload type.")
+
+        return payload_request, request_token
+
+
+
+class BinaryWrapper:
+    def __init__(self, payload_wrapper:PayloadWrapper):
+        self.payload_wrapper = payload_wrapper
+        
+        
+    def is_acceptable(self, payload):
+        return isinstance(payload, bytes) or isinstance(payload, bytearray)
+
+        
+    def unpack(self, payload:bytes):
+        payload_body = payload[len(WRAPPER_REQUEST_HEAD_BYTES):]
+        payload_json = pickle.loads(payload_body)
+
+        if VERSION != payload_json["version"]:
+            raise Exception("Invalid payload version.")
+
+        return payload_json
+
+
+    def wrap_for_request(self, payload, request_id, source_payload) -> bytes:
+        request_json = self.payload_wrapper.create_request_json(payload, request_id, source_payload)
+        request_payload = WRAPPER_REQUEST_HEAD_BYTES + pickle.dumps(request_json)
+        
+        return request_payload, request_json['request_token']
+     
+        
+    def wrap_for_response(self, response_payload:bytes, managed_request_payload) -> bytes:
+        response_json = self.payload_wrapper.create_response_json(response_payload, managed_request_payload)
+        response_payload = WRAPPER_RESPONSE_HEAD_BYTES + pickle.dumps(response_json)
+        
+        return response_payload
+
+
+            
+class TextWrapper:
+    def __init__(self, payload_wrapper:PayloadWrapper):
+        self.payload_wrapper = payload_wrapper
+        
+        
+    def is_acceptable(self, payload):
+        if isinstance(payload, str):
+            acceptable = True
+        else:
+            try:
+                _ = payload.decode('utf-8')
+                acceptable = True
+            except UnicodeDecodeError:
+                acceptable = False
+            
+        return acceptable
+
+        
+    def unpack(self, payload:str):
+        payload_text = payload.decode('utf-8')
+        payload_json = json.loads(payload_text[len(WRAPPER_REQUEST_HEAD):])
+        logger.debug(f"payload_json: {str(payload_json)[:300]}...")
+        if VERSION != payload_json["version"]:
+            raise Exception("Invalid payload version.")
+        return payload_json
+
+
+    def wrap_for_request(self, payload, request_id, source_payload) -> str:
+        request_json = self.payload_wrapper.create_request_json(payload, request_id, source_payload)
+        request_payload = f"{WRAPPER_REQUEST_HEAD}{json.dumps(request_json)}"
+        
+        return request_payload, request_json['request_token']
+                
+        
+    def wrap_for_response(self, response_payload:str, managed_request_payload) -> str:
+        response_json = self.payload_wrapper.create_response_json(response_payload, managed_request_payload)
+        response_payload = f"{WRAPPER_RESPONSE_HEAD}{json.dumps(response_json)}"
+        
+        return response_payload
```

### Comparing `agent-bdi-2.4.1/src/holon/logistics/request_logistic.py` & `agent-bdi-2.4.2/src/_bak/request_logistic-20240502.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import logging
-
-from abdi_config import LOGGER_NAME
-from holon.HolonicAgent import HolonicAgent
-from holon.logistics.base_logistic import BaseLogistic
-from holon.logistics.payload_wrapper import PayloadWrapper
-
-
-logger = logging.getLogger(LOGGER_NAME)
-PUBLISH_HEADER = "@request"
-SUBSCRIBE_HEADER = "@response"
-
-
-class RequestLogistic(BaseLogistic):
-    __handlers = {}
-    
-    
-    def __init__(self, agent:HolonicAgent, request_id=""):
-        self.agent = agent
-        self.request_id = request_id
-        self.response_topic_header = f"{SUBSCRIBE_HEADER}.{self.agent.agent_id}.{self.request_id}"
-        logger.debug(f"self, agent_id: {self.agent.agent_id}, short_id: {self.agent.short_id}, request_id: {self.request_id}")
-        self._payload_wrapper = PayloadWrapper(self.agent.agent_id)
-        
-        
-    def publish(self, topic, payload):
-        logistic_topic = f"{PUBLISH_HEADER}.{topic}"
-        logger.debug(f"agent_id: {self.agent.agent_id}, request_id: {self.request_id}")
-        packed_payload, request_token = self._payload_wrapper.wrap_for_request(payload, self.request_id)
-        # logistic_topic, packed_payload = self.pack(topic, payload)
-        logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)[:300]}")
-        self.agent.publish(logistic_topic, packed_payload)
-        
-        return request_token
-
-
-    def subscribe(self, topic, topic_handler=None, datatype="str"):
-        response_topic = f"{self.response_topic_header}.{topic}"
-        logger.debug(f"response_topic: {response_topic}")
-        self.agent.subscribe(response_topic, datatype, self.handle_response)
-        RequestLogistic.__handlers[self.response_topic_header] = topic_handler
-
-
-    def handle_response(self, topic:str, payload):
-        responsed_topic = topic[len(self.response_topic_header)+1:]
-        unpacked = self._payload_wrapper.unpack(payload)
-        logger.debug(f"topic: {topic}, unpacked: {str(unpacked)[:300]}")
-
-        if topic_handler := RequestLogistic.__handlers[self.response_topic_header]:
-            self.agent.set_topic_handler(responsed_topic, topic_handler)
-        self.agent._on_message(topic=responsed_topic, 
-                               payload=unpacked["content"], 
-                               payload_info=unpacked["request_token"])
-
-
-    # def handle_response(self, topic:str, payload):
-    #     responsed_topic = topic[len(self.response_topic_header)+1:]
-    #     # unpacked = self.unpack(payload)
-    #     unpacked = self._payload_wrapper.unpack(payload)
-    #     if unpacked["receiver"] == self.agent.agent_id:
-    #         if unpacked["request_id"] == self.request_id:
-    #             logger.debug(f"MATCHED, agent_id: {self.agent.agent_id}, request_id: {self.request_id}")
-    #             self.agent._on_message(responsed_topic, unpacked["content"])
-    #         else:
-    #             logger.debug(f"NOT matched, request_id: {unpacked['request_id']}, self.request_id: {self.request_id}")
-    #     else:
-    #         logger.debug(f"NOT matched, receiver: {unpacked['receiver']}, agent_id: {self.agent.agent_id}")
-            
-
-
-    # def pack(self, topic:str, payload):
-    #     if topic == self.request_topic:
-    #         # request_id = str(uuid.uuid4())
-    #         packed = self._payload_wrapper.wrap_for_request(payload, self.request_id)
-    #         # logger.debug(f"packed: {packed}")
-    #         return f"{PUBLISH_HEADER}.{topic}", packed
-    #     else:
-    #         return topic, payload
-
-
-    # def unpack(self, payload):
-    #     unpacked = self._payload_wrapper.unpack(payload)
-    #     return unpacked
+import logging
+
+from abdi_config import LOGGER_NAME
+from holon.HolonicAgent import HolonicAgent
+from holon.logistics.base_logistic import BaseLogistic
+from holon.logistics.payload_wrapper import PayloadWrapper
+
+
+logger = logging.getLogger(LOGGER_NAME)
+PUBLISH_HEADER = "@request"
+SUBSCRIBE_HEADER = "@response"
+
+
+class RequestLogistic(BaseLogistic):
+    __handlers = {}
+    
+    
+    def __init__(self, agent:HolonicAgent, request_id=""):
+        self.agent = agent
+        self.request_id = request_id
+        self.response_topic_header = f"{SUBSCRIBE_HEADER}.{self.agent.agent_id}.{self.request_id}"
+        logger.debug(f"self, agent_id: {self.agent.agent_id}, short_id: {self.agent.short_id}, request_id: {self.request_id}")
+        self._payload_wrapper = PayloadWrapper(self.agent.agent_id)
+        
+        
+    def publish(self, topic, payload):
+        logistic_topic = f"{PUBLISH_HEADER}.{topic}"
+        logger.debug(f"agent_id: {self.agent.agent_id}, request_id: {self.request_id}")
+        packed_payload, request_token = self._payload_wrapper.wrap_for_request(payload, self.request_id)
+        # logistic_topic, packed_payload = self.pack(topic, payload)
+        logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)[:300]}")
+        self.agent.publish(logistic_topic, packed_payload)
+
+        return request_token
+
+
+    def subscribe(self, topic, topic_handler=None, datatype="str"):
+        response_topic = f"{self.response_topic_header}.{topic}"
+        logger.debug(f"response_topic: {response_topic}")
+        self.agent.subscribe(response_topic, datatype, self.handle_response)
+        RequestLogistic.__handlers[self.response_topic_header] = topic_handler
+
+
+    def handle_response(self, topic:str, payload):
+        responsed_topic = topic[len(self.response_topic_header)+1:]
+        unpacked = self._payload_wrapper.unpack(payload)
+        logger.debug(f"topic: {topic}, unpacked: {str(unpacked)[:300]}")
+
+        if topic_handler := RequestLogistic.__handlers[self.response_topic_header]:
+            self.agent.set_topic_handler(responsed_topic, topic_handler)
+        self.agent._on_message(topic=responsed_topic, 
+                               payload=unpacked["content"], 
+                               payload_info=unpacked["request_token"])
+
+
+    # def handle_response(self, topic:str, payload):
+    #     responsed_topic = topic[len(self.response_topic_header)+1:]
+    #     # unpacked = self.unpack(payload)
+    #     unpacked = self._payload_wrapper.unpack(payload)
+    #     if unpacked["receiver"] == self.agent.agent_id:
+    #         if unpacked["request_id"] == self.request_id:
+    #             logger.debug(f"MATCHED, agent_id: {self.agent.agent_id}, request_id: {self.request_id}")
+    #             self.agent._on_message(responsed_topic, unpacked["content"])
+    #         else:
+    #             logger.debug(f"NOT matched, request_id: {unpacked['request_id']}, self.request_id: {self.request_id}")
+    #     else:
+    #         logger.debug(f"NOT matched, receiver: {unpacked['receiver']}, agent_id: {self.agent.agent_id}")
+            
+
+
+    # def pack(self, topic:str, payload):
+    #     if topic == self.request_topic:
+    #         # request_id = str(uuid.uuid4())
+    #         packed = self._payload_wrapper.wrap_for_request(payload, self.request_id)
+    #         # logger.debug(f"packed: {packed}")
+    #         return f"{PUBLISH_HEADER}.{topic}", packed
+    #     else:
+    #         return topic, payload
+
+
+    # def unpack(self, payload):
+    #     unpacked = self._payload_wrapper.unpack(payload)
+    #     return unpacked
```

### Comparing `agent-bdi-2.4.1/src/holon/logistics/response_logistic.py` & `agent-bdi-2.4.2/src/holon/logistics/request_logistic.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,69 @@
-import logging
-import threading
-
-from abdi_config import LOGGER_NAME
-from holon.HolonicAgent import HolonicAgent
-from holon.logistics.base_logistic import BaseLogistic
-from holon.logistics.payload_wrapper import PayloadWrapper
-
-
-logger = logging.getLogger(LOGGER_NAME)
-PUBLISH_HEADER = "@response"
-SUBSCRIBE_HEADER = "@request"
-
-
-class ResponseLogistic(BaseLogistic):
-    def __init__(self, agent:HolonicAgent):
-        self.agent = agent
-        self._payload_wrapper = PayloadWrapper(self.agent.agent_id)
-        
-        
-    # def publish(self, topic, payload):
-    #     sender_id = self.request_payload['sender']
-    #     request_id = self.request_payload['request_id']
-    #     logistic_topic = f"{PUBLISH_HEADER}.{sender_id}.{request_id}.{topic}"
-    #     packed_payload = self._payload_wrapper.wrap_for_response(payload, self.request_payload)
-    #     logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)[:300]}")
-    #     # logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)}")
-    #     # self.agent.publish(logistic_topic, str(packed_payload))
-    #     self.agent.publish(logistic_topic, packed_payload)
-
-
-    def subscribe(self, topic, topic_handler=None, datatype="str"):
-        request_topic = f"{SUBSCRIBE_HEADER}.{topic}"
-        logger.debug(f"request_topic: {request_topic}")
-        self.agent.subscribe(request_topic, datatype, self.handle_request)
-
-        if topic_handler:
-            self.agent.set_topic_handler(topic, topic_handler)
-
-        
-    def handle_request(self, topic:str, payload):
-        logger.debug(f"topic: {topic}, payload: {str(payload)[:300]}...")
-        request_topic = topic[len(SUBSCRIBE_HEADER)+1:]
-        request_payload = self._payload_wrapper.unpack(payload)
-        
-        def on_message(request_topic, request_payload):
-            output = self.agent._on_message(request_topic, request_payload["content"])
-            if output and isinstance(output, tuple) and len(output) == 2:
-                resp_topic, resp_result = output
-                sender_id = request_payload['sender']
-                request_id = request_payload['request_id']
-                logistic_topic = f"{PUBLISH_HEADER}.{sender_id}.{request_id}.{resp_topic}"
-                packed_payload = self._payload_wrapper.wrap_for_response(resp_result, request_payload)
-                logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)[:300]}")
-                self.agent.publish(logistic_topic, packed_payload)
-            
-        threading.Thread(target=on_message, 
-                         args=(request_topic, request_payload)).start()
-        # self.agent._on_message(request_topic, request_payload["content"])
-
-        
-    # def handle_request(self, topic:str, payload):
-    #     logger.debug(f"topic: {topic}, payload: {str(payload)[:300]}...")
-    #     request_topic = topic[len(SUBSCRIBE_HEADER)+1:]
-    #     self.request_payload = self._payload_wrapper.unpack(payload)
-    #     content = self.request_payload["content"]
-    #     # logger.debug(f"request_topic: {request_topic}, agent_id: {self.agent.agent_id}, content: {content}")
-    #     self.agent._on_message(request_topic, content)
+import logging
+
+from abdi_config import LOGGER_NAME
+from holon.HolonicAgent import HolonicAgent
+from holon.logistics.base_logistic import BaseLogistic
+from holon.logistics.payload_wrapper import PayloadWrapper
+
+
+logger = logging.getLogger(LOGGER_NAME)
+PUBLISH_HEADER = "@request"
+SUBSCRIBE_HEADER = "@response"
+
+
+class RequestLogistic(BaseLogistic):
+    __handlers = {}
+    
+    
+    def __init__(self, agent:HolonicAgent, request_id=""):
+        self.agent = agent
+        self.request_id = request_id
+        self.response_topic_header = f"{SUBSCRIBE_HEADER}.{self.agent.agent_id}.{self.request_id}"
+        logger.debug(f"self, agent_id: {self.agent.agent_id}, short_id: {self.agent.short_id}, request_id: {self.request_id}")
+        self._payload_wrapper = PayloadWrapper(self.agent.agent_id)
+        
+        
+    def publish(self, topic, payload, source_payload=None):
+        logger.debug(f"topic: {topic}, source_payload: {source_payload}")
+        logistic_topic = f"{PUBLISH_HEADER}.{topic}"
+        logger.debug(f"agent_id: {self.agent.agent_id}, request_id: {self.request_id}")
+        packed_payload, request_token = self._payload_wrapper.wrap_for_request(payload, self.request_id, source_payload)
+        # logistic_topic, packed_payload = self.pack(topic, payload)
+        logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)}")
+        # logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)[:300]}")
+        self.agent.publish(logistic_topic, packed_payload)
+
+        return request_token
+
+
+    def subscribe(self, topic, topic_handler=None, datatype="str"):
+        response_topic = f"{self.response_topic_header}.{topic}"
+        logger.debug(f"response_topic: {response_topic}")
+        self.agent.subscribe(response_topic, datatype, self.handle_response)
+        RequestLogistic.__handlers[self.response_topic_header] = topic_handler
+
+
+    def handle_response(self, topic:str, payload):
+        responsed_topic = topic[len(self.response_topic_header)+1:]
+        unpacked = self._payload_wrapper.unpack(payload)
+        logger.debug(f"topic: {topic}, unpacked: {str(unpacked)}")
+
+        if topic_handler := RequestLogistic.__handlers[self.response_topic_header]:
+            self.agent.set_topic_handler(responsed_topic, topic_handler)
+        self.agent._on_message(topic=responsed_topic, 
+                               payload=unpacked["content"], 
+                               source_payload=unpacked)
+
+
+    # def handle_response(self, topic:str, payload):
+    #     responsed_topic = topic[len(self.response_topic_header)+1:]
+    #     # unpacked = self.unpack(payload)
+    #     unpacked = self._payload_wrapper.unpack(payload)
+    #     if unpacked["receiver"] == self.agent.agent_id:
+    #         if unpacked["request_id"] == self.request_id:
+    #             logger.debug(f"MATCHED, agent_id: {self.agent.agent_id}, request_id: {self.request_id}")
+    #             self.agent._on_message(responsed_topic, unpacked["content"])
+    #         else:
+    #             logger.debug(f"NOT matched, request_id: {unpacked['request_id']}, self.request_id: {self.request_id}")
+    #     else:
+    #         logger.debug(f"NOT matched, receiver: {unpacked['receiver']}, agent_id: {self.agent.agent_id}")
```

