# Comparing `tmp/operationbattleshipcommonutilities-0.4.5.tar.gz` & `tmp/operationbattleshipcommonutilities-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operationbattleshipcommonutilities-0.4.5.tar", last modified: Mon Apr 29 00:43:48 2024, max compression
+gzip compressed data, was "operationbattleshipcommonutilities-0.4.6.tar", last modified: Wed May  1 13:38:06 2024, max compression
```

## Comparing `operationbattleshipcommonutilities-0.4.5.tar` & `operationbattleshipcommonutilities-0.4.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 00:43:48.019741 operationbattleshipcommonutilities-0.4.5/
--rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 operationbattleshipcommonutilities-0.4.5/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-29 00:43:48.010781 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/
--rw-rw-rw-   0        0        0     3177 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3177 2024-04-29 00:43:48.013732 operationbattleshipcommonutilities-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 operationbattleshipcommonutilities-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 00:43:47.967735 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/
--rw-rw-rw-   0        0        0     4577 2024-03-24 01:03:06.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/ApifyJobsCaller.py
--rw-rw-rw-   0        0        0     2601 2024-04-01 21:52:27.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/CandidateRequirementsDao.py
--rw-rw-rw-   0        0        0     6556 2024-04-23 05:23:30.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/CompanyDao.py
--rw-rw-rw-   0        0        0     3143 2024-04-01 21:48:50.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/FailureLogger.py
--rw-rw-rw-   0        0        0     1513 2024-04-01 23:24:18.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/GenaricDatabaseDao.py
--rw-rw-rw-   0        0        0     2219 2024-04-01 21:47:52.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/GeographyHelper.py
--rw-rw-rw-   0        0        0     3365 2024-04-01 21:47:37.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobKeyWordsDao.py
--rw-rw-rw-   0        0        0     4132 2024-04-28 16:36:13.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobPostingDao.py
--rw-rw-rw-   0        0        0     1706 2024-04-01 21:39:48.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobResponsibilitiesDao.py
--rw-rw-rw-   0        0        0     2848 2024-04-01 21:39:04.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobSkillsDao.py
--rw-rw-rw-   0        0        0     1830 2024-02-17 14:46:22.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
--rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/NomicAICaller.py
--rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/OpenAICaller.py
--rw-rw-rw-   0        0        0     3332 2024-04-23 05:20:23.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/PineConeDatabaseCaller.py
--rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-29 00:43:48.019741 operationbattleshipcommonutilities-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-04-29 00:38:03.000000 operationbattleshipcommonutilities-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 13:38:06.569834 operationbattleshipcommonutilities-0.4.6/
+-rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 operationbattleshipcommonutilities-0.4.6/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-01 13:38:06.563837 operationbattleshipcommonutilities-0.4.6/OperationBattleshipCommonUtilities.egg-info/
+-rw-rw-rw-   0        0        0     3177 2024-05-01 13:38:06.000000 operationbattleshipcommonutilities-0.4.6/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3177 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.6/OperationBattleshipCommonUtilities.egg-info/PKG-INFO-DESKTOP-QHT5QD9
+-rw-rw-rw-   0        0        0     1251 2024-05-01 13:38:06.000000 operationbattleshipcommonutilities-0.4.6/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 13:38:06.000000 operationbattleshipcommonutilities-0.4.6/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-01 13:38:06.000000 operationbattleshipcommonutilities-0.4.6/OperationBattleshipCommonUtilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-05-01 13:38:06.000000 operationbattleshipcommonutilities-0.4.6/OperationBattleshipCommonUtilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3177 2024-05-01 13:38:06.565348 operationbattleshipcommonutilities-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 operationbattleshipcommonutilities-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 13:38:06.561834 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/
+-rw-rw-rw-   0        0        0     4579 2024-04-30 13:45:27.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/ApifyJobsCaller.py
+-rw-rw-rw-   0        0        0     2601 2024-04-01 21:52:27.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/CandidateRequirementsDao.py
+-rw-rw-rw-   0        0        0     6557 2024-04-30 13:36:40.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/CompanyDao.py
+-rw-rw-rw-   0        0        0     3143 2024-04-01 21:48:50.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/FailureLogger.py
+-rw-rw-rw-   0        0        0     1513 2024-04-01 23:24:18.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/GenaricDatabaseDao.py
+-rw-rw-rw-   0        0        0     2219 2024-04-01 21:47:52.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/GeographyHelper.py
+-rw-rw-rw-   0        0        0     3365 2024-04-01 21:47:37.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/JobKeyWordsDao.py
+-rw-rw-rw-   0        0        0     5843 2024-05-01 13:34:36.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/JobPostingDao.py
+-rw-rw-rw-   0        0        0     1706 2024-04-01 21:39:48.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/JobResponsibilitiesDao.py
+-rw-rw-rw-   0        0        0     2848 2024-04-01 21:39:04.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/JobSkillsDao.py
+-rw-rw-rw-   0        0        0     1727 2024-04-30 13:44:59.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
+-rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/NomicAICaller.py
+-rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/OpenAICaller.py
+-rw-rw-rw-   0        0        0     3332 2024-04-23 05:20:23.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/PineConeDatabaseCaller.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-01 13:38:06.569834 operationbattleshipcommonutilities-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-05-01 13:28:47.000000 operationbattleshipcommonutilities-0.4.6/setup.py
```

### Comparing `operationbattleshipcommonutilities-0.4.5/LICENSE` & `operationbattleshipcommonutilities-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/PKG-INFO` & `operationbattleshipcommonutilities-0.4.6/OperationBattleshipCommonUtilities.egg-info/PKG-INFO-DESKTOP-QHT5QD9`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt` & `operationbattleshipcommonutilities-0.4.6/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 OperationBattleshipCommonUtilities.egg-info/PKG-INFO
+OperationBattleshipCommonUtilities.egg-info/PKG-INFO-DESKTOP-QHT5QD9
 OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
 OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
 OperationBattleshipCommonUtilities.egg-info/requires.txt
 OperationBattleshipCommonUtilities.egg-info/top_level.txt
 operation_battleship_common_utilities/ApifyJobsCaller.py
 operation_battleship_common_utilities/CandidateRequirementsDao.py
 operation_battleship_common_utilities/CompanyDao.py
```

