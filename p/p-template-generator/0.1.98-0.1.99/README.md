# Comparing `tmp/p-template-generator-0.1.98.tar.gz` & `tmp/p-template-generator-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-template-generator-0.1.98.tar", last modified: Fri Dec  8 08:34:29 2023, max compression
+gzip compressed data, was "p-template-generator-0.1.99.tar", last modified: Thu Dec 28 05:10:56 2023, max compression
```

## Comparing `p-template-generator-0.1.98.tar` & `p-template-generator-0.1.99.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-12-08 08:34:29.407476 p-template-generator-0.1.98/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-template-generator-0.1.98/LICENSE
--rw-rw-rw-   0        0        0      406 2023-12-08 08:34:29.407476 p-template-generator-0.1.98/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-03-14 06:24:47.000000 p-template-generator-0.1.98/README.md
-drwxrwxrwx   0        0        0        0 2023-12-08 08:34:29.384344 p-template-generator-0.1.98/p_template_generator.egg-info/
--rw-rw-rw-   0        0        0      406 2023-12-08 08:34:29.000000 p-template-generator-0.1.98/p_template_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-12-08 08:34:29.000000 p-template-generator-0.1.98/p_template_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-08 08:34:29.000000 p-template-generator-0.1.98/p_template_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-12-08 08:34:29.000000 p-template-generator-0.1.98/p_template_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-12-08 08:34:29.000000 p-template-generator-0.1.98/p_template_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-12-08 08:34:29.000000 p-template-generator-0.1.98/p_template_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-08 08:34:29.408478 p-template-generator-0.1.98/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-12-08 08:34:25.000000 p-template-generator-0.1.98/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-08 08:34:29.392352 p-template-generator-0.1.98/template_generator/
--rw-rw-rw-   0        0        0        0 2023-12-07 02:47:11.000000 p-template-generator-0.1.98/template_generator/__init__.py
--rw-rw-rw-   0        0        0     6065 2023-11-30 12:32:15.000000 p-template-generator-0.1.98/template_generator/aigc_input.py
-drwxrwxrwx   0        0        0        0 2023-12-08 08:34:29.394863 p-template-generator-0.1.98/template_generator/bin/
--rw-rw-rw-   0        0        0        0 2023-12-07 02:47:11.000000 p-template-generator-0.1.98/template_generator/bin/__init__.py
--rw-rw-rw-   0        0        0      709 2023-11-30 12:32:25.000000 p-template-generator-0.1.98/template_generator/bin/print_md5.py
--rw-rw-rw-   0        0        0     4881 2023-12-08 08:34:18.000000 p-template-generator-0.1.98/template_generator/binary.py
-drwxrwxrwx   0        0        0        0 2023-12-08 08:34:29.397951 p-template-generator-0.1.98/template_generator/convertor/
--rw-rw-rw-   0        0        0        0 2023-12-07 02:47:11.000000 p-template-generator-0.1.98/template_generator/convertor/__init__.py
--rw-rw-rw-   0        0        0     8692 2023-11-21 09:36:44.000000 p-template-generator-0.1.98/template_generator/convertor/convertor.py
--rw-rw-rw-   0        0        0    55927 2023-11-10 11:06:14.000000 p-template-generator-0.1.98/template_generator/convertor/of_to_skymedia.py
--rw-rw-rw-   0        0        0     4269 2023-11-28 10:25:30.000000 p-template-generator-0.1.98/template_generator/ffmpeg.py
--rw-rw-rw-   0        0        0     9455 2023-11-30 12:31:34.000000 p-template-generator-0.1.98/template_generator/main.py
--rw-rw-rw-   0        0        0     8693 2023-12-02 09:28:58.000000 p-template-generator-0.1.98/template_generator/server_generator.py
--rw-rw-rw-   0        0        0    15537 2023-12-04 05:39:09.000000 p-template-generator-0.1.98/template_generator/template.py
--rw-rw-rw-   0        0        0     3822 2023-11-30 09:02:49.000000 p-template-generator-0.1.98/template_generator/template_service.py
--rw-rw-rw-   0        0        0    10844 2023-11-30 12:32:17.000000 p-template-generator-0.1.98/template_generator/template_test.py
-drwxrwxrwx   0        0        0        0 2023-12-08 08:34:29.398959 p-template-generator-0.1.98/template_generator/test/
--rw-rw-rw-   0        0        0        0 2023-12-07 02:47:11.000000 p-template-generator-0.1.98/template_generator/test/__init__.py
--rw-rw-rw-   0        0        0  9341185 2023-11-21 10:17:45.000000 p-template-generator-0.1.98/template_generator/test/tp_2023112102.zip.py
+drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.369647 p-template-generator-0.1.99/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-template-generator-0.1.99/LICENSE
+-rw-rw-rw-   0        0        0      406 2023-12-28 05:10:56.369647 p-template-generator-0.1.99/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-03-14 06:24:47.000000 p-template-generator-0.1.99/README.md
+drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.344969 p-template-generator-0.1.99/p_template_generator.egg-info/
+-rw-rw-rw-   0        0        0      406 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-12-28 05:10:56.000000 p-template-generator-0.1.99/p_template_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-28 05:10:56.370643 p-template-generator-0.1.99/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-12-28 05:10:46.000000 p-template-generator-0.1.99/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.353426 p-template-generator-0.1.99/template_generator/
+-rw-rw-rw-   0        0        0        0 2023-12-28 02:03:28.000000 p-template-generator-0.1.99/template_generator/__init__.py
+-rw-rw-rw-   0        0        0     6065 2023-11-30 12:32:15.000000 p-template-generator-0.1.99/template_generator/aigc_input.py
+drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.355114 p-template-generator-0.1.99/template_generator/bin/
+-rw-rw-rw-   0        0        0        0 2023-12-28 02:03:28.000000 p-template-generator-0.1.99/template_generator/bin/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-11-30 12:32:25.000000 p-template-generator-0.1.99/template_generator/bin/print_md5.py
+-rw-rw-rw-   0        0        0     4875 2023-12-28 05:10:29.000000 p-template-generator-0.1.99/template_generator/binary.py
+drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.359125 p-template-generator-0.1.99/template_generator/convertor/
+-rw-rw-rw-   0        0        0        0 2023-12-28 02:03:28.000000 p-template-generator-0.1.99/template_generator/convertor/__init__.py
+-rw-rw-rw-   0        0        0     8692 2023-11-21 09:36:44.000000 p-template-generator-0.1.99/template_generator/convertor/convertor.py
+-rw-rw-rw-   0        0        0    55927 2023-11-10 11:06:14.000000 p-template-generator-0.1.99/template_generator/convertor/of_to_skymedia.py
+-rw-rw-rw-   0        0        0     4269 2023-11-28 10:25:30.000000 p-template-generator-0.1.99/template_generator/ffmpeg.py
+-rw-rw-rw-   0        0        0     9455 2023-11-30 12:31:34.000000 p-template-generator-0.1.99/template_generator/main.py
+-rw-rw-rw-   0        0        0     8693 2023-12-02 09:28:58.000000 p-template-generator-0.1.99/template_generator/server_generator.py
+-rw-rw-rw-   0        0        0    15537 2023-12-04 05:39:09.000000 p-template-generator-0.1.99/template_generator/template.py
+-rw-rw-rw-   0        0        0     3822 2023-11-30 09:02:49.000000 p-template-generator-0.1.99/template_generator/template_service.py
+-rw-rw-rw-   0        0        0    10941 2023-12-27 07:06:17.000000 p-template-generator-0.1.99/template_generator/template_test.py
+drwxrwxrwx   0        0        0        0 2023-12-28 05:10:56.360125 p-template-generator-0.1.99/template_generator/test/
+-rw-rw-rw-   0        0        0        0 2023-12-28 02:03:28.000000 p-template-generator-0.1.99/template_generator/test/__init__.py
+-rw-rw-rw-   0        0        0  9341185 2023-11-21 10:17:45.000000 p-template-generator-0.1.99/template_generator/test/tp_2023112102.zip.py
```

### Comparing `p-template-generator-0.1.98/LICENSE` & `p-template-generator-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/p_template_generator.egg-info/SOURCES.txt` & `p-template-generator-0.1.99/p_template_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/setup.py` & `p-template-generator-0.1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-template-generator",
-    version="0.1.98",
+    version="0.1.99",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="temple tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `p-template-generator-0.1.98/template_generator/aigc_input.py` & `p-template-generator-0.1.99/template_generator/aigc_input.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/template_generator/bin/print_md5.py` & `p-template-generator-0.1.99/template_generator/bin/print_md5.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/template_generator/binary.py` & `p-template-generator-0.1.99/template_generator/binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,16 @@
             fext = key[key.index("."):]
             fdirpath = os.path.join(rootDir, fname)
             if os.path.exists(fdirpath) and fmd5 != readDirChecksum(fdirpath):
                 logging.info(f"remove old {fdirpath}")
                 shutil.rmtree(fdirpath)
         
 def updateBin(rootDir):
