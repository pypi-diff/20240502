# Comparing `tmp/pupil_labs_realtime_api-1.2.0a3.tar.gz` & `tmp/pupil_labs_realtime_api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pupil_labs_realtime_api-1.2.0a3.tar", last modified: Mon Oct 10 12:04:41 2022, max compression
+gzip compressed data, was "pupil_labs_realtime_api-1.2.1.tar", last modified: Thu May  2 11:23:41 2024, max compression
```

## Comparing `pupil_labs_realtime_api-1.2.0a3.tar` & `pupil_labs_realtime_api-1.2.1.tar`

### file list

```diff
@@ -1,93 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.856255 pupil_labs_realtime_api-1.2.0a3/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6134 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-10-10 12:04:41.856255 pupil_labs_realtime_api-1.2.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/api/async.rst
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/api/base.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/api/simple.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/examples/async.rst
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2185 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/examples/simple.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13663 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/guides/under-the-hood.rst
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.844255 pupil_labs_realtime_api-1.2.0a3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.848255 pupil_labs_realtime_api-1.2.0a3/examples/async/
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/device_camera_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_get_current.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_update_via_callback.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_update_wait.py
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/device_time_offset.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/discover_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/send_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/start_stop_recordings.py
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/stream_gaze.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/stream_scene_camera_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/async/stream_video_with_overlayed_gaze.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.852255 pupil_labs_realtime_api-1.2.0a3/examples/simple/
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/device_time_offset.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/discover_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/get_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/send_event.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/start_stop_recordings.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/status_auto_update.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_gaze.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_scene_camera_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_video_with_overlayed_gaze.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1572 2022-10-10 12:04:41.856255 pupil_labs_realtime_api-1.2.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.844255 pupil_labs_realtime_api-1.2.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.844255 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.852255 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/camera_control.py
--rw-r--r--   0 runner    (1001) docker     (121)    13297 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     4170 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     8191 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.852255 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7031 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13746 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.852255 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4087 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/gaze.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/nal_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/video.py
--rw-r--r--   0 runner    (1001) docker     (121)     7361 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/time_echo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.856255 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-10 12:04:41.000000 pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 12:04:41.856255 pupil_labs_realtime_api-1.2.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/tests/test_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-10-10 12:04:14.000000 pupil_labs_realtime_api-1.2.0a3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.545349 pupil_labs_realtime_api-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.533349 pupil_labs_realtime_api-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.533349 pupil_labs_realtime_api-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-02 11:23:41.545349 pupil_labs_realtime_api-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.533349 pupil_labs_realtime_api-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.537349 pupil_labs_realtime_api-1.2.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/api/async.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/api/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/api/simple.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.537349 pupil_labs_realtime_api-1.2.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/examples/async.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/examples/simple.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.537349 pupil_labs_realtime_api-1.2.1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/guides/simple-vs-async-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13663 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/guides/under-the-hood.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.529349 pupil_labs_realtime_api-1.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.537349 pupil_labs_realtime_api-1.2.1/examples/async/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/device_status_get_current.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/device_status_update_via_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/device_status_update_wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/device_time_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/discover_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/send_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/start_stop_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/stream_eyes_camera_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/stream_gaze.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/stream_imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/stream_scene_camera_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/async/stream_video_with_overlayed_gaze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.541349 pupil_labs_realtime_api-1.2.1/examples/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/camera_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/device_time_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/discover_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/get_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/send_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/start_stop_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/status_auto_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/stream_eyes_camera_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/stream_gaze.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/stream_imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/stream_scene_camera_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/stream_scene_eyes_and_gaze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/examples/simple/stream_video_with_overlayed_gaze.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-02 11:23:41.549349 pupil_labs_realtime_api-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.529349 pupil_labs_realtime_api-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.529349 pupil_labs_realtime_api-1.2.1/src/pupil_labs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.541349 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.541349 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/simple/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/simple/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/simple/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/simple/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.545349 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/gaze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14734 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/imu_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/nal_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/time_echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.545349 pupil_labs_realtime_api-1.2.1/src/pupil_labs_realtime_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-02 11:23:41.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs_realtime_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-02 11:23:41.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs_realtime_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:23:41.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs_realtime_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-02 11:23:41.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs_realtime_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 11:23:41.000000 pupil_labs_realtime_api-1.2.1/src/pupil_labs_realtime_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:41.545349 pupil_labs_realtime_api-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-02 11:23:26.000000 pupil_labs_realtime_api-1.2.1/tox.ini
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/.github/workflows/main.yml` & `pupil_labs_realtime_api-1.2.1/.github/workflows/main.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,68 @@
 name: tests
 
