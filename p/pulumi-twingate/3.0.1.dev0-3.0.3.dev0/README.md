# Comparing `tmp/pulumi_twingate-3.0.1.dev0.tar.gz` & `tmp/pulumi_twingate-3.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_twingate-3.0.1.dev0.tar", last modified: Fri Apr 19 17:02:00 2024, max compression
+gzip compressed data, was "pulumi_twingate-3.0.3.dev0.tar", last modified: Thu May  2 20:16:17 2024, max compression
```

## Comparing `pulumi_twingate-3.0.1.dev0.tar` & `pulumi_twingate-3.0.3.dev0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:00.908081 pulumi_twingate-3.0.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-19 17:02:00.908081 pulumi_twingate-3.0.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:00.908081 pulumi_twingate-3.0.1.dev0/pulumi_twingate/
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:00.908081 pulumi_twingate-3.0.1.dev0/pulumi_twingate/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_remote_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_security_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    27091 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_connector_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_service_account_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:02:00.908081 pulumi_twingate-3.0.1.dev0/pulumi_twingate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/pulumi_twingate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:02:00.908081 pulumi_twingate-3.0.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-19 17:02:00.000000 pulumi_twingate-3.0.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/pulumi_twingate/
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/pulumi_twingate/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_remote_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_security_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21219 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27880 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12361 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_connector_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14760 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34418 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_service_account_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17041 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/setup.py
```

### Comparing `pulumi_twingate-3.0.1.dev0/PKG-INFO` & `pulumi_twingate-3.0.3.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_twingate
-Version: 3.0.1.dev0
+Version: 3.0.3.dev0
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.twingate.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Twingate/pulumi-twingate
 Keywords: pulumi twingate category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_twingate-3.0.1.dev0/README.md` & `pulumi_twingate-3.0.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/__init__.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/_inputs.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/_inputs.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,23 +20,27 @@
     'GetTwingateResourceProtocolsUdpArgs',
 ]
 
 @pulumi.input_type
 class TwingateResourceAccessGroupArgs:
     def __init__(__self__, *,
                  group_id: Optional[pulumi.Input[str]] = None,
-                 security_policy_id: Optional[pulumi.Input[str]] = None):
+                 security_policy_id: Optional[pulumi.Input[str]] = None,
+                 usage_based_autolock_duration_days: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[str] group_id: Group ID that will have permission to access the Resource.
         :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
+        :param pulumi.Input[int] usage_based_autolock_duration_days: The usage-based auto-lock duration configured on the edge (in days).
         """
         if group_id is not None:
             pulumi.set(__self__, "group_id", group_id)
         if security_policy_id is not None:
             pulumi.set(__self__, "security_policy_id", security_policy_id)
+        if usage_based_autolock_duration_days is not None:
+            pulumi.set(__self__, "usage_based_autolock_duration_days", usage_based_autolock_duration_days)
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> Optional[pulumi.Input[str]]:
         """
         Group ID that will have permission to access the Resource.
         """
@@ -54,14 +58,26 @@
         """
         return pulumi.get(self, "security_policy_id")
 
     @security_policy_id.setter
     def security_policy_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_policy_id", value)
 
