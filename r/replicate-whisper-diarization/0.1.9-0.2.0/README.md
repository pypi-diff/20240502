# Comparing `tmp/replicate_whisper_diarization-0.1.9.tar.gz` & `tmp/replicate_whisper_diarization-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicate_whisper_diarization-0.1.9.tar", last modified: Tue Dec 12 15:38:12 2023, max compression
+gzip compressed data, was "replicate_whisper_diarization-0.2.0.tar", last modified: Thu May  2 15:35:58 2024, max compression
```

## Comparing `replicate_whisper_diarization-0.1.9.tar` & `replicate_whisper_diarization-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/.devcontainer/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.524728 replicate_whisper_diarization-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/.github/workflows/pypi-publish.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/notebooks/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)   123303 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/notebooks/01-transcript-with-diarization.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/diarization/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/diarization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/diarization/diarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/diarization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/whisper/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/whisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/whisper/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-12-12 15:38:12.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-12-12 15:38:12.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 15:38:12.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-12 15:38:12.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-12 15:38:12.000000 replicate_whisper_diarization-0.1.9/replicate_whisper_diarization.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 15:38:00.000000 replicate_whisper_diarization-0.1.9/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-12 15:38:12.528728 replicate_whisper_diarization-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.devcontainer/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.610195 replicate_whisper_diarization-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.github/workflows/pypi-publish.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/notebooks/01-transcript-with-diarization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/diarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-02 15:35:58.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-02 15:35:58.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:35:58.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 15:35:58.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 15:35:58.000000 replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:35:54.000000 replicate_whisper_diarization-0.2.0/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:35:58.614195 replicate_whisper_diarization-0.2.0/setup.cfg
```

### Comparing `replicate_whisper_diarization-0.1.9/.devcontainer/Dockerfile` & `replicate_whisper_diarization-0.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.1.9/.devcontainer/devcontainer.json` & `replicate_whisper_diarization-0.2.0/.devcontainer/devcontainer.json`

 * *Files 13% similar despite different names*

```diff
@@ -8,30 +8,32 @@
 	"runServices": [
 		"devcontainer"
 	],
 	"workspaceFolder": "/workspace",
 	"customizations": {
 		"vscode": {
 			"settings": {
-				"python.pythonPath": "/bin/local/python",
 				"python.languageServer": "Pylance",
+				"python.formatting.provider": "none",
+				"python.linting.enabled": true,
 				"editor.formatOnSave": true,
-				"notebook.formatOnSave.enabled": true,
 				"[python]": {
-					"editor.defaultFormatter": "ms-python.black-formatter",
+					"editor.defaultFormatter": "charliermarsh.ruff",
 					"editor.formatOnSave": true,
 					"editor.codeActionsOnSave": {
-						"source.organizeImports": true
+						"source.fixAll": "never",
+						"source.organizeImports": "explicit"
 					},
 					"ruff.organizeImports": false
 				},
-				"black-formatter.args": [
-					"--line-length",
-					"88"
-				],
+				"notebook.formatOnSave.enabled": true,
+				"notebook.codeActionsOnSave": {
+					"notebook.source.fixAll": "never",
+					"notebook.source.organizeImports": "explicit"
+				},
 				"isort.args": [
 					"--profile",
 					"black",
 					"--length-sort",
 					"--combine-as",
 					"--force-sort-within-sections"
 				],
@@ -41,23 +43,21 @@
 					"**/.git/objects/**": true,
 					"**/.git/subtree-cache/**": true
 				}
 			},
 			// Add the IDs of extensions you want installed when the container is created.
 			"extensions": [
 				"ms-python.python",
+				"charliermarsh.ruff",
 				"magicstack.magicpython",
-				"ms-python.black-formatter",
 				"ms-python.isort",
 				"eamodio.gitlens",
 				"GitHub.copilot",
 				"GitHub.copilot-labs",
-				"charliermarsh.ruff",
-				"GitHub.vscode-pull-request-github",
-				"github.vscode-github-actions"
+				"ms-toolsai.jupyter"
 			]
 		}
 	},
 	// Use 'forwardPorts' to make a list of ports inside the container available locally.
 	// "forwardPorts": [],
 	// Use 'postCreateCommand' to run commands after the container is created.
 	"postCreateCommand": "sudo pip install -e /workspace/"
```

### Comparing `replicate_whisper_diarization-0.1.9/.devcontainer/docker-compose.yml` & `replicate_whisper_diarization-0.2.0/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.1.9/.github/workflows/pypi-publish.yaml` & `replicate_whisper_diarization-0.2.0/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.1.9/.gitignore` & `replicate_whisper_diarization-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.1.9/.pre-commit-config.yaml` & `replicate_whisper_diarization-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.1.9/LICENSE` & `replicate_whisper_diarization-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.1.9/PKG-INFO` & `replicate_whisper_diarization-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.1.9
+Version: 0.2.0
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -18,16 +18,17 @@
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: replicate==0.15.5
-Requires-Dist: rich==13.6.0
+Requires-Dist: replicate>=0.25.2
+Requires-Dist: mediapipe<0.11,>=0.10.11
+Requires-Dist: flask<4,>=3.0.3
 
 whisper_diarization
 ==============================
 
 A short description of the project.
 
 # Development
