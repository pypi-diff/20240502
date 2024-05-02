# Comparing `tmp/dig_ass_text_protos-1.0.0.tar.gz` & `tmp/dig_ass_text_protos-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_text_protos-1.0.0.tar", last modified: Thu May  2 11:13:18 2024, max compression
+gzip compressed data, was "dig_ass_text_protos-1.0.1.tar", last modified: Thu May  2 14:36:39 2024, max compression
```

## Comparing `dig_ass_text_protos-1.0.0.tar` & `dig_ass_text_protos-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:18.417823 dig_ass_text_protos-1.0.0/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.0/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 11:13:18.417823 dig_ass_text_protos-1.0.0/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-1.0.0/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:18.413822 dig_ass_text_protos-1.0.0/dig_ass_text_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2764 2024-05-02 11:13:17.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2470 2024-05-02 11:13:17.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-05-02 11:13:17.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1647 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:18.417823 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 11:13:18.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-05-02 11:13:18.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 11:13:18.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 11:13:18.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-05-02 11:13:18.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.0/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 11:13:18.417823 dig_ass_text_protos-1.0.0/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.0/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 14:36:39.167640 dig_ass_text_protos-1.0.1/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.1/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 14:36:39.167640 dig_ass_text_protos-1.0.1/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-1.0.1/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 14:36:39.167640 dig_ass_text_protos-1.0.1/dig_ass_text_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2764 2024-05-02 14:36:37.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2470 2024-05-02 14:36:37.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-05-02 14:36:37.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 14:35:07.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1646 2024-05-02 14:34:57.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 14:36:39.167640 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 14:36:39.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-05-02 14:36:39.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 14:36:39.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 14:36:39.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-05-02 14:36:39.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.1/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 14:36:39.167640 dig_ass_text_protos-1.0.1/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.1/setup.py
```

### Comparing `dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2.py` & `dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2.pyi` & `dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py` & `dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.0/dig_ass_text_protos/client.py` & `dig_ass_text_protos-1.0.1/dig_ass_text_protos/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                         self.__rep_to_obj(replica)
                         for replica in inner_context['Replicas']
                     ]
                 ),
             ),
         )
         response: DigitalAssistantTextResponse = self._stub.GetTextResponse(request)
-        return response.Score
+        return response.Text
 
     def __rep_to_obj(self, replica_dict):
         return ReplicaItem(
             Body=replica_dict['Body'],
             Role=replica_dict['Role'],
             DateTime=replica_dict['DateTime'],
         )
```

### Comparing `dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/SOURCES.txt` & `dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.0/setup.py` & `dig_ass_text_protos-1.0.1/setup.py`

 * *Files identical despite different names*