-on: [push, pull_request]
+on:
+  pull_request:
+  push:
+    tags:
+      - "**"
+  workflow_dispatch:
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - 3.7
-        - 3.8
-        - 3.9
-        - "3.10"
+          - 3.8
+          - 3.9
+          - "3.10"
+          - "3.11"
         platform:
-        - ubuntu-latest
-        - macos-latest
-        - windows-latest
+          - ubuntu-latest
+          - macos-latest
+          - windows-latest
     runs-on: ${{ matrix.platform }}
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}
+          python-version: ${{ matrix.python }}-dev
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
+  check: # This job does nothing and is only used for the branch protection
+    if: always()
+
+    needs:
+      - test
+
+    runs-on: ubuntu-latest
+
+    steps:
+      - name: Decide whether the needed jobs succeeded or failed
+        uses: re-actors/alls-green@release/v1
+        with:
+          jobs: ${{ toJSON(needs) }}
+
   release:
-    needs: test
+    needs:
+      - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11-dev"
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Release
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/.gitignore` & `pupil_labs_realtime_api-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/.pre-commit-config.yaml` & `pupil_labs_realtime_api-1.2.1/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-yaml
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.37.3
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
         name: PyUpgrade 3.7+
         args: ["--py37-plus"]
         exclude: ^bin/
 
   - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
-    - id: flake8
+      - id: flake8
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         args: [--profile, black]
 
   - repo: https://github.com/psf/black
-    rev: 22.8.0
+    rev: 22.12.0
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.0.0
+    rev: v2.2.0
     hooks:
       - id: setup-cfg-fmt
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/CHANGES.rst` & `pupil_labs_realtime_api-1.2.1/CHANGES.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+1.2.1
+###########
+- Add typing annotations for various gaze data types
+
+1.2.0
+###########
+- Add support for streaming eye state data from Neon Companion app (2.8.8+)
+
+    - :py:class:`pupil_labs.realtime_api.streaming.gaze.EyestateGazeData`
+
+1.1.2
+###########
+- Add support for streaming eyes video from Neon Companion app
+
+  - Simple API
+
+    - :py:func:`pupil_labs.realtime_api.simple.Device.receive_eyes_video_frame`
+    - :py:func:`pupil_labs.realtime_api.simple.Device.receive_matched_scene_and_eyes_video_frames_and_gaze`
+
+  - Async API
+
+    - :py:func:`pupil_labs.realtime_api.models.Status.direct_eyes_sensor`, providing an
+      url that can be used with :py:func:`pupil_labs.realtime_api.streaming.video.receive_video_frames`
+
+- Add async support for streaming IMU from Neon Companion app
+
+  - Async API
+
+    - :py:func:`pupil_labs.realtime_api.streaming.imu.receive_imu_data`
+
+1.1.1
+#####
+- Use ``numpy.typing`` instead of ``nptyping``
+- Add :ref:`simple_vs_async_api_guide` guide
+
 1.1.0
 #####
 
 - Rename ``pupil_labs.realtime_api.clock_echo`` to :py:mod:`pupil_labs.realtime_api.time_echo`
   and all corresponding class and function prefixes.
 - Expose Time Echo port via :py:attr:`pupil_labs.realtime_api.models.Phone.time_echo_port`
 - Add simple API to estimate time offset :py:func:`pupil_labs.realtime_api.simple.Device.estimate_time_offset`
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/LICENSE` & `pupil_labs_realtime_api-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/README.rst` & `pupil_labs_realtime_api-1.2.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/pupil-labs-realtime-api/badge/?version=latest
    :target: https://pupil-labs-realtime-api.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2022-informational
    :target: https://blog.jaraco.com/skeleton
 
 *******************************
 Pupil Labs' Realtime API Client
 *******************************
 
 - `Documentation <https://pupil-labs-realtime-api.readthedocs.io/>`_
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/docs/api/async.rst` & `pupil_labs_realtime_api-1.2.1/docs/api/async.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,24 +15,35 @@
 ==============
 
 .. automodule:: pupil_labs.realtime_api.device
     :members:
     :undoc-members:
     :show-inheritance:
 
