# Comparing `tmp/fivesim-1.1.0.tar.gz` & `tmp/fivesim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fivesim-1.1.0.tar", last modified: Sat Aug  6 10:44:38 2022, max compression
+gzip compressed data, was "fivesim-1.2.0.tar", last modified: Thu May  2 21:30:52 2024, max compression
```

## Comparing `fivesim-1.1.0.tar` & `fivesim-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-08-06 10:44:38.391870 fivesim-1.1.0/
--rw-rw-rw-   0        0        0     1092 2022-07-23 14:08:11.000000 fivesim-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     5274 2022-08-06 10:44:38.387869 fivesim-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3290 2022-07-31 14:24:08.000000 fivesim-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-08-06 10:44:38.360870 fivesim-1.1.0/fivesim/
--rw-rw-rw-   0        0        0      640 2022-07-31 20:45:49.000000 fivesim-1.1.0/fivesim/__init__.py
--rw-rw-rw-   0        0        0    16043 2022-07-31 12:58:42.000000 fivesim-1.1.0/fivesim/api.py
--rw-rw-rw-   0        0        0    21200 2022-07-30 10:52:01.000000 fivesim-1.1.0/fivesim/enums.py
--rw-rw-rw-   0        0        0     1819 2022-08-06 10:36:31.000000 fivesim-1.1.0/fivesim/errors.py
--rw-rw-rw-   0        0        0      384 2022-07-31 11:46:52.000000 fivesim-1.1.0/fivesim/fivesim.py
--rw-rw-rw-   0        0        0     7227 2022-07-31 13:49:10.000000 fivesim-1.1.0/fivesim/json_response.py
--rw-rw-rw-   0        0        0        0 2022-07-31 20:36:11.000000 fivesim-1.1.0/fivesim/py.typed
--rw-rw-rw-   0        0        0     3696 2022-08-06 10:40:44.000000 fivesim-1.1.0/fivesim/request.py
--rw-rw-rw-   0        0        0     2229 2022-07-31 14:08:02.000000 fivesim-1.1.0/fivesim/response.py
-drwxrwxrwx   0        0        0        0 2022-08-06 10:44:38.385871 fivesim-1.1.0/fivesim.egg-info/
--rw-rw-rw-   0        0        0     5274 2022-08-06 10:44:38.000000 fivesim-1.1.0/fivesim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2022-08-06 10:44:38.000000 fivesim-1.1.0/fivesim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-06 10:44:38.000000 fivesim-1.1.0/fivesim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2022-08-06 10:44:38.000000 fivesim-1.1.0/fivesim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-06 10:44:38.000000 fivesim-1.1.0/fivesim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      767 2022-08-06 10:43:35.000000 fivesim-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-06 10:44:38.392871 fivesim-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0       88 2022-07-31 20:51:50.000000 fivesim-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:30:52.351658 fivesim-1.2.0/
+-rw-rw-rw-   0        0        0     1092 2024-05-02 21:16:33.000000 fivesim-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5317 2024-05-02 21:30:52.349657 fivesim-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3276 2024-05-02 21:16:33.000000 fivesim-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 21:30:52.328618 fivesim-1.2.0/fivesim/
+-rw-rw-rw-   0        0        0      640 2024-05-02 21:16:33.000000 fivesim-1.2.0/fivesim/__init__.py
+-rw-rw-rw-   0        0        0    16043 2024-05-02 21:16:33.000000 fivesim-1.2.0/fivesim/api.py
+-rw-rw-rw-   0        0        0    21641 2024-05-02 21:16:33.000000 fivesim-1.2.0/fivesim/enums.py
+-rw-rw-rw-   0        0        0     1819 2024-05-02 21:16:33.000000 fivesim-1.2.0/fivesim/errors.py
+-rw-rw-rw-   0        0        0      384 2024-05-02 21:16:33.000000 fivesim-1.2.0/fivesim/fivesim.py
+-rw-rw-rw-   0        0        0     7227 2024-05-02 21:16:33.000000 fivesim-1.2.0/fivesim/json_response.py
+-rw-rw-rw-   0        0        0        0 2024-05-02 21:16:33.000000 fivesim-1.2.0/fivesim/py.typed
+-rw-rw-rw-   0        0        0     3696 2024-05-02 21:16:33.000000 fivesim-1.2.0/fivesim/request.py
+-rw-rw-rw-   0        0        0     2229 2024-05-02 21:16:33.000000 fivesim-1.2.0/fivesim/response.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:30:52.348650 fivesim-1.2.0/fivesim.egg-info/
+-rw-rw-rw-   0        0        0     5317 2024-05-02 21:30:52.000000 fivesim-1.2.0/fivesim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-05-02 21:30:52.000000 fivesim-1.2.0/fivesim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 21:30:52.000000 fivesim-1.2.0/fivesim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-02 21:30:52.000000 fivesim-1.2.0/fivesim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 21:30:52.000000 fivesim-1.2.0/fivesim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      767 2024-05-02 21:30:02.000000 fivesim-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 21:30:52.351658 fivesim-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       88 2024-05-02 21:16:33.000000 fivesim-1.2.0/setup.py
```

### Comparing `fivesim-1.1.0/LICENSE` & `fivesim-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fivesim-1.1.0/PKG-INFO` & `fivesim-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fivesim
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python API client for 5sim.net
 Author: Erik Pellizzon
 Author-email: erikpellizzon@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Erik Pellizzon
         
