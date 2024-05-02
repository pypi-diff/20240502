# Comparing `tmp/k8sai-0.1.1.tar.gz` & `tmp/k8sai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8sai-0.1.1.tar", last modified: Thu May  2 00:18:10 2024, max compression
+gzip compressed data, was "k8sai-0.1.2.tar", last modified: Thu May  2 05:50:25 2024, max compression
```

## Comparing `k8sai-0.1.1.tar` & `k8sai-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 00:18:10.494043 k8sai-0.1.1/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)    34523 2024-05-01 19:17:58.000000 k8sai-0.1.1/LICENSE
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       45 2024-05-02 00:01:57.000000 k8sai-0.1.1/MANIFEST.in
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3706 2024-05-02 00:18:10.493780 k8sai-0.1.1/PKG-INFO
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3311 2024-05-02 00:16:00.000000 k8sai-0.1.1/README.md
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 00:18:10.479097 k8sai-0.1.1/k8sAI/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:29:38.000000 k8sai-0.1.1/k8sAI/__init__.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 00:18:10.480298 k8sai-0.1.1/k8sAI/kuberag/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-04-30 19:56:40.000000 k8sai-0.1.1/k8sAI/kuberag/__init__.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     2599 2024-05-02 00:01:57.000000 k8sai-0.1.1/k8sAI/kuberag/chat.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 00:18:10.480402 k8sai-0.1.1/k8sAI/kuberag/embeddings/
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 00:18:10.493336 k8sai-0.1.1/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)  6284000 2024-05-01 22:10:06.000000 k8sai-0.1.1/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/data_level0.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      100 2024-05-01 22:10:05.000000 k8sai-0.1.1/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/header.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     4000 2024-05-01 22:10:06.000000 k8sai-0.1.1/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/length.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:10:05.000000 k8sai-0.1.1/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/link_lists.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)  3272704 2024-04-30 23:46:31.000000 k8sai-0.1.1/k8sAI/kuberag/embeddings/chroma.sqlite3
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3139 2024-05-02 00:02:30.000000 k8sai-0.1.1/k8sAI/kuberag/main.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      746 2024-05-02 00:01:57.000000 k8sai-0.1.1/k8sAI/kuberag/retriever.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     2508 2024-05-02 00:01:57.000000 k8sai-0.1.1/k8sAI/kuberag/tool_handler.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     5663 2024-05-02 00:01:57.000000 k8sai-0.1.1/k8sAI/kuberag/tools.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     4144 2024-05-02 00:02:30.000000 k8sai-0.1.1/k8sAI/main.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       87 2024-05-01 22:29:29.000000 k8sai-0.1.1/k8sAI/util.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 00:18:10.493505 k8sai-0.1.1/k8sAI.egg-info/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3706 2024-05-02 00:18:10.000000 k8sai-0.1.1/k8sAI.egg-info/PKG-INFO
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      751 2024-05-02 00:18:10.000000 k8sai-0.1.1/k8sAI.egg-info/SOURCES.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        1 2024-05-02 00:18:10.000000 k8sai-0.1.1/k8sAI.egg-info/dependency_links.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       42 2024-05-02 00:18:10.000000 k8sai-0.1.1/k8sAI.egg-info/entry_points.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       65 2024-05-02 00:18:10.000000 k8sai-0.1.1/k8sAI.egg-info/requires.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        6 2024-05-02 00:18:10.000000 k8sai-0.1.1/k8sAI.egg-info/top_level.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       38 2024-05-02 00:18:10.494089 k8sai-0.1.1/setup.cfg
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      653 2024-05-02 00:02:56.000000 k8sai-0.1.1/setup.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.441635 k8sai-0.1.2/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)    34523 2024-05-01 19:17:58.000000 k8sai-0.1.2/LICENSE
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       45 2024-05-02 00:01:57.000000 k8sai-0.1.2/MANIFEST.in
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3706 2024-05-02 05:50:25.441377 k8sai-0.1.2/PKG-INFO
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3311 2024-05-02 00:16:00.000000 k8sai-0.1.2/README.md
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.426312 k8sai-0.1.2/k8sAI/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:29:38.000000 k8sai-0.1.2/k8sAI/__init__.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.428259 k8sai-0.1.2/k8sAI/kuberag/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-04-30 19:56:40.000000 k8sai-0.1.2/k8sAI/kuberag/__init__.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     2599 2024-05-02 00:01:57.000000 k8sai-0.1.2/k8sAI/kuberag/chat.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.428505 k8sai-0.1.2/k8sAI/kuberag/embeddings/
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.440862 k8sai-0.1.2/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)  6284000 2024-05-01 22:10:06.000000 k8sai-0.1.2/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/data_level0.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      100 2024-05-01 22:10:05.000000 k8sai-0.1.2/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/header.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     4000 2024-05-01 22:10:06.000000 k8sai-0.1.2/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/length.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:10:05.000000 k8sai-0.1.2/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/link_lists.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)  3272704 2024-04-30 23:46:31.000000 k8sai-0.1.2/k8sAI/kuberag/embeddings/chroma.sqlite3
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3415 2024-05-02 05:42:12.000000 k8sai-0.1.2/k8sAI/kuberag/main.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      746 2024-05-02 00:01:57.000000 k8sai-0.1.2/k8sAI/kuberag/retriever.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     1810 2024-05-02 05:42:12.000000 k8sai-0.1.2/k8sAI/kuberag/tool_handler.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     6276 2024-05-02 05:42:12.000000 k8sai-0.1.2/k8sAI/kuberag/tools.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     4144 2024-05-02 05:47:26.000000 k8sai-0.1.2/k8sAI/main.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       87 2024-05-01 22:29:29.000000 k8sai-0.1.2/k8sAI/util.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.441067 k8sai-0.1.2/k8sAI.egg-info/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3706 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/PKG-INFO
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      751 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/SOURCES.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        1 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/dependency_links.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       42 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/entry_points.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       65 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/requires.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        6 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/top_level.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       38 2024-05-02 05:50:25.441684 k8sai-0.1.2/setup.cfg
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      653 2024-05-02 05:42:12.000000 k8sai-0.1.2/setup.py
```

### Comparing `k8sai-0.1.1/LICENSE` & `k8sai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.1/PKG-INFO` & `k8sai-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8sAI
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple example package
 Home-page: https://github.com/wilson090/k8sAI
 Author: Wilson Spearman
 Author-email: wilsonspearman@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `k8sai-0.1.1/README.md` & `k8sai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.1/k8sAI/kuberag/chat.py` & `k8sai-0.1.2/k8sAI/kuberag/chat.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.1/k8sAI/kuberag/embeddings/chroma.sqlite3` & `k8sai-0.1.2/k8sAI/kuberag/embeddings/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.1/k8sAI/kuberag/main.py` & `k8sai-0.1.2/k8sAI/kuberag/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,23 +41,27 @@
         terminal=False,
     ):
         """
         Start a chat with the bot. User can end with 'exit'.
             Args:
                 logs (str): The logs to provide to the bot.
         """
+        additional_context = None
         while True:
             if prompt:
                 user_prompt = prompt
                 prompt = None
             else:
                 user_prompt = input("Prompt: ")
             if user_prompt.lower() == "exit":
                 break
             # result = self.bot.invoke()
+            if additional_context != None:
+                user_prompt = f"using this \n{additional_context} \nrespond to this: {user_prompt}"
+                additional_context = None
             for chunk in self.bot.stream(
                 {"input": user_prompt, "logs": logs, "command_output": command_output},
                 config={"configurable": {"session_id": "<foo>"}},
             ):
                 # Agent Action
                 if "actions" in chunk:
                     for action in chunk["actions"]:
@@ -66,24 +70,24 @@
                                 f":hammer: Calling Tool: `{action.tool}` with input `\
                                               {action.tool_input}`",
                                 pad=(0, 0, 0, 2),
                             )
                         )
                 # Observation
                 elif "steps" in chunk:
-                    pass
+                    continue
                 # Final result
                 elif "output" in chunk:
                     if registry.has_tool_handler(chunk["output"]):
-                        terminate = registry.use_handler(chunk["output"])
+                        additional_context, terminate = registry.use_handler(chunk["output"])
                         if terminate:
                             break
-
-                    console.print("k8sAI:")
-                    console.print(Markdown(chunk["output"]))
+                    else:
+                        console.print("k8sAI:")
+                        console.print(Markdown(chunk["output"]))
 
                 else:
                     raise ValueError()
                 console.print("---")
 
             if terminal:
                 break
```

