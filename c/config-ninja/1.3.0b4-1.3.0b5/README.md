# Comparing `tmp/config_ninja-1.3.0b4.tar.gz` & `tmp/config_ninja-1.3.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_ninja-1.3.0b4.tar", max compression
+gzip compressed data, was "config_ninja-1.3.0b5.tar", max compression
```

## Comparing `config_ninja-1.3.0b4.tar` & `config_ninja-1.3.0b5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-28 21:02:47.107949 config_ninja-1.3.0b4/LICENSE
--rw-r--r--   0        0        0     5427 2024-04-28 21:02:47.107949 config_ninja-1.3.0b4/README.md
--rw-r--r--   0        0        0    32807 2024-04-28 21:03:24.983878 config_ninja-1.3.0b4/pyproject.toml
--rw-r--r--   0        0        0     1454 2024-04-28 21:03:24.987878 config_ninja-1.3.0b4/src/config_ninja/__init__.py
--rw-r--r--   0        0        0      465 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/__main__.py
--rw-r--r--   0        0        0     2433 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/backend.py
--rw-r--r--   0        0        0     3592 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/cli.md
--rw-r--r--   0        0        0    18047 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/cli.py
--rw-r--r--   0        0        0     1015 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/contrib/__init__.py
--rw-r--r--   0        0        0    10870 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/contrib/appconfig.py
--rw-r--r--   0        0        0     2143 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/contrib/local.py
--rw-r--r--   0        0        0     7643 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/systemd.py
--rw-r--r--   0        0        0      620 2024-04-28 21:02:47.119949 config_ninja-1.3.0b4/src/config_ninja/templates/systemd.service.j2
--rw-r--r--   0        0        0     7002 1970-01-01 00:00:00.000000 config_ninja-1.3.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-29 00:41:09.870424 config_ninja-1.3.0b5/LICENSE
+-rw-r--r--   0        0        0     5427 2024-04-29 00:41:09.870424 config_ninja-1.3.0b5/README.md
+-rw-r--r--   0        0        0    32812 2024-04-29 00:41:54.462352 config_ninja-1.3.0b5/pyproject.toml
+-rw-r--r--   0        0        0     1454 2024-04-29 00:41:54.466352 config_ninja-1.3.0b5/src/config_ninja/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-29 00:41:09.878424 config_ninja-1.3.0b5/src/config_ninja/__main__.py
+-rw-r--r--   0        0        0     2433 2024-04-29 00:41:09.878424 config_ninja-1.3.0b5/src/config_ninja/backend.py
+-rw-r--r--   0        0        0     3592 2024-04-29 00:41:09.878424 config_ninja-1.3.0b5/src/config_ninja/cli.md
+-rw-r--r--   0        0        0    17917 2024-04-29 00:41:09.878424 config_ninja-1.3.0b5/src/config_ninja/cli.py
+-rw-r--r--   0        0        0     1015 2024-04-29 00:41:09.878424 config_ninja-1.3.0b5/src/config_ninja/contrib/__init__.py
+-rw-r--r--   0        0        0    10870 2024-04-29 00:41:09.878424 config_ninja-1.3.0b5/src/config_ninja/contrib/appconfig.py
+-rw-r--r--   0        0        0     2143 2024-04-29 00:41:09.878424 config_ninja-1.3.0b5/src/config_ninja/contrib/local.py
+-rw-r--r--   0        0        0     7643 2024-04-29 00:41:09.878424 config_ninja-1.3.0b5/src/config_ninja/systemd.py
+-rw-r--r--   0        0        0      620 2024-04-29 00:41:09.878424 config_ninja-1.3.0b5/src/config_ninja/templates/systemd.service.j2
+-rw-r--r--   0        0        0     6998 1970-01-01 00:00:00.000000 config_ninja-1.3.0b5/PKG-INFO
```

### Comparing `config_ninja-1.3.0b4/LICENSE` & `config_ninja-1.3.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `config_ninja-1.3.0b4/README.md` & `config_ninja-1.3.0b5/README.md`

 * *Files identical despite different names*

### Comparing `config_ninja-1.3.0b4/pyproject.toml` & `config_ninja-1.3.0b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 # https://python-poetry.org/docs/pyproject/
 name = "config-ninja"
-version = "1.3.0b4"
+version = "1.3.0b5"
 description = "Use special ninja powers to manage system configurations 🥷"
 authors = ["Bryant Finney <bryant.finney@outlook.com>"]
 documentation = "https://config-ninja.readthedocs.org/home.html"
 exclude = ["**/conftest.py"]
 homepage = "https://config-ninja.github.io/config-ninja/config_ninja.html"
 license = "MIT"
 readme = "README.md"
@@ -110,15 +110,15 @@
 upload_to_vcs_release = true
 
 [tool.poetry.dependencies]
 # https://python-poetry.org/docs/dependency-specification/
 python = "^3.8.1"
 pyyaml = "^6.0"
 typing-extensions = { version = "^4.7.1", python = "3.8" }
-typer = {extras = ["all"], version = "^0.9.0"}
+typer = {extras = ["all"], version = ">=0.9,<0.13"}
 boto3 = { version = "^1.34.11", optional = true }
 pyspry = "^1.0.2"
 watchfiles = { version = "^0.21.0", optional = true }
 jinja2 = "^3.1.2"
 tomlkit = "^0.12.3"
 # sdnotify is designed to handle errors when systemd is missing
 sdnotify = "^0.3.2"
