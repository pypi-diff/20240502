# Comparing `tmp/xontrib-prompt-bar-0.5.7.tar.gz` & `tmp/xontrib_prompt_bar-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-prompt-bar-0.5.7.tar", last modified: Wed Nov 22 13:33:51 2023, max compression
+gzip compressed data, was "xontrib_prompt_bar-0.5.8.tar", last modified: Thu May  2 18:15:20 2024, max compression
```

## Comparing `xontrib-prompt-bar-0.5.7.tar` & `xontrib_prompt_bar-0.5.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:33:51.139314 xontrib-prompt-bar-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-11-22 13:33:42.000000 xontrib-prompt-bar-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-22 13:33:42.000000 xontrib-prompt-bar-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2023-11-22 13:33:51.139314 xontrib-prompt-bar-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2023-11-22 13:33:42.000000 xontrib-prompt-bar-0.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-22 13:33:51.139314 xontrib-prompt-bar-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-11-22 13:33:42.000000 xontrib-prompt-bar-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:33:51.135314 xontrib-prompt-bar-0.5.7/xontrib/
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2023-11-22 13:33:42.000000 xontrib-prompt-bar-0.5.7/xontrib/prompt_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 13:33:51.139314 xontrib-prompt-bar-0.5.7/xontrib_prompt_bar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2023-11-22 13:33:51.000000 xontrib-prompt-bar-0.5.7/xontrib_prompt_bar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-11-22 13:33:51.000000 xontrib-prompt-bar-0.5.7/xontrib_prompt_bar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 13:33:51.000000 xontrib-prompt-bar-0.5.7/xontrib_prompt_bar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-22 13:33:51.000000 xontrib-prompt-bar-0.5.7/xontrib_prompt_bar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:15:20.057872 xontrib_prompt_bar-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-02 18:15:05.000000 xontrib_prompt_bar-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 18:15:05.000000 xontrib_prompt_bar-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-02 18:15:20.057872 xontrib_prompt_bar-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-05-02 18:15:05.000000 xontrib_prompt_bar-0.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:15:20.057872 xontrib_prompt_bar-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-02 18:15:05.000000 xontrib_prompt_bar-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:15:20.057872 xontrib_prompt_bar-0.5.8/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-02 18:15:05.000000 xontrib_prompt_bar-0.5.8/xontrib/prompt_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:15:20.057872 xontrib_prompt_bar-0.5.8/xontrib_prompt_bar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-02 18:15:20.000000 xontrib_prompt_bar-0.5.8/xontrib_prompt_bar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 18:15:20.000000 xontrib_prompt_bar-0.5.8/xontrib_prompt_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:15:20.000000 xontrib_prompt_bar-0.5.8/xontrib_prompt_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 18:15:20.000000 xontrib_prompt_bar-0.5.8/xontrib_prompt_bar.egg-info/top_level.txt
```

### Comparing `xontrib-prompt-bar-0.5.7/LICENSE` & `xontrib_prompt_bar-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-prompt-bar-0.5.7/PKG-INFO` & `xontrib_prompt_bar-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-prompt-bar
-Version: 0.5.7
+Version: 0.5.8
 Summary: The bar theme for xonsh shell.
 Home-page: https://github.com/anki-code/xontrib-prompt-bar
 Author: anki
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/anki-code/xontrib-prompt-bar/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xontrib-prompt-bar
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-prompt-bar Version: 0.5.7 Summary: The bar
+Metadata-Version: 2.1 Name: xontrib-prompt-bar Version: 0.5.8 Summary: The bar
 theme for xonsh shell. Home-page: https://github.com/anki-code/xontrib-prompt-
 bar Author: anki Author-email: author@example.com License: BSD Project-URL:
 Documentation, https://github.com/anki-code/xontrib-prompt-bar/blob/master/
 README.md Project-URL: Code, https://github.com/anki-code/xontrib-prompt-bar
 Project-URL: Issue tracker, https://github.com/anki-code/xontrib-prompt-bar/
 issues Platform: any Classifier: Environment :: Console Classifier: Intended
 Audience :: End Users/Desktop Classifier: Operating System :: OS Independent
