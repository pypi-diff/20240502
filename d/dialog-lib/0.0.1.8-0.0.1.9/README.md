# Comparing `tmp/dialog_lib-0.0.1.8.tar.gz` & `tmp/dialog_lib-0.0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog_lib-0.0.1.8.tar", max compression
+gzip compressed data, was "dialog_lib-0.0.1.9.tar", max compression
```

## Comparing `dialog_lib-0.0.1.8.tar` & `dialog_lib-0.0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       98 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/dialog_lib/agents/__init__.py
--rw-r--r--   0        0        0     3238 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/dialog_lib/agents/abstract.py
--rw-r--r--   0        0        0      117 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/dialog_lib/db/__init__.py
--rw-r--r--   0        0        0     2717 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/dialog_lib/db/memory.py
--rw-r--r--   0        0        0     1325 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/dialog_lib/db/models.py
--rw-r--r--   0        0        0      394 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/dialog_lib/db/utils.py
--rw-r--r--   0        0        0        0 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/dialog_lib/embeddings/__init__.py
--rw-r--r--   0        0        0     1471 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/dialog_lib/embeddings/generate.py
--rw-r--r--   0        0        0      148 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/dialog_lib/main.py
--rw-r--r--   0        0        0      629 2024-04-13 19:49:04.535054 dialog_lib-0.0.1.8/pyproject.toml
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 dialog_lib-0.0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       98 2024-04-12 00:39:12.358734 dialog_lib-0.0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 00:17:13.466371 dialog_lib-0.0.1.9/dialog_lib/agents/__init__.py
+-rw-r--r--   0        0        0     3439 2024-04-20 00:41:32.646898 dialog_lib-0.0.1.9/dialog_lib/agents/abstract.py
+-rw-r--r--   0        0        0      135 2024-04-20 00:41:32.595885 dialog_lib-0.0.1.9/dialog_lib/db/__init__.py
+-rw-r--r--   0        0        0     2910 2024-04-20 00:41:32.648234 dialog_lib-0.0.1.9/dialog_lib/db/memory.py
+-rw-r--r--   0        0        0     1344 2024-04-20 00:41:32.639578 dialog_lib-0.0.1.9/dialog_lib/db/models.py
+-rw-r--r--   0        0        0      408 2024-04-20 00:04:41.645026 dialog_lib-0.0.1.9/dialog_lib/db/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 00:27:53.398079 dialog_lib-0.0.1.9/dialog_lib/embeddings/__init__.py
+-rw-r--r--   0        0        0     1498 2024-04-20 00:41:32.645563 dialog_lib-0.0.1.9/dialog_lib/embeddings/generate.py
+-rw-r--r--   0        0        0      152 2024-04-20 00:41:32.625077 dialog_lib-0.0.1.9/dialog_lib/main.py
+-rw-r--r--   0        0        0      629 2024-04-20 00:41:40.026157 dialog_lib-0.0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 dialog_lib-0.0.1.9/PKG-INFO
```

### Comparing `dialog_lib-0.0.1.8/dialog_lib/agents/abstract.py` & `dialog_lib-0.0.1.9/dialog_lib/agents/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from langchain.chains.llm import LLMChain
 from langchain.memory.chat_memory import BaseChatMemory
 from langchain.prompts import ChatPromptTemplate
 
 
 class AbstractLLM:
-    def __init__(self, config, session_id=None, parent_session_id=None, dataset=None, llm_api_key=None, dbsession=None):
+    def __init__(
+        self,
+        config,
+        session_id=None,
+        parent_session_id=None,
+        dataset=None,
+        llm_api_key=None,
+        dbsession=None,
+    ):
         """
         :param config: Configuration dictionary
 
         The constructor of the AbstractLLM class allows users to pass
         a configuration dictionary to the LLM. This configuration dictionary
         can be used to configure the LLM temperature, prompt and other
         necessities.
@@ -17,15 +25,17 @@
             raise ValueError("Config must be a dictionary")
 
         self.config = config
         self.prompt = None
         self.session_id = None
         self.relevant_contents = None
         if session_id:
-            self.session_id = session_id if dataset is None else f"{dataset}_{session_id}"
+            self.session_id = (
+                session_id if dataset is None else f"{dataset}_{session_id}"
+            )
         self.dataset = dataset
         self.llm_api_key = self.config.get("llm_api_key", llm_api_key)
         self.parent_session_id = parent_session_id
         self.dbsession = dbsession
 
     def get_prompt(self, input) -> ChatPromptTemplate:
         """
