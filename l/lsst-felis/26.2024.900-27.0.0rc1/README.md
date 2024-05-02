# Comparing `tmp/lsst-felis-26.2024.900.tar.gz` & `tmp/lsst_felis-27.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-felis-26.2024.900.tar", last modified: Thu Feb 29 10:20:00 2024, max compression
+gzip compressed data, was "lsst_felis-27.0.0rc1.tar", last modified: Wed May  1 21:15:44 2024, max compression
```

## Comparing `lsst-felis-26.2024.900.tar` & `lsst_felis-27.0.0rc1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.968162 lsst-felis-26.2024.900/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-29 10:20:00.968162 lsst-felis-26.2024.900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.960162 lsst-felis-26.2024.900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.964162 lsst-felis-26.2024.900/python/felis/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/datamodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.964162 lsst-felis-26.2024.900/python/felis/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/db/sqltypes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    17704 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/tap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/felis/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.968162 lsst-felis-26.2024.900/python/lsst_felis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-29 10:20:00.968162 lsst-felis-26.2024.900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.964162 lsst-felis-26.2024.900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19080 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_tap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:44.745215 lsst_felis-27.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-01 21:15:44.745215 lsst_felis-27.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:44.737215 lsst_felis-27.0.0rc1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:44.741215 lsst_felis-27.0.0rc1/python/felis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17041 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/datamodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:44.741215 lsst_felis-27.0.0rc1/python/felis/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/db/_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/db/sqltypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18542 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17704 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/tap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:15:44.000000 lsst_felis-27.0.0rc1/python/felis/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/python/felis/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:44.741215 lsst_felis-27.0.0rc1/python/lsst_felis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-01 21:15:44.000000 lsst_felis-27.0.0rc1/python/lsst_felis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-01 21:15:44.000000 lsst_felis-27.0.0rc1/python/lsst_felis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:15:44.000000 lsst_felis-27.0.0rc1/python/lsst_felis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 21:15:44.000000 lsst_felis-27.0.0rc1/python/lsst_felis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 21:15:44.000000 lsst_felis-27.0.0rc1/python/lsst_felis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 21:15:44.000000 lsst_felis-27.0.0rc1/python/lsst_felis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:15:44.000000 lsst_felis-27.0.0rc1/python/lsst_felis.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-01 21:15:44.745215 lsst_felis-27.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:44.741215 lsst_felis-27.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19713 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/tests/test_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/tests/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/tests/test_tap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-01 21:15:38.000000 lsst_felis-27.0.0rc1/tests/test_validation.py
```

### Comparing `lsst-felis-26.2024.900/LICENSE` & `lsst_felis-27.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/PKG-INFO` & `lsst_felis-27.0.0rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-felis
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: A vocabulary for describing catalogs and acting on those descriptions
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/lsst/felis
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -19,9 +19,10 @@
 License-File: LICENSE
 Requires-Dist: astropy>=4
 Requires-Dist: sqlalchemy>=1.4
 Requires-Dist: click>=7
 Requires-Dist: pyyaml>=6
 Requires-Dist: pyld>=2
 Requires-Dist: pydantic<3,>=2
+Requires-Dist: lsst-utils
 Provides-Extra: test
 Requires-Dist: pytest>=3.2; extra == "test"
```

### Comparing `lsst-felis-26.2024.900/README.rst` & `lsst_felis-27.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/pyproject.toml` & `lsst_felis-27.0.0rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 keywords = ["lsst"]
 dependencies = [
     "astropy >= 4",
     "sqlalchemy >= 1.4",
     "click >= 7",
     "pyyaml >= 6",
     "pyld >= 2",
-    "pydantic >= 2, < 3"
+    "pydantic >= 2, < 3",
+    "lsst-utils"
 ]
 requires-python = ">=3.11.0"
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/lsst/felis"
 
@@ -143,7 +144,17 @@
 ]
 target-version = "py311"
 # Commented out to suppress "unused noqa" in jenkins which has older ruff not
 # generating E721.
 extend-select = [
     "RUF100", # Warn about unused noqa
 ]
+
+[tool.pydeps]
+max_bacon = 2
+no_show = true
+verbose = 0
+pylib = false
+format = "png"
+exclude = [
+    "sqlalchemy"
+]
```

### Comparing `lsst-felis-26.2024.900/python/felis/__init__.py` & `lsst_felis-27.0.0rc1/python/felis/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/python/felis/check.py` & `lsst_felis-27.0.0rc1/python/felis/check.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/python/felis/cli.py` & `lsst_felis-27.0.0rc1/python/felis/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,62 +22,123 @@
 from __future__ import annotations
 
 import io
 import json
 import logging
 import sys
 from collections.abc import Iterable, Mapping, MutableMapping
-from typing import Any
+from typing import IO, Any
 
 import click
 import yaml
 from pydantic import ValidationError
 from pyld import jsonld
 from sqlalchemy.engine import Engine, create_engine, create_mock_engine, make_url
 from sqlalchemy.engine.mock import MockConnection
 
 from . import DEFAULT_CONTEXT, DEFAULT_FRAME, __version__
 from .check import CheckingVisitor
 from .datamodel import Schema