+    @property
+    @pulumi.getter(name="usageBasedAutolockDurationDays")
+    def usage_based_autolock_duration_days(self) -> Optional[pulumi.Input[int]]:
+        """
+        The usage-based auto-lock duration configured on the edge (in days).
+        """
+        return pulumi.get(self, "usage_based_autolock_duration_days")
+
+    @usage_based_autolock_duration_days.setter
+    def usage_based_autolock_duration_days(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "usage_based_autolock_duration_days", value)
+
 
 @pulumi.input_type
 class TwingateResourceAccessServiceArgs:
     def __init__(__self__, *,
                  service_account_id: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] service_account_id: The ID of the service account that should have access to this Resource.
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/_utilities.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/config/vars.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_connector.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,22 +83,20 @@
 def get_twingate_connector(id: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateConnectorResult:
     """
     Connectors provide connectivity to Remote Networks. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/understanding-access-nodes).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_connector(id="<your connector's id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Connector. The ID for the Connector can be obtained from the Admin API or the URL string in the Admin Console.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -115,20 +113,18 @@
 def get_twingate_connector_output(id: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateConnectorResult]:
     """
     Connectors provide connectivity to Remote Networks. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/understanding-access-nodes).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_connector(id="<your connector's id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Connector. The ID for the Connector can be obtained from the Admin API or the URL string in the Admin Console.
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_connectors.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_connectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,25 +137,23 @@
                             name_suffix: Optional[str] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateConnectorsResult:
     """
     Connectors provide connectivity to Remote Networks. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/understanding-access-nodes).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     all = twingate.get_twingate_connectors(name="<your connector's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str name: The Name of the Connector.
+    :param str name: Returns only connectors that exactly match this name. If no options are passed it will return all connectors. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the connector.
     :param str name_exclude: Match when the exact value does not exist in the name of the connector.
     :param str name_prefix: The name of the connector must start with the value.
     :param str name_regexp: The regular expression match of the name of the connector.
     :param str name_suffix: The name of the connector must end with the value.
     """
     __args__ = dict()
@@ -188,25 +186,23 @@
                                    name_suffix: Optional[pulumi.Input[Optional[str]]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateConnectorsResult]:
     """
     Connectors provide connectivity to Remote Networks. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/understanding-access-nodes).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     all = twingate.get_twingate_connectors(name="<your connector's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str name: The Name of the Connector.
+    :param str name: Returns only connectors that exactly match this name. If no options are passed it will return all connectors. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the connector.
     :param str name_exclude: Match when the exact value does not exist in the name of the connector.
     :param str name_prefix: The name of the connector must start with the value.
     :param str name_regexp: The regular expression match of the name of the connector.
     :param str name_suffix: The name of the connector must end with the value.
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_group.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,22 +95,20 @@
 def get_twingate_group(id: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateGroupResult:
     """
     Groups are how users are authorized to access Resources. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/groups).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_group(id="<your group's id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Group. The ID for the Group can be obtained from the Admin API or the URL string in the Admin Console.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -128,20 +126,18 @@
 def get_twingate_group_output(id: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateGroupResult]:
     """
     Groups are how users are authorized to access Resources. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/groups).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_group(id="<your group's id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Group. The ID for the Group can be obtained from the Admin API or the URL string in the Admin Console.
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_groups.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,26 +163,24 @@
                         types: Optional[Sequence[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateGroupsResult:
     """
     Groups are how users are authorized to access Resources. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/groups).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_groups(name="<your group's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param bool is_active: Indicates if the Group is active
-    :param str name: The name of the Group
+    :param bool is_active: Returns only Groups matching the specified state.
+    :param str name: Returns only groups that exactly match this name. If no options are passed it will return all resources. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the group.
     :param str name_exclude: Match when the exact value does not exist in the name of the group.
     :param str name_prefix: The name of the group must start with the value.
     :param str name_regexp: The regular expression match of the name of the group.
     :param str name_suffix: The name of the group must end with the value.
     :param Sequence[str] types: Returns groups that match a list of types. valid types: `MANUAL`, `SYNCED`, `SYSTEM`.
     """
@@ -222,26 +220,24 @@
                                types: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateGroupsResult]:
     """
     Groups are how users are authorized to access Resources. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/groups).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_groups(name="<your group's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param bool is_active: Indicates if the Group is active
-    :param str name: The name of the Group
+    :param bool is_active: Returns only Groups matching the specified state.
+    :param str name: Returns only groups that exactly match this name. If no options are passed it will return all resources. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the group.
     :param str name_exclude: Match when the exact value does not exist in the name of the group.
     :param str name_prefix: The name of the group must start with the value.
     :param str name_regexp: The regular expression match of the name of the group.
     :param str name_suffix: The name of the group must end with the value.
     :param Sequence[str] types: Returns groups that match a list of types. valid types: `MANUAL`, `SYNCED`, `SYSTEM`.
     """
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_remote_network.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_remote_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,22 +72,20 @@
                                 name: Optional[str] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateRemoteNetworkResult:
     """
     A Remote Network represents a single private network in Twingate that can have one or more Connectors and Resources assigned to it. You must create a Remote Network before creating Resources and Connectors that belong to it. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/remote-networks).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_remote_network(name="<your network's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Remote Network
     :param str name: The name of the Remote Network
     """
     __args__ = dict()
     __args__['id'] = id
@@ -106,21 +104,19 @@
                                        name: Optional[pulumi.Input[Optional[str]]] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateRemoteNetworkResult]:
     """
     A Remote Network represents a single private network in Twingate that can have one or more Connectors and Resources assigned to it. You must create a Remote Network before creating Resources and Connectors that belong to it. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/remote-networks).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_remote_network(name="<your network's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Remote Network
     :param str name: The name of the Remote Network
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_remote_networks.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_remote_networks.py`

 * *Files 18% similar despite different names*

```diff
@@ -137,25 +137,23 @@
                                  name_suffix: Optional[str] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateRemoteNetworksResult:
     """
     A Remote Network represents a single private network in Twingate that can have one or more Connectors and Resources assigned to it. You must create a Remote Network before creating Resources and Connectors that belong to it. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/remote-networks).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     all = twingate.get_twingate_remote_networks(name="<your network's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str name: The name of the Remote Network.
+    :param str name: Returns only remote networks that exactly match this name. If no options are passed it will return all remote networks. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the remote network.
     :param str name_exclude: Match when the exact value does not exist in the name of the remote network.
     :param str name_prefix: The name of the remote network must start with the value.
     :param str name_regexp: The regular expression match of the name of the remote network.
     :param str name_suffix: The name of the remote network must end with the value.
     """
     __args__ = dict()
@@ -188,25 +186,23 @@
                                         name_suffix: Optional[pulumi.Input[Optional[str]]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateRemoteNetworksResult]:
     """
     A Remote Network represents a single private network in Twingate that can have one or more Connectors and Resources assigned to it. You must create a Remote Network before creating Resources and Connectors that belong to it. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/remote-networks).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     all = twingate.get_twingate_remote_networks(name="<your network's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str name: The name of the Remote Network.
+    :param str name: Returns only remote networks that exactly match this name. If no options are passed it will return all remote networks. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the remote network.
     :param str name_exclude: Match when the exact value does not exist in the name of the remote network.
     :param str name_prefix: The name of the remote network must start with the value.
     :param str name_regexp: The regular expression match of the name of the remote network.
     :param str name_suffix: The name of the remote network must end with the value.
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_resource.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,22 +98,20 @@
                           protocols: Optional[pulumi.InputType['GetTwingateResourceProtocolsArgs']] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateResourceResult:
     """
     Resources in Twingate represent any network destination address that you wish to provide private access to for users authorized via the Twingate Client application. Resources can be defined by either IP or DNS address, and all private DNS addresses will be automatically resolved with no client configuration changes. For more information, see the Twingate [documentation](https://docs.twingate.com/docs/resources-and-access-nodes).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_resource(id="<your resource's id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Resource. The ID for the Resource can be obtained from the Admin API or the URL string in the Admin Console.
     :param pulumi.InputType['GetTwingateResourceProtocolsArgs'] protocols: By default (when this argument is not defined) no restriction is applied, and all protocols and ports are allowed.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -134,21 +132,19 @@
                                  protocols: Optional[pulumi.Input[Optional[pulumi.InputType['GetTwingateResourceProtocolsArgs']]]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateResourceResult]:
     """
     Resources in Twingate represent any network destination address that you wish to provide private access to for users authorized via the Twingate Client application. Resources can be defined by either IP or DNS address, and all private DNS addresses will be automatically resolved with no client configuration changes. For more information, see the Twingate [documentation](https://docs.twingate.com/docs/resources-and-access-nodes).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_resource(id="<your resource's id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Resource. The ID for the Resource can be obtained from the Admin API or the URL string in the Admin Console.
     :param pulumi.InputType['GetTwingateResourceProtocolsArgs'] protocols: By default (when this argument is not defined) no restriction is applied, and all protocols and ports are allowed.
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_resources.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,25 +137,23 @@
                            name_suffix: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateResourcesResult:
     """
     Resources in Twingate represent servers on the private network that clients can connect to. Resources can be defined by IP, CIDR range, FQDN, or DNS zone. For more information, see the Twingate [documentation](https://docs.twingate.com/docs/resources-and-access-nodes).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_resources(name="<your resource's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str name: The name of the Resource
+    :param str name: Returns only resources that exactly match this name. If no options are passed it will return all resources. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the resource.
     :param str name_exclude: Match when the exact value does not exist in the name of the resource.
     :param str name_prefix: The name of the resource must start with the value.
     :param str name_regexp: The regular expression match of the name of the resource.
     :param str name_suffix: The name of the resource must end with the value.
     """
     __args__ = dict()
@@ -188,25 +186,23 @@
                                   name_suffix: Optional[pulumi.Input[Optional[str]]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateResourcesResult]:
     """
     Resources in Twingate represent servers on the private network that clients can connect to. Resources can be defined by IP, CIDR range, FQDN, or DNS zone. For more information, see the Twingate [documentation](https://docs.twingate.com/docs/resources-and-access-nodes).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_resources(name="<your resource's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str name: The name of the Resource
+    :param str name: Returns only resources that exactly match this name. If no options are passed it will return all resources. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the resource.
     :param str name_exclude: Match when the exact value does not exist in the name of the resource.
     :param str name_prefix: The name of the resource must start with the value.
     :param str name_regexp: The regular expression match of the name of the resource.
     :param str name_suffix: The name of the resource must end with the value.
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_security_policies.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_security_policies.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,25 +134,23 @@
                                    name_suffix: Optional[str] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateSecurityPoliciesResult:
     """
     Security Policies are defined in the Twingate Admin Console and determine user and device authentication requirements for Resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     all = twingate.get_twingate_security_policies(name="<your security policy's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str name: Return a Security Policy that exactly matches this name.
+    :param str name: Returns only security policies that exactly match this name. If no options are passed it will return all security policies. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the security policy.
     :param str name_exclude: Match when the exact value does not exist in the name of the security policy.
     :param str name_prefix: The name of the security policy must start with the value.
     :param str name_regexp: The regular expression match of the name of the security policy.
     :param str name_suffix: The name of the security policy must end with the value.
     """
     __args__ = dict()
@@ -185,25 +183,23 @@
                                           name_suffix: Optional[pulumi.Input[Optional[str]]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateSecurityPoliciesResult]:
     """
     Security Policies are defined in the Twingate Admin Console and determine user and device authentication requirements for Resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     all = twingate.get_twingate_security_policies(name="<your security policy's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str name: Return a Security Policy that exactly matches this name.
+    :param str name: Returns only security policies that exactly match this name. If no options are passed it will return all security policies. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the security policy.
     :param str name_exclude: Match when the exact value does not exist in the name of the security policy.
     :param str name_prefix: The name of the security policy must start with the value.
     :param str name_regexp: The regular expression match of the name of the security policy.
     :param str name_suffix: The name of the security policy must end with the value.
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_security_policy.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_security_policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,22 +60,20 @@
                                  name: Optional[str] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateSecurityPolicyResult:
     """
     Security Policies are defined in the Twingate Admin Console and determine user and device authentication requirements for Resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_security_policy(name="<your security policy name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: Return a Security Policy by its ID. The ID for the Security Policy can be obtained from the Admin API or the URL string in the Admin Console.
     :param str name: Return a Security Policy that exactly matches this name.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -93,21 +91,19 @@
                                         name: Optional[pulumi.Input[Optional[str]]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateSecurityPolicyResult]:
     """
     Security Policies are defined in the Twingate Admin Console and determine user and device authentication requirements for Resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_security_policy(name="<your security policy name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: Return a Security Policy by its ID. The ID for the Security Policy can be obtained from the Admin API or the URL string in the Admin Console.
     :param str name: Return a Security Policy that exactly matches this name.
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_service_accounts.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_service_accounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,25 +137,23 @@
                                   name_suffix: Optional[str] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateServiceAccountsResult:
     """
     Service Accounts offer a way to provide programmatic, centrally-controlled, and consistent access controls.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_service_accounts(name="<your service account's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str name: Name of the Service Account
+    :param str name: Returns only service accounts that exactly match this name. If no options are passed it will return all service accounts. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the service account.
     :param str name_exclude: Match when the exact value does not exist in the name of the service account.
     :param str name_prefix: The name of the service account must start with the value.
     :param str name_regexp: The regular expression match of the name of the service account.
     :param str name_suffix: The name of the service account must end with the value.
     """
     __args__ = dict()
@@ -188,25 +186,23 @@
                                          name_suffix: Optional[pulumi.Input[Optional[str]]] = None,
                                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateServiceAccountsResult]:
     """
     Service Accounts offer a way to provide programmatic, centrally-controlled, and consistent access controls.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_service_accounts(name="<your service account's name>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str name: Name of the Service Account
+    :param str name: Returns only service accounts that exactly match this name. If no options are passed it will return all service accounts. Only one option can be used at a time.
     :param str name_contains: Match when the value exist in the name of the service account.
     :param str name_exclude: Match when the exact value does not exist in the name of the service account.
     :param str name_prefix: The name of the service account must start with the value.
     :param str name_regexp: The regular expression match of the name of the service account.
     :param str name_suffix: The name of the service account must end with the value.
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_user.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,22 +107,20 @@
 def get_twingate_user(id: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateUserResult:
     """
     Users in Twingate can be given access to Twingate Resources and may either be added manually or automatically synchronized with a 3rd party identity provider. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/users).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_user(id="<your user's id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the User. The ID for the User can be obtained from the Admin API or the URL string in the Admin Console.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -141,20 +139,18 @@
 def get_twingate_user_output(id: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateUserResult]:
     """
     Users in Twingate can be given access to Twingate Resources and may either be added manually or automatically synchronized with a 3rd party identity provider. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/users).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     foo = twingate.get_twingate_user(id="<your user's id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the User. The ID for the User can be obtained from the Admin API or the URL string in the Admin Console.
     """
     ...
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/get_twingate_users.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_users.py`

 * *Files 3% similar despite different names*

```diff
@@ -303,37 +303,35 @@
                        roles: Optional[Sequence[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTwingateUsersResult:
     """
     Users in Twingate can be given access to Twingate Resources and may either be added manually or automatically synchronized with a 3rd party identity provider. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/users).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     all = twingate.get_twingate_users()
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str email: The email address of the User
+    :param str email: Returns only users that exactly match this email.
     :param str email_contains: Match when the value exist in the email of the user.
     :param str email_exclude: Match when the value does not exist in the email of the user.
     :param str email_prefix: The email of the user must start with the value.
     :param str email_regexp: The regular expression match of the email of the user.
     :param str email_suffix: The email of the user must end with the value.
-    :param str first_name: The first name of the User
+    :param str first_name: Returns only users that exactly match the first name.
     :param str first_name_contains: Match when the value exist in the first name of the user.
     :param str first_name_exclude: Match when the value does not exist in the first name of the user.
     :param str first_name_prefix: The first name of the user must start with the value.
     :param str first_name_regexp: The regular expression match of the first name of the user.
     :param str first_name_suffix: The first name of the user must end with the value.
-    :param str last_name: The last name of the User
+    :param str last_name: Returns only users that exactly match the last name.
     :param str last_name_contains: Match when the value exist in the last name of the user.
     :param str last_name_exclude: Match when the value does not exist in the last name of the user.
     :param str last_name_prefix: The last name of the user must start with the value.
     :param str last_name_regexp: The regular expression match of the last name of the user.
     :param str last_name_suffix: The last name of the user must end with the value.
     :param Sequence[str] roles: Returns users that match a list of roles. Valid roles: `ADMIN`, `DEVOPS`, `SUPPORT`, `MEMBER`.
     """
@@ -406,37 +404,35 @@
                               roles: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTwingateUsersResult]:
     """
     Users in Twingate can be given access to Twingate Resources and may either be added manually or automatically synchronized with a 3rd party identity provider. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/users).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_twingate as twingate
 
     all = twingate.get_twingate_users()
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str email: The email address of the User
+    :param str email: Returns only users that exactly match this email.
     :param str email_contains: Match when the value exist in the email of the user.
     :param str email_exclude: Match when the value does not exist in the email of the user.
     :param str email_prefix: The email of the user must start with the value.
     :param str email_regexp: The regular expression match of the email of the user.
     :param str email_suffix: The email of the user must end with the value.
-    :param str first_name: The first name of the User
+    :param str first_name: Returns only users that exactly match the first name.
     :param str first_name_contains: Match when the value exist in the first name of the user.
     :param str first_name_exclude: Match when the value does not exist in the first name of the user.
     :param str first_name_prefix: The first name of the user must start with the value.
     :param str first_name_regexp: The regular expression match of the first name of the user.
     :param str first_name_suffix: The first name of the user must end with the value.
-    :param str last_name: The last name of the User
+    :param str last_name: Returns only users that exactly match the last name.
     :param str last_name_contains: Match when the value exist in the last name of the user.
     :param str last_name_exclude: Match when the value does not exist in the last name of the user.
     :param str last_name_prefix: The last name of the user must start with the value.
     :param str last_name_regexp: The regular expression match of the last name of the user.
     :param str last_name_suffix: The last name of the user must end with the value.
     :param Sequence[str] roles: Returns users that match a list of roles. Valid roles: `ADMIN`, `DEVOPS`, `SUPPORT`, `MEMBER`.
     """
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/outputs.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/outputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,37 +36,43 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "groupId":
             suggest = "group_id"
         elif key == "securityPolicyId":
             suggest = "security_policy_id"
+        elif key == "usageBasedAutolockDurationDays":
+            suggest = "usage_based_autolock_duration_days"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in TwingateResourceAccessGroup. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         TwingateResourceAccessGroup.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         TwingateResourceAccessGroup.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  group_id: Optional[str] = None,
-                 security_policy_id: Optional[str] = None):
+                 security_policy_id: Optional[str] = None,
+                 usage_based_autolock_duration_days: Optional[int] = None):
         """
         :param str group_id: Group ID that will have permission to access the Resource.
         :param str security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
+        :param int usage_based_autolock_duration_days: The usage-based auto-lock duration configured on the edge (in days).
         """
         if group_id is not None:
             pulumi.set(__self__, "group_id", group_id)
         if security_policy_id is not None:
             pulumi.set(__self__, "security_policy_id", security_policy_id)
+        if usage_based_autolock_duration_days is not None:
+            pulumi.set(__self__, "usage_based_autolock_duration_days", usage_based_autolock_duration_days)
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> Optional[str]:
         """
         Group ID that will have permission to access the Resource.
         """
@@ -76,14 +82,22 @@
     @pulumi.getter(name="securityPolicyId")
     def security_policy_id(self) -> Optional[str]:
         """
         The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
         """
         return pulumi.get(self, "security_policy_id")
 
+    @property
+    @pulumi.getter(name="usageBasedAutolockDurationDays")
+    def usage_based_autolock_duration_days(self) -> Optional[int]:
+        """
+        The usage-based auto-lock duration configured on the edge (in days).
+        """
+        return pulumi.get(self, "usage_based_autolock_duration_days")
+
 
 @pulumi.output_type
 class TwingateResourceAccessService(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "serviceAccountId":
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/provider.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_connector.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,25 +132,23 @@
                  status_updates_enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Connectors provide connectivity to Remote Networks. This resource type will create the Connector in the Twingate Admin Console, but in order to successfully deploy it, you must also generate Connector tokens that authenticate the Connector with Twingate. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/understanding-access-nodes).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         aws_network = twingate.TwingateRemoteNetwork("awsNetwork")
         aws_connector = twingate.TwingateConnector("awsConnector",
             remote_network_id=aws_network.id,
             status_updates_enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ```sh
         $ pulumi import twingate:index/twingateConnector:TwingateConnector aws_connector Q29ubmVjdG9yOjI2NzM=
         ```
 
@@ -167,25 +165,23 @@
                  args: TwingateConnectorArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Connectors provide connectivity to Remote Networks. This resource type will create the Connector in the Twingate Admin Console, but in order to successfully deploy it, you must also generate Connector tokens that authenticate the Connector with Twingate. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/understanding-access-nodes).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         aws_network = twingate.TwingateRemoteNetwork("awsNetwork")
         aws_connector = twingate.TwingateConnector("awsConnector",
             remote_network_id=aws_network.id,
             status_updates_enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ```sh
         $ pulumi import twingate:index/twingateConnector:TwingateConnector aws_connector Q29ubmVjdG9yOjI2NzM=
         ```
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_connector_tokens.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_connector_tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,24 +131,22 @@
                  keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         This resource type will generate tokens for a Connector, which are needed to successfully provision one on your network. The Connector itself has its own resource type and must be created before you can provision tokens.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         aws_network = twingate.TwingateRemoteNetwork("awsNetwork")
         aws_connector = twingate.TwingateConnector("awsConnector", remote_network_id=aws_network.id)
         aws_connector_tokens = twingate.TwingateConnectorTokens("awsConnectorTokens", connector_id=aws_connector.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] connector_id: The ID of the parent Connector
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. Use this to automatically rotate Connector tokens on a schedule.
         """
         ...
@@ -158,24 +156,22 @@
                  args: TwingateConnectorTokensArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource type will generate tokens for a Connector, which are needed to successfully provision one on your network. The Connector itself has its own resource type and must be created before you can provision tokens.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         aws_network = twingate.TwingateRemoteNetwork("awsNetwork")
         aws_connector = twingate.TwingateConnector("awsConnector", remote_network_id=aws_network.id)
         aws_connector_tokens = twingate.TwingateConnectorTokens("awsConnectorTokens", connector_id=aws_connector.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param TwingateConnectorTokensArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_group.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,22 +170,20 @@
                  user_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Groups are how users are authorized to access Resources. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/groups).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         aws = twingate.TwingateGroup("aws")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ```sh
         $ pulumi import twingate:index/twingateGroup:TwingateGroup aws R3JvdXA6MzQ4OTE=
         ```
 
@@ -204,22 +202,20 @@
                  args: Optional[TwingateGroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Groups are how users are authorized to access Resources. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/groups).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         aws = twingate.TwingateGroup("aws")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ```sh
         $ pulumi import twingate:index/twingateGroup:TwingateGroup aws R3JvdXA6MzQ4OTE=
         ```
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_remote_network.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_remote_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,22 +100,20 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         A Remote Network represents a single private network in Twingate that can have one or more Connectors and Resources assigned to it. You must create a Remote Network before creating Resources and Connectors that belong to it. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/remote-networks).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         aws_network = twingate.TwingateRemoteNetwork("awsNetwork")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ```sh
         $ pulumi import twingate:index/twingateRemoteNetwork:TwingateRemoteNetwork network UmVtb3RlTmV0d29zaipgMKIkNg==
         ```
 
@@ -131,22 +129,20 @@
                  args: Optional[TwingateRemoteNetworkArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         A Remote Network represents a single private network in Twingate that can have one or more Connectors and Resources assigned to it. You must create a Remote Network before creating Resources and Connectors that belong to it. For more information, see Twingate's [documentation](https://docs.twingate.com/docs/remote-networks).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         aws_network = twingate.TwingateRemoteNetwork("awsNetwork")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ```sh
         $ pulumi import twingate:index/twingateRemoteNetwork:TwingateRemoteNetwork network UmVtb3RlTmV0d29zaipgMKIkNg==
         ```
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_resource.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         :param pulumi.Input[bool] is_active: Set the resource as active or inactive. Default is `true`.
         :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
                `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input['TwingateResourceProtocolsArgs'] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
-        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
+        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "remote_network_id", remote_network_id)
         if access_groups is not None:
             pulumi.set(__self__, "access_groups", access_groups)
         if access_services is not None:
             pulumi.set(__self__, "access_services", access_services)
@@ -200,15 +200,15 @@
     def protocols(self, value: Optional[pulumi.Input['TwingateResourceProtocolsArgs']]):
         pulumi.set(self, "protocols", value)
 
     @property
     @pulumi.getter(name="securityPolicyId")
     def security_policy_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
+        The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
         return pulumi.get(self, "security_policy_id")
 
     @security_policy_id.setter
     def security_policy_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_policy_id", value)
 
@@ -238,15 +238,15 @@
         :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
                `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input['TwingateResourceProtocolsArgs'] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
-        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
+        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
         if access_groups is not None:
             pulumi.set(__self__, "access_groups", access_groups)
         if access_services is not None:
             pulumi.set(__self__, "access_services", access_services)
         if address is not None:
             pulumi.set(__self__, "address", address)
@@ -402,15 +402,15 @@
     def remote_network_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "remote_network_id", value)
 
     @property
     @pulumi.getter(name="securityPolicyId")
     def security_policy_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
+        The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
         return pulumi.get(self, "security_policy_id")
 
     @security_policy_id.setter
     def security_policy_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_policy_id", value)
 
@@ -452,15 +452,15 @@
         :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
                `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input[pulumi.InputType['TwingateResourceProtocolsArgs']] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
-        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
+        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TwingateResourceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -562,15 +562,15 @@
         :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
                `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input[pulumi.InputType['TwingateResourceProtocolsArgs']] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
-        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
+        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TwingateResourceState.__new__(_TwingateResourceState)
 
         __props__.__dict__["access_groups"] = access_groups
         __props__.__dict__["access_services"] = access_services
@@ -675,11 +675,11 @@
         """
         return pulumi.get(self, "remote_network_id")
 
     @property
     @pulumi.getter(name="securityPolicyId")
     def security_policy_id(self) -> pulumi.Output[str]:
         """
-        The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
+        The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
         return pulumi.get(self, "security_policy_id")
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_service_account.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_service_account.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,22 +67,20 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Service Accounts offer a way to provide programmatic, centrally-controlled, and consistent access controls.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         github_actions_prod = twingate.TwingateServiceAccount("githubActionsProd")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of the Service Account in Twingate
         """
         ...
     @overload
@@ -91,22 +89,20 @@
                  args: Optional[TwingateServiceAccountArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Service Accounts offer a way to provide programmatic, centrally-controlled, and consistent access controls.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         github_actions_prod = twingate.TwingateServiceAccount("githubActionsProd")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param TwingateServiceAccountArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_service_account_key.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_service_account_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,28 +164,26 @@
                  service_account_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         A Service Key authorizes access to all Resources assigned to a Service Account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
         import pulumiverse_time as time
 
         github_actions_prod = twingate.TwingateServiceAccount("githubActionsProd")
         github_key = twingate.TwingateServiceAccountKey("githubKey", service_account_id=github_actions_prod.id)
         # Key rotation using the time provider (see https://registry.terraform.io/providers/hashicorp/time/latest)
         key_rotation_rotating = time.Rotating("keyRotationRotating", rotation_days=30)
         key_rotation_static = time.Static("keyRotationStatic", rfc3339=key_rotation_rotating.rfc3339)
         github_key_with_rotation = twingate.TwingateServiceAccountKey("githubKeyWithRotation", service_account_id=github_actions_prod.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] expiration_time: Specifies how many days until a Service Account Key expires. This should be an integer between 0 and 365 representing the number of days until the Service Account Key will expire. Defaults to 0, meaning the key will never expire.
         :param pulumi.Input[str] name: The name of the Service Key
         :param pulumi.Input[str] service_account_id: The id of the Service Account
         """
@@ -196,28 +194,26 @@
                  args: TwingateServiceAccountKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         A Service Key authorizes access to all Resources assigned to a Service Account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
         import pulumiverse_time as time
 
         github_actions_prod = twingate.TwingateServiceAccount("githubActionsProd")
         github_key = twingate.TwingateServiceAccountKey("githubKey", service_account_id=github_actions_prod.id)
         # Key rotation using the time provider (see https://registry.terraform.io/providers/hashicorp/time/latest)
         key_rotation_rotating = time.Rotating("keyRotationRotating", rotation_days=30)
         key_rotation_static = time.Static("keyRotationStatic", rfc3339=key_rotation_rotating.rfc3339)
         github_key_with_rotation = twingate.TwingateServiceAccountKey("githubKeyWithRotation", service_account_id=github_actions_prod.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param TwingateServiceAccountKeyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate/twingate_user.py` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,27 +247,25 @@
                  send_invite: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Users provides different levels of write capabilities across the Twingate Admin Console. For more information, see Twingate's [documentation](https://www.twingate.com/docs/users).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         user = twingate.TwingateUser("user",
             email="sample@company.com",
             first_name="Twin",
             last_name="Gate",
             role="DEVOPS",
             send_invite=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] email: The User's email address
         :param pulumi.Input[str] first_name: The User's first name
         :param pulumi.Input[bool] is_active: Determines whether the User is active or not. Inactive users will be not able to sign in.
         :param pulumi.Input[str] last_name: The User's last name
@@ -281,27 +279,25 @@
                  args: TwingateUserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Users provides different levels of write capabilities across the Twingate Admin Console. For more information, see Twingate's [documentation](https://www.twingate.com/docs/users).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_twingate as twingate
 
         user = twingate.TwingateUser("user",
             email="sample@company.com",
             first_name="Twin",
             last_name="Gate",
             role="DEVOPS",
             send_invite=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param TwingateUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate.egg-info/PKG-INFO` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-twingate
-Version: 3.0.1.dev0
+Version: 3.0.3.dev0
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.twingate.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Twingate/pulumi-twingate
 Keywords: pulumi twingate category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_twingate-3.0.1.dev0/pulumi_twingate.egg-info/SOURCES.txt` & `pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.1.dev0/setup.py` & `pulumi_twingate-3.0.3.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.0.1dev0"
+VERSION = "3.0.3dev0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "twingate Pulumi Package - Development Version"
```

