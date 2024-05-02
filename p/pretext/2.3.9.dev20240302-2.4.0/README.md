# Comparing `tmp/pretext-2.3.9.dev20240302.tar.gz` & `tmp/pretext-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-2.3.9.dev20240302.tar", max compression
+gzip compressed data, was "pretext-2.4.0.tar", max compression
```

## Comparing `pretext-2.3.9.dev20240302.tar` & `pretext-2.4.0.tar`

### file list

```diff
@@ -1,29 +1,70 @@
--rw-r--r--   0        0        0    35148 2024-03-02 06:13:55.904540 pretext-2.3.9.dev20240302/LICENSE
--rw-r--r--   0        0        0     9757 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/README.md
--rw-r--r--   0        0        0     1505 2024-03-02 06:14:26.060811 pretext-2.3.9.dev20240302/pretext/__init__.py
--rw-r--r--   0        0        0       61 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/__main__.py
--rw-r--r--   0        0        0    28397 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/cli.py
--rw-r--r--   0        0        0     6149 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/codechat.py
--rw-r--r--   0        0        0     3310 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/constants.py
--rw-r--r--   0        0        0      714 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/core/__init__.py
--rw-r--r--   0        0        0   184007 2024-03-02 06:14:29.864845 pretext-2.3.9.dev20240302/pretext/core/pretext.py
--rw-r--r--   0        0        0     1848 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/core/resources.py
--rw-r--r--   0        0        0  1115903 2024-03-02 06:14:29.864845 pretext-2.3.9.dev20240302/pretext/core/resources.zip
--rw-r--r--   0        0        0    66064 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/project/__init__.py
--rw-r--r--   0        0        0     3329 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/project/xml.py
--rw-r--r--   0        0        0     1173 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/templates/__init__.py
--rw-r--r--   0        0        0     3149 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/.devcontainer.json
--rw-r--r--   0        0        0     1939 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160335 2024-03-02 06:14:29.936846 pretext-2.3.9.dev20240302/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0    10351 2024-03-02 06:14:29.940846 pretext-2.3.9.dev20240302/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0     3028 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/codechat_config.yaml
--rw-r--r--   0        0        0   174088 2024-03-02 06:14:29.928846 pretext-2.3.9.dev20240302/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     5045 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      432 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8885 2024-03-02 06:14:29.944846 pretext-2.3.9.dev20240302/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0      183 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/types.py
--rw-r--r--   0        0        0    26658 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/utils.py
--rw-r--r--   0        0        0     3514 2024-03-02 06:14:26.064811 pretext-2.3.9.dev20240302/pyproject.toml
--rw-r--r--   0        0        0    10923 1970-01-01 00:00:00.000000 pretext-2.3.9.dev20240302/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-05-02 01:58:25.787331 pretext-2.4.0/LICENSE
+-rw-r--r--   0        0        0     9936 2024-05-02 01:58:25.787331 pretext-2.4.0/README.md
+-rw-r--r--   0        0        0     1505 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/__main__.py
+-rw-r--r--   0        0        0    31572 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/cli.py
+-rw-r--r--   0        0        0     6149 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/codechat.py
+-rw-r--r--   0        0        0     3592 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/constants.py
+-rw-r--r--   0        0        0      714 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/core/__init__.py
+-rw-r--r--   0        0        0   185418 2024-05-02 01:59:03.023396 pretext-2.4.0/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1848 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/core/resources.py
+-rw-r--r--   0        0        0  1129799 2024-05-02 01:59:03.023396 pretext-2.4.0/pretext/core/resources.zip
+-rw-r--r--   0        0        0      409 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Alignment.jinja2s
+-rw-r--r--   0        0        0      294 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Arrays.jinja2s
+-rw-r--r--   0        0        0      198 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Bibliography.jinja2s
+-rw-r--r--   0        0        0      236 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Boxes.jinja2s
+-rw-r--r--   0        0        0      105 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Breaking.jinja2s
+-rw-r--r--   0        0        0      634 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Crossref.jinja2s
+-rw-r--r--   0        0        0      344 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Floats.jinja2s
+-rw-r--r--   0        0        0     1476 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/FontSelection.jinja2s
+-rw-r--r--   0        0        0       93 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Footnotes.jinja2s
+-rwxr-xr-x   0        0        0      197 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Index.jinja2s
+-rw-r--r--   0        0        0      343 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Lists.jinja2s
+-rw-r--r--   0        0        0      172 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Pictures.jinja2s
+-rw-r--r--   0        0        0      147 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Quotations.jinja2s
+-rw-r--r--   0        0        0     2032 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Sectioning.jinja2s
+-rw-r--r--   0        0        0      493 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Sentences.jinja2s
+-rw-r--r--   0        0        0      329 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Space.jinja2s
+-rw-r--r--   0        0        0       90 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Tabbing.jinja2s
+-rw-r--r--   0        0        0        0 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Themes/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Themes/default/__init__.py
+-rw-r--r--   0        0        0       51 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Themes/default/default-layout.jinja2
+-rw-r--r--   0        0        0     1049 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Themes/default/document-layout.jinja2
+-rw-r--r--   0        0        0      248 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Thms.jinja2s
+-rw-r--r--   0        0        0       65 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/Verbatim.jinja2s
+-rw-r--r--   0        0        0     1882 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/babel.jinja2s
+-rwxr-xr-x   0        0        0      263 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/graphicx.jinja2s
+-rw-r--r--   0        0        0      652 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/hyperref.jinja2s
+-rwxr-xr-x   0        0        0       27 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/lipsum.jinja2s
+-rw-r--r--   0        0        0      251 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/longtable.jinja2s
+-rw-r--r--   0        0        0      436 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/math.jinja2s
+-rw-r--r--   0        0        0        0 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/misc.jinja2s
+-rw-r--r--   0        0        0      270 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/natbib.jinja2s
+-rw-r--r--   0        0        0       87 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/p.jinja2s
+-rw-r--r--   0        0        0      673 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/subfig.jinja2s
+-rw-r--r--   0        0        0      130 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/textcomp.jinja2s
+-rw-r--r--   0        0        0       95 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/tikzcd.jinja2
+-rw-r--r--   0        0        0       94 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/tikzpicture.jinja2
+-rw-r--r--   0        0        0      184 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/url.jinja2s
+-rwxr-xr-x   0        0        0       96 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/plastex/wrapfig.jinja2s
+-rw-r--r--   0        0        0    66255 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/project/__init__.py
+-rw-r--r--   0        0        0     3329 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/project/xml.py
+-rw-r--r--   0        0        0     1173 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     3259 2024-05-02 01:59:03.107396 pretext-2.4.0/pretext/templates/resources/.devcontainer.json
+-rw-r--r--   0        0        0     1939 2024-05-02 01:59:03.107396 pretext-2.4.0/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-02 01:59:03.107396 pretext-2.4.0/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160389 2024-05-02 01:59:03.107396 pretext-2.4.0/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0    10405 2024-05-02 01:59:03.095396 pretext-2.4.0/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0     3028 2024-05-02 01:59:03.107396 pretext-2.4.0/pretext/templates/resources/codechat_config.yaml
+-rw-r--r--   0        0        0   174142 2024-05-02 01:59:03.087396 pretext-2.4.0/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2456 2024-05-02 01:59:03.107396 pretext-2.4.0/pretext/templates/resources/deploy.yml
+-rw-r--r--   0        0        0     5099 2024-05-02 01:59:03.091396 pretext-2.4.0/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0      432 2024-05-02 01:59:03.107396 pretext-2.4.0/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2024-05-02 01:59:03.107396 pretext-2.4.0/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8939 2024-05-02 01:59:03.099396 pretext-2.4.0/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0     1127 2024-05-02 01:59:03.107396 pretext-2.4.0/pretext/templates/resources/test-build.yml
+-rw-r--r--   0        0        0      183 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/types.py
+-rw-r--r--   0        0        0    27080 2024-05-02 01:58:25.791331 pretext-2.4.0/pretext/utils.py
+-rw-r--r--   0        0        0     3803 2024-05-02 01:59:03.811397 pretext-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11153 1970-01-01 00:00:00.000000 pretext-2.4.0/PKG-INFO
```

### Comparing `pretext-2.3.9.dev20240302/LICENSE` & `pretext-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240302/README.md` & `pretext-2.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -240,30 +240,33 @@
 need to be rebuilt by each user when pulled from GitHub.
 
 The file `pretext/__init__.py` tracks the upstream
 commit of core PreTeXt XSL/Python code we're developing against
 (from `PreTeXtBook/pretext`).
 To fetch these updates from upstream, run:
 
-```
+```bash
 poetry run python scripts/fetch_core.py
 ```
 
 If you instead want to point to a local copy of `PreTeXtBook/pretext`,
 try this instead to set up symlinks:
 
-```
+```bash
 poetry run python scripts/symlink_core.py path/to/pretext
 ```
 
+For more detailed directions on using a local copy of the core resources to develop core and CLI together, see [docs/core_development.md](docs/core_development.md).
+
+
 Updates to `templates/` must be zipped and moved into
 `pretext/templates/resources`. This is done automatically by
 running:
 
-```
+```bash
 poetry run python scripts/zip_templates.py
 ```
 
 ### Formatting code before a commit
 
 All `.py` files are formatted with the [black](https://black.readthedocs.io/en/stable/)
 python formatter and checked by [flake8](https://flake8.pycqa.org/en/latest/).
```

### Comparing `pretext-2.3.9.dev20240302/pretext/__init__.py` & `pretext-2.4.0/pretext/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from single_version import get_version
 
 log = logging.getLogger("ptxlogger")
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = '7aef3b1d4f73a6409da1efefef3528a3b9fb0cfa'
+CORE_COMMIT = "5e1c5f622d5a3dfd829d5392960432898b98513b"
 
 
 def activate() -> None:
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-2.3.9.dev20240302/pretext/cli.py` & `pretext-2.4.0/pretext/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 from pathlib import Path
 import atexit
 import subprocess
 from pydantic import ValidationError
 from typing import Any, Callable, List, Literal, Optional
 from functools import update_wrapper
 
+
 from . import (
     utils,
     templates,
     core,
     constants,
+    plastex,
     VERSION,
     CORE_COMMIT,
 )
 
 
 from .project import Project
 
@@ -138,14 +140,15 @@
         logfile = logdir / f"{datetime.datetime.now().strftime('%Y%m%d-%H%M%S')}.log"
         fh = logging.FileHandler(logfile, mode="w")
         fh.setLevel(logging.DEBUG)
         file_log_format = logging.Formatter("{levelname:<8}: {message}", style="{")
         fh.setFormatter(file_log_format)
         log.addHandler(fh)
         # output info
+        log.info(f"PreTeXt-CLI version: {VERSION}\n")
         log.info(f"PreTeXt project found in `{utils.project_path()}`.")
         # permanently change working directory for rest of process
         os.chdir(pp)
         if utils.requirements_version() is None:
             log.warning(
                 "Project's CLI version could not be detected from `requirements.txt`."
             )
@@ -160,14 +163,15 @@
             )
             log.warning(f"to update `requirements.txt` to match {VERSION}.")
         else:
             log.debug(
                 f"CLI version {VERSION} matches requirements.txt {utils.requirements_version()}."
             )
     else:
+        log.info(f"PreTeXt-CLI version: {VERSION}\n")
         log.info("No existing PreTeXt project found.")
     if ctx.invoked_subcommand is None:
         log.info("Run `pretext --help` for help.")
 
 
 # pretext support
 @main.command(
@@ -277,15 +281,15 @@
         with templates.resource_path(f"{template}.zip") as template_path:
             archive = zipfile.ZipFile(template_path)
     # find (first) project.ptx to use as root of template
     filenames = [Path(filepath).name for filepath in archive.namelist()]
     project_ptx_index = filenames.index("project.ptx")
     project_ptx_path = Path(archive.namelist()[project_ptx_index])
     project_dir_path = project_ptx_path.parent
-    with tempfile.TemporaryDirectory() as tmpdirname:
+    with tempfile.TemporaryDirectory(prefix="pretext_") as tmpdirname:
         temp_path = Path(tmpdirname) / "new-project"
         temp_path.mkdir()
         for filepath in [
             filepath
             for filepath in archive.namelist()
             if project_dir_path in Path(filepath).parents
         ]:
@@ -318,15 +322,15 @@
 )
 @click.option(
     "-f",
     "--file",
     "files",
     help="Specify file to refresh.",
     multiple=True,
-    type=click.Choice(constants.PROJECT_RESOURCES, case_sensitive=False),
+    type=click.Choice([r for r in constants.PROJECT_RESOURCES], case_sensitive=False),
 )
 @nice_errors
 def init(refresh: bool, files: List[str]) -> None:
     """
     Generates/updates CLI-specific files for the current version of PreTeXt-CLI.
     This feature is mainly intended for updating existing PreTeXt projects to use this CLI,
     or to update project files generated from earlier CLI versions.
@@ -638,25 +642,32 @@
 @click.option(
     "-d",
     "--stage",
     is_flag=True,
     default=False,
     help="View the staged deployment.",
 )
+@click.option(
+    "--default-server",
+    is_flag=True,
+    default=False,
+    help="Use the standard python server, even if in a codespace (for debugging)",
+)
 @nice_errors
 def view(
     target_name: str,
     access: Literal["public", "private"],
     port: int,
     build: bool,
     generate: bool,
     no_launch: bool,
     restart_server: bool,
     stop_server: bool,
     stage: bool,
+    default_server: str,
 ) -> None:
     """
     Starts a local server to preview built PreTeXt documents in your browser.
     TARGET is the name of a <target/> defined in `project.ptx` (defaults to the first target).
 
     After running this command, you can switch to a new terminal to rebuild your project and see the changes automatically reflected in your browser.
 
@@ -698,14 +709,40 @@
     if stage:
         target_name = "staged deployment"
         url_path = "/" + project.stage.as_posix()
     else:
         target_name = f"target `{target.name}`"
         url_path = "/" + target.output_dir_relpath().as_posix()
 
+    in_codespace = os.environ.get("CODESPACES")
+
+    if in_codespace and not default_server:
+        log.info(
+            "Running in a codespace, so using the codespace server instead of the standard python server."
+        )
+        used_port = utils.active_server_port()
+        # First terminate any existing server using this port
+        if used_port == port:
+            utils.stop_server(used_port)
+        # set the url
+        url_base = utils.url_for_access(access=access, port=port)
+        url = url_base + url_path
+        log.info(f"Server will soon be available at {url_base}")
+        if no_launch:
+            log.info(f"The {target_name} will be available at {url}")
+        else:
+            SECONDS = 5
+            log.info(f"Opening browser for {target_name} at {url} in {SECONDS} seconds")
+            time.sleep(SECONDS)
+            webbrowser.open(url)
+        utils.start_codespace_server(port=port, access=access)
+        log.info(
+            f"Server will soon be available at {utils.url_for_access(access, port)}"
+        )
+        return
     # Start server if there isn't one running already:
     used_port = utils.active_server_port()
     if restart_server or (port != used_port) or (used_port is None):
         log.info(
             f"Now preparing local server to preview your project directory `{project.abspath()}`."
         )
         log.info(
@@ -731,17 +768,17 @@
         # set the url
         url_base = utils.url_for_access(access=access, port=actual_port)
         url = url_base + url_path
         log.info(f"Server will soon be available at {url_base}")
         if no_launch:
             log.info(f"The {target_name} will be available at {url}")
         else:
-            SECONDS = 3
-            log.info(f"Opening browser for {target_name} at {url} in {SECONDS} seconds")
-            time.sleep(SECONDS)
+            # SECONDS = 2
+            log.info(f"Opening browser for {target_name} at {url}")
+            # time.sleep(SECONDS)
             webbrowser.open(url)
         try:
             while server.is_alive():
                 time.sleep(1)
         except KeyboardInterrupt:
             log.info("Stopping server.")
             server.terminate()
@@ -783,7 +820,51 @@
     project.stage_deployment()
     if stage_only:
         return
     if preview:
         ctx.invoke(view, stage=True)
     else:
         project.deploy(update_source=update_source, skip_staging=True)
+
+
+# pretext import
+@main.command(
+    short_help="Experimental: convert a latex file to pretext",
+    context_settings=CONTEXT_SETTINGS,
+    name="import",
+)
+@nice_errors
+@click.pass_context
+@click.argument("latex_file", required=True)
+@click.option("-o", "--output", help="Specify output directory", required=False)
+def import_command(ctx: click.Context, latex_file: str, output: str) -> None:
+    """
+    Experimental: convert a latex file to pretext
+    """
+    latex_file_path = Path(latex_file).resolve()
+    if not latex_file_path.exists():
+        log.error(f"File {latex_file_path} does not exist.")
+        return
+    if output is not None:
+        output_path = Path(output).resolve()
+        if not output_path.exists():
+            log.warning("Output directory does not exist. Creating it.")
+            output_path.mkdir(parents=True)
+    else:
+        output_path = Path.cwd() / "imports" / latex_file_path.stem
+        output_path.mkdir(parents=True, exist_ok=True)
+    # Now we use plastex to convert:
+    log.info(f"Converting {latex_file_path} to PreTeXt.")
+    with tempfile.TemporaryDirectory(prefix="pretext_") as tmpdirname:
+        temp_path = Path(tmpdirname) / "import"
+        temp_path.mkdir()
+        log.info(f"Using temporary directory {temp_path}")
+        # change to this directory to run plastex
+        with utils.working_directory(temp_path):
+            try:
+                plastex.convert(latex_file_path, output_path)
+                shutil.copytree(temp_path, output_path, dirs_exist_ok=True)
+                log.debug(f"Conversion done in {temp_path}")
+            except Exception as e:
+                log.error(e)
+                log.debug("Exception info:\n------------------------\n", exc_info=True)
+                raise SystemExit(1)
```

### Comparing `pretext-2.3.9.dev20240302/pretext/codechat.py` & `pretext-2.4.0/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240302/pretext/constants.py` & `pretext-2.4.0/pretext/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing as t
+from pathlib import Path
 
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 
 FORMATS = ["html", "pdf", "latex", "epub", "kindle", "braille", "webwork", "custom"]
 
 # Give list of assets that each build format requires.
 ASSETS_BY_FORMAT = {
@@ -139,14 +140,16 @@
     "custom": {
         "asymptote": ["all"],
         "latex-image": ["all"],
         "sageplot": ["all"],
     },
 }
 
-PROJECT_RESOURCES = [
-    "project.ptx",
-    "codechat_config.yaml",
-    ".gitignore",
-    ".devcontainer.json",
-    "requirements.txt",
-]
+PROJECT_RESOURCES = {
+    "project.ptx": Path("project.ptx"),
+    "codechat_config.yaml": Path("codechat_config.yaml"),
+    ".gitignore": Path(".gitignore"),
+    ".devcontainer.json": Path(".devcontainer.json"),
+    "requirements.txt": Path("requirements.txt"),
+    "deploy.yml": Path(".github", "workflows", "deploy.yml"),
+    "test-build.yml": Path(".github", "workflows", "test-build.yml"),
+}
```

### Comparing `pretext-2.3.9.dev20240302/pretext/core/__init__.py` & `pretext-2.4.0/pretext/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240302/pretext/core/pretext.py` & `pretext-2.4.0/pretext/core/pretext.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
                 )
                 # bytes -> ASCII, strip final newline
                 asyversion = proc.stderr.read().decode("ascii")[:-1]
                 # build command line to suit
                 # 2021-12-10, Michael Doob: "-noprc" is default for the server,
                 # and newer CLI versions.  Retain for explicit use locally when
                 # perhaps an older version is being employed
-                asy_cli = asy_executable_cmd + ["-f", outform]
+                asy_cli = asy_executable_cmd + ["-f", outform, "-noV"]
                 if outform in ["pdf", "eps"]:
                     asy_cli += ["-noprc", "-iconify", "-tex", "xelatex", "-batchMask"]
                 elif outform in ["svg", "png"]:
                     asy_cli += ["-render=4", "-tex", "xelatex", "-iconify"]
             if method == "server":
                 alberta = "http://asymptote.ualberta.ca:10007?f={}".format(outform)
             # loop over .asy files, doing conversions
@@ -484,25 +484,44 @@
                 log.info("copying {} to {}".format(latex_image, dest_dir))
             else:
                 filebase, _ = os.path.splitext(latex_image)
                 latex_image_pdf = "{}.pdf".format(filebase)
                 latex_image_svg = "{}.svg".format(filebase)
                 latex_image_png = "{}.png".format(filebase)
                 latex_image_eps = "{}.eps".format(filebase)
+                latex_image_log = "{}.log".format(filebase)
                 # process with a  latex  engine
                 latex_key = get_deprecated_tex_fallback(method)
                 tex_executable_cmd = get_executable_cmd(latex_key)
                 # TODO why this debug line? get_executable_cmd() outputs the same debug info
                 log.debug("tex executable: {}".format(tex_executable_cmd[0]))
                 latex_cmd = tex_executable_cmd + ["-interaction=nonstopmode", "-halt-on-error", latex_image]
                 log.info("converting {} to {}".format(latex_image, latex_image_pdf))
                 # Run LaTeX on the image file, usual console transcript is stdout.
                 # "result" is a "CompletedProcess" object.  Specifying an encoding
                 # causes captured output to be a string, which is convenient.
                 result = subprocess.run(latex_cmd, stdout=subprocess.PIPE, encoding="utf-8")
