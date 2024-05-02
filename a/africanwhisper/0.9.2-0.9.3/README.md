# Comparing `tmp/africanwhisper-0.9.2.tar.gz` & `tmp/africanwhisper-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.9.2.tar", max compression
+gzip compressed data, was "africanwhisper-0.9.3.tar", max compression
```

## Comparing `africanwhisper-0.9.2.tar` & `africanwhisper-0.9.3.tar`

### file list

```diff
@@ -1,43 +1,38 @@
--rw-r--r--   0        0        0     1067 2024-05-01 10:55:03.102471 africanwhisper-0.9.2/LICENSE
--rw-r--r--   0        0        0    11868 2024-05-01 10:55:03.102471 africanwhisper-0.9.2/README.md
--rw-r--r--   0        0        0     1248 2024-05-01 10:55:03.110471 africanwhisper-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     8196 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/.DS_Store
--rw-r--r--   0        0        0       60 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/.dockerignore
--rw-r--r--   0        0        0      100 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/.env
--rw-r--r--   0        0        0      361 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/Dockerfile
--rw-r--r--   0        0        0        0 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/__init__.py
--rw-r--r--   0        0        0     7479 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/app.py
--rw-r--r--   0        0        0    11598 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/dashboard.json
--rw-r--r--   0        0        0      538 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/docker-compose.yaml
--rw-r--r--   0        0        0        0 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/__init__.py
--rw-r--r--   0        0        0    18321 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/alignment.py
--rw-r--r--   0        0        0    11001 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/asr.py
--rw-r--r--   0        0        0     4894 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/audio.py
--rw-r--r--   0        0        0     3276 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/diarize.py
--rw-r--r--   0        0        0     3759 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/load_asr_model.py
--rw-r--r--   0        0        0     4271 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/mel_filters.npz
--rw-r--r--   0        0        0     9103 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/subtitles_processor.py
--rw-r--r--   0        0        0     1126 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/types.py
--rw-r--r--   0        0        0    14411 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/utils.py
--rw-r--r--   0        0        0    11354 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/vad.py
--rw-r--r--   0        0        0     2847 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/main.py
--rw-r--r--   0        0        0     3537 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/peft_speech_inference.py
--rw-r--r--   0        0        0     1064 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/peft_speech_inference_cli.py
--rw-r--r--   0        0        0      136 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/prometheus.yml
--rw-r--r--   0        0        0      231 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/requirements.txt
--rw-r--r--   0        0        0     7667 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/speech_inference.py
--rw-r--r--   0        0        0     2451 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/speech_inference_cli.py
--rw-r--r--   0        0        0     2027 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/transcription_model.py
--rw-r--r--   0        0        0        0 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/__init__.py
--rw-r--r--   0        0        0     1910 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/audio_data_processor.py
--rw-r--r--   0        0        0     1986 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/collator.py
--rw-r--r--   0        0        0     4819 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/data_prep.py
--rw-r--r--   0        0        0     1806 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/evaluation.py
--rw-r--r--   0        0        0      688 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/gradio_demo.py
--rw-r--r--   0        0        0     6318 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/gradio_inference.py
--rw-r--r--   0        0        0     2595 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/load_data.py
--rw-r--r--   0        0        0     2592 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/main.py
--rw-r--r--   0        0        0     7356 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/model_trainer.py
--rw-r--r--   0        0        0     7952 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/wandb_callback.py
--rw-r--r--   0        0        0     4336 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/whisper_model_prep.py
--rw-r--r--   0        0        0    13625 1970-01-01 00:00:00.000000 africanwhisper-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 20:37:57.515738 africanwhisper-0.9.3/LICENSE
+-rw-r--r--   0        0        0    11066 2024-05-02 20:37:57.515738 africanwhisper-0.9.3/README.md
+-rw-r--r--   0        0        0     1248 2024-05-02 20:37:57.523738 africanwhisper-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       60 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/.dockerignore
+-rw-r--r--   0        0        0      361 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/Dockerfile
+-rw-r--r--   0        0        0        0 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/__init__.py
+-rw-r--r--   0        0        0     7479 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/app.py
+-rw-r--r--   0        0        0      538 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/docker-compose.yaml
+-rw-r--r--   0        0        0        0 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/__init__.py
+-rw-r--r--   0        0        0    18321 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/alignment.py
+-rw-r--r--   0        0        0    11001 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/asr.py
+-rw-r--r--   0        0        0     4894 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/audio.py
+-rw-r--r--   0        0        0     3276 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/diarize.py
+-rw-r--r--   0        0        0     3759 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/load_asr_model.py
+-rw-r--r--   0        0        0     4271 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/mel_filters.npz
+-rw-r--r--   0        0        0     9103 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/subtitles_processor.py
+-rw-r--r--   0        0        0     1126 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/types.py
+-rw-r--r--   0        0        0    14411 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/utils.py
+-rw-r--r--   0        0        0    11354 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/faster_whisper/vad.py
+-rw-r--r--   0        0        0     2847 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/main.py
+-rw-r--r--   0        0        0     3537 2024-05-02 20:37:57.531738 africanwhisper-0.9.3/src/deployment/peft_speech_inference.py
+-rw-r--r--   0        0        0     1064 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/peft_speech_inference_cli.py
+-rw-r--r--   0        0        0      136 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/prometheus.yml
+-rw-r--r--   0        0        0      231 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/requirements.txt
+-rw-r--r--   0        0        0     7667 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/speech_inference.py
+-rw-r--r--   0        0        0     2451 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/speech_inference_cli.py
+-rw-r--r--   0        0        0     2027 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/deployment/transcription_model.py
+-rw-r--r--   0        0        0        0 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/__init__.py
+-rw-r--r--   0        0        0     1910 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/audio_data_processor.py
+-rw-r--r--   0        0        0     1986 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/collator.py
+-rw-r--r--   0        0        0     4959 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/data_prep.py
+-rw-r--r--   0        0        0     1806 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/evaluation.py
+-rw-r--r--   0        0        0     2660 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/load_data.py
+-rw-r--r--   0        0        0     2592 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/main.py
+-rw-r--r--   0        0        0    11165 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/model_trainer.py
+-rw-r--r--   0        0        0     7952 2024-05-02 20:37:57.535738 africanwhisper-0.9.3/src/training/wandb_callback.py
+-rw-r--r--   0        0        0     4336 2024-05-02 20:37:57.539738 africanwhisper-0.9.3/src/training/whisper_model_prep.py
+-rw-r--r--   0        0        0    12823 1970-01-01 00:00:00.000000 africanwhisper-0.9.3/PKG-INFO
```

### Comparing `africanwhisper-0.9.2/LICENSE` & `africanwhisper-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/README.md` & `africanwhisper-0.9.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -141,25 +141,15 @@
 #     learning_rate (float): The learning rate for training (default is 1e-5).
 #     per_device_train_batch_size (int): The batch size per GPU for training (default is 96).
 #     per_device_eval_batch_size (int): The batch size per GPU for evaluation (default is 64).
 #     optim (str): The optimizer used for training (default is "adamw_bnb_8bit")
 
 ```
 
-## Step 6: Generate a Demo using GradioUI
-```python
-from training.gradio_inference import WhisperDemo
-
-# Generate a demo
-model_name = "your-finetuned-model-name-on-huggingface-hub"     # e.g., "KevinKibe/whisper-small-af"
-demo = WhisperDemo(model_name, huggingface_read_token)
-demo.generate_demo()
-```
-
-## Step 7: Test Model using Audio File
+## Step 6: Test Model using an Audio File
 
 ```python
 # Using a PEFT fine-tuned model
 from deployment.peft_speech_inference import SpeechInference
 
 model_name = "your-finetuned-model-name-on-huggingface-hub"   # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " "
@@ -266,24 +256,16 @@
 
 # on Windows using Chocolatey (https://chocolatey.org/)
 choco install ffmpeg
 
 # on Windows using Scoop (https://scoop.sh/)
 scoop install ffmpeg
 ```
-### To get inference on Gradio UI
-
-- To get the Gradio UI URL:
-```bash
-python -m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE 
-```
-- **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
-- **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
 
-### To get inference on CLI
+### To get inference on CLI Locally
 ```bash
 cd src/deployment
 ```
 - Create a `.env` file using `nano .env` command and add these keys and save the file.
 ```python
 MODEL_NAME = "your-finetuned-model"
 HUGGINGFACE_READ_TOKEN = "huggingface-read-token"
```

#### html2text {}

```diff
@@ -56,19 +56,15 @@
 per_device_train_batch_size=96, per_device_eval_batch_size=64,
 optim="adamw_bnb_8bit" ) # Optional parameters for training: # max_steps (int):
 The maximum number of training steps (default is 100). # learning_rate (float):
 The learning rate for training (default is 1e-5). # per_device_train_batch_size
 (int): The batch size per GPU for training (default is 96). #
 per_device_eval_batch_size (int): The batch size per GPU for evaluation
 (default is 64). # optim (str): The optimizer used for training (default is
