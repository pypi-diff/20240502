# Comparing `tmp/python_gemini_api-2.4.8.tar.gz` & `tmp/python_gemini_api-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_gemini_api-2.4.8.tar", last modified: Sun Apr 28 14:01:14 2024, max compression
+gzip compressed data, was "python_gemini_api-2.4.9.tar", last modified: Mon Apr 29 07:34:40 2024, max compression
```

## Comparing `python_gemini_api-2.4.8.tar` & `python_gemini_api-2.4.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.342026 python_gemini_api-2.4.8/
--rw-rw-rw-   0        0        0     1097 2024-04-24 10:59:38.000000 python_gemini_api-2.4.8/LICENSE
--rw-rw-rw-   0        0        0    37858 2024-04-28 14:01:14.340018 python_gemini_api-2.4.8/PKG-INFO
--rw-rw-rw-   0        0        0    36531 2024-04-28 14:00:17.000000 python_gemini_api-2.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.288352 python_gemini_api-2.4.8/gemini/
--rw-rw-rw-   0        0        0     1511 2024-04-28 14:00:46.000000 python_gemini_api-2.4.8/gemini/__init__.py
--rw-rw-rw-   0        0        0    15168 2024-04-28 13:24:37.000000 python_gemini_api-2.4.8/gemini/async_client.py
--rw-rw-rw-   0        0        0    19528 2024-04-28 13:24:49.000000 python_gemini_api-2.4.8/gemini/client.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.289357 python_gemini_api-2.4.8/gemini/src/
--rw-rw-rw-   0        0        0        0 2024-03-05 10:25:37.000000 python_gemini_api-2.4.8/gemini/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.293360 python_gemini_api-2.4.8/gemini/src/extensions/
--rw-rw-rw-   0        0        0       40 2024-03-16 06:40:55.000000 python_gemini_api-2.4.8/gemini/src/extensions/__init__.py
--rw-rw-rw-   0        0        0      622 2024-03-18 04:30:10.000000 python_gemini_api-2.4.8/gemini/src/extensions/replit.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.301358 python_gemini_api-2.4.8/gemini/src/misc/
--rw-rw-rw-   0        0        0      265 2024-04-17 09:46:31.000000 python_gemini_api-2.4.8/gemini/src/misc/__init__.py
--rw-rw-rw-   0        0        0     9279 2024-04-05 10:13:11.000000 python_gemini_api-2.4.8/gemini/src/misc/constants.py
--rw-rw-rw-   0        0        0     3063 2024-03-18 04:29:01.000000 python_gemini_api-2.4.8/gemini/src/misc/decorator.py
--rw-rw-rw-   0        0        0     2421 2024-04-20 13:54:53.000000 python_gemini_api-2.4.8/gemini/src/misc/exceptions.py
--rw-rw-rw-   0        0        0     4487 2024-04-17 09:46:59.000000 python_gemini_api-2.4.8/gemini/src/misc/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.307601 python_gemini_api-2.4.8/gemini/src/model/
--rw-rw-rw-   0        0        0       88 2024-03-16 06:40:55.000000 python_gemini_api-2.4.8/gemini/src/model/__init__.py
--rw-rw-rw-   0        0        0     9159 2024-04-28 13:59:51.000000 python_gemini_api-2.4.8/gemini/src/model/image.py
--rw-rw-rw-   0        0        0     1858 2024-03-31 11:20:09.000000 python_gemini_api-2.4.8/gemini/src/model/output.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.314139 python_gemini_api-2.4.8/gemini/src/model/parser/
--rw-rw-rw-   0        0        0      130 2024-03-17 09:52:54.000000 python_gemini_api-2.4.8/gemini/src/model/parser/__init__.py
--rw-rw-rw-   0        0        0     1490 2024-03-05 10:15:40.000000 python_gemini_api-2.4.8/gemini/src/model/parser/base.py
--rw-rw-rw-   0        0        0     5433 2024-03-31 11:20:09.000000 python_gemini_api-2.4.8/gemini/src/model/parser/custom_parser.py
--rw-rw-rw-   0        0        0     7692 2024-03-31 11:20:09.000000 python_gemini_api-2.4.8/gemini/src/model/parser/response_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.316139 python_gemini_api-2.4.8/gemini/src/modules/
--rw-rw-rw-   0        0        0        0 2024-03-29 00:25:32.000000 python_gemini_api-2.4.8/gemini/src/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.322616 python_gemini_api-2.4.8/gemini/src/modules/openrouter/
--rw-rw-rw-   0        0        0      102 2024-04-21 13:59:49.000000 python_gemini_api-2.4.8/gemini/src/modules/openrouter/__init__.py
--rw-rw-rw-   0        0        0     3048 2024-04-27 13:13:20.000000 python_gemini_api-2.4.8/gemini/src/modules/openrouter/async_client.py
--rw-rw-rw-   0        0        0     4753 2024-04-24 12:56:08.000000 python_gemini_api-2.4.8/gemini/src/modules/openrouter/client.py
--rw-rw-rw-   0        0        0      505 2024-04-24 13:06:12.000000 python_gemini_api-2.4.8/gemini/src/modules/openrouter/const.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.326744 python_gemini_api-2.4.8/gemini/src/modules/voice/
--rw-rw-rw-   0        0        0       88 2024-03-18 04:18:39.000000 python_gemini_api-2.4.8/gemini/src/modules/voice/__init__.py
--rw-rw-rw-   0        0        0     2441 2024-03-18 04:18:26.000000 python_gemini_api-2.4.8/gemini/src/modules/voice/google.py
--rw-rw-rw-   0        0        0     3144 2024-03-17 14:01:32.000000 python_gemini_api-2.4.8/gemini/src/modules/voice/openai.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:01:14.337736 python_gemini_api-2.4.8/python_gemini_api.egg-info/
--rw-rw-rw-   0        0        0    37858 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-28 14:01:14.000000 python_gemini_api-2.4.8/python_gemini_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 14:01:14.342026 python_gemini_api-2.4.8/setup.cfg
--rw-rw-rw-   0        0        0     2204 2024-04-27 13:14:03.000000 python_gemini_api-2.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.919821 python_gemini_api-2.4.9/
+-rw-rw-rw-   0        0        0     1097 2024-04-24 10:59:38.000000 python_gemini_api-2.4.9/LICENSE
+-rw-rw-rw-   0        0        0    37611 2024-04-29 07:34:40.917809 python_gemini_api-2.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0    36284 2024-04-29 07:32:03.000000 python_gemini_api-2.4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.869270 python_gemini_api-2.4.9/gemini/
+-rw-rw-rw-   0        0        0     1511 2024-04-29 07:34:16.000000 python_gemini_api-2.4.9/gemini/__init__.py
+-rw-rw-rw-   0        0        0    15168 2024-04-28 13:24:37.000000 python_gemini_api-2.4.9/gemini/async_client.py
+-rw-rw-rw-   0        0        0    19528 2024-04-28 13:24:49.000000 python_gemini_api-2.4.9/gemini/client.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.870693 python_gemini_api-2.4.9/gemini/src/
+-rw-rw-rw-   0        0        0        0 2024-03-05 10:25:37.000000 python_gemini_api-2.4.9/gemini/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.873267 python_gemini_api-2.4.9/gemini/src/extensions/
+-rw-rw-rw-   0        0        0       40 2024-03-16 06:40:55.000000 python_gemini_api-2.4.9/gemini/src/extensions/__init__.py
+-rw-rw-rw-   0        0        0      622 2024-03-18 04:30:10.000000 python_gemini_api-2.4.9/gemini/src/extensions/replit.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.880888 python_gemini_api-2.4.9/gemini/src/misc/
+-rw-rw-rw-   0        0        0      265 2024-04-17 09:46:31.000000 python_gemini_api-2.4.9/gemini/src/misc/__init__.py
+-rw-rw-rw-   0        0        0     9279 2024-04-05 10:13:11.000000 python_gemini_api-2.4.9/gemini/src/misc/constants.py
+-rw-rw-rw-   0        0        0     3063 2024-03-18 04:29:01.000000 python_gemini_api-2.4.9/gemini/src/misc/decorator.py
+-rw-rw-rw-   0        0        0     2421 2024-04-20 13:54:53.000000 python_gemini_api-2.4.9/gemini/src/misc/exceptions.py
+-rw-rw-rw-   0        0        0     4575 2024-04-28 14:17:22.000000 python_gemini_api-2.4.9/gemini/src/misc/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.886345 python_gemini_api-2.4.9/gemini/src/model/
+-rw-rw-rw-   0        0        0       88 2024-03-16 06:40:55.000000 python_gemini_api-2.4.9/gemini/src/model/__init__.py
+-rw-rw-rw-   0        0        0     8609 2024-04-29 07:31:12.000000 python_gemini_api-2.4.9/gemini/src/model/image.py
+-rw-rw-rw-   0        0        0     1858 2024-04-29 06:45:23.000000 python_gemini_api-2.4.9/gemini/src/model/output.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.893121 python_gemini_api-2.4.9/gemini/src/model/parser/
+-rw-rw-rw-   0        0        0      130 2024-03-17 09:52:54.000000 python_gemini_api-2.4.9/gemini/src/model/parser/__init__.py
+-rw-rw-rw-   0        0        0     1490 2024-03-05 10:15:40.000000 python_gemini_api-2.4.9/gemini/src/model/parser/base.py
+-rw-rw-rw-   0        0        0     5433 2024-03-31 11:20:09.000000 python_gemini_api-2.4.9/gemini/src/model/parser/custom_parser.py
+-rw-rw-rw-   0        0        0     7692 2024-03-31 11:20:09.000000 python_gemini_api-2.4.9/gemini/src/model/parser/response_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.894120 python_gemini_api-2.4.9/gemini/src/modules/
+-rw-rw-rw-   0        0        0        0 2024-03-29 00:25:32.000000 python_gemini_api-2.4.9/gemini/src/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.900563 python_gemini_api-2.4.9/gemini/src/modules/openrouter/
+-rw-rw-rw-   0        0        0      102 2024-04-21 13:59:49.000000 python_gemini_api-2.4.9/gemini/src/modules/openrouter/__init__.py
+-rw-rw-rw-   0        0        0     3048 2024-04-27 13:13:20.000000 python_gemini_api-2.4.9/gemini/src/modules/openrouter/async_client.py
+-rw-rw-rw-   0        0        0     4753 2024-04-24 12:56:08.000000 python_gemini_api-2.4.9/gemini/src/modules/openrouter/client.py
+-rw-rw-rw-   0        0        0      505 2024-04-24 13:06:12.000000 python_gemini_api-2.4.9/gemini/src/modules/openrouter/const.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.904708 python_gemini_api-2.4.9/gemini/src/modules/voice/
+-rw-rw-rw-   0        0        0       88 2024-03-18 04:18:39.000000 python_gemini_api-2.4.9/gemini/src/modules/voice/__init__.py
+-rw-rw-rw-   0        0        0     2441 2024-03-18 04:18:26.000000 python_gemini_api-2.4.9/gemini/src/modules/voice/google.py
+-rw-rw-rw-   0        0        0     3144 2024-03-17 14:01:32.000000 python_gemini_api-2.4.9/gemini/src/modules/voice/openai.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:34:40.916810 python_gemini_api-2.4.9/python_gemini_api.egg-info/
+-rw-rw-rw-   0        0        0    37611 2024-04-29 07:34:40.000000 python_gemini_api-2.4.9/python_gemini_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2024-04-29 07:34:40.000000 python_gemini_api-2.4.9/python_gemini_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:34:40.000000 python_gemini_api-2.4.9/python_gemini_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-29 07:34:40.000000 python_gemini_api-2.4.9/python_gemini_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2024-04-29 07:34:40.000000 python_gemini_api-2.4.9/python_gemini_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-29 07:34:40.000000 python_gemini_api-2.4.9/python_gemini_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:34:40.919821 python_gemini_api-2.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     2204 2024-04-27 13:14:03.000000 python_gemini_api-2.4.9/setup.py
```

### Comparing `python_gemini_api-2.4.8/LICENSE` & `python_gemini_api-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/PKG-INFO` & `python_gemini_api-2.4.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gemini-api
-Version: 2.4.8
+Version: 2.4.9
 Summary: The python package that returns Response of Google Gemini through API.
 Home-page: https://github.com/dsdanielpark/Gemini-API
 Author: Daniel Park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -329,20 +329,19 @@
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
-
 generated_images = response.generated_images # Check generated images [Dict]
 