+.. _streaming_api:
+
 Streaming
 =========
 
 Gaze Data
 ---------
 
 .. automodule:: pupil_labs.realtime_api.streaming.gaze
     :members:
     :undoc-members:
     :show-inheritance:
+    :exclude-members: DualMonocularGazeData
+
+IMU Data
+---------
+
+.. automodule:: pupil_labs.realtime_api.streaming.imu
+    :members:
+    :undoc-members:
+    :show-inheritance:
 
 Scene Video
 -----------
 
 .. automodule:: pupil_labs.realtime_api.streaming.video
     :members:
     :undoc-members:
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/docs/examples/async.rst` & `pupil_labs_realtime_api-1.2.1/docs/examples/async.rst`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,22 @@
 ------------------
 
 .. literalinclude:: ../../examples/async/stream_scene_camera_video.py
    :language: python
    :emphasize-lines: 18,24-26
    :linenos:
 
+Eyes Camera Video
+------------------
+
+.. literalinclude:: ../../examples/async/stream_eyes_camera_video.py
+   :language: python
+   :emphasize-lines: 20,28
+   :linenos:
+
 .. _stream_video_with_overlayed_gaze_example:
 
 Scene Camera Video With Overlayed Gaze
 --------------------------------------
 
 This example processes two streams (video and gaze data) at the same time, matches each
 video frame with its temporally closest gaze point, and previews both in a window.
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/docs/examples/simple.rst` & `pupil_labs_realtime_api-1.2.1/docs/examples/simple.rst`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 .. literalinclude:: ../../examples/simple/discover_devices.py
    :language: python
    :linenos:
 
 Remote control devices
 ======================
 
+.. _simple_get_status_example:
+
 Get current status
 ------------------
 
 .. literalinclude:: ../../examples/simple/get_status.py
    :language: python
    :linenos:
 
@@ -44,15 +46,15 @@
 ----------
 
 An event without an explicit timestamp, will be timestamped on arrival at the Pupil
 Invisible Companion device.
 
 .. literalinclude:: ../../examples/simple/send_event.py
    :language: python
-   :emphasize-lines: 12,15
+   :emphasize-lines: 12,16-19,24,25,29,30,32-34
    :linenos:
 
 Start, stop and save, and cancel recordings
 -------------------------------------------
 
 .. literalinclude:: ../../examples/simple/start_stop_recordings.py
    :language: python
@@ -75,24 +77,55 @@
 ------------------
 
 .. literalinclude:: ../../examples/simple/stream_scene_camera_video.py
    :language: python
    :emphasize-lines: 18
    :linenos:
 
+Eyes camera video
+-----------------
+
+.. note:: Only available when connecting to a Neon Companion app
+
+.. literalinclude:: ../../examples/simple/stream_eyes_camera_video.py
+   :language: python
+   :emphasize-lines: 18
+   :linenos:
+
+Camera calibration
+------------------
+
+.. note:: Only available when connecting to a Neon Companion app
+
+.. literalinclude:: ../../examples/simple/camera_calibration.py
+   :language: python
+   :emphasize-lines: 12
+   :linenos:
+
+
 .. _stream_video_with_overlayed_gaze_example_simple:
 
 Scene camera video with overlayed gaze
 --------------------------------------
 
 .. literalinclude:: ../../examples/simple/stream_video_with_overlayed_gaze.py
    :language: python
    :emphasize-lines: 18,20,21
    :linenos:
 
