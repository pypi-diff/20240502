# Comparing `tmp/medicafe-0.240501.3.tar.gz` & `tmp/medicafe-0.240501.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240501.3.tar", last modified: Thu May  2 02:18:41 2024, max compression
+gzip compressed data, was "medicafe-0.240501.4.tar", last modified: Thu May  2 02:50:40 2024, max compression
```

## Comparing `medicafe-0.240501.3.tar` & `medicafe-0.240501.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 02:18:41.310000 medicafe-0.240501.3/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240501.3/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240501.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-02 02:18:40.326000 medicafe-0.240501.3/MediBot/
--rwxrwxrwx   0        0        0     2712 2024-05-02 00:07:18.000000 medicafe-0.240501.3/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    16168 2024-05-01 03:57:12.000000 medicafe-0.240501.3/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240501.3/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    29432 2024-05-02 02:13:29.000000 medicafe-0.240501.3/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240501.3/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240501.3/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240501.3/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240501.3/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240501.3/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240501.3/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240501.3/MediBot/update_json.py
--rw-rw-rw-   0        0        0      801 2024-04-20 02:05:15.000000 medicafe-0.240501.3/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-02 02:18:40.964000 medicafe-0.240501.3/MediLink/
--rw-rw-rw-   0        0        0    17570 2024-05-02 00:11:11.000000 medicafe-0.240501.3/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240501.3/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240501.3/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    33088 2024-05-01 04:35:27.000000 medicafe-0.240501.3/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3791 2024-05-01 23:56:13.000000 medicafe-0.240501.3/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    10677 2024-05-01 03:49:34.000000 medicafe-0.240501.3/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7123 2024-05-01 03:44:49.000000 medicafe-0.240501.3/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240501.3/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6313 2024-05-01 03:44:48.000000 medicafe-0.240501.3/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240501.3/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240501.3/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4950 2024-04-30 21:38:34.000000 medicafe-0.240501.3/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     6051 2024-05-01 03:44:47.000000 medicafe-0.240501.3/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240501.3/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240501.3/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240501.3/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-02 02:18:41.283000 medicafe-0.240501.3/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240501.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 02:18:41.256000 medicafe-0.240501.3/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-02 02:18:39.000000 medicafe-0.240501.3/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-02 02:18:39.000000 medicafe-0.240501.3/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 02:18:39.000000 medicafe-0.240501.3/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240501.3/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-02 02:18:39.000000 medicafe-0.240501.3/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-02 02:18:39.000000 medicafe-0.240501.3/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 02:18:41.303000 medicafe-0.240501.3/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-02 02:18:36.000000 medicafe-0.240501.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:50:40.669000 medicafe-0.240501.4/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240501.4/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240501.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-02 02:50:40.078000 medicafe-0.240501.4/MediBot/
+-rwxrwxrwx   0        0        0     2712 2024-05-02 00:07:18.000000 medicafe-0.240501.4/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    16168 2024-05-01 03:57:12.000000 medicafe-0.240501.4/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240501.4/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    29031 2024-05-02 02:41:51.000000 medicafe-0.240501.4/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240501.4/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240501.4/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240501.4/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240501.4/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240501.4/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240501.4/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240501.4/MediBot/update_json.py
+-rw-rw-rw-   0        0        0      829 2024-05-02 02:20:59.000000 medicafe-0.240501.4/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:50:40.492000 medicafe-0.240501.4/MediLink/
+-rw-rw-rw-   0        0        0    17570 2024-05-02 00:11:11.000000 medicafe-0.240501.4/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240501.4/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240501.4/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    33088 2024-05-01 04:35:27.000000 medicafe-0.240501.4/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3791 2024-05-01 23:56:13.000000 medicafe-0.240501.4/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    10677 2024-05-01 03:49:34.000000 medicafe-0.240501.4/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7123 2024-05-01 03:44:49.000000 medicafe-0.240501.4/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240501.4/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6313 2024-05-01 03:44:48.000000 medicafe-0.240501.4/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240501.4/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240501.4/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4950 2024-04-30 21:38:34.000000 medicafe-0.240501.4/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     6051 2024-05-01 03:44:47.000000 medicafe-0.240501.4/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240501.4/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240501.4/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240501.4/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-02 02:50:40.657000 medicafe-0.240501.4/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240501.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 02:50:40.642000 medicafe-0.240501.4/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-02 02:50:39.000000 medicafe-0.240501.4/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-02 02:50:39.000000 medicafe-0.240501.4/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 02:50:39.000000 medicafe-0.240501.4/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240501.4/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-02 02:50:39.000000 medicafe-0.240501.4/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-02 02:50:39.000000 medicafe-0.240501.4/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 02:50:40.667000 medicafe-0.240501.4/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-02 02:50:36.000000 medicafe-0.240501.4/setup.py
```

### Comparing `medicafe-0.240501.3/LICENSE` & `medicafe-0.240501.4/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediBot/MediBot.bat` & `medicafe-0.240501.4/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediBot/MediBot.py` & `medicafe-0.240501.4/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediBot/MediBot_Charges.py` & `medicafe-0.240501.4/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240501.4/MediBot/MediBot_Preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,38 +209,27 @@
         for filename in os.listdir(directory_path):
             file_path = os.path.join(directory_path, filename)
             if filename.endswith('.csv'):
                 try:
                     with open(file_path, 'r', encoding='utf-8') as csvfile:
                         reader = csv.DictReader(csvfile)
                         found_data = False  # Flag to track if any valid data is found in the CSV