-await image_client.save(generated_images, "save_dir", cookies=cookies)
-# image_data_dict = await image_client.fetch_images_dict(generated_images, cookies=cookies)
-# await image_client.save_images(image_data_dict, "save_dir")
+await image_client.save(generated_images, "output")
+# image_data_dict = await image_client.fetch_images_dict(generated_images)
+# await image_client.save_images(image_data_dict, "output")
 ```
 
 
 <details><summary>Further</summary>
 
 *Display images in IPython*
   You can display the image or transmit it to another application in byte format.
@@ -351,16 +350,15 @@
   import io
   from gemini import Gemini, GeminiImage
   from IPython.display import display, Image
   
   cookies = {}
   client = Gemini(cookies=cookies)
   image_client = GeminiImage(cookies=cookies)
-
-  bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
+  bytes_images_dict = image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict
   
   for image_name, image_bytes in bytes_images_dict.items():
       print(image_name)
       image = Image(data=image_bytes)
       display(image)
   ```
 
@@ -372,60 +370,60 @@
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
-image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies) # Save default folder is `cached`
+image_client.save_sync(generated_images, save_path="output")
 
 # You can use byte type image dict for printing images as follow:
-# bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
-# image_client.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+# bytes_images_dict = image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, path="output") # Save to dir
 ```
 
 *Async downloader wrapper*
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    await image_client.save(generated_imagse, save_path=save_path, cookies=cookies)
+async def save_generated_imagse(generated_imagse, save_path="output"):
+    await image_client.save(generated_imagse, save_path=save_path)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  
-    asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_generated_imagse(generated_imagse, save_path="output"))
 ```
 
 `GeminiImage.save` method logic
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    image_data_dict = await image_client.fetch_images_dict(generated_imagse, cookies=cookies)  # Get bytes images dict asynchronously
+async def save_generated_imagse(generated_imagse, save_path="output"):
+    image_data_dict = await image_client.fetch_images_dict(generated_imagse)  # Get bytes images dict asynchronously
     await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  # Check response images [Dict]
-    asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_generated_imagse(generated_imagse, save_path="output"))
 ```
 
 </details>
 
 > [!NOTE]
 > Use GeminiImage for image processing. `web_images` works without cookies, but for images like `generated_image` from Gemini, pass cookies. Cookies are needed to download images from Google's storage. Check the response or use existing cookies variable.
 
@@ -440,20 +438,19 @@
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
-
 response_images = response.web_images # Check generated images [Dict]
 
-await image_client.save(response_images, "save_dir")
+await image_client.save(response_images, "output")
 # image_data_dict = await image_client.fetch_images_dict(response_images)
-# await image_client.save_images(image_data_dict, "save_dir")
+# await image_client.save_images(image_data_dict, "output")
 ```
 
 <details><summary>Further</summary>
 
 
 *Sync downloader*
 ```python
@@ -462,58 +459,58 @@
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Please recommend a travel itinerary for Seoul.")
 response_images = response.web_images # Check response images [Dict]
 
-GeminiImage.save_sync(response_images, save_path="save_dir")
+GeminiImage.save_sync(response_images, save_path="output")
 
 # You can use byte type image dict as follow:
-# bytes_images_dict = image_client.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
+# bytes_images_dict = image_client.fetch_bytes_sync(response_images) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, save_path="output") # Save to path
 ```
 
 *Async downloader wrapper*
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_response_web_imagse(response_images, save_path="save_dir"):
+async def save_response_web_imagse(response_images, save_path="output"):
     await image_client.save(response_images, save_path=save_path)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     response_images = response.web_images  
-    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
+    asyncio.run(save_response_web_imagse(response_images, save_path="output"))
 ```
 
 `GeminiImage.save` method logic
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
-    image_data_dict = await image_client.fetch_images_dict(response_images, cookies=cookies)  # Get bytes images dict asynchronously
+async def save_response_web_imagse(response_images, save_path="output"):
+    image_data_dict = await image_client.fetch_images_dict(response_images)  # Get bytes images dict asynchronously
     await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     response_images = response.web_images  # Check response images [Dict]
-    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_response_web_imagse(response_images, save_path="output"))
 ```
 
 </details>
 
 <br>
 
 ### # 07. Generate content from images
@@ -773,16 +770,22 @@
 First review [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://aistudio.google.com/) before using this package.
 You can find most help on the [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues) pages. 
             
 ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues)
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated. Frequent errors may occur due to changes in Google's service API interface. Both [Issue reports](https://github.com/dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome. We strive to maintain an active and courteous open community.
 
 ## Contributors
+
+<p align="center"><i>dig the well before you are thirsty.</i></p>
+
+
 We would like to express our sincere gratitude to all the contributors. 
 