+Scene camera video with overlayed eyes video and gaze circle
+------------------------------------------------------------
+
+.. note:: Only available when connecting to a Neon Companion app
+
+.. literalinclude:: ../../examples/simple/stream_scene_eyes_and_gaze.py
+   :language: python
+   :emphasize-lines: 18,27,35-36
+   :linenos:
+
 Time Offset Estimation
 ======================
 
 See :py:mod:`pupil_labs.realtime_api.time_echo` for details.
 
 .. literalinclude:: ../../examples/simple/device_time_offset.py
    :language: python
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/docs/guides/under-the-hood.rst` & `pupil_labs_realtime_api-1.2.1/docs/guides/under-the-hood.rst`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/docs/index.rst` & `pupil_labs_realtime_api-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_get_current.py` & `pupil_labs_realtime_api-1.2.1/examples/async/device_status_get_current.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_update_via_callback.py` & `pupil_labs_realtime_api-1.2.1/examples/async/device_status_update_via_callback.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/async/device_status_update_wait.py` & `pupil_labs_realtime_api-1.2.1/examples/async/device_status_update_wait.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/async/device_time_offset.py` & `pupil_labs_realtime_api-1.2.1/examples/async/device_time_offset.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/async/discover_devices.py` & `pupil_labs_realtime_api-1.2.1/examples/async/discover_devices.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/async/send_event.py` & `pupil_labs_realtime_api-1.2.1/examples/async/send_event.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/async/start_stop_recordings.py` & `pupil_labs_realtime_api-1.2.1/examples/async/start_stop_recordings.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/async/stream_gaze.py` & `pupil_labs_realtime_api-1.2.1/examples/async/stream_gaze.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/async/stream_scene_camera_video.py` & `pupil_labs_realtime_api-1.2.1/examples/async/stream_scene_camera_video.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/async/stream_video_with_overlayed_gaze.py` & `pupil_labs_realtime_api-1.2.1/examples/async/stream_video_with_overlayed_gaze.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/simple/device_time_offset.py` & `pupil_labs_realtime_api-1.2.1/examples/simple/device_time_offset.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/simple/get_status.py` & `pupil_labs_realtime_api-1.2.1/examples/simple/get_status.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/simple/start_stop_recordings.py` & `pupil_labs_realtime_api-1.2.1/examples/simple/start_stop_recordings.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/simple/status_auto_update.py` & `pupil_labs_realtime_api-1.2.1/examples/simple/status_auto_update.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_gaze.py` & `pupil_labs_realtime_api-1.2.1/examples/simple/stream_gaze.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_scene_camera_video.py` & `pupil_labs_realtime_api-1.2.1/examples/simple/stream_scene_camera_video.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/examples/simple/stream_video_with_overlayed_gaze.py` & `pupil_labs_realtime_api-1.2.1/examples/simple/stream_video_with_overlayed_gaze.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/__init__.py` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """pupil_labs.realtime_api"""
 
 # .version is generated on install via setuptools_scm, see pyproject.toml
 from .device import APIPath, Device, DeviceError, StatusUpdateNotifier
 from .discovery import Network, discover_devices
 from .streaming import (
+    DualMonocularGazeData,
+    EyestateGazeData,
     GazeData,
     RTSPData,
     RTSPGazeStreamer,
+    RTSPImuStreamer,
     RTSPRawStreamer,
     RTSPVideoFrameStreamer,
     VideoFrame,
     receive_gaze_data,
+    receive_imu_data,
     receive_raw_rtsp_data,
     receive_video_frames,
 )
 
 try:
     from importlib.metadata import PackageNotFoundError, version
 except ImportError:
@@ -23,24 +27,28 @@
 try:
     __version__ = version("pupil_labs.realtime_api")
 except PackageNotFoundError:
     __version__ = "unknown"
 
 __all__ = [
     "__version__",
-    "__version_info__",
     "APIPath",
     "Device",
     "DeviceError",
     "discover_devices",
     "GazeData",
+    "DualMonocularGazeData",
+    "EyestateGazeData",
     "Network",
     "receive_gaze_data",
     "receive_raw_rtsp_data",
     "receive_video_frames",
     "RTSPData",
     "RTSPGazeStreamer",
     "RTSPRawStreamer",
     "RTSPVideoFrameStreamer",
     "StatusUpdateNotifier",
     "VideoFrame",
+    "receive_imu_data",
+    "RTSPImuStreamer",
+    "imu_pb2",
 ]
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/base.py` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/base.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/discovery.py` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/discovery.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import logging
 import time
 import types
 import typing as T
 
