# Comparing `tmp/lokzzpylib-0.2.dev83.tar.gz` & `tmp/lokzzpylib-0.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokzzpylib-0.2.dev83.tar", last modified: Wed May  1 22:38:48 2024, max compression
+gzip compressed data, was "lokzzpylib-0.2.dev9.tar", last modified: Mon Jul  3 10:10:27 2023, max compression
```

## Comparing `lokzzpylib-0.2.dev83.tar` & `lokzzpylib-0.2.dev9.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 22:38:48.093910 lokzzpylib-0.2.dev83/
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-13 17:35:11.000000 lokzzpylib-0.2.dev83/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      508 2024-05-01 22:38:48.089910 lokzzpylib-0.2.dev83/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-13 17:35:11.000000 lokzzpylib-0.2.dev83/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 22:38:48.089910 lokzzpylib-0.2.dev83/lokzzpylib/
--rw-r--r--   0 root         (0) root         (0)     5080 2024-05-01 22:38:09.000000 lokzzpylib-0.2.dev83/lokzzpylib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 22:38:48.089910 lokzzpylib-0.2.dev83/lokzzpylib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      508 2024-05-01 22:38:48.000000 lokzzpylib-0.2.dev83/lokzzpylib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2024-05-01 22:38:48.000000 lokzzpylib-0.2.dev83/lokzzpylib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 22:38:48.000000 lokzzpylib-0.2.dev83/lokzzpylib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-05-01 22:38:48.000000 lokzzpylib-0.2.dev83/lokzzpylib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-01 22:38:48.000000 lokzzpylib-0.2.dev83/lokzzpylib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      681 2024-04-13 17:35:11.000000 lokzzpylib-0.2.dev83/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 22:38:48.093910 lokzzpylib-0.2.dev83/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:10:27.950512 lokzzpylib-0.2.dev9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:10:27.946512 lokzzpylib-0.2.dev9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:10:27.946512 lokzzpylib-0.2.dev9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 10:10:27.950512 lokzzpylib-0.2.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:10:27.946512 lokzzpylib-0.2.dev9/lokzzpylib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/lokzzpylib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:10:27.946512 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 10:10:27.000000 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 10:10:27.000000 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:10:27.000000 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 10:10:27.000000 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 10:10:27.000000 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:10:27.950512 lokzzpylib-0.2.dev9/setup.cfg
```