+
+
 This package aims to re-implement the functionality of the [Bard API](https://github.com/dsdanielpark/Bard-API/), which has been archived for the contributions of the beloved open-source community, despite Gemini's official API already being available.
 
 Contributors to the [Bard API](https://github.com/dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/Gemini-API/).
 
 <a href="https://github.com/dsdanielpark/Bard_API/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=dsdanielpark/Bard_API" />
 </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.8 Summary: The
+Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.9 Summary: The
 python package that returns Response of Google Gemini through API. Home-page:
 https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
 Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -188,89 +188,85 @@
 "Hello, Gemini. What's the weather like in Seoul today?" response =
 client.generate_content(prompt) print(response.text) ```
 ### # 05. Image generation Returns images generated by Gemini. *Async
 downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
 client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
 response = client.generate_content("Create illustrations of Seoul, South
 Korea.") generated_images = response.generated_images # Check generated images
-[Dict] await image_client.save(generated_images, "save_dir", cookies=cookies) #
-image_data_dict = await image_client.fetch_images_dict(generated_images,
-cookies=cookies) # await image_client.save_images(image_data_dict, "save_dir")
-``` Further *Display images in IPython* You can display the image or transmit
-it to another application in byte format. ```python import io from gemini
-import Gemini, GeminiImage from IPython.display import display, Image cookies =
-{} client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
-bytes_images_dict = image_client.fetch_images_dict_sync(generated_images,
-cookies) # Get bytes images dict for image_name, image_bytes in
-bytes_images_dict.items(): print(image_name) image = Image(data=image_bytes)
-display(image) ``` *Sync downloader* ```python from gemini import Gemini,
-GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client =
-GeminiImage(cookies=cookies) response = client.generate_content("Create
-illustrations of Seoul, South Korea.") generated_images =
-response.generated_images # Check generated images [Dict]
-image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies)
-# Save default folder is `cached` # You can use byte type image dict for
-printing images as follow: # bytes_images_dict =
-image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
-bytes images dict # image_client.save_images_sync(bytes_images_dict,
-path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
-```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
-client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
-async def save_generated_imagse(generated_imagse, save_path="save_dir",
-cookies=cookies): await image_client.save(generated_imagse,
-save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+[Dict] await image_client.save(generated_images, "output") # image_data_dict =
+await image_client.fetch_images_dict(generated_images) # await
+image_client.save_images(image_data_dict, "output") ``` Further *Display images
+in IPython* You can display the image or transmit it to another application in
+byte format. ```python import io from gemini import Gemini, GeminiImage from
+IPython.display import display, Image cookies = {} client = Gemini
+(cookies=cookies) image_client = GeminiImage(cookies=cookies) bytes_images_dict
+= image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict
+for image_name, image_bytes in bytes_images_dict.items(): print(image_name)
+image = Image(data=image_bytes) display(image) ``` *Sync downloader* ```python
+from gemini import Gemini, GeminiImage cookies = {} client = Gemini
+(cookies=cookies) image_client = GeminiImage(cookies=cookies) response =
+client.generate_content("Create illustrations of Seoul, South Korea.")
+generated_images = response.generated_images # Check generated images [Dict]
+image_client.save_sync(generated_images, save_path="output") # You can use byte
+type image dict for printing images as follow: # bytes_images_dict =
+image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict #
+image_client.save_images_sync(bytes_images_dict, path="output") # Save to dir
+``` *Async downloader wrapper* ```python import asyncio from gemini import
+Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
+= GeminiImage(cookies=cookies) async def save_generated_imagse
+(generated_imagse, save_path="output"): await image_client.save
+(generated_imagse, save_path=save_path) # Run the async function if __name__ ==
 "__main__": cookies = {"key" : "value"} generated_imagse =
 response.generated_imagse asyncio.run(save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies)) ``` `GeminiImage.save` method logic
-```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
-client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
-async def save_generated_imagse(generated_imagse, save_path="save_dir",
-cookies=cookies): image_data_dict = await image_client.fetch_images_dict
-(generated_imagse, cookies=cookies) # Get bytes images dict asynchronously
-await image_client.save_images(image_data_dict, save_path=save_path) # Run the
-async function if __name__ == "__main__": cookies = {"key" : "value"}
-generated_imagse = response.generated_imagse # Check response images [Dict]
-asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir",
-cookies=cookies)) ``` > [!NOTE] > Use GeminiImage for image processing.
-`web_images` works without cookies, but for images like `generated_image` from
-Gemini, pass cookies. Cookies are needed to download images from Google's
-storage. Check the response or use existing cookies variable.
+save_path="output")) ``` `GeminiImage.save` method logic ```python import
+asyncio from gemini import Gemini, GeminiImage cookies = {} client = Gemini
+(cookies=cookies) image_client = GeminiImage(cookies=cookies) async def
+save_generated_imagse(generated_imagse, save_path="output"): image_data_dict =
+await image_client.fetch_images_dict(generated_imagse) # Get bytes images dict
+asynchronously await image_client.save_images(image_data_dict,
+save_path=save_path) # Run the async function if __name__ == "__main__":
+cookies = {"key" : "value"} generated_imagse = response.generated_imagse #
+Check response images [Dict] asyncio.run(save_generated_imagse
+(generated_imagse, save_path="output")) ``` > [!NOTE] > Use GeminiImage for
+image processing. `web_images` works without cookies, but for images like
+`generated_image` from Gemini, pass cookies. Cookies are needed to download
+images from Google's storage. Check the response or use existing cookies
+variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
 Gemini. *Async downloader* ```python from gemini import Gemini, GeminiImage
 cookies = {} client = Gemini(cookies=cookies) image_client = GeminiImage
 (cookies=cookies) response = client.generate_content("Create illustrations of
 Seoul, South Korea.") response_images = response.web_images # Check generated
-images [Dict] await image_client.save(response_images, "save_dir") #
+images [Dict] await image_client.save(response_images, "output") #
 image_data_dict = await image_client.fetch_images_dict(response_images) # await
-image_client.save_images(image_data_dict, "save_dir") ``` Further *Sync
+image_client.save_images(image_data_dict, "output") ``` Further *Sync
 downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
 client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
 response = client.generate_content("Please recommend a travel itinerary for
 Seoul.") response_images = response.web_images # Check response images [Dict]
-GeminiImage.save_sync(response_images, save_path="save_dir") # You can use byte
+GeminiImage.save_sync(response_images, save_path="output") # You can use byte
 type image dict as follow: # bytes_images_dict = image_client.fetch_bytes_sync
-(response_images, cookies) # Get bytes images dict #
-image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to
-path ``` *Async downloader wrapper* ```python import asyncio from gemini import
-Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
-= GeminiImage(cookies=cookies) async def save_response_web_imagse
-(response_images, save_path="save_dir"): await image_client.save
-(response_images, save_path=save_path) # Run the async function if __name__ ==
-"__main__": cookies = {"key" : "value"} response_images = response.web_images
-asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
-``` `GeminiImage.save` method logic ```python import asyncio from gemini import
+(response_images) # Get bytes images dict # image_client.save_images_sync
+(bytes_images_dict, save_path="output") # Save to path ``` *Async downloader
+wrapper* ```python import asyncio from gemini import Gemini, GeminiImage
+cookies = {} client = Gemini(cookies=cookies) image_client = GeminiImage
+(cookies=cookies) async def save_response_web_imagse(response_images,
+save_path="output"): await image_client.save(response_images,
+save_path=save_path) # Run the async function if __name__ == "__main__":
+cookies = {"key" : "value"} response_images = response.web_images asyncio.run
+(save_response_web_imagse(response_images, save_path="output")) ```
+`GeminiImage.save` method logic ```python import asyncio from gemini import
 Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
 = GeminiImage(cookies=cookies) async def save_response_web_imagse
-(response_images, save_path="save_dir", cookies=cookies): image_data_dict =
-await image_client.fetch_images_dict(response_images, cookies=cookies) # Get
-bytes images dict asynchronously await image_client.save_images
-(image_data_dict, save_path=save_path) # Run the async function if __name__ ==
-"__main__": response_images = response.web_images # Check response images
-[Dict] asyncio.run(save_response_web_imagse(response_images,
-save_path="save_dir", cookies=cookies)) ```
+(response_images, save_path="output"): image_data_dict = await
+image_client.fetch_images_dict(response_images) # Get bytes images dict
+asynchronously await image_client.save_images(image_data_dict,
+save_path=save_path) # Run the async function if __name__ == "__main__":
+response_images = response.web_images # Check response images [Dict]
+asyncio.run(save_response_web_imagse(response_images, save_path="output")) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
 image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. # Image file
 path or Byte-formatted image array response = client.generate_content("What
 does the text in this image say?", image=image) response.response_dict ```
 ### # 08. Generate content using Google Services To begin, you must link Google
 Workspace to activate this extension via the [Gemini web extension](https://
@@ -429,14 +425,15 @@
 pages. ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues) Sincerely
 grateful for any reports on new features or bugs. Your valuable feedback on the
 code is highly appreciated. Frequent errors may occur due to changes in
 Google's service API interface. Both [Issue reports](https://github.com/
 dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/
 dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome.
 We strive to maintain an active and courteous open community. ## Contributors
+                     dig the well before you are thirsty.
 We would like to express our sincere gratitude to all the contributors. This
 package aims to re-implement the functionality of the [Bard API](https://
 github.com/dsdanielpark/Bard-API/), which has been archived for the
 contributions of the beloved open-source community, despite Gemini's official
 API already being available. Contributors to the [Bard API](https://github.com/
 dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/
 Gemini-API/). _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_s_d_a_n_i_e_l_p_a_r_k_/_B_a_r_d___A_P_I_]
```

### Comparing `python_gemini_api-2.4.8/README.md` & `python_gemini_api-2.4.9/python_gemini_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: python-gemini-api
+Version: 2.4.9
+Summary: The python package that returns Response of Google Gemini through API.
+Home-page: https://github.com/dsdanielpark/Gemini-API
+Author: Daniel Park
+Author-email: parkminwoo1991@gmail.com
+Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: httpx[http2]>=0.20.0
+Requires-Dist: requests
+Requires-Dist: browser_cookie3
+Requires-Dist: loguru
+Requires-Dist: pydantic
+Requires-Dist: aiohttp
+Provides-Extra: voice
+Requires-Dist: gTTS; extra == "voice"
+Requires-Dist: SpeechRecognition; extra == "voice"
+Requires-Dist: openai; extra == "voice"
+Requires-Dist: anthropic; extra == "voice"
+
 
 # <img src="https://www.gstatic.com/lamda/images/favicon_v1_150160cddff7f294ce30.svg" width="35px" alt="Gemini Icon" /> Gemini API  <a href="https://pypi.org/project/python-gemini-api/"> <img alt="PyPI" src="https://img.shields.io/pypi/v/python-gemini-api?color=black"></a>
 
 
 <p align="right">
     <a href="https://github.com/dsdanielpark/Gemini-API"><img alt="pip download" src="https://img.shields.io/badge/pip_install-python_gemini_api-black"></a> 
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
@@ -296,20 +329,19 @@
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
-
 generated_images = response.generated_images # Check generated images [Dict]
 
