# Comparing `tmp/iamlistening-5.1.8.tar.gz` & `tmp/iamlistening-5.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-5.1.8.tar", max compression
+gzip compressed data, was "iamlistening-5.1.9.tar", max compression
```

## Comparing `iamlistening-5.1.8.tar` & `iamlistening-5.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2024-04-18 05:16:31.547231 iamlistening-5.1.8/LICENSE
--rw-r--r--   0        0        0     2467 2024-04-18 05:16:31.547231 iamlistening-5.1.8/README.md
--rw-r--r--   0        0        0      113 2024-04-18 05:17:05.695458 iamlistening-5.1.8/iamlistening/__init__.py
--rw-r--r--   0        0        0      443 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/config.py
--rw-r--r--   0        0        0     1824 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/default_settings.toml
--rw-r--r--   0        0        0      548 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/__init__.py
--rw-r--r--   0        0        0     3441 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/client.py
--rw-r--r--   0        0        0      790 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/discord.py
--rw-r--r--   0        0        0      668 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/guilded.py
--rw-r--r--   0        0        0      834 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/lemmy.py
--rw-r--r--   0        0        0     1281 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/mastodon.py
--rw-r--r--   0        0        0     1413 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/matrix.py
--rw-r--r--   0        0        0      698 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/revolt.py
--rw-r--r--   0        0        0      899 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/telegram.py
--rw-r--r--   0        0        0      761 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/twitch.py
--rw-r--r--   0        0        0     6600 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/main.py
--rw-r--r--   0        0        0     4027 2024-04-18 05:17:05.695458 iamlistening-5.1.8/pyproject.toml
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 iamlistening-5.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-19 04:26:23.474845 iamlistening-5.1.9/LICENSE
+-rw-r--r--   0        0        0     2467 2024-04-19 04:26:23.474845 iamlistening-5.1.9/README.md
+-rw-r--r--   0        0        0      113 2024-04-19 04:27:00.038824 iamlistening-5.1.9/iamlistening/__init__.py
+-rw-r--r--   0        0        0      443 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/config.py
+-rw-r--r--   0        0        0     1824 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0      548 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/handler/__init__.py
+-rw-r--r--   0        0        0     3441 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/handler/client.py
+-rw-r--r--   0        0        0      790 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/handler/discord.py
+-rw-r--r--   0        0        0      668 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/handler/guilded.py
+-rw-r--r--   0        0        0      834 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/handler/lemmy.py
+-rw-r--r--   0        0        0     1281 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/handler/mastodon.py
+-rw-r--r--   0        0        0     1413 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/handler/matrix.py
+-rw-r--r--   0        0        0      698 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/handler/revolt.py
+-rw-r--r--   0        0        0      899 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/handler/telegram.py
+-rw-r--r--   0        0        0      761 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/handler/twitch.py
+-rw-r--r--   0        0        0     6600 2024-04-19 04:26:23.478845 iamlistening-5.1.9/iamlistening/main.py
+-rw-r--r--   0        0        0     4029 2024-04-19 04:27:00.038824 iamlistening-5.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 iamlistening-5.1.9/PKG-INFO
```

### Comparing `iamlistening-5.1.8/LICENSE` & `iamlistening-5.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/README.md` & `iamlistening-5.1.9/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/default_settings.toml` & `iamlistening-5.1.9/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/handler/__init__.py` & `iamlistening-5.1.9/iamlistening/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/handler/client.py` & `iamlistening-5.1.9/iamlistening/handler/client.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/handler/discord.py` & `iamlistening-5.1.9/iamlistening/handler/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/handler/guilded.py` & `iamlistening-5.1.9/iamlistening/handler/guilded.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/handler/lemmy.py` & `iamlistening-5.1.9/iamlistening/handler/lemmy.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/handler/mastodon.py` & `iamlistening-5.1.9/iamlistening/handler/mastodon.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/handler/matrix.py` & `iamlistening-5.1.9/iamlistening/handler/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/handler/revolt.py` & `iamlistening-5.1.9/iamlistening/handler/revolt.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/handler/telegram.py` & `iamlistening-5.1.9/iamlistening/handler/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/handler/twitch.py` & `iamlistening-5.1.9/iamlistening/handler/twitch.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/iamlistening/main.py` & `iamlistening-5.1.9/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.8/pyproject.toml` & `iamlistening-5.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "5.1.8"
+version = "5.1.9"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix",
@@ -37,15 +37,15 @@
 "guilded.py" = "1.13.0"
 "revolt.py" = "0.2.0"
 pythorhead = {version ="0.24.0", python = ">=3.10,<3.12"}
 twitchio = "2.9.1"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = ">=8.0.8"
-ruff = "^0.3.0"
+ruff = "^0.4.0"
 black = "^24.0.0"
 pre-commit = "^3.3.1"
 
 
 [tool.ruff]
 exclude = [
   ".github/*",
@@ -134,27 +134,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `iamlistening-5.1.8/PKG-INFO` & `iamlistening-5.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 5.1.8
+Version: 5.1.9
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 5.1.8 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 5.1.9 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: Mastodon.py (==1.8.1) Requires-Dist:
```

