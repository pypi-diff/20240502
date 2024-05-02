# Comparing `tmp/reflex_wrapper-0.0.1.tar.gz` & `tmp/reflex_wrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_wrapper-0.0.1.tar", last modified: Thu May  2 13:25:59 2024, max compression
+gzip compressed data, was "reflex_wrapper-0.0.2.tar", last modified: Thu May  2 19:00:57 2024, max compression
```

## Comparing `reflex_wrapper-0.0.1.tar` & `reflex_wrapper-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-02 13:25:59.588674 reflex_wrapper-0.0.1/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1073 2024-05-01 15:13:57.000000 reflex_wrapper-0.0.1/LICENSE
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     2917 2024-05-02 13:25:59.588674 reflex_wrapper-0.0.1/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     2369 2024-05-02 13:12:38.000000 reflex_wrapper-0.0.1/README.md
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-02 13:25:59.588674 reflex_wrapper-0.0.1/reflex_wrapper/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       26 2024-05-02 13:04:35.000000 reflex_wrapper-0.0.1/reflex_wrapper/__init__.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    11389 2024-05-02 13:16:39.000000 reflex_wrapper-0.0.1/reflex_wrapper/rx_wrapper.py
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-02 13:25:59.588674 reflex_wrapper-0.0.1/reflex_wrapper.egg-info/
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     2917 2024-05-02 13:25:59.000000 reflex_wrapper-0.0.1/reflex_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      271 2024-05-02 13:25:59.000000 reflex_wrapper-0.0.1/reflex_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-05-02 13:25:59.000000 reflex_wrapper-0.0.1/reflex_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       14 2024-05-02 13:25:59.000000 reflex_wrapper-0.0.1/reflex_wrapper.egg-info/requires.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       15 2024-05-02 13:25:59.000000 reflex_wrapper-0.0.1/reflex_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-05-02 13:25:59.588674 reflex_wrapper-0.0.1/setup.cfg
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      788 2024-05-01 15:52:12.000000 reflex_wrapper-0.0.1/setup.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-02 19:00:57.876110 reflex_wrapper-0.0.2/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1073 2024-05-01 15:13:57.000000 reflex_wrapper-0.0.2/LICENSE
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     3876 2024-05-02 19:00:57.876110 reflex_wrapper-0.0.2/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3328 2024-05-02 15:35:19.000000 reflex_wrapper-0.0.2/README.md
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-02 19:00:57.876110 reflex_wrapper-0.0.2/reflex_wrapper/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       26 2024-05-02 13:04:35.000000 reflex_wrapper-0.0.2/reflex_wrapper/__init__.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    11393 2024-05-02 18:59:39.000000 reflex_wrapper-0.0.2/reflex_wrapper/rx_wrapper.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-02 19:00:57.876110 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     3876 2024-05-02 19:00:57.000000 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      271 2024-05-02 19:00:57.000000 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-05-02 19:00:57.000000 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       14 2024-05-02 19:00:57.000000 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       15 2024-05-02 19:00:57.000000 reflex_wrapper-0.0.2/reflex_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-05-02 19:00:57.876110 reflex_wrapper-0.0.2/setup.cfg
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      788 2024-05-02 19:00:44.000000 reflex_wrapper-0.0.2/setup.py
```

### Comparing `reflex_wrapper-0.0.1/LICENSE` & `reflex_wrapper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_wrapper-0.0.1/PKG-INFO` & `reflex_wrapper-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-Metadata-Version: 2.1
-Name: reflex_wrapper
-Version: 0.0.1
-Summary: A custom wrapper on top of the reflex library to ease creating and interacting with custom components.
-Home-page: https://github.com/B4PT0R/reflex_wrapper
-Author: Baptiste Ferrand
-Author-email: bferrand.maths@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: reflex>=0.4.8
-
 # reflex-wrapper
 
-`reflex-wrapper` is a Python module that provides a wrapper on top of the reflex library to ease creating custom components as well as adding syntactic sugar to setup and interact with components after they are instantiated. It is meant to be "without loss", meaning that all that was possible to achieve with reflex is still possible using the wrapper, and as easily or more.
+`reflex-wrapper` is a Python module that provides a wrapper on top of the reflex library. It mostly behaves just like the reflex module, but simplifies the public API to make creating custom components more user-friendly. The idea behind this wrapper was that, in reflex, States are pydantic models (classes) who are only instantiated per-session by the server itself. This means that you never should instantiate a state classes directly in your reflex code. As a matter of fact, what would be considered "instances" of a State in reflex are actualy subclasses of an initial pydantic rx.State class (but still classes!).
+This design choice, while being very elegant on a technical point of view for input validation and multi-session state management, also made the objet model less intuitive to a regular python developper, who expects to create 3 independant stateful components by instantiating the component class three times and that's it. To work around this, I created a custom Component class that abstracts away these pydantic state shenanigans and allows to use reflex components as normal instances of their Component subclass. 
+
+All standard reflex components are also automatically converted into Component objects so that you don't have to think about it and just focus on creating your app.
 
 ## Installation
 
 ```bash
 pip install reflex-wrapper
 ```
 
