# Comparing `tmp/agentdesk-0.2.8.tar.gz` & `tmp/agentdesk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentdesk-0.2.8.tar", max compression
+gzip compressed data, was "agentdesk-0.2.9.tar", max compression
```

## Comparing `agentdesk-0.2.8.tar` & `agentdesk-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11357 2024-01-08 22:45:37.309736 agentdesk-0.2.8/LICENSE
--rw-r--r--   0        0        0     3026 2024-02-26 21:41:53.951319 agentdesk-0.2.8/README.md
--rw-r--r--   0        0        0       49 2024-02-21 20:55:04.924191 agentdesk-0.2.8/agentdesk/__init__.py
--rw-r--r--   0        0        0     7094 2024-02-14 04:00:04.398474 agentdesk-0.2.8/agentdesk/cli/main.py
--rw-r--r--   0        0        0     1866 2024-01-31 16:53:44.642711 agentdesk-0.2.8/agentdesk/db/conn.py
--rw-r--r--   0        0        0     1075 2024-02-10 17:59:13.694187 agentdesk-0.2.8/agentdesk/db/models.py
--rw-r--r--   0        0        0       32 2024-02-16 20:22:08.955828 agentdesk-0.2.8/agentdesk/processors/__init__.py
--rw-r--r--   0        0        0      588 2024-02-16 18:30:50.330971 agentdesk-0.2.8/agentdesk/processors/base.py
--rw-r--r--   0        0        0     2302 2024-02-17 04:35:39.829916 agentdesk-0.2.8/agentdesk/processors/grid.py
--rw-r--r--   0        0        0     9825 2024-02-11 00:43:28.862801 agentdesk-0.2.8/agentdesk/proxy.py
--rw-r--r--   0        0        0     1165 2024-02-10 18:30:36.328489 agentdesk-0.2.8/agentdesk/server/models.py
--rw-r--r--   0        0        0     1297 2024-02-01 20:00:04.347080 agentdesk-0.2.8/agentdesk/server/server.py
--rw-r--r--   0        0        0    20241 2024-02-26 21:41:37.275088 agentdesk-0.2.8/agentdesk/tool.py
--rw-r--r--   0        0        0     4949 2024-02-11 00:02:25.072183 agentdesk-0.2.8/agentdesk/util.py
--rw-r--r--   0        0        0      134 2024-01-31 23:16:24.915445 agentdesk-0.2.8/agentdesk/vm/__init__.py
--rw-r--r--   0        0        0    11720 2024-02-12 05:16:51.561490 agentdesk-0.2.8/agentdesk/vm/base.py
--rw-r--r--   0        0        0    15220 2024-02-11 21:41:49.898874 agentdesk-0.2.8/agentdesk/vm/ec2.py
--rw-r--r--   0        0        0    12805 2024-02-16 18:12:02.591435 agentdesk-0.2.8/agentdesk/vm/gce.py
--rw-r--r--   0        0        0      490 2024-02-16 18:10:25.600966 agentdesk-0.2.8/agentdesk/vm/img.py
--rw-r--r--   0        0        0      578 2024-02-10 16:50:22.116036 agentdesk-0.2.8/agentdesk/vm/load.py
--rw-r--r--   0        0        0     9623 2024-02-14 05:53:59.478961 agentdesk-0.2.8/agentdesk/vm/qemu.py
--rw-r--r--   0        0        0     1163 2024-02-26 21:42:24.696556 agentdesk-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 agentdesk-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-08 22:45:37.309736 agentdesk-0.2.9/LICENSE
+-rw-r--r--   0        0        0     3026 2024-02-26 21:41:53.951319 agentdesk-0.2.9/README.md
+-rw-r--r--   0        0        0       49 2024-02-21 20:55:04.924191 agentdesk-0.2.9/agentdesk/__init__.py
+-rw-r--r--   0        0        0     7094 2024-02-14 04:00:04.398474 agentdesk-0.2.9/agentdesk/cli/main.py
+-rw-r--r--   0        0        0     1866 2024-01-31 16:53:44.642711 agentdesk-0.2.9/agentdesk/db/conn.py
+-rw-r--r--   0        0        0     1075 2024-02-10 17:59:13.694187 agentdesk-0.2.9/agentdesk/db/models.py
+-rw-r--r--   0        0        0       32 2024-02-16 20:22:08.955828 agentdesk-0.2.9/agentdesk/processors/__init__.py
+-rw-r--r--   0        0        0      588 2024-02-16 18:30:50.330971 agentdesk-0.2.9/agentdesk/processors/base.py
+-rw-r--r--   0        0        0     2302 2024-02-17 04:35:39.829916 agentdesk-0.2.9/agentdesk/processors/grid.py
+-rw-r--r--   0        0        0     9825 2024-02-11 00:43:28.862801 agentdesk-0.2.9/agentdesk/proxy.py
+-rw-r--r--   0        0        0     1165 2024-02-10 18:30:36.328489 agentdesk-0.2.9/agentdesk/server/models.py
+-rw-r--r--   0        0        0     1297 2024-02-01 20:00:04.347080 agentdesk-0.2.9/agentdesk/server/server.py
+-rw-r--r--   0        0        0    20511 2024-02-29 04:52:13.540525 agentdesk-0.2.9/agentdesk/tool.py
+-rw-r--r--   0        0        0     4949 2024-02-11 00:02:25.072183 agentdesk-0.2.9/agentdesk/util.py
+-rw-r--r--   0        0        0       76 2024-02-29 04:51:40.258667 agentdesk-0.2.9/agentdesk/vm/__init__.py
+-rw-r--r--   0        0        0    11720 2024-02-12 05:16:51.561490 agentdesk-0.2.9/agentdesk/vm/base.py
+-rw-r--r--   0        0        0    15220 2024-02-11 21:41:49.898874 agentdesk-0.2.9/agentdesk/vm/ec2.py
+-rw-r--r--   0        0        0    12805 2024-02-16 18:12:02.591435 agentdesk-0.2.9/agentdesk/vm/gce.py
+-rw-r--r--   0        0        0      490 2024-02-16 18:10:25.600966 agentdesk-0.2.9/agentdesk/vm/img.py
+-rw-r--r--   0        0        0      578 2024-02-10 16:50:22.116036 agentdesk-0.2.9/agentdesk/vm/load.py
+-rw-r--r--   0        0        0     9623 2024-02-14 05:53:59.478961 agentdesk-0.2.9/agentdesk/vm/qemu.py
+-rw-r--r--   0        0        0     1198 2024-02-29 17:27:54.875647 agentdesk-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4097 1970-01-01 00:00:00.000000 agentdesk-0.2.9/PKG-INFO
```

### Comparing `agentdesk-0.2.8/LICENSE` & `agentdesk-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/README.md` & `agentdesk-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/cli/main.py` & `agentdesk-0.2.9/agentdesk/cli/main.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/db/conn.py` & `agentdesk-0.2.9/agentdesk/db/conn.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/db/models.py` & `agentdesk-0.2.9/agentdesk/db/models.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/processors/base.py` & `agentdesk-0.2.9/agentdesk/processors/base.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/processors/grid.py` & `agentdesk-0.2.9/agentdesk/processors/grid.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/proxy.py` & `agentdesk-0.2.9/agentdesk/proxy.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/server/models.py` & `agentdesk-0.2.9/agentdesk/server/models.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/server/server.py` & `agentdesk-0.2.9/agentdesk/server/server.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/tool.py` & `agentdesk-0.2.9/agentdesk/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,28 @@
 import requests
 
 from PIL import Image
 from google.cloud import storage
 from opentool import Tool, action, observation, Action, Observation
 
 from .vm.base import DesktopVM, DesktopProvider
