# Comparing `tmp/aiproxy_python-0.3.6-py3-none-any.whl.zip` & `tmp/aiproxy_python-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,18 @@
-Zip file size: 23260 bytes, number of entries: 13
+Zip file size: 28779 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      243 b- defN 23-Dec-07 17:22 aiproxy/__init__.py
 -rw-r--r--  2.0 unx     1539 b- defN 23-Dec-08 14:24 aiproxy/__main__.py
--rw-r--r--  2.0 unx     9086 b- defN 24-Feb-03 03:32 aiproxy/accesslog.py
+-rw-r--r--  2.0 unx     7728 b- defN 24-May-01 13:52 aiproxy/accesslog.py
+-rw-r--r--  2.0 unx     7296 b- defN 24-May-01 14:02 aiproxy/anthropic_claude.py
 -rw-r--r--  2.0 unx     1337 b- defN 23-Dec-08 14:24 aiproxy/azurequeueclient.py
--rw-r--r--  2.0 unx    21900 b- defN 24-Jan-29 23:45 aiproxy/chatgpt.py
+-rw-r--r--  2.0 unx    11119 b- defN 24-May-01 13:52 aiproxy/chatgpt.py
 -rw-r--r--  2.0 unx    16284 b- defN 23-Dec-11 15:51 aiproxy/claude2.py
--rw-r--r--  2.0 unx     2165 b- defN 23-Dec-18 13:12 aiproxy/proxy.py
--rw-r--r--  2.0 unx     1143 b- defN 23-Dec-09 15:03 aiproxy/queueclient.py
--rw-r--r--  2.0 unx    11324 b- defN 24-Feb-03 03:33 aiproxy_python-0.3.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    13405 b- defN 24-Feb-03 03:33 aiproxy_python-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-03 03:33 aiproxy_python-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Feb-03 03:33 aiproxy_python-0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1038 b- defN 24-Feb-03 03:33 aiproxy_python-0.3.6.dist-info/RECORD
-13 files, 79564 bytes uncompressed, 21544 bytes compressed:  72.9%
+-rw-r--r--  2.0 unx    10891 b- defN 24-May-01 14:15 aiproxy/gemini.py
+-rw-r--r--  2.0 unx    15793 b- defN 24-May-01 13:52 aiproxy/httpx_proxy.py
+-rw-r--r--  2.0 unx     2165 b- defN 24-Apr-02 01:14 aiproxy/proxy.py
+-rw-r--r--  2.0 unx      731 b- defN 24-May-01 13:52 aiproxy/queueclient.py
+-rw-r--r--  2.0 unx    11324 b- defN 24-May-01 14:16 aiproxy_python-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13405 b- defN 24-May-01 14:16 aiproxy_python-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-01 14:16 aiproxy_python-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-01 14:16 aiproxy_python-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1276 b- defN 24-May-01 14:16 aiproxy_python-0.4.0.dist-info/RECORD
+16 files, 101231 bytes uncompressed, 26703 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,38 +3,47 @@
 
 Filename: aiproxy/__main__.py
 Comment: 
 
 Filename: aiproxy/accesslog.py
 Comment: 
 
+Filename: aiproxy/anthropic_claude.py
+Comment: 
+
 Filename: aiproxy/azurequeueclient.py
 Comment: 
 
 Filename: aiproxy/chatgpt.py
 Comment: 
 
 Filename: aiproxy/claude2.py
 Comment: 
 
+Filename: aiproxy/gemini.py
+Comment: 
+
+Filename: aiproxy/httpx_proxy.py
+Comment: 
+
 Filename: aiproxy/proxy.py
 Comment: 
 
 Filename: aiproxy/queueclient.py
 Comment: 
 
-Filename: aiproxy_python-0.3.6.dist-info/LICENSE
+Filename: aiproxy_python-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: aiproxy_python-0.3.6.dist-info/METADATA
+Filename: aiproxy_python-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: aiproxy_python-0.3.6.dist-info/WHEEL
+Filename: aiproxy_python-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: aiproxy_python-0.3.6.dist-info/top_level.txt
+Filename: aiproxy_python-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aiproxy_python-0.3.6.dist-info/RECORD
+Filename: aiproxy_python-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiproxy/accesslog.py

