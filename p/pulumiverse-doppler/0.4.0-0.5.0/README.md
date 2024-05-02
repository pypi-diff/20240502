# Comparing `tmp/pulumiverse_doppler-0.4.0.tar.gz` & `tmp/pulumiverse_doppler-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_doppler-0.4.0.tar", last modified: Wed May  1 18:57:22 2024, max compression
+gzip compressed data, was "pulumiverse_doppler-0.5.0.tar", last modified: Wed May  1 20:34:42 2024, max compression
```

## Comparing `pulumiverse_doppler-0.4.0.tar` & `pulumiverse_doppler-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.898080 pulumiverse_doppler-0.4.0/pulumiverse_doppler/
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/branch_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/pulumiverse_doppler/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/get_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/aws_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/aws_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler/service_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:57:22.902080 pulumiverse_doppler-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-01 18:57:22.000000 pulumiverse_doppler-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.666921 pulumiverse_doppler-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 20:34:42.666921 pulumiverse_doppler-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.662921 pulumiverse_doppler-0.5.0/pulumiverse_doppler/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/branch_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.662921 pulumiverse_doppler-0.5.0/pulumiverse_doppler/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/get_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.662921 pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/terraform_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.662921 pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.666921 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/terraform_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler/service_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:34:42.662921 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:34:42.666921 pulumiverse_doppler-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-01 20:34:42.000000 pulumiverse_doppler-0.5.0/setup.py
```

### Comparing `pulumiverse_doppler-0.4.0/PKG-INFO` & `pulumiverse_doppler-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_doppler
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.4.0/README.md` & `pulumiverse_doppler-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/__init__.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -104,14 +104,22 @@
   "fqn": "pulumiverse_doppler.integration",
   "classes": {
    "doppler:integration/awsSecretsManager:AwsSecretsManager": "AwsSecretsManager"
   }
  },
  {
   "pkg": "doppler",
+  "mod": "integration/terraformCloud",
+  "fqn": "pulumiverse_doppler.integration",
+  "classes": {
+   "doppler:integration/terraformCloud:TerraformCloud": "TerraformCloud"
+  }
+ },
+ {
+  "pkg": "doppler",
   "mod": "projectMember/group",
   "fqn": "pulumiverse_doppler.projectmember",
   "classes": {
    "doppler:projectMember/group:Group": "Group"
   }
  },
  {
@@ -133,14 +141,22 @@
  {
   "pkg": "doppler",
   "mod": "secretsSync/awsSecretsManager",
   "fqn": "pulumiverse_doppler.secretssync",
   "classes": {
    "doppler:secretsSync/awsSecretsManager:AwsSecretsManager": "AwsSecretsManager"
   }
+ },
+ {
+  "pkg": "doppler",
+  "mod": "secretsSync/terraformCloud",
+  "fqn": "pulumiverse_doppler.secretssync",
+  "classes": {
+   "doppler:secretsSync/terraformCloud:TerraformCloud": "TerraformCloud"
+  }
  }
 ]
 """,
     resource_packages="""
 [
  {
   "pkg": "doppler",
```

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/_utilities.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/branch_config.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/branch_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/environment.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/environment.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/get_secrets.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/get_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/group.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/aws_parameter_store.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/aws_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/integration/aws_secrets_manager.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/integration/aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/project.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/group.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/projectmember/service_account.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/projectmember/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/provider.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,53 +15,53 @@
 class ProviderArgs:
     def __init__(__self__, *,
                  doppler_token: pulumi.Input[str],
                  host: Optional[pulumi.Input[str]] = None,
                  verify_tls: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Provider resource.
-        :param pulumi.Input[str] doppler_token: A Doppler token, either a personal or service token
-        :param pulumi.Input[str] host: The Doppler API host (i.e. https://api.doppler.com)
-        :param pulumi.Input[bool] verify_tls: Whether or not to verify TLS
+        :param pulumi.Input[str] doppler_token: A Doppler token, either a personal or service token. This can also be set via the DOPPLER_TOKEN environment variable.
+        :param pulumi.Input[str] host: The Doppler API host (i.e. https://api.doppler.com). This can also be set via the DOPPLER_API_HOST environment variable.
+        :param pulumi.Input[bool] verify_tls: Whether or not to verify TLS. This can also be set via the DOPPLER_VERIFY_TLS environment variable.
         """
         pulumi.set(__self__, "doppler_token", doppler_token)
         if host is not None:
             pulumi.set(__self__, "host", host)
         if verify_tls is not None:
             pulumi.set(__self__, "verify_tls", verify_tls)
 
     @property
     @pulumi.getter(name="dopplerToken")
     def doppler_token(self) -> pulumi.Input[str]:
         """
-        A Doppler token, either a personal or service token
+        A Doppler token, either a personal or service token. This can also be set via the DOPPLER_TOKEN environment variable.
         """
         return pulumi.get(self, "doppler_token")
 
     @doppler_token.setter
     def doppler_token(self, value: pulumi.Input[str]):
         pulumi.set(self, "doppler_token", value)
 
     @property
     @pulumi.getter
     def host(self) -> Optional[pulumi.Input[str]]:
         """
-        The Doppler API host (i.e. https://api.doppler.com)
+        The Doppler API host (i.e. https://api.doppler.com). This can also be set via the DOPPLER_API_HOST environment variable.
         """
         return pulumi.get(self, "host")
 
     @host.setter
     def host(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "host", value)
 
     @property
     @pulumi.getter(name="verifyTls")
     def verify_tls(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether or not to verify TLS
+        Whether or not to verify TLS. This can also be set via the DOPPLER_VERIFY_TLS environment variable.
         """
         return pulumi.get(self, "verify_tls")
 
     @verify_tls.setter
     def verify_tls(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "verify_tls", value)
 
@@ -79,17 +79,17 @@
         The provider type for the doppler package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] doppler_token: A Doppler token, either a personal or service token
-        :param pulumi.Input[str] host: The Doppler API host (i.e. https://api.doppler.com)
-        :param pulumi.Input[bool] verify_tls: Whether or not to verify TLS
+        :param pulumi.Input[str] doppler_token: A Doppler token, either a personal or service token. This can also be set via the DOPPLER_TOKEN environment variable.
+        :param pulumi.Input[str] host: The Doppler API host (i.e. https://api.doppler.com). This can also be set via the DOPPLER_API_HOST environment variable.
+        :param pulumi.Input[bool] verify_tls: Whether or not to verify TLS. This can also be set via the DOPPLER_VERIFY_TLS environment variable.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProviderArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -137,19 +137,19 @@
             __props__,
             opts)
 
     @property
     @pulumi.getter(name="dopplerToken")
     def doppler_token(self) -> pulumi.Output[str]:
         """
-        A Doppler token, either a personal or service token
+        A Doppler token, either a personal or service token. This can also be set via the DOPPLER_TOKEN environment variable.
         """
         return pulumi.get(self, "doppler_token")
 
     @property
     @pulumi.getter
     def host(self) -> pulumi.Output[Optional[str]]:
         """
-        The Doppler API host (i.e. https://api.doppler.com)
+        The Doppler API host (i.e. https://api.doppler.com). This can also be set via the DOPPLER_API_HOST environment variable.
         """
         return pulumi.get(self, "host")
```

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/secret.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/secret.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/aws_parameter_store.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/aws_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/service_account.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler/service_token.py` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler/service_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/PKG-INFO` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-doppler
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.4.0/pulumiverse_doppler.egg-info/SOURCES.txt` & `pulumiverse_doppler-0.5.0/pulumiverse_doppler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,13 +20,15 @@
 pulumiverse_doppler.egg-info/requires.txt
 pulumiverse_doppler.egg-info/top_level.txt
 pulumiverse_doppler/config/__init__.py
 pulumiverse_doppler/config/vars.py
 pulumiverse_doppler/integration/__init__.py
 pulumiverse_doppler/integration/aws_parameter_store.py
 pulumiverse_doppler/integration/aws_secrets_manager.py
+pulumiverse_doppler/integration/terraform_cloud.py
 pulumiverse_doppler/projectmember/__init__.py
 pulumiverse_doppler/projectmember/group.py
 pulumiverse_doppler/projectmember/service_account.py
 pulumiverse_doppler/secretssync/__init__.py
 pulumiverse_doppler/secretssync/aws_parameter_store.py
-pulumiverse_doppler/secretssync/aws_secrets_manager.py
+pulumiverse_doppler/secretssync/aws_secrets_manager.py
+pulumiverse_doppler/secretssync/terraform_cloud.py
```

### Comparing `pulumiverse_doppler-0.4.0/setup.py` & `pulumiverse_doppler-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.0"
+VERSION = "0.5.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "doppler Pulumi Package - Development Version"
```

