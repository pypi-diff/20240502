# Comparing `tmp/mypy_boto3_ec2-1.34.96.tar.gz` & `tmp/mypy_boto3_ec2-1.34.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_ec2-1.34.96.tar", last modified: Wed May  1 19:21:15 2024, max compression
+gzip compressed data, was "mypy_boto3_ec2-1.34.97.tar", last modified: Thu May  2 19:33:15 2024, max compression
```

## Comparing `mypy_boto3_ec2-1.34.96.tar` & `mypy_boto3_ec2-1.34.97.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.804324 mypy_boto3_ec2-1.34.96/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-05-01 19:21:15.800324 mypy_boto3_ec2-1.34.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    48950 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.800324 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/
--rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   544008 2024-05-01 19:20:17.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   544005 2024-05-01 19:20:14.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    96930 2024-05-01 19:20:23.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    96930 2024-05-01 19:20:23.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   187386 2024-05-01 19:20:21.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)   187243 2024-05-01 19:20:20.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   272189 2024-05-01 19:20:20.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)   272111 2024-05-01 19:20:18.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   885369 2024-05-01 19:20:40.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   885369 2024-05-01 19:20:34.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:20:11.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-05-01 19:20:22.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    39737 2024-05-01 19:20:21.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:15.800324 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 19:21:15.000000 mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:21:15.804324 mypy_boto3_ec2-1.34.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-01 19:20:10.000000 mypy_boto3_ec2-1.34.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:15.126121 mypy_boto3_ec2-1.34.97/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 19:32:24.000000 mypy_boto3_ec2-1.34.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-05-02 19:33:15.126121 mypy_boto3_ec2-1.34.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    48950 2024-05-02 19:32:24.000000 mypy_boto3_ec2-1.34.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:15.122121 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-05-02 19:32:24.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-05-02 19:32:24.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 19:32:24.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   544778 2024-05-02 19:32:30.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   544775 2024-05-02 19:32:28.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    97079 2024-05-02 19:32:39.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97079 2024-05-02 19:32:38.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   187386 2024-05-02 19:32:36.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   187243 2024-05-02 19:32:35.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:32:24.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   272189 2024-05-02 19:32:35.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)   272111 2024-05-02 19:32:33.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   886036 2024-05-02 19:32:56.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   886036 2024-05-02 19:32:50.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 19:32:24.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-05-02 19:32:36.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39737 2024-05-02 19:32:36.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:15.126121 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-05-02 19:33:15.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-02 19:33:15.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:33:15.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:33:15.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 19:33:15.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 19:33:15.000000 mypy_boto3_ec2-1.34.97/mypy_boto3_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:33:15.126121 mypy_boto3_ec2-1.34.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-02 19:32:24.000000 mypy_boto3_ec2-1.34.97/setup.py
```

### Comparing `mypy_boto3_ec2-1.34.96/LICENSE` & `mypy_boto3_ec2-1.34.97/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.96/PKG-INFO` & `mypy_boto3_ec2-1.34.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.34.96
-Summary: Type annotations for boto3.EC2 1.34.96 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.97
+Summary: Type annotations for boto3.EC2 1.34.97 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_ec2-1.34.96/README.md` & `mypy_boto3_ec2-1.34.97/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__init__.py` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__init__.pyi` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/__main__.py` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EC2 1.34.96\n"
-        "Version:         1.34.96\n"
+        "Type annotations for boto3.EC2 1.34.97\n"
+        "Version:         1.34.97\n"
         "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.96")
+    print("1.34.97")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/client.py` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     CapacityReservationTenancyType,
     ConnectivityTypeType,
     DefaultInstanceMetadataEndpointStateType,
     DefaultInstanceMetadataTagsStateType,
     DeviceTrustProviderTypeType,
     DiskImageFormatType,
     DomainTypeType,
+    EkPubKeyFormatType,
+    EkPubKeyTypeType,
     EndDateTypeType,
     EventTypeType,
     ExcessCapacityTerminationPolicyType,
     ExportEnvironmentType,
     FleetEventTypeType,
     FleetExcessCapacityTerminationPolicyType,
     FleetTypeType,
@@ -695,14 +697,15 @@
     GetEbsDefaultKmsKeyIdResultTypeDef,
     GetEbsEncryptionByDefaultResultTypeDef,
     GetFlowLogsIntegrationTemplateResultTypeDef,
     GetGroupsForCapacityReservationResultTypeDef,
     GetHostReservationPurchasePreviewResultTypeDef,
     GetImageBlockPublicAccessStateResultTypeDef,
     GetInstanceMetadataDefaultsResultTypeDef,
