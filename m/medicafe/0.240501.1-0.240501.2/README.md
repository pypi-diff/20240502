# Comparing `tmp/medicafe-0.240501.1.tar.gz` & `tmp/medicafe-0.240501.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240501.1.tar", last modified: Wed May  1 16:13:20 2024, max compression
+gzip compressed data, was "medicafe-0.240501.2.tar", last modified: Thu May  2 00:15:12 2024, max compression
```

## Comparing `medicafe-0.240501.1.tar` & `medicafe-0.240501.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 16:13:20.362000 medicafe-0.240501.1/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240501.1/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240501.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-01 16:13:19.696000 medicafe-0.240501.1/MediBot/
--rwxrwxrwx   0        0        0     2108 2024-04-19 21:07:40.000000 medicafe-0.240501.1/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    16168 2024-05-01 03:57:12.000000 medicafe-0.240501.1/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240501.1/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    27674 2024-05-01 15:59:41.000000 medicafe-0.240501.1/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4940 2024-05-01 15:57:54.000000 medicafe-0.240501.1/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240501.1/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240501.1/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240501.1/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240501.1/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240501.1/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240501.1/MediBot/update_json.py
--rw-rw-rw-   0        0        0      801 2024-04-20 02:05:15.000000 medicafe-0.240501.1/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-01 16:13:20.093000 medicafe-0.240501.1/MediLink/
--rw-rw-rw-   0        0        0    17255 2024-05-01 16:07:23.000000 medicafe-0.240501.1/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240501.1/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240501.1/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    33088 2024-05-01 04:35:27.000000 medicafe-0.240501.1/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3399 2024-05-01 03:49:31.000000 medicafe-0.240501.1/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    10677 2024-05-01 03:49:34.000000 medicafe-0.240501.1/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7123 2024-05-01 03:44:49.000000 medicafe-0.240501.1/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240501.1/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6313 2024-05-01 03:44:48.000000 medicafe-0.240501.1/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240501.1/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240501.1/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4950 2024-04-30 21:38:34.000000 medicafe-0.240501.1/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     6051 2024-05-01 03:44:47.000000 medicafe-0.240501.1/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240501.1/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240501.1/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240501.1/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-01 16:13:20.309000 medicafe-0.240501.1/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240501.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 16:13:20.254000 medicafe-0.240501.1/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-01 16:13:19.000000 medicafe-0.240501.1/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-01 16:13:19.000000 medicafe-0.240501.1/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 16:13:19.000000 medicafe-0.240501.1/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240501.1/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-01 16:13:19.000000 medicafe-0.240501.1/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-01 16:13:19.000000 medicafe-0.240501.1/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 16:13:20.359000 medicafe-0.240501.1/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-01 16:12:16.000000 medicafe-0.240501.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:15:12.186000 medicafe-0.240501.2/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240501.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240501.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-02 00:15:11.550000 medicafe-0.240501.2/MediBot/
+-rwxrwxrwx   0        0        0     2712 2024-05-02 00:07:18.000000 medicafe-0.240501.2/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    16168 2024-05-01 03:57:12.000000 medicafe-0.240501.2/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240501.2/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    27949 2024-05-02 00:02:26.000000 medicafe-0.240501.2/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4940 2024-05-01 15:57:54.000000 medicafe-0.240501.2/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240501.2/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240501.2/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240501.2/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240501.2/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240501.2/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240501.2/MediBot/update_json.py
+-rw-rw-rw-   0        0        0      801 2024-04-20 02:05:15.000000 medicafe-0.240501.2/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-02 00:15:11.993000 medicafe-0.240501.2/MediLink/
+-rw-rw-rw-   0        0        0    17570 2024-05-02 00:11:11.000000 medicafe-0.240501.2/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240501.2/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240501.2/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    33088 2024-05-01 04:35:27.000000 medicafe-0.240501.2/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3791 2024-05-01 23:56:13.000000 medicafe-0.240501.2/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    10677 2024-05-01 03:49:34.000000 medicafe-0.240501.2/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7123 2024-05-01 03:44:49.000000 medicafe-0.240501.2/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240501.2/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6313 2024-05-01 03:44:48.000000 medicafe-0.240501.2/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240501.2/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240501.2/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4950 2024-04-30 21:38:34.000000 medicafe-0.240501.2/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     6051 2024-05-01 03:44:47.000000 medicafe-0.240501.2/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240501.2/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240501.2/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240501.2/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-02 00:15:12.170000 medicafe-0.240501.2/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240501.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 00:15:12.149000 medicafe-0.240501.2/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-02 00:15:10.000000 medicafe-0.240501.2/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-02 00:15:11.000000 medicafe-0.240501.2/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 00:15:10.000000 medicafe-0.240501.2/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240501.2/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-02 00:15:10.000000 medicafe-0.240501.2/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-02 00:15:10.000000 medicafe-0.240501.2/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 00:15:12.183000 medicafe-0.240501.2/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-02 00:15:09.000000 medicafe-0.240501.2/setup.py
```

### Comparing `medicafe-0.240501.1/LICENSE` & `medicafe-0.240501.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediBot/MediBot.py` & `medicafe-0.240501.2/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediBot/MediBot_Charges.py` & `medicafe-0.240501.2/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240501.2/MediBot/MediBot_Preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,21 +208,25 @@
         # Loop through each file in the directory containing Carol's historical CSVs
         for filename in os.listdir(directory_path):
             file_path = os.path.join(directory_path, filename)
             if filename.endswith('.csv'):
                 try:
                     with open(file_path, 'r', encoding='utf-8') as csvfile:
                         reader = csv.DictReader(csvfile)
