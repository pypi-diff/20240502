# Comparing `tmp/pokernow-0.4.0.tar.gz` & `tmp/pokernow-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokernow-0.4.0.tar", last modified: Wed May  1 20:05:30 2024, max compression
+gzip compressed data, was "pokernow-0.5.1.tar", last modified: Thu May  2 21:23:31 2024, max compression
```

## Comparing `pokernow-0.4.0.tar` & `pokernow-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 20:05:30.721054 pokernow-0.4.0/
--rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10069 2024-05-01 20:05:30.721054 pokernow-0.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 20:05:30.707553 pokernow-0.4.0/PokerNow/
--rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.4.0/PokerNow/__init__.py
--rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.4.0/PokerNow/client.py
--rw-rw-rw-   0        0        0     9379 2024-05-01 20:01:50.000000 pokernow-0.4.0/PokerNow/managers.py
--rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.4.0/PokerNow/models.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:05:30.720055 pokernow-0.4.0/PokerNow.egg-info/
--rw-rw-rw-   0        0        0    10069 2024-05-01 20:05:30.000000 pokernow-0.4.0/PokerNow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-01 20:05:30.000000 pokernow-0.4.0/PokerNow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 20:05:30.000000 pokernow-0.4.0/PokerNow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 20:05:30.000000 pokernow-0.4.0/PokerNow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 20:05:30.000000 pokernow-0.4.0/PokerNow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 20:05:30.721054 pokernow-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-05-01 20:03:12.000000 pokernow-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:23:31.160185 pokernow-0.5.1/
+-rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    10069 2024-05-02 21:23:31.159156 pokernow-0.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 21:23:31.144553 pokernow-0.5.1/PokerNow/
+-rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.5.1/PokerNow/__init__.py
+-rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.5.1/PokerNow/client.py
+-rw-rw-rw-   0        0        0     9444 2024-05-02 21:19:56.000000 pokernow-0.5.1/PokerNow/managers.py
+-rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.5.1/PokerNow/models.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:23:31.158650 pokernow-0.5.1/PokerNow.egg-info/
+-rw-rw-rw-   0        0        0    10069 2024-05-02 21:23:31.000000 pokernow-0.5.1/PokerNow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-02 21:23:31.000000 pokernow-0.5.1/PokerNow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 21:23:31.000000 pokernow-0.5.1/PokerNow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 21:23:31.000000 pokernow-0.5.1/PokerNow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 21:23:31.000000 pokernow-0.5.1/PokerNow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 21:23:31.160185 pokernow-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-05-02 21:22:52.000000 pokernow-0.5.1/setup.py
```

### Comparing `pokernow-0.4.0/LICENSE` & `pokernow-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pokernow-0.4.0/PKG-INFO` & `pokernow-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.4.0
+Version: 0.5.1
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.4.0/PokerNow/client.py` & `pokernow-0.5.1/PokerNow/client.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.4.0/PokerNow/managers.py` & `pokernow-0.5.1/PokerNow/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import pickle
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
+from selenium.common.exceptions import NoSuchElementException 
 from selenium.webdriver.support import expected_conditions as EC
 from .models import Card, GameState, PlayerInfo, PlayerState
 
 class CookieManager:
     def __init__(self, driver, cookie_path):
         self.driver = driver
         self.cookie_path = cookie_path
@@ -33,15 +34,15 @@
             pot_size=self.parse_stack_value(self.element_helper.get_text('.table-pot-size .main-value')),
             community_cards=self.get_community_cards(),
             players=self.get_players_info(),
             dealer_position=self.get_dealer_position(),
             current_player=self.get_current_player(),
             blinds=self.get_blinds(),
             winners=self.get_winners(),
-            is_your_turn=self.is_your_turn()
+            is_your_turn=self.is_your_turn() 
         )
 
     def is_your_turn(self):
         try:
             action_signal = self.element_helper.get_element('.action-signal')
             return action_signal.text.strip() == 'Your Turn'
         except NoSuchElementException:
```

### Comparing `pokernow-0.4.0/PokerNow/models.py` & `pokernow-0.5.1/PokerNow/models.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.4.0/PokerNow.egg-info/PKG-INFO` & `pokernow-0.5.1/PokerNow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.4.0
+Version: 0.5.1
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.4.0/README.md` & `pokernow-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pokernow-0.4.0/setup.py` & `pokernow-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PokerNow',
-    version='0.4.0',
+    version='0.5.1',
     author='Zehm',
     author_email='mrtentacleshasallthetalent@gmail.com',
     description='A Python client for interacting with PokerNow games via the web.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Zehmosu/PokerNow/',
     packages=find_packages(),
```

