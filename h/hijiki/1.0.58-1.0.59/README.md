# Comparing `tmp/hijiki-1.0.58.tar.gz` & `tmp/hijiki-1.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hijiki-1.0.58.tar", last modified: Mon Apr  8 20:47:56 2024, max compression
+gzip compressed data, was "hijiki-1.0.59.tar", last modified: Thu May  2 20:03:02 2024, max compression
```

## Comparing `hijiki-1.0.58.tar` & `hijiki-1.0.59.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.566949 hijiki-1.0.58/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 20:46:29.000000 hijiki-1.0.58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-08 20:47:56.566949 hijiki-1.0.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-08 20:46:29.000000 hijiki-1.0.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.562950 hijiki-1.0.58/hijiki/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.562950 hijiki-1.0.58/hijiki/broker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/broker/broker_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/broker/hijiki_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/broker/hijiki_rabbit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.562950 hijiki-1.0.58/hijiki/decorator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/decorator/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/hijiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.562950 hijiki-1.0.58/hijiki/publisher/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/publisher/Publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:46:29.000000 hijiki-1.0.58/hijiki/publisher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.566949 hijiki-1.0.58/hijiki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-08 20:47:56.000000 hijiki-1.0.58/hijiki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 20:47:56.000000 hijiki-1.0.58/hijiki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:47:56.000000 hijiki-1.0.58/hijiki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 20:47:56.000000 hijiki-1.0.58/hijiki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 20:47:56.000000 hijiki-1.0.58/hijiki.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:47:56.566949 hijiki-1.0.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-08 20:47:00.000000 hijiki-1.0.58/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:56.562950 hijiki-1.0.58/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-08 20:46:29.000000 hijiki-1.0.58/tests/test_broker_data_server_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-08 20:46:29.000000 hijiki-1.0.58/tests/test_broker_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-08 20:46:29.000000 hijiki-1.0.58/tests/test_publisher_consumer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.988008 hijiki-1.0.59/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 20:01:32.000000 hijiki-1.0.59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-02 20:03:02.988008 hijiki-1.0.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-02 20:01:32.000000 hijiki-1.0.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.984008 hijiki-1.0.59/hijiki/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.984008 hijiki-1.0.59/hijiki/broker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/broker/broker_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/broker/hijiki_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/broker/hijiki_rabbit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.984008 hijiki-1.0.59/hijiki/decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/decorator/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/hijiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.984008 hijiki-1.0.59/hijiki/publisher/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/publisher/Publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/publisher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.988008 hijiki-1.0.59/hijiki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-02 20:03:02.000000 hijiki-1.0.59/hijiki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-02 20:03:02.000000 hijiki-1.0.59/hijiki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:03:02.000000 hijiki-1.0.59/hijiki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 20:03:02.000000 hijiki-1.0.59/hijiki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 20:03:02.000000 hijiki-1.0.59/hijiki.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:03:02.988008 hijiki-1.0.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-02 20:02:06.000000 hijiki-1.0.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.988008 hijiki-1.0.59/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-02 20:01:32.000000 hijiki-1.0.59/tests/test_broker_data_server_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-02 20:01:32.000000 hijiki-1.0.59/tests/test_broker_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-02 20:01:32.000000 hijiki-1.0.59/tests/test_publisher_consumer_test.py
```

### Comparing `hijiki-1.0.58/LICENSE` & `hijiki-1.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.58/PKG-INFO` & `hijiki-1.0.59/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: hijiki
-Version: 1.0.58
-Summary: Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
-Author: Leandro Vilson Battisti
-Keywords: Celery,Kombu,RabbitMQ,decorator
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: celery==5.3.4
-Requires-Dist: urllib3<2.0
-
 # Hijiki
 Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
 
 ## Configurations
 Hijiki uses environment variables to configure connection with BROKER. 
 
 ### COMMON
@@ -46,15 +35,15 @@
 If server is not present, even BROKER_CLUSTER_SERVER, the connection url will be a default, and to others configs will be changed for "teste".
 
 ## How to use
 ### Publisher
 The example demonstrate how to publish a simple message to topic "teste1_event" with a json message:
 
 ```python
-pub = Publisher("localhost", "rabbitmq", "rabbitmq", 5672)
+pub = Publisher("localhost", "rabbitmq", "rabbitmq", 5672, heartbeat=30)
 pub.publish_message('teste1_event', '{"value": "Esta é a mensagem"}')
 ```
 
 ### Consumer
 Consumer uses a configuration to define QUEUES and Exchanges and the consumer is a decorator for the queue.
 
 ```python
@@ -62,14 +51,15 @@
 
 qs = [HijikiQueueExchange('teste1', 'teste1_event'), HijikiQueueExchange('teste2', 'teste2_event')]
 gr = HijikiRabbit().with_queues_exchange(qs) \
     .with_username("rabbitmq") \
     .with_password("rabbitmq") \
     .with_host("localhost") \
     .with_port(5672) \
+    .with_heartbeat_interval(30)\
     .build()
 
 class MyConsumer():
     @gr.task(queue_name='teste1')
     def my_consumer(data):
         print(f"consumer 1 executed with data : {data}")
```