+                        found_data = False  # Flag to track if any valid data is found in the CSV
                         for row in reader:
                             if 'Patient ID' not in row or 'Ins1 Payer ID' not in row:
-                                raise ValueError("CSV file '{}' is misformatted or empty.".format(filename))
+                                raise ValueError("CSV file '{}' is misformatted.".format(filename))
                             if row['Patient ID'].strip() and row['Ins1 Payer ID'].strip():
+                                found_data = True
                                 payer_id = row['Ins1 Payer ID'].strip()
                                 patient_id = row['Patient ID'].strip()
                                 payer_to_patient_ids[payer_id].add(patient_id)
+                        if not found_data:
+                            raise ValueError("CSV file '{}' is empty.".format(filename))
                 except Exception as e:
                     print("Error processing file {}: {}".format(filename, e))
     except FileNotFoundError as e:
         print("Error: {}".format(e))
 
     if not payer_to_patient_ids:
         print("No historical mappings were generated.")
```

### Comparing `medicafe-0.240501.1/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240501.2/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediBot/MediBot_UI.py` & `medicafe-0.240501.2/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240501.2/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240501.2/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediBot/update_json.py` & `medicafe-0.240501.2/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediBot/update_medicafe.py` & `medicafe-0.240501.2/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediLink/MediLink.py` & `medicafe-0.240501.2/MediLink/MediLink.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,18 @@
     """
     Initializes the main menu loop and handles the overall program flow,
     including loading configurations and managing user input for menu selections.
     """
     # Load configuration settings and display the initial welcome message.
     config, crosswalk = MediLink_ConfigLoader.load_configuration() # BUG does this need an argument?
     
+    # TODO Add here a check in config.json for key "MediLink_Config": { "TestMode": true, ...}. If it is true,
+    # prompt the user to say that MediLink is in Test Mode and ask if the user wants to stay in test mode? 
+    # Then put placeholder text for now because I don't know what the logic should be.
+    
     # Display Welcome Message
     MediLink_UI.display_welcome()
 
     # Normalize the directory path for file operations.
     directory_path = os.path.normpath(config['MediLink_Config']['inputFilePath'])
 
     # Detect new files and collect detailed patient data if available.
