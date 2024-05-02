# Comparing `tmp/dataextractoroeg-0.4.0.tar.gz` & `tmp/dataextractoroeg-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.4.0.tar", last modified: Thu May  2 10:52:23 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.4.1.tar", last modified: Thu May  2 11:24:32 2024, max compression
```

## Comparing `dataextractoroeg-0.4.0.tar` & `dataextractoroeg-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 10:52:23.393151 dataextractoroeg-0.4.0/
--rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.0/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-02 10:52:23.389054 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3046 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3046 2024-05-02 10:52:23.390055 dataextractoroeg-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 10:52:23.371416 dataextractoroeg-0.4.0/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-05-02 10:52:23.377655 dataextractoroeg-0.4.0/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.0/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.0/doiExtractor/ExistingPapers/name_doi_papers.csv
-drwxrwxrwx   0        0        0        0 2024-05-02 10:52:23.381822 dataextractoroeg-0.4.0/doiExtractor/Outputs/
--rw-rw-rw-   0        0        0        0 2024-05-02 09:14:00.000000 dataextractoroeg-0.4.0/doiExtractor/Outputs/dois.txt
--rw-rw-rw-   0        0        0        0 2024-05-02 09:32:18.000000 dataextractoroeg-0.4.0/doiExtractor/Outputs/results.csv
--rw-rw-rw-   0        0        0   129283 2024-05-02 08:58:23.000000 dataextractoroeg-0.4.0/doiExtractor/Outputs/results.json
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.0/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8307 2024-05-02 10:51:20.000000 dataextractoroeg-0.4.0/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2365 2024-05-02 09:09:51.000000 dataextractoroeg-0.4.0/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4109 2024-05-02 10:51:07.000000 dataextractoroeg-0.4.0/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-05-02 10:52:23.393151 dataextractoroeg-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      592 2024-05-02 10:52:17.000000 dataextractoroeg-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:24:32.629406 dataextractoroeg-0.4.1/
+-rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.1/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-02 11:24:32.623432 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3046 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3046 2024-05-02 11:24:32.626126 dataextractoroeg-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 11:24:32.602765 dataextractoroeg-0.4.1/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-05-02 11:24:32.610029 dataextractoroeg-0.4.1/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.1/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.1/doiExtractor/ExistingPapers/name_doi_papers.csv
+drwxrwxrwx   0        0        0        0 2024-05-02 11:24:32.620453 dataextractoroeg-0.4.1/doiExtractor/Outputs/
+-rw-rw-rw-   0        0        0        0 2024-05-02 10:56:36.000000 dataextractoroeg-0.4.1/doiExtractor/Outputs/dois.txt
+-rw-rw-rw-   0        0        0    54972 2024-05-02 11:00:54.000000 dataextractoroeg-0.4.1/doiExtractor/Outputs/results.csv
+-rw-rw-rw-   0        0        0   129283 2024-05-02 08:58:23.000000 dataextractoroeg-0.4.1/doiExtractor/Outputs/results.json
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.1/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8394 2024-05-02 11:18:54.000000 dataextractoroeg-0.4.1/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2454 2024-05-02 11:04:45.000000 dataextractoroeg-0.4.1/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4105 2024-05-02 11:18:31.000000 dataextractoroeg-0.4.1/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 11:24:32.630369 dataextractoroeg-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      592 2024-05-02 11:23:58.000000 dataextractoroeg-0.4.1/setup.py
```

### Comparing `dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.0
+Version: 0.4.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/SOURCES.txt` & `dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.0/LICENSE.txt` & `dataextractoroeg-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.0/PKG-INFO` & `dataextractoroeg-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.0
+Version: 0.4.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.0/README.md` & `dataextractoroeg-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.0/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.4.1/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.0/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.4.1/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.0/doiExtractor/Outputs/results.json` & `dataextractoroeg-0.4.1/doiExtractor/Outputs/results.json`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.0/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.4.1/doiExtractor/doiExtractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,28 +120,28 @@
 
         print("Total de Publicaciones:", total_publications)
         print("URLs con DOI:", publications_with_doi)
         print("Porcentaje de Publicaciones con DOI: {:.2f}%".format(doi_percentage))
 
 
 def remove_duplicates(csv_file):
-    df = pd.read_csv(csv_file)
+    df = pd.read_csv(csv_file, quoting=csv.QUOTE_ALL)
     
     # Drop duplicate rows based on the specified column
     df.drop_duplicates(subset=['NAME'], keep='first', inplace=True)
     
     # Write the modified DataFrame back to the CSV file
-    df.to_csv(csv_file, index=False)
+    df.to_csv(csv_file, index=False, quoting=csv.QUOTE_ALL)
 
 
 # Function to merge two CSV files
 def merge_csv(csv1, csv2):
     existing_dois = set()
 
-    # Collect DOIs from name-doi.csv
+    # Collect DOIs from results.csv
     with open(csv1, 'r', newline='', encoding='utf-8') as existing_file:
         reader = csv.reader(existing_file)
         next(reader)  # Skip header row
         for row in reader:
             doi = row[1]
             existing_dois.add(doi)
 
@@ -186,14 +186,15 @@
                 elif doi != "" and doi.startswith('10'):
                     output_file.write(doi + "\n")
                     print(f"No pdf found for {name}, wrote DOI instead: {doi}")
                 else:
                     print(f"No pdf or DOI found for {name}")
                 print("-----------------------------------------------------------------")
 
+create_txt("Outputs.csv", "Outputs.txt")
 
 def csv_to_json(csv_file, json_file):
     df = pd.read_csv(csv_file)
     df.to_json(json_file, orient='records', indent=4)
 
 
 def find_file_by_name(path, name):
```

### Comparing `dataextractoroeg-0.4.0/doiExtractor/main.py` & `dataextractoroeg-0.4.1/doiExtractor/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         logging.info(f"Search in: {url}, Output csv: {csv_filename}, Output txt: {txt_filename}")
 
         # Delete contents of the files if already created
         if os.path.exists(csv_filename):
             open(csv_filename, 'w').close()
         if os.path.exists(txt_filename):
             open(txt_filename, 'w').close()
+        if os.path.exists(json_filename):
+            open(json_filename, 'w').close()
 
         # Extract dois from url
         search_papers(url, url_docs, csv_filename)
 
         # Merge them with the existing from the papers
         merge_csv(csv_filename, papers)
```

### Comparing `dataextractoroeg-0.4.0/doiExtractor/openAlex.py` & `dataextractoroeg-0.4.1/doiExtractor/openAlex.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,9 +91,8 @@
     new_columns = list(rows[0].keys())  
     if "PRIMARY_LOCATION" not in new_columns: 
         new_columns.append("PRIMARY_LOCATION")
 
     with open(csv_filename, mode='w', newline='', encoding='utf-8') as file:
         writer = csv.DictWriter(file, quoting=csv.QUOTE_ALL, fieldnames=new_columns)
         writer.writeheader()
-        writer.writerows(rows)
-
+        writer.writerows(rows)
```

### Comparing `dataextractoroeg-0.4.0/setup.py` & `dataextractoroeg-0.4.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.4.0",
+    version="0.4.1",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
         "pandas"
```

