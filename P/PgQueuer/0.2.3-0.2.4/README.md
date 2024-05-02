# Comparing `tmp/pgqueuer-0.2.3.tar.gz` & `tmp/pgqueuer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.2.3.tar", last modified: Tue Apr 30 21:07:23 2024, max compression
+gzip compressed data, was "pgqueuer-0.2.4.tar", last modified: Thu May  2 17:21:17 2024, max compression
```

## Comparing `pgqueuer-0.2.3.tar` & `pgqueuer-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.492325 pgqueuer-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.492325 pgqueuer-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.492325 pgqueuer-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 21:07:23.000000 pgqueuer-0.2.3/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/test/test_tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:07:23.496325 pgqueuer-0.2.3/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-30 21:07:12.000000 pgqueuer-0.2.3/tools/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:17.832759 pgqueuer-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:17.828760 pgqueuer-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:17.828760 pgqueuer-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-02 17:21:17.832759 pgqueuer-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:21:17.832759 pgqueuer-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:17.828760 pgqueuer-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:17.832759 pgqueuer-0.2.4/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:17.832759 pgqueuer-0.2.4/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-02 17:21:17.000000 pgqueuer-0.2.4/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-02 17:21:17.000000 pgqueuer-0.2.4/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:21:17.000000 pgqueuer-0.2.4/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 17:21:17.000000 pgqueuer-0.2.4/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 17:21:17.000000 pgqueuer-0.2.4/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 17:21:17.000000 pgqueuer-0.2.4/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:17.832759 pgqueuer-0.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:17.832759 pgqueuer-0.2.4/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:21:17.832759 pgqueuer-0.2.4/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-02 17:21:03.000000 pgqueuer-0.2.4/tools/benchmark.py
```

### Comparing `pgqueuer-0.2.3/.github/workflows/ci.yml` & `pgqueuer-0.2.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/.github/workflows/linting.yml` & `pgqueuer-0.2.4/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/.github/workflows/release.yml` & `pgqueuer-0.2.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/.gitignore` & `pgqueuer-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/LICENSE` & `pgqueuer-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/PKG-INFO` & `pgqueuer-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.2.3
+Version: 0.2.4
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
```

### Comparing `pgqueuer-0.2.3/README.md` & `pgqueuer-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/pyproject.toml` & `pgqueuer-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/src/PgQueuer/cli.py` & `pgqueuer-0.2.4/src/PgQueuer/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import argparse
 import asyncio
 import os
 from datetime import timedelta
 
 import asyncpg
-from tabulate import tabulate
+from tabulate import tabulate, tabulate_formats
 
 from PgQueuer.models import LogStatistics
 from PgQueuer.queries import Queries
 
 
