# Comparing `tmp/imviz-0.2.3.tar.gz` & `tmp/imviz-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imviz-0.2.3.tar", last modified: Thu Sep 14 14:18:27 2023, max compression
+gzip compressed data, was "imviz-0.2.4.tar", last modified: Thu May  2 10:12:15 2024, max compression
```

## Comparing `imviz-0.2.3.tar` & `imviz-0.2.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2023-09-14 14:18:27.317630 imviz-0.2.3/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     5369 2023-03-23 16:13:28.000000 imviz-0.2.3/CMakeLists.txt
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1071 2023-08-10 09:58:03.000000 imviz-0.2.3/LICENSE
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       61 2021-11-18 07:19:23.000000 imviz-0.2.3/MANIFEST.in
--rw-r--r--   0 ruof      (1000) ruof      (1000)     2467 2023-09-14 14:18:27.317630 imviz-0.2.3/PKG-INFO
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     2063 2021-11-18 07:19:23.000000 imviz-0.2.3/README.md
-drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2023-09-14 14:18:27.313630 imviz-0.2.3/imviz/
--rw-r--r--   0 ruof      (1000) ruof      (1000)     1677 2023-08-10 10:07:10.000000 imviz-0.2.3/imviz/__init__.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)     9627 2023-07-19 13:09:12.000000 imviz-0.2.3/imviz/autogui.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)     6200 2023-08-10 10:14:32.000000 imviz-0.2.3/imviz/common.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)     5573 2023-08-16 15:45:26.000000 imviz-0.2.3/imviz/dev.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1187 2023-08-16 15:45:00.000000 imviz-0.2.3/imviz/dev_main.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)    23863 2023-05-03 07:18:56.000000 imviz-0.2.3/imviz/export.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)       33 2023-08-10 10:09:11.000000 imviz-0.2.3/imviz/storage.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1824 2023-08-10 10:02:29.000000 imviz-0.2.3/imviz/task.py
-drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2023-09-14 14:18:27.313630 imviz-0.2.3/imviz.egg-info/
--rw-r--r--   0 ruof      (1000) ruof      (1000)     2467 2023-09-14 14:18:27.000000 imviz-0.2.3/imviz.egg-info/PKG-INFO
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      731 2023-09-14 14:18:27.000000 imviz-0.2.3/imviz.egg-info/SOURCES.txt
--rw-rw-r--   0 ruof      (1000) ruof      (1000)        1 2023-09-14 14:18:27.000000 imviz-0.2.3/imviz.egg-info/dependency_links.txt
--rw-rw-r--   0 ruof      (1000) ruof      (1000)        1 2023-09-14 14:18:27.000000 imviz-0.2.3/imviz.egg-info/not-zip-safe
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       56 2023-09-14 14:18:27.000000 imviz-0.2.3/imviz.egg-info/requires.txt
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       15 2023-09-14 14:18:27.000000 imviz-0.2.3/imviz.egg-info/top_level.txt
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      117 2023-08-14 12:34:08.000000 imviz-0.2.3/pyproject.toml
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       38 2023-09-14 14:18:27.317630 imviz-0.2.3/setup.cfg
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     4337 2023-09-14 14:17:12.000000 imviz-0.2.3/setup.py
-drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2023-09-14 14:18:27.317630 imviz-0.2.3/src/
--rw-r--r--   0 ruof      (1000) ruof      (1000)    10227 2023-07-13 12:09:10.000000 imviz-0.2.3/src/binding_helpers.cpp
--rw-r--r--   0 ruof      (1000) ruof      (1000)     5202 2023-07-13 12:10:22.000000 imviz-0.2.3/src/binding_helpers.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    14598 2023-07-19 11:30:12.000000 imviz-0.2.3/src/bindings.cpp
--rw-r--r--   0 ruof      (1000) ruof      (1000)    73895 2023-08-04 05:54:00.000000 imviz-0.2.3/src/bindings_imgui.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      146 2023-02-13 10:53:33.000000 imviz-0.2.3/src/bindings_imgui.hpp
--rw-r--r--   0 ruof      (1000) ruof      (1000)    36706 2023-08-12 07:57:26.000000 imviz-0.2.3/src/bindings_implot.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      125 2023-02-13 10:53:33.000000 imviz-0.2.3/src/bindings_implot.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     5856 2023-09-14 14:15:05.000000 imviz-0.2.3/src/file_dialog.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      204 2023-09-14 13:48:19.000000 imviz-0.2.3/src/file_dialog.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      123 2023-02-13 10:53:33.000000 imviz-0.2.3/src/im_user_config.h
--rw-r--r--   0 ruof      (1000) ruof      (1000)    11091 2023-08-13 08:48:45.000000 imviz-0.2.3/src/implot_ext.cpp
--rw-r--r--   0 ruof      (1000) ruof      (1000)      229 2023-08-12 08:08:48.000000 imviz-0.2.3/src/implot_ext.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     6680 2023-07-19 13:06:25.000000 imviz-0.2.3/src/imviz.cpp
--rw-r--r--   0 ruof      (1000) ruof      (1000)      979 2023-07-19 11:58:49.000000 imviz-0.2.3/src/imviz.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    17988 2023-02-13 10:53:33.000000 imviz-0.2.3/src/input.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1464 2023-02-13 10:53:33.000000 imviz-0.2.3/src/input.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)   558672 2023-02-13 10:53:33.000000 imviz-0.2.3/src/source_sans_pro.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       95 2023-02-13 10:53:33.000000 imviz-0.2.3/src/source_sans_pro.hpp
+drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-02 10:12:15.711217 imviz-0.2.4/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     5499 2024-05-02 10:00:45.000000 imviz-0.2.4/CMakeLists.txt
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1071 2024-05-02 10:00:45.000000 imviz-0.2.4/LICENSE
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)       61 2021-11-18 07:19:23.000000 imviz-0.2.4/MANIFEST.in
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     2410 2024-05-02 10:12:15.711217 imviz-0.2.4/PKG-INFO
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     2006 2024-05-02 10:00:45.000000 imviz-0.2.4/README.md
+drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-02 10:12:15.707217 imviz-0.2.4/imviz/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1677 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/__init__.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     9777 2024-05-02 10:00:53.000000 imviz-0.2.4/imviz/autogui.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     6200 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/common.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     5573 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/dev.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1187 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/dev_main.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    23863 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/export.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)       33 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/storage.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1824 2023-08-10 10:02:29.000000 imviz-0.2.4/imviz/task.py
+drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-02 10:12:15.711217 imviz-0.2.4/imviz.egg-info/
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     2410 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/PKG-INFO
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      731 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)        1 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)        1 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/not-zip-safe
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)       56 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/requires.txt
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)       15 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/top_level.txt
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      117 2024-05-02 09:40:07.000000 imviz-0.2.4/pyproject.toml
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)       38 2024-05-02 10:12:15.711217 imviz-0.2.4/setup.cfg
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     4337 2024-05-02 10:00:45.000000 imviz-0.2.4/setup.py
+drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-02 10:12:15.711217 imviz-0.2.4/src/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    10227 2024-05-02 09:40:07.000000 imviz-0.2.4/src/binding_helpers.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     5202 2024-05-02 09:40:07.000000 imviz-0.2.4/src/binding_helpers.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    14972 2024-05-02 10:00:45.000000 imviz-0.2.4/src/bindings.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    73814 2024-05-02 10:00:45.000000 imviz-0.2.4/src/bindings_imgui.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      146 2023-02-13 10:53:33.000000 imviz-0.2.4/src/bindings_imgui.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    36660 2024-05-02 10:00:45.000000 imviz-0.2.4/src/bindings_implot.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      125 2023-02-13 10:53:33.000000 imviz-0.2.4/src/bindings_implot.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     5856 2024-05-02 09:40:07.000000 imviz-0.2.4/src/file_dialog.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      204 2023-09-14 13:48:19.000000 imviz-0.2.4/src/file_dialog.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      159 2024-05-02 10:00:45.000000 imviz-0.2.4/src/im_user_config.h
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    11091 2024-05-02 09:40:07.000000 imviz-0.2.4/src/implot_ext.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      229 2024-05-02 09:40:07.000000 imviz-0.2.4/src/implot_ext.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    10847 2024-05-02 10:00:45.000000 imviz-0.2.4/src/imviz.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1116 2024-05-02 10:00:45.000000 imviz-0.2.4/src/imviz.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    17988 2023-02-13 10:53:33.000000 imviz-0.2.4/src/input.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1464 2023-02-13 10:53:33.000000 imviz-0.2.4/src/input.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)   558672 2023-02-13 10:53:33.000000 imviz-0.2.4/src/source_sans_pro.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)       95 2023-02-13 10:53:33.000000 imviz-0.2.4/src/source_sans_pro.hpp
```

### Comparing `imviz-0.2.3/CMakeLists.txt` & `imviz-0.2.4/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 cmake_minimum_required(VERSION 3.0)
 project(cppimviz)
 
 # Exports compile commands to .json file for vim YouCompleteMe support.
