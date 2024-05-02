# Comparing `tmp/simic-1.5.1.tar.gz` & `tmp/simic-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simic-1.5.1.tar", last modified: Thu May  2 17:27:24 2024, max compression
+gzip compressed data, was "simic-1.5.2.tar", last modified: Thu May  2 17:35:45 2024, max compression
```

## Comparing `simic-1.5.1.tar` & `simic-1.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 17:27:24.056000 simic-1.5.1/
--rw-rw-rw-   0        0        0       52 2024-05-02 17:27:24.014000 simic-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-02 17:27:24.043000 simic-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      171 2024-05-02 17:27:17.000000 simic-1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:27:23.618000 simic-1.5.1/simic/
--rw-rw-rw-   0        0        0       20 2024-04-25 14:59:26.000000 simic-1.5.1/simic/__init__.py
--rw-rw-rw-   0        0        0     4383 2024-05-02 16:48:28.000000 simic-1.5.1/simic/xpath.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:27:23.945000 simic-1.5.1/simic.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-02 17:27:23.000000 simic-1.5.1/simic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-05-02 17:27:23.000000 simic-1.5.1/simic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 17:27:23.000000 simic-1.5.1/simic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 17:27:23.000000 simic-1.5.1/simic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-02 17:27:23.000000 simic-1.5.1/simic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 17:35:45.623000 simic-1.5.2/
+-rw-rw-rw-   0        0        0       52 2024-05-02 17:35:45.568000 simic-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-02 17:35:45.609000 simic-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      171 2024-05-02 17:35:35.000000 simic-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:35:45.002000 simic-1.5.2/simic/
+-rw-rw-rw-   0        0        0      304 2024-05-02 17:35:03.000000 simic-1.5.2/simic/__init__.py
+-rw-rw-rw-   0        0        0     4103 2024-05-02 17:34:57.000000 simic-1.5.2/simic/xpath.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:35:45.508000 simic-1.5.2/simic.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-02 17:35:44.000000 simic-1.5.2/simic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-02 17:35:44.000000 simic-1.5.2/simic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 17:35:44.000000 simic-1.5.2/simic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 17:35:44.000000 simic-1.5.2/simic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 17:35:44.000000 simic-1.5.2/simic.egg-info/top_level.txt
```

### Comparing `simic-1.5.1/simic/xpath.py` & `simic-1.5.2/simic/xpath.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-from selenium import webdriver
+
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import TimeoutException
 import time
 from selenium.webdriver.common.action_chains import ActionChains 
 from selenium.webdriver.common.keys import Keys
-from concurrent.futures import ThreadPoolExecutor
-import pandas as pd
-import random
-from selenium.webdriver import Firefox
-from selenium.webdriver.firefox.options import Options
-from selenium.webdriver.firefox.firefox_binary import FirefoxBinary
+
 
 
 def crtl_a(navegador):
     action = ActionChains(navegador)
     action.key_down(Keys.CONTROL).send_keys('A').key_up(Keys.CONTROL).perform()
 
 def Try_find_xp(navegador,elemento,timee):
```

