# Comparing `tmp/cylc-rose-1.3.3.tar.gz` & `tmp/cylc-rose-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylc-rose-1.3.3.tar", last modified: Fri Apr  5 14:59:53 2024, max compression
+gzip compressed data, was "cylc-rose-1.3.4.tar", last modified: Thu May  2 12:36:47 2024, max compression
```

## Comparing `cylc-rose-1.3.3.tar` & `cylc-rose-1.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:59:53.801746 cylc-rose-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-05 14:59:53.801746 cylc-rose-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:59:53.801746 cylc-rose-1.3.3/cylc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:59:53.801746 cylc-rose-1.3.3/cylc/rose/
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/jinja2_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/platform_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21197 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/stem.py
--rw-r--r--   0 runner    (1001) docker     (127)    27151 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/cylc/rose/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:59:53.801746 cylc-rose-1.3.3/cylc_rose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 14:59:53.000000 cylc-rose-1.3.3/cylc_rose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-05 14:59:53.805746 cylc-rose-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-05 14:59:50.000000 cylc-rose-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:36:47.347566 cylc-rose-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-02 12:36:31.000000 cylc-rose-1.3.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-02 12:36:47.347566 cylc-rose-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-02 12:36:31.000000 cylc-rose-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:36:47.343567 cylc-rose-1.3.4/cylc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:36:47.343567 cylc-rose-1.3.4/cylc/rose/
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-02 12:36:31.000000 cylc-rose-1.3.4/cylc/rose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-05-02 12:36:31.000000 cylc-rose-1.3.4/cylc/rose/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-05-02 12:36:31.000000 cylc-rose-1.3.4/cylc/rose/jinja2_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-02 12:36:31.000000 cylc-rose-1.3.4/cylc/rose/platform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21197 2024-05-02 12:36:31.000000 cylc-rose-1.3.4/cylc/rose/stem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27199 2024-05-02 12:36:31.000000 cylc-rose-1.3.4/cylc/rose/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:36:47.347566 cylc-rose-1.3.4/cylc_rose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-02 12:36:47.000000 cylc-rose-1.3.4/cylc_rose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 12:36:47.000000 cylc-rose-1.3.4/cylc_rose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:36:47.000000 cylc-rose-1.3.4/cylc_rose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 12:36:47.000000 cylc-rose-1.3.4/cylc_rose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-02 12:36:47.000000 cylc-rose-1.3.4/cylc_rose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 12:36:47.000000 cylc-rose-1.3.4/cylc_rose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-02 12:36:47.347566 cylc-rose-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-02 12:36:31.000000 cylc-rose-1.3.4/setup.py
```

### Comparing `cylc-rose-1.3.3/COPYING` & `cylc-rose-1.3.4/COPYING`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.3/PKG-INFO` & `cylc-rose-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-rose
-Version: 1.3.3
+Version: 1.3.4
 Summary: A Cylc plugin providing support for the Rose rose-suite.conf file.
 Home-page: https://cylc.github.io/cylc-doc/latest/html/plugins/cylc-rose.html
 Author: British Crown (Met Office) & Contributors
 Author-email: metomi@metoffice.gov.uk
 License: GPL
 Keywords: cylc,rose,workflow,configuration,workflow-engine,workflow-automation,workflow-management
 Platform: any
```

### Comparing `cylc-rose-1.3.3/README.md` & `cylc-rose-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.3/cylc/rose/__init__.py` & `cylc-rose-1.3.4/cylc/rose/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,8 +201,8 @@
    To reinstall a rose stem suite use ``cylc reinstall``.  Cylc can get any
    options you do not change from the ``rose-suite-cylc-install.conf``` file.
    Using ``rose stem`` a second time will attempt install a new copy
    of your rose stem suite.
 
 """
 
-__version__ = '1.3.3'
+__version__ = '1.3.4'
```

### Comparing `cylc-rose-1.3.3/cylc/rose/entry_points.py` & `cylc-rose-1.3.4/cylc/rose/entry_points.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import shutil
 
 from pathlib import Path
 
 from metomi.rose.config import ConfigLoader, ConfigDumper
 from cylc.rose.utilities import (
     ROSE_ORIG_HOST_INSTALLED_OVERRIDE_STRING,
+    ROSE_SUITE_OPT_CONF_KEYS,
     deprecation_warnings,
     dump_rose_log,
     get_rose_vars_from_config_node,
     identify_templating_section,
     invalid_defines_check,
     rose_config_exists,
     rose_config_tree_loader,
@@ -50,20 +51,20 @@
             '\n * "--opt-conf-key" or "-O"'
             '\n * "--define" or "-D"'
             '\n * "--rose-template-variable" or "-S"'
         )
         return msg
 
 
-def pre_configure(srcdir=None, opts=None, rundir=None):
-    srcdir, rundir = paths_to_pathlib([srcdir, rundir])
+def pre_configure(srcdir, opts):
+    srcdir = Path(srcdir)
     return get_rose_vars(srcdir=srcdir, opts=opts)
 
 