-import click
 from zeroconf import ServiceStateChange
 from zeroconf.asyncio import AsyncServiceBrowser, AsyncServiceInfo, AsyncZeroconf
 
 from .models import DiscoveredDeviceInfo
 
 logger = logging.getLogger(__name__)
 
@@ -70,15 +69,15 @@
     ):
         info = AsyncServiceInfo(service_type, name)
         if await info.async_request(zeroconf, timeout_ms):
             device = DiscoveredDeviceInfo(
                 name,
                 info.server,
                 info.port,
-                ['.'.join([str(symbol) for symbol in addr]) for addr in info.addresses],
+                [".".join([str(symbol) for symbol in addr]) for addr in info.addresses],
             )
             self._devices[name] = device
             await self._new_devices.put(device)
 
     async def __aenter__(self) -> "Network":
         return self
 
@@ -111,23 +110,7 @@
                 yield device
             if timeout_seconds is not None:
                 timeout_seconds -= time.perf_counter() - t0
 
 
 def is_valid_service_name(name: str) -> bool:
     return name.split(":")[0] == "PI monitor"
-
-
-@click.command()
-@click.option("-t", "--search-duration", type=float)
-def cli(search_duration: T.Optional[float] = None):
-    async def print_devices():
-        from rich import print
-
-        async for dev in discover_devices(timeout_seconds=search_duration):
-            print(dev)
-
-    asyncio.run(print_devices())
-
-
-if __name__ == "__main__":
-    cli()
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/models.py` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class APIPath(enum.Enum):
     STATUS = "/status"
     RECORDING_START = "/recording:start"
     RECORDING_STOP_AND_SAVE = "/recording:stop_and_save"
     RECORDING_CANCEL = "/recording:cancel"
     EVENT = "/event"
-    CAMERA_CONTROL = "/camera_control"
+    CALIBRATION = "/../calibration.bin"
 
     def full_address(
         self, address: str, port: int, protocol: str = "http", prefix: str = "/api"
     ) -> str:
         return f"{protocol}://{address}:{port}" + prefix + self.value
 
 
@@ -77,14 +77,15 @@
     time_echo_port: T.Optional[int] = None
 
 
 class Hardware(T.NamedTuple):
     version: str = "unknown"
     glasses_serial: str = "unknown"
     world_camera_serial: str = "unknown"
+    module_serial: str = "unknown"
 
 
 class NetworkDevice(T.NamedTuple):
     """Information about devices discovered by the host device, not the client.
 
     .. note::
         This class represents device information made available via the websocket update
@@ -117,14 +118,16 @@
             return f"{self.protocol}://{self.ip}:{self.port}/?{self.params}"
         return None
 
     class Name(enum.Enum):
         ANY = None
         GAZE = "gaze"
         WORLD = "world"
+        IMU = "imu"
+        EYES = "eyes"
 
     class Connection(enum.Enum):
         ANY = None
         WEBSOCKET = "WEBSOCKET"
         DIRECT = "DIRECT"
 
 
@@ -256,7 +259,23 @@
     def direct_gaze_sensor(self) -> T.Optional[Sensor]:
         return next(
             self.matching_sensors(Sensor.Name.GAZE, Sensor.Connection.DIRECT),
             Sensor(
                 sensor=Sensor.Name.GAZE.value, conn_type=Sensor.Connection.DIRECT.value
             ),
         )
+
+    def direct_imu_sensor(self) -> T.Optional[Sensor]:
+        return next(
+            self.matching_sensors(Sensor.Name.IMU, Sensor.Connection.DIRECT),
+            Sensor(
+                sensor=Sensor.Name.IMU.value, conn_type=Sensor.Connection.DIRECT.value
+            ),
+        )
+
+    def direct_eyes_sensor(self) -> T.Optional[Sensor]:
+        return next(
+            self.matching_sensors(Sensor.Name.EYES, Sensor.Connection.DIRECT),
+            Sensor(
+                sensor=Sensor.Name.EYES.value, conn_type=Sensor.Connection.DIRECT.value
+            ),
+        )
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/device.py` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/simple/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,31 @@
     # FIXME: Remove when dropping py3.7 support
     from typing_extensions import Literal
 
 from ..base import DeviceBase
 from ..device import Device as _DeviceAsync
 from ..device import StatusUpdateNotifier
 from ..models import Component, Event, Sensor, Status
