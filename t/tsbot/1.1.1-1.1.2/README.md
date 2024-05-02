# Comparing `tmp/tsbot-1.1.1.tar.gz` & `tmp/tsbot-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsbot-1.1.1.tar", last modified: Tue Apr 30 15:45:09 2024, max compression
+gzip compressed data, was "tsbot-1.1.2.tar", last modified: Thu May  2 13:44:17 2024, max compression
```

## Comparing `tsbot-1.1.1.tar` & `tsbot-1.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.046346 tsbot-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 15:45:05.000000 tsbot-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-30 15:45:09.046346 tsbot-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-30 15:45:05.000000 tsbot-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-30 15:45:05.000000 tsbot-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:45:09.046346 tsbot-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.038346 tsbot-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-30 15:45:05.000000 tsbot-1.1.1/tests/test_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.042346 tsbot-1.1.1/tsbot/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.042346 tsbot-1.1.1/tsbot/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/commands/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.042346 tsbot-1.1.1/tsbot/default_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/default_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/default_plugins/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/default_plugins/keepalive.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.042346 tsbot-1.1.1/tsbot/events/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/events/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/events/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/events/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.046346 tsbot-1.1.1/tsbot/query_builder/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/query_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/query_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/query_builder/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.046346 tsbot-1.1.1/tsbot/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/tasks/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-30 15:45:05.000000 tsbot-1.1.1/tsbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:45:09.046346 tsbot-1.1.1/tsbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-30 15:45:09.000000 tsbot-1.1.1/tsbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-30 15:45:09.000000 tsbot-1.1.1/tsbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:45:09.000000 tsbot-1.1.1/tsbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 15:45:09.000000 tsbot-1.1.1/tsbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 15:45:09.000000 tsbot-1.1.1/tsbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:44:17.845217 tsbot-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-02 13:44:13.000000 tsbot-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-02 13:44:17.845217 tsbot-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-02 13:44:13.000000 tsbot-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-02 13:44:13.000000 tsbot-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:44:17.845217 tsbot-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:44:17.837217 tsbot-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-02 13:44:13.000000 tsbot-1.1.2/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-02 13:44:13.000000 tsbot-1.1.2/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 13:44:13.000000 tsbot-1.1.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-02 13:44:13.000000 tsbot-1.1.2/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-02 13:44:13.000000 tsbot-1.1.2/tests/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-02 13:44:13.000000 tsbot-1.1.2/tests/test_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-02 13:44:13.000000 tsbot-1.1.2/tests/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:44:17.841217 tsbot-1.1.2/tsbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:44:17.841217 tsbot-1.1.2/tsbot/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/commands/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:44:17.841217 tsbot-1.1.2/tsbot/default_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/default_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/default_plugins/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/default_plugins/keepalive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:44:17.845217 tsbot-1.1.2/tsbot/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/events/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/events/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/events/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:44:17.845217 tsbot-1.1.2/tsbot/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/query_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/query_builder/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:44:17.845217 tsbot-1.1.2/tsbot/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/tasks/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-02 13:44:13.000000 tsbot-1.1.2/tsbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:44:17.845217 tsbot-1.1.2/tsbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-02 13:44:17.000000 tsbot-1.1.2/tsbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-02 13:44:17.000000 tsbot-1.1.2/tsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:44:17.000000 tsbot-1.1.2/tsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-02 13:44:17.000000 tsbot-1.1.2/tsbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 13:44:17.000000 tsbot-1.1.2/tsbot.egg-info/top_level.txt
```

### Comparing `tsbot-1.1.1/LICENSE` & `tsbot-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/README.md` & `tsbot-1.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # TSBot
 
 Asynchronous framework to build **TeamSpeak 3 Server Query** bots
 
 ## ✅ Features
 
-- Uses modern Python `async` and `await` syntax
+- Modern Python `async` and `await` syntax
 - Secure connection through SSH
 - Ease of use query building
-- Built-in and configurable ratelimiter if no access to `whitelist.txt`
+- Built-in and configurable ratelimiter if no access to `query_ip_allowlist.txt`
 
 ## ✏️ Examples
 
 ```python
 from __future__ import annotations
 
 import asyncio
```

### Comparing `tsbot-1.1.1/pyproject.toml` & `tsbot-1.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [project]
 name = "tsbot"
-version = "1.1.1"
+version = "1.1.2"
 authors = [{ name = "0x4aK" }]
 description = "Asynchronous framework to build TeamSpeak 3 Server Query bots"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: AsyncIO",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
 ]
-dependencies = ["asyncssh == 2.14.0"]
-license = { file = "LICENCE" }
+dependencies = ["asyncssh == 2.14.0", "tsformatter >= 0.2.1"]
+license = { file = "LICENSE" }
 urls = { repository = "https://github.com/0x4aK/tsbot", documentation = "https://tsbot.readthedocs.io/en/latest/" }
 
 
 [project.optional-dependencies]
