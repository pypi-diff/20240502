# Comparing `tmp/qai_agent-0.5.1.tar.gz` & `tmp/qai_agent-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_agent-0.5.1.tar", max compression
+gzip compressed data, was "qai_agent-0.5.2.tar", max compression
```

## Comparing `qai_agent-0.5.1.tar` & `qai_agent-0.5.2.tar`

### file list

```diff
@@ -1,43 +1,28 @@
--rw-r--r--   0        0        0       37 2024-05-01 17:37:25.187159 qai_agent-0.5.1/README.md
--rw-r--r--   0        0        0     1887 2024-05-02 03:20:06.721191 qai_agent-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1227 2024-04-30 20:51:02.838309 qai_agent-0.5.1/src/qai/agent/__init__.py
--rw-r--r--   0        0        0    14064 2024-05-01 17:42:03.041730 qai_agent-0.5.1/src/qai/agent/agents/campaign/campaign.py
--rw-r--r--   0        0        0     1252 2024-05-01 15:49:03.307593 qai_agent-0.5.1/src/qai/agent/agents/campaign/qrev_emailagent.py
--rw-r--r--   0        0        0     3666 2024-04-26 02:55:26.136573 qai_agent-0.5.1/src/qai/agent/agents/campaign copy 2.py
--rw-r--r--   0        0        0     2129 2024-04-19 23:58:17.882460 qai_agent-0.5.1/src/qai/agent/agents/campaign copy.py
--rw-r--r--   0        0        0     4358 2024-04-26 02:55:29.618634 qai_agent-0.5.1/src/qai/agent/agents/conversation.py
--rw-r--r--   0        0        0    14917 2024-05-01 21:56:22.067706 qai_agent-0.5.1/src/qai/agent/agents/email.py
--rw-r--r--   0        0        0     4335 2024-04-15 04:54:10.408696 qai_agent-0.5.1/src/qai/agent/agents/example_agent.py
--rw-r--r--   0        0        0     3826 2024-04-26 00:28:53.722668 qai_agent-0.5.1/src/qai/agent/agents/find_agent.py
--rw-r--r--   0        0        0     8734 2024-04-26 02:55:32.911873 qai_agent-0.5.1/src/qai/agent/agents/sql_query copy 2.py
--rw-r--r--   0        0        0    12820 2024-04-26 02:55:35.318095 qai_agent-0.5.1/src/qai/agent/agents/sql_query copy 3.py
--rw-r--r--   0        0        0    10748 2024-04-26 02:55:38.833304 qai_agent-0.5.1/src/qai/agent/agents/sql_query copy.py
--rw-r--r--   0        0        0    11069 2024-05-01 21:11:20.490262 qai_agent-0.5.1/src/qai/agent/agents/sql_query.py
--rw-r--r--   0        0        0      442 2024-04-23 01:58:48.739947 qai_agent-0.5.1/src/qai/agent/agents/test.py
--rw-r--r--   0        0        0        0 2024-04-15 22:16:56.666275 qai_agent-0.5.1/src/qai/agent/agents/tools/__init__.py
--rw-r--r--   0        0        0     2155 2024-04-25 15:45:37.602364 qai_agent-0.5.1/src/qai/agent/agents/tools/outreach.py
--rw-r--r--   0        0        0     2369 2024-04-30 05:17:28.462522 qai_agent-0.5.1/src/qai/agent/agents/tools/types.py
--rw-r--r--   0        0        0        0 2024-04-15 04:05:07.959600 qai_agent-0.5.1/src/qai/agent/agents/worker/__init__.py
--rw-r--r--   0        0        0     4851 2024-04-26 02:55:42.760558 qai_agent-0.5.1/src/qai/agent/agents/worker/campaign_worker copy.py
--rw-r--r--   0        0        0     5401 2024-04-24 15:51:11.790090 qai_agent-0.5.1/src/qai/agent/agents/worker/retry_worker copy.py
--rw-r--r--   0        0        0     4046 2024-04-24 15:44:27.850895 qai_agent-0.5.1/src/qai/agent/agents/worker/retry_worker.py
--rw-r--r--   0        0        0     3951 2024-04-26 02:55:13.429897 qai_agent-0.5.1/src/qai/agent/basic.py
--rw-r--r--   0        0        0     2972 2024-04-12 13:12:16.580326 qai_agent-0.5.1/src/qai/agent/custom_bot.py
--rw-r--r--   0        0        0        0 2024-04-12 13:12:16.649604 qai_agent-0.5.1/src/qai/agent/data/__init__.py
--rw-r--r--   0        0        0     1284 2024-04-12 13:12:16.649487 qai_agent-0.5.1/src/qai/agent/data/state_codes.py
--rw-r--r--   0        0        0     1671 2024-04-26 21:05:29.498832 qai_agent-0.5.1/src/qai/agent/llama_index/llm_program.py
--rw-r--r--   0        0        0      170 2024-04-24 22:13:53.649180 qai_agent-0.5.1/src/qai/agent/models.py
--rw-r--r--   0        0        0     4683 2024-04-25 21:15:40.430411 qai_agent-0.5.1/src/qai/agent/qaibot.py
--rw-r--r--   0        0        0     3404 2024-04-26 00:29:13.276728 qai_agent-0.5.1/src/qai/agent/serve.py
--rw-r--r--   0        0        0     1658 2024-04-25 21:15:55.808197 qai_agent-0.5.1/src/qai/agent/sessions/qai_session.py
--rw-r--r--   0        0        0      623 2024-04-19 23:56:44.441519 qai_agent-0.5.1/src/qai/agent/sessions/session_factory.py
--rw-r--r--   0        0        0        0 2024-04-15 22:17:20.139827 qai_agent-0.5.1/src/qai/agent/tools/__init__.py
--rw-r--r--   0        0        0      423 2024-04-15 21:28:23.268771 qai_agent-0.5.1/src/qai/agent/tools/types.py
--rw-r--r--   0        0        0     4497 2024-04-12 13:12:16.582078 qai_agent-0.5.1/src/qai/agent/tools.py
--rw-r--r--   0        0        0       56 2024-04-25 02:05:04.018482 qai_agent-0.5.1/src/qai/agent/utils/__init__.py
--rw-r--r--   0        0        0      397 2024-04-12 15:02:35.886303 qai_agent-0.5.1/src/qai/agent/utils/db_utils.py
--rw-r--r--   0        0        0     8150 2024-05-01 16:31:43.583775 qai_agent-0.5.1/src/qai/agent/utils/distribute.py
--rw-r--r--   0        0        0     3646 2024-04-19 23:56:44.441543 qai_agent-0.5.1/src/qai/agent/utils/utils.py
--rw-r--r--   0        0        0     1359 2024-04-12 13:12:16.660004 qai_agent-0.5.1/src/qai/agent/vapi/qai_call.py
--rw-r--r--   0        0        0      766 2024-04-12 13:12:16.667827 qai_agent-0.5.1/src/qai/agent/vapi/vapi_qai.py
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 qai_agent-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-01 17:37:25.187159 qai_agent-0.5.2/README.md
+-rw-r--r--   0        0        0     1920 2024-05-02 05:30:20.088645 qai_agent-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1227 2024-04-30 20:51:02.838309 qai_agent-0.5.2/src/qai/agent/__init__.py
+-rw-r--r--   0        0        0    10173 2024-05-02 05:19:41.510594 qai_agent-0.5.2/src/qai/agent/agents/campaign/campaign.py
+-rw-r--r--   0        0        0     4358 2024-04-26 02:55:29.618634 qai_agent-0.5.2/src/qai/agent/agents/conversation.py
+-rw-r--r--   0        0        0    13135 2024-05-02 05:19:09.399319 qai_agent-0.5.2/src/qai/agent/agents/email.py
+-rw-r--r--   0        0        0     3389 2024-05-02 05:19:15.871949 qai_agent-0.5.2/src/qai/agent/agents/example_agent.py
+-rw-r--r--   0        0        0     3505 2024-05-02 05:18:58.522327 qai_agent-0.5.2/src/qai/agent/agents/find_agent.py
+-rw-r--r--   0        0        0    11013 2024-05-02 05:18:49.979317 qai_agent-0.5.2/src/qai/agent/agents/sql_query.py
+-rw-r--r--   0        0        0        0 2024-04-15 22:16:56.666275 qai_agent-0.5.2/src/qai/agent/agents/tools/__init__.py
+-rw-r--r--   0        0        0     1399 2024-05-02 05:23:24.210450 qai_agent-0.5.2/src/qai/agent/agents/tools/outreach.py
+-rw-r--r--   0        0        0        0 2024-04-15 04:05:07.959600 qai_agent-0.5.2/src/qai/agent/agents/worker/__init__.py
+-rw-r--r--   0        0        0     3166 2024-05-02 05:21:41.273125 qai_agent-0.5.2/src/qai/agent/basic.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:12:16.649604 qai_agent-0.5.2/src/qai/agent/data/__init__.py
+-rw-r--r--   0        0        0     1284 2024-04-12 13:12:16.649487 qai_agent-0.5.2/src/qai/agent/data/state_codes.py
+-rw-r--r--   0        0        0     1322 2024-05-02 05:19:57.743021 qai_agent-0.5.2/src/qai/agent/llama_index/llm_program.py
+-rw-r--r--   0        0        0      170 2024-04-24 22:13:53.649180 qai_agent-0.5.2/src/qai/agent/models.py
+-rw-r--r--   0        0        0     3312 2024-05-02 05:21:46.573311 qai_agent-0.5.2/src/qai/agent/qaibot.py
+-rw-r--r--   0        0        0     3403 2024-05-02 05:21:56.520197 qai_agent-0.5.2/src/qai/agent/serve.py
+-rw-r--r--   0        0        0     1270 2024-05-02 05:20:08.067204 qai_agent-0.5.2/src/qai/agent/sessions/qai_session.py
+-rw-r--r--   0        0        0        0 2024-04-15 22:17:20.139827 qai_agent-0.5.2/src/qai/agent/tools/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-15 21:28:23.268771 qai_agent-0.5.2/src/qai/agent/tools/types.py
+-rw-r--r--   0        0        0     4497 2024-04-12 13:12:16.582078 qai_agent-0.5.2/src/qai/agent/tools.py
+-rw-r--r--   0        0        0       56 2024-04-25 02:05:04.018482 qai_agent-0.5.2/src/qai/agent/utils/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-12 15:02:35.886303 qai_agent-0.5.2/src/qai/agent/utils/db_utils.py
+-rw-r--r--   0        0        0     8150 2024-05-01 16:31:43.583775 qai_agent-0.5.2/src/qai/agent/utils/distribute.py
+-rw-r--r--   0        0        0     3636 2024-05-02 05:21:23.859476 qai_agent-0.5.2/src/qai/agent/utils/utils.py
+-rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 qai_agent-0.5.2/PKG-INFO
```

### Comparing `qai_agent-0.5.1/pyproject.toml` & `qai_agent-0.5.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
 description = "Qai Agents for the Qai AI Platform"
 name = "qai-agent"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.1"