-from ..streaming import GazeData, RTSPGazeStreamer, RTSPVideoFrameStreamer
+from ..streaming import (
+    ImuPacket,
+    RTSPGazeStreamer,
+    RTSPImuStreamer,
+    RTSPVideoFrameStreamer,
+)
 from ..time_echo import TimeEchoEstimates, TimeOffsetEstimator
 from ._utils import _AsyncEventManager, _StreamManager, logger
-from .models import MATCHED_ITEM_LABEL, MatchedItem, SimpleVideoFrame, VideoFrame
+from .models import (
+    MATCHED_GAZE_EYES_LABEL,
+    MATCHED_ITEM_LABEL,
+    GazeDataType,
+    MatchedGazeEyesSceneItem,
+    MatchedItem,
+    SimpleVideoFrame,
+    VideoFrame,
+)
 
 
 class Device(DeviceBase):
     """
     .. hint::
         Use :py:func:`pupil_labs.realtime_api.simple.discover_devices` instead of
         initializing the class manually. See the :ref:`simple_discovery_example`
@@ -77,14 +90,19 @@
         return self._status.phone.memory_state
 
     @property
     def version_glasses(self) -> str:
         return self._status.hardware.version
 
     @property
+    def module_serial(self) -> T.Union[str, None, Literal["default"]]:
+        """Returns ``None`` or ``"default"`` if no glasses are connected"""
+        return self._status.hardware.module_serial
+
+    @property
     def serial_number_glasses(self) -> T.Union[str, None, Literal["default"]]:
         """Returns ``None`` or ``"default"`` if no glasses are connected"""
         return self._status.hardware.glasses_serial
 
     @property
     def serial_number_scene_cam(self) -> T.Optional[str]:
         """Returns ``None`` if no scene camera is connected"""
@@ -92,14 +110,21 @@
 
     def world_sensor(self) -> T.Optional[Sensor]:
         return self._status.direct_world_sensor()
 
     def gaze_sensor(self) -> T.Optional[Sensor]:
         return self._status.direct_gaze_sensor()
 
+    def get_calibration(self):
+        async def _get_calibration():
+            async with _DeviceAsync.convert_from(self) as control:
+                return await control.get_calibration()
+
+        return asyncio.run(_get_calibration())
+
     def recording_start(self) -> str:
         """Wraps :py:meth:`pupil_labs.realtime_api.device.Device.recording_start`
 
         :raises pupil_labs.realtime_api.device.DeviceError:
             if the recording could not be started. Possible reasons include
             - Recording already running
             - Template has required fields
@@ -164,25 +189,40 @@
     def receive_scene_video_frame(
         self, timeout_seconds: T.Optional[float] = None
     ) -> T.Optional[SimpleVideoFrame]:
         return self._receive_item(Sensor.Name.WORLD.value, timeout_seconds)
 
     def receive_gaze_datum(
         self, timeout_seconds: T.Optional[float] = None
-    ) -> T.Optional[GazeData]:
+    ) -> T.Optional[GazeDataType]:
         return self._receive_item(Sensor.Name.GAZE.value, timeout_seconds)
 
