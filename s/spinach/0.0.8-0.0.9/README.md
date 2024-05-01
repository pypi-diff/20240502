# Comparing `tmp/spinach-0.0.8.tar.gz` & `tmp/spinach-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spinach-0.0.8.tar", last modified: Thu Oct 11 20:39:12 2018, max compression
+gzip compressed data, was "dist/spinach-0.0.9.tar", last modified: Tue Dec  4 10:01:28 2018, max compression
```

## Comparing `spinach-0.0.8.tar` & `spinach-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-10-11 20:39:12.000000 spinach-0.0.8/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       38 2018-10-11 20:39:12.000000 spinach-0.0.8/setup.cfg
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1636 2018-10-11 20:16:00.000000 spinach-0.0.8/README.rst
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     9862 2018-10-11 11:09:01.000000 spinach-0.0.8/spinach/task.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     9145 2018-10-11 11:11:28.000000 spinach-0.0.8/spinach/engine.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     6988 2018-10-10 20:30:13.000000 spinach-0.0.8/spinach/job.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      377 2018-10-11 20:37:18.000000 spinach-0.0.8/spinach/const.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     2828 2018-02-22 19:59:25.000000 spinach-0.0.8/spinach/signals.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach/contrib/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3058 2018-10-10 09:48:00.000000 spinach-0.0.8/spinach/contrib/flask_spinach.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach/contrib/spinachd/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1229 2018-10-11 12:26:56.000000 spinach-0.0.8/spinach/contrib/spinachd/mail.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach/contrib/spinachd/management/
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach/contrib/spinachd/management/commands/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1334 2018-10-10 11:17:15.000000 spinach-0.0.8/spinach/contrib/spinachd/management/commands/spinach.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2018-10-09 09:16:32.000000 spinach-0.0.8/spinach/contrib/spinachd/management/commands/__init__.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2018-10-09 09:16:32.000000 spinach-0.0.8/spinach/contrib/spinachd/management/__init__.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      380 2018-10-09 09:43:17.000000 spinach-0.0.8/spinach/contrib/spinachd/signals.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      513 2018-10-10 09:59:22.000000 spinach-0.0.8/spinach/contrib/spinachd/settings.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1342 2018-10-09 09:43:17.000000 spinach-0.0.8/spinach/contrib/spinachd/tasks.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1519 2018-10-09 21:43:35.000000 spinach-0.0.8/spinach/contrib/spinachd/apps.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       92 2018-10-09 10:59:35.000000 spinach-0.0.8/spinach/contrib/spinachd/__init__.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1446 2018-02-24 15:12:49.000000 spinach-0.0.8/spinach/contrib/sentry.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2018-02-19 20:57:40.000000 spinach-0.0.8/spinach/contrib/__init__.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     2691 2018-10-10 09:25:26.000000 spinach-0.0.8/spinach/utils.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3949 2018-10-10 20:30:13.000000 spinach-0.0.8/spinach/worker.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      172 2018-02-24 21:27:23.000000 spinach-0.0.8/spinach/exc.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach/brokers/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3502 2018-03-06 19:44:42.000000 spinach-0.0.8/spinach/brokers/base.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     8202 2018-10-07 13:51:49.000000 spinach-0.0.8/spinach/brokers/redis.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4513 2018-03-06 19:44:42.000000 spinach-0.0.8/spinach/brokers/memory.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach/brokers/redis_scripts/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      656 2018-02-25 15:29:58.000000 spinach-0.0.8/spinach/brokers/redis_scripts/get_jobs_from_queue.lua
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      435 2018-02-25 10:49:11.000000 spinach-0.0.8/spinach/brokers/redis_scripts/enqueue_job.lua
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     2309 2018-10-07 14:01:25.000000 spinach-0.0.8/spinach/brokers/redis_scripts/move_future_jobs.lua
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      498 2018-02-25 10:53:41.000000 spinach-0.0.8/spinach/brokers/redis_scripts/enqueue_future_job.lua
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      186 2018-02-10 13:09:44.000000 spinach-0.0.8/spinach/brokers/redis_scripts/flush.lua
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1536 2018-08-30 12:50:31.000000 spinach-0.0.8/spinach/brokers/redis_scripts/register_periodic_tasks.lua
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2017-09-04 20:02:05.000000 spinach-0.0.8/spinach/brokers/redis_scripts/__init__.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2017-08-18 19:59:16.000000 spinach-0.0.8/spinach/brokers/__init__.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      204 2018-02-25 11:39:26.000000 spinach-0.0.8/spinach/__init__.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4490 2018-10-11 20:39:12.000000 spinach-0.0.8/PKG-INFO
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach.egg-info/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        8 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach.egg-info/top_level.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4490 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach.egg-info/PKG-INFO
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1233 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       84 2018-10-11 20:39:12.000000 spinach-0.0.8/spinach.egg-info/requires.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     2069 2018-10-09 12:10:59.000000 spinach-0.0.8/setup.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-12-04 10:01:28.000000 spinach-0.0.9/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       38 2018-12-04 10:01:28.000000 spinach-0.0.9/setup.cfg
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1645 2018-12-04 09:19:44.000000 spinach-0.0.9/README.rst
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     9862 2018-10-11 11:09:01.000000 spinach-0.0.9/spinach/task.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     9145 2018-10-11 11:11:28.000000 spinach-0.0.9/spinach/engine.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     6988 2018-10-10 20:30:13.000000 spinach-0.0.9/spinach/job.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      409 2018-12-04 09:59:02.000000 spinach-0.0.9/spinach/const.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     2828 2018-02-22 19:59:25.000000 spinach-0.0.9/spinach/signals.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach/contrib/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3058 2018-10-10 09:48:00.000000 spinach-0.0.9/spinach/contrib/flask_spinach.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach/contrib/spinachd/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1229 2018-10-11 12:26:56.000000 spinach-0.0.9/spinach/contrib/spinachd/mail.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach/contrib/spinachd/management/
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach/contrib/spinachd/management/commands/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1540 2018-12-03 10:40:32.000000 spinach-0.0.9/spinach/contrib/spinachd/management/commands/spinach.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2018-10-09 09:16:32.000000 spinach-0.0.9/spinach/contrib/spinachd/management/commands/__init__.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2018-10-09 09:16:32.000000 spinach-0.0.9/spinach/contrib/spinachd/management/__init__.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      380 2018-10-09 09:43:17.000000 spinach-0.0.9/spinach/contrib/spinachd/signals.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      513 2018-10-10 09:59:22.000000 spinach-0.0.9/spinach/contrib/spinachd/settings.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1342 2018-10-09 09:43:17.000000 spinach-0.0.9/spinach/contrib/spinachd/tasks.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1519 2018-10-09 21:43:35.000000 spinach-0.0.9/spinach/contrib/spinachd/apps.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       92 2018-10-09 10:59:35.000000 spinach-0.0.9/spinach/contrib/spinachd/__init__.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1503 2018-12-03 12:58:43.000000 spinach-0.0.9/spinach/contrib/datadog.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1446 2018-02-24 15:12:49.000000 spinach-0.0.9/spinach/contrib/sentry.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2018-02-19 20:57:40.000000 spinach-0.0.9/spinach/contrib/__init__.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3230 2018-11-08 20:35:36.000000 spinach-0.0.9/spinach/utils.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3949 2018-10-10 20:30:13.000000 spinach-0.0.9/spinach/worker.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      172 2018-02-24 21:27:23.000000 spinach-0.0.9/spinach/exc.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach/brokers/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3502 2018-03-06 19:44:42.000000 spinach-0.0.9/spinach/brokers/base.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     9144 2018-11-09 09:13:48.000000 spinach-0.0.9/spinach/brokers/redis.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4513 2018-03-06 19:44:42.000000 spinach-0.0.9/spinach/brokers/memory.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach/brokers/redis_scripts/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      656 2018-02-25 15:29:58.000000 spinach-0.0.9/spinach/brokers/redis_scripts/get_jobs_from_queue.lua
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1002 2018-11-09 09:13:48.000000 spinach-0.0.9/spinach/brokers/redis_scripts/enqueue_job.lua
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     2309 2018-11-05 20:19:22.000000 spinach-0.0.9/spinach/brokers/redis_scripts/move_future_jobs.lua
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      186 2018-02-10 13:09:44.000000 spinach-0.0.9/spinach/brokers/redis_scripts/flush.lua
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1536 2018-08-30 12:50:31.000000 spinach-0.0.9/spinach/brokers/redis_scripts/register_periodic_tasks.lua
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2017-09-04 20:02:05.000000 spinach-0.0.9/spinach/brokers/redis_scripts/__init__.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        0 2017-08-18 19:59:16.000000 spinach-0.0.9/spinach/brokers/__init__.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      204 2018-02-25 11:39:26.000000 spinach-0.0.9/spinach/__init__.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4499 2018-12-04 10:01:28.000000 spinach-0.0.9/PKG-INFO
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach.egg-info/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        8 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach.egg-info/top_level.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4499 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1207 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       84 2018-12-04 10:01:28.000000 spinach-0.0.9/spinach.egg-info/requires.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     2031 2018-11-09 09:13:47.000000 spinach-0.0.9/setup.py
```

### Comparing `spinach-0.0.8/README.rst` & `spinach-0.0.9/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Redis task queue for Python 3 heavily inspired by Celery and RQ.
 
 Distinctive features:
 
 - At-least-once or at-most-once delivery per task
 - Periodic tasks without an additional process
 - Scheduling of tasks in batch
