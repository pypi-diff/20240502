# Comparing `tmp/aws_ssm_juggle-24.4.5.tar.gz` & `tmp/aws_ssm_juggle-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ssm_juggle-24.4.5.tar", max compression
+gzip compressed data, was "aws_ssm_juggle-24.5.0.tar", max compression
```

## Comparing `aws_ssm_juggle-24.4.5.tar` & `aws_ssm_juggle-24.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-04-26 13:12:27.770715 aws_ssm_juggle-24.4.5/LICENSE
--rw-r--r--   0        0        0     2003 2024-04-26 13:24:15.999968 aws_ssm_juggle-24.4.5/README.md
--rw-r--r--   0        0        0     2100 2024-04-30 07:21:14.831680 aws_ssm_juggle-24.4.5/aws_ssm_juggle/__init__.py
--rw-r--r--   0        0        0     6821 2024-04-30 07:21:14.831784 aws_ssm_juggle-24.4.5/aws_ssm_juggle/ec2.py
--rw-r--r--   0        0        0    10655 2024-04-30 07:20:49.297057 aws_ssm_juggle-24.4.5/aws_ssm_juggle/ecs.py
--rw-r--r--   0        0        0      729 2024-04-30 07:10:58.717631 aws_ssm_juggle-24.4.5/pyproject.toml
--rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.4.5/setup.py
--rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-26 13:12:27.770715 aws_ssm_juggle-24.5.0/LICENSE
+-rw-r--r--   0        0        0     2003 2024-04-26 13:24:15.999968 aws_ssm_juggle-24.5.0/README.md
+-rw-r--r--   0        0        0     2117 2024-05-02 09:08:44.744453 aws_ssm_juggle-24.5.0/aws_ssm_juggle/__init__.py
+-rw-r--r--   0        0        0     6910 2024-05-02 08:56:53.335273 aws_ssm_juggle-24.5.0/aws_ssm_juggle/ec2.py
+-rw-r--r--   0        0        0    10744 2024-05-02 08:56:49.672674 aws_ssm_juggle-24.5.0/aws_ssm_juggle/ecs.py
+-rw-r--r--   0        0        0      728 2024-05-02 09:08:12.480337 aws_ssm_juggle-24.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.0/setup.py
+-rw-r--r--   0        0        0     3074 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.0/PKG-INFO
```

### Comparing `aws_ssm_juggle-24.4.5/LICENSE` & `aws_ssm_juggle-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.4.5/README.md` & `aws_ssm_juggle-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.4.5/aws_ssm_juggle/__init__.py` & `aws_ssm_juggle-24.5.0/aws_ssm_juggle/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def show_menu(
     items: list,
     title: str,
     source: list = None,
     back: bool = True,
     clear_screen: bool = False,
-):
+) -> tuple:
     """
     menu function
     """
     index = None
     source = source or items
     if back:
         items = items + ["Back"]
@@ -30,15 +30,15 @@
     if index is None:
         exit(0)
     if items[index] == "Back":
         return None, index
     return source[index], index
 
 
-def port_forward(boto3_session: session.Session, remote_port: int, local_port: int, target: str):
+def port_forward(boto3_session: session.Session, remote_port: int, local_port: int, target: str) -> None:
     """
     forward port
     """
     parameters = {
         "portNumber": [str(remote_port)],
         "localPortNumber": [str(local_port)],
     }
```

### Comparing `aws_ssm_juggle-24.4.5/aws_ssm_juggle/ec2.py` & `aws_ssm_juggle-24.5.0/aws_ssm_juggle/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,17 +108,22 @@
     parser = configargparse.ArgParser(
         prog="ec2-juggle",
         auto_env_var_prefix="EC2_JUGGLE_",
     )
     shtab.add_argument_to(
         parser,
         ["--print-completion"],
-        help="Print shell-completion. Run '. <(ecs-session --print-completion)' to load.",
+        help="Print shell-completion. Run '. <(ecs-juggle --print-completion bash)' to load.",
+    )
+    parser.add_argument(
+        "--profile",
+        help="AWS Profile",
+        default="default",
+        choices=session.Session().available_profiles,
     )
