# Comparing `tmp/pylinweb-1.9.2.tar.gz` & `tmp/pylinweb-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinweb-1.9.2.tar", last modified: Tue Apr 30 03:38:15 2024, max compression
+gzip compressed data, was "pylinweb-1.9.3.tar", last modified: Thu May  2 21:11:17 2024, max compression
```

## Comparing `pylinweb-1.9.2.tar` & `pylinweb-1.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 03:38:15.762730 pylinweb-1.9.2/
--rw-rw-rw-   0        0        0       34 2024-04-29 20:50:14.000000 pylinweb-1.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2520 2024-04-30 03:38:15.760932 pylinweb-1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2024-04-26 00:01:05.000000 pylinweb-1.9.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 03:38:15.734439 pylinweb-1.9.2/pylinweb/
--rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.9.2/pylinweb/__init__.py
--rw-rw-rw-   0        0        0     3299 2024-04-30 03:35:51.000000 pylinweb-1.9.2/pylinweb/functions.py
--rw-rw-rw-   0        0        0     1544 2024-04-29 20:51:43.000000 pylinweb-1.9.2/pylinweb/main.py
--rw-rw-rw-   0        0        0      115 2024-04-30 03:37:53.000000 pylinweb-1.9.2/pylinweb/variables.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:38:15.759137 pylinweb-1.9.2/pylinweb.egg-info/
--rw-rw-rw-   0        0        0     2520 2024-04-30 03:38:15.000000 pylinweb-1.9.2/pylinweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-30 03:38:15.000000 pylinweb-1.9.2/pylinweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 03:38:15.000000 pylinweb-1.9.2/pylinweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-30 03:38:15.000000 pylinweb-1.9.2/pylinweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2024-04-30 03:38:15.000000 pylinweb-1.9.2/pylinweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 03:38:15.000000 pylinweb-1.9.2/pylinweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 03:38:15.762730 pylinweb-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1500 2024-04-29 23:30:55.000000 pylinweb-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:11:17.223515 pylinweb-1.9.3/
+-rw-rw-rw-   0        0        0       46 2024-04-30 04:05:30.000000 pylinweb-1.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3042 2024-05-02 21:11:17.221550 pylinweb-1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2103 2024-05-02 20:43:22.000000 pylinweb-1.9.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 21:11:17.178045 pylinweb-1.9.3/pylinweb/
+-rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.9.3/pylinweb/__init__.py
+-rw-rw-rw-   0        0        0     4020 2024-05-02 21:09:25.000000 pylinweb-1.9.3/pylinweb/functions.py
+-rw-rw-rw-   0        0        0     1686 2024-05-02 20:47:00.000000 pylinweb-1.9.3/pylinweb/main.py
+-rw-rw-rw-   0        0        0       99 2024-05-02 21:10:45.000000 pylinweb-1.9.3/pylinweb/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:11:17.219166 pylinweb-1.9.3/pylinweb.egg-info/
+-rw-rw-rw-   0        0        0     3042 2024-05-02 21:11:16.000000 pylinweb-1.9.3/pylinweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-02 21:11:17.000000 pylinweb-1.9.3/pylinweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 21:11:16.000000 pylinweb-1.9.3/pylinweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-02 21:11:16.000000 pylinweb-1.9.3/pylinweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2024-05-02 21:11:16.000000 pylinweb-1.9.3/pylinweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 21:11:16.000000 pylinweb-1.9.3/pylinweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 21:11:17.224001 pylinweb-1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1460 2024-04-30 03:40:44.000000 pylinweb-1.9.3/setup.py
```

### Comparing `pylinweb-1.9.2/pylinweb/main.py` & `pylinweb-1.9.3/pylinweb/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,37 +3,40 @@
 from .variables import *
 from .functions import (
 print_version, reset_files, 
 generate_report_html, 
 generate_report_word,
 install_dependencies, 
 execute_tests,
-clone_repository)
+clone_repository,
+open_application)
 
 def main():
     parser = argparse.ArgumentParser(description='Testing utility for web applications.')
     
     # Define arguments
-    parser.add_argument('--setup', action='store_true', help='Copy app directory and install dependencies')
+    parser.add_argument('--setup', action='store_true', help=f'Copy {app} directory and install dependencies')
     parser.add_argument('--version', action='store_true', help='Show version')
     parser.add_argument('--run-tests', action='store_true', help='Run tests')
     parser.add_argument('--report-html', action='store_true', help='Generate html report')
     parser.add_argument('--report-word', action='store_true', help='Generate word report')
     parser.add_argument('--reset', action='store_true', help='Delete innecesary directories and files')
-    
+    parser.add_argument('--open-app', action='store_true', help='Open application')
+
     args = parser.parse_args()
     
     #Define actions and their corresponding functions
     actions = {
         'setup': lambda: (clone_repository(), install_dependencies()),
         'version': print_version,
         'run_tests': execute_tests,
         'report_html': generate_report_html,
         'report_word': generate_report_word,
-        'reset': reset_files
+        'reset': reset_files,
+        'open_app': open_application
     }
 
     # Get the first truthy argument
     arg = next((arg for arg in vars(args) if getattr(args, arg)), None)
 
     if arg in actions:
         actions[arg]()
```

### Comparing `pylinweb-1.9.2/setup.py` & `pylinweb-1.9.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         "docxtpl==0.16.8",
         "playwright==1.42.0",
         "psutil==5.9.2",
         "PyPDF2==3.0.1",
         "python-docx==1.1.0",
         "pycparser==2.21",
         "screeninfo==0.8",
-        "selenium==4.12", #cambiar 4.20.0 instalamos webdriver 0.
+        "selenium==4.12",
         "keyboard==0.13.5"
     ],
     entry_points={
         'console_scripts': [
             'pylinweb=pylinweb.main:main',
         ],
     },
```