-from .sql import SQLVisitor
+from .metadata import DatabaseContext, InsertDump, MetaDataBuilder
 from .tap import Tap11Base, TapLoadingVisitor, init_tables
 from .utils import ReorderingVisitor
 from .validation import get_schema
 
 logger = logging.getLogger("felis")
 
+loglevel_choices = ["CRITICAL", "FATAL", "ERROR", "WARNING", "INFO", "DEBUG"]
+
 
 @click.group()
 @click.version_option(__version__)
-def cli() -> None:
+@click.option(
+    "--log-level",
+    type=click.Choice(loglevel_choices),
+    envvar="FELIS_LOGLEVEL",
+    help="Felis log level",
+    default=logging.getLevelName(logging.INFO),
+)
+@click.option(
+    "--log-file",
+    type=click.Path(),
+    envvar="FELIS_LOGFILE",
+    help="Felis log file path",
+)
+def cli(log_level: str, log_file: str | None) -> None:
     """Felis Command Line Tools."""
-    logging.basicConfig(level=logging.INFO)
+    if log_file:
+        logging.basicConfig(filename=log_file, level=log_level)
+    else:
+        logging.basicConfig(level=log_level)
 
 
-@cli.command("create-all")
-@click.option("--engine-url", envvar="ENGINE_URL", help="SQLAlchemy Engine URL")
-@click.option("--schema-name", help="Alternate Schema Name for Felis File")
-@click.option("--dry-run", is_flag=True, help="Dry Run Only. Prints out the DDL that would be executed")
+@cli.command("create")
+@click.option("--engine-url", envvar="ENGINE_URL", help="SQLAlchemy Engine URL", default="sqlite://")
+@click.option("--schema-name", help="Alternate schema name to override Felis file")
+@click.option(
+    "--create-if-not-exists", is_flag=True, help="Create the schema in the database if it does not exist"
+)
+@click.option("--drop-if-exists", is_flag=True, help="Drop schema if it already exists in the database")
+@click.option("--echo", is_flag=True, help="Echo database commands as they are executed")
+@click.option("--dry-run", is_flag=True, help="Dry run only to print out commands instead of executing")
+@click.option(
+    "--output-file", "-o", type=click.File(mode="w"), help="Write SQL commands to a file instead of executing"
+)
 @click.argument("file", type=click.File())
-def create_all(engine_url: str, schema_name: str, dry_run: bool, file: io.TextIOBase) -> None:
-    """Create schema objects from the Felis FILE."""
-    schema_obj = yaml.load(file, Loader=yaml.SafeLoader)
-    visitor = SQLVisitor(schema_name=schema_name)
-    schema = visitor.visit_schema(schema_obj)
-
-    metadata = schema.metadata
+def create(
+    engine_url: str,
+    schema_name: str | None,
+    create_if_not_exists: bool,
+    drop_if_exists: bool,
+    echo: bool,
+    dry_run: bool,
+    output_file: IO[str] | None,
+    file: IO,
+) -> None:
+    """Create database objects from the Felis file."""
+    yaml_data = yaml.safe_load(file)
+    schema = Schema.model_validate(yaml_data)
+    url_obj = make_url(engine_url)
+    if schema_name:
+        logger.info(f"Overriding schema name with: {schema_name}")
+        schema.name = schema_name
+    elif url_obj.drivername == "sqlite":
+        logger.info("Overriding schema name for sqlite with: main")
+        schema.name = "main"
+    if not url_obj.host and not url_obj.drivername == "sqlite":
+        dry_run = True
+        logger.info("Forcing dry run for non-sqlite engine URL with no host")
+
+    builder = MetaDataBuilder(schema)
+    builder.build()
+    metadata = builder.metadata
+    logger.debug(f"Created metadata with schema name: {metadata.schema}")
 
     engine: Engine | MockConnection
-    if not dry_run:
-        engine = create_engine(engine_url)
+    if not dry_run and not output_file:
+        engine = create_engine(engine_url, echo=echo)
     else:
-        _insert_dump = InsertDump()
-        engine = create_mock_engine(make_url(engine_url), executor=_insert_dump.dump)
-        _insert_dump.dialect = engine.dialect
-    metadata.create_all(engine)
+        if dry_run:
+            logger.info("Dry run will be executed")
+        engine = DatabaseContext.create_mock_engine(url_obj, output_file)
+        if output_file:
+            logger.info("Writing SQL output to: " + output_file.name)
+
+    context = DatabaseContext(metadata, engine)
+
+    if drop_if_exists:
+        logger.debug("Dropping schema if it exists")
+        context.drop_if_exists()
+        create_if_not_exists = True  # If schema is dropped, it needs to be recreated.
+
+    if create_if_not_exists:
+        logger.debug("Creating schema if not exists")
+        context.create_if_not_exists()
+
+    context.create_all()
 
 
 @cli.command("init-tap")
 @click.option("--tap-schema-name", help="Alt Schema Name for TAP_SCHEMA")
 @click.option("--tap-schemas-table", help="Alt Table Name for TAP_SCHEMA.schemas")
 @click.option("--tap-tables-table", help="Alt Table Name for TAP_SCHEMA.tables")
 @click.option("--tap-columns-table", help="Alt Table Name for TAP_SCHEMA.columns")