### Comparing `k8sai-0.1.1/k8sAI/kuberag/retriever.py` & `k8sai-0.1.2/k8sAI/kuberag/retriever.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.1/k8sAI/kuberag/tool_handler.py` & `k8sai-0.1.2/k8sAI/kuberag/tool_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # file: k8sAI/kuberag/tool_handler.py
 
 import json
 import os
 from prompt_toolkit import prompt
 from k8sAI.util import console
+import subprocess
 
 
 class ToolHandlerRegistry:
     """
     A registry for tool handlers.
     """
 
@@ -41,46 +42,24 @@
         console.print("Error: No handler found for the input string.")
         return None
 
 
 # TODO: create proper tool handler objects with data parse fn, etc.
 
 
-def handle_kubectl_tool(input_string, prefix) -> bool:
+def handle_suggest_kubectl_tool(input_string, prefix) -> bool:
     """
     Handle the kubectl tool data.
 
     returns: True if the tool should terminate. False otherwise
     """
-    json_part = input_string[len(prefix) :]
-    json_part = json_part.strip("'")
+    cmd_and_output = input_string[len(prefix) :]
+    cmd_and_output = (cmd_and_output.strip("'")).split("||")
+    output, cmd = cmd_and_output[0], cmd_and_output[1]
+    
+    context = f"{cmd} was just run and it outputed {output}"
 
