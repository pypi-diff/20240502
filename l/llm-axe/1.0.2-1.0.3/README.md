# Comparing `tmp/llm_axe-1.0.2.tar.gz` & `tmp/llm_axe-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_axe-1.0.2.tar", last modified: Sun Apr 28 20:05:22 2024, max compression
+gzip compressed data, was "llm_axe-1.0.3.tar", last modified: Thu May  2 02:34:10 2024, max compression
```

## Comparing `llm_axe-1.0.2.tar` & `llm_axe-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 20:05:22.982692 llm_axe-1.0.2/
--rw-rw-rw-   0        0        0      722 2024-04-28 20:05:22.982692 llm_axe-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-28 20:05:22.976194 llm_axe-1.0.2/llm_axe/
--rw-rw-rw-   0        0        0       67 2024-04-22 04:52:11.000000 llm_axe-1.0.2/llm_axe/__init__.py
--rw-rw-rw-   0        0        0    19134 2024-04-28 19:57:57.000000 llm_axe-1.0.2/llm_axe/agents.py
--rw-rw-rw-   0        0        0     5933 2024-04-28 05:38:57.000000 llm_axe-1.0.2/llm_axe/core.py
--rw-rw-rw-   0        0        0      551 2024-04-27 04:29:01.000000 llm_axe-1.0.2/llm_axe/models.py
--rw-rw-rw-   0        0        0     6760 2024-04-28 19:53:55.000000 llm_axe-1.0.2/llm_axe/system_prompts.yaml
-drwxrwxrwx   0        0        0        0 2024-04-28 20:05:22.981690 llm_axe-1.0.2/llm_axe.egg-info/
--rw-rw-rw-   0        0        0      722 2024-04-28 20:05:22.000000 llm_axe-1.0.2/llm_axe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-04-28 20:05:22.000000 llm_axe-1.0.2/llm_axe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 20:05:22.000000 llm_axe-1.0.2/llm_axe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2024-04-28 20:05:22.000000 llm_axe-1.0.2/llm_axe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-28 20:05:22.000000 llm_axe-1.0.2/llm_axe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 20:05:22.983191 llm_axe-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1403 2024-04-28 20:04:52.000000 llm_axe-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:34:10.205529 llm_axe-1.0.3/
+-rw-rw-rw-   0        0        0      722 2024-05-02 02:34:10.205028 llm_axe-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 02:34:10.150431 llm_axe-1.0.3/llm_axe/
+-rw-rw-rw-   0        0        0       67 2024-04-22 04:52:11.000000 llm_axe-1.0.3/llm_axe/__init__.py
+-rw-rw-rw-   0        0        0    19134 2024-05-02 02:25:56.000000 llm_axe-1.0.3/llm_axe/agents.py
+-rw-rw-rw-   0        0        0     5933 2024-04-28 05:38:57.000000 llm_axe-1.0.3/llm_axe/core.py
+-rw-rw-rw-   0        0        0      551 2024-04-27 04:29:01.000000 llm_axe-1.0.3/llm_axe/models.py
+-rw-rw-rw-   0        0        0     6760 2024-04-28 19:53:55.000000 llm_axe-1.0.3/llm_axe/system_prompts.yaml
+drwxrwxrwx   0        0        0        0 2024-05-02 02:34:10.204028 llm_axe-1.0.3/llm_axe.egg-info/
+-rw-rw-rw-   0        0        0      722 2024-05-02 02:34:09.000000 llm_axe-1.0.3/llm_axe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-02 02:34:09.000000 llm_axe-1.0.3/llm_axe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 02:34:09.000000 llm_axe-1.0.3/llm_axe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2024-05-02 02:34:09.000000 llm_axe-1.0.3/llm_axe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 02:34:09.000000 llm_axe-1.0.3/llm_axe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 02:34:10.205529 llm_axe-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2024-05-02 02:33:46.000000 llm_axe-1.0.3/setup.py
```

### Comparing `llm_axe-1.0.2/PKG-INFO` & `llm_axe-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_axe
-Version: 1.0.2
+Version: 1.0.3
 Summary: A toolkit for quickly implementing llm powered functionalities.
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `llm_axe-1.0.2/llm_axe/agents.py` & `llm_axe-1.0.3/llm_axe/agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             return None
         if history is not None:
             self.chat_history.extend(history)
 
         user_prompt = make_prompt("user", prompt)
         coder_prompts = [self.system_prompt, user_prompt]
         code_response = self.llm.ask(coder_prompts)
-        self.chat_history.append(coder_prompts[1:])
+        self.chat_history.extend(coder_prompts[1:])
         self.chat_history.append(make_prompt("assistant", code_response))
 
         code = code_response.split("```")[1]
 
         # Clean up code
         if "Python" in code:
             code = code.replace("Python", "")
```

### Comparing `llm_axe-1.0.2/llm_axe/core.py` & `llm_axe-1.0.3/llm_axe/core.py`

 * *Files identical despite different names*

### Comparing `llm_axe-1.0.2/llm_axe/models.py` & `llm_axe-1.0.3/llm_axe/models.py`

 * *Files identical despite different names*

### Comparing `llm_axe-1.0.2/llm_axe/system_prompts.yaml` & `llm_axe-1.0.3/llm_axe/system_prompts.yaml`

 * *Files identical despite different names*

### Comparing `llm_axe-1.0.2/llm_axe.egg-info/PKG-INFO` & `llm_axe-1.0.3/llm_axe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-axe
-Version: 1.0.2
+Version: 1.0.3
 Summary: A toolkit for quickly implementing llm powered functionalities.
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `llm_axe-1.0.2/setup.py` & `llm_axe-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.2' 
+VERSION = '1.0.3' 
 DESCRIPTION = 'A toolkit for quickly implementing llm powered functionalities.'
 LONG_DESCRIPTION = 'llm_axe allows you to quickly implement complex interactions for local LLMs, such as function callers, online agents, pre-made generic agents, and more.'
 
 # Setting up
 setup(
         name="llm_axe", 
         version=VERSION,
```