-from .vm.gce import GCEProvider
-from .vm.ec2 import EC2Provider
+
+try:
+    from .vm.gce import GCEProvider
+except ImportError:
+    print(
+        "GCE provider unavailable, install with `pip install agentdesk[gce] if desired"
+    )
+try:
+    from .vm.ec2 import EC2Provider
+except ImportError:
+    print(
+        "AWS provider unavailable, install with `pip install agentdesk[aws] if desired"
+    )
+
 from .vm.qemu import QemuProvider
 from .util import extract_file_path, extract_gcs_info, generate_random_string
 
 
 class StorageStrategy(Enum):
     GCS = "gcs"
     LOCAL = "local"
```

### Comparing `agentdesk-0.2.8/agentdesk/util.py` & `agentdesk-0.2.9/agentdesk/util.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/vm/base.py` & `agentdesk-0.2.9/agentdesk/vm/base.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/vm/ec2.py` & `agentdesk-0.2.9/agentdesk/vm/ec2.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/vm/gce.py` & `agentdesk-0.2.9/agentdesk/vm/gce.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/vm/load.py` & `agentdesk-0.2.9/agentdesk/vm/load.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/agentdesk/vm/qemu.py` & `agentdesk-0.2.9/agentdesk/vm/qemu.py`

 * *Files identical despite different names*

### Comparing `agentdesk-0.2.8/pyproject.toml` & `agentdesk-0.2.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 [tool.poetry]
 name = "agentdesk"
