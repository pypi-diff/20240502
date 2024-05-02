# Comparing `tmp/replicate_whisper_diarization-0.2.1.tar.gz` & `tmp/replicate_whisper_diarization-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicate_whisper_diarization-0.2.1.tar", last modified: Thu May  2 17:07:22 2024, max compression
+gzip compressed data, was "replicate_whisper_diarization-0.2.2.tar", last modified: Thu May  2 21:22:31 2024, max compression
```

## Comparing `replicate_whisper_diarization-0.2.1.tar` & `replicate_whisper_diarization-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.785272 replicate_whisper_diarization-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.devcontainer/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.777273 replicate_whisper_diarization-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.github/workflows/pypi-publish.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/notebooks/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/notebooks/01-transcript-with-diarization.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/diarization.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 17:07:22.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-02 17:07:22.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:07:22.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 17:07:22.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 17:07:22.000000 replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:22.781273 replicate_whisper_diarization-0.2.1/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:07:18.000000 replicate_whisper_diarization-0.2.1/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:07:22.785272 replicate_whisper_diarization-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.843383 replicate_whisper_diarization-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.devcontainer/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.835384 replicate_whisper_diarization-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.github/workflows/pypi-publish.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1012 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1086 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 21:22:31.843383 replicate_whisper_diarization-0.2.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/notebooks/01-transcript-with-diarization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/diarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 21:22:31.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-02 21:22:31.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:22:31.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 21:22:31.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 21:22:31.000000 replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:31.839383 replicate_whisper_diarization-0.2.2/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:22:26.000000 replicate_whisper_diarization-0.2.2/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:22:31.843383 replicate_whisper_diarization-0.2.2/setup.cfg
```

### Comparing `replicate_whisper_diarization-0.2.1/.devcontainer/Dockerfile` & `replicate_whisper_diarization-0.2.2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/.devcontainer/devcontainer.json` & `replicate_whisper_diarization-0.2.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/.devcontainer/docker-compose.yml` & `replicate_whisper_diarization-0.2.2/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/.github/workflows/pypi-publish.yaml` & `replicate_whisper_diarization-0.2.2/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/.gitignore` & `replicate_whisper_diarization-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/.pre-commit-config.yaml` & `replicate_whisper_diarization-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/LICENSE` & `replicate_whisper_diarization-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/PKG-INFO` & `replicate_whisper_diarization-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.2.1
+Version: 0.2.2
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `replicate_whisper_diarization-0.2.1/README.md` & `replicate_whisper_diarization-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/notebooks/01-transcript-with-diarization.ipynb` & `replicate_whisper_diarization-0.2.2/notebooks/01-transcript-with-diarization.ipynb`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/pyproject.toml` & `replicate_whisper_diarization-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/diarization.py` & `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/diarization.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/language.py` & `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/language.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,22 +13,23 @@
     response = requests.get(url)
 
     os.makedirs("/tmp/cache", exist_ok=True)
     with open("/tmp/cache/language_detector.tflite", "wb") as f:
         f.write(response.content)
 
 
+@lru_cache
 def load_model():
     download_model()
     base_options = python.BaseOptions(
         model_asset_path="/tmp/cache/language_detector.tflite"
     )
     options = text.LanguageDetectorOptions(base_options=base_options)
     return text.LanguageDetector.create_from_options(options)
 
 
 def detect_language(text: str):
     model = load_model()
 
     preds = model.detect(text)
 
-    return {pred.language_code: f"{pred.probability:.2f}" for pred in preds}
+    return {pred.language_code: f"{pred.probability:.2f}" for pred in preds.detections}
```

### Comparing `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/main.py` & `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from replicate_whisper_diarization.whisper import transcribe
-from replicate_whisper_diarization.segmentation import segmentation
+from replicate_whisper_diarization.segmentation import segmentate
 from replicate_whisper_diarization.diarization import align_word_and_speaker_segments
+from replicate_whisper_diarization.language import detect_language
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def run_transcript_with_diarization(
     audio_url: str,
@@ -21,16 +22,17 @@
         audio_url (str): The URL of the audio file to be transcribed.
 
     Returns:
         list[dict]: A list of dictionaries, where each dictionary represents a word segment with its corresponding
         transcription and speaker information.
     """
     transcription = transcribe(audio_url=audio_url, language=language)
-    speaker_segments = segmentation(audio_url, num_speakers, min_speakers, max_speakers)
+    speaker_segments = segmentate(audio_url, num_speakers, min_speakers, max_speakers)
 
     if not language:
         logger.error("Language not provided. using auto")
+        language = detect_language(transcription["transcript"])
 
     # language = transcript["detected_language"]
     word_timestamps = transcription["chunks"]
     segments = speaker_segments["segments"]
     return align_word_and_speaker_segments(segments, word_timestamps)
```

### Comparing `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/segmentation.py` & `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 MODEL_VERSION = os.getenv(
     "DIARIZATION_MODEL_VERSION",
     "f7425066750cd06fdf95b831c08bba1530f222a2eb4145f40493f431b7483b95",
 )
 
 
-def segmentation(
+def segmentate(
     audio_url: str,
     num_speakers: int | None = None,
     min_speakers: int | None = None,
     max_speakers: int | None = None,
     webhook_url: str | None = None,
 ) -> dict:
     model = replicate.models.get(MODEL_NAME)
```

### Comparing `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization/whisper.py` & `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization/whisper.py`

 * *Files identical despite different names*

### Comparing `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/PKG-INFO` & `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate_whisper_diarization
-Version: 0.2.1
+Version: 0.2.2
 Summary: Transcribe and diarize audio files using Replicate models
 Author-email: "Collective.ai" <info@collectiveai.io>
 License: 
         The MIT License (MIT)
         Copyright (c) 2023, team-collectiveai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `replicate_whisper_diarization-0.2.1/replicate_whisper_diarization.egg-info/SOURCES.txt` & `replicate_whisper_diarization-0.2.2/replicate_whisper_diarization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

