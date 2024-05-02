# Comparing `tmp/atspm-1.2.0.tar.gz` & `tmp/atspm-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atspm-1.2.0.tar", last modified: Thu Apr 18 18:49:37 2024, max compression
+gzip compressed data, was "atspm-1.3.0a1.tar", last modified: Thu May  2 16:46:50 2024, max compression
```

## Comparing `atspm-1.2.0.tar` & `atspm-1.3.0a1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.290141 atspm-1.2.0/
--rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 atspm-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       85 2024-04-12 01:08:02.000000 atspm-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3441 2024-04-18 18:49:37.290141 atspm-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2024-04-18 18:32:57.000000 atspm-1.2.0/README.md
--rw-rw-rw-   0        0        0      568 2024-04-18 18:06:31.000000 atspm-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 18:49:37.290141 atspm-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.243796 atspm-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.258886 atspm-1.2.0/src/atspm/
--rw-rw-rw-   0        0        0       92 2024-04-18 18:05:56.000000 atspm-1.2.0/src/atspm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.274579 atspm-1.2.0/src/atspm/data/
--rw-rw-rw-   0        0        0     3321 2024-04-18 18:01:38.000000 atspm-1.2.0/src/atspm/data/sample_config.parquet
--rw-rw-rw-   0        0        0   271222 2024-04-16 00:47:05.000000 atspm-1.2.0/src/atspm/data/sample_raw_data.parquet
--rw-rw-rw-   0        0        0      999 2024-04-16 16:12:10.000000 atspm-1.2.0/src/atspm/data_aggregator.py
--rw-rw-rw-   0        0        0     1792 2024-04-18 17:11:03.000000 atspm-1.2.0/src/atspm/data_loader.py
--rw-rw-rw-   0        0        0     1326 2024-04-18 17:49:58.000000 atspm-1.2.0/src/atspm/data_saver.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.274579 atspm-1.2.0/src/atspm/queries/
--rw-rw-rw-   0        0        0      406 2024-04-16 01:24:53.000000 atspm-1.2.0/src/atspm/queries/actuations.sql
--rw-rw-rw-   0        0        0     3867 2024-04-18 16:10:41.000000 atspm-1.2.0/src/atspm/queries/arrival_on_green.sql
--rw-rw-rw-   0        0        0      532 2024-04-16 01:24:58.000000 atspm-1.2.0/src/atspm/queries/communications.sql
--rw-rw-rw-   0        0        0      409 2024-04-15 21:20:28.000000 atspm-1.2.0/src/atspm/queries/coordination.sql
--rw-rw-rw-   0        0        0     2602 2024-04-17 00:12:30.000000 atspm-1.2.0/src/atspm/queries/detector_faults.sql
--rw-rw-rw-   0        0        0      668 2024-04-18 01:09:44.000000 atspm-1.2.0/src/atspm/queries/ped.sql
--rw-rw-rw-   0        0        0    10285 2024-04-16 21:28:57.000000 atspm-1.2.0/src/atspm/queries/split_failures.sql
--rw-rw-rw-   0        0        0      376 2024-04-18 13:37:09.000000 atspm-1.2.0/src/atspm/queries/splits.sql
--rw-rw-rw-   0        0        0      571 2024-04-16 01:25:11.000000 atspm-1.2.0/src/atspm/queries/terminations.sql
--rw-rw-rw-   0        0        0     1017 2024-04-18 15:20:29.000000 atspm-1.2.0/src/atspm/queries/unique_ped.sql
--rw-rw-rw-   0        0        0     4776 2024-04-18 16:01:23.000000 atspm-1.2.0/src/atspm/queries/yellow_red.sql
--rw-rw-rw-   0        0        0      493 2024-04-18 18:04:49.000000 atspm-1.2.0/src/atspm/sample_data.py
--rw-rw-rw-   0        0        0     2261 2024-04-18 17:44:46.000000 atspm-1.2.0/src/atspm/signal_data_processor.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:49:37.290141 atspm-1.2.0/src/atspm.egg-info/
--rw-rw-rw-   0        0        0     3441 2024-04-18 18:49:37.000000 atspm-1.2.0/src/atspm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2024-04-18 18:49:37.000000 atspm-1.2.0/src/atspm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 18:49:37.000000 atspm-1.2.0/src/atspm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-18 18:49:37.000000 atspm-1.2.0/src/atspm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.528613 atspm-1.3.0a1/
+-rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 atspm-1.3.0a1/LICENSE
+-rw-rw-rw-   0        0        0       85 2024-04-12 01:08:02.000000 atspm-1.3.0a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3481 2024-05-02 16:46:50.528613 atspm-1.3.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0     2968 2024-04-18 18:32:57.000000 atspm-1.3.0a1/README.md
+-rw-rw-rw-   0        0        0      627 2024-05-02 16:44:22.000000 atspm-1.3.0a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 16:46:50.529610 atspm-1.3.0a1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.451997 atspm-1.3.0a1/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.486880 atspm-1.3.0a1/src/atspm/
+-rw-rw-rw-   0        0        0       92 2024-04-18 18:05:56.000000 atspm-1.3.0a1/src/atspm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.507681 atspm-1.3.0a1/src/atspm/data/
+-rw-rw-rw-   0        0        0     3321 2024-04-18 18:01:38.000000 atspm-1.3.0a1/src/atspm/data/sample_config.parquet
+-rw-rw-rw-   0        0        0   271222 2024-04-16 00:47:05.000000 atspm-1.3.0a1/src/atspm/data/sample_raw_data.parquet
+-rw-rw-rw-   0        0        0     1270 2024-05-01 17:20:10.000000 atspm-1.3.0a1/src/atspm/data_aggregator.py
+-rw-rw-rw-   0        0        0     1749 2024-05-01 21:44:28.000000 atspm-1.3.0a1/src/atspm/data_loader.py
+-rw-rw-rw-   0        0        0     1326 2024-04-18 17:49:58.000000 atspm-1.3.0a1/src/atspm/data_saver.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.526620 atspm-1.3.0a1/src/atspm/queries/
+-rw-rw-rw-   0        0        0      348 2024-05-01 17:51:34.000000 atspm-1.3.0a1/src/atspm/queries/actuations.sql
+-rw-rw-rw-   0        0        0     3683 2024-05-01 18:13:20.000000 atspm-1.3.0a1/src/atspm/queries/arrival_on_green.sql
+-rw-rw-rw-   0        0        0      508 2024-05-01 18:16:22.000000 atspm-1.3.0a1/src/atspm/queries/communications.sql
+-rw-rw-rw-   0        0        0      447 2024-05-01 18:22:39.000000 atspm-1.3.0a1/src/atspm/queries/coordination.sql
+-rw-rw-rw-   0        0        0     2537 2024-05-01 22:20:36.000000 atspm-1.3.0a1/src/atspm/queries/detector_faults.sql
+-rw-rw-rw-   0        0        0      907 2024-05-01 16:24:38.000000 atspm-1.3.0a1/src/atspm/queries/has_data.sql
+-rw-rw-rw-   0        0        0      694 2024-05-01 22:26:09.000000 atspm-1.3.0a1/src/atspm/queries/ped.sql
+-rw-rw-rw-   0        0        0    10634 2024-05-02 16:35:05.000000 atspm-1.3.0a1/src/atspm/queries/split_failures.sql
+-rw-rw-rw-   0        0        0      408 2024-05-01 23:51:36.000000 atspm-1.3.0a1/src/atspm/queries/splits.sql
+-rw-rw-rw-   0        0        0      584 2024-05-01 23:54:46.000000 atspm-1.3.0a1/src/atspm/queries/terminations.sql
+-rw-rw-rw-   0        0        0     1037 2024-05-01 23:56:18.000000 atspm-1.3.0a1/src/atspm/queries/unique_ped.sql
+-rw-rw-rw-   0        0        0     4724 2024-05-02 00:27:14.000000 atspm-1.3.0a1/src/atspm/queries/yellow_red.sql
+-rw-rw-rw-   0        0        0      493 2024-04-18 18:04:49.000000 atspm-1.3.0a1/src/atspm/sample_data.py
+-rw-rw-rw-   0        0        0     4602 2024-05-02 16:43:31.000000 atspm-1.3.0a1/src/atspm/signal_data_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.527616 atspm-1.3.0a1/src/atspm.egg-info/
+-rw-rw-rw-   0        0        0     3481 2024-05-02 16:46:50.000000 atspm-1.3.0a1/src/atspm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      850 2024-05-02 16:46:50.000000 atspm-1.3.0a1/src/atspm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 16:46:50.000000 atspm-1.3.0a1/src/atspm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-02 16:46:50.000000 atspm-1.3.0a1/src/atspm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 16:46:50.000000 atspm-1.3.0a1/src/atspm.egg-info/top_level.txt
```

### Comparing `atspm-1.2.0/LICENSE` & `atspm-1.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `atspm-1.2.0/PKG-INFO` & `atspm-1.3.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: atspm
-Version: 1.2.0
+Version: 1.3.0a1
 Summary: Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures.
 Author-email: Shawn Strasser <shawn.strasser@odot.oregon.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: duckdb<0.10.2,>=0.9.1
 
 # ATSPM Aggregation
 
 `atspm` is a Python package to transform hi-res ATC signal controller data into aggregate ATSPMs (Automated Traffic Signal Performance Measures). It works on multiple devices/detectors at once.
 
 ## Installation
```

