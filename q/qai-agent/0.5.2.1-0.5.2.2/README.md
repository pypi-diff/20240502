# Comparing `tmp/qai_agent-0.5.2.1.tar.gz` & `tmp/qai_agent-0.5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_agent-0.5.2.1.tar", max compression
+gzip compressed data, was "qai_agent-0.5.2.2.tar", max compression
```

## Comparing `qai_agent-0.5.2.1.tar` & `qai_agent-0.5.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       37 2024-05-01 17:37:25.187159 qai_agent-0.5.2.1/README.md
--rw-r--r--   0        0        0     1922 2024-05-02 05:34:51.897094 qai_agent-0.5.2.1/pyproject.toml
--rw-r--r--   0        0        0     1227 2024-04-30 20:51:02.838309 qai_agent-0.5.2.1/src/qai/agent/__init__.py
--rw-r--r--   0        0        0    10173 2024-05-02 05:19:41.510594 qai_agent-0.5.2.1/src/qai/agent/agents/campaign/campaign.py
--rw-r--r--   0        0        0     4358 2024-04-26 02:55:29.618634 qai_agent-0.5.2.1/src/qai/agent/agents/conversation.py
--rw-r--r--   0        0        0    13254 2024-05-02 05:33:53.017724 qai_agent-0.5.2.1/src/qai/agent/agents/email.py
--rw-r--r--   0        0        0     3389 2024-05-02 05:19:15.871949 qai_agent-0.5.2.1/src/qai/agent/agents/example_agent.py
--rw-r--r--   0        0        0     3505 2024-05-02 05:18:58.522327 qai_agent-0.5.2.1/src/qai/agent/agents/find_agent.py
--rw-r--r--   0        0        0    11013 2024-05-02 05:18:49.979317 qai_agent-0.5.2.1/src/qai/agent/agents/sql_query.py
--rw-r--r--   0        0        0        0 2024-04-15 22:16:56.666275 qai_agent-0.5.2.1/src/qai/agent/agents/tools/__init__.py
--rw-r--r--   0        0        0     1399 2024-05-02 05:23:24.210450 qai_agent-0.5.2.1/src/qai/agent/agents/tools/outreach.py
--rw-r--r--   0        0        0        0 2024-04-15 04:05:07.959600 qai_agent-0.5.2.1/src/qai/agent/agents/worker/__init__.py
--rw-r--r--   0        0        0     3166 2024-05-02 05:21:41.273125 qai_agent-0.5.2.1/src/qai/agent/basic.py
--rw-r--r--   0        0        0        0 2024-04-12 13:12:16.649604 qai_agent-0.5.2.1/src/qai/agent/data/__init__.py
--rw-r--r--   0        0        0     1284 2024-04-12 13:12:16.649487 qai_agent-0.5.2.1/src/qai/agent/data/state_codes.py
--rw-r--r--   0        0        0     1322 2024-05-02 05:19:57.743021 qai_agent-0.5.2.1/src/qai/agent/llama_index/llm_program.py
--rw-r--r--   0        0        0      170 2024-04-24 22:13:53.649180 qai_agent-0.5.2.1/src/qai/agent/models.py
--rw-r--r--   0        0        0     3312 2024-05-02 05:21:46.573311 qai_agent-0.5.2.1/src/qai/agent/qaibot.py
--rw-r--r--   0        0        0     3403 2024-05-02 05:21:56.520197 qai_agent-0.5.2.1/src/qai/agent/serve.py
--rw-r--r--   0        0        0     1270 2024-05-02 05:20:08.067204 qai_agent-0.5.2.1/src/qai/agent/sessions/qai_session.py
--rw-r--r--   0        0        0        0 2024-04-15 22:17:20.139827 qai_agent-0.5.2.1/src/qai/agent/tools/__init__.py
--rw-r--r--   0        0        0      423 2024-04-15 21:28:23.268771 qai_agent-0.5.2.1/src/qai/agent/tools/types.py
--rw-r--r--   0        0        0     4497 2024-04-12 13:12:16.582078 qai_agent-0.5.2.1/src/qai/agent/tools.py
--rw-r--r--   0        0        0       56 2024-04-25 02:05:04.018482 qai_agent-0.5.2.1/src/qai/agent/utils/__init__.py
--rw-r--r--   0        0        0      397 2024-04-12 15:02:35.886303 qai_agent-0.5.2.1/src/qai/agent/utils/db_utils.py
--rw-r--r--   0        0        0     8150 2024-05-01 16:31:43.583775 qai_agent-0.5.2.1/src/qai/agent/utils/distribute.py
--rw-r--r--   0        0        0     3636 2024-05-02 05:21:23.859476 qai_agent-0.5.2.1/src/qai/agent/utils/utils.py
--rw-r--r--   0        0        0     1885 1970-01-01 00:00:00.000000 qai_agent-0.5.2.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-05-02 06:52:44.114033 qai_agent-0.5.2.2/README.md
+-rw-r--r--   0        0        0     1922 2024-05-02 16:09:05.869587 qai_agent-0.5.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1227 2024-05-02 06:52:44.117744 qai_agent-0.5.2.2/src/qai/agent/__init__.py
+-rw-r--r--   0        0        0    10173 2024-05-02 06:52:44.123828 qai_agent-0.5.2.2/src/qai/agent/agents/campaign/campaign.py
+-rw-r--r--   0        0        0     3164 2024-05-02 06:52:44.120615 qai_agent-0.5.2.2/src/qai/agent/agents/conversation.py
+-rw-r--r--   0        0        0    13254 2024-05-02 06:52:44.122385 qai_agent-0.5.2.2/src/qai/agent/agents/email.py
+-rw-r--r--   0        0        0     3389 2024-05-02 06:52:44.120375 qai_agent-0.5.2.2/src/qai/agent/agents/example_agent.py
+-rw-r--r--   0        0        0     3505 2024-05-02 06:52:44.118310 qai_agent-0.5.2.2/src/qai/agent/agents/find_agent.py
+-rw-r--r--   0        0        0    11013 2024-05-02 06:52:44.120971 qai_agent-0.5.2.2/src/qai/agent/agents/sql_query.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.118819 qai_agent-0.5.2.2/src/qai/agent/agents/tools/__init__.py
+-rw-r--r--   0        0        0     1399 2024-05-02 06:52:44.118768 qai_agent-0.5.2.2/src/qai/agent/agents/tools/outreach.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.124088 qai_agent-0.5.2.2/src/qai/agent/agents/worker/__init__.py
+-rw-r--r--   0        0        0     3166 2024-05-02 06:52:44.131675 qai_agent-0.5.2.2/src/qai/agent/basic.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.132044 qai_agent-0.5.2.2/src/qai/agent/data/__init__.py
+-rw-r--r--   0        0        0     1284 2024-05-02 06:52:44.131968 qai_agent-0.5.2.2/src/qai/agent/data/state_codes.py
+-rw-r--r--   0        0        0     1322 2024-05-02 06:52:44.117542 qai_agent-0.5.2.2/src/qai/agent/llama_index/llm_program.py
+-rw-r--r--   0        0        0      170 2024-05-02 06:52:44.116688 qai_agent-0.5.2.2/src/qai/agent/models.py
+-rw-r--r--   0        0        0     3312 2024-05-02 06:52:44.116889 qai_agent-0.5.2.2/src/qai/agent/qaibot.py
+-rw-r--r--   0        0        0     3403 2024-05-02 06:52:44.117981 qai_agent-0.5.2.2/src/qai/agent/serve.py
+-rw-r--r--   0        0        0     1270 2024-05-02 06:52:44.130644 qai_agent-0.5.2.2/src/qai/agent/sessions/qai_session.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.115489 qai_agent-0.5.2.2/src/qai/agent/tools/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-02 06:52:44.115702 qai_agent-0.5.2.2/src/qai/agent/tools/types.py
+-rw-r--r--   0        0        0     4497 2024-05-02 06:52:44.117132 qai_agent-0.5.2.2/src/qai/agent/tools.py
+-rw-r--r--   0        0        0       56 2024-05-02 06:52:44.126120 qai_agent-0.5.2.2/src/qai/agent/utils/__init__.py
+-rw-r--r--   0        0        0      397 2024-05-02 06:52:44.128007 qai_agent-0.5.2.2/src/qai/agent/utils/db_utils.py
+-rw-r--r--   0        0        0     8150 2024-05-02 06:52:44.125814 qai_agent-0.5.2.2/src/qai/agent/utils/distribute.py
+-rw-r--r--   0        0        0     3636 2024-05-02 06:52:44.127769 qai_agent-0.5.2.2/src/qai/agent/utils/utils.py
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 qai_agent-0.5.2.2/PKG-INFO
```

### Comparing `qai_agent-0.5.2.1/pyproject.toml` & `qai_agent-0.5.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
 description = "Qai Agents for the Qai AI Platform"
 name = "qai-agent"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.2.1"
