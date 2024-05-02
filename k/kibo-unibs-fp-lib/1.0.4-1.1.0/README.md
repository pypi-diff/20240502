# Comparing `tmp/kibo_unibs_fp_lib-1.0.4.tar.gz` & `tmp/kibo_unibs_fp_lib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kibo_unibs_fp_lib-1.0.4.tar", last modified: Fri Apr 12 13:05:58 2024, max compression
+gzip compressed data, was "kibo_unibs_fp_lib-1.1.0.tar", last modified: Thu May  2 14:05:23 2024, max compression
```

## Comparing `kibo_unibs_fp_lib-1.0.4.tar` & `kibo_unibs_fp_lib-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:05:58.345670 kibo_unibs_fp_lib-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-12 13:05:58.345670 kibo_unibs_fp_lib-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:05:58.345670 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/ansi_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/file_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/known_problems.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/pretty_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/random_draws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:05:58.345670 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-12 13:05:58.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-12 13:05:58.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:05:58.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 13:05:58.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:05:58.345670 kibo_unibs_fp_lib-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:05:23.169391 kibo_unibs_fp_lib-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-02 14:05:23.169391 kibo_unibs_fp_lib-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:05:23.169391 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/ansi_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11949 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/known_problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/pretty_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/random_draws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:05:23.169391 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-02 14:05:23.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-02 14:05:23.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:05:23.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 14:05:23.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:05:23.169391 kibo_unibs_fp_lib-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/setup.py
```

### Comparing `kibo_unibs_fp_lib-1.0.4/LICENSE.txt` & `kibo_unibs_fp_lib-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kibo_unibs_fp_lib-1.0.4/PKG-INFO` & `kibo_unibs_fp_lib-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kibo_unibs_fp_lib
-Version: 1.0.4
-Summary: UniBSFpLib modified, documented and converted in python.
+Version: 1.1.0
+Summary: KiboUniBSFpLib modified, documented and converted in python.
 Home-page: https://github.com/AlessandroMuscio/kibo_unibs_fp_lib
 Author: Alessandro Muscio
 Author-email: Alessandro Muscio <a.muscio001@studenti.unibs.it>
 License: MIT License
         
         Copyright (c) 2024 Alessandro Muscio
         
@@ -39,10 +39,22 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # kibo_unibs_fp_lib
 
