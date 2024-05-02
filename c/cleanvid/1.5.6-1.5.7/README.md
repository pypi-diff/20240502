# Comparing `tmp/cleanvid-1.5.6.tar.gz` & `tmp/cleanvid-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanvid-1.5.6.tar", last modified: Tue Dec 19 04:37:12 2023, max compression
+gzip compressed data, was "cleanvid-1.5.7.tar", last modified: Thu May  2 03:36:35 2024, max compression
```

## Comparing `cleanvid-1.5.6.tar` & `cleanvid-1.5.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:37:12.024245 cleanvid-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-12-19 04:37:04.000000 cleanvid-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2023-12-19 04:37:12.024245 cleanvid-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2023-12-19 04:37:04.000000 cleanvid-1.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-19 04:37:04.000000 cleanvid-1.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-19 04:37:12.024245 cleanvid-1.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:37:12.020245 cleanvid-1.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:37:12.024245 cleanvid-1.5.6/src/cleanvid/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-19 04:37:04.000000 cleanvid-1.5.6/src/cleanvid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2023-12-19 04:37:04.000000 cleanvid-1.5.6/src/cleanvid/caselessdictionary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26643 2023-12-19 04:37:04.000000 cleanvid-1.5.6/src/cleanvid/cleanvid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2023-12-19 04:37:04.000000 cleanvid-1.5.6/src/cleanvid/swears.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:37:12.024245 cleanvid-1.5.6/src/cleanvid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2023-12-19 04:37:12.000000 cleanvid-1.5.6/src/cleanvid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-12-19 04:37:12.000000 cleanvid-1.5.6/src/cleanvid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 04:37:12.000000 cleanvid-1.5.6/src/cleanvid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-19 04:37:12.000000 cleanvid-1.5.6/src/cleanvid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 04:37:11.000000 cleanvid-1.5.6/src/cleanvid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 04:37:12.000000 cleanvid-1.5.6/src/cleanvid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-19 04:37:12.000000 cleanvid-1.5.6/src/cleanvid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:36:35.944471 cleanvid-1.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-02 03:36:32.000000 cleanvid-1.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-02 03:36:35.944471 cleanvid-1.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-05-02 03:36:32.000000 cleanvid-1.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 03:36:32.000000 cleanvid-1.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-02 03:36:35.944471 cleanvid-1.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:36:35.940471 cleanvid-1.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:36:35.944471 cleanvid-1.5.7/src/cleanvid/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-02 03:36:32.000000 cleanvid-1.5.7/src/cleanvid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-02 03:36:32.000000 cleanvid-1.5.7/src/cleanvid/caselessdictionary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28246 2024-05-02 03:36:32.000000 cleanvid-1.5.7/src/cleanvid/cleanvid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-05-02 03:36:32.000000 cleanvid-1.5.7/src/cleanvid/swears.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:36:35.944471 cleanvid-1.5.7/src/cleanvid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-02 03:36:35.000000 cleanvid-1.5.7/src/cleanvid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-02 03:36:35.000000 cleanvid-1.5.7/src/cleanvid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:36:35.000000 cleanvid-1.5.7/src/cleanvid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 03:36:35.000000 cleanvid-1.5.7/src/cleanvid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:36:35.000000 cleanvid-1.5.7/src/cleanvid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 03:36:35.000000 cleanvid-1.5.7/src/cleanvid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 03:36:35.000000 cleanvid-1.5.7/src/cleanvid.egg-info/top_level.txt
```

### Comparing `cleanvid-1.5.6/LICENSE` & `cleanvid-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanvid-1.5.6/PKG-INFO` & `cleanvid-1.5.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvid
-Version: 1.5.6
+Version: 1.5.7
 Summary: cleanvid is a little script to mute profanity in video files.
 Home-page: https://github.com/mmguero/cleanvid
 Author: Seth Grover
 Author-email: mero.mero.guero@gmail.com
 Project-URL: Bug Tracker, https://github.com/mmguero/cleanvid/issues
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -31,18 +31,17 @@
 
 You can then use your favorite media player to play the cleaned video file together with the cleaned subtitles.
 
 As an alternative to creating a new video file, cleanvid can create a simple EDL file (see the [mplayer](http://www.mplayerhq.hu/DOCS/HTML/en/edl.html) or KODI [documentation](https://kodi.wiki/view/Edit_decision_list)) or a custom JSON definition file for [PlexAutoSkip](https://github.com/mdhiggins/PlexAutoSkip).
 
 **cleanvid** is part of a family of projects with similar goals:
 
-* 📼 [cleanvid](https://github.com/mmguero/cleanvid) for video files
-* 🎤 [monkeyplug](https://github.com/mmguero/monkeyplug) for audio files
+* 📼 [cleanvid](https://github.com/mmguero/cleanvid) for video files (using [SRT-formatted](https://en.wikipedia.org/wiki/SubRip#Format) subtitles)
+* 🎤 [monkeyplug](https://github.com/mmguero/monkeyplug) for audio and video files (using either [Whisper](https://openai.com/research/whisper) or the [Vosk](https://alphacephei.com/vosk/)-[API](https://github.com/alphacep/vosk-api) for speech recognition)
 * 📕 [montag](https://github.com/mmguero/montag) for ebooks
-
 ## Installation
 
 Using `pip`, to install the latest [release from PyPI](https://pypi.org/project/cleanvid/):
 
 ```
 python3 -m pip install -U cleanvid
 ```
```

### Comparing `cleanvid-1.5.6/README.md` & `cleanvid-1.5.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
 You can then use your favorite media player to play the cleaned video file together with the cleaned subtitles.
 
 As an alternative to creating a new video file, cleanvid can create a simple EDL file (see the [mplayer](http://www.mplayerhq.hu/DOCS/HTML/en/edl.html) or KODI [documentation](https://kodi.wiki/view/Edit_decision_list)) or a custom JSON definition file for [PlexAutoSkip](https://github.com/mdhiggins/PlexAutoSkip).
 
 **cleanvid** is part of a family of projects with similar goals:
 
-* 📼 [cleanvid](https://github.com/mmguero/cleanvid) for video files
-* 🎤 [monkeyplug](https://github.com/mmguero/monkeyplug) for audio files
+* 📼 [cleanvid](https://github.com/mmguero/cleanvid) for video files (using [SRT-formatted](https://en.wikipedia.org/wiki/SubRip#Format) subtitles)
+* 🎤 [monkeyplug](https://github.com/mmguero/monkeyplug) for audio and video files (using either [Whisper](https://openai.com/research/whisper) or the [Vosk](https://alphacephei.com/vosk/)-[API](https://github.com/alphacep/vosk-api) for speech recognition)
 * 📕 [montag](https://github.com/mmguero/montag) for ebooks
-
 ## Installation
 
 Using `pip`, to install the latest [release from PyPI](https://pypi.org/project/cleanvid/):
 
 ```
 python3 -m pip install -U cleanvid
 ```
```

### Comparing `cleanvid-1.5.6/setup.cfg` & `cleanvid-1.5.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cleanvid
-version = 1.5.6
+version = 1.5.7
 author = Seth Grover
 author_email = mero.mero.guero@gmail.com
 description = cleanvid is a little script to mute profanity in video files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mmguero/cleanvid
 project_urls =
```

### Comparing `cleanvid-1.5.6/src/cleanvid/caselessdictionary.py` & `cleanvid-1.5.7/src/cleanvid/caselessdictionary.py`

 * *Files identical despite different names*

### Comparing `cleanvid-1.5.6/src/cleanvid/cleanvid.py` & `cleanvid-1.5.7/src/cleanvid/cleanvid.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,17 +107,19 @@
 
 
 ######## ExtractSubtitles #####################################################
 def ExtractSubtitles(vidFileSpec, srtLanguage):
     subFileSpec = ""
     srtLanguage, srtForceIndex = SplitLanguageIfForced(srtLanguage)
     if (streamInfo := GetStreamSubtitleMap(vidFileSpec)) and (
-        stream := next(iter([k for k, v in streamInfo.items() if (v == srtLanguage)]), None)
-        if not srtForceIndex
-        else srtForceIndex
+        stream := (
+            next(iter([k for k, v in streamInfo.items() if (v == srtLanguage)]), None)
+            if not srtForceIndex
+            else srtForceIndex
+        )
     ):
         subFileParts = os.path.splitext(vidFileSpec)
         subFileSpec = subFileParts[0] + "." + srtLanguage + ".srt"
         ffmpegCmd = (
             "ffmpeg -hide_banner -nostats -loglevel error -y -i \""
             + vidFileSpec
             + f"\" -map 0:{stream} \""
@@ -191,20 +193,23 @@
     swearsFileSpec = ""
     swearsPadMillisec = 0
     embedSubs = False
     fullSubs = False
     subsOnly = False
     edl = False
     hardCode = False
-    reEncode = False
+    reEncodeVideo = False
+    reEncodeAudio = False
     unalteredVideo = False
     subsLang = SUBTITLE_DEFAULT_LANG
     vParams = VIDEO_DEFAULT_PARAMS
     aParams = AUDIO_DEFAULT_PARAMS
     aDownmix = False
+    threadsInput = None
+    threadsEncoding = None
     plexAutoSkipJson = ""
     plexAutoSkipId = ""
     swearsMap = CaselessDictionary({})
     muteTimeList = []
     jsonDumpList = None
 
     ######## init #################################################################
@@ -219,19 +224,22 @@
         swearsPadSec=0.0,
         embedSubs=False,
         fullSubs=False,
         subsOnly=False,
         edl=False,
         jsonDump=False,
         subsLang=SUBTITLE_DEFAULT_LANG,
-        reEncode=False,
+        reEncodeVideo=False,
+        reEncodeAudio=False,
         hardCode=False,
         vParams=VIDEO_DEFAULT_PARAMS,
         aParams=AUDIO_DEFAULT_PARAMS,
         aDownmix=False,
+        threadsInput=None,
+        threadsEncoding=None,
         plexAutoSkipJson="",
         plexAutoSkipId="",
     ):
         if (iVidFileSpec is not None) and os.path.isfile(iVidFileSpec):
             self.inputVidFileSpec = iVidFileSpec
         else:
             raise IOError(errno.ENOENT, os.strerror(errno.ENOENT), iVidFileSpec)
@@ -258,20 +266,23 @@
         self.embedSubs = embedSubs
         self.fullSubs = fullSubs
         self.subsOnly = subsOnly or edl or (plexAutoSkipJson and plexAutoSkipId)
         self.edl = edl
         self.jsonDumpList = [] if jsonDump else None
         self.plexAutoSkipJson = plexAutoSkipJson
         self.plexAutoSkipId = plexAutoSkipId
-        self.reEncode = reEncode
+        self.reEncodeVideo = reEncodeVideo
+        self.reEncodeAudio = reEncodeAudio
         self.hardCode = hardCode
         self.subsLang = subsLang
         self.vParams = vParams
         self.aParams = aParams
         self.aDownmix = aDownmix
+        self.threadsInput = threadsInput
+        self.threadsEncoding = threadsEncoding
         if self.vParams.startswith('base64:'):
             self.vParams = base64.b64decode(self.vParams[7:]).decode('utf-8')
         if self.aParams.startswith('base64:'):
             self.aParams = base64.b64decode(self.aParams[7:]).decode('utf-8')
 
     ######## del ##################################################################
     def __del__(self):
@@ -492,16 +503,22 @@
     def MultiplexCleanVideo(self):
         # if we're don't *have* to generate a new video file, don't
         # we need to generate a video file if any of the following are true:
         # - we were explicitly asked to re-encode
         # - we are hard-coding (burning) subs
         # - we are embedding a subtitle stream
         # - we are not doing "subs only" or EDL mode and there more than zero mute sections
-        if self.reEncode or self.hardCode or self.embedSubs or ((not self.subsOnly) and (len(self.muteTimeList) > 0)):
-            if self.reEncode or self.hardCode:
+        if (
+            self.reEncodeVideo
+            or self.reEncodeAudio
+            or self.hardCode
+            or self.embedSubs
+            or ((not self.subsOnly) and (len(self.muteTimeList) > 0))
+        ):
+            if self.reEncodeVideo or self.hardCode:
                 if self.hardCode and os.path.isfile(self.cleanSubsFileSpec):
                     self.assSubsFileSpec = self.cleanSubsFileSpec + '.ass'
                     subConvCmd = f"ffmpeg -hide_banner -nostats -loglevel error -y -i {self.cleanSubsFileSpec} {self.assSubsFileSpec}"
                     subConvResult = delegator.run(subConvCmd, block=True)
                     if (subConvResult.return_code == 0) and os.path.isfile(self.assSubsFileSpec):
                         videoArgs = f"{self.vParams} -vf \"ass={self.assSubsFileSpec}\""
                     else:
@@ -520,21 +537,21 @@
                 audioFilter = " "
             if self.embedSubs and os.path.isfile(self.cleanSubsFileSpec):
                 outFileParts = os.path.splitext(self.outputVidFileSpec)
                 subsArgs = f" -i \"{self.cleanSubsFileSpec}\" -map 0 -map -0:s -map 1 -c:s {'mov_text' if outFileParts[1] == '.mp4' else 'srt'} -disposition:s:0 default -metadata:s:s:0 language={self.subsLang} "
             else:
                 subsArgs = " -sn "
             ffmpegCmd = (
-                "ffmpeg -hide_banner -nostats -loglevel error -y -i \""
+                f"ffmpeg -hide_banner -nostats -loglevel error -y {'' if self.threadsInput is None else ('-threads '+ str(int(self.threadsInput)))} -i \""
                 + self.inputVidFileSpec
                 + "\""
                 + subsArgs
                 + videoArgs
                 + audioFilter
-                + f"{self.aParams} \""
+                + f"{self.aParams} {'' if self.threadsEncoding is None else ('-threads '+ str(int(self.threadsEncoding)))} \""
                 + self.outputVidFileSpec
                 + "\""
             )
             ffmpegResult = delegator.run(ffmpegCmd, block=True)
             if (ffmpegResult.return_code != 0) or (not os.path.isfile(self.outputVidFileSpec)):
                 print(ffmpegCmd)
                 print(ffmpegResult.err)
@@ -618,15 +635,16 @@
     )
     parser.add_argument(
         '--json',
         help='generate JSON file with muted subtitles and their contents',
         dest='json',
         action='store_true',
     )
-    parser.add_argument('-r', '--re-encode', help='Re-encode video', dest='reEncode', action='store_true')
+    parser.add_argument('--re-encode-video', help='Re-encode video', dest='reEncodeVideo', action='store_true')
+    parser.add_argument('--re-encode-audio', help='Re-encode audio', dest='reEncodeAudio', action='store_true')
     parser.add_argument(
         '-b', '--burn', help='Hard-coded subtitles (implies re-encode)', dest='hardCode', action='store_true'
     )
     parser.add_argument(
         '-v',
         '--video-params',
         help='Video parameters for ffmpeg (only if re-encoding)',
@@ -635,20 +653,45 @@
     )
     parser.add_argument(
         '-a', '--audio-params', help='Audio parameters for ffmpeg', dest='aParams', default=AUDIO_DEFAULT_PARAMS
     )
     parser.add_argument(
         '-d', '--downmix', help='Downmix to stereo (if not already stereo)', dest='aDownmix', action='store_true'
     )
+    parser.add_argument(
+        '--threads-input',
+        help='ffmpeg global options -threads value',
+        metavar='<int>',
+        dest="threadsInput",
+        type=int,
+        default=None,
+    )
+    parser.add_argument(
+        '--threads-encoding',
+        help='ffmpeg encoding options -threads value',
+        metavar='<int>',
+        dest="threadsEncoding",
+        type=int,
+        default=None,
+    )
+    parser.add_argument(
+        '--threads',
+        help='ffmpeg -threads value (for both global options and encoding)',
+        metavar='<int>',
+        dest="threads",
+        type=int,
+        default=None,
+    )
     parser.set_defaults(
         embedSubs=False,
         fullSubs=False,
         subsOnly=False,
         offline=False,
-        reEncode=False,
+        reEncodeVideo=False,
+        reEncodeAudio=False,
         hardCode=False,
         edl=False,
     )
     args = parser.parse_args()
 
     inFile = args.input
     outFile = args.output
@@ -678,19 +721,22 @@
         args.pad,
         args.embedSubs,
         args.fullSubs,
         args.subsOnly,
         args.edl,
         args.json,
         lang,
-        args.reEncode,
+        args.reEncodeVideo,
+        args.reEncodeAudio,
         args.hardCode,
         args.vParams,
         args.aParams,
         args.aDownmix,
+        args.threadsInput if args.threadsInput is not None else args.threads,
+        args.threadsEncoding if args.threadsEncoding is not None else args.threads,
         plexFile,
         args.plexAutoSkipId,
     )
     cleaner.CreateCleanSubAndMuteList()
     cleaner.MultiplexCleanVideo()
```

### Comparing `cleanvid-1.5.6/src/cleanvid/swears.txt` & `cleanvid-1.5.7/src/cleanvid/swears.txt`

 * *Files 1% similar despite different names*

```diff
@@ -475,15 +475,15 @@
 goddamnit|dangit
 goddamnmuthafucker
 goddamn|gosh darn
 godshit
 godshits
 handjob
 handjobs
-hard on
+hardon
 headfuck
 headfucks
 hell|heck
 henshit
 henshits
 homo
 homodumbshit
@@ -502,14 +502,16 @@
 jackoffs
 jerk off
 jesus|moses
 jigaboo
 jizz
 joyshit
 joyshits
+kickass
+kick-ass
 kitchenshit
 kitchenshits
 kooch
 kootch
 kunt
 labia
 lezzie
```

### Comparing `cleanvid-1.5.6/src/cleanvid.egg-info/PKG-INFO` & `cleanvid-1.5.7/src/cleanvid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvid
-Version: 1.5.6
+Version: 1.5.7
 Summary: cleanvid is a little script to mute profanity in video files.
 Home-page: https://github.com/mmguero/cleanvid
 Author: Seth Grover
 Author-email: mero.mero.guero@gmail.com
 Project-URL: Bug Tracker, https://github.com/mmguero/cleanvid/issues
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -31,18 +31,17 @@
 
 You can then use your favorite media player to play the cleaned video file together with the cleaned subtitles.
 
 As an alternative to creating a new video file, cleanvid can create a simple EDL file (see the [mplayer](http://www.mplayerhq.hu/DOCS/HTML/en/edl.html) or KODI [documentation](https://kodi.wiki/view/Edit_decision_list)) or a custom JSON definition file for [PlexAutoSkip](https://github.com/mdhiggins/PlexAutoSkip).
 
 **cleanvid** is part of a family of projects with similar goals:
 
-* 📼 [cleanvid](https://github.com/mmguero/cleanvid) for video files
-* 🎤 [monkeyplug](https://github.com/mmguero/monkeyplug) for audio files
+* 📼 [cleanvid](https://github.com/mmguero/cleanvid) for video files (using [SRT-formatted](https://en.wikipedia.org/wiki/SubRip#Format) subtitles)
+* 🎤 [monkeyplug](https://github.com/mmguero/monkeyplug) for audio and video files (using either [Whisper](https://openai.com/research/whisper) or the [Vosk](https://alphacephei.com/vosk/)-[API](https://github.com/alphacep/vosk-api) for speech recognition)
 * 📕 [montag](https://github.com/mmguero/montag) for ebooks
-
 ## Installation
 
 Using `pip`, to install the latest [release from PyPI](https://pypi.org/project/cleanvid/):
 
 ```
 python3 -m pip install -U cleanvid
 ```
```

