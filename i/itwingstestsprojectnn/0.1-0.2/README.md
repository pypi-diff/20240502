# Comparing `tmp/itwingstestsprojectnn-0.1.tar.gz` & `tmp/itwingstestsprojectnn-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itwingstestsprojectnn-0.1.tar", last modified: Thu May  2 10:32:52 2024, max compression
+gzip compressed data, was "itwingstestsprojectnn-0.2.tar", last modified: Thu May  2 11:34:44 2024, max compression
```

## Comparing `itwingstestsprojectnn-0.1.tar` & `itwingstestsprojectnn-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 10:32:52.801042 itwingstestsprojectnn-0.1/
--rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.1/LICENSE
--rw-rw-rw-   0        0        0     2811 2024-05-02 10:32:52.801042 itwingstestsprojectnn-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.1/README.md
--rw-rw-rw-   0        0        0      103 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.1/pyproject.toml
--rw-rw-rw-   0        0        0      533 2024-05-02 10:32:52.808037 itwingstestsprojectnn-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-02 10:32:52.613149 itwingstestsprojectnn-0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 10:32:52.633137 itwingstestsprojectnn-0.1/src/gac/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:46:40.000000 itwingstestsprojectnn-0.1/src/gac/__init__.py
--rw-rw-rw-   0        0        0     4347 2024-05-02 08:29:07.000000 itwingstestsprojectnn-0.1/src/gac/config.py
--rw-rw-rw-   0        0        0     4169 2024-05-02 10:29:07.000000 itwingstestsprojectnn-0.1/src/gac/main.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:32:52.799043 itwingstestsprojectnn-0.1/src/itwingstestsprojectnn.egg-info/
--rw-rw-rw-   0        0        0     2811 2024-05-02 10:32:52.000000 itwingstestsprojectnn-0.1/src/itwingstestsprojectnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-02 10:32:52.000000 itwingstestsprojectnn-0.1/src/itwingstestsprojectnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 10:32:52.000000 itwingstestsprojectnn-0.1/src/itwingstestsprojectnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-02 10:32:52.000000 itwingstestsprojectnn-0.1/src/itwingstestsprojectnn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 11:34:44.581987 itwingstestsprojectnn-0.2/
+-rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.2/LICENSE
+-rw-rw-rw-   0        0        0      393 2024-05-02 11:34:44.581987 itwingstestsprojectnn-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-02 11:00:34.000000 itwingstestsprojectnn-0.2/README.md
+-rw-rw-rw-   0        0        0      103 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      533 2024-05-02 11:34:44.603972 itwingstestsprojectnn-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 11:34:44.419079 itwingstestsprojectnn-0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 11:34:44.578987 itwingstestsprojectnn-0.2/src/itwingstestsprojectnn.egg-info/
+-rw-rw-rw-   0        0        0      393 2024-05-02 11:34:44.000000 itwingstestsprojectnn-0.2/src/itwingstestsprojectnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-02 11:34:44.000000 itwingstestsprojectnn-0.2/src/itwingstestsprojectnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 11:34:44.000000 itwingstestsprojectnn-0.2/src/itwingstestsprojectnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 11:34:44.000000 itwingstestsprojectnn-0.2/src/itwingstestsprojectnn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 11:34:44.564996 itwingstestsprojectnn-0.2/src/mymodule/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:46:40.000000 itwingstestsprojectnn-0.2/src/mymodule/__init__.py
+-rw-rw-rw-   0        0        0     4347 2024-05-02 08:29:07.000000 itwingstestsprojectnn-0.2/src/mymodule/config.py
+-rw-rw-rw-   0        0        0     3649 2024-05-02 11:33:59.000000 itwingstestsprojectnn-0.2/src/mymodule/main.py
```

### Comparing `itwingstestsprojectnn-0.1/setup.cfg` & `itwingstestsprojectnn-0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 7477 696e 6773 7465 7374 7370   = itwingstestsp
 00000020: 726f 6a65 6374 6e6e 0d0a 7665 7273 696f  rojectnn..versio
-00000030: 6e20 3d20 302e 310d 0a61 7574 686f 7220  n = 0.1..author 
+00000030: 6e20 3d20 302e 320d 0a61 7574 686f 7220  n = 0.2..author 
 00000040: 3d20 4d61 7961 6e6b 0d0a 6175 7468 6f72  = Mayank..author
 00000050: 5f65 6d61 696c 203d 206d 6179 616e 6b74  _email = mayankt
 00000060: 696d 6261 6469 6140 676d 6169 6c2e 636f  imbadia@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2041 2073 6d61 6c6c 2065 7861 6d70 6c65   A small example
 00000090: 2070 6163 6b61 6765 0d0a 6c6f 6e67 5f64   package..long_d
 000000a0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `itwingstestsprojectnn-0.1/src/gac/config.py` & `itwingstestsprojectnn-0.2/src/mymodule/config.py`

 * *Files identical despite different names*

### Comparing `itwingstestsprojectnn-0.1/src/gac/main.py` & `itwingstestsprojectnn-0.2/src/mymodule/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,101 +1,91 @@
 from google.oauth2 import service_account
 from datetime import datetime, timedelta
 from googleapiclient.discovery import build
-from config import *
-
-# define needed variables
+from gacs.config import *
 
+# Define needed variables
 SCOPES = ['https://www.googleapis.com/auth/webmasters',
           'https://www.googleapis.com/auth/webmasters.readonly']
 