+    GetInstanceTpmEkPubResultTypeDef,
     GetInstanceTypesFromInstanceRequirementsResultTypeDef,
     GetInstanceUefiDataResultTypeDef,
     GetIpamAddressHistoryResultTypeDef,
     GetIpamDiscoveredAccountsResultTypeDef,
     GetIpamDiscoveredPublicAddressesResultTypeDef,
     GetIpamDiscoveredResourceCidrsResultTypeDef,
     GetIpamPoolAllocationsResultTypeDef,
@@ -7444,14 +7447,31 @@
         account level in the specified Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.get_instance_metadata_defaults)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#get_instance_metadata_defaults)
         """
 
+    def get_instance_tpm_ek_pub(
+        self,
+        *,
+        InstanceId: str,
+        KeyType: EkPubKeyTypeType,
+        KeyFormat: EkPubKeyFormatType,
+        DryRun: bool = ...,
+    ) -> GetInstanceTpmEkPubResultTypeDef:
+        """
+        Gets the public endorsement key associated with the Nitro Trusted Platform
+        Module (NitroTPM) for the specified
+        instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.get_instance_tpm_ek_pub)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#get_instance_tpm_ek_pub)
+        """
+
     def get_instance_types_from_instance_requirements(
         self,
         *,
         ArchitectureTypes: Sequence[ArchitectureTypeType],
         VirtualizationTypes: Sequence[VirtualizationTypeType],
         InstanceRequirements: InstanceRequirementsRequestTypeDef,
         DryRun: bool = ...,
```

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/client.pyi` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     CapacityReservationTenancyType,
     ConnectivityTypeType,
     DefaultInstanceMetadataEndpointStateType,
     DefaultInstanceMetadataTagsStateType,
     DeviceTrustProviderTypeType,
     DiskImageFormatType,
     DomainTypeType,
+    EkPubKeyFormatType,
+    EkPubKeyTypeType,
     EndDateTypeType,
     EventTypeType,
     ExcessCapacityTerminationPolicyType,
     ExportEnvironmentType,
     FleetEventTypeType,
     FleetExcessCapacityTerminationPolicyType,
     FleetTypeType,
@@ -695,14 +697,15 @@
     GetEbsDefaultKmsKeyIdResultTypeDef,
     GetEbsEncryptionByDefaultResultTypeDef,
     GetFlowLogsIntegrationTemplateResultTypeDef,
     GetGroupsForCapacityReservationResultTypeDef,
     GetHostReservationPurchasePreviewResultTypeDef,
     GetImageBlockPublicAccessStateResultTypeDef,
     GetInstanceMetadataDefaultsResultTypeDef,
+    GetInstanceTpmEkPubResultTypeDef,
     GetInstanceTypesFromInstanceRequirementsResultTypeDef,
     GetInstanceUefiDataResultTypeDef,
     GetIpamAddressHistoryResultTypeDef,
     GetIpamDiscoveredAccountsResultTypeDef,
     GetIpamDiscoveredPublicAddressesResultTypeDef,
     GetIpamDiscoveredResourceCidrsResultTypeDef,
     GetIpamPoolAllocationsResultTypeDef,
@@ -7441,14 +7444,31 @@
         account level in the specified Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.get_instance_metadata_defaults)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#get_instance_metadata_defaults)
         """
 
+    def get_instance_tpm_ek_pub(
+        self,
+        *,
+        InstanceId: str,
+        KeyType: EkPubKeyTypeType,
+        KeyFormat: EkPubKeyFormatType,
+        DryRun: bool = ...,
+    ) -> GetInstanceTpmEkPubResultTypeDef:
+        """
+        Gets the public endorsement key associated with the Nitro Trusted Platform
+        Module (NitroTPM) for the specified
+        instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.get_instance_tpm_ek_pub)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#get_instance_tpm_ek_pub)
+        """
+
     def get_instance_types_from_instance_requirements(
         self,
         *,
         ArchitectureTypes: Sequence[ArchitectureTypeType],
         VirtualizationTypes: Sequence[VirtualizationTypeType],
         InstanceRequirements: InstanceRequirementsRequestTypeDef,
         DryRun: bool = ...,
```

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/literals.py` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,14 +219,16 @@
     "DnsSupportValueType",
     "DomainTypeType",
     "DynamicRoutingValueType",
     "EbsEncryptionSupportType",
     "EbsNvmeSupportType",
     "EbsOptimizedSupportType",
     "Ec2InstanceConnectEndpointStateType",
+    "EkPubKeyFormatType",
+    "EkPubKeyTypeType",
     "ElasticGpuStateType",
     "ElasticGpuStatusType",
     "EnaSupportType",
     "EndDateTypeType",
     "EphemeralNvmeSupportType",
     "EventCodeType",
     "EventTypeType",
@@ -898,14 +900,16 @@
     "create-complete",
     "create-failed",
     "create-in-progress",
     "delete-complete",
     "delete-failed",
     "delete-in-progress",
 ]
