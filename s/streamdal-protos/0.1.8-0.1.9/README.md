# Comparing `tmp/streamdal-protos-0.1.8.tar.gz` & `tmp/streamdal-protos-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdal-protos-0.1.8.tar", last modified: Wed Jan  3 18:57:12 2024, max compression
+gzip compressed data, was "streamdal-protos-0.1.9.tar", last modified: Fri Jan  5 14:16:10 2024, max compression
```

## Comparing `streamdal-protos-0.1.8.tar` & `streamdal-protos-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:57:12.549123 streamdal-protos-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-03 18:57:12.549123 streamdal-protos-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-03 18:56:45.000000 streamdal-protos-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 18:57:12.549123 streamdal-protos-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-03 18:57:11.000000 streamdal-protos-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:57:12.549123 streamdal-protos-0.1.8/streamdal_protos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 18:56:45.000000 streamdal-protos-0.1.8/streamdal_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:57:12.549123 streamdal-protos-0.1.8/streamdal_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (127)    88102 2024-01-03 18:56:45.000000 streamdal-protos-0.1.8/streamdal_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:57:12.549123 streamdal-protos-0.1.8/streamdal_protos/protos/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-03 18:56:45.000000 streamdal-protos-0.1.8/streamdal_protos/protos/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:57:12.549123 streamdal-protos-0.1.8/streamdal_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (127)    12250 2024-01-03 18:56:45.000000 streamdal-protos-0.1.8/streamdal_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 18:57:12.549123 streamdal-protos-0.1.8/streamdal_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-03 18:57:12.000000 streamdal-protos-0.1.8/streamdal_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-01-03 18:57:12.000000 streamdal-protos-0.1.8/streamdal_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 18:57:12.000000 streamdal-protos-0.1.8/streamdal_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-03 18:57:12.000000 streamdal-protos-0.1.8/streamdal_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 14:16:10.334605 streamdal-protos-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-05 14:16:10.334605 streamdal-protos-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-05 14:15:39.000000 streamdal-protos-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 14:16:10.334605 streamdal-protos-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-05 14:16:10.000000 streamdal-protos-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 14:16:10.334605 streamdal-protos-0.1.9/streamdal_protos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 14:15:39.000000 streamdal-protos-0.1.9/streamdal_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 14:16:10.334605 streamdal-protos-0.1.9/streamdal_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)    88102 2024-01-05 14:15:39.000000 streamdal-protos-0.1.9/streamdal_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 14:16:10.334605 streamdal-protos-0.1.9/streamdal_protos/protos/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-05 14:15:39.000000 streamdal-protos-0.1.9/streamdal_protos/protos/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 14:16:10.334605 streamdal-protos-0.1.9/streamdal_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)    13010 2024-01-05 14:15:39.000000 streamdal-protos-0.1.9/streamdal_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 14:16:10.334605 streamdal-protos-0.1.9/streamdal_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-05 14:16:10.000000 streamdal-protos-0.1.9/streamdal_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-01-05 14:16:10.000000 streamdal-protos-0.1.9/streamdal_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 14:16:10.000000 streamdal-protos-0.1.9/streamdal_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-05 14:16:10.000000 streamdal-protos-0.1.9/streamdal_protos.egg-info/top_level.txt
```

### Comparing `streamdal-protos-0.1.8/PKG-INFO` & `streamdal-protos-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdal-protos
-Version: 0.1.8
+Version: 0.1.9
 Summary: Protobuf python package for Streamdal.com server and SDKs
 Home-page: https://github.com/streamdal/streamdal/tree/main/libs/protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `streamdal-protos-0.1.8/setup.py` & `streamdal-protos-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='streamdal-protos',
-    version='0.1.8',
+    version='0.1.9',
     description='Protobuf python package for Streamdal.com server and SDKs',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/streamdal/tree/main/libs/protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `streamdal-protos-0.1.8/streamdal_protos/protos/__init__.py` & `streamdal-protos-0.1.9/streamdal_protos/protos/__init__.py`

 * *Files identical despite different names*

### Comparing `streamdal-protos-0.1.8/streamdal_protos/protos/shared/__init__.py` & `streamdal-protos-0.1.9/streamdal_protos/protos/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `streamdal-protos-0.1.8/streamdal_protos/protos/steps/__init__.py` & `streamdal-protos-0.1.9/streamdal_protos/protos/steps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,15 @@
 class TransformType(betterproto.Enum):
     TRANSFORM_TYPE_UNKNOWN = 0
     TRANSFORM_TYPE_REPLACE_VALUE = 1
     TRANSFORM_TYPE_DELETE_FIELD = 2
     TRANSFORM_TYPE_OBFUSCATE_VALUE = 3
     TRANSFORM_TYPE_MASK_VALUE = 4
     TRANSFORM_TYPE_TRUNCATE_VALUE = 5
+    TRANSFORM_TYPE_EXTRACT = 6
 
 
 class TransformTruncateType(betterproto.Enum):
     TRANSFORM_TRUNCATE_TYPE_UNKNOWN = 0
     TRANSFORM_TRUNCATE_TYPE_LENGTH = 1
     TRANSFORM_TRUNCATE_TYPE_PERCENTAGE = 2
 
@@ -325,26 +326,43 @@
 class TransformStep(betterproto.Message):
     path: str = betterproto.string_field(1)
     value: str = betterproto.string_field(2)
     type: "TransformType" = betterproto.enum_field(3)
     replace_value_options: "TransformReplaceValueOptions" = betterproto.message_field(
         101, group="options"
     )
+    """Replace the value of a field with a new value"""
+
     delete_field_options: "TransformDeleteFieldOptions" = betterproto.message_field(
         102, group="options"
     )
+    """Delete a field from a JSON payload"""
+
     obfuscate_options: "TransformObfuscateOptions" = betterproto.message_field(
         103, group="options"
     )
+    """Obfuscate hashes the value of a field with sha256"""
+
     mask_options: "TransformMaskOptions" = betterproto.message_field(
         104, group="options"
     )
+    """Mask part of a field's value with the given character"""
+
     truncate_options: "TransformTruncateOptions" = betterproto.message_field(
         105, group="options"
     )
+    """
+    Truncate the value of a field to a maximum number of characters, or to a
+    percentage of characters based on the field length
+    """
+
+    extract_options: "TransformExtractOptions" = betterproto.message_field(
+        106, group="options"
+    )
+    """Extract one or multiple values from a payload"""
 
     def __post_init__(self) -> None:
         super().__post_init__()
         if self.is_set("path"):
             warnings.warn("TransformStep.path is deprecated", DeprecationWarning)
         if self.is_set("value"):
             warnings.warn("TransformStep.value is deprecated", DeprecationWarning)
@@ -379,9 +397,15 @@
 @dataclass(eq=False, repr=False)
 class TransformMaskOptions(betterproto.Message):
     path: str = betterproto.string_field(1)
     mask: str = betterproto.string_field(2)
 
 
 @dataclass(eq=False, repr=False)
+class TransformExtractOptions(betterproto.Message):
+    paths: List[str] = betterproto.string_field(1)
+    flatten: bool = betterproto.bool_field(2)
+
+
+@dataclass(eq=False, repr=False)
 class ValidJsonStep(betterproto.Message):
     pass
```

### Comparing `streamdal-protos-0.1.8/streamdal_protos.egg-info/PKG-INFO` & `streamdal-protos-0.1.9/streamdal_protos.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdal-protos
-Version: 0.1.8
+Version: 0.1.9
 Summary: Protobuf python package for Streamdal.com server and SDKs
 Home-page: https://github.com/streamdal/streamdal/tree/main/libs/protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

