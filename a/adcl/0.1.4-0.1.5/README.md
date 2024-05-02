# Comparing `tmp/adcl-0.1.4.tar.gz` & `tmp/adcl-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adcl-0.1.4.tar", last modified: Thu May  2 06:54:11 2024, max compression
+gzip compressed data, was "dist\adcl-0.1.5.tar", last modified: Thu May  2 07:05:48 2024, max compression
```

## Comparing `adcl-0.1.4.tar` & `adcl-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 06:54:11.000000 adcl-0.1.4/
--rw-rw-rw-   0        0        0     1091 2024-05-01 20:17:28.000000 adcl-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     4292 2024-05-02 06:54:11.000000 adcl-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3754 2024-05-01 20:17:28.000000 adcl-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 06:54:11.000000 adcl-0.1.4/adcl/
--rw-rw-rw-   0        0        0       35 2024-05-01 20:17:28.000000 adcl-0.1.4/adcl/__init__.py
--rw-rw-rw-   0        0        0    53906 2024-05-01 20:17:28.000000 adcl-0.1.4/adcl/data_preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:54:11.000000 adcl-0.1.4/adcl.egg-info/
--rw-rw-rw-   0        0        0     4292 2024-05-02 06:54:10.000000 adcl-0.1.4/adcl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-02 06:54:10.000000 adcl-0.1.4/adcl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 06:54:10.000000 adcl-0.1.4/adcl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      226 2024-05-02 06:54:10.000000 adcl-0.1.4/adcl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-02 06:54:10.000000 adcl-0.1.4/adcl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 06:54:11.000000 adcl-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1020 2024-05-02 06:53:37.000000 adcl-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:05:48.000000 adcl-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2024-05-01 20:17:28.000000 adcl-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      967 2024-05-02 07:05:48.000000 adcl-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3754 2024-05-01 20:17:28.000000 adcl-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl/
+-rw-rw-rw-   0        0        0       35 2024-05-01 20:17:28.000000 adcl-0.1.5/adcl/__init__.py
+-rw-rw-rw-   0        0        0    53906 2024-05-01 20:17:28.000000 adcl-0.1.5/adcl/data_preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/
+-rw-rw-rw-   0        0        0      967 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      131 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 07:05:48.000000 adcl-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1862 2024-05-02 07:04:43.000000 adcl-0.1.5/setup.py
```

### Comparing `adcl-0.1.4/LICENSE` & `adcl-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adcl-0.1.4/PKG-INFO` & `adcl-0.1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: adcl
-Version: 0.1.4
-Summary: Data preprocessing and cleaning tools for data science projects
-Home-page: https://github.com/maykov-stepan/ADCL-Automatic-Data-Cleaning
-Author: Maykov Stepan
-Author-email: steve19992@mail.ru
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # README for ADCL-Automatic-Data-Cleaning Project
 
 ## Overview
 ADCL-Automatic-Data-Cleaning is a Python package designed to facilitate automated data cleaning, particularly leveraging deep learning techniques. This project focuses on improving accuracy and efficiency in preprocessing tasks essential for data science and machine learning workflows.
 
 ## Features
 - **Data Preprocessing:** Standardize, normalize, and format your data for machine learning models.
```

### Comparing `adcl-0.1.4/adcl/data_preprocessing.py` & `adcl-0.1.5/adcl/data_preprocessing.py`

 * *Files identical despite different names*