+version = "0.5.2"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 install = "^1.3.5"
 llama-index-agent-openai = "^0.2.3"
 llama-index-core = "^0.10.30"
 llama-index-embeddings-huggingface = "^0.2.0"
@@ -20,45 +20,45 @@
 llama-index-llms-openai = "^0.1.14"
 llama-index-llms-replicate = "^0.1.3"
 llama-index-program-openai = ">=0.1.5"
 llama-index-tools-database = "^0.1.3"
 llama-index-tools-google = "^0.1.3"
 llama-index-vector-stores-mongodb = "^0.1.4"
 multiprocess = "^0.70.16"
+mysql-connector-python = "^8.4.0"
 openai = "^1.23.2"
 pandas = "^2.2.1"
 pi-conf = "^0.7.7.5"
 pi-log = "^0.5.7.3"
 pip = "^24.0"
 pydantic = "^2.7.0"
 pymongo = "^4.6.3"
 python-dateutil = "2.8.2"
 python-dotenv = "^1.0.1"
+qai-ai = "0.5.2.3"
 qai-core = "^0.5.0"
+sqlalchemy = "^2.0.29"
 torch = [
     {markers = "sys_platform == 'darwin' and platform_machine == 'arm64'", source = "pypi", version = "^2.3.0"},
     {platform = "darwin", source = "pypi", version = "^2.3.0"},
     {platform = "linux", source = "pytorch-cpu-src", version = "=2.3.0+cpu"},
     {platform = "win32", source = "pytorch-cpu-src", version = "=2.3.0+cpu"},
 ]
 
