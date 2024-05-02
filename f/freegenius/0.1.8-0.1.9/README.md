# Comparing `tmp/freegenius-0.1.8.tar.gz` & `tmp/freegenius-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.1.8.tar", last modified: Sun Apr 28 21:39:08 2024, max compression
+gzip compressed data, was "freegenius-0.1.9.tar", last modified: Thu May  2 18:52:19 2024, max compression
```

## Comparing `freegenius-0.1.8.tar` & `freegenius-0.1.9.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.818296 freegenius-0.1.8/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-04-28 21:39:08.818296 freegenius-0.1.8/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.786296 freegenius-0.1.8/freegenius/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11766 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.1.8/freegenius/__init__.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.790296 freegenius-0.1.8/freegenius/audio/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.1.8/freegenius/audio/notification1.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.1.8/freegenius/audio/notification1_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.1.8/freegenius/audio/notification2.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.1.8/freegenius/audio/notification2_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7006 2024-04-28 21:17:47.000000 freegenius-0.1.8/freegenius/autoassist.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.1.8/freegenius/autobuilder.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11081 2024-04-28 21:19:22.000000 freegenius-0.1.8/freegenius/autoretriever.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.1.8/freegenius/chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.1.8/freegenius/codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.1.8/freegenius/commandprompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius/config.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.1.8/freegenius/eTextEdit.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.790296 freegenius-0.1.8/freegenius/files/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.1.8/freegenius/files/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.1.8/freegenius/geminipro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.1.8/freegenius/geminiprovision.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6492 2024-04-28 21:26:13.000000 freegenius-0.1.8/freegenius/groqchat.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.790296 freegenius-0.1.8/freegenius/gui/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.1.8/freegenius/gui/chatgui.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.1.8/freegenius/gui/worker.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.790296 freegenius-0.1.8/freegenius/history/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.1.8/freegenius/history/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.802296 freegenius-0.1.8/freegenius/icons/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.1.8/freegenius/icons/FreeGenius.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.1.8/freegenius/icons/FreeGenius.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.1.8/freegenius/icons/FreeGenius_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.1.8/freegenius/icons/ai.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.1.8/freegenius/icons/ai_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.1.8/freegenius/llamacpp.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.1.8/freegenius/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.1.8/freegenius/ollamachat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius/package_name.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.1.8/freegenius/palm2.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.814296 freegenius-0.1.8/freegenius/plugins/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.1.8/freegenius/plugins/000_check_ffmpeg.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.1.8/freegenius/plugins/000_check_pyaudio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.1.8/freegenius/plugins/000_check_vlc.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.1.8/freegenius/plugins/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.1.8/freegenius/plugins/add calendar event.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/aliases.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.1.8/freegenius/plugins/analyze audio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.1.8/freegenius/plugins/analyze files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.1.8/freegenius/plugins/analyze images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.1.8/freegenius/plugins/analyze web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.1.8/freegenius/plugins/auto correct python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/awesome prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/character analysis.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.1.8/freegenius/plugins/chat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.1.8/freegenius/plugins/contexts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/counselling.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.1.8/freegenius/plugins/create ai assistants.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.1.8/freegenius/plugins/create images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.1.8/freegenius/plugins/create maps.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.1.8/freegenius/plugins/create qrcode.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.1.8/freegenius/plugins/create statistical graphics.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.1.8/freegenius/plugins/dates and times.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.1.8/freegenius/plugins/download youtube or web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.1.8/freegenius/plugins/edit text.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.1.8/freegenius/plugins/execute computing tasks.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.1.8/freegenius/plugins/execute termux command.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/global finance.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/improve British English.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.1.8/freegenius/plugins/input suggestions.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.1.8/freegenius/plugins/install python package.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.1.8/freegenius/plugins/integrate google searches.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.1.8/freegenius/plugins/memory.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.1.8/freegenius/plugins/modify images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.1.8/freegenius/plugins/open web browser.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.1.8/freegenius/plugins/pronounce words.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.1.8/freegenius/plugins/remove image background.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.1.8/freegenius/plugins/search chat records.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.1.8/freegenius/plugins/search financial data.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.1.8/freegenius/plugins/search latest news.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.1.8/freegenius/plugins/search sqlite.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.1.8/freegenius/plugins/search weather info.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.1.8/freegenius/plugins/send email.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.1.8/freegenius/plugins/send tweet.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.1.8/freegenius/plugins/send whatsapp messages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.1.8/freegenius/qt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.1.8/freegenius/rag.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-04-26 22:24:44.000000 freegenius-0.1.8/freegenius/requirements.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.1.8/freegenius/servers.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.1.8/freegenius/systemtray.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.814296 freegenius-0.1.8/freegenius/temp/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.1.8/freegenius/temp/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.818296 freegenius-0.1.8/freegenius/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   112155 2024-04-27 15:16:32.000000 freegenius-0.1.8/freegenius/utils/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29734 2024-04-26 22:27:56.000000 freegenius-0.1.8/freegenius/utils/call_chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17269 2024-04-25 20:53:07.000000 freegenius-0.1.8/freegenius/utils/call_gemini.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17228 2024-04-28 21:27:08.000000 freegenius-0.1.8/freegenius/utils/call_groq.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    24612 2024-04-25 20:52:45.000000 freegenius-0.1.8/freegenius/utils/call_llamacpp.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.1.8/freegenius/utils/call_llm.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18713 2024-04-25 20:53:07.000000 freegenius-0.1.8/freegenius/utils/call_ollama.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18372 2024-04-28 21:23:25.000000 freegenius-0.1.8/freegenius/utils/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.1.8/freegenius/utils/config_tools.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.1.8/freegenius/utils/download.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.1.8/freegenius/utils/get_path_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.1.8/freegenius/utils/ollama_models.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.1.8/freegenius/utils/promptValidator.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.1.8/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.1.8/freegenius/utils/prompt_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.1.8/freegenius/utils/prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.1.8/freegenius/utils/python_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    50846 2024-04-28 21:25:47.000000 freegenius-0.1.8/freegenius/utils/shared_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.1.8/freegenius/utils/shortcuts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.1.8/freegenius/utils/single_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.1.8/freegenius/utils/streaming_word_wrapper.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.1.8/freegenius/utils/sttLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.1.8/freegenius/utils/terminal_mode_dialogs.py
--rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.1.8/freegenius/utils/terminal_system_command_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.1.8/freegenius/utils/text_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.1.8/freegenius/utils/tool_plugins.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.1.8/freegenius/utils/ttsLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.1.8/freegenius/utils/tts_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.1.8/freegenius/utils/vlc_utils.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.818296 freegenius-0.1.8/freegenius.egg-info/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-28 21:39:08.818296 freegenius-0.1.8/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10449 2024-04-28 21:39:01.000000 freegenius-0.1.8/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.494638 freegenius-0.1.9/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-05-02 18:52:19.494638 freegenius-0.1.9/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.462638 freegenius-0.1.9/freegenius/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11766 2024-05-02 18:52:18.000000 freegenius-0.1.9/freegenius/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.1.9/freegenius/__init__.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.462638 freegenius-0.1.9/freegenius/audio/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.1.9/freegenius/audio/notification1.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.1.9/freegenius/audio/notification1_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.1.9/freegenius/audio/notification2.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.1.9/freegenius/audio/notification2_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7006 2024-04-28 21:17:47.000000 freegenius-0.1.9/freegenius/autoassist.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.1.9/freegenius/autobuilder.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11081 2024-04-28 21:19:22.000000 freegenius-0.1.9/freegenius/autoretriever.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.1.9/freegenius/chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.1.9/freegenius/codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.1.9/freegenius/commandprompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:18.000000 freegenius-0.1.9/freegenius/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.1.9/freegenius/eTextEdit.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.462638 freegenius-0.1.9/freegenius/files/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.1.9/freegenius/files/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.1.9/freegenius/geminipro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.1.9/freegenius/geminiprovision.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6470 2024-05-02 18:09:51.000000 freegenius-0.1.9/freegenius/groqchat.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.462638 freegenius-0.1.9/freegenius/gui/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.1.9/freegenius/gui/chatgui.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.1.9/freegenius/gui/worker.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.462638 freegenius-0.1.9/freegenius/history/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.1.9/freegenius/history/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.478638 freegenius-0.1.9/freegenius/icons/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.1.9/freegenius/icons/FreeGenius.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.1.9/freegenius/icons/FreeGenius.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.1.9/freegenius/icons/FreeGenius_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.1.9/freegenius/icons/ai.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.1.9/freegenius/icons/ai_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.1.9/freegenius/llamacpp.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.458638 freegenius-0.1.9/freegenius/macOS_service/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.454638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.478638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.454638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.454638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.458638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.458638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.458638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.458638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.458638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.482638 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.1.9/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.1.9/freegenius/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.1.9/freegenius/ollamachat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-05-02 18:52:18.000000 freegenius-0.1.9/freegenius/package_name.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.1.9/freegenius/palm2.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.486637 freegenius-0.1.9/freegenius/plugins/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.1.9/freegenius/plugins/000_check_ffmpeg.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.1.9/freegenius/plugins/000_check_pyaudio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.1.9/freegenius/plugins/000_check_vlc.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.1.9/freegenius/plugins/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.1.9/freegenius/plugins/add calendar event.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.1.9/freegenius/plugins/aliases.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.1.9/freegenius/plugins/analyze audio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.1.9/freegenius/plugins/analyze files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.1.9/freegenius/plugins/analyze images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.1.9/freegenius/plugins/analyze web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.1.9/freegenius/plugins/auto correct python code.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.1.9/freegenius/plugins/awesome prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.1.9/freegenius/plugins/character analysis.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.1.9/freegenius/plugins/chat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.1.9/freegenius/plugins/contexts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.1.9/freegenius/plugins/counselling.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.1.9/freegenius/plugins/create ai assistants.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.1.9/freegenius/plugins/create images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.1.9/freegenius/plugins/create maps.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.1.9/freegenius/plugins/create qrcode.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.1.9/freegenius/plugins/create statistical graphics.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.1.9/freegenius/plugins/dates and times.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.1.9/freegenius/plugins/download youtube or web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.1.9/freegenius/plugins/edit text.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.1.9/freegenius/plugins/execute computing tasks.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.1.9/freegenius/plugins/execute termux command.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.1.9/freegenius/plugins/global finance.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.1.9/freegenius/plugins/improve British English.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.1.9/freegenius/plugins/input suggestions.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.1.9/freegenius/plugins/install python package.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.1.9/freegenius/plugins/integrate google searches.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.1.9/freegenius/plugins/memory.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.1.9/freegenius/plugins/modify images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.1.9/freegenius/plugins/open web browser.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.1.9/freegenius/plugins/pronounce words.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.1.9/freegenius/plugins/remove image background.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.1.9/freegenius/plugins/search chat records.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.1.9/freegenius/plugins/search financial data.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.1.9/freegenius/plugins/search latest news.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.1.9/freegenius/plugins/search sqlite.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.1.9/freegenius/plugins/search weather info.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.1.9/freegenius/plugins/send email.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.1.9/freegenius/plugins/send tweet.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.1.9/freegenius/plugins/send whatsapp messages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.1.9/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.1.9/freegenius/qt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.1.9/freegenius/rag.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-04-26 22:24:44.000000 freegenius-0.1.9/freegenius/requirements.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.1.9/freegenius/servers.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.1.9/freegenius/systemtray.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.486637 freegenius-0.1.9/freegenius/temp/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.1.9/freegenius/temp/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.490638 freegenius-0.1.9/freegenius/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   112149 2024-05-02 18:49:22.000000 freegenius-0.1.9/freegenius/utils/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29750 2024-05-02 18:43:53.000000 freegenius-0.1.9/freegenius/utils/call_chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17281 2024-05-02 18:43:53.000000 freegenius-0.1.9/freegenius/utils/call_gemini.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19915 2024-05-02 18:43:53.000000 freegenius-0.1.9/freegenius/utils/call_groq.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    24628 2024-05-02 18:43:56.000000 freegenius-0.1.9/freegenius/utils/call_llamacpp.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.1.9/freegenius/utils/call_llm.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18685 2024-05-02 18:43:53.000000 freegenius-0.1.9/freegenius/utils/call_ollama.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18484 2024-05-02 18:14:18.000000 freegenius-0.1.9/freegenius/utils/config_essential.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.1.9/freegenius/utils/config_tools.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.1.9/freegenius/utils/download.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.1.9/freegenius/utils/get_path_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.1.9/freegenius/utils/ollama_models.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.1.9/freegenius/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.1.9/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.1.9/freegenius/utils/prompt_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.1.9/freegenius/utils/prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.1.9/freegenius/utils/python_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    50846 2024-04-28 21:25:47.000000 freegenius-0.1.9/freegenius/utils/shared_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.1.9/freegenius/utils/shortcuts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.1.9/freegenius/utils/single_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.1.9/freegenius/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.1.9/freegenius/utils/sttLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.1.9/freegenius/utils/terminal_mode_dialogs.py
+-rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.1.9/freegenius/utils/terminal_system_command_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.1.9/freegenius/utils/text_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4353 2024-05-02 17:22:30.000000 freegenius-0.1.9/freegenius/utils/tool_plugins.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.1.9/freegenius/utils/ttsLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.1.9/freegenius/utils/tts_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.1.9/freegenius/utils/vlc_utils.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-02 18:52:19.490638 freegenius-0.1.9/freegenius.egg-info/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-05-02 18:52:19.000000 freegenius-0.1.9/freegenius.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-05-02 18:52:19.000000 freegenius-0.1.9/freegenius.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-05-02 18:52:19.000000 freegenius-0.1.9/freegenius.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-05-02 18:52:19.000000 freegenius-0.1.9/freegenius.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-05-02 18:52:19.000000 freegenius-0.1.9/freegenius.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-05-02 18:52:19.000000 freegenius-0.1.9/freegenius.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-05-02 18:52:19.494638 freegenius-0.1.9/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10449 2024-05-02 18:46:33.000000 freegenius-0.1.9/setup.py
```

### Comparing `freegenius-0.1.8/PKG-INFO` & `freegenius-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.1.8
+Version: 0.1.9
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.1.8/freegenius/README.md` & `freegenius-0.1.9/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/__init__.py` & `freegenius-0.1.9/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/audio/notification1.mp3` & `freegenius-0.1.9/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/audio/notification1_mild.mp3` & `freegenius-0.1.9/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/audio/notification2.mp3` & `freegenius-0.1.9/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/audio/notification2_mild.mp3` & `freegenius-0.1.9/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/autoassist.py` & `freegenius-0.1.9/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/autobuilder.py` & `freegenius-0.1.9/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/autoretriever.py` & `freegenius-0.1.9/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/chatgpt.py` & `freegenius-0.1.9/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/codey.py` & `freegenius-0.1.9/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/commandprompt.py` & `freegenius-0.1.9/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/eTextEdit.py` & `freegenius-0.1.9/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/geminipro.py` & `freegenius-0.1.9/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/geminiprovision.py` & `freegenius-0.1.9/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/groqchat.py` & `freegenius-0.1.9/freegenius/groqchat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from freegenius import config
 from freegenius import print2, getGroqClient
 from freegenius.utils.streaming_word_wrapper import StreamingWordWrapper
 from freegenius.utils.single_prompt import SinglePrompt
 
-from groq import Groq
 from prompt_toolkit.styles import Style
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.shortcuts import clear
 from pathlib import Path
 import threading, argparse, os, traceback
```

### Comparing `freegenius-0.1.8/freegenius/gui/chatgui.py` & `freegenius-0.1.9/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/gui/worker.py` & `freegenius-0.1.9/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/icons/FreeGenius.ico` & `freegenius-0.1.9/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/icons/FreeGenius.png` & `freegenius-0.1.9/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/icons/FreeGenius_original.png` & `freegenius-0.1.9/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/icons/ai.png` & `freegenius-0.1.9/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/icons/ai_original.png` & `freegenius-0.1.9/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/llamacpp.py` & `freegenius-0.1.9/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.1.9/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/main.py` & `freegenius-0.1.9/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/ollamachat.py` & `freegenius-0.1.9/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/palm2.py` & `freegenius-0.1.9/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.1.9/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.1.9/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/000_check_vlc.py` & `freegenius-0.1.9/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/add calendar event.py` & `freegenius-0.1.9/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/aliases.py` & `freegenius-0.1.9/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/analyze audio.py` & `freegenius-0.1.9/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/analyze files.py` & `freegenius-0.1.9/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/analyze images.py` & `freegenius-0.1.9/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/analyze web content.py` & `freegenius-0.1.9/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/auto correct python code.py` & `freegenius-0.1.9/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/awesome prompts.py` & `freegenius-0.1.9/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/character analysis.py` & `freegenius-0.1.9/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/chat.py` & `freegenius-0.1.9/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/contexts.py` & `freegenius-0.1.9/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/counselling.py` & `freegenius-0.1.9/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/create ai assistants.py` & `freegenius-0.1.9/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/create images.py` & `freegenius-0.1.9/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/create maps.py` & `freegenius-0.1.9/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/create qrcode.py` & `freegenius-0.1.9/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/create statistical graphics.py` & `freegenius-0.1.9/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/dates and times.py` & `freegenius-0.1.9/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/download youtube or web content.py` & `freegenius-0.1.9/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/edit text.py` & `freegenius-0.1.9/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/execute computing tasks.py` & `freegenius-0.1.9/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/execute termux command.py` & `freegenius-0.1.9/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/global finance.py` & `freegenius-0.1.9/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/improve British English.py` & `freegenius-0.1.9/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/input suggestions.py` & `freegenius-0.1.9/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/install python package.py` & `freegenius-0.1.9/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/integrate google searches.py` & `freegenius-0.1.9/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/memory.py` & `freegenius-0.1.9/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/modify images.py` & `freegenius-0.1.9/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/open web browser.py` & `freegenius-0.1.9/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/pronounce words.py` & `freegenius-0.1.9/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/remove image background.py` & `freegenius-0.1.9/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/search chat records.py` & `freegenius-0.1.9/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/search financial data.py` & `freegenius-0.1.9/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/search latest news.py` & `freegenius-0.1.9/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/search sqlite.py` & `freegenius-0.1.9/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/search weather info.py` & `freegenius-0.1.9/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/send email.py` & `freegenius-0.1.9/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/send tweet.py` & `freegenius-0.1.9/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.1.9/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.1.9/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/rag.py` & `freegenius-0.1.9/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/requirements.txt` & `freegenius-0.1.9/freegenius/requirements.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/servers.py` & `freegenius-0.1.9/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/systemtray.py` & `freegenius-0.1.9/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/assistant.py` & `freegenius-0.1.9/freegenius/utils/assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -3814,3197 +3814,3197 @@
 0000ee50: 332d 3862 2d38 3139 3222 2c0a 2020 2020  3-8b-8192",.    
 0000ee60: 2020 2020 2020 2020 2020 2020 226c 6c61              "lla
 0000ee70: 6d61 332d 3730 622d 3831 3932 222c 0a20  ma3-70b-8192",. 
 0000ee80: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
 0000ee90: 2020 2020 2020 2020 2020 7469 746c 653d            title=
 0000eea0: 2247 726f 7120 4d6f 6465 6c22 2c0a 2020  "Groq Model",.  
 0000eeb0: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
-0000eec0: 743d 636f 6e66 6967 2e63 6861 7447 5054  t=config.chatGPT
-0000eed0: 4170 694d 6f64 656c 2069 6620 636f 6e66  ApiModel if conf
-0000eee0: 6967 2e63 6861 7447 5054 4170 694d 6f64  ig.chatGPTApiMod
-0000eef0: 656c 2069 6e20 7365 6c66 2e6d 6f64 656c  el in self.model
-0000ef00: 7320 656c 7365 2073 656c 662e 6d6f 6465  s else self.mode
-0000ef10: 6c73 5b30 5d2c 0a20 2020 2020 2020 2020  ls[0],.         
-0000ef20: 2020 2074 6578 743d 2253 656c 6563 7420     text="Select 
-0000ef30: 6120 6675 6e63 7469 6f6e 2063 616c 6c20  a function call 
-0000ef40: 6d6f 6465 6c3a 5c6e 2866 6f72 2062 6f74  model:\n(for bot
-0000ef50: 6820 6368 6174 2061 6e64 2074 6173 6b20  h chat and task 
-0000ef60: 6578 6563 7574 696f 6e29 222c 0a20 2020  execution)",.   
-0000ef70: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-0000ef80: 6620 6d6f 6465 6c3a 0a20 2020 2020 2020  f model:.       
-0000ef90: 2020 2020 2069 6620 6665 6174 7572 6520       if feature 
-0000efa0: 3d3d 2022 6465 6661 756c 7422 3a0a 2020  == "default":.  
-0000efb0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000efc0: 6e66 6967 2e67 726f 7141 7069 5f6d 6169  nfig.groqApi_mai
-0000efd0: 6e5f 6d6f 6465 6c20 3d20 6d6f 6465 6c0a  n_model = model.
-0000efe0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000eff0: 2066 6561 7475 7265 203d 3d20 2263 6861   feature == "cha
-0000f000: 7422 3a0a 2020 2020 2020 2020 2020 2020  t":.            
-0000f010: 2020 2020 636f 6e66 6967 2e67 726f 7141      config.groqA
-0000f020: 7069 5f63 6861 745f 6d6f 6465 6c20 3d20  pi_chat_model = 
-0000f030: 6d6f 6465 6c0a 2020 2020 2020 2020 2020  model.          
-0000f040: 2020 7072 696e 7433 2866 2247 726f 7120    print3(f"Groq 
-0000f050: 6d6f 6465 6c3a 207b 6d6f 6465 6c7d 2229  model: {model}")
-0000f060: 0a0a 2020 2020 6465 6620 7365 744c 6c6d  ..    def setLlm
-0000f070: 4d6f 6465 6c5f 6368 6174 6770 7428 7365  Model_chatgpt(se
-0000f080: 6c66 293a 0a20 2020 2020 2020 206d 6f64  lf):.        mod
-0000f090: 656c 203d 2073 656c 662e 6469 616c 6f67  el = self.dialog
-0000f0a0: 732e 6765 7456 616c 6964 4f70 7469 6f6e  s.getValidOption
-0000f0b0: 7328 0a20 2020 2020 2020 2020 2020 206f  s(.            o
-0000f0c0: 7074 696f 6e73 3d73 656c 662e 6d6f 6465  ptions=self.mode
-0000f0d0: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
-0000f0e0: 7469 746c 653d 2243 6861 7447 5054 204d  title="ChatGPT M
-0000f0f0: 6f64 656c 222c 0a20 2020 2020 2020 2020  odel",.         
-0000f100: 2020 2064 6566 6175 6c74 3d63 6f6e 6669     default=confi
-0000f110: 672e 6368 6174 4750 5441 7069 4d6f 6465  g.chatGPTApiMode
-0000f120: 6c20 6966 2063 6f6e 6669 672e 6368 6174  l if config.chat
-0000f130: 4750 5441 7069 4d6f 6465 6c20 696e 2073  GPTApiModel in s
-0000f140: 656c 662e 6d6f 6465 6c73 2065 6c73 6520  elf.models else 
-0000f150: 7365 6c66 2e6d 6f64 656c 735b 305d 2c0a  self.models[0],.
-0000f160: 2020 2020 2020 2020 2020 2020 7465 7874              text
-0000f170: 3d22 5365 6c65 6374 2061 2066 756e 6374  ="Select a funct
-0000f180: 696f 6e20 6361 6c6c 206d 6f64 656c 3a5c  ion call model:\
-0000f190: 6e28 666f 7220 626f 7468 2063 6861 7420  n(for both chat 
-0000f1a0: 616e 6420 7461 736b 2065 7865 6375 7469  and task executi
-0000f1b0: 6f6e 2922 2c0a 2020 2020 2020 2020 290a  on)",.        ).
-0000f1c0: 2020 2020 2020 2020 6966 206d 6f64 656c          if model
-0000f1d0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-0000f1e0: 6e66 6967 2e63 6861 7447 5054 4170 694d  nfig.chatGPTApiM
-0000f1f0: 6f64 656c 203d 206d 6f64 656c 0a20 2020  odel = model.   
-0000f200: 2020 2020 2020 2020 2070 7269 6e74 3328           print3(
-0000f210: 6622 4368 6174 4750 5420 6d6f 6465 6c3a  f"ChatGPT model:
-0000f220: 207b 6d6f 6465 6c7d 2229 0a20 2020 2020   {model}").     
-0000f230: 2020 2020 2020 2023 2073 6574 206d 6178         # set max
-0000f240: 2074 6f6b 656e 730a 2020 2020 2020 2020   tokens.        
-0000f250: 2020 2020 636f 6e66 6967 2e63 6861 7447      config.chatG
-0000f260: 5054 4170 694d 6178 546f 6b65 6e73 203d  PTApiMaxTokens =
-0000f270: 2073 656c 662e 6765 744d 6178 546f 6b65   self.getMaxToke
-0000f280: 6e73 2829 5b2d 315d 0a20 2020 2020 2020  ns()[-1].       
-0000f290: 2020 2020 2070 7269 6e74 3328 6622 4d61       print3(f"Ma
-0000f2a0: 7869 6d75 6d20 6f75 7470 7574 2074 6f6b  ximum output tok
-0000f2b0: 656e 733a 207b 636f 6e66 6967 2e63 6861  ens: {config.cha
-0000f2c0: 7447 5054 4170 694d 6178 546f 6b65 6e73  tGPTApiMaxTokens
-0000f2d0: 7d22 290a 0a20 2020 2064 6566 2073 6574  }")..    def set
-0000f2e0: 4368 6174 626f 7428 7365 6c66 293a 0a20  Chatbot(self):. 
-0000f2f0: 2020 2020 2020 206d 6f64 656c 203d 2073         model = s
-0000f300: 656c 662e 6469 616c 6f67 732e 6765 7456  elf.dialogs.getV
-0000f310: 616c 6964 4f70 7469 6f6e 7328 0a20 2020  alidOptions(.   
-0000f320: 2020 2020 2020 2020 206f 7074 696f 6e73           options
-0000f330: 3d28 2263 6861 7467 7074 222c 2022 6765  =("chatgpt", "ge
-0000f340: 6d69 6e69 7072 6f22 2c20 2270 616c 6d32  minipro", "palm2
-0000f350: 222c 2022 636f 6465 7922 292c 0a20 2020  ", "codey"),.   
-0000f360: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
-0000f370: 4368 6174 2d6f 6e6c 7920 6d6f 6465 6c22  Chat-only model"
-0000f380: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
-0000f390: 6661 756c 743d 636f 6e66 6967 2e63 6861  fault=config.cha
-0000f3a0: 7462 6f74 2c0a 2020 2020 2020 2020 2020  tbot,.          
-0000f3b0: 2020 7465 7874 3d22 5365 6c65 6374 2064    text="Select d
-0000f3c0: 6566 6175 6c74 2063 6861 742d 6f6e 6c79  efault chat-only
-0000f3d0: 206d 6f64 656c 3a5c 6e28 4465 6661 756c   model:\n(Defaul
-0000f3e0: 7420 6d6f 6465 6c20 6973 206c 6f61 6465  t model is loade
-0000f3f0: 6420 7768 656e 2079 6f75 2069 6e63 6c75  d when you inclu
-0000f400: 6465 2027 5b43 4841 545d 2720 696e 2079  de '[CHAT]' in y
-0000f410: 6f75 7220 696e 7075 7429 222c 0a20 2020  our input)",.   
-0000f420: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-0000f430: 6620 6d6f 6465 6c3a 0a20 2020 2020 2020  f model:.       
-0000f440: 2020 2020 2063 6f6e 6669 672e 6368 6174       config.chat
-0000f450: 626f 7420 3d20 6d6f 6465 6c0a 2020 2020  bot = model.    
-0000f460: 2020 2020 2020 2020 7072 696e 7433 2866          print3(f
-0000f470: 2243 6861 742d 6f6e 6c79 206d 6f64 656c  "Chat-only model
-0000f480: 3a20 7b6d 6f64 656c 7d22 290a 0a20 2020  : {model}")..   
-0000f490: 2064 6566 2073 6574 456d 6265 6464 696e   def setEmbeddin
-0000f4a0: 674d 6f64 656c 2873 656c 6629 3a0a 2020  gModel(self):.  
-0000f4b0: 2020 2020 2020 6f6c 6445 6d62 6564 6469        oldEmbeddi
-0000f4c0: 6e67 4d6f 6465 6c20 3d20 636f 6e66 6967  ngModel = config
-0000f4d0: 2e65 6d62 6564 6469 6e67 4d6f 6465 6c0a  .embeddingModel.
-0000f4e0: 2020 2020 2020 2020 6d6f 6465 6c20 3d20          model = 
-0000f4f0: 7365 6c66 2e64 6961 6c6f 6773 2e67 6574  self.dialogs.get
-0000f500: 5661 6c69 644f 7074 696f 6e73 280a 2020  ValidOptions(.  
-0000f510: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-0000f520: 733d 2822 7465 7874 2d65 6d62 6564 6469  s=("text-embeddi
-0000f530: 6e67 2d33 2d6c 6172 6765 222c 2022 7465  ng-3-large", "te
-0000f540: 7874 2d65 6d62 6564 6469 6e67 2d33 2d73  xt-embedding-3-s
-0000f550: 6d61 6c6c 222c 2022 7465 7874 2d65 6d62  mall", "text-emb
-0000f560: 6564 6469 6e67 2d61 6461 2d30 3032 222c  edding-ada-002",
-0000f570: 2022 7061 7261 7068 7261 7365 2d6d 756c   "paraphrase-mul
-0000f580: 7469 6c69 6e67 7561 6c2d 6d70 6e65 742d  tilingual-mpnet-
-0000f590: 6261 7365 2d76 3222 2c20 2261 6c6c 2d6d  base-v2", "all-m
-0000f5a0: 706e 6574 2d62 6173 652d 7632 222c 2022  pnet-base-v2", "
-0000f5b0: 616c 6c2d 4d69 6e69 4c4d 2d4c 362d 7632  all-MiniLM-L6-v2
-0000f5c0: 222c 2022 6375 7374 6f6d 2229 2c0a 2020  ", "custom"),.  
-0000f5d0: 2020 2020 2020 2020 2020 7469 746c 653d            title=
-0000f5e0: 2245 6d62 6564 6469 6e67 206d 6f64 656c  "Embedding model
-0000f5f0: 222c 0a20 2020 2020 2020 2020 2020 2064  ",.            d
-0000f600: 6566 6175 6c74 3d63 6f6e 6669 672e 656d  efault=config.em
-0000f610: 6265 6464 696e 674d 6f64 656c 2c0a 2020  beddingModel,.  
-0000f620: 2020 2020 2020 2020 2020 7465 7874 3d22            text="
-0000f630: 5365 6c65 6374 2061 6e20 656d 6265 6464  Select an embedd
-0000f640: 696e 6720 6d6f 6465 6c3a 222c 0a20 2020  ing model:",.   
-0000f650: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-0000f660: 6620 6d6f 6465 6c3a 0a20 2020 2020 2020  f model:.       
-0000f670: 2020 2020 2069 6620 6d6f 6465 6c20 3d3d       if model ==
-0000f680: 2022 6375 7374 6f6d 223a 0a20 2020 2020   "custom":.     
-0000f690: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000f6a0: 3128 2245 6e74 6572 204f 7065 6e41 4920  1("Enter OpenAI 
-0000f6b0: 6f72 2053 656e 7465 6e63 6520 5472 616e  or Sentence Tran
-0000f6c0: 7366 6f72 6d65 7220 456d 6265 6464 696e  sformer Embeddin
-0000f6d0: 6720 6d6f 6465 6c3a 2229 0a20 2020 2020  g model:").     
-0000f6e0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000f6f0: 3128 2252 6561 6420 6d6f 7265 2061 743a  1("Read more at:
-0000f700: 2068 7474 7073 3a2f 2f77 7777 2e73 6265   https://www.sbe
-0000f710: 7274 2e6e 6574 2f64 6f63 732f 7072 6574  rt.net/docs/pret
-0000f720: 7261 696e 6564 5f6d 6f64 656c 732e 6874  rained_models.ht
-0000f730: 6d6c 2229 0a20 2020 2020 2020 2020 2020  ml").           
-0000f740: 2020 2020 2063 7573 746f 6d4d 6f64 656c       customModel
-0000f750: 203d 2073 656c 662e 7072 6f6d 7074 732e   = self.prompts.
-0000f760: 7369 6d70 6c65 5072 6f6d 7074 2873 7479  simplePrompt(sty
-0000f770: 6c65 3d73 656c 662e 7072 6f6d 7074 732e  le=self.prompts.
-0000f780: 7072 6f6d 7074 5374 796c 6532 2c20 6465  promptStyle2, de
-0000f790: 6661 756c 743d 636f 6e66 6967 2e65 6d62  fault=config.emb
-0000f7a0: 6564 6469 6e67 4d6f 6465 6c29 0a20 2020  eddingModel).   
-0000f7b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000f7c0: 6375 7374 6f6d 4d6f 6465 6c20 616e 6420  customModel and 
-0000f7d0: 6e6f 7420 6375 7374 6f6d 4d6f 6465 6c2e  not customModel.
-0000f7e0: 7374 7269 7028 292e 6c6f 7765 7228 2920  strip().lower() 
-0000f7f0: 3d3d 2063 6f6e 6669 672e 6578 6974 5f65  == config.exit_e
-0000f800: 6e74 7279 3a0a 2020 2020 2020 2020 2020  ntry:.          
-0000f810: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-0000f820: 2e65 6d62 6564 6469 6e67 4d6f 6465 6c20  .embeddingModel 
-0000f830: 3d20 6375 7374 6f6d 4d6f 6465 6c20 0a20  = customModel . 
-0000f840: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000f850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f860: 2063 6f6e 6669 672e 656d 6265 6464 696e   config.embeddin
-0000f870: 674d 6f64 656c 203d 206d 6f64 656c 0a20  gModel = model. 
-0000f880: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000f890: 3328 6622 456d 6265 6464 696e 6720 6d6f  3(f"Embedding mo
-0000f8a0: 6465 6c3a 207b 6d6f 6465 6c7d 2229 0a20  del: {model}"). 
-0000f8b0: 2020 2020 2020 2069 6620 6e6f 7420 6f6c         if not ol
-0000f8c0: 6445 6d62 6564 6469 6e67 4d6f 6465 6c20  dEmbeddingModel 
-0000f8d0: 3d3d 2063 6f6e 6669 672e 656d 6265 6464  == config.embedd
-0000f8e0: 696e 674d 6f64 656c 3a0a 2020 2020 2020  ingModel:.      
-0000f8f0: 2020 2020 2020 7072 696e 7431 2866 2259        print1(f"Y
-0000f900: 6f75 2776 6520 6368 616e 6765 2074 6865  ou've change the
-0000f910: 2065 6d62 6564 6469 6e67 206d 6f64 656c   embedding model
-0000f920: 2066 726f 6d20 277b 6f6c 6445 6d62 6564   from '{oldEmbed
-0000f930: 6469 6e67 4d6f 6465 6c7d 2720 746f 2027  dingModel}' to '
-0000f940: 7b63 6f6e 6669 672e 656d 6265 6464 696e  {config.embeddin
-0000f950: 674d 6f64 656c 7d27 2e22 290a 2020 2020  gModel}'.").    
-0000f960: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
-0000f970: 546f 2077 6f72 6b20 7769 7468 2074 6865  To work with the
-0000f980: 206e 6577 6c79 2073 656c 6563 7465 6420   newly selected 
-0000f990: 6d6f 6465 6c2c 2070 7265 7669 6f75 7320  model, previous 
-0000f9a0: 6d65 6d6f 7279 2073 746f 7265 2061 6e64  memory store and
-0000f9b0: 2072 6574 7269 6576 6564 2063 6f6c 6c65   retrieved colle
-0000f9c0: 6374 696f 6e73 206e 6565 6420 746f 2062  ctions need to b
-0000f9d0: 6520 6465 6c65 7465 642e 2229 0a20 2020  e deleted.").   
-0000f9e0: 2020 2020 2020 2020 2070 7269 6e74 3128           print1(
-0000f9f0: 2244 6f20 796f 7520 7761 6e74 2074 6f20  "Do you want to 
-0000fa00: 6465 6c65 7465 2074 6865 6d20 6e6f 773f  delete them now?
-0000fa10: 205b 795d 6573 202f 205b 4e5d 6f22 290a   [y]es / [N]o").
-0000fa20: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-0000fa30: 6972 6d61 7469 6f6e 203d 2073 656c 662e  irmation = self.
-0000fa40: 7072 6f6d 7074 732e 7369 6d70 6c65 5072  prompts.simplePr
-0000fa50: 6f6d 7074 2873 7479 6c65 3d73 656c 662e  ompt(style=self.
-0000fa60: 7072 6f6d 7074 732e 7072 6f6d 7074 5374  prompts.promptSt
-0000fa70: 796c 6532 2c20 6465 6661 756c 743d 2279  yle2, default="y
-0000fa80: 6573 2229 0a20 2020 2020 2020 2020 2020  es").           
-0000fa90: 2069 6620 636f 6e66 6972 6d61 7469 6f6e   if confirmation
-0000faa0: 2e6c 6f77 6572 2829 2069 6e20 2822 7922  .lower() in ("y"
-0000fab0: 2c20 2279 6573 2229 3a0a 2020 2020 2020  , "yes"):.      
-0000fac0: 2020 2020 2020 2020 2020 6d65 6d6f 7279            memory
-0000fad0: 5f73 746f 7265 203d 206f 732e 7061 7468  _store = os.path
-0000fae0: 2e6a 6f69 6e28 636f 6e66 6967 2e6c 6f63  .join(config.loc
-0000faf0: 616c 5374 6f72 6167 652c 2022 6d65 6d6f  alStorage, "memo
-0000fb00: 7279 2229 0a20 2020 2020 2020 2020 2020  ry").           
-0000fb10: 2020 2020 2072 6574 7269 6576 6564 5f63       retrieved_c
-0000fb20: 6f6c 6c65 6374 696f 6e73 203d 206f 732e  ollections = os.
-0000fb30: 7061 7468 2e6a 6f69 6e28 636f 6e66 6967  path.join(config
-0000fb40: 2e6c 6f63 616c 5374 6f72 6167 652c 2022  .localStorage, "
-0000fb50: 6175 746f 6765 6e22 2c20 2272 6574 7269  autogen", "retri
-0000fb60: 6576 6572 2229 0a20 2020 2020 2020 2020  ever").         
-0000fb70: 2020 2020 2020 2066 6f72 2066 6f6c 6465         for folde
-0000fb80: 7220 696e 2028 6d65 6d6f 7279 5f73 746f  r in (memory_sto
-0000fb90: 7265 2c20 7265 7472 6965 7665 645f 636f  re, retrieved_co
-0000fba0: 6c6c 6563 7469 6f6e 7329 3a0a 2020 2020  llections):.    
-0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbc0: 7368 7574 696c 2e72 6d74 7265 6528 666f  shutil.rmtree(fo
-0000fbd0: 6c64 6572 2c20 6967 6e6f 7265 5f65 7272  lder, ignore_err
-0000fbe0: 6f72 733d 5472 7565 290a 2020 2020 2020  ors=True).      
-0000fbf0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000fc00: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000fc10: 7431 2866 2244 6f20 796f 7520 7761 6e74  t1(f"Do you want
-0000fc20: 2074 6f20 6368 616e 6765 2062 6163 6b20   to change back 
-0000fc30: 7468 6520 656d 6265 6464 696e 6720 6d6f  the embedding mo
-0000fc40: 6465 6c20 6672 6f6d 2027 7b63 6f6e 6669  del from '{confi
-0000fc50: 672e 656d 6265 6464 696e 674d 6f64 656c  g.embeddingModel
-0000fc60: 7d27 2074 6f20 277b 6f6c 6445 6d62 6564  }' to '{oldEmbed
-0000fc70: 6469 6e67 4d6f 6465 6c7d 273f 205b 795d  dingModel}'? [y]
-0000fc80: 6573 202f 205b 4e5d 6f22 290a 2020 2020  es / [N]o").    
-0000fc90: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-0000fca0: 6972 6d61 7469 6f6e 203d 2073 656c 662e  irmation = self.
-0000fcb0: 7072 6f6d 7074 732e 7369 6d70 6c65 5072  prompts.simplePr
-0000fcc0: 6f6d 7074 2873 7479 6c65 3d73 656c 662e  ompt(style=self.
-0000fcd0: 7072 6f6d 7074 732e 7072 6f6d 7074 5374  prompts.promptSt
-0000fce0: 796c 6532 2c20 6465 6661 756c 743d 2279  yle2, default="y
-0000fcf0: 6573 2229 0a20 2020 2020 2020 2020 2020  es").           
-0000fd00: 2020 2020 2069 6620 6e6f 7420 636f 6e66       if not conf
-0000fd10: 6972 6d61 7469 6f6e 2e6c 6f77 6572 2829  irmation.lower()
-0000fd20: 2069 6e20 2822 7922 2c20 2279 6573 2229   in ("y", "yes")
-0000fd30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fd40: 2020 2020 2020 636f 6e66 6967 2e65 6d62        config.emb
-0000fd50: 6564 6469 6e67 4d6f 6465 6c20 3d20 6f6c  eddingModel = ol
-0000fd60: 6445 6d62 6564 6469 6e67 4d6f 6465 6c0a  dEmbeddingModel.
-0000fd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd80: 2020 2020 7072 696e 7433 2866 2245 6d62      print3(f"Emb
-0000fd90: 6564 6469 6e67 206d 6f64 656c 3a20 7b6f  edding model: {o
-0000fda0: 6c64 456d 6265 6464 696e 674d 6f64 656c  ldEmbeddingModel
-0000fdb0: 7d22 290a 2020 2020 2020 2020 6966 206e  }").        if n
-0000fdc0: 6f74 206f 6c64 456d 6265 6464 696e 674d  ot oldEmbeddingM
-0000fdd0: 6f64 656c 203d 3d20 636f 6e66 6967 2e65  odel == config.e
-0000fde0: 6d62 6564 6469 6e67 4d6f 6465 6c3a 0a20  mbeddingModel:. 
-0000fdf0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-0000fe00: 672e 7361 7665 436f 6e66 6967 2829 0a0a  g.saveConfig()..
-0000fe10: 2020 2020 6465 6620 7365 7441 7574 6f47      def setAutoG
-0000fe20: 656e 4275 696c 6465 7243 6f6e 6669 6728  enBuilderConfig(
-0000fe30: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-0000fe40: 6620 6e6f 7420 636f 6e66 6967 2e69 7354  f not config.isT
-0000fe50: 6572 6d75 783a 0a20 2020 2020 2020 2020  ermux:.         
-0000fe60: 2020 2041 7574 6f47 656e 4275 696c 6465     AutoGenBuilde
-0000fe70: 7228 292e 7072 6f6d 7074 436f 6e66 6967  r().promptConfig
-0000fe80: 2829 0a0a 2020 2020 6465 6620 7365 7441  ()..    def setA
-0000fe90: 7373 6973 7461 6e74 4e61 6d65 2873 656c  ssistantName(sel
-0000fea0: 6629 3a0a 2020 2020 2020 2020 7072 696e  f):.        prin
-0000feb0: 7431 2822 596f 7520 6d61 7920 6d6f 6469  t1("You may modi
-0000fec0: 6679 206d 7920 6e61 6d65 2062 656c 6f77  fy my name below
-0000fed0: 3a22 290a 2020 2020 2020 2020 6672 6565  :").        free
-0000fee0: 4765 6e69 7573 4149 4e61 6d65 203d 2073  GeniusAIName = s
-0000fef0: 656c 662e 7072 6f6d 7074 732e 7369 6d70  elf.prompts.simp
-0000ff00: 6c65 5072 6f6d 7074 2873 7479 6c65 3d73  lePrompt(style=s
-0000ff10: 656c 662e 7072 6f6d 7074 732e 7072 6f6d  elf.prompts.prom
-0000ff20: 7074 5374 796c 6532 2c20 6465 6661 756c  ptStyle2, defaul
-0000ff30: 743d 636f 6e66 6967 2e66 7265 6547 656e  t=config.freeGen
-0000ff40: 6975 7341 494e 616d 6529 0a20 2020 2020  iusAIName).     
-0000ff50: 2020 2069 6620 6672 6565 4765 6e69 7573     if freeGenius
-0000ff60: 4149 4e61 6d65 2061 6e64 206e 6f74 2066  AIName and not f
-0000ff70: 7265 6547 656e 6975 7341 494e 616d 652e  reeGeniusAIName.
-0000ff80: 7374 7269 7028 292e 6c6f 7765 7228 2920  strip().lower() 
-0000ff90: 3d3d 2063 6f6e 6669 672e 6578 6974 5f65  == config.exit_e
-0000ffa0: 6e74 7279 3a0a 2020 2020 2020 2020 2020  ntry:.          
-0000ffb0: 2020 636f 6e66 6967 2e66 7265 6547 656e    config.freeGen
-0000ffc0: 6975 7341 494e 616d 6520 3d20 6672 6565  iusAIName = free
-0000ffd0: 4765 6e69 7573 4149 4e61 6d65 0a20 2020  GeniusAIName.   
-0000ffe0: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
-0000fff0: 6c6f 6361 6c53 746f 7261 6765 203d 2067  localStorage = g
-00010000: 6574 4c6f 6361 6c53 746f 7261 6765 2829  etLocalStorage()
-00010010: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00010020: 6669 672e 7361 7665 436f 6e66 6967 2829  fig.saveConfig()
-00010030: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00010040: 6e74 3328 6622 596f 7520 6861 7665 2063  nt3(f"You have c
-00010050: 6861 6e67 6564 206d 7920 6e61 6d65 2074  hanged my name t
-00010060: 6f3a 207b 636f 6e66 6967 2e66 7265 6547  o: {config.freeG
-00010070: 656e 6975 7341 494e 616d 657d 2229 0a0a  eniusAIName}")..
-00010080: 2020 2020 6465 6620 7365 7443 7573 746f      def setCusto
-00010090: 6d53 7973 7465 6d4d 6573 7361 6765 2873  mSystemMessage(s
-000100a0: 656c 6629 3a0a 2020 2020 2020 2020 7072  elf):.        pr
-000100b0: 696e 7431 2822 596f 7520 6361 6e20 6d6f  int1("You can mo
-000100c0: 6469 6679 2074 6865 2073 7973 7465 6d20  dify the system 
-000100d0: 6d65 7373 6167 6520 746f 2066 7572 6e69  message to furni
-000100e0: 7368 206d 6520 7769 7468 2064 6574 6169  sh me with detai
-000100f0: 6c73 2061 626f 7574 206d 7920 6361 7061  ls about my capa
-00010100: 6269 6c69 7469 6573 2c20 636f 6e73 7472  bilities, constr
-00010110: 6169 6e74 732c 206f 7220 616e 7920 7065  aints, or any pe
-00010120: 7274 696e 656e 7420 636f 6e74 6578 7420  rtinent context 
-00010130: 7468 6174 206d 6179 2069 6e66 6f72 6d20  that may inform 
-00010140: 6f75 7220 696e 7465 7261 6374 696f 6e73  our interactions
-00010150: 2e20 5468 6973 2077 696c 6c20 6775 6964  . This will guid
-00010160: 6520 6d65 2069 6e20 6d61 6e61 6769 6e67  e me in managing
-00010170: 2061 6e64 2072 6573 706f 6e64 696e 6720   and responding 
-00010180: 746f 2079 6f75 7220 7265 7175 6573 7473  to your requests
-00010190: 2061 7070 726f 7072 6961 7465 6c79 2e22   appropriately."
-000101a0: 290a 2020 2020 2020 2020 7072 696e 7431  ).        print1
-000101b0: 2822 506c 6561 7365 206e 6f74 6520 7468  ("Please note th
-000101c0: 6174 2061 6c74 6572 696e 6720 6d79 2073  at altering my s
-000101d0: 7973 7465 6d20 6d65 7373 6167 6520 6469  ystem message di
-000101e0: 7265 6374 6c79 2061 6666 6563 7473 206d  rectly affects m
-000101f0: 7920 6675 6e63 7469 6f6e 616c 6974 792e  y functionality.
-00010200: 2048 616e 646c 6520 7769 7468 2063 6172   Handle with car
-00010210: 652e 2229 0a20 2020 2020 2020 2070 7269  e.").        pri
-00010220: 6e74 3128 2245 6e74 6572 2063 7573 746f  nt1("Enter custo
-00010230: 6d20 7379 7374 656d 206d 6573 7361 6765  m system message
-00010240: 2062 656c 6f77 3a22 290a 2020 2020 2020   below:").      
-00010250: 2020 7072 696e 7431 2866 2228 4b65 6570    print1(f"(Keep
-00010260: 2069 7420 626c 616e 6b20 746f 2075 7365   it blank to use
-00010270: 207b 636f 6e66 6967 2e66 7265 6547 656e   {config.freeGen
-00010280: 6975 7341 494e 616d 657d 2064 6566 6175  iusAIName} defau
-00010290: 6c74 2073 7973 7465 6d20 6d65 7373 6167  lt system messag
-000102a0: 652e 2922 290a 2020 2020 2020 2020 6d65  e.)").        me
-000102b0: 7373 6167 6520 3d20 7365 6c66 2e70 726f  ssage = self.pro
-000102c0: 6d70 7473 2e73 696d 706c 6550 726f 6d70  mpts.simplePromp
-000102d0: 7428 7374 796c 653d 7365 6c66 2e70 726f  t(style=self.pro
-000102e0: 6d70 7473 2e70 726f 6d70 7453 7479 6c65  mpts.promptStyle
-000102f0: 322c 2064 6566 6175 6c74 3d63 6f6e 6669  2, default=confi
-00010300: 672e 7379 7374 656d 4d65 7373 6167 655f  g.systemMessage_
-00010310: 6c65 746d 6564 6f69 7429 0a20 2020 2020  letmedoit).     
-00010320: 2020 2069 6620 6d65 7373 6167 6520 616e     if message an
-00010330: 6420 6e6f 7420 6d65 7373 6167 652e 7374  d not message.st
-00010340: 7269 7028 292e 6c6f 7765 7228 2920 3d3d  rip().lower() ==
-00010350: 2063 6f6e 6669 672e 6578 6974 5f65 6e74   config.exit_ent
-00010360: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00010370: 636f 6e66 6967 2e73 7973 7465 6d4d 6573  config.systemMes
-00010380: 7361 6765 5f6c 6574 6d65 646f 6974 203d  sage_letmedoit =
-00010390: 206d 6573 7361 6765 0a20 2020 2020 2020   message.       
-000103a0: 2020 2020 2063 6f6e 6669 672e 7361 7665       config.save
-000103b0: 436f 6e66 6967 2829 0a20 2020 2020 2020  Config().       
-000103c0: 2020 2020 2070 7269 6e74 3328 6622 4375       print3(f"Cu
-000103d0: 7374 6f6d 2073 7973 7465 6d20 6d65 7373  stom system mess
-000103e0: 6167 653a 207b 636f 6e66 6967 2e66 7265  age: {config.fre
-000103f0: 6547 656e 6975 7341 494e 616d 657d 2229  eGeniusAIName}")
-00010400: 0a0a 2020 2020 6465 6620 7365 7443 7573  ..    def setCus
-00010410: 746f 6d54 6578 7445 6469 746f 7228 7365  tomTextEditor(se
-00010420: 6c66 293a 0a20 2020 2020 2020 2070 7269  lf):.        pri
-00010430: 6e74 3128 2250 6c65 6173 6520 7370 6563  nt1("Please spec
-00010440: 6966 7920 6375 7374 6f6d 2074 6578 7420  ify custom text 
-00010450: 6564 6974 6f72 2063 6f6d 6d61 6e64 2062  editor command b
-00010460: 656c 6f77 3a22 290a 2020 2020 2020 2020  elow:").        
-00010470: 7072 696e 7431 2822 652e 672e 2027 6d69  print1("e.g. 'mi
-00010480: 6372 6f20 2d73 6f66 7477 7261 7020 7472  cro -softwrap tr
-00010490: 7565 202d 776f 7264 7772 6170 2074 7275  ue -wordwrap tru
-000104a0: 6527 2229 0a20 2020 2020 2020 2070 7269  e'").        pri
-000104b0: 6e74 3128 224c 6561 7665 2069 7420 626c  nt1("Leave it bl
-000104c0: 616e 6b20 746f 2075 7365 206f 7572 2062  ank to use our b
-000104d0: 7569 6c74 2d69 6e20 7465 7874 2065 6469  uilt-in text edi
-000104e0: 746f 7220 2765 5465 7874 4564 6974 2720  tor 'eTextEdit' 
-000104f0: 6279 2064 6566 6175 6c74 2e22 290a 2020  by default.").  
-00010500: 2020 2020 2020 6375 7374 6f6d 5465 7874        customText
-00010510: 4564 6974 6f72 203d 2073 656c 662e 7072  Editor = self.pr
-00010520: 6f6d 7074 732e 7369 6d70 6c65 5072 6f6d  ompts.simpleProm
-00010530: 7074 2873 7479 6c65 3d73 656c 662e 7072  pt(style=self.pr
-00010540: 6f6d 7074 732e 7072 6f6d 7074 5374 796c  ompts.promptStyl
-00010550: 6532 2c20 6465 6661 756c 743d 636f 6e66  e2, default=conf
-00010560: 6967 2e63 7573 746f 6d54 6578 7445 6469  ig.customTextEdi
-00010570: 746f 7229 0a20 2020 2020 2020 2069 6620  tor).        if 
-00010580: 6375 7374 6f6d 5465 7874 4564 6974 6f72  customTextEditor
-00010590: 2061 6e64 206e 6f74 2063 7573 746f 6d54   and not customT
-000105a0: 6578 7445 6469 746f 722e 7374 7269 7028  extEditor.strip(
-000105b0: 292e 6c6f 7765 7228 2920 3d3d 2063 6f6e  ).lower() == con
-000105c0: 6669 672e 6578 6974 5f65 6e74 7279 3a0a  fig.exit_entry:.
-000105d0: 2020 2020 2020 2020 2020 2020 7465 7874              text
-000105e0: 4564 6974 6f72 203d 2072 652e 7375 6228  Editor = re.sub(
-000105f0: 2220 2e2a 3f24 222c 2022 222c 2063 7573  " .*?$", "", cus
-00010600: 746f 6d54 6578 7445 6469 746f 7229 0a20  tomTextEditor). 
-00010610: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00010620: 7420 7465 7874 4564 6974 6f72 206f 7220  t textEditor or 
-00010630: 6e6f 7420 6973 436f 6d6d 616e 6449 6e73  not isCommandIns
-00010640: 7461 6c6c 6564 2874 6578 7445 6469 746f  talled(textEdito
-00010650: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00010660: 2020 2020 7072 696e 7432 2822 436f 6d6d      print2("Comm
-00010670: 616e 6420 6e6f 7420 666f 756e 6420 6f6e  and not found on
-00010680: 2079 6f75 7220 6465 7669 6365 2122 290a   your device!").
-00010690: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000106a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000106b0: 2020 636f 6e66 6967 2e63 7573 746f 6d54    config.customT
-000106c0: 6578 7445 6469 746f 7220 3d20 6375 7374  extEditor = cust
-000106d0: 6f6d 5465 7874 4564 6974 6f72 0a20 2020  omTextEditor.   
-000106e0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000106f0: 6669 672e 7361 7665 436f 6e66 6967 2829  fig.saveConfig()
-00010700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010710: 2070 7269 6e74 3328 6622 4375 7374 6f6d   print3(f"Custom
-00010720: 2074 6578 7420 6564 6974 6f72 3a20 7b63   text editor: {c
-00010730: 6f6e 6669 672e 6375 7374 6f6d 5465 7874  onfig.customText
-00010740: 4564 6974 6f72 7d22 290a 0a20 2020 2064  Editor}")..    d
-00010750: 6566 2073 6574 4368 6174 5265 636f 7264  ef setChatRecord
-00010760: 436c 6f73 6573 744d 6174 6368 6573 2873  ClosestMatches(s
-00010770: 656c 6629 3a0a 2020 2020 2020 2020 7072  elf):.        pr
-00010780: 696e 7431 2822 506c 6561 7365 2073 7065  int1("Please spe
-00010790: 6369 6679 2074 6865 206e 756d 6265 7220  cify the number 
-000107a0: 6f66 2063 6c6f 7365 7374 206d 6174 6368  of closest match
-000107b0: 6573 2069 6e20 6561 6368 206d 656d 6f72  es in each memor
-000107c0: 7920 7265 7472 6965 7661 6c3a 2229 0a20  y retrieval:"). 
-000107d0: 2020 2020 2020 2063 6861 7452 6563 6f72         chatRecor
-000107e0: 6443 6c6f 7365 7374 4d61 7463 6865 7320  dClosestMatches 
-000107f0: 3d20 7365 6c66 2e70 726f 6d70 7473 2e73  = self.prompts.s
-00010800: 696d 706c 6550 726f 6d70 7428 7374 796c  implePrompt(styl
-00010810: 653d 7365 6c66 2e70 726f 6d70 7473 2e70  e=self.prompts.p
-00010820: 726f 6d70 7453 7479 6c65 322c 206e 756d  romptStyle2, num
-00010830: 6265 724f 6e6c 793d 5472 7565 2c20 6465  berOnly=True, de
-00010840: 6661 756c 743d 7374 7228 636f 6e66 6967  fault=str(config
-00010850: 2e63 6861 7452 6563 6f72 6443 6c6f 7365  .chatRecordClose
-00010860: 7374 4d61 7463 6865 7329 290a 2020 2020  stMatches)).    
-00010870: 2020 2020 6966 2063 6861 7452 6563 6f72      if chatRecor
-00010880: 6443 6c6f 7365 7374 4d61 7463 6865 7320  dClosestMatches 
-00010890: 616e 6420 6e6f 7420 6368 6174 5265 636f  and not chatReco
-000108a0: 7264 436c 6f73 6573 744d 6174 6368 6573  rdClosestMatches
-000108b0: 2e73 7472 6970 2829 2e6c 6f77 6572 2829  .strip().lower()
-000108c0: 203d 3d20 636f 6e66 6967 2e65 7869 745f   == config.exit_
-000108d0: 656e 7472 7920 616e 6420 696e 7428 6368  entry and int(ch
-000108e0: 6174 5265 636f 7264 436c 6f73 6573 744d  atRecordClosestM
-000108f0: 6174 6368 6573 2920 3e3d 2030 3a0a 2020  atches) >= 0:.  
-00010900: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-00010910: 2e63 6861 7452 6563 6f72 6443 6c6f 7365  .chatRecordClose
-00010920: 7374 4d61 7463 6865 7320 3d20 696e 7428  stMatches = int(
-00010930: 6368 6174 5265 636f 7264 436c 6f73 6573  chatRecordCloses
-00010940: 744d 6174 6368 6573 290a 2020 2020 2020  tMatches).      
-00010950: 2020 2020 2020 636f 6e66 6967 2e73 6176        config.sav
-00010960: 6543 6f6e 6669 6728 290a 2020 2020 2020  eConfig().      
-00010970: 2020 2020 2020 7072 696e 7433 2866 224e        print3(f"N
-00010980: 756d 6265 7220 6f66 206d 656d 6f72 7920  umber of memory 
-00010990: 636c 6f73 6573 7420 6d61 7463 6865 733a  closest matches:
-000109a0: 207b 636f 6e66 6967 2e63 6861 7452 6563   {config.chatRec
-000109b0: 6f72 6443 6c6f 7365 7374 4d61 7463 6865  ordClosestMatche
-000109c0: 737d 2229 0a0a 2020 2020 6465 6620 7365  s}")..    def se
-000109d0: 744d 656d 6f72 7943 6c6f 7365 7374 4d61  tMemoryClosestMa
-000109e0: 7463 6865 7328 7365 6c66 293a 0a20 2020  tches(self):.   
-000109f0: 2020 2020 2070 7269 6e74 3128 2250 6c65       print1("Ple
-00010a00: 6173 6520 7370 6563 6966 7920 7468 6520  ase specify the 
-00010a10: 6e75 6d62 6572 206f 6620 636c 6f73 6573  number of closes
-00010a20: 7420 6d61 7463 6865 7320 696e 2065 6163  t matches in eac
-00010a30: 6820 6d65 6d6f 7279 2072 6574 7269 6576  h memory retriev
-00010a40: 616c 3a22 290a 2020 2020 2020 2020 6d65  al:").        me
-00010a50: 6d6f 7279 436c 6f73 6573 744d 6174 6368  moryClosestMatch
-00010a60: 6573 203d 2073 656c 662e 7072 6f6d 7074  es = self.prompt
-00010a70: 732e 7369 6d70 6c65 5072 6f6d 7074 2873  s.simplePrompt(s
-00010a80: 7479 6c65 3d73 656c 662e 7072 6f6d 7074  tyle=self.prompt
-00010a90: 732e 7072 6f6d 7074 5374 796c 6532 2c20  s.promptStyle2, 
-00010aa0: 6e75 6d62 6572 4f6e 6c79 3d54 7275 652c  numberOnly=True,
-00010ab0: 2064 6566 6175 6c74 3d73 7472 2863 6f6e   default=str(con
-00010ac0: 6669 672e 6d65 6d6f 7279 436c 6f73 6573  fig.memoryCloses
-00010ad0: 744d 6174 6368 6573 2929 0a20 2020 2020  tMatches)).     
-00010ae0: 2020 2069 6620 6d65 6d6f 7279 436c 6f73     if memoryClos
-00010af0: 6573 744d 6174 6368 6573 2061 6e64 206e  estMatches and n
-00010b00: 6f74 206d 656d 6f72 7943 6c6f 7365 7374  ot memoryClosest
-00010b10: 4d61 7463 6865 732e 7374 7269 7028 292e  Matches.strip().
-00010b20: 6c6f 7765 7228 2920 3d3d 2063 6f6e 6669  lower() == confi
-00010b30: 672e 6578 6974 5f65 6e74 7279 2061 6e64  g.exit_entry and
-00010b40: 2069 6e74 286d 656d 6f72 7943 6c6f 7365   int(memoryClose
-00010b50: 7374 4d61 7463 6865 7329 203e 3d20 303a  stMatches) >= 0:
-00010b60: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00010b70: 6669 672e 6d65 6d6f 7279 436c 6f73 6573  fig.memoryCloses
-00010b80: 744d 6174 6368 6573 203d 2069 6e74 286d  tMatches = int(m
-00010b90: 656d 6f72 7943 6c6f 7365 7374 4d61 7463  emoryClosestMatc
-00010ba0: 6865 7329 0a20 2020 2020 2020 2020 2020  hes).           
-00010bb0: 2063 6f6e 6669 672e 7361 7665 436f 6e66   config.saveConf
-00010bc0: 6967 2829 0a20 2020 2020 2020 2020 2020  ig().           
-00010bd0: 2070 7269 6e74 3328 6622 4e75 6d62 6572   print3(f"Number
-00010be0: 206f 6620 6d65 6d6f 7279 2063 6c6f 7365   of memory close
-00010bf0: 7374 206d 6174 6368 6573 3a20 7b63 6f6e  st matches: {con
-00010c00: 6669 672e 6d65 6d6f 7279 436c 6f73 6573  fig.memoryCloses
-00010c10: 744d 6174 6368 6573 7d22 290a 0a20 2020  tMatches}")..   
-00010c20: 2064 6566 2073 6574 4d61 7841 7574 6f43   def setMaxAutoC
-00010c30: 6f72 7265 6374 2873 656c 6629 3a0a 2020  orrect(self):.  
-00010c40: 2020 2020 2020 7072 696e 7431 2866 2254        print1(f"T
-00010c50: 6865 2061 7574 6f2d 636f 7272 6563 7469  he auto-correcti
-00010c60: 6f6e 2066 6561 7475 7265 2065 6e61 626c  on feature enabl
-00010c70: 6573 207b 636f 6e66 6967 2e66 7265 6547  es {config.freeG
-00010c80: 656e 6975 7341 494e 616d 657d 2074 6f20  eniusAIName} to 
-00010c90: 6175 746f 6d61 7469 6361 6c6c 7920 6669  automatically fi
-00010ca0: 7820 6272 6f6b 656e 2050 7974 686f 6e20  x broken Python 
-00010cb0: 636f 6465 2069 6620 6974 2077 6173 206e  code if it was n
-00010cc0: 6f74 2065 7865 6375 7465 6420 7072 6f70  ot executed prop
-00010cd0: 6572 6c79 2e22 290a 2020 2020 2020 2020  erly.").        
-00010ce0: 7072 696e 7431 2822 506c 6561 7365 2073  print1("Please s
-00010cf0: 7065 6369 6679 206d 6178 696d 756d 206e  pecify maximum n
-00010d00: 756d 6265 7220 6f66 2061 7574 6f2d 636f  umber of auto-co
-00010d10: 7272 6563 7469 6f6e 2061 7474 656d 7074  rrection attempt
-00010d20: 7320 6265 6c6f 773a 2229 0a20 2020 2020  s below:").     
-00010d30: 2020 2070 7269 6e74 3128 2228 5265 6d61     print1("(Rema
-00010d40: 726b 733a 2045 6e74 6572 2027 3027 2069  rks: Enter '0' i
-00010d50: 6620 796f 7520 7761 6e74 2074 6f20 6469  f you want to di
-00010d60: 7361 626c 6520 6175 746f 2d63 6f72 7265  sable auto-corre
-00010d70: 6374 696f 6e20 6665 6174 7572 6529 2229  ction feature)")
-00010d80: 0a20 2020 2020 2020 206d 6178 4175 746f  .        maxAuto
-00010d90: 436f 7272 6563 7420 3d20 7365 6c66 2e70  Correct = self.p
-00010da0: 726f 6d70 7473 2e73 696d 706c 6550 726f  rompts.simplePro
-00010db0: 6d70 7428 7374 796c 653d 7365 6c66 2e70  mpt(style=self.p
-00010dc0: 726f 6d70 7473 2e70 726f 6d70 7453 7479  rompts.promptSty
-00010dd0: 6c65 322c 206e 756d 6265 724f 6e6c 793d  le2, numberOnly=
-00010de0: 5472 7565 2c20 6465 6661 756c 743d 7374  True, default=st
-00010df0: 7228 636f 6e66 6967 2e6d 6178 5f63 6f6e  r(config.max_con
-00010e00: 7365 6375 7469 7665 5f61 7574 6f5f 636f  secutive_auto_co
-00010e10: 7272 6563 7469 6f6e 2929 0a20 2020 2020  rrection)).     
-00010e20: 2020 2069 6620 6d61 7841 7574 6f43 6f72     if maxAutoCor
-00010e30: 7265 6374 2061 6e64 206e 6f74 206d 6178  rect and not max
-00010e40: 4175 746f 436f 7272 6563 742e 7374 7269  AutoCorrect.stri
-00010e50: 7028 292e 6c6f 7765 7228 2920 3d3d 2063  p().lower() == c
-00010e60: 6f6e 6669 672e 6578 6974 5f65 6e74 7279  onfig.exit_entry
-00010e70: 2061 6e64 2069 6e74 286d 6178 4175 746f   and int(maxAuto
-00010e80: 436f 7272 6563 7429 203e 3d20 303a 0a20  Correct) >= 0:. 
-00010e90: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00010ea0: 672e 6d61 785f 636f 6e73 6563 7574 6976  g.max_consecutiv
-00010eb0: 655f 6175 746f 5f63 6f72 7265 6374 696f  e_auto_correctio
-00010ec0: 6e20 3d20 696e 7428 6d61 7841 7574 6f43  n = int(maxAutoC
-00010ed0: 6f72 7265 6374 290a 2020 2020 2020 2020  orrect).        
-00010ee0: 2020 2020 636f 6e66 6967 2e73 6176 6543      config.saveC
-00010ef0: 6f6e 6669 6728 290a 2020 2020 2020 2020  onfig().        
-00010f00: 2020 2020 7072 696e 7433 2866 224d 6178      print3(f"Max
-00010f10: 696d 756d 2063 6f6e 7365 6375 7469 7665  imum consecutive
-00010f20: 2061 7574 6f2d 636f 7272 6563 7469 6f6e   auto-correction
-00010f30: 3a20 7b63 6f6e 6669 672e 6d61 785f 636f  : {config.max_co
-00010f40: 6e73 6563 7574 6976 655f 6175 746f 5f63  nsecutive_auto_c
-00010f50: 6f72 7265 6374 696f 6e7d 2229 0a0a 2020  orrection}")..  
-00010f60: 2020 6465 6620 7365 744d 696e 546f 6b65    def setMinToke
-00010f70: 6e73 2873 656c 6629 3a0a 2020 2020 2020  ns(self):.      
-00010f80: 2020 7072 696e 7431 2822 506c 6561 7365    print1("Please
-00010f90: 2073 7065 6369 6679 206d 696e 696d 756d   specify minimum
-00010fa0: 206f 7574 7075 7420 746f 6b65 6e73 2062   output tokens b
-00010fb0: 656c 6f77 3a22 290a 2020 2020 2020 2020  elow:").        
-00010fc0: 7072 696e 7431 2822 2861 7070 6c69 6361  print1("(applica
-00010fd0: 626c 6520 746f 2027 6368 6174 6770 7427  ble to 'chatgpt'
-00010fe0: 2061 6e64 2027 6c65 746d 6564 6f69 7427   and 'letmedoit'
-00010ff0: 2069 6e74 6572 6661 6365 7320 6f6e 6c79   interfaces only
-00011000: 2922 290a 2020 2020 2020 2020 6d69 6e74  )").        mint
-00011010: 6f6b 656e 7320 3d20 7365 6c66 2e70 726f  okens = self.pro
-00011020: 6d70 7473 2e73 696d 706c 6550 726f 6d70  mpts.simplePromp
-00011030: 7428 7374 796c 653d 7365 6c66 2e70 726f  t(style=self.pro
-00011040: 6d70 7473 2e70 726f 6d70 7453 7479 6c65  mpts.promptStyle
-00011050: 322c 206e 756d 6265 724f 6e6c 793d 5472  2, numberOnly=Tr
-00011060: 7565 2c20 6465 6661 756c 743d 7374 7228  ue, default=str(
-00011070: 636f 6e66 6967 2e63 6861 7447 5054 4170  config.chatGPTAp
-00011080: 694d 696e 546f 6b65 6e73 2929 0a20 2020  iMinTokens)).   
-00011090: 2020 2020 2069 6620 6d69 6e74 6f6b 656e       if mintoken
-000110a0: 7320 616e 6420 6e6f 7420 6d69 6e74 6f6b  s and not mintok
-000110b0: 656e 732e 7374 7269 7028 292e 6c6f 7765  ens.strip().lowe
-000110c0: 7228 2920 3d3d 2063 6f6e 6669 672e 6578  r() == config.ex
-000110d0: 6974 5f65 6e74 7279 2061 6e64 2069 6e74  it_entry and int
-000110e0: 286d 696e 746f 6b65 6e73 2920 3e20 303a  (mintokens) > 0:
-000110f0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00011100: 6669 672e 6368 6174 4750 5441 7069 4d69  fig.chatGPTApiMi
-00011110: 6e54 6f6b 656e 7320 3d20 696e 7428 6d69  nTokens = int(mi
-00011120: 6e74 6f6b 656e 7329 0a20 2020 2020 2020  ntokens).       
-00011130: 2020 2020 2069 6620 636f 6e66 6967 2e63       if config.c
-00011140: 6861 7447 5054 4170 694d 696e 546f 6b65  hatGPTApiMinToke
-00011150: 6e73 203e 2063 6f6e 6669 672e 6368 6174  ns > config.chat
-00011160: 4750 5441 7069 4d61 7854 6f6b 656e 733a  GPTApiMaxTokens:
-00011170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011180: 2063 6f6e 6669 672e 6368 6174 4750 5441   config.chatGPTA
-00011190: 7069 4d69 6e54 6f6b 656e 7320 3d20 636f  piMinTokens = co
-000111a0: 6e66 6967 2e63 6861 7447 5054 4170 694d  nfig.chatGPTApiM
-000111b0: 6178 546f 6b65 6e73 0a20 2020 2020 2020  axTokens.       
-000111c0: 2020 2020 2063 6f6e 6669 672e 7361 7665       config.save
-000111d0: 436f 6e66 6967 2829 0a20 2020 2020 2020  Config().       
-000111e0: 2020 2020 2070 7269 6e74 3328 6622 4d69       print3(f"Mi
-000111f0: 6e69 6d75 6d20 6f75 7470 7574 2074 6f6b  nimum output tok
-00011200: 656e 733a 207b 636f 6e66 6967 2e63 6861  ens: {config.cha
-00011210: 7447 5054 4170 694d 696e 546f 6b65 6e73  tGPTApiMinTokens
-00011220: 7d22 290a 0a20 2020 2064 6566 2067 6574  }")..    def get
-00011230: 4d61 7854 6f6b 656e 7328 7365 6c66 293a  MaxTokens(self):
-00011240: 0a20 2020 2020 2020 2063 6f6e 7465 7874  .        context
-00011250: 5769 6e64 6f77 4c69 6d69 7420 3d20 746f  WindowLimit = to
-00011260: 6b65 6e4c 696d 6974 735b 636f 6e66 6967  kenLimits[config
-00011270: 2e63 6861 7447 5054 4170 694d 6f64 656c  .chatGPTApiModel
-00011280: 5d0a 2020 2020 2020 2020 6675 6e63 7469  ].        functi
-00011290: 6f6e 546f 6b65 6e73 203d 2063 6f75 6e74  onTokens = count
-000112a0: 5f74 6f6b 656e 735f 6672 6f6d 5f66 756e  _tokens_from_fun
-000112b0: 6374 696f 6e73 2863 6f6e 6669 672e 746f  ctions(config.to
-000112c0: 6f6c 4675 6e63 7469 6f6e 5363 6865 6d61  olFunctionSchema
-000112d0: 732e 7661 6c75 6573 2829 290a 2020 2020  s.values()).    
-000112e0: 2020 2020 6d61 7854 6f6b 656e 203d 2063      maxToken = c
-000112f0: 6f6e 7465 7874 5769 6e64 6f77 4c69 6d69  ontextWindowLimi
-00011300: 7420 2d20 6675 6e63 7469 6f6e 546f 6b65  t - functionToke
-00011310: 6e73 202d 2063 6f6e 6669 672e 6368 6174  ns - config.chat
-00011320: 4750 5441 7069 4d69 6e54 6f6b 656e 730a  GPTApiMinTokens.
-00011330: 2020 2020 2020 2020 6966 206d 6178 546f          if maxTo
-00011340: 6b65 6e20 3e20 3430 3936 2061 6e64 2063  ken > 4096 and c
-00011350: 6f6e 6669 672e 6368 6174 4750 5441 7069  onfig.chatGPTApi
-00011360: 4d6f 6465 6c20 696e 2028 0a20 2020 2020  Model in (.     
-00011370: 2020 2020 2020 2022 6770 742d 342d 7475         "gpt-4-tu
-00011380: 7262 6f22 2c0a 2020 2020 2020 2020 2020  rbo",.          
-00011390: 2020 2267 7074 2d34 2d74 7572 626f 2d70    "gpt-4-turbo-p
-000113a0: 7265 7669 6577 222c 0a20 2020 2020 2020  review",.       
-000113b0: 2020 2020 2022 6770 742d 342d 3031 3235       "gpt-4-0125
-000113c0: 2d70 7265 7669 6577 222c 0a20 2020 2020  -preview",.     
-000113d0: 2020 2020 2020 2022 6770 742d 342d 3131         "gpt-4-11
-000113e0: 3036 2d70 7265 7669 6577 222c 0a20 2020  06-preview",.   
-000113f0: 2020 2020 2020 2020 2022 6770 742d 332e           "gpt-3.
-00011400: 352d 7475 7262 6f22 2c0a 2020 2020 2020  5-turbo",.      
-00011410: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-00011420: 206d 6178 546f 6b65 6e20 3d20 3430 3936   maxToken = 4096
-00011430: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011440: 636f 6e74 6578 7457 696e 646f 774c 696d  contextWindowLim
-00011450: 6974 2c20 6675 6e63 7469 6f6e 546f 6b65  it, functionToke
-00011460: 6e73 2c20 6d61 7854 6f6b 656e 0a0a 2020  ns, maxToken..  
-00011470: 2020 6465 6620 7365 744d 6178 546f 6b65    def setMaxToke
-00011480: 6e73 5f6e 6f6e 5f63 6861 7467 7074 2873  ns_non_chatgpt(s
-00011490: 656c 6629 3a0a 2020 2020 2020 2020 7072  elf):.        pr
-000114a0: 696e 7431 2822 506c 6561 7365 2073 7065  int1("Please spe
-000114b0: 6369 6679 206d 6178 696d 756d 206f 7574  cify maximum out
-000114c0: 7075 7420 746f 6b65 6e73 2062 656c 6f77  put tokens below
-000114d0: 3a22 290a 2020 2020 2020 2020 6966 2063  :").        if c
-000114e0: 6f6e 6669 672e 6c6c 6d49 6e74 6572 6661  onfig.llmInterfa
-000114f0: 6365 203d 3d20 2267 656d 696e 6922 3a0a  ce == "gemini":.
-00011500: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-00011510: 756c 7420 3d20 636f 6e66 6967 2e67 656d  ult = config.gem
-00011520: 696e 6970 726f 5f6d 6178 5f6f 7574 7075  inipro_max_outpu
-00011530: 745f 746f 6b65 6e73 0a20 2020 2020 2020  t_tokens.       
-00011540: 2065 6c69 6620 636f 6e66 6967 2e6c 6c6d   elif config.llm
-00011550: 496e 7465 7266 6163 6520 3d3d 2022 6c6c  Interface == "ll
-00011560: 616d 6163 7070 223a 0a20 2020 2020 2020  amacpp":.       
-00011570: 2020 2020 2064 6566 6175 6c74 203d 2063       default = c
-00011580: 6f6e 6669 672e 6c6c 616d 6163 7070 4d61  onfig.llamacppMa
-00011590: 696e 4d6f 6465 6c5f 6d61 785f 746f 6b65  inModel_max_toke
-000115a0: 6e73 0a20 2020 2020 2020 2065 6c69 6620  ns.        elif 
-000115b0: 636f 6e66 6967 2e6c 6c6d 496e 7465 7266  config.llmInterf
-000115c0: 6163 6520 3d3d 2022 6f6c 6c61 6d61 223a  ace == "ollama":
-000115d0: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-000115e0: 6175 6c74 203d 2063 6f6e 6669 672e 6f6c  ault = config.ol
-000115f0: 6c61 6d61 4d61 696e 4d6f 6465 6c5f 6e75  lamaMainModel_nu
-00011600: 6d5f 7072 6564 6963 740a 2020 2020 2020  m_predict.      
-00011610: 2020 6d61 7874 6f6b 656e 7320 3d20 7365    maxtokens = se
-00011620: 6c66 2e70 726f 6d70 7473 2e73 696d 706c  lf.prompts.simpl
-00011630: 6550 726f 6d70 7428 7374 796c 653d 7365  ePrompt(style=se
-00011640: 6c66 2e70 726f 6d70 7473 2e70 726f 6d70  lf.prompts.promp
-00011650: 7453 7479 6c65 322c 206e 756d 6265 724f  tStyle2, numberO
-00011660: 6e6c 793d 5472 7565 2c20 6465 6661 756c  nly=True, defaul
-00011670: 743d 7374 7228 6465 6661 756c 7429 290a  t=str(default)).
-00011680: 2020 2020 2020 2020 6966 206d 6178 746f          if maxto
-00011690: 6b65 6e73 2061 6e64 206e 6f74 206d 6178  kens and not max
-000116a0: 746f 6b65 6e73 2e73 7472 6970 2829 2e6c  tokens.strip().l
-000116b0: 6f77 6572 2829 203d 3d20 636f 6e66 6967  ower() == config
-000116c0: 2e65 7869 745f 656e 7472 7920 616e 6420  .exit_entry and 
-000116d0: 696e 7428 6d61 7874 6f6b 656e 7329 203e  int(maxtokens) >
-000116e0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-000116f0: 6d61 7874 6f6b 656e 7320 3d20 696e 7428  maxtokens = int(
-00011700: 6d61 7874 6f6b 656e 7329 0a20 2020 2020  maxtokens).     
-00011710: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
-00011720: 2e6c 6c6d 496e 7465 7266 6163 6520 3d3d  .llmInterface ==
-00011730: 2022 6765 6d69 6e69 223a 0a20 2020 2020   "gemini":.     
-00011740: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00011750: 672e 6765 6d69 6e69 7072 6f5f 6d61 785f  g.geminipro_max_
-00011760: 6f75 7470 7574 5f74 6f6b 656e 7320 3d20  output_tokens = 
-00011770: 6d61 7874 6f6b 656e 730a 2020 2020 2020  maxtokens.      
-00011780: 2020 2020 2020 656c 6966 2063 6f6e 6669        elif confi
-00011790: 672e 6c6c 6d49 6e74 6572 6661 6365 203d  g.llmInterface =
-000117a0: 3d20 226c 6c61 6d61 6370 7022 3a0a 2020  = "llamacpp":.  
-000117b0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000117c0: 6e66 6967 2e6c 6c61 6d61 6370 704d 6169  nfig.llamacppMai
-000117d0: 6e4d 6f64 656c 5f6d 6178 5f74 6f6b 656e  nModel_max_token
-000117e0: 7320 3d20 6d61 7874 6f6b 656e 730a 2020  s = maxtokens.  
-000117f0: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
-00011800: 6f6e 6669 672e 6c6c 6d49 6e74 6572 6661  onfig.llmInterfa
-00011810: 6365 203d 3d20 226f 6c6c 616d 6122 3a0a  ce == "ollama":.
-00011820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011830: 636f 6e66 6967 2e6f 6c6c 616d 614d 6169  config.ollamaMai
-00011840: 6e4d 6f64 656c 5f6e 756d 5f70 7265 6469  nModel_num_predi
-00011850: 6374 203d 206d 6178 746f 6b65 6e73 0a20  ct = maxtokens. 
-00011860: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00011870: 672e 7361 7665 436f 6e66 6967 2829 0a20  g.saveConfig(). 
-00011880: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00011890: 3328 6622 4d61 7869 6d75 6d20 6f75 7470  3(f"Maximum outp
-000118a0: 7574 2074 6f6b 656e 733a 207b 636f 6e66  ut tokens: {conf
-000118b0: 6967 2e63 6861 7447 5054 4170 694d 696e  ig.chatGPTApiMin
-000118c0: 546f 6b65 6e73 7d22 290a 0a20 2020 2064  Tokens}")..    d
-000118d0: 6566 2073 6574 4d61 7854 6f6b 656e 7328  ef setMaxTokens(
-000118e0: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
-000118f0: 206e 6f6e 2d63 6861 7467 7074 2073 6574   non-chatgpt set
-00011900: 7469 6e67 730a 2020 2020 2020 2020 6966  tings.        if
-00011910: 206e 6f74 2063 6f6e 6669 672e 6c6c 6d49   not config.llmI
-00011920: 6e74 6572 6661 6365 2069 6e20 2822 6368  nterface in ("ch
-00011930: 6174 6770 7422 2c20 226c 6574 6d65 646f  atgpt", "letmedo
-00011940: 6974 2229 3a0a 2020 2020 2020 2020 2020  it"):.          
-00011950: 2020 7365 6c66 2e73 6574 4d61 7854 6f6b    self.setMaxTok
-00011960: 656e 735f 6e6f 6e5f 6368 6174 6770 7428  ens_non_chatgpt(
-00011970: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00011980: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-00011990: 2020 2320 6368 6174 6770 7420 7365 7474    # chatgpt sett
-000119a0: 696e 6773 0a20 2020 2020 2020 2063 6f6e  ings.        con
-000119b0: 7465 7874 5769 6e64 6f77 4c69 6d69 742c  textWindowLimit,
-000119c0: 2066 756e 6374 696f 6e54 6f6b 656e 732c   functionTokens,
-000119d0: 2074 6f6b 656e 4c69 6d69 7420 3d20 7365   tokenLimit = se
-000119e0: 6c66 2e67 6574 4d61 7854 6f6b 656e 7328  lf.getMaxTokens(
-000119f0: 290a 2020 2020 2020 2020 6966 2074 6f6b  ).        if tok
-00011a00: 656e 4c69 6d69 7420 3c20 636f 6e66 6967  enLimit < config
-00011a10: 2e63 6861 7447 5054 4170 694d 696e 546f  .chatGPTApiMinTo
-00011a20: 6b65 6e73 3a0a 2020 2020 2020 2020 2020  kens:.          
-00011a30: 2020 7072 696e 7432 2866 2246 756e 6374    print2(f"Funct
-00011a40: 696f 6e20 746f 6b65 6e73 205b 7b66 756e  ion tokens [{fun
-00011a50: 6374 696f 6e54 6f6b 656e 737d 5d20 6578  ctionTokens}] ex
-00011a60: 6365 6564 207b 636f 6e66 6967 2e63 6861  ceed {config.cha
-00011a70: 7447 5054 4170 694d 6f64 656c 7d20 6f75  tGPTApiModel} ou
-00011a80: 7470 7574 2074 6f6b 656e 206c 696d 6974  tput token limit
-00011a90: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-00011aa0: 7072 696e 7431 2822 4569 7468 6572 2063  print1("Either c
-00011ab0: 6861 6e67 6520 746f 2061 206d 6f64 656c  hange to a model
-00011ac0: 2077 6974 6820 6869 6768 6572 2074 6f6b   with higher tok
-00011ad0: 656e 206c 696d 6974 206f 7220 6469 7361  en limit or disa
-00011ae0: 626c 6520 756e 7573 6564 2066 756e 6374  ble unused funct
-00011af0: 696f 6e2d 6361 6c6c 2070 6c67 7569 6e73  ion-call plguins
-00011b00: 2e22 290a 2020 2020 2020 2020 656c 7365  .").        else
-00011b10: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00011b20: 696e 7431 2873 656c 662e 6469 7669 6465  int1(self.divide
-00011b30: 7229 0a20 2020 2020 2020 2020 2020 2070  r).            p
-00011b40: 7269 6e74 3128 2247 5054 2061 6e64 2065  rint1("GPT and e
-00011b50: 6d62 6564 6469 6e67 7320 6d6f 6465 6c73  mbeddings models
-00011b60: 2070 726f 6365 7373 2074 6578 7420 696e   process text in
-00011b70: 2063 6875 6e6b 7320 6361 6c6c 6564 2074   chunks called t
-00011b80: 6f6b 656e 732e 2041 7320 6120 726f 7567  okens. As a roug
-00011b90: 6820 7275 6c65 206f 6620 7468 756d 622c  h rule of thumb,
-00011ba0: 2031 2074 6f6b 656e 2069 7320 6170 7072   1 token is appr
-00011bb0: 6f78 696d 6174 656c 7920 3420 6368 6172  oximately 4 char
-00011bc0: 6163 7465 7273 206f 7220 302e 3735 2077  acters or 0.75 w
-00011bd0: 6f72 6473 2066 6f72 2045 6e67 6c69 7368  ords for English
-00011be0: 2074 6578 742e 204f 6e65 206c 696d 6974   text. One limit
-00011bf0: 6174 696f 6e20 746f 206b 6565 7020 696e  ation to keep in
-00011c00: 206d 696e 6420 6973 2074 6861 7420 666f   mind is that fo
-00011c10: 7220 6120 4750 5420 6d6f 6465 6c20 7468  r a GPT model th
-00011c20: 6520 7072 6f6d 7074 2061 6e64 2074 6865  e prompt and the
-00011c30: 2067 656e 6572 6174 6564 206f 7574 7075   generated outpu
-00011c40: 7420 636f 6d62 696e 6564 206d 7573 7420  t combined must 
-00011c50: 6265 206e 6f20 6d6f 7265 2074 6861 6e20  be no more than 
-00011c60: 7468 6520 6d6f 6465 6c27 7320 6d61 7869  the model's maxi
-00011c70: 6d75 6d20 636f 6e74 6578 7420 6c65 6e67  mum context leng
-00011c80: 7468 2e22 290a 2020 2020 2020 2020 2020  th.").          
-00011c90: 2020 7072 696e 7433 2866 2243 7572 7265    print3(f"Curre
-00011ca0: 6e74 2047 5054 206d 6f64 656c 3a20 7b63  nt GPT model: {c
-00011cb0: 6f6e 6669 672e 6368 6174 4750 5441 7069  onfig.chatGPTApi
-00011cc0: 4d6f 6465 6c7d 2229 0a20 2020 2020 2020  Model}").       
-00011cd0: 2020 2020 2070 7269 6e74 3328 6622 4d61       print3(f"Ma
-00011ce0: 7869 6d75 6d20 636f 6e74 6578 7420 6c65  ximum context le
-00011cf0: 6e67 7468 3a20 7b63 6f6e 7465 7874 5769  ngth: {contextWi
-00011d00: 6e64 6f77 4c69 6d69 747d 2229 0a20 2020  ndowLimit}").   
-00011d10: 2020 2020 2020 2020 2070 7269 6e74 3328           print3(
-00011d20: 6622 4375 7272 656e 7420 6675 6e63 7469  f"Current functi
-00011d30: 6f6e 2074 6f6b 656e 733a 207b 6675 6e63  on tokens: {func
-00011d40: 7469 6f6e 546f 6b65 6e73 7d22 290a 2020  tionTokens}").  
-00011d50: 2020 2020 2020 2020 2020 7072 696e 7433            print3
-00011d60: 2866 224d 6178 696d 756d 206f 7574 7075  (f"Maximum outpu
-00011d70: 7420 746f 6b65 6e20 616c 6c6f 7765 6420  t token allowed 
-00011d80: 2865 7863 6c2e 2066 756e 6374 696f 6e73  (excl. functions
-00011d90: 293a 207b 746f 6b65 6e4c 696d 6974 7d22  ): {tokenLimit}"
-00011da0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00011db0: 696e 7431 2873 656c 662e 6469 7669 6465  int1(self.divide
-00011dc0: 7229 0a20 2020 2020 2020 2020 2020 2070  r).            p
-00011dd0: 7269 6e74 3128 2250 6c65 6173 6520 7370  rint1("Please sp
-00011de0: 6563 6966 7920 6d61 7869 6d75 6d20 6f75  ecify maximum ou
-00011df0: 7470 7574 2074 6f6b 656e 7320 6265 6c6f  tput tokens belo
-00011e00: 773a 2229 0a20 2020 2020 2020 2020 2020  w:").           
-00011e10: 206d 6178 746f 6b65 6e73 203d 2073 656c   maxtokens = sel
-00011e20: 662e 7072 6f6d 7074 732e 7369 6d70 6c65  f.prompts.simple
-00011e30: 5072 6f6d 7074 2873 7479 6c65 3d73 656c  Prompt(style=sel
-00011e40: 662e 7072 6f6d 7074 732e 7072 6f6d 7074  f.prompts.prompt
-00011e50: 5374 796c 6532 2c20 6e75 6d62 6572 4f6e  Style2, numberOn
-00011e60: 6c79 3d54 7275 652c 2064 6566 6175 6c74  ly=True, default
-00011e70: 3d73 7472 2863 6f6e 6669 672e 6368 6174  =str(config.chat
-00011e80: 4750 5441 7069 4d61 7854 6f6b 656e 7329  GPTApiMaxTokens)
-00011e90: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00011ea0: 206d 6178 746f 6b65 6e73 2061 6e64 206e   maxtokens and n
-00011eb0: 6f74 206d 6178 746f 6b65 6e73 2e73 7472  ot maxtokens.str
-00011ec0: 6970 2829 2e6c 6f77 6572 2829 203d 3d20  ip().lower() == 
-00011ed0: 636f 6e66 6967 2e65 7869 745f 656e 7472  config.exit_entr
-00011ee0: 7920 616e 6420 696e 7428 6d61 7874 6f6b  y and int(maxtok
-00011ef0: 656e 7329 203e 2030 3a0a 2020 2020 2020  ens) > 0:.      
-00011f00: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-00011f10: 2e63 6861 7447 5054 4170 694d 6178 546f  .chatGPTApiMaxTo
-00011f20: 6b65 6e73 203d 2069 6e74 286d 6178 746f  kens = int(maxto
-00011f30: 6b65 6e73 290a 2020 2020 2020 2020 2020  kens).          
-00011f40: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
-00011f50: 6368 6174 4750 5441 7069 4d61 7854 6f6b  chatGPTApiMaxTok
-00011f60: 656e 7320 3e20 746f 6b65 6e4c 696d 6974  ens > tokenLimit
-00011f70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011f80: 2020 2020 2020 636f 6e66 6967 2e63 6861        config.cha
-00011f90: 7447 5054 4170 694d 6178 546f 6b65 6e73  tGPTApiMaxTokens
-00011fa0: 203d 2074 6f6b 656e 4c69 6d69 740a 2020   = tokenLimit.  
-00011fb0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00011fc0: 6e66 6967 2e73 6176 6543 6f6e 6669 6728  nfig.saveConfig(
-00011fd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011fe0: 2020 7072 696e 7433 2866 224d 6178 696d    print3(f"Maxim
-00011ff0: 756d 206f 7574 7075 7420 746f 6b65 6e73  um output tokens
-00012000: 3a20 7b63 6f6e 6669 672e 6368 6174 4750  : {config.chatGP
-00012010: 5441 7069 4d61 7854 6f6b 656e 737d 2229  TApiMaxTokens}")
-00012020: 0a0a 2020 2020 6465 6620 7275 6e53 7973  ..    def runSys
-00012030: 7465 6d43 6f6d 6d61 6e64 2873 656c 662c  temCommand(self,
-00012040: 2063 6f6d 6d61 6e64 293a 0a20 2020 2020   command):.     
-00012050: 2020 2063 6f6d 6d61 6e64 203d 2063 6f6d     command = com
-00012060: 6d61 6e64 2e73 7472 6970 2829 5b31 3a5d  mand.strip()[1:]
-00012070: 0a20 2020 2020 2020 2069 6620 225c 6e22  .        if "\n"
-00012080: 2069 6e20 636f 6d6d 616e 643a 0a20 2020   in command:.   
-00012090: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
-000120a0: 203d 2022 3b22 2e6a 6f69 6e28 636f 6d6d   = ";".join(comm
-000120b0: 616e 642e 7370 6c69 7428 225c 6e22 2929  and.split("\n"))
-000120c0: 0a20 2020 2020 2020 2069 6620 636f 6e66  .        if conf
-000120d0: 6967 2e74 6869 7350 6c61 7466 6f72 6d20  ig.thisPlatform 
-000120e0: 3d3d 2022 5769 6e64 6f77 7322 3a0a 2020  == "Windows":.  
-000120f0: 2020 2020 2020 2020 2020 6f73 2e73 7973            os.sys
-00012100: 7465 6d28 636f 6d6d 616e 6429 0a20 2020  tem(command).   
-00012110: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00012120: 2020 2020 2020 206f 732e 7379 7374 656d         os.system
-00012130: 2866 2265 6e76 2051 545f 5150 415f 504c  (f"env QT_QPA_PL
-00012140: 4154 464f 524d 5f50 4c55 4749 4e5f 5041  ATFORM_PLUGIN_PA
-00012150: 5448 3d27 7b63 6f6e 6669 672e 656e 765f  TH='{config.env_
-00012160: 5154 5f51 5041 5f50 4c41 5446 4f52 4d5f  QT_QPA_PLATFORM_
-00012170: 504c 5547 494e 5f50 4154 487d 2720 7b63  PLUGIN_PATH}' {c
-00012180: 6f6d 6d61 6e64 7d22 290a 0a20 2020 2064  ommand}")..    d
-00012190: 6566 2074 6f67 676c 654d 756c 7469 6c69  ef toggleMultili
-000121a0: 6e65 2873 656c 6629 3a0a 2020 2020 2020  ne(self):.      
-000121b0: 2020 636f 6e66 6967 2e6d 756c 7469 6c69    config.multili
-000121c0: 6e65 496e 7075 7420 3d20 6e6f 7420 636f  neInput = not co
-000121d0: 6e66 6967 2e6d 756c 7469 6c69 6e65 496e  nfig.multilineIn
-000121e0: 7075 740a 2020 2020 2020 2020 7275 6e5f  put.        run_
-000121f0: 696e 5f74 6572 6d69 6e61 6c28 6c61 6d62  in_terminal(lamb
-00012200: 6461 3a20 7072 696e 7431 2866 224d 756c  da: print1(f"Mul
-00012210: 7469 2d6c 696e 6520 696e 7075 7420 7b27  ti-line input {'
-00012220: 656e 6162 6c65 6427 2069 6620 636f 6e66  enabled' if conf
-00012230: 6967 2e6d 756c 7469 6c69 6e65 496e 7075  ig.multilineInpu
-00012240: 7420 656c 7365 2027 6469 7361 626c 6564  t else 'disabled
-00012250: 277d 2122 2929 0a20 2020 2020 2020 2069  '}!")).        i
-00012260: 6620 636f 6e66 6967 2e6d 756c 7469 6c69  f config.multili
-00012270: 6e65 496e 7075 743a 0a20 2020 2020 2020  neInput:.       
-00012280: 2020 2020 2072 756e 5f69 6e5f 7465 726d       run_in_term
-00012290: 696e 616c 286c 616d 6264 613a 2070 7269  inal(lambda: pri
-000122a0: 6e74 3128 2255 7365 2027 6573 6361 7065  nt1("Use 'escape
-000122b0: 202b 2065 6e74 6572 2720 746f 2063 6f6d   + enter' to com
-000122c0: 706c 6574 6520 796f 7572 2065 6e74 7279  plete your entry
-000122d0: 2e22 2929 0a0a 2020 2020 6465 6620 6973  ."))..    def is
-000122e0: 5474 7341 7661 696c 6162 6c65 2873 656c  TtsAvailable(sel
-000122f0: 6629 3a0a 2020 2020 2020 2020 6966 206e  f):.        if n
-00012300: 6f74 2063 6f6e 6669 672e 6973 566c 6350  ot config.isVlcP
-00012310: 6c61 7965 7249 6e73 7461 6c6c 6564 2061  layerInstalled a
-00012320: 6e64 206e 6f74 2063 6f6e 6669 672e 6973  nd not config.is
-00012330: 5079 6761 6d65 496e 7374 616c 6c65 6420  PygameInstalled 
-00012340: 616e 6420 6e6f 7420 636f 6e66 6967 2e74  and not config.t
-00012350: 7473 436f 6d6d 616e 6420 616e 6420 6e6f  tsCommand and no
-00012360: 7420 636f 6e66 6967 2e65 6c65 7665 6e6c  t config.elevenl
-00012370: 6162 7341 7069 3a0a 2020 2020 2020 2020  absApi:.        
-00012380: 2020 2020 7072 696e 7432 2822 5465 7874      print2("Text
-00012390: 2d74 6f2d 7370 6565 6368 2066 6561 7475  -to-speech featu
-000123a0: 7265 2069 7320 6e6f 7420 656e 6162 6c65  re is not enable
-000123b0: 6421 2229 0a20 2020 2020 2020 2020 2020  d!").           
-000123c0: 2070 7269 6e74 3328 2252 6561 643a 2068   print3("Read: h
-000123d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000123e0: 6d2f 656c 6972 616e 776f 6e67 2f6c 6574  m/eliranwong/let
-000123f0: 6d65 646f 6974 2f77 696b 692f 6c65 744d  medoit/wiki/letM
-00012400: 6544 6f49 742d 5370 6561 6b73 2229 0a20  eDoIt-Speaks"). 
-00012410: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00012420: 672e 7474 7320 3d20 4661 6c73 650a 2020  g.tts = False.  
-00012430: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00012440: 2020 2020 2020 2020 636f 6e66 6967 2e74          config.t
-00012450: 7473 203d 2054 7275 650a 2020 2020 2020  ts = True.      
-00012460: 2020 7265 7475 726e 2063 6f6e 6669 672e    return config.
-00012470: 7474 730a 0a20 2020 2064 6566 2074 6f67  tts..    def tog
-00012480: 676c 6569 6e70 7574 6175 6469 6f28 7365  gleinputaudio(se
-00012490: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-000124a0: 7365 6c66 2e69 7354 7473 4176 6169 6c61  self.isTtsAvaila
-000124b0: 626c 653a 0a20 2020 2020 2020 2020 2020  ble:.           
-000124c0: 2063 6f6e 6669 672e 7474 7349 6e70 7574   config.ttsInput
-000124d0: 203d 206e 6f74 2063 6f6e 6669 672e 7474   = not config.tt
-000124e0: 7349 6e70 7574 0a20 2020 2020 2020 2020  sInput.         
-000124f0: 2020 2063 6f6e 6669 672e 7361 7665 436f     config.saveCo
-00012500: 6e66 6967 2829 0a20 2020 2020 2020 2020  nfig().         
-00012510: 2020 2070 7269 6e74 3328 6622 496e 7075     print3(f"Inpu
-00012520: 7420 4175 6469 6f3a 2027 7b27 656e 6162  t Audio: '{'enab
-00012530: 6c65 6427 2069 6620 636f 6e66 6967 2e74  led' if config.t
-00012540: 7473 496e 7075 7420 656c 7365 2027 6469  tsInput else 'di
-00012550: 7361 626c 6564 277d 2721 2229 0a0a 2020  sabled'}'!")..  
-00012560: 2020 6465 6620 746f 6767 6c65 7265 7370    def toggleresp
-00012570: 6f6e 7365 6175 6469 6f28 7365 6c66 293a  onseaudio(self):
-00012580: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00012590: 2e69 7354 7473 4176 6169 6c61 626c 653a  .isTtsAvailable:
-000125a0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-000125b0: 6669 672e 7474 734f 7574 7075 7420 3d20  fig.ttsOutput = 
-000125c0: 6e6f 7420 636f 6e66 6967 2e74 7473 4f75  not config.ttsOu
-000125d0: 7470 7574 0a20 2020 2020 2020 2020 2020  tput.           
-000125e0: 2063 6f6e 6669 672e 7361 7665 436f 6e66   config.saveConf
-000125f0: 6967 2829 0a20 2020 2020 2020 2020 2020  ig().           
-00012600: 2070 7269 6e74 3328 6622 5265 7370 6f6e   print3(f"Respon
-00012610: 7365 2041 7564 696f 3a20 277b 2765 6e61  se Audio: '{'ena
-00012620: 626c 6564 2720 6966 2063 6f6e 6669 672e  bled' if config.
-00012630: 7474 734f 7574 7075 7420 656c 7365 2027  ttsOutput else '
-00012640: 6469 7361 626c 6564 277d 2721 2229 0a0a  disabled'}'!")..
-00012650: 2020 2020 6465 6620 6465 6669 6e65 5474      def defineTt
-00012660: 7343 6f6d 6d61 6e64 2873 656c 6629 3a0a  sCommand(self):.
-00012670: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
-00012680: 4465 6669 6e65 2063 7573 746f 6d20 7465  Define custom te
-00012690: 7874 2d74 6f2d 7370 6565 6368 2063 6f6d  xt-to-speech com
-000126a0: 6d61 6e64 2062 656c 6f77 3a22 290a 2020  mand below:").  
-000126b0: 2020 2020 2020 7072 696e 7431 2822 2222        print1("""
-000126c0: 2a20 6f6e 206d 6163 4f53 205b 2773 6179  * on macOS ['say
-000126d0: 202d 7620 223f 2227 2074 6f20 6368 6563   -v "?"' to chec
-000126e0: 6b20 766f 6963 6573 5d2c 2065 2e67 2e3a  k voices], e.g.:
-000126f0: 5c6e 2773 6179 2720 6f72 2027 7361 7920  \n'say' or 'say 
-00012700: 2d72 2032 3030 202d 7620 4461 6e69 656c  -r 200 -v Daniel
-00012710: 2722 2222 290a 2020 2020 2020 2020 7072  '""").        pr
-00012720: 696e 7431 2822 2a20 6f6e 2055 6275 6e74  int1("* on Ubunt
-00012730: 7520 5b27 6573 7065 616b 202d 2d76 6f69  u ['espeak --voi
-00012740: 6365 7327 2074 6f20 6368 6563 6b20 766f  ces' to check vo
-00012750: 6963 6573 5d2c 2065 2e67 2e3a 5c6e 2765  ices], e.g.:\n'e
-00012760: 7370 6561 6b27 206f 7220 2765 7370 6561  speak' or 'espea
-00012770: 6b20 2d73 2031 3735 202d 7620 656e 2d67  k -s 175 -v en-g
-00012780: 6227 2229 0a20 2020 2020 2020 2070 7269  b'").        pri
-00012790: 6e74 3128 222a 206f 6e20 5769 6e64 6f77  nt1("* on Window
-000127a0: 732c 2073 696d 706c 7920 656e 7465 7220  s, simply enter 
-000127b0: 2777 696e 646f 7773 2720 6865 7265 2074  'windows' here t
-000127c0: 6f20 7573 6520 5769 6e64 6f77 7320 6275  o use Windows bu
-000127d0: 696c 742d 696e 2073 7065 6563 6820 656e  ilt-in speech en
-000127e0: 6769 6e65 2229 2023 206c 6574 6d65 646f  gine") # letmedo
-000127f0: 6974 2e61 6920 7769 6c6c 2068 616e 646c  it.ai will handl
-00012800: 6520 7468 6520 636f 6d6d 616e 6420 666f  e the command fo
-00012810: 7220 5769 6e64 6f77 7320 7573 6572 730a  r Windows users.
-00012820: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
-00012830: 7265 6d61 726b 733a 2061 6c77 6179 7320  remarks: always 
-00012840: 706c 6163 6520 7468 6520 766f 6963 6520  place the voice 
-00012850: 6f70 7469 6f6e 2c20 6966 2061 6e79 2c20  option, if any, 
-00012860: 6174 2074 6865 2065 6e64 2229 0a20 2020  at the end").   
-00012870: 2020 2020 2074 7473 436f 6d6d 616e 6420       ttsCommand 
-00012880: 3d20 7365 6c66 2e70 726f 6d70 7473 2e73  = self.prompts.s
-00012890: 696d 706c 6550 726f 6d70 7428 7374 796c  implePrompt(styl
-000128a0: 653d 7365 6c66 2e70 726f 6d70 7473 2e70  e=self.prompts.p
-000128b0: 726f 6d70 7453 7479 6c65 322c 2064 6566  romptStyle2, def
-000128c0: 6175 6c74 3d63 6f6e 6669 672e 7474 7343  ault=config.ttsC
-000128d0: 6f6d 6d61 6e64 290a 2020 2020 2020 2020  ommand).        
-000128e0: 6966 2074 7473 436f 6d6d 616e 643a 0a20  if ttsCommand:. 
-000128f0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00012900: 3128 2253 7065 6369 6679 2063 6f6d 6d61  1("Specify comma
-00012910: 6e64 2073 7566 6669 7820 6265 6c6f 772c  nd suffix below,
-00012920: 2069 6620 616e 7920 5b6c 6561 7665 2069   if any [leave i
-00012930: 7420 626c 616e 6b20 6966 204e 2f41 5d3a  t blank if N/A]:
-00012940: 2229 0a20 2020 2020 2020 2020 2020 2074  ").            t
-00012950: 7473 436f 6d6d 616e 6453 7566 6669 7820  tsCommandSuffix 
-00012960: 3d20 7365 6c66 2e70 726f 6d70 7473 2e73  = self.prompts.s
-00012970: 696d 706c 6550 726f 6d70 7428 7374 796c  implePrompt(styl
-00012980: 653d 7365 6c66 2e70 726f 6d70 7473 2e70  e=self.prompts.p
-00012990: 726f 6d70 7453 7479 6c65 322c 2064 6566  romptStyle2, def
-000129a0: 6175 6c74 3d63 6f6e 6669 672e 7474 7343  ault=config.ttsC
-000129b0: 6f6d 6d61 6e64 5375 6666 6978 290a 2020  ommandSuffix).  
-000129c0: 2020 2020 2020 2020 2020 6966 2074 7473            if tts
-000129d0: 436f 6d6d 616e 642e 6c6f 7765 7228 2920  Command.lower() 
-000129e0: 3d3d 2022 7769 6e64 6f77 7322 3a0a 2020  == "windows":.  
-000129f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00012a00: 6d6d 616e 6420 3d20 6627 2727 506f 7765  mmand = f'''Powe
-00012a10: 7253 6865 6c6c 202d 436f 6d6d 616e 6420  rShell -Command 
-00012a20: 2241 6464 2d54 7970 6520 e280 9341 7373  "Add-Type ...Ass
-00012a30: 656d 626c 794e 616d 6520 5379 7374 656d  emblyName System
-00012a40: 2e53 7065 6563 683b 2028 4e65 772d 4f62  .Speech; (New-Ob
-00012a50: 6a65 6374 2053 7973 7465 6d2e 5370 6565  ject System.Spee
-00012a60: 6368 2e53 796e 7468 6573 6973 2e53 7065  ch.Synthesis.Spe
-00012a70: 6563 6853 796e 7468 6573 697a 6572 292e  echSynthesizer).
-00012a80: 5370 6561 6b28 2774 6573 7469 6e67 2729  Speak('testing')
-00012a90: 3b22 2727 270a 2020 2020 2020 2020 2020  ;"'''.          
-00012aa0: 2020 2020 2020 7474 7343 6f6d 6d61 6e64        ttsCommand
-00012ab0: 5375 6666 6978 203d 2022 220a 2020 2020  Suffix = "".    
-00012ac0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00012ae0: 6d6d 616e 6420 3d20 6627 2727 7b74 7473  mmand = f'''{tts
-00012af0: 436f 6d6d 616e 647d 2022 7465 7374 696e  Command} "testin
-00012b00: 6722 7b74 7473 436f 6d6d 616e 6453 7566  g"{ttsCommandSuf
-00012b10: 6669 787d 2727 270a 2020 2020 2020 2020  fix}'''.        
-00012b20: 2020 2020 5f2c 2073 7464 4572 7220 3d20      _, stdErr = 
-00012b30: 7375 6270 726f 6365 7373 2e50 6f70 656e  subprocess.Popen
-00012b40: 2863 6f6d 6d61 6e64 2c20 7368 656c 6c3d  (command, shell=
-00012b50: 5472 7565 2c20 7374 646f 7574 3d73 7562  True, stdout=sub
-00012b60: 7072 6f63 6573 732e 5049 5045 2c20 7374  process.PIPE, st
-00012b70: 6465 7272 3d73 7562 7072 6f63 6573 732e  derr=subprocess.
-00012b80: 5049 5045 292e 636f 6d6d 756e 6963 6174  PIPE).communicat
-00012b90: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00012ba0: 6966 2073 7464 4572 723a 0a20 2020 2020  if stdErr:.     
-00012bb0: 2020 2020 2020 2020 2020 2073 686f 7745             showE
-00012bc0: 7272 6f72 7328 2920 6966 2063 6f6e 6669  rrors() if confi
-00012bd0: 672e 6465 7665 6c6f 7065 7220 656c 7365  g.developer else
-00012be0: 2070 7269 6e74 3128 2245 6e74 6572 6564   print1("Entered
-00012bf0: 2063 6f6d 6d61 6e64 2069 6e76 616c 6964   command invalid
-00012c00: 2122 290a 2020 2020 2020 2020 2020 2020  !").            
-00012c10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00012c20: 2020 2020 2020 636f 6e66 6967 2e74 7473        config.tts
-00012c30: 436f 6d6d 616e 642c 2063 6f6e 6669 672e  Command, config.
-00012c40: 7474 7343 6f6d 6d61 6e64 5375 6666 6978  ttsCommandSuffix
-00012c50: 203d 2074 7473 436f 6d6d 616e 642c 2074   = ttsCommand, t
-00012c60: 7473 436f 6d6d 616e 6453 7566 6669 780a  tsCommandSuffix.
-00012c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c80: 636f 6e66 6967 2e73 6176 6543 6f6e 6669  config.saveConfi
-00012c90: 6728 290a 2020 2020 2020 2020 656c 7365  g().        else
-00012ca0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00012cb0: 6e66 6967 2e74 7473 436f 6d6d 616e 642c  nfig.ttsCommand,
-00012cc0: 2063 6f6e 6669 672e 7474 7343 6f6d 6d61   config.ttsComma
-00012cd0: 6e64 5375 6666 6978 203d 2022 222c 2022  ndSuffix = "", "
-00012ce0: 220a 0a20 2020 2064 6566 2074 6f67 676c  "..    def toggl
-00012cf0: 6557 6f72 6457 7261 7028 7365 6c66 293a  eWordWrap(self):
-00012d00: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
-00012d10: 7772 6170 576f 7264 7320 3d20 6e6f 7420  wrapWords = not 
-00012d20: 636f 6e66 6967 2e77 7261 7057 6f72 6473  config.wrapWords
-00012d30: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
-00012d40: 7361 7665 436f 6e66 6967 2829 0a20 2020  saveConfig().   
-00012d50: 2020 2020 2070 7269 6e74 3328 6622 576f       print3(f"Wo
-00012d60: 7264 2057 7261 703a 2027 7b27 656e 6162  rd Wrap: '{'enab
-00012d70: 6c65 6427 2069 6620 636f 6e66 6967 2e77  led' if config.w
-00012d80: 7261 7057 6f72 6473 2065 6c73 6520 2764  rapWords else 'd
-00012d90: 6973 6162 6c65 6427 7d27 2122 290a 0a20  isabled'}'!").. 
-00012da0: 2020 2064 6566 2074 6f67 676c 654d 6f75     def toggleMou
-00012db0: 7365 5375 7070 6f72 7428 7365 6c66 293a  seSupport(self):
-00012dc0: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
-00012dd0: 6d6f 7573 6553 7570 706f 7274 203d 206e  mouseSupport = n
-00012de0: 6f74 2063 6f6e 6669 672e 6d6f 7573 6553  ot config.mouseS
-00012df0: 7570 706f 7274 0a20 2020 2020 2020 2063  upport.        c
-00012e00: 6f6e 6669 672e 7361 7665 436f 6e66 6967  onfig.saveConfig
-00012e10: 2829 0a20 2020 2020 2020 2070 7269 6e74  ().        print
-00012e20: 3328 6622 456e 7472 7920 4d6f 7573 6520  3(f"Entry Mouse 
-00012e30: 5375 7070 6f72 743a 2027 7b27 656e 6162  Support: '{'enab
-00012e40: 6c65 6427 2069 6620 636f 6e66 6967 2e6d  led' if config.m
-00012e50: 6f75 7365 5375 7070 6f72 7420 656c 7365  ouseSupport else
-00012e60: 2027 6469 7361 626c 6564 277d 2721 2229   'disabled'}'!")
-00012e70: 0a0a 2020 2020 6465 6620 746f 6767 6c65  ..    def toggle
-00012e80: 496d 7072 6f76 6564 5772 6974 696e 6728  ImprovedWriting(
-00012e90: 7365 6c66 293a 0a20 2020 2020 2020 2063  self):.        c
-00012ea0: 6f6e 6669 672e 6469 7370 6c61 7949 6d70  onfig.displayImp
-00012eb0: 726f 7665 6457 7269 7469 6e67 203d 206e  rovedWriting = n
-00012ec0: 6f74 2063 6f6e 6669 672e 6469 7370 6c61  ot config.displa
-00012ed0: 7949 6d70 726f 7665 6457 7269 7469 6e67  yImprovedWriting
-00012ee0: 0a20 2020 2020 2020 2069 6620 636f 6e66  .        if conf
-00012ef0: 6967 2e64 6973 706c 6179 496d 7072 6f76  ig.displayImprov
-00012f00: 6564 5772 6974 696e 673a 0a20 2020 2020  edWriting:.     
-00012f10: 2020 2020 2020 2070 7269 6e74 3128 2250         print1("P
-00012f20: 6c65 6173 6520 7370 6563 6966 7920 7468  lease specify th
-00012f30: 6520 7772 6974 696e 6720 7374 796c 6520  e writing style 
-00012f40: 6265 6c6f 773a 2229 0a20 2020 2020 2020  below:").       
-00012f50: 2020 2020 2073 7479 6c65 203d 2073 656c       style = sel
-00012f60: 662e 7072 6f6d 7074 732e 7369 6d70 6c65  f.prompts.simple
-00012f70: 5072 6f6d 7074 2873 7479 6c65 3d73 656c  Prompt(style=sel
-00012f80: 662e 7072 6f6d 7074 732e 7072 6f6d 7074  f.prompts.prompt
-00012f90: 5374 796c 6532 2c20 6465 6661 756c 743d  Style2, default=
-00012fa0: 636f 6e66 6967 2e69 6d70 726f 7665 6457  config.improvedW
-00012fb0: 7269 7469 6e67 5379 746c 6529 0a20 2020  ritingSytle).   
-00012fc0: 2020 2020 2020 2020 2069 6620 7374 796c           if styl
-00012fd0: 6520 616e 6420 6e6f 7420 7374 796c 6520  e and not style 
-00012fe0: 696e 2028 636f 6e66 6967 2e65 7869 745f  in (config.exit_
-00012ff0: 656e 7472 792c 2063 6f6e 6669 672e 6361  entry, config.ca
-00013000: 6e63 656c 5f65 6e74 7279 293a 0a20 2020  ncel_entry):.   
-00013010: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00013020: 6669 672e 696d 7072 6f76 6564 5772 6974  fig.improvedWrit
-00013030: 696e 6753 7974 6c65 203d 2073 7479 6c65  ingSytle = style
-00013040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013050: 2063 6f6e 6669 672e 7361 7665 436f 6e66   config.saveConf
-00013060: 6967 2829 0a20 2020 2020 2020 2070 7269  ig().        pri
-00013070: 6e74 3328 6622 496d 7072 6f76 6564 2057  nt3(f"Improved W
-00013080: 7269 7469 6e67 2044 6973 706c 6179 3a20  riting Display: 
-00013090: 277b 2765 6e61 626c 6564 2720 6966 2063  '{'enabled' if c
-000130a0: 6f6e 6669 672e 6469 7370 6c61 7949 6d70  onfig.displayImp
-000130b0: 726f 7665 6457 7269 7469 6e67 2065 6c73  rovedWriting els
-000130c0: 6520 2764 6973 6162 6c65 6427 7d27 2122  e 'disabled'}'!"
-000130d0: 290a 0a20 2020 2064 6566 2073 6574 4175  )..    def setAu
-000130e0: 6469 6f50 6c61 7962 6163 6b54 6f6f 6c28  dioPlaybackTool(
-000130f0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00013100: 6c61 7962 6163 6b20 3d20 7365 6c66 2e64  layback = self.d
-00013110: 6961 6c6f 6773 2e67 6574 5661 6c69 644f  ialogs.getValidO
-00013120: 7074 696f 6e73 280a 2020 2020 2020 2020  ptions(.        
-00013130: 2020 2020 6f70 7469 6f6e 733d 2822 7079      options=("py
-00013140: 6761 6d65 222c 2022 766c 6322 292c 0a20  game", "vlc"),. 
-00013150: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00013160: 6970 7469 6f6e 733d 2822 5079 4761 6d65  iptions=("PyGame
-00013170: 222c 2066 2256 4c43 2050 6c61 7965 7220  ", f"VLC Player 
-00013180: 2877 2f20 7370 6565 6420 636f 6e74 726f  (w/ speed contro
-00013190: 6c29 7b27 205b 696e 7374 616c 6c61 7469  l){' [installati
-000131a0: 6f6e 2072 6571 7569 7265 645d 2720 6966  on required]' if
-000131b0: 206e 6f74 2063 6f6e 6669 672e 6973 566c   not config.isVl
-000131c0: 6350 6c61 7965 7249 6e73 7461 6c6c 6564  cPlayerInstalled
-000131d0: 2065 6c73 6520 2727 7d22 292c 0a20 2020   else ''}"),.   
-000131e0: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
-000131f0: 5465 7874 2d74 6f2d 5370 6565 6368 2050  Text-to-Speech P
-00013200: 6c61 7962 6163 6b22 2c0a 2020 2020 2020  layback",.      
-00013210: 2020 2020 2020 7465 7874 3d22 5365 6c65        text="Sele
-00013220: 6374 2061 2074 6578 742d 746f 2d73 7065  ct a text-to-spe
-00013230: 6563 6820 706c 6163 6b62 6163 6b20 746f  ech plackback to
-00013240: 6f6c 3a22 2c0a 2020 2020 2020 2020 2020  ol:",.          
-00013250: 2020 6465 6661 756c 743d 2276 6c63 2220    default="vlc" 
-00013260: 6966 2063 6f6e 6669 672e 6973 566c 6350  if config.isVlcP
-00013270: 6c61 7965 7249 6e73 7461 6c6c 6564 2061  layerInstalled a
-00013280: 6e64 206e 6f74 2063 6f6e 6669 672e 7573  nd not config.us
-00013290: 6550 7967 616d 6520 656c 7365 2022 7079  ePygame else "py
-000132a0: 6761 6d65 222c 0a20 2020 2020 2020 2029  game",.        )
-000132b0: 0a20 2020 2020 2020 2069 6620 706c 6179  .        if play
-000132c0: 6261 636b 3a0a 2020 2020 2020 2020 2020  back:.          
-000132d0: 2020 6966 2070 6c61 7962 6163 6b20 3d3d    if playback ==
-000132e0: 2022 766c 6322 3a0a 2020 2020 2020 2020   "vlc":.        
-000132f0: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
-00013300: 6f6e 6669 672e 6973 566c 6350 6c61 7965  onfig.isVlcPlaye
-00013310: 7249 6e73 7461 6c6c 6564 3a0a 2020 2020  rInstalled:.    
-00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013330: 7072 696e 7431 2822 564c 4320 706c 6179  print1("VLC play
-00013340: 6572 206e 6f74 2066 6f75 6e64 2120 496e  er not found! In
-00013350: 7374 616c 6c20 6974 2066 6972 7374 2122  stall it first!"
-00013360: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013370: 2020 2020 2020 7072 696e 7433 2822 5465        print3("Te
-00013380: 7874 2d74 6f2d 5370 6565 6368 2050 6c61  xt-to-Speech Pla
-00013390: 7962 6163 6b20 6368 616e 6765 6420 746f  yback changed to
-000133a0: 3a20 5079 4761 6d65 2229 0a20 2020 2020  : PyGame").     
-000133b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000133c0: 6f6e 6669 672e 7573 6550 7967 616d 6520  onfig.usePygame 
-000133d0: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-000133e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000133f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013400: 2063 6f6e 6669 672e 7573 6550 7967 616d   config.usePygam
-00013410: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
-00013420: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00013430: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-00013440: 6967 2e75 7365 5079 6761 6d65 203d 2054  ig.usePygame = T
-00013450: 7275 650a 0a20 2020 2064 6566 2073 6574  rue..    def set
-00013460: 5465 7874 546f 5370 6565 6368 436f 6e66  TextToSpeechConf
-00013470: 6967 2873 656c 6629 3a0a 2020 2020 2020  ig(self):.      
-00013480: 2020 7474 7350 6c61 7466 6f72 6d20 3d20    ttsPlatform = 
-00013490: 7365 6c66 2e64 6961 6c6f 6773 2e67 6574  self.dialogs.get
-000134a0: 5661 6c69 644f 7074 696f 6e73 280a 2020  ValidOptions(.  
-000134b0: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-000134c0: 733d 2822 676f 6f67 6c65 222c 2022 676f  s=("google", "go
-000134d0: 6f67 6c65 636c 6f75 6422 2c20 2265 6c65  oglecloud", "ele
-000134e0: 7665 6e6c 6162 7322 2c20 2263 7573 746f  venlabs", "custo
-000134f0: 6d22 292c 0a20 2020 2020 2020 2020 2020  m"),.           
-00013500: 2064 6573 6372 6970 7469 6f6e 733d 2822   descriptions=("
-00013510: 476f 6f67 6c65 2054 6578 742d 746f 2d53  Google Text-to-S
-00013520: 7065 6563 6820 2847 656e 6572 6963 2922  peech (Generic)"
-00013530: 2c20 2247 6f6f 676c 6520 5465 7874 2d74  , "Google Text-t
-00013540: 6f2d 5370 6565 6368 2028 4150 4929 222c  o-Speech (API)",
-00013550: 2022 456c 6576 656e 4c61 6273 2028 4150   "ElevenLabs (AP
-00013560: 4929 222c 2022 4375 7374 6f6d 2054 6578  I)", "Custom Tex
-00013570: 742d 746f 2d53 7065 6563 6820 436f 6d6d  t-to-Speech Comm
-00013580: 616e 6420 5b61 6476 616e 6365 645d 2229  and [advanced]")
-00013590: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
-000135a0: 746c 653d 2254 6578 742d 746f 2d53 7065  tle="Text-to-Spe
-000135b0: 6563 6820 436f 6e66 6967 7572 6174 696f  ech Configuratio
-000135c0: 6e73 222c 0a20 2020 2020 2020 2020 2020  ns",.           
-000135d0: 2074 6578 743d 2253 656c 6563 7420 6120   text="Select a 
-000135e0: 7465 7874 2d74 6f2d 7370 6565 6368 2070  text-to-speech p
-000135f0: 6c61 7466 6f72 6d3a 222c 0a20 2020 2020  latform:",.     
-00013600: 2020 2020 2020 2064 6566 6175 6c74 3d63         default=c
-00013610: 6f6e 6669 672e 7474 7350 6c61 7466 6f72  onfig.ttsPlatfor
-00013620: 6d2c 0a20 2020 2020 2020 2029 0a20 2020  m,.        ).   
-00013630: 2020 2020 2069 6620 7474 7350 6c61 7466       if ttsPlatf
-00013640: 6f72 6d3a 0a20 2020 2020 2020 2020 2020  orm:.           
-00013650: 2069 6620 7474 7350 6c61 7466 6f72 6d20   if ttsPlatform 
-00013660: 3d3d 2022 676f 6f67 6c65 636c 6f75 6422  == "googlecloud"
-00013670: 2061 6e64 206e 6f74 2028 6f73 2e65 6e76   and not (os.env
-00013680: 6972 6f6e 5b22 474f 4f47 4c45 5f41 5050  iron["GOOGLE_APP
-00013690: 4c49 4341 5449 4f4e 5f43 5245 4445 4e54  LICATION_CREDENT
-000136a0: 4941 4c53 225d 2061 6e64 2022 5465 7874  IALS"] and "Text
-000136b0: 2d74 6f2d 5370 6565 6368 2220 696e 2063  -to-Speech" in c
-000136c0: 6f6e 6669 672e 656e 6162 6c65 6447 6f6f  onfig.enabledGoo
-000136d0: 676c 6541 5049 7329 3a0a 2020 2020 2020  gleAPIs):.      
-000136e0: 2020 2020 2020 2020 2020 7072 696e 7432            print2
-000136f0: 2822 476f 6f67 6c65 2043 6c6f 7564 2054  ("Google Cloud T
-00013700: 6578 742d 746f 2d53 7065 6563 6820 6665  ext-to-Speech fe
-00013710: 6174 7572 6520 6973 206e 6f74 2065 6e61  ature is not ena
-00013720: 626c 6564 2122 290a 2020 2020 2020 2020  bled!").        
-00013730: 2020 2020 2020 2020 7072 696e 7433 2822          print3("
-00013740: 5265 6164 3a20 6874 7470 733a 2f2f 6769  Read: https://gi
-00013750: 7468 7562 2e63 6f6d 2f65 6c69 7261 6e77  thub.com/eliranw
-00013760: 6f6e 672f 6c65 746d 6564 6f69 742f 7769  ong/letmedoit/wi
-00013770: 6b69 2f47 6f6f 676c 652d 4150 492d 5365  ki/Google-API-Se
-00013780: 7475 7022 290a 2020 2020 2020 2020 2020  tup").          
-00013790: 2020 2020 2020 7072 696e 7433 2822 5465        print3("Te
-000137a0: 7874 2d74 6f2d 5370 6565 6368 2070 6c61  xt-to-Speech pla
-000137b0: 7466 6f72 6d20 6368 616e 6765 6420 746f  tform changed to
-000137c0: 3a20 476f 6f67 6c65 2054 6578 742d 746f  : Google Text-to
-000137d0: 2d53 7065 6563 6820 2847 656e 6572 6963  -Speech (Generic
-000137e0: 2922 290a 2020 2020 2020 2020 2020 2020  )").            
-000137f0: 2020 2020 636f 6e66 6967 2e74 7473 506c      config.ttsPl
-00013800: 6174 666f 726d 203d 2022 676f 6f67 6c65  atform = "google
-00013810: 220a 2020 2020 2020 2020 2020 2020 656c  ".            el
-00013820: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00013830: 2020 2020 636f 6e66 6967 2e74 7473 506c      config.ttsPl
-00013840: 6174 666f 726d 203d 2074 7473 506c 6174  atform = ttsPlat
-00013850: 666f 726d 0a20 2020 2020 2020 2023 2066  form.        # f
-00013860: 7572 7468 6572 206f 7074 696f 6e73 0a20  urther options. 
-00013870: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
-00013880: 2e74 7473 506c 6174 666f 726d 203d 3d20  .ttsPlatform == 
-00013890: 2267 6f6f 676c 6522 3a0a 2020 2020 2020  "google":.      
-000138a0: 2020 2020 2020 7365 6c66 2e73 6574 4774        self.setGt
-000138b0: 7473 4c61 6e67 7561 6765 2829 0a20 2020  tsLanguage().   
-000138c0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000138d0: 7441 7564 696f 506c 6179 6261 636b 546f  tAudioPlaybackTo
-000138e0: 6f6c 2829 0a20 2020 2020 2020 2020 2020  ol().           
-000138f0: 2073 656c 662e 7365 7456 6c63 5370 6565   self.setVlcSpee
-00013900: 6428 290a 2020 2020 2020 2020 656c 6966  d().        elif
-00013910: 2063 6f6e 6669 672e 7474 7350 6c61 7466   config.ttsPlatf
-00013920: 6f72 6d20 3d3d 2022 676f 6f67 6c65 636c  orm == "googlecl
-00013930: 6f75 6422 3a0a 2020 2020 2020 2020 2020  oud":.          
-00013940: 2020 7365 6c66 2e73 6574 4763 7474 734c    self.setGcttsL
-00013950: 616e 6775 6167 6528 290a 2020 2020 2020  anguage().      
-00013960: 2020 2020 2020 7365 6c66 2e73 6574 4763        self.setGc
-00013970: 7474 7353 7065 6564 2829 0a20 2020 2020  ttsSpeed().     
-00013980: 2020 2020 2020 2073 656c 662e 7365 7441         self.setA
-00013990: 7564 696f 506c 6179 6261 636b 546f 6f6c  udioPlaybackTool
-000139a0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-000139b0: 656c 662e 7365 7456 6c63 5370 6565 6428  elf.setVlcSpeed(
-000139c0: 290a 2020 2020 2020 2020 656c 6966 2063  ).        elif c
-000139d0: 6f6e 6669 672e 7474 7350 6c61 7466 6f72  onfig.ttsPlatfor
-000139e0: 6d20 3d3d 2022 656c 6576 656e 6c61 6273  m == "elevenlabs
-000139f0: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
-00013a00: 6620 6e6f 7420 636f 6e66 6967 2e65 6c65  f not config.ele
-00013a10: 7665 6e6c 6162 7341 7069 3a0a 2020 2020  venlabsApi:.    
-00013a20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013a30: 2e63 6861 6e67 6545 6c65 7665 6e6c 6162  .changeElevenlab
-00013a40: 7341 7069 2829 0a20 2020 2020 2020 2020  sApi().         
-00013a50: 2020 2069 6620 6e6f 7420 636f 6e66 6967     if not config
-00013a60: 2e65 6c65 7665 6e6c 6162 7341 7069 3a0a  .elevenlabsApi:.
-00013a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a80: 7072 696e 7431 2822 456c 6576 656e 4c61  print1("ElevenLa
-00013a90: 6273 2041 5049 206b 6579 206e 6f74 2066  bs API key not f
-00013aa0: 6f75 6e64 2122 290a 2020 2020 2020 2020  ound!").        
-00013ab0: 2020 2020 2020 2020 7072 696e 7433 2822          print3("
-00013ac0: 5465 7874 2d74 6f2d 5370 6565 6368 2070  Text-to-Speech p
-00013ad0: 6c61 7466 6f72 6d20 6368 616e 6765 6420  latform changed 
-00013ae0: 746f 3a20 476f 6f67 6c65 2054 6578 742d  to: Google Text-
-00013af0: 746f 2d53 7065 6563 6820 2847 656e 6572  to-Speech (Gener
-00013b00: 6963 2922 290a 2020 2020 2020 2020 2020  ic)").          
-00013b10: 2020 2020 2020 636f 6e66 6967 2e74 7473        config.tts
-00013b20: 506c 6174 666f 726d 203d 2022 676f 6f67  Platform = "goog
-00013b30: 6c65 220a 2020 2020 2020 2020 2020 2020  le".            
-00013b40: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00013b50: 2020 2020 2020 7365 6c66 2e73 6574 456c        self.setEl
-00013b60: 6576 656e 6c61 6273 566f 6963 6528 290a  evenlabsVoice().
-00013b70: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
-00013b80: 6669 672e 7474 7350 6c61 7466 6f72 6d20  fig.ttsPlatform 
-00013b90: 3d3d 2022 6375 7374 6f6d 223a 0a20 2020  == "custom":.   
-00013ba0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00013bb0: 6669 6e65 5474 7343 6f6d 6d61 6e64 2829  fineTtsCommand()
-00013bc0: 0a20 2020 2020 2020 2023 2073 6176 6520  .        # save 
-00013bd0: 636f 6e66 6967 730a 2020 2020 2020 2020  configs.        
-00013be0: 636f 6e66 6967 2e73 6176 6543 6f6e 6669  config.saveConfi
-00013bf0: 6728 290a 0a20 2020 2064 6566 2073 6574  g()..    def set
-00013c00: 566f 6963 6554 7970 696e 6743 6f6e 6669  VoiceTypingConfi
-00013c10: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
-00013c20: 2076 6f69 6365 5479 7069 6e67 506c 6174   voiceTypingPlat
-00013c30: 666f 726d 203d 2073 656c 662e 6469 616c  form = self.dial
-00013c40: 6f67 732e 6765 7456 616c 6964 4f70 7469  ogs.getValidOpti
-00013c50: 6f6e 7328 0a20 2020 2020 2020 2020 2020  ons(.           
-00013c60: 206f 7074 696f 6e73 3d28 2267 6f6f 676c   options=("googl
-00013c70: 6522 2c20 2267 6f6f 676c 6563 6c6f 7564  e", "googlecloud
-00013c80: 222c 2022 7768 6973 7065 7222 292c 0a20  ", "whisper"),. 
-00013c90: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00013ca0: 6970 7469 6f6e 733d 2822 476f 6f67 6c65  iptions=("Google
-00013cb0: 2053 7065 6563 682d 746f 2d54 6578 7420   Speech-to-Text 
-00013cc0: 2847 656e 6572 6963 2920 5b6f 6e6c 696e  (Generic) [onlin
-00013cd0: 655d 222c 2022 476f 6f67 6c65 2053 7065  e]", "Google Spe
-00013ce0: 6563 682d 746f 2d54 6578 7420 2841 5049  ech-to-Text (API
-00013cf0: 2920 5b6f 6e6c 696e 655d 222c 2022 4f70  ) [online]", "Op
-00013d00: 656e 4149 2057 6869 7370 6572 205b 6f66  enAI Whisper [of
-00013d10: 666c 696e 653b 2073 6c6f 7765 7220 7769  fline; slower wi
-00013d20: 7468 206e 6f6e 2d45 6e67 6c69 7368 2076  th non-English v
-00013d30: 6f69 6365 735d 2229 2c0a 2020 2020 2020  oices]"),.      
-00013d40: 2020 2020 2020 7469 746c 653d 2256 6f69        title="Voi
-00013d50: 6365 2054 7970 696e 6720 436f 6e66 6967  ce Typing Config
-00013d60: 7572 6174 696f 6e73 222c 0a20 2020 2020  urations",.     
-00013d70: 2020 2020 2020 2074 6578 743d 2253 656c         text="Sel
-00013d80: 6563 7420 6120 766f 6963 6520 7479 7069  ect a voice typi
-00013d90: 6e67 2070 6c61 7466 6f72 6d3a 222c 0a20  ng platform:",. 
-00013da0: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-00013db0: 6c74 3d63 6f6e 6669 672e 766f 6963 6554  lt=config.voiceT
-00013dc0: 7970 696e 6750 6c61 7466 6f72 6d2c 0a20  ypingPlatform,. 
-00013dd0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00013de0: 2069 6620 766f 6963 6554 7970 696e 6750   if voiceTypingP
-00013df0: 6c61 7466 6f72 6d3a 0a20 2020 2020 2020  latform:.       
-00013e00: 2020 2020 2069 6620 766f 6963 6554 7970       if voiceTyp
-00013e10: 696e 6750 6c61 7466 6f72 6d20 3d3d 2022  ingPlatform == "
-00013e20: 676f 6f67 6c65 636c 6f75 6422 2061 6e64  googlecloud" and
-00013e30: 206e 6f74 2028 6f73 2e65 6e76 6972 6f6e   not (os.environ
-00013e40: 5b22 474f 4f47 4c45 5f41 5050 4c49 4341  ["GOOGLE_APPLICA
-00013e50: 5449 4f4e 5f43 5245 4445 4e54 4941 4c53  TION_CREDENTIALS
-00013e60: 225d 2061 6e64 2022 5370 6565 6368 2d74  "] and "Speech-t
-00013e70: 6f2d 5465 7874 2220 696e 2063 6f6e 6669  o-Text" in confi
-00013e80: 672e 656e 6162 6c65 6447 6f6f 676c 6541  g.enabledGoogleA
-00013e90: 5049 7329 3a0a 2020 2020 2020 2020 2020  PIs):.          
-00013ea0: 2020 2020 2020 7072 696e 7432 2822 476f        print2("Go
-00013eb0: 6f67 6c65 2043 6c6f 7564 2053 7065 6563  ogle Cloud Speec
-00013ec0: 682d 746f 2d54 6578 7420 6665 6174 7572  h-to-Text featur
-00013ed0: 6520 6973 206e 6f74 2065 6e61 626c 6564  e is not enabled
-00013ee0: 2122 290a 2020 2020 2020 2020 2020 2020  !").            
-00013ef0: 2020 2020 7072 696e 7433 2822 5265 6164      print3("Read
-00013f00: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00013f10: 2e63 6f6d 2f65 6c69 7261 6e77 6f6e 672f  .com/eliranwong/
-00013f20: 6c65 746d 6564 6f69 742f 7769 6b69 2f47  letmedoit/wiki/G
-00013f30: 6f6f 676c 652d 4150 492d 5365 7475 7022  oogle-API-Setup"
-00013f40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013f50: 2020 7072 696e 7433 2822 566f 6963 6520    print3("Voice 
-00013f60: 7479 7069 6e67 2070 6c61 7466 6f72 6d20  typing platform 
-00013f70: 6368 616e 6765 6420 746f 3a20 476f 6f67  changed to: Goog
-00013f80: 6c65 2053 7065 6563 682d 746f 2d54 6578  le Speech-to-Tex
-00013f90: 7420 2847 656e 6572 6963 2922 290a 2020  t (Generic)").  
-00013fa0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00013fb0: 6e66 6967 2e76 6f69 6365 5479 7069 6e67  nfig.voiceTyping
-00013fc0: 506c 6174 666f 726d 203d 2022 676f 6f67  Platform = "goog
-00013fd0: 6c65 220a 2020 2020 2020 2020 2020 2020  le".            
-00013fe0: 656c 6966 2076 6f69 6365 5479 7069 6e67  elif voiceTyping
-00013ff0: 506c 6174 666f 726d 203d 3d20 2277 6869  Platform == "whi
-00014000: 7370 6572 2220 616e 6420 6e6f 7420 6973  sper" and not is
-00014010: 436f 6d6d 616e 6449 6e73 7461 6c6c 6564  CommandInstalled
-00014020: 2822 6666 6d70 6567 2229 3a0a 2020 2020  ("ffmpeg"):.    
-00014030: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00014040: 7432 2822 496e 7374 616c 6c20 2766 666d  t2("Install 'ffm
-00014050: 7065 6727 2066 6972 7374 2074 6f20 7573  peg' first to us
-00014060: 6520 6f66 666c 696e 6520 6f70 656e 6169  e offline openai
-00014070: 2077 6869 7370 6572 206d 6f64 656c 2122   whisper model!"
-00014080: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014090: 2020 7072 696e 7433 2822 5265 6164 3a20    print3("Read: 
-000140a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000140b0: 6f6d 2f6f 7065 6e61 692f 7768 6973 7065  om/openai/whispe
-000140c0: 7223 7365 7475 7022 290a 2020 2020 2020  r#setup").      
-000140d0: 2020 2020 2020 2020 2020 7072 696e 7433            print3
-000140e0: 2822 566f 6963 6520 7479 7069 6e67 2070  ("Voice typing p
-000140f0: 6c61 7466 6f72 6d20 6368 616e 6765 6420  latform changed 
-00014100: 746f 3a20 476f 6f67 6c65 2053 7065 6563  to: Google Speec
-00014110: 682d 746f 2d54 6578 7420 2847 656e 6572  h-to-Text (Gener
-00014120: 6963 2922 290a 2020 2020 2020 2020 2020  ic)").          
-00014130: 2020 2020 2020 636f 6e66 6967 2e76 6f69        config.voi
-00014140: 6365 5479 7069 6e67 506c 6174 666f 726d  ceTypingPlatform
-00014150: 203d 2022 676f 6f67 6c65 220a 2020 2020   = "google".    
-00014160: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00014170: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00014180: 6e66 6967 2e76 6f69 6365 5479 7069 6e67  nfig.voiceTyping
-00014190: 506c 6174 666f 726d 203d 2076 6f69 6365  Platform = voice
-000141a0: 5479 7069 6e67 506c 6174 666f 726d 0a20  TypingPlatform. 
-000141b0: 2020 2020 2020 2023 206c 616e 6775 6167         # languag
-000141c0: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
-000141d0: 6574 5370 6565 6368 546f 5465 7874 4c61  etSpeechToTextLa
-000141e0: 6e67 7561 6765 2829 0a20 2020 2020 2020  nguage().       
-000141f0: 2023 2063 6f6e 6669 6775 7265 2063 6f6e   # configure con
-00014200: 6669 672e 766f 6963 6554 7970 696e 6741  fig.voiceTypingA
-00014210: 646a 7573 7441 6d62 6965 6e74 4e6f 6973  djustAmbientNois
-00014220: 650a 2020 2020 2020 2020 766f 6963 6554  e.        voiceT
-00014230: 7970 696e 6741 646a 7573 7441 6d62 6965  ypingAdjustAmbie
-00014240: 6e74 4e6f 6973 6520 3d20 7365 6c66 2e64  ntNoise = self.d
-00014250: 6961 6c6f 6773 2e67 6574 5661 6c69 644f  ialogs.getValidO
-00014260: 7074 696f 6e73 280a 2020 2020 2020 2020  ptions(.        
-00014270: 2020 2020 6f70 7469 6f6e 733d 2822 5965      options=("Ye
-00014280: 7322 2c20 224e 6f22 292c 0a20 2020 2020  s", "No"),.     
-00014290: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000142a0: 6f6e 733d 2822 5965 7320 5b73 6c6f 7765  ons=("Yes [slowe
-000142b0: 725d 222c 2022 4e6f 2229 2c0a 2020 2020  r]", "No"),.    
-000142c0: 2020 2020 2020 2020 7469 746c 653d 2241          title="A
-000142d0: 646a 7573 7420 416d 6269 656e 7420 4e6f  djust Ambient No
-000142e0: 6973 6522 2c0a 2020 2020 2020 2020 2020  ise",.          
-000142f0: 2020 7465 7874 3d22 446f 2079 6f75 2077    text="Do you w
-00014300: 616e 7420 746f 2061 646a 7573 7420 616d  ant to adjust am
-00014310: 6269 656e 7420 6e6f 6973 653f 222c 0a20  bient noise?",. 
-00014320: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-00014330: 6c74 3d22 5965 7322 2069 6620 636f 6e66  lt="Yes" if conf
-00014340: 6967 2e76 6f69 6365 5479 7069 6e67 4164  ig.voiceTypingAd
-00014350: 6a75 7374 416d 6269 656e 744e 6f69 7365  justAmbientNoise
-00014360: 2065 6c73 6520 224e 6f22 2c0a 2020 2020   else "No",.    
-00014370: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
-00014380: 2076 6f69 6365 5479 7069 6e67 4164 6a75   voiceTypingAdju
-00014390: 7374 416d 6269 656e 744e 6f69 7365 3a0a  stAmbientNoise:.
-000143a0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-000143b0: 6967 2e76 6f69 6365 5479 7069 6e67 4164  ig.voiceTypingAd
-000143c0: 6a75 7374 416d 6269 656e 744e 6f69 7365  justAmbientNoise
-000143d0: 203d 2054 7275 6520 6966 2076 6f69 6365   = True if voice
-000143e0: 5479 7069 6e67 4164 6a75 7374 416d 6269  TypingAdjustAmbi
-000143f0: 656e 744e 6f69 7365 203d 3d20 2259 6573  entNoise == "Yes
-00014400: 2220 656c 7365 2046 616c 7365 0a20 2020  " else False.   
-00014410: 2020 2020 2023 2061 7564 696f 206e 6f74       # audio not
-00014420: 6966 6963 6174 696f 6e0a 2020 2020 2020  ification.      
-00014430: 2020 766f 6963 6554 7970 696e 674e 6f74    voiceTypingNot
-00014440: 6966 6963 6174 696f 6e20 3d20 7365 6c66  ification = self
-00014450: 2e64 6961 6c6f 6773 2e67 6574 5661 6c69  .dialogs.getVali
-00014460: 644f 7074 696f 6e73 280a 2020 2020 2020  dOptions(.      
-00014470: 2020 2020 2020 6f70 7469 6f6e 733d 2822        options=("
-00014480: 5965 7322 2c20 224e 6f22 292c 0a20 2020  Yes", "No"),.   
-00014490: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
-000144a0: 4175 6469 6f20 4e6f 7469 6669 6361 7469  Audio Notificati
-000144b0: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
-000144c0: 2074 6578 743d 2244 6f20 796f 7520 7761   text="Do you wa
-000144d0: 6e74 2061 7564 696f 206e 6f74 6966 6963  nt audio notific
-000144e0: 6174 696f 6e20 7768 656e 2079 6f75 2075  ation when you u
-000144f0: 7365 206d 6963 726f 7068 6f6e 653f 222c  se microphone?",
-00014500: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-00014510: 6175 6c74 3d22 5965 7322 2069 6620 636f  ault="Yes" if co
-00014520: 6e66 6967 2e76 6f69 6365 5479 7069 6e67  nfig.voiceTyping
-00014530: 4e6f 7469 6669 6361 7469 6f6e 2065 6c73  Notification els
-00014540: 6520 224e 6f22 2c0a 2020 2020 2020 2020  e "No",.        
-00014550: 290a 2020 2020 2020 2020 6966 2076 6f69  ).        if voi
-00014560: 6365 5479 7069 6e67 4e6f 7469 6669 6361  ceTypingNotifica
-00014570: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-00014580: 2020 636f 6e66 6967 2e76 6f69 6365 5479    config.voiceTy
-00014590: 7069 6e67 4e6f 7469 6669 6361 7469 6f6e  pingNotification
-000145a0: 203d 2054 7275 6520 6966 2076 6f69 6365   = True if voice
-000145b0: 5479 7069 6e67 4e6f 7469 6669 6361 7469  TypingNotificati
-000145c0: 6f6e 203d 3d20 2259 6573 2220 656c 7365  on == "Yes" else
-000145d0: 2046 616c 7365 0a20 2020 2020 2020 2023   False.        #
-000145e0: 2061 7574 6f20 636f 6d70 6c65 7469 6f6e   auto completion
-000145f0: 3a20 766f 6963 6554 7970 696e 6741 7574  : voiceTypingAut
-00014600: 6f43 6f6d 706c 6574 650a 2020 2020 2020  oComplete.      
-00014610: 2020 766f 6963 6554 7970 696e 6741 7574    voiceTypingAut
-00014620: 6f43 6f6d 706c 6574 6520 3d20 7365 6c66  oComplete = self
-00014630: 2e64 6961 6c6f 6773 2e67 6574 5661 6c69  .dialogs.getVali
-00014640: 644f 7074 696f 6e73 280a 2020 2020 2020  dOptions(.      
-00014650: 2020 2020 2020 6f70 7469 6f6e 733d 2822        options=("
-00014660: 5965 7322 2c20 224e 6f22 292c 0a20 2020  Yes", "No"),.   
-00014670: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
-00014680: 4175 6469 6f20 456e 7472 7920 4175 746f  Audio Entry Auto
-00014690: 2043 6f6d 706c 6574 696f 6e22 2c0a 2020   Completion",.  
-000146a0: 2020 2020 2020 2020 2020 7465 7874 3d22            text="
-000146b0: 446f 2079 6f75 2077 616e 7420 746f 2061  Do you want to a
-000146c0: 7574 6f6d 6174 6963 616c 6c79 2063 6f6d  utomatically com
-000146d0: 706c 6574 6520 796f 7572 2065 6e74 7279  plete your entry
-000146e0: 2077 6865 6e20 6d69 6372 6f70 686f 6e65   when microphone
-000146f0: 2073 746f 7073 3f22 2c0a 2020 2020 2020   stops?",.      
-00014700: 2020 2020 2020 6465 6661 756c 743d 2259        default="Y
-00014710: 6573 2220 6966 2063 6f6e 6669 672e 766f  es" if config.vo
-00014720: 6963 6554 7970 696e 6741 7574 6f43 6f6d  iceTypingAutoCom
-00014730: 706c 6574 6520 656c 7365 2022 4e6f 222c  plete else "No",
-00014740: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00014750: 2020 2069 6620 766f 6963 6554 7970 696e     if voiceTypin
-00014760: 6741 7574 6f43 6f6d 706c 6574 653a 0a20  gAutoComplete:. 
-00014770: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00014780: 672e 766f 6963 6554 7970 696e 6741 7574  g.voiceTypingAut
-00014790: 6f43 6f6d 706c 6574 6520 3d20 5472 7565  oComplete = True
-000147a0: 2069 6620 766f 6963 6554 7970 696e 6741   if voiceTypingA
-000147b0: 7574 6f43 6f6d 706c 6574 6520 3d3d 2022  utoComplete == "
-000147c0: 5965 7322 2065 6c73 6520 4661 6c73 650a  Yes" else False.
-000147d0: 2020 2020 2020 2020 2320 6e6f 7469 6679          # notify
-000147e0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-000147f0: 2229 0a20 2020 2020 2020 2070 7269 6e74  ").        print
-00014800: 3328 6622 566f 6963 6520 5479 7069 6e67  3(f"Voice Typing
-00014810: 204d 6f64 656c 3a20 7b63 6f6e 6669 672e   Model: {config.
-00014820: 766f 6963 6554 7970 696e 6750 6c61 7466  voiceTypingPlatf
-00014830: 6f72 6d7d 2229 0a20 2020 2020 2020 2070  orm}").        p
-00014840: 7269 6e74 3328 6622 566f 6963 6520 5479  rint3(f"Voice Ty
-00014850: 7069 6e67 204c 616e 6775 6167 653a 207b  ping Language: {
-00014860: 636f 6e66 6967 2e76 6f69 6365 5479 7069  config.voiceTypi
-00014870: 6e67 4c61 6e67 7561 6765 7d22 290a 2020  ngLanguage}").  
-00014880: 2020 2020 2020 7072 696e 7433 2866 2241        print3(f"A
-00014890: 6d62 6965 6e74 204e 6f69 7365 2041 646a  mbient Noise Adj
-000148a0: 7573 746d 656e 743a 207b 636f 6e66 6967  ustment: {config
-000148b0: 2e76 6f69 6365 5479 7069 6e67 4164 6a75  .voiceTypingAdju
-000148c0: 7374 416d 6269 656e 744e 6f69 7365 7d22  stAmbientNoise}"
-000148d0: 290a 2020 2020 2020 2020 7072 696e 7433  ).        print3
-000148e0: 2866 2241 7564 696f 204e 6f74 6966 6963  (f"Audio Notific
-000148f0: 6174 696f 6e3a 207b 636f 6e66 6967 2e76  ation: {config.v
-00014900: 6f69 6365 5479 7069 6e67 4e6f 7469 6669  oiceTypingNotifi
-00014910: 6361 7469 6f6e 7d22 290a 2020 2020 2020  cation}").      
-00014920: 2020 7072 696e 7433 2866 2241 7574 6f20    print3(f"Auto 
-00014930: 436f 6d70 6c65 7469 6f6e 3a20 7b63 6f6e  Completion: {con
-00014940: 6669 672e 766f 6963 6554 7970 696e 6741  fig.voiceTypingA
-00014950: 7574 6f43 6f6d 706c 6574 657d 2229 0a20  utoComplete}"). 
-00014960: 2020 2020 2020 2023 2073 6176 6520 636f         # save co
-00014970: 6e66 6967 730a 2020 2020 2020 2020 636f  nfigs.        co
-00014980: 6e66 6967 2e73 6176 6543 6f6e 6669 6728  nfig.saveConfig(
-00014990: 290a 0a20 2020 2064 6566 2073 6176 6543  )..    def saveC
-000149a0: 6861 7428 7365 6c66 2c20 6d65 7373 6167  hat(self, messag
-000149b0: 6573 293a 0a20 2020 2020 2020 206d 6573  es):.        mes
-000149c0: 7361 6765 7343 6f70 7920 3d20 636f 7079  sagesCopy = copy
-000149d0: 2e64 6565 7063 6f70 7928 6d65 7373 6167  .deepcopy(messag
-000149e0: 6573 290a 0a20 2020 2020 2020 2069 6620  es)..        if 
-000149f0: 636f 6e66 6967 2e63 6f6e 7665 7273 6174  config.conversat
-00014a00: 696f 6e53 7461 7274 6564 3a0a 2020 2020  ionStarted:.    
-00014a10: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
-00014a20: 7020 3d20 6765 7443 7572 7265 6e74 4461  p = getCurrentDa
-00014a30: 7465 5469 6d65 2829 0a0a 2020 2020 2020  teTime()..      
-00014a40: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
-00014a50: 2863 6f6e 6669 672c 2022 7361 7665 5f63  (config, "save_c
-00014a60: 6861 745f 7265 636f 7264 2229 3a0a 2020  hat_record"):.  
-00014a70: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00014a80: 7768 656e 2070 6c75 6769 6e20 2273 6176  when plugin "sav
-00014a90: 6520 6368 6174 2072 6563 6f72 6473 2220  e chat records" 
-00014aa0: 6973 2065 6e61 626c 6564 0a20 2020 2020  is enabled.     
-00014ab0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00014ac0: 6765 4c65 6e67 7468 203d 206c 656e 286d  geLength = len(m
-00014ad0: 6573 7361 6765 7343 6f70 7929 0a20 2020  essagesCopy).   
-00014ae0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00014af0: 206f 7264 6572 2c20 6920 696e 2065 6e75   order, i in enu
-00014b00: 6d65 7261 7465 286d 6573 7361 6765 7343  merate(messagesC
-00014b10: 6f70 7929 3a0a 2020 2020 2020 2020 2020  opy):.          
-00014b20: 2020 2020 2020 2020 2020 6973 4c61 7374            isLast
-00014b30: 4974 656d 203d 2028 6f72 6465 7220 3d3d  Item = (order ==
-00014b40: 2028 6d65 7373 6167 654c 656e 6774 6820   (messageLength 
-00014b50: 2d20 3129 290a 2020 2020 2020 2020 2020  - 1)).          
-00014b60: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
-00014b70: 6669 672e 6c6c 6d49 6e74 6572 6661 6365  fig.llmInterface
-00014b80: 2069 6e20 2822 6368 6174 6770 7422 2c20   in ("chatgpt", 
-00014b90: 226c 6574 6d65 646f 6974 222c 2022 6772  "letmedoit", "gr
-00014ba0: 6f71 2229 2061 6e64 206e 6f74 2069 734c  oq") and not isL
-00014bb0: 6173 7449 7465 6d20 616e 6420 692e 6765  astItem and i.ge
-00014bc0: 7428 2272 6f6c 6522 2c20 2222 2920 3d3d  t("role", "") ==
-00014bd0: 2022 7573 6572 2220 616e 6420 2266 756e   "user" and "fun
-00014be0: 6374 696f 6e5f 6361 6c6c 2220 696e 206d  ction_call" in m
-00014bf0: 6573 7361 6765 7343 6f70 795b 6f72 6465  essagesCopy[orde
-00014c00: 722b 315d 3a0a 2020 2020 2020 2020 2020  r+1]:.          
-00014c10: 2020 2020 2020 2020 2020 2020 2020 695b                i[
-00014c20: 2274 6f6f 6c22 5d20 3d20 6d65 7373 6167  "tool"] = messag
-00014c30: 6573 436f 7079 5b6f 7264 6572 2b31 5d5b  esCopy[order+1][
-00014c40: 2266 756e 6374 696f 6e5f 6361 6c6c 225d  "function_call"]
-00014c50: 2e67 6574 2822 6e61 6d65 222c 2022 2229  .get("name", "")
-00014c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014c70: 2020 2020 2063 6f6e 6669 672e 7361 7665       config.save
-00014c80: 5f63 6861 745f 7265 636f 7264 2874 696d  _chat_record(tim
-00014c90: 6573 7461 6d70 2c20 6f72 6465 722c 2069  estamp, order, i
-00014ca0: 290a 0a20 2020 2020 2020 2020 2020 2074  )..            t
-00014cb0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00014cc0: 2020 2020 666f 6c64 6572 5061 7468 203d      folderPath =
-00014cd0: 206f 732e 7061 7468 2e6a 6f69 6e28 636f   os.path.join(co
-00014ce0: 6e66 6967 2e6c 6f63 616c 5374 6f72 6167  nfig.localStorag
-00014cf0: 652c 2022 6368 6174 7322 2c20 7265 2e73  e, "chats", re.s
-00014d00: 7562 2822 5e28 5b30 2d39 5d2b 3f5c 2d5b  ub("^([0-9]+?\-[
-00014d10: 302d 395d 2b3f 295c 2d2e 2a3f 2422 2c20  0-9]+?)\-.*?$", 
-00014d20: 7222 5c31 222c 2074 696d 6573 7461 6d70  r"\1", timestamp
-00014d30: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00014d40: 2020 2050 6174 6828 666f 6c64 6572 5061     Path(folderPa
-00014d50: 7468 292e 6d6b 6469 7228 7061 7265 6e74  th).mkdir(parent
-00014d60: 733d 5472 7565 2c20 6578 6973 745f 6f6b  s=True, exist_ok
-00014d70: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00014d80: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-00014d90: 682e 6973 6469 7228 666f 6c64 6572 5061  h.isdir(folderPa
-00014da0: 7468 293a 0a20 2020 2020 2020 2020 2020  th):.           
-00014db0: 2020 2020 2020 2020 2063 6861 7446 696c           chatFil
-00014dc0: 6520 3d20 6f73 2e70 6174 682e 6a6f 696e  e = os.path.join
-00014dd0: 2866 6f6c 6465 7250 6174 682c 2066 227b  (folderPath, f"{
-00014de0: 7469 6d65 7374 616d 707d 2e74 7874 2229  timestamp}.txt")
-00014df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014e00: 2020 2020 2077 6974 6820 6f70 656e 2863       with open(c
-00014e10: 6861 7446 696c 652c 2022 7722 2c20 656e  hatFile, "w", en
-00014e20: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-00014e30: 6173 2066 696c 654f 626a 3a0a 2020 2020  as fileObj:.    
-00014e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e50: 2020 2020 6669 6c65 4f62 6a2e 7772 6974      fileObj.writ
-00014e60: 6528 7070 7269 6e74 2e70 666f 726d 6174  e(pprint.pformat
-00014e70: 286d 6573 7361 6765 7343 6f70 7929 290a  (messagesCopy)).
-00014e80: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00014e90: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-00014ea0: 2020 2020 7072 696e 7432 2822 4661 696c      print2("Fail
-00014eb0: 6564 2074 6f20 7361 7665 2063 6861 7421  ed to save chat!
-00014ec0: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
-00014ed0: 2020 2020 2073 686f 7745 7272 6f72 7328       showErrors(
-00014ee0: 290a 0a20 2020 2064 6566 2065 7870 6f72  )..    def expor
-00014ef0: 7443 6861 7428 7365 6c66 2c20 6d65 7373  tChat(self, mess
-00014f00: 6167 6573 2c20 6f70 656e 4669 6c65 3d54  ages, openFile=T
-00014f10: 7275 6529 3a0a 2020 2020 2020 2020 6966  rue):.        if
-00014f20: 2063 6f6e 6669 672e 636f 6e76 6572 7361   config.conversa
-00014f30: 7469 6f6e 5374 6172 7465 643a 0a20 2020  tionStarted:.   
-00014f40: 2020 2020 2020 2020 2070 6c61 696e 5465           plainTe
-00014f50: 7874 203d 2022 220a 2020 2020 2020 2020  xt = "".        
-00014f60: 2020 2020 7469 6d65 7374 616d 7020 3d20      timestamp = 
-00014f70: 6765 7443 7572 7265 6e74 4461 7465 5469  getCurrentDateTi
-00014f80: 6d65 2829 0a0a 2020 2020 2020 2020 2020  me()..          
-00014f90: 2020 666f 7220 6920 696e 206d 6573 7361    for i in messa
-00014fa0: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
-00014fb0: 2020 2020 2069 6620 695b 2272 6f6c 6522       if i["role"
-00014fc0: 5d20 3d3d 2022 7573 6572 223a 0a20 2020  ] == "user":.   
-00014fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fe0: 2063 6f6e 7465 6e74 203d 2069 5b22 636f   content = i["co
-00014ff0: 6e74 656e 7422 5d0a 2020 2020 2020 2020  ntent"].        
-00015000: 2020 2020 2020 2020 2020 2020 706c 6169              plai
-00015010: 6e54 6578 7420 2b3d 2066 223e 3e3e 207b  nText += f">>> {
-00015020: 636f 6e74 656e 747d 220a 2020 2020 2020  content}".      
-00015030: 2020 2020 2020 2020 2020 6966 2069 5b22            if i["
-00015040: 726f 6c65 225d 203d 3d20 2266 756e 6374  role"] == "funct
-00015050: 696f 6e22 3a0a 2020 2020 2020 2020 2020  ion":.          
-00015060: 2020 2020 2020 2020 2020 6966 2070 6c61            if pla
-00015070: 696e 5465 7874 3a0a 2020 2020 2020 2020  inText:.        
-00015080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015090: 706c 6169 6e54 6578 7420 2b3d 2022 5c6e  plainText += "\n
-000150a0: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-000150b0: 2020 2020 2020 2020 6e61 6d65 203d 2069          name = i
-000150c0: 5b22 6e61 6d65 225d 0a20 2020 2020 2020  ["name"].       
-000150d0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-000150e0: 696e 5465 7874 202b 3d20 6622 6060 605c  inText += f"```\
-000150f0: 6e7b 6e61 6d65 7d5c 6e60 6060 220a 2020  n{name}\n```".  
-00015100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015110: 2020 636f 6e74 656e 7420 3d20 695b 2263    content = i["c
-00015120: 6f6e 7465 6e74 225d 0a20 2020 2020 2020  ontent"].       
-00015130: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-00015140: 696e 5465 7874 202b 3d20 6622 5c6e 5c6e  inText += f"\n\n
-00015150: 7b63 6f6e 7465 6e74 7d5c 6e5c 6e22 0a20  {content}\n\n". 
-00015160: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00015170: 6c69 6620 695b 2272 6f6c 6522 5d20 3d3d  lif i["role"] ==
-00015180: 2022 6173 7369 7374 616e 7422 3a0a 2020   "assistant":.  
-00015190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151a0: 2020 636f 6e74 656e 7420 3d20 695b 2263    content = i["c
-000151b0: 6f6e 7465 6e74 225d 0a20 2020 2020 2020  ontent"].       
-000151c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000151d0: 636f 6e74 656e 7420 6973 206e 6f74 204e  content is not N
-000151e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000151f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00015200: 706c 6169 6e54 6578 743a 0a20 2020 2020  plainText:.     
+0000eec0: 743d 636f 6e66 6967 2e67 726f 7141 7069  t=config.groqApi
+0000eed0: 5f63 6861 745f 6d6f 6465 6c20 6966 2066  _chat_model if f
+0000eee0: 6561 7475 7265 203d 3d20 2263 6861 7422  eature == "chat"
+0000eef0: 2065 6c73 6520 636f 6e66 6967 2e67 726f   else config.gro
+0000ef00: 7141 7069 5f6d 6169 6e5f 6d6f 6465 6c2c  qApi_main_model,
+0000ef10: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+0000ef20: 743d 2253 656c 6563 7420 6120 6675 6e63  t="Select a func
+0000ef30: 7469 6f6e 2063 616c 6c20 6d6f 6465 6c3a  tion call model:
+0000ef40: 5c6e 2866 6f72 2062 6f74 6820 6368 6174  \n(for both chat
+0000ef50: 2061 6e64 2074 6173 6b20 6578 6563 7574   and task execut
+0000ef60: 696f 6e29 222c 0a20 2020 2020 2020 2029  ion)",.        )
+0000ef70: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+0000ef80: 6c3a 0a20 2020 2020 2020 2020 2020 2069  l:.            i
+0000ef90: 6620 6665 6174 7572 6520 3d3d 2022 6465  f feature == "de
+0000efa0: 6661 756c 7422 3a0a 2020 2020 2020 2020  fault":.        
+0000efb0: 2020 2020 2020 2020 636f 6e66 6967 2e67          config.g
+0000efc0: 726f 7141 7069 5f6d 6169 6e5f 6d6f 6465  roqApi_main_mode
+0000efd0: 6c20 3d20 6d6f 6465 6c0a 2020 2020 2020  l = model.      
+0000efe0: 2020 2020 2020 656c 6966 2066 6561 7475        elif featu
+0000eff0: 7265 203d 3d20 2263 6861 7422 3a0a 2020  re == "chat":.  
+0000f000: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000f010: 6e66 6967 2e67 726f 7141 7069 5f63 6861  nfig.groqApi_cha
+0000f020: 745f 6d6f 6465 6c20 3d20 6d6f 6465 6c0a  t_model = model.
+0000f030: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000f040: 7433 2866 2247 726f 7120 6d6f 6465 6c3a  t3(f"Groq model:
+0000f050: 207b 6d6f 6465 6c7d 2229 0a0a 2020 2020   {model}")..    
+0000f060: 6465 6620 7365 744c 6c6d 4d6f 6465 6c5f  def setLlmModel_
+0000f070: 6368 6174 6770 7428 7365 6c66 293a 0a20  chatgpt(self):. 
+0000f080: 2020 2020 2020 206d 6f64 656c 203d 2073         model = s
+0000f090: 656c 662e 6469 616c 6f67 732e 6765 7456  elf.dialogs.getV
+0000f0a0: 616c 6964 4f70 7469 6f6e 7328 0a20 2020  alidOptions(.   
+0000f0b0: 2020 2020 2020 2020 206f 7074 696f 6e73           options
+0000f0c0: 3d73 656c 662e 6d6f 6465 6c73 2c0a 2020  =self.models,.  
+0000f0d0: 2020 2020 2020 2020 2020 7469 746c 653d            title=
+0000f0e0: 2243 6861 7447 5054 204d 6f64 656c 222c  "ChatGPT Model",
+0000f0f0: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+0000f100: 6175 6c74 3d63 6f6e 6669 672e 6368 6174  ault=config.chat
+0000f110: 4750 5441 7069 4d6f 6465 6c20 6966 2063  GPTApiModel if c
+0000f120: 6f6e 6669 672e 6368 6174 4750 5441 7069  onfig.chatGPTApi
+0000f130: 4d6f 6465 6c20 696e 2073 656c 662e 6d6f  Model in self.mo
+0000f140: 6465 6c73 2065 6c73 6520 7365 6c66 2e6d  dels else self.m
+0000f150: 6f64 656c 735b 305d 2c0a 2020 2020 2020  odels[0],.      
+0000f160: 2020 2020 2020 7465 7874 3d22 5365 6c65        text="Sele
+0000f170: 6374 2061 2066 756e 6374 696f 6e20 6361  ct a function ca
+0000f180: 6c6c 206d 6f64 656c 3a5c 6e28 666f 7220  ll model:\n(for 
+0000f190: 626f 7468 2063 6861 7420 616e 6420 7461  both chat and ta
+0000f1a0: 736b 2065 7865 6375 7469 6f6e 2922 2c0a  sk execution)",.
+0000f1b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000f1c0: 2020 6966 206d 6f64 656c 3a0a 2020 2020    if model:.    
+0000f1d0: 2020 2020 2020 2020 636f 6e66 6967 2e63          config.c
+0000f1e0: 6861 7447 5054 4170 694d 6f64 656c 203d  hatGPTApiModel =
+0000f1f0: 206d 6f64 656c 0a20 2020 2020 2020 2020   model.         
+0000f200: 2020 2070 7269 6e74 3328 6622 4368 6174     print3(f"Chat
+0000f210: 4750 5420 6d6f 6465 6c3a 207b 6d6f 6465  GPT model: {mode
+0000f220: 6c7d 2229 0a20 2020 2020 2020 2020 2020  l}").           
+0000f230: 2023 2073 6574 206d 6178 2074 6f6b 656e   # set max token
+0000f240: 730a 2020 2020 2020 2020 2020 2020 636f  s.            co
+0000f250: 6e66 6967 2e63 6861 7447 5054 4170 694d  nfig.chatGPTApiM
+0000f260: 6178 546f 6b65 6e73 203d 2073 656c 662e  axTokens = self.
+0000f270: 6765 744d 6178 546f 6b65 6e73 2829 5b2d  getMaxTokens()[-
+0000f280: 315d 0a20 2020 2020 2020 2020 2020 2070  1].            p
+0000f290: 7269 6e74 3328 6622 4d61 7869 6d75 6d20  rint3(f"Maximum 
+0000f2a0: 6f75 7470 7574 2074 6f6b 656e 733a 207b  output tokens: {
+0000f2b0: 636f 6e66 6967 2e63 6861 7447 5054 4170  config.chatGPTAp
+0000f2c0: 694d 6178 546f 6b65 6e73 7d22 290a 0a20  iMaxTokens}").. 
+0000f2d0: 2020 2064 6566 2073 6574 4368 6174 626f     def setChatbo
+0000f2e0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0000f2f0: 206d 6f64 656c 203d 2073 656c 662e 6469   model = self.di
+0000f300: 616c 6f67 732e 6765 7456 616c 6964 4f70  alogs.getValidOp
+0000f310: 7469 6f6e 7328 0a20 2020 2020 2020 2020  tions(.         
+0000f320: 2020 206f 7074 696f 6e73 3d28 2263 6861     options=("cha
+0000f330: 7467 7074 222c 2022 6765 6d69 6e69 7072  tgpt", "geminipr
+0000f340: 6f22 2c20 2270 616c 6d32 222c 2022 636f  o", "palm2", "co
+0000f350: 6465 7922 292c 0a20 2020 2020 2020 2020  dey"),.         
+0000f360: 2020 2074 6974 6c65 3d22 4368 6174 2d6f     title="Chat-o
+0000f370: 6e6c 7920 6d6f 6465 6c22 2c0a 2020 2020  nly model",.    
+0000f380: 2020 2020 2020 2020 6465 6661 756c 743d          default=
+0000f390: 636f 6e66 6967 2e63 6861 7462 6f74 2c0a  config.chatbot,.
+0000f3a0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+0000f3b0: 3d22 5365 6c65 6374 2064 6566 6175 6c74  ="Select default
+0000f3c0: 2063 6861 742d 6f6e 6c79 206d 6f64 656c   chat-only model
+0000f3d0: 3a5c 6e28 4465 6661 756c 7420 6d6f 6465  :\n(Default mode
+0000f3e0: 6c20 6973 206c 6f61 6465 6420 7768 656e  l is loaded when
+0000f3f0: 2079 6f75 2069 6e63 6c75 6465 2027 5b43   you include '[C
+0000f400: 4841 545d 2720 696e 2079 6f75 7220 696e  HAT]' in your in
+0000f410: 7075 7429 222c 0a20 2020 2020 2020 2029  put)",.        )
+0000f420: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+0000f430: 6c3a 0a20 2020 2020 2020 2020 2020 2063  l:.            c
+0000f440: 6f6e 6669 672e 6368 6174 626f 7420 3d20  onfig.chatbot = 
+0000f450: 6d6f 6465 6c0a 2020 2020 2020 2020 2020  model.          
+0000f460: 2020 7072 696e 7433 2866 2243 6861 742d    print3(f"Chat-
+0000f470: 6f6e 6c79 206d 6f64 656c 3a20 7b6d 6f64  only model: {mod
+0000f480: 656c 7d22 290a 0a20 2020 2064 6566 2073  el}")..    def s
+0000f490: 6574 456d 6265 6464 696e 674d 6f64 656c  etEmbeddingModel
+0000f4a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000f4b0: 6f6c 6445 6d62 6564 6469 6e67 4d6f 6465  oldEmbeddingMode
+0000f4c0: 6c20 3d20 636f 6e66 6967 2e65 6d62 6564  l = config.embed
+0000f4d0: 6469 6e67 4d6f 6465 6c0a 2020 2020 2020  dingModel.      
+0000f4e0: 2020 6d6f 6465 6c20 3d20 7365 6c66 2e64    model = self.d
+0000f4f0: 6961 6c6f 6773 2e67 6574 5661 6c69 644f  ialogs.getValidO
+0000f500: 7074 696f 6e73 280a 2020 2020 2020 2020  ptions(.        
+0000f510: 2020 2020 6f70 7469 6f6e 733d 2822 7465      options=("te
+0000f520: 7874 2d65 6d62 6564 6469 6e67 2d33 2d6c  xt-embedding-3-l
+0000f530: 6172 6765 222c 2022 7465 7874 2d65 6d62  arge", "text-emb
+0000f540: 6564 6469 6e67 2d33 2d73 6d61 6c6c 222c  edding-3-small",
+0000f550: 2022 7465 7874 2d65 6d62 6564 6469 6e67   "text-embedding
+0000f560: 2d61 6461 2d30 3032 222c 2022 7061 7261  -ada-002", "para
+0000f570: 7068 7261 7365 2d6d 756c 7469 6c69 6e67  phrase-multiling
+0000f580: 7561 6c2d 6d70 6e65 742d 6261 7365 2d76  ual-mpnet-base-v
+0000f590: 3222 2c20 2261 6c6c 2d6d 706e 6574 2d62  2", "all-mpnet-b
+0000f5a0: 6173 652d 7632 222c 2022 616c 6c2d 4d69  ase-v2", "all-Mi
+0000f5b0: 6e69 4c4d 2d4c 362d 7632 222c 2022 6375  niLM-L6-v2", "cu
+0000f5c0: 7374 6f6d 2229 2c0a 2020 2020 2020 2020  stom"),.        
+0000f5d0: 2020 2020 7469 746c 653d 2245 6d62 6564      title="Embed
+0000f5e0: 6469 6e67 206d 6f64 656c 222c 0a20 2020  ding model",.   
+0000f5f0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+0000f600: 3d63 6f6e 6669 672e 656d 6265 6464 696e  =config.embeddin
+0000f610: 674d 6f64 656c 2c0a 2020 2020 2020 2020  gModel,.        
+0000f620: 2020 2020 7465 7874 3d22 5365 6c65 6374      text="Select
+0000f630: 2061 6e20 656d 6265 6464 696e 6720 6d6f   an embedding mo
+0000f640: 6465 6c3a 222c 0a20 2020 2020 2020 2029  del:",.        )
+0000f650: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+0000f660: 6c3a 0a20 2020 2020 2020 2020 2020 2069  l:.            i
+0000f670: 6620 6d6f 6465 6c20 3d3d 2022 6375 7374  f model == "cust
+0000f680: 6f6d 223a 0a20 2020 2020 2020 2020 2020  om":.           
+0000f690: 2020 2020 2070 7269 6e74 3128 2245 6e74       print1("Ent
+0000f6a0: 6572 204f 7065 6e41 4920 6f72 2053 656e  er OpenAI or Sen
+0000f6b0: 7465 6e63 6520 5472 616e 7366 6f72 6d65  tence Transforme
+0000f6c0: 7220 456d 6265 6464 696e 6720 6d6f 6465  r Embedding mode
+0000f6d0: 6c3a 2229 0a20 2020 2020 2020 2020 2020  l:").           
+0000f6e0: 2020 2020 2070 7269 6e74 3128 2252 6561       print1("Rea
+0000f6f0: 6420 6d6f 7265 2061 743a 2068 7474 7073  d more at: https
+0000f700: 3a2f 2f77 7777 2e73 6265 7274 2e6e 6574  ://www.sbert.net
+0000f710: 2f64 6f63 732f 7072 6574 7261 696e 6564  /docs/pretrained
+0000f720: 5f6d 6f64 656c 732e 6874 6d6c 2229 0a20  _models.html"). 
+0000f730: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000f740: 7573 746f 6d4d 6f64 656c 203d 2073 656c  ustomModel = sel
+0000f750: 662e 7072 6f6d 7074 732e 7369 6d70 6c65  f.prompts.simple
+0000f760: 5072 6f6d 7074 2873 7479 6c65 3d73 656c  Prompt(style=sel
+0000f770: 662e 7072 6f6d 7074 732e 7072 6f6d 7074  f.prompts.prompt
+0000f780: 5374 796c 6532 2c20 6465 6661 756c 743d  Style2, default=
+0000f790: 636f 6e66 6967 2e65 6d62 6564 6469 6e67  config.embedding
+0000f7a0: 4d6f 6465 6c29 0a20 2020 2020 2020 2020  Model).         
+0000f7b0: 2020 2020 2020 2069 6620 6375 7374 6f6d         if custom
+0000f7c0: 4d6f 6465 6c20 616e 6420 6e6f 7420 6375  Model and not cu
+0000f7d0: 7374 6f6d 4d6f 6465 6c2e 7374 7269 7028  stomModel.strip(
+0000f7e0: 292e 6c6f 7765 7228 2920 3d3d 2063 6f6e  ).lower() == con
+0000f7f0: 6669 672e 6578 6974 5f65 6e74 7279 3a0a  fig.exit_entry:.
+0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f810: 2020 2020 636f 6e66 6967 2e65 6d62 6564      config.embed
+0000f820: 6469 6e67 4d6f 6465 6c20 3d20 6375 7374  dingModel = cust
+0000f830: 6f6d 4d6f 6465 6c20 0a20 2020 2020 2020  omModel .       
+0000f840: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000f850: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+0000f860: 672e 656d 6265 6464 696e 674d 6f64 656c  g.embeddingModel
+0000f870: 203d 206d 6f64 656c 0a20 2020 2020 2020   = model.       
+0000f880: 2020 2020 2070 7269 6e74 3328 6622 456d       print3(f"Em
+0000f890: 6265 6464 696e 6720 6d6f 6465 6c3a 207b  bedding model: {
+0000f8a0: 6d6f 6465 6c7d 2229 0a20 2020 2020 2020  model}").       
+0000f8b0: 2069 6620 6e6f 7420 6f6c 6445 6d62 6564   if not oldEmbed
+0000f8c0: 6469 6e67 4d6f 6465 6c20 3d3d 2063 6f6e  dingModel == con
+0000f8d0: 6669 672e 656d 6265 6464 696e 674d 6f64  fig.embeddingMod
+0000f8e0: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
+0000f8f0: 7072 696e 7431 2866 2259 6f75 2776 6520  print1(f"You've 
+0000f900: 6368 616e 6765 2074 6865 2065 6d62 6564  change the embed
+0000f910: 6469 6e67 206d 6f64 656c 2066 726f 6d20  ding model from 
+0000f920: 277b 6f6c 6445 6d62 6564 6469 6e67 4d6f  '{oldEmbeddingMo
+0000f930: 6465 6c7d 2720 746f 2027 7b63 6f6e 6669  del}' to '{confi
+0000f940: 672e 656d 6265 6464 696e 674d 6f64 656c  g.embeddingModel
+0000f950: 7d27 2e22 290a 2020 2020 2020 2020 2020  }'.").          
+0000f960: 2020 7072 696e 7431 2822 546f 2077 6f72    print1("To wor
+0000f970: 6b20 7769 7468 2074 6865 206e 6577 6c79  k with the newly
+0000f980: 2073 656c 6563 7465 6420 6d6f 6465 6c2c   selected model,
+0000f990: 2070 7265 7669 6f75 7320 6d65 6d6f 7279   previous memory
+0000f9a0: 2073 746f 7265 2061 6e64 2072 6574 7269   store and retri
+0000f9b0: 6576 6564 2063 6f6c 6c65 6374 696f 6e73  eved collections
+0000f9c0: 206e 6565 6420 746f 2062 6520 6465 6c65   need to be dele
+0000f9d0: 7465 642e 2229 0a20 2020 2020 2020 2020  ted.").         
+0000f9e0: 2020 2070 7269 6e74 3128 2244 6f20 796f     print1("Do yo
+0000f9f0: 7520 7761 6e74 2074 6f20 6465 6c65 7465  u want to delete
+0000fa00: 2074 6865 6d20 6e6f 773f 205b 795d 6573   them now? [y]es
+0000fa10: 202f 205b 4e5d 6f22 290a 2020 2020 2020   / [N]o").      
+0000fa20: 2020 2020 2020 636f 6e66 6972 6d61 7469        confirmati
+0000fa30: 6f6e 203d 2073 656c 662e 7072 6f6d 7074  on = self.prompt
+0000fa40: 732e 7369 6d70 6c65 5072 6f6d 7074 2873  s.simplePrompt(s
+0000fa50: 7479 6c65 3d73 656c 662e 7072 6f6d 7074  tyle=self.prompt
+0000fa60: 732e 7072 6f6d 7074 5374 796c 6532 2c20  s.promptStyle2, 
+0000fa70: 6465 6661 756c 743d 2279 6573 2229 0a20  default="yes"). 
+0000fa80: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+0000fa90: 6e66 6972 6d61 7469 6f6e 2e6c 6f77 6572  nfirmation.lower
+0000faa0: 2829 2069 6e20 2822 7922 2c20 2279 6573  () in ("y", "yes
+0000fab0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+0000fac0: 2020 2020 6d65 6d6f 7279 5f73 746f 7265      memory_store
+0000fad0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+0000fae0: 636f 6e66 6967 2e6c 6f63 616c 5374 6f72  config.localStor
+0000faf0: 6167 652c 2022 6d65 6d6f 7279 2229 0a20  age, "memory"). 
+0000fb00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000fb10: 6574 7269 6576 6564 5f63 6f6c 6c65 6374  etrieved_collect
+0000fb20: 696f 6e73 203d 206f 732e 7061 7468 2e6a  ions = os.path.j
+0000fb30: 6f69 6e28 636f 6e66 6967 2e6c 6f63 616c  oin(config.local
+0000fb40: 5374 6f72 6167 652c 2022 6175 746f 6765  Storage, "autoge
+0000fb50: 6e22 2c20 2272 6574 7269 6576 6572 2229  n", "retriever")
+0000fb60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fb70: 2066 6f72 2066 6f6c 6465 7220 696e 2028   for folder in (
+0000fb80: 6d65 6d6f 7279 5f73 746f 7265 2c20 7265  memory_store, re
+0000fb90: 7472 6965 7665 645f 636f 6c6c 6563 7469  trieved_collecti
+0000fba0: 6f6e 7329 3a0a 2020 2020 2020 2020 2020  ons):.          
+0000fbb0: 2020 2020 2020 2020 2020 7368 7574 696c            shutil
+0000fbc0: 2e72 6d74 7265 6528 666f 6c64 6572 2c20  .rmtree(folder, 
+0000fbd0: 6967 6e6f 7265 5f65 7272 6f72 733d 5472  ignore_errors=Tr
+0000fbe0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+0000fbf0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000fc00: 2020 2020 2020 7072 696e 7431 2866 2244        print1(f"D
+0000fc10: 6f20 796f 7520 7761 6e74 2074 6f20 6368  o you want to ch
+0000fc20: 616e 6765 2062 6163 6b20 7468 6520 656d  ange back the em
+0000fc30: 6265 6464 696e 6720 6d6f 6465 6c20 6672  bedding model fr
+0000fc40: 6f6d 2027 7b63 6f6e 6669 672e 656d 6265  om '{config.embe
+0000fc50: 6464 696e 674d 6f64 656c 7d27 2074 6f20  ddingModel}' to 
+0000fc60: 277b 6f6c 6445 6d62 6564 6469 6e67 4d6f  '{oldEmbeddingMo
+0000fc70: 6465 6c7d 273f 205b 795d 6573 202f 205b  del}'? [y]es / [
+0000fc80: 4e5d 6f22 290a 2020 2020 2020 2020 2020  N]o").          
+0000fc90: 2020 2020 2020 636f 6e66 6972 6d61 7469        confirmati
+0000fca0: 6f6e 203d 2073 656c 662e 7072 6f6d 7074  on = self.prompt
+0000fcb0: 732e 7369 6d70 6c65 5072 6f6d 7074 2873  s.simplePrompt(s
+0000fcc0: 7479 6c65 3d73 656c 662e 7072 6f6d 7074  tyle=self.prompt
+0000fcd0: 732e 7072 6f6d 7074 5374 796c 6532 2c20  s.promptStyle2, 
+0000fce0: 6465 6661 756c 743d 2279 6573 2229 0a20  default="yes"). 
+0000fcf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000fd00: 6620 6e6f 7420 636f 6e66 6972 6d61 7469  f not confirmati
+0000fd10: 6f6e 2e6c 6f77 6572 2829 2069 6e20 2822  on.lower() in ("
+0000fd20: 7922 2c20 2279 6573 2229 3a0a 2020 2020  y", "yes"):.    
+0000fd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd40: 636f 6e66 6967 2e65 6d62 6564 6469 6e67  config.embedding
+0000fd50: 4d6f 6465 6c20 3d20 6f6c 6445 6d62 6564  Model = oldEmbed
+0000fd60: 6469 6e67 4d6f 6465 6c0a 2020 2020 2020  dingModel.      
+0000fd70: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000fd80: 696e 7433 2866 2245 6d62 6564 6469 6e67  int3(f"Embedding
+0000fd90: 206d 6f64 656c 3a20 7b6f 6c64 456d 6265   model: {oldEmbe
+0000fda0: 6464 696e 674d 6f64 656c 7d22 290a 2020  ddingModel}").  
+0000fdb0: 2020 2020 2020 6966 206e 6f74 206f 6c64        if not old
+0000fdc0: 456d 6265 6464 696e 674d 6f64 656c 203d  EmbeddingModel =
+0000fdd0: 3d20 636f 6e66 6967 2e65 6d62 6564 6469  = config.embeddi
+0000fde0: 6e67 4d6f 6465 6c3a 0a20 2020 2020 2020  ngModel:.       
+0000fdf0: 2020 2020 2063 6f6e 6669 672e 7361 7665       config.save
+0000fe00: 436f 6e66 6967 2829 0a0a 2020 2020 6465  Config()..    de
+0000fe10: 6620 7365 7441 7574 6f47 656e 4275 696c  f setAutoGenBuil
+0000fe20: 6465 7243 6f6e 6669 6728 7365 6c66 293a  derConfig(self):
+0000fe30: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000fe40: 636f 6e66 6967 2e69 7354 6572 6d75 783a  config.isTermux:
+0000fe50: 0a20 2020 2020 2020 2020 2020 2041 7574  .            Aut
+0000fe60: 6f47 656e 4275 696c 6465 7228 292e 7072  oGenBuilder().pr
+0000fe70: 6f6d 7074 436f 6e66 6967 2829 0a0a 2020  omptConfig()..  
+0000fe80: 2020 6465 6620 7365 7441 7373 6973 7461    def setAssista
+0000fe90: 6e74 4e61 6d65 2873 656c 6629 3a0a 2020  ntName(self):.  
+0000fea0: 2020 2020 2020 7072 696e 7431 2822 596f        print1("Yo
+0000feb0: 7520 6d61 7920 6d6f 6469 6679 206d 7920  u may modify my 
+0000fec0: 6e61 6d65 2062 656c 6f77 3a22 290a 2020  name below:").  
+0000fed0: 2020 2020 2020 6672 6565 4765 6e69 7573        freeGenius
+0000fee0: 4149 4e61 6d65 203d 2073 656c 662e 7072  AIName = self.pr
+0000fef0: 6f6d 7074 732e 7369 6d70 6c65 5072 6f6d  ompts.simpleProm
+0000ff00: 7074 2873 7479 6c65 3d73 656c 662e 7072  pt(style=self.pr
+0000ff10: 6f6d 7074 732e 7072 6f6d 7074 5374 796c  ompts.promptStyl
+0000ff20: 6532 2c20 6465 6661 756c 743d 636f 6e66  e2, default=conf
+0000ff30: 6967 2e66 7265 6547 656e 6975 7341 494e  ig.freeGeniusAIN
+0000ff40: 616d 6529 0a20 2020 2020 2020 2069 6620  ame).        if 
+0000ff50: 6672 6565 4765 6e69 7573 4149 4e61 6d65  freeGeniusAIName
+0000ff60: 2061 6e64 206e 6f74 2066 7265 6547 656e   and not freeGen
+0000ff70: 6975 7341 494e 616d 652e 7374 7269 7028  iusAIName.strip(
+0000ff80: 292e 6c6f 7765 7228 2920 3d3d 2063 6f6e  ).lower() == con
+0000ff90: 6669 672e 6578 6974 5f65 6e74 7279 3a0a  fig.exit_entry:.
+0000ffa0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+0000ffb0: 6967 2e66 7265 6547 656e 6975 7341 494e  ig.freeGeniusAIN
+0000ffc0: 616d 6520 3d20 6672 6565 4765 6e69 7573  ame = freeGenius
+0000ffd0: 4149 4e61 6d65 0a20 2020 2020 2020 2020  AIName.         
+0000ffe0: 2020 2063 6f6e 6669 672e 6c6f 6361 6c53     config.localS
+0000fff0: 746f 7261 6765 203d 2067 6574 4c6f 6361  torage = getLoca
+00010000: 6c53 746f 7261 6765 2829 0a20 2020 2020  lStorage().     
+00010010: 2020 2020 2020 2063 6f6e 6669 672e 7361         config.sa
+00010020: 7665 436f 6e66 6967 2829 0a20 2020 2020  veConfig().     
+00010030: 2020 2020 2020 2070 7269 6e74 3328 6622         print3(f"
+00010040: 596f 7520 6861 7665 2063 6861 6e67 6564  You have changed
+00010050: 206d 7920 6e61 6d65 2074 6f3a 207b 636f   my name to: {co
+00010060: 6e66 6967 2e66 7265 6547 656e 6975 7341  nfig.freeGeniusA
+00010070: 494e 616d 657d 2229 0a0a 2020 2020 6465  IName}")..    de
+00010080: 6620 7365 7443 7573 746f 6d53 7973 7465  f setCustomSyste
+00010090: 6d4d 6573 7361 6765 2873 656c 6629 3a0a  mMessage(self):.
+000100a0: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+000100b0: 596f 7520 6361 6e20 6d6f 6469 6679 2074  You can modify t
+000100c0: 6865 2073 7973 7465 6d20 6d65 7373 6167  he system messag
+000100d0: 6520 746f 2066 7572 6e69 7368 206d 6520  e to furnish me 
+000100e0: 7769 7468 2064 6574 6169 6c73 2061 626f  with details abo
+000100f0: 7574 206d 7920 6361 7061 6269 6c69 7469  ut my capabiliti
+00010100: 6573 2c20 636f 6e73 7472 6169 6e74 732c  es, constraints,
+00010110: 206f 7220 616e 7920 7065 7274 696e 656e   or any pertinen
+00010120: 7420 636f 6e74 6578 7420 7468 6174 206d  t context that m
+00010130: 6179 2069 6e66 6f72 6d20 6f75 7220 696e  ay inform our in
+00010140: 7465 7261 6374 696f 6e73 2e20 5468 6973  teractions. This
+00010150: 2077 696c 6c20 6775 6964 6520 6d65 2069   will guide me i
+00010160: 6e20 6d61 6e61 6769 6e67 2061 6e64 2072  n managing and r
+00010170: 6573 706f 6e64 696e 6720 746f 2079 6f75  esponding to you
+00010180: 7220 7265 7175 6573 7473 2061 7070 726f  r requests appro
+00010190: 7072 6961 7465 6c79 2e22 290a 2020 2020  priately.").    
+000101a0: 2020 2020 7072 696e 7431 2822 506c 6561      print1("Plea
+000101b0: 7365 206e 6f74 6520 7468 6174 2061 6c74  se note that alt
+000101c0: 6572 696e 6720 6d79 2073 7973 7465 6d20  ering my system 
+000101d0: 6d65 7373 6167 6520 6469 7265 6374 6c79  message directly
+000101e0: 2061 6666 6563 7473 206d 7920 6675 6e63   affects my func
+000101f0: 7469 6f6e 616c 6974 792e 2048 616e 646c  tionality. Handl
+00010200: 6520 7769 7468 2063 6172 652e 2229 0a20  e with care."). 
+00010210: 2020 2020 2020 2070 7269 6e74 3128 2245         print1("E
+00010220: 6e74 6572 2063 7573 746f 6d20 7379 7374  nter custom syst
+00010230: 656d 206d 6573 7361 6765 2062 656c 6f77  em message below
+00010240: 3a22 290a 2020 2020 2020 2020 7072 696e  :").        prin
+00010250: 7431 2866 2228 4b65 6570 2069 7420 626c  t1(f"(Keep it bl
+00010260: 616e 6b20 746f 2075 7365 207b 636f 6e66  ank to use {conf
+00010270: 6967 2e66 7265 6547 656e 6975 7341 494e  ig.freeGeniusAIN
+00010280: 616d 657d 2064 6566 6175 6c74 2073 7973  ame} default sys
+00010290: 7465 6d20 6d65 7373 6167 652e 2922 290a  tem message.)").
+000102a0: 2020 2020 2020 2020 6d65 7373 6167 6520          message 
+000102b0: 3d20 7365 6c66 2e70 726f 6d70 7473 2e73  = self.prompts.s
+000102c0: 696d 706c 6550 726f 6d70 7428 7374 796c  implePrompt(styl
+000102d0: 653d 7365 6c66 2e70 726f 6d70 7473 2e70  e=self.prompts.p
+000102e0: 726f 6d70 7453 7479 6c65 322c 2064 6566  romptStyle2, def
+000102f0: 6175 6c74 3d63 6f6e 6669 672e 7379 7374  ault=config.syst
+00010300: 656d 4d65 7373 6167 655f 6c65 746d 6564  emMessage_letmed
+00010310: 6f69 7429 0a20 2020 2020 2020 2069 6620  oit).        if 
+00010320: 6d65 7373 6167 6520 616e 6420 6e6f 7420  message and not 
+00010330: 6d65 7373 6167 652e 7374 7269 7028 292e  message.strip().
+00010340: 6c6f 7765 7228 2920 3d3d 2063 6f6e 6669  lower() == confi
+00010350: 672e 6578 6974 5f65 6e74 7279 3a0a 2020  g.exit_entry:.  
+00010360: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00010370: 2e73 7973 7465 6d4d 6573 7361 6765 5f6c  .systemMessage_l
+00010380: 6574 6d65 646f 6974 203d 206d 6573 7361  etmedoit = messa
+00010390: 6765 0a20 2020 2020 2020 2020 2020 2063  ge.            c
+000103a0: 6f6e 6669 672e 7361 7665 436f 6e66 6967  onfig.saveConfig
+000103b0: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
+000103c0: 7269 6e74 3328 6622 4375 7374 6f6d 2073  rint3(f"Custom s
+000103d0: 7973 7465 6d20 6d65 7373 6167 653a 207b  ystem message: {
+000103e0: 636f 6e66 6967 2e66 7265 6547 656e 6975  config.freeGeniu
+000103f0: 7341 494e 616d 657d 2229 0a0a 2020 2020  sAIName}")..    
+00010400: 6465 6620 7365 7443 7573 746f 6d54 6578  def setCustomTex
+00010410: 7445 6469 746f 7228 7365 6c66 293a 0a20  tEditor(self):. 
+00010420: 2020 2020 2020 2070 7269 6e74 3128 2250         print1("P
+00010430: 6c65 6173 6520 7370 6563 6966 7920 6375  lease specify cu
+00010440: 7374 6f6d 2074 6578 7420 6564 6974 6f72  stom text editor
+00010450: 2063 6f6d 6d61 6e64 2062 656c 6f77 3a22   command below:"
+00010460: 290a 2020 2020 2020 2020 7072 696e 7431  ).        print1
+00010470: 2822 652e 672e 2027 6d69 6372 6f20 2d73  ("e.g. 'micro -s
+00010480: 6f66 7477 7261 7020 7472 7565 202d 776f  oftwrap true -wo
+00010490: 7264 7772 6170 2074 7275 6527 2229 0a20  rdwrap true'"). 
+000104a0: 2020 2020 2020 2070 7269 6e74 3128 224c         print1("L
+000104b0: 6561 7665 2069 7420 626c 616e 6b20 746f  eave it blank to
+000104c0: 2075 7365 206f 7572 2062 7569 6c74 2d69   use our built-i
+000104d0: 6e20 7465 7874 2065 6469 746f 7220 2765  n text editor 'e
+000104e0: 5465 7874 4564 6974 2720 6279 2064 6566  TextEdit' by def
+000104f0: 6175 6c74 2e22 290a 2020 2020 2020 2020  ault.").        
+00010500: 6375 7374 6f6d 5465 7874 4564 6974 6f72  customTextEditor
+00010510: 203d 2073 656c 662e 7072 6f6d 7074 732e   = self.prompts.
+00010520: 7369 6d70 6c65 5072 6f6d 7074 2873 7479  simplePrompt(sty
+00010530: 6c65 3d73 656c 662e 7072 6f6d 7074 732e  le=self.prompts.
+00010540: 7072 6f6d 7074 5374 796c 6532 2c20 6465  promptStyle2, de
+00010550: 6661 756c 743d 636f 6e66 6967 2e63 7573  fault=config.cus
+00010560: 746f 6d54 6578 7445 6469 746f 7229 0a20  tomTextEditor). 
+00010570: 2020 2020 2020 2069 6620 6375 7374 6f6d         if custom
+00010580: 5465 7874 4564 6974 6f72 2061 6e64 206e  TextEditor and n
+00010590: 6f74 2063 7573 746f 6d54 6578 7445 6469  ot customTextEdi
+000105a0: 746f 722e 7374 7269 7028 292e 6c6f 7765  tor.strip().lowe
+000105b0: 7228 2920 3d3d 2063 6f6e 6669 672e 6578  r() == config.ex
+000105c0: 6974 5f65 6e74 7279 3a0a 2020 2020 2020  it_entry:.      
+000105d0: 2020 2020 2020 7465 7874 4564 6974 6f72        textEditor
+000105e0: 203d 2072 652e 7375 6228 2220 2e2a 3f24   = re.sub(" .*?$
+000105f0: 222c 2022 222c 2063 7573 746f 6d54 6578  ", "", customTex
+00010600: 7445 6469 746f 7229 0a20 2020 2020 2020  tEditor).       
+00010610: 2020 2020 2069 6620 6e6f 7420 7465 7874       if not text
+00010620: 4564 6974 6f72 206f 7220 6e6f 7420 6973  Editor or not is
+00010630: 436f 6d6d 616e 6449 6e73 7461 6c6c 6564  CommandInstalled
+00010640: 2874 6578 7445 6469 746f 7229 3a0a 2020  (textEditor):.  
+00010650: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00010660: 696e 7432 2822 436f 6d6d 616e 6420 6e6f  int2("Command no
+00010670: 7420 666f 756e 6420 6f6e 2079 6f75 7220  t found on your 
+00010680: 6465 7669 6365 2122 290a 2020 2020 2020  device!").      
+00010690: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000106a0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+000106b0: 6967 2e63 7573 746f 6d54 6578 7445 6469  ig.customTextEdi
+000106c0: 746f 7220 3d20 6375 7374 6f6d 5465 7874  tor = customText
+000106d0: 4564 6974 6f72 0a20 2020 2020 2020 2020  Editor.         
+000106e0: 2020 2020 2020 2063 6f6e 6669 672e 7361         config.sa
+000106f0: 7665 436f 6e66 6967 2829 0a20 2020 2020  veConfig().     
+00010700: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00010710: 3328 6622 4375 7374 6f6d 2074 6578 7420  3(f"Custom text 
+00010720: 6564 6974 6f72 3a20 7b63 6f6e 6669 672e  editor: {config.
+00010730: 6375 7374 6f6d 5465 7874 4564 6974 6f72  customTextEditor
+00010740: 7d22 290a 0a20 2020 2064 6566 2073 6574  }")..    def set
+00010750: 4368 6174 5265 636f 7264 436c 6f73 6573  ChatRecordCloses
+00010760: 744d 6174 6368 6573 2873 656c 6629 3a0a  tMatches(self):.
+00010770: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+00010780: 506c 6561 7365 2073 7065 6369 6679 2074  Please specify t
+00010790: 6865 206e 756d 6265 7220 6f66 2063 6c6f  he number of clo
+000107a0: 7365 7374 206d 6174 6368 6573 2069 6e20  sest matches in 
+000107b0: 6561 6368 206d 656d 6f72 7920 7265 7472  each memory retr
+000107c0: 6965 7661 6c3a 2229 0a20 2020 2020 2020  ieval:").       
+000107d0: 2063 6861 7452 6563 6f72 6443 6c6f 7365   chatRecordClose
+000107e0: 7374 4d61 7463 6865 7320 3d20 7365 6c66  stMatches = self
+000107f0: 2e70 726f 6d70 7473 2e73 696d 706c 6550  .prompts.simpleP
+00010800: 726f 6d70 7428 7374 796c 653d 7365 6c66  rompt(style=self
+00010810: 2e70 726f 6d70 7473 2e70 726f 6d70 7453  .prompts.promptS
+00010820: 7479 6c65 322c 206e 756d 6265 724f 6e6c  tyle2, numberOnl
+00010830: 793d 5472 7565 2c20 6465 6661 756c 743d  y=True, default=
+00010840: 7374 7228 636f 6e66 6967 2e63 6861 7452  str(config.chatR
+00010850: 6563 6f72 6443 6c6f 7365 7374 4d61 7463  ecordClosestMatc
+00010860: 6865 7329 290a 2020 2020 2020 2020 6966  hes)).        if
+00010870: 2063 6861 7452 6563 6f72 6443 6c6f 7365   chatRecordClose
+00010880: 7374 4d61 7463 6865 7320 616e 6420 6e6f  stMatches and no
+00010890: 7420 6368 6174 5265 636f 7264 436c 6f73  t chatRecordClos
+000108a0: 6573 744d 6174 6368 6573 2e73 7472 6970  estMatches.strip
+000108b0: 2829 2e6c 6f77 6572 2829 203d 3d20 636f  ().lower() == co
+000108c0: 6e66 6967 2e65 7869 745f 656e 7472 7920  nfig.exit_entry 
+000108d0: 616e 6420 696e 7428 6368 6174 5265 636f  and int(chatReco
+000108e0: 7264 436c 6f73 6573 744d 6174 6368 6573  rdClosestMatches
+000108f0: 2920 3e3d 2030 3a0a 2020 2020 2020 2020  ) >= 0:.        
+00010900: 2020 2020 636f 6e66 6967 2e63 6861 7452      config.chatR
+00010910: 6563 6f72 6443 6c6f 7365 7374 4d61 7463  ecordClosestMatc
+00010920: 6865 7320 3d20 696e 7428 6368 6174 5265  hes = int(chatRe
+00010930: 636f 7264 436c 6f73 6573 744d 6174 6368  cordClosestMatch
+00010940: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+00010950: 636f 6e66 6967 2e73 6176 6543 6f6e 6669  config.saveConfi
+00010960: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+00010970: 7072 696e 7433 2866 224e 756d 6265 7220  print3(f"Number 
+00010980: 6f66 206d 656d 6f72 7920 636c 6f73 6573  of memory closes
+00010990: 7420 6d61 7463 6865 733a 207b 636f 6e66  t matches: {conf
+000109a0: 6967 2e63 6861 7452 6563 6f72 6443 6c6f  ig.chatRecordClo
+000109b0: 7365 7374 4d61 7463 6865 737d 2229 0a0a  sestMatches}")..
+000109c0: 2020 2020 6465 6620 7365 744d 656d 6f72      def setMemor
+000109d0: 7943 6c6f 7365 7374 4d61 7463 6865 7328  yClosestMatches(
+000109e0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+000109f0: 7269 6e74 3128 2250 6c65 6173 6520 7370  rint1("Please sp
+00010a00: 6563 6966 7920 7468 6520 6e75 6d62 6572  ecify the number
+00010a10: 206f 6620 636c 6f73 6573 7420 6d61 7463   of closest matc
+00010a20: 6865 7320 696e 2065 6163 6820 6d65 6d6f  hes in each memo
+00010a30: 7279 2072 6574 7269 6576 616c 3a22 290a  ry retrieval:").
+00010a40: 2020 2020 2020 2020 6d65 6d6f 7279 436c          memoryCl
+00010a50: 6f73 6573 744d 6174 6368 6573 203d 2073  osestMatches = s
+00010a60: 656c 662e 7072 6f6d 7074 732e 7369 6d70  elf.prompts.simp
+00010a70: 6c65 5072 6f6d 7074 2873 7479 6c65 3d73  lePrompt(style=s
+00010a80: 656c 662e 7072 6f6d 7074 732e 7072 6f6d  elf.prompts.prom
+00010a90: 7074 5374 796c 6532 2c20 6e75 6d62 6572  ptStyle2, number
+00010aa0: 4f6e 6c79 3d54 7275 652c 2064 6566 6175  Only=True, defau
+00010ab0: 6c74 3d73 7472 2863 6f6e 6669 672e 6d65  lt=str(config.me
+00010ac0: 6d6f 7279 436c 6f73 6573 744d 6174 6368  moryClosestMatch
+00010ad0: 6573 2929 0a20 2020 2020 2020 2069 6620  es)).        if 
+00010ae0: 6d65 6d6f 7279 436c 6f73 6573 744d 6174  memoryClosestMat
+00010af0: 6368 6573 2061 6e64 206e 6f74 206d 656d  ches and not mem
+00010b00: 6f72 7943 6c6f 7365 7374 4d61 7463 6865  oryClosestMatche
+00010b10: 732e 7374 7269 7028 292e 6c6f 7765 7228  s.strip().lower(
+00010b20: 2920 3d3d 2063 6f6e 6669 672e 6578 6974  ) == config.exit
+00010b30: 5f65 6e74 7279 2061 6e64 2069 6e74 286d  _entry and int(m
+00010b40: 656d 6f72 7943 6c6f 7365 7374 4d61 7463  emoryClosestMatc
+00010b50: 6865 7329 203e 3d20 303a 0a20 2020 2020  hes) >= 0:.     
+00010b60: 2020 2020 2020 2063 6f6e 6669 672e 6d65         config.me
+00010b70: 6d6f 7279 436c 6f73 6573 744d 6174 6368  moryClosestMatch
+00010b80: 6573 203d 2069 6e74 286d 656d 6f72 7943  es = int(memoryC
+00010b90: 6c6f 7365 7374 4d61 7463 6865 7329 0a20  losestMatches). 
+00010ba0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00010bb0: 672e 7361 7665 436f 6e66 6967 2829 0a20  g.saveConfig(). 
+00010bc0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00010bd0: 3328 6622 4e75 6d62 6572 206f 6620 6d65  3(f"Number of me
+00010be0: 6d6f 7279 2063 6c6f 7365 7374 206d 6174  mory closest mat
+00010bf0: 6368 6573 3a20 7b63 6f6e 6669 672e 6d65  ches: {config.me
+00010c00: 6d6f 7279 436c 6f73 6573 744d 6174 6368  moryClosestMatch
+00010c10: 6573 7d22 290a 0a20 2020 2064 6566 2073  es}")..    def s
+00010c20: 6574 4d61 7841 7574 6f43 6f72 7265 6374  etMaxAutoCorrect
+00010c30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00010c40: 7072 696e 7431 2866 2254 6865 2061 7574  print1(f"The aut
+00010c50: 6f2d 636f 7272 6563 7469 6f6e 2066 6561  o-correction fea
+00010c60: 7475 7265 2065 6e61 626c 6573 207b 636f  ture enables {co
+00010c70: 6e66 6967 2e66 7265 6547 656e 6975 7341  nfig.freeGeniusA
+00010c80: 494e 616d 657d 2074 6f20 6175 746f 6d61  IName} to automa
+00010c90: 7469 6361 6c6c 7920 6669 7820 6272 6f6b  tically fix brok
+00010ca0: 656e 2050 7974 686f 6e20 636f 6465 2069  en Python code i
+00010cb0: 6620 6974 2077 6173 206e 6f74 2065 7865  f it was not exe
+00010cc0: 6375 7465 6420 7072 6f70 6572 6c79 2e22  cuted properly."
+00010cd0: 290a 2020 2020 2020 2020 7072 696e 7431  ).        print1
+00010ce0: 2822 506c 6561 7365 2073 7065 6369 6679  ("Please specify
+00010cf0: 206d 6178 696d 756d 206e 756d 6265 7220   maximum number 
+00010d00: 6f66 2061 7574 6f2d 636f 7272 6563 7469  of auto-correcti
+00010d10: 6f6e 2061 7474 656d 7074 7320 6265 6c6f  on attempts belo
+00010d20: 773a 2229 0a20 2020 2020 2020 2070 7269  w:").        pri
+00010d30: 6e74 3128 2228 5265 6d61 726b 733a 2045  nt1("(Remarks: E
+00010d40: 6e74 6572 2027 3027 2069 6620 796f 7520  nter '0' if you 
+00010d50: 7761 6e74 2074 6f20 6469 7361 626c 6520  want to disable 
+00010d60: 6175 746f 2d63 6f72 7265 6374 696f 6e20  auto-correction 
+00010d70: 6665 6174 7572 6529 2229 0a20 2020 2020  feature)").     
+00010d80: 2020 206d 6178 4175 746f 436f 7272 6563     maxAutoCorrec
+00010d90: 7420 3d20 7365 6c66 2e70 726f 6d70 7473  t = self.prompts
+00010da0: 2e73 696d 706c 6550 726f 6d70 7428 7374  .simplePrompt(st
+00010db0: 796c 653d 7365 6c66 2e70 726f 6d70 7473  yle=self.prompts
+00010dc0: 2e70 726f 6d70 7453 7479 6c65 322c 206e  .promptStyle2, n
+00010dd0: 756d 6265 724f 6e6c 793d 5472 7565 2c20  umberOnly=True, 
+00010de0: 6465 6661 756c 743d 7374 7228 636f 6e66  default=str(conf
+00010df0: 6967 2e6d 6178 5f63 6f6e 7365 6375 7469  ig.max_consecuti
+00010e00: 7665 5f61 7574 6f5f 636f 7272 6563 7469  ve_auto_correcti
+00010e10: 6f6e 2929 0a20 2020 2020 2020 2069 6620  on)).        if 
+00010e20: 6d61 7841 7574 6f43 6f72 7265 6374 2061  maxAutoCorrect a
+00010e30: 6e64 206e 6f74 206d 6178 4175 746f 436f  nd not maxAutoCo
+00010e40: 7272 6563 742e 7374 7269 7028 292e 6c6f  rrect.strip().lo
+00010e50: 7765 7228 2920 3d3d 2063 6f6e 6669 672e  wer() == config.
+00010e60: 6578 6974 5f65 6e74 7279 2061 6e64 2069  exit_entry and i
+00010e70: 6e74 286d 6178 4175 746f 436f 7272 6563  nt(maxAutoCorrec
+00010e80: 7429 203e 3d20 303a 0a20 2020 2020 2020  t) >= 0:.       
+00010e90: 2020 2020 2063 6f6e 6669 672e 6d61 785f       config.max_
+00010ea0: 636f 6e73 6563 7574 6976 655f 6175 746f  consecutive_auto
+00010eb0: 5f63 6f72 7265 6374 696f 6e20 3d20 696e  _correction = in
+00010ec0: 7428 6d61 7841 7574 6f43 6f72 7265 6374  t(maxAutoCorrect
+00010ed0: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+00010ee0: 6e66 6967 2e73 6176 6543 6f6e 6669 6728  nfig.saveConfig(
+00010ef0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00010f00: 696e 7433 2866 224d 6178 696d 756d 2063  int3(f"Maximum c
+00010f10: 6f6e 7365 6375 7469 7665 2061 7574 6f2d  onsecutive auto-
+00010f20: 636f 7272 6563 7469 6f6e 3a20 7b63 6f6e  correction: {con
+00010f30: 6669 672e 6d61 785f 636f 6e73 6563 7574  fig.max_consecut
+00010f40: 6976 655f 6175 746f 5f63 6f72 7265 6374  ive_auto_correct
+00010f50: 696f 6e7d 2229 0a0a 2020 2020 6465 6620  ion}")..    def 
+00010f60: 7365 744d 696e 546f 6b65 6e73 2873 656c  setMinTokens(sel
+00010f70: 6629 3a0a 2020 2020 2020 2020 7072 696e  f):.        prin
+00010f80: 7431 2822 506c 6561 7365 2073 7065 6369  t1("Please speci
+00010f90: 6679 206d 696e 696d 756d 206f 7574 7075  fy minimum outpu
+00010fa0: 7420 746f 6b65 6e73 2062 656c 6f77 3a22  t tokens below:"
+00010fb0: 290a 2020 2020 2020 2020 7072 696e 7431  ).        print1
+00010fc0: 2822 2861 7070 6c69 6361 626c 6520 746f  ("(applicable to
+00010fd0: 2027 6368 6174 6770 7427 2061 6e64 2027   'chatgpt' and '
+00010fe0: 6c65 746d 6564 6f69 7427 2069 6e74 6572  letmedoit' inter
+00010ff0: 6661 6365 7320 6f6e 6c79 2922 290a 2020  faces only)").  
+00011000: 2020 2020 2020 6d69 6e74 6f6b 656e 7320        mintokens 
+00011010: 3d20 7365 6c66 2e70 726f 6d70 7473 2e73  = self.prompts.s
+00011020: 696d 706c 6550 726f 6d70 7428 7374 796c  implePrompt(styl
+00011030: 653d 7365 6c66 2e70 726f 6d70 7473 2e70  e=self.prompts.p
+00011040: 726f 6d70 7453 7479 6c65 322c 206e 756d  romptStyle2, num
+00011050: 6265 724f 6e6c 793d 5472 7565 2c20 6465  berOnly=True, de
+00011060: 6661 756c 743d 7374 7228 636f 6e66 6967  fault=str(config
+00011070: 2e63 6861 7447 5054 4170 694d 696e 546f  .chatGPTApiMinTo
+00011080: 6b65 6e73 2929 0a20 2020 2020 2020 2069  kens)).        i
+00011090: 6620 6d69 6e74 6f6b 656e 7320 616e 6420  f mintokens and 
+000110a0: 6e6f 7420 6d69 6e74 6f6b 656e 732e 7374  not mintokens.st
+000110b0: 7269 7028 292e 6c6f 7765 7228 2920 3d3d  rip().lower() ==
+000110c0: 2063 6f6e 6669 672e 6578 6974 5f65 6e74   config.exit_ent
+000110d0: 7279 2061 6e64 2069 6e74 286d 696e 746f  ry and int(minto
+000110e0: 6b65 6e73 2920 3e20 303a 0a20 2020 2020  kens) > 0:.     
+000110f0: 2020 2020 2020 2063 6f6e 6669 672e 6368         config.ch
+00011100: 6174 4750 5441 7069 4d69 6e54 6f6b 656e  atGPTApiMinToken
+00011110: 7320 3d20 696e 7428 6d69 6e74 6f6b 656e  s = int(mintoken
+00011120: 7329 0a20 2020 2020 2020 2020 2020 2069  s).            i
+00011130: 6620 636f 6e66 6967 2e63 6861 7447 5054  f config.chatGPT
+00011140: 4170 694d 696e 546f 6b65 6e73 203e 2063  ApiMinTokens > c
+00011150: 6f6e 6669 672e 6368 6174 4750 5441 7069  onfig.chatGPTApi
+00011160: 4d61 7854 6f6b 656e 733a 0a20 2020 2020  MaxTokens:.     
+00011170: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00011180: 672e 6368 6174 4750 5441 7069 4d69 6e54  g.chatGPTApiMinT
+00011190: 6f6b 656e 7320 3d20 636f 6e66 6967 2e63  okens = config.c
+000111a0: 6861 7447 5054 4170 694d 6178 546f 6b65  hatGPTApiMaxToke
+000111b0: 6e73 0a20 2020 2020 2020 2020 2020 2063  ns.            c
+000111c0: 6f6e 6669 672e 7361 7665 436f 6e66 6967  onfig.saveConfig
+000111d0: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
+000111e0: 7269 6e74 3328 6622 4d69 6e69 6d75 6d20  rint3(f"Minimum 
+000111f0: 6f75 7470 7574 2074 6f6b 656e 733a 207b  output tokens: {
+00011200: 636f 6e66 6967 2e63 6861 7447 5054 4170  config.chatGPTAp
+00011210: 694d 696e 546f 6b65 6e73 7d22 290a 0a20  iMinTokens}").. 
+00011220: 2020 2064 6566 2067 6574 4d61 7854 6f6b     def getMaxTok
+00011230: 656e 7328 7365 6c66 293a 0a20 2020 2020  ens(self):.     
+00011240: 2020 2063 6f6e 7465 7874 5769 6e64 6f77     contextWindow
+00011250: 4c69 6d69 7420 3d20 746f 6b65 6e4c 696d  Limit = tokenLim
+00011260: 6974 735b 636f 6e66 6967 2e63 6861 7447  its[config.chatG
+00011270: 5054 4170 694d 6f64 656c 5d0a 2020 2020  PTApiModel].    
+00011280: 2020 2020 6675 6e63 7469 6f6e 546f 6b65      functionToke
+00011290: 6e73 203d 2063 6f75 6e74 5f74 6f6b 656e  ns = count_token
+000112a0: 735f 6672 6f6d 5f66 756e 6374 696f 6e73  s_from_functions
+000112b0: 2863 6f6e 6669 672e 746f 6f6c 4675 6e63  (config.toolFunc
+000112c0: 7469 6f6e 5363 6865 6d61 732e 7661 6c75  tionSchemas.valu
+000112d0: 6573 2829 290a 2020 2020 2020 2020 6d61  es()).        ma
+000112e0: 7854 6f6b 656e 203d 2063 6f6e 7465 7874  xToken = context
+000112f0: 5769 6e64 6f77 4c69 6d69 7420 2d20 6675  WindowLimit - fu
+00011300: 6e63 7469 6f6e 546f 6b65 6e73 202d 2063  nctionTokens - c
+00011310: 6f6e 6669 672e 6368 6174 4750 5441 7069  onfig.chatGPTApi
+00011320: 4d69 6e54 6f6b 656e 730a 2020 2020 2020  MinTokens.      
+00011330: 2020 6966 206d 6178 546f 6b65 6e20 3e20    if maxToken > 
+00011340: 3430 3936 2061 6e64 2063 6f6e 6669 672e  4096 and config.
+00011350: 6368 6174 4750 5441 7069 4d6f 6465 6c20  chatGPTApiModel 
+00011360: 696e 2028 0a20 2020 2020 2020 2020 2020  in (.           
+00011370: 2022 6770 742d 342d 7475 7262 6f22 2c0a   "gpt-4-turbo",.
+00011380: 2020 2020 2020 2020 2020 2020 2267 7074              "gpt
+00011390: 2d34 2d74 7572 626f 2d70 7265 7669 6577  -4-turbo-preview
+000113a0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000113b0: 6770 742d 342d 3031 3235 2d70 7265 7669  gpt-4-0125-previ
+000113c0: 6577 222c 0a20 2020 2020 2020 2020 2020  ew",.           
+000113d0: 2022 6770 742d 342d 3131 3036 2d70 7265   "gpt-4-1106-pre
+000113e0: 7669 6577 222c 0a20 2020 2020 2020 2020  view",.         
+000113f0: 2020 2022 6770 742d 332e 352d 7475 7262     "gpt-3.5-turb
+00011400: 6f22 2c0a 2020 2020 2020 2020 293a 0a20  o",.        ):. 
+00011410: 2020 2020 2020 2020 2020 206d 6178 546f             maxTo
+00011420: 6b65 6e20 3d20 3430 3936 0a20 2020 2020  ken = 4096.     
+00011430: 2020 2072 6574 7572 6e20 636f 6e74 6578     return contex
+00011440: 7457 696e 646f 774c 696d 6974 2c20 6675  tWindowLimit, fu
+00011450: 6e63 7469 6f6e 546f 6b65 6e73 2c20 6d61  nctionTokens, ma
+00011460: 7854 6f6b 656e 0a0a 2020 2020 6465 6620  xToken..    def 
+00011470: 7365 744d 6178 546f 6b65 6e73 5f6e 6f6e  setMaxTokens_non
+00011480: 5f63 6861 7467 7074 2873 656c 6629 3a0a  _chatgpt(self):.
+00011490: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+000114a0: 506c 6561 7365 2073 7065 6369 6679 206d  Please specify m
+000114b0: 6178 696d 756d 206f 7574 7075 7420 746f  aximum output to
+000114c0: 6b65 6e73 2062 656c 6f77 3a22 290a 2020  kens below:").  
+000114d0: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
+000114e0: 6c6c 6d49 6e74 6572 6661 6365 203d 3d20  llmInterface == 
+000114f0: 2267 656d 696e 6922 3a0a 2020 2020 2020  "gemini":.      
+00011500: 2020 2020 2020 6465 6661 756c 7420 3d20        default = 
+00011510: 636f 6e66 6967 2e67 656d 696e 6970 726f  config.geminipro
+00011520: 5f6d 6178 5f6f 7574 7075 745f 746f 6b65  _max_output_toke
+00011530: 6e73 0a20 2020 2020 2020 2065 6c69 6620  ns.        elif 
+00011540: 636f 6e66 6967 2e6c 6c6d 496e 7465 7266  config.llmInterf
+00011550: 6163 6520 3d3d 2022 6c6c 616d 6163 7070  ace == "llamacpp
+00011560: 223a 0a20 2020 2020 2020 2020 2020 2064  ":.            d
+00011570: 6566 6175 6c74 203d 2063 6f6e 6669 672e  efault = config.
+00011580: 6c6c 616d 6163 7070 4d61 696e 4d6f 6465  llamacppMainMode
+00011590: 6c5f 6d61 785f 746f 6b65 6e73 0a20 2020  l_max_tokens.   
+000115a0: 2020 2020 2065 6c69 6620 636f 6e66 6967       elif config
+000115b0: 2e6c 6c6d 496e 7465 7266 6163 6520 3d3d  .llmInterface ==
+000115c0: 2022 6f6c 6c61 6d61 223a 0a20 2020 2020   "ollama":.     
+000115d0: 2020 2020 2020 2064 6566 6175 6c74 203d         default =
+000115e0: 2063 6f6e 6669 672e 6f6c 6c61 6d61 4d61   config.ollamaMa
+000115f0: 696e 4d6f 6465 6c5f 6e75 6d5f 7072 6564  inModel_num_pred
+00011600: 6963 740a 2020 2020 2020 2020 6d61 7874  ict.        maxt
+00011610: 6f6b 656e 7320 3d20 7365 6c66 2e70 726f  okens = self.pro
+00011620: 6d70 7473 2e73 696d 706c 6550 726f 6d70  mpts.simplePromp
+00011630: 7428 7374 796c 653d 7365 6c66 2e70 726f  t(style=self.pro
+00011640: 6d70 7473 2e70 726f 6d70 7453 7479 6c65  mpts.promptStyle
+00011650: 322c 206e 756d 6265 724f 6e6c 793d 5472  2, numberOnly=Tr
+00011660: 7565 2c20 6465 6661 756c 743d 7374 7228  ue, default=str(
+00011670: 6465 6661 756c 7429 290a 2020 2020 2020  default)).      
+00011680: 2020 6966 206d 6178 746f 6b65 6e73 2061    if maxtokens a
+00011690: 6e64 206e 6f74 206d 6178 746f 6b65 6e73  nd not maxtokens
+000116a0: 2e73 7472 6970 2829 2e6c 6f77 6572 2829  .strip().lower()
+000116b0: 203d 3d20 636f 6e66 6967 2e65 7869 745f   == config.exit_
+000116c0: 656e 7472 7920 616e 6420 696e 7428 6d61  entry and int(ma
+000116d0: 7874 6f6b 656e 7329 203e 2030 3a0a 2020  xtokens) > 0:.  
+000116e0: 2020 2020 2020 2020 2020 6d61 7874 6f6b            maxtok
+000116f0: 656e 7320 3d20 696e 7428 6d61 7874 6f6b  ens = int(maxtok
+00011700: 656e 7329 0a20 2020 2020 2020 2020 2020  ens).           
+00011710: 2069 6620 636f 6e66 6967 2e6c 6c6d 496e   if config.llmIn
+00011720: 7465 7266 6163 6520 3d3d 2022 6765 6d69  terface == "gemi
+00011730: 6e69 223a 0a20 2020 2020 2020 2020 2020  ni":.           
+00011740: 2020 2020 2063 6f6e 6669 672e 6765 6d69       config.gemi
+00011750: 6e69 7072 6f5f 6d61 785f 6f75 7470 7574  nipro_max_output
+00011760: 5f74 6f6b 656e 7320 3d20 6d61 7874 6f6b  _tokens = maxtok
+00011770: 656e 730a 2020 2020 2020 2020 2020 2020  ens.            
+00011780: 656c 6966 2063 6f6e 6669 672e 6c6c 6d49  elif config.llmI
+00011790: 6e74 6572 6661 6365 203d 3d20 226c 6c61  nterface == "lla
+000117a0: 6d61 6370 7022 3a0a 2020 2020 2020 2020  macpp":.        
+000117b0: 2020 2020 2020 2020 636f 6e66 6967 2e6c          config.l
+000117c0: 6c61 6d61 6370 704d 6169 6e4d 6f64 656c  lamacppMainModel
+000117d0: 5f6d 6178 5f74 6f6b 656e 7320 3d20 6d61  _max_tokens = ma
+000117e0: 7874 6f6b 656e 730a 2020 2020 2020 2020  xtokens.        
+000117f0: 2020 2020 656c 6966 2063 6f6e 6669 672e      elif config.
+00011800: 6c6c 6d49 6e74 6572 6661 6365 203d 3d20  llmInterface == 
+00011810: 226f 6c6c 616d 6122 3a0a 2020 2020 2020  "ollama":.      
+00011820: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00011830: 2e6f 6c6c 616d 614d 6169 6e4d 6f64 656c  .ollamaMainModel
+00011840: 5f6e 756d 5f70 7265 6469 6374 203d 206d  _num_predict = m
+00011850: 6178 746f 6b65 6e73 0a20 2020 2020 2020  axtokens.       
+00011860: 2020 2020 2063 6f6e 6669 672e 7361 7665       config.save
+00011870: 436f 6e66 6967 2829 0a20 2020 2020 2020  Config().       
+00011880: 2020 2020 2070 7269 6e74 3328 6622 4d61       print3(f"Ma
+00011890: 7869 6d75 6d20 6f75 7470 7574 2074 6f6b  ximum output tok
+000118a0: 656e 733a 207b 636f 6e66 6967 2e63 6861  ens: {config.cha
+000118b0: 7447 5054 4170 694d 696e 546f 6b65 6e73  tGPTApiMinTokens
+000118c0: 7d22 290a 0a20 2020 2064 6566 2073 6574  }")..    def set
+000118d0: 4d61 7854 6f6b 656e 7328 7365 6c66 293a  MaxTokens(self):
+000118e0: 0a20 2020 2020 2020 2023 206e 6f6e 2d63  .        # non-c
+000118f0: 6861 7467 7074 2073 6574 7469 6e67 730a  hatgpt settings.
+00011900: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00011910: 6f6e 6669 672e 6c6c 6d49 6e74 6572 6661  onfig.llmInterfa
+00011920: 6365 2069 6e20 2822 6368 6174 6770 7422  ce in ("chatgpt"
+00011930: 2c20 226c 6574 6d65 646f 6974 2229 3a0a  , "letmedoit"):.
+00011940: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011950: 2e73 6574 4d61 7854 6f6b 656e 735f 6e6f  .setMaxTokens_no
+00011960: 6e5f 6368 6174 6770 7428 290a 2020 2020  n_chatgpt().    
+00011970: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00011980: 6f6e 650a 2020 2020 2020 2020 2320 6368  one.        # ch
+00011990: 6174 6770 7420 7365 7474 696e 6773 0a20  atgpt settings. 
+000119a0: 2020 2020 2020 2063 6f6e 7465 7874 5769         contextWi
+000119b0: 6e64 6f77 4c69 6d69 742c 2066 756e 6374  ndowLimit, funct
+000119c0: 696f 6e54 6f6b 656e 732c 2074 6f6b 656e  ionTokens, token
+000119d0: 4c69 6d69 7420 3d20 7365 6c66 2e67 6574  Limit = self.get
+000119e0: 4d61 7854 6f6b 656e 7328 290a 2020 2020  MaxTokens().    
+000119f0: 2020 2020 6966 2074 6f6b 656e 4c69 6d69      if tokenLimi
+00011a00: 7420 3c20 636f 6e66 6967 2e63 6861 7447  t < config.chatG
+00011a10: 5054 4170 694d 696e 546f 6b65 6e73 3a0a  PTApiMinTokens:.
+00011a20: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00011a30: 7432 2866 2246 756e 6374 696f 6e20 746f  t2(f"Function to
+00011a40: 6b65 6e73 205b 7b66 756e 6374 696f 6e54  kens [{functionT
+00011a50: 6f6b 656e 737d 5d20 6578 6365 6564 207b  okens}] exceed {
+00011a60: 636f 6e66 6967 2e63 6861 7447 5054 4170  config.chatGPTAp
+00011a70: 694d 6f64 656c 7d20 6f75 7470 7574 2074  iModel} output t
+00011a80: 6f6b 656e 206c 696d 6974 2e22 290a 2020  oken limit.").  
+00011a90: 2020 2020 2020 2020 2020 7072 696e 7431            print1
+00011aa0: 2822 4569 7468 6572 2063 6861 6e67 6520  ("Either change 
+00011ab0: 746f 2061 206d 6f64 656c 2077 6974 6820  to a model with 
+00011ac0: 6869 6768 6572 2074 6f6b 656e 206c 696d  higher token lim
+00011ad0: 6974 206f 7220 6469 7361 626c 6520 756e  it or disable un
+00011ae0: 7573 6564 2066 756e 6374 696f 6e2d 6361  used function-ca
+00011af0: 6c6c 2070 6c67 7569 6e73 2e22 290a 2020  ll plguins.").  
+00011b00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00011b10: 2020 2020 2020 2020 7072 696e 7431 2873          print1(s
+00011b20: 656c 662e 6469 7669 6465 7229 0a20 2020  elf.divider).   
+00011b30: 2020 2020 2020 2020 2070 7269 6e74 3128           print1(
+00011b40: 2247 5054 2061 6e64 2065 6d62 6564 6469  "GPT and embeddi
+00011b50: 6e67 7320 6d6f 6465 6c73 2070 726f 6365  ngs models proce
+00011b60: 7373 2074 6578 7420 696e 2063 6875 6e6b  ss text in chunk
+00011b70: 7320 6361 6c6c 6564 2074 6f6b 656e 732e  s called tokens.
+00011b80: 2041 7320 6120 726f 7567 6820 7275 6c65   As a rough rule
+00011b90: 206f 6620 7468 756d 622c 2031 2074 6f6b   of thumb, 1 tok
+00011ba0: 656e 2069 7320 6170 7072 6f78 696d 6174  en is approximat
+00011bb0: 656c 7920 3420 6368 6172 6163 7465 7273  ely 4 characters
+00011bc0: 206f 7220 302e 3735 2077 6f72 6473 2066   or 0.75 words f
+00011bd0: 6f72 2045 6e67 6c69 7368 2074 6578 742e  or English text.
+00011be0: 204f 6e65 206c 696d 6974 6174 696f 6e20   One limitation 
+00011bf0: 746f 206b 6565 7020 696e 206d 696e 6420  to keep in mind 
+00011c00: 6973 2074 6861 7420 666f 7220 6120 4750  is that for a GP
+00011c10: 5420 6d6f 6465 6c20 7468 6520 7072 6f6d  T model the prom
+00011c20: 7074 2061 6e64 2074 6865 2067 656e 6572  pt and the gener
+00011c30: 6174 6564 206f 7574 7075 7420 636f 6d62  ated output comb
+00011c40: 696e 6564 206d 7573 7420 6265 206e 6f20  ined must be no 
+00011c50: 6d6f 7265 2074 6861 6e20 7468 6520 6d6f  more than the mo
+00011c60: 6465 6c27 7320 6d61 7869 6d75 6d20 636f  del's maximum co
+00011c70: 6e74 6578 7420 6c65 6e67 7468 2e22 290a  ntext length.").
+00011c80: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00011c90: 7433 2866 2243 7572 7265 6e74 2047 5054  t3(f"Current GPT
+00011ca0: 206d 6f64 656c 3a20 7b63 6f6e 6669 672e   model: {config.
+00011cb0: 6368 6174 4750 5441 7069 4d6f 6465 6c7d  chatGPTApiModel}
+00011cc0: 2229 0a20 2020 2020 2020 2020 2020 2070  ").            p
+00011cd0: 7269 6e74 3328 6622 4d61 7869 6d75 6d20  rint3(f"Maximum 
+00011ce0: 636f 6e74 6578 7420 6c65 6e67 7468 3a20  context length: 
+00011cf0: 7b63 6f6e 7465 7874 5769 6e64 6f77 4c69  {contextWindowLi
+00011d00: 6d69 747d 2229 0a20 2020 2020 2020 2020  mit}").         
+00011d10: 2020 2070 7269 6e74 3328 6622 4375 7272     print3(f"Curr
+00011d20: 656e 7420 6675 6e63 7469 6f6e 2074 6f6b  ent function tok
+00011d30: 656e 733a 207b 6675 6e63 7469 6f6e 546f  ens: {functionTo
+00011d40: 6b65 6e73 7d22 290a 2020 2020 2020 2020  kens}").        
+00011d50: 2020 2020 7072 696e 7433 2866 224d 6178      print3(f"Max
+00011d60: 696d 756d 206f 7574 7075 7420 746f 6b65  imum output toke
+00011d70: 6e20 616c 6c6f 7765 6420 2865 7863 6c2e  n allowed (excl.
+00011d80: 2066 756e 6374 696f 6e73 293a 207b 746f   functions): {to
+00011d90: 6b65 6e4c 696d 6974 7d22 290a 2020 2020  kenLimit}").    
+00011da0: 2020 2020 2020 2020 7072 696e 7431 2873          print1(s
+00011db0: 656c 662e 6469 7669 6465 7229 0a20 2020  elf.divider).   
+00011dc0: 2020 2020 2020 2020 2070 7269 6e74 3128           print1(
+00011dd0: 2250 6c65 6173 6520 7370 6563 6966 7920  "Please specify 
+00011de0: 6d61 7869 6d75 6d20 6f75 7470 7574 2074  maximum output t
+00011df0: 6f6b 656e 7320 6265 6c6f 773a 2229 0a20  okens below:"). 
+00011e00: 2020 2020 2020 2020 2020 206d 6178 746f             maxto
+00011e10: 6b65 6e73 203d 2073 656c 662e 7072 6f6d  kens = self.prom
+00011e20: 7074 732e 7369 6d70 6c65 5072 6f6d 7074  pts.simplePrompt
+00011e30: 2873 7479 6c65 3d73 656c 662e 7072 6f6d  (style=self.prom
+00011e40: 7074 732e 7072 6f6d 7074 5374 796c 6532  pts.promptStyle2
+00011e50: 2c20 6e75 6d62 6572 4f6e 6c79 3d54 7275  , numberOnly=Tru
+00011e60: 652c 2064 6566 6175 6c74 3d73 7472 2863  e, default=str(c
+00011e70: 6f6e 6669 672e 6368 6174 4750 5441 7069  onfig.chatGPTApi
+00011e80: 4d61 7854 6f6b 656e 7329 290a 2020 2020  MaxTokens)).    
+00011e90: 2020 2020 2020 2020 6966 206d 6178 746f          if maxto
+00011ea0: 6b65 6e73 2061 6e64 206e 6f74 206d 6178  kens and not max
+00011eb0: 746f 6b65 6e73 2e73 7472 6970 2829 2e6c  tokens.strip().l
+00011ec0: 6f77 6572 2829 203d 3d20 636f 6e66 6967  ower() == config
+00011ed0: 2e65 7869 745f 656e 7472 7920 616e 6420  .exit_entry and 
+00011ee0: 696e 7428 6d61 7874 6f6b 656e 7329 203e  int(maxtokens) >
+00011ef0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00011f00: 2020 2020 636f 6e66 6967 2e63 6861 7447      config.chatG
+00011f10: 5054 4170 694d 6178 546f 6b65 6e73 203d  PTApiMaxTokens =
+00011f20: 2069 6e74 286d 6178 746f 6b65 6e73 290a   int(maxtokens).
+00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f40: 6966 2063 6f6e 6669 672e 6368 6174 4750  if config.chatGP
+00011f50: 5441 7069 4d61 7854 6f6b 656e 7320 3e20  TApiMaxTokens > 
+00011f60: 746f 6b65 6e4c 696d 6974 3a0a 2020 2020  tokenLimit:.    
+00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f80: 636f 6e66 6967 2e63 6861 7447 5054 4170  config.chatGPTAp
+00011f90: 694d 6178 546f 6b65 6e73 203d 2074 6f6b  iMaxTokens = tok
+00011fa0: 656e 4c69 6d69 740a 2020 2020 2020 2020  enLimit.        
+00011fb0: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
+00011fc0: 6176 6543 6f6e 6669 6728 290a 2020 2020  aveConfig().    
+00011fd0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00011fe0: 7433 2866 224d 6178 696d 756d 206f 7574  t3(f"Maximum out
+00011ff0: 7075 7420 746f 6b65 6e73 3a20 7b63 6f6e  put tokens: {con
+00012000: 6669 672e 6368 6174 4750 5441 7069 4d61  fig.chatGPTApiMa
+00012010: 7854 6f6b 656e 737d 2229 0a0a 2020 2020  xTokens}")..    
+00012020: 6465 6620 7275 6e53 7973 7465 6d43 6f6d  def runSystemCom
+00012030: 6d61 6e64 2873 656c 662c 2063 6f6d 6d61  mand(self, comma
+00012040: 6e64 293a 0a20 2020 2020 2020 2063 6f6d  nd):.        com
+00012050: 6d61 6e64 203d 2063 6f6d 6d61 6e64 2e73  mand = command.s
+00012060: 7472 6970 2829 5b31 3a5d 0a20 2020 2020  trip()[1:].     
+00012070: 2020 2069 6620 225c 6e22 2069 6e20 636f     if "\n" in co
+00012080: 6d6d 616e 643a 0a20 2020 2020 2020 2020  mmand:.         
+00012090: 2020 2063 6f6d 6d61 6e64 203d 2022 3b22     command = ";"
+000120a0: 2e6a 6f69 6e28 636f 6d6d 616e 642e 7370  .join(command.sp
+000120b0: 6c69 7428 225c 6e22 2929 0a20 2020 2020  lit("\n")).     
+000120c0: 2020 2069 6620 636f 6e66 6967 2e74 6869     if config.thi
+000120d0: 7350 6c61 7466 6f72 6d20 3d3d 2022 5769  sPlatform == "Wi
+000120e0: 6e64 6f77 7322 3a0a 2020 2020 2020 2020  ndows":.        
+000120f0: 2020 2020 6f73 2e73 7973 7465 6d28 636f      os.system(co
+00012100: 6d6d 616e 6429 0a20 2020 2020 2020 2065  mmand).        e
+00012110: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00012120: 206f 732e 7379 7374 656d 2866 2265 6e76   os.system(f"env
+00012130: 2051 545f 5150 415f 504c 4154 464f 524d   QT_QPA_PLATFORM
+00012140: 5f50 4c55 4749 4e5f 5041 5448 3d27 7b63  _PLUGIN_PATH='{c
+00012150: 6f6e 6669 672e 656e 765f 5154 5f51 5041  onfig.env_QT_QPA
+00012160: 5f50 4c41 5446 4f52 4d5f 504c 5547 494e  _PLATFORM_PLUGIN
+00012170: 5f50 4154 487d 2720 7b63 6f6d 6d61 6e64  _PATH}' {command
+00012180: 7d22 290a 0a20 2020 2064 6566 2074 6f67  }")..    def tog
+00012190: 676c 654d 756c 7469 6c69 6e65 2873 656c  gleMultiline(sel
+000121a0: 6629 3a0a 2020 2020 2020 2020 636f 6e66  f):.        conf
+000121b0: 6967 2e6d 756c 7469 6c69 6e65 496e 7075  ig.multilineInpu
+000121c0: 7420 3d20 6e6f 7420 636f 6e66 6967 2e6d  t = not config.m
+000121d0: 756c 7469 6c69 6e65 496e 7075 740a 2020  ultilineInput.  
+000121e0: 2020 2020 2020 7275 6e5f 696e 5f74 6572        run_in_ter
+000121f0: 6d69 6e61 6c28 6c61 6d62 6461 3a20 7072  minal(lambda: pr
+00012200: 696e 7431 2866 224d 756c 7469 2d6c 696e  int1(f"Multi-lin
+00012210: 6520 696e 7075 7420 7b27 656e 6162 6c65  e input {'enable
+00012220: 6427 2069 6620 636f 6e66 6967 2e6d 756c  d' if config.mul
+00012230: 7469 6c69 6e65 496e 7075 7420 656c 7365  tilineInput else
+00012240: 2027 6469 7361 626c 6564 277d 2122 2929   'disabled'}!"))
+00012250: 0a20 2020 2020 2020 2069 6620 636f 6e66  .        if conf
+00012260: 6967 2e6d 756c 7469 6c69 6e65 496e 7075  ig.multilineInpu
+00012270: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+00012280: 756e 5f69 6e5f 7465 726d 696e 616c 286c  un_in_terminal(l
+00012290: 616d 6264 613a 2070 7269 6e74 3128 2255  ambda: print1("U
+000122a0: 7365 2027 6573 6361 7065 202b 2065 6e74  se 'escape + ent
+000122b0: 6572 2720 746f 2063 6f6d 706c 6574 6520  er' to complete 
+000122c0: 796f 7572 2065 6e74 7279 2e22 2929 0a0a  your entry."))..
+000122d0: 2020 2020 6465 6620 6973 5474 7341 7661      def isTtsAva
+000122e0: 696c 6162 6c65 2873 656c 6629 3a0a 2020  ilable(self):.  
+000122f0: 2020 2020 2020 6966 206e 6f74 2063 6f6e        if not con
+00012300: 6669 672e 6973 566c 6350 6c61 7965 7249  fig.isVlcPlayerI
+00012310: 6e73 7461 6c6c 6564 2061 6e64 206e 6f74  nstalled and not
+00012320: 2063 6f6e 6669 672e 6973 5079 6761 6d65   config.isPygame
+00012330: 496e 7374 616c 6c65 6420 616e 6420 6e6f  Installed and no
+00012340: 7420 636f 6e66 6967 2e74 7473 436f 6d6d  t config.ttsComm
+00012350: 616e 6420 616e 6420 6e6f 7420 636f 6e66  and and not conf
+00012360: 6967 2e65 6c65 7665 6e6c 6162 7341 7069  ig.elevenlabsApi
+00012370: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00012380: 696e 7432 2822 5465 7874 2d74 6f2d 7370  int2("Text-to-sp
+00012390: 6565 6368 2066 6561 7475 7265 2069 7320  eech feature is 
+000123a0: 6e6f 7420 656e 6162 6c65 6421 2229 0a20  not enabled!"). 
+000123b0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000123c0: 3328 2252 6561 643a 2068 7474 7073 3a2f  3("Read: https:/
+000123d0: 2f67 6974 6875 622e 636f 6d2f 656c 6972  /github.com/elir
+000123e0: 616e 776f 6e67 2f6c 6574 6d65 646f 6974  anwong/letmedoit
+000123f0: 2f77 696b 692f 6c65 744d 6544 6f49 742d  /wiki/letMeDoIt-
+00012400: 5370 6561 6b73 2229 0a20 2020 2020 2020  Speaks").       
+00012410: 2020 2020 2063 6f6e 6669 672e 7474 7320       config.tts 
+00012420: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00012430: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00012440: 2020 636f 6e66 6967 2e74 7473 203d 2054    config.tts = T
+00012450: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
+00012460: 726e 2063 6f6e 6669 672e 7474 730a 0a20  rn config.tts.. 
+00012470: 2020 2064 6566 2074 6f67 676c 6569 6e70     def toggleinp
+00012480: 7574 6175 6469 6f28 7365 6c66 293a 0a20  utaudio(self):. 
+00012490: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+000124a0: 7354 7473 4176 6169 6c61 626c 653a 0a20  sTtsAvailable:. 
+000124b0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+000124c0: 672e 7474 7349 6e70 7574 203d 206e 6f74  g.ttsInput = not
+000124d0: 2063 6f6e 6669 672e 7474 7349 6e70 7574   config.ttsInput
+000124e0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+000124f0: 6669 672e 7361 7665 436f 6e66 6967 2829  fig.saveConfig()
+00012500: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00012510: 6e74 3328 6622 496e 7075 7420 4175 6469  nt3(f"Input Audi
+00012520: 6f3a 2027 7b27 656e 6162 6c65 6427 2069  o: '{'enabled' i
+00012530: 6620 636f 6e66 6967 2e74 7473 496e 7075  f config.ttsInpu
+00012540: 7420 656c 7365 2027 6469 7361 626c 6564  t else 'disabled
+00012550: 277d 2721 2229 0a0a 2020 2020 6465 6620  '}'!")..    def 
+00012560: 746f 6767 6c65 7265 7370 6f6e 7365 6175  toggleresponseau
+00012570: 6469 6f28 7365 6c66 293a 0a20 2020 2020  dio(self):.     
+00012580: 2020 2069 6620 7365 6c66 2e69 7354 7473     if self.isTts
+00012590: 4176 6169 6c61 626c 653a 0a20 2020 2020  Available:.     
+000125a0: 2020 2020 2020 2063 6f6e 6669 672e 7474         config.tt
+000125b0: 734f 7574 7075 7420 3d20 6e6f 7420 636f  sOutput = not co
+000125c0: 6e66 6967 2e74 7473 4f75 7470 7574 0a20  nfig.ttsOutput. 
+000125d0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+000125e0: 672e 7361 7665 436f 6e66 6967 2829 0a20  g.saveConfig(). 
+000125f0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00012600: 3328 6622 5265 7370 6f6e 7365 2041 7564  3(f"Response Aud
+00012610: 696f 3a20 277b 2765 6e61 626c 6564 2720  io: '{'enabled' 
+00012620: 6966 2063 6f6e 6669 672e 7474 734f 7574  if config.ttsOut
+00012630: 7075 7420 656c 7365 2027 6469 7361 626c  put else 'disabl
+00012640: 6564 277d 2721 2229 0a0a 2020 2020 6465  ed'}'!")..    de
+00012650: 6620 6465 6669 6e65 5474 7343 6f6d 6d61  f defineTtsComma
+00012660: 6e64 2873 656c 6629 3a0a 2020 2020 2020  nd(self):.      
+00012670: 2020 7072 696e 7431 2822 4465 6669 6e65    print1("Define
+00012680: 2063 7573 746f 6d20 7465 7874 2d74 6f2d   custom text-to-
+00012690: 7370 6565 6368 2063 6f6d 6d61 6e64 2062  speech command b
+000126a0: 656c 6f77 3a22 290a 2020 2020 2020 2020  elow:").        
+000126b0: 7072 696e 7431 2822 2222 2a20 6f6e 206d  print1("""* on m
+000126c0: 6163 4f53 205b 2773 6179 202d 7620 223f  acOS ['say -v "?
+000126d0: 2227 2074 6f20 6368 6563 6b20 766f 6963  "' to check voic
+000126e0: 6573 5d2c 2065 2e67 2e3a 5c6e 2773 6179  es], e.g.:\n'say
+000126f0: 2720 6f72 2027 7361 7920 2d72 2032 3030  ' or 'say -r 200
+00012700: 202d 7620 4461 6e69 656c 2722 2222 290a   -v Daniel'""").
+00012710: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+00012720: 2a20 6f6e 2055 6275 6e74 7520 5b27 6573  * on Ubuntu ['es
+00012730: 7065 616b 202d 2d76 6f69 6365 7327 2074  peak --voices' t
+00012740: 6f20 6368 6563 6b20 766f 6963 6573 5d2c  o check voices],
+00012750: 2065 2e67 2e3a 5c6e 2765 7370 6561 6b27   e.g.:\n'espeak'
+00012760: 206f 7220 2765 7370 6561 6b20 2d73 2031   or 'espeak -s 1
+00012770: 3735 202d 7620 656e 2d67 6227 2229 0a20  75 -v en-gb'"). 
+00012780: 2020 2020 2020 2070 7269 6e74 3128 222a         print1("*
+00012790: 206f 6e20 5769 6e64 6f77 732c 2073 696d   on Windows, sim
+000127a0: 706c 7920 656e 7465 7220 2777 696e 646f  ply enter 'windo
+000127b0: 7773 2720 6865 7265 2074 6f20 7573 6520  ws' here to use 
+000127c0: 5769 6e64 6f77 7320 6275 696c 742d 696e  Windows built-in
+000127d0: 2073 7065 6563 6820 656e 6769 6e65 2229   speech engine")
+000127e0: 2023 206c 6574 6d65 646f 6974 2e61 6920   # letmedoit.ai 
+000127f0: 7769 6c6c 2068 616e 646c 6520 7468 6520  will handle the 
+00012800: 636f 6d6d 616e 6420 666f 7220 5769 6e64  command for Wind
+00012810: 6f77 7320 7573 6572 730a 2020 2020 2020  ows users.      
+00012820: 2020 7072 696e 7431 2822 7265 6d61 726b    print1("remark
+00012830: 733a 2061 6c77 6179 7320 706c 6163 6520  s: always place 
+00012840: 7468 6520 766f 6963 6520 6f70 7469 6f6e  the voice option
+00012850: 2c20 6966 2061 6e79 2c20 6174 2074 6865  , if any, at the
+00012860: 2065 6e64 2229 0a20 2020 2020 2020 2074   end").        t
+00012870: 7473 436f 6d6d 616e 6420 3d20 7365 6c66  tsCommand = self
+00012880: 2e70 726f 6d70 7473 2e73 696d 706c 6550  .prompts.simpleP
+00012890: 726f 6d70 7428 7374 796c 653d 7365 6c66  rompt(style=self
+000128a0: 2e70 726f 6d70 7473 2e70 726f 6d70 7453  .prompts.promptS
+000128b0: 7479 6c65 322c 2064 6566 6175 6c74 3d63  tyle2, default=c
+000128c0: 6f6e 6669 672e 7474 7343 6f6d 6d61 6e64  onfig.ttsCommand
+000128d0: 290a 2020 2020 2020 2020 6966 2074 7473  ).        if tts
+000128e0: 436f 6d6d 616e 643a 0a20 2020 2020 2020  Command:.       
+000128f0: 2020 2020 2070 7269 6e74 3128 2253 7065       print1("Spe
+00012900: 6369 6679 2063 6f6d 6d61 6e64 2073 7566  cify command suf
+00012910: 6669 7820 6265 6c6f 772c 2069 6620 616e  fix below, if an
+00012920: 7920 5b6c 6561 7665 2069 7420 626c 616e  y [leave it blan
+00012930: 6b20 6966 204e 2f41 5d3a 2229 0a20 2020  k if N/A]:").   
+00012940: 2020 2020 2020 2020 2074 7473 436f 6d6d           ttsComm
+00012950: 616e 6453 7566 6669 7820 3d20 7365 6c66  andSuffix = self
+00012960: 2e70 726f 6d70 7473 2e73 696d 706c 6550  .prompts.simpleP
+00012970: 726f 6d70 7428 7374 796c 653d 7365 6c66  rompt(style=self
+00012980: 2e70 726f 6d70 7473 2e70 726f 6d70 7453  .prompts.promptS
+00012990: 7479 6c65 322c 2064 6566 6175 6c74 3d63  tyle2, default=c
+000129a0: 6f6e 6669 672e 7474 7343 6f6d 6d61 6e64  onfig.ttsCommand
+000129b0: 5375 6666 6978 290a 2020 2020 2020 2020  Suffix).        
+000129c0: 2020 2020 6966 2074 7473 436f 6d6d 616e      if ttsComman
+000129d0: 642e 6c6f 7765 7228 2920 3d3d 2022 7769  d.lower() == "wi
+000129e0: 6e64 6f77 7322 3a0a 2020 2020 2020 2020  ndows":.        
+000129f0: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
+00012a00: 3d20 6627 2727 506f 7765 7253 6865 6c6c  = f'''PowerShell
+00012a10: 202d 436f 6d6d 616e 6420 2241 6464 2d54   -Command "Add-T
+00012a20: 7970 6520 e280 9341 7373 656d 626c 794e  ype ...AssemblyN
+00012a30: 616d 6520 5379 7374 656d 2e53 7065 6563  ame System.Speec
+00012a40: 683b 2028 4e65 772d 4f62 6a65 6374 2053  h; (New-Object S
+00012a50: 7973 7465 6d2e 5370 6565 6368 2e53 796e  ystem.Speech.Syn
+00012a60: 7468 6573 6973 2e53 7065 6563 6853 796e  thesis.SpeechSyn
+00012a70: 7468 6573 697a 6572 292e 5370 6561 6b28  thesizer).Speak(
+00012a80: 2774 6573 7469 6e67 2729 3b22 2727 270a  'testing');"'''.
+00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012aa0: 7474 7343 6f6d 6d61 6e64 5375 6666 6978  ttsCommandSuffix
+00012ab0: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
+00012ac0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012ad0: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
+00012ae0: 3d20 6627 2727 7b74 7473 436f 6d6d 616e  = f'''{ttsComman
+00012af0: 647d 2022 7465 7374 696e 6722 7b74 7473  d} "testing"{tts
+00012b00: 436f 6d6d 616e 6453 7566 6669 787d 2727  CommandSuffix}''
+00012b10: 270a 2020 2020 2020 2020 2020 2020 5f2c  '.            _,
+00012b20: 2073 7464 4572 7220 3d20 7375 6270 726f   stdErr = subpro
+00012b30: 6365 7373 2e50 6f70 656e 2863 6f6d 6d61  cess.Popen(comma
+00012b40: 6e64 2c20 7368 656c 6c3d 5472 7565 2c20  nd, shell=True, 
+00012b50: 7374 646f 7574 3d73 7562 7072 6f63 6573  stdout=subproces
+00012b60: 732e 5049 5045 2c20 7374 6465 7272 3d73  s.PIPE, stderr=s
+00012b70: 7562 7072 6f63 6573 732e 5049 5045 292e  ubprocess.PIPE).
+00012b80: 636f 6d6d 756e 6963 6174 6528 290a 2020  communicate().  
+00012b90: 2020 2020 2020 2020 2020 6966 2073 7464            if std
+00012ba0: 4572 723a 0a20 2020 2020 2020 2020 2020  Err:.           
+00012bb0: 2020 2020 2073 686f 7745 7272 6f72 7328       showErrors(
+00012bc0: 2920 6966 2063 6f6e 6669 672e 6465 7665  ) if config.deve
+00012bd0: 6c6f 7065 7220 656c 7365 2070 7269 6e74  loper else print
+00012be0: 3128 2245 6e74 6572 6564 2063 6f6d 6d61  1("Entered comma
+00012bf0: 6e64 2069 6e76 616c 6964 2122 290a 2020  nd invalid!").  
+00012c00: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 636f 6e66 6967 2e74 7473 436f 6d6d 616e  config.ttsComman
+00012c30: 642c 2063 6f6e 6669 672e 7474 7343 6f6d  d, config.ttsCom
+00012c40: 6d61 6e64 5375 6666 6978 203d 2074 7473  mandSuffix = tts
+00012c50: 436f 6d6d 616e 642c 2074 7473 436f 6d6d  Command, ttsComm
+00012c60: 616e 6453 7566 6669 780a 2020 2020 2020  andSuffix.      
+00012c70: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00012c80: 2e73 6176 6543 6f6e 6669 6728 290a 2020  .saveConfig().  
+00012c90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00012ca0: 2020 2020 2020 2020 636f 6e66 6967 2e74          config.t
+00012cb0: 7473 436f 6d6d 616e 642c 2063 6f6e 6669  tsCommand, confi
+00012cc0: 672e 7474 7343 6f6d 6d61 6e64 5375 6666  g.ttsCommandSuff
+00012cd0: 6978 203d 2022 222c 2022 220a 0a20 2020  ix = "", ""..   
+00012ce0: 2064 6566 2074 6f67 676c 6557 6f72 6457   def toggleWordW
+00012cf0: 7261 7028 7365 6c66 293a 0a20 2020 2020  rap(self):.     
+00012d00: 2020 2063 6f6e 6669 672e 7772 6170 576f     config.wrapWo
+00012d10: 7264 7320 3d20 6e6f 7420 636f 6e66 6967  rds = not config
+00012d20: 2e77 7261 7057 6f72 6473 0a20 2020 2020  .wrapWords.     
+00012d30: 2020 2063 6f6e 6669 672e 7361 7665 436f     config.saveCo
+00012d40: 6e66 6967 2829 0a20 2020 2020 2020 2070  nfig().        p
+00012d50: 7269 6e74 3328 6622 576f 7264 2057 7261  rint3(f"Word Wra
+00012d60: 703a 2027 7b27 656e 6162 6c65 6427 2069  p: '{'enabled' i
+00012d70: 6620 636f 6e66 6967 2e77 7261 7057 6f72  f config.wrapWor
+00012d80: 6473 2065 6c73 6520 2764 6973 6162 6c65  ds else 'disable
+00012d90: 6427 7d27 2122 290a 0a20 2020 2064 6566  d'}'!")..    def
+00012da0: 2074 6f67 676c 654d 6f75 7365 5375 7070   toggleMouseSupp
+00012db0: 6f72 7428 7365 6c66 293a 0a20 2020 2020  ort(self):.     
+00012dc0: 2020 2063 6f6e 6669 672e 6d6f 7573 6553     config.mouseS
+00012dd0: 7570 706f 7274 203d 206e 6f74 2063 6f6e  upport = not con
+00012de0: 6669 672e 6d6f 7573 6553 7570 706f 7274  fig.mouseSupport
+00012df0: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
+00012e00: 7361 7665 436f 6e66 6967 2829 0a20 2020  saveConfig().   
+00012e10: 2020 2020 2070 7269 6e74 3328 6622 456e       print3(f"En
+00012e20: 7472 7920 4d6f 7573 6520 5375 7070 6f72  try Mouse Suppor
+00012e30: 743a 2027 7b27 656e 6162 6c65 6427 2069  t: '{'enabled' i
+00012e40: 6620 636f 6e66 6967 2e6d 6f75 7365 5375  f config.mouseSu
+00012e50: 7070 6f72 7420 656c 7365 2027 6469 7361  pport else 'disa
+00012e60: 626c 6564 277d 2721 2229 0a0a 2020 2020  bled'}'!")..    
+00012e70: 6465 6620 746f 6767 6c65 496d 7072 6f76  def toggleImprov
+00012e80: 6564 5772 6974 696e 6728 7365 6c66 293a  edWriting(self):
+00012e90: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
+00012ea0: 6469 7370 6c61 7949 6d70 726f 7665 6457  displayImprovedW
+00012eb0: 7269 7469 6e67 203d 206e 6f74 2063 6f6e  riting = not con
+00012ec0: 6669 672e 6469 7370 6c61 7949 6d70 726f  fig.displayImpro
+00012ed0: 7665 6457 7269 7469 6e67 0a20 2020 2020  vedWriting.     
+00012ee0: 2020 2069 6620 636f 6e66 6967 2e64 6973     if config.dis
+00012ef0: 706c 6179 496d 7072 6f76 6564 5772 6974  playImprovedWrit
+00012f00: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00012f10: 2070 7269 6e74 3128 2250 6c65 6173 6520   print1("Please 
+00012f20: 7370 6563 6966 7920 7468 6520 7772 6974  specify the writ
+00012f30: 696e 6720 7374 796c 6520 6265 6c6f 773a  ing style below:
+00012f40: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+00012f50: 7479 6c65 203d 2073 656c 662e 7072 6f6d  tyle = self.prom
+00012f60: 7074 732e 7369 6d70 6c65 5072 6f6d 7074  pts.simplePrompt
+00012f70: 2873 7479 6c65 3d73 656c 662e 7072 6f6d  (style=self.prom
+00012f80: 7074 732e 7072 6f6d 7074 5374 796c 6532  pts.promptStyle2
+00012f90: 2c20 6465 6661 756c 743d 636f 6e66 6967  , default=config
+00012fa0: 2e69 6d70 726f 7665 6457 7269 7469 6e67  .improvedWriting
+00012fb0: 5379 746c 6529 0a20 2020 2020 2020 2020  Sytle).         
+00012fc0: 2020 2069 6620 7374 796c 6520 616e 6420     if style and 
+00012fd0: 6e6f 7420 7374 796c 6520 696e 2028 636f  not style in (co
+00012fe0: 6e66 6967 2e65 7869 745f 656e 7472 792c  nfig.exit_entry,
+00012ff0: 2063 6f6e 6669 672e 6361 6e63 656c 5f65   config.cancel_e
+00013000: 6e74 7279 293a 0a20 2020 2020 2020 2020  ntry):.         
+00013010: 2020 2020 2020 2063 6f6e 6669 672e 696d         config.im
+00013020: 7072 6f76 6564 5772 6974 696e 6753 7974  provedWritingSyt
+00013030: 6c65 203d 2073 7479 6c65 0a20 2020 2020  le = style.     
+00013040: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00013050: 672e 7361 7665 436f 6e66 6967 2829 0a20  g.saveConfig(). 
+00013060: 2020 2020 2020 2070 7269 6e74 3328 6622         print3(f"
+00013070: 496d 7072 6f76 6564 2057 7269 7469 6e67  Improved Writing
+00013080: 2044 6973 706c 6179 3a20 277b 2765 6e61   Display: '{'ena
+00013090: 626c 6564 2720 6966 2063 6f6e 6669 672e  bled' if config.
+000130a0: 6469 7370 6c61 7949 6d70 726f 7665 6457  displayImprovedW
+000130b0: 7269 7469 6e67 2065 6c73 6520 2764 6973  riting else 'dis
+000130c0: 6162 6c65 6427 7d27 2122 290a 0a20 2020  abled'}'!")..   
+000130d0: 2064 6566 2073 6574 4175 6469 6f50 6c61   def setAudioPla
+000130e0: 7962 6163 6b54 6f6f 6c28 7365 6c66 293a  ybackTool(self):
+000130f0: 0a20 2020 2020 2020 2070 6c61 7962 6163  .        playbac
+00013100: 6b20 3d20 7365 6c66 2e64 6961 6c6f 6773  k = self.dialogs
+00013110: 2e67 6574 5661 6c69 644f 7074 696f 6e73  .getValidOptions
+00013120: 280a 2020 2020 2020 2020 2020 2020 6f70  (.            op
+00013130: 7469 6f6e 733d 2822 7079 6761 6d65 222c  tions=("pygame",
+00013140: 2022 766c 6322 292c 0a20 2020 2020 2020   "vlc"),.       
+00013150: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00013160: 733d 2822 5079 4761 6d65 222c 2066 2256  s=("PyGame", f"V
+00013170: 4c43 2050 6c61 7965 7220 2877 2f20 7370  LC Player (w/ sp
+00013180: 6565 6420 636f 6e74 726f 6c29 7b27 205b  eed control){' [
+00013190: 696e 7374 616c 6c61 7469 6f6e 2072 6571  installation req
+000131a0: 7569 7265 645d 2720 6966 206e 6f74 2063  uired]' if not c
+000131b0: 6f6e 6669 672e 6973 566c 6350 6c61 7965  onfig.isVlcPlaye
+000131c0: 7249 6e73 7461 6c6c 6564 2065 6c73 6520  rInstalled else 
+000131d0: 2727 7d22 292c 0a20 2020 2020 2020 2020  ''}"),.         
+000131e0: 2020 2074 6974 6c65 3d22 5465 7874 2d74     title="Text-t
+000131f0: 6f2d 5370 6565 6368 2050 6c61 7962 6163  o-Speech Playbac
+00013200: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
+00013210: 7465 7874 3d22 5365 6c65 6374 2061 2074  text="Select a t
+00013220: 6578 742d 746f 2d73 7065 6563 6820 706c  ext-to-speech pl
+00013230: 6163 6b62 6163 6b20 746f 6f6c 3a22 2c0a  ackback tool:",.
+00013240: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00013250: 756c 743d 2276 6c63 2220 6966 2063 6f6e  ult="vlc" if con
+00013260: 6669 672e 6973 566c 6350 6c61 7965 7249  fig.isVlcPlayerI
+00013270: 6e73 7461 6c6c 6564 2061 6e64 206e 6f74  nstalled and not
+00013280: 2063 6f6e 6669 672e 7573 6550 7967 616d   config.usePygam
+00013290: 6520 656c 7365 2022 7079 6761 6d65 222c  e else "pygame",
+000132a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000132b0: 2020 2069 6620 706c 6179 6261 636b 3a0a     if playback:.
+000132c0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+000132d0: 6c61 7962 6163 6b20 3d3d 2022 766c 6322  layback == "vlc"
+000132e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000132f0: 2020 6966 206e 6f74 2063 6f6e 6669 672e    if not config.
+00013300: 6973 566c 6350 6c61 7965 7249 6e73 7461  isVlcPlayerInsta
+00013310: 6c6c 6564 3a0a 2020 2020 2020 2020 2020  lled:.          
+00013320: 2020 2020 2020 2020 2020 7072 696e 7431            print1
+00013330: 2822 564c 4320 706c 6179 6572 206e 6f74  ("VLC player not
+00013340: 2066 6f75 6e64 2120 496e 7374 616c 6c20   found! Install 
+00013350: 6974 2066 6972 7374 2122 290a 2020 2020  it first!").    
+00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013370: 7072 696e 7433 2822 5465 7874 2d74 6f2d  print3("Text-to-
+00013380: 5370 6565 6368 2050 6c61 7962 6163 6b20  Speech Playback 
+00013390: 6368 616e 6765 6420 746f 3a20 5079 4761  changed to: PyGa
+000133a0: 6d65 2229 0a20 2020 2020 2020 2020 2020  me").           
+000133b0: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
+000133c0: 7573 6550 7967 616d 6520 3d20 5472 7565  usePygame = True
+000133d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000133e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000133f0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00013400: 672e 7573 6550 7967 616d 6520 3d20 4661  g.usePygame = Fa
+00013410: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00013420: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00013430: 2020 2020 2020 636f 6e66 6967 2e75 7365        config.use
+00013440: 5079 6761 6d65 203d 2054 7275 650a 0a20  Pygame = True.. 
+00013450: 2020 2064 6566 2073 6574 5465 7874 546f     def setTextTo
+00013460: 5370 6565 6368 436f 6e66 6967 2873 656c  SpeechConfig(sel
+00013470: 6629 3a0a 2020 2020 2020 2020 7474 7350  f):.        ttsP
+00013480: 6c61 7466 6f72 6d20 3d20 7365 6c66 2e64  latform = self.d
+00013490: 6961 6c6f 6773 2e67 6574 5661 6c69 644f  ialogs.getValidO
+000134a0: 7074 696f 6e73 280a 2020 2020 2020 2020  ptions(.        
+000134b0: 2020 2020 6f70 7469 6f6e 733d 2822 676f      options=("go
+000134c0: 6f67 6c65 222c 2022 676f 6f67 6c65 636c  ogle", "googlecl
+000134d0: 6f75 6422 2c20 2265 6c65 7665 6e6c 6162  oud", "elevenlab
+000134e0: 7322 2c20 2263 7573 746f 6d22 292c 0a20  s", "custom"),. 
+000134f0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00013500: 6970 7469 6f6e 733d 2822 476f 6f67 6c65  iptions=("Google
+00013510: 2054 6578 742d 746f 2d53 7065 6563 6820   Text-to-Speech 
+00013520: 2847 656e 6572 6963 2922 2c20 2247 6f6f  (Generic)", "Goo
+00013530: 676c 6520 5465 7874 2d74 6f2d 5370 6565  gle Text-to-Spee
+00013540: 6368 2028 4150 4929 222c 2022 456c 6576  ch (API)", "Elev
+00013550: 656e 4c61 6273 2028 4150 4929 222c 2022  enLabs (API)", "
+00013560: 4375 7374 6f6d 2054 6578 742d 746f 2d53  Custom Text-to-S
+00013570: 7065 6563 6820 436f 6d6d 616e 6420 5b61  peech Command [a
+00013580: 6476 616e 6365 645d 2229 2c0a 2020 2020  dvanced]"),.    
+00013590: 2020 2020 2020 2020 7469 746c 653d 2254          title="T
+000135a0: 6578 742d 746f 2d53 7065 6563 6820 436f  ext-to-Speech Co
+000135b0: 6e66 6967 7572 6174 696f 6e73 222c 0a20  nfigurations",. 
+000135c0: 2020 2020 2020 2020 2020 2074 6578 743d             text=
+000135d0: 2253 656c 6563 7420 6120 7465 7874 2d74  "Select a text-t
+000135e0: 6f2d 7370 6565 6368 2070 6c61 7466 6f72  o-speech platfor
+000135f0: 6d3a 222c 0a20 2020 2020 2020 2020 2020  m:",.           
+00013600: 2064 6566 6175 6c74 3d63 6f6e 6669 672e   default=config.
+00013610: 7474 7350 6c61 7466 6f72 6d2c 0a20 2020  ttsPlatform,.   
+00013620: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00013630: 6620 7474 7350 6c61 7466 6f72 6d3a 0a20  f ttsPlatform:. 
+00013640: 2020 2020 2020 2020 2020 2069 6620 7474             if tt
+00013650: 7350 6c61 7466 6f72 6d20 3d3d 2022 676f  sPlatform == "go
+00013660: 6f67 6c65 636c 6f75 6422 2061 6e64 206e  oglecloud" and n
+00013670: 6f74 2028 6f73 2e65 6e76 6972 6f6e 5b22  ot (os.environ["
+00013680: 474f 4f47 4c45 5f41 5050 4c49 4341 5449  GOOGLE_APPLICATI
+00013690: 4f4e 5f43 5245 4445 4e54 4941 4c53 225d  ON_CREDENTIALS"]
+000136a0: 2061 6e64 2022 5465 7874 2d74 6f2d 5370   and "Text-to-Sp
+000136b0: 6565 6368 2220 696e 2063 6f6e 6669 672e  eech" in config.
+000136c0: 656e 6162 6c65 6447 6f6f 676c 6541 5049  enabledGoogleAPI
+000136d0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+000136e0: 2020 2020 7072 696e 7432 2822 476f 6f67      print2("Goog
+000136f0: 6c65 2043 6c6f 7564 2054 6578 742d 746f  le Cloud Text-to
+00013700: 2d53 7065 6563 6820 6665 6174 7572 6520  -Speech feature 
+00013710: 6973 206e 6f74 2065 6e61 626c 6564 2122  is not enabled!"
+00013720: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013730: 2020 7072 696e 7433 2822 5265 6164 3a20    print3("Read: 
+00013740: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00013750: 6f6d 2f65 6c69 7261 6e77 6f6e 672f 6c65  om/eliranwong/le
+00013760: 746d 6564 6f69 742f 7769 6b69 2f47 6f6f  tmedoit/wiki/Goo
+00013770: 676c 652d 4150 492d 5365 7475 7022 290a  gle-API-Setup").
+00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013790: 7072 696e 7433 2822 5465 7874 2d74 6f2d  print3("Text-to-
+000137a0: 5370 6565 6368 2070 6c61 7466 6f72 6d20  Speech platform 
+000137b0: 6368 616e 6765 6420 746f 3a20 476f 6f67  changed to: Goog
+000137c0: 6c65 2054 6578 742d 746f 2d53 7065 6563  le Text-to-Speec
+000137d0: 6820 2847 656e 6572 6963 2922 290a 2020  h (Generic)").  
+000137e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000137f0: 6e66 6967 2e74 7473 506c 6174 666f 726d  nfig.ttsPlatform
+00013800: 203d 2022 676f 6f67 6c65 220a 2020 2020   = "google".    
+00013810: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00013820: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00013830: 6e66 6967 2e74 7473 506c 6174 666f 726d  nfig.ttsPlatform
+00013840: 203d 2074 7473 506c 6174 666f 726d 0a20   = ttsPlatform. 
+00013850: 2020 2020 2020 2023 2066 7572 7468 6572         # further
+00013860: 206f 7074 696f 6e73 0a20 2020 2020 2020   options.       
+00013870: 2069 6620 636f 6e66 6967 2e74 7473 506c   if config.ttsPl
+00013880: 6174 666f 726d 203d 3d20 2267 6f6f 676c  atform == "googl
+00013890: 6522 3a0a 2020 2020 2020 2020 2020 2020  e":.            
+000138a0: 7365 6c66 2e73 6574 4774 7473 4c61 6e67  self.setGttsLang
+000138b0: 7561 6765 2829 0a20 2020 2020 2020 2020  uage().         
+000138c0: 2020 2073 656c 662e 7365 7441 7564 696f     self.setAudio
+000138d0: 506c 6179 6261 636b 546f 6f6c 2829 0a20  PlaybackTool(). 
+000138e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000138f0: 7365 7456 6c63 5370 6565 6428 290a 2020  setVlcSpeed().  
+00013900: 2020 2020 2020 656c 6966 2063 6f6e 6669        elif confi
+00013910: 672e 7474 7350 6c61 7466 6f72 6d20 3d3d  g.ttsPlatform ==
+00013920: 2022 676f 6f67 6c65 636c 6f75 6422 3a0a   "googlecloud":.
+00013930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013940: 2e73 6574 4763 7474 734c 616e 6775 6167  .setGcttsLanguag
+00013950: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00013960: 7365 6c66 2e73 6574 4763 7474 7353 7065  self.setGcttsSpe
+00013970: 6564 2829 0a20 2020 2020 2020 2020 2020  ed().           
+00013980: 2073 656c 662e 7365 7441 7564 696f 506c   self.setAudioPl
+00013990: 6179 6261 636b 546f 6f6c 2829 0a20 2020  aybackTool().   
+000139a0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+000139b0: 7456 6c63 5370 6565 6428 290a 2020 2020  tVlcSpeed().    
+000139c0: 2020 2020 656c 6966 2063 6f6e 6669 672e      elif config.
+000139d0: 7474 7350 6c61 7466 6f72 6d20 3d3d 2022  ttsPlatform == "
+000139e0: 656c 6576 656e 6c61 6273 223a 0a20 2020  elevenlabs":.   
+000139f0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00013a00: 636f 6e66 6967 2e65 6c65 7665 6e6c 6162  config.elevenlab
+00013a10: 7341 7069 3a0a 2020 2020 2020 2020 2020  sApi:.          
+00013a20: 2020 2020 2020 7365 6c66 2e63 6861 6e67        self.chang
+00013a30: 6545 6c65 7665 6e6c 6162 7341 7069 2829  eElevenlabsApi()
+00013a40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013a50: 6e6f 7420 636f 6e66 6967 2e65 6c65 7665  not config.eleve
+00013a60: 6e6c 6162 7341 7069 3a0a 2020 2020 2020  nlabsApi:.      
+00013a70: 2020 2020 2020 2020 2020 7072 696e 7431            print1
+00013a80: 2822 456c 6576 656e 4c61 6273 2041 5049  ("ElevenLabs API
+00013a90: 206b 6579 206e 6f74 2066 6f75 6e64 2122   key not found!"
+00013aa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013ab0: 2020 7072 696e 7433 2822 5465 7874 2d74    print3("Text-t
+00013ac0: 6f2d 5370 6565 6368 2070 6c61 7466 6f72  o-Speech platfor
+00013ad0: 6d20 6368 616e 6765 6420 746f 3a20 476f  m changed to: Go
+00013ae0: 6f67 6c65 2054 6578 742d 746f 2d53 7065  ogle Text-to-Spe
+00013af0: 6563 6820 2847 656e 6572 6963 2922 290a  ech (Generic)").
+00013b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b10: 636f 6e66 6967 2e74 7473 506c 6174 666f  config.ttsPlatfo
+00013b20: 726d 203d 2022 676f 6f67 6c65 220a 2020  rm = "google".  
+00013b30: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00013b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b50: 7365 6c66 2e73 6574 456c 6576 656e 6c61  self.setElevenla
+00013b60: 6273 566f 6963 6528 290a 2020 2020 2020  bsVoice().      
+00013b70: 2020 656c 6966 2063 6f6e 6669 672e 7474    elif config.tt
+00013b80: 7350 6c61 7466 6f72 6d20 3d3d 2022 6375  sPlatform == "cu
+00013b90: 7374 6f6d 223a 0a20 2020 2020 2020 2020  stom":.         
+00013ba0: 2020 2073 656c 662e 6465 6669 6e65 5474     self.defineTt
+00013bb0: 7343 6f6d 6d61 6e64 2829 0a20 2020 2020  sCommand().     
+00013bc0: 2020 2023 2073 6176 6520 636f 6e66 6967     # save config
+00013bd0: 730a 2020 2020 2020 2020 636f 6e66 6967  s.        config
+00013be0: 2e73 6176 6543 6f6e 6669 6728 290a 0a20  .saveConfig().. 
+00013bf0: 2020 2064 6566 2073 6574 566f 6963 6554     def setVoiceT
+00013c00: 7970 696e 6743 6f6e 6669 6728 7365 6c66  ypingConfig(self
+00013c10: 293a 0a20 2020 2020 2020 2076 6f69 6365  ):.        voice
+00013c20: 5479 7069 6e67 506c 6174 666f 726d 203d  TypingPlatform =
+00013c30: 2073 656c 662e 6469 616c 6f67 732e 6765   self.dialogs.ge
+00013c40: 7456 616c 6964 4f70 7469 6f6e 7328 0a20  tValidOptions(. 
+00013c50: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+00013c60: 6e73 3d28 2267 6f6f 676c 6522 2c20 2267  ns=("google", "g
+00013c70: 6f6f 676c 6563 6c6f 7564 222c 2022 7768  ooglecloud", "wh
+00013c80: 6973 7065 7222 292c 0a20 2020 2020 2020  isper"),.       
+00013c90: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00013ca0: 733d 2822 476f 6f67 6c65 2053 7065 6563  s=("Google Speec
+00013cb0: 682d 746f 2d54 6578 7420 2847 656e 6572  h-to-Text (Gener
+00013cc0: 6963 2920 5b6f 6e6c 696e 655d 222c 2022  ic) [online]", "
+00013cd0: 476f 6f67 6c65 2053 7065 6563 682d 746f  Google Speech-to
+00013ce0: 2d54 6578 7420 2841 5049 2920 5b6f 6e6c  -Text (API) [onl
+00013cf0: 696e 655d 222c 2022 4f70 656e 4149 2057  ine]", "OpenAI W
+00013d00: 6869 7370 6572 205b 6f66 666c 696e 653b  hisper [offline;
+00013d10: 2073 6c6f 7765 7220 7769 7468 206e 6f6e   slower with non
+00013d20: 2d45 6e67 6c69 7368 2076 6f69 6365 735d  -English voices]
+00013d30: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00013d40: 7469 746c 653d 2256 6f69 6365 2054 7970  title="Voice Typ
+00013d50: 696e 6720 436f 6e66 6967 7572 6174 696f  ing Configuratio
+00013d60: 6e73 222c 0a20 2020 2020 2020 2020 2020  ns",.           
+00013d70: 2074 6578 743d 2253 656c 6563 7420 6120   text="Select a 
+00013d80: 766f 6963 6520 7479 7069 6e67 2070 6c61  voice typing pla
+00013d90: 7466 6f72 6d3a 222c 0a20 2020 2020 2020  tform:",.       
+00013da0: 2020 2020 2064 6566 6175 6c74 3d63 6f6e       default=con
+00013db0: 6669 672e 766f 6963 6554 7970 696e 6750  fig.voiceTypingP
+00013dc0: 6c61 7466 6f72 6d2c 0a20 2020 2020 2020  latform,.       
+00013dd0: 2029 0a20 2020 2020 2020 2069 6620 766f   ).        if vo
+00013de0: 6963 6554 7970 696e 6750 6c61 7466 6f72  iceTypingPlatfor
+00013df0: 6d3a 0a20 2020 2020 2020 2020 2020 2069  m:.            i
+00013e00: 6620 766f 6963 6554 7970 696e 6750 6c61  f voiceTypingPla
+00013e10: 7466 6f72 6d20 3d3d 2022 676f 6f67 6c65  tform == "google
+00013e20: 636c 6f75 6422 2061 6e64 206e 6f74 2028  cloud" and not (
+00013e30: 6f73 2e65 6e76 6972 6f6e 5b22 474f 4f47  os.environ["GOOG
+00013e40: 4c45 5f41 5050 4c49 4341 5449 4f4e 5f43  LE_APPLICATION_C
+00013e50: 5245 4445 4e54 4941 4c53 225d 2061 6e64  REDENTIALS"] and
+00013e60: 2022 5370 6565 6368 2d74 6f2d 5465 7874   "Speech-to-Text
+00013e70: 2220 696e 2063 6f6e 6669 672e 656e 6162  " in config.enab
+00013e80: 6c65 6447 6f6f 676c 6541 5049 7329 3a0a  ledGoogleAPIs):.
+00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ea0: 7072 696e 7432 2822 476f 6f67 6c65 2043  print2("Google C
+00013eb0: 6c6f 7564 2053 7065 6563 682d 746f 2d54  loud Speech-to-T
+00013ec0: 6578 7420 6665 6174 7572 6520 6973 206e  ext feature is n
+00013ed0: 6f74 2065 6e61 626c 6564 2122 290a 2020  ot enabled!").  
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00013ef0: 696e 7433 2822 5265 6164 3a20 6874 7470  int3("Read: http
+00013f00: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00013f10: 6c69 7261 6e77 6f6e 672f 6c65 746d 6564  liranwong/letmed
+00013f20: 6f69 742f 7769 6b69 2f47 6f6f 676c 652d  oit/wiki/Google-
+00013f30: 4150 492d 5365 7475 7022 290a 2020 2020  API-Setup").    
+00013f40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00013f50: 7433 2822 566f 6963 6520 7479 7069 6e67  t3("Voice typing
+00013f60: 2070 6c61 7466 6f72 6d20 6368 616e 6765   platform change
+00013f70: 6420 746f 3a20 476f 6f67 6c65 2053 7065  d to: Google Spe
+00013f80: 6563 682d 746f 2d54 6578 7420 2847 656e  ech-to-Text (Gen
+00013f90: 6572 6963 2922 290a 2020 2020 2020 2020  eric)").        
+00013fa0: 2020 2020 2020 2020 636f 6e66 6967 2e76          config.v
+00013fb0: 6f69 6365 5479 7069 6e67 506c 6174 666f  oiceTypingPlatfo
+00013fc0: 726d 203d 2022 676f 6f67 6c65 220a 2020  rm = "google".  
+00013fd0: 2020 2020 2020 2020 2020 656c 6966 2076            elif v
+00013fe0: 6f69 6365 5479 7069 6e67 506c 6174 666f  oiceTypingPlatfo
+00013ff0: 726d 203d 3d20 2277 6869 7370 6572 2220  rm == "whisper" 
+00014000: 616e 6420 6e6f 7420 6973 436f 6d6d 616e  and not isComman
+00014010: 6449 6e73 7461 6c6c 6564 2822 6666 6d70  dInstalled("ffmp
+00014020: 6567 2229 3a0a 2020 2020 2020 2020 2020  eg"):.          
+00014030: 2020 2020 2020 7072 696e 7432 2822 496e        print2("In
+00014040: 7374 616c 6c20 2766 666d 7065 6727 2066  stall 'ffmpeg' f
+00014050: 6972 7374 2074 6f20 7573 6520 6f66 666c  irst to use offl
+00014060: 696e 6520 6f70 656e 6169 2077 6869 7370  ine openai whisp
+00014070: 6572 206d 6f64 656c 2122 290a 2020 2020  er model!").    
+00014080: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00014090: 7433 2822 5265 6164 3a20 6874 7470 733a  t3("Read: https:
+000140a0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7065  //github.com/ope
+000140b0: 6e61 692f 7768 6973 7065 7223 7365 7475  nai/whisper#setu
+000140c0: 7022 290a 2020 2020 2020 2020 2020 2020  p").            
+000140d0: 2020 2020 7072 696e 7433 2822 566f 6963      print3("Voic
+000140e0: 6520 7479 7069 6e67 2070 6c61 7466 6f72  e typing platfor
+000140f0: 6d20 6368 616e 6765 6420 746f 3a20 476f  m changed to: Go
+00014100: 6f67 6c65 2053 7065 6563 682d 746f 2d54  ogle Speech-to-T
+00014110: 6578 7420 2847 656e 6572 6963 2922 290a  ext (Generic)").
+00014120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014130: 636f 6e66 6967 2e76 6f69 6365 5479 7069  config.voiceTypi
+00014140: 6e67 506c 6174 666f 726d 203d 2022 676f  ngPlatform = "go
+00014150: 6f67 6c65 220a 2020 2020 2020 2020 2020  ogle".          
+00014160: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00014170: 2020 2020 2020 2020 636f 6e66 6967 2e76          config.v
+00014180: 6f69 6365 5479 7069 6e67 506c 6174 666f  oiceTypingPlatfo
+00014190: 726d 203d 2076 6f69 6365 5479 7069 6e67  rm = voiceTyping
+000141a0: 506c 6174 666f 726d 0a20 2020 2020 2020  Platform.       
+000141b0: 2023 206c 616e 6775 6167 650a 2020 2020   # language.    
+000141c0: 2020 2020 7365 6c66 2e73 6574 5370 6565      self.setSpee
+000141d0: 6368 546f 5465 7874 4c61 6e67 7561 6765  chToTextLanguage
+000141e0: 2829 0a20 2020 2020 2020 2023 2063 6f6e  ().        # con
+000141f0: 6669 6775 7265 2063 6f6e 6669 672e 766f  figure config.vo
+00014200: 6963 6554 7970 696e 6741 646a 7573 7441  iceTypingAdjustA
+00014210: 6d62 6965 6e74 4e6f 6973 650a 2020 2020  mbientNoise.    
+00014220: 2020 2020 766f 6963 6554 7970 696e 6741      voiceTypingA
+00014230: 646a 7573 7441 6d62 6965 6e74 4e6f 6973  djustAmbientNois
+00014240: 6520 3d20 7365 6c66 2e64 6961 6c6f 6773  e = self.dialogs
+00014250: 2e67 6574 5661 6c69 644f 7074 696f 6e73  .getValidOptions
+00014260: 280a 2020 2020 2020 2020 2020 2020 6f70  (.            op
+00014270: 7469 6f6e 733d 2822 5965 7322 2c20 224e  tions=("Yes", "N
+00014280: 6f22 292c 0a20 2020 2020 2020 2020 2020  o"),.           
+00014290: 2064 6573 6372 6970 7469 6f6e 733d 2822   descriptions=("
+000142a0: 5965 7320 5b73 6c6f 7765 725d 222c 2022  Yes [slower]", "
+000142b0: 4e6f 2229 2c0a 2020 2020 2020 2020 2020  No"),.          
+000142c0: 2020 7469 746c 653d 2241 646a 7573 7420    title="Adjust 
+000142d0: 416d 6269 656e 7420 4e6f 6973 6522 2c0a  Ambient Noise",.
+000142e0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+000142f0: 3d22 446f 2079 6f75 2077 616e 7420 746f  ="Do you want to
+00014300: 2061 646a 7573 7420 616d 6269 656e 7420   adjust ambient 
+00014310: 6e6f 6973 653f 222c 0a20 2020 2020 2020  noise?",.       
+00014320: 2020 2020 2064 6566 6175 6c74 3d22 5965       default="Ye
+00014330: 7322 2069 6620 636f 6e66 6967 2e76 6f69  s" if config.voi
+00014340: 6365 5479 7069 6e67 4164 6a75 7374 416d  ceTypingAdjustAm
+00014350: 6269 656e 744e 6f69 7365 2065 6c73 6520  bientNoise else 
+00014360: 224e 6f22 2c0a 2020 2020 2020 2020 290a  "No",.        ).
+00014370: 2020 2020 2020 2020 6966 2076 6f69 6365          if voice
+00014380: 5479 7069 6e67 4164 6a75 7374 416d 6269  TypingAdjustAmbi
+00014390: 656e 744e 6f69 7365 3a0a 2020 2020 2020  entNoise:.      
+000143a0: 2020 2020 2020 636f 6e66 6967 2e76 6f69        config.voi
+000143b0: 6365 5479 7069 6e67 4164 6a75 7374 416d  ceTypingAdjustAm
+000143c0: 6269 656e 744e 6f69 7365 203d 2054 7275  bientNoise = Tru
+000143d0: 6520 6966 2076 6f69 6365 5479 7069 6e67  e if voiceTyping
+000143e0: 4164 6a75 7374 416d 6269 656e 744e 6f69  AdjustAmbientNoi
+000143f0: 7365 203d 3d20 2259 6573 2220 656c 7365  se == "Yes" else
+00014400: 2046 616c 7365 0a20 2020 2020 2020 2023   False.        #
+00014410: 2061 7564 696f 206e 6f74 6966 6963 6174   audio notificat
+00014420: 696f 6e0a 2020 2020 2020 2020 766f 6963  ion.        voic
+00014430: 6554 7970 696e 674e 6f74 6966 6963 6174  eTypingNotificat
+00014440: 696f 6e20 3d20 7365 6c66 2e64 6961 6c6f  ion = self.dialo
+00014450: 6773 2e67 6574 5661 6c69 644f 7074 696f  gs.getValidOptio
+00014460: 6e73 280a 2020 2020 2020 2020 2020 2020  ns(.            
+00014470: 6f70 7469 6f6e 733d 2822 5965 7322 2c20  options=("Yes", 
+00014480: 224e 6f22 292c 0a20 2020 2020 2020 2020  "No"),.         
+00014490: 2020 2074 6974 6c65 3d22 4175 6469 6f20     title="Audio 
+000144a0: 4e6f 7469 6669 6361 7469 6f6e 222c 0a20  Notification",. 
+000144b0: 2020 2020 2020 2020 2020 2074 6578 743d             text=
+000144c0: 2244 6f20 796f 7520 7761 6e74 2061 7564  "Do you want aud
+000144d0: 696f 206e 6f74 6966 6963 6174 696f 6e20  io notification 
+000144e0: 7768 656e 2079 6f75 2075 7365 206d 6963  when you use mic
+000144f0: 726f 7068 6f6e 653f 222c 0a20 2020 2020  rophone?",.     
+00014500: 2020 2020 2020 2064 6566 6175 6c74 3d22         default="
+00014510: 5965 7322 2069 6620 636f 6e66 6967 2e76  Yes" if config.v
+00014520: 6f69 6365 5479 7069 6e67 4e6f 7469 6669  oiceTypingNotifi
+00014530: 6361 7469 6f6e 2065 6c73 6520 224e 6f22  cation else "No"
+00014540: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00014550: 2020 2020 6966 2076 6f69 6365 5479 7069      if voiceTypi
+00014560: 6e67 4e6f 7469 6669 6361 7469 6f6e 3a0a  ngNotification:.
+00014570: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+00014580: 6967 2e76 6f69 6365 5479 7069 6e67 4e6f  ig.voiceTypingNo
+00014590: 7469 6669 6361 7469 6f6e 203d 2054 7275  tification = Tru
+000145a0: 6520 6966 2076 6f69 6365 5479 7069 6e67  e if voiceTyping
+000145b0: 4e6f 7469 6669 6361 7469 6f6e 203d 3d20  Notification == 
+000145c0: 2259 6573 2220 656c 7365 2046 616c 7365  "Yes" else False
+000145d0: 0a20 2020 2020 2020 2023 2061 7574 6f20  .        # auto 
+000145e0: 636f 6d70 6c65 7469 6f6e 3a20 766f 6963  completion: voic
+000145f0: 6554 7970 696e 6741 7574 6f43 6f6d 706c  eTypingAutoCompl
+00014600: 6574 650a 2020 2020 2020 2020 766f 6963  ete.        voic
+00014610: 6554 7970 696e 6741 7574 6f43 6f6d 706c  eTypingAutoCompl
+00014620: 6574 6520 3d20 7365 6c66 2e64 6961 6c6f  ete = self.dialo
+00014630: 6773 2e67 6574 5661 6c69 644f 7074 696f  gs.getValidOptio
+00014640: 6e73 280a 2020 2020 2020 2020 2020 2020  ns(.            
+00014650: 6f70 7469 6f6e 733d 2822 5965 7322 2c20  options=("Yes", 
+00014660: 224e 6f22 292c 0a20 2020 2020 2020 2020  "No"),.         
+00014670: 2020 2074 6974 6c65 3d22 4175 6469 6f20     title="Audio 
+00014680: 456e 7472 7920 4175 746f 2043 6f6d 706c  Entry Auto Compl
+00014690: 6574 696f 6e22 2c0a 2020 2020 2020 2020  etion",.        
+000146a0: 2020 2020 7465 7874 3d22 446f 2079 6f75      text="Do you
+000146b0: 2077 616e 7420 746f 2061 7574 6f6d 6174   want to automat
+000146c0: 6963 616c 6c79 2063 6f6d 706c 6574 6520  ically complete 
+000146d0: 796f 7572 2065 6e74 7279 2077 6865 6e20  your entry when 
+000146e0: 6d69 6372 6f70 686f 6e65 2073 746f 7073  microphone stops
+000146f0: 3f22 2c0a 2020 2020 2020 2020 2020 2020  ?",.            
+00014700: 6465 6661 756c 743d 2259 6573 2220 6966  default="Yes" if
+00014710: 2063 6f6e 6669 672e 766f 6963 6554 7970   config.voiceTyp
+00014720: 696e 6741 7574 6f43 6f6d 706c 6574 6520  ingAutoComplete 
+00014730: 656c 7365 2022 4e6f 222c 0a20 2020 2020  else "No",.     
+00014740: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00014750: 766f 6963 6554 7970 696e 6741 7574 6f43  voiceTypingAutoC
+00014760: 6f6d 706c 6574 653a 0a20 2020 2020 2020  omplete:.       
+00014770: 2020 2020 2063 6f6e 6669 672e 766f 6963       config.voic
+00014780: 6554 7970 696e 6741 7574 6f43 6f6d 706c  eTypingAutoCompl
+00014790: 6574 6520 3d20 5472 7565 2069 6620 766f  ete = True if vo
+000147a0: 6963 6554 7970 696e 6741 7574 6f43 6f6d  iceTypingAutoCom
+000147b0: 706c 6574 6520 3d3d 2022 5965 7322 2065  plete == "Yes" e
+000147c0: 6c73 6520 4661 6c73 650a 2020 2020 2020  lse False.      
+000147d0: 2020 2320 6e6f 7469 6679 0a20 2020 2020    # notify.     
+000147e0: 2020 2070 7269 6e74 2822 2229 0a20 2020     print("").   
+000147f0: 2020 2020 2070 7269 6e74 3328 6622 566f       print3(f"Vo
+00014800: 6963 6520 5479 7069 6e67 204d 6f64 656c  ice Typing Model
+00014810: 3a20 7b63 6f6e 6669 672e 766f 6963 6554  : {config.voiceT
+00014820: 7970 696e 6750 6c61 7466 6f72 6d7d 2229  ypingPlatform}")
+00014830: 0a20 2020 2020 2020 2070 7269 6e74 3328  .        print3(
+00014840: 6622 566f 6963 6520 5479 7069 6e67 204c  f"Voice Typing L
+00014850: 616e 6775 6167 653a 207b 636f 6e66 6967  anguage: {config
+00014860: 2e76 6f69 6365 5479 7069 6e67 4c61 6e67  .voiceTypingLang
+00014870: 7561 6765 7d22 290a 2020 2020 2020 2020  uage}").        
+00014880: 7072 696e 7433 2866 2241 6d62 6965 6e74  print3(f"Ambient
+00014890: 204e 6f69 7365 2041 646a 7573 746d 656e   Noise Adjustmen
+000148a0: 743a 207b 636f 6e66 6967 2e76 6f69 6365  t: {config.voice
+000148b0: 5479 7069 6e67 4164 6a75 7374 416d 6269  TypingAdjustAmbi
+000148c0: 656e 744e 6f69 7365 7d22 290a 2020 2020  entNoise}").    
+000148d0: 2020 2020 7072 696e 7433 2866 2241 7564      print3(f"Aud
+000148e0: 696f 204e 6f74 6966 6963 6174 696f 6e3a  io Notification:
+000148f0: 207b 636f 6e66 6967 2e76 6f69 6365 5479   {config.voiceTy
+00014900: 7069 6e67 4e6f 7469 6669 6361 7469 6f6e  pingNotification
+00014910: 7d22 290a 2020 2020 2020 2020 7072 696e  }").        prin
+00014920: 7433 2866 2241 7574 6f20 436f 6d70 6c65  t3(f"Auto Comple
+00014930: 7469 6f6e 3a20 7b63 6f6e 6669 672e 766f  tion: {config.vo
+00014940: 6963 6554 7970 696e 6741 7574 6f43 6f6d  iceTypingAutoCom
+00014950: 706c 6574 657d 2229 0a20 2020 2020 2020  plete}").       
+00014960: 2023 2073 6176 6520 636f 6e66 6967 730a   # save configs.
+00014970: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
+00014980: 6176 6543 6f6e 6669 6728 290a 0a20 2020  aveConfig()..   
+00014990: 2064 6566 2073 6176 6543 6861 7428 7365   def saveChat(se
+000149a0: 6c66 2c20 6d65 7373 6167 6573 293a 0a20  lf, messages):. 
+000149b0: 2020 2020 2020 206d 6573 7361 6765 7343         messagesC
+000149c0: 6f70 7920 3d20 636f 7079 2e64 6565 7063  opy = copy.deepc
+000149d0: 6f70 7928 6d65 7373 6167 6573 290a 0a20  opy(messages).. 
+000149e0: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
+000149f0: 2e63 6f6e 7665 7273 6174 696f 6e53 7461  .conversationSta
+00014a00: 7274 6564 3a0a 2020 2020 2020 2020 2020  rted:.          
+00014a10: 2020 7469 6d65 7374 616d 7020 3d20 6765    timestamp = ge
+00014a20: 7443 7572 7265 6e74 4461 7465 5469 6d65  tCurrentDateTime
+00014a30: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00014a40: 6966 2068 6173 6174 7472 2863 6f6e 6669  if hasattr(confi
+00014a50: 672c 2022 7361 7665 5f63 6861 745f 7265  g, "save_chat_re
+00014a60: 636f 7264 2229 3a0a 2020 2020 2020 2020  cord"):.        
+00014a70: 2020 2020 2020 2020 2320 7768 656e 2070          # when p
+00014a80: 6c75 6769 6e20 2273 6176 6520 6368 6174  lugin "save chat
+00014a90: 2072 6563 6f72 6473 2220 6973 2065 6e61   records" is ena
+00014aa0: 626c 6564 0a20 2020 2020 2020 2020 2020  bled.           
+00014ab0: 2020 2020 206d 6573 7361 6765 4c65 6e67       messageLeng
+00014ac0: 7468 203d 206c 656e 286d 6573 7361 6765  th = len(message
+00014ad0: 7343 6f70 7929 0a20 2020 2020 2020 2020  sCopy).         
+00014ae0: 2020 2020 2020 2066 6f72 206f 7264 6572         for order
+00014af0: 2c20 6920 696e 2065 6e75 6d65 7261 7465  , i in enumerate
+00014b00: 286d 6573 7361 6765 7343 6f70 7929 3a0a  (messagesCopy):.
+00014b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b20: 2020 2020 6973 4c61 7374 4974 656d 203d      isLastItem =
+00014b30: 2028 6f72 6465 7220 3d3d 2028 6d65 7373   (order == (mess
+00014b40: 6167 654c 656e 6774 6820 2d20 3129 290a  ageLength - 1)).
+00014b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b60: 2020 2020 6966 2063 6f6e 6669 672e 6c6c      if config.ll
+00014b70: 6d49 6e74 6572 6661 6365 2069 6e20 2822  mInterface in ("
+00014b80: 6368 6174 6770 7422 2c20 226c 6574 6d65  chatgpt", "letme
+00014b90: 646f 6974 222c 2022 6772 6f71 2229 2061  doit", "groq") a
+00014ba0: 6e64 206e 6f74 2069 734c 6173 7449 7465  nd not isLastIte
+00014bb0: 6d20 616e 6420 692e 6765 7428 2272 6f6c  m and i.get("rol
+00014bc0: 6522 2c20 2222 2920 3d3d 2022 7573 6572  e", "") == "user
+00014bd0: 2220 616e 6420 2266 756e 6374 696f 6e5f  " and "function_
+00014be0: 6361 6c6c 2220 696e 206d 6573 7361 6765  call" in message
+00014bf0: 7343 6f70 795b 6f72 6465 722b 315d 3a0a  sCopy[order+1]:.
+00014c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c10: 2020 2020 2020 2020 695b 2274 6f6f 6c22          i["tool"
+00014c20: 5d20 3d20 6d65 7373 6167 6573 436f 7079  ] = messagesCopy
+00014c30: 5b6f 7264 6572 2b31 5d5b 2266 756e 6374  [order+1]["funct
+00014c40: 696f 6e5f 6361 6c6c 225d 2e67 6574 2822  ion_call"].get("
+00014c50: 6e61 6d65 222c 2022 2229 0a20 2020 2020  name", "").     
+00014c60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00014c70: 6f6e 6669 672e 7361 7665 5f63 6861 745f  onfig.save_chat_
+00014c80: 7265 636f 7264 2874 696d 6573 7461 6d70  record(timestamp
+00014c90: 2c20 6f72 6465 722c 2069 290a 0a20 2020  , order, i)..   
+00014ca0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00014cb0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00014cc0: 6c64 6572 5061 7468 203d 206f 732e 7061  lderPath = os.pa
+00014cd0: 7468 2e6a 6f69 6e28 636f 6e66 6967 2e6c  th.join(config.l
+00014ce0: 6f63 616c 5374 6f72 6167 652c 2022 6368  ocalStorage, "ch
+00014cf0: 6174 7322 2c20 7265 2e73 7562 2822 5e28  ats", re.sub("^(
+00014d00: 5b30 2d39 5d2b 3f5c 2d5b 302d 395d 2b3f  [0-9]+?\-[0-9]+?
+00014d10: 295c 2d2e 2a3f 2422 2c20 7222 5c31 222c  )\-.*?$", r"\1",
+00014d20: 2074 696d 6573 7461 6d70 2929 0a20 2020   timestamp)).   
+00014d30: 2020 2020 2020 2020 2020 2020 2050 6174               Pat
+00014d40: 6828 666f 6c64 6572 5061 7468 292e 6d6b  h(folderPath).mk
+00014d50: 6469 7228 7061 7265 6e74 733d 5472 7565  dir(parents=True
+00014d60: 2c20 6578 6973 745f 6f6b 3d54 7275 6529  , exist_ok=True)
+00014d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014d80: 2069 6620 6f73 2e70 6174 682e 6973 6469   if os.path.isdi
+00014d90: 7228 666f 6c64 6572 5061 7468 293a 0a20  r(folderPath):. 
+00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014db0: 2020 2063 6861 7446 696c 6520 3d20 6f73     chatFile = os
+00014dc0: 2e70 6174 682e 6a6f 696e 2866 6f6c 6465  .path.join(folde
+00014dd0: 7250 6174 682c 2066 227b 7469 6d65 7374  rPath, f"{timest
+00014de0: 616d 707d 2e74 7874 2229 0a20 2020 2020  amp}.txt").     
+00014df0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00014e00: 6974 6820 6f70 656e 2863 6861 7446 696c  ith open(chatFil
+00014e10: 652c 2022 7722 2c20 656e 636f 6469 6e67  e, "w", encoding
+00014e20: 3d22 7574 662d 3822 2920 6173 2066 696c  ="utf-8") as fil
+00014e30: 654f 626a 3a0a 2020 2020 2020 2020 2020  eObj:.          
+00014e40: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00014e50: 6c65 4f62 6a2e 7772 6974 6528 7070 7269  leObj.write(ppri
+00014e60: 6e74 2e70 666f 726d 6174 286d 6573 7361  nt.pformat(messa
+00014e70: 6765 7343 6f70 7929 290a 2020 2020 2020  gesCopy)).      
+00014e80: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00014e90: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00014ea0: 696e 7432 2822 4661 696c 6564 2074 6f20  int2("Failed to 
+00014eb0: 7361 7665 2063 6861 7421 5c6e 2229 0a20  save chat!\n"). 
+00014ec0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014ed0: 686f 7745 7272 6f72 7328 290a 0a20 2020  howErrors()..   
+00014ee0: 2064 6566 2065 7870 6f72 7443 6861 7428   def exportChat(
+00014ef0: 7365 6c66 2c20 6d65 7373 6167 6573 2c20  self, messages, 
+00014f00: 6f70 656e 4669 6c65 3d54 7275 6529 3a0a  openFile=True):.
+00014f10: 2020 2020 2020 2020 6966 2063 6f6e 6669          if confi
+00014f20: 672e 636f 6e76 6572 7361 7469 6f6e 5374  g.conversationSt
+00014f30: 6172 7465 643a 0a20 2020 2020 2020 2020  arted:.         
+00014f40: 2020 2070 6c61 696e 5465 7874 203d 2022     plainText = "
+00014f50: 220a 2020 2020 2020 2020 2020 2020 7469  ".            ti
+00014f60: 6d65 7374 616d 7020 3d20 6765 7443 7572  mestamp = getCur
+00014f70: 7265 6e74 4461 7465 5469 6d65 2829 0a0a  rentDateTime()..
+00014f80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00014f90: 6920 696e 206d 6573 7361 6765 733a 0a20  i in messages:. 
+00014fa0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014fb0: 6620 695b 2272 6f6c 6522 5d20 3d3d 2022  f i["role"] == "
+00014fc0: 7573 6572 223a 0a20 2020 2020 2020 2020  user":.         
+00014fd0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00014fe0: 6e74 203d 2069 5b22 636f 6e74 656e 7422  nt = i["content"
+00014ff0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00015000: 2020 2020 2020 706c 6169 6e54 6578 7420        plainText 
+00015010: 2b3d 2066 223e 3e3e 207b 636f 6e74 656e  += f">>> {conten
+00015020: 747d 220a 2020 2020 2020 2020 2020 2020  t}".            
+00015030: 2020 2020 6966 2069 5b22 726f 6c65 225d      if i["role"]
+00015040: 203d 3d20 2266 756e 6374 696f 6e22 3a0a   == "function":.
+00015050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015060: 2020 2020 6966 2070 6c61 696e 5465 7874      if plainText
+00015070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015080: 2020 2020 2020 2020 2020 706c 6169 6e54            plainT
+00015090: 6578 7420 2b3d 2022 5c6e 5c6e 220a 2020  ext += "\n\n".  
+000150a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150b0: 2020 6e61 6d65 203d 2069 5b22 6e61 6d65    name = i["name
+000150c0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+000150d0: 2020 2020 2020 2070 6c61 696e 5465 7874         plainText
+000150e0: 202b 3d20 6622 6060 605c 6e7b 6e61 6d65   += f"```\n{name
+000150f0: 7d5c 6e60 6060 220a 2020 2020 2020 2020  }\n```".        
+00015100: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00015110: 656e 7420 3d20 695b 2263 6f6e 7465 6e74  ent = i["content
+00015120: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00015130: 2020 2020 2020 2070 6c61 696e 5465 7874         plainText
+00015140: 202b 3d20 6622 5c6e 5c6e 7b63 6f6e 7465   += f"\n\n{conte
+00015150: 6e74 7d5c 6e5c 6e22 0a20 2020 2020 2020  nt}\n\n".       
+00015160: 2020 2020 2020 2020 2065 6c69 6620 695b           elif i[
+00015170: 2272 6f6c 6522 5d20 3d3d 2022 6173 7369  "role"] == "assi
+00015180: 7374 616e 7422 3a0a 2020 2020 2020 2020  stant":.        
+00015190: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000151a0: 656e 7420 3d20 695b 2263 6f6e 7465 6e74  ent = i["content
+000151b0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+000151c0: 2020 2020 2020 2069 6620 636f 6e74 656e         if conten
+000151d0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+000151e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151f0: 2020 2020 2020 2069 6620 706c 6169 6e54         if plainT
+00015200: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
 00015210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015220: 2020 2020 2020 2070 6c61 696e 5465 7874         plainText
-00015230: 202b 3d20 225c 6e5c 6e22 0a20 2020 2020   += "\n\n".     
-00015240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015250: 2020 2070 6c61 696e 5465 7874 202b 3d20     plainText += 
-00015260: 6622 7b63 6f6e 7465 6e74 7d5c 6e5c 6e22  f"{content}\n\n"
-00015270: 0a20 2020 2020 2020 2020 2020 2070 6c61  .            pla
-00015280: 696e 5465 7874 203d 2070 6c61 696e 5465  inText = plainTe
-00015290: 7874 2e73 7472 6970 2829 0a20 2020 2020  xt.strip().     
-000152a0: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
-000152b0: 2e74 6572 6d69 6e61 6c45 6e61 626c 6554  .terminalEnableT
-000152c0: 6572 6d75 7841 5049 3a0a 2020 2020 2020  ermuxAPI:.      
-000152d0: 2020 2020 2020 2020 2020 7079 646f 632e            pydoc.
-000152e0: 7069 7065 7061 6765 7228 706c 6169 6e54  pipepager(plainT
-000152f0: 6578 742c 2063 6d64 3d22 7465 726d 7578  ext, cmd="termux
-00015300: 2d73 6861 7265 202d 6120 7365 6e64 2229  -share -a send")
-00015310: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00015320: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00015330: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00015340: 2020 2020 2020 2020 2020 2020 666f 6c64              fold
-00015350: 6572 5061 7468 203d 206f 732e 7061 7468  erPath = os.path
-00015360: 2e6a 6f69 6e28 636f 6e66 6967 2e6c 6f63  .join(config.loc
-00015370: 616c 5374 6f72 6167 652c 2022 6368 6174  alStorage, "chat
-00015380: 7322 2c20 2265 7870 6f72 7422 290a 2020  s", "export").  
-00015390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153a0: 2020 5061 7468 2866 6f6c 6465 7250 6174    Path(folderPat
-000153b0: 6829 2e6d 6b64 6972 2870 6172 656e 7473  h).mkdir(parents
-000153c0: 3d54 7275 652c 2065 7869 7374 5f6f 6b3d  =True, exist_ok=
-000153d0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-000153e0: 2020 2020 2020 2020 2020 6966 206f 732e            if os.
-000153f0: 7061 7468 2e69 7364 6972 2866 6f6c 6465  path.isdir(folde
-00015400: 7250 6174 6829 3a0a 2020 2020 2020 2020  rPath):.        
-00015410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015420: 6368 6174 4669 6c65 203d 206f 732e 7061  chatFile = os.pa
-00015430: 7468 2e6a 6f69 6e28 666f 6c64 6572 5061  th.join(folderPa
-00015440: 7468 2c20 6622 7b74 696d 6573 7461 6d70  th, f"{timestamp
-00015450: 7d2e 7478 7422 290a 2020 2020 2020 2020  }.txt").        
-00015460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015470: 7769 7468 206f 7065 6e28 6368 6174 4669  with open(chatFi
-00015480: 6c65 2c20 2277 222c 2065 6e63 6f64 696e  le, "w", encodin
-00015490: 673d 2275 7466 2d38 2229 2061 7320 6669  g="utf-8") as fi
-000154a0: 6c65 4f62 6a3a 0a20 2020 2020 2020 2020  leObj:.         
-000154b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154c0: 2020 2066 696c 654f 626a 2e77 7269 7465     fileObj.write
-000154d0: 2870 6c61 696e 5465 7874 290a 2020 2020  (plainText).    
-000154e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154f0: 2020 2020 6966 206f 7065 6e46 696c 6520      if openFile 
-00015500: 616e 6420 6f73 2e70 6174 682e 6973 6669  and os.path.isfi
-00015510: 6c65 2863 6861 7446 696c 6529 3a0a 2020  le(chatFile):.  
+00015220: 2070 6c61 696e 5465 7874 202b 3d20 225c   plainText += "\
+00015230: 6e5c 6e22 0a20 2020 2020 2020 2020 2020  n\n".           
+00015240: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00015250: 696e 5465 7874 202b 3d20 6622 7b63 6f6e  inText += f"{con
+00015260: 7465 6e74 7d5c 6e5c 6e22 0a20 2020 2020  tent}\n\n".     
+00015270: 2020 2020 2020 2070 6c61 696e 5465 7874         plainText
+00015280: 203d 2070 6c61 696e 5465 7874 2e73 7472   = plainText.str
+00015290: 6970 2829 0a20 2020 2020 2020 2020 2020  ip().           
+000152a0: 2069 6620 636f 6e66 6967 2e74 6572 6d69   if config.termi
+000152b0: 6e61 6c45 6e61 626c 6554 6572 6d75 7841  nalEnableTermuxA
+000152c0: 5049 3a0a 2020 2020 2020 2020 2020 2020  PI:.            
+000152d0: 2020 2020 7079 646f 632e 7069 7065 7061      pydoc.pipepa
+000152e0: 6765 7228 706c 6169 6e54 6578 742c 2063  ger(plainText, c
+000152f0: 6d64 3d22 7465 726d 7578 2d73 6861 7265  md="termux-share
+00015300: 202d 6120 7365 6e64 2229 0a20 2020 2020   -a send").     
+00015310: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00015320: 2020 2020 2020 2020 2020 2020 2074 7279               try
+00015330: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015340: 2020 2020 2020 666f 6c64 6572 5061 7468        folderPath
+00015350: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00015360: 636f 6e66 6967 2e6c 6f63 616c 5374 6f72  config.localStor
+00015370: 6167 652c 2022 6368 6174 7322 2c20 2265  age, "chats", "e
+00015380: 7870 6f72 7422 290a 2020 2020 2020 2020  xport").        
+00015390: 2020 2020 2020 2020 2020 2020 5061 7468              Path
+000153a0: 2866 6f6c 6465 7250 6174 6829 2e6d 6b64  (folderPath).mkd
+000153b0: 6972 2870 6172 656e 7473 3d54 7275 652c  ir(parents=True,
+000153c0: 2065 7869 7374 5f6f 6b3d 5472 7565 290a   exist_ok=True).
+000153d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153e0: 2020 2020 6966 206f 732e 7061 7468 2e69      if os.path.i
+000153f0: 7364 6972 2866 6f6c 6465 7250 6174 6829  sdir(folderPath)
+00015400: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015410: 2020 2020 2020 2020 2020 6368 6174 4669            chatFi
+00015420: 6c65 203d 206f 732e 7061 7468 2e6a 6f69  le = os.path.joi
+00015430: 6e28 666f 6c64 6572 5061 7468 2c20 6622  n(folderPath, f"
+00015440: 7b74 696d 6573 7461 6d70 7d2e 7478 7422  {timestamp}.txt"
+00015450: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015460: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+00015470: 7065 6e28 6368 6174 4669 6c65 2c20 2277  pen(chatFile, "w
+00015480: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+00015490: 2d38 2229 2061 7320 6669 6c65 4f62 6a3a  -8") as fileObj:
+000154a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000154b0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+000154c0: 654f 626a 2e77 7269 7465 2870 6c61 696e  eObj.write(plain
+000154d0: 5465 7874 290a 2020 2020 2020 2020 2020  Text).          
+000154e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000154f0: 206f 7065 6e46 696c 6520 616e 6420 6f73   openFile and os
+00015500: 2e70 6174 682e 6973 6669 6c65 2863 6861  .path.isfile(cha
+00015510: 7446 696c 6529 3a0a 2020 2020 2020 2020  tFile):.        
 00015520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015530: 2020 2020 2020 2020 2020 6f73 2e73 7973            os.sys
-00015540: 7465 6d28 6627 2727 7b63 6f6e 6669 672e  tem(f'''{config.
-00015550: 6f70 656e 7d20 227b 6368 6174 4669 6c65  open} "{chatFile
-00015560: 7d22 2727 2729 0a20 2020 2020 2020 2020  }"''').         
-00015570: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
-00015580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015590: 2020 2070 7269 6e74 3228 2246 6169 6c65     print2("Faile
-000155a0: 6420 746f 2073 6176 6520 6368 6174 215c  d to save chat!\
-000155b0: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
-000155c0: 2020 2020 2020 2020 7368 6f77 4572 726f          showErro
-000155d0: 7273 2829 0a0a 2020 2020 6465 6620 7275  rs()..    def ru
-000155e0: 6e49 6e73 7472 7563 7469 6f6e 2873 656c  nInstruction(sel
-000155f0: 6629 3a0a 2020 2020 2020 2020 696e 7374  f):.        inst
-00015600: 7275 6374 696f 6e73 203d 206c 6973 7428  ructions = list(
-00015610: 636f 6e66 6967 2e70 7265 6465 6669 6e65  config.predefine
-00015620: 6449 6e73 7472 7563 7469 6f6e 732e 6b65  dInstructions.ke
-00015630: 7973 2829 290a 2020 2020 2020 2020 696e  ys()).        in
-00015640: 7374 7275 6374 696f 6e20 3d20 7365 6c66  struction = self
-00015650: 2e64 6961 6c6f 6773 2e67 6574 5661 6c69  .dialogs.getVali
-00015660: 644f 7074 696f 6e73 280a 2020 2020 2020  dOptions(.      
-00015670: 2020 2020 2020 6f70 7469 6f6e 733d 696e        options=in
-00015680: 7374 7275 6374 696f 6e73 2c0a 2020 2020  structions,.    
-00015690: 2020 2020 2020 2020 7469 746c 653d 2250          title="P
-000156a0: 7265 6465 6669 6e65 6420 496e 7374 7275  redefined Instru
-000156b0: 6374 696f 6e73 222c 0a20 2020 2020 2020  ctions",.       
-000156c0: 2020 2020 2074 6578 743d 2253 656c 6563       text="Selec
-000156d0: 7420 616e 2069 6e73 7472 7563 7469 6f6e  t an instruction
-000156e0: 3a22 2c0a 2020 2020 2020 2020 290a 2020  :",.        ).  
-000156f0: 2020 2020 2020 6966 2069 6e73 7472 7563        if instruc
-00015700: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-00015710: 2020 636f 6e66 6967 2e64 6566 6175 6c74    config.default
-00015720: 456e 7472 7920 3d20 636f 6e66 6967 2e70  Entry = config.p
-00015730: 7265 6465 6669 6e65 6449 6e73 7472 7563  redefinedInstruc
-00015740: 7469 6f6e 735b 696e 7374 7275 6374 696f  tions[instructio
-00015750: 6e5d 0a20 2020 2020 2020 2020 2020 2063  n].            c
-00015760: 6f6e 6669 672e 6163 6365 7074 5f64 6566  onfig.accept_def
-00015770: 6175 6c74 203d 2054 7275 650a 0a20 2020  ault = True..   
-00015780: 2064 6566 2063 6861 6e67 6543 6f6e 7465   def changeConte
-00015790: 7874 2873 656c 6629 3a0a 2020 2020 2020  xt(self):.      
-000157a0: 2020 636f 6e74 6578 7473 203d 206c 6973    contexts = lis
-000157b0: 7428 636f 6e66 6967 2e70 7265 6465 6669  t(config.predefi
-000157c0: 6e65 6443 6f6e 7465 7874 732e 6b65 7973  nedContexts.keys
-000157d0: 2829 290a 2020 2020 2020 2020 7072 6564  ()).        pred
-000157e0: 6566 696e 6564 436f 6e74 6578 7420 3d20  efinedContext = 
-000157f0: 7365 6c66 2e64 6961 6c6f 6773 2e67 6574  self.dialogs.get
-00015800: 5661 6c69 644f 7074 696f 6e73 280a 2020  ValidOptions(.  
-00015810: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-00015820: 733d 636f 6e74 6578 7473 2c0a 2020 2020  s=contexts,.    
-00015830: 2020 2020 2020 2020 7469 746c 653d 2250          title="P
-00015840: 7265 6465 6669 6e65 6420 436f 6e74 6578  redefined Contex
-00015850: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
-00015860: 2064 6566 6175 6c74 3d63 6f6e 6669 672e   default=config.
-00015870: 7072 6564 6566 696e 6564 436f 6e74 6578  predefinedContex
-00015880: 742c 0a20 2020 2020 2020 2020 2020 2074  t,.            t
-00015890: 6578 743d 2253 656c 6563 7420 6120 636f  ext="Select a co
-000158a0: 6e74 6578 743a 222c 0a20 2020 2020 2020  ntext:",.       
-000158b0: 2029 0a20 2020 2020 2020 2069 6620 7072   ).        if pr
-000158c0: 6564 6566 696e 6564 436f 6e74 6578 743a  edefinedContext:
-000158d0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-000158e0: 6669 672e 7072 6564 6566 696e 6564 436f  fig.predefinedCo
-000158f0: 6e74 6578 7420 3d20 7072 6564 6566 696e  ntext = predefin
-00015900: 6564 436f 6e74 6578 740a 2020 2020 2020  edContext.      
-00015910: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
-00015920: 7072 6564 6566 696e 6564 436f 6e74 6578  predefinedContex
-00015930: 7420 3d3d 2022 5b63 7573 746f 6d5d 223a  t == "[custom]":
-00015940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015950: 2070 7269 6e74 3128 2245 6469 7420 6375   print1("Edit cu
-00015960: 7374 6f6d 2063 6f6e 7465 7874 2062 656c  stom context bel
-00015970: 6f77 3a22 290a 2020 2020 2020 2020 2020  ow:").          
-00015980: 2020 2020 2020 6375 7374 6f6d 436f 6e74        customCont
-00015990: 6578 7420 3d20 7365 6c66 2e70 726f 6d70  ext = self.promp
-000159a0: 7473 2e73 696d 706c 6550 726f 6d70 7428  ts.simplePrompt(
-000159b0: 7374 796c 653d 7365 6c66 2e70 726f 6d70  style=self.promp
-000159c0: 7473 2e70 726f 6d70 7453 7479 6c65 322c  ts.promptStyle2,
-000159d0: 2064 6566 6175 6c74 3d63 6f6e 6669 672e   default=config.
-000159e0: 6375 7374 6f6d 5072 6564 6566 696e 6564  customPredefined
-000159f0: 436f 6e74 6578 7429 0a20 2020 2020 2020  Context).       
-00015a00: 2020 2020 2020 2020 2069 6620 6375 7374           if cust
-00015a10: 6f6d 436f 6e74 6578 7420 616e 6420 6e6f  omContext and no
-00015a20: 7420 6375 7374 6f6d 436f 6e74 6578 742e  t customContext.
-00015a30: 7374 7269 7028 292e 6c6f 7765 7228 2920  strip().lower() 
-00015a40: 3d3d 2063 6f6e 6669 672e 6578 6974 5f65  == config.exit_e
-00015a50: 6e74 7279 3a0a 2020 2020 2020 2020 2020  ntry:.          
-00015a60: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-00015a70: 2e63 7573 746f 6d50 7265 6465 6669 6e65  .customPredefine
-00015a80: 6443 6f6e 7465 7874 203d 2063 7573 746f  dContext = custo
-00015a90: 6d43 6f6e 7465 7874 2e73 7472 6970 2829  mContext.strip()
-00015aa0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00015ab0: 2020 2020 2020 2020 2020 2023 2061 2077             # a w
-00015ac0: 6179 2074 6f20 7175 6963 6b6c 7920 636c  ay to quickly cl
-00015ad0: 6561 6e20 7570 2063 6f6e 7465 7874 0a20  ean up context. 
-00015ae0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00015af0: 672e 7072 6564 6566 696e 6564 436f 6e74  g.predefinedCont
-00015b00: 6578 7420 3d20 225b 6e6f 6e65 5d22 0a20  ext = "[none]". 
-00015b10: 2020 2020 2020 2063 6f6e 6669 672e 7361         config.sa
-00015b20: 7665 436f 6e66 6967 2829 0a20 2020 2020  veConfig().     
-00015b30: 2020 2073 656c 662e 7368 6f77 4375 7272     self.showCurr
-00015b40: 656e 7443 6f6e 7465 7874 2829 0a0a 2020  entContext()..  
-00015b50: 2020 6465 6620 6765 7444 6972 6563 746f    def getDirecto
-00015b60: 7279 4c69 7374 2873 656c 6629 3a0a 2020  ryList(self):.  
-00015b70: 2020 2020 2020 6469 7265 6374 6f72 794c        directoryL
-00015b80: 6973 7420 3d20 5b5d 0a20 2020 2020 2020  ist = [].       
-00015b90: 2066 6f72 2066 2069 6e20 6f73 2e6c 6973   for f in os.lis
-00015ba0: 7464 6972 2827 2e27 293a 0a20 2020 2020  tdir('.'):.     
-00015bb0: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-00015bc0: 682e 6973 6469 7228 6629 3a0a 2020 2020  h.isdir(f):.    
-00015bd0: 2020 2020 2020 2020 2020 2020 7365 7061              sepa
-00015be0: 7261 746f 7220 3d20 225c 5c22 2069 6620  rator = "\\" if 
-00015bf0: 636f 6e66 6967 2e74 6869 7350 6c61 7466  config.thisPlatf
-00015c00: 6f72 6d20 3d3d 2022 5769 6e64 6f77 7322  orm == "Windows"
-00015c10: 2065 6c73 6520 222f 220a 2020 2020 2020   else "/".      
-00015c20: 2020 2020 2020 2020 2020 6469 7265 6374            direct
-00015c30: 6f72 794c 6973 742e 6170 7065 6e64 2866  oryList.append(f
-00015c40: 227b 667d 7b73 6570 6172 6174 6f72 7d22  "{f}{separator}"
-00015c50: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00015c60: 6966 206f 732e 7061 7468 2e69 7366 696c  if os.path.isfil
-00015c70: 6528 6629 3a0a 2020 2020 2020 2020 2020  e(f):.          
-00015c80: 2020 2020 2020 6469 7265 6374 6f72 794c        directoryL
-00015c90: 6973 742e 6170 7065 6e64 2866 290a 2020  ist.append(f).  
-00015ca0: 2020 2020 2020 7265 7475 726e 2064 6972        return dir
-00015cb0: 6563 746f 7279 4c69 7374 0a0a 2020 2020  ectoryList..    
-00015cc0: 6465 6620 7368 6f77 4c6f 676f 2873 656c  def showLogo(sel
-00015cd0: 6629 3a0a 2020 2020 2020 2020 6170 704e  f):.        appN
-00015ce0: 616d 6520 3d20 636f 6e66 6967 2e66 7265  ame = config.fre
-00015cf0: 6547 656e 6975 7341 494e 616d 652e 7370  eGeniusAIName.sp
-00015d00: 6c69 7428 295b 305d 2e75 7070 6572 2829  lit()[0].upper()
-00015d10: 0a20 2020 2020 2020 2074 6572 6d69 6e61  .        termina
-00015d20: 6c5f 7769 6474 6820 3d20 7368 7574 696c  l_width = shutil
-00015d30: 2e67 6574 5f74 6572 6d69 6e61 6c5f 7369  .get_terminal_si
-00015d40: 7a65 2829 2e63 6f6c 756d 6e73 0a20 2020  ze().columns.   
-00015d50: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00015d60: 2020 2020 2020 6672 6f6d 2061 7274 2069        from art i
-00015d70: 6d70 6f72 7420 7465 7874 3261 7274 0a20  mport text2art. 
-00015d80: 2020 2020 2020 2020 2020 2069 6620 7465             if te
-00015d90: 726d 696e 616c 5f77 6964 7468 203e 3d20  rminal_width >= 
-00015da0: 3332 3a0a 2020 2020 2020 2020 2020 2020  32:.            
-00015db0: 2020 2020 6c6f 676f 203d 2074 6578 7432      logo = text2
-00015dc0: 6172 7428 6170 704e 616d 652c 2066 6f6e  art(appName, fon
-00015dd0: 743d 2263 7962 6572 6d65 6475 6d22 290a  t="cybermedum").
-00015de0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00015df0: 2074 6572 6d69 6e61 6c5f 7769 6474 6820   terminal_width 
-00015e00: 3e3d 2032 303a 0a20 2020 2020 2020 2020  >= 20:.         
-00015e10: 2020 2020 2020 206c 6f67 6f20 3d20 7465         logo = te
-00015e20: 7874 3261 7274 2822 2022 2e6a 6f69 6e28  xt2art(" ".join(
-00015e30: 6170 704e 616d 6529 202b 2022 2022 2c20  appName) + " ", 
-00015e40: 666f 6e74 3d22 7768 6974 655f 6275 6262  font="white_bubb
-00015e50: 6c65 2229 0a20 2020 2020 2020 2020 2020  le").           
-00015e60: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00015e70: 2020 2020 2020 206c 6f67 6f20 3d20 636f         logo = co
-00015e80: 6e66 6967 2e66 7265 6547 656e 6975 7341  nfig.freeGeniusA
-00015e90: 494e 616d 650a 2020 2020 2020 2020 2020  IName.          
-00015ea0: 2020 6c6f 676f 203d 206c 6f67 6f5b 3a2d    logo = logo[:-
-00015eb0: 315d 2023 2072 656d 6f76 6520 7468 6520  1] # remove the 
-00015ec0: 6c69 6e65 6272 6561 6b20 6174 2074 6865  linebreak at the
-00015ed0: 2065 6e64 0a20 2020 2020 2020 2065 7863   end.        exc
-00015ee0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-00015ef0: 206c 6f67 6f20 3d20 636f 6e66 6967 2e66   logo = config.f
-00015f00: 7265 6547 656e 6975 7341 494e 616d 650a  reeGeniusAIName.
-00015f10: 2020 2020 2020 2020 7072 696e 745f 666f          print_fo
-00015f20: 726d 6174 7465 645f 7465 7874 2848 544d  rmatted_text(HTM
-00015f30: 4c28 6622 3c7b 636f 6e66 6967 2e74 6572  L(f"<{config.ter
-00015f40: 6d69 6e61 6c43 6f6d 6d61 6e64 456e 7472  minalCommandEntr
-00015f50: 7943 6f6c 6f72 327d 3e7b 6c6f 676f 7d3c  yColor2}>{logo}<
-00015f60: 2f7b 636f 6e66 6967 2e74 6572 6d69 6e61  /{config.termina
-00015f70: 6c43 6f6d 6d61 6e64 456e 7472 7943 6f6c  lCommandEntryCol
-00015f80: 6f72 327d 3e22 2929 0a0a 2020 2020 6465  or2}>"))..    de
-00015f90: 6620 7275 6e50 7974 686f 6e53 6372 6970  f runPythonScrip
-00015fa0: 7428 7365 6c66 2c20 7363 7269 7074 293a  t(self, script):
-00015fb0: 0a20 2020 2020 2020 2073 6372 6970 7420  .        script 
-00015fc0: 3d20 7363 7269 7074 2e73 7472 6970 2829  = script.strip()
-00015fd0: 5b33 3a2d 335d 0a20 2020 2020 2020 2074  [3:-3].        t
-00015fe0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00015ff0: 6578 6563 2873 6372 6970 742c 2067 6c6f  exec(script, glo
-00016000: 6261 6c73 2829 290a 2020 2020 2020 2020  bals()).        
-00016010: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00016020: 2020 2020 7472 6163 6520 3d20 7472 6163      trace = trac
-00016030: 6562 6163 6b2e 666f 726d 6174 5f65 7863  eback.format_exc
-00016040: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
-00016050: 7269 6e74 2874 7261 6365 2069 6620 636f  rint(trace if co
-00016060: 6e66 6967 2e64 6576 656c 6f70 6572 2065  nfig.developer e
-00016070: 6c73 6520 2245 7272 6f72 2065 6e63 6f75  lse "Error encou
-00016080: 6e74 6572 6564 2122 290a 2020 2020 2020  ntered!").      
-00016090: 2020 2020 2020 7072 696e 7431 2863 6f6e        print1(con
-000160a0: 6669 672e 6469 7669 6465 7229 0a20 2020  fig.divider).   
-000160b0: 2020 2020 2020 2020 2069 6620 636f 6e66           if conf
-000160c0: 6967 2e6d 6178 5f63 6f6e 7365 6375 7469  ig.max_consecuti
-000160d0: 7665 5f61 7574 6f5f 636f 7272 6563 7469  ve_auto_correcti
-000160e0: 6f6e 203e 2030 3a0a 2020 2020 2020 2020  on > 0:.        
-000160f0: 2020 2020 2020 2020 4361 6c6c 4c4c 4d2e          CallLLM.
-00016100: 6175 746f 436f 7272 6563 7450 7974 686f  autoCorrectPytho
-00016110: 6e43 6f64 6528 7363 7269 7074 2c20 7472  nCode(script, tr
-00016120: 6163 6529 0a0a 2020 2020 6465 6620 7374  ace)..    def st
-00016130: 6172 7443 6861 7473 2873 656c 6629 3a0a  artChats(self):.
-00016140: 2020 2020 2020 2020 746f 6b65 6e56 616c          tokenVal
-00016150: 6964 6174 6f72 203d 2054 6f6b 656e 5661  idator = TokenVa
-00016160: 6c69 6461 746f 7228 290a 2020 2020 2020  lidator().      
-00016170: 2020 6465 6620 6765 7444 796e 616d 6963    def getDynamic
-00016180: 546f 6f6c 4261 7228 293a 0a20 2020 2020  ToolBar():.     
-00016190: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
-000161a0: 6e66 6967 2e64 796e 616d 6963 546f 6f6c  nfig.dynamicTool
-000161b0: 4261 7254 6578 740a 2020 2020 2020 2020  BarText.        
-000161c0: 6465 6620 7374 6172 7443 6861 7428 293a  def startChat():
-000161d0: 0a20 2020 2020 2020 2020 2020 2063 6c65  .            cle
-000161e0: 6172 2829 0a20 2020 2020 2020 2020 2020  ar().           
-000161f0: 2070 7269 6e74 3128 7365 6c66 2e64 6976   print1(self.div
-00016200: 6964 6572 290a 2020 2020 2020 2020 2020  ider).          
-00016210: 2020 7365 6c66 2e73 686f 774c 6f67 6f28    self.showLogo(
-00016220: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00016230: 6c66 2e73 686f 7743 7572 7265 6e74 436f  lf.showCurrentCo
-00016240: 6e74 6578 7428 290a 2020 2020 2020 2020  ntext().        
-00016250: 2020 2020 2320 676f 2074 6f20 7374 6172      # go to star
-00016260: 7475 7020 6469 7265 6374 6f72 790a 2020  tup directory.  
-00016270: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
-00016280: 6564 6972 6563 746f 7279 203d 2063 6f6e  edirectory = con
-00016290: 6669 672e 6c6f 6361 6c53 746f 7261 6765  fig.localStorage
-000162a0: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
-000162b0: 6368 6469 7228 7374 6f72 6167 6564 6972  chdir(storagedir
-000162c0: 6563 746f 7279 290a 2020 2020 2020 2020  ectory).        
-000162d0: 2020 2020 6d65 7373 6167 6573 203d 2043      messages = C
-000162e0: 616c 6c4c 4c4d 2e72 6573 6574 4d65 7373  allLLM.resetMess
-000162f0: 6167 6573 2829 0a20 2020 2020 2020 2020  ages().         
-00016300: 2020 2023 7072 696e 7431 2866 2273 7461     #print1(f"sta
-00016310: 7274 7570 2064 6972 6563 746f 7279 3a5c  rtup directory:\
-00016320: 6e7b 7374 6f72 6167 6564 6972 6563 746f  n{storagedirecto
-00016330: 7279 7d22 290a 2020 2020 2020 2020 2020  ry}").          
-00016340: 2020 7072 696e 745f 666f 726d 6174 7465    print_formatte
-00016350: 645f 7465 7874 2848 544d 4c28 6622 3c7b  d_text(HTML(f"<{
-00016360: 636f 6e66 6967 2e74 6572 6d69 6e61 6c50  config.terminalP
-00016370: 726f 6d70 7449 6e64 6963 6174 6f72 436f  romptIndicatorCo
-00016380: 6c6f 7232 7d3e 4469 7265 6374 6f72 793a  lor2}>Directory:
-00016390: 3c2f 7b63 6f6e 6669 672e 7465 726d 696e  </{config.termin
-000163a0: 616c 5072 6f6d 7074 496e 6469 6361 746f  alPromptIndicato
-000163b0: 7243 6f6c 6f72 327d 3e20 7b73 746f 7261  rColor2}> {stora
-000163c0: 6765 6469 7265 6374 6f72 797d 2229 290a  gedirectory}")).
-000163d0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000163e0: 7431 2873 656c 662e 6469 7669 6465 7229  t1(self.divider)
-000163f0: 0a0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00016400: 6e66 6967 2e63 6f6e 7665 7273 6174 696f  nfig.conversatio
-00016410: 6e53 7461 7274 6564 203d 2046 616c 7365  nStarted = False
-00016420: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00016430: 7572 6e20 2873 746f 7261 6765 6469 7265  urn (storagedire
-00016440: 6374 6f72 792c 206d 6573 7361 6765 7329  ctory, messages)
-00016450: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
-00016460: 6469 7265 6374 6f72 792c 2063 6f6e 6669  directory, confi
-00016470: 672e 6375 7272 656e 744d 6573 7361 6765  g.currentMessage
-00016480: 7320 3d20 7374 6172 7443 6861 7428 290a  s = startChat().
-00016490: 2020 2020 2020 2020 636f 6e66 6967 2e6d          config.m
-000164a0: 756c 7469 6c69 6e65 496e 7075 7420 3d20  ultilineInput = 
-000164b0: 4661 6c73 650a 2020 2020 2020 2020 6665  False.        fe
-000164c0: 6174 7572 6573 4c6f 7765 7220 3d20 6c69  aturesLower = li
-000164d0: 7374 2873 656c 662e 6163 7469 6f6e 732e  st(self.actions.
-000164e0: 6b65 7973 2829 2920 2b20 5b22 2e2e 2e22  keys()) + ["..."
-000164f0: 5d0a 2020 2020 2020 2020 2320 696e 7075  ].        # inpu
-00016500: 7420 7375 6767 6573 7469 6f6e 730a 2020  t suggestions.  
-00016510: 2020 2020 2020 636f 6e66 6967 2e69 6e70        config.inp
-00016520: 7574 5375 6767 6573 7469 6f6e 7320 2b3d  utSuggestions +=
-00016530: 2066 6561 7475 7265 734c 6f77 6572 0a20   featuresLower. 
-00016540: 2020 2020 2020 2063 6f6d 706c 6574 6572         completer
-00016550: 203d 2046 757a 7a79 436f 6d70 6c65 7465   = FuzzyComplete
-00016560: 7228 576f 7264 436f 6d70 6c65 7465 7228  r(WordCompleter(
-00016570: 636f 6e66 6967 2e69 6e70 7574 5375 6767  config.inputSugg
-00016580: 6573 7469 6f6e 732c 2069 676e 6f72 655f  estions, ignore_
-00016590: 6361 7365 3d54 7275 6529 2920 6966 2063  case=True)) if c
-000165a0: 6f6e 6669 672e 696e 7075 7453 7567 6765  onfig.inputSugge
-000165b0: 7374 696f 6e73 2065 6c73 6520 4e6f 6e65  stions else None
-000165c0: 0a20 2020 2020 2020 2063 6f6d 706c 6574  .        complet
-000165d0: 6572 5f64 6576 656c 6f70 6572 203d 2046  er_developer = F
-000165e0: 757a 7a79 436f 6d70 6c65 7465 7228 576f  uzzyCompleter(Wo
-000165f0: 7264 436f 6d70 6c65 7465 7228 636f 6e66  rdCompleter(conf
-00016600: 6967 2e69 6e70 7574 5375 6767 6573 7469  ig.inputSuggesti
-00016610: 6f6e 735b 3a5d 202b 205b 6622 636f 6e66  ons[:] + [f"conf
-00016620: 6967 2e7b 697d 2220 666f 7220 6920 696e  ig.{i}" for i in
-00016630: 2064 6972 2863 6f6e 6669 6729 2069 6620   dir(config) if 
-00016640: 6e6f 7420 692e 7374 6172 7473 7769 7468  not i.startswith
-00016650: 2822 5f5f 2229 5d20 2b20 7365 6c66 2e67  ("__")] + self.g
-00016660: 6574 4469 7265 6374 6f72 794c 6973 7428  etDirectoryList(
-00016670: 292c 2069 676e 6f72 655f 6361 7365 3d54  ), ignore_case=T
-00016680: 7275 6529 290a 2020 2020 2020 2020 7768  rue)).        wh
-00016690: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
-000166a0: 2020 2020 2020 2320 6465 6661 756c 7420        # default 
-000166b0: 746f 6f6c 6261 7220 7465 7874 0a20 2020  toolbar text.   
-000166c0: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
-000166d0: 6479 6e61 6d69 6354 6f6f 6c42 6172 5465  dynamicToolBarTe
-000166e0: 7874 203d 2066 2222 2220 7b73 7472 2863  xt = f""" {str(c
-000166f0: 6f6e 6669 672e 686f 746b 6579 5f65 7869  onfig.hotkey_exi
-00016700: 7429 2e72 6570 6c61 6365 2822 2722 2c20  t).replace("'", 
-00016710: 2222 297d 2065 7869 7420 7b73 7472 2863  "")} exit {str(c
-00016720: 6f6e 6669 672e 686f 746b 6579 5f64 6973  onfig.hotkey_dis
-00016730: 706c 6179 5f6b 6579 5f63 6f6d 626f 292e  play_key_combo).
-00016740: 7265 706c 6163 6528 2227 222c 2022 2229  replace("'", "")
-00016750: 7d20 7368 6f72 7463 7574 7320 2222 220a  } shortcuts """.
-00016760: 2020 2020 2020 2020 2020 2020 2320 6469              # di
-00016770: 7370 6c61 7920 6375 7272 656e 7420 6469  splay current di
-00016780: 7265 6374 6f72 7920 6966 2063 6861 6e67  rectory if chang
-00016790: 6564 0a20 2020 2020 2020 2020 2020 2063  ed.            c
-000167a0: 7572 7265 6e74 4469 7265 6374 6f72 7920  urrentDirectory 
-000167b0: 3d20 6f73 2e67 6574 6377 6428 290a 2020  = os.getcwd().  
-000167c0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-000167d0: 2063 7572 7265 6e74 4469 7265 6374 6f72   currentDirector
-000167e0: 7920 3d3d 2073 746f 7261 6765 6469 7265  y == storagedire
-000167f0: 6374 6f72 793a 0a20 2020 2020 2020 2020  ctory:.         
-00016800: 2020 2020 2020 2023 7072 696e 7431 2873         #print1(s
-00016810: 656c 662e 6469 7669 6465 7229 0a20 2020  elf.divider).   
-00016820: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00016830: 6e74 3328 6622 4375 7272 656e 7420 6469  nt3(f"Current di
-00016840: 7265 6374 6f72 793a 207b 6375 7272 656e  rectory: {curren
-00016850: 7444 6972 6563 746f 7279 7d22 290a 2020  tDirectory}").  
-00016860: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00016870: 696e 7431 2873 656c 662e 6469 7669 6465  int1(self.divide
-00016880: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-00016890: 2020 2073 746f 7261 6765 6469 7265 6374     storagedirect
-000168a0: 6f72 7920 3d20 6375 7272 656e 7444 6972  ory = currentDir
-000168b0: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
-000168c0: 2020 2023 2064 6566 6175 6c74 2069 6e70     # default inp
-000168d0: 7574 2065 6e74 7279 0a20 2020 2020 2020  ut entry.       
-000168e0: 2020 2020 2061 6363 6570 745f 6465 6661       accept_defa
-000168f0: 756c 7420 3d20 636f 6e66 6967 2e61 6363  ult = config.acc
-00016900: 6570 745f 6465 6661 756c 740a 2020 2020  ept_default.    
-00016910: 2020 2020 2020 2020 636f 6e66 6967 2e61          config.a
-00016920: 6363 6570 745f 6465 6661 756c 7420 3d20  ccept_default = 
-00016930: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00016940: 2020 6465 6661 756c 7445 6e74 7279 203d    defaultEntry =
-00016950: 2063 6f6e 6669 672e 6465 6661 756c 7445   config.defaultE
-00016960: 6e74 7279 0a20 2020 2020 2020 2020 2020  ntry.           
-00016970: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
-00016980: 6c65 2864 6566 6175 6c74 456e 7472 7929  le(defaultEntry)
-00016990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000169a0: 2020 6465 6661 756c 7445 6e74 7279 203d    defaultEntry =
-000169b0: 2066 2746 696c 653a 2022 7b64 6566 6175   f'File: "{defau
-000169c0: 6c74 456e 7472 797d 225c 6e27 0a20 2020  ltEntry}"\n'.   
-000169d0: 2020 2020 2020 2020 2065 6c69 6620 6f73           elif os
-000169e0: 2e70 6174 682e 6973 6469 7228 6465 6661  .path.isdir(defa
-000169f0: 756c 7445 6e74 7279 293a 0a20 2020 2020  ultEntry):.     
-00016a00: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-00016a10: 6c74 456e 7472 7920 3d20 6627 466f 6c64  ltEntry = f'Fold
-00016a20: 6572 3a20 227b 6465 6661 756c 7445 6e74  er: "{defaultEnt
-00016a30: 7279 7d22 5c6e 270a 2020 2020 2020 2020  ry}"\n'.        
-00016a40: 2020 2020 636f 6e66 6967 2e64 6566 6175      config.defau
-00016a50: 6c74 456e 7472 7920 3d20 2222 0a0a 2020  ltEntry = ""..  
-00016a60: 2020 2020 2020 2020 2020 2320 7573 6572            # user
-00016a70: 2069 6e70 7574 0a20 2020 2020 2020 2020   input.         
-00016a80: 2020 2075 7365 7249 6e70 7574 203d 2073     userInput = s
-00016a90: 656c 662e 7072 6f6d 7074 732e 7369 6d70  elf.prompts.simp
-00016aa0: 6c65 5072 6f6d 7074 2870 726f 6d70 7453  lePrompt(promptS
-00016ab0: 6573 7369 6f6e 3d73 656c 662e 7465 726d  ession=self.term
-00016ac0: 696e 616c 5f63 6861 745f 7365 7373 696f  inal_chat_sessio
-00016ad0: 6e2c 2063 6f6d 706c 6574 6572 3d63 6f6d  n, completer=com
-00016ae0: 706c 6574 6572 5f64 6576 656c 6f70 6572  pleter_developer
-00016af0: 2069 6620 636f 6e66 6967 2e64 6576 656c   if config.devel
-00016b00: 6f70 6572 2065 6c73 6520 636f 6d70 6c65  oper else comple
-00016b10: 7465 722c 2064 6566 6175 6c74 3d64 6566  ter, default=def
-00016b20: 6175 6c74 456e 7472 792c 2061 6363 6570  aultEntry, accep
-00016b30: 745f 6465 6661 756c 743d 6163 6365 7074  t_default=accept
-00016b40: 5f64 6566 6175 6c74 2c20 7661 6c69 6461  _default, valida
-00016b50: 746f 723d 746f 6b65 6e56 616c 6964 6174  tor=tokenValidat
-00016b60: 6f72 2c20 626f 7474 6f6d 5f74 6f6f 6c62  or, bottom_toolb
-00016b70: 6172 3d67 6574 4479 6e61 6d69 6354 6f6f  ar=getDynamicToo
-00016b80: 6c42 6172 290a 2020 2020 2020 2020 2020  lBar).          
-00016b90: 2020 0a20 2020 2020 2020 2020 2020 2023    .            #
-00016ba0: 2075 7064 6174 6520 7379 7374 656d 206d   update system m
-00016bb0: 6573 7361 6765 2077 6865 6e20 7573 6572  essage when user
-00016bc0: 2065 6e74 6572 2061 206e 6577 2069 6e70   enter a new inp
-00016bd0: 7574 0a20 2020 2020 2020 2020 2020 2063  ut.            c
-00016be0: 6f6e 6669 672e 6375 7272 656e 744d 6573  onfig.currentMes
-00016bf0: 7361 6765 7320 3d20 7365 6c66 2e75 7064  sages = self.upd
-00016c00: 6174 6553 7973 7465 6d4d 6573 7361 6765  ateSystemMessage
-00016c10: 2863 6f6e 6669 672e 6375 7272 656e 744d  (config.currentM
-00016c20: 6573 7361 6765 7329 0a20 2020 2020 2020  essages).       
-00016c30: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00016c40: 2020 2320 6469 7370 6c61 7920 6f70 7469    # display opti
-00016c50: 6f6e 7320 7768 656e 2065 6d70 7479 2073  ons when empty s
-00016c60: 7472 696e 6720 6973 2065 6e74 6572 6564  tring is entered
-00016c70: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
-00016c80: 7249 6e70 7574 4c6f 7765 7220 3d20 7573  rInputLower = us
-00016c90: 6572 496e 7075 742e 6c6f 7765 7228 290a  erInput.lower().
-00016ca0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00016cb0: 6f6e 6669 672e 6164 6450 6174 6841 7420  onfig.addPathAt 
-00016cc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00016cd0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00016ce0: 6669 7820 3d20 7573 6572 496e 7075 745b  fix = userInput[
-00016cf0: 3a63 6f6e 6669 672e 6164 6450 6174 6841  :config.addPathA
-00016d00: 745d 0a20 2020 2020 2020 2020 2020 2020  t].             
-00016d10: 2020 2070 7265 6669 7853 706c 6974 203d     prefixSplit =
-00016d20: 2070 7265 6669 782e 7273 706c 6974 2822   prefix.rsplit("
-00016d30: 2022 2c20 3129 0a20 2020 2020 2020 2020   ", 1).         
-00016d40: 2020 2020 2020 2069 6620 6c65 6e28 7072         if len(pr
-00016d50: 6566 6978 5370 6c69 7429 203e 2031 3a0a  efixSplit) > 1:.
-00016d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d70: 2020 2020 6465 6661 756c 7420 3d20 7072      default = pr
-00016d80: 6566 6978 5370 6c69 745b 2d31 5d0a 2020  efixSplit[-1].  
-00016d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016da0: 2020 7072 6566 6978 203d 2066 227b 7072    prefix = f"{pr
-00016db0: 6566 6978 5370 6c69 745b 305d 7d20 220a  efixSplit[0]} ".
-00016dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dd0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00016de0: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
-00016df0: 7420 3d20 7072 6566 6978 0a20 2020 2020  t = prefix.     
-00016e00: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00016e10: 7265 6669 7820 3d20 2222 0a20 2020 2020  refix = "".     
-00016e20: 2020 2020 2020 2020 2020 2073 7566 6669             suffi
-00016e30: 7820 3d20 7573 6572 496e 7075 745b 636f  x = userInput[co
-00016e40: 6e66 6967 2e61 6464 5061 7468 4174 3a5d  nfig.addPathAt:]
-00016e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016e60: 2063 6f6e 6669 672e 6164 6450 6174 6841   config.addPathA
-00016e70: 7420 3d20 4e6f 6e65 0a20 2020 2020 2020  t = None.       
-00016e80: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00016e90: 6465 6661 756c 743a 0a20 2020 2020 2020  default:.       
-00016ea0: 2020 2020 2020 2020 2020 2020 2064 6566               def
-00016eb0: 6175 6c74 203d 206f 732e 6765 7463 7764  ault = os.getcwd
-00016ec0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00016ed0: 2020 2075 7365 7250 6174 6820 3d20 7365     userPath = se
-00016ee0: 6c66 2e67 6574 5061 7468 2e67 6574 5061  lf.getPath.getPa
-00016ef0: 7468 286d 6573 7361 6765 3d66 227b 7072  th(message=f"{pr
-00016f00: 6566 6978 7d3c 7b63 6f6e 6669 672e 7465  efix}<{config.te
-00016f10: 726d 696e 616c 436f 6d6d 616e 6445 6e74  rminalCommandEnt
-00016f20: 7279 436f 6c6f 7232 7d3e 5b61 6464 2061  ryColor2}>[add a
-00016f30: 2070 6174 6820 6865 7265 5d3c 2f7b 636f   path here]</{co
-00016f40: 6e66 6967 2e74 6572 6d69 6e61 6c43 6f6d  nfig.terminalCom
-00016f50: 6d61 6e64 456e 7472 7943 6f6c 6f72 327d  mandEntryColor2}
-00016f60: 3e7b 7375 6666 6978 7d22 2c20 7072 6f6d  >{suffix}", prom
-00016f70: 7074 496e 6469 6361 746f 723d 223e 3e3e  ptIndicator=">>>
-00016f80: 2022 2c20 656d 7074 795f 746f 5f63 616e   ", empty_to_can
-00016f90: 6365 6c3d 5472 7565 2c20 6465 6661 756c  cel=True, defaul
-00016fa0: 743d 6465 6661 756c 7429 0a20 2020 2020  t=default).     
-00016fb0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00016fc0: 672e 6465 6661 756c 7445 6e74 7279 203d  g.defaultEntry =
-00016fd0: 2066 227b 7072 6566 6978 7d7b 7573 6572   f"{prefix}{user
-00016fe0: 5061 7468 7d7b 7375 6666 6978 7d22 0a20  Path}{suffix}". 
-00016ff0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00017000: 7365 7249 6e70 7574 203d 2022 220a 2020  serInput = "".  
-00017010: 2020 2020 2020 2020 2020 656c 6966 206e            elif n
-00017020: 6f74 2075 7365 7249 6e70 7574 4c6f 7765  ot userInputLowe
-00017030: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00017040: 2020 2075 7365 7249 6e70 7574 203d 2063     userInput = c
-00017050: 6f6e 6669 672e 626c 616e 6b45 6e74 7279  onfig.blankEntry
-00017060: 4163 7469 6f6e 0a20 2020 2020 2020 2020  Action.         
-00017070: 2020 2069 6620 7573 6572 496e 7075 7420     if userInput 
-00017080: 3d3d 2022 2e2e 2e22 3a0a 2020 2020 2020  == "...":.      
-00017090: 2020 2020 2020 2020 2020 7573 6572 496e            userIn
-000170a0: 7075 7420 3d20 7573 6572 496e 7075 744c  put = userInputL
-000170b0: 6f77 6572 203d 2073 656c 662e 7275 6e41  ower = self.runA
-000170c0: 6374 696f 6e73 2875 7365 7249 6e70 7574  ctions(userInput
-000170d0: 290a 2020 2020 2020 2020 2020 2020 2365  ).            #e
-000170e0: 6c69 6620 7573 6572 496e 7075 744c 6f77  lif userInputLow
-000170f0: 6572 2069 6e20 7475 706c 6528 7365 6c66  er in tuple(self
-00017100: 2e61 6374 696f 6e73 2e6b 6579 7328 2929  .actions.keys())
-00017110: 3a0a 2020 2020 2020 2020 2020 2020 656c  :.            el
-00017120: 6966 2075 7365 7249 6e70 7574 4c6f 7765  if userInputLowe
-00017130: 722e 7374 6172 7473 7769 7468 2822 2e22  r.startswith("."
-00017140: 2920 616e 6420 6e6f 7420 7573 6572 496e  ) and not userIn
-00017150: 7075 744c 6f77 6572 2069 6e20 2863 6f6e  putLower in (con
-00017160: 6669 672e 6578 6974 5f65 6e74 7279 2c20  fig.exit_entry, 
-00017170: 636f 6e66 6967 2e63 616e 6365 6c5f 656e  config.cancel_en
-00017180: 7472 792c 2022 2e6e 6577 222c 2022 2e63  try, ".new", ".c
-00017190: 6f6e 7465 7874 2229 3a0a 2020 2020 2020  ontext"):.      
-000171a0: 2020 2020 2020 2020 2020 7573 6572 496e            userIn
-000171b0: 7075 7420 3d20 7573 6572 496e 7075 744c  put = userInputL
-000171c0: 6f77 6572 203d 2073 656c 662e 7275 6e41  ower = self.runA
-000171d0: 6374 696f 6e73 2822 2e2e 2e22 2c20 7573  ctions("...", us
-000171e0: 6572 496e 7075 7429 0a0a 2020 2020 2020  erInput)..      
-000171f0: 2020 2020 2020 6966 2073 6574 546f 6f6c        if setTool
-00017200: 4465 7065 6e64 656e 6365 2875 7365 7249  Dependence(userI
-00017210: 6e70 7574 293a 0a20 2020 2020 2020 2020  nput):.         
-00017220: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-00017230: 0a20 2020 2020 2020 2020 2020 2023 2072  .            # r
-00017240: 6570 6c61 6365 2061 6c69 6173 2c20 6966  eplace alias, if
-00017250: 2061 6e79 2c20 7769 7468 2066 756c 6c20   any, with full 
-00017260: 656e 7472 790a 2020 2020 2020 2020 2020  entry.          
-00017270: 2020 666f 7220 616c 6961 732c 2066 756c    for alias, ful
-00017280: 6c45 6e74 7279 2069 6e20 636f 6e66 6967  lEntry in config
-00017290: 2e61 6c69 6173 6573 2e69 7465 6d73 2829  .aliases.items()
-000172a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000172b0: 2020 2375 7365 7249 6e70 7574 203d 2072    #userInput = r
-000172c0: 652e 7375 6228 616c 6961 732c 2066 756c  e.sub(alias, ful
-000172d0: 6c45 6e74 7279 2c20 7573 6572 496e 7075  lEntry, userInpu
-000172e0: 7429 2023 2065 7272 6f72 206f 6e20 5769  t) # error on Wi
-000172f0: 6e64 6f77 7320 636f 7a20 6f66 2057 696e  ndows coz of Win
-00017300: 646f 7773 2070 6174 680a 2020 2020 2020  dows path.      
-00017310: 2020 2020 2020 2020 2020 7573 6572 496e            userIn
-00017320: 7075 7420 3d20 7573 6572 496e 7075 742e  put = userInput.
-00017330: 7265 706c 6163 6528 616c 6961 732c 2066  replace(alias, f
-00017340: 756c 6c45 6e74 7279 290a 0a20 2020 2020  ullEntry)..     
-00017350: 2020 2020 2020 2023 206f 7065 6e20 6669         # open fi
-00017360: 6c65 202f 2064 6972 6563 746f 7279 2064  le / directory d
-00017370: 6972 6563 746c 790a 2020 2020 2020 2020  irectly.        
-00017380: 2020 2020 646f 6373 5f70 6174 6820 3d20      docs_path = 
-00017390: 6973 4578 6973 7469 6e67 5061 7468 2875  isExistingPath(u
-000173a0: 7365 7249 6e70 7574 290a 2020 2020 2020  serInput).      
-000173b0: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
-000173c0: 2e69 7366 696c 6528 646f 6373 5f70 6174  .isfile(docs_pat
-000173d0: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
-000173e0: 2020 2020 6f73 2e73 7973 7465 6d28 6622      os.system(f"
-000173f0: 7b63 6f6e 6669 672e 6f70 656e 7d20 7b64  {config.open} {d
-00017400: 6f63 735f 7061 7468 7d22 290a 2020 2020  ocs_path}").    
-00017410: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00017420: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-00017430: 2065 6c69 6620 6f73 2e70 6174 682e 6973   elif os.path.is
-00017440: 6469 7228 646f 6373 5f70 6174 6829 3a0a  dir(docs_path):.
-00017450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017460: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00017470: 2020 2020 2020 2020 206f 732e 6368 6469           os.chdi
-00017480: 7228 646f 6373 5f70 6174 6829 0a20 2020  r(docs_path).   
-00017490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174a0: 2070 7269 6e74 3328 6622 4469 7265 6374   print3(f"Direct
-000174b0: 6f72 7920 6368 616e 6765 6420 746f 3a20  ory changed to: 
-000174c0: 7b64 6f63 735f 7061 7468 7d22 290a 2020  {docs_path}").  
-000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174e0: 2020 7365 6c66 2e67 6574 5061 7468 2e64    self.getPath.d
-000174f0: 6973 706c 6179 4469 7265 6374 6f72 7943  isplayDirectoryC
-00017500: 6f6e 7465 6e74 2829 0a20 2020 2020 2020  ontent().       
-00017510: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00017520: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-00017530: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017550: 2020 7061 7373 0a0a 2020 2020 2020 2020    pass..        
-00017560: 2020 2020 2320 7472 7920 6576 616c 0a20      # try eval. 
-00017570: 2020 2020 2020 2020 2020 2069 6620 636f             if co
-00017580: 6e66 6967 2e64 6576 656c 6f70 6572 2061  nfig.developer a
-00017590: 6e64 206e 6f74 2075 7365 7249 6e70 7574  nd not userInput
-000175a0: 203d 3d20 222e 2e2e 223a 0a20 2020 2020   == "...":.     
-000175b0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-000175c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175d0: 2020 2020 7661 6c75 6520 3d20 6576 616c      value = eval
-000175e0: 2875 7365 7249 6e70 7574 2920 2320 6974  (userInput) # it
-000175f0: 2073 6f6c 7665 2073 696d 706c 6520 6d61   solve simple ma
-00017600: 7468 2c20 652e 672e 2031 2b31 2c20 6f72  th, e.g. 1+1, or
-00017610: 2072 6561 6420 7661 7269 6162 6c65 732c   read variables,
-00017620: 2065 2e67 2e20 6469 7228 636f 6e66 6967   e.g. dir(config
-00017630: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00017640: 2020 2020 2020 6966 2076 616c 7565 2069        if value i
-00017650: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00017660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017670: 2020 2020 2370 7269 6e74 2876 616c 7565      #print(value
-00017680: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00017690: 2020 2020 2020 2020 2020 7070 7269 6e74            pprint
-000176a0: 2e70 7072 696e 7428 7661 6c75 6529 0a20  .pprint(value). 
+00015530: 2020 2020 6f73 2e73 7973 7465 6d28 6627      os.system(f'
+00015540: 2727 7b63 6f6e 6669 672e 6f70 656e 7d20  ''{config.open} 
+00015550: 227b 6368 6174 4669 6c65 7d22 2727 2729  "{chatFile}"''')
+00015560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015570: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+00015580: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00015590: 6e74 3228 2246 6169 6c65 6420 746f 2073  nt2("Failed to s
+000155a0: 6176 6520 6368 6174 215c 6e22 290a 2020  ave chat!\n").  
+000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155c0: 2020 7368 6f77 4572 726f 7273 2829 0a0a    showErrors()..
+000155d0: 2020 2020 6465 6620 7275 6e49 6e73 7472      def runInstr
+000155e0: 7563 7469 6f6e 2873 656c 6629 3a0a 2020  uction(self):.  
+000155f0: 2020 2020 2020 696e 7374 7275 6374 696f        instructio
+00015600: 6e73 203d 206c 6973 7428 636f 6e66 6967  ns = list(config
+00015610: 2e70 7265 6465 6669 6e65 6449 6e73 7472  .predefinedInstr
+00015620: 7563 7469 6f6e 732e 6b65 7973 2829 290a  uctions.keys()).
+00015630: 2020 2020 2020 2020 696e 7374 7275 6374          instruct
+00015640: 696f 6e20 3d20 7365 6c66 2e64 6961 6c6f  ion = self.dialo
+00015650: 6773 2e67 6574 5661 6c69 644f 7074 696f  gs.getValidOptio
+00015660: 6e73 280a 2020 2020 2020 2020 2020 2020  ns(.            
+00015670: 6f70 7469 6f6e 733d 696e 7374 7275 6374  options=instruct
+00015680: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
+00015690: 2020 7469 746c 653d 2250 7265 6465 6669    title="Predefi
+000156a0: 6e65 6420 496e 7374 7275 6374 696f 6e73  ned Instructions
+000156b0: 222c 0a20 2020 2020 2020 2020 2020 2074  ",.            t
+000156c0: 6578 743d 2253 656c 6563 7420 616e 2069  ext="Select an i
+000156d0: 6e73 7472 7563 7469 6f6e 3a22 2c0a 2020  nstruction:",.  
+000156e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000156f0: 6966 2069 6e73 7472 7563 7469 6f6e 3a0a  if instruction:.
+00015700: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+00015710: 6967 2e64 6566 6175 6c74 456e 7472 7920  ig.defaultEntry 
+00015720: 3d20 636f 6e66 6967 2e70 7265 6465 6669  = config.predefi
+00015730: 6e65 6449 6e73 7472 7563 7469 6f6e 735b  nedInstructions[
+00015740: 696e 7374 7275 6374 696f 6e5d 0a20 2020  instruction].   
+00015750: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
+00015760: 6163 6365 7074 5f64 6566 6175 6c74 203d  accept_default =
+00015770: 2054 7275 650a 0a20 2020 2064 6566 2063   True..    def c
+00015780: 6861 6e67 6543 6f6e 7465 7874 2873 656c  hangeContext(sel
+00015790: 6629 3a0a 2020 2020 2020 2020 636f 6e74  f):.        cont
+000157a0: 6578 7473 203d 206c 6973 7428 636f 6e66  exts = list(conf
+000157b0: 6967 2e70 7265 6465 6669 6e65 6443 6f6e  ig.predefinedCon
+000157c0: 7465 7874 732e 6b65 7973 2829 290a 2020  texts.keys()).  
+000157d0: 2020 2020 2020 7072 6564 6566 696e 6564        predefined
+000157e0: 436f 6e74 6578 7420 3d20 7365 6c66 2e64  Context = self.d
+000157f0: 6961 6c6f 6773 2e67 6574 5661 6c69 644f  ialogs.getValidO
+00015800: 7074 696f 6e73 280a 2020 2020 2020 2020  ptions(.        
+00015810: 2020 2020 6f70 7469 6f6e 733d 636f 6e74      options=cont
+00015820: 6578 7473 2c0a 2020 2020 2020 2020 2020  exts,.          
+00015830: 2020 7469 746c 653d 2250 7265 6465 6669    title="Predefi
+00015840: 6e65 6420 436f 6e74 6578 7473 222c 0a20  ned Contexts",. 
+00015850: 2020 2020 2020 2020 2020 2064 6566 6175             defau
+00015860: 6c74 3d63 6f6e 6669 672e 7072 6564 6566  lt=config.predef
+00015870: 696e 6564 436f 6e74 6578 742c 0a20 2020  inedContext,.   
+00015880: 2020 2020 2020 2020 2074 6578 743d 2253           text="S
+00015890: 656c 6563 7420 6120 636f 6e74 6578 743a  elect a context:
+000158a0: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
+000158b0: 2020 2020 2069 6620 7072 6564 6566 696e       if predefin
+000158c0: 6564 436f 6e74 6578 743a 0a20 2020 2020  edContext:.     
+000158d0: 2020 2020 2020 2063 6f6e 6669 672e 7072         config.pr
+000158e0: 6564 6566 696e 6564 436f 6e74 6578 7420  edefinedContext 
+000158f0: 3d20 7072 6564 6566 696e 6564 436f 6e74  = predefinedCont
+00015900: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
+00015910: 6966 2063 6f6e 6669 672e 7072 6564 6566  if config.predef
+00015920: 696e 6564 436f 6e74 6578 7420 3d3d 2022  inedContext == "
+00015930: 5b63 7573 746f 6d5d 223a 0a20 2020 2020  [custom]":.     
+00015940: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00015950: 3128 2245 6469 7420 6375 7374 6f6d 2063  1("Edit custom c
+00015960: 6f6e 7465 7874 2062 656c 6f77 3a22 290a  ontext below:").
+00015970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015980: 6375 7374 6f6d 436f 6e74 6578 7420 3d20  customContext = 
+00015990: 7365 6c66 2e70 726f 6d70 7473 2e73 696d  self.prompts.sim
+000159a0: 706c 6550 726f 6d70 7428 7374 796c 653d  plePrompt(style=
+000159b0: 7365 6c66 2e70 726f 6d70 7473 2e70 726f  self.prompts.pro
+000159c0: 6d70 7453 7479 6c65 322c 2064 6566 6175  mptStyle2, defau
+000159d0: 6c74 3d63 6f6e 6669 672e 6375 7374 6f6d  lt=config.custom
+000159e0: 5072 6564 6566 696e 6564 436f 6e74 6578  PredefinedContex
+000159f0: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00015a00: 2020 2069 6620 6375 7374 6f6d 436f 6e74     if customCont
+00015a10: 6578 7420 616e 6420 6e6f 7420 6375 7374  ext and not cust
+00015a20: 6f6d 436f 6e74 6578 742e 7374 7269 7028  omContext.strip(
+00015a30: 292e 6c6f 7765 7228 2920 3d3d 2063 6f6e  ).lower() == con
+00015a40: 6669 672e 6578 6974 5f65 6e74 7279 3a0a  fig.exit_entry:.
+00015a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a60: 2020 2020 636f 6e66 6967 2e63 7573 746f      config.custo
+00015a70: 6d50 7265 6465 6669 6e65 6443 6f6e 7465  mPredefinedConte
+00015a80: 7874 203d 2063 7573 746f 6d43 6f6e 7465  xt = customConte
+00015a90: 7874 2e73 7472 6970 2829 0a20 2020 2020  xt.strip().     
+00015aa0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00015ab0: 2020 2020 2023 2061 2077 6179 2074 6f20       # a way to 
+00015ac0: 7175 6963 6b6c 7920 636c 6561 6e20 7570  quickly clean up
+00015ad0: 2063 6f6e 7465 7874 0a20 2020 2020 2020   context.       
+00015ae0: 2020 2020 2063 6f6e 6669 672e 7072 6564       config.pred
+00015af0: 6566 696e 6564 436f 6e74 6578 7420 3d20  efinedContext = 
+00015b00: 225b 6e6f 6e65 5d22 0a20 2020 2020 2020  "[none]".       
+00015b10: 2063 6f6e 6669 672e 7361 7665 436f 6e66   config.saveConf
+00015b20: 6967 2829 0a20 2020 2020 2020 2073 656c  ig().        sel
+00015b30: 662e 7368 6f77 4375 7272 656e 7443 6f6e  f.showCurrentCon
+00015b40: 7465 7874 2829 0a0a 2020 2020 6465 6620  text()..    def 
+00015b50: 6765 7444 6972 6563 746f 7279 4c69 7374  getDirectoryList
+00015b60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00015b70: 6469 7265 6374 6f72 794c 6973 7420 3d20  directoryList = 
+00015b80: 5b5d 0a20 2020 2020 2020 2066 6f72 2066  [].        for f
+00015b90: 2069 6e20 6f73 2e6c 6973 7464 6972 2827   in os.listdir('
+00015ba0: 2e27 293a 0a20 2020 2020 2020 2020 2020  .'):.           
+00015bb0: 2069 6620 6f73 2e70 6174 682e 6973 6469   if os.path.isdi
+00015bc0: 7228 6629 3a0a 2020 2020 2020 2020 2020  r(f):.          
+00015bd0: 2020 2020 2020 7365 7061 7261 746f 7220        separator 
+00015be0: 3d20 225c 5c22 2069 6620 636f 6e66 6967  = "\\" if config
+00015bf0: 2e74 6869 7350 6c61 7466 6f72 6d20 3d3d  .thisPlatform ==
+00015c00: 2022 5769 6e64 6f77 7322 2065 6c73 6520   "Windows" else 
+00015c10: 222f 220a 2020 2020 2020 2020 2020 2020  "/".            
+00015c20: 2020 2020 6469 7265 6374 6f72 794c 6973      directoryLis
+00015c30: 742e 6170 7065 6e64 2866 227b 667d 7b73  t.append(f"{f}{s
+00015c40: 6570 6172 6174 6f72 7d22 290a 2020 2020  eparator}").    
+00015c50: 2020 2020 2020 2020 656c 6966 206f 732e          elif os.
+00015c60: 7061 7468 2e69 7366 696c 6528 6629 3a0a  path.isfile(f):.
+00015c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c80: 6469 7265 6374 6f72 794c 6973 742e 6170  directoryList.ap
+00015c90: 7065 6e64 2866 290a 2020 2020 2020 2020  pend(f).        
+00015ca0: 7265 7475 726e 2064 6972 6563 746f 7279  return directory
+00015cb0: 4c69 7374 0a0a 2020 2020 6465 6620 7368  List..    def sh
+00015cc0: 6f77 4c6f 676f 2873 656c 6629 3a0a 2020  owLogo(self):.  
+00015cd0: 2020 2020 2020 6170 704e 616d 6520 3d20        appName = 
+00015ce0: 636f 6e66 6967 2e66 7265 6547 656e 6975  config.freeGeniu
+00015cf0: 7341 494e 616d 652e 7370 6c69 7428 295b  sAIName.split()[
+00015d00: 305d 2e75 7070 6572 2829 0a20 2020 2020  0].upper().     
+00015d10: 2020 2074 6572 6d69 6e61 6c5f 7769 6474     terminal_widt
+00015d20: 6820 3d20 7368 7574 696c 2e67 6574 5f74  h = shutil.get_t
+00015d30: 6572 6d69 6e61 6c5f 7369 7a65 2829 2e63  erminal_size().c
+00015d40: 6f6c 756d 6e73 0a20 2020 2020 2020 2074  olumns.        t
+00015d50: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00015d60: 6672 6f6d 2061 7274 2069 6d70 6f72 7420  from art import 
+00015d70: 7465 7874 3261 7274 0a20 2020 2020 2020  text2art.       
+00015d80: 2020 2020 2069 6620 7465 726d 696e 616c       if terminal
+00015d90: 5f77 6964 7468 203e 3d20 3332 3a0a 2020  _width >= 32:.  
+00015da0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00015db0: 676f 203d 2074 6578 7432 6172 7428 6170  go = text2art(ap
+00015dc0: 704e 616d 652c 2066 6f6e 743d 2263 7962  pName, font="cyb
+00015dd0: 6572 6d65 6475 6d22 290a 2020 2020 2020  ermedum").      
+00015de0: 2020 2020 2020 656c 6966 2074 6572 6d69        elif termi
+00015df0: 6e61 6c5f 7769 6474 6820 3e3d 2032 303a  nal_width >= 20:
+00015e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015e10: 206c 6f67 6f20 3d20 7465 7874 3261 7274   logo = text2art
+00015e20: 2822 2022 2e6a 6f69 6e28 6170 704e 616d  (" ".join(appNam
+00015e30: 6529 202b 2022 2022 2c20 666f 6e74 3d22  e) + " ", font="
+00015e40: 7768 6974 655f 6275 6262 6c65 2229 0a20  white_bubble"). 
+00015e50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00015e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015e70: 206c 6f67 6f20 3d20 636f 6e66 6967 2e66   logo = config.f
+00015e80: 7265 6547 656e 6975 7341 494e 616d 650a  reeGeniusAIName.
+00015e90: 2020 2020 2020 2020 2020 2020 6c6f 676f              logo
+00015ea0: 203d 206c 6f67 6f5b 3a2d 315d 2023 2072   = logo[:-1] # r
+00015eb0: 656d 6f76 6520 7468 6520 6c69 6e65 6272  emove the linebr
+00015ec0: 6561 6b20 6174 2074 6865 2065 6e64 0a20  eak at the end. 
+00015ed0: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
+00015ee0: 2020 2020 2020 2020 2020 206c 6f67 6f20             logo 
+00015ef0: 3d20 636f 6e66 6967 2e66 7265 6547 656e  = config.freeGen
+00015f00: 6975 7341 494e 616d 650a 2020 2020 2020  iusAIName.      
+00015f10: 2020 7072 696e 745f 666f 726d 6174 7465    print_formatte
+00015f20: 645f 7465 7874 2848 544d 4c28 6622 3c7b  d_text(HTML(f"<{
+00015f30: 636f 6e66 6967 2e74 6572 6d69 6e61 6c43  config.terminalC
+00015f40: 6f6d 6d61 6e64 456e 7472 7943 6f6c 6f72  ommandEntryColor
+00015f50: 327d 3e7b 6c6f 676f 7d3c 2f7b 636f 6e66  2}>{logo}</{conf
+00015f60: 6967 2e74 6572 6d69 6e61 6c43 6f6d 6d61  ig.terminalComma
+00015f70: 6e64 456e 7472 7943 6f6c 6f72 327d 3e22  ndEntryColor2}>"
+00015f80: 2929 0a0a 2020 2020 6465 6620 7275 6e50  ))..    def runP
+00015f90: 7974 686f 6e53 6372 6970 7428 7365 6c66  ythonScript(self
+00015fa0: 2c20 7363 7269 7074 293a 0a20 2020 2020  , script):.     
+00015fb0: 2020 2073 6372 6970 7420 3d20 7363 7269     script = scri
+00015fc0: 7074 2e73 7472 6970 2829 5b33 3a2d 335d  pt.strip()[3:-3]
+00015fd0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00015fe0: 2020 2020 2020 2020 2020 6578 6563 2873            exec(s
+00015ff0: 6372 6970 742c 2067 6c6f 6261 6c73 2829  cript, globals()
+00016000: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+00016010: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
+00016020: 6163 6520 3d20 7472 6163 6562 6163 6b2e  ace = traceback.
+00016030: 666f 726d 6174 5f65 7863 2829 0a20 2020  format_exc().   
+00016040: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
+00016050: 7261 6365 2069 6620 636f 6e66 6967 2e64  race if config.d
+00016060: 6576 656c 6f70 6572 2065 6c73 6520 2245  eveloper else "E
+00016070: 7272 6f72 2065 6e63 6f75 6e74 6572 6564  rror encountered
+00016080: 2122 290a 2020 2020 2020 2020 2020 2020  !").            
+00016090: 7072 696e 7431 2863 6f6e 6669 672e 6469  print1(config.di
+000160a0: 7669 6465 7229 0a20 2020 2020 2020 2020  vider).         
+000160b0: 2020 2069 6620 636f 6e66 6967 2e6d 6178     if config.max
+000160c0: 5f63 6f6e 7365 6375 7469 7665 5f61 7574  _consecutive_aut
+000160d0: 6f5f 636f 7272 6563 7469 6f6e 203e 2030  o_correction > 0
+000160e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000160f0: 2020 4361 6c6c 4c4c 4d2e 6175 746f 436f    CallLLM.autoCo
+00016100: 7272 6563 7450 7974 686f 6e43 6f64 6528  rrectPythonCode(
+00016110: 7363 7269 7074 2c20 7472 6163 6529 0a0a  script, trace)..
+00016120: 2020 2020 6465 6620 7374 6172 7443 6861      def startCha
+00016130: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
+00016140: 2020 746f 6b65 6e56 616c 6964 6174 6f72    tokenValidator
+00016150: 203d 2054 6f6b 656e 5661 6c69 6461 746f   = TokenValidato
+00016160: 7228 290a 2020 2020 2020 2020 6465 6620  r().        def 
+00016170: 6765 7444 796e 616d 6963 546f 6f6c 4261  getDynamicToolBa
+00016180: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
+00016190: 2072 6574 7572 6e20 636f 6e66 6967 2e64   return config.d
+000161a0: 796e 616d 6963 546f 6f6c 4261 7254 6578  ynamicToolBarTex
+000161b0: 740a 2020 2020 2020 2020 6465 6620 7374  t.        def st
+000161c0: 6172 7443 6861 7428 293a 0a20 2020 2020  artChat():.     
+000161d0: 2020 2020 2020 2063 6c65 6172 2829 0a20         clear(). 
+000161e0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000161f0: 3128 7365 6c66 2e64 6976 6964 6572 290a  1(self.divider).
+00016200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016210: 2e73 686f 774c 6f67 6f28 290a 2020 2020  .showLogo().    
+00016220: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
+00016230: 7743 7572 7265 6e74 436f 6e74 6578 7428  wCurrentContext(
+00016240: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00016250: 676f 2074 6f20 7374 6172 7475 7020 6469  go to startup di
+00016260: 7265 6374 6f72 790a 2020 2020 2020 2020  rectory.        
+00016270: 2020 2020 7374 6f72 6167 6564 6972 6563      storagedirec
+00016280: 746f 7279 203d 2063 6f6e 6669 672e 6c6f  tory = config.lo
+00016290: 6361 6c53 746f 7261 6765 0a20 2020 2020  calStorage.     
+000162a0: 2020 2020 2020 206f 732e 6368 6469 7228         os.chdir(
+000162b0: 7374 6f72 6167 6564 6972 6563 746f 7279  storagedirectory
+000162c0: 290a 2020 2020 2020 2020 2020 2020 6d65  ).            me
+000162d0: 7373 6167 6573 203d 2043 616c 6c4c 4c4d  ssages = CallLLM
+000162e0: 2e72 6573 6574 4d65 7373 6167 6573 2829  .resetMessages()
+000162f0: 0a20 2020 2020 2020 2020 2020 2023 7072  .            #pr
+00016300: 696e 7431 2866 2273 7461 7274 7570 2064  int1(f"startup d
+00016310: 6972 6563 746f 7279 3a5c 6e7b 7374 6f72  irectory:\n{stor
+00016320: 6167 6564 6972 6563 746f 7279 7d22 290a  agedirectory}").
+00016330: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00016340: 745f 666f 726d 6174 7465 645f 7465 7874  t_formatted_text
+00016350: 2848 544d 4c28 6622 3c7b 636f 6e66 6967  (HTML(f"<{config
+00016360: 2e74 6572 6d69 6e61 6c50 726f 6d70 7449  .terminalPromptI
+00016370: 6e64 6963 6174 6f72 436f 6c6f 7232 7d3e  ndicatorColor2}>
+00016380: 4469 7265 6374 6f72 793a 3c2f 7b63 6f6e  Directory:</{con
+00016390: 6669 672e 7465 726d 696e 616c 5072 6f6d  fig.terminalProm
+000163a0: 7074 496e 6469 6361 746f 7243 6f6c 6f72  ptIndicatorColor
+000163b0: 327d 3e20 7b73 746f 7261 6765 6469 7265  2}> {storagedire
+000163c0: 6374 6f72 797d 2229 290a 2020 2020 2020  ctory}")).      
+000163d0: 2020 2020 2020 7072 696e 7431 2873 656c        print1(sel
+000163e0: 662e 6469 7669 6465 7229 0a0a 2020 2020  f.divider)..    
+000163f0: 2020 2020 2020 2020 636f 6e66 6967 2e63          config.c
+00016400: 6f6e 7665 7273 6174 696f 6e53 7461 7274  onversationStart
+00016410: 6564 203d 2046 616c 7365 0a20 2020 2020  ed = False.     
+00016420: 2020 2020 2020 2072 6574 7572 6e20 2873         return (s
+00016430: 746f 7261 6765 6469 7265 6374 6f72 792c  toragedirectory,
+00016440: 206d 6573 7361 6765 7329 0a20 2020 2020   messages).     
+00016450: 2020 2073 746f 7261 6765 6469 7265 6374     storagedirect
+00016460: 6f72 792c 2063 6f6e 6669 672e 6375 7272  ory, config.curr
+00016470: 656e 744d 6573 7361 6765 7320 3d20 7374  entMessages = st
+00016480: 6172 7443 6861 7428 290a 2020 2020 2020  artChat().      
+00016490: 2020 636f 6e66 6967 2e6d 756c 7469 6c69    config.multili
+000164a0: 6e65 496e 7075 7420 3d20 4661 6c73 650a  neInput = False.
+000164b0: 2020 2020 2020 2020 6665 6174 7572 6573          features
+000164c0: 4c6f 7765 7220 3d20 6c69 7374 2873 656c  Lower = list(sel
+000164d0: 662e 6163 7469 6f6e 732e 6b65 7973 2829  f.actions.keys()
+000164e0: 2920 2b20 5b22 2e2e 2e22 5d0a 2020 2020  ) + ["..."].    
+000164f0: 2020 2020 2320 696e 7075 7420 7375 6767      # input sugg
+00016500: 6573 7469 6f6e 730a 2020 2020 2020 2020  estions.        
+00016510: 636f 6e66 6967 2e69 6e70 7574 5375 6767  config.inputSugg
+00016520: 6573 7469 6f6e 7320 2b3d 2066 6561 7475  estions += featu
+00016530: 7265 734c 6f77 6572 0a20 2020 2020 2020  resLower.       
+00016540: 2063 6f6d 706c 6574 6572 203d 2046 757a   completer = Fuz
+00016550: 7a79 436f 6d70 6c65 7465 7228 576f 7264  zyCompleter(Word
+00016560: 436f 6d70 6c65 7465 7228 636f 6e66 6967  Completer(config
+00016570: 2e69 6e70 7574 5375 6767 6573 7469 6f6e  .inputSuggestion
+00016580: 732c 2069 676e 6f72 655f 6361 7365 3d54  s, ignore_case=T
+00016590: 7275 6529 2920 6966 2063 6f6e 6669 672e  rue)) if config.
+000165a0: 696e 7075 7453 7567 6765 7374 696f 6e73  inputSuggestions
+000165b0: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
+000165c0: 2020 2063 6f6d 706c 6574 6572 5f64 6576     completer_dev
+000165d0: 656c 6f70 6572 203d 2046 757a 7a79 436f  eloper = FuzzyCo
+000165e0: 6d70 6c65 7465 7228 576f 7264 436f 6d70  mpleter(WordComp
+000165f0: 6c65 7465 7228 636f 6e66 6967 2e69 6e70  leter(config.inp
+00016600: 7574 5375 6767 6573 7469 6f6e 735b 3a5d  utSuggestions[:]
+00016610: 202b 205b 6622 636f 6e66 6967 2e7b 697d   + [f"config.{i}
+00016620: 2220 666f 7220 6920 696e 2064 6972 2863  " for i in dir(c
+00016630: 6f6e 6669 6729 2069 6620 6e6f 7420 692e  onfig) if not i.
+00016640: 7374 6172 7473 7769 7468 2822 5f5f 2229  startswith("__")
+00016650: 5d20 2b20 7365 6c66 2e67 6574 4469 7265  ] + self.getDire
+00016660: 6374 6f72 794c 6973 7428 292c 2069 676e  ctoryList(), ign
+00016670: 6f72 655f 6361 7365 3d54 7275 6529 290a  ore_case=True)).
+00016680: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
+00016690: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+000166a0: 2320 6465 6661 756c 7420 746f 6f6c 6261  # default toolba
+000166b0: 7220 7465 7874 0a20 2020 2020 2020 2020  r text.         
+000166c0: 2020 2063 6f6e 6669 672e 6479 6e61 6d69     config.dynami
+000166d0: 6354 6f6f 6c42 6172 5465 7874 203d 2066  cToolBarText = f
+000166e0: 2222 2220 7b73 7472 2863 6f6e 6669 672e  """ {str(config.
+000166f0: 686f 746b 6579 5f65 7869 7429 2e72 6570  hotkey_exit).rep
+00016700: 6c61 6365 2822 2722 2c20 2222 297d 2065  lace("'", "")} e
+00016710: 7869 7420 7b73 7472 2863 6f6e 6669 672e  xit {str(config.
+00016720: 686f 746b 6579 5f64 6973 706c 6179 5f6b  hotkey_display_k
+00016730: 6579 5f63 6f6d 626f 292e 7265 706c 6163  ey_combo).replac
+00016740: 6528 2227 222c 2022 2229 7d20 7368 6f72  e("'", "")} shor
+00016750: 7463 7574 7320 2222 220a 2020 2020 2020  tcuts """.      
+00016760: 2020 2020 2020 2320 6469 7370 6c61 7920        # display 
+00016770: 6375 7272 656e 7420 6469 7265 6374 6f72  current director
+00016780: 7920 6966 2063 6861 6e67 6564 0a20 2020  y if changed.   
+00016790: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000167a0: 4469 7265 6374 6f72 7920 3d20 6f73 2e67  Directory = os.g
+000167b0: 6574 6377 6428 290a 2020 2020 2020 2020  etcwd().        
+000167c0: 2020 2020 6966 206e 6f74 2063 7572 7265      if not curre
+000167d0: 6e74 4469 7265 6374 6f72 7920 3d3d 2073  ntDirectory == s
+000167e0: 746f 7261 6765 6469 7265 6374 6f72 793a  toragedirectory:
+000167f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016800: 2023 7072 696e 7431 2873 656c 662e 6469   #print1(self.di
+00016810: 7669 6465 7229 0a20 2020 2020 2020 2020  vider).         
+00016820: 2020 2020 2020 2070 7269 6e74 3328 6622         print3(f"
+00016830: 4375 7272 656e 7420 6469 7265 6374 6f72  Current director
+00016840: 793a 207b 6375 7272 656e 7444 6972 6563  y: {currentDirec
+00016850: 746f 7279 7d22 290a 2020 2020 2020 2020  tory}").        
+00016860: 2020 2020 2020 2020 7072 696e 7431 2873          print1(s
+00016870: 656c 662e 6469 7669 6465 7229 0a20 2020  elf.divider).   
+00016880: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+00016890: 7261 6765 6469 7265 6374 6f72 7920 3d20  ragedirectory = 
+000168a0: 6375 7272 656e 7444 6972 6563 746f 7279  currentDirectory
+000168b0: 0a20 2020 2020 2020 2020 2020 2023 2064  .            # d
+000168c0: 6566 6175 6c74 2069 6e70 7574 2065 6e74  efault input ent
+000168d0: 7279 0a20 2020 2020 2020 2020 2020 2061  ry.            a
+000168e0: 6363 6570 745f 6465 6661 756c 7420 3d20  ccept_default = 
+000168f0: 636f 6e66 6967 2e61 6363 6570 745f 6465  config.accept_de
+00016900: 6661 756c 740a 2020 2020 2020 2020 2020  fault.          
+00016910: 2020 636f 6e66 6967 2e61 6363 6570 745f    config.accept_
+00016920: 6465 6661 756c 7420 3d20 4661 6c73 650a  default = False.
+00016930: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00016940: 756c 7445 6e74 7279 203d 2063 6f6e 6669  ultEntry = confi
+00016950: 672e 6465 6661 756c 7445 6e74 7279 0a20  g.defaultEntry. 
+00016960: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+00016970: 2e70 6174 682e 6973 6669 6c65 2864 6566  .path.isfile(def
+00016980: 6175 6c74 456e 7472 7929 3a0a 2020 2020  aultEntry):.    
+00016990: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+000169a0: 756c 7445 6e74 7279 203d 2066 2746 696c  ultEntry = f'Fil
+000169b0: 653a 2022 7b64 6566 6175 6c74 456e 7472  e: "{defaultEntr
+000169c0: 797d 225c 6e27 0a20 2020 2020 2020 2020  y}"\n'.         
+000169d0: 2020 2065 6c69 6620 6f73 2e70 6174 682e     elif os.path.
+000169e0: 6973 6469 7228 6465 6661 756c 7445 6e74  isdir(defaultEnt
+000169f0: 7279 293a 0a20 2020 2020 2020 2020 2020  ry):.           
+00016a00: 2020 2020 2064 6566 6175 6c74 456e 7472       defaultEntr
+00016a10: 7920 3d20 6627 466f 6c64 6572 3a20 227b  y = f'Folder: "{
+00016a20: 6465 6661 756c 7445 6e74 7279 7d22 5c6e  defaultEntry}"\n
+00016a30: 270a 2020 2020 2020 2020 2020 2020 636f  '.            co
+00016a40: 6e66 6967 2e64 6566 6175 6c74 456e 7472  nfig.defaultEntr
+00016a50: 7920 3d20 2222 0a0a 2020 2020 2020 2020  y = ""..        
+00016a60: 2020 2020 2320 7573 6572 2069 6e70 7574      # user input
+00016a70: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+00016a80: 7249 6e70 7574 203d 2073 656c 662e 7072  rInput = self.pr
+00016a90: 6f6d 7074 732e 7369 6d70 6c65 5072 6f6d  ompts.simpleProm
+00016aa0: 7074 2870 726f 6d70 7453 6573 7369 6f6e  pt(promptSession
+00016ab0: 3d73 656c 662e 7465 726d 696e 616c 5f63  =self.terminal_c
+00016ac0: 6861 745f 7365 7373 696f 6e2c 2063 6f6d  hat_session, com
+00016ad0: 706c 6574 6572 3d63 6f6d 706c 6574 6572  pleter=completer
+00016ae0: 5f64 6576 656c 6f70 6572 2069 6620 636f  _developer if co
+00016af0: 6e66 6967 2e64 6576 656c 6f70 6572 2065  nfig.developer e
+00016b00: 6c73 6520 636f 6d70 6c65 7465 722c 2064  lse completer, d
+00016b10: 6566 6175 6c74 3d64 6566 6175 6c74 456e  efault=defaultEn
+00016b20: 7472 792c 2061 6363 6570 745f 6465 6661  try, accept_defa
+00016b30: 756c 743d 6163 6365 7074 5f64 6566 6175  ult=accept_defau
+00016b40: 6c74 2c20 7661 6c69 6461 746f 723d 746f  lt, validator=to
+00016b50: 6b65 6e56 616c 6964 6174 6f72 2c20 626f  kenValidator, bo
+00016b60: 7474 6f6d 5f74 6f6f 6c62 6172 3d67 6574  ttom_toolbar=get
+00016b70: 4479 6e61 6d69 6354 6f6f 6c42 6172 290a  DynamicToolBar).
+00016b80: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00016b90: 2020 2020 2020 2020 2023 2075 7064 6174           # updat
+00016ba0: 6520 7379 7374 656d 206d 6573 7361 6765  e system message
+00016bb0: 2077 6865 6e20 7573 6572 2065 6e74 6572   when user enter
+00016bc0: 2061 206e 6577 2069 6e70 7574 0a20 2020   a new input.   
+00016bd0: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
+00016be0: 6375 7272 656e 744d 6573 7361 6765 7320  currentMessages 
+00016bf0: 3d20 7365 6c66 2e75 7064 6174 6553 7973  = self.updateSys
+00016c00: 7465 6d4d 6573 7361 6765 2863 6f6e 6669  temMessage(confi
+00016c10: 672e 6375 7272 656e 744d 6573 7361 6765  g.currentMessage
+00016c20: 7329 0a20 2020 2020 2020 2020 2020 200a  s).            .
+00016c30: 2020 2020 2020 2020 2020 2020 2320 6469              # di
+00016c40: 7370 6c61 7920 6f70 7469 6f6e 7320 7768  splay options wh
+00016c50: 656e 2065 6d70 7479 2073 7472 696e 6720  en empty string 
+00016c60: 6973 2065 6e74 6572 6564 0a20 2020 2020  is entered.     
+00016c70: 2020 2020 2020 2075 7365 7249 6e70 7574         userInput
+00016c80: 4c6f 7765 7220 3d20 7573 6572 496e 7075  Lower = userInpu
+00016c90: 742e 6c6f 7765 7228 290a 2020 2020 2020  t.lower().      
+00016ca0: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
+00016cb0: 6164 6450 6174 6841 7420 6973 206e 6f74  addPathAt is not
+00016cc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00016cd0: 2020 2020 2020 2070 7265 6669 7820 3d20         prefix = 
+00016ce0: 7573 6572 496e 7075 745b 3a63 6f6e 6669  userInput[:confi
+00016cf0: 672e 6164 6450 6174 6841 745d 0a20 2020  g.addPathAt].   
+00016d00: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00016d10: 6669 7853 706c 6974 203d 2070 7265 6669  fixSplit = prefi
+00016d20: 782e 7273 706c 6974 2822 2022 2c20 3129  x.rsplit(" ", 1)
+00016d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d40: 2069 6620 6c65 6e28 7072 6566 6978 5370   if len(prefixSp
+00016d50: 6c69 7429 203e 2031 3a0a 2020 2020 2020  lit) > 1:.      
+00016d60: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00016d70: 6661 756c 7420 3d20 7072 6566 6978 5370  fault = prefixSp
+00016d80: 6c69 745b 2d31 5d0a 2020 2020 2020 2020  lit[-1].        
+00016d90: 2020 2020 2020 2020 2020 2020 7072 6566              pref
+00016da0: 6978 203d 2066 227b 7072 6566 6978 5370  ix = f"{prefixSp
+00016db0: 6c69 745b 305d 7d20 220a 2020 2020 2020  lit[0]} ".      
+00016dc0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00016dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016de0: 2020 2020 6465 6661 756c 7420 3d20 7072      default = pr
+00016df0: 6566 6978 0a20 2020 2020 2020 2020 2020  efix.           
+00016e00: 2020 2020 2020 2020 2070 7265 6669 7820           prefix 
+00016e10: 3d20 2222 0a20 2020 2020 2020 2020 2020  = "".           
+00016e20: 2020 2020 2073 7566 6669 7820 3d20 7573       suffix = us
+00016e30: 6572 496e 7075 745b 636f 6e66 6967 2e61  erInput[config.a
+00016e40: 6464 5061 7468 4174 3a5d 0a20 2020 2020  ddPathAt:].     
+00016e50: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00016e60: 672e 6164 6450 6174 6841 7420 3d20 4e6f  g.addPathAt = No
+00016e70: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00016e80: 2020 2069 6620 6e6f 7420 6465 6661 756c     if not defaul
+00016e90: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00016ea0: 2020 2020 2020 2064 6566 6175 6c74 203d         default =
+00016eb0: 206f 732e 6765 7463 7764 2829 0a20 2020   os.getcwd().   
+00016ec0: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00016ed0: 7250 6174 6820 3d20 7365 6c66 2e67 6574  rPath = self.get
+00016ee0: 5061 7468 2e67 6574 5061 7468 286d 6573  Path.getPath(mes
+00016ef0: 7361 6765 3d66 227b 7072 6566 6978 7d3c  sage=f"{prefix}<
+00016f00: 7b63 6f6e 6669 672e 7465 726d 696e 616c  {config.terminal
+00016f10: 436f 6d6d 616e 6445 6e74 7279 436f 6c6f  CommandEntryColo
+00016f20: 7232 7d3e 5b61 6464 2061 2070 6174 6820  r2}>[add a path 
+00016f30: 6865 7265 5d3c 2f7b 636f 6e66 6967 2e74  here]</{config.t
+00016f40: 6572 6d69 6e61 6c43 6f6d 6d61 6e64 456e  erminalCommandEn
+00016f50: 7472 7943 6f6c 6f72 327d 3e7b 7375 6666  tryColor2}>{suff
+00016f60: 6978 7d22 2c20 7072 6f6d 7074 496e 6469  ix}", promptIndi
+00016f70: 6361 746f 723d 223e 3e3e 2022 2c20 656d  cator=">>> ", em
+00016f80: 7074 795f 746f 5f63 616e 6365 6c3d 5472  pty_to_cancel=Tr
+00016f90: 7565 2c20 6465 6661 756c 743d 6465 6661  ue, default=defa
+00016fa0: 756c 7429 0a20 2020 2020 2020 2020 2020  ult).           
+00016fb0: 2020 2020 2063 6f6e 6669 672e 6465 6661       config.defa
+00016fc0: 756c 7445 6e74 7279 203d 2066 227b 7072  ultEntry = f"{pr
+00016fd0: 6566 6978 7d7b 7573 6572 5061 7468 7d7b  efix}{userPath}{
+00016fe0: 7375 6666 6978 7d22 0a20 2020 2020 2020  suffix}".       
+00016ff0: 2020 2020 2020 2020 2075 7365 7249 6e70           userInp
+00017000: 7574 203d 2022 220a 2020 2020 2020 2020  ut = "".        
+00017010: 2020 2020 656c 6966 206e 6f74 2075 7365      elif not use
+00017020: 7249 6e70 7574 4c6f 7765 723a 0a20 2020  rInputLower:.   
+00017030: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00017040: 7249 6e70 7574 203d 2063 6f6e 6669 672e  rInput = config.
+00017050: 626c 616e 6b45 6e74 7279 4163 7469 6f6e  blankEntryAction
+00017060: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017070: 7573 6572 496e 7075 7420 3d3d 2022 2e2e  userInput == "..
+00017080: 2e22 3a0a 2020 2020 2020 2020 2020 2020  .":.            
+00017090: 2020 2020 7573 6572 496e 7075 7420 3d20      userInput = 
+000170a0: 7573 6572 496e 7075 744c 6f77 6572 203d  userInputLower =
+000170b0: 2073 656c 662e 7275 6e41 6374 696f 6e73   self.runActions
+000170c0: 2875 7365 7249 6e70 7574 290a 2020 2020  (userInput).    
+000170d0: 2020 2020 2020 2020 2365 6c69 6620 7573          #elif us
+000170e0: 6572 496e 7075 744c 6f77 6572 2069 6e20  erInputLower in 
+000170f0: 7475 706c 6528 7365 6c66 2e61 6374 696f  tuple(self.actio
+00017100: 6e73 2e6b 6579 7328 2929 3a0a 2020 2020  ns.keys()):.    
+00017110: 2020 2020 2020 2020 656c 6966 2075 7365          elif use
+00017120: 7249 6e70 7574 4c6f 7765 722e 7374 6172  rInputLower.star
+00017130: 7473 7769 7468 2822 2e22 2920 616e 6420  tswith(".") and 
+00017140: 6e6f 7420 7573 6572 496e 7075 744c 6f77  not userInputLow
+00017150: 6572 2069 6e20 2863 6f6e 6669 672e 6578  er in (config.ex
+00017160: 6974 5f65 6e74 7279 2c20 636f 6e66 6967  it_entry, config
+00017170: 2e63 616e 6365 6c5f 656e 7472 792c 2022  .cancel_entry, "
+00017180: 2e6e 6577 222c 2022 2e63 6f6e 7465 7874  .new", ".context
+00017190: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+000171a0: 2020 2020 7573 6572 496e 7075 7420 3d20      userInput = 
+000171b0: 7573 6572 496e 7075 744c 6f77 6572 203d  userInputLower =
+000171c0: 2073 656c 662e 7275 6e41 6374 696f 6e73   self.runActions
+000171d0: 2822 2e2e 2e22 2c20 7573 6572 496e 7075  ("...", userInpu
+000171e0: 7429 0a0a 2020 2020 2020 2020 2020 2020  t)..            
+000171f0: 6966 2073 6574 546f 6f6c 4465 7065 6e64  if setToolDepend
+00017200: 656e 6365 2875 7365 7249 6e70 7574 293a  ence(userInput):
+00017210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017220: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
+00017230: 2020 2020 2020 2023 2072 6570 6c61 6365         # replace
+00017240: 2061 6c69 6173 2c20 6966 2061 6e79 2c20   alias, if any, 
+00017250: 7769 7468 2066 756c 6c20 656e 7472 790a  with full entry.
+00017260: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00017270: 616c 6961 732c 2066 756c 6c45 6e74 7279  alias, fullEntry
+00017280: 2069 6e20 636f 6e66 6967 2e61 6c69 6173   in config.alias
+00017290: 6573 2e69 7465 6d73 2829 3a0a 2020 2020  es.items():.    
+000172a0: 2020 2020 2020 2020 2020 2020 2375 7365              #use
+000172b0: 7249 6e70 7574 203d 2072 652e 7375 6228  rInput = re.sub(
+000172c0: 616c 6961 732c 2066 756c 6c45 6e74 7279  alias, fullEntry
+000172d0: 2c20 7573 6572 496e 7075 7429 2023 2065  , userInput) # e
+000172e0: 7272 6f72 206f 6e20 5769 6e64 6f77 7320  rror on Windows 
+000172f0: 636f 7a20 6f66 2057 696e 646f 7773 2070  coz of Windows p
+00017300: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+00017310: 2020 2020 7573 6572 496e 7075 7420 3d20      userInput = 
+00017320: 7573 6572 496e 7075 742e 7265 706c 6163  userInput.replac
+00017330: 6528 616c 6961 732c 2066 756c 6c45 6e74  e(alias, fullEnt
+00017340: 7279 290a 0a20 2020 2020 2020 2020 2020  ry)..           
+00017350: 2023 206f 7065 6e20 6669 6c65 202f 2064   # open file / d
+00017360: 6972 6563 746f 7279 2064 6972 6563 746c  irectory directl
+00017370: 790a 2020 2020 2020 2020 2020 2020 646f  y.            do
+00017380: 6373 5f70 6174 6820 3d20 6973 4578 6973  cs_path = isExis
+00017390: 7469 6e67 5061 7468 2875 7365 7249 6e70  tingPath(userInp
+000173a0: 7574 290a 2020 2020 2020 2020 2020 2020  ut).            
+000173b0: 6966 206f 732e 7061 7468 2e69 7366 696c  if os.path.isfil
+000173c0: 6528 646f 6373 5f70 6174 6829 3a0a 2020  e(docs_path):.  
+000173d0: 2020 2020 2020 2020 2020 2020 2020 6f73                os
+000173e0: 2e73 7973 7465 6d28 6622 7b63 6f6e 6669  .system(f"{confi
+000173f0: 672e 6f70 656e 7d20 7b64 6f63 735f 7061  g.open} {docs_pa
+00017400: 7468 7d22 290a 2020 2020 2020 2020 2020  th}").          
+00017410: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00017420: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00017430: 6f73 2e70 6174 682e 6973 6469 7228 646f  os.path.isdir(do
+00017440: 6373 5f70 6174 6829 3a0a 2020 2020 2020  cs_path):.      
+00017450: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00017460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017470: 2020 206f 732e 6368 6469 7228 646f 6373     os.chdir(docs
+00017480: 5f70 6174 6829 0a20 2020 2020 2020 2020  _path).         
+00017490: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000174a0: 3328 6622 4469 7265 6374 6f72 7920 6368  3(f"Directory ch
+000174b0: 616e 6765 6420 746f 3a20 7b64 6f63 735f  anged to: {docs_
+000174c0: 7061 7468 7d22 290a 2020 2020 2020 2020  path}").        
+000174d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000174e0: 2e67 6574 5061 7468 2e64 6973 706c 6179  .getPath.display
+000174f0: 4469 7265 6374 6f72 7943 6f6e 7465 6e74  DirectoryContent
+00017500: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00017510: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017530: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+00017540: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00017550: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00017560: 7472 7920 6576 616c 0a20 2020 2020 2020  try eval.       
+00017570: 2020 2020 2069 6620 636f 6e66 6967 2e64       if config.d
+00017580: 6576 656c 6f70 6572 2061 6e64 206e 6f74  eveloper and not
+00017590: 2075 7365 7249 6e70 7574 203d 3d20 222e   userInput == ".
+000175a0: 2e2e 223a 0a20 2020 2020 2020 2020 2020  ..":.           
+000175b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000175c0: 2020 2020 2020 2020 2020 2020 2020 7661                va
+000175d0: 6c75 6520 3d20 6576 616c 2875 7365 7249  lue = eval(userI
+000175e0: 6e70 7574 2920 2320 6974 2073 6f6c 7665  nput) # it solve
+000175f0: 2073 696d 706c 6520 6d61 7468 2c20 652e   simple math, e.
+00017600: 672e 2031 2b31 2c20 6f72 2072 6561 6420  g. 1+1, or read 
+00017610: 7661 7269 6162 6c65 732c 2065 2e67 2e20  variables, e.g. 
+00017620: 6469 7228 636f 6e66 6967 290a 2020 2020  dir(config).    
+00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017640: 6966 2076 616c 7565 2069 7320 6e6f 7420  if value is not 
+00017650: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00017660: 2020 2020 2020 2020 2020 2020 2020 2370                #p
+00017670: 7269 6e74 2876 616c 7565 290a 2020 2020  rint(value).    
+00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017690: 2020 2020 7070 7269 6e74 2e70 7072 696e      pprint.pprin
+000176a0: 7428 7661 6c75 6529 0a20 2020 2020 2020  t(value).       
 000176b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176c0: 2020 2020 2020 2070 7269 6e74 2822 2229         print("")
-000176d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000176e0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000176f0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00017700: 2020 2020 2020 656c 6966 2072 652e 7365        elif re.se
-00017710: 6172 6368 2822 5e70 7269 6e74 5c28 5b5e  arch("^print\([^
-00017720: 5c29 5c29 5d2b 3f5c 2924 222c 2075 7365  \)\)]+?\)$", use
-00017730: 7249 6e70 7574 293a 0a20 2020 2020 2020  rInput):.       
-00017740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017750: 2070 7269 6e74 2822 2229 0a20 2020 2020   print("").     
-00017760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017770: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00017780: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00017790: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-000177a0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-000177b0: 2020 2020 2020 2020 2023 2074 7279 2074           # try t
-000177c0: 6f20 7275 6e20 6173 2061 2070 7974 686f  o run as a pytho
-000177d0: 6e20 7363 7269 7074 2066 6972 7374 0a20  n script first. 
-000177e0: 2020 2020 2020 2020 2020 2069 6620 636f             if co
-000177f0: 6e66 6967 2e64 6576 656c 6f70 6572 3a0a  nfig.developer:.
-00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017810: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00017820: 2020 2020 2020 2020 2065 7865 6328 7573           exec(us
-00017830: 6572 496e 7075 742c 2067 6c6f 6261 6c73  erInput, globals
-00017840: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-00017850: 2020 2020 2020 2020 7072 696e 7428 2222          print(""
-00017860: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00017870: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00017880: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00017890: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
-000178a0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-000178b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000178c0: 7573 6572 496e 7075 742e 7374 6172 7473  userInput.starts
-000178d0: 7769 7468 2822 2122 293a 0a20 2020 2020  with("!"):.     
-000178e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000178f0: 7275 6e53 7973 7465 6d43 6f6d 6d61 6e64  runSystemCommand
-00017900: 2875 7365 7249 6e70 7574 290a 2020 2020  (userInput).    
-00017910: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00017920: 7428 2222 290a 2020 2020 2020 2020 2020  t("").          
-00017930: 2020 656c 6966 2063 6f6e 6669 672e 6465    elif config.de
-00017940: 7665 6c6f 7065 7220 616e 6420 7573 6572  veloper and user
-00017950: 496e 7075 742e 7374 6172 7473 7769 7468  Input.startswith
-00017960: 2822 6060 6022 2920 616e 6420 7573 6572  ("```") and user
-00017970: 496e 7075 742e 656e 6473 7769 7468 2822  Input.endswith("
-00017980: 6060 6022 2920 616e 6420 6e6f 7420 7573  ```") and not us
-00017990: 6572 496e 7075 7420 3d3d 2022 6060 6060  erInput == "````
-000179a0: 6060 223a 0a20 2020 2020 2020 2020 2020  ``":.           
-000179b0: 2020 2020 2075 7365 7249 6e70 7574 203d       userInput =
-000179c0: 2072 652e 7375 6228 2260 6060 7079 7468   re.sub("```pyth
-000179d0: 6f6e 222c 2022 6060 6022 2c20 7573 6572  on", "```", user
-000179e0: 496e 7075 7429 0a20 2020 2020 2020 2020  Input).         
-000179f0: 2020 2020 2020 2073 656c 662e 7275 6e50         self.runP
-00017a00: 7974 686f 6e53 6372 6970 7428 7573 6572  ythonScript(user
-00017a10: 496e 7075 7429 0a20 2020 2020 2020 2020  Input).         
-00017a20: 2020 2020 2020 2070 7269 6e74 2822 2229         print("")
-00017a30: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00017a40: 6620 7573 6572 496e 7075 744c 6f77 6572  f userInputLower
-00017a50: 203d 3d20 636f 6e66 6967 2e65 7869 745f   == config.exit_
-00017a60: 656e 7472 793a 0a20 2020 2020 2020 2020  entry:.         
-00017a70: 2020 2020 2020 2073 656c 662e 7361 7665         self.save
-00017a80: 4368 6174 2863 6f6e 6669 672e 6375 7272  Chat(config.curr
-00017a90: 656e 744d 6573 7361 6765 7329 0a20 2020  entMessages).   
-00017aa0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00017ab0: 7572 6e20 7365 6c66 2e65 7869 7441 6374  urn self.exitAct
-00017ac0: 696f 6e28 290a 2020 2020 2020 2020 2020  ion().          
-00017ad0: 2020 656c 6966 2075 7365 7249 6e70 7574    elif userInput
-00017ae0: 4c6f 7765 7220 3d3d 2063 6f6e 6669 672e  Lower == config.
-00017af0: 6361 6e63 656c 5f65 6e74 7279 3a0a 2020  cancel_entry:.  
-00017b00: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00017b10: 7373 0a20 2020 2020 2020 2020 2020 2065  ss.            e
-00017b20: 6c69 6620 7573 6572 496e 7075 744c 6f77  lif userInputLow
-00017b30: 6572 203d 3d20 222e 636f 6e74 6578 7422  er == ".context"
-00017b40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017b50: 2020 7365 6c66 2e63 6861 6e67 6543 6f6e    self.changeCon
-00017b60: 7465 7874 2829 0a20 2020 2020 2020 2020  text().         
-00017b70: 2020 2020 2020 2069 6620 6e6f 7420 636f         if not co
-00017b80: 6e66 6967 2e61 7070 6c79 5072 6564 6566  nfig.applyPredef
-00017b90: 696e 6564 436f 6e74 6578 7441 6c77 6179  inedContextAlway
-00017ba0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00017bb0: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
-00017bc0: 2e63 6f6e 7665 7273 6174 696f 6e53 7461  .conversationSta
-00017bd0: 7274 6564 3a0a 2020 2020 2020 2020 2020  rted:.          
-00017be0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017bf0: 6c66 2e73 6176 6543 6861 7428 636f 6e66  lf.saveChat(conf
-00017c00: 6967 2e63 7572 7265 6e74 4d65 7373 6167  ig.currentMessag
-00017c10: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
-00017c20: 2020 2020 2020 2020 7374 6f72 6167 6564          storaged
-00017c30: 6972 6563 746f 7279 2c20 636f 6e66 6967  irectory, config
-00017c40: 2e63 7572 7265 6e74 4d65 7373 6167 6573  .currentMessages
-00017c50: 203d 2073 7461 7274 4368 6174 2829 0a20   = startChat(). 
-00017c60: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00017c70: 7573 6572 496e 7075 744c 6f77 6572 203d  userInputLower =
-00017c80: 3d20 222e 6e65 7722 3a0a 2020 2020 2020  = ".new":.      
-00017c90: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00017ca0: 6176 6543 6861 7428 636f 6e66 6967 2e63  aveChat(config.c
-00017cb0: 7572 7265 6e74 4d65 7373 6167 6573 290a  urrentMessages).
-00017cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cd0: 7374 6f72 6167 6564 6972 6563 746f 7279  storagedirectory
-00017ce0: 2c20 636f 6e66 6967 2e63 7572 7265 6e74  , config.current
-00017cf0: 4d65 7373 6167 6573 203d 2073 7461 7274  Messages = start
-00017d00: 4368 6174 2829 0a20 2020 2020 2020 2020  Chat().         
-00017d10: 2020 2065 6c69 6620 7573 6572 496e 7075     elif userInpu
-00017d20: 7420 616e 6420 6e6f 7420 7573 6572 496e  t and not userIn
-00017d30: 7075 744c 6f77 6572 2069 6e20 6665 6174  putLower in feat
-00017d40: 7572 6573 4c6f 7765 723a 0a20 2020 2020  uresLower:.     
-00017d50: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d70: 2020 2020 6966 2075 7365 7249 6e70 7574      if userInput
-00017d80: 2061 6e64 2063 6f6e 6669 672e 7474 7349   and config.ttsI
-00017d90: 6e70 7574 3a0a 2020 2020 2020 2020 2020  nput:.          
-00017da0: 2020 2020 2020 2020 2020 2020 2020 5454                TT
-00017db0: 5355 7469 6c2e 706c 6179 2875 7365 7249  SUtil.play(userI
-00017dc0: 6e70 7574 290a 2020 2020 2020 2020 2020  nput).          
-00017dd0: 2020 2020 2020 2020 2020 2320 4665 6174            # Feat
-00017de0: 7572 653a 2069 6d70 726f 7665 2077 7269  ure: improve wri
-00017df0: 7469 6e67 3a0a 2020 2020 2020 2020 2020  ting:.          
-00017e00: 2020 2020 2020 2020 2020 7370 6563 6961            specia
-00017e10: 6c45 6e74 7279 5061 7474 6572 6e20 3d20  lEntryPattern = 
-00017e20: 225c 5b54 4f4f 4c5f 5b5e 5c5b 5c5d 5d2a  "\[TOOL_[^\[\]]*
-00017e30: 3f5c 5d7c 5c5b 4e4f 5f54 4f4f 4c5c 5d7c  ?\]|\[NO_TOOL\]|
-00017e40: 5c5b 4e4f 5f53 4352 4545 4e49 4e47 5c5d  \[NO_SCREENING\]
-00017e50: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00017e60: 2020 2020 2020 7370 6563 6961 6c45 6e74        specialEnt
-00017e70: 7279 203d 2072 652e 7365 6172 6368 2873  ry = re.search(s
-00017e80: 7065 6369 616c 456e 7472 7950 6174 7465  pecialEntryPatte
-00017e90: 726e 2c20 7573 6572 496e 7075 7429 0a20  rn, userInput). 
-00017ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017eb0: 2020 2073 7065 6369 616c 456e 7472 7920     specialEntry 
-00017ec0: 3d20 7370 6563 6961 6c45 6e74 7279 2e67  = specialEntry.g
-00017ed0: 726f 7570 2830 2920 6966 2073 7065 6369  roup(0) if speci
-00017ee0: 616c 456e 7472 7920 656c 7365 2022 220a  alEntry else "".
-00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f00: 2020 2020 7573 6572 496e 7075 7420 3d20      userInput = 
-00017f10: 7265 2e73 7562 2873 7065 6369 616c 456e  re.sub(specialEn
-00017f20: 7472 7950 6174 7465 726e 2c20 2222 2c20  tryPattern, "", 
-00017f30: 7573 6572 496e 7075 7429 2023 2072 656d  userInput) # rem
-00017f40: 6f76 6520 7370 6563 6961 6c20 656e 7472  ove special entr
-00017f50: 7920 7465 6d70 6f72 6172 696c 790a 2020  y temporarily.  
-00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f70: 2020 6966 2075 7365 7249 6e70 7574 2061    if userInput a
-00017f80: 6e64 2063 6f6e 6669 672e 6469 7370 6c61  nd config.displa
-00017f90: 7949 6d70 726f 7665 6457 7269 7469 6e67  yImprovedWriting
-00017fa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017fb0: 2020 2020 2020 2020 2020 7573 6572 496e            userIn
-00017fc0: 7075 7420 3d20 7265 2e73 7562 2822 5c6e  put = re.sub("\n
-00017fd0: 5c5b 4375 7272 656e 7420 7469 6d65 3a20  \[Current time: 
-00017fe0: 5b5e 5c6e 5d2a 3f24 222c 2022 222c 2075  [^\n]*?$", "", u
-00017ff0: 7365 7249 6e70 7574 290a 2020 2020 2020  serInput).      
-00018000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018010: 2020 6966 2063 6f6e 6669 672e 6973 5465    if config.isTe
-00018020: 726d 7578 3a0a 2020 2020 2020 2020 2020  rmux:.          
-00018030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018040: 2020 6461 795f 6f66 5f77 6565 6b20 3d20    day_of_week = 
-00018050: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
-00018060: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00018070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018080: 2020 2020 2020 2020 2020 2020 2064 6179               day
-00018090: 5f6f 665f 7765 656b 203d 2066 2274 6f64  _of_week = f"tod
-000180a0: 6179 2069 7320 7b67 6574 4461 794f 6657  ay is {getDayOfW
-000180b0: 6565 6b28 297d 2061 6e64 2022 0a20 2020  eek()} and ".   
-000180c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180d0: 2020 2020 2069 6d70 726f 7665 6456 6572       improvedVer
-000180e0: 7369 6f6e 203d 2043 616c 6c4c 4c4d 2e67  sion = CallLLM.g
-000180f0: 6574 5369 6e67 6c65 4368 6174 5265 7370  etSingleChatResp
-00018100: 6f6e 7365 2866 2222 2249 6d70 726f 7665  onse(f"""Improve
-00018110: 2074 6865 2066 6f6c 6c6f 7769 6e67 2077   the following w
-00018120: 7269 7469 6e67 2c20 6163 636f 7264 696e  riting, accordin
-00018130: 6720 746f 207b 636f 6e66 6967 2e69 6d70  g to {config.imp
-00018140: 726f 7665 6457 7269 7469 6e67 5379 746c  rovedWritingSytl
-00018150: 657d 0a49 6e20 6164 6469 7469 6f6e 2c20  e}.In addition, 
-00018160: 4920 776f 756c 6420 6c69 6b65 2079 6f75  I would like you
-00018170: 2074 6f20 6865 6c70 206d 6520 7769 7468   to help me with
-00018180: 2063 6f6e 7665 7274 696e 6720 7265 6c61   converting rela
-00018190: 7469 7665 2064 6174 6573 2061 6e64 2074  tive dates and t
-000181a0: 696d 6573 2c20 6966 2061 6e79 2c20 696e  imes, if any, in
-000181b0: 746f 2065 7861 6374 2064 6174 6573 2061  to exact dates a
-000181c0: 6e64 2074 696d 6573 2062 6173 6564 206f  nd times based o
-000181d0: 6e20 7468 6520 7265 6665 7265 6e63 6520  n the reference 
-000181e0: 7468 6174 207b 6461 795f 6f66 5f77 6565  that {day_of_wee
-000181f0: 6b7d 6375 7272 656e 7420 6461 7465 7469  k}current dateti
-00018200: 6d65 2069 7320 7b73 7472 2864 6174 6574  me is {str(datet
-00018210: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
-00018220: 2829 297d 2e0a 5265 6d65 6d62 6572 2c20  ())}..Remember, 
-00018230: 7072 6f76 6964 6520 6d65 2077 6974 6820  provide me with 
-00018240: 7468 6520 696d 7072 6f76 6564 2077 7269  the improved wri
-00018250: 7469 6e67 206f 6e6c 792c 2065 6e63 6c6f  ting only, enclo
-00018260: 7365 6420 696e 2074 7269 706c 6520 7175  sed in triple qu
-00018270: 6f74 6573 2060 6060 2061 6e64 2077 6974  otes ``` and wit
-00018280: 686f 7574 2061 6e79 2061 6464 6974 696f  hout any additio
-00018290: 6e61 6c20 696e 666f 726d 6174 696f 6e20  nal information 
-000182a0: 6f72 2063 6f6d 6d65 6e74 732e 0a4d 7920  or comments..My 
-000182b0: 7772 6974 696e 673a 0a7b 7573 6572 496e  writing:.{userIn
-000182c0: 7075 747d 2222 2229 0a20 2020 2020 2020  put}""").       
-000182d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182e0: 2069 6620 696d 7072 6f76 6564 5665 7273   if improvedVers
-000182f0: 696f 6e20 616e 6420 696d 7072 6f76 6564  ion and improved
-00018300: 5665 7273 696f 6e2e 7374 6172 7473 7769  Version.startswi
-00018310: 7468 2822 6060 6022 2920 616e 6420 696d  th("```") and im
-00018320: 7072 6f76 6564 5665 7273 696f 6e2e 656e  provedVersion.en
-00018330: 6473 7769 7468 2822 6060 6022 293a 0a20  dswith("```"):. 
+000176c0: 2070 7269 6e74 2822 2229 0a20 2020 2020   print("").     
+000176d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176e0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+000176f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017700: 656c 6966 2072 652e 7365 6172 6368 2822  elif re.search("
+00017710: 5e70 7269 6e74 5c28 5b5e 5c29 5c29 5d2b  ^print\([^\)\)]+
+00017720: 3f5c 2924 222c 2075 7365 7249 6e70 7574  ?\)$", userInput
+00017730: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00017740: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00017750: 2822 2229 0a20 2020 2020 2020 2020 2020  ("").           
+00017760: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00017770: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+00017780: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177a0: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
+000177b0: 2020 2023 2074 7279 2074 6f20 7275 6e20     # try to run 
+000177c0: 6173 2061 2070 7974 686f 6e20 7363 7269  as a python scri
+000177d0: 7074 2066 6972 7374 0a20 2020 2020 2020  pt first.       
+000177e0: 2020 2020 2069 6620 636f 6e66 6967 2e64       if config.d
+000177f0: 6576 656c 6f70 6572 3a0a 2020 2020 2020  eveloper:.      
+00017800: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017820: 2020 2065 7865 6328 7573 6572 496e 7075     exec(userInpu
+00017830: 742c 2067 6c6f 6261 6c73 2829 290a 2020  t, globals()).  
+00017840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017850: 2020 7072 696e 7428 2222 290a 2020 2020    print("").    
+00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017870: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+00017880: 2020 2020 2020 2020 2065 7863 6570 743a           except:
+00017890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000178a0: 2020 2020 2070 6173 730a 0a20 2020 2020       pass..     
+000178b0: 2020 2020 2020 2069 6620 7573 6572 496e         if userIn
+000178c0: 7075 742e 7374 6172 7473 7769 7468 2822  put.startswith("
+000178d0: 2122 293a 0a20 2020 2020 2020 2020 2020  !"):.           
+000178e0: 2020 2020 2073 656c 662e 7275 6e53 7973       self.runSys
+000178f0: 7465 6d43 6f6d 6d61 6e64 2875 7365 7249  temCommand(userI
+00017900: 6e70 7574 290a 2020 2020 2020 2020 2020  nput).          
+00017910: 2020 2020 2020 7072 696e 7428 2222 290a        print("").
+00017920: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00017930: 2063 6f6e 6669 672e 6465 7665 6c6f 7065   config.develope
+00017940: 7220 616e 6420 7573 6572 496e 7075 742e  r and userInput.
+00017950: 7374 6172 7473 7769 7468 2822 6060 6022  startswith("```"
+00017960: 2920 616e 6420 7573 6572 496e 7075 742e  ) and userInput.
+00017970: 656e 6473 7769 7468 2822 6060 6022 2920  endswith("```") 
+00017980: 616e 6420 6e6f 7420 7573 6572 496e 7075  and not userInpu
+00017990: 7420 3d3d 2022 6060 6060 6060 223a 0a20  t == "``````":. 
+000179a0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+000179b0: 7365 7249 6e70 7574 203d 2072 652e 7375  serInput = re.su
+000179c0: 6228 2260 6060 7079 7468 6f6e 222c 2022  b("```python", "
+000179d0: 6060 6022 2c20 7573 6572 496e 7075 7429  ```", userInput)
+000179e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000179f0: 2073 656c 662e 7275 6e50 7974 686f 6e53   self.runPythonS
+00017a00: 6372 6970 7428 7573 6572 496e 7075 7429  cript(userInput)
+00017a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017a20: 2070 7269 6e74 2822 2229 0a20 2020 2020   print("").     
+00017a30: 2020 2020 2020 2065 6c69 6620 7573 6572         elif user
+00017a40: 496e 7075 744c 6f77 6572 203d 3d20 636f  InputLower == co
+00017a50: 6e66 6967 2e65 7869 745f 656e 7472 793a  nfig.exit_entry:
+00017a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017a70: 2073 656c 662e 7361 7665 4368 6174 2863   self.saveChat(c
+00017a80: 6f6e 6669 672e 6375 7272 656e 744d 6573  onfig.currentMes
+00017a90: 7361 6765 7329 0a20 2020 2020 2020 2020  sages).         
+00017aa0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00017ab0: 6c66 2e65 7869 7441 6374 696f 6e28 290a  lf.exitAction().
+00017ac0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00017ad0: 2075 7365 7249 6e70 7574 4c6f 7765 7220   userInputLower 
+00017ae0: 3d3d 2063 6f6e 6669 672e 6361 6e63 656c  == config.cancel
+00017af0: 5f65 6e74 7279 3a0a 2020 2020 2020 2020  _entry:.        
+00017b00: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+00017b10: 2020 2020 2020 2020 2065 6c69 6620 7573           elif us
+00017b20: 6572 496e 7075 744c 6f77 6572 203d 3d20  erInputLower == 
+00017b30: 222e 636f 6e74 6578 7422 3a0a 2020 2020  ".context":.    
+00017b40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017b50: 2e63 6861 6e67 6543 6f6e 7465 7874 2829  .changeContext()
+00017b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017b70: 2069 6620 6e6f 7420 636f 6e66 6967 2e61   if not config.a
+00017b80: 7070 6c79 5072 6564 6566 696e 6564 436f  pplyPredefinedCo
+00017b90: 6e74 6578 7441 6c77 6179 733a 0a20 2020  ntextAlways:.   
+00017ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bb0: 2069 6620 636f 6e66 6967 2e63 6f6e 7665   if config.conve
+00017bc0: 7273 6174 696f 6e53 7461 7274 6564 3a0a  rsationStarted:.
+00017bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017be0: 2020 2020 2020 2020 7365 6c66 2e73 6176          self.sav
+00017bf0: 6543 6861 7428 636f 6e66 6967 2e63 7572  eChat(config.cur
+00017c00: 7265 6e74 4d65 7373 6167 6573 290a 2020  rentMessages).  
+00017c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c20: 2020 7374 6f72 6167 6564 6972 6563 746f    storagedirecto
+00017c30: 7279 2c20 636f 6e66 6967 2e63 7572 7265  ry, config.curre
+00017c40: 6e74 4d65 7373 6167 6573 203d 2073 7461  ntMessages = sta
+00017c50: 7274 4368 6174 2829 0a20 2020 2020 2020  rtChat().       
+00017c60: 2020 2020 2065 6c69 6620 7573 6572 496e       elif userIn
+00017c70: 7075 744c 6f77 6572 203d 3d20 222e 6e65  putLower == ".ne
+00017c80: 7722 3a0a 2020 2020 2020 2020 2020 2020  w":.            
+00017c90: 2020 2020 7365 6c66 2e73 6176 6543 6861      self.saveCha
+00017ca0: 7428 636f 6e66 6967 2e63 7572 7265 6e74  t(config.current
+00017cb0: 4d65 7373 6167 6573 290a 2020 2020 2020  Messages).      
+00017cc0: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
+00017cd0: 6564 6972 6563 746f 7279 2c20 636f 6e66  edirectory, conf
+00017ce0: 6967 2e63 7572 7265 6e74 4d65 7373 6167  ig.currentMessag
+00017cf0: 6573 203d 2073 7461 7274 4368 6174 2829  es = startChat()
+00017d00: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00017d10: 6620 7573 6572 496e 7075 7420 616e 6420  f userInput and 
+00017d20: 6e6f 7420 7573 6572 496e 7075 744c 6f77  not userInputLow
+00017d30: 6572 2069 6e20 6665 6174 7572 6573 4c6f  er in featuresLo
+00017d40: 7765 723a 0a20 2020 2020 2020 2020 2020  wer:.           
+00017d50: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00017d60: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00017d70: 2075 7365 7249 6e70 7574 2061 6e64 2063   userInput and c
+00017d80: 6f6e 6669 672e 7474 7349 6e70 7574 3a0a  onfig.ttsInput:.
+00017d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017da0: 2020 2020 2020 2020 5454 5355 7469 6c2e          TTSUtil.
+00017db0: 706c 6179 2875 7365 7249 6e70 7574 290a  play(userInput).
+00017dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017dd0: 2020 2020 2320 4665 6174 7572 653a 2069      # Feature: i
+00017de0: 6d70 726f 7665 2077 7269 7469 6e67 3a0a  mprove writing:.
+00017df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e00: 2020 2020 7370 6563 6961 6c45 6e74 7279      specialEntry
+00017e10: 5061 7474 6572 6e20 3d20 225c 5b54 4f4f  Pattern = "\[TOO
+00017e20: 4c5f 5b5e 5c5b 5c5d 5d2a 3f5c 5d7c 5c5b  L_[^\[\]]*?\]|\[
+00017e30: 4e4f 5f54 4f4f 4c5c 5d7c 5c5b 4e4f 5f53  NO_TOOL\]|\[NO_S
+00017e40: 4352 4545 4e49 4e47 5c5d 220a 2020 2020  CREENING\]".    
+00017e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e60: 7370 6563 6961 6c45 6e74 7279 203d 2072  specialEntry = r
+00017e70: 652e 7365 6172 6368 2873 7065 6369 616c  e.search(special
+00017e80: 456e 7472 7950 6174 7465 726e 2c20 7573  EntryPattern, us
+00017e90: 6572 496e 7075 7429 0a20 2020 2020 2020  erInput).       
+00017ea0: 2020 2020 2020 2020 2020 2020 2073 7065               spe
+00017eb0: 6369 616c 456e 7472 7920 3d20 7370 6563  cialEntry = spec
+00017ec0: 6961 6c45 6e74 7279 2e67 726f 7570 2830  ialEntry.group(0
+00017ed0: 2920 6966 2073 7065 6369 616c 456e 7472  ) if specialEntr
+00017ee0: 7920 656c 7365 2022 220a 2020 2020 2020  y else "".      
+00017ef0: 2020 2020 2020 2020 2020 2020 2020 7573                us
+00017f00: 6572 496e 7075 7420 3d20 7265 2e73 7562  erInput = re.sub
+00017f10: 2873 7065 6369 616c 456e 7472 7950 6174  (specialEntryPat
+00017f20: 7465 726e 2c20 2222 2c20 7573 6572 496e  tern, "", userIn
+00017f30: 7075 7429 2023 2072 656d 6f76 6520 7370  put) # remove sp
+00017f40: 6563 6961 6c20 656e 7472 7920 7465 6d70  ecial entry temp
+00017f50: 6f72 6172 696c 790a 2020 2020 2020 2020  orarily.        
+00017f60: 2020 2020 2020 2020 2020 2020 6966 2075              if u
+00017f70: 7365 7249 6e70 7574 2061 6e64 2063 6f6e  serInput and con
+00017f80: 6669 672e 6469 7370 6c61 7949 6d70 726f  fig.displayImpro
+00017f90: 7665 6457 7269 7469 6e67 3a0a 2020 2020  vedWriting:.    
+00017fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fb0: 2020 2020 7573 6572 496e 7075 7420 3d20      userInput = 
+00017fc0: 7265 2e73 7562 2822 5c6e 5c5b 4375 7272  re.sub("\n\[Curr
+00017fd0: 656e 7420 7469 6d65 3a20 5b5e 5c6e 5d2a  ent time: [^\n]*
+00017fe0: 3f24 222c 2022 222c 2075 7365 7249 6e70  ?$", "", userInp
+00017ff0: 7574 290a 2020 2020 2020 2020 2020 2020  ut).            
+00018000: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00018010: 6f6e 6669 672e 6973 5465 726d 7578 3a0a  onfig.isTermux:.
+00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018030: 2020 2020 2020 2020 2020 2020 6461 795f              day_
+00018040: 6f66 5f77 6565 6b20 3d20 2222 0a20 2020  of_week = "".   
+00018050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018060: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00018070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018080: 2020 2020 2020 2064 6179 5f6f 665f 7765         day_of_we
+00018090: 656b 203d 2066 2274 6f64 6179 2069 7320  ek = f"today is 
+000180a0: 7b67 6574 4461 794f 6657 6565 6b28 297d  {getDayOfWeek()}
+000180b0: 2061 6e64 2022 0a20 2020 2020 2020 2020   and ".         
+000180c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000180d0: 6d70 726f 7665 6456 6572 7369 6f6e 203d  mprovedVersion =
+000180e0: 2043 616c 6c4c 4c4d 2e67 6574 5369 6e67   CallLLM.getSing
+000180f0: 6c65 4368 6174 5265 7370 6f6e 7365 2866  leChatResponse(f
+00018100: 2222 2249 6d70 726f 7665 2074 6865 2066  """Improve the f
+00018110: 6f6c 6c6f 7769 6e67 2077 7269 7469 6e67  ollowing writing
+00018120: 2c20 6163 636f 7264 696e 6720 746f 207b  , according to {
+00018130: 636f 6e66 6967 2e69 6d70 726f 7665 6457  config.improvedW
+00018140: 7269 7469 6e67 5379 746c 657d 0a49 6e20  ritingSytle}.In 
+00018150: 6164 6469 7469 6f6e 2c20 4920 776f 756c  addition, I woul
+00018160: 6420 6c69 6b65 2079 6f75 2074 6f20 6865  d like you to he
+00018170: 6c70 206d 6520 7769 7468 2063 6f6e 7665  lp me with conve
+00018180: 7274 696e 6720 7265 6c61 7469 7665 2064  rting relative d
+00018190: 6174 6573 2061 6e64 2074 696d 6573 2c20  ates and times, 
+000181a0: 6966 2061 6e79 2c20 696e 746f 2065 7861  if any, into exa
+000181b0: 6374 2064 6174 6573 2061 6e64 2074 696d  ct dates and tim
+000181c0: 6573 2062 6173 6564 206f 6e20 7468 6520  es based on the 
+000181d0: 7265 6665 7265 6e63 6520 7468 6174 207b  reference that {
+000181e0: 6461 795f 6f66 5f77 6565 6b7d 6375 7272  day_of_week}curr
+000181f0: 656e 7420 6461 7465 7469 6d65 2069 7320  ent datetime is 
+00018200: 7b73 7472 2864 6174 6574 696d 652e 6461  {str(datetime.da
+00018210: 7465 7469 6d65 2e6e 6f77 2829 297d 2e0a  tetime.now())}..
+00018220: 5265 6d65 6d62 6572 2c20 7072 6f76 6964  Remember, provid
+00018230: 6520 6d65 2077 6974 6820 7468 6520 696d  e me with the im
+00018240: 7072 6f76 6564 2077 7269 7469 6e67 206f  proved writing o
+00018250: 6e6c 792c 2065 6e63 6c6f 7365 6420 696e  nly, enclosed in
+00018260: 2074 7269 706c 6520 7175 6f74 6573 2060   triple quotes `
+00018270: 6060 2061 6e64 2077 6974 686f 7574 2061  `` and without a
+00018280: 6e79 2061 6464 6974 696f 6e61 6c20 696e  ny additional in
+00018290: 666f 726d 6174 696f 6e20 6f72 2063 6f6d  formation or com
+000182a0: 6d65 6e74 732e 0a4d 7920 7772 6974 696e  ments..My writin
+000182b0: 673a 0a7b 7573 6572 496e 7075 747d 2222  g:.{userInput}""
+000182c0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+000182d0: 2020 2020 2020 2020 2020 2069 6620 696d             if im
+000182e0: 7072 6f76 6564 5665 7273 696f 6e20 616e  provedVersion an
+000182f0: 6420 696d 7072 6f76 6564 5665 7273 696f  d improvedVersio
+00018300: 6e2e 7374 6172 7473 7769 7468 2822 6060  n.startswith("``
+00018310: 6022 2920 616e 6420 696d 7072 6f76 6564  `") and improved
+00018320: 5665 7273 696f 6e2e 656e 6473 7769 7468  Version.endswith
+00018330: 2822 6060 6022 293a 0a20 2020 2020 2020  ("```"):.       
 00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018350: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00018360: 3128 696d 7072 6f76 6564 5665 7273 696f  1(improvedVersio
-00018370: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00018380: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00018390: 7365 7249 6e70 7574 203d 2069 6d70 726f  serInput = impro
-000183a0: 7665 6456 6572 7369 6f6e 5b33 3a2d 335d  vedVersion[3:-3]
-000183b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000183c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000183d0: 636f 6e66 6967 2e74 7473 4f75 7470 7574  config.ttsOutput
-000183e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000183f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018400: 2020 5454 5355 7469 6c2e 706c 6179 2875    TTSUtil.play(u
-00018410: 7365 7249 6e70 7574 290a 2020 2020 2020  serInput).      
-00018420: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00018430: 2073 7065 6369 616c 456e 7472 793a 0a20   specialEntry:. 
+00018350: 2020 2020 2070 7269 6e74 3128 696d 7072       print1(impr
+00018360: 6f76 6564 5665 7273 696f 6e29 0a20 2020  ovedVersion).   
+00018370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018380: 2020 2020 2020 2020 2075 7365 7249 6e70           userInp
+00018390: 7574 203d 2069 6d70 726f 7665 6456 6572  ut = improvedVer
+000183a0: 7369 6f6e 5b33 3a2d 335d 0a20 2020 2020  sion[3:-3].     
+000183b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183c0: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
+000183d0: 2e74 7473 4f75 7470 7574 3a0a 2020 2020  .ttsOutput:.    
+000183e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183f0: 2020 2020 2020 2020 2020 2020 5454 5355              TTSU
+00018400: 7469 6c2e 706c 6179 2875 7365 7249 6e70  til.play(userInp
+00018410: 7574 290a 2020 2020 2020 2020 2020 2020  ut).            
+00018420: 2020 2020 2020 2020 6966 2073 7065 6369          if speci
+00018430: 616c 456e 7472 793a 0a20 2020 2020 2020  alEntry:.       
 00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018450: 2020 2020 2020 2075 7365 7249 6e70 7574         userInput
-00018460: 203d 2066 227b 7573 6572 496e 7075 747d   = f"{userInput}
-00018470: 7b73 7065 6369 616c 456e 7472 797d 220a  {specialEntry}".
-00018480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018490: 2020 2020 2320 7265 6669 6e65 206d 6573      # refine mes
-000184a0: 7361 6765 7320 6265 666f 7265 2072 756e  sages before run
-000184b0: 6e69 6e67 2063 6f6d 706c 6574 696f 6e0a  ning completion.
-000184c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184d0: 2020 2020 6669 6e65 5475 6e65 6455 7365      fineTunedUse
-000184e0: 7249 6e70 7574 203d 2073 656c 662e 6669  rInput = self.fi
-000184f0: 6e65 5475 6e65 5573 6572 496e 7075 7428  neTuneUserInput(
-00018500: 7573 6572 496e 7075 7429 0a20 2020 2020  userInput).     
-00018510: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00018520: 2069 6e20 6361 7365 206f 6620 7472 616e   in case of tran
-00018530: 736c 6174 696f 6e0a 2020 2020 2020 2020  slation.        
-00018540: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00018550: 6f6e 6669 672e 7072 6564 6566 696e 6564  onfig.predefined
-00018560: 436f 6e74 6578 7420 3d3d 2022 4c65 7420  Context == "Let 
-00018570: 6d65 2054 7261 6e73 6c61 7465 2220 616e  me Translate" an
-00018580: 6420 6669 6e65 5475 6e65 6455 7365 7249  d fineTunedUserI
-00018590: 6e70 7574 2e73 7461 7274 7377 6974 6828  nput.startswith(
-000185a0: 2241 7373 6973 7420 6d65 2062 7920 6163  "Assist me by ac
-000185b0: 7469 6e67 2061 7320 6120 7472 616e 736c  ting as a transl
-000185c0: 6174 6f72 2e5c 6e50 6c65 6173 6520 7472  ator.\nPlease tr
-000185d0: 616e 736c 6174 6522 293a 0a20 2020 2020  anslate"):.     
-000185e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185f0: 2020 2070 7269 6e74 3128 2250 6c65 6173     print1("Pleas
-00018600: 6520 7370 6563 6966 7920 6265 6c6f 7720  e specify below 
-00018610: 7468 6520 6c61 6e67 7561 6765 2079 6f75  the language you
-00018620: 2077 6f75 6c64 206c 696b 6520 7468 6520   would like the 
-00018630: 636f 6e74 656e 7420 746f 2062 6520 7472  content to be tr
-00018640: 616e 736c 6174 6564 2069 6e74 6f3a 2229  anslated into:")
-00018650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018660: 2020 2020 2020 2020 206c 616e 6775 6167           languag
-00018670: 6520 3d20 7365 6c66 2e70 726f 6d70 7473  e = self.prompts
-00018680: 2e73 696d 706c 6550 726f 6d70 7428 7374  .simplePrompt(st
-00018690: 796c 653d 7365 6c66 2e70 726f 6d70 7473  yle=self.prompts
-000186a0: 2e70 726f 6d70 7453 7479 6c65 322c 2064  .promptStyle2, d
-000186b0: 6566 6175 6c74 3d63 6f6e 6669 672e 7472  efault=config.tr
-000186c0: 616e 736c 6174 6554 6f4c 616e 6775 6167  anslateToLanguag
-000186d0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-000186e0: 2020 2020 2020 2020 2020 2069 6620 6c61             if la
-000186f0: 6e67 7561 6765 2061 6e64 206e 6f74 206c  nguage and not l
-00018700: 616e 6775 6167 652e 7374 7269 7028 292e  anguage.strip().
-00018710: 6c6f 7765 7228 2920 696e 2028 636f 6e66  lower() in (conf
-00018720: 6967 2e63 616e 6365 6c5f 656e 7472 792c  ig.cancel_entry,
-00018730: 2063 6f6e 6669 672e 6578 6974 5f65 6e74   config.exit_ent
-00018740: 7279 293a 0a20 2020 2020 2020 2020 2020  ry):.           
-00018750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018760: 2066 696e 6554 756e 6564 5573 6572 496e   fineTunedUserIn
-00018770: 7075 7420 3d20 6622 7b66 696e 6554 756e  put = f"{fineTun
-00018780: 6564 5573 6572 496e 7075 747d 5c6e 5c6e  edUserInput}\n\n
-00018790: 506c 6561 7365 2074 7261 6e73 6c61 7465  Please translate
-000187a0: 2074 6865 2063 6f6e 7465 6e74 2069 6e74   the content int
-000187b0: 6f20 3c6c 616e 6775 6167 653e 7b6c 616e  o <language>{lan
-000187c0: 6775 6167 657d 3c2f 6c61 6e67 7561 6765  guage}</language
-000187d0: 3e2e 220a 2020 2020 2020 2020 2020 2020  >.".            
-000187e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187f0: 636f 6e66 6967 2e74 7261 6e73 6c61 7465  config.translate
-00018800: 546f 4c61 6e67 7561 6765 203d 206c 616e  ToLanguage = lan
-00018810: 6775 6167 650a 2020 2020 2020 2020 2020  guage.          
-00018820: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00018830: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00018840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018850: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-00018860: 2020 2020 2020 2020 2020 2020 2023 2063               # c
-00018870: 6c65 6172 2063 6f6e 6669 672e 7072 6564  lear config.pred
-00018880: 6566 696e 6564 436f 6e74 6578 7454 656d  efinedContextTem
-00018890: 7020 6966 2061 6e79 0a20 2020 2020 2020  p if any.       
-000188a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000188b0: 636f 6e66 6967 2e70 7265 6465 6669 6e65  config.predefine
-000188c0: 6443 6f6e 7465 7874 5465 6d70 3a0a 2020  dContextTemp:.  
+00018450: 2075 7365 7249 6e70 7574 203d 2066 227b   userInput = f"{
+00018460: 7573 6572 496e 7075 747d 7b73 7065 6369  userInput}{speci
+00018470: 616c 456e 7472 797d 220a 2020 2020 2020  alEntry}".      
+00018480: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00018490: 7265 6669 6e65 206d 6573 7361 6765 7320  refine messages 
+000184a0: 6265 666f 7265 2072 756e 6e69 6e67 2063  before running c
+000184b0: 6f6d 706c 6574 696f 6e0a 2020 2020 2020  ompletion.      
+000184c0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+000184d0: 6e65 5475 6e65 6455 7365 7249 6e70 7574  neTunedUserInput
+000184e0: 203d 2073 656c 662e 6669 6e65 5475 6e65   = self.fineTune
+000184f0: 5573 6572 496e 7075 7428 7573 6572 496e  UserInput(userIn
+00018500: 7075 7429 0a20 2020 2020 2020 2020 2020  put).           
+00018510: 2020 2020 2020 2020 2023 2069 6e20 6361           # in ca
+00018520: 7365 206f 6620 7472 616e 736c 6174 696f  se of translatio
+00018530: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00018540: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
+00018550: 7072 6564 6566 696e 6564 436f 6e74 6578  predefinedContex
+00018560: 7420 3d3d 2022 4c65 7420 6d65 2054 7261  t == "Let me Tra
+00018570: 6e73 6c61 7465 2220 616e 6420 6669 6e65  nslate" and fine
+00018580: 5475 6e65 6455 7365 7249 6e70 7574 2e73  TunedUserInput.s
+00018590: 7461 7274 7377 6974 6828 2241 7373 6973  tartswith("Assis
+000185a0: 7420 6d65 2062 7920 6163 7469 6e67 2061  t me by acting a
+000185b0: 7320 6120 7472 616e 736c 6174 6f72 2e5c  s a translator.\
+000185c0: 6e50 6c65 6173 6520 7472 616e 736c 6174  nPlease translat
+000185d0: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
+000185e0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000185f0: 6e74 3128 2250 6c65 6173 6520 7370 6563  nt1("Please spec
+00018600: 6966 7920 6265 6c6f 7720 7468 6520 6c61  ify below the la
+00018610: 6e67 7561 6765 2079 6f75 2077 6f75 6c64  nguage you would
+00018620: 206c 696b 6520 7468 6520 636f 6e74 656e   like the conten
+00018630: 7420 746f 2062 6520 7472 616e 736c 6174  t to be translat
+00018640: 6564 2069 6e74 6f3a 2229 0a20 2020 2020  ed into:").     
+00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018660: 2020 206c 616e 6775 6167 6520 3d20 7365     language = se
+00018670: 6c66 2e70 726f 6d70 7473 2e73 696d 706c  lf.prompts.simpl
+00018680: 6550 726f 6d70 7428 7374 796c 653d 7365  ePrompt(style=se
+00018690: 6c66 2e70 726f 6d70 7473 2e70 726f 6d70  lf.prompts.promp
+000186a0: 7453 7479 6c65 322c 2064 6566 6175 6c74  tStyle2, default
+000186b0: 3d63 6f6e 6669 672e 7472 616e 736c 6174  =config.translat
+000186c0: 6554 6f4c 616e 6775 6167 6529 0a20 2020  eToLanguage).   
+000186d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186e0: 2020 2020 2069 6620 6c61 6e67 7561 6765       if language
+000186f0: 2061 6e64 206e 6f74 206c 616e 6775 6167   and not languag
+00018700: 652e 7374 7269 7028 292e 6c6f 7765 7228  e.strip().lower(
+00018710: 2920 696e 2028 636f 6e66 6967 2e63 616e  ) in (config.can
+00018720: 6365 6c5f 656e 7472 792c 2063 6f6e 6669  cel_entry, confi
+00018730: 672e 6578 6974 5f65 6e74 7279 293a 0a20  g.exit_entry):. 
+00018740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018750: 2020 2020 2020 2020 2020 2066 696e 6554             fineT
+00018760: 756e 6564 5573 6572 496e 7075 7420 3d20  unedUserInput = 
+00018770: 6622 7b66 696e 6554 756e 6564 5573 6572  f"{fineTunedUser
+00018780: 496e 7075 747d 5c6e 5c6e 506c 6561 7365  Input}\n\nPlease
+00018790: 2074 7261 6e73 6c61 7465 2074 6865 2063   translate the c
+000187a0: 6f6e 7465 6e74 2069 6e74 6f20 3c6c 616e  ontent into <lan
+000187b0: 6775 6167 653e 7b6c 616e 6775 6167 657d  guage>{language}
+000187c0: 3c2f 6c61 6e67 7561 6765 3e2e 220a 2020  </language>.".  
+000187d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187e0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+000187f0: 2e74 7261 6e73 6c61 7465 546f 4c61 6e67  .translateToLang
+00018800: 7561 6765 203d 206c 616e 6775 6167 650a  uage = language.
+00018810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018820: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018840: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00018850: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00018860: 2020 2020 2020 2023 2063 6c65 6172 2063         # clear c
+00018870: 6f6e 6669 672e 7072 6564 6566 696e 6564  onfig.predefined
+00018880: 436f 6e74 6578 7454 656d 7020 6966 2061  ContextTemp if a
+00018890: 6e79 0a20 2020 2020 2020 2020 2020 2020  ny.             
+000188a0: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
+000188b0: 2e70 7265 6465 6669 6e65 6443 6f6e 7465  .predefinedConte
+000188c0: 7874 5465 6d70 3a0a 2020 2020 2020 2020  xtTemp:.        
 000188d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188e0: 2020 2020 2020 636f 6e66 6967 2e70 7265        config.pre
-000188f0: 6465 6669 6e65 6443 6f6e 7465 7874 203d  definedContext =
-00018900: 2063 6f6e 6669 672e 7072 6564 6566 696e   config.predefin
-00018910: 6564 436f 6e74 6578 7454 656d 700a 2020  edContextTemp.  
+000188e0: 636f 6e66 6967 2e70 7265 6465 6669 6e65  config.predefine
+000188f0: 6443 6f6e 7465 7874 203d 2063 6f6e 6669  dContext = confi
+00018900: 672e 7072 6564 6566 696e 6564 436f 6e74  g.predefinedCont
+00018910: 6578 7454 656d 700a 2020 2020 2020 2020  extTemp.        
 00018920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018930: 2020 2020 2020 636f 6e66 6967 2e70 7265        config.pre
-00018940: 6465 6669 6e65 6443 6f6e 7465 7874 5465  definedContextTe
-00018950: 6d70 203d 2022 220a 2020 2020 2020 2020  mp = "".        
-00018960: 2020 2020 2020 2020 2020 2020 2320 656d              # em
-00018970: 7074 7920 636f 6e66 6967 2e70 6167 6572  pty config.pager
-00018980: 436f 6e74 656e 740a 2020 2020 2020 2020  Content.        
-00018990: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-000189a0: 6967 2e70 6167 6572 436f 6e74 656e 7420  ig.pagerContent 
-000189b0: 3d20 2222 0a0a 2020 2020 2020 2020 2020  = ""..          
-000189c0: 2020 2020 2020 2020 2020 2320 6368 6563            # chec
-000189d0: 6b20 7370 6563 6961 6c20 656e 7472 6965  k special entrie
-000189e0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-000189f0: 2020 2020 2020 2320 6966 2075 7365 7220        # if user 
-00018a00: 6361 6c6c 2061 2063 6861 7462 6f74 2077  call a chatbot w
-00018a10: 6974 686f 7574 2066 756e 6374 696f 6e20  ithout function 
-00018a20: 6361 6c6c 696e 670a 2020 2020 2020 2020  calling.        
-00018a30: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-00018a40: 5b43 4841 545d 2220 696e 2066 696e 6554  [CHAT]" in fineT
-00018a50: 756e 6564 5573 6572 496e 7075 743a 0a20  unedUserInput:. 
+00018930: 636f 6e66 6967 2e70 7265 6465 6669 6e65  config.predefine
+00018940: 6443 6f6e 7465 7874 5465 6d70 203d 2022  dContextTemp = "
+00018950: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00018960: 2020 2020 2020 2320 656d 7074 7920 636f        # empty co
+00018970: 6e66 6967 2e70 6167 6572 436f 6e74 656e  nfig.pagerConten
+00018980: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00018990: 2020 2020 2020 636f 6e66 6967 2e70 6167        config.pag
+000189a0: 6572 436f 6e74 656e 7420 3d20 2222 0a0a  erContent = ""..
+000189b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189c0: 2020 2020 2320 6368 6563 6b20 7370 6563      # check spec
+000189d0: 6961 6c20 656e 7472 6965 730a 2020 2020  ial entries.    
+000189e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189f0: 2320 6966 2075 7365 7220 6361 6c6c 2061  # if user call a
+00018a00: 2063 6861 7462 6f74 2077 6974 686f 7574   chatbot without
+00018a10: 2066 756e 6374 696f 6e20 6361 6c6c 696e   function callin
+00018a20: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+00018a30: 2020 2020 2020 6966 2022 5b43 4841 545d        if "[CHAT]
+00018a40: 2220 696e 2066 696e 6554 756e 6564 5573  " in fineTunedUs
+00018a50: 6572 496e 7075 743a 0a20 2020 2020 2020  erInput:.       
 00018a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a70: 2020 2020 2020 2063 6861 7462 6f74 203d         chatbot =
-00018a80: 2063 6f6e 6669 672e 6c6c 6d49 6e74 6572   config.llmInter
-00018a90: 6661 6365 0a20 2020 2020 2020 2020 2020  face.           
-00018aa0: 2020 2020 2020 2020 2065 6c69 6620 6361           elif ca
-00018ab0: 6c6c 4368 6174 426f 7420 3a3d 2072 652e  llChatBot := re.
-00018ac0: 7365 6172 6368 2822 5c5b 4348 4154 5f28  search("\[CHAT_(
-00018ad0: 5b5e 5c5b 5c5d 5d2b 3f29 5c5d 222c 2066  [^\[\]]+?)\]", f
-00018ae0: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
-00018af0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00018b00: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-00018b10: 626f 7420 3d20 6361 6c6c 4368 6174 426f  bot = callChatBo
-00018b20: 742e 6772 6f75 7028 3129 2e6c 6f77 6572  t.group(1).lower
-00018b30: 2829 2069 6620 6361 6c6c 4368 6174 426f  () if callChatBo
-00018b40: 7420 616e 6420 6361 6c6c 4368 6174 426f  t and callChatBo
-00018b50: 742e 6772 6f75 7028 3129 2e6c 6f77 6572  t.group(1).lower
-00018b60: 2829 2069 6e20 2822 6368 6174 6770 7422  () in ("chatgpt"
-00018b70: 2c20 2267 656d 696e 6970 726f 222c 2022  , "geminipro", "
-00018b80: 7061 6c6d 3222 2c20 2263 6f64 6579 2229  palm2", "codey")
-00018b90: 2065 6c73 6520 2222 0a20 2020 2020 2020   else "".       
-00018ba0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00018bb0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00018bc0: 2020 2020 2020 2020 2020 2063 6861 7462             chatb
-00018bd0: 6f74 203d 2022 220a 2020 2020 2020 2020  ot = "".        
-00018be0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00018bf0: 6861 7462 6f74 3a0a 2020 2020 2020 2020  hatbot:.        
-00018c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c10: 2320 6361 6c6c 2074 6865 2073 7063 6966  # call the spcif
-00018c20: 6965 6420 6368 6174 626f 7420 746f 2063  ied chatbot to c
-00018c30: 6f6e 7469 6e75 6520 7468 6520 636f 6e76  ontinue the conv
-00018c40: 6572 7361 7469 6f6e 0a20 2020 2020 2020  ersation.       
-00018c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c60: 2066 696e 6554 756e 6564 5573 6572 496e   fineTunedUserIn
-00018c70: 7075 7420 3d20 7265 2e73 7562 2822 5c5b  put = re.sub("\[
-00018c80: 4348 4154 5c5d 7c5c 5b43 4841 545f 5b5e  CHAT\]|\[CHAT_[^
-00018c90: 5c5b 5c5d 5d2b 3f5c 5d22 2c20 2222 2c20  \[\]]+?\]", "", 
-00018ca0: 6669 6e65 5475 6e65 6455 7365 7249 6e70  fineTunedUserInp
-00018cb0: 7574 290a 2020 2020 2020 2020 2020 2020  ut).            
-00018cc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018cd0: 2e6c 6175 6e63 6843 6861 7462 6f74 2863  .launchChatbot(c
-00018ce0: 6861 7462 6f74 2c20 6669 6e65 5475 6e65  hatbot, fineTune
-00018cf0: 6455 7365 7249 6e70 7574 290a 2020 2020  dUserInput).    
-00018d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d10: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-00018d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d30: 2023 2077 6865 6e20 7573 6572 2064 6f6e   # when user don
-00018d40: 2774 2077 616e 7420 6120 6675 6e63 7469  't want a functi
-00018d50: 6f6e 2063 616c 6c0a 2020 2020 2020 2020  on call.        
-00018d60: 2020 2020 2020 2020 2020 2020 6e6f 4675              noFu
-00018d70: 6e63 7469 6f6e 4361 6c6c 203d 2028 225b  nctionCall = ("[
-00018d80: 4e4f 5f54 4f4f 4c5d 2220 696e 2066 696e  NO_TOOL]" in fin
-00018d90: 6554 756e 6564 5573 6572 496e 7075 7429  eTunedUserInput)
-00018da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018db0: 2020 2020 2023 2077 6865 6e20 7573 6572       # when user
-00018dc0: 2077 616e 7420 746f 2063 616c 6c20 6120   want to call a 
-00018dd0: 7061 7274 6963 756c 6172 2066 756e 6374  particular funct
-00018de0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00018df0: 2020 2020 2020 2020 6368 6563 6b43 616c          checkCal
-00018e00: 6c53 7065 6369 6669 6346 756e 6374 696f  lSpecificFunctio
-00018e10: 6e20 3d20 7265 2e73 6561 7263 6828 225c  n = re.search("\
-00018e20: 5b54 4f4f 4c5f 285b 5e5c 5b5c 5d5d 2b3f  [TOOL_([^\[\]]+?
-00018e30: 295c 5d22 2c20 6669 6e65 5475 6e65 6455  )\]", fineTunedU
-00018e40: 7365 7249 6e70 7574 290a 2020 2020 2020  serInput).      
-00018e50: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00018e60: 6e66 6967 2e73 656c 6563 7465 6454 6f6f  nfig.selectedToo
-00018e70: 6c20 3d20 6368 6563 6b43 616c 6c53 7065  l = checkCallSpe
-00018e80: 6369 6669 6346 756e 6374 696f 6e2e 6772  cificFunction.gr
-00018e90: 6f75 7028 3129 2069 6620 6368 6563 6b43  oup(1) if checkC
-00018ea0: 616c 6c53 7065 6369 6669 6346 756e 6374  allSpecificFunct
-00018eb0: 696f 6e20 616e 6420 6368 6563 6b43 616c  ion and checkCal
-00018ec0: 6c53 7065 6369 6669 6346 756e 6374 696f  lSpecificFunctio
-00018ed0: 6e2e 6772 6f75 7028 3129 2069 6e20 636f  n.group(1) in co
-00018ee0: 6e66 6967 2e74 6f6f 6c46 756e 6374 696f  nfig.toolFunctio
-00018ef0: 6e4d 6574 686f 6473 2065 6c73 6520 2222  nMethods else ""
-00018f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018f10: 2020 2020 2069 6620 636f 6e66 6967 2e64       if config.d
-00018f20: 6576 656c 6f70 6572 2061 6e64 2063 6f6e  eveloper and con
-00018f30: 6669 672e 7365 6c65 6374 6564 546f 6f6c  fig.selectedTool
-00018f40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00018f50: 2020 2020 2020 2020 2020 2370 7269 6e74            #print
-00018f60: 3128 6622 6361 6c6c 696e 6720 6675 6e63  1(f"calling func
-00018f70: 7469 6f6e 2027 7b63 6f6e 6669 672e 7365  tion '{config.se
-00018f80: 6c65 6374 6564 546f 6f6c 7d27 202e 2e2e  lectedTool}' ...
-00018f90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00018fa0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00018fb0: 5f66 6f72 6d61 7474 6564 5f74 6578 7428  _formatted_text(
-00018fc0: 4854 4d4c 2866 223c 7b63 6f6e 6669 672e  HTML(f"<{config.
-00018fd0: 7465 726d 696e 616c 5072 6f6d 7074 496e  terminalPromptIn
-00018fe0: 6469 6361 746f 7243 6f6c 6f72 327d 3e43  dicatorColor2}>C
-00018ff0: 616c 6c69 6e67 2066 756e 6374 696f 6e3c  alling function<
-00019000: 2f7b 636f 6e66 6967 2e74 6572 6d69 6e61  /{config.termina
-00019010: 6c50 726f 6d70 7449 6e64 6963 6174 6f72  lPromptIndicator
-00019020: 436f 6c6f 7232 7d3e 203c 7b63 6f6e 6669  Color2}> <{confi
-00019030: 672e 7465 726d 696e 616c 436f 6d6d 616e  g.terminalComman
-00019040: 6445 6e74 7279 436f 6c6f 7232 7d3e 277b  dEntryColor2}>'{
-00019050: 636f 6e66 6967 2e73 656c 6563 7465 6454  config.selectedT
-00019060: 6f6f 6c7d 273c 2f7b 636f 6e66 6967 2e74  ool}'</{config.t
-00019070: 6572 6d69 6e61 6c43 6f6d 6d61 6e64 456e  erminalCommandEn
-00019080: 7472 7943 6f6c 6f72 327d 3e20 3c7b 636f  tryColor2}> <{co
-00019090: 6e66 6967 2e74 6572 6d69 6e61 6c50 726f  nfig.terminalPro
-000190a0: 6d70 7449 6e64 6963 6174 6f72 436f 6c6f  mptIndicatorColo
-000190b0: 7232 7d3e 2e2e 2e3c 2f7b 636f 6e66 6967  r2}>...</{config
-000190c0: 2e74 6572 6d69 6e61 6c50 726f 6d70 7449  .terminalPromptI
-000190d0: 6e64 6963 6174 6f72 436f 6c6f 7232 7d3e  ndicatorColor2}>
-000190e0: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
-000190f0: 2020 2020 2020 2020 6669 6e65 5475 6e65          fineTune
-00019100: 6455 7365 7249 6e70 7574 203d 2072 652e  dUserInput = re.
-00019110: 7375 6228 7370 6563 6961 6c45 6e74 7279  sub(specialEntry
-00019120: 5061 7474 6572 6e2c 2022 222c 2066 696e  Pattern, "", fin
-00019130: 6554 756e 6564 5573 6572 496e 7075 7429  eTunedUserInput)
-00019140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019150: 2020 2020 2063 6f6e 6669 672e 6375 7272       config.curr
-00019160: 656e 744d 6573 7361 6765 732e 6170 7065  entMessages.appe
-00019170: 6e64 287b 2272 6f6c 6522 3a20 2275 7365  nd({"role": "use
-00019180: 7222 2c20 2263 6f6e 7465 6e74 223a 2066  r", "content": f
-00019190: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
-000191a0: 747d 290a 0a20 2020 2020 2020 2020 2020  t})..           
-000191b0: 2020 2020 2020 2020 2023 2073 7461 7274           # start
-000191c0: 2073 7069 6e6e 696e 670a 2020 2020 2020   spinning.      
-000191d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000191e0: 6e66 6967 2e73 746f 705f 6576 656e 7420  nfig.stop_event 
-000191f0: 3d20 7468 7265 6164 696e 672e 4576 656e  = threading.Even
-00019200: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00019210: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
-00019220: 7069 6e6e 6572 5f74 6872 6561 6420 3d20  pinner_thread = 
-00019230: 7468 7265 6164 696e 672e 5468 7265 6164  threading.Thread
-00019240: 2874 6172 6765 743d 7370 696e 6e69 6e67  (target=spinning
-00019250: 5f61 6e69 6d61 7469 6f6e 2c20 6172 6773  _animation, args
-00019260: 3d28 636f 6e66 6967 2e73 746f 705f 6576  =(config.stop_ev
-00019270: 656e 742c 2929 0a20 2020 2020 2020 2020  ent,)).         
-00019280: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00019290: 672e 7370 696e 6e65 725f 7468 7265 6164  g.spinner_thread
-000192a0: 2e73 7461 7274 2829 0a0a 2020 2020 2020  .start()..      
-000192b0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000192c0: 666f 7263 6520 6c6f 6164 696e 6720 696e  force loading in
-000192d0: 7465 726e 6574 2073 6561 7263 6865 730a  ternet searches.
-000192e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192f0: 2020 2020 6966 2063 6f6e 6669 672e 6c6f      if config.lo
-00019300: 6164 696e 6749 6e74 6572 6e65 7453 6561  adingInternetSea
-00019310: 7263 6865 7320 3d3d 2022 616c 7761 7973  rches == "always
-00019320: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00019330: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00018a70: 2063 6861 7462 6f74 203d 2063 6f6e 6669   chatbot = confi
+00018a80: 672e 6c6c 6d49 6e74 6572 6661 6365 0a20  g.llmInterface. 
+00018a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018aa0: 2020 2065 6c69 6620 6361 6c6c 4368 6174     elif callChat
+00018ab0: 426f 7420 3a3d 2072 652e 7365 6172 6368  Bot := re.search
+00018ac0: 2822 5c5b 4348 4154 5f28 5b5e 5c5b 5c5d  ("\[CHAT_([^\[\]
+00018ad0: 5d2b 3f29 5c5d 222c 2066 696e 6554 756e  ]+?)\]", fineTun
+00018ae0: 6564 5573 6572 496e 7075 7429 3a0a 2020  edUserInput):.  
+00018af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b00: 2020 2020 2020 6368 6174 626f 7420 3d20        chatbot = 
+00018b10: 6361 6c6c 4368 6174 426f 742e 6772 6f75  callChatBot.grou
+00018b20: 7028 3129 2e6c 6f77 6572 2829 2069 6620  p(1).lower() if 
+00018b30: 6361 6c6c 4368 6174 426f 7420 616e 6420  callChatBot and 
+00018b40: 6361 6c6c 4368 6174 426f 742e 6772 6f75  callChatBot.grou
+00018b50: 7028 3129 2e6c 6f77 6572 2829 2069 6e20  p(1).lower() in 
+00018b60: 2822 6368 6174 6770 7422 2c20 2267 656d  ("chatgpt", "gem
+00018b70: 696e 6970 726f 222c 2022 7061 6c6d 3222  inipro", "palm2"
+00018b80: 2c20 2263 6f64 6579 2229 2065 6c73 6520  , "codey") else 
+00018b90: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+00018ba0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00018bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bc0: 2020 2020 2063 6861 7462 6f74 203d 2022       chatbot = "
+00018bd0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00018be0: 2020 2020 2020 6966 2063 6861 7462 6f74        if chatbot
+00018bf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018c00: 2020 2020 2020 2020 2020 2320 6361 6c6c            # call
+00018c10: 2074 6865 2073 7063 6966 6965 6420 6368   the spcified ch
+00018c20: 6174 626f 7420 746f 2063 6f6e 7469 6e75  atbot to continu
+00018c30: 6520 7468 6520 636f 6e76 6572 7361 7469  e the conversati
+00018c40: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+00018c50: 2020 2020 2020 2020 2020 2066 696e 6554             fineT
+00018c60: 756e 6564 5573 6572 496e 7075 7420 3d20  unedUserInput = 
+00018c70: 7265 2e73 7562 2822 5c5b 4348 4154 5c5d  re.sub("\[CHAT\]
+00018c80: 7c5c 5b43 4841 545f 5b5e 5c5b 5c5d 5d2b  |\[CHAT_[^\[\]]+
+00018c90: 3f5c 5d22 2c20 2222 2c20 6669 6e65 5475  ?\]", "", fineTu
+00018ca0: 6e65 6455 7365 7249 6e70 7574 290a 2020  nedUserInput).  
+00018cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cc0: 2020 2020 2020 7365 6c66 2e6c 6175 6e63        self.launc
+00018cd0: 6843 6861 7462 6f74 2863 6861 7462 6f74  hChatbot(chatbot
+00018ce0: 2c20 6669 6e65 5475 6e65 6455 7365 7249  , fineTunedUserI
+00018cf0: 6e70 7574 290a 2020 2020 2020 2020 2020  nput).          
+00018d00: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00018d10: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+00018d20: 2020 2020 2020 2020 2020 2023 2077 6865             # whe
+00018d30: 6e20 7573 6572 2064 6f6e 2774 2077 616e  n user don't wan
+00018d40: 7420 6120 6675 6e63 7469 6f6e 2063 616c  t a function cal
+00018d50: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
+00018d60: 2020 2020 2020 6e6f 4675 6e63 7469 6f6e        noFunction
+00018d70: 4361 6c6c 203d 2028 225b 4e4f 5f54 4f4f  Call = ("[NO_TOO
+00018d80: 4c5d 2220 696e 2066 696e 6554 756e 6564  L]" in fineTuned
+00018d90: 5573 6572 496e 7075 7429 0a20 2020 2020  UserInput).     
+00018da0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00018db0: 2077 6865 6e20 7573 6572 2077 616e 7420   when user want 
+00018dc0: 746f 2063 616c 6c20 6120 7061 7274 6963  to call a partic
+00018dd0: 756c 6172 2066 756e 6374 696f 6e0a 2020  ular function.  
+00018de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018df0: 2020 6368 6563 6b43 616c 6c53 7065 6369    checkCallSpeci
+00018e00: 6669 6346 756e 6374 696f 6e20 3d20 7265  ficFunction = re
+00018e10: 2e73 6561 7263 6828 225c 5b54 4f4f 4c5f  .search("\[TOOL_
+00018e20: 285b 5e5c 5b5c 5d5d 2b3f 295c 5d22 2c20  ([^\[\]]+?)\]", 
+00018e30: 6669 6e65 5475 6e65 6455 7365 7249 6e70  fineTunedUserInp
+00018e40: 7574 290a 2020 2020 2020 2020 2020 2020  ut).            
+00018e50: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
+00018e60: 656c 6563 7465 6454 6f6f 6c20 3d20 6368  electedTool = ch
+00018e70: 6563 6b43 616c 6c53 7065 6369 6669 6346  eckCallSpecificF
+00018e80: 756e 6374 696f 6e2e 6772 6f75 7028 3129  unction.group(1)
+00018e90: 2069 6620 6368 6563 6b43 616c 6c53 7065   if checkCallSpe
+00018ea0: 6369 6669 6346 756e 6374 696f 6e20 616e  cificFunction an
+00018eb0: 6420 6368 6563 6b43 616c 6c53 7065 6369  d checkCallSpeci
+00018ec0: 6669 6346 756e 6374 696f 6e2e 6772 6f75  ficFunction.grou
+00018ed0: 7028 3129 2069 6e20 636f 6e66 6967 2e74  p(1) in config.t
+00018ee0: 6f6f 6c46 756e 6374 696f 6e4d 6574 686f  oolFunctionMetho
+00018ef0: 6473 2065 6c73 6520 2222 0a20 2020 2020  ds else "".     
+00018f00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00018f10: 6620 636f 6e66 6967 2e64 6576 656c 6f70  f config.develop
+00018f20: 6572 2061 6e64 2063 6f6e 6669 672e 7365  er and config.se
+00018f30: 6c65 6374 6564 546f 6f6c 3a0a 2020 2020  lectedTool:.    
+00018f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f50: 2020 2020 2370 7269 6e74 3128 6622 6361      #print1(f"ca
+00018f60: 6c6c 696e 6720 6675 6e63 7469 6f6e 2027  lling function '
+00018f70: 7b63 6f6e 6669 672e 7365 6c65 6374 6564  {config.selected
+00018f80: 546f 6f6c 7d27 202e 2e2e 2229 0a20 2020  Tool}' ...").   
+00018f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fa0: 2020 2020 2070 7269 6e74 5f66 6f72 6d61       print_forma
+00018fb0: 7474 6564 5f74 6578 7428 4854 4d4c 2866  tted_text(HTML(f
+00018fc0: 223c 7b63 6f6e 6669 672e 7465 726d 696e  "<{config.termin
+00018fd0: 616c 5072 6f6d 7074 496e 6469 6361 746f  alPromptIndicato
+00018fe0: 7243 6f6c 6f72 327d 3e43 616c 6c69 6e67  rColor2}>Calling
+00018ff0: 2066 756e 6374 696f 6e3c 2f7b 636f 6e66   function</{conf
+00019000: 6967 2e74 6572 6d69 6e61 6c50 726f 6d70  ig.terminalPromp
+00019010: 7449 6e64 6963 6174 6f72 436f 6c6f 7232  tIndicatorColor2
+00019020: 7d3e 203c 7b63 6f6e 6669 672e 7465 726d  }> <{config.term
+00019030: 696e 616c 436f 6d6d 616e 6445 6e74 7279  inalCommandEntry
+00019040: 436f 6c6f 7232 7d3e 277b 636f 6e66 6967  Color2}>'{config
+00019050: 2e73 656c 6563 7465 6454 6f6f 6c7d 273c  .selectedTool}'<
+00019060: 2f7b 636f 6e66 6967 2e74 6572 6d69 6e61  /{config.termina
+00019070: 6c43 6f6d 6d61 6e64 456e 7472 7943 6f6c  lCommandEntryCol
+00019080: 6f72 327d 3e20 3c7b 636f 6e66 6967 2e74  or2}> <{config.t
+00019090: 6572 6d69 6e61 6c50 726f 6d70 7449 6e64  erminalPromptInd
+000190a0: 6963 6174 6f72 436f 6c6f 7232 7d3e 2e2e  icatorColor2}>..
+000190b0: 2e3c 2f7b 636f 6e66 6967 2e74 6572 6d69  .</{config.termi
+000190c0: 6e61 6c50 726f 6d70 7449 6e64 6963 6174  nalPromptIndicat
+000190d0: 6f72 436f 6c6f 7232 7d3e 2229 290a 2020  orColor2}>")).  
+000190e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190f0: 2020 6669 6e65 5475 6e65 6455 7365 7249    fineTunedUserI
+00019100: 6e70 7574 203d 2072 652e 7375 6228 7370  nput = re.sub(sp
+00019110: 6563 6961 6c45 6e74 7279 5061 7474 6572  ecialEntryPatter
+00019120: 6e2c 2022 222c 2066 696e 6554 756e 6564  n, "", fineTuned
+00019130: 5573 6572 496e 7075 7429 0a20 2020 2020  UserInput).     
+00019140: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00019150: 6f6e 6669 672e 6375 7272 656e 744d 6573  onfig.currentMes
+00019160: 7361 6765 732e 6170 7065 6e64 287b 2272  sages.append({"r
+00019170: 6f6c 6522 3a20 2275 7365 7222 2c20 2263  ole": "user", "c
+00019180: 6f6e 7465 6e74 223a 2066 696e 6554 756e  ontent": fineTun
+00019190: 6564 5573 6572 496e 7075 747d 290a 0a20  edUserInput}).. 
+000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191b0: 2020 2023 2073 7461 7274 2073 7069 6e6e     # start spinn
+000191c0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+000191d0: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
+000191e0: 746f 705f 6576 656e 7420 3d20 7468 7265  top_event = thre
+000191f0: 6164 696e 672e 4576 656e 7428 290a 2020  ading.Event().  
+00019200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019210: 2020 636f 6e66 6967 2e73 7069 6e6e 6572    config.spinner
+00019220: 5f74 6872 6561 6420 3d20 7468 7265 6164  _thread = thread
+00019230: 696e 672e 5468 7265 6164 2874 6172 6765  ing.Thread(targe
+00019240: 743d 7370 696e 6e69 6e67 5f61 6e69 6d61  t=spinning_anima
+00019250: 7469 6f6e 2c20 6172 6773 3d28 636f 6e66  tion, args=(conf
+00019260: 6967 2e73 746f 705f 6576 656e 742c 2929  ig.stop_event,))
+00019270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019280: 2020 2020 2063 6f6e 6669 672e 7370 696e       config.spin
+00019290: 6e65 725f 7468 7265 6164 2e73 7461 7274  ner_thread.start
+000192a0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+000192b0: 2020 2020 2020 2020 2320 666f 7263 6520          # force 
+000192c0: 6c6f 6164 696e 6720 696e 7465 726e 6574  loading internet
+000192d0: 2073 6561 7263 6865 730a 2020 2020 2020   searches.      
+000192e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000192f0: 2063 6f6e 6669 672e 6c6f 6164 696e 6749   config.loadingI
+00019300: 6e74 6572 6e65 7453 6561 7263 6865 7320  nternetSearches 
+00019310: 3d3d 2022 616c 7761 7973 223a 0a20 2020  == "always":.   
+00019320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019330: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
 00019340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019350: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-00019360: 6967 2e63 7572 7265 6e74 4d65 7373 6167  ig.currentMessag
-00019370: 6573 203d 2043 616c 6c4c 4c4d 2e72 756e  es = CallLLM.run
-00019380: 5369 6e67 6c65 4675 6e63 7469 6f6e 4361  SingleFunctionCa
-00019390: 6c6c 2863 6f6e 6669 672e 6375 7272 656e  ll(config.curren
-000193a0: 744d 6573 7361 6765 732c 2022 696e 7465  tMessages, "inte
-000193b0: 6772 6174 655f 676f 6f67 6c65 5f73 6561  grate_google_sea
-000193c0: 7263 6865 7322 290a 2020 2020 2020 2020  rches").        
-000193d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193e0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-000193f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019400: 2020 2020 7072 696e 7431 2822 556e 6162      print1("Unab
-00019410: 6c65 2074 6f20 6c6f 6164 2069 6e74 6572  le to load inter
-00019420: 6e65 7420 7265 736f 7572 6365 732e 2229  net resources.")
-00019430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019440: 2020 2020 2020 2020 2020 2020 2073 686f               sho
-00019450: 7745 7272 6f72 7328 290a 0a20 2020 2020  wErrors()..     
-00019460: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00019470: 6f6d 706c 6574 696f 6e20 3d20 4361 6c6c  ompletion = Call
-00019480: 4c4c 4d2e 7275 6e47 656e 6975 7343 616c  LLM.runGeniusCal
-00019490: 6c28 636f 6e66 6967 2e63 7572 7265 6e74  l(config.current
-000194a0: 4d65 7373 6167 6573 2c20 6e6f 4675 6e63  Messages, noFunc
-000194b0: 7469 6f6e 4361 6c6c 290a 2020 2020 2020  tionCall).      
-000194c0: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-000194d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194e0: 2020 2023 2073 746f 7020 7370 696e 6e69     # stop spinni
-000194f0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-00019500: 2020 2020 2020 2063 6f6e 6669 672e 7275         config.ru
-00019510: 6e50 7974 686f 6e20 3d20 5472 7565 0a20  nPython = True. 
-00019520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019530: 2020 2073 746f 7053 7069 6e6e 696e 6728     stopSpinning(
-00019540: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019550: 2020 2020 2020 2069 6620 636f 6d70 6c65         if comple
-00019560: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
-00019570: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019580: 2020 2020 2020 2020 2020 2320 4372 6561            # Crea
-00019590: 7465 2061 206e 6577 2074 6872 6561 6420  te a new thread 
-000195a0: 666f 7220 7468 6520 7374 7265 616d 696e  for the streamin
-000195b0: 6720 7461 736b 0a20 2020 2020 2020 2020  g task.         
-000195c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000195d0: 7472 6561 6d69 6e67 576f 7264 5772 6170  treamingWordWrap
-000195e0: 7065 7220 3d20 5374 7265 616d 696e 6757  per = StreamingW
-000195f0: 6f72 6457 7261 7070 6572 2829 0a20 2020  ordWrapper().   
-00019600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019610: 2020 2020 2073 7472 6561 6d69 6e67 5f65       streaming_e
-00019620: 7665 6e74 203d 2074 6872 6561 6469 6e67  vent = threading
-00019630: 2e45 7665 6e74 2829 0a20 2020 2020 2020  .Event().       
-00019640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019650: 2073 656c 662e 7374 7265 616d 696e 675f   self.streaming_
-00019660: 7468 7265 6164 203d 2074 6872 6561 6469  thread = threadi
-00019670: 6e67 2e54 6872 6561 6428 7461 7267 6574  ng.Thread(target
-00019680: 3d73 7472 6561 6d69 6e67 576f 7264 5772  =streamingWordWr
-00019690: 6170 7065 722e 7374 7265 616d 4f75 7470  apper.streamOutp
-000196a0: 7574 732c 2061 7267 733d 2873 7472 6561  uts, args=(strea
-000196b0: 6d69 6e67 5f65 7665 6e74 2c20 636f 6d70  ming_event, comp
-000196c0: 6c65 7469 6f6e 2c20 5472 7565 2069 6620  letion, True if 
-000196d0: 636f 6e66 6967 2e6c 6c6d 496e 7465 7266  config.llmInterf
-000196e0: 6163 6520 696e 2028 2263 6861 7467 7074  ace in ("chatgpt
-000196f0: 222c 2022 6c65 746d 6564 6f69 7422 2c20  ", "letmedoit", 
-00019700: 2267 726f 7122 2920 656c 7365 2046 616c  "groq") else Fal
-00019710: 7365 2929 0a20 2020 2020 2020 2020 2020  se)).           
-00019720: 2020 2020 2020 2020 2020 2020 2023 2053               # S
-00019730: 7461 7274 2074 6865 2073 7472 6561 6d69  tart the streami
-00019740: 6e67 2074 6872 6561 640a 2020 2020 2020  ng thread.      
-00019750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019760: 2020 7365 6c66 2e73 7472 6561 6d69 6e67    self.streaming
-00019770: 5f74 6872 6561 642e 7374 6172 7428 290a  _thread.start().
-00019780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019790: 2020 2020 2020 2020 2023 2077 6169 7420           # wait 
-000197a0: 7768 696c 6520 7465 7874 206f 7574 7075  while text outpu
-000197b0: 7420 6973 2073 7465 616d 696e 673b 2063  t is steaming; c
-000197c0: 6170 7475 7265 206b 6579 2063 6f6d 626f  apture key combo
-000197d0: 2027 6374 726c 2b71 2720 6f72 2027 6374   'ctrl+q' or 'ct
-000197e0: 726c 2b7a 2720 746f 2073 746f 7020 7468  rl+z' to stop th
-000197f0: 6520 7374 7265 616d 696e 670a 2020 2020  e streaming.    
-00019800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019810: 2020 2020 7374 7265 616d 696e 6757 6f72      streamingWor
-00019820: 6457 7261 7070 6572 2e6b 6579 546f 5374  dWrapper.keyToSt
-00019830: 6f70 5374 7265 616d 696e 6728 7374 7265  opStreaming(stre
-00019840: 616d 696e 675f 6576 656e 7429 0a0a 2020  aming_event)..  
+00019350: 2020 2020 2020 636f 6e66 6967 2e63 7572        config.cur
+00019360: 7265 6e74 4d65 7373 6167 6573 203d 2043  rentMessages = C
+00019370: 616c 6c4c 4c4d 2e72 756e 5369 6e67 6c65  allLLM.runSingle
+00019380: 4675 6e63 7469 6f6e 4361 6c6c 2863 6f6e  FunctionCall(con
+00019390: 6669 672e 6375 7272 656e 744d 6573 7361  fig.currentMessa
+000193a0: 6765 732c 2022 696e 7465 6772 6174 655f  ges, "integrate_
+000193b0: 676f 6f67 6c65 5f73 6561 7263 6865 7322  google_searches"
+000193c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000193d0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+000193e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000193f0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00019400: 696e 7431 2822 556e 6162 6c65 2074 6f20  int1("Unable to 
+00019410: 6c6f 6164 2069 6e74 6572 6e65 7420 7265  load internet re
+00019420: 736f 7572 6365 732e 2229 0a20 2020 2020  sources.").     
+00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019440: 2020 2020 2020 2073 686f 7745 7272 6f72         showError
+00019450: 7328 290a 0a20 2020 2020 2020 2020 2020  s()..           
+00019460: 2020 2020 2020 2020 2063 6f6d 706c 6574           complet
+00019470: 696f 6e20 3d20 4361 6c6c 4c4c 4d2e 7275  ion = CallLLM.ru
+00019480: 6e47 656e 6975 7343 616c 6c28 636f 6e66  nGeniusCall(conf
+00019490: 6967 2e63 7572 7265 6e74 4d65 7373 6167  ig.currentMessag
+000194a0: 6573 2c20 6e6f 4675 6e63 7469 6f6e 4361  es, noFunctionCa
+000194b0: 6c6c 290a 2020 2020 2020 2020 2020 2020  ll).            
+000194c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000194d0: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+000194e0: 746f 7020 7370 696e 6e69 6e67 0a20 2020  top spinning.   
+000194f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019500: 2063 6f6e 6669 672e 7275 6e50 7974 686f   config.runPytho
+00019510: 6e20 3d20 5472 7565 0a20 2020 2020 2020  n = True.       
+00019520: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+00019530: 7053 7069 6e6e 696e 6728 290a 0a20 2020  pSpinning()..   
+00019540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019550: 2069 6620 636f 6d70 6c65 7469 6f6e 2069   if completion i
+00019560: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00019570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019580: 2020 2020 2320 4372 6561 7465 2061 206e      # Create a n
+00019590: 6577 2074 6872 6561 6420 666f 7220 7468  ew thread for th
+000195a0: 6520 7374 7265 616d 696e 6720 7461 736b  e streaming task
+000195b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000195c0: 2020 2020 2020 2020 2073 7472 6561 6d69           streami
+000195d0: 6e67 576f 7264 5772 6170 7065 7220 3d20  ngWordWrapper = 
+000195e0: 5374 7265 616d 696e 6757 6f72 6457 7261  StreamingWordWra
+000195f0: 7070 6572 2829 0a20 2020 2020 2020 2020  pper().         
+00019600: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019610: 7472 6561 6d69 6e67 5f65 7665 6e74 203d  treaming_event =
+00019620: 2074 6872 6561 6469 6e67 2e45 7665 6e74   threading.Event
+00019630: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00019640: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019650: 7374 7265 616d 696e 675f 7468 7265 6164  streaming_thread
+00019660: 203d 2074 6872 6561 6469 6e67 2e54 6872   = threading.Thr
+00019670: 6561 6428 7461 7267 6574 3d73 7472 6561  ead(target=strea
+00019680: 6d69 6e67 576f 7264 5772 6170 7065 722e  mingWordWrapper.
+00019690: 7374 7265 616d 4f75 7470 7574 732c 2061  streamOutputs, a
+000196a0: 7267 733d 2873 7472 6561 6d69 6e67 5f65  rgs=(streaming_e
+000196b0: 7665 6e74 2c20 636f 6d70 6c65 7469 6f6e  vent, completion
+000196c0: 2c20 5472 7565 2069 6620 636f 6e66 6967  , True if config
+000196d0: 2e6c 6c6d 496e 7465 7266 6163 6520 696e  .llmInterface in
+000196e0: 2028 2263 6861 7467 7074 222c 2022 6c65   ("chatgpt", "le
+000196f0: 746d 6564 6f69 7422 2c20 2267 726f 7122  tmedoit", "groq"
+00019700: 2920 656c 7365 2046 616c 7365 2929 0a20  ) else False)). 
+00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019720: 2020 2020 2020 2023 2053 7461 7274 2074         # Start t
+00019730: 6865 2073 7472 6561 6d69 6e67 2074 6872  he streaming thr
+00019740: 6561 640a 2020 2020 2020 2020 2020 2020  ead.            
+00019750: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019760: 2e73 7472 6561 6d69 6e67 5f74 6872 6561  .streaming_threa
+00019770: 642e 7374 6172 7428 290a 0a20 2020 2020  d.start()..     
+00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019790: 2020 2023 2077 6169 7420 7768 696c 6520     # wait while 
+000197a0: 7465 7874 206f 7574 7075 7420 6973 2073  text output is s
+000197b0: 7465 616d 696e 673b 2063 6170 7475 7265  teaming; capture
+000197c0: 206b 6579 2063 6f6d 626f 2027 6374 726c   key combo 'ctrl
+000197d0: 2b71 2720 6f72 2027 6374 726c 2b7a 2720  +q' or 'ctrl+z' 
+000197e0: 746f 2073 746f 7020 7468 6520 7374 7265  to stop the stre
+000197f0: 616d 696e 670a 2020 2020 2020 2020 2020  aming.          
+00019800: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00019810: 7265 616d 696e 6757 6f72 6457 7261 7070  reamingWordWrapp
+00019820: 6572 2e6b 6579 546f 5374 6f70 5374 7265  er.keyToStopStre
+00019830: 616d 696e 6728 7374 7265 616d 696e 675f  aming(streaming_
+00019840: 6576 656e 7429 0a0a 2020 2020 2020 2020  event)..        
 00019850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019860: 2020 2020 2020 2320 7768 656e 2073 7472        # when str
-00019870: 6561 6d69 6e67 2069 7320 646f 6e65 206f  eaming is done o
-00019880: 7220 7768 656e 2075 7365 7220 7072 6573  r when user pres
-00019890: 7320 2263 7472 6c2b 7122 0a20 2020 2020  s "ctrl+q".     
-000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198b0: 2020 2073 656c 662e 7374 7265 616d 696e     self.streamin
-000198c0: 675f 7468 7265 6164 2e6a 6f69 6e28 290a  g_thread.join().
-000198d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000198e0: 2023 2065 7272 6f72 2063 6f64 6573 3a20   # error codes: 
-000198f0: 6874 7470 733a 2f2f 706c 6174 666f 726d  https://platform
-00019900: 2e6f 7065 6e61 692e 636f 6d2f 646f 6373  .openai.com/docs
-00019910: 2f67 7569 6465 732f 6572 726f 722d 636f  /guides/error-co
-00019920: 6465 732f 7079 7468 6f6e 2d6c 6962 7261  des/python-libra
-00019930: 7279 2d65 7272 6f72 2d74 7970 6573 0a20  ry-error-types. 
-00019940: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00019950: 7863 6570 7420 6f70 656e 6169 2e41 5049  xcept openai.API
-00019960: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-00019970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019980: 7374 6f70 5370 696e 6e69 6e67 2829 0a20  stopSpinning(). 
-00019990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199a0: 2020 2023 4861 6e64 6c65 2041 5049 2065     #Handle API e
-000199b0: 7272 6f72 2068 6572 652c 2065 2e67 2e20  rror here, e.g. 
-000199c0: 7265 7472 7920 6f72 206c 6f67 0a20 2020  retry or log.   
-000199d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199e0: 2070 7269 6e74 3128 6622 4f70 656e 4149   print1(f"OpenAI
-000199f0: 2041 5049 2072 6574 7572 6e65 6420 616e   API returned an
-00019a00: 2041 5049 2045 7272 6f72 3a20 7b65 7d22   API Error: {e}"
-00019a10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00019a20: 2020 6578 6365 7074 206f 7065 6e61 692e    except openai.
-00019a30: 4150 4943 6f6e 6e65 6374 696f 6e45 7272  APIConnectionErr
-00019a40: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
-00019a50: 2020 2020 2020 2020 2020 2020 2073 746f               sto
-00019a60: 7053 7069 6e6e 696e 6728 290a 2020 2020  pSpinning().    
-00019a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a80: 2348 616e 646c 6520 636f 6e6e 6563 7469  #Handle connecti
-00019a90: 6f6e 2065 7272 6f72 2068 6572 650a 2020  on error here.  
-00019aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ab0: 2020 7072 696e 7431 2866 2246 6169 6c65    print1(f"Faile
-00019ac0: 6420 746f 2063 6f6e 6e65 6374 2074 6f20  d to connect to 
-00019ad0: 4f70 656e 4149 2041 5049 3a20 7b65 7d22  OpenAI API: {e}"
-00019ae0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00019af0: 2020 6578 6365 7074 206f 7065 6e61 692e    except openai.
-00019b00: 5261 7465 4c69 6d69 7445 7272 6f72 2061  RateLimitError a
-00019b10: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-00019b20: 2020 2020 2020 2020 2073 746f 7053 7069           stopSpi
-00019b30: 6e6e 696e 6728 290a 2020 2020 2020 2020  nning().        
-00019b40: 2020 2020 2020 2020 2020 2020 2348 616e              #Han
-00019b50: 646c 6520 7261 7465 206c 696d 6974 2065  dle rate limit e
-00019b60: 7272 6f72 2028 7765 2072 6563 6f6d 6d65  rror (we recomme
-00019b70: 6e64 2075 7369 6e67 2065 7870 6f6e 656e  nd using exponen
-00019b80: 7469 616c 2062 6163 6b6f 6666 290a 2020  tial backoff).  
-00019b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ba0: 2020 7072 696e 7431 2866 224f 7065 6e41    print1(f"OpenA
-00019bb0: 4920 4150 4920 7265 7175 6573 7420 6578  I API request ex
-00019bc0: 6365 6564 6564 2072 6174 6520 6c69 6d69  ceeded rate limi
-00019bd0: 743a 207b 657d 2229 0a20 2020 2020 2020  t: {e}").       
-00019be0: 2020 2020 2020 2020 2065 7863 6570 743a           except:
-00019bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019c00: 2020 2020 2073 746f 7053 7069 6e6e 696e       stopSpinnin
-00019c10: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
-00019c20: 2020 2020 2020 2020 7472 6163 6520 3d20          trace = 
-00019c30: 7472 6163 6562 6163 6b2e 666f 726d 6174  traceback.format
-00019c40: 5f65 7863 2829 0a20 2020 2020 2020 2020  _exc().         
-00019c50: 2020 2020 2020 2020 2020 2069 6620 2250             if "P
-00019c60: 6c65 6173 6520 7265 6475 6365 2074 6865  lease reduce the
-00019c70: 206c 656e 6774 6820 6f66 2074 6865 206d   length of the m
-00019c80: 6573 7361 6765 7320 6f72 2063 6f6d 706c  essages or compl
-00019c90: 6574 696f 6e22 2069 6e20 7472 6163 653a  etion" in trace:
-00019ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019cb0: 2020 2020 2020 2020 2070 7269 6e74 3128           print1(
-00019cc0: 224d 6178 696d 756d 2074 6f6b 656e 7320  "Maximum tokens 
-00019cd0: 7265 6163 6865 6421 2229 0a20 2020 2020  reached!").     
-00019ce0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00019cf0: 6c69 6620 636f 6e66 6967 2e64 6576 656c  lif config.devel
-00019d00: 6f70 6572 3a0a 2020 2020 2020 2020 2020  oper:.          
-00019d10: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00019d20: 696e 7431 2873 656c 662e 6469 7669 6465  int1(self.divide
-00019d30: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-00019d40: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00019d50: 3128 7472 6163 6529 0a20 2020 2020 2020  1(trace).       
-00019d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d70: 2070 7269 6e74 3128 7365 6c66 2e64 6976   print1(self.div
-00019d80: 6964 6572 290a 2020 2020 2020 2020 2020  ider).          
-00019d90: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00019860: 2320 7768 656e 2073 7472 6561 6d69 6e67  # when streaming
+00019870: 2069 7320 646f 6e65 206f 7220 7768 656e   is done or when
+00019880: 2075 7365 7220 7072 6573 7320 2263 7472   user press "ctr
+00019890: 6c2b 7122 0a20 2020 2020 2020 2020 2020  l+q".           
+000198a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000198b0: 662e 7374 7265 616d 696e 675f 7468 7265  f.streaming_thre
+000198c0: 6164 2e6a 6f69 6e28 290a 0a20 2020 2020  ad.join()..     
+000198d0: 2020 2020 2020 2020 2020 2023 2065 7272             # err
+000198e0: 6f72 2063 6f64 6573 3a20 6874 7470 733a  or codes: https:
+000198f0: 2f2f 706c 6174 666f 726d 2e6f 7065 6e61  //platform.opena
+00019900: 692e 636f 6d2f 646f 6373 2f67 7569 6465  i.com/docs/guide
+00019910: 732f 6572 726f 722d 636f 6465 732f 7079  s/error-codes/py
+00019920: 7468 6f6e 2d6c 6962 7261 7279 2d65 7272  thon-library-err
+00019930: 6f72 2d74 7970 6573 0a20 2020 2020 2020  or-types.       
+00019940: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00019950: 6f70 656e 6169 2e41 5049 4572 726f 7220  openai.APIError 
+00019960: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00019970: 2020 2020 2020 2020 2020 7374 6f70 5370            stopSp
+00019980: 696e 6e69 6e67 2829 0a20 2020 2020 2020  inning().       
+00019990: 2020 2020 2020 2020 2020 2020 2023 4861               #Ha
+000199a0: 6e64 6c65 2041 5049 2065 7272 6f72 2068  ndle API error h
+000199b0: 6572 652c 2065 2e67 2e20 7265 7472 7920  ere, e.g. retry 
+000199c0: 6f72 206c 6f67 0a20 2020 2020 2020 2020  or log.         
+000199d0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000199e0: 3128 6622 4f70 656e 4149 2041 5049 2072  1(f"OpenAI API r
+000199f0: 6574 7572 6e65 6420 616e 2041 5049 2045  eturned an API E
+00019a00: 7272 6f72 3a20 7b65 7d22 290a 2020 2020  rror: {e}").    
+00019a10: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00019a20: 7074 206f 7065 6e61 692e 4150 4943 6f6e  pt openai.APICon
+00019a30: 6e65 6374 696f 6e45 7272 6f72 2061 7320  nectionError as 
+00019a40: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00019a50: 2020 2020 2020 2073 746f 7053 7069 6e6e         stopSpinn
+00019a60: 696e 6728 290a 2020 2020 2020 2020 2020  ing().          
+00019a70: 2020 2020 2020 2020 2020 2348 616e 646c            #Handl
+00019a80: 6520 636f 6e6e 6563 7469 6f6e 2065 7272  e connection err
+00019a90: 6f72 2068 6572 650a 2020 2020 2020 2020  or here.        
+00019aa0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00019ab0: 7431 2866 2246 6169 6c65 6420 746f 2063  t1(f"Failed to c
+00019ac0: 6f6e 6e65 6374 2074 6f20 4f70 656e 4149  onnect to OpenAI
+00019ad0: 2041 5049 3a20 7b65 7d22 290a 2020 2020   API: {e}").    
+00019ae0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00019af0: 7074 206f 7065 6e61 692e 5261 7465 4c69  pt openai.RateLi
+00019b00: 6d69 7445 7272 6f72 2061 7320 653a 0a20  mitError as e:. 
+00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b20: 2020 2073 746f 7053 7069 6e6e 696e 6728     stopSpinning(
+00019b30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00019b40: 2020 2020 2020 2348 616e 646c 6520 7261        #Handle ra
+00019b50: 7465 206c 696d 6974 2065 7272 6f72 2028  te limit error (
+00019b60: 7765 2072 6563 6f6d 6d65 6e64 2075 7369  we recommend usi
+00019b70: 6e67 2065 7870 6f6e 656e 7469 616c 2062  ng exponential b
+00019b80: 6163 6b6f 6666 290a 2020 2020 2020 2020  ackoff).        
+00019b90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00019ba0: 7431 2866 224f 7065 6e41 4920 4150 4920  t1(f"OpenAI API 
+00019bb0: 7265 7175 6573 7420 6578 6365 6564 6564  request exceeded
+00019bc0: 2072 6174 6520 6c69 6d69 743a 207b 657d   rate limit: {e}
+00019bd0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00019be0: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+00019bf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019c00: 746f 7053 7069 6e6e 696e 6728 290a 2020  topSpinning().  
+00019c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c20: 2020 7472 6163 6520 3d20 7472 6163 6562    trace = traceb
+00019c30: 6163 6b2e 666f 726d 6174 5f65 7863 2829  ack.format_exc()
+00019c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019c50: 2020 2020 2069 6620 2250 6c65 6173 6520       if "Please 
+00019c60: 7265 6475 6365 2074 6865 206c 656e 6774  reduce the lengt
+00019c70: 6820 6f66 2074 6865 206d 6573 7361 6765  h of the message
+00019c80: 7320 6f72 2063 6f6d 706c 6574 696f 6e22  s or completion"
+00019c90: 2069 6e20 7472 6163 653a 0a20 2020 2020   in trace:.     
+00019ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cb0: 2020 2070 7269 6e74 3128 224d 6178 696d     print1("Maxim
+00019cc0: 756d 2074 6f6b 656e 7320 7265 6163 6865  um tokens reache
+00019cd0: 6421 2229 0a20 2020 2020 2020 2020 2020  d!").           
+00019ce0: 2020 2020 2020 2020 2065 6c69 6620 636f           elif co
+00019cf0: 6e66 6967 2e64 6576 656c 6f70 6572 3a0a  nfig.developer:.
+00019d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d10: 2020 2020 2020 2020 7072 696e 7431 2873          print1(s
+00019d20: 656c 662e 6469 7669 6465 7229 0a20 2020  elf.divider).   
+00019d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d40: 2020 2020 2070 7269 6e74 3128 7472 6163       print1(trac
+00019d50: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00019d60: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00019d70: 3128 7365 6c66 2e64 6976 6964 6572 290a  1(self.divider).
+00019d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
 00019da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019db0: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
-00019dc0: 4572 726f 7220 656e 636f 756e 7465 7265  Error encountere
-00019dd0: 6421 2229 0a0a 2020 2020 2020 2020 2020  d!")..          
-00019de0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-00019df0: 2e64 6566 6175 6c74 456e 7472 7920 3d20  .defaultEntry = 
-00019e00: 7573 6572 496e 7075 740a 2020 2020 2020  userInput.      
-00019e10: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00019e20: 696e 7431 2822 7374 6172 7469 6e67 2061  int1("starting a
-00019e30: 206e 6577 2063 6861 7421 2229 0a20 2020   new chat!").   
-00019e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e50: 2073 656c 662e 7361 7665 4368 6174 2863   self.saveChat(c
-00019e60: 6f6e 6669 672e 6375 7272 656e 744d 6573  onfig.currentMes
-00019e70: 7361 6765 7329 0a20 2020 2020 2020 2020  sages).         
-00019e80: 2020 2020 2020 2020 2020 2073 746f 7261             stora
-00019e90: 6765 6469 7265 6374 6f72 792c 2063 6f6e  gedirectory, con
-00019ea0: 6669 672e 6375 7272 656e 744d 6573 7361  fig.currentMessa
-00019eb0: 6765 7320 3d20 7374 6172 7443 6861 7428  ges = startChat(
-00019ec0: 290a 0a20 2020 2064 6566 206c 6175 6e63  )..    def launc
-00019ed0: 6843 6861 7462 6f74 2873 656c 662c 2063  hChatbot(self, c
-00019ee0: 6861 7462 6f74 2c20 6669 6e65 5475 6e65  hatbot, fineTune
-00019ef0: 6455 7365 7249 6e70 7574 293a 0a20 2020  dUserInput):.   
-00019f00: 2020 2020 2069 6620 6e6f 7420 6368 6174       if not chat
-00019f10: 626f 743a 0a20 2020 2020 2020 2020 2020  bot:.           
-00019f20: 2063 6861 7462 6f74 203d 2063 6f6e 6669   chatbot = confi
-00019f30: 672e 6c6c 6d49 6e74 6572 6661 6365 0a20  g.llmInterface. 
-00019f40: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
-00019f50: 2e69 7354 6572 6d75 783a 0a20 2020 2020  .isTermux:.     
-00019f60: 2020 2020 2020 2023 6368 6174 626f 7420         #chatbot 
-00019f70: 3d20 2263 6861 7467 7074 220a 2020 2020  = "chatgpt".    
-00019f80: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-00019f90: 2020 2020 6368 6174 626f 7473 203d 207b      chatbots = {
-00019fa0: 0a20 2020 2020 2020 2020 2020 2022 6c6c  .            "ll
-00019fb0: 616d 6163 7070 223a 206c 616d 6264 613a  amacpp": lambda:
-00019fc0: 204c 6c61 6d61 6370 7043 6861 7428 6d6f   LlamacppChat(mo
-00019fd0: 6465 6c3d 4e6f 6e65 2069 6620 636f 6e66  del=None if conf
-00019fe0: 6967 2e75 7365 4164 6469 7469 6f6e 616c  ig.useAdditional
-00019ff0: 4368 6174 4d6f 6465 6c20 656c 7365 2063  ChatModel else c
-0001a000: 6f6e 6669 672e 6c6c 616d 6163 7070 4d61  onfig.llamacppMa
-0001a010: 696e 4d6f 6465 6c29 2e72 756e 2866 696e  inModel).run(fin
-0001a020: 6554 756e 6564 5573 6572 496e 7075 7429  eTunedUserInput)
-0001a030: 2c0a 2020 2020 2020 2020 2020 2020 226f  ,.            "o
-0001a040: 6c6c 616d 6122 3a20 6c61 6d62 6461 3a20  llama": lambda: 
-0001a050: 4f6c 6c61 6d61 4368 6174 2829 2e72 756e  OllamaChat().run
-0001a060: 2866 696e 6554 756e 6564 5573 6572 496e  (fineTunedUserIn
-0001a070: 7075 742c 206d 6f64 656c 3d63 6f6e 6669  put, model=confi
-0001a080: 672e 6f6c 6c61 6d61 4368 6174 4d6f 6465  g.ollamaChatMode
-0001a090: 6c20 6966 2063 6f6e 6669 672e 7573 6541  l if config.useA
-0001a0a0: 6464 6974 696f 6e61 6c43 6861 744d 6f64  dditionalChatMod
-0001a0b0: 656c 2065 6c73 6520 636f 6e66 6967 2e6f  el else config.o
-0001a0c0: 6c6c 616d 614d 6169 6e4d 6f64 656c 292c  llamaMainModel),
-0001a0d0: 0a20 2020 2020 2020 2020 2020 2022 6772  .            "gr
-0001a0e0: 6f71 223a 206c 616d 6264 613a 2047 726f  oq": lambda: Gro
-0001a0f0: 7143 6861 7462 6f74 2829 2e72 756e 2866  qChatbot().run(f
-0001a100: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
-0001a110: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
-0001a120: 2263 6861 7467 7074 223a 206c 616d 6264  "chatgpt": lambd
-0001a130: 613a 2043 6861 7447 5054 2829 2e72 756e  a: ChatGPT().run
-0001a140: 2866 696e 6554 756e 6564 5573 6572 496e  (fineTunedUserIn
-0001a150: 7075 7429 2c0a 2020 2020 2020 2020 2020  put),.          
-0001a160: 2020 226c 6574 6d65 646f 6974 223a 206c    "letmedoit": l
-0001a170: 616d 6264 613a 2043 6861 7447 5054 2829  ambda: ChatGPT()
-0001a180: 2e72 756e 2866 696e 6554 756e 6564 5573  .run(fineTunedUs
-0001a190: 6572 496e 7075 7429 2c0a 2020 2020 2020  erInput),.      
-0001a1a0: 2020 2020 2020 2267 656d 696e 6922 3a20        "gemini": 
-0001a1b0: 6c61 6d62 6461 3a20 4765 6d69 6e69 5072  lambda: GeminiPr
-0001a1c0: 6f28 7465 6d70 6572 6174 7572 653d 636f  o(temperature=co
-0001a1d0: 6e66 6967 2e6c 6c6d 5465 6d70 6572 6174  nfig.llmTemperat
-0001a1e0: 7572 6529 2e72 756e 2866 696e 6554 756e  ure).run(fineTun
-0001a1f0: 6564 5573 6572 496e 7075 7429 2c0a 2020  edUserInput),.  
-0001a200: 2020 2020 2020 2020 2020 2267 656d 696e            "gemin
-0001a210: 6970 726f 223a 206c 616d 6264 613a 2047  ipro": lambda: G
-0001a220: 656d 696e 6950 726f 2874 656d 7065 7261  eminiPro(tempera
-0001a230: 7475 7265 3d63 6f6e 6669 672e 6c6c 6d54  ture=config.llmT
-0001a240: 656d 7065 7261 7475 7265 292e 7275 6e28  emperature).run(
-0001a250: 6669 6e65 5475 6e65 6455 7365 7249 6e70  fineTunedUserInp
-0001a260: 7574 292c 0a20 2020 2020 2020 2020 2020  ut),.           
-0001a270: 2022 7061 6c6d 3222 3a20 6c61 6d62 6461   "palm2": lambda
-0001a280: 3a20 5061 6c6d 3228 292e 7275 6e28 6669  : Palm2().run(fi
-0001a290: 6e65 5475 6e65 6455 7365 7249 6e70 7574  neTunedUserInput
-0001a2a0: 2c20 7465 6d70 6572 6174 7572 653d 636f  , temperature=co
-0001a2b0: 6e66 6967 2e6c 6c6d 5465 6d70 6572 6174  nfig.llmTemperat
-0001a2c0: 7572 6529 2c0a 2020 2020 2020 2020 2020  ure),.          
-0001a2d0: 2020 2263 6f64 6579 223a 206c 616d 6264    "codey": lambd
-0001a2e0: 613a 2043 6f64 6579 2829 2e72 756e 2866  a: Codey().run(f
-0001a2f0: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
-0001a300: 742c 2074 656d 7065 7261 7475 7265 3d63  t, temperature=c
-0001a310: 6f6e 6669 672e 6c6c 6d54 656d 7065 7261  onfig.llmTempera
-0001a320: 7475 7265 292c 0a20 2020 2020 2020 207d  ture),.        }
-0001a330: 0a20 2020 2020 2020 2069 6620 6368 6174  .        if chat
-0001a340: 626f 7420 696e 2063 6861 7462 6f74 733a  bot in chatbots:
-0001a350: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
-0001a360: 7462 6f74 735b 6368 6174 626f 745d 2829  tbots[chatbot]()
-0001a370: 0a0a 2020 2020 6465 6620 6164 6450 6167  ..    def addPag
-0001a380: 6572 5465 7874 2873 656c 662c 2074 6578  erText(self, tex
-0001a390: 742c 2077 7261 7057 6f72 6473 3d46 616c  t, wrapWords=Fal
-0001a3a0: 7365 293a 0a20 2020 2020 2020 2069 6620  se):.        if 
-0001a3b0: 7772 6170 576f 7264 733a 0a20 2020 2020  wrapWords:.     
-0001a3c0: 2020 2020 2020 2074 6578 7420 3d20 7365         text = se
-0001a3d0: 6c66 2e67 6574 5772 6170 7065 6448 544d  lf.getWrappedHTM
-0001a3e0: 4c54 6578 7428 7465 7874 290a 2020 2020  LText(text).    
-0001a3f0: 2020 2020 636f 6e66 6967 2e70 6167 6572      config.pager
-0001a400: 436f 6e74 656e 7420 2b3d 2066 227b 7465  Content += f"{te
-0001a410: 7874 7d5c 6e22 0a0a 2020 2020 6465 6620  xt}\n"..    def 
-0001a420: 6c61 756e 6368 5061 6765 7228 7365 6c66  launchPager(self
-0001a430: 2c20 7061 6765 7243 6f6e 7465 6e74 3d4e  , pagerContent=N
-0001a440: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-0001a450: 2070 6167 6572 436f 6e74 656e 7420 6973   pagerContent is
-0001a460: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001a470: 2020 2070 6167 6572 436f 6e74 656e 7420     pagerContent 
-0001a480: 3d20 636f 6e66 6967 2e70 6167 6572 436f  = config.pagerCo
-0001a490: 6e74 656e 740a 2020 2020 2020 2020 6966  ntent.        if
-0001a4a0: 2070 6167 6572 436f 6e74 656e 743a 0a20   pagerContent:. 
-0001a4b0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0001a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4d0: 6966 2073 6875 7469 6c2e 7768 6963 6828  if shutil.which(
-0001a4e0: 2262 6174 2229 3a0a 2020 2020 2020 2020  "bat"):.        
-0001a4f0: 2020 2020 2020 2020 2020 2020 2320 5769              # Wi
-0001a500: 6e64 6f77 7320 7573 6572 7320 6361 6e20  ndows users can 
-0001a510: 696e 7374 616c 6c20 6261 7420 636f 6d6d  install bat comm
-0001a520: 616e 6420 7769 7468 2073 636f 6f70 0a20  and with scoop. 
-0001a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a540: 2020 2023 2072 6561 643a 2068 7474 7073     # read: https
-0001a550: 3a2f 2f67 6974 6875 622e 636f 6d2f 5363  ://github.com/Sc
-0001a560: 6f6f 7049 6e73 7461 6c6c 6572 2f53 636f  oopInstaller/Sco
-0001a570: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
-0001a580: 2020 2020 2020 2023 203e 2069 7772 202d         # > iwr -
-0001a590: 7573 6562 2067 6574 2e73 636f 6f70 2e73  useb get.scoop.s
-0001a5a0: 6820 7c20 6965 780a 2020 2020 2020 2020  h | iex.        
-0001a5b0: 2020 2020 2020 2020 2020 2020 2320 3e20              # > 
-0001a5c0: 7363 6f6f 7020 696e 7374 616c 6c20 6172  scoop install ar
-0001a5d0: 6961 3220 6261 740a 2020 2020 2020 2020  ia2 bat.        
-0001a5e0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-0001a5f0: 652e 7365 6172 6368 2822 3c5b 5e3c 3e5d  e.search("<[^<>]
-0001a600: 2b3f 3e22 2c20 7061 6765 7243 6f6e 7465  +?>", pagerConte
-0001a610: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-0001a620: 2020 2020 2020 2020 2020 2020 2070 6167               pag
-0001a630: 6572 436f 6e74 656e 7420 3d20 5465 7874  erContent = Text
-0001a640: 5574 696c 2e63 6f6e 7665 7274 4874 6d6c  Util.convertHtml
-0001a650: 5461 6754 6f43 6f6c 6f72 616d 6128 7061  TagToColorama(pa
-0001a660: 6765 7243 6f6e 7465 6e74 290a 2020 2020  gerContent).    
-0001a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a680: 6c61 6e67 7561 6765 203d 2022 5079 7468  language = "Pyth
-0001a690: 6f6e 2220 6966 2022 6060 6070 7974 686f  on" if "```pytho
-0001a6a0: 6e22 2069 6e20 7061 6765 7243 6f6e 7465  n" in pagerConte
-0001a6b0: 6e74 2065 6c73 6520 224d 6172 6b64 6f77  nt else "Markdow
-0001a6c0: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
-0001a6d0: 2020 2020 2020 2070 7964 6f63 2e70 6970         pydoc.pip
-0001a6e0: 6570 6167 6572 2870 6167 6572 436f 6e74  epager(pagerCont
-0001a6f0: 656e 742c 2063 6d64 3d66 2262 6174 202d  ent, cmd=f"bat -
-0001a700: 6c20 7b6c 616e 6775 6167 657d 202d 2d70  l {language} --p
-0001a710: 6167 696e 6720 616c 7761 7973 2229 0a20  aging always"). 
-0001a720: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001a730: 6c69 6620 7368 7574 696c 2e77 6869 6368  lif shutil.which
-0001a740: 2822 6c65 7373 2229 3a0a 2020 2020 2020  ("less"):.      
-0001a750: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001a760: 5769 6e64 6f77 7320 7573 6572 7320 6361  Windows users ca
-0001a770: 6e20 696e 7374 616c 6c20 6c65 7373 2063  n install less c
-0001a780: 6f6d 6d61 6e64 2077 6974 6820 7363 6f6f  ommand with scoo
-0001a790: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-0001a7a0: 2020 2020 2020 2320 7265 6164 3a20 6874        # read: ht
-0001a7b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0001a7c0: 2f53 636f 6f70 496e 7374 616c 6c65 722f  /ScoopInstaller/
-0001a7d0: 5363 6f6f 700a 2020 2020 2020 2020 2020  Scoop.          
-0001a7e0: 2020 2020 2020 2020 2020 2320 3e20 6977            # > iw
-0001a7f0: 7220 2d75 7365 6220 6765 742e 7363 6f6f  r -useb get.scoo
-0001a800: 702e 7368 207c 2069 6578 0a20 2020 2020  p.sh | iex.     
-0001a810: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001a820: 203e 2073 636f 6f70 2069 6e73 7461 6c6c   > scoop install
-0001a830: 2061 7269 6132 206c 6573 730a 2020 2020   aria2 less.    
-0001a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a850: 6966 2072 652e 7365 6172 6368 2822 3c5b  if re.search("<[
-0001a860: 5e3c 3e5d 2b3f 3e22 2c20 7061 6765 7243  ^<>]+?>", pagerC
-0001a870: 6f6e 7465 6e74 293a 0a20 2020 2020 2020  ontent):.       
-0001a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a890: 2070 6167 6572 436f 6e74 656e 7420 3d20   pagerContent = 
-0001a8a0: 5465 7874 5574 696c 2e63 6f6e 7665 7274  TextUtil.convert
-0001a8b0: 4874 6d6c 5461 6754 6f43 6f6c 6f72 616d  HtmlTagToColoram
-0001a8c0: 6128 7061 6765 7243 6f6e 7465 6e74 290a  a(pagerContent).
-0001a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a8e0: 2020 2020 7079 646f 632e 7069 7065 7061      pydoc.pipepa
-0001a8f0: 6765 7228 7061 6765 7243 6f6e 7465 6e74  ger(pagerContent
-0001a900: 2c20 636d 643d 276c 6573 7320 2d52 2729  , cmd='less -R')
-0001a910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a920: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001a930: 2020 2020 2020 2020 2020 2070 7964 6f63             pydoc
-0001a940: 2e70 6167 6572 2870 6167 6572 436f 6e74  .pager(pagerCont
-0001a950: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
-0001a960: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-0001a970: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
-0001a980: 7061 6765 7256 6965 7720 3d20 4661 6c73  pagerView = Fals
-0001a990: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0001a9a0: 2020 7368 6f77 4572 726f 7273 2829 0a0a    showErrors()..
-0001a9b0: 2020 2020 2320 7772 6170 2068 746d 6c20      # wrap html 
-0001a9c0: 7465 7874 2061 7420 7370 6163 6573 0a20  text at spaces. 
-0001a9d0: 2020 2064 6566 2067 6574 5772 6170 7065     def getWrappe
-0001a9e0: 6448 544d 4c54 6578 7428 7365 6c66 2c20  dHTMLText(self, 
-0001a9f0: 7465 7874 2c20 7465 726d 696e 616c 5f77  text, terminal_w
-0001aa00: 6964 7468 3d4e 6f6e 6529 3a0a 2020 2020  idth=None):.    
-0001aa10: 2020 2020 6966 206e 6f74 2022 2022 2069      if not " " i
-0001aa20: 6e20 7465 7874 3a0a 2020 2020 2020 2020  n text:.        
-0001aa30: 2020 2020 7265 7475 726e 2074 6578 740a      return text.
-0001aa40: 2020 2020 2020 2020 6966 2074 6572 6d69          if termi
-0001aa50: 6e61 6c5f 7769 6474 6820 6973 204e 6f6e  nal_width is Non
-0001aa60: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-0001aa70: 6572 6d69 6e61 6c5f 7769 6474 6820 3d20  erminal_width = 
-0001aa80: 7368 7574 696c 2e67 6574 5f74 6572 6d69  shutil.get_termi
-0001aa90: 6e61 6c5f 7369 7a65 2829 2e63 6f6c 756d  nal_size().colum
-0001aaa0: 6e73 0a20 2020 2020 2020 2073 656c 662e  ns.        self.
-0001aab0: 7772 6170 7065 6454 6578 7420 3d20 2222  wrappedText = ""
-0001aac0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-0001aad0: 6e65 5769 6474 6820 3d20 300a 0a20 2020  neWidth = 0..   
-0001aae0: 2020 2020 2064 6566 2061 6464 576f 7264       def addWord
-0001aaf0: 7328 776f 7264 7329 3a0a 2020 2020 2020  s(words):.      
-0001ab00: 2020 2020 2020 776f 7264 7320 3d20 776f        words = wo
-0001ab10: 7264 732e 7370 6c69 7428 2220 2229 0a20  rds.split(" "). 
-0001ab20: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0001ab30: 6e64 6578 2c20 6974 656d 2069 6e20 656e  ndex, item in en
-0001ab40: 756d 6572 6174 6528 776f 7264 7329 3a0a  umerate(words):.
-0001ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab60: 6973 4c61 7374 4974 656d 203d 2028 6c65  isLastItem = (le
-0001ab70: 6e28 776f 7264 7329 202d 2069 6e64 6578  n(words) - index
-0001ab80: 203d 3d20 3129 0a20 2020 2020 2020 2020   == 1).         
-0001ab90: 2020 2020 2020 2069 6620 6973 5f43 4a4b         if is_CJK
-0001aba0: 2869 7465 6d29 3a0a 2020 2020 2020 2020  (item):.        
-0001abb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001abc0: 6949 6e64 6578 2c20 6920 696e 2065 6e75  iIndex, i in enu
-0001abd0: 6d65 7261 7465 2869 7465 6d29 3a0a 2020  merate(item):.  
+00019db0: 2020 7072 696e 7431 2822 4572 726f 7220    print1("Error 
+00019dc0: 656e 636f 756e 7465 7265 6421 2229 0a0a  encountered!")..
+00019dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019de0: 2020 2020 636f 6e66 6967 2e64 6566 6175      config.defau
+00019df0: 6c74 456e 7472 7920 3d20 7573 6572 496e  ltEntry = userIn
+00019e00: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
+00019e10: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+00019e20: 7374 6172 7469 6e67 2061 206e 6577 2063  starting a new c
+00019e30: 6861 7421 2229 0a20 2020 2020 2020 2020  hat!").         
+00019e40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019e50: 7361 7665 4368 6174 2863 6f6e 6669 672e  saveChat(config.
+00019e60: 6375 7272 656e 744d 6573 7361 6765 7329  currentMessages)
+00019e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019e80: 2020 2020 2073 746f 7261 6765 6469 7265       storagedire
+00019e90: 6374 6f72 792c 2063 6f6e 6669 672e 6375  ctory, config.cu
+00019ea0: 7272 656e 744d 6573 7361 6765 7320 3d20  rrentMessages = 
+00019eb0: 7374 6172 7443 6861 7428 290a 0a20 2020  startChat()..   
+00019ec0: 2064 6566 206c 6175 6e63 6843 6861 7462   def launchChatb
+00019ed0: 6f74 2873 656c 662c 2063 6861 7462 6f74  ot(self, chatbot
+00019ee0: 2c20 6669 6e65 5475 6e65 6455 7365 7249  , fineTunedUserI
+00019ef0: 6e70 7574 293a 0a20 2020 2020 2020 2069  nput):.        i
+00019f00: 6620 6e6f 7420 6368 6174 626f 743a 0a20  f not chatbot:. 
+00019f10: 2020 2020 2020 2020 2020 2063 6861 7462             chatb
+00019f20: 6f74 203d 2063 6f6e 6669 672e 6c6c 6d49  ot = config.llmI
+00019f30: 6e74 6572 6661 6365 0a20 2020 2020 2020  nterface.       
+00019f40: 2069 6620 636f 6e66 6967 2e69 7354 6572   if config.isTer
+00019f50: 6d75 783a 0a20 2020 2020 2020 2020 2020  mux:.           
+00019f60: 2023 6368 6174 626f 7420 3d20 2263 6861   #chatbot = "cha
+00019f70: 7467 7074 220a 2020 2020 2020 2020 2020  tgpt".          
+00019f80: 2020 2e2e 2e0a 2020 2020 2020 2020 6368    ....        ch
+00019f90: 6174 626f 7473 203d 207b 0a20 2020 2020  atbots = {.     
+00019fa0: 2020 2020 2020 2022 6c6c 616d 6163 7070         "llamacpp
+00019fb0: 223a 206c 616d 6264 613a 204c 6c61 6d61  ": lambda: Llama
+00019fc0: 6370 7043 6861 7428 6d6f 6465 6c3d 4e6f  cppChat(model=No
+00019fd0: 6e65 2069 6620 636f 6e66 6967 2e75 7365  ne if config.use
+00019fe0: 4164 6469 7469 6f6e 616c 4368 6174 4d6f  AdditionalChatMo
+00019ff0: 6465 6c20 656c 7365 2063 6f6e 6669 672e  del else config.
+0001a000: 6c6c 616d 6163 7070 4d61 696e 4d6f 6465  llamacppMainMode
+0001a010: 6c29 2e72 756e 2866 696e 6554 756e 6564  l).run(fineTuned
+0001a020: 5573 6572 496e 7075 7429 2c0a 2020 2020  UserInput),.    
+0001a030: 2020 2020 2020 2020 226f 6c6c 616d 6122          "ollama"
+0001a040: 3a20 6c61 6d62 6461 3a20 4f6c 6c61 6d61  : lambda: Ollama
+0001a050: 4368 6174 2829 2e72 756e 2866 696e 6554  Chat().run(fineT
+0001a060: 756e 6564 5573 6572 496e 7075 742c 206d  unedUserInput, m
+0001a070: 6f64 656c 3d63 6f6e 6669 672e 6f6c 6c61  odel=config.olla
+0001a080: 6d61 4368 6174 4d6f 6465 6c20 6966 2063  maChatModel if c
+0001a090: 6f6e 6669 672e 7573 6541 6464 6974 696f  onfig.useAdditio
+0001a0a0: 6e61 6c43 6861 744d 6f64 656c 2065 6c73  nalChatModel els
+0001a0b0: 6520 636f 6e66 6967 2e6f 6c6c 616d 614d  e config.ollamaM
+0001a0c0: 6169 6e4d 6f64 656c 292c 0a20 2020 2020  ainModel),.     
+0001a0d0: 2020 2020 2020 2022 6772 6f71 223a 206c         "groq": l
+0001a0e0: 616d 6264 613a 2047 726f 7143 6861 7462  ambda: GroqChatb
+0001a0f0: 6f74 2829 2e72 756e 2866 696e 6554 756e  ot().run(fineTun
+0001a100: 6564 5573 6572 496e 7075 7429 2c0a 2020  edUserInput),.  
+0001a110: 2020 2020 2020 2020 2020 2263 6861 7467            "chatg
+0001a120: 7074 223a 206c 616d 6264 613a 2043 6861  pt": lambda: Cha
+0001a130: 7447 5054 2829 2e72 756e 2866 696e 6554  tGPT().run(fineT
+0001a140: 756e 6564 5573 6572 496e 7075 7429 2c0a  unedUserInput),.
+0001a150: 2020 2020 2020 2020 2020 2020 226c 6574              "let
+0001a160: 6d65 646f 6974 223a 206c 616d 6264 613a  medoit": lambda:
+0001a170: 2043 6861 7447 5054 2829 2e72 756e 2866   ChatGPT().run(f
+0001a180: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
+0001a190: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
+0001a1a0: 2267 656d 696e 6922 3a20 6c61 6d62 6461  "gemini": lambda
+0001a1b0: 3a20 4765 6d69 6e69 5072 6f28 7465 6d70  : GeminiPro(temp
+0001a1c0: 6572 6174 7572 653d 636f 6e66 6967 2e6c  erature=config.l
+0001a1d0: 6c6d 5465 6d70 6572 6174 7572 6529 2e72  lmTemperature).r
+0001a1e0: 756e 2866 696e 6554 756e 6564 5573 6572  un(fineTunedUser
+0001a1f0: 496e 7075 7429 2c0a 2020 2020 2020 2020  Input),.        
+0001a200: 2020 2020 2267 656d 696e 6970 726f 223a      "geminipro":
+0001a210: 206c 616d 6264 613a 2047 656d 696e 6950   lambda: GeminiP
+0001a220: 726f 2874 656d 7065 7261 7475 7265 3d63  ro(temperature=c
+0001a230: 6f6e 6669 672e 6c6c 6d54 656d 7065 7261  onfig.llmTempera
+0001a240: 7475 7265 292e 7275 6e28 6669 6e65 5475  ture).run(fineTu
+0001a250: 6e65 6455 7365 7249 6e70 7574 292c 0a20  nedUserInput),. 
+0001a260: 2020 2020 2020 2020 2020 2022 7061 6c6d             "palm
+0001a270: 3222 3a20 6c61 6d62 6461 3a20 5061 6c6d  2": lambda: Palm
+0001a280: 3228 292e 7275 6e28 6669 6e65 5475 6e65  2().run(fineTune
+0001a290: 6455 7365 7249 6e70 7574 2c20 7465 6d70  dUserInput, temp
+0001a2a0: 6572 6174 7572 653d 636f 6e66 6967 2e6c  erature=config.l
+0001a2b0: 6c6d 5465 6d70 6572 6174 7572 6529 2c0a  lmTemperature),.
+0001a2c0: 2020 2020 2020 2020 2020 2020 2263 6f64              "cod
+0001a2d0: 6579 223a 206c 616d 6264 613a 2043 6f64  ey": lambda: Cod
+0001a2e0: 6579 2829 2e72 756e 2866 696e 6554 756e  ey().run(fineTun
+0001a2f0: 6564 5573 6572 496e 7075 742c 2074 656d  edUserInput, tem
+0001a300: 7065 7261 7475 7265 3d63 6f6e 6669 672e  perature=config.
+0001a310: 6c6c 6d54 656d 7065 7261 7475 7265 292c  llmTemperature),
+0001a320: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+0001a330: 2020 2069 6620 6368 6174 626f 7420 696e     if chatbot in
+0001a340: 2063 6861 7462 6f74 733a 0a20 2020 2020   chatbots:.     
+0001a350: 2020 2020 2020 2063 6861 7462 6f74 735b         chatbots[
+0001a360: 6368 6174 626f 745d 2829 0a0a 2020 2020  chatbot]()..    
+0001a370: 6465 6620 6164 6450 6167 6572 5465 7874  def addPagerText
+0001a380: 2873 656c 662c 2074 6578 742c 2077 7261  (self, text, wra
+0001a390: 7057 6f72 6473 3d46 616c 7365 293a 0a20  pWords=False):. 
+0001a3a0: 2020 2020 2020 2069 6620 7772 6170 576f         if wrapWo
+0001a3b0: 7264 733a 0a20 2020 2020 2020 2020 2020  rds:.           
+0001a3c0: 2074 6578 7420 3d20 7365 6c66 2e67 6574   text = self.get
+0001a3d0: 5772 6170 7065 6448 544d 4c54 6578 7428  WrappedHTMLText(
+0001a3e0: 7465 7874 290a 2020 2020 2020 2020 636f  text).        co
+0001a3f0: 6e66 6967 2e70 6167 6572 436f 6e74 656e  nfig.pagerConten
+0001a400: 7420 2b3d 2066 227b 7465 7874 7d5c 6e22  t += f"{text}\n"
+0001a410: 0a0a 2020 2020 6465 6620 6c61 756e 6368  ..    def launch
+0001a420: 5061 6765 7228 7365 6c66 2c20 7061 6765  Pager(self, page
+0001a430: 7243 6f6e 7465 6e74 3d4e 6f6e 6529 3a0a  rContent=None):.
+0001a440: 2020 2020 2020 2020 6966 2070 6167 6572          if pager
+0001a450: 436f 6e74 656e 7420 6973 204e 6f6e 653a  Content is None:
+0001a460: 0a20 2020 2020 2020 2020 2020 2070 6167  .            pag
+0001a470: 6572 436f 6e74 656e 7420 3d20 636f 6e66  erContent = conf
+0001a480: 6967 2e70 6167 6572 436f 6e74 656e 740a  ig.pagerContent.
+0001a490: 2020 2020 2020 2020 6966 2070 6167 6572          if pager
+0001a4a0: 436f 6e74 656e 743a 0a20 2020 2020 2020  Content:.       
+0001a4b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0001a4c0: 2020 2020 2020 2020 2020 6966 2073 6875            if shu
+0001a4d0: 7469 6c2e 7768 6963 6828 2262 6174 2229  til.which("bat")
+0001a4e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a4f0: 2020 2020 2020 2320 5769 6e64 6f77 7320        # Windows 
+0001a500: 7573 6572 7320 6361 6e20 696e 7374 616c  users can instal
+0001a510: 6c20 6261 7420 636f 6d6d 616e 6420 7769  l bat command wi
+0001a520: 7468 2073 636f 6f70 0a20 2020 2020 2020  th scoop.       
+0001a530: 2020 2020 2020 2020 2020 2020 2023 2072               # r
+0001a540: 6561 643a 2068 7474 7073 3a2f 2f67 6974  ead: https://git
+0001a550: 6875 622e 636f 6d2f 5363 6f6f 7049 6e73  hub.com/ScoopIns
+0001a560: 7461 6c6c 6572 2f53 636f 6f70 0a20 2020  taller/Scoop.   
+0001a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a580: 2023 203e 2069 7772 202d 7573 6562 2067   # > iwr -useb g
+0001a590: 6574 2e73 636f 6f70 2e73 6820 7c20 6965  et.scoop.sh | ie
+0001a5a0: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+0001a5b0: 2020 2020 2020 2320 3e20 7363 6f6f 7020        # > scoop 
+0001a5c0: 696e 7374 616c 6c20 6172 6961 3220 6261  install aria2 ba
+0001a5d0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0001a5e0: 2020 2020 2020 6966 2072 652e 7365 6172        if re.sear
+0001a5f0: 6368 2822 3c5b 5e3c 3e5d 2b3f 3e22 2c20  ch("<[^<>]+?>", 
+0001a600: 7061 6765 7243 6f6e 7465 6e74 293a 0a20  pagerContent):. 
+0001a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a620: 2020 2020 2020 2070 6167 6572 436f 6e74         pagerCont
+0001a630: 656e 7420 3d20 5465 7874 5574 696c 2e63  ent = TextUtil.c
+0001a640: 6f6e 7665 7274 4874 6d6c 5461 6754 6f43  onvertHtmlTagToC
+0001a650: 6f6c 6f72 616d 6128 7061 6765 7243 6f6e  olorama(pagerCon
+0001a660: 7465 6e74 290a 2020 2020 2020 2020 2020  tent).          
+0001a670: 2020 2020 2020 2020 2020 6c61 6e67 7561            langua
+0001a680: 6765 203d 2022 5079 7468 6f6e 2220 6966  ge = "Python" if
+0001a690: 2022 6060 6070 7974 686f 6e22 2069 6e20   "```python" in 
+0001a6a0: 7061 6765 7243 6f6e 7465 6e74 2065 6c73  pagerContent els
+0001a6b0: 6520 224d 6172 6b64 6f77 6e22 0a20 2020  e "Markdown".   
+0001a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6d0: 2070 7964 6f63 2e70 6970 6570 6167 6572   pydoc.pipepager
+0001a6e0: 2870 6167 6572 436f 6e74 656e 742c 2063  (pagerContent, c
+0001a6f0: 6d64 3d66 2262 6174 202d 6c20 7b6c 616e  md=f"bat -l {lan
+0001a700: 6775 6167 657d 202d 2d70 6167 696e 6720  guage} --paging 
+0001a710: 616c 7761 7973 2229 0a20 2020 2020 2020  always").       
+0001a720: 2020 2020 2020 2020 2065 6c69 6620 7368           elif sh
+0001a730: 7574 696c 2e77 6869 6368 2822 6c65 7373  util.which("less
+0001a740: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+0001a750: 2020 2020 2020 2020 2320 5769 6e64 6f77          # Window
+0001a760: 7320 7573 6572 7320 6361 6e20 696e 7374  s users can inst
+0001a770: 616c 6c20 6c65 7373 2063 6f6d 6d61 6e64  all less command
+0001a780: 2077 6974 6820 7363 6f6f 700a 2020 2020   with scoop.    
+0001a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7a0: 2320 7265 6164 3a20 6874 7470 733a 2f2f  # read: https://
+0001a7b0: 6769 7468 7562 2e63 6f6d 2f53 636f 6f70  github.com/Scoop
+0001a7c0: 496e 7374 616c 6c65 722f 5363 6f6f 700a  Installer/Scoop.
+0001a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7e0: 2020 2020 2320 3e20 6977 7220 2d75 7365      # > iwr -use
+0001a7f0: 6220 6765 742e 7363 6f6f 702e 7368 207c  b get.scoop.sh |
+0001a800: 2069 6578 0a20 2020 2020 2020 2020 2020   iex.           
+0001a810: 2020 2020 2020 2020 2023 203e 2073 636f           # > sco
+0001a820: 6f70 2069 6e73 7461 6c6c 2061 7269 6132  op install aria2
+0001a830: 206c 6573 730a 2020 2020 2020 2020 2020   less.          
+0001a840: 2020 2020 2020 2020 2020 6966 2072 652e            if re.
+0001a850: 7365 6172 6368 2822 3c5b 5e3c 3e5d 2b3f  search("<[^<>]+?
+0001a860: 3e22 2c20 7061 6765 7243 6f6e 7465 6e74  >", pagerContent
+0001a870: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001a880: 2020 2020 2020 2020 2020 2070 6167 6572             pager
+0001a890: 436f 6e74 656e 7420 3d20 5465 7874 5574  Content = TextUt
+0001a8a0: 696c 2e63 6f6e 7665 7274 4874 6d6c 5461  il.convertHtmlTa
+0001a8b0: 6754 6f43 6f6c 6f72 616d 6128 7061 6765  gToColorama(page
+0001a8c0: 7243 6f6e 7465 6e74 290a 2020 2020 2020  rContent).      
+0001a8d0: 2020 2020 2020 2020 2020 2020 2020 7079                py
+0001a8e0: 646f 632e 7069 7065 7061 6765 7228 7061  doc.pipepager(pa
+0001a8f0: 6765 7243 6f6e 7465 6e74 2c20 636d 643d  gerContent, cmd=
+0001a900: 276c 6573 7320 2d52 2729 0a20 2020 2020  'less -R').     
+0001a910: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001a920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a930: 2020 2020 2070 7964 6f63 2e70 6167 6572       pydoc.pager
+0001a940: 2870 6167 6572 436f 6e74 656e 7429 0a20  (pagerContent). 
+0001a950: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0001a960: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0001a970: 2020 2063 6f6e 6669 672e 7061 6765 7256     config.pagerV
+0001a980: 6965 7720 3d20 4661 6c73 650a 2020 2020  iew = False.    
+0001a990: 2020 2020 2020 2020 2020 2020 7368 6f77              show
+0001a9a0: 4572 726f 7273 2829 0a0a 2020 2020 2320  Errors()..    # 
+0001a9b0: 7772 6170 2068 746d 6c20 7465 7874 2061  wrap html text a
+0001a9c0: 7420 7370 6163 6573 0a20 2020 2064 6566  t spaces.    def
+0001a9d0: 2067 6574 5772 6170 7065 6448 544d 4c54   getWrappedHTMLT
+0001a9e0: 6578 7428 7365 6c66 2c20 7465 7874 2c20  ext(self, text, 
+0001a9f0: 7465 726d 696e 616c 5f77 6964 7468 3d4e  terminal_width=N
+0001aa00: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
+0001aa10: 206e 6f74 2022 2022 2069 6e20 7465 7874   not " " in text
+0001aa20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0001aa30: 7475 726e 2074 6578 740a 2020 2020 2020  turn text.      
+0001aa40: 2020 6966 2074 6572 6d69 6e61 6c5f 7769    if terminal_wi
+0001aa50: 6474 6820 6973 204e 6f6e 653a 0a20 2020  dth is None:.   
+0001aa60: 2020 2020 2020 2020 2074 6572 6d69 6e61           termina
+0001aa70: 6c5f 7769 6474 6820 3d20 7368 7574 696c  l_width = shutil
+0001aa80: 2e67 6574 5f74 6572 6d69 6e61 6c5f 7369  .get_terminal_si
+0001aa90: 7a65 2829 2e63 6f6c 756d 6e73 0a20 2020  ze().columns.   
+0001aaa0: 2020 2020 2073 656c 662e 7772 6170 7065       self.wrappe
+0001aab0: 6454 6578 7420 3d20 2222 0a20 2020 2020  dText = "".     
+0001aac0: 2020 2073 656c 662e 6c69 6e65 5769 6474     self.lineWidt
+0001aad0: 6820 3d20 300a 0a20 2020 2020 2020 2064  h = 0..        d
+0001aae0: 6566 2061 6464 576f 7264 7328 776f 7264  ef addWords(word
+0001aaf0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0001ab00: 776f 7264 7320 3d20 776f 7264 732e 7370  words = words.sp
+0001ab10: 6c69 7428 2220 2229 0a20 2020 2020 2020  lit(" ").       
+0001ab20: 2020 2020 2066 6f72 2069 6e64 6578 2c20       for index, 
+0001ab30: 6974 656d 2069 6e20 656e 756d 6572 6174  item in enumerat
+0001ab40: 6528 776f 7264 7329 3a0a 2020 2020 2020  e(words):.      
+0001ab50: 2020 2020 2020 2020 2020 6973 4c61 7374            isLast
+0001ab60: 4974 656d 203d 2028 6c65 6e28 776f 7264  Item = (len(word
+0001ab70: 7329 202d 2069 6e64 6578 203d 3d20 3129  s) - index == 1)
+0001ab80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ab90: 2069 6620 6973 5f43 4a4b 2869 7465 6d29   if is_CJK(item)
+0001aba0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001abb0: 2020 2020 2020 666f 7220 6949 6e64 6578        for iIndex
+0001abc0: 2c20 6920 696e 2065 6e75 6d65 7261 7465  , i in enumerate
+0001abd0: 2869 7465 6d29 3a0a 2020 2020 2020 2020  (item):.        
 0001abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001abf0: 2020 2020 2020 6973 5370 6163 6549 7465        isSpaceIte
-0001ac00: 6d20 3d20 286e 6f74 2069 734c 6173 7449  m = (not isLastI
-0001ac10: 7465 6d20 616e 6420 286c 656e 2869 7465  tem and (len(ite
-0001ac20: 6d29 202d 2069 496e 6465 7820 3d3d 2031  m) - iIndex == 1
-0001ac30: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0001ac40: 2020 2020 2020 2020 2020 2069 5769 6474             iWidt
-0001ac50: 6820 3d20 6765 7453 7472 696e 6757 6964  h = getStringWid
-0001ac60: 7468 2869 290a 2020 2020 2020 2020 2020  th(i).          
-0001ac70: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001ac80: 2069 7353 7061 6365 4974 656d 3a0a 2020   isSpaceItem:.  
+0001abf0: 6973 5370 6163 6549 7465 6d20 3d20 286e  isSpaceItem = (n
+0001ac00: 6f74 2069 734c 6173 7449 7465 6d20 616e  ot isLastItem an
+0001ac10: 6420 286c 656e 2869 7465 6d29 202d 2069  d (len(item) - i
+0001ac20: 496e 6465 7820 3d3d 2031 2929 0a20 2020  Index == 1)).   
+0001ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac40: 2020 2020 2069 5769 6474 6820 3d20 6765       iWidth = ge
+0001ac50: 7453 7472 696e 6757 6964 7468 2869 290a  tStringWidth(i).
+0001ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac70: 2020 2020 2020 2020 6966 2069 7353 7061          if isSpa
+0001ac80: 6365 4974 656d 3a0a 2020 2020 2020 2020  ceItem:.        
 0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aca0: 2020 2020 2020 2020 2020 6e65 774c 696e            newLin
-0001acb0: 6557 6964 7468 203d 2073 656c 662e 6c69  eWidth = self.li
-0001acc0: 6e65 5769 6474 6820 2b20 6957 6964 7468  neWidth + iWidth
-0001acd0: 202b 2031 0a20 2020 2020 2020 2020 2020   + 1.           
-0001ace0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0001acf0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001ad00: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0001ad10: 6577 4c69 6e65 5769 6474 6820 3d20 7365  ewLineWidth = se
-0001ad20: 6c66 2e6c 696e 6557 6964 7468 202b 2069  lf.lineWidth + i
-0001ad30: 5769 6474 680a 2020 2020 2020 2020 2020  Width.          
-0001ad40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001ad50: 206e 6577 4c69 6e65 5769 6474 6820 3e20   newLineWidth > 
-0001ad60: 7465 726d 696e 616c 5f77 6964 7468 3a0a  terminal_width:.
+0001aca0: 2020 2020 6e65 774c 696e 6557 6964 7468      newLineWidth
+0001acb0: 203d 2073 656c 662e 6c69 6e65 5769 6474   = self.lineWidt
+0001acc0: 6820 2b20 6957 6964 7468 202b 2031 0a20  h + iWidth + 1. 
+0001acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ace0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad00: 2020 2020 2020 2020 206e 6577 4c69 6e65           newLine
+0001ad10: 5769 6474 6820 3d20 7365 6c66 2e6c 696e  Width = self.lin
+0001ad20: 6557 6964 7468 202b 2069 5769 6474 680a  eWidth + iWidth.
+0001ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad40: 2020 2020 2020 2020 6966 206e 6577 4c69          if newLi
+0001ad50: 6e65 5769 6474 6820 3e20 7465 726d 696e  neWidth > termin
+0001ad60: 616c 5f77 6964 7468 3a0a 2020 2020 2020  al_width:.      
 0001ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001ad90: 2e77 7261 7070 6564 5465 7874 202b 3d20  .wrappedText += 
-0001ada0: 6622 5c6e 7b69 7d20 2220 6966 2069 7353  f"\n{i} " if isS
-0001adb0: 7061 6365 4974 656d 2065 6c73 6520 6622  paceItem else f"
-0001adc0: 5c6e 7b69 7d22 0a20 2020 2020 2020 2020  \n{i}".         
-0001add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ade0: 2020 2073 656c 662e 6c69 6e65 5769 6474     self.lineWidt
-0001adf0: 6820 3d20 6957 6964 7468 202b 2031 2069  h = iWidth + 1 i
-0001ae00: 6620 6973 5370 6163 6549 7465 6d20 656c  f isSpaceItem el
-0001ae10: 7365 2069 5769 6474 680a 2020 2020 2020  se iWidth.      
-0001ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae50: 2020 2020 7365 6c66 2e77 7261 7070 6564      self.wrapped
-0001ae60: 5465 7874 202b 3d20 6622 7b69 7d20 2220  Text += f"{i} " 
-0001ae70: 6966 2069 7353 7061 6365 4974 656d 2065  if isSpaceItem e
-0001ae80: 6c73 6520 690a 2020 2020 2020 2020 2020  lse i.          
-0001ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aea0: 2020 7365 6c66 2e6c 696e 6557 6964 7468    self.lineWidth
-0001aeb0: 202b 3d20 6957 6964 7468 202b 2031 2069   += iWidth + 1 i
-0001aec0: 6620 6973 5370 6163 6549 7465 6d20 656c  f isSpaceItem el
-0001aed0: 7365 2069 5769 6474 680a 2020 2020 2020  se iWidth.      
-0001aee0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0001aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af00: 2020 2020 6974 656d 5769 6474 6820 3d20      itemWidth = 
-0001af10: 6765 7453 7472 696e 6757 6964 7468 2869  getStringWidth(i
-0001af20: 7465 6d29 0a20 2020 2020 2020 2020 2020  tem).           
-0001af30: 2020 2020 2020 2020 2069 6620 6973 4c61           if isLa
-0001af40: 7374 4974 656d 3a0a 2020 2020 2020 2020  stItem:.        
-0001af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af60: 6e65 774c 696e 6557 6964 7468 203d 2073  newLineWidth = s
-0001af70: 656c 662e 6c69 6e65 5769 6474 6820 2b20  elf.lineWidth + 
-0001af80: 6974 656d 5769 6474 680a 2020 2020 2020  itemWidth.      
-0001af90: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0001afa0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001afb0: 2020 2020 2020 2020 2020 2020 6e65 774c              newL
-0001afc0: 696e 6557 6964 7468 203d 2073 656c 662e  ineWidth = self.
-0001afd0: 6c69 6e65 5769 6474 6820 2b20 6974 656d  lineWidth + item
-0001afe0: 5769 6474 6820 2b20 310a 2020 2020 2020  Width + 1.      
-0001aff0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001b000: 206e 6577 4c69 6e65 5769 6474 6820 3e20   newLineWidth > 
-0001b010: 7465 726d 696e 616c 5f77 6964 7468 3a0a  terminal_width:.
+0001ad80: 2020 2020 2020 7365 6c66 2e77 7261 7070        self.wrapp
+0001ad90: 6564 5465 7874 202b 3d20 6622 5c6e 7b69  edText += f"\n{i
+0001ada0: 7d20 2220 6966 2069 7353 7061 6365 4974  } " if isSpaceIt
+0001adb0: 656d 2065 6c73 6520 6622 5c6e 7b69 7d22  em else f"\n{i}"
+0001adc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001add0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001ade0: 662e 6c69 6e65 5769 6474 6820 3d20 6957  f.lineWidth = iW
+0001adf0: 6964 7468 202b 2031 2069 6620 6973 5370  idth + 1 if isSp
+0001ae00: 6163 6549 7465 6d20 656c 7365 2069 5769  aceItem else iWi
+0001ae10: 6474 680a 2020 2020 2020 2020 2020 2020  dth.            
+0001ae20: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001ae30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001ae40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001ae50: 6c66 2e77 7261 7070 6564 5465 7874 202b  lf.wrappedText +
+0001ae60: 3d20 6622 7b69 7d20 2220 6966 2069 7353  = f"{i} " if isS
+0001ae70: 7061 6365 4974 656d 2065 6c73 6520 690a  paceItem else i.
+0001ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001aea0: 2e6c 696e 6557 6964 7468 202b 3d20 6957  .lineWidth += iW
+0001aeb0: 6964 7468 202b 2031 2069 6620 6973 5370  idth + 1 if isSp
+0001aec0: 6163 6549 7465 6d20 656c 7365 2069 5769  aceItem else iWi
+0001aed0: 6474 680a 2020 2020 2020 2020 2020 2020  dth.            
+0001aee0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001aef0: 2020 2020 2020 2020 2020 2020 2020 6974                it
+0001af00: 656d 5769 6474 6820 3d20 6765 7453 7472  emWidth = getStr
+0001af10: 696e 6757 6964 7468 2869 7465 6d29 0a20  ingWidth(item). 
+0001af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af30: 2020 2069 6620 6973 4c61 7374 4974 656d     if isLastItem
+0001af40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001af50: 2020 2020 2020 2020 2020 6e65 774c 696e            newLin
+0001af60: 6557 6964 7468 203d 2073 656c 662e 6c69  eWidth = self.li
+0001af70: 6e65 5769 6474 6820 2b20 6974 656d 5769  neWidth + itemWi
+0001af80: 6474 680a 2020 2020 2020 2020 2020 2020  dth.            
+0001af90: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afb0: 2020 2020 2020 6e65 774c 696e 6557 6964        newLineWid
+0001afc0: 7468 203d 2073 656c 662e 6c69 6e65 5769  th = self.lineWi
+0001afd0: 6474 6820 2b20 6974 656d 5769 6474 6820  dth + itemWidth 
+0001afe0: 2b20 310a 2020 2020 2020 2020 2020 2020  + 1.            
+0001aff0: 2020 2020 2020 2020 6966 206e 6577 4c69          if newLi
+0001b000: 6e65 5769 6474 6820 3e20 7465 726d 696e  neWidth > termin
+0001b010: 616c 5f77 6964 7468 3a0a 2020 2020 2020  al_width:.      
 0001b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b030: 2020 2020 2020 2020 7365 6c66 2e77 7261          self.wra
-0001b040: 7070 6564 5465 7874 202b 3d20 6622 5c6e  ppedText += f"\n
-0001b050: 7b69 7465 6d7d 2220 6966 2069 734c 6173  {item}" if isLas
-0001b060: 7449 7465 6d20 656c 7365 2066 225c 6e7b  tItem else f"\n{
-0001b070: 6974 656d 7d20 220a 2020 2020 2020 2020  item} ".        
-0001b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b090: 7365 6c66 2e6c 696e 6557 6964 7468 203d  self.lineWidth =
-0001b0a0: 2069 7465 6d57 6964 7468 2069 6620 6973   itemWidth if is
-0001b0b0: 4c61 7374 4974 656d 2065 6c73 6520 6974  LastItem else it
-0001b0c0: 656d 5769 6474 6820 2b20 310a 2020 2020  emWidth + 1.    
-0001b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b0e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001b0f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001b100: 6c66 2e77 7261 7070 6564 5465 7874 202b  lf.wrappedText +
-0001b110: 3d20 6974 656d 2069 6620 6973 4c61 7374  = item if isLast
-0001b120: 4974 656d 2065 6c73 6520 6622 7b69 7465  Item else f"{ite
-0001b130: 6d7d 2022 0a20 2020 2020 2020 2020 2020  m} ".           
-0001b140: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001b150: 662e 6c69 6e65 5769 6474 6820 2b3d 2069  f.lineWidth += i
-0001b160: 7465 6d57 6964 7468 2069 6620 6973 4c61  temWidth if isLa
-0001b170: 7374 4974 656d 2065 6c73 6520 6974 656d  stItem else item
-0001b180: 5769 6474 6820 2b20 310a 0a20 2020 2020  Width + 1..     
-0001b190: 2020 2064 6566 2070 726f 6365 7373 4c69     def processLi
-0001b1a0: 6e65 286c 696e 6554 6578 7429 3a0a 2020  ne(lineText):.  
-0001b1b0: 2020 2020 2020 2020 2020 6966 2072 652e            if re.
-0001b1c0: 7365 6172 6368 2822 3c5b 5e3c 3e5d 2b3f  search("<[^<>]+?
-0001b1d0: 3e22 2c20 6c69 6e65 5465 7874 293a 0a20  >", lineText):. 
-0001b1e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001b1f0: 2068 616e 646c 6520 6874 6d6c 2f78 6d6c   handle html/xml
-0001b200: 2074 6167 730a 2020 2020 2020 2020 2020   tags.          
-0001b210: 2020 2020 2020 6368 756e 6b73 203d 206c        chunks = l
-0001b220: 696e 6554 6578 742e 7370 6c69 7428 223e  ineText.split(">
-0001b230: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0001b240: 2020 2074 6f74 616c 4368 756e 6b73 203d     totalChunks =
-0001b250: 206c 656e 2863 6875 6e6b 7329 0a20 2020   len(chunks).   
-0001b260: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0001b270: 2069 6e64 6578 2c20 6368 756e 6b20 696e   index, chunk in
-0001b280: 2065 6e75 6d65 7261 7465 2863 6875 6e6b   enumerate(chunk
-0001b290: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0001b2a0: 2020 2020 2020 2020 6973 4c61 7374 4368          isLastCh
-0001b2b0: 756e 6b20 3d20 2874 6f74 616c 4368 756e  unk = (totalChun
-0001b2c0: 6b73 202d 2069 6e64 6578 203d 3d20 3129  ks - index == 1)
-0001b2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b2e0: 2020 2020 2069 6620 6973 4c61 7374 4368       if isLastCh
-0001b2f0: 756e 6b3a 0a20 2020 2020 2020 2020 2020  unk:.           
-0001b300: 2020 2020 2020 2020 2020 2020 2061 6464               add
-0001b310: 576f 7264 7328 6368 756e 6b29 0a20 2020  Words(chunk).   
-0001b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b330: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001b340: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001b350: 6167 203d 2054 7275 6520 6966 2022 3c22  ag = True if "<"
-0001b360: 2069 6e20 6368 756e 6b20 656c 7365 2046   in chunk else F
-0001b370: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-0001b380: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001b390: 7461 673a 0a20 2020 2020 2020 2020 2020  tag:.           
-0001b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3b0: 206e 6f6e 5461 672c 2074 6167 436f 6e74   nonTag, tagCont
-0001b3c0: 656e 7420 3d20 6368 756e 6b2e 7273 706c  ent = chunk.rspl
-0001b3d0: 6974 2822 3c22 2c20 3129 0a20 2020 2020  it("<", 1).     
+0001b030: 2020 7365 6c66 2e77 7261 7070 6564 5465    self.wrappedTe
+0001b040: 7874 202b 3d20 6622 5c6e 7b69 7465 6d7d  xt += f"\n{item}
+0001b050: 2220 6966 2069 734c 6173 7449 7465 6d20  " if isLastItem 
+0001b060: 656c 7365 2066 225c 6e7b 6974 656d 7d20  else f"\n{item} 
+0001b070: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0001b080: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0001b090: 696e 6557 6964 7468 203d 2069 7465 6d57  ineWidth = itemW
+0001b0a0: 6964 7468 2069 6620 6973 4c61 7374 4974  idth if isLastIt
+0001b0b0: 656d 2065 6c73 6520 6974 656d 5769 6474  em else itemWidt
+0001b0c0: 6820 2b20 310a 2020 2020 2020 2020 2020  h + 1.          
+0001b0d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0001b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0f0: 2020 2020 2020 2020 7365 6c66 2e77 7261          self.wra
+0001b100: 7070 6564 5465 7874 202b 3d20 6974 656d  ppedText += item
+0001b110: 2069 6620 6973 4c61 7374 4974 656d 2065   if isLastItem e
+0001b120: 6c73 6520 6622 7b69 7465 6d7d 2022 0a20  lse f"{item} ". 
+0001b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b140: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
+0001b150: 5769 6474 6820 2b3d 2069 7465 6d57 6964  Width += itemWid
+0001b160: 7468 2069 6620 6973 4c61 7374 4974 656d  th if isLastItem
+0001b170: 2065 6c73 6520 6974 656d 5769 6474 6820   else itemWidth 
+0001b180: 2b20 310a 0a20 2020 2020 2020 2064 6566  + 1..        def
+0001b190: 2070 726f 6365 7373 4c69 6e65 286c 696e   processLine(lin
+0001b1a0: 6554 6578 7429 3a0a 2020 2020 2020 2020  eText):.        
+0001b1b0: 2020 2020 6966 2072 652e 7365 6172 6368      if re.search
+0001b1c0: 2822 3c5b 5e3c 3e5d 2b3f 3e22 2c20 6c69  ("<[^<>]+?>", li
+0001b1d0: 6e65 5465 7874 293a 0a20 2020 2020 2020  neText):.       
+0001b1e0: 2020 2020 2020 2020 2023 2068 616e 646c           # handl
+0001b1f0: 6520 6874 6d6c 2f78 6d6c 2074 6167 730a  e html/xml tags.
+0001b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b210: 6368 756e 6b73 203d 206c 696e 6554 6578  chunks = lineTex
+0001b220: 742e 7370 6c69 7428 223e 2229 0a20 2020  t.split(">").   
+0001b230: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
+0001b240: 616c 4368 756e 6b73 203d 206c 656e 2863  alChunks = len(c
+0001b250: 6875 6e6b 7329 0a20 2020 2020 2020 2020  hunks).         
+0001b260: 2020 2020 2020 2066 6f72 2069 6e64 6578         for index
+0001b270: 2c20 6368 756e 6b20 696e 2065 6e75 6d65  , chunk in enume
+0001b280: 7261 7465 2863 6875 6e6b 7329 3a0a 2020  rate(chunks):.  
+0001b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b2a0: 2020 6973 4c61 7374 4368 756e 6b20 3d20    isLastChunk = 
+0001b2b0: 2874 6f74 616c 4368 756e 6b73 202d 2069  (totalChunks - i
+0001b2c0: 6e64 6578 203d 3d20 3129 0a20 2020 2020  ndex == 1).     
+0001b2d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001b2e0: 6620 6973 4c61 7374 4368 756e 6b3a 0a20  f isLastChunk:. 
+0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b300: 2020 2020 2020 2061 6464 576f 7264 7328         addWords(
+0001b310: 6368 756e 6b29 0a20 2020 2020 2020 2020  chunk).         
+0001b320: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001b330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b340: 2020 2020 2020 2020 2074 6167 203d 2054           tag = T
+0001b350: 7275 6520 6966 2022 3c22 2069 6e20 6368  rue if "<" in ch
+0001b360: 756e 6b20 656c 7365 2046 616c 7365 0a20  unk else False. 
+0001b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b380: 2020 2020 2020 2069 6620 7461 673a 0a20         if tag:. 
+0001b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b3a0: 2020 2020 2020 2020 2020 206e 6f6e 5461             nonTa
+0001b3b0: 672c 2074 6167 436f 6e74 656e 7420 3d20  g, tagContent = 
+0001b3c0: 6368 756e 6b2e 7273 706c 6974 2822 3c22  chunk.rsplit("<"
+0001b3d0: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
 0001b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3f0: 2020 2020 2020 2061 6464 576f 7264 7328         addWords(
-0001b400: 6e6f 6e54 6167 290a 2020 2020 2020 2020  nonTag).        
-0001b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b420: 2020 2020 7365 6c66 2e77 7261 7070 6564      self.wrapped
-0001b430: 5465 7874 202b 3d20 6622 3c7b 7461 6743  Text += f"<{tagC
-0001b440: 6f6e 7465 6e74 7d3e 220a 2020 2020 2020  ontent}>".      
-0001b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b460: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b480: 2020 2020 6164 6457 6f72 6473 2866 227b      addWords(f"{
-0001b490: 6368 756e 6b7d 3e22 290a 2020 2020 2020  chunk}>").      
-0001b4a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001b4b0: 2020 2020 2020 2020 2020 2020 6164 6457              addW
-0001b4c0: 6f72 6473 286c 696e 6554 6578 7429 0a0a  ords(lineText)..
-0001b4d0: 2020 2020 2020 2020 6c69 6e65 7320 3d20          lines = 
-0001b4e0: 7465 7874 2e73 706c 6974 2822 5c6e 2229  text.split("\n")
-0001b4f0: 0a20 2020 2020 2020 2074 6f74 616c 4c69  .        totalLi
-0001b500: 6e65 7320 3d20 6c65 6e28 6c69 6e65 7329  nes = len(lines)
-0001b510: 0a20 2020 2020 2020 2066 6f72 2069 6e64  .        for ind
-0001b520: 6578 2c20 6c69 6e65 2069 6e20 656e 756d  ex, line in enum
-0001b530: 6572 6174 6528 6c69 6e65 7329 3a0a 2020  erate(lines):.  
-0001b540: 2020 2020 2020 2020 2020 6973 4c61 7374            isLast
-0001b550: 4c69 6e65 203d 2028 746f 7461 6c4c 696e  Line = (totalLin
-0001b560: 6573 202d 2069 6e64 6578 203d 3d20 3129  es - index == 1)
-0001b570: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-0001b580: 6365 7373 4c69 6e65 286c 696e 6529 0a20  cessLine(line). 
-0001b590: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0001b5a0: 7420 6973 4c61 7374 4c69 6e65 3a0a 2020  t isLastLine:.  
-0001b5b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001b5c0: 6c66 2e77 7261 7070 6564 5465 7874 202b  lf.wrappedText +
-0001b5d0: 3d20 225c 6e22 0a20 2020 2020 2020 2020  = "\n".         
-0001b5e0: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
-0001b5f0: 5769 6474 6820 3d20 300a 0a20 2020 2020  Width = 0..     
-0001b600: 2020 2072 6574 7572 6e20 7365 6c66 2e77     return self.w
-0001b610: 7261 7070 6564 5465 7874 0a              rappedText.
+0001b3f0: 2061 6464 576f 7264 7328 6e6f 6e54 6167   addWords(nonTag
+0001b400: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001b410: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001b420: 6c66 2e77 7261 7070 6564 5465 7874 202b  lf.wrappedText +
+0001b430: 3d20 6622 3c7b 7461 6743 6f6e 7465 6e74  = f"<{tagContent
+0001b440: 7d3e 220a 2020 2020 2020 2020 2020 2020  }>".            
+0001b450: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001b460: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b470: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+0001b480: 6457 6f72 6473 2866 227b 6368 756e 6b7d  dWords(f"{chunk}
+0001b490: 3e22 290a 2020 2020 2020 2020 2020 2020  >").            
+0001b4a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001b4b0: 2020 2020 2020 6164 6457 6f72 6473 286c        addWords(l
+0001b4c0: 696e 6554 6578 7429 0a0a 2020 2020 2020  ineText)..      
+0001b4d0: 2020 6c69 6e65 7320 3d20 7465 7874 2e73    lines = text.s
+0001b4e0: 706c 6974 2822 5c6e 2229 0a20 2020 2020  plit("\n").     
+0001b4f0: 2020 2074 6f74 616c 4c69 6e65 7320 3d20     totalLines = 
+0001b500: 6c65 6e28 6c69 6e65 7329 0a20 2020 2020  len(lines).     
+0001b510: 2020 2066 6f72 2069 6e64 6578 2c20 6c69     for index, li
+0001b520: 6e65 2069 6e20 656e 756d 6572 6174 6528  ne in enumerate(
+0001b530: 6c69 6e65 7329 3a0a 2020 2020 2020 2020  lines):.        
+0001b540: 2020 2020 6973 4c61 7374 4c69 6e65 203d      isLastLine =
+0001b550: 2028 746f 7461 6c4c 696e 6573 202d 2069   (totalLines - i
+0001b560: 6e64 6578 203d 3d20 3129 0a20 2020 2020  ndex == 1).     
+0001b570: 2020 2020 2020 2070 726f 6365 7373 4c69         processLi
+0001b580: 6e65 286c 696e 6529 0a20 2020 2020 2020  ne(line).       
+0001b590: 2020 2020 2069 6620 6e6f 7420 6973 4c61       if not isLa
+0001b5a0: 7374 4c69 6e65 3a0a 2020 2020 2020 2020  stLine:.        
+0001b5b0: 2020 2020 2020 2020 7365 6c66 2e77 7261          self.wra
+0001b5c0: 7070 6564 5465 7874 202b 3d20 225c 6e22  ppedText += "\n"
+0001b5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b5e0: 2073 656c 662e 6c69 6e65 5769 6474 6820   self.lineWidth 
+0001b5f0: 3d20 300a 0a20 2020 2020 2020 2072 6574  = 0..        ret
+0001b600: 7572 6e20 7365 6c66 2e77 7261 7070 6564  urn self.wrapped
+0001b610: 5465 7874 0a                             Text.
```

### Comparing `freegenius-0.1.8/freegenius/utils/call_chatgpt.py` & `freegenius-0.1.9/freegenius/utils/call_chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,15 @@
             max_tokens=getDynamicTokens(messages),
             stream=True,
             **kwargs,
         )
 
     @staticmethod
     @check_openai_errors
-    def getResponseDict(messages: list, schema: dict, **kwargs) -> dict:
+    def getDictionaryOutput(messages: list, schema: dict, **kwargs) -> dict:
         completion = config.oai_client.chat.completions.create(
             model=config.chatGPTApiModel,
             messages=messages,
             n=1,
             temperature=config.llmTemperature,
             max_tokens=getDynamicTokens(messages, [schema]),
             tools=[{"type": "function", "function": schema}],
@@ -403,15 +403,15 @@
             if tool_name == "chat":
                 return CallChatGPT.regularCall(messages)
             # 3. Parameter Extraction
             if config.developer:
                 print1("extracting parameters ...")
             try:
                 #tool_parameters = CallChatGPT.extractToolParameters(schema=tool_schema, ongoingMessages=messages)
-                tool_parameters = CallChatGPT.getResponseDict(messages=messages, schema=tool_schema)
+                tool_parameters = CallChatGPT.getDictionaryOutput(messages=messages, schema=tool_schema)
                 if not tool_parameters:
                     if config.developer:
                         print1("Failed to extract parameters!")
                     return CallChatGPT.regularCall(messages)
                 # 4. Function Execution
                 tool_response = executeToolFunction(func_arguments=tool_parameters, function_name=tool_name)
             except:
@@ -477,26 +477,26 @@
             "description": f'''Estimate user request''',
             "parameters": {
                 "type": "object",
                 "properties": properties,
                 "required": ["code"],
             },
         }
-        output = CallChatGPT.getResponseDict(messages, schema=schema)
+        output = CallChatGPT.getDictionaryOutput(messages, schema=schema)
         chatOnly = True if "yes" in str(output).lower() else False
         print3(f"""Tool may {"not " if chatOnly else ""}be required.""")
         print2("```")
         return chatOnly
 
     @staticmethod
     def extractToolParameters(schema: dict, ongoingMessages: list = [], **kwargs) -> dict:
         """
         Extract action parameters
         """
-        parameters = CallChatGPT.getResponseDict(messages=ongoingMessages, schema=schema, **kwargs)
+        parameters = CallChatGPT.getDictionaryOutput(messages=ongoingMessages, schema=schema, **kwargs)
         if config.developer:
             print2("```parameters")
             pprint.pprint(parameters)
             print2("```")
         return parameters
```

### Comparing `freegenius-0.1.8/freegenius/utils/call_gemini.py` & `freegenius-0.1.9/freegenius/utils/call_gemini.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             generation_config=config.geminipro_generation_config,
             safety_settings=config.geminipro_safety_settings,
             stream=True,
             **kwargs,
         )
 
     @staticmethod
-    def getResponseDict(history: list, schema: dict, userMessage: str, **kwargs) -> dict:
+    def getDictionaryOutput(history: list, schema: dict, userMessage: str, **kwargs) -> dict:
         name, description, parameters = schema["name"], schema["description"], schema["parameters"]
         chat = config.geminipro_model.start_chat(history=history)
         # declare a function
         function_declaration = FunctionDeclaration(
             name=name,
             description=description,
             parameters=parameters,
@@ -319,15 +319,15 @@
 
 <request>
 {user_request}{deviceInfo}
 </request>"""
 
         history, *_ = toGeminiMessages(messages=messages)
 
-        output = CallGemini.getResponseDict(history, schema=schema, userMessage=userMessage)
+        output = CallGemini.getDictionaryOutput(history, schema=schema, userMessage=userMessage)
         chatOnly = True if "yes" in str(output).lower() else False
         print3(f"""Tool may {"not " if chatOnly else ""}be required.""")
         print2("```")
         return chatOnly
 
     @staticmethod
     def extractToolParameters(schema: dict, userInput: str, ongoingMessages: list = [], **kwargs) -> dict:
@@ -373,15 +373,15 @@
         
         userMessage = f"""<request>
 {lastUserMessage}
 </request>{deviceInfo}{code}
 
 When necessary, generate content based on your knowledge."""
 
-        parameters = CallGemini.getResponseDict(history=history, schema=schema, userMessage=userMessage, **kwargs)
+        parameters = CallGemini.getDictionaryOutput(history=history, schema=schema, userMessage=userMessage, **kwargs)
         # fix linebreak
         if code and "code" in parameters:
             parameters["code"] = codecs.decode(parameters["code"], "unicode_escape")
 
         if config.developer:
             print2("```parameters")
             pprint.pprint(parameters)
```

### Comparing `freegenius-0.1.8/freegenius/utils/call_groq.py` & `freegenius-0.1.9/freegenius/utils/call_groq.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from freegenius import showErrors, get_or_create_collection, query_vectors, showRisk, executeToolFunction, getPythonFunctionResponse, getPygmentsStyle, fineTunePythonCode, confirmExecution
 from freegenius import config
-from freegenius import print1, print2, print3, selectTool, check_llm_errors, getGroqClient
+from freegenius import print1, print2, print3, selectTool, check_llm_errors, getGroqClient, toParameterSchema, extractPythonCode
 import re, traceback, pprint, copy, textwrap, json, pygments
 from pygments.lexers.python import PythonLexer
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit.formatted_text import PygmentsTokens
 from prompt_toolkit import prompt
-from groq import Groq
+from typing import Optional
 
 class CallGroq:
 
     @staticmethod
     def riskAssessment(code):
         content = f"""You are a senior python engineer.
     Assess the risk level of damaging my device upon executing the python code that I will provide for you.
@@ -79,26 +79,28 @@
             config.defaultEntry = f"```python\n{code}\n```"
             return ""
         else:
             return "[INVALID]"
 
     @staticmethod
     @check_llm_errors
-    def getSingleChatResponse(userInput, messages=[], temperature=None):
+    def getSingleChatResponse(userInput, messages=[], temperature: Optional[float]=None, max_tokens: Optional[int]=None):
         """
         non-streaming single call
         """
         messages.append({"role": "user", "content" : userInput})
         try:
             completion = getGroqClient().chat.completions.create(
                 model=config.groqApi_main_model,
                 messages=messages,
                 n=1,
                 temperature=temperature if temperature is not None else config.llmTemperature,
-                max_tokens=config.groqApi_max_tokens,
+                max_tokens=max_tokens if max_tokens is not None else config.groqApi_max_tokens,
+                stream=False,
+                **config.groqApi_main_model_additional_chat_options,
             )
             return completion.choices[0].message.content
         except:
             return ""
 
     @staticmethod
     def finetuneSingleFunctionCallResponse(func_arguments, function_name):
@@ -187,26 +189,26 @@
         except:
             showErrors()
             return messagesCopy
         return messages
 
     @staticmethod
     @check_llm_errors
-    def getSingleFunctionCallResponse(messages: list[dict], function_name: str, temperature=None, **kwargs):
+    def getSingleFunctionCallResponse(messages: list[dict], function_name: str, temperature: Optional[float]=None, max_tokens: Optional[int]=None):
         functionSignatures = [config.toolFunctionSchemas[function_name]]
         completion = getGroqClient().chat.completions.create(
             model=config.groqApi_main_model,
             messages=messages,
             n=1,
             temperature=temperature if temperature is not None else config.llmTemperature,
-            max_tokens=config.groqApi_max_tokens,
+            max_tokens=max_tokens if max_tokens is not None else config.groqApi_max_tokens,
             tools=CallGroq.convertFunctionSignaturesIntoTools(functionSignatures),
             tool_choice={"type": "function", "function": {"name": function_name}},
             stream=False,
-            **kwargs,
+            **config.groqApi_main_model_additional_chat_options,
         )
         function_call_message = completion.choices[0].message
         tool_call = function_call_message.tool_calls[0]
         func_arguments = tool_call.function.arguments
         function_call_message_mini = {
             "role": "assistant",
             "content": "",
@@ -216,38 +218,38 @@
             }
         }
         function_call_response = CallGroq.finetuneSingleFunctionCallResponse(func_arguments, function_name)
         return function_call_message_mini, function_call_response
 
     @staticmethod
     @check_llm_errors
-    def regularCall(messages: dict, **kwargs):
+    def regularCall(messages: dict, temperature: Optional[float]=None, max_tokens: Optional[int]=None):
         return getGroqClient().chat.completions.create(
             model=config.groqApi_main_model,
             messages=messages,
             n=1,
-            temperature=config.llmTemperature,
-            max_tokens=config.groqApi_max_tokens,
+            temperature=temperature if temperature is not None else config.llmTemperature,
+            max_tokens=max_tokens if max_tokens is not None else config.groqApi_max_tokens,
             stream=True,
-            **kwargs,
+            **config.groqApi_main_model_additional_chat_options,
         )
 
     @staticmethod
     @check_llm_errors
-    def getResponseDict(messages: list, schema: dict, **kwargs) -> dict:
+    def getDictionaryOutput(messages: list, schema: dict, temperature: Optional[float]=None, max_tokens: Optional[int]=None) -> dict:
         completion = getGroqClient().chat.completions.create(
             model=config.groqApi_main_model,
             messages=messages,
             n=1,
-            temperature=config.llmTemperature,
-            max_tokens=config.groqApi_max_tokens,
+            temperature=temperature if temperature is not None else config.llmTemperature,
+            max_tokens=max_tokens if max_tokens is not None else config.groqApi_max_tokens,
             tools=[{"type": "function", "function": schema}],
             tool_choice={"type": "function", "function": {"name": schema["name"]}},
             stream=False,
-            **kwargs,
+            **config.groqApi_main_model_additional_chat_options,
         )
         responseDict = json.loads(completion.choices[0].message.tool_calls[0].function.arguments)
         return responseDict
 
     # Auto Function Call equivalence
 
     @staticmethod
@@ -295,16 +297,15 @@
                     print3(f"Selected: {tool_name} ({semantic_distance})")
             if tool_name == "chat":
                 return CallGroq.regularCall(messages)
             # 3. Parameter Extraction
             if config.developer:
                 print1("extracting parameters ...")
             try:
-                #tool_parameters = CallGroq.extractToolParameters(schema=tool_schema, ongoingMessages=messages)
-                tool_parameters = CallGroq.getResponseDict(messages=messages, schema=tool_schema)
+                tool_parameters = CallGroq.extractToolParameters(schema=tool_schema, userInput=user_request, ongoingMessages=messages)
                 if not tool_parameters:
                     if config.developer:
                         print1("Failed to extract parameters!")
                     return CallGroq.regularCall(messages)
                 # 4. Function Execution
                 tool_response = executeToolFunction(func_arguments=tool_parameters, function_name=tool_name)
             except:
@@ -361,24 +362,80 @@
             "description": f'''Estimate user request''',
             "parameters": {
                 "type": "object",
                 "properties": properties,
                 "required": ["code"],
             },
         }
-        output = CallGroq.getResponseDict(messages, schema=schema)
+        output = CallGroq.getDictionaryOutput(messages, schema=schema)
         chatOnly = True if "yes" in str(output).lower() else False
         print3(f"""Tool may {"not " if chatOnly else ""}be required.""")
         print2("```")
         return chatOnly
 
     @staticmethod
-    def extractToolParameters(schema: dict, ongoingMessages: list = [], **kwargs) -> dict:
+    def extractToolParameters(schema: dict, userInput: str, ongoingMessages: list = [], temperature: Optional[float]=None, max_tokens: Optional[int]=None) -> dict:
         """
         Extract action parameters
         """
-        parameters = CallGroq.getResponseDict(messages=ongoingMessages, schema=schema, **kwargs)
+        schema = toParameterSchema(schema)
+        schemaCopy = copy.deepcopy(schema)
+
+        # Generate Code when required
+        if "code" in schema["required"]:
+            del schemaCopy["properties"]["code"]
+            schemaCopy["required"].remove("code")
+            enforceCodeOutput = """ Remember, you should format the requested information, if any, into a string that is easily readable by humans. Use the 'print' function in the final line to display the requested information."""
+            code_instruction = schema["properties"]["code"]["description"] + enforceCodeOutput
+            code_instruction = f"""Generate python code according to the following instruction:
+</instruction>
+{code_instruction}
+</instruction>
+
+Here is my request:
+<request>
+{userInput}
+</request>
+
+Remember, response with the required python code ONLY, WITHOUT extra notes or explanations."""
+
+            code = CallGroq.getSingleChatResponse(code_instruction, ongoingMessages[:-1], temperature, max_tokens).replace(r"\\n", "\n")
+            code = extractPythonCode(code, keepInvalid=True)
+            if len(schema["properties"]) == 1:
+                return {"code": code}
+        else:
+            code = ""
+
+        codeContext = f"""
+
+Find required code below:
+{code}""" if code else ""
+
+        messages = ongoingMessages[:-2] + [
+            {
+                "role": "system",
+                "content": f"""You are a JSON builder expert that outputs in JSON.""",
+            },
+            {
+                "role": "user",
+                "content": f"""Response in JSON based on the following content:
+
+<content>
+{userInput}{codeContext}
+</content>
+
+Generate content to fill up the value of each required key in the JSON, if information is not provided.
+
+Remember, output in JSON.""",
+            },
+        ]
+
+        # schema alternative: properties if len(properties) == 1 else schema
+        parameters = CallGroq.getDictionaryOutput(messages, schemaCopy, temperature, max_tokens)
+        if code:
+            parameters["code"] = code
+
         if config.developer:
             print2("```parameters")
             pprint.pprint(parameters)
             print2("```")
         return parameters
```

### Comparing `freegenius-0.1.8/freegenius/utils/call_llamacpp.py` & `freegenius-0.1.9/freegenius/utils/call_llamacpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
                 **config.llamacppVisionModel_additional_chat_options,
             )
             return completion["choices"][0]["message"].get("content", "")
         except:
             return ""
 
     @staticmethod
-    def getResponseDict(messages: list, schema: dict={}, temperature: Optional[float]=None, max_tokens: Optional[int]=None) -> dict:
+    def getDictionaryOutput(messages: list, schema: dict={}, temperature: Optional[float]=None, max_tokens: Optional[int]=None) -> dict:
         schema = toParameterSchema(schema)
         try:
             completion = config.llamacppMainModel.create_chat_completion(
                 messages=messages,
                 response_format={"type": "json_object", "schema": schema} if schema else {"type": "json_object"},
                 temperature=temperature if temperature is not None else config.llmTemperature,
                 max_tokens=max_tokens if max_tokens is not None else config.llamacppMainModel_max_tokens,
@@ -278,18 +278,18 @@
             config.tempContent = ""
         except:
             showErrors()
             return messagesCopy
         return messages
 
     @staticmethod
-    def getSingleFunctionCallResponse(messages: list, function_name: str, temperature: Optional[float]=None, max_tokens: Optional[int]=None, **kwargs):
+    def getSingleFunctionCallResponse(messages: list, function_name: str, temperature: Optional[float]=None, max_tokens: Optional[int]=None):
         tool_schema = config.toolFunctionSchemas[function_name]["parameters"]
         user_request = messages[-1]["content"]
-        func_arguments = CallLlamaCpp.extractToolParameters(schema=tool_schema, userInput=user_request, ongoingMessages=messages, temperature=temperature, max_tokens=max_tokens, **kwargs)
+        func_arguments = CallLlamaCpp.extractToolParameters(schema=tool_schema, userInput=user_request, ongoingMessages=messages, temperature=temperature, max_tokens=max_tokens)
         function_call_response = executeToolFunction(func_arguments=func_arguments, function_name=function_name)
         function_call_message_mini = {
             "role": "assistant",
             "content": "",
             "function_call": {
                 "name": function_name,
                 "arguments": func_arguments,
@@ -441,23 +441,24 @@
 {user_request}{deviceInfo}
 </request>
 
 Remember, response in JSON with the filled template ONLY.""",
             },
         ]
 
-        output = CallLlamaCpp.getResponseDict(messages_for_screening, schema=schema, temperature=0.0, max_tokens=20)
+        output = CallLlamaCpp.getDictionaryOutput(messages_for_screening, schema=schema, temperature=0.0, max_tokens=20)
         try:
             output = output["answer"]
         except:
             return False
         return True if (not output) or str(output).lower() == "yes" else False
 
     @staticmethod
     def extractToolParameters_testing(schema: dict, userInput: str, ongoingMessages: list = [], temperature: Optional[float]=None, max_tokens: Optional[int]=None, **kwargs) -> dict:
+        # guidance
         lm = models.LlamaCpp(
             config.llamacppMainModel_model_path,
             echo = False,
             chat_format="chatml",
             n_ctx=config.llamacppMainModel_n_ctx,
             n_batch=config.llamacppMainModel_n_batch,
             verbose=config.llamacppMainModel_verbose,
@@ -478,15 +479,15 @@
         except:
             response = {}
         lm.reset()
         del lm
         return response
 
     @staticmethod
-    def extractToolParameters(schema: dict, userInput: str, ongoingMessages: list = [], temperature: Optional[float]=None, max_tokens: Optional[int]=None, **kwargs) -> dict:
+    def extractToolParameters(schema: dict, userInput: str, ongoingMessages: list = [], temperature: Optional[float]=None, max_tokens: Optional[int]=None) -> dict:
         """
         Extract action parameters
         """
         schema = toParameterSchema(schema)
         schemaCopy = copy.deepcopy(schema)
 
         # Generate Code when required
@@ -503,15 +504,15 @@
 Here is my request:
 <request>
 {userInput}
 </request>
 
 Remember, response with the required python code ONLY, WITHOUT extra notes or explanations."""
 
-            code = CallLlamaCpp.getSingleChatResponse(code_instruction, ongoingMessages[:-1]).replace(r"\\n", "\n")
+            code = CallLlamaCpp.getSingleChatResponse(code_instruction, ongoingMessages[:-1], temperature, max_tokens).replace(r"\\n", "\n")
             code = extractPythonCode(code, keepInvalid=True)
             if len(schema["properties"]) == 1:
                 return {"code": code}
         else:
             code = ""
 
         codeContext = f"""
@@ -535,15 +536,15 @@
 Generate content to fill up the value of each required key in the JSON, if information is not provided.
 
 Remember, output in JSON.""",
             },
         ]
 
         # schema alternative: properties if len(properties) == 1 else schema
-        parameters = CallLlamaCpp.getResponseDict(messages, schemaCopy, temperature=temperature, max_tokens=max_tokens, **kwargs)
+        parameters = CallLlamaCpp.getDictionaryOutput(messages, schemaCopy, temperature=temperature, max_tokens=max_tokens)
         if code:
             parameters["code"] = code
 
         if config.developer:
             print2("```parameters")
             pprint.pprint(parameters)
             print2("```")
```

### Comparing `freegenius-0.1.8/freegenius/utils/call_llm.py` & `freegenius-0.1.9/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/call_ollama.py` & `freegenius-0.1.9/freegenius/utils/call_ollama.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                 num_predict=num_predict if num_predict is not None else config.ollamaMainModel_num_predict,
                 **config.ollamaMainModel_additional_options,
             ),
         )
 
     @staticmethod
     @check_ollama_errors
-    def getResponseDict(messages: list, temperature: Optional[float]=None, num_ctx: Optional[int]=None, num_batch: Optional[int]=None, num_predict: Optional[int]=None):
+    def getDictionaryOutput(messages: list, temperature: Optional[float]=None, num_ctx: Optional[int]=None, num_batch: Optional[int]=None, num_predict: Optional[int]=None):
         #pprint.pprint(messages)
         try:
             completion = ollama.chat(
                 keep_alive=config.ollamaMainModel_keep_alive,
                 model=config.ollamaMainModel,
                 messages=messages,
                 format="json",
@@ -193,18 +193,18 @@
         except:
             showErrors()
             return messagesCopy
         return messages
 
     @staticmethod
     @check_ollama_errors
-    def getSingleFunctionCallResponse(messages: list, function_name: str, temperature: Optional[float]=None, num_ctx: Optional[int]=None, num_batch: Optional[int]=None, num_predict: Optional[int]=None, **kwargs):
+    def getSingleFunctionCallResponse(messages: list, function_name: str, temperature: Optional[float]=None, num_ctx: Optional[int]=None, num_batch: Optional[int]=None, num_predict: Optional[int]=None):
         tool_schema = config.toolFunctionSchemas[function_name]["parameters"]
         user_request = messages[-1]["content"]
-        func_arguments = CallOllama.extractToolParameters(schema=tool_schema, userInput=user_request, ongoingMessages=messages, temperature=temperature, num_ctx=num_ctx, num_batch=num_batch, num_predict=num_predict, **kwargs)
+        func_arguments = CallOllama.extractToolParameters(schema=tool_schema, userInput=user_request, ongoingMessages=messages, temperature=temperature, num_ctx=num_ctx, num_batch=num_batch, num_predict=num_predict)
         function_call_response = executeToolFunction(func_arguments=func_arguments, function_name=function_name)
         function_call_message_mini = {
             "role": "assistant",
             "content": "",
             "function_call": {
                 "name": function_name,
                 "arguments": func_arguments,
@@ -340,19 +340,19 @@
 {user_request}{deviceInfo}
 </request>
 
 Remember, response in JSON with the filled template ONLY.""",
             },
         ]
 
-        output = CallOllama.getResponseDict(messages_for_screening, temperature=0.0, num_predict=20)
+        output = CallOllama.getDictionaryOutput(messages_for_screening, temperature=0.0, num_predict=20)
         return True if "yes" in str(output).lower() else False
 
     @staticmethod
-    def extractToolParameters(schema: dict, userInput: str, ongoingMessages: list = [], temperature: Optional[float]=None, num_ctx: Optional[int]=None, num_batch: Optional[int]=None, num_predict: Optional[int]=None, **kwargs) -> dict:
+    def extractToolParameters(schema: dict, userInput: str, ongoingMessages: list = [], temperature: Optional[float]=None, num_ctx: Optional[int]=None, num_batch: Optional[int]=None, num_predict: Optional[int]=None) -> dict:
         """
         Extract action parameters
         """
         schema = toParameterSchema(schema)
         schemaCopy = copy.deepcopy(schema)
 
         # Generate Code when required
@@ -409,15 +409,15 @@
 
 Generate content to fill up the value of each required key in the JSON, if information is not provided.
 
 Remember, response in JSON with the filled template ONLY.""",
             },
         ]
 
-        parameters = CallOllama.getResponseDict(messages, temperature=temperature, num_ctx=num_ctx, num_batch=num_batch, num_predict=num_predict, **kwargs)
+        parameters = CallOllama.getDictionaryOutput(messages, temperature=temperature, num_ctx=num_ctx, num_batch=num_batch, num_predict=num_predict)
         if code:
             parameters["code"] = code
 
         if config.developer:
             print2("```parameters")
             pprint.pprint(parameters)
             print2("```")
```

### Comparing `freegenius-0.1.8/freegenius/utils/config_essential.py` & `freegenius-0.1.9/freegenius/utils/config_essential.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,17 @@
     ('rag_useAutoRetriever', False),
     ('rag_closestMatches', 5),
     ('rag_retrieverSettings', {'search_kwargs': {'k': 5}}),
     ('chatRecordClosestMatches', 5),
     ('runPythonScriptGlobally', False),
     ('groqApi_key', ''),
     ('groqApi_main_model', 'mixtral-8x7b-32768'),
+    ('groqApi_main_model_additional_chat_options', {}),
     ('groqApi_chat_model', 'llama3-70b-8192'),
+    ('groqApi_chat_model_additional_chat_options', {}),
     ('groqApi_max_tokens', 10000),
     ('openaiApiKey', ''),
     ('openaiApiOrganization', ''),
     ('loadingInternetSearches', "auto"),
     ('maximumInternetSearchResults', 5),
     ('predefinedContext', '[none]'),
     ('customPredefinedContext', ''),
```

### Comparing `freegenius-0.1.8/freegenius/utils/config_tools.py` & `freegenius-0.1.9/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/download.py` & `freegenius-0.1.9/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/get_path_prompt.py` & `freegenius-0.1.9/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/ollama_models.py` & `freegenius-0.1.9/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/promptValidator.py` & `freegenius-0.1.9/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.1.9/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.1.9/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/prompts.py` & `freegenius-0.1.9/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/python_utils.py` & `freegenius-0.1.9/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/shared_utils.py` & `freegenius-0.1.9/freegenius/utils/shared_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/shortcuts.py` & `freegenius-0.1.9/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/single_prompt.py` & `freegenius-0.1.9/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.1.9/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/sttLanguages.py` & `freegenius-0.1.9/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.1.9/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.1.9/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/text_utils.py` & `freegenius-0.1.9/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/tool_plugins.py` & `freegenius-0.1.9/freegenius/utils/tool_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 if not callEntry in config.inputSuggestions:
                     config.inputSuggestions.append(callEntry)
 
     # integrate function call plugin
     @staticmethod
     def addFunctionCall(signature: str, method: Callable[[dict], str], deviceInfo=False):
         name = signature["name"]
-        if not name in config.toolFunctionSchemas: # prvent duplicaiton
+        if not name in config.toolFunctionSchemas: # prevent duplicaiton
             config.toolFunctionSchemas[name] = {key: value for key, value in signature.items() if not key in ("intent", "examples")}
             config.toolFunctionMethods[name] = method
             ToolStore.add_tool(signature)
             if deviceInfo:
                 config.deviceInfoPlugins.append(name)
 
 class ToolStore:
```

### Comparing `freegenius-0.1.8/freegenius/utils/ttsLanguages.py` & `freegenius-0.1.9/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/tts_utils.py` & `freegenius-0.1.9/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius/utils/vlc_utils.py` & `freegenius-0.1.9/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius.egg-info/PKG-INFO` & `freegenius-0.1.9/freegenius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.1.8
+Version: 0.1.9
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.1.8/freegenius.egg-info/SOURCES.txt` & `freegenius-0.1.9/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius.egg-info/entry_points.txt` & `freegenius-0.1.9/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/freegenius.egg-info/requires.txt` & `freegenius-0.1.9/freegenius.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.8/setup.py` & `freegenius-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.1.8",
+    version="0.1.9",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```