### Comparing `atspm-1.2.0/README.md` & `atspm-1.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `atspm-1.2.0/pyproject.toml` & `atspm-1.3.0a1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [project]
 name = "atspm"
-version = "1.2.0"
+version = "1.3.0alpha1"
 authors = [
   { name="Shawn Strasser", email="shawn.strasser@odot.oregon.gov" },
 ]
 description = "Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+    "duckdb>=0.9.1,<0.10.2",
+]
+
 [tools.setuptools]
 include_package_data = true
 package_data = {"atspm" = ["queries/*", "data/*"]}
```

### Comparing `atspm-1.2.0/src/atspm/data/sample_config.parquet` & `atspm-1.3.0a1/src/atspm/data/sample_config.parquet`

 * *Files identical despite different names*

### Comparing `atspm-1.2.0/src/atspm/data/sample_raw_data.parquet` & `atspm-1.3.0a1/src/atspm/data/sample_raw_data.parquet`

 * *Files identical despite different names*

### Comparing `atspm-1.2.0/src/atspm/data_aggregator.py` & `atspm-1.3.0a1/src/atspm/data_aggregator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import os
 from jinja2 import Environment, FileSystemLoader
-from .data_saver import save_data
-
 
 def render_query(query_name, **kwargs):
-    print(query_name)
     # add from_table = 'raw_data' to the kwargs dictionary
     kwargs['from_table'] = 'raw_data'
     # Get the directory that contains the SQL templates
     template_dir = os.path.join(os.path.dirname(__file__), 'queries')
     # Create a Jinja2 environment with the FileSystemLoader
     env = Environment(loader=FileSystemLoader(template_dir))
     # Get the template by name
     template = env.get_template(f"{query_name}.sql")
     #print(template)
     # Render the template with the provided keyword arguments
     return template.render(**kwargs)
 
 def aggregate_data(conn, aggregation_name, **kwargs):
     query = render_query(aggregation_name, **kwargs)