-- Integrations with `Flask, Django, Logging and Sentry
+- Integrations with `Flask, Django, Logging, Sentry and Datadog
   <https://spinach.readthedocs.io/en/stable/user/integrations.html>`_
 - Embeddable workers for easier testing
 - Python 3, threaded, explicit... see `design choices
   <https://spinach.readthedocs.io/en/latest/user/design.html>`_ for more
   details
 
 Quickstart
```

### Comparing `spinach-0.0.8/spinach/task.py` & `spinach-0.0.9/spinach/task.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/engine.py` & `spinach-0.0.9/spinach/engine.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/job.py` & `spinach-0.0.9/spinach/job.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/signals.py` & `spinach-0.0.9/spinach/signals.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/contrib/flask_spinach.py` & `spinach-0.0.9/spinach/contrib/flask_spinach.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/contrib/spinachd/mail.py` & `spinach-0.0.9/spinach/contrib/spinachd/mail.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/contrib/spinachd/management/commands/spinach.py` & `spinach-0.0.9/spinach/contrib/spinachd/management/commands/spinach.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.apps import apps
 from django.core.management.base import BaseCommand
 try:
     from raven.contrib.django.models import client as raven_client
 except ImportError:
     raven_client = None
 
 from spinach.const import DEFAULT_QUEUE, DEFAULT_WORKER_NUMBER