-                        found_patient_id = False
-                        found_payer_id = False
                         for row in reader:
                             if 'Patient ID' not in row:
-                                found_patient_id = False
-                            else:
-                                found_patient_id = True
-                            if 'Ins1 Payer ID' not in row:
-                                found_payer_id = False
-                            else:
-                                found_payer_id = True
-
-                            if not found_patient_id and not found_payer_id:
                                 raise ValueError("CSV file '{}' is misformatted or empty.".format(filename))
-                            elif not found_patient_id:
-                                raise ValueError("CSV file '{}' is misformatted: Missing 'Patient ID' column.".format(filename))
-                            elif not found_payer_id:
-                                raise ValueError("CSV file '{}' is misformatted: Missing 'Ins1 Payer ID' column.".format(filename))
-
-                            if row['Patient ID'].strip() and row['Ins1 Payer ID'].strip():
+                            elif not row.get('Patient ID').strip():
+                                raise ValueError("CSV file '{}' is misformatted: Missing or empty 'Patient ID' in row {}".format(filename, row))
+                            elif not row.get('Ins1 Payer ID').strip():
+                                raise ValueError("CSV file '{}' is misformatted: Missing or empty 'Ins1 Payer ID' in row {}".format(filename, row))
+                            else:
                                 found_data = True
                                 payer_id = row['Ins1 Payer ID'].strip()
                                 patient_id = row['Patient ID'].strip()
                                 payer_to_patient_ids[payer_id].add(patient_id)
+                                MediLink_ConfigLoader.log("Found Patient ID {} with Payer ID {}".format(patient_id, payer_id))
                         if not found_data:
                             raise ValueError("CSV file '{}' is empty.".format(filename))
                 except Exception as e:
                     print("Error processing file {}: {}".format(filename, e))
     except FileNotFoundError as e:
         print("Error: {}".format(e))
```

### Comparing `medicafe-0.240501.3/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240501.4/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediBot/MediBot_UI.py` & `medicafe-0.240501.4/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240501.4/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240501.4/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediBot/update_json.py` & `medicafe-0.240501.4/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediBot/update_medicafe.py` & `medicafe-0.240501.4/MediBot/update_medicafe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import subprocess
 import sys
 from tqdm import tqdm
 
+# BUG This keeps failing
+
 def upgrade_medicafe(package):
     try:
         # Use tqdm to create a progress bar
         with tqdm(total=100, desc="Upgrading %s" % package, unit="%") as progress_bar:
             subprocess.check_call([sys.executable, '-m', 'pip', 'install', '--upgrade', package, '--no-deps', '--disable-pip-version-check'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
             # Update progress bar to 100% upon completion
             progress_bar.update(100 - progress_bar.n)
```

### Comparing `medicafe-0.240501.3/MediLink/MediLink.py` & `medicafe-0.240501.4/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_277_decoder.py` & `medicafe-0.240501.4/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240501.4/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240501.4/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240501.4/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240501.4/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_Down.py` & `medicafe-0.240501.4/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240501.4/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_Gmail.py` & `medicafe-0.240501.4/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_Scheduler.py` & `medicafe-0.240501.4/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_UI.py` & `medicafe-0.240501.4/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/MediLink/MediLink_Up.py` & `medicafe-0.240501.4/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/PKG-INFO` & `medicafe-0.240501.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240501.3
+Version: 0.240501.4
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240501.3/README.md` & `medicafe-0.240501.4/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/medicafe.egg-info/PKG-INFO` & `medicafe-0.240501.4/medicafe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240501.3
+Version: 0.240501.4
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240501.3/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240501.4/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240501.3/setup.py` & `medicafe-0.240501.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240501.3",
+    version="0.240501.4",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