+EkPubKeyFormatType = Literal["der", "tpmt"]
+EkPubKeyTypeType = Literal["ecc-sec-p384", "rsa-2048"]
 ElasticGpuStateType = Literal["ATTACHED"]
 ElasticGpuStatusType = Literal["IMPAIRED", "OK"]
 EnaSupportType = Literal["required", "supported", "unsupported"]
 EndDateTypeType = Literal["limited", "unlimited"]
 EphemeralNvmeSupportType = Literal["required", "supported", "unsupported"]
 EventCodeType = Literal[
     "instance-reboot", "instance-retirement", "instance-stop", "system-maintenance", "system-reboot"
```

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/literals.pyi` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -219,14 +219,16 @@
     "DnsSupportValueType",
     "DomainTypeType",
     "DynamicRoutingValueType",
     "EbsEncryptionSupportType",
     "EbsNvmeSupportType",
     "EbsOptimizedSupportType",
     "Ec2InstanceConnectEndpointStateType",
+    "EkPubKeyFormatType",
+    "EkPubKeyTypeType",
     "ElasticGpuStateType",
     "ElasticGpuStatusType",
     "EnaSupportType",
     "EndDateTypeType",
     "EphemeralNvmeSupportType",
     "EventCodeType",
     "EventTypeType",
@@ -898,14 +900,16 @@
     "create-complete",
     "create-failed",
     "create-in-progress",
     "delete-complete",
     "delete-failed",
     "delete-in-progress",
 ]
+EkPubKeyFormatType = Literal["der", "tpmt"]
+EkPubKeyTypeType = Literal["ecc-sec-p384", "rsa-2048"]
 ElasticGpuStateType = Literal["ATTACHED"]
 ElasticGpuStatusType = Literal["IMPAIRED", "OK"]
 EnaSupportType = Literal["required", "supported", "unsupported"]
 EndDateTypeType = Literal["limited", "unlimited"]
 EphemeralNvmeSupportType = Literal["required", "supported", "unsupported"]
 EventCodeType = Literal[
     "instance-reboot", "instance-retirement", "instance-stop", "system-maintenance", "system-reboot"
```

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/paginator.py` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/paginator.pyi` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/service_resource.py` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/service_resource.pyi` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/type_defs.py` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,16 @@
     DnsSupportValueType,
     DomainTypeType,
     DynamicRoutingValueType,
     EbsEncryptionSupportType,
     EbsNvmeSupportType,
     EbsOptimizedSupportType,
     Ec2InstanceConnectEndpointStateType,
+    EkPubKeyFormatType,
+    EkPubKeyTypeType,
     ElasticGpuStatusType,
     EnaSupportType,
     EndDateTypeType,
     EphemeralNvmeSupportType,
     EventCodeType,
     EventTypeType,
     ExcessCapacityTerminationPolicyType,
@@ -820,14 +822,15 @@
     "GetEbsEncryptionByDefaultRequestRequestTypeDef",
     "GetGroupsForCapacityReservationRequestRequestTypeDef",
     "GetHostReservationPurchasePreviewRequestRequestTypeDef",
     "PurchaseTypeDef",
     "GetImageBlockPublicAccessStateRequestRequestTypeDef",
     "GetInstanceMetadataDefaultsRequestRequestTypeDef",
     "InstanceMetadataDefaultsResponseTypeDef",
+    "GetInstanceTpmEkPubRequestRequestTypeDef",
     "InstanceTypeInfoFromInstanceRequirementsTypeDef",
     "GetInstanceUefiDataRequestRequestTypeDef",
     "IpamAddressHistoryRecordTypeDef",
     "GetLaunchTemplateDataRequestRequestTypeDef",
     "GetManagedPrefixListAssociationsRequestRequestTypeDef",
     "PrefixListAssociationTypeDef",
     "GetManagedPrefixListEntriesRequestRequestTypeDef",
@@ -1239,14 +1242,15 @@
     "ExportTransitGatewayRoutesResultTypeDef",
     "GetConsoleOutputResultTypeDef",
     "GetConsoleScreenshotResultTypeDef",
     "GetEbsDefaultKmsKeyIdResultTypeDef",
     "GetEbsEncryptionByDefaultResultTypeDef",
     "GetFlowLogsIntegrationTemplateResultTypeDef",
     "GetImageBlockPublicAccessStateResultTypeDef",
+    "GetInstanceTpmEkPubResultTypeDef",
     "GetInstanceUefiDataResultTypeDef",
     "GetPasswordDataResultTypeDef",
     "GetSerialConsoleAccessStatusResultTypeDef",
     "GetSnapshotBlockPublicAccessStateResultTypeDef",
     "GetVerifiedAccessEndpointPolicyResultTypeDef",
     "GetVerifiedAccessGroupPolicyResultTypeDef",
     "GetVpnConnectionDeviceSampleConfigurationResultTypeDef",
@@ -6526,14 +6530,23 @@
     {
         "HttpTokens": NotRequired[HttpTokensStateType],
         "HttpPutResponseHopLimit": NotRequired[int],
         "HttpEndpoint": NotRequired[InstanceMetadataEndpointStateType],
         "InstanceMetadataTags": NotRequired[InstanceMetadataTagsStateType],
     },
 )
