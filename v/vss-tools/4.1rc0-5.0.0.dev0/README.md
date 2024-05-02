# Comparing `tmp/vss-tools-4.1rc0.tar.gz` & `tmp/vss_tools-5.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss-tools-4.1rc0.tar", last modified: Fri Dec  1 15:46:00 2023, max compression
+gzip compressed data, was "vss_tools-5.0.0.dev0.tar", last modified: Thu May  2 13:25:05 2024, max compression
```

## Comparing `vss-tools-4.1rc0.tar` & `vss_tools-5.0.0.dev0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.956628 vss-tools-4.1rc0/
--rw-r--r--   0 erik      (1000) erik      (1000)    16725 2023-10-18 07:14:13.000000 vss-tools-4.1rc0/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)       23 2023-12-01 12:16:45.000000 vss-tools-4.1rc0/MANIFEST.in
--rw-r--r--   0 erik      (1000) erik      (1000)     2190 2023-12-01 15:46:00.956628 vss-tools-4.1rc0/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     1794 2023-12-01 12:16:45.000000 vss-tools-4.1rc0/README-PYPI.md
--rw-r--r--   0 erik      (1000) erik      (1000)    11798 2023-12-01 15:41:27.000000 vss-tools-4.1rc0/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)       90 2023-10-18 07:14:13.000000 vss-tools-4.1rc0/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-12-01 15:46:00.956628 vss-tools-4.1rc0/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     1922 2023-12-01 15:43:47.000000 vss-tools-4.1rc0/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.948628 vss-tools-4.1rc0/vspec/
--rwxr-xr-x   0 erik      (1000) erik      (1000)    36655 2023-12-01 15:14:41.000000 vss-tools-4.1rc0/vspec/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)      497 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/loggingconfig.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.952628 vss-tools-4.1rc0/vspec/model/
--rw-r--r--   0 erik      (1000) erik      (1000)      263 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/model/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     8174 2023-12-01 15:14:41.000000 vss-tools-4.1rc0/vspec/model/constants.py
--rw-r--r--   0 erik      (1000) erik      (1000)      844 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/model/exceptions.py
--rw-r--r--   0 erik      (1000) erik      (1000)    19844 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec/model/vsstree.py
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-10-18 07:14:13.000000 vss-tools-4.1rc0/vspec/py.typed
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.952628 vss-tools-4.1rc0/vspec/utils/
--rw-r--r--   0 erik      (1000) erik      (1000)      850 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec/utils/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2366 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec/utils/idgen_utils.py
--rw-r--r--   0 erik      (1000) erik      (1000)      774 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/utils/stringstyle.py
--rw-r--r--   0 erik      (1000) erik      (1000)     6777 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec/utils/vss2id_val.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.952628 vss-tools-4.1rc0/vspec/vssexporters/
--rw-r--r--   0 erik      (1000) erik      (1000)      263 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4828 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2binary.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3365 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2csv.py
--rw-r--r--   0 erik      (1000) erik      (1000)    12074 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2ddsidl.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2714 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2franca.py
--rw-r--r--   0 erik      (1000) erik      (1000)     5191 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2graphql.py
--rw-r--r--   0 erik      (1000) erik      (1000)     5285 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2id.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4307 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2json.py
--rw-r--r--   0 erik      (1000) erik      (1000)     5792 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2jsonschema.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     6085 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2protobuf.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4226 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2yaml.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      439 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2csv.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      439 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2ddsidl.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      441 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2franca.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      446 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2graphql.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      427 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec2id.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      441 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2json.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      453 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2jsonschema.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      449 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2protobuf.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)    10878 2023-12-01 15:41:27.000000 vss-tools-4.1rc0/vspec2x.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      441 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2yaml.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.956628 vss-tools-4.1rc0/vss_tools.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     2190 2023-12-01 15:46:00.000000 vss-tools-4.1rc0/vss_tools.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      998 2023-12-01 15:46:00.000000 vss-tools-4.1rc0/vss_tools.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-12-01 15:46:00.000000 vss-tools-4.1rc0/vss_tools.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       59 2023-12-01 15:46:00.000000 vss-tools-4.1rc0/vss_tools.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        6 2023-12-01 15:46:00.000000 vss-tools-4.1rc0/vss_tools.egg-info/top_level.txt
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/
+-rw-r--r--   0 erik      (1000) erik      (1000)    16725 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)       23 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 erik      (1000) erik      (1000)     2197 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1797 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/README-PYPI.md
+-rw-r--r--   0 erik      (1000) erik      (1000)    13319 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)      253 2024-04-30 07:46:11.000000 vss_tools-5.0.0.dev0/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1886 2024-05-02 12:01:50.000000 vss_tools-5.0.0.dev0/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/vspec/
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    37003 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      497 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/loggingconfig.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/vspec/model/
+-rw-r--r--   0 erik      (1000) erik      (1000)      263 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/model/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9629 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/model/constants.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      844 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/model/exceptions.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    21714 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/model/vsstree.py
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/py.typed
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/vspec/utils/
+-rw-r--r--   0 erik      (1000) erik      (1000)      850 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/utils/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2799 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/utils/idgen_utils.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      774 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/utils/stringstyle.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     7064 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/utils/vss2id_val.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2163 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/vspec2vss_config.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    10076 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/vspec2x.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1346 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vss2x.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/vspec/vssexporters/
+-rw-r--r--   0 erik      (1000) erik      (1000)      263 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     5057 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2binary.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3424 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2csv.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    12374 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2ddsidl.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3232 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2franca.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     5418 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2graphql.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     6184 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2id.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4409 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2json.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     6110 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2jsonschema.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     6644 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2protobuf.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4293 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec/vssexporters/vss2yaml.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      684 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2csv.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      711 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2ddsidl.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      714 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2franca.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      723 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2graphql.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      677 2024-04-29 11:03:17.000000 vss_tools-5.0.0.dev0/vspec2id.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      690 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2json.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      726 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2jsonschema.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      730 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2protobuf.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      690 2024-04-30 07:38:36.000000 vss_tools-5.0.0.dev0/vspec2yaml.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-02 13:25:04.994572 vss_tools-5.0.0.dev0/vss_tools.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2197 2024-05-02 13:25:04.000000 vss_tools-5.0.0.dev0/vss_tools.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1045 2024-05-02 13:25:04.000000 vss_tools-5.0.0.dev0/vss_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-02 13:25:04.000000 vss_tools-5.0.0.dev0/vss_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       59 2024-05-02 13:25:04.000000 vss_tools-5.0.0.dev0/vss_tools.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        6 2024-05-02 13:25:04.000000 vss_tools-5.0.0.dev0/vss_tools.egg-info/top_level.txt
```

### Comparing `vss-tools-4.1rc0/LICENSE` & `vss_tools-5.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `vss-tools-4.1rc0/PKG-INFO` & `vss_tools-5.0.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vss-tools
-Version: 4.1rc0
+Version: 5.0.0.dev0
 Summary: COVESA Vehicle Signal Specification tooling.
 Home-page: https://github.com/COVESA/vss-tools
 License: Mozilla Public License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml>=5.1
@@ -34,15 +34,15 @@
 
 If you just want the latest version this should be sufficient:
 
 ```sh
 pip install vss-tools
 ```
 
-When installed tools like `vspec2x.py` shall be available on your path.
+When installed tools like `vspec2json.py` shall be available on your path.
 
 For more information see the [VSS-Tools wiki](https://github.com/COVESA/vss-tools/wiki/PyPI-packing)
 
 ## Usage
 
 For more information please visit the [COVESA VSS-Tools repository](https://github.com/COVESA/vss-tools).
```

### Comparing `vss-tools-4.1rc0/README-PYPI.md` & `vss_tools-5.0.0.dev0/README-PYPI.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 If you just want the latest version this should be sufficient:
 
 ```sh
 pip install vss-tools
 ```
 
