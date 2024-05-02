# Comparing `tmp/medicafe-0.240501.2.tar.gz` & `tmp/medicafe-0.240501.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240501.2.tar", last modified: Thu May  2 00:15:12 2024, max compression
+gzip compressed data, was "medicafe-0.240501.3.tar", last modified: Thu May  2 02:18:41 2024, max compression
```

## Comparing `medicafe-0.240501.2.tar` & `medicafe-0.240501.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 00:15:12.186000 medicafe-0.240501.2/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240501.2/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240501.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-02 00:15:11.550000 medicafe-0.240501.2/MediBot/
--rwxrwxrwx   0        0        0     2712 2024-05-02 00:07:18.000000 medicafe-0.240501.2/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    16168 2024-05-01 03:57:12.000000 medicafe-0.240501.2/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240501.2/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    27949 2024-05-02 00:02:26.000000 medicafe-0.240501.2/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4940 2024-05-01 15:57:54.000000 medicafe-0.240501.2/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240501.2/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240501.2/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240501.2/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240501.2/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240501.2/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240501.2/MediBot/update_json.py
--rw-rw-rw-   0        0        0      801 2024-04-20 02:05:15.000000 medicafe-0.240501.2/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-02 00:15:11.993000 medicafe-0.240501.2/MediLink/
--rw-rw-rw-   0        0        0    17570 2024-05-02 00:11:11.000000 medicafe-0.240501.2/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240501.2/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240501.2/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    33088 2024-05-01 04:35:27.000000 medicafe-0.240501.2/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3791 2024-05-01 23:56:13.000000 medicafe-0.240501.2/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    10677 2024-05-01 03:49:34.000000 medicafe-0.240501.2/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7123 2024-05-01 03:44:49.000000 medicafe-0.240501.2/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240501.2/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6313 2024-05-01 03:44:48.000000 medicafe-0.240501.2/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240501.2/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240501.2/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4950 2024-04-30 21:38:34.000000 medicafe-0.240501.2/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     6051 2024-05-01 03:44:47.000000 medicafe-0.240501.2/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240501.2/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240501.2/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240501.2/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-02 00:15:12.170000 medicafe-0.240501.2/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240501.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 00:15:12.149000 medicafe-0.240501.2/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-02 00:15:10.000000 medicafe-0.240501.2/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-02 00:15:11.000000 medicafe-0.240501.2/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 00:15:10.000000 medicafe-0.240501.2/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240501.2/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-02 00:15:10.000000 medicafe-0.240501.2/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-02 00:15:10.000000 medicafe-0.240501.2/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 00:15:12.183000 medicafe-0.240501.2/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-02 00:15:09.000000 medicafe-0.240501.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:18:41.310000 medicafe-0.240501.3/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240501.3/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240501.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-02 02:18:40.326000 medicafe-0.240501.3/MediBot/
+-rwxrwxrwx   0        0        0     2712 2024-05-02 00:07:18.000000 medicafe-0.240501.3/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    16168 2024-05-01 03:57:12.000000 medicafe-0.240501.3/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240501.3/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    29432 2024-05-02 02:13:29.000000 medicafe-0.240501.3/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240501.3/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240501.3/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240501.3/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240501.3/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240501.3/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240501.3/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240501.3/MediBot/update_json.py
+-rw-rw-rw-   0        0        0      801 2024-04-20 02:05:15.000000 medicafe-0.240501.3/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:18:40.964000 medicafe-0.240501.3/MediLink/
+-rw-rw-rw-   0        0        0    17570 2024-05-02 00:11:11.000000 medicafe-0.240501.3/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240501.3/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240501.3/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    33088 2024-05-01 04:35:27.000000 medicafe-0.240501.3/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3791 2024-05-01 23:56:13.000000 medicafe-0.240501.3/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    10677 2024-05-01 03:49:34.000000 medicafe-0.240501.3/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7123 2024-05-01 03:44:49.000000 medicafe-0.240501.3/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240501.3/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6313 2024-05-01 03:44:48.000000 medicafe-0.240501.3/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240501.3/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240501.3/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4950 2024-04-30 21:38:34.000000 medicafe-0.240501.3/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     6051 2024-05-01 03:44:47.000000 medicafe-0.240501.3/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240501.3/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240501.3/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240501.3/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-02 02:18:41.283000 medicafe-0.240501.3/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240501.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 02:18:41.256000 medicafe-0.240501.3/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-02 02:18:39.000000 medicafe-0.240501.3/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-02 02:18:39.000000 medicafe-0.240501.3/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 02:18:39.000000 medicafe-0.240501.3/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240501.3/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-02 02:18:39.000000 medicafe-0.240501.3/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-02 02:18:39.000000 medicafe-0.240501.3/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 02:18:41.303000 medicafe-0.240501.3/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-02 02:18:36.000000 medicafe-0.240501.3/setup.py
```

### Comparing `medicafe-0.240501.2/LICENSE` & `medicafe-0.240501.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediBot/MediBot.bat` & `medicafe-0.240501.3/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediBot/MediBot.py` & `medicafe-0.240501.3/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediBot/MediBot_Charges.py` & `medicafe-0.240501.3/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240501.3/MediBot/MediBot_Preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -209,17 +209,33 @@
         for filename in os.listdir(directory_path):
             file_path = os.path.join(directory_path, filename)
             if filename.endswith('.csv'):
                 try:
                     with open(file_path, 'r', encoding='utf-8') as csvfile:
                         reader = csv.DictReader(csvfile)
                         found_data = False  # Flag to track if any valid data is found in the CSV
