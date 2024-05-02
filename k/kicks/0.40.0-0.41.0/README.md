# Comparing `tmp/kicks-0.40.0.tar.gz` & `tmp/kicks-0.41.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicks-0.40.0.tar", last modified: Mon Mar 11 22:50:09 2024, max compression
+gzip compressed data, was "kicks-0.41.0.tar", last modified: Thu May  2 16:55:57 2024, max compression
```

## Comparing `kicks-0.40.0.tar` & `kicks-0.41.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-11 22:50:09.326518 kicks-0.40.0/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.40.0/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-03-11 22:50:09.326356 kicks-0.40.0/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.40.0/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      603 2024-03-11 22:50:07.000000 kicks-0.40.0/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-03-11 22:50:09.326551 kicks-0.40.0/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-11 22:50:09.324609 kicks-0.40.0/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-11 22:50:09.325302 kicks-0.40.0/src/kicks/
--rw-r--r--   0 robertdegen   (501) staff       (20)    15981 2024-03-11 22:50:01.000000 kicks-0.40.0/src/kicks/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-11 22:50:09.326207 kicks-0.40.0/src/kicks.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-03-11 22:50:09.000000 kicks-0.40.0/src/kicks.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      218 2024-03-11 22:50:09.000000 kicks-0.40.0/src/kicks.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-03-11 22:50:09.000000 kicks-0.40.0/src/kicks.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       24 2024-03-11 22:50:09.000000 kicks-0.40.0/src/kicks.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        6 2024-03-11 22:50:09.000000 kicks-0.40.0/src/kicks.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 16:55:57.675320 kicks-0.41.0/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.41.0/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 16:55:57.675148 kicks-0.41.0/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-01 14:51:43.000000 kicks-0.41.0/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      603 2024-05-02 16:55:55.000000 kicks-0.41.0/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-02 16:55:57.675357 kicks-0.41.0/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 16:55:57.673113 kicks-0.41.0/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 16:55:57.673754 kicks-0.41.0/src/kicks/
+-rw-r--r--   0 robertdegen   (501) staff       (20)    17225 2024-05-02 16:55:48.000000 kicks-0.41.0/src/kicks/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-02 16:55:57.674970 kicks-0.41.0/src/kicks.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      543 2024-05-02 16:55:57.000000 kicks-0.41.0/src/kicks.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      218 2024-05-02 16:55:57.000000 kicks-0.41.0/src/kicks.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-02 16:55:57.000000 kicks-0.41.0/src/kicks.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       24 2024-05-02 16:55:57.000000 kicks-0.41.0/src/kicks.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        6 2024-05-02 16:55:57.000000 kicks-0.41.0/src/kicks.egg-info/top_level.txt
```

### Comparing `kicks-0.40.0/PKG-INFO` & `kicks-0.41.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicks
-Version: 0.40.0
+Version: 0.41.0
 Summary: A small example package
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert
 Project-URL: Issues, https://github.com/turbo-bert
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kicks-0.40.0/pyproject.toml` & `kicks-0.41.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kicks"
-version = "0.40.0"
+version = "0.41.0"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `kicks-0.40.0/src/kicks/__main__.py` & `kicks-0.41.0/src/kicks/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 
 import rich
 from rich.pretty import pprint as PP
 from rich.console import Console
 from rich.table import Table
 CONSOLE = Console()
 
+
+# curl -o p.exe -L https://www.python.org/ftp/python/3.12.3/python-3.12.3-amd64.exe
+# p.exe PrependPath=1 /passive
+
+
 # written by robert degen
 # 2015-2024
 # notes:
 # c:\cygwin64\bin\mintty.exe -w max -s 80x25  -e python -m dcx
 # vs code / xdebug php extension + devsense php extension
 # windows server 2022:
 # https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022
@@ -22,24 +27,30 @@
 
 
 home = os.getenv("USERPROFILE")
 
 OP=os.path.join(home, "_kicks")
 OD=os.makedirs(OP, exist_ok=True)
 
+
 def tryversion(pkg):
     import importlib.metadata
     try:
         res = pkg + '-' + importlib.metadata.version(pkg)
     except:
         res = pkg + '-dev'
     return res
 
+
 def generic_pip_install(pkg_name, rcon):
-    pass
+    install_command = 'pip install "%s"' % pkg_name
+    confirm = CONSOLE.input("run '%s' ? # 'y' to continue... " % install_command)
+    if confirm == "y":
+        subprocess.call(install_command, shell=True)
+
 
 t = Table(title=tryversion("kicks"))
 t.add_column("#")
 t.add_column("File")
 t.add_column("#")
 t.add_column("File")
 t.add_row("u", "update kicks", "id", "install dcx")
@@ -50,16 +61,16 @@
 t.add_row("2", "chrome windows 64", "6", "virtualbox")
 t.add_section()
 t.add_row("4", "process explorer", "wp", "latest wordpress")
 t.add_row("5", "vc_redist", "www", "WP->htdocs (req:wp)")
 t.add_row("7", "grml small iso", "2k22", "windows server 2022 en iso")
 t.add_row("8", "fpc win64")
 t.add_row("9", "sublime", "npp", "notepad plus plus")
-t.add_row("10", "emacs")
-t.add_row("11", "cygwin")
+t.add_row("10", "emacs", "j21", "Java JDK v21 Oracle")
+t.add_row("11", "cygwin", "j22", "Java JDK v22 Oracle")
 t.add_row("12", "git", "is", "inno setup")
 t.add_row("13", "xampp")
 t.add_row("14", "visual studio code", "15", "LibreOffice")
 t.add_section()
 t.add_row("q", "QUIT")
 
 while True:
@@ -176,14 +187,30 @@
         subprocess.call(cmd, shell=True)
         run_confirm = CONSOLE.input('run it? type "run" to execute or anything else to exit # ')
         if run_confirm == "run":
             subprocess.call("""powershell -Command Expand-Archive -Path '%s' -DestinationPath '%s'""" % (outfile, outzipdir), shell=True)
             subprocess.call("""%s""" % os.path.join(outzipdir, "Installers", "GoogleChromeStandaloneEnterprise64.msi"), shell=True)
             #subprocess.call("""explorer %s""" % (outzipdir), shell=True)
 
+    if x == "j21":
+        outfile = os.path.join(OP, "j21.msi")
+        cmd = 'curl -C - -L -o "%s" "https://download.oracle.com/java/21/latest/jdk-21_windows-x64_bin.msi"' % outfile
+        subprocess.call(cmd, shell=True)
+        run_confirm = CONSOLE.input('run it? type "run" to execute or anything else to exit # ')
+        if run_confirm == "run":
+            subprocess.call("msiexec.exe /i %s /qn" % outfile, shell=True)
+
+    if x == "j22":
+        outfile = os.path.join(OP, "j22.msi")
+        cmd = 'curl -C - -L -o "%s" "https://download.oracle.com/java/22/latest/jdk-22_windows-x64_bin.msi"' % outfile
+        subprocess.call(cmd, shell=True)
+        run_confirm = CONSOLE.input('run it? type "run" to execute or anything else to exit # ')
+        if run_confirm == "run":
+            subprocess.call("msiexec.exe /i %s /qn" % outfile, shell=True)
+
     if x == "wp":
         outfile = os.path.join(OP, "wp.zip")
         outzipdir = os.path.join(OP, "wp")
         cmd = 'curl -C - -L -o "%s" "https://wordpress.org/latest.zip"' % outfile
         subprocess.call(cmd, shell=True)
         run_confirm = CONSOLE.input('run it? type "run" to execute or anything else to exit # ')
         if run_confirm == "run":
```

### Comparing `kicks-0.40.0/src/kicks.egg-info/PKG-INFO` & `kicks-0.41.0/src/kicks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicks
-Version: 0.40.0
+Version: 0.41.0
 Summary: A small example package
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert
 Project-URL: Issues, https://github.com/turbo-bert
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

