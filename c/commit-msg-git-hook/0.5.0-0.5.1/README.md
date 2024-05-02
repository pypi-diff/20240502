# Comparing `tmp/commit_msg_git_hook-0.5.0.tar.gz` & `tmp/commit_msg_git_hook-0.5.1.tar.gz`

## Comparing `commit_msg_git_hook-0.5.0.tar` & `commit_msg_git_hook-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/__builtins__.pyi
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/.vscode/settings.json
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/commit_msg.pot
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/setup.pot
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/commit_msg.mo
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/commit_msg.po
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/setup.mo
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/setup.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/__init__.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/commit_msg.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/scan_git.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/setup.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/templates/commit-msg.config.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/templates/darwin/commit-msg
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/templates/linux/commit-msg
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/templates/win32/commit-msg
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/LICENSE
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/__builtins__.pyi
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/commit_msg.pot
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/setup.pot
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/commit_msg.mo
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/commit_msg.po
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/setup.mo
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/setup.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/__init__.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/commit_msg.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/scan_git.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/setup.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/templates/commit-msg.config.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/templates/darwin/commit-msg
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/templates/linux/commit-msg
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/templates/win32/commit-msg
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.5.1/PKG-INFO
```

### Comparing `commit_msg_git_hook-0.5.0/locales/commit_msg.pot` & `commit_msg_git_hook-0.5.1/locales/commit_msg.pot`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.0/locales/setup.pot` & `commit_msg_git_hook-0.5.1/locales/setup.pot`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/commit_msg.mo` & `commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/commit_msg.mo`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/commit_msg.po` & `commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/commit_msg.po`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/setup.mo` & `commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/setup.mo`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.0/locales/pt_BR/LC_MESSAGES/setup.po` & `commit_msg_git_hook-0.5.1/locales/pt_BR/LC_MESSAGES/setup.po`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/commit_msg.py` & `commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/commit_msg.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 def check_msg_empty(msg) -> None:
     if msg == "" or msg == "\n":
         exit(0)
 
 
 def check_msg_length(msg, max_length) -> None:
     lc_msg_title = _("COMMIT MESSAGE TOO LONG")
-    lc_msg_divider = "-" * len(lc_msg_title)
+    lc_msg_divider = "-" * (len(lc_msg_title) + 2)
     lc_msg_body = _("Configured max length (first line)")
 
     if len(msg) > max_length:
         print(
             f"\n{msg}",
             f"\n{BOLD}{FG_RED}[{lc_msg_title}]{RESET}",
             f"{BOLD}{FG_RED}{lc_msg_divider}{RESET}",
@@ -91,15 +91,15 @@
         )
 
         exit(1)
 
 
 def check_msg_pattern(pattern, msg, config) -> None:
     lc_msg_title = _("INVALID COMMIT MESSAGE")
-    lc_msg_divider = "-" * len(lc_msg_title)
+    lc_msg_divider = "-" * (len(lc_msg_title) + 2)
     lc_msg_use = _("Use the Conventional Commits specification.")
     lc_msg_types = _("Valid types")
     lc_msg_scopes = _("Valid scopes")
     lc_msg_specs = _("See the specification")
     lc_msg_specs_url = _("https://www.conventionalcommits.org/en/v1.0.0/")
 
     if not re.match(pattern, msg):
```

### Comparing `commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/scan_git.py` & `commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/scan_git.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.0/src/commit_msg_git_hook/setup.py` & `commit_msg_git_hook-0.5.1/src/commit_msg_git_hook/setup.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.0/LICENSE` & `commit_msg_git_hook-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.0/README.md` & `commit_msg_git_hook-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.5.0/pyproject.toml` & `commit_msg_git_hook-0.5.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "commit_msg_git_hook"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Lucio Meira David", email="lucio.meira@om30.com.br" },
 ]
 description = "A set of tools to validate git Conventional Commit messages."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `commit_msg_git_hook-0.5.0/PKG-INFO` & `commit_msg_git_hook-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: commit_msg_git_hook
-Version: 0.5.0
+Version: 0.5.1
 Summary: A set of tools to validate git Conventional Commit messages.
 Project-URL: Homepage, https://github.com/OM30/commit-msg-git-hook-package
 Project-URL: Bug Tracker, https://github.com/OM30/commit-msg-git-hook-package/issues
 Author-email: Lucio Meira David <lucio.meira@om30.com.br>
 License-File: LICENSE
 Keywords: ci,commit-msg,git,git hook,git-hook,scan
 Classifier: Development Status :: 4 - Beta
```