-
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 
+# Sometimes helps to find the right python version.
+set(PYBIND11_FINDPYTHON ON)
+
 set(PY_TARGET_NAME "${PROJECT_NAME}")
 
 # ---[ Check for OpenGL (mandatory) ]---
 
 set(OpenGL_GL_PREFERENCE GLVND)
 
 find_package(OpenGL QUIET)
@@ -27,33 +29,33 @@
 set(BUILD_STATIC_LIBS OFF CACHE BOOL "" FORCE)
 
 include(FetchContent)
 
 FetchContent_Declare(
     imgui
     GIT_REPOSITORY "https://github.com/ocornut/imgui"
-    GIT_TAG "c191faf0ba478e9c58a69c63306986a21ebfb6e4"
+    GIT_TAG "c6aa051629753f0ef0d26bf775a8b6a92aa213b2"
 )
 
 message(STATUS "Loading imgui ...")
 FetchContent_MakeAvailable(imgui)
 
 FetchContent_Declare(
     implot
     GIT_REPOSITORY "https://github.com/epezent/implot"
-    GIT_TAG "d87512353495e7760e7fda7566a05beef7627d8f"
+    GIT_TAG "f156599faefe316f7dd20fe6c783bf87c8bb6fd9"
 )
 
 message(STATUS "Loading implot ...")
 FetchContent_MakeAvailable(implot)
 
 FetchContent_Declare(
     pybind
     GIT_REPOSITORY "https://github.com/pybind/pybind11"
-    GIT_TAG "v2.10.0"
+    GIT_TAG "v2.11.1"
 )
 
 message(STATUS "Loading pybind ...")
 FetchContent_MakeAvailable(pybind)
 
 if(WIN32 OR APPLE)
 