```diff
@@ -106,25 +106,24 @@
 
     @abstractmethod
     def to_accesslog(self, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
         ...
 
 
 class StreamChunkItemBase(QueueItemBase):
-    def __init__(self, request_id: str, chunk_json: dict = None, response_headers: dict = None, duration: float = 0, duration_api: float = 0, request_json: dict = None, status_code: int = 0) -> None:
+    def __init__(self, request_id: str, response_content: str = None, response_headers: dict = None, duration: float = 0, duration_api: float = 0, status_code: int = 0) -> None:
         self.request_id = request_id
-        self.chunk_json = chunk_json
+        self.response_content = response_content
         self.response_headers = response_headers
         self.duration = duration
         self.duration_api = duration_api
-        self.request_json = request_json
         self.status_code = status_code
 
     @abstractmethod
-    def to_accesslog(self, chunks: list, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
+    def to_accesslog(self, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
         ...
 
 
 class ErrorItemBase(QueueItemBase):
     def __init__(self, request_id: str, exception: Exception, traceback_info: str, response_json: dict = None, response_headers: dict = None, status_code: int = 0) -> None:
         self.request_id = request_id
         self.exception = exception
@@ -180,61 +179,29 @@
             self.db_engine = db_engine
         else:
             self.db_engine = create_engine(connection_str)
         self.accesslog_cls = accesslog_cls
         self.accesslog_cls.metadata.create_all(bind=self.db_engine)
         self.get_session = sessionmaker(autocommit=False, autoflush=False, bind=self.db_engine)
         self.queue_client = queue_client or DefaultQueueClient()
-        self.chunk_buffer = {}
 
     def insert_request(self, accesslog: _AccessLogBase, db: Session):
         db.add(accesslog)
         db.commit()
 
     def insert_response(self, accesslog: _AccessLogBase, db: Session):
         db.add(accesslog)
         db.commit()
 
-    def use_db(self, item: QueueItemBase):
-        return not (isinstance(item, StreamChunkItemBase) and item.duration == 0)
-
     def process_item(self, item: QueueItemBase, db: Session):
         try:
-            # Request
-            if isinstance(item, RequestItemBase):
-                self.insert_request(item.to_accesslog(self.accesslog_cls), db)
-
-            # Non-stream response
-            elif isinstance(item, ResponseItemBase):
-                self.insert_response(item.to_accesslog(self.accesslog_cls), db)
-
-            # Stream response
-            elif isinstance(item, StreamChunkItemBase):
-                if not self.chunk_buffer.get(item.request_id):
-                    self.chunk_buffer[item.request_id] = []
-
-                if item.duration == 0:
-                    self.chunk_buffer[item.request_id].append(item)
-
-                else:
-                    # Last chunk data for specific request_id
-                    self.insert_response(item.to_accesslog(
-                        self.chunk_buffer[item.request_id], self.accesslog_cls
-                    ), db)
-                    # Remove chunks from buffer
-                    del self.chunk_buffer[item.request_id]
-
-            # Error response
-            elif isinstance(item, ErrorItemBase):
-                self.insert_response(item.to_accesslog(self.accesslog_cls), db)
-
+            self.insert_response(item.to_accesslog(self.accesslog_cls), db)
         except Exception as ex:
             logger.error(f"Error at processing queue item: {ex}\n{traceback.format_exc()}")
 
-
     def run(self):
         while True:
             sleep(self.queue_client.dequeue_interval)
             db = None
             try:
                 items = self.queue_client.get()
             except Exception as ex:
@@ -242,16 +209,16 @@
                 continue
 
             for item in items:
                 try:
                     if isinstance(item, WorkerShutdownItem) or item is None:
                         return
 
-                    if db is None and self.use_db(item):
-                        # Get db session just once in the loop when the item that uses db found
+                    if db is None:
+                        # Get db session just once in the loop
                         db = self.get_session()
 
                     self.process_item(item, db)
 
                 except Exception as pex:
                     logger.error(f"Error at processing loop: {pex}\n{traceback.format_exc()}")
                     # Try to persist data in error log instead
```

## aiproxy/chatgpt.py