-sqlalchemy = "^2.0.29"
-qai-ai = "0.5.2.3"
-
-[[tool.poetry.source]]
-name = "pytorch-cpu-src"
-priority = "explicit"
-url = "https://download.pytorch.org/whl/cpu"
-
 [tool.poetry.group.dev.dependencies]
 accelerate = "^0.29.3"
 bitsandbytes = "^0.42.0"
 toml-sort = "^0.23.1"
 transformers = "^4.40.1"
 
+[[tool.poetry.source]]
+name = "pytorch-cpu-src"
+priority = "explicit"
+url = "https://download.pytorch.org/whl/cpu"
+
 [tool.tomlsort]
 all = true
 in_place = true
 spaces_before_inline_comment = 2  # Match Python PEP 8
 spaces_indent_inline_array = 4  # Match Python PEP 8
 trailing_comma_inline_array = true
 overrides."tool.poetry.dependencies".first = ["python"]
```

### Comparing `qai_agent-0.5.1/src/qai/agent/__init__.py` & `qai_agent-0.5.2/src/qai/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.1/src/qai/agent/agents/campaign/campaign.py` & `qai_agent-0.5.2/src/qai/agent/agents/campaign/campaign.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,26 @@
 import uuid
-from collections import defaultdict
-from dataclasses import dataclass, field
-from enum import StrEnum
-from functools import partial
-from typing import Any, Dict, List, Optional, Self, Sequence, Type, TypeVar, Union
+from dataclasses import dataclass
+from typing import Any, Dict, List, Optional, Self, Union
 
-import requests
 from llama_index.agent.openai import OpenAIAgent
-from llama_index.agent.openai.base import DEFAULT_MAX_FUNCTION_CALLS
-from llama_index.agent.openai.step import OpenAIAgentWorker
-from llama_index.core import SQLDatabase
 from llama_index.core.agent import AgentChatResponse, Task
-from llama_index.core.agent.runner.base import AgentRunner
 from llama_index.core.agent.types import Task
-from llama_index.core.base.llms.types import ChatMessage, MessageRole
+from llama_index.core.base.llms.types import ChatMessage
 from llama_index.core.bridge.pydantic import BaseModel, Field
-from llama_index.core.callbacks import CallbackManager
 from llama_index.core.chat_engine.types import AgentChatResponse
 from llama_index.core.llms import ChatMessage
-from llama_index.core.llms.llm import LLM
-from llama_index.core.memory import ChatMemoryBuffer
-from llama_index.core.memory.chat_memory_buffer import ChatMemoryBuffer
-from llama_index.core.memory.types import BaseMemory
-from llama_index.core.objects.base import ObjectRetriever
-from llama_index.core.query_engine import NLSQLTableQueryEngine
-from llama_index.core.query_pipeline import CustomQueryComponent
-from llama_index.core.settings import Settings
-from llama_index.core.storage.chat_store import SimpleChatStore
-from llama_index.core.tools import BaseTool, FunctionTool, QueryEngineTool
+from llama_index.core.tools import BaseTool
 from llama_index.core.tools.tool_spec.base import BaseToolSpec
-from llama_index.core.tools.types import BaseTool, ToolMetadata
-from llama_index.llms.openai import OpenAI
-from llama_index.llms.openai.utils import OpenAIToolCall
-from pi_conf import AttrDict, load_config
-from pi_log import logs
-from pymongo import MongoClient
-from qai.ai import MessageRole, QueryReturn, to_message
-from qai.ai.frameworks.openai.llm import OpenAILLM
-from sqlalchemy import create_engine
+from llama_index.core.tools.types import BaseTool
 
 from qai.agent import cfg
-from qai.agent.agents.find_agent import AgentType, FindAgentWorker
+from qai.agent.agents.email import EmailAgent, EmailModel
 from qai.agent.agents.sql_query import RefineSQLQuery, StepModel
-from qai.agent.agents.email import EmailModel, EmailAgent
-from qai.agent.agents.tools.outreach import OutreachToolSpec
 from qai.agent.models import OutreachType
-from qai.agent.qaibot import QaiSession
-from qai.agent.sessions.qai_session import QaiSession
-from qai.agent.tools.types import StringEnum
-from qai.agent.utils.distribute import adistribute
 
 
 class PersonID(BaseModel):
     id: str = Field(description="The database id of the person.")
 
 
 class PersonModel(BaseModel):
