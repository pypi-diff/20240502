# Comparing `tmp/tictacsync-0.4a0.tar.gz` & `tmp/tictacsync-0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictacsync-0.4a0.tar", last modified: Thu Apr 18 16:08:29 2024, max compression
+gzip compressed data, was "tictacsync-0.5a0.tar", last modified: Thu May  2 16:36:23 2024, max compression
```

## Comparing `tictacsync-0.4a0.tar` & `tictacsync-0.5a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-18 16:08:29.820608 tictacsync-0.4a0/
--rwxr-xr-x   0 lutzray    (501) staff       (20)     1068 2021-11-05 23:38:28.000000 tictacsync-0.4a0/LICENSE
--rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-18 16:08:29.820223 tictacsync-0.4a0/PKG-INFO
--rw-rw-r--   0 lutzray    (501) staff       (20)     4170 2024-03-26 23:09:32.000000 tictacsync-0.4a0/README.md
--rw-r--r--   0 lutzray    (501) staff       (20)       38 2024-04-18 16:08:29.820741 tictacsync-0.4a0/setup.cfg
--rw-r--r--   0 lutzray    (501) staff       (20)     1789 2024-04-18 16:07:57.000000 tictacsync-0.4a0/setup.py
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-18 16:08:29.815693 tictacsync-0.4a0/tictacsync/
--rw-rw-r--   0 lutzray    (501) staff       (20)        0 2022-01-08 15:24:31.000000 tictacsync-0.4a0/tictacsync/__init__.py
--rw-r--r--   0 lutzray    (501) staff       (20)    27339 2024-04-12 00:39:24.000000 tictacsync-0.4a0/tictacsync/device_scanner.py
--rw-r--r--   0 lutzray    (501) staff       (20)    11386 2024-04-18 15:36:05.000000 tictacsync-0.4a0/tictacsync/entry.py
--rw-r--r--   0 lutzray    (501) staff       (20)     7279 2024-03-24 12:15:34.000000 tictacsync-0.4a0/tictacsync/multi2polywav.py
--rw-r--r--   0 lutzray    (501) staff       (20)     4885 2024-03-27 22:40:38.000000 tictacsync-0.4a0/tictacsync/remergemix.py
--rw-r--r--   0 lutzray    (501) staff       (20)    56225 2024-04-18 15:35:51.000000 tictacsync-0.4a0/tictacsync/timeline.py
--rw-r--r--   0 lutzray    (501) staff       (20)    78490 2024-04-12 00:34:48.000000 tictacsync-0.4a0/tictacsync/yaltc.py
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-18 16:08:29.819738 tictacsync-0.4a0/tictacsync.egg-info/
--rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/PKG-INFO
--rw-r--r--   0 lutzray    (501) staff       (20)      433 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/SOURCES.txt
--rw-r--r--   0 lutzray    (501) staff       (20)        1 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/dependency_links.txt
--rw-r--r--   0 lutzray    (501) staff       (20)      139 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/entry_points.txt
--rw-r--r--   0 lutzray    (501) staff       (20)        1 2022-01-31 00:58:06.000000 tictacsync-0.4a0/tictacsync.egg-info/not-zip-safe
--rw-r--r--   0 lutzray    (501) staff       (20)      132 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/requires.txt
--rw-r--r--   0 lutzray    (501) staff       (20)       11 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/top_level.txt
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-05-02 16:36:23.983511 tictacsync-0.5a0/
+-rwxr-xr-x   0 lutzray    (501) staff       (20)     1068 2021-11-05 23:38:28.000000 tictacsync-0.5a0/LICENSE
+-rw-r--r--   0 lutzray    (501) staff       (20)     5234 2024-05-02 16:36:23.983075 tictacsync-0.5a0/PKG-INFO
+-rw-rw-r--   0 lutzray    (501) staff       (20)     4381 2024-04-26 11:27:56.000000 tictacsync-0.5a0/README.md
+-rw-r--r--   0 lutzray    (501) staff       (20)       38 2024-05-02 16:36:23.983679 tictacsync-0.5a0/setup.cfg
+-rw-r--r--   0 lutzray    (501) staff       (20)     1789 2024-05-02 16:35:53.000000 tictacsync-0.5a0/setup.py
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-05-02 16:36:23.977207 tictacsync-0.5a0/tictacsync/
+-rw-rw-r--   0 lutzray    (501) staff       (20)        0 2022-01-08 15:24:31.000000 tictacsync-0.5a0/tictacsync/__init__.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    27515 2024-04-18 21:56:19.000000 tictacsync-0.5a0/tictacsync/device_scanner.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    11391 2024-04-20 02:26:49.000000 tictacsync-0.5a0/tictacsync/entry.py
+-rw-r--r--   0 lutzray    (501) staff       (20)     7282 2024-04-18 19:12:22.000000 tictacsync-0.5a0/tictacsync/multi2polywav.py
+-rw-r--r--   0 lutzray    (501) staff       (20)     9829 2024-04-22 14:23:25.000000 tictacsync-0.5a0/tictacsync/remergemix.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    57449 2024-04-21 03:26:26.000000 tictacsync-0.5a0/tictacsync/timeline.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    78490 2024-04-12 00:34:48.000000 tictacsync-0.5a0/tictacsync/yaltc.py
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-05-02 16:36:23.982414 tictacsync-0.5a0/tictacsync.egg-info/
+-rw-r--r--   0 lutzray    (501) staff       (20)     5234 2024-05-02 16:36:23.000000 tictacsync-0.5a0/tictacsync.egg-info/PKG-INFO
+-rw-r--r--   0 lutzray    (501) staff       (20)      433 2024-05-02 16:36:23.000000 tictacsync-0.5a0/tictacsync.egg-info/SOURCES.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)        1 2024-05-02 16:36:23.000000 tictacsync-0.5a0/tictacsync.egg-info/dependency_links.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)      139 2024-05-02 16:36:23.000000 tictacsync-0.5a0/tictacsync.egg-info/entry_points.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)        1 2022-01-31 00:58:06.000000 tictacsync-0.5a0/tictacsync.egg-info/not-zip-safe
+-rw-r--r--   0 lutzray    (501) staff       (20)      132 2024-05-02 16:36:23.000000 tictacsync-0.5a0/tictacsync.egg-info/requires.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)       11 2024-05-02 16:36:23.000000 tictacsync-0.5a0/tictacsync.egg-info/top_level.txt
```

### Comparing `tictacsync-0.4a0/LICENSE` & `tictacsync-0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tictacsync-0.4a0/PKG-INFO` & `tictacsync-0.5a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictacsync
-Version: 0.4a0
+Version: 0.5a0
 Summary: command for syncing audio video recordings
 Home-page: https://tictacsync.org/
 Author: Raymond Lutz
 Author-email: lutzrayblog@mac.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -25,23 +25,29 @@
 
 ## Warning: this is at pre-alpha stage
 
 Unfinished sloppy code ahead, but should run without errors. Some functionalities are still missing. Don't run the code without parental supervision. Suggestions and enquiries are welcome via the [lists hosted on sourcehut](https://sr.ht/~proflutz/TicTacSync/lists).
 
 ## Description
 