```

### Comparing `medicafe-0.240501.1/MediLink/MediLink_277_decoder.py` & `medicafe-0.240501.2/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240501.2/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240501.2/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240501.2/MediLink/MediLink_ConfigLoader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 import os
 import json
 import logging
 from datetime import datetime
 from collections import OrderedDict
 import sys
+import platform
 
 """
 This function should be generalizable to have a initialization script over all the Medi* functions
 """
 
 def load_configuration(config_path=os.path.join(os.path.dirname(__file__), '..', 'json', 'config.json'), crosswalk_path=os.path.join(os.path.dirname(__file__), '..', 'json', 'crosswalk.json')):
     """
     Loads endpoint configuration, credentials, and other settings from JSON files.
         
     Returns: A tuple containing dictionaries with configuration settings for the main config and crosswalk.
     """
-    # BUG HARDCODE FOR NOW
-    config_path="G:\\My Drive\\Codes\\MediCafe\\json\\config.json"
-    # "F:\\Medibot\\json\\config.json"
-    crosswalk_path="G:\\My Drive\\Codes\\MediCafe\\json\\crosswalk.json"
-    # "F:\\Medibot\\json\\crosswalk.json"
+    # BUG HARDCODE FOR NOW:
+    # Detect the operating system
+    if platform.system() == 'Windows' and platform.release() == 'XP':
+        # Use F: paths for Windows XP
+        config_path = "F:\\Medibot\\json\\config.json"
+        crosswalk_path = "F:\\Medibot\\json\\crosswalk.json"
+    else:
+        # Use G: paths for other versions of Windows
+        config_path = "G:\\My Drive\\Codes\\MediCafe\\json\\config.json"
+        crosswalk_path = "G:\\My Drive\\Codes\\MediCafe\\json\\crosswalk.json"
     
     try:
         with open(config_path, 'r') as config_file:
             config = json.load(config_file, object_pairs_hook=OrderedDict)
             if 'MediLink_Config' not in config:
                 raise KeyError("MediLink_Config key is missing from the loaded configuration.")
             # MediLink_config = config['MediLink_Config']
 
         with open(crosswalk_path, 'r') as crosswalk_file:
             crosswalk = json.load(crosswalk_file)
 
         return config, crosswalk
-    except json.JSONDecodeError as e:
-        print("Error parsing JSON file: {}".format(e))
+    except ValueError as e:
+        if isinstance(e, UnicodeDecodeError):
+            print("Error decoding JSON file: {}".format(e))
+        else:
+            print("Error parsing JSON file: {}".format(e))
         sys.exit(1)  # Exit the script due to a critical error in configuration loading
     except FileNotFoundError:
         print("One or both JSON files not found. Config: {}, Crosswalk: {}".format(config_path, crosswalk_path))
         sys.exit(1)  # Exit the script due to a critical error in configuration loading
     except KeyError as e:
         print("Critical configuration is missing: {}".format(e))
         sys.exit(1)  # Exit the script due to a critical error in configuration loading
```

### Comparing `medicafe-0.240501.1/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240501.2/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediLink/MediLink_Down.py` & `medicafe-0.240501.2/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240501.2/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediLink/MediLink_Gmail.py` & `medicafe-0.240501.2/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediLink/MediLink_Scheduler.py` & `medicafe-0.240501.2/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediLink/MediLink_UI.py` & `medicafe-0.240501.2/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/MediLink/MediLink_Up.py` & `medicafe-0.240501.2/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/PKG-INFO` & `medicafe-0.240501.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240501.1
+Version: 0.240501.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240501.1/README.md` & `medicafe-0.240501.2/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/medicafe.egg-info/PKG-INFO` & `medicafe-0.240501.2/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240501.1
+Version: 0.240501.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240501.1/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240501.2/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.1/setup.py` & `medicafe-0.240501.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version='0.240501.1',
+    version="0.240501.2",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

