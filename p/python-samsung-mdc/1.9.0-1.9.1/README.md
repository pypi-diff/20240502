# Comparing `tmp/python-samsung-mdc-1.9.0.tar.gz` & `tmp/python-samsung-mdc-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-samsung-mdc-1.9.0.tar", last modified: Wed Dec  8 17:23:48 2021, max compression
+gzip compressed data, was "python-samsung-mdc-1.9.1.tar", last modified: Wed Dec  8 21:27:54 2021, max compression
```

## Comparing `python-samsung-mdc-1.9.0.tar` & `python-samsung-mdc-1.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 vgavro    (1001) vgavro    (1002)        0 2021-12-08 17:23:48.185326 python-samsung-mdc-1.9.0/
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)    41811 2021-12-08 17:23:48.188660 python-samsung-mdc-1.9.0/PKG-INFO
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)    32843 2021-12-08 17:21:49.000000 python-samsung-mdc-1.9.0/README.md
-drwxr-xr-x   0 vgavro    (1001) vgavro    (1002)        0 2021-12-08 17:23:48.181993 python-samsung-mdc-1.9.0/python_samsung_mdc.egg-info/
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)    41811 2021-12-08 17:23:48.000000 python-samsung-mdc-1.9.0/python_samsung_mdc.egg-info/PKG-INFO
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)      514 2021-12-08 17:23:48.000000 python-samsung-mdc-1.9.0/python_samsung_mdc.egg-info/SOURCES.txt
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)        1 2021-12-08 17:23:48.000000 python-samsung-mdc-1.9.0/python_samsung_mdc.egg-info/dependency_links.txt
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)       53 2021-12-08 17:23:48.000000 python-samsung-mdc-1.9.0/python_samsung_mdc.egg-info/entry_points.txt
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)       23 2021-12-08 17:23:48.000000 python-samsung-mdc-1.9.0/python_samsung_mdc.egg-info/requires.txt
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)       12 2021-12-08 17:23:48.000000 python-samsung-mdc-1.9.0/python_samsung_mdc.egg-info/top_level.txt
-drwxr-xr-x   0 vgavro    (1001) vgavro    (1002)        0 2021-12-08 17:23:48.185326 python-samsung-mdc-1.9.0/samsung_mdc/
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)      545 2021-10-26 06:25:56.000000 python-samsung-mdc-1.9.0/samsung_mdc/__init__.py
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)       85 2021-05-06 17:50:47.000000 python-samsung-mdc-1.9.0/samsung_mdc/__main__.py
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)    27292 2021-12-08 17:20:49.000000 python-samsung-mdc-1.9.0/samsung_mdc/cli.py
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)     3217 2021-11-08 13:29:16.000000 python-samsung-mdc-1.9.0/samsung_mdc/command.py
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)    24118 2021-11-29 00:15:29.000000 python-samsung-mdc-1.9.0/samsung_mdc/commands.py
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)     8249 2021-10-28 14:01:32.000000 python-samsung-mdc-1.9.0/samsung_mdc/connection.py
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)      834 2021-10-25 17:03:33.000000 python-samsung-mdc-1.9.0/samsung_mdc/exceptions.py
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)     4500 2021-11-29 00:01:44.000000 python-samsung-mdc-1.9.0/samsung_mdc/fields.py
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)     1603 2021-12-01 04:16:50.000000 python-samsung-mdc-1.9.0/samsung_mdc/utils.py
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)       22 2021-12-08 17:22:44.000000 python-samsung-mdc-1.9.0/samsung_mdc/version.py
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)      105 2021-12-08 17:23:48.188660 python-samsung-mdc-1.9.0/setup.cfg
--rw-r--r--   0 vgavro    (1001) vgavro    (1002)     1434 2021-11-04 15:47:31.000000 python-samsung-mdc-1.9.0/setup.py
+drwxr-xr-x   0 vgavro    (1001) vgavro    (1002)        0 2021-12-08 21:27:54.510988 python-samsung-mdc-1.9.1/
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)    41989 2021-12-08 21:27:54.510988 python-samsung-mdc-1.9.1/PKG-INFO
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)    32997 2021-12-08 21:26:59.000000 python-samsung-mdc-1.9.1/README.md
+drwxr-xr-x   0 vgavro    (1001) vgavro    (1002)        0 2021-12-08 21:27:54.507655 python-samsung-mdc-1.9.1/python_samsung_mdc.egg-info/
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)    41989 2021-12-08 21:27:54.000000 python-samsung-mdc-1.9.1/python_samsung_mdc.egg-info/PKG-INFO
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)      514 2021-12-08 21:27:54.000000 python-samsung-mdc-1.9.1/python_samsung_mdc.egg-info/SOURCES.txt
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)        1 2021-12-08 21:27:54.000000 python-samsung-mdc-1.9.1/python_samsung_mdc.egg-info/dependency_links.txt
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)       53 2021-12-08 21:27:54.000000 python-samsung-mdc-1.9.1/python_samsung_mdc.egg-info/entry_points.txt
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)       30 2021-12-08 21:27:54.000000 python-samsung-mdc-1.9.1/python_samsung_mdc.egg-info/requires.txt
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)       12 2021-12-08 21:27:54.000000 python-samsung-mdc-1.9.1/python_samsung_mdc.egg-info/top_level.txt
+drwxr-xr-x   0 vgavro    (1001) vgavro    (1002)        0 2021-12-08 21:27:54.510988 python-samsung-mdc-1.9.1/samsung_mdc/
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)      545 2021-10-26 06:25:56.000000 python-samsung-mdc-1.9.1/samsung_mdc/__init__.py
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)       85 2021-05-06 17:50:47.000000 python-samsung-mdc-1.9.1/samsung_mdc/__main__.py
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)    27631 2021-12-08 21:26:10.000000 python-samsung-mdc-1.9.1/samsung_mdc/cli.py
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)     3217 2021-11-08 13:29:16.000000 python-samsung-mdc-1.9.1/samsung_mdc/command.py
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)    24118 2021-11-29 00:15:29.000000 python-samsung-mdc-1.9.1/samsung_mdc/commands.py
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)     8249 2021-10-28 14:01:32.000000 python-samsung-mdc-1.9.1/samsung_mdc/connection.py
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)      834 2021-10-25 17:03:33.000000 python-samsung-mdc-1.9.1/samsung_mdc/exceptions.py
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)     4500 2021-11-29 00:01:44.000000 python-samsung-mdc-1.9.1/samsung_mdc/fields.py
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)     1603 2021-12-01 04:16:50.000000 python-samsung-mdc-1.9.1/samsung_mdc/utils.py
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)       22 2021-12-08 21:20:55.000000 python-samsung-mdc-1.9.1/samsung_mdc/version.py
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)      105 2021-12-08 21:27:54.510988 python-samsung-mdc-1.9.1/setup.cfg
+-rw-r--r--   0 vgavro    (1001) vgavro    (1002)     1448 2021-12-08 21:17:43.000000 python-samsung-mdc-1.9.1/setup.py
```

### Comparing `python-samsung-mdc-1.9.0/PKG-INFO` & `python-samsung-mdc-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-samsung-mdc
-Version: 1.9.0
+Version: 1.9.1
 Summary: Samsung Multiple Display Control (MDC) protocol implementation (asyncio library + CLI interface)
 Home-page: http://github.com/vgavro/samsung-mdc
 Author: Victor Gavro
 Author-email: vgavro@gmail.com
 License: BSD
 Description: # Samsung-MDC
         