### Comparing `operationbattleshipcommonutilities-0.4.5/PKG-INFO` & `operationbattleshipcommonutilities-0.4.6/OperationBattleshipCommonUtilities.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.4.5
+Version: 0.4.6
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `operationbattleshipcommonutilities-0.4.5/README.md` & `operationbattleshipcommonutilities-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/ApifyJobsCaller.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/ApifyJobsCaller.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 import random
 import string
 from datetime import datetime
 from dotenv import load_dotenv
 from apify_client import ApifyClient
 
 
+load_dotenv('.env')
 
 # Configure logging
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
-load_dotenv('.env')
 
 class ApifyJobsCaller:
     def __init__(self):
         logging.info(f"{self.__class__.__name__} class initialized")
 
 
 
     
     #This function will call the Apify Python SDK and run the job. It requires a job title. 
     #The expectation is that this is the only function that actually calls the API SDK. 
     def execute_new_jobs_crawler(self, job_title_name, duration):
-        logging.info(f"Beginning the process for collecting {job_title_name} jobs from Apify Job Crawler")
+        logging.info(f"Beginning the process for collecting {job_title_name} jobs from Apify Job Crawlerin")
 
         apifytokenFromEnv = os.getenv("APIFY_CLIENT_TOKEN")  # Ensure correct environment variable name
         client = ApifyClient(apifytokenFromEnv)
 
         # Prepare the Actor input based on duration
         publishedAt = ""  # Default to empty, assuming it handles 'anytime' if not provided
         if duration == 1:
```

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/CandidateRequirementsDao.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/CandidateRequirementsDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/CompanyDao.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/CompanyDao.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             
             cur.close()
             conn.close()
 
             if rows:
                 return rows[0][0]  
             else:
-                logging.info(f"Error in getting Company Name. We always expect an name in this function. Failed for company id: {company_id} ")
+                logging.error(f"Error in getting Company Name. We always expect an name in this function. Failed for company id: {company_id} ")
                 return None  
 
         except Exception as e:
             logging.error("Database connection error:", e)
             logging.error(f"Database error in CompanyDao.getCompanyNameByCompanyId for Company at: {company_id} ")
             
             if 'conn' in locals():
```

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/FailureLogger.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/FailureLogger.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/GenaricDatabaseDao.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/GenaricDatabaseDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/GeographyHelper.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/GeographyHelper.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobKeyWordsDao.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/JobKeyWordsDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobResponsibilitiesDao.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/JobResponsibilitiesDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobSkillsDao.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/JobSkillsDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobTitleCategoryClassifier.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/JobTitleCategoryClassifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,20 +22,23 @@
 
 import logging
 from dotenv import load_dotenv
 import pandas as pd
 
 load_dotenv('.env')
 
+logging.basicConfig(level=logging.INFO)  
+
+
 class JobTitleCategoryClassifier:
     def __init__(self):
-        logging.basicConfig(level=logging.INFO)  # Ensure logger is set up
-        self.logger = logging.getLogger(__name__)  # Get a logger for this class
-        self.logger.info(f"{self.__class__.__name__} class initialized")
+
+        logging.info(f"{self.__class__.__name__} class initialized")
         self.data_frame = pd.read_csv('CommonUtilities/Configuration/JobCategories.csv')
+        
 
     def get_job_category(self, job_title):
         """
         Load the CSV Configuration File as a Pandas DataFrame.
         Relative Path = CommonUtilities\Configuration\JobCategories.csv
         Check to see if the Job title is listed in the data frame and then use the job category. 
         Return whatever category has been found.
```

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/NomicAICaller.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/NomicAICaller.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/OpenAICaller.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/OpenAICaller.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/PineConeDatabaseCaller.py` & `operationbattleshipcommonutilities-0.4.6/operation_battleship_common_utilities/PineConeDatabaseCaller.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.5/setup.py` & `operationbattleshipcommonutilities-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='OperationBattleshipCommonUtilities',
-    version='0.4.5',
+    version='0.4.6',
     packages=find_packages(),
     license='Apache-2.0 license',
     description='Classes and Utilities that are shared in the Operation Battleship Application',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Matthew Caraway',
     author_email='matthew@CarawayLabs.com',
```