@@ -34,14 +34,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dateutil
+Requires-Dist: requests
 
 # 5sim
 At the moment this is the most advanced FiveSim API library, and tries to map responses to Python objects as much as possible.
 
 This library is unofficial and is not directly linked to the website in question.
 
 It was created out of need to use their API easily, without having to handle all possible cases in the application.
@@ -62,29 +64,28 @@
 - Use foreign virtual numbers from more than 180 countries all over the world. Practically you can find mobile numbers for registration of almost any country, including the UK, Russia, Sweden, Germany, Ukraine, France, India, Indonesia, Malaysia, Cambodia, Mongolia, Nicaragua, Canada, the USA, Thailand, the Philippines, Ethiopia and others.
 - Top up the balance with a minimum commission on the website (Visa/MasterCard/MIR, Alipay, Apple Pay, Google Play, Samsung Pay and others).
 - Register accounts automatically via the API.
 
 ## Rating System
 Actual rating is displayed in account settings, tab "General".
 
-Number of points rating equals number of orders that you can create simultaneously.
-
-Initial rating for new users is 8 points.
+Initial rating for new users is 96 points.
 
 Highest possible rating is 96 points.
 
 | Action                                          | Rating (points) |
-| ----------------------------------------------- | --------------- |
+|-------------------------------------------------|-----------------|
+| Add money into account                          | +8.0            |
 | Receive sms and finish the order before timeout | +0.5            |
-| Receive sms and order finished after timeout    | +0.25           |
-| Cancel                                          | -0.125          |
-| Ban number                                      | -0.125          |
-| Timeout                                         | -0.35           |
+| Automatic completed order after timeout         | +0.4            |
+| Cancel                                          | -0.1            |
+| Ban number                                      | -0.1            |
+| Timeout                                         | -0.15           |
 
-If rating drops to zero, you will not be able order within 24 hours. After 24 hours, rating will return to initial value of 8 points.
+If rating drops to zero, you will not be able order within 24 hours. After 24 hours, rating will return to initial value of 96 points.
 
 ## Examples
 
 ### Buy a number
 ```python
 from fivesim import FiveSim, Country, Operator, FiveSimError
```