@@ -167,19 +135,14 @@
         """
         print(f"Chatting with message {message} and tool_choice {tool_choice}")
         print(
             f"  People IDs: {len(self.people)}, company IDs: {len(self.companies)}, "
             f"outreach types: {len(self.outreach_types)}"
         )
 
-        # host (Optional[str]): host of the database connection.
-        # port (Optional[int]): port of the database connection.
-        # user (Optional[str]): user of the database connection.
-        # password (Optional[str]): password of the database connection.
-
         refine_tools = RefineSQLQuery(**cfg.db)
 
         refining_agent = OpenAIAgent.from_tools(
             refine_tools.to_tool_list(),
             verbose=True,
             system_prompt=refine_tools.refine_query_system_message,
         )
@@ -284,62 +247,7 @@
         agent.from_person = from_person or {}
         agent.from_company = from_company or {}
         agent.email_agent = email_agent or EmailAgent.create(
             agent.from_person,
             agent.from_company,
         )
         return agent
-
-
-if __name__ == "__main__":
-    from pprint import pprint
-
-    from pi_conf import AttrDict, load_config
-
-    cfg = load_config("qai")
-    cfg.to_env()
-    # Create a new CampaignToolSpec object
-    campaign_tool = CampaignToolSpec(companies=["Apple", "Google", "Microsoft"])
-    # find_outreach_tool = OutreachToolSpec()
-    # pprint(campaign_tool.to_tool_list()[0].metadata.to_openai_function())
-    tools = campaign_tool.to_tool_list()
-
-    agent = CampaignAgent.from_tools(
-        tools=tools,
-        system_prompt=(
-            "Create a campaign for a list of people and companies. If a parameter is missing, please ask for it, do not try to infer it."
-        ),
-        verbose=True,
-    )
-    # llm = OpenAI(model="gpt-3.5-turbo", temperature=0.0)
-    # OpenAIAgent
-    # agent = OpenAIAgent(llm=llm, callback_manager=llm.callback_manager)
-    r = agent.chat("Make an email campaign ")
-    # pprint(r)
-    # r = agent.chat("Sure, send them emails")
-    pprint(r)
-    r = agent.chat("Umm, to 5 of the some heads of companies around las vegas")
-    pprint(r)
-    print("DONE")
-    # from qai.ai.frameworks.openai.llm import OpenAILLM
-    # llm = OpenAILLM(config={"name":"gpt-3.5-turbo", "temperature":0.0})
-    # msgs = [
-    #     {"role": "system", "content": "Create a campaign for a list of people and companies. If a parameter is missing, please ask for it, do not try to infer it."},
-    #     {"role": "user", "content": "Make a campaign "},
-    # ]
-    # msgs = [m.dict() for m in msgs]
-    # print(msgs)
-    # qr = llm.query(
-    #     messages=msgs,
-    #     tools=[campaign_tool.to_tool_list()[0].metadata.to_openai_tool()],
-    #     tool_choice="auto",
-    #     validate=True,
-    #     # required_fields=["steps"],
-    # )
-    # print(qr.response)
-
-    # r = agent.chat("Make a campaign ")
-    # pprint(r)
-    # r = agent.chat("Sure, send them emails")
-    # pprint(r)
-    # r = agent.chat("Umm, to the head of google")
-    # pprint(r)
```

### Comparing `qai_agent-0.5.1/src/qai/agent/agents/conversation.py` & `qai_agent-0.5.2/src/qai/agent/agents/conversation.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.1/src/qai/agent/agents/email.py` & `qai_agent-0.5.2/src/qai/agent/agents/email.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,28 @@
 import os
-import uuid
-from collections import defaultdict
-from dataclasses import dataclass, field
-from enum import StrEnum
 from functools import partial
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Self,
-    Sequence,
-    Type,
-    TypeVar,
-    Union,
-)
+from logging import getLogger
+from typing import Callable, List, Optional, Self, Union
 
 import requests
 from llama_index.agent.openai import OpenAIAgent
-from llama_index.agent.openai.base import DEFAULT_MAX_FUNCTION_CALLS
-from llama_index.agent.openai.step import OpenAIAgentWorker
-from llama_index.core import SQLDatabase
-from llama_index.core.agent import AgentChatResponse, Task
-from llama_index.core.agent.runner.base import AgentRunner
-from llama_index.core.agent.types import Task
-from llama_index.core.base.llms.types import ChatMessage, MessageRole
+from llama_index.core.agent import AgentChatResponse
+from llama_index.core.base.llms.types import ChatMessage
 from llama_index.core.bridge.pydantic import BaseModel, Field
-from llama_index.core.callbacks import CallbackManager
 from llama_index.core.chat_engine.types import AgentChatResponse
 from llama_index.core.llms import ChatMessage
-from llama_index.core.llms.llm import LLM
-from llama_index.core.memory import ChatMemoryBuffer
-from llama_index.core.memory.chat_memory_buffer import ChatMemoryBuffer
-from llama_index.core.memory.types import BaseMemory
-from llama_index.core.objects.base import ObjectRetriever
 from llama_index.core.program import LLMTextCompletionProgram
-from llama_index.core.query_engine import NLSQLTableQueryEngine
-from llama_index.core.query_pipeline import CustomQueryComponent
-from llama_index.core.settings import Settings
-from llama_index.core.storage.chat_store import SimpleChatStore
-from llama_index.core.tools import BaseTool, FunctionTool, QueryEngineTool
+from llama_index.core.tools import BaseTool
 from llama_index.core.tools.tool_spec.base import BaseToolSpec
-from llama_index.core.tools.types import BaseTool, ToolMetadata
-from llama_index.llms.openai import OpenAI
-from llama_index.llms.openai.utils import OpenAIToolCall
-from pi_conf import AttrDict, load_config
-from pi_log import logs
+from llama_index.core.tools.types import BaseTool
 from pydantic import BaseModel, Field
 from pymongo import MongoClient
-from qai.ai import MessageRole, QueryReturn, to_message
-from qai.ai.frameworks.openai.llm import OpenAILLM
-from sqlalchemy import create_engine
 
 from qai.agent import ROOT_DIR, cfg
-from qai.agent.agents.find_agent import AgentType, FindAgentWorker
-from qai.agent.agents.sql_query import RefineSQLQuery, StepModel
-from qai.agent.agents.tools.outreach import OutreachToolSpec
-from qai.agent.models import OutreachType
-from qai.agent.qaibot import QaiSession
-from qai.agent.sessions.qai_session import QaiSession
-from qai.agent.tools.types import StringEnum
 from qai.agent.utils.distribute import adistribute
-from logging import getLogger
 
 log = getLogger(__name__)
 PROJ_DIR = os.path.dirname(os.path.dirname(os.path.dirname(ROOT_DIR)))
 
 example_template = """"""
 job_title_template = """, who holds the job title {job_title}"""
 industry_template = """Industry of {company_name} is {industry}"""
@@ -279,15 +235,18 @@
     def _create_emails(
         kwargs_list: list[dict],
         on_complete: Optional[Callable] = None,
         asynchronous: bool = True,
     ) -> None:
         if asynchronous:
             adistribute(
-                EmailToolSpec._create_email, kwargs_list=kwargs_list, on_complete=on_complete
+                EmailToolSpec._create_email,
+                kwargs_list=kwargs_list,
+                on_complete=on_complete,
+                nprocs=4,
             )
         else:
             for kwargs in kwargs_list:
                 EmailToolSpec._create_email(**kwargs)
             if on_complete:
                 on_complete()
 
@@ -302,42 +261,40 @@
         chat_history: Optional[List[ChatMessage]] = None,
         tool_choice: Optional[Union[str, dict]] = None,
     ) -> AgentChatResponse:
         return super().chat(message, chat_history, tool_choice)
 
     @staticmethod
     def on_email_complete(sequence_id, email: EmailModel) -> None:
-        log.debug(f"Email completed: {sequence_id} {email}")
-        mongo = cfg.db.mongo
+        print(f"Email completed: {sequence_id} {email}")
+        mongo = cfg.mongo
         client = MongoClient(mongo.uri)
         db = client[mongo.db]
 
         collection = db[mongo.collection]
         js = {
             "sequence_id": sequence_id,
             "prospect_email": email.email,
             "prospect_name": email.name,
             "prospect_phone": email.phone,
             "message_subject": email.subject,
             "message_body": email.body,
             "is_message_generation_complete": True,
         }
-        log.debug(f"Inserting into collection: {mongo.uri} {db} {collection.name} ")
+        print(f"Inserting into collection: {mongo.uri} {db} {collection.name} ")
         result = collection.insert_one(js)
-        log.debug(f"Insert Result: {result}")
+        print(f"Insert Result: {result}")
 
     @staticmethod
-    def on_all_emails_complete(sequence_id: str,  successes: int, errors: int) -> None:
-        log.debug(f"All Email completed: {successes} success, {errors} errors.")
+    def on_all_emails_complete(sequence_id: str, successes: int, errors: int) -> None:
+        print(f"All Email completed: {successes} success, {errors} errors.")
         url = cfg.email.on_complete_emails_url
-        log.debug(f"Sending call to {url}  sequence_id={sequence_id}")
-        r = requests.post(
-            url, json={"sequence_id": sequence_id}
-        )
-        log.debug(r.json())
+        print(f"Sending call to {url}  sequence_id={sequence_id}")
+        r = requests.post(url, json={"sequence_id": sequence_id})
+        print(r.json())
 
     def create_emails(
         self,
         sequence_id: str,
         from_person: dict,
         from_company: dict,
         to_people: dict,
```

### Comparing `qai_agent-0.5.1/src/qai/agent/agents/find_agent.py` & `qai_agent-0.5.2/src/qai/agent/agents/find_agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-from enum import StrEnum
-from typing import Any, Callable, Dict, List, Optional, Self, Sequence, Type
+from typing import Any, Callable, Dict, List, Optional, Sequence, Type
 
 from llama_index.agent.openai import OpenAIAgent
 from llama_index.agent.openai.base import DEFAULT_MAX_FUNCTION_CALLS
-from llama_index.agent.openai.step import OpenAIAgentWorker
-from llama_index.core.agent.runner.base import AgentRunner
 from llama_index.core.base.llms.types import ChatMessage
 from llama_index.core.bridge.pydantic import BaseModel, Field
 from llama_index.core.callbacks import CallbackManager
 from llama_index.core.llms.llm import LLM
 from llama_index.core.memory import ChatMemoryBuffer
 from llama_index.core.memory.chat_memory_buffer import ChatMemoryBuffer
 from llama_index.core.memory.types import BaseMemory
 from llama_index.core.objects.base import ObjectRetriever
-from llama_index.core.settings import Settings
-from llama_index.core.storage.chat_store import SimpleChatStore
-from llama_index.core.tools import BaseTool, FunctionTool, QueryEngineTool
+from llama_index.core.tools import BaseTool, FunctionTool
 from llama_index.core.tools.types import ToolMetadata
-from llama_index.llms.openai import OpenAI
 from llama_index.llms.openai.utils import OpenAIToolCall
 
 from qai.agent.tools.types import StringEnum
 
 
 class AgentType(StringEnum):
     campaign = "campaign"
```

### Comparing `qai_agent-0.5.1/src/qai/agent/agents/sql_query copy 3.py` & `qai_agent-0.5.2/src/qai/agent/agents/sql_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,42 @@
 import os
-import re
-import uuid
-from abc import abstractmethod
-from collections import defaultdict, deque
-from dataclasses import dataclass, field
-from inspect import signature
+from typing import List, Optional
+
+from llama_index.core import SQLDatabase
 from llama_index.core.base.response.schema import Response
-from pprint import pprint
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    Deque,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-    cast,
-)
-
-import llama_index.core.instrumentation as instrument
-from llama_index.agent.openai import OpenAIAgent
-from llama_index.agent.openai.base import DEFAULT_MAX_FUNCTION_CALLS
-from llama_index.agent.openai.step import OpenAIAgentWorker
-from llama_index.core import PromptTemplate, Settings, SQLDatabase
-from llama_index.core.agent.runner.base import AgentRunner
-from pydantic.type_adapter import TypeAdapter
-from llama_index.core.agent.types import (
-    BaseAgent,
-    BaseAgentWorker,
-    Task,
-    TaskStep,
-    TaskStepOutput,
-)
-from llama_index.core.base.llms.types import (
-    ChatMessage,
-    ChatResponse,
-    ChatResponseAsyncGen,
-    ChatResponseGen,
-    CompletionResponse,
-    CompletionResponseAsyncGen,
-    CompletionResponseGen,
-    LLMMetadata,
-    MessageRole,
-)
 from llama_index.core.bridge.pydantic import BaseModel, Field
-
-# from pydantic.v1 import BaseModel, Field
-from llama_index.core.callbacks import (
-    CallbackManager,
-    CBEventType,
-    EventPayload,
-    trace_method,
-)
-from llama_index.core.chat_engine.types import (
-    AGENT_CHAT_RESPONSE_TYPE,
-    AgentChatResponse,
-    ChatResponseMode,
-    StreamingAgentChatResponse,
-)
-from llama_index.core.instrumentation.events.agent import (
-    AgentChatWithStepEndEvent,
-    AgentChatWithStepStartEvent,
-    AgentRunStepEndEvent,
-    AgentRunStepStartEvent,
-)
-from llama_index.core.llms import ChatMessage
 from llama_index.core.llms.llm import LLM
-from llama_index.core.memory import BaseMemory, ChatMemoryBuffer
-from llama_index.core.memory.chat_memory_buffer import ChatMemoryBuffer
-from llama_index.core.memory.types import BaseMemory
-from llama_index.core.objects.base import ObjectRetriever
 from llama_index.core.query_engine import NLSQLTableQueryEngine
-from llama_index.core.query_pipeline import CustomQueryComponent
-from llama_index.core.settings import Settings
-from llama_index.core.storage.chat_store import SimpleChatStore
-from llama_index.core.tools import BaseTool, FunctionTool, QueryEngineTool
-from llama_index.core.tools.function_tool import FunctionTool
-from llama_index.core.tools.tool_spec.base import BaseToolSpec
-from llama_index.core.tools.types import BaseTool, ToolMetadata
-from llama_index.core.tools.utils import create_schema_from_function
-from llama_index.llms.huggingface import HuggingFaceLLM
-from llama_index.llms.openai import OpenAI
-from llama_index.llms.openai.utils import OpenAIToolCall
+from llama_index.core.tools.types import ToolOutput
 from llama_index.tools.database import DatabaseToolSpec
-from pi_conf import AttrDict, load_config
-from pi_log import logs
-
-from qai.ai import MessageRole, QueryReturn, to_message
-from qai.ai.frameworks.openai.llm import OpenAILLM
-from sqlalchemy import create_engine
+from qai.ai import QueryReturn
+from sqlalchemy import create_engine, text
 from sqlalchemy.exc import NoSuchTableError
 from sqlalchemy.schema import CreateTable
 
-from qai.agent import ROOT_DIR, cfg
-from qai.agent.agents.find_agent import AgentType, FindAgentWorker
-from qai.agent.qaibot import QaiBot, QaiSession
-from qai.agent.sessions.qai_session import QaiSession
-from qai.agent.tools.types import StringEnum
-from pydantic.tools import parse_obj_as
+from qai.agent import ROOT_DIR
 
-PROJ_DIR = os.path.dirname(os.path.dirname(os.path.dirname(ROOT_DIR)))
-import pydantic
+# Current supported fields in backend: email, name, phone_number, company_name, company_url, job_title, linkedin_url, timezone
 
-# db_config = {"connect_str": f"sqlite:///{PROJ_DIR}/scripts/qrev-org-intel.merged.sqlite3"}
-# print(db_config)
-from llama_index.core.agent.runner.base import dispatcher
+PROJ_DIR = os.path.dirname(os.path.dirname(os.path.dirname(ROOT_DIR)))
 
-Settings.llm = OpenAI(model="gpt-3.5-turbo", temperature=0.0)
 
+# Settings.llm = OpenAI(model="gpt-4", temperature=0.0)
 
 
 class PeopleIds(BaseModel):
-    id : str = Field(..., description="The id of the person")
+    id: str = Field(..., description="The id of the person")
+
 
 class CompanyIds(BaseModel):
-    id : str = Field(..., description="The id of the company")
+    id: str = Field(..., description="The id of the company")
+
 
 class IndustryIds(BaseModel):
-    id : str = Field(..., description="The id of the industry")
+    id: str = Field(..., description="The id of the industry")
 
 
 class StepModel(BaseModel):
     sentence: str = Field(
         ...,
         description=(
             "A revised sentence that captures the business logic. the revised sentence keeps details such as numbers."
@@ -140,30 +52,41 @@
 
 class RefineSQLQuery(DatabaseToolSpec):
     """Simple Database tool."""
 
     ## List of tables in the database, None for all tables
     tables: Optional[list[str]] = None
     llm: Optional[LLM] = None
+    limit: int = None  ## Limit the number of results returned
 
     refine_query_system_message: str = (
         "Separate the text into a list of logical execution steps for a business user and categorize the step."
+        "Do not create steps, only refine the given sentences into logical execution steps."
         "The steps should be in the order of execution. "
+        "If there are no steps ask for clarification."
         "Keep details such as quantities or numbers."
-        "WHen choosing a category only use one of the following: {categories}"
+        "When choosing a category only use one of the following: [company, people, industry, location, time, campaign, email, extraneous]"
         "For example if the user query is 'Get me the head of sales for the top 5 companies in the seattle area' and the following database schema {schema}, the refined query should be: "
         "step: Get the top 5 companies in the seattle area, category: company"
         "step: Get the head of sales for each company, category: people"
         ""
     )
-    spec_functions = ["find_steps", "load_data", "describe_tables", "list_tables"]
+    spec_functions = [
+        "find_steps",
+        "load_data",
+        "describe_tables",
+        "list_tables",
+        "load_people",
+        "load_companies",
+    ]
 
-    def __init__(self, llm: LLM = None, *args, **kwargs):
+    def __init__(self, llm: LLM = None, limit: int = 5, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.llm = llm
+        self.limit = limit
         ## get columns from the database
         self.columns = self.list_tables
         # self.spec_functions.extend(self.extra_spec_functions)
 
     def tables_to_json(self, tables: Optional[List[str]] = None) -> dict:
         """
         Converts the specified tables in the database into a simple json format
