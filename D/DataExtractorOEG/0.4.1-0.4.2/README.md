# Comparing `tmp/dataextractoroeg-0.4.1.tar.gz` & `tmp/dataextractoroeg-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.4.1.tar", last modified: Thu May  2 11:24:32 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.4.2.tar", last modified: Thu May  2 11:31:09 2024, max compression
```

## Comparing `dataextractoroeg-0.4.1.tar` & `dataextractoroeg-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 11:24:32.629406 dataextractoroeg-0.4.1/
--rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.1/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-02 11:24:32.623432 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3046 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-02 11:24:32.000000 dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3046 2024-05-02 11:24:32.626126 dataextractoroeg-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 11:24:32.602765 dataextractoroeg-0.4.1/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-05-02 11:24:32.610029 dataextractoroeg-0.4.1/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.1/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.1/doiExtractor/ExistingPapers/name_doi_papers.csv
-drwxrwxrwx   0        0        0        0 2024-05-02 11:24:32.620453 dataextractoroeg-0.4.1/doiExtractor/Outputs/
--rw-rw-rw-   0        0        0        0 2024-05-02 10:56:36.000000 dataextractoroeg-0.4.1/doiExtractor/Outputs/dois.txt
--rw-rw-rw-   0        0        0    54972 2024-05-02 11:00:54.000000 dataextractoroeg-0.4.1/doiExtractor/Outputs/results.csv
--rw-rw-rw-   0        0        0   129283 2024-05-02 08:58:23.000000 dataextractoroeg-0.4.1/doiExtractor/Outputs/results.json
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.1/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8394 2024-05-02 11:18:54.000000 dataextractoroeg-0.4.1/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2454 2024-05-02 11:04:45.000000 dataextractoroeg-0.4.1/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4105 2024-05-02 11:18:31.000000 dataextractoroeg-0.4.1/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-05-02 11:24:32.630369 dataextractoroeg-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      592 2024-05-02 11:23:58.000000 dataextractoroeg-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:31:09.198516 dataextractoroeg-0.4.2/
+-rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.2/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-02 11:31:09.192032 dataextractoroeg-0.4.2/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3046 2024-05-02 11:31:08.000000 dataextractoroeg-0.4.2/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-05-02 11:31:09.000000 dataextractoroeg-0.4.2/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 11:31:08.000000 dataextractoroeg-0.4.2/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-02 11:31:08.000000 dataextractoroeg-0.4.2/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-02 11:31:08.000000 dataextractoroeg-0.4.2/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-02 11:31:08.000000 dataextractoroeg-0.4.2/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3046 2024-05-02 11:31:09.194035 dataextractoroeg-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 11:31:09.173378 dataextractoroeg-0.4.2/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-05-02 11:31:09.182453 dataextractoroeg-0.4.2/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.2/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.2/doiExtractor/ExistingPapers/name_doi_papers.csv
+drwxrwxrwx   0        0        0        0 2024-05-02 11:31:09.190036 dataextractoroeg-0.4.2/doiExtractor/Outputs/
+-rw-rw-rw-   0        0        0        0 2024-05-02 10:56:36.000000 dataextractoroeg-0.4.2/doiExtractor/Outputs/dois.txt
+-rw-rw-rw-   0        0        0    54972 2024-05-02 11:00:54.000000 dataextractoroeg-0.4.2/doiExtractor/Outputs/results.csv
+-rw-rw-rw-   0        0        0   129283 2024-05-02 08:58:23.000000 dataextractoroeg-0.4.2/doiExtractor/Outputs/results.json
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.2/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-02 11:30:33.000000 dataextractoroeg-0.4.2/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2454 2024-05-02 11:04:45.000000 dataextractoroeg-0.4.2/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4105 2024-05-02 11:18:31.000000 dataextractoroeg-0.4.2/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 11:31:09.198516 dataextractoroeg-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      592 2024-05-02 11:31:04.000000 dataextractoroeg-0.4.2/setup.py
```

### Comparing `dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.4.2/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.1
+Version: 0.4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.1/DataExtractorOEG.egg-info/SOURCES.txt` & `dataextractoroeg-0.4.2/DataExtractorOEG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.1/LICENSE.txt` & `dataextractoroeg-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.1/PKG-INFO` & `dataextractoroeg-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.4.1
+Version: 0.4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.4.1/README.md` & `dataextractoroeg-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.1/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.4.2/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.1/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.4.2/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.1/doiExtractor/Outputs/results.csv` & `dataextractoroeg-0.4.2/doiExtractor/Outputs/results.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.1/doiExtractor/Outputs/results.json` & `dataextractoroeg-0.4.2/doiExtractor/Outputs/results.json`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.1/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.4.2/doiExtractor/doiExtractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,14 @@
                 elif doi != "" and doi.startswith('10'):
                     output_file.write(doi + "\n")
                     print(f"No pdf found for {name}, wrote DOI instead: {doi}")
                 else:
                     print(f"No pdf or DOI found for {name}")
                 print("-----------------------------------------------------------------")
 
-create_txt("Outputs.csv", "Outputs.txt")
 
 def csv_to_json(csv_file, json_file):
     df = pd.read_csv(csv_file)
     df.to_json(json_file, orient='records', indent=4)
 
 
 def find_file_by_name(path, name):
```

### Comparing `dataextractoroeg-0.4.1/doiExtractor/main.py` & `dataextractoroeg-0.4.2/doiExtractor/main.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.1/doiExtractor/openAlex.py` & `dataextractoroeg-0.4.2/doiExtractor/openAlex.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.1/setup.py` & `dataextractoroeg-0.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.4.1",
+    version="0.4.2",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
         "pandas"
```

