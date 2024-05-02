# Comparing `tmp/jira-commands-0.8.0.tar.gz` & `tmp/jira-commands-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira-commands-0.8.0.tar", max compression
+gzip compressed data, was "jira-commands-0.9.0.tar", max compression
```

## Comparing `jira-commands-0.8.0.tar` & `jira-commands-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2022-02-10 19:51:18.831653 jira-commands-0.8.0/LICENSE
--rw-r--r--   0        0        0     5812 2022-08-10 18:10:13.340763 jira-commands-0.8.0/README.md
--rw-r--r--   0        0        0       22 2022-09-27 22:26:04.272864 jira-commands-0.8.0/jira_commands/__init__.py
--rw-r--r--   0        0        0        0 2022-02-10 20:10:16.075773 jira-commands-0.8.0/jira_commands/cli/__init__.py
--rw-r--r--   0        0        0     3559 2022-03-11 23:11:23.235893 jira-commands-0.8.0/jira_commands/cli/common.py
--rwxr-xr-x   0        0        0    10791 2022-03-11 23:11:23.236332 jira-commands-0.8.0/jira_commands/cli/crudops.py
--rw-r--r--   0        0        0     1565 2022-03-11 23:11:23.236678 jira-commands-0.8.0/jira_commands/cli/jc.py
--rwxr-xr-x   0        0        0     1152 2022-03-11 23:11:24.253570 jira-commands-0.8.0/jira_commands/cli/list.py
--rwxr-xr-x   0        0        0     4523 2022-09-27 22:26:04.273558 jira-commands-0.8.0/jira_commands/cli/vivisect.py
--rw-r--r--   0        0        0    20727 2022-09-27 22:26:04.274016 jira-commands-0.8.0/jira_commands/jira.py
--rw-r--r--   0        0        0      297 2022-02-10 19:51:18.833906 jira-commands-0.8.0/jira_commands/utils.py
--rw-r--r--   0        0        0     2509 2022-09-27 22:26:04.275468 jira-commands-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9488 2022-09-27 22:30:08.590170 jira-commands-0.8.0/setup.py
--rw-r--r--   0        0        0     6500 2022-09-27 22:30:08.591031 jira-commands-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-02-10 19:51:18.831653 jira-commands-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6309 2022-10-25 21:16:02.913480 jira-commands-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2022-10-25 21:16:02.919147 jira-commands-0.9.0/jira_commands/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-01 16:30:38.283166 jira-commands-0.9.0/jira_commands/cli/__init__.py
+-rw-r--r--   0        0        0     4447 2022-10-25 21:16:02.921708 jira-commands-0.9.0/jira_commands/cli/common.py
+-rwxr-xr-x   0        0        0    10791 2022-10-01 16:30:38.284751 jira-commands-0.9.0/jira_commands/cli/crudops.py
+-rw-r--r--   0        0        0     1565 2022-03-11 23:11:23.236678 jira-commands-0.9.0/jira_commands/cli/jc.py
+-rwxr-xr-x   0        0        0     1152 2022-10-01 16:30:38.285556 jira-commands-0.9.0/jira_commands/cli/list.py
+-rwxr-xr-x   0        0        0     4523 2022-10-01 16:30:38.286565 jira-commands-0.9.0/jira_commands/cli/vivisect.py
+-rw-r--r--   0        0        0    23535 2022-10-25 21:16:02.927511 jira-commands-0.9.0/jira_commands/jira.py
+-rw-r--r--   0        0        0      297 2022-02-10 19:51:18.833906 jira-commands-0.9.0/jira_commands/utils.py
+-rw-r--r--   0        0        0     2529 2022-10-25 21:16:02.929614 jira-commands-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10005 2022-10-25 21:17:04.822145 jira-commands-0.9.0/setup.py
+-rw-r--r--   0        0        0     7101 2022-10-25 21:17:04.822970 jira-commands-0.9.0/PKG-INFO
```

### Comparing `jira-commands-0.8.0/LICENSE` & `jira-commands-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jira-commands-0.8.0/README.md` & `jira-commands-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 ![Megalinter](https://github.com/unixorn/jira-commands/actions/workflows/mega-linter.yml/badge.svg)
 ![PyPI - Format](https://img.shields.io/pypi/format/jira-commands?style=plastic)
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 ## Table of Contents
 
-- [jira-commands](#jira-commands)
-  - [Scripts](#scripts)
-  - [Configuration](#configuration)
-  - [Installation](#installation)
-    - [Run via docker / nerdctl](#run-via-docker--nerdctl)
-    - [Direct pip install](#direct-pip-install)
-    - [ZSH plugin](#zsh-plugin)
-      - [zgenom](#zgenom)
-      - [Antigen](#antigen)
-      - [oh-my-zsh](#oh-my-zsh)
+- [Scripts](#scripts)
+- [Configuration](#configuration)
+  - [Basic Authentication](#basic-authentication)
+  - [OAuth Authentication](#oauth-authentication)
+- [Installation](#installation)
+  - [Run via docker / nerdctl](#run-via-docker--nerdctl)
+  - [Direct pip install](#direct-pip-install)
+  - [ZSH plugin](#zsh-plugin)
+    - [zgenom](#zgenom)
+    - [Antigen](#antigen)
+    - [oh-my-zsh](#oh-my-zsh)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 Some command-line tools for interacting with JIRA.
 
 ## Scripts
 
@@ -49,23 +50,38 @@
 
 If you're using the docker method, `jc` will automatically run the subcommands inside a container for you. If you've installed via pip, it'll find the commands where they were installed in your `$PATH`.
 
 ## Configuration
 
 The `jc` commands all read settings from `~/.jira-commands/jira.yaml`. Settings in the file can be overridden by specifying command-line options.
 
+### Basic Authentication
+
 I'm setting my username and jira server in the example below. The tools will ask for my password when I run them.
 
 ```yaml
-username: yourusername
 jira_server: https://jira.example.com
+username: yourusername
 ```
 
 You can specify a `password` key but it's a terrible idea.
 
+### OAuth Authentication
+
+Here's an example settings file for oauth authentication. Add `--auth=OAUTH` to use oath instead of basic authentication.
+
+```yaml
+jira_server: https://jira.example.com/
+oauth_access_token: ABCDabcdABCDabcdABCDabcdABCDabcd
+oauth_access_token_secret: ABCDabcdABCDabcdABCDabcdABCDabcd
+oauth_consumer_key: OAUTH_CONSUMER_KEY_ID
+oauth_private_key_pem_pathL: /path/to/pem/file
+username: JIRA_USER
+```
+
 ## Installation
 
 ### Run via docker / nerdctl
 
 This is the recommended way to use the `jc` commands, and how it will be run if you use one of the ZSH frameworks detailed below.
 
 If you're not using a ZSH framework, clone this repository and add its `bin` directory to your `$PATH`. It contains a `jc` script that will detect whether you have `nerdctl` or `docker` and if it finds them, map `~/jira-commands` (and the configuration file there) into a volume in the `jira-commands` container and run the tools inside the container.
```

### Comparing `jira-commands-0.8.0/jira_commands/cli/common.py` & `jira-commands-0.9.0/jira_commands/cli/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,14 +22,47 @@
         "--logging",
         "-l",
         type=str.upper,
         help="set log level",
         choices=["DEBUG", "INFO", "ERROR", "WARNING", "CRITICAL"],
         default="INFO",
     )
+    parser.add_argument(
+        "--auth",
+        "--auth-type",
+        type=str.upper,
+        help="Set authentication method to use.",
+        choices=["BASIC", "OAUTH"],
+        default="BASIC",
+    )
+    parser.add_argument(
+        "--oauth-access-token",
+        "--oauth-access_token",
+        help="Oauth access_token",
+        type=str,
+    )
+    parser.add_argument(
+        "--oauth-access-token-secret",
+        "--oauth-access_token_secret",
+        help="Oauth access_token_secret",
+        type=str,
+    )
+    parser.add_argument(
+        "--oauth-consumer-key",
+        "--oauth-consumer_key",
+        help="Oauth consumer_key",
+        type=str,
+    )
+    parser.add_argument(
+        "--oauth-private-key-pem-path",
+        "--oauth-pem-path",
+        "--oauth-pem_path",
+        help="Path to file containing a PEM format Oauth private key",
+        type=str,
+    )
 
     # We have different default settings file paths based on whether we're
     # running in a container, on a server, or on a laptop.
     settingsFileDefault = "/config/jira.yaml"
     settingsFileCandidates = [settingsFileDefault, "/etc/zscaler/jira/jira.yaml"]
     if "HOME" in os.environ:
         settingsFileCandidates.append(f"{os.environ.get('HOME')}/.zscaler/jira.yaml")
```

### Comparing `jira-commands-0.8.0/jira_commands/cli/crudops.py` & `jira-commands-0.9.0/jira_commands/cli/crudops.py`

 * *Files identical despite different names*

### Comparing `jira-commands-0.8.0/jira_commands/cli/jc.py` & `jira-commands-0.9.0/jira_commands/cli/jc.py`

 * *Files identical despite different names*

### Comparing `jira-commands-0.8.0/jira_commands/cli/list.py` & `jira-commands-0.9.0/jira_commands/cli/list.py`

 * *Files identical despite different names*

### Comparing `jira-commands-0.8.0/jira_commands/cli/vivisect.py` & `jira-commands-0.9.0/jira_commands/cli/vivisect.py`

 * *Files identical despite different names*

### Comparing `jira-commands-0.8.0/jira_commands/jira.py` & `jira-commands-0.9.0/jira_commands/jira.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,47 +18,88 @@
 
 
 def loadJiraSettings(path: str, cli):
     """
     Load JIRA settings from a yaml file, allowing overrides from the CLI
     """
     settings = readYamlFile(path=path)
+
     # Command line arguments should override the settings file
     if cli.server:
         settings["jira_server"] = cli.server
 
     if cli.username:
         settings["username"] = cli.username
 
     if cli.password:
         settings["password"] = cli.password
 
-    if "username" not in settings:
-        settings["username"] = input("Username: ")
+    if cli.oauth_access_token:
+        settings["oauth_access_token"] = cli.oauth_access_token
+    if cli.oauth_access_token_secret:
+        settings["oauth_access_token_secret"] = cli.oauth_access_token_secret
+    if cli.oauth_consumer_key:
+        settings["oauth_consumer_key"] = cli.oauth_consumer_key
+    if cli.oauth_private_key_pem_path:
+        settings["oauth_private_key_pem_path"] = cli.oauth_private_key_pem_path
 
-    if "password" not in settings:
-        settings["password"] = getpass.getpass("Password: ")
+    if cli.auth:
+        settings["auth"] = cli.auth
 
     # Make sure we have all the settings we need
     if "jira_server" not in settings:
         raise RuntimeError("You must specify the jira server")
-    if not settings["username"]:
-        raise RuntimeError("You must specify the jira server username")
-    if not settings["password"]:
-        raise RuntimeError("You must specify the jira server password")
+
+    if cli.auth == "BASIC":
+        # We can fall back to asking the user if we're doing basic auth
+        if "username" not in settings:
+            settings["username"] = input("Username: ")
+
+        if "password" not in settings:
+            settings["password"] = getpass.getpass("Password: ")
+
+    if cli.auth == "BASIC":
+        if not settings["username"]:
+            raise RuntimeError("You must specify the jira server username")
+        if not settings["password"]:
+            raise RuntimeError("You must specify the jira server password")
+
+        credentials = {
+            "username": settings["username"],
+            "password": settings["password"],
+        }
+        if "credentials" not in settings:
+            logging.debug("Setting credentials key in settings")
+            settings["credentials"] = credentials
+        else:
+            logging.warning(f"There is already a credentials key in {path}")
+
+    if cli.auth == "OAUTH":
+        # We need all of these when auth is set to OAUTH
+        logging.info(f"settings: {settings}")
+        if "oauth_access_token" not in settings:
+            raise RuntimeError(
+                "You must specify an Oauth access_token when auth is set to OAUTH"
+            )
+        if "oauth_access_token_secret" not in settings:
+            raise RuntimeError(
+                "You must specify an Oauth access_token_secret when auth is set to OAUTH"
+            )
+        if "oauth_consumer_key" not in settings:
+            raise RuntimeError(
+                "You must specify an Oauth consumer_key when auth is set to OAUTH"
+            )
+        if "oauth_private_key_pem_path" not in settings:
+            raise RuntimeError(
+                "You must specify the path to a pem file containing the Oauth private key when auth is set to OAUTH"
+            )
 
     logging.debug(f"Using JIRA server: {settings['jira_server']}")
     logging.debug(f"username: {settings['username']}")
 
-    credentials = {"username": settings["username"], "password": settings["password"]}
-    if "credentials" not in settings:
-        logging.debug("Setting credentials key in settings")
-        settings["credentials"] = credentials
-    else:
-        logging.warning(f"There is already a credentials key in {path}")
     return settings
 
 
 def makeIssueData(cli):
     """
     Create issue_data from command line arguments
 
@@ -166,33 +207,57 @@
 
 class JiraTool:
     # Jira housekeeping
     def __init__(self, settings: dict):
         """
         Create a JIRA helper object
         """
-        self.username = settings["username"]
-        self.password = settings["password"]
+        if "username" in settings:
+            self.username = settings["username"]
+        if "password" in settings:
+            self.password = settings["password"]
         self.jira_server = settings["jira_server"]
-        self.connect()
+
+        # Load OAUTH credentials
+        if "oauth_access_token" in settings:
+            self.oauth_access_token = settings["oauth_access_token"]
+        if "oauth_access_token_secret" in settings:
+            self.oauth_access_token_secret = settings["oauth_access_token_secret"]
+        if "oauth_consumer_key" in settings:
+            self.oauth_consumer_key = settings["oauth_consumer_key"]
+        if "oauth_private_key_pem_path" in settings:
+            self.oauth_private_key_pem_path = settings["oauth_private_key_pem_path"]
+        self.connect(auth=settings["auth"])
 
     def __str__(self):
         """
         Print a representation of the object
         """
         raw = {"username": self.username, "jira_server": self.jira_server}
         return raw.__str__()
 
-    def connect(self):
+    def connect(self, auth: str = "BASIC"):
         jiraOptions = {"server": self.jira_server}
-        jiraBasicAuth = (self.username, self.password)
-        logging.debug(
-            f"Creating connection to {self.jira_server} with user {self.username}"
-        )
-        self.connection = JIRA(options=jiraOptions, basic_auth=jiraBasicAuth)
+        if auth == "BASIC":
+            jiraBasicAuth = (self.username, self.password)
+            logging.debug(
+                f"Creating connection to {self.jira_server} with user {self.username}"
+            )
+            self.connection = JIRA(options=jiraOptions, basic_auth=jiraBasicAuth)
+        if auth == "OAUTH":
+            with open(self.oauth_private_key_pem_path, "r") as key_cert_file:
+                key_cert_data = key_cert_file.read()
+
+            oauth_dict = {
+                "access_token": self.oauth_access_token,
+                "access_token_secret": self.oauth_access_token_secret,
+                "consumer_key": self.oauth_consumer_key,
+                "key_cert": key_cert_data,
+            }
+            self.connection = JIRA(options=jiraOptions, oauth=oauth_dict)
 
     # Field manipulations
 
     def allowedValuesForField(self, ticket: str, custom_field: str):
         """
         Get the allowed values for a custom field on an issue
```

### Comparing `jira-commands-0.8.0/pyproject.toml` & `jira-commands-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "jira-commands"
-version = "0.8.0"
+version = "0.9.0"
 description = "Command line utilities for interacting with JIRA"
 authors = ["Joe Block <jpb@unixorn.net>"]
 homepage = "https://github.com/unixorn/jira-commands"
 repository = "https://github.com/unixorn/jira-commands"
 readme = 'README.md'
 
 [tool.poetry.dependencies]
-python = "^3.9"
+# python = "^3.9"
+python = "^3.6.5"
 jira = "^3.1.1"
 PyYAML = "^6.0"
-thelogrus = "^0.6.2"
+thelogrus = "^0.7.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 nose = "^1.3.7"
 black = "^22.1.0"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
```

### Comparing `jira-commands-0.8.0/setup.py` & `jira-commands-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 packages = \
 ['jira_commands', 'jira_commands.cli']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyYAML>=6.0,<7.0', 'jira>=3.1.1,<4.0.0', 'thelogrus>=0.6.2,<0.7.0']
+['PyYAML>=6.0,<7.0', 'jira>=3.1.1,<4.0.0', 'thelogrus>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['jc = jira_commands.cli.jc:jc_driver',
                      'jc-assign-ticket = '
                      'jira_commands.cli.crudops:assignTicket',
                      'jc-close-ticket = jira_commands.cli.crudops:closeTicket',
                      'jc-comment-on-ticket = '
@@ -56,24 +56,24 @@
                      'jc-transition-ticket-to = '
                      'jira_commands.cli.crudops:transitionTo',
                      'jc-vivisect-ticket = '
                      'jira_commands.cli.vivisect:vivisect']}
 
 setup_kwargs = {
     'name': 'jira-commands',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Command line utilities for interacting with JIRA',
-    'long_description': "# jira-commands\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Funixorn%2Fjira-commands%2Fbadge%3Fref%3Dmain&style=plastic)](https://actions-badge.atrox.dev/unixorn/jira-commands/goto?ref=main)\n![Megalinter](https://github.com/unixorn/jira-commands/actions/workflows/mega-linter.yml/badge.svg)\n![PyPI - Format](https://img.shields.io/pypi/format/jira-commands?style=plastic)\n\n<!-- START doctoc generated TOC please keep comment here to allow auto update -->\n<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->\n## Table of Contents\n\n- [jira-commands](#jira-commands)\n  - [Scripts](#scripts)\n  - [Configuration](#configuration)\n  - [Installation](#installation)\n    - [Run via docker / nerdctl](#run-via-docker--nerdctl)\n    - [Direct pip install](#direct-pip-install)\n    - [ZSH plugin](#zsh-plugin)\n      - [zgenom](#zgenom)\n      - [Antigen](#antigen)\n      - [oh-my-zsh](#oh-my-zsh)\n\n<!-- END doctoc generated TOC please keep comment here to allow auto update -->\n\nSome command-line tools for interacting with JIRA.\n\n## Scripts\n\nAll of these scripts support `--help` to get a detailed list of command line options.\n\n| Name                         | Description                                           |\n| -----------------------------| ----------------------------------------------------- |\n| `jc` | Main driver. Will run all the other commands inside a docker container for you. |\n| `jc assign ticket` / `jc ticket assign` | Assign a ticket to someone. |\n| `jc close ticket` / `jc ticket close` | Close a ticket |\n| `jc comment on ticket` / `jc ticket comment` | Comment on a ticket |\n| `jc create ticket` / `jc ticket create` | Create a ticket. You will need|\n| `jc custom field allowed values` | List a custom field's allowed values since JIRA isn't forthcoming about them. |\n| `jc examine ticket` / `jc ticket examine` | Detailed dump of a ticket and all its custom field names |\n| `jc get link types` | Prints the names of all link types defined on your JIRA instance. |\n| `jc get priority ids` | Prints the names of all ticket priorities defined on your JIRA instance. |\n| `jc link tickets` / `jc ticket link` | Link two tickets. Use `jc get link types` to see what link names are defined on your JIRA server. Case matters. |\n| `jc list project tickets` | List open tickets in a given JIRA project |\n| `jc list ticket transitions` / `jc ticket transition list` | See the availale transitions for a given ticket. |\n| `jc transition ticket to` / `jc ticket transition set` | Transition a ticket to another state. Use `jc list ticket transitions` to see which are available  |\n| `jc vivisect ticket` / `jc ticket vivisect` | Detailed dump of a ticket to find out all the custom field names and other innards. |\n\nThe `jc` program is the main driver script and will find the subcommands, so you can do `jc ticket comment --ticket ABC-123 --comment 'foo bar baz'` and it will find the `jc-ticket-comment` script and run it with the `--ticket` and `--comment` arguments.\n\nIf you're using the docker method, `jc` will automatically run the subcommands inside a container for you. If you've installed via pip, it'll find the commands where they were installed in your `$PATH`.\n\n## Configuration\n\nThe `jc` commands all read settings from `~/.jira-commands/jira.yaml`. Settings in the file can be overridden by specifying command-line options.\n\nI'm setting my username and jira server in the example below. The tools will ask for my password when I run them.\n\n```yaml\nusername: yourusername\njira_server: https://jira.example.com\n```\n\nYou can specify a `password` key but it's a terrible idea.\n\n## Installation\n\n### Run via docker / nerdctl\n\nThis is the recommended way to use the `jc` commands, and how it will be run if you use one of the ZSH frameworks detailed below.\n\nIf you're not using a ZSH framework, clone this repository and add its `bin` directory to your `$PATH`. It contains a `jc` script that will detect whether you have `nerdctl` or `docker` and if it finds them, map `~/jira-commands` (and the configuration file there) into a volume in the `jira-commands` container and run the tools inside the container.\n\n### Direct pip install\n\n`sudo pip install jira-commands` will install the command-line tools via `pip`. This may cause compatibility annoyances with other python tools on your system, so there's a `docker`/`nerdctl` option as well.\n\n### ZSH plugin\n\nThe tooling has been packaged as a ZSH plugin to make using it as easy as possible for ZSH users.\n\n#### zgenom\n\nIf you're using [Zgenom](https://github.com/jandamm/zgenom):\n\n1. Add `zgenom load unixorn/jira-commands` to your `.zshrc` with your other plugins\n2. `zgenom reset && zgenom save`\n\n#### Antigen\n\nIf you're using [Antigen](https://github.com/zsh-users/antigen):\n\n1. Add `antigen bundle unixorn/jira-commands` to your .zshrc where you've listed your other plugins.\n2. Close and reopen your Terminal/iTerm window to refresh context and use the plugin. Alternatively, you can run `antigen bundle unixorn/jira-commands` in a running shell to have `antigen` load the new plugin.\n\n#### oh-my-zsh\n\nIf you're using [oh-my-zsh](https://ohmyz.sh):\n\n1. Clone the repository into a new `jira-commands` directory in oh-my-zsh's plugin folder:\n\n    `git clone https://github.com/unixorn/jira-commands.git $ZSH_CUSTOM/plugins/jira-commands`\n\n2. Edit your `~/.zshrc` and add `jira-commands` – same as clone directory – to the list of plugins to enable:\n\n    `plugins=( ... jira-commands )`\n\n3. Then, restart your terminal application to refresh context and use the plugin. Alternatively, you can source your current shell configuration:\n\n    `source ~/.zshrc`\n",
+    'long_description': "# jira-commands\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Funixorn%2Fjira-commands%2Fbadge%3Fref%3Dmain&style=plastic)](https://actions-badge.atrox.dev/unixorn/jira-commands/goto?ref=main)\n![Megalinter](https://github.com/unixorn/jira-commands/actions/workflows/mega-linter.yml/badge.svg)\n![PyPI - Format](https://img.shields.io/pypi/format/jira-commands?style=plastic)\n\n<!-- START doctoc generated TOC please keep comment here to allow auto update -->\n<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->\n## Table of Contents\n\n- [Scripts](#scripts)\n- [Configuration](#configuration)\n  - [Basic Authentication](#basic-authentication)\n  - [OAuth Authentication](#oauth-authentication)\n- [Installation](#installation)\n  - [Run via docker / nerdctl](#run-via-docker--nerdctl)\n  - [Direct pip install](#direct-pip-install)\n  - [ZSH plugin](#zsh-plugin)\n    - [zgenom](#zgenom)\n    - [Antigen](#antigen)\n    - [oh-my-zsh](#oh-my-zsh)\n\n<!-- END doctoc generated TOC please keep comment here to allow auto update -->\n\nSome command-line tools for interacting with JIRA.\n\n## Scripts\n\nAll of these scripts support `--help` to get a detailed list of command line options.\n\n| Name                         | Description                                           |\n| -----------------------------| ----------------------------------------------------- |\n| `jc` | Main driver. Will run all the other commands inside a docker container for you. |\n| `jc assign ticket` / `jc ticket assign` | Assign a ticket to someone. |\n| `jc close ticket` / `jc ticket close` | Close a ticket |\n| `jc comment on ticket` / `jc ticket comment` | Comment on a ticket |\n| `jc create ticket` / `jc ticket create` | Create a ticket. You will need|\n| `jc custom field allowed values` | List a custom field's allowed values since JIRA isn't forthcoming about them. |\n| `jc examine ticket` / `jc ticket examine` | Detailed dump of a ticket and all its custom field names |\n| `jc get link types` | Prints the names of all link types defined on your JIRA instance. |\n| `jc get priority ids` | Prints the names of all ticket priorities defined on your JIRA instance. |\n| `jc link tickets` / `jc ticket link` | Link two tickets. Use `jc get link types` to see what link names are defined on your JIRA server. Case matters. |\n| `jc list project tickets` | List open tickets in a given JIRA project |\n| `jc list ticket transitions` / `jc ticket transition list` | See the availale transitions for a given ticket. |\n| `jc transition ticket to` / `jc ticket transition set` | Transition a ticket to another state. Use `jc list ticket transitions` to see which are available  |\n| `jc vivisect ticket` / `jc ticket vivisect` | Detailed dump of a ticket to find out all the custom field names and other innards. |\n\nThe `jc` program is the main driver script and will find the subcommands, so you can do `jc ticket comment --ticket ABC-123 --comment 'foo bar baz'` and it will find the `jc-ticket-comment` script and run it with the `--ticket` and `--comment` arguments.\n\nIf you're using the docker method, `jc` will automatically run the subcommands inside a container for you. If you've installed via pip, it'll find the commands where they were installed in your `$PATH`.\n\n## Configuration\n\nThe `jc` commands all read settings from `~/.jira-commands/jira.yaml`. Settings in the file can be overridden by specifying command-line options.\n\n### Basic Authentication\n\nI'm setting my username and jira server in the example below. The tools will ask for my password when I run them.\n\n```yaml\njira_server: https://jira.example.com\nusername: yourusername\n```\n\nYou can specify a `password` key but it's a terrible idea.\n\n### OAuth Authentication\n\nHere's an example settings file for oauth authentication. Add `--auth=OAUTH` to use oath instead of basic authentication.\n\n```yaml\njira_server: https://jira.example.com/\noauth_access_token: ABCDabcdABCDabcdABCDabcdABCDabcd\noauth_access_token_secret: ABCDabcdABCDabcdABCDabcdABCDabcd\noauth_consumer_key: OAUTH_CONSUMER_KEY_ID\noauth_private_key_pem_pathL: /path/to/pem/file\nusername: JIRA_USER\n```\n\n## Installation\n\n### Run via docker / nerdctl\n\nThis is the recommended way to use the `jc` commands, and how it will be run if you use one of the ZSH frameworks detailed below.\n\nIf you're not using a ZSH framework, clone this repository and add its `bin` directory to your `$PATH`. It contains a `jc` script that will detect whether you have `nerdctl` or `docker` and if it finds them, map `~/jira-commands` (and the configuration file there) into a volume in the `jira-commands` container and run the tools inside the container.\n\n### Direct pip install\n\n`sudo pip install jira-commands` will install the command-line tools via `pip`. This may cause compatibility annoyances with other python tools on your system, so there's a `docker`/`nerdctl` option as well.\n\n### ZSH plugin\n\nThe tooling has been packaged as a ZSH plugin to make using it as easy as possible for ZSH users.\n\n#### zgenom\n\nIf you're using [Zgenom](https://github.com/jandamm/zgenom):\n\n1. Add `zgenom load unixorn/jira-commands` to your `.zshrc` with your other plugins\n2. `zgenom reset && zgenom save`\n\n#### Antigen\n\nIf you're using [Antigen](https://github.com/zsh-users/antigen):\n\n1. Add `antigen bundle unixorn/jira-commands` to your .zshrc where you've listed your other plugins.\n2. Close and reopen your Terminal/iTerm window to refresh context and use the plugin. Alternatively, you can run `antigen bundle unixorn/jira-commands` in a running shell to have `antigen` load the new plugin.\n\n#### oh-my-zsh\n\nIf you're using [oh-my-zsh](https://ohmyz.sh):\n\n1. Clone the repository into a new `jira-commands` directory in oh-my-zsh's plugin folder:\n\n    `git clone https://github.com/unixorn/jira-commands.git $ZSH_CUSTOM/plugins/jira-commands`\n\n2. Edit your `~/.zshrc` and add `jira-commands` – same as clone directory – to the list of plugins to enable:\n\n    `plugins=( ... jira-commands )`\n\n3. Then, restart your terminal application to refresh context and use the plugin. Alternatively, you can source your current shell configuration:\n\n    `source ~/.zshrc`\n",
     'author': 'Joe Block',
     'author_email': 'jpb@unixorn.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/unixorn/jira-commands',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.6.5,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `jira-commands-0.8.0/PKG-INFO` & `jira-commands-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: jira-commands
-Version: 0.8.0
+Version: 0.9.0
 Summary: Command line utilities for interacting with JIRA
 Home-page: https://github.com/unixorn/jira-commands
 Author: Joe Block
 Author-email: jpb@unixorn.net
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.6.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: jira (>=3.1.1,<4.0.0)
-Requires-Dist: thelogrus (>=0.6.2,<0.7.0)
+Requires-Dist: thelogrus (>=0.7.0,<0.8.0)
 Project-URL: Bug Tracker, https://github.com/unixorn/jira-commands/issues
 Project-URL: Repository, https://github.com/unixorn/jira-commands
 Description-Content-Type: text/markdown
 
 # jira-commands
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -23,24 +25,25 @@
 ![Megalinter](https://github.com/unixorn/jira-commands/actions/workflows/mega-linter.yml/badge.svg)
 ![PyPI - Format](https://img.shields.io/pypi/format/jira-commands?style=plastic)
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 ## Table of Contents
 
-- [jira-commands](#jira-commands)
-  - [Scripts](#scripts)
-  - [Configuration](#configuration)
-  - [Installation](#installation)
-    - [Run via docker / nerdctl](#run-via-docker--nerdctl)
-    - [Direct pip install](#direct-pip-install)
-    - [ZSH plugin](#zsh-plugin)
-      - [zgenom](#zgenom)
-      - [Antigen](#antigen)
-      - [oh-my-zsh](#oh-my-zsh)
+- [Scripts](#scripts)
+- [Configuration](#configuration)
+  - [Basic Authentication](#basic-authentication)
+  - [OAuth Authentication](#oauth-authentication)
+- [Installation](#installation)
+  - [Run via docker / nerdctl](#run-via-docker--nerdctl)
+  - [Direct pip install](#direct-pip-install)
+  - [ZSH plugin](#zsh-plugin)
+    - [zgenom](#zgenom)
+    - [Antigen](#antigen)
+    - [oh-my-zsh](#oh-my-zsh)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 Some command-line tools for interacting with JIRA.
 
 ## Scripts
 
@@ -67,23 +70,38 @@
 
 If you're using the docker method, `jc` will automatically run the subcommands inside a container for you. If you've installed via pip, it'll find the commands where they were installed in your `$PATH`.
 
 ## Configuration
 
 The `jc` commands all read settings from `~/.jira-commands/jira.yaml`. Settings in the file can be overridden by specifying command-line options.
 
+### Basic Authentication
+
 I'm setting my username and jira server in the example below. The tools will ask for my password when I run them.
 
 ```yaml
-username: yourusername
 jira_server: https://jira.example.com
+username: yourusername
 ```
 
 You can specify a `password` key but it's a terrible idea.
 
+### OAuth Authentication
+
+Here's an example settings file for oauth authentication. Add `--auth=OAUTH` to use oath instead of basic authentication.
+
+```yaml
+jira_server: https://jira.example.com/
+oauth_access_token: ABCDabcdABCDabcdABCDabcdABCDabcd
+oauth_access_token_secret: ABCDabcdABCDabcdABCDabcdABCDabcd
+oauth_consumer_key: OAUTH_CONSUMER_KEY_ID
+oauth_private_key_pem_pathL: /path/to/pem/file
+username: JIRA_USER
+```
+
 ## Installation
 
 ### Run via docker / nerdctl
 
 This is the recommended way to use the `jc` commands, and how it will be run if you use one of the ZSH frameworks detailed below.
 
 If you're not using a ZSH framework, clone this repository and add its `bin` directory to your `$PATH`. It contains a `jc` script that will detect whether you have `nerdctl` or `docker` and if it finds them, map `~/jira-commands` (and the configuration file there) into a volume in the `jira-commands` container and run the tools inside the container.
```

