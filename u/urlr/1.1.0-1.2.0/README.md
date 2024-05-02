# Comparing `tmp/urlr-1.1.0.tar.gz` & `tmp/urlr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlr-1.1.0.tar", last modified: Tue Feb 13 12:54:18 2024, max compression
+gzip compressed data, was "urlr-1.2.0.tar", last modified: Thu May  2 18:44:43 2024, max compression
```

## Comparing `urlr-1.1.0.tar` & `urlr-1.2.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-02-13 12:54:18.982986 urlr-1.1.0/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      409 2024-02-13 12:54:18.982986 urlr-1.1.0/PKG-INFO
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     4037 2024-02-13 12:53:10.000000 urlr-1.1.0/README.md
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1875 2024-02-13 12:53:10.000000 urlr-1.1.0/pyproject.toml
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)       69 2024-02-13 12:54:18.982986 urlr-1.1.0/setup.cfg
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1200 2024-02-13 12:53:10.000000 urlr-1.1.0/setup.py
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-02-13 12:54:18.978986 urlr-1.1.0/test/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1494 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_authentification200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1544 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_authentification401_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      771 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_authentification_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1480 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_authentification_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1596 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_folder200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1571 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_folder200_response_folders_inner.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      701 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_folder_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1354 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_folder_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      696 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_link_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1610 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_reduce_link200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1481 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_reduce_link400_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1624 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_reduce_link_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1399 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_stats200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1390 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_stats400_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      699 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_stats_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1499 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_stats_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1549 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_team200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1510 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_team200_response_teams_inner.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      685 2024-02-13 12:53:10.000000 urlr-1.1.0/test/test_team_api.py
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-02-13 12:54:18.979986 urlr-1.1.0/urlr/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1953 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/__init__.py
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-02-13 12:54:18.980986 urlr-1.1.0/urlr/api/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      268 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/api/__init__.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11965 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/api/authentification_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11562 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/api/folder_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11798 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/api/link_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11683 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/api/stats_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     9928 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/api/team_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    25699 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/api_client.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      652 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/api_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    14738 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/configuration.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     5940 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/exceptions.py
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-02-13 12:54:18.981986 urlr-1.1.0/urlr/models/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1279 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/__init__.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2510 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/authentification200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2611 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/authentification401_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2686 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/authentification_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2987 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/folder200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2688 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/folder200_response_folders_inner.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2486 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/folder_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3386 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/reduce_link200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2827 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/reduce_link400_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3745 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/reduce_link_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2695 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/stats200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2548 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/stats400_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3373 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/stats_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2945 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/team200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2668 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/models/team200_response_teams_inner.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-02-13 07:55:59.000000 urlr-1.1.0/urlr/py.typed
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     9190 2024-02-13 12:53:10.000000 urlr-1.1.0/urlr/rest.py
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-02-13 12:54:18.982986 urlr-1.1.0/urlr.egg-info/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      409 2024-02-13 12:54:18.000000 urlr-1.1.0/urlr.egg-info/PKG-INFO
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1617 2024-02-13 12:54:18.000000 urlr-1.1.0/urlr.egg-info/SOURCES.txt
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        1 2024-02-13 12:54:18.000000 urlr-1.1.0/urlr.egg-info/dependency_links.txt
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)       76 2024-02-13 12:54:18.000000 urlr-1.1.0/urlr.egg-info/requires.txt
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        5 2024-02-13 12:54:18.000000 urlr-1.1.0/urlr.egg-info/top_level.txt
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.535401 urlr-1.2.0/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      409 2024-05-02 18:44:43.535401 urlr-1.2.0/PKG-INFO
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     4037 2024-05-02 18:42:46.000000 urlr-1.2.0/README.md
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1875 2024-05-02 18:42:46.000000 urlr-1.2.0/pyproject.toml
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)       69 2024-05-02 18:44:43.535401 urlr-1.2.0/setup.cfg
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1200 2024-05-02 18:42:46.000000 urlr-1.2.0/setup.py
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.531401 urlr-1.2.0/test/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1494 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_authentification200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1544 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_authentification401_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      771 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_authentification_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1480 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_authentification_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1596 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_folder200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1571 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_folder200_response_folders_inner.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      701 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_folder_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1354 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_folder_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      696 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_link_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1610 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_reduce_link200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1481 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_reduce_link400_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1624 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_reduce_link_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1399 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_stats200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1390 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_stats400_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      699 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_stats_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1499 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_stats_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1549 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_team200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1510 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_team200_response_teams_inner.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      685 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_team_api.py
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.532401 urlr-1.2.0/urlr/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1953 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/__init__.py
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.533401 urlr-1.2.0/urlr/api/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      268 2024-02-13 12:53:10.000000 urlr-1.2.0/urlr/api/__init__.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11979 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api/authentification_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11576 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api/folder_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11812 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api/link_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11697 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api/stats_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     9942 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api/team_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    26250 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api_client.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      652 2024-02-13 12:53:10.000000 urlr-1.2.0/urlr/api_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    14738 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/configuration.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     5940 2024-02-13 12:53:10.000000 urlr-1.2.0/urlr/exceptions.py
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.534401 urlr-1.2.0/urlr/models/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1279 2024-02-13 12:53:10.000000 urlr-1.2.0/urlr/models/__init__.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2523 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/authentification200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2624 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/authentification401_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2699 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/authentification_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3000 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/folder200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2701 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/folder200_response_folders_inner.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2499 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/folder_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3399 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/reduce_link200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2840 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/reduce_link400_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3758 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/reduce_link_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2708 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/stats200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2561 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/stats400_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3386 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/stats_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2958 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/team200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2681 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/team200_response_teams_inner.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-02-13 07:55:59.000000 urlr-1.2.0/urlr/py.typed
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     9366 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/rest.py
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.534401 urlr-1.2.0/urlr.egg-info/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      409 2024-05-02 18:44:43.000000 urlr-1.2.0/urlr.egg-info/PKG-INFO
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1617 2024-05-02 18:44:43.000000 urlr-1.2.0/urlr.egg-info/SOURCES.txt
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        1 2024-05-02 18:44:43.000000 urlr-1.2.0/urlr.egg-info/dependency_links.txt
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)       76 2024-05-02 18:44:43.000000 urlr-1.2.0/urlr.egg-info/requires.txt
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        5 2024-05-02 18:44:43.000000 urlr-1.2.0/urlr.egg-info/top_level.txt
```

### Comparing `urlr-1.1.0/README.md` & `urlr-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# urlr@1.1.0
+# urlr@1.2.0
 
 ![PyPI - Version](https://img.shields.io/pypi/v/urlr) ![PyPI - Downloads](https://img.shields.io/pypi/dm/urlr) ![PyPI - License](https://img.shields.io/pypi/l/urlr)
 
 This SDK is automatically generated with the [OpenAPI Generator](https://openapi-generator.tech) project.
 
 - API version: 0.3
-- Package version: 1.1.0
+- Package version: 1.2.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://urlr.me/en](https://urlr.me/en)
 
 ## Installation & Usage
 
 ## Requirements
```

### Comparing `urlr-1.1.0/pyproject.toml` & `urlr-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "urlr"
-version = "1.1.0"
+version = "1.2.0"
 description = "Python client for URLR"
 authors = ["URLR <contact@urlr.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/urlr/urlr-python"
 keywords = ["link shortener", "api", "sdk", "client"]
 include = ["urlr/py.typed"]
```

### Comparing `urlr-1.1.0/setup.py` & `urlr-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "urlr"
-VERSION = "1.1.0"
+VERSION = "1.2.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `urlr-1.1.0/test/test_authentification200_response.py` & `urlr-1.2.0/test/test_authentification200_response.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_authentification401_response.py` & `urlr-1.2.0/test/test_authentification401_response.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_authentification_api.py` & `urlr-1.2.0/test/test_authentification_api.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_authentification_request.py` & `urlr-1.2.0/test/test_authentification_request.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_folder200_response.py` & `urlr-1.2.0/test/test_folder200_response.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_folder200_response_folders_inner.py` & `urlr-1.2.0/test/test_folder200_response_folders_inner.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_folder_api.py` & `urlr-1.2.0/test/test_folder_api.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_folder_request.py` & `urlr-1.2.0/test/test_folder_request.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_link_api.py` & `urlr-1.2.0/test/test_link_api.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_reduce_link200_response.py` & `urlr-1.2.0/test/test_reduce_link200_response.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_reduce_link400_response.py` & `urlr-1.2.0/test/test_reduce_link400_response.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_reduce_link_request.py` & `urlr-1.2.0/test/test_reduce_link_request.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_stats200_response.py` & `urlr-1.2.0/test/test_stats200_response.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_stats400_response.py` & `urlr-1.2.0/test/test_stats400_response.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_stats_api.py` & `urlr-1.2.0/test/test_stats_api.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_stats_request.py` & `urlr-1.2.0/test/test_stats_request.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_team200_response.py` & `urlr-1.2.0/test/test_team200_response.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_team200_response_teams_inner.py` & `urlr-1.2.0/test/test_team200_response_teams_inner.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/test/test_team_api.py` & `urlr-1.2.0/test/test_team_api.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/urlr/__init__.py` & `urlr-1.2.0/urlr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 # import apis into sdk package
 from urlr.api.authentification_api import AuthentificationApi
 from urlr.api.folder_api import FolderApi
 from urlr.api.link_api import LinkApi
 from urlr.api.stats_api import StatsApi
 from urlr.api.team_api import TeamApi
```

### Comparing `urlr-1.1.0/urlr/api/authentification_api.py` & `urlr-1.2.0/urlr/api/authentification_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
```

### Comparing `urlr-1.1.0/urlr/api/folder_api.py` & `urlr-1.2.0/urlr/api/folder_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
```

### Comparing `urlr-1.1.0/urlr/api/link_api.py` & `urlr-1.2.0/urlr/api/link_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
```

### Comparing `urlr-1.1.0/urlr/api/stats_api.py` & `urlr-1.2.0/urlr/api/stats_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
```

### Comparing `urlr-1.1.0/urlr/api/team_api.py` & `urlr-1.2.0/urlr/api/team_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
```

### Comparing `urlr-1.1.0/urlr/api_client.py` & `urlr-1.2.0/urlr/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 import json
 import mimetypes
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
-from typing import Tuple, Optional, List, Dict
+from typing import Tuple, Optional, List, Dict, Union
+from pydantic import SecretStr
 
 from urlr.configuration import Configuration
 from urlr.api_response import ApiResponse, T as ApiResponseT
 import urlr.models
 from urlr import rest
 from urlr.exceptions import (
     ApiValueError,
@@ -84,15 +85,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.1.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.2.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
@@ -204,15 +205,16 @@
         if post_params or files:
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(
                 post_params,
                 collection_formats
             )
-            post_params.extend(self.files_parameters(files))
+            if files:
+                post_params.extend(self.files_parameters(files))
 
         # auth setting
         self.update_params_for_auth(
             header_params,
             query_params,
             auth_settings,
             resource_path,
@@ -309,15 +311,18 @@
             elif response_type is not None:
                 match = None
                 content_type = response_data.getheader('content-type')
                 if content_type is not None:
                     match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
                 encoding = match.group(1) if match else "utf-8"
                 response_text = response_data.data.decode(encoding)
-                return_data = self.deserialize(response_text, response_type)
+                if response_type in ["bytearray", "str"]:
+                    return_data = self.__deserialize_primitive(response_text, response_type)
+                else:
+                    return_data = self.deserialize(response_text, response_type)
         finally:
             if not 200 <= response_data.status <= 299:
                 raise ApiException.from_response(
                     http_resp=response_data,
                     body=response_text,
                     data=return_data,
                 )
@@ -329,26 +334,31 @@
             raw_data = response_data.data
         )
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
+        If obj is SecretStr, return obj.get_secret_value()
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
             convert to string in iso8601 format.
         If obj is list, sanitize each element in the list.
         If obj is dict, return the dict.
         If obj is OpenAPI model, return the properties dict.
 
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
         if obj is None:
             return None
+        elif isinstance(obj, Enum):
+            return obj.value
+        elif isinstance(obj, SecretStr):
+            return obj.get_secret_value()
         elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
         elif isinstance(obj, list):
             return [
                 self.sanitize_for_serialization(sub_obj) for sub_obj in obj
             ]
         elif isinstance(obj, tuple):
@@ -362,15 +372,18 @@
             obj_dict = obj
         else:
             # Convert model obj to dict except
             # attributes `openapi_types`, `attribute_map`
             # and attributes which value is not None.
             # Convert attribute name to json key in
             # model definition for request.
-            obj_dict = obj.to_dict()
+            if hasattr(obj, 'to_dict') and callable(getattr(obj, 'to_dict')):
+                obj_dict = obj.to_dict()
+            else:
+                obj_dict = obj.__dict__
 
         return {
             key: self.sanitize_for_serialization(val)
             for key, val in obj_dict.items()
         }
 
     def deserialize(self, response_text, response_type):
@@ -501,39 +514,38 @@
                         (k, delimiter.join(quote(str(value)) for value in v))
                     )
             else:
                 new_params.append((k, quote(str(v))))
 
         return "&".join(["=".join(map(str, item)) for item in new_params])
 
-    def files_parameters(self, files=None):
+    def files_parameters(self, files: Dict[str, Union[str, bytes]]):
         """Builds form parameters.
 
         :param files: File parameters.
         :return: Form parameters with files.
         """
         params = []
-
-        if files:
-            for k, v in files.items():
-                if not v:
-                    continue
-                file_names = v if type(v) is list else [v]
-                for n in file_names:
-                    with open(n, 'rb') as f:
-                        filename = os.path.basename(f.name)
-                        filedata = f.read()
-                        mimetype = (
-                            mimetypes.guess_type(filename)[0]
-                            or 'application/octet-stream'
-                        )
-                        params.append(
-                            tuple([k, tuple([filename, filedata, mimetype])])
-                        )
-
+        for k, v in files.items():
+            if isinstance(v, str):
+                with open(v, 'rb') as f:
+                    filename = os.path.basename(f.name)
+                    filedata = f.read()
+            elif isinstance(v, bytes):
+                filename = k
+                filedata = v
+            else:
+                raise ValueError("Unsupported file value")
+            mimetype = (
+                mimetypes.guess_type(filename)[0]
+                or 'application/octet-stream'
+            )
+            params.append(
+                tuple([k, tuple([filename, filedata, mimetype])])
+            )
         return params
 
     def select_header_accept(self, accepts: List[str]) -> Optional[str]:
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
         :return: Accept (e.g. application/json).
```

### Comparing `urlr-1.1.0/urlr/api_response.py` & `urlr-1.2.0/urlr/api_response.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/urlr/configuration.py` & `urlr-1.2.0/urlr/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.3\n"\
-               "SDK Package Version: 1.1.0".\
+               "SDK Package Version: 1.2.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `urlr-1.1.0/urlr/exceptions.py` & `urlr-1.2.0/urlr/exceptions.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/urlr/models/__init__.py` & `urlr-1.2.0/urlr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `urlr-1.1.0/urlr/models/authentification200_response.py` & `urlr-1.2.0/urlr/models/authentification200_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Authentification200Response(BaseModel):
     """
     Authentification200Response
     """ # noqa: E501
     token: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["token"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/authentification401_response.py` & `urlr-1.2.0/urlr/models/authentification401_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Authentification401Response(BaseModel):
     """
     Authentification401Response
     """ # noqa: E501
     code: Optional[StrictInt] = None
     message: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["code", "message"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/authentification_request.py` & `urlr-1.2.0/urlr/models/authentification_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AuthentificationRequest(BaseModel):
     """
     AuthentificationRequest
     """ # noqa: E501
     username: Optional[StrictStr] = Field(default=None, description="Email")
     password: Optional[StrictStr] = Field(default=None, description="Password")
     __properties: ClassVar[List[str]] = ["username", "password"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/folder200_response.py` & `urlr-1.2.0/urlr/models/folder200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
 from urlr.models.folder200_response_folders_inner import Folder200ResponseFoldersInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Folder200Response(BaseModel):
     """
     Folder200Response
     """ # noqa: E501
     folders: Optional[List[Folder200ResponseFoldersInner]] = None
     __properties: ClassVar[List[str]] = ["folders"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/folder200_response_folders_inner.py` & `urlr-1.2.0/urlr/models/folder200_response_folders_inner.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Folder200ResponseFoldersInner(BaseModel):
     """
     Folder200ResponseFoldersInner
     """ # noqa: E501
     id: Optional[StrictInt] = Field(default=None, description="Folder ID")
     name: Optional[StrictStr] = Field(default=None, description="Folder name")
     __properties: ClassVar[List[str]] = ["id", "name"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/folder_request.py` & `urlr-1.2.0/urlr/models/folder_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
 class FolderRequest(BaseModel):
     """
     FolderRequest
     """ # noqa: E501
     team: StrictInt = Field(description="Team ID (displayed on dashboard)")
     __properties: ClassVar[List[str]] = ["team"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/reduce_link200_response.py` & `urlr-1.2.0/urlr/models/reduce_link200_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ReduceLink200Response(BaseModel):
     """
     ReduceLink200Response
@@ -32,19 +32,19 @@
     team: Optional[StrictInt] = Field(default=None, description="Team ID (displayed on dashboard)")
     folder: Optional[StrictInt] = Field(default=None, description="Folder ID (displayed on dashboard)")
     url_code: Optional[StrictStr] = Field(default=None, description="Short code")
     domain: Optional[StrictStr] = Field(default=None, description="Domain")
     code: Optional[StrictInt] = Field(default=None, description="HTTP status code")
     __properties: ClassVar[List[str]] = ["url", "expired_at", "team", "folder", "url_code", "domain", "code"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/reduce_link400_response.py` & `urlr-1.2.0/urlr/models/reduce_link400_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ReduceLink400Response(BaseModel):
     """
     ReduceLink400Response
     """ # noqa: E501
     code: Optional[StrictInt] = Field(default=None, description="HTTP status code")
     error: Optional[StrictInt] = Field(default=None, description="Error code")
     message: Optional[StrictStr] = Field(default=None, description="Message describing the error")
     __properties: ClassVar[List[str]] = ["code", "error", "message"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/reduce_link_request.py` & `urlr-1.2.0/urlr/models/reduce_link_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ReduceLinkRequest(BaseModel):
     """
@@ -43,19 +43,19 @@
         if value is None:
             return value
 
         if not re.match(r"^[a-zA-Z0-9!-]{3,50}$", value):
             raise ValueError(r"must validate the regular expression /^[a-zA-Z0-9!-]{3,50}$/")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/stats200_response.py` & `urlr-1.2.0/urlr/models/stats200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Stats200Response(BaseModel):
     """
     Stats200Response
     """ # noqa: E501
     clicks: Optional[StrictInt] = Field(default=None, description="Clicks")
     unique_clicks: Optional[StrictInt] = Field(default=None, description="Unique clicks", alias="uniqueClicks")
     __properties: ClassVar[List[str]] = ["clicks", "uniqueClicks"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/stats400_response.py` & `urlr-1.2.0/urlr/models/stats400_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Stats400Response(BaseModel):
     """
     Stats400Response
     """ # noqa: E501
     code: Optional[StrictInt] = None
     error: Optional[StrictInt] = None
     __properties: ClassVar[List[str]] = ["code", "error"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/stats_request.py` & `urlr-1.2.0/urlr/models/stats_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
 class StatsRequest(BaseModel):
     """
@@ -37,19 +37,19 @@
     @field_validator('code')
     def code_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if not re.match(r"^[a-zA-Z0-9!-]{3,50}$", value):
             raise ValueError(r"must validate the regular expression /^[a-zA-Z0-9!-]{3,50}$/")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/team200_response.py` & `urlr-1.2.0/urlr/models/team200_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
 from urlr.models.team200_response_teams_inner import Team200ResponseTeamsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Team200Response(BaseModel):
     """
     Team200Response
     """ # noqa: E501
     teams: Optional[List[Team200ResponseTeamsInner]] = None
     __properties: ClassVar[List[str]] = ["teams"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/models/team200_response_teams_inner.py` & `urlr-1.2.0/urlr/models/team200_response_teams_inner.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Team200ResponseTeamsInner(BaseModel):
     """
     Team200ResponseTeamsInner
     """ # noqa: E501
     id: Optional[StrictInt] = Field(default=None, description="Team ID")
     name: Optional[StrictStr] = Field(default=None, description="Team name")
     __properties: ClassVar[List[str]] = ["id", "name"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `urlr-1.1.0/urlr/rest.py` & `urlr-1.2.0/urlr/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,16 @@
                         preload_content=False
                     )
                 elif content_type == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers['Content-Type']
+                    # Ensures that dict objects are serialized
+                    post_params = [(a, json.dumps(b)) if isinstance(b, dict) else (a,b) for a, b in post_params]
                     r = self.pool_manager.request(
                         method,
                         url,
                         fields=post_params,
                         encode_multipart=True,
                         timeout=timeout,
                         headers=headers,
```

### Comparing `urlr-1.1.0/urlr.egg-info/SOURCES.txt` & `urlr-1.2.0/urlr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

