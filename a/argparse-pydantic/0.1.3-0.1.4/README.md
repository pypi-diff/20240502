# Comparing `tmp/argparse_pydantic-0.1.3.tar.gz` & `tmp/argparse_pydantic-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse_pydantic-0.1.3.tar", last modified: Tue Aug  1 11:32:23 2023, max compression
+gzip compressed data, was "argparse_pydantic-0.1.4.tar", last modified: Thu May  2 09:05:12 2024, max compression
```

## Comparing `argparse_pydantic-0.1.3.tar` & `argparse_pydantic-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-08-01 11:32:23.144056 argparse_pydantic-0.1.3/
--rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/LICENSE
--rw-rw-r--   0 aya       (1000) aya       (1000)     4308 2023-08-01 11:32:23.144056 argparse_pydantic-0.1.3/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)     3601 2023-08-01 11:30:08.000000 argparse_pydantic-0.1.3/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      833 2023-08-01 11:32:23.144056 argparse_pydantic-0.1.3/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-08-01 11:32:23.136056 argparse_pydantic-0.1.3/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-08-01 11:32:23.140056 argparse_pydantic-0.1.3/src/argparse_pydantic/
--rw-rw-r--   0 aya       (1000) aya       (1000)      139 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/src/argparse_pydantic/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     5900 2023-07-31 14:58:01.000000 argparse_pydantic-0.1.3/src/argparse_pydantic/core.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1284 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/src/argparse_pydantic/helpers.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3240 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/src/argparse_pydantic/test_tools.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-08-01 11:30:26.000000 argparse_pydantic-0.1.3/src/argparse_pydantic/version.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-08-01 11:32:23.140056 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/
--rw-rw-r--   0 aya       (1000) aya       (1000)     4308 2023-08-01 11:32:23.000000 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      705 2023-08-01 11:32:23.000000 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-08-01 11:32:23.000000 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       61 2023-08-01 11:32:23.000000 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       18 2023-08-01 11:32:23.000000 argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/top_level.txt
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-08-01 11:32:23.144056 argparse_pydantic-0.1.3/tests/
--rw-rw-r--   0 aya       (1000) aya       (1000)     2469 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_add_argument_action.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2170 2023-08-01 08:57:52.000000 argparse_pydantic-0.1.3/tests/test_add_argument_base.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1956 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_add_argument_flag.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4752 2023-07-31 12:31:22.000000 argparse_pydantic-0.1.3/tests/test_add_argument_json_schema_extra.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2311 2023-07-31 11:01:21.000000 argparse_pydantic-0.1.3/tests/test_add_argument_simple.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      980 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_core_base.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1199 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_create_parser.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      521 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_parse_args.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3778 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.3/tests/test_test_tools.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-05-02 09:05:12.996118 argparse_pydantic-0.1.4/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2024-02-10 10:24:04.000000 argparse_pydantic-0.1.4/LICENSE
+-rw-r--r--   0 aya       (1000) aya       (1000)     4489 2024-05-02 09:05:12.996118 argparse_pydantic-0.1.4/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3632 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      886 2024-05-02 09:05:12.996118 argparse_pydantic-0.1.4/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      596 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-05-02 09:05:12.992118 argparse_pydantic-0.1.4/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-05-02 09:05:12.996118 argparse_pydantic-0.1.4/src/argparse_pydantic/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      340 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/src/argparse_pydantic/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     7179 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/src/argparse_pydantic/app.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     7708 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/src/argparse_pydantic/core.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1285 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/src/argparse_pydantic/helpers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3240 2024-02-10 10:24:04.000000 argparse_pydantic-0.1.4/src/argparse_pydantic/test_tools.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       22 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/src/argparse_pydantic/version.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-05-02 09:05:12.996118 argparse_pydantic-0.1.4/src/argparse_pydantic.egg-info/
+-rw-r--r--   0 aya       (1000) aya       (1000)     4489 2024-05-02 09:05:12.000000 argparse_pydantic-0.1.4/src/argparse_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      782 2024-05-02 09:05:12.000000 argparse_pydantic-0.1.4/src/argparse_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2024-05-02 09:05:12.000000 argparse_pydantic-0.1.4/src/argparse_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       46 2024-05-02 09:05:12.000000 argparse_pydantic-0.1.4/src/argparse_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       18 2024-05-02 09:05:12.000000 argparse_pydantic-0.1.4/src/argparse_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-05-02 09:05:12.996118 argparse_pydantic-0.1.4/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2469 2024-02-10 10:36:16.000000 argparse_pydantic-0.1.4/tests/test_add_argument_action.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2171 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/tests/test_add_argument_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1956 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/tests/test_add_argument_flag.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4752 2024-02-10 10:36:16.000000 argparse_pydantic-0.1.4/tests/test_add_argument_json_schema_extra.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2311 2024-02-10 10:36:16.000000 argparse_pydantic-0.1.4/tests/test_add_argument_simple.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4599 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/tests/test_add_models.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      981 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/tests/test_core_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1199 2024-02-10 10:36:16.000000 argparse_pydantic-0.1.4/tests/test_create_parser.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      356 2024-05-02 09:04:28.000000 argparse_pydantic-0.1.4/tests/test_examples.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      521 2024-02-10 10:24:04.000000 argparse_pydantic-0.1.4/tests/test_parse_args.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3778 2024-02-10 10:36:16.000000 argparse_pydantic-0.1.4/tests/test_test_tools.py
```

### Comparing `argparse_pydantic-0.1.3/LICENSE` & `argparse_pydantic-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.3/PKG-INFO` & `argparse_pydantic-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: argparse_pydantic
-Version: 0.1.3
+Version: 0.1.4
 Summary: argparse config with pydantic model.
 Home-page: https://github.com/ayasyrev/argparse_pydantic
 Author: Yasyrev Andrei
 Author-email: a.yasyrev@gmail.com
 License: apache2
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: pydantic
+Provides-Extra: test
+Requires-Dist: cli-result; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 # Argparse Pydantic
 
 Config for argparse with pydantic model.
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/argparse_pydantic)](https://pypi.org/project/argparse_pydantic/)
-![PyPI](https://img.shields.io/pypi/v/argparse_pydantic?color=blue)  
-[![Tests](https://github.com/ayasyrev/argparse_pydantic/workflows/Tests/badge.svg)](https://github.com/ayasyrev/argparse_pydantic/actions?workflow=Tests)  [![Codecov](https://codecov.io/gh/ayasyrev/argparse_pydantic/branch/main/graph/badge.svg)](https://codecov.io/gh/ayasyrev/argparse_pydantic)  
+[![PyPI version](https://img.shields.io/pypi/v/argparse_pydantic?color=blue)](https://pypi.org/project/argparse_pydantic/)
+[![Tests](https://github.com/ayasyrev/argparse_pydantic/workflows/Tests/badge.svg)](https://github.com/ayasyrev/argparse_pydantic/actions?workflow=Tests)  [![Codecov](https://codecov.io/gh/ayasyrev/argparse_pydantic/branch/main/graph/badge.svg)](https://codecov.io/gh/ayasyrev/argparse_pydantic)
 
-Simple wrapper for python argparse.  
-Use pydantic model for you app config.  
+Simple wrapper for python argparse.
+Use pydantic model for you app config.
 It gives you typed config instead of default Namespace from argparse.
 
-Tested on python 3.7 - 3.11
+Tested on python 3.8 - 3.12
 
 WIP
 
 ## Install
 
-Install from pypi:  
+Install from pypi:
 
 `pip install argparse_pydantic`
 
 Or install from github repo:
 
 `pip install git+https://github.com/ayasyrev/argparse_pydantic.git`
 
 ## Base use.
 
-We use python argparse to parse arguments from command line.  
+We use python argparse to parse arguments from command line.
 So, just create parser as usual:
 
 
 ```python
 import argparse
 
 parser = argparse.ArgumentParser(prog="MyApp")
@@ -74,15 +78,15 @@
 from argparse_pydantic import add_args_from_model
 
 parser = add_args_from_model(parser, AppCfg)
 ```
 
 So we got parser with arguments from config.
 
-It exactly like parser made classic way:  
+It exactly like parser made classic way:
 `parser.add_argument("echo")`
 
 Now we can use parser in you script usual way - `parser.parse_args()`
 
 <!-- termynal -->
 ```
 $ python my_app.py -h
@@ -98,15 +102,15 @@
 Parse command line as usual.
 
 
 ```python
 args = parser.parse_args(["argument from command line"])
 ```
 
-When we parse command line, we got Namespace object.  
+When we parse command line, we got Namespace object.
 Bat we can convert it to config object.
 
 
 ```python
 from argparse_pydantic import create_model_obj
 
 cfg = create_model_obj(AppCfg, args)
@@ -114,25 +118,25 @@
 
 Now we got  config with type checks / validation ont type hinting when use it at IDE.
 
 
 ```python
 cfg
 ```
-<details open> <summary>output</summary>  
+<details open> <summary>output</summary>
     <pre>AppCfg(echo='argument from command line')</pre>
 </details>
 
 
 
 
 ```python
 cfg.echo
 ```
-<details open> <summary>output</summary>  
+<details open> <summary>output</summary>
     <pre>'argument from command line'</pre>
 </details>
 
 
 
 ### Optional if undefined.
 
@@ -160,15 +164,15 @@
   -h, --help            show this help message and exit
   --arg_int ARG_INT
   --arg_float ARG_FLOAT
 ```
 
 ### Add types and defaults values.
 
-And we can add type hints to help message from our config.  
+And we can add type hints to help message from our config.
 
 
 
 ```python
 parser = argparse.ArgumentParser(prog="MyApp")
 parser = add_args_from_model(
     parser,
@@ -188,8 +192,8 @@
   --arg_int ARG_INT     [int]
   --arg_float ARG_FLOAT
                         [float] default: 0.1
 ```
 
 ## Examples
 
-You can see examples at `examples` folder - Same examples as at python docs and tutorial for argparse.  
+You can see examples at `examples` folder - Same examples as at python docs and tutorial for argparse.
```

### Comparing `argparse_pydantic-0.1.3/README.md` & `argparse_pydantic-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # Argparse Pydantic
 
 Config for argparse with pydantic model.
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/argparse_pydantic)](https://pypi.org/project/argparse_pydantic/)
-![PyPI](https://img.shields.io/pypi/v/argparse_pydantic?color=blue)  
-[![Tests](https://github.com/ayasyrev/argparse_pydantic/workflows/Tests/badge.svg)](https://github.com/ayasyrev/argparse_pydantic/actions?workflow=Tests)  [![Codecov](https://codecov.io/gh/ayasyrev/argparse_pydantic/branch/main/graph/badge.svg)](https://codecov.io/gh/ayasyrev/argparse_pydantic)  
+[![PyPI version](https://img.shields.io/pypi/v/argparse_pydantic?color=blue)](https://pypi.org/project/argparse_pydantic/)
+[![Tests](https://github.com/ayasyrev/argparse_pydantic/workflows/Tests/badge.svg)](https://github.com/ayasyrev/argparse_pydantic/actions?workflow=Tests)  [![Codecov](https://codecov.io/gh/ayasyrev/argparse_pydantic/branch/main/graph/badge.svg)](https://codecov.io/gh/ayasyrev/argparse_pydantic)
 
-Simple wrapper for python argparse.  
-Use pydantic model for you app config.  
+Simple wrapper for python argparse.
+Use pydantic model for you app config.
 It gives you typed config instead of default Namespace from argparse.
 
-Tested on python 3.7 - 3.11
+Tested on python 3.8 - 3.12
 
 WIP
 
 ## Install
 
-Install from pypi:  
+Install from pypi:
 
 `pip install argparse_pydantic`
 
 Or install from github repo:
 
 `pip install git+https://github.com/ayasyrev/argparse_pydantic.git`
 
 ## Base use.
 
-We use python argparse to parse arguments from command line.  
+We use python argparse to parse arguments from command line.
 So, just create parser as usual:
 
 
 ```python
 import argparse
 
 parser = argparse.ArgumentParser(prog="MyApp")
@@ -54,15 +54,15 @@
 from argparse_pydantic import add_args_from_model
 
 parser = add_args_from_model(parser, AppCfg)
 ```
 
 So we got parser with arguments from config.
 
-It exactly like parser made classic way:  
+It exactly like parser made classic way:
 `parser.add_argument("echo")`
 
 Now we can use parser in you script usual way - `parser.parse_args()`
 
 <!-- termynal -->
 ```
 $ python my_app.py -h
@@ -78,15 +78,15 @@
 Parse command line as usual.
 
 
 ```python
 args = parser.parse_args(["argument from command line"])
 ```
 
-When we parse command line, we got Namespace object.  
+When we parse command line, we got Namespace object.
 Bat we can convert it to config object.
 
 
 ```python
 from argparse_pydantic import create_model_obj
 
 cfg = create_model_obj(AppCfg, args)
@@ -94,25 +94,25 @@
 
 Now we got  config with type checks / validation ont type hinting when use it at IDE.
 
 
 ```python
 cfg
 ```
-<details open> <summary>output</summary>  
+<details open> <summary>output</summary>
     <pre>AppCfg(echo='argument from command line')</pre>
 </details>
 
 
 
 
 ```python
 cfg.echo
 ```
-<details open> <summary>output</summary>  
+<details open> <summary>output</summary>
     <pre>'argument from command line'</pre>
 </details>
 
 
 
 ### Optional if undefined.
 
@@ -140,15 +140,15 @@
   -h, --help            show this help message and exit
   --arg_int ARG_INT
   --arg_float ARG_FLOAT
 ```
 
 ### Add types and defaults values.
 
-And we can add type hints to help message from our config.  
+And we can add type hints to help message from our config.
 
 
 
 ```python
 parser = argparse.ArgumentParser(prog="MyApp")
 parser = add_args_from_model(
     parser,
@@ -168,8 +168,8 @@
   --arg_int ARG_INT     [int]
   --arg_float ARG_FLOAT
                         [float] default: 0.1
 ```
 
 ## Examples
 
-You can see examples at `examples` folder - Same examples as at python docs and tutorial for argparse.  
+You can see examples at `examples` folder - Same examples as at python docs and tutorial for argparse.
```

### Comparing `argparse_pydantic-0.1.3/setup.cfg` & `argparse_pydantic-0.1.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -5,32 +5,36 @@
 author_email = a.yasyrev@gmail.com
 description = argparse config with pydantic model.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ayasyrev/argparse_pydantic
 license = apache2
 classifiers = 
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 where = src
 exclude = 
 	tests*
 	Nbs*
 	docs*
 
+[coverage:paths]
+source = 
+	src/argparse_pydantic/
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `argparse_pydantic-0.1.3/src/argparse_pydantic/helpers.py` & `argparse_pydantic-0.1.4/src/argparse_pydantic/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pydantic import BaseModel, ConfigDict, Field
 
 
 class ArgumentParserCfg(BaseModel):
     """Config schema for argparse parser.
     Parameters same as at argparse.ArgumentParser.
     """
+
     prog: Optional[str] = None
     usage: Optional[str] = None
     description: Optional[str] = None
     epilog: Optional[str] = None
     parents: Sequence[argparse.ArgumentParser] = Field(default_factory=list)
     formatter_class: Type[argparse.HelpFormatter] = argparse.HelpFormatter
     prefix_chars: str = "-"
```

### Comparing `argparse_pydantic-0.1.3/src/argparse_pydantic/test_tools.py` & `argparse_pydantic-0.1.4/src/argparse_pydantic/test_tools.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/PKG-INFO` & `argparse_pydantic-0.1.4/src/argparse_pydantic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
-Name: argparse-pydantic
-Version: 0.1.3
+Name: argparse_pydantic
+Version: 0.1.4
 Summary: argparse config with pydantic model.
 Home-page: https://github.com/ayasyrev/argparse_pydantic
 Author: Yasyrev Andrei
 Author-email: a.yasyrev@gmail.com
 License: apache2
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: pydantic
+Provides-Extra: test
+Requires-Dist: cli-result; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 # Argparse Pydantic
 
 Config for argparse with pydantic model.
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/argparse_pydantic)](https://pypi.org/project/argparse_pydantic/)
-![PyPI](https://img.shields.io/pypi/v/argparse_pydantic?color=blue)  
-[![Tests](https://github.com/ayasyrev/argparse_pydantic/workflows/Tests/badge.svg)](https://github.com/ayasyrev/argparse_pydantic/actions?workflow=Tests)  [![Codecov](https://codecov.io/gh/ayasyrev/argparse_pydantic/branch/main/graph/badge.svg)](https://codecov.io/gh/ayasyrev/argparse_pydantic)  
+[![PyPI version](https://img.shields.io/pypi/v/argparse_pydantic?color=blue)](https://pypi.org/project/argparse_pydantic/)
+[![Tests](https://github.com/ayasyrev/argparse_pydantic/workflows/Tests/badge.svg)](https://github.com/ayasyrev/argparse_pydantic/actions?workflow=Tests)  [![Codecov](https://codecov.io/gh/ayasyrev/argparse_pydantic/branch/main/graph/badge.svg)](https://codecov.io/gh/ayasyrev/argparse_pydantic)
 
-Simple wrapper for python argparse.  
-Use pydantic model for you app config.  
+Simple wrapper for python argparse.
+Use pydantic model for you app config.
 It gives you typed config instead of default Namespace from argparse.
 
-Tested on python 3.7 - 3.11
+Tested on python 3.8 - 3.12
 
 WIP
 
 ## Install
 
-Install from pypi:  
+Install from pypi:
 
 `pip install argparse_pydantic`
 
 Or install from github repo:
 
 `pip install git+https://github.com/ayasyrev/argparse_pydantic.git`
 
 ## Base use.
 
-We use python argparse to parse arguments from command line.  
+We use python argparse to parse arguments from command line.
 So, just create parser as usual:
 
 
 ```python
 import argparse
 
 parser = argparse.ArgumentParser(prog="MyApp")
@@ -74,15 +78,15 @@
 from argparse_pydantic import add_args_from_model
 
 parser = add_args_from_model(parser, AppCfg)
 ```
 
 So we got parser with arguments from config.
 
-It exactly like parser made classic way:  
+It exactly like parser made classic way:
 `parser.add_argument("echo")`
 
 Now we can use parser in you script usual way - `parser.parse_args()`
 
 <!-- termynal -->
 ```
 $ python my_app.py -h
@@ -98,15 +102,15 @@
 Parse command line as usual.
 
 
 ```python
 args = parser.parse_args(["argument from command line"])
 ```
 
-When we parse command line, we got Namespace object.  
+When we parse command line, we got Namespace object.
 Bat we can convert it to config object.
 
 
 ```python
 from argparse_pydantic import create_model_obj
 
 cfg = create_model_obj(AppCfg, args)
@@ -114,25 +118,25 @@
 
 Now we got  config with type checks / validation ont type hinting when use it at IDE.
 
 
 ```python
 cfg
 ```
-<details open> <summary>output</summary>  
+<details open> <summary>output</summary>
     <pre>AppCfg(echo='argument from command line')</pre>
 </details>
 
 
 
 
 ```python
 cfg.echo
 ```
-<details open> <summary>output</summary>  
+<details open> <summary>output</summary>
     <pre>'argument from command line'</pre>
 </details>
 
 
 
 ### Optional if undefined.
 
@@ -160,15 +164,15 @@
   -h, --help            show this help message and exit
   --arg_int ARG_INT
   --arg_float ARG_FLOAT
 ```
 
 ### Add types and defaults values.
 
-And we can add type hints to help message from our config.  
+And we can add type hints to help message from our config.
 
 
 
 ```python
 parser = argparse.ArgumentParser(prog="MyApp")
 parser = add_args_from_model(
     parser,
@@ -188,8 +192,8 @@
   --arg_int ARG_INT     [int]
   --arg_float ARG_FLOAT
                         [float] default: 0.1
 ```
 
 ## Examples
 
-You can see examples at `examples` folder - Same examples as at python docs and tutorial for argparse.  
+You can see examples at `examples` folder - Same examples as at python docs and tutorial for argparse.
```

### Comparing `argparse_pydantic-0.1.3/src/argparse_pydantic.egg-info/SOURCES.txt` & `argparse_pydantic-0.1.4/src/argparse_pydantic.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/argparse_pydantic/__init__.py
+src/argparse_pydantic/app.py
 src/argparse_pydantic/core.py
 src/argparse_pydantic/helpers.py
 src/argparse_pydantic/test_tools.py
 src/argparse_pydantic/version.py
 src/argparse_pydantic.egg-info/PKG-INFO
 src/argparse_pydantic.egg-info/SOURCES.txt
 src/argparse_pydantic.egg-info/dependency_links.txt
 src/argparse_pydantic.egg-info/requires.txt
 src/argparse_pydantic.egg-info/top_level.txt
 tests/test_add_argument_action.py
 tests/test_add_argument_base.py
 tests/test_add_argument_flag.py
 tests/test_add_argument_json_schema_extra.py
 tests/test_add_argument_simple.py
+tests/test_add_models.py
 tests/test_core_base.py
 tests/test_create_parser.py
+tests/test_examples.py
 tests/test_parse_args.py
 tests/test_test_tools.py
```

### Comparing `argparse_pydantic-0.1.3/tests/test_add_argument_action.py` & `argparse_pydantic-0.1.4/tests/test_add_argument_action.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.3/tests/test_add_argument_base.py` & `argparse_pydantic-0.1.4/tests/test_add_argument_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     add_args_from_model(parser, Cfg2, undefined_positional=False)
 
     assert parsers_equal(parser_base, parser)
 
 
 def test_add_help_def_type():
     """test add help_def_type"""
+
     class Cfg1(BaseModel):
         arg_int: int
 
     parser = create_parser()
     add_args_from_model(parser, Cfg1, help_def_type=True)
 
     assert "positional arguments:\n  arg_int     [int]\n" in parser.format_help()
```

### Comparing `argparse_pydantic-0.1.3/tests/test_add_argument_flag.py` & `argparse_pydantic-0.1.4/tests/test_add_argument_flag.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 
 from pydantic import BaseModel, Field
 
 from argparse_pydantic.core import (
     add_args_from_model,
-    create_model_obj,
     argument_kwargs,
+    create_model_obj,
 )
 from argparse_pydantic.test_tools import (
     parsers_actions_diff,
     parsers_actions_equal,
     parsers_args_equal,
 )
```

### Comparing `argparse_pydantic-0.1.3/tests/test_add_argument_json_schema_extra.py` & `argparse_pydantic-0.1.4/tests/test_add_argument_json_schema_extra.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.3/tests/test_add_argument_simple.py` & `argparse_pydantic-0.1.4/tests/test_add_argument_simple.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.3/tests/test_core_base.py` & `argparse_pydantic-0.1.4/tests/test_core_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional
+
 from pydantic import BaseModel
 from pydantic_core import PydanticUndefined
 
 from argparse_pydantic.core import argument_kwargs, get_field_type, process_flag
 
 
 def test_argument_kwargs():
```

### Comparing `argparse_pydantic-0.1.3/tests/test_create_parser.py` & `argparse_pydantic-0.1.4/tests/test_create_parser.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.3/tests/test_parse_args.py` & `argparse_pydantic-0.1.4/tests/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.3/tests/test_test_tools.py` & `argparse_pydantic-0.1.4/tests/test_test_tools.py`

 * *Files identical despite different names*