+version = "0.5.2.2"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 install = "^1.3.5"
 llama-index-agent-openai = "^0.2.3"
 llama-index-core = "^0.10.30"
 llama-index-embeddings-huggingface = "^0.2.0"
@@ -31,15 +31,15 @@
 pi-log = "^0.5.7.3"
 pip = "^24.0"
 pydantic = "^2.7.0"
 pymongo = "^4.6.3"
 python-dateutil = "2.8.2"
 python-dotenv = "^1.0.1"
 qai-ai = "0.5.2.3"
-qai-core = "^0.5.0"
+qai-core = "^0.5.1"
 sqlalchemy = "^2.0.29"
 torch = [
     {markers = "sys_platform == 'darwin' and platform_machine == 'arm64'", source = "pypi", version = "^2.3.0"},
     {platform = "darwin", source = "pypi", version = "^2.3.0"},
     {platform = "linux", source = "pytorch-cpu-src", version = "=2.3.0+cpu"},
     {platform = "win32", source = "pytorch-cpu-src", version = "=2.3.0+cpu"},
 ]
```

### Comparing `qai_agent-0.5.2.1/src/qai/agent/__init__.py` & `qai_agent-0.5.2.2/src/qai/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/agents/campaign/campaign.py` & `qai_agent-0.5.2.2/src/qai/agent/agents/campaign/campaign.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/agents/email.py` & `qai_agent-0.5.2.2/src/qai/agent/agents/email.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/agents/example_agent.py` & `qai_agent-0.5.2.2/src/qai/agent/agents/example_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/agents/find_agent.py` & `qai_agent-0.5.2.2/src/qai/agent/agents/find_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/agents/sql_query.py` & `qai_agent-0.5.2.2/src/qai/agent/agents/sql_query.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/agents/tools/outreach.py` & `qai_agent-0.5.2.2/src/qai/agent/agents/tools/outreach.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/basic.py` & `qai_agent-0.5.2.2/src/qai/agent/basic.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/data/state_codes.py` & `qai_agent-0.5.2.2/src/qai/agent/data/state_codes.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/llama_index/llm_program.py` & `qai_agent-0.5.2.2/src/qai/agent/llama_index/llm_program.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/qaibot.py` & `qai_agent-0.5.2.2/src/qai/agent/qaibot.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/serve.py` & `qai_agent-0.5.2.2/src/qai/agent/serve.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/sessions/qai_session.py` & `qai_agent-0.5.2.2/src/qai/agent/sessions/qai_session.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/tools.py` & `qai_agent-0.5.2.2/src/qai/agent/tools.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/utils/distribute.py` & `qai_agent-0.5.2.2/src/qai/agent/utils/distribute.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/src/qai/agent/utils/utils.py` & `qai_agent-0.5.2.2/src/qai/agent/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.1/PKG-INFO` & `qai_agent-0.5.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qai-agent
-Version: 0.5.2.1
+Version: 0.5.2.2
 Summary: Qai Agents for the Qai AI Platform
 Author: parnell
 Author-email: 152523161+leeparnell@users.noreply.github.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: install (>=1.3.5,<2.0.0)
@@ -26,18 +26,18 @@
 Requires-Dist: pi-log (>=0.5.7.3,<0.6.0.0)
 Requires-Dist: pip (>=24.0,<25.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: qai-ai (==0.5.2.3)
-Requires-Dist: qai-core (>=0.5.0,<0.6.0)
+Requires-Dist: qai-core (>=0.5.1,<0.6.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: torch (==2.3.0+cpu) ; sys_platform == "linux"
 Requires-Dist: torch (==2.3.0+cpu) ; sys_platform == "win32"
 Requires-Dist: torch (>=2.3.0,<3.0.0) ; sys_platform == "darwin"
 Requires-Dist: torch (>=2.3.0,<3.0.0) ; sys_platform == "darwin" and platform_machine == "arm64"
 Description-Content-Type: text/markdown
 
-# Example Project
+# Qai-Agent
+
 
-brew install mysql
```

