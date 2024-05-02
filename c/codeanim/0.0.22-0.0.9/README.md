# Comparing `tmp/codeanim-0.0.22.tar.gz` & `tmp/codeanim-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeanim-0.0.22.tar", max compression
+gzip compressed data, was "codeanim-0.0.9.tar", max compression
```

## Comparing `codeanim-0.0.22.tar` & `codeanim-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1068 2024-05-01 21:19:56.229618 codeanim-0.0.22/LICENSE
--rw-r--r--   0        0        0     2263 2024-05-01 21:19:56.229618 codeanim-0.0.22/README.md
--rw-r--r--   0        0        0      408 2024-05-01 21:19:56.229618 codeanim-0.0.22/pyproject.toml
--rwxr-xr-x   0        0        0     2773 2024-05-01 21:19:56.229618 codeanim-0.0.22/src/codeanim/__init__.py
--rw-r--r--   0        0        0     1719 2024-05-01 21:19:56.229618 codeanim-0.0.22/src/codeanim/chrome.py
--rw-r--r--   0        0        0     4162 2024-05-01 21:19:56.229618 codeanim-0.0.22/src/codeanim/core.py
--rw-r--r--   0        0        0     1152 2024-05-01 21:19:56.229618 codeanim-0.0.22/src/codeanim/delayer.py
--rw-r--r--   0        0        0      751 2024-05-01 21:19:56.229618 codeanim-0.0.22/src/codeanim/interpolators.py
--rw-r--r--   0        0        0     1653 2024-05-01 21:19:56.233618 codeanim-0.0.22/src/codeanim/keyboard.py
--rw-r--r--   0        0        0     1338 2024-05-01 21:19:56.233618 codeanim-0.0.22/src/codeanim/markdown.py
--rw-r--r--   0        0        0     1058 2024-05-01 21:19:56.233618 codeanim-0.0.22/src/codeanim/shell.py
--rw-r--r--   0        0        0     3018 2024-05-01 21:19:56.233618 codeanim-0.0.22/src/codeanim/vscode.py
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 codeanim-0.0.22/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-02-03 20:12:45.447570 codeanim-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3222 2024-03-03 05:35:42.985531 codeanim-0.0.9/README.md
+-rw-r--r--   0        0        0      407 2024-03-03 22:14:09.461599 codeanim-0.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0     1917 2024-03-03 21:47:24.662461 codeanim-0.0.9/src/codeanim/__init__.py
+-rw-r--r--   0        0        0     1745 2024-03-03 21:47:24.662778 codeanim-0.0.9/src/codeanim/chrome.py
+-rw-r--r--   0        0        0     1933 2024-03-03 21:47:24.662996 codeanim-0.0.9/src/codeanim/core.py
+-rw-r--r--   0        0        0     1152 2024-03-03 21:47:24.663275 codeanim-0.0.9/src/codeanim/delayer.py
+-rw-r--r--   0        0        0     1776 2024-03-03 21:48:41.342963 codeanim-0.0.9/src/codeanim/keyboard.py
+-rw-r--r--   0        0        0     1338 2024-03-03 01:51:34.373628 codeanim-0.0.9/src/codeanim/markdown.py
+-rw-r--r--   0        0        0     1058 2024-03-03 21:47:24.663704 codeanim-0.0.9/src/codeanim/shell.py
+-rw-r--r--   0        0        0     3047 2024-03-03 21:47:24.663985 codeanim-0.0.9/src/codeanim/vscode.py
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 codeanim-0.0.9/PKG-INFO
```

### Comparing `codeanim-0.0.22/LICENSE` & `codeanim-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codeanim-0.0.22/src/codeanim/__init__.py` & `codeanim-0.0.9/src/codeanim/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,25 @@
 #!/usr/bin/env python3
 import argparse
 import os
-from functools import partial
-from importlib.metadata import version
 
-from pynput.keyboard import Key  # noqa: F401
-from pynput.mouse import Button  # noqa: F401
-
-from . import chrome, vscode  # noqa: F401
+from . import chrome, core, markdown, vscode  # noqa: F401
 from .core import codeanim
-from .interpolators import Sigmoid, Spring  # noqa: F401
-from .markdown import parse
 
 # Public API
