# Comparing `tmp/templated_setup-0.967.tar.gz` & `tmp/templated_setup-0.968.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.967.tar", last modified: Thu May  2 10:16:17 2024, max compression
+gzip compressed data, was "templated_setup-0.968.tar", last modified: Thu May  2 10:18:35 2024, max compression
```

## Comparing `templated_setup-0.967.tar` & `templated_setup-0.968.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:16:17.545325 templated_setup-0.967/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.967/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2477 2024-05-02 10:16:17.544401 templated_setup-0.967/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.967/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 10:16:17.545634 templated_setup-0.967/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.967/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:16:17.539712 templated_setup-0.967/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    18192 2024-05-02 10:15:11.000000 templated_setup-0.967/templated_setup/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 10:16:17.000000 templated_setup-0.967/templated_setup/_hardcoded_version.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:16:17.543502 templated_setup-0.967/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2477 2024-05-02 10:16:17.000000 templated_setup-0.967/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 10:16:17.000000 templated_setup-0.967/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 10:16:17.000000 templated_setup-0.967/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 10:16:17.000000 templated_setup-0.967/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:18:35.387659 templated_setup-0.968/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.968/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2477 2024-05-02 10:18:35.386885 templated_setup-0.968/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.968/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 10:18:35.387853 templated_setup-0.968/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.968/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:18:35.383158 templated_setup-0.968/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    18180 2024-05-02 10:17:46.000000 templated_setup-0.968/templated_setup/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 10:18:34.000000 templated_setup-0.968/templated_setup/_hardcoded_version.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:18:35.385816 templated_setup-0.968/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2477 2024-05-02 10:18:35.000000 templated_setup-0.968/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 10:18:35.000000 templated_setup-0.968/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 10:18:35.000000 templated_setup-0.968/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 10:18:35.000000 templated_setup-0.968/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.967/LICENCE` & `templated_setup-0.968/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.967/PKG-INFO` & `templated_setup-0.968/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.967
+Version: 0.968
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Standardized `setup.py`
@@ -65,9 +65,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.967 released on 2nd/5/2024
+## V0.968 released on 2nd/5/2024
 Almost decent working condition.
```

### Comparing `templated_setup-0.967/README.md` & `templated_setup-0.968/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.967/templated_setup/__init__.py` & `templated_setup-0.968/templated_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,17 +267,17 @@
 	def __inner_load_date(cls) -> "None":
 		assert cls._json_data is not None
 		assert not cls._is_using_pip
 		do_want_to_use_current_date = _Setup_Helper.__get_y_n("Would you like to use the current date?")
 		new = None
 		if do_want_to_use_current_date:
 
-			cls._date_of_last_modified = datetime_x_date.today()
-			cls._json_data["date"] = cls._date_of_last_modified.isoformat()
-			new = cls._date_of_last_modified.isoformat()
+			cls._date_of_last_modified = datetime_x_date.today().isoformat()
+			cls._json_data["date"] = cls._date_of_last_modified
+			new = cls._date_of_last_modified
 
 		else:
 
 			day = int(_Setup_Helper.__get_answer(
 				"What day was it last modified? ",
 				lambda x: (x.isdigit(), "Please enter a number."))
 			)
```

### Comparing `templated_setup-0.967/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.968/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.967
+Version: 0.968
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Standardized `setup.py`
@@ -65,9 +65,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.967 released on 2nd/5/2024
+## V0.968 released on 2nd/5/2024
 Almost decent working condition.
```

