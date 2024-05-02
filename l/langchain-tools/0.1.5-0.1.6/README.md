# Comparing `tmp/langchain-tools-0.1.5.tar.gz` & `tmp/langchain-tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-tools-0.1.5.tar", last modified: Mon Apr 15 08:14:22 2024, max compression
+gzip compressed data, was "langchain-tools-0.1.6.tar", last modified: Mon Apr 15 08:21:22 2024, max compression
```

## Comparing `langchain-tools-0.1.5.tar` & `langchain-tools-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:22.227804 langchain-tools-0.1.5/
--rw-rw-rw-   0        0        0     1583 2024-04-15 08:14:22.225802 langchain-tools-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      459 2024-04-15 05:12:46.000000 langchain-tools-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 08:14:22.227804 langchain-tools-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1721 2024-04-15 08:12:19.000000 langchain-tools-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:22.179853 langchain-tools-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:22.212839 langchain-tools-0.1.5/src/langchain_tools.egg-info/
--rw-rw-rw-   0        0        0     1583 2024-04-15 08:14:21.000000 langchain-tools-0.1.5/src/langchain_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-04-15 08:14:22.000000 langchain-tools-0.1.5/src/langchain_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:14:21.000000 langchain-tools-0.1.5/src/langchain_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-15 08:14:21.000000 langchain-tools-0.1.5/src/langchain_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-15 08:14:21.000000 langchain-tools-0.1.5/src/langchain_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:22.219802 langchain-tools-0.1.5/src/retriever/
--rw-rw-rw-   0        0        0     5223 2024-04-12 10:12:19.000000 langchain-tools-0.1.5/src/retriever/LangchainRetriever.py
--rw-rw-rw-   0        0        0        0 2024-04-06 13:57:16.000000 langchain-tools-0.1.5/src/retriever/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:14:22.224806 langchain-tools-0.1.5/src/retriever/md/
--rw-rw-rw-   0        0        0        0 2024-04-06 13:57:09.000000 langchain-tools-0.1.5/src/retriever/md/__init__.py
--rw-rw-rw-   0        0        0     1607 2024-04-05 12:30:49.000000 langchain-tools-0.1.5/src/retriever/md/split_md.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:21:22.491978 langchain-tools-0.1.6/
+-rw-rw-rw-   0        0        0     1343 2024-04-15 08:21:22.490978 langchain-tools-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2024-04-15 05:12:46.000000 langchain-tools-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 08:21:22.432424 langchain-tools-0.1.6/langchain_tools.egg-info/
+-rw-rw-rw-   0        0        0     1343 2024-04-15 08:21:21.000000 langchain-tools-0.1.6/langchain_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2024-04-15 08:21:21.000000 langchain-tools-0.1.6/langchain_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:21:21.000000 langchain-tools-0.1.6/langchain_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-15 08:21:21.000000 langchain-tools-0.1.6/langchain_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-15 08:21:21.000000 langchain-tools-0.1.6/langchain_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:21:22.492994 langchain-tools-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2073 2024-04-15 08:21:14.000000 langchain-tools-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:21:22.438435 langchain-tools-0.1.6/src/
+-rw-rw-rw-   0        0        0        0 2024-04-11 11:26:59.000000 langchain-tools-0.1.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:21:22.445449 langchain-tools-0.1.6/src/retriever/
+-rw-rw-rw-   0        0        0     5223 2024-04-12 10:12:19.000000 langchain-tools-0.1.6/src/retriever/LangchainRetriever.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 13:57:16.000000 langchain-tools-0.1.6/src/retriever/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:21:22.460423 langchain-tools-0.1.6/src/retriever/md/
+-rw-rw-rw-   0        0        0        0 2024-04-06 13:57:09.000000 langchain-tools-0.1.6/src/retriever/md/__init__.py
+-rw-rw-rw-   0        0        0     1607 2024-04-05 12:30:49.000000 langchain-tools-0.1.6/src/retriever/md/split_md.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:21:22.488964 langchain-tools-0.1.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-11 15:52:09.000000 langchain-tools-0.1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     1061 2024-04-12 10:33:46.000000 langchain-tools-0.1.6/tests/main_tests.py
+-rw-rw-rw-   0        0        0     1273 2024-04-12 12:33:00.000000 langchain-tools-0.1.6/tests/test_retriever_from_md_file.py
+-rw-rw-rw-   0        0        0     1213 2024-04-12 12:32:51.000000 langchain-tools-0.1.6/tests/test_retriever_from_url.py
+-rw-rw-rw-   0        0        0      857 2024-04-12 12:34:18.000000 langchain-tools-0.1.6/tests/test_runnable_from_md_file.py
+-rw-rw-rw-   0        0        0      797 2024-04-12 12:34:40.000000 langchain-tools-0.1.6/tests/test_runnable_from_url.py
```

### Comparing `langchain-tools-0.1.5/PKG-INFO` & `langchain-tools-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: langchain-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simplifying, enhancing, and extending the LangChain library functionality
 Home-page: https://github.com/MartinChen1973/langchain-tools
 Author: Langchain Tools Team
 Author-email: cheny@cheny.com
-Project-URL: Bug Tracker, https://github.com/MartinChen1973/langchain-tools/issues
-Project-URL: Documentation, https://MartinChen1973.github.io/langchain-tools/
-Project-URL: Source Code, https://github.com/MartinChen1973/langchain-tools
 Keywords: language processing,AI,natural language understanding,LangChain,LLM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `langchain-tools-0.1.5/src/langchain_tools.egg-info/PKG-INFO` & `langchain-tools-0.1.6/langchain_tools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: langchain-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simplifying, enhancing, and extending the LangChain library functionality
 Home-page: https://github.com/MartinChen1973/langchain-tools
 Author: Langchain Tools Team
 Author-email: cheny@cheny.com
-Project-URL: Bug Tracker, https://github.com/MartinChen1973/langchain-tools/issues
-Project-URL: Documentation, https://MartinChen1973.github.io/langchain-tools/
-Project-URL: Source Code, https://github.com/MartinChen1973/langchain-tools
 Keywords: language processing,AI,natural language understanding,LangChain,LLM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `langchain-tools-0.1.5/src/retriever/LangchainRetriever.py` & `langchain-tools-0.1.6/src/retriever/LangchainRetriever.py`

 * *Files identical despite different names*

### Comparing `langchain-tools-0.1.5/src/retriever/md/split_md.py` & `langchain-tools-0.1.6/src/retriever/md/split_md.py`

 * *Files identical despite different names*

