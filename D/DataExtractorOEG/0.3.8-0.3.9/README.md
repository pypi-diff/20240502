# Comparing `tmp/dataextractoroeg-0.3.8.tar.gz` & `tmp/dataextractoroeg-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.3.8.tar", last modified: Mon Apr 29 13:45:03 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.3.9.tar", last modified: Thu May  2 08:35:53 2024, max compression
```

## Comparing `dataextractoroeg-0.3.8.tar` & `dataextractoroeg-0.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 13:45:03.961120 dataextractoroeg-0.3.8/
--rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.3.8/.gitignore
-drwxrwxrwx   0        0        0        0 2024-04-29 13:45:03.955124 dataextractoroeg-0.3.8/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3046 2024-04-29 13:45:03.000000 dataextractoroeg-0.3.8/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2024-04-29 13:45:03.000000 dataextractoroeg-0.3.8/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 13:45:03.000000 dataextractoroeg-0.3.8/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-29 13:45:03.000000 dataextractoroeg-0.3.8/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-29 13:45:03.000000 dataextractoroeg-0.3.8/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 13:45:03.000000 dataextractoroeg-0.3.8/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0     3046 2024-04-29 13:45:03.958117 dataextractoroeg-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 13:45:03.933314 dataextractoroeg-0.3.8/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-04-29 13:45:03.941675 dataextractoroeg-0.3.8/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.3.8/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.3.8/doiExtractor/ExistingPapers/name_doi_papers.csv
-drwxrwxrwx   0        0        0        0 2024-04-29 13:45:03.951122 dataextractoroeg-0.3.8/doiExtractor/Outputs/
--rw-rw-rw-   0        0        0    14166 2024-04-26 10:27:22.000000 dataextractoroeg-0.3.8/doiExtractor/Outputs/dois.txt
--rw-rw-rw-   0        0        0    77928 2024-04-25 14:42:00.000000 dataextractoroeg-0.3.8/doiExtractor/Outputs/results.csv
--rw-rw-rw-   0        0        0   123715 2024-04-29 12:01:52.000000 dataextractoroeg-0.3.8/doiExtractor/Outputs/results.json
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.3.8/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8259 2024-04-29 13:44:36.000000 dataextractoroeg-0.3.8/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2365 2024-04-29 13:44:46.000000 dataextractoroeg-0.3.8/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4086 2024-04-29 11:57:15.000000 dataextractoroeg-0.3.8/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-04-29 13:45:03.961120 dataextractoroeg-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      592 2024-04-29 13:44:55.000000 dataextractoroeg-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 08:35:53.305415 dataextractoroeg-0.3.9/
+-rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.3.9/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-02 08:35:53.298184 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3046 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3046 2024-05-02 08:35:53.298184 dataextractoroeg-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 08:35:53.252202 dataextractoroeg-0.3.9/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-05-02 08:35:53.284916 dataextractoroeg-0.3.9/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.3.9/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.3.9/doiExtractor/ExistingPapers/name_doi_papers.csv
+drwxrwxrwx   0        0        0        0 2024-05-02 08:35:53.290180 dataextractoroeg-0.3.9/doiExtractor/Outputs/
+-rw-rw-rw-   0        0        0    14166 2024-04-26 10:27:22.000000 dataextractoroeg-0.3.9/doiExtractor/Outputs/dois.txt
+-rw-rw-rw-   0        0        0    77928 2024-04-25 14:42:00.000000 dataextractoroeg-0.3.9/doiExtractor/Outputs/results.csv
+-rw-rw-rw-   0        0        0   123715 2024-04-29 12:01:52.000000 dataextractoroeg-0.3.9/doiExtractor/Outputs/results.json
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.3.9/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8406 2024-05-02 08:32:41.000000 dataextractoroeg-0.3.9/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2365 2024-04-29 13:44:46.000000 dataextractoroeg-0.3.9/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4086 2024-04-29 11:57:15.000000 dataextractoroeg-0.3.9/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 08:35:53.305415 dataextractoroeg-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      592 2024-05-02 08:27:10.000000 dataextractoroeg-0.3.9/setup.py
```

### Comparing `dataextractoroeg-0.3.8/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3.8
+Version: 0.3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.3.8/DataExtractorOEG.egg-info/SOURCES.txt` & `dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.8/LICENSE.txt` & `dataextractoroeg-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.8/PKG-INFO` & `dataextractoroeg-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3.8
+Version: 0.3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.3.8/README.md` & `dataextractoroeg-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.8/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.3.9/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.8/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.3.9/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.8/doiExtractor/Outputs/dois.txt` & `dataextractoroeg-0.3.9/doiExtractor/Outputs/dois.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.8/doiExtractor/Outputs/results.csv` & `dataextractoroeg-0.3.9/doiExtractor/Outputs/results.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.8/doiExtractor/Outputs/results.json` & `dataextractoroeg-0.3.9/doiExtractor/Outputs/results.json`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.8/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.3.9/doiExtractor/doiExtractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,18 @@
                 next_sibling = doi_text.find_next_sibling(string=True)
                 if next_sibling and next_sibling.strip():
                     # Extract DOI
                     doi = next_sibling.strip()
                     if doi.startswith('https://doi.org/'):
                         doi = doi[len('https://doi.org/'):]  # Remove "https://doi.org/" from the beginning if present
                     # Write the resulting DOI to the CSV file
-                    csv_file.writerow([title, doi])
+                    if title.startswith('"'):
+                        csv_file.writerow([title, doi])
+                    else:
+                        csv_file.writerow(['"' + title + '"', doi])
                     doi_found = True
                 else:
                     csv_file.writerow([title, "None"])
                     doi_found = False
                     
         return doi_found  # Return if DOI is found or not
     else:
```

### Comparing `dataextractoroeg-0.3.8/doiExtractor/main.py` & `dataextractoroeg-0.3.9/doiExtractor/main.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.8/doiExtractor/openAlex.py` & `dataextractoroeg-0.3.9/doiExtractor/openAlex.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.8/setup.py` & `dataextractoroeg-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.3.8",
+    version="0.3.9",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
         "pandas"
```

