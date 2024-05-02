# Comparing `tmp/itwingstestsprojectnn-0.2.tar.gz` & `tmp/itwingstestsprojectnn-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itwingstestsprojectnn-0.2.tar", last modified: Thu May  2 11:34:44 2024, max compression
+gzip compressed data, was "itwingstestsprojectnn-0.3.tar", last modified: Thu May  2 13:03:42 2024, max compression
```

## Comparing `itwingstestsprojectnn-0.2.tar` & `itwingstestsprojectnn-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 11:34:44.581987 itwingstestsprojectnn-0.2/
--rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.2/LICENSE
--rw-rw-rw-   0        0        0      393 2024-05-02 11:34:44.581987 itwingstestsprojectnn-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-02 11:00:34.000000 itwingstestsprojectnn-0.2/README.md
--rw-rw-rw-   0        0        0      103 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.2/pyproject.toml
--rw-rw-rw-   0        0        0      533 2024-05-02 11:34:44.603972 itwingstestsprojectnn-0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-02 11:34:44.419079 itwingstestsprojectnn-0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 11:34:44.578987 itwingstestsprojectnn-0.2/src/itwingstestsprojectnn.egg-info/
--rw-rw-rw-   0        0        0      393 2024-05-02 11:34:44.000000 itwingstestsprojectnn-0.2/src/itwingstestsprojectnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-05-02 11:34:44.000000 itwingstestsprojectnn-0.2/src/itwingstestsprojectnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 11:34:44.000000 itwingstestsprojectnn-0.2/src/itwingstestsprojectnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 11:34:44.000000 itwingstestsprojectnn-0.2/src/itwingstestsprojectnn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 11:34:44.564996 itwingstestsprojectnn-0.2/src/mymodule/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:46:40.000000 itwingstestsprojectnn-0.2/src/mymodule/__init__.py
--rw-rw-rw-   0        0        0     4347 2024-05-02 08:29:07.000000 itwingstestsprojectnn-0.2/src/mymodule/config.py
--rw-rw-rw-   0        0        0     3649 2024-05-02 11:33:59.000000 itwingstestsprojectnn-0.2/src/mymodule/main.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:03:42.943703 itwingstestsprojectnn-0.3/
+-rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.3/LICENSE
+-rw-rw-rw-   0        0        0      393 2024-05-02 13:03:42.943703 itwingstestsprojectnn-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-02 11:00:34.000000 itwingstestsprojectnn-0.3/README.md
+-rw-rw-rw-   0        0        0      103 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      533 2024-05-02 13:03:42.949709 itwingstestsprojectnn-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 13:03:42.885744 itwingstestsprojectnn-0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 13:03:42.942703 itwingstestsprojectnn-0.3/src/itwingstestsprojectnn.egg-info/
+-rw-rw-rw-   0        0        0      393 2024-05-02 13:03:42.000000 itwingstestsprojectnn-0.3/src/itwingstestsprojectnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-02 13:03:42.000000 itwingstestsprojectnn-0.3/src/itwingstestsprojectnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 13:03:42.000000 itwingstestsprojectnn-0.3/src/itwingstestsprojectnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 13:03:42.000000 itwingstestsprojectnn-0.3/src/itwingstestsprojectnn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 13:03:42.939705 itwingstestsprojectnn-0.3/src/mymodule/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:46:40.000000 itwingstestsprojectnn-0.3/src/mymodule/__init__.py
+-rw-rw-rw-   0        0        0     4347 2024-05-02 08:29:07.000000 itwingstestsprojectnn-0.3/src/mymodule/config.py
+-rw-rw-rw-   0        0        0     3775 2024-05-02 13:02:56.000000 itwingstestsprojectnn-0.3/src/mymodule/main.py
```

### Comparing `itwingstestsprojectnn-0.2/setup.cfg` & `itwingstestsprojectnn-0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 7477 696e 6773 7465 7374 7370   = itwingstestsp
 00000020: 726f 6a65 6374 6e6e 0d0a 7665 7273 696f  rojectnn..versio
-00000030: 6e20 3d20 302e 320d 0a61 7574 686f 7220  n = 0.2..author 
+00000030: 6e20 3d20 302e 330d 0a61 7574 686f 7220  n = 0.3..author 
 00000040: 3d20 4d61 7961 6e6b 0d0a 6175 7468 6f72  = Mayank..author
 00000050: 5f65 6d61 696c 203d 206d 6179 616e 6b74  _email = mayankt
 00000060: 696d 6261 6469 6140 676d 6169 6c2e 636f  imbadia@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2041 2073 6d61 6c6c 2065 7861 6d70 6c65   A small example
 00000090: 2070 6163 6b61 6765 0d0a 6c6f 6e67 5f64   package..long_d
 000000a0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `itwingstestsprojectnn-0.2/src/mymodule/config.py` & `itwingstestsprojectnn-0.3/src/mymodule/config.py`

 * *Files identical despite different names*

### Comparing `itwingstestsprojectnn-0.2/src/mymodule/main.py` & `itwingstestsprojectnn-0.3/src/mymodule/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,94 @@
 from google.oauth2 import service_account
 from datetime import datetime, timedelta
 from googleapiclient.discovery import build
