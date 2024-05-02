# Comparing `tmp/simic-1.1.tar.gz` & `tmp/simic-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simic-1.1.tar", last modified: Fri Apr 26 17:43:46 2024, max compression
+gzip compressed data, was "simic-1.2.tar", last modified: Thu May  2 15:31:02 2024, max compression
```

## Comparing `simic-1.1.tar` & `simic-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 17:43:46.027000 simic-1.1/
--rw-rw-rw-   0        0        0       50 2024-04-26 17:43:45.981000 simic-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-26 17:43:46.014000 simic-1.1/setup.cfg
--rw-rw-rw-   0        0        0      169 2024-04-26 17:37:07.000000 simic-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 17:43:45.117000 simic-1.1/simic/
--rw-rw-rw-   0        0        0       20 2024-04-25 14:59:26.000000 simic-1.1/simic/__init__.py
--rw-rw-rw-   0        0        0     5070 2024-04-26 17:42:12.000000 simic-1.1/simic/xpath.py
-drwxrwxrwx   0        0        0        0 2024-04-26 17:43:45.917000 simic-1.1/simic.egg-info/
--rw-rw-rw-   0        0        0       50 2024-04-26 17:43:43.000000 simic-1.1/simic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-04-26 17:43:44.000000 simic-1.1/simic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 17:43:43.000000 simic-1.1/simic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-26 17:43:43.000000 simic-1.1/simic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 17:43:43.000000 simic-1.1/simic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 15:31:02.620000 simic-1.2/
+-rw-rw-rw-   0        0        0       50 2024-05-02 15:31:02.569000 simic-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-02 15:31:02.609000 simic-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      169 2024-05-02 14:15:09.000000 simic-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:31:01.836000 simic-1.2/simic/
+-rw-rw-rw-   0        0        0       20 2024-04-25 14:59:26.000000 simic-1.2/simic/__init__.py
+-rw-rw-rw-   0        0        0     4444 2024-05-02 14:15:52.000000 simic-1.2/simic/xpath.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:31:02.503000 simic-1.2/simic.egg-info/
+-rw-rw-rw-   0        0        0       50 2024-05-02 15:31:01.000000 simic-1.2/simic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-02 15:31:01.000000 simic-1.2/simic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 15:31:01.000000 simic-1.2/simic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 15:31:01.000000 simic-1.2/simic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 15:31:01.000000 simic-1.2/simic.egg-info/top_level.txt
```

### Comparing `simic-1.1/simic/xpath.py` & `simic-1.2/simic/xpath.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,29 +11,14 @@
 import sqlite3
 import os
 import random
 from selenium.webdriver import Firefox
 from selenium.webdriver.firefox.options import Options
 from selenium.webdriver.firefox.firefox_binary import FirefoxBinary
 
-'''
-firefox_options = Options()
-firefox_options.headless = False
-binary = FirefoxBinary(r"C:\Program Files\Mozilla Firefox\firefox.exe")
-navegador = Firefox(executable_path=r"C:\Users\GabrielSoaresSímic\AppData\Local\Programs\Python\Python311\geckodriver.exe", firefox_binary=binary, options=firefox_options)
-navegador.get('https://one.fracttal.com/')
-navegador.maximize_window()
-'''
-
-engine = pyttsx3.init()
-def speak(audio):
-    engine.say(audio)
-    engine.runAndWait()
-
-# Funções selenium
 
 def crtl_a(navegador):
     action = ActionChains(navegador)
     action.key_down(Keys.CONTROL).send_keys('A').key_up(Keys.CONTROL).perform()
 
 def Try_find_xp(navegador,elemento,timee):
     found=False
@@ -118,15 +103,15 @@
 
 def get_text(navegador,elemento):
 
     a = navegador.find_element(By.XPATH,elemento).text
     
     return a
 
-def click_in_list(elemento,string):
+def click_in_list(navegador,elemento,string):
     err=True
     loop=0
     while loop<5:
         for i in navegador.find_elements(By.XPATH, elemento):
             try:
                 if string in i.text:
                     a=i.text
@@ -155,16 +140,9 @@
             err1+=1
             print ("Loading took too much time!" + str(elemento))
             time.sleep(1)
     if error: return boo
     if not boo: 1/0 #forçar error
     return boo
 
-    
-# Funções automação
-
-engine = pyttsx3.init()
-def speak(audio):
-    engine.say(audio)
-    engine.runAndWait()
```