-version = "0.2.8"
+version = "0.2.9"
 description = "A desktop for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "agentdesk"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<3.12"
 pillow = "^10.2.0"
 requests = "^2.31.0"
 fastapi = {extras = ["all"], version = "^0.109.0"}
 sqlalchemy = "^2.0.25"
 psycopg2-binary = "^2.9.9"
 psutil = "^5.9.8"
-google-cloud-storage = "^2.14.0"
 docker = "^7.0.0"
 pycdlib = "^1.14.0"
 namesgenerator = "^0.3"
 paramiko = "^3.4.0"
 typer = "^0.9.0"
 tabulate = "^0.9.0"
 tqdm = "^4.66.2"
 tenacity = "^8.2.3"
 opentool-ai = "^0.1.7"
 
 
 [tool.poetry.group.gcp.dependencies]
 google-cloud-compute = "^1.15.0"
 google-cloud-container = "^2.38.0"
+google-cloud-storage = "^2.14.0"
 
 
 [tool.poetry.group.aws.dependencies]
 boto3 = "^1.34.28"
 boto3-stubs = {extras = ["ec2"], version = "^1.34.28"}
+mypy-boto3-ec2 = "^1.34.52"
 
 
 [tool.poetry.group.demo.dependencies]
 openai = "^1.12.0"
 
 [tool.poetry.scripts]
 agentdesk = "agentdesk.cli.main:app"
```

### Comparing `agentdesk-0.2.8/PKG-INFO` & `agentdesk-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: agentdesk
-Version: 0.2.8
+Version: 0.2.9
 Summary: A desktop for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: fastapi[all] (>=0.109.0,<0.110.0)
-Requires-Dist: google-cloud-storage (>=2.14.0,<3.0.0)
 Requires-Dist: namesgenerator (>=0.3,<0.4)
 Requires-Dist: opentool-ai (>=0.1.7,<0.2.0)
 Requires-Dist: paramiko (>=3.4.0,<4.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: pycdlib (>=1.14.0,<2.0.0)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: agentdesk Version: 0.2.8 Summary: A desktop for AI
+Metadata-Version: 2.1 Name: agentdesk Version: 0.2.9 Summary: A desktop for AI
 agents License: Apache 2.0 Author: Patrick Barker Author-email:
-patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
+patrickbarkerco@gmail.com Requires-Python: >=3.10,<3.12 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: docker (>=7.0.0,<8.0.0) Requires-
-Dist: fastapi[all] (>=0.109.0,<0.110.0) Requires-Dist: google-cloud-storage
-(>=2.14.0,<3.0.0) Requires-Dist: namesgenerator (>=0.3,<0.4) Requires-Dist:
-opentool-ai (>=0.1.7,<0.2.0) Requires-Dist: paramiko (>=3.4.0,<4.0.0) Requires-
-Dist: pillow (>=10.2.0,<11.0.0) Requires-Dist: psutil (>=5.9.8,<6.0.0)
-Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) Requires-Dist: pycdlib
-(>=1.14.0,<2.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
-sqlalchemy (>=2.0.25,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: tenacity (>=8.2.3,<9.0.0) Requires-Dist: tqdm (>=4.66.2,<5.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0) Description-Content-Type: text/markdown
+Dist: fastapi[all] (>=0.109.0,<0.110.0) Requires-Dist: namesgenerator
+(>=0.3,<0.4) Requires-Dist: opentool-ai (>=0.1.7,<0.2.0) Requires-Dist:
+paramiko (>=3.4.0,<4.0.0) Requires-Dist: pillow (>=10.2.0,<11.0.0) Requires-
+Dist: psutil (>=5.9.8,<6.0.0) Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
+Requires-Dist: pycdlib (>=1.14.0,<2.0.0) Requires-Dist: requests
+(>=2.31.0,<3.0.0) Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0) Requires-Dist:
+tabulate (>=0.9.0,<0.10.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0) Requires-
+Dist: tqdm (>=4.66.2,<5.0.0) Requires-Dist: typer (>=0.9.0,<0.10.0)
+Description-Content-Type: text/markdown
                             ************ AAggeennttDDeesskk ************
                      Desktops for AI agents   :computer:
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
 Agentdesk provides full featured desktop environments which can be
```

