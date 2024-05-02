# Comparing `tmp/datatrail_cli-0.5.4.tar.gz` & `tmp/datatrail_cli-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.5.4.tar", max compression
+gzip compressed data, was "datatrail_cli-0.5.5.tar", max compression
```

## Comparing `datatrail_cli-0.5.4.tar` & `datatrail_cli-0.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1080 2024-04-24 20:06:06.301454 datatrail_cli-0.5.4/LICENSE
--rw-r--r--   0        0        0     3558 2024-04-24 20:06:06.301454 datatrail_cli-0.5.4/README.md
--rw-r--r--   0        0        0      214 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/__init__.py
--rw-r--r--   0        0        0     4590 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/clear.py
--rw-r--r--   0        0        0     1437 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/cli.py
--rw-r--r--   0        0        0     4037 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/config.py
--rw-r--r--   0        0        0     1062 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/config.yaml
--rw-r--r--   0        0        0     3924 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/ls.py
--rw-r--r--   0        0        0     7992 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/ps.py
--rw-r--r--   0        0        0     4576 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/pull.py
--rw-r--r--   0        0        0    15932 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/src/functions.py
--rw-r--r--   0        0        0     9241 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/utilities/cadcclient.py
--rw-r--r--   0        0        0     3089 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/dtcli/utilities/utilities.py
--rw-r--r--   0        0        0     1073 2024-04-24 20:06:06.313454 datatrail_cli-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 datatrail_cli-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-02 00:08:23.777665 datatrail_cli-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3558 2024-05-02 00:08:23.777665 datatrail_cli-0.5.5/README.md
+-rw-r--r--   0        0        0      214 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/__init__.py
+-rw-r--r--   0        0        0     4590 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/clear.py
+-rw-r--r--   0        0        0     1437 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/cli.py
+-rw-r--r--   0        0        0     4037 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/config.yaml
+-rw-r--r--   0        0        0     3924 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/ls.py
+-rw-r--r--   0        0        0     7990 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/ps.py
+-rw-r--r--   0        0        0     4576 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/pull.py
+-rw-r--r--   0        0        0    15932 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/src/functions.py
+-rw-r--r--   0        0        0     9241 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     3089 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1073 2024-05-02 00:08:23.785664 datatrail_cli-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 datatrail_cli-0.5.5/PKG-INFO
```

### Comparing `datatrail_cli-0.5.4/LICENSE` & `datatrail_cli-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/README.md` & `datatrail_cli-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/dtcli/clear.py` & `datatrail_cli-0.5.5/dtcli/clear.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/dtcli/cli.py` & `datatrail_cli-0.5.5/dtcli/cli.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/dtcli/config.py` & `datatrail_cli-0.5.5/dtcli/config.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/dtcli/config.yaml` & `datatrail_cli-0.5.5/dtcli/config.yaml`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/dtcli/ls.py` & `datatrail_cli-0.5.5/dtcli/ls.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/dtcli/ps.py` & `datatrail_cli-0.5.5/dtcli/ps.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         footer_style="bold red",
     )
     if len(policies["belongs_to"]) > 1:
         belongs_to = ", ".join([lgr_ds["name"] for lgr_ds in policies["belongs_to"]])
     elif len(policies["belongs_to"]) == 1:
         belongs_to = policies["belongs_to"][0]["name"]
     else:
-        belongs_to = None
+        belongs_to = ""
     policy_table.add_column("Policy", style="bold", footer="Belongs to")
     policy_table.add_column("Storage Element", footer=belongs_to)
     policy_table.add_column("Priority")
     policy_table.add_column("Default")
     policy_table.add_column(r"Delete After \[days]")
 
     rp = policies["replication_policy"]
```

### Comparing `datatrail_cli-0.5.4/dtcli/pull.py` & `datatrail_cli-0.5.5/dtcli/pull.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/dtcli/src/functions.py` & `datatrail_cli-0.5.5/dtcli/src/functions.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/dtcli/utilities/cadcclient.py` & `datatrail_cli-0.5.5/dtcli/utilities/cadcclient.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/dtcli/utilities/utilities.py` & `datatrail_cli-0.5.5/dtcli/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.4/pyproject.toml` & `datatrail_cli-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datatrail-cli"
-version = "0.5.4"
+version = "0.5.5"
 description = "CHIME/FRB Datatrail CLI"
 authors = ["CHIME FRB Project Office"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dtcli" }]
 
 [tool.poetry.dependencies]
```

### Comparing `datatrail_cli-0.5.4/PKG-INFO` & `datatrail_cli-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrail-cli
-Version: 0.5.4
+Version: 0.5.5
 Summary: CHIME/FRB Datatrail CLI
 License: MIT
 Author: CHIME FRB Project Office
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datatrail-cli Version: 0.5.4 Summary: CHIME/FRB
+Metadata-Version: 2.1 Name: datatrail-cli Version: 0.5.5 Summary: CHIME/FRB
 Datatrail CLI License: MIT Author: CHIME FRB Project Office Requires-Python:
 >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: cadcdata (>=2.5.0,<3.0.0) Requires-Dist: cadctap
 (>=0.9.11,<0.10.0) Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0) Requires-Dist:
```