```

### Comparing `replicate_whisper_diarization-0.1.9/README.md` & `replicate_whisper_diarization-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.1.9/pyproject.toml` & `replicate_whisper_diarization-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["feed", "reader", "tutorial"]
 dependencies = [
-    "replicate==0.15.5",
-    "rich==13.6.0",
+    "replicate>=0.25.2",
+    "mediapipe>=0.10.11, <0.11",
+    "flask>=3.0.3, <4",
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/collectiveai-team/whisper-diarization"
 
 [tool.setuptools.packages.find]
```

### Comparing `replicate_whisper_diarization-0.1.9/replicate_whisper_diarization/main.py` & `replicate_whisper_diarization-0.2.0/replicate_whisper_diarization/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 from replicate_whisper_diarization.whisper import transcribe
-from replicate_whisper_diarization.diarization import run_diarization, run_segmentation
+from replicate_whisper_diarization.segmentation import segmentation
+from replicate_whisper_diarization.diarization import align_word_and_speaker_segments
+import logging
 
-
-def extract_word_timestamps(segments: list[dict]) -> list[dict]:
-    word_timestamps = []
-
-    for segment in segments:
-        for word in segment["words"]:
-            word_timestamps.append(word.update({"text": word["word"]}) or word)
-    return word_timestamps
+logger = logging.getLogger(__name__)
 
 
 def run_transcript_with_diarization(
-    audio_url: str, whisper_model: str = "base"
+    audio_url: str,
+    language: str | None = None,
+    num_speakers: int | None = None,
+    min_speakers: int | None = None,
+    max_speakers: int | None = None,
 ) -> list[dict]:
-    transcript = transcribe(audio_url=audio_url, model=whisper_model)
-    segments = transcript["segments"]
-    language = transcript["detected_language"]
-    word_timestamps = extract_word_timestamps(segments)
-    segments = run_segmentation(audio_url)["segments"]
-    return run_diarization(segments, word_timestamps, language)
+    """
+    Runs diarization on the given audio and returns a list of dictionaries containing word-level transcriptions
+    along with speaker information.
+
+    Args:
+        audio_url (str): The URL of the audio file to be transcribed.
+
+    Returns:
+        list[dict]: A list of dictionaries, where each dictionary represents a word segment with its corresponding
+        transcription and speaker information.
+    """
+    transcription = transcribe(audio_url=audio_url, language=language)
+    speaker_segments = segmentation(audio_url, num_speakers, min_speakers, max_speakers)
+
+    if not language:
+        logger.error("Language not provided. using auto")
+
+    # language = transcript["detected_language"]
+    word_timestamps = transcription["chunks"]
+    segments = speaker_segments["segments"]
+    return align_word_and_speaker_segments(segments, word_timestamps)
```

### Comparing `replicate_whisper_diarization-0.1.9/replicate_whisper_diarization.egg-info/PKG-INFO` & `replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: replicate-whisper-diarization
-Version: 0.1.9
+Name: replicate_whisper_diarization
+Version: 0.2.0
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -18,16 +18,17 @@
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: replicate==0.15.5
-Requires-Dist: rich==13.6.0
+Requires-Dist: replicate>=0.25.2
+Requires-Dist: mediapipe<0.11,>=0.10.11
+Requires-Dist: flask<4,>=3.0.3
 
 whisper_diarization
 ==============================
 
 A short description of the project.
 
 # Development
```

### Comparing `replicate_whisper_diarization-0.1.9/replicate_whisper_diarization.egg-info/SOURCES.txt` & `replicate_whisper_diarization-0.2.0/replicate_whisper_diarization.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,19 @@
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .devcontainer/docker-compose.yml
 .github/workflows/pypi-publish.yaml
 notebooks/.gitkeep
 notebooks/01-transcript-with-diarization.ipynb
 replicate_whisper_diarization/__init__.py
+replicate_whisper_diarization/diarization.py
+replicate_whisper_diarization/language.py
 replicate_whisper_diarization/main.py
+replicate_whisper_diarization/segmentation.py
 replicate_whisper_diarization/webhook.py
+replicate_whisper_diarization/whisper.py
 replicate_whisper_diarization.egg-info/PKG-INFO
 replicate_whisper_diarization.egg-info/SOURCES.txt
 replicate_whisper_diarization.egg-info/dependency_links.txt
 replicate_whisper_diarization.egg-info/requires.txt
 replicate_whisper_diarization.egg-info/top_level.txt
-replicate_whisper_diarization/diarization/__init__.py
-replicate_whisper_diarization/diarization/diarization.py
-replicate_whisper_diarization/diarization/utils.py
-replicate_whisper_diarization/logger/__init__.py
-replicate_whisper_diarization/logger/logger.py
-replicate_whisper_diarization/whisper/__init__.py
-replicate_whisper_diarization/whisper/whisper.py
 resources/.gitkeep
```