```

### Comparing `xontrib-prompt-bar-0.5.7/README.md` & `xontrib_prompt_bar-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `xontrib-prompt-bar-0.5.7/setup.py` & `xontrib_prompt_bar-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except (IOError, OSError):
     long_description = ''
 
 setup(
     name='xontrib-prompt-bar',
-    version='0.5.7',
+    version='0.5.8',
     license='BSD',
     author='anki',
     author_email='author@example.com',
     description="The bar theme for xonsh shell.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
```

### Comparing `xontrib-prompt-bar-0.5.7/xontrib/prompt_bar.py` & `xontrib_prompt_bar-0.5.8/xontrib/prompt_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,18 @@
 __xonsh__.env['PROMPT_FIELDS']['date_time_tz'] = _field_date_time_tz
 __xonsh__.env['PROMPT_FIELDS']['hist_status'] = lambda: '' if __xonsh__.history.remember_history else 'hist off'
 
 
 def _screens():
     line = []
     sty = None
-    for l in __xonsh__.subproc_captured_stdout(['bash', '-c', 'screen -ls; exit 0']).splitlines():  # bash is to fix https://github.com/xonsh/xonsh/issues/4912 
+    scrs = __xonsh__.subproc_captured_stdout(['bash', '-c', 'screen -ls; exit 0'])
+    if isinstance(scrs, str):
+        scrs = scrs.splitlines()
+    for l in scrs:  # bash is to fix https://github.com/xonsh/xonsh/issues/4912 
         if '\t' in l:
             screen_name = l.split('\t')[1].split('.')[1]
             if sty is None:  # lazy load
                 sty = __xonsh__.env.get('STY', '.').split('.')[1]
             line.append(f"({screen_name})" if sty == screen_name else screen_name)
     return ', '.join(line)
 __xonsh__.env['PROMPT_FIELDS']['screens'] = _screens
@@ -133,15 +136,15 @@
     # Jump to parent if the current directory does not exist.
     try:
         d = Path(__xonsh__.env['PWD'])
         nd = d
         while not nd.exists():
             nd = nd.parent
         if nd != d:
-            printx(f'{{YELLOW}}The directory {d} does not exist. Jump to parent: {nd}{{RESET}}')
+            printx(f'{{YELLOW}}The directory {d} does not exist.\nJump to parent: {nd}{{RESET}}')
             execx(f'cd {repr(str(nd))}')
     except:
         pass
 
     # Get the terminal size
     try:
         ts = os.get_terminal_size()
```

### Comparing `xontrib-prompt-bar-0.5.7/xontrib_prompt_bar.egg-info/PKG-INFO` & `xontrib_prompt_bar-0.5.8/xontrib_prompt_bar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-prompt-bar
-Version: 0.5.7
+Version: 0.5.8
 Summary: The bar theme for xonsh shell.
 Home-page: https://github.com/anki-code/xontrib-prompt-bar
 Author: anki
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/anki-code/xontrib-prompt-bar/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xontrib-prompt-bar
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-prompt-bar Version: 0.5.7 Summary: The bar
+Metadata-Version: 2.1 Name: xontrib-prompt-bar Version: 0.5.8 Summary: The bar
 theme for xonsh shell. Home-page: https://github.com/anki-code/xontrib-prompt-
 bar Author: anki Author-email: author@example.com License: BSD Project-URL:
 Documentation, https://github.com/anki-code/xontrib-prompt-bar/blob/master/
 README.md Project-URL: Code, https://github.com/anki-code/xontrib-prompt-bar
 Project-URL: Issue tracker, https://github.com/anki-code/xontrib-prompt-bar/
 issues Platform: any Classifier: Environment :: Console Classifier: Intended
 Audience :: End Users/Desktop Classifier: Operating System :: OS Independent
```