+    def receive_eyes_video_frame(
+        self, timeout_seconds: T.Optional[float] = None
+    ) -> T.Optional[SimpleVideoFrame]:
+        return self._receive_item(Sensor.Name.EYES.value, timeout_seconds)
+
+    def receive_imu_datum(
+        self, timeout_seconds: T.Optional[float] = None
+    ) -> T.Optional[ImuPacket]:
+        return self._receive_item(Sensor.Name.IMU.value, timeout_seconds)
+
     def receive_matched_scene_video_frame_and_gaze(
         self, timeout_seconds: T.Optional[float] = None
     ) -> T.Optional[MatchedItem]:
         return self._receive_item(MATCHED_ITEM_LABEL, timeout_seconds)
 
+    def receive_matched_scene_and_eyes_video_frames_and_gaze(
+        self, timeout_seconds: T.Optional[float] = None
+    ) -> T.Optional[MatchedGazeEyesSceneItem]:
+        return self._receive_item(MATCHED_GAZE_EYES_LABEL, timeout_seconds)
+
     def _receive_item(
         self, sensor: str, timeout_seconds: T.Optional[float] = None
-    ) -> T.Optional[T.Union[VideoFrame, GazeData]]:
+    ) -> T.Optional[T.Union[VideoFrame, GazeDataType]]:
         if not self.is_currently_streaming:
             logger.debug("receive_* called without being streaming")
             self.streaming_start()
         try:
             return self._most_recent_item[sensor].popleft()
         except IndexError:
             # no cached frame available, waiting for new one
@@ -253,23 +293,28 @@
         self._event_manager = None
         self._background_loop = None
 
         # List of sensors that will
         sensor_names = [
             Sensor.Name.GAZE.value,
             Sensor.Name.WORLD.value,
+            Sensor.Name.EYES.value,
+            Sensor.Name.IMU.value,
             MATCHED_ITEM_LABEL,
+            MATCHED_GAZE_EYES_LABEL,
         ]
         self._most_recent_item = {
             name: collections.deque(maxlen=1) for name in sensor_names
         }
         self._event_new_item = {name: threading.Event() for name in sensor_names}
         # only cache 3-4 seconds worth of gaze data in case no scene camera is connected
-        GazeCacheType = T.Deque[T.Tuple[float, GazeData]]
+        GazeCacheType = T.Deque[T.Tuple[float, GazeDataType]]
+        EyesCacheType = T.Deque[T.Tuple[float, SimpleVideoFrame]]
         self._cached_gaze_for_matching: GazeCacheType = collections.deque(maxlen=200)
+        self._cached_eyes_for_matching: EyesCacheType = collections.deque(maxlen=200)
 
         event_auto_update_started = threading.Event()
         self._is_streaming_flag = threading.Event()
         self._auto_update_thread = threading.Thread(
             target=self._auto_update,
             kwargs=dict(
                 device_weakref=weakref.ref(self),  # weak ref to avoid cycling ref
@@ -310,14 +355,24 @@
                 should_be_streaming_by_default=start_streaming_by_default,
             ),
             Sensor.Name.WORLD.value: _StreamManager(
                 device_weakref,
                 RTSPVideoFrameStreamer,
                 should_be_streaming_by_default=start_streaming_by_default,
             ),
+            Sensor.Name.EYES.value: _StreamManager(
+                device_weakref,
+                RTSPVideoFrameStreamer,
+                should_be_streaming_by_default=start_streaming_by_default,
+            ),
+            Sensor.Name.IMU.value: _StreamManager(
+                device_weakref,
+                RTSPImuStreamer,
+                should_be_streaming_by_default=start_streaming_by_default,
+            ),
         }
 
         async def _process_status_changes(changed: Component):
             if (
                 isinstance(changed, Sensor)
                 and changed.conn_type == Sensor.Connection.DIRECT.value
             ):
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/simple/discovery.py` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/simple/discovery.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/base.py` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/base.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/nal_unit.py` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/nal_unit.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/streaming/video.py` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/streaming/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import base64
 import datetime
 import logging
 import typing as T
 
 import av
-import nptyping as npt
+import numpy as np
+import numpy.typing as npt
 
 from .base import RTSPRawStreamer, SDPDataNotAvailableError
 from .nal_unit import extract_payload_from_nal_unit
 
 logger = logging.getLogger(__name__)
 