+                        found_patient_id = False
+                        found_payer_id = False
                         for row in reader:
-                            if 'Patient ID' not in row or 'Ins1 Payer ID' not in row:
-                                raise ValueError("CSV file '{}' is misformatted.".format(filename))
+                            if 'Patient ID' not in row:
+                                found_patient_id = False
+                            else:
+                                found_patient_id = True
+                            if 'Ins1 Payer ID' not in row:
+                                found_payer_id = False
+                            else:
+                                found_payer_id = True
+
+                            if not found_patient_id and not found_payer_id:
+                                raise ValueError("CSV file '{}' is misformatted or empty.".format(filename))
+                            elif not found_patient_id:
+                                raise ValueError("CSV file '{}' is misformatted: Missing 'Patient ID' column.".format(filename))
+                            elif not found_payer_id:
+                                raise ValueError("CSV file '{}' is misformatted: Missing 'Ins1 Payer ID' column.".format(filename))
+
                             if row['Patient ID'].strip() and row['Ins1 Payer ID'].strip():
                                 found_data = True
                                 payer_id = row['Ins1 Payer ID'].strip()
                                 patient_id = row['Patient ID'].strip()
                                 payer_to_patient_ids[payer_id].add(patient_id)
                         if not found_data:
                             raise ValueError("CSV file '{}' is empty.".format(filename))
@@ -244,18 +260,28 @@
 
     Output: A fully populated crosswalk.json file that serves as a baseline for future updates.
     """
     payer_id_to_details = {}
     
     # Load historical Patient ID to Insurance ID mappings from MAPAT
     patient_id_to_insurance_id = load_insurance_data_from_mapat(config, crosswalk)
-    
+
+    # Check if patient_id_to_insurance_id is empty
+    if not patient_id_to_insurance_id:
+        print("Error: Failed to load historical Patient ID to Insurance ID mappings from MAPAT.")
+        sys.exit(1)
+
     # Process historical Carol's CSVs
     payer_id_to_patient_ids = load_historical_payer_to_patient_mappings(config)
     
+    # Check if payer_id_to_patient_ids is empty
+    if not payer_id_to_patient_ids:
+        print("Error: Failed to load historical Carol's CSVs.")
+        sys.exit(1)
+
     # Map Payer IDs to Insurance IDs
     for payer_id, patient_ids in payer_id_to_patient_ids.items():
         medisoft_ids = set()
         for patient_id in patient_ids:
             if patient_id in patient_id_to_insurance_id:
                 medisoft_id = patient_id_to_insurance_id[patient_id]
                 medisoft_ids.add(medisoft_id)
@@ -313,27 +339,28 @@
             "345678": {
                 "endpoint": "OPTUMEDI",
                 "medisoft_id": ["004", "005", "006"]
             }
         },
         "mapat_mapping": {
             "slices": {
-                "MAPATPXID": "slice definition",
-                "MAPATINID": "slice definition"
+                "MAPATPXID": [195,200],
+                "MAPATINID": [159,161],
+                "MAPATINID2":[163,166]
             }
         },
         "mains_mapping": {
             "slices": {
-                "MAINSNAME": "slice definition"
+                "MAINSNAME": [0,30],
+                "MAINSADDR": [31,60]
             }
         }
     }
 
-    """
-
+    """    
     # Load insurance mappings from MAINS (Insurance Name to Insurance ID)
     insurance_name_to_id = load_insurance_data_from_mains(config)
     MediLink_ConfigLoader.log("Loaded insurance data from MAINS...")
     
     # Load new Patient ID to Payer ID mappings from Carol's CSV (This is really just a performance increment)
     # patient_id_to_payer_id = load_patient_to_payer_mappings(config)
     
@@ -350,15 +377,18 @@
     # Update the crosswalk with new or revised mappings
     for patient_id, payer_id in patient_id_to_payer_id.items():
         insurance_name = patient_id_to_insurance_name.get(patient_id)
         if insurance_name and insurance_name in insurance_name_to_id:
             insurance_id = insurance_name_to_id[insurance_name]
 
             # Ensure payer ID is in the crosswalk and initialize if not
+            MediLink_ConfigLoader.log("Initializing payer_id key...")
             # BUG OPTUMEDI hardcode should be gathered via API
+            if 'payer_id' not in crosswalk:
+                crosswalk['payer_id'] = {}
             if payer_id not in crosswalk['payer_id']:
                 crosswalk['payer_id'][payer_id] = {'endpoint': 'OPTUMEDI', 'medisoft_id': set()}
 
             # Update the medisoft_id set, temporarily using a set to avoid duplicates
             crosswalk['payer_id'][payer_id]['medisoft_id'].add(insurance_id)
             MediLink_ConfigLoader.log("Added new insurance ID {} to payer ID {}".format(insurance_id, payer_id))
```

### Comparing `medicafe-0.240501.2/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240501.3/MediBot/MediBot_Preprocessor_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,28 +38,26 @@
     Args:
         crosswalk_path (str): Path to the crosswalk.json file.
         crosswalk (dict): The updated crosswalk data.
     Returns:
         bool: True if the file was successfully saved, False otherwise.
     """
     try:
