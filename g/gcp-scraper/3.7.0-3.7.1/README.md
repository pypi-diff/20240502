# Comparing `tmp/gcp-scraper-3.7.0.tar.gz` & `tmp/gcp-scraper-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp-scraper-3.7.0.tar", last modified: Thu Apr 18 13:01:06 2024, max compression
+gzip compressed data, was "gcp-scraper-3.7.1.tar", last modified: Thu May  2 11:11:40 2024, max compression
```

## Comparing `gcp-scraper-3.7.0.tar` & `gcp-scraper-3.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-18 13:01:06.203067 gcp-scraper-3.7.0/
--rw-r--r--   0 cuz        (501) staff       (20)    35149 2023-08-11 13:24:50.000000 gcp-scraper-3.7.0/LICENSE
--rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-18 13:01:06.202779 gcp-scraper-3.7.0/PKG-INFO
--rw-r--r--   0 cuz        (501) staff       (20)       45 2023-08-11 13:24:50.000000 gcp-scraper-3.7.0/README.md
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-18 13:01:06.198430 gcp-scraper-3.7.0/gcp_scraper.egg-info/
--rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-18 13:01:05.000000 gcp-scraper-3.7.0/gcp_scraper.egg-info/PKG-INFO
--rw-r--r--   0 cuz        (501) staff       (20)      497 2024-04-18 13:01:06.000000 gcp-scraper-3.7.0/gcp_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 cuz        (501) staff       (20)        1 2024-04-18 13:01:05.000000 gcp-scraper-3.7.0/gcp_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 cuz        (501) staff       (20)      198 2024-04-18 13:01:05.000000 gcp-scraper-3.7.0/gcp_scraper.egg-info/requires.txt
--rw-r--r--   0 cuz        (501) staff       (20)        9 2024-04-18 13:01:05.000000 gcp-scraper-3.7.0/gcp_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-18 13:01:06.183237 gcp-scraper-3.7.0/gscraper/
--rwxr-xr-x   0 cuz        (501) staff       (20)      284 2024-04-18 13:00:36.000000 gcp-scraper-3.7.0/gscraper/__init__.py
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-18 13:01:06.195134 gcp-scraper-3.7.0/gscraper/base/
--rwxr-xr-x   0 cuz        (501) staff       (20)        0 2023-10-27 05:39:56.000000 gcp-scraper-3.7.0/gscraper/base/__init__.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    22817 2024-04-13 00:20:53.000000 gcp-scraper-3.7.0/gscraper/base/abstract.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    38670 2024-03-23 03:20:34.000000 gcp-scraper-3.7.0/gscraper/base/gcloud.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    89023 2024-04-18 12:57:21.000000 gcp-scraper-3.7.0/gscraper/base/session.py
--rwxr-xr-x   0 cuz        (501) staff       (20)   117188 2024-04-18 13:00:09.000000 gcp-scraper-3.7.0/gscraper/base/spider.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    19111 2024-03-23 03:20:19.000000 gcp-scraper-3.7.0/gscraper/base/types.py
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-18 13:01:06.198098 gcp-scraper-3.7.0/gscraper/utils/
--rwxr-xr-x   0 cuz        (501) staff       (20)      962 2023-12-05 12:25:11.000000 gcp-scraper-3.7.0/gscraper/utils/__init__.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    11448 2024-03-30 10:37:57.000000 gcp-scraper-3.7.0/gscraper/utils/cast.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    16069 2024-02-24 02:47:12.000000 gcp-scraper-3.7.0/gscraper/utils/date.py
--rwxr-xr-x   0 cuz        (501) staff       (20)     8113 2023-11-08 14:08:25.000000 gcp-scraper-3.7.0/gscraper/utils/logs.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    69662 2024-04-18 12:54:00.000000 gcp-scraper-3.7.0/gscraper/utils/map.py
--rw-r--r--   0 cuz        (501) staff       (20)       38 2024-04-18 13:01:06.204021 gcp-scraper-3.7.0/setup.cfg
--rw-r--r--   0 cuz        (501) staff       (20)      764 2023-09-10 13:21:42.000000 gcp-scraper-3.7.0/setup.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-05-02 11:11:40.862336 gcp-scraper-3.7.1/
+-rw-r--r--   0 cuz        (501) staff       (20)    35149 2023-08-11 13:24:50.000000 gcp-scraper-3.7.1/LICENSE
+-rw-r--r--   0 cuz        (501) staff       (20)      679 2024-05-02 11:11:40.862055 gcp-scraper-3.7.1/PKG-INFO
+-rw-r--r--   0 cuz        (501) staff       (20)       45 2023-08-11 13:24:50.000000 gcp-scraper-3.7.1/README.md
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-05-02 11:11:40.861339 gcp-scraper-3.7.1/gcp_scraper.egg-info/
+-rw-r--r--   0 cuz        (501) staff       (20)      679 2024-05-02 11:11:40.000000 gcp-scraper-3.7.1/gcp_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 cuz        (501) staff       (20)      497 2024-05-02 11:11:40.000000 gcp-scraper-3.7.1/gcp_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 cuz        (501) staff       (20)        1 2024-05-02 11:11:40.000000 gcp-scraper-3.7.1/gcp_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 cuz        (501) staff       (20)      198 2024-05-02 11:11:40.000000 gcp-scraper-3.7.1/gcp_scraper.egg-info/requires.txt
+-rw-r--r--   0 cuz        (501) staff       (20)        9 2024-05-02 11:11:40.000000 gcp-scraper-3.7.1/gcp_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-05-02 11:11:40.851445 gcp-scraper-3.7.1/gscraper/
+-rwxr-xr-x   0 cuz        (501) staff       (20)      284 2024-05-02 11:11:20.000000 gcp-scraper-3.7.1/gscraper/__init__.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-05-02 11:11:40.856703 gcp-scraper-3.7.1/gscraper/base/
+-rwxr-xr-x   0 cuz        (501) staff       (20)        0 2023-10-27 05:39:56.000000 gcp-scraper-3.7.1/gscraper/base/__init__.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    22834 2024-05-02 11:07:36.000000 gcp-scraper-3.7.1/gscraper/base/abstract.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    38670 2024-03-23 03:20:34.000000 gcp-scraper-3.7.1/gscraper/base/gcloud.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    89023 2024-04-18 12:57:21.000000 gcp-scraper-3.7.1/gscraper/base/session.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)   117211 2024-05-02 11:11:02.000000 gcp-scraper-3.7.1/gscraper/base/spider.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    19111 2024-03-23 03:20:19.000000 gcp-scraper-3.7.1/gscraper/base/types.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-05-02 11:11:40.860490 gcp-scraper-3.7.1/gscraper/utils/
+-rwxr-xr-x   0 cuz        (501) staff       (20)      962 2023-12-05 12:25:11.000000 gcp-scraper-3.7.1/gscraper/utils/__init__.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    11448 2024-03-30 10:37:57.000000 gcp-scraper-3.7.1/gscraper/utils/cast.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    16069 2024-02-24 02:47:12.000000 gcp-scraper-3.7.1/gscraper/utils/date.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)     8113 2023-11-08 14:08:25.000000 gcp-scraper-3.7.1/gscraper/utils/logs.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    69662 2024-04-18 12:54:00.000000 gcp-scraper-3.7.1/gscraper/utils/map.py
+-rw-r--r--   0 cuz        (501) staff       (20)       38 2024-05-02 11:11:40.863138 gcp-scraper-3.7.1/setup.cfg
+-rw-r--r--   0 cuz        (501) staff       (20)      764 2023-09-10 13:21:42.000000 gcp-scraper-3.7.1/setup.py
```

### Comparing `gcp-scraper-3.7.0/LICENSE` & `gcp-scraper-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.7.0/PKG-INFO` & `gcp-scraper-3.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-scraper
-Version: 3.7.0
+Version: 3.7.1
 Summary: Scraping utils with GCP functions
 Home-page: https://github.com/minyeamer/gscraper.git
 Author: minyeamer
 Author-email: minyeamer@gmail.com
 License: minyeamer
 Keywords: gcp-scraper,scraper,gcp
 Requires-Python: >=3.7
