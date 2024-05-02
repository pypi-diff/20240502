# Comparing `tmp/gtauthclient-0.0.6.tar.gz` & `tmp/gtauthclient-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtauthclient-0.0.6.tar", last modified: Fri Mar  8 22:08:52 2024, max compression
+gzip compressed data, was "gtauthclient-0.0.7.tar", last modified: Thu May  2 00:56:54 2024, max compression
```

## Comparing `gtauthclient-0.0.6.tar` & `gtauthclient-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:08:52.371018 gtauthclient-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-08 22:08:47.000000 gtauthclient-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-08 22:08:47.000000 gtauthclient-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-08 22:08:52.371018 gtauthclient-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-08 22:08:47.000000 gtauthclient-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:08:52.367017 gtauthclient-0.0.6/gtauthclient/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-08 22:08:47.000000 gtauthclient-0.0.6/gtauthclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:08:52.371018 gtauthclient-0.0.6/gtauthclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-08 22:08:52.000000 gtauthclient-0.0.6/gtauthclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-08 22:08:52.000000 gtauthclient-0.0.6/gtauthclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 22:08:52.000000 gtauthclient-0.0.6/gtauthclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-08 22:08:52.000000 gtauthclient-0.0.6/gtauthclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-08 22:08:52.000000 gtauthclient-0.0.6/gtauthclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-08 22:08:47.000000 gtauthclient-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-08 22:08:47.000000 gtauthclient-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 22:08:52.371018 gtauthclient-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-08 22:08:47.000000 gtauthclient-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:56:54.445114 gtauthclient-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 00:56:43.000000 gtauthclient-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 00:56:43.000000 gtauthclient-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-02 00:56:54.445114 gtauthclient-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-02 00:56:43.000000 gtauthclient-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:56:54.441114 gtauthclient-0.0.7/gtauthclient/
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-02 00:56:43.000000 gtauthclient-0.0.7/gtauthclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:56:54.445114 gtauthclient-0.0.7/gtauthclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-02 00:56:54.000000 gtauthclient-0.0.7/gtauthclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 00:56:54.000000 gtauthclient-0.0.7/gtauthclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:56:54.000000 gtauthclient-0.0.7/gtauthclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 00:56:54.000000 gtauthclient-0.0.7/gtauthclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 00:56:54.000000 gtauthclient-0.0.7/gtauthclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 00:56:43.000000 gtauthclient-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 00:56:43.000000 gtauthclient-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:56:54.445114 gtauthclient-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-02 00:56:43.000000 gtauthclient-0.0.7/setup.py
```

### Comparing `gtauthclient-0.0.6/LICENSE` & `gtauthclient-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gtauthclient-0.0.6/PKG-INFO` & `gtauthclient-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: gtauthclient
-Version: 0.0.6
-Summary: GT Auth Client for FastAPI
-Author: Josh XT
-Author-email: josh@devxt.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: fastapi
-Requires-Dist: PyJWT
-
 [![GitHub](https://img.shields.io/badge/GitHub-Sponsor%20Josh%20XT-blue?logo=github&style=plastic)](https://github.com/sponsors/Josh-XT) [![PayPal](https://img.shields.io/badge/PayPal-Sponsor%20Josh%20XT-blue.svg?logo=paypal&style=plastic)](https://paypal.me/joshxt) [![Ko-Fi](https://img.shields.io/badge/Kofi-Sponsor%20Josh%20XT-blue.svg?logo=kofi&style=plastic)](https://ko-fi.com/joshxt)
 # GT Auth Client
 
 This is the Python GT Auth Client for FastAPI. It is used to authenticate with the GT Auth API.
 ## Installation
 
 You can install the package using pip:
@@ -32,8 +20,8 @@
 
 auth = GTAuthClient(key="Your encryption key")
 app = FastAPI()
 
 @app.get("/v1/users", dependencies=[Depends(auth.verify_user)])
 async def list_users():
     return ["John", "Jane", "Jack"]
-```
+```
```

