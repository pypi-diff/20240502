# Comparing `tmp/skillpacks-0.1.8.tar.gz` & `tmp/skillpacks-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillpacks-0.1.8.tar", max compression
+gzip compressed data, was "skillpacks-0.1.9.tar", max compression
```

## Comparing `skillpacks-0.1.8.tar` & `skillpacks-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11357 2024-01-08 19:16:31.383824 skillpacks-0.1.8/LICENSE
--rw-r--r--   0        0        0     3025 2024-04-29 03:02:23.181667 skillpacks-0.1.8/README.md
--rw-r--r--   0        0        0      600 2024-05-01 20:54:02.105637 skillpacks-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      152 2024-04-30 21:29:50.632480 skillpacks-0.1.8/skillpacks/__init__.py
--rw-r--r--   0        0        0       23 2024-04-28 03:37:56.034277 skillpacks-0.1.8/skillpacks/auth/default.py
--rw-r--r--   0        0        0     2546 2024-04-28 03:37:56.034595 skillpacks-0.1.8/skillpacks/auth/key.py
--rw-r--r--   0        0        0     2112 2024-04-28 03:37:56.034886 skillpacks-0.1.8/skillpacks/auth/provider.py
--rw-r--r--   0        0        0      735 2024-04-28 03:37:56.035160 skillpacks-0.1.8/skillpacks/auth/transport.py
--rw-r--r--   0        0        0    11392 2024-04-29 21:23:19.876063 skillpacks-0.1.8/skillpacks/base.py
--rw-r--r--   0        0        0     2253 2024-04-30 02:54:04.489588 skillpacks-0.1.8/skillpacks/db/conn.py
--rw-r--r--   0        0        0     1604 2024-04-29 21:22:55.291710 skillpacks-0.1.8/skillpacks/db/models.py
--rw-r--r--   0        0        0       74 2024-04-27 19:34:23.040044 skillpacks-0.1.8/skillpacks/env.py
--rw-r--r--   0        0        0        0 2024-02-21 19:35:35.693257 skillpacks-0.1.8/skillpacks/explore.py
--rw-r--r--   0        0        0       87 2024-02-22 23:30:11.834067 skillpacks-0.1.8/skillpacks/history/__init__.py
--rw-r--r--   0        0        0      855 2024-04-26 18:04:27.667449 skillpacks-0.1.8/skillpacks/history/base.py
--rw-r--r--   0        0        0      280 2024-04-26 18:04:50.655262 skillpacks-0.1.8/skillpacks/model/base.py
--rw-r--r--   0        0        0        0 2024-04-26 17:43:23.657039 skillpacks-0.1.8/skillpacks/model/qwenvl.py
--rw-r--r--   0        0        0      779 2024-02-22 00:28:00.918717 skillpacks-0.1.8/skillpacks/models/v1alpha/__init__.py
--rw-r--r--   0        0        0       60 2024-02-22 04:16:18.237373 skillpacks-0.1.8/skillpacks/select/__init__.py
--rw-r--r--   0        0        0     2076 2024-04-29 21:22:30.272421 skillpacks-0.1.8/skillpacks/select/base.py
--rw-r--r--   0        0        0       36 2024-02-22 23:57:15.420929 skillpacks-0.1.8/skillpacks/select/gpt4v/__init__.py
--rw-r--r--   0        0        0     4448 2024-04-26 18:05:05.435366 skillpacks-0.1.8/skillpacks/select/gpt4v/instruct.py
--rw-r--r--   0        0        0      838 2024-02-22 04:46:48.024589 skillpacks-0.1.8/skillpacks/select/gpt4v/oai.py
--rw-r--r--   0        0        0     2387 2024-04-26 18:05:20.328047 skillpacks-0.1.8/skillpacks/select/gpt4v/selector.py
--rw-r--r--   0        0        0     2890 2024-04-26 18:05:28.464384 skillpacks-0.1.8/skillpacks/select/qwenvl/instruct.py
--rw-r--r--   0        0        0     2765 2024-04-26 18:05:35.975702 skillpacks-0.1.8/skillpacks/select/qwenvl/selector.py
--rw-r--r--   0        0        0      230 2024-02-22 04:46:17.754077 skillpacks-0.1.8/skillpacks/select/util.py
--rw-r--r--   0        0        0     1657 2024-05-01 20:53:49.995360 skillpacks-0.1.8/skillpacks/server/models.py
--rw-r--r--   0        0        0     2077 2024-04-29 21:15:22.895837 skillpacks-0.1.8/skillpacks/server/routes/action.py
--rw-r--r--   0        0        0     2602 2024-04-29 21:15:30.688255 skillpacks-0.1.8/skillpacks/server/routes/episode.py
--rw-r--r--   0        0        0     2669 2024-04-29 21:23:35.336627 skillpacks-0.1.8/skillpacks/task_old.py
--rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 skillpacks-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-08 19:16:31.383824 skillpacks-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3025 2024-04-29 03:02:23.181667 skillpacks-0.1.9/README.md
+-rw-r--r--   0        0        0      601 2024-05-02 18:52:31.064696 skillpacks-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-04-30 21:29:50.632480 skillpacks-0.1.9/skillpacks/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-28 03:37:56.034277 skillpacks-0.1.9/skillpacks/auth/default.py
+-rw-r--r--   0        0        0     2546 2024-04-28 03:37:56.034595 skillpacks-0.1.9/skillpacks/auth/key.py
+-rw-r--r--   0        0        0     2112 2024-04-28 03:37:56.034886 skillpacks-0.1.9/skillpacks/auth/provider.py
+-rw-r--r--   0        0        0      735 2024-04-28 03:37:56.035160 skillpacks-0.1.9/skillpacks/auth/transport.py
+-rw-r--r--   0        0        0    11392 2024-04-29 21:23:19.876063 skillpacks-0.1.9/skillpacks/base.py
+-rw-r--r--   0        0        0     2319 2024-05-02 18:51:58.063019 skillpacks-0.1.9/skillpacks/db/conn.py
+-rw-r--r--   0        0        0     1604 2024-04-29 21:22:55.291710 skillpacks-0.1.9/skillpacks/db/models.py
+-rw-r--r--   0        0        0       74 2024-04-27 19:34:23.040044 skillpacks-0.1.9/skillpacks/env.py
+-rw-r--r--   0        0        0        0 2024-02-21 19:35:35.693257 skillpacks-0.1.9/skillpacks/explore.py
+-rw-r--r--   0        0        0       87 2024-02-22 23:30:11.834067 skillpacks-0.1.9/skillpacks/history/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-26 18:04:27.667449 skillpacks-0.1.9/skillpacks/history/base.py
+-rw-r--r--   0        0        0      280 2024-04-26 18:04:50.655262 skillpacks-0.1.9/skillpacks/model/base.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:43:23.657039 skillpacks-0.1.9/skillpacks/model/qwenvl.py
+-rw-r--r--   0        0        0      779 2024-02-22 00:28:00.918717 skillpacks-0.1.9/skillpacks/models/v1alpha/__init__.py
+-rw-r--r--   0        0        0       60 2024-02-22 04:16:18.237373 skillpacks-0.1.9/skillpacks/select/__init__.py
+-rw-r--r--   0        0        0     2076 2024-04-29 21:22:30.272421 skillpacks-0.1.9/skillpacks/select/base.py
+-rw-r--r--   0        0        0       36 2024-02-22 23:57:15.420929 skillpacks-0.1.9/skillpacks/select/gpt4v/__init__.py
+-rw-r--r--   0        0        0     4448 2024-04-26 18:05:05.435366 skillpacks-0.1.9/skillpacks/select/gpt4v/instruct.py
+-rw-r--r--   0        0        0      838 2024-02-22 04:46:48.024589 skillpacks-0.1.9/skillpacks/select/gpt4v/oai.py
+-rw-r--r--   0        0        0     2387 2024-04-26 18:05:20.328047 skillpacks-0.1.9/skillpacks/select/gpt4v/selector.py
+-rw-r--r--   0        0        0     2890 2024-04-26 18:05:28.464384 skillpacks-0.1.9/skillpacks/select/qwenvl/instruct.py
+-rw-r--r--   0        0        0     2765 2024-04-26 18:05:35.975702 skillpacks-0.1.9/skillpacks/select/qwenvl/selector.py
+-rw-r--r--   0        0        0      230 2024-02-22 04:46:17.754077 skillpacks-0.1.9/skillpacks/select/util.py
+-rw-r--r--   0        0        0     1657 2024-05-01 20:53:49.995360 skillpacks-0.1.9/skillpacks/server/models.py
+-rw-r--r--   0        0        0     2077 2024-04-29 21:15:22.895837 skillpacks-0.1.9/skillpacks/server/routes/action.py
+-rw-r--r--   0        0        0     2602 2024-04-29 21:15:30.688255 skillpacks-0.1.9/skillpacks/server/routes/episode.py
+-rw-r--r--   0        0        0     2669 2024-04-29 21:23:35.336627 skillpacks-0.1.9/skillpacks/task_old.py
+-rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 skillpacks-0.1.9/PKG-INFO
```

### Comparing `skillpacks-0.1.8/LICENSE` & `skillpacks-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/README.md` & `skillpacks-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/pyproject.toml` & `skillpacks-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "skillpacks"
-version = "0.1.8"
+version = "0.1.9"
 description = "Pluggable skills for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.6.1"
 sqlalchemy = "^2.0.27"
