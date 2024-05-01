# Comparing `tmp/modelpark-0.1.7.tar.gz` & `tmp/modelpark-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelpark-0.1.7.tar", last modified: Tue Apr 30 16:04:18 2024, max compression
+gzip compressed data, was "modelpark-0.1.8.tar", last modified: Tue Apr 30 16:47:12 2024, max compression
```

## Comparing `modelpark-0.1.7.tar` & `modelpark-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-30 16:04:18.628250 modelpark-0.1.7/
--rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.7/LICENSE
--rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.7/MANIFEST.in
--rw-r--r--   0 vkocaman   (501) staff       (20)     3425 2024-04-30 16:04:18.628028 modelpark-0.1.7/PKG-INFO
--rw-r--r--   0 vkocaman   (501) staff       (20)     2524 2024-04-28 20:18:29.000000 modelpark-0.1.7/README.md
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-30 16:04:18.626955 modelpark-0.1.7/modelpark/
--rw-rw-r--   0 vkocaman   (501) staff       (20)      345 2024-04-30 15:17:46.000000 modelpark-0.1.7/modelpark/__init__.py
--rw-rw-r--   0 vkocaman   (501) staff       (20)     4836 2024-04-30 16:04:10.000000 modelpark-0.1.7/modelpark/modelpark.py
-drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-30 16:04:18.627798 modelpark-0.1.7/modelpark.egg-info/
--rw-r--r--   0 vkocaman   (501) staff       (20)     3425 2024-04-30 16:04:18.000000 modelpark-0.1.7/modelpark.egg-info/PKG-INFO
--rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-30 16:04:18.000000 modelpark-0.1.7/modelpark.egg-info/SOURCES.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-30 16:04:18.000000 modelpark-0.1.7/modelpark.egg-info/dependency_links.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-30 16:04:18.000000 modelpark-0.1.7/modelpark.egg-info/requires.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-30 16:04:18.000000 modelpark-0.1.7/modelpark.egg-info/top_level.txt
--rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-30 16:04:18.628292 modelpark-0.1.7/setup.cfg
--rw-r--r--   0 vkocaman   (501) staff       (20)     4544 2024-04-30 15:48:13.000000 modelpark-0.1.7/setup.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-30 16:47:12.254287 modelpark-0.1.8/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     1067 2024-04-28 09:08:05.000000 modelpark-0.1.8/LICENSE
+-rw-rw-r--   0 vkocaman   (501) staff       (20)       20 2024-04-28 09:08:05.000000 modelpark-0.1.8/MANIFEST.in
+-rw-r--r--   0 vkocaman   (501) staff       (20)     3425 2024-04-30 16:47:12.254053 modelpark-0.1.8/PKG-INFO
+-rw-r--r--   0 vkocaman   (501) staff       (20)     2524 2024-04-28 20:18:29.000000 modelpark-0.1.8/README.md
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-30 16:47:12.252909 modelpark-0.1.8/modelpark/
+-rw-rw-r--   0 vkocaman   (501) staff       (20)      345 2024-04-30 16:46:39.000000 modelpark-0.1.8/modelpark/__init__.py
+-rw-rw-r--   0 vkocaman   (501) staff       (20)     4836 2024-04-30 16:04:10.000000 modelpark-0.1.8/modelpark/modelpark.py
+drwxr-xr-x   0 vkocaman   (501) staff       (20)        0 2024-04-30 16:47:12.253820 modelpark-0.1.8/modelpark.egg-info/
+-rw-r--r--   0 vkocaman   (501) staff       (20)     3425 2024-04-30 16:47:12.000000 modelpark-0.1.8/modelpark.egg-info/PKG-INFO
+-rw-r--r--   0 vkocaman   (501) staff       (20)      247 2024-04-30 16:47:12.000000 modelpark-0.1.8/modelpark.egg-info/SOURCES.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        1 2024-04-30 16:47:12.000000 modelpark-0.1.8/modelpark.egg-info/dependency_links.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)        9 2024-04-30 16:47:12.000000 modelpark-0.1.8/modelpark.egg-info/requires.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       10 2024-04-30 16:47:12.000000 modelpark-0.1.8/modelpark.egg-info/top_level.txt
+-rw-r--r--   0 vkocaman   (501) staff       (20)       38 2024-04-30 16:47:12.254327 modelpark-0.1.8/setup.cfg
+-rw-r--r--   0 vkocaman   (501) staff       (20)     5548 2024-04-30 16:46:39.000000 modelpark-0.1.8/setup.py
```

### Comparing `modelpark-0.1.7/LICENSE` & `modelpark-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.7/PKG-INFO` & `modelpark-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.7
+Version: 0.1.8
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `modelpark-0.1.7/README.md` & `modelpark-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.7/modelpark/modelpark.py` & `modelpark-0.1.8/modelpark/modelpark.py`

 * *Files identical despite different names*