@@ -36,12 +37,16 @@
         )
 
     def handle(self, *args, **options):
 
         if raven_client is not None:
             register_sentry(raven_client, spin.namespace)
 
+        if apps.is_installed('ddtrace.contrib.django'):
+            from spinach.contrib.datadog import register_datadog
+            register_datadog(namespace=spin.namespace)
+
         spin.start_workers(
             number=options['threads'],
             queue=options['queue'],
             stop_when_queue_empty=options['stop_when_queue_empty']
         )
```

### Comparing `spinach-0.0.8/spinach/contrib/spinachd/settings.py` & `spinach-0.0.9/spinach/contrib/spinachd/settings.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/contrib/spinachd/tasks.py` & `spinach-0.0.9/spinach/contrib/spinachd/tasks.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/contrib/spinachd/apps.py` & `spinach-0.0.9/spinach/contrib/spinachd/apps.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/contrib/sentry.py` & `spinach-0.0.9/spinach/contrib/sentry.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/utils.py` & `spinach-0.0.9/spinach/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,26 +42,42 @@
                                delay)
             else:
                 logger.exception('Unexpected error. Retrying in %s', delay)
 
             must_stop.wait(delay.total_seconds())
 
 
+def call_with_retry(func: Callable, exceptions, max_retries: int,
+                    logger: Logger, *args, **kwargs):
+    """Call a function and retry it on failure."""
+    attempt = 0
+    while True:
+        try:
+            return func(*args, **kwargs)
+        except exceptions as e:
+            attempt += 1
+            if attempt >= max_retries:
+                raise
+
+            delay = exponential_backoff(attempt, cap=60)
+            logger.warning('%s: retrying in %s', e, delay)
+            time.sleep(delay.total_seconds())
+
+
 def exponential_backoff(attempt: int, cap: int=1200) -> timedelta:
     """Calculate a delay to retry using an exponential backoff algorithm.
 
     It is an exponential backoff with random jitter to prevent failures
     from being retried at the same time. It is a good fit for most
     applications.
 
     :arg attempt: the number of attempts made
     :arg cap: maximum delay, defaults to 20 minutes
     """
     base = 3
