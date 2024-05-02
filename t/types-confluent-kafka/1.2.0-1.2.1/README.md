# Comparing `tmp/types_confluent_kafka-1.2.0.tar.gz` & `tmp/types_confluent_kafka-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types_confluent_kafka-1.2.0.tar", max compression
+gzip compressed data, was "types_confluent_kafka-1.2.1.tar", max compression
```

## Comparing `types_confluent_kafka-1.2.0.tar` & `types_confluent_kafka-1.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11366 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/LICENSE
--rw-r--r--   0        0        0     3243 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/README.md
--rw-r--r--   0        0        0     1894 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/__init__.pyi
--rw-r--r--   0        0        0      971 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/_model/__init__.pyi
--rw-r--r--   0        0        0      317 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/_util/__init__.pyi
--rw-r--r--   0        0        0      359 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/_util/conversion_util.pyi
--rw-r--r--   0        0        0      691 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/_util/validation_util.pyi
--rw-r--r--   0        0        0     6514 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/__init__.pyi
--rw-r--r--   0        0        0     3218 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/_acl.pyi
--rw-r--r--   0        0        0     2387 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/_config.pyi
--rw-r--r--   0        0        0     2164 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/_group.pyi
--rw-r--r--   0        0        0     1955 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/_metadata.pyi
--rw-r--r--   0        0        0      687 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/_resource.pyi
--rw-r--r--   0        0        0     1575 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/_scram.pyi
--rw-r--r--   0        0        0     1782 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/avro/__init__.pyi
--rw-r--r--   0        0        0     2438 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/avro/cached_schema_registry_client.pyi
--rw-r--r--   0        0        0      436 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/avro/error.pyi
--rw-r--r--   0        0        0      750 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/avro/load.pyi
--rw-r--r--   0        0        0      450 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/avro/serializer/__init__.pyi
--rw-r--r--   0        0        0     1873 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/avro/serializer/message_serializer.pyi
--rw-r--r--   0        0        0    18924 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/cimpl.pyi
--rw-r--r--   0        0        0      938 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/deserializing_consumer.pyi
--rw-r--r--   0        0        0     2566 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/error.pyi
--rw-r--r--   0        0        0      270 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/kafkatest/__init__.pyi
--rw-r--r--   0        0        0      192 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/kafkatest/verifiable_client.pyi
--rw-r--r--   0        0        0      192 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/kafkatest/verifiable_consumer.pyi
--rw-r--r--   0        0        0      192 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/kafkatest/verifiable_producer.pyi
--rw-r--r--   0        0        0      951 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/__init__.pyi
--rw-r--r--   0        0        0     1734 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/avro.pyi
--rw-r--r--   0        0        0      633 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/error.pyi
--rw-r--r--   0        0        0     1685 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/json_schema.pyi
--rw-r--r--   0        0        0     1285 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/protobuf.pyi
--rw-r--r--   0        0        0     3410 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/schema_registry_client.pyi
--rw-r--r--   0        0        0     1745 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/serialization/__init__.pyi
--rw-r--r--   0        0        0     1085 2024-02-08 07:12:59.478102 types_confluent_kafka-1.2.0/confluent_kafka-stubs/serializing_producer.pyi
--rw-r--r--   0        0        0     2701 2024-02-08 07:13:23.045922 types_confluent_kafka-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4455 1970-01-01 00:00:00.000000 types_confluent_kafka-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11366 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3243 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/README.md
+-rw-r--r--   0        0        0     1894 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/__init__.pyi
+-rw-r--r--   0        0        0      873 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/_model/__init__.pyi
+-rw-r--r--   0        0        0      317 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/_util/__init__.pyi
+-rw-r--r--   0        0        0      359 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/_util/conversion_util.pyi
+-rw-r--r--   0        0        0      691 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/_util/validation_util.pyi
+-rw-r--r--   0        0        0     6514 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/__init__.pyi
+-rw-r--r--   0        0        0     3098 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/_acl.pyi
+-rw-r--r--   0        0        0     2257 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/_config.pyi
+-rw-r--r--   0        0        0     1946 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/_group.pyi
+-rw-r--r--   0        0        0     1481 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/_metadata.pyi
+-rw-r--r--   0        0        0      687 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/_resource.pyi
+-rw-r--r--   0        0        0     1495 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/_scram.pyi
+-rw-r--r--   0        0        0     1782 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/avro/__init__.pyi
+-rw-r--r--   0        0        0     2378 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/avro/cached_schema_registry_client.pyi
+-rw-r--r--   0        0        0      368 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/avro/error.pyi
+-rw-r--r--   0        0        0      750 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/avro/load.pyi
+-rw-r--r--   0        0        0      392 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/avro/serializer/__init__.pyi
+-rw-r--r--   0        0        0     1813 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/avro/serializer/message_serializer.pyi
+-rw-r--r--   0        0        0    18924 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/cimpl.pyi
+-rw-r--r--   0        0        0      938 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/deserializing_consumer.pyi
+-rw-r--r--   0        0        0     2498 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/error.pyi
+-rw-r--r--   0        0        0      270 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/kafkatest/__init__.pyi
+-rw-r--r--   0        0        0      192 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/kafkatest/verifiable_client.pyi
+-rw-r--r--   0        0        0      192 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/kafkatest/verifiable_consumer.pyi
+-rw-r--r--   0        0        0      192 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/kafkatest/verifiable_producer.pyi
+-rw-r--r--   0        0        0      951 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/__init__.pyi
+-rw-r--r--   0        0        0     1882 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/avro.pyi
+-rw-r--r--   0        0        0      555 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/error.pyi
+-rw-r--r--   0        0        0     1765 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/json_schema.pyi
+-rw-r--r--   0        0        0     1285 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/protobuf.pyi
+-rw-r--r--   0        0        0     3260 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/schema_registry_client.pyi
+-rw-r--r--   0        0        0     1815 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/serialization/__init__.pyi
+-rw-r--r--   0        0        0     1085 2024-05-02 10:49:38.654158 types_confluent_kafka-1.2.1/confluent_kafka-stubs/serializing_producer.pyi
+-rw-r--r--   0        0        0     2701 2024-05-02 10:50:10.310190 types_confluent_kafka-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4455 1970-01-01 00:00:00.000000 types_confluent_kafka-1.2.1/PKG-INFO
```

### Comparing `types_confluent_kafka-1.2.0/LICENSE` & `types_confluent_kafka-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/README.md` & `types_confluent_kafka-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/__init__.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/_model/__init__.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/_model/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 types-confluent-kafka: A package providing type hints for the confluent-kafka Python package.
 This package is licensed under the Apache 2.0 License.
 """
 from __future__ import annotations
 
 # standard library
 from enum import Enum
-from typing import ClassVar
 
 from ..cimpl import TopicPartition
 
 class Node:
-    id: ClassVar[int]
-    id_string: ClassVar[str]
-    host: ClassVar[str]
-    port: ClassVar[int]
-    rack: ClassVar[str]
+    id: int
+    id_string: str
+    host: str
+    port: int
+    rack: str
 
     def __init__(self, id: int, host: str, port: int, rack: str | None = None) -> None: ...
 
 class ConsumerGroupTopicPartitions:
-    group_id: ClassVar[str]
-    topic_partitions: ClassVar[list["TopicPartition"]]
+    group_id: str
+    topic_partitions: list["TopicPartition"]
 
     def __init__(self, group_id: str, topic_partitions: list["TopicPartition"] | None = None) -> None: ...
 
 class ConsumerGroupState(Enum):
     UNKNOWN: int
     UNKOWN: int
     PREPARING_REBALANCING: int
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/_util/validation_util.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/_util/validation_util.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/__init__.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/_acl.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/_acl.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 types-confluent-kafka: A package providing type hints for the confluent-kafka Python package.
 This package is licensed under the Apache 2.0 License.
 """
 from __future__ import annotations
 
 # standard library
 from enum import Enum, EnumMeta