```diff
@@ -1,30 +1,22 @@
 from datetime import datetime
 import json
 import logging
-import os
-import time
-import traceback
-from typing import List, Union, AsyncGenerator
-from uuid import uuid4
-from fastapi import FastAPI, Request
-from fastapi.responses import JSONResponse
-from sse_starlette.sse import EventSourceResponse, AsyncContentStream
-from openai import AsyncClient, APIStatusError, APIResponseValidationError, APIError, OpenAIError
-from openai.types.chat import ChatCompletion
+from typing import List
 import tiktoken
-from .proxy import ProxyBase, RequestFilterBase, ResponseFilterBase, RequestFilterException, ResponseFilterException
-from .accesslog import _AccessLogBase, RequestItemBase, ResponseItemBase, StreamChunkItemBase, ErrorItemBase
+from fastapi import Request
+from .proxy import RequestFilterBase, ResponseFilterBase
+from .httpx_proxy import HTTPXProxy, SessionInfo, SessionRequestItemBase, SessionResponseItemBase, SessionStreamChunkItemBase, SessionErrorItemBase
+from .accesslog import _AccessLogBase
 from .queueclient import QueueClientBase
 
-
 logger = logging.getLogger(__name__)
 
 
-class ChatGPTRequestItem(RequestItemBase):
+class ChatGPTRequestItem(SessionRequestItemBase):
     def to_accesslog(self, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
         request_headers_copy = self.request_headers.copy()
         if auth := request_headers_copy.get("authorization"):
             request_headers_copy["authorization"] = auth[:12] + "*****" + auth[-2:]
 
         content = self.request_json["messages"][-1]["content"]
         if isinstance(content, list):
@@ -44,15 +36,15 @@
             raw_headers=json.dumps(request_headers_copy, ensure_ascii=False),
             model=self.request_json.get("model")
         )
 
         return accesslog
 
 
-class ChatGPTResponseItem(ResponseItemBase):
+class ChatGPTResponseItem(SessionResponseItemBase):
     def to_accesslog(self, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
         content=self.response_json["choices"][0]["message"].get("content")
         function_call=self.response_json["choices"][0]["message"].get("function_call")
         tool_calls=self.response_json["choices"][0]["message"].get("tool_calls")
         response_headers = json.dumps(dict(self.response_headers.items()), ensure_ascii=False) if self.response_headers is not None else None
         model=self.response_json["model"]
         prompt_tokens=self.response_json["usage"]["prompt_tokens"]
@@ -119,32 +111,42 @@
     if tool_choice := request_json.get("tool_choice"):
         token_count += count_token(json.dumps(tool_choice))
 
     token_count += 3
     return token_count
 
 
-class ChatGPTStreamResponseItem(StreamChunkItemBase):
-    def to_accesslog(self, chunks: list, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
-        chunk_jsons = []
-        response_content = ""
+class ChatGPTStreamResponseItem(SessionStreamChunkItemBase):
+    def to_accesslog(self, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
+        response_text = ""
+        model = ""
         function_call = None
         tool_calls = None
         prompt_tokens = 0
         completion_tokens = 0
 
         # Parse info from chunks
+        chunks = self.response_content.split("\n\n")
         for chunk in chunks:
-            chunk_jsons.append(chunk.chunk_json)
+            chunk_strip = chunk.strip()
+            if not chunk_strip.startswith("data:"):
+                continue    # Skip invalid data
+            if chunk_strip.endswith("[DONE]"):
+                break       # Break when [DONE]
+
+            chunk_json = json.loads(chunk_strip[5:])
 
-            if len(chunk.chunk_json["choices"]) == 0:
+            if len(chunk_json["choices"]) == 0:
                 # Azure returns the first delta with empty choices
                 continue
+            
+            if not model and "model" in chunk_json:
+                model = chunk_json.get("model")
 
-            delta = chunk.chunk_json["choices"][0]["delta"]
+            delta = chunk_json["choices"][0]["delta"]
 
             # Make tool_calls
             if delta.get("tool_calls"):
                 if tool_calls is None:
                     tool_calls = []
                 if delta["tool_calls"][0]["function"].get("name"):
                     tool_calls.append({
@@ -165,351 +167,125 @@
                     function_call["name"] = delta["function_call"]["name"]
                     function_call["arguments"] = ""
                 elif delta["function_call"].get("arguments"):
                     function_call["arguments"] += delta["function_call"]["arguments"]
 
             # Text content
             else:
-                response_content += delta.get("content") or ""
+                response_text += delta.get("content") or ""
         
         # Serialize
         function_call_str = json.dumps(function_call, ensure_ascii=False) if function_call is not None else None
         tool_calls_str = json.dumps(tool_calls, ensure_ascii=False) if tool_calls is not None else None
         response_headers = json.dumps(dict(self.response_headers.items()), ensure_ascii=False) if self.response_headers is not None else None
 
         # Count tokens
-        prompt_tokens = count_request_token(self.request_json)
+        prompt_tokens = count_request_token(self.session.request_json)
 
         if tool_calls_str:
             completion_tokens = count_token(tool_calls_str)
         elif function_call_str:
             completion_tokens = count_token(function_call_str)
         else:
-            completion_tokens = count_token(response_content)
+            completion_tokens = count_token(response_text)
 
         return accesslog_cls(
             request_id=self.request_id,
             created_at=datetime.utcnow(),
             direction="response",
             status_code=self.status_code,
-            content=response_content,
+            content=response_text,
             function_call=function_call_str,
             tool_calls=tool_calls_str,
-            raw_body=json.dumps(chunk_jsons, ensure_ascii=False),
+            raw_body=self.response_content,
             raw_headers=response_headers,
-            model=chunk_jsons[0]["model"],
+            model=model,
             prompt_tokens=prompt_tokens,
             completion_tokens=completion_tokens,
             request_time=self.duration,
             request_time_api=self.duration_api
         )
 
 
-class ChatGPTErrorItem(ErrorItemBase):
+class ChatGPTErrorItem(SessionErrorItemBase):
     ...
 
 
 queue_item_types = [ChatGPTRequestItem, ChatGPTResponseItem, ChatGPTStreamResponseItem, ChatGPTErrorItem]
 
 
-# Reverse proxy application for ChatGPT
-class ChatGPTProxy(ProxyBase):
-    _empty_openai_api_key = "OPENAI_API_KEY_IS_NOT_SET"
-
+# Reverse proxy application for OpenAI ChatGPT API
+class ChatGPTProxy(HTTPXProxy):
     def __init__(
         self,
         *,
         api_key: str = None,
-        async_client: AsyncClient = None,
-        max_retries: int = 0,
-        timeout: float = 60.0,
+        timeout=60.0,
         request_filters: List[RequestFilterBase] = None,
         response_filters: List[ResponseFilterBase] = None,
         request_item_class: type = ChatGPTRequestItem,
         response_item_class: type = ChatGPTResponseItem,
         stream_response_item_class: type = ChatGPTStreamResponseItem,
         error_item_class: type = ChatGPTErrorItem,
-        access_logger_queue: QueueClientBase,
+        access_logger_queue: QueueClientBase
     ):
         super().__init__(
+            timeout=timeout,
             request_filters=request_filters,
             response_filters=response_filters,
+            request_item_class=request_item_class,
+            response_item_class=response_item_class,
+            stream_response_item_class=stream_response_item_class,
+            error_item_class=error_item_class,
             access_logger_queue=access_logger_queue
         )
 
-        # Log items
-        self.request_item_class = request_item_class
-        self.response_item_class = response_item_class
-        self.stream_response_item_class = stream_response_item_class
-        self.error_item_class = error_item_class
-
-        # ChatGPT client config
-        self.api_key = api_key or os.getenv("OPENAI_API_KEY") or self._empty_openai_api_key
-        self.max_retries = max_retries
-        self.timeout = timeout
-        self.async_client = async_client
-
-    async def filter_request(self, request_id: str, request_json: dict, request_headers: dict) -> Union[dict, JSONResponse, EventSourceResponse]:
-        for f in self.request_filters:
-            if json_resp := await f.filter(request_id, request_json, request_headers):
-                # Return response if filter returns string
-                resp_for_log = {
-                    "id": "-",
-                    "choices": [{"message": {"role": "assistant", "content": json_resp}, "finish_reason": "stop", "index": 0}],
-                    "created": 0,
-                    "model": "request_filter",
-                    "object": "chat.completion",
-                    "usage": {"prompt_tokens": 0, "completion_tokens": 0, "total_tokens": 0}
-                }
-                # Response log
-                self.access_logger_queue.put(self.response_item_class(
-                    request_id=request_id,
-                    response_json=resp_for_log,
-                    status_code=200
-                ))
-
-                if request_json.get("stream"):
-                    # Stream
-                    async def filter_response_stream(content: str):
-                        # First delta
-                        resp = {
-                            "id": "-",
-                            "choices": [{"delta": {"role": "assistant", "content": ""}, "finish_reason": None, "index": 0}],
-                            "created": 0,
-                            "model": "request_filter",
-                            "object": "chat.completion",
-                            "usage": {"prompt_tokens": 0, "completion_tokens": 0, "total_tokens": 0}
-                        }
-                        yield json.dumps(resp)
-                        # Last delta
-                        resp["choices"][0] = {"delta": {"content": content}, "finish_reason": "stop", "index": 0}
-                        yield json.dumps(resp)
-
-                    return self.return_response_with_headers(EventSourceResponse(
-                        filter_response_stream(json_resp)
-                    ), request_id)
-
-                else:
-                    # Non-stream
-                    return self.return_response_with_headers(JSONResponse(resp_for_log), request_id)
-
-        return request_json
-
-    def get_client(self):
-        return self.async_client or AsyncClient(
-            api_key=self.api_key,
-            max_retries=self.max_retries,
-            timeout=self.timeout
-        )
-
-    async def filter_response(self, request_id: str, response: ChatCompletion) -> ChatCompletion:
-        response_json = response.model_dump()
-
-        for f in self.response_filters:
-            if json_resp := await f.filter(request_id, response_json):
-                return response.model_validate(json_resp)
-
-        return response.model_validate(response_json)
-
-    def return_response_with_headers(self, resp: JSONResponse, request_id: str):
-        self.add_response_headers(response=resp, request_id=request_id)
-        return resp
-
-    def add_route(self, app: FastAPI, base_url: str):
-        @app.post(base_url)
-        async def handle_request(request: Request):
-            request_id = str(uuid4())
-            async_client = None
-
-            try:
-                start_time = time.time()
-                request_json = await request.json()
-                request_headers = dict(request.headers.items())
-
-                # Log request
-                self.access_logger_queue.put(self.request_item_class(
-                    request_id=request_id,
-                    request_json=request_json,
-                    request_headers=request_headers
-                ))
-
-                # Filter request
-                request_json = await self.filter_request(request_id, request_json, request_headers)
-                if isinstance(request_json, JSONResponse) or isinstance(request_json, EventSourceResponse):
-                    return request_json
-
-                # Call API
-                async_client = self.get_client()
-                start_time_api = time.time()
-                if self.api_key != self._empty_openai_api_key:
-                    # Always use server api key if set to client
-                    raw_response = await async_client.chat.completions.with_raw_response.create(**request_json)
-                elif user_auth_header := request_headers.get("authorization"):  # Lower case from client.
-                    raw_response = await async_client.chat.completions.with_raw_response.create(
-                        **request_json, extra_headers={"Authorization": user_auth_header}   # Pascal to server
-                    )
-                else:
-                    # Call API anyway ;)
-                    raw_response = await async_client.chat.completions.with_raw_response.create(**request_json)
-
-                completion_response = raw_response.parse()
-                completion_response_headers = raw_response.headers
-                completion_status_code = raw_response.status_code
-                if "content-encoding" in completion_response_headers:
-                    completion_response_headers.pop("content-encoding") # Remove "br" that will be changed by this proxy
-
-                # Handling response from API
-                if request_json.get("stream"):
-                    async def process_stream(stream: AsyncContentStream) -> AsyncGenerator[str, None]:
-                        # Async content generator
-                        try:
-                            async for chunk in stream:
-                                self.access_logger_queue.put(self.stream_response_item_class(
-                                    request_id=request_id,
-                                    chunk_json=chunk.model_dump()
-                                ))
-                                if chunk:
-                                    yield chunk.model_dump_json()
-
-                        finally:
-                            # Close client after reading stream
-                            await async_client.close()
-
-                            # Response log
-                            now = time.time()
-                            self.access_logger_queue.put(self.stream_response_item_class(
-                                request_id=request_id,
-                                response_headers=completion_response_headers,
-                                duration=now - start_time,
-                                duration_api=now - start_time_api,
-                                request_json=request_json,
-                                status_code=completion_status_code
-                            ))
-
-                    return self.return_response_with_headers(EventSourceResponse(
-                        process_stream(completion_response),
-                        headers=completion_response_headers
-                    ), request_id)
-
-                else:
-                    # Close client imediately
-                    await async_client.close()
-
-                    duration_api = time.time() - start_time_api
-
-                    # Filter response
-                    completion_response = await self.filter_response(request_id, completion_response)
-
-                    # Response log
-                    self.access_logger_queue.put(self.response_item_class(
-                        request_id=request_id,
-                        response_json=completion_response.model_dump(),
-                        response_headers=completion_response_headers,
-                        duration=time.time() - start_time,
-                        duration_api=duration_api,
-                        status_code=completion_status_code
-                    ))
-
-                    return self.return_response_with_headers(JSONResponse(
-                        content=completion_response.model_dump(),
-                        headers=completion_response_headers
-                    ), request_id)
-
-            # Error handlers
-            except RequestFilterException as rfex:
-                logger.error(f"Request filter error: {rfex}\n{traceback.format_exc()}")
-
-                resp_json = {"error": {"message": rfex.message, "type": "request_filter_error", "param": None, "code": None}}
-
-                # Error log
-                self.access_logger_queue.put(self.error_item_class(
-                    request_id=request_id,
-                    exception=rfex,
-                    traceback_info=traceback.format_exc(),
-                    response_json=resp_json,
-                    status_code=rfex.status_code
-                ))
-
-                return self.return_response_with_headers(JSONResponse(resp_json, status_code=rfex.status_code), request_id)
-
-            except ResponseFilterException as rfex:
-                logger.error(f"Response filter error: {rfex}\n{traceback.format_exc()}")
-
-                resp_json = {"error": {"message": rfex.message, "type": "response_filter_error", "param": None, "code": None}}
-
-                # Error log
-                self.access_logger_queue.put(self.error_item_class(
-                    request_id=request_id,
-                    exception=rfex,
-                    traceback_info=traceback.format_exc(),
-                    response_json=resp_json,
-                    status_code=rfex.status_code
-                ))
-
-                return self.return_response_with_headers(JSONResponse(resp_json, status_code=rfex.status_code), request_id)
-
-            except (APIStatusError, APIResponseValidationError) as status_err:
-                logger.error(f"APIStatusError from ChatGPT: {status_err}\n{traceback.format_exc()}")
-
-                # Error log
-                try:
-                    resp_json = status_err.response.json()
-                except:
-                    resp_json = str(status_err.response.content)
-
-                self.access_logger_queue.put(self.error_item_class(
-                    request_id=request_id,
-                    exception=status_err,
-                    traceback_info=traceback.format_exc(),
-                    response_json=resp_json,
-                    status_code=status_err.status_code
-                ))
-
-                return self.return_response_with_headers(JSONResponse(resp_json, status_code=status_err.status_code), request_id)
-
-            except APIError as api_err:
-                logger.error(f"APIError from ChatGPT: {api_err}\n{traceback.format_exc()}")
-
-                resp_json = {"error": {"message": api_err.message, "type": api_err.type, "param": api_err.param, "code": api_err.code}}
-
-                # Error log
-                self.access_logger_queue.put(self.error_item_class(
-                    request_id=request_id,
-                    exception=api_err,
-                    traceback_info=traceback.format_exc(),
-                    response_json=resp_json,
-                    status_code=502
-                ))
-
-                return self.return_response_with_headers(JSONResponse(resp_json, status_code=502), request_id)
-
-            except OpenAIError as oai_err:
-                logger.error(f"OpenAIError: {oai_err}\n{traceback.format_exc()}")
-
-                resp_json = {"error": {"message": str(oai_err), "type": "openai_error", "param": None, "code": None}}
-
-                # Error log
-                self.access_logger_queue.put(self.error_item_class(
-                    request_id=request_id,
-                    exception=oai_err,
-                    traceback_info=traceback.format_exc(),
-                    response_json=resp_json,
-                    status_code=502
-                ))
-
-                return self.return_response_with_headers(JSONResponse(resp_json, status_code=502), request_id)
-
-            except Exception as ex:
-                logger.error(f"Error at server: {ex}\n{traceback.format_exc()}")
-
-                resp_json = {"error": {"message": "Proxy error", "type": "proxy_error", "param": None, "code": None}}
-
-                # Error log
-                self.access_logger_queue.put(self.error_item_class(
-                    request_id=request_id,
-                    exception=ex,
-                    traceback_info=traceback.format_exc(),
-                    response_json=resp_json,
-                    status_code=502
-                ))
+        self.api_key = api_key
+        self.api_base_url = "https://api.openai.com/v1/chat/completions"
 
-                return self.return_response_with_headers(JSONResponse(resp_json, status_code=502), request_id)
+    def text_to_response_json(self, text: str) -> dict:
+        return {
+            "id": "-",
+            "object": "chat.completion",
+            "created": int(datetime.utcnow().timestamp()),
+            "model": "request_filter",
+            "choices": [{
+                "index": 0,
+                "message": {
+                "role": "assistant",
+                "content": text,
+                },
+                "finish_reason": "stop"
+            }],
+            "usage": {
+                "prompt_tokens": 0,
+                "completion_tokens": 0,
+                "total_tokens": 0
+            }
+        }
+
+    def text_to_response_chunks(self, text: str) -> List[dict]:
+        first_chunk = {
+            "id": "-",
+            "choices": [{"delta": {"role": "assistant", "content": ""}, "finish_reason": None, "index": 0}],
+            "created": 0,
+            "model": "request_filter",
+            "object": "chat.completion",
+            "usage": {"prompt_tokens": 0, "completion_tokens": 0, "total_tokens": 0}
+        }
+        last_chunk = {
+            "id": "-",
+            "choices": [{"delta": {"content": text}, "finish_reason": "stop", "index": 0}],
+            "created": 0,
+            "model": "request_filter",
+            "object": "chat.completion",
+            "usage": {"prompt_tokens": 0, "completion_tokens": 0, "total_tokens": 0}
+        }
+        return [first_chunk, last_chunk]
+
+    async def parse_request(self, fastapi_request: Request, session: SessionInfo):
+        await super().parse_request(fastapi_request, session)
+        session.stream = session.request_json.get("stream") is True
+
+    def prepare_httpx_request_headers(self, session: SessionInfo):
+        super().prepare_httpx_request_headers(session)
+        session.request_headers["authorization"] = f"Bearer {self.api_key}"
```