@@ -187,26 +110,38 @@
                     s = str(col).split(" ")
                     name = s[0].strip('"')
                     type = s[1]
                     columns.append({"name": name, "type": type})
             except:
                 raise
             json_tables[table_name] = columns
-
         return json_tables
 
+    @staticmethod
+    def sources_to_json(sources: list) -> list[dict]:
+        if not sources:
+            return {}
+        source: ToolOutput
+        for source in sources:
+            if source.raw_output:
+                return source.raw_output
+
     def query(self, query: str) -> QueryReturn:
         return self.query_engine.query(query)
 
     def find_steps(self, steps: list[StepModel]) -> list[StepModel]:
         """
-        Separate the text into a list of logical execution steps for a business user.
+        Separate the text into a list of logical execution steps for a business user and categorize the step.
+        Do not create steps, only refine the given sentences into logical execution steps.
         The steps should be in the order of execution.
         Keep details such as quantities or numbers.
-        Non business steps should be classified as extraneous.
+        When choosing a category only use one of the following: [company, people, industry, location, time, campaign, email, extraneous]
+        For example if the user query is 'Get me the head of sales for the top 5 companies in the seattle area' the refined query should be:
+        step: Get the top 5 companies in the seattle area, category: company
+        step: Get the head of sales for each company, category: people
 
         Args:
             steps (List[StepModel]): A list of StepModel objects, each containing a sentence and a category
 
         """
         ## Input is not perfect from the llm, it can be a list of steps but in dict form
         ## or it can be a dict with a list of dicts
