# Comparing `tmp/Andreani_QA_Selenium-0.0.8.tar.gz` & `tmp/Andreani_QA_Selenium-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Selenium-0.0.8.tar", last modified: Wed Jul 19 19:51:12 2023, max compression
+gzip compressed data, was "Andreani_QA_Selenium-0.0.9.tar", last modified: Tue Jul 25 14:50:21 2023, max compression
```

## Comparing `Andreani_QA_Selenium-0.0.8.tar` & `Andreani_QA_Selenium-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 19:51:12.443936 Andreani_QA_Selenium-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-07-19 19:51:12.402715 Andreani_QA_Selenium-0.0.8/Andreani_QA_Selenium/
--rw-rw-rw-   0        0        0    97766 2023-07-19 19:44:19.000000 Andreani_QA_Selenium-0.0.8/Andreani_QA_Selenium/Selenium.py
--rw-rw-rw-   0        0        0       32 2023-06-14 17:07:42.000000 Andreani_QA_Selenium-0.0.8/Andreani_QA_Selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 19:51:12.437270 Andreani_QA_Selenium-0.0.8/Andreani_QA_Selenium.egg-info/
--rw-rw-rw-   0        0        0      310 2023-07-19 19:51:12.000000 Andreani_QA_Selenium-0.0.8/Andreani_QA_Selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-19 19:51:12.000000 Andreani_QA_Selenium-0.0.8/Andreani_QA_Selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 19:51:12.000000 Andreani_QA_Selenium-0.0.8/Andreani_QA_Selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2023-07-19 19:51:12.000000 Andreani_QA_Selenium-0.0.8/Andreani_QA_Selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-19 19:51:12.000000 Andreani_QA_Selenium-0.0.8/Andreani_QA_Selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      310 2023-07-19 19:51:12.441404 Andreani_QA_Selenium-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Selenium-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-19 19:51:12.443936 Andreani_QA_Selenium-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1259 2023-07-19 19:50:46.000000 Andreani_QA_Selenium-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:50:21.354986 Andreani_QA_Selenium-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-07-25 14:50:21.329517 Andreani_QA_Selenium-0.0.9/Andreani_QA_Selenium/
+-rw-rw-rw-   0        0        0    97912 2023-07-24 18:05:15.000000 Andreani_QA_Selenium-0.0.9/Andreani_QA_Selenium/Selenium.py
+-rw-rw-rw-   0        0        0       32 2023-06-14 17:07:42.000000 Andreani_QA_Selenium-0.0.9/Andreani_QA_Selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:50:21.349855 Andreani_QA_Selenium-0.0.9/Andreani_QA_Selenium.egg-info/
+-rw-rw-rw-   0        0        0      271 2023-07-25 14:50:21.000000 Andreani_QA_Selenium-0.0.9/Andreani_QA_Selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-25 14:50:21.000000 Andreani_QA_Selenium-0.0.9/Andreani_QA_Selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:50:21.000000 Andreani_QA_Selenium-0.0.9/Andreani_QA_Selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2023-07-25 14:50:21.000000 Andreani_QA_Selenium-0.0.9/Andreani_QA_Selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-25 14:50:21.000000 Andreani_QA_Selenium-0.0.9/Andreani_QA_Selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      271 2023-07-25 14:50:21.353988 Andreani_QA_Selenium-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Selenium-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:50:21.354986 Andreani_QA_Selenium-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1259 2023-07-25 14:28:22.000000 Andreani_QA_Selenium-0.0.9/setup.py
```

### Comparing `Andreani_QA_Selenium-0.0.8/Andreani_QA_Selenium/Selenium.py` & `Andreani_QA_Selenium-0.0.9/Andreani_QA_Selenium/Selenium.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,16 +202,17 @@
 
         if version == "":
             return version
 
         if browser == "CHROME":
             version = f"{version.split('.')[0]}.{version.split('.')[1]}.{version.split('.')[2]}"
             response = requests.get(f"https://chromedriver.storage.googleapis.com/LATEST_RELEASE_{version}")
+            if response.status_code == 404:
+                response = requests.get("https://chromedriver.storage.googleapis.com/LATEST_RELEASE")
             version = response.text
-
         return version
 
     def tear_down(self):
 
         """
             Descripcion:
                 Finaliza la ejecución cerrando el Web Driver.
```

### Comparing `Andreani_QA_Selenium-0.0.8/setup.py` & `Andreani_QA_Selenium-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 PACKAGE_NAME = 'Andreani_QA_Selenium'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'SeleniumFramework para ejecución de casos automatizados'  # Descripción corta
```

