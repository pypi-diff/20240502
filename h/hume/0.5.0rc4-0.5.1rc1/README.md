# Comparing `tmp/hume-0.5.0rc4.tar.gz` & `tmp/hume-0.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hume-0.5.0rc4.tar", max compression
+gzip compressed data, was "hume-0.5.1rc1.tar", max compression
```

## Comparing `hume-0.5.0rc4.tar` & `hume-0.5.1rc1.tar`

### file list

```diff
@@ -1,56 +1,58 @@
--rw-r--r--   0        0        0     1070 2023-06-29 18:23:24.716306 hume-0.5.0rc4/LICENSE
--rw-r--r--   0        0        0     2256 2024-04-16 17:05:53.964549 hume-0.5.0rc4/README.md
--rw-r--r--   0        0        0      824 2024-04-23 08:46:40.806342 hume-0.5.0rc4/hume/__init__.py
--rw-r--r--   0        0        0       19 2023-06-29 18:23:24.724774 hume-0.5.0rc4/hume/_common/__init__.py
--rw-r--r--   0        0        0     4853 2024-04-23 08:07:03.239984 hume-0.5.0rc4/hume/_common/client_base.py
--rw-r--r--   0        0        0     1804 2024-04-08 23:00:47.349405 hume-0.5.0rc4/hume/_common/config_base.py
--rw-r--r--   0        0        0      121 2024-04-09 04:12:04.402577 hume-0.5.0rc4/hume/_common/protocol.py
--rw-r--r--   0        0        0       19 2024-04-08 23:37:14.346157 hume-0.5.0rc4/hume/_common/utilities/__init__.py
--rw-r--r--   0        0        0     2320 2024-04-08 23:37:14.348937 hume-0.5.0rc4/hume/_common/utilities/config_utilities.py
--rw-r--r--   0        0        0      291 2024-04-09 04:20:34.829615 hume-0.5.0rc4/hume/_common/utilities/model_utilities.py
--rw-r--r--   0        0        0      215 2024-04-09 04:20:36.584244 hume-0.5.0rc4/hume/_common/utilities/paging_utilities.py
--rw-r--r--   0        0        0     3545 2024-04-08 23:37:14.349713 hume-0.5.0rc4/hume/_common/utilities/retry_utilities.py
--rw-r--r--   0        0        0       58 2024-04-09 04:12:04.403581 hume-0.5.0rc4/hume/_common/utilities/typing_utilities.py
--rw-r--r--   0        0        0       19 2024-04-08 22:57:09.806665 hume-0.5.0rc4/hume/_measurement/__init__.py
--rw-r--r--   0        0        0      573 2024-04-08 22:57:09.806941 hume-0.5.0rc4/hume/_measurement/batch/__init__.py
--rw-r--r--   0        0        0     4387 2024-04-08 22:57:09.807530 hume-0.5.0rc4/hume/_measurement/batch/batch_job.py
--rw-r--r--   0        0        0     6046 2024-04-08 22:57:09.807740 hume-0.5.0rc4/hume/_measurement/batch/batch_job_details.py
--rw-r--r--   0        0        0      643 2024-04-08 22:57:09.807893 hume-0.5.0rc4/hume/_measurement/batch/batch_job_state.py
--rw-r--r--   0        0        0      994 2024-04-08 23:00:47.349544 hume-0.5.0rc4/hume/_measurement/batch/batch_job_status.py
--rw-r--r--   0        0        0    10353 2024-04-09 04:20:39.402038 hume-0.5.0rc4/hume/_measurement/batch/hume_batch_client.py
--rw-r--r--   0        0        0      940 2024-04-08 23:00:47.349881 hume-0.5.0rc4/hume/_measurement/batch/transcription_config.py
--rw-r--r--   0        0        0      216 2024-04-08 22:57:09.808459 hume-0.5.0rc4/hume/_measurement/stream/__init__.py
--rw-r--r--   0        0        0     3288 2024-04-09 04:12:04.404187 hume-0.5.0rc4/hume/_measurement/stream/hume_stream_client.py
--rw-r--r--   0        0        0     9411 2024-04-09 03:27:28.257593 hume-0.5.0rc4/hume/_measurement/stream/stream_socket.py
--rw-r--r--   0        0        0      435 2024-04-23 08:46:40.806650 hume-0.5.0rc4/hume/_voice/__init__.py
--rw-r--r--   0        0        0      363 2024-04-23 08:46:41.019929 hume-0.5.0rc4/hume/_voice/hume_voice_client.py
--rw-r--r--   0        0        0       19 2024-04-18 07:05:31.675674 hume-0.5.0rc4/hume/_voice/microphone/__init__.py
--rw-r--r--   0        0        0     1371 2024-04-23 08:46:41.020172 hume-0.5.0rc4/hume/_voice/microphone/asyncio_utilities.py
--rw-r--r--   0        0        0      728 2024-04-23 08:46:41.020466 hume-0.5.0rc4/hume/_voice/microphone/audio_utilities.py
--rw-r--r--   0        0        0     2976 2024-04-23 08:46:41.242380 hume-0.5.0rc4/hume/_voice/microphone/chat_client.py
--rw-r--r--   0        0        0     3350 2024-04-23 08:46:41.181842 hume-0.5.0rc4/hume/_voice/microphone/microphone.py
--rw-r--r--   0        0        0     1667 2024-04-23 08:46:41.242633 hume-0.5.0rc4/hume/_voice/microphone/microphone_interface.py
--rw-r--r--   0        0        0     2001 2024-04-23 08:46:41.242806 hume-0.5.0rc4/hume/_voice/microphone/microphone_sender.py
--rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676175 hume-0.5.0rc4/hume/_voice/mixins/__init__.py
--rw-r--r--   0        0        0     2017 2024-04-23 08:46:41.243072 hume-0.5.0rc4/hume/_voice/mixins/chat_mixin.py
--rw-r--r--   0        0        0     2841 2024-04-23 08:46:41.021491 hume-0.5.0rc4/hume/_voice/mixins/chats_mixin.py
--rw-r--r--   0        0        0     4960 2024-04-23 08:46:41.243382 hume-0.5.0rc4/hume/_voice/mixins/configs_mixin.py
--rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676663 hume-0.5.0rc4/hume/_voice/models/__init__.py
--rw-r--r--   0        0        0     2608 2024-04-23 08:46:41.021941 hume-0.5.0rc4/hume/_voice/models/chats_models.py
--rw-r--r--   0        0        0     1916 2024-04-23 08:46:41.243661 hume-0.5.0rc4/hume/_voice/models/configs_models.py
--rw-r--r--   0        0        0      461 2024-04-23 08:46:41.243897 hume-0.5.0rc4/hume/_voice/session_settings.py
--rw-r--r--   0        0        0     2814 2024-04-23 10:05:14.835518 hume-0.5.0rc4/hume/_voice/voice_socket.py
--rw-r--r--   0        0        0       19 2023-06-29 18:23:24.726173 hume-0.5.0rc4/hume/error/__init__.py
--rw-r--r--   0        0        0      571 2023-11-09 21:00:40.007182 hume-0.5.0rc4/hume/error/hume_client_exception.py
--rw-r--r--   0        0        0       97 2024-04-08 23:00:47.350438 hume-0.5.0rc4/hume/models/__init__.py
--rw-r--r--   0        0        0      588 2024-04-08 23:00:47.350573 hume-0.5.0rc4/hume/models/config/__init__.py
--rw-r--r--   0        0        0      498 2024-04-08 23:00:47.350848 hume-0.5.0rc4/hume/models/config/burst_config.py
--rw-r--r--   0        0        0     2574 2024-04-08 23:00:47.351014 hume-0.5.0rc4/hume/models/config/face_config.py
--rw-r--r--   0        0        0      510 2024-04-08 23:00:47.351168 hume-0.5.0rc4/hume/models/config/facemesh_config.py
--rw-r--r--   0        0        0     2236 2024-04-08 23:00:47.351315 hume-0.5.0rc4/hume/models/config/language_config.py
--rw-r--r--   0        0        0      632 2024-04-08 23:00:47.351466 hume-0.5.0rc4/hume/models/config/model_config_base.py
--rw-r--r--   0        0        0     1001 2024-04-08 23:00:47.351600 hume-0.5.0rc4/hume/models/config/ner_config.py
--rw-r--r--   0        0        0     1786 2024-04-08 23:00:47.351778 hume-0.5.0rc4/hume/models/config/prosody_config.py
--rw-r--r--   0        0        0      805 2024-04-08 23:00:47.351947 hume-0.5.0rc4/hume/models/model_type.py
--rw-r--r--   0        0        0     2783 2024-04-23 10:56:06.250670 hume-0.5.0rc4/pyproject.toml
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 hume-0.5.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-29 18:23:24.716306 hume-0.5.1rc1/LICENSE
+-rw-r--r--   0        0        0     2256 2024-04-16 17:05:53.964549 hume-0.5.1rc1/README.md
+-rw-r--r--   0        0        0      985 2024-04-30 12:10:05.693231 hume-0.5.1rc1/hume/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-29 18:23:24.724774 hume-0.5.1rc1/hume/_common/__init__.py
+-rw-r--r--   0        0        0     4907 2024-04-30 13:04:16.986600 hume-0.5.1rc1/hume/_common/client_base.py
+-rw-r--r--   0        0        0     1804 2024-04-08 23:00:47.349405 hume-0.5.1rc1/hume/_common/config_base.py
+-rw-r--r--   0        0        0      121 2024-04-09 04:12:04.402577 hume-0.5.1rc1/hume/_common/protocol.py
+-rw-r--r--   0        0        0       19 2024-04-08 23:37:14.346157 hume-0.5.1rc1/hume/_common/utilities/__init__.py
+-rw-r--r--   0        0        0     2320 2024-04-08 23:37:14.348937 hume-0.5.1rc1/hume/_common/utilities/config_utilities.py
+-rw-r--r--   0        0        0      291 2024-04-09 04:20:34.829615 hume-0.5.1rc1/hume/_common/utilities/model_utilities.py
+-rw-r--r--   0        0        0      215 2024-04-09 04:20:36.584244 hume-0.5.1rc1/hume/_common/utilities/paging_utilities.py
+-rw-r--r--   0        0        0     3545 2024-04-08 23:37:14.349713 hume-0.5.1rc1/hume/_common/utilities/retry_utilities.py
+-rw-r--r--   0        0        0       58 2024-04-09 04:12:04.403581 hume-0.5.1rc1/hume/_common/utilities/typing_utilities.py
+-rw-r--r--   0        0        0       19 2024-04-08 22:57:09.806665 hume-0.5.1rc1/hume/_measurement/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-08 22:57:09.806941 hume-0.5.1rc1/hume/_measurement/batch/__init__.py
+-rw-r--r--   0        0        0     4387 2024-04-08 22:57:09.807530 hume-0.5.1rc1/hume/_measurement/batch/batch_job.py
+-rw-r--r--   0        0        0     6046 2024-04-08 22:57:09.807740 hume-0.5.1rc1/hume/_measurement/batch/batch_job_details.py
+-rw-r--r--   0        0        0      643 2024-04-08 22:57:09.807893 hume-0.5.1rc1/hume/_measurement/batch/batch_job_state.py
+-rw-r--r--   0        0        0      994 2024-04-08 23:00:47.349544 hume-0.5.1rc1/hume/_measurement/batch/batch_job_status.py
+-rw-r--r--   0        0        0    10353 2024-04-09 04:20:39.402038 hume-0.5.1rc1/hume/_measurement/batch/hume_batch_client.py
+-rw-r--r--   0        0        0      940 2024-04-08 23:00:47.349881 hume-0.5.1rc1/hume/_measurement/batch/transcription_config.py
+-rw-r--r--   0        0        0      216 2024-04-08 22:57:09.808459 hume-0.5.1rc1/hume/_measurement/stream/__init__.py
+-rw-r--r--   0        0        0     3288 2024-04-09 04:12:04.404187 hume-0.5.1rc1/hume/_measurement/stream/hume_stream_client.py
+-rw-r--r--   0        0        0     9411 2024-04-09 03:27:28.257593 hume-0.5.1rc1/hume/_measurement/stream/stream_socket.py
+-rw-r--r--   0        0        0      602 2024-04-30 12:09:39.889889 hume-0.5.1rc1/hume/_voice/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-29 19:31:03.047474 hume-0.5.1rc1/hume/_voice/hume_voice_client.py
+-rw-r--r--   0        0        0       19 2024-04-24 21:46:26.078781 hume-0.5.1rc1/hume/_voice/microphone/__init__.py
+-rw-r--r--   0        0        0     1371 2024-04-24 21:46:26.079063 hume-0.5.1rc1/hume/_voice/microphone/asyncio_utilities.py
+-rw-r--r--   0        0        0      728 2024-04-24 21:46:26.079508 hume-0.5.1rc1/hume/_voice/microphone/audio_utilities.py
+-rw-r--r--   0        0        0     3652 2024-05-02 12:12:57.948714 hume-0.5.1rc1/hume/_voice/microphone/chat_client.py
+-rw-r--r--   0        0        0     3350 2024-04-24 21:46:26.080119 hume-0.5.1rc1/hume/_voice/microphone/microphone.py
+-rw-r--r--   0        0        0     1667 2024-04-24 21:46:26.080399 hume-0.5.1rc1/hume/_voice/microphone/microphone_interface.py
+-rw-r--r--   0        0        0     2925 2024-05-02 12:27:07.229612 hume-0.5.1rc1/hume/_voice/microphone/microphone_sender.py
+-rw-r--r--   0        0        0       19 2024-04-24 21:46:26.080728 hume-0.5.1rc1/hume/_voice/mixins/__init__.py
+-rw-r--r--   0        0        0     2017 2024-04-24 21:46:26.081139 hume-0.5.1rc1/hume/_voice/mixins/chat_mixin.py
+-rw-r--r--   0        0        0     2841 2024-04-24 21:46:26.081459 hume-0.5.1rc1/hume/_voice/mixins/chats_mixin.py
+-rw-r--r--   0        0        0     5337 2024-04-30 12:07:23.305131 hume-0.5.1rc1/hume/_voice/mixins/configs_mixin.py
+-rw-r--r--   0        0        0     4289 2024-04-30 12:10:17.367400 hume-0.5.1rc1/hume/_voice/mixins/tools_mixin.py
+-rw-r--r--   0        0        0       19 2024-04-24 21:46:26.082013 hume-0.5.1rc1/hume/_voice/models/__init__.py
+-rw-r--r--   0        0        0     2608 2024-04-24 21:46:26.082284 hume-0.5.1rc1/hume/_voice/models/chats_models.py
+-rw-r--r--   0        0        0     2425 2024-05-02 12:19:24.347700 hume-0.5.1rc1/hume/_voice/models/configs_models.py
+-rw-r--r--   0        0        0     1140 2024-04-30 11:49:55.154292 hume-0.5.1rc1/hume/_voice/models/tools_models.py
+-rw-r--r--   0        0        0      461 2024-04-24 21:46:26.083048 hume-0.5.1rc1/hume/_voice/session_settings.py
+-rw-r--r--   0        0        0     3192 2024-05-02 12:32:05.859932 hume-0.5.1rc1/hume/_voice/voice_socket.py
+-rw-r--r--   0        0        0       19 2023-06-29 18:23:24.726173 hume-0.5.1rc1/hume/error/__init__.py
+-rw-r--r--   0        0        0      571 2023-11-09 21:00:40.007182 hume-0.5.1rc1/hume/error/hume_client_exception.py
+-rw-r--r--   0        0        0       97 2024-04-08 23:00:47.350438 hume-0.5.1rc1/hume/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-04-08 23:00:47.350573 hume-0.5.1rc1/hume/models/config/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-08 23:00:47.350848 hume-0.5.1rc1/hume/models/config/burst_config.py
+-rw-r--r--   0        0        0     2574 2024-04-08 23:00:47.351014 hume-0.5.1rc1/hume/models/config/face_config.py
+-rw-r--r--   0        0        0      510 2024-04-08 23:00:47.351168 hume-0.5.1rc1/hume/models/config/facemesh_config.py
+-rw-r--r--   0        0        0     2236 2024-04-08 23:00:47.351315 hume-0.5.1rc1/hume/models/config/language_config.py
+-rw-r--r--   0        0        0      632 2024-04-08 23:00:47.351466 hume-0.5.1rc1/hume/models/config/model_config_base.py
+-rw-r--r--   0        0        0     1001 2024-04-08 23:00:47.351600 hume-0.5.1rc1/hume/models/config/ner_config.py
+-rw-r--r--   0        0        0     1786 2024-04-08 23:00:47.351778 hume-0.5.1rc1/hume/models/config/prosody_config.py
+-rw-r--r--   0        0        0      805 2024-04-08 23:00:47.351947 hume-0.5.1rc1/hume/models/model_type.py
+-rw-r--r--   0        0        0     2640 2024-05-02 12:34:26.254311 hume-0.5.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 hume-0.5.1rc1/PKG-INFO
```

### Comparing `hume-0.5.0rc4/LICENSE` & `hume-0.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/README.md` & `hume-0.5.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/__init__.py` & `hume-0.5.1rc1/hume/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,29 +7,41 @@
     BatchJobDetails,
     BatchJobState,
     BatchJobStatus,
     HumeBatchClient,
     TranscriptionConfig,
 )
 from hume._measurement.stream import HumeStreamClient, StreamSocket