-
     temp = min(base * 2 ** attempt, cap)
     return timedelta(seconds=temp / 2 + random.randint(0, temp / 2))
 
 
 @contextlib.contextmanager
 def handle_sigterm():
     """Handle SIGTERM like a normal SIGINT (KeyboardInterrupt).
```

### Comparing `spinach-0.0.8/spinach/worker.py` & `spinach-0.0.9/spinach/worker.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/brokers/base.py` & `spinach-0.0.9/spinach/brokers/base.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/brokers/redis.py` & `spinach-0.0.9/spinach/brokers/redis.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,47 +4,50 @@
 import math
 from os import path
 import socket
 import threading
 from typing import Optional, Iterable, List, Tuple
 import uuid
 
-from redis import StrictRedis
+from redis import StrictRedis, ConnectionError, TimeoutError
 from redis.client import Script
 
 from ..brokers.base import Broker
 from ..job import Job, JobStatus
 from ..task import Task
 from ..const import (
     FUTURE_JOBS_KEY, NOTIFICATIONS_KEY, RUNNING_JOBS_KEY,
-    PERIODIC_TASKS_HASH_KEY, PERIODIC_TASKS_QUEUE_KEY
+    PERIODIC_TASKS_HASH_KEY, PERIODIC_TASKS_QUEUE_KEY,
+    DEFAULT_ENQUEUE_JOB_RETRIES
 )
-from ..utils import run_forever
+from ..utils import run_forever, call_with_retry
 
 
 logger = getLogger('spinach.broker')
 here = path.abspath(path.dirname(__file__))
 
 
 # Todo: make move_future_jobs into a more generic task not always executed at
 # arbiter loop (like once per minute) that:
 # - moves future jobs
 # - registers the broker
 # - moves running jobs from stale brokers
 
 class RedisBroker(Broker):
 
-    def __init__(self, redis: Optional[StrictRedis]=None):
+    def __init__(self, redis: Optional[StrictRedis]=None,
+                 enqueue_job_max_retries: int=DEFAULT_ENQUEUE_JOB_RETRIES):
         super().__init__()
         self._r = redis if redis else StrictRedis(**recommended_socket_opts)
+        self.enqueue_job_max_retries = enqueue_job_max_retries
 
         # Register the lua scripts
+        self._idempotency_protected_scripts = list()
         self._move_future_jobs = self._load_script('move_future_jobs.lua')
         self._enqueue_job = self._load_script('enqueue_job.lua')
-        self._enqueue_future_job = self._load_script('enqueue_future_job.lua')
         self._flush = self._load_script('flush.lua')
         self._get_jobs_from_queue = self._load_script(
             'get_jobs_from_queue.lua'
         )
         self._register_periodic_tasks = self._load_script(
             'register_periodic_tasks.lua'
         )
@@ -53,50 +56,69 @@
     def _reset(self):
         """Initialization that must happen before the broker is (re)started."""
         self._subscriber_thread = None
         self._must_stop = threading.Event()
         self._number_periodic_tasks = 0
 
     def _load_script(self, filename: str) -> Script:
+        """Load a Lua script.
+
+        Read the Lua script file to generate its Script object. If the script
+        starts with a magic string, add it to the list of scripts requiring an
+        idempotency token to execute.
+        """
         with open(path.join(here, 'redis_scripts', filename), mode='rb') as f:
             script_data = f.read()
-        return self._r.register_script(script_data)
+        rv = self._r.register_script(script_data)
+        if script_data.startswith(b'-- idempotency protected script'):
+            self._idempotency_protected_scripts.append(rv)
+        return rv
 
     def _run_script(self, script: Script, *args):
         args = [str(self._id)] + list(args)
-        return script(args=args)
+
+        if script not in self._idempotency_protected_scripts:
+            return script(args=args)
+
+        # Script is protected by idempotency token, can be retried safely
+        idempotency_token = generate_idempotency_token()
+        args.insert(
+            0, self._to_namespaced('idempotency_{}'.format(idempotency_token))
+        )
+        rv = call_with_retry(
+            script,
+            (ConnectionError, TimeoutError),
+            self.enqueue_job_max_retries,
+            logger,
+            args=args
+        )
+        if rv == -1:
+            logger.info('Script not reprocessed because it was '
+                        'already processed once')
+
+        return rv
 
     def enqueue_jobs(self, jobs: Iterable[Job]):
         """Enqueue a batch of jobs."""
         jobs_to_queue = list()
-        future_jobs = list()
         for job in jobs:
             if job.should_start:
                 job.status = JobStatus.QUEUED
-                jobs_to_queue.append(job.serialize())
             else:
                 job.status = JobStatus.WAITING
-                future_jobs.append(job.serialize())
+            jobs_to_queue.append(job.serialize())
 
         if jobs_to_queue:
             self._run_script(
                 self._enqueue_job,
                 self._to_namespaced(NOTIFICATIONS_KEY),
                 self._to_namespaced(RUNNING_JOBS_KEY.format(self._id)),
                 self.namespace,
-                *jobs_to_queue
-            )
-
-        if future_jobs:
-            self._run_script(
-                self._enqueue_future_job,
-                self._to_namespaced(NOTIFICATIONS_KEY),
-                self._to_namespaced(RUNNING_JOBS_KEY.format(self._id)),
                 self._to_namespaced(FUTURE_JOBS_KEY),
-                *future_jobs
+                *jobs_to_queue
             )
 
     def move_future_jobs(self) -> int:
         num_jobs_moved = self._run_script(
             self._move_future_jobs,
             self.namespace,
             self._to_namespaced(FUTURE_JOBS_KEY),
@@ -216,14 +238,18 @@
         next_event_time = rv[0][1]
         if next_event_time < now:
             return 0
 
         return next_event_time - now
 
 
+def generate_idempotency_token():
+    return str(uuid.uuid4())
+
+
 recommended_socket_opts = {
     'socket_timeout': 60,
     'socket_connect_timeout': 15
 }
 try:
     # These are the values used by Redis itself by default
     recommended_socket_opts['socket_keepalive_options'] = {
```

### Comparing `spinach-0.0.8/spinach/brokers/memory.py` & `spinach-0.0.9/spinach/brokers/memory.py`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/brokers/redis_scripts/get_jobs_from_queue.lua` & `spinach-0.0.9/spinach/brokers/redis_scripts/get_jobs_from_queue.lua`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/brokers/redis_scripts/move_future_jobs.lua` & `spinach-0.0.9/spinach/brokers/redis_scripts/move_future_jobs.lua`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/spinach/brokers/redis_scripts/register_periodic_tasks.lua` & `spinach-0.0.9/spinach/brokers/redis_scripts/register_periodic_tasks.lua`

 * *Files identical despite different names*

### Comparing `spinach-0.0.8/PKG-INFO` & `spinach-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinach
-Version: 0.0.8
+Version: 0.0.9
 Summary: Modern Redis task queue for Python 3
 Home-page: https://github.com/NicolasLM/spinach
 Author: Nicolas Le Manchet
 Author-email: nicolas@lemanchet.fr
 License: BSD 2-clause
 Description: Spinach
         =======
@@ -19,15 +19,15 @@
         Redis task queue for Python 3 heavily inspired by Celery and RQ.
         
         Distinctive features:
         
         - At-least-once or at-most-once delivery per task
         - Periodic tasks without an additional process
         - Scheduling of tasks in batch
-        - Integrations with `Flask, Django, Logging and Sentry
+        - Integrations with `Flask, Django, Logging, Sentry and Datadog
           <https://spinach.readthedocs.io/en/stable/user/integrations.html>`_
         - Embeddable workers for easier testing
         - Python 3, threaded, explicit... see `design choices
           <https://spinach.readthedocs.io/en/latest/user/design.html>`_ for more
           details
         
         Quickstart
```

### Comparing `spinach-0.0.8/spinach.egg-info/PKG-INFO` & `spinach-0.0.9/spinach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinach
-Version: 0.0.8
+Version: 0.0.9
 Summary: Modern Redis task queue for Python 3
 Home-page: https://github.com/NicolasLM/spinach
 Author: Nicolas Le Manchet
 Author-email: nicolas@lemanchet.fr
 License: BSD 2-clause
 Description: Spinach
         =======
@@ -19,15 +19,15 @@
         Redis task queue for Python 3 heavily inspired by Celery and RQ.
         
         Distinctive features:
         
         - At-least-once or at-most-once delivery per task
         - Periodic tasks without an additional process
         - Scheduling of tasks in batch
-        - Integrations with `Flask, Django, Logging and Sentry
+        - Integrations with `Flask, Django, Logging, Sentry and Datadog
           <https://spinach.readthedocs.io/en/stable/user/integrations.html>`_
         - Embeddable workers for easier testing
         - Python 3, threaded, explicit... see `design choices
           <https://spinach.readthedocs.io/en/latest/user/design.html>`_ for more
           details
         
         Quickstart
```

### Comparing `spinach-0.0.8/spinach.egg-info/SOURCES.txt` & `spinach-0.0.9/spinach.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 spinach.egg-info/requires.txt
 spinach.egg-info/top_level.txt
 spinach/brokers/__init__.py
 spinach/brokers/base.py
 spinach/brokers/memory.py
 spinach/brokers/redis.py
 spinach/brokers/redis_scripts/__init__.py
-spinach/brokers/redis_scripts/enqueue_future_job.lua
 spinach/brokers/redis_scripts/enqueue_job.lua
 spinach/brokers/redis_scripts/flush.lua
 spinach/brokers/redis_scripts/get_jobs_from_queue.lua
 spinach/brokers/redis_scripts/move_future_jobs.lua
 spinach/brokers/redis_scripts/register_periodic_tasks.lua
 spinach/contrib/__init__.py
+spinach/contrib/datadog.py
 spinach/contrib/flask_spinach.py
 spinach/contrib/sentry.py
 spinach/contrib/spinachd/__init__.py
 spinach/contrib/spinachd/apps.py
 spinach/contrib/spinachd/mail.py
 spinach/contrib/spinachd/settings.py
 spinach/contrib/spinachd/signals.py
```

### Comparing `spinach-0.0.8/setup.py` & `spinach-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,13 @@
         ],
     },
 
     package_data={
         'spinach.brokers.redis_scripts': [
             'move_future_jobs.lua',
             'enqueue_job.lua',
-            'enqueue_future_job.lua',
             'flush.lua',
             'get_jobs_from_queue.lua',
             'register_periodic_tasks.lua'
         ],
     },
 )
```

