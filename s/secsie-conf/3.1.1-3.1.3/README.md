# Comparing `tmp/secsie-conf-3.1.1.tar.gz` & `tmp/secsie-conf-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secsie-conf-3.1.1.tar", last modified: Mon Jan  9 00:38:34 2023, max compression
+gzip compressed data, was "secsie-conf-3.1.3.tar", last modified: Thu May  2 17:46:40 2024, max compression
```

## Comparing `secsie-conf-3.1.1.tar` & `secsie-conf-3.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:38:34.735807 secsie-conf-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-09 00:38:24.000000 secsie-conf-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-01-09 00:38:34.735807 secsie-conf-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-01-09 00:38:24.000000 secsie-conf-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:38:34.731807 secsie-conf-3.1.1/secsie/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-01-09 00:38:24.000000 secsie-conf-3.1.1/secsie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-09 00:38:24.000000 secsie-conf-3.1.1/secsie/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-01-09 00:38:24.000000 secsie-conf-3.1.1/secsie/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-01-09 00:38:24.000000 secsie-conf-3.1.1/secsie/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-01-09 00:38:24.000000 secsie-conf-3.1.1/secsie/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:38:34.735807 secsie-conf-3.1.1/secsie_conf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-01-09 00:38:34.000000 secsie-conf-3.1.1/secsie_conf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-01-09 00:38:34.000000 secsie-conf-3.1.1/secsie_conf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 00:38:34.000000 secsie-conf-3.1.1/secsie_conf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-09 00:38:34.000000 secsie-conf-3.1.1/secsie_conf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 00:38:34.735807 secsie-conf-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-09 00:38:24.000000 secsie-conf-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:46:40.396145 secsie-conf-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 17:46:33.000000 secsie-conf-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-05-02 17:46:40.396145 secsie-conf-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-05-02 17:46:33.000000 secsie-conf-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:46:40.396145 secsie-conf-3.1.3/secsie/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-02 17:46:33.000000 secsie-conf-3.1.3/secsie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-02 17:46:33.000000 secsie-conf-3.1.3/secsie/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-02 17:46:33.000000 secsie-conf-3.1.3/secsie/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-02 17:46:33.000000 secsie-conf-3.1.3/secsie/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-02 17:46:33.000000 secsie-conf-3.1.3/secsie/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:46:40.396145 secsie-conf-3.1.3/secsie_conf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-05-02 17:46:40.000000 secsie-conf-3.1.3/secsie_conf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-02 17:46:40.000000 secsie-conf-3.1.3/secsie_conf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:46:40.000000 secsie-conf-3.1.3/secsie_conf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 17:46:40.000000 secsie-conf-3.1.3/secsie_conf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:46:40.396145 secsie-conf-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-02 17:46:33.000000 secsie-conf-3.1.3/setup.py
```

### Comparing `secsie-conf-3.1.1/LICENSE` & `secsie-conf-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `secsie-conf-3.1.1/PKG-INFO` & `secsie-conf-3.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: secsie-conf
-Version: 3.1.1
+Version: 3.1.3
 Summary: A small library for parsing configuration files
 Home-page: https://github.com/noahbroyles/secsie-conf
 Author: Noah Broyles
 Author-email: noah@javamate.net
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # secsie-conf
 
 [![PyPi Deployment](https://github.com/noahbroyles/secsie-conf/actions/workflows/deploy-to-pypi.yaml/badge.svg?event=release)](https://github.com/noahbroyles/secsie-conf/actions/workflows/deploy-to-pypi.yaml)
 [![Unit Tests](https://github.com/noahbroyles/secsie-conf/actions/workflows/unit-tests.yaml/badge.svg)](https://github.com/noahbroyles/secsie-conf/actions/workflows/unit-tests.yaml)
 
 ```console
 pip3 install secsie-conf
 ```
 Secsie is a configuration language parser for Python, made for speed and beauty. Instead of writing config files in JSON (don't get me wrong, JSON is *FAR* better than a lot of other things you could use (cough cough XML)), you can save time writing your config files in `secsie`.  
 The `secsie` language format is very similar to `ini`, except just a little better. You can use `secsie-conf` to read `.ini` files into Python `dict`s. `secsie-conf` will NOT write `.ini` files however, at least at this stage.  
 
-I also wrote a version for Java, which is available at [github.com/noahbroyles/secsie-java](https://github.com/noahbroyles/secsie-java). You can use it to parse `.properties` files. Minecraft will probably adopt this in the next few months for their `server.properties` ;)  
 
 ### Advantages over JSON:
 - easier to read
 - faster and more natural to write
 - no special syntax required for strings vs ints, floats, bools, etc.
 - file size usually smaller than readable JSON
 
@@ -505,7 +506,8 @@
 
 
 ```
 You should notice 2 things: 
 1. Keys and value assignments are separated by an equals sign with a space ON BOTH SIDES! `key = value`, **NOT** `key=value`. That is ugly and lazy. This ain't minified JS, son. [They make things for that...](https://www.amazon.com/dp/B089C3TZL9)
 2. Blank values were commented out. If you disagree with that, *MAKE 'EM NULL*! `key = ` doesn't say anything.
 
