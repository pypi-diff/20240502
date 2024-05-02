# Comparing `tmp/kernels-mixer-0.0.8.tar.gz` & `tmp/kernels-mixer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kernels-mixer-0.0.8.tar", last modified: Thu Feb 29 00:32:47 2024, max compression
+gzip compressed data, was "kernels-mixer-0.0.9.tar", last modified: Tue Mar  5 19:17:22 2024, max compression
```

## Comparing `kernels-mixer-0.0.8.tar` & `kernels-mixer-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 weiyans  (871667) primarygroup (89939)        0 2024-02-29 00:32:47.312258 kernels-mixer-0.0.8/
--rw-r-----   0 weiyans  (871667) primarygroup (89939)    11358 2024-02-23 22:35:08.000000 kernels-mixer-0.0.8/LICENSE
--rw-r-----   0 weiyans  (871667) primarygroup (89939)       15 2024-02-23 22:35:08.000000 kernels-mixer-0.0.8/MANIFEST.in
--rw-r--r--   0 weiyans  (871667) primarygroup (89939)     2130 2024-02-29 00:32:47.312258 kernels-mixer-0.0.8/PKG-INFO
--rw-r-----   0 weiyans  (871667) primarygroup (89939)     1651 2024-02-23 22:35:08.000000 kernels-mixer-0.0.8/README.md
-drwxr-x---   0 weiyans  (871667) primarygroup (89939)        0 2024-02-29 00:32:47.308257 kernels-mixer-0.0.8/kernels_mixer/
--rw-r-----   0 weiyans  (871667) primarygroup (89939)      633 2024-02-23 22:35:08.000000 kernels-mixer-0.0.8/kernels_mixer/__init__.py
--rw-r-----   0 weiyans  (871667) primarygroup (89939)     1327 2024-02-23 22:35:08.000000 kernels-mixer-0.0.8/kernels_mixer/config.py
--rw-r-----   0 weiyans  (871667) primarygroup (89939)     4773 2024-02-29 00:25:32.000000 kernels-mixer-0.0.8/kernels_mixer/kernels.py
--rw-r-----   0 weiyans  (871667) primarygroup (89939)     6853 2024-02-29 00:25:32.000000 kernels-mixer-0.0.8/kernels_mixer/kernels_test.py
--rw-r-----   0 weiyans  (871667) primarygroup (89939)     5854 2024-02-23 22:35:08.000000 kernels-mixer-0.0.8/kernels_mixer/kernelspecs.py
--rw-r-----   0 weiyans  (871667) primarygroup (89939)     5760 2024-02-23 22:35:08.000000 kernels-mixer-0.0.8/kernels_mixer/websockets.py
-drwxr-x---   0 weiyans  (871667) primarygroup (89939)        0 2024-02-29 00:32:47.312258 kernels-mixer-0.0.8/kernels_mixer.egg-info/
--rw-r--r--   0 weiyans  (871667) primarygroup (89939)     2130 2024-02-29 00:32:47.000000 kernels-mixer-0.0.8/kernels_mixer.egg-info/PKG-INFO
--rw-r-----   0 weiyans  (871667) primarygroup (89939)      384 2024-02-29 00:32:47.000000 kernels-mixer-0.0.8/kernels_mixer.egg-info/SOURCES.txt
--rw-r-----   0 weiyans  (871667) primarygroup (89939)        1 2024-02-29 00:32:47.000000 kernels-mixer-0.0.8/kernels_mixer.egg-info/dependency_links.txt
--rw-r-----   0 weiyans  (871667) primarygroup (89939)       60 2024-02-29 00:32:47.000000 kernels-mixer-0.0.8/kernels_mixer.egg-info/requires.txt
--rw-r-----   0 weiyans  (871667) primarygroup (89939)       14 2024-02-29 00:32:47.000000 kernels-mixer-0.0.8/kernels_mixer.egg-info/top_level.txt
--rw-r-----   0 weiyans  (871667) primarygroup (89939)       38 2024-02-29 00:32:47.312258 kernels-mixer-0.0.8/setup.cfg
--rw-r-----   0 weiyans  (871667) primarygroup (89939)     1228 2024-02-29 00:25:32.000000 kernels-mixer-0.0.8/setup.py
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-03-05 19:17:22.535130 kernels-mixer-0.0.9/
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)    11358 2023-08-16 23:16:35.000000 kernels-mixer-0.0.9/LICENSE
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       15 2023-08-16 23:16:35.000000 kernels-mixer-0.0.9/MANIFEST.in
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2130 2024-03-05 19:17:22.535130 kernels-mixer-0.0.9/PKG-INFO
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1651 2023-08-16 23:16:35.000000 kernels-mixer-0.0.9/README.md
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-03-05 19:17:22.534130 kernels-mixer-0.0.9/kernels_mixer/
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      633 2023-08-16 23:16:35.000000 kernels-mixer-0.0.9/kernels_mixer/__init__.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1327 2023-08-16 23:16:35.000000 kernels-mixer-0.0.9/kernels_mixer/config.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     4815 2024-03-05 19:16:36.000000 kernels-mixer-0.0.9/kernels_mixer/kernels.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     6885 2024-03-05 19:16:36.000000 kernels-mixer-0.0.9/kernels_mixer/kernels_test.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     5854 2023-10-26 23:26:45.000000 kernels-mixer-0.0.9/kernels_mixer/kernelspecs.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     5760 2023-11-01 20:53:37.000000 kernels-mixer-0.0.9/kernels_mixer/websockets.py
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-03-05 19:17:22.535130 kernels-mixer-0.0.9/kernels_mixer.egg-info/
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2130 2024-03-05 19:17:22.000000 kernels-mixer-0.0.9/kernels_mixer.egg-info/PKG-INFO
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      384 2024-03-05 19:17:22.000000 kernels-mixer-0.0.9/kernels_mixer.egg-info/SOURCES.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)        1 2024-03-05 19:17:22.000000 kernels-mixer-0.0.9/kernels_mixer.egg-info/dependency_links.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       60 2024-03-05 19:17:22.000000 kernels-mixer-0.0.9/kernels_mixer.egg-info/requires.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       14 2024-03-05 19:17:22.000000 kernels-mixer-0.0.9/kernels_mixer.egg-info/top_level.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       38 2024-03-05 19:17:22.535130 kernels-mixer-0.0.9/setup.cfg
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1228 2024-03-05 19:16:36.000000 kernels-mixer-0.0.9/setup.py
```

### Comparing `kernels-mixer-0.0.8/LICENSE` & `kernels-mixer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kernels-mixer-0.0.8/PKG-INFO` & `kernels-mixer-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kernels-mixer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Jupyter server extension that allows mixing local and remote kernels together
 Home-page: https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/kernels-mixer
 Author: Google, Inc.
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `kernels-mixer-0.0.8/README.md` & `kernels-mixer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kernels-mixer-0.0.8/kernels_mixer/__init__.py` & `kernels-mixer-0.0.9/kernels_mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `kernels-mixer-0.0.8/kernels_mixer/config.py` & `kernels-mixer-0.0.9/kernels_mixer/config.py`

 * *Files identical despite different names*

### Comparing `kernels-mixer-0.0.8/kernels_mixer/kernels.py` & `kernels-mixer-0.0.9/kernels_mixer/kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,18 @@
         # Set up the remote kernel management.
         self.remote_manager = GatewayMappingKernelManager(
             parent=self.parent,
             log=self.log,
             connection_dir=self.connection_dir,
             kernel_spec_manager=self.kernel_spec_manager.remote_manager)
 