-await image_client.save(generated_images, "save_dir", cookies=cookies)
-# image_data_dict = await image_client.fetch_images_dict(generated_images, cookies=cookies)
-# await image_client.save_images(image_data_dict, "save_dir")
+await image_client.save(generated_images, "output")
+# image_data_dict = await image_client.fetch_images_dict(generated_images)
+# await image_client.save_images(image_data_dict, "output")
 ```
 
 
 <details><summary>Further</summary>
 
 *Display images in IPython*
   You can display the image or transmit it to another application in byte format.
@@ -318,16 +350,15 @@
   import io
   from gemini import Gemini, GeminiImage
   from IPython.display import display, Image
   
   cookies = {}
   client = Gemini(cookies=cookies)
   image_client = GeminiImage(cookies=cookies)
-
-  bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
+  bytes_images_dict = image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict
   
   for image_name, image_bytes in bytes_images_dict.items():
       print(image_name)
       image = Image(data=image_bytes)
       display(image)
   ```
 
@@ -339,60 +370,60 @@
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
-image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies) # Save default folder is `cached`
+image_client.save_sync(generated_images, save_path="output")
 
 # You can use byte type image dict for printing images as follow:
-# bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
-# image_client.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+# bytes_images_dict = image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, path="output") # Save to dir
 ```
 
 *Async downloader wrapper*
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    await image_client.save(generated_imagse, save_path=save_path, cookies=cookies)
+async def save_generated_imagse(generated_imagse, save_path="output"):
+    await image_client.save(generated_imagse, save_path=save_path)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  
-    asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_generated_imagse(generated_imagse, save_path="output"))
 ```
 
 `GeminiImage.save` method logic
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    image_data_dict = await image_client.fetch_images_dict(generated_imagse, cookies=cookies)  # Get bytes images dict asynchronously
+async def save_generated_imagse(generated_imagse, save_path="output"):
+    image_data_dict = await image_client.fetch_images_dict(generated_imagse)  # Get bytes images dict asynchronously
     await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  # Check response images [Dict]
-    asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_generated_imagse(generated_imagse, save_path="output"))
 ```
 
 </details>
 
 > [!NOTE]
 > Use GeminiImage for image processing. `web_images` works without cookies, but for images like `generated_image` from Gemini, pass cookies. Cookies are needed to download images from Google's storage. Check the response or use existing cookies variable.
 
@@ -407,20 +438,19 @@
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
-
 response_images = response.web_images # Check generated images [Dict]
 
-await image_client.save(response_images, "save_dir")
+await image_client.save(response_images, "output")
 # image_data_dict = await image_client.fetch_images_dict(response_images)
-# await image_client.save_images(image_data_dict, "save_dir")
+# await image_client.save_images(image_data_dict, "output")
 ```
 
 <details><summary>Further</summary>
 
 
 *Sync downloader*
 ```python
@@ -429,58 +459,58 @@
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Please recommend a travel itinerary for Seoul.")
 response_images = response.web_images # Check response images [Dict]
 
-GeminiImage.save_sync(response_images, save_path="save_dir")
+GeminiImage.save_sync(response_images, save_path="output")
 
 # You can use byte type image dict as follow:
-# bytes_images_dict = image_client.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
+# bytes_images_dict = image_client.fetch_bytes_sync(response_images) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, save_path="output") # Save to path
 ```
 
 *Async downloader wrapper*
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_response_web_imagse(response_images, save_path="save_dir"):
+async def save_response_web_imagse(response_images, save_path="output"):
     await image_client.save(response_images, save_path=save_path)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     response_images = response.web_images  
-    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
+    asyncio.run(save_response_web_imagse(response_images, save_path="output"))
 ```
 
 `GeminiImage.save` method logic
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
-    image_data_dict = await image_client.fetch_images_dict(response_images, cookies=cookies)  # Get bytes images dict asynchronously
+async def save_response_web_imagse(response_images, save_path="output"):
+    image_data_dict = await image_client.fetch_images_dict(response_images)  # Get bytes images dict asynchronously
     await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     response_images = response.web_images  # Check response images [Dict]
-    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_response_web_imagse(response_images, save_path="output"))
 ```
 
 </details>
 
 <br>
 
 ### # 07. Generate content from images
@@ -740,16 +770,22 @@
 First review [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://aistudio.google.com/) before using this package.
 You can find most help on the [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues) pages. 
             
 ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues)
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated. Frequent errors may occur due to changes in Google's service API interface. Both [Issue reports](https://github.com/dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome. We strive to maintain an active and courteous open community.
 
 ## Contributors
+
+<p align="center"><i>dig the well before you are thirsty.</i></p>
+
+
 We would like to express our sincere gratitude to all the contributors. 
 