-"adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI ```python from
-training.gradio_inference import WhisperDemo # Generate a demo model_name =
-"your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-
-small-af" demo = WhisperDemo(model_name, huggingface_read_token)
-demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python #
+"adamw_bnb_8bit") ``` ## Step 6: Test Model using an Audio File ```python #
 Using a PEFT fine-tuned model from deployment.peft_speech_inference import
 SpeechInference model_name = "your-finetuned-model-name-on-huggingface-hub" #
 e.g., "KevinKibe/whisper-small-af" huggingface_read_token = " " task =
 "desired-task" # either 'translate' or 'transcribe' audiofile_dir = "location-
 of-audio-file" # filetype should be .mp3 or .wav # Initialize the
 SpeechInference class and run inference inference = SpeechInference(model_name,
 huggingface_read_token) pipeline = inference.pipe_initialization()
@@ -111,35 +107,28 @@
 Whisper/blob/master/DOCS/PARAMETERS.md). ## Step 3: Get Inference ### Install
 ffmpeg - To get inference from your fine-tuned model, follow these steps: -
 Ensure that ffmpeg is installed by running the following commands: ```bash # on
 Ubuntu or Debian sudo apt update && sudo apt install ffmpeg # on Arch Linux
 sudo pacman -S ffmpeg # on MacOS using Homebrew (https://brew.sh/) brew install
 ffmpeg # on Windows using Chocolatey (https://chocolatey.org/) choco install
 ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop install ffmpeg ```