-    try:
-        data = json.loads(json_part)
-        if "notes" in data:
-            console.print("\n")
-            console.print(data["notes"])
-        if "query" in data:
-            cmd = prompt(
-                "Edit the cmd and press (enter) to run, \
-                          leave empty to return to GPT\n\n",
-                default=data["query"],
-            )
-            # Split the command into the command and its arguments for execvp
-            args = cmd.split()
-
-            # Check if any command is entered, then execute it
-            if args:
-                console.print("\n")
-                # Replace the current process with the new command
-                os.execvp(args[0], args)
-            else:
-                console.print("No command entered.")
-
-    except json.JSONDecodeError:
-        console.print("Error: The string is not valid JSON.", {json_part})
-
-    return True
+    return context, False
 
 
 registry = ToolHandlerRegistry()
-registry.register_tool("[Suggest_Kubectl_CMD_Tool]", handle_kubectl_tool)
+registry.register_tool("[Suggest_Kubectl_CMD_Tool]", handle_suggest_kubectl_tool)
```

### Comparing `k8sai-0.1.1/k8sAI/kuberag/tools.py` & `k8sai-0.1.2/k8sAI/kuberag/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     CallbackManagerForToolRun,
 )
 from langchain.tools.retriever import create_retriever_tool
 from langchain.pydantic_v1 import BaseModel, Field
 from langchain.tools import BaseTool
 from rich.padding import Padding
 from k8sAI.util import console
+from prompt_toolkit import prompt
+
 
 
 def retriever_tool(retriever):
     """
     Create the retriever tool.
     """
     return create_retriever_tool(
@@ -62,18 +64,36 @@
         self,
         notes: str,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         # return this as a jsonified string so that we can parse and return it in the frontend
         data_dict = {"notes": notes, "query": query}
+        if notes:
+            console.print("\n")
+            console.print(notes)
+        if query:
+            cmd = prompt(
+                "Edit the cmd and press (enter) to run, leave empty to return to GPT\n\n",
+                default=query,
+            )
+        args = cmd.split()
+
+        # Check if any command is entered, then execute it
+        if args:
+            console.print("\n")
+            try:
+                output = subprocess.check_output(cmd, shell=True).decode("utf-8")
+                console.print(output)
+            except Exception as e:
+                output = str(e)
+        else:
+            console.print("No command entered.")
 
-        # Convert the dictionary to a JSON string
-        jsonified = json.dumps(data_dict)
-        return f"[Suggest_Kubectl_CMD_Tool]{jsonified}"
+        return f"[Suggest_Kubectl_CMD_Tool]{output}||{cmd}"
 
     async def _arun(
         self,
         notes: str,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
```

### Comparing `k8sai-0.1.1/k8sAI/main.py` & `k8sai-0.1.2/k8sAI/main.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.1/k8sAI.egg-info/PKG-INFO` & `k8sai-0.1.2/k8sAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8sAI
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple example package
 Home-page: https://github.com/wilson090/k8sAI
 Author: Wilson Spearman
 Author-email: wilsonspearman@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `k8sai-0.1.1/k8sAI.egg-info/SOURCES.txt` & `k8sai-0.1.2/k8sAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.1/setup.py` & `k8sai-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="k8sAI",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     description="A simple example package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Wilson Spearman",
     author_email="wilsonspearman@gmail.com",
     url="https://github.com/wilson090/k8sAI",
```

