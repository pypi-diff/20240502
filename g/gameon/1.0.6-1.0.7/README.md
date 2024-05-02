# Comparing `tmp/gameon-1.0.6.tar.gz` & `tmp/gameon-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameon-1.0.6.tar", last modified: Sat Apr 27 20:52:24 2024, max compression
+gzip compressed data, was "gameon-1.0.7.tar", last modified: Thu May  2 19:52:08 2024, max compression
```

## Comparing `gameon-1.0.6.tar` & `gameon-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 20:52:24.507185 gameon-1.0.6/
--rw-rw-rw-   0        0        0      548 2024-04-27 20:52:14.000000 gameon-1.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.6/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      262 2024-04-27 20:52:24.502761 gameon-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 20:52:24.490755 gameon-1.0.6/gameon/
--rw-rw-rw-   0        0        0    19116 2024-04-27 20:51:47.000000 gameon-1.0.6/gameon/__init__.py
--rw-rw-rw-   0        0        0    11661 2024-04-25 10:58:03.000000 gameon-1.0.6/gameon/icon.ico
-drwxrwxrwx   0        0        0        0 2024-04-27 20:52:24.502761 gameon-1.0.6/gameon.egg-info/
--rw-rw-rw-   0        0        0      262 2024-04-27 20:52:24.000000 gameon-1.0.6/gameon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-04-27 20:52:24.000000 gameon-1.0.6/gameon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 20:52:24.000000 gameon-1.0.6/gameon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-27 20:52:24.000000 gameon-1.0.6/gameon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-27 20:52:24.000000 gameon-1.0.6/gameon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 20:52:24.508185 gameon-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      396 2024-04-27 20:51:58.000000 gameon-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:52:08.959020 gameon-1.0.7/
+-rw-rw-rw-   0        0        0      628 2024-05-02 19:51:48.000000 gameon-1.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      262 2024-05-02 19:52:08.959020 gameon-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 19:52:08.944713 gameon-1.0.7/gameon/
+-rw-rw-rw-   0        0        0    19268 2024-05-02 19:50:50.000000 gameon-1.0.7/gameon/__init__.py
+-rw-rw-rw-   0        0        0    11661 2024-04-25 10:58:03.000000 gameon-1.0.7/gameon/icon.ico
+drwxrwxrwx   0        0        0        0 2024-05-02 19:52:08.957775 gameon-1.0.7/gameon.egg-info/
+-rw-rw-rw-   0        0        0      262 2024-05-02 19:52:08.000000 gameon-1.0.7/gameon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-05-02 19:52:08.000000 gameon-1.0.7/gameon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 19:52:08.000000 gameon-1.0.7/gameon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-02 19:52:08.000000 gameon-1.0.7/gameon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-02 19:52:08.000000 gameon-1.0.7/gameon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 19:52:08.959020 gameon-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-05-02 19:51:57.000000 gameon-1.0.7/setup.py
```

### Comparing `gameon-1.0.6/CHANGELOG.txt` & `gameon-1.0.7/CHANGELOG.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,10 +21,14 @@
 -------------------
 - Fixed icon not loading causing issues
 
 1.0.5 (4/27/2024)
 -------------------
 - Fixed icon not loading causing issues again
 
-1.0. 6(4/27/2024)
+1.0.6 (4/27/2024)
 -------------------
 - Fixed icon not loading causing issues again x2
+
+1.0.7 (5/02/2024)
+-------------------
+- Added load() function to load images
```

### Comparing `gameon-1.0.6/LICENCE.txt` & `gameon-1.0.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `gameon-1.0.6/gameon/__init__.py` & `gameon-1.0.7/gameon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,18 @@
 
 def fps(frames=120):
     clock.tick(frames)
     return clock.get_fps()
     pass
 
 def icon(image):
-    pygame.display.set_icon(pygame.image.load(image))
+    if isinstance(image, str):
+        pygame.display.set_icon(pygame.image.load(image))
+    else:
+        pygame.display.set_icon(image)
     pass
 
 def title(title):
     pygame.display.set_caption(title)
     pass
 
 def update():
@@ -499,7 +502,11 @@
             return False
     elif isinstance(rect2, tuple) and rect1 == 'mouse':
         if pygame.Rect(rect2).collidepoint((mx,my)):
             return True
         else:
             return False
     pass
+
+def load(image):
+    return pygame.image.load(image)
+    pass
```

### Comparing `gameon-1.0.6/gameon/icon.ico` & `gameon-1.0.7/gameon/icon.ico`

 * *Files identical despite different names*