@@ -76,15 +86,22 @@
     def process(self, input: str):
         """
         Function that encapsulates the pre-processing, processing and post-processing
         of the LLM.
         """
         processed_input = self.preprocess(input)
         self.generate_prompt(processed_input)
-        if len(self.relevant_contents) == 0 and \
-            self.config.get("prompt").get("fallback_not_found_relevant_contents"):
-            return {"text": self.config.get("prompt").get("fallback_not_found_relevant_contents")}
-        output = self.llm({
-            "user_message": processed_input,
-        })
+        if len(self.relevant_contents) == 0 and self.config.get("prompt").get(
+            "fallback_not_found_relevant_contents"
+        ):
+            return {
+                "text": self.config.get("prompt").get(
+                    "fallback_not_found_relevant_contents"
+                )
+            }
+        output = self.llm(
+            {
+                "user_message": processed_input,
+            }
+        )
         processed_output = self.postprocess(output)
         return processed_output
```

### Comparing `dialog_lib-0.0.1.8/dialog_lib/db/memory.py` & `dialog_lib-0.0.1.9/dialog_lib/db/memory.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,17 +5,25 @@
 
 
 class CustomPostgresChatMessageHistory(PostgresChatMessageHistory):
     """
     Custom chat message history for LLM
     """
 
-    def __init__(self, *args, parent_session_id=None, dbsession=None, **kwargs):
+    def __init__(
+        self,
+        *args,
+        parent_session_id=None,
+        dbsession=None,
+        chat_messages_model=ChatMessages,
+        **kwargs,
+    ):
         self.parent_session_id = parent_session_id
         self.dbsession = dbsession
+        self.chat_messages_model = chat_messages_model
         super().__init__(*args, **kwargs)
 
     def _create_table_if_not_exists(self) -> None:
         """
         create table if it does not exist
         add a new column for timestamp
         """
@@ -42,39 +50,47 @@
         )
         if self.parent_session_id:
             message.parent = self.parent_session_id
         self.dbsession.add(message)
         self.dbsession.commit()
 
 
-def generate_memory_instance(session_id, parent_session_id=None, dbsession=None, database_url=None):
+def generate_memory_instance(
+    session_id, parent_session_id=None, dbsession=None, database_url=None
+):
     """
     Generate a memory instance for a given session_id
     """
 
     return CustomPostgresChatMessageHistory(
         connection_string=database_url,
         session_id=session_id,
         parent_session_id=parent_session_id,
         table_name="chat_messages",
-        dbsession=dbsession
+        dbsession=dbsession,
     )
 
 
-def add_user_message_to_message_history(session_id, message, memory=None, dbsession=None, database_url=None):
+def add_user_message_to_message_history(
+    session_id, message, memory=None, dbsession=None, database_url=None
+):
     """
     Add a user message to the message history and returns the updated
     memory instance
     """
     if not memory:
-        memory = generate_memory_instance(session_id, dbsession=dbsession, database_url=database_url)
+        memory = generate_memory_instance(
+            session_id, dbsession=dbsession, database_url=database_url
+        )
 
     memory.add_user_message(message)
     return memory
 
 
 def get_messages(session_id, dbsession=None, database_url=None):
     """
     Get all messages for a given session_id
     """
-    memory = generate_memory_instance(session_id, dbsession=dbsession, database_url=database_url)
+    memory = generate_memory_instance(
+        session_id, dbsession=dbsession, database_url=database_url
+    )
     return memory.messages
```

### Comparing `dialog_lib-0.0.1.8/dialog_lib/db/models.py` & `dialog_lib-0.0.1.9/dialog_lib/db/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import uuid
 
 from sqlalchemy import Table, MetaData
-from sqlalchemy import (
-    Column, Integer, DateTime, String, text, Text
-)
+from sqlalchemy import Column, Integer, DateTime, String, text, Text
 from sqlalchemy.orm import DeclarativeBase
 from sqlalchemy.dialects.postgresql import UUID, JSONB
 
 from pgvector.sqlalchemy import Vector
 
 
 class Base(DeclarativeBase):