```

### Comparing `gcp-scraper-3.7.0/gcp_scraper.egg-info/PKG-INFO` & `gcp-scraper-3.7.1/gcp_scraper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-scraper
-Version: 3.7.0
+Version: 3.7.1
 Summary: Scraping utils with GCP functions
 Home-page: https://github.com/minyeamer/gscraper.git
 Author: minyeamer
 Author-email: minyeamer@gmail.com
 License: minyeamer
 Keywords: gcp-scraper,scraper,gcp
 Requires-Python: >=3.7
```

### Comparing `gcp-scraper-3.7.0/gscraper/base/abstract.py` & `gcp-scraper-3.7.1/gscraper/base/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 SPIDER_CONTEXT = lambda asyncio=None, host=None, field=None, ssl=None, mappedReturn=None, \
                         maxLimit=None, redirectLimit=None, **context: context
 
 
 ENCRYPTED_CONTEXT = lambda decryptedKey=None, auth=None, authKey=None, sessionCookies=None, **context: context
 
 
-UNIQUE_CONTEXT = lambda derivFields=None, dags=None, **context: \
+UNIQUE_CONTEXT = lambda derivFields=None, taskErrors=None, dags=None, **context: \
     ENCRYPTED_CONTEXT(**SPIDER_CONTEXT(**MAP_CONTEXT(**ITERATOR_CONTEXT(**LOG_CONTEXT(**BASE_CONTEXT(**context))))))
 
 
 PARAMS_CONTEXT = lambda init=None, data=None, task=None, worker=None, locals=None, which=None, where=None, by=None, verb=None, \
                         how=None, default=None, dropna=None, strict=None, unique=None, drop=None, index=None, log=None, \
                         depth=None, hier=None, to=None, countPath=None, hasSize=None, **context: context
