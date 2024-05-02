# Comparing `tmp/xiomedon-1.0.1.tar.gz` & `tmp/xiomedon-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiomedon-1.0.1.tar", last modified: Wed May  1 13:14:17 2024, max compression
+gzip compressed data, was "xiomedon-1.0.2.tar", last modified: Thu May  2 08:20:20 2024, max compression
```

## Comparing `xiomedon-1.0.1.tar` & `xiomedon-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,30 @@
-drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-01 13:14:17.091139 xiomedon-1.0.1/
--rw-r--r--   0 ashwinaravind   (501) staff       (20)    11357 2024-05-01 12:01:47.000000 xiomedon-1.0.1/LICENSE
--rw-r--r--   0 ashwinaravind   (501) staff       (20)     1636 2024-05-01 13:14:17.091072 xiomedon-1.0.1/PKG-INFO
--rw-r--r--   0 ashwinaravind   (501) staff       (20)     1286 2024-05-01 10:39:08.000000 xiomedon-1.0.1/README.md
--rw-r--r--   0 ashwinaravind   (501) staff       (20)      551 2024-05-01 12:51:47.000000 xiomedon-1.0.1/pyproject.toml
--rw-r--r--   0 ashwinaravind   (501) staff       (20)      645 2024-05-01 13:14:17.091427 xiomedon-1.0.1/setup.cfg
-drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-01 13:14:17.087917 xiomedon-1.0.1/src/
-drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-01 13:14:17.089614 xiomedon-1.0.1/src/xiomedon/
--rw-r--r--   0 ashwinaravind   (501) staff       (20)      205 2024-05-01 13:08:33.000000 xiomedon-1.0.1/src/xiomedon/__init__.py
--rw-r--r--   0 ashwinaravind   (501) staff       (20)      442 2024-05-01 12:46:37.000000 xiomedon-1.0.1/src/xiomedon/_version.py
--rw-r--r--   0 ashwinaravind   (501) staff       (20)      424 2024-05-01 12:42:54.000000 xiomedon-1.0.1/src/xiomedon/openai_wrapper.py
-drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-01 13:14:17.090740 xiomedon-1.0.1/src/xiomedon.egg-info/
--rw-r--r--   0 ashwinaravind   (501) staff       (20)     1636 2024-05-01 13:14:17.000000 xiomedon-1.0.1/src/xiomedon.egg-info/PKG-INFO
--rw-r--r--   0 ashwinaravind   (501) staff       (20)      302 2024-05-01 13:14:17.000000 xiomedon-1.0.1/src/xiomedon.egg-info/SOURCES.txt
--rw-r--r--   0 ashwinaravind   (501) staff       (20)        1 2024-05-01 13:14:17.000000 xiomedon-1.0.1/src/xiomedon.egg-info/dependency_links.txt
--rw-r--r--   0 ashwinaravind   (501) staff       (20)       18 2024-05-01 13:14:17.000000 xiomedon-1.0.1/src/xiomedon.egg-info/requires.txt
--rw-r--r--   0 ashwinaravind   (501) staff       (20)        9 2024-05-01 13:14:17.000000 xiomedon-1.0.1/src/xiomedon.egg-info/top_level.txt
+drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-02 08:20:20.472843 xiomedon-1.0.2/
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)       32 2024-05-02 07:08:08.000000 xiomedon-1.0.2/.gitignore
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)    11357 2024-05-01 12:01:47.000000 xiomedon-1.0.2/LICENSE
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)     1755 2024-05-02 08:20:20.472737 xiomedon-1.0.2/PKG-INFO
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)     1152 2024-05-01 15:20:14.000000 xiomedon-1.0.2/README.md
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      812 2024-05-02 08:20:16.000000 xiomedon-1.0.2/pyproject.toml
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      404 2024-05-02 07:35:38.000000 xiomedon-1.0.2/pytest.ini
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      118 2024-05-02 06:55:53.000000 xiomedon-1.0.2/requirements.txt
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      645 2024-05-02 08:20:20.473171 xiomedon-1.0.2/setup.cfg
+drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-02 08:20:20.466381 xiomedon-1.0.2/src/
+drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-02 08:20:20.468762 xiomedon-1.0.2/src/xiomedon/
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      205 2024-05-01 13:08:33.000000 xiomedon-1.0.2/src/xiomedon/__init__.py
+drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-02 08:20:20.470360 xiomedon-1.0.2/src/xiomedon/__pycache__/
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      874 2024-05-01 12:29:57.000000 xiomedon-1.0.2/src/xiomedon/__pycache__/openai.cpython-311.pyc
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      843 2024-05-01 12:36:46.000000 xiomedon-1.0.2/src/xiomedon/__pycache__/openai_wrapper.cpython-311.pyc
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      460 2024-05-02 08:20:20.000000 xiomedon-1.0.2/src/xiomedon/_version.py
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      424 2024-05-01 15:20:28.000000 xiomedon-1.0.2/src/xiomedon/openai_wrapper.py
+drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-02 08:20:20.472364 xiomedon-1.0.2/src/xiomedon.egg-info/
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)     1755 2024-05-02 08:20:20.000000 xiomedon-1.0.2/src/xiomedon.egg-info/PKG-INFO
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      681 2024-05-02 08:20:20.000000 xiomedon-1.0.2/src/xiomedon.egg-info/SOURCES.txt
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)        1 2024-05-02 08:20:20.000000 xiomedon-1.0.2/src/xiomedon.egg-info/dependency_links.txt
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      122 2024-05-02 08:20:20.000000 xiomedon-1.0.2/src/xiomedon.egg-info/requires.txt
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)        9 2024-05-02 08:20:20.000000 xiomedon-1.0.2/src/xiomedon.egg-info/top_level.txt
+drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-02 08:20:20.471054 xiomedon-1.0.2/tests/
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)        0 2024-05-02 06:35:11.000000 xiomedon-1.0.2/tests/__init.py
+drwxr-xr-x   0 ashwinaravind   (501) staff       (20)        0 2024-05-02 08:20:20.472020 xiomedon-1.0.2/tests/__pycache__/
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)     1717 2024-05-02 06:50:52.000000 xiomedon-1.0.2/tests/__pycache__/openai_wrapper.cpython-311-pytest-7.2.1.pyc
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)     1717 2024-05-02 06:31:56.000000 xiomedon-1.0.2/tests/__pycache__/openai_wrapper.cpython-311-pytest-8.2.0.pyc
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)     2872 2024-05-02 06:58:57.000000 xiomedon-1.0.2/tests/__pycache__/test_openai_wrapper.cpython-311-pytest-7.2.1.pyc
+-rw-r--r--   0 ashwinaravind   (501) staff       (20)      366 2024-05-02 06:58:55.000000 xiomedon-1.0.2/tests/test_openai_wrapper.py
```

### Comparing `xiomedon-1.0.1/LICENSE` & `xiomedon-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xiomedon-1.0.1/README.md` & `xiomedon-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -50,23 +50,19 @@
    pip show xiomedon
    ```
 
 ## Usage
 
 
    ```
-      from datasets import Dataset 
-      import os
-      from xiomedon import openai_invoke
+   import os
+   import xiomedon as x
 
-      os.environ["OPENAI_API_KEY"] = "your-openai-key"
+   # Set your OpenAI API key
+   os.environ["OPENAI_API_KEY"] = "your-openai-key"
 
-      question_answer_sample = {
-         'question': 'What is the name of the magical device used in the Harry Potter series to store and view memories?',
-         'answer': 'Pensieve',
-      }
+   # 'xiomedon` provides a function `invoke_openai` caling gpt3.5 turbo  and returns string with response
+   response = x.invoke_openai("what is the capital of Austria?")
+   print(response)
 
-      dataset = Dataset.from_dict(question_answer_sample)
-
-      response = openai_invoke(dataset)
    ```
```

### Comparing `xiomedon-1.0.1/setup.cfg` & `xiomedon-1.0.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xiomedon
-version = 1.0.1
+version = 1.0.2
 author = Ashwin Aravind
 author_email = ashwinaravind@gmail.com
 description = Library to call Open AI gpt3.5t-turbo
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ashwinaravind/xiomedon
 project_urls =
```