@@ -262,106 +197,84 @@
         Returns:
             list[StepModel]: The refined list of steps.
         """
 
         steps = self._merge_steps(steps)
         return steps
 
-
-    def load_people(self, query: str) -> List[PeopleIds]:
+    def load_people(self, query: str) -> List[dict]:
         """
         Load people from the database using the query.
         Args:
             query (str): Natural language of the query to load people from the database.
         Returns:
-            List[PeopleIds]: A list of people ids.
+            List[dict[str, str]]: A list of dict, containing the people information.
         """
+        if isinstance(query, dict):
+            query = query["query"]
+        engine = create_engine(self.uri)
+        tables = ["Companies", "Industries", "CompanyIndustries", "People"]
+
+        sql_database = SQLDatabase(engine, include_tables=tables)
+        query += "return all the people information using '*' in the resulting sql query."
+        if self.limit:
+            query += f" Place a limit of {self.limit} on the resulting query"
+
+        query_engine = NLSQLTableQueryEngine(
+            sql_database=sql_database,
+            tables=tables,
+        )
+        return_dict = []
+        r: Response = query_engine.query(str(query))
+        if r.metadata and "sql_query" in r.metadata:
+            sql_query = r.metadata["sql_query"]
+            print("##", sql_query)
+            with self.sql_database.engine.connect() as connection:
+                result = connection.execute(text(sql_query))
+                for item in result.fetchall():
+                    return_dict.append({k: v for k, v in zip(item._fields, item._t)})
+        return return_dict
 
-
-
-if __name__ == "__main__":
-    cfg = load_config("qai-chat")
-    # db_config = cfg["db"]
-
-    # pprint(cfg.db)
-    refine_tools = RefineSQLQuery(
-        uri=cfg.db.uri, 
-    )
-    db_tools = DatabaseToolSpec(
-        uri=cfg.db.uri,
-    )
-
-    query = "Get me the head of sales for the top 5 companies in the seattle area"
-    query += "Only use the tool 'find_steps' to refine the query."
-    # # #
-    # tools = db_tools.to_tool_list()
-    # # # pprint(tools[0].metadata.to_openai_function())
-    refining_agent = OpenAIAgent.from_tools(refine_tools.to_tool_list(), verbose=True)
-    r = refining_agent.chat(query, tool_choice="find_steps")
-    # r = agent.run_step()
-    # # # # r = db_tools.refine_query(query)
-    print("@@@@@@@@@")
-    print(r)
-    print("!!!!!!!!!!!!!!!!!!")
-    query2_list = []
-    try:
-        source = r.sources[-1]
-        for raw_output in source.raw_output:
-            print("   ###########")
-            sm: StepModel = raw_output
-            query2_list.append(sm.sentence)
-        query2 = " ".join(query2_list)
-    except:
-        raise
-    # query2 = " ".join([s["sentence"] for s in r.sources if r.category != "extraneous"])
-    # agent = OpenAIAgent.from_tools(db_tools.to_tool_list(), verbose=True)
-    print(f" ###### Q2 = {query2} ######")
-    engine = create_engine(cfg.db.uri)
-    tables = ["Companies", "Industries", "CompanyIndustries", "People"]
-
-    sql_database = SQLDatabase(engine, include_tables=tables)
-
-    query_engine = NLSQLTableQueryEngine(
-        sql_database=sql_database,
-        tables=tables,
-    )
-    query2 += "return all the information using '*' in the resulting sql query"
-    r2: Response = query_engine.query(str(query2))
-    # r2 = agent.chat(query2)
-
-    print("@@@@@@@@@")
-    print(r2)
-    print("!!!!!!!!!!!!!!!!!!")
-    sql_query = None
-    if r2.metadata and "sql_query" in r2.metadata:
-        sql_query = r2.metadata["sql_query"]
-        print("##", sql_query)
-
-    # r3 = agent.chat("actually, I want to see 5 different companies")
-    # print("@@@@@@@@@ R3")
-    # print(r3)
-    # print("!!!!!!!!!!!!!!!!!!")
-    print("@*#*#*# DONE @*#*#*#")
-    # engine = create_engine(cfg.db.uri)
-    # tables = ["Companies", "Industries", "CompanyIndustries"]
-    # if True:
-    #     sql_database = SQLDatabase(engine, include_tables=tables)
-
-    #     query_engine = NLSQLTableQueryEngine(
-    #         sql_database=sql_database,
-    #         tables=tables,
-    #     )
-
-    #     # print("****************")
-    #     qr = query_engine.query(str(query))
-    #     print("!!!!!!!!!!!!!!!!!!")
-    #     print(qr)
-    #     if qr.metadata and "sql_query" in qr.metadata:
-    #         sql_query = qr.metadata["sql_query"]
-    #         print("##", sql_query)
-
-    #     # print(agent.chat(str(r)))
-    # else:
-    #     agent = OpenAIAgent.from_tools(db_tools.to_tool_list(), verbose=True)
-    #     qr = agent.chat(str(r))
-    # print("@@@@@@@@@")
-    # print(qr)
+    def load_companies(self, query: str) -> List[dict]:
+        """
+        Load companies from the database using the query.
+        Args:
+            query (str): Natural language of the query to load companies from the database.
+        Returns:
+            List[dict]: A list of dict, containing the company information.
+        """
+        if isinstance(query, dict):
+            query = query["query"]
+        engine = create_engine(self.uri)
+        tables = ["Companies", "Industries", "CompanyIndustries", "People"]
+        query += "Return all the company information using '*' in the resulting sql query."
+        if self.limit:
+            query += f" place a limit of {self.limit} on the resulting query"
+
+        sql_database = SQLDatabase(engine, include_tables=tables)
+
+        query_engine = NLSQLTableQueryEngine(
+            sql_database=sql_database,
+            tables=tables,
+        )
+        return_dict = []
+        r: Response = query_engine.query(str(query))
+        if r.metadata and "sql_query" in r.metadata:
+            sql_query = r.metadata["sql_query"]
+            print("##", sql_query)
+            with self.sql_database.engine.connect() as connection:
+                result = connection.execute(text(sql_query))
+                for item in result.fetchall():
+                    return_dict.append({k: v for k, v in zip(item._fields, item._t)})
+        return return_dict
+
+    def get_return_query(self, return_result: QueryReturn) -> str:
+        query_list = []
+        try:
+            source = return_result.sources[-1]
+            for raw_output in source.raw_output:
+                print("   ###########")
+                sm: StepModel = raw_output
+                query_list.append(sm.sentence)
+            return " ".join(query_list)
+        except:
+            raise
```

### Comparing `qai_agent-0.5.1/src/qai/agent/basic.py` & `qai_agent-0.5.2/src/qai/agent/basic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,18 @@
-import uuid
-from collections import defaultdict
-from dataclasses import dataclass, field
-from enum import StrEnum
-from typing import Any, List, Optional, Self, Sequence, Type, TypeVar
 
-from llama_index.agent.openai import OpenAIAgent
-from llama_index.core import Settings, SQLDatabase
-from llama_index.core.base.response.schema import Response
+from llama_index.core import Settings
 from llama_index.core.bridge.pydantic import BaseModel, Field
-from llama_index.core.llms.llm import LLM
-from llama_index.core.query_engine import NLSQLTableQueryEngine
 from llama_index.core.settings import Settings
-from llama_index.core.tools import BaseTool, FunctionTool, QueryEngineTool
+from llama_index.core.tools import FunctionTool
 from llama_index.core.tools.tool_spec.base import BaseToolSpec
 from llama_index.core.tools.types import ToolMetadata, ToolOutput
 from llama_index.llms.openai import OpenAI
-from llama_index.tools.database import DatabaseToolSpec
-from pi_conf import AttrDict, load_config
-from qai.ai import QueryReturn
-from sqlalchemy import MetaData, create_engine, text
-from sqlalchemy.exc import NoSuchTableError
-from sqlalchemy.schema import CreateTable
+from pi_conf import load_config
 
-from qai.agent.agents.find_agent import AgentType, FindAgentWorker
-from qai.agent.qaibot import QaiSession
-from qai.agent.sessions.qai_session import QaiSession
+from qai.agent.agents.find_agent import AgentType
 from qai.agent.tools.types import StringEnum
 
 Settings.llm = OpenAI(model="gpt-3.5-turbo", temperature=0.1)
 
 
 class QueryType(StringEnum):
     campaign = "campaign"
```

### Comparing `qai_agent-0.5.1/src/qai/agent/data/state_codes.py` & `qai_agent-0.5.2/src/qai/agent/data/state_codes.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.1/src/qai/agent/llama_index/llm_program.py` & `qai_agent-0.5.2/src/qai/agent/llama_index/llm_program.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-from llama_index.core.program import LLMTextCompletionProgram
-from typing import Any, Dict, Optional, Type, cast
+from typing import Any, Dict, Optional
 
+from llama_index.core.base.llms.types import ChatResponse
 from llama_index.core.bridge.pydantic import BaseModel
-from llama_index.core.llms.llm import LLM
-from llama_index.core.output_parsers.pydantic import PydanticOutputParser
-from llama_index.core.prompts.base import BasePromptTemplate, PromptTemplate
-from llama_index.core.settings import Settings
-from llama_index.core.types import BaseOutputParser, BasePydanticProgram
-from llama_index.core.base.llms.types import (
-    ChatMessage,
-    ChatResponse,
-)
+from llama_index.core.program import LLMTextCompletionProgram
+
+
 class StructuredResponse:
     model : BaseModel
     response : ChatResponse
 
 class StructuredLLM(LLMTextCompletionProgram):
 
     def __init__(self, *args, **kwargs):
```

### Comparing `qai_agent-0.5.1/src/qai/agent/serve.py` & `qai_agent-0.5.2/src/qai/agent/serve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from pprint import pformat
 
 from flask import jsonify, request
 from flask_pydantic import validate
 from pi_log import logs
-
 from qai.chat import VERSION, create_app
 from qai.chat.config import cfg
 from qai.chat.models import CompanyQueryModel
 
 app = create_app(cfg)  ## app should be created before importing other modules
```

### Comparing `qai_agent-0.5.1/src/qai/agent/tools.py` & `qai_agent-0.5.2/src/qai/agent/tools.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.1/src/qai/agent/utils/distribute.py` & `qai_agent-0.5.2/src/qai/agent/utils/distribute.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.1/src/qai/agent/utils/utils.py` & `qai_agent-0.5.2/src/qai/agent/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import re
 
 from qai.agent.data.state_codes import state_codes
 
 
 def refine_step_queries(steps: list[dict[str, str]]) -> list[dict[str, str]]:
     """
     Refine the step queries by replacing the technology names with the correct case from the database.