@@ -17,29 +15,32 @@
 class ChatMessages(Base):
     __tablename__ = "chat_messages"
 
     id = Column(Integer, nullable=False, primary_key=True, autoincrement=True)
     parent = Column(Integer, nullable=True)
     session_id = Column(String, nullable=False)
     message = Column(JSONB, nullable=False)
-    timestamp = Column(DateTime, nullable=False, server_default=text("CURRENT_TIMESTAMP"))
+    timestamp = Column(
+        DateTime, nullable=False, server_default=text("CURRENT_TIMESTAMP")
+    )
 
 
 class Chat(Base):
     __tablename__ = "chats"
 
-    session_id = Column(String, nullable=False, default=str(uuid.uuid4()), primary_key=True)
+    session_id = Column(
+        String, nullable=False, default=str(uuid.uuid4()), primary_key=True
+    )
     tags = Column(String, nullable=True)
 
+
 class CompanyContent(Base):
     __tablename__ = "contents"
 
     id = Column(Integer, nullable=False, primary_key=True, autoincrement=True)
     category = Column(String, nullable=False)
     subcategory = Column(String, nullable=False)
     question = Column(String, nullable=False)
     content = Column(Text, nullable=False)
     embedding = Column(Vector(1536), nullable=False)
     dataset = Column(String, nullable=True)
     link = Column(String, nullable=True)
-
-
```

### Comparing `dialog_lib-0.0.1.8/dialog_lib/embeddings/generate.py` & `dialog_lib-0.0.1.9/dialog_lib/embeddings/generate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import List
 
 from sqlalchemy import select
 from langchain_core.embeddings import Embeddings
 from dialog_lib.db.models import CompanyContent
 
 
-def generate_embeddings(documents: List[str], embedding_llm_instance : Embeddings = None):
+def generate_embeddings(
+    documents: List[str], embedding_llm_instance: Embeddings = None
+):
     """
     Generate embeddings for a list of documents
     """
     return embedding_llm_instance.embed_documents(documents)
 
 
 def generate_embedding(document: str, embedding_llm_instance: Embeddings = None):
@@ -20,29 +22,32 @@
     :param embedding_llm_instance: - The Embedding LLM instance to use for generating embeddings
 
     """
     return embedding_llm_instance.embed_query(document)
 
 
 def get_most_relevant_contents_from_message(
-        message,
-        top=5,
-        dataset=None,
-        session=None,
-        embeddings_llm=None,
-        cosine_similarity_threshold=0.5
-    ):
+    message,
+    top=5,
+    dataset=None,
+    session=None,
+    embeddings_llm=None,
+    cosine_similarity_threshold=0.5,
+    model=CompanyContent,
+    embedding_column="embedding",
+):
     message_embedding = generate_embedding(message, embeddings_llm)
     filters = [
-        CompanyContent.embedding.cosine_distance(message_embedding) < cosine_similarity_threshold,
+        model.embedding.cosine_distance(message_embedding)
+        < cosine_similarity_threshold,
     ]
 
     if dataset is not None:
-        filters.append(CompanyContent.dataset == dataset)
+        filters.append(model.dataset == dataset)
 
     possible_contents = session.scalars(
-        select(CompanyContent)
+        select(model)
         .filter(*filters)
-        .order_by(CompanyContent.embedding.cosine_distance(message_embedding))
+        .order_by(getattr(model, embedding_column).cosine_distance(message_embedding))
         .limit(top)
     ).all()
     return possible_contents
```

### Comparing `dialog_lib-0.0.1.8/pyproject.toml` & `dialog_lib-0.0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialog-lib"
-version = "0.0.1.8"
+version = "0.0.1.9"
 description = ""
 authors = ["Talkd.AI <foss@talkd.ai>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dialog_lib-0.0.1.8/PKG-INFO` & `dialog_lib-0.0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-lib
-Version: 0.0.1.8
+Version: 0.0.1.9
 Summary: 
 License: MIT
 Author: Talkd.AI
 Author-email: foss@talkd.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