+
+                # It may be that the image needs to be compiled twice. If the .log file contains
+                # the string `Rerun to get`, then the document should be compiled again.
+
+                # We keep track of how many times we've tried to compile the document and
+                # bail if it looks like we're stuck in a loop.
+                loop_count = 0
+                MAX_LOOPS = 10
+                while result.returncode == 0 and "Rerun to get" in open(latex_image_log).read() and loop_count < MAX_LOOPS:
+                    msg = "File {} needs to be processed with LaTeX again. Rerunning LaTeX for pass number {}."
+                    log.info(msg.format(latex_image, loop_count + 2))
+                    result = subprocess.run(latex_cmd, stdout=subprocess.PIPE, encoding="utf-8")
+                    loop_count += 1
+
+                if loop_count == MAX_LOOPS:
+                    log.error("Detected infinite loop while compiling {}. Aborting.".format(latex_image))
+                    result.returncode = 1
+
                 if result.returncode != 0:
                     # failed
                     failed_images.append(latex_image)
                     # and we help as much as we can
                     msg = "\n".join(
                         [
                             "LaTeX compilation of {} failed.",
@@ -559,15 +578,15 @@
                         if pyMuPDF:
                             # create svg using pymupdf:
                             with fitz.Document(latex_image_pdf) as doc:
                                 svg = doc.load_page(0).get_svg_image()
                             with open(latex_image_svg, "w") as f:
                                 f.write(svg)
                             shutil.copy2(latex_image_svg, dest_dir)
-                            # clasic way to produce svg, using pdf2svg:
+                            # classic way to produce svg, using pdf2svg:
                             latex_image_svg = "classic-" + latex_image_svg
                         pdfsvg_executable_cmd = get_executable_cmd("pdfsvg")
                         # TODO why this debug line? get_executable_cmd() outputs the same debug info
                         log.debug("pdfsvg executable: {}".format(pdfsvg_executable_cmd[0]))
                         svg_cmd = pdfsvg_executable_cmd + [latex_image_pdf, latex_image_svg]
                         log.info(
                             "converting {} to {}".format(latex_image_pdf, latex_image_svg)
@@ -3560,24 +3579,30 @@
         nonlocal result_tree, texc
         try:
             result_tree = xslt(src_tree, **stringparams)
         except Exception as e:
             texc = e
 
     try:
-        outputfn("comprehensive messages, warnings, and errors:")
         parse_t = threading.Thread(target=transform)
         parse_t.start()
         still_alive = True
         start = 0
         while still_alive:
             parse_t.join(0.5)  # Wait 0.5 seconds for thread to complete
             still_alive = parse_t.is_alive()
 
             end = len(xslt.error_log)
+
+            # if there are any messages and we are just
+            # starting out, produce an explanatory line
+            # start will be reset to non-zero, so this is
+            # one-time only, and never if there are no messages
+            if (start == 0) and (end > 0):
+                outputfn("messages from the log for XSL processing (indented):")
             # print out any unprinted messages from error_log
             for line in range(start, end):
                 outputfn(f"    * {xslt.error_log[line].message}")
             start = end
         if texc is None:
             outputfn("successful application of {}".format(xsl))
         else:
@@ -3960,15 +3985,15 @@
 
 def get_temporary_directory():
     """Create, record, and return a scratch directory"""
     import tempfile  #  mkdtemp()
 
     global __temps  #  cache of temporary directories
 
-    temp_dir = tempfile.mkdtemp()
+    temp_dir = tempfile.mkdtemp(prefix="ptx-")
     # Register the directory for cleanup at the end of successful
     # execution iff the verbosity is set to level 2 ("debug")
     # So errors, or requesting gross debugging info, will leave the
     # directories behind for inspection, otherwise they get removed
     __temps.append(temp_dir)
     return temp_dir
```

### Comparing `pretext-2.3.9.dev20240302/pretext/core/resources.py` & `pretext-2.4.0/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240302/pretext/core/resources.zip` & `pretext-2.4.0/pretext/core/resources.zip`

 * *Files 21% similar despite different names*

#### zipinfo {}

```diff
@@ -1,194 +1,196 @@
-Zip file size: 1115903 bytes, number of entries: 192
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 css/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js_lib/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 script/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/utilities/
--rw-r--r--  2.0 unx     1768 b- defN 24-Mar-02 06:14 xsl/README.md
--rw-r--r--  2.0 unx     2597 b- defN 24-Mar-02 06:14 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     6066 b- defN 24-Mar-02 06:14 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    13189 b- defN 24-Mar-02 06:14 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    17295 b- defN 24-Mar-02 06:14 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx    40230 b- defN 24-Mar-02 06:14 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    21086 b- defN 24-Mar-02 06:14 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx   235477 b- defN 24-Mar-02 06:14 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   173803 b- defN 24-Mar-02 06:14 xsl/html-symbols.xsl
--rw-r--r--  2.0 unx     2248 b- defN 24-Mar-02 06:14 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx   119777 b- defN 24-Mar-02 06:14 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    22121 b- defN 24-Mar-02 06:14 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     8783 b- defN 24-Mar-02 06:14 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx    11766 b- defN 24-Mar-02 06:14 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     8130 b- defN 24-Mar-02 06:14 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     9787 b- defN 24-Mar-02 06:14 xsl/entities.ent
--rw-r--r--  2.0 unx     2847 b- defN 24-Mar-02 06:14 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    67630 b- defN 24-Mar-02 06:14 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     2601 b- defN 24-Mar-02 06:14 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    41730 b- defN 24-Mar-02 06:14 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx     2740 b- defN 24-Mar-02 06:14 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     2709 b- defN 24-Mar-02 06:14 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     2734 b- defN 24-Mar-02 06:14 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    19092 b- defN 24-Mar-02 06:14 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     3560 b- defN 24-Mar-02 06:14 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    10708 b- defN 24-Mar-02 06:14 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx    95377 b- defN 24-Mar-02 06:14 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     4571 b- defN 24-Mar-02 06:14 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     3239 b- defN 24-Mar-02 06:14 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     8134 b- defN 24-Mar-02 06:14 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   606337 b- defN 24-Mar-02 06:14 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx   138087 b- defN 24-Mar-02 06:14 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx    13037 b- defN 24-Mar-02 06:14 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    46431 b- defN 24-Mar-02 06:14 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx     6281 b- defN 24-Mar-02 06:14 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   551514 b- defN 24-Mar-02 06:14 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    12084 b- defN 24-Mar-02 06:14 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx    39918 b- defN 24-Mar-02 06:14 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx   114772 b- defN 24-Mar-02 06:14 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx   556693 b- defN 24-Mar-02 06:14 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     4810 b- defN 24-Mar-02 06:14 xsl/localizations/README.md
--rw-r--r--  2.0 unx    16378 b- defN 24-Mar-02 06:14 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    16566 b- defN 24-Mar-02 06:14 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    15924 b- defN 24-Mar-02 06:14 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    15648 b- defN 24-Mar-02 06:14 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17147 b- defN 24-Mar-02 06:14 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16904 b- defN 24-Mar-02 06:14 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    19251 b- defN 24-Mar-02 06:14 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16151 b- defN 24-Mar-02 06:14 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16415 b- defN 24-Mar-02 06:14 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17297 b- defN 24-Mar-02 06:14 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    20546 b- defN 24-Mar-02 06:14 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    19076 b- defN 24-Mar-02 06:14 xsl/localizations/zh-HANS.xml
--rw-r--r--  2.0 unx    17122 b- defN 24-Mar-02 06:14 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16600 b- defN 24-Mar-02 06:14 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    17368 b- defN 24-Mar-02 06:14 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx     2347 b- defN 24-Mar-02 06:14 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    19453 b- defN 24-Mar-02 06:14 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    16318 b- defN 24-Mar-02 06:14 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx     1810 b- defN 24-Mar-02 06:14 xsl/utilities/README.md
--rw-r--r--  2.0 unx     4299 b- defN 24-Mar-02 06:14 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     4926 b- defN 24-Mar-02 06:14 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      787 b- defN 24-Mar-02 06:14 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx    30257 b- defN 24-Mar-02 06:14 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx      513 b- defN 24-Mar-02 06:14 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx    14322 b- defN 24-Mar-02 06:14 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     3024 b- defN 24-Mar-02 06:14 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     7277 b- defN 24-Mar-02 06:14 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     5135 b- defN 24-Mar-02 06:14 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2261 b- defN 24-Mar-02 06:14 xsl/latex/pretext-latex-AIM.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 24-Mar-02 06:14 xsl/support/README.md
--rw-r--r--  2.0 unx    10300 b- defN 24-Mar-02 06:14 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 24-Mar-02 06:14 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 24-Mar-02 06:14 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     5061 b- defN 24-Mar-02 06:14 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5800 b- defN 24-Mar-02 06:14 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      521 b- defN 24-Mar-02 06:14 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     2657 b- defN 24-Mar-02 06:14 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 24-Mar-02 06:14 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 24-Mar-02 06:14 xsl/support/play-button/play-button.png
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 24-Mar-02 06:14 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 24-Mar-02 06:14 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 24-Mar-02 06:14 script/mjsre/README.md
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-02 06:14 script/mjsre/update-sre
--rw-r--r--  2.0 unx      116 b- defN 24-Mar-02 06:14 script/mjsre/package.json
--rw-r--r--  2.0 unx     9251 b- defN 24-Mar-02 06:14 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx     1367 b- defN 24-Mar-02 06:14 pretext/README.md
--rw-r--r--  2.0 unx    36176 b- defN 24-Mar-02 06:14 pretext/braille_format.py
--rw-r--r--  2.0 unx     1955 b- defN 24-Mar-02 06:14 pretext/module-test.py
--rw-r--r--  2.0 unx   184007 b- defN 24-Mar-02 06:14 pretext/pretext.py
--rw-r--r--  2.0 unx      215 b- defN 24-Mar-02 06:14 pretext/requirements.txt
--rw-r--r--  2.0 unx    30970 b- defN 24-Mar-02 06:14 pretext/pretext
--rw-r--r--  2.0 unx     2566 b- defN 24-Mar-02 06:14 pretext/pretext.cfg
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-02 06:14 pretext/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js/pretext-webwork/
--rw-r--r--  2.0 unx    42973 b- defN 24-Mar-02 06:14 js/pretext_add_on.js
--rw-r--r--  2.0 unx    10957 b- defN 24-Mar-02 06:14 js/login.js
--rw-r--r--  2.0 unx     6509 b- defN 24-Mar-02 06:14 js/pretext.js
--rw-r--r--  2.0 unx   228054 b- defN 24-Mar-02 06:14 js/edit.js
--rw-r--r--  2.0 unx    12113 b- defN 24-Mar-02 06:14 js/pretext_search.js
--rw-r--r--  2.0 unx     5318 b- defN 24-Mar-02 06:14 js/instructor.js
--rw-r--r--  2.0 unx    25633 b- defN 24-Mar-02 06:14 js/answer.js
--rw-r--r--  2.0 unx     3693 b- defN 24-Mar-02 06:14 js/ptx_search.js
--rw-r--r--  2.0 unx    23560 b- defN 24-Mar-02 06:14 js/highlight.js
--rw-r--r--  2.0 unx    20911 b- defN 24-Mar-02 06:14 js/user_preferences.js
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js/pretext-webwork/2.16/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js/pretext-webwork/2.17/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js/pretext-webwork/2.18/
--rw-r--r--  2.0 unx    44152 b- defN 24-Mar-02 06:14 js/pretext-webwork/2.18/pretext-webwork.js
--rw-r--r--  2.0 unx    37123 b- defN 24-Mar-02 06:14 js/pretext-webwork/2.16/pretext-webwork.js
--rw-r--r--  2.0 unx    44152 b- defN 24-Mar-02 06:14 js/pretext-webwork/2.17/pretext-webwork.js
--rw-r--r--  2.0 unx     1180 b- defN 24-Mar-02 06:14 schema/README.md
--rw-r--r--  2.0 unx     3135 b- defN 24-Mar-02 06:14 schema/build.sh
--rw-r--r--  2.0 unx   103777 b- defN 24-Mar-02 06:14 schema/pretext.rng
--rw-r--r--  2.0 unx   127312 b- defN 24-Mar-02 06:14 schema/pretext.xsd
--rw-r--r--  2.0 unx    17572 b- defN 24-Mar-02 06:14 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx    18421 b- defN 24-Mar-02 06:14 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    58885 b- defN 24-Mar-02 06:14 schema/pretext.rnc
--rw-r--r--  2.0 unx    25870 b- defN 24-Mar-02 06:14 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx      326 b- defN 24-Mar-02 06:14 schema/xml.xsd
--rw-r--r--  2.0 unx    34176 b- defN 24-Mar-02 06:14 schema/pretext-dev.rng
--rw-r--r--  2.0 unx      162 b- defN 24-Mar-02 06:14 schema/publication.xml
--rw-r--r--  2.0 unx   134640 b- defN 24-Mar-02 06:14 schema/pretext.xml
--rw-r--r--  2.0 unx     6674 b- defN 24-Mar-02 06:14 js_lib/jquery.espy.min.js
--rw-r--r--  2.0 unx     1390 b- defN 24-Mar-02 06:14 js_lib/mathjaxknowl3.js
--rw-r--r--  2.0 unx    12611 b- defN 24-Mar-02 06:14 js_lib/knowl.js
--rw-r--r--  2.0 unx    86927 b- defN 24-Mar-02 06:14 js_lib/jquery.min.js
--rw-r--r--  2.0 unx     3177 b- defN 24-Mar-02 06:14 js_lib/mathjaxknowl.js
--rw-r--r--  2.0 unx     5275 b- defN 24-Mar-02 06:14 js_lib/jquery.sticky.js
--rw-r--r--  2.0 unx     8496 b- defN 24-Mar-02 06:14 css/shell_crc.css
--rw-r--r--  2.0 unx     1255 b- defN 24-Mar-02 06:14 css/colors_focused_gray_aqua.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     1683 b- defN 24-Mar-02 06:14 css/catalog.css
--rw-r--r--  2.0 unx      691 b- defN 24-Mar-02 06:14 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     1280 b- defN 24-Mar-02 06:14 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     6966 b- defN 24-Mar-02 06:14 css/navbar_crc.css
--rw-r--r--  2.0 unx     1330 b- defN 24-Mar-02 06:14 css/reveal.css
--rw-r--r--  2.0 unx     3769 b- defN 24-Mar-02 06:14 css/navbar_default.css
--rw-r--r--  2.0 unx     5374 b- defN 24-Mar-02 06:14 css/shell_default.css
--rw-r--r--  2.0 unx    24707 b- defN 24-Mar-02 06:14 css/pretext.css
--rw-r--r--  2.0 unx      389 b- defN 24-Mar-02 06:14 css/banner_wide.css
--rw-r--r--  2.0 unx    13638 b- defN 24-Mar-02 06:14 css/style_oscarlevin.css
--rw-r--r--  2.0 unx      533 b- defN 24-Mar-02 06:14 css/toc_wide.css
--rw-r--r--  2.0 unx     3757 b- defN 24-Mar-02 06:14 css/colors_blue_red_dark.css
--rw-r--r--  2.0 unx     1276 b- defN 24-Mar-02 06:14 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2446 b- defN 24-Mar-02 06:14 css/colors_martiansands.css
--rw-r--r--  2.0 unx     8179 b- defN 24-Mar-02 06:14 css/style_default.css
--rw-r--r--  2.0 unx     2781 b- defN 24-Mar-02 06:14 css/colors_default.css
--rw-r--r--  2.0 unx     1804 b- defN 24-Mar-02 06:14 css/knowls_default.css
--rw-r--r--  2.0 unx     3473 b- defN 24-Mar-02 06:14 css/style_soundwriting.css
--rw-r--r--  2.0 unx     4308 b- defN 24-Mar-02 06:14 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2720 b- defN 24-Mar-02 06:14 css/pretext_search.css
--rw-r--r--  2.0 unx     2441 b- defN 24-Mar-02 06:14 css/kindle.css
--rw-r--r--  2.0 unx      679 b- defN 24-Mar-02 06:14 css/navbar_wide.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     4236 b- defN 24-Mar-02 06:14 css/style_wide.css
--rw-r--r--  2.0 unx     6012 b- defN 24-Mar-02 06:14 css/features.css
--rw-r--r--  2.0 unx     4348 b- defN 24-Mar-02 06:14 css/colors_bluegreen_grey.css
--rw-r--r--  2.0 unx     3240 b- defN 24-Mar-02 06:14 css/banner_default.css
--rw-r--r--  2.0 unx     8096 b- defN 24-Mar-02 06:14 css/toc_crc.css
--rw-r--r--  2.0 unx     2438 b- defN 24-Mar-02 06:14 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     1102 b- defN 24-Mar-02 06:14 css/webwork.css
--rw-r--r--  2.0 unx     5875 b- defN 24-Mar-02 06:14 css/banner_crc.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx    14207 b- defN 24-Mar-02 06:14 css/setcolors.css
--rw-r--r--  2.0 unx     1207 b- defN 24-Mar-02 06:14 css/colors_focused_light.css
--rw-r--r--  2.0 unx     5836 b- defN 24-Mar-02 06:14 css/shell_min.css
--rw-r--r--  2.0 unx    74960 b- defN 24-Mar-02 06:14 css/pretext_add_on.css
--rw-r--r--  2.0 unx    10602 b- defN 24-Mar-02 06:14 css/edit.css
--rw-r--r--  2.0 unx     2446 b- defN 24-Mar-02 06:14 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     1338 b- defN 24-Mar-02 06:14 css/colors_red_blue.css
--rw-r--r--  2.0 unx     1362 b- defN 24-Mar-02 06:14 css/epub.css
--rw-r--r--  2.0 unx     9821 b- defN 24-Mar-02 06:14 css/toc_default.css
--rw-r--r--  2.0 unx     7521 b- defN 24-Mar-02 06:14 css/shell_wide.css
--rw-r--r--  2.0 unx     3818 b- defN 24-Mar-02 06:14 css/toc_min.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_green_blue.css
-192 files, 5172184 bytes uncompressed, 1092489 bytes compressed:  78.9%
+Zip file size: 1129799 bytes, number of entries: 194
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 css/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 js/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 js_lib/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 script/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 xsl/utilities/
+-rw-r--r--  2.0 unx   608815 b- defN 24-May-02 01:59 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     8134 b- defN 24-May-02 01:59 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 24-May-02 01:59 xsl/README.md
+-rw-r--r--  2.0 unx     2248 b- defN 24-May-02 01:59 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx   552864 b- defN 24-May-02 01:59 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 24-May-02 01:59 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx   138087 b- defN 24-May-02 01:59 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx    44062 b- defN 24-May-02 01:59 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 24-May-02 01:59 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     2734 b- defN 24-May-02 01:59 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 24-May-02 01:59 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 24-May-02 01:59 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    13189 b- defN 24-May-02 01:59 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 24-May-02 01:59 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 24-May-02 01:59 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx     2847 b- defN 24-May-02 01:59 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    19092 b- defN 24-May-02 01:59 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 24-May-02 01:59 xsl/entities.ent
+-rw-r--r--  2.0 unx    17295 b- defN 24-May-02 01:59 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 24-May-02 01:59 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx    22094 b- defN 24-May-02 01:59 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    95377 b- defN 24-May-02 01:59 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     8783 b- defN 24-May-02 01:59 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx   132279 b- defN 24-May-02 01:59 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 24-May-02 01:59 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx   120690 b- defN 24-May-02 01:59 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 24-May-02 01:59 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 24-May-02 01:59 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 24-May-02 01:59 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx   173803 b- defN 24-May-02 01:59 xsl/html-symbols.xsl
+-rw-r--r--  2.0 unx   235477 b- defN 24-May-02 01:59 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   551514 b- defN 24-May-02 01:59 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    67630 b- defN 24-May-02 01:59 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 24-May-02 01:59 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 24-May-02 01:59 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 24-May-02 01:59 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx    40687 b- defN 24-May-02 01:59 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 24-May-02 01:59 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 24-May-02 01:59 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 24-May-02 01:59 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    14322 b- defN 24-May-02 01:59 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 24-May-02 01:59 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 24-May-02 01:59 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-02 01:59 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 24-May-02 01:59 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     4810 b- defN 24-May-02 01:59 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    16378 b- defN 24-May-02 01:59 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    16151 b- defN 24-May-02 01:59 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    17147 b- defN 24-May-02 01:59 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    19076 b- defN 24-May-02 01:59 xsl/localizations/zh-HANS.xml
+-rw-r--r--  2.0 unx    20546 b- defN 24-May-02 01:59 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    16318 b- defN 24-May-02 01:59 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx     2347 b- defN 24-May-02 01:59 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    17122 b- defN 24-May-02 01:59 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    15924 b- defN 24-May-02 01:59 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    17368 b- defN 24-May-02 01:59 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    15648 b- defN 24-May-02 01:59 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17297 b- defN 24-May-02 01:59 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    19453 b- defN 24-May-02 01:59 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    16600 b- defN 24-May-02 01:59 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    19251 b- defN 24-May-02 01:59 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16415 b- defN 24-May-02 01:59 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16566 b- defN 24-May-02 01:59 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    16904 b- defN 24-May-02 01:59 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    30257 b- defN 24-May-02 01:59 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 24-May-02 01:59 xsl/utilities/README.md
+-rw-r--r--  2.0 unx     4926 b- defN 24-May-02 01:59 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      787 b- defN 24-May-02 01:59 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx      513 b- defN 24-May-02 01:59 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 24-May-02 01:59 xsl/utilities/author-report.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 24-May-02 01:59 xsl/support/README.md
+-rw-r--r--  2.0 unx     5061 b- defN 24-May-02 01:59 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx      522 b- defN 24-May-02 01:59 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5800 b- defN 24-May-02 01:59 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx    10300 b- defN 24-May-02 01:59 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 24-May-02 01:59 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 24-May-02 01:59 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 24-May-02 01:59 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 24-May-02 01:59 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 24-May-02 01:59 xsl/support/play-button/play-button.png
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 js/pretext-webwork/
+-rw-r--r--  2.0 unx    10957 b- defN 24-May-02 01:59 js/login.js
+-rw-r--r--  2.0 unx     3693 b- defN 24-May-02 01:59 js/ptx_search.js
+-rw-r--r--  2.0 unx     5318 b- defN 24-May-02 01:59 js/instructor.js
+-rw-r--r--  2.0 unx    42973 b- defN 24-May-02 01:59 js/pretext_add_on.js
+-rw-r--r--  2.0 unx    25633 b- defN 24-May-02 01:59 js/answer.js
+-rw-r--r--  2.0 unx    20911 b- defN 24-May-02 01:59 js/user_preferences.js
+-rw-r--r--  2.0 unx    12113 b- defN 24-May-02 01:59 js/pretext_search.js
+-rw-r--r--  2.0 unx   228054 b- defN 24-May-02 01:59 js/edit.js
+-rw-r--r--  2.0 unx     6509 b- defN 24-May-02 01:59 js/pretext.js
+-rw-r--r--  2.0 unx    23560 b- defN 24-May-02 01:59 js/highlight.js
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 js/pretext-webwork/2.16/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 js/pretext-webwork/2.17/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 js/pretext-webwork/2.18/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 js/pretext-webwork/2.19/
+-rw-r--r--  2.0 unx    37123 b- defN 24-May-02 01:59 js/pretext-webwork/2.16/pretext-webwork.js
+-rw-r--r--  2.0 unx    32570 b- defN 24-May-02 01:59 js/pretext-webwork/2.19/pretext-webwork.js
+-rw-r--r--  2.0 unx    44152 b- defN 24-May-02 01:59 js/pretext-webwork/2.17/pretext-webwork.js
+-rw-r--r--  2.0 unx    44152 b- defN 24-May-02 01:59 js/pretext-webwork/2.18/pretext-webwork.js
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:59 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 24-May-02 01:59 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 24-May-02 01:59 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 24-May-02 01:59 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 24-May-02 01:59 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 01:59 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 24-May-02 01:59 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx    24707 b- defN 24-May-02 01:59 css/pretext.css
+-rw-r--r--  2.0 unx     1280 b- defN 24-May-02 01:59 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-02 01:59 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-02 01:59 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-02 01:59 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     1804 b- defN 24-May-02 01:59 css/knowls_default.css
+-rw-r--r--  2.0 unx     4348 b- defN 24-May-02 01:59 css/colors_bluegreen_grey.css
+-rw-r--r--  2.0 unx    14207 b- defN 24-May-02 01:59 css/setcolors.css
+-rw-r--r--  2.0 unx     8179 b- defN 24-May-02 01:59 css/style_default.css
+-rw-r--r--  2.0 unx     7521 b- defN 24-May-02 01:59 css/shell_wide.css
+-rw-r--r--  2.0 unx     1102 b- defN 24-May-02 01:59 css/webwork.css
+-rw-r--r--  2.0 unx     2446 b- defN 24-May-02 01:59 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     6012 b- defN 24-May-02 01:59 css/features.css
+-rw-r--r--  2.0 unx     3757 b- defN 24-May-02 01:59 css/colors_blue_red_dark.css
+-rw-r--r--  2.0 unx     3818 b- defN 24-May-02 01:59 css/toc_min.css
+-rw-r--r--  2.0 unx    10602 b- defN 24-May-02 01:59 css/edit.css
+-rw-r--r--  2.0 unx      533 b- defN 24-May-02 01:59 css/toc_wide.css
+-rw-r--r--  2.0 unx     1276 b- defN 24-May-02 01:59 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     1207 b- defN 24-May-02 01:59 css/colors_focused_light.css
+-rw-r--r--  2.0 unx    74960 b- defN 24-May-02 01:59 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     2720 b- defN 24-May-02 01:59 css/pretext_search.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-02 01:59 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx      679 b- defN 24-May-02 01:59 css/navbar_wide.css
+-rw-r--r--  2.0 unx     4236 b- defN 24-May-02 01:59 css/style_wide.css
+-rw-r--r--  2.0 unx     8496 b- defN 24-May-02 01:59 css/shell_crc.css
+-rw-r--r--  2.0 unx     1683 b- defN 24-May-02 01:59 css/catalog.css
+-rw-r--r--  2.0 unx      389 b- defN 24-May-02 01:59 css/banner_wide.css
+-rw-r--r--  2.0 unx     5875 b- defN 24-May-02 01:59 css/banner_crc.css
+-rw-r--r--  2.0 unx     2441 b- defN 24-May-02 01:59 css/kindle.css
+-rw-r--r--  2.0 unx     5374 b- defN 24-May-02 01:59 css/shell_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-02 01:59 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     1338 b- defN 24-May-02 01:59 css/colors_red_blue.css
+-rw-r--r--  2.0 unx    13638 b- defN 24-May-02 01:59 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx      691 b- defN 24-May-02 01:59 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     1330 b- defN 24-May-02 01:59 css/reveal.css
+-rw-r--r--  2.0 unx     1362 b- defN 24-May-02 01:59 css/epub.css
+-rw-r--r--  2.0 unx     3769 b- defN 24-May-02 01:59 css/navbar_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-02 01:59 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     9821 b- defN 24-May-02 01:59 css/toc_default.css
+-rw-r--r--  2.0 unx     2781 b- defN 24-May-02 01:59 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-02 01:59 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     1255 b- defN 24-May-02 01:59 css/colors_focused_gray_aqua.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-02 01:59 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     3240 b- defN 24-May-02 01:59 css/banner_default.css
+-rw-r--r--  2.0 unx     6966 b- defN 24-May-02 01:59 css/navbar_crc.css
+-rw-r--r--  2.0 unx     4308 b- defN 24-May-02 01:59 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     3473 b- defN 24-May-02 01:59 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     2446 b- defN 24-May-02 01:59 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     8096 b- defN 24-May-02 01:59 css/toc_crc.css
+-rw-r--r--  2.0 unx     5836 b- defN 24-May-02 01:59 css/shell_min.css
+-rw-r--r--  2.0 unx     1367 b- defN 24-May-02 01:59 pretext/README.md
+-rw-r--r--  2.0 unx   185418 b- defN 24-May-02 01:59 pretext/pretext.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 01:59 pretext/__init__.py
+-rw-r--r--  2.0 unx    30970 b- defN 24-May-02 01:59 pretext/pretext
+-rw-r--r--  2.0 unx      215 b- defN 24-May-02 01:59 pretext/requirements.txt
+-rw-r--r--  2.0 unx     1955 b- defN 24-May-02 01:59 pretext/module-test.py
+-rw-r--r--  2.0 unx    36176 b- defN 24-May-02 01:59 pretext/braille_format.py
+-rw-r--r--  2.0 unx     2566 b- defN 24-May-02 01:59 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     6674 b- defN 24-May-02 01:59 js_lib/jquery.espy.min.js
+-rw-r--r--  2.0 unx    12611 b- defN 24-May-02 01:59 js_lib/knowl.js
+-rw-r--r--  2.0 unx     5275 b- defN 24-May-02 01:59 js_lib/jquery.sticky.js
+-rw-r--r--  2.0 unx    86927 b- defN 24-May-02 01:59 js_lib/jquery.min.js
+-rw-r--r--  2.0 unx     1390 b- defN 24-May-02 01:59 js_lib/mathjaxknowl3.js
+-rw-r--r--  2.0 unx     3177 b- defN 24-May-02 01:59 js_lib/mathjaxknowl.js
+-rw-r--r--  2.0 unx     1180 b- defN 24-May-02 01:59 schema/README.md
+-rw-r--r--  2.0 unx     3135 b- defN 24-May-02 01:59 schema/build.sh
+-rw-r--r--  2.0 unx   107306 b- defN 24-May-02 01:59 schema/pretext.rng
+-rw-r--r--  2.0 unx   129207 b- defN 24-May-02 01:59 schema/pretext.xsd
+-rw-r--r--  2.0 unx    39988 b- defN 24-May-02 01:59 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx   140214 b- defN 24-May-02 01:59 schema/pretext.xml
+-rw-r--r--  2.0 unx    21415 b- defN 24-May-02 01:59 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx    25870 b- defN 24-May-02 01:59 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx      162 b- defN 24-May-02 01:59 schema/publication.xml
+-rw-r--r--  2.0 unx    60821 b- defN 24-May-02 01:59 schema/pretext.rnc
+-rw-r--r--  2.0 unx      326 b- defN 24-May-02 01:59 schema/xml.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 24-May-02 01:59 schema/pretext-schematron.xsl
+194 files, 5244197 bytes uncompressed, 1106101 bytes compressed:  78.9%
```

#### zipnote {}

```diff
@@ -27,551 +27,557 @@
 
 Filename: xsl/support/
 Comment: 
 
 Filename: xsl/utilities/
 Comment: 
 
-Filename: xsl/README.md
+Filename: xsl/pretext-html.xsl
 Comment: 
 
-Filename: xsl/extract-trace.xsl
+Filename: xsl/extract-sageplot.xsl
 Comment: 
 
-Filename: xsl/pretext-json-manifest.xsl
+Filename: xsl/README.md
 Comment: 
 
-Filename: xsl/pretext-solution-manual-latex.xsl
+Filename: xsl/extract-mom.xsl
 Comment: 
 
-Filename: xsl/pretext-ww-problem-sets.xsl
+Filename: xsl/pretext-common.xsl
 Comment: 
 
 Filename: xsl/pretext-jupyter.xsl
 Comment: 
 
-Filename: xsl/pretext-smc.xsl
-Comment: 
-
-Filename: xsl/publisher-variables.xsl
+Filename: xsl/extract-pg.xsl
 Comment: 
 
-Filename: xsl/html-symbols.xsl
+Filename: xsl/pretext-text-utilities.xsl
 Comment: 
 
-Filename: xsl/extract-mom.xsl
+Filename: xsl/extract-youtube.xsl
 Comment: 
 
-Filename: xsl/pretext-assembly.xsl
+Filename: xsl/extract-asymptote.xsl
 Comment: 
 
-Filename: xsl/pretext-revealjs.xsl
+Filename: xsl/pretext-beamer.xsl
 Comment: 
 
-Filename: xsl/pretext-view-source.xsl
+Filename: xsl/pretext-basic-html.xsl
 Comment: 
 
-Filename: xsl/pretext-sage-doctest.xsl
+Filename: xsl/pretext-solution-manual-latex.xsl
 Comment: 
 
-Filename: xsl/extract-identity.xsl
+Filename: xsl/pretext-smc.xsl
 Comment: 
 
-Filename: xsl/entities.ent
+Filename: xsl/pretext-json-manifest.xsl
 Comment: 
 
 Filename: xsl/extract-datafile.xsl
 Comment: 
 
-Filename: xsl/pretext-epub.xsl
+Filename: xsl/extract-latex-image.xsl
 Comment: 
 
-Filename: xsl/pretext-merge.xsl
+Filename: xsl/entities.ent
 Comment: 
 
-Filename: xsl/pretext-beamer.xsl
+Filename: xsl/pretext-ww-problem-sets.xsl
 Comment: 
 
-Filename: xsl/extract-youtube.xsl
+Filename: xsl/pretext-units.xsl
 Comment: 
 
-Filename: xsl/extract-qrcode.xsl
+Filename: xsl/pretext-revealjs.xsl
 Comment: 
 
-Filename: xsl/extract-asymptote.xsl
+Filename: xsl/pretext-braille-preprint.xsl
 Comment: 
 
-Filename: xsl/extract-latex-image.xsl
+Filename: xsl/pretext-view-source.xsl
 Comment: 
 
-Filename: xsl/pretext-basic-html.xsl
+Filename: xsl/pretext-assembly.xsl
 Comment: 
 
-Filename: xsl/pretext-units.xsl
+Filename: xsl/extract-trace.xsl
 Comment: 
 
-Filename: xsl/pretext-braille-preprint.xsl
+Filename: xsl/pretext-runestone.xsl
 Comment: 
 
 Filename: xsl/pretext-litprog.xsl
 Comment: 
 
-Filename: xsl/extract-interactive.xsl
+Filename: xsl/pretext-text.xsl
 Comment: 
 
-Filename: xsl/extract-sageplot.xsl
+Filename: xsl/extract-qrcode.xsl
 Comment: 
 
-Filename: xsl/pretext-html.xsl
+Filename: xsl/html-symbols.xsl
 Comment: 
 
-Filename: xsl/extract-pg.xsl
+Filename: xsl/publisher-variables.xsl
 Comment: 
 
-Filename: xsl/pretext-text.xsl
+Filename: xsl/pretext-latex.xsl
 Comment: 
 
-Filename: xsl/pretext-text-utilities.xsl
+Filename: xsl/pretext-epub.xsl
 Comment: 
 
 Filename: xsl/pretext-numbers.xsl
 Comment: 
 
-Filename: xsl/pretext-latex.xsl
+Filename: xsl/pretext-merge.xsl
 Comment: 
 
-Filename: xsl/xml-to-json.xsl
+Filename: xsl/extract-identity.xsl
 Comment: 
 
 Filename: xsl/pretext-runestone-static.xsl
 Comment: 
 
-Filename: xsl/pretext-runestone.xsl
+Filename: xsl/pretext-sage-doctest.xsl
 Comment: 
 
-Filename: xsl/pretext-common.xsl
+Filename: xsl/xml-to-json.xsl
 Comment: 
 
-Filename: xsl/localizations/README.md
+Filename: xsl/extract-interactive.xsl
 Comment: 
 
-Filename: xsl/localizations/pt-BR.xml
+Filename: xsl/latex/pretext-latex-chaos.xsl
 Comment: 
 
-Filename: xsl/localizations/fr-CA.xml
+Filename: xsl/latex/pretext-latex-guide.xsl
 Comment: 
 
-Filename: xsl/localizations/it-IT.xml
+Filename: xsl/latex/pretext-latex-AIM.xsl
 Comment: 
 
-Filename: xsl/localizations/cs-CZ.xml
+Filename: xsl/latex/pretext-latex-CLP.xsl
 Comment: 
 
-Filename: xsl/localizations/pt-PT.xml
+Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
 Comment: 
 
-Filename: xsl/localizations/af-ZA.xml
+Filename: xsl/localizations/README.md
 Comment: 
 
-Filename: xsl/localizations/nl-NL.xml
+Filename: xsl/localizations/pt-BR.xml
 Comment: 
 
 Filename: xsl/localizations/hu-HU.xml
 Comment: 
 
-Filename: xsl/localizations/fr-FR.xml
+Filename: xsl/localizations/pt-PT.xml
 Comment: 
 
-Filename: xsl/localizations/de-DE.xml
+Filename: xsl/localizations/zh-HANS.xml
 Comment: 
 
 Filename: xsl/localizations/ku-CKB.xml
 Comment: 
 
-Filename: xsl/localizations/zh-HANS.xml
+Filename: xsl/localizations/ca-ES.xml
+Comment: 
+
+Filename: xsl/localizations/localizations.xml
 Comment: 
 
 Filename: xsl/localizations/bg-BG.xml
 Comment: 
 
-Filename: xsl/localizations/es-ES.xml
+Filename: xsl/localizations/it-IT.xml
 Comment: 
 
 Filename: xsl/localizations/fi-FI.xml
 Comment: 
 
-Filename: xsl/localizations/localizations.xml
+Filename: xsl/localizations/cs-CZ.xml
 Comment: 
 
-Filename: xsl/localizations/en-US.xml
+Filename: xsl/localizations/de-DE.xml
 Comment: 
 
-Filename: xsl/localizations/ca-ES.xml
+Filename: xsl/localizations/en-US.xml
 Comment: 
 
-Filename: xsl/utilities/README.md
+Filename: xsl/localizations/es-ES.xml
 Comment: 
 
-Filename: xsl/utilities/author-report.xsl
+Filename: xsl/localizations/nl-NL.xml
 Comment: 
 
-Filename: xsl/utilities/pretext-enhanced-source.xsl
+Filename: xsl/localizations/fr-FR.xml
 Comment: 
 
-Filename: xsl/utilities/deprecate-index.sed
+Filename: xsl/localizations/fr-CA.xml
 Comment: 
 
-Filename: xsl/utilities/fix-deprecations.xsl
+Filename: xsl/localizations/af-ZA.xml
 Comment: 
 
-Filename: xsl/utilities/deprecate-autoname.sed
+Filename: xsl/utilities/fix-deprecations.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-chaos.xsl
+Filename: xsl/utilities/README.md
 Comment: 
 
-Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
+Filename: xsl/utilities/pretext-enhanced-source.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-CLP.xsl
+Filename: xsl/utilities/deprecate-index.sed
 Comment: 
 
-Filename: xsl/latex/pretext-latex-guide.xsl
+Filename: xsl/utilities/deprecate-autoname.sed
 Comment: 
 
-Filename: xsl/latex/pretext-latex-AIM.xsl
+Filename: xsl/utilities/author-report.xsl
 Comment: 
 
 Filename: xsl/support/play-button/
 Comment: 
 
 Filename: xsl/support/README.md
 Comment: 
 
-Filename: xsl/support/extract-math.xsl
+Filename: xsl/support/extract-latex-image-labels.xsl
 Comment: 
 
-Filename: xsl/support/pretext-pg-macros.xsl
+Filename: xsl/support/runestone-services.xml
 Comment: 
 
-Filename: xsl/support/package-math.xsl
+Filename: xsl/support/tactile-svg.xsl
 Comment: 
 
-Filename: xsl/support/extract-latex-image-labels.xsl
+Filename: xsl/support/extract-math.xsl
 Comment: 
 
-Filename: xsl/support/tactile-svg.xsl
+Filename: xsl/support/package-math.xsl
 Comment: 
 
-Filename: xsl/support/runestone-services.xml
+Filename: xsl/support/pretext-pg-macros.xsl
 Comment: 
 
 Filename: xsl/support/play-button/README.md
 Comment: 
 
 Filename: xsl/support/play-button/play-button.svg
 Comment: 
 
 Filename: xsl/support/play-button/play-button.png
 Comment: 
 
-Filename: script/mjsre/
+Filename: js/pretext-webwork/
 Comment: 
 
-Filename: script/README.md
+Filename: js/login.js
 Comment: 
 
-Filename: script/mbx
+Filename: js/ptx_search.js
 Comment: 
 
-Filename: script/mjsre/README.md
+Filename: js/instructor.js
 Comment: 
 
-Filename: script/mjsre/update-sre
+Filename: js/pretext_add_on.js
 Comment: 
 
-Filename: script/mjsre/package.json
+Filename: js/answer.js
 Comment: 
 
-Filename: script/mjsre/mj-sre-page.js
+Filename: js/user_preferences.js
 Comment: 
 
-Filename: pretext/README.md
+Filename: js/pretext_search.js
 Comment: 
 
-Filename: pretext/braille_format.py
+Filename: js/edit.js
 Comment: 
 
-Filename: pretext/module-test.py
+Filename: js/pretext.js
 Comment: 
 
-Filename: pretext/pretext.py
+Filename: js/highlight.js
 Comment: 
 
-Filename: pretext/requirements.txt
+Filename: js/pretext-webwork/2.16/
 Comment: 
 
-Filename: pretext/pretext
+Filename: js/pretext-webwork/2.17/
 Comment: 
 
-Filename: pretext/pretext.cfg
+Filename: js/pretext-webwork/2.18/
 Comment: 
 
-Filename: pretext/__init__.py
+Filename: js/pretext-webwork/2.19/
 Comment: 
 
-Filename: js/pretext-webwork/
+Filename: js/pretext-webwork/2.16/pretext-webwork.js
 Comment: 
 
-Filename: js/pretext_add_on.js
+Filename: js/pretext-webwork/2.19/pretext-webwork.js
 Comment: 
 
-Filename: js/login.js
+Filename: js/pretext-webwork/2.17/pretext-webwork.js
 Comment: 
 
-Filename: js/pretext.js
+Filename: js/pretext-webwork/2.18/pretext-webwork.js
 Comment: 
 
-Filename: js/edit.js
+Filename: script/mjsre/
 Comment: 
 
-Filename: js/pretext_search.js
+Filename: script/README.md
 Comment: 
 
-Filename: js/instructor.js
+Filename: script/mbx
 Comment: 
 
-Filename: js/answer.js
+Filename: script/mjsre/README.md
 Comment: 
 
-Filename: js/ptx_search.js
+Filename: script/mjsre/package.json
 Comment: 
 
-Filename: js/highlight.js
+Filename: script/mjsre/update-sre
 Comment: 
 
-Filename: js/user_preferences.js
+Filename: script/mjsre/mj-sre-page.js
 Comment: 
 
-Filename: js/pretext-webwork/2.16/
+Filename: css/pretext.css
 Comment: 
 
-Filename: js/pretext-webwork/2.17/
+Filename: css/colors_brown_gold.css
 Comment: 
 
-Filename: js/pretext-webwork/2.18/
+Filename: css/colors_green_blue.css
 Comment: 
 
-Filename: js/pretext-webwork/2.18/pretext-webwork.js
+Filename: css/colors_ruby_emerald.css
 Comment: 
 
-Filename: js/pretext-webwork/2.16/pretext-webwork.js
+Filename: css/colors_ruby_amethyst.css
 Comment: 
 
-Filename: js/pretext-webwork/2.17/pretext-webwork.js
+Filename: css/knowls_default.css
 Comment: 
 
-Filename: schema/README.md
+Filename: css/colors_bluegreen_grey.css
 Comment: 
 
-Filename: schema/build.sh
+Filename: css/setcolors.css
 Comment: 
 
-Filename: schema/pretext.rng
+Filename: css/style_default.css
 Comment: 
 
-Filename: schema/pretext.xsd
+Filename: css/shell_wide.css
 Comment: 
 
-Filename: schema/pretext-dev.rnc
+Filename: css/webwork.css
 Comment: 
 
-Filename: schema/pretext-schematron.xsl
+Filename: css/colors_martiansands.css
 Comment: 
 
-Filename: schema/pretext.rnc
+Filename: css/features.css
 Comment: 
 
-Filename: schema/pretext-validation-plus.xsl
+Filename: css/colors_blue_red_dark.css
 Comment: 
 
-Filename: schema/xml.xsd
+Filename: css/toc_min.css
 Comment: 
 
-Filename: schema/pretext-dev.rng
+Filename: css/edit.css
 Comment: 
 
-Filename: schema/publication.xml
+Filename: css/toc_wide.css
 Comment: 
 
-Filename: schema/pretext.xml
+Filename: css/colors_maroon_grey.css
 Comment: 
 
-Filename: js_lib/jquery.espy.min.js
+Filename: css/colors_focused_light.css
 Comment: 
 
-Filename: js_lib/mathjaxknowl3.js
+Filename: css/pretext_add_on.css
 Comment: 
 
-Filename: js_lib/knowl.js
+Filename: css/pretext_search.css
 Comment: 
 
-Filename: js_lib/jquery.min.js
+Filename: css/colors_orange_navy.css
 Comment: 
 
-Filename: js_lib/mathjaxknowl.js
+Filename: css/navbar_wide.css
 Comment: 
 
-Filename: js_lib/jquery.sticky.js
+Filename: css/style_wide.css
 Comment: 
 
 Filename: css/shell_crc.css
 Comment: 
 
-Filename: css/colors_focused_gray_aqua.css
+Filename: css/catalog.css
 Comment: 
 
-Filename: css/colors_orange_navy.css
+Filename: css/banner_wide.css
 Comment: 
 
-Filename: css/colors_ruby_emerald.css
+Filename: css/banner_crc.css
 Comment: 
 
-Filename: css/catalog.css
+Filename: css/kindle.css
 Comment: 
 
-Filename: css/colors_pastel_blue_orange.css
+Filename: css/shell_default.css
 Comment: 
 
-Filename: css/colors_brown_gold.css
+Filename: css/colors_blue_grey.css
 Comment: 
 
-Filename: css/navbar_crc.css
+Filename: css/colors_red_blue.css
 Comment: 
 
-Filename: css/reveal.css
+Filename: css/style_oscarlevin.css
 Comment: 
 
-Filename: css/navbar_default.css
+Filename: css/colors_pastel_blue_orange.css
 Comment: 
 
-Filename: css/shell_default.css
+Filename: css/reveal.css
 Comment: 
 
-Filename: css/pretext.css
+Filename: css/epub.css
 Comment: 
 
-Filename: css/banner_wide.css
+Filename: css/navbar_default.css
 Comment: 
 
-Filename: css/style_oscarlevin.css
+Filename: css/colors_blue_red.css
 Comment: 
 
-Filename: css/toc_wide.css
+Filename: css/toc_default.css
 Comment: 
 
-Filename: css/colors_blue_red_dark.css
+Filename: css/colors_default.css
 Comment: 
 
-Filename: css/colors_maroon_grey.css
+Filename: css/colors_green_plum.css
 Comment: 
 
-Filename: css/colors_blue_red.css
+Filename: css/colors_focused_gray_aqua.css
 Comment: 
 
-Filename: css/colors_martiansands.css
+Filename: css/colors_ruby_turquoise.css
 Comment: 
 
-Filename: css/style_default.css
+Filename: css/banner_default.css
 Comment: 
 
-Filename: css/colors_default.css
+Filename: css/navbar_crc.css
 Comment: 
 
-Filename: css/knowls_default.css
+Filename: css/colors_blue_green.css
 Comment: 
 
 Filename: css/style_soundwriting.css
 Comment: 
 
-Filename: css/colors_blue_green.css
+Filename: css/colors_darkmartiansands.css
 Comment: 
 
-Filename: css/pretext_search.css
+Filename: css/toc_crc.css
 Comment: 
 
-Filename: css/kindle.css
+Filename: css/shell_min.css
 Comment: 
 
-Filename: css/navbar_wide.css
+Filename: pretext/README.md
 Comment: 
 
-Filename: css/colors_ruby_turquoise.css
+Filename: pretext/pretext.py
 Comment: 
 
-Filename: css/style_wide.css
+Filename: pretext/__init__.py
 Comment: 
 
-Filename: css/features.css
+Filename: pretext/pretext
 Comment: 
 
-Filename: css/colors_bluegreen_grey.css
+Filename: pretext/requirements.txt
 Comment: 
 
-Filename: css/banner_default.css
+Filename: pretext/module-test.py
 Comment: 
 
-Filename: css/toc_crc.css
+Filename: pretext/braille_format.py
 Comment: 
 
-Filename: css/colors_blue_grey.css
+Filename: pretext/pretext.cfg
 Comment: 
 
-Filename: css/webwork.css
+Filename: js_lib/jquery.espy.min.js
 Comment: 
 
-Filename: css/banner_crc.css
+Filename: js_lib/knowl.js
 Comment: 
 
-Filename: css/colors_green_plum.css
+Filename: js_lib/jquery.sticky.js
 Comment: 
 
-Filename: css/colors_ruby_amethyst.css
+Filename: js_lib/jquery.min.js
 Comment: 
 
-Filename: css/setcolors.css
+Filename: js_lib/mathjaxknowl3.js
 Comment: 
 
-Filename: css/colors_focused_light.css
+Filename: js_lib/mathjaxknowl.js
 Comment: 
 
-Filename: css/shell_min.css
+Filename: schema/README.md
 Comment: 
 
-Filename: css/pretext_add_on.css
+Filename: schema/build.sh
 Comment: 
 
-Filename: css/edit.css
+Filename: schema/pretext.rng
 Comment: 
 
-Filename: css/colors_darkmartiansands.css
+Filename: schema/pretext.xsd
 Comment: 
 
-Filename: css/colors_red_blue.css
+Filename: schema/pretext-dev.rng
 Comment: 
 
-Filename: css/epub.css
+Filename: schema/pretext.xml
 Comment: 
 
-Filename: css/toc_default.css
+Filename: schema/pretext-dev.rnc
 Comment: 
 
-Filename: css/shell_wide.css
+Filename: schema/pretext-validation-plus.xsl
 Comment: 
 
-Filename: css/toc_min.css
+Filename: schema/publication.xml
 Comment: 
 
-Filename: css/colors_green_blue.css
+Filename: schema/pretext.rnc
+Comment: 
+
+Filename: schema/xml.xsd
+Comment: 
+
+Filename: schema/pretext-schematron.xsl
 Comment: 
 
 Zip file comment:
```

#### xsl/pretext-assembly.xsl

##### xsl/pretext-assembly.xsl

```diff
@@ -17,15 +17,15 @@
 You should have received a copy of the GNU General Public License
 along with PreTeXt.  If not, see <http://www.gnu.org/licenses/>.
 *********************************************************************-->
 <!DOCTYPE stylesheet [
     <!ENTITY % entities SYSTEM "entities.ent">
     %entities;
 ]>
-<xsl:stylesheet xmlns:xsl="http://www.w3.org/1999/XSL/Transform" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xhtml="http://www.w3.org/1999/xhtml" xmlns:pi="http://pretextbook.org/2020/pretext/internal" xmlns:exsl="http://exslt.org/common" xmlns:date="http://exslt.org/dates-and-times" version="1.0" extension-element-prefixes="exsl date" exclude-result-prefixes="pi">
+<xsl:stylesheet xmlns:xsl="http://www.w3.org/1999/XSL/Transform" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xhtml="http://www.w3.org/1999/xhtml" xmlns:pi="http://pretextbook.org/2020/pretext/internal" xmlns:exsl="http://exslt.org/common" xmlns:date="http://exslt.org/dates-and-times" xmlns:str="http://exslt.org/strings" version="1.0" extension-element-prefixes="exsl date str" exclude-result-prefixes="pi">
   <!-- This is the once-mythical pre-processor, though we prefer     -->
   <!-- to describe it as the "assembly" of "enhanced" source.  By    -->
   <!-- "assembly" we mean pre-processing of source, by "assembling"  -->
   <!-- various pieces of material or content, authored or computed,  -->
   <!-- into an enhanced source tree. This template operates by       -->
   <!-- successive passes through the entire source tree making       -->
   <!-- adjustments into a new "enhanced" or modified source tree     -->
@@ -81,14 +81,24 @@
   <!-- such as locations of customizations or private solutions,     -->
   <!-- are needed early in assembly, while other variables, such     -->
   <!-- as options for numbering, are needed for later enhancements   -->
   <!-- to the source.  If new code results in undefined, or          -->
   <!-- recursively defined, variables, this discussion may be        -->
   <!-- relevant.  (This is repeated verbatim in the other            -->
   <!-- stylesheet).                                                  -->
+  <!--  -->
+  <!-- Note too, that we want this stylesheet to be independent, and -->
+  <!-- that can be tested with the  pretext-enhanced-source.xsl      -->
+  <!-- stylesheet.  There is one danger: any (modal) template        -->
+  <!-- applied here, needs to be defined here.  "Normal" conversions -->
+  <!-- will import things like "pretext-common.xsl" and templates    -->
+  <!-- defined there will be available.  But when not defined here,  -->
+  <!-- the default is to just apply default templates to the         -->
+  <!-- content, which may generally just produce a lot of text.      -->
+  <!-- Which is no good, say as an attribute value.                  -->
   <!-- Isolate computation of numbers -->
   <xsl:import href="./pretext-numbers.xsl"/>
   <!-- Isolate conversion of Runestone/interactive to PreTeXt/static -->
   <xsl:import href="./pretext-runestone-static.xsl"/>
   <!-- We explicitly do not import "pretext-common.xsl" as we want    -->
   <!-- this important pre-processing stylesheet to have no hidden     -->
   <!-- dependencies.  In almost every rational use, the "-common"     -->
@@ -250,16 +260,23 @@
   <xsl:variable name="exercise-rtf">
     <!-- initialize with default, 'inline' -->
     <xsl:apply-templates select="$assembly" mode="exercise">
       <xsl:with-param name="division" select="'inline'"/>
     </xsl:apply-templates>
   </xsl:variable>
   <xsl:variable name="exercise" select="exsl:node-set($exercise-rtf)"/>
+  <xsl:variable name="assembly-label-rtf">
+    <xsl:apply-templates select="$exercise" mode="id-attribute">
+      <!-- $parent-id defaults to 'root' in template -->
+      <xsl:with-param name="attr-name" select="'assembly-id'"/>
+    </xsl:apply-templates>
+  </xsl:variable>
+  <xsl:variable name="assembly-label" select="exsl:node-set($assembly-label-rtf)"/>
   <xsl:variable name="representations-rtf">
-    <xsl:apply-templates select="$exercise" mode="representations"/>
+    <xsl:apply-templates select="$assembly-label" mode="representations"/>
   </xsl:variable>
   <xsl:variable name="representations" select="exsl:node-set($representations-rtf)"/>
   <!-- Dependency: "repair" will fix some exercise representations, -->
   <!-- especially coming from an "old" WeBWorK server, so the       -->
   <!-- "repair" pass must come after the "representations" pass.    -->
   <xsl:variable name="repair-rtf">
     <xsl:apply-templates select="$representations" mode="repair"/>
@@ -1052,35 +1069,68 @@
   <xsl:template match="paragraph" mode="repair"/>
   <!-- 2019-02-20  deprecated and killed simultaneously -->
   <xsl:template match="todo" mode="repair"/>
   <!-- A "pagebreak" should have had limited -->
   <!-- uptake, so no real care taken,        -->
   <!-- Deprecated 2021-03-17                 -->
   <xsl:template match="pagebreak" mode="repair"/>
+  <!-- ########### -->
+  <!-- Assembly ID -->
+  <!-- ########### -->
   <!-- Some maniulations of source require stable identification *before*     -->
   <!-- we assign @unique-id values for general use in the very late           -->
-  <!-- "identification" phase.  This is a role for the "original-id" which    -->
-  <!-- is formed based soley on the author's source (which may get versioned, -->
-  <!-- customized, repaired, etc.).  It should suffice for "big" objects      -->
+  <!-- "identification" phase.  This is a role for the "@assembly-id" which   -->
+  <!-- is formed after the author's source has been versioned, customized,    -->
+  <!-- repaired, but before replacements. It should suffice for "big" objects -->
   <!-- which are unlikely to change much (other than going away in a version) -->
   <!-- and may only be "repaired" in a one-to-one cosmetic rename.  We use    -->
   <!-- this sparingly, thus we are careful about the match, along with        -->
   <!-- documenting rationale for each object.                                 -->
   <!--                                                                        -->
   <!-- Another way to think about this is as an "early" id, versus the        -->
   <!-- more general "late" id.                                                -->
   <!--                                                                        -->
+  <!-- audio|video|interactive                                                -->
+  <!--     Static versions of these interactive elements have previews        -->
+  <!--     (YouTube thumbnails, automatically generated screenshots),         -->
+  <!--     generated QR codes, and various links meant for use in static      -->
+  <!--     contexts.  So we form names of these related objects based on      -->
+  <!--     an "earlier" id.                                                   -->
+  <!--                                                                        -->
   <!-- datafile                                                               -->
   <!--     For static versions of this Runestone component, when the file is  -->
   <!--     a text file provided in the external directory, we need to         -->
   <!--     interrogate the file manufactured in the generated directory in    -->
   <!--     order to make a sample of its content.  This happens before we     -->
   <!--     construct unique-id.                                               -->
+  <!-- NB: we believe the @assembly-id will equal the @unique-id    -->
+  <!-- ("visible-id" template) for objects at the level of blocks,  -->
+  <!-- and certainly for any object replaced by a different static  -->
+  <!-- representation.  But for generated objects, e.g. QR codes,   -->
+  <!-- it would be best if the generation process used the          -->
+  <!-- "assembly-id" template for guranteed consistency.  This *is* -->
+  <!-- being done for "datafile" but is technical debt otherwise.   -->
+  <!-- [Ed. this once prefaced the "visible-id-early" template, a weak  -->
+  <!-- forerunner of the "assembly-id" template.  But the commentary    -->
+  <!-- is still good, so we have preserved it here.]                    -->
+  <!-- This template produces identification that happens early in the  -->
+  <!-- passes this stylesheet executes.  The idea is that some elements -->
+  <!-- get replaced wholesale (such as an "interactive" being replaced  -->
+  <!-- by a "sidebyside" in the creation of a static precursor.  But we -->
+  <!-- want these ids, especially if automatic, to be consistent when   -->
+  <!-- used in derived versions (such as manufacturing, or displaying,  -->
+  <!-- a QR code file for a static "interactive").                      -->
+  <!-- NB: this template needs to be defined in this stylesheet, since  -->
+  <!-- we want the stylesheet to be independent, and the template is    -->
+  <!-- also applied here.                                               -->
+  <xsl:template match="audio|video|interactive" mode="assembly-id">
+    <xsl:value-of select="@assembly-id"/>
+  </xsl:template>
   <xsl:template match="datafile" mode="assembly-id">
-    <xsl:value-of select="@original-id"/>
+    <xsl:value-of select="@assembly-id"/>
   </xsl:template>
   <xsl:template match="*" mode="assembly-id">
     <xsl:message>PTX:BUG:  the &quot;assembly-id&quot; template was applied to an element it did not expect</xsl:message>
     <xsl:text>unexpected-assembly-id-template-use-here</xsl:text>
   </xsl:template>
   <!-- ############## -->
   <!-- Identification -->
@@ -1960,15 +2010,15 @@
         <xsl:when test="($exercise-style = 'dynamic') or ($exercise-style = 'pg-problems')">
           <!-- duplicate authored content for the non-static conversions -->
           <xsl:apply-templates select="node()" mode="representations"/>
         </xsl:when>
       </xsl:choose>
     </xsl:copy>
   </xsl:template>
-  <xsl:template match="datafile" mode="representations">
+  <xsl:template match="datafile|query" mode="representations">
     <xsl:choose>
       <!-- make a static version, in a PreTeXt style -->
       <!-- for use naturally by most conversions     -->
       <xsl:when test="$exercise-style = 'static'">
         <xsl:apply-templates select="." mode="runestone-to-static"/>
       </xsl:when>
       <!-- duplicate for a dynamic version -->
@@ -2014,25 +2064,25 @@
             <!-- video: we scrape YouTube, only           -->
             <!--        YouTube playlist gets generic     -->
             <!-- audio: immature                          -->
             <xsl:when test="self::interactive">
               <image>
                 <xsl:attribute name="pi:generated">
                   <xsl:text>preview/</xsl:text>
-                  <xsl:apply-templates select="." mode="visible-id-early"/>
+                  <xsl:apply-templates select="." mode="assembly-id"/>
                   <xsl:text>-preview.png</xsl:text>
                 </xsl:attribute>
               </image>
             </xsl:when>
             <!--  -->
             <xsl:when test="self::video and @youtube">
               <image>
                 <xsl:attribute name="pi:generated">
                   <xsl:text>youtube/</xsl:text>
-                  <xsl:apply-templates select="." mode="visible-id-early"/>
+                  <xsl:apply-templates select="." mode="assembly-id"/>
                   <xsl:text>.jpg</xsl:text>
                 </xsl:attribute>
               </image>
             </xsl:when>
             <!--  -->
             <xsl:when test="self::video and @youtubeplaylist">
               <image>
@@ -2056,15 +2106,15 @@
           </xsl:choose>
           <stack>
             <!-- 2023-02-07: wrapping in a URL failed    -->
             <!-- for a LaTeX build of the sample article -->
             <image>
               <xsl:attribute name="pi:generated">
                 <xsl:text>qrcode/</xsl:text>
-                <xsl:apply-templates select="." mode="visible-id-early"/>
+                <xsl:apply-templates select="." mode="assembly-id"/>
                 <xsl:text>.png</xsl:text>
               </xsl:attribute>
             </image>
             <!-- URL templates create empty strings as signals URLs do not (yet) exist -->
             <!-- We kill the automatic footnotes, a debatable decision                 -->
             <!--  -->
             <xsl:variable name="standalone-url">
@@ -2112,8 +2162,185 @@
         <!-- duplicate authored content for the non-static conversions -->
         <xsl:copy>
           <xsl:apply-templates select="node()|@*" mode="representations"/>
         </xsl:copy>
       </xsl:when>
     </xsl:choose>
   </xsl:template>
+  <!-- ###################################### -->
+  <!-- Static versions of Interactive Content -->
+  <!-- ###################################### -->
+  <!-- Templates for the pre-processor (and other stylesheets) to use -->
+  <!-- for the creation of static versions of interactive content.    -->
+  <!-- The HTML conversion generates "standalone" pages for videos   -->
+  <!-- and other interactives.  Then the LaTeX conversion will make  -->
+  <!-- links to these pages (eg, via QR codes).  And we might use    -->
+  <!-- these pages as the basis for scraping preview images.  So we  -->
+  <!-- place a template here to achieve consistency across uses.     -->
+  <!--                                                               -->
+  <!-- We need to always import this assembly stylesheet, so these   -->
+  <!-- templates will be available in all conversions, but notably   -->
+  <!-- in the creation of a "universal" static version of the        -->
+  <!-- document ("assembly-static" in the pretext/pretext script)    -->
+  <!-- which is fed to specific conversion into static output        -->
+  <!-- formats (e.g. LaTeX, braille).  As such, these templates      -->
+  <!-- should                                                        -->
+  <!--   (a) be applied someplace as part of the assembly process    -->
+  <!--   (b) produce only text (i.e. not XML, not HTML, not LaTeX)   -->
+  <!-- NB: it could be tempting to change the next template to stuff -->
+  <!-- these "iframe" files into a dedicated directory.  Even though -->
+  <!-- this template ensures some consistency, a pile of links still -->
+  <!-- need to change, such as the "script" tag for locations of     -->
+  <!-- extra JS as part of making one of these go.                   -->
+  <xsl:template match="audio|video|interactive" mode="iframe-filename">
+    <xsl:apply-templates select="." mode="assembly-id"/>
+    <xsl:text>-if.html</xsl:text>
+  </xsl:template>
+  <xsl:template match="audio|video|interactive" mode="standalone-filename">
+    <xsl:apply-templates select="." mode="assembly-id"/>
+    <xsl:text>.html</xsl:text>
+  </xsl:template>
+  <xsl:template match="*" mode="standalone-filename">
+    <xsl:apply-templates select="." mode="visible-id"/>
+    <xsl:text>-ERROR-no-standalone-filename.html</xsl:text>
+  </xsl:template>
+  <xsl:template match="audio|video|interactive" mode="standalone-url">
+    <xsl:if test="$b-has-baseurl">
+      <xsl:value-of select="$baseurl"/>
+      <xsl:apply-templates select="." mode="standalone-filename"/>
+    </xsl:if>
+    <!-- empty without a baseurl -->
+  </xsl:template>
+  <xsl:template match="audio|video|interactive" mode="embed-iframe-url">
+    <xsl:if test="$b-has-baseurl">
+      <xsl:value-of select="$baseurl"/>
+      <xsl:apply-templates select="." mode="iframe-filename"/>
+    </xsl:if>
+    <!-- empty without a baseurl -->
+  </xsl:template>
+  <!-- These interactives *are* iFrames, so we don't build a dedicated   -->
+  <!-- page to make them into iFrames.  Over in -html we construct a URL -->
+  <!-- for each one, embedded in a iFrame construction.  We need to work -->
+  <!-- out the right thing to do for an "Embed" link in static formats.  -->
+  <!-- For now, an empty result means no link in sttic formats.          -->
+  <!-- NB: coordinate with "create-iframe-page" in -html                 -->
+  <xsl:template match="audio|video" mode="embed-iframe-url"/>
+  <xsl:template match="interactive[@desmos|@geogebra|@calcplot3d|@circuitjs|@iframe]" mode="embed-iframe-url"/>
+  <!-- Static URL's -->
+  <!-- Predictable and/or stable URLs for versions         -->
+  <!-- of interactives available online.  These are        -->
+  <!--                                                     -->
+  <!--   (1) "standalone" pages for author/local material, -->
+  <!--       as a product of the HTML conversion           -->
+  <!--   (2) computable addresses of network resources,    -->
+  <!--       eg the YouTube page of a resource             -->
+  <!-- Point to HTML-produced, and canonically-hosted, standalone page -->
+  <!-- NB: baseurl is assumed to have a trailing slash                 -->
+  <xsl:template match="audio[@source|@href]|video[@source|@href]|interactive" mode="static-url">
+    <xsl:value-of select="$baseurl"/>
+    <xsl:apply-templates select="." mode="standalone-filename"/>
+  </xsl:template>
+  <!-- Natural override for YouTube videos               -->
+  <!-- Better - standalone page, with "View on You Tube" -->
+  <!-- NB: ampersand is escaped for LaTeX use, be careful with switch to QR codes via Python! -->
+  <!-- POTENTIAL BUG: this should be un-LaTeX'ed for general use and then  -->
+  <!-- sanitized on the receiving end in the LaTeX conversion, or maybe    -->
+  <!-- the LaTeX conversion will do just fine if the right URL package is  -->
+  <!-- used and the ampersand is handled correctly?                        -->
+  <xsl:template match="video[@youtube|@youtubeplaylist]" mode="static-url">
+    <xsl:apply-templates select="." mode="youtube-view-url"/>
+    <xsl:if test="@start">
+      <xsl:text>\&amp;start=</xsl:text>
+      <xsl:value-of select="@start"/>
+    </xsl:if>
+    <xsl:if test="@end">
+      <xsl:text>\&amp;end=</xsl:text>
+      <xsl:value-of select="@end"/>
+    </xsl:if>
+  </xsl:template>
+  <xsl:template match="video[@youtube|@youtubeplaylist]" mode="youtube-view-url">
+    <xsl:variable name="youtube">
+      <xsl:choose>
+        <xsl:when test="@youtubeplaylist">
+          <xsl:value-of select="normalize-space(@youtubeplaylist)"/>
+        </xsl:when>
+        <xsl:otherwise>
+          <xsl:value-of select="normalize-space(str:replace(@youtube, ',', ' '))"/>
+        </xsl:otherwise>
+      </xsl:choose>
+    </xsl:variable>
+    <xsl:text>https://www.youtube.com/</xsl:text>
+    <xsl:choose>
+      <xsl:when test="@youtubeplaylist">
+        <xsl:text>playlist?list=</xsl:text>
+        <xsl:value-of select="$youtube"/>
+      </xsl:when>
+      <xsl:when test="contains($youtube, ' ')">
+        <xsl:text>watch_videos?video_ids=</xsl:text>
+        <xsl:value-of select="str:replace($youtube, ' ', ',')"/>
+      </xsl:when>
+      <xsl:otherwise>
+        <xsl:text>watch?v=</xsl:text>
+        <xsl:value-of select="$youtube"/>
+      </xsl:otherwise>
+    </xsl:choose>
+  </xsl:template>
+  <!-- Vimeo view URL -->
+  <xsl:template match="video[@vimeo]" mode="static-url">
+    <xsl:text>https://vimeo.com/</xsl:text>
+    <xsl:value-of select="@vimeo"/>
+  </xsl:template>
+  <!-- A bit different than above, but same mode -->
+  <!-- When a "datafile" is produced in a static -->
+  <!-- context, then we append the $baseurl, and -->
+  <!-- provide the external directory.           -->
+  <xsl:template match="dataurl[@source]" mode="static-url">
+    <xsl:value-of select="$baseurl"/>
+    <!-- empty when not using managed directories -->
+    <xsl:value-of select="$external-directory"/>
+    <xsl:apply-templates select="@source"/>
+  </xsl:template>
+  <!-- The contents of a datafile may be encoded as text in an XML   -->
+  <!-- file within the generated/datafile directory.  The filename   -->
+  <!-- has this construction, even if we do not always consult it.   -->
+  <!-- NB: these XML files will be read with a "document()" call,    -->
+  <!-- with a path relative to the author's main source file, hence  -->
+  <!-- the filename uses the directory name in author's source.      -->
+  <!-- NB: identical code in static constructions.                   -->
+  <xsl:template match="datafile" mode="datafile-filename">
+    <xsl:value-of select="$generated-directory-source"/>
+    <xsl:text>datafile/</xsl:text>
+    <!-- context is "datafile", the basis for identifier -->
+    <!-- ned an early identifier in assembly phase       -->
+    <xsl:apply-templates select="." mode="assembly-id"/>
+    <xsl:text>.xml</xsl:text>
+  </xsl:template>
+  <!-- The actual text contents of a "datafile", specified in a "pre" element.  -->
+  <!-- We assume (enforce) a "pre" child.  Then actual text comes authored in   -->
+  <!-- the source "pre" element or in an author-provided external file.         -->
+  <xsl:template match="datafile[pre]" mode="datafile-text-contents">
+    <xsl:choose>
+      <!-- via an external file -->
+      <!-- Once upon a time, we hit the text from a file with   -->
+      <!-- "sanitize-text".  This was a bad idea because        -->
+      <!--   (a) the manipulations (especially pad-length (?) ) -->
+      <!--       caused a false infinite recursion warning, and -->
+      <!--   (b) the file should be *exactly* what is desired.  -->
+      <xsl:when test="pre/@source">
+        <!-- filename is relative to author's source -->
+        <xsl:variable name="data-filename">
+          <xsl:apply-templates select="." mode="datafile-filename"/>
+        </xsl:variable>
+        <xsl:variable name="text-file-elt" select="document($data-filename, $original)/pi:text-file"/>
+        <xsl:value-of select="$text-file-elt"/>
+      </xsl:when>
+      <!-- via source "pre" element content -->
+      <xsl:otherwise>
+        <xsl:call-template name="sanitize-text">
+          <xsl:with-param name="text">
+            <xsl:value-of select="pre"/>
+          </xsl:with-param>
+        </xsl:call-template>
+      </xsl:otherwise>
+    </xsl:choose>
+  </xsl:template>
 </xsl:stylesheet>
```

#### xsl/pretext-revealjs.xsl

##### xsl/pretext-revealjs.xsl

```diff
@@ -395,26 +395,20 @@
         <xsl:attribute name="class">
           <xsl:text>fragment</xsl:text>
         </xsl:attribute>
       </xsl:if>
       <xsl:apply-templates/>
     </p>
   </xsl:template>
-  <xsl:template match="image">
-    <img>
-      <xsl:attribute name="src">
-        <xsl:value-of select="@source"/>
-      </xsl:attribute>
-      <xsl:if test="@pause = 'yes'">
-        <xsl:attribute name="class">
-          <xsl:text>fragment</xsl:text>
-        </xsl:attribute>
-      </xsl:if>
-      <xsl:apply-templates/>
-    </img>
+  <!-- Images get wrapped in a div with @class="fragment" if they are  -->
+  <!-- paused                                                          -->
+  <xsl:template match="image[not(ancestor::sidebyside) and (@pause='yes')]">
+    <div class="fragment">
+      <xsl:apply-imports/>
+    </div>
   </xsl:template>
   <!-- A "url" with content gets an automatic footnote with the @visual -->
   <!-- attribute value (if non-empty) or a mildly-sanitized version of  -->
   <!-- @href.  This template identifies and kills that special          -->
   <!-- construction, since a slideshow really doesn't need footnotes.   -->
   <xsl:template match="fn[@pi:url]"/>
   <!-- Side-By-Side -->
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -5758,15 +5758,15 @@
   </xsl:template>
   <xsl:template match="image" mode="description">
     <xsl:if test="description">
       <!-- @aria-live means screenreaders will make announcements -->
       <details class="image-description" aria-live="polite">
         <summary title="details">
           <xsl:call-template name="insert-symbol">
-            <xsl:with-param name="name" select="'description'"/>
+            <xsl:with-param name="name" select="'info'"/>
           </xsl:call-template>
         </summary>
         <div>
           <xsl:attribute name="id">
             <xsl:apply-templates select="." mode="describedby-id"/>
           </xsl:attribute>
           <xsl:apply-templates select="description"/>
@@ -8625,14 +8625,18 @@
       </pre>
     </xsl:if>
   </xsl:template>
   <!-- Data Files -->
   <xsl:template match="datafile">
     <xsl:apply-templates select="." mode="runestone-to-interactive"/>
   </xsl:template>
+  <!-- Queries -->
+  <xsl:template match="query">
+    <xsl:apply-templates select="." mode="runestone-to-interactive"/>
+  </xsl:template>
   <!-- Console Session -->
   <!-- An interactive command-line session with a prompt, input and output -->
   <xsl:template match="console" mode="code-inclusion">
     <!-- ignore prompt, and pick it up in trailing input -->
     <pre class="console">
       <xsl:apply-templates select="input|output"/>
     </pre>
@@ -8881,15 +8885,29 @@
       <xsl:apply-templates select="." mode="permid-attribute"/>
       <xsl:apply-templates select="." mode="size-pixels-attributes"/>
     </iframe>
   </xsl:template>
   <!-- For more complicated interactives, we just point to the page we generate -->
   <xsl:template match="interactive[@platform]" mode="iframe-interactive">
     <iframe>
-      <xsl:apply-templates select="." mode="html-id-attribute"/>
+      <!-- A DoenetML interactive lives two lives.  Plain 'ol PreTeXt,  -->
+      <!-- supported by a Doenet CDN for its interactivity.  But when   -->
+      <!-- hosted on Runestone it can communicate its results.  So in   -->
+      <!-- the manifest and then the database and it needs a better id. -->
+      <!-- This is nearly identical to the plain-PreTeXt "html-id",     -->
+      <!-- but with a preference (to become a necessity) for @label.    -->
+      <!-- document-id and version only result inside Runestone builds. -->
+      <xsl:choose>
+        <xsl:when test="@platform = 'doenetml'">
+          <xsl:apply-templates select="." mode="runestone-id-attribute"/>
+        </xsl:when>
+        <xsl:otherwise>
+          <xsl:apply-templates select="." mode="html-id-attribute"/>
+        </xsl:otherwise>
+      </xsl:choose>
       <xsl:apply-templates select="." mode="permid-attribute"/>
       <xsl:apply-templates select="." mode="size-pixels-attributes"/>
       <xsl:attribute name="src">
         <xsl:apply-templates select="." mode="iframe-filename"/>
       </xsl:attribute>
     </iframe>
   </xsl:template>
@@ -8931,14 +8949,16 @@
           <div>
             <!-- the actual interactive bit          -->
             <xsl:apply-templates select="." mode="size-pixels-style-attribute"/>
             <!-- stack, else use a layout -->
             <xsl:apply-templates select="slate|sidebyside|sbsgroup"/>
             <!-- accumulate script tags *after* HTML elements -->
             <xsl:apply-templates select="@source"/>
+            <!-- accumulate script elements *after* @source scripts -->
+            <xsl:apply-templates select="script"/>
           </div>
         </body>
       </html>
     </exsl:document>
   </xsl:template>
   <!-- These forms *are* iframes, so we don't need to build their content -->
   <!-- NB: coordinate with "embed-iframe-url" in -common                  -->
@@ -8995,14 +9015,22 @@
           <xsl:text>5</xsl:text>
         </xsl:otherwise>
       </xsl:choose>
       <xsl:text>.min.js</xsl:text>
     </xsl:variable>
     <script src="{$d3-library-url}"/>
   </xsl:template>
+  <!-- DoenetML header libraries -->
+  <xsl:template match="interactive[@platform = 'doenetml']" mode="header-libraries">
+    <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/doenet-standalone-test@0.6.0/dist/style.css"/>
+    <script onload="onLoad()" type="module" src="https://cdn.jsdelivr.net/npm/doenet-standalone-test@0.6.0/dist/doenet-standalone.min.js"/>
+    <script>
+      <xsl:text>function onLoad() {window.renderDoenetToContainer(document.querySelector(&quot;.doenetml-applet&quot;))}</xsl:text>
+    </script>
+  </xsl:template>
   <!-- Javascript header libraries (none) -->
   <xsl:template match="interactive[@platform = 'javascript']" mode="header-libraries"/>
   <!-- ########################### -->
   <!-- Slates (objects to draw on) -->
   <!-- ########################### -->
   <!-- Slates are where we draw, with different surfaces -->
   <xsl:template match="slate[@surface='div']">
@@ -9279,14 +9307,29 @@
           <xsl:value-of select="$external-directory"/>
           <xsl:value-of select="@source"/>
           <xsl:text>').then(function(response) { response.text().then( function(text) { parseJessie(text); }); });</xsl:text>
         </xsl:element>
       </xsl:when>
     </xsl:choose>
   </xsl:template>
+  <xsl:template match="slate[@surface = 'doenetml']">
+    <div class="doenetml-applet">
+      <div class="doenetml-loading" style="text-align:center">
+        <p>
+          <img src="https://www.doenet.org/Doenet_Logo_Frontpage.png"/>
+        </p>
+        <p>
+          <xsl:text>Waiting on the page to load...</xsl:text>
+        </p>
+      </div>
+      <script type="text/doenetml">
+        <xsl:value-of select="text()"/>
+      </script>
+    </div>
+  </xsl:template>
   <!-- Utilities -->
   <!-- These can be vastly improved with a call to "tokenize()"   -->
   <!-- and then a "for-each" can effectively loop over the pieces -->
   <!-- @source attribute to multiple script tags -->
   <xsl:template match="interactive[@platform]/@source">
     <xsl:variable name="scripts" select="str:tokenize(., ', ')"/>
     <!-- $scripts is a collection of "token" and does not have -->
@@ -9380,14 +9423,23 @@
       <xsl:text>height:</xsl:text>
       <xsl:value-of select="$height"/>
       <xsl:text>px;</xsl:text>
       <xsl:text>display: block;</xsl:text>
       <xsl:text>box-sizing: border-box; -moz-box-sizing: border-box; -webkit-box-sizing: border-box;</xsl:text>
     </xsl:attribute>
   </xsl:template>
+  <!-- Add js from script elemenets inside interactives     -->
+  <!-- Scripts are added in order, after all other elements -->
+  <!-- in the interactive, include scripts created from     -->
+  <!-- @source directives in the interactive element        -->
+  <xsl:template match="interactive[@platform = 'javascript']/script">
+    <script>
+      <xsl:value-of select="."/>
+    </script>
+  </xsl:template>
   <!-- JSXGraph -->
   <!-- DEPRECATED (2018-04-06)                             -->
   <!-- Restrict edits to cosmetic, no functional change    -->
   <!-- Remove when continued maintenance becomes untenable -->
   <!-- Not updated to be part of @permid scheme            -->
   <xsl:template match="jsxgraph">
     <!-- interpret @width percentage and @aspect ratio -->
```

#### xsl/pretext-text-utilities.xsl

##### xsl/pretext-text-utilities.xsl

```diff
@@ -853,29 +853,14 @@
   <!-- templates generally.  They are necessary to create static  -->
   <!-- versions of Runestone datafile elements during the         -->
   <!-- assembly phase, and the enhanced-source stylesheet avoids  -->
   <!-- using -common, hence movement here on 2023-10-30.          -->
   <!-- Datafiles have default rows and columns -->
   <xsl:variable name="datafile-default-rows" select="20"/>
   <xsl:variable name="datafile-default-cols" select="60"/>
-  <!-- The contents of a datafile may be encoded as text in an XML   -->
-  <!-- file within the generated/datafile directory.  The filename   -->
-  <!-- has this construction, even if we do not always consult it.   -->
-  <!-- NB: these XML files will be read with a "document()" call,    -->
-  <!-- with a path relative to the author's main source file, hence  -->
-  <!-- the filename uses the directory name in author's source.      -->
-  <!-- NB: identical code in static constructions.                   -->
-  <xsl:template match="datafile" mode="datafile-filename">
-    <xsl:value-of select="$generated-directory-source"/>
-    <xsl:text>datafile/</xsl:text>
-    <!-- context is "datafile", the basis for identifier -->
-    <!-- ned an early identifier in assembly phase       -->
-    <xsl:apply-templates select="." mode="assembly-id"/>
-    <xsl:text>.xml</xsl:text>
-  </xsl:template>
   <!-- Get a "view" of a chunk of text, from the "upper-left corner".  -->
   <!-- Motivation is a static version of a (large) datafile of text    -->
   <!-- for interactive programs to consume.                            -->
   <!--   text: the text, we provide a version hit by "santitize-tex"   -->
   <!--         above, which pulls left, and drops leading blank lines. -->
   <!--   nrows: the number of (initial) lines output                   -->
   <!--   ncols: the number of (initial) characters on each line        -->
@@ -924,37 +909,8 @@
 ')"/>
           <xsl:with-param name="nrows" select="$nrows - 1"/>
           <xsl:with-param name="ncols" select="$ncols"/>
         </xsl:call-template>
       </xsl:otherwise>
     </xsl:choose>
   </xsl:template>
-  <!-- The actual text contents of a "datafile", specified in a "pre" element.  -->
-  <!-- We assume (enforce) a "pre" child.  Then actual text comes authored in   -->
-  <!-- the source "pre" element or in an author-provided external file.         -->
-  <xsl:template match="datafile[pre]" mode="datafile-text-contents">
-    <xsl:choose>
-      <!-- via an external file -->
-      <!-- Once upon a time, we hit the text from a file with   -->
-      <!-- "sanitize-text".  This was a bad idea because        -->
-      <!--   (a) the manipulations (especially pad-length (?) ) -->
-      <!--       caused a false infinite recursion warning, and -->
-      <!--   (b) the file should be *exactly* what is desired.  -->
-      <xsl:when test="pre/@source">
-        <!-- filename is relative to author's source -->
-        <xsl:variable name="data-filename">
-          <xsl:apply-templates select="." mode="datafile-filename"/>
-        </xsl:variable>
-        <xsl:variable name="text-file-elt" select="document($data-filename, $original)/pi:text-file"/>
-        <xsl:value-of select="$text-file-elt"/>
-      </xsl:when>
-      <!-- via source "pre" element content -->
-      <xsl:otherwise>
-        <xsl:call-template name="sanitize-text">
-          <xsl:with-param name="text">
-            <xsl:value-of select="pre"/>
-          </xsl:with-param>
-        </xsl:call-template>
-      </xsl:otherwise>
-    </xsl:choose>
-  </xsl:template>
 </xsl:stylesheet>
```

#### xsl/pretext-runestone-static.xsl

##### xsl/pretext-runestone-static.xsl

```diff
@@ -783,14 +783,37 @@
     <!-- reproduce usual components -->
     <xsl:copy-of select="statement"/>
     <!-- skip over response until it carries something relevant -->
     <xsl:copy-of select="hint"/>
     <xsl:copy-of select="answer"/>
     <xsl:copy-of select="solution"/>
   </xsl:template>
+  <!-- Queries -->
+  <xsl:template match="query" mode="runestone-to-static">
+    <paragraphs>
+      <!-- no period, it is supplied by conversions -->
+      <!-- TODO: internationalize the term -->
+      <title>Query</title>
+      <!-- reproduce structured statement's pieces -->
+      <xsl:copy-of select="statement/*"/>
+      <!-- nothing to do for @scale style query -->
+      <!-- TODO: perhaps automatically indicate scale -->
+      <xsl:if test="choices">
+        <p>
+          <ol format="1.">
+            <xsl:for-each select="choices/choice">
+              <li>
+                <xsl:copy-of select="."/>
+              </li>
+            </xsl:for-each>
+          </ol>
+        </p>
+      </xsl:if>
+    </paragraphs>
+  </xsl:template>
   <!-- Active Code -->
   <xsl:template match="*[@exercise-interactive = 'coding']" mode="runestone-to-static">
     <!-- metadata (idx, title) -->
     <xsl:copy-of select="statement/preceding-sibling::*"/>
     <statement>
       <!-- duplicate the authored prompt/statement -->
       <xsl:copy-of select="statement/node()"/>
```

#### xsl/pretext-runestone.xsl

##### xsl/pretext-runestone.xsl

```diff
@@ -405,15 +405,15 @@
           <xsl:with-param name="name" select="'edit'"/>
         </xsl:call-template>
         <span class="name">Scratch ActiveCode</span>
       </button>
     </xsl:if>
   </xsl:template>
   <!-- A convenience for attaching a Runestone id -->
-  <xsl:template match="exercise|program|datafile||task|video[@youtube]|exercises" mode="runestone-id-attribute">
+  <xsl:template match="exercise|program|datafile|query||task|video[@youtube]|exercises|interactive[@platform = 'doenetml']" mode="runestone-id-attribute">
     <xsl:attribute name="id">
       <xsl:apply-templates select="." mode="runestone-id"/>
     </xsl:attribute>
   </xsl:template>
   <!-- ############### -->
   <!-- Runestone Hooks -->
   <!-- ############### -->
@@ -534,18 +534,19 @@
             <xsl:apply-templates select="$document-root" mode="title-plain"/>
           </title>
           <subtitle>
             <xsl:apply-templates select="$document-root" mode="subtitle"/>
           </subtitle>
           <!-- edition, too? -->
           <document-id>
+            <!-- global variables defined in -common -->
             <xsl:attribute name="edition">
-              <xsl:value-of select="$docinfo/document-id/@edition"/>
+              <xsl:value-of select="$edition"/>
             </xsl:attribute>
-            <xsl:value-of select="$docinfo/document-id"/>
+            <xsl:value-of select="$document-id"/>
           </document-id>
           <!-- duplicate blurb, blurb/@shelf for Runestone's convenience -->
           <!-- use "value-of" to enforce assumption there is no markup   -->
           <!-- NB: if absent in PTX source, these are empty in manifest  -->
           <shelf>
             <xsl:value-of select="$docinfo/blurb/@shelf"/>
           </shelf>
@@ -612,15 +613,15 @@
       </title>
       <!-- nearly a dead end, recurse into "exercise" and PROJECT-LIKE at *any* PTX -->
       <!-- depth, for example within a "subsection" (which Runestone does not have) -->
       <!-- If any of the next select are containers (full of "task") they will not  -->
       <!-- meet the dead-end monster match below, and the default template will     -->
       <!-- recurse into non-container "task" eventually, so "task" do get           -->
       <!-- processed, even if they seem to be missing from this select.             -->
-      <xsl:apply-templates select=".//exercise|.//project|.//activity|.//exploration|.//investigation|.//video[@youtube]|.//program[(@interactive = 'codelens') and not(parent::exercise)]|.//program[(@interactive = 'activecode') and not(parent::exercise)]|.//datafile" mode="runestone-manifest"/>
+      <xsl:apply-templates select=".//exercise|.//project|.//activity|.//exploration|.//investigation|.//video[@youtube]|.//program[(@interactive = 'codelens') and not(parent::exercise)]|.//program[(@interactive = 'activecode') and not(parent::exercise)]|.//datafile|.//interactive[@platform = 'doenetml']" mode="runestone-manifest"/>
     </subchapter>
     <!-- dead end structurally, no more recursion, even if "subsection", etc. -->
   </xsl:template>
   <!-- A Runestone exercise needs to identify itself when an instructor wants   -->
   <!-- to select it for assignment, so we want to provide enough identification -->
   <!-- in the manifest, via a "label" element full of raw text.                 -->
   <xsl:template match="exercise|project|activity|exploration|investigation|task" mode="runestone-manifest-label">
@@ -635,14 +636,22 @@
   <!-- Minimal label.  In database for obvious reasons, -->
   <!-- this is best (only?) thing to use as a label.    -->
   <xsl:template match="datafile" mode="runestone-manifest-label">
     <label>
       <xsl:value-of select="@filename"/>
     </label>
   </xsl:template>
+  <xsl:template match="interactive[@platform = 'doenetml']" mode="runestone-manifest-label">
+    <label>
+      <!-- This is not very informative.  Perhaps look up     -->
+      <!-- the tree to find a containing figure with a title  -->
+      <!-- TODO: perhaps via a type name -->
+      <xsl:text>DoenetML Interactive</xsl:text>
+    </label>
+  </xsl:template>
   <!-- Runestone tracks engagement with YouTube videos and "stray" -->
   <!-- ActiveCode and CodeLens (i.e. an "inline" "program", not as -->
   <!-- a portion of an "exercise".  As these are atomic elements,  -->
   <!-- there is little to grab onto for a label in a report for an -->
   <!-- instructor.  So we provide examination of an enclosing      -->
   <!-- figure ("video") or listing ("program").                    -->
   <xsl:template match="video[@youtube]|program[((@interactive = 'codelens') or (@interactive = 'activecode')) and not(parent::exercise)]" mode="runestone-manifest-label">
@@ -805,14 +814,22 @@
       <!-- label is from the "program", or enclosing "listing" -->
       <xsl:apply-templates select="." mode="runestone-manifest-label"/>
       <htmlsrc>
         <xsl:apply-templates select="." mode="runestone-to-interactive"/>
       </htmlsrc>
     </question>
   </xsl:template>
+  <xsl:template match="interactive[@platform = 'doenetml']" mode="runestone-manifest">
+    <question>
+      <xsl:apply-templates select="." mode="runestone-manifest-label"/>
+      <htmlsrc>
+        <xsl:apply-templates select="." mode="iframe-interactive"/>
+      </htmlsrc>
+    </question>
+  </xsl:template>
   <!-- Appendix is explicitly no-op, so we do not recurse into "section"  -->
   <xsl:template match="appendix" mode="runestone-manifest"/>
   <!-- Traverse the tree,looking for things to do          -->
   <!-- http://stackoverflow.com/questions/3776333/         -->
   <!-- stripping-all-elements-except-one-in-xml-using-xslt -->
   <xsl:template match="*" mode="runestone-manifest">
     <xsl:apply-templates select="*" mode="runestone-manifest"/>
@@ -1275,14 +1292,15 @@
                   <xsl:apply-templates select="." mode="horizontal-blocks">
                     <xsl:with-param name="b-natural" select="$b-natural"/>
                   </xsl:apply-templates>
                 </xsl:for-each>
               </xsl:otherwise>
             </xsl:choose>
             <!-- a block of unit tests for automatic feedback (with, say, an SQL database) -->
+            <!-- NB: could mimic "program/tests" to avoid empty "tests" elements           -->
             <xsl:if test="tests">
               <xsl:text>--unittest--</xsl:text>
               <xsl:call-template name="sanitize-text">
                 <xsl:with-param name="text" select="tests"/>
               </xsl:call-template>
             </xsl:if>
           </textarea>
@@ -1751,14 +1769,17 @@
                 <xsl:attribute name="id">
                   <xsl:value-of select="concat($hid, '_editor')"/>
                 </xsl:attribute>
                 <xsl:attribute name="data-question_label"/>
                 <!-- Code Lens only for certain languages -->
                 <xsl:attribute name="data-codelens">
                   <xsl:choose>
+                    <xsl:when test="@codelens = 'no'">
+                      <xsl:text>false</xsl:text>
+                    </xsl:when>
                     <xsl:when test="($active-language = 'python') or ($active-language = 'python2') or ($active-language = 'python3')">
                       <xsl:text>true</xsl:text>
                     </xsl:when>
                     <xsl:when test="($active-language = 'c') or ($active-language = 'cpp') or ($active-language = 'java')">
                       <xsl:text>true</xsl:text>
                     </xsl:when>
                     <xsl:otherwise>
@@ -1814,18 +1835,32 @@
                 </xsl:if>
                 <!-- the code itself as text -->
                 <xsl:call-template name="sanitize-text">
                   <xsl:with-param name="text" select="input"/>
                 </xsl:call-template>
                 <!-- optional unit testing, with RS markup to keep it hidden -->
                 <xsl:if test="tests">
-                  <xsl:text>====</xsl:text>
-                  <xsl:call-template name="sanitize-text">
-                    <xsl:with-param name="text" select="tests"/>
-                  </xsl:call-template>
+                  <!-- Be wary of empty "test" elements which lead to -->
+                  <!-- empty files, which are possibly not legal      -->
+                  <!-- programs for their target languages, and hence -->
+                  <!-- raise errors due to  the Runestone back-end    -->
+                  <!-- trying to process them.                        -->
+                  <!-- NB: static versions never show "tests" anyway  -->
+                  <xsl:variable name="tests-content">
+                    <xsl:call-template name="sanitize-text">
+                      <xsl:with-param name="text" select="tests"/>
+                    </xsl:call-template>
+                  </xsl:variable>
+                  <!-- Even if there is no content, the sanitization -->
+                  <!-- template adds a concluding newline            -->
+                  <xsl:if test="not(normalize-space($tests-content) = '')">
+                    <xsl:text>====</xsl:text>
+                    <!-- historical behavior is to use sanitized version -->
+                    <xsl:value-of select="$tests-content"/>
+                  </xsl:if>
                 </xsl:if>
               </textarea>
             </div>
           </div>
         </div>
       </xsl:when>
     </xsl:choose>
@@ -2074,14 +2109,99 @@
               <xsl:apply-templates select="conclusion"/>
             </div>
           </xsl:if>
         </div>
       </div>
     </div>
   </xsl:template>
+  <!-- ####### -->
+  <!-- Queries -->
+  <!-- ####### -->
+  <xsl:template match="query" mode="runestone-to-interactive">
+    <!-- <xsl:text>FOO</xsl:text> -->
+    <xsl:variable name="the-choices" select="choices/choice"/>
+    <div class="ptx-runestone-container">
+      <div class="runestone">
+        <ul data-component="poll">
+          <xsl:apply-templates select="." mode="runestone-id-attribute"/>
+          <xsl:attribute name="data-results">
+            <xsl:choose>
+              <xsl:when test="(@visibility = 'instructor') or (@visibility = 'all')">
+                <xsl:value-of select="@visibility"/>
+              </xsl:when>
+              <xsl:otherwise>
+                <xsl:text>instructor</xsl:text>
+              </xsl:otherwise>
+            </xsl:choose>
+          </xsl:attribute>
+          <xsl:apply-templates select="statement"/>
+          <!-- infrastructure to here is common to a query with -->
+          <!-- explicit distinct choices, versus a query with a -->
+          <!-- simple scale for responses                       -->
+          <!-- NB: could define a variable early on indicating  -->
+          <!-- the nature of the poll, should there need to be  -->
+          <!-- more differentiation                             -->
+          <xsl:choose>
+            <xsl:when test="choices">
+              <xsl:apply-templates select="choices/choice"/>
+            </xsl:when>
+            <xsl:when test="foome">
+              <!-- context switch will allow "position()" to behave -->
+              <xsl:for-each select="$the-choices">
+                <li>
+                  <span class="poll-choice">
+                    <xsl:value-of select="position()"/>
+                  </span>
+                  <xsl:apply-templates/>
+                </li>
+              </xsl:for-each>
+            </xsl:when>
+            <xsl:when test="@scale">
+              <!-- generate list items with numbers recursively -->
+              <xsl:call-template name="numbered-list-items">
+                <xsl:with-param name="max" select="@scale"/>
+              </xsl:call-template>
+            </xsl:when>
+            <!-- could add error warning here?  Or rely on schema? -->
+            <xsl:otherwise/>
+          </xsl:choose>
+        </ul>
+      </div>
+    </div>
+  </xsl:template>
+  <xsl:template match="query/choices/choice">
+    <li>
+      <!-- <span class="poll-choice">
+            <xsl:number/>
+        </span> -->
+      <xsl:number/>
+      <xsl:text>.</xsl:text>
+      <xsl:apply-templates/>
+    </li>
+  </xsl:template>
+  <xsl:template name="numbered-list-items">
+    <!-- always initialize with 1 to start -->
+    <xsl:param name="current" select="'1'"/>
+    <xsl:param name="max"/>
+    <xsl:choose>
+      <!-- $current is too big, done with recursion -->
+      <xsl:when test="$current &gt; $max"/>
+      <xsl:otherwise>
+        <!-- make numbered list-item -->
+        <li>
+          <xsl:value-of select="$current"/>
+        </li>
+        <!-- recurse with next integer -->
+        <xsl:call-template name="numbered-list-items">
+          <xsl:with-param name="current" select="$current + 1"/>
+          <xsl:with-param name="max" select="$max"/>
+        </xsl:call-template>
+      </xsl:otherwise>
+    </xsl:choose>
+  </xsl:template>
   <!-- ######### -->
   <!-- Utilities -->
   <!-- ######### -->
   <!-- Runestone components, such as data files and select questions,  -->
   <!-- frequently point to other Runestone components in the database. -->
   <!--   * Authors point in their source with @xml:id                  -->
   <!--     values in a space- or comma- separated list                 -->
```

#### xsl/pretext-common.xsl

##### xsl/pretext-common.xsl

```diff
@@ -171,16 +171,27 @@
     <xsl:value-of select="$root/@xml:lang"/>
   </xsl:variable>
   <!-- An author may elect to place a unique string into   -->
   <!-- the docinfo/document-id element and conversions may -->
   <!-- use this to distinguish one document from another.  -->
   <!-- The global variable here is empty to signal         -->
   <!-- "no choice" by the author.                          -->
+  <!-- NB: at some point this should be specified as an    -->
+  <!-- attribute, rather than as content, which would make -->
+  <!-- things like newlines less likely to appear.  Much   -->
+  <!-- as "doucment-id/@edition" is given.  Keep the       -->
+  <!-- normalizationcan, it just becomes less necessary.   -->
   <xsl:variable name="document-id">
-    <xsl:value-of select="$docinfo/document-id"/>
+    <xsl:value-of select="normalize-space($docinfo/document-id)"/>
+  </xsl:variable>
+  <!-- And an edition is critical for maintaing the -->
+  <!-- Runestone database, though it may have other -->
+  <!-- uses related to maintaining changes.         -->
+  <xsl:variable name="edition">
+    <xsl:value-of select="normalize-space($docinfo/document-id/@edition)"/>
   </xsl:variable>
   <!-- The new version can return to the generic version  -->
   <!-- once we kill the dashed version for author use.    -->
   <xsl:variable name="author-tools-new">
     <xsl:choose>
       <!-- respect old switch, if set properly -->
       <!-- but don't error check or anything   -->
@@ -2986,134 +2997,14 @@
     <xsl:variable name="aspect-ratio">
       <xsl:apply-templates select="." mode="get-aspect-ratio">
         <xsl:with-param name="default-aspect" select="$default-aspect"/>
       </xsl:apply-templates>
     </xsl:variable>
     <xsl:value-of select="round($design-width-pixels * $width-fraction div $aspect-ratio)"/>
   </xsl:template>
-  <!-- ###################################### -->
-  <!-- Static versions of Interactive Content -->
-  <!-- ###################################### -->
-  <!-- Templates for the pre-processor (and other stylesheets) to use -->
-  <!-- for the creation of static versions of interactive content.    -->
-  <!-- The HTML conversion generates "standalone" pages for videos   -->
-  <!-- and other interactives.  Then the LaTeX conversion will make  -->
-  <!-- links to these pages (eg, via QR codes).  And we might use    -->
-  <!-- these pages as the basis for scraping preview images.  So we  -->
-  <!-- place a template here to achieve consistency across uses.     -->
-  <!--  -->
-  <!-- NB: it could be tempting to change this template to stuff     -->
-  <!-- these "iframe" files into a dedicated directory.  Even though -->
-  <!-- this template ensures some consistency, a pile of links still -->
-  <!-- need to change, such as the "script" tag for locations of     -->
-  <!-- extra JS as part of making one of these go.                   -->
-  <xsl:template match="*" mode="iframe-filename">
-    <xsl:apply-templates select="." mode="visible-id-early"/>
-    <xsl:text>-if.html</xsl:text>
-  </xsl:template>
-  <xsl:template match="audio|video|interactive" mode="standalone-filename">
-    <xsl:apply-templates select="." mode="visible-id-early"/>
-    <xsl:text>.html</xsl:text>
-  </xsl:template>
-  <xsl:template match="*" mode="standalone-filename">
-    <xsl:apply-templates select="." mode="visible-id"/>
-    <xsl:text>-ERROR-no-standalone-filename.html</xsl:text>
-  </xsl:template>
-  <xsl:template match="audio|video|interactive" mode="standalone-url">
-    <xsl:if test="$b-has-baseurl">
-      <xsl:value-of select="$baseurl"/>
-      <xsl:apply-templates select="." mode="standalone-filename"/>
-    </xsl:if>
-    <!-- empty without a baseurl -->
-  </xsl:template>
-  <xsl:template match="audio|video|interactive" mode="embed-iframe-url">
-    <xsl:if test="$b-has-baseurl">
-      <xsl:value-of select="$baseurl"/>
-      <xsl:apply-templates select="." mode="iframe-filename"/>
-    </xsl:if>
-    <!-- empty without a baseurl -->
-  </xsl:template>
-  <!-- These interactives *are* iFrames, so we don't build a dedicated   -->
-  <!-- page to make them into iFrames.  Over in -html we construct a URL -->
-  <!-- for each one, embedded in a iFrame construction.  We need to work -->
-  <!-- out the right thing to do for an "Embed" link in static formats.  -->
-  <!-- For now, an empty result means no link in sttic formats.          -->
-  <!-- NB: coordinate with "create-iframe-page" in -html                 -->
-  <xsl:template match="audio|video" mode="embed-iframe-url"/>
-  <xsl:template match="interactive[@desmos|@geogebra|@calcplot3d|@circuitjs|@iframe]" mode="embed-iframe-url"/>
-  <!-- Static URL's -->
-  <!-- Predictable and/or stable URLs for versions         -->
-  <!-- of interactives available online.  These are        -->
-  <!--                                                     -->
-  <!--   (1) "standalone" pages for author/local material, -->
-  <!--       as a product of the HTML conversion           -->
-  <!--   (2) computable addresses of network resources,    -->
-  <!--       eg the YouTube page of a resource             -->
-  <!-- Point to HTML-produced, and canonically-hosted, standalone page -->
-  <!-- NB: baseurl is assumed to have a trailing slash                 -->
-  <xsl:template match="audio[@source|@href]|video[@source|@href]|interactive" mode="static-url">
-    <xsl:value-of select="$baseurl"/>
-    <xsl:apply-templates select="." mode="standalone-filename"/>
-  </xsl:template>
-  <!-- Natural override for YouTube videos               -->
-  <!-- Better - standalone page, with "View on You Tube" -->
-  <!-- NB: ampersand is escaped for LaTeX use, be careful with switch to QR codes via Python! -->
-  <xsl:template match="video[@youtube|@youtubeplaylist]" mode="static-url">
-    <xsl:apply-templates select="." mode="youtube-view-url"/>
-    <xsl:if test="@start">
-      <xsl:text>\&amp;start=</xsl:text>
-      <xsl:value-of select="@start"/>
-    </xsl:if>
-    <xsl:if test="@end">
-      <xsl:text>\&amp;end=</xsl:text>
-      <xsl:value-of select="@end"/>
-    </xsl:if>
-  </xsl:template>
-  <xsl:template match="video[@youtube|@youtubeplaylist]" mode="youtube-view-url">
-    <xsl:variable name="youtube">
-      <xsl:choose>
-        <xsl:when test="@youtubeplaylist">
-          <xsl:value-of select="normalize-space(@youtubeplaylist)"/>
-        </xsl:when>
-        <xsl:otherwise>
-          <xsl:value-of select="normalize-space(str:replace(@youtube, ',', ' '))"/>
-        </xsl:otherwise>
-      </xsl:choose>
-    </xsl:variable>
-    <xsl:text>https://www.youtube.com/</xsl:text>
-    <xsl:choose>
-      <xsl:when test="@youtubeplaylist">
-        <xsl:text>playlist?list=</xsl:text>
-        <xsl:value-of select="$youtube"/>
-      </xsl:when>
-      <xsl:when test="contains($youtube, ' ')">
-        <xsl:text>watch_videos?video_ids=</xsl:text>
-        <xsl:value-of select="str:replace($youtube, ' ', ',')"/>
-      </xsl:when>
-      <xsl:otherwise>
-        <xsl:text>watch?v=</xsl:text>
-        <xsl:value-of select="$youtube"/>
-      </xsl:otherwise>
-    </xsl:choose>
-  </xsl:template>
-  <!-- Vimeo view URL -->
-  <xsl:template match="video[@vimeo]" mode="static-url">
-    <xsl:text>https://vimeo.com/</xsl:text>
-    <xsl:value-of select="@vimeo"/>
-  </xsl:template>
-  <!-- A bit different than above, but same mode -->
-  <!-- When a "datafile" is produced in a static -->
-  <!-- context, then we append the $baseurl, and -->
-  <!-- provide the external directory.           -->
-  <xsl:template match="dataurl[@source]" mode="static-url">
-    <xsl:value-of select="$baseurl"/>
-    <!-- empty when not using managed directories -->
-    <xsl:value-of select="$external-directory"/>
-    <xsl:apply-templates select="@source"/>
-  </xsl:template>
   <!-- ################ -->
   <!-- Names of Objects -->
   <!-- ################ -->
   <!-- The  xsl/localizations/localizations.xml  file contains the base -->
   <!-- filenames for the individual (per-language) files.  We form a    -->
   <!-- node-set of these filenames in the  $locale-files  variable.     -->
   <!-- Then the  document()  function will read multiple files and      -->
@@ -3460,35 +3351,14 @@
   <!-- These strings are used for items an author must manage              -->
   <!-- (image files) or that a reader will interact with (shared URLs)     -->
   <!-- Since items like filenames and URLs are sometimes shared across     -->
   <!-- conversions (or extractions) this template is in -common            -->
   <xsl:template match="*" mode="visible-id">
     <xsl:value-of select="@unique-id"/>
   </xsl:template>
-  <!-- The "visible-id" version above assumes any (legacy) @xml:id have -->
-  <!-- been upgraded by the assembly/pre-processor stylesheet.  But in  -->
-  <!-- that stylesheet we sometimes need this identifier **before** the -->
-  <!-- upgrade happens.  This matter of timing might be resolved by     -->
-  <!-- being more careful about when static representations are         -->
-  <!-- substituted into assembled source.                               -->
-  <xsl:template match="*" mode="visible-id-early">
-    <xsl:choose>
-      <xsl:when test="@label">
-        <xsl:value-of select="@label"/>
-      </xsl:when>
-      <xsl:when test="@xml:id">
-        <xsl:value-of select="@xml:id"/>
-      </xsl:when>
-      <xsl:otherwise>
-        <xsl:value-of select="local-name(.)"/>
-        <xsl:text>-</xsl:text>
-        <xsl:number from="book|article|letter|memo" level="any"/>
-      </xsl:otherwise>
-    </xsl:choose>
-  </xsl:template>
   <!-- An image described by source code, using languages Asymptote,     -->
   <!-- Sage, or LaTeX, should have its filename determined by properties -->
   <!-- of the associated language-specific element, specifically this is -->
   <!-- the province of the @label attribute.  So this is the preference  -->
   <!-- from approximately 2023-08-12.  Looking to the enclosing (parent) -->
   <!-- "image" is historical, preserving backward-compatibility.         -->
   <xsl:template match="asymptote|sageplot|latex-image" mode="image-source-basename">
@@ -3519,15 +3389,15 @@
   <!-- And the HTML representation of an interactive exercise, when powered -->
   <!-- by Runestone services, needs an HTML id.  But the PreTeXt "exercise" -->
   <!-- that wraps it has its own HTML id necessary for targets of           -->
   <!-- cross-reference (in-context) URLs.  We will prefer @label for the    -->
   <!-- PreTeXt "exercise" HTML id.  And we will require a *stable* @label   -->
   <!-- from an author, which we will dress up here.  Notice that this can   -->
   <!-- change when an author declares a new edition.                        -->
-  <xsl:template match="exercise|program|datafile||task|video[@youtube]|exercises" mode="runestone-id">
+  <xsl:template match="exercise|program|datafile|query||task|video[@youtube]|exercises|interactive[@platform = 'doenetml']" mode="runestone-id">
     <!-- With no @xml:id and no @label we realize the author has not given    -->
     <!-- any thought to a (semi-)peersistent identifire for the Runestone     -->
     <!-- database.  So we call that out as an error.  And we do not even      -->
     <!-- attempt to fallback to an automatically generated string, which      -->
     <!-- would be malleable over time and editing.                            -->
     <!-- As part of backwards-compatibility, we copy old @xml:id values into  -->
     <!-- fresh @label.  But have an internal  @authored-label attribute whose -->
@@ -3566,17 +3436,18 @@
         </xsl:message>
         <xsl:apply-templates select="." mode="location-report"/>
       </xsl:when>
     </xsl:choose>
     <!-- Prefix just for RS server builds, in order that the database -->
     <!-- of exercises gets a globally unique identifier.              -->
     <xsl:if test="$b-host-runestone">
-      <xsl:value-of select="$docinfo/document-id"/>
+      <!-- global variables defined in this stylesheet -->
+      <xsl:value-of select="$document-id"/>
       <xsl:text>_</xsl:text>
-      <xsl:value-of select="$docinfo/document-id/@edition"/>
+      <xsl:value-of select="$edition"/>
       <xsl:text>_</xsl:text>
     </xsl:if>
     <!-- We require a @label attribute, but allow it to be -->
     <!-- the result of an automatic copy from an @xml:id.  -->
     <xsl:value-of select="@label"/>
   </xsl:template>
   <!--            -->
@@ -7923,14 +7794,21 @@
       </xsl:when>
       <xsl:when test="@text='type-local'">
         <xsl:text>type-local</xsl:text>
       </xsl:when>
       <xsl:when test="@text='type-hybrid'">
         <xsl:text>type-hybrid</xsl:text>
       </xsl:when>
+      <xsl:when test="@text='type-global-title'">
+        <xsl:text>type-global-title</xsl:text>
+      </xsl:when>
+      <xsl:when test="@text='type-local-title'">
+        <xsl:text>type-local-title</xsl:text>
+      </xsl:when>
+      <!-- no 'type-hybrid-title' yet -->
       <xsl:when test="@text='phrase-global'">
         <xsl:text>phrase-global</xsl:text>
       </xsl:when>
       <xsl:when test="@text='phrase-hybrid'">
         <xsl:text>phrase-hybrid</xsl:text>
       </xsl:when>
       <xsl:when test="@text='title'">
@@ -7968,14 +7846,21 @@
       </xsl:when>
       <xsl:when test="$xref-text-style='type-local'">
         <xsl:text>type-local</xsl:text>
       </xsl:when>
       <xsl:when test="$xref-text-style='type-hybrid'">
         <xsl:text>type-hybrid</xsl:text>
       </xsl:when>
+      <xsl:when test="$xref-text-style='type-global-title'">
+        <xsl:text>type-global-title</xsl:text>
+      </xsl:when>
+      <xsl:when test="$xref-text-style='type-local-title'">
+        <xsl:text>type-local-title</xsl:text>
+      </xsl:when>
+      <!-- no 'type-hybrid-title' yet -->
       <xsl:when test="$xref-text-style='phrase-global'">
         <xsl:text>phrase-global</xsl:text>
       </xsl:when>
       <xsl:when test="$xref-text-style='phrase-hybrid'">
         <xsl:text>phrase-hybrid</xsl:text>
       </xsl:when>
       <xsl:when test="$xref-text-style='title'">
@@ -8072,15 +7957,15 @@
             <xsl:value-of select="@ref"/>
             <xsl:text>&quot;) does not have a number. You could try 'text=&quot;title&quot;' or 'text=&quot;custom&quot;' on the &quot;xref&quot;.</xsl:text>
           </xsl:message>
           <xsl:apply-templates select="." mode="location-report"/>
         </xsl:if>
       </xsl:otherwise>
     </xsl:choose>
-    <!-- Start massive "choose" for exceptions and ten general styles -->
+    <!-- Start massive "choose" for exceptions and twelve general styles -->
     <xsl:choose>
       <xsl:when test="$b-is-contributor-target">
         <xsl:apply-templates select="$target/personname"/>
       </xsl:when>
       <!-- equations are different -->
       <!-- custom or full number   -->
       <xsl:when test="$b-is-equation-target">
@@ -8162,14 +8047,48 @@
           <xsl:otherwise>
             <xsl:apply-templates select="$target" mode="type-name"/>
             <xsl:apply-templates select="." mode="xref-text-separator"/>
             <xsl:apply-templates select="$target" mode="serial-number"/>
           </xsl:otherwise>
         </xsl:choose>
       </xsl:when>
+      <xsl:when test="($text-style = 'type-global-title') or ($text-style = 'type-local-title')">
+        <xsl:choose>
+          <!-- content override of type-prefix -->
+          <xsl:when test="$b-has-content">
+            <xsl:copy-of select="$custom-text"/>
+          </xsl:when>
+          <!-- usual, default case -->
+          <xsl:otherwise>
+            <xsl:apply-templates select="$target" mode="type-name"/>
+          </xsl:otherwise>
+        </xsl:choose>
+        <xsl:apply-templates select="." mode="xref-text-separator"/>
+        <!-- only difference in behavior is global/local number -->
+        <xsl:choose>
+          <xsl:when test="$text-style = 'type-global-title'">
+            <xsl:apply-templates select="$target" mode="xref-number">
+              <xsl:with-param name="xref" select="."/>
+            </xsl:apply-templates>
+          </xsl:when>
+          <xsl:when test="$text-style = 'type-local-title'">
+            <xsl:apply-templates select="$target" mode="serial-number"/>
+          </xsl:when>
+          <xsl:otherwise/>
+        </xsl:choose>
+        <xsl:variable name="the-title">
+          <xsl:apply-templates select="$target" mode="title-xref"/>
+        </xsl:variable>
+        <!-- no title, no problem -->
+        <xsl:if test="not($the-title = '')">
+          <xsl:apply-templates select="." mode="xref-text-separator"/>
+          <!-- title might have markup (eg math in HTML), so copy -->
+          <xsl:copy-of select="$the-title"/>
+        </xsl:if>
+      </xsl:when>
       <!-- special case for phrase options and list items of anonymous lists        -->
       <!-- catch this first and provide no text at all (could provide busted text?) -->
       <!-- anonymous lists live in "p", but this is an unreliable indication        -->
       <xsl:when test="($text-style = 'phrase-global' or $text-style = 'phrase-hybrid') and ($target/self::li and not($target/ancestor::list or $target/ancestor::objectives or $target/ancestor::outcomes or $target/ancestor::exercise))">
         <xsl:message>
           PTX:WARNING: a cross-reference to a list item of an anonymous list (&quot;
           <xsl:apply-templates select="$target" mode="serial-number"/>
```

#### xsl/support/runestone-services.xml

##### xsl/support/runestone-services.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <all>
   <js type="list">
-    <item type="str">prefix-runtime.2438a8bdd6d43b5c.bundle.js</item>
+    <item type="str">prefix-runtime.d30f9fb21d6c7b70.bundle.js</item>
     <item type="str">prefix-347.8328b60515045466.bundle.js</item>
     <item type="str">prefix-runestone.aeac7cf9ad5c07ef.bundle.js</item>
   </js>
   <css type="list">
     <item type="str">prefix-347.f9add1ca35d5ad93.css</item>
     <item type="str">prefix-runestone.f64dcc3632d7a0c3.css</item>
   </css>
   <cdn-url type="str">https://runestone.academy/cdn/runestone/</cdn-url>
-  <version type="str">7.2.9</version>
+  <version type="str">7.2.15</version>
 </all>
```

#### pretext/pretext.py

```diff
@@ -322,15 +322,15 @@
                 )
                 # bytes -> ASCII, strip final newline
                 asyversion = proc.stderr.read().decode("ascii")[:-1]
                 # build command line to suit
                 # 2021-12-10, Michael Doob: "-noprc" is default for the server,
                 # and newer CLI versions.  Retain for explicit use locally when
                 # perhaps an older version is being employed
-                asy_cli = asy_executable_cmd + ["-f", outform]
+                asy_cli = asy_executable_cmd + ["-f", outform, "-noV"]
                 if outform in ["pdf", "eps"]:
                     asy_cli += ["-noprc", "-iconify", "-tex", "xelatex", "-batchMask"]
                 elif outform in ["svg", "png"]:
                     asy_cli += ["-render=4", "-tex", "xelatex", "-iconify"]
             if method == "server":
                 alberta = "http://asymptote.ualberta.ca:10007?f={}".format(outform)
             # loop over .asy files, doing conversions
@@ -484,25 +484,44 @@
                 log.info("copying {} to {}".format(latex_image, dest_dir))
             else:
                 filebase, _ = os.path.splitext(latex_image)
                 latex_image_pdf = "{}.pdf".format(filebase)
                 latex_image_svg = "{}.svg".format(filebase)
                 latex_image_png = "{}.png".format(filebase)
                 latex_image_eps = "{}.eps".format(filebase)
+                latex_image_log = "{}.log".format(filebase)
                 # process with a  latex  engine
                 latex_key = get_deprecated_tex_fallback(method)
                 tex_executable_cmd = get_executable_cmd(latex_key)
                 # TODO why this debug line? get_executable_cmd() outputs the same debug info
                 log.debug("tex executable: {}".format(tex_executable_cmd[0]))
                 latex_cmd = tex_executable_cmd + ["-interaction=nonstopmode", "-halt-on-error", latex_image]
                 log.info("converting {} to {}".format(latex_image, latex_image_pdf))
                 # Run LaTeX on the image file, usual console transcript is stdout.
                 # "result" is a "CompletedProcess" object.  Specifying an encoding
                 # causes captured output to be a string, which is convenient.
                 result = subprocess.run(latex_cmd, stdout=subprocess.PIPE, encoding="utf-8")
+
+                # It may be that the image needs to be compiled twice. If the .log file contains
+                # the string `Rerun to get`, then the document should be compiled again.
+
+                # We keep track of how many times we've tried to compile the document and
+                # bail if it looks like we're stuck in a loop.
+                loop_count = 0
+                MAX_LOOPS = 10
+                while result.returncode == 0 and "Rerun to get" in open(latex_image_log).read() and loop_count < MAX_LOOPS:
+                    msg = "File {} needs to be processed with LaTeX again. Rerunning LaTeX for pass number {}."
+                    log.info(msg.format(latex_image, loop_count + 2))
+                    result = subprocess.run(latex_cmd, stdout=subprocess.PIPE, encoding="utf-8")
+                    loop_count += 1
+
+                if loop_count == MAX_LOOPS:
+                    log.error("Detected infinite loop while compiling {}. Aborting.".format(latex_image))
+                    result.returncode = 1
+
                 if result.returncode != 0:
                     # failed
                     failed_images.append(latex_image)
                     # and we help as much as we can
                     msg = "\n".join(
                         [
                             "LaTeX compilation of {} failed.",
@@ -559,15 +578,15 @@
                         if pyMuPDF:
                             # create svg using pymupdf:
                             with fitz.Document(latex_image_pdf) as doc:
                                 svg = doc.load_page(0).get_svg_image()
                             with open(latex_image_svg, "w") as f:
                                 f.write(svg)
                             shutil.copy2(latex_image_svg, dest_dir)
-                            # clasic way to produce svg, using pdf2svg:
+                            # classic way to produce svg, using pdf2svg:
                             latex_image_svg = "classic-" + latex_image_svg
                         pdfsvg_executable_cmd = get_executable_cmd("pdfsvg")
                         # TODO why this debug line? get_executable_cmd() outputs the same debug info
                         log.debug("pdfsvg executable: {}".format(pdfsvg_executable_cmd[0]))
                         svg_cmd = pdfsvg_executable_cmd + [latex_image_pdf, latex_image_svg]
                         log.info(
                             "converting {} to {}".format(latex_image_pdf, latex_image_svg)
@@ -3560,24 +3579,30 @@
         nonlocal result_tree, texc
         try:
             result_tree = xslt(src_tree, **stringparams)
         except Exception as e:
             texc = e
 
     try:
-        outputfn("comprehensive messages, warnings, and errors:")
         parse_t = threading.Thread(target=transform)
         parse_t.start()
         still_alive = True
         start = 0
         while still_alive:
             parse_t.join(0.5)  # Wait 0.5 seconds for thread to complete
             still_alive = parse_t.is_alive()
 
             end = len(xslt.error_log)
+
+            # if there are any messages and we are just
+            # starting out, produce an explanatory line
+            # start will be reset to non-zero, so this is
+            # one-time only, and never if there are no messages
+            if (start == 0) and (end > 0):
+                outputfn("messages from the log for XSL processing (indented):")
             # print out any unprinted messages from error_log
             for line in range(start, end):
                 outputfn(f"    * {xslt.error_log[line].message}")
             start = end
         if texc is None:
             outputfn("successful application of {}".format(xsl))
         else:
@@ -3960,15 +3985,15 @@
 
 def get_temporary_directory():
     """Create, record, and return a scratch directory"""
     import tempfile  #  mkdtemp()
 
     global __temps  #  cache of temporary directories
 
-    temp_dir = tempfile.mkdtemp()
+    temp_dir = tempfile.mkdtemp(prefix="ptx-")
     # Register the directory for cleanup at the end of successful
     # execution iff the verbosity is set to level 2 ("debug")
     # So errors, or requesting gross debugging info, will leave the
     # directories behind for inspection, otherwise they get removed
     __temps.append(temp_dir)
     return temp_dir
```

#### schema/pretext.rng

##### schema/pretext.rng

```diff
@@ -1264,14 +1264,17 @@
   </define>
   <define name="Console">
     <element name="console">
       <optional>
         <ref name="PermanentID"/>
       </optional>
       <optional>
+        <ref name="Component"/>
+      </optional>
+      <optional>
         <attribute name="prompt"/>
       </optional>
       <optional>
         <attribute name="width"/>
       </optional>
       <optional>
         <attribute name="margins"/>
@@ -1293,14 +1296,17 @@
   </define>
   <define name="Program">
     <element name="program">
       <optional>
         <ref name="PermanentID"/>
       </optional>
       <optional>
+        <ref name="Component"/>
+      </optional>
+      <optional>
         <attribute name="width"/>
       </optional>
       <optional>
         <attribute name="margins"/>
       </optional>
       <optional>
         <attribute name="language"/>
@@ -1329,14 +1335,17 @@
   <define name="List">
     <choice>
       <element name="ol">
         <optional>
           <ref name="PermanentID"/>
         </optional>
         <optional>
+          <ref name="Component"/>
+        </optional>
+        <optional>
           <attribute name="cols">
             <choice>
               <value>2</value>
               <value>3</value>
               <value>4</value>
               <value>5</value>
               <value>6</value>
@@ -1364,14 +1373,17 @@
         </oneOrMore>
       </element>
       <element name="ul">
         <optional>
           <ref name="PermanentID"/>
         </optional>
         <optional>
+          <ref name="Component"/>
+        </optional>
+        <optional>
           <attribute name="cols">
             <choice>
               <value>2</value>
               <value>3</value>
               <value>4</value>
               <value>5</value>
               <value>6</value>
@@ -1406,14 +1418,17 @@
         </oneOrMore>
       </element>
       <element name="dl">
         <optional>
           <ref name="PermanentID"/>
         </optional>
         <optional>
+          <ref name="Component"/>
+        </optional>
+        <optional>
           <attribute name="width">
             <choice>
               <value>narrow</value>
               <value>medium</value>
               <value>wide</value>
             </choice>
           </attribute>
@@ -1829,14 +1844,17 @@
     </element>
   </define>
   <define name="SidebySideAttributes">
     <optional>
       <ref name="PermanentID"/>
     </optional>
     <optional>
+      <ref name="Component"/>
+    </optional>
+    <optional>
       <attribute name="margins"/>
     </optional>
     <optional>
       <choice>
         <attribute name="width"/>
         <attribute name="widths"/>
       </choice>
@@ -1914,173 +1932,203 @@
       <optional>
         <ref name="UniqueID"/>
       </optional>
       <optional>
         <ref name="PermanentID"/>
       </optional>
       <optional>
+        <ref name="Component"/>
+      </optional>
+      <optional>
         <attribute name="width"/>
       </optional>
       <optional>
         <attribute name="margins"/>
       </optional>
       <optional>
         <attribute name="rotate"/>
       </optional>
       <optional>
         <attribute name="archive"/>
       </optional>
       <attribute name="source"/>
-      <optional>
-        <choice>
+      <choice>
+        <attribute name="decorative">
+          <value>yes</value>
+        </attribute>
+        <group>
           <optional>
             <attribute name="decorative">
-              <choice>
-                <value>yes</value>
-                <value>no</value>
-              </choice>
+              <value>no</value>
             </attribute>
           </optional>
-          <group>
-            <element name="shortdescription">
-              <text/>
-            </element>
+          <interleave>
+            <optional>
+              <element name="shortdescription">
+                <text/>
+              </element>
+            </optional>
             <optional>
               <element name="description">
                 <oneOrMore>
                   <choice>
                     <ref name="Paragraph"/>
                     <ref name="Tabular"/>
                   </choice>
                 </oneOrMore>
               </element>
             </optional>
-          </group>
-        </choice>
-      </optional>
+          </interleave>
+        </group>
+      </choice>
     </element>
   </define>
   <define name="ImageCode">
     <element name="image">
       <optional>
         <ref name="UniqueID"/>
       </optional>
       <optional>
         <ref name="PermanentID"/>
       </optional>
       <optional>
+        <ref name="Component"/>
+      </optional>
+      <optional>
         <attribute name="width"/>
       </optional>
       <optional>
         <attribute name="margins"/>
       </optional>
       <optional>
         <attribute name="archive"/>
       </optional>
-      <optional>
-        <choice>
+      <choice>
+        <attribute name="decorative">
+          <value>yes</value>
+        </attribute>
+        <group>
           <optional>
             <attribute name="decorative">
-              <choice>
-                <value>yes</value>
-                <value>no</value>
-              </choice>
+              <value>no</value>
             </attribute>
           </optional>
-          <group>
-            <element name="shortdescription">
-              <oneOrMore>
-                <choice>
-                  <text/>
-                  <ref name="WWVariable"/>
-                </choice>
-              </oneOrMore>
-            </element>
+          <interleave>
+            <optional>
+              <element name="shortdescription">
+                <oneOrMore>
+                  <choice>
+                    <text/>
+                    <ref name="WWVariable"/>
+                  </choice>
+                </oneOrMore>
+              </element>
+            </optional>
             <optional>
               <element name="description">
                 <oneOrMore>
                   <choice>
                     <ref name="Paragraph"/>
                     <ref name="Tabular"/>
                   </choice>
                 </oneOrMore>
               </element>
             </optional>
-          </group>
-        </choice>
-      </optional>
-      <choice>
-        <element name="latex-image">
-          <text/>
-        </element>
-        <element name="asymptote">
-          <text/>
-        </element>
-        <element name="sageplot">
-          <optional>
-            <attribute name="variant">
-              <choice>
-                <value>2d</value>
-                <value>3d</value>
-              </choice>
-            </attribute>
-          </optional>
-          <optional>
-            <attribute name="aspect"/>
-          </optional>
-          <text/>
-        </element>
+            <choice>
+              <element name="latex-image">
+                <optional>
+                  <ref name="LabelID"/>
+                </optional>
+                <optional>
+                  <ref name="Component"/>
+                </optional>
+                <text/>
+              </element>
+              <element name="asymptote">
+                <optional>
+                  <ref name="LabelID"/>
+                </optional>
+                <optional>
+                  <ref name="Component"/>
+                </optional>
+                <text/>
+              </element>
+              <element name="sageplot">
+                <optional>
+                  <ref name="LabelID"/>
+                </optional>
+                <optional>
+                  <ref name="Component"/>
+                </optional>
+                <optional>
+                  <attribute name="variant">
+                    <choice>
+                      <value>2d</value>
+                      <value>3d</value>
+                    </choice>
+                  </attribute>
+                </optional>
+                <optional>
+                  <attribute name="aspect"/>
+                </optional>
+                <text/>
+              </element>
+            </choice>
+          </interleave>
+        </group>
       </choice>
     </element>
   </define>
   <define name="ImageWW">
     <element name="image">
       <optional>
         <attribute name="pg-name"/>
       </optional>
       <optional>
         <attribute name="width"/>
       </optional>
-      <optional>
-        <choice>
+      <choice>
+        <attribute name="decorative">
+          <value>yes</value>
+        </attribute>
+        <group>
           <optional>
             <attribute name="decorative">
-              <choice>
-                <value>yes</value>
-                <value>no</value>
-              </choice>
+              <value>no</value>
             </attribute>
           </optional>
-          <group>
-            <element name="shortdescription">
-              <oneOrMore>
-                <choice>
-                  <text/>
-                  <ref name="WWVariable"/>
-                </choice>
-              </oneOrMore>
-            </element>
+          <interleave>
+            <optional>
+              <element name="shortdescription">
+                <oneOrMore>
+                  <choice>
+                    <text/>
+                    <ref name="WWVariable"/>
+                  </choice>
+                </oneOrMore>
+              </element>
+            </optional>
             <optional>
               <element name="description">
                 <oneOrMore>
                   <choice>
                     <ref name="Paragraph"/>
                     <ref name="Tabular"/>
                   </choice>
                 </oneOrMore>
               </element>
             </optional>
-          </group>
-        </choice>
-      </optional>
-      <optional>
-        <element name="latex-image">
-          <text/>
-        </element>
-      </optional>
+            <optional>
+              <element name="latex-image">
+                <text/>
+              </element>
+            </optional>
+          </interleave>
+        </group>
+      </choice>
     </element>
   </define>
   <define name="BorderThickness">
     <choice>
       <value>none</value>
       <value>minor</value>
       <value>medium</value>
@@ -2154,14 +2202,15 @@
   <define name="TableRow">
     <element name="row">
       <optional>
         <attribute name="header">
           <choice>
             <value>yes</value>
             <value>no</value>
+            <value>vertical</value>
           </choice>
         </attribute>
       </optional>
       <optional>
         <ref name="AlignmentHorizontal"/>
       </optional>
       <optional>
@@ -2196,14 +2245,17 @@
   </define>
   <define name="Tabular">
     <element name="tabular">
       <optional>
         <ref name="PermanentID"/>
       </optional>
       <optional>
+        <ref name="Component"/>
+      </optional>
+      <optional>
         <attribute name="width"/>
       </optional>
       <optional>
         <attribute name="margins"/>
       </optional>
       <optional>
         <attribute name="row-headers">
@@ -2241,14 +2293,17 @@
   </define>
   <define name="Sage">
     <element name="sage">
       <optional>
         <ref name="PermanentID"/>
       </optional>
       <optional>
+        <ref name="Component"/>
+      </optional>
+      <optional>
         <attribute name="doctest"/>
       </optional>
       <optional>
         <attribute name="tolerance"/>
       </optional>
       <optional>
         <attribute name="auto-evaluate">
@@ -2284,17 +2339,23 @@
   </define>
   <define name="Video">
     <element name="video">
       <optional>
         <ref name="UniqueID"/>
       </optional>
       <optional>
+        <ref name="LabelID"/>
+      </optional>
+      <optional>
         <ref name="PermanentID"/>
       </optional>
       <optional>
+        <ref name="Component"/>
+      </optional>
+      <optional>
         <attribute name="width"/>
       </optional>
       <optional>
         <attribute name="margins"/>
       </optional>
       <optional>
         <attribute name="aspect"/>
@@ -2696,14 +2757,20 @@
   </define>
   <define name="WebWorkAuthored">
     <element name="webwork">
       <optional>
         <ref name="UniqueID"/>
       </optional>
       <optional>
+        <ref name="LabelID"/>
+      </optional>
+      <optional>
+        <ref name="Component"/>
+      </optional>
+      <optional>
         <attribute name="seed">
           <data type="integer"/>
         </attribute>
       </optional>
       <optional>
         <attribute name="copy"/>
       </optional>
@@ -2910,17 +2977,23 @@
         </oneOrMore>
       </choice>
     </element>
   </define>
   <define name="UniqueID">
     <attribute name="xml:id"/>
   </define>
+  <define name="LabelID">
+    <attribute name="label"/>
+  </define>
   <define name="PermanentID">
     <attribute name="permid"/>
   </define>
+  <define name="Component">
+    <attribute name="component"/>
+  </define>
   <define name="Title">
     <element name="title">
       <ref name="TextLong"/>
     </element>
   </define>
   <define name="LinedTitle">
     <element name="title">
@@ -2963,28 +3036,40 @@
     <attribute name="xml:lang"/>
   </define>
   <define name="MetaDataTarget">
     <optional>
       <ref name="UniqueID"/>
     </optional>
     <optional>
+      <ref name="LabelID"/>
+    </optional>
+    <optional>
       <ref name="PermanentID"/>
     </optional>
+    <optional>
+      <ref name="Component"/>
+    </optional>
     <zeroOrMore>
       <ref name="Index"/>
     </zeroOrMore>
   </define>
   <define name="MetaDataTitle">
     <optional>
       <ref name="UniqueID"/>
     </optional>
     <optional>
+      <ref name="LabelID"/>
+    </optional>
+    <optional>
       <ref name="PermanentID"/>
     </optional>
     <optional>
+      <ref name="Component"/>
+    </optional>
+    <optional>
       <ref name="XMLBase"/>
     </optional>
     <optional>
       <ref name="XMLLang"/>
     </optional>
     <ref name="Title"/>
     <zeroOrMore>
@@ -2992,17 +3077,23 @@
     </zeroOrMore>
   </define>
   <define name="MetaDataAltTitle">
     <optional>
       <ref name="UniqueID"/>
     </optional>
     <optional>
+      <ref name="LabelID"/>
+    </optional>
+    <optional>
       <ref name="PermanentID"/>
     </optional>
     <optional>
+      <ref name="Component"/>
+    </optional>
+    <optional>
       <ref name="XMLBase"/>
     </optional>
     <optional>
       <ref name="XMLLang"/>
     </optional>
     <ref name="Title"/>
     <optional>
@@ -3016,17 +3107,23 @@
     </zeroOrMore>
   </define>
   <define name="MetaDataLinedTitle">
     <optional>
       <ref name="UniqueID"/>
     </optional>
     <optional>
+      <ref name="LabelID"/>
+    </optional>
+    <optional>
       <ref name="PermanentID"/>
     </optional>
     <optional>
+      <ref name="Component"/>
+    </optional>
+    <optional>
       <ref name="XMLBase"/>
     </optional>
     <optional>
       <ref name="XMLLang"/>
     </optional>
     <choice>
       <ref name="Title"/>
@@ -3043,17 +3140,23 @@
     </zeroOrMore>
   </define>
   <define name="MetaDataSubtitle">
     <optional>
       <ref name="UniqueID"/>
     </optional>
     <optional>
+      <ref name="LabelID"/>
+    </optional>
+    <optional>
       <ref name="PermanentID"/>
     </optional>
     <optional>
+      <ref name="Component"/>
+    </optional>
+    <optional>
       <ref name="XMLBase"/>
     </optional>
     <optional>
       <ref name="XMLLang"/>
     </optional>
     <ref name="Title"/>
     <optional>
@@ -3070,17 +3173,23 @@
     </zeroOrMore>
   </define>
   <define name="MetaDataLinedSubtitle">
     <optional>
       <ref name="UniqueID"/>
     </optional>
     <optional>
+      <ref name="LabelID"/>
+    </optional>
+    <optional>
       <ref name="PermanentID"/>
     </optional>
     <optional>
+      <ref name="Component"/>
+    </optional>
+    <optional>
       <ref name="XMLBase"/>
     </optional>
     <optional>
       <ref name="XMLLang"/>
     </optional>
     <choice>
       <ref name="Title"/>
@@ -3103,17 +3212,23 @@
     </zeroOrMore>
   </define>
   <define name="MetaDataTitleOptional">
     <optional>
       <ref name="UniqueID"/>
     </optional>
     <optional>
+      <ref name="LabelID"/>
+    </optional>
+    <optional>
       <ref name="PermanentID"/>
     </optional>
     <optional>
+      <ref name="Component"/>
+    </optional>
+    <optional>
       <ref name="XMLBase"/>
     </optional>
     <optional>
       <ref name="XMLLang"/>
     </optional>
     <optional>
       <ref name="Title"/>
@@ -3123,17 +3238,23 @@
     </zeroOrMore>
   </define>
   <define name="MetaDataAltTitleOptional">
     <optional>
       <ref name="UniqueID"/>
     </optional>
     <optional>
+      <ref name="LabelID"/>
+    </optional>
+    <optional>
       <ref name="PermanentID"/>
     </optional>
     <optional>
+      <ref name="Component"/>
+    </optional>
+    <optional>
       <ref name="XMLBase"/>
     </optional>
     <optional>
       <ref name="XMLLang"/>
     </optional>
     <optional>
       <ref name="Title"/>
@@ -3149,17 +3270,23 @@
     </zeroOrMore>
   </define>
   <define name="MetaDataTitleCreatorOptional">
     <optional>
       <ref name="UniqueID"/>
     </optional>
     <optional>
+      <ref name="LabelID"/>
+    </optional>
+    <optional>
       <ref name="PermanentID"/>
     </optional>
     <optional>
+      <ref name="Component"/>
+    </optional>
+    <optional>
       <ref name="XMLBase"/>
     </optional>
     <optional>
       <ref name="XMLLang"/>
     </optional>
     <optional>
       <ref name="Title"/>
@@ -3172,17 +3299,23 @@
     </zeroOrMore>
   </define>
   <define name="MetaDataCaption">
     <optional>
       <ref name="UniqueID"/>
     </optional>
     <optional>
+      <ref name="LabelID"/>
+    </optional>
+    <optional>
       <ref name="PermanentID"/>
     </optional>
     <optional>
+      <ref name="Component"/>
+    </optional>
+    <optional>
       <ref name="XMLBase"/>
     </optional>
     <optional>
       <ref name="XMLLang"/>
     </optional>
     <optional>
       <ref name="Title"/>
@@ -3216,27 +3349,39 @@
   </define>
   <define name="Paragraph">
     <element name="p">
       <optional>
         <ref name="UniqueID"/>
       </optional>
       <optional>
+        <ref name="LabelID"/>
+      </optional>
+      <optional>
         <ref name="PermanentID"/>
       </optional>
+      <optional>
+        <ref name="Component"/>
+      </optional>
       <ref name="TextParagraph"/>
     </element>
   </define>
   <define name="ParagraphLined">
     <element name="p">
       <optional>
         <ref name="UniqueID"/>
       </optional>
       <optional>
+        <ref name="LabelID"/>
+      </optional>
+      <optional>
         <ref name="PermanentID"/>
       </optional>
+      <optional>
+        <ref name="Component"/>
+      </optional>
       <oneOrMore>
         <element name="line">
           <ref name="TextShort"/>
         </element>
       </oneOrMore>
     </element>
   </define>
```

#### schema/pretext.xsd

##### schema/pretext.xsd

```diff
@@ -1135,26 +1135,28 @@
           <xs:complexType mixed="true">
             <xs:attribute name="prompt"/>
           </xs:complexType>
         </xs:element>
         <xs:element minOccurs="0" ref="output"/>
       </xs:sequence>
       <xs:attribute name="permid"/>
+      <xs:attribute name="component"/>
       <xs:attribute name="prompt"/>
       <xs:attribute name="width"/>
       <xs:attribute name="margins"/>
     </xs:complexType>
   </xs:element>
   <xs:element name="output" type="xs:string"/>
   <xs:element name="program">
     <xs:complexType>
       <xs:sequence>
         <xs:element name="input" type="xs:string"/>
       </xs:sequence>
       <xs:attribute name="permid"/>
+      <xs:attribute name="component"/>
       <xs:attribute name="width"/>
       <xs:attribute name="margins"/>
       <xs:attribute name="language"/>
       <xs:attribute name="line-numbers">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="yes"/>
@@ -1192,14 +1194,15 @@
                 <xs:attributeGroup ref="MetaDataTarget"/>
                 <xs:attribute ref="xml:base"/>
                 <xs:attribute ref="xml:lang"/>
               </xs:complexType>
             </xs:element>
           </xs:sequence>
           <xs:attribute name="permid"/>
+          <xs:attribute name="component"/>
           <xs:attribute name="cols">
             <xs:simpleType>
               <xs:restriction base="xs:token">
                 <xs:enumeration value="2"/>
                 <xs:enumeration value="3"/>
                 <xs:enumeration value="4"/>
                 <xs:enumeration value="5"/>
@@ -1232,14 +1235,15 @@
             <xs:attributeGroup ref="MetaDataTarget"/>
             <xs:attribute ref="xml:base"/>
             <xs:attribute ref="xml:lang"/>
           </xs:complexType>
         </xs:element>
       </xs:sequence>
       <xs:attribute name="permid"/>
+      <xs:attribute name="component"/>
       <xs:attribute name="cols">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="2"/>
             <xs:enumeration value="3"/>
             <xs:enumeration value="4"/>
             <xs:enumeration value="5"/>
@@ -1269,14 +1273,15 @@
                 <xs:group maxOccurs="unbounded" ref="BlockStatement"/>
               </xs:extension>
             </xs:complexContent>
           </xs:complexType>
         </xs:element>
       </xs:sequence>
       <xs:attribute name="permid"/>
+      <xs:attribute name="component"/>
       <xs:attribute name="width">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="narrow"/>
             <xs:enumeration value="medium"/>
             <xs:enumeration value="wide"/>
           </xs:restriction>
@@ -1657,14 +1662,15 @@
         <xs:element ref="pre"/>
         <xs:group ref="List"/>
       </xs:choice>
     </xs:complexType>
   </xs:element>
   <xs:attributeGroup name="SidebySideAttributes">
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
     <xs:attribute name="margins"/>
     <xs:attribute name="width"/>
     <xs:attribute name="widths"/>
     <xs:attribute name="valign">
       <xs:simpleType>
         <xs:restriction base="xs:token">
           <xs:enumeration value="top"/>
@@ -1744,27 +1750,28 @@
       <xs:group ref="ImageCode"/>
     </xs:choice>
   </xs:group>
   <xs:group name="ImageRaster">
     <xs:sequence>
       <xs:element name="image">
         <xs:complexType>
-          <xs:sequence minOccurs="0">
+          <xs:choice minOccurs="0" maxOccurs="unbounded">
             <xs:element name="shortdescription" type="xs:string"/>
-            <xs:element minOccurs="0" name="description">
+            <xs:element name="description">
               <xs:complexType>
                 <xs:choice maxOccurs="unbounded">
                   <xs:group ref="Paragraph"/>
                   <xs:element ref="tabular"/>
                 </xs:choice>
               </xs:complexType>
             </xs:element>
-          </xs:sequence>
+          </xs:choice>
           <xs:attribute ref="xml:id"/>
           <xs:attribute name="permid"/>
+          <xs:attribute name="component"/>
           <xs:attribute name="width"/>
           <xs:attribute name="margins"/>
           <xs:attribute name="rotate"/>
           <xs:attribute name="archive"/>
           <xs:attribute name="source" use="required"/>
           <xs:attribute name="decorative">
             <xs:simpleType>
@@ -1778,40 +1785,44 @@
       </xs:element>
     </xs:sequence>
   </xs:group>
   <xs:group name="ImageCode">
     <xs:sequence>
       <xs:element name="image">
         <xs:complexType>
-          <xs:sequence>
-            <xs:sequence minOccurs="0">
-              <xs:element name="shortdescription">
+          <xs:choice minOccurs="0" maxOccurs="unbounded">
+            <xs:element name="shortdescription">
+              <xs:complexType mixed="true">
+                <xs:sequence>
+                  <xs:element minOccurs="0" maxOccurs="unbounded" ref="var"/>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="description">
+              <xs:complexType>
+                <xs:choice maxOccurs="unbounded">
+                  <xs:group ref="Paragraph"/>
+                  <xs:element ref="tabular"/>
+                </xs:choice>
+              </xs:complexType>
+            </xs:element>
+            <xs:choice>
+              <xs:element name="latex-image">
                 <xs:complexType mixed="true">
-                  <xs:sequence>
-                    <xs:element minOccurs="0" maxOccurs="unbounded" ref="var"/>
-                  </xs:sequence>
+                  <xs:attribute name="label"/>
+                  <xs:attribute name="component"/>
                 </xs:complexType>
               </xs:element>
-              <xs:element minOccurs="0" name="description">
-                <xs:complexType>
-                  <xs:choice maxOccurs="unbounded">
-                    <xs:group ref="Paragraph"/>
-                    <xs:element ref="tabular"/>
-                  </xs:choice>
-                </xs:complexType>
-              </xs:element>
-            </xs:sequence>
-            <xs:choice>
-              <xs:element ref="latex-image"/>
               <xs:element ref="asymptote"/>
               <xs:element ref="sageplot"/>
             </xs:choice>
-          </xs:sequence>
+          </xs:choice>
           <xs:attribute ref="xml:id"/>
           <xs:attribute name="permid"/>
+          <xs:attribute name="component"/>
           <xs:attribute name="width"/>
           <xs:attribute name="margins"/>
           <xs:attribute name="archive"/>
           <xs:attribute name="decorative">
             <xs:simpleType>
               <xs:restriction base="xs:token">
                 <xs:enumeration value="yes"/>
@@ -1819,18 +1830,24 @@
               </xs:restriction>
             </xs:simpleType>
           </xs:attribute>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
   </xs:group>
-  <xs:element name="latex-image" type="xs:string"/>
-  <xs:element name="asymptote" type="xs:string"/>
+  <xs:element name="asymptote">
+    <xs:complexType mixed="true">
+      <xs:attribute name="label"/>
+      <xs:attribute name="component"/>
+    </xs:complexType>
+  </xs:element>
   <xs:element name="sageplot">
     <xs:complexType mixed="true">
+      <xs:attribute name="label"/>
+      <xs:attribute name="component"/>
       <xs:attribute name="variant">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="2d"/>
             <xs:enumeration value="3d"/>
           </xs:restriction>
         </xs:simpleType>
@@ -1838,34 +1855,32 @@
       <xs:attribute name="aspect"/>
     </xs:complexType>
   </xs:element>
   <xs:group name="ImageWW">
     <xs:sequence>
       <xs:element name="image">
         <xs:complexType>
-          <xs:sequence>
-            <xs:sequence minOccurs="0">
-              <xs:element name="shortdescription">
-                <xs:complexType mixed="true">
-                  <xs:sequence>
-                    <xs:element minOccurs="0" maxOccurs="unbounded" ref="var"/>
-                  </xs:sequence>
-                </xs:complexType>
-              </xs:element>
-              <xs:element minOccurs="0" name="description">
-                <xs:complexType>
-                  <xs:choice maxOccurs="unbounded">
-                    <xs:group ref="Paragraph"/>
-                    <xs:element ref="tabular"/>
-                  </xs:choice>
-                </xs:complexType>
-              </xs:element>
-            </xs:sequence>
-            <xs:element minOccurs="0" ref="latex-image"/>
-          </xs:sequence>
+          <xs:choice minOccurs="0" maxOccurs="unbounded">
+            <xs:element name="shortdescription">
+              <xs:complexType mixed="true">
+                <xs:sequence>
+                  <xs:element minOccurs="0" maxOccurs="unbounded" ref="var"/>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="description">
+              <xs:complexType>
+                <xs:choice maxOccurs="unbounded">
+                  <xs:group ref="Paragraph"/>
+                  <xs:element ref="tabular"/>
+                </xs:choice>
+              </xs:complexType>
+            </xs:element>
+            <xs:element name="latex-image" type="xs:string"/>
+          </xs:choice>
           <xs:attribute name="pg-name"/>
           <xs:attribute name="width"/>
           <xs:attribute name="decorative">
             <xs:simpleType>
               <xs:restriction base="xs:token">
                 <xs:enumeration value="yes"/>
                 <xs:enumeration value="no"/>
@@ -1947,14 +1962,15 @@
         <xs:element maxOccurs="unbounded" ref="cell"/>
       </xs:sequence>
       <xs:attribute name="header">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="yes"/>
             <xs:enumeration value="no"/>
+            <xs:enumeration value="vertical"/>
           </xs:restriction>
         </xs:simpleType>
       </xs:attribute>
       <xs:attribute name="halign">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="left"/>
@@ -1997,14 +2013,15 @@
   <xs:element name="tabular">
     <xs:complexType>
       <xs:sequence>
         <xs:element minOccurs="0" maxOccurs="unbounded" ref="col"/>
         <xs:element maxOccurs="unbounded" ref="row"/>
       </xs:sequence>
       <xs:attribute name="permid"/>
+      <xs:attribute name="component"/>
       <xs:attribute name="width"/>
       <xs:attribute name="margins"/>
       <xs:attribute name="row-headers">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="yes"/>
             <xs:enumeration value="no"/>
@@ -2039,14 +2056,15 @@
   <xs:element name="sage">
     <xs:complexType>
       <xs:sequence minOccurs="0">
         <xs:element name="input" type="xs:string"/>
         <xs:element minOccurs="0" ref="output"/>
       </xs:sequence>
       <xs:attribute name="permid"/>
+      <xs:attribute name="component"/>
       <xs:attribute name="doctest"/>
       <xs:attribute name="tolerance"/>
       <xs:attribute name="auto-evaluate">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="no"/>
             <xs:enumeration value="yes"/>
@@ -2062,15 +2080,17 @@
       <xs:attribute name="musescoreuser" use="required"/>
       <xs:attribute name="musescore" use="required"/>
     </xs:complexType>
   </xs:element>
   <xs:element name="video">
     <xs:complexType>
       <xs:attribute ref="xml:id"/>
+      <xs:attribute name="label"/>
       <xs:attribute name="permid"/>
+      <xs:attribute name="component"/>
       <xs:attribute name="width"/>
       <xs:attribute name="margins"/>
       <xs:attribute name="aspect"/>
       <xs:attribute name="start" type="xs:integer"/>
       <xs:attribute name="end" type="xs:integer"/>
       <xs:attribute name="play-at">
         <xs:simpleType>
@@ -2441,14 +2461,16 @@
                 <xs:group minOccurs="0" ref="IntroductionText"/>
                 <xs:group maxOccurs="unbounded" ref="TaskWW"/>
                 <xs:group minOccurs="0" ref="ConclusionText"/>
               </xs:sequence>
             </xs:choice>
           </xs:sequence>
           <xs:attribute ref="xml:id"/>
+          <xs:attribute name="label"/>
+          <xs:attribute name="component"/>
           <xs:attribute name="seed" type="xs:integer"/>
           <xs:attribute name="copy"/>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
   </xs:group>
   <xs:element name="pg-code" type="xs:string"/>
@@ -2595,17 +2617,23 @@
         <xs:group maxOccurs="unbounded" ref="LongLine"/>
       </xs:choice>
     </xs:complexType>
   </xs:element>
   <xs:attributeGroup name="UniqueID">
     <xs:attribute ref="xml:id" use="required"/>
   </xs:attributeGroup>
+  <xs:attributeGroup name="LabelID">
+    <xs:attribute name="label" use="required"/>
+  </xs:attributeGroup>
   <xs:attributeGroup name="PermanentID">
     <xs:attribute name="permid" use="required"/>
   </xs:attributeGroup>
+  <xs:attributeGroup name="Component">
+    <xs:attribute name="component" use="required"/>
+  </xs:attributeGroup>
   <xs:group name="Title">
     <xs:sequence>
       <xs:element name="title">
         <xs:complexType mixed="true">
           <xs:group ref="TextLong"/>
         </xs:complexType>
       </xs:element>
@@ -2658,65 +2686,75 @@
   <xs:group name="MetaDataTarget">
     <xs:sequence>
       <xs:element minOccurs="0" maxOccurs="unbounded" ref="idx"/>
     </xs:sequence>
   </xs:group>
   <xs:attributeGroup name="MetaDataTarget">
     <xs:attribute ref="xml:id"/>
+    <xs:attribute name="label"/>
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
   </xs:attributeGroup>
   <xs:complexType name="MetaDataTitle">
     <xs:sequence>
       <xs:group ref="Title"/>
       <xs:element minOccurs="0" maxOccurs="unbounded" ref="idx"/>
     </xs:sequence>
     <xs:attribute ref="xml:id"/>
+    <xs:attribute name="label"/>
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
     <xs:attribute ref="xml:base"/>
     <xs:attribute ref="xml:lang"/>
   </xs:complexType>
   <xs:complexType name="MetaDataAltTitle">
     <xs:sequence>
       <xs:group ref="Title"/>
       <xs:element minOccurs="0" ref="shorttitle"/>
       <xs:element minOccurs="0" ref="plaintitle"/>
       <xs:element minOccurs="0" maxOccurs="unbounded" ref="idx"/>
     </xs:sequence>
     <xs:attribute ref="xml:id"/>
+    <xs:attribute name="label"/>
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
     <xs:attribute ref="xml:base"/>
     <xs:attribute ref="xml:lang"/>
   </xs:complexType>
   <xs:complexType name="MetaDataLinedTitle">
     <xs:sequence>
       <xs:choice>
         <xs:group ref="Title"/>
         <xs:group ref="LinedTitle"/>
       </xs:choice>
       <xs:element minOccurs="0" ref="shorttitle"/>
       <xs:element minOccurs="0" ref="plaintitle"/>
       <xs:element minOccurs="0" maxOccurs="unbounded" ref="idx"/>
     </xs:sequence>
     <xs:attribute ref="xml:id"/>
+    <xs:attribute name="label"/>
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
     <xs:attribute ref="xml:base"/>
     <xs:attribute ref="xml:lang"/>
   </xs:complexType>
   <xs:group name="MetaDataSubtitle">
     <xs:sequence>
       <xs:group ref="Title"/>
       <xs:group minOccurs="0" ref="Subtitle"/>
       <xs:element minOccurs="0" ref="shorttitle"/>
       <xs:element minOccurs="0" ref="plaintitle"/>
       <xs:element minOccurs="0" maxOccurs="unbounded" ref="idx"/>
     </xs:sequence>
   </xs:group>
   <xs:attributeGroup name="MetaDataSubtitle">
     <xs:attribute ref="xml:id"/>
+    <xs:attribute name="label"/>
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
     <xs:attribute ref="xml:base"/>
     <xs:attribute ref="xml:lang"/>
   </xs:attributeGroup>
   <xs:complexType name="MetaDataLinedSubtitle">
     <xs:sequence>
       <xs:choice>
         <xs:group ref="Title"/>
@@ -2727,63 +2765,73 @@
         <xs:group ref="LinedSubtitle"/>
       </xs:choice>
       <xs:element minOccurs="0" ref="shorttitle"/>
       <xs:element minOccurs="0" ref="plaintitle"/>
       <xs:element minOccurs="0" maxOccurs="unbounded" ref="idx"/>
     </xs:sequence>
     <xs:attribute ref="xml:id"/>
+    <xs:attribute name="label"/>
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
     <xs:attribute ref="xml:base"/>
     <xs:attribute ref="xml:lang"/>
   </xs:complexType>
   <xs:group name="MetaDataTitleOptional">
     <xs:sequence>
       <xs:group minOccurs="0" ref="Title"/>
       <xs:element minOccurs="0" maxOccurs="unbounded" ref="idx"/>
     </xs:sequence>
   </xs:group>
   <xs:attributeGroup name="MetaDataTitleOptional">
     <xs:attribute ref="xml:id"/>
+    <xs:attribute name="label"/>
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
     <xs:attribute ref="xml:base"/>
     <xs:attribute ref="xml:lang"/>
   </xs:attributeGroup>
   <xs:complexType name="MetaDataAltTitleOptional">
     <xs:sequence>
       <xs:sequence minOccurs="0">
         <xs:group ref="Title"/>
         <xs:element minOccurs="0" ref="shorttitle"/>
         <xs:element minOccurs="0" ref="plaintitle"/>
       </xs:sequence>
       <xs:element minOccurs="0" maxOccurs="unbounded" ref="idx"/>
     </xs:sequence>
     <xs:attribute ref="xml:id"/>
+    <xs:attribute name="label"/>
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
     <xs:attribute ref="xml:base"/>
     <xs:attribute ref="xml:lang"/>
   </xs:complexType>
   <xs:complexType name="MetaDataTitleCreatorOptional">
     <xs:sequence>
       <xs:group minOccurs="0" ref="Title"/>
       <xs:element minOccurs="0" ref="creator"/>
       <xs:element minOccurs="0" maxOccurs="unbounded" ref="idx"/>
     </xs:sequence>
     <xs:attribute ref="xml:id"/>
+    <xs:attribute name="label"/>
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
     <xs:attribute ref="xml:base"/>
     <xs:attribute ref="xml:lang"/>
   </xs:complexType>
   <xs:complexType name="MetaDataCaption">
     <xs:sequence>
       <xs:group minOccurs="0" ref="Title"/>
       <xs:element ref="caption"/>
       <xs:element minOccurs="0" maxOccurs="unbounded" ref="idx"/>
     </xs:sequence>
     <xs:attribute ref="xml:id"/>
+    <xs:attribute name="label"/>
     <xs:attribute name="permid"/>
+    <xs:attribute name="component"/>
     <xs:attribute ref="xml:base"/>
     <xs:attribute ref="xml:lang"/>
   </xs:complexType>
   <xs:group name="TextParagraph">
     <xs:sequence>
       <xs:choice minOccurs="0" maxOccurs="unbounded">
         <xs:group ref="Character"/>
@@ -2805,15 +2853,17 @@
   </xs:group>
   <xs:group name="Paragraph">
     <xs:sequence>
       <xs:element name="p">
         <xs:complexType mixed="true">
           <xs:group ref="TextParagraph"/>
           <xs:attribute ref="xml:id"/>
+          <xs:attribute name="label"/>
           <xs:attribute name="permid"/>
+          <xs:attribute name="component"/>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
   </xs:group>
   <xs:group name="ParagraphLined">
     <xs:sequence>
       <xs:element name="p">
@@ -2822,15 +2872,17 @@
             <xs:element maxOccurs="unbounded" name="line">
               <xs:complexType mixed="true">
                 <xs:group ref="TextShort"/>
               </xs:complexType>
             </xs:element>
           </xs:sequence>
           <xs:attribute ref="xml:id"/>
+          <xs:attribute name="label"/>
           <xs:attribute name="permid"/>
+          <xs:attribute name="component"/>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
   </xs:group>
   <xs:group name="TextSimple">
     <xs:sequence>
       <xs:group minOccurs="0" maxOccurs="unbounded" ref="Character"/>
```

#### schema/pretext-dev.rnc

```diff
@@ -1,34 +1,106 @@
 
+              namespace xhtml = "http://www.w3.org/1999/xhtml"
                 grammar {
 
                 include "pretext.rnc"
             
             Interactive =
                 element interactive {
                     UniqueID?,
+                    LabelID?,
                     PermanentID?,
+                    Component?,
                     attribute aspect { text }?,
                     attribute width { text }?,
                     attribute platform { text }?,
                     attribute preview { text }?,
                     attribute iframe { text }?,
                     attribute source { text }?,
                     attribute version { text }?,
-                    (Slate | SideBySideNoCaption | SideBySideGroupNoCaption)*,
-                    element instructions { BlockText* | text }?
+                    (
+                      (
+                        Slate |
+                        SideBySideNoCaption |
+                        SideBySideGroupNoCaption
+                      )* &
+                      element instructions { mixed { MetaDataTitleOptional, BlockText } }? &
+                      element static { Image }?
+                    )
+
+                }
+
+            Stack |=
+                element stack {
+                    (
+                        Tabular |
+                        Image |
+                        Video |
+                        Program |
+                        Console |
+                        Paragraph |
+                        Preformatted |
+                        List |
+                        Slate
+                    )+
                 }
 
             Slate =
                 element slate {
                     UniqueID?,
-                    attribute surface { text },
-                    (attribute source { text } | attribute material { text })?,
-                    attribute aspect { text }?,
-                    (Paragraph | Tabular | SideBySideNoCaption)*
+                    LabelID?,
+                    Component?,
+                    (
+                      JessieCodeAtt |
+                      (
+                        attribute surface { text },
+                        (
+                          attribute source { text } |
+                          attribute material { text }
+                        )?,
+                        attribute aspect { text }?,
+                        (
+                          Paragraph |
+                          Tabular |
+                          SideBySideNoCaption |
+                          SlateInput |
+                          element xhtml:button {
+                            attribute type { text },
+                            attribute id { text },
+                            text*
+                          }? |
+                          text*
+                        )*
+                      )
+                    )
+                }
+
+              JessieCodeAtt =
+                attribute surface {"jessiecode"},
+                attribute axis {"true" | "false"}?,
+                attribute grid {"true" | "false"}?,
+                (
+                  attribute source {text} |
+                  text*
+                )
+
+              SlateInput =
+                element xhtml:input {
+                  attribute type {text}?,
+                  attribute value {text}?,
+                  attribute onkeypress {text}?,
+                  attribute onclick {text}?,
+                  attribute style {text}?
+                } |
+                element input {
+                  attribute type {text}?,
+                  attribute value {text}?,
+                  attribute onkeypress {text}?,
+                  attribute onclick {text}?,
+                  attribute style {text}?
                 }
 
             # add Interactives where used
             BlockStatement |= Interactive
 
             Figure |= element figure { MetaDataCaption, Interactive }
 
@@ -353,18 +425,14 @@
                     attribute break {"yes" | "no"}?,
                     attribute alignment {text}?,
                     attribute alignat-columns {text}?,
                     MathRow,
                     (MathRow | MathIntertext)*
                 }
             
-            UniqueID |=
-                attribute xml:id {text}?,
-                attribute label {text}?
-            
             TrueFalse =
                 MetaDataTitleOptional,
                 attribute number {text}?,
                 element statement {
                     attribute correct {"yes"|"no"},
                     Paragraph
                 },
@@ -398,20 +466,20 @@
                     },
                     Hint*, Answer*, Solution*
             Block =
                 element block {
                     attribute order {xsd:integer}?,
                     ((
                         attribute correct {"yes"|"no"}?,
-                        mixed {BlockText?}
+                        mixed {BlockText?, CodeLine?}+
                     ) |
                     (
                         element choice {
                             attribute correct {"yes"|"no"}?,
-                            mixed {BlockText?}
+                            mixed {BlockText?, CodeLine?}+
                         }+
                     ))
                 }
             Matching =
                 MetaDataTitleOptional,
                 attribute number {text}?,
                 StatementExercise,
@@ -436,31 +504,89 @@
                 (
                 (ExerciseBody, Response?) |
                 (StatementExercise, Response?, Hint*, Answer*, Solution*) |
                 (IntroductionStatement?, Task+, ConclusionStatement?)
                 )
             Response =
                 element response {empty}
+
+
+            # Selectable areas
+            Area =
+                element area {
+                    attribute correct {"yes"|"no"}?,
+                    TextLong
+                }
+            TextLongAreas =  mixed { (
+                  Area |
+                  Character |
+                  Generator |
+                  Verbatim |
+                  GroupAreas |
+                  MathInline |
+                  Music |
+                  Reference |
+                  WWVariable)* }
+            GroupAreas |=
+                element q {TextLongAreas} |
+                element sq {TextLongAreas}
+            TextParagraphAreas = mixed { (
+              Character |
+              Generator |
+              Verbatim |
+              Group |
+              WWVariable |
+              MathInline |
+              Music |
+              Reference |
+              CodeDisplay |
+              MathDisplay |
+              List |
+              Footnote |
+              Notation |
+              Index |
+              Area |
+              GroupAreas)* }
+            ParagraphAreas =
+                element p {
+                    UniqueID?,
+                    LabelID?,
+                    PermanentID?,
+                    Component?,
+                    TextParagraphAreas
+                }
+            Areas =
+                MetaDataTitleOptional,
+                attribute number {text}?,
+                StatementExercise,
+                Feedback?,
+                element areas {
+                  ParagraphAreas+
+                },
+                Hint*, Answer*, Solution*
+
             # General feedback element
             Feedback =
                 element feedback {
                     MetaDataTitleOptional,
                     BlockSolution+
                 }
             # Include all exercise types in exercise and activity
             Exercise |=
                 element exercise {
                     TrueFalse |
                     MultipleChoice |
                     Parsons |
                     Matching |
-                    FreeResponse
+                    FreeResponse |
+                    Areas
                 }
             ProjectLike |=
                 TrueFalse |
                 MultipleChoice |
                 Parsons |
                 Matching |
-                FreeResponse
+                FreeResponse |
+                Areas
             
                 }
```

#### schema/pretext.rnc

```diff
@@ -475,64 +475,69 @@
             Preformatted =
                 element pre {
                     text | CodeLine+
                 }
             Console =
                 element console {
                     PermanentID?,
+                    Component?,
                     attribute prompt {text}?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     (
                         element input {
                             attribute prompt {text}?,
                             text
                         },
                         element output {text}?
                     )+
                 }
             Program =
                 element program {
                     PermanentID?,
+                    Component?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     attribute language {text}?,
                     attribute line-numbers {"yes"|"no"}?,
                     attribute highlight-lines {text}?,
                     attribute interactive {"codelens"}?,
                     element input {text}
                 }
             
             List =
                 element ol {
                     PermanentID?,
+                    Component?,
                     attribute cols {"2"|"3"|"4"|"5"|"6"}?,
                     attribute marker {text}?,
                     element li {
                         (
                             (MetaDataTarget, TextParagraph)
                         |
                             (MetaDataTitleOptional, BlockStatement+)
                         )
                     }+
                 } |
                 element ul {
                     PermanentID?,
+                    Component?,
                     attribute cols {"2"|"3"|"4"|"5"|"6"}?,
                     attribute marker {"disc" | "circle" | "square" | ""}?,
                     element li {
                         (
                             (MetaDataTarget, TextParagraph)
                         |
                             (MetaDataTitleOptional, BlockStatement+)
                         )
                     }+
                 } |
                 element dl {
                     PermanentID?,
+                    Component?,
                     attribute width {"narrow" | "medium" | "wide"}?,
                     element li {
                         MetaDataTitle,
                         BlockStatement+
                     }+
                 }
             
@@ -700,14 +705,15 @@
                         Paragraph |
                         Preformatted |
                         List
                     )+
                 }
             SidebySideAttributes =
                 PermanentID?,
+                Component?,
                 attribute margins {text}?,
                 (attribute width {text} | attribute widths {text})?,
                 (AlignmentVertical | attribute valigns {text})?
             SideBySide =
                 element sidebyside {
                     SidebySideAttributes,
                     (
@@ -752,65 +758,86 @@
                 }
             
             Image = ImageRaster | ImageCode
             ImageRaster =
                 element image {
                     UniqueID?,
                     PermanentID?,
+                    Component?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     attribute rotate {text}?,
                     attribute archive {text}?,
                     attribute source {text},
                     (
-                        attribute decorative {"yes" | "no"}? |
+                      attribute decorative {"yes"} |
+                      (
+                        attribute decorative {"no"}?,
                         (
-                            element shortdescription {text},
-                            element description {(Paragraph | Tabular)+}?
+                          element shortdescription {text}? &
+                          element description {(Paragraph | Tabular)+}?
                         )
-                    )?
+                      )
+                    )
                 }
             ImageCode =
                 element image {
                     UniqueID?,
                     PermanentID?,
+                    Component?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     attribute archive {text}?,
                     (
-                        attribute decorative {"yes" | "no"}? |
+                      attribute decorative {"yes"} |
+                      (
+                        attribute decorative {"no"}?,
                         (
-                            element shortdescription {(text | WWVariable)+},
-                            element description {(Paragraph | Tabular)+}?
+                          element shortdescription {(text | WWVariable)+}? &
+                          element description {(Paragraph | Tabular)+}? &
+                          (
+                            element latex-image {
+                              LabelID?,
+                              Component?,
+                              text
+                            } |
+                            element asymptote {
+                              LabelID?,
+                              Component?,
+                              text
+                            } |
+                            element sageplot {
+                                LabelID?,
+                                Component?,
+                                attribute variant {'2d'|'3d'}?,
+                                attribute aspect {text}?,
+                                text
+                            }
+                          )
                         )
-                    )?,
-                    (
-                        element latex-image {text} |
-                        element asymptote {text} |
-                        element sageplot {
-                            attribute variant {'2d'|'3d'}?,
-                            attribute aspect {text}?,
-                            text
-                        }
+                      )
                     )
                 }
             ImageWW =
                 element image {
                     attribute pg-name {text}?,
                     attribute width {text}?,
                     (
-                        attribute decorative {"yes" | "no"}? |
+                      attribute decorative {"yes"} |
+                      (
+                        attribute decorative {"no"}?,
                         (
-                            element shortdescription {(text | WWVariable)+},
-                            element description {(Paragraph | Tabular)+}?
+                          element shortdescription {(text | WWVariable)+}? &
+                          element description {(Paragraph | Tabular)+}? &
+                          element latex-image {
+                            text
+                          }?
                         )
-                    )?,
-                    element latex-image {
-                        text
-                    }?
+                      )
+                    )
                 }
             
             BorderThickness = "none" | "minor" | "medium" | "major"
             BorderTop =
                 attribute top {BorderThickness}
             BorderBottom =
                 attribute bottom {BorderThickness}
@@ -833,15 +860,15 @@
                         TextLong |
                         LongLine+ |
                         Paragraph+
                     )
                 }
             TableRow =
                 element row {
-                    attribute header {"yes" | "no"}?,
+                    attribute header {"yes" | "no" | "vertical"}?,
                     AlignmentHorizontal?,
                     AlignmentVertical?,
                     BorderBottom?,
                     BorderLeft?,
                     TableCell+
                 }
             TableColumn =
@@ -850,14 +877,15 @@
                     BorderTop?,
                     BorderRight?,
                     attribute width {text}?
                 }
             Tabular =
                 element tabular {
                     PermanentID?,
+                    Component?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     attribute row-headers {"yes" | "no"}?,
                     AlignmentHorizontal?,
                     AlignmentVertical?,
                     BorderTop?,
                     BorderBottom?,
@@ -865,14 +893,15 @@
                     BorderRight?,
                     TableColumn*,
                     TableRow+
                 }
             
             Sage = element sage {
                 PermanentID?,
+                Component?,
                 attribute doctest {text}?,
                 attribute tolerance {text}?,
                 attribute auto-evaluate {'no'|'yes'}?,
                 attribute language {text}?,
                 attribute type {text}?,
                 (element input {text}, element output {text}?)?
             }
@@ -882,15 +911,17 @@
                     attribute musescoreuser {text},
                     attribute musescore {text}
                 }
             
             Video =
                 element video {
                     UniqueID?,
+                    LabelID?,
                     PermanentID?,
+                    Component?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     attribute aspect {text}?,
                     attribute start {xsd:integer}?,
                     attribute end {xsd:integer}?,
                     attribute play-at {"embed" | "popout" | "select"}?,
                     attribute preview {"default" | "generic" | text}?,
@@ -1043,14 +1074,16 @@
                 element webwork {
                     attribute source {text}?,
                     attribute seed {xsd:integer}?
                 }
             WebWorkAuthored =
                 element webwork {
                     UniqueID?,
+                    LabelID?,
+                    Component?,
                     attribute seed {xsd:integer}?,
                     attribute copy {text}?,
                     element description {
                         (
                             TextSimple |
                             SimpleLine+
                         )
@@ -1135,16 +1168,20 @@
             Attribution =
                 element attribution {
                     (TextLong | LongLine+)
                 }
             
             UniqueID =
                 attribute xml:id {text}
+            LabelID =
+                attribute label {text}
             PermanentID =
                 attribute permid {text}
+            Component =
+                attribute component {text}
             Title =
                 element title {TextLong}
             LinedTitle =
                 element title {LongLine+}
             Subtitle =
                 element subtitle {TextLong}
             LinedSubtitle =
@@ -1155,86 +1192,106 @@
                 element plaintitle {text}
             Creator =
                 element creator {TextShort}
             XMLBase = attribute xml:base {text}
             XMLLang = attribute xml:lang {text}
             MetaDataTarget =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 Index*
             MetaDataTitle =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title,
                 Index*
             MetaDataAltTitle =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title,
                 ShortTitle?,
                 PlainTitle?,
                 Index*
             MetaDataLinedTitle =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 (Title | LinedTitle),
                 ShortTitle?,
                 PlainTitle?,
                 Index*
             MetaDataSubtitle =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title,
                 Subtitle?,
                 ShortTitle?,
                 PlainTitle?,
                 Index*
             MetaDataLinedSubtitle =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 (Title | LinedTitle),
                 (Subtitle | LinedSubtitle)?,
                 ShortTitle?,
                 PlainTitle?,
                 Index*
             MetaDataTitleOptional =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title?,
                 Index*
             MetaDataAltTitleOptional =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 (Title, ShortTitle?, PlainTitle?)?,
                 Index*
             MetaDataTitleCreatorOptional =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title?,
                 Creator?,
                 Index*
             MetaDataCaption =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title?,
                 Caption,
                 Index*
             
             TextParagraph = mixed { (
@@ -1251,21 +1308,25 @@
                 List |
                 Footnote |
                 Notation |
                 Index)* }
             Paragraph =
                 element p {
                     UniqueID?,
+                    LabelID?,
                     PermanentID?,
+                    Component?,
                     TextParagraph
                 }
             ParagraphLined =
                 element p {
                     UniqueID?,
+                    LabelID?,
                     PermanentID?,
+                    Component?,
                     element line {TextShort}+
                 }
             
             TextSimple = mixed {
                 Character* }
             TextShort = mixed { (
                 Character |
```

#### schema/pretext-dev.rng

##### schema/pretext-dev.rng

```diff
@@ -1,19 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
-<grammar xmlns="http://relaxng.org/ns/structure/1.0" datatypeLibrary="http://www.w3.org/2001/XMLSchema-datatypes">
+<grammar xmlns:xhtml="http://www.w3.org/1999/xhtml" xmlns="http://relaxng.org/ns/structure/1.0" datatypeLibrary="http://www.w3.org/2001/XMLSchema-datatypes">
   <include href="pretext.rng"/>
   <define name="Interactive">
     <element name="interactive">
       <optional>
         <ref name="UniqueID"/>
       </optional>
       <optional>
+        <ref name="LabelID"/>
+      </optional>
+      <optional>
         <ref name="PermanentID"/>
       </optional>
       <optional>
+        <ref name="Component"/>
+      </optional>
+      <optional>
         <attribute name="aspect"/>
       </optional>
       <optional>
         <attribute name="width"/>
       </optional>
       <optional>
         <attribute name="platform"/>
@@ -26,56 +32,167 @@
       </optional>
       <optional>
         <attribute name="source"/>
       </optional>
       <optional>
         <attribute name="version"/>
       </optional>
-      <zeroOrMore>
+      <interleave>
+        <zeroOrMore>
+          <choice>
+            <ref name="Slate"/>
+            <ref name="SideBySideNoCaption"/>
+            <ref name="SideBySideGroupNoCaption"/>
+          </choice>
+        </zeroOrMore>
+        <optional>
+          <element name="instructions">
+            <mixed>
+              <ref name="MetaDataTitleOptional"/>
+              <ref name="BlockText"/>
+            </mixed>
+          </element>
+        </optional>
+        <optional>
+          <element name="static">
+            <ref name="Image"/>
+          </element>
+        </optional>
+      </interleave>
+    </element>
+  </define>
+  <define name="Stack" combine="choice">
+    <element name="stack">
+      <oneOrMore>
         <choice>
+          <ref name="Tabular"/>
+          <ref name="Image"/>
+          <ref name="Video"/>
+          <ref name="Program"/>
+          <ref name="Console"/>
+          <ref name="Paragraph"/>
+          <ref name="Preformatted"/>
+          <ref name="List"/>
           <ref name="Slate"/>
-          <ref name="SideBySideNoCaption"/>
-          <ref name="SideBySideGroupNoCaption"/>
         </choice>
-      </zeroOrMore>
-      <optional>
-        <element name="instructions">
-          <choice>
-            <zeroOrMore>
-              <ref name="BlockText"/>
-            </zeroOrMore>
-            <text/>
-          </choice>
-        </element>
-      </optional>
+      </oneOrMore>
     </element>
   </define>
   <define name="Slate">
     <element name="slate">
       <optional>
         <ref name="UniqueID"/>
       </optional>
-      <attribute name="surface"/>
       <optional>
-        <choice>
-          <attribute name="source"/>
-          <attribute name="material"/>
-        </choice>
+        <ref name="LabelID"/>
       </optional>
       <optional>
-        <attribute name="aspect"/>
+        <ref name="Component"/>
       </optional>
-      <zeroOrMore>
+      <choice>
+        <ref name="JessieCodeAtt"/>
+        <group>
+          <attribute name="surface"/>
+          <optional>
+            <choice>
+              <attribute name="source"/>
+              <attribute name="material"/>
+            </choice>
+          </optional>
+          <optional>
+            <attribute name="aspect"/>
+          </optional>
+          <zeroOrMore>
+            <choice>
+              <ref name="Paragraph"/>
+              <ref name="Tabular"/>
+              <ref name="SideBySideNoCaption"/>
+              <ref name="SlateInput"/>
+              <optional>
+                <element name="xhtml:button">
+                  <attribute name="type"/>
+                  <attribute name="id"/>
+                  <zeroOrMore>
+                    <text/>
+                  </zeroOrMore>
+                </element>
+              </optional>
+              <zeroOrMore>
+                <text/>
+              </zeroOrMore>
+            </choice>
+          </zeroOrMore>
+        </group>
+      </choice>
+    </element>
+  </define>
+  <define name="JessieCodeAtt">
+    <attribute name="surface">
+      <value>jessiecode</value>
+    </attribute>
+    <optional>
+      <attribute name="axis">
         <choice>
-          <ref name="Paragraph"/>
-          <ref name="Tabular"/>
-          <ref name="SideBySideNoCaption"/>
+          <value>true</value>
+          <value>false</value>
         </choice>
+      </attribute>
+    </optional>
+    <optional>
+      <attribute name="grid">
+        <choice>
+          <value>true</value>
+          <value>false</value>
+        </choice>
+      </attribute>
+    </optional>
+    <choice>
+      <attribute name="source"/>
+      <zeroOrMore>
+        <text/>
       </zeroOrMore>
-    </element>
+    </choice>
+  </define>
+  <define name="SlateInput">
+    <choice>
+      <element name="xhtml:input">
+        <optional>
+          <attribute name="type"/>
+        </optional>
+        <optional>
+          <attribute name="value"/>
+        </optional>
+        <optional>
+          <attribute name="onkeypress"/>
+        </optional>
+        <optional>
+          <attribute name="onclick"/>
+        </optional>
+        <optional>
+          <attribute name="style"/>
+        </optional>
+      </element>
+      <element name="input">
+        <optional>
+          <attribute name="type"/>
+        </optional>
+        <optional>
+          <attribute name="value"/>
+        </optional>
+        <optional>
+          <attribute name="onkeypress"/>
+        </optional>
+        <optional>
+          <attribute name="onclick"/>
+        </optional>
+        <optional>
+          <attribute name="style"/>
+        </optional>
+      </element>
+    </choice>
   </define>
   <!-- add Interactives where used -->
   <define name="BlockStatement" combine="choice">
     <ref name="Interactive"/>
   </define>
   <define name="Figure" combine="choice">
     <element name="figure">
@@ -1007,22 +1124,14 @@
             <ref name="MathRow"/>
             <ref name="MathIntertext"/>
           </choice>
         </zeroOrMore>
       </element>
     </choice>
   </define>
-  <define name="UniqueID" combine="choice">
-    <optional>
-      <attribute name="xml:id"/>
-    </optional>
-    <optional>
-      <attribute name="label"/>
-    </optional>
-  </define>
   <define name="TrueFalse">
     <ref name="MetaDataTitleOptional"/>
     <optional>
       <attribute name="number"/>
     </optional>
     <element name="statement">
       <attribute name="correct">
@@ -1161,35 +1270,45 @@
             <attribute name="correct">
               <choice>
                 <value>yes</value>
                 <value>no</value>
               </choice>
             </attribute>
           </optional>
-          <mixed>
-            <optional>
-              <ref name="BlockText"/>
-            </optional>
-          </mixed>
+          <oneOrMore>
+            <mixed>
+              <optional>
+                <ref name="BlockText"/>
+              </optional>
+              <optional>
+                <ref name="CodeLine"/>
+              </optional>
+            </mixed>
+          </oneOrMore>
         </group>
         <oneOrMore>
           <element name="choice">
             <optional>
               <attribute name="correct">
                 <choice>
                   <value>yes</value>
                   <value>no</value>
                 </choice>
               </attribute>
             </optional>
-            <mixed>
-              <optional>
-                <ref name="BlockText"/>
-              </optional>
-            </mixed>
+            <oneOrMore>
+              <mixed>
+                <optional>
+                  <ref name="BlockText"/>
+                </optional>
+                <optional>
+                  <ref name="CodeLine"/>
+                </optional>
+              </mixed>
+            </oneOrMore>
           </element>
         </oneOrMore>
       </choice>
     </element>
   </define>
   <define name="Matching">
     <ref name="MetaDataTitleOptional"/>
@@ -1279,14 +1398,120 @@
     </choice>
   </define>
   <define name="Response">
     <element name="response">
       <empty/>
     </element>
   </define>
+  <!-- Selectable areas -->
+  <define name="Area">
+    <element name="area">
+      <optional>
+        <attribute name="correct">
+          <choice>
+            <value>yes</value>
+            <value>no</value>
+          </choice>
+        </attribute>
+      </optional>
+      <ref name="TextLong"/>
+    </element>
+  </define>
+  <define name="TextLongAreas">
+    <mixed>
+      <zeroOrMore>
+        <choice>
+          <ref name="Area"/>
+          <ref name="Character"/>
+          <ref name="Generator"/>
+          <ref name="Verbatim"/>
+          <ref name="GroupAreas"/>
+          <ref name="MathInline"/>
+          <ref name="Music"/>
+          <ref name="Reference"/>
+          <ref name="WWVariable"/>
+        </choice>
+      </zeroOrMore>
+    </mixed>
+  </define>
+  <define name="GroupAreas" combine="choice">
+    <choice>
+      <element name="q">
+        <ref name="TextLongAreas"/>
+      </element>
+      <element name="sq">
+        <ref name="TextLongAreas"/>
+      </element>
+    </choice>
+  </define>
+  <define name="TextParagraphAreas">
+    <mixed>
+      <zeroOrMore>
+        <choice>
+          <ref name="Character"/>
+          <ref name="Generator"/>
+          <ref name="Verbatim"/>
+          <ref name="Group"/>
+          <ref name="WWVariable"/>
+          <ref name="MathInline"/>
+          <ref name="Music"/>
+          <ref name="Reference"/>
+          <ref name="CodeDisplay"/>
+          <ref name="MathDisplay"/>
+          <ref name="List"/>
+          <ref name="Footnote"/>
+          <ref name="Notation"/>
+          <ref name="Index"/>
+          <ref name="Area"/>
+          <ref name="GroupAreas"/>
+        </choice>
+      </zeroOrMore>
+    </mixed>
+  </define>
+  <define name="ParagraphAreas">
+    <element name="p">
+      <optional>
+        <ref name="UniqueID"/>
+      </optional>
+      <optional>
+        <ref name="LabelID"/>
+      </optional>
+      <optional>
+        <ref name="PermanentID"/>
+      </optional>
+      <optional>
+        <ref name="Component"/>
+      </optional>
+      <ref name="TextParagraphAreas"/>
+    </element>
+  </define>
+  <define name="Areas">
+    <ref name="MetaDataTitleOptional"/>
+    <optional>
+      <attribute name="number"/>
+    </optional>
+    <ref name="StatementExercise"/>
+    <optional>
+      <ref name="Feedback"/>
+    </optional>
+    <element name="areas">
+      <oneOrMore>
+        <ref name="ParagraphAreas"/>
+      </oneOrMore>
+    </element>
+    <zeroOrMore>
+      <ref name="Hint"/>
+    </zeroOrMore>
+    <zeroOrMore>
+      <ref name="Answer"/>
+    </zeroOrMore>
+    <zeroOrMore>
+      <ref name="Solution"/>
+    </zeroOrMore>
+  </define>
   <!-- General feedback element -->
   <define name="Feedback">
     <element name="feedback">
       <ref name="MetaDataTitleOptional"/>
       <oneOrMore>
         <ref name="BlockSolution"/>
       </oneOrMore>
@@ -1297,20 +1522,22 @@
     <element name="exercise">
       <choice>
         <ref name="TrueFalse"/>
         <ref name="MultipleChoice"/>
         <ref name="Parsons"/>
         <ref name="Matching"/>
         <ref name="FreeResponse"/>
+        <ref name="Areas"/>
       </choice>
     </element>
   </define>
   <define name="ProjectLike" combine="choice">
     <choice>
       <ref name="TrueFalse"/>
       <ref name="MultipleChoice"/>
       <ref name="Parsons"/>
       <ref name="Matching"/>
       <ref name="FreeResponse"/>
+      <ref name="Areas"/>
     </choice>
   </define>
 </grammar>
```

#### schema/pretext.xml

##### schema/pretext.xml

```diff
@@ -767,21 +767,25 @@
                 List |
                 Footnote |
                 Notation |
                 Index)* }
             Paragraph =
                 element p {
                     UniqueID?,
+                    LabelID?,
                     PermanentID?,
+                    Component?,
                     TextParagraph
                 }
             ParagraphLined =
                 element p {
                     UniqueID?,
+                    LabelID?,
                     PermanentID?,
+                    Component?,
                     element line {TextShort}+
                 }</code>
       </fragment>
       <p>
         Fundamentally
         <pretext/>
         allows for conversion to other markup languages, such as
@@ -1637,28 +1641,30 @@
             Preformatted =
                 element pre {
                     text | CodeLine+
                 }
             Console =
                 element console {
                     PermanentID?,
+                    Component?,
                     attribute prompt {text}?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     (
                         element input {
                             attribute prompt {text}?,
                             text
                         },
                         element output {text}?
                     )+
                 }
             Program =
                 element program {
                     PermanentID?,
+                    Component?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     attribute language {text}?,
                     attribute line-numbers {&quot;yes&quot;|&quot;no&quot;}?,
                     attribute highlight-lines {text}?,
                     attribute interactive {&quot;codelens&quot;}?,
                     element input {text}
@@ -1674,38 +1680,41 @@
         and point to that.
       </p>
       <fragment xml:id="list">
         <title>Lists</title>
         <code>List =
                 element ol {
                     PermanentID?,
+                    Component?,
                     attribute cols {&quot;2&quot;|&quot;3&quot;|&quot;4&quot;|&quot;5&quot;|&quot;6&quot;}?,
                     attribute marker {text}?,
                     element li {
                         (
                             (MetaDataTarget, TextParagraph)
                         |
                             (MetaDataTitleOptional, BlockStatement+)
                         )
                     }+
                 } |
                 element ul {
                     PermanentID?,
+                    Component?,
                     attribute cols {&quot;2&quot;|&quot;3&quot;|&quot;4&quot;|&quot;5&quot;|&quot;6&quot;}?,
                     attribute marker {&quot;disc&quot; | &quot;circle&quot; | &quot;square&quot; | &quot;&quot;}?,
                     element li {
                         (
                             (MetaDataTarget, TextParagraph)
                         |
                             (MetaDataTitleOptional, BlockStatement+)
                         )
                     }+
                 } |
                 element dl {
                     PermanentID?,
+                    Component?,
                     attribute width {&quot;narrow&quot; | &quot;medium&quot; | &quot;wide&quot;}?,
                     element li {
                         MetaDataTitle,
                         BlockStatement+
                     }+
                 }</code>
       </fragment>
@@ -2004,15 +2013,15 @@
                         TextLong |
                         LongLine+ |
                         Paragraph+
                     )
                 }
             TableRow =
                 element row {
-                    attribute header {&quot;yes&quot; | &quot;no&quot;}?,
+                    attribute header {&quot;yes&quot; | &quot;no&quot; | &quot;vertical&quot;}?,
                     AlignmentHorizontal?,
                     AlignmentVertical?,
                     BorderBottom?,
                     BorderLeft?,
                     TableCell+
                 }
             TableColumn =
@@ -2021,14 +2030,15 @@
                     BorderTop?,
                     BorderRight?,
                     attribute width {text}?
                 }
             Tabular =
                 element tabular {
                     PermanentID?,
+                    Component?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     attribute row-headers {&quot;yes&quot; | &quot;no&quot;}?,
                     AlignmentHorizontal?,
                     AlignmentVertical?,
                     BorderTop?,
                     BorderBottom?,
@@ -2098,14 +2108,15 @@
                         Paragraph |
                         Preformatted |
                         List
                     )+
                 }
             SidebySideAttributes =
                 PermanentID?,
+                Component?,
                 attribute margins {text}?,
                 (attribute width {text} | attribute widths {text})?,
                 (AlignmentVertical | attribute valigns {text})?
             SideBySide =
                 element sidebyside {
                     SidebySideAttributes,
                     (
@@ -2167,75 +2178,97 @@
       <fragment xml:id="image">
         <title>Images</title>
         <code>Image = ImageRaster | ImageCode
             ImageRaster =
                 element image {
                     UniqueID?,
                     PermanentID?,
+                    Component?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     attribute rotate {text}?,
                     attribute archive {text}?,
                     attribute source {text},
                     (
-                        attribute decorative {&quot;yes&quot; | &quot;no&quot;}? |
+                      attribute decorative {&quot;yes&quot;} |
+                      (
+                        attribute decorative {&quot;no&quot;}?,
                         (
-                            element shortdescription {text},
-                            element description {(Paragraph | Tabular)+}?
+                          element shortdescription {text}? &amp;
+                          element description {(Paragraph | Tabular)+}?
                         )
-                    )?
+                      )
+                    )
                 }
             ImageCode =
                 element image {
                     UniqueID?,
                     PermanentID?,
+                    Component?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     attribute archive {text}?,
                     (
-                        attribute decorative {&quot;yes&quot; | &quot;no&quot;}? |
+                      attribute decorative {&quot;yes&quot;} |
+                      (
+                        attribute decorative {&quot;no&quot;}?,
                         (
-                            element shortdescription {(text | WWVariable)+},
-                            element description {(Paragraph | Tabular)+}?
+                          element shortdescription {(text | WWVariable)+}? &amp;
+                          element description {(Paragraph | Tabular)+}? &amp;
+                          (
+                            element latex-image {
+                              LabelID?,
+                              Component?,
+                              text
+                            } |
+                            element asymptote {
+                              LabelID?,
+                              Component?,
+                              text
+                            } |
+                            element sageplot {
+                                LabelID?,
+                                Component?,
+                                attribute variant {'2d'|'3d'}?,
+                                attribute aspect {text}?,
+                                text
+                            }
+                          )
                         )
-                    )?,
-                    (
-                        element latex-image {text} |
-                        element asymptote {text} |
-                        element sageplot {
-                            attribute variant {'2d'|'3d'}?,
-                            attribute aspect {text}?,
-                            text
-                        }
+                      )
                     )
                 }
             ImageWW =
                 element image {
                     attribute pg-name {text}?,
                     attribute width {text}?,
                     (
-                        attribute decorative {&quot;yes&quot; | &quot;no&quot;}? |
+                      attribute decorative {&quot;yes&quot;} |
+                      (
+                        attribute decorative {&quot;no&quot;}?,
                         (
-                            element shortdescription {(text | WWVariable)+},
-                            element description {(Paragraph | Tabular)+}?
+                          element shortdescription {(text | WWVariable)+}? &amp;
+                          element description {(Paragraph | Tabular)+}? &amp;
+                          element latex-image {
+                            text
+                          }?
                         )
-                    )?,
-                    element latex-image {
-                        text
-                    }?
+                      )
+                    )
                 }</code>
       </fragment>
     </section>
     <section>
       <title>Sage Code</title>
       <p>Sage is integral.</p>
       <fragment xml:id="sage">
         <title>Sage code</title>
         <code>Sage = element sage {
                 PermanentID?,
+                Component?,
                 attribute doctest {text}?,
                 attribute tolerance {text}?,
                 attribute auto-evaluate {'no'|'yes'}?,
                 attribute language {text}?,
                 attribute type {text}?,
                 (element input {text}, element output {text}?)?
             }</code>
@@ -2265,33 +2298,104 @@
         element.
       </p>
       <fragment xml:id="interactive">
         <title>Interactives</title>
         <code>Interactive =
                 element interactive {
                     UniqueID?,
+                    LabelID?,
                     PermanentID?,
+                    Component?,
                     attribute aspect { text }?,
                     attribute width { text }?,
                     attribute platform { text }?,
                     attribute preview { text }?,
                     attribute iframe { text }?,
                     attribute source { text }?,
                     attribute version { text }?,
-                    (Slate | SideBySideNoCaption | SideBySideGroupNoCaption)*,
-                    element instructions { BlockText* | text }?
+                    (
+                      (
+                        Slate |
+                        SideBySideNoCaption |
+                        SideBySideGroupNoCaption
+                      )* &amp;
+                      element instructions { mixed { MetaDataTitleOptional, BlockText } }? &amp;
+                      element static { Image }?
+                    )
+
+                }
+
+            Stack |=
+                element stack {
+                    (
+                        Tabular |
+                        Image |
+                        Video |
+                        Program |
+                        Console |
+                        Paragraph |
+                        Preformatted |
+                        List |
+                        Slate
+                    )+
                 }
 
             Slate =
                 element slate {
                     UniqueID?,
-                    attribute surface { text },
-                    (attribute source { text } | attribute material { text })?,
-                    attribute aspect { text }?,
-                    (Paragraph | Tabular | SideBySideNoCaption)*
+                    LabelID?,
+                    Component?,
+                    (
+                      JessieCodeAtt |
+                      (
+                        attribute surface { text },
+                        (
+                          attribute source { text } |
+                          attribute material { text }
+                        )?,
+                        attribute aspect { text }?,
+                        (
+                          Paragraph |
+                          Tabular |
+                          SideBySideNoCaption |
+                          SlateInput |
+                          element xhtml:button {
+                            attribute type { text },
+                            attribute id { text },
+                            text*
+                          }? |
+                          text*
+                        )*
+                      )
+                    )
+                }
+
+              JessieCodeAtt =
+                attribute surface {&quot;jessiecode&quot;},
+                attribute axis {&quot;true&quot; | &quot;false&quot;}?,
+                attribute grid {&quot;true&quot; | &quot;false&quot;}?,
+                (
+                  attribute source {text} |
+                  text*
+                )
+
+              SlateInput =
+                element xhtml:input {
+                  attribute type {text}?,
+                  attribute value {text}?,
+                  attribute onkeypress {text}?,
+                  attribute onclick {text}?,
+                  attribute style {text}?
+                } |
+                element input {
+                  attribute type {text}?,
+                  attribute value {text}?,
+                  attribute onkeypress {text}?,
+                  attribute onclick {text}?,
+                  attribute style {text}?
                 }
 
             # add Interactives where used
             BlockStatement |= Interactive
 
             Figure |= element figure { MetaDataCaption, Interactive }
 
@@ -2337,15 +2441,17 @@
         ), especially when scraped.
       </p>
       <fragment xml:id="audiovideo">
         <title>Video and audio</title>
         <code>Video =
                 element video {
                     UniqueID?,
+                    LabelID?,
                     PermanentID?,
+                    Component?,
                     attribute width {text}?,
                     attribute margins {text}?,
                     attribute aspect {text}?,
                     attribute start {xsd:integer}?,
                     attribute end {xsd:integer}?,
                     attribute play-at {&quot;embed&quot; | &quot;popout&quot; | &quot;select&quot;}?,
                     attribute preview {&quot;default&quot; | &quot;generic&quot; | text}?,
@@ -2478,20 +2584,20 @@
                     },
                     Hint*, Answer*, Solution*
             Block =
                 element block {
                     attribute order {xsd:integer}?,
                     ((
                         attribute correct {&quot;yes&quot;|&quot;no&quot;}?,
-                        mixed {BlockText?}
+                        mixed {BlockText?, CodeLine?}+
                     ) |
                     (
                         element choice {
                             attribute correct {&quot;yes&quot;|&quot;no&quot;}?,
-                            mixed {BlockText?}
+                            mixed {BlockText?, CodeLine?}+
                         }+
                     ))
                 }
             Matching =
                 MetaDataTitleOptional,
                 attribute number {text}?,
                 StatementExercise,
@@ -2516,35 +2622,93 @@
                 (
                 (ExerciseBody, Response?) |
                 (StatementExercise, Response?, Hint*, Answer*, Solution*) |
                 (IntroductionStatement?, Task+, ConclusionStatement?)
                 )
             Response =
                 element response {empty}
+
+
+            # Selectable areas
+            Area =
+                element area {
+                    attribute correct {&quot;yes&quot;|&quot;no&quot;}?,
+                    TextLong
+                }
+            TextLongAreas =  mixed { (
+                  Area |
+                  Character |
+                  Generator |
+                  Verbatim |
+                  GroupAreas |
+                  MathInline |
+                  Music |
+                  Reference |
+                  WWVariable)* }
+            GroupAreas |=
+                element q {TextLongAreas} |
+                element sq {TextLongAreas}
+            TextParagraphAreas = mixed { (
+              Character |
+              Generator |
+              Verbatim |
+              Group |
+              WWVariable |
+              MathInline |
+              Music |
+              Reference |
+              CodeDisplay |
+              MathDisplay |
+              List |
+              Footnote |
+              Notation |
+              Index |
+              Area |
+              GroupAreas)* }
+            ParagraphAreas =
+                element p {
+                    UniqueID?,
+                    LabelID?,
+                    PermanentID?,
+                    Component?,
+                    TextParagraphAreas
+                }
+            Areas =
+                MetaDataTitleOptional,
+                attribute number {text}?,
+                StatementExercise,
+                Feedback?,
+                element areas {
+                  ParagraphAreas+
+                },
+                Hint*, Answer*, Solution*
+
             # General feedback element
             Feedback =
                 element feedback {
                     MetaDataTitleOptional,
                     BlockSolution+
                 }
             # Include all exercise types in exercise and activity
             Exercise |=
                 element exercise {
                     TrueFalse |
                     MultipleChoice |
                     Parsons |
                     Matching |
-                    FreeResponse
+                    FreeResponse |
+                    Areas
                 }
             ProjectLike |=
                 TrueFalse |
                 MultipleChoice |
                 Parsons |
                 Matching |
-                FreeResponse</code>
+                FreeResponse |
+                Areas</code>
       </fragment>
     </section>
     <section>
       <title>Bibliography</title>
       <p>This is all stop-gap and will change radically.  But it seems to work for now.  So these rules should not be taken as definitive, at all.</p>
       <fragment xml:id="bibliography">
         <title>Bibliography</title>
@@ -2666,14 +2830,16 @@
                 element webwork {
                     attribute source {text}?,
                     attribute seed {xsd:integer}?
                 }
             WebWorkAuthored =
                 element webwork {
                     UniqueID?,
+                    LabelID?,
+                    Component?,
                     attribute seed {xsd:integer}?,
                     attribute copy {text}?,
                     element description {
                         (
                             TextSimple |
                             SimpleLine+
                         )
@@ -2811,14 +2977,19 @@
             The
             <c>xinclude</c>
             mechanism inserts a
             <c>@xml:base</c>
             attribute on the root element of an included file.  So we allow this attribute on any element that allows a title.
           </li>
           <li>
+            The
+            <c>component</c>
+            attribute allows versions to be controlled by a publisher file.
+          </li>
+          <li>
             These are not unordered specifications since they contain several attributes, and we enforce a
             <c>title</c>
             ,
             <c>subtitle</c>
             ,
             <tag>shorttitle</tag>
             ,
@@ -2899,16 +3070,20 @@
           </li>
         </ul>
       </p>
       <fragment xml:id="metadata">
         <title>Metadata</title>
         <code>UniqueID =
                 attribute xml:id {text}
+            LabelID =
+                attribute label {text}
             PermanentID =
                 attribute permid {text}
+            Component =
+                attribute component {text}
             Title =
                 element title {TextLong}
             LinedTitle =
                 element title {LongLine+}
             Subtitle =
                 element subtitle {TextLong}
             LinedSubtitle =
@@ -2919,104 +3094,114 @@
                 element plaintitle {text}
             Creator =
                 element creator {TextShort}
             XMLBase = attribute xml:base {text}
             XMLLang = attribute xml:lang {text}
             MetaDataTarget =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 Index*
             MetaDataTitle =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title,
                 Index*
             MetaDataAltTitle =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title,
                 ShortTitle?,
                 PlainTitle?,
                 Index*
             MetaDataLinedTitle =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 (Title | LinedTitle),
                 ShortTitle?,
                 PlainTitle?,
                 Index*
             MetaDataSubtitle =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title,
                 Subtitle?,
                 ShortTitle?,
                 PlainTitle?,
                 Index*
             MetaDataLinedSubtitle =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 (Title | LinedTitle),
                 (Subtitle | LinedSubtitle)?,
                 ShortTitle?,
                 PlainTitle?,
                 Index*
             MetaDataTitleOptional =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title?,
                 Index*
             MetaDataAltTitleOptional =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 (Title, ShortTitle?, PlainTitle?)?,
                 Index*
             MetaDataTitleCreatorOptional =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title?,
                 Creator?,
                 Index*
             MetaDataCaption =
                 UniqueID?,
+                LabelID?,
                 PermanentID?,
+                Component?,
                 XMLBase?,
                 XMLLang?,
                 Title?,
                 Caption,
                 Index*</code>
       </fragment>
     </section>
     <section>
-      <title>Labels as Unique IDs (experimental)</title>
-      <p>We assume that everywhere an xml:id can go, we can also now put a label.</p>
-      <fragment xml:id="label">
-        <title>Labels as Unique IDs</title>
-        <code>UniqueID |=
-                attribute xml:id {text}?,
-                attribute label {text}?</code>
-      </fragment>
-    </section>
-    <section>
       <title>Miscellaneous</title>
       <p>Provisional items, with uncertain futures.</p>
       <fragment xml:id="miscellaneous">
         <title>Miscellaneous or uncertain</title>
         <code/>
       </fragment>
     </section>
@@ -3534,27 +3719,27 @@
     <section>
       <title>Development
                 Schema</title>
       <p>Here we collect all fragments that are still experimental and put them
                 in a rnc file that includes the stable schema.</p>
       <fragment filename="pretext-dev.rnc">
         <title>Development Schema</title>
-        <code>grammar {
+        <code>namespace xhtml = &quot;http://www.w3.org/1999/xhtml&quot;
+                grammar {
 
                 include &quot;pretext.rnc&quot;</code>
         <fragref ref="interactive"/>
         <fragref ref="frontmatter-dev"/>
         <fragref ref="docinfo-dev"/>
         <fragref ref="proof-like"/>
         <fragref ref="figure-dev"/>
         <fragref ref="worksheet"/>
         <fragref ref="solutions-dev"/>
         <fragref ref="reference-dev"/>
         <fragref ref="mathematics-dev"/>
-        <fragref ref="label"/>
         <fragref ref="exercise-dev"/>
         <code>}</code>
       </fragment>
     </section>
     <backmatter>
       <appendix xml:id="fragment-list">
         <title>Fragments</title>
```

### Comparing `pretext-2.3.9.dev20240302/pretext/project/__init__.py` & `pretext-2.4.0/pretext/project/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,15 +518,15 @@
         if generate:
             self.generate_assets(xmlid=xmlid)
 
         # Ensure the output directories exist.
         self.ensure_output_directory()
 
         # Proceed with the build
-        with tempfile.TemporaryDirectory() as tmp_xsl_str:
+        with tempfile.TemporaryDirectory(prefix="pretext_") as tmp_xsl_str:
             tmp_xsl_path = Path(tmp_xsl_str)
             # if custom xsl, copy it into a temporary directory (different from the building temporary directory)
             if (txp := self.xsl_abspath()) is not None:
                 log.info(f"Building with custom xsl {txp}")
                 utils.copy_custom_xsl(txp, tmp_xsl_path)
                 custom_xsl = tmp_xsl_path / txp.name
             else:
@@ -1375,21 +1375,23 @@
         a PreTeXt project. Existing files will be overwritten
         as long as they have a comment confirmed they are managed
         by this library and not the user. If `skip_unmanaged` is
         `False`, unmanaged files will be backed up to a `.bak` file
         and then overwritten.
         """
         if resources is None or len(resources) == 0:
-            resources = constants.PROJECT_RESOURCES
+            resources = [resource for resource in constants.PROJECT_RESOURCES]
         if not set(resources) <= set(constants.PROJECT_RESOURCES):
             raise TypeError(
                 f"{resources} includes a resource not in {constants.PROJECT_RESOURCES}"
             )
         for resource in resources:
-            project_resource_path = (self.abspath() / resource).resolve()
+            project_resource_path = (
+                self.abspath() / constants.PROJECT_RESOURCES[resource]
+            ).resolve()
             if project_resource_path.exists():
                 # check if file is unmanaged by PreTeXt
                 if (
                     "<!-- Managed automatically by PreTeXt authoring tools -->"
                     not in project_resource_path.read_text()
                 ):
                     if skip_unmanaged:
@@ -1410,14 +1412,15 @@
             if resource != "requirements.txt":
                 with templates.resource_path(resource) as resource_path:
                     if (
                         not project_resource_path.exists()
                         or resource_path.read_text()
                         != project_resource_path.read_text()
                     ):
+                        project_resource_path.parent.mkdir(parents=True, exist_ok=True)
                         shutil.copyfile(resource_path, project_resource_path)
             elif update_requirements:
                 requirements_txt = f"# <!-- Managed automatically by PreTeXt authoring tools -->\npretext == {VERSION}\n"
                 if (
                     not project_resource_path.exists()
                     or project_resource_path.read_text() != requirements_txt
                 ):
```

### Comparing `pretext-2.3.9.dev20240302/pretext/project/xml.py` & `pretext-2.4.0/pretext/project/xml.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240302/pretext/templates/__init__.py` & `pretext-2.4.0/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240302/pretext/templates/resources/.devcontainer.json` & `pretext-2.4.0/pretext/templates/resources/.devcontainer.json`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,17 @@
   // "image": "oscarlevin/pretext:lite",
 
   // Add gh cli as a feature (to support codechat)
   "features": {
     "ghcr.io/devcontainers/features/github-cli:1": {}
   },
 
+  // Respect the project's designated dependencies
+  "postCreateCommand": "pip install -r requirements.txt",
+
   // Port forwarding
   // ---------------
   // This is needed by the CodeChat Server.
   "forwardPorts": [
     // The port used for a Thrift connection between the VSCode CodeChat
     // extension and the CodeChat Server.
     27376,
```

### Comparing `pretext-2.3.9.dev20240302/pretext/templates/resources/.gitignore` & `pretext-2.4.0/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240302/pretext/templates/resources/article.zip` & `pretext-2.4.0/pretext/templates/resources/article.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 160335 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/
--rw-r--r--  2.0 unx       86 b- defN 24-Mar-02 06:13 README.md
--rw-r--r--  2.0 unx     3028 b- defN 24-Mar-02 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx      432 b- defN 24-Mar-02 06:14 project.ptx
--rw-r--r--  2.0 unx     1939 b- defN 24-Mar-02 06:14 .gitignore
--rw-r--r--  2.0 unx     3149 b- defN 24-Mar-02 06:14 .devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 24-Mar-02 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx   154806 b- defN 24-Mar-02 06:13 assets/frog.jpg
--rw-r--r--  2.0 unx      576 b- defN 24-Mar-02 06:13 source/section-1.ptx
--rw-r--r--  2.0 unx      765 b- defN 24-Mar-02 06:13 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 24-Mar-02 06:13 source/main.ptx
-13 files, 165453 bytes uncompressed, 158943 bytes compressed:  3.9%
+Zip file size: 160389 bytes, number of entries: 13
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 source/
+-rw-r--r--  2.0 unx       86 b- defN 24-May-02 01:58 README.md
+-rw-r--r--  2.0 unx      432 b- defN 24-May-02 01:59 project.ptx
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-02 01:59 codechat_config.yaml
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-02 01:59 .devcontainer.json
+-rw-r--r--  2.0 unx     1939 b- defN 24-May-02 01:59 .gitignore
+-rw-r--r--  2.0 unx      242 b- defN 24-May-02 01:58 publication/publication.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 24-May-02 01:58 assets/frog.jpg
+-rw-r--r--  2.0 unx      765 b- defN 24-May-02 01:58 source/section-2.ptx
+-rw-r--r--  2.0 unx      576 b- defN 24-May-02 01:58 source/section-1.ptx
+-rw-r--r--  2.0 unx      430 b- defN 24-May-02 01:58 source/main.ptx
+13 files, 165563 bytes uncompressed, 158997 bytes compressed:  4.0%
```

#### zipnote {}

```diff
@@ -6,35 +6,35 @@
 
 Filename: source/
 Comment: 
 
 Filename: README.md
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
 Filename: project.ptx
 Comment: 
 
-Filename: .gitignore
+Filename: codechat_config.yaml
 Comment: 
 
 Filename: .devcontainer.json
 Comment: 
 
+Filename: .gitignore
+Comment: 
+
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: assets/frog.jpg
 Comment: 
 
-Filename: source/section-1.ptx
+Filename: source/section-2.ptx
 Comment: 
 
-Filename: source/section-2.ptx
+Filename: source/section-1.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Zip file comment:
```

#### .devcontainer.json

```diff
@@ -22,14 +22,17 @@
   // "image": "oscarlevin/pretext:lite",
 
   // Add gh cli as a feature (to support codechat)
   "features": {
     "ghcr.io/devcontainers/features/github-cli:1": {}
   },
 
+  // Respect the project's designated dependencies
+  "postCreateCommand": "pip install -r requirements.txt",
+
   // Port forwarding
   // ---------------
   // This is needed by the CodeChat Server.
   "forwardPorts": [
     // The port used for a Thrift connection between the VSCode CodeChat
     // extension and the CodeChat Server.
     27376,
```

### Comparing `pretext-2.3.9.dev20240302/pretext/templates/resources/book.zip` & `pretext-2.4.0/pretext/templates/resources/book.zip`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 10351 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/
--rw-r--r--  2.0 unx       82 b- defN 24-Mar-02 06:13 README.md
--rw-r--r--  2.0 unx     3028 b- defN 24-Mar-02 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx      432 b- defN 24-Mar-02 06:14 project.ptx
--rw-r--r--  2.0 unx     1939 b- defN 24-Mar-02 06:14 .gitignore
--rw-r--r--  2.0 unx     3149 b- defN 24-Mar-02 06:14 .devcontainer.json
--rw-r--r--  2.0 unx     6207 b- defN 24-Mar-02 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx     1047 b- defN 24-Mar-02 06:13 source/frontmatter.ptx
--rw-r--r--  2.0 unx     2131 b- defN 24-Mar-02 06:13 source/docinfo.ptx
--rw-r--r--  2.0 unx      873 b- defN 24-Mar-02 06:13 source/backmatter.ptx
--rw-r--r--  2.0 unx      315 b- defN 24-Mar-02 06:13 source/ch-chapter-title.ptx
--rw-r--r--  2.0 unx      190 b- defN 24-Mar-02 06:13 source/sec-section-name.ptx
--rw-r--r--  2.0 unx      597 b- defN 24-Mar-02 06:13 source/main.ptx
-14 files, 19990 bytes uncompressed, 8777 bytes compressed:  56.1%
+Zip file size: 10405 bytes, number of entries: 14
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 source/
+-rw-r--r--  2.0 unx       82 b- defN 24-May-02 01:58 README.md
+-rw-r--r--  2.0 unx      432 b- defN 24-May-02 01:59 project.ptx
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-02 01:59 codechat_config.yaml
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-02 01:59 .devcontainer.json
+-rw-r--r--  2.0 unx     1939 b- defN 24-May-02 01:59 .gitignore
+-rw-r--r--  2.0 unx     6207 b- defN 24-May-02 01:58 publication/publication.ptx
+-rw-r--r--  2.0 unx      315 b- defN 24-May-02 01:58 source/ch-chapter-title.ptx
+-rw-r--r--  2.0 unx      190 b- defN 24-May-02 01:58 source/sec-section-name.ptx
+-rw-r--r--  2.0 unx     1047 b- defN 24-May-02 01:58 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      873 b- defN 24-May-02 01:58 source/backmatter.ptx
+-rw-r--r--  2.0 unx      597 b- defN 24-May-02 01:58 source/main.ptx
+-rw-r--r--  2.0 unx     2131 b- defN 24-May-02 01:58 source/docinfo.ptx
+14 files, 20100 bytes uncompressed, 8831 bytes compressed:  56.1%
```

#### zipnote {}

```diff
@@ -3,41 +3,41 @@
 
 Filename: source/
 Comment: 
 
 Filename: README.md
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
 Filename: project.ptx
 Comment: 
 
-Filename: .gitignore
+Filename: codechat_config.yaml
 Comment: 
 
 Filename: .devcontainer.json
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: .gitignore
 Comment: 
 
-Filename: source/frontmatter.ptx
+Filename: publication/publication.ptx
 Comment: 
 
-Filename: source/docinfo.ptx
+Filename: source/ch-chapter-title.ptx
 Comment: 
 
-Filename: source/backmatter.ptx
+Filename: source/sec-section-name.ptx
 Comment: 
 
-Filename: source/ch-chapter-title.ptx
+Filename: source/frontmatter.ptx
 Comment: 
 
-Filename: source/sec-section-name.ptx
+Filename: source/backmatter.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
+Filename: source/docinfo.ptx
+Comment: 
+
 Zip file comment:
```

#### .devcontainer.json

```diff
@@ -22,14 +22,17 @@
   // "image": "oscarlevin/pretext:lite",
 
   // Add gh cli as a feature (to support codechat)
   "features": {
     "ghcr.io/devcontainers/features/github-cli:1": {}
   },
 
+  // Respect the project's designated dependencies
+  "postCreateCommand": "pip install -r requirements.txt",
+
   // Port forwarding
   // ---------------
   // This is needed by the CodeChat Server.
   "forwardPorts": [
     // The port used for a Thrift connection between the VSCode CodeChat
     // extension and the CodeChat Server.
     27376,
```

### Comparing `pretext-2.3.9.dev20240302/pretext/templates/resources/codechat_config.yaml` & `pretext-2.4.0/pretext/templates/resources/codechat_config.yaml`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240302/pretext/templates/resources/demo.zip` & `pretext-2.4.0/pretext/templates/resources/demo.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
-Zip file size: 174088 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/
--rw-r--r--  2.0 unx       82 b- defN 24-Mar-02 06:13 README.md
--rw-r--r--  2.0 unx     3028 b- defN 24-Mar-02 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx      432 b- defN 24-Mar-02 06:14 project.ptx
--rw-r--r--  2.0 unx     1939 b- defN 24-Mar-02 06:14 .gitignore
--rw-r--r--  2.0 unx     3149 b- defN 24-Mar-02 06:14 .devcontainer.json
--rw-r--r--  2.0 unx     6092 b- defN 24-Mar-02 06:13 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 24-Mar-02 06:13 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 24-Mar-02 06:13 assets/jsxgraph/infinity.js
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/images/
--rw-r--r--  2.0 unx     2050 b- defN 24-Mar-02 06:13 source/frontmatter.ptx
--rw-r--r--  2.0 unx      229 b- defN 24-Mar-02 06:13 source/ch-empty.ptx
--rw-r--r--  2.0 unx      867 b- defN 24-Mar-02 06:13 source/sec-features.ptx
--rw-r--r--  2.0 unx     1115 b- defN 24-Mar-02 06:13 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx     1697 b- defN 24-Mar-02 06:13 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      339 b- defN 24-Mar-02 06:13 source/ch-features.ptx
--rw-r--r--  2.0 unx      375 b- defN 24-Mar-02 06:13 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx     2427 b- defN 24-Mar-02 06:13 source/docinfo.ptx
--rw-r--r--  2.0 unx      885 b- defN 24-Mar-02 06:13 source/backmatter.ptx
--rw-r--r--  2.0 unx      411 b- defN 24-Mar-02 06:13 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx      777 b- defN 24-Mar-02 06:13 source/ww.ptx
--rw-r--r--  2.0 unx     2531 b- defN 24-Mar-02 06:13 source/ch-generate.ptx
--rw-r--r--  2.0 unx      381 b- defN 24-Mar-02 06:13 source/fig-tikz.ptx
--rw-r--r--  2.0 unx     2428 b- defN 24-Mar-02 06:13 source/main.ptx
--rw-r--r--  2.0 unx      335 b- defN 24-Mar-02 06:13 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     1515 b- defN 24-Mar-02 06:13 source/ex-first.ptx
--rw-r--r--  2.0 unx      847 b- defN 24-Mar-02 06:13 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      835 b- defN 24-Mar-02 06:13 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 24-Mar-02 06:13 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 24-Mar-02 06:13 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx       10 b- defN 24-Mar-02 06:13 source/images/sageplot2d.sage
-34 files, 191769 bytes uncompressed, 170160 bytes compressed:  11.3%
+Zip file size: 174142 bytes, number of entries: 34
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 source/
+-rw-r--r--  2.0 unx       82 b- defN 24-May-02 01:58 README.md
+-rw-r--r--  2.0 unx      432 b- defN 24-May-02 01:59 project.ptx
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-02 01:59 codechat_config.yaml
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-02 01:59 .devcontainer.json
+-rw-r--r--  2.0 unx     1939 b- defN 24-May-02 01:59 .gitignore
+-rw-r--r--  2.0 unx     6092 b- defN 24-May-02 01:58 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 24-May-02 01:58 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-02 01:58 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 source/images/
+-rw-r--r--  2.0 unx     2531 b- defN 24-May-02 01:58 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      847 b- defN 24-May-02 01:58 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      375 b- defN 24-May-02 01:58 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      867 b- defN 24-May-02 01:58 source/sec-features.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 24-May-02 01:58 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      229 b- defN 24-May-02 01:58 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      411 b- defN 24-May-02 01:58 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx      335 b- defN 24-May-02 01:58 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      381 b- defN 24-May-02 01:58 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx     2050 b- defN 24-May-02 01:58 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 24-May-02 01:58 source/ex-first.ptx
+-rw-r--r--  2.0 unx      885 b- defN 24-May-02 01:58 source/backmatter.ptx
+-rw-r--r--  2.0 unx      777 b- defN 24-May-02 01:58 source/ww.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 24-May-02 01:58 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx     2428 b- defN 24-May-02 01:58 source/main.ptx
+-rw-r--r--  2.0 unx      339 b- defN 24-May-02 01:58 source/ch-features.ptx
+-rw-r--r--  2.0 unx     2427 b- defN 24-May-02 01:58 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 24-May-02 01:58 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx       93 b- defN 24-May-02 01:58 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      835 b- defN 24-May-02 01:58 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 24-May-02 01:58 source/images/tikz.tex
+34 files, 191879 bytes uncompressed, 170214 bytes compressed:  11.3%
```

#### zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: source/
 Comment: 
 
 Filename: README.md
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
 Filename: project.ptx
 Comment: 
 
-Filename: .gitignore
+Filename: codechat_config.yaml
 Comment: 
 
 Filename: .devcontainer.json
 Comment: 
 
+Filename: .gitignore
+Comment: 
+
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: assets/jsxgraph/
 Comment: 
 
 Filename: assets/frog.jpg
@@ -33,71 +33,71 @@
 
 Filename: assets/jsxgraph/infinity.js
 Comment: 
 
 Filename: source/images/
 Comment: 
 
-Filename: source/frontmatter.ptx
+Filename: source/ch-generate.ptx
 Comment: 
 
-Filename: source/ch-empty.ptx
+Filename: source/sec-first-intro.ptx
 Comment: 
 
-Filename: source/sec-features.ptx
+Filename: source/fig-sage2d.ptx
 Comment: 
 
-Filename: source/ch-first with spaces.ptx
+Filename: source/sec-features.ptx
 Comment: 
 
 Filename: source/sec-first-examples.ptx
 Comment: 
 
-Filename: source/ch-features.ptx
+Filename: source/ch-empty.ptx
 Comment: 
 
-Filename: source/fig-sage2d.ptx
+Filename: source/fig-sage3d.ptx
 Comment: 
 
-Filename: source/docinfo.ptx
+Filename: source/fig-asymptote.ptx
 Comment: 
 
-Filename: source/backmatter.ptx
+Filename: source/fig-tikz.ptx
 Comment: 
 
-Filename: source/fig-sage3d.ptx
+Filename: source/frontmatter.ptx
 Comment: 
 
-Filename: source/ww.ptx
+Filename: source/ex-first.ptx
 Comment: 
 
-Filename: source/ch-generate.ptx
+Filename: source/backmatter.ptx
 Comment: 
 
-Filename: source/fig-tikz.ptx
+Filename: source/ww.ptx
 Comment: 
 
-Filename: source/main.ptx
+Filename: source/ch-first with spaces.ptx
 Comment: 
 
-Filename: source/fig-asymptote.ptx
+Filename: source/main.ptx
 Comment: 
 
-Filename: source/ex-first.ptx
+Filename: source/ch-features.ptx
 Comment: 
 
-Filename: source/sec-first-intro.ptx
+Filename: source/docinfo.ptx
 Comment: 
 
-Filename: source/images/cflag.asy
+Filename: source/images/sageplot2d.sage
 Comment: 
 
-Filename: source/images/tikz.tex
+Filename: source/images/sageplot3d.sage
 Comment: 
 
-Filename: source/images/sageplot3d.sage
+Filename: source/images/cflag.asy
 Comment: 
 
-Filename: source/images/sageplot2d.sage
+Filename: source/images/tikz.tex
 Comment: 
 
 Zip file comment:
```

#### .devcontainer.json

```diff
@@ -22,14 +22,17 @@
   // "image": "oscarlevin/pretext:lite",
 
   // Add gh cli as a feature (to support codechat)
   "features": {
     "ghcr.io/devcontainers/features/github-cli:1": {}
   },
 
+  // Respect the project's designated dependencies
+  "postCreateCommand": "pip install -r requirements.txt",
+
   // Port forwarding
   // ---------------
   // This is needed by the CodeChat Server.
   "forwardPorts": [
     // The port used for a Thrift connection between the VSCode CodeChat
     // extension and the CodeChat Server.
     27376,
```

### Comparing `pretext-2.3.9.dev20240302/pretext/templates/resources/hello.zip` & `pretext-2.4.0/pretext/templates/resources/hello.zip`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5045 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/
--rw-r--r--  2.0 unx       69 b- defN 24-Mar-02 06:13 README.md
--rw-r--r--  2.0 unx     3028 b- defN 24-Mar-02 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx      432 b- defN 24-Mar-02 06:14 project.ptx
--rw-r--r--  2.0 unx     1939 b- defN 24-Mar-02 06:14 .gitignore
--rw-r--r--  2.0 unx     3149 b- defN 24-Mar-02 06:14 .devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 24-Mar-02 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 24-Mar-02 06:13 source/main.ptx
-9 files, 9015 bytes uncompressed, 4081 bytes compressed:  54.7%
+Zip file size: 5099 bytes, number of entries: 9
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 source/
+-rw-r--r--  2.0 unx       69 b- defN 24-May-02 01:58 README.md
+-rw-r--r--  2.0 unx      432 b- defN 24-May-02 01:59 project.ptx
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-02 01:59 codechat_config.yaml
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-02 01:59 .devcontainer.json
+-rw-r--r--  2.0 unx     1939 b- defN 24-May-02 01:59 .gitignore
+-rw-r--r--  2.0 unx      242 b- defN 24-May-02 01:58 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 24-May-02 01:58 source/main.ptx
+9 files, 9125 bytes uncompressed, 4135 bytes compressed:  54.7%
```

#### zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: source/
 Comment: 
 
 Filename: README.md
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
 Filename: project.ptx
 Comment: 
 
-Filename: .gitignore
+Filename: codechat_config.yaml
 Comment: 
 
 Filename: .devcontainer.json
 Comment: 
 
+Filename: .gitignore
+Comment: 
+
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Zip file comment:
```

#### .devcontainer.json

```diff
@@ -22,14 +22,17 @@
   // "image": "oscarlevin/pretext:lite",
 
   // Add gh cli as a feature (to support codechat)
   "features": {
     "ghcr.io/devcontainers/features/github-cli:1": {}
   },
 
+  // Respect the project's designated dependencies
+  "postCreateCommand": "pip install -r requirements.txt",
+
   // Port forwarding
   // ---------------
   // This is needed by the CodeChat Server.
   "forwardPorts": [
     // The port used for a Thrift connection between the VSCode CodeChat
     // extension and the CodeChat Server.
     27376,
```

### Comparing `pretext-2.3.9.dev20240302/pretext/templates/resources/slideshow.zip` & `pretext-2.4.0/pretext/templates/resources/slideshow.zip`

 * *Files 17% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8885 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 xsl/
--rw-r--r--  2.0 unx     3028 b- defN 24-Mar-02 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx      480 b- defN 24-Mar-02 06:13 project.ptx
--rw-r--r--  2.0 unx     1939 b- defN 24-Mar-02 06:14 .gitignore
--rw-r--r--  2.0 unx     3149 b- defN 24-Mar-02 06:14 .devcontainer.json
--rw-r--r--  2.0 unx      190 b- defN 24-Mar-02 06:13 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 24-Mar-02 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 24-Mar-02 06:13 source/main.ptx
-10 files, 22083 bytes uncompressed, 7827 bytes compressed:  64.6%
+Zip file size: 8939 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 source/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 01:58 xsl/
+-rw-r--r--  2.0 unx      480 b- defN 24-May-02 01:58 project.ptx
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-02 01:59 codechat_config.yaml
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-02 01:59 .devcontainer.json
+-rw-r--r--  2.0 unx     1939 b- defN 24-May-02 01:59 .gitignore
+-rw-r--r--  2.0 unx     2097 b- defN 24-May-02 01:58 publication/publication.ptx
+-rw-r--r--  2.0 unx      190 b- defN 24-May-02 01:58 xsl/slides.xsl
+-rw-r--r--  2.0 unx    11200 b- defN 24-May-02 01:58 source/main.ptx
+10 files, 22193 bytes uncompressed, 7881 bytes compressed:  64.5%
```

#### zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: source/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
 Filename: project.ptx
 Comment: 
 
-Filename: .gitignore
+Filename: codechat_config.yaml
 Comment: 
 
 Filename: .devcontainer.json
 Comment: 
 
-Filename: xsl/slides.xsl
+Filename: .gitignore
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
+Filename: xsl/slides.xsl
+Comment: 
+
 Filename: source/main.ptx
 Comment: 
 
 Zip file comment:
```

#### .devcontainer.json

```diff
@@ -22,14 +22,17 @@
   // "image": "oscarlevin/pretext:lite",
 
   // Add gh cli as a feature (to support codechat)
   "features": {
     "ghcr.io/devcontainers/features/github-cli:1": {}
   },
 
+  // Respect the project's designated dependencies
+  "postCreateCommand": "pip install -r requirements.txt",
+
   // Port forwarding
   // ---------------
   // This is needed by the CodeChat Server.
   "forwardPorts": [
     // The port used for a Thrift connection between the VSCode CodeChat
     // extension and the CodeChat Server.
     27376,
```

### Comparing `pretext-2.3.9.dev20240302/pretext/utils.py` & `pretext-2.4.0/pretext/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,15 @@
     base_dir: Path,
     access: t.Literal["public", "private"] = "private",
     port: int = 8128,
 ) -> None:
     binding = binding_for_access(access)
 
     # Previously we defined a custom handler to prevent caching, but we don't need to do that anymore.  It was causing issues with the _static js/css files inside codespaces for an unknown reason.  Might bring this back in the future.
+    # 2024-04-05: try using this again to let Firefox work
     class RequestHandler(SimpleHTTPRequestHandler):
         def __init__(self, *args: Any, **kwargs: Any):
             super().__init__(*args, directory=base_dir.as_posix(), **kwargs)
 
         """HTTP request handler with no caching"""
 
         def end_headers(self) -> None:
@@ -246,23 +247,37 @@
 
     class TCPServer(socketserver.TCPServer):
         allow_reuse_address = True
 
     looking_for_port = True
     while looking_for_port:
         try:
-            with TCPServer((binding, port), SimpleHTTPRequestHandler) as httpd:
+            with TCPServer((binding, port), RequestHandler) as httpd:
                 looking_for_port = False
                 httpd.serve_forever()
         except OSError:
             log.warning(f"Port {port} could not be used.")
             port += 1
             log.warning(f"Trying port {port} instead.\n")
 
 
+def start_codespace_server(
+    access: t.Literal["public", "private"] = "private",
+    port: int = 8128,
+) -> None:
+    """
+    Temporary hack until we can figure out what is going on with codespaces an the (possibly more robust) server process we usually define.
+    """
+    subprocess.run(
+        f"python -m http.server {port}",
+        shell=True,
+    )
+    return
+
+
 # Info on namespaces: http://lxml.de/tutorial.html#namespaces
 NSMAP = {
     "xi": "http://www.w3.org/2001/XInclude",
     "xml": "http://www.w3.org/XML/1998/namespace",
 }
```

### Comparing `pretext-2.3.9.dev20240302/pyproject.toml` & `pretext-2.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "2.3.9.dev20240302"
+version = "2.4.0"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
@@ -38,19 +38,21 @@
 click-log = "^0.4"
 ghp-import = "^2"
 single-version = "^1"
 playwright = "^1"
 pydantic-xml = ">=2"
 qrcode = "^7"
 psutil = "^5"
+plastex = "^3"
+jinja2 = "^3"
 
 # Development dependencies
 # ------------------------
 [tool.poetry.group.dev.dependencies]
-black = "^23"
+black = ">=23,<25"
 codechat-server = "^0"
 flake8 = "^6"
 lxml-stubs = "^0"
 mypy = "^1"
 pytest = "^7"
 pytest-console-scripts = "^1"
 pytest-cov = "^4"
@@ -63,14 +65,20 @@
 [tool.poetry.scripts]
 pretext = 'pretext.cli:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+# Fix for `poetry install` not installing the correct docutils version.  
+# see https://github.com/python-poetry/poetry/issues/9293
+[[tool.poetry.source]]
+name = "pypi-public"
+url = "https://pypi.org/simple/"
+
 
 # Pytest configuration
 # ====================
 [tool.pytest.ini_options]
 script_launch_mode = "subprocess"
 
 
@@ -93,14 +101,16 @@
     "click_log",
     "single_version",
     "ghp_import",
     # We're installing ``lxml-stubs``, but it doesn't have stubs for this yet.
     "lxml.ElementInclude",
     "pytest",
     "pytest_console_scripts",
+    "plasTeX.TeX",
+    "plasTeX.Renderers.PageTemplate",
 ]
 ignore_missing_imports = true
 
 # Tell mypy to skip imports of the core. Per [SO](https://stackoverflow.com/a/70367929/16038919),
 # the `exclude` above will be overridden when code mypy scans includes the core.
 # The setting below prevents this.
 [[tool.mypy.overrides]]
```

### Comparing `pretext-2.3.9.dev20240302/PKG-INFO` & `pretext-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 2.3.9.dev20240302
+Version: 2.4.0
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -13,16 +13,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3,<4)
 Requires-Dist: PyPDF2 (>=2.5,<2.6)
 Requires-Dist: click (>=8,<9)
 Requires-Dist: click-log (>=0.4,<0.5)
 Requires-Dist: ghp-import (>=2,<3)
+Requires-Dist: jinja2 (>=3,<4)
 Requires-Dist: lxml (>=4.8,<5.0)
 Requires-Dist: pdfCropMargins (>=1.0.9,<1.1.0)
+Requires-Dist: plastex (>=3,<4)
 Requires-Dist: playwright (>=1,<2)
 Requires-Dist: psutil (>=5,<6)
 Requires-Dist: pyMuPDF (>=1.23,<2.0)
 Requires-Dist: pydantic-xml (>=2)
 Requires-Dist: qrcode (>=7,<8)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: single-version (>=1,<2)
@@ -271,30 +273,33 @@
 need to be rebuilt by each user when pulled from GitHub.
 
 The file `pretext/__init__.py` tracks the upstream
 commit of core PreTeXt XSL/Python code we're developing against
 (from `PreTeXtBook/pretext`).
 To fetch these updates from upstream, run:
 
-```
+```bash
 poetry run python scripts/fetch_core.py
 ```
 
 If you instead want to point to a local copy of `PreTeXtBook/pretext`,
 try this instead to set up symlinks:
 
-```
+```bash
 poetry run python scripts/symlink_core.py path/to/pretext
 ```
 
+For more detailed directions on using a local copy of the core resources to develop core and CLI together, see [docs/core_development.md](docs/core_development.md).
+
+
 Updates to `templates/` must be zipped and moved into
 `pretext/templates/resources`. This is done automatically by
 running:
 
-```
+```bash
 poetry run python scripts/zip_templates.py
 ```
 
 ### Formatting code before a commit
 
 All `.py` files are formatted with the [black](https://black.readthedocs.io/en/stable/)
 python formatter and checked by [flake8](https://flake8.pycqa.org/en/latest/).
```

