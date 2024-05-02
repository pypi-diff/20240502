# Comparing `tmp/atoti_kafka-0.8.8-py3-none-any.whl.zip` & `tmp/atoti_kafka-0.8.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6265591 bytes, number of entries: 9
+Zip file size: 6265587 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      130 b- defN 80-Jan-01 00:00 atoti_kafka/__init__.py
 -rw-r--r--  2.0 unx      672 b- defN 80-Jan-01 00:00 atoti_kafka/_plugin.py
--rw-r--r--  2.0 unx     1823 b- defN 80-Jan-01 00:00 atoti_kafka/_source.py
--rw-r--r--  2.0 unx  6572320 b- defN 80-Jan-01 00:00 atoti_kafka/data/atoti-kafka.jar
+-rw-r--r--  2.0 unx     1803 b- defN 80-Jan-01 00:00 atoti_kafka/_source.py
+-rw-r--r--  2.0 unx  6572338 b- defN 80-Jan-01 00:00 atoti_kafka/data/atoti-kafka.jar
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 atoti_kafka/py.typed
--rw-r--r--  2.0 unx     1039 b- defN 80-Jan-01 00:00 atoti_kafka-0.8.8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 atoti_kafka-0.8.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 80-Jan-01 00:00 atoti_kafka-0.8.8.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      719 b- defN 16-Jan-01 00:00 atoti_kafka-0.8.8.dist-info/RECORD
-9 files, 6576846 bytes uncompressed, 6264353 bytes compressed:  4.8%
+-rw-r--r--  2.0 unx     1039 b- defN 80-Jan-01 00:00 atoti_kafka-0.8.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 atoti_kafka-0.8.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 80-Jan-01 00:00 atoti_kafka-0.8.9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      719 b- defN 16-Jan-01 00:00 atoti_kafka-0.8.9.dist-info/RECORD
+9 files, 6576844 bytes uncompressed, 6264349 bytes compressed:  4.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: atoti_kafka/data/atoti-kafka.jar
 Comment: 
 
 Filename: atoti_kafka/py.typed
 Comment: 
 
-Filename: atoti_kafka-0.8.8.dist-info/METADATA
+Filename: atoti_kafka-0.8.9.dist-info/METADATA
 Comment: 
 
-Filename: atoti_kafka-0.8.8.dist-info/WHEEL
+Filename: atoti_kafka-0.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: atoti_kafka-0.8.8.dist-info/entry_points.txt
+Filename: atoti_kafka-0.8.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: atoti_kafka-0.8.8.dist-info/RECORD
+Filename: atoti_kafka-0.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atoti_kafka/_source.py

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
-from typing import Any
 
 from atoti._java_api import JavaApi
 from atoti._sources.data_source import DataSource
 from atoti_core import TableIdentifier
 from typing_extensions import override
 
 
@@ -23,15 +22,15 @@
         topic: str,
         group_id: str,
         batch_duration: int,
         consumer_config: Mapping[str, str],
         scenario_name: str,
     ) -> None:
         """Consume a Kafka topic and stream its records in an existing table."""