### Comparing `hijiki-1.0.58/README.md` & `hijiki-1.0.59/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: hijiki
+Version: 1.0.59
+Summary: Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
+Author: Leandro Vilson Battisti
+Keywords: Celery,Kombu,RabbitMQ,decorator
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: celery==5.3.4
+Requires-Dist: urllib3<2.0
+
 # Hijiki
 Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
 
 ## Configurations
 Hijiki uses environment variables to configure connection with BROKER. 
 
 ### COMMON
@@ -35,15 +46,15 @@
 If server is not present, even BROKER_CLUSTER_SERVER, the connection url will be a default, and to others configs will be changed for "teste".
 
 ## How to use
 ### Publisher
 The example demonstrate how to publish a simple message to topic "teste1_event" with a json message:
 
 ```python
-pub = Publisher("localhost", "rabbitmq", "rabbitmq", 5672)
+pub = Publisher("localhost", "rabbitmq", "rabbitmq", 5672, heartbeat=30)
 pub.publish_message('teste1_event', '{"value": "Esta é a mensagem"}')
 ```
 
 ### Consumer
 Consumer uses a configuration to define QUEUES and Exchanges and the consumer is a decorator for the queue.
 
 ```python
@@ -51,14 +62,15 @@
 
 qs = [HijikiQueueExchange('teste1', 'teste1_event'), HijikiQueueExchange('teste2', 'teste2_event')]
 gr = HijikiRabbit().with_queues_exchange(qs) \
     .with_username("rabbitmq") \
     .with_password("rabbitmq") \
     .with_host("localhost") \
     .with_port(5672) \
+    .with_heartbeat_interval(30)\
     .build()
 
 class MyConsumer():
     @gr.task(queue_name='teste1')
     def my_consumer(data):
         print(f"consumer 1 executed with data : {data}")
```

### Comparing `hijiki-1.0.58/hijiki/broker/broker_data.py` & `hijiki-1.0.59/hijiki/broker/broker_data.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.58/hijiki/broker/hijiki_broker.py` & `hijiki-1.0.59/hijiki/broker/hijiki_broker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import time
 from celery import Celery
+from typing import Optional
 
 from hijiki.broker.broker_data import get_broker_url, init_os_environ
 
 
 class HijikiBroker:
     celery_broker = None
 
-    def __init__(self, app_name, host, username, password, port, cluster_hosts):
+    def __init__(self, app_name, host, username, password, port, cluster_hosts, heartbeat: Optional[float] = 60):
         init_os_environ(host, username, password, port, cluster_hosts)
-        self.celery_broker = Celery(app_name, broker=get_broker_url(), set_as_current=True)
+        self.celery_broker = Celery(app_name, broker=get_broker_url(), set_as_current=True, heartbeat=heartbeat)
 
     def get_celery_broker(self):
         return self.celery_broker
 
     def ping(self):
         try:
             success_ping = False
```

### Comparing `hijiki-1.0.58/hijiki/broker/hijiki_rabbit.py` & `hijiki-1.0.59/hijiki/broker/hijiki_rabbit.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         self.host = None
         self.cluster_hosts = None
         self.password = None
         self.username = None
         self.queue_exchanges = None
         self.worker = None
         self.port = None
+        self.heartbeat_interval = None
 
     def terminate(self):
         self.worker.should_stop = True
 
     def with_queues_exchange(self, queue_exchanges: List[HijikiQueueExchange]):
         self.queue_exchanges = queue_exchanges
         return self
@@ -56,17 +57,21 @@
     def with_port(self, port: str):
         self.port = port
         return self
 
     def ping(self):
         return self.broker.ping()
 
+    def with_heartbeat_interval(self, heartbeat_interval: int):
+        self.heartbeat_interval = heartbeat_interval
+        return self
+
     def build(self):
         self.broker = HijikiBroker('worker', self.host, self.username, self.password, self.port, self.cluster_hosts)
-        self.connection = self.broker.get_celery_broker().broker_connection()
+        self.connection = self.broker.get_celery_broker().broker_connection(heartbeat=self.heartbeat_interval)
         self.init_queues()
         return self
 
     def init_queues(self, ):
         for q in self.queue_exchanges:
             name = q.name
             if name not in self.queues:
