# Comparing `tmp/musicnotes-1.0.1.tar.gz` & `tmp/musicnotes-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicnotes-1.0.1.tar", last modified: Thu May  2 00:47:47 2024, max compression
+gzip compressed data, was "musicnotes-1.0.2.tar", last modified: Thu May  2 01:22:47 2024, max compression
```

## Comparing `musicnotes-1.0.1.tar` & `musicnotes-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 00:47:47.363648 musicnotes-1.0.1/
--rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     4437 2024-05-02 00:47:47.361635 musicnotes-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2902 2024-05-01 23:44:11.000000 musicnotes-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 00:47:47.359587 musicnotes-1.0.1/musicnotes.egg-info/
--rw-rw-rw-   0        0        0     4437 2024-05-02 00:47:47.000000 musicnotes-1.0.1/musicnotes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-05-02 00:47:47.000000 musicnotes-1.0.1/musicnotes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 00:47:47.000000 musicnotes-1.0.1/musicnotes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 00:47:47.000000 musicnotes-1.0.1/musicnotes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1210 2024-05-02 00:00:06.000000 musicnotes-1.0.1/musicnotes.py
--rw-rw-rw-   0        0        0       42 2024-05-02 00:47:47.364647 musicnotes-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1887 2024-05-02 00:45:59.000000 musicnotes-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 01:22:47.676878 musicnotes-1.0.2/
+-rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4686 2024-05-02 01:22:47.674366 musicnotes-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3091 2024-05-02 00:50:49.000000 musicnotes-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 01:22:47.669490 musicnotes-1.0.2/musicnotes.egg-info/
+-rw-rw-rw-   0        0        0     4686 2024-05-02 01:22:47.000000 musicnotes-1.0.2/musicnotes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-05-02 01:22:47.000000 musicnotes-1.0.2/musicnotes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 01:22:47.000000 musicnotes-1.0.2/musicnotes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 01:22:47.000000 musicnotes-1.0.2/musicnotes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1210 2024-05-02 00:00:06.000000 musicnotes-1.0.2/musicnotes.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 01:22:47.676878 musicnotes-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1939 2024-05-02 01:21:38.000000 musicnotes-1.0.2/setup.py
```

### Comparing `musicnotes-1.0.1/LICENSE` & `musicnotes-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.1/PKG-INFO` & `musicnotes-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: musicnotes
-Version: 1.0.1
+Version: 1.0.2
 Summary: Play music notes in your Python scripts with ease.
+Home-page: https://github.com/must108/musicnotes
 Author: Mustaeen Ahmed
 Author-email: contact@mustaeen.dev
 License: MIT
 Keywords: sound,music,mp3,wave,wav,media,song,play,audio,notes,music notes,melody
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,14 +32,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # musicnotes
 
 *Play music notes in your Python scripts with ease.*
 
+# Installation
+
+Install with pip:
+
+```
+pip install musicnotes
+```
+
+You can also install manually from the GitHub repository linked [here](https://github.com/must108/musicnotes).
+
 # Issues
 
 Anyone wishing to contribute to this project can focus on the following issues.
 
 ### Instruments
 We need to add more instruments, and more keys to the piano as well. This would be a good first PR for anyone willing to contribute to this project.
```

### Comparing `musicnotes-1.0.1/README.md` & `musicnotes-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # musicnotes
 
 *Play music notes in your Python scripts with ease.*
 
+# Installation
+
+Install with pip:
+
+```
+pip install musicnotes
+```
+
+You can also install manually from the GitHub repository linked [here](https://github.com/must108/musicnotes).
+
 # Issues
 
 Anyone wishing to contribute to this project can focus on the following issues.
 
 ### Instruments
 We need to add more instruments, and more keys to the piano as well. This would be a good first PR for anyone willing to contribute to this project.
```

### Comparing `musicnotes-1.0.1/musicnotes.egg-info/PKG-INFO` & `musicnotes-1.0.2/musicnotes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: musicnotes
-Version: 1.0.1
+Version: 1.0.2
 Summary: Play music notes in your Python scripts with ease.
+Home-page: https://github.com/must108/musicnotes
 Author: Mustaeen Ahmed
 Author-email: contact@mustaeen.dev
 License: MIT
 Keywords: sound,music,mp3,wave,wav,media,song,play,audio,notes,music notes,melody
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,14 +32,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # musicnotes
 
 *Play music notes in your Python scripts with ease.*
 
+# Installation
+
+Install with pip:
+
+```
+pip install musicnotes
+```
+
+You can also install manually from the GitHub repository linked [here](https://github.com/must108/musicnotes).
+
 # Issues
 
 Anyone wishing to contribute to this project can focus on the following issues.
 
 ### Instruments
 We need to add more instruments, and more keys to the piano as well. This would be a good first PR for anyone willing to contribute to this project.
```

### Comparing `musicnotes-1.0.1/musicnotes.py` & `musicnotes-1.0.2/musicnotes.py`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.1/setup.py` & `musicnotes-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 here = abspath(dirname(getsource(lambda: 0)))
 
 with open(join(here, 'README.md'), encoding = 'utf-8') as f:
     desc = f.read()
 
 setup (
     name = 'musicnotes',
-    version = '1.0.1',
+    version = '1.0.2',
     description = 'Play music notes in your Python scripts with ease.',
     long_description = desc,
     long_description_content_type = 'text/markdown',
+    url = 'https://github.com/must108/musicnotes',
     author = 'Mustaeen Ahmed',
     author_email = 'contact@mustaeen.dev',
     license = 'MIT',
     keywords = ['sound', 'music', 'mp3', 'wave', 'wav', 'media', 'song', 'play', 'audio', 'notes', 'music notes', 'melody'],
     classifiers = [
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

