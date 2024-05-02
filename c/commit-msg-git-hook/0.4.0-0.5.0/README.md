# Comparing `tmp/commit_msg_git_hook-0.4.0.tar.gz` & `tmp/commit_msg_git_hook-0.5.0.tar.gz`

## Comparing `commit_msg_git_hook-0.4.0.tar` & `commit_msg_git_hook-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/src/commit_msg_git_hook/__init__.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/src/commit_msg_git_hook/commit_msg.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/src/commit_msg_git_hook/scan_git.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/src/commit_msg_git_hook/setup.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/src/commit_msg_git_hook/templates/commit-msg.config.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/src/commit_msg_git_hook/templates/darwin/commit-msg
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/src/commit_msg_git_hook/templates/linux/commit-msg
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/src/commit_msg_git_hook/templates/win32/commit-msg
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/LICENSE
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/README.md
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/__builtins__.pyi
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/commit_msg.pot
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/setup.pot
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/commit_msg.mo
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/commit_msg.po
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/setup.mo
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/setup.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/__init__.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/commit_msg.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/scan_git.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/setup.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/templates/commit-msg.config.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/templates/darwin/commit-msg
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/templates/linux/commit-msg
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/templates/win32/commit-msg
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/PKG-INFO
```

### Comparing `commit_msg_git_hook-0.4.0/src/commit_msg_git_hook/commit_msg.py` & `commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/commit_msg.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,22 @@
+import gettext
+import locale
 import json
 import re
 import sys
 
+
+app_name = "commit_msg_git_hook"
+locale_dir = "./locales"
+
+translations = gettext.translation(
+    app_name, locale_dir, fallback=True, languages=[locale.getlocale()[0]]
+)
+translations.install()
+
 # ANSI Escape Codes
 BOLD = "\033[1m"
 UNDERLINE = "\033[4m"
 RESET = "\033[00m"
 FG_RED = "\033[31m"
 FG_BLUE = "\033[34m"
 
@@ -33,15 +44,15 @@
 def create_regex(config: dict[str]) -> str:
     regex = r"(^"
 
     if config["github_revert_commit"] == True:
         regex += r'Revert ".+"$)|(^'
 
     if config["github_merge_commit"] == True:
-        regex += r'Merge .+)|(^'
+        regex += r"Merge .+)|(^"
 
     regex += r"("
     regex += r"|".join(config["types"])
 
     regex += r")(\(("
     regex += r"|".join(config["scopes"])
 
@@ -62,36 +73,48 @@
 
 def check_msg_empty(msg) -> None:
     if msg == "" or msg == "\n":
         exit(0)
 
 
 def check_msg_length(msg, max_length) -> None:
+    lc_msg_title = _("COMMIT MESSAGE TOO LONG")
+    lc_msg_divider = "-" * len(lc_msg_title)
+    lc_msg_body = _("Configured max length (first line)")
+
     if len(msg) > max_length:
         print(
             f"\n{msg}",
-            f"\n{BOLD}{FG_RED}[COMMIT MESSAGE TOO LONG]{RESET}",
-            f"{BOLD}{FG_RED}------------------------{RESET}",
-            f"{BOLD}Configured max length (first line):{RESET} {FG_BLUE}{max_length}{RESET}\n",
+            f"\n{BOLD}{FG_RED}[{lc_msg_title}]{RESET}",
+            f"{BOLD}{FG_RED}{lc_msg_divider}{RESET}",
+            f"{BOLD}{lc_msg_body}:{RESET} {FG_BLUE}{max_length}{RESET}\n",
             sep="\n",
         )
 
         exit(1)
 
 
 def check_msg_pattern(pattern, msg, config) -> None:
+    lc_msg_title = _("INVALID COMMIT MESSAGE")
+    lc_msg_divider = "-" * len(lc_msg_title)
+    lc_msg_use = _("Use the Conventional Commits specification.")
+    lc_msg_types = _("Valid types")
+    lc_msg_scopes = _("Valid scopes")
+    lc_msg_specs = _("See the specification")
+    lc_msg_specs_url = _("https://www.conventionalcommits.org/en/v1.0.0/")
+
     if not re.match(pattern, msg):
         print(
             f"\n{msg}",
-            f"\n{BOLD}{FG_RED}[INVALID COMMIT MESSAGE]{RESET}",
-            f"{BOLD}{FG_RED}------------------------{RESET}",
-            f"{BOLD}Use the Conventional Commits specification.\n{RESET}",
-            f"{BOLD}Valid types:{RESET} {FG_BLUE}{config['types']}{RESET}",
-            f"{BOLD}Valid scopes:{RESET} {FG_BLUE}{config['scopes']}{RESET}",
-            f"\nSee the specification:\n{UNDERLINE}https://www.conventionalcommits.org/en/v1.0.0/{RESET}\n",
+            f"\n{BOLD}{FG_RED}[{lc_msg_title}]{RESET}",
+            f"{BOLD}{FG_RED}{lc_msg_divider}{RESET}",
+            f"{BOLD}{lc_msg_use}\n{RESET}",
+            f"{BOLD}{lc_msg_types}:{RESET} {FG_BLUE}{config['types']}{RESET}",
+            f"{BOLD}{lc_msg_scopes}:{RESET} {FG_BLUE}{config['scopes']}{RESET}",
+            f"\n{lc_msg_specs}:\n{UNDERLINE}{lc_msg_specs_url}{RESET}\n",
             sep="\n",
         )
 
         exit(2)
 
 
 def check_msg(pattern, msg, config):
```

### Comparing `commit_msg_git_hook-0.4.0/src/commit_msg_git_hook/scan_git.py` & `commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/scan_git.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.4.0/LICENSE` & `commit_msg_git_hook-0.5.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Lucio Meira David
+Copyright (c) 2024 Lucio Meira David
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `commit_msg_git_hook-0.4.0/README.md` & `commit_msg_git_hook-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.4.0/pyproject.toml` & `commit_msg_git_hook-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "commit_msg_git_hook"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="Lucio Meira David", email="lucio.meira@om30.com.br" },
 ]
 description = "A set of tools to validate git Conventional Commit messages."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,14 +16,16 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Version Control :: Git",
+    "Natural Language :: English",
+    "Natural Language :: Portuguese (Brazilian)",
     "Development Status :: 4 - Beta",
 ]
 keywords = ["commit-msg", "git", "git-hook", "git hook", "scan", "ci"]
 
 [project.urls]
 "Homepage" = "https://github.com/OM30/commit-msg-git-hook-package"
 "Bug Tracker" = "https://github.com/OM30/commit-msg-git-hook-package/issues"
```

### Comparing `commit_msg_git_hook-0.4.0/PKG-INFO` & `commit_msg_git_hook-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: commit_msg_git_hook
-Version: 0.4.0
+Version: 0.5.0
 Summary: A set of tools to validate git Conventional Commit messages.
 Project-URL: Homepage, https://github.com/OM30/commit-msg-git-hook-package
 Project-URL: Bug Tracker, https://github.com/OM30/commit-msg-git-hook-package/issues
 Author-email: Lucio Meira David <lucio.meira@om30.com.br>
 License-File: LICENSE
 Keywords: ci,commit-msg,git,git hook,git-hook,scan
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Python: >=3.7
```

