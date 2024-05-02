# Comparing `tmp/panoptica_genai_protection-0.1.3.tar.gz` & `tmp/panoptica_genai_protection-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptica_genai_protection-0.1.3.tar", last modified: Thu May  2 10:08:05 2024, max compression
+gzip compressed data, was "panoptica_genai_protection-0.1.4.tar", last modified: Thu May  2 11:23:45 2024, max compression
```

## Comparing `panoptica_genai_protection-0.1.3.tar` & `panoptica_genai_protection-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:08:05.916166 panoptica_genai_protection-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-02 10:08:05.912166 panoptica_genai_protection-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-02 10:07:54.000000 panoptica_genai_protection-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:08:05.916166 panoptica_genai_protection-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:23:45.272153 panoptica_genai_protection-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-02 11:23:45.272153 panoptica_genai_protection-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-02 11:23:36.000000 panoptica_genai_protection-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 11:23:45.276153 panoptica_genai_protection-0.1.4/setup.cfg
```

### Comparing `panoptica_genai_protection-0.1.3/PKG-INFO` & `panoptica_genai_protection-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptica_genai_protection
-Version: 0.1.3
+Version: 0.1.4
 Summary: Protecting GenAI from Prompt Injection
 Author: marvin-team@cisco.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `panoptica_genai_protection-0.1.3/README.md` & `panoptica_genai_protection-0.1.4/README.md`

 * *Files identical despite different names*