-from hume._voice import HumeVoiceClient, MicrophoneInterface, VoiceChat, VoiceConfig, VoiceSocket
+from hume._voice import (
+    HumeVoiceClient,
+    LanguageModelConfig,
+    MicrophoneInterface,
+    VoiceChat,
+    VoiceConfig,
+    VoiceIdentityConfig,
+    VoiceSocket,
+    VoiceTool,
+)
 from hume.error.hume_client_exception import HumeClientException
 
 __version__ = version("hume")
 
 __all__ = [
     "__version__",
     "BatchJob",
     "BatchJobDetails",
     "BatchJobState",
     "BatchJobStatus",
     "HumeBatchClient",
     "HumeClientException",
     "HumeStreamClient",
     "HumeVoiceClient",
+    "LanguageModelConfig",
     "MicrophoneInterface",
     "StreamSocket",
     "TranscriptionConfig",
     "VoiceChat",
     "VoiceConfig",
+    "VoiceIdentityConfig",
     "VoiceSocket",
+    "VoiceTool",
 ]
```

### Comparing `hume-0.5.0rc4/hume/_common/client_base.py` & `hume-0.5.1rc1/hume/_common/client_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,16 @@
             headers=headers,
         )
 
         try:
             response = self._http_client.send(request)
             response.raise_for_status()
         except Exception as exc:  # pylint: disable=broad-exception-caught