+GetInstanceTpmEkPubRequestRequestTypeDef = TypedDict(
+    "GetInstanceTpmEkPubRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "KeyType": EkPubKeyTypeType,
+        "KeyFormat": EkPubKeyFormatType,
+        "DryRun": NotRequired[bool],
+    },
+)
 InstanceTypeInfoFromInstanceRequirementsTypeDef = TypedDict(
     "InstanceTypeInfoFromInstanceRequirementsTypeDef",
     {
         "InstanceType": NotRequired[str],
     },
 )
 GetInstanceUefiDataRequestRequestTypeDef = TypedDict(
@@ -9836,14 +9849,24 @@
 GetImageBlockPublicAccessStateResultTypeDef = TypedDict(
     "GetImageBlockPublicAccessStateResultTypeDef",
     {
         "ImageBlockPublicAccessState": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetInstanceTpmEkPubResultTypeDef = TypedDict(
+    "GetInstanceTpmEkPubResultTypeDef",
+    {
+        "InstanceId": str,
+        "KeyType": EkPubKeyTypeType,
+        "KeyFormat": EkPubKeyFormatType,
+        "KeyValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetInstanceUefiDataResultTypeDef = TypedDict(
     "GetInstanceUefiDataResultTypeDef",
     {
         "InstanceId": str,
         "UefiData": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -19694,15 +19717,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 RevokeSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeSecurityGroupIngressResultTypeDef",
     {
         "Return": bool,
-        "UnknownIpPermissions": List[IpPermissionExtraExtraOutputTypeDef],
+        "UnknownIpPermissions": List[IpPermissionOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SecurityGroupTypeDef = TypedDict(
     "SecurityGroupTypeDef",
     {
         "Description": NotRequired[str],
```

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/type_defs.pyi` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,16 @@
     DnsSupportValueType,
     DomainTypeType,
     DynamicRoutingValueType,
     EbsEncryptionSupportType,
     EbsNvmeSupportType,
     EbsOptimizedSupportType,
     Ec2InstanceConnectEndpointStateType,
+    EkPubKeyFormatType,
+    EkPubKeyTypeType,
     ElasticGpuStatusType,
     EnaSupportType,
     EndDateTypeType,
     EphemeralNvmeSupportType,
     EventCodeType,
     EventTypeType,
     ExcessCapacityTerminationPolicyType,
@@ -820,14 +822,15 @@
     "GetEbsEncryptionByDefaultRequestRequestTypeDef",
     "GetGroupsForCapacityReservationRequestRequestTypeDef",
     "GetHostReservationPurchasePreviewRequestRequestTypeDef",
     "PurchaseTypeDef",
     "GetImageBlockPublicAccessStateRequestRequestTypeDef",
     "GetInstanceMetadataDefaultsRequestRequestTypeDef",
     "InstanceMetadataDefaultsResponseTypeDef",
+    "GetInstanceTpmEkPubRequestRequestTypeDef",
     "InstanceTypeInfoFromInstanceRequirementsTypeDef",
     "GetInstanceUefiDataRequestRequestTypeDef",
     "IpamAddressHistoryRecordTypeDef",
     "GetLaunchTemplateDataRequestRequestTypeDef",
     "GetManagedPrefixListAssociationsRequestRequestTypeDef",
     "PrefixListAssociationTypeDef",
     "GetManagedPrefixListEntriesRequestRequestTypeDef",
@@ -1239,14 +1242,15 @@
     "ExportTransitGatewayRoutesResultTypeDef",
     "GetConsoleOutputResultTypeDef",
     "GetConsoleScreenshotResultTypeDef",
     "GetEbsDefaultKmsKeyIdResultTypeDef",
     "GetEbsEncryptionByDefaultResultTypeDef",
     "GetFlowLogsIntegrationTemplateResultTypeDef",
     "GetImageBlockPublicAccessStateResultTypeDef",
+    "GetInstanceTpmEkPubResultTypeDef",
     "GetInstanceUefiDataResultTypeDef",
     "GetPasswordDataResultTypeDef",
     "GetSerialConsoleAccessStatusResultTypeDef",
     "GetSnapshotBlockPublicAccessStateResultTypeDef",
     "GetVerifiedAccessEndpointPolicyResultTypeDef",
     "GetVerifiedAccessGroupPolicyResultTypeDef",
     "GetVpnConnectionDeviceSampleConfigurationResultTypeDef",
@@ -6526,14 +6530,23 @@
     {
         "HttpTokens": NotRequired[HttpTokensStateType],
         "HttpPutResponseHopLimit": NotRequired[int],
         "HttpEndpoint": NotRequired[InstanceMetadataEndpointStateType],
         "InstanceMetadataTags": NotRequired[InstanceMetadataTagsStateType],
     },
 )
+GetInstanceTpmEkPubRequestRequestTypeDef = TypedDict(
+    "GetInstanceTpmEkPubRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "KeyType": EkPubKeyTypeType,
+        "KeyFormat": EkPubKeyFormatType,
+        "DryRun": NotRequired[bool],
+    },
+)
 InstanceTypeInfoFromInstanceRequirementsTypeDef = TypedDict(
     "InstanceTypeInfoFromInstanceRequirementsTypeDef",
     {
         "InstanceType": NotRequired[str],
     },
 )
 GetInstanceUefiDataRequestRequestTypeDef = TypedDict(
@@ -9836,14 +9849,24 @@
 GetImageBlockPublicAccessStateResultTypeDef = TypedDict(
     "GetImageBlockPublicAccessStateResultTypeDef",
     {
         "ImageBlockPublicAccessState": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetInstanceTpmEkPubResultTypeDef = TypedDict(
+    "GetInstanceTpmEkPubResultTypeDef",
+    {
+        "InstanceId": str,
+        "KeyType": EkPubKeyTypeType,
+        "KeyFormat": EkPubKeyFormatType,
+        "KeyValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetInstanceUefiDataResultTypeDef = TypedDict(
     "GetInstanceUefiDataResultTypeDef",
     {
         "InstanceId": str,
         "UefiData": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -19694,15 +19717,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 RevokeSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeSecurityGroupIngressResultTypeDef",
     {
         "Return": bool,
-        "UnknownIpPermissions": List[IpPermissionExtraExtraOutputTypeDef],
+        "UnknownIpPermissions": List[IpPermissionOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SecurityGroupTypeDef = TypedDict(
     "SecurityGroupTypeDef",
     {
         "Description": NotRequired[str],
```

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/waiter.py` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2/waiter.pyi` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/PKG-INFO` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.34.96
-Summary: Type annotations for boto3.EC2 1.34.96 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.97
+Summary: Type annotations for boto3.EC2 1.34.97 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_ec2-1.34.96/mypy_boto3_ec2.egg-info/SOURCES.txt` & `mypy_boto3_ec2-1.34.97/mypy_boto3_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.96/setup.py` & `mypy_boto3_ec2-1.34.97/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ec2",
-    version="1.34.96",
+    version="1.34.97",
     packages=["mypy_boto3_ec2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EC2 1.34.96 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.EC2 1.34.97 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