-When installed tools like `vspec2x.py` shall be available on your path.
+When installed tools like `vspec2json.py` shall be available on your path.
 
 For more information see the [VSS-Tools wiki](https://github.com/COVESA/vss-tools/wiki/PyPI-packing)
 
 ## Usage
 
 For more information please visit the [COVESA VSS-Tools repository](https://github.com/COVESA/vss-tools).
```

### Comparing `vss-tools-4.1rc0/README.md` & `vss_tools-5.0.0.dev0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -21,125 +21,157 @@
 A tool in the Contributed Tools category may be moved to the Obsolete category if it has been non-functional for at least 6 months.
 Tools in the Obsolete Tools category may be deleted after 12 months.
 
 Examples on tool usage can be found in the [VSS Makefile](https://github.com/COVESA/vehicle_signal_specification/blob/master/Makefile) and in tool-specific documentation, if existing.
 
  Tool | Description | Tool Category         | Documentation                                                                                                         |
 | ------------------ | ----------- |-----------------------|-----------------------------------------------------------------------------------------------------------------------|
-| [vspec2x.py](vspec2x.py) | Parses and expands VSS into different text based output formats. Currently supports `json`, `yaml`,`csv`,`idl`  | Community Supported   | Try `./vspec2x --help` or check [vspec2x documentation](docs/vspec2x.md)                                              |
-[vspec2csv.py](vspec2csv.py) | Shortcut for [vspec2x.py](vspec2x.py) generating CSV output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
-[vspec2ddsidl.py](vspec2ddsidl.py) | Shortcut for [vspec2x.py](vspec2x.py) generating DDS-IDL output | Community Supported   | [VSS2DDSIDL Documentation](docs/VSS2DDSIDL.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
-[vspec2json.py](vspec2json.py) |  Shortcut for [vspec2x.py](vspec2x.py) generating JSON output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
-[vspec2yaml.py](vspec2yaml.py) | Shortcut for [vspec2x.py](vspec2x.py) generating flattened YAML output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
+[vspec2csv.py](vspec2csv.py) | Generating CSV output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
+[vspec2ddsidl.py](vspec2ddsidl.py) | Generating DDS-IDL output | Community Supported   | [VSS2DDSIDL Documentation](docs/VSS2DDSIDL.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
+[vspec2json.py](vspec2json.py) |  Generating JSON output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
+[vspec2yaml.py](vspec2yaml.py) | Generating flattened YAML output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
 [vspec2binary.py](vspec2binary.py) | The binary toolset consists of a tool that translates the VSS YAML specification to the binary file format (see below), and two libraries that provides methods that are likely to be needed by a server that manages the VSS tree, one written in C, and one in Go | Community Supported   | [vspec2binary Documentation](binary/README.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
 [vspec2franca.py](vspec2franca.py) | Parses and expands a VSS and generates a Franca IDL specification | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
 [vspec2c.py](obsolete/vspec2c.py) | The vspec2c tooling allows a vehicle signal specification to be translated from its source YAML file to native C code that has the entire specification encoded in it. | Obsolete (2022-11-01) | [Documentation](obsolete/vspec2c/README.md)                                                                           |
 [vspec2ocf.py](obsolete/ocf/vspec2ocf.py) | Parses and expands a VSS and generates a OCF specification | Obsolete (2022-11-01) | -                                                                                                                     |
 [vspec2protobuf.py](vspec2protobuf.py) | Parses and expands a VSS and generates a Protobuf specification | Contrib               | -                                                                                                                     |
 [vspec2ttl.py](contrib/vspec2ttl/vspec2ttl.py) | Parses and expands a VSS and generates a TTL specification | Contrib               | -                                                                                                                     |
 [vspec2graphql.py](vspec2graphql.py) | Parses and expands a VSS and generates a GraphQL specification | Community Supported   | [Documentation](docs/VSS2GRAPHQL.md)                                                                                  |
 [vspec2id.py](vspec2id.py) | Generates and validates static UIDs for a VSS | WIP                   | [vspec2id Documentation](./docs/vspec2id.md)                                                                          |
 
 ## Tool Architecture
 
 All current tools are based on common Python functionality in the `vspec` folder to read, parse and expand a Vehicle Signal Specification files(*.vspec files). As an example, if the standard [VSS root file](https://github.com/COVESA/vehicle_signal_specification/blob/master/spec/VehicleSignalSpecification.vspec) is given as input then the Python tooling will read all included files, do a validation of the content, expand any instances used and create an in-memory representation which then can be used by specialized tools to generate the wanted output.
 
+## Compatibility with VSS
+
+The [COVESA VSS project repository](https://github.com/COVESA/vehicle_signal_specification) includes vss-tools as a submodule.
+The vss-tools version linked by the VSS repository is the preferred vss-tools version to use for that particular version of the VSS repository. It is not guaranteed that newer or older versions of vss-tools can successfully handle that particular version of the VSS repository. The table below gives an overview of basic version support for`vspec2json.py`,
+other exporters may have stricter requirements.
+
+VSS-tools version | Supported VSS versions | Comments
+-----------------|------------------------|----------------
+`v3.0`| `v3.0` - `v3.1.1`
+`v3.1`| `v3.0` -`v4.0`
+`v4.0`| `v4.0`
+`v4.1`| `v4.0` -
+`<latest source>`| `v4.0` -
+
+### Changes affecting compatibility
+
+Examples on changes affecting compatibility
+
+* VSS version `v4.1` introduced a new syntax for the unit files that cannot be handled by `vss-tools < v4.1`
+* From `v4.0` vss-tools expects unit file to be explicitly specified or provided in the same directory as the VSS input.
+  VSS `v3.1` is the first VSS version including a unit file in the VSS repository.
+  This means vss-tools from `v4.0` onwards cannot handle VSS-versions prior to VSS `v3.1`
+* VSS-tools `v3.1` only supported `default` for attributes, resulting in that newer VSS-versions is not supported.
+* VSS-tools `v4.0` requires case-sensitive for type, resulting in that VSS versions `v3.1` and earlier is not supported.
+
 ## Getting started
 
 ## Prerequisites
 
 * If your environment behind a (corporate) proxy, the following environments variables must typically be set: `http_proxy` and `https_proxy` (including authentication e.g., `http://${proxy_username):$(proxy_password)@yourproxy.yourdomain`).
 * If using `apt` and you are behind a proxy, you may also need to configure proxy in `/etc/apt/apt.conf.d/proxy.conf`.
 
-## Basic Setup
-
-The tools are in [continuous integration](https://github.com/COVESA/vss-tools/blob/master/.github/workflows/buildcheck.yml) tested using Python 3.8.12,
-but they are generally expected to be compatible with at least Python 3.8, 3.9 and 3.10.
-The setup example shown below is based on a fresh minimal install of Ubuntu 22.04.
-
-The first step is to make sure that python and required dependencies are installed. A possible installation flow is shown below.
-
-
-```sh
-# Install Python, in this case Python 3.10 as that is a version available on the update sites of Ununtu 22.04
-sudo apt install python3.10
-
-# For convenience make Python 3.10 available as default Python
-sudo update-alternatives --install /usr/bin/python python /usr/bin/python3.10 100
-
-# Install required dependencies, running pip without sudo means that a user installation will be performed
-sudo apt install pip
-pip install anytree deprecation graphql-core
-```
-
-
-```sh
-# Install protobuf compiler
-sudo apt install -y protobuf-compiler
-protoc --version  # Ensure compiler version is 3+
-```
-
-The environment can be tested by calling one of the tools without arguments, then usage instructions shall be printed similar to below.
-
-```sh
-user@ubuntu:~/vss-tools$ ./vspec2csv.py
-usage: vspec2csv.py [-h] [-I dir] [-e EXTENDED_ATTRIBUTES] [-s] [--abort-on-unknown-attribute] [--abort-on-name-style] [--format format] [--uuid]
-                    [--no-uuid] [-o overlays] [-u unit_file] [--json-all-extended-attributes] [--json-pretty] [--yaml-all-extended-attributes]
-                    [-v version] [--all-idl-features] [--gqlfield GQLFIELD GQLFIELD]
-                    <vspec_file> <output_file>
-vspec2csv.py: error: the following arguments are required: <vspec_file>, <output_file>
+## Environment and Python Version
 
-```
+This repository use the Github `ubuntu-latest` [runner-image](https://github.com/actions/runner-images) for continuous nntegration.
+The Python version used is typically the [default version](https://packages.ubuntu.com/search?keywords=python3) for that Ubuntu release,
+currently Python `3.10.6`.
+Other environments and Python versions may be supported, but are not tested as part of continuous integration or relase testing.
 
-## Advanced Setup
+## Setup using venv
 
 If you want to run the tools with a specific Python version, or you do not want to change your current/global Python configuration you can use pyenv/pipenv.
 If you use a custom pip installation directory, set the `PYTHONPATH` environment variable to the directory that you set in the `pip.ini` file.
 [pipenv](https://pypi.org/project/pipenv/) is a tool that manages a virtual environment and install the package and its dependencies, making the process much simpler and predictable, since the `Pipfile` states the dependencies, while `Pipfile.lock` freezes the exact version in use.
 
 The setup example shown below is based on a fresh minimal install of Ubuntu 22.04.
 
-The first step is to make sure that pyenv and the wanted Python version (in the example 3.8.12) is installed
+The first step is to make sure that pyenv and the wanted Python version (in the example 3.10.6) is installed
 
 ```sh
 # Install dependencies, to be able to use curl and build python from source
 sudo apt-get install make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
 
 # Fetch and install pyenv and update variables
 curl https://pyenv.run | bash
 export PYENV_ROOT="$HOME/.pyenv"
 command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"
 eval "$(pyenv init -)"
 
-# Build and install wanted python version
-pyenv install 3.8.12
+# Build and install wanted python version, shall match the version specified in Pipfile
+pyenv install 3.10.6
 ```
 
 Install this project and its dependencies in the local `.venv` folder in this project, then use it (`pipenv shell`):
 
 ```sh
 export PIPENV_VENV_IN_PROJECT=1 # will create a local `.venv` in the project, otherwise uses global location
 pip install pipenv
-export PATH=/home/user/.local/bin:$PATH
+export PATH=/home/${USER}/.local/bin:${PATH}
 pipenv install --dev # install the development dependencies as well
 ```
 
 Then the virtual environment can be started and tested using (`pipenv shell`):
 
 ```sh
 user@ubuntu:~/vss-tools$ pipenv shell
 Launching subshell in virtual environment...
 user@ubuntu:~/vss-tools$  . /home/user/vss-tools/.venv/bin/activate
 (vss-tools) user@ubuntu:~/vss-tools$ ./vspec2yaml.py
 usage: vspec2yaml.py [-h] [-I dir] [-e EXTENDED_ATTRIBUTES] [-s] [--abort-on-unknown-attribute] [--abort-on-name-style] [--format format] [--uuid]
-                     [--no-uuid] [-o overlays] [-u unit_file] [--json-all-extended-attributes] [--json-pretty] [--yaml-all-extended-attributes]
+                     [-o overlays] [-u unit_file] [--json-all-extended-attributes] [--json-pretty] [--yaml-all-extended-attributes]
                      [-v version] [--all-idl-features] [--gqlfield GQLFIELD GQLFIELD]
                      <vspec_file> <output_file>
 vspec2yaml.py: error: the following arguments are required: <vspec_file>, <output_file>
 ```
 
+## Native Setup
+
+It is also possible to run the tools in native setup if you have a matching Python environment.
+The setup example shown below is based on a fresh minimal install of Ubuntu 22.04.
+
+The first step is to make sure that python and required dependencies are installed. A possible installation flow is shown below.
+
+
+```sh
+# Install Python, in this case Python 3.10 as that is a version available on the update sites of Ununtu 22.04
+sudo apt install python3.10
+
+# For convenience make Python 3.10 available as default Python
+sudo update-alternatives --install /usr/bin/python python /usr/bin/python3.10 100
+
+# Install required dependencies, running pip without sudo means that a user installation will be performed
+sudo apt install pip
+pip install anytree deprecation graphql-core
+```
+
+The environment can be tested by calling one of the tools without arguments, then usage instructions shall be printed similar to below.
+
+```sh
+user@ubuntu:~/vss-tools$ ./vspec2csv.py
+usage: vspec2csv.py [-h] [-I dir] [-e EXTENDED_ATTRIBUTES] [-s] [--abort-on-unknown-attribute] [--abort-on-name-style] [--format format] [--uuid]
+                    [-o overlays] [-u unit_file] [--json-all-extended-attributes] [--json-pretty] [--yaml-all-extended-attributes]
+                    [-v version] [--all-idl-features] [--gqlfield GQLFIELD GQLFIELD]
+                    <vspec_file> <output_file>
+vspec2csv.py: error: the following arguments are required: <vspec_file>, <output_file>
+
+```
+
+## Installing additional tools
+
+If you intend to run testcases related to `vspec2protobuf.py` you need to install the protobuf compiler
+
+```sh
+sudo apt install -y protobuf-compiler
+protoc --version  # Ensure compiler version is 3+
+```
+
 ## Pre-commit set up
 This repository is set up to use pre-commit hooks. After you clone the project, run `pre-commit install` to install pre-commit into your git hooks. pre-commit will now run on every commit. Every time you clone a project using pre-commit running pre-commit install should always be the first thing you do.
 
 ## Building and installing with Pip
 
 For usage of VSS-Tools with Pip (PyPI) please see [README-PYPI.md](README-PYPI.md)
```

### Comparing `vss-tools-4.1rc0/setup.py` & `vss_tools-5.0.0.dev0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,19 +27,18 @@
 long_description = (this_directory / "README-PYPI.md").read_text()
 
 setup(
     name='vss-tools',
     description='COVESA Vehicle Signal Specification tooling.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='4.1rc0',
     url='https://github.com/COVESA/vss-tools',
     license='Mozilla Public License 2.0',
     packages=find_packages(exclude=('tests', 'contrib')),
-    scripts=['vspec2csv.py', 'vspec2x.py', 'vspec2franca.py', 'vspec2json.py', 'vspec2jsonschema.py',
+    scripts=['vspec2csv.py', 'vspec2franca.py', 'vspec2json.py', 'vspec2jsonschema.py',
              'vspec2ddsidl.py', 'vspec2yaml.py', 'vspec2protobuf.py', 'vspec2graphql.py',
              'vspec2id.py'],
     python_requires='>=3.8',
     install_requires=['pyyaml>=5.1', 'anytree>=2.8.0', 'deprecation>=2.1.0', 'graphql-core'],
     tests_require=['pytest>=2.7.2'],
     package_data={'vspec': [
         'py.typed'
```

### Comparing `vss-tools-4.1rc0/vspec/__init__.py` & `vss_tools-5.0.0.dev0/vspec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,14 +294,21 @@
 def verify_mandatory_attributes(node, abort_on_unknown_attribute: bool):
     """
     Verify that mandatory attributes are present.
     Need to be checked first after overlays (if any) have been applied, as attributes are not
     mandatory in individual files but only in the final tree
     """
     if isinstance(node, VSSNode):
+        if node.delete:
+            logging.info(
+                f"Node {node.qualified_name()} will be deleted. Please note, that if {node.qualified_name()} "
+                f"is a branch all subsequent nodes will also be deleted irrespective of their 'delete' value."
+            )
+            node.parent = None
+            node.children = []
         node.verify_attributes(abort_on_unknown_attribute)
         for child in node.children:
             verify_mandatory_attributes(child, abort_on_unknown_attribute)
 
 
 #
 # Verify that we are using correct YAML in the model
```

### Comparing `vss-tools-4.1rc0/vspec/model/exceptions.py` & `vss_tools-5.0.0.dev0/vspec/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.1rc0/vspec/model/vsstree.py` & `vss_tools-5.0.0.dev0/vspec/model/vsstree.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,36 @@
 #
 # This program and the accompanying materials are made available under the
 # terms of the Mozilla Public License 2.0 which is available at
 # https://www.mozilla.org/en-US/MPL/2.0/
 #
 # SPDX-License-Identifier: MPL-2.0
 
-from anytree import Node, Resolver, ChildResolverError, RenderTree  # type: ignore[import]
-from .constants import VSSType, VSSDataType, VSSUnitCollection, VSSUnit
-from .exceptions import NameStyleValidationException, \
-    ImpossibleMergeException, IncompleteElementException
-from typing import Any, Optional, Set, List
 import copy
+import logging
 import re
 import sys
-import logging
+from typing import Any, List, Optional, Set
+
+from anytree import (  # type: ignore[import]
+    ChildResolverError,
+    Node,
+    RenderTree,
+    Resolver,
+)
+
+from .constants import VSSDataType, VSSType, VSSUnit, VSSUnitCollection
+from .exceptions import (
+    ImpossibleMergeException,
+    IncompleteElementException,
+    NameStyleValidationException,
+)
 
 DEFAULT_SEPARATOR = "."
-ARRAY_SUBSCRIPT_OP = '[]'
+ARRAY_SUBSCRIPT_OP = "[]"
 
 
 class VSSNode(Node):
     """Representation of an VSS element according to the vehicle signal specification."""
 
     type: VSSType
     description = None
@@ -34,17 +44,35 @@
     data_type_str: str = ""
     # data type - enum representation if available
     datatype: Optional[VSSDataType]
 
     # The node types that the nodes can take
     available_types: Set[str] = set()
 
-    core_attributes = ["type", "children", "datatype", "description", "unit", "uuid", "min", "max", "allowed",
-                       "instantiate", "aggregate", "default", "instances", "deprecation", "arraysize",
-                       "comment", "$file_name$", "fka"]
+    core_attributes = [
+        "type",
+        "children",
+        "datatype",
+        "description",
+        "unit",
+        "uuid",
+        "min",
+        "max",
+        "allowed",
+        "instantiate",
+        "aggregate",
+        "default",
+        "instances",
+        "deprecation",
+        "arraysize",
+        "comment",
+        "$file_name$",
+        "fka",
+        "delete",
+    ]
 
     # List of accepted extended attributes. In strict terminate if an attribute is
     # neither in core or extended,
     whitelisted_extended_attributes: List[str] = []
 
     unit: Optional[VSSUnit] = None
 
@@ -57,164 +85,215 @@
 
     default = ""
 
     instances = None
     expanded = False
     deprecation = ""
     fka = ""
+    delete: bool = False
 
     def __deepcopy__(self, memo):
         # Deep copy of source_dict and children needed as overlay or programmatic changes
         # in exporters otherwise risk changing values not only for current instances but also for others
-        return VSSNode(self.name, copy.deepcopy(self.source_dict), self.available_types.copy(),
-                       parent=None, children=copy.deepcopy(self.children, memo))
-
-    def __init__(self, name, source_dict: dict, available_types: Set[str], parent=None,
-                 children=None, break_on_unknown_attribute=False, break_on_name_style_violation=False):
+        return VSSNode(
+            self.name,
+            copy.deepcopy(self.source_dict),
+            self.available_types.copy(),
+            parent=None,
+            children=copy.deepcopy(self.children, memo),
+        )
+
+    def __init__(
+        self,
+        name,
+        source_dict: dict,
+        available_types: Set[str],
+        parent=None,
+        children=None,
+        break_on_unknown_attribute=False,
+        break_on_name_style_violation=False,
+    ):
         """Creates an VSS Node object from parsed yaml instance represented as a dict.
 
-            Args:
-                name: Name of this VSS instance.
-                source_dict: VSS instance represented as dict from yaml parsing.
-                available_types: Available node types asa string list
-                parent: Optional parent of this node instance.
-                children: Optional children instances of this node.
-                break_on_unknown_attribute: Throw if the node contains attributes not in core VSS specification
-                break_on_name_style_vioation: Throw if this node's name is not follwing th VSS recommended style
+        Args:
+            name: Name of this VSS instance.
+            source_dict: VSS instance represented as dict from yaml parsing.
+            available_types: Available node types asa string list
+            parent: Optional parent of this node instance.
+            children: Optional children instances of this node.
+            break_on_unknown_attribute: Throw if the node contains attributes not in core VSS specification
+            break_on_name_style_vioation: Throw if this node's name is not follwing th VSS recommended style
 
-            Returns:
-                VSSNode object according to the Vehicle Signal Specification.
+        Returns:
+            VSSNode object according to the Vehicle Signal Specification.
 
         """
 
         super().__init__(name, parent, children)
         self.available_types = available_types
 
-        if (source_dict["type"] not in available_types):
+        if source_dict["type"] not in available_types:
             logging.error(
-                f'Invalid type provided for VSSNode: {source_dict["type"]}. Allowed types are {self.available_types}')
+                f'Invalid type provided for VSSNode: {source_dict["type"]}. Allowed types are {self.available_types}'
+            )
             sys.exit(-1)
 
         self.source_dict = source_dict
         self.unpack_source_dict()
 
-        if (self.is_property() and not self.parent.is_struct()):
-            logging.error(f"Orphan property detected. {self.name} is not defined under a struct")
+        if self.is_property() and not self.parent.is_struct():
+            logging.error(
+                f"Orphan property detected. {self.name} is not defined under a struct"
+            )
             sys.exit(-1)
 
         try:
             self.validate_name_style(self.source_dict["$file_name$"])
         except NameStyleValidationException as e:
-            logging.warning(f"Exception: {e}")
+            info_string = str(e)
             if break_on_name_style_violation:
+                logging.warning(info_string)
                 logging.error("You asked for strict checking. Terminating.")
                 sys.exit(-1)
+            else:
+                logging.info(info_string)
 
     def unpack_source_dict(self):
         self.extended_attributes = self.source_dict.copy()
 
         # Clean special cases
         if "children" in self.extended_attributes:
             del self.extended_attributes["children"]
         if "type" in self.extended_attributes:
             del self.extended_attributes["type"]
 
         def extractCoreAttribute(name: str):
-            if name != "children" and name != "type" and name in self.source_dict.keys():
+            if (
+                name != "children"
+                and name != "type"
+                and name in self.source_dict.keys()
+            ):
                 setattr(self, name, self.source_dict[name])
                 del self.extended_attributes[name]
 
         self.type = VSSType.from_str(self.source_dict["type"])
 
         for attribute in VSSNode.core_attributes:
             extractCoreAttribute(attribute)
 
         # Datatype and unit need special handling, so we do some further analysis
-        # self.data_type shall only be set if base type is a primitive (VSSDataType)
-        if self.has_datatype():
-            if self.is_signal() or self.is_property():
-                self.data_type_str = self.source_dict["datatype"]
-                self.validate_and_set_datatype()
-            else:
-                logging.error("Item %s cannot have datatype, only allowed for signal and property!", self.name)
-                sys.exit(-1)
-        elif (self.is_signal() or self.is_property()):
-            raise IncompleteElementException(
-                (f"Incomplete element {self.name} from {self.source_dict['$file_name$']}: "
-                 f"Elements of type {self.type.value} need to have a datatype declared."))
 
         # Units are applicable only for primitives. Not user defined types.
         if self.has_unit():
 
             if not (self.is_signal() or self.is_property()):
-                logging.error("Item %s cannot have unit, only allowed for signal and property!", self.name)
+                logging.error(
+                    "Item %s cannot have unit, only allowed for signal and property!",
+                    self.name,
+                )
                 sys.exit(-1)
 
             unit = self.source_dict["unit"]
             self.unit = VSSUnitCollection.get_unit(unit)
             if self.unit is None:
-                logging.error(f"Unknown unit {unit} for signal {self.qualified_name()}. Terminating.")
+                logging.error(
+                    f"Unknown unit {unit} for signal {self.qualified_name()}. Terminating."
+                )
+                sys.exit(-1)
+
+        # self.data_type shall only be set if base type is a primitive (VSSDataType)
+        if self.has_datatype():
+            if self.is_signal() or self.is_property():
+                self.data_type_str = self.source_dict["datatype"]
+                self.validate_and_set_datatype()
+            else:
+                logging.error(
+                    "Item %s cannot have datatype, only allowed for signal and property!",
+                    self.name,
+                )
                 sys.exit(-1)
+        elif self.is_signal() or self.is_property():
+            raise IncompleteElementException(
+                f"Incomplete element {self.name} from {self.source_dict['$file_name$']}: "
+                f"Elements of type {self.type.value} need to have a datatype declared."
+            )
+
+        # Datatype check for unit performed first when we have set the right datatype
+        if self.has_unit():
 
             if not self.has_datatype():
-                logging.error("Unit specified for item not using standard datatype: %s", self.name)
+                logging.error(
+                    "Unit specified for item not using standard datatype: %s", self.name
+                )
                 sys.exit(-1)
 
         if self.has_instances() and not self.is_branch():
             logging.error(
-                f"Only branches can be instantiated. {self.qualified_name()} is of type {self.type}")
+                f"Only branches can be instantiated. {self.qualified_name()} is of type {self.type}"
+            )
             sys.exit(-1)
 
     def validate_name_style(self, sourcefile):
         """Checks wether this node is adhering to VSS style conventions.
 
-            Throws NameStyleValidationException when deviations are detected. A VSS model violating
-            this conventions can still be a valid model.
+        Throws NameStyleValidationException when deviations are detected. A VSS model violating
+        this conventions can still be a valid model.
 
         """
-        camel_regexp = re.compile('[A-Z][A-Za-z0-9]*$')
-        if self.is_signal() and self.datatype == VSSDataType.BOOLEAN and not self.name.startswith("Is"):
+        camel_regexp = re.compile("[A-Z][A-Za-z0-9]*$")
+        if (
+            self.is_signal()
+            and self.datatype == VSSDataType.BOOLEAN
+            and not self.name.startswith("Is")
+        ):
             raise NameStyleValidationException(
-                (f'Boolean node "{self.name}" found in file "{sourcefile}" is not following naming conventions. ',
-                 'It is recommended that boolean nodes start with "Is".'))
+                (
+                    f'Boolean node "{self.name}" found in file "{sourcefile}" is not following naming conventions. ',
+                    'It is recommended that boolean nodes start with "Is".',
+                )
+            )
 
+        camel_regexp = re.compile('[A-Z][A-Za-z0-9]*$')
         # relax camel case requirement for struct properties
         if not self.is_property() and not camel_regexp.match(self.name):
             raise NameStyleValidationException(
-                (f'Node "{self.name}" found in file "{sourcefile}" is not following naming conventions. ',
-                 'It is recommended that node names use camel case, starting with a capital letter, ',
-                 'only using letters A-z and numbers 0-9.'))
+                (
+                    f'Node "{self.name}" found in file "{sourcefile}" is not following naming conventions. ',
+                    "It is recommended that node names use camel case, starting with a capital letter, ",
+                    "only using letters A-z and numbers 0-9.",
+                )
+            )
 
     def base_data_type_str(self) -> str:
         """
         This gives the base type of the type, i.e. without array suffix if present
         """
         suffix = "[]"
         if self.data_type_str.endswith(suffix):
-            return self.data_type_str[:-len(suffix)]
+            return self.data_type_str[: -len(suffix)]
         return self.data_type_str
 
     def qualified_name(self, separator=DEFAULT_SEPARATOR) -> str:
         """Returns fully qualified name of a VSS object (including path) using the defined separator (or default ='.')
-            Args:
-                separator: Optional parameter as custom separator between path elements of this instance
+        Args:
+            separator: Optional parameter as custom separator between path elements of this instance
 
-            Returns:
-                Fully Qualified VSS Node string representation including complete path.
+        Returns:
+            Fully Qualified VSS Node string representation including complete path.
 
         """
 
         name = self.name
 
         path = self
         while not path.is_root:
             path = path.parent
             node_name = path.name
 
-            name = "%s%s%s" % (node_name, separator, name)
+            name = f"{node_name}{separator}{name}"
         return name
 
     def is_branch(self):
         return self.type == VSSType.BRANCH
 
     def is_sensor(self):
         return self.type == VSSType.SENSOR
@@ -233,16 +312,16 @@
 
     def is_signal(self):
         return self.is_sensor() or self.is_actuator() or self.is_attribute()
 
     def is_orphan(self) -> bool:
         """Checks if this instance is a branch without any child nodes
 
-            Returns:
-                True if this instance is a branch and has no children.
+        Returns:
+            True if this instance is a branch and has no children.
         """
         if self.is_branch() or self.is_struct():
             return self.is_leaf
         return False
 
     def get_struct_qualified_name(self, struct_name) -> Optional[str]:
         """
@@ -282,72 +361,76 @@
                 return child.qualified_name()
 
         return None
 
     def is_instantiated(self) -> bool:
         """Checks if node shall be instantiated through its parent
 
-            Returns:
-                True if it shall be instantiated
+        Returns:
+            True if it shall be instantiated
         """
         return self.instantiate
 
     def has_unit(self) -> bool:
         """Checks if this instance has a unit
 
-            Returns:
-                True if this instance has a unit, False otherwise
+        Returns:
+            True if this instance has a unit, False otherwise
         """
         return hasattr(self, "unit") and self.unit is not None
 
     def get_unit(self) -> str:
         """Returns:
-                The name of the unit or empty string if no unit
+        The name of the unit or empty string if no unit
         """
         if hasattr(self, "unit") and self.unit is not None:
             return self.unit.value
         else:
-            return ''
+            return ""
 
     def has_datatype(self) -> bool:
         """Check if this instance has a datatype
 
-            Returns:
-                True if this instance has a data type, False otherwise
+        Returns:
+            True if this instance has a data type, False otherwise
         """
         return hasattr(self, "datatype") and self.datatype is not None
 
     def get_datatype(self) -> str:
         """Returns:
-                The name of the datatype or empty string if no datatype
+        The name of the datatype or empty string if no datatype
         """
         return self.data_type_str
 
     def has_instances(self) -> bool:
         """Check if this instance has a VSS instances
 
-            Returns:
-                True if this instance declares instances, False otherwise
+        Returns:
+            True if this instance declares instances, False otherwise
         """
         return hasattr(self, "instances") and self.instances is not None
 
     def merge(self, other: "VSSNode"):
         """Merges two VSSNode, other parameter overwrites the caller object,
-           if it is not None
-            Args:
-                other: other node to merge into the caller object
+        if it is not None
+         Args:
+             other: other node to merge into the caller object
         """
         if self.is_branch() and not other.is_branch():
             raise ImpossibleMergeException(
-                (f"Impossible merging {self.name} from {self.source_dict['$file_name$']} with {other.name} ",
-                 f"from {other.source_dict['$file_name$']}, can not change branch to {other.type.value}."))
+                (
+                    f"Impossible merging {self.name} from {self.source_dict['$file_name$']} with {other.name} ",
+                    f"from {other.source_dict['$file_name$']}, can not change branch to {other.type.value}.",
+                )
+            )
         elif not self.is_branch() and other.is_branch():
             raise ImpossibleMergeException(
-                (f"Impossible merging {self.name} from {self.source_dict['$file_name$']} with {other.name} "
-                 f"from {other.source_dict['$file_name$']}, can not change {self.type.value} to branch."))
+                f"Impossible merging {self.name} from {self.source_dict['$file_name$']} with {other.name} "
+                f"from {other.source_dict['$file_name$']}, can not change {self.type.value} to branch."
+            )
 
         self.source_dict.update(other.source_dict)
         self.unpack_source_dict()
 
     def validate_and_set_datatype(self):
         """
         For signals:
@@ -358,71 +441,95 @@
         1. the data type string represents the corresponding VSSDataType enumeration, OR
         2. the data type string refers to a struct name that is defined under the same branch.
         Note that only struct names relative to the branch under which they are defined are checked.
         Data types provided as fully qualified struct names are skipped from validation as they
         require the entire tree to be rendered first. These are validated after the entire tree is rendered.
         """
         is_array = ARRAY_SUBSCRIPT_OP in self.data_type_str
+        # get the base name without subscript decoration
+        undecorated_datatype_str = self.data_type_str.split(DEFAULT_SEPARATOR)[
+            -1
+        ].replace(ARRAY_SUBSCRIPT_OP, "")
+
         try:
             self.datatype = VSSDataType.from_str(self.data_type_str)
+
+            if self.unit and self.unit.allowed_datatypes:
+                if not (
+                    (undecorated_datatype_str in self.unit.allowed_datatypes)
+                    or (
+                        VSSDataType.is_numeric(self.datatype)
+                        and "numeric" in self.unit.allowed_datatypes
+                    )
+                ):
+                    logging.error(
+                        "Datatype %s not allowed for unit %s",
+                        self.data_type_str,
+                        self.unit.id,
+                    )
+                    sys.exit(-1)
         except KeyError as e:
             if self.type == VSSType.PROPERTY:
                 # Fully Qualified name as data type name
                 if DEFAULT_SEPARATOR in self.data_type_str:
                     logging.info(
-                        (f"Qualified datatype name {self.data_type_str} provided in node {self.qualified_name()}. ",
-                         "Semantic checks will be performed after the entire tree is rendered. SKIPPING NOW..."))
+                        (
+                            f"Qualified datatype name {self.data_type_str} provided in node {self.qualified_name()}. ",
+                            "Semantic checks will be performed after the entire tree is rendered. SKIPPING NOW...",
+                        )
+                    )
                 else:
-                    # get the base name without subscript decoration
-                    undecorated_datatype_str = self.data_type_str.split(
-                        DEFAULT_SEPARATOR)[-1].replace(ARRAY_SUBSCRIPT_OP, '')
                     # Custom data types can contain names defined under the
                     # same branch
                     struct_fqn = self.get_struct_qualified_name(
-                        undecorated_datatype_str)
+                        undecorated_datatype_str
+                    )
                     if struct_fqn is None:
                         logging.error(
-                            f"Data type not found. Data Type: {undecorated_datatype_str}")
+                            f"Data type not found. Data Type: {undecorated_datatype_str}"
+                        )
                         sys.exit(-1)
 
                     # replace data type with qualified name
                     if is_array:
                         self.data_type_str = struct_fqn + ARRAY_SUBSCRIPT_OP
                     else:
                         self.data_type_str = struct_fqn
             elif self.is_signal():
                 # This is a signal possibly referencing a user-defined type.
                 # Just assign the string value for now. Validation will be
                 # performed after the entire tree is rendered.
-                logging.debug(f"Possible struct-type encountered - {self.data_type_str} in node {self.name}. ")
+                logging.debug(
+                    f"Possible struct-type encountered - {self.data_type_str} in node {self.name}. "
+                )
             else:
                 raise e
             self.datatype = None  # reset the enum
 
-    def does_attribute_exist(self, other: 'VSSNode',
-                             attr_fn, other_attr_fn, other_filter_fn):
+    def does_attribute_exist(
+        self, other: "VSSNode", attr_fn, other_attr_fn, other_filter_fn
+    ):
         """
         Returns whether the an attribute of this node exists as another attribute in the specified tree
 
         Keyword arguments:
         other: Tree root of the search tree
         attr_fn: Attribute projection function for this node that takes in a VSSNode as argument.
         other_attr_fn: Attribute projection function for nodes in the search tree. The argument is of type VSSNode.
         other_filter_fn: A filter function for node search in the "other" tree. The argument is of type VSSNode.
         """
         key = attr_fn(self)
-        return key in set(VSSNode.get_tree_attrs(
-            other, other_attr_fn, other_filter_fn))
+        return key in set(VSSNode.get_tree_attrs(other, other_attr_fn, other_filter_fn))
 
     @staticmethod
     def node_exists(root, node_name) -> bool:
         """Checks if a node with the name provided to this method exists
-            Args:
-                root: root node of tree or root of search if search is applied to subtree
-                node_name: name of the node that is searched for. Full path (excluding root) is required.
+        Args:
+            root: root node of tree or root of search if search is applied to subtree
+            node_name: name of the node that is searched for. Full path (excluding root) is required.
         """
         try:
             r = Resolver()
             r.get(root, node_name)
             return True
         except ChildResolverError:
             return False
@@ -442,26 +549,40 @@
 
         if "description" not in self.source_dict.keys():
             logging.error("Invalid VSS element %s, must have description", self.name)
             sys.exit(-1)
 
         unknown = []
         for aKey in self.source_dict.keys():
-            if aKey not in VSSNode.core_attributes and aKey not in VSSNode.whitelisted_extended_attributes:
+            if (
+                aKey not in VSSNode.core_attributes
+                and aKey not in VSSNode.whitelisted_extended_attributes
+            ):
                 unknown.append(aKey)
 
         unknown_found = False
         if len(unknown) > 0:
-            logging.warning(f"Attribute(s) {', '.join(map(str, unknown))} in element {self.name} not a core "
-                            "or known extended attribute.")
+            logging.warning(
+                f"Attribute(s) {', '.join(map(str, unknown))} in element {self.name} not a core "
+                "or known extended attribute."
+            )
             unknown_found = True
 
         if "default" in self.source_dict.keys():
-            if self.source_dict["type"] not in {"attribute", "property", "sensor", "actuator"}:
-                logging.warning("Invalid VSS element %s, %s cannot use default", self.name, self.source_dict["type"])
+            if self.source_dict["type"] not in {
+                "attribute",
+                "property",
+                "sensor",
+                "actuator",
+            }:
+                logging.warning(
+                    "Invalid VSS element %s, %s cannot use default",
+                    self.name,
+                    self.source_dict["type"],
+                )
                 unknown_found = True
 
         if unknown_found and abort_on_unknown_attribute:
             logging.error("You asked for strict checking. Terminating.")
             sys.exit(-1)
 
     @staticmethod
```

### Comparing `vss-tools-4.1rc0/vspec/utils/__init__.py` & `vss_tools-5.0.0.dev0/vspec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.1rc0/vspec/utils/stringstyle.py` & `vss_tools-5.0.0.dev0/vspec/utils/stringstyle.py`

 * *Files identical despite different names*

### Comparing `vss-tools-4.1rc0/vspec/utils/vss2id_val.py` & `vss_tools-5.0.0.dev0/vspec/utils/vss2id_val.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 #
 # This program and the accompanying materials are made available under the
 # terms of the Mozilla Public License 2.0 which is available at
 # https://www.mozilla.org/en-US/MPL/2.0/
 #
 # SPDX-License-Identifier: MPL-2.0
 
-from anytree import PreOrderIter  # type: ignore
 import argparse
 import logging
 import sys
 from typing import Optional
+
+from anytree import PreOrderIter  # type: ignore
+
 from vspec.model.vsstree import VSSNode
 from vspec.utils.idgen_utils import fnv1_32_wrapper
 
 
 def validate_static_uids(
     signals_dict: dict, validation_tree: VSSNode, config: argparse.Namespace
 ):
@@ -36,27 +38,28 @@
             logging.warning(
                 "[Validation] "
                 f"DESCRIPTION MISMATCH: The description of {k} has changed from "
                 f"\n\t   Validation: '{validation_node.description}' to \n\t   Current "
                 f"vspec: '{v['description']}'"
             )
 
-    def check_semantics(k: str, v: dict) -> Optional[int]:
+    def check_semantics(k: str, v: dict, strict_mode: bool) -> Optional[int]:
         """Checks if the change was a semantic or path change. This can be triggered by
         manually adding a fka (formerly known as) attribute to the vspec. The result
         is that the old hash can be matched such that a node keeps the same UID.
 
         @param k: the current key
         @param v: the current value (dict)
+        @param strict_mode: strict mode means case sensitivity for static UID generation
         @return: boolean if it was a semantic or path change
         """
         if "fka" in v.keys():
             semantic_match: Optional[int] = None
             for fka_val in v["fka"]:
-                old_static_uid = "0x" + fnv1_32_wrapper(fka_val, v)
+                old_static_uid = "0x" + fnv1_32_wrapper(fka_val, v, strict_mode)
                 for i, validation_node in enumerate(validation_tree_nodes):
                     if (
                         old_static_uid
                         == validation_node.extended_attributes["staticUID"]
                     ):
                         logging.warning(
                             f"[Validation] SEMANTIC NAME CHANGE or PATH CHANGE for '{k}', "
@@ -94,23 +97,23 @@
         corresponding logs.
         In the end the remaining nodes correspond to deleted nodes, so we throw a
         `DELETED ATTRIBUTE` warning.
         """
         nonlocal validation_tree_nodes
 
         for key, value in signals_dict.items():
-            matched_uids = [
-                (key, id_validation_tree)
-                for id_validation_tree, other_node in enumerate(validation_tree_nodes)
-                if value["staticUID"] == other_node.extended_attributes["staticUID"]
-            ]
-
+            matched_uids = []
+            for id_validation_tree, other_node in enumerate(validation_tree_nodes):
+                if value["staticUID"] == other_node.extended_attributes["staticUID"]:
+                    if key != other_node.qualified_name():
+                        _ = check_semantics(key, value, config.strict_mode)
+                    matched_uids.append((key, id_validation_tree))
             # if not matched via UID check semantics or path change
             if len(matched_uids) == 0:
-                semantic_match = check_semantics(key, value)
+                semantic_match = check_semantics(key, value, config.strict_mode)
                 if semantic_match is None:
                     key_found: bool = False
                     for i, node in enumerate(validation_tree_nodes):
                         if key == node.qualified_name():
                             key_found = True
                             validation_tree_nodes.pop(i)
                             break
```

### Comparing `vss-tools-4.1rc0/vspec/vssexporters/vss2binary.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2binary.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,23 @@
 
 # Convert vspec tree to binary format
 
 import argparse
 import logging
 import ctypes
 import os.path
+from typing import Optional
 from vspec.model.vsstree import VSSNode, VSSType
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 
 out_file = ""
 _cbinary = None
 
 
-def feature_supported(feature_name: str):
-    """Return true for supported optional arguments/features"""
-    return False
-
-
 def createBinaryCnode(fname, nodename, nodetype, uuid, description, nodedatatype, nodemin, nodemax, unit, allowed,
                       defaultAllowed, validate, children):
     global _cbinary
     _cbinary.createBinaryCnode(fname, nodename, nodetype, uuid, description, nodedatatype, nodemin, nodemax, unit,
                                allowed, defaultAllowed, validate, children)
 
 
@@ -50,18 +48,14 @@
 def intToHexChar(hexInt):
     if (hexInt < 10):
         return chr(hexInt + ord('0'))
     else:
         return chr(hexInt - 10 + ord('A'))
 
 
-def add_arguments(parser: argparse.ArgumentParser):
-    parser.description = "The binary exporter does not support any additional arguments."
-
-
 def export_node(node, generate_uuid, out_file):
     nodename = str(node.name)
     b_nodename = nodename.encode('utf-8')
 
     nodetype = str(node.type.value)
     b_nodetype = nodetype.encode('utf-8')
 
@@ -120,27 +114,34 @@
     createBinaryCnode(b_fname, b_nodename, b_nodetype, b_nodeuuid, b_nodedescription, b_nodedatatype, b_nodemin,
                       b_nodemax, b_nodeunit, b_nodeallowed, b_nodedefault, b_nodevalidate, children)
 
     for child in node.children:
         export_node(child, generate_uuid, out_file)
 
 
-def export(config: argparse.Namespace, root: VSSNode, print_uuid):
-    global _cbinary
-    dllName = "../../binary/binarytool.so"
-    dllAbsPath = os.path.dirname(os.path.abspath(__file__)) + os.path.sep + dllName
-    if not os.path.isfile(dllAbsPath):
-        logging.error("The required library binarytool.so is not available, exiting!")
-        logging.info("You must build the library, "
-                     "see https://github.com/COVESA/vss-tools/blob/master/binary/README.md!")
-        return
-    _cbinary = ctypes.CDLL(dllAbsPath)
-
-    _cbinary.createBinaryCnode.argtypes = (ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p,
-                                           ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p,
-                                           ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p,
-                                           ctypes.c_int)
-
-    logging.info("Generating binary output...")
-    out_file = config.output_file
-    export_node(root, print_uuid, out_file)
-    logging.info("Binary output generated in " + out_file)
+class Vss2Binary(Vss2X):
+
+    def __init__(self, vspec2vss_config: Vspec2VssConfig):
+        vspec2vss_config.type_tree_supported = False
+        vspec2vss_config.no_expand_option_supported = False
+
+    def generate(self, config: argparse.Namespace, root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
+        global _cbinary
+        dllName = "../../binary/binarytool.so"
+        dllAbsPath = os.path.dirname(os.path.abspath(__file__)) + os.path.sep + dllName
+        if not os.path.isfile(dllAbsPath):
+            logging.error("The required library binarytool.so is not available, exiting!")
+            logging.info("You must build the library, "
+                         "see https://github.com/COVESA/vss-tools/blob/master/binary/README.md!")
+            return
+        _cbinary = ctypes.CDLL(dllAbsPath)
+
+        _cbinary.createBinaryCnode.argtypes = (ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p,
+                                               ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p,
+                                               ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p,
+                                               ctypes.c_int)
+
+        logging.info("Generating binary output...")
+        out_file = config.output_file
+        export_node(root, vspec2vss_config.generate_uuid, out_file)
+        logging.info("Binary output generated in " + out_file)
```

### Comparing `vss-tools-4.1rc0/vspec/vssexporters/vss2csv.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2csv.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,28 +11,20 @@
 # Convert vspec tree to CSV
 
 
 import argparse
 import logging
 from vspec.model.vsstree import VSSNode
 from anytree import PreOrderIter  # type: ignore[import]
-from vspec.loggingconfig import initLogging
 from typing import AnyStr
+from typing import Optional
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 
 
-def feature_supported(feature_name: str):
-    """Return true for supported arguments/features"""
-    if feature_name in ['no_expand']:
-        return True
-    return False
-
-
-def add_arguments(parser: argparse.ArgumentParser):
-    parser.description = "The csv exporter does not support any additional arguments."
-
 # Write the header line
 
 
 def print_csv_header(file, uuid, entry_type: AnyStr, include_instance_column: bool):
     arg_list = [entry_type, "Type", "DataType", "Deprecated", "Unit",
                 "Min", "Max", "Desc", "Comment", "Allowed", "Default"]
     if uuid:
@@ -64,27 +56,27 @@
         if uuid:
             arg_list.append(tree_node.uuid)
         if include_instance_column and tree_node.instances is not None:
             arg_list.append(tree_node.instances)
         file.write(format_csv_line(arg_list))
 
 
-def export(config: argparse.Namespace, signal_root: VSSNode, print_uuid, data_type_root: VSSNode):
-    logging.info("Generating CSV output...")
-
-    # generic entry should be written when both data types and signals are being written to the same file
-    generic_entry = data_type_root is not None and config.types_output_file is None
-    with open(config.output_file, 'w') as f:
-        signal_entry_type = "Node" if generic_entry else "Signal"
-        print_csv_header(f, print_uuid, signal_entry_type, config.no_expand)
-        print_csv_content(f, signal_root, print_uuid, config.no_expand)
-        if data_type_root is not None and generic_entry is True:
-            print_csv_content(f, data_type_root, print_uuid, config.no_expand)
-
-    if data_type_root is not None and generic_entry is False:
-        with open(config.types_output_file, 'w') as f:
-            print_csv_header(f, print_uuid, "Node", config.no_expand)
-            print_csv_content(f, data_type_root, print_uuid, config.no_expand)
-
+class Vss2Csv(Vss2X):
 
-if __name__ == "__main__":
-    initLogging()
+    def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
+        logging.info("Generating CSV output...")
+
+        # generic entry should be written when both data types and signals are being written to the same file
+        generic_entry = data_type_root is not None and config.types_output_file is None
+        include_instance_column = not vspec2vss_config.expand_model
+        with open(config.output_file, 'w') as f:
+            signal_entry_type = "Node" if generic_entry else "Signal"
+            print_csv_header(f, vspec2vss_config.generate_uuid, signal_entry_type, include_instance_column)
+            print_csv_content(f, signal_root, vspec2vss_config.generate_uuid, include_instance_column)
+            if data_type_root is not None and generic_entry is True:
+                print_csv_content(f, data_type_root, vspec2vss_config.generate_uuid, include_instance_column)
+
+        if data_type_root is not None and generic_entry is False:
+            with open(config.types_output_file, 'w') as f:
+                print_csv_header(f, vspec2vss_config.generate_uuid, "Node", include_instance_column)
+                print_csv_content(f, data_type_root, vspec2vss_config.generate_uuid, include_instance_column)
```

### Comparing `vss-tools-4.1rc0/vspec/vssexporters/vss2ddsidl.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2ddsidl.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,29 +11,19 @@
 #
 # Convert vspec files to DDS-IDL
 #
 
 import argparse
 import keyword
 import logging
+from typing import Optional
 
-from vspec.loggingconfig import initLogging
 from vspec.model.vsstree import VSSNode, VSSType
-
-
-def feature_supported(feature_name: str):
-    """Return true for supported optional arguments/features"""
-    return False
-
-
-def add_arguments(parser: argparse.ArgumentParser):
-    parser.description = "The DDS-IDL exporter"
-    parser.add_argument('--all-idl-features', action='store_true',
-                        help='Generate all features based on DDS IDL 4.2 specification')
-
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 
 c_keywords = [
     "auto", "break", "case", "char", "const", "continue", "default", "do", "double", "else", "enum", "extern", "float",
     "for", "goto", "if", "int", "long", "register", "return", "short", "signed", "sizeof", "static", "struct", "switch",
     "typedef", "union", "unsigned", "void", "volatile", "while"
     ]
 
@@ -274,20 +264,32 @@
        -> DDS IDL equivalent string buffer and to serialize it acccordingly into a file
     """
     export_node(root, generate_uuids, generate_all_idl_features)
     file.write('\n'.join(idlFileBuffer))
     logging.info("IDL file generated at location : " + file.name)
 
 
-def export(config: argparse.Namespace, signal_root: VSSNode, print_uuid, data_type_root: VSSNode):
-    logging.info("Generating DDS-IDL output...")
+class Vss2DdsIdl(Vss2X):
 
-    if data_type_root is not None:
-        exporter = StructExporter()
-        with open(config.output_file, 'w') as idl_out:
-            idl_out.write(exporter.export(data_type_root))
+    def __init__(self, vspec2vss_config: Vspec2VssConfig):
+        vspec2vss_config.no_expand_option_supported = False
+        vspec2vss_config.separate_output_type_file_supported = False
+
+    def add_arguments(self, parser: argparse.ArgumentParser):
+        parser.description = "The DDS-IDL exporter"
+        parser.add_argument('--all-idl-features', action='store_true',
+                            help='Generate all features based on DDS IDL 4.2 specification')
+
+    def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
+        logging.info("Generating DDS-IDL output...")
+
+        if data_type_root is not None:
+            exporter = StructExporter()
+            with open(config.output_file, 'w') as idl_out:
+                idl_out.write(exporter.export(data_type_root))
 
-    with open(config.output_file, 'a' if data_type_root is not None else 'w') as idl_out:
-        export_idl(idl_out, signal_root, print_uuid, config.all_idl_features)
+        with open(config.output_file, 'a' if data_type_root is not None else 'w') as idl_out:
+            export_idl(idl_out, signal_root, vspec2vss_config.generate_uuid, config.all_idl_features)
 
-    if __name__ == "__main__":
-        initLogging()
+    def __del__(self):
+        idlFileBuffer.clear()
```

### Comparing `vss-tools-4.1rc0/vspec/vssexporters/vss2franca.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2franca.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,27 +8,21 @@
 #
 # SPDX-License-Identifier: MPL-2.0
 
 # Convert vspec tree to franca
 
 
 import argparse
+from typing import Optional
 from vspec.model.vsstree import VSSNode
 from anytree import PreOrderIter  # type: ignore[import]
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 
 
-def feature_supported(feature_name: str):
-    """Return true for supported optional arguments/features"""
-    return False
-
-
-def add_arguments(parser: argparse.ArgumentParser):
-    # no additional output for Franca at this moment
-    parser.add_argument('-v', metavar='version', help=" Add version information to franca file.")
-
 # Write the header line
 
 
 def print_franca_header(file, version="unknown"):
     file.write(f"""
 // Copyright (C) 2022, COVESA
 //
@@ -78,14 +72,27 @@
             if tree_node.allowed:
                 output += f",\n\tallowed: {tree_node.allowed}"
 
             output += "\n}"
     file.write(f"{output}")
 
 
-def export(config: argparse.Namespace, root: VSSNode, print_uuid):
-    print("Generating Franca output...")
-    outfile = open(config.output_file, 'w')
-    print_franca_header(outfile, config.v)
-    print_franca_content(outfile, root, print_uuid)
-    outfile.write("\n]")
-    outfile.close()
+class Vss2Franca(Vss2X):
+
+    def __init__(self, vspec2vss_config: Vspec2VssConfig):
+        vspec2vss_config.no_expand_option_supported = False
+        vspec2vss_config.type_tree_supported = False
+
+    def add_arguments(self, parser: argparse.ArgumentParser):
+        # Renamed from -v to --franca-vss-version to avoid conflict when using
+        # -vt (Otherwise -vt would be interpreted as "-v t")
+        parser.add_argument('--franca-vss-version', metavar='franca_vss_version',
+                            help=" Add version information to franca file.")
+
+    def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
+        print("Generating Franca output...")
+        outfile = open(config.output_file, 'w')
+        print_franca_header(outfile, config.franca_vss_version)
+        print_franca_content(outfile, signal_root, vspec2vss_config.generate_uuid)
+        outfile.write("\n]")
+        outfile.close()
```

### Comparing `vss-tools-4.1rc0/vspec/vssexporters/vss2graphql.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2graphql.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 import argparse
 from vspec.model.vsstree import VSSNode
 from vspec.utils.stringstyle import camel_back
 from vspec.model.constants import VSSDataType
 from vspec import VSpecError
 from typing import Dict
+from typing import Optional
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 
 from graphql import (
     GraphQLSchema,
     GraphQLObjectType,
     GraphQLField,
     GraphQLArgument,
     GraphQLNonNull,
@@ -53,27 +56,14 @@
     VSSDataType.BOOLEAN: GraphQLBoolean,
     VSSDataType.BOOLEAN_ARRAY: GraphQLList(GraphQLBoolean),
     VSSDataType.STRING: GraphQLString,
     VSSDataType.STRING_ARRAY: GraphQLList(GraphQLString),
 }
 
 
-def feature_supported(feature_name: str):
-    """Return true for supported optional arguments/features"""
-    return False
-
-
-def add_arguments(parser: argparse.ArgumentParser):
-    # no additional output for graphql at this moment
-    parser.description = "The graphql exporter never generates uuid, i.e. the --uuid option has no effect."
-    parser.add_argument('--gqlfield', action='append', nargs=2,
-                        help=" Add additional fields to the nodes in the graphql schema. "
-                             "use: <field_name> <description>")
-
-
 def get_schema_from_tree(root_node: VSSNode, additional_leaf_fields: list) -> str:
     """Takes a VSSNode and additional fields for the leafs. Returns a graphql schema as string."""
     args = dict(
         id=GraphQLArgument(
             GraphQLNonNull(GraphQLString),
             description="VIN of the vehicle that you want to request data for.",
         ),
@@ -128,13 +118,26 @@
     return GraphQLField(
         type,
         deprecation_reason=node.deprecation or None,
         description=f"{description_prefix}{node.description}",
     )
 
 
-def export(config: argparse.Namespace, root: VSSNode, print_uuid):
-    print("Generating graphql output...")
-    outfile = open(config.output_file, 'w')
-    outfile.write(get_schema_from_tree(root, config.gqlfield))
-    outfile.write("\n")
-    outfile.close()
+class Vss2Graphql(Vss2X):
+
+    def __init__(self, vspec2vss_config: Vspec2VssConfig):
+        vspec2vss_config.no_expand_option_supported = False
+        vspec2vss_config.type_tree_supported = False
+        vspec2vss_config.uuid_supported = False
+
+    def add_arguments(self, parser: argparse.ArgumentParser):
+        parser.add_argument('--gqlfield', action='append', nargs=2,
+                            help=" Add additional fields to the nodes in the graphql schema. "
+                                 "use: <field_name> <description>")
+
+    def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
+        print("Generating graphql output...")
+        outfile = open(config.output_file, 'w')
+        outfile.write(get_schema_from_tree(signal_root, config.gqlfield))
+        outfile.write("\n")
+        outfile.close()
```

### Comparing `vss-tools-4.1rc0/vspec/vssexporters/vss2id.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2id.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,75 +10,69 @@
 #
 # Generate IDs of 4bytes size, 3 bytes incremental value + 1 byte for layer id.
 
 import argparse
 import logging
 import os
 import sys
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Optional
+
+import yaml
+
 from vspec import load_tree
 from vspec.model.constants import VSSTreeType
-from vspec.loggingconfig import initLogging
 from vspec.model.vsstree import VSSNode
 from vspec.utils import vss2id_val
-from vspec.utils.idgen_utils import (
-    get_node_identifier_bytes,
-    fnv1_32_hash,
-    get_all_keys_values,
-)
-import yaml
+from vspec.utils.idgen_utils import (fnv1_32_hash, get_all_keys_values,
+                                     get_node_identifier_bytes)
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 
 
-def add_arguments(parser: argparse.ArgumentParser) -> None:
-    """Adds command line arguments to a pre-existing argument parser
-
-    @param parser: the pre-existing argument parser
-    """
-    parser.add_argument(
-        "--validate-static-uid", type=str, default="", help="Path to validation file."
-    )
-    parser.add_argument(
-        "--only-validate-no-export",
-        action="store_true",
-        default=False,
-        help="For pytests and pipelines you can skip the export of the vspec file.",
-    )
+def generate_split_id(
+    node: VSSNode, id_counter: int, strict_mode: bool
+) -> Tuple[str, int]:
 
-
-def generate_split_id(node: VSSNode, id_counter: int) -> Tuple[str, int]:
     """Generates static UIDs using 4-byte FNV-1 hash.
 
     @param node: VSSNode that we want to generate a static UID for
     @param id_counter: consecutive numbers counter for amount of nodes
+    @param strict_mode: strict mode means case sensitivity for static UID generation
     @return: tuple of hashed string and id counter
     """
 
+    if hasattr(node, "fka") and node.fka:
+        name = node.fka[0] if isinstance(node.fka, list) else node.fka
+    else:
+        name = node.qualified_name()
     identifier = get_node_identifier_bytes(
-        node.qualified_name(),
+        name,
         node.data_type_str,
         node.type.value,
         node.get_unit(),
         node.allowed,
         node.min,
         node.max,
+        strict_mode,
     )
     hashed_str = format(fnv1_32_hash(identifier), "08X")
 
     return hashed_str, id_counter + 1
 
 
-def export_node(yaml_dict, node, id_counter) -> Tuple[int, int]:
+def export_node(yaml_dict, node, id_counter, strict_mode: bool) -> Tuple[int, int]:
     """Recursive function to export the full tree to a dict
 
     @param yaml_dict: the to be exported dict
     @param node: parent node of the tree
     @param id_counter: counter for amount of ids
+    @param strict_mode: strict mode means case sensitivity for static UID generation
     @return: id_counter, id_counter
     """
-    node_id, id_counter = generate_split_id(node, id_counter)
+    node_id, id_counter = generate_split_id(node, id_counter, strict_mode)
 
     # check for hash duplicates
     for key, value in get_all_keys_values(yaml_dict):
         if not isinstance(value, dict) and key == "staticUID":
             if node_id == value[2:]:
                 logging.fatal(
                     f"There is a small chance that the result of FNV-1 "
@@ -110,51 +104,69 @@
     elif "fka" in node.extended_attributes.keys():
         yaml_dict[node_path]["fka"] = node.extended_attributes["fka"]
 
     if node.deprecation:
         yaml_dict[node_path]["deprecation"] = node.deprecation
 
     for child in node.children:
-        id_counter, id_counter = export_node(
-            yaml_dict,
-            child,
-            id_counter,
-        )
+        id_counter, id_counter = export_node(yaml_dict, child, id_counter, strict_mode)
 
     return id_counter, id_counter
 
 
-def export(config: argparse.Namespace, signal_root: VSSNode, print_uuid):
-    """Main export function used to generate the output id vspec.
+class Vss2Id(Vss2X):
 
-    @param config: Command line arguments it was run with
-    @param signal_root: root of the signal tree
-    @param print_uuid: Not used here but needed by main script
-    """
-    logging.info("Generating YAML output...")
+    def add_arguments(self, parser: argparse.ArgumentParser) -> None:
+        """Adds command line arguments to a pre-existing argument parser
 
-    id_counter: int = 0
-    signals_yaml_dict: Dict[str, str] = {}  # Use str for ID values
-    id_counter, _ = export_node(signals_yaml_dict, signal_root, id_counter)
-
-    if config.validate_static_uid:
-        logging.info(
-            f"Now validating nodes, static UIDs, types, units and description with "
-            f"file '{config.validate_static_uid}'"
+        @param parser: the pre-existing argument parser
+        """
+        parser.add_argument(
+            "--validate-static-uid", type=str, default="", help="Path to validation file."
         )
-        if os.path.isabs(config.validate_static_uid):
-            other_path = config.validate_static_uid
-        else:
-            other_path = os.path.join(os.getcwd(), config.validate_static_uid)
-
-        validation_tree = load_tree(
-            other_path, ["."], tree_type=VSSTreeType.SIGNAL_TREE
+        parser.add_argument(
+            "--only-validate-no-export",
+            action="store_true",
+            default=False,
+            help="For pytests and pipelines you can skip the export of the vspec file.",
         )
-        vss2id_val.validate_static_uids(signals_yaml_dict, validation_tree, config)
+        parser.add_argument(
+            "--strict-mode",
+            action="store_true",
+            help="Strict mode means that the generation of static UIDs is case-sensitive.",
+        )
+
+    def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
 
-    if not config.only_validate_no_export:
-        with open(config.output_file, "w") as f:
-            yaml.dump(signals_yaml_dict, f)
+        """Main export function used to generate the output id vspec.
 
+        @param config: Command line arguments it was run with
+        @param signal_root: root of the signal tree
+        @param print_uuid: Not used here but needed by main script
+        """
+        logging.info("Generating YAML output...")
+
+        id_counter: int = 0
+        signals_yaml_dict: Dict[str, str] = {}  # Use str for ID values
+        id_counter, _ = export_node(
+            signals_yaml_dict, signal_root, id_counter, config.strict_mode
+        )
 
-if __name__ == "__main__":
-    initLogging()
+        if config.validate_static_uid:
+            logging.info(
+                f"Now validating nodes, static UIDs, types, units and description with "
+                f"file '{config.validate_static_uid}'"
+            )
+            if os.path.isabs(config.validate_static_uid):
+                other_path = config.validate_static_uid
+            else:
+                other_path = os.path.join(os.getcwd(), config.validate_static_uid)
+
+            validation_tree = load_tree(
+                other_path, ["."], tree_type=VSSTreeType.SIGNAL_TREE
+            )
+            vss2id_val.validate_static_uids(signals_yaml_dict, validation_tree, config)
+
+        if not config.only_validate_no_export:
+            with open(config.output_file, "w") as f:
+                yaml.dump(signals_yaml_dict, f)
```

### Comparing `vss-tools-4.1rc0/vspec/vssexporters/vss2json.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2json.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,17 @@
 # Convert vspec tree to JSON
 
 from vspec.model.vsstree import VSSNode
 import argparse
 import json
 import logging
 from typing import Dict, Any
-from vspec.loggingconfig import initLogging
-
-
-def feature_supported(feature_name: str):
-    """Return true for supported arguments/features"""
-    if feature_name in ['no_expand']:
-        return True
-    return False
-
-
-def add_arguments(parser: argparse.ArgumentParser):
-    parser.add_argument('--json-all-extended-attributes', action='store_true',
-                        help="Generate all extended attributes found in the model "
-                             "(default is generating only those given by the -e/--extended-attributes parameter).")
-    parser.add_argument('--json-pretty', action='store_true',
-                        help=" Pretty print JSON output.")
+from typing import Optional
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 
 
 def export_node(json_dict, node, config, print_uuid):
 
     json_dict[node.name] = {}
 
     if node.is_signal() or node.is_property():
@@ -89,35 +76,41 @@
         json_dict[node.name]["children"] = {}
 
     for child in node.children:
         export_node(json_dict[node.name]["children"],
                     child, config, print_uuid)
 
 
-def export(config: argparse.Namespace, signal_root: VSSNode, print_uuid, data_type_root: VSSNode):
-    logging.info("Generating JSON output...")
-    indent = None
-    if config.json_pretty:
-        logging.info("Serializing pretty JSON...")
-        indent = 2
-    else:
-        logging.info("Serializing compact JSON...")
-
-    signals_json_dict: Dict[str, Any] = {}
-    export_node(signals_json_dict, signal_root, config, print_uuid)
-
-    if data_type_root is not None:
-        data_types_json_dict: Dict[str, Any] = {}
-        export_node(data_types_json_dict, data_type_root, config, print_uuid)
-        if config.types_output_file is None:
-            logging.info("Adding custom data types to signal dictionary")
-            signals_json_dict["ComplexDataTypes"] = data_types_json_dict
+class Vss2Json(Vss2X):
+
+    def add_arguments(self, parser: argparse.ArgumentParser) -> None:
+        parser.add_argument('--json-all-extended-attributes', action='store_true',
+                            help="Generate all extended attributes found in the model "
+                                 "(default is generating only those given by the -e/--extended-attributes parameter).")
+        parser.add_argument('--json-pretty', action='store_true',
+                            help=" Pretty print JSON output.")
+
+    def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
+        logging.info("Generating JSON output...")
+        indent = None
+        if config.json_pretty:
+            logging.info("Serializing pretty JSON...")
+            indent = 2
         else:
-            with open(config.types_output_file, 'w') as f:
-                json.dump(data_types_json_dict, f, indent=indent, sort_keys=True)
+            logging.info("Serializing compact JSON...")
 
-    with open(config.output_file, 'w') as f:
-        json.dump(signals_json_dict, f, indent=indent, sort_keys=True)
+        signals_json_dict: Dict[str, Any] = {}
+        export_node(signals_json_dict, signal_root, config, vspec2vss_config.generate_uuid)
 
+        if data_type_root is not None:
+            data_types_json_dict: Dict[str, Any] = {}
+            export_node(data_types_json_dict, data_type_root, config, vspec2vss_config.generate_uuid)
+            if config.types_output_file is None:
+                logging.info("Adding custom data types to signal dictionary")
+                signals_json_dict["ComplexDataTypes"] = data_types_json_dict
+            else:
+                with open(config.types_output_file, 'w') as f:
+                    json.dump(data_types_json_dict, f, indent=indent, sort_keys=True)
 
-if __name__ == "__main__":
-    initLogging()
+        with open(config.output_file, 'w') as f:
+            json.dump(signals_json_dict, f, indent=indent, sort_keys=True)
```

### Comparing `vss-tools-4.1rc0/vspec/vssexporters/vss2jsonschema.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2jsonschema.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 #
 # Convert vspec tree compatible JSON schema
 
 import argparse
 import json
 import logging
 from typing import Dict, Any
+from typing import Optional
 from vspec.model.vsstree import VSSNode
-from vspec.loggingconfig import initLogging
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 
 type_map = {
     "int8": "integer",
     "uint8": "integer",
     "int16": "integer",
     "uint16": "integer",
     "int32": "integer",
@@ -41,27 +43,14 @@
     "boolean[]": "array",
     "float[]": "array",
     "double[]": "array",
     "string[]": "array"
 }
 
 
-def add_arguments(parser: argparse.ArgumentParser):
-    """Check for input arguments."""
-    parser.add_argument('--jsonschema-all-extended-attributes', action='store_true',
-                        help="Generate all extended attributes found in the model."
-                        "Should not be used with strict mode JSON Schema validators.")
-    parser.add_argument("--jsonschema-disallow-additional-properties", action='store_true',
-                        help="Do not allow properties not defined in VSS tree")
-    parser.add_argument("--jsonschema-require-all-properties", action='store_true',
-                        help="Require all elements defined in VSS tree for a valid object")
-    parser.add_argument('--jsonschema-pretty', action='store_true',
-                        help=" Pretty print JSON Schema output.")
-
-
 def export_node(json_dict, node, config, print_uuid):
     """Preparing nodes for JSON schema output."""
     # keyword with X- sign are left for extensions and they are not part of official JSON schema
     json_dict[node.name] = {
         "description": node.description,
     }
 
@@ -118,42 +107,53 @@
         json_dict[node.name]["properties"] = {}
         if config.jsonschema_require_all_properties:
             json_dict[node.name]["required"] = [child.name for child in node.children]
         for child in node.children:
             export_node(json_dict[node.name]["properties"], child, config, print_uuid)
 
 
-def export(config: argparse.Namespace, signal_root: VSSNode, print_uuid, data_type_root: VSSNode):
-    """Export function for generating JSON schema file."""
-    logging.info("Generating JSON schema...")
-    indent = None
-    if config.jsonschema_pretty:
-        logging.info("Serializing pretty JSON schema...")
-        indent = 2
-
-    signals_json_schema: Dict[str, Any] = {}
-    export_node(signals_json_schema, signal_root, config, print_uuid)
-
-    # Add data types to the schema
-    if data_type_root is not None:
-        data_types_json_schema: Dict[str, Any] = {}
-        export_node(data_types_json_schema, data_type_root, config, print_uuid)
-        if config.jsonschema_all_extended_attributes:
-            signals_json_schema["x-ComplexDataTypes"] = data_types_json_schema
-
-    # VSS models only have one root, so there should only be one
-    # key in the dict
-    assert (len(signals_json_schema.keys()) == 1)
-    top_node_name = list(signals_json_schema.keys())[0]
-    signals_json_schema = signals_json_schema.pop(top_node_name)
-
-    json_schema = {
-        "$schema": "https://json-schema.org/draft/2020-12/schema",
-        "title": top_node_name,
-        "type": "object",
-        **signals_json_schema}
-    with open(config.output_file, 'w', encoding="utf-8") as output_file:
-        json.dump(json_schema, output_file, indent=indent, sort_keys=False)
-
+class Vss2JsonSchema(Vss2X):
 
-if __name__ == "__main__":
-    initLogging()
+    def add_arguments(self, parser: argparse.ArgumentParser):
+        """Check for input arguments."""
+        parser.add_argument('--jsonschema-all-extended-attributes', action='store_true',
+                            help="Generate all extended attributes found in the model."
+                            "Should not be used with strict mode JSON Schema validators.")
+        parser.add_argument("--jsonschema-disallow-additional-properties", action='store_true',
+                            help="Do not allow properties not defined in VSS tree")
+        parser.add_argument("--jsonschema-require-all-properties", action='store_true',
+                            help="Require all elements defined in VSS tree for a valid object")
+        parser.add_argument('--jsonschema-pretty', action='store_true',
+                            help=" Pretty print JSON Schema output.")
+
+    def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
+        """Export function for generating JSON schema file."""
+        logging.info("Generating JSON schema...")
+        indent = None
+        if config.jsonschema_pretty:
+            logging.info("Serializing pretty JSON schema...")
+            indent = 2
+
+        signals_json_schema: Dict[str, Any] = {}
+        export_node(signals_json_schema, signal_root, config, vspec2vss_config.generate_uuid)
+
+        # Add data types to the schema
+        if data_type_root is not None:
+            data_types_json_schema: Dict[str, Any] = {}
+            export_node(data_types_json_schema, data_type_root, config, vspec2vss_config.generate_uuid)
+            if config.jsonschema_all_extended_attributes:
+                signals_json_schema["x-ComplexDataTypes"] = data_types_json_schema
+
+        # VSS models only have one root, so there should only be one
+        # key in the dict
+        assert (len(signals_json_schema.keys()) == 1)
+        top_node_name = list(signals_json_schema.keys())[0]
+        signals_json_schema = signals_json_schema.pop(top_node_name)
+
+        json_schema = {
+            "$schema": "https://json-schema.org/draft/2020-12/schema",
+            "title": top_node_name,
+            "type": "object",
+            **signals_json_schema}
+        with open(config.output_file, 'w', encoding="utf-8") as output_file:
+            json.dump(json_schema, output_file, indent=indent, sort_keys=False)
```

### Comparing `vss-tools-4.1rc0/vspec/vssexporters/vss2protobuf.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2protobuf.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 
 import argparse
 import logging
 import os
 import sys
 from pathlib import Path
 from typing import Set
+from typing import Optional
 
 from anytree import PreOrderIter  # type: ignore[import]
-from vspec.loggingconfig import initLogging
 from vspec.model.vsstree import VSSNode
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 
 # Add path to main py vspec  parser
 myDir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(myDir, ".."))
 
 PATH_DELIMITER = "."
 DIR_DELIMITER = "/"
@@ -34,23 +36,14 @@
     "uint8": "uint32",
     "int8": "int32",
     "int16": "int32",
     "boolean": "bool"
 }
 
 
-def feature_supported(feature_name: str):
-    """Return true for supported optional arguments/features"""
-    return False
-
-
-def add_arguments(parser: argparse.ArgumentParser):
-    parser.description = "The protobuf exporter does not support any additional arguments."
-
-
 class ProtoExporter(object):
     def __init__(self, out_dir: Path):
         self.out_files: Set[Path] = set()
         self.out_dir = out_dir
 
     def setup_file(self, fp: Path, package_name: str):
         with open(fp, 'w') as proto_file:
@@ -144,25 +137,35 @@
         if not (node.is_branch() or node.is_struct()):
             dt_val = node.get_datatype()
             data_type = mapped.get(dt_val.strip("[]"), dt_val.strip("[]"))
             data_type = ("repeated " if dt_val.endswith("[]") else "") + data_type
         proto_file.write(f"  {data_type} {node.name} = {i};" + "\n")
 
 
-def export(config: argparse.Namespace, signal_root: VSSNode, print_uuid, data_type_root: VSSNode):
-    logging.info("Generating protobuf output...")
-    if data_type_root is not None:
-        if config.types_output_file is not None:
-            fp = Path(config.types_output_file)
-            exporter_path = Path(os.path.dirname(fp))
-        else:
-            exporter_path = Path(Path.cwd())
-        logging.debug(f"Will use {exporter_path} for type exports")
-        exporter = ProtoExporter(exporter_path)
-        exporter.traverse_data_type_tree(data_type_root)
-
-    with open(config.output_file, 'w') as f:
-        traverse_signal_tree(signal_root, f)
+class Vss2Protobuf(Vss2X):
 
+    def __init__(self, vspec2vss_config: Vspec2VssConfig):
+        vspec2vss_config.no_expand_option_supported = False
+        vspec2vss_config.uuid_supported = False
+
+    def add_arguments(self, parser: argparse.ArgumentParser) -> None:
+        parser.add_argument('--json-all-extended-attributes', action='store_true',
+                            help="Generate all extended attributes found in the model "
+                                 "(default is generating only those given by the -e/--extended-attributes parameter).")
+        parser.add_argument('--json-pretty', action='store_true',
+                            help=" Pretty print JSON output.")
+
+    def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
+        logging.info("Generating protobuf output...")
+        if data_type_root is not None:
+            if config.types_output_file is not None:
+                fp = Path(config.types_output_file)
+                exporter_path = Path(os.path.dirname(fp))
+            else:
+                exporter_path = Path(Path.cwd())
+            logging.debug(f"Will use {exporter_path} for type exports")
+            exporter = ProtoExporter(exporter_path)
+            exporter.traverse_data_type_tree(data_type_root)
 
-if __name__ == "__main__":
-    initLogging()
+        with open(config.output_file, 'w') as f:
+            traverse_signal_tree(signal_root, f)
```

### Comparing `vss-tools-4.1rc0/vspec/vssexporters/vss2yaml.py` & `vss_tools-5.0.0.dev0/vspec/vssexporters/vss2yaml.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,30 +13,18 @@
 #
 
 
 import argparse
 from vspec.model.vsstree import VSSNode
 import yaml
 import logging
-from vspec.loggingconfig import initLogging
 from typing import Dict, Any
-
-
-def feature_supported(feature_name: str):
-    """Return true for supported arguments/features"""
-    if feature_name in ['no_expand']:
-        return True
-    return False
-
-
-def add_arguments(parser: argparse.ArgumentParser):
-    parser.add_argument('--yaml-all-extended-attributes', action='store_true',
-                        help=("Generate all extended attributes found in the model "
-                              "(default is generating only those given by the "
-                              "-e/--extended-attributes parameter)."))
+from typing import Optional
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 
 
 def export_node(yaml_dict, node, config, print_uuid):
 
     node_path = node.qualified_name()
 
     yaml_dict[node_path] = {}
@@ -102,27 +90,33 @@
 
     def write_line_break(self, data=None):
         super().write_line_break(data)
         if len(self.indents) == 1:
             super().write_line_break()
 
 
-def export(config: argparse.Namespace, signal_root: VSSNode, print_uuid, data_type_root: VSSNode):
-    logging.info("Generating YAML output...")
-
-    signals_yaml_dict: Dict[str, Any] = {}
-    export_node(signals_yaml_dict, signal_root, config, print_uuid)
-
-    if data_type_root is not None:
-        data_types_yaml_dict: Dict[str, Any] = {}
-        export_node(data_types_yaml_dict, data_type_root, config, print_uuid)
-        if config.types_output_file is None:
-            logging.info("Adding custom data types to signal dictionary")
-            signals_yaml_dict["ComplexDataTypes"] = data_types_yaml_dict
-        else:
-            export_yaml(config.types_output_file, data_types_yaml_dict)
-
-    export_yaml(config.output_file, signals_yaml_dict)
+class Vss2Yaml(Vss2X):
 
+    def add_arguments(self, parser: argparse.ArgumentParser) -> None:
+        parser.add_argument('--yaml-all-extended-attributes', action='store_true',
+                            help=("Generate all extended attributes found in the model "
+                                  "(default is generating only those given by the "
+                                  "-e/--extended-attributes parameter)."))
+
+    def generate(self, config: argparse.Namespace, signal_root: VSSNode, vspec2vss_config: Vspec2VssConfig,
+                 data_type_root: Optional[VSSNode] = None) -> None:
+
+        logging.info("Generating YAML output...")
+
+        signals_yaml_dict: Dict[str, Any] = {}
+        export_node(signals_yaml_dict, signal_root, config, vspec2vss_config.generate_uuid)
+
+        if data_type_root is not None:
+            data_types_yaml_dict: Dict[str, Any] = {}
+            export_node(data_types_yaml_dict, data_type_root, config, vspec2vss_config.generate_uuid)
+            if config.types_output_file is None:
+                logging.info("Adding custom data types to signal dictionary")
+                signals_yaml_dict["ComplexDataTypes"] = data_types_yaml_dict
+            else:
+                export_yaml(config.types_output_file, data_types_yaml_dict)
 
-if __name__ == "__main__":
-    initLogging()
+        export_yaml(config.output_file, signals_yaml_dict)
```

### Comparing `vss-tools-4.1rc0/vspec2x.py` & `vss_tools-5.0.0.dev0/vspec/vspec2x.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,247 +1,191 @@
-#!/usr/bin/env python3
+
 
 # Copyright (c) 2016 Contributors to COVESA
 #
 # This program and the accompanying materials are made available under the
 # terms of the Mozilla Public License 2.0 which is available at
 # https://www.mozilla.org/en-US/MPL/2.0/
 #
 # SPDX-License-Identifier: MPL-2.0
 
 #
 # Convert vspec files to various other formats
 #
 
-from enum import Enum
 from vspec.model.vsstree import VSSNode
 from vspec.model.constants import VSSTreeType
 from vspec.loggingconfig import initLogging
+from vspec.vss2x import Vss2X
+from vspec.vspec2vss_config import Vspec2VssConfig
 import argparse
 import logging
 import sys
 import vspec
 
-
-from vspec.vssexporters import vss2json, vss2csv, vss2yaml, \
-    vss2binary, vss2franca, vss2ddsidl, vss2graphql, vss2protobuf, vss2jsonschema, vss2id
-
-SUPPORTED_STRUCT_EXPORT_FORMATS = set(["json", "yaml", "csv", "protobuf", "jsonschema", "idl"])
+import pkg_resources  # part of setuptools
+VERSION = pkg_resources.require("vss-tools")[0].version
 
 
-class Exporter(Enum):
+class Vspec2X():
     """
-    You can add new exporters here. Put the code in vssexporters and add it here
-    See one of the existing exporters for an example.
-    Mandatory functions are
-    def add_arguments(parser: argparse.ArgumentParser)
-    def export(config: argparse.Namespace, root: VSSNode):
+    Framework for translating from *.vspec files to first an internal VSS model,
+    and then to something else called X.
+    Users must provide a Vss2X generator that can generate X if they get a VSS model as input.
     """
-    json = vss2json
-    csv = vss2csv
-    yaml = vss2yaml
-    binary = vss2binary
-    franca = vss2franca
-    idl = vss2ddsidl
-    graphql = vss2graphql
-    protobuf = vss2protobuf
+    def __init__(self, generator: Vss2X, vspec2vss_config: Vspec2VssConfig):
 
-    jsonschema = vss2jsonschema
-    idgen = vss2id
+        self.generator = generator
+        self.vspec2vss_config = vspec2vss_config
 
-    def __str__(self):
-        return self.name
-
-    @staticmethod
-    def from_string(s):
-        try:
-            return Exporter[s]
-        except KeyError:
-            raise ValueError()
-
-
-def main(arguments):
-    parser = argparse.ArgumentParser(description="Convert vspec to other formats.")
-
-    initLogging()
-
-    parser.add_argument('-I', '--include-dir', action='append', metavar='dir', type=str, default=[],
-                        help='Add include directory to search for included vspec files.')
-    parser.add_argument('-e', '--extended-attributes', type=str, default="",
-                        help='Whitelisted extended attributes as comma separated list. '
-                             'Note, that not all exporters will support (all) extended attributes.')
-    parser.add_argument('-s', '--strict', action='store_true',
-                        help='Use strict checking: Terminate when anything not covered or not recommended '
-                             'by VSS language or extensions is found.')
-    parser.add_argument('--abort-on-unknown-attribute', action='store_true',
-                        help=" Terminate when an unknown attribute is found.")
-    parser.add_argument('--abort-on-name-style', action='store_true',
-                        help=" Terminate naming style not follows recommendations.")
-    parser.add_argument('--format', metavar='format', type=Exporter.from_string, choices=list(Exporter),
-                        help='Output format, choose one from ' +
-                             str(Exporter._member_names_) +  # pylint: disable=no-member
-                             ". If omitted we try to guess form output_file suffix.")
-    parser.add_argument('--uuid', action='store_true',
-                        help='Include uuid in generated files.')
-    parser.add_argument('--no-expand', action='store_true',
-                        help='Do not expand tree.')
-    parser.add_argument('--no-uuid', action='store_true',
-                        help='Exclude uuid in generated files.  This is currently the default behavior. ' +
-                             ' This argument is deprecated and will be removed in VSS 5.0')
-    parser.add_argument('-o', '--overlays', action='append', metavar='overlays', type=str, default=[],
-                        help='Add overlay that will be layered on top of the VSS file in the order they appear.')
-    parser.add_argument('-u', '--unit-file', action='append', metavar='unit_file', type=str, default=[],
-                        help='Unit file to be used for generation. Argument -u may be used multiple times.')
-    parser.add_argument('-q', '--quantity-file', action='append', metavar='quantity_file', type=str, default=[],
-                        help='Quantity file to be used for generation. Argument -uqmay be used multiple times.')
-    parser.add_argument('vspec_file', metavar='<vspec_file>',
-                        help='The vehicle specification file to convert.')
-    parser.add_argument('output_file', metavar='<output_file>',
-                        help='The file to write output to.')
-
-    type_group = parser.add_argument_group(
-        'VSS Data Type Tree arguments',
-        'Arguments related to struct/type support')
-    type_group.add_argument('-vt', '--vspec-types-file', action='append', metavar='vspec_types_file', type=str,
-                            default=[],
-                            help='Data types file in vspec format.')
-    type_group.add_argument('-ot', '--types-output-file', metavar='<types_output_file>',
-                            help='Output file for writing data types from vspec file. ' +
-                                 'If not specified, a single file is used where applicable. ' +
-                                 'In case of JSON and YAML, the data is exported under a ' +
-                                 'special key - "ComplexDataTypes"')
-
-    for entry in Exporter:
-        entry.value.add_arguments(parser.add_argument_group(
-            f"{entry.name.upper()} arguments", ""))
-
-    args = parser.parse_args(arguments)
-
-    # Figure out output format
-    if args.format is not None:  # User has given format parameter
-        logging.info("Output to " + str(args.format.name) + " format")
-    else:  # Else try to figure from output file suffix
-        try:
-            suffix = args.output_file[args.output_file.rindex(".") + 1:]
-        except BaseException:
-            logging.error(
-                "Can not determine output format. Try setting --format parameter")
-            sys.exit(-1)
-        try:
-            args.format = Exporter.from_string(suffix)
-        except BaseException:
-            logging.error(
-                "Can not determine output format. Try setting --format parameter")
-            sys.exit(-1)
-
-        logging.info("Output to " + str(args.format.name) + " format")
-
-    include_dirs = ["."]
-    include_dirs.extend(args.include_dir)
-
-    abort_on_unknown_attribute = False
-    abort_on_namestyle = False
-
-    if args.abort_on_unknown_attribute or args.strict:
-        abort_on_unknown_attribute = True
-    if args.abort_on_name_style or args.strict:
-        abort_on_namestyle = True
-
-    known_extended_attributes_list = args.extended_attributes.split(",")
-    if len(known_extended_attributes_list) > 0:
-        vspec.model.vsstree.VSSNode.whitelisted_extended_attributes = known_extended_attributes_list
-        logging.info(
-            f"Known extended attributes: {', '.join(known_extended_attributes_list)}")
-
-    exporter = args.format.value
-
-    if args.uuid and args.no_uuid:
-        logging.error("Can not use --uuid and --no-uuid at the same time")
-        sys.exit(-1)
-    if args.no_uuid:
-        logging.warning("The argument --no-uuid is deprecated and will be removed in VSS 5.0")
-    print_uuid = False
-    if args.uuid:
-        print_uuid = True
-
-    vspec.load_quantities(args.vspec_file, args.quantity_file)
-    vspec.load_units(args.vspec_file, args.unit_file)
-
-    # Warn if unsupported feature is used
-    if args.no_expand and not exporter.feature_supported("no_expand"):
-        logging.warning("--no_expand not supported by exporter")
-
-    # process data type tree
-    if args.types_output_file is not None and not args.vspec_types_file:
-        parser.error("An output file for data types was provided. Please also provide "
-                     "the input vspec file for data types")
-    data_type_tree = None
-    if args.vspec_types_file:
-        data_type_tree = processDataTypeTree(
-            parser, args, include_dirs, abort_on_namestyle)
-        vspec.verify_mandatory_attributes(data_type_tree, abort_on_unknown_attribute)
-
-    try:
-        logging.info(f"Loading vspec from {args.vspec_file}...")
-        tree = vspec.load_tree(
-            args.vspec_file, include_dirs, VSSTreeType.SIGNAL_TREE,
-            break_on_name_style_violation=abort_on_namestyle,
-            expand_inst=False, data_type_tree=data_type_tree)
-
-        for overlay in args.overlays:
-            logging.info(f"Applying VSS overlay from {overlay}...")
-            othertree = vspec.load_tree(overlay, include_dirs, VSSTreeType.SIGNAL_TREE,
-                                        break_on_name_style_violation=abort_on_namestyle, expand_inst=False,
-                                        data_type_tree=data_type_tree)
-            vspec.merge_tree(tree, othertree)
-
-        vspec.check_type_usage(tree, VSSTreeType.SIGNAL_TREE, data_type_tree)
-        if not args.no_expand:
-            vspec.expand_tree_instances(tree)
-
-        vspec.clean_metadata(tree)
-        vspec.verify_mandatory_attributes(tree, abort_on_unknown_attribute)
-        logging.info("Calling exporter...")
-
-        # temporary until all exporters support data type tree
-        if args.format.name in SUPPORTED_STRUCT_EXPORT_FORMATS:
-            exporter.export(args, tree, print_uuid, data_type_tree)
+    def main(self, arguments):
+        initLogging()
+        parser = argparse.ArgumentParser(description="Convert vspec to other formats.")
+
+        parser.add_argument('--version', action='version', version=VERSION)
+        parser.add_argument('-I', '--include-dir', action='append', metavar='dir', type=str, default=[],
+                            help='Add include directory to search for included vspec files.')
+        if self.vspec2vss_config.extended_attributes_supported:
+            parser.add_argument('-e', '--extended-attributes', type=str, default="",
+                                help='Whitelisted extended attributes as comma separated list.')
+        parser.add_argument('-s', '--strict', action='store_true',
+                            help='Use strict checking: Terminate when anything not covered or not recommended '
+                                 'by VSS language or extensions is found.')
+        parser.add_argument('--abort-on-unknown-attribute', action='store_true',
+                            help="Terminate when an unknown attribute is found.")
+        parser.add_argument('--abort-on-name-style', action='store_true',
+                            help="Terminate if name style does not follow VSS standard catalog naming convention.")
+        if self.vspec2vss_config.uuid_supported:
+            parser.add_argument('--uuid', action='store_true',
+                                help='Include uuid in generated files. (Deprecated, will be removed in VSS-tools 6.0)')
+        if self.vspec2vss_config.expand_model and self.vspec2vss_config.no_expand_option_supported:
+            parser.add_argument('--no-expand', action='store_true',
+                                help='Do not expand tree.')
+        parser.add_argument('-o', '--overlays', action='append', metavar='overlays', type=str, default=[],
+                            help='Add overlay that will be layered on top of the VSS file in the order they appear.')
+        parser.add_argument('-q', '--quantity-file', action='append', metavar='quantity_file', type=str, default=[],
+                            help='Quantity file to be used for generation. Argument -q may be used multiple times.')
+        parser.add_argument('-u', '--unit-file', action='append', metavar='unit_file', type=str, default=[],
+                            help='Unit file to be used for generation. Argument -u may be used multiple times.')
+        parser.add_argument('vspec_file', metavar='<vspec_file>',
+                            help='The vehicle specification file to convert.')
+        if self.vspec2vss_config.output_file_required:
+            parser.add_argument('output_file', metavar='<output_file>',
+                                help='The file to write output to.')
+
+        if self.vspec2vss_config.type_tree_supported:
+            type_group = parser.add_argument_group('VSS Data Type Tree arguments',
+                                                   'Arguments related to struct/type support')
+
+            type_group.add_argument('-vt', '--vspec-types-file', action='append', metavar='vspec_types_file', type=str,
+                                    default=[],
+                                    help='Data types file in vspec format.')
+            if self.vspec2vss_config.separate_output_type_file_supported:
+                # Note we might get some odd errors if using -ot in a tool not supporting it due to conflict with -o
+                type_group.add_argument('-ot', '--types-output-file', metavar='<types_output_file>',
+                                        help='Output file for writing data types from vspec file. ' +
+                                        'If not specified, a single file is used where applicable. ' +
+                                        'In case of JSON and YAML, the data is exported under a ' +
+                                        'special key - "ComplexDataTypes"')
+
+        self.generator.add_arguments(parser.add_argument_group(
+            "Exporter specific arguments", ""))
+
+        args = parser.parse_args(arguments)
+
+        logging.info("VSS-tools version %s", VERSION)
+
+        include_dirs = ["."]
+        include_dirs.extend(args.include_dir)
+
+        abort_on_unknown_attribute = False
+        abort_on_namestyle = False
+
+        if args.abort_on_unknown_attribute or args.strict:
+            abort_on_unknown_attribute = True
+        if args.abort_on_name_style or args.strict:
+            abort_on_namestyle = True
+
+        if self.vspec2vss_config.extended_attributes_supported and (len(args.extended_attributes) > 0):
+            known_extended_attributes_list = args.extended_attributes.split(",")
+            vspec.model.vsstree.VSSNode.whitelisted_extended_attributes = known_extended_attributes_list
+            logging.info(f"Known extended attributes: {', '.join(known_extended_attributes_list)}")
         else:
-            if data_type_tree is not None:
-                parser.error(
-                    f"{args.format.name} format is not yet supported in vspec struct/data type support feature")
-            exporter.export(args, tree, print_uuid)
-        logging.info("All done.")
-    except vspec.VSpecError as e:
-        logging.error(f"Error: {e}")
-        sys.exit(255)
-
+            known_extended_attributes_list = list()
 
-def processDataTypeTree(parser: argparse.ArgumentParser, args, include_dirs,
-                        abort_on_namestyle: bool) -> VSSNode:
-    """
-    Helper function to process command line arguments and invoke logic for processing data
-    type information provided in vspec format
-    """
-    if args.types_output_file is None:
-        logging.info("Sensors and custom data types will be consolidated into one file.")
-        if args.format == Exporter.protobuf:
-            logging.info("Proto files will be written to the current working directory")
-
-    logging.warning("All exports do not yet support structs. Please check documentation for your exporter!")
-
-    first_tree = True
-    for type_file in args.vspec_types_file:
-        logging.info(f"Loading and processing struct/data type tree from {type_file}")
-        new_tree = vspec.load_tree(type_file, include_dirs, VSSTreeType.DATA_TYPE_TREE,
-                                   break_on_name_style_violation=abort_on_namestyle, expand_inst=False)
-        if first_tree:
-            tree = new_tree
-            first_tree = False
-        else:
-            vspec.merge_tree(tree, new_tree)
-    vspec.check_type_usage(tree, VSSTreeType.DATA_TYPE_TREE)
-    return tree
+        self.vspec2vss_config.generate_uuid = self.vspec2vss_config.uuid_supported and args.uuid
 
+        # Follow up to https://github.com/COVESA/vehicle_signal_specification/pull/721
+        # Deprecate --uuid
+        if self.vspec2vss_config.generate_uuid:
+            logging.warning("The argument --uuid is deprecated and the uuid feature is planned "
+                            "to be removed in VSS-tools 6.0")
+            logging.info("If you need static identifiers consider using the vspec2id tool")
+
+        self.vspec2vss_config.expand_model = (self.vspec2vss_config.expand_model and not
+                                              (self.vspec2vss_config.no_expand_option_supported and args.no_expand))
+
+        vspec.load_quantities(args.vspec_file, args.quantity_file)
+        vspec.load_units(args.vspec_file, args.unit_file)
+
+        # process data type tree
+        data_type_tree = None
+        if self.vspec2vss_config.type_tree_supported:
+            if self.vspec2vss_config.separate_output_type_file_supported:
+                if args.types_output_file is not None and not args.vspec_types_file:
+                    parser.error("An output file for data types was provided. Please also provide "
+                                 "the input vspec file for data types")
+            if args.vspec_types_file:
+                data_type_tree = self.processDataTypeTree(
+                    parser, args, include_dirs, abort_on_namestyle)
+                vspec.verify_mandatory_attributes(data_type_tree, abort_on_unknown_attribute)
 
-if __name__ == "__main__":
-    main(sys.argv[1:])
+        try:
+            logging.info(f"Loading vspec from {args.vspec_file}...")
+            tree = vspec.load_tree(
+                args.vspec_file, include_dirs, VSSTreeType.SIGNAL_TREE,
+                break_on_name_style_violation=abort_on_namestyle,
+                expand_inst=False, data_type_tree=data_type_tree)
+
+            for overlay in args.overlays:
+                logging.info(f"Applying VSS overlay from {overlay}...")
+                othertree = vspec.load_tree(overlay, include_dirs, VSSTreeType.SIGNAL_TREE,
+                                            break_on_name_style_violation=abort_on_namestyle, expand_inst=False,
+                                            data_type_tree=data_type_tree)
+                vspec.merge_tree(tree, othertree)
+
+            vspec.check_type_usage(tree, VSSTreeType.SIGNAL_TREE, data_type_tree)
+            if self.vspec2vss_config.expand_model:
+                vspec.expand_tree_instances(tree)
+
+            vspec.clean_metadata(tree)
+            vspec.verify_mandatory_attributes(tree, abort_on_unknown_attribute)
+            logging.info("Calling exporter...")
+
+            self.generator.generate(args, tree, self.vspec2vss_config, data_type_tree)
+            logging.info("All done.")
+        except vspec.VSpecError as e:
+            logging.error(f"Error: {e}")
+            sys.exit(255)
+
+    def processDataTypeTree(self, parser: argparse.ArgumentParser, args, include_dirs,
+                            abort_on_namestyle: bool) -> VSSNode:
+        """
+        Helper function to process command line arguments and invoke logic for processing data
+        type information provided in vspec format
+        """
+        if self.vspec2vss_config.separate_output_type_file_supported and \
+           args.types_output_file is None:
+            logging.info("Sensors and custom data types will be consolidated into one file.")
+
+        first_tree = True
+        for type_file in args.vspec_types_file:
+            logging.info(f"Loading and processing struct/data type tree from {type_file}")
+            new_tree = vspec.load_tree(type_file, include_dirs, VSSTreeType.DATA_TYPE_TREE,
+                                       break_on_name_style_violation=abort_on_namestyle, expand_inst=False)
+            if first_tree:
+                tree = new_tree
+                first_tree = False
+            else:
+                vspec.merge_tree(tree, new_tree)
+        vspec.check_type_usage(tree, VSSTreeType.DATA_TYPE_TREE)
+        return tree
```

### Comparing `vss-tools-4.1rc0/vss_tools.egg-info/PKG-INFO` & `vss_tools-5.0.0.dev0/vss_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vss-tools
-Version: 4.1rc0
+Version: 5.0.0.dev0
 Summary: COVESA Vehicle Signal Specification tooling.
 Home-page: https://github.com/COVESA/vss-tools
 License: Mozilla Public License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml>=5.1
@@ -34,15 +34,15 @@
 
 If you just want the latest version this should be sufficient:
 
 ```sh
 pip install vss-tools
 ```
 
-When installed tools like `vspec2x.py` shall be available on your path.
+When installed tools like `vspec2json.py` shall be available on your path.
 
 For more information see the [VSS-Tools wiki](https://github.com/COVESA/vss-tools/wiki/PyPI-packing)
 
 ## Usage
 
 For more information please visit the [COVESA VSS-Tools repository](https://github.com/COVESA/vss-tools).
```

### Comparing `vss-tools-4.1rc0/vss_tools.egg-info/SOURCES.txt` & `vss_tools-5.0.0.dev0/vss_tools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 vspec2ddsidl.py
 vspec2franca.py
 vspec2graphql.py
 vspec2id.py
 vspec2json.py
 vspec2jsonschema.py
 vspec2protobuf.py
-vspec2x.py
 vspec2yaml.py
 vspec/__init__.py
 vspec/loggingconfig.py
 vspec/py.typed
+vspec/vspec2vss_config.py
+vspec/vspec2x.py
+vspec/vss2x.py
 vspec/model/__init__.py
 vspec/model/constants.py
 vspec/model/exceptions.py
 vspec/model/vsstree.py
 vspec/utils/__init__.py
 vspec/utils/idgen_utils.py
 vspec/utils/stringstyle.py
```