+
+
 This package aims to re-implement the functionality of the [Bard API](https://github.com/dsdanielpark/Bard-API/), which has been archived for the contributions of the beloved open-source community, despite Gemini's official API already being available.
 
 Contributors to the [Bard API](https://github.com/dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/Gemini-API/).
 
 <a href="https://github.com/dsdanielpark/Bard_API/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=dsdanielpark/Bard_API" />
 </a>
```

#### html2text {}

```diff
@@ -1,8 +1,25 @@
-# [Gemini Icon]Gemini API_[_P_y_P_I_]
+Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.9 Summary: The
+python package that returns Response of Google Gemini through API. Home-page:
+https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
+parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
+Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
+2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
+Natural Language :: English Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
+Approved :: MIT License Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Python: >=3.9 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: httpx[http2]>=0.20.0 Requires-
+Dist: requests Requires-Dist: browser_cookie3 Requires-Dist: loguru Requires-
+Dist: pydantic Requires-Dist: aiohttp Provides-Extra: voice Requires-Dist:
+gTTS; extra == "voice" Requires-Dist: SpeechRecognition; extra == "voice"
+Requires-Dist: openai; extra == "voice" Requires-Dist: anthropic; extra ==
+"voice" # [Gemini Icon]Gemini API_[_P_y_P_I_]
   _[_p_i_p_ _d_o_w_n_l_o_a_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
                 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_d_s_d_a_n_i_e_l_p_a_r_k_%_2_F_G_e_m_i_n_i_-
 _A_P_I_&_c_o_u_n_t___b_g_=_%_2_3_0_0_0_0_0_0_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_v_i_e_w_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
                                                                     _[_D_o_w_n_l_o_a_d_s_]
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-
 ba79-d9f89b637324 An **unofficial* Python wrapper, [python-gemini-api](https://
 pypi.org/project/python-gemini-api/), is available for users facing frequent
@@ -171,89 +188,85 @@
 "Hello, Gemini. What's the weather like in Seoul today?" response =
 client.generate_content(prompt) print(response.text) ```
 ### # 05. Image generation Returns images generated by Gemini. *Async
 downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
 client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
 response = client.generate_content("Create illustrations of Seoul, South
 Korea.") generated_images = response.generated_images # Check generated images
-[Dict] await image_client.save(generated_images, "save_dir", cookies=cookies) #
-image_data_dict = await image_client.fetch_images_dict(generated_images,
-cookies=cookies) # await image_client.save_images(image_data_dict, "save_dir")
-``` Further *Display images in IPython* You can display the image or transmit
-it to another application in byte format. ```python import io from gemini
-import Gemini, GeminiImage from IPython.display import display, Image cookies =
-{} client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
-bytes_images_dict = image_client.fetch_images_dict_sync(generated_images,
-cookies) # Get bytes images dict for image_name, image_bytes in
-bytes_images_dict.items(): print(image_name) image = Image(data=image_bytes)
-display(image) ``` *Sync downloader* ```python from gemini import Gemini,
-GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client =
-GeminiImage(cookies=cookies) response = client.generate_content("Create
-illustrations of Seoul, South Korea.") generated_images =
-response.generated_images # Check generated images [Dict]
-image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies)
-# Save default folder is `cached` # You can use byte type image dict for
-printing images as follow: # bytes_images_dict =
-image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
-bytes images dict # image_client.save_images_sync(bytes_images_dict,
-path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
-```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
-client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
-async def save_generated_imagse(generated_imagse, save_path="save_dir",
-cookies=cookies): await image_client.save(generated_imagse,
-save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+[Dict] await image_client.save(generated_images, "output") # image_data_dict =
+await image_client.fetch_images_dict(generated_images) # await
+image_client.save_images(image_data_dict, "output") ``` Further *Display images
+in IPython* You can display the image or transmit it to another application in
+byte format. ```python import io from gemini import Gemini, GeminiImage from
+IPython.display import display, Image cookies = {} client = Gemini
+(cookies=cookies) image_client = GeminiImage(cookies=cookies) bytes_images_dict
+= image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict
+for image_name, image_bytes in bytes_images_dict.items(): print(image_name)
+image = Image(data=image_bytes) display(image) ``` *Sync downloader* ```python
+from gemini import Gemini, GeminiImage cookies = {} client = Gemini
+(cookies=cookies) image_client = GeminiImage(cookies=cookies) response =
+client.generate_content("Create illustrations of Seoul, South Korea.")
+generated_images = response.generated_images # Check generated images [Dict]
+image_client.save_sync(generated_images, save_path="output") # You can use byte
+type image dict for printing images as follow: # bytes_images_dict =
+image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict #
+image_client.save_images_sync(bytes_images_dict, path="output") # Save to dir
+``` *Async downloader wrapper* ```python import asyncio from gemini import
+Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
+= GeminiImage(cookies=cookies) async def save_generated_imagse
+(generated_imagse, save_path="output"): await image_client.save
+(generated_imagse, save_path=save_path) # Run the async function if __name__ ==
 "__main__": cookies = {"key" : "value"} generated_imagse =
 response.generated_imagse asyncio.run(save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies)) ``` `GeminiImage.save` method logic
-```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
-client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
-async def save_generated_imagse(generated_imagse, save_path="save_dir",
-cookies=cookies): image_data_dict = await image_client.fetch_images_dict
-(generated_imagse, cookies=cookies) # Get bytes images dict asynchronously
-await image_client.save_images(image_data_dict, save_path=save_path) # Run the
-async function if __name__ == "__main__": cookies = {"key" : "value"}
-generated_imagse = response.generated_imagse # Check response images [Dict]
-asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir",
-cookies=cookies)) ``` > [!NOTE] > Use GeminiImage for image processing.
-`web_images` works without cookies, but for images like `generated_image` from
-Gemini, pass cookies. Cookies are needed to download images from Google's
-storage. Check the response or use existing cookies variable.
+save_path="output")) ``` `GeminiImage.save` method logic ```python import
+asyncio from gemini import Gemini, GeminiImage cookies = {} client = Gemini
+(cookies=cookies) image_client = GeminiImage(cookies=cookies) async def
+save_generated_imagse(generated_imagse, save_path="output"): image_data_dict =
+await image_client.fetch_images_dict(generated_imagse) # Get bytes images dict
+asynchronously await image_client.save_images(image_data_dict,
+save_path=save_path) # Run the async function if __name__ == "__main__":
+cookies = {"key" : "value"} generated_imagse = response.generated_imagse #
+Check response images [Dict] asyncio.run(save_generated_imagse
+(generated_imagse, save_path="output")) ``` > [!NOTE] > Use GeminiImage for
+image processing. `web_images` works without cookies, but for images like
+`generated_image` from Gemini, pass cookies. Cookies are needed to download
+images from Google's storage. Check the response or use existing cookies
+variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
 Gemini. *Async downloader* ```python from gemini import Gemini, GeminiImage
 cookies = {} client = Gemini(cookies=cookies) image_client = GeminiImage
 (cookies=cookies) response = client.generate_content("Create illustrations of
 Seoul, South Korea.") response_images = response.web_images # Check generated
-images [Dict] await image_client.save(response_images, "save_dir") #
+images [Dict] await image_client.save(response_images, "output") #
 image_data_dict = await image_client.fetch_images_dict(response_images) # await
-image_client.save_images(image_data_dict, "save_dir") ``` Further *Sync
+image_client.save_images(image_data_dict, "output") ``` Further *Sync
 downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
 client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
 response = client.generate_content("Please recommend a travel itinerary for
 Seoul.") response_images = response.web_images # Check response images [Dict]
-GeminiImage.save_sync(response_images, save_path="save_dir") # You can use byte
+GeminiImage.save_sync(response_images, save_path="output") # You can use byte
 type image dict as follow: # bytes_images_dict = image_client.fetch_bytes_sync
-(response_images, cookies) # Get bytes images dict #
-image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to
-path ``` *Async downloader wrapper* ```python import asyncio from gemini import
-Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
-= GeminiImage(cookies=cookies) async def save_response_web_imagse
-(response_images, save_path="save_dir"): await image_client.save
-(response_images, save_path=save_path) # Run the async function if __name__ ==
-"__main__": cookies = {"key" : "value"} response_images = response.web_images
-asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
-``` `GeminiImage.save` method logic ```python import asyncio from gemini import
+(response_images) # Get bytes images dict # image_client.save_images_sync
+(bytes_images_dict, save_path="output") # Save to path ``` *Async downloader
+wrapper* ```python import asyncio from gemini import Gemini, GeminiImage
+cookies = {} client = Gemini(cookies=cookies) image_client = GeminiImage
+(cookies=cookies) async def save_response_web_imagse(response_images,
+save_path="output"): await image_client.save(response_images,
+save_path=save_path) # Run the async function if __name__ == "__main__":
+cookies = {"key" : "value"} response_images = response.web_images asyncio.run
+(save_response_web_imagse(response_images, save_path="output")) ```
+`GeminiImage.save` method logic ```python import asyncio from gemini import
 Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
 = GeminiImage(cookies=cookies) async def save_response_web_imagse
-(response_images, save_path="save_dir", cookies=cookies): image_data_dict =
-await image_client.fetch_images_dict(response_images, cookies=cookies) # Get
-bytes images dict asynchronously await image_client.save_images
-(image_data_dict, save_path=save_path) # Run the async function if __name__ ==
-"__main__": response_images = response.web_images # Check response images
-[Dict] asyncio.run(save_response_web_imagse(response_images,
-save_path="save_dir", cookies=cookies)) ```
+(response_images, save_path="output"): image_data_dict = await
+image_client.fetch_images_dict(response_images) # Get bytes images dict
+asynchronously await image_client.save_images(image_data_dict,
+save_path=save_path) # Run the async function if __name__ == "__main__":
+response_images = response.web_images # Check response images [Dict]
+asyncio.run(save_response_web_imagse(response_images, save_path="output")) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
 image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. # Image file
 path or Byte-formatted image array response = client.generate_content("What
 does the text in this image say?", image=image) response.response_dict ```
 ### # 08. Generate content using Google Services To begin, you must link Google
 Workspace to activate this extension via the [Gemini web extension](https://
@@ -412,14 +425,15 @@
 pages. ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues) Sincerely
 grateful for any reports on new features or bugs. Your valuable feedback on the
 code is highly appreciated. Frequent errors may occur due to changes in
 Google's service API interface. Both [Issue reports](https://github.com/
 dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/
 dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome.
 We strive to maintain an active and courteous open community. ## Contributors
+                     dig the well before you are thirsty.
 We would like to express our sincere gratitude to all the contributors. This
 package aims to re-implement the functionality of the [Bard API](https://
 github.com/dsdanielpark/Bard-API/), which has been archived for the
 contributions of the beloved open-source community, despite Gemini's official
 API already being available. Contributors to the [Bard API](https://github.com/
 dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/
 Gemini-API/). _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_s_d_a_n_i_e_l_p_a_r_k_/_B_a_r_d___A_P_I_]
```

### Comparing `python_gemini_api-2.4.8/gemini/__init__.py` & `python_gemini_api-2.4.9/gemini/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     from .src.modules.voice.google import google_tts, google_stt
     from .src.modules.voice.openai import openai_tts, openai_stt
 except ImportError as e:
     pass
 
 gemini_api_key = environ.get("GEMINI_COOKIES")
 
-__version__ = "2.4.8"
+__version__ = "2.4.9"
 __author__ = (
     "daniel park <parkminwoo1991@gmail.com>, antonio cheang <teapotv8@proton.me>, "
     "HanaokaYuzu, CBoYXD, veonua, thewh1teagle, jjkoh95, yihong0618, nishantchauhan949, MeemeeLab, kota113, "
     "sachnun, amit9021, zeelsheladiya, ayansengupta17, thecodekitchen, SalimLouDev, Qewertyy, "
     "senseibence, mirusu400, szv99, sudoAlireza"
 )
```

### Comparing `python_gemini_api-2.4.8/gemini/async_client.py` & `python_gemini_api-2.4.9/gemini/async_client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/client.py` & `python_gemini_api-2.4.9/gemini/client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/extensions/replit.py` & `python_gemini_api-2.4.9/gemini/src/extensions/replit.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/misc/constants.py` & `python_gemini_api-2.4.9/gemini/src/misc/constants.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/misc/decorator.py` & `python_gemini_api-2.4.9/gemini/src/misc/decorator.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/misc/exceptions.py` & `python_gemini_api-2.4.9/gemini/src/misc/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/misc/utils.py` & `python_gemini_api-2.4.9/gemini/src/misc/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import json
 import requests
 from typing import Union
 from gemini.src.misc.constants import Headers
+from typing import Dict, Union
 
 
-def load_cookies(file_path):
+def load_cookies(file_path: str) -> Dict:
     """
     Reads a text file and tries to parse it into a Python dictionary.
     Assumes the file might contain a cookies string or is in JSON format.
 
-    :param file_path: Path to the file containing cookie data
-    :return: A dictionary containing cookie data
+    Args:
+        file_path (str): Path to the file containing cookie data.
+
+    Returns:
+        Dict: A dictionary containing cookie data.
     """
     with open(file_path, "r") as file:
         content = file.read().strip()
 
     # If content includes '=', assume it's a cookie string
     if "=" in content:
         try:
@@ -98,22 +102,22 @@
     response.raise_for_status()
 
     return response.text
 
 
 def max_token(text: str, n: int) -> str:
     """
-    Return the first 'n' tokens (words) of the given text.
+    Return the first `n` words, not actual token, of the given text.
 
     Args:
         text (str): The input text to be processed.
         n (int): The number of tokens (words) to be included in the result.
 
     Returns:
-        str: The first 'n' tokens from the input text.
+        str: The first `n` tokens from the input text.
     """
     if not isinstance(text, str):
         raise ValueError("Input 'text' must be a valid string.")
 
     tokens = text.split()  # Split the text into tokens (words)
     if n <= len(tokens):
         return " ".join(tokens[:n])  # Return the first 'n' tokens as a string
```

### Comparing `python_gemini_api-2.4.8/gemini/src/model/image.py` & `python_gemini_api-2.4.9/gemini/src/model/image.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,81 @@
-# Will be refactored.
 import os
-import httpx
 import random
+import httpx
 import asyncio
 import datetime
 from pathlib import Path
 from loguru import logger
-from pydantic import BaseModel, HttpUrl
 from typing import List, Optional, Dict
+from pydantic import BaseModel, HttpUrl
 
 
 class GeminiImage(BaseModel):
     """
     Represents an image with URL, title, and alt text.
 
     Attributes:
         url (HttpUrl): The URL of the image.
         title (str): The title of the image. Defaults to "[Image]".
         alt (str): The alt text of the image. Defaults to "".
-        cookies (Optional[Dict[str, str]]): Optional cookies to be used for fetching the image.
-            This parameter is required if you want to fetch generated images.
 
     Methods:
-        validate_images(images: List["GeminiImage"]) -> bool:
-            Validates the input images list.
-        save(images: List["GeminiImage"], save_path: str = "cached", cookies: Optional[dict] = None) -> Optional[Path]:
+        validate_images(cls, images): Validates the input images list.
+        save(cls, images: List["GeminiImage"], save_path: str = "cached", cookies: Optional[dict] = None) -> Optional[Path]:
             Downloads and saves images asynchronously.
         fetch_bytes(url: HttpUrl, cookies: Optional[dict] = None) -> Optional[bytes]:
             Fetches bytes of an image asynchronously.
-        fetch_images_dict(images: List["GeminiImage"], cookies: Optional[dict] = None) -> Dict[str, bytes]:
+        fetch_images_dict(cls, images: List["GeminiImage"], cookies: Optional[dict] = None) -> Dict[str, bytes]:
             Fetches images asynchronously and returns a dictionary of image data.
-        save_images(image_data: Dict[str, bytes], save_path: str = "cached"):
+        save_images(cls, image_data: Dict[str, bytes], save_path: str = "cached"):
             Saves images locally.
     """
 
     url: HttpUrl
     title: str = "[Image]"
     alt: str = ""
-    cookies: Optional[Dict[str, str]] = None
-
-    def __init__(self, cookies: Optional[Dict[str, str]] = None):
-        """
-        Initialize GeminiImage with optional cookies.
 
-        Args:
-            cookies (Optional[Dict[str, str]]): Optional cookies to be used for fetching the image.
-                *This parameter is required if you want to fetch `generated images`.
-        """
-        self.cookies = cookies
-
-    def validate_images(self, images):
+    @classmethod
+    def validate_images(cls, images):
         """
         Validates the input images list.
 
         Args:
             images: The list of GeminiImage objects.
 
         Raises:
             ValueError: If the input images list is empty.
         """
         if not images:
             raise ValueError(
-                "Input is empty. Please provide GeminiOutput formatted images list to proceed."
+                "Input is empty. Please provide images infomation to proceed."
             )
 
     # Async downloader
+    @classmethod
     async def save(
-        self,
+        cls,
         images: List["GeminiImage"],
         save_path: str = "cached",
+        cookies: Optional[dict] = None,
     ) -> Optional[Path]:
         """
         Downloads and saves images asynchronously.
 
         Args:
             images (List["GeminiImage"]): The list of GeminiImage objects to download.
             save_path (str): The directory path to save the images. Defaults to "cached".
             cookies (Optional[dict]): Cookies to be used for downloading images. Defaults to None.
 
         Returns:
             Optional[Path]: The path to the directory where the images are saved, or None if saving fails.
         """
-        self.validate_images(images)
-        image_data = await self.fetch_images_dict(images, self.cookies)
-        await self.save_images(image_data, save_path)
+        cls.validate_images(images)
+        image_data = await cls.fetch_images_dict(images, cookies)
+        await cls.save_images(image_data, save_path)
 
     @staticmethod
     async def fetch_bytes(
         url: HttpUrl, cookies: Optional[dict] = None
     ) -> Optional[bytes]:
         """
         Fetches bytes of an image asynchronously.
@@ -104,29 +92,30 @@
                 response = await client.get(str(url), cookies=cookies)
                 response.raise_for_status()
                 return response.content
         except Exception as e:
             print(f"Failed to download {url}: {str(e)}")
             return None
 
+    @classmethod
     async def fetch_images_dict(
-        self, images: List["GeminiImage"], cookies: Optional[dict] = None
+        cls, images: List["GeminiImage"], cookies: Optional[dict] = None
     ) -> Dict[str, bytes]:
         """
         Fetches images asynchronously and returns a dictionary of image data.
 
         Args:
             images (List["GeminiImage"]): The list of GeminiImage objects to fetch.
             cookies (Optional[dict]): Cookies to be used for fetching the images. Defaults to None.
 
         Returns:
             Dict[str, bytes]: A dictionary containing image titles as keys and image bytes as values.
         """
-        self.validate_images(images)
-        tasks = [self.fetch_bytes(image.url, cookies=cookies) for image in images]
+        cls.validate_images(images)
+        tasks = [cls.fetch_bytes(image.url, cookies=cookies) for image in images]
         results = await asyncio.gather(*tasks)
         return {image.title: result for image, result in zip(images, results) if result}
 
     @staticmethod
     async def save_images(image_data: Dict[str, bytes], save_path: str = "cached"):
         """
         Saves images locally.
@@ -144,31 +133,32 @@
                 with open(filepath, "wb") as f:
                     f.write(data)
                 print(f"Saved {title} to {filepath}")
             except Exception as e:
                 print(f"Error saving {title}: {str(e)}")
 
     # Sync downloader
+    @staticmethod
     def save_sync(
-        self,
         images: List["GeminiImage"],
+        cookies: Optional[dict] = None,
         save_path: str = "cached",
     ) -> Optional[Path]:
         """Synchronously saves the image to the specified path.
 
         Args:
             path (str): The directory where the image will be saved.
             filename (str, optional): The filename for the saved image. If not provided,
                 a filename is generated based on the image title.
             cookies (dict, optional): Cookies to be used for downloading the image.
 
         Returns:
             Optional[Path]: The path where the image is saved, or None if saving fails.
         """
-        image_data = GeminiImage.fetch_images_dict_sync(images, self.cookies)
+        image_data = GeminiImage.fetch_images_dict_sync(images, cookies)
         GeminiImage.validate_images(image_data)
         GeminiImage.save_images_sync(image_data, save_path)
 
     @staticmethod
     def fetch_bytes_sync(
         url: HttpUrl, cookies: Optional[dict] = None
     ) -> Optional[bytes]:
@@ -224,8 +214,8 @@
             now = datetime.datetime.now().strftime("%y%m%d%H%M%S%f")
             filename = f"{title.replace(' ', '_').replace('[Image]', '').replace('/', '_').replace(':', '_')}_{random.randint(10,99)}_{now}.jpg"
             filepath = Path(save_path) / filename
             try:
                 filepath.write_bytes(data)
             except:
                 pass
-            print(f"Saved {title} to {save_path}")
+            print(f"Saved {title} to {save_path}")
```

### Comparing `python_gemini_api-2.4.8/gemini/src/model/output.py` & `python_gemini_api-2.4.9/gemini/src/model/output.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/model/parser/base.py` & `python_gemini_api-2.4.9/gemini/src/model/parser/base.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/model/parser/custom_parser.py` & `python_gemini_api-2.4.9/gemini/src/model/parser/custom_parser.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/model/parser/response_parser.py` & `python_gemini_api-2.4.9/gemini/src/model/parser/response_parser.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/modules/openrouter/async_client.py` & `python_gemini_api-2.4.9/gemini/src/modules/openrouter/async_client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/modules/openrouter/client.py` & `python_gemini_api-2.4.9/gemini/src/modules/openrouter/client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/modules/voice/google.py` & `python_gemini_api-2.4.9/gemini/src/modules/voice/google.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/gemini/src/modules/voice/openai.py` & `python_gemini_api-2.4.9/gemini/src/modules/voice/openai.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/python_gemini_api.egg-info/PKG-INFO` & `python_gemini_api-2.4.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: python-gemini-api
-Version: 2.4.8
-Summary: The python package that returns Response of Google Gemini through API.
-Home-page: https://github.com/dsdanielpark/Gemini-API
-Author: Daniel Park
-Author-email: parkminwoo1991@gmail.com
-Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx[http2]>=0.20.0
-Requires-Dist: requests
-Requires-Dist: browser_cookie3
-Requires-Dist: loguru
-Requires-Dist: pydantic
-Requires-Dist: aiohttp
-Provides-Extra: voice
-Requires-Dist: gTTS; extra == "voice"
-Requires-Dist: SpeechRecognition; extra == "voice"
-Requires-Dist: openai; extra == "voice"
-Requires-Dist: anthropic; extra == "voice"
-
 
 # <img src="https://www.gstatic.com/lamda/images/favicon_v1_150160cddff7f294ce30.svg" width="35px" alt="Gemini Icon" /> Gemini API  <a href="https://pypi.org/project/python-gemini-api/"> <img alt="PyPI" src="https://img.shields.io/pypi/v/python-gemini-api?color=black"></a>
 
 
 <p align="right">
     <a href="https://github.com/dsdanielpark/Gemini-API"><img alt="pip download" src="https://img.shields.io/badge/pip_install-python_gemini_api-black"></a> 
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
@@ -329,20 +296,19 @@
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
-
 generated_images = response.generated_images # Check generated images [Dict]
 
-await image_client.save(generated_images, "save_dir", cookies=cookies)
-# image_data_dict = await image_client.fetch_images_dict(generated_images, cookies=cookies)
-# await image_client.save_images(image_data_dict, "save_dir")
+await image_client.save(generated_images, "output")
+# image_data_dict = await image_client.fetch_images_dict(generated_images)
+# await image_client.save_images(image_data_dict, "output")
 ```
 
 
 <details><summary>Further</summary>
 
 *Display images in IPython*
   You can display the image or transmit it to another application in byte format.
@@ -351,16 +317,15 @@
   import io
   from gemini import Gemini, GeminiImage
   from IPython.display import display, Image
   
   cookies = {}
   client = Gemini(cookies=cookies)
   image_client = GeminiImage(cookies=cookies)
-
-  bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
+  bytes_images_dict = image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict
   
   for image_name, image_bytes in bytes_images_dict.items():
       print(image_name)
       image = Image(data=image_bytes)
       display(image)
   ```
 
@@ -372,60 +337,60 @@
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
-image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies) # Save default folder is `cached`
+image_client.save_sync(generated_images, save_path="output")
 
 # You can use byte type image dict for printing images as follow:
-# bytes_images_dict = image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
-# image_client.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+# bytes_images_dict = image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, path="output") # Save to dir
 ```
 
 *Async downloader wrapper*
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    await image_client.save(generated_imagse, save_path=save_path, cookies=cookies)
+async def save_generated_imagse(generated_imagse, save_path="output"):
+    await image_client.save(generated_imagse, save_path=save_path)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  
-    asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_generated_imagse(generated_imagse, save_path="output"))
 ```
 
 `GeminiImage.save` method logic
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
-    image_data_dict = await image_client.fetch_images_dict(generated_imagse, cookies=cookies)  # Get bytes images dict asynchronously
+async def save_generated_imagse(generated_imagse, save_path="output"):
+    image_data_dict = await image_client.fetch_images_dict(generated_imagse)  # Get bytes images dict asynchronously
     await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     generated_imagse = response.generated_imagse  # Check response images [Dict]
-    asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_generated_imagse(generated_imagse, save_path="output"))
 ```
 
 </details>
 
 > [!NOTE]
 > Use GeminiImage for image processing. `web_images` works without cookies, but for images like `generated_image` from Gemini, pass cookies. Cookies are needed to download images from Google's storage. Check the response or use existing cookies variable.
 
@@ -440,20 +405,19 @@
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Create illustrations of Seoul, South Korea.")
-
 response_images = response.web_images # Check generated images [Dict]
 
-await image_client.save(response_images, "save_dir")
+await image_client.save(response_images, "output")
 # image_data_dict = await image_client.fetch_images_dict(response_images)
-# await image_client.save_images(image_data_dict, "save_dir")
+# await image_client.save_images(image_data_dict, "output")
 ```
 
 <details><summary>Further</summary>
 
 
 *Sync downloader*
 ```python
@@ -462,58 +426,58 @@
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
 response = client.generate_content("Please recommend a travel itinerary for Seoul.")
 response_images = response.web_images # Check response images [Dict]
 
-GeminiImage.save_sync(response_images, save_path="save_dir")
+GeminiImage.save_sync(response_images, save_path="output")
 
 # You can use byte type image dict as follow:
-# bytes_images_dict = image_client.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
+# bytes_images_dict = image_client.fetch_bytes_sync(response_images) # Get bytes images dict
+# image_client.save_images_sync(bytes_images_dict, save_path="output") # Save to path
 ```
 
 *Async downloader wrapper*
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_response_web_imagse(response_images, save_path="save_dir"):
+async def save_response_web_imagse(response_images, save_path="output"):
     await image_client.save(response_images, save_path=save_path)
 
 # Run the async function
 if __name__ == "__main__":
     cookies = {"key" : "value"}
     response_images = response.web_images  
