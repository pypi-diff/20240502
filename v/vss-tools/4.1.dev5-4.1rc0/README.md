# Comparing `tmp/vss-tools-4.1.dev5.tar.gz` & `tmp/vss-tools-4.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss-tools-4.1.dev5.tar", last modified: Mon May 15 13:28:48 2023, max compression
+gzip compressed data, was "vss-tools-4.1rc0.tar", last modified: Fri Dec  1 15:46:00 2023, max compression
```

## Comparing `vss-tools-4.1.dev5.tar` & `vss-tools-4.1rc0.tar`

### file list

```diff
@@ -1,43 +1,51 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/
--rw-r--r--   0 erik      (1000) erik      (1000)    16725 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)      238 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)    11930 2023-05-15 12:18:48.000000 vss-tools-4.1.dev5/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)       90 2023-05-15 11:45:18.000000 vss-tools-4.1.dev5/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     1380 2023-05-15 12:29:02.000000 vss-tools-4.1.dev5/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.104762 vss-tools-4.1.dev5/vspec/
--rwxr-xr-x   0 erik      (1000) erik      (1000)    35008 2023-05-04 13:37:39.000000 vss-tools-4.1.dev5/vspec/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)      379 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/loggingconfig.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/vspec/model/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec/model/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     6254 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec/model/constants.py
--rw-r--r--   0 erik      (1000) erik      (1000)      734 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec/model/exceptions.py
--rw-r--r--   0 erik      (1000) erik      (1000)    18800 2023-05-04 13:37:39.000000 vss-tools-4.1.dev5/vspec/model/vsstree.py
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/py.typed
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/vspec/utils/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/utils/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)      662 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/utils/stringstyle.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/vspec/vssexporters/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/vssexporters/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4612 2023-05-15 09:35:05.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2binary.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2786 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2csv.py
--rw-r--r--   0 erik      (1000) erik      (1000)     8117 2023-05-15 09:11:01.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2ddsidl.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2497 2023-02-22 10:27:00.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2franca.py
--rw-r--r--   0 erik      (1000) erik      (1000)     5029 2023-04-17 11:54:24.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2graphql.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3863 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2json.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     5933 2023-05-04 13:37:39.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2protobuf.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3864 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec/vssexporters/vss2yaml.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      355 2023-03-29 09:18:58.000000 vss-tools-4.1.dev5/vspec2csv.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      355 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec2ddsidl.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      375 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec2franca.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      354 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec2graphql.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      357 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec2json.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      185 2023-05-04 07:44:52.000000 vss-tools-4.1.dev5/vspec2protobuf.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     9867 2023-05-04 13:37:39.000000 vss-tools-4.1.dev5/vspec2x.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)      357 2022-08-23 11:55:56.000000 vss-tools-4.1.dev5/vspec2yaml.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-05-15 13:28:48.108762 vss-tools-4.1.dev5/vss_tools.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)      238 2023-05-15 13:28:48.000000 vss-tools-4.1.dev5/vss_tools.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      820 2023-05-15 13:28:48.000000 vss-tools-4.1.dev5/vss_tools.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-05-15 13:28:48.000000 vss-tools-4.1.dev5/vss_tools.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       59 2023-05-15 13:28:48.000000 vss-tools-4.1.dev5/vss_tools.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        6 2023-05-15 13:28:48.000000 vss-tools-4.1.dev5/vss_tools.egg-info/top_level.txt
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.956628 vss-tools-4.1rc0/
+-rw-r--r--   0 erik      (1000) erik      (1000)    16725 2023-10-18 07:14:13.000000 vss-tools-4.1rc0/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)       23 2023-12-01 12:16:45.000000 vss-tools-4.1rc0/MANIFEST.in
+-rw-r--r--   0 erik      (1000) erik      (1000)     2190 2023-12-01 15:46:00.956628 vss-tools-4.1rc0/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1794 2023-12-01 12:16:45.000000 vss-tools-4.1rc0/README-PYPI.md
+-rw-r--r--   0 erik      (1000) erik      (1000)    11798 2023-12-01 15:41:27.000000 vss-tools-4.1rc0/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)       90 2023-10-18 07:14:13.000000 vss-tools-4.1rc0/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2023-12-01 15:46:00.956628 vss-tools-4.1rc0/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1922 2023-12-01 15:43:47.000000 vss-tools-4.1rc0/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.948628 vss-tools-4.1rc0/vspec/
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    36655 2023-12-01 15:14:41.000000 vss-tools-4.1rc0/vspec/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      497 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/loggingconfig.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.952628 vss-tools-4.1rc0/vspec/model/
+-rw-r--r--   0 erik      (1000) erik      (1000)      263 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/model/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     8174 2023-12-01 15:14:41.000000 vss-tools-4.1rc0/vspec/model/constants.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      844 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/model/exceptions.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    19844 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec/model/vsstree.py
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-10-18 07:14:13.000000 vss-tools-4.1rc0/vspec/py.typed
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.952628 vss-tools-4.1rc0/vspec/utils/
+-rw-r--r--   0 erik      (1000) erik      (1000)      850 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec/utils/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2366 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec/utils/idgen_utils.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      774 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/utils/stringstyle.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     6777 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec/utils/vss2id_val.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.952628 vss-tools-4.1rc0/vspec/vssexporters/
+-rw-r--r--   0 erik      (1000) erik      (1000)      263 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4828 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2binary.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3365 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2csv.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    12074 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2ddsidl.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2714 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2franca.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     5191 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2graphql.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     5285 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2id.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4307 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2json.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     5792 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2jsonschema.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     6085 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2protobuf.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4226 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec/vssexporters/vss2yaml.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      439 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2csv.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      439 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2ddsidl.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      441 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2franca.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      446 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2graphql.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      427 2023-12-01 14:57:23.000000 vss-tools-4.1rc0/vspec2id.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      441 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2json.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      453 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2jsonschema.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      449 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2protobuf.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    10878 2023-12-01 15:41:27.000000 vss-tools-4.1rc0/vspec2x.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      441 2023-12-01 12:23:34.000000 vss-tools-4.1rc0/vspec2yaml.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-12-01 15:46:00.956628 vss-tools-4.1rc0/vss_tools.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2190 2023-12-01 15:46:00.000000 vss-tools-4.1rc0/vss_tools.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      998 2023-12-01 15:46:00.000000 vss-tools-4.1rc0/vss_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-12-01 15:46:00.000000 vss-tools-4.1rc0/vss_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       59 2023-12-01 15:46:00.000000 vss-tools-4.1rc0/vss_tools.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        6 2023-12-01 15:46:00.000000 vss-tools-4.1rc0/vss_tools.egg-info/top_level.txt
```

### Comparing `vss-tools-4.1.dev5/LICENSE` & `vss-tools-4.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `vss-tools-4.1.dev5/README.md` & `vss-tools-4.1rc0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -19,28 +19,29 @@
 * Obsolete Tools are tools that are not maintained and not functional.
 
 A tool in the Contributed Tools category may be moved to the Obsolete category if it has been non-functional for at least 6 months.
 Tools in the Obsolete Tools category may be deleted after 12 months.
 
 Examples on tool usage can be found in the [VSS Makefile](https://github.com/COVESA/vehicle_signal_specification/blob/master/Makefile) and in tool-specific documentation, if existing.
 
- Tool | Description | Tool Category | Documentation |
-| ------------------ | ----------- | -------------------- |-------------------- |
-| [vspec2x.py](vspec2x.py) | Parses and expands VSS into different text based output formats. Currently supports `json`, `yaml`,`csv`,`idl`  | Community Supported | Try `./vspec2x --help` or check [vspec2x documentation](docs/vspec2x.md) |
-[vspec2csv.py](vspec2csv.py) | Shortcut for [vspec2x.py](vspec2x.py) generating CSV output | Community Supported |  Check [vspec2x documentation](docs/vspec2x.md) |
-[vspec2ddsidl.py](vspec2ddsidl.py) | Shortcut for [vspec2x.py](vspec2x.py) generating DDS-IDL output | Community Supported | [VSS2DDSIDL Documentation](docs/VSS2DDSIDL.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
-[vspec2json.py](vspec2json.py) |  Shortcut for [vspec2x.py](vspec2x.py) generating JSON output | Community Supported | Check [vspec2x documentation](docs/vspec2x.md) |
-[vspec2yaml.py](vspec2yaml.py) | Shortcut for [vspec2x.py](vspec2x.py) generating flattened YAML output | Community Supported | Check [vspec2x documentation](docs/vspec2x.md) |
-[vspec2binary.py](vspec2binary.py) | The binary toolset consists of a tool that translates the VSS YAML specification to the binary file format (see below), and two libraries that provides methods that are likely to be needed by a server that manages the VSS tree, one written in C, and one in Go | Community Supported | [vspec2binary Documentation](binary/README.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
-[vspec2franca.py](vspec2franca.py) | Parses and expands a VSS and generates a Franca IDL specification | Community Supported | Check [vspec2x documentation](docs/vspec2x.md) |
-[vspec2c.py](contrib/vspec2c.py) | The vspec2c tooling allows a vehicle signal specification to be translated from its source YAML file to native C code that has the entire specification encoded in it. | Obsolete (2022-11-01) | [Documentation](obsolete/vspec2c/README.md) |
-[vspec2ocf.py](contrib/ocf/vspec2ocf.py) | Parses and expands a VSS and generates a OCF specification | Obsolete (2022-11-01) | - |
-[vspec2protobuf.py](vspec2protobuf.py) | Parses and expands a VSS and generates a Protobuf specification | Contrib | - |
-[vspec2ttl.py](contrib/vspec2ttl/vspec2ttl.py) | Parses and expands a VSS and generates a TTL specification | Contrib  | - |
-[vspec2graphql.py](contrib/vspec2graphql.py) | Parses and expands a VSS and generates a GraphQL specification | Community Supported  | [Documentation](docs/VSS2GRAPHQL.md) |
+ Tool | Description | Tool Category         | Documentation                                                                                                         |
+| ------------------ | ----------- |-----------------------|-----------------------------------------------------------------------------------------------------------------------|
+| [vspec2x.py](vspec2x.py) | Parses and expands VSS into different text based output formats. Currently supports `json`, `yaml`,`csv`,`idl`  | Community Supported   | Try `./vspec2x --help` or check [vspec2x documentation](docs/vspec2x.md)                                              |
+[vspec2csv.py](vspec2csv.py) | Shortcut for [vspec2x.py](vspec2x.py) generating CSV output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
+[vspec2ddsidl.py](vspec2ddsidl.py) | Shortcut for [vspec2x.py](vspec2x.py) generating DDS-IDL output | Community Supported   | [VSS2DDSIDL Documentation](docs/VSS2DDSIDL.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
+[vspec2json.py](vspec2json.py) |  Shortcut for [vspec2x.py](vspec2x.py) generating JSON output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
+[vspec2yaml.py](vspec2yaml.py) | Shortcut for [vspec2x.py](vspec2x.py) generating flattened YAML output | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
+[vspec2binary.py](vspec2binary.py) | The binary toolset consists of a tool that translates the VSS YAML specification to the binary file format (see below), and two libraries that provides methods that are likely to be needed by a server that manages the VSS tree, one written in C, and one in Go | Community Supported   | [vspec2binary Documentation](binary/README.md). For general parameters check [vspec2x documentation](docs/vspec2x.md) |
+[vspec2franca.py](vspec2franca.py) | Parses and expands a VSS and generates a Franca IDL specification | Community Supported   | Check [vspec2x documentation](docs/vspec2x.md)                                                                        |
+[vspec2c.py](obsolete/vspec2c.py) | The vspec2c tooling allows a vehicle signal specification to be translated from its source YAML file to native C code that has the entire specification encoded in it. | Obsolete (2022-11-01) | [Documentation](obsolete/vspec2c/README.md)                                                                           |
+[vspec2ocf.py](obsolete/ocf/vspec2ocf.py) | Parses and expands a VSS and generates a OCF specification | Obsolete (2022-11-01) | -                                                                                                                     |
+[vspec2protobuf.py](vspec2protobuf.py) | Parses and expands a VSS and generates a Protobuf specification | Contrib               | -                                                                                                                     |
+[vspec2ttl.py](contrib/vspec2ttl/vspec2ttl.py) | Parses and expands a VSS and generates a TTL specification | Contrib               | -                                                                                                                     |
+[vspec2graphql.py](vspec2graphql.py) | Parses and expands a VSS and generates a GraphQL specification | Community Supported   | [Documentation](docs/VSS2GRAPHQL.md)                                                                                  |
+[vspec2id.py](vspec2id.py) | Generates and validates static UIDs for a VSS | WIP                   | [vspec2id Documentation](./docs/vspec2id.md)                                                                          |
 
 ## Tool Architecture
 
 All current tools are based on common Python functionality in the `vspec` folder to read, parse and expand a Vehicle Signal Specification files(*.vspec files). As an example, if the standard [VSS root file](https://github.com/COVESA/vehicle_signal_specification/blob/master/spec/VehicleSignalSpecification.vspec) is given as input then the Python tooling will read all included files, do a validation of the content, expand any instances used and create an in-memory representation which then can be used by specialized tools to generate the wanted output.
 
 ## Getting started
 
@@ -137,46 +138,8 @@
 ```
 
 ## Pre-commit set up
 This repository is set up to use pre-commit hooks. After you clone the project, run `pre-commit install` to install pre-commit into your git hooks. pre-commit will now run on every commit. Every time you clone a project using pre-commit running pre-commit install should always be the first thing you do.
 
 ## Building and installing with Pip
 