+
```

### Comparing `secsie-conf-3.1.1/README.md` & `secsie-conf-3.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 ```console
 pip3 install secsie-conf
 ```
 Secsie is a configuration language parser for Python, made for speed and beauty. Instead of writing config files in JSON (don't get me wrong, JSON is *FAR* better than a lot of other things you could use (cough cough XML)), you can save time writing your config files in `secsie`.  
 The `secsie` language format is very similar to `ini`, except just a little better. You can use `secsie-conf` to read `.ini` files into Python `dict`s. `secsie-conf` will NOT write `.ini` files however, at least at this stage.  
 
-I also wrote a version for Java, which is available at [github.com/noahbroyles/secsie-java](https://github.com/noahbroyles/secsie-java). You can use it to parse `.properties` files. Minecraft will probably adopt this in the next few months for their `server.properties` ;)  
 
 ### Advantages over JSON:
 - easier to read
 - faster and more natural to write
 - no special syntax required for strings vs ints, floats, bools, etc.
 - file size usually smaller than readable JSON
 
@@ -486,8 +485,8 @@
 [ldap]
 	ldap.max_links = -1
 
 
 ```
 You should notice 2 things: 
 1. Keys and value assignments are separated by an equals sign with a space ON BOTH SIDES! `key = value`, **NOT** `key=value`. That is ugly and lazy. This ain't minified JS, son. [They make things for that...](https://www.amazon.com/dp/B089C3TZL9)
-2. Blank values were commented out. If you disagree with that, *MAKE 'EM NULL*! `key = ` doesn't say anything.
+2. Blank values were commented out. If you disagree with that, *MAKE 'EM NULL*! `key = ` doesn't say anything.
```

### Comparing `secsie-conf-3.1.1/secsie/__init__.py` & `secsie-conf-3.1.3/secsie/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Supports secsie and ini formats. Not suitable for writing .ini files, but reads them just fine.
 """
 from .exceptions import InvalidSyntax
 from .parser import parse_config, parse_config_file
 from .generator import generate_config, generate_config_file
 
 
-__version__ = '3.1.1'
+__version__ = '3.1.3'
 __author__ = 'Noah Broyles'
 __all__ = [
     'InvalidSyntax',
     'parse_config',
     'parse_config_file',
     'generate_config',
     'generate_config_file'
```

### Comparing `secsie-conf-3.1.1/secsie/generator.py` & `secsie-conf-3.1.3/secsie/generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+from os import PathLike
 from pathlib import Path
 
 
 def generate_config(conf_obj: dict) -> str:
     """
     Generate and return a valid config from an object.
     Will save the config if an output file is passed.
@@ -26,15 +29,15 @@
         elif isinstance(value, list):
             conf += f'{key} = {", ".join(value)}\n'
         conf += f"{key} = {value}\n"
 
     return conf
 
 
-def generate_config_file(conf_obj: dict, output_file: str):
+def generate_config_file(conf_obj: dict, output_file: str | PathLike):
     """
     Generate and write a config file from a dictionary of keys and values
 
     :param conf_obj: The dictionary to render into the secsie config language
     :param output_file: The file to write to
     """
     output_file = Path(output_file)
```

### Comparing `secsie-conf-3.1.1/secsie/modes.py` & `secsie-conf-3.1.3/secsie/modes.py`

 * *Files identical despite different names*

### Comparing `secsie-conf-3.1.1/secsie/parser.py` & `secsie-conf-3.1.3/secsie/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 parser.py
 
 Contains code relative to parsing configuration language.
 """
-from typing import Any
+from __future__ import annotations
 
-from secsie import InvalidSyntax
+from typing import Any
+from os import PathLike
 from secsie.modes import MODES
+from secsie import InvalidSyntax
 
 
 def _parse_value(value: str, mode: str = 'secsie') -> Any:
     """
     INTENDED FOR INTERNAL USE ONLY
 
     Determine whether a value is of a special type. If so, will convert the value to that type and return it.
@@ -97,15 +99,15 @@
             c_section = MODES[mode]["SECTION_EX"].findall(line)[0]
             continue
         conf = _write_to_conf_(conf, line, line_number=lineno, section=c_section, mode=mode)
 
     return conf
 
 
-def parse_config_file(conf_file: str, mode: str = 'secsie') -> dict:
+def parse_config_file(conf_file: str | PathLike, mode: str = 'secsie') -> dict:
     """
     Read a config file and return a dictionary of the values inside.
 
     :param conf_file: A file path to a configuration file
     :param mode: The language of the config file, 'secsie' or 'ini' are supported
     :return: The config as a dict
     """
```

### Comparing `secsie-conf-3.1.1/secsie_conf.egg-info/PKG-INFO` & `secsie-conf-3.1.3/secsie_conf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: secsie-conf
-Version: 3.1.1
+Version: 3.1.3
 Summary: A small library for parsing configuration files
 Home-page: https://github.com/noahbroyles/secsie-conf
 Author: Noah Broyles
 Author-email: noah@javamate.net
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # secsie-conf
 
 [![PyPi Deployment](https://github.com/noahbroyles/secsie-conf/actions/workflows/deploy-to-pypi.yaml/badge.svg?event=release)](https://github.com/noahbroyles/secsie-conf/actions/workflows/deploy-to-pypi.yaml)
 [![Unit Tests](https://github.com/noahbroyles/secsie-conf/actions/workflows/unit-tests.yaml/badge.svg)](https://github.com/noahbroyles/secsie-conf/actions/workflows/unit-tests.yaml)
 
 ```console
 pip3 install secsie-conf
 ```
 Secsie is a configuration language parser for Python, made for speed and beauty. Instead of writing config files in JSON (don't get me wrong, JSON is *FAR* better than a lot of other things you could use (cough cough XML)), you can save time writing your config files in `secsie`.  
 The `secsie` language format is very similar to `ini`, except just a little better. You can use `secsie-conf` to read `.ini` files into Python `dict`s. `secsie-conf` will NOT write `.ini` files however, at least at this stage.  
 
-I also wrote a version for Java, which is available at [github.com/noahbroyles/secsie-java](https://github.com/noahbroyles/secsie-java). You can use it to parse `.properties` files. Minecraft will probably adopt this in the next few months for their `server.properties` ;)  
 
 ### Advantages over JSON:
 - easier to read
 - faster and more natural to write
 - no special syntax required for strings vs ints, floats, bools, etc.
 - file size usually smaller than readable JSON
 
@@ -505,7 +506,8 @@
 
 
 ```
 You should notice 2 things: 
 1. Keys and value assignments are separated by an equals sign with a space ON BOTH SIDES! `key = value`, **NOT** `key=value`. That is ugly and lazy. This ain't minified JS, son. [They make things for that...](https://www.amazon.com/dp/B089C3TZL9)
 2. Blank values were commented out. If you disagree with that, *MAKE 'EM NULL*! `key = ` doesn't say anything.
 
+
```

### Comparing `secsie-conf-3.1.1/setup.py` & `secsie-conf-3.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,12 +20,14 @@
     author_email="noah@javamate.net",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10"
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12"
     ],
     packages=["secsie"],
     include_package_data=True
 )
```