@@ -308,30 +369,45 @@
 @click.option(
     "-s",
     "--schema-name",
     help="Schema name for validation",
     type=click.Choice(["RSP", "default"]),
     default="default",
 )
-@click.option("-d", "--require-description", is_flag=True, help="Require description for all objects")
+@click.option(
+    "-d", "--require-description", is_flag=True, help="Require description for all objects", default=False
+)
+@click.option(
+    "-t", "--check-redundant-datatypes", is_flag=True, help="Check for redundant datatypes", default=False
+)
 @click.argument("files", nargs=-1, type=click.File())
-def validate(schema_name: str, require_description: bool, files: Iterable[io.TextIOBase]) -> None:
+def validate(
+    schema_name: str,
+    require_description: bool,
+    check_redundant_datatypes: bool,
+    files: Iterable[io.TextIOBase],
+) -> None:
     """Validate one or more felis YAML files."""
     schema_class = get_schema(schema_name)
-    logger.info(f"Using schema '{schema_class.__name__}'")
-
-    if require_description:
-        Schema.require_description(True)
+    if schema_name != "default":
+        logger.info(f"Using schema '{schema_class.__name__}'")
 
     rc = 0
     for file in files:
         file_name = getattr(file, "name", None)
         logger.info(f"Validating {file_name}")
         try:
-            schema_class.model_validate(yaml.load(file, Loader=yaml.SafeLoader))
+            data = yaml.load(file, Loader=yaml.SafeLoader)
+            schema_class.model_validate(
+                data,
+                context={
+                    "check_redundant_datatypes": check_redundant_datatypes,
+                    "require_description": require_description,
+                },
+            )
         except ValidationError as e:
             logger.error(e)
             rc = 1
     if rc:
         raise click.exceptions.Exit(rc)
 
 
@@ -382,34 +458,9 @@
     compacted = jsonld.compact(framed, DEFAULT_CONTEXT, options=dict(graph=True))
     graph = compacted["@graph"]
     graph = [ReorderingVisitor(add_type=True).visit_schema(schema_obj) for schema_obj in graph]
     compacted["@graph"] = graph if len(graph) > 1 else graph[0]
     return compacted
 
 
-class InsertDump:
-    """An Insert Dumper for SQL statements."""
-
-    dialect: Any = None
-
-    def dump(self, sql: Any, *multiparams: Any, **params: Any) -> None:
-        compiled = sql.compile(dialect=self.dialect)
-        sql_str = str(compiled) + ";"
-        params_list = [compiled.params]
-        for params in params_list:
-            if not params:
-                print(sql_str)
-                continue
-            new_params = {}
-            for key, value in params.items():
-                if isinstance(value, str):
-                    new_params[key] = f"'{value}'"
-                elif value is None:
-                    new_params[key] = "null"
-                else:
-                    new_params[key] = value
-
-            print(sql_str % new_params)
-
-
 if __name__ == "__main__":
     cli()
```

### Comparing `lsst-felis-26.2024.900/python/felis/datamodel.py` & `lsst_felis-27.0.0rc1/python/felis/datamodel.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,24 +18,32 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 import logging
+import re
 from collections.abc import Mapping, Sequence
-from enum import Enum
+from enum import StrEnum, auto
 from typing import Annotated, Any, Literal, TypeAlias
 
 from astropy import units as units  # type: ignore
 from astropy.io.votable import ucd  # type: ignore
-from pydantic import BaseModel, ConfigDict, Field, field_validator, model_validator
+from pydantic import BaseModel, ConfigDict, Field, ValidationInfo, field_validator, model_validator
+from sqlalchemy import dialects
+from sqlalchemy import types as sqa_types
+from sqlalchemy.engine import create_mock_engine
+from sqlalchemy.engine.interfaces import Dialect
+from sqlalchemy.types import TypeEngine
+
+from .db.sqltypes import get_type_func
+from .types import FelisType
 
 logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
 
 __all__ = (
     "BaseObject",
     "Column",
     "CheckConstraint",
     "Constraint",
     "DescriptionStr",
@@ -46,16 +54,14 @@
     "Table",
     "UniqueConstraint",
 )
 
 CONFIG = ConfigDict(
     populate_by_name=True,  # Populate attributes by name.
     extra="forbid",  # Do not allow extra fields.
-    use_enum_values=True,  # Use enum values instead of names.
-    validate_assignment=True,  # Validate assignments after model is created.
     str_strip_whitespace=True,  # Strip whitespace from string fields.
 )
 """Pydantic model configuration as described in:
 https://docs.pydantic.dev/2.0/api/config/#pydantic.config.ConfigDict
 """
 
 DESCR_MIN_LENGTH = 3
@@ -81,71 +87,122 @@
     id: str = Field(alias="@id")
     """The unique identifier of the database object.
 
     All Felis database objects must have a unique identifier.
     """
 
     description: DescriptionStr | None = None
-    """A description of the database object.
-
-    By default, the description is optional but will be required if
-    `BaseObject.Config.require_description` is set to `True` by the user.
-    """
+    """A description of the database object."""
 
-    @model_validator(mode="before")
+    @model_validator(mode="after")  # type: ignore[arg-type]
     @classmethod