-BGRBuffer = npt.NDArray[(1080, 1088, 3), npt.UInt8]
+BGRBuffer = npt.NDArray[np.uint8]
 """Type annotation for raw BGR image buffers of the scene camera"""
 
 
 class VideoFrame(T.NamedTuple):
     av_frame: av.VideoFrame
     timestamp_unix_seconds: float
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs/realtime_api/time_echo.py` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs/realtime_api/time_echo.py`

 * *Files identical despite different names*

### Comparing `pupil_labs_realtime_api-1.2.0a3/src/pupil_labs_realtime_api.egg-info/SOURCES.txt` & `pupil_labs_realtime_api-1.2.1/src/pupil_labs_realtime_api.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 CHANGES.rst
 LICENSE
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
-setup.py
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 docs/api/async.rst
@@ -23,53 +22,58 @@
 docs/api/index.rst
 docs/api/models.rst
 docs/api/simple.rst
 docs/examples/async.rst
 docs/examples/index.rst
 docs/examples/simple.rst
 docs/guides/index.rst
+docs/guides/simple-vs-async-api.rst
 docs/guides/under-the-hood.rst
-examples/async/device_camera_controls.py
 examples/async/device_status_get_current.py
 examples/async/device_status_update_via_callback.py
 examples/async/device_status_update_wait.py
 examples/async/device_time_offset.py
 examples/async/discover_devices.py
 examples/async/send_event.py
 examples/async/start_stop_recordings.py
+examples/async/stream_eyes_camera_video.py
 examples/async/stream_gaze.py
+examples/async/stream_imu.py
 examples/async/stream_scene_camera_video.py
 examples/async/stream_video_with_overlayed_gaze.py
+examples/simple/camera_calibration.py
 examples/simple/device_time_offset.py
 examples/simple/discover_devices.py
 examples/simple/get_status.py
 examples/simple/send_event.py
 examples/simple/start_stop_recordings.py
 examples/simple/status_auto_update.py
+examples/simple/stream_eyes_camera_video.py
 examples/simple/stream_gaze.py
+examples/simple/stream_imu.py
 examples/simple/stream_scene_camera_video.py
+examples/simple/stream_scene_eyes_and_gaze.py
 examples/simple/stream_video_with_overlayed_gaze.py
 src/pupil_labs/realtime_api/__init__.py
 src/pupil_labs/realtime_api/base.py
-src/pupil_labs/realtime_api/camera_control.py
 src/pupil_labs/realtime_api/device.py
 src/pupil_labs/realtime_api/discovery.py
 src/pupil_labs/realtime_api/models.py
 src/pupil_labs/realtime_api/time_echo.py
 src/pupil_labs/realtime_api/simple/__init__.py
 src/pupil_labs/realtime_api/simple/_utils.py
 src/pupil_labs/realtime_api/simple/device.py
 src/pupil_labs/realtime_api/simple/discovery.py
 src/pupil_labs/realtime_api/simple/models.py
 src/pupil_labs/realtime_api/streaming/__init__.py
 src/pupil_labs/realtime_api/streaming/base.py
 src/pupil_labs/realtime_api/streaming/gaze.py
+src/pupil_labs/realtime_api/streaming/imu.py
+src/pupil_labs/realtime_api/streaming/imu_pb2.py
 src/pupil_labs/realtime_api/streaming/nal_unit.py
 src/pupil_labs/realtime_api/streaming/video.py
 src/pupil_labs_realtime_api.egg-info/PKG-INFO
 src/pupil_labs_realtime_api.egg-info/SOURCES.txt
 src/pupil_labs_realtime_api.egg-info/dependency_links.txt
-src/pupil_labs_realtime_api.egg-info/entry_points.txt
 src/pupil_labs_realtime_api.egg-info/requires.txt
 src/pupil_labs_realtime_api.egg-info/top_level.txt
-tests/test_api.py
-tests/test_controls.py
+tests/test_api.py
```

### Comparing `pupil_labs_realtime_api-1.2.0a3/tox.ini` & `pupil_labs_realtime_api-1.2.1/tox.ini`

 * *Files identical despite different names*