-def post_install(srcdir=None, opts=None, rundir=None):
+def post_install(srcdir, opts, rundir):
     if not rose_config_exists(srcdir, opts):
         return False
     srcdir, rundir = paths_to_pathlib([srcdir, rundir])
     results = {}
     copy_config_file(srcdir=srcdir, rundir=rundir)
     results['record_install'] = record_cylc_install_options(
         srcdir=srcdir, opts=opts, rundir=rundir
@@ -71,14 +72,22 @@
     results['fileinstall'] = rose_fileinstall(
         srcdir=srcdir, opts=opts, rundir=rundir
     )
     # Finally dump a log of the rose-conf in its final state.
     if results['fileinstall']:
         dump_rose_log(rundir=rundir, node=results['fileinstall'])
 
+    # Having dumped the config we clear rose options
+    # as they do not apply after this.
+    # see https://github.com/cylc/cylc-rose/pull/312
+    opts.rose_template_vars = []
+    opts.opt_conf_keys = []
+    opts.defines = []
+    os.unsetenv(ROSE_SUITE_OPT_CONF_KEYS)
+
     return results
 
 
 def get_rose_vars(srcdir=None, opts=None):
     """Load template variables from Rose suite configuration.
 
     Loads the Rose suite configuration tree from the filesystem
```

### Comparing `cylc-rose-1.3.3/cylc/rose/jinja2_parser.py` & `cylc-rose-1.3.4/cylc/rose/jinja2_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.3/cylc/rose/platform_utils.py` & `cylc-rose-1.3.4/cylc/rose/platform_utils.py`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.3/cylc/rose/stem.py` & `cylc-rose-1.3.4/cylc/rose/stem.py`

 * *Files identical despite different names*

### Comparing `cylc-rose-1.3.3/cylc/rose/utilities.py` & `cylc-rose-1.3.4/cylc/rose/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from metomi.rose.config_processor import ConfigProcessError
 from metomi.rose.env import env_var_process, UnboundEnvironmentVariableError
 
 if TYPE_CHECKING:
     from optparse import Values
 
 
+ROSE_SUITE_OPT_CONF_KEYS = "ROSE_SUITE_OPT_CONF_KEYS"
 SECTIONS = {'jinja2:suite.rc', 'empy:suite.rc', 'template variables'}
 SET_BY_CYLC = 'set by Cylc'
 ROSE_ORIG_HOST_INSTALLED_OVERRIDE_STRING = (
     ' ROSE_ORIG_HOST set by cylc install.'
 )
 MESSAGE = 'message'
 ALL_MODES = 'all modes'
@@ -253,15 +254,15 @@
             specification of optional configuarations.
     Returns:
         A Rose ConfigTree object.
     """
     opt_conf_keys = []
 
     # get optional config key set as environment variable:
-    opt_conf_keys_env = os.getenv("ROSE_SUITE_OPT_CONF_KEYS")
+    opt_conf_keys_env = os.getenv(ROSE_SUITE_OPT_CONF_KEYS)
     if opt_conf_keys_env:
         opt_conf_keys += shlex.split(opt_conf_keys_env)
 
     # ... or as command line options
     if opts and 'opt_conf_keys' in dir(opts) and opts.opt_conf_keys:
         if isinstance(opts.opt_conf_keys, str):
             opt_conf_keys += opts.opt_conf_keys.split()
@@ -587,16 +588,16 @@
         ...     mp.setenv('ROSE_SUITE_OPT_CONF_KEYS', 'bet')
         ...     merge_opts(conf, 'gimmel')
         'aleph bet gimmel'
     """
     all_opt_conf_keys = []
     if 'opts' in config:
         all_opt_conf_keys.append(config['opts'].value)
-    if "ROSE_SUITE_OPT_CONF_KEYS" in os.environ:
-        all_opt_conf_keys.append(os.environ["ROSE_SUITE_OPT_CONF_KEYS"])
+    if ROSE_SUITE_OPT_CONF_KEYS in os.environ:
+        all_opt_conf_keys.append(os.environ[ROSE_SUITE_OPT_CONF_KEYS])
     if opt_conf_keys and isinstance(opt_conf_keys, str):
         all_opt_conf_keys.append(opt_conf_keys)
     if opt_conf_keys and isinstance(opt_conf_keys, list):
         all_opt_conf_keys += opt_conf_keys
     return simplify_opts_strings(' '.join(all_opt_conf_keys))
```

### Comparing `cylc-rose-1.3.3/cylc_rose.egg-info/PKG-INFO` & `cylc-rose-1.3.4/cylc_rose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-rose
-Version: 1.3.3
+Version: 1.3.4
 Summary: A Cylc plugin providing support for the Rose rose-suite.conf file.
 Home-page: https://cylc.github.io/cylc-doc/latest/html/plugins/cylc-rose.html
 Author: British Crown (Met Office) & Contributors
 Author-email: metomi@metoffice.gov.uk
 License: GPL
 Keywords: cylc,rose,workflow,configuration,workflow-engine,workflow-automation,workflow-management
 Platform: any
```

### Comparing `cylc-rose-1.3.3/cylc_rose.egg-info/requires.txt` & `cylc-rose-1.3.4/cylc_rose.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 metomi-rose<2.3.0,>=2.1.0
-cylc-flow==8.2.*
+cylc-flow<8.3,>8.2.5
 metomi-isodatetime
 ansimarkup
 jinja2
 
 [all]
 coverage>=5.0.0
 pytest
```

### Comparing `cylc-rose-1.3.3/setup.cfg` & `cylc-rose-1.3.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 [options]
 packages = find_namespace:
 python_requires = >=3.7
 include_package_data = True
 install_requires = 
 	metomi-rose>=2.1.0, <2.3.0
-	cylc-flow==8.2.*
+	cylc-flow>8.2.5, <8.3
 	metomi-isodatetime
 	ansimarkup
 	jinja2
 
 [options.packages.find]
 include = cylc*
```

### Comparing `cylc-rose-1.3.3/setup.py` & `cylc-rose-1.3.4/setup.py`

 * *Files identical despite different names*