## aiproxy/queueclient.py

```diff
@@ -1,31 +1,15 @@
 from abc import ABC, abstractmethod
 import json
 from queue import Queue
 from typing import Iterator
 
 
 class QueueItemBase(ABC):
-    def to_dict(self) -> dict:
-        d = self.__dict__
-        d["type"] = self.__class__.__name__
-        return d
-
-    def to_json(self) -> str:
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_dict(cls, d: dict):
-        _d = d.copy()
-        del _d["type"]
-        return cls(**_d)
-
-    @classmethod
-    def from_json(cls, json_str: str):
-        return cls.from_dict(json.loads(json_str))
+    ...
 
 
 class QueueClientBase(ABC):
     dequeue_interval = 0.5
 
     @abstractmethod
     def put(self, item: QueueItemBase):
```

## Comparing `aiproxy_python-0.3.6.dist-info/LICENSE` & `aiproxy_python-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiproxy_python-0.3.6.dist-info/METADATA` & `aiproxy_python-0.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aiproxy-python
-Version: 0.3.6
+Version: 0.4.0
 Summary: 🦉AIProxy is a reverse proxy for ChatGPT API that provides monitoring, logging, and filtering requests and responses.
 Home-page: https://github.com/uezo/aiproxy
 Author: uezo
 Author-email: uezo@uezo.net
 Maintainer: uezo
 Maintainer-email: uezo@uezo.net
 License: Apache v2
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai ==1.3.6
+Requires-Dist: httpx ==0.27.0
 Requires-Dist: fastapi ==0.103.2
 Requires-Dist: uvicorn ==0.23.2
 Requires-Dist: sse-starlette ==1.8.2
 Requires-Dist: tiktoken ==0.5.1
 Requires-Dist: SQLAlchemy ==2.0.23
 
 # 🦉 AIProxy
```