-*Note: This is still an experimental feature*
-
-Vss-tools can be be built and uploaded to pypi. Currently it is built and published to [TestPypPI](https://test.pypi.org/)
-only as shown below. Version used is hardcoded in [setup.py](setup.py].
-
-```sh
-git clean -fdx
-python -m build
-python -m twine upload --repository testpypi dist/*
-```
-
-Available versions can be found [here](https://test.pypi.org/project/vss-tools/).
-Currently only pre-releases exist, which means that `--pre` must be used to install it.
-
-```sh
-pip install --pre --index-url -U https://test.pypi.org/simple/ vss-tools
-```
-
-As `--pre` is used you might need to also specify default repository to find dependencies like anytree.
-
-```sh
-python -m pip install --pre --index-url https://test.pypi.org/simple/ --extra-index-url  https://pypi.org/simple/ vss-tools
-```
-
-After installation, tools like `vspec2x.py` shall be available on your path without the need of cloning the repository.
-For development purposes you can install directly from source:
-
-```sh
-pip install -e .
-```
-
-### Pip versioning
-
-This is the versions types that may exist in PyPI for vss-tools and used for local pip install (`pip install -e .`)
-
-* X.Y or X.Y.Z - A released version.
-* X.Y.devN, N starting from 0 - Developer builds - normally not published to PyPI.
-* X.YaN, N starting from 0 - Pre-releases, may be published to PyPI if needed for testing purposes.
-* X.YrcN, N starting from 0 - Release candidates, to be published around two weeks before a major/minor release.
+For usage of VSS-Tools with Pip (PyPI) please see [README-PYPI.md](README-PYPI.md)
```

### Comparing `vss-tools-4.1.dev5/vspec/__init__.py` & `vss-tools-4.1rc0/vspec/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+# Copyright (c) 2016 Contributors to COVESA
 #
-# (C) 2021 Robert Bosch GmbH
-# (C) 2018 Volvo Cars
-# (C) 2016 Jaguar Land Rover
-#
-# All files and artifacts in this repository are licensed under the
-# provisions of the license provided by the LICENSE file in this repository.
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
+# SPDX-License-Identifier: MPL-2.0
+
 #
 # VSpec file parser.
 #
 
 import yaml
 import os
 import uuid
@@ -19,15 +19,15 @@
 from copy import deepcopy
 from typing import List, Optional
 
 from anytree import (Resolver, LevelOrderIter, PreOrderIter, RenderTree)  # type: ignore[import]
 
 from .model.vsstree import VSSNode
 from .model.exceptions import ImpossibleMergeException, IncompleteElementException
-from .model.constants import VSSTreeType, Unit
+from .model.constants import VSSTreeType, VSSUnitCollection, VSSQuantityCollection
 
 nestable_types = set(["branch", "struct"])
 
 
 class VSpecError(Exception):
     def __init__(self, *args, **kwargs):
         self.file_name = args[0]
@@ -771,14 +771,18 @@
         for item in tree_dict.keys():
             logging.info(f"Found root node {item}")
         raise Exception(
             f"Invalid VSS model, must have single root node, found {len(tree_dict)}")
 
     root_element_name = next(iter(tree_dict.keys()))
     root_element = tree_dict[root_element_name]
+    if root_element['type'] != 'branch':
+        raise Exception(
+            f"Invalid VSS model, root must be branch, found {root_element_name} of type {root_element['type']}")
+
     tree_root = VSSNode(
         root_element_name,
         root_element,
         tree_type.available_types(),
         break_on_name_style_violation=break_on_name_style_violation)
 
     if "children" in root_element.keys():
@@ -855,27 +859,60 @@
     namespace_uuid = uuid.uuid5(uuid.NAMESPACE_OID, VSS_NAMESPACE)
     vss_element: VSSNode
     for vss_element in PreOrderIter(root):
         vss_element.uuid = uuid.uuid5(
             namespace_uuid, vss_element.qualified_name()).hex
 
 
+def load_quantities(vspec_file: str, quantity_files: List[str]):
+    """
+    Reset the list of quantities defined (if any)
+    and add new quantities
+    """
+    VSSQuantityCollection.reset_quantities()
+
+    total_nbr_quantities = 0
+    if not quantity_files:
+        # Search for a file quantities.yaml in same directory as vspec file
+        vspec_dir = os.path.dirname(os.path.realpath(vspec_file))
+        default_vss_quantity_file = vspec_dir + os.path.sep + 'quantities.yaml'
+        if os.path.exists(default_vss_quantity_file):
+            total_nbr_quantities = VSSQuantityCollection.load_config_file(default_vss_quantity_file)
+            logging.info(f"Added {total_nbr_quantities} quantities from {default_vss_quantity_file}")
+    else:
+        for quantity_file in quantity_files:
+            nbr_quantities = VSSQuantityCollection.load_config_file(quantity_file)
+            if (nbr_quantities == 0):
+                logging.warning(f"Warning: No quantities found in {quantity_file}")
+            else:
+                logging.info(f"Added {nbr_quantities} quantities from {quantity_file}")
+                total_nbr_quantities += nbr_quantities
+
+    if (total_nbr_quantities == 0):
+        logging.info("No quantities defined!")
+
+
 def load_units(vspec_file: str, unit_files: List[str]):
+    """
+    Reset the list of units defined (if any)
+    and add new units
+    """
+    VSSUnitCollection.reset_units()
 
     total_nbr_units = 0
     if not unit_files:
         # Search for a file units.yaml in same directory as vspec file
         vspec_dir = os.path.dirname(os.path.realpath(vspec_file))
         default_vss_unit_file = vspec_dir + os.path.sep + 'units.yaml'
         if os.path.exists(default_vss_unit_file):
-            total_nbr_units = Unit.load_config_file(default_vss_unit_file)
+            total_nbr_units = VSSUnitCollection.load_config_file(default_vss_unit_file)
             logging.info(f"Added {total_nbr_units} units from {default_vss_unit_file}")
     else:
         for unit_file in unit_files:
-            nbr_units = Unit.load_config_file(unit_file)
+            nbr_units = VSSUnitCollection.load_config_file(unit_file)
             if (nbr_units == 0):
                 logging.warning(f"Warning: No units found in {unit_file}")
             else:
                 logging.info(f"Added {nbr_units} units from {unit_file}")
                 total_nbr_units += nbr_units
 
     if (total_nbr_units == 0):
@@ -933,15 +970,15 @@
     """
     nonexistant_types = []
     for _, _, node in RenderTree(signal_root):
         # signals with user-defined data types
         if node.is_signal() and node.datatype is None:
             if data_type_root is None or (not node.does_attribute_exist(
                     data_type_root,
-                    lambda n: n.data_type_str,
+                    lambda n: n.base_data_type_str(),
                     lambda n: n.qualified_name(),
                     lambda n: n.is_struct())):
                 nonexistant_types.append(f'{node.data_type_str}')
 
     if len(nonexistant_types) > 0:
         error_str = ", ".join(nonexistant_types)
         logging.error(
```

### Comparing `vss-tools-4.1.dev5/vspec/model/exceptions.py` & `vss-tools-4.1rc0/vspec/model/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
+# Copyright (c) 2023 Contributors to COVESA
 #
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
-#
-# All files and artifacts in this repository are licensed under the
-# provisions of the license provided by the LICENSE file in this repository.
-#
+# SPDX-License-Identifier: MPL-2.0
 
 class NameStyleValidationException(Exception):
     def __init__(self, message):
 
         # Call the base class constructor with the parameters it needs
         super().__init__(message)
```

### Comparing `vss-tools-4.1.dev5/vspec/model/vsstree.py` & `vss-tools-4.1rc0/vspec/model/vsstree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 
+# Copyright (c) 2021 Contributors to COVESA
 #
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
-#
-# All files and artifacts in this repository are licensed under the
-# provisions of the license provided by the LICENSE file in this repository.
-#
+# SPDX-License-Identifier: MPL-2.0
 
 from anytree import Node, Resolver, ChildResolverError, RenderTree  # type: ignore[import]
-from .constants import VSSType, VSSDataType, Unit, VSSConstant
+from .constants import VSSType, VSSDataType, VSSUnitCollection, VSSUnit
 from .exceptions import NameStyleValidationException, \
     ImpossibleMergeException, IncompleteElementException
 from typing import Any, Optional, Set, List
 import copy
 import re
 import sys
 import logging
@@ -35,36 +36,40 @@
     datatype: Optional[VSSDataType]
 
     # The node types that the nodes can take
     available_types: Set[str] = set()
 
     core_attributes = ["type", "children", "datatype", "description", "unit", "uuid", "min", "max", "allowed",
                        "instantiate", "aggregate", "default", "instances", "deprecation", "arraysize",
-                       "comment", "$file_name$"]
+                       "comment", "$file_name$", "fka"]
 
     # List of accepted extended attributes. In strict terminate if an attribute is
     # neither in core or extended,
     whitelisted_extended_attributes: List[str] = []
 
-    unit: Optional[VSSConstant]
+    unit: Optional[VSSUnit] = None
 
     min = ""
     max = ""
     allowed = ""
     instantiate = True
 
     ttl_name = ""
 
     default = ""
 
     instances = None
+    expanded = False
     deprecation = ""
+    fka = ""
 
     def __deepcopy__(self, memo):
-        return VSSNode(self.name, self.source_dict.copy(), self.available_types.copy(),
+        # Deep copy of source_dict and children needed as overlay or programmatic changes
+        # in exporters otherwise risk changing values not only for current instances but also for others
+        return VSSNode(self.name, copy.deepcopy(self.source_dict), self.available_types.copy(),
                        parent=None, children=copy.deepcopy(self.children, memo))
 
     def __init__(self, name, source_dict: dict, available_types: Set[str], parent=None,
                  children=None, break_on_unknown_attribute=False, break_on_name_style_violation=False):
         """Creates an VSS Node object from parsed yaml instance represented as a dict.
 
             Args:
@@ -92,19 +97,14 @@
         self.source_dict = source_dict
         self.unpack_source_dict()
 
         if (self.is_property() and not self.parent.is_struct()):
             logging.error(f"Orphan property detected. {self.name} is not defined under a struct")
             sys.exit(-1)
 
-        if (self.is_signal() or self.is_property()) and "datatype" not in self.source_dict.keys():
-            raise IncompleteElementException(
-                (f"Incomplete element {self.name} from {self.source_dict['$file_name$']}: "
-                 f"Elements of type {self.type.value} need to have a datatype declared."))
-
         try:
             self.validate_name_style(self.source_dict["$file_name$"])
         except NameStyleValidationException as e:
             logging.warning(f"Exception: {e}")
             if break_on_name_style_violation:
                 logging.error("You asked for strict checking. Terminating.")
                 sys.exit(-1)
@@ -124,32 +124,44 @@
                 del self.extended_attributes[name]
 
         self.type = VSSType.from_str(self.source_dict["type"])
 
         for attribute in VSSNode.core_attributes:
             extractCoreAttribute(attribute)
 
-        # Datatype and unit need special handling, so we extract them again
-        if "datatype" in self.source_dict.keys():
-            if not self.is_struct():
+        # Datatype and unit need special handling, so we do some further analysis
+        # self.data_type shall only be set if base type is a primitive (VSSDataType)
+        if self.has_datatype():
+            if self.is_signal() or self.is_property():
                 self.data_type_str = self.source_dict["datatype"]
                 self.validate_and_set_datatype()
             else:
-                logging.warning(f"Data type specified for struct node: {self.name}. Ignoring it")
+                logging.error("Item %s cannot have datatype, only allowed for signal and property!", self.name)
+                sys.exit(-1)
+        elif (self.is_signal() or self.is_property()):
+            raise IncompleteElementException(
+                (f"Incomplete element {self.name} from {self.source_dict['$file_name$']}: "
+                 f"Elements of type {self.type.value} need to have a datatype declared."))
 
         # Units are applicable only for primitives. Not user defined types.
-        if "unit" in self.source_dict.keys() and self.has_datatype():
+        if self.has_unit():
+
+            if not (self.is_signal() or self.is_property()):
+                logging.error("Item %s cannot have unit, only allowed for signal and property!", self.name)
+                sys.exit(-1)
+
             unit = self.source_dict["unit"]
-            try:
-                self.unit = Unit.from_str(unit)
-            except KeyError:
+            self.unit = VSSUnitCollection.get_unit(unit)
+            if self.unit is None:
                 logging.error(f"Unknown unit {unit} for signal {self.qualified_name()}. Terminating.")
                 sys.exit(-1)
-        else:
-            self.unit = None
+
+            if not self.has_datatype():
+                logging.error("Unit specified for item not using standard datatype: %s", self.name)
+                sys.exit(-1)
 
         if self.has_instances() and not self.is_branch():
             logging.error(
                 f"Only branches can be instantiated. {self.qualified_name()} is of type {self.type}")
             sys.exit(-1)
 
     def validate_name_style(self, sourcefile):
@@ -168,14 +180,23 @@
         # relax camel case requirement for struct properties
         if not self.is_property() and not camel_regexp.match(self.name):
             raise NameStyleValidationException(
                 (f'Node "{self.name}" found in file "{sourcefile}" is not following naming conventions. ',
                  'It is recommended that node names use camel case, starting with a capital letter, ',
                  'only using letters A-z and numbers 0-9.'))
 
+    def base_data_type_str(self) -> str:
+        """
+        This gives the base type of the type, i.e. without array suffix if present
+        """
+        suffix = "[]"
+        if self.data_type_str.endswith(suffix):
+            return self.data_type_str[:-len(suffix)]
+        return self.data_type_str
+
     def qualified_name(self, separator=DEFAULT_SEPARATOR) -> str:
         """Returns fully qualified name of a VSS object (including path) using the defined separator (or default ='.')
             Args:
                 separator: Optional parameter as custom separator between path elements of this instance
 
             Returns:
                 Fully Qualified VSS Node string representation including complete path.
@@ -293,15 +314,15 @@
             Returns:
                 True if this instance has a data type, False otherwise
         """
         return hasattr(self, "datatype") and self.datatype is not None
 
     def get_datatype(self) -> str:
         """Returns:
-                The name of the dataype or empty string if no datatype
+                The name of the datatype or empty string if no datatype
         """
         return self.data_type_str
 
     def has_instances(self) -> bool:
         """Check if this instance has a VSS instances
 
             Returns:
```

### Comparing `vss-tools-4.1.dev5/vspec/vssexporters/vss2binary.py` & `vss-tools-4.1rc0/vspec/vssexporters/vss2binary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 #!/usr/bin/env python3
 
-# (c) 2022 Geotab Inc
-#
-# All files and artifacts in this repository are licensed under the
-# provisions of the license provided by the LICENSE file in this repository.
+# Copyright (c) 2022 Contributors to COVESA
 #
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
+# SPDX-License-Identifier: MPL-2.0
+
 # Convert vspec tree to binary format
 
 import argparse
 import logging
 import ctypes
 import os.path
 from vspec.model.vsstree import VSSNode, VSSType
 
 out_file = ""
 _cbinary = None
 
 
+def feature_supported(feature_name: str):
+    """Return true for supported optional arguments/features"""
+    return False
+
+
 def createBinaryCnode(fname, nodename, nodetype, uuid, description, nodedatatype, nodemin, nodemax, unit, allowed,
                       defaultAllowed, validate, children):
     global _cbinary
     _cbinary.createBinaryCnode(fname, nodename, nodetype, uuid, description, nodedatatype, nodemin, nodemax, unit,
                                allowed, defaultAllowed, validate, children)
```

### Comparing `vss-tools-4.1.dev5/vspec/vssexporters/vss2csv.py` & `vss-tools-4.1rc0/vspec/vssexporters/vss2csv.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,90 @@
 #!/usr/bin/env python3
 
-# (c) 2022 Robert Bosch GmbH
-# (c) 2021 BMW Group
-#
-# All files and artifacts in this repository are licensed under the
-# provisions of the license provided by the LICENSE file in this repository.
+# Copyright (c) 2021 Contributors to COVESA
 #
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
+# SPDX-License-Identifier: MPL-2.0
+
 # Convert vspec tree to CSV
 
 
 import argparse
 import logging
 from vspec.model.vsstree import VSSNode
 from anytree import PreOrderIter  # type: ignore[import]
 from vspec.loggingconfig import initLogging
 from typing import AnyStr
 
 
+def feature_supported(feature_name: str):
+    """Return true for supported arguments/features"""
+    if feature_name in ['no_expand']:
+        return True
+    return False
+
+
 def add_arguments(parser: argparse.ArgumentParser):
     parser.description = "The csv exporter does not support any additional arguments."
 
 # Write the header line
 
 
-def print_csv_header(file, uuid, entry_type: AnyStr):
+def print_csv_header(file, uuid, entry_type: AnyStr, include_instance_column: bool):
     arg_list = [entry_type, "Type", "DataType", "Deprecated", "Unit",
                 "Min", "Max", "Desc", "Comment", "Allowed", "Default"]
     if uuid:
         arg_list.append("Id")
+    if include_instance_column:
+        arg_list.append("Instances")
     file.write(format_csv_line(arg_list))
 
 # Format a data or header line according to the CSV standard (IETF RFC 4180)
 
 
 def format_csv_line(csv_fields):
     formatted_csv_line = ""
     for csv_field in csv_fields:
         formatted_csv_line = formatted_csv_line + '"' + str(csv_field).replace('"', '""') + '",'
     return formatted_csv_line[:-1] + '\n'
 
 # Write the data lines
 
 
-def print_csv_content(file, tree: VSSNode, uuid):
+def print_csv_content(file, tree: VSSNode, uuid, include_instance_column: bool):
     tree_node: VSSNode
     for tree_node in PreOrderIter(tree):
         data_type_str = tree_node.get_datatype()
         unit_str = tree_node.get_unit()
         arg_list = [tree_node.qualified_name('.'), tree_node.type.value, data_type_str, tree_node.deprecation,
                     unit_str, tree_node.min, tree_node.max, tree_node.description, tree_node.comment,
                     tree_node.allowed, tree_node.default]
         if uuid:
             arg_list.append(tree_node.uuid)
+        if include_instance_column and tree_node.instances is not None:
+            arg_list.append(tree_node.instances)
         file.write(format_csv_line(arg_list))
 
 
 def export(config: argparse.Namespace, signal_root: VSSNode, print_uuid, data_type_root: VSSNode):
     logging.info("Generating CSV output...")
 
     # generic entry should be written when both data types and signals are being written to the same file
     generic_entry = data_type_root is not None and config.types_output_file is None
     with open(config.output_file, 'w') as f:
         signal_entry_type = "Node" if generic_entry else "Signal"
-        print_csv_header(f, print_uuid, signal_entry_type)
-        print_csv_content(f, signal_root, print_uuid)
+        print_csv_header(f, print_uuid, signal_entry_type, config.no_expand)
+        print_csv_content(f, signal_root, print_uuid, config.no_expand)
         if data_type_root is not None and generic_entry is True:
-            print_csv_content(f, data_type_root, print_uuid)
+            print_csv_content(f, data_type_root, print_uuid, config.no_expand)
 
     if data_type_root is not None and generic_entry is False:
         with open(config.types_output_file, 'w') as f:
-            print_csv_header(f, print_uuid, "Node")
-            print_csv_content(f, data_type_root, print_uuid)
+            print_csv_header(f, print_uuid, "Node", config.no_expand)
+            print_csv_content(f, data_type_root, print_uuid, config.no_expand)
 
 
 if __name__ == "__main__":
     initLogging()
```

### Comparing `vss-tools-4.1.dev5/vspec/vssexporters/vss2franca.py` & `vss-tools-4.1rc0/vspec/vssexporters/vss2franca.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 #!/usr/bin/env python3
 
-# (c) 2021 BMW Group
-#
-# All files and artifacts in this repository are licensed under the
-# provisions of the license provided by the LICENSE file in this repository.
+# Copyright (c) 2021 Contributors to COVESA
 #
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
+# SPDX-License-Identifier: MPL-2.0
+
 # Convert vspec tree to franca
 
 
 import argparse
 from vspec.model.vsstree import VSSNode
 from anytree import PreOrderIter  # type: ignore[import]
 
 
+def feature_supported(feature_name: str):
+    """Return true for supported optional arguments/features"""
+    return False
+
+
 def add_arguments(parser: argparse.ArgumentParser):
     # no additional output for Franca at this moment
     parser.add_argument('-v', metavar='version', help=" Add version information to franca file.")
 
 # Write the header line
```

### Comparing `vss-tools-4.1.dev5/vspec/vssexporters/vss2graphql.py` & `vss-tools-4.1rc0/vspec/vssexporters/vss2graphql.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
+# Copyright (c) 2022 Contributors to COVESA
 #
-# Copyright (C) 2022, Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
-#
-# All files and artifacts in this repository are licensed under the
-# provisions of the license provided by the LICENSE file in this repository.
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
+# SPDX-License-Identifier: MPL-2.0
 
 import argparse
 from vspec.model.vsstree import VSSNode
 from vspec.utils.stringstyle import camel_back
 from vspec.model.constants import VSSDataType
 from vspec import VSpecError
 from typing import Dict
@@ -52,14 +53,19 @@
     VSSDataType.BOOLEAN: GraphQLBoolean,
     VSSDataType.BOOLEAN_ARRAY: GraphQLList(GraphQLBoolean),
     VSSDataType.STRING: GraphQLString,
     VSSDataType.STRING_ARRAY: GraphQLList(GraphQLString),
 }
 
 
+def feature_supported(feature_name: str):
+    """Return true for supported optional arguments/features"""
+    return False
+
+
 def add_arguments(parser: argparse.ArgumentParser):
     # no additional output for graphql at this moment
     parser.description = "The graphql exporter never generates uuid, i.e. the --uuid option has no effect."
     parser.add_argument('--gqlfield', action='append', nargs=2,
                         help=" Add additional fields to the nodes in the graphql schema. "
                              "use: <field_name> <description>")
```

### Comparing `vss-tools-4.1.dev5/vspec/vssexporters/vss2json.py` & `vss-tools-4.1rc0/vspec/vssexporters/vss2json.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 #!/usr/bin/env python3
 
-# (c) 2022 Robert Bosch GmbH
-#
-# All files and artifacts in this repository are licensed under the
-# provisions of the license provided by the LICENSE file in this repository.
+# Copyright (c) 2022 Contributors to COVESA
 #
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
+# SPDX-License-Identifier: MPL-2.0
+
 # Convert vspec tree to JSON
 
 from vspec.model.vsstree import VSSNode
 import argparse
 import json
 import logging
 from typing import Dict, Any
 from vspec.loggingconfig import initLogging
 
 
+def feature_supported(feature_name: str):
+    """Return true for supported arguments/features"""
+    if feature_name in ['no_expand']:
+        return True
+    return False
+
+
 def add_arguments(parser: argparse.ArgumentParser):
     parser.add_argument('--json-all-extended-attributes', action='store_true',
                         help="Generate all extended attributes found in the model "
                              "(default is generating only those given by the -e/--extended-attributes parameter).")
     parser.add_argument('--json-pretty', action='store_true',
                         help=" Pretty print JSON output.")
 
@@ -63,14 +72,18 @@
         json_dict[node.name]["uuid"] = node.uuid
 
     for k, v in node.extended_attributes.items():
         if not config.json_all_extended_attributes and k not in VSSNode.whitelisted_extended_attributes:
             continue
         json_dict[node.name][k] = v
 
+    # Include instance information if we run tool in "no-expand" mode
+    if config.no_expand and node.instances is not None:
+        json_dict[node.name]["instances"] = node.instances
+
     # Might be better to not generate child dict, if there are no children
     # if node.type == VSSType.BRANCH and len(node.children) != 0:
     #    json_dict[node.name]["children"]={}
 
     # But old JSON code always generates children, so lets do so to
     if node.is_branch() or node.is_struct():
         json_dict[node.name]["children"] = {}
```

### Comparing `vss-tools-4.1.dev5/vspec/vssexporters/vss2protobuf.py` & `vss-tools-4.1rc0/vspec/vssexporters/vss2protobuf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2021 Motius GmbH
+# Copyright (c) 2021 Contributors to COVESA
 #
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at https://mozilla.org/MPL/2.0/.
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
+# SPDX-License-Identifier: MPL-2.0
+
 # Convert vspec file to proto
 #
 
 import argparse
 import logging
 import os
 import sys
@@ -32,14 +34,19 @@
     "uint8": "uint32",
     "int8": "int32",
     "int16": "int32",
     "boolean": "bool"
 }
 
 
+def feature_supported(feature_name: str):
+    """Return true for supported optional arguments/features"""
+    return False
+
+
 def add_arguments(parser: argparse.ArgumentParser):
     parser.description = "The protobuf exporter does not support any additional arguments."
 
 
 class ProtoExporter(object):
     def __init__(self, out_dir: Path):
         self.out_files: Set[Path] = set()
```

### Comparing `vss-tools-4.1.dev5/vspec/vssexporters/vss2yaml.py` & `vss-tools-4.1rc0/vspec/vssexporters/vss2yaml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 #!/usr/bin/env python3
 
+# Copyright (c) 2016 Contributors to COVESA
 #
-# (c) 2021 Robert Bosch GmbH
-# (c) 2021 Pavel Sokolov (pavel.sokolov@gmail.com)
-# (c) 2016 Jaguar Land Rover
-#
-#
-# All files and artifacts in this repository are licensed under the
-# provisions of the license provided by the LICENSE file in this repository.
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
+# SPDX-License-Identifier: MPL-2.0
+
 #
 # Convert all vspec input files to a single flat YAML file.
 #
 
 
 import argparse
 from vspec.model.vsstree import VSSNode
 import yaml
 import logging
 from vspec.loggingconfig import initLogging
 from typing import Dict, Any
 
 
+def feature_supported(feature_name: str):
+    """Return true for supported arguments/features"""
+    if feature_name in ['no_expand']:
+        return True
+    return False
+
+
 def add_arguments(parser: argparse.ArgumentParser):
     parser.add_argument('--yaml-all-extended-attributes', action='store_true',
                         help=("Generate all extended attributes found in the model "
                               "(default is generating only those given by the "
                               "-e/--extended-attributes parameter)."))
 
 
@@ -71,14 +77,18 @@
         yaml_dict[node_path]["uuid"] = node.uuid
 
     for k, v in node.extended_attributes.items():
         if not config.yaml_all_extended_attributes and k not in VSSNode.whitelisted_extended_attributes:
             continue
         yaml_dict[node_path][k] = v
 
+    # Include instance information if we run tool in "no-expand" mode
+    if config.no_expand and node.instances is not None:
+        yaml_dict[node_path]["instances"] = node.instances
+
     for child in node.children:
         export_node(yaml_dict, child, config, print_uuid)
 
 
 def export_yaml(file_name, content_dict):
     with open(file_name, 'w') as f:
         yaml.dump(content_dict, f, default_flow_style=False, Dumper=NoAliasDumper,
```

### Comparing `vss-tools-4.1.dev5/vspec2x.py` & `vss-tools-4.1rc0/vspec2x.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
-# (c) 2022 BMW Group
-# (c) 2022 Robert Bosch GmbH
-# (c) 2016 Jaguar Land Rover
+# Copyright (c) 2016 Contributors to COVESA
 #
-# All files and artifacts in this repository are licensed under the
-# provisions of the license provided by the LICENSE file in this repository.
+# This program and the accompanying materials are made available under the
+# terms of the Mozilla Public License 2.0 which is available at
+# https://www.mozilla.org/en-US/MPL/2.0/
 #
+# SPDX-License-Identifier: MPL-2.0
+
 #
 # Convert vspec files to various other formats
 #
 
 from enum import Enum
 from vspec.model.vsstree import VSSNode
 from vspec.model.constants import VSSTreeType
@@ -18,17 +19,17 @@
 import argparse
 import logging
 import sys
 import vspec
 
 
 from vspec.vssexporters import vss2json, vss2csv, vss2yaml, \
-    vss2binary, vss2franca, vss2ddsidl, vss2graphql, vss2protobuf
+    vss2binary, vss2franca, vss2ddsidl, vss2graphql, vss2protobuf, vss2jsonschema, vss2id
 
-SUPPORTED_STRUCT_EXPORT_FORMATS = set(["json", "yaml", "csv", "protobuf"])
+SUPPORTED_STRUCT_EXPORT_FORMATS = set(["json", "yaml", "csv", "protobuf", "jsonschema", "idl"])
 
 
 class Exporter(Enum):
     """
     You can add new exporters here. Put the code in vssexporters and add it here
     See one of the existing exporters for an example.
     Mandatory functions are
@@ -40,29 +41,31 @@
     yaml = vss2yaml
     binary = vss2binary
     franca = vss2franca
     idl = vss2ddsidl
     graphql = vss2graphql
     protobuf = vss2protobuf
 
+    jsonschema = vss2jsonschema
+    idgen = vss2id
+
     def __str__(self):
         return self.name
 
     @staticmethod
     def from_string(s):
         try:
             return Exporter[s]
         except KeyError:
             raise ValueError()
 
 
-parser = argparse.ArgumentParser(description="Convert vspec to other formats.")
-
-
 def main(arguments):
+    parser = argparse.ArgumentParser(description="Convert vspec to other formats.")
+
     initLogging()
 
     parser.add_argument('-I', '--include-dir', action='append', metavar='dir', type=str, default=[],
                         help='Add include directory to search for included vspec files.')
     parser.add_argument('-e', '--extended-attributes', type=str, default="",
                         help='Whitelisted extended attributes as comma separated list. '
                              'Note, that not all exporters will support (all) extended attributes.')
@@ -75,34 +78,41 @@
                         help=" Terminate naming style not follows recommendations.")
     parser.add_argument('--format', metavar='format', type=Exporter.from_string, choices=list(Exporter),
                         help='Output format, choose one from ' +
                              str(Exporter._member_names_) +  # pylint: disable=no-member
                              ". If omitted we try to guess form output_file suffix.")
     parser.add_argument('--uuid', action='store_true',
                         help='Include uuid in generated files.')
+    parser.add_argument('--no-expand', action='store_true',
+                        help='Do not expand tree.')
     parser.add_argument('--no-uuid', action='store_true',
                         help='Exclude uuid in generated files.  This is currently the default behavior. ' +
                              ' This argument is deprecated and will be removed in VSS 5.0')
     parser.add_argument('-o', '--overlays', action='append', metavar='overlays', type=str, default=[],
                         help='Add overlay that will be layered on top of the VSS file in the order they appear.')
     parser.add_argument('-u', '--unit-file', action='append', metavar='unit_file', type=str, default=[],
                         help='Unit file to be used for generation. Argument -u may be used multiple times.')
+    parser.add_argument('-q', '--quantity-file', action='append', metavar='quantity_file', type=str, default=[],
+                        help='Quantity file to be used for generation. Argument -uqmay be used multiple times.')
     parser.add_argument('vspec_file', metavar='<vspec_file>',
                         help='The vehicle specification file to convert.')
     parser.add_argument('output_file', metavar='<output_file>',
                         help='The file to write output to.')
 
     type_group = parser.add_argument_group(
         'VSS Data Type Tree arguments',
         'Arguments related to struct/type support')
     type_group.add_argument('-vt', '--vspec-types-file', action='append', metavar='vspec_types_file', type=str,
                             default=[],
                             help='Data types file in vspec format.')
     type_group.add_argument('-ot', '--types-output-file', metavar='<types_output_file>',
-                            help='Output file for writing data types from vspec file.')
+                            help='Output file for writing data types from vspec file. ' +
+                                 'If not specified, a single file is used where applicable. ' +
+                                 'In case of JSON and YAML, the data is exported under a ' +
+                                 'special key - "ComplexDataTypes"')
 
     for entry in Exporter:
         entry.value.add_arguments(parser.add_argument_group(
             f"{entry.name.upper()} arguments", ""))
 
     args = parser.parse_args(arguments)
 