### Comparing `fivesim-1.1.0/README.md` & `fivesim-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,29 +21,28 @@
 - Use foreign virtual numbers from more than 180 countries all over the world. Practically you can find mobile numbers for registration of almost any country, including the UK, Russia, Sweden, Germany, Ukraine, France, India, Indonesia, Malaysia, Cambodia, Mongolia, Nicaragua, Canada, the USA, Thailand, the Philippines, Ethiopia and others.
 - Top up the balance with a minimum commission on the website (Visa/MasterCard/MIR, Alipay, Apple Pay, Google Play, Samsung Pay and others).
 - Register accounts automatically via the API.
 
 ## Rating System
 Actual rating is displayed in account settings, tab "General".
 
-Number of points rating equals number of orders that you can create simultaneously.
-
-Initial rating for new users is 8 points.
+Initial rating for new users is 96 points.
 
 Highest possible rating is 96 points.
 
 | Action                                          | Rating (points) |
-| ----------------------------------------------- | --------------- |
+|-------------------------------------------------|-----------------|
+| Add money into account                          | +8.0            |
 | Receive sms and finish the order before timeout | +0.5            |
-| Receive sms and order finished after timeout    | +0.25           |
-| Cancel                                          | -0.125          |
-| Ban number                                      | -0.125          |
-| Timeout                                         | -0.35           |
+| Automatic completed order after timeout         | +0.4            |
+| Cancel                                          | -0.1            |
+| Ban number                                      | -0.1            |
+| Timeout                                         | -0.15           |
 
-If rating drops to zero, you will not be able order within 24 hours. After 24 hours, rating will return to initial value of 8 points.
+If rating drops to zero, you will not be able order within 24 hours. After 24 hours, rating will return to initial value of 96 points.
 
 ## Examples
 
 ### Buy a number
 ```python
 from fivesim import FiveSim, Country, Operator, FiveSimError
```

### Comparing `fivesim-1.1.0/fivesim/__init__.py` & `fivesim-1.2.0/fivesim/__init__.py`

 * *Files identical despite different names*

### Comparing `fivesim-1.1.0/fivesim/api.py` & `fivesim-1.2.0/fivesim/api.py`

 * *Files identical despite different names*

### Comparing `fivesim-1.1.0/fivesim/enums.py` & `fivesim-1.2.0/fivesim/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         try:
             return cls[status]
         except:
             return Status.INVALID
 
 
 class Language(str, Enum):
+    CHINESE = 'zh'
     ENGLISH = 'en'
     RUSSIAN = 'ru'
 
 
 class Category(str, Enum):
     HOSTING = 'hosting'
     ACTIVATION = 'activation'
@@ -75,14 +76,15 @@
     KCELL = 'kcell'
     KYIVSTAR = 'kyivstar'
     LEBARA = 'lebara'
     LYCAMOBILE = 'lycamobile'
     MATRIX = 'matrix'
     MEGAFON = 'megafon'
     MTS = 'mts'
+    O2 = 'o2'
     ORANGE = 'orange'
     PILDYK = 'pildyk'
     PLAY = 'play'
     REDBULLMOBILE = 'redbullmobile'
     ROSTELECOM = 'rostelecom'
     SYMA = 'syma'
     SMART = 'smart'
@@ -114,14 +116,28 @@
     VIRTUAL26 = 'virtual26'
     VIRTUAL27 = 'virtual27'
     VIRTUAL28 = 'virtual28'
     VIRTUAL29 = 'virtual29'
     VIRTUAL30 = 'virtual30'
     VIRTUAL31 = 'virtual31'
     VIRTUAL32 = 'virtual32'
+    VIRTUAL33 = 'virtual33'
+    VIRTUAL34 = 'virtual34'
+    VIRTUAL35 = 'virtual35'
+    VIRTUAL36 = 'virtual36'
+    VIRTUAL37 = 'virtual37'
+    VIRTUAL38 = 'virtual38'
+    VIRTUAL40 = 'virtual40'
+    VIRTUAL41 = 'virtual41'
+    VIRTUAL47 = 'virtual47'
+    VIRTUAL49 = 'virtual49'
+    VIRTUAL50 = 'virtual50'
+    VIRTUAL51 = 'virtual51'
+    VIRTUAL52 = 'virtual52'
+    VIRTUAL53 = 'virtual53'
     VODAFONE = 'vodafone'
     YOTA = 'yota'
     ZZ = 'zz'
 
 
 class Country(str, Enum):
     ANY_COUNTRY = 'any'
