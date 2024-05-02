# Comparing `tmp/pulumiverse_doppler-0.5.0.tar.gz` & `tmp/pulumiverse_doppler-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_doppler-0.5.0.tar", last modified: Wed May  1 20:34:42 2024, max compression
+gzip compressed data, was "pulumiverse_doppler-0.6.0.tar", last modified: Thu May  2 08:08:33 2024, max compression
```

## Comparing `pulumiverse_doppler-0.5.0.tar` & `pulumiverse_doppler-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.666921 pulumiverse_doppler-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 20:34:42.666921 pulumiverse_doppler-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.662921 pulumiverse_doppler-0.5.0/pulumiverse_doppler/
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/branch_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.662921 pulumiverse_doppler-0.5.0/pulumiverse_doppler/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/get_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.662921 pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/aws_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/terraform_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.662921 pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.666921 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/aws_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/terraform_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/service_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.662921 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:34:42.666921 pulumiverse_doppler-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:08:33.106338 pulumiverse_doppler-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-02 08:08:33.106338 pulumiverse_doppler-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:08:33.102338 pulumiverse_doppler-0.6.0/pulumiverse_doppler/
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/branch_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:08:33.102338 pulumiverse_doppler-0.6.0/pulumiverse_doppler/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/get_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/group_member.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:08:33.102338 pulumiverse_doppler-0.6.0/pulumiverse_doppler/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/integration/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/integration/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/integration/terraform_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:08:33.106338 pulumiverse_doppler-0.6.0/pulumiverse_doppler/projectmember/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/projectmember/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/projectmember/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/projectmember/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:08:33.106338 pulumiverse_doppler-0.6.0/pulumiverse_doppler/secretssync/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/secretssync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/secretssync/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/secretssync/terraform_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler/service_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:08:33.102338 pulumiverse_doppler-0.6.0/pulumiverse_doppler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-02 08:08:33.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-02 08:08:33.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:08:33.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:08:33.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 08:08:33.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 08:08:33.000000 pulumiverse_doppler-0.6.0/pulumiverse_doppler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:08:33.106338 pulumiverse_doppler-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-02 08:08:32.000000 pulumiverse_doppler-0.6.0/setup.py
```

### Comparing `pulumiverse_doppler-0.5.0/PKG-INFO` & `pulumiverse_doppler-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_doppler
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.5.0/README.md` & `pulumiverse_doppler-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/__init__.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .branch_config import *
 from .environment import *
 from .get_secrets import *
+from .get_user import *
 from .group import *
+from .group_member import *
 from .project import *
 from .provider import *
 from .secret import *
 from .service_account import *
 from .service_token import *
 
 # Make subpackages available:
@@ -56,14 +58,22 @@
   "fqn": "pulumiverse_doppler",
   "classes": {
    "doppler:index/group:Group": "Group"
   }
  },
  {
   "pkg": "doppler",
+  "mod": "index/groupMember",
+  "fqn": "pulumiverse_doppler",
+  "classes": {
+   "doppler:index/groupMember:GroupMember": "GroupMember"
+  }
+ },
+ {
+  "pkg": "doppler",
   "mod": "index/project",
   "fqn": "pulumiverse_doppler",
   "classes": {
    "doppler:index/project:Project": "Project"
   }
  },
  {
```

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/_utilities.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/branch_config.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/branch_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/config/vars.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/environment.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/environment.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/get_secrets.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/get_secrets.py`

 * *Files 14% similar despite different names*

```diff
@@ -80,16 +80,15 @@
             project=self.project)
 
 
 def get_secrets(config: Optional[str] = None,
                 project: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSecretsResult:
     """
-    Retrieve all secrets in the config.
-
+    Use this data source to access information about an existing resource.
 
     :param str config: The name of the Doppler config (required for personal tokens)
     :param str project: The name of the Doppler project (required for personal tokens)
     """
     __args__ = dict()
     __args__['config'] = config
     __args__['project'] = project
@@ -104,14 +103,13 @@
 
 
 @_utilities.lift_output_func(get_secrets)
 def get_secrets_output(config: Optional[pulumi.Input[Optional[str]]] = None,
                        project: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSecretsResult]:
     """
-    Retrieve all secrets in the config.
-
+    Use this data source to access information about an existing resource.
 
     :param str config: The name of the Doppler config (required for personal tokens)
     :param str project: The name of the Doppler project (required for personal tokens)
     """
     ...
```

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/group.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/aws_parameter_store.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/integration/aws_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/aws_secrets_manager.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/integration/aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/terraform_cloud.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/integration/terraform_cloud.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/project.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/group.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/projectmember/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/service_account.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/projectmember/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/provider.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/secret.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/secret.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/aws_parameter_store.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/secretssync/aws_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/terraform_cloud.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/secretssync/terraform_cloud.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/service_account.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler/service_token.py` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler/service_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/PKG-INFO` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-doppler
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/SOURCES.txt` & `pulumiverse_doppler-0.6.0/pulumiverse_doppler.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 README.md
 setup.py
 pulumiverse_doppler/__init__.py
 pulumiverse_doppler/_utilities.py
 pulumiverse_doppler/branch_config.py
 pulumiverse_doppler/environment.py
 pulumiverse_doppler/get_secrets.py
+pulumiverse_doppler/get_user.py
 pulumiverse_doppler/group.py
+pulumiverse_doppler/group_member.py
 pulumiverse_doppler/project.py
 pulumiverse_doppler/provider.py
 pulumiverse_doppler/pulumi-plugin.json
 pulumiverse_doppler/py.typed
 pulumiverse_doppler/secret.py
 pulumiverse_doppler/service_account.py
 pulumiverse_doppler/service_token.py
```

### Comparing `pulumiverse_doppler-0.5.0/setup.py` & `pulumiverse_doppler-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.5.0"
+VERSION = "0.6.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "doppler Pulumi Package - Development Version"
```