+Key = core.Key
 backspace = codeanim.backspace
-click = codeanim.click
 delay = codeanim.delay
-drag = codeanim.drag
-move = codeanim.move
-paste = codeanim.paste
 pause = codeanim.delay.pause
-scroll = codeanim.scroll
+paste = codeanim.paste
 tap = codeanim.tap
 wait = codeanim.wait
 write = codeanim.write
 
 
-class VersionAction(argparse.Action):
-    def __call__(self, parser, namespace, values, option_string=None):
-        print(version("codeanim"))
-        parser.exit()
-
-
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "markdown",
         help="The markdown file containing the animation commands",
     )
     parser.add_argument(
@@ -68,33 +52,20 @@
         help="The delay at the end of each animation command",
     )
     parser.add_argument(
         "--live",
         action="store_true",
         help="Insert wait after each codeanim block",
     )
-    parser.add_argument(
-        "--abort-key",
-        default=Key.shift_r,
-        type=partial(getattr, Key),
-        help="Abort CodeAnim execution when this key is pressed",
-    )
-    parser.add_argument(
-        "--version",
-        nargs=0,
-        action=VersionAction,
-        help="Print the version information and exit",
-    )
     args = parser.parse_args()
 
     delay.set(end=args.end_delay, tap=args.tap_delay)
-    codeanim.keyboard.set_abort_key(args.abort_key)
 
     with codeanim:
-        expressions = parse(
+        expressions = markdown.parse(
             args.markdown,
             live=args.live,
             labels=args.labels,
             start_label=args.start_label,
         )
         for expression in expressions:
             if args.verbose:
```

### Comparing `codeanim-0.0.22/src/codeanim/chrome.py` & `codeanim-0.0.9/src/codeanim/chrome.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 def resize(ca: CodeAnim, position: tuple[int, int], size: tuple[int, int]):
     ca.shell.resize(APP_NAME, position, size)
 
 
 @CodeAnim.cmd
 def navigate(ca: CodeAnim, url: str):
     ca.tap("l", modifiers=[Key.cmd])
-    ca.write(url)
+    with ca.delay(0):
+        ca.write(url)
     ca.tap(Key.enter)
 
 
 @CodeAnim.cmd
 def back(ca: CodeAnim):
     ca.tap(Key.left, modifiers=[Key.cmd])
```

### Comparing `codeanim-0.0.22/src/codeanim/delayer.py` & `codeanim-0.0.9/src/codeanim/delayer.py`

 * *Files identical despite different names*

### Comparing `codeanim-0.0.22/src/codeanim/markdown.py` & `codeanim-0.0.9/src/codeanim/markdown.py`

 * *Files identical despite different names*

### Comparing `codeanim-0.0.22/src/codeanim/shell.py` & `codeanim-0.0.9/src/codeanim/shell.py`

 * *Files identical despite different names*

### Comparing `codeanim-0.0.22/src/codeanim/vscode.py` & `codeanim-0.0.9/src/codeanim/vscode.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     ca.write(cmd)
     ca.tap(Key.enter)
 
 
 @CodeAnim.cmd
 def newline(ca: CodeAnim, line: int = 0, *, above: bool = False):
     if line > 0:
-        jump(line)
+        with ca.delay(0):
+            jump(line)
         ca.tap(Key.enter, modifiers=[Key.cmd, Key.shift])
     else:
         ca.tap(Key.enter, modifiers=[Key.cmd, Key.shift] if above else [Key.cmd])
 
 
 @CodeAnim.cmd
 def jump(ca: CodeAnim, line: int, col: int = 1):
@@ -69,15 +70,15 @@
 
 @CodeAnim.cmd
 def bottom(ca: CodeAnim, *, select: bool = False):
     ca.tap(Key.down, modifiers=[Key.cmd, Key.shift] if select else [Key.cmd])
 
 
 @CodeAnim.cmd
-def new_file(ca: CodeAnim):
+def newfile(ca: CodeAnim):
     ca.tap("n", modifiers=[Key.cmd])
 
 
 @CodeAnim.cmd
 def save(ca: CodeAnim, file: str | None = None):
     if file is None:
         ca.tap("s", modifiers=[Key.cmd])
```

### Comparing `codeanim-0.0.22/PKG-INFO` & `codeanim-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeanim
-Version: 0.0.22
+Version: 0.0.9
 Summary: A tool that automates presentation of software demos.
 Author: Shad Sharma
 Author-email: shadanan@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pynput (>=1.7.6,<2.0.0)
@@ -13,27 +13,47 @@
 
 # CodeAnim
 
 CodeAnim is a tool to help you animate VS Code. It provides methods that enable you to type, move the cursor, and send commands to VS Code. It works by sending keystrokes using the pynput library.
 
 ## Installation
 
-We recommend install CodeAnim using [pipx](https://pipx.pypa.io/).
+Create a venv and then pip install CodeAnim from the GitHub repo:
 
 ```shell
-pipx install codeanim
+python3 -m venv .venv
+. .venv/bin/activate
+pip install git+https://github.com/shadanan/codeanim
+```
+
+The run command uses a custom keybinding. Please add this to your `keybindings.json` file in VS Code:
+
+```json
+[
+  {
+    "key": "ctrl+shift+alt+cmd+enter",
+    "command": "python.execInTerminal"
+  }
+]
 ```
 
 ## Usage
 
-CodeAnim runs commands from Markdown files where codeanim commands are enclosed in a `python codeanim` fence.
+There are two ways to use CodeAnim:
+
+- As commands in a Markdown file
+- Imported as a library and executed in a Python script
+
+### Usage of CodeAnim CLI
 
-### Example
+Create a Markdown file and enclose codeanim commands in a `python codeanim` fence.
 
-Create a Markdown file called `codeanim-markdown-demo.md` with the following contents:
+#### Example
+
+Add this to `codeanim-markdown-demo.md`:
 
 ````markdown
 # A Markdown Header
 
 Some text to be read.
 
 ```python codeanim
@@ -53,27 +73,59 @@
 
 To execute the CodeAnim commands in the Markdown file:
 
 ```shell
 codeanim codeanim-markdown-demo.md
 ```
 
-### Flags
+#### Flags
 
 - Set `-v` or `--verbose` to enable verbose mode. Commands will be printed out as they are executed.
 - Set `--live` to enable presentation mode. In this mode, a wait() will be injected after every codeanim fence.
 
+### Usage of CodeAnim Library
+
+Import CodeAnim, and call the functions.
+
+#### Example
+
+Add this to `codeanim_script_demo.py`:
+
+```python
+#!/usr/bin/env python3
+from codeanim import *
+
+# Bring VS Code to the front
+vscode.activate()
+
+# Open myfile.py
+vscode.focus("myfile.py")
+
+# Insert print("Hello, World!") into myfile.py
+write('print("Hello, World!")\n')
+
+# Execute the script
+vscode.run()
+```
+
+Execute your Python script:
+
+```sh
+./codeanim_script_demo.py
+```
+
 ## Development
 
-We use Poetry for development.
+Clone the repo, create a venv, and install dependencies:
 
 ```shell
 git clone https://github.com/shadanan/codeanim.git
 cd codeanim
-poetry install
+python3 -m venv .venv
+pip install .
 ```
 
 ### Formatting
 
 This project adopts the Ruff formatter and is enforced by a GitHub action.
 
 ### VS Code
@@ -84,22 +136,28 @@
 - [Ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff)
 
 ## Tests
 
 There aren't any unit tests yet. In the tests folder, there is an end-to-end test that uses CodeAnim to open the `scratch.py` file, types out some code, and executes it. To run the test:
 
 ```sh
-./e2e-test.sh
+PYTHONPATH=src codeanim tests/e2e.md -v
 ```
 
 Then, validate that it worked by observing that the animation runs, types out:
 
 ```python
 print("Hello, World!")
 ```
 
 And executes the script.
 
+### VS Code Tests
+
+```sh
+PYTHONPATH=src tests/vscode.py
+```
+
 ## Limitations
 
 CodeAnim currently only works on MacOS because of a dependency on AppleScript, which is used to switch to the VS Code window. Also, many of the commands send Mac specific keystrokes. With some effort, CodeAnim can be made to work on other platforms.
```

