# Comparing `tmp/kicks-0.42.0.tar.gz` & `tmp/kicks-0.43.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicks-0.42.0.tar", last modified: Thu May  2 17:10:59 2024, max compression
+gzip compressed data, was "kicks-0.43.0.tar", last modified: Thu May  2 17:21:47 2024, max compression
```

## Comparing `kicks-0.42.0.tar` & `kicks-0.43.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:10:59.425782 kicks-0.42.0/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.42.0/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:10:59.425587 kicks-0.42.0/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.42.0/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      603 2024-05-02 17:10:57.000000 kicks-0.42.0/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-02 17:10:59.425824 kicks-0.42.0/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:10:59.423385 kicks-0.42.0/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:10:59.424108 kicks-0.42.0/src/kicks/
--rw-r--r--   0 robertdegen   (501) staff       (20)    19011 2024-05-02 17:10:43.000000 kicks-0.42.0/src/kicks/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:10:59.425388 kicks-0.42.0/src/kicks.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:10:59.000000 kicks-0.42.0/src/kicks.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      218 2024-05-02 17:10:59.000000 kicks-0.42.0/src/kicks.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-02 17:10:59.000000 kicks-0.42.0/src/kicks.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       24 2024-05-02 17:10:59.000000 kicks-0.42.0/src/kicks.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        6 2024-05-02 17:10:59.000000 kicks-0.42.0/src/kicks.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:21:47.467239 kicks-0.43.0/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.43.0/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:21:47.467072 kicks-0.43.0/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.43.0/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      603 2024-05-02 17:21:45.000000 kicks-0.43.0/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-02 17:21:47.467275 kicks-0.43.0/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:21:47.465229 kicks-0.43.0/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:21:47.465866 kicks-0.43.0/src/kicks/
+-rw-r--r--   0 robertdegen   (501) staff       (20)    19226 2024-05-02 17:21:33.000000 kicks-0.43.0/src/kicks/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 17:21:47.466906 kicks-0.43.0/src/kicks.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 17:21:47.000000 kicks-0.43.0/src/kicks.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      218 2024-05-02 17:21:47.000000 kicks-0.43.0/src/kicks.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-02 17:21:47.000000 kicks-0.43.0/src/kicks.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       24 2024-05-02 17:21:47.000000 kicks-0.43.0/src/kicks.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        6 2024-05-02 17:21:47.000000 kicks-0.43.0/src/kicks.egg-info/top_level.txt
```

### Comparing `kicks-0.42.0/PKG-INFO` & `kicks-0.43.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicks
-Version: 0.42.0
+Version: 0.43.0
 Summary: A small example package
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert
 Project-URL: Issues, https://github.com/turbo-bert
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kicks-0.42.0/pyproject.toml` & `kicks-0.43.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kicks"
-version = "0.42.0"
+version = "0.43.0"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `kicks-0.42.0/src/kicks/__main__.py` & `kicks-0.43.0/src/kicks/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -363,28 +363,32 @@
         if run_confirm == "run":
             subprocess.call("%s /passive /qr" % outfile, shell=True)
 
     if x == "sshd1":
         #https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell
         cmd="""powershell -Command Add-WindowsCapability -Online -Name OpenSSH.Server~~~~0.0.1.0"""
         subprocess.call(cmd, shell=True)
+        # cmd="""powershell -Command Start-Service sshd"""
+        # subprocess.call(cmd, shell=True)
+        # cmd="""powershell -Command Stop-Service sshd"""
+        # subprocess.call(cmd, shell=True)
 
     if x == "sshd2":
         #https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell
-        cmd="""notepad C:\ProgramData\ssh\administrators_authorized_keys"""
+        cmd="""notepad C:\\ProgramData\\ssh\\administrators_authorized_keys"""
         subprocess.call(cmd, shell=True)
 
     if x == "sshd3":
         #https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell
-        cmd="""mv C:\ProgramData\ssh\administrators_authorized_keys.txt C:\ProgramData\ssh\administrators_authorized_keys"""
+        cmd="""mv C:\\ProgramData\\ssh\\administrators_authorized_keys.txt C:\\ProgramData\\ssh\\administrators_authorized_keys"""
         subprocess.call(cmd, shell=True)
 
     if x == "sshd4":
         #https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell
-        cmd="""icacls.exe "C:\ProgramData\ssh\administrators_authorized_keys" /inheritance:r /grant "Administrators:F" /grant "SYSTEM:F" """
+        cmd="""icacls.exe "C:\\ProgramData\\ssh\\administrators_authorized_keys" /inheritance:r /grant "Administrators:F" /grant "SYSTEM:F" """
         subprocess.call(cmd, shell=True)
 
     if x == "sshd5":
         #https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell
         cmd="""powershell -Command Start-Service sshd"""
         subprocess.call(cmd, shell=True)
```

### Comparing `kicks-0.42.0/src/kicks.egg-info/PKG-INFO` & `kicks-0.43.0/src/kicks.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicks
-Version: 0.42.0
+Version: 0.43.0
 Summary: A small example package
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert
 Project-URL: Issues, https://github.com/turbo-bert
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