@@ -31,15 +19,15 @@
 # Define a custom component by subclassing the rx.Component class
 
 class Counter(rx.Component):
 
     count: int = 0
 
     @rx.var
-    def double_count(self):
+    def twice_the_count(self):
         return 2*self.count
 
     def increment(self):
         self.count += 1
 
     def decrement(self):
         self.count -= 1
@@ -64,21 +52,21 @@
 
 @rx.page() # Decorators still work
 def index():
     cnt=Counter(count=10,background='blue') # we can intialize the count state value directly from props
     cnt.count=5
     cnt.background='green' # we can also edit via attribute style access after instantiation
     btn1=rx.button("Click to add 2",on_click=cnt.set_count(cnt.count+2)) # we can use state setters like this
-    cnt2=Counter(count=cnt.double_count) # we can link a second counter's state to the first's, thus synchronizing their states.
+    cnt2=Counter(count=cnt.twice_the_count) # we can link a second counter's state to some state var of the first, thus synchronizing the second counter. 
     box=rx.box(
         cnt,
         cnt2
         btn1,
     )
     return box
 
 app=rx.App()
 ```
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `reflex_wrapper-0.0.1/reflex_wrapper/rx_wrapper.py` & `reflex_wrapper-0.0.2/reflex_wrapper/rx_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
     """
     Meta class to override __getattr__ in the RX class
     Does the routing to the appropriate object
     """
 
     def __getattr__(cls, key):
         if key in cls._reserved:
-            return getattr(rx,key)
+            return getattr(reflex,key)
         elif key in cls._submodules:
             return rx_submodule(key)
         elif key in globals():
             return globals()[key]
         elif key in cls._dict:
             return cls._dict[key]
         elif hasattr(reflex,key):
```

### Comparing `reflex_wrapper-0.0.1/reflex_wrapper.egg-info/PKG-INFO` & `reflex_wrapper-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: reflex_wrapper
-Version: 0.0.1
+Version: 0.0.2
 Summary: A custom wrapper on top of the reflex library to ease creating and interacting with custom components.
 Home-page: https://github.com/B4PT0R/reflex_wrapper
 Author: Baptiste Ferrand
 Author-email: bferrand.maths@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: reflex>=0.4.8
 
 # reflex-wrapper
 
-`reflex-wrapper` is a Python module that provides a wrapper on top of the reflex library to ease creating custom components as well as adding syntactic sugar to setup and interact with components after they are instantiated. It is meant to be "without loss", meaning that all that was possible to achieve with reflex is still possible using the wrapper, and as easily or more.
+`reflex-wrapper` is a Python module that provides a wrapper on top of the reflex library. It mostly behaves just like the reflex module, but simplifies the public API to make creating custom components more user-friendly. The idea behind this wrapper was that, in reflex, States are pydantic models (classes) who are only instantiated per-session by the server itself. This means that you never should instantiate a state classes directly in your reflex code. As a matter of fact, what would be considered "instances" of a State in reflex are actualy subclasses of an initial pydantic rx.State class (but still classes!).
+This design choice, while being very elegant on a technical point of view for input validation and multi-session state management, also made the objet model less intuitive to a regular python developper, who expects to create 3 independant stateful components by instantiating the component class three times and that's it. To work around this, I created a custom Component class that abstracts away these pydantic state shenanigans and allows to use reflex components as normal instances of their Component subclass. 
+
+All standard reflex components are also automatically converted into Component objects so that you don't have to think about it and just focus on creating your app.
 
 ## Installation
 
 ```bash
 pip install reflex-wrapper
 ```
 
@@ -31,15 +34,15 @@
 # Define a custom component by subclassing the rx.Component class
 
 class Counter(rx.Component):
 
     count: int = 0
 
     @rx.var
-    def double_count(self):
+    def twice_the_count(self):
         return 2*self.count
 
     def increment(self):
         self.count += 1
 
     def decrement(self):
         self.count -= 1
@@ -64,15 +67,15 @@
 
 @rx.page() # Decorators still work
 def index():
     cnt=Counter(count=10,background='blue') # we can intialize the count state value directly from props
     cnt.count=5
     cnt.background='green' # we can also edit via attribute style access after instantiation
     btn1=rx.button("Click to add 2",on_click=cnt.set_count(cnt.count+2)) # we can use state setters like this
-    cnt2=Counter(count=cnt.double_count) # we can link a second counter's state to the first's, thus synchronizing their states.
+    cnt2=Counter(count=cnt.twice_the_count) # we can link a second counter's state to some state var of the first, thus synchronizing the second counter. 
     box=rx.box(
         cnt,
         cnt2
         btn1,
     )
     return box
```

### Comparing `reflex_wrapper-0.0.1/setup.py` & `reflex_wrapper-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="reflex_wrapper",
-    version="0.0.1",
+    version="0.0.2",
     author="Baptiste Ferrand",
     author_email="bferrand.maths@gmail.com",
     description="A custom wrapper on top of the reflex library to ease creating and interacting with custom components.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/B4PT0R/reflex_wrapper",
     packages=setuptools.find_packages(),
```