```

### Comparing `fivesim-1.1.0/fivesim/errors.py` & `fivesim-1.2.0/fivesim/errors.py`

 * *Files identical despite different names*

### Comparing `fivesim-1.1.0/fivesim/json_response.py` & `fivesim-1.2.0/fivesim/json_response.py`

 * *Files identical despite different names*

### Comparing `fivesim-1.1.0/fivesim/request.py` & `fivesim-1.2.0/fivesim/request.py`

 * *Files identical despite different names*

### Comparing `fivesim-1.1.0/fivesim/response.py` & `fivesim-1.2.0/fivesim/response.py`

 * *Files identical despite different names*

### Comparing `fivesim-1.1.0/fivesim.egg-info/PKG-INFO` & `fivesim-1.2.0/fivesim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fivesim
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python API client for 5sim.net
 Author: Erik Pellizzon
 Author-email: erikpellizzon@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Erik Pellizzon
         
@@ -34,14 +34,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dateutil
+Requires-Dist: requests
 
 # 5sim
 At the moment this is the most advanced FiveSim API library, and tries to map responses to Python objects as much as possible.
 
 This library is unofficial and is not directly linked to the website in question.
 
 It was created out of need to use their API easily, without having to handle all possible cases in the application.
@@ -62,29 +64,28 @@
 - Use foreign virtual numbers from more than 180 countries all over the world. Practically you can find mobile numbers for registration of almost any country, including the UK, Russia, Sweden, Germany, Ukraine, France, India, Indonesia, Malaysia, Cambodia, Mongolia, Nicaragua, Canada, the USA, Thailand, the Philippines, Ethiopia and others.
 - Top up the balance with a minimum commission on the website (Visa/MasterCard/MIR, Alipay, Apple Pay, Google Play, Samsung Pay and others).
 - Register accounts automatically via the API.
 
 ## Rating System
 Actual rating is displayed in account settings, tab "General".
 
-Number of points rating equals number of orders that you can create simultaneously.
-
-Initial rating for new users is 8 points.
+Initial rating for new users is 96 points.
 
 Highest possible rating is 96 points.
 
 | Action                                          | Rating (points) |
-| ----------------------------------------------- | --------------- |
+|-------------------------------------------------|-----------------|
+| Add money into account                          | +8.0            |
 | Receive sms and finish the order before timeout | +0.5            |
-| Receive sms and order finished after timeout    | +0.25           |
-| Cancel                                          | -0.125          |
-| Ban number                                      | -0.125          |
-| Timeout                                         | -0.35           |
+| Automatic completed order after timeout         | +0.4            |
+| Cancel                                          | -0.1            |
+| Ban number                                      | -0.1            |
+| Timeout                                         | -0.15           |
 
-If rating drops to zero, you will not be able order within 24 hours. After 24 hours, rating will return to initial value of 8 points.
+If rating drops to zero, you will not be able order within 24 hours. After 24 hours, rating will return to initial value of 96 points.
 
 ## Examples
 
 ### Buy a number
 ```python
 from fivesim import FiveSim, Country, Operator, FiveSimError
```

### Comparing `fivesim-1.1.0/pyproject.toml` & `fivesim-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fivesim"
-version = "1.1.0"
+version = "1.2.0"
 description = "Python API client for 5sim.net"
 readme = "README.md"
 requires-python = ">=3.6"
 license= {file = "LICENSE"}
 keywords=["number", "telephone-numbers", "5sim", "fivesim", "python-5sim"]
 authors = [
   {email = "erikpellizzon@gmail.com"},
```

