# Comparing `tmp/replicate_whisper_diarization-0.2.0.tar.gz` & `tmp/replicate_whisper_diarization-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicate_whisper_diarization-0.2.0.tar", last modified: Thu May  2 15:35:58 2024, max compression
+gzip compressed data, was "replicate_whisper_diarization-0.2.1.tar", last modified: Thu May  2 17:07:22 2024, max compression
```

## Comparing `replicate_whisper_diarization-0.2.0.tar` & `replicate_whisper_diarization-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.devcontainer/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.610195 replicate_whisper_diarization-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.github/workflows/pypi-publish.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/notebooks/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/notebooks/01-transcript-with-diarization.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/diarization.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-02 15:35:58.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-02 15:35:58.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:35:58.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 15:35:58.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 15:35:58.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.785272 replicate_whisper_diarization-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.devcontainer/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.777273 replicate_whisper_diarization-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.github/workflows/pypi-publish.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/notebooks/01-transcript-with-diarization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/diarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 17:07:22.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-02 17:07:22.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:07:22.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 17:07:22.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 17:07:22.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:07:22.785272 replicate_whisper_diarization-0.2.1/setup.cfg
```

### Comparing `replicate_whisper_diarization-0.2.0/.devcontainer/Dockerfile` & `replicate_whisper_diarization-0.2.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/.devcontainer/devcontainer.json` & `replicate_whisper_diarization-0.2.1/.devcontainer/devcontainer.json`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 				"ms-python.python",
 				"charliermarsh.ruff",
 				"magicstack.magicpython",
 				"ms-python.isort",
 				"eamodio.gitlens",
 				"GitHub.copilot",
 				"GitHub.copilot-labs",
-				"ms-toolsai.jupyter"
+				"ms-toolsai.jupyter",
+				"github.vscode-github-actions"
 			]
 		}
 	},
 	// Use 'forwardPorts' to make a list of ports inside the container available locally.
 	// "forwardPorts": [],
 	// Use 'postCreateCommand' to run commands after the container is created.
 	"postCreateCommand": "sudo pip install -e /workspace/"
```

### Comparing `replicate_whisper_diarization-0.2.0/.devcontainer/docker-compose.yml` & `replicate_whisper_diarization-0.2.1/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/.github/workflows/pypi-publish.yaml` & `replicate_whisper_diarization-0.2.1/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/.gitignore` & `replicate_whisper_diarization-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/.pre-commit-config.yaml` & `replicate_whisper_diarization-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/LICENSE` & `replicate_whisper_diarization-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/PKG-INFO` & `replicate_whisper_diarization-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.2.0
+Version: 0.2.1
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -19,15 +19,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: replicate>=0.25.2
-Requires-Dist: mediapipe<0.11,>=0.10.11
 Requires-Dist: flask<4,>=3.0.3
 
 whisper_diarization
 ==============================
 
 A short description of the project.
```

### Comparing `replicate_whisper_diarization-0.2.0/README.md` & `replicate_whisper_diarization-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/notebooks/01-transcript-with-diarization.ipynb` & `replicate_whisper_diarization-0.2.1/notebooks/01-transcript-with-diarization.ipynb`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/pyproject.toml` & `replicate_whisper_diarization-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["feed", "reader", "tutorial"]
 dependencies = [
     "replicate>=0.25.2",
-    "mediapipe>=0.10.11, <0.11",
+#    "mediapipe>=0.10.11, <0.11",
     "flask>=3.0.3, <4",
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/collectiveai-team/whisper-diarization"
```

### Comparing `replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/diarization.py` & `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/diarization.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/language.py` & `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/language.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/main.py` & `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/main.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/segmentation.py` & `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/segmentation.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/whisper.py` & `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/whisper.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/PKG-INFO` & `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.2.0
+Version: 0.2.1
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -19,15 +19,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: replicate>=0.25.2
-Requires-Dist: mediapipe<0.11,>=0.10.11
 Requires-Dist: flask<4,>=3.0.3
 
 whisper_diarization
 ==============================
 
 A short description of the project.
```

### Comparing `replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/SOURCES.txt` & `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

