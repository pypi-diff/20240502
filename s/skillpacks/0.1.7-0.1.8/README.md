# Comparing `tmp/skillpacks-0.1.7.tar.gz` & `tmp/skillpacks-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillpacks-0.1.7.tar", max compression
+gzip compressed data, was "skillpacks-0.1.8.tar", max compression
```

## Comparing `skillpacks-0.1.7.tar` & `skillpacks-0.1.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11357 2024-01-08 19:16:31.383824 skillpacks-0.1.7/LICENSE
--rw-r--r--   0        0        0     3025 2024-04-29 03:02:23.181667 skillpacks-0.1.7/README.md
--rw-r--r--   0        0        0      600 2024-04-30 21:53:05.432591 skillpacks-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      152 2024-04-30 21:29:50.632480 skillpacks-0.1.7/skillpacks/__init__.py
--rw-r--r--   0        0        0       23 2024-04-28 03:37:56.034277 skillpacks-0.1.7/skillpacks/auth/default.py
--rw-r--r--   0        0        0     2546 2024-04-28 03:37:56.034595 skillpacks-0.1.7/skillpacks/auth/key.py
--rw-r--r--   0        0        0     2112 2024-04-28 03:37:56.034886 skillpacks-0.1.7/skillpacks/auth/provider.py
--rw-r--r--   0        0        0      735 2024-04-28 03:37:56.035160 skillpacks-0.1.7/skillpacks/auth/transport.py
--rw-r--r--   0        0        0    11392 2024-04-29 21:23:19.876063 skillpacks-0.1.7/skillpacks/base.py
--rw-r--r--   0        0        0     2253 2024-04-30 02:54:04.489588 skillpacks-0.1.7/skillpacks/db/conn.py
--rw-r--r--   0        0        0     1604 2024-04-29 21:22:55.291710 skillpacks-0.1.7/skillpacks/db/models.py
--rw-r--r--   0        0        0       74 2024-04-27 19:34:23.040044 skillpacks-0.1.7/skillpacks/env.py
--rw-r--r--   0        0        0        0 2024-02-21 19:35:35.693257 skillpacks-0.1.7/skillpacks/explore.py
--rw-r--r--   0        0        0       87 2024-02-22 23:30:11.834067 skillpacks-0.1.7/skillpacks/history/__init__.py
--rw-r--r--   0        0        0      855 2024-04-26 18:04:27.667449 skillpacks-0.1.7/skillpacks/history/base.py
--rw-r--r--   0        0        0      280 2024-04-26 18:04:50.655262 skillpacks-0.1.7/skillpacks/model/base.py
--rw-r--r--   0        0        0        0 2024-04-26 17:43:23.657039 skillpacks-0.1.7/skillpacks/model/qwenvl.py
--rw-r--r--   0        0        0      779 2024-02-22 00:28:00.918717 skillpacks-0.1.7/skillpacks/models/v1alpha/__init__.py
--rw-r--r--   0        0        0       60 2024-02-22 04:16:18.237373 skillpacks-0.1.7/skillpacks/select/__init__.py
--rw-r--r--   0        0        0     2076 2024-04-29 21:22:30.272421 skillpacks-0.1.7/skillpacks/select/base.py
--rw-r--r--   0        0        0       36 2024-02-22 23:57:15.420929 skillpacks-0.1.7/skillpacks/select/gpt4v/__init__.py
--rw-r--r--   0        0        0     4448 2024-04-26 18:05:05.435366 skillpacks-0.1.7/skillpacks/select/gpt4v/instruct.py
--rw-r--r--   0        0        0      838 2024-02-22 04:46:48.024589 skillpacks-0.1.7/skillpacks/select/gpt4v/oai.py
--rw-r--r--   0        0        0     2387 2024-04-26 18:05:20.328047 skillpacks-0.1.7/skillpacks/select/gpt4v/selector.py
--rw-r--r--   0        0        0     2890 2024-04-26 18:05:28.464384 skillpacks-0.1.7/skillpacks/select/qwenvl/instruct.py
--rw-r--r--   0        0        0     2765 2024-04-26 18:05:35.975702 skillpacks-0.1.7/skillpacks/select/qwenvl/selector.py
--rw-r--r--   0        0        0      230 2024-02-22 04:46:17.754077 skillpacks-0.1.7/skillpacks/select/util.py
--rw-r--r--   0        0        0     1756 2024-04-29 21:19:18.545481 skillpacks-0.1.7/skillpacks/server/models.py
--rw-r--r--   0        0        0     2077 2024-04-29 21:15:22.895837 skillpacks-0.1.7/skillpacks/server/routes/action.py
--rw-r--r--   0        0        0     2602 2024-04-29 21:15:30.688255 skillpacks-0.1.7/skillpacks/server/routes/episode.py
--rw-r--r--   0        0        0     2669 2024-04-29 21:23:35.336627 skillpacks-0.1.7/skillpacks/task_old.py
--rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 skillpacks-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-08 19:16:31.383824 skillpacks-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3025 2024-04-29 03:02:23.181667 skillpacks-0.1.8/README.md
+-rw-r--r--   0        0        0      600 2024-05-01 20:54:02.105637 skillpacks-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-04-30 21:29:50.632480 skillpacks-0.1.8/skillpacks/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-28 03:37:56.034277 skillpacks-0.1.8/skillpacks/auth/default.py
+-rw-r--r--   0        0        0     2546 2024-04-28 03:37:56.034595 skillpacks-0.1.8/skillpacks/auth/key.py
+-rw-r--r--   0        0        0     2112 2024-04-28 03:37:56.034886 skillpacks-0.1.8/skillpacks/auth/provider.py
+-rw-r--r--   0        0        0      735 2024-04-28 03:37:56.035160 skillpacks-0.1.8/skillpacks/auth/transport.py
+-rw-r--r--   0        0        0    11392 2024-04-29 21:23:19.876063 skillpacks-0.1.8/skillpacks/base.py
+-rw-r--r--   0        0        0     2253 2024-04-30 02:54:04.489588 skillpacks-0.1.8/skillpacks/db/conn.py
+-rw-r--r--   0        0        0     1604 2024-04-29 21:22:55.291710 skillpacks-0.1.8/skillpacks/db/models.py
+-rw-r--r--   0        0        0       74 2024-04-27 19:34:23.040044 skillpacks-0.1.8/skillpacks/env.py
+-rw-r--r--   0        0        0        0 2024-02-21 19:35:35.693257 skillpacks-0.1.8/skillpacks/explore.py
+-rw-r--r--   0        0        0       87 2024-02-22 23:30:11.834067 skillpacks-0.1.8/skillpacks/history/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-26 18:04:27.667449 skillpacks-0.1.8/skillpacks/history/base.py
+-rw-r--r--   0        0        0      280 2024-04-26 18:04:50.655262 skillpacks-0.1.8/skillpacks/model/base.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:43:23.657039 skillpacks-0.1.8/skillpacks/model/qwenvl.py
+-rw-r--r--   0        0        0      779 2024-02-22 00:28:00.918717 skillpacks-0.1.8/skillpacks/models/v1alpha/__init__.py
+-rw-r--r--   0        0        0       60 2024-02-22 04:16:18.237373 skillpacks-0.1.8/skillpacks/select/__init__.py
+-rw-r--r--   0        0        0     2076 2024-04-29 21:22:30.272421 skillpacks-0.1.8/skillpacks/select/base.py
+-rw-r--r--   0        0        0       36 2024-02-22 23:57:15.420929 skillpacks-0.1.8/skillpacks/select/gpt4v/__init__.py
+-rw-r--r--   0        0        0     4448 2024-04-26 18:05:05.435366 skillpacks-0.1.8/skillpacks/select/gpt4v/instruct.py
+-rw-r--r--   0        0        0      838 2024-02-22 04:46:48.024589 skillpacks-0.1.8/skillpacks/select/gpt4v/oai.py
+-rw-r--r--   0        0        0     2387 2024-04-26 18:05:20.328047 skillpacks-0.1.8/skillpacks/select/gpt4v/selector.py
+-rw-r--r--   0        0        0     2890 2024-04-26 18:05:28.464384 skillpacks-0.1.8/skillpacks/select/qwenvl/instruct.py
+-rw-r--r--   0        0        0     2765 2024-04-26 18:05:35.975702 skillpacks-0.1.8/skillpacks/select/qwenvl/selector.py
+-rw-r--r--   0        0        0      230 2024-02-22 04:46:17.754077 skillpacks-0.1.8/skillpacks/select/util.py
+-rw-r--r--   0        0        0     1657 2024-05-01 20:53:49.995360 skillpacks-0.1.8/skillpacks/server/models.py
+-rw-r--r--   0        0        0     2077 2024-04-29 21:15:22.895837 skillpacks-0.1.8/skillpacks/server/routes/action.py
+-rw-r--r--   0        0        0     2602 2024-04-29 21:15:30.688255 skillpacks-0.1.8/skillpacks/server/routes/episode.py
+-rw-r--r--   0        0        0     2669 2024-04-29 21:23:35.336627 skillpacks-0.1.8/skillpacks/task_old.py
+-rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 skillpacks-0.1.8/PKG-INFO
```

### Comparing `skillpacks-0.1.7/LICENSE` & `skillpacks-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/README.md` & `skillpacks-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/pyproject.toml` & `skillpacks-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skillpacks"
-version = "0.1.7"
+version = "0.1.8"
 description = "Pluggable skills for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `skillpacks-0.1.7/skillpacks/auth/key.py` & `skillpacks-0.1.8/skillpacks/auth/key.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/auth/provider.py` & `skillpacks-0.1.8/skillpacks/auth/provider.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/auth/transport.py` & `skillpacks-0.1.8/skillpacks/auth/transport.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/base.py` & `skillpacks-0.1.8/skillpacks/base.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/db/conn.py` & `skillpacks-0.1.8/skillpacks/db/conn.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/db/models.py` & `skillpacks-0.1.8/skillpacks/db/models.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/history/base.py` & `skillpacks-0.1.8/skillpacks/history/base.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/models/v1alpha/__init__.py` & `skillpacks-0.1.8/skillpacks/models/v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/select/base.py` & `skillpacks-0.1.8/skillpacks/select/base.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/select/gpt4v/instruct.py` & `skillpacks-0.1.8/skillpacks/select/gpt4v/instruct.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/select/gpt4v/oai.py` & `skillpacks-0.1.8/skillpacks/select/gpt4v/oai.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/select/gpt4v/selector.py` & `skillpacks-0.1.8/skillpacks/select/gpt4v/selector.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/select/qwenvl/instruct.py` & `skillpacks-0.1.8/skillpacks/select/qwenvl/instruct.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/select/qwenvl/selector.py` & `skillpacks-0.1.8/skillpacks/select/qwenvl/selector.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/server/routes/action.py` & `skillpacks-0.1.8/skillpacks/server/routes/action.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/server/routes/episode.py` & `skillpacks-0.1.8/skillpacks/server/routes/episode.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/skillpacks/task_old.py` & `skillpacks-0.1.8/skillpacks/task_old.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.7/PKG-INFO` & `skillpacks-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillpacks
-Version: 0.1.7
+Version: 0.1.8
 Summary: Pluggable skills for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skillpacks Version: 0.1.7 Summary: Pluggable skills
+Metadata-Version: 2.1 Name: skillpacks Version: 0.1.8 Summary: Pluggable skills
 for AI agents License: Apache 2.0 Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: mllm (>=0.1.8,<0.2.0) Requires-Dist:
 pydantic (>=2.6.1,<3.0.0) Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
 Description-Content-Type: text/markdown
```

