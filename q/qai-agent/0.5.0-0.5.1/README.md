# Comparing `tmp/qai_agent-0.5.0.tar.gz` & `tmp/qai_agent-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_agent-0.5.0.tar", max compression
+gzip compressed data, was "qai_agent-0.5.1.tar", max compression
```

## Comparing `qai_agent-0.5.0.tar` & `qai_agent-0.5.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       37 2024-05-01 17:37:25.187159 qai_agent-0.5.0/README.md
--rw-r--r--   0        0        0     1454 2024-05-01 22:49:17.850951 qai_agent-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1227 2024-04-30 20:51:02.838309 qai_agent-0.5.0/src/qai/agent/__init__.py
--rw-r--r--   0        0        0    14064 2024-05-01 17:42:03.041730 qai_agent-0.5.0/src/qai/agent/agents/campaign/campaign.py
--rw-r--r--   0        0        0     1252 2024-05-01 15:49:03.307593 qai_agent-0.5.0/src/qai/agent/agents/campaign/qrev_emailagent.py
--rw-r--r--   0        0        0     3666 2024-04-26 02:55:26.136573 qai_agent-0.5.0/src/qai/agent/agents/campaign copy 2.py
--rw-r--r--   0        0        0     2129 2024-04-19 23:58:17.882460 qai_agent-0.5.0/src/qai/agent/agents/campaign copy.py
--rw-r--r--   0        0        0     4358 2024-04-26 02:55:29.618634 qai_agent-0.5.0/src/qai/agent/agents/conversation.py
--rw-r--r--   0        0        0    14917 2024-05-01 21:56:22.067706 qai_agent-0.5.0/src/qai/agent/agents/email.py
--rw-r--r--   0        0        0     4335 2024-04-15 04:54:10.408696 qai_agent-0.5.0/src/qai/agent/agents/example_agent.py
--rw-r--r--   0        0        0     3826 2024-04-26 00:28:53.722668 qai_agent-0.5.0/src/qai/agent/agents/find_agent.py
--rw-r--r--   0        0        0     8734 2024-04-26 02:55:32.911873 qai_agent-0.5.0/src/qai/agent/agents/sql_query copy 2.py
--rw-r--r--   0        0        0    12820 2024-04-26 02:55:35.318095 qai_agent-0.5.0/src/qai/agent/agents/sql_query copy 3.py
--rw-r--r--   0        0        0    10748 2024-04-26 02:55:38.833304 qai_agent-0.5.0/src/qai/agent/agents/sql_query copy.py
--rw-r--r--   0        0        0    11069 2024-05-01 21:11:20.490262 qai_agent-0.5.0/src/qai/agent/agents/sql_query.py
--rw-r--r--   0        0        0      442 2024-04-23 01:58:48.739947 qai_agent-0.5.0/src/qai/agent/agents/test.py
--rw-r--r--   0        0        0        0 2024-04-15 22:16:56.666275 qai_agent-0.5.0/src/qai/agent/agents/tools/__init__.py
--rw-r--r--   0        0        0     2155 2024-04-25 15:45:37.602364 qai_agent-0.5.0/src/qai/agent/agents/tools/outreach.py
--rw-r--r--   0        0        0     2369 2024-04-30 05:17:28.462522 qai_agent-0.5.0/src/qai/agent/agents/tools/types.py
--rw-r--r--   0        0        0        0 2024-04-15 04:05:07.959600 qai_agent-0.5.0/src/qai/agent/agents/worker/__init__.py
--rw-r--r--   0        0        0     4851 2024-04-26 02:55:42.760558 qai_agent-0.5.0/src/qai/agent/agents/worker/campaign_worker copy.py
--rw-r--r--   0        0        0     5401 2024-04-24 15:51:11.790090 qai_agent-0.5.0/src/qai/agent/agents/worker/retry_worker copy.py
--rw-r--r--   0        0        0     4046 2024-04-24 15:44:27.850895 qai_agent-0.5.0/src/qai/agent/agents/worker/retry_worker.py
--rw-r--r--   0        0        0     3951 2024-04-26 02:55:13.429897 qai_agent-0.5.0/src/qai/agent/basic.py
--rw-r--r--   0        0        0     2972 2024-04-12 13:12:16.580326 qai_agent-0.5.0/src/qai/agent/custom_bot.py
--rw-r--r--   0        0        0        0 2024-04-12 13:12:16.649604 qai_agent-0.5.0/src/qai/agent/data/__init__.py
--rw-r--r--   0        0        0     1284 2024-04-12 13:12:16.649487 qai_agent-0.5.0/src/qai/agent/data/state_codes.py
--rw-r--r--   0        0        0     1671 2024-04-26 21:05:29.498832 qai_agent-0.5.0/src/qai/agent/llama_index/llm_program.py
--rw-r--r--   0        0        0      170 2024-04-24 22:13:53.649180 qai_agent-0.5.0/src/qai/agent/models.py
--rw-r--r--   0        0        0     4683 2024-04-25 21:15:40.430411 qai_agent-0.5.0/src/qai/agent/qaibot.py
--rw-r--r--   0        0        0     3404 2024-04-26 00:29:13.276728 qai_agent-0.5.0/src/qai/agent/serve.py
--rw-r--r--   0        0        0     1658 2024-04-25 21:15:55.808197 qai_agent-0.5.0/src/qai/agent/sessions/qai_session.py
--rw-r--r--   0        0        0      623 2024-04-19 23:56:44.441519 qai_agent-0.5.0/src/qai/agent/sessions/session_factory.py
--rw-r--r--   0        0        0        0 2024-04-15 22:17:20.139827 qai_agent-0.5.0/src/qai/agent/tools/__init__.py
--rw-r--r--   0        0        0      423 2024-04-15 21:28:23.268771 qai_agent-0.5.0/src/qai/agent/tools/types.py
--rw-r--r--   0        0        0     4497 2024-04-12 13:12:16.582078 qai_agent-0.5.0/src/qai/agent/tools.py
--rw-r--r--   0        0        0       56 2024-04-25 02:05:04.018482 qai_agent-0.5.0/src/qai/agent/utils/__init__.py
--rw-r--r--   0        0        0      397 2024-04-12 15:02:35.886303 qai_agent-0.5.0/src/qai/agent/utils/db_utils.py
--rw-r--r--   0        0        0     8150 2024-05-01 16:31:43.583775 qai_agent-0.5.0/src/qai/agent/utils/distribute.py
--rw-r--r--   0        0        0     3646 2024-04-19 23:56:44.441543 qai_agent-0.5.0/src/qai/agent/utils/utils.py
--rw-r--r--   0        0        0     1359 2024-04-12 13:12:16.660004 qai_agent-0.5.0/src/qai/agent/vapi/qai_call.py
--rw-r--r--   0        0        0      766 2024-04-12 13:12:16.667827 qai_agent-0.5.0/src/qai/agent/vapi/vapi_qai.py
--rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 qai_agent-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-01 17:37:25.187159 qai_agent-0.5.1/README.md
+-rw-r--r--   0        0        0     1887 2024-05-02 03:20:06.721191 qai_agent-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1227 2024-04-30 20:51:02.838309 qai_agent-0.5.1/src/qai/agent/__init__.py
+-rw-r--r--   0        0        0    14064 2024-05-01 17:42:03.041730 qai_agent-0.5.1/src/qai/agent/agents/campaign/campaign.py
+-rw-r--r--   0        0        0     1252 2024-05-01 15:49:03.307593 qai_agent-0.5.1/src/qai/agent/agents/campaign/qrev_emailagent.py
+-rw-r--r--   0        0        0     3666 2024-04-26 02:55:26.136573 qai_agent-0.5.1/src/qai/agent/agents/campaign copy 2.py
+-rw-r--r--   0        0        0     2129 2024-04-19 23:58:17.882460 qai_agent-0.5.1/src/qai/agent/agents/campaign copy.py
+-rw-r--r--   0        0        0     4358 2024-04-26 02:55:29.618634 qai_agent-0.5.1/src/qai/agent/agents/conversation.py
+-rw-r--r--   0        0        0    14917 2024-05-01 21:56:22.067706 qai_agent-0.5.1/src/qai/agent/agents/email.py
+-rw-r--r--   0        0        0     4335 2024-04-15 04:54:10.408696 qai_agent-0.5.1/src/qai/agent/agents/example_agent.py
+-rw-r--r--   0        0        0     3826 2024-04-26 00:28:53.722668 qai_agent-0.5.1/src/qai/agent/agents/find_agent.py
+-rw-r--r--   0        0        0     8734 2024-04-26 02:55:32.911873 qai_agent-0.5.1/src/qai/agent/agents/sql_query copy 2.py
+-rw-r--r--   0        0        0    12820 2024-04-26 02:55:35.318095 qai_agent-0.5.1/src/qai/agent/agents/sql_query copy 3.py
+-rw-r--r--   0        0        0    10748 2024-04-26 02:55:38.833304 qai_agent-0.5.1/src/qai/agent/agents/sql_query copy.py
+-rw-r--r--   0        0        0    11069 2024-05-01 21:11:20.490262 qai_agent-0.5.1/src/qai/agent/agents/sql_query.py
+-rw-r--r--   0        0        0      442 2024-04-23 01:58:48.739947 qai_agent-0.5.1/src/qai/agent/agents/test.py
+-rw-r--r--   0        0        0        0 2024-04-15 22:16:56.666275 qai_agent-0.5.1/src/qai/agent/agents/tools/__init__.py
+-rw-r--r--   0        0        0     2155 2024-04-25 15:45:37.602364 qai_agent-0.5.1/src/qai/agent/agents/tools/outreach.py
+-rw-r--r--   0        0        0     2369 2024-04-30 05:17:28.462522 qai_agent-0.5.1/src/qai/agent/agents/tools/types.py
+-rw-r--r--   0        0        0        0 2024-04-15 04:05:07.959600 qai_agent-0.5.1/src/qai/agent/agents/worker/__init__.py
+-rw-r--r--   0        0        0     4851 2024-04-26 02:55:42.760558 qai_agent-0.5.1/src/qai/agent/agents/worker/campaign_worker copy.py
+-rw-r--r--   0        0        0     5401 2024-04-24 15:51:11.790090 qai_agent-0.5.1/src/qai/agent/agents/worker/retry_worker copy.py
+-rw-r--r--   0        0        0     4046 2024-04-24 15:44:27.850895 qai_agent-0.5.1/src/qai/agent/agents/worker/retry_worker.py
+-rw-r--r--   0        0        0     3951 2024-04-26 02:55:13.429897 qai_agent-0.5.1/src/qai/agent/basic.py
+-rw-r--r--   0        0        0     2972 2024-04-12 13:12:16.580326 qai_agent-0.5.1/src/qai/agent/custom_bot.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:12:16.649604 qai_agent-0.5.1/src/qai/agent/data/__init__.py
+-rw-r--r--   0        0        0     1284 2024-04-12 13:12:16.649487 qai_agent-0.5.1/src/qai/agent/data/state_codes.py
+-rw-r--r--   0        0        0     1671 2024-04-26 21:05:29.498832 qai_agent-0.5.1/src/qai/agent/llama_index/llm_program.py
+-rw-r--r--   0        0        0      170 2024-04-24 22:13:53.649180 qai_agent-0.5.1/src/qai/agent/models.py
+-rw-r--r--   0        0        0     4683 2024-04-25 21:15:40.430411 qai_agent-0.5.1/src/qai/agent/qaibot.py
+-rw-r--r--   0        0        0     3404 2024-04-26 00:29:13.276728 qai_agent-0.5.1/src/qai/agent/serve.py
+-rw-r--r--   0        0        0     1658 2024-04-25 21:15:55.808197 qai_agent-0.5.1/src/qai/agent/sessions/qai_session.py
+-rw-r--r--   0        0        0      623 2024-04-19 23:56:44.441519 qai_agent-0.5.1/src/qai/agent/sessions/session_factory.py
+-rw-r--r--   0        0        0        0 2024-04-15 22:17:20.139827 qai_agent-0.5.1/src/qai/agent/tools/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-15 21:28:23.268771 qai_agent-0.5.1/src/qai/agent/tools/types.py
+-rw-r--r--   0        0        0     4497 2024-04-12 13:12:16.582078 qai_agent-0.5.1/src/qai/agent/tools.py
+-rw-r--r--   0        0        0       56 2024-04-25 02:05:04.018482 qai_agent-0.5.1/src/qai/agent/utils/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-12 15:02:35.886303 qai_agent-0.5.1/src/qai/agent/utils/db_utils.py
+-rw-r--r--   0        0        0     8150 2024-05-01 16:31:43.583775 qai_agent-0.5.1/src/qai/agent/utils/distribute.py
+-rw-r--r--   0        0        0     3646 2024-04-19 23:56:44.441543 qai_agent-0.5.1/src/qai/agent/utils/utils.py
+-rw-r--r--   0        0        0     1359 2024-04-12 13:12:16.660004 qai_agent-0.5.1/src/qai/agent/vapi/qai_call.py
+-rw-r--r--   0        0        0      766 2024-04-12 13:12:16.667827 qai_agent-0.5.1/src/qai/agent/vapi/vapi_qai.py
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 qai_agent-0.5.1/PKG-INFO
```

### Comparing `qai_agent-0.5.0/pyproject.toml` & `qai_agent-0.5.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
-description = ""
+description = "Qai Agents for the Qai AI Platform"
 name = "qai-agent"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.0"