-        params: dict[str, Any] = {
+        params: dict[str, object] = {
             "bootstrapServers": bootstrap_servers,
             "topic": topic,
             "consumerGroupId": group_id,
             "keyDeserializerClass": "org.apache.kafka.common.serialization.StringDeserializer",
             "batchDuration": batch_duration,
             "additionalParameters": consumer_config,
         }
```

## atoti_kafka/data/atoti-kafka.jar

### zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6572320 bytes, number of entries: 2014
--rw-r--r--  2.0 unx       60 b- defN 24-Jan-05 14:28 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-05 14:28 META-INF/
+Zip file size: 6572338 bytes, number of entries: 2014
+-rw-r--r--  2.0 unx       60 b- defN 24-Feb-01 15:30 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-01 15:30 META-INF/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Dec-10 19:31 org/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Dec-10 19:31 org/apache/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Dec-10 19:31 org/apache/kafka/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Dec-10 19:31 org/apache/kafka/clients/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Dec-10 19:31 org/apache/kafka/clients/producer/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Dec-10 19:31 org/apache/kafka/clients/producer/internals/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Dec-10 19:31 org/apache/kafka/clients/admin/
@@ -117,22 +117,22 @@
 drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-08 13:31 org/slf4j/
 drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-08 13:31 org/slf4j/event/
 drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-08 13:31 org/slf4j/helpers/
 drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-08 13:31 org/slf4j/spi/
 drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-08 13:31 META-INF/maven/
 drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-08 13:31 META-INF/maven/org.slf4j/
 drwxr-xr-x  2.0 unx        0 b- stor 22-Feb-08 13:31 META-INF/maven/org.slf4j/slf4j-api/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-05 14:18 io/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-05 14:18 io/atoti/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-05 14:18 io/atoti/loading/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-05 14:28 io/atoti/loading/kafka/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-05 14:28 io/atoti/loading/kafka/impl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-05 14:28 io/atoti/loading/kafka/impl/serialization/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-05 14:28 META-INF/maven/io.atoti/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-05 14:28 META-INF/maven/io.atoti/kafka-source/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-01 15:20 io/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-01 15:20 io/atoti/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-01 15:20 io/atoti/loading/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-01 15:30 io/atoti/loading/kafka/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-01 15:30 io/atoti/loading/kafka/impl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-01 15:30 io/atoti/loading/kafka/impl/serialization/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-01 15:30 META-INF/maven/io.atoti/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-01 15:30 META-INF/maven/io.atoti/kafka-source/
 -rw-r--r--  2.0 unx     3383 b- defN 20-Dec-10 19:31 org/apache/kafka/clients/ClusterConnectionStates$NodeConnectionState.class
 -rw-r--r--  2.0 unx    19286 b- defN 20-Dec-10 19:31 org/apache/kafka/clients/Metadata.class
 -rw-r--r--  2.0 unx     9418 b- defN 20-Dec-10 19:31 org/apache/kafka/clients/FetchSessionHandler.class
 -rw-r--r--  2.0 unx    35231 b- defN 20-Dec-10 19:31 org/apache/kafka/clients/NetworkClient.class
 -rw-r--r--  2.0 unx     2242 b- defN 20-Dec-10 19:31 org/apache/kafka/clients/ApiVersions.class
 -rw-r--r--  2.0 unx    28083 b- defN 20-Dec-10 19:31 org/apache/kafka/clients/producer/ProducerConfig.class
 -rw-r--r--  2.0 unx    17445 b- defN 20-Dec-10 19:31 org/apache/kafka/clients/producer/MockProducer.class
@@ -1998,19 +1998,19 @@
 -rw-r--r--  2.0 unx     2952 b- defN 22-Feb-08 13:31 org/slf4j/helpers/Util.class
 -rw-r--r--  2.0 unx      455 b- defN 22-Feb-08 13:31 org/slf4j/spi/LocationAwareLogger.class
 -rw-r--r--  2.0 unx      249 b- defN 22-Feb-08 13:31 org/slf4j/spi/LoggerFactoryBinder.class
 -rw-r--r--  2.0 unx      529 b- defN 22-Feb-08 13:31 org/slf4j/spi/MDCAdapter.class
 -rw-r--r--  2.0 unx      249 b- defN 22-Feb-08 13:31 org/slf4j/spi/MarkerFactoryBinder.class
 -rw-r--r--  2.0 unx     2743 b- defN 22-Feb-08 13:31 META-INF/maven/org.slf4j/slf4j-api/pom.xml
 -rw-r--r--  2.0 unx       57 b- defN 22-Feb-08 13:31 META-INF/maven/org.slf4j/slf4j-api/pom.properties
--rw-r--r--  2.0 unx     1532 b- defN 24-Jan-05 14:28 io/atoti/loading/kafka/impl/serialization/KafkaDeserializer.class
--rw-r--r--  2.0 unx     4632 b- defN 24-Jan-05 14:28 io/atoti/loading/kafka/impl/serialization/JsonDeserializer.class
--rw-r--r--  2.0 unx     5193 b- defN 24-Jan-05 14:28 io/atoti/loading/kafka/impl/KafkaDataTable.class
--rw-r--r--  2.0 unx     2328 b- defN 24-Jan-05 14:28 io/atoti/loading/kafka/impl/KafkaConsumerProperties.class
--rw-r--r--  2.0 unx     2162 b- defN 24-Jan-05 14:28 io/atoti/loading/kafka/impl/KafkaThreadManager.class
--rw-r--r--  2.0 unx     6941 b- defN 24-Jan-05 14:28 io/atoti/loading/kafka/impl/KafkaRunnable.class
--rw-r--r--  2.0 unx     4066 b- defN 24-Jan-05 14:28 io/atoti/loading/kafka/impl/KafkaLoaderParams.class
--rw-r--r--  2.0 unx     2682 b- defN 24-Jan-05 14:28 io/atoti/loading/kafka/impl/KafkaDataTableFactory.class
--rw-r--r--  2.0 unx      527 b- defN 24-Jan-05 14:28 io/atoti/loading/kafka/KafkaPlugin.class
--rw-r--r--  2.0 unx     3509 b- defN 24-Jan-05 14:10 META-INF/maven/io.atoti/kafka-source/pom.xml
--rw-r--r--  2.0 unx       72 b- defN 24-Jan-05 14:18 META-INF/maven/io.atoti/kafka-source/pom.properties
-2014 files, 16297396 bytes uncompressed, 6178646 bytes compressed:  62.1%
+-rw-r--r--  2.0 unx     1532 b- defN 24-Feb-01 15:30 io/atoti/loading/kafka/impl/serialization/KafkaDeserializer.class
+-rw-r--r--  2.0 unx     4644 b- defN 24-Feb-01 15:30 io/atoti/loading/kafka/impl/serialization/JsonDeserializer.class
+-rw-r--r--  2.0 unx     5193 b- defN 24-Feb-01 15:30 io/atoti/loading/kafka/impl/KafkaDataTable.class
+-rw-r--r--  2.0 unx     2324 b- defN 24-Feb-01 15:30 io/atoti/loading/kafka/impl/KafkaConsumerProperties.class
+-rw-r--r--  2.0 unx     2162 b- defN 24-Feb-01 15:30 io/atoti/loading/kafka/impl/KafkaThreadManager.class
+-rw-r--r--  2.0 unx     6941 b- defN 24-Feb-01 15:30 io/atoti/loading/kafka/impl/KafkaRunnable.class
+-rw-r--r--  2.0 unx     4082 b- defN 24-Feb-01 15:30 io/atoti/loading/kafka/impl/KafkaLoaderParams.class
+-rw-r--r--  2.0 unx     2682 b- defN 24-Feb-01 15:30 io/atoti/loading/kafka/impl/KafkaDataTableFactory.class
+-rw-r--r--  2.0 unx      527 b- defN 24-Feb-01 15:30 io/atoti/loading/kafka/KafkaPlugin.class
+-rw-r--r--  2.0 unx     3509 b- defN 24-Feb-01 15:10 META-INF/maven/io.atoti/kafka-source/pom.xml
+-rw-r--r--  2.0 unx       72 b- defN 24-Feb-01 15:20 META-INF/maven/io.atoti/kafka-source/pom.properties
+2014 files, 16297420 bytes uncompressed, 6178664 bytes compressed:  62.1%
```

### io/atoti/loading/kafka/impl/serialization/KafkaDeserializer.class

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum ef673ef24ca0f9a44d6237937d304a078473017a5d8d373ed8c9289babdbf7d0
+  SHA-256 checksum afc5d707d2f99eb6f88b56505040f3bbc3a605069cebb3bb301263127dded962
   Compiled from "KafkaDeserializer.java"
 public final class io.atoti.loading.kafka.impl.serialization.KafkaDeserializer extends java.lang.Enum<io.atoti.loading.kafka.impl.serialization.KafkaDeserializer>
   minor version: 0
   major version: 55
   flags: (0x4031) ACC_PUBLIC, ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #1                          // io/atoti/loading/kafka/impl/serialization/KafkaDeserializer
   super_class: #17                        // java/lang/Enum
@@ -87,28 +87,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #7                  // Field $VALUES:[Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;
          3: invokevirtual #11                 // Method "[Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;".clone:()Ljava/lang/Object;
          6: checkcast     #12                 // class "[Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;"
          9: areturn
       LineNumberTable:
-        line 6: 0
+        line 4: 0
 
   public static io.atoti.loading.kafka.impl.serialization.KafkaDeserializer valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #1                  // class io/atoti/loading/kafka/impl/serialization/KafkaDeserializer
          2: aload_0
          3: invokestatic  #16                 // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #1                  // class io/atoti/loading/kafka/impl/serialization/KafkaDeserializer
          9: areturn
       LineNumberTable:
-        line 6: 0
+        line 4: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
 
   private io.atoti.loading.kafka.impl.serialization.KafkaDeserializer(java.lang.String);
     descriptor: (Ljava/lang/String;ILjava/lang/String;)V
     flags: (0x0002) ACC_PRIVATE
@@ -119,17 +119,17 @@
          2: iload_2
          3: invokespecial #22                 // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: aload_0
          7: aload_3
          8: putfield      #26                 // Field className:Ljava/lang/String;
         11: return
       LineNumberTable:
-        line 12: 0
-        line 13: 6
-        line 14: 11
+        line 9: 0
+        line 10: 6
+        line 11: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;
             0      12     3 className   Ljava/lang/String;
     Signature: #54                          // (Ljava/lang/String;)V
 
   public java.lang.String getClassName();
@@ -137,15 +137,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #26                 // Field className:Ljava/lang/String;
          4: areturn
       LineNumberTable:
-        line 22: 0
+        line 19: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;
 
   private static io.atoti.loading.kafka.impl.serialization.KafkaDeserializer[] $values();
     descriptor: ()[Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;
     flags: (0x100a) ACC_PRIVATE, ACC_STATIC, ACC_SYNTHETIC
@@ -155,15 +155,15 @@
          1: anewarray     #1                  // class io/atoti/loading/kafka/impl/serialization/KafkaDeserializer
          4: dup
          5: iconst_0
          6: getstatic     #3                  // Field JSON_DESERIALIZER:Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;
          9: aastore
         10: areturn
       LineNumberTable:
-        line 6: 0
+        line 4: 0
 
   static {};
     descriptor: ()V
     flags: (0x0008) ACC_STATIC
     Code:
       stack=5, locals=0, args_size=0
          0: new           #1                  // class io/atoti/loading/kafka/impl/serialization/KafkaDeserializer
@@ -174,12 +174,12 @@
          9: invokevirtual #33                 // Method java/lang/Class.getName:()Ljava/lang/String;
         12: invokespecial #39                 // Method "<init>":(Ljava/lang/String;ILjava/lang/String;)V
         15: putstatic     #3                  // Field JSON_DESERIALIZER:Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;
         18: invokestatic  #42                 // Method $values:()[Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;
         21: putstatic     #7                  // Field $VALUES:[Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;
         24: return
       LineNumberTable:
-        line 8: 0
-        line 6: 18
+        line 5: 0
+        line 4: 18
 }
 Signature: #58                          // Ljava/lang/Enum<Lio/atoti/loading/kafka/impl/serialization/KafkaDeserializer;>;
 SourceFile: "KafkaDeserializer.java"
```

### io/atoti/loading/kafka/impl/serialization/JsonDeserializer.class

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 05fc64e556aacdff6d0ffeb1030f0e297b8dc4bc9a3d93e74c4f9f5ab719502f
+  SHA-256 checksum 38fb069ff4579b771695b03e3172ec3fbb73f223cb8befc71ea8f449963aa2e3
   Compiled from "JsonDeserializer.java"
 public class io.atoti.loading.kafka.impl.serialization.JsonDeserializer extends java.lang.Object implements org.apache.kafka.common.serialization.Deserializer<java.lang.String[]>
   minor version: 0
   major version: 55
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #20                         // io/atoti/loading/kafka/impl/serialization/JsonDeserializer
   super_class: #2                         // java/lang/Object
@@ -210,15 +210,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 19: 0
+        line 20: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lio/atoti/loading/kafka/impl/serialization/JsonDeserializer;
 
   public void configure(java.util.Map<java.lang.String, ?>, boolean);
     descriptor: (Ljava/util/Map;Z)V
     flags: (0x0001) ACC_PUBLIC
@@ -238,19 +238,21 @@
         28: invokeinterface #34,  2           // InterfaceMethod java/util/stream/Stream.map:(Ljava/util/function/Function;)Ljava/util/stream/Stream;
         33: invokestatic  #40                 // Method java/util/stream/Collectors.toSet:()Ljava/util/stream/Collector;
         36: invokeinterface #46,  2           // InterfaceMethod java/util/stream/Stream.collect:(Ljava/util/stream/Collector;)Ljava/lang/Object;
         41: checkcast     #50                 // class java/util/Set
         44: putfield      #52                 // Field datastoreColumns:Ljava/util/Set;
         47: return
       LineNumberTable:
-        line 26: 0
-        line 27: 15
-        line 28: 28
-        line 29: 33
-        line 30: 47
+        line 27: 0
+        line 28: 4
+        line 29: 15
+        line 30: 20
+        line 31: 28
+        line 32: 33
+        line 33: 47
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      48     0  this   Lio/atoti/loading/kafka/impl/serialization/JsonDeserializer;
             0      48     1 configs   Ljava/util/Map;
             0      48     2 isKey   Z
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -321,26 +323,27 @@
        132: aload_3
        133: invokespecial #107                // Method com/activeviam/fwk/ActiveViamRuntimeException."<init>":(Ljava/lang/String;Ljava/lang/Throwable;)V
        136: athrow
       Exception table:
          from    to  target type
              0   120   121   Class java/io/IOException
       LineNumberTable:
-        line 35: 0
-        line 37: 4
-        line 39: 16
-        line 40: 35
-        line 42: 43
-        line 44: 62
-        line 45: 72
-        line 46: 85
-        line 45: 112
-        line 48: 118
-        line 49: 121
-        line 50: 122
+        line 38: 0
+        line 40: 4
+        line 42: 16
+        line 43: 35
+        line 45: 43
+        line 47: 48
+        line 49: 62
+        line 50: 72
+        line 51: 85
+        line 50: 112
+        line 53: 118
+        line 54: 121
+        line 55: 122
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            75      43     6     j   I
             4     117     3 mapper   Lcom/fasterxml/jackson/databind/ObjectMapper;
            16     105     4 jsonMap   Ljava/util/Map;
            72      49     5   row   [Ljava/lang/String;
           122      15     3     e   Ljava/io/IOException;
@@ -371,30 +374,30 @@
       stack=3, locals=4, args_size=4
          0: aload_0
          1: aload_1
          2: aload_3
          3: invokevirtual #110                // Method deserialize:(Ljava/lang/String;[B)[Ljava/lang/String;
          6: areturn
       LineNumberTable:
-        line 56: 0
+        line 61: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lio/atoti/loading/kafka/impl/serialization/JsonDeserializer;
             0       7     1 topic   Ljava/lang/String;
             0       7     2 headers   Lorg/apache/kafka/common/header/Headers;
             0       7     3  data   [B
 
   public void close();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=0, locals=1, args_size=1
          0: return
       LineNumberTable:
-        line 61: 0
+        line 65: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       1     0  this   Lio/atoti/loading/kafka/impl/serialization/JsonDeserializer;
 
   public java.lang.Object deserialize(java.lang.String, org.apache.kafka.common.header.Headers, byte[]);
     descriptor: (Ljava/lang/String;Lorg/apache/kafka/common/header/Headers;[B)Ljava/lang/Object;
     flags: (0x1041) ACC_PUBLIC, ACC_BRIDGE, ACC_SYNTHETIC
@@ -403,15 +406,15 @@
          0: aload_0
          1: aload_1
          2: aload_2
          3: aload_3
          4: invokevirtual #114                // Method deserialize:(Ljava/lang/String;Lorg/apache/kafka/common/header/Headers;[B)[Ljava/lang/String;
          7: areturn
       LineNumberTable:
-        line 19: 0
+        line 20: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lio/atoti/loading/kafka/impl/serialization/JsonDeserializer;
 
   public java.lang.Object deserialize(java.lang.String, byte[]);
     descriptor: (Ljava/lang/String;[B)Ljava/lang/Object;
     flags: (0x1041) ACC_PUBLIC, ACC_BRIDGE, ACC_SYNTHETIC
@@ -419,15 +422,15 @@
       stack=3, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: aload_2
          3: invokevirtual #110                // Method deserialize:(Ljava/lang/String;[B)[Ljava/lang/String;
          6: areturn
       LineNumberTable:
-        line 19: 0
+        line 20: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lio/atoti/loading/kafka/impl/serialization/JsonDeserializer;
 }
 Signature: #157                         // Ljava/lang/Object;Lorg/apache/kafka/common/serialization/Deserializer<[Ljava/lang/String;>;
 SourceFile: "JsonDeserializer.java"
 BootstrapMethods:
```

### io/atoti/loading/kafka/impl/KafkaDataTable.class

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum dc012b0ed33a68596a832309adc6ec6008555742c1156ec5143c60dbc6285b63
+  SHA-256 checksum 420f053948589d83b8b92fcf6acdf2b829a853e8b567c4c6d01186ac37df7111
   Compiled from "KafkaDataTable.java"
 public class io.atoti.loading.kafka.impl.KafkaDataTable extends io.atoti.loading.impl.ADataTable implements io.atoti.loading.RealTimeDataTable
   minor version: 0
   major version: 55
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #8                          // io/atoti/loading/kafka/impl/KafkaDataTable
   super_class: #2                         // io/atoti/loading/impl/ADataTable
@@ -276,22 +276,22 @@
         68: invokedynamic #53,  0             // InvokeDynamic #0:accept:(Lio/atoti/loading/kafka/impl/KafkaDataTable;)Ljava/util/function/Consumer;
         73: aload_0
         74: invokedynamic #57,  0             // InvokeDynamic #1:accept:(Lio/atoti/loading/kafka/impl/KafkaDataTable;)Ljava/util/function/Consumer;
         79: invokespecial #58                 // Method io/atoti/loading/kafka/impl/KafkaThreadManager."<init>":(Lio/atoti/loading/kafka/impl/KafkaConsumerProperties;Ljava/util/function/Consumer;Ljava/util/function/Consumer;)V
         82: putfield      #61                 // Field kafkaThreadManager:Lio/atoti/loading/kafka/impl/KafkaThreadManager;
         85: return
       LineNumberTable:
-        line 42: 0
-        line 43: 7
-        line 44: 13
-        line 45: 26
-        line 46: 34
-        line 47: 46
-        line 48: 58
-        line 50: 85
+        line 40: 0
+        line 41: 7
+        line 42: 13
+        line 43: 26
+        line 44: 34
+        line 45: 46
+        line 46: 58
+        line 48: 85
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      86     0  this   Lio/atoti/loading/kafka/impl/KafkaDataTable;
             0      86     1 manager   Lio/atoti/DataManager;
             0      86     2 storeToFeed   Ljava/lang/String;
             0      86     3 loadingParams   Lio/atoti/loading/impl/LoadingParams;
             0      86     4 kafkaConsumerParams   Lio/atoti/loading/kafka/impl/KafkaConsumerProperties;
@@ -300,47 +300,47 @@
   protected void init();
     descriptor: ()V
     flags: (0x0004) ACC_PROTECTED
     Code:
       stack=0, locals=1, args_size=1
          0: return
       LineNumberTable:
-        line 54: 0
+        line 51: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       1     0  this   Lio/atoti/loading/kafka/impl/KafkaDataTable;
 
   public void startRealTime();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #61                 // Field kafkaThreadManager:Lio/atoti/loading/kafka/impl/KafkaThreadManager;
          4: invokevirtual #65                 // Method io/atoti/loading/kafka/impl/KafkaThreadManager.start:()V
          7: return
       LineNumberTable:
-        line 58: 0
-        line 59: 7
+        line 55: 0
+        line 56: 7
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lio/atoti/loading/kafka/impl/KafkaDataTable;
 
   public void stopRealTime();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #61                 // Field kafkaThreadManager:Lio/atoti/loading/kafka/impl/KafkaThreadManager;
          4: invokevirtual #69                 // Method io/atoti/loading/kafka/impl/KafkaThreadManager.stop:()V
          7: return
       LineNumberTable:
-        line 63: 0
-        line 64: 7
+        line 60: 0
+        line 61: 7
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lio/atoti/loading/kafka/impl/KafkaDataTable;
 
   private void loadWithTransactions(java.lang.String[][]);
     descriptor: ([[Ljava/lang/String;)V
     flags: (0x0002) ACC_PRIVATE
@@ -389,23 +389,23 @@
         85: iconst_1
         86: anewarray     #123                // class com/qfs/condition/ICondition
         89: invokeinterface #125,  4          // InterfaceMethod com/qfs/store/service/IDatabaseService.editDatabase:(Ljava/lang/String;Lcom/qfs/pivot/json/database/JsonDatabaseEdit;[Lcom/qfs/condition/ICondition;)Ljava/util/Map;
         94: pop
         95: goto          38
         98: return
       LineNumberTable:
-        line 67: 0
-        line 68: 8
-        line 69: 15
-        line 70: 20
-        line 71: 28
-        line 72: 58
-        line 73: 77
-        line 74: 95
-        line 75: 98
+        line 64: 0
+        line 65: 8
+        line 66: 15
+        line 67: 20
+        line 68: 28
+        line 69: 58
+        line 71: 77
+        line 72: 95
+        line 73: 98
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            77      18     5  edit   Lcom/qfs/pivot/json/database/JsonDatabaseEdit;
            58      37     4 branch   Ljava/lang/String;
             0      99     0  this   Lio/atoti/loading/kafka/impl/KafkaDataTable;
             0      99     1  data   [[Ljava/lang/String;
             8      91     2 action   Lcom/qfs/pivot/json/database/JsonDatabaseAction;
@@ -428,16 +428,16 @@
         14: aload_0
         15: getfield      #27                 // Field storeToFeed:Ljava/lang/String;
         18: aload_1
         19: invokevirtual #139                // Method io/atoti/loading/report/LoadingReports.addReport:(Ljava/lang/String;Lio/atoti/loading/report/SingleLoadingReport;)I
         22: pop
         23: return
       LineNumberTable:
-        line 78: 0
-        line 79: 23
+        line 76: 0
+        line 77: 23
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      24     0  this   Lio/atoti/loading/kafka/impl/KafkaDataTable;
             0      24     1 report   Lio/atoti/loading/report/SingleLoadingReport;
 
   public void loadWithinTransaction(com.qfs.store.transaction.impl.TransactionPerformer, java.lang.String);
     descriptor: (Lcom/qfs/store/transaction/impl/TransactionPerformer;Ljava/lang/String;)V
@@ -446,15 +446,15 @@
       stack=3, locals=3, args_size=3
          0: new           #145                // class com/activeviam/fwk/ActiveViamRuntimeException
          3: dup
          4: ldc           #147                // String The loading of a Kafka stream cannot be part of a transaction
          6: invokespecial #149                // Method com/activeviam/fwk/ActiveViamRuntimeException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 83: 0
+        line 82: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lio/atoti/loading/kafka/impl/KafkaDataTable;
             0      10     1 transactionPerformer   Lcom/qfs/store/transaction/impl/TransactionPerformer;
             0      10     2 branch   Ljava/lang/String;
 }
 SourceFile: "KafkaDataTable.java"
```

### io/atoti/loading/kafka/impl/KafkaConsumerProperties.class

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 3225025cd314de7af68d03ba106d5e43252e4c1b05c45e5cb7d55f9ce96afeeb
+  SHA-256 checksum 33f472ac8653a0c6db35f0d20390abed9c77996f59eba7f4ddaf78c1e094945a
   Compiled from "KafkaConsumerProperties.java"
 public class io.atoti.loading.kafka.impl.KafkaConsumerProperties extends java.util.Properties
   minor version: 0
   major version: 55
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #8                          // io/atoti/loading/kafka/impl/KafkaConsumerProperties
   super_class: #2                         // java/util/Properties
@@ -112,15 +112,14 @@
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/util/Properties."<init>":()V
          4: return
       LineNumberTable:
         line 18: 0
-        line 19: 4
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lio/atoti/loading/kafka/impl/KafkaConsumerProperties;
 
   public io.atoti.loading.kafka.impl.KafkaConsumerProperties(java.lang.String, java.lang.String, java.lang.String, java.lang.String, int, java.util.Map<java.lang.String, java.lang.String>);
     descriptor: (Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;ILjava/util/Map;)V
     flags: (0x0001) ACC_PUBLIC
@@ -160,26 +159,26 @@
         57: aload         6
         59: ifnull        68
         62: aload_0
         63: aload         6
         65: invokevirtual #47                 // Method putAll:(Ljava/util/Map;)V
         68: return
       LineNumberTable:
-        line 38: 0
-        line 39: 4
-        line 40: 9
-        line 41: 19
-        line 42: 27
-        line 43: 35
-        line 44: 44
-        line 46: 50
-        line 44: 53
-        line 47: 57
-        line 48: 62
-        line 50: 68
+        line 37: 0
+        line 38: 4
+        line 39: 9
+        line 40: 19
+        line 41: 27
+        line 42: 35
+        line 43: 44
+        line 45: 50
+        line 43: 53
+        line 46: 57
+        line 47: 62
+        line 49: 68
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      69     0  this   Lio/atoti/loading/kafka/impl/KafkaConsumerProperties;
             0      69     1 bootstrapServers   Ljava/lang/String;
             0      69     2 topic   Ljava/lang/String;
             0      69     3 consumerGroupId   Ljava/lang/String;
             0      69     4 keyDeserializerClass   Ljava/lang/String;
@@ -202,31 +201,31 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: putfield      #7                  // Field topic:Ljava/lang/String;
          5: aload_0
          6: areturn
       LineNumberTable:
-        line 59: 0
-        line 60: 5
+        line 58: 0
+        line 59: 5
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lio/atoti/loading/kafka/impl/KafkaConsumerProperties;
             0       7     1 topic   Ljava/lang/String;
 
   public java.lang.String getTopic();
     descriptor: ()Ljava/lang/String;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #7                  // Field topic:Ljava/lang/String;
          4: areturn
       LineNumberTable:
-        line 69: 0
+        line 68: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lio/atoti/loading/kafka/impl/KafkaConsumerProperties;
 
   public io.atoti.loading.kafka.impl.KafkaConsumerProperties withBatchDuration(int);
     descriptor: (I)Lio/atoti/loading/kafka/impl/KafkaConsumerProperties;
     flags: (0x0001) ACC_PUBLIC
@@ -236,29 +235,29 @@
          1: iload_1
          2: i2l
          3: invokestatic  #13                 // Method java/time/Duration.ofMillis:(J)Ljava/time/Duration;
          6: putfield      #19                 // Field batchDuration:Ljava/time/Duration;
          9: aload_0
         10: areturn
       LineNumberTable:
-        line 79: 0
-        line 80: 9
+        line 78: 0
+        line 79: 9
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lio/atoti/loading/kafka/impl/KafkaConsumerProperties;
             0      11     1 batchDuration   I
 
   public java.time.Duration getBatchDuration();
     descriptor: ()Ljava/time/Duration;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #19                 // Field batchDuration:Ljava/time/Duration;
          4: areturn
       LineNumberTable:
-        line 89: 0
+        line 88: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lio/atoti/loading/kafka/impl/KafkaConsumerProperties;
 }
 SourceFile: "KafkaConsumerProperties.java"
```

### io/atoti/loading/kafka/impl/KafkaRunnable.class

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 0b1df0a575aadeec5b5f968b19c01c007818b0615152bb5482ec4e2e75f49673
+  SHA-256 checksum 94c2b9d5e2fb30d12525bc32106c00c563e7f220f0477f2d70a83c1438bf2338
   Compiled from "KafkaRunnable.java"
 class io.atoti.loading.kafka.impl.KafkaRunnable implements java.lang.Runnable
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #13                         // io/atoti/loading/kafka/impl/KafkaRunnable
   super_class: #2                         // java/lang/Object
@@ -420,24 +420,24 @@
        134: return
       LineNumberTable:
         line 41: 0
         line 24: 4
         line 42: 16
         line 45: 26
         line 46: 33
-        line 47: 42
-        line 50: 57
-        line 51: 64
-        line 52: 73
-        line 54: 88
-        line 55: 108
-        line 56: 116
-        line 57: 124
-        line 58: 129
-        line 59: 134
+        line 48: 42
+        line 51: 57
+        line 52: 64
+        line 54: 73
+        line 56: 88
+        line 58: 108
+        line 59: 116
+        line 60: 124
+        line 61: 129
+        line 62: 134
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0     135     0  this   Lio/atoti/loading/kafka/impl/KafkaRunnable;
             0     135     1 kafkaConsumerParams   Lio/atoti/loading/kafka/impl/KafkaConsumerProperties;
             0     135     2 loadWithTransaction   Ljava/util/function/Consumer;
             0     135     3 loadReporter   Ljava/util/function/Consumer;
            26     109     4 config   Lorg/apache/kafka/clients/consumer/ConsumerConfig;
@@ -556,43 +556,43 @@
       Exception table:
          from    to  target type
              0   144   170   Class org/apache/kafka/common/errors/WakeupException
              0   144   218   any
            170   192   218   any
            218   220   218   any
       LineNumberTable:
-        line 64: 0
-        line 65: 14
-        line 66: 24
-        line 67: 28
-        line 68: 40
-        line 69: 46
-        line 70: 56
-        line 71: 80
-        line 72: 85
-        line 73: 97
-        line 75: 109
-        line 77: 121
-        line 79: 128
-        line 73: 136
-        line 82: 141
-        line 88: 144
-        line 89: 151
-        line 90: 158
-        line 83: 170
-        line 84: 171
-        line 85: 181
-        line 88: 192
-        line 89: 199
-        line 90: 206
-        line 88: 218
-        line 89: 227
-        line 90: 234
-        line 92: 243
-        line 93: 246
+        line 67: 0
+        line 68: 14
+        line 69: 24
+        line 70: 28
+        line 71: 40
+        line 72: 46
+        line 73: 56
+        line 74: 80
+        line 75: 85
+        line 76: 97
+        line 78: 109
+        line 80: 121
+        line 82: 128
+        line 76: 136
+        line 85: 141
+        line 91: 144
+        line 92: 151
+        line 93: 158
+        line 86: 170
+        line 87: 171
+        line 88: 181
+        line 91: 192
+        line 92: 199
+        line 93: 206
+        line 91: 218
+        line 92: 227
+        line 93: 234
+        line 95: 243
+        line 96: 246
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            85      56     5 endTime   J
            97      44     7 duration   J
            28     113     1 timeBeforePoll   J
            40     101     3 records   Lorg/apache/kafka/clients/consumer/ConsumerRecords;
            46      95     4 polledData   Ljava/util/List;
@@ -635,17 +635,17 @@
         12: aload_0
         13: aload_1
         14: invokedynamic #196,  0            // InvokeDynamic #2:accept:(Ljava/util/List;)Ljava/util/function/Consumer;
         19: invokevirtual #199                // Method org/apache/kafka/clients/consumer/ConsumerRecords.forEach:(Ljava/util/function/Consumer;)V
         22: aload_1
         23: areturn
       LineNumberTable:
-        line 96: 0
-        line 98: 12
-        line 99: 22
+        line 99: 0
+        line 101: 12
+        line 102: 22
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      24     0 records   Lorg/apache/kafka/clients/consumer/ConsumerRecords;
            12      12     1 polledData   Ljava/util/List;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      24     0 records   Lorg/apache/kafka/clients/consumer/ConsumerRecords<**>;
@@ -665,18 +665,18 @@
          9: getfield      #53                 // Field consumer:Lorg/apache/kafka/clients/consumer/KafkaConsumer;
         12: invokevirtual #206                // Method org/apache/kafka/clients/consumer/KafkaConsumer.wakeup:()V
         15: aload_0
         16: aload_1
         17: putfield      #168                // Field interrupt:Ljava/lang/Runnable;
         20: return
       LineNumberTable:
-        line 108: 0
-        line 109: 8
-        line 110: 15
-        line 111: 20
+        line 111: 0
+        line 112: 8
+        line 113: 15
+        line 114: 20
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      21     0  this   Lio/atoti/loading/kafka/impl/KafkaRunnable;
             0      21     1 interrupt   Ljava/lang/Runnable;
 
   private static void lambda$getRecordsValue$1(java.util.List, org.apache.kafka.clients.consumer.ConsumerRecord);
     descriptor: (Ljava/util/List;Lorg/apache/kafka/clients/consumer/ConsumerRecord;)V
@@ -687,30 +687,30 @@
          1: aload_1
          2: invokevirtual #209                // Method org/apache/kafka/clients/consumer/ConsumerRecord.value:()Ljava/lang/Object;
          5: checkcast     #215                // class "[Ljava/lang/String;"
          8: invokeinterface #217,  2          // InterfaceMethod java/util/List.add:(Ljava/lang/Object;)Z
         13: pop
         14: return
       LineNumberTable:
-        line 98: 0
+        line 101: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0 polledData   Ljava/util/List;
             0      15     1     c   Lorg/apache/kafka/clients/consumer/ConsumerRecord;
 
   private static java.lang.String[][] lambda$run$0(int);
     descriptor: (I)[[Ljava/lang/String;
     flags: (0x100a) ACC_PRIVATE, ACC_STATIC, ACC_SYNTHETIC
     Code:
       stack=1, locals=1, args_size=1
          0: iload_0
          1: anewarray     #215                // class "[Ljava/lang/String;"
          4: areturn
       LineNumberTable:
-        line 70: 0
+        line 73: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0   x$0   I
 }
 SourceFile: "KafkaRunnable.java"
 BootstrapMethods:
   0: #267 REF_invokeStatic java/lang/invoke/LambdaMetafactory.metafactory:(Ljava/lang/invoke/MethodHandles$Lookup;Ljava/lang/String;Ljava/lang/invoke/MethodType;Ljava/lang/invoke/MethodType;Ljava/lang/invoke/MethodHandle;Ljava/lang/invoke/MethodType;)Ljava/lang/invoke/CallSite;
```

### io/atoti/loading/kafka/impl/KafkaLoaderParams.class

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 51d0dde32ed3f6ab583414fe451804b3a09d68f60ae0be3483aabf7ac352996b
+  SHA-256 checksum 402f36c1260f0311c6313c8ee847171efbbee720821e2a6c706f433678275fc6
   Compiled from "KafkaLoaderParams.java"
 public class io.atoti.loading.kafka.impl.KafkaLoaderParams
   minor version: 0
   major version: 55
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #8                          // io/atoti/loading/kafka/impl/KafkaLoaderParams
   super_class: #2                         // java/lang/Object
@@ -391,16 +391,16 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: putfield      #26                 // Field additionalParameters:Ljava/util/Map;
          5: aload_0
          6: areturn
       LineNumberTable:
-        line 107: 0
-        line 108: 5
+        line 108: 0
+        line 109: 5
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lio/atoti/loading/kafka/impl/KafkaLoaderParams;
             0       7     1 additionalParameters   Ljava/util/Map;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0       7     1 additionalParameters   Ljava/util/Map<Ljava/lang/String;Ljava/lang/String;>;
@@ -411,15 +411,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #35                 // Field batchSize:I
          4: ireturn
       LineNumberTable:
-        line 112: 0
+        line 113: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lio/atoti/loading/kafka/impl/KafkaLoaderParams;
 
   public io.atoti.loading.kafka.impl.KafkaLoaderParams withBatchSize(int);
     descriptor: (I)Lio/atoti/loading/kafka/impl/KafkaLoaderParams;
     flags: (0x0001) ACC_PUBLIC
@@ -427,16 +427,16 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: iload_1
          2: putfield      #35                 // Field batchSize:I
          5: aload_0
          6: areturn
       LineNumberTable:
-        line 116: 0
-        line 117: 5
+        line 117: 0
+        line 118: 5
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lio/atoti/loading/kafka/impl/KafkaLoaderParams;
             0       7     1 batchSize   I
 
   public int hashCode();
     descriptor: ()I
@@ -525,24 +525,28 @@
        139: getfield      #13                 // Field topic:Ljava/lang/String;
        142: invokevirtual #44                 // Method java/lang/String.hashCode:()I
        145: iadd
        146: istore_2
        147: iload_2
        148: ireturn
       LineNumberTable:
-        line 122: 0
-        line 123: 3
-        line 124: 5
-        line 125: 31
-        line 126: 41
-        line 127: 51
-        line 128: 75
-        line 129: 99
-        line 130: 123
-        line 131: 147
+        line 123: 0
+        line 124: 3
+        line 125: 5
+        line 127: 9
+        line 128: 31
+        line 129: 41
+        line 130: 51
+        line 131: 55
+        line 132: 75
+        line 133: 79
+        line 134: 99
+        line 136: 103
+        line 137: 123
+        line 138: 147
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0     149     0  this   Lio/atoti/loading/kafka/impl/KafkaLoaderParams;
             3     146     1 prime   I
             5     144     2 result   I
       StackMapTable: number_of_entries = 10
         frame_type = 255 /* full_frame */
@@ -695,51 +699,51 @@
        211: invokevirtual #55                 // Method java/lang/String.equals:(Ljava/lang/Object;)Z
        214: ifne          219
        217: iconst_0
        218: ireturn
        219: iconst_1
        220: ireturn
       LineNumberTable:
-        line 136: 0
-        line 137: 5
-        line 139: 7
-        line 140: 11
-        line 142: 13
-        line 143: 24
-        line 145: 26
-        line 146: 31
-        line 147: 38
-        line 148: 45
-        line 150: 47
-        line 151: 63
-        line 153: 65
-        line 154: 76
-        line 156: 78
-        line 157: 89
-        line 159: 91
-        line 160: 98
-        line 161: 105
-        line 163: 107
-        line 164: 121
-        line 166: 123
-        line 167: 130
-        line 168: 137
-        line 170: 139
-        line 171: 153
-        line 173: 155
-        line 174: 162
-        line 175: 169
-        line 177: 171
-        line 178: 185
-        line 180: 187
-        line 181: 194
-        line 182: 201
-        line 184: 203
-        line 185: 217
-        line 187: 219
+        line 143: 0
+        line 144: 5
+        line 146: 7
+        line 147: 11
+        line 149: 13
+        line 150: 24
+        line 152: 26
+        line 153: 31
+        line 154: 38
+        line 155: 45
+        line 157: 47
+        line 158: 63
+        line 160: 65
+        line 161: 76
+        line 163: 78
+        line 164: 89
+        line 166: 91
+        line 167: 98
+        line 168: 105
+        line 170: 107
+        line 171: 121
+        line 173: 123
+        line 174: 130
+        line 175: 137
+        line 177: 139
+        line 178: 153
+        line 180: 155
+        line 181: 162
+        line 182: 169
+        line 184: 171
+        line 185: 185
+        line 187: 187
+        line 188: 194
+        line 189: 201
+        line 191: 203
+        line 192: 217
+        line 194: 219
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0     221     0  this   Lio/atoti/loading/kafka/impl/KafkaLoaderParams;
             0     221     1   obj   Ljava/lang/Object;
            31     190     2 other   Lio/atoti/loading/kafka/impl/KafkaLoaderParams;
       StackMapTable: number_of_entries = 15
         frame_type = 7 /* same */
```

### io/atoti/loading/kafka/impl/KafkaDataTableFactory.class

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 08f835175b8517bc9c103e53a7d488dec53b2be610b4d068c3a30d12a7c29b7a
+  SHA-256 checksum 317803c90bf5417a6bc70707e999656a68121ae0443baefba5ab5e58ff7578de
   Compiled from "KafkaDataTableFactory.java"
 public class io.atoti.loading.kafka.impl.KafkaDataTableFactory extends java.lang.Object implements io.atoti.loading.DataTableFactory<io.atoti.loading.kafka.impl.KafkaDataTable>
   minor version: 0
   major version: 55
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #7                          // io/atoti/loading/kafka/impl/KafkaDataTableFactory
   super_class: #2                         // java/lang/Object
@@ -190,22 +190,22 @@
         62: aload_0
         63: ldc           #50                 // String additionalParameters
         65: invokeinterface #28,  2           // InterfaceMethod java/util/Map.get:(Ljava/lang/Object;)Ljava/lang/Object;
         70: checkcast     #29                 // class java/util/Map
         73: invokespecial #52                 // Method io/atoti/loading/kafka/impl/KafkaLoaderParams."<init>":(Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;ILjava/util/Map;)V
         76: areturn
       LineNumberTable:
-        line 40: 0
-        line 41: 7
-        line 42: 18
-        line 43: 29
-        line 44: 40
-        line 45: 51
-        line 46: 65
-        line 40: 76
+        line 41: 0
+        line 42: 7
+        line 43: 18
+        line 44: 29
+        line 45: 40
+        line 46: 51
+        line 47: 65
+        line 41: 76
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      77     0 values   Ljava/util/Map;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      77     0 values   Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;
     Signature: #83                          // (Ljava/util/Map<Ljava/lang/String;Ljava/lang/Object;>;)Lio/atoti/loading/kafka/impl/KafkaLoaderParams;
```

### META-INF/maven/io.atoti/kafka-source/pom.xml

#### META-INF/maven/io.atoti/kafka-source/pom.xml

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <parent>
     <groupId>io.atoti</groupId>
     <artifactId>plugins</artifactId>
-    <version>6.0.11-20240105-140955</version>
+    <version>6.0.12-20240201-150858</version>
   </parent>
   <modelVersion>4.0.0</modelVersion>
   <artifactId>kafka-source</artifactId>
   <name>kafka-source</name>
   <packaging>jar</packaging>
   <dependencies>
     <dependency>
```

### META-INF/maven/io.atoti/kafka-source/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=kafka-source
 groupId=io.atoti
-version=6.0.11-20240105-140955
+version=6.0.12-20240201-150858
```

## Comparing `atoti_kafka-0.8.8.dist-info/METADATA` & `atoti_kafka-0.8.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atoti-kafka
-Version: 0.8.8
+Version: 0.8.9
 Summary: Plugin to load real time Kafka streams into Atoti tables
 Home-page: https://www.atoti.io
 License: Proprietary
 Keywords: atoti,kafka,load,table,source,realtime,stream
 Author: ActiveViam
 Author-email: dev@atoti.io
 Requires-Python: >=3.9
@@ -15,12 +15,12 @@
 Classifier: Programming Language :: Java
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Dist: atoti (==0.8.8)
+Requires-Dist: atoti (==0.8.9)
 Requires-Dist: atoti-core
 Requires-Dist: typing-extensions
 Project-URL: Bug Tracker, https://github.com/atoti/atoti/issues
-Project-URL: Documentation, https://docs.atoti.io/0.8.8/api/atoti_kafka.html
+Project-URL: Documentation, https://docs.atoti.io/0.8.9/api/atoti_kafka.html
```