-mllm = "^0.1.8"
+mllm = "^0.1.10"
 
 
 [tool.poetry.group.openai.dependencies]
 openai = "^1.12.0"
 
 
 [tool.poetry.group.qwen.dependencies]
```

### Comparing `skillpacks-0.1.8/skillpacks/auth/key.py` & `skillpacks-0.1.9/skillpacks/auth/key.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/auth/provider.py` & `skillpacks-0.1.9/skillpacks/auth/provider.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/auth/transport.py` & `skillpacks-0.1.9/skillpacks/auth/transport.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/base.py` & `skillpacks-0.1.9/skillpacks/base.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/db/conn.py` & `skillpacks-0.1.9/skillpacks/db/conn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 import os
 import time
+import logging
 
 from sqlalchemy import create_engine, Engine
 from sqlalchemy.orm import sessionmaker
 
 from .models import Base
 
+logger = logging.getLogger(__name__)
 
 DB_TYPE = os.environ.get("DB_TYPE", "sqlite")
 
 
 def get_pg_conn() -> Engine:
     # Helper function to get environment variable with fallback
     def get_env_var(key: str) -> str:
-        task_key = f"SKILL_{key}"
+        task_key = f"SKILLS_{key}"
         value = os.environ.get(task_key)
         if value is None:
             value = os.environ.get(key)
             if value is None:
                 raise ValueError(f"${key} must be set")
         return value
 
     # Retrieve environment variables with fallbacks
     db_user = get_env_var("DB_USER")
     db_password = get_env_var("DB_PASS")
     db_host = get_env_var("DB_HOST")
     db_name = get_env_var("DB_NAME")
 