-    def check_description(cls, values: dict[str, Any]) -> dict[str, Any]:
+    def check_description(cls, object: BaseObject, info: ValidationInfo) -> BaseObject:
         """Check that the description is present if required."""
-        if Schema.is_description_required():
-            if "description" not in values or not values["description"]:
-                raise ValueError("Description is required and must be non-empty")
-            if len(values["description"].strip()) < DESCR_MIN_LENGTH:
-                raise ValueError(f"Description must be at least {DESCR_MIN_LENGTH} characters long")
-        return values
+        context = info.context
+        if not context or not context.get("require_description", False):
+            return object
+        if object.description is None or object.description == "":
+            raise ValueError("Description is required and must be non-empty")
+        if len(object.description) < DESCR_MIN_LENGTH:
+            raise ValueError(f"Description must be at least {DESCR_MIN_LENGTH} characters long")
+        return object
 
 
-class DataType(Enum):
+class DataType(StrEnum):
     """`Enum` representing the data types supported by Felis."""
 
-    BOOLEAN = "boolean"
-    BYTE = "byte"
-    SHORT = "short"
-    INT = "int"
-    LONG = "long"
-    FLOAT = "float"
-    DOUBLE = "double"
-    CHAR = "char"
-    STRING = "string"
-    UNICODE = "unicode"
-    TEXT = "text"
-    BINARY = "binary"
-    TIMESTAMP = "timestamp"
+    boolean = auto()
+    byte = auto()
+    short = auto()
+    int = auto()
+    long = auto()
+    float = auto()
+    double = auto()
+    char = auto()
+    string = auto()
+    unicode = auto()
+    text = auto()
+    binary = auto()
+    timestamp = auto()
+
+
+_DIALECTS = {
+    "mysql": create_mock_engine("mysql://", executor=None).dialect,
+    "postgresql": create_mock_engine("postgresql://", executor=None).dialect,
+}
+"""Dictionary of dialect names to SQLAlchemy dialects."""
+
+_DIALECT_MODULES = {"mysql": getattr(dialects, "mysql"), "postgresql": getattr(dialects, "postgresql")}
+"""Dictionary of dialect names to SQLAlchemy dialect modules."""
+
+_DATATYPE_REGEXP = re.compile(r"(\w+)(\((.*)\))?")
+"""Regular expression to match data types in the form "type(length)"""
+
+
+def string_to_typeengine(
+    type_string: str, dialect: Dialect | None = None, length: int | None = None
+) -> TypeEngine:
+    match = _DATATYPE_REGEXP.search(type_string)
+    if not match:
+        raise ValueError(f"Invalid type string: {type_string}")
+
+    type_name, _, params = match.groups()
+    if dialect is None:
+        type_class = getattr(sqa_types, type_name.upper(), None)
+    else:
+        try:
+            dialect_module = _DIALECT_MODULES[dialect.name]
+        except KeyError:
+            raise ValueError(f"Unsupported dialect: {dialect}")
+        type_class = getattr(dialect_module, type_name.upper(), None)
+
+    if not type_class:
+        raise ValueError(f"Unsupported type: {type_class}")
+
+    if params:
+        params = [int(param) if param.isdigit() else param for param in params.split(",")]
+        type_obj = type_class(*params)
+    else:
+        type_obj = type_class()
+
+    if hasattr(type_obj, "length") and getattr(type_obj, "length") is None and length is not None:
+        type_obj.length = length
+
+    return type_obj
 
 
 class Column(BaseObject):
     """A column in a table."""
 
     datatype: DataType
     """The datatype of the column."""
 
     length: int | None = None
     """The length of the column."""
 
-    nullable: bool = True
-    """Whether the column can be `NULL`."""
+    nullable: bool | None = None
+    """Whether the column can be ``NULL``.
+
+    If `None`, this value was not set explicitly in the YAML data. In this
+    case, it will be set to `False` for columns with numeric types and `True`
+    otherwise.
+    """
 
     value: Any = None
     """The default value of the column."""
 
     autoincrement: bool | None = None
     """Whether the column is autoincremented."""
 
     mysql_datatype: str | None = Field(None, alias="mysql:datatype")
     """The MySQL datatype of the column."""
 
+    postgresql_datatype: str | None = Field(None, alias="postgresql:datatype")
+    """The PostgreSQL datatype of the column."""
+
     ivoa_ucd: str | None = Field(None, alias="ivoa:ucd")
     """The IVOA UCD of the column."""
 
     fits_tunit: str | None = Field(None, alias="fits:tunit")
     """The FITS TUNIT of the column."""
 
     ivoa_unit: str | None = Field(None, alias="ivoa:unit")
@@ -197,14 +254,61 @@
             try:
                 units.Unit(unit)
             except ValueError as e:
                 raise ValueError(f"Invalid unit: {e}")
 
         return values
 