-from gacs.config import *
+from mymodule.config import *
 
 # Define needed variables
 SCOPES = ['https://www.googleapis.com/auth/webmasters',
           'https://www.googleapis.com/auth/webmasters.readonly']
 
+
 def passed_or_failed(check_impressions, check_clicks, check_average_position):
     # Check Impressions
     if check_impressions < thresholds['Impressions']['Red']:
         return 'failed'
     # Check Clicks
     elif check_clicks < thresholds['Clicks']['Red']:
         return 'failed'
     # Check Average Position
     elif check_average_position > thresholds['Average Position']['Green']:
         return 'failed'
     else:
         return 'passed'
 
-def main(url, gsc, max_rows, credentials):
+
+def main(credentials, parameters):
     try:
-        if gsc == "yes":
-            try:
-                webmasters_service = initialize_service(credentials)
-                if webmasters_service is None:
-                    return None
-            except Exception as e:
-                print(f"Error initializing service: {e}")
+        try:
+            webmasters_service = initialize_service(credentials)
+            if webmasters_service is None:
                 return None
+        except Exception as e:
+            print(f"Error initializing service: {e}")
+            return None
+        start_date_str = start_date.strftime('%Y-%m-%d')
+        current_end_date_str = end_date.strftime('%Y-%m-%d')
+        start_row = 0
+        request = {
+            'startDate': parameters['start_date'],
+            'endDate': parameters['end_date'],
+            # Assign dimensions from parameters
+            'dimensions': parameters['dimensions'],
+            'rowLimit': parameters['max_rows'],
+            'startRow': start_row
+        }
+        response = webmasters_service.searchanalytics().query(
+            siteUrl=parameters['url'], body=request).execute()
 
-            start_date_str = start_date.strftime('%Y-%m-%d')
-            current_end_date_str = end_date.strftime('%Y-%m-%d')
-            start_row = 0
-            request = {
-                'startDate': start_date_str,
-                'endDate': current_end_date_str,
-                'dimensions': [],
-                'rowLimit': max_rows,
-                'startRow': start_row
+        if 'rows' in response and response['rows'] and all(key in response['rows'][0] for key in ['impressions', 'clicks', 'position']):
+            data = {
+                'url': parameters['url'],
+                'GSC Impressions': response['rows'][0]['impressions'],
+                'GSC Clicks': response['rows'][0]['clicks'],
+                'GSC CTR': "{:.2%}".format(response['rows'][0]['clicks'] / response['rows'][0]['impressions']),
+                'GSC Average Position': round(response['rows'][0]['position']),
+                'Phase 2': passed_or_failed(response['rows'][0]['impressions'], response['rows'][0]['clicks'], round(response['rows'][0]['position']))
             }
-            response = webmasters_service.searchanalytics().query(siteUrl=url, body=request).execute()
-            if 'rows' in response and response['rows'] and all(key in response['rows'][0] for key in ['impressions', 'clicks', 'position']):
-                data = {
-                    'url': url,
-                    'GSC Impressions': response['rows'][0]['impressions'],
-                    'GSC Clicks': response['rows'][0]['clicks'],
-                    'GSC CTR': "{:.2%}".format(response['rows'][0]['clicks'] / response['rows'][0]['impressions']),
-                    'GSC Average Position': round(response['rows'][0]['position']),
-                    'Phase 2': passed_or_failed(response['rows'][0]['impressions'], response['rows'][0]['clicks'], round(response['rows'][0]['position']))
-                }
-                print("Result of adding:", data)
-                return data
-            else:
-                data = {
-                    'url': url,
-                    'GSC Impressions': "-",
-                    'GSC Clicks': "-",
-                    'GSC CTR': "-",
-                    'GSC Average Position': "-",
-                    'Phase 2': "no access"
-                }
-                return data
+            # Add dimensions dynamically to the data dictionary
+            for dim in parameters.get('dimensions', []):
+                data[f'GSC {dim.capitalize()}'] = response['rows'][0]['keys'][parameters['dimensions'].index(
+                    dim)]
+            print("Result of data:", data)
+
+            return data
         else:
             data = {
-                'url': url,
+                'url': parameters['url'],
                 'GSC Impressions': "-",
                 'GSC Clicks': "-",
                 'GSC CTR': "-",
                 'GSC Average Position': "-",
                 'Phase 2': "no access"
             }
+            # Add dimensions dynamically to the data dictionary
+            for dim in parameters.get('dimensions', []):
+                data[f'GSC {dim.capitalize()}'] = "-"
             return data
     except Exception as e:
         print(f"Error: {e}")
         data = {
-            'url': url,
+            'url': parameters['url'],
             'GSC Impressions': "-",
             'GSC Clicks': "-",
             'GSC CTR': "-",
             'GSC Average Position': "-",
             'Phase 2': "no access"
         }
         return data
-        
+
+
 def initialize_service(gsc_credentials):
-    credentials = service_account.Credentials.from_service_account_info(gsc_credentials, scopes=SCOPES)
+    credentials = service_account.Credentials.from_service_account_info(
+        gsc_credentials, scopes=SCOPES)
     service = build('webmasters', 'v3', credentials=credentials)
     return service
```