@@ -915,14 +915,17 @@
         
           Script file with commands to execute.
         
           Commands for multiple targets will be running async, but commands order is
           preserved for device (and is running on same connection), exit on first fail
           unless retry options provided.
         
+          You may use jinja2 templating engine to {% include "other_script" %} or {{
+          VAR_KEY }} rendering in combination with --var VAR_KEY VAR_VALUE options.
+        
           It's highly recommended to use sleep option for virtual_remote!
         
           Additional commands:
           sleep SECONDS  (FLOAT, --sleep option for this command is ignored)
           disconnect
         
           Format:
```

### Comparing `python-samsung-mdc-1.9.0/README.md` & `python-samsung-mdc-1.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -907,14 +907,17 @@
 
   Script file with commands to execute.
 
   Commands for multiple targets will be running async, but commands order is
   preserved for device (and is running on same connection), exit on first fail
   unless retry options provided.
 
+  You may use jinja2 templating engine to {% include "other_script" %} or {{
+  VAR_KEY }} rendering in combination with --var VAR_KEY VAR_VALUE options.
+
   It's highly recommended to use sleep option for virtual_remote!
 
   Additional commands:
   sleep SECONDS  (FLOAT, --sleep option for this command is ignored)
   disconnect
 
   Format:
```

### Comparing `python-samsung-mdc-1.9.0/python_samsung_mdc.egg-info/PKG-INFO` & `python-samsung-mdc-1.9.1/python_samsung_mdc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-samsung-mdc
-Version: 1.9.0
+Version: 1.9.1
 Summary: Samsung Multiple Display Control (MDC) protocol implementation (asyncio library + CLI interface)
 Home-page: http://github.com/vgavro/samsung-mdc
 Author: Victor Gavro
 Author-email: vgavro@gmail.com
 License: BSD
 Description: # Samsung-MDC
         