```

### Comparing `config_ninja-1.3.0b4/src/config_ninja/__init__.py` & `config_ninja-1.3.0b5/src/config_ninja/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     - `config_ninja.contrib.local`
 - `config_ninja.cli` for commands and CLI documentation
 - `config_ninja.systemd` for `systemd` integration
 """  # noqa: D415
 
 from __future__ import annotations
 
-__version__ = '1.3.0b4'
+__version__ = '1.3.0b5'
 
 from pathlib import Path
 
 from pyspry import Settings
 
 __all__ = ['DEFAULT_SETTINGS_PATHS', 'load_settings', 'resolve_settings_path']
```

### Comparing `config_ninja-1.3.0b4/src/config_ninja/backend.py` & `config_ninja-1.3.0b5/src/config_ninja/backend.py`

 * *Files identical despite different names*

### Comparing `config_ninja-1.3.0b4/src/config_ninja/cli.md` & `config_ninja-1.3.0b5/src/config_ninja/cli.md`

 * *Files identical despite different names*

### Comparing `config_ninja-1.3.0b4/src/config_ninja/cli.py` & `config_ninja-1.3.0b5/src/config_ninja/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,23 +141,18 @@
     typing.Optional[Path],
     typer.Option(
         '-w', '--workdir', help='Run the service from this directory.', show_default=False
     ),
 ]
 
 
-def parse_env(
-    ctx: typer.Context, value: typing.Optional[typing.List[str]]
-) -> typing.Optional[typing.List[str]]:
+def parse_env(ctx: typer.Context, value: typing.Optional[typing.List[str]]) -> typing.List[str]:
     """Parse the environment variables from the command line."""
-    if ctx.resilient_parsing:  # pragma: no cover  # this is for tab completions
-        return None
-
-    if not value:
-        return value
+    if ctx.resilient_parsing or not value:
+        return []
 
     return [v for val in value for v in val.split(',')]
 
 
 EnvNamesAnnotation: TypeAlias = Annotated[
     typing.Optional[typing.List[str]],
     typer.Option(
@@ -182,15 +177,15 @@
 
     @classmethod
     def parse(cls, value: str) -> 'UserGroup':
         """Parse the `--run-as user[:group]` argument for the `systemd` service."""
         return cls(*value.split(':'))
 
 
-RunAsAnnotation: TypeAlias = typing.Annotated[
+RunAsAnnotation: TypeAlias = Annotated[
     typing.Optional[UserGroup],
     typer.Option(
         '--run-as',
         help='Configure the systemd unit to run the service as this user (and optionally group).',
         metavar='user[:group]',
         parser=UserGroup.parse,
     ),
@@ -487,15 +482,15 @@
 
     Example:
             config-ninja self install --env FOO,BAR,BAZ --env SPAM --var EGGS=42
 
     The environment variables [purple]FOO[/], [purple]BAR[/], [purple]BAZ[/], and [purple]SPAM[/] will be read from the current shell and written to the service file, while [purple]EGGS[/] will be set to [yellow]42[/].
     """
     environ = {name: os.environ[name] for name in env_names or [] if name in os.environ}
-    environ.update(variables)  # type: ignore[arg-type]
+    environ.update(variables or [])
 
     kwargs = {
         # the command to use when invoking config-ninja from systemd
         'config_ninja_cmd': sys.argv[0]
         if sys.argv[0].endswith('config-ninja')
         else f'{sys.executable} {sys.argv[0]}',
         # write these environment variables into the systemd service file
```

### Comparing `config_ninja-1.3.0b4/src/config_ninja/contrib/__init__.py` & `config_ninja-1.3.0b5/src/config_ninja/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `config_ninja-1.3.0b4/src/config_ninja/contrib/appconfig.py` & `config_ninja-1.3.0b5/src/config_ninja/contrib/appconfig.py`

 * *Files identical despite different names*

### Comparing `config_ninja-1.3.0b4/src/config_ninja/contrib/local.py` & `config_ninja-1.3.0b5/src/config_ninja/contrib/local.py`

 * *Files identical despite different names*

### Comparing `config_ninja-1.3.0b4/src/config_ninja/systemd.py` & `config_ninja-1.3.0b5/src/config_ninja/systemd.py`

 * *Files identical despite different names*

### Comparing `config_ninja-1.3.0b4/src/config_ninja/templates/systemd.service.j2` & `config_ninja-1.3.0b5/src/config_ninja/templates/systemd.service.j2`

 * *Files identical despite different names*

### Comparing `config_ninja-1.3.0b4/PKG-INFO` & `config_ninja-1.3.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-ninja
-Version: 1.3.0b4
+Version: 1.3.0b5
 Summary: Use special ninja powers to manage system configurations 🥷
 Home-page: https://config-ninja.github.io/config-ninja/config_ninja.html
 License: MIT
 Author: Bryant Finney
 Author-email: bryant.finney@outlook.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,15 @@
 Requires-Dist: boto3 (>=1.34.11,<2.0.0) ; extra == "all" or extra == "appconfig"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pyspry (>=1.0.2,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: sdnotify (>=0.3.2,<0.4.0)
 Requires-Dist: sh (>=2.0.6,<3.0.0) ; sys_platform != "win32"
 Requires-Dist: tomlkit (>=0.12.3,<0.13.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer[all] (>=0.9,<0.13)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0) ; python_version == "3.8"
 Requires-Dist: watchfiles (>=0.21.0,<0.22.0) ; extra == "all" or extra == "local"
 Project-URL: Documentation, https://config-ninja.readthedocs.org/home.html
 Project-URL: Repository, https://github.com/config-ninja/config-ninja
 Description-Content-Type: text/markdown
 
 # Config Ninja 🥷
```