-class MyModule:
-    @staticmethod
-    # Function to determine passed or failed based on thresholds
-    def passed_or_failed(check_impressions, check_clicks, check_average_position):
-        # Check Impressions
-        if check_impressions < thresholds['Impressions']['Red']:
-            return 'failed'
-        # Check Clicks
-        elif check_clicks < thresholds['Clicks']['Red']:
-            return 'failed'
-        # Check Average Position
-        elif check_average_position > thresholds['Average Position']['Green']:
-            return 'failed'
-        else:
-            return 'passed'
+def passed_or_failed(check_impressions, check_clicks, check_average_position):
+    # Check Impressions
+    if check_impressions < thresholds['Impressions']['Red']:
+        return 'failed'
+    # Check Clicks
+    elif check_clicks < thresholds['Clicks']['Red']:
+        return 'failed'
+    # Check Average Position
+    elif check_average_position > thresholds['Average Position']['Green']:
+        return 'failed'
+    else:
+        return 'passed'
 
-    
-    @staticmethod
-    def test(url, gsc, max_rows, credentials):
-        try:
-            if gsc == "yes":
-                try:
-                    webmasters_service = initialize_service(credentials)
-                    if webmasters_service is None:
-                        return None
-                except Exception as e:
-                    print(f"Error initializing service: {e}")
+def main(url, gsc, max_rows, credentials):
+    try:
+        if gsc == "yes":
+            try:
+                webmasters_service = initialize_service(credentials)
+                if webmasters_service is None:
                     return None
+            except Exception as e:
+                print(f"Error initializing service: {e}")
+                return None
 
-                start_date_str = start_date.strftime('%Y-%m-%d')
-                current_end_date_str = end_date.strftime('%Y-%m-%d')
-                start_row = 0
-                request = {
-                    'startDate': start_date_str,
-                    'endDate': current_end_date_str,
-                    'dimensions': [],
-                    'rowLimit': max_rows,
-                    'startRow': start_row
+            start_date_str = start_date.strftime('%Y-%m-%d')
+            current_end_date_str = end_date.strftime('%Y-%m-%d')
+            start_row = 0
+            request = {
+                'startDate': start_date_str,
+                'endDate': current_end_date_str,
+                'dimensions': [],
+                'rowLimit': max_rows,
+                'startRow': start_row
+            }
+            response = webmasters_service.searchanalytics().query(siteUrl=url, body=request).execute()
+            if 'rows' in response and response['rows'] and all(key in response['rows'][0] for key in ['impressions', 'clicks', 'position']):
+                data = {
+                    'url': url,
+                    'GSC Impressions': response['rows'][0]['impressions'],
+                    'GSC Clicks': response['rows'][0]['clicks'],
+                    'GSC CTR': "{:.2%}".format(response['rows'][0]['clicks'] / response['rows'][0]['impressions']),
+                    'GSC Average Position': round(response['rows'][0]['position']),
+                    'Phase 2': passed_or_failed(response['rows'][0]['impressions'], response['rows'][0]['clicks'], round(response['rows'][0]['position']))
                 }
-                response = webmasters_service.searchanalytics().query(
-                    siteUrl=url, body=request).execute()
-                if 'rows' in response and response['rows'] and all(key in response['rows'][0] for key in ['impressions', 'clicks', 'position']):
-                    data = {
-                        'url': url,
-                        'GSC Impressions': response['rows'][0]['impressions'],
-                        'GSC Clicks': response['rows'][0]['clicks'],
-                        'GSC CTR': "{:.2%}".format(response['rows'][0]['clicks'] / response['rows'][0]['impressions']),
-                        'GSC Average Position': round(response['rows'][0]['position']),
-                        'Phase 2': passed_or_failed(response['rows'][0]['impressions'], response['rows'][0]['clicks'], round(response['rows'][0]['position']))
-                    }
-                    print("Result of adding:", data)
-                    return data
-                else:
-                    data = {
-                        'url': url,
-                        'GSC Impressions': "-",
-                        'GSC Clicks': "-",
-                        'GSC CTR': "-",
-                        'GSC Average Position': "-",
-                        'Phase 2': "no access"
-                    }
-                    return data
+                print("Result of adding:", data)
+                return data
             else:
                 data = {
                     'url': url,
                     'GSC Impressions': "-",
                     'GSC Clicks': "-",
                     'GSC CTR': "-",
                     'GSC Average Position': "-",
                     'Phase 2': "no access"
                 }
                 return data
-        
-        except Exception as e:
-            print(f"Error: {e}")
+        else:
             data = {
                 'url': url,
                 'GSC Impressions': "-",
                 'GSC Clicks': "-",
                 'GSC CTR': "-",
                 'GSC Average Position': "-",
                 'Phase 2': "no access"
             }
             return data
+    except Exception as e:
+        print(f"Error: {e}")
+        data = {
+            'url': url,
+            'GSC Impressions': "-",
+            'GSC Clicks': "-",
+            'GSC CTR': "-",
+            'GSC Average Position': "-",
+            'Phase 2': "no access"
+        }
+        return data
         
-    @staticmethod               
-    def initialize_service(gsc_credentials):
-        credentials = service_account.Credentials.from_service_account_info(
-            gsc_credentials, scopes=SCOPES)
-        service = build('webmasters', 'v3', credentials=credentials)
-        return service
+def initialize_service(gsc_credentials):
+    credentials = service_account.Credentials.from_service_account_info(gsc_credentials, scopes=SCOPES)
+    service = build('webmasters', 'v3', credentials=credentials)
+    return service
```

