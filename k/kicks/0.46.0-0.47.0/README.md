# Comparing `tmp/kicks-0.46.0.tar.gz` & `tmp/kicks-0.47.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicks-0.46.0.tar", last modified: Thu May  2 17:40:39 2024, max compression
+gzip compressed data, was "kicks-0.47.0.tar", last modified: Thu May  2 17:42:34 2024, max compression
```

## Comparing `kicks-0.46.0.tar` & `kicks-0.47.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:40:39.204434 kicks-0.46.0/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.46.0/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:40:39.204256 kicks-0.46.0/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.46.0/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      603 2024-05-02 17:40:37.000000 kicks-0.46.0/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-02 17:40:39.204482 kicks-0.46.0/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:40:39.202398 kicks-0.46.0/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:40:39.203040 kicks-0.46.0/src/kicks/
--rw-r--r--   0 robertdegen   (501) staff       (20)    19902 2024-05-02 17:40:06.000000 kicks-0.46.0/src/kicks/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:40:39.204089 kicks-0.46.0/src/kicks.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:40:39.000000 kicks-0.46.0/src/kicks.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      218 2024-05-02 17:40:39.000000 kicks-0.46.0/src/kicks.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-02 17:40:39.000000 kicks-0.46.0/src/kicks.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       24 2024-05-02 17:40:39.000000 kicks-0.46.0/src/kicks.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        6 2024-05-02 17:40:39.000000 kicks-0.46.0/src/kicks.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:42:34.240631 kicks-0.47.0/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.47.0/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:42:34.240456 kicks-0.47.0/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.47.0/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      603 2024-05-02 17:42:32.000000 kicks-0.47.0/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-02 17:42:34.240668 kicks-0.47.0/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:42:34.238766 kicks-0.47.0/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:42:34.239174 kicks-0.47.0/src/kicks/
+-rw-r--r--   0 robertdegen   (501) staff       (20)    19904 2024-05-02 17:42:29.000000 kicks-0.47.0/src/kicks/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:42:34.240291 kicks-0.47.0/src/kicks.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:42:34.000000 kicks-0.47.0/src/kicks.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      218 2024-05-02 17:42:34.000000 kicks-0.47.0/src/kicks.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-02 17:42:34.000000 kicks-0.47.0/src/kicks.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       24 2024-05-02 17:42:34.000000 kicks-0.47.0/src/kicks.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        6 2024-05-02 17:42:34.000000 kicks-0.47.0/src/kicks.egg-info/top_level.txt
```

### Comparing `kicks-0.46.0/PKG-INFO` & `kicks-0.47.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicks
-Version: 0.46.0
+Version: 0.47.0
 Summary: A small example package
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert
 Project-URL: Issues, https://github.com/turbo-bert
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kicks-0.46.0/pyproject.toml` & `kicks-0.47.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kicks"
-version = "0.46.0"
+version = "0.47.0"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `kicks-0.46.0/src/kicks/__main__.py` & `kicks-0.47.0/src/kicks/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     if x == "j":
         #https://www.jenkins.io/download/
         outfile = os.path.join(OP, "jenkins.msi")
         cmd = 'curl -C - -L -o "%s" "https://get.jenkins.io/windows-stable/2.440.3/jenkins.msi"' % outfile
         subprocess.call(cmd, shell=True)
         run_confirm = CONSOLE.input('run it? type "run" to execute or anything else to exit # ')
         if run_confirm == "run":
-            subprocess.call("""msiexec.exe /i %s /passive JENKINSDIR="C:\\Program Files\\Jenkins\\" PORTNUMBER=18080 JENKINS_ROOT="%ProgramData%\\Jenkins\\" JAVA_HOME="C:\\Program Files\\Java\\jdk-21\\" SERVICE_LOGON_TYPE=ServiceLocalSystem ALLUSERS=1""" % outfile, shell=True)
+            subprocess.call("""msiexec.exe /i %s /passive JENKINSDIR="C:\\Program Files\\Jenkins\\" PORTNUMBER=18080 JENKINS_ROOT="%%ProgramData%%\\Jenkins\\" JAVA_HOME="C:\\Program Files\\Java\\jdk-21\\" SERVICE_LOGON_TYPE=ServiceLocalSystem ALLUSERS=1""" % outfile, shell=True)
 
     if x == "j21":
         outfile = os.path.join(OP, "j21.msi")
         cmd = 'curl -C - -L -o "%s" "https://download.oracle.com/java/21/latest/jdk-21_windows-x64_bin.msi"' % outfile
         subprocess.call(cmd, shell=True)
         run_confirm = CONSOLE.input('run it? type "run" to execute or anything else to exit # ')
         if run_confirm == "run":
```

### Comparing `kicks-0.46.0/src/kicks.egg-info/PKG-INFO` & `kicks-0.47.0/src/kicks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicks
-Version: 0.46.0
+Version: 0.47.0
 Summary: A small example package
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert
 Project-URL: Issues, https://github.com/turbo-bert
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