-    
     getOssResource(rootDir, "https://m.mecordai.com/res/ffmpeg.zip", "a9e6b05ac70f6416d5629c07793b4fcf", "ffmpeg.zip.py")
-    getOssResource(rootDir, "https://m.mecordai.com/res/skymedia_20231208.zip", "8a996cc289005cdd5999ddaf628cb313", "skymedia.zip.py")
+    getOssResource(rootDir, "https://m.mecordai.com/res/skymedia_20231228.zip", "0adb05e450cf3fc8d5ad4651e7c04649", "skymedia.zip.py")
     getOssResource(rootDir, "https://m.mecordai.com/res/randomTemplates_20230625.zip", "e0cf7eaed4a90d59fe82f41b02f3d17e", "randomTemplates.zip.py")
     getOssResource(rootDir, "https://m.mecordai.com/res/subEffect.zip", "08651251e4351fd8cd5829b2ef65a8b9", "subEffect.zip.py")
     getOssResource(rootDir, "https://m.mecordai.com/res/fonts.zip", "b1f190ba1cea49177eccde2eb2a6cb13", "fonts.zip.py")
     checkFileMd5(rootDir)
 
     for root,dirs,files in os.walk(rootDir):
         for file in files:
```

### Comparing `p-template-generator-0.1.98/template_generator/convertor/convertor.py` & `p-template-generator-0.1.99/template_generator/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/template_generator/convertor/of_to_skymedia.py` & `p-template-generator-0.1.99/template_generator/convertor/of_to_skymedia.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/template_generator/ffmpeg.py` & `p-template-generator-0.1.99/template_generator/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/template_generator/main.py` & `p-template-generator-0.1.99/template_generator/main.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/template_generator/server_generator.py` & `p-template-generator-0.1.99/template_generator/server_generator.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/template_generator/template.py` & `p-template-generator-0.1.99/template_generator/template.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/template_generator/template_service.py` & `p-template-generator-0.1.99/template_generator/template_service.py`

 * *Files identical despite different names*

### Comparing `p-template-generator-0.1.98/template_generator/template_test.py` & `p-template-generator-0.1.99/template_generator/template_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,17 @@
             output_height = 100
             fn_name = "aicamera"
             params = {"batch_count":1,"batch_size":1,"cfg_scale":7,"creative_strength":1,"denoising_strength":1,"era":"spaceSuit","face_index":1,"fn_name":"aicamera","func":"d849eff2cfb2d09a0bb7ae573e69b1cc.png","height":1536,"musicUrl":"","negative_prompt":"","package_url":"https://m-beta-yesdesktop.2tianxin.com/upload/beta/undefined/6079/2763/607947D9CFD52763.zip","prompt":"","restore_faces":True,"sampler_index":"DPM++ SDE Karras","scratch":1,"seed":-1,"steps":25,"text_mark_url":"","type":"image","user_file_name":"d59e9302-f17f-4468-aa23-5b3fd3d44685.png","user_url":"","width":1152}
             server_generator.MecordAIGC().testTask(378 , inputs, fn_name, params, output_width, output_height)
             print("pushed one!")
         except:
             print("")
+
+# server_generator.MecordAIGC().testTask(386 , [], "test fnname", {}, 100, 100)
+            
 # testAigc(1)
 # def testToon():
 #     try:
 #         inputs = []
 #         output_width = 100
 #         output_height = 100
 #         fn_name = "Toon"
```

### Comparing `p-template-generator-0.1.98/template_generator/test/tp_2023112102.zip.py` & `p-template-generator-0.1.99/template_generator/test/tp_2023112102.zip.py`

 * *Files identical despite different names*

