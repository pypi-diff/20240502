# Comparing `tmp/json2gbnf-0.0.1.tar.gz` & `tmp/json2gbnf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json2gbnf-0.0.1.tar", last modified: Mon Apr 29 11:21:05 2024, max compression
+gzip compressed data, was "json2gbnf-0.0.4.tar", last modified: Thu May  2 11:22:37 2024, max compression
```

## Comparing `json2gbnf-0.0.1.tar` & `json2gbnf-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 thekevinscott   (501) staff       (20)        0 2024-04-29 11:21:05.210249 json2gbnf-0.0.1/
--rw-r--r--   0 thekevinscott   (501) staff       (20)       18 2024-04-29 11:18:48.000000 json2gbnf-0.0.1/MANIFEST.in
--rw-r--r--   0 thekevinscott   (501) staff       (20)      180 2024-04-29 11:21:05.210029 json2gbnf-0.0.1/PKG-INFO
--rw-r--r--   0 thekevinscott   (501) staff       (20)       12 2024-04-29 11:18:48.000000 json2gbnf-0.0.1/README.md
-drwxr-xr-x   0 thekevinscott   (501) staff       (20)        0 2024-04-29 11:21:05.209197 json2gbnf-0.0.1/json2gbnf/
--rw-r--r--   0 thekevinscott   (501) staff       (20)       58 2024-04-29 11:18:48.000000 json2gbnf-0.0.1/json2gbnf/__init__.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)       39 2024-04-29 11:18:48.000000 json2gbnf-0.0.1/json2gbnf/json2gbnf.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)       82 2024-04-29 11:18:48.000000 json2gbnf-0.0.1/json2gbnf/json2gbnf_test.py
-drwxr-xr-x   0 thekevinscott   (501) staff       (20)        0 2024-04-29 11:21:05.209824 json2gbnf-0.0.1/json2gbnf.egg-info/
--rw-r--r--   0 thekevinscott   (501) staff       (20)      180 2024-04-29 11:21:05.000000 json2gbnf-0.0.1/json2gbnf.egg-info/PKG-INFO
--rw-r--r--   0 thekevinscott   (501) staff       (20)      241 2024-04-29 11:21:05.000000 json2gbnf-0.0.1/json2gbnf.egg-info/SOURCES.txt
--rw-r--r--   0 thekevinscott   (501) staff       (20)        1 2024-04-29 11:21:05.000000 json2gbnf-0.0.1/json2gbnf.egg-info/dependency_links.txt
--rw-r--r--   0 thekevinscott   (501) staff       (20)       10 2024-04-29 11:21:05.000000 json2gbnf-0.0.1/json2gbnf.egg-info/top_level.txt
--rw-r--r--   0 thekevinscott   (501) staff       (20)      211 2024-04-29 11:18:48.000000 json2gbnf-0.0.1/pyproject.toml
--rw-r--r--   0 thekevinscott   (501) staff       (20)       38 2024-04-29 11:21:05.210296 json2gbnf-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:22:37.065638 json2gbnf-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 11:22:22.000000 json2gbnf-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 11:21:42.000000 json2gbnf-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 11:22:37.065638 json2gbnf-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 11:21:42.000000 json2gbnf-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:22:37.061638 json2gbnf-0.0.4/json2gbnf/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 11:21:42.000000 json2gbnf-0.0.4/json2gbnf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:22:37.065638 json2gbnf-0.0.4/json2gbnf/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-02 11:22:35.000000 json2gbnf-0.0.4/json2gbnf/js/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 11:21:42.000000 json2gbnf-0.0.4/json2gbnf/json2gbnf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-02 11:21:42.000000 json2gbnf-0.0.4/json2gbnf/json2gbnf_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:22:37.065638 json2gbnf-0.0.4/json2gbnf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 11:22:37.000000 json2gbnf-0.0.4/json2gbnf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-02 11:22:37.000000 json2gbnf-0.0.4/json2gbnf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:22:37.000000 json2gbnf-0.0.4/json2gbnf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 11:22:37.000000 json2gbnf-0.0.4/json2gbnf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 11:22:37.000000 json2gbnf-0.0.4/json2gbnf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-02 11:21:42.000000 json2gbnf-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 11:22:37.065638 json2gbnf-0.0.4/setup.cfg
```

