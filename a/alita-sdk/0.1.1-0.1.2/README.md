# Comparing `tmp/alita_sdk-0.1.1.tar.gz` & `tmp/alita_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_sdk-0.1.1.tar", last modified: Tue Apr 30 17:56:01 2024, max compression
+gzip compressed data, was "alita_sdk-0.1.2.tar", last modified: Wed May  1 13:49:59 2024, max compression
```

## Comparing `alita_sdk-0.1.1.tar` & `alita_sdk-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.313858 alita_sdk-0.1.1/
--rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.1/LICENSE
--rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-04-30 17:56:01.313598 alita_sdk-0.1.1/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.1/README.md
--rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-04-30 17:55:53.000000 alita_sdk-0.1.1/pyproject.toml
--rw-r--r--   0 arozumenko   (501) staff       (20)      175 2024-04-30 17:55:06.000000 alita_sdk-0.1.1/requirements.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-04-30 17:56:01.313909 alita_sdk-0.1.1/setup.cfg
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.280529 alita_sdk-0.1.1/src/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.1/src/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.280633 alita_sdk-0.1.1/src/alita_sdk/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.1/src/alita_sdk/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.282655 alita_sdk-0.1.1/src/alita_sdk/agents/
--rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.1/src/alita_sdk/agents/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3122 2024-04-30 17:52:10.000000 alita_sdk-0.1.1/src/alita_sdk/agents/alita_openai.py
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-10 11:28:03.000000 alita_sdk-0.1.1/src/alita_sdk/agents/base_actions.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3095 2024-04-30 17:52:10.000000 alita_sdk-0.1.1/src/alita_sdk/agents/mixedAgentParser.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2283 2024-03-18 10:31:02.000000 alita_sdk-0.1.1/src/alita_sdk/agents/mixedAgentRenderes.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1169 2024-04-30 17:52:10.000000 alita_sdk-0.1.1/src/alita_sdk/agents/utils.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.285219 alita_sdk-0.1.1/src/alita_sdk/clients/
--rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.1/src/alita_sdk/clients/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    17899 2024-04-30 17:52:10.000000 alita_sdk-0.1.1/src/alita_sdk/clients/client.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.291137 alita_sdk-0.1.1/src/alita_sdk/llms/
--rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.1/src/alita_sdk/llms/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     8383 2024-04-30 17:52:10.000000 alita_sdk-0.1.1/src/alita_sdk/llms/alita.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.291669 alita_sdk-0.1.1/src/alita_sdk/toolkits/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.1/src/alita_sdk/toolkits/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.1/src/alita_sdk/toolkits/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.1/src/alita_sdk/toolkits/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.294979 alita_sdk-0.1.1/src/alita_sdk/tools/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.1/src/alita_sdk/tools/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.1/src/alita_sdk/tools/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-04-12 14:28:45.000000 alita_sdk-0.1.1/src/alita_sdk/tools/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.299229 alita_sdk-0.1.1/src/alita_sdk/utils/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.1/src/alita_sdk/utils/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.1/src/alita_sdk/utils/streamlit.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.313208 alita_sdk-0.1.1/src/alita_sdk.egg-info/
--rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-04-30 17:56:01.000000 alita_sdk-0.1.1/src/alita_sdk.egg-info/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)      887 2024-04-30 17:56:01.000000 alita_sdk-0.1.1/src/alita_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-04-30 17:56:01.000000 alita_sdk-0.1.1/src/alita_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)      176 2024-04-30 17:56:01.000000 alita_sdk-0.1.1/src/alita_sdk.egg-info/requires.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-04-30 17:56:01.000000 alita_sdk-0.1.1/src/alita_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-01 13:49:59.985814 alita_sdk-0.1.2/
+-rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.2/LICENSE
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-01 13:49:59.985591 alita_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.2/README.md
+-rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-05-01 13:49:10.000000 alita_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0 arozumenko   (501) staff       (20)      175 2024-04-30 17:55:06.000000 alita_sdk-0.1.2/requirements.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-05-01 13:49:59.985857 alita_sdk-0.1.2/setup.cfg
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-01 13:49:59.979189 alita_sdk-0.1.2/src/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.2/src/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-01 13:49:59.979299 alita_sdk-0.1.2/src/alita_sdk/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.2/src/alita_sdk/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-01 13:49:59.981362 alita_sdk-0.1.2/src/alita_sdk/agents/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.2/src/alita_sdk/agents/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3122 2024-04-30 17:52:10.000000 alita_sdk-0.1.2/src/alita_sdk/agents/alita_openai.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-10 11:28:03.000000 alita_sdk-0.1.2/src/alita_sdk/agents/base_actions.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3095 2024-04-30 17:52:10.000000 alita_sdk-0.1.2/src/alita_sdk/agents/mixedAgentParser.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2283 2024-03-18 10:31:02.000000 alita_sdk-0.1.2/src/alita_sdk/agents/mixedAgentRenderes.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1169 2024-04-30 17:52:10.000000 alita_sdk-0.1.2/src/alita_sdk/agents/utils.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-01 13:49:59.981963 alita_sdk-0.1.2/src/alita_sdk/clients/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.2/src/alita_sdk/clients/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    20661 2024-05-01 13:48:52.000000 alita_sdk-0.1.2/src/alita_sdk/clients/client.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-01 13:49:59.982732 alita_sdk-0.1.2/src/alita_sdk/llms/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.2/src/alita_sdk/llms/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     8383 2024-04-30 17:52:10.000000 alita_sdk-0.1.2/src/alita_sdk/llms/alita.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-01 13:49:59.983504 alita_sdk-0.1.2/src/alita_sdk/toolkits/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.2/src/alita_sdk/toolkits/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.2/src/alita_sdk/toolkits/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.2/src/alita_sdk/toolkits/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-01 13:49:59.984291 alita_sdk-0.1.2/src/alita_sdk/tools/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.2/src/alita_sdk/tools/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.2/src/alita_sdk/tools/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-04-12 14:28:45.000000 alita_sdk-0.1.2/src/alita_sdk/tools/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-01 13:49:59.984650 alita_sdk-0.1.2/src/alita_sdk/utils/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.2/src/alita_sdk/utils/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.2/src/alita_sdk/utils/streamlit.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-01 13:49:59.985310 alita_sdk-0.1.2/src/alita_sdk.egg-info/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-01 13:49:59.000000 alita_sdk-0.1.2/src/alita_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)      887 2024-05-01 13:49:59.000000 alita_sdk-0.1.2/src/alita_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-05-01 13:49:59.000000 alita_sdk-0.1.2/src/alita_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)      176 2024-05-01 13:49:59.000000 alita_sdk-0.1.2/src/alita_sdk.egg-info/requires.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-05-01 13:49:59.000000 alita_sdk-0.1.2/src/alita_sdk.egg-info/top_level.txt
```

### Comparing `alita_sdk-0.1.1/LICENSE` & `alita_sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/PKG-INFO` & `alita_sdk-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_sdk-0.1.1/README.md` & `alita_sdk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/pyproject.toml` & `alita_sdk-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_sdk"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Artem Rozumenko", email="support@analysta.ai" },
 ]
 description = "SDK for building langchain agents using resouces from Alita"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `alita_sdk-0.1.1/src/alita_sdk/agents/__init__.py` & `alita_sdk-0.1.2/src/alita_sdk/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/src/alita_sdk/agents/alita_openai.py` & `alita_sdk-0.1.2/src/alita_sdk/agents/alita_openai.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/src/alita_sdk/agents/mixedAgentParser.py` & `alita_sdk-0.1.2/src/alita_sdk/agents/mixedAgentParser.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/src/alita_sdk/agents/mixedAgentRenderes.py` & `alita_sdk-0.1.2/src/alita_sdk/agents/mixedAgentRenderes.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/src/alita_sdk/agents/utils.py` & `alita_sdk-0.1.2/src/alita_sdk/agents/utils.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/src/alita_sdk/clients/client.py` & `alita_sdk-0.1.2/src/alita_sdk/clients/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import requests
+from importlib import import_module
 from typing import Dict, List, Any, Optional
 from jinja2 import Environment, DebugUndefined, meta
 from langchain_core.pydantic_v1 import BaseModel, Field
 
 from langchain_core.messages import (
     AIMessage,
     HumanMessage,
@@ -15,15 +16,18 @@
 from langchain.agents import AgentExecutor
 from langchain_core.utils.function_calling import convert_to_openai_function
 
 from ..agents import create_mixed_agent
 from ..agents.alita_openai import AlitaAssistantRunnable
 from ..toolkits.prompt import PromptToolkit
 from ..toolkits.datasource import DatasourcesToolkit
+from alita_tools.github import AlitaGitHubToolkit
 from alita_tools.openapi import AlitaOpenAPIToolkit
+from alita_tools.jira import JiraToolkit
+from alita_tools.confluence import ConfluenceToolkit
 from pydantic import create_model
 
 logger = logging.getLogger(__name__)
 
 
 class Jinja2TemplatedChatMessagesTemplate(ChatPromptTemplate):
 
@@ -249,14 +253,56 @@
                             headers[
                                 tool["settings"]["authentication"]["settings"]["custom_header_name"]] = f'{auth_key}'
                 tools.extend(AlitaOpenAPIToolkit.get_toolkit(
                     openapi_spec=tool['settings']['schema_settings'],
                     selected_tools=tool['settings'].get('selected_tools', []),
                     headers={}
                 ).get_tools())
+            elif tool['type'] == 'github':
+                github_toolkit = AlitaGitHubToolkit().get_toolkit(
+                    selected_tools=tool['settings'].get('selected_tools', []),
+                    github_repository=tool['settings']['repository'],
+                    active_branch=tool['settings']['active_branch'],
+                    github_base_branch=tool['settings']['base_branch'],
+                    github_access_token=tool['settings'].get('access_token', None),
+                )
+                tools.extend(github_toolkit.get_tools())
+            elif tool['type'] == 'jira':
+                jira_tools = JiraToolkit().get_toolkit(
+                    selected_tools=tool['settings'].get('selected_tools', []),
+                    base_url=tool['settings']['base_url'], 
+                    cloud=tool['settings'].get('cloud', True),
+                    api_key=tool['settings'].get('api_key', None),
+                    username=tool['settings'].get('username', None),
+                    token=tool['settings'].get('token', None),
+                    limit=tool['settings'].get('limit', 5),
+                    additional_fields=tool['settings'].get('additional_fields', []),
+                    verify_ssl=tool['settings'].get('verify_ssl', True))
+                tools.extend(jira_tools.get_tools())
+            elif tool['type'] == 'confluence':
+                confluence_tools = ConfluenceToolkit().get_toolkit(
+                    selected_tools=tool['settings'].get('selected_tools', []),
+                    base_url=tool['settings']['base_url'],
+                    cloud=tool['settings'].get('cloud', True),
+                    api_key=tool['settings'].get('api_key', None),
+                    username=tool['settings'].get('username', None),
+                    token=tool['settings'].get('token', None),
+                    limit=tool['settings'].get('limit', 5),
+                    additional_fields=tool['settings'].get('additional_fields', []),
+                    verify_ssl=tool['settings'].get('verify_ssl', True))
+                tools.extend(confluence_tools.get_tools())
+            else:
+                if tool.get("module"):
+                    try:
+                        mod = import_module(tool.get("module"))
+                        tkitclass = getattr(mod, tool.get("class"))
+                        toolkit = tkitclass.get_toolkit(**tool["settings"])
+                        tools.extend(toolkit.get_tools())
+                    except Exception as e:
+                        logger.error(f"Error in getting toolkit: {e}")
         if len(prompts) > 0:
             tools += PromptToolkit.get_toolkit(self, prompts).get_tools()
         if prompt_type == 'openai':
             open_ai_funcs = [convert_to_openai_function(t) for t in tools]
             return Assistant(client, template, tools, open_ai_funcs).getOpenAIAgentExecutor()
         else:
             return Assistant(client, template, tools).getAgentExecutor()
```

### Comparing `alita_sdk-0.1.1/src/alita_sdk/llms/alita.py` & `alita_sdk-0.1.2/src/alita_sdk/llms/alita.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/src/alita_sdk/toolkits/datasource.py` & `alita_sdk-0.1.2/src/alita_sdk/toolkits/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/src/alita_sdk/toolkits/prompt.py` & `alita_sdk-0.1.2/src/alita_sdk/toolkits/prompt.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/src/alita_sdk/tools/datasource.py` & `alita_sdk-0.1.2/src/alita_sdk/tools/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/src/alita_sdk/utils/streamlit.py` & `alita_sdk-0.1.2/src/alita_sdk/utils/streamlit.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.1/src/alita_sdk.egg-info/PKG-INFO` & `alita_sdk-0.1.2/src/alita_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_sdk-0.1.1/src/alita_sdk.egg-info/SOURCES.txt` & `alita_sdk-0.1.2/src/alita_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