-from typing import Any, ClassVar, Literal
+from typing import Any, Literal
 
 from .._util import ConversionUtil as ConversionUtil
 from .._util import ValidationUtil as ValidationUtil
 from ._resource import ResourcePatternType as ResourcePatternType
 from ._resource import ResourceType as ResourceType
 
 class AclOperation(Enum):
@@ -35,25 +35,25 @@
     ANY: int
     DENY: int
     ALLOW: int
 
     def __lt__(self, other: AclPermissionType) -> bool: ...
 
 class AclBinding:
-    restype: ClassVar[ResourceType]
-    name: ClassVar[str]
-    resource_pattern_type: ClassVar[ResourcePatternType]
-    principal: ClassVar[str]
-    host: ClassVar[str]
-    operation: ClassVar[AclOperation]
-    permission_type: ClassVar[AclPermissionType]
-    restype_int: ClassVar[int]
-    resource_pattern_type_int: ClassVar[int]
-    operation_int: ClassVar[int]
-    permission_type_int: ClassVar[int]
+    restype: ResourceType
+    name: str
+    resource_pattern_type: ResourcePatternType
+    principal: str
+    host: str
+    operation: AclOperation
+    permission_type: AclPermissionType
+    restype_int: int
+    resource_pattern_type_int: int
+    operation_int: int
+    permission_type_int: int
 
     def __init__(
         self,
         restype: ResourceType,
         name: str,
         resource_pattern_type: ResourcePatternType,
         principal: str,
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/_group.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/_group.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 """
 types-confluent-kafka: A package providing type hints for the confluent-kafka Python package.
 This package is licensed under the Apache 2.0 License.
 """
 from __future__ import annotations
 
-# standard library
-from typing import ClassVar
-
 from .._model import ConsumerGroupState as ConsumerGroupState
 from .._model import Node as Node
 from .._util import ConversionUtil as ConversionUtil
 from ..cimpl import TopicPartition as TopicPartition
 from ..error import KafkaException as KafkaException
 
 class ConsumerGroupListing:
-    group_id: ClassVar[str]
-    is_simple_consumer_group: ClassVar[bool]
-    state: ClassVar[ConsumerGroupState]
+    group_id: str
+    is_simple_consumer_group: bool
+    state: ConsumerGroupState
 
     def __init__(
         self,
         group_id: str,
         is_simple_consumer_group: bool,
         state: ConsumerGroupState | None = None,
     ) -> None: ...
 
 class ListConsumerGroupsResult:
-    valid: ClassVar[list[ConsumerGroupListing]]
-    errors: ClassVar[list[KafkaException]]
+    valid: list[ConsumerGroupListing]
+    errors: list[KafkaException]
 
     def __init__(
         self,
         valid: list["ConsumerGroupListing"] | None = None,
         errors: list[KafkaException] | None = None,
     ) -> None: ...
 
 class MemberAssignment:
-    topic_partitions: ClassVar[list[TopicPartition]]
+    topic_partitions: list[TopicPartition]
 
     def __init__(self, topic_partitions: list[TopicPartition] | None = None) -> None: ...
 
 class MemberDescription:
-    member_id: ClassVar[str]
-    client_id: ClassVar[str]
-    host: ClassVar[str]
-    assignment: ClassVar[MemberAssignment]
-    group_instance_id: ClassVar[str]
+    member_id: str
+    client_id: str
+    host: str
+    assignment: MemberAssignment
+    group_instance_id: str
 
     def __init__(
         self,
         member_id: str,
         client_id: str,
         host: str,
         assignment: MemberAssignment,
         group_instance_id: str | None = None,
     ) -> None: ...
 
 class ConsumerGroupDescription:
-    group_id: ClassVar[str]
-    is_simple_consumer_group: ClassVar[bool]
-    members: ClassVar[list[MemberDescription]]
-    partition_assignor: ClassVar[str]
-    state: ClassVar[ConsumerGroupState]
-    coordinator: ClassVar[Node]
+    group_id: str
+    is_simple_consumer_group: bool
+    members: list[MemberDescription]
+    partition_assignor: str
+    state: ConsumerGroupState
+    coordinator: Node
 
     def __init__(
         self,
         group_id: str,
         is_simple_consumer_group: bool,
         members: list[MemberDescription],
         partition_assignor: str,
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/_resource.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/_resource.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/admin/_scram.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/admin/_scram.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -14,42 +14,42 @@
     UNKNOWN: ClassVar[int]
     SCRAM_SHA_256: ClassVar[int]
     SCRAM_SHA_512: ClassVar[int]
 
     def __lt__(self, other: "ScramMechanism") -> bool: ...
 
 class ScramCredentialInfo:
-    mechanism: ClassVar[ScramMechanism]
+    mechanism: ScramMechanism
     iterations: int
 
     def __init__(self, mechanism: ScramMechanism, iterations: int) -> None: ...
 
 class UserScramCredentialsDescription:
     user: ClassVar[str]
     scram_credential_info: ClassVar[ScramCredentialInfo]
 
     def __init__(self, user: str, scram_credential_infos: list[ScramCredentialInfo]) -> None: ...
 
 class UserScramCredentialAlteration:
-    user: ClassVar[str]
+    user: str
 
     def __init__(self, user: str) -> None: ...
 
 class UserScramCredentialUpsertion(UserScramCredentialAlteration):
-    user: ClassVar[str]
-    scram_credential_info: ClassVar[ScramCredentialInfo]
-    password: ClassVar[bytes]
-    salt: ClassVar[bytes | None]
+    user: str
+    scram_credential_info: ScramCredentialInfo
+    password: bytes
+    salt: bytes | None
 
     def __init__(
         self,
         user: str,
         scram_credential_info: ScramCredentialInfo,
         password: bytes,
         salt: bytes | None = None,
     ) -> None: ...
 
 class UserScramCredentialDeletion(UserScramCredentialAlteration):
-    user: ClassVar[str]
-    mechanism: ClassVar[ScramMechanism]
+    user: str
+    mechanism: ScramMechanism
 
     def __init__(self, user: str, mechanism: ScramMechanism) -> None: ...
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/avro/__init__.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/avro/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/avro/cached_schema_registry_client.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/avro/cached_schema_registry_client.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This package is licensed under the Apache 2.0 License.
 """
 from __future__ import annotations
 
 # standard library
 from logging import Logger
 from pathlib import Path
-from typing import TYPE_CHECKING, ClassVar, DefaultDict, Literal
+from typing import TYPE_CHECKING, DefaultDict, Literal
 
 from .error import ClientError as ClientError
 from .load import loads as loads
 
 if TYPE_CHECKING:
     """Helping users who installed avro package can get type hints"""
     try:
@@ -24,19 +24,19 @@
 VALID_LEVELS = Literal["NONE", "FULL", "FORWARD", "BACKWARD"]
 VALID_METHODS = Literal["GET", "POST", "PUT", "DELETE"]
 VALID_AUTH_PROVIDERS = Literal["URL", "USER_INFO", "SASL_INHERIT"]
 ACCEPT_HDR: str
 log: Logger
 
 class CachedSchemaRegistryClient:
-    url: ClassVar[str | dict]
-    subject_to_schema_ids: ClassVar[DefaultDict[str, dict]]
-    id_to_schema: ClassVar[DefaultDict[str, dict]]
-    subject_to_schema_versions: ClassVar[DefaultDict[str, dict]]
-    auto_register_schemas: ClassVar[bool]
+    url: str | dict
+    subject_to_schema_ids: DefaultDict[str, dict]
+    id_to_schema: DefaultDict[str, dict]
+    subject_to_schema_versions: DefaultDict[str, dict]
+    auto_register_schemas: bool
 
     def __init__(
         self,
         url: str | dict,
         max_schemas_per_subject: int,
         ca_location: str | Path | None = None,
         cert_location: str | Path | None = None,
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/avro/load.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/avro/load.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/avro/serializer/message_serializer.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/avro/serializer/message_serializer.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This package is licensed under the Apache 2.0 License.
 """
 from __future__ import annotations
 
 # standard library
 from io import BytesIO
 from logging import Logger
-from typing import TYPE_CHECKING, Any, Callable, ClassVar
+from typing import TYPE_CHECKING, Any, Callable
 
 from ...schema_registry.schema_registry_client import SchemaRegistryClient
 from .. import ClientError as ClientError
 from . import KeySerializerError as KeySerializerError
 from . import SerializerError as SerializerError
 from . import ValueSerializerError as ValueSerializerError
 
@@ -29,19 +29,19 @@
         from typing import Any as Schema  # type: ignore
 
 class ContextStringIO(BytesIO):
     def __enter__(self): ...
     def __exit__(self, *args): ...
 
 class MessageSerializer:
-    registry_client: ClassVar[SchemaRegistryClient]
-    id_to_decoder_func: ClassVar[dict[int, Callable]]
-    id_to_writers: ClassVar[dict[int, bytes]]
-    reader_key_schema: ClassVar[str | bytes | None]
-    reader_value_schema: ClassVar[str | bytes | None]
+    registry_client: SchemaRegistryClient
+    id_to_decoder_func: dict[int, Callable]
+    id_to_writers: dict[int, bytes]
+    reader_key_schema: str | bytes | None
+    reader_value_schema: str | bytes | None
 
     def __init__(
         self,
         registry_client,
         reader_key_schema: Any | None = None,
         reader_value_schema: Any | None = None,
     ) -> None: ...
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/cimpl.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/cimpl.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/deserializing_consumer.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/deserializing_consumer.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/error.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/error.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """
 types-confluent-kafka: A package providing type hints for the confluent-kafka Python package.
 This package is licensed under the Apache 2.0 License.
 """
 from __future__ import annotations
 
-# standard library
-from typing import ClassVar
-
 from .cimpl import KafkaError as KafkaError
 from .cimpl import KafkaException as KafkaException
 from .cimpl import Message
 from .serialization import SerializationError as SerializationError
 
 class _KafkaClientError(KafkaException):
     """
@@ -21,16 +18,16 @@
 
         exception(Exception, optional): The original exception
 
         kafka_message (Message, optional): The Kafka Message returned
         by the broker.
     """
 
-    exception: ClassVar[KafkaException]
-    kafka_message: ClassVar[Message]
+    exception: KafkaException
+    kafka_message: Message
 
     def __init__(
         self,
         kafka_error: KafkaError,
         exception: Exception | None = None,
         kafka_message: Message | None = None,
     ) -> None: ...
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/__init__.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/avro.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/json_schema.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,38 +4,37 @@
 """
 from __future__ import annotations
 
 # standard library
 from io import BytesIO
 from typing import Any, Callable
 
+from ..schema_registry import Schema as Schema
+from ..schema_registry import topic_subject_name_strategy as topic_subject_name_strategy
+from ..schema_registry.schema_registry_client import SchemaRegistryClient
 from ..serialization import Deserializer as Deserializer
 from ..serialization import SerializationContext
 from ..serialization import SerializationError as SerializationError
 from ..serialization import Serializer as Serializer
-from . import Schema as Schema
-from . import topic_subject_name_strategy as topic_subject_name_strategy
-from .schema_registry_client import SchemaRegistryClient
 
 class _ContextStringIO(BytesIO):
     def __enter__(self) -> _ContextStringIO: ...
     def __exit__(self, *args): ...
 
-class AvroSerializer(Serializer):
+class JSONSerializer(Serializer):
     def __init__(
         self,
-        schema_registry_client: SchemaRegistryClient,
         schema_str: str | Schema,
+        schema_registry_client: SchemaRegistryClient,
         to_dict: Callable[[object, SerializationContext], dict[Any, Any]] | None = None,
         conf: dict | None = None,
     ) -> None: ...
-    def __call__(self, obj: object, ctx: SerializationContext) -> None: ...  # type: ignore # issue: https://github.com/confluentinc/confluent-kafka-python/issues/1631
+    def __call__(self, obj: object, ctx: SerializationContext) -> bytes | None: ...  # type: ignore # issue: https://github.com/confluentinc/confluent-kafka-python/issues/1631
 
-class AvroDeserializer(Deserializer):
+class JSONDeserializer(Deserializer):
     def __init__(
         self,
-        schema_registry_client: SchemaRegistryClient,
-        schema_str: str | Schema | None = None,
+        schema_str: str | Schema,
         from_dict: Callable[[dict[Any, Any], SerializationContext], object] | None = None,
-        return_record_name: bool = False,
+        schema_registry_client: SchemaRegistryClient | None = None,
     ) -> None: ...
-    def __call__(self, data: bytes, ctx: SerializationContext) -> None: ...  # type: ignore # issue: https://github.com/confluentinc/confluent-kafka-python/issues/1631
+    def __call__(self, data: bytes, ctx: SerializationContext) -> object | dict | None: ...  # type: ignore # issue: https://github.com/confluentinc/confluent-kafka-python/issues/1631
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/json_schema.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/avro.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,39 +2,44 @@
 types-confluent-kafka: A package providing type hints for the confluent-kafka Python package.
 This package is licensed under the Apache 2.0 License.
 """
 from __future__ import annotations
 
 # standard library
 from io import BytesIO
-from typing import Callable
+from typing import TYPE_CHECKING, Any, Callable
 
-from ..schema_registry import Schema as Schema
-from ..schema_registry import topic_subject_name_strategy as topic_subject_name_strategy
-from ..schema_registry.schema_registry_client import SchemaRegistryClient
 from ..serialization import Deserializer as Deserializer
 from ..serialization import SerializationContext
 from ..serialization import SerializationError as SerializationError
 from ..serialization import Serializer as Serializer
+from . import Schema as Schema
+from . import topic_subject_name_strategy as topic_subject_name_strategy
+from .schema_registry_client import SchemaRegistryClient
+
+if TYPE_CHECKING:
+    # pypi/conda library
+    from fastavro.types import AvroMessage as AvroMessage
 
 class _ContextStringIO(BytesIO):
     def __enter__(self) -> _ContextStringIO: ...
     def __exit__(self, *args): ...
 
-class JSONSerializer(Serializer):
+class AvroSerializer(Serializer):
     def __init__(
         self,
-        schema_str: str | Schema,
         schema_registry_client: SchemaRegistryClient,
-        to_dict: Callable[[object], SerializationContext] | None = None,
+        schema_str: str | Schema,
+        to_dict: Callable[[object, SerializationContext], dict[Any, Any]] | None = None,
         conf: dict | None = None,
     ) -> None: ...
-    def __call__(self, obj: object, ctx: SerializationContext): ...  # type: ignore # issue: https://github.com/confluentinc/confluent-kafka-python/issues/1631
+    def __call__(self, obj: object, ctx: SerializationContext) -> bytes | None: ...  # type: ignore # issue: https://github.com/confluentinc/confluent-kafka-python/issues/1631
 
-class JSONDeserializer(Deserializer):
+class AvroDeserializer(Deserializer):
     def __init__(
         self,
-        schema_str: str | Schema,
-        from_dict: Callable[[dict], SerializationContext] | None = ...,
-        schema_registry_client: SchemaRegistryClient | None = None,
+        schema_registry_client: SchemaRegistryClient,
+        schema_str: str | Schema | None = None,
+        from_dict: Callable[[dict[Any, Any], SerializationContext], object] | None = None,
+        return_record_name: bool = False,
     ) -> None: ...
-    def __call__(self, data: bytes, ctx: SerializationContext): ...  # type: ignore # issue: https://github.com/confluentinc/confluent-kafka-python/issues/1631
+    def __call__(self, data: bytes, ctx: SerializationContext) -> "AvroMessage | dict | None": ...  # type: ignore # issue: https://github.com/confluentinc/confluent-kafka-python/issues/1631
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/protobuf.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/protobuf.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/schema_registry/schema_registry_client.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/schema_registry/schema_registry_client.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 This package is licensed under the Apache 2.0 License.
 """
 from __future__ import annotations
 
 # standard library
 from logging import Logger
 from threading import Lock
-from typing import ClassVar, DefaultDict, Literal
+from typing import DefaultDict, Literal
 
 # pypi/conda library
 from requests import Session
 
 from .error import SchemaRegistryError as SchemaRegistryError
 
 log: Logger
 VALID_AUTH_PROVIDERS: Literal["URL", "USER_INFO"]
 
 class _RestClient:
     session: Session
-    base_url: ClassVar[str]
+    base_url: str
 
     def __init__(self, conf: dict) -> None: ...
     def get(self, url: str, query: dict | None = ...): ...
     def post(self, url: str, body, **kwargs): ...
     def delete(self, url: str): ...
     def put(self, url: str, body: str | None = None): ...
     def send_request(
@@ -31,17 +31,17 @@
         url: str,
         method: Literal["GET", "POST", "DELETE", "PUT"],
         body: str | None = None,
         query: dict | None = None,
     ): ...
 
 class _SchemaCache:
-    lock: ClassVar[Lock]
-    schema_id_index: ClassVar[dict]
-    schema_index: ClassVar[dict]
+    lock: Lock
+    schema_id_index: dict
+    schema_index: dict
     subject_schemas: DefaultDict[str, set]
 
     def __init__(self) -> None: ...
     def set(self, schema_id: int, schema: Schema, subject_name: str | None = None) -> None: ...
     def get_schema(self, schema_id: int) -> Schema | None: ...
     def get_schema_id_by_subject(self, subject, schema: Schema) -> Schema | None: ...
 
@@ -64,29 +64,29 @@
         self,
         subject_name: str,
         schema: Schema,
         version: int | Literal["latest"] = "latest",
     ) -> bool: ...
 
 class Schema:
-    schema_str: ClassVar[str]
-    schema_type: ClassVar[str]
-    references: ClassVar[list[SchemaReference]]
+    schema_str: str
+    schema_type: str
+    references: list[SchemaReference]
 
     def __init__(self, schema_str: str, schema_type: str, references: list[SchemaReference] | None = None) -> None: ...
     def __eq__(self, other) -> bool: ...
     def __hash__(self) -> int: ...
 
 class RegisteredSchema:
-    schema_id: ClassVar[int]
-    schema: ClassVar[Schema]
-    subject: ClassVar[str]
-    version: ClassVar[int]
+    schema_id: int
+    schema: Schema
+    subject: str
+    version: int
 
     def __init__(self, schema_id: int, schema: Schema, subject: str, version: int) -> None: ...
 
 class SchemaReference:
-    name: ClassVar[str]
-    subject: ClassVar[str]
-    version: ClassVar[str]
+    name: str
+    subject: str
+    version: str
 
     def __init__(self, name: str, subject: str, version: str) -> None: ...
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/serialization/__init__.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/serialization/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -20,35 +20,35 @@
     headers: ClassVar[str]
 
     def __init__(self, topic: str, field: str, headers: list[tuple] | None = None) -> None: ...
 
 class SerializationError(KafkaException): ...
 
 class Serializer:
-    def __call__(self, obj: object, ctx: SerializationContext | None = None) -> None: ...
+    def __call__(self, obj: object, ctx: SerializationContext | None = None) -> bytes | None: ...
 
 class Deserializer:
-    def __call__(self, value: bytes, ctx: SerializationContext | None = None) -> None: ...
+    def __call__(self, value: bytes | None, ctx: SerializationContext | None = None) -> object: ...
 
 class DoubleSerializer(Serializer):
-    def __call__(self, obj: object, ctx: SerializationContext | None = None) -> None: ...
+    def __call__(self, obj: object, ctx: SerializationContext | None = None) -> bytes | None: ...
 
 class DoubleDeserializer(Deserializer):
-    def __call__(self, value: bytes, ctx: SerializationContext | None = None) -> None: ...
+    def __call__(self, value: bytes | None, ctx: SerializationContext | None = None) -> float | None: ...
 
 class IntegerSerializer(Serializer):
-    def __call__(self, obj, ctx: SerializationContext | None = None) -> None: ...
+    def __call__(self, obj: object, ctx: SerializationContext | None = None) -> bytes | None: ...
 
 class IntegerDeserializer(Deserializer):
-    def __call__(self, value: bytes, ctx: SerializationContext | None = None) -> None: ...
+    def __call__(self, value: bytes | None, ctx: SerializationContext | None = None) -> int | None: ...
 
 class StringSerializer(Serializer):
-    codec: ClassVar[str]
+    codec: str
 
     def __init__(self, codec: str = ...) -> None: ...
-    def __call__(self, obj: object, ctx: SerializationContext | None = None) -> None: ...
+    def __call__(self, obj: object, ctx: SerializationContext | None = None) -> bytes | None: ...
 
 class StringDeserializer(Deserializer):
-    codec: ClassVar[str]
+    codec: str
 
     def __init__(self, codec: str = "utf_8") -> None: ...
-    def __call__(self, value: bytes, ctx: SerializationContext | None = None) -> None: ...
+    def __call__(self, value: bytes | None, ctx: SerializationContext | None = None) -> str | None: ...
```

### Comparing `types_confluent_kafka-1.2.0/confluent_kafka-stubs/serializing_producer.pyi` & `types_confluent_kafka-1.2.1/confluent_kafka-stubs/serializing_producer.pyi`

 * *Files identical despite different names*

### Comparing `types_confluent_kafka-1.2.0/pyproject.toml` & `types_confluent_kafka-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "types-confluent-kafka"
-version = "1.2.0"
+version = "1.2.1"
 description = ""
 authors = ["benbenbang <bn@bitbrew.dev>"]
 license = "Apache-2.0 license"
 readme = "README.md"
 repository = "https://github.com/benbenbang/types-confluent-kafka"
 packages = [
     { include = "confluent_kafka-stubs" }
```

### Comparing `types_confluent_kafka-1.2.0/PKG-INFO` & `types_confluent_kafka-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-confluent-kafka
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
 Home-page: https://github.com/benbenbang/types-confluent-kafka
 License: Apache-2.0 license
 Keywords: types,typings,stubs,confluent_kafka,mypy,lsp,completion,type hints,type checking
 Author: benbenbang
 Author-email: bn@bitbrew.dev
 Requires-Python: >=3.8,<4.0
```