@@ -149,16 +159,21 @@
         sys.exit(-1)
     if args.no_uuid:
         logging.warning("The argument --no-uuid is deprecated and will be removed in VSS 5.0")
     print_uuid = False
     if args.uuid:
         print_uuid = True
 
+    vspec.load_quantities(args.vspec_file, args.quantity_file)
     vspec.load_units(args.vspec_file, args.unit_file)
 
+    # Warn if unsupported feature is used
+    if args.no_expand and not exporter.feature_supported("no_expand"):
+        logging.warning("--no_expand not supported by exporter")
+
     # process data type tree
     if args.types_output_file is not None and not args.vspec_types_file:
         parser.error("An output file for data types was provided. Please also provide "
                      "the input vspec file for data types")
     data_type_tree = None
     if args.vspec_types_file:
         data_type_tree = processDataTypeTree(
@@ -176,15 +191,16 @@
             logging.info(f"Applying VSS overlay from {overlay}...")
             othertree = vspec.load_tree(overlay, include_dirs, VSSTreeType.SIGNAL_TREE,
                                         break_on_name_style_violation=abort_on_namestyle, expand_inst=False,
                                         data_type_tree=data_type_tree)
             vspec.merge_tree(tree, othertree)
 
         vspec.check_type_usage(tree, VSSTreeType.SIGNAL_TREE, data_type_tree)
-        vspec.expand_tree_instances(tree)
+        if not args.no_expand:
+            vspec.expand_tree_instances(tree)
 
         vspec.clean_metadata(tree)
         vspec.verify_mandatory_attributes(tree, abort_on_unknown_attribute)
         logging.info("Calling exporter...")
 
         # temporary until all exporters support data type tree
         if args.format.name in SUPPORTED_STRUCT_EXPORT_FORMATS:
```