@@ -188,13 +190,14 @@
                             -Wextra
                             -Wpedantic
                             -Wunreachable-code
                             -std=c++17)
 
     target_link_libraries(${PY_TARGET_NAME} PUBLIC
                             ${OPENGL_LIBRARIES}
+                            ${OPENGL_egl_LIBRARY}
                             ${GLEW_LIBRARIES}
                             stdc++fs
                             pybind11::module
                             glfw)
 
 endif()
```

### Comparing `imviz-0.2.3/LICENSE` & `imviz-0.2.4/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-2023 Jona Ruof
+Copyright (c) 2021-2024 Jona Ruof
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `imviz-0.2.3/PKG-INFO` & `imviz-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: imviz
-Version: 0.2.3
+Version: 0.2.4
 Summary: Pythonic bindings for imgui/implot
 Home-page: https://github.com/joruof/imviz
 Author: Jona Ruof
 Author-email: jona.ruof@uni-ulm.de
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: Pillow>=9.0.1
 Requires-Dist: objtoolbox>=0.0.9
 Requires-Dist: minireload>=0.0.5
 
 # imviz
 
 Pythonic bindings for the great [imgui](https://github.com/ocornut/imgui) and
 [implot](https://github.com/epezent/implot) libraries.
 
-**This is work in progress and at a very early state.**
-
 ## What?
 
 The goal of this project is to create bindings, which map the immediate mode
 gui paradigm in a pythonic way, so that writing GUIs in python (especially
 visualization heavy ones, meaning plots and stuff) becomes easy.
 
 ## Why?
@@ -51,15 +49,15 @@
 [pybind11](https://github.com/pybind/pybind11).
 
 ## Installation
 
 OpenGL libraries, GLFW, and GLEW are mandatory dependencies and are expected
 to be installed on the system.
 
-On Ubuntu 20.04 OpenGL libraries are already installed and GLFW, GLEW can be
+On Ubuntu 22.04 OpenGL libraries are already installed and GLFW, GLEW can be
 installed with:
 
 ```
 sudo apt-get install -y libglfw3-dev
 sudo apt-get install -y libglew-dev
 ```
```