+    @model_validator(mode="after")  # type: ignore[arg-type]
+    @classmethod
+    def validate_datatypes(cls, col: Column, info: ValidationInfo) -> Column:
+        """Check for redundant datatypes on columns."""
+        context = info.context
+        if not context or not context.get("check_redundant_datatypes", False):
+            return col
+        if all(getattr(col, f"{dialect}:datatype", None) is not None for dialect in _DIALECTS.keys()):
+            return col
+
+        datatype = col.datatype
+        length: int | None = col.length or None
+
+        datatype_func = get_type_func(datatype)
+        felis_type = FelisType.felis_type(datatype)
+        if felis_type.is_sized:
+            if length is not None:
+                datatype_obj = datatype_func(length)
+            else:
+                raise ValueError(f"Length must be provided for sized type '{datatype}' in column '{col.id}'")
+        else:
+            datatype_obj = datatype_func()
+
+        for dialect_name, dialect in _DIALECTS.items():
+            db_annotation = f"{dialect_name}_datatype"
+            if datatype_string := col.model_dump().get(db_annotation):
+                db_datatype_obj = string_to_typeengine(datatype_string, dialect, length)
+                if datatype_obj.compile(dialect) == db_datatype_obj.compile(dialect):
+                    raise ValueError(
+                        "'{}: {}' is the same as 'datatype: {}' in column '{}'".format(
+                            db_annotation, datatype_string, col.datatype, col.id
+                        )
+                    )
+                else:
+                    logger.debug(
+                        "Valid type override of 'datatype: {}' with '{}: {}' in column '{}'".format(
+                            col.datatype, db_annotation, datatype_string, col.id
+                        )
+                    )
+                    logger.debug(
+                        "Compiled datatype '{}' with {} compiled override '{}'".format(
+                            datatype_obj.compile(dialect), dialect_name, db_datatype_obj.compile(dialect)
+                        )
+                    )
+
+        return col
+
 
 class Constraint(BaseObject):
     """A database table constraint."""
 
     deferrable: bool = False
     """If `True` then this constraint will be declared as deferrable."""
 
@@ -276,15 +380,15 @@
 
     constraints: list[Constraint] = Field(default_factory=list)
     """The constraints on the table."""
 
     indexes: list[Index] = Field(default_factory=list)
     """The indexes on the table."""
 