```

### Comparing `qai_agent-0.5.1/PKG-INFO` & `qai_agent-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qai-agent
-Version: 0.5.1
+Version: 0.5.2
 Summary: Qai Agents for the Qai AI Platform
 Author: parnell
 Author-email: 152523161+leeparnell@users.noreply.github.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: install (>=1.3.5,<2.0.0)
@@ -15,14 +15,15 @@
 Requires-Dist: llama-index-llms-openai (>=0.1.14,<0.2.0)
 Requires-Dist: llama-index-llms-replicate (>=0.1.3,<0.2.0)
 Requires-Dist: llama-index-program-openai (>=0.1.5)
 Requires-Dist: llama-index-tools-database (>=0.1.3,<0.2.0)
 Requires-Dist: llama-index-tools-google (>=0.1.3,<0.2.0)
 Requires-Dist: llama-index-vector-stores-mongodb (>=0.1.4,<0.2.0)
 Requires-Dist: multiprocess (>=0.70.16,<0.71.0)
+Requires-Dist: mysql-connector-python (>=8.4.0,<9.0.0)
 Requires-Dist: openai (>=1.23.2,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pi-conf (>=0.7.7.5,<0.8.0.0)
 Requires-Dist: pi-log (>=0.5.7.3,<0.6.0.0)
 Requires-Dist: pip (>=24.0,<25.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pymongo (>=4.6.3,<5.0.0)
```