-            raise HumeClientException(str(exc)) from exc
+            response_body = response.json()
+            raise HumeClientException(str(response_body)) from exc
 
         return response
 
     def _get_client_headers(self) -> Dict[str, str]:
         return {
             "X-Hume-Api-Key": self._api_key,
             "X-Hume-Client-Name": "python_sdk",
```

### Comparing `hume-0.5.0rc4/hume/_common/config_base.py` & `hume-0.5.1rc1/hume/_common/config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_common/utilities/config_utilities.py` & `hume-0.5.1rc1/hume/_common/utilities/config_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_common/utilities/retry_utilities.py` & `hume-0.5.1rc1/hume/_common/utilities/retry_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_measurement/batch/__init__.py` & `hume-0.5.1rc1/hume/_measurement/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_measurement/batch/batch_job.py` & `hume-0.5.1rc1/hume/_measurement/batch/batch_job.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_measurement/batch/batch_job_details.py` & `hume-0.5.1rc1/hume/_measurement/batch/batch_job_details.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_measurement/batch/batch_job_state.py` & `hume-0.5.1rc1/hume/_measurement/batch/batch_job_state.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_measurement/batch/batch_job_status.py` & `hume-0.5.1rc1/hume/_measurement/batch/batch_job_status.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_measurement/batch/hume_batch_client.py` & `hume-0.5.1rc1/hume/_measurement/batch/hume_batch_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_measurement/batch/transcription_config.py` & `hume-0.5.1rc1/hume/_measurement/batch/transcription_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_measurement/stream/hume_stream_client.py` & `hume-0.5.1rc1/hume/_measurement/stream/hume_stream_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_measurement/stream/stream_socket.py` & `hume-0.5.1rc1/hume/_measurement/stream/stream_socket.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_voice/microphone/asyncio_utilities.py` & `hume-0.5.1rc1/hume/_voice/microphone/asyncio_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_voice/microphone/audio_utilities.py` & `hume-0.5.1rc1/hume/_voice/microphone/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_voice/microphone/chat_client.py` & `hume-0.5.1rc1/hume/_voice/microphone/chat_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     def _map_role(cls, role: str) -> str:
         if role == "user":
             return cls.DEFAULT_USER_ROLE_NAME
         if role == "assistant":
             return cls.DEFAULT_ASSISTANT_ROLE_NAME
         return role
 
+    def _print_prompt(self, text: str) -> None:
+        now = datetime.datetime.now(tz=datetime.timezone.utc)
+        now_str = now.strftime("%H:%M:%S")
+        print(f"[{now_str}] {text}")
+
     async def _recv(self, *, socket: VoiceSocket) -> None:
         async for socket_message in socket:
             message = json.loads(socket_message)
             if message["type"] in ["user_message", "assistant_message"]:
                 role = self._map_role(message["message"]["role"])
                 message_text = message["message"]["content"]
                 text = f"{role}: {message_text}"
@@ -56,22 +61,30 @@
                 message_bytes = base64.b64decode(message_str.encode("utf-8"))
                 await self.byte_strs.put(message_bytes)
                 continue
             elif message["type"] == "error":
                 error_message: str = message["message"]
                 error_code: str = message["code"]
                 raise HumeClientException(f"Error ({error_code}): {error_message}")
+            elif message["type"] == "tool_call":
+                print(
+                    "Warning: EVI is trying to make a tool call. "
+                    "Either remove tool calling from your config or "
+                    "use the VoiceSocket directly without a MicrophoneInterface."
+                )
+                tool_call_id = message["tool_call_id"]
+                if message["response_required"]:
+                    content = "Let's start over"
+                    await self.sender.send_tool_response(socket=socket, tool_call_id=tool_call_id, content=content)
+                continue
             else:
                 message_type = message["type"].upper()
                 text = f"<{message_type}>"
 
-            now = datetime.datetime.now(tz=datetime.timezone.utc)
-            now_str = now.strftime("%H:%M:%S")
-
-            print(f"[{now_str}] {text}")
+            self._print_prompt(text)
 
     async def _play(self) -> None:
         async for byte_str in self.byte_strs:
             await self.sender.on_audio_begin()
             await play_audio(byte_str)
             await self.sender.on_audio_end()
```

### Comparing `hume-0.5.0rc4/hume/_voice/microphone/microphone.py` & `hume-0.5.1rc1/hume/_voice/microphone/microphone.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_voice/microphone/microphone_interface.py` & `hume-0.5.1rc1/hume/_voice/microphone/microphone_interface.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_voice/mixins/chat_mixin.py` & `hume-0.5.1rc1/hume/_voice/mixins/chat_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_voice/mixins/chats_mixin.py` & `hume-0.5.1rc1/hume/_voice/mixins/chats_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_voice/mixins/configs_mixin.py` & `hume-0.5.1rc1/hume/_voice/mixins/configs_mixin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Client operations for managing EVI configurations."""
 
 import logging
-from typing import Iterator, Optional
+from typing import Iterator, List, Optional
 
 from hume._common.client_base import ClientBase
 from hume._common.utilities.paging_utilities import Paging
 from hume._voice.models.configs_models import (
     ConfigResponse,
     ConfigsResponse,
+    LanguageModelConfig,
     PostConfigRequest,
     PostPromptRequest,
     PromptMeta,
     PromptResponse,
     VoiceConfig,
     VoiceIdentityConfig,
 )
+from hume._voice.models.tools_models import ToolMeta, VoiceTool
 from hume.error.hume_client_exception import HumeClientException
 
 logger = logging.getLogger(__name__)
 
 
 # pylint: disable=redefined-builtin
 class ConfigsMixin(ClientBase):
@@ -28,15 +30,17 @@
 
     def create_config(
         self,
         *,
         name: str,
         prompt: str,
         description: Optional[str] = None,
-        voice_name: Optional[str] = DEFAULT_VOICE_NAME,
+        voice_identity_config: Optional[VoiceIdentityConfig] = None,
+        tools: Optional[List[VoiceTool]] = None,
+        language_model: Optional[LanguageModelConfig] = None,
     ) -> VoiceConfig:
         """Create a new EVI config.
 
         Args:
             name (str): Config name.
             prompt (str): System prompt text.
             description (Optional[str]): Config description.
@@ -44,19 +48,22 @@
         post_prompt_request = PostPromptRequest(name=name, version_description=description, text=prompt)
         post_prompt_body = post_prompt_request.to_json_str()
         endpoint = self._build_endpoint("evi", "prompts")
         response = self._request(endpoint, method="POST", body_json_str=post_prompt_body)
         prompt_response = PromptResponse.model_validate_json(response.text)
         prompt_meta = PromptMeta(id=prompt_response.id, version=prompt_response.version)
 
+        tool_metas = None if tools is None else [ToolMeta(id=tool.id, version=0) for tool in tools]
         post_config_request = PostConfigRequest(
             name=name,
             version_description=description,
             prompt=prompt_meta,
-            voice=VoiceIdentityConfig(name=voice_name),
+            voice=voice_identity_config,
+            tools=tool_metas,
+            language_model=language_model,
         )
         post_config_body = post_config_request.to_json_str()
         endpoint = self._build_endpoint("evi", "configs")
         response = self._request(endpoint, method="POST", body_json_str=post_config_body)
         config_response = ConfigResponse.model_validate_json(response.text)
 
         return self._config_from_response(config_response)
```

### Comparing `hume-0.5.0rc4/hume/_voice/models/chats_models.py` & `hume-0.5.1rc1/hume/_voice/models/chats_models.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/_voice/models/configs_models.py` & `hume-0.5.1rc1/hume/_voice/models/configs_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """API request and response models for EVI configurations."""
 
 from typing import List, Optional
 
 from hume._common.utilities.model_utilities import BaseModel
+from hume._voice.models.tools_models import ToolMeta
 
 
 class PromptResponse(BaseModel):
     """Response model for an EVI prompt."""
 
     id: str
     version: int
@@ -28,14 +29,22 @@
 class PromptMeta(BaseModel):
     """Prompt metadata."""
 
     id: str
     version: int
 
 
+class LanguageModelConfig(BaseModel):
+    """Language model configuration for EVI."""
+
+    model_provider: str
+    model_resource: str
+    temperature: Optional[float] = None
+
+
 class PostPromptRequest(BaseModel):
     """Post request model for creating a new EVI prompt."""
 
     name: str
     version_description: Optional[str]
     text: Optional[str]
 
@@ -63,21 +72,31 @@
 class VoiceIdentityConfig(BaseModel):
     """Configuration for changing the voice of EVI."""
 
     provider: Optional[str] = None
     name: Optional[str] = None
 
 
+class BuiltinToolConfig(BaseModel):
+    """Configuration for a built-in EVI tool."""
+
+    name: str
+    tool_type: str
+    fallback_content: Optional[str]
+
+
 class PostConfigRequest(BaseModel):
     """Post request model for creating a new EVI configuration."""
 
     name: str
     version_description: Optional[str]
     prompt: PromptMeta
-    voice: VoiceIdentityConfig
+    voice: Optional[VoiceIdentityConfig]
+    language_model: Optional[LanguageModelConfig]
+    tools: Optional[List[ToolMeta]]
 
 
 class ConfigMeta(BaseModel):
     """EVI configuration metadata."""
 
     id: Optional[str]
     version: Optional[int]
@@ -87,8 +106,9 @@
     """EVI configuration."""
 
     id: str
     name: str
     description: Optional[str]
     created_on: int
     modified_on: int
+    # TODO: Add tool info
     prompt: Optional[str]
```

### Comparing `hume-0.5.0rc4/hume/_voice/voice_socket.py` & `hume-0.5.1rc1/hume/_voice/voice_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 from pathlib import Path
 from typing import Any, AsyncIterator, ClassVar, Optional
 
 from pydub import AudioSegment
 from websockets.client import WebSocketClientProtocol as WebSocket
 
+from hume._common.utilities.typing_utilities import JsonObject
 from hume._voice.session_settings import AudioSettings, SessionSettings
 
 logger = logging.getLogger(__name__)
 
 
 class VoiceSocket:
     """Voice socket connection."""
@@ -43,14 +44,22 @@
         """Send a byte string over the voice socket.
 
         Args:
             byte_str (bytes): Byte string to send.
         """
         await self._protocol.send(byte_str)
 
+    async def send_json(self, message: JsonObject) -> None:
+        """Send JSON as a byte string over the voice socket.
+
+        Args:
+            message (JsonObject): A dictionary representing a full JSON payload to the server.
+        """
+        await self._protocol.send(json.dumps(message).encode("utf-8"))
+
     async def recv(self) -> Any:
         """Receive a message on the voice socket."""
         await self._protocol.recv()
 
     async def update_session_settings(
         self,
         *,
```

### Comparing `hume-0.5.0rc4/hume/error/hume_client_exception.py` & `hume-0.5.1rc1/hume/error/hume_client_exception.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/models/config/__init__.py` & `hume-0.5.1rc1/hume/models/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/models/config/face_config.py` & `hume-0.5.1rc1/hume/models/config/face_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/models/config/language_config.py` & `hume-0.5.1rc1/hume/models/config/language_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/models/config/model_config_base.py` & `hume-0.5.1rc1/hume/models/config/model_config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/models/config/ner_config.py` & `hume-0.5.1rc1/hume/models/config/ner_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/models/config/prosody_config.py` & `hume-0.5.1rc1/hume/models/config/prosody_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/hume/models/model_type.py` & `hume-0.5.1rc1/hume/models/model_type.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.0rc4/pyproject.toml` & `hume-0.5.1rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   "communication",
   "learning",
 ]
 license = "Proprietary"
 name = "hume"
 readme = "README.md"
 repository = "https://github.com/HumeAI/hume-python-sdk"
-version = "0.5.0rc4"
+version = "0.5.1rc1"
 
 [tool.poetry.dependencies]
 httpx = { extras = ["http2"], version = "^0.27.0" }
 jupyter = { version = "^1.0.0", optional = true }
 pydantic = "^2.6.4"
 pydub = "^0.25.1"
 python = ">=3.9,<4"
@@ -46,20 +46,18 @@
 sounddevice = { version = "^0.4.6", optional = true }
 typing-extensions = "^4.3.0"
 websockets = "^12.0"
 
 [tool.poetry.dev-dependencies]
 black = "^24.4.0"
 covcheck = { version = "^0.4.3", extras = ["toml"] }
-flake8 = "^6.0.0"
 ipykernel = "^6.22.0"
 mypy = "^1.0.1"
 pydocstyle = "^6.1.1"
 pylint = "^2.16.2"
-pyproject-flake8 = "^6.0.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.19.0"
 pytest-cov = "^4.0.0"
 pytest-forked = "^1.4.0"
 pytest-xdist = "^2.5.0"
 semver = "^2.13.0"
 testbook = "^0.4.2"
@@ -84,25 +82,21 @@
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.black]
 line-length = 120
 
 [tool.covcheck.group.unit.coverage]
-branch = 49.0
-line = 72.0
+branch = 45.0
+line = 71.0
 
 [tool.covcheck.group.service.coverage]
 branch = 57.0
 line = 80.0
 
-[tool.flake8]
-ignore = ""           # Required to disable default ignores
-max-line-length = 120
-
 [tool.isort]
 line_length = 120
 profile = "black"
 src_paths = "*"
 
 [tool.mypy]
 disallow_incomplete_defs = true
```

### Comparing `hume-0.5.0rc4/PKG-INFO` & `hume-0.5.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hume
-Version: 0.5.0rc4
+Version: 0.5.1rc1
 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk
 License: Proprietary
 Keywords: hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev
 Author-email: dev@hume.ai
 Requires-Python: >=3.9,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hume Version: 0.5.0rc4 Summary: Hume AI Python SDK
+Metadata-Version: 2.1 Name: hume Version: 0.5.1rc1 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk License: Proprietary
 Keywords:
 hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev Author-email: dev@hume.ai Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

