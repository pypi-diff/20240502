# Comparing `tmp/moonss-0.96.tar.gz` & `tmp/moonss-0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonss-0.96.tar", last modified: Fri Apr 26 04:07:26 2024, max compression
+gzip compressed data, was "moonss-0.97.tar", last modified: Thu May  2 09:47:38 2024, max compression
```

## Comparing `moonss-0.96.tar` & `moonss-0.97.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:07:26.695057 moonss-0.96/
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-26 04:07:18.000000 moonss-0.96/DownloadHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-26 04:07:26.695057 moonss-0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 04:07:18.000000 moonss-0.96/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-26 04:07:18.000000 moonss-0.96/SourceDataHelper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:07:26.695057 moonss-0.96/moonss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-26 04:07:26.000000 moonss-0.96/moonss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 04:07:26.000000 moonss-0.96/moonss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:07:26.000000 moonss-0.96/moonss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 04:07:26.000000 moonss-0.96/moonss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 04:07:26.000000 moonss-0.96/moonss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-26 04:07:18.000000 moonss-0.96/moonss.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 04:07:26.695057 moonss-0.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-26 04:07:18.000000 moonss-0.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:47:38.927942 moonss-0.97/
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-02 09:47:30.000000 moonss-0.97/DownloadHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-02 09:47:38.923942 moonss-0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 09:47:30.000000 moonss-0.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-02 09:47:30.000000 moonss-0.97/SourceDataHelper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:47:38.923942 moonss-0.97/moonss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-02 09:47:38.000000 moonss-0.97/moonss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-02 09:47:38.000000 moonss-0.97/moonss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:47:38.000000 moonss-0.97/moonss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 09:47:38.000000 moonss-0.97/moonss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 09:47:38.000000 moonss-0.97/moonss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-02 09:47:30.000000 moonss-0.97/moonss.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:47:38.927942 moonss-0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-02 09:47:30.000000 moonss-0.97/setup.py
```

### Comparing `moonss-0.96/DownloadHelper.py` & `moonss-0.97/DownloadHelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,20 @@
     return download_file(f"https://aweme.snssdk.com/aweme/v1/play/?video_id={video_id}&ratio=1080p&line=0",None, "mp4")
 def donwload_instagram_video(crawl_data_txt):
     crawl_data = json.loads(crawl_data_txt)
     if "video_url" in crawl_data:
         return download_file(crawl_data['video_url'],None, "mp4")
     else:
         return None
+def download_ffmpeg(url):
+    file_path=os.path.join(get_dir(),uuid.uuid4().hex+".mp4")
+    cmd=f"ffmpeg -i \"{url}\" -c copy {file_path}"
+    os.system(cmd)
+    return file_path
 def donwload_artlistio_video(crawl_data_txt):
     crawl_data = json.loads(crawl_data_txt)
-    if "video_url" in crawl_data:
-        return download_file(crawl_data['video_url'],None, "mp4")
+    if "video_m3u8" in crawl_data:
+        url=crawl_data['video_m3u8'].replace("_playlist","_1080p")
+        return download_ffmpeg(url)
     else:
         return None
```

### Comparing `moonss-0.96/PKG-INFO` & `moonss-0.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonss
-Version: 0.96
+Version: 0.97
 Summary: A Des of moonss
 Home-page: https://github.com/vtandroid/dokr
 Author: Thanh Hoa
 Author-email: thanhhoakhmt1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moonss-0.96/SourceDataHelper.py` & `moonss-0.97/SourceDataHelper.py`

 * *Files identical despite different names*

### Comparing `moonss-0.96/moonss.egg-info/PKG-INFO` & `moonss-0.97/moonss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonss
-Version: 0.96
+Version: 0.97
 Summary: A Des of moonss
 Home-page: https://github.com/vtandroid/dokr
 Author: Thanh Hoa
 Author-email: thanhhoakhmt1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moonss-0.96/moonss.py` & `moonss-0.97/moonss.py`

 * *Files identical despite different names*

### Comparing `moonss-0.96/setup.py` & `moonss-0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='moonss',
-    version='0.96',
+    version='0.97',
     author="Thanh Hoa",
     author_email="thanhhoakhmt1@gmail.com",
     description="A Des of moonss",
     long_description="Des",
     long_description_content_type="text/markdown",
     url="https://github.com/vtandroid/dokr",
     packages=setuptools.find_packages(),
```

