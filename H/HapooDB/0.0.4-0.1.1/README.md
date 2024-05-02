# Comparing `tmp/HapooDB-0.0.4.tar.gz` & `tmp/HapooDB-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HapooDB-0.0.4.tar", last modified: Sat Apr 27 09:47:08 2024, max compression
+gzip compressed data, was "HapooDB-0.1.1.tar", last modified: Thu May  2 14:11:08 2024, max compression
```

## Comparing `HapooDB-0.0.4.tar` & `HapooDB-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 09:47:08.587703 HapooDB-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-04-27 09:47:08.569751 HapooDB-0.0.4/HapooDB/
--rw-rw-rw-   0        0        0     4460 2024-04-27 09:16:01.000000 HapooDB-0.0.4/HapooDB/HapooDB.py
--rw-rw-rw-   0        0        0       28 2024-04-27 08:41:15.000000 HapooDB-0.0.4/HapooDB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 09:47:08.584711 HapooDB-0.0.4/HapooDB.egg-info/
--rw-rw-rw-   0        0        0      478 2024-04-27 09:47:08.000000 HapooDB-0.0.4/HapooDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-04-27 09:47:08.000000 HapooDB-0.0.4/HapooDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 09:47:08.000000 HapooDB-0.0.4/HapooDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 09:47:08.000000 HapooDB-0.0.4/HapooDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1299 2024-04-27 09:31:12.000000 HapooDB-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      478 2024-04-27 09:47:08.586706 HapooDB-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      493 2024-04-27 09:31:38.000000 HapooDB-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 09:47:08.587703 HapooDB-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      699 2024-04-27 09:46:47.000000 HapooDB-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 14:11:08.770538 HapooDB-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-02 14:11:08.744606 HapooDB-0.1.1/HapooDB/
+-rw-rw-rw-   0        0        0     5033 2024-05-02 14:08:34.000000 HapooDB-0.1.1/HapooDB/HapooDB.py
+-rw-rw-rw-   0        0        0       28 2024-04-27 08:41:15.000000 HapooDB-0.1.1/HapooDB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 14:11:08.766548 HapooDB-0.1.1/HapooDB.egg-info/
+-rw-rw-rw-   0        0        0      478 2024-05-02 14:11:08.000000 HapooDB-0.1.1/HapooDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2024-05-02 14:11:08.000000 HapooDB-0.1.1/HapooDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 14:11:08.000000 HapooDB-0.1.1/HapooDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 14:11:08.000000 HapooDB-0.1.1/HapooDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1299 2024-04-27 09:31:12.000000 HapooDB-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      478 2024-05-02 14:11:08.768544 HapooDB-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-04-27 09:31:38.000000 HapooDB-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 14:11:08.770538 HapooDB-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      699 2024-05-02 14:08:52.000000 HapooDB-0.1.1/setup.py
```

### Comparing `HapooDB-0.0.4/HapooDB/HapooDB.py` & `HapooDB-0.1.1/HapooDB/HapooDB.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import os
 
+
+
 class HapooDB:
+
+
     def __init__(self,*title) -> None:
         self.variables = []
         if title:
             self.filename = f"{title[0]}.txt"
         else:
             self.filename = f"HapooDB.txt"
         try:
@@ -14,49 +18,51 @@
 
             except IndexError:
                 with open(self.filename,"xt") as file:
                     pass
         except FileExistsError: 
             pass
 
+    
     def destroyfile(self) -> None:
         if os.path.exists(self.filename):
             os.remove(self.filename)
         else:
             print("!The file, {} does not exist".format(self.filename))
 
-
     def declare(self, key, val):
         with open(self.filename, "at") as self.file:
             self.file.write(f"{key}={val}\n")
 
     def access(self) -> dict:
         with  open(self.filename,"rt") as self.file:
             lines = [line.strip("\n") for line in self.file.readlines()]
             variables = {}
             for line in lines:
                 line = [element for element in line.split("=")]
                 variables[line[0]] = line[1]
             return variables  
       
     def accessSingle(self,key) -> str:
+        key = str(key)
         with open(self.filename,"rt") as self.file:
             lines = [line.strip("\n") for line in self.file.readlines()]
             val = None
             for line in lines:
                 if key in line:
                     val = line.split("=")[1]
                     break
                 else:
                     continue
             try:
                 return val.strip("\n")         
            
             except AttributeError:
                 print("!There is no such of key in the DB.")
+                return None
 
 
     def declareCluster(self,keyValPair:dict) -> None:
         with open(self.filename,"at") as self.file:
             content = list(keyValPair.items())
             for branchlist in content:
                 self.file.write(f"{branchlist[0]}={branchlist[1]}\n")   
@@ -89,15 +95,14 @@
                 return self.__private_Decrypt(val.strip("\n"))
             except AttributeError:
                 print("!There is no such of key in the DB.")
         ##todo
     def changeValue(self,key,changingValue):
         with open(self.filename,"rt") as self.file:
             lines = [line for line in self.file.readlines()]
-        print(lines)
         for index,line in enumerate(lines):
             if key in line:
                 indexOfLine = index
                 break
         lines[indexOfLine] = f"{key}={changingValue}\n"
         with open(self.filename, "w") as file: 
             file.write("".join(lines))  
@@ -120,8 +125,25 @@
         for letter in val:
             if letter in val:
                 index = alphabets.index(letter)
                 newPosition = (index - 3) % 62
                 EncodedMsg.append(alphabets[newPosition])
             else:
                 EncodedMsg.append(letter)
-        return "".join(EncodedMsg)
+        return "".join(EncodedMsg)
+    
+    def Listen(self):
+        _all_ =["DECLARE","ACCESS_SINGLE","QUIT"]
+        print(_all_)
+
+        while True:
+            choice = input()
+            choice = choice.split(" ")
+            print(choice)
+            if (x:=choice[0].upper()) == "DECLARE":
+                self.declare(choice[1],choice[2])
+                print(self.file.closed)
+            elif x == "ACCESS_SINGLE":
+                print(self.accessSingle(choice[1]))
+            elif x == "QUIT":
+                break
+
```

### Comparing `HapooDB-0.0.4/LICENSE.txt` & `HapooDB-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `HapooDB-0.0.4/setup.py` & `HapooDB-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.1.1'
 DESCRIPTION = 'Hapoo DB'
 
 
 # Setting up
 setup(
     name="HapooDB",
     version=VERSION,
```