-    print(f"\nconnecting to db on postgres host '{db_host}' with db '{db_name}'")
+    logger.debug(f"connecting to db on postgres host '{db_host}' with db '{db_name}'")
     engine = create_engine(
         f"postgresql+psycopg2://{db_user}:{db_password}@{db_host}/{db_name}",
         client_encoding="utf8",
     )
 
     return engine
 
 
 def get_sqlite_conn() -> Engine:
-    db_name = os.environ.get("SKILL_DB_NAME", "skills.db")
-    db_path = os.environ.get("SKILL_DB_PATH", "./.data")
-    db_test = os.environ.get("SKILL_DB_TEST", "false") == "true"
+    db_name = os.environ.get("SKILLS_DB_NAME", "skills.db")
+    db_path = os.environ.get("SKILLS_DB_PATH", "./.data")
+    db_test = os.environ.get("SKILLS_DB_TEST", "false") == "true"
     if db_test:
         db_name = f"skill_test_{int(time.time())}.db"
-    print(f"\nconnecting to local sqlite db ./data/{db_name}")
+    logger.debug(f"connecting to local sqlite db ./data/{db_name}")
     os.makedirs(os.path.dirname(f"{db_path}/{db_name}"), exist_ok=True)
     engine = create_engine(f"sqlite:///{db_path}/{db_name}")
     return engine
 
 
 if DB_TYPE == "postgres":
     engine = get_pg_conn()
```

### Comparing `skillpacks-0.1.8/skillpacks/db/models.py` & `skillpacks-0.1.9/skillpacks/db/models.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/history/base.py` & `skillpacks-0.1.9/skillpacks/history/base.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/models/v1alpha/__init__.py` & `skillpacks-0.1.9/skillpacks/models/v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/select/base.py` & `skillpacks-0.1.9/skillpacks/select/base.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/select/gpt4v/instruct.py` & `skillpacks-0.1.9/skillpacks/select/gpt4v/instruct.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/select/gpt4v/oai.py` & `skillpacks-0.1.9/skillpacks/select/gpt4v/oai.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/select/gpt4v/selector.py` & `skillpacks-0.1.9/skillpacks/select/gpt4v/selector.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/select/qwenvl/instruct.py` & `skillpacks-0.1.9/skillpacks/select/qwenvl/instruct.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/select/qwenvl/selector.py` & `skillpacks-0.1.9/skillpacks/select/qwenvl/selector.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/server/models.py` & `skillpacks-0.1.9/skillpacks/server/models.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/server/routes/action.py` & `skillpacks-0.1.9/skillpacks/server/routes/action.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/server/routes/episode.py` & `skillpacks-0.1.9/skillpacks/server/routes/episode.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/skillpacks/task_old.py` & `skillpacks-0.1.9/skillpacks/task_old.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.8/PKG-INFO` & `skillpacks-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: skillpacks
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pluggable skills for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: mllm (>=0.1.8,<0.2.0)
+Requires-Dist: mllm (>=0.1.10,<0.2.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
 Description-Content-Type: text/markdown
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: skillpacks Version: 0.1.8 Summary: Pluggable skills
+Metadata-Version: 2.1 Name: skillpacks Version: 0.1.9 Summary: Pluggable skills
 for AI agents License: Apache 2.0 Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: mllm (>=0.1.8,<0.2.0) Requires-Dist:
+Language :: Python :: 3.11 Requires-Dist: mllm (>=0.1.10,<0.2.0) Requires-Dist:
 pydantic (>=2.6.1,<3.0.0) Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
 Description-Content-Type: text/markdown
                            ************ SSkkiillllPPaacckkss ************
                       Pluggable skillsets for AI agents
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
```