-### To get inference on Gradio UI - To get the Gradio UI URL: ```bash python -
-m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --
-huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE ``` - **--
-model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
-This should match the model's identifier on the Hugging Face Model Hub. - **--
-huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. ### To
-get inference on CLI ```bash cd src/deployment ``` - Create a `.env` file using
-`nano .env` command and add these keys and save the file. ```python MODEL_NAME
-= "your-finetuned-model" HUGGINGFACE_READ_TOKEN = "huggingface-read-token" ```
-- To perform transcriptions and translations: ```bash # PEFT FINETUNED MODELS
-python -m deployment.peft_speech_inference_cli --audio_file FILENAME --task
-TASK # FULLY FINETUNED MODELS python -m deployment.speech_inference_cli --
-audio_file FILENAME --task TASK --perform_diarization --perform_alignment
-Flags: # --perform_diarization: Optional flag to perform speaker diarization. #
---perform_alignment: Optional flag to perform alignment. ``` ## ð³ï¸ Step 4:
-Deployment - To deploy your fine-tuned model as a REST API endpoint, follow
-these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/
-DOCS/deployment.md). ## Contributing Contributions are welcome and encouraged.
-Before contributing, please take a moment to review our [Contribution
-Guidelines](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/
-CONTRIBUTING.md) for important information on how to contribute to this
-project. If you're unsure about anything or need assistance, don't hesitate to
-reach out to us or open an issue to discuss your ideas. We look forward to your
-contributions! ## License This project is licensed under the MIT License - see
-the [LICENSE](https://github.com/KevKibe/African-Whisper/blob/main/LICENSE)
-file for details. ## Contact For any enquiries, please reach out to me through
-keviinkibe@gmail.com
+### To get inference on CLI Locally ```bash cd src/deployment ``` - Create a
+`.env` file using `nano .env` command and add these keys and save the file.
+```python MODEL_NAME = "your-finetuned-model" HUGGINGFACE_READ_TOKEN =
+"huggingface-read-token" ``` - To perform transcriptions and translations:
+```bash # PEFT FINETUNED MODELS python -m deployment.peft_speech_inference_cli
+--audio_file FILENAME --task TASK # FULLY FINETUNED MODELS python -
+m deployment.speech_inference_cli --audio_file FILENAME --task TASK --
+perform_diarization --perform_alignment Flags: # --perform_diarization:
+Optional flag to perform speaker diarization. # --perform_alignment: Optional
+flag to perform alignment. ``` ## ð³ï¸ Step 4: Deployment - To deploy your
+fine-tuned model as a REST API endpoint, follow these [instructions](https://
+github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
+Contributing Contributions are welcome and encouraged. Before contributing,
+please take a moment to review our [Contribution Guidelines](https://
+github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for
+important information on how to contribute to this project. If you're unsure
+about anything or need assistance, don't hesitate to reach out to us or open an
+issue to discuss your ideas. We look forward to your contributions! ## License
+This project is licensed under the MIT License - see the [LICENSE](https://
+github.com/KevKibe/African-Whisper/blob/main/LICENSE) file for details. ##
+Contact For any enquiries, please reach out to me through keviinkibe@gmail.com
```