```

### Comparing `gcp-scraper-3.7.0/gscraper/base/gcloud.py` & `gcp-scraper-3.7.1/gscraper/base/gcloud.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.7.0/gscraper/base/session.py` & `gcp-scraper-3.7.1/gscraper/base/session.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.7.0/gscraper/base/spider.py` & `gcp-scraper-3.7.1/gscraper/base/spider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1669,15 +1669,15 @@
         if isinstance(self.authKey, Sequence): return kloc(auth_info, self.authKey, if_null="pass")
         elif isinstance(self.authKey, Callable): return self.authKey(**auth_info)
         else: raise AuthenticationError(INVALID_OBJECT_TYPE_MSG(self.authKey, AUTH_KEY))
 
     def validate_account(self, auth: LoginSpider, sessionCookies=False, **context) -> Context:
         try: self.login(auth, **context)
         except: raise AuthenticationError(INVALID_USER_INFO_MSG(self.where))
-        if isinstance(auth, LoginCookie) or not (sessionCookies and self.sessionCookies):
+        if isinstance(auth, LoginCookie) or (not self.sessionCookies):
             context["cookies"] = self.cookies
         return context
 
     def login(self, auth: LoginSpider, **context):
         auth.login()
         auth.update_cookies(self.set_cookies(**context), if_exists="replace")
         self.checkpoint("login", where="login", msg={"cookies":auth.get_cookies(encode=False)})
@@ -2017,14 +2017,15 @@
     ranges = list()
     numRetries = 0
     delay = 1.
     interruptType = tuple()
     errorType = tuple()
     returnType = "dataframe"
     mappedReturn = False
+    taskErrors = dict()
     info = PipelineInfo()
     dags = Dag()
 
     @abstractmethod
     @EncryptedSession.init_task
     def crawl(self, **context) -> Data:
         return self.gather(**context)
@@ -2047,15 +2048,15 @@
             data[task[DATANAME]] = self.run_task(task, fields=fields, data=data, **context)
         return self.map_reduce(fields=fields, returnType=returnType, **dict(context, **data))
 
     def run_task(self, task: Task, fields: IndexLabel=list(), data: Dict[_KT,Data]=dict(), **context) -> Data:
         fields = self._get_fields(fields, allowed=task.get(ALLOWED), name=task[DATANAME])
         method, worker, params = self._from_task(task, fields=fields, data=data, **context)
         response = method(**params)
-        self.errors.append({task[NAME]:worker.errors})
+        self.taskErrors[task[NAME]] = worker.errors
         self.checkpoint(task[NAME], where=method.__name__, msg={"data":response}, save=response)
         return response
 
     def _get_fields(self, fields: IndexLabel=list(), allowed: Optional[IndexLabel]=None, name=str()) -> IndexLabel:
         if self.mappedReturn and isinstance(fields, Dict):
             fields = fields.get(name, list())
             if isinstance(fields, Dict):
@@ -2136,14 +2137,15 @@
     ranges = list()
     numRetries = 0
     delay = 1.
     interruptType = tuple()
     errorType = tuple()
     returnType = "dataframe"
     mappedReturn = False
+    taskErrors = dict()
     info = PipelineInfo()
     dags = Dag()
 
     @abstractmethod
     @EncryptedAsyncSession.init_task
     async def crawl(self, **context) -> Data:
         return await self.gather(**context)
@@ -2158,14 +2160,14 @@
             else: data[task[DATANAME]] = await self.run_task(task, fields=fields, data=data, **context)
         return self.map_reduce(fields=fields, returnType=returnType, **dict(context, **data))
 
     async def run_task(self, task: Task, fields: IndexLabel=list(), data: Dict[_KT,Data]=dict(), **context) -> Data:
         fields = self._get_fields(fields, allowed=task.get(ALLOWED), name=task[DATANAME])
         method, worker, params = self._from_task(task, fields=fields, data=data, **context)
         response = (await method(**params)) if inspect.iscoroutinefunction(method) else method(**params)
-        self.errors.append({task[NAME]:worker.errors})
+        self.taskErrors[task[NAME]] = worker.errors
         self.checkpoint(task[NAME], where=task, msg={"data":response}, save=response)
         return response
 
     @EncryptedAsyncSession.limit_request
     async def async_crawl(self, worker: AsyncSpider, **params) -> Data:
         return await worker.crawl(**params)
```

### Comparing `gcp-scraper-3.7.0/gscraper/base/types.py` & `gcp-scraper-3.7.1/gscraper/base/types.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.7.0/gscraper/utils/__init__.py` & `gcp-scraper-3.7.1/gscraper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.7.0/gscraper/utils/cast.py` & `gcp-scraper-3.7.1/gscraper/utils/cast.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.7.0/gscraper/utils/date.py` & `gcp-scraper-3.7.1/gscraper/utils/date.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.7.0/gscraper/utils/logs.py` & `gcp-scraper-3.7.1/gscraper/utils/logs.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.7.0/gscraper/utils/map.py` & `gcp-scraper-3.7.1/gscraper/utils/map.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.7.0/setup.py` & `gcp-scraper-3.7.1/setup.py`

 * *Files identical despite different names*