-    #if aggregation_name == 'split_failures':
+    if aggregation_name != 'has_data' and kwargs['remove_incomplete']:
+        # Add natural join with has_data table
+        query = f"SELECT * FROM ({query}) main_query NATURAL JOIN has_data"
+    query = f"CREATE OR REPLACE TABLE {aggregation_name} AS {query};"
+    #print(query)
+    try:
+        conn.execute(query)
+    except Exception as e:
+        print('Error when executing query for: ', aggregation_name)
+        print(e)
+        #print('\n\nQuery:\n')
         #print(query)
-    query = f"CREATE OR REPLACE TABLE {aggregation_name} AS {query}"
-    conn.execute(query)
```

### Comparing `atspm-1.2.0/src/atspm/data_loader.py` & `atspm-1.3.0a1/src/atspm/data_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,13 @@
         If raw_data or detector_config is a string and the file does not exist.
     """
     # Check if raw_data is an instance of str
     if isinstance(raw_data, str):
         conn.execute(f"CREATE OR REPLACE TABLE raw_data AS SELECT * FROM '{raw_data}'")
     else:
         conn.execute(f"CREATE OR REPLACE TABLE raw_data AS SELECT * FROM raw_data")
-    print("Raw data loaded successfully")
     # Check that detector_config is not None
     if detector_config is not None:
         if isinstance(detector_config, str):
             conn.execute(f"CREATE OR REPLACE TABLE detector_config AS SELECT * FROM '{detector_config}'")
         else:
             conn.execute(f"CREATE OR REPLACE TABLE detector_config AS SELECT * FROM detector_config")
```

### Comparing `atspm-1.2.0/src/atspm/data_saver.py` & `atspm-1.3.0a1/src/atspm/data_saver.py`

 * *Files identical despite different names*

### Comparing `atspm-1.2.0/src/atspm/queries/arrival_on_green.sql` & `atspm-1.3.0a1/src/atspm/queries/arrival_on_green.sql`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     -- This is for arrival on green, or yellow/red actuation, where we only need detector ON events
     -- It shift timestamps back to account for latency
     -- And joins Phase Number to each Detector Event
     -- Rename parameter as Detector to avoid cofusion
     SELECT d.TimeStamp - INTERVAL ({{latency_offset_seconds}} * 1000) MILLISECOND as TimeStamp,
         d.DeviceId, 
         d.EventId, 
-        0 as Detector, --combine detectors by phase
-        CAST(c.Phase AS UTINYINT) AS Phase
+        c.Phase::int16 AS Phase,
     FROM {{from_table}} AS d
     JOIN detector_config AS c ON 
         d.DeviceId = c.DeviceId 
         AND d.Parameter = c.Parameter
     WHERE EventId = 82 
         AND c.Function = 'Advance'
 ),
@@ -25,16 +24,15 @@
     -- phase_with_detector_ByApproach
     -- Combined phase and detector data without duplicating phase data (no need since detector/phases are combined already)
     WITH 
     phase AS (
         SELECT TimeStamp, 
             DeviceId, 
             EventId,
-            0 as Detector,
-            Parameter AS Phase 
+            Parameter::int16 AS Phase 
         FROM {{from_table}}
         WHERE EventId IN (1, 8, 10)
     )
     SELECT * FROM phase
     UNION ALL
     SELECT * FROM view1
 ),
@@ -47,50 +45,49 @@
             CASE WHEN EventId = 1 THEN 1 ELSE 0 END AS Cycle_Number_Mask,
             CASE WHEN EventId < 81 THEN EventId ELSE 0 END AS Signal_State_Mask,
             CASE WHEN EventId = 81 THEN 0 WHEN EventId =82 THEN 1 END AS Detector_State_Change
         FROM view2
     ),
     step2 as (
         SELECT *,
-            CAST(SUM(Cycle_Number_Mask) OVER (PARTITION BY DeviceId, Detector, Phase ORDER BY TimeStamp, EventId) AS UINTEGER) AS Cycle_Number,
-            COUNT(Detector_State_Change) OVER (PARTITION BY DeviceId, Detector, Phase ORDER BY TimeStamp, EventId) AS Detector_Group
+            CAST(SUM(Cycle_Number_Mask) OVER (PARTITION BY DeviceId, Phase ORDER BY TimeStamp, EventId) AS UINTEGER) AS Cycle_Number,
+            COUNT(Detector_State_Change) OVER (PARTITION BY DeviceId, Phase ORDER BY TimeStamp, EventId) AS Detector_Group
             FROM step1
     )
     SELECT TimeStamp,
         DeviceId, 
         EventId, 
-        Detector,
         Phase,
         Cycle_Number,
-        CAST(MAX(Signal_State_Mask) OVER (PARTITION BY DeviceId, Detector, Phase, Cycle_Number ORDER BY TimeStamp, EventId) AS UTINYINT) AS Signal_State,
-        CAST(MAX(Detector_State_Change) OVER (PARTITION BY DeviceId, Detector, Phase, Detector_Group ORDER BY TimeStamp, EventId) AS BOOL) AS Detector_State--, Detector_Group, Detector_State_Mask
+        CAST(MAX(Signal_State_Mask) OVER (PARTITION BY DeviceId, Phase, Cycle_Number ORDER BY TimeStamp, EventId) AS UTINYINT) AS Signal_State,
+        CAST(MAX(Detector_State_Change) OVER (PARTITION BY DeviceId, Phase, Detector_Group ORDER BY TimeStamp, EventId) AS BOOL) AS Detector_State
     FROM step2
 ),
 
 view4 AS (
     -- arrival_on_green
     -- Transforms actuations into arrivals on green after they've been asssigned a signal state
     WITH green AS (
         SELECT
             time_bucket(interval '{{bin_size}} minutes', TimeStamp) as Rounded_TimeStamp,
             DeviceId,
             Phase,
-            COUNT(*)::uint16 as Green_Actuations
+            COUNT(*)::int16 as Green_Actuations
         FROM view3
         WHERE
             EventId = 82
             and Signal_State = 1
         GROUP BY Rounded_TimeStamp, DeviceId, Phase
     ),
     not_green AS(
         SELECT
             time_bucket(interval '{{bin_size}} minutes', TimeStamp) as Rounded_TimeStamp,
             DeviceId,
             Phase,
-            COUNT(*)::uint16 as Total_Actuations
+            COUNT(*)::int16 as Total_Actuations
         FROM view3
         WHERE
             EventId = 82
         GROUP BY Rounded_TimeStamp, DeviceId, Phase
     )
     SELECT
         g.Rounded_TimeStamp as TimeStamp,
```

### Comparing `atspm-1.2.0/src/atspm/queries/ped.sql` & `atspm-1.3.0a1/src/atspm/queries/ped.sql`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 --Aggregate Pedestiran Services and Actuations 
 --Written in SQL for DuckDB. This is a jinja2 template, with variables inside curly braces.
 
 SELECT *
 FROM (
 	SELECT 
 		TimeStamp, 
-		DeviceID, 
-		Parameter AS Phase, 
-		COALESCE("21", 0) + COALESCE("67", 0) AS PedServices, 
-		COALESCE("90", 0) AS PedActuation
+		DeviceId, 
+		Parameter::int16 AS Phase, 
+		COALESCE("21", 0)::int16 + COALESCE("67", 0)::int16 AS PedServices, 
+		COALESCE("90", 0)::int16 AS PedActuation
 	FROM (
 		SELECT 
 			TIME_BUCKET(interval '15 minutes', TimeStamp) AS TimeStamp, 
-			DeviceID, 
-			EventID, 
-			Parameter, 
+			DeviceId, 
+			EventId, 
+			Parameter,
 			COUNT(*) AS Total
 		FROM 
 			{{from_table}}
 		GROUP BY ALL
 	) q
 	PIVOT (
 		SUM(Total) FOR EventID IN (21 AS "21", 90 AS "90", 67 AS "67")
 	)
 ) subquery
 WHERE 
 	PedServices > 0 
-	OR PedActuation > 0;
+	OR PedActuation > 0
```

### Comparing `atspm-1.2.0/src/atspm/queries/split_failures.sql` & `atspm-1.3.0a1/src/atspm/queries/split_failures.sql`

 * *Files 12% similar despite different names*

```diff
@@ -295,15 +295,23 @@
         CAST(Green_ON + Green_OFF AS FLOAT) / 1000 AS Green_Time,
         CAST(Green_ON AS FLOAT) / (Green_ON + Green_OFF) AS Green_Occupancy,
         CAST(Red_5_ON AS FLOAT) / {{red_time}}000 AS Red_Occupancy
     FROM step1b
 )
 
 
-SELECT *,
-CASE WHEN 
-    Red_Occupancy>={{red_occupancy_threshold}}
-    AND Green_Occupancy>={{green_occupancy_threshold}}
-    THEN True ELSE False END AS Split_Failure
-FROM step8;
-
---select * from step3
+SELECT 
+    time_bucket(interval '{{bin_size}} minutes', TimeStamp) as TimeStamp,
+    DeviceId,
+    {% if not by_approach %}
+    Detector::int16 as Detector,
+    {% endif %}
+    Phase::int16 as Phase,
+    AVG(Green_Time)::float as Green_Time,
+    AVG(Green_Occupancy)::float as Green_Occupancy,
+    AVG(Red_Occupancy)::float as Red_Occupancy,
+    SUM(CASE WHEN 
+        Red_Occupancy>={{red_occupancy_threshold}}
+        AND Green_Occupancy>={{green_occupancy_threshold}}
+        THEN 1 ELSE 0 END)::int16 AS Split_Failure
+FROM step8
+GROUP BY ALL
```

### Comparing `atspm-1.2.0/src/atspm/queries/terminations.sql` & `atspm-1.3.0a1/src/atspm/queries/terminations.sql`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 --Aggregate terminations (GapOut, MaxOut, ForceOff, and also, PhaseCall for some reason)
 --Written in SQL for DuckDB. This is a jinja2 template, with variables inside curly braces.
 
 SELECT
     time_bucket(interval '{{bin_size}} minutes', TimeStamp) as TimeStamp,
     DeviceId as DeviceId,
-    Parameter as Phase,
+    Parameter::int16 as Phase,
     CASE 
         WHEN EventId = 4 THEN 'GapOut'
         WHEN EventId = 5 THEN 'MaxOut'
         WHEN EventId = 6 THEN 'ForceOff'
     END AS PerformanceMeasure,
-    COUNT(*) as Total
+    COUNT(*)::int16 as Total
 FROM {{from_table}}
 WHERE EventId IN (4, 5, 6) 
-GROUP BY ALL;
+GROUP BY ALL
```

### Comparing `atspm-1.2.0/src/atspm/queries/unique_ped.sql` & `atspm-1.3.0a1/src/atspm/queries/unique_ped.sql`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 --The intention of "unique" actuations is that back-to-back actuations from the same person are removed
 --The default time lapse before a new unique actuation for a given ped phase may be counted is 15 seconds
 --see this study: https://doi.org/10.1177/0361198121994126
 
 SELECT
     TimeStamp,
-    DeviceID, 
+    DeviceId, 
     Phase,
-    COUNT(*) as Unique_Actuations
+    COUNT(*)::int16 as Unique_Actuations
 FROM
     (SELECT 
         TIME_BUCKET(interval '15 minutes', TimeStamp) as TimeStamp,
         DeviceId,
-        Parameter as Phase,
-        DATEDIFF('MILLISECOND', LAG(TimeStamp) OVER (PARTITION BY DeviceID, Parameter ORDER BY TimeStamp), TimeStamp) as Diff_Milliseconds    
+        Parameter::int16 as Phase,
+        DATEDIFF('MILLISECOND', LAG(TimeStamp) OVER (PARTITION BY DeviceID, Parameter ORDER BY TimeStamp), TimeStamp)::float as Diff_Milliseconds    
     FROM 
         {{from_table}}
     WHERE
-        EventID = 90
+        EventId = 90
     ) q
 WHERE
     q.Diff_Milliseconds > {{seconds_between_actuations}}000 --convert seconds to milliseconds
 GROUP BY
-    TimeStamp, DeviceID, Phase;
+    TimeStamp, DeviceID, Phase
```

### Comparing `atspm-1.2.0/src/atspm/queries/yellow_red.sql` & `atspm-1.3.0a1/src/atspm/queries/yellow_red.sql`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,16 @@
     -- detector_with_phase_ON_ONLY
     -- This is for arrival on green, or yellow/red actuation, where we only need detector ON events
     -- It shift timestamps back to account for latency
     -- And joins Phase Number to each Detector Event
     -- Rename parameter as Detector to avoid cofusion
     SELECT d.TimeStamp - INTERVAL ({{latency_offset_seconds}} * 1000) MILLISECOND as TimeStamp,
         d.DeviceId, 
-        d.EventId, 
-        0 as Detector, --combine detectors by phase
-        CAST(c.Phase AS UTINYINT) AS Phase
+        d.EventId::int16 AS EventId, 
+        c.Phase::int16 AS Phase
     FROM {{from_table}} AS d
     JOIN detector_config AS c ON 
         d.DeviceId = c.DeviceId 
         AND d.Parameter = c.Parameter
     WHERE EventId = 82 
         AND c.Function = 'Yellow_Red'
 ),
@@ -23,17 +22,16 @@
 view2 AS (
     -- phase_with_detector_ByApproach
     -- Combined phase and detector data without duplicating phase data (no need since detector/phases are combined already)
     WITH 
     phase AS (
         SELECT TimeStamp, 
             DeviceId, 
-            EventId,
-            0 as Detector,
-            Parameter AS Phase 
+            EventId::int16 AS EventId,
+            Parameter::int16 AS Phase 
         FROM {{from_table}}
         WHERE EventId IN (1, 8, 10)
     )
     SELECT * FROM phase
     UNION ALL
     SELECT * FROM view1
 ),
@@ -46,26 +44,25 @@
             CASE WHEN EventId = 1 THEN 1 ELSE 0 END AS Cycle_Number_Mask,
             CASE WHEN EventId < 81 THEN EventId ELSE 0 END AS Signal_State_Mask,
             CASE WHEN EventId = 81 THEN 0 WHEN EventId =82 THEN 1 END AS Detector_State_Change
         FROM view2
     ),
     step2 as (
         SELECT *,
-            CAST(SUM(Cycle_Number_Mask) OVER (PARTITION BY DeviceId, Detector, Phase ORDER BY TimeStamp, EventId) AS UINTEGER) AS Cycle_Number,
-            COUNT(Detector_State_Change) OVER (PARTITION BY DeviceId, Detector, Phase ORDER BY TimeStamp, EventId) AS Detector_Group
+            SUM(Cycle_Number_Mask) OVER (PARTITION BY DeviceId, Phase ORDER BY TimeStamp, EventId) AS Cycle_Number,
+            COUNT(Detector_State_Change) OVER (PARTITION BY DeviceId, Phase ORDER BY TimeStamp, EventId) AS Detector_Group
             FROM step1
     )
     SELECT TimeStamp,
         DeviceId, 
         EventId, 
-        Detector,
         Phase,
         Cycle_Number,
-        CAST(MAX(Signal_State_Mask) OVER (PARTITION BY DeviceId, Detector, Phase, Cycle_Number ORDER BY TimeStamp, EventId) AS UTINYINT) AS Signal_State,
-        CAST(MAX(Detector_State_Change) OVER (PARTITION BY DeviceId, Detector, Phase, Detector_Group ORDER BY TimeStamp, EventId) AS BOOL) AS Detector_State--, Detector_Group, Detector_State_Mask
+        MAX(Signal_State_Mask) OVER (PARTITION BY DeviceId, Phase, Cycle_Number ORDER BY TimeStamp, EventId)::int16 AS Signal_State,
+        CAST(MAX(Detector_State_Change) OVER (PARTITION BY DeviceId, Phase, Detector_Group ORDER BY TimeStamp, EventId) AS BOOL) AS Detector_State--, Detector_Group, Detector_State_Mask
     FROM step2
 ),
 
 view4 AS (
     -- valid_cycles
     -- remove cycles where there is not exactly one EventId equal to 1, 8, and 10
     -- this is to remove cycles where there is missing data for yellow_red actuations. 
@@ -106,31 +103,34 @@
         SELECT 
             time_bucket(interval '15 minutes', Red_TimeStamp) as New_TimeStamp,
             DeviceId,
             Phase,
             Signal_State,
             --Red Offset is rounded to nearest half second. This was based on visual observation of the smoothness of rounding from 0.2 seconds to 1 second, seemed to look good
             ROUND(DATEDIFF('MILLISECOND', Red_TimeStamp, TimeStamp)::float * 2 / 1000) / 2 AS Red_Offset,
-            COUNT(*) as Count
+            COUNT(*)::float as Count
         FROM view4
         NATURAL JOIN begin_reds
         WHERE EventId=82
         GROUP BY
             New_TimeStamp,
             DeviceId,
             Phase,
             Signal_State,
             Red_Offset
     )
     SELECT 
         New_TimeStamp AS TimeStamp,
         DeviceId,
-        Phase,
+        Phase::int16 AS Phase,
         Signal_State,
         Red_Offset,
         Count
     FROM renamed_table
-    ORDER BY TimeStamp
+    {% if min_red_offset is defined %}
+    WHERE Red_Offset >= {{ min_red_offset }}
+    {% endif %}
+
 )
 
 
-SELECT * FROM view5 order by timestamp
+SELECT * FROM view5
```

### Comparing `atspm-1.2.0/src/atspm.egg-info/PKG-INFO` & `atspm-1.3.0a1/src/atspm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: atspm
-Version: 1.2.0
+Version: 1.3.0a1
 Summary: Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures.
 Author-email: Shawn Strasser <shawn.strasser@odot.oregon.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: duckdb<0.10.2,>=0.9.1
 
 # ATSPM Aggregation
 
 `atspm` is a Python package to transform hi-res ATC signal controller data into aggregate ATSPMs (Automated Traffic Signal Performance Measures). It works on multiple devices/detectors at once.
 
 ## Installation
```

### Comparing `atspm-1.2.0/src/atspm.egg-info/SOURCES.txt` & `atspm-1.3.0a1/src/atspm.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 src/atspm/data_loader.py
 src/atspm/data_saver.py
 src/atspm/sample_data.py
 src/atspm/signal_data_processor.py
 src/atspm.egg-info/PKG-INFO
 src/atspm.egg-info/SOURCES.txt
 src/atspm.egg-info/dependency_links.txt
+src/atspm.egg-info/requires.txt
 src/atspm.egg-info/top_level.txt
 src/atspm/data/sample_config.parquet
 src/atspm/data/sample_raw_data.parquet
 src/atspm/queries/actuations.sql
 src/atspm/queries/arrival_on_green.sql
 src/atspm/queries/communications.sql
 src/atspm/queries/coordination.sql
 src/atspm/queries/detector_faults.sql
+src/atspm/queries/has_data.sql
 src/atspm/queries/ped.sql
 src/atspm/queries/split_failures.sql
 src/atspm/queries/splits.sql
 src/atspm/queries/terminations.sql
 src/atspm/queries/unique_ped.sql
 src/atspm/queries/yellow_red.sql
```

