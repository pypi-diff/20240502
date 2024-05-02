# Comparing `tmp/svinsight-0.3.4.tar.gz` & `tmp/svinsight-0.3.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svinsight-0.3.4.tar", last modified: Mon Apr 29 14:19:27 2024, max compression
+gzip compressed data, was "svinsight-0.3.62.tar", max compression
```

## Comparing `svinsight-0.3.4.tar` & `svinsight-0.3.62.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:19:27.220581 svinsight-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 14:19:22.000000 svinsight-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 14:19:27.220581 svinsight-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-29 14:19:22.000000 svinsight-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:19:27.220581 svinsight-0.3.4/SVInsight/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-29 14:19:22.000000 svinsight-0.3.4/SVInsight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-29 14:19:22.000000 svinsight-0.3.4/SVInsight/census_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    76953 2024-04-29 14:19:22.000000 svinsight-0.3.4/SVInsight/svi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:19:27.220581 svinsight-0.3.4/SVInsight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 14:19:27.000000 svinsight-0.3.4/SVInsight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-29 14:19:27.000000 svinsight-0.3.4/SVInsight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:19:27.000000 svinsight-0.3.4/SVInsight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 14:19:27.000000 svinsight-0.3.4/SVInsight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 14:19:22.000000 svinsight-0.3.4/long_desc.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 14:19:22.000000 svinsight-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:19:27.224581 svinsight-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:19:27.220581 svinsight-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-29 14:19:22.000000 svinsight-0.3.4/tests/test_svinsight.py
+-rw-r--r--   0        0        0     1073 2024-05-01 17:05:45.110819 svinsight-0.3.62/LICENSE
+-rw-r--r--   0        0        0      111 2024-05-01 17:05:45.310820 svinsight-0.3.62/long_desc.md
+-rw-r--r--   0        0        0      547 2024-05-01 17:05:45.310820 svinsight-0.3.62/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-05-01 17:05:45.310820 svinsight-0.3.62/svinsight/__init__.py
+-rw-r--r--   0        0        0    17061 2024-05-01 17:05:45.310820 svinsight-0.3.62/svinsight/census_variables.py
+-rw-r--r--   0        0        0    77547 2024-05-01 17:05:45.310820 svinsight-0.3.62/svinsight/svi.py
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 svinsight-0.3.62/PKG-INFO
```

### Comparing `svinsight-0.3.4/LICENSE` & `svinsight-0.3.62/LICENSE`

 * *Files identical despite different names*

### Comparing `svinsight-0.3.4/SVInsight/census_variables.py` & `svinsight-0.3.62/svinsight/census_variables.py`

 * *Files identical despite different names*

### Comparing `svinsight-0.3.4/SVInsight/svi.py` & `svinsight-0.3.62/svinsight/svi.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 
             return output
     
 
     # Method to pull census data and fill holes
     def census_data(self, boundary: str = 'bg', year: int = 2019, interpolate: bool = True, verbose: bool = False, overwrite: bool = False):
         """
-        Pulls Census data for a specific boundary and year.
+        Pulls Census data for a specific boundary and year. The Census API can sometimes error out. Waiting a few seconds/minutes and re-running should solve the issue. 
 
         :param boundary: The boundary type to retrieve data for. Valid options are 'bg' (block group) and 'tract' (census tract).
         :type boundary: str
         :param year: The year of the Census data to retrieve. Valid options are from 2011 to 2021.
         :type year: int
         :param interpolate: Whether to interpolate missing data. Defaults to True. If year is before 2014, ignored and not-interpolated.
         :type interpolate: bool, optional
@@ -1075,14 +1075,26 @@
                 data_pre = c.acs5.state_county_blockgroup(var, state, county, Census.ALL, year=year)
             elif boundary == 'tract':
                 data_pre = c.acs5.state_county_tract(var, state, county, Census.ALL, year=year)
             else:
                 data_pre = c.acs5.state_county(var, state, county, year=year)
             return data_pre
         
+           # TODO: Add retry attempt
+            # import time
+            # for i in range(5):
+            #     try:
+            #         data_pre = c.acs5.state_county_blockgroup(var, state, county, Census.ALL, year=year)
+            #         break
+            #     except Exception as e:
+            #         print(f"Attempt {i+1} failed with error: {e}")
+            #         if i < 4:  # Don't sleep after the last attempt
+            #             time.sleep(5)
+
+        
         for geoid in geoids:
             if len(geoid) == 2:
                 county = Census.ALL
                 state = geoid
             else:
                 county = int(geoid[2:])
                 state = int(geoid[:2])
```