-    parser.add_argument("--profile", help="AWS Profile", default="default")
     parser.add_argument(
         "--region",
         help="AWS region name",
         default="eu-central-1",
     )
     parser.add_argument(
         "--instance-id",
```

### Comparing `aws_ssm_juggle-24.4.5/aws_ssm_juggle/ecs.py` & `aws_ssm_juggle-24.5.0/aws_ssm_juggle/ecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,17 +97,22 @@
     parser = configargparse.ArgParser(
         prog="ecs-juggle",
         auto_env_var_prefix="ECS_JUGGLE_",
     )
     shtab.add_argument_to(
         parser,
         ["--print-completion"],
-        help="Print shell-completion. Run '. <(ecs-session --print-completion)' to load.",
+        help="Print shell-completion. Run '. <(ec2-juggle --print-completion bash)' to load.",
+    )
+    parser.add_argument(
+        "--profile",
+        help="AWS Profile",
+        default="default",
+        choices=session.Session().available_profiles,
     )
-    parser.add_argument("--profile", help="AWS Profile", default="default")
     parser.add_argument(
         "--region",
         help="AWS region name",
         default="eu-central-1",
     )
     parser.add_argument(
         "--cluster",
```

### Comparing `aws_ssm_juggle-24.4.5/pyproject.toml` & `aws_ssm_juggle-24.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "aws-ssm-juggle"
-version = "24.4.5"
-description = "AWS SSM tool for ECS/EC2 (Shell, Port Forwardingm, ...)"
+version = "24.5.0"
+description = "AWS SSM tool for ECS/EC2 (Shell, Port Forwarding, ...)"
 authors = ["Stefan Heitmüller <stefan.heitmueller@gmx.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/morph027/aws-ssm-juggle"
 
 [tool.poetry.dependencies]
 configargparse = "*"
```

### Comparing `aws_ssm_juggle-24.4.5/setup.py` & `aws_ssm_juggle-24.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 entry_points = \
 {'console_scripts': ['ec2-juggle = aws_ssm_juggle.ec2:run',
                      'ecs-juggle = aws_ssm_juggle.ecs:run']}
 
 setup_kwargs = {
     'name': 'aws-ssm-juggle',
-    'version': '24.4.5',
-    'description': 'AWS SSM tool for ECS/EC2 (Shell, Port Forwardingm, ...)',
+    'version': '24.5.0',
+    'description': 'AWS SSM tool for ECS/EC2 (Shell, Port Forwarding, ...)',
     'long_description': '# aws-ssm-juggle\n\n## Installation\n\n```\npip install aws-ssm-juggle\n```\n\n## Pre-requisites\n\n### [session-manager-plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html)\n\n#### Linux\n\n```bash\ncurl https://s3.amazonaws.com/session-manager-downloads/plugin/latest/ubuntu_64bit/session-manager-plugin.deb -o "/tmp/session-manager-plugin.deb"\nmkdir -p ~/bin\ndpkg-deb --fsys-tarfile /tmp/session-manager-plugin.deb | tar --strip-components=4 -C ~/bin/ -xvf - usr/local/sessionmanagerplugin/bin/session-manager-plugin\n```\n\n#### MacOS\n\n`brew install --cask session-manager-plugin`\n\n### Infrastructure\n\nUse [ecs-exec-checker](https://github.com/aws-containers/amazon-ecs-exec-checker) to check for the pre-requisites to use ECS exec.\n\n## ecs-juggle\n\nInspired by [ecsgo](https://github.com/tedsmitt/ecsgo).\n\nProvides a tool to interact with AWS ECS tasks.\n\nCurrently provides:\n\n* interactive execute-command (e.g. shell)\n* port-forwarding\n\nYou can supply command-line arguments to specify which cluster/service/task/... to use or will be prompted with a nice menu.\n\n\n### Usage\n\nSee `ecs-juggle --help` for all features.\n\n#### Execute command\n\nSelect all from menu:\n\n```bash\necs-juggle command\n```\n\n#### Port forwarding\n\nSelect all from menu:\n\n```bash\necs-juggle forward\n```\n\nSpecify port and select the rest from menu:\n\n```bash\necs-juggle forward --remote-port 8080\n```\n\n## ec2-juggle\n\nInspired by [gossm](https://github.com/gjbae1212/gossm/).\n\nProvides a tool to interact with AWS EC2 instances.\n\nCurrently provides:\n\n* interactive shell (e.g. shell)\n* ssh shell\n* port-forwarding\n\n### Usage\n\nSee `ec2-juggle --help` for all features.\n\n#### Start session\n\n```bash\nec2-juggle start\n```\n\n#### Start ssh session\n\nDefault:\n\n```bash\nec2-juggle ssh\n```\n\nWith extra arguments:\n\n```bash\nec2-juggle ssh --ssh-args="-o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null -l ubuntu"\n```\n\n#### Port forwarding\n\n```bash\necs-juggle forward --remote-port 80\n```\n',
     'author': 'Stefan Heitmüller',
     'author_email': 'stefan.heitmueller@gmx.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/morph027/aws-ssm-juggle',
     'packages': packages,
```

### Comparing `aws_ssm_juggle-24.4.5/PKG-INFO` & `aws_ssm_juggle-24.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aws-ssm-juggle
-Version: 24.4.5
-Summary: AWS SSM tool for ECS/EC2 (Shell, Port Forwardingm, ...)
+Version: 24.5.0
+Summary: AWS SSM tool for ECS/EC2 (Shell, Port Forwarding, ...)
 Home-page: https://github.com/morph027/aws-ssm-juggle
 License: MIT
 Author: Stefan Heitmüller
 Author-email: stefan.heitmueller@gmx.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