+    def list_kernels(self):
+        run_sync(self.remote_manager.list_kernels)()
+        return super().list_kernels()
+
     def kernel_model(self, kernel_id):
         self._check_kernel_id(kernel_id)
         kernel = self._kernels[kernel_id]
         return run_sync(kernel.model)()
 
 class MixingKernelManager(ServerKernelManager):
     _kernel_id_map = {}
@@ -117,13 +121,12 @@
             self.delegate_kernel_id))
 
     async def restart_kernel(self, *args, **kwargs):
         await ensure_async(self.delegate_multi_kernel_manager.restart_kernel(
             self.delegate_kernel_id, *args, **kwargs))
 
     async def model(self):
-        await ensure_async(self.delegate_multi_kernel_manager.list_kernels())
         delegate_model = await ensure_async(
             self.delegate_multi_kernel_manager.kernel_model(self.delegate_kernel_id))
         model = copy.deepcopy(delegate_model)
         model["id"] = self.kernel_id
         return model
```

### Comparing `kernels-mixer-0.0.8/kernels_mixer/kernels_test.py` & `kernels-mixer-0.0.9/kernels_mixer/kernels_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,15 @@
         self.assertEqual(local_kernel_model["execution_state"], "idle")
         self.assertNotIn("additional", local_kernel_model)
         run_sync(self.interrupt_kernel)(local_kernel_id)
         run_sync(self.mkm.restart_kernel)(local_kernel_id)
 
     def test_remote_kernel_model(self):
         remote_kernel_id = run_sync(self.mkm.start_kernel)(kernel_name=remote_kernel)
+        self.mkm.list_kernels()
         remote_kernel_model = self.mkm.kernel_model(remote_kernel_id)
         self.assertEqual(remote_kernel_model["id"], remote_kernel_id)
         self.assertEqual(remote_kernel_model["name"], remote_kernel)
         self.assertEqual(remote_kernel_model["additional"]["foo"], "bar")
         self.assertEqual(remote_kernel_model["execution_state"], "idle")
         run_sync(self.interrupt_kernel)(remote_kernel_id)
         run_sync(self.mkm.restart_kernel)(remote_kernel_id)
```

### Comparing `kernels-mixer-0.0.8/kernels_mixer/kernelspecs.py` & `kernels-mixer-0.0.9/kernels_mixer/kernelspecs.py`

 * *Files identical despite different names*

### Comparing `kernels-mixer-0.0.8/kernels_mixer/websockets.py` & `kernels-mixer-0.0.9/kernels_mixer/websockets.py`

 * *Files identical despite different names*

### Comparing `kernels-mixer-0.0.8/kernels_mixer.egg-info/PKG-INFO` & `kernels-mixer-0.0.9/kernels_mixer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kernels-mixer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Jupyter server extension that allows mixing local and remote kernels together
 Home-page: https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/kernels-mixer
 Author: Google, Inc.
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `kernels-mixer-0.0.8/setup.py` & `kernels-mixer-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="kernels-mixer",
-  version="0.0.8",
+  version="0.0.9",
   author="Google, Inc.",
   description="Jupyter server extension that allows mixing local and remote kernels together",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/kernels-mixer",
   license="Apache License 2.0",
   packages=setuptools.find_packages(),
```