### Comparing `imviz-0.2.3/README.md` & `imviz-0.2.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # imviz
 
 Pythonic bindings for the great [imgui](https://github.com/ocornut/imgui) and
 [implot](https://github.com/epezent/implot) libraries.
 
-**This is work in progress and at a very early state.**
-
 ## What?
 
 The goal of this project is to create bindings, which map the immediate mode
 gui paradigm in a pythonic way, so that writing GUIs in python (especially
 visualization heavy ones, meaning plots and stuff) becomes easy.
 
 ## Why?
@@ -35,15 +33,15 @@
 [pybind11](https://github.com/pybind/pybind11).
 
 ## Installation
 
 OpenGL libraries, GLFW, and GLEW are mandatory dependencies and are expected
 to be installed on the system.
 
-On Ubuntu 20.04 OpenGL libraries are already installed and GLFW, GLEW can be
+On Ubuntu 22.04 OpenGL libraries are already installed and GLFW, GLEW can be
 installed with:
 
 ```
 sudo apt-get install -y libglfw3-dev
 sudo apt-get install -y libglew-dev
 ```
```

### Comparing `imviz-0.2.3/imviz/__init__.py` & `imviz-0.2.4/imviz/__init__.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/imviz/autogui.py` & `imviz-0.2.4/imviz/autogui.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,16 @@
 
         if hasattr(obj, "__dict__"):
             attr_dict = obj.__dict__
         elif hasattr(obj, "__slots__"):
             attr_dict = {n: getattr(obj, n) for n in obj.__slots__}
         elif isinstance(obj, dict):
             attr_dict = obj
+        elif isinstance(obj, set):
+            attr_dict = {i: n for i, n in enumerate(obj)}
         elif hasattr(obj, "__len__") and hasattr(obj, "__getitem__"):
             if tree_open:
                 for i in range(len(obj)):
 
                     self.post_header_hooks.append(list_item_context)
 
                     self.path.append(i)
@@ -262,14 +264,16 @@
             if len(name) > 0 and tree_open:
                 viz.tree_pop()
 
             return obj
         else:
             if len(name) == 0:
                 viz.text(f"{name}: " + "???")
+            if tree_open:
+                viz.tree_pop()
             return obj
 
         obj_annots = getattr(obj, "__annotations__", {})
     
         # default case: generic object
 
         if tree_open:
```

### Comparing `imviz-0.2.3/imviz/common.py` & `imviz-0.2.4/imviz/common.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/imviz/dev.py` & `imviz-0.2.4/imviz/dev.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/imviz/dev_main.py` & `imviz-0.2.4/imviz/dev_main.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/imviz/export.py` & `imviz-0.2.4/imviz/export.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/imviz/task.py` & `imviz-0.2.4/imviz/task.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/imviz.egg-info/PKG-INFO` & `imviz-0.2.4/imviz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: imviz
-Version: 0.2.3
+Version: 0.2.4
 Summary: Pythonic bindings for imgui/implot
 Home-page: https://github.com/joruof/imviz
 Author: Jona Ruof
 Author-email: jona.ruof@uni-ulm.de
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: Pillow>=9.0.1
 Requires-Dist: objtoolbox>=0.0.9
 Requires-Dist: minireload>=0.0.5
 
 # imviz
 
 Pythonic bindings for the great [imgui](https://github.com/ocornut/imgui) and
 [implot](https://github.com/epezent/implot) libraries.
 
-**This is work in progress and at a very early state.**
-
 ## What?
 
 The goal of this project is to create bindings, which map the immediate mode
 gui paradigm in a pythonic way, so that writing GUIs in python (especially
 visualization heavy ones, meaning plots and stuff) becomes easy.
 
 ## Why?
@@ -51,15 +49,15 @@
 [pybind11](https://github.com/pybind/pybind11).
 
 ## Installation
 
 OpenGL libraries, GLFW, and GLEW are mandatory dependencies and are expected
 to be installed on the system.
 
-On Ubuntu 20.04 OpenGL libraries are already installed and GLFW, GLEW can be
+On Ubuntu 22.04 OpenGL libraries are already installed and GLFW, GLEW can be
 installed with:
 
 ```
 sudo apt-get install -y libglfw3-dev
 sudo apt-get install -y libglew-dev
 ```
```

### Comparing `imviz-0.2.3/imviz.egg-info/SOURCES.txt` & `imviz-0.2.4/imviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/setup.py` & `imviz-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,24 +115,24 @@
             for m in matches:
                 binary_files.append(m)
                 if not is_wheel:
                     self.copy_file(m, dest_dir / m.name) # tmp => lib
 
 
 setup(name="imviz",
-      version="0.2.3",
+      version="0.2.4",
       description="Pythonic bindings for imgui/implot",
       url="https://github.com/joruof/imviz",
       author="Jona Ruof",
       author_email="jona.ruof@uni-ulm.de",
       license="MIT",
       zip_safe=False,
       long_description=Path('README.md').read_text('utf-8'),
       long_description_content_type="text/markdown",
-      python_requires=">=3.6",
+      python_requires=">=3.8",
       packages=find_packages(),
       ext_modules=[CMakeExtension("cppimviz")],
       cmdclass=dict(build_ext=CMakeBuild, install=Install),
       include_package_data=True,
       install_requires=[
             "numpy", "Pillow>=9.0.1", "objtoolbox>=0.0.9", "minireload>=0.0.5"
           ]
```

### Comparing `imviz-0.2.3/src/binding_helpers.cpp` & `imviz-0.2.4/src/binding_helpers.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/src/binding_helpers.hpp` & `imviz-0.2.4/src/binding_helpers.hpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/src/bindings.cpp` & `imviz-0.2.4/src/bindings.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 #include <pybind11/pytypes.h>
 #include <stdexcept>
 
 #include <GL/glew.h>
 
 #include "implot.h"
 #include "implot_internal.h"
-
 #include "im_user_config.h"
 
 #include "imviz.hpp"
 #include "input.hpp"
 #include "file_dialog.hpp"
 #include "binding_helpers.hpp"
 #include "bindings_implot.hpp"
@@ -45,79 +44,88 @@
     loadImplotPythonBindings(m, viz);
 
     /**
      * GLFW functions
      */
 
     m.def("set_main_window_title", [&](std::string title) {
-        glfwSetWindowTitle(viz.window, title.c_str());
+        if (nullptr != viz.window) {
+            glfwSetWindowTitle(viz.window, title.c_str());
+        }
     },
     py::arg("title"));
 
     m.def("set_main_window_size", [&](ImVec2 size) {
-        glfwSetWindowSize(viz.window, size.x, size.y);
+        viz.setWindowSize(size);
     },
     py::arg("size"));
 
+    m.def("get_main_window_size", [&]() {
+        return viz.getWindowSize();
+    });
+
     m.def("enter_fullscreen", [&]() {
 
         GLFWmonitor* monitor = glfwGetPrimaryMonitor();
         const GLFWvidmode* mode = glfwGetVideoMode(monitor);
 
-        glfwSetWindowMonitor(viz.window, monitor,
-                             0, 0,
-                             mode->width, mode->height,
-                             mode->refreshRate);
+        if (nullptr != viz.window) {
+            glfwSetWindowMonitor(viz.window, monitor,
+                                 0, 0,
+                                 mode->width, mode->height,
+                                 mode->refreshRate);
+        }
     });
 
     m.def("leave_fullscreen", [&]() {
-        glfwSetWindowMonitor(viz.window, nullptr, 0, 0, 800, 600, 0);
-    });
-
-    m.def("get_main_window_size", [&]() {
-        int w, h;
-        glfwGetWindowSize(viz.window, &w, &h);
-        return ImVec2(w, h);
+        if (nullptr != viz.window) {
+            glfwSetWindowMonitor(viz.window, nullptr, 0, 0, 800, 600, 0);
+        }
     });
 
     m.def("set_main_window_pos", [&](ImVec2 pos) {
-        glfwSetWindowPos(viz.window, pos.x, pos.y);
+        if (nullptr != viz.window) {
+            glfwSetWindowPos(viz.window, pos.x, pos.y);
+        }
     },
     py::arg("size"));
 
     m.def("get_main_window_pos", [&]() {
-        int x, y;
-        glfwGetWindowPos(viz.window, &x, &y);
+        int x = 0;
+        int y = 0;
+        if (nullptr != viz.window) {
+            glfwGetWindowPos(viz.window, &x, &y);
+        }
         return ImVec2(x, y);
     });
 
-    m.def("get_main_window_size", [&]() {
-        int w, h;
-        glfwGetWindowSize(viz.window, &w, &h);
-        return ImVec2(w, h);
-    });
-
     m.def("hide_main_window", [&]() {
-        glfwHideWindow(viz.window);
+        if (nullptr != viz.window) {
+            glfwHideWindow(viz.window);
+        }
     });
 
     m.def("show_main_window", [&]() {
-        glfwShowWindow(viz.window);
+        if (nullptr != viz.window) {
+            glfwShowWindow(viz.window);
+        }
     });
 
     m.def("set_main_window_icon", [&](array_like<uint8_t> icon) {
 
         assert_shape(icon, {{-1, -1, 4}});
 
         GLFWimage img;
         img.height = icon.shape(0);
         img.width = icon.shape(1);
         img.pixels = icon.mutable_data();
 
-        glfwSetWindowIcon(viz.window, 1, &img);
+        if (nullptr != viz.window) {
+            glfwSetWindowIcon(viz.window, 1, &img);
+        }
     },
     R"raw(
     This sets the icon of the main window shown in e.g. taskbars.
     The *icon* must be an RGBA image given as an array_like with shape (-1, -1, 4).
     )raw", 
     py::arg("icon"));
 
@@ -400,15 +408,19 @@
             // reconfigure and load ini
             ImGuiIO& io = ImGui::GetIO();
             io.IniFilename = viz.iniFilePath.c_str();
             ImGui::LoadIniSettingsFromDisk(io.IniFilename);
 
             viz.prepareUpdate();
 
-            return !glfwWindowShouldClose(viz.window);
+            if (viz.window != nullptr) {
+                return !glfwWindowShouldClose(viz.window);
+            } else {
+                return true;
+            }
         }
 
         input::update();
 
         if (powersave) {
             if (viz.powerSaveFrameCounter > 0) {
                 glfwPollEvents();
@@ -418,15 +430,18 @@
                 viz.powerSaveFrameCounter = 5;
             }
         } else {
             glfwPollEvents();
         }
 
         viz.prepareUpdate();
-        return !glfwWindowShouldClose(viz.window);
+        if (viz.window != nullptr) {
+            return !glfwWindowShouldClose(viz.window);
+        }
+        return true;
     },
     R"raw(
     This is the main update function of imviz.
     It must be called once for each frame/update/tick of the application.
 
     It is typically called as the condition for the main while loop of
     the application. Like so:
@@ -453,16 +468,15 @@
      * Image export
      */
 
     m.def("get_pixels", [&](int x, int y, int width, int height) {
 
         py::array_t<uint8_t> pixels({height, width, 4});
 
-        int w, h;
-        glfwGetWindowSize(viz.window, &w, &h);
+        int h = (int)viz.getWindowSize().y;
 
         glReadPixels(
                 x, h - y - height,
                 width, height,
                 GL_RGBA,
                 GL_UNSIGNED_BYTE,
                 pixels.mutable_data());
```

### Comparing `imviz-0.2.3/src/bindings_imgui.cpp` & `imviz-0.2.4/src/bindings_imgui.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 #include "bindings_implot.hpp"
-
 #include "binding_helpers.hpp"
 #include "imviz.hpp"
-#include <pybind11/pybind11.h>
 
 #define _USE_MATH_DEFINES
 #include <cmath>
-#include <imgui.h>
-#include <pybind11/pytypes.h>
 #include <sstream>
 #include <iomanip>
 
-#ifndef IMGUI_DEFINE_MATH_OPERATORS
-#define IMGUI_DEFINE_MATH_OPERATORS
-#endif
+#include <pybind11/pytypes.h>
+#include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
 
+#include "imgui.h"
 #include "imgui_internal.h"
 #include "implot_internal.h"
 #include "misc/cpp/imgui_stdlib.h"
 
-#include "pybind11/stl.h"
-
 static py::object dragDropRef = py::none();
 static int dragDropClearCounter = 0;
 
 namespace ImPlot {
 
     double PreciseAxisPlotToPixels (ImPlotAxis& axs, double plt) {
```

### Comparing `imviz-0.2.3/src/bindings_implot.cpp` & `imviz-0.2.4/src/bindings_implot.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #include "bindings_implot.hpp"
 
 #include "binding_helpers.hpp"
 #include "imviz.hpp"
 
 #define _USE_MATH_DEFINES
 #include <cmath>
-#include "implot_internal.h"
-#include "implot_ext.hpp"
-#include <imgui.h>
-#include <implot.h>
+
 #include <pybind11/pytypes.h>
 #include <pybind11/stl.h>
 
+#include "imgui.h"
+#include "implot.h"
+#include "implot_internal.h"
+#include "implot_ext.hpp"
+
 
 void loadImplotPythonBindings(pybind11::module& m, ImViz& viz) {
 
     /**
      * Flags and defines
      */
 
@@ -31,15 +33,14 @@
         .value("NONE", ImPlotFlags_None)
         .value("NO_TITLE", ImPlotFlags_NoTitle)
         .value("NO_LEGEND", ImPlotFlags_NoLegend)
         .value("NO_MOUSE_TEXT", ImPlotFlags_NoMouseText)
         .value("NO_INPUTS", ImPlotFlags_NoInputs)
         .value("NO_MENUS", ImPlotFlags_NoMenus)
         .value("NO_BOX_SELECT", ImPlotFlags_NoBoxSelect)
-        .value("NO_CHILD", ImPlotFlags_NoChild)
         .value("EQUAL", ImPlotFlags_Equal)
         .value("CROSSHAIRS", ImPlotFlags_Crosshairs)
         .value("CANVAS_ONLY", ImPlotFlags_CanvasOnly);
 
     py::enum_<ImPlotItemFlags_>(m, "PlotItemFlags", py::arithmetic())
         .value("NONE", ImPlotItemFlags_None)
         .value("NO_FIT", ImPlotItemFlags_NoFit)
```

### Comparing `imviz-0.2.3/src/file_dialog.cpp` & `imviz-0.2.4/src/file_dialog.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/src/implot_ext.cpp` & `imviz-0.2.4/src/implot_ext.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/src/imviz.hpp` & `imviz-0.2.4/src/imviz.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     GLFWwindow* window = nullptr;
 
     ImGuiContext* imGuiCtx = nullptr;
     ImPlotContext* imPlotCtx = nullptr;
 
     ImFont* smallFont = nullptr;
     ImFont* largeFont = nullptr;
-    double fontBaseSize = 20.0;
+    float fontBaseSize = 20.0;
 
     ImGuiID mainDockSpaceId;
 
     bool currentWindowOpen = false;
     bool figurePlotOpen = false;
 
     bool plotPopupOpen = false;
@@ -43,8 +43,16 @@
     void prepareUpdate();
     void reloadFonts();
     void setupImLibs();
     void doUpdate(bool useVsync);
     void recover();
     void trigger();
     void setMod(bool m);
+
+    void setWindowSize(ImVec2 size);
+    ImVec2 getWindowSize();
+
+private:
+
+    int eglWindowWidth = 800;
+    int eglWindowHeight = 600;
 };
```

### Comparing `imviz-0.2.3/src/input.cpp` & `imviz-0.2.4/src/input.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/src/input.hpp` & `imviz-0.2.4/src/input.hpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.3/src/source_sans_pro.cpp` & `imviz-0.2.4/src/source_sans_pro.cpp`

 * *Files identical despite different names*

