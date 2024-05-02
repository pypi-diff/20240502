# Comparing `tmp/better-ffmpeg-progress-2.1.4.tar.gz` & `tmp/better-ffmpeg-progress-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\better-ffmpeg-progress-2.1.4.tar", last modified: Sun Apr 28 16:12:35 2024, max compression
+gzip compressed data, was "dist\better-ffmpeg-progress-2.1.5.tar", last modified: Thu May  2 18:37:40 2024, max compression
```

## Comparing `better-ffmpeg-progress-2.1.4.tar` & `better-ffmpeg-progress-2.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/
-drwxrwxrwx   0        0        0        0 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress/
--rw-rw-rw-   0        0        0     6098 2024-04-28 15:59:22.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress/better_ffmpeg_progress.py
--rw-rw-rw-   0        0        0       50 2024-04-22 18:00:24.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     6458 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       19 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/requires.txt
--rw-rw-rw-   0        0        0      339 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       23 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-08-29 21:18:31.000000 better-ffmpeg-progress-2.1.4/LICENSE
--rw-rw-rw-   0        0        0     6458 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4801 2024-04-28 16:01:33.000000 better-ffmpeg-progress-2.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 16:12:35.000000 better-ffmpeg-progress-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      808 2024-04-28 16:00:20.000000 better-ffmpeg-progress-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:37:40.000000 better-ffmpeg-progress-2.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:37:40.000000 better-ffmpeg-progress-2.1.5/better_ffmpeg_progress/
+-rw-rw-rw-   0        0        0     6367 2024-05-02 18:31:35.000000 better-ffmpeg-progress-2.1.5/better_ffmpeg_progress/better_ffmpeg_progress.py
+-rw-rw-rw-   0        0        0       50 2024-04-22 18:00:24.000000 better-ffmpeg-progress-2.1.5/better_ffmpeg_progress/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:37:40.000000 better-ffmpeg-progress-2.1.5/better_ffmpeg_progress.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-02 18:37:40.000000 better-ffmpeg-progress-2.1.5/better_ffmpeg_progress.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     6458 2024-05-02 18:37:40.000000 better-ffmpeg-progress-2.1.5/better_ffmpeg_progress.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2024-05-02 18:37:40.000000 better-ffmpeg-progress-2.1.5/better_ffmpeg_progress.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      339 2024-05-02 18:37:40.000000 better-ffmpeg-progress-2.1.5/better_ffmpeg_progress.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       23 2024-05-02 18:37:40.000000 better-ffmpeg-progress-2.1.5/better_ffmpeg_progress.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-08-29 21:18:31.000000 better-ffmpeg-progress-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6458 2024-05-02 18:37:40.000000 better-ffmpeg-progress-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4801 2024-05-02 18:36:23.000000 better-ffmpeg-progress-2.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 18:37:40.000000 better-ffmpeg-progress-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      808 2024-05-02 18:34:41.000000 better-ffmpeg-progress-2.1.5/setup.py
```

### Comparing `better-ffmpeg-progress-2.1.4/better_ffmpeg_progress/better_ffmpeg_progress.py` & `better-ffmpeg-progress-2.1.5/better_ffmpeg_progress/better_ffmpeg_progress.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,60 +68,55 @@
                 return False
 
             self._ffmpeg_args.insert(1, "-y")
             return True
 
         return True
 
-    def _update_progress(self, ffmpeg_output, progress_handler):
-        if ffmpeg_output:
-            value = ffmpeg_output.split("=")[1].strip()
-
-            if progress_handler is None:
-                if "out_time_ms" in ffmpeg_output:
-                    seconds_processed = round(int(value) / 1_000_000, 1)
-                    seconds_increase = seconds_processed - self._previous_seconds_processed
-                    self._progress_bar.update(seconds_increase)
-                    self._previous_seconds_processed = seconds_processed
-
-            else:
-                if "total_size" in ffmpeg_output and "N/A" not in value:
-                    self._current_size = int(value)
+    def _update_progress(self, ffmpeg_output, metric_name, value, progress_handler):
+        if progress_handler is None:
+            if metric_name == "out_time_ms":
+                seconds_processed = round(int(value) / 1_000_000, 1)
+                seconds_increase = seconds_processed - self._previous_seconds_processed
+                self._progress_bar.update(seconds_increase)
+                self._previous_seconds_processed = seconds_processed
+
+        else:
+            if metric_name == "total_size":
+                self._current_size = int(value)
+
+            elif metric_name == "out_time_ms":
+                self._seconds_processed = int(value) / 1_000_000
+
+                if self._can_get_duration:
+                    self._percentage_progress = (
+                        self._seconds_processed / self._duration_secs
+                    ) * 100
+
+                    if self._current_size is not None and self._percentage_progress != 0.0:
+                        self._estimated_size = self._current_size * (
+                            100 / self._percentage_progress
+                        )
 
-                elif "out_time_ms" in ffmpeg_output:
-                    self._seconds_processed = int(value) / 1_000_000
+            elif metric_name == "speed":
+                speed_str = value[:-1]
+
+                if speed_str != "0":
+                    self._speed = float(speed_str)
 
                     if self._can_get_duration:
-                        self._percentage_progress = (
-                            self._seconds_processed / self._duration_secs
-                        ) * 100
-
-                        if self._current_size is not None and self._percentage_progress != 0.0:
-                            self._estimated_size = self._current_size * (
-                                100 / self._percentage_progress
-                            )
-
-                elif "speed" in ffmpeg_output:
-                    speed_str = value[:-1]
-
-                    if speed_str != "0" and "N/A" not in value:
-                        self._speed = float(speed_str)
-
-                        if self._can_get_duration:
-                            self._eta = (
-                                self._duration_secs - self._seconds_processed
-                            ) / self._speed
-
-                if ffmpeg_output == "progress=end":
-                    self._percentage_progress = 100
-                    self._eta = 0
+                        self._eta = (self._duration_secs - self._seconds_processed) / self._speed
 
-                progress_handler(
-                    self._percentage_progress, self._speed, self._eta, self._estimated_size
-                )
+            if ffmpeg_output == "progress=end":
+                self._percentage_progress = 100
+                self._eta = 0
+
+            progress_handler(
+                self._percentage_progress, self._speed, self._eta, self._estimated_size
+            )
 
     def run(
         self,
         progress_handler=None,
         ffmpeg_output_file=None,
         success_handler=None,
         error_handler=None,
@@ -141,33 +136,49 @@
             self._progress_bar = tqdm(
                 total=round(self._duration_secs, 1),
                 unit="s",
                 dynamic_ncols=True,
                 leave=False,
             )
 
-        try:
             while process.poll() is None:
-                ffmpeg_output = process.stdout.readline().decode().strip()
-                self._update_progress(ffmpeg_output, progress_handler)
+                try:
+                    ffmpeg_output = process.stdout.readline().decode().strip()
+
+                except KeyboardInterrupt:
+                    self._progress_bar.close()
+                    print("[KeyboardInterrupt] FFmpeg process killed.")
+                    sys.exit()
+
+                except Exception as e:
+                    print(f"Unable to read FFmpeg output:\n{e}")
+
+                else:
+                    if not ffmpeg_output:
+                        continue
+
+                    metric_name = ffmpeg_output.split("=")[0]
+                    wanted_metrics = ["out_time_ms", "total_size", "speed"]
+
+                    if metric_name not in wanted_metrics:
+                        continue
+
+                    value = ffmpeg_output.split("=")[1].strip()
+
+                    if not value or "N/A" in value:
+                        continue
+
+                    self._update_progress(ffmpeg_output, metric_name, value, progress_handler)
 
             if process.returncode != 0:
                 if error_handler:
                     error_handler()
                     return
 
                 print(
                     f"The FFmpeg process encountered an error. The output of FFmpeg can be found in {ffmpeg_output_file}"
                 )
 
             if success_handler:
                 success_handler()
 
             print(f"\n\nDone! To see FFmpeg's output, check out {ffmpeg_output_file}")
-
-        except KeyboardInterrupt:
-            self._progress_bar.close()
-            print("[KeyboardInterrupt] FFmpeg process killed.")
-            sys.exit()
-
-        except Exception as e:
-            print(f"[Better FFmpeg Process] {e}")
```

### Comparing `better-ffmpeg-progress-2.1.4/better_ffmpeg_progress.egg-info/PKG-INFO` & `better-ffmpeg-progress-2.1.5/better_ffmpeg_progress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-ffmpeg-progress
-Version: 2.1.4
+Version: 2.1.5
 Summary: Run FFmpeg & see percentage progress + ETA.
 Home-page: https://github.com/CrypticSignal/better-ffmpeg-progress
 Author: GitHub.com/CrypticSignal
 Author-email: theaudiophile@outlook.com
 License: UNKNOWN
 Description: <div align="center">
```

### Comparing `better-ffmpeg-progress-2.1.4/LICENSE` & `better-ffmpeg-progress-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `better-ffmpeg-progress-2.1.4/PKG-INFO` & `better-ffmpeg-progress-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-ffmpeg-progress
-Version: 2.1.4
+Version: 2.1.5
 Summary: Run FFmpeg & see percentage progress + ETA.
 Home-page: https://github.com/CrypticSignal/better-ffmpeg-progress
 Author: GitHub.com/CrypticSignal
 Author-email: theaudiophile@outlook.com
 License: UNKNOWN
 Description: <div align="center">
```

### Comparing `better-ffmpeg-progress-2.1.4/README.md` & `better-ffmpeg-progress-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `better-ffmpeg-progress-2.1.4/setup.py` & `better-ffmpeg-progress-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="better-ffmpeg-progress",
-    version="2.1.4",
+    version="2.1.5",
     author="GitHub.com/CrypticSignal",
     author_email="theaudiophile@outlook.com",
     description="Run FFmpeg & see percentage progress + ETA.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CrypticSignal/better-ffmpeg-progress",
     packages=["better_ffmpeg_progress"],
```