-    primaryKey: str | list[str] | None = None
+    primary_key: str | list[str] | None = Field(None, alias="primaryKey")
     """The primary key of the table."""
 
     tap_table_index: int | None = Field(None, alias="tap:table_index")
     """The IVOA TAP_SCHEMA table index of the table."""
 
     mysql_engine: str | None = Field(None, alias="mysql:engine")
     """The mysql engine to use for the table.
@@ -394,23 +498,14 @@
         """Visit a constraint object."""
         self.add(constraint)
 
 
 class Schema(BaseObject):
     """The database schema containing the tables."""
 
-    class ValidationConfig:
-        """Validation configuration which is specific to Felis."""
-
-        _require_description = False
-        """Flag to require a description for all objects.
-
-        This is set by the `require_description` class method.
-        """
-
     version: SchemaVersion | str | None = None
     """The version of the schema."""
 
     tables: Sequence[Table]
     """The tables in the schema."""
 
     id_map: dict[str, Any] = Field(default_factory=dict, exclude=True)
@@ -420,45 +515,39 @@
     @classmethod
     def check_unique_table_names(cls, tables: list[Table]) -> list[Table]:
         """Check that table names are unique."""
         if len(tables) != len(set(table.name for table in tables)):
             raise ValueError("Table names must be unique")
         return tables
 
-    @model_validator(mode="after")
-    def create_id_map(self: Schema) -> Schema:
-        """Create a map of IDs to objects."""
+    def _create_id_map(self: Schema) -> Schema:
+        """Create a map of IDs to objects.
+
+        This method should not be called by users. It is called automatically
+        by the ``model_post_init()`` method. If the ID map is already
+        populated, this method will return immediately.
+        """
+        if len(self.id_map):
+            logger.debug("Ignoring call to create_id_map() - ID map was already populated")
+            return self
         visitor: SchemaIdVisitor = SchemaIdVisitor()
         visitor.visit_schema(self)
-        logger.debug(f"ID map contains {len(self.id_map.keys())} objects")
+        logger.debug(f"Created schema ID map with {len(self.id_map.keys())} objects")
         if len(visitor.duplicates):
             raise ValueError(
                 "Duplicate IDs found in schema:\n    " + "\n    ".join(visitor.duplicates) + "\n"
             )
         return self
 
+    def model_post_init(self, ctx: Any) -> None:
+        """Post-initialization hook for the model."""
+        self._create_id_map()
+
     def __getitem__(self, id: str) -> BaseObject:
         """Get an object by its ID."""
         if id not in self:
             raise KeyError(f"Object with ID '{id}' not found in schema")
         return self.id_map[id]
 
     def __contains__(self, id: str) -> bool:
         """Check if an object with the given ID is in the schema."""
         return id in self.id_map
-
-    @classmethod
-    def require_description(cls, rd: bool = True) -> None:
-        """Set whether a description is required for all objects.
-
-        This includes the schema, tables, columns, and constraints.
-
-        Users should call this method to set the requirement for a description
-        when validating schemas, rather than change the flag value directly.
-        """
-        logger.debug(f"Setting description requirement to '{rd}'")
-        cls.ValidationConfig._require_description = rd
-
-    @classmethod
-    def is_description_required(cls) -> bool:
-        """Return whether a description is required for all objects."""
-        return cls.ValidationConfig._require_description
```

### Comparing `lsst-felis-26.2024.900/python/felis/db/sqltypes.py` & `lsst_felis-27.0.0rc1/python/felis/db/sqltypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import builtins
 from collections.abc import Mapping
-from typing import Any
+from typing import Any, Callable
 
-from sqlalchemy import Float, SmallInteger, types
+from sqlalchemy import SmallInteger, types
 from sqlalchemy.dialects import mysql, oracle, postgresql
 from sqlalchemy.ext.compiler import compiles
 
 MYSQL = "mysql"
 ORACLE = "oracle"
 POSTGRES = "postgresql"
 SQLITE = "sqlite"
@@ -35,32 +35,20 @@
 
 class TINYINT(SmallInteger):
     """The non-standard TINYINT type."""
 
     __visit_name__ = "TINYINT"
 
 
-class DOUBLE(Float):
-    """The non-standard DOUBLE type."""
-
-    __visit_name__ = "DOUBLE"
-
-
 @compiles(TINYINT)
 def compile_tinyint(type_: Any, compiler: Any, **kw: Any) -> str:
     """Return type name for TINYINT."""
     return "TINYINT"
 
 
-@compiles(DOUBLE)
-def compile_double(type_: Any, compiler: Any, **kw: Any) -> str:
-    """Return type name for double precision type."""
-    return "DOUBLE"
-
-
 _TypeMap = Mapping[str, types.TypeEngine | type[types.TypeEngine]]
 
 boolean_map: _TypeMap = {MYSQL: mysql.BIT(1), ORACLE: oracle.NUMBER(1), POSTGRES: postgresql.BOOLEAN()}
 
 byte_map: _TypeMap = {
     MYSQL: mysql.TINYINT(),
     ORACLE: oracle.NUMBER(3),
@@ -156,15 +144,15 @@
 def float(**kwargs: Any) -> types.TypeEngine:
     """Return SQLAlchemy type for single precision float."""
     return _vary(types.FLOAT(), float_map, kwargs)
 
 
 def double(**kwargs: Any) -> types.TypeEngine:
     """Return SQLAlchemy type for double precision float."""
-    return _vary(DOUBLE(), double_map, kwargs)
+    return _vary(types.DOUBLE(), double_map, kwargs)
 
 
 def char(length: builtins.int, **kwargs: Any) -> types.TypeEngine:
     """Return SQLAlchemy type for character."""
     return _vary(types.CHAR(length), char_map, kwargs, length)
 
 
@@ -174,36 +162,43 @@
 
 
 def unicode(length: builtins.int, **kwargs: Any) -> types.TypeEngine:
     """Return SQLAlchemy type for unicode string."""
     return _vary(types.NVARCHAR(length), unicode_map, kwargs, length)
 
 
-def text(length: builtins.int, **kwargs: Any) -> types.TypeEngine:
+def text(**kwargs: Any) -> types.TypeEngine:
     """Return SQLAlchemy type for text."""
-    return _vary(types.CLOB(length), text_map, kwargs, length)
+    return _vary(types.TEXT(), text_map, kwargs)
 
 
 def binary(length: builtins.int, **kwargs: Any) -> types.TypeEngine:
     """Return SQLAlchemy type for binary."""
     return _vary(types.BLOB(length), binary_map, kwargs, length)
 
 
 def timestamp(**kwargs: Any) -> types.TypeEngine:
     """Return SQLAlchemy type for timestamp."""
     return types.TIMESTAMP()
 
 
+def get_type_func(type_name: str) -> Callable:
+    """Return the function for the type with the given name."""
+    if type_name not in globals():
+        raise ValueError(f"Unknown type: {type_name}")
+    return globals()[type_name]
+
+
 def _vary(
     type_: types.TypeEngine,
     variant_map: _TypeMap,
     overrides: _TypeMap,
     *args: Any,
 ) -> types.TypeEngine:
     variants: dict[str, types.TypeEngine | type[types.TypeEngine]] = dict(variant_map)
     variants.update(overrides)
     for dialect, variant in variants.items():
         # If this is a class and not an instance, instantiate
-        if isinstance(variant, type):
+        if callable(variant):
             variant = variant(*args)
         type_ = type_.with_variant(variant, dialect)
     return type_
```

### Comparing `lsst-felis-26.2024.900/python/felis/simple.py` & `lsst_felis-27.0.0rc1/python/felis/simple.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/python/felis/tap.py` & `lsst_felis-27.0.0rc1/python/felis/tap.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/python/felis/types.py` & `lsst_felis-27.0.0rc1/python/felis/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     """Felis definition of string type."""
 
 
 class Unicode(FelisType, felis_name="unicode", votable_name="unicodeChar", is_sized=True):
     """Felis definition of unicode string type."""
 
 
-class Text(FelisType, felis_name="text", votable_name="unicodeChar", is_sized=True):
+class Text(FelisType, felis_name="text", votable_name="char"):
     """Felis definition of text type."""
 
 
 class Binary(FelisType, felis_name="binary", votable_name="unsignedByte", is_sized=True):
     """Felis definition of binary type."""
```

### Comparing `lsst-felis-26.2024.900/python/felis/utils.py` & `lsst_felis-27.0.0rc1/python/felis/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/python/felis/validation.py` & `lsst_felis-27.0.0rc1/python/felis/validation.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/python/felis/visitor.py` & `lsst_felis-27.0.0rc1/python/felis/visitor.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/python/lsst_felis.egg-info/PKG-INFO` & `lsst_felis-27.0.0rc1/python/lsst_felis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-felis
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: A vocabulary for describing catalogs and acting on those descriptions
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/lsst/felis
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -19,9 +19,10 @@
 License-File: LICENSE
 Requires-Dist: astropy>=4
 Requires-Dist: sqlalchemy>=1.4
 Requires-Dist: click>=7
 Requires-Dist: pyyaml>=6
 Requires-Dist: pyld>=2
 Requires-Dist: pydantic<3,>=2
+Requires-Dist: lsst-utils
 Provides-Extra: test
 Requires-Dist: pytest>=3.2; extra == "test"
```

### Comparing `lsst-felis-26.2024.900/python/lsst_felis.egg-info/SOURCES.txt` & `lsst_felis-27.0.0rc1/python/lsst_felis.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,35 @@
 README.rst
 pyproject.toml
 setup.cfg
 python/felis/__init__.py
 python/felis/check.py
 python/felis/cli.py
 python/felis/datamodel.py
+python/felis/metadata.py
 python/felis/py.typed
 python/felis/simple.py
-python/felis/sql.py
 python/felis/tap.py
 python/felis/types.py
 python/felis/utils.py
 python/felis/validation.py
 python/felis/version.py
 python/felis/visitor.py
 python/felis/db/__init__.py
+python/felis/db/_variants.py
 python/felis/db/sqltypes.py
 python/lsst_felis.egg-info/PKG-INFO
 python/lsst_felis.egg-info/SOURCES.txt
 python/lsst_felis.egg-info/dependency_links.txt
 python/lsst_felis.egg-info/entry_points.txt
 python/lsst_felis.egg-info/requires.txt
 python/lsst_felis.egg-info/top_level.txt
 python/lsst_felis.egg-info/zip-safe
 tests/test_check.py
 tests/test_cli.py
 tests/test_datamodel.py
+tests/test_datatypes.py
+tests/test_metadata.py
 tests/test_simple.py
-tests/test_sql.py
 tests/test_tap.py
 tests/test_utils.py
 tests/test_validation.py
```

### Comparing `lsst-felis-26.2024.900/tests/test_check.py` & `lsst_felis-27.0.0rc1/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/tests/test_cli.py` & `lsst_felis-27.0.0rc1/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import unittest
 from collections.abc import MutableMapping
 from typing import Any
 
 from click.testing import CliRunner
 
 from felis.cli import cli
-from felis.datamodel import Schema
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
 TEST_YAML = os.path.join(TESTDIR, "data", "test.yml")
 TEST_MERGE_YAML = os.path.join(TESTDIR, "data", "test-merge.yml")
 
 
 class CliTestCase(unittest.TestCase):
@@ -50,33 +49,33 @@
     def test_basic_check(self) -> None:
         """Test for basic-check command."""
         runner = CliRunner()
         result = runner.invoke(cli, ["basic-check", TEST_YAML], catch_exceptions=False)
         self.assertEqual(result.exit_code, 0)
 
     def test_create_all(self) -> None:
-        """Test for create-all command."""
+        """Test for create command."""
         url = f"sqlite:///{self.tmpdir}/tap.sqlite3"
 
         runner = CliRunner()
         result = runner.invoke(
             cli,
-            ["create-all", "--schema-name=main", f"--engine-url={url}", TEST_YAML],
+            ["create", "--schema-name=main", f"--engine-url={url}", TEST_YAML],
             catch_exceptions=False,
         )
         self.assertEqual(result.exit_code, 0)
 
     def test_create_all_dry_run(self) -> None:
-        """Test for create-all --dry-run command."""
+        """Test for create --dry-run command."""
         url = f"sqlite:///{self.tmpdir}/tap.sqlite3"
 
         runner = CliRunner()
         result = runner.invoke(
             cli,
-            ["create-all", "--schema-name=main", f"--engine-url={url}", "--dry-run", TEST_YAML],
+            ["create", "--schema-name=main", f"--engine-url={url}", "--dry-run", TEST_YAML],
             catch_exceptions=False,
         )
         self.assertEqual(result.exit_code, 0)
 
     def test_normalize(self) -> None:
         """Test for normalize command."""
         runner = CliRunner()
@@ -141,17 +140,14 @@
             # Wrap this in a try/catch in case an exception is thrown.
             result = runner.invoke(
                 cli, ["validate", "--require-description", TEST_YAML], catch_exceptions=False
             )
         except Exception as e:
             # Reraise exception.
             raise e
-        finally:
-            # Turn the flag off so it does not effect subsequent tests.
-            Schema.require_description(False)
 
         self.assertEqual(result.exit_code, 0)
 
     def test_validate_rsp(self) -> None:
         """Test RSP schema type validation."""
         runner = CliRunner()
         result = runner.invoke(cli, ["validate", "-s", "RSP", TEST_YAML], catch_exceptions=False)
```

### Comparing `lsst-felis-26.2024.900/tests/test_datamodel.py` & `lsst_felis-27.0.0rc1/tests/test_datamodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,22 +71,22 @@
             Column(name="testColumn", id="#test_id")
 
         # Setting name, id, and datatype should not throw an exception and
         # should load data correctly.
         col = Column(name="testColumn", id="#test_id", datatype="string")
         self.assertEqual(col.name, "testColumn", "name should be 'testColumn'")
         self.assertEqual(col.id, "#test_id", "id should be '#test_id'")
-        self.assertEqual(col.datatype, DataType.STRING.value, "datatype should be 'DataType.STRING'")
+        self.assertEqual(col.datatype, DataType.string, "datatype should be 'DataType.string'")
 
         # Creating from data dictionary should work and load data correctly.
         data = {"name": "testColumn", "id": "#test_id", "datatype": "string"}
         col = Column(**data)
         self.assertEqual(col.name, "testColumn", "name should be 'testColumn'")
         self.assertEqual(col.id, "#test_id", "id should be '#test_id'")
-        self.assertEqual(col.datatype, DataType.STRING.value, "datatype should be 'DataType.STRING'")
+        self.assertEqual(col.datatype, DataType.string, "datatype should be 'DataType.string'")
 
         # Setting a bad IVOA UCD should throw an error.
         with self.assertRaises(ValidationError):
             Column(**data, ivoa_ucd="bad")
 
         # Setting a valid IVOA UCD should not throw an error.
         col = Column(**data, ivoa_ucd="meta.id")
@@ -119,52 +119,82 @@
         # Setting both IVOA unit and FITS TUNIT should throw an error.
         units_data["ivoa:unit"] = "m"
         with self.assertRaises(ValidationError):
             Column(**units_data)
 
     def test_require_description(self) -> None:
         """Test the require_description flag for the `Column` class."""
-        # Turn on description requirement for this test.
-        Schema.require_description(True)
 
-        # Make sure that setting the flag for description requirement works
-        # correctly.
-        self.assertTrue(Schema.is_description_required(), "description should be required")
-
-        # Creating a column without a description when required should throw an
-        # error.
-        with self.assertRaises(ValidationError):
-            Column(
-                **{
-                    "name": "testColumn",
-                    "@id": "#test_col_id",
-                    "datatype": "string",
-                }
+        class MockValidationInfo:
+            """Mock context object for passing to validation method."""
+
+            def __init__(self):
+                self.context = {"require_description": True}
+
+        info = MockValidationInfo()
+
+        def _check_description(col: Column):
+            Schema.check_description(col, info)
+
+        # Creating a column without a description should throw.
+        with self.assertRaises(ValueError):
+            _check_description(
+                Column(
+                    **{
+                        "name": "testColumn",
+                        "@id": "#test_col_id",
+                        "datatype": "string",
+                    }
+                )
             )
 
-        # Creating a column with a None description when required should throw.
-        with self.assertRaises(ValidationError):
-            Column(**{"name": "testColumn", "@id": "#test_col_id", "datatype": "string", "description": None})
+        # Creating a column with a description of 'None' should throw.
+        with self.assertRaises(ValueError):
+            _check_description(
+                Column(
+                    **{
+                        "name": "testColumn",
+                        "@id": "#test_col_id",
+                        "datatype": "string",
+                        "description": None,
+                    }
+                )
+            )
 
-        # Creating a column with an empty description when required should
-        # throw.
-        with self.assertRaises(ValidationError):
-            Column(**{"name": "testColumn", "@id": "#test_col_id", "datatype": "string", "description": ""})
+        # Creating a column with an empty description should throw.
+        with self.assertRaises(ValueError):
+            _check_description(
+                Column(
+                    **{
+                        "name": "testColumn",
+                        "@id": "#test_col_id",
+                        "datatype": "string",
+                        "require_description": True,
+                        "description": "",
+                    }
+                )
+            )
 
-        # Creating a column with a description that is not long enough should
-        # throw.
+        # Creating a column with a description that is too short should throw.
         with self.assertRaises(ValidationError):
-            Column(**{"name": "testColumn", "@id": "#test_col_id", "datatype": "string", "description": "xy"})
-
-        # Turn off flag or it will affect subsequent tests.
-        Schema.require_description(False)
+            _check_description(
+                Column(
+                    **{
+                        "name": "testColumn",
+                        "@id": "#test_col_id",
+                        "datatype": "string",
+                        "require_description": True,
+                        "description": "xy",
+                    }
+                )
+            )
 
 
 class ConstraintTestCase(unittest.TestCase):
-    """Test the `UniqueConstraint`, `Index`, `CheckCosntraint`, and
+    """Test the `UniqueConstraint`, `Index`, `CheckConstraint`, and
     `ForeignKeyConstraint` classes.
     """
 
     def test_unique_constraint_validation(self) -> None:
         """Test validation of the `UniqueConstraint` class."""
         # Default initialization should throw an exception.
         with self.assertRaises(ValidationError):
```

### Comparing `lsst-felis-26.2024.900/tests/test_simple.py` & `lsst_felis-27.0.0rc1/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/tests/test_tap.py` & `lsst_felis-27.0.0rc1/tests/test_tap.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/tests/test_utils.py` & `lsst_felis-27.0.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.900/tests/test_validation.py` & `lsst_felis-27.0.0rc1/tests/test_validation.py`

 * *Files identical despite different names*