-        # Check if 'payer_id' key already exists
+        # Initialize 'payer_id' key if not present
         if 'payer_id' not in crosswalk:
-            crosswalk['payer_id'] = {}  # Initialize 'payer_id' key if not present
+            print("save_crosswalk is initializing 'payer_id' key...")
+            crosswalk['payer_id'] = {}
 
         # Convert all 'medisoft_id' fields from sets to lists if necessary
-        formatted_crosswalk = {
-            k: {
-                'endpoint': v['endpoint'],
-                'medisoft_id': list(v['medisoft_id']) if isinstance(v['medisoft_id'], set) else v['medisoft_id']
-            } for k, v in crosswalk['payer_id'].items()
-        }
+        for k, v in crosswalk.get('payer_id', {}).items():
+            if isinstance(v.get('medisoft_id'), set):
+                v['medisoft_id'] = list(v['medisoft_id'])
 
         with open(crosswalk_path, 'w') as file:
-            json.dump({'payer_id': formatted_crosswalk}, file, indent=4)
+            json.dump(crosswalk, file, indent=4)  # Save the entire dictionary
         return True
 
     except KeyError as e:
         # Log the KeyError with specific information about what was missing
         print("Key Error: A required key is missing in the crosswalk data -", e)
         return False
 
@@ -69,19 +67,14 @@
         return False
 
     except IOError as e:
         # Handle I/O errors related to file operations
         print("I/O Error: An error occurred while writing to the crosswalk file -", e)
         return False
 
-    except json.JSONDecodeError as e:
-        # Handle errors specifically related to JSON decoding
-        print("JSON Decode Error: An error occurred while decoding the crosswalk data -", e)
-        return False
-
     except Exception as e:
         # A general exception catch to log any other exceptions that may not have been anticipated
         print("Unexpected crosswalk error:", e)
         return False
 
 
 def open_csv_for_editing(csv_file_path):
```

### Comparing `medicafe-0.240501.2/MediBot/MediBot_UI.py` & `medicafe-0.240501.3/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240501.3/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240501.3/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediBot/update_json.py` & `medicafe-0.240501.3/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediBot/update_medicafe.py` & `medicafe-0.240501.3/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink.py` & `medicafe-0.240501.3/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_277_decoder.py` & `medicafe-0.240501.3/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240501.3/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240501.3/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240501.3/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240501.3/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_Down.py` & `medicafe-0.240501.3/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240501.3/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_Gmail.py` & `medicafe-0.240501.3/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_Scheduler.py` & `medicafe-0.240501.3/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_UI.py` & `medicafe-0.240501.3/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/MediLink/MediLink_Up.py` & `medicafe-0.240501.3/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/PKG-INFO` & `medicafe-0.240501.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240501.2
+Version: 0.240501.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240501.2/README.md` & `medicafe-0.240501.3/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/medicafe.egg-info/PKG-INFO` & `medicafe-0.240501.3/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240501.2
+Version: 0.240501.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240501.2/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240501.3/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.2/setup.py` & `medicafe-0.240501.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240501.2",
+    version="0.240501.3",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

