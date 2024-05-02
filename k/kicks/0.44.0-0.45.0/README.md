# Comparing `tmp/kicks-0.44.0.tar.gz` & `tmp/kicks-0.45.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicks-0.44.0.tar", last modified: Thu May  2 17:30:08 2024, max compression
+gzip compressed data, was "kicks-0.45.0.tar", last modified: Thu May  2 17:35:19 2024, max compression
```

## Comparing `kicks-0.44.0.tar` & `kicks-0.45.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:30:08.573393 kicks-0.44.0/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.44.0/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:30:08.573199 kicks-0.44.0/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.44.0/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      603 2024-05-02 17:30:06.000000 kicks-0.44.0/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-02 17:30:08.573433 kicks-0.44.0/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:30:08.571295 kicks-0.44.0/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:30:08.571998 kicks-0.44.0/src/kicks/
--rw-r--r--   0 robertdegen   (501) staff       (20)    19228 2024-05-02 17:30:02.000000 kicks-0.44.0/src/kicks/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:30:08.573018 kicks-0.44.0/src/kicks.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:30:08.000000 kicks-0.44.0/src/kicks.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      218 2024-05-02 17:30:08.000000 kicks-0.44.0/src/kicks.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-02 17:30:08.000000 kicks-0.44.0/src/kicks.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       24 2024-05-02 17:30:08.000000 kicks-0.44.0/src/kicks.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        6 2024-05-02 17:30:08.000000 kicks-0.44.0/src/kicks.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:35:19.551628 kicks-0.45.0/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.45.0/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:35:19.551465 kicks-0.45.0/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.45.0/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      603 2024-05-02 17:35:17.000000 kicks-0.45.0/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-02 17:35:19.551663 kicks-0.45.0/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:35:19.549543 kicks-0.45.0/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:35:19.550242 kicks-0.45.0/src/kicks/
+-rw-r--r--   0 robertdegen   (501) staff       (20)    19704 2024-05-02 17:35:13.000000 kicks-0.45.0/src/kicks/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:35:19.551305 kicks-0.45.0/src/kicks.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:35:19.000000 kicks-0.45.0/src/kicks.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      218 2024-05-02 17:35:19.000000 kicks-0.45.0/src/kicks.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-02 17:35:19.000000 kicks-0.45.0/src/kicks.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       24 2024-05-02 17:35:19.000000 kicks-0.45.0/src/kicks.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        6 2024-05-02 17:35:19.000000 kicks-0.45.0/src/kicks.egg-info/top_level.txt
```

### Comparing `kicks-0.44.0/PKG-INFO` & `kicks-0.45.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicks
-Version: 0.44.0
+Version: 0.45.0
 Summary: A small example package
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert
 Project-URL: Issues, https://github.com/turbo-bert
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kicks-0.44.0/pyproject.toml` & `kicks-0.45.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kicks"
-version = "0.44.0"
+version = "0.45.0"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `kicks-0.44.0/src/kicks/__main__.py` & `kicks-0.45.0/src/kicks/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,23 @@
         subprocess.call(cmd, shell=True)
         run_confirm = CONSOLE.input('run it? type "run" to execute or anything else to exit # ')
         if run_confirm == "run":
             subprocess.call("""powershell -Command Expand-Archive -Path '%s' -DestinationPath '%s'""" % (outfile, outzipdir), shell=True)
             subprocess.call("""%s""" % os.path.join(outzipdir, "Installers", "GoogleChromeStandaloneEnterprise64.msi"), shell=True)
             #subprocess.call("""explorer %s""" % (outzipdir), shell=True)
 
+    if x == "j":
+        #https://www.jenkins.io/download/
+        outfile = os.path.join(OP, "jenkins.msi")
+        cmd = 'curl -C - -L -o "%s" "https://get.jenkins.io/windows-stable/2.440.3/jenkins.msi"' % outfile
+        subprocess.call(cmd, shell=True)
+        run_confirm = CONSOLE.input('run it? type "run" to execute or anything else to exit # ')
+        if run_confirm == "run":
+            subprocess.call("msiexec.exe /i %s /log c:\\jenkins.log.txt" % outfile, shell=True)
+
     if x == "j21":
         outfile = os.path.join(OP, "j21.msi")
         cmd = 'curl -C - -L -o "%s" "https://download.oracle.com/java/21/latest/jdk-21_windows-x64_bin.msi"' % outfile
         subprocess.call(cmd, shell=True)
         run_confirm = CONSOLE.input('run it? type "run" to execute or anything else to exit # ')
         if run_confirm == "run":
             subprocess.call("msiexec.exe /i %s /qn" % outfile, shell=True)
@@ -363,18 +372,18 @@
         if run_confirm == "run":
             subprocess.call("%s /passive /qr" % outfile, shell=True)
 
     if x == "sshd1":
         #https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell
         cmd="""powershell -Command Add-WindowsCapability -Online -Name OpenSSH.Server~~~~0.0.1.0"""
         subprocess.call(cmd, shell=True)
-        # cmd="""powershell -Command Start-Service sshd"""
-        # subprocess.call(cmd, shell=True)
-        # cmd="""powershell -Command Stop-Service sshd"""
-        # subprocess.call(cmd, shell=True)
+        cmd="""powershell -Command Start-Service sshd"""
+        subprocess.call(cmd, shell=True)
+        cmd="""powershell -Command Stop-Service sshd"""
+        subprocess.call(cmd, shell=True)
 
     if x == "sshd2":
         #https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell
         cmd="""notepad C:\\ProgramData\\ssh\\administrators_authorized_keys"""
         subprocess.call(cmd, shell=True)
 
     if x == "sshd3":
```

### Comparing `kicks-0.44.0/src/kicks.egg-info/PKG-INFO` & `kicks-0.45.0/src/kicks.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicks
-Version: 0.44.0
+Version: 0.45.0
 Summary: A small example package
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert
 Project-URL: Issues, https://github.com/turbo-bert
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

