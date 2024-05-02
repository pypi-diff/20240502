# Comparing `tmp/qfpy-8.0.0.tar.gz` & `tmp/qfpy-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-8.0.0.tar", last modified: Tue Apr 30 18:25:41 2024, max compression
+gzip compressed data, was "qfpy-8.0.1.tar", last modified: Thu May  2 05:55:45 2024, max compression
```

## Comparing `qfpy-8.0.0.tar` & `qfpy-8.0.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 18:25:41.869123 qfpy-8.0.0/
--rw-rw-rw-   0        0        0      159 2024-04-30 18:25:41.868122 qfpy-8.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-30 18:24:48.000000 qfpy-8.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 18:25:41.870124 qfpy-8.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 18:25:41.846122 qfpy-8.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 18:25:41.860203 qfpy-8.0.0/src/qfpy/
--rw-rw-rw-   0        0        0       90 2024-04-30 18:19:38.000000 qfpy-8.0.0/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0      210 2024-04-29 16:48:36.000000 qfpy-8.0.0/src/qfpy/character.py
--rw-rw-rw-   0        0        0      131 2024-04-29 17:01:55.000000 qfpy-8.0.0/src/qfpy/crypto.py
--rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-8.0.0/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     3067 2024-04-29 16:52:59.000000 qfpy-8.0.0/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-8.0.0/src/qfpy/folder.py
--rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-8.0.0/src/qfpy/function.py
--rw-rw-rw-   0        0        0     1170 2024-04-30 18:20:15.000000 qfpy-8.0.0/src/qfpy/process.py
--rw-rw-rw-   0        0        0      525 2024-04-30 18:24:38.000000 qfpy-8.0.0/src/qfpy/system.py
-drwxrwxrwx   0        0        0        0 2024-04-30 18:25:41.867123 qfpy-8.0.0/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      159 2024-04-30 18:25:41.000000 qfpy-8.0.0/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-04-30 18:25:41.000000 qfpy-8.0.0/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 18:25:41.000000 qfpy-8.0.0/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-30 18:25:41.000000 qfpy-8.0.0/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 05:55:45.484305 qfpy-8.0.1/
+-rw-rw-rw-   0        0        0      229 2024-05-02 05:55:45.481434 qfpy-8.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-02 05:55:33.000000 qfpy-8.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 05:55:45.484305 qfpy-8.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 05:55:45.447538 qfpy-8.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 05:55:45.469097 qfpy-8.0.1/src/qfpy/
+-rw-rw-rw-   0        0        0       90 2024-04-30 18:19:38.000000 qfpy-8.0.1/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0      210 2024-04-29 16:48:36.000000 qfpy-8.0.1/src/qfpy/character.py
+-rw-rw-rw-   0        0        0      131 2024-04-29 17:01:55.000000 qfpy-8.0.1/src/qfpy/crypto.py
+-rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-8.0.1/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     2988 2024-05-02 05:54:03.000000 qfpy-8.0.1/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-8.0.1/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-8.0.1/src/qfpy/function.py
+-rw-rw-rw-   0        0        0     1170 2024-04-30 18:20:15.000000 qfpy-8.0.1/src/qfpy/process.py
+-rw-rw-rw-   0        0        0      525 2024-04-30 18:24:38.000000 qfpy-8.0.1/src/qfpy/system.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:55:45.479839 qfpy-8.0.1/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      229 2024-05-02 05:55:45.000000 qfpy-8.0.1/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-05-02 05:55:45.000000 qfpy-8.0.1/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 05:55:45.000000 qfpy-8.0.1/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-02 05:55:45.000000 qfpy-8.0.1/src/qfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-02 05:55:45.000000 qfpy-8.0.1/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-8.0.0/src/qfpy/exif.py` & `qfpy-8.0.1/src/qfpy/exif.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.0.0/src/qfpy/ffmpeg.py` & `qfpy-8.0.1/src/qfpy/ffmpeg.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,36 +39,28 @@
     # 将合并后的视频写入指定的输出文件
     final_clip.write_videofile(output_file)
     # 删除所有原始视频文件
     for f in files:
         f.unlink()
 
 
-class MetadataParsedError(OSError):
-    """
-    metadata 解析错误
-    """
-
-    pass
-
-
 class FFprobe:
     """
     方法
 
     duration：获取视频时长
 
     codec：获取视频编码
 
     size：获取视频大小
     """
     def __init__(self, file: str):
         self.metadata = self.__ffprobe(file)
         if not self.metadata:
-            raise MetadataParsedError(file)
+            raise Exception("metadata 解析错误：" + file)
 
     def __repr__(self):
         return str(self.metadata)
 
     def __ffprobe(self, file: str) -> dict:
         """
         私有方法：获取视频的元数据信息。
```

### Comparing `qfpy-8.0.0/src/qfpy/folder.py` & `qfpy-8.0.1/src/qfpy/folder.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.0.0/src/qfpy/function.py` & `qfpy-8.0.1/src/qfpy/function.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.0.0/src/qfpy/process.py` & `qfpy-8.0.1/src/qfpy/process.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.0.0/src/qfpy/system.py` & `qfpy-8.0.1/src/qfpy/system.py`

 * *Files identical despite different names*

