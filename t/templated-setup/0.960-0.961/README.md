# Comparing `tmp/templated_setup-0.960.tar.gz` & `tmp/templated_setup-0.961.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.960.tar", last modified: Thu May  2 09:34:34 2024, max compression
+gzip compressed data, was "templated_setup-0.961.tar", last modified: Thu May  2 09:43:36 2024, max compression
```

## Comparing `templated_setup-0.960.tar` & `templated_setup-0.961.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:34:34.735397 templated_setup-0.960/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.960/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:34:34.734431 templated_setup-0.960/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.960/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:34:34.735501 templated_setup-0.960/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.960/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:34:34.731465 templated_setup-0.960/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    16765 2024-05-02 09:34:25.000000 templated_setup-0.960/templated_setup/__init__.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:34:34.733874 templated_setup-0.960/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:34:34.000000 templated_setup-0.960/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 09:34:34.000000 templated_setup-0.960/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:34:34.000000 templated_setup-0.960/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:34:34.000000 templated_setup-0.960/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:43:36.285005 templated_setup-0.961/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.961/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:43:36.283887 templated_setup-0.961/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.961/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 09:43:36.285161 templated_setup-0.961/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.961/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:43:36.239311 templated_setup-0.961/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    17269 2024-05-02 09:43:01.000000 templated_setup-0.961/templated_setup/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 09:43:34.000000 templated_setup-0.961/templated_setup/_hardcoded_version.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 09:43:36.282462 templated_setup-0.961/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 09:43:35.000000 templated_setup-0.961/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      248 2024-05-02 09:43:35.000000 templated_setup-0.961/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 09:43:35.000000 templated_setup-0.961/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 09:43:35.000000 templated_setup-0.961/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.960/LICENCE` & `templated_setup-0.961/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.960/PKG-INFO` & `templated_setup-0.961/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.960
+Version: 0.961
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
 
-## V0.960 released on 2nd/5/2024
+## V0.961 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.960/README.md` & `templated_setup-0.961/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.960/templated_setup/__init__.py` & `templated_setup-0.961/templated_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -631,16 +631,20 @@
 	#################
 
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
+		# NOTE: If we do not hardcode the version, then pip will throw a fit when trying to install the 
+		# NOTE:   `templated-setup` package.
+		from . import _hardcoded_version
+
 		setup(
-			name=name,
+			name=_hardcoded_version.__version__, #type:ignore
 			version="0.960"
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
 
@@ -662,18 +666,24 @@
 		print(f"Current Directory: [{os.path.abspath(os.getcwd())}].\n\n")
 		is_root_of_project = _Setup_Helper.__get_y_n("Is this the root of the project?")
 		_Setup_Helper.__clear_screen()
 
 		if not is_root_of_project:
 			raise Exception("This script must be run from the root of the project directory.")
 		
+		egg_infos = []
+		for p, dirs, __ in os.walk(os.getcwd()):
+			for d in dirs:
+				if d.endswith(".egg-info"):
+					egg_infos.append(os.path.join(p, d))
+
 		dirs_to_remove = [
 			"dist",
 			"build",
-			f"{cls._name}.egg-info"
+			*egg_infos
 		]
 
 		if not cls._is_using_pip:
 			try:
 				for d in dirs_to_remove:
 					if os.path.exists(d):
 						print(f"\n] WARNING: ABOUT TO REMOVE THE `{os.path.join(os.getcwd(),d)}` DIRECTORY!!")
@@ -688,14 +698,18 @@
 		cls._old_sys_argv = sys.argv
 		sys.argv = [sys.argv[0], "sdist"]
 		do_proceed = _Setup_Helper.__get_y_n("Would you like to proceed with the build?")
 		if not do_proceed:
 			exit(0)
 		_Setup_Helper.__clear_screen()
 
+		from . import _hardcoded_version
+		with open(_hardcoded_version.__file__, "w") as f:
+			f.write(f"__version__ = \"{cls._version.version_number}\"")
+
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
```

### Comparing `templated_setup-0.960/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.961/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.960
+Version: 0.961
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
 
-## V0.960 released on 2nd/5/2024
+## V0.961 released on 2nd/5/2024
 god please kill me. ;(
```

