# Comparing `tmp/panoptica_genai_protection-0.1.0.tar.gz` & `tmp/panoptica_genai_protection-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptica_genai_protection-0.1.0.tar", last modified: Thu Mar  7 13:18:00 2024, max compression
+gzip compressed data, was "panoptica_genai_protection-0.1.3.tar", last modified: Thu May  2 10:08:05 2024, max compression
```

## Comparing `panoptica_genai_protection-0.1.0.tar` & `panoptica_genai_protection-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:18:00.450587 panoptica_genai_protection-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-03-07 13:18:00.450587 panoptica_genai_protection-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-07 13:17:51.000000 panoptica_genai_protection-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 13:18:00.450587 panoptica_genai_protection-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:08:05.916166 panoptica_genai_protection-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-02 10:08:05.912166 panoptica_genai_protection-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-02 10:07:54.000000 panoptica_genai_protection-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:08:05.916166 panoptica_genai_protection-0.1.3/setup.cfg
```

### Comparing `panoptica_genai_protection-0.1.0/PKG-INFO` & `panoptica_genai_protection-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptica_genai_protection
-Version: 0.1.0
+Version: 0.1.3
 Summary: Protecting GenAI from Prompt Injection
 Author: marvin-team@cisco.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -38,15 +38,15 @@
 
 GenAIProtectionClient provides the check_llm_prompt method to determine the safety level of a given prompt.
 
 
 ### Sample Snippet
 ```python
 from panoptica_genai_protection.client import GenAIProtectionClient
-from panoptica_genai_protection.models import Result as InspectionResult
+from panoptica_genai_protection.gen.models import Result as InspectionResult
 
 # ... Other code in your module ...
 
 # initialize the client
 genai_protection_client = GenAIProtectionClient()
 
 # Send the prompt for inspection BEFORE sending it to the LLM
```

