# Comparing `tmp/wbx_workspaces-1.1.1.tar.gz` & `tmp/wbx_workspaces-1.3.1.tar.gz`

## Comparing `wbx_workspaces-1.1.1.tar` & `wbx_workspaces-1.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/src/wbx_workspaces/__init__.py
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/src/wbx_workspaces/__main__.py
--rw-r--r--   0        0        0    13183 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/src/wbx_workspaces/wbx.py
--rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/src/wbx_workspaces/wbx_dataframe.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/src/wbx_workspaces/wbx_utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/LICENSE
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbx_workspaces-1.3.1/src/wbx_workspaces/__init__.py
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 wbx_workspaces-1.3.1/src/wbx_workspaces/__main__.py
+-rw-r--r--   0        0        0    13183 2020-02-02 00:00:00.000000 wbx_workspaces-1.3.1/src/wbx_workspaces/wbx.py
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 wbx_workspaces-1.3.1/src/wbx_workspaces/wbx_dataframe.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 wbx_workspaces-1.3.1/src/wbx_workspaces/wbx_utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wbx_workspaces-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 wbx_workspaces-1.3.1/LICENSE
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 wbx_workspaces-1.3.1/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 wbx_workspaces-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 wbx_workspaces-1.3.1/PKG-INFO
```

### Comparing `wbx_workspaces-1.1.1/src/wbx_workspaces/__main__.py` & `wbx_workspaces-1.3.1/src/wbx_workspaces/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,67 +36,65 @@
 ### Workspaces ### 
 ###################
 
 @click.command()
 @click.option('-c', '--csvfile', help='Save results to CSV file.')
 @click.option('-r', '--rawdata', is_flag=True, help='Show json raw data')
 def locations(csvfile, rawdata):
-    """ List locations IDs"""
-    # get data   
-    #
+    """ List locations IDs."""
     locDF=wbxdf.locationsDF()
     locDF.print(csvfile)        
     if (rawdata):
         pprint(locDF.jsonList)
 
+
 @click.command()
 @click.option('-l', '--location_id', help='Restrict list to location Id')
 @click.option('-c', '--csvfile', help='Save results to CSV file.')
 @click.option('-r', '--rawdata', is_flag=True, help='Show json raw data')
 def workspaces(csvfile, rawdata, location_id):
-    """ Get the list of workspaces in given location """
-    # get data   
-    #
+    """ List workspaces in given location. """
     workspacesDF=wbxdf.workspacesDF(location_id)
     workspacesDF.print(csvfile)        
     if (rawdata):
         pprint(workspacesDF.jsonList)
 
+
 @click.command()
 @click.option('-l', '--location_id', help='Restrict list to location Id')
 @click.option('-c', '--csvfile', help='Save results to CSV file.')
 def devices(csvfile, location_id):
-    """ Get the list of devices in given location """
-    # get data   
-    #
+    """ List devices in given location. """
     devicesDF=wbxdf.devicesDF(location_id)
-    devicesDF.print(csvfile)        
+    devicesDF.print(csvfile)      
+
 
 @click.command()
 @click.argument('device_id')
 @click.argument('name')
 def device_status(device_id, name):
-    """ Show device status """
-    # get data   
-    #
+    """ Show device status. """
     data=wbxr.get_wbx_data(f"xapi/status", f"?deviceId={device_id}&name={name}")
     pprint(data)        
 
+
 def print_metrics(workspace_id, metric, fmt):
     metricDF=wbxdf.metricsDF(workspace_id, metric)
     metricDF.print(fmt)
 
+
 @click.command()
 @click.argument('metric')
 @click.option('-l', '--location_id', help='Get metrics data for all workspaces under location ID')
 @click.option('-w', '--workspace_id', help='Get metrics data for specific workspace ID')
-@click.option('-f', '--fmt', help='Save to CSV or JSON file.')
-def metrics(metric, fmt, location_id="", workspace_id=""):
-    """ Gather yesteray's hourly peopleCount or timeUsed metric for a workspace or workspaces in a location"""
-
+# @click.option('-f', '--fmt', help='Save to CSV or JSON file.')
+@click.option('-a', '--aggreate', is_flag=True, help='Aggreate workspaces data in a single file. Only applicable to if --location_id is selected')
+def metrics(metric, aggreate=False, location_id="", workspace_id=""):
+    """ Gather yesteray's hourly peopleCount or timeUsed metric for a workspace or workspaces in a location.
+    """
     if ( not (location_id or workspace_id) ):
 
         print ( "I need a location or a workspace ID")
         return (400)
     
     match metric:
         case 'peopleCount':
@@ -104,22 +102,38 @@
         case 'timeUsed':
             pass
         case _ :
             print(f"{metric} value not supported")
             return(400)
         
     if (workspace_id):
-        print_metrics( workspace_id, metric, fmt )
+        print_metrics( workspace_id, metric, 'JSON' )
 
     elif (location_id):
+        aggreate_data=[]
         workspacesDF=wbxdf.workspacesDF(location_id)
-        workspace_items=workspacesDF.jsonList['items']
-        for workspace in workspace_items :
+        workspaces=workspacesDF.jsonList['items']
+        for workspace in workspaces :
             workspace_id = workspace['id']