### Comparing `modelpark-0.1.7/modelpark.egg-info/PKG-INFO` & `modelpark-0.1.8/modelpark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelpark
-Version: 0.1.7
+Version: 0.1.8
 Summary: Versatile solution for sharing apps through secure URLs
 Home-page: https://github.com/model-park/modelpark
 Author: Your Name
 Author-email: info@modelpark.app
 License: MIT
 Keywords: modelpark,deployment,cloud,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `modelpark-0.1.7/setup.py` & `modelpark-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import platform
 import subprocess
 from setuptools import setup, find_packages
 from setuptools.command.install import install
+import requests
 
 class CustomInstall(install):
     def run(self):
         install.run(self)
         self.remove_existing_binary()  # Ensure any existing version is removed
         self.install_system_specific_dependencies()
 
@@ -25,28 +26,51 @@
             if os.path.exists(executable_path):
                 os.remove(executable_path)
                 print(f"Removed existing binary at {executable_path}")
 
     def install_system_specific_dependencies(self):
         """Install system-specific dependencies based on the OS."""
         os_type = platform.system().lower()
-        if os_type in ["linux", "darwin"]:  # Unix-like systems including macOS
-            url = "https://modelpark.app/dist-folder/modelpark-cli-linux" if os_type == "linux" else "https://modelpark.app/dist-folder/modelpark-cli-macos"
-            self.download_and_install(url)
+        #if os_type in ["linux", "darwin"]:  # Unix-like systems including macOS
+        if os_type == "linux":
+            url = "https://modelpark.app/dist-folder/modelpark-cli-linux" 
+            self.download_and_install_linux(url)
+        elif os_type == "darwin":
+            url = "https://modelpark.app/dist-folder/modelpark-cli-macos"
+            self.download_and_install_macos(url)
         elif os_type == "windows":
             url = "https://modelpark.app/dist/mpinstaller.exe"
             self.download_and_install_windows(url)
 
-    def download_and_install(self, url):
+    def download_and_install_macos(self, url):
         """Download and install binary for Unix-like systems."""
         home_dir = os.path.expanduser('~')
         binary_path = os.path.join(home_dir, "modelpark")
         subprocess.check_call(['curl', url, '-o', binary_path])
         subprocess.check_call(['chmod', '+x', binary_path])
         #self.add_to_path(home_dir)
+    
+    def download_and_install_linux(self, url):
+        """Download and install binary for Unix-like systems using Python's requests library."""
+        home_dir = os.path.expanduser('~')
+        binary_path = os.path.join(home_dir, "modelpark")
+        
+        # Download the file
+        response = requests.get(url, stream=True)
+        if response.status_code == 200:
+            with open(binary_path, 'wb') as f:
+                for chunk in response.iter_content(chunk_size=8192): 
+                    if chunk:  # filter out keep-alive new chunks
+                        f.write(chunk)
+            # Make the file executable (specifically for Unix-like systems)
+            os.chmod(binary_path, 0o755)
+            print(f"Installed binary to {binary_path}")
+        else:
+            print(f"Failed to download file: Status code {response.status_code}")
+
 
     def add_to_path(self, target_dir):
         """Add the installation directory to the user's PATH in .bashrc or .bash_profile."""
         path_update_script = f'\nexport PATH="$PATH:{target_dir}"\n'
         profile_path = os.path.join(os.path.expanduser('~'), '.bash_profile' if platform.system().lower() == 'darwin' else '.bashrc')
         with open(profile_path, 'a') as profile_file:
             profile_file.write(path_update_script)
@@ -63,15 +87,15 @@
         """Add the installation directory to the PATH for Windows."""
         command = f'[Environment]::SetEnvironmentVariable("Path", [Environment]::GetEnvironmentVariable("Path", [EnvironmentVariableTarget]::User) + ";{install_path}", [EnvironmentVariableTarget]::User)'
         subprocess.check_call(['powershell', command], shell=True)
         print(f"Added {install_path} to PATH for Windows")
 
 setup(
     name='modelpark',
-    version='0.1.7',
+    version='0.1.8',
     description='Versatile solution for sharing apps through secure URLs',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/model-park/modelpark',
     author='Your Name',
     author_email='info@modelpark.app',
     license='MIT',
```

