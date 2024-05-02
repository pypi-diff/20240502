# Comparing `tmp/pyircsdk-1.0.2.tar.gz` & `tmp/pyircsdk-1.1.0.tar.gz`

## Comparing `pyircsdk-1.0.2.tar` & `pyircsdk-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/pyircsdk/__about__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/pyircsdk/__init__.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/pyircsdk/command.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/pyircsdk/message.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/pyircsdk/pyircsdk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/pyircsdk/event/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/pyircsdk/event/event.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/LICENSE
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/README.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/__about__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/command.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/message.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/pyircsdk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/event/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/event/event.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/README.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/PKG-INFO
```

### Comparing `pyircsdk-1.0.2/pyircsdk/command.py` & `pyircsdk-1.1.0/pyircsdk/command.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,28 @@
     def __init__(self, irc, fantasy, command):
         self.irc = irc
         self.command = command
         self.fantasy = fantasy
 
     def startListening(self):
         self.irc.event.on('message', lambda x: print(x.command, x.messageFrom, x.messageTo, x.message))
-        self.irc.event.on('message', lambda x: self.handleCommand(x, self.messageToCommandWithArgs(x)))
+        self.irc.event.on('message', lambda x: self.handleMessage(x))
+
+    def handleMessage(self, x):
+        try:
+            self.handleCommand(x, self.messageToCommandWithArgs(x))
+        except Exception as e:
+            self.handleError(x, self.messageToCommandWithArgs(x), e)
 
     def messageToCommandWithArgs(self, message):
         command = Command()
         if message is not None and message.message is not None:
             return command.parse(message.message.split(' '))
-        return command
+            return command
 
     @abstractmethod
     def handleCommand(self, message, command):
         pass
+
+    @abstractmethod
+    def handleError(self, message, command, error):
+        pass
```

### Comparing `pyircsdk-1.0.2/pyircsdk/message.py` & `pyircsdk-1.1.0/pyircsdk/message.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.0.2/pyircsdk/pyircsdk.py` & `pyircsdk-1.1.0/pyircsdk/pyircsdk.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.0.2/pyircsdk/event/event.py` & `pyircsdk-1.1.0/pyircsdk/event/event.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.0.2/.gitignore` & `pyircsdk-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.0.2/LICENSE` & `pyircsdk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.0.2/README.md` & `pyircsdk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.0.2/pyproject.toml` & `pyircsdk-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "pyircsdk"
 authors = [
   { name="Bludot", email="admin@floretos.com" },
 ]
-version = "1.0.2"
+version = "1.1.0"
 description = "pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyircsdk-1.0.2/PKG-INFO` & `pyircsdk-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyircsdk
-Version: 1.0.2
+Version: 1.1.0
 Summary: pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages.
 Project-URL: Homepage, https://github.com/bludot/pyircsdk
 Project-URL: Issues, https://github.com/bludot/pyircsdk/issues
 Author-email: Bludot <admin@floretos.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