-tests = ["mypy >= 1.9.0", "pytest == 8.1.1", "pytest-cov == 5.0.0"]
+dev = ["black >= 24.4.0", "isort >= 5.13.2", "sphinx-autobuild >= 2024.4.16"]
+tests = ["mypy >= 1.9.0", "pytest == 8.1.1"]
 docs = [
     "sphinx >= 7.3.7",
     "myst-parser >= 2.0.0",
     "sphinx-autodoc-typehints >= 2.1.0",
-    "sphinx-autobuild >= 2024.4.16",
     "sphinx_rtd_theme >= 2.0.0",
 ]
 
 
 [build-system]
 requires = ["setuptools >= 69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
@@ -40,15 +40,14 @@
 
 
 [tool.setuptools.package-data]
 tsbot = ["py.typed"]
 
 
 [tool.pytest.ini_options]
-addopts = "--cov"
 testpaths = ["tests"]
 
 
 [tool.black]
 line-length = 100
 target-version = ['py310']
 
@@ -68,28 +67,28 @@
 show_error_codes = true
 
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 minversion = 3.8.0
-envlist = py310, py311, mypy
+envlist = py310, py311, py312, mypy
 isolated_build = true
 
 [gh-actions]
 python =
     3.10: py310, mypy
     3.11: py311
     3.12: py312
 
 [testenv]
 setenv =
     PYTHONPATH = {toxinidir}
 extras = tests
-commands = pytest --basetemp={envtmpdir} --cov
+commands = pytest --basetemp={envtmpdir}
 
 [testenv:mypy]
 basepython = python3.10
 deps =
     mypy
 commands = mypy tsbot
 """
```

### Comparing `tsbot-1.1.1/tests/test_connection.py` & `tsbot-1.1.2/tests/test_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 
 async def mock_connect(*args: Any, **kwargs: Any):
     return MockClientConnection()
 
 
 @pytest.fixture
 def conn(monkeypatch: pytest.MonkeyPatch, conn_info: ConnectionInfo):
-    monkeypatch.setattr(asyncssh.connection, "connect", mock_connect)
+    monkeypatch.setattr(asyncssh, "connect", mock_connect)
 
     return connection.TSConnection(
         conn_info.username, conn_info.password, conn_info.address, conn_info.port
     )
 
 
 @pytest.fixture
 def connected_conn(monkeypatch: pytest.MonkeyPatch, conn_info: ConnectionInfo):
-    monkeypatch.setattr(asyncssh.connection, "connect", mock_connect)
+    monkeypatch.setattr(asyncssh, "connect", mock_connect)
 
     c = connection.TSConnection(
         conn_info.username, conn_info.password, conn_info.address, conn_info.port
     )
     asyncio.run(c.connect())
     return c
```

### Comparing `tsbot-1.1.1/tests/test_encoders.py` & `tsbot-1.1.2/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tests/test_parsers.py` & `tsbot-1.1.2/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tests/test_query_builder.py` & `tsbot-1.1.2/tests/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tests/test_ratelimiter.py` & `tsbot-1.1.2/tests/test_ratelimiter.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tests/test_response.py` & `tsbot-1.1.2/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/bot.py` & `tsbot-1.1.2/tsbot/bot.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/commands/command.py` & `tsbot-1.1.2/tsbot/commands/command.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/commands/handler.py` & `tsbot-1.1.2/tsbot/commands/handler.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/connection.py` & `tsbot-1.1.2/tsbot/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 class TSConnection:
     def __init__(self, username: str, password: str, address: str, port: int = 10022) -> None:
         self.username = username
         self.password = password
         self.address = address
         self.port = port
 
-        self._connection: asyncssh.connection.SSHClientConnection | None = None
-        self._writer: asyncssh.stream.SSHWriter[str] | None = None
-        self._reader: asyncssh.stream.SSHReader[str] | None = None
+        self._connection: asyncssh.SSHClientConnection | None = None
+        self._writer: asyncssh.SSHWriter[str] | None = None
+        self._reader: asyncssh.SSHReader[str] | None = None
 
     async def connect(self) -> None:
-        self._connection = await asyncssh.connection.connect(
-            self.address,
+        self._connection = await asyncssh.connect(
+            host=self.address,
             port=self.port,
             username=self.username,
             password=self.password,
             known_hosts=None,
+            preferred_auth="password",
         )
 
         self._writer, self._reader, _ = await self._connection.open_session()  # type: ignore
         logger.info("Connected")
 
     async def close(self) -> None:
         if self._writer:
```

### Comparing `tsbot-1.1.1/tsbot/default_plugins/keepalive.py` & `tsbot-1.1.2/tsbot/default_plugins/keepalive.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/encoders.py` & `tsbot-1.1.2/tsbot/encoders.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/events/event.py` & `tsbot-1.1.2/tsbot/events/event.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/events/event_handler.py` & `tsbot-1.1.2/tsbot/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/events/handler.py` & `tsbot-1.1.2/tsbot/events/handler.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/exceptions.py` & `tsbot-1.1.2/tsbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/parsers.py` & `tsbot-1.1.2/tsbot/parsers.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/plugin.py` & `tsbot-1.1.2/tsbot/plugin.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/query_builder/builder.py` & `tsbot-1.1.2/tsbot/query_builder/builder.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/query_builder/commands.py` & `tsbot-1.1.2/tsbot/query_builder/commands.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/ratelimiter.py` & `tsbot-1.1.2/tsbot/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/response.py` & `tsbot-1.1.2/tsbot/response.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/tasks/handler.py` & `tsbot-1.1.2/tsbot/tasks/handler.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/tasks/task.py` & `tsbot-1.1.2/tsbot/tasks/task.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot/utils.py` & `tsbot-1.1.2/tsbot/utils.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.1.1/tsbot.egg-info/SOURCES.txt` & `tsbot-1.1.2/tsbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