-`tictacsync` is a python script to sync audio and video files shot
-with [dual system sound](https://www.learnlightandsound.com/blog/2017/2/23/how-to-record-sound-for-video-dual-systemsync-sound)  using a specific hardware timecode generator
-called [Tic Tac Sync](https://tictacsync.org). The timecode is named YaLTC for *yet
-another longitudinal time code* and should be recorded on a scratch
-track on each device for the syncing to be performed, later in _postprod_ before editing.
-
+`tictacsync` is a python script to sync, cut and join audio files against camera files shot using a specific hardware timecode generator
+called [Tic Tac Sync](https://tictacsync.org). The timecode is named TicTacCode and should be recorded on a scratch
+track on each device for `tictacsync` to work.
 ## Status
 
-`tictacsync`  scans for audio video files and displays their starting time and then merges overlapping audio and video recordings. Multicam syncing with one stereo audio recorder has been tested (spring 2023, [see demo](https://youtu.be/pklTSTi7cqs)). Multi audio recorders coming soon... 
+Feature complete! `tictacsync`  scans for audio video files and then merges overlapping audio and video recordings, It
+
+* Decodes the TicTacCode audio track alongside your audio tracks
+* Establishes UTC start time (and end time) within 100 μs!
+* Syncs, cuts and joins any concurrent audio to camera files (using `FFmpeg`)
+* Processes _multiple_ audio recorders
+* Corrects device clock drift so _both_ ends coincide (thanks to `sox`)
+* Sets video metadata TC of multicam files for NLE timeline alignement
+* Writes _synced_ ISO files with dedicated file names declared in `tracks.txt`
+* Produces nice plots.
 
 
 ## Installation
 
 This uses the [python interpreter](https://www.python.org/downloads/) and multiple packages (so you need python 3 + pip). Also, you need to install two non-python command line executables: [ffmpeg](https://windowsloop.com/install-ffmpeg-windows-10/) and [sox](https://sourceforge.net/projects/sox/files/). Make sure those are _accessible through your `PATH` system environment variable_.
 Then pip install the syncing program:
 
@@ -73,15 +79,15 @@
     > tictacsync -v dailies/loose/MVI_0024.MP4
 
 For a one line output (or to suppress the progress bars) use the `--terse` flag:
 
 	> tictacsync --terse dailies/loose/MVI_0024.MP4 
 	dailies/loose/MVI_0024.MP4 UTC:2024-03-12 23:07:01.4281 pulse: 27450 in chan 0
 
-To also produce _synced_ ISO audio files, specify `--isos` . A directory named `ISOs` will contain _for each synced video_ a set of audio files of exact same length, padded or trimmed to coincide with the video track. After re-editing and re-mixing a `remergemix` command will resync the new sound track with the video [TODO].
+To also produce _synced_ ISO audio files, specify `--isos` . A directory named `ISOs` will contain _for each synced video_ a set of ISO audio files of exact same length, padded or trimmed to coincide with the video track. After re-editing and re-mixing a `remergemix` command will resync the new audio with the video and _the new sound track will be updated on your NLE timeline_, at least in Kdenlive...
 
 	> tictacsync --isos dailies/structured
 
 When called with the `-p` flag, zoomable plots will be produced for diagnostic purpose (close the plotting window for the 2nd one) and the decoded starting time will be output to stdin:
 
     > tictacsync -p dailies/loose/MVI_0024.MP4
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tictacsync-0.4a0/README.md` & `tictacsync-0.5a0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,29 @@
 
 ## Warning: this is at pre-alpha stage
 
 Unfinished sloppy code ahead, but should run without errors. Some functionalities are still missing. Don't run the code without parental supervision. Suggestions and enquiries are welcome via the [lists hosted on sourcehut](https://sr.ht/~proflutz/TicTacSync/lists).
 
 ## Description
 
-`tictacsync` is a python script to sync audio and video files shot
-with [dual system sound](https://www.learnlightandsound.com/blog/2017/2/23/how-to-record-sound-for-video-dual-systemsync-sound)  using a specific hardware timecode generator
-called [Tic Tac Sync](https://tictacsync.org). The timecode is named YaLTC for *yet
-another longitudinal time code* and should be recorded on a scratch
-track on each device for the syncing to be performed, later in _postprod_ before editing.
-
+`tictacsync` is a python script to sync, cut and join audio files against camera files shot using a specific hardware timecode generator
+called [Tic Tac Sync](https://tictacsync.org). The timecode is named TicTacCode and should be recorded on a scratch
+track on each device for `tictacsync` to work.
 ## Status
 
-`tictacsync`  scans for audio video files and displays their starting time and then merges overlapping audio and video recordings. Multicam syncing with one stereo audio recorder has been tested (spring 2023, [see demo](https://youtu.be/pklTSTi7cqs)). Multi audio recorders coming soon... 
+Feature complete! `tictacsync`  scans for audio video files and then merges overlapping audio and video recordings, It
+
+* Decodes the TicTacCode audio track alongside your audio tracks
+* Establishes UTC start time (and end time) within 100 μs!
+* Syncs, cuts and joins any concurrent audio to camera files (using `FFmpeg`)
+* Processes _multiple_ audio recorders
+* Corrects device clock drift so _both_ ends coincide (thanks to `sox`)
+* Sets video metadata TC of multicam files for NLE timeline alignement
+* Writes _synced_ ISO files with dedicated file names declared in `tracks.txt`
+* Produces nice plots.
 
 
 ## Installation
 
 This uses the [python interpreter](https://www.python.org/downloads/) and multiple packages (so you need python 3 + pip). Also, you need to install two non-python command line executables: [ffmpeg](https://windowsloop.com/install-ffmpeg-windows-10/) and [sox](https://sourceforge.net/projects/sox/files/). Make sure those are _accessible through your `PATH` system environment variable_.
 Then pip install the syncing program:
 
@@ -50,15 +56,15 @@
     > tictacsync -v dailies/loose/MVI_0024.MP4
 
 For a one line output (or to suppress the progress bars) use the `--terse` flag:
 
 	> tictacsync --terse dailies/loose/MVI_0024.MP4 
 	dailies/loose/MVI_0024.MP4 UTC:2024-03-12 23:07:01.4281 pulse: 27450 in chan 0
 
-To also produce _synced_ ISO audio files, specify `--isos` . A directory named `ISOs` will contain _for each synced video_ a set of audio files of exact same length, padded or trimmed to coincide with the video track. After re-editing and re-mixing a `remergemix` command will resync the new sound track with the video [TODO].
+To also produce _synced_ ISO audio files, specify `--isos` . A directory named `ISOs` will contain _for each synced video_ a set of ISO audio files of exact same length, padded or trimmed to coincide with the video track. After re-editing and re-mixing a `remergemix` command will resync the new audio with the video and _the new sound track will be updated on your NLE timeline_, at least in Kdenlive...
 
 	> tictacsync --isos dailies/structured
 
 When called with the `-p` flag, zoomable plots will be produced for diagnostic purpose (close the plotting window for the 2nd one) and the decoded starting time will be output to stdin:
 
     > tictacsync -p dailies/loose/MVI_0024.MP4
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tictacsync-0.4a0/setup.py` & `tictacsync-0.5a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     entry_points = {
         "console_scripts": [
         'tictacsync = tictacsync.entry:main',
         'remergemix = tictacsync.remergemix:main',
         'multi2polywav = tictacsync.multi2polywav:main',
         ]
         },
-    version = '0.4a',
+    version = '0.5a',
     description = "command for syncing audio video recordings",
     long_description_content_type='text/markdown',
     long_description = long_descr,
     include_package_data=True,
     zip_safe=False,
     author = "Raymond Lutz",
     author_email = "lutzrayblog@mac.com",
```

### Comparing `tictacsync-0.4a0/tictacsync/device_scanner.py` & `tictacsync-0.5a0/tictacsync/device_scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,18 +86,20 @@
 
 @dataclass
 class Media:
     """A custom data type that represents data for a media file.
     """
     path: Path
     device: Device
+
 def media_at_path(input_structure, p):
     # return Media object for mediafile using ffprobe
     dev_UID, dt = get_device_ffprobe_UID(p)
-    dev_name = None 
+    dev_name = None
+    logger.debug('ffprobe dev_UID:%s dt:%s'%(dev_UID, dt))
     if input_structure == 'folder_is_device':
         dev_name = p.parent.name
         if dev_UID is None:
             dev_UID = hash(dev_name)
     if dt == 'CAM':
         streams = ffmpeg.probe(p)['streams']
         audio_streams = [
@@ -110,17 +112,18 @@
             raise Exception('ffprobe gave multiple audio streams?')
         audio_str = audio_streams[0]
         n = audio_str['channels']
         # pprint(ffmpeg.probe(p))
     else:
         n = sox.file_info.channels(_pathname(p)) # eg 2
     logger.debug('for file %s dev_UID established %s'%(p.name, dev_UID))
-    return Media(p,
-        Device(UID=dev_UID, folder=p.parent, name=dev_name, dev_type=dt,
-                n_chan=n, ttc=None, tracks=None))
+    device = Device(UID=dev_UID, folder=p.parent, name=dev_name, dev_type=dt,
+                n_chan=n, ttc=None, tracks=None)
+    logger.debug('for path: %s, device:%s'%(p,device))
+    return Media(p, device)
 
 def get_device_ffprobe_UID(file):
     """
     Tries to find an unique hash integer identifying the device that produced
     the file based on the string inside ffprobe metadata  without any
     reference to date nor length nor time. Find out with ffprobe the type
     of device: CAM or REC for videocamera or audio recorder.
@@ -137,31 +140,34 @@
     file = Path(file)
     logger.debug('trying to find UID probe for %s'%file)
     try:
         probe = ffmpeg.probe(file)
     except ffmpeg.Error as e:
         print('ffmpeg.probe error')
         print(e.stderr, file)
-        return None, None
+        return None, None #-----------------------------------------------------
         # fall back to folder name
     streams = probe['streams']
     codecs = [stream['codec_type'] for stream in streams]
     device_type = 'CAM' if 'video' in codecs else 'REC'
     format_dict = probe['format'] # all files should have this
     if 'tags' in format_dict:
         probe_string = pformat(format_dict['tags'])
         probe_lines = [l for l in probe_string.split('\n') 
                 if '_time' not in l 
                 and 'time_' not in l 
                 and 'date' not in l ]
         # this removes any metadata related to the file
         # but keeps metadata related to the device
+        logger.debug('probe_lines %s'%probe_lines)
         UID = hash(''.join(probe_lines))
     else:
         UID = None
+    if UID == 0: # empty probe_lines from Audacity ?!?
+        UID = None
     logger.debug('ffprobe_UID is: %s'%UID)
     return UID, device_type
 
 class Scanner:
     """
     Class that encapsulates scanning of the directory given as CLI argument.
     Depending on the input_structure detected (loose|folder_is_device), enforce
@@ -253,44 +259,41 @@
         else:
             # check later if inside each folder, media have same device,
             # for now, we'll guess structure is 'folder_is_device'
             self.input_structure = 'folder_is_device'
         for p in paths:
             new_media = media_at_path(self.input_structure, p) # dev UID set here
             self.found_media_files.append(new_media)
-        # files from devices without UID or name
-        # def _list_all_the_same(l):
-        #     return all(e == l[0] for e in l)
         def _try_name(medias):
             # return common first strings in filename
             names = [m.path.name for m in medias]
             transposed_names = list(map(list, zip(*names)))
             same = list(map(_list_all_the_same, transposed_names))
             try:
                 first_diff = same.index(False)
             except:
                 return names[0].split('.')[0]
             return names[0][:first_diff]
         no_device_UID_media = [m for m in self.found_media_files
                     if not m.device.UID]
         if no_device_UID_media:
             logger.debug('no_device_UID_media %s'%no_device_UID_media)
-            # print(no_device_UID_media)
             start_string = _try_name(no_device_UID_media)
             if len(start_string) < 2:
                 print('\nError, cant identify the device for those files:')
                 [print('%s, '%m.path.name, end='') for m in no_device_UID_media]
                 print('\n')
                 sys.exit(1)
             one_device = no_device_UID_media[0].device
             one_device.name = start_string
             if not one_device.UID:
                 one_device.UID = hash(start_string)
             print('\nWarning, guessing a device ID for those files:')
-            [print('[gold1]%s[/gold1], '%m.path.name, end='') for m in no_device_UID_media]
+            [print('[gold1]%s[/gold1], '%m.path.name, end='') for m
+                                            in no_device_UID_media]
             print('UID: [gold1]%s[/gold1]'%start_string)
             for m in no_device_UID_media:
                 m.device = one_device
             logger.debug('new device added %s'%self.found_media_files)
         logger.debug('Scanner.found_media_files = %s'%self.found_media_files)
         if self.input_structure == 'folder_is_device':
             self._check_folders_have_same_device()
```

### Comparing `tictacsync-0.4a0/tictacsync/entry.py` & `tictacsync-0.5a0/tictacsync/entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,17 +122,17 @@
                     help='terse output')
     args = parser.parse_args()
     if args.verbose_output:
         logger.add(sys.stderr, level="DEBUG")
     # logger.add(sys.stdout, filter="__main__")
     # logger.add(sys.stdout, filter="device_scanner")
     # logger.add(sys.stdout, filter="yaltc") _extract_sound_to_merge
-    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_get_tracks_from_file")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "media_at_path")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "scan_media_and_build_devices_UID")
     # logger.add(sys.stdout, filter=lambda r: r["function"] == "_get_device_mix")
-    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_sox_mono2stereo")
     # logger.add(sys.stdout, filter=lambda r: r["function"] == "_sox_mix_files")
     top_dir = args.directory[0]
     if os.path.isfile(top_dir):
         file = top_dir
         process_single(file, args)
     if not os.path.isdir(top_dir):
         print('%s is not a directory or doesnt exist.'%top_dir)
@@ -273,10 +273,7 @@
     sys.exit(0)
     
 if __name__ == '__main__':
     main()
 
 
 
-
-
-
```

### Comparing `tictacsync-0.4a0/tictacsync/multi2polywav.py` & `tictacsync-0.5a0/tictacsync/multi2polywav.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     return n_frames
 
 
 def build_poly_name(multifiles):
     """
     Returns string of polywav filename, constructed from similitudes between
     multifile names. Ex:
-    /full/path/4CH002I.wav and /full/path/4CH002M.wav returns 4CH002X.wav
+    4CH002I.wav and 4CH002M.wav returns 4CH002X.wav
     """
     s1 = str(multifiles[0].stem)
     s2 = str(multifiles[1].stem)
     if len(s1) != len(s2):
         print('Can not build compound name with %s.wav and %s.wav'%(s1,s2))
         print('names lengths differ.')
         print('In folder "%s", quitting.'%multifiles[0].parent)
@@ -92,14 +92,15 @@
     os.replace(tempfile_for_metadata, to_file)
 
 def build_poly(multifiles):
     # constructs poly name and calls sox
     # multifiles is list of Path
     # change extensions to mfw (multifile wav)
     dir_multi = multifiles[0].parent
+    multifiles.reverse()
     poly_name_b = build_poly_name(multifiles) # base only
     poly_name = str(dir_multi/Path(poly_name_b))
     filenames = [str(p) for p in multifiles]
     logger.debug('sox.build args: %s %s'%(
         filenames,
         poly_name))
     cbn = sox.Combiner()
```

### Comparing `tictacsync-0.4a0/tictacsync/timeline.py` & `tictacsync-0.5a0/tictacsync/timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from loguru import logger
 import sox
 from pathlib import Path
 from rich import print
 from itertools import groupby
 # import opentimelineio as otio
 from datetime import timedelta
-import pprint, shutil, os
+import pprint, shutil, os, sys
 from subprocess import Popen, PIPE
 
 from inspect import currentframe, getframeinfo
 try:
     from . import yaltc
+    from . import device_scanner
 except:
     import yaltc
+    import device_scanner
 
 CLUSTER_GAP = 0.5 # secs between multicam clusters
 DEL_TEMP = False
 DB_OSX_NORM = -6 #dB
 OUT_DIR_DEFAULT = 'SyncedMedia'
 
 # utility for accessing pathnames
@@ -214,15 +216,14 @@
             print('Error, sox did not normalize file in _sox_mix_channels()')
             sys.exit(1)
         return mono_tpfl
     else:
         # stereo tracks present, so stereo output
         logger.debug('stereo tracks present %s, so stereo output'%stereo_pairs)
         stereo_files = [_sox_keep(pair) for pair in stereo_pairs]
-    #### ???
     return 
 
 def _sox_mono2stereo(temp_file) -> tempfile.NamedTemporaryFile:
     # upgrade a mono file to stereo panning 50-50
     stereo_tempfile = tempfile.NamedTemporaryFile(suffix='.wav',
                     delete=DEL_TEMP)
     tfm = sox.Transformer()
@@ -713,38 +714,54 @@
         logger.debug('device %s'%device)
         if device.n_chan == 2:
             # tracks.txt or not,
             # it's stereo, ie audio + TTC, so remove TTC and return
             kept_channel = (device.ttc + 1)%2 # 1 -> 0 and 0 -> 1
             logger.debug('no tracks.txt, keeping one chan %i'%kept_channel)
             return _sox_keep(multichan_tmpfl, [kept_channel + 1]) #-------------
+        logger.debug('device.n_chan != 2, so multitrack')
         # it's multitrack (more than 2 channels)
         if device.tracks is None:
             # multitrack but no mix done on location, so do mono mix with all
             all_channels = list(range(device.n_chan))
             logger.debug('multitrack but no tracks.txt, mixing %s except TTC at %i'%
                 (all_channels, device.ttc))
             all_channels.remove(device.ttc)
             sox_kept_channels = [i + 1 for i in all_channels] # sox indexing
             logger.debug('mixing channels: %s (sox #)'%sox_kept_channels)
             kept_audio = _sox_keep(multichan_tmpfl, sox_kept_channels)
             return _sox_mix_channels(kept_audio) #------------------------------
-        # user wrote a tracks.txt metadata file, check it
+        logger.debug('there IS a device.tracks')
+        # user wrote a tracks.txt metadata file, check it to get the mix(or do
+        # it). But first a check is done if the ttc tracks concur: the track
+        # detected by the Decoder class, stored in device.ttc VS the track
+        # declared by the user, device.tracks.ttc (see device_scanner.py). If
+        # not, warn the user and exit.
+        logger.debug('ttc channel declared for the device: %i, ttc detected: %i, non zero base indexing'%
+                        (device.ttc, device.tracks.ttc))
+        if device.ttc + 1 != device.tracks.ttc: # warn and quit
+            print('Error: TicTacCode channel detected is [gold1]%i[/gold1]'%
+                device.ttc + 1, end=' ')
+            print('and the file [gold1]%s[/gold1] specifies channel [gold1]%i[/gold1],'%
+                (device_scanner.TRACKSFN, device.tracks.ttc))
+            print('Please correct the discrepancy and rerun. Quitting.')
+            sys.exit(1)
         if device.tracks.mix == [] and device.tracks.stereomics == []:
             # it's multitrac and no mix done on location, so do a mono mix with
             # all, but here remove '0' and TTC tracks from mix
             all_channels = list(range(1, device.n_chan + 1)) # sox not ZBIDX
             to_remove = device.tracks.unused + [device.ttc+1]# unused is sox idx
             logger.debug('multitrack but no tracks.txt, mixing %s except # %s (sox #)'%
                 (all_channels, to_remove))
             sox_kept_channels = [i for i in all_channels
                                             if i not in to_remove]
             logger.debug('mixing channels: %s (sox #)'%sox_kept_channels)
             kept_audio = _sox_keep(multichan_tmpfl, sox_kept_channels)
             return _sox_mix_channels(kept_audio) #------------------------------
+        logger.debug('device.tracks.mix != [] or device.tracks.stereomics != []')
         if device.tracks.mix != []:
             # Mix were done on location, no and we only have to extracted it
             # from the recording. If mono mix, device.tracks.mix has one element;
             # if stereo mix, device.tracks.mix is a pair of number:
             logger.debug('%s has mix %s'%(device.name, device.tracks.mix))
             logger.debug('device %s'%device)
             # just checking coherency
@@ -760,30 +777,33 @@
                 print('Error: ttc channel # incoherency in track.txt')
                 sys.exit(1)
             # coherency check done, extract mix track (or tracks if stereo)
             mix_kind = 'mono' if len(device.tracks.mix) == 1 else 'stereo'
             logger.debug('%s mix declared on channel %s (sox #)'%
                     (mix_kind, device.tracks.mix))
             return _sox_keep(multichan_tmpfl, device.tracks.mix) #--------------
-        # if here, all cases have been covered except tracks.txt AND no mix AND
-        # stereo mic(s) so first a coherency check, and then proceed
+        logger.debug('device.tracks.mix == []')
+        # if here, all cases have been covered, all is remaining is this case:
+        # tracks.txt exists  AND there is no mix AND stereo mic(s) so first a
+        # coherency check, and then proceed
         if device.tracks.stereomics == []:
             print('Error, no stereo mic?, check tracks.txt. Quitting')
             sys.exit(1)
         logger.debug('processing stereo pair(s) %s'%device.tracks.stereomics)
         stereo_mic_idx_pairs = [pair for name, pair in device.tracks.stereomics]
         logger.debug('stereo pairs idxs %s'%stereo_mic_idx_pairs)
         mic_stereo_files = [_sox_keep(multichan_tmpfl, pair) for pair
                                                     in stereo_mic_idx_pairs]
         # flatten list of tuples of channels being stereo mics
         stereo_mic_idx_flat = [item for sublist in stereo_mic_idx_pairs
                                                     for item in sublist]
         logger.debug('stereo_mic_idx_flat %s'%stereo_mic_idx_flat)
         mono_tracks = [i for i in range(1, device.n_chan + 1)
                                 if i not in stereo_mic_idx_flat]
+        logger.debug('mono_tracks: %s'%mono_tracks)
         # remove TTC track number
         mono_tracks.remove(device.ttc + 1)
         logger.debug('mono_tracks %s'%mono_tracks)
         mono_files = [_sox_keep(multichan_tmpfl, [chan]) for chan
                                                     in mono_tracks]
         new_stereo_files = [_sox_mono2stereo(f) for f in mono_files]
         stereo_files = mic_stereo_files + new_stereo_files
@@ -827,16 +847,19 @@
             synced_clip_dir = synced_clip_dir/device_name # = synced_clip_dir/ZOOM
         self.synced_clip_dir = synced_clip_dir
         os.makedirs(synced_clip_dir, exist_ok=True)
         logger.debug('synced_clip_dir is: %s'%synced_clip_dir)
         synced_clip_file = synced_clip_dir/\
             Path(self.videoclip.new_rec_name).name
         logger.debug('editing files for %s'%synced_clip_file)
-        self.videoclip.final_synced_file = synced_clip_file # relative
-        # collecting edited audio by device, in (Device, tempfile) pairs:
+        self.videoclip.final_synced_file = synced_clip_file # relative path
+        # Collecting edited audio by device, in (Device, tempfile) pairs:
+        # for a given self.videoclip, each audio device will have a sequence
+        # of matched, synced and joined audio files present in a single
+        # edited audio file, returned by _get_concatenated_audiofile_for
         merged_audio_files_by_device = [
                             (d, self._get_concatenated_audiofile_for(d)) 
                             for d in self._get_audio_devices()]
         if len(merged_audio_files_by_device) == 0:
             # no audio file overlaps for this clip
             return #############################################################
         if len(merged_audio_files_by_device) == 1:
@@ -875,26 +898,14 @@
         multiple_recorders = len(merged_audio_files_by_device) > 1
         logger.debug('multiple_recorder: %s'%multiple_recorders)
         # the device_mixes list contains all audio recorders if many. If only
         # one audiorecorder was used (most of the cases) len(device_mixes) is 1
         device_mixes = [self._get_device_mix(device, multi_chan_audio)
                 for device, multi_chan_audio
                 in merged_audio_files_by_device]
-
-
-
-        # If multiple audio recorders were used and one of
-        # them has mixL and mixR tracks, two possibilities:
-
-        #     A- others have mixL mixR too: mix of device_mixes are done (and none mix
-        #     tracks are ignored but copied in the ISOs folder if asked)
-        #     B- others don't have mixL-mixR: all tracks from them are panned
-        #     50-50 and stereo-mixed
-
-
         logger.debug('there are %i dev device_mixes'%len(device_mixes))
         logger.debug('device_mixes %s'%device_mixes)
         mix_of_device_mixes = _sox_mix_files(device_mixes)
         logger.debug('will merge with %s'%(_pathname(mix_of_device_mixes)))
         self.videoclip.synced_audio = mix_of_device_mixes
         logger.debug('mix_of_device_mixes n chan: %i'%
             sox.file_info.channels(_pathname(mix_of_device_mixes)))
@@ -906,15 +917,15 @@
         # devices_and_monofiles:
         if asked_ISOs:
             devices_and_monofiles = [(device, _split_channels(multi_chan_audio))
                     for device, multi_chan_audio
                     in merged_audio_files_by_device]
             logger.debug('devices_and_monofiles: %s'%
                 pprint.pformat(devices_and_monofiles))
-            def _trnm(dev, idx): # used in the list comprehension just below
+            def _trnm(dev, idx): # used in the loop just below
                 # generates track name for later if asked_ISOs
                 # idx is from 0 to nchan-1 for this device
                 if dev.tracks == None:
                     tag = 'chan%s'%str(idx+1).zfill(2)
                 else:
                     # audio_tags = [tag for tag in dev.tracks.rawtrx
                     #     if tag not in ['ttc','0','tc']]
@@ -924,15 +935,18 @@
                 logger.debug('tag %s'%tag)
                 return tag #####################################################
             # replace device, idx pair with track name (+ device name if many)
             # loop over devices than loop over tracks
             names_audio_tempfiles = []
             for dev, mono_tmpfiles_list in devices_and_monofiles:
                 for idx, monotf in enumerate(mono_tmpfiles_list):
-                    names_audio_tempfiles.append((_trnm(dev, idx), monotf))
+                    track_name = _trnm(dev, idx)
+                    if track_name[0] == '0': # muted, skip
+                        continue
+                    names_audio_tempfiles.append((track_name, monotf))
             logger.debug('names_audio_tempfiles %s'%names_audio_tempfiles)
             self._write_ISOs(names_audio_tempfiles)
         logger.debug('merged_audio_files_by_device %s'%
             merged_audio_files_by_device)
         # This loop below for logging purpose only:
         for idx, pair in enumerate(merged_audio_files_by_device):
             # dev_joined_audio is mono, stereo or even polywav from multitrack
```

### Comparing `tictacsync-0.4a0/tictacsync/yaltc.py` & `tictacsync-0.5a0/tictacsync/yaltc.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.4a0/tictacsync.egg-info/PKG-INFO` & `tictacsync-0.5a0/tictacsync.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictacsync
-Version: 0.4a0
+Version: 0.5a0
 Summary: command for syncing audio video recordings
 Home-page: https://tictacsync.org/
 Author: Raymond Lutz
 Author-email: lutzrayblog@mac.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -25,23 +25,29 @@
 
 ## Warning: this is at pre-alpha stage
 
 Unfinished sloppy code ahead, but should run without errors. Some functionalities are still missing. Don't run the code without parental supervision. Suggestions and enquiries are welcome via the [lists hosted on sourcehut](https://sr.ht/~proflutz/TicTacSync/lists).
 
 ## Description
 
-`tictacsync` is a python script to sync audio and video files shot
-with [dual system sound](https://www.learnlightandsound.com/blog/2017/2/23/how-to-record-sound-for-video-dual-systemsync-sound)  using a specific hardware timecode generator
-called [Tic Tac Sync](https://tictacsync.org). The timecode is named YaLTC for *yet
-another longitudinal time code* and should be recorded on a scratch
-track on each device for the syncing to be performed, later in _postprod_ before editing.
-
+`tictacsync` is a python script to sync, cut and join audio files against camera files shot using a specific hardware timecode generator
+called [Tic Tac Sync](https://tictacsync.org). The timecode is named TicTacCode and should be recorded on a scratch
+track on each device for `tictacsync` to work.
 ## Status
 
-`tictacsync`  scans for audio video files and displays their starting time and then merges overlapping audio and video recordings. Multicam syncing with one stereo audio recorder has been tested (spring 2023, [see demo](https://youtu.be/pklTSTi7cqs)). Multi audio recorders coming soon... 
+Feature complete! `tictacsync`  scans for audio video files and then merges overlapping audio and video recordings, It
+
+* Decodes the TicTacCode audio track alongside your audio tracks
+* Establishes UTC start time (and end time) within 100 μs!
+* Syncs, cuts and joins any concurrent audio to camera files (using `FFmpeg`)
+* Processes _multiple_ audio recorders
+* Corrects device clock drift so _both_ ends coincide (thanks to `sox`)
+* Sets video metadata TC of multicam files for NLE timeline alignement
+* Writes _synced_ ISO files with dedicated file names declared in `tracks.txt`
+* Produces nice plots.
 
 
 ## Installation
 
 This uses the [python interpreter](https://www.python.org/downloads/) and multiple packages (so you need python 3 + pip). Also, you need to install two non-python command line executables: [ffmpeg](https://windowsloop.com/install-ffmpeg-windows-10/) and [sox](https://sourceforge.net/projects/sox/files/). Make sure those are _accessible through your `PATH` system environment variable_.
 Then pip install the syncing program:
 
@@ -73,15 +79,15 @@
     > tictacsync -v dailies/loose/MVI_0024.MP4
 
 For a one line output (or to suppress the progress bars) use the `--terse` flag:
 
 	> tictacsync --terse dailies/loose/MVI_0024.MP4 
 	dailies/loose/MVI_0024.MP4 UTC:2024-03-12 23:07:01.4281 pulse: 27450 in chan 0
 
-To also produce _synced_ ISO audio files, specify `--isos` . A directory named `ISOs` will contain _for each synced video_ a set of audio files of exact same length, padded or trimmed to coincide with the video track. After re-editing and re-mixing a `remergemix` command will resync the new sound track with the video [TODO].
+To also produce _synced_ ISO audio files, specify `--isos` . A directory named `ISOs` will contain _for each synced video_ a set of ISO audio files of exact same length, padded or trimmed to coincide with the video track. After re-editing and re-mixing a `remergemix` command will resync the new audio with the video and _the new sound track will be updated on your NLE timeline_, at least in Kdenlive...
 
 	> tictacsync --isos dailies/structured
 
 When called with the `-p` flag, zoomable plots will be produced for diagnostic purpose (close the plotting window for the 2nd one) and the decoded starting time will be output to stdin:
 
     > tictacsync -p dailies/loose/MVI_0024.MP4
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