### Comparing `africanwhisper-0.9.2/pyproject.toml` & `africanwhisper-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "africanwhisper"
-version = "0.9.2"
+version = "0.9.3"
 description = "A package for fast fine-tuning and API endpoint deployment of the Whisper model, specifically developed to accelerate Automatic Speech Recognition (ASR) for African languages."
 authors = ["Kevin Kibe <keviinkibe@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/KevKibe/African-Whisper"
 packages = [
     { include = "deployment", from = "src" },
```

### Comparing `africanwhisper-0.9.2/src/deployment/app.py` & `africanwhisper-0.9.3/src/deployment/app.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/docker-compose.yaml` & `africanwhisper-0.9.3/src/deployment/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/faster_whisper/alignment.py` & `africanwhisper-0.9.3/src/deployment/faster_whisper/alignment.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/faster_whisper/asr.py` & `africanwhisper-0.9.3/src/deployment/faster_whisper/asr.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/faster_whisper/audio.py` & `africanwhisper-0.9.3/src/deployment/faster_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/faster_whisper/diarize.py` & `africanwhisper-0.9.3/src/deployment/faster_whisper/diarize.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/faster_whisper/load_asr_model.py` & `africanwhisper-0.9.3/src/deployment/faster_whisper/load_asr_model.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/faster_whisper/mel_filters.npz` & `africanwhisper-0.9.3/src/deployment/faster_whisper/mel_filters.npz`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/faster_whisper/subtitles_processor.py` & `africanwhisper-0.9.3/src/deployment/faster_whisper/subtitles_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/faster_whisper/types.py` & `africanwhisper-0.9.3/src/deployment/faster_whisper/types.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/faster_whisper/utils.py` & `africanwhisper-0.9.3/src/deployment/faster_whisper/utils.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/faster_whisper/vad.py` & `africanwhisper-0.9.3/src/deployment/faster_whisper/vad.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/main.py` & `africanwhisper-0.9.3/src/deployment/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/peft_speech_inference.py` & `africanwhisper-0.9.3/src/deployment/peft_speech_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/peft_speech_inference_cli.py` & `africanwhisper-0.9.3/src/deployment/peft_speech_inference_cli.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/speech_inference.py` & `africanwhisper-0.9.3/src/deployment/speech_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/speech_inference_cli.py` & `africanwhisper-0.9.3/src/deployment/speech_inference_cli.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/deployment/transcription_model.py` & `africanwhisper-0.9.3/src/deployment/transcription_model.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/training/audio_data_processor.py` & `africanwhisper-0.9.3/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/training/collator.py` & `africanwhisper-0.9.3/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/training/data_prep.py` & `africanwhisper-0.9.3/src/training/data_prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,16 @@
         )
 
     def load_dataset(
         self,  
         feature_extractor: WhisperFeatureExtractor, 
         tokenizer: WhisperTokenizer, 
         processor: WhisperProcessor,
-        num_samples: int = None,) -> DatasetDict:
+        train_num_samples: int = None,
+        test_num_samples: int = None) -> DatasetDict:
         """
         Retrieves and preprocesses the specified dataset for model training and evaluation.
 
         Parameters:
         feature_extractor (PreTrainedFeatureExtractor): The feature extractor instance to be used for
                                                         audio data preprocessing.
         tokenizer (PreTrainedTokenizer): The tokenizer instance for processing textual data associated
@@ -100,15 +101,16 @@
 
         Returns:
             DatasetDict: A dictionary containing the preprocessed 'train' and 'test' splits of the dataset,
                         ready for use in model training and evaluation. Each split has been cleaned and
                         processed to include only the necessary features for model input.
         """
 
-        dataset = self.data_loader.load_dataset(num_samples = num_samples)
+        dataset = self.data_loader.load_dataset(train_num_samples = train_num_samples,
+                                                test_num_samples = test_num_samples)
         print(f"Training dataset size: {self.data_loader.count_examples(dataset['train'])}")
         print(f"Test dataset size: {self.data_loader.count_examples(dataset['test'])}")
         processor = AudioDataProcessor(dataset, feature_extractor, tokenizer, processor)
         dataset['train']= dataset['train'].map(processor.resampled_dataset, remove_columns=list(next(iter(dataset['train'])).keys()))
         dataset['test']= dataset['test'].map(processor.resampled_dataset)
         return dataset
```

### Comparing `africanwhisper-0.9.2/src/training/evaluation.py` & `africanwhisper-0.9.3/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/training/load_data.py` & `africanwhisper-0.9.3/src/training/load_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,28 +23,28 @@
             dataset_name (str): Name of the dataset.
             language_abbr (str): Language abbreviation for the dataset.
         """
         self.huggingface_token = huggingface_token
         self.dataset_name = dataset_name
         self.language_abbr = language_abbr
     
-    def load_dataset(self, num_samples: int = None):
+    def load_dataset(self, train_num_samples: int = None, test_num_samples: int = None):
         """Load datasets for each language abbreviation and concatenate train/test splits.
 
         Parameters:
             num_samples(int): Number of training samples to load from each dataset eg if num_samples = 100, 200 samples, 100 from each dataset will be loaded.   
             
         Returns:
             dict: A dictionary containing concatenated train and test splits for each language.
         """
         data = {}
         for lang in self.language_abbr:
             dataset = load_dataset(self.dataset_name, lang, streaming=True, token=self.huggingface_token, trust_remote_code=True)
-            train_split = dataset['train'].take(num_samples)
-            test_split = dataset['test']
+            train_split = dataset['train'].take(train_num_samples)
+            test_split = dataset['test'].take(test_num_samples)
             if "train" in data:
                 data["train"] = concatenate_datasets([data["train"], train_split])
             else:
                 data["train"] = train_split
             if "test" in data:
                 data["test"] = concatenate_datasets([data["test"], test_split])
             else:
```

### Comparing `africanwhisper-0.9.2/src/training/main.py` & `africanwhisper-0.9.3/src/training/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/training/wandb_callback.py` & `africanwhisper-0.9.3/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/src/training/whisper_model_prep.py` & `africanwhisper-0.9.3/src/training/whisper_model_prep.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.2/PKG-INFO` & `africanwhisper-0.9.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.9.2
+Version: 0.9.3
 Summary: A package for fast fine-tuning and API endpoint deployment of the Whisper model, specifically developed to accelerate Automatic Speech Recognition (ASR) for African languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 License: MIT
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -186,25 +186,15 @@
 #     learning_rate (float): The learning rate for training (default is 1e-5).
 #     per_device_train_batch_size (int): The batch size per GPU for training (default is 96).
 #     per_device_eval_batch_size (int): The batch size per GPU for evaluation (default is 64).
 #     optim (str): The optimizer used for training (default is "adamw_bnb_8bit")
 
 ```
 
-## Step 6: Generate a Demo using GradioUI
-```python
-from training.gradio_inference import WhisperDemo
-
-# Generate a demo
-model_name = "your-finetuned-model-name-on-huggingface-hub"     # e.g., "KevinKibe/whisper-small-af"
-demo = WhisperDemo(model_name, huggingface_read_token)
-demo.generate_demo()
-```
-
-## Step 7: Test Model using Audio File
+## Step 6: Test Model using an Audio File
 
 ```python
 # Using a PEFT fine-tuned model
 from deployment.peft_speech_inference import SpeechInference
 
 model_name = "your-finetuned-model-name-on-huggingface-hub"   # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " "
@@ -311,24 +301,16 @@
 
 # on Windows using Chocolatey (https://chocolatey.org/)
 choco install ffmpeg
 
 # on Windows using Scoop (https://scoop.sh/)
 scoop install ffmpeg
 ```
-### To get inference on Gradio UI
-
-- To get the Gradio UI URL:
-```bash
-python -m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE 
-```
-- **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
-- **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
 
-### To get inference on CLI
+### To get inference on CLI Locally
 ```bash
 cd src/deployment
 ```
 - Create a `.env` file using `nano .env` command and add these keys and save the file.
 ```python
 MODEL_NAME = "your-finetuned-model"
 HUGGINGFACE_READ_TOKEN = "huggingface-read-token"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.2 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.3 Summary: A package
 for fast fine-tuning and API endpoint deployment of the Whisper model,
 specifically developed to accelerate Automatic Speech Recognition (ASR) for
 African languages. Home-page: https://github.com/KevKibe/African-Whisper
 License: MIT Author: Kevin Kibe Author-email: keviinkibe@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -80,19 +80,15 @@
 per_device_train_batch_size=96, per_device_eval_batch_size=64,
 optim="adamw_bnb_8bit" ) # Optional parameters for training: # max_steps (int):
 The maximum number of training steps (default is 100). # learning_rate (float):
 The learning rate for training (default is 1e-5). # per_device_train_batch_size
 (int): The batch size per GPU for training (default is 96). #
 per_device_eval_batch_size (int): The batch size per GPU for evaluation
 (default is 64). # optim (str): The optimizer used for training (default is
-"adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI ```python from
-training.gradio_inference import WhisperDemo # Generate a demo model_name =
-"your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-
-small-af" demo = WhisperDemo(model_name, huggingface_read_token)
-demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python #
+"adamw_bnb_8bit") ``` ## Step 6: Test Model using an Audio File ```python #
 Using a PEFT fine-tuned model from deployment.peft_speech_inference import
 SpeechInference model_name = "your-finetuned-model-name-on-huggingface-hub" #
 e.g., "KevinKibe/whisper-small-af" huggingface_read_token = " " task =
 "desired-task" # either 'translate' or 'transcribe' audiofile_dir = "location-
 of-audio-file" # filetype should be .mp3 or .wav # Initialize the
 SpeechInference class and run inference inference = SpeechInference(model_name,
 huggingface_read_token) pipeline = inference.pipe_initialization()
@@ -135,35 +131,28 @@
 Whisper/blob/master/DOCS/PARAMETERS.md). ## Step 3: Get Inference ### Install
 ffmpeg - To get inference from your fine-tuned model, follow these steps: -
 Ensure that ffmpeg is installed by running the following commands: ```bash # on
 Ubuntu or Debian sudo apt update && sudo apt install ffmpeg # on Arch Linux
 sudo pacman -S ffmpeg # on MacOS using Homebrew (https://brew.sh/) brew install
 ffmpeg # on Windows using Chocolatey (https://chocolatey.org/) choco install
 ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop install ffmpeg ```
-### To get inference on Gradio UI - To get the Gradio UI URL: ```bash python -
-m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --
-huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE ``` - **--
-model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
-This should match the model's identifier on the Hugging Face Model Hub. - **--
-huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face. ### To
-get inference on CLI ```bash cd src/deployment ``` - Create a `.env` file using
-`nano .env` command and add these keys and save the file. ```python MODEL_NAME
-= "your-finetuned-model" HUGGINGFACE_READ_TOKEN = "huggingface-read-token" ```
-- To perform transcriptions and translations: ```bash # PEFT FINETUNED MODELS
-python -m deployment.peft_speech_inference_cli --audio_file FILENAME --task
-TASK # FULLY FINETUNED MODELS python -m deployment.speech_inference_cli --
-audio_file FILENAME --task TASK --perform_diarization --perform_alignment
-Flags: # --perform_diarization: Optional flag to perform speaker diarization. #
---perform_alignment: Optional flag to perform alignment. ``` ## ð³ï¸ Step 4:
-Deployment - To deploy your fine-tuned model as a REST API endpoint, follow
-these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/
-DOCS/deployment.md). ## Contributing Contributions are welcome and encouraged.
-Before contributing, please take a moment to review our [Contribution
-Guidelines](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/
-CONTRIBUTING.md) for important information on how to contribute to this
-project. If you're unsure about anything or need assistance, don't hesitate to
-reach out to us or open an issue to discuss your ideas. We look forward to your
-contributions! ## License This project is licensed under the MIT License - see
-the [LICENSE](https://github.com/KevKibe/African-Whisper/blob/main/LICENSE)
-file for details. ## Contact For any enquiries, please reach out to me through
-keviinkibe@gmail.com
+### To get inference on CLI Locally ```bash cd src/deployment ``` - Create a
+`.env` file using `nano .env` command and add these keys and save the file.
+```python MODEL_NAME = "your-finetuned-model" HUGGINGFACE_READ_TOKEN =
+"huggingface-read-token" ``` - To perform transcriptions and translations:
+```bash # PEFT FINETUNED MODELS python -m deployment.peft_speech_inference_cli
+--audio_file FILENAME --task TASK # FULLY FINETUNED MODELS python -
+m deployment.speech_inference_cli --audio_file FILENAME --task TASK --
+perform_diarization --perform_alignment Flags: # --perform_diarization:
+Optional flag to perform speaker diarization. # --perform_alignment: Optional
+flag to perform alignment. ``` ## ð³ï¸ Step 4: Deployment - To deploy your
+fine-tuned model as a REST API endpoint, follow these [instructions](https://
+github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
+Contributing Contributions are welcome and encouraged. Before contributing,
+please take a moment to review our [Contribution Guidelines](https://
+github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for
+important information on how to contribute to this project. If you're unsure
+about anything or need assistance, don't hesitate to reach out to us or open an
+issue to discuss your ideas. We look forward to your contributions! ## License
+This project is licensed under the MIT License - see the [LICENSE](https://
+github.com/KevKibe/African-Whisper/blob/main/LICENSE) file for details. ##
+Contact For any enquiries, please reach out to me through keviinkibe@gmail.com
```