-    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
+    asyncio.run(save_response_web_imagse(response_images, save_path="output"))
 ```
 
 `GeminiImage.save` method logic
 
 ```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 cookies = {}
 client = Gemini(cookies=cookies)
 image_client = GeminiImage(cookies=cookies)
 
-async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
-    image_data_dict = await image_client.fetch_images_dict(response_images, cookies=cookies)  # Get bytes images dict asynchronously
+async def save_response_web_imagse(response_images, save_path="output"):
+    image_data_dict = await image_client.fetch_images_dict(response_images)  # Get bytes images dict asynchronously
     await image_client.save_images(image_data_dict, save_path=save_path)  
 
 # Run the async function
 if __name__ == "__main__":
     response_images = response.web_images  # Check response images [Dict]
-    asyncio.run(save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies))
+    asyncio.run(save_response_web_imagse(response_images, save_path="output"))
 ```
 
 </details>
 
 <br>
 
 ### # 07. Generate content from images
@@ -773,16 +737,22 @@
 First review [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://aistudio.google.com/) before using this package.
 You can find most help on the [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues) pages. 
             
 ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues)
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated. Frequent errors may occur due to changes in Google's service API interface. Both [Issue reports](https://github.com/dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome. We strive to maintain an active and courteous open community.
 
 ## Contributors
+
+<p align="center"><i>dig the well before you are thirsty.</i></p>
+
+
 We would like to express our sincere gratitude to all the contributors. 
 
+
+
 This package aims to re-implement the functionality of the [Bard API](https://github.com/dsdanielpark/Bard-API/), which has been archived for the contributions of the beloved open-source community, despite Gemini's official API already being available.
 
 Contributors to the [Bard API](https://github.com/dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/Gemini-API/).
 
 <a href="https://github.com/dsdanielpark/Bard_API/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=dsdanielpark/Bard_API" />
 </a>
```

#### html2text {}