-Libreria UniBSFpLib modificata e convertita in Python da me per l'utilizzo durante il Programma Arnaldo, ma non ristretta solo a questo utilizzo.
+This library is converted from its original Java counterpart tha can be found [here](https://github.com/AlessandroMuscio/KiboUniBSFpLib). For whatever problem may arise form the use of this library report it on the [github issues](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/issues) of this repository.
 
-*Questo progetto è concesso in licenza secondo i termini della licenza MIT.*
+## Installation
+
+This library is available for all on [PyPI](https://pypi.org) that means it can be installed with:
+
+```bash
+pip install kibo-unibs-fp-lib
+```
+
+## Usage
+
+For an overview of its usages consults the [wiki](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/wiki) (**WIP!!**).
+
+*This library is distributed under the MIT license, provided [here](LICENSE.txt)*
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/input_data.py` & `kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/input_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,339 +1,376 @@
 """Module for the InputData class"""
 
 # Internal Libraries
-from kibo_unibs_fp_lib.ansi_colors import AnsiColors
+from kibo_unibs_fp_lib.ansi_colors import (
+    RESET,
+    AnsiFontColors,
+    AnsiFontWeights,
+    AnsiFontDecorations,
+)
 
 
 class InputData:
     """
     This class can read a specific data type inserted in input by the user, while also allowing to
-    make controls on the data inserted.
+    make controls on the data inserted and printing errors to the user.
     """
 
-    _RED_ATTENTION = f"{AnsiColors.RED}Attention!{AnsiColors.RESET}"
-    _ALPHANUMERIC_CHARACTERS_ERROR = (
-        f"{_RED_ATTENTION}\nOnly alphanumeric characters are allowed."
+    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
+    _RED_ERROR: str = f"\n{AnsiFontColors.RED}{AnsiFontWeights.BOLD}Error!{RESET}"
+
+    _ALPHANUMERIC_CHARACTERS_ERROR: str = (
+        f"Only {AnsiFontWeights.BOLD}alphanumeric{RESET} characters are allowed.\n"
     )
-    _EMPTY_STRING_ERROR = f"{_RED_ATTENTION}\nNo characters were inserted."
-    _ALLOWED_CHARACTERS_ERROR = f"{_RED_ATTENTION}\nThe only allowed characters are: "
-    _YES_ANSWERS = "yY"
-    _NO_ANSWERS = "nN"
-    _INTEGER_FORMAT_ERROR = f"""
-    {_RED_ATTENTION}\nThe inserted data is in an incorrect format.
-    An integer is required.
-    """
-    _MINIMUM_ERROR = (
-        f"{_RED_ATTENTION}\nA value greater than or equal to %.2f is required."
+    _EMPTY_STRING_ERROR: str = (
+        f"No {AnsiFontWeights.BOLD}characters{RESET} or only \
+            {AnsiFontWeights.BOLD}whitespaces{RESET} were inserted.\n"
     )
-    _MAXIMUM_ERROR = (
-        f"{_RED_ATTENTION}\nA value less than or equal to %.2f is required."
+    _ALLOWED_CHARACTERS_ERROR: str = "The only allowed characters are: %s\n"
+    _YES_ANSWERS: str = "yY"
+    _NO_ANSWERS: str = "nN"
+    _INTEGER_FORMAT_ERROR: str = (
+        f"The inserted data is in an {AnsiFontWeights.BOLD}incorrect{RESET} format. An \
+            {AnsiFontDecorations.UNDERLINE}integer{RESET} is required.\n"
+    )
+    _MINIMUM_ERROR: str = "A value greater than or equal to %.2f is required.\n"
+    _MAXIMUM_ERROR: str = "A value less than or equal to %.2f is required.\n"
+    _FLOAT_FORMAT_ERROR: str = (
+        f"The inserted data is in an {AnsiFontWeights.BOLD}incorrect{RESET} format. A \
+            {AnsiFontDecorations.UNDERLINE}float{RESET} is required.\n"
     )
-    _FLOAT_FORMAT_ERROR = f"""
-    {_RED_ATTENTION}\nThe inserted data is in an incorrect format.
-    A float is required.
-    """
 
     def __init__(self) -> None:
-        """Prevents instantiation of this class
+        """Prevents the instantiation of this class.
 
-        Raises:
-            NotImplementedError
+        Raises
+        ------
+        - NotImplementedError
         """
-
-        raise NotImplementedError("This class isn't instantiable!")
+        raise NotImplementedError(InputData._CONSTRUCTOR_ERROR)
 
     @staticmethod
-    def read_string(message: str, alphanumeric: bool) -> str:
-        """Prints message in the terminal and reads the text inserted by the user. If it isn't a
-        string an error message is printed. It's also possible to select if the inserted text needs
-        to be alphanumeric or not via the alphanumeric input variable.
+    def read_string(message: str, alphanumeric: bool = False) -> str:
+        """Prints message in the terminal and reads the text inserted by the user. It's also
+        possible to select if the inserted text needs to be alphanumeric or not via the
+        alphanumeric variable.
 
-        Params:
-            message -> The message to print.
+        Params
+        ------
+        - message -> The message to print.
+        - alphanumeric -> If the input needs to be alphanumeric or not, defaulted to False.
 
-            alphanumeric -> If the input needs to be alphanumeric or not.
-
-        Returns:
-            A string representing the user input.
+        Returns
+        -------
+        A string representing the user input.
         """
-
         if not alphanumeric:
-            return input(message).strip()
+            return input(message)
 
-        is_alphanumeric = False
+        is_alphanumeric: bool = False
         while not is_alphanumeric:
-            read = input(message).strip()
+            read: str = input(message)
 
             is_alphanumeric = read.isalnum()
 
             if not is_alphanumeric:
+                print(InputData._RED_ERROR)
                 print(InputData._ALPHANUMERIC_CHARACTERS_ERROR)
 
         return read
 
     @staticmethod
-    def read_non_empty_string(message: str, alphanumeric: bool) -> str:
+    def read_non_empty_string(message: str, alphanumeric: bool = False) -> str:
         """Prints message in the terminal and reads the text inserted by the user, given that it
-        isn't empty. If it isn't a string an error message is printed. It's also possible to select
-        if the inserted text needs to be alphanumeric or not via the alphanumeric input variable.
-
-        Params:
-            message -> The message to print.
-
-            alphanumeric -> If the input needs to be alphanumeric or not.
+        isn't empty. It's also possible to select if the inserted text needs to be alphanumeric or
+        not via the alphanumeric variable.
 
-        Returns:
-            A string representing the user input.
+        Params
+        ------
+        - message -> The message to print.
+        - alphanumeric -> If the input needs to be alphanumeric or not.
+
+        Returns
+        -------
+        A string representing the user input.
         """
-
-        is_empty = True
+        is_empty: bool = True
 
         while is_empty:
-            read = InputData.read_string(message, alphanumeric)
+            read: str = InputData.read_string(message, alphanumeric).strip()
 
-            is_empty = not bool(read)
+            is_empty = not read
             if is_empty:
+                print(InputData._RED_ERROR)
                 print(InputData._EMPTY_STRING_ERROR)
 
         return read
 
     @staticmethod
     def read_char(message: str, allowed: str = None) -> str:
-        """Read a single character input from the user.
-
-        Params:
-            message -> The message to display to the user.
-
-            allowed (optional) -> Contains the allowed characters, defaults to None.
+        """Read a single character input from the user. It's also possible to give a list, in the
+        form of a string, of the possible allowed characters.
 
-        Returns:
-            The single character input by the user.
+        Params
+        ------
+        - message -> The message to display to the user.
+        - allowed -> Contains the allowed characters, defaulted to None.
+
+        Returns
+        -------
+        The single character input by the user.
         """
+        if not allowed:
+            return InputData.read_non_empty_string(message, False)[0]
 
         is_allowed = False
 
         while not is_allowed:
             read = InputData.read_non_empty_string(message, False)[0]
 
-            if allowed and read in allowed:
+            if read in allowed:
                 is_allowed = True
             else:
-                print(InputData._ALLOWED_CHARACTERS_ERROR, list(allowed))
+                print(InputData._RED_ERROR)
+                print(InputData._ALLOWED_CHARACTERS_ERROR % list(allowed))
 
         return read
 
     @staticmethod
     def read_yes_or_no(question: str) -> bool:
         """Prompts the user with a question and expects a yes or no response.
 
-        Params:
-            question -> The question to display the user without question mark.
-
-        Returns:
-            True if the user reponds with 'y' or 'Y', False otherwise.
+        The idea is to give the question the usual unix terminal aspects, where the question is
+        followed by square brackets and the two possible answers, the upper case one is the default
+        if no answer is given.
+
+        Params
+        ------
+        - question -> The question to display the user without question mark.
+
+        Returns
+        -------
+        True if the user respond with 'y' or 'Y', False otherwise.
         """
-
         question = (
-            f"{question}? [{InputData._YES_ANSWERS[1]}/{InputData._NO_ANSWERS[0]}]"
+            f"{question}? [{InputData._YES_ANSWERS[1]}/{InputData._NO_ANSWERS[0]}] "
         )
-        response = InputData.read_char(question)
+        response = InputData.read_string(question)
 
-        return response in InputData._YES_ANSWERS
+        if not response:
+            return True
+
+        return response[0] in InputData._YES_ANSWERS
 
     @staticmethod
     def read_integer(message: str) -> int:
         """Reads an integer input from the user.
 
-        Params:
-            message -> The message to display the user.
-
-        Returns:
-            The integer input by the user.
+        Params
+        ------
+        - message -> The message to display the user.
+
+        Returns
+        -------
+        The integer input by the user.
         """
-
-        is_integer = False
+        is_integer: bool = False
 
         while not is_integer:
             try:
-                read = int(input(message))
+                read: int = int(input(message))
                 is_integer = True
             except ValueError:
+                print(InputData._RED_ERROR)
                 print(InputData._INTEGER_FORMAT_ERROR)
 
         return read
 
     @staticmethod
     def read_integer_with_minimum(message: str, min_value: int) -> int:
         """Reads an integer input from the user with a minimum value constraint.
 
-        Params:
-            message -> The message to display the user.
-
-            min_value -> The minimum allowed value for the input.
-
-        Returns:
-            The integer input by the user that is greater than or equal to min.
+        Params
+        ------
+        - message -> The message to display the user.
+        - min_value -> The minimum allowed value for the input.
+
+        Returns
+        -------
+        The integer input by the user that is greater than or equal to min_value.
         """
+        is_input_out_of_range: bool = True
 
-        is_input_valid = False
+        while is_input_out_of_range:
+            read: int = InputData.read_integer(message)
 
-        while not is_input_valid:
-            read = InputData.read_integer(message)
             if read >= min_value:
-                is_input_valid = True
+                is_input_out_of_range = False
             else:
+                print(InputData._RED_ERROR)
                 print(InputData._MINIMUM_ERROR % min_value)
 
         return read
 
     @staticmethod
     def read_integer_with_maximum(message: str, max_value: int) -> int:
         """Reads an integer input from the user with a maximum value constraint.
 
-        Params:
-            message -> The message to display the user.
-
-            max_value -> The maximum allowed value for the input.
-
-        Returns:
-            The integer input by the user that is less than or equal to max.
+        Params
+        ------
+        - message -> The message to display the user.
+        - max_value -> The maximum allowed value for the input.
+
+        Returns
+        -------
+        The integer input by the user that is less than or equal to max_value.
         """
+        is_input_out_of_range: bool = True
 
-        is_input_valid = False
+        while is_input_out_of_range:
+            read: int = InputData.read_integer(message)
 
-        while not is_input_valid:
-            read = InputData.read_integer(message)
             if read <= max_value:
-                is_input_valid = True
+                is_input_out_of_range = False
             else:
+                print(InputData._RED_ERROR)
                 print(InputData._MAXIMUM_ERROR % max_value)
 
         return read
 
     @staticmethod
     def read_integer_between(message: str, min_value: int, max_value: int) -> int:
         """Reads an integer input from the user with a minimum and maximum value constraint.
 
-        Params:
-            message -> The message to display the user.
-
-            min_value -> The minimum allowed value for the input.
-
-            max_value -> The maximum allowed value for the input.
-
-        Returns:
-            The integer input by the user that is greater than or equal to min and less than or
-            equal to max.
+        Params
+        ------
+        - message -> The message to display the user.
+        - min_value -> The minimum allowed value for the input.
+        - max_value -> The maximum allowed value for the input.
+
+        Returns
+        -------
+        The integer input by the user that is greater than or equal to min_value and less than or
+        equal to max_value.
         """
+        is_input_out_of_range: bool = True
 
-        is_input_valid = False
+        while is_input_out_of_range:
+            read: int = InputData.read_integer(message)
 
-        while not is_input_valid:
-            read = InputData.read_integer(message)
             if read < min_value:
-                print(InputData._MINIMUM_ERROR % max_value)
+                print(InputData._RED_ERROR)
+                print(InputData._MINIMUM_ERROR % min_value)
             elif read > max_value:
+                print(InputData._RED_ERROR)
                 print(InputData._MAXIMUM_ERROR % max_value)
             else:
-                is_input_valid = True
+                is_input_out_of_range = False
 
         return read
 
     @staticmethod
     def read_float(message: str) -> float:
         """Reads a float input from the user.
 
-        Params:
-            message -> The message to display the user.
-
-        Returns:
-            The float input by the user.
+        Params
+        ------
+        - message -> The message to display the user.
+
+        Returns
+        -------
+        The float input by the user.
         """
-
-        is_float = False
+        is_float: bool = False
 
         while not is_float:
             try:
                 read = float(input(message))
                 is_float = True
             except ValueError:
+                print(InputData._RED_ERROR)
                 print(InputData._FLOAT_FORMAT_ERROR)
 
         return read
 
     @staticmethod
     def read_float_with_minimum(message: str, min_value: float) -> float:
         """Reads a float input from the user with a minimum value constraint.
 
-        Params:
-            message -> The message to display the user.
-
-            min_value -> The minimum allowed value for the input.
-
-        Returns:
-            The float input by the user that is greater than or equal to min.
+        Params
+        ------
+        - message -> The message to display the user.
+        - min_value -> The minimum allowed value for the input.
+
+        Returns
+        -------
+        The float input by the user that is greater than or equal to min_value.
         """
+        is_input_out_of_range: bool = True
 
-        is_input_valid = False
+        while is_input_out_of_range:
+            read: float = InputData.read_float(message)
 
-        while not is_input_valid:
-            read = InputData.read_float(message)
             if read >= min_value:
-                is_input_valid = True
+                is_input_out_of_range = False
             else:
+                print(InputData._RED_ERROR)
                 print(InputData._MINIMUM_ERROR % min_value)
 
         return read
 
     @staticmethod
     def read_float_with_maximum(message: str, max_value: float) -> float:
         """Reads a float input from the user with a maximum value constraint.
 
-        Params:
-            message -> The message to display the user.
-
-            max_value -> The maximum allowed value for the input.
-
-        Returns:
-            The float input by the user that is less than or equal to max.
+        Params
+        ------
+        - message -> The message to display the user.
+        - max_value -> The maximum allowed value for the input.
+
+        Returns
+        -------
+        The float input by the user that is less than or equal to max_value.
         """
+        is_input_out_of_range: bool = True
 
-        is_input_valid = False
+        while is_input_out_of_range:
+            read: float = InputData.read_float(message)
 
-        while not is_input_valid:
-            read = InputData.read_float(message)
             if read <= max_value:
-                is_input_valid = True
+                is_input_out_of_range = False
             else:
+                print(InputData._RED_ERROR)
                 print(InputData._MAXIMUM_ERROR % max_value)
 
         return read
 
     @staticmethod
     def read_float_between(message: str, min_value: float, max_value: float) -> float:
         """Reads a float input from the user with a minimum and maximum value constraint.
 
-        Params:
-            message -> The message to display the user.
-
-            min_value -> The minimum allowed value for the input.
-
-            max_value -> The maximum allowed value for the input.
-
-        Returns:
-            The float input by the user that is greater than or equal to min and less than or equal
-            to max.
+        Params
+        ------
+        - message -> The message to display the user.
+        - min_value -> The minimum allowed value for the input.
+        - max_value -> The maximum allowed value for the input.
+
+        Returns
+        -------
+        The float input by the user that is greater than or equal to min_value and less than or
+        equal to max_value.
         """
+        is_input_out_of_range: bool = True
 
-        is_input_valid = False
+        while is_input_out_of_range:
+            read: float = InputData.read_float(message)
 
-        while not is_input_valid:
-            read = InputData.read_float(message)
             if read < min_value:
-                print(InputData._MINIMUM_ERROR % max_value)
+                print(InputData._RED_ERROR)
+                print(InputData._MINIMUM_ERROR % min_value)
             elif read > max_value:
+                print(InputData._RED_ERROR)
                 print(InputData._MAXIMUM_ERROR % max_value)
             else:
-                is_input_valid = True
+                is_input_out_of_range = False
 
         return read
```

### Comparing `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/menu.py` & `kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/menu.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,93 @@
 """Module for the Menu class"""
 
 # Standard Libraries
-import os
+# import os
 import time
 
 # Internal Libraries
-from kibo_unibs_fp_lib.ansi_colors import AnsiColors
+from kibo_unibs_fp_lib.ansi_colors import AnsiFontColors
 from kibo_unibs_fp_lib.input_data import InputData
 from kibo_unibs_fp_lib.known_problems import KnownProblems
 from kibo_unibs_fp_lib.pretty_strings import PrettyStrings
 
 
 class Menu:
     """
     This class creates a menu with multiple entries, assuming that zero is always the exit option.
     The class also contains some methods that may be useful for visualizing the menu.
     """
 
     _NEW_LINE = "\n"
     _EXIT_ENTRY = "0. Exit"
     _INSERT_REQUEST = "> "
-    _NEGATIVE_MILLIS_ERROR = (
-        f"{AnsiColors.RED}Attention!{AnsiColors.RESET}\nYou can't have negative time."
-    )
+    _NEGATIVE_MILLIS_ERROR = "Impossible to wait for a negative time."
 
     def __init__(
         self,
         title: str,
         entries: list[str],
         use_exit_entry: bool,
         centred_title: bool,
     ) -> None:
-        """Constructor that creates a Menu object specifying a title, the entries of the menu, if
-        you want the exit entry or not, if you want the title centred, and the vertical frame will
-        be off by default. It will also automatically calculate the frame length.
+        """Creates a Menu object specifying some configuration parameters.
 
-        Params:
-            title -> Represents the title of the menu.
-
-            entries -> Represents the entries of the menu.
-
-            use_exit_entry -> If you want the exit entry or not.
-
-            centred_title -> If you want the title to be centred or not.
-
-            use_vertical_frame -> If you want to use the vertical frame or not.
+        Params
+        ------
+        - title -> The title of the menu.
+        - entries -> The entries, options, of the menu.
+        - use_exit_entry -> If you want the exit entry or not.
+        - centred_title -> If you want the title to be centred or not.
         """
-
         self._title = title
         self._entries = entries
         self._use_exit_entry = use_exit_entry
         self._frame_length = self._calculate_frame_length()
         self._centred_title = centred_title
         self._use_vertical_frame = False
 
     @property
     def use_vertical_frame(self) -> bool:
-        """Getter of attribute use_vertical_frame.
+        """Gets the value of the use_vertical_frame attribute.
 
-        Returns:
-            A bool representing the current value of use_vertical_frame.
+        Returns
+        -------
+        A bool representing the attribute value.
         """
-
         return self._use_vertical_frame
 
     @use_vertical_frame.setter
     def use_vertical_frame(self, value: bool) -> None:
-        """Setter of attribute use_vertical_frame.
+        """Sets the value of the use_vertical_frame attribute.
 
-        Params:
-            value -> The new value of use_vertical_frame.
+        Params
+        ------
+        - value -> The value to set the attribute to.
         """
-
         self._use_vertical_frame = value
 
     def _calculate_frame_length(self) -> int:
         """Calculates the frame length by measuring the length of the title and of all the entries
         of the menu, accounting for their number and the ". " string before the actual entry.
 
-        Params:
-            title -> The title of the menu.
-
-            entries -> The entries of the menu.
-
-        Returns:
-            An integer representing the length of the frame.
+        Returns
+        -------
+        An integer representing the length of the frame.
         """
-
         frame_length = len(self._title)
 
         for i, entry in enumerate(self._entries):
             frame_length = max(
                 frame_length, len(entry) + KnownProblems.count_integer_digits(i + 1) + 2
             )
 
         return frame_length + 10  # Adding a bit of extra space
 
     def _print_menu(self) -> None:
-        """
-        Prints the menu: first the framed title and then all the entries.
-        """
-
+        """Prints the menu, the framed title, followed by all the entries."""
         menu = []
 
         menu.append(
             PrettyStrings.frame(
                 self._title,
                 self._frame_length,
                 self._centred_title,
@@ -121,58 +104,61 @@
             menu.append(PrettyStrings.isolated_line(self._EXIT_ENTRY))
 
         print("".join(menu))
 
     def choose(self) -> int:
         """Prints the menu and lets the user choose an option from it.
 
-        Returns:
-            An integer representing the choice of the user.
+        Returns
+        -------
+        An integer representing the choice of the user.
         """
-
         self._print_menu()
 
         if self._use_exit_entry:
             min_value = 0
         else:
             min_value = 1
 
         return InputData.read_integer_between(
             self._INSERT_REQUEST, min_value, len(self._entries)
         )
 
     @staticmethod
     def clear_console() -> None:
-        """
-        Clear the console screen.
-        """
-
-        os.system("cls" if os.name == "nt" else "clear")
+        """Clears the console screen."""
+        # os.system("cls" if os.name == "nt" else "clear")
+        print(AnsiFontColors.CLEAR)
 
     @staticmethod
     def wait(milliseconds: int) -> None:
         """Stops the program for a certain amount of milliseconds.
 
-        Params:
-            milliseconds -> The number of milliseconds to stop the program.
+        Params
+        ------
+        - milliseconds -> The number of milliseconds to stop the program.
+
+        Raises
+        ------
+        - ValueError -> When the milliseconds are negative.
         """
-
         if milliseconds < 0:
-            print(Menu._NEGATIVE_MILLIS_ERROR)
-            return
+            raise ValueError(Menu._NEGATIVE_MILLIS_ERROR)
 
         time.sleep(milliseconds / 1000)
 
     @staticmethod
     def loading_message(message: str) -> None:
-        """Prints a certain message simulating a loading by adding dots slowly.
+        """Prints a certain message simulating a loading by adding dots to it slowly.
 
-        Params:
-            message -> The message to print.
+        Params
+        ------
+        - message -> The message to print.
         """
 
         print(message, end="", flush=True)
         for _ in range(3):
             Menu.wait(1000)
             print(".", end="", flush=True)
 
+        Menu.wait(1000)
         Menu.clear_console()
```

### Comparing `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/pretty_strings.py` & `kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/pretty_strings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,155 +1,187 @@
 """Module for the PrettyStrings class"""
 
 
 class PrettyStrings:
-    """
-    This class contains various methods to better print strings to the terminal.
-    """
+    """This class contains various methods to prettify print strings to the terminal."""
 
+    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
     _SPACE = " "
     _HORIZONTAL_FRAME = "-"
     _VERTICAL_FRAME = "|"
     _NEW_LINE = "\n"
 
     def __init__(self) -> None:
-        """Prevents instantiation of this class
+        """Prevents the instantiation of this class.
 
-        Raises:
-            NotImplementedError
+        Raises
+        ------
+        - NotImplementedError
         """
-
-        raise NotImplementedError("This class isn't instantiable!")
+        raise NotImplementedError(PrettyStrings._CONSTRUCTOR_ERROR)
 
     @staticmethod
     def frame(
         to_frame: str, frame_length: int, centered: bool, vertical_frame: bool
     ) -> str:
         """Puts the given string in the center or in the beginning of the line surrounded by the
         horizontal frame above and below and, if needed, also the vertical frame before and after.
         It's required to specify a frame length for the horizontal frame.
 
-        Params:
-            to_frame -> The string to put in the frame
-
-            frame_length -> The length of the horizontal frame.
-
-            centered -> If the string needs to be centered or not.
-
-            vertical_frame -> If the vertical frame is needed or not.
-
-        Returns:
-            A string containing the framed original string.
-        """
-
-        framed = []
-
-        framed.append(
-            PrettyStrings.repeat_char(PrettyStrings._HORIZONTAL_FRAME, frame_length)
-            + PrettyStrings._NEW_LINE
+        Params
+        ------
+        - to_frame -> The string to put in the frame
+        - frame_length -> The length of the horizontal frame.
+        - centered -> If the string needs to be centered or not.
+        - vertical_frame -> If the vertical frame is needed or not.
+
+        Returns
+        -------
+        A string containing the framed original string.
+        """
+        framed: list[str] = []
+        horizontal_frame: list[str] = "".join(
+            [
+                PrettyStrings.repeat_char(
+                    PrettyStrings._HORIZONTAL_FRAME, frame_length
+                ),
+                PrettyStrings._NEW_LINE,
+            ]
         )
 
+        framed.append(horizontal_frame)
+
         if vertical_frame:
             framed.append(PrettyStrings._VERTICAL_FRAME)
 
+        to_append: str
         if centered:
-            framed.append(
+            to_append = (
                 PrettyStrings.center(to_frame, frame_length - 2)
                 if vertical_frame
-                else PrettyStrings.center(to_frame, frame_length)
-                + PrettyStrings._NEW_LINE
+                else "".join(
+                    [
+                        PrettyStrings.center(to_frame, frame_length),
+                        PrettyStrings._NEW_LINE,
+                    ]
+                )
             )
         else:
-            framed.append(
+            to_append = (
                 PrettyStrings.column(to_frame, frame_length - 2)
                 if vertical_frame
-                else PrettyStrings.column(to_frame, frame_length)
-                + PrettyStrings._NEW_LINE
+                else "".join(
+                    [
+                        PrettyStrings.column(to_frame, frame_length),
+                        PrettyStrings._NEW_LINE,
+                    ]
+                )
             )
+        framed.append(to_append)
 
         if vertical_frame:
-            framed.append(PrettyStrings._VERTICAL_FRAME + PrettyStrings._NEW_LINE)
+            framed.append(
+                "".join([PrettyStrings._VERTICAL_FRAME, PrettyStrings._NEW_LINE])
+            )
 
-        framed.append(
-            PrettyStrings.repeat_char(PrettyStrings._HORIZONTAL_FRAME, frame_length)
-            + PrettyStrings._NEW_LINE
-        )
+        framed.append(horizontal_frame)
 
         return "".join(framed)
 
     @staticmethod
     def column(to_columnize: str, width: int) -> str:
-        """Puts teh given string at the beginning of the line and adds _SPACEs until the end of the
-        line. If the string is too long for the width of the line, it will be cut off.
-
-        Params:
-            to_columnize -> The string to put in column.
+        """Puts teh given string at the beginning of the line and adds spaces until the end of it.
+        If the string is too long for the width of the line, it will be cut off.
 
-            width -> The length of the line.
-
-        Returns:
-            A string containing the columned string.
-        """
+        Params
+        ------
+        - to_columnize -> The string to put in column.
+        - width -> The length of the line.
+
+        Returns
+        -------
+        A string containing the columned string.
+        """
+        columned: list[str] = []
+        to_columnize_length: int = len(to_columnize)
+        chars_to_print: int = min(width, to_columnize_length)
+
+        columned.append(
+            to_columnize[:chars_to_print]
+            if to_columnize_length > chars_to_print
+            else to_columnize
+        )
 
-        to_columnize_length = len(to_columnize)
-        char_to_print = min(width, to_columnize_length)
-        columned = to_columnize[:char_to_print]
-        columned += PrettyStrings.repeat_char(
-            PrettyStrings._SPACE, max(0, width - to_columnize_length)
+        columned.append(
+            PrettyStrings.repeat_char(
+                PrettyStrings._SPACE, max(0, width - to_columnize_length)
+            )
         )
 
-        return columned
+        return "".join(columned)
 
     @staticmethod
     def center(to_center: str, width: int) -> str:
-        """Puts the given string in the center of the line of the given length. If the string is
-        too long it will be cut off.
+        """Puts the given string in the center of the line of the given width. If the string is too
+        long it will be cut off.
 
-        Params:
-            to_center -> The string to center.
+        Params
+        ------
+        - to_center -> The string to center.
+        - width -> The length of the line where to center the string.
 
-            width -> The length of the line where to center the string.
+        Returns
+        -------
+        A string containing the centered string.
         """
+        to_center_length: int = len(to_center)
 
-        to_center_length = len(to_center)
-        if width < to_center_length:
-            centred = to_center[:width]
-        elif width == to_center_length:
-            centred = to_center
-        else:
-            white_spaces = width - to_center_length
-            spaces_before = white_spaces // 2
-            spaces_after = white_spaces - spaces_before
-
-            centred = PrettyStrings.repeat_char(PrettyStrings._SPACE, spaces_before)
-            centred += to_center
-            centred += PrettyStrings.repeat_char(PrettyStrings._SPACE, spaces_after)
+        if to_center_length > width:
+            return to_center[:width]
+
+        if to_center_length == width:
+            return to_center
+
+        centered: list[str] = []
+        whitespaces: int = width - to_center_length
+        whitespaces_before: int = whitespaces // 2
+        whitespaces_after: int = whitespaces - whitespaces_before
 
-        return centred
+        centered.append(
+            PrettyStrings.repeat_char(PrettyStrings._SPACE, whitespaces_before)
+        )
+        centered.append(to_center)
+        centered.append(
+            PrettyStrings.repeat_char(PrettyStrings._SPACE, whitespaces_after)
+        )
+
+        return "".join(centered)
 
     @staticmethod
     def repeat_char(char: str, times: int) -> str:
         """Repeats a given character a given number of times.
 
-        Params:
-            char -> The character to repeat.
-
-            times -> The number of times to repeat the character.
-
-        Returns:
-            A string containing the character repeated.
+        Params
+        ------
+        - char -> The character to repeat.
+        - times -> The number of times to repeat the character.
+
+        Returns
+        -------
+        A string containing the character repeated. If times is less than or equal to 0 an empty
+        string will be returned.
         """
-
         return char * max(0, times)
 
     @staticmethod
     def isolated_line(to_isolate: str) -> str:
-        """Isolated a given string by adding an empty line before and after it.
+        """Isolates a given string by adding an empty line before and after it.
 
-        Params:
-            to_isolate -> The string to isolate.
+        Params
+        ------
+        - to_isolate -> The string to isolate.
 
-        Returns:
-            A string containing the isolated string.
+        Returns
+        -------
+        A string containing the isolated string.
         """
-
-        return PrettyStrings._NEW_LINE + to_isolate + PrettyStrings._NEW_LINE
+        return f"{PrettyStrings._NEW_LINE}{to_isolate}{PrettyStrings._NEW_LINE}"
```

### Comparing `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/random_draws.py` & `kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/random_draws.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,92 +1,89 @@
 """Module for the RandomDraws class"""
 
 # Standard Libraries
 import random
 
 
 class RandomDraws:
-    """
-    This class provides methods for drawing a specific data type in a pseudo-random way.
-    """
+    """This class provides methods for drawing a specific data type in a pseudo-random way."""
 
     _RAND = random.Random()
+    _CONSTRUCTOR_ERROR: str = "This class is not instantiable!"
 
     def __init__(self) -> None:
-        """Prevents instantiation of this class
+        """Prevents the instantiation of this class.
 
-        Raises:
-            NotImplementedError
+        Raises
+        ------
+        - NotImplementedError
         """
-
-        raise NotImplementedError("This class isn't instantiable!")
+        raise NotImplementedError(RandomDraws._CONSTRUCTOR_ERROR)
 
     @staticmethod
     def draw_integer(minimum: int, maximum: int) -> int:
-        """Draws a random integer between given minimum and maximum values.
-
-        Params:
-            minimum -> The minimum value to draw.
-            maximum -> The maximum value to draw
+        """Draws a random integer between given minimum and maximum values included.
 
-        Returns:
-            An integer representing the drawn number.
+        Params
+        ------
+        - minimum -> The minimum value to draw.
+        - maximum -> The maximum value to draw
+
+        Returns
+        -------
+        An integer representing the drawn number.
         """
-
         return RandomDraws._RAND.randint(minimum, maximum)
 
     @staticmethod
     def draw_float(minimum: float, maximum: float) -> float:
-        """Draws a random float between given minimum and maximum values.
-
-        Params:
-            minimum -> The minimum value to draw.
-            maximum -> The maximum value to draw
+        """Draws a random float between given minimum and maximum values included.
 
-        Returns:
-            An float representing the drawn number.
+        Params
+        ------
+        - minimum -> The minimum value to draw.
+        - maximum -> The maximum value to draw
+
+        Returns
+        -------
+        An float representing the drawn number.
         """
-
         return RandomDraws._RAND.uniform(minimum, maximum)
 
     @staticmethod
     def draw_integer_with_distribution(
         minimum: int, maximum: int, exponent: float
     ) -> int:
         """Draws a random integer between given minimum and maximum values, with a certain
         distribution. In order to distribute the values you use the exponent:
-        • exponent &#8804; 0: Completely random values will be given, almost always not between the
+        - exponent &#8804; 0: Completely random values will be given, almost always not between the
         given minimum and maximum values. This usage is not encouraged.
-
-        • 0 < exponent < 1: The values near the maximum have a greater probability of being drawn,
+        - 0 < exponent < 1: The values near the maximum have a greater probability of being drawn,
         closer the exponent is to 0.
-
-        • exponent = 1: All the values have the same probability of being drawn.
-
-        • exponent &#8805; 1: The values near the minimum have a greater probability of being
+        - exponent = 1: All the values have the same probability of being drawn.
+        - exponent &#8805; 1: The values near the minimum have a greater probability of being
         drawn, greater exponents will increase this probability.
 
-        Params:
-            minimum -> The minimum value to draw.
-
-            maximum -> The maximum value to draw.
-
-            exponent -> The exponent of the distribution.
-
-        Returns:
-            An integer representing the drawn number.
+        Params
+        ------
+        - minimum -> The minimum value to draw.
+        - maximum -> The maximum value to draw.
+        - exponent -> The exponent of the distribution.
+
+        Returns
+        -------
+        An integer representing the drawn number.
         """
-
-        drawing_range = maximum + 1 - minimum
-        random_float = RandomDraws._RAND.random() ** exponent
+        drawing_range: int = maximum + 1 - minimum
+        random_float: float = RandomDraws._RAND.random() ** exponent
 
         return minimum + int(drawing_range * random_float)
 
     @staticmethod
     def draw_bool() -> bool:
         """Draws a random bool.
 
-        Returns:
-            The drawn boolean.
+        Returns
+        -------
+        The drawn boolean.
         """
-
         return RandomDraws._RAND.choice([True, False])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/PKG-INFO` & `kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kibo_unibs_fp_lib
-Version: 1.0.4
-Summary: UniBSFpLib modified, documented and converted in python.
+Version: 1.1.0
+Summary: KiboUniBSFpLib modified, documented and converted in python.
 Home-page: https://github.com/AlessandroMuscio/kibo_unibs_fp_lib
 Author: Alessandro Muscio
 Author-email: Alessandro Muscio <a.muscio001@studenti.unibs.it>
 License: MIT License
         
         Copyright (c) 2024 Alessandro Muscio
         
@@ -39,10 +39,22 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # kibo_unibs_fp_lib
 
-Libreria UniBSFpLib modificata e convertita in Python da me per l'utilizzo durante il Programma Arnaldo, ma non ristretta solo a questo utilizzo.
+This library is converted from its original Java counterpart tha can be found [here](https://github.com/AlessandroMuscio/KiboUniBSFpLib). For whatever problem may arise form the use of this library report it on the [github issues](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/issues) of this repository.
 
-*Questo progetto è concesso in licenza secondo i termini della licenza MIT.*
+## Installation
+
+This library is available for all on [PyPI](https://pypi.org) that means it can be installed with:
+
+```bash
+pip install kibo-unibs-fp-lib
+```
+
+## Usage
+
+For an overview of its usages consults the [wiki](https://github.com/AlessandroMuscio/kibo_unibs_fp_lib/wiki) (**WIP!!**).
+
+*This library is distributed under the MIT license, provided [here](LICENSE.txt)*
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kibo_unibs_fp_lib-1.0.4/pyproject.toml` & `kibo_unibs_fp_lib-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kibo_unibs_fp_lib"
-version = "1.0.4"
+version = "1.1.0"
 license = {file = "LICENSE.txt"}
 
-description = "UniBSFpLib modified, documented and converted in python."
+description = "KiboUniBSFpLib modified, documented and converted in python."
 authors = [{ name="Alessandro Muscio", email="a.muscio001@studenti.unibs.it"}]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