```

### Comparing `hijiki-1.0.58/hijiki/decorator/worker.py` & `hijiki-1.0.59/hijiki/decorator/worker.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.58/hijiki/publisher/Publisher.py` & `hijiki-1.0.59/hijiki/publisher/Publisher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from typing import Optional
+
 from kombu import producers, Exchange
 
 from hijiki.broker.hijiki_broker import HijikiBroker
 
 
 class Publisher():
 
-    def __init__(self, host, username, password, port, cluster_hosts: str = None):
-        self.client = HijikiBroker('client', host, username, password, port, cluster_hosts)
+    def __init__(self, host, username, password, port, cluster_hosts: str = None, heartbeat: Optional[float] = 60):
+        self.client = HijikiBroker('client', host, username, password, port, cluster_hosts, heartbeat=heartbeat)
 
     def publish_message(self, event_name: str, data: str):
         payload = {"value": data}
         connection = self.client.get_celery_broker().broker_connection()
         with producers[connection].acquire(block=True) as producer:
             task_exchange = Exchange(event_name, type='topic')
             producer.publish(payload,  exchange=task_exchange, declare=[task_exchange], routing_key='x')
```

### Comparing `hijiki-1.0.58/hijiki.egg-info/PKG-INFO` & `hijiki-1.0.59/hijiki.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hijiki
-Version: 1.0.58
+Version: 1.0.59
 Summary: Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
 Author: Leandro Vilson Battisti
 Keywords: Celery,Kombu,RabbitMQ,decorator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: celery==5.3.4
 Requires-Dist: urllib3<2.0
@@ -46,15 +46,15 @@
 If server is not present, even BROKER_CLUSTER_SERVER, the connection url will be a default, and to others configs will be changed for "teste".
 
 ## How to use
 ### Publisher
 The example demonstrate how to publish a simple message to topic "teste1_event" with a json message:
 
 ```python
-pub = Publisher("localhost", "rabbitmq", "rabbitmq", 5672)
+pub = Publisher("localhost", "rabbitmq", "rabbitmq", 5672, heartbeat=30)
 pub.publish_message('teste1_event', '{"value": "Esta é a mensagem"}')
 ```
 
 ### Consumer
 Consumer uses a configuration to define QUEUES and Exchanges and the consumer is a decorator for the queue.
 
 ```python
@@ -62,14 +62,15 @@
 
 qs = [HijikiQueueExchange('teste1', 'teste1_event'), HijikiQueueExchange('teste2', 'teste2_event')]
 gr = HijikiRabbit().with_queues_exchange(qs) \
     .with_username("rabbitmq") \
     .with_password("rabbitmq") \
     .with_host("localhost") \
     .with_port(5672) \
+    .with_heartbeat_interval(30)\
     .build()
 
 class MyConsumer():
     @gr.task(queue_name='teste1')
     def my_consumer(data):
         print(f"consumer 1 executed with data : {data}")
```

### Comparing `hijiki-1.0.58/hijiki.egg-info/SOURCES.txt` & `hijiki-1.0.59/hijiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.58/tests/test_broker_data_server_exists.py` & `hijiki-1.0.59/tests/test_broker_data_server_exists.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.58/tests/test_broker_ping.py` & `hijiki-1.0.59/tests/test_broker_ping.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.58/tests/test_publisher_consumer_test.py` & `hijiki-1.0.59/tests/test_publisher_consumer_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class TestPublisherConsumer(unittest.TestCase):
     runner = None
 
     def setUp(self):
         self.runner = Runner()
         self.runner.run()
-        self.pub = Publisher("localhost", "user", "pwd", 5672)
+        self.pub = Publisher("localhost", "user", "pwd", 5672, heartbeat=30)
         self.NUMBER_OF_QUEUED_MESSAGES = 2
 
     def tearDown(self):
         self.runner.stop()
 
     def test_publish_a_message(self):
         self.runner.clear_results()
@@ -45,15 +45,15 @@
             self.pub.publish_message(
                 'erro_event',
                 f'{{"value": "This is message number {number} that will be sent to dlq"}}'
             )
 
         time.sleep(SECS_TO_AWAIT_BROKER)
         self.assertEqual(self.NUMBER_OF_QUEUED_MESSAGES, len(self.runner.get_results_dlq()))
-    
+
     def test_consume_a_message_without_consumer_dlq(self):
         self.runner.clear_results()
         time.sleep(SECS_TO_AWAIT_BROKER)
         for number in range(self.NUMBER_OF_QUEUED_MESSAGES):
             self.pub.publish_message(
                 'without_dlq',
                 '{"value": "This is the message that will fall into a dlq queue, which has no consumer"}'
```