-async def display_stats(log_stats: list[LogStatistics]) -> None:
+async def display_stats(
+    log_stats: list[LogStatistics],
+    tablefmt: str,
+) -> None:
     print(
         tabulate(
             [
                 (
                     stat.created,
                     stat.count,
                     stat.entrypoint,
@@ -28,29 +31,30 @@
                 "Created",
                 "Count",
                 "Entrypoint",
                 "Time in Queue (HH:MM:SS)",
                 "Status",
                 "Priority",
             ],
-            tablefmt="pretty",
+            tablefmt=tablefmt,
         )
     )
 
 
 async def fetch_and_dispay(
     queries: Queries,
     interval: timedelta | None,
     tail: int,
+    tablefmt: str,
 ) -> None:
     clear_and_home = "\033[2J\033[H"
     while True:
         print(clear_and_home, end="")
         stats = await queries.log_statistics(tail)  # Fetch stats once and reuse
-        await display_stats(stats)
+        await display_stats(stats, tablefmt)
         if interval is None:
             return
         await asyncio.sleep(interval.total_seconds())
 
 
 def cliparser() -> argparse.Namespace:
     common_arguments = argparse.ArgumentParser(
@@ -161,14 +165,23 @@
     dashboardparser.add_argument(
         "-n",
         "--tail",
         help="The number of the most recent log entries to display on the dashboard.",
         type=int,
         default=25,
     )
+    dashboardparser.add_argument(
+        "--table-format",
+        default="pretty",
+        help=(
+            "Specify the format of the table used to display statistics. "
+            "Options are provided by the tabulate library."
+        ),
+        choices=tabulate_formats,
+    )
 
     return parser.parse_args()
 
 
 async def main() -> None:
     parsed = cliparser()
 
@@ -182,20 +195,23 @@
     async with asyncpg.create_pool(
         parsed.pg_dsn,
         database=parsed.pg_database,
         password=parsed.pg_password,
         port=parsed.pg_port,
         user=parsed.pg_user,
         host=parsed.pg_host,
+        max_size=1,
+        min_size=0,
     ) as pool:
         queries = Queries(pool)
         match parsed.command:
             case "install":
                 await queries.install()
             case "uninstall":
                 await queries.uninstall()
             case "dashboard":
                 await fetch_and_dispay(
                     queries,
                     parsed.interval,
                     parsed.tail,
+                    parsed.table_format,
                 )
```

### Comparing `pgqueuer-0.2.3/src/PgQueuer/models.py` & `pgqueuer-0.2.4/src/PgQueuer/models.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/src/PgQueuer/qm.py` & `pgqueuer-0.2.4/src/PgQueuer/qm.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,24 +107,23 @@
         self,
         dequeue_timeout: timedelta = timedelta(seconds=30),
     ) -> None:
         """
         Continuously listens for events and dispatches jobs. Manages connections and
         tasks, logs timeouts, and resets connections upon termination.
         """
-
         async with (
             self.pool.acquire() as conn,
             TaskManager() as tm,
         ):
             listener = PGEventQueue()
             await listener.connect(conn, self.channel)
 
             while self.alive:
-                while job := await self.queries.dequeue():
+                while self.alive and (job := await self.queries.dequeue()):
                     tm.add(asyncio.create_task(self._dispatch(job)))
 
                 try:
                     await asyncio.wait_for(
                         listener.get(),
                         timeout=dequeue_timeout.total_seconds(),
                     )
```

### Comparing `pgqueuer-0.2.3/src/PgQueuer/queries.py` & `pgqueuer-0.2.4/src/PgQueuer/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         if row := await self.pool.fetchrow(query):
             return models.Job.model_validate(dict(row))
         return None
 
     async def enqueue(
         self,
         entrypoint: str | list[str],
-        payload: bytes | None | list[bytes | None],
+        payload: bytes | None | list[bytes] | list[None] | list[bytes | None],
         priority: int | list[int] = 0,
     ) -> None:
         """
         Inserts a new job into the queue with the specified
         entrypoint, payload, and priority, marking it as 'queued'.
         This method ensures that if any of entrypoint, payload, or priority is a list,
         all list arguments must be of the same length.
```

### Comparing `pgqueuer-0.2.3/src/PgQueuer/tm.py` & `pgqueuer-0.2.4/src/PgQueuer/tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/src/PgQueuer.egg-info/PKG-INFO` & `pgqueuer-0.2.4/src/PgQueuer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PgQueuer
-Version: 0.2.3
+Version: 0.2.4
 Summary: PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
 Author: janbjorge
 License: MIT License
 Project-URL: Documentation, https://github.com/janbjorge/PgQueuer/
 Project-URL: Homepage, https://github.com/janbjorge/PgQueuer/
 Project-URL: Issues, https://github.com/janbjorge/PgQueuer/issues
 Project-URL: Repository, https://github.com/janbjorge/PgQueuer/
```

### Comparing `pgqueuer-0.2.3/src/PgQueuer.egg-info/SOURCES.txt` & `pgqueuer-0.2.4/src/PgQueuer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/test/conftest.py` & `pgqueuer-0.2.4/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/test/db/Dockerfile` & `pgqueuer-0.2.4/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/test/test_qm.py` & `pgqueuer-0.2.4/test/test_qm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/test/test_queries.py` & `pgqueuer-0.2.4/test/test_queries.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.2.3/test/test_tm.py` & `pgqueuer-0.2.4/test/test_tm.py`

 * *Files identical despite different names*

