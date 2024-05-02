# Comparing `tmp/templated_setup-0.981.tar.gz` & `tmp/templated_setup-0.982.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.981.tar", last modified: Thu May  2 10:28:10 2024, max compression
+gzip compressed data, was "templated_setup-0.982.tar", last modified: Thu May  2 11:53:35 2024, max compression
```

## Comparing `templated_setup-0.981.tar` & `templated_setup-0.982.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:28:10.303134 templated_setup-0.981/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.981/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2542 2024-05-02 10:28:10.302629 templated_setup-0.981/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.981/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 10:28:10.303244 templated_setup-0.981/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      412 2024-05-02 10:26:21.000000 templated_setup-0.981/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:28:10.298564 templated_setup-0.981/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    18181 2024-05-02 10:26:24.000000 templated_setup-0.981/templated_setup/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)       21 2024-05-02 10:28:09.000000 templated_setup-0.981/templated_setup/_hardcoded_version.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 10:28:10.301960 templated_setup-0.981/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2542 2024-05-02 10:28:10.000000 templated_setup-0.981/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      286 2024-05-02 10:28:10.000000 templated_setup-0.981/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 10:28:10.000000 templated_setup-0.981/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       17 2024-05-02 10:28:10.000000 templated_setup-0.981/templated_setup.egg-info/requires.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 10:28:10.000000 templated_setup-0.981/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 11:53:35.493414 templated_setup-0.982/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.982/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2542 2024-05-02 11:53:35.492763 templated_setup-0.982/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.982/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 11:53:35.493578 templated_setup-0.982/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      412 2024-05-02 11:52:45.000000 templated_setup-0.982/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 11:53:35.451440 templated_setup-0.982/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    19528 2024-05-02 11:52:42.000000 templated_setup-0.982/templated_setup/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)     3306 2024-05-02 11:53:34.000000 templated_setup-0.982/templated_setup/_hardcoded.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 11:53:35.454480 templated_setup-0.982/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2542 2024-05-02 11:53:34.000000 templated_setup-0.982/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      278 2024-05-02 11:53:35.000000 templated_setup-0.982/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 11:53:34.000000 templated_setup-0.982/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       17 2024-05-02 11:53:34.000000 templated_setup-0.982/templated_setup.egg-info/requires.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 11:53:34.000000 templated_setup-0.982/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.981/LICENCE` & `templated_setup-0.982/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.981/PKG-INFO` & `templated_setup-0.982/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.981
+Version: 0.982
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 Requires-Dist: setuptools
 Requires-Dist: twine
@@ -67,9 +67,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.981 released on 2nd/5/2024
+## V0.982 released on 2nd/5/2024
 added "setuptools", "twine" to `install_requires`.
```

### Comparing `templated_setup-0.981/README.md` & `templated_setup-0.982/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.981/templated_setup/__init__.py` & `templated_setup-0.982/templated_setup/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from dataclasses import dataclass as dataclass_x_dataclass
 from json import load as json_x_load, dump as json_x_dump, loads as json_x_loads, dumps as json_x_dumps
 from datetime import date as datetime_x_date
 from time import sleep as time_x_sleep
 from typing import Callable, overload
 from setuptools import setup
+from pickle import dumps as pickle_x_dumps, loads as pickle_x_loads
+from base64 import b64decode as base64_x_b64decode
+from base64 import b64encode as base64_x_b64encode
 import shutil
 import sys
 import os
 
 
 
 
@@ -23,22 +26,21 @@
 By using this software, you, the user, acknowledge and agree that you are solely responsible for the content that is published using this tool.
 The software is provided "as is", and the developers make no representations or warranties of any kind regarding its use.
 
 You assume all responsibility and risk for the use of this software and the materials you create or publish with it.
 
 The developers shall not be liable for any claims, damages, or other liabilities arising from the use of the software or content published therein.
 
--- END OF LEGAL NOTICE --
+===================
+END OF LEGAL NOTICE
+===================
 
 NOTE: If you would like to remove this legal notice in future, simply set "_TEMPLATED_SETUP_PLEASE="STFU" as an environment variable.
 
-========================
-THANK YOU AND TAKE CARE!
-========================
-
+-- THANK YOU AND TAKE CARE! --
 """
 
 
 
 
 
 
@@ -663,19 +665,27 @@
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
 		# NOTE: If we do not hardcode the version, then pip will throw a fit when trying to install the 
 		# NOTE:   `templated-setup` package.
-		from . import _hardcoded_version
-
+		from . import _hardcoded #type:ignore
+		kwargs_for_setup_tools = base64_x_b64decode(_hardcoded.__kwargs_for_setup_tools__.encode("utf-8")) #type:ignore
+		kwargs_for_setup_tools = pickle_x_loads(kwargs_for_setup_tools)
+		long_description = base64_x_b64decode(_hardcoded.__long_description__.encode("utf-8")) #type:ignore
+		long_description = pickle_x_loads(long_description)
 		setup(
 			name=name,
-			version=_hardcoded_version.__version__, #type:ignore
+			version=_hardcoded.__version__, #type:ignore
+			author=_hardcoded.__author__, #type:ignore
+			description=_hardcoded.__description__, #type:ignore
+			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
+			long_description=long_description, #type:ignore
+			**kwargs_for_setup_tools
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
 
 
@@ -728,17 +738,25 @@
 		cls._old_sys_argv = sys.argv
 		sys.argv = [sys.argv[0], "sdist"]
 		do_proceed = _Setup_Helper.__get_y_n("Would you like to proceed with the build?")
 		if not do_proceed:
 			exit(0)
 		_Setup_Helper.__clear_screen()
 
-		from . import _hardcoded_version
-		with open(_hardcoded_version.__file__, "w") as f:
-			f.write(f"__version__ = \"{cls._version.version_number}\"")
+		from . import _hardcoded # No `type:ignore` here since this file should exists.
+		s_long_description = pickle_x_dumps(long_description)
+		s_long_description = base64_x_b64encode(s_long_description).decode("utf-8")
+		s_kwargs_for_setup_tools = pickle_x_dumps(kwargs_for_setup_tools)
+		s_kwargs_for_setup_tools = base64_x_b64encode(s_kwargs_for_setup_tools).decode("utf-8")
+		with open(_hardcoded.__file__, "w") as f:
+			f.write(f"__version__ = \"{cls._version.version_number}\"\n")
+			f.write(f"__author__ = \"{cls._author}\"\n")
+			f.write(f"__description__ = \"{cls._description}\"\n")
+			f.write(f"__long_description__ = \"\"\"{s_long_description}\"\"\"\n")
+			f.write(f"__kwargs_for_setup_tools__ = \"\"\"{s_kwargs_for_setup_tools}\"\"\"\n")
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
```

### Comparing `templated_setup-0.981/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.982/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.981
+Version: 0.982
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 Requires-Dist: setuptools
 Requires-Dist: twine
@@ -67,9 +67,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.981 released on 2nd/5/2024
+## V0.982 released on 2nd/5/2024
 added "setuptools", "twine" to `install_requires`.
```