-            print_metrics( workspace_id, metric, fmt )
+            if ( aggreate ):
+                print(f"Fetching metrics for Workspace {workspace_id}")
+                item = {}
+                metricsDF=wbxdf.metricsDF(workspace_id, metric)
+                item[metric] = metricsDF.jsonList
+                item['workspace'] = workspace
+                aggreate_data.append(item)
+            else :
+                print_metrics( workspace_id, metric, 'JSON' )
+        if ( aggreate ):
+            frm = wbx_utils.midnight_iso_ms(1)
+            fn=f"{metric}_{location_id}_{frm}.json"
+            with open(fn, "w") as jsfile:
+                jsfile.write(json.dumps(aggreate_data, indent=2))
+                print(f"Created {fn}")
+            
     
 #####################
 ### Top Lev       ###
 #####################
 
 @click.group()
 @click.version_option(__version__)
```

### Comparing `wbx_workspaces-1.1.1/src/wbx_workspaces/wbx.py` & `wbx_workspaces-1.3.1/src/wbx_workspaces/wbx.py`

 * *Files identical despite different names*

### Comparing `wbx_workspaces-1.1.1/src/wbx_workspaces/wbx_dataframe.py` & `wbx_workspaces-1.3.1/src/wbx_workspaces/wbx_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         # get row data
         self.jsonList = wbxr.get_wbx_data(f"workspaces", f"{params}")
         # pprint(self.jsonList)
         #
         # build DF 
         if 'items' in self.jsonList:
             for item in self.jsonList['items']:
-                ut.trace(3, f"Processing item {item}")
+                ut.trace(3, f"Processing workspace {item['id']}")
                 new_row={}
                 for f in self.cols:
                     if f in item:
                         new_row[f]=item[f]
                 self.df = pd.concat([self.df, pd.DataFrame([new_row])], ignore_index=True)
         else:
             ut.trace(3, f"Error listing workspaces")
```

### Comparing `wbx_workspaces-1.1.1/src/wbx_workspaces/wbx_utils.py` & `wbx_workspaces-1.3.1/src/wbx_workspaces/wbx_utils.py`

 * *Files identical despite different names*

### Comparing `wbx_workspaces-1.1.1/LICENSE` & `wbx_workspaces-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wbx_workspaces-1.1.1/README.md` & `wbx_workspaces-1.3.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ## Webex workspaces commands utilities 
 
 ## Usage:
-```
 Usage: python -m wbx_workspaces [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --version            Show the version and exit.
   -t, --token TEXT     Your access token. Read from AUTH_BEARER env variable
                        by default. You can find your personal token at
                        https://developer.webex.com/docs/getting-started.
   -d, --debug INTEGER  Debug level.
   --help               Show this message and exit.
 
 Commands:
-  locations   List locations IDs
-  metrics     Gather yesterday's hourly peopleCount or timeUsed metric...
-  workspaces  Get the list of workspaces in given location
+  device-status  Show device status.
+  devices        List devices in given location.
+  locations      List locations IDs.
+  metrics        Gather yesteray's hourly peopleCount or timeUsed metric...
+  workspaces     List workspaces in given location.
 ```
 
 # Examples:
 ```
-ython -m wbx_workspaces workspaces -l Y2lzY29zcGFyazovL3VzL0xPQ0FUSU9OLzhkZDI0ZWRmLWFjOWQtNDcxYi05MTIxLTJmM2EzYjk0YzRlYQ
-
+# get yesterday's peopleCount hourly metric for all workspaces under a location ID in a single JSON file
+python -m wbx_workspaces metrics -l <locationID> -a peopleCount 
 ```
 
-## Notes:
```

### Comparing `wbx_workspaces-1.1.1/pyproject.toml` & `wbx_workspaces-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wbx-workspaces"
-version = "1.1.1"
+version = "1.3.1"
 description = "Commands to download Webex Workspaces stats"
 readme = "README.md"
 authors = [{ name = "Stephane Cohen", email = "stecohen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `wbx_workspaces-1.1.1/PKG-INFO` & `wbx_workspaces-1.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wbx-workspaces
-Version: 1.1.1
+Version: 1.3.1
 Summary: Commands to download Webex Workspaces stats
 Author-email: Stephane Cohen <stecohen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephane Cohen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,31 +34,31 @@
 Requires-Dist: pandas==2.1.4
 Requires-Dist: requests==2.31.0
 Description-Content-Type: text/markdown
 
 ## Webex workspaces commands utilities 
 
 ## Usage:
-```
 Usage: python -m wbx_workspaces [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --version            Show the version and exit.
   -t, --token TEXT     Your access token. Read from AUTH_BEARER env variable
                        by default. You can find your personal token at
                        https://developer.webex.com/docs/getting-started.
   -d, --debug INTEGER  Debug level.
   --help               Show this message and exit.
 
 Commands:
-  locations   List locations IDs
-  metrics     Gather yesterday's hourly peopleCount or timeUsed metric...
-  workspaces  Get the list of workspaces in given location
+  device-status  Show device status.
+  devices        List devices in given location.
+  locations      List locations IDs.
+  metrics        Gather yesteray's hourly peopleCount or timeUsed metric...
+  workspaces     List workspaces in given location.
 ```
 
 # Examples:
 ```
-ython -m wbx_workspaces workspaces -l Y2lzY29zcGFyazovL3VzL0xPQ0FUSU9OLzhkZDI0ZWRmLWFjOWQtNDcxYi05MTIxLTJmM2EzYjk0YzRlYQ
-
+# get yesterday's peopleCount hourly metric for all workspaces under a location ID in a single JSON file
+python -m wbx_workspaces metrics -l <locationID> -a peopleCount 
 ```
 
-## Notes:
```