@@ -915,14 +915,17 @@
         
           Script file with commands to execute.
         
           Commands for multiple targets will be running async, but commands order is
           preserved for device (and is running on same connection), exit on first fail
           unless retry options provided.
         
+          You may use jinja2 templating engine to {% include "other_script" %} or {{
+          VAR_KEY }} rendering in combination with --var VAR_KEY VAR_VALUE options.
+        
           It's highly recommended to use sleep option for virtual_remote!
         
           Additional commands:
           sleep SECONDS  (FLOAT, --sleep option for this command is ignored)
           disconnect
         
           Format:
```

### Comparing `python-samsung-mdc-1.9.0/python_samsung_mdc.egg-info/SOURCES.txt` & `python-samsung-mdc-1.9.1/python_samsung_mdc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-samsung-mdc-1.9.0/samsung_mdc/__init__.py` & `python-samsung-mdc-1.9.1/samsung_mdc/__init__.py`

 * *Files identical despite different names*

### Comparing `python-samsung-mdc-1.9.0/samsung_mdc/cli.py` & `python-samsung-mdc-1.9.1/samsung_mdc/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -554,14 +554,17 @@
 SCRIPT_HELP = """
 Script file with commands to execute.
 
 Commands for multiple targets will be running async, but
 commands order is preserved for device (and is running on same connection),
 exit on first fail unless retry options provided.
 
+You may use jinja2 templating engine to {% include "other_script" %}
+or {{ VAR_KEY }} rendering in combination with --var VAR_KEY VAR_VALUE options.
+
 It\'s highly recommended to use sleep option for virtual_remote!
 
 \b
 Additional commands:
 sleep SECONDS  (FLOAT, --sleep option for this command is ignored)
 disconnect
 
@@ -578,16 +581,14 @@
 clear_menu
 virtual_remote key_menu
 virtual_remote key_down
 virtual_remote {{ KEY }}
 clear_menu
 """
 