+version = "0.5.1"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 install = "^1.3.5"
-llama-index = "^0.10.30"
 llama-index-agent-openai = "^0.2.3"
 llama-index-core = "^0.10.30"
 llama-index-embeddings-huggingface = "^0.2.0"
 llama-index-embeddings-openai = "^0.1.7"
-llama-index-llms-huggingface = "^0.1.4"
 llama-index-llms-openai = "^0.1.14"
 llama-index-llms-replicate = "^0.1.3"
-llama-index-program-openai = "^0.1.5"
+llama-index-program-openai = ">=0.1.5"
 llama-index-tools-database = "^0.1.3"
 llama-index-tools-google = "^0.1.3"
 llama-index-vector-stores-mongodb = "^0.1.4"
 multiprocess = "^0.70.16"
 openai = "^1.23.2"
 pandas = "^2.2.1"
 pi-conf = "^0.7.7.5"
 pi-log = "^0.5.7.3"
 pip = "^24.0"
 pydantic = "^2.7.0"
 pymongo = "^4.6.3"
 python-dateutil = "2.8.2"
 python-dotenv = "^1.0.1"
-qai-ai = "^0.5.0"
 qai-core = "^0.5.0"
+torch = [
+    {markers = "sys_platform == 'darwin' and platform_machine == 'arm64'", source = "pypi", version = "^2.3.0"},
+    {platform = "darwin", source = "pypi", version = "^2.3.0"},
+    {platform = "linux", source = "pytorch-cpu-src", version = "=2.3.0+cpu"},
+    {platform = "win32", source = "pytorch-cpu-src", version = "=2.3.0+cpu"},
+]
+
 sqlalchemy = "^2.0.29"