```diff
@@ -1,25 +1,8 @@
-Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.8 Summary: The
-python package that returns Response of Google Gemini through API. Home-page:
-https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
-parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
-Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
-2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
-Natural Language :: English Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
-Approved :: MIT License Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.9 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: httpx[http2]>=0.20.0 Requires-
-Dist: requests Requires-Dist: browser_cookie3 Requires-Dist: loguru Requires-
-Dist: pydantic Requires-Dist: aiohttp Provides-Extra: voice Requires-Dist:
-gTTS; extra == "voice" Requires-Dist: SpeechRecognition; extra == "voice"
-Requires-Dist: openai; extra == "voice" Requires-Dist: anthropic; extra ==
-"voice" # [Gemini Icon]Gemini API_[_P_y_P_I_]
+# [Gemini Icon]Gemini API_[_P_y_P_I_]
   _[_p_i_p_ _d_o_w_n_l_o_a_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
                 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_d_s_d_a_n_i_e_l_p_a_r_k_%_2_F_G_e_m_i_n_i_-
 _A_P_I_&_c_o_u_n_t___b_g_=_%_2_3_0_0_0_0_0_0_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_v_i_e_w_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
                                                                     _[_D_o_w_n_l_o_a_d_s_]
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-
 ba79-d9f89b637324 An **unofficial* Python wrapper, [python-gemini-api](https://
 pypi.org/project/python-gemini-api/), is available for users facing frequent
@@ -188,89 +171,85 @@
 "Hello, Gemini. What's the weather like in Seoul today?" response =
 client.generate_content(prompt) print(response.text) ```
 ### # 05. Image generation Returns images generated by Gemini. *Async
 downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
 client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
 response = client.generate_content("Create illustrations of Seoul, South
 Korea.") generated_images = response.generated_images # Check generated images
-[Dict] await image_client.save(generated_images, "save_dir", cookies=cookies) #
-image_data_dict = await image_client.fetch_images_dict(generated_images,
-cookies=cookies) # await image_client.save_images(image_data_dict, "save_dir")
-``` Further *Display images in IPython* You can display the image or transmit
-it to another application in byte format. ```python import io from gemini
-import Gemini, GeminiImage from IPython.display import display, Image cookies =
-{} client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
-bytes_images_dict = image_client.fetch_images_dict_sync(generated_images,
-cookies) # Get bytes images dict for image_name, image_bytes in
-bytes_images_dict.items(): print(image_name) image = Image(data=image_bytes)
-display(image) ``` *Sync downloader* ```python from gemini import Gemini,
-GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client =
-GeminiImage(cookies=cookies) response = client.generate_content("Create
-illustrations of Seoul, South Korea.") generated_images =
-response.generated_images # Check generated images [Dict]
-image_client.save_sync(generated_images, save_path="save_dir", cookies=cookies)
-# Save default folder is `cached` # You can use byte type image dict for
-printing images as follow: # bytes_images_dict =
-image_client.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
-bytes images dict # image_client.save_images_sync(bytes_images_dict,
-path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
-```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
-client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
-async def save_generated_imagse(generated_imagse, save_path="save_dir",
-cookies=cookies): await image_client.save(generated_imagse,
-save_path=save_path, cookies=cookies) # Run the async function if __name__ ==
+[Dict] await image_client.save(generated_images, "output") # image_data_dict =
+await image_client.fetch_images_dict(generated_images) # await
+image_client.save_images(image_data_dict, "output") ``` Further *Display images
+in IPython* You can display the image or transmit it to another application in
+byte format. ```python import io from gemini import Gemini, GeminiImage from
+IPython.display import display, Image cookies = {} client = Gemini
+(cookies=cookies) image_client = GeminiImage(cookies=cookies) bytes_images_dict
+= image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict
+for image_name, image_bytes in bytes_images_dict.items(): print(image_name)
+image = Image(data=image_bytes) display(image) ``` *Sync downloader* ```python
+from gemini import Gemini, GeminiImage cookies = {} client = Gemini
+(cookies=cookies) image_client = GeminiImage(cookies=cookies) response =
+client.generate_content("Create illustrations of Seoul, South Korea.")
+generated_images = response.generated_images # Check generated images [Dict]
+image_client.save_sync(generated_images, save_path="output") # You can use byte
+type image dict for printing images as follow: # bytes_images_dict =
+image_client.fetch_images_dict_sync(generated_images) # Get bytes images dict #
+image_client.save_images_sync(bytes_images_dict, path="output") # Save to dir
+``` *Async downloader wrapper* ```python import asyncio from gemini import
+Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
+= GeminiImage(cookies=cookies) async def save_generated_imagse
+(generated_imagse, save_path="output"): await image_client.save
+(generated_imagse, save_path=save_path) # Run the async function if __name__ ==
 "__main__": cookies = {"key" : "value"} generated_imagse =
 response.generated_imagse asyncio.run(save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies)) ``` `GeminiImage.save` method logic
-```python import asyncio from gemini import Gemini, GeminiImage cookies = {}
-client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
-async def save_generated_imagse(generated_imagse, save_path="save_dir",
-cookies=cookies): image_data_dict = await image_client.fetch_images_dict
-(generated_imagse, cookies=cookies) # Get bytes images dict asynchronously
-await image_client.save_images(image_data_dict, save_path=save_path) # Run the
-async function if __name__ == "__main__": cookies = {"key" : "value"}
-generated_imagse = response.generated_imagse # Check response images [Dict]
-asyncio.run(save_generated_imagse(generated_imagse, save_path="save_dir",
-cookies=cookies)) ``` > [!NOTE] > Use GeminiImage for image processing.
-`web_images` works without cookies, but for images like `generated_image` from
-Gemini, pass cookies. Cookies are needed to download images from Google's
-storage. Check the response or use existing cookies variable.
+save_path="output")) ``` `GeminiImage.save` method logic ```python import
+asyncio from gemini import Gemini, GeminiImage cookies = {} client = Gemini
+(cookies=cookies) image_client = GeminiImage(cookies=cookies) async def
+save_generated_imagse(generated_imagse, save_path="output"): image_data_dict =
+await image_client.fetch_images_dict(generated_imagse) # Get bytes images dict
+asynchronously await image_client.save_images(image_data_dict,
+save_path=save_path) # Run the async function if __name__ == "__main__":
+cookies = {"key" : "value"} generated_imagse = response.generated_imagse #
+Check response images [Dict] asyncio.run(save_generated_imagse
+(generated_imagse, save_path="output")) ``` > [!NOTE] > Use GeminiImage for
+image processing. `web_images` works without cookies, but for images like
+`generated_image` from Gemini, pass cookies. Cookies are needed to download
+images from Google's storage. Check the response or use existing cookies
+variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
 Gemini. *Async downloader* ```python from gemini import Gemini, GeminiImage
 cookies = {} client = Gemini(cookies=cookies) image_client = GeminiImage
 (cookies=cookies) response = client.generate_content("Create illustrations of
 Seoul, South Korea.") response_images = response.web_images # Check generated
-images [Dict] await image_client.save(response_images, "save_dir") #
+images [Dict] await image_client.save(response_images, "output") #
 image_data_dict = await image_client.fetch_images_dict(response_images) # await
-image_client.save_images(image_data_dict, "save_dir") ``` Further *Sync
+image_client.save_images(image_data_dict, "output") ``` Further *Sync
 downloader* ```python from gemini import Gemini, GeminiImage cookies = {}
 client = Gemini(cookies=cookies) image_client = GeminiImage(cookies=cookies)
 response = client.generate_content("Please recommend a travel itinerary for
 Seoul.") response_images = response.web_images # Check response images [Dict]
-GeminiImage.save_sync(response_images, save_path="save_dir") # You can use byte
+GeminiImage.save_sync(response_images, save_path="output") # You can use byte
 type image dict as follow: # bytes_images_dict = image_client.fetch_bytes_sync
-(response_images, cookies) # Get bytes images dict #
-image_client.save_images_sync(bytes_images_dict, path="save_dir") # Save to
-path ``` *Async downloader wrapper* ```python import asyncio from gemini import
-Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
-= GeminiImage(cookies=cookies) async def save_response_web_imagse
-(response_images, save_path="save_dir"): await image_client.save
-(response_images, save_path=save_path) # Run the async function if __name__ ==
-"__main__": cookies = {"key" : "value"} response_images = response.web_images
-asyncio.run(save_response_web_imagse(response_images, save_path="save_dir"))
-``` `GeminiImage.save` method logic ```python import asyncio from gemini import
+(response_images) # Get bytes images dict # image_client.save_images_sync
+(bytes_images_dict, save_path="output") # Save to path ``` *Async downloader
+wrapper* ```python import asyncio from gemini import Gemini, GeminiImage
+cookies = {} client = Gemini(cookies=cookies) image_client = GeminiImage
+(cookies=cookies) async def save_response_web_imagse(response_images,
+save_path="output"): await image_client.save(response_images,
+save_path=save_path) # Run the async function if __name__ == "__main__":
+cookies = {"key" : "value"} response_images = response.web_images asyncio.run
+(save_response_web_imagse(response_images, save_path="output")) ```
+`GeminiImage.save` method logic ```python import asyncio from gemini import
 Gemini, GeminiImage cookies = {} client = Gemini(cookies=cookies) image_client
 = GeminiImage(cookies=cookies) async def save_response_web_imagse
-(response_images, save_path="save_dir", cookies=cookies): image_data_dict =
-await image_client.fetch_images_dict(response_images, cookies=cookies) # Get
-bytes images dict asynchronously await image_client.save_images
-(image_data_dict, save_path=save_path) # Run the async function if __name__ ==
-"__main__": response_images = response.web_images # Check response images
-[Dict] asyncio.run(save_response_web_imagse(response_images,
-save_path="save_dir", cookies=cookies)) ```
+(response_images, save_path="output"): image_data_dict = await
+image_client.fetch_images_dict(response_images) # Get bytes images dict
+asynchronously await image_client.save_images(image_data_dict,
+save_path=save_path) # Run the async function if __name__ == "__main__":
+response_images = response.web_images # Check response images [Dict]
+asyncio.run(save_response_web_imagse(response_images, save_path="output")) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
 image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. # Image file
 path or Byte-formatted image array response = client.generate_content("What
 does the text in this image say?", image=image) response.response_dict ```
 ### # 08. Generate content using Google Services To begin, you must link Google
 Workspace to activate this extension via the [Gemini web extension](https://
@@ -429,14 +408,15 @@
 pages. ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues) Sincerely
 grateful for any reports on new features or bugs. Your valuable feedback on the
 code is highly appreciated. Frequent errors may occur due to changes in
 Google's service API interface. Both [Issue reports](https://github.com/
 dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/
 dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome.
 We strive to maintain an active and courteous open community. ## Contributors
+                     dig the well before you are thirsty.
 We would like to express our sincere gratitude to all the contributors. This
 package aims to re-implement the functionality of the [Bard API](https://
 github.com/dsdanielpark/Bard-API/), which has been archived for the
 contributions of the beloved open-source community, despite Gemini's official
 API already being available. Contributors to the [Bard API](https://github.com/
 dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/
 Gemini-API/). _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_s_d_a_n_i_e_l_p_a_r_k_/_B_a_r_d___A_P_I_]
```

### Comparing `python_gemini_api-2.4.8/python_gemini_api.egg-info/SOURCES.txt` & `python_gemini_api-2.4.9/python_gemini_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.8/setup.py` & `python_gemini_api-2.4.9/setup.py`

 * *Files identical despite different names*