-VAR_TEMPLATE = re.compile(r'{{\s*(.*?)\s*}}')
-
 
 @cli.command(help=SCRIPT_HELP, cls=FixedSubcommand)
 @click.option('-s', '--sleep', default=0, type=float,
               help='Pause between commands (seconds)')
 @click.option('--retry-command', default=0, type=int,
               help='Retry command if failed (count)')
 @click.option('--retry-command-sleep', default=0, type=float,
@@ -608,14 +609,28 @@
 def script(ctx, script_file, sleep, retry_command, retry_command_sleep,
            retry_script, retry_script_sleep, ignore_nak, var):
     import shlex
 
     var = dict(var)
     retry_command_sleep = retry_command_sleep or sleep
     retry_script_sleep = retry_script_sleep or sleep
+    script_content = script_file.read()
+
+    if var or '{{' in script_content or '{%' in script_content:
+        from jinja2 import Environment, FileSystemLoader, StrictUndefined
+
+        class RelativeEnvironment(Environment):
+            def join_path(self, template, parent):
+                # Allowing include based on path relative to script
+                return os.path.join(os.path.dirname(parent), template)
+
+        env = RelativeEnvironment(loader=FileSystemLoader(['/', './']),
+                                  undefined=StrictUndefined)
+        template = env.get_template(script_file.name)
+        script_content = template.render(**var)
 
     def fail(lineno, line, reason):
         raise click.UsageError(
             f'{script_file.name}:{lineno}:"{line}": {reason}')
 
     def create_disconnect():
         async def disconnect(connection, display_id):
@@ -631,31 +646,21 @@
             return tuple()
         sleep.name = 'sleep'
         sleep.args = [seconds]
         return sleep
 
     lines = [
         (i + 1, line.strip())
-        for i, line in enumerate(script_file.read().split('\n'))
+        for i, line in enumerate(script_content.splitlines())
     ]
     calls = []
     for lineno, line in lines:
         if not line or line.startswith('#'):
             continue
 
-        var_match = VAR_TEMPLATE.search(line)
-        while var_match:
-            var_name = var_match.groups()[0]
-            var_value = var.get(var_name)
-            if var_value is None:
-                fail(lineno, line, f'Unknown variable: {var_name}')
-            line = (line[0:var_match.start()] +
-                    var_value + line[var_match.end():])
-            var_match = VAR_TEMPLATE.search(line)
-
         command, *args = shlex.split(line)
         command = command.lower()
         if (command not in cli.commands
            and command not in ['sleep', 'disconnect']):
             fail(lineno, line, f'Unknown command: {command}')
         if command == 'sleep':
             if len(args) != 1:
```

### Comparing `python-samsung-mdc-1.9.0/samsung_mdc/command.py` & `python-samsung-mdc-1.9.1/samsung_mdc/command.py`

 * *Files identical despite different names*

### Comparing `python-samsung-mdc-1.9.0/samsung_mdc/commands.py` & `python-samsung-mdc-1.9.1/samsung_mdc/commands.py`

 * *Files identical despite different names*

### Comparing `python-samsung-mdc-1.9.0/samsung_mdc/connection.py` & `python-samsung-mdc-1.9.1/samsung_mdc/connection.py`

 * *Files identical despite different names*

### Comparing `python-samsung-mdc-1.9.0/samsung_mdc/exceptions.py` & `python-samsung-mdc-1.9.1/samsung_mdc/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-samsung-mdc-1.9.0/samsung_mdc/fields.py` & `python-samsung-mdc-1.9.1/samsung_mdc/fields.py`

 * *Files identical despite different names*

### Comparing `python-samsung-mdc-1.9.0/samsung_mdc/utils.py` & `python-samsung-mdc-1.9.1/samsung_mdc/utils.py`

 * *Files identical despite different names*

### Comparing `python-samsung-mdc-1.9.0/setup.py` & `python-samsung-mdc-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 
 exec(open('samsung_mdc/version.py').read())
 
 requires = [
     'click',  # tested: click >=7,<=8
+    'jinja2',
     'pyserial-asyncio'  # tested: pyserial==3.5; pyserial-asyncio==0.5
 ]
 
 setup(
     name='python-samsung-mdc',
     version=__version__,  # noqa
     description=('Samsung Multiple Display Control (MDC) '
```