+qai-ai = "0.5.2.3"
+
+[[tool.poetry.source]]
+name = "pytorch-cpu-src"
+priority = "explicit"
+url = "https://download.pytorch.org/whl/cpu"
 
 [tool.poetry.group.dev.dependencies]
 accelerate = "^0.29.3"
 bitsandbytes = "^0.42.0"
 toml-sort = "^0.23.1"
 transformers = "^4.40.1"
```

### Comparing `qai_agent-0.5.0/src/qai/agent/__init__.py` & `qai_agent-0.5.1/src/qai/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/campaign/campaign.py` & `qai_agent-0.5.1/src/qai/agent/agents/campaign/campaign.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/campaign/qrev_emailagent.py` & `qai_agent-0.5.1/src/qai/agent/agents/campaign/qrev_emailagent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/campaign copy 2.py` & `qai_agent-0.5.1/src/qai/agent/agents/campaign copy 2.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/campaign copy.py` & `qai_agent-0.5.1/src/qai/agent/agents/campaign copy.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/conversation.py` & `qai_agent-0.5.1/src/qai/agent/agents/conversation.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/email.py` & `qai_agent-0.5.1/src/qai/agent/agents/email.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/example_agent.py` & `qai_agent-0.5.1/src/qai/agent/agents/example_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/find_agent.py` & `qai_agent-0.5.1/src/qai/agent/agents/find_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/sql_query copy 2.py` & `qai_agent-0.5.1/src/qai/agent/agents/sql_query copy 2.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/sql_query copy 3.py` & `qai_agent-0.5.1/src/qai/agent/agents/sql_query copy 3.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/sql_query copy.py` & `qai_agent-0.5.1/src/qai/agent/agents/sql_query copy.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/sql_query.py` & `qai_agent-0.5.1/src/qai/agent/agents/sql_query.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/tools/outreach.py` & `qai_agent-0.5.1/src/qai/agent/agents/tools/outreach.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/tools/types.py` & `qai_agent-0.5.1/src/qai/agent/agents/tools/types.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/worker/campaign_worker copy.py` & `qai_agent-0.5.1/src/qai/agent/agents/worker/campaign_worker copy.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/worker/retry_worker copy.py` & `qai_agent-0.5.1/src/qai/agent/agents/worker/retry_worker copy.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/agents/worker/retry_worker.py` & `qai_agent-0.5.1/src/qai/agent/agents/worker/retry_worker.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/basic.py` & `qai_agent-0.5.1/src/qai/agent/basic.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/custom_bot.py` & `qai_agent-0.5.1/src/qai/agent/custom_bot.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/data/state_codes.py` & `qai_agent-0.5.1/src/qai/agent/data/state_codes.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/llama_index/llm_program.py` & `qai_agent-0.5.1/src/qai/agent/llama_index/llm_program.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/qaibot.py` & `qai_agent-0.5.1/src/qai/agent/qaibot.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/serve.py` & `qai_agent-0.5.1/src/qai/agent/serve.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/sessions/qai_session.py` & `qai_agent-0.5.1/src/qai/agent/sessions/qai_session.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/sessions/session_factory.py` & `qai_agent-0.5.1/src/qai/agent/sessions/session_factory.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/tools.py` & `qai_agent-0.5.1/src/qai/agent/tools.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/utils/distribute.py` & `qai_agent-0.5.1/src/qai/agent/utils/distribute.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/utils/utils.py` & `qai_agent-0.5.1/src/qai/agent/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/vapi/qai_call.py` & `qai_agent-0.5.1/src/qai/agent/vapi/qai_call.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.0/src/qai/agent/vapi/vapi_qai.py` & `qai_agent-0.5.1/src/qai/agent/vapi/vapi_qai.py`

 * *Files identical despite different names*

