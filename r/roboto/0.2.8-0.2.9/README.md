# Comparing `tmp/roboto-0.2.8.tar.gz` & `tmp/roboto-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto-0.2.8.tar", max compression
+gzip compressed data, was "roboto-0.2.9.tar", max compression
```

## Comparing `roboto-0.2.8.tar` & `roboto-0.2.9.tar`

### file list

```diff
@@ -1,363 +1,363 @@
--rw-r--r--   0        0        0      472 2024-01-11 21:12:42.008484 roboto-0.2.8/README.md
--rw-r--r--   0        0        0      993 2024-01-11 21:16:42.588708 roboto-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       62 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/__init__.py
--rw-r--r--   0        0        0     1470 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/association.py
--rw-r--r--   0        0        0      114 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/auth/__init__.py
--rw-r--r--   0        0        0      376 2024-01-11 21:14:15.428552 roboto-0.2.8/src/roboto/auth/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3810 2024-01-11 21:14:15.432552 roboto-0.2.8/src/roboto/auth/__pycache__/pat.cpython-310.pyc
--rw-r--r--   0        0        0     1002 2024-01-11 21:14:15.428552 roboto-0.2.8/src/roboto/auth/__pycache__/permissions.cpython-310.pyc
--rw-r--r--   0        0        0     4037 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/auth/pat.py
--rw-r--r--   0        0        0      548 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/auth/permissions.py
--rw-r--r--   0        0        0      170 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/__init__.py
--rw-r--r--   0        0        0      430 2024-01-11 21:14:15.068552 roboto-0.2.8/src/roboto/cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1718 2024-01-11 21:14:15.800552 roboto-0.2.8/src/roboto/cli/__pycache__/argparse.cpython-310.pyc
--rw-r--r--   0        0        0     2272 2024-01-11 21:14:15.828552 roboto-0.2.8/src/roboto/cli/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     2140 2024-01-11 21:14:15.800552 roboto-0.2.8/src/roboto/cli/__pycache__/context.cpython-310.pyc
--rw-r--r--   0        0        0     5828 2024-01-11 21:14:15.072552 roboto-0.2.8/src/roboto/cli/__pycache__/entry.cpython-310.pyc
--rw-r--r--   0        0        0      990 2024-01-11 21:14:15.804552 roboto-0.2.8/src/roboto/cli/__pycache__/terminal.cpython-310.pyc
--rw-r--r--   0        0        0     1887 2024-01-11 21:14:15.808552 roboto-0.2.8/src/roboto/cli/__pycache__/validation.cpython-310.pyc
--rw-r--r--   0        0        0      111 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/actions/__init__.py
--rw-r--r--   0        0        0      380 2024-01-11 21:14:15.800552 roboto-0.2.8/src/roboto/cli/actions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2267 2024-01-11 21:14:15.808552 roboto-0.2.8/src/roboto/cli/actions/__pycache__/action_config.cpython-310.pyc
--rw-r--r--   0        0        0      902 2024-01-11 21:14:15.800552 roboto-0.2.8/src/roboto/cli/actions/__pycache__/commands.cpython-310.pyc
--rw-r--r--   0        0        0     8256 2024-01-11 21:14:15.804552 roboto-0.2.8/src/roboto/cli/actions/__pycache__/create.cpython-310.pyc
--rw-r--r--   0        0        0     1351 2024-01-11 21:14:15.816552 roboto-0.2.8/src/roboto/cli/actions/__pycache__/delete.cpython-310.pyc
--rw-r--r--   0        0        0     3237 2024-01-11 21:14:15.816552 roboto-0.2.8/src/roboto/cli/actions/__pycache__/invoke.cpython-310.pyc
--rw-r--r--   0        0        0     2376 2024-01-11 21:14:15.816552 roboto-0.2.8/src/roboto/cli/actions/__pycache__/list_invocations.cpython-310.pyc
--rw-r--r--   0        0        0     2889 2024-01-11 21:14:15.820552 roboto-0.2.8/src/roboto/cli/actions/__pycache__/search.cpython-310.pyc
--rw-r--r--   0        0        0     1303 2024-01-11 21:14:15.820552 roboto-0.2.8/src/roboto/cli/actions/__pycache__/show.cpython-310.pyc
--rw-r--r--   0        0        0     5032 2024-01-11 21:14:15.820552 roboto-0.2.8/src/roboto/cli/actions/__pycache__/update.cpython-310.pyc
--rw-r--r--   0        0        0     1989 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/actions/action_config.py
--rw-r--r--   0        0        0      714 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/actions/commands.py
--rw-r--r--   0        0        0    12384 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/actions/create.py
--rw-r--r--   0        0        0      981 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/actions/delete.py
--rw-r--r--   0        0        0     3643 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/actions/invoke.py
--rw-r--r--   0        0        0     2614 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/actions/list_invocations.py
--rw-r--r--   0        0        0     3366 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/actions/search.py
--rw-r--r--   0        0        0      941 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/actions/show.py
--rw-r--r--   0        0        0     6375 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/actions/update.py
--rw-r--r--   0        0        0     1103 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/argparse.py
--rw-r--r--   0        0        0      579 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/collections/__init__.py
--rw-r--r--   0        0        0      794 2024-01-11 21:14:15.820552 roboto-0.2.8/src/roboto/cli/collections/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1643 2024-01-11 21:14:15.824552 roboto-0.2.8/src/roboto/cli/collections/__pycache__/changes.cpython-310.pyc
--rw-r--r--   0        0        0     2186 2024-01-11 21:14:15.824552 roboto-0.2.8/src/roboto/cli/collections/__pycache__/create.cpython-310.pyc
--rw-r--r--   0        0        0     1220 2024-01-11 21:14:15.824552 roboto-0.2.8/src/roboto/cli/collections/__pycache__/delete.cpython-310.pyc
--rw-r--r--   0        0        0      946 2024-01-11 21:14:15.824552 roboto-0.2.8/src/roboto/cli/collections/__pycache__/list.cpython-310.pyc
--rw-r--r--   0        0        0      869 2024-01-11 21:14:15.824552 roboto-0.2.8/src/roboto/cli/collections/__pycache__/shared_helpdoc.cpython-310.pyc
--rw-r--r--   0        0        0     1924 2024-01-11 21:14:15.824552 roboto-0.2.8/src/roboto/cli/collections/__pycache__/show.cpython-310.pyc
--rw-r--r--   0        0        0     3072 2024-01-11 21:14:15.824552 roboto-0.2.8/src/roboto/cli/collections/__pycache__/update.cpython-310.pyc
--rw-r--r--   0        0        0     1388 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/collections/changes.py
--rw-r--r--   0        0        0     2276 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/collections/create.py
--rw-r--r--   0        0        0      885 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/collections/delete.py
--rw-r--r--   0        0        0      591 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/collections/list.py
--rw-r--r--   0        0        0     1063 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/collections/list_all.py
--rw-r--r--   0        0        0      620 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/collections/shared_helpdoc.py
--rw-r--r--   0        0        0     1482 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/collections/show.py
--rw-r--r--   0        0        0     3924 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/collections/update.py
--rw-r--r--   0        0        0      334 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/command/__init__.py
--rw-r--r--   0        0        0      543 2024-01-11 21:14:15.800552 roboto-0.2.8/src/roboto/cli/command/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1915 2024-01-11 21:14:15.800552 roboto-0.2.8/src/roboto/cli/command/__pycache__/args.cpython-310.pyc
--rw-r--r--   0        0        0     3819 2024-01-11 21:14:15.800552 roboto-0.2.8/src/roboto/cli/command/__pycache__/model.cpython-310.pyc
--rw-r--r--   0        0        0     1691 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/command/args.py
--rw-r--r--   0        0        0     3247 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/command/model.py
--rw-r--r--   0        0        0      579 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/common_args/__init__.py
--rw-r--r--   0        0        0      692 2024-01-11 21:14:15.804552 roboto-0.2.8/src/roboto/cli/common_args/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9562 2024-01-11 21:14:15.808552 roboto-0.2.8/src/roboto/cli/common_args/__pycache__/actions.cpython-310.pyc
--rw-r--r--   0        0        0      834 2024-01-11 21:14:15.808552 roboto-0.2.8/src/roboto/cli/common_args/__pycache__/orgs.cpython-310.pyc
--rw-r--r--   0        0        0    11809 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/common_args/actions.py
--rw-r--r--   0        0        0      500 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/common_args/orgs.py
--rw-r--r--   0        0        0     2257 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/config.py
--rw-r--r--   0        0        0     1700 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/context.py
--rw-r--r--   0        0        0      110 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/__init__.py
--rw-r--r--   0        0        0      388 2024-01-11 21:14:15.828552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1061 2024-01-11 21:14:15.832552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/commands.cpython-310.pyc
--rw-r--r--   0        0        0     1737 2024-01-11 21:14:15.832552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/create.cpython-310.pyc
--rw-r--r--   0        0        0     1341 2024-01-11 21:14:15.832552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/delete_dataset.cpython-310.pyc
--rw-r--r--   0        0        0     1529 2024-01-11 21:14:15.832552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/delete_files.cpython-310.pyc
--rw-r--r--   0        0        0     1765 2024-01-11 21:14:15.832552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/download_files.cpython-310.pyc
--rw-r--r--   0        0        0     1624 2024-01-11 21:14:15.832552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/list_files.cpython-310.pyc
--rw-r--r--   0        0        0     2411 2024-01-11 21:14:15.836552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/search.cpython-310.pyc
--rw-r--r--   0        0        0      394 2024-01-11 21:14:15.832552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/shared_helpdoc.cpython-310.pyc
--rw-r--r--   0        0        0     1307 2024-01-11 21:14:15.836552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/show.cpython-310.pyc
--rw-r--r--   0        0        0     2728 2024-01-11 21:14:15.836552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/update.cpython-310.pyc
--rw-r--r--   0        0        0     2115 2024-01-11 21:14:15.836552 roboto-0.2.8/src/roboto/cli/datasets/__pycache__/upload_files.cpython-310.pyc
--rw-r--r--   0        0        0      882 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/commands.py
--rw-r--r--   0        0        0     1527 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/create.py
--rw-r--r--   0        0        0      981 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/delete_dataset.py
--rw-r--r--   0        0        0     1271 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/delete_files.py
--rw-r--r--   0        0        0     1585 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/download_files.py
--rw-r--r--   0        0        0     1351 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/list_files.py
--rw-r--r--   0        0        0     2566 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/search.py
--rw-r--r--   0        0        0       67 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/shared_helpdoc.py
--rw-r--r--   0        0        0      903 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/show.py
--rw-r--r--   0        0        0     2885 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/update.py
--rw-r--r--   0        0        0     2083 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/datasets/upload_files.py
--rw-r--r--   0        0        0     8248 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/entry.py
--rw-r--r--   0        0        0      313 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/extension/__init__.py
--rw-r--r--   0        0        0      490 2024-01-11 21:14:15.836552 roboto-0.2.8/src/roboto/cli/extension/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2540 2024-01-11 21:14:15.836552 roboto-0.2.8/src/roboto/cli/extension/__pycache__/cli_extension.cpython-310.pyc
--rw-r--r--   0        0        0     2347 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/extension/cli_extension.py
--rw-r--r--   0        0        0      111 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/images/__init__.py
--rw-r--r--   0        0        0      379 2024-01-11 21:14:15.840552 roboto-0.2.8/src/roboto/cli/images/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      886 2024-01-11 21:14:15.840552 roboto-0.2.8/src/roboto/cli/images/__pycache__/commands.cpython-310.pyc
--rw-r--r--   0        0        0     1346 2024-01-11 21:14:15.840552 roboto-0.2.8/src/roboto/cli/images/__pycache__/delete_image.cpython-310.pyc
--rw-r--r--   0        0        0     1463 2024-01-11 21:14:15.856552 roboto-0.2.8/src/roboto/cli/images/__pycache__/delete_repo.cpython-310.pyc
--rw-r--r--   0        0        0     1531 2024-01-11 21:14:15.856552 roboto-0.2.8/src/roboto/cli/images/__pycache__/list_images.cpython-310.pyc
--rw-r--r--   0        0        0     1366 2024-01-11 21:14:15.856552 roboto-0.2.8/src/roboto/cli/images/__pycache__/list_repos.cpython-310.pyc
--rw-r--r--   0        0        0     2183 2024-01-11 21:14:15.856552 roboto-0.2.8/src/roboto/cli/images/__pycache__/login.cpython-310.pyc
--rw-r--r--   0        0        0     2337 2024-01-11 21:14:15.856552 roboto-0.2.8/src/roboto/cli/images/__pycache__/pull.cpython-310.pyc
--rw-r--r--   0        0        0     4438 2024-01-11 21:14:15.856552 roboto-0.2.8/src/roboto/cli/images/__pycache__/push.cpython-310.pyc
--rw-r--r--   0        0        0      631 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/images/commands.py
--rw-r--r--   0        0        0     1058 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/images/delete_image.py
--rw-r--r--   0        0        0     1254 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/images/delete_repo.py
--rw-r--r--   0        0        0     1444 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/images/list_images.py
--rw-r--r--   0        0        0     1173 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/images/list_repos.py
--rw-r--r--   0        0        0     1939 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/images/login.py
--rw-r--r--   0        0        0     2307 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/images/pull.py
--rw-r--r--   0        0        0     5238 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/images/push.py
--rw-r--r--   0        0        0      516 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/invocations/__init__.py
--rw-r--r--   0        0        0      743 2024-01-11 21:14:15.860552 roboto-0.2.8/src/roboto/cli/invocations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2024-01-11 21:14:15.860552 roboto-0.2.8/src/roboto/cli/invocations/__pycache__/cancel.cpython-310.pyc
--rw-r--r--   0        0        0     2707 2024-01-11 21:14:15.860552 roboto-0.2.8/src/roboto/cli/invocations/__pycache__/logs.cpython-310.pyc
--rw-r--r--   0        0        0     1169 2024-01-11 21:14:15.860552 roboto-0.2.8/src/roboto/cli/invocations/__pycache__/show.cpython-310.pyc
--rw-r--r--   0        0        0     1981 2024-01-11 21:14:15.860552 roboto-0.2.8/src/roboto/cli/invocations/__pycache__/status.cpython-310.pyc
--rw-r--r--   0        0        0      818 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/invocations/cancel.py
--rw-r--r--   0        0        0     4227 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/invocations/logs.py
--rw-r--r--   0        0        0      780 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/invocations/show.py
--rw-r--r--   0        0        0     2025 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/invocations/status.py
--rw-r--r--   0        0        0      110 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/orgs/__init__.py
--rw-r--r--   0        0        0      384 2024-01-11 21:14:15.860552 roboto-0.2.8/src/roboto/cli/orgs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9643 2024-01-11 21:14:15.864552 roboto-0.2.8/src/roboto/cli/orgs/__pycache__/commands.cpython-310.pyc
--rw-r--r--   0        0        0    11296 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/orgs/commands.py
--rw-r--r--   0        0        0      490 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/terminal.py
--rw-r--r--   0        0        0      110 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/tokens/__init__.py
--rw-r--r--   0        0        0      386 2024-01-11 21:14:15.864552 roboto-0.2.8/src/roboto/cli/tokens/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3276 2024-01-11 21:14:15.864552 roboto-0.2.8/src/roboto/cli/tokens/__pycache__/commands.cpython-310.pyc
--rw-r--r--   0        0        0     3269 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/triggers/__init__.py
--rw-r--r--   0        0        0      388 2024-01-11 21:14:15.864552 roboto-0.2.8/src/roboto/cli/triggers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    11543 2024-01-11 21:14:15.868552 roboto-0.2.8/src/roboto/cli/triggers/__pycache__/commands.cpython-310.pyc
--rw-r--r--   0        0        0    17798 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/users/__init__.py
--rw-r--r--   0        0        0      385 2024-01-11 21:14:15.868552 roboto-0.2.8/src/roboto/cli/users/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3315 2024-01-11 21:14:15.868552 roboto-0.2.8/src/roboto/cli/users/__pycache__/commands.cpython-310.pyc
--rw-r--r--   0        0        0     3277 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/users/commands.py
--rw-r--r--   0        0        0     1162 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/cli/validation.py
--rw-r--r--   0        0        0      120 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/__init__.py
--rw-r--r--   0        0        0      390 2024-01-11 21:14:15.072552 roboto-0.2.8/src/roboto/domain/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2382 2024-01-11 21:14:15.072552 roboto-0.2.8/src/roboto/domain/__pycache__/http_delegates.cpython-310.pyc
--rw-r--r--   0        0        0     2094 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/__init__.py
--rw-r--r--   0        0        0     1839 2024-01-11 21:14:15.508552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7503 2024-01-11 21:14:15.508552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/action.cpython-310.pyc
--rw-r--r--   0        0        0     3119 2024-01-11 21:14:15.512552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/action_container_resources.cpython-310.pyc
--rw-r--r--   0        0        0     3295 2024-01-11 21:14:15.516552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/action_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     6529 2024-01-11 21:14:15.560552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     2667 2024-01-11 21:14:15.560552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/action_http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     6403 2024-01-11 21:14:15.516552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/action_record.cpython-310.pyc
--rw-r--r--   0        0        0     7838 2024-01-11 21:14:15.536552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation.cpython-310.pyc
--rw-r--r--   0        0        0     3024 2024-01-11 21:14:15.536552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     6556 2024-01-11 21:14:15.576552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1445 2024-01-11 21:14:15.576552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     6152 2024-01-11 21:14:15.536552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation_record.cpython-310.pyc
--rw-r--r--   0        0        0     1199 2024-01-11 21:14:15.580552 roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation_runtime_resources.cpython-310.pyc
--rw-r--r--   0        0        0     9326 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/action.py
--rw-r--r--   0        0        0     3165 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/action_container_resources.py
--rw-r--r--   0        0        0     3138 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/action_delegate.py
--rw-r--r--   0        0        0     8201 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/action_http_delegate.py
--rw-r--r--   0        0        0     2302 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/action_http_resources.py
--rw-r--r--   0        0        0     5697 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/action_record.py
--rw-r--r--   0        0        0     7657 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/invocation.py
--rw-r--r--   0        0        0     2506 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/invocation_delegate.py
--rw-r--r--   0        0        0     7117 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      827 2024-01-11 21:12:42.008484 roboto-0.2.8/src/roboto/domain/actions/invocation_http_resources.py
--rw-r--r--   0        0        0     6240 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/actions/invocation_record.py
--rw-r--r--   0        0        0      990 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/actions/invocation_runtime_resources.py
--rw-r--r--   0        0        0      827 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/collections/__init__.py
--rw-r--r--   0        0        0      906 2024-01-11 21:14:15.580552 roboto-0.2.8/src/roboto/domain/collections/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3937 2024-01-11 21:14:15.584552 roboto-0.2.8/src/roboto/domain/collections/__pycache__/collection.cpython-310.pyc
--rw-r--r--   0        0        0     2915 2024-01-11 21:14:15.584552 roboto-0.2.8/src/roboto/domain/collections/__pycache__/collection_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     5732 2024-01-11 21:14:15.600552 roboto-0.2.8/src/roboto/domain/collections/__pycache__/collection_http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1475 2024-01-11 21:14:15.600552 roboto-0.2.8/src/roboto/domain/collections/__pycache__/collection_http_resource.cpython-310.pyc
--rw-r--r--   0        0        0     2508 2024-01-11 21:14:15.584552 roboto-0.2.8/src/roboto/domain/collections/__pycache__/collection_record.cpython-310.pyc
--rw-r--r--   0        0        0     4861 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/collections/collection.py
--rw-r--r--   0        0        0     2679 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/collections/collection_delegate.py
--rw-r--r--   0        0        0     6721 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/collections/collection_http_delegate.py
--rw-r--r--   0        0        0      971 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/collections/collection_http_resource.py
--rw-r--r--   0        0        0     1697 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/collections/collection_record.py
--rw-r--r--   0        0        0      468 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/comments/__init__.py
--rw-r--r--   0        0        0      676 2024-01-11 21:14:15.604552 roboto-0.2.8/src/roboto/domain/comments/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3612 2024-01-11 21:14:15.608552 roboto-0.2.8/src/roboto/domain/comments/__pycache__/comment.cpython-310.pyc
--rw-r--r--   0        0        0     2418 2024-01-11 21:14:15.608552 roboto-0.2.8/src/roboto/domain/comments/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     4548 2024-01-11 21:14:15.612552 roboto-0.2.8/src/roboto/domain/comments/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      853 2024-01-11 21:14:15.612552 roboto-0.2.8/src/roboto/domain/comments/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1172 2024-01-11 21:14:15.608552 roboto-0.2.8/src/roboto/domain/comments/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     3549 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/comments/comment.py
--rw-r--r--   0        0        0     1964 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/comments/delegate.py
--rw-r--r--   0        0        0     5153 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/comments/http_delegate.py
--rw-r--r--   0        0        0      239 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/comments/http_resources.py
--rw-r--r--   0        0        0      776 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/comments/record.py
--rw-r--r--   0        0        0      678 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/datasets/__init__.py
--rw-r--r--   0        0        0      813 2024-01-11 21:14:15.616552 roboto-0.2.8/src/roboto/domain/datasets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    16874 2024-01-11 21:14:15.620552 roboto-0.2.8/src/roboto/domain/datasets/__pycache__/dataset.cpython-310.pyc
--rw-r--r--   0        0        0     4248 2024-01-11 21:14:15.708552 roboto-0.2.8/src/roboto/domain/datasets/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     7311 2024-01-11 21:14:15.716552 roboto-0.2.8/src/roboto/domain/datasets/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1912 2024-01-11 21:14:15.720552 roboto-0.2.8/src/roboto/domain/datasets/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1367 2024-01-11 21:14:15.708552 roboto-0.2.8/src/roboto/domain/datasets/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0    21457 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/datasets/dataset.py
--rw-r--r--   0        0        0     3479 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/datasets/delegate.py
--rw-r--r--   0        0        0     7970 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/datasets/http_delegate.py
--rw-r--r--   0        0        0     1089 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/datasets/http_resources.py
--rw-r--r--   0        0        0     1239 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/datasets/record.py
--rw-r--r--   0        0        0      943 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/files/__init__.py
--rw-r--r--   0        0        0     1027 2024-01-11 21:14:15.628552 roboto-0.2.8/src/roboto/domain/files/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    10480 2024-01-11 21:14:15.632552 roboto-0.2.8/src/roboto/domain/files/__pycache__/client_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     3708 2024-01-11 21:14:15.680552 roboto-0.2.8/src/roboto/domain/files/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     4518 2024-01-11 21:14:15.704552 roboto-0.2.8/src/roboto/domain/files/__pycache__/file.cpython-310.pyc
--rw-r--r--   0        0        0     1322 2024-01-11 21:14:15.704552 roboto-0.2.8/src/roboto/domain/files/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     6512 2024-01-11 21:14:15.680552 roboto-0.2.8/src/roboto/domain/files/__pycache__/progress.cpython-310.pyc
--rw-r--r--   0        0        0     1230 2024-01-11 21:14:15.700552 roboto-0.2.8/src/roboto/domain/files/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0    13261 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/files/client_delegate.py
--rw-r--r--   0        0        0     3294 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/files/delegate.py
--rw-r--r--   0        0        0     3910 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/files/file.py
--rw-r--r--   0        0        0      500 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/files/http_resources.py
--rw-r--r--   0        0        0     4606 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/files/progress.py
--rw-r--r--   0        0        0      921 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/files/record.py
--rw-r--r--   0        0        0     2677 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/http_delegates.py
--rw-r--r--   0        0        0      902 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/orgs/__init__.py
--rw-r--r--   0        0        0     1002 2024-01-11 21:14:15.728552 roboto-0.2.8/src/roboto/domain/orgs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4329 2024-01-11 21:14:15.728552 roboto-0.2.8/src/roboto/domain/orgs/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     8391 2024-01-11 21:14:15.748552 roboto-0.2.8/src/roboto/domain/orgs/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1757 2024-01-11 21:14:15.748552 roboto-0.2.8/src/roboto/domain/orgs/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     4929 2024-01-11 21:14:15.756552 roboto-0.2.8/src/roboto/domain/orgs/__pycache__/org.cpython-310.pyc
--rw-r--r--   0        0        0     3310 2024-01-11 21:14:15.756552 roboto-0.2.8/src/roboto/domain/orgs/__pycache__/org_invite.cpython-310.pyc
--rw-r--r--   0        0        0     2913 2024-01-11 21:14:15.756552 roboto-0.2.8/src/roboto/domain/orgs/__pycache__/org_role.cpython-310.pyc
--rw-r--r--   0        0        0     1750 2024-01-11 21:14:15.728552 roboto-0.2.8/src/roboto/domain/orgs/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     3589 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/orgs/delegate.py
--rw-r--r--   0        0        0     8997 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      740 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     4075 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/orgs/org.py
--rw-r--r--   0        0        0     2413 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/orgs/org_invite.py
--rw-r--r--   0        0        0     1921 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/orgs/org_role.py
--rw-r--r--   0        0        0      775 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/orgs/record.py
--rw-r--r--   0        0        0      452 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/tokens/__init__.py
--rw-r--r--   0        0        0      669 2024-01-11 21:14:15.756552 roboto-0.2.8/src/roboto/domain/tokens/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1453 2024-01-11 21:14:15.756552 roboto-0.2.8/src/roboto/domain/tokens/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     2967 2024-01-11 21:14:15.760552 roboto-0.2.8/src/roboto/domain/tokens/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      858 2024-01-11 21:14:15.764552 roboto-0.2.8/src/roboto/domain/tokens/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0      995 2024-01-11 21:14:15.756552 roboto-0.2.8/src/roboto/domain/tokens/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     2877 2024-01-11 21:14:15.764552 roboto-0.2.8/src/roboto/domain/tokens/__pycache__/token.cpython-310.pyc
--rw-r--r--   0        0        0      857 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/tokens/delegate.py
--rw-r--r--   0        0        0     2226 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      283 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      455 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/tokens/record.py
--rw-r--r--   0        0        0     2128 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/tokens/token.py
--rw-r--r--   0        0        0      888 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/topics/__init__.py
--rw-r--r--   0        0        0     2885 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/topics/topic.py
--rw-r--r--   0        0        0     2252 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/topics/topic_delegate.py
--rw-r--r--   0        0        0     3887 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/topics/topic_http_delegate.py
--rw-r--r--   0        0        0     5418 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/topics/topic_record.py
--rw-r--r--   0        0        0     2340 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/topics/topic_requests.py
--rw-r--r--   0        0        0      761 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/triggers/__init__.py
--rw-r--r--   0        0        0      864 2024-01-11 21:14:15.764552 roboto-0.2.8/src/roboto/domain/triggers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5341 2024-01-11 21:14:15.768552 roboto-0.2.8/src/roboto/domain/triggers/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     4468 2024-01-11 21:14:15.768552 roboto-0.2.8/src/roboto/domain/triggers/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     7954 2024-01-11 21:14:15.796552 roboto-0.2.8/src/roboto/domain/triggers/__pycache__/trigger.cpython-310.pyc
--rw-r--r--   0        0        0     2857 2024-01-11 21:14:15.792552 roboto-0.2.8/src/roboto/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     2105 2024-01-11 21:14:15.768552 roboto-0.2.8/src/roboto/domain/triggers/__pycache__/trigger_record.cpython-310.pyc
--rw-r--r--   0        0        0     6389 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0     4073 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/triggers/http_resources.py
--rw-r--r--   0        0        0    10159 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/triggers/trigger.py
--rw-r--r--   0        0        0     2837 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0     1667 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      357 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/users/__init__.py
--rw-r--r--   0        0        0      612 2024-01-11 21:14:15.728552 roboto-0.2.8/src/roboto/domain/users/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2587 2024-01-11 21:14:15.728552 roboto-0.2.8/src/roboto/domain/users/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     2864 2024-01-11 21:14:15.740552 roboto-0.2.8/src/roboto/domain/users/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1458 2024-01-11 21:14:15.732552 roboto-0.2.8/src/roboto/domain/users/__pycache__/user_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      899 2024-01-11 21:14:15.736552 roboto-0.2.8/src/roboto/domain/users/__pycache__/user_http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1393 2024-01-11 21:14:15.732552 roboto-0.2.8/src/roboto/domain/users/__pycache__/user_record.cpython-310.pyc
--rw-r--r--   0        0        0     2308 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/users/http_delegate.py
--rw-r--r--   0        0        0     2271 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/users/user.py
--rw-r--r--   0        0        0      935 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/users/user_delegate.py
--rw-r--r--   0        0        0      456 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/users/user_http_resources.py
--rw-r--r--   0        0        0      886 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/domain/users/user_record.py
--rw-r--r--   0        0        0     1101 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/exceptions/__init__.py
--rw-r--r--   0        0        0     1052 2024-01-11 21:14:15.120552 roboto-0.2.8/src/roboto/exceptions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    10221 2024-01-11 21:14:15.124552 roboto-0.2.8/src/roboto/exceptions/__pycache__/domain.cpython-310.pyc
--rw-r--r--   0        0        0     2278 2024-01-11 21:14:15.124552 roboto-0.2.8/src/roboto/exceptions/__pycache__/http.cpython-310.pyc
--rw-r--r--   0        0        0     8433 2024-01-11 21:12:42.012484 roboto-0.2.8/src/roboto/exceptions/domain.py
--rw-r--r--   0        0        0     1334 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/exceptions/http.py
--rw-r--r--   0        0        0     1316 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/http/__init__.py
--rw-r--r--   0        0        0     1260 2024-01-11 21:14:15.072552 roboto-0.2.8/src/roboto/http/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      646 2024-01-11 21:14:15.072552 roboto-0.2.8/src/roboto/http/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0      874 2024-01-11 21:14:15.072552 roboto-0.2.8/src/roboto/http/__pycache__/headers.cpython-310.pyc
--rw-r--r--   0        0        0     9668 2024-01-11 21:14:15.076552 roboto-0.2.8/src/roboto/http/__pycache__/http_client.cpython-310.pyc
--rw-r--r--   0        0        0     3977 2024-01-11 21:14:15.124552 roboto-0.2.8/src/roboto/http/__pycache__/request_decorators.cpython-310.pyc
--rw-r--r--   0        0        0     6721 2024-01-11 21:14:15.496552 roboto-0.2.8/src/roboto/http/__pycache__/response.cpython-310.pyc
--rw-r--r--   0        0        0     2489 2024-01-11 21:14:15.508552 roboto-0.2.8/src/roboto/http/__pycache__/testing_util.cpython-310.pyc
--rw-r--r--   0        0        0      834 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/http/constants.py
--rw-r--r--   0        0        0      766 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/http/headers.py
--rw-r--r--   0        0        0    10563 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/http/http_client.py
--rw-r--r--   0        0        0     3177 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/http/request_decorators.py
--rw-r--r--   0        0        0     5800 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/http/response.py
--rw-r--r--   0        0        0     1819 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/http/testing_util.py
--rw-r--r--   0        0        0      951 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/image_registry/__init__.py
--rw-r--r--   0        0        0      967 2024-01-11 21:14:15.840552 roboto-0.2.8/src/roboto/image_registry/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2024-01-11 21:14:15.840552 roboto-0.2.8/src/roboto/image_registry/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     8394 2024-01-11 21:14:15.848552 roboto-0.2.8/src/roboto/image_registry/__pycache__/image_registry.cpython-310.pyc
--rw-r--r--   0        0        0      800 2024-01-11 21:14:15.848552 roboto-0.2.8/src/roboto/image_registry/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0      913 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/image_registry/http_resources.py
--rw-r--r--   0        0        0     9136 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/image_registry/image_registry.py
--rw-r--r--   0        0        0      283 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/image_registry/record.py
--rw-r--r--   0        0        0      154 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/logging.py
--rw-r--r--   0        0        0      201 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/notifications/__init__.py
--rw-r--r--   0        0        0      498 2024-01-11 21:14:15.728552 roboto-0.2.8/src/roboto/notifications/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2282 2024-01-11 21:14:15.732552 roboto-0.2.8/src/roboto/notifications/__pycache__/http_client.cpython-310.pyc
--rw-r--r--   0        0        0      721 2024-01-11 21:14:15.732552 roboto-0.2.8/src/roboto/notifications/__pycache__/notifications.cpython-310.pyc
--rw-r--r--   0        0        0     1929 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/notifications/http_client.py
--rw-r--r--   0        0        0      444 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/notifications/notifications.py
--rw-r--r--   0        0        0      303 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/profile/__init__.py
--rw-r--r--   0        0        0      502 2024-01-11 21:14:15.492552 roboto-0.2.8/src/roboto/profile/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3828 2024-01-11 21:14:15.492552 roboto-0.2.8/src/roboto/profile/__pycache__/profile.cpython-310.pyc
--rw-r--r--   0        0        0     3730 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/profile/profile.py
--rw-r--r--   0        0        0        0 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/py.typed
--rw-r--r--   0        0        0      238 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/pydantic/__init__.py
--rw-r--r--   0        0        0      456 2024-01-11 21:14:15.520552 roboto-0.2.8/src/roboto/pydantic/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      804 2024-01-11 21:14:15.520552 roboto-0.2.8/src/roboto/pydantic/__pycache__/serializers.cpython-310.pyc
--rw-r--r--   0        0        0     2441 2024-01-11 21:14:15.520552 roboto-0.2.8/src/roboto/pydantic/__pycache__/validators.cpython-310.pyc
--rw-r--r--   0        0        0      524 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/pydantic/serializers.py
--rw-r--r--   0        0        0     1869 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/pydantic/validators.py
--rw-r--r--   0        0        0      543 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/query/__init__.py
--rw-r--r--   0        0        0      728 2024-01-11 21:14:14.804551 roboto-0.2.8/src/roboto/query/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4550 2024-01-11 21:14:14.804551 roboto-0.2.8/src/roboto/query/__pycache__/conditions.cpython-310.pyc
--rw-r--r--   0        0        0     1511 2024-01-11 21:14:15.016552 roboto-0.2.8/src/roboto/query/__pycache__/precanned.cpython-310.pyc
--rw-r--r--   0        0        0     4438 2024-01-11 21:14:15.016552 roboto-0.2.8/src/roboto/query/__pycache__/query.cpython-310.pyc
--rw-r--r--   0        0        0     1948 2024-01-11 21:14:15.020552 roboto-0.2.8/src/roboto/query/__pycache__/visitor.cpython-310.pyc
--rw-r--r--   0        0        0     4516 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/query/conditions.py
--rw-r--r--   0        0        0     1671 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/query/precanned.py
--rw-r--r--   0        0        0     3861 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/query/query.py
--rw-r--r--   0        0        0     1394 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/query/visitor.py
--rw-r--r--   0        0        0     2449 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/sentinels.py
--rw-r--r--   0        0        0      734 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/serde/__init__.py
--rw-r--r--   0        0        0      873 2024-01-11 21:14:14.812551 roboto-0.2.8/src/roboto/serde/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      493 2024-01-11 21:14:14.812551 roboto-0.2.8/src/roboto/serde/__pycache__/arrays.cpython-310.pyc
--rw-r--r--   0        0        0     2199 2024-01-11 21:14:14.812551 roboto-0.2.8/src/roboto/serde/__pycache__/dicts.cpython-310.pyc
--rw-r--r--   0        0        0      901 2024-01-11 21:14:14.928552 roboto-0.2.8/src/roboto/serde/__pycache__/paths.cpython-310.pyc
--rw-r--r--   0        0        0      158 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/serde/arrays.py
--rw-r--r--   0        0        0     1713 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/serde/dicts.py
--rw-r--r--   0        0        0      801 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/serde/paths.py
--rw-r--r--   0        0        0      182 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/time.py
--rw-r--r--   0        0        0      558 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/transactions/__init__.py
--rw-r--r--   0        0        0      732 2024-01-11 21:14:15.620552 roboto-0.2.8/src/roboto/transactions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      947 2024-01-11 21:14:15.620552 roboto-0.2.8/src/roboto/transactions/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1550 2024-01-11 21:14:15.628552 roboto-0.2.8/src/roboto/transactions/__pycache__/manager_abc.cpython-310.pyc
--rw-r--r--   0        0        0     1841 2024-01-11 21:14:15.620552 roboto-0.2.8/src/roboto/transactions/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     2983 2024-01-11 21:14:15.628552 roboto-0.2.8/src/roboto/transactions/__pycache__/transaction_manager.cpython-310.pyc
--rw-r--r--   0        0        0      318 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/transactions/http_resources.py
--rw-r--r--   0        0        0     1043 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/transactions/manager_abc.py
--rw-r--r--   0        0        0     1099 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/transactions/record.py
--rw-r--r--   0        0        0     3198 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/transactions/transaction_manager.py
--rw-r--r--   0        0        0      225 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/types.py
--rw-r--r--   0        0        0     7347 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/updates.py
--rw-r--r--   0        0        0     1819 2024-01-11 21:12:42.016484 roboto-0.2.8/src/roboto/waiters.py
--rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 roboto-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      472 2024-01-17 21:35:46.697574 roboto-0.2.9/README.md
+-rw-r--r--   0        0        0      993 2024-01-17 21:39:27.304904 roboto-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/__init__.py
+-rw-r--r--   0        0        0     1470 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/association.py
+-rw-r--r--   0        0        0      114 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/auth/__init__.py
+-rw-r--r--   0        0        0      376 2024-01-17 21:37:10.825320 roboto-0.2.9/src/roboto/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3810 2024-01-17 21:37:10.829320 roboto-0.2.9/src/roboto/auth/__pycache__/pat.cpython-310.pyc
+-rw-r--r--   0        0        0     1002 2024-01-17 21:37:10.825320 roboto-0.2.9/src/roboto/auth/__pycache__/permissions.cpython-310.pyc
+-rw-r--r--   0        0        0     4037 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/auth/pat.py
+-rw-r--r--   0        0        0      548 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/auth/permissions.py
+-rw-r--r--   0        0        0      170 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/cli/__init__.py
+-rw-r--r--   0        0        0      430 2024-01-17 21:37:10.489321 roboto-0.2.9/src/roboto/cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1718 2024-01-17 21:37:11.165319 roboto-0.2.9/src/roboto/cli/__pycache__/argparse.cpython-310.pyc
+-rw-r--r--   0        0        0     2272 2024-01-17 21:37:11.189319 roboto-0.2.9/src/roboto/cli/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     2140 2024-01-17 21:37:11.165319 roboto-0.2.9/src/roboto/cli/__pycache__/context.cpython-310.pyc
+-rw-r--r--   0        0        0     5828 2024-01-17 21:37:10.489321 roboto-0.2.9/src/roboto/cli/__pycache__/entry.cpython-310.pyc
+-rw-r--r--   0        0        0      990 2024-01-17 21:37:11.165319 roboto-0.2.9/src/roboto/cli/__pycache__/terminal.cpython-310.pyc
+-rw-r--r--   0        0        0     1887 2024-01-17 21:37:11.173318 roboto-0.2.9/src/roboto/cli/__pycache__/validation.cpython-310.pyc
+-rw-r--r--   0        0        0      111 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/cli/actions/__init__.py
+-rw-r--r--   0        0        0      380 2024-01-17 21:37:11.161319 roboto-0.2.9/src/roboto/cli/actions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2267 2024-01-17 21:37:11.173318 roboto-0.2.9/src/roboto/cli/actions/__pycache__/action_config.cpython-310.pyc
+-rw-r--r--   0        0        0      902 2024-01-17 21:37:11.165319 roboto-0.2.9/src/roboto/cli/actions/__pycache__/commands.cpython-310.pyc
+-rw-r--r--   0        0        0     8256 2024-01-17 21:37:11.169319 roboto-0.2.9/src/roboto/cli/actions/__pycache__/create.cpython-310.pyc
+-rw-r--r--   0        0        0     1351 2024-01-17 21:37:11.181319 roboto-0.2.9/src/roboto/cli/actions/__pycache__/delete.cpython-310.pyc
+-rw-r--r--   0        0        0     3237 2024-01-17 21:37:11.181319 roboto-0.2.9/src/roboto/cli/actions/__pycache__/invoke.cpython-310.pyc
+-rw-r--r--   0        0        0     2376 2024-01-17 21:37:11.181319 roboto-0.2.9/src/roboto/cli/actions/__pycache__/list_invocations.cpython-310.pyc
+-rw-r--r--   0        0        0     2889 2024-01-17 21:37:11.181319 roboto-0.2.9/src/roboto/cli/actions/__pycache__/search.cpython-310.pyc
+-rw-r--r--   0        0        0     1303 2024-01-17 21:37:11.181319 roboto-0.2.9/src/roboto/cli/actions/__pycache__/show.cpython-310.pyc
+-rw-r--r--   0        0        0     5032 2024-01-17 21:37:11.185319 roboto-0.2.9/src/roboto/cli/actions/__pycache__/update.cpython-310.pyc
+-rw-r--r--   0        0        0     1989 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/cli/actions/action_config.py
+-rw-r--r--   0        0        0      714 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/cli/actions/commands.py
+-rw-r--r--   0        0        0    12384 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/cli/actions/create.py
+-rw-r--r--   0        0        0      981 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/cli/actions/delete.py
+-rw-r--r--   0        0        0     3643 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/cli/actions/invoke.py
+-rw-r--r--   0        0        0     2614 2024-01-17 21:35:46.697574 roboto-0.2.9/src/roboto/cli/actions/list_invocations.py
+-rw-r--r--   0        0        0     3366 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/actions/search.py
+-rw-r--r--   0        0        0      941 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/actions/show.py
+-rw-r--r--   0        0        0     6375 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/actions/update.py
+-rw-r--r--   0        0        0     1103 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/argparse.py
+-rw-r--r--   0        0        0      579 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/collections/__init__.py
+-rw-r--r--   0        0        0      794 2024-01-17 21:37:11.185319 roboto-0.2.9/src/roboto/cli/collections/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1643 2024-01-17 21:37:11.185319 roboto-0.2.9/src/roboto/cli/collections/__pycache__/changes.cpython-310.pyc
+-rw-r--r--   0        0        0     2186 2024-01-17 21:37:11.189319 roboto-0.2.9/src/roboto/cli/collections/__pycache__/create.cpython-310.pyc
+-rw-r--r--   0        0        0     1220 2024-01-17 21:37:11.189319 roboto-0.2.9/src/roboto/cli/collections/__pycache__/delete.cpython-310.pyc
+-rw-r--r--   0        0        0      946 2024-01-17 21:37:11.189319 roboto-0.2.9/src/roboto/cli/collections/__pycache__/list.cpython-310.pyc
+-rw-r--r--   0        0        0      869 2024-01-17 21:37:11.185319 roboto-0.2.9/src/roboto/cli/collections/__pycache__/shared_helpdoc.cpython-310.pyc
+-rw-r--r--   0        0        0     1924 2024-01-17 21:37:11.189319 roboto-0.2.9/src/roboto/cli/collections/__pycache__/show.cpython-310.pyc
+-rw-r--r--   0        0        0     3072 2024-01-17 21:37:11.189319 roboto-0.2.9/src/roboto/cli/collections/__pycache__/update.cpython-310.pyc
+-rw-r--r--   0        0        0     1388 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/collections/changes.py
+-rw-r--r--   0        0        0     2276 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/collections/create.py
+-rw-r--r--   0        0        0      885 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/collections/delete.py
+-rw-r--r--   0        0        0      591 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/collections/list.py
+-rw-r--r--   0        0        0     1063 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/collections/list_all.py
+-rw-r--r--   0        0        0      620 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/collections/shared_helpdoc.py
+-rw-r--r--   0        0        0     1482 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/collections/show.py
+-rw-r--r--   0        0        0     3924 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/collections/update.py
+-rw-r--r--   0        0        0      334 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/command/__init__.py
+-rw-r--r--   0        0        0      543 2024-01-17 21:37:11.165319 roboto-0.2.9/src/roboto/cli/command/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1915 2024-01-17 21:37:11.165319 roboto-0.2.9/src/roboto/cli/command/__pycache__/args.cpython-310.pyc
+-rw-r--r--   0        0        0     3819 2024-01-17 21:37:11.165319 roboto-0.2.9/src/roboto/cli/command/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     1691 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/command/args.py
+-rw-r--r--   0        0        0     3247 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/command/model.py
+-rw-r--r--   0        0        0      579 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/common_args/__init__.py
+-rw-r--r--   0        0        0      692 2024-01-17 21:37:11.169319 roboto-0.2.9/src/roboto/cli/common_args/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9562 2024-01-17 21:37:11.169319 roboto-0.2.9/src/roboto/cli/common_args/__pycache__/actions.cpython-310.pyc
+-rw-r--r--   0        0        0      834 2024-01-17 21:37:11.173318 roboto-0.2.9/src/roboto/cli/common_args/__pycache__/orgs.cpython-310.pyc
+-rw-r--r--   0        0        0    11809 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/common_args/actions.py
+-rw-r--r--   0        0        0      500 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/common_args/orgs.py
+-rw-r--r--   0        0        0     2257 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/config.py
+-rw-r--r--   0        0        0     1700 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/context.py
+-rw-r--r--   0        0        0      110 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/__init__.py
+-rw-r--r--   0        0        0      388 2024-01-17 21:37:11.193318 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1061 2024-01-17 21:37:11.193318 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/commands.cpython-310.pyc
+-rw-r--r--   0        0        0     1737 2024-01-17 21:37:11.193318 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/create.cpython-310.pyc
+-rw-r--r--   0        0        0     1256 2024-01-17 21:37:11.197318 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/delete_dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     1444 2024-01-17 21:37:11.197318 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/delete_files.cpython-310.pyc
+-rw-r--r--   0        0        0     1680 2024-01-17 21:37:11.197318 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/download_files.cpython-310.pyc
+-rw-r--r--   0        0        0     1539 2024-01-17 21:37:11.197318 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/list_files.cpython-310.pyc
+-rw-r--r--   0        0        0     2411 2024-01-17 21:37:11.197318 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/search.cpython-310.pyc
+-rw-r--r--   0        0        0      394 2024-01-17 21:37:11.197318 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/shared_helpdoc.cpython-310.pyc
+-rw-r--r--   0        0        0     1222 2024-01-17 21:37:11.201319 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/show.cpython-310.pyc
+-rw-r--r--   0        0        0     2643 2024-01-17 21:37:11.201319 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/update.cpython-310.pyc
+-rw-r--r--   0        0        0     2030 2024-01-17 21:37:11.201319 roboto-0.2.9/src/roboto/cli/datasets/__pycache__/upload_files.cpython-310.pyc
+-rw-r--r--   0        0        0      882 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/commands.py
+-rw-r--r--   0        0        0     1527 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/create.py
+-rw-r--r--   0        0        0      894 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/delete_dataset.py
+-rw-r--r--   0        0        0     1184 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/delete_files.py
+-rw-r--r--   0        0        0     1498 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/download_files.py
+-rw-r--r--   0        0        0     1264 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/list_files.py
+-rw-r--r--   0        0        0     2566 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/search.py
+-rw-r--r--   0        0        0       67 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/shared_helpdoc.py
+-rw-r--r--   0        0        0      816 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/show.py
+-rw-r--r--   0        0        0     2798 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/update.py
+-rw-r--r--   0        0        0     1996 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/datasets/upload_files.py
+-rw-r--r--   0        0        0     8248 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/entry.py
+-rw-r--r--   0        0        0      313 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/extension/__init__.py
+-rw-r--r--   0        0        0      490 2024-01-17 21:37:11.201319 roboto-0.2.9/src/roboto/cli/extension/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2540 2024-01-17 21:37:11.201319 roboto-0.2.9/src/roboto/cli/extension/__pycache__/cli_extension.cpython-310.pyc
+-rw-r--r--   0        0        0     2347 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/extension/cli_extension.py
+-rw-r--r--   0        0        0      111 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/images/__init__.py
+-rw-r--r--   0        0        0      379 2024-01-17 21:37:11.201319 roboto-0.2.9/src/roboto/cli/images/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      886 2024-01-17 21:37:11.201319 roboto-0.2.9/src/roboto/cli/images/__pycache__/commands.cpython-310.pyc
+-rw-r--r--   0        0        0     1346 2024-01-17 21:37:11.201319 roboto-0.2.9/src/roboto/cli/images/__pycache__/delete_image.cpython-310.pyc
+-rw-r--r--   0        0        0     1463 2024-01-17 21:37:11.217318 roboto-0.2.9/src/roboto/cli/images/__pycache__/delete_repo.cpython-310.pyc
+-rw-r--r--   0        0        0     1531 2024-01-17 21:37:11.217318 roboto-0.2.9/src/roboto/cli/images/__pycache__/list_images.cpython-310.pyc
+-rw-r--r--   0        0        0     1366 2024-01-17 21:37:11.217318 roboto-0.2.9/src/roboto/cli/images/__pycache__/list_repos.cpython-310.pyc
+-rw-r--r--   0        0        0     2183 2024-01-17 21:37:11.217318 roboto-0.2.9/src/roboto/cli/images/__pycache__/login.cpython-310.pyc
+-rw-r--r--   0        0        0     2337 2024-01-17 21:37:11.221318 roboto-0.2.9/src/roboto/cli/images/__pycache__/pull.cpython-310.pyc
+-rw-r--r--   0        0        0     4438 2024-01-17 21:37:11.221318 roboto-0.2.9/src/roboto/cli/images/__pycache__/push.cpython-310.pyc
+-rw-r--r--   0        0        0      631 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/images/commands.py
+-rw-r--r--   0        0        0     1058 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/images/delete_image.py
+-rw-r--r--   0        0        0     1254 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/images/delete_repo.py
+-rw-r--r--   0        0        0     1444 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/images/list_images.py
+-rw-r--r--   0        0        0     1173 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/images/list_repos.py
+-rw-r--r--   0        0        0     1939 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/images/login.py
+-rw-r--r--   0        0        0     2307 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/images/pull.py
+-rw-r--r--   0        0        0     5238 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/images/push.py
+-rw-r--r--   0        0        0      516 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/invocations/__init__.py
+-rw-r--r--   0        0        0      743 2024-01-17 21:37:11.221318 roboto-0.2.9/src/roboto/cli/invocations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2024-01-17 21:37:11.221318 roboto-0.2.9/src/roboto/cli/invocations/__pycache__/cancel.cpython-310.pyc
+-rw-r--r--   0        0        0     2707 2024-01-17 21:37:11.221318 roboto-0.2.9/src/roboto/cli/invocations/__pycache__/logs.cpython-310.pyc
+-rw-r--r--   0        0        0     1169 2024-01-17 21:37:11.225319 roboto-0.2.9/src/roboto/cli/invocations/__pycache__/show.cpython-310.pyc
+-rw-r--r--   0        0        0     1981 2024-01-17 21:37:11.225319 roboto-0.2.9/src/roboto/cli/invocations/__pycache__/status.cpython-310.pyc
+-rw-r--r--   0        0        0      818 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/invocations/cancel.py
+-rw-r--r--   0        0        0     4227 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/invocations/logs.py
+-rw-r--r--   0        0        0      780 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/invocations/show.py
+-rw-r--r--   0        0        0     2025 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/invocations/status.py
+-rw-r--r--   0        0        0      110 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/orgs/__init__.py
+-rw-r--r--   0        0        0      384 2024-01-17 21:37:11.225319 roboto-0.2.9/src/roboto/cli/orgs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9643 2024-01-17 21:37:11.225319 roboto-0.2.9/src/roboto/cli/orgs/__pycache__/commands.cpython-310.pyc
+-rw-r--r--   0        0        0    11296 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/orgs/commands.py
+-rw-r--r--   0        0        0      490 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/terminal.py
+-rw-r--r--   0        0        0      110 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/tokens/__init__.py
+-rw-r--r--   0        0        0      386 2024-01-17 21:37:11.225319 roboto-0.2.9/src/roboto/cli/tokens/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3276 2024-01-17 21:37:11.229318 roboto-0.2.9/src/roboto/cli/tokens/__pycache__/commands.cpython-310.pyc
+-rw-r--r--   0        0        0     3269 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/triggers/__init__.py
+-rw-r--r--   0        0        0      388 2024-01-17 21:37:11.229318 roboto-0.2.9/src/roboto/cli/triggers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    11543 2024-01-17 21:37:11.229318 roboto-0.2.9/src/roboto/cli/triggers/__pycache__/commands.cpython-310.pyc
+-rw-r--r--   0        0        0    17798 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/users/__init__.py
+-rw-r--r--   0        0        0      385 2024-01-17 21:37:11.229318 roboto-0.2.9/src/roboto/cli/users/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3315 2024-01-17 21:37:11.233318 roboto-0.2.9/src/roboto/cli/users/__pycache__/commands.cpython-310.pyc
+-rw-r--r--   0        0        0     3277 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/users/commands.py
+-rw-r--r--   0        0        0     1162 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/cli/validation.py
+-rw-r--r--   0        0        0      120 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/__init__.py
+-rw-r--r--   0        0        0      390 2024-01-17 21:37:10.493321 roboto-0.2.9/src/roboto/domain/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2382 2024-01-17 21:37:10.493321 roboto-0.2.9/src/roboto/domain/__pycache__/http_delegates.cpython-310.pyc
+-rw-r--r--   0        0        0     2094 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/__init__.py
+-rw-r--r--   0        0        0     1839 2024-01-17 21:37:10.897319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7503 2024-01-17 21:37:10.897319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/action.cpython-310.pyc
+-rw-r--r--   0        0        0     3119 2024-01-17 21:37:10.901319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/action_container_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     3295 2024-01-17 21:37:10.905319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/action_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     6529 2024-01-17 21:37:10.945319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     2667 2024-01-17 21:37:10.945319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/action_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     6403 2024-01-17 21:37:10.905319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/action_record.cpython-310.pyc
+-rw-r--r--   0        0        0     7838 2024-01-17 21:37:10.921319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation.cpython-310.pyc
+-rw-r--r--   0        0        0     3024 2024-01-17 21:37:10.921319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     6556 2024-01-17 21:37:10.957319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1445 2024-01-17 21:37:10.957319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     6152 2024-01-17 21:37:10.925319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation_record.cpython-310.pyc
+-rw-r--r--   0        0        0     1199 2024-01-17 21:37:10.961319 roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation_runtime_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     9326 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/action.py
+-rw-r--r--   0        0        0     3165 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/action_container_resources.py
+-rw-r--r--   0        0        0     3138 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/action_delegate.py
+-rw-r--r--   0        0        0     8201 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/action_http_delegate.py
+-rw-r--r--   0        0        0     2302 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/action_http_resources.py
+-rw-r--r--   0        0        0     5697 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/action_record.py
+-rw-r--r--   0        0        0     7657 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/invocation.py
+-rw-r--r--   0        0        0     2506 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     7117 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      827 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0     6240 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/invocation_record.py
+-rw-r--r--   0        0        0      990 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/actions/invocation_runtime_resources.py
+-rw-r--r--   0        0        0      827 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/collections/__init__.py
+-rw-r--r--   0        0        0      906 2024-01-17 21:37:10.965319 roboto-0.2.9/src/roboto/domain/collections/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3937 2024-01-17 21:37:10.965319 roboto-0.2.9/src/roboto/domain/collections/__pycache__/collection.cpython-310.pyc
+-rw-r--r--   0        0        0     2915 2024-01-17 21:37:10.965319 roboto-0.2.9/src/roboto/domain/collections/__pycache__/collection_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5732 2024-01-17 21:37:10.977319 roboto-0.2.9/src/roboto/domain/collections/__pycache__/collection_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1475 2024-01-17 21:37:10.981319 roboto-0.2.9/src/roboto/domain/collections/__pycache__/collection_http_resource.cpython-310.pyc
+-rw-r--r--   0        0        0     2508 2024-01-17 21:37:10.965319 roboto-0.2.9/src/roboto/domain/collections/__pycache__/collection_record.cpython-310.pyc
+-rw-r--r--   0        0        0     4861 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/collections/collection.py
+-rw-r--r--   0        0        0     2679 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/collections/collection_delegate.py
+-rw-r--r--   0        0        0     6721 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/collections/collection_http_delegate.py
+-rw-r--r--   0        0        0      971 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/collections/collection_http_resource.py
+-rw-r--r--   0        0        0     1697 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/collections/collection_record.py
+-rw-r--r--   0        0        0      468 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/comments/__init__.py
+-rw-r--r--   0        0        0      676 2024-01-17 21:37:10.985319 roboto-0.2.9/src/roboto/domain/comments/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3612 2024-01-17 21:37:10.985319 roboto-0.2.9/src/roboto/domain/comments/__pycache__/comment.cpython-310.pyc
+-rw-r--r--   0        0        0     2418 2024-01-17 21:37:10.985319 roboto-0.2.9/src/roboto/domain/comments/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     4548 2024-01-17 21:37:10.993319 roboto-0.2.9/src/roboto/domain/comments/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      853 2024-01-17 21:37:10.993319 roboto-0.2.9/src/roboto/domain/comments/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1172 2024-01-17 21:37:10.989319 roboto-0.2.9/src/roboto/domain/comments/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     3549 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/comments/comment.py
+-rw-r--r--   0        0        0     1964 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/comments/delegate.py
+-rw-r--r--   0        0        0     5153 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/comments/http_delegate.py
+-rw-r--r--   0        0        0      239 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/comments/http_resources.py
+-rw-r--r--   0        0        0      776 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/comments/record.py
+-rw-r--r--   0        0        0      678 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/datasets/__init__.py
+-rw-r--r--   0        0        0      813 2024-01-17 21:37:10.993319 roboto-0.2.9/src/roboto/domain/datasets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    17652 2024-01-17 21:37:10.997319 roboto-0.2.9/src/roboto/domain/datasets/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     4179 2024-01-17 21:37:11.081319 roboto-0.2.9/src/roboto/domain/datasets/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     7197 2024-01-17 21:37:11.089319 roboto-0.2.9/src/roboto/domain/datasets/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1912 2024-01-17 21:37:11.089319 roboto-0.2.9/src/roboto/domain/datasets/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1367 2024-01-17 21:37:11.081319 roboto-0.2.9/src/roboto/domain/datasets/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0    22456 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/datasets/dataset.py
+-rw-r--r--   0        0        0     3350 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/datasets/delegate.py
+-rw-r--r--   0        0        0     7796 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/datasets/http_delegate.py
+-rw-r--r--   0        0        0     1089 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/datasets/http_resources.py
+-rw-r--r--   0        0        0     1239 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/datasets/record.py
+-rw-r--r--   0        0        0      943 2024-01-17 21:35:46.701574 roboto-0.2.9/src/roboto/domain/files/__init__.py
+-rw-r--r--   0        0        0     1027 2024-01-17 21:37:11.009319 roboto-0.2.9/src/roboto/domain/files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    10478 2024-01-17 21:37:11.009319 roboto-0.2.9/src/roboto/domain/files/__pycache__/client_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     3675 2024-01-17 21:37:11.053319 roboto-0.2.9/src/roboto/domain/files/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     4493 2024-01-17 21:37:11.077319 roboto-0.2.9/src/roboto/domain/files/__pycache__/file.cpython-310.pyc
+-rw-r--r--   0        0        0     1322 2024-01-17 21:37:11.077319 roboto-0.2.9/src/roboto/domain/files/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     6512 2024-01-17 21:37:11.053319 roboto-0.2.9/src/roboto/domain/files/__pycache__/progress.cpython-310.pyc
+-rw-r--r--   0        0        0     1230 2024-01-17 21:37:11.069319 roboto-0.2.9/src/roboto/domain/files/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0    13226 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/files/client_delegate.py
+-rw-r--r--   0        0        0     3250 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/files/delegate.py
+-rw-r--r--   0        0        0     3864 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/files/file.py
+-rw-r--r--   0        0        0      500 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/files/http_resources.py
+-rw-r--r--   0        0        0     4606 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/files/progress.py
+-rw-r--r--   0        0        0      921 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/files/record.py
+-rw-r--r--   0        0        0     2677 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/http_delegates.py
+-rw-r--r--   0        0        0      902 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/orgs/__init__.py
+-rw-r--r--   0        0        0     1002 2024-01-17 21:37:11.097319 roboto-0.2.9/src/roboto/domain/orgs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4329 2024-01-17 21:37:11.097319 roboto-0.2.9/src/roboto/domain/orgs/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     8391 2024-01-17 21:37:11.117319 roboto-0.2.9/src/roboto/domain/orgs/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1757 2024-01-17 21:37:11.117319 roboto-0.2.9/src/roboto/domain/orgs/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     4929 2024-01-17 21:37:11.125319 roboto-0.2.9/src/roboto/domain/orgs/__pycache__/org.cpython-310.pyc
+-rw-r--r--   0        0        0     3310 2024-01-17 21:37:11.125319 roboto-0.2.9/src/roboto/domain/orgs/__pycache__/org_invite.cpython-310.pyc
+-rw-r--r--   0        0        0     2913 2024-01-17 21:37:11.125319 roboto-0.2.9/src/roboto/domain/orgs/__pycache__/org_role.cpython-310.pyc
+-rw-r--r--   0        0        0     1750 2024-01-17 21:37:11.097319 roboto-0.2.9/src/roboto/domain/orgs/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     3589 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     8997 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      740 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     4075 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/orgs/org.py
+-rw-r--r--   0        0        0     2413 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/orgs/org_invite.py
+-rw-r--r--   0        0        0     1921 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      775 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/orgs/record.py
+-rw-r--r--   0        0        0      452 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      669 2024-01-17 21:37:11.125319 roboto-0.2.9/src/roboto/domain/tokens/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1453 2024-01-17 21:37:11.125319 roboto-0.2.9/src/roboto/domain/tokens/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     2967 2024-01-17 21:37:11.129319 roboto-0.2.9/src/roboto/domain/tokens/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      858 2024-01-17 21:37:11.129319 roboto-0.2.9/src/roboto/domain/tokens/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0      995 2024-01-17 21:37:11.125319 roboto-0.2.9/src/roboto/domain/tokens/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     2877 2024-01-17 21:37:11.133319 roboto-0.2.9/src/roboto/domain/tokens/__pycache__/token.cpython-310.pyc
+-rw-r--r--   0        0        0      857 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     2226 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      283 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      455 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/tokens/record.py
+-rw-r--r--   0        0        0     2128 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/tokens/token.py
+-rw-r--r--   0        0        0      936 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/topics/__init__.py
+-rw-r--r--   0        0        0     3615 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/topics/topic.py
+-rw-r--r--   0        0        0     2588 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/topics/topic_delegate.py
+-rw-r--r--   0        0        0     9533 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/topics/topic_http_delegate.py
+-rw-r--r--   0        0        0     6838 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/topics/topic_record.py
+-rw-r--r--   0        0        0     2406 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/topics/topic_requests.py
+-rw-r--r--   0        0        0      761 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/triggers/__init__.py
+-rw-r--r--   0        0        0      864 2024-01-17 21:37:11.133319 roboto-0.2.9/src/roboto/domain/triggers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5341 2024-01-17 21:37:11.133319 roboto-0.2.9/src/roboto/domain/triggers/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     4468 2024-01-17 21:37:11.137319 roboto-0.2.9/src/roboto/domain/triggers/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     7954 2024-01-17 21:37:11.161319 roboto-0.2.9/src/roboto/domain/triggers/__pycache__/trigger.cpython-310.pyc
+-rw-r--r--   0        0        0     2857 2024-01-17 21:37:11.157319 roboto-0.2.9/src/roboto/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     2105 2024-01-17 21:37:11.137319 roboto-0.2.9/src/roboto/domain/triggers/__pycache__/trigger_record.cpython-310.pyc
+-rw-r--r--   0        0        0     6389 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0     4073 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0    10159 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/triggers/trigger.py
+-rw-r--r--   0        0        0     2837 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0     1667 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      357 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/users/__init__.py
+-rw-r--r--   0        0        0      612 2024-01-17 21:37:11.101319 roboto-0.2.9/src/roboto/domain/users/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2587 2024-01-17 21:37:11.101319 roboto-0.2.9/src/roboto/domain/users/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     2864 2024-01-17 21:37:11.109319 roboto-0.2.9/src/roboto/domain/users/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1458 2024-01-17 21:37:11.101319 roboto-0.2.9/src/roboto/domain/users/__pycache__/user_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      899 2024-01-17 21:37:11.105319 roboto-0.2.9/src/roboto/domain/users/__pycache__/user_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1393 2024-01-17 21:37:11.101319 roboto-0.2.9/src/roboto/domain/users/__pycache__/user_record.cpython-310.pyc
+-rw-r--r--   0        0        0     2308 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     2271 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/users/user.py
+-rw-r--r--   0        0        0      935 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      456 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/users/user_http_resources.py
+-rw-r--r--   0        0        0      886 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/domain/users/user_record.py
+-rw-r--r--   0        0        0     1101 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/exceptions/__init__.py
+-rw-r--r--   0        0        0     1052 2024-01-17 21:37:10.537320 roboto-0.2.9/src/roboto/exceptions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    10221 2024-01-17 21:37:10.537320 roboto-0.2.9/src/roboto/exceptions/__pycache__/domain.cpython-310.pyc
+-rw-r--r--   0        0        0     2278 2024-01-17 21:37:10.541320 roboto-0.2.9/src/roboto/exceptions/__pycache__/http.cpython-310.pyc
+-rw-r--r--   0        0        0     8433 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/exceptions/domain.py
+-rw-r--r--   0        0        0     1334 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/exceptions/http.py
+-rw-r--r--   0        0        0     1316 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/http/__init__.py
+-rw-r--r--   0        0        0     1260 2024-01-17 21:37:10.493321 roboto-0.2.9/src/roboto/http/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      646 2024-01-17 21:37:10.493321 roboto-0.2.9/src/roboto/http/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0      874 2024-01-17 21:37:10.493321 roboto-0.2.9/src/roboto/http/__pycache__/headers.cpython-310.pyc
+-rw-r--r--   0        0        0     9856 2024-01-17 21:37:10.497321 roboto-0.2.9/src/roboto/http/__pycache__/http_client.cpython-310.pyc
+-rw-r--r--   0        0        0     3977 2024-01-17 21:37:10.541320 roboto-0.2.9/src/roboto/http/__pycache__/request_decorators.cpython-310.pyc
+-rw-r--r--   0        0        0     6728 2024-01-17 21:37:10.885319 roboto-0.2.9/src/roboto/http/__pycache__/response.cpython-310.pyc
+-rw-r--r--   0        0        0     2489 2024-01-17 21:37:10.897319 roboto-0.2.9/src/roboto/http/__pycache__/testing_util.cpython-310.pyc
+-rw-r--r--   0        0        0      834 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/http/constants.py
+-rw-r--r--   0        0        0      766 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/http/headers.py
+-rw-r--r--   0        0        0    10931 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/http/http_client.py
+-rw-r--r--   0        0        0     3177 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/http/request_decorators.py
+-rw-r--r--   0        0        0     5809 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/http/response.py
+-rw-r--r--   0        0        0     1819 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/http/testing_util.py
+-rw-r--r--   0        0        0      951 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/image_registry/__init__.py
+-rw-r--r--   0        0        0      967 2024-01-17 21:37:11.205319 roboto-0.2.9/src/roboto/image_registry/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2024-01-17 21:37:11.205319 roboto-0.2.9/src/roboto/image_registry/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     8394 2024-01-17 21:37:11.209318 roboto-0.2.9/src/roboto/image_registry/__pycache__/image_registry.cpython-310.pyc
+-rw-r--r--   0        0        0      800 2024-01-17 21:37:11.209318 roboto-0.2.9/src/roboto/image_registry/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0      913 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/image_registry/http_resources.py
+-rw-r--r--   0        0        0     9136 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/image_registry/image_registry.py
+-rw-r--r--   0        0        0      283 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/image_registry/record.py
+-rw-r--r--   0        0        0      154 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/logging.py
+-rw-r--r--   0        0        0      201 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/notifications/__init__.py
+-rw-r--r--   0        0        0      498 2024-01-17 21:37:11.101319 roboto-0.2.9/src/roboto/notifications/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2282 2024-01-17 21:37:11.101319 roboto-0.2.9/src/roboto/notifications/__pycache__/http_client.cpython-310.pyc
+-rw-r--r--   0        0        0      721 2024-01-17 21:37:11.101319 roboto-0.2.9/src/roboto/notifications/__pycache__/notifications.cpython-310.pyc
+-rw-r--r--   0        0        0     1929 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/notifications/http_client.py
+-rw-r--r--   0        0        0      444 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/notifications/notifications.py
+-rw-r--r--   0        0        0      303 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/profile/__init__.py
+-rw-r--r--   0        0        0      502 2024-01-17 21:37:10.881319 roboto-0.2.9/src/roboto/profile/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3828 2024-01-17 21:37:10.881319 roboto-0.2.9/src/roboto/profile/__pycache__/profile.cpython-310.pyc
+-rw-r--r--   0        0        0     3730 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/profile/profile.py
+-rw-r--r--   0        0        0        0 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/py.typed
+-rw-r--r--   0        0        0      238 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/pydantic/__init__.py
+-rw-r--r--   0        0        0      456 2024-01-17 21:37:10.905319 roboto-0.2.9/src/roboto/pydantic/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      804 2024-01-17 21:37:10.909319 roboto-0.2.9/src/roboto/pydantic/__pycache__/serializers.cpython-310.pyc
+-rw-r--r--   0        0        0     2441 2024-01-17 21:37:10.905319 roboto-0.2.9/src/roboto/pydantic/__pycache__/validators.cpython-310.pyc
+-rw-r--r--   0        0        0      524 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/pydantic/serializers.py
+-rw-r--r--   0        0        0     1869 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/pydantic/validators.py
+-rw-r--r--   0        0        0      543 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/query/__init__.py
+-rw-r--r--   0        0        0      728 2024-01-17 21:37:10.209321 roboto-0.2.9/src/roboto/query/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4550 2024-01-17 21:37:10.209321 roboto-0.2.9/src/roboto/query/__pycache__/conditions.cpython-310.pyc
+-rw-r--r--   0        0        0     1511 2024-01-17 21:37:10.409321 roboto-0.2.9/src/roboto/query/__pycache__/precanned.cpython-310.pyc
+-rw-r--r--   0        0        0     4438 2024-01-17 21:37:10.409321 roboto-0.2.9/src/roboto/query/__pycache__/query.cpython-310.pyc
+-rw-r--r--   0        0        0     1948 2024-01-17 21:37:10.413321 roboto-0.2.9/src/roboto/query/__pycache__/visitor.cpython-310.pyc
+-rw-r--r--   0        0        0     4516 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/query/conditions.py
+-rw-r--r--   0        0        0     1671 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/query/precanned.py
+-rw-r--r--   0        0        0     3861 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/query/query.py
+-rw-r--r--   0        0        0     1394 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/query/visitor.py
+-rw-r--r--   0        0        0     2449 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/sentinels.py
+-rw-r--r--   0        0        0      734 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/serde/__init__.py
+-rw-r--r--   0        0        0      873 2024-01-17 21:37:10.217321 roboto-0.2.9/src/roboto/serde/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      493 2024-01-17 21:37:10.217321 roboto-0.2.9/src/roboto/serde/__pycache__/arrays.cpython-310.pyc
+-rw-r--r--   0        0        0     2199 2024-01-17 21:37:10.217321 roboto-0.2.9/src/roboto/serde/__pycache__/dicts.cpython-310.pyc
+-rw-r--r--   0        0        0      901 2024-01-17 21:37:10.325321 roboto-0.2.9/src/roboto/serde/__pycache__/paths.cpython-310.pyc
+-rw-r--r--   0        0        0      158 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/serde/arrays.py
+-rw-r--r--   0        0        0     1713 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/serde/dicts.py
+-rw-r--r--   0        0        0      801 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/serde/paths.py
+-rw-r--r--   0        0        0      182 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/time.py
+-rw-r--r--   0        0        0      558 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/transactions/__init__.py
+-rw-r--r--   0        0        0      732 2024-01-17 21:37:10.997319 roboto-0.2.9/src/roboto/transactions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      947 2024-01-17 21:37:11.001319 roboto-0.2.9/src/roboto/transactions/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1550 2024-01-17 21:37:11.005319 roboto-0.2.9/src/roboto/transactions/__pycache__/manager_abc.cpython-310.pyc
+-rw-r--r--   0        0        0     1841 2024-01-17 21:37:11.001319 roboto-0.2.9/src/roboto/transactions/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     2983 2024-01-17 21:37:11.009319 roboto-0.2.9/src/roboto/transactions/__pycache__/transaction_manager.cpython-310.pyc
+-rw-r--r--   0        0        0      318 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/transactions/http_resources.py
+-rw-r--r--   0        0        0     1043 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/transactions/manager_abc.py
+-rw-r--r--   0        0        0     1099 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/transactions/record.py
+-rw-r--r--   0        0        0     3198 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/transactions/transaction_manager.py
+-rw-r--r--   0        0        0      225 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/types.py
+-rw-r--r--   0        0        0     7347 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/updates.py
+-rw-r--r--   0        0        0     1819 2024-01-17 21:35:46.705574 roboto-0.2.9/src/roboto/waiters.py
+-rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 roboto-0.2.9/PKG-INFO
```

### Comparing `roboto-0.2.8/pyproject.toml` & `roboto-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires-python = ">=3.9"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto"
-version = "0.2.8"
+version = "0.2.9"
 description = "Tools for interacting with roboto.ai"
 license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `roboto-0.2.8/src/roboto/association.py` & `roboto-0.2.9/src/roboto/association.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/auth/__pycache__/pat.cpython-310.pyc` & `roboto-0.2.9/src/roboto/auth/__pycache__/pat.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 4037 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 c50f 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 c50f 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6403  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 0100 6403 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6508 8300 5a0b 6401 5a0c  m.Z...e...Z.d.Z.
@@ -26,16 +26,16 @@
 00000190: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
 000001a0: 005a 0264 0153 0029 02da 1652 656a 6563  .Z.d.S.)...Rejec
 000001b0: 7465 6454 6f6b 656e 4578 6365 7074 696f  tedTokenExceptio
 000001c0: 6e4e 2903 da08 5f5f 6e61 6d65 5f5f da0a  nN)...__name__..
 000001d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 000001e0: 616c 6e61 6d65 5f5f a900 720b 0000 0072  alname__..r....r
 000001f0: 0b00 0000 fad8 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000200: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000210: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000200: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000210: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000220: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000230: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000240: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000250: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000260: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000270: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000280: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/auth/__pycache__/permissions.cpython-310.pyc` & `roboto-0.2.9/src/roboto/auth/__pycache__/permissions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 548 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 2402 0000  o........Y.e$...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 2402 0000  o.......2H.e$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 6401 5300 2904 e900  e.j...Z.d.S.)...
 00000050: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
 00000060: 0000 0000 0001 0000 0040 0000 0073 1800  .........@...s..
 00000070: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
@@ -38,15 +38,15 @@
 00000250: 2020 2020 da08 5265 6164 4f6e 6c79 da09      ..ReadOnly..
 00000260: 5265 6164 5772 6974 654e 2906 da08 5f5f  ReadWriteN)...__
 00000270: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 00000280: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 00000290: da07 5f5f 646f 635f 5f72 0300 0000 7204  ..__doc__r....r.
 000002a0: 0000 00a9 0072 0900 0000 7209 0000 00fa  .....r....r.....
 000002b0: e02f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000002c0: 7574 2f73 7263 3130 3531 3138 3230 3839  ut/src1051182089
+000002c0: 7574 2f73 7263 3330 3739 3233 3632 3634  ut/src3079236264
 000002d0: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 000002e0: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 000002f0: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000300: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000310: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000320: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000330: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto-0.2.8/src/roboto/auth/pat.py` & `roboto-0.2.9/src/roboto/auth/pat.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/auth/permissions.py` & `roboto-0.2.9/src/roboto/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/__pycache__/argparse.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/__pycache__/argparse.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1103 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4f04 0000  o........Y.eO...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 4f04 0000  o.......2H.eO...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000050: 8400 6404 6500 6a04 8303 5a05 4700 6405  ..d.e.j...Z.G.d.
 00000060: 6406 8400 6406 6500 6a06 8303 5a07 6401  d...d.e.j...Z.d.
 00000070: 5300 2907 e900 0000 004e 2901 da0a 6174  S.)......N)...at
@@ -30,15 +30,15 @@
 000001d0: 04da 0573 7570 6572 7203 0000 00da 085f  ...superr......_
 000001e0: 5f69 6e69 745f 5f72 0400 0000 2906 da04  _init__r....)...
 000001f0: 7365 6c66 da0e 6f70 7469 6f6e 5f73 7472  self..option_str
 00000200: 696e 6773 da04 6465 7374 7207 0000 0072  ings..destr....r
 00000210: 0500 0000 da06 6b77 6172 6773 a901 da09  ......kwargs....
 00000220: 5f5f 636c 6173 735f 5fa9 00fa dc2f 636f  __class__..../co
 00000230: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-00000240: 7263 3130 3531 3138 3230 3839 2f73 7263  rc1051182089/src
+00000240: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
 00000250: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
 00000260: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
 00000270: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
 00000280: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
 00000290: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
 000002a0: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
 000002b0: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
```

### Comparing `roboto-0.2.8/src/roboto/cli/__pycache__/config.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/__pycache__/config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2257 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 d108 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 d108 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a04 6400 6401 6c05  ..d.d.l.Z.d.d.l.
 00000050: 5a05 6400 6401 6c06 5a06 6400 6403 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 0100 6400 6401 6c09 5a09 6400  m.Z...d.d.l.Z.d.
 00000070: 6404 6c0a 6d0b 5a0b 0100 6400 6405 6c0c  d.l.m.Z...d.d.l.
@@ -30,15 +30,15 @@
 000001d0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 000001e0: 6d65 5f5f 720a 0000 0072 0300 0000 da08  me__r....r......
 000001f0: 6461 7465 7469 6d65 da0f 5f5f 616e 6e6f  datetime..__anno
 00000200: 7461 7469 6f6e 735f 5f72 0b00 0000 da03  tations__r......
 00000210: 7374 7272 0c00 0000 da04 626f 6f6c a900  strr......bool..
 00000220: 7214 0000 0072 1400 0000 fada 2f63 6f64  r....r....../cod
 00000230: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000240: 6331 3035 3131 3832 3038 392f 7372 632f  c1051182089/src/
+00000240: 6333 3037 3932 3336 3236 342f 7372 632f  c3079236264/src/
 00000250: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000260: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000270: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000280: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 00000290: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 000002a0: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 000002b0: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto-0.2.8/src/roboto/cli/__pycache__/context.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/__pycache__/context.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1700 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 a406 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 a406 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6402  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6402 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6402 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6402 6407 6c0c 6d0d 5a0d 0100 6402  ..d.d.l.m.Z...d.
@@ -58,15 +58,15 @@
 00000390: 0075 0072 0974 0164 0183 0182 017c 006a  .u.r.t.d.....|.j
 000003a0: 0053 0029 024e 7a20 726f 626f 746f 5f73  .S.).Nz roboto_s
 000003b0: 6572 7669 6365 5f62 6173 655f 7572 6c20  ervice_base_url 
 000003c0: 6973 2075 6e73 6574 2902 7211 0000 00da  is unset).r.....
 000003d0: 0a56 616c 7565 4572 726f 72a9 01da 0473  .ValueError....s
 000003e0: 656c 66a9 0072 2300 0000 fadb 2f63 6f64  elf..r#...../cod
 000003f0: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000400: 6331 3035 3131 3832 3038 392f 7372 632f  c1051182089/src/
+00000400: 6333 3037 3932 3336 3236 342f 7372 632f  c3079236264/src/
 00000410: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000420: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000430: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000440: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 00000450: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000460: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 00000470: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto-0.2.8/src/roboto/cli/__pycache__/entry.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/__pycache__/entry.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 8248 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 3820 0000  o........Y.e8 ..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 3820 0000  o.......2H.e8 ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 d201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6401 6c05 5a05 6400 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 6d08 5a08 0100 6404 6405 6c09  m.Z.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 0100 6404 6406 6c0c  m.Z.m.Z...d.d.l.
@@ -120,15 +120,15 @@
 00000770: 00da 0575 7365 7273 720c 0000 00da 0674  ...usersr......t
 00000780: 6f6b 656e 73da 0a65 7874 656e 7369 6f6e  okens..extension
 00000790: 7329 0572 1e00 0000 721f 0000 005a 0d70  s).r....r....Z.p
 000007a0: 726f 6669 6c65 5f65 6e74 7279 5a10 6874  rofile_entryZ.ht
 000007b0: 7470 5f63 6c69 656e 745f 6172 6773 7226  tp_client_argsr&
 000007c0: 0000 0072 2400 0000 7224 0000 00fa d92f  ...r$...r$...../
 000007d0: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-000007e0: 2f73 7263 3130 3531 3138 3230 3839 2f73  /src1051182089/s
+000007e0: 2f73 7263 3330 3739 3233 3632 3634 2f73  /src3079236264/s
 000007f0: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000800: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000810: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000820: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000830: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000840: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000850: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto-0.2.8/src/roboto/cli/__pycache__/terminal.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/__pycache__/terminal.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 490 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 ea01 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 ea01 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000050: 6503 6500 6a04 8304 5a05 6404 6502 6a06  e.e.j...Z.d.e.j.
 00000060: 6503 6507 6503 1900 6602 1900 6405 6502  e.e.e...f...d.e.
 00000070: 6a08 6604 6406 6407 8404 5a09 6401 5300  j.f.d.d...Z.d.S.
@@ -15,15 +15,15 @@
 000000e0: 6d7a 071b 5b30 3b33 346d 7a04 1b5b 306d  mz..[0;34mz..[0m
 000000f0: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
 00000100: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00000110: 6c6e 616d 655f 5fda 0352 4544 da05 4752  lname__..RED..GR
 00000120: 4545 4eda 0442 4c55 45da 0345 4e44 a900  EEN..BLUE..END..
 00000130: 720a 0000 0072 0a00 0000 fadc 2f63 6f64  r....r....../cod
 00000140: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000150: 6331 3035 3131 3832 3038 392f 7372 632f  c1051182089/src/
+00000150: 6333 3037 3932 3336 3236 342f 7372 632f  c3079236264/src/
 00000160: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000170: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000180: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000190: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 000001a0: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 000001b0: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 000001c0: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto-0.2.8/src/roboto/cli/__pycache__/validation.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/__pycache__/validation.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1162 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 8a04 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 8a04 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6500 6a05  ..G.d.d...d.e.j.
 00000060: 8303 5a06 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 1470 7269 6e74 5f65  .....)...print_e
@@ -28,16 +28,16 @@
 000001b0: 5f6e 616d 654e da0e 7061 7273 6561 626c  _nameN..parseabl
 000001c0: 655f 6e61 6d65 6302 0000 0000 0000 0000  e_namec.........
 000001d0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
 000001e0: 1600 0000 7c01 6400 7501 7209 7c01 7c00  ....|.d.u.r.|.|.
 000001f0: 5f00 6400 5300 6400 5300 a901 4e29 0172  _.d.S.d.S...N).r
 00000200: 0500 0000 2902 da04 7365 6c66 7206 0000  ....)...selfr...
 00000210: 00a9 0072 0900 0000 fade 2f63 6f64 6562  ...r....../codeb
-00000220: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-00000230: 3035 3131 3832 3038 392f 7372 632f 636f  051182089/src/co
+00000220: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+00000230: 3037 3932 3336 3236 342f 7372 632f 636f  079236264/src/co
 00000240: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 00000250: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000260: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000270: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000280: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000290: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 000002a0: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto-0.2.8/src/roboto/cli/actions/__pycache__/action_config.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/actions/__pycache__/action_config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1989 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 c507 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 c507 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6403 6404 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6502 6a06 8303 5a07  d.d...d.e.j...Z.
 00000070: 4700 6407 6408 8400 6408 6502 6a06 8303  G.d.d...d.e.j...
@@ -26,16 +26,16 @@
 00000190: 5f5f 7175 616c 6e61 6d65 5f5f da07 7061  __qualname__..pa
 000001a0: 7468 6c69 62da 0450 6174 68da 0363 7764  thlib..Path..cwd
 000001b0: 7206 0000 00da 0f5f 5f61 6e6e 6f74 6174  r......__annotat
 000001c0: 696f 6e73 5f5f 7207 0000 00da 0870 7964  ions__r......pyd
 000001d0: 616e 7469 63da 0546 6965 6c64 da04 6469  antic..Field..di
 000001e0: 6374 720a 0000 00da 0373 7472 a900 7216  ctr......str..r.
 000001f0: 0000 0072 1600 0000 fae9 2f63 6f64 6562  ...r....../codeb
-00000200: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-00000210: 3035 3131 3832 3038 392f 7372 632f 636f  051182089/src/co
+00000200: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+00000210: 3037 3932 3336 3236 342f 7372 632f 636f  079236264/src/co
 00000220: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 00000230: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000240: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000250: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000260: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000270: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000280: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto-0.2.8/src/roboto/cli/actions/__pycache__/commands.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/actions/__pycache__/commands.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 714 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 ca02 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 ca02 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6402 6405 6c06 6d07 5a07 0100 6402  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6402 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6402 6408 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -33,16 +33,16 @@
 00000200: 766f 6b65 7206 0000 005a 106c 6973 745f  voker....Z.list_
 00000210: 696e 766f 6361 7469 6f6e 7372 0700 0000  invocationsr....
 00000220: da06 7365 6172 6368 7208 0000 005a 0473  ..searchr....Z.s
 00000230: 686f 7772 0900 0000 da06 7570 6461 7465  howr......update
 00000240: 720a 0000 0072 0e00 0000 da0b 636f 6d6d  r....r......comm
 00000250: 616e 645f 7365 74a9 0072 1600 0000 7216  and_set..r....r.
 00000260: 0000 00fa e42f 636f 6465 6275 696c 642f  ...../codebuild/
-00000270: 6f75 7470 7574 2f73 7263 3130 3531 3138  output/src105118
-00000280: 3230 3839 2f73 7263 2f63 6f64 6573 7461  2089/src/codesta
+00000270: 6f75 7470 7574 2f73 7263 3330 3739 3233  output/src307923
+00000280: 3632 3634 2f73 7263 2f63 6f64 6573 7461  6264/src/codesta
 00000290: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 000002a0: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 000002b0: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 000002c0: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 000002d0: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 000002e0: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 000002f0: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto-0.2.8/src/roboto/cli/actions/__pycache__/create.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/actions/__pycache__/create.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 12384 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 6030 0000  o........Y.e`0..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 6030 0000  o.......2H.e`0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 1201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6402 6403 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6402 6404 6c08 6d09 5a09 0100 6402  ..d.d.l.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 0100 6406 6407 6c0c  d.l.m.Z...d.d.l.
@@ -89,16 +89,16 @@
 00000580: 696f 6eda 126d 6574 6164 6174 615f 6368  ion..metadata_ch
 00000590: 616e 6765 7365 7463 0100 0000 0000 0000  angesetc........
 000005a0: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
 000005b0: f312 0000 0068 007c 005d 057d 017c 016a  .....h.|.].}.|.j
 000005c0: 0092 0271 0253 00a9 00a9 01da 046e 616d  ...q.S.......nam
 000005d0: 65a9 02da 022e 30da 0570 6172 616d 721e  e.....0..paramr.
 000005e0: 0000 0072 1e00 0000 fae2 2f63 6f64 6562  ...r....../codeb
-000005f0: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-00000600: 3035 3131 3832 3038 392f 7372 632f 636f  051182089/src/co
+000005f0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+00000600: 3037 3932 3336 3236 342f 7372 632f 636f  079236264/src/co
 00000610: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 00000620: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000630: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000640: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000650: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000660: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000670: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto-0.2.8/src/roboto/cli/actions/__pycache__/delete.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/actions/__pycache__/delete.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 981 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 d503 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 d503 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6406 6c05 6d06 5a06 0100 6404 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6408 6500 6a09 6409 6508  m.Z...d.e.j.d.e.
 00000070: 640a 6500 6a0a 640b 6401 6608 640c 640d  d.e.j.d.d.f.d.d.
@@ -29,15 +29,15 @@
 000001c0: da09 6672 6f6d 5f6e 616d 65da 0661 6374  ..from_name..act
 000001d0: 696f 6eda 0761 6374 696f 6e73 da0b 696e  ion..actions..in
 000001e0: 766f 6361 7469 6f6e 73da 036f 7267 da06  vocations..org..
 000001f0: 6465 6c65 7465 da05 7072 696e 7429 0472  delete..print).r
 00000200: 0800 0000 7209 0000 0072 0a00 0000 7212  ....r....r....r.
 00000210: 0000 00a9 0072 1800 0000 fae2 2f63 6f64  .....r....../cod
 00000220: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000230: 6331 3035 3131 3832 3038 392f 7372 632f  c1051182089/src/
+00000230: 6333 3037 3932 3336 3236 342f 7372 632f  c3079236264/src/
 00000240: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000250: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000260: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000270: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 00000280: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000290: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 000002a0: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto-0.2.8/src/roboto/cli/actions/__pycache__/invoke.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/actions/__pycache__/invoke.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3643 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 3b0e 0000  o........Y.e;...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 3b0e 0000  o.......2H.e;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 aa00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6404 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6404 6406 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
@@ -75,15 +75,15 @@
 000004a0: 616c 7565 7221 0000 00da 0570 7269 6e74  aluer!.....print
 000004b0: da06 7265 636f 7264 da09 7265 6665 7265  ..record..refere
 000004c0: 6e63 65da 0269 6429 0772 1000 0000 7211  nce..id).r....r.
 000004d0: 0000 0072 1200 0000 7224 0000 0072 2900  ...r....r$...r).
 000004e0: 0000 722a 0000 00da 0a69 6e76 6f63 6174  ..r*.....invocat
 000004f0: 696f 6ea9 0072 3400 0000 fae2 2f63 6f64  ion..r4...../cod
 00000500: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000510: 6331 3035 3131 3832 3038 392f 7372 632f  c1051182089/src/
+00000510: 6333 3037 3932 3336 3236 342f 7372 632f  c3079236264/src/
 00000520: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000530: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000540: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000550: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 00000560: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000570: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 00000580: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto-0.2.8/src/roboto/cli/actions/__pycache__/list_invocations.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/actions/__pycache__/list_invocations.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2614 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 360a 0000  o........Y.e6...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 360a 0000  o.......2H.e6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6404 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6405 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -41,15 +41,15 @@
 00000280: 6162 6c65 2909 da0a 6973 696e 7374 616e  able)...isinstan
 00000290: 6365 7203 0000 00da 0269 6472 1400 0000  cer......idr....
 000002a0: da09 6973 6f66 6f72 6d61 74da 0373 7472  ..isoformat..str
 000002b0: da0e 6375 7272 656e 745f 7374 6174 7573  ..current_status
 000002c0: da09 5479 7065 4572 726f 72da 0474 7970  ..TypeError..typ
 000002d0: 6529 0172 1100 0000 a900 721d 0000 00fa  e).r......r.....
 000002e0: ec2f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000002f0: 7574 2f73 7263 3130 3531 3138 3230 3839  ut/src1051182089
+000002f0: 7574 2f73 7263 3330 3739 3233 3632 3634  ut/src3079236264
 00000300: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 00000310: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000320: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000330: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000340: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000350: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000360: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto-0.2.8/src/roboto/cli/actions/__pycache__/search.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/actions/__pycache__/search.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3366 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 260d 0000  o........Y.e&...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 260d 0000  o.......2H.e&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6402 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6405 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -60,15 +60,15 @@
 000003b0: 675f 6964 6301 0000 0000 0000 0000 0000  g_idc...........
 000003c0: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
 000003d0: 0000 6700 7c00 5d06 7d01 7c01 a000 a100  ..g.|.].}.|.....
 000003e0: 9102 7102 5300 a900 2901 da07 746f 5f64  ..q.S...)...to_d
 000003f0: 6963 7429 02da 022e 30da 0661 6374 696f  ict)....0..actio
 00000400: 6e72 2200 0000 7222 0000 00fa e22f 636f  nr"...r"...../co
 00000410: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-00000420: 7263 3130 3531 3138 3230 3839 2f73 7263  rc1051182089/src
+00000420: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
 00000430: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
 00000440: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
 00000450: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
 00000460: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
 00000470: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
 00000480: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
 00000490: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
```

### Comparing `roboto-0.2.8/src/roboto/cli/actions/__pycache__/show.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/actions/__pycache__/show.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 941 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 ad03 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 ad03 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 6404 6405 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6404 6406 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6404 6407 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6408 6500 6a0b 6409 650a 640a 6500  ..d.e.j.d.e.d.e.
@@ -35,15 +35,15 @@
 00000220: 696f 6e73 da0b 696e 766f 6361 7469 6f6e  ions..invocation
 00000230: 73da 036f 7267 7212 0000 00da 056f 776e  s..orgr......own
 00000240: 6572 da05 7072 696e 74da 046a 736f 6eda  er..print..json.
 00000250: 0564 756d 7073 da07 746f 5f64 6963 7429  .dumps..to_dict)
 00000260: 0472 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
 00000270: 7217 0000 00a9 0072 2000 0000 fae0 2f63  r......r ...../c
 00000280: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000290: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+00000290: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 000002a0: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 000002b0: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 000002c0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 000002d0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 000002e0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 000002f0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 00000300: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/cli/actions/__pycache__/update.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/actions/__pycache__/update.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 6375 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 e718 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 e718 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6404 6c05 6d06 5a06 0100 6402  ..d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6406 6407 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 0100 6406 6408 6c0c  m.Z.m.Z...d.d.l.
@@ -116,16 +116,16 @@
 00000730: 696e 7472 1600 0000 da04 6a73 6f6e da05  intr......json..
 00000740: 6475 6d70 73da 0774 6f5f 6469 6374 290a  dumps..to_dict).
 00000750: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
 00000760: 2c00 0000 da07 7570 6461 7465 73da 0873  ,.....updates..s
 00000770: 7472 6970 7065 6472 1f00 0000 7224 0000  trippedr....r$..
 00000780: 0072 2500 0000 7226 0000 0072 2900 0000  .r%...r&...r)...
 00000790: 7229 0000 00fa e22f 636f 6465 6275 696c  r)...../codebuil
-000007a0: 642f 6f75 7470 7574 2f73 7263 3130 3531  d/output/src1051
-000007b0: 3138 3230 3839 2f73 7263 2f63 6f64 6573  182089/src/codes
+000007a0: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+000007b0: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
 000007c0: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 000007d0: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 000007e0: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 000007f0: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 00000800: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 00000810: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 00000820: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto-0.2.8/src/roboto/cli/actions/action_config.py` & `roboto-0.2.9/src/roboto/cli/actions/action_config.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/actions/commands.py` & `roboto-0.2.9/src/roboto/cli/actions/commands.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/actions/create.py` & `roboto-0.2.9/src/roboto/cli/actions/create.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/actions/delete.py` & `roboto-0.2.9/src/roboto/cli/actions/delete.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/actions/invoke.py` & `roboto-0.2.9/src/roboto/cli/actions/invoke.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/actions/list_invocations.py` & `roboto-0.2.9/src/roboto/cli/actions/list_invocations.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/actions/search.py` & `roboto-0.2.9/src/roboto/cli/actions/search.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/actions/show.py` & `roboto-0.2.9/src/roboto/cli/actions/show.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/actions/update.py` & `roboto-0.2.9/src/roboto/cli/actions/update.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/argparse.py` & `roboto-0.2.9/src/roboto/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/collections/__init__.py` & `roboto-0.2.9/src/roboto/cli/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/collections/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/datasets/__pycache__/commands.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 579 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,67 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4302 0000  o........Y.eC...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 7203 0000  o.......2H.er...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
+00000020: 0009 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6402 6405 6c06 6d07 5a07 0100 6402  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6402 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6402 6408 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
-00000080: 0100 6501 6409 640a 6503 6505 6507 6509  ..e.d.d.e.e.e.e.
-00000090: 650b 650d 6706 640b 8d03 5a0e 640c 5300  e.e.g.d...Z.d.S.
-000000a0: 290d e902 0000 0029 01da 1052 6f62 6f74  )......)...Robot
-000000b0: 6f43 6f6d 6d61 6e64 5365 74e9 0100 0000  oCommandSet.....
-000000c0: 2901 da0f 6368 616e 6765 735f 636f 6d6d  )...changes_comm
-000000d0: 616e 6429 01da 0e63 7265 6174 655f 636f  and)...create_co
-000000e0: 6d6d 616e 6429 01da 0e64 656c 6574 655f  mmand)...delete_
-000000f0: 636f 6d6d 616e 6429 01da 0c6c 6973 745f  command)...list_
-00000100: 636f 6d6d 616e 6429 01da 0c73 686f 775f  command)...show_
-00000110: 636f 6d6d 616e 6429 01da 0e75 7064 6174  command)...updat
-00000120: 655f 636f 6d6d 616e 64da 0b63 6f6c 6c65  e_command..colle
-00000130: 6374 696f 6e73 7a34 4375 7261 7465 2063  ctionsz4Curate c
-00000140: 6f6c 6c65 6374 696f 6e73 206f 6620 6461  ollections of da
-00000150: 7461 7365 7473 2061 6e64 206f 7468 6572  tasets and other
-00000160: 2064 6174 6120 7479 7065 732e 2903 da04   data types.)...
-00000170: 6e61 6d65 da04 6865 6c70 da08 636f 6d6d  name..help..comm
-00000180: 616e 6473 4e29 0fda 0763 6f6d 6d61 6e64  andsN)...command
-00000190: 7202 0000 00da 0763 6861 6e67 6573 7204  r......changesr.
-000001a0: 0000 00da 0663 7265 6174 6572 0500 0000  .....creater....
-000001b0: da06 6465 6c65 7465 7206 0000 00da 046c  ..deleter......l
-000001c0: 6973 7472 0700 0000 da04 7368 6f77 7208  istr......showr.
-000001d0: 0000 00da 0675 7064 6174 6572 0900 0000  .....updater....
-000001e0: da0b 636f 6d6d 616e 645f 7365 74a9 0072  ..command_set..r
-000001f0: 1600 0000 7216 0000 00fa e82f 636f 6465  ....r....../code
-00000200: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000210: 3130 3531 3138 3230 3839 2f73 7263 2f63  1051182089/src/c
-00000220: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
-00000230: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
-00000240: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
-00000250: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
-00000260: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
-00000270: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
-00000280: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
-00000290: 2f72 6f62 6f74 6f2d 6169 2f72 6f62 6f74  /roboto-ai/robot
-000002a0: 6f2d 686f 7374 6564 2d61 7070 2f70 6163  o-hosted-app/pac
-000002b0: 6b61 6765 732f 726f 626f 746f 2f73 7263  kages/roboto/src
-000002c0: 2f72 6f62 6f74 6f2f 636c 692f 636f 6c6c  /roboto/cli/coll
-000002d0: 6563 7469 6f6e 732f 5f5f 696e 6974 5f5f  ections/__init__
-000002e0: 2e70 79da 083c 6d6f 6475 6c65 3e01 0000  .py..<module>...
-000002f0: 0073 2400 0000 0c02 0c01 0c01 0c01 0c01  .s$.............
-00000300: 0c01 0c01 0202 0201 0201 0202 0201 0201  ................
-00000310: 0201 0201 0201 02fa 0afd                 ..........
+00000080: 0100 6402 6409 6c0e 6d0f 5a0f 0100 6402  ..d.d.l.m.Z...d.
+00000090: 640a 6c10 6d11 5a11 0100 6402 640b 6c12  d.l.m.Z...d.d.l.
+000000a0: 6d13 5a13 0100 6503 6505 6507 6509 650b  m.Z...e.e.e.e.e.
+000000b0: 650f 650d 6511 6513 6709 5a14 6501 640c  e.e.e.e.g.Z.e.d.
+000000c0: 640d 6514 640e 8d03 5a15 640f 5300 2910  d.e.d...Z.d.S.).
+000000d0: e902 0000 0029 01da 1052 6f62 6f74 6f43  .....)...RobotoC
+000000e0: 6f6d 6d61 6e64 5365 74e9 0100 0000 2901  ommandSet.....).
+000000f0: da0e 6372 6561 7465 5f63 6f6d 6d61 6e64  ..create_command
+00000100: 2901 da16 6465 6c65 7465 5f64 6174 6173  )...delete_datas
+00000110: 6574 5f63 6f6d 6d61 6e64 2901 da14 6465  et_command)...de
+00000120: 6c65 7465 5f66 696c 6573 5f63 6f6d 6d61  lete_files_comma
+00000130: 6e64 2901 da16 646f 776e 6c6f 6164 5f66  nd)...download_f
+00000140: 696c 6573 5f63 6f6d 6d61 6e64 2901 da12  iles_command)...
+00000150: 6c69 7374 5f66 696c 6573 5f63 6f6d 6d61  list_files_comma
+00000160: 6e64 2901 da0e 7365 6172 6368 5f63 6f6d  nd)...search_com
+00000170: 6d61 6e64 2901 da0c 7368 6f77 5f63 6f6d  mand)...show_com
+00000180: 6d61 6e64 2901 da0e 7570 6461 7465 5f63  mand)...update_c
+00000190: 6f6d 6d61 6e64 2901 da14 7570 6c6f 6164  ommand)...upload
+000001a0: 5f66 696c 6573 5f63 6f6d 6d61 6e64 da08  _files_command..
+000001b0: 6461 7461 7365 7473 7a65 4d61 6e61 6765  datasetszeManage
+000001c0: 2064 6174 6120 6672 6f6d 2061 2073 696e   data from a sin
+000001d0: 676c 6520 6576 656e 742c 2073 7563 6820  gle event, such 
+000001e0: 6120 726f 626f 7420 7275 6e20 6f72 2064  a robot run or d
+000001f0: 726f 6e65 2066 6c69 6768 742e 2049 6e63  rone flight. Inc
+00000200: 6c75 6465 7320 6669 6c65 2075 706c 6f61  ludes file uploa
+00000210: 6420 616e 6420 646f 776e 6c6f 6164 2e29  d and download.)
+00000220: 03da 046e 616d 65da 0468 656c 70da 0863  ...name..help..c
+00000230: 6f6d 6d61 6e64 734e 2916 da07 636f 6d6d  ommandsN)...comm
+00000240: 616e 6472 0200 0000 da06 6372 6561 7465  andr......create
+00000250: 7204 0000 00da 0e64 656c 6574 655f 6461  r......delete_da
+00000260: 7461 7365 7472 0500 0000 da0c 6465 6c65  tasetr......dele
+00000270: 7465 5f66 696c 6573 7206 0000 00da 0e64  te_filesr......d
+00000280: 6f77 6e6c 6f61 645f 6669 6c65 7372 0700  ownload_filesr..
+00000290: 0000 da0a 6c69 7374 5f66 696c 6573 7208  ....list_filesr.
+000002a0: 0000 00da 0673 6561 7263 6872 0900 0000  .....searchr....
+000002b0: da04 7368 6f77 720a 0000 00da 0675 7064  ..showr......upd
+000002c0: 6174 6572 0b00 0000 da0c 7570 6c6f 6164  ater......upload
+000002d0: 5f66 696c 6573 720c 0000 0072 1000 0000  _filesr....r....
+000002e0: da0b 636f 6d6d 616e 645f 7365 74a9 0072  ..command_set..r
+000002f0: 1c00 0000 721c 0000 00fa e52f 636f 6465  ....r....../code
+00000300: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
+00000310: 3330 3739 3233 3632 3634 2f73 7263 2f63  3079236264/src/c
+00000320: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
+00000330: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
+00000340: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
+00000350: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
+00000360: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
+00000370: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
+00000380: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
+00000390: 2f72 6f62 6f74 6f2d 6169 2f72 6f62 6f74  /roboto-ai/robot
+000003a0: 6f2d 686f 7374 6564 2d61 7070 2f70 6163  o-hosted-app/pac
+000003b0: 6b61 6765 732f 726f 626f 746f 2f73 7263  kages/roboto/src
+000003c0: 2f72 6f62 6f74 6f2f 636c 692f 6461 7461  /roboto/cli/data
+000003d0: 7365 7473 2f63 6f6d 6d61 6e64 732e 7079  sets/commands.py
+000003e0: da08 3c6d 6f64 756c 653e 0100 0000 7332  ..<module>....s2
+000003f0: 0000 000c 020c 010c 010c 010c 010c 010c  ................
+00000400: 010c 010c 010c 0102 0302 0102 0102 0102  ................
+00000410: 0102 0102 0102 0102 0104 f702 0c02 0102  ................
+00000420: 0102 010a fd                             .....
```

### Comparing `roboto-0.2.8/src/roboto/cli/collections/__pycache__/changes.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/collections/__pycache__/changes.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1388 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 6c05 0000  o........Y.el...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 6c05 0000  o.......2H.el...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6406 6c05 6d06 5a06 0100 6404 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6408 6409 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 640a 6508 640b 6500 6a0b 6604 640c  ..d.e.d.e.j.f.d.
@@ -30,16 +30,16 @@
 000001d0: 0000 00da 036f 7267 da0b 636f 6c6c 6563  .....org..collec
 000001e0: 7469 6f6e 73da 0763 6861 6e67 6573 720f  tions..changesr.
 000001f0: 0000 0072 1000 0000 da05 7072 696e 74da  ...r......print.
 00000200: 046a 736f 6e29 05da 0461 7267 7372 0a00  .json)...argsr..
 00000210: 0000 720b 0000 00da 0a63 6f6c 6c65 6374  ..r......collect
 00000220: 696f 6e5a 0663 6861 6e67 65a9 0072 1900  ionZ.change..r..
 00000230: 0000 fae7 2f63 6f64 6562 7569 6c64 2f6f  ..../codebuild/o
-00000240: 7574 7075 742f 7372 6331 3035 3131 3832  utput/src1051182
-00000250: 3038 392f 7372 632f 636f 6465 7374 6172  089/src/codestar
+00000240: 7574 7075 742f 7372 6333 3037 3932 3336  utput/src3079236
+00000250: 3236 342f 7372 632f 636f 6465 7374 6172  264/src/codestar
 00000260: 2d63 6f6e 6e65 6374 696f 6e73 2e75 732d  -connections.us-
 00000270: 7765 7374 2d32 2e61 6d61 7a6f 6e61 7773  west-2.amazonaws
 00000280: 2e63 6f6d 2f67 6974 2d68 7474 702f 3036  .com/git-http/06
 00000290: 3631 3935 3131 3233 3835 2f75 732d 7765  6195112385/us-we
 000002a0: 7374 2d32 2f65 3635 3032 6138 302d 6262  st-2/e6502a80-bb
 000002b0: 3465 2d34 6662 652d 3837 3263 2d35 6434  4e-4fbe-872c-5d4
 000002c0: 3263 3139 3336 3939 642f 726f 626f 746f  2c193699d/roboto
```

### Comparing `roboto-0.2.8/src/roboto/cli/collections/__pycache__/create.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/collections/__pycache__/create.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2276 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 e408 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 e408 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6404 6405 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6407 6c09 6d0a 5a0a 0100 6408  ..d.d.l.m.Z...d.
 00000070: 650a 6409 6500 6a0b 6604 640a 640b 8404  e.d.e.j.f.d.d...
@@ -33,15 +33,15 @@
 00000200: 016a 027c 0164 008d 0291 0271 0253 00a9  .j.|.d.....q.S..
 00000210: 0129 02da 0d72 6573 6f75 7263 655f 7479  .)...resource_ty
 00000220: 7065 da0b 7265 736f 7572 6365 5f69 6429  pe..resource_id)
 00000230: 0372 0400 0000 7205 0000 00da 0744 6174  .r....r......Dat
 00000240: 6173 6574 2902 da02 2e30 da0a 6461 7461  aset)....0..data
 00000250: 7365 745f 6964 a900 7213 0000 00fa e62f  set_id..r....../
 00000260: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000270: 2f73 7263 3130 3531 3138 3230 3839 2f73  /src1051182089/s
+00000270: 2f73 7263 3330 3739 3233 3632 3634 2f73  /src3079236264/s
 00000280: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000290: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 000002a0: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 000002b0: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 000002c0: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 000002d0: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 000002e0: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto-0.2.8/src/roboto/cli/collections/__pycache__/delete.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/collections/__pycache__/delete.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 885 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 7503 0000  o........Y.eu...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 7503 0000  o.......2H.eu...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6406 6c05 6d06 5a06 0100 6404 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6408 6409 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 640a 6508 640b 6500 6a0b 6604 640c  ..d.e.d.e.j.f.d.
@@ -26,16 +26,16 @@
 00000190: 7465 7a13 4465 6c65 7465 6420 636f 6c6c  tez.Deleted coll
 000001a0: 6563 7469 6f6e 2029 0772 0300 0000 da07  ection ).r......
 000001b0: 6672 6f6d 5f69 6472 0c00 0000 da03 6f72  from_idr......or
 000001c0: 67da 0b63 6f6c 6c65 6374 696f 6e73 da06  g..collections..
 000001d0: 6465 6c65 7465 da05 7072 696e 7429 03da  delete..print)..
 000001e0: 0461 7267 7372 0a00 0000 720b 0000 00a9  .argsr....r.....
 000001f0: 0072 1500 0000 fae6 2f63 6f64 6562 7569  .r....../codebui
-00000200: 6c64 2f6f 7574 7075 742f 7372 6331 3035  ld/output/src105
-00000210: 3131 3832 3038 392f 7372 632f 636f 6465  1182089/src/code
+00000200: 6c64 2f6f 7574 7075 742f 7372 6333 3037  ld/output/src307
+00000210: 3932 3336 3236 342f 7372 632f 636f 6465  9236264/src/code
 00000220: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000230: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000240: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000250: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000260: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000270: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000280: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto-0.2.8/src/roboto/cli/collections/__pycache__/list.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/collections/__pycache__/list.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 591 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4f02 0000  o........Y.eO...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 4f02 0000  o.......2H.eO...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6406 6c05 6d06 5a06 0100 6404 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6408 6508 6409 6500 6a09  m.Z...d.e.d.e.j.
 00000070: 6604 640a 640b 8404 5a0a 6504 640b 650a  f.d.d...Z.e.d.e.
@@ -22,15 +22,15 @@
 00000150: 2907 7203 0000 00da 086c 6973 745f 616c  ).r......list_al
 00000160: 6cda 036f 7267 da0b 636f 6c6c 6563 7469  l..org..collecti
 00000170: 6f6e 73da 0570 7269 6e74 da06 7265 636f  ons..print..reco
 00000180: 7264 da04 6a73 6f6e 2904 da04 6172 6773  rd..json)...args
 00000190: 7208 0000 0072 0900 0000 da0a 636f 6c6c  r....r......coll
 000001a0: 6563 7469 6f6e a900 7214 0000 00fa e42f  ection..r....../
 000001b0: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-000001c0: 2f73 7263 3130 3531 3138 3230 3839 2f73  /src1051182089/s
+000001c0: 2f73 7263 3330 3739 3233 3632 3634 2f73  /src3079236264/s
 000001d0: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 000001e0: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 000001f0: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000200: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000210: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000220: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000230: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto-0.2.8/src/roboto/cli/collections/__pycache__/shared_helpdoc.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/collections/__pycache__/shared_helpdoc.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 620 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 6c02 0000  o........Y.el...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 6c02 0000  o.......2H.el...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 1000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5300 2904  Z.d.Z.d.Z.d.S.).
 00000040: 7a3f 4120 756e 6971 7565 2049 4420 7573  z?A unique ID us
 00000050: 6564 2074 6f20 7265 6665 7265 6e63 6520  ed to reference 
 00000060: 6120 636f 6c6c 6563 7469 6f6e 206f 6620  a collection of 
 00000070: 526f 626f 746f 2072 6573 6f75 7263 6573  Roboto resources
@@ -32,16 +32,16 @@
 000001f0: 736f 7572 6365 2069 6e20 7468 6520 636f  source in the co
 00000200: 6c6c 6563 7469 6f6e 2e4e 2903 da12 434f  llection.N)...CO
 00000210: 4c4c 4543 5449 4f4e 5f49 445f 4845 4c50  LLECTION_ID_HELP
 00000220: 5a17 434f 4c4c 4543 5449 4f4e 5f56 4552  Z.COLLECTION_VER
 00000230: 5349 4f4e 5f48 454c 505a 1143 4f4e 5445  SION_HELPZ.CONTE
 00000240: 4e54 5f4d 4f44 455f 4845 4c50 a900 7202  NT_MODE_HELP..r.
 00000250: 0000 0072 0200 0000 faee 2f63 6f64 6562  ...r....../codeb
-00000260: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-00000270: 3035 3131 3832 3038 392f 7372 632f 636f  051182089/src/co
+00000260: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+00000270: 3037 3932 3336 3236 342f 7372 632f 636f  079236264/src/co
 00000280: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 00000290: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 000002a0: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 000002b0: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 000002c0: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 000002d0: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 000002e0: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto-0.2.8/src/roboto/cli/collections/__pycache__/show.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/collections/__pycache__/show.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1482 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 ca05 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 ca05 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6404 6405 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6404 6406 6c06 6d07 5a07 0100 6404  ..d.d.l.m.Z...d.
 00000060: 6407 6c08 6d09 5a09 0100 6408 6409 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 640a  m.Z.m.Z.m.Z...d.
@@ -31,15 +31,15 @@
 000001e0: 0002 0000 0004 0000 0013 0000 0073 1c00  .............s..
 000001f0: 0000 6700 7c00 5d0a 7d01 7c01 6a00 8800  ..g.|.].}.|.j...
 00000200: 6a01 6b02 7202 7c01 9102 7102 5300 a900  j.k.r.|...q.S...
 00000210: 2902 da05 7661 6c75 65da 0c63 6f6e 7465  )...value..conte
 00000220: 6e74 5f6d 6f64 6529 02da 022e 30da 0178  nt_mode)....0..x
 00000230: a901 da04 6172 6773 720f 0000 00fa e42f  ....argsr....../
 00000240: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000250: 2f73 7263 3130 3531 3138 3230 3839 2f73  /src1051182089/s
+00000250: 2f73 7263 3330 3739 3233 3632 3634 2f73  /src3079236264/s
 00000260: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000270: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000280: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000290: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 000002a0: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 000002b0: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 000002c0: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto-0.2.8/src/roboto/cli/collections/__pycache__/update.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/collections/__pycache__/update.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3924 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 540f 0000  o........Y.eT...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 540f 0000  o.......2H.eT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6405 6406 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6405 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6408 6c0c 6d0d 5a0d 0100 6409  ..d.d.l.m.Z...d.
@@ -47,15 +47,15 @@
 000002e0: 027c 0164 008d 0291 0271 0253 00a9 0129  .|.d.....q.S...)
 000002f0: 02da 0d72 6573 6f75 7263 655f 7479 7065  ...resource_type
 00000300: da0b 7265 736f 7572 6365 5f69 64a9 0372  ..resource_id..r
 00000310: 0600 0000 7207 0000 00da 0744 6174 6173  ....r......Datas
 00000320: 6574 a902 da02 2e30 da0a 6461 7461 7365  et.....0..datase
 00000330: 745f 6964 a900 721c 0000 00fa e62f 636f  t_id..r....../co
 00000340: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-00000350: 7263 3130 3531 3138 3230 3839 2f73 7263  rc1051182089/src
+00000350: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
 00000360: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
 00000370: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
 00000380: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
 00000390: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
 000003a0: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
 000003b0: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
 000003c0: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
```

### Comparing `roboto-0.2.8/src/roboto/cli/collections/changes.py` & `roboto-0.2.9/src/roboto/cli/collections/changes.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/collections/create.py` & `roboto-0.2.9/src/roboto/cli/collections/create.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/collections/delete.py` & `roboto-0.2.9/src/roboto/cli/collections/delete.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/collections/list.py` & `roboto-0.2.9/src/roboto/cli/collections/list.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/collections/list_all.py` & `roboto-0.2.9/src/roboto/cli/collections/list_all.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/collections/shared_helpdoc.py` & `roboto-0.2.9/src/roboto/cli/collections/shared_helpdoc.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/collections/show.py` & `roboto-0.2.9/src/roboto/cli/collections/show.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/collections/update.py` & `roboto-0.2.9/src/roboto/cli/collections/update.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/command/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/command/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 334 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4e01 0000  o........Y.eN...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 4e01 0000  o.......2H.eN...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6700 6403 a201 5a07 6404 5300 2905  ..g.d...Z.d.S.).
 00000060: e901 0000 0029 03da 1345 7869 7374 696e  .....)...Existin
 00000070: 6750 6174 686c 6962 5061 7468 da11 4a73  gPathlibPath..Js
@@ -13,16 +13,16 @@
 000000c0: 6d61 6e64 5365 7429 0572 0200 0000 7203  mandSet).r....r.
 000000d0: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
 000000e0: 0000 4e29 08da 0461 7267 7372 0200 0000  ..N)...argsr....
 000000f0: 7203 0000 0072 0400 0000 da05 6d6f 6465  r....r......mode
 00000100: 6c72 0500 0000 7206 0000 00da 075f 5f61  lr....r......__a
 00000110: 6c6c 5f5f a900 720a 0000 0072 0a00 0000  ll__..r....r....
 00000120: fae4 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-00000130: 7075 742f 7372 6331 3035 3131 3832 3038  put/src105118208
-00000140: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+00000130: 7075 742f 7372 6333 3037 3932 3336 3236  put/src307923626
+00000140: 342f 7372 632f 636f 6465 7374 6172 2d63  4/src/codestar-c
 00000150: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 00000160: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 00000170: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 00000180: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 00000190: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 000001a0: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 000001b0: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto-0.2.8/src/roboto/cli/command/__pycache__/args.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/command/__pycache__/args.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1691 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 9b06 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 9b06 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 8400 5a05 4700  d.l.Z.d.d...Z.G.
 00000060: 6404 6405 8400 6405 6500 6a06 8303 5a07  d.d...d.e.j...Z.
 00000070: 6406 6407 8400 5a08 6401 5300 2908 e900  d.d...Z.d.S.)...
@@ -25,15 +25,15 @@
 00000180: 736f 6eda 056c 6f61 6473 da0a 5661 6c75  son..loads..Valu
 00000190: 6545 7272 6f72 da08 6172 6770 6172 7365  eError..argparse
 000001a0: da11 4172 6775 6d65 6e74 5479 7065 4572  ..ArgumentTypeEr
 000001b0: 726f 72da 0666 6f72 6d61 7429 04da 0361  ror..format)...a
 000001c0: 7267 5a08 6172 675f 7479 7065 da01 66da  rgZ.arg_type..f.
 000001d0: 0770 6179 6c6f 6164 a900 7213 0000 00fa  .payload..r.....
 000001e0: e02f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000001f0: 7574 2f73 7263 3130 3531 3138 3230 3839  ut/src1051182089
+000001f0: 7574 2f73 7263 3330 3739 3233 3632 3634  ut/src3079236264
 00000200: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 00000210: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000220: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000230: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000240: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000250: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000260: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto-0.2.8/src/roboto/cli/command/__pycache__/model.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/command/__pycache__/model.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3247 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 af0c 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 af0c 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6403 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6405 6406 6c00  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6405 6407 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6408 6c0b 6d0c 5a0c 0100 4700  ..d.d.l.m.Z...G.
@@ -44,16 +44,16 @@
 000002b0: 0043 0000 0073 1c00 0000 7c01 7c00 5f00  .C...s....|.|._.
 000002c0: 7c02 7c00 5f01 7c04 7c00 5f02 7c03 7c00  |.|._.|.|._.|.|.
 000002d0: 5f03 6400 5300 a901 4e29 0472 0d00 0000  _.d.S...N).r....
 000002e0: 720e 0000 0072 0f00 0000 7210 0000 0029  r....r....r....)
 000002f0: 05da 0473 656c 6672 1100 0000 7212 0000  ...selfr....r...
 00000300: 0072 1300 0000 7214 0000 00a9 0072 1700  .r....r......r..
 00000310: 0000 fae1 2f63 6f64 6562 7569 6c64 2f6f  ..../codebuild/o
-00000320: 7574 7075 742f 7372 6331 3035 3131 3832  utput/src1051182
-00000330: 3038 392f 7372 632f 636f 6465 7374 6172  089/src/codestar
+00000320: 7574 7075 742f 7372 6333 3037 3932 3336  utput/src3079236
+00000330: 3236 342f 7372 632f 636f 6465 7374 6172  264/src/codestar
 00000340: 2d63 6f6e 6e65 6374 696f 6e73 2e75 732d  -connections.us-
 00000350: 7765 7374 2d32 2e61 6d61 7a6f 6e61 7773  west-2.amazonaws
 00000360: 2e63 6f6d 2f67 6974 2d68 7474 702f 3036  .com/git-http/06
 00000370: 3631 3935 3131 3233 3835 2f75 732d 7765  6195112385/us-we
 00000380: 7374 2d32 2f65 3635 3032 6138 302d 6262  st-2/e6502a80-bb
 00000390: 3465 2d34 6662 652d 3837 3263 2d35 6434  4e-4fbe-872c-5d4
 000003a0: 3263 3139 3336 3939 642f 726f 626f 746f  2c193699d/roboto
```

### Comparing `roboto-0.2.8/src/roboto/cli/command/args.py` & `roboto-0.2.9/src/roboto/cli/command/args.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/command/model.py` & `roboto-0.2.9/src/roboto/cli/command/model.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/common_args/__init__.py` & `roboto-0.2.9/src/roboto/cli/common_args/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/common_args/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/common_args/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 579 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4302 0000  o........Y.eC...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 4302 0000  o.......2H.eC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a09 0100 6403  ..d.d.l.m.Z...d.
 00000060: 5a0a 6404 5300 2905 e901 0000 0029 07da  Z.d.S.)......)..
 00000070: 1241 6374 696f 6e50 6172 616d 6574 6572  .ActionParameter
@@ -22,16 +22,16 @@
 00000150: 0000 0072 0900 0000 7207 0000 0072 0800  ...r....r....r..
 00000160: 0000 4e29 0bda 0761 6374 696f 6e73 7202  ..N)...actionsr.
 00000170: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
 00000180: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
 00000190: 00da 046f 7267 7372 0900 0000 da07 5f5f  ...orgsr......__
 000001a0: 616c 6c5f 5fa9 0072 0d00 0000 720d 0000  all__..r....r...
 000001b0: 00fa e82f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-000001c0: 7470 7574 2f73 7263 3130 3531 3138 3230  tput/src10511820
-000001d0: 3839 2f73 7263 2f63 6f64 6573 7461 722d  89/src/codestar-
+000001c0: 7470 7574 2f73 7263 3330 3739 3233 3632  tput/src30792362
+000001d0: 3634 2f73 7263 2f63 6f64 6573 7461 722d  64/src/codestar-
 000001e0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000001f0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 00000200: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 00000210: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 00000220: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 00000230: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000240: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto-0.2.8/src/roboto/cli/common_args/__pycache__/actions.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/common_args/__pycache__/actions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 11809 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 212e 0000  o........Y.e!...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 212e 0000  o.......2H.e!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 3e01 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6402  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 6d08 5a08 0100 6404 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6404 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -73,16 +73,16 @@
 00000480: 655f 7061 7274 735a 096e 616d 655f 7061  e_partsZ.name_pa
 00000490: 7274 5a11 6e61 6d65 5f64 6967 6573 745f  rtZ.name_digest_
 000004a0: 7061 7274 73da 0c70 6172 7365 5f72 6573  parts..parse_res
 000004b0: 756c 745a 0c61 6374 696f 6e5f 6f77 6e65  ultZ.action_owne
 000004c0: 72da 0b61 6374 696f 6e5f 6e61 6d65 da0d  r..action_name..
 000004d0: 6163 7469 6f6e 5f64 6967 6573 74a9 0072  action_digest..r
 000004e0: 2300 0000 fae7 2f63 6f64 6562 7569 6c64  #...../codebuild
-000004f0: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000500: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+000004f0: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000500: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000510: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000520: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000530: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000540: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000550: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000560: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000570: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/cli/common_args/__pycache__/orgs.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/common_args/__pycache__/orgs.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 500 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 f401 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 f401 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 5a02 6501 a003 6403 a101 5a04 6502 6601  Z.e...d...Z.e.f.
 00000050: 6404 6500 6a05 6405 6506 6604 6406 6407  d.e.j.d.e.f.d.d.
 00000060: 8405 5a07 6401 5300 2908 e900 0000 004e  ..Z.d.S.)......N
 00000070: 7a96 5468 6520 6361 6c6c 696e 6720 6f72  z.The calling or
@@ -23,16 +23,16 @@
 00000160: 044e 7a05 2d2d 6f72 6746 2904 da08 7265  .Nz.--orgF)...re
 00000170: 7175 6972 6564 da04 7479 7065 da04 6865  quired..type..he
 00000180: 6c70 da07 6465 6661 756c 7429 03da 0c61  lp..default)...a
 00000190: 6464 5f61 7267 756d 656e 74da 0373 7472  dd_argument..str
 000001a0: da0e 4445 4641 554c 545f 4f52 475f 4944  ..DEFAULT_ORG_ID
 000001b0: 2902 7202 0000 0072 0300 0000 a900 720b  ).r....r......r.
 000001c0: 0000 00fa e42f 636f 6465 6275 696c 642f  ...../codebuild/
-000001d0: 6f75 7470 7574 2f73 7263 3130 3531 3138  output/src105118
-000001e0: 3230 3839 2f73 7263 2f63 6f64 6573 7461  2089/src/codesta
+000001d0: 6f75 7470 7574 2f73 7263 3330 3739 3233  output/src307923
+000001e0: 3632 3634 2f73 7263 2f63 6f64 6573 7461  6264/src/codesta
 000001f0: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 00000200: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 00000210: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 00000220: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 00000230: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 00000240: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 00000250: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto-0.2.8/src/roboto/cli/common_args/actions.py` & `roboto-0.2.9/src/roboto/cli/common_args/actions.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/config.py` & `roboto-0.2.9/src/roboto/cli/config.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/context.py` & `roboto-0.2.9/src/roboto/cli/context.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/__pycache__/create.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/datasets/__pycache__/create.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1527 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 f705 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 f705 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 6404 6405 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6404 6406 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6404 6407 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6408 650a 6409 6500 6a0b 6604 640a  ..d.e.d.e.j.f.d.
@@ -30,16 +30,16 @@
 000001d0: 7472 616e 7361 6374 696f 6e5f 6d61 6e61  transaction_mana
 000001e0: 6765 7272 0b00 0000 da03 7461 67da 036f  gerr......tag..o
 000001f0: 7267 720e 0000 00da 0570 7269 6e74 da04  rgr......print..
 00000200: 6a73 6f6e da05 6475 6d70 73da 0774 6f5f  json..dumps..to_
 00000210: 6469 6374 2904 da04 6172 6773 7209 0000  dict)...argsr...
 00000220: 0072 0a00 0000 da07 6461 7461 7365 74a9  .r......dataset.
 00000230: 0072 1d00 0000 fae3 2f63 6f64 6562 7569  .r....../codebui
-00000240: 6c64 2f6f 7574 7075 742f 7372 6331 3035  ld/output/src105
-00000250: 3131 3832 3038 392f 7372 632f 636f 6465  1182089/src/code
+00000240: 6c64 2f6f 7574 7075 742f 7372 6333 3037  ld/output/src307
+00000250: 3932 3336 3236 342f 7372 632f 636f 6465  9236264/src/code
 00000260: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000270: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000280: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000290: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 000002a0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 000002b0: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 000002c0: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/__pycache__/delete_dataset.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/datasets/__pycache__/show.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 981 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,84 +1,77 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 d503 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 3003 0000  o.......2H.e0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
-00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
-00000050: 6406 6c05 6d06 5a06 0100 6404 6407 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6408 6409 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 640a 6508 640b 6500 6a0b 6604 640c  ..d.e.d.e.j.f.d.
-00000080: 640d 8404 5a0c 640e 640f 8400 5a0d 6504  d...Z.d.d...Z.e.
-00000090: 6410 650c 650d 6411 6412 6901 6413 8d04  d.e.e.d.d.i.d...
-000000a0: 5a0e 6401 5300 2914 e900 0000 004e e903  Z.d.S.)......N..
-000000b0: 0000 0029 01da 0744 6174 6173 6574 e902  ...)...Dataset..
-000000c0: 0000 0029 01da 0d52 6f62 6f74 6f43 6f6d  ...)...RobotoCom
-000000d0: 6d61 6e64 2901 da0b 6164 645f 6f72 675f  mand)...add_org_
-000000e0: 6172 6729 01da 0a43 4c49 436f 6e74 6578  arg)...CLIContex
-000000f0: 74e9 0100 0000 2901 da0f 4441 5441 5345  t.....)...DATASE
-00000100: 545f 4944 5f48 454c 50da 0763 6f6e 7465  T_ID_HELP..conte
-00000110: 7874 da06 7061 7273 6572 6303 0000 0000  xt..parserc.....
-00000120: 0000 0000 0000 0004 0000 0007 0000 0043  ...............C
-00000130: 0000 0073 3a00 0000 7400 6a01 7c00 6a02  ...s:...t.j.|.j.
-00000140: 7c01 6a03 7c01 6a04 7c01 6a05 7c00 6a06  |.j.|.j.|.j.|.j.
-00000150: 6401 8d05 7d03 7c03 a007 a100 0100 7408  d...}.|.......t.
-00000160: 6402 7c00 6a02 9b00 9d02 8301 0100 6400  d.|.j.........d.
-00000170: 5300 2903 4e29 01da 066f 7267 5f69 647a  S.).N)...org_idz
-00000180: 1044 656c 6574 6564 2064 6174 6173 6574  .Deleted dataset
-00000190: 2029 0972 0300 0000 da07 6672 6f6d 5f69   ).r......from_i
-000001a0: 64da 0a64 6174 6173 6574 5f69 64da 0864  d..dataset_id..d
-000001b0: 6174 6173 6574 73da 0566 696c 6573 da13  atasets..files..
-000001c0: 7472 616e 7361 6374 696f 6e5f 6d61 6e61  transaction_mana
-000001d0: 6765 72da 036f 7267 da0e 6465 6c65 7465  ger..org..delete
-000001e0: 5f64 6174 6173 6574 da05 7072 696e 7429  _dataset..print)
-000001f0: 04da 0461 7267 7372 0a00 0000 720b 0000  ...argsr....r...
-00000200: 00da 0764 6174 6173 6574 a900 7217 0000  ...dataset..r...
-00000210: 00fa eb2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000220: 7470 7574 2f73 7263 3130 3531 3138 3230  tput/src10511820
-00000230: 3839 2f73 7263 2f63 6f64 6573 7461 722d  89/src/codestar-
-00000240: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
-00000250: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
-00000260: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
-00000270: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
-00000280: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
-00000290: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
-000002a0: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
-000002b0: 6169 2f72 6f62 6f74 6f2d 686f 7374 6564  ai/roboto-hosted
-000002c0: 2d61 7070 2f70 6163 6b61 6765 732f 726f  -app/packages/ro
-000002d0: 626f 746f 2f73 7263 2f72 6f62 6f74 6f2f  boto/src/roboto/
-000002e0: 636c 692f 6461 7461 7365 7473 2f64 656c  cli/datasets/del
-000002f0: 6574 655f 6461 7461 7365 742e 7079 7213  ete_dataset.pyr.
-00000300: 0000 000b 0000 0073 1200 0000 0401 0401  .......s........
-00000310: 0401 0401 0401 0401 06fb 0807 1401 7213  ..............r.
-00000320: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000330: 0100 0000 0700 0000 4300 0000 7320 0000  ........C...s ..
-00000340: 007c 006a 0064 0164 0274 0164 0374 0264  .|.j.d.d.t.d.t.d
-00000350: 048d 0501 0074 037c 0083 0101 0064 0053  .....t.|.....d.S
-00000360: 0029 054e 7a02 2d64 7a0c 2d2d 6461 7461  .).Nz.-dz.--data
-00000370: 7365 742d 6964 5429 03da 0474 7970 65da  set-idT)...type.
-00000380: 0872 6571 7569 7265 64da 0468 656c 7029  .required..help)
-00000390: 04da 0c61 6464 5f61 7267 756d 656e 74da  ...add_argument.
-000003a0: 0373 7472 7209 0000 0072 0600 0000 2901  .strr....r....).
-000003b0: 720b 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-000003c0: 1800 0000 da1b 6465 6c65 7465 5f64 6174  ......delete_dat
-000003d0: 6173 6574 5f73 6574 7570 5f70 6172 7365  aset_setup_parse
-000003e0: 7217 0000 0073 0800 0000 0401 0a01 06ff  r....s..........
-000003f0: 0c03 721e 0000 00da 0664 656c 6574 6572  ..r......deleter
-00000400: 1b00 0000 7a34 4465 6c65 7465 2064 6174  ....z4Delete dat
-00000410: 6173 6574 2028 616e 6420 616c 6c20 7265  aset (and all re
-00000420: 6c61 7465 6420 7375 6272 6573 6f75 7263  lated subresourc
-00000430: 6573 2920 6279 2069 642e 2904 da04 6e61  es) by id.)...na
-00000440: 6d65 da05 6c6f 6769 63da 0c73 6574 7570  me..logic..setup
-00000450: 5f70 6172 7365 72da 0e63 6f6d 6d61 6e64  _parser..command
-00000460: 5f6b 7761 7267 7329 0fda 0861 7267 7061  _kwargs)...argpa
-00000470: 7273 65da 0f64 6f6d 6169 6e2e 6461 7461  rse..domain.data
-00000480: 7365 7473 7203 0000 00da 0763 6f6d 6d61  setsr......comma
-00000490: 6e64 7205 0000 00da 0b63 6f6d 6d6f 6e5f  ndr......common_
-000004a0: 6172 6773 7206 0000 0072 0a00 0000 7207  argsr....r....r.
-000004b0: 0000 00da 0e73 6861 7265 645f 6865 6c70  .....shared_help
-000004c0: 646f 6372 0900 0000 da0e 4172 6775 6d65  docr......Argume
-000004d0: 6e74 5061 7273 6572 7213 0000 0072 1e00  ntParserr....r..
-000004e0: 0000 da16 6465 6c65 7465 5f64 6174 6173  ....delete_datas
-000004f0: 6574 5f63 6f6d 6d61 6e64 7217 0000 0072  et_commandr....r
-00000500: 1700 0000 7217 0000 0072 1800 0000 da08  ....r....r......
-00000510: 3c6d 6f64 756c 653e 0100 0000 731c 0000  <module>....s...
-00000520: 0008 010c 020c 010c 010c 010c 0114 0308  ................
-00000530: 0c02 0702 0102 0102 0106 010a fc         .............
+00000020: 0006 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
+00000040: 6403 6c02 6d03 5a03 0100 6404 6405 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6404 6406 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6407 6408 6c08 6d09 5a09 0100 6409  ..d.d.l.m.Z...d.
+00000070: 6507 640a 6500 6a0a 6604 640b 640c 8404  e.d.e.j.f.d.d...
+00000080: 5a0b 640d 640e 8400 5a0c 6505 640c 650b  Z.d.d...Z.e.d.e.
+00000090: 650c 640f 6410 6901 6411 8d04 5a0d 6401  e.d.d.i.d...Z.d.
+000000a0: 5300 2912 e900 0000 004e e903 0000 0029  S.)......N.....)
+000000b0: 01da 0744 6174 6173 6574 e902 0000 0029  ...Dataset.....)
+000000c0: 01da 0d52 6f62 6f74 6f43 6f6d 6d61 6e64  ...RobotoCommand
+000000d0: 2901 da0a 434c 4943 6f6e 7465 7874 e901  )...CLIContext..
+000000e0: 0000 0029 01da 0f44 4154 4153 4554 5f49  ...)...DATASET_I
+000000f0: 445f 4845 4c50 da07 636f 6e74 6578 74da  D_HELP..context.
+00000100: 0670 6172 7365 7263 0300 0000 0000 0000  .parserc........
+00000110: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
+00000120: 7332 0000 0074 00a0 017c 006a 027c 016a  s2...t...|.j.|.j
+00000130: 037c 016a 047c 016a 05a1 047d 0374 0674  .|.j.|.j...}.t.t
+00000140: 076a 087c 03a0 09a1 0064 0164 028d 0283  .j.|.....d.d....
+00000150: 0101 0064 0053 0029 034e e904 0000 0029  ...d.S.).N.....)
+00000160: 01da 0669 6e64 656e 7429 0a72 0300 0000  ...indent).r....
+00000170: da07 6672 6f6d 5f69 64da 0a64 6174 6173  ..from_id..datas
+00000180: 6574 5f69 64da 0864 6174 6173 6574 73da  et_id..datasets.
+00000190: 0566 696c 6573 da13 7472 616e 7361 6374  .files..transact
+000001a0: 696f 6e5f 6d61 6e61 6765 72da 0570 7269  ion_manager..pri
+000001b0: 6e74 da04 6a73 6f6e da05 6475 6d70 73da  nt..json..dumps.
+000001c0: 0774 6f5f 6469 6374 2904 da04 6172 6773  .to_dict)...args
+000001d0: 7209 0000 0072 0a00 0000 da06 7265 636f  r....r......reco
+000001e0: 7264 a900 7218 0000 00fa e12f 636f 6465  rd..r....../code
+000001f0: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
+00000200: 3330 3739 3233 3632 3634 2f73 7263 2f63  3079236264/src/c
+00000210: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
+00000220: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
+00000230: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
+00000240: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
+00000250: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
+00000260: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
+00000270: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
+00000280: 2f72 6f62 6f74 6f2d 6169 2f72 6f62 6f74  /roboto-ai/robot
+00000290: 6f2d 686f 7374 6564 2d61 7070 2f70 6163  o-hosted-app/pac
+000002a0: 6b61 6765 732f 726f 626f 746f 2f73 7263  kages/roboto/src
+000002b0: 2f72 6f62 6f74 6f2f 636c 692f 6461 7461  /roboto/cli/data
+000002c0: 7365 7473 2f73 686f 772e 7079 da04 7368  sets/show.py..sh
+000002d0: 6f77 0b00 0000 730e 0000 0004 0104 0104  ow....s.........
+000002e0: 0104 0104 0104 fc1a 0672 1a00 0000 6301  .........r....c.
+000002f0: 0000 0000 0000 0000 0000 0001 0000 0007  ................
+00000300: 0000 0043 0000 0073 1800 0000 7c00 6a00  ...C...s....|.j.
+00000310: 6401 6402 7401 6403 7402 6404 8d05 0100  d.d.t.d.t.d.....
+00000320: 6400 5300 2905 4e7a 022d 647a 0c2d 2d64  d.S.).Nz.-dz.--d
+00000330: 6174 6173 6574 2d69 6454 2903 da04 7479  ataset-idT)...ty
+00000340: 7065 da08 7265 7175 6972 6564 da04 6865  pe..required..he
+00000350: 6c70 2903 da0c 6164 645f 6172 6775 6d65  lp)...add_argume
+00000360: 6e74 da03 7374 7272 0800 0000 2901 720a  nt..strr....).r.
+00000370: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00000380: 0000 da11 7368 6f77 5f73 6574 7570 5f70  ....show_setup_p
+00000390: 6172 7365 7215 0000 0073 0600 0000 0401  arser....s......
+000003a0: 0a01 0aff 7220 0000 0072 1d00 0000 7a2a  ....r ...r....z*
+000003b0: 5368 6f77 2069 6e66 6f72 6d61 7469 6f6e  Show information
+000003c0: 2061 626f 7574 2061 2073 7065 6369 6669   about a specifi
+000003d0: 6320 6461 7461 7365 742e 2904 da04 6e61  c dataset.)...na
+000003e0: 6d65 da05 6c6f 6769 63da 0c73 6574 7570  me..logic..setup
+000003f0: 5f70 6172 7365 72da 0e63 6f6d 6d61 6e64  _parser..command
+00000400: 5f6b 7761 7267 7329 0eda 0861 7267 7061  _kwargs)...argpa
+00000410: 7273 6572 1300 0000 da0f 646f 6d61 696e  rser......domain
+00000420: 2e64 6174 6173 6574 7372 0300 0000 da07  .datasetsr......
+00000430: 636f 6d6d 616e 6472 0500 0000 7209 0000  commandr....r...
+00000440: 0072 0600 0000 da0e 7368 6172 6564 5f68  .r......shared_h
+00000450: 656c 7064 6f63 7208 0000 00da 0e41 7267  elpdocr......Arg
+00000460: 756d 656e 7450 6172 7365 7272 1a00 0000  umentParserr....
+00000470: 7220 0000 00da 0c73 686f 775f 636f 6d6d  r .....show_comm
+00000480: 616e 6472 1800 0000 7218 0000 0072 1800  andr....r....r..
+00000490: 0000 7219 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000004a0: 3e01 0000 0073 1c00 0000 0801 0801 0c02  >....s..........
+000004b0: 0c01 0c01 0c01 1403 080a 0206 0201 0201  ................
+000004c0: 0201 0601 0afc                           ......
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/__pycache__/delete_files.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/datasets/__pycache__/download_files.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1271 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,105 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 f704 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 da05 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
-00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
-00000050: 6406 6c05 6d06 5a06 0100 6404 6407 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6408 6409 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 640a 6508 640b 6500 6a0b 6604 640c  ..d.e.d.e.j.f.d.
-00000080: 640d 8404 5a0c 640e 640f 8400 5a0d 6504  d...Z.d.d...Z.e.
-00000090: 6410 650c 650d 6411 6412 6901 6413 8d04  d.e.e.d.d.i.d...
-000000a0: 5a0e 6401 5300 2914 e900 0000 004e e903  Z.d.S.)......N..
-000000b0: 0000 0029 01da 0744 6174 6173 6574 e902  ...)...Dataset..
-000000c0: 0000 0029 01da 0d52 6f62 6f74 6f43 6f6d  ...)...RobotoCom
-000000d0: 6d61 6e64 2901 da0b 6164 645f 6f72 675f  mand)...add_org_
-000000e0: 6172 6729 01da 0a43 4c49 436f 6e74 6578  arg)...CLIContex
-000000f0: 74e9 0100 0000 2901 da0f 4441 5441 5345  t.....)...DATASE
-00000100: 545f 4944 5f48 454c 50da 0763 6f6e 7465  T_ID_HELP..conte
-00000110: 7874 da06 7061 7273 6572 6303 0000 0000  xt..parserc.....
-00000120: 0000 0000 0000 0004 0000 0007 0000 0043  ...............C
-00000130: 0000 0073 3400 0000 7400 6a01 7c00 6a02  ...s4...t.j.|.j.
-00000140: 7c01 6a03 7c01 6a04 7c01 6a05 7c00 6a06  |.j.|.j.|.j.|.j.
-00000150: 6401 8d05 7d03 7c03 6a07 7c00 6a08 7c00  d...}.|.j.|.j.|.
-00000160: 6a09 6402 8d02 0100 6400 5300 2903 4e29  j.d.....d.S.).N)
-00000170: 01da 066f 7267 5f69 6429 02da 1069 6e63  ...org_id)...inc
-00000180: 6c75 6465 5f70 6174 7465 726e 73da 1065  lude_patterns..e
-00000190: 7863 6c75 6465 5f70 6174 7465 726e 7329  xclude_patterns)
-000001a0: 0a72 0300 0000 da07 6672 6f6d 5f69 64da  .r......from_id.
-000001b0: 0a64 6174 6173 6574 5f69 64da 0864 6174  .dataset_id..dat
-000001c0: 6173 6574 73da 0566 696c 6573 da13 7472  asets..files..tr
-000001d0: 616e 7361 6374 696f 6e5f 6d61 6e61 6765  ansaction_manage
-000001e0: 72da 036f 7267 da0c 6465 6c65 7465 5f66  r..org..delete_f
-000001f0: 696c 6573 da07 696e 636c 7564 65da 0765  iles..include..e
-00000200: 7863 6c75 6465 2904 da04 6172 6773 720a  xclude)...argsr.
-00000210: 0000 0072 0b00 0000 da07 6461 7461 7365  ...r......datase
-00000220: 74a9 0072 1a00 0000 fae9 2f63 6f64 6562  t..r....../codeb
-00000230: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-00000240: 3035 3131 3832 3038 392f 7372 632f 636f  051182089/src/co
-00000250: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
-00000260: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
-00000270: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
-00000280: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
-00000290: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
-000002a0: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
-000002b0: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
-000002c0: 726f 626f 746f 2d61 692f 726f 626f 746f  roboto-ai/roboto
-000002d0: 2d68 6f73 7465 642d 6170 702f 7061 636b  -hosted-app/pack
-000002e0: 6167 6573 2f72 6f62 6f74 6f2f 7372 632f  ages/roboto/src/
-000002f0: 726f 626f 746f 2f63 6c69 2f64 6174 6173  roboto/cli/datas
-00000300: 6574 732f 6465 6c65 7465 5f66 696c 6573  ets/delete_files
-00000310: 2e70 7972 1500 0000 0b00 0000 7310 0000  .pyr........s...
-00000320: 0004 0104 0104 0104 0104 0104 0106 fb16  ................
-00000330: 0872 1500 0000 6301 0000 0000 0000 0000  .r....c.........
-00000340: 0000 0001 0000 0007 0000 0043 0000 0073  ...........C...s
-00000350: 4800 0000 7c00 6a00 6401 6402 7401 6403  H...|.j.d.d.t.d.
-00000360: 7402 6404 8d05 0100 7c00 6a00 6405 6406  t.d.....|.j.d.d.
-00000370: 7401 6407 6408 6409 8d05 0100 7c00 6a00  t.d.d.d.....|.j.
-00000380: 640a 640b 7401 6407 640c 6409 8d05 0100  d.d.t.d.d.d.....
-00000390: 7403 7c00 8301 0100 6400 5300 290d 4e7a  t.|.....d.S.).Nz
-000003a0: 022d 647a 0c2d 2d64 6174 6173 6574 2d69  .-dz.--dataset-i
-000003b0: 6454 2903 da04 7479 7065 da08 7265 7175  dT)...type..requ
-000003c0: 6972 6564 da04 6865 6c70 7a02 2d69 7a09  ired..helpz.-iz.
-000003d0: 2d2d 696e 636c 7564 65da 012a 7a1c 5a65  --include..*z.Ze
-000003e0: 726f 206f 7220 6d6f 7265 2069 6e63 6c75  ro or more inclu
-000003f0: 6465 2066 696c 7465 7273 2903 721c 0000  de filters).r...
-00000400: 00da 056e 6172 6773 721e 0000 007a 022d  ...nargsr....z.-
-00000410: 787a 092d 2d65 7863 6c75 6465 7a1c 5a65  xz.--excludez.Ze
-00000420: 726f 206f 7220 6d6f 7265 2065 7863 6c75  ro or more exclu
-00000430: 6465 2066 696c 7465 7273 2904 da0c 6164  de filters)...ad
-00000440: 645f 6172 6775 6d65 6e74 da03 7374 7272  d_argument..strr
-00000450: 0900 0000 7206 0000 0029 0172 0b00 0000  ....r....).r....
-00000460: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-00000470: 1964 656c 6574 655f 6669 6c65 735f 7365  .delete_files_se
-00000480: 7475 705f 7061 7273 6572 1700 0000 7324  tup_parser....s$
-00000490: 0000 0004 010a 0106 ff04 0302 0102 0102  ................
-000004a0: 0102 0102 0106 fb04 0702 0102 0102 0102  ................
-000004b0: 0102 0106 fb0c 0772 2300 0000 7a0c 6465  .......r#...z.de
-000004c0: 6c65 7465 2d66 696c 6573 721e 0000 007a  lete-filesr....z
-000004d0: 2744 656c 6574 6520 6669 6c65 2873 2920  'Delete file(s) 
-000004e0: 6672 6f6d 2061 2073 7065 6369 6669 6320  from a specific 
-000004f0: 6461 7461 7365 742e 2904 da04 6e61 6d65  dataset.)...name
-00000500: da05 6c6f 6769 63da 0c73 6574 7570 5f70  ..logic..setup_p
-00000510: 6172 7365 72da 0e63 6f6d 6d61 6e64 5f6b  arser..command_k
-00000520: 7761 7267 7329 0fda 0861 7267 7061 7273  wargs)...argpars
-00000530: 65da 0f64 6f6d 6169 6e2e 6461 7461 7365  e..domain.datase
-00000540: 7473 7203 0000 00da 0763 6f6d 6d61 6e64  tsr......command
-00000550: 7205 0000 00da 0b63 6f6d 6d6f 6e5f 6172  r......common_ar
-00000560: 6773 7206 0000 0072 0a00 0000 7207 0000  gsr....r....r...
-00000570: 00da 0e73 6861 7265 645f 6865 6c70 646f  ...shared_helpdo
-00000580: 6372 0900 0000 da0e 4172 6775 6d65 6e74  cr......Argument
-00000590: 5061 7273 6572 7215 0000 0072 2300 0000  Parserr....r#...
-000005a0: da14 6465 6c65 7465 5f66 696c 6573 5f63  ..delete_files_c
-000005b0: 6f6d 6d61 6e64 721a 0000 0072 1a00 0000  ommandr....r....
-000005c0: 721a 0000 0072 1b00 0000 da08 3c6d 6f64  r....r......<mod
-000005d0: 756c 653e 0100 0000 731c 0000 0008 010c  ule>....s.......
-000005e0: 020c 010c 010c 010c 0114 0308 0c02 1502  ................
-000005f0: 0102 0102 0106 010a fc                   .........
+00000020: 0006 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
+00000040: 6403 6c02 6d03 5a03 0100 6404 6405 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6404 6406 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6407 6408 6c08 6d09 5a09 0100 6409  ..d.d.l.m.Z...d.
+00000070: 6507 640a 6500 6a0a 6604 640b 640c 8404  e.d.e.j.f.d.d...
+00000080: 5a0b 640d 640e 8400 5a0c 6505 640f 650b  Z.d.d...Z.e.d.e.
+00000090: 650c 6410 6411 6901 6412 8d04 5a0d 6401  e.d.d.i.d...Z.d.
+000000a0: 5300 2913 e900 0000 004e e903 0000 0029  S.)......N.....)
+000000b0: 01da 0744 6174 6173 6574 e902 0000 0029  ...Dataset.....)
+000000c0: 01da 0d52 6f62 6f74 6f43 6f6d 6d61 6e64  ...RobotoCommand
+000000d0: 2901 da0a 434c 4943 6f6e 7465 7874 e901  )...CLIContext..
+000000e0: 0000 0029 01da 0f44 4154 4153 4554 5f49  ...)...DATASET_I
+000000f0: 445f 4845 4c50 da07 636f 6e74 6578 74da  D_HELP..context.
+00000100: 0670 6172 7365 7263 0300 0000 0000 0000  .parserc........
+00000110: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
+00000120: 7332 0000 0074 00a0 017c 006a 027c 016a  s2...t...|.j.|.j
+00000130: 037c 016a 047c 016a 05a1 047d 037c 036a  .|.j.|.j...}.|.j
+00000140: 067c 006a 077c 006a 087c 006a 0964 018d  .|.j.|.j.|.j.d..
+00000150: 0301 0064 0053 0029 024e 2903 da08 6f75  ...d.S.).N)...ou
+00000160: 745f 7061 7468 da10 696e 636c 7564 655f  t_path..include_
+00000170: 7061 7474 6572 6e73 da10 6578 636c 7564  patterns..exclud
+00000180: 655f 7061 7474 6572 6e73 290a 7203 0000  e_patterns).r...
+00000190: 00da 0766 726f 6d5f 6964 da0a 6461 7461  ...from_id..data
+000001a0: 7365 745f 6964 da08 6461 7461 7365 7473  set_id..datasets
+000001b0: da05 6669 6c65 73da 1374 7261 6e73 6163  ..files..transac
+000001c0: 7469 6f6e 5f6d 616e 6167 6572 da0e 646f  tion_manager..do
+000001d0: 776e 6c6f 6164 5f66 696c 6573 da04 7061  wnload_files..pa
+000001e0: 7468 da07 696e 636c 7564 65da 0765 7863  th..include..exc
+000001f0: 6c75 6465 2904 da04 6172 6773 7209 0000  lude)...argsr...
+00000200: 0072 0a00 0000 da06 7265 636f 7264 a900  .r......record..
+00000210: 7219 0000 00fa eb2f 636f 6465 6275 696c  r....../codebuil
+00000220: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+00000230: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
+00000240: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
+00000250: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
+00000260: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
+00000270: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
+00000280: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
+00000290: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
+000002a0: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
+000002b0: 6f74 6f2d 6169 2f72 6f62 6f74 6f2d 686f  oto-ai/roboto-ho
+000002c0: 7374 6564 2d61 7070 2f70 6163 6b61 6765  sted-app/package
+000002d0: 732f 726f 626f 746f 2f73 7263 2f72 6f62  s/roboto/src/rob
+000002e0: 6f74 6f2f 636c 692f 6461 7461 7365 7473  oto/cli/datasets
+000002f0: 2f64 6f77 6e6c 6f61 645f 6669 6c65 732e  /download_files.
+00000300: 7079 7213 0000 000b 0000 0073 1200 0000  pyr........s....
+00000310: 0401 0401 0401 0401 0401 04fc 0407 0c01  ................
+00000320: 0aff 7213 0000 0063 0100 0000 0000 0000  ..r....c........
+00000330: 0000 0000 0100 0000 0700 0000 4300 0000  ............C...
+00000340: 7356 0000 007c 006a 0064 0164 0274 0164  sV...|.j.d.d.t.d
+00000350: 0374 0264 048d 0501 007c 006a 0064 0564  .t.d.....|.j.d.d
+00000360: 0674 036a 0464 0364 0764 048d 0501 007c  .t.j.d.d.d.....|
+00000370: 006a 0064 0864 0974 0164 0a64 0b64 0c8d  .j.d.d.t.d.d.d..
+00000380: 0501 007c 006a 0064 0d64 0e74 0164 0a64  ...|.j.d.d.t.d.d
+00000390: 0f64 0c8d 0501 0064 0053 0029 104e 7a02  .d.....d.S.).Nz.
+000003a0: 2d64 7a0c 2d2d 6461 7461 7365 742d 6964  -dz.--dataset-id
+000003b0: 5429 03da 0474 7970 65da 0872 6571 7569  T)...type..requi
+000003c0: 7265 64da 0468 656c 707a 022d 707a 062d  red..helpz.-pz.-
+000003d0: 2d70 6174 687a 2c54 6865 2064 6f77 6e6c  -pathz,The downl
+000003e0: 6f61 6420 6465 7374 696e 6174 696f 6e20  oad destination 
+000003f0: 666f 7220 7468 6973 206f 7065 7261 7469  for this operati
+00000400: 6f6e 2e7a 022d 697a 092d 2d69 6e63 6c75  on.z.-iz.--inclu
+00000410: 6465 da01 2a7a 3c5a 6572 6f20 6f72 206d  de..*z<Zero or m
+00000420: 6f72 6520 696e 636c 7564 6520 6669 6c74  ore include filt
+00000430: 6572 7320 2869 6620 7061 7468 2070 6f69  ers (if path poi
+00000440: 6e74 7320 746f 2061 2064 6972 6563 746f  nts to a directo
+00000450: 7279 2929 0372 1b00 0000 da05 6e61 7267  ry)).r......narg
+00000460: 7372 1d00 0000 7a02 2d78 7a09 2d2d 6578  sr....z.-xz.--ex
+00000470: 636c 7564 657a 3c5a 6572 6f20 6f72 206d  cludez<Zero or m
+00000480: 6f72 6520 6578 636c 7564 6520 6669 6c74  ore exclude filt
+00000490: 6572 7320 2869 6620 7061 7468 2070 6f69  ers (if path poi
+000004a0: 6e74 7320 746f 2061 2064 6972 6563 746f  nts to a directo
+000004b0: 7279 2929 05da 0c61 6464 5f61 7267 756d  ry))...add_argum
+000004c0: 656e 74da 0373 7472 7208 0000 00da 0770  ent..strr......p
+000004d0: 6174 686c 6962 da04 5061 7468 2901 720a  athlib..Path).r.
+000004e0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+000004f0: 0000 da1b 646f 776e 6c6f 6164 5f66 696c  ....download_fil
+00000500: 6573 5f73 6574 7570 5f70 6172 7365 7218  es_setup_parser.
+00000510: 0000 0073 3000 0000 0401 0a01 06ff 0403  ...s0...........
+00000520: 0201 0201 0401 0201 0201 06fb 0407 0201  ................
+00000530: 0201 0201 0201 0201 06fb 0407 0201 0201  ................
+00000540: 0201 0201 0201 0afb 7224 0000 007a 0e64  ........r$...z.d
+00000550: 6f77 6e6c 6f61 642d 6669 6c65 7372 1d00  ownload-filesr..
+00000560: 0000 7a36 446f 776e 6c6f 6164 7320 6120  ..z6Downloads a 
+00000570: 6669 6c65 206f 7220 6469 7265 6374 6f72  file or director
+00000580: 7920 6672 6f6d 2061 2073 7065 6369 6669  y from a specifi
+00000590: 6320 6461 7461 7365 742e 2904 da04 6e61  c dataset.)...na
+000005a0: 6d65 da05 6c6f 6769 63da 0c73 6574 7570  me..logic..setup
+000005b0: 5f70 6172 7365 72da 0e63 6f6d 6d61 6e64  _parser..command
+000005c0: 5f6b 7761 7267 7329 0eda 0861 7267 7061  _kwargs)...argpa
+000005d0: 7273 6572 2200 0000 da0f 646f 6d61 696e  rser".....domain
+000005e0: 2e64 6174 6173 6574 7372 0300 0000 da07  .datasetsr......
+000005f0: 636f 6d6d 616e 6472 0500 0000 7209 0000  commandr....r...
+00000600: 0072 0600 0000 da0e 7368 6172 6564 5f68  .r......shared_h
+00000610: 656c 7064 6f63 7208 0000 00da 0e41 7267  elpdocr......Arg
+00000620: 756d 656e 7450 6172 7365 7272 1300 0000  umentParserr....
+00000630: 7224 0000 00da 1664 6f77 6e6c 6f61 645f  r$.....download_
+00000640: 6669 6c65 735f 636f 6d6d 616e 6472 1900  files_commandr..
+00000650: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00000660: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000670: 1c00 0000 0801 0801 0c02 0c01 0c01 0c01  ................
+00000680: 1403 080d 021b 0201 0201 0201 0601 0afc  ................
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/__pycache__/download_files.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/datasets/__pycache__/list_files.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1585 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,111 +1,97 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 3106 0000  o........Y.e1...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 f004 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 6404 6405 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6404 6406 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6404 6407 6c08 6d09 5a09 0100 6408  ..d.d.l.m.Z...d.
-00000070: 6409 6c0a 6d0b 5a0b 0100 640a 6509 640b  d.l.m.Z...d.e.d.
-00000080: 6500 6a0c 6604 640c 640d 8404 5a0d 640e  e.j.f.d.d...Z.d.
-00000090: 640f 8400 5a0e 6505 6410 650d 650e 6411  d...Z.e.d.e.e.d.
-000000a0: 6412 6901 6413 8d04 5a0f 6401 5300 2914  d.i.d...Z.d.S.).
-000000b0: e900 0000 004e e903 0000 0029 01da 0744  .....N.....)...D
-000000c0: 6174 6173 6574 e902 0000 0029 01da 0d52  ataset.....)...R
-000000d0: 6f62 6f74 6f43 6f6d 6d61 6e64 2901 da0b  obotoCommand)...
-000000e0: 6164 645f 6f72 675f 6172 6729 01da 0a43  add_org_arg)...C
-000000f0: 4c49 436f 6e74 6578 74e9 0100 0000 2901  LIContext.....).
-00000100: da0f 4441 5441 5345 545f 4944 5f48 454c  ..DATASET_ID_HEL
-00000110: 50da 0763 6f6e 7465 7874 da06 7061 7273  P..context..pars
-00000120: 6572 6303 0000 0000 0000 0000 0000 0004  erc.............
-00000130: 0000 0007 0000 0043 0000 0073 3800 0000  .......C...s8...
-00000140: 7400 6a01 7c00 6a02 7c01 6a03 7c01 6a04  t.j.|.j.|.j.|.j.
-00000150: 7c01 6a05 7c00 6a06 6401 8d05 7d03 7c03  |.j.|.j.d...}.|.
-00000160: 6a07 7c00 6a08 7c00 6a09 7c00 6a0a 6402  j.|.j.|.j.|.j.d.
-00000170: 8d03 0100 6400 5300 2903 4e29 01da 066f  ....d.S.).N)...o
-00000180: 7267 5f69 6429 03da 086f 7574 5f70 6174  rg_id)...out_pat
-00000190: 68da 1069 6e63 6c75 6465 5f70 6174 7465  h..include_patte
-000001a0: 726e 73da 1065 7863 6c75 6465 5f70 6174  rns..exclude_pat
-000001b0: 7465 726e 7329 0b72 0300 0000 da07 6672  terns).r......fr
-000001c0: 6f6d 5f69 64da 0a64 6174 6173 6574 5f69  om_id..dataset_i
-000001d0: 64da 0864 6174 6173 6574 73da 0566 696c  d..datasets..fil
-000001e0: 6573 da13 7472 616e 7361 6374 696f 6e5f  es..transaction_
-000001f0: 6d61 6e61 6765 72da 036f 7267 da0e 646f  manager..org..do
-00000200: 776e 6c6f 6164 5f66 696c 6573 da04 7061  wnload_files..pa
-00000210: 7468 da07 696e 636c 7564 65da 0765 7863  th..include..exc
-00000220: 6c75 6465 2904 da04 6172 6773 720a 0000  lude)...argsr...
-00000230: 0072 0b00 0000 da06 7265 636f 7264 a900  .r......record..
-00000240: 721c 0000 00fa eb2f 636f 6465 6275 696c  r....../codebuil
-00000250: 642f 6f75 7470 7574 2f73 7263 3130 3531  d/output/src1051
-00000260: 3138 3230 3839 2f73 7263 2f63 6f64 6573  182089/src/codes
-00000270: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
-00000280: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
-00000290: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
-000002a0: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
-000002b0: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
-000002c0: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
-000002d0: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
-000002e0: 6f74 6f2d 6169 2f72 6f62 6f74 6f2d 686f  oto-ai/roboto-ho
-000002f0: 7374 6564 2d61 7070 2f70 6163 6b61 6765  sted-app/package
-00000300: 732f 726f 626f 746f 2f73 7263 2f72 6f62  s/roboto/src/rob
-00000310: 6f74 6f2f 636c 692f 6461 7461 7365 7473  oto/cli/datasets
-00000320: 2f64 6f77 6e6c 6f61 645f 6669 6c65 732e  /download_files.
-00000330: 7079 7216 0000 000c 0000 0073 1400 0000  pyr........s....
-00000340: 0401 0401 0401 0401 0401 0401 06fb 0408  ................
-00000350: 0c01 0aff 7216 0000 0063 0100 0000 0000  ....r....c......
-00000360: 0000 0000 0000 0100 0000 0700 0000 4300  ..............C.
-00000370: 0000 735e 0000 007c 006a 0064 0164 0274  ..s^...|.j.d.d.t
-00000380: 0164 0374 0264 048d 0501 007c 006a 0064  .d.t.d.....|.j.d
-00000390: 0564 0674 036a 0464 0364 0764 048d 0501  .d.t.j.d.d.d....
-000003a0: 007c 006a 0064 0864 0974 0164 0a64 0b64  .|.j.d.d.t.d.d.d
-000003b0: 0c8d 0501 007c 006a 0064 0d64 0e74 0164  .....|.j.d.d.t.d
-000003c0: 0a64 0f64 0c8d 0501 0074 057c 0083 0101  .d.d.....t.|....
-000003d0: 0064 0053 0029 104e 7a02 2d64 7a0c 2d2d  .d.S.).Nz.-dz.--
-000003e0: 6461 7461 7365 742d 6964 5429 03da 0474  dataset-idT)...t
-000003f0: 7970 65da 0872 6571 7569 7265 64da 0468  ype..required..h
-00000400: 656c 707a 022d 707a 062d 2d70 6174 687a  elpz.-pz.--pathz
-00000410: 2c54 6865 2064 6f77 6e6c 6f61 6420 6465  ,The download de
-00000420: 7374 696e 6174 696f 6e20 666f 7220 7468  stination for th
-00000430: 6973 206f 7065 7261 7469 6f6e 2e7a 022d  is operation.z.-
-00000440: 697a 092d 2d69 6e63 6c75 6465 da01 2a7a  iz.--include..*z
-00000450: 3c5a 6572 6f20 6f72 206d 6f72 6520 696e  <Zero or more in
-00000460: 636c 7564 6520 6669 6c74 6572 7320 2869  clude filters (i
-00000470: 6620 7061 7468 2070 6f69 6e74 7320 746f  f path points to
-00000480: 2061 2064 6972 6563 746f 7279 2929 0372   a directory)).r
-00000490: 1e00 0000 da05 6e61 7267 7372 2000 0000  ......nargsr ...
-000004a0: 7a02 2d78 7a09 2d2d 6578 636c 7564 657a  z.-xz.--excludez
-000004b0: 3c5a 6572 6f20 6f72 206d 6f72 6520 6578  <Zero or more ex
-000004c0: 636c 7564 6520 6669 6c74 6572 7320 2869  clude filters (i
-000004d0: 6620 7061 7468 2070 6f69 6e74 7320 746f  f path points to
-000004e0: 2061 2064 6972 6563 746f 7279 2929 06da   a directory))..
-000004f0: 0c61 6464 5f61 7267 756d 656e 74da 0373  .add_argument..s
-00000500: 7472 7209 0000 00da 0770 6174 686c 6962  trr......pathlib
-00000510: da04 5061 7468 7206 0000 0029 0172 0b00  ..Pathr....).r..
-00000520: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00000530: 00da 1b64 6f77 6e6c 6f61 645f 6669 6c65  ...download_file
-00000540: 735f 7365 7475 705f 7061 7273 6572 1a00  s_setup_parser..
-00000550: 0000 7332 0000 0004 010a 0106 ff04 0302  ..s2............
-00000560: 0102 0104 0102 0102 0106 fb04 0702 0102  ................
-00000570: 0102 0102 0102 0106 fb04 0702 0102 0102  ................
-00000580: 0102 0102 0106 fb0c 0772 2700 0000 7a0e  .........r'...z.
-00000590: 646f 776e 6c6f 6164 2d66 696c 6573 7220  download-filesr 
-000005a0: 0000 007a 3644 6f77 6e6c 6f61 6473 2061  ...z6Downloads a
-000005b0: 2066 696c 6520 6f72 2064 6972 6563 746f   file or directo
-000005c0: 7279 2066 726f 6d20 6120 7370 6563 6966  ry from a specif
-000005d0: 6963 2064 6174 6173 6574 2e29 04da 046e  ic dataset.)...n
-000005e0: 616d 65da 056c 6f67 6963 da0c 7365 7475  ame..logic..setu
-000005f0: 705f 7061 7273 6572 da0e 636f 6d6d 616e  p_parser..comman
-00000600: 645f 6b77 6172 6773 2910 da08 6172 6770  d_kwargs)...argp
-00000610: 6172 7365 7225 0000 00da 0f64 6f6d 6169  arser%.....domai
-00000620: 6e2e 6461 7461 7365 7473 7203 0000 00da  n.datasetsr.....
-00000630: 0763 6f6d 6d61 6e64 7205 0000 00da 0b63  .commandr......c
-00000640: 6f6d 6d6f 6e5f 6172 6773 7206 0000 0072  ommon_argsr....r
-00000650: 0a00 0000 7207 0000 00da 0e73 6861 7265  ....r......share
-00000660: 645f 6865 6c70 646f 6372 0900 0000 da0e  d_helpdocr......
-00000670: 4172 6775 6d65 6e74 5061 7273 6572 7216  ArgumentParserr.
-00000680: 0000 0072 2700 0000 da16 646f 776e 6c6f  ...r'.....downlo
-00000690: 6164 5f66 696c 6573 5f63 6f6d 6d61 6e64  ad_files_command
-000006a0: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-000006b0: 1d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-000006c0: 0000 731e 0000 0008 0108 010c 020c 010c  ..s.............
-000006d0: 010c 010c 0114 0308 0e02 1c02 0102 0102  ................
-000006e0: 0106 010a fc                             .....
+00000060: 0100 6407 6408 6c08 6d09 5a09 0100 6409  ..d.d.l.m.Z...d.
+00000070: 6507 640a 6500 6a0a 6604 640b 640c 8404  e.d.e.j.f.d.d...
+00000080: 5a0b 640d 640e 8400 5a0c 6505 640f 650b  Z.d.d...Z.e.d.e.
+00000090: 650c 6410 6411 6901 6412 8d04 5a0d 6401  e.d.d.i.d...Z.d.
+000000a0: 5300 2913 e900 0000 004e e903 0000 0029  S.)......N.....)
+000000b0: 01da 0744 6174 6173 6574 e902 0000 0029  ...Dataset.....)
+000000c0: 01da 0d52 6f62 6f74 6f43 6f6d 6d61 6e64  ...RobotoCommand
+000000d0: 2901 da0a 434c 4943 6f6e 7465 7874 e901  )...CLIContext..
+000000e0: 0000 0029 01da 0f44 4154 4153 4554 5f49  ...)...DATASET_I
+000000f0: 445f 4845 4c50 da07 636f 6e74 6578 74da  D_HELP..context.
+00000100: 0670 6172 7365 7263 0300 0000 0000 0000  .parserc........
+00000110: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
+00000120: 7346 0000 0074 00a0 017c 006a 027c 016a  sF...t...|.j.|.j
+00000130: 037c 016a 047c 016a 05a1 047d 037c 03a0  .|.j.|.j...}.|..
+00000140: 067c 006a 077c 006a 08a1 0244 005d 0c7d  .|.j.|.j...D.].}
+00000150: 0474 096a 0aa0 0b7c 046a 0c9b 0064 019d  .t.j...|.j...d..
+00000160: 02a1 0101 0071 1464 0053 0029 024e da01  .....q.d.S.).N..
+00000170: 0a29 0d72 0300 0000 da07 6672 6f6d 5f69  .).r......from_i
+00000180: 64da 0a64 6174 6173 6574 5f69 64da 0864  d..dataset_id..d
+00000190: 6174 6173 6574 73da 0566 696c 6573 da13  atasets..files..
+000001a0: 7472 616e 7361 6374 696f 6e5f 6d61 6e61  transaction_mana
+000001b0: 6765 72da 0a6c 6973 745f 6669 6c65 73da  ger..list_files.
+000001c0: 0769 6e63 6c75 6465 da07 6578 636c 7564  .include..exclud
+000001d0: 65da 0373 7973 da06 7374 646f 7574 da05  e..sys..stdout..
+000001e0: 7772 6974 65da 0d72 656c 6174 6976 655f  write..relative_
+000001f0: 7061 7468 2905 da04 6172 6773 7209 0000  path)...argsr...
+00000200: 0072 0a00 0000 da06 7265 636f 7264 da01  .r......record..
+00000210: 66a9 0072 1b00 0000 fae7 2f63 6f64 6562  f..r....../codeb
+00000220: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+00000230: 3037 3932 3336 3236 342f 7372 632f 636f  079236264/src/co
+00000240: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
+00000250: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
+00000260: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
+00000270: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
+00000280: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
+00000290: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
+000002a0: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
+000002b0: 726f 626f 746f 2d61 692f 726f 626f 746f  roboto-ai/roboto
+000002c0: 2d68 6f73 7465 642d 6170 702f 7061 636b  -hosted-app/pack
+000002d0: 6167 6573 2f72 6f62 6f74 6f2f 7372 632f  ages/roboto/src/
+000002e0: 726f 626f 746f 2f63 6c69 2f64 6174 6173  roboto/cli/datas
+000002f0: 6574 732f 6c69 7374 5f66 696c 6573 2e70  ets/list_files.p
+00000300: 7972 1100 0000 0b00 0000 7312 0000 0004  yr........s.....
+00000310: 0104 0104 0104 0104 0104 fc14 0716 0104  ................
+00000320: ff72 1100 0000 6301 0000 0000 0000 0000  .r....c.........
+00000330: 0000 0001 0000 0007 0000 0043 0000 0073  ...........C...s
+00000340: 4000 0000 7c00 6a00 6401 6402 7401 6403  @...|.j.d.d.t.d.
+00000350: 7402 6404 8d05 0100 7c00 6a00 6405 6406  t.d.....|.j.d.d.
+00000360: 7401 6407 6408 6409 8d05 0100 7c00 6a00  t.d.d.d.....|.j.
+00000370: 640a 640b 7401 6407 640c 6409 8d05 0100  d.d.t.d.d.d.....
+00000380: 6400 5300 290d 4e7a 022d 647a 0c2d 2d64  d.S.).Nz.-dz.--d
+00000390: 6174 6173 6574 2d69 6454 2903 da04 7479  ataset-idT)...ty
+000003a0: 7065 da08 7265 7175 6972 6564 da04 6865  pe..required..he
+000003b0: 6c70 7a02 2d69 7a09 2d2d 696e 636c 7564  lpz.-iz.--includ
+000003c0: 65da 012a 7a3c 5a65 726f 206f 7220 6d6f  e..*z<Zero or mo
+000003d0: 7265 2069 6e63 6c75 6465 2066 696c 7465  re include filte
+000003e0: 7273 2028 6966 2070 6174 6820 706f 696e  rs (if path poin
+000003f0: 7473 2074 6f20 6120 6469 7265 6374 6f72  ts to a director
+00000400: 7929 2903 721d 0000 00da 056e 6172 6773  y)).r......nargs
+00000410: 721f 0000 007a 022d 787a 092d 2d65 7863  r....z.-xz.--exc
+00000420: 6c75 6465 7a3c 5a65 726f 206f 7220 6d6f  ludez<Zero or mo
+00000430: 7265 2065 7863 6c75 6465 2066 696c 7465  re exclude filte
+00000440: 7273 2028 6966 2070 6174 6820 706f 696e  rs (if path poin
+00000450: 7473 2074 6f20 6120 6469 7265 6374 6f72  ts to a director
+00000460: 7929 2903 da0c 6164 645f 6172 6775 6d65  y))...add_argume
+00000470: 6e74 da03 7374 7272 0800 0000 2901 720a  nt..strr....).r.
+00000480: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000490: 0000 da17 6c69 7374 5f66 696c 6573 5f73  ....list_files_s
+000004a0: 6574 7570 5f70 6172 7365 7217 0000 0073  etup_parser....s
+000004b0: 2200 0000 0401 0a01 06ff 0403 0201 0201  "...............
+000004c0: 0201 0201 0201 06fb 0407 0201 0201 0201  ................
+000004d0: 0201 0201 0afb 7224 0000 007a 0a6c 6973  ......r$...z.lis
+000004e0: 742d 6669 6c65 7372 1f00 0000 7a23 4c69  t-filesr....z#Li
+000004f0: 7374 7320 6669 6c65 7320 666f 7220 6120  sts files for a 
+00000500: 7370 6563 6966 6963 2064 6174 6173 6574  specific dataset
+00000510: 2e29 04da 046e 616d 65da 056c 6f67 6963  .)...name..logic
+00000520: da0c 7365 7475 705f 7061 7273 6572 da0e  ..setup_parser..
+00000530: 636f 6d6d 616e 645f 6b77 6172 6773 290e  command_kwargs).
+00000540: da08 6172 6770 6172 7365 7214 0000 00da  ..argparser.....
+00000550: 0f64 6f6d 6169 6e2e 6461 7461 7365 7473  .domain.datasets
+00000560: 7203 0000 00da 0763 6f6d 6d61 6e64 7205  r......commandr.
+00000570: 0000 0072 0900 0000 7206 0000 00da 0e73  ...r....r......s
+00000580: 6861 7265 645f 6865 6c70 646f 6372 0800  hared_helpdocr..
+00000590: 0000 da0e 4172 6775 6d65 6e74 5061 7273  ....ArgumentPars
+000005a0: 6572 7211 0000 0072 2400 0000 da12 6c69  err....r$.....li
+000005b0: 7374 5f66 696c 6573 5f63 6f6d 6d61 6e64  st_files_command
+000005c0: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+000005d0: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000005e0: 0000 731c 0000 0008 0108 010c 020c 010c  ..s.............
+000005f0: 010c 0114 0308 0c02 1402 0102 0102 0106  ................
+00000600: 010a fc                                  ...
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/__pycache__/search.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/datasets/__pycache__/search.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2566 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 060a 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 060a 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6404 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6405 6406 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
@@ -50,16 +50,16 @@
 00000310: 01da 066f 7267 5f69 6463 0100 0000 0000  ...org_idc......
 00000320: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
 00000330: 0000 7314 0000 0067 007c 005d 067d 017c  ..s....g.|.].}.|
 00000340: 01a0 00a1 0091 0271 0253 00a9 0029 01da  .......q.S...)..
 00000350: 0774 6f5f 6469 6374 2902 da02 2e30 da06  .to_dict)....0..
 00000360: 7265 636f 7264 721b 0000 0072 1b00 0000  recordr....r....
 00000370: fae3 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-00000380: 7075 742f 7372 6331 3035 3131 3832 3038  put/src105118208
-00000390: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+00000380: 7075 742f 7372 6333 3037 3932 3336 3236  put/src307923626
+00000390: 342f 7372 632f 636f 6465 7374 6172 2d63  4/src/codestar-c
 000003a0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 000003b0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 000003c0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 000003d0: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 000003e0: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 000003f0: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000400: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/__pycache__/show.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/datasets/__pycache__/delete_dataset.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 903 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,79 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 8703 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 7e03 0000  o.......2H.e~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
-00000040: 6403 6c02 6d03 5a03 0100 6404 6405 6c04  d.l.m.Z...d.d.l.
-00000050: 6d05 5a05 0100 6404 6406 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6404 6407 6c08 6d09 5a09 0100 6408  ..d.d.l.m.Z...d.
-00000070: 6409 6c0a 6d0b 5a0b 0100 640a 6509 640b  d.l.m.Z...d.e.d.
-00000080: 6500 6a0c 6604 640c 640d 8404 5a0d 640e  e.j.f.d.d...Z.d.
-00000090: 640f 8400 5a0e 6505 640d 650d 650e 6410  d...Z.e.d.e.e.d.
-000000a0: 6411 6901 6412 8d04 5a0f 6401 5300 2913  d.i.d...Z.d.S.).
-000000b0: e900 0000 004e e903 0000 0029 01da 0744  .....N.....)...D
-000000c0: 6174 6173 6574 e902 0000 0029 01da 0d52  ataset.....)...R
-000000d0: 6f62 6f74 6f43 6f6d 6d61 6e64 2901 da0b  obotoCommand)...
-000000e0: 6164 645f 6f72 675f 6172 6729 01da 0a43  add_org_arg)...C
-000000f0: 4c49 436f 6e74 6578 74e9 0100 0000 2901  LIContext.....).
-00000100: da0f 4441 5441 5345 545f 4944 5f48 454c  ..DATASET_ID_HEL
-00000110: 50da 0763 6f6e 7465 7874 da06 7061 7273  P..context..pars
-00000120: 6572 6303 0000 0000 0000 0000 0000 0004  erc.............
-00000130: 0000 0007 0000 0043 0000 0073 3800 0000  .......C...s8...
-00000140: 7400 6a01 7c00 6a02 7c01 6a03 7c01 6a04  t.j.|.j.|.j.|.j.
-00000150: 7c01 6a05 7c00 6a06 6401 8d05 7d03 7407  |.j.|.j.d...}.t.
-00000160: 7408 6a09 7c03 a00a a100 6402 6403 8d02  t.j.|.....d.d...
-00000170: 8301 0100 6400 5300 2904 4e29 01da 066f  ....d.S.).N)...o
-00000180: 7267 5f69 64e9 0400 0000 2901 da06 696e  rg_id.....)...in
-00000190: 6465 6e74 290b 7203 0000 00da 0766 726f  dent).r......fro
-000001a0: 6d5f 6964 da0a 6461 7461 7365 745f 6964  m_id..dataset_id
-000001b0: da08 6461 7461 7365 7473 da05 6669 6c65  ..datasets..file
-000001c0: 73da 1374 7261 6e73 6163 7469 6f6e 5f6d  s..transaction_m
-000001d0: 616e 6167 6572 da03 6f72 67da 0570 7269  anager..org..pri
-000001e0: 6e74 da04 6a73 6f6e da05 6475 6d70 73da  nt..json..dumps.
-000001f0: 0774 6f5f 6469 6374 2904 da04 6172 6773  .to_dict)...args
-00000200: 720a 0000 0072 0b00 0000 da06 7265 636f  r....r......reco
-00000210: 7264 a900 721b 0000 00fa e12f 636f 6465  rd..r....../code
-00000220: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000230: 3130 3531 3138 3230 3839 2f73 7263 2f63  1051182089/src/c
-00000240: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
-00000250: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
-00000260: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
-00000270: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
-00000280: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
-00000290: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
-000002a0: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
-000002b0: 2f72 6f62 6f74 6f2d 6169 2f72 6f62 6f74  /roboto-ai/robot
-000002c0: 6f2d 686f 7374 6564 2d61 7070 2f70 6163  o-hosted-app/pac
-000002d0: 6b61 6765 732f 726f 626f 746f 2f73 7263  kages/roboto/src
-000002e0: 2f72 6f62 6f74 6f2f 636c 692f 6461 7461  /roboto/cli/data
-000002f0: 7365 7473 2f73 686f 772e 7079 da04 7368  sets/show.py..sh
-00000300: 6f77 0c00 0000 7310 0000 0004 0104 0104  ow....s.........
-00000310: 0104 0104 0104 0106 fb1a 0772 1d00 0000  ...........r....
-00000320: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000330: 0007 0000 0043 0000 0073 2000 0000 7c00  .....C...s ...|.
-00000340: 6a00 6401 6402 7401 6403 7402 6404 8d05  j.d.d.t.d.t.d...
-00000350: 0100 7403 7c00 8301 0100 6400 5300 2905  ..t.|.....d.S.).
-00000360: 4e7a 022d 647a 0c2d 2d64 6174 6173 6574  Nz.-dz.--dataset
-00000370: 2d69 6454 2903 da04 7479 7065 da08 7265  -idT)...type..re
-00000380: 7175 6972 6564 da04 6865 6c70 2904 da0c  quired..help)...
-00000390: 6164 645f 6172 6775 6d65 6e74 da03 7374  add_argument..st
-000003a0: 7272 0900 0000 7206 0000 0029 0172 0b00  rr....r....).r..
-000003b0: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-000003c0: 00da 1173 686f 775f 7365 7475 705f 7061  ...show_setup_pa
-000003d0: 7273 6572 1700 0000 7308 0000 0004 010a  rser....s.......
-000003e0: 0106 ff0c 0372 2300 0000 7220 0000 007a  .....r#...r ...z
-000003f0: 2a53 686f 7720 696e 666f 726d 6174 696f  *Show informatio
-00000400: 6e20 6162 6f75 7420 6120 7370 6563 6966  n about a specif
-00000410: 6963 2064 6174 6173 6574 2e29 04da 046e  ic dataset.)...n
-00000420: 616d 65da 056c 6f67 6963 da0c 7365 7475  ame..logic..setu
-00000430: 705f 7061 7273 6572 da0e 636f 6d6d 616e  p_parser..comman
-00000440: 645f 6b77 6172 6773 2910 da08 6172 6770  d_kwargs)...argp
-00000450: 6172 7365 7216 0000 00da 0f64 6f6d 6169  arser......domai
-00000460: 6e2e 6461 7461 7365 7473 7203 0000 00da  n.datasetsr.....
-00000470: 0763 6f6d 6d61 6e64 7205 0000 00da 0b63  .commandr......c
-00000480: 6f6d 6d6f 6e5f 6172 6773 7206 0000 0072  ommon_argsr....r
-00000490: 0a00 0000 7207 0000 00da 0e73 6861 7265  ....r......share
-000004a0: 645f 6865 6c70 646f 6372 0900 0000 da0e  d_helpdocr......
-000004b0: 4172 6775 6d65 6e74 5061 7273 6572 721d  ArgumentParserr.
-000004c0: 0000 0072 2300 0000 da0c 7368 6f77 5f63  ...r#.....show_c
-000004d0: 6f6d 6d61 6e64 721b 0000 0072 1b00 0000  ommandr....r....
-000004e0: 721b 0000 0072 1c00 0000 da08 3c6d 6f64  r....r......<mod
-000004f0: 756c 653e 0100 0000 731e 0000 0008 0108  ule>....s.......
-00000500: 010c 020c 010c 010c 010c 0114 0308 0b02  ................
-00000510: 0702 0102 0102 0106 010a fc              ...........
+00000020: 0006 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
+00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
+00000050: 6406 6c05 6d06 5a06 0100 6407 6408 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6409 6506 640a 6500 6a09  m.Z...d.e.d.e.j.
+00000070: 6604 640b 640c 8404 5a0a 640d 640e 8400  f.d.d...Z.d.d...
+00000080: 5a0b 6504 640f 650a 650b 6410 6411 6901  Z.e.d.e.e.d.d.i.
+00000090: 6412 8d04 5a0c 6401 5300 2913 e900 0000  d...Z.d.S.).....
+000000a0: 004e e903 0000 0029 01da 0744 6174 6173  .N.....)...Datas
+000000b0: 6574 e902 0000 0029 01da 0d52 6f62 6f74  et.....)...Robot
+000000c0: 6f43 6f6d 6d61 6e64 2901 da0a 434c 4943  oCommand)...CLIC
+000000d0: 6f6e 7465 7874 e901 0000 0029 01da 0f44  ontext.....)...D
+000000e0: 4154 4153 4554 5f49 445f 4845 4c50 da07  ATASET_ID_HELP..
+000000f0: 636f 6e74 6578 74da 0670 6172 7365 7263  context..parserc
+00000100: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+00000110: 0600 0000 4300 0000 7334 0000 0074 00a0  ....C...s4...t..
+00000120: 017c 006a 027c 016a 037c 016a 047c 016a  .|.j.|.j.|.j.|.j
+00000130: 05a1 047d 037c 03a0 06a1 0001 0074 0764  ...}.|.......t.d
+00000140: 017c 006a 029b 009d 0283 0101 0064 0053  .|.j.........d.S
+00000150: 0029 024e 7a10 4465 6c65 7465 6420 6461  .).Nz.Deleted da
+00000160: 7461 7365 7420 2908 7203 0000 00da 0766  taset ).r......f
+00000170: 726f 6d5f 6964 da0a 6461 7461 7365 745f  rom_id..dataset_
+00000180: 6964 da08 6461 7461 7365 7473 da05 6669  id..datasets..fi
+00000190: 6c65 73da 1374 7261 6e73 6163 7469 6f6e  les..transaction
+000001a0: 5f6d 616e 6167 6572 da0e 6465 6c65 7465  _manager..delete
+000001b0: 5f64 6174 6173 6574 da05 7072 696e 7429  _dataset..print)
+000001c0: 04da 0461 7267 7372 0900 0000 720a 0000  ...argsr....r...
+000001d0: 00da 0764 6174 6173 6574 a900 7214 0000  ...dataset..r...
+000001e0: 00fa eb2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
+000001f0: 7470 7574 2f73 7263 3330 3739 3233 3632  tput/src30792362
+00000200: 3634 2f73 7263 2f63 6f64 6573 7461 722d  64/src/codestar-
+00000210: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
+00000220: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
+00000230: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
+00000240: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
+00000250: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
+00000260: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
+00000270: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
+00000280: 6169 2f72 6f62 6f74 6f2d 686f 7374 6564  ai/roboto-hosted
+00000290: 2d61 7070 2f70 6163 6b61 6765 732f 726f  -app/packages/ro
+000002a0: 626f 746f 2f73 7263 2f72 6f62 6f74 6f2f  boto/src/roboto/
+000002b0: 636c 692f 6461 7461 7365 7473 2f64 656c  cli/datasets/del
+000002c0: 6574 655f 6461 7461 7365 742e 7079 7210  ete_dataset.pyr.
+000002d0: 0000 000a 0000 0073 1000 0000 0401 0401  .......s........
+000002e0: 0401 0401 0401 04fc 0806 1401 7210 0000  ............r...
+000002f0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000300: 0000 0700 0000 4300 0000 7318 0000 007c  ......C...s....|
+00000310: 006a 0064 0164 0274 0164 0374 0264 048d  .j.d.d.t.d.t.d..
+00000320: 0501 0064 0053 0029 054e 7a02 2d64 7a0c  ...d.S.).Nz.-dz.
+00000330: 2d2d 6461 7461 7365 742d 6964 5429 03da  --dataset-idT)..
+00000340: 0474 7970 65da 0872 6571 7569 7265 64da  .type..required.
+00000350: 0468 656c 7029 03da 0c61 6464 5f61 7267  .help)...add_arg
+00000360: 756d 656e 74da 0373 7472 7208 0000 0029  ument..strr....)
+00000370: 0172 0a00 0000 7214 0000 0072 1400 0000  .r....r....r....
+00000380: 7215 0000 00da 1b64 656c 6574 655f 6461  r......delete_da
+00000390: 7461 7365 745f 7365 7475 705f 7061 7273  taset_setup_pars
+000003a0: 6572 1500 0000 7306 0000 0004 010a 010a  er....s.........
+000003b0: ff72 1b00 0000 da06 6465 6c65 7465 7218  .r......deleter.
+000003c0: 0000 007a 3444 656c 6574 6520 6461 7461  ...z4Delete data
+000003d0: 7365 7420 2861 6e64 2061 6c6c 2072 656c  set (and all rel
+000003e0: 6174 6564 2073 7562 7265 736f 7572 6365  ated subresource
+000003f0: 7329 2062 7920 6964 2e29 04da 046e 616d  s) by id.)...nam
+00000400: 65da 056c 6f67 6963 da0c 7365 7475 705f  e..logic..setup_
+00000410: 7061 7273 6572 da0e 636f 6d6d 616e 645f  parser..command_
+00000420: 6b77 6172 6773 290d da08 6172 6770 6172  kwargs)...argpar
+00000430: 7365 da0f 646f 6d61 696e 2e64 6174 6173  se..domain.datas
+00000440: 6574 7372 0300 0000 da07 636f 6d6d 616e  etsr......comman
+00000450: 6472 0500 0000 7209 0000 0072 0600 0000  dr....r....r....
+00000460: da0e 7368 6172 6564 5f68 656c 7064 6f63  ..shared_helpdoc
+00000470: 7208 0000 00da 0e41 7267 756d 656e 7450  r......ArgumentP
+00000480: 6172 7365 7272 1000 0000 721b 0000 00da  arserr....r.....
+00000490: 1664 656c 6574 655f 6461 7461 7365 745f  .delete_dataset_
+000004a0: 636f 6d6d 616e 6472 1400 0000 7214 0000  commandr....r...
+000004b0: 0072 1400 0000 7215 0000 00da 083c 6d6f  .r....r......<mo
+000004c0: 6475 6c65 3e01 0000 0073 1a00 0000 0801  dule>....s......
+000004d0: 0c02 0c01 0c01 0c01 1403 080b 0206 0201  ................
+000004e0: 0201 0201 0601 0afc                      ........
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/__pycache__/update.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/datasets/__pycache__/update.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2885 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,171 +1,166 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 450b 0000  o........Y.eE...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 ee0a 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 6402 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6405 6406 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6405 6407 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 6405 6408 6c0b 6d0c 5a0c 0100 6409  ..d.d.l.m.Z...d.
-00000080: 640a 6c0d 6d0e 5a0e 0100 640b 6500 6a0f  d.l.m.Z...d.e.j.
-00000090: 640c 650c 640d 6500 6a10 640e 6401 6608  d.e.d.e.j.d.d.f.
-000000a0: 640f 6410 8404 5a11 640d 6500 6a10 6602  d.d...Z.d.e.j.f.
-000000b0: 6411 6412 8404 5a12 6508 6410 6511 6512  d.d...Z.e.d.e.e.
-000000c0: 6413 6414 6901 6415 8d04 5a13 6401 5300  d.d.i.d...Z.d.S.
-000000d0: 2916 e900 0000 004e e903 0000 0029 01da  )......N.....)..
-000000e0: 0744 6174 6173 6574 2901 da11 4d65 7461  .Dataset)...Meta
-000000f0: 6461 7461 4368 616e 6765 7365 74e9 0200  dataChangeset...
-00000100: 0000 2902 da13 4b65 7956 616c 7565 5061  ..)...KeyValuePa
-00000110: 6972 7341 6374 696f 6eda 0d52 6f62 6f74  irsAction..Robot
-00000120: 6f43 6f6d 6d61 6e64 2901 da0b 6164 645f  oCommand)...add_
-00000130: 6f72 675f 6172 6729 01da 0a43 4c49 436f  org_arg)...CLICo
-00000140: 6e74 6578 74e9 0100 0000 2901 da0f 4441  ntext.....)...DA
-00000150: 5441 5345 545f 4944 5f48 454c 50da 0461  TASET_ID_HELP..a
-00000160: 7267 73da 0763 6f6e 7465 7874 da06 7061  rgs..context..pa
-00000170: 7273 6572 da06 7265 7475 726e 6303 0000  rser..returnc...
-00000180: 0000 0000 0000 0000 0005 0000 0007 0000  ................
-00000190: 0043 0000 0073 8a00 0000 7400 7c00 6a01  .C...s....t.|.j.
-000001a0: 7c00 6a02 7c00 6a03 7c00 6a04 6401 8d04  |.j.|.j.|.j.d...
-000001b0: 7d03 7c03 a005 a100 7218 7c00 6a06 7318  }.|.....r.|.j.s.
-000001c0: 7c02 a007 6402 a101 0100 7408 6a09 7c00  |...d.....t.j.|.
-000001d0: 6a0a 7c01 6a0b 7c01 6a0c 7c01 6a0d 7c00  j.|.j.|.j.|.j.|.
-000001e0: 6a0e 6403 8d05 7d04 7c04 6a0f 7c03 7c00  j.d...}.|.j.|.|.
-000001f0: 6a06 6404 8d02 0100 7410 6405 7c04 6a0a  j.d.....t.d.|.j.
-00000200: 9b00 6406 9d03 8301 0100 7410 7411 6a12  ..d.......t.t.j.
-00000210: 7c04 a013 a100 6407 6408 8d02 8301 0100  |.....d.d.......
-00000220: 6400 5300 2909 4e29 04da 0870 7574 5f74  d.S.).N)...put_t
-00000230: 6167 73da 0b72 656d 6f76 655f 7461 6773  ags..remove_tags
-00000240: da0a 7075 745f 6669 656c 6473 da0d 7265  ..put_fields..re
-00000250: 6d6f 7665 5f66 6965 6c64 737a 1d4e 6f20  move_fieldsz.No 
-00000260: 6461 7461 7365 7420 6368 616e 6765 7320  dataset changes 
-00000270: 7370 6563 6966 6965 642e 2901 da06 6f72  specified.)...or
-00000280: 675f 6964 2902 da12 6d65 7461 6461 7461  g_id)...metadata
-00000290: 5f63 6861 6e67 6573 6574 da0b 6465 7363  _changeset..desc
-000002a0: 7269 7074 696f 6e7a 1e53 7563 6365 7373  riptionz.Success
-000002b0: 6675 6c6c 7920 7570 6461 7465 6420 6461  fully updated da
-000002c0: 7461 7365 7420 277a 0b27 2e20 5265 636f  taset 'z.'. Reco
-000002d0: 7264 3a20 e904 0000 0029 01da 0669 6e64  rd: .....)...ind
-000002e0: 656e 7429 1472 0400 0000 7210 0000 0072  ent).r....r....r
-000002f0: 1100 0000 da0c 7075 745f 6d65 7461 6461  ......put_metada
-00000300: 7461 da0f 7265 6d6f 7665 5f6d 6574 6164  ta..remove_metad
-00000310: 6174 61da 0869 735f 656d 7074 7972 1600  ata..is_emptyr..
-00000320: 0000 da05 6572 726f 7272 0300 0000 da07  ....errorr......
-00000330: 6672 6f6d 5f69 64da 0a64 6174 6173 6574  from_id..dataset
-00000340: 5f69 64da 0864 6174 6173 6574 73da 0566  _id..datasets..f
-00000350: 696c 6573 da13 7472 616e 7361 6374 696f  iles..transactio
-00000360: 6e5f 6d61 6e61 6765 72da 036f 7267 da06  n_manager..org..
-00000370: 7570 6461 7465 da05 7072 696e 74da 046a  update..print..j
-00000380: 736f 6eda 0564 756d 7073 da07 746f 5f64  son..dumps..to_d
-00000390: 6963 7429 0572 0c00 0000 720d 0000 0072  ict).r....r....r
-000003a0: 0e00 0000 7215 0000 00da 0764 6174 6173  ....r......datas
-000003b0: 6574 a900 7229 0000 00fa e32f 636f 6465  et..r)...../code
-000003c0: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-000003d0: 3130 3531 3138 3230 3839 2f73 7263 2f63  1051182089/src/c
-000003e0: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
-000003f0: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
-00000400: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
-00000410: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
-00000420: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
-00000430: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
-00000440: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
-00000450: 2f72 6f62 6f74 6f2d 6169 2f72 6f62 6f74  /roboto-ai/robot
-00000460: 6f2d 686f 7374 6564 2d61 7070 2f70 6163  o-hosted-app/pac
-00000470: 6b61 6765 732f 726f 626f 746f 2f73 7263  kages/roboto/src
-00000480: 2f72 6f62 6f74 6f2f 636c 692f 6461 7461  /roboto/cli/data
-00000490: 7365 7473 2f75 7064 6174 652e 7079 7223  sets/update.pyr#
-000004a0: 0000 0010 0000 0073 2400 0000 0203 0401  .......s$.......
-000004b0: 0401 0401 0401 06fc 0e06 0a01 0402 0401  ................
-000004c0: 0401 0401 0401 0401 06fb 1007 1202 1a01  ................
-000004d0: 7223 0000 0063 0100 0000 0000 0000 0000  r#...c..........
-000004e0: 0000 0100 0000 0800 0000 4300 0000 7378  ..........C...sx
-000004f0: 0000 007c 006a 0064 0164 0274 0164 0374  ...|.j.d.d.t.d.t
-00000500: 0264 048d 0501 0074 037c 0083 0101 007c  .d.....t.|.....|
-00000510: 006a 0064 0564 0664 078d 0201 007c 006a  .j.d.d.d.....|.j
-00000520: 0064 0864 0964 0a64 0b8d 0301 007c 006a  .d.d.d.d.....|.j
-00000530: 0064 0c64 0d64 0a64 0b8d 0301 007c 006a  .d.d.d.d.....|.j
-00000540: 0064 0e64 0f64 1064 0a74 0464 1164 128d  .d.d.d.d.t.d.d..
-00000550: 0601 007c 006a 0064 1364 0f64 1464 0a64  ...|.j.d.d.d.d.d
-00000560: 1564 168d 0501 0064 0053 0029 174e 7a02  .d.....d.S.).Nz.
-00000570: 2d64 7a0c 2d2d 6461 7461 7365 742d 6964  -dz.--dataset-id
-00000580: 5429 03da 0474 7970 65da 0872 6571 7569  T)...type..requi
-00000590: 7265 64da 0468 656c 707a 0d2d 2d64 6573  red..helpz.--des
-000005a0: 6372 6970 7469 6f6e 7a28 4120 6e65 7720  criptionz(A new 
-000005b0: 6465 7363 7269 7074 696f 6e20 746f 2061  description to a
-000005c0: 6464 2074 6f20 7468 6973 2064 6174 6173  dd to this datas
-000005d0: 6574 2901 722d 0000 007a 0a2d 2d70 7574  et).r-...z.--put
-000005e0: 2d74 6167 737a 3141 6464 2065 6163 6820  -tagsz1Add each 
-000005f0: 7461 6720 696e 2074 6869 7320 7365 7175  tag in this sequ
-00000600: 656e 6365 2069 6620 6974 2064 6f65 736e  ence if it doesn
-00000610: 2774 2065 7869 7374 da01 2a29 0272 2d00  't exist..*).r-.
-00000620: 0000 da05 6e61 7267 737a 0d2d 2d72 656d  ....nargsz.--rem
-00000630: 6f76 652d 7461 6773 7a2d 5265 6d6f 7665  ove-tagsz-Remove
-00000640: 2065 6163 6820 7461 6720 696e 2074 6869   each tag in thi
-00000650: 7320 7365 7175 656e 6365 2069 6620 6974  s sequence if it
-00000660: 2065 7869 7374 737a 0e2d 2d70 7574 2d6d   existsz.--put-m
-00000670: 6574 6164 6174 6146 7a0e 4b45 595f 5041  etadataFz.KEY_PA
-00000680: 5448 3d56 414c 5545 6151 0100 005a 6572  TH=VALUEaQ...Zer
-00000690: 6f20 6f72 206d 6f72 6520 276b 6579 5f70  o or more 'key_p
-000006a0: 6174 683d 7661 6c75 6527 2066 6f72 6d61  ath=value' forma
-000006b0: 7474 6564 2070 6169 7273 2e20 416e 2061  tted pairs. An a
-000006c0: 7474 656d 7074 2069 7320 6d61 6465 2074  ttempt is made t
-000006d0: 6f20 7061 7273 6520 6076 616c 7565 6020  o parse `value` 
-000006e0: 6173 204a 534f 4e3b 2069 6620 7468 6973  as JSON; if this
-000006f0: 2066 6169 6c73 2c20 6076 616c 7565 6020   fails, `value` 
-00000700: 6973 2073 746f 7265 6420 6173 2061 2073  is stored as a s
-00000710: 7472 696e 672e 2049 6620 606b 6579 5f70  tring. If `key_p
-00000720: 6174 6860 2061 6c72 6561 6479 2065 7869  ath` already exi
-00000730: 7374 732c 2065 7869 7374 696e 6720 7661  sts, existing va
-00000740: 6c75 6520 7769 6c6c 2062 6520 6f76 6572  lue will be over
-00000750: 7772 6974 7465 6e2e 2044 6f74 206e 6f74  written. Dot not
-00000760: 6174 696f 6e20 6973 2073 7570 706f 7274  ation is support
-00000770: 6564 2066 6f72 206e 6573 7465 6420 6b65  ed for nested ke
-00000780: 7973 2e20 4578 616d 706c 6573 3a20 2d2d  ys. Examples: --
-00000790: 7075 742d 6d65 7461 6461 7461 2027 6b65  put-metadata 'ke
-000007a0: 7931 3d76 616c 7565 3127 2027 6b65 7932  y1=value1' 'key2
-000007b0: 2e73 7562 6b65 7931 3d76 616c 7565 3227  .subkey1=value2'
-000007c0: 2027 6b65 7933 2e73 7562 6c69 7374 313d   'key3.sublist1=
-000007d0: 5b22 6122 2c22 6222 2c22 6322 5d27 2905  ["a","b","c"]').
-000007e0: 722c 0000 00da 076d 6574 6176 6172 722f  r,.....metavarr/
-000007f0: 0000 00da 0661 6374 696f 6e72 2d00 0000  .....actionr-...
-00000800: 7a11 2d2d 7265 6d6f 7665 2d6d 6574 6164  z.--remove-metad
-00000810: 6174 61da 084b 4559 5f50 4154 487a 8852  ata..KEY_PATHz.R
-00000820: 656d 6f76 6520 6561 6368 206b 6579 2066  emove each key f
-00000830: 726f 6d20 6461 7461 7365 7420 6d65 7461  rom dataset meta
-00000840: 6461 7461 2069 6620 6974 2065 7869 7374  data if it exist
-00000850: 732e 2044 6f74 206e 6f74 6174 696f 6e20  s. Dot notation 
-00000860: 6973 2073 7570 706f 7274 6564 2066 6f72  is supported for
-00000870: 206e 6573 7465 6420 6b65 7973 2e20 452e   nested keys. E.
-00000880: 672e 3a20 2d2d 7265 6d6f 7665 2d6d 6574  g.: --remove-met
-00000890: 6164 6174 6120 6b65 7931 206b 6579 322e  adata key1 key2.
-000008a0: 7375 626b 6579 3329 0472 2c00 0000 7230  subkey3).r,...r0
-000008b0: 0000 0072 2f00 0000 722d 0000 0029 05da  ...r/...r-...)..
-000008c0: 0c61 6464 5f61 7267 756d 656e 74da 0373  .add_argument..s
-000008d0: 7472 720b 0000 0072 0800 0000 7206 0000  trr....r....r...
-000008e0: 0029 0172 0e00 0000 7229 0000 0072 2900  .).r....r)...r).
-000008f0: 0000 722a 0000 00da 0d75 7064 6174 655f  ..r*.....update_
-00000900: 7061 7273 6572 2900 0000 7340 0000 0004  parser)...s@....
-00000910: 010a 0106 ff08 0304 0204 0106 ff04 0402  ................
-00000920: 0102 0102 0106 fd04 0602 0102 0102 0106  ................
-00000930: fd04 0602 0102 0102 0102 0102 0102 0206  ................
-00000940: f904 1002 0102 0102 0102 0102 020a fa72  ...............r
-00000950: 3500 0000 722d 0000 007a 1b55 7064 6174  5...r-...z.Updat
-00000960: 6520 616e 2065 7869 7374 696e 6720 6461  e an existing da
-00000970: 7461 7365 742e 2904 da04 6e61 6d65 da05  taset.)...name..
-00000980: 6c6f 6769 63da 0c73 6574 7570 5f70 6172  logic..setup_par
-00000990: 7365 72da 0e63 6f6d 6d61 6e64 5f6b 7761  ser..command_kwa
-000009a0: 7267 7329 14da 0861 7267 7061 7273 6572  rgs)...argparser
-000009b0: 2500 0000 da0f 646f 6d61 696e 2e64 6174  %.....domain.dat
-000009c0: 6173 6574 7372 0300 0000 da07 7570 6461  asetsr......upda
-000009d0: 7465 7372 0400 0000 da07 636f 6d6d 616e  tesr......comman
-000009e0: 6472 0600 0000 7207 0000 00da 0b63 6f6d  dr....r......com
-000009f0: 6d6f 6e5f 6172 6773 7208 0000 0072 0d00  mon_argsr....r..
-00000a00: 0000 7209 0000 00da 0e73 6861 7265 645f  ..r......shared_
-00000a10: 6865 6c70 646f 6372 0b00 0000 da09 4e61  helpdocr......Na
-00000a20: 6d65 7370 6163 65da 0e41 7267 756d 656e  mespace..Argumen
-00000a30: 7450 6172 7365 7272 2300 0000 7235 0000  tParserr#...r5..
-00000a40: 00da 0e75 7064 6174 655f 636f 6d6d 616e  ...update_comman
-00000a50: 6472 2900 0000 7229 0000 0072 2900 0000  dr)...r)...r)...
-00000a60: 722a 0000 00da 083c 6d6f 6475 6c65 3e01  r*.....<module>.
-00000a70: 0000 0073 3000 0000 0801 0801 0c02 0c01  ...s0...........
-00000a80: 1001 0c04 0c01 0c01 0203 0401 02ff 0201  ................
-00000a90: 02ff 0401 02ff 0202 0afe 1019 0232 0201  .............2..
-00000aa0: 0201 0201 0601 0afc                      ........
+00000070: 0100 6408 6409 6c0b 6d0c 5a0c 0100 640a  ..d.d.l.m.Z...d.
+00000080: 6500 6a0d 640b 650a 640c 6500 6a0e 640d  e.j.d.e.d.e.j.d.
+00000090: 6401 6608 640e 640f 8404 5a0f 640c 6500  d.f.d.d...Z.d.e.
+000000a0: 6a0e 6602 6410 6411 8404 5a10 6508 640f  j.f.d.d...Z.e.d.
+000000b0: 650f 6510 6412 6413 6901 6414 8d04 5a11  e.e.d.d.i.d...Z.
+000000c0: 6401 5300 2915 e900 0000 004e e903 0000  d.S.)......N....
+000000d0: 0029 01da 0744 6174 6173 6574 2901 da11  .)...Dataset)...
+000000e0: 4d65 7461 6461 7461 4368 616e 6765 7365  MetadataChangese
+000000f0: 74e9 0200 0000 2902 da13 4b65 7956 616c  t.....)...KeyVal
+00000100: 7565 5061 6972 7341 6374 696f 6eda 0d52  uePairsAction..R
+00000110: 6f62 6f74 6f43 6f6d 6d61 6e64 2901 da0a  obotoCommand)...
+00000120: 434c 4943 6f6e 7465 7874 e901 0000 0029  CLIContext.....)
+00000130: 01da 0f44 4154 4153 4554 5f49 445f 4845  ...DATASET_ID_HE
+00000140: 4c50 da04 6172 6773 da07 636f 6e74 6578  LP..args..contex
+00000150: 74da 0670 6172 7365 72da 0672 6574 7572  t..parser..retur
+00000160: 6e63 0300 0000 0000 0000 0000 0000 0500  nc..............
+00000170: 0000 0600 0000 4300 0000 7384 0000 0074  ......C...s....t
+00000180: 007c 006a 017c 006a 027c 006a 037c 006a  .|.j.|.j.|.j.|.j
+00000190: 0464 018d 047d 037c 03a0 05a1 0072 187c  .d...}.|.....r.|
+000001a0: 006a 0673 187c 02a0 0764 02a1 0101 0074  .j.s.|...d.....t
+000001b0: 08a0 097c 006a 0a7c 016a 0b7c 016a 0c7c  ...|.j.|.j.|.j.|
+000001c0: 016a 0da1 047d 047c 046a 0e7c 037c 006a  .j...}.|.j.|.|.j
+000001d0: 0664 038d 0201 0074 0f64 047c 046a 0a9b  .d.....t.d.|.j..
+000001e0: 0064 059d 0383 0101 0074 0f74 106a 117c  .d.......t.t.j.|
+000001f0: 04a0 12a1 0064 0664 078d 0283 0101 0064  .....d.d.......d
+00000200: 0053 0029 084e 2904 da08 7075 745f 7461  .S.).N)...put_ta
+00000210: 6773 da0b 7265 6d6f 7665 5f74 6167 73da  gs..remove_tags.
+00000220: 0a70 7574 5f66 6965 6c64 73da 0d72 656d  .put_fields..rem
+00000230: 6f76 655f 6669 656c 6473 7a1d 4e6f 2064  ove_fieldsz.No d
+00000240: 6174 6173 6574 2063 6861 6e67 6573 2073  ataset changes s
+00000250: 7065 6369 6669 6564 2e29 02da 126d 6574  pecified.)...met
+00000260: 6164 6174 615f 6368 616e 6765 7365 74da  adata_changeset.
+00000270: 0b64 6573 6372 6970 7469 6f6e 7a1e 5375  .descriptionz.Su
+00000280: 6363 6573 7366 756c 6c79 2075 7064 6174  ccessfully updat
+00000290: 6564 2064 6174 6173 6574 2027 7a0b 272e  ed dataset 'z.'.
+000002a0: 2052 6563 6f72 643a 20e9 0400 0000 2901   Record: .....).
+000002b0: da06 696e 6465 6e74 2913 7204 0000 0072  ..indent).r....r
+000002c0: 0f00 0000 7210 0000 00da 0c70 7574 5f6d  ....r......put_m
+000002d0: 6574 6164 6174 61da 0f72 656d 6f76 655f  etadata..remove_
+000002e0: 6d65 7461 6461 7461 da08 6973 5f65 6d70  metadata..is_emp
+000002f0: 7479 7214 0000 00da 0565 7272 6f72 7203  tyr......errorr.
+00000300: 0000 00da 0766 726f 6d5f 6964 da0a 6461  .....from_id..da
+00000310: 7461 7365 745f 6964 da08 6461 7461 7365  taset_id..datase
+00000320: 7473 da05 6669 6c65 73da 1374 7261 6e73  ts..files..trans
+00000330: 6163 7469 6f6e 5f6d 616e 6167 6572 da06  action_manager..
+00000340: 7570 6461 7465 da05 7072 696e 74da 046a  update..print..j
+00000350: 736f 6eda 0564 756d 7073 da07 746f 5f64  son..dumps..to_d
+00000360: 6963 7429 0572 0b00 0000 720c 0000 0072  ict).r....r....r
+00000370: 0d00 0000 7213 0000 00da 0764 6174 6173  ....r......datas
+00000380: 6574 a900 7226 0000 00fa e32f 636f 6465  et..r&...../code
+00000390: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
+000003a0: 3330 3739 3233 3632 3634 2f73 7263 2f63  3079236264/src/c
+000003b0: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
+000003c0: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
+000003d0: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
+000003e0: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
+000003f0: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
+00000400: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
+00000410: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
+00000420: 2f72 6f62 6f74 6f2d 6169 2f72 6f62 6f74  /roboto-ai/robot
+00000430: 6f2d 686f 7374 6564 2d61 7070 2f70 6163  o-hosted-app/pac
+00000440: 6b61 6765 732f 726f 626f 746f 2f73 7263  kages/roboto/src
+00000450: 2f72 6f62 6f74 6f2f 636c 692f 6461 7461  /roboto/cli/data
+00000460: 7365 7473 2f75 7064 6174 652e 7079 7220  sets/update.pyr 
+00000470: 0000 000f 0000 0073 2200 0000 0203 0401  .......s".......
+00000480: 0401 0401 0401 06fc 0e06 0a01 0402 0401  ................
+00000490: 0401 0401 0401 04fc 1006 1202 1a01 7220  ..............r 
+000004a0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000004b0: 0100 0000 0800 0000 4300 0000 7370 0000  ........C...sp..
+000004c0: 007c 006a 0064 0164 0274 0164 0374 0264  .|.j.d.d.t.d.t.d
+000004d0: 048d 0501 007c 006a 0064 0564 0664 078d  .....|.j.d.d.d..
+000004e0: 0201 007c 006a 0064 0864 0964 0a64 0b8d  ...|.j.d.d.d.d..
+000004f0: 0301 007c 006a 0064 0c64 0d64 0a64 0b8d  ...|.j.d.d.d.d..
+00000500: 0301 007c 006a 0064 0e64 0f64 1064 0a74  ...|.j.d.d.d.d.t
+00000510: 0364 1164 128d 0601 007c 006a 0064 1364  .d.d.....|.j.d.d
+00000520: 0f64 1464 0a64 1564 168d 0501 0064 0053  .d.d.d.d.....d.S
+00000530: 0029 174e 7a02 2d64 7a0c 2d2d 6461 7461  .).Nz.-dz.--data
+00000540: 7365 742d 6964 5429 03da 0474 7970 65da  set-idT)...type.
+00000550: 0872 6571 7569 7265 64da 0468 656c 707a  .required..helpz
+00000560: 0d2d 2d64 6573 6372 6970 7469 6f6e 7a28  .--descriptionz(
+00000570: 4120 6e65 7720 6465 7363 7269 7074 696f  A new descriptio
+00000580: 6e20 746f 2061 6464 2074 6f20 7468 6973  n to add to this
+00000590: 2064 6174 6173 6574 2901 722a 0000 007a   dataset).r*...z
+000005a0: 0a2d 2d70 7574 2d74 6167 737a 3141 6464  .--put-tagsz1Add
+000005b0: 2065 6163 6820 7461 6720 696e 2074 6869   each tag in thi
+000005c0: 7320 7365 7175 656e 6365 2069 6620 6974  s sequence if it
+000005d0: 2064 6f65 736e 2774 2065 7869 7374 da01   doesn't exist..
+000005e0: 2a29 0272 2a00 0000 da05 6e61 7267 737a  *).r*.....nargsz
+000005f0: 0d2d 2d72 656d 6f76 652d 7461 6773 7a2d  .--remove-tagsz-
+00000600: 5265 6d6f 7665 2065 6163 6820 7461 6720  Remove each tag 
+00000610: 696e 2074 6869 7320 7365 7175 656e 6365  in this sequence
+00000620: 2069 6620 6974 2065 7869 7374 737a 0e2d   if it existsz.-
+00000630: 2d70 7574 2d6d 6574 6164 6174 6146 7a0e  -put-metadataFz.
+00000640: 4b45 595f 5041 5448 3d56 414c 5545 6151  KEY_PATH=VALUEaQ
+00000650: 0100 005a 6572 6f20 6f72 206d 6f72 6520  ...Zero or more 
+00000660: 276b 6579 5f70 6174 683d 7661 6c75 6527  'key_path=value'
+00000670: 2066 6f72 6d61 7474 6564 2070 6169 7273   formatted pairs
+00000680: 2e20 416e 2061 7474 656d 7074 2069 7320  . An attempt is 
+00000690: 6d61 6465 2074 6f20 7061 7273 6520 6076  made to parse `v
+000006a0: 616c 7565 6020 6173 204a 534f 4e3b 2069  alue` as JSON; i
+000006b0: 6620 7468 6973 2066 6169 6c73 2c20 6076  f this fails, `v
+000006c0: 616c 7565 6020 6973 2073 746f 7265 6420  alue` is stored 
+000006d0: 6173 2061 2073 7472 696e 672e 2049 6620  as a string. If 
+000006e0: 606b 6579 5f70 6174 6860 2061 6c72 6561  `key_path` alrea
+000006f0: 6479 2065 7869 7374 732c 2065 7869 7374  dy exists, exist
+00000700: 696e 6720 7661 6c75 6520 7769 6c6c 2062  ing value will b
+00000710: 6520 6f76 6572 7772 6974 7465 6e2e 2044  e overwritten. D
+00000720: 6f74 206e 6f74 6174 696f 6e20 6973 2073  ot notation is s
+00000730: 7570 706f 7274 6564 2066 6f72 206e 6573  upported for nes
+00000740: 7465 6420 6b65 7973 2e20 4578 616d 706c  ted keys. Exampl
+00000750: 6573 3a20 2d2d 7075 742d 6d65 7461 6461  es: --put-metada
+00000760: 7461 2027 6b65 7931 3d76 616c 7565 3127  ta 'key1=value1'
+00000770: 2027 6b65 7932 2e73 7562 6b65 7931 3d76   'key2.subkey1=v
+00000780: 616c 7565 3227 2027 6b65 7933 2e73 7562  alue2' 'key3.sub
+00000790: 6c69 7374 313d 5b22 6122 2c22 6222 2c22  list1=["a","b","
+000007a0: 6322 5d27 2905 7229 0000 00da 076d 6574  c"]').r).....met
+000007b0: 6176 6172 722c 0000 00da 0661 6374 696f  avarr,.....actio
+000007c0: 6e72 2a00 0000 7a11 2d2d 7265 6d6f 7665  nr*...z.--remove
+000007d0: 2d6d 6574 6164 6174 61da 084b 4559 5f50  -metadata..KEY_P
+000007e0: 4154 487a 8852 656d 6f76 6520 6561 6368  ATHz.Remove each
+000007f0: 206b 6579 2066 726f 6d20 6461 7461 7365   key from datase
+00000800: 7420 6d65 7461 6461 7461 2069 6620 6974  t metadata if it
+00000810: 2065 7869 7374 732e 2044 6f74 206e 6f74   exists. Dot not
+00000820: 6174 696f 6e20 6973 2073 7570 706f 7274  ation is support
+00000830: 6564 2066 6f72 206e 6573 7465 6420 6b65  ed for nested ke
+00000840: 7973 2e20 452e 672e 3a20 2d2d 7265 6d6f  ys. E.g.: --remo
+00000850: 7665 2d6d 6574 6164 6174 6120 6b65 7931  ve-metadata key1
+00000860: 206b 6579 322e 7375 626b 6579 3329 0472   key2.subkey3).r
+00000870: 2900 0000 722d 0000 0072 2c00 0000 722a  )...r-...r,...r*
+00000880: 0000 0029 04da 0c61 6464 5f61 7267 756d  ...)...add_argum
+00000890: 656e 74da 0373 7472 720a 0000 0072 0600  ent..strr....r..
+000008a0: 0000 2901 720d 0000 0072 2600 0000 7226  ..).r....r&...r&
+000008b0: 0000 0072 2700 0000 da0d 7570 6461 7465  ...r'.....update
+000008c0: 5f70 6172 7365 7227 0000 0073 3e00 0000  _parser'...s>...
+000008d0: 0401 0a01 06ff 0404 0401 06ff 0404 0201  ................
+000008e0: 0201 0201 06fd 0406 0201 0201 0201 06fd  ................
+000008f0: 0406 0201 0201 0201 0201 0201 0202 06f9  ................
+00000900: 0410 0201 0201 0201 0201 0202 0afa 7232  ..............r2
+00000910: 0000 0072 2a00 0000 7a1b 5570 6461 7465  ...r*...z.Update
+00000920: 2061 6e20 6578 6973 7469 6e67 2064 6174   an existing dat
+00000930: 6173 6574 2e29 04da 046e 616d 65da 056c  aset.)...name..l
+00000940: 6f67 6963 da0c 7365 7475 705f 7061 7273  ogic..setup_pars
+00000950: 6572 da0e 636f 6d6d 616e 645f 6b77 6172  er..command_kwar
+00000960: 6773 2912 da08 6172 6770 6172 7365 7222  gs)...argparser"
+00000970: 0000 00da 0f64 6f6d 6169 6e2e 6461 7461  .....domain.data
+00000980: 7365 7473 7203 0000 00da 0775 7064 6174  setsr......updat
+00000990: 6573 7204 0000 00da 0763 6f6d 6d61 6e64  esr......command
+000009a0: 7206 0000 0072 0700 0000 720c 0000 0072  r....r....r....r
+000009b0: 0800 0000 da0e 7368 6172 6564 5f68 656c  ......shared_hel
+000009c0: 7064 6f63 720a 0000 00da 094e 616d 6573  pdocr......Names
+000009d0: 7061 6365 da0e 4172 6775 6d65 6e74 5061  pace..ArgumentPa
+000009e0: 7273 6572 7220 0000 0072 3200 0000 da0e  rserr ...r2.....
+000009f0: 7570 6461 7465 5f63 6f6d 6d61 6e64 7226  update_commandr&
+00000a00: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
+00000a10: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000a20: 732e 0000 0008 0108 010c 020c 0110 010c  s...............
+00000a30: 040c 0102 0304 0102 ff02 0102 ff04 0102  ................
+00000a40: ff02 020a fe10 1802 3102 0102 0102 0106  ........1.......
+00000a50: 010a fc                                  ...
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/__pycache__/upload_files.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/datasets/__pycache__/upload_files.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2083 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,133 +1,127 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 2308 0000  o........Y.e#...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 cc07 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 6404 6405 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6404 6406 6c07  m.Z.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6404 6407 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 6408 6409 6c0b 6d0c 5a0c 0100 640a  ..d.d.l.m.Z...d.
-00000080: 650a 640b 6500 6a0d 6604 640c 640d 8404  e.d.e.j.f.d.d...
-00000090: 5a0e 640e 640f 8400 5a0f 6506 6410 650e  Z.d.d...Z.e.d.e.
-000000a0: 650f 6411 6412 6901 6413 8d04 5a10 6401  e.d.d.i.d...Z.d.
-000000b0: 5300 2914 e900 0000 004e e903 0000 0029  S.)......N.....)
-000000c0: 01da 0744 6174 6173 6574 e902 0000 0029  ...Dataset.....)
-000000d0: 02da 1345 7869 7374 696e 6750 6174 686c  ...ExistingPathl
-000000e0: 6962 5061 7468 da0d 526f 626f 746f 436f  ibPath..RobotoCo
-000000f0: 6d6d 616e 6429 01da 0b61 6464 5f6f 7267  mmand)...add_org
-00000100: 5f61 7267 2901 da0a 434c 4943 6f6e 7465  _arg)...CLIConte
-00000110: 7874 e901 0000 0029 01da 0f44 4154 4153  xt.....)...DATAS
-00000120: 4554 5f49 445f 4845 4c50 da07 636f 6e74  ET_ID_HELP..cont
-00000130: 6578 74da 0670 6172 7365 7263 0300 0000  ext..parserc....
-00000140: 0000 0000 0000 0000 0600 0000 0700 0000  ................
-00000150: 4300 0000 739e 0000 007c 006a 007d 037c  C...s....|.j.}.|
-00000160: 006a 0164 0075 0172 117c 03a0 02a1 0073  .j.d.u.r.|.....s
-00000170: 117c 02a0 0364 01a1 0101 007c 006a 0464  .|...d.....|.j.d
-00000180: 0075 0172 1f7c 03a0 02a1 0072 1f7c 02a0  .u.r.|.....r.|..
-00000190: 0364 02a1 0101 0074 056a 067c 006a 077c  .d.....t.j.|.j.|
-000001a0: 016a 087c 016a 097c 016a 0a7c 006a 0b64  .j.|.j.|.j.|.j.d
-000001b0: 038d 057d 047c 03a0 02a1 0072 3c7c 046a  ...}.|.....r<|.j
-000001c0: 0c7c 037c 006a 0164 048d 0201 0064 0053  .|.|.j.d.....d.S
-000001d0: 007c 006a 0464 0075 0072 447c 036a 0d6e  .|.j.d.u.rD|.j.n
-000001e0: 027c 006a 047d 057c 04a0 0e7c 037c 05a1  .|.j.}.|...|.|..
-000001f0: 0201 0064 0053 0029 054e 7a4b 4578 636c  ...d.S.).NzKExcl
-00000200: 7564 6520 6669 6c74 6572 7320 6172 6520  ude filters are 
-00000210: 6f6e 6c79 2073 7570 706f 7274 6564 2066  only supported f
-00000220: 6f72 2064 6972 6563 746f 7279 2075 706c  or directory upl
-00000230: 6f61 6473 2c20 6e6f 7420 7369 6e67 6c65  oads, not single
-00000240: 2066 696c 6573 2e7a 4a4b 6579 206f 7665   files.zJKey ove
-00000250: 7272 6964 6573 2061 7265 206f 6e6c 7920  rrides are only 
-00000260: 7375 7070 6f72 7465 6420 666f 7220 7369  supported for si
-00000270: 6e67 6c65 2066 696c 6520 7570 6c6f 6164  ngle file upload
-00000280: 732c 206e 6f77 2064 6972 6563 746f 7269  s, now directori
-00000290: 6573 2e29 01da 066f 7267 5f69 6429 02da  es.)...org_id)..
-000002a0: 0e64 6972 6563 746f 7279 5f70 6174 68da  .directory_path.
-000002b0: 1065 7863 6c75 6465 5f70 6174 7465 726e  .exclude_pattern
-000002c0: 7329 0fda 0470 6174 68da 0765 7863 6c75  s)...path..exclu
-000002d0: 6465 da06 6973 5f64 6972 da05 6572 726f  de..is_dir..erro
-000002e0: 72da 036b 6579 7203 0000 00da 0766 726f  r..keyr......fro
-000002f0: 6d5f 6964 da0a 6461 7461 7365 745f 6964  m_id..dataset_id
-00000300: da08 6461 7461 7365 7473 da05 6669 6c65  ..datasets..file
-00000310: 73da 1374 7261 6e73 6163 7469 6f6e 5f6d  s..transaction_m
-00000320: 616e 6167 6572 da03 6f72 67da 1075 706c  anager..org..upl
-00000330: 6f61 645f 6469 7265 6374 6f72 79da 046e  oad_directory..n
-00000340: 616d 65da 0b75 706c 6f61 645f 6669 6c65  ame..upload_file
-00000350: 2906 da04 6172 6773 720b 0000 0072 0c00  )...argsr....r..
-00000360: 0000 7210 0000 00da 0764 6174 6173 6574  ..r......dataset
-00000370: 7214 0000 00a9 0072 2000 0000 fae9 2f63  r......r ...../c
-00000380: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000390: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
-000003a0: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
-000003b0: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
-000003c0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
-000003d0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
-000003e0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
-000003f0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
-00000400: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
-00000410: 3939 642f 726f 626f 746f 2d61 692f 726f  99d/roboto-ai/ro
-00000420: 626f 746f 2d68 6f73 7465 642d 6170 702f  boto-hosted-app/
-00000430: 7061 636b 6167 6573 2f72 6f62 6f74 6f2f  packages/roboto/
-00000440: 7372 632f 726f 626f 746f 2f63 6c69 2f64  src/roboto/cli/d
-00000450: 6174 6173 6574 732f 7570 6c6f 6164 5f66  atasets/upload_f
-00000460: 696c 6573 2e70 79da 0c75 706c 6f61 645f  iles.py..upload_
-00000470: 6669 6c65 730f 0000 0073 2800 0000 0601  files....s(.....
-00000480: 1201 0401 0201 04ff 1203 0401 0201 04ff  ................
-00000490: 0404 0401 0401 0401 0401 0401 06fb 0808  ................
-000004a0: 1401 1602 1001 7222 0000 0063 0100 0000  ......r"...c....
-000004b0: 0000 0000 0000 0000 0100 0000 0700 0000  ................
-000004c0: 4300 0000 735a 0000 007c 006a 0064 0164  C...sZ...|.j.d.d
-000004d0: 0274 0164 0374 0264 048d 0501 007c 006a  .t.d.t.d.....|.j
-000004e0: 0064 0564 0674 0164 0764 088d 0401 007c  .d.d.t.d.d.....|
-000004f0: 006a 0064 0964 0a74 0364 0364 0b64 048d  .j.d.d.t.d.d.d..
-00000500: 0501 007c 006a 0064 0c64 0d74 0164 0e64  ...|.j.d.d.t.d.d
-00000510: 0f64 108d 0501 0074 047c 0083 0101 0064  .d.....t.|.....d
-00000520: 0053 0029 114e 7a02 2d64 7a0c 2d2d 6461  .S.).Nz.-dz.--da
-00000530: 7461 7365 742d 6964 5429 03da 0474 7970  taset-idT)...typ
-00000540: 65da 0872 6571 7569 7265 64da 0468 656c  e..required..hel
-00000550: 707a 022d 6b7a 052d 2d6b 6579 7a54 4120  pz.-kz.--keyzTA 
-00000560: 6b65 7920 746f 2061 6c69 6173 2061 2066  key to alias a f
-00000570: 696c 6520 746f 2077 6865 6e20 7374 6f72  ile to when stor
-00000580: 696e 6720 6974 2074 6f20 6120 6461 7461  ing it to a data
-00000590: 7365 742e 2044 6f65 7320 6e6f 7468 696e  set. Does nothin
-000005a0: 6720 666f 7220 6469 7265 6374 6f72 6965  g for directorie
-000005b0: 732e 2902 7223 0000 0072 2500 0000 7a02  s.).r#...r%...z.
-000005c0: 2d70 7a06 2d2d 7061 7468 7a2a 5468 6520  -pz.--pathz*The 
-000005d0: 7061 7468 2074 6f20 6120 6669 6c65 206f  path to a file o
-000005e0: 7220 6469 7265 6374 6f72 7920 746f 2075  r directory to u
-000005f0: 706c 6f61 642e 7a02 2d78 7a09 2d2d 6578  pload.z.-xz.--ex
-00000600: 636c 7564 65da 012a 7a3c 5a65 726f 206f  clude..*z<Zero o
-00000610: 7220 6d6f 7265 2065 7863 6c75 6465 2066  r more exclude f
-00000620: 696c 7465 7273 2028 6966 2070 6174 6820  ilters (if path 
-00000630: 706f 696e 7473 2074 6f20 6120 6469 7265  points to a dire
-00000640: 6374 6f72 7929 2903 7223 0000 00da 056e  ctory)).r#.....n
-00000650: 6172 6773 7225 0000 0029 05da 0c61 6464  argsr%...)...add
-00000660: 5f61 7267 756d 656e 74da 0373 7472 720a  _argument..strr.
-00000670: 0000 0072 0500 0000 7207 0000 0029 0172  ...r....r....).r
-00000680: 0c00 0000 7220 0000 0072 2000 0000 7221  ....r ...r ...r!
-00000690: 0000 00da 1975 706c 6f61 645f 6669 6c65  .....upload_file
-000006a0: 735f 7365 7475 705f 7061 7273 6572 2900  s_setup_parser).
-000006b0: 0000 7330 0000 0004 010a 0106 ff04 0302  ..s0............
-000006c0: 0102 0102 0102 0106 fc04 0602 0102 0102  ................
-000006d0: 0102 0102 0106 fb04 0702 0102 0102 0102  ................
-000006e0: 0102 0106 fb0c 0772 2a00 0000 7a0c 7570  .......r*...z.up
-000006f0: 6c6f 6164 2d66 696c 6573 7225 0000 007a  load-filesr%...z
-00000700: 3255 706c 6f61 6473 2061 2066 696c 6520  2Uploads a file 
-00000710: 6f72 2064 6972 6563 746f 7279 2074 6f20  or directory to 
-00000720: 6120 7370 6563 6966 6963 2064 6174 6173  a specific datas
-00000730: 6574 2e29 0472 1c00 0000 da05 6c6f 6769  et.).r......logi
-00000740: 63da 0c73 6574 7570 5f70 6172 7365 72da  c..setup_parser.
-00000750: 0e63 6f6d 6d61 6e64 5f6b 7761 7267 7329  .command_kwargs)
-00000760: 11da 0861 7267 7061 7273 65da 0770 6174  ...argparse..pat
-00000770: 686c 6962 da0f 646f 6d61 696e 2e64 6174  hlib..domain.dat
-00000780: 6173 6574 7372 0300 0000 da07 636f 6d6d  asetsr......comm
-00000790: 616e 6472 0500 0000 7206 0000 00da 0b63  andr....r......c
-000007a0: 6f6d 6d6f 6e5f 6172 6773 7207 0000 0072  ommon_argsr....r
-000007b0: 0b00 0000 7208 0000 00da 0e73 6861 7265  ....r......share
-000007c0: 645f 6865 6c70 646f 6372 0a00 0000 da0e  d_helpdocr......
-000007d0: 4172 6775 6d65 6e74 5061 7273 6572 7222  ArgumentParserr"
-000007e0: 0000 0072 2a00 0000 da14 7570 6c6f 6164  ...r*.....upload
-000007f0: 5f66 696c 6573 5f63 6f6d 6d61 6e64 7220  _files_commandr 
-00000800: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00000810: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000820: 731e 0000 0008 0108 010c 0210 010c 040c  s...............
-00000830: 010c 0114 0308 1a02 1b02 0102 0102 0106  ................
-00000840: 010a fc                                  ...
+00000060: 6d08 5a08 0100 6407 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000070: 0100 6409 6508 640a 6500 6a0b 6604 640b  ..d.e.d.e.j.f.d.
+00000080: 640c 8404 5a0c 640d 640e 8400 5a0d 6506  d...Z.d.d...Z.e.
+00000090: 640f 650c 650d 6410 6411 6901 6412 8d04  d.e.e.d.d.i.d...
+000000a0: 5a0e 6401 5300 2913 e900 0000 004e e903  Z.d.S.)......N..
+000000b0: 0000 0029 01da 0744 6174 6173 6574 e902  ...)...Dataset..
+000000c0: 0000 0029 02da 1345 7869 7374 696e 6750  ...)...ExistingP
+000000d0: 6174 686c 6962 5061 7468 da0d 526f 626f  athlibPath..Robo
+000000e0: 746f 436f 6d6d 616e 6429 01da 0a43 4c49  toCommand)...CLI
+000000f0: 436f 6e74 6578 74e9 0100 0000 2901 da0f  Context.....)...
+00000100: 4441 5441 5345 545f 4944 5f48 454c 50da  DATASET_ID_HELP.
+00000110: 0763 6f6e 7465 7874 da06 7061 7273 6572  .context..parser
+00000120: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
+00000130: 0006 0000 0043 0000 0073 9800 0000 7c00  .....C...s....|.
+00000140: 6a00 7d03 7c00 6a01 6400 7501 7211 7c03  j.}.|.j.d.u.r.|.
+00000150: a002 a100 7311 7c02 a003 6401 a101 0100  ....s.|...d.....
+00000160: 7c00 6a04 6400 7501 721f 7c03 a002 a100  |.j.d.u.r.|.....
+00000170: 721f 7c02 a003 6402 a101 0100 7405 a006  r.|...d.....t...
+00000180: 7c00 6a07 7c01 6a08 7c01 6a09 7c01 6a0a  |.j.|.j.|.j.|.j.
+00000190: a104 7d04 7c03 a002 a100 7239 7c04 6a0b  ..}.|.....r9|.j.
+000001a0: 7c03 7c00 6a01 6403 8d02 0100 6400 5300  |.|.j.d.....d.S.
+000001b0: 7c00 6a04 6400 7500 7241 7c03 6a0c 6e02  |.j.d.u.rA|.j.n.
+000001c0: 7c00 6a04 7d05 7c04 a00d 7c03 7c05 a102  |.j.}.|...|.|...
+000001d0: 0100 6400 5300 2904 4e7a 4b45 7863 6c75  ..d.S.).NzKExclu
+000001e0: 6465 2066 696c 7465 7273 2061 7265 206f  de filters are o
+000001f0: 6e6c 7920 7375 7070 6f72 7465 6420 666f  nly supported fo
+00000200: 7220 6469 7265 6374 6f72 7920 7570 6c6f  r directory uplo
+00000210: 6164 732c 206e 6f74 2073 696e 676c 6520  ads, not single 
+00000220: 6669 6c65 732e 7a4a 4b65 7920 6f76 6572  files.zJKey over
+00000230: 7269 6465 7320 6172 6520 6f6e 6c79 2073  rides are only s
+00000240: 7570 706f 7274 6564 2066 6f72 2073 696e  upported for sin
+00000250: 676c 6520 6669 6c65 2075 706c 6f61 6473  gle file uploads
+00000260: 2c20 6e6f 7720 6469 7265 6374 6f72 6965  , now directorie
+00000270: 732e 2902 da0e 6469 7265 6374 6f72 795f  s.)...directory_
+00000280: 7061 7468 da10 6578 636c 7564 655f 7061  path..exclude_pa
+00000290: 7474 6572 6e73 290e da04 7061 7468 da07  tterns)...path..
+000002a0: 6578 636c 7564 65da 0669 735f 6469 72da  exclude..is_dir.
+000002b0: 0565 7272 6f72 da03 6b65 7972 0300 0000  .error..keyr....
+000002c0: da07 6672 6f6d 5f69 64da 0a64 6174 6173  ..from_id..datas
+000002d0: 6574 5f69 64da 0864 6174 6173 6574 73da  et_id..datasets.
+000002e0: 0566 696c 6573 da13 7472 616e 7361 6374  .files..transact
+000002f0: 696f 6e5f 6d61 6e61 6765 72da 1075 706c  ion_manager..upl
+00000300: 6f61 645f 6469 7265 6374 6f72 79da 046e  oad_directory..n
+00000310: 616d 65da 0b75 706c 6f61 645f 6669 6c65  ame..upload_file
+00000320: 2906 da04 6172 6773 720a 0000 0072 0b00  )...argsr....r..
+00000330: 0000 720e 0000 00da 0764 6174 6173 6574  ..r......dataset
+00000340: 7212 0000 00a9 0072 1d00 0000 fae9 2f63  r......r....../c
+00000350: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
+00000360: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
+00000370: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
+00000380: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
+00000390: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
+000003a0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
+000003b0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
+000003c0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
+000003d0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
+000003e0: 3939 642f 726f 626f 746f 2d61 692f 726f  99d/roboto-ai/ro
+000003f0: 626f 746f 2d68 6f73 7465 642d 6170 702f  boto-hosted-app/
+00000400: 7061 636b 6167 6573 2f72 6f62 6f74 6f2f  packages/roboto/
+00000410: 7372 632f 726f 626f 746f 2f63 6c69 2f64  src/roboto/cli/d
+00000420: 6174 6173 6574 732f 7570 6c6f 6164 5f66  atasets/upload_f
+00000430: 696c 6573 2e70 79da 0c75 706c 6f61 645f  iles.py..upload_
+00000440: 6669 6c65 730e 0000 0073 2600 0000 0601  files....s&.....
+00000450: 1201 0401 0201 04ff 1203 0401 0201 04ff  ................
+00000460: 0404 0401 0401 0401 0401 04fc 0807 1401  ................
+00000470: 1602 1001 721f 0000 0063 0100 0000 0000  ....r....c......
+00000480: 0000 0000 0000 0100 0000 0700 0000 4300  ..............C.
+00000490: 0000 7352 0000 007c 006a 0064 0164 0274  ..sR...|.j.d.d.t
+000004a0: 0164 0374 0264 048d 0501 007c 006a 0064  .d.t.d.....|.j.d
+000004b0: 0564 0674 0164 0764 088d 0401 007c 006a  .d.t.d.d.....|.j
+000004c0: 0064 0964 0a74 0364 0364 0b64 048d 0501  .d.d.t.d.d.d....
+000004d0: 007c 006a 0064 0c64 0d74 0164 0e64 0f64  .|.j.d.d.t.d.d.d
+000004e0: 108d 0501 0064 0053 0029 114e 7a02 2d64  .....d.S.).Nz.-d
+000004f0: 7a0c 2d2d 6461 7461 7365 742d 6964 5429  z.--dataset-idT)
+00000500: 03da 0474 7970 65da 0872 6571 7569 7265  ...type..require
+00000510: 64da 0468 656c 707a 022d 6b7a 052d 2d6b  d..helpz.-kz.--k
+00000520: 6579 7a54 4120 6b65 7920 746f 2061 6c69  eyzTA key to ali
+00000530: 6173 2061 2066 696c 6520 746f 2077 6865  as a file to whe
+00000540: 6e20 7374 6f72 696e 6720 6974 2074 6f20  n storing it to 
+00000550: 6120 6461 7461 7365 742e 2044 6f65 7320  a dataset. Does 
+00000560: 6e6f 7468 696e 6720 666f 7220 6469 7265  nothing for dire
+00000570: 6374 6f72 6965 732e 2902 7220 0000 0072  ctories.).r ...r
+00000580: 2200 0000 7a02 2d70 7a06 2d2d 7061 7468  "...z.-pz.--path
+00000590: 7a2a 5468 6520 7061 7468 2074 6f20 6120  z*The path to a 
+000005a0: 6669 6c65 206f 7220 6469 7265 6374 6f72  file or director
+000005b0: 7920 746f 2075 706c 6f61 642e 7a02 2d78  y to upload.z.-x
+000005c0: 7a09 2d2d 6578 636c 7564 65da 012a 7a3c  z.--exclude..*z<
+000005d0: 5a65 726f 206f 7220 6d6f 7265 2065 7863  Zero or more exc
+000005e0: 6c75 6465 2066 696c 7465 7273 2028 6966  lude filters (if
+000005f0: 2070 6174 6820 706f 696e 7473 2074 6f20   path points to 
+00000600: 6120 6469 7265 6374 6f72 7929 2903 7220  a directory)).r 
+00000610: 0000 00da 056e 6172 6773 7222 0000 0029  .....nargsr"...)
+00000620: 04da 0c61 6464 5f61 7267 756d 656e 74da  ...add_argument.
+00000630: 0373 7472 7209 0000 0072 0500 0000 2901  .strr....r....).
+00000640: 720b 0000 0072 1d00 0000 721d 0000 0072  r....r....r....r
+00000650: 1e00 0000 da19 7570 6c6f 6164 5f66 696c  ......upload_fil
+00000660: 6573 5f73 6574 7570 5f70 6172 7365 7227  es_setup_parser'
+00000670: 0000 0073 2e00 0000 0401 0a01 06ff 0403  ...s............
+00000680: 0201 0201 0201 0201 06fc 0406 0201 0201  ................
+00000690: 0201 0201 0201 06fb 0407 0201 0201 0201  ................
+000006a0: 0201 0201 0afb 7227 0000 007a 0c75 706c  ......r'...z.upl
+000006b0: 6f61 642d 6669 6c65 7372 2200 0000 7a32  oad-filesr"...z2
+000006c0: 5570 6c6f 6164 7320 6120 6669 6c65 206f  Uploads a file o
+000006d0: 7220 6469 7265 6374 6f72 7920 746f 2061  r directory to a
+000006e0: 2073 7065 6369 6669 6320 6461 7461 7365   specific datase
+000006f0: 742e 2904 7219 0000 00da 056c 6f67 6963  t.).r......logic
+00000700: da0c 7365 7475 705f 7061 7273 6572 da0e  ..setup_parser..
+00000710: 636f 6d6d 616e 645f 6b77 6172 6773 290f  command_kwargs).
+00000720: da08 6172 6770 6172 7365 da07 7061 7468  ..argparse..path
+00000730: 6c69 62da 0f64 6f6d 6169 6e2e 6461 7461  lib..domain.data
+00000740: 7365 7473 7203 0000 00da 0763 6f6d 6d61  setsr......comma
+00000750: 6e64 7205 0000 0072 0600 0000 720a 0000  ndr....r....r...
+00000760: 0072 0700 0000 da0e 7368 6172 6564 5f68  .r......shared_h
+00000770: 656c 7064 6f63 7209 0000 00da 0e41 7267  elpdocr......Arg
+00000780: 756d 656e 7450 6172 7365 7272 1f00 0000  umentParserr....
+00000790: 7227 0000 00da 1475 706c 6f61 645f 6669  r'.....upload_fi
+000007a0: 6c65 735f 636f 6d6d 616e 6472 1d00 0000  les_commandr....
+000007b0: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
+000007c0: 083c 6d6f 6475 6c65 3e01 0000 0073 1c00  .<module>....s..
+000007d0: 0000 0801 0801 0c02 1001 0c04 0c01 1403  ................
+000007e0: 0819 021a 0201 0201 0201 0601 0afc       ..............
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/commands.py` & `roboto-0.2.9/src/roboto/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/create.py` & `roboto-0.2.9/src/roboto/cli/datasets/create.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/delete_dataset.py` & `roboto-0.2.9/src/roboto/cli/datasets/delete_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 import argparse
 
 from ...domain.datasets import Dataset
 from ..command import RobotoCommand
-from ..common_args import add_org_arg
 from ..context import CLIContext
 from .shared_helpdoc import DATASET_ID_HELP
 
 
 def delete_dataset(args, context: CLIContext, parser: argparse.ArgumentParser):
     dataset = Dataset.from_id(
         args.dataset_id,
         context.datasets,
         context.files,
         context.transaction_manager,
-        org_id=args.org,
     )
     dataset.delete_dataset()
     print(f"Deleted dataset {args.dataset_id}")
 
 
 def delete_dataset_setup_parser(parser):
     parser.add_argument(
         "-d", "--dataset-id", type=str, required=True, help=DATASET_ID_HELP
     )
-    add_org_arg(parser)
 
 
 delete_dataset_command = RobotoCommand(
     name="delete",
     logic=delete_dataset,
     setup_parser=delete_dataset_setup_parser,
     command_kwargs={"help": "Delete dataset (and all related subresources) by id."},
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/delete_files.py` & `roboto-0.2.9/src/roboto/cli/datasets/delete_files.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 import argparse
 
 from ...domain.datasets import Dataset
 from ..command import RobotoCommand
-from ..common_args import add_org_arg
 from ..context import CLIContext
 from .shared_helpdoc import DATASET_ID_HELP
 
 
 def delete_files(args, context: CLIContext, parser: argparse.ArgumentParser):
     dataset = Dataset.from_id(
         args.dataset_id,
         context.datasets,
         context.files,
         context.transaction_manager,
-        org_id=args.org,
     )
 
     dataset.delete_files(include_patterns=args.include, exclude_patterns=args.exclude)
 
 
 def delete_files_setup_parser(parser):
     parser.add_argument(
@@ -34,15 +32,14 @@
     parser.add_argument(
         "-x",
         "--exclude",
         type=str,
         nargs="*",
         help="Zero or more exclude filters",
     )
-    add_org_arg(parser)
 
 
 delete_files_command = RobotoCommand(
     name="delete-files",
     logic=delete_files,
     setup_parser=delete_files_setup_parser,
     command_kwargs={"help": "Delete file(s) from a specific dataset."},
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/download_files.py` & `roboto-0.2.9/src/roboto/cli/datasets/download_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 import argparse
 import pathlib
 
 from ...domain.datasets import Dataset
 from ..command import RobotoCommand
-from ..common_args import add_org_arg
 from ..context import CLIContext
 from .shared_helpdoc import DATASET_ID_HELP
 
 
 def download_files(args, context: CLIContext, parser: argparse.ArgumentParser):
     record = Dataset.from_id(
         args.dataset_id,
         context.datasets,
         context.files,
         context.transaction_manager,
-        org_id=args.org,
     )
 
     record.download_files(
         out_path=args.path, include_patterns=args.include, exclude_patterns=args.exclude
     )
 
 
@@ -44,15 +42,14 @@
     parser.add_argument(
         "-x",
         "--exclude",
         type=str,
         nargs="*",
         help="Zero or more exclude filters (if path points to a directory)",
     )
-    add_org_arg(parser)
 
 
 download_files_command = RobotoCommand(
     name="download-files",
     logic=download_files,
     setup_parser=download_files_setup_parser,
     command_kwargs={"help": "Downloads a file or directory from a specific dataset."},
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/list_files.py` & `roboto-0.2.9/src/roboto/cli/datasets/list_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 import argparse
 import sys
 
 from ...domain.datasets import Dataset
 from ..command import RobotoCommand
-from ..common_args import add_org_arg
 from ..context import CLIContext
 from .shared_helpdoc import DATASET_ID_HELP
 
 
 def list_files(args, context: CLIContext, parser: argparse.ArgumentParser):
     record = Dataset.from_id(
         args.dataset_id,
         context.datasets,
         context.files,
         context.transaction_manager,
-        org_id=args.org,
     )
 
     for f in record.list_files(args.include, args.exclude):
         sys.stdout.write(f"{f.relative_path}\n")
 
 
 def list_files_setup_parser(parser):
@@ -36,15 +34,14 @@
     parser.add_argument(
         "-x",
         "--exclude",
         type=str,
         nargs="*",
         help="Zero or more exclude filters (if path points to a directory)",
     )
-    add_org_arg(parser)
 
 
 list_files_command = RobotoCommand(
     name="list-files",
     logic=list_files,
     setup_parser=list_files_setup_parser,
     command_kwargs={"help": "Lists files for a specific dataset."},
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/search.py` & `roboto-0.2.9/src/roboto/cli/datasets/search.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/show.py` & `roboto-0.2.9/src/roboto/cli/datasets/show.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 import argparse
 import json
 
 from ...domain.datasets import Dataset
 from ..command import RobotoCommand
-from ..common_args import add_org_arg
 from ..context import CLIContext
 from .shared_helpdoc import DATASET_ID_HELP
 
 
 def show(args, context: CLIContext, parser: argparse.ArgumentParser):
     record = Dataset.from_id(
         args.dataset_id,
         context.datasets,
         context.files,
         context.transaction_manager,
-        org_id=args.org,
     )
     print(json.dumps(record.to_dict(), indent=4))
 
 
 def show_setup_parser(parser):
     parser.add_argument(
         "-d", "--dataset-id", type=str, required=True, help=DATASET_ID_HELP
     )
-    add_org_arg(parser)
 
 
 show_command = RobotoCommand(
     name="show",
     logic=show,
     setup_parser=show_setup_parser,
     command_kwargs={"help": "Show information about a specific dataset."},
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/update.py` & `roboto-0.2.9/src/roboto/cli/datasets/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from ...domain.datasets import Dataset
 from ...updates import MetadataChangeset
 from ..command import (
     KeyValuePairsAction,
     RobotoCommand,
 )
-from ..common_args import add_org_arg
 from ..context import CLIContext
 from .shared_helpdoc import DATASET_ID_HELP
 
 
 def update(
     args: argparse.Namespace, context: CLIContext, parser: argparse.ArgumentParser
 ) -> None:
@@ -26,27 +25,25 @@
         parser.error("No dataset changes specified.")
 
     dataset = Dataset.from_id(
         args.dataset_id,
         context.datasets,
         context.files,
         context.transaction_manager,
-        org_id=args.org,
     )
     dataset.update(metadata_changeset=metadata_changeset, description=args.description)
 
     print(f"Successfully updated dataset '{dataset.dataset_id}'. Record: ")
     print(json.dumps(dataset.to_dict(), indent=4))
 
 
 def update_parser(parser: argparse.ArgumentParser):
     parser.add_argument(
         "-d", "--dataset-id", type=str, required=True, help=DATASET_ID_HELP
     )
-    add_org_arg(parser)
 
     parser.add_argument(
         "--description", help="A new description to add to this dataset"
     )
 
     parser.add_argument(
         "--put-tags",
```

### Comparing `roboto-0.2.8/src/roboto/cli/datasets/upload_files.py` & `roboto-0.2.9/src/roboto/cli/datasets/upload_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import pathlib
 
 from ...domain.datasets import Dataset
 from ..command import (
     ExistingPathlibPath,
     RobotoCommand,
 )
-from ..common_args import add_org_arg
 from ..context import CLIContext
 from .shared_helpdoc import DATASET_ID_HELP
 
 
 def upload_files(args, context: CLIContext, parser: argparse.ArgumentParser):
     path: pathlib.Path = args.path
     if args.exclude is not None and not path.is_dir():
@@ -24,15 +23,14 @@
         )
 
     dataset = Dataset.from_id(
         args.dataset_id,
         context.datasets,
         context.files,
         context.transaction_manager,
-        org_id=args.org,
     )
 
     if path.is_dir():
         dataset.upload_directory(directory_path=path, exclude_patterns=args.exclude)
     else:
         key = path.name if args.key is None else args.key
         dataset.upload_file(path, key)
@@ -58,15 +56,14 @@
     parser.add_argument(
         "-x",
         "--exclude",
         type=str,
         nargs="*",
         help="Zero or more exclude filters (if path points to a directory)",
     )
-    add_org_arg(parser)
 
 
 upload_files_command = RobotoCommand(
     name="upload-files",
     logic=upload_files,
     setup_parser=upload_files_setup_parser,
     command_kwargs={"help": "Uploads a file or directory to a specific dataset."},
```

### Comparing `roboto-0.2.8/src/roboto/cli/entry.py` & `roboto-0.2.9/src/roboto/cli/entry.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/extension/__pycache__/cli_extension.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/extension/__pycache__/cli_extension.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2347 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 2b09 0000  o........Y.e+...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 2b09 0000  o.......2H.e+...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6403 6405 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6406 6407 8400 6407 6500 6a08 8303 5a09  d.d...d.e.j...Z.
 00000070: 6408 650a 6505 1900 6409 650a 6505 1900  d.e.e...d.e.e...
@@ -26,16 +26,16 @@
 00000190: 6e73 696f 6eda 0672 6574 7572 6e63 0100  nsion..returnc..
 000001a0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
 000001b0: 0000 4300 0000 f308 0000 0074 0064 0183  ..C........t.d..
 000001c0: 0182 0129 024e da08 6765 745f 6e61 6d65  ...).N..get_name
 000001d0: a901 da13 4e6f 7449 6d70 6c65 6d65 6e74  ....NotImplement
 000001e0: 6564 4572 726f 72a9 01da 0363 6c73 a900  edError....cls..
 000001f0: 720f 0000 00fa eb2f 636f 6465 6275 696c  r....../codebuil
-00000200: 642f 6f75 7470 7574 2f73 7263 3130 3531  d/output/src1051
-00000210: 3138 3230 3839 2f73 7263 2f63 6f64 6573  182089/src/codes
+00000200: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+00000210: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
 00000220: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 00000230: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 00000240: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 00000250: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 00000260: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 00000270: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 00000280: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto-0.2.8/src/roboto/cli/extension/cli_extension.py` & `roboto-0.2.9/src/roboto/cli/extension/cli_extension.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/images/__pycache__/commands.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/images/__pycache__/commands.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 631 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 7702 0000  o........Y.ew...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 7702 0000  o.......2H.ew...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6402 6405 6c06 6d07 5a07 0100 6402  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6402 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6402 6408 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -32,16 +32,16 @@
 000001f0: 005a 0b6c 6973 745f 696d 6167 6573 7206  .Z.list_imagesr.
 00000200: 0000 005a 0a6c 6973 745f 7265 706f 7372  ...Z.list_reposr
 00000210: 0700 0000 da05 6c6f 6769 6e72 0800 0000  ......loginr....
 00000220: 5a04 7075 6c6c 7209 0000 00da 0470 7573  Z.pullr......pus
 00000230: 6872 0a00 0000 720e 0000 00da 0b63 6f6d  hr....r......com
 00000240: 6d61 6e64 5f73 6574 a900 7213 0000 0072  mand_set..r....r
 00000250: 1300 0000 fae3 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000260: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000270: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000260: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000270: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000280: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000290: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000002a0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000002b0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000002c0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000002d0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000002e0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/cli/images/__pycache__/delete_image.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/images/__pycache__/delete_image.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1058 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 2204 0000  o........Y.e"...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 2204 0000  o.......2H.e"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6406 6c05 6d06 5a06 0100 6404 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6408 6500 6a09 6409 6508  m.Z...d.e.j.d.e.
 00000070: 640a 6500 6a0a 640b 6401 6608 640c 640d  d.e.j.d.d.f.d.d.
@@ -25,15 +25,15 @@
 00000180: 6572 7669 6365 5f62 6173 655f 7572 6cda  ervice_base_url.
 00000190: 0468 7474 70da 0c64 656c 6574 655f 696d  .http..delete_im
 000001a0: 6167 65da 0c72 656d 6f74 655f 696d 6167  age..remote_imag
 000001b0: 65da 036f 7267 2904 7208 0000 0072 0900  e..org).r....r..
 000001c0: 0000 720a 0000 00da 0e69 6d61 6765 5f72  ..r......image_r
 000001d0: 6567 6973 7472 79a9 0072 1300 0000 fae7  egistry..r......
 000001e0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000001f0: 742f 7372 6331 3035 3131 3832 3038 392f  t/src1051182089/
+000001f0: 742f 7372 6333 3037 3932 3336 3236 342f  t/src3079236264/
 00000200: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000210: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000220: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000230: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000240: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000250: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000260: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto-0.2.8/src/roboto/cli/images/__pycache__/delete_repo.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/images/__pycache__/delete_repo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1254 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 e604 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 e604 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6406 6c05 6d06 5a06 0100 6404 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6408 6500 6a09 6409 6508  m.Z...d.e.j.d.e.
 00000070: 640a 6500 6a0a 640b 6401 6608 640c 640d  d.e.j.d.d.f.d.d.
@@ -26,16 +26,16 @@
 00000190: 655f 6261 7365 5f75 726c da04 6874 7470  e_base_url..http
 000001a0: da11 6465 6c65 7465 5f72 6570 6f73 6974  ..delete_reposit
 000001b0: 6f72 79da 0f72 6570 6f73 6974 6f72 795f  ory..repository_
 000001c0: 6e61 6d65 da03 6f72 6772 0d00 0000 2904  name..orgr....).
 000001d0: 7208 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
 000001e0: 0e69 6d61 6765 5f72 6567 6973 7472 79a9  .image_registry.
 000001f0: 0072 1400 0000 fae6 2f63 6f64 6562 7569  .r....../codebui
-00000200: 6c64 2f6f 7574 7075 742f 7372 6331 3035  ld/output/src105
-00000210: 3131 3832 3038 392f 7372 632f 636f 6465  1182089/src/code
+00000200: 6c64 2f6f 7574 7075 742f 7372 6333 3037  ld/output/src307
+00000210: 3932 3336 3236 342f 7372 632f 636f 6465  9236264/src/code
 00000220: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000230: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000240: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000250: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000260: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000270: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000280: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto-0.2.8/src/roboto/cli/images/__pycache__/list_images.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/images/__pycache__/list_images.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1444 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 a405 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 a405 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 6404 6405 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6404 6406 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6407 6c08 6d09 5a09 0100 6408  ..d.d.l.m.Z...d.
 00000070: 6500 6a0a 6409 6509 640a 6500 6a0b 640b  e.j.d.e.d.e.j.d.
@@ -37,16 +37,16 @@
 00000240: 046a 736f 6eda 0564 756d 7073 da04 6469  .json..dumps..di
 00000250: 6374 da0a 6e65 7874 5f74 6f6b 656e 2906  ct..next_token).
 00000260: 7208 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
 00000270: 0e69 6d61 6765 5f72 6567 6973 7472 79da  .image_registry.
 00000280: 1170 6167 696e 6174 6564 5f72 6573 756c  .paginated_resul
 00000290: 7473 da05 696d 6167 65a9 0072 1d00 0000  ts..image..r....
 000002a0: fae6 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-000002b0: 7075 742f 7372 6331 3035 3131 3832 3038  put/src105118208
-000002c0: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+000002b0: 7075 742f 7372 6333 3037 3932 3336 3236  put/src307923626
+000002c0: 342f 7372 632f 636f 6465 7374 6172 2d63  4/src/codestar-c
 000002d0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 000002e0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 000002f0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 00000300: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 00000310: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 00000320: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000330: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto-0.2.8/src/roboto/cli/images/__pycache__/list_repos.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/images/__pycache__/list_repos.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1173 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 9504 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 9504 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 6404 6405 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6404 6406 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6407 6c08 6d09 5a09 0100 6408  ..d.d.l.m.Z...d.
 00000070: 6500 6a0a 6409 6509 640a 6500 6a0b 640b  e.j.d.e.d.e.j.d.
@@ -35,16 +35,16 @@
 00000220: 6e74 da04 6a73 6f6e da05 6475 6d70 73da  nt..json..dumps.
 00000230: 0464 6963 74da 0a6e 6578 745f 746f 6b65  .dict..next_toke
 00000240: 6e29 0672 0900 0000 720a 0000 0072 0b00  n).r....r....r..
 00000250: 0000 da0e 696d 6167 655f 7265 6769 7374  ....image_regist
 00000260: 7279 da11 7061 6769 6e61 7465 645f 7265  ry..paginated_re
 00000270: 7375 6c74 735a 0472 6570 6fa9 0072 1c00  sultsZ.repo..r..
 00000280: 0000 fae5 2f63 6f64 6562 7569 6c64 2f6f  ..../codebuild/o
-00000290: 7574 7075 742f 7372 6331 3035 3131 3832  utput/src1051182
-000002a0: 3038 392f 7372 632f 636f 6465 7374 6172  089/src/codestar
+00000290: 7574 7075 742f 7372 6333 3037 3932 3336  utput/src3079236
+000002a0: 3236 342f 7372 632f 636f 6465 7374 6172  264/src/codestar
 000002b0: 2d63 6f6e 6e65 6374 696f 6e73 2e75 732d  -connections.us-
 000002c0: 7765 7374 2d32 2e61 6d61 7a6f 6e61 7773  west-2.amazonaws
 000002d0: 2e63 6f6d 2f67 6974 2d68 7474 702f 3036  .com/git-http/06
 000002e0: 3631 3935 3131 3233 3835 2f75 732d 7765  6195112385/us-we
 000002f0: 7374 2d32 2f65 3635 3032 6138 302d 6262  st-2/e6502a80-bb
 00000300: 3465 2d34 6662 652d 3837 3263 2d35 6434  4e-4fbe-872c-5d4
 00000310: 3263 3139 3336 3939 642f 726f 626f 746f  2c193699d/roboto
```

### Comparing `roboto-0.2.8/src/roboto/cli/images/__pycache__/login.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/images/__pycache__/login.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1939 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 9307 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 9307 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6404 6c05 6d06 5a06 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c07 6d08 5a08 0100 6405 6407 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6405 6408 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -48,15 +48,15 @@
 000002f0: 0900 0000 720a 0000 0072 0b00 0000 da0e  ....r....r......
 00000300: 696d 6167 655f 7265 6769 7374 7279 7214  image_registryr.
 00000310: 0000 00da 0b63 7265 6465 6e74 6961 6c73  .....credentials
 00000320: da03 636d 645a 1e64 6f63 6b65 725f 6c6f  ..cmdZ.docker_lo
 00000330: 6769 6e5f 636f 6d70 6c65 7465 645f 7072  gin_completed_pr
 00000340: 6f63 6573 73a9 0072 2400 0000 fae0 2f63  ocess..r$...../c
 00000350: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000360: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+00000360: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 00000370: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 00000380: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 00000390: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 000003a0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 000003b0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 000003c0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 000003d0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/cli/images/__pycache__/pull.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/images/__pycache__/pull.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2307 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 0309 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 0309 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c04 6d05 5a05 0100 6402 6404 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6405 6406 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6407 6c0a 6d0b 5a0b 0100 6405  ..d.d.l.m.Z...d.
@@ -82,15 +82,15 @@
 00000510: 5f72 6567 6973 7472 79da 0570 6172 7473  _registry..parts
 00000520: da0e 7265 706f 7369 746f 7279 5f75 7269  ..repository_uri
 00000530: da01 5fda 0b63 7265 6465 6e74 6961 6c73  .._..credentials
 00000540: 5a09 6c6f 6769 6e5f 636d 64da 0365 7863  Z.login_cmd..exc
 00000550: 5a08 7075 6c6c 5f63 6d64 5a09 7075 6c6c  Z.pull_cmdZ.pull
 00000560: 5f70 726f 63a9 0072 3300 0000 fadf 2f63  _proc..r3...../c
 00000570: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000580: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+00000580: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 00000590: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 000005a0: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 000005b0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 000005c0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 000005d0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 000005e0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 000005f0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/cli/images/__pycache__/push.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/images/__pycache__/push.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 5238 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 7614 0000  o........Y.ev...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 7614 0000  o.......2H.ev...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 ca00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6402 6404 6c07 6d08 5a08 0100 6402  ..d.d.l.m.Z...d.
 00000070: 6405 6c09 6d0a 5a0a 6d0b 5a0b 0100 6406  d.l.m.Z.m.Z...d.
@@ -136,16 +136,16 @@
 00000870: 6f73 6974 6f72 795f 6e61 6d65 6301 0000  ository_namec...
 00000880: 0000 0000 0000 0000 0001 0000 0003 0000  ................
 00000890: 0053 0000 0073 1200 0000 7400 6401 7c00  .S...s....t.d.|.
 000008a0: 1300 6401 1b00 6402 8302 5300 2903 4e72  ..d...d...S.).Nr
 000008b0: 0700 0000 e920 0000 0029 01da 036d 696e  ..... ...)...min
 000008c0: 2901 da09 6974 6572 6174 696f 6ea9 0072  )...iteration..r
 000008d0: 2000 0000 fadf 2f63 6f64 6562 7569 6c64   ...../codebuild
-000008e0: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-000008f0: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+000008e0: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+000008f0: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000900: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000910: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000920: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000930: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000940: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000950: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000960: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/cli/images/commands.py` & `roboto-0.2.9/src/roboto/cli/images/commands.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/images/delete_image.py` & `roboto-0.2.9/src/roboto/cli/images/delete_image.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/images/delete_repo.py` & `roboto-0.2.9/src/roboto/cli/images/delete_repo.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/images/list_images.py` & `roboto-0.2.9/src/roboto/cli/images/list_images.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/images/list_repos.py` & `roboto-0.2.9/src/roboto/cli/images/list_repos.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/images/login.py` & `roboto-0.2.9/src/roboto/cli/images/login.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/images/pull.py` & `roboto-0.2.9/src/roboto/cli/images/pull.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/images/push.py` & `roboto-0.2.9/src/roboto/cli/images/push.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/invocations/__init__.py` & `roboto-0.2.9/src/roboto/cli/invocations/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/invocations/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/invocations/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 516 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 0402 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 0402 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6402 6405 6c06 6d07 5a07 0100 6402  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6503 6505 6507  d.l.m.Z...e.e.e.
 00000070: 6509 6704 5a0a 6501 6407 6408 650a 6409  e.g.Z.e.d.d.e.d.
@@ -24,15 +24,15 @@
 00000170: da07 636f 6d6d 616e 6472 0200 0000 da06  ..commandr......
 00000180: 6361 6e63 656c 7204 0000 00da 046c 6f67  cancelr......log
 00000190: 7372 0500 0000 da04 7368 6f77 7206 0000  sr......showr...
 000001a0: 00da 0673 7461 7475 7372 0700 0000 720b  ...statusr....r.
 000001b0: 0000 00da 0b63 6f6d 6d61 6e64 5f73 6574  .....command_set
 000001c0: a900 7212 0000 0072 1200 0000 fae8 2f63  ..r....r....../c
 000001d0: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-000001e0: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+000001e0: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 000001f0: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 00000200: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 00000210: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 00000220: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 00000230: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 00000240: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 00000250: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/cli/invocations/__pycache__/cancel.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/invocations/__pycache__/cancel.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 818 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 3203 0000  o........Y.e2...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 3203 0000  o.......2H.e2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6406 6c05 6d06 5a06 0100 6404 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6408 6500 6a09 6409 6508  m.Z...d.e.j.d.e.
 00000070: 640a 6500 6a0a 640b 6401 6608 640c 640d  d.e.j.d.d.f.d.d.
@@ -27,15 +27,15 @@
 000001a0: 00da 0766 726f 6d5f 6964 da0d 696e 766f  ...from_id..invo
 000001b0: 6361 7469 6f6e 5f69 64da 0b69 6e76 6f63  cation_id..invoc
 000001c0: 6174 696f 6e73 da03 6f72 67da 0663 616e  ations..org..can
 000001d0: 6365 6cda 0570 7269 6e74 2904 7208 0000  cel..print).r...
 000001e0: 0072 0900 0000 720a 0000 00da 0a69 6e76  .r....r......inv
 000001f0: 6f63 6174 696f 6ea9 0072 1500 0000 fae6  ocation..r......
 00000200: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000210: 742f 7372 6331 3035 3131 3832 3038 392f  t/src1051182089/
+00000210: 742f 7372 6333 3037 3932 3336 3236 342f  t/src3079236264/
 00000220: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000230: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000240: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000250: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000260: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000270: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000280: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto-0.2.8/src/roboto/cli/invocations/__pycache__/logs.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/invocations/__pycache__/logs.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 4227 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 8310 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 8310 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 d200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6403  d.l.m.Z.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6405 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6405 6407 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6408 6c0b 6d0c 5a0c 0100 6409  ..d.d.l.m.Z...d.
@@ -47,15 +47,15 @@
 000002e0: 7469 616c 5f69 64da 036c 6f67 2907 720a  tial_id..log).r.
 000002f0: 0000 0072 0b00 0000 720c 0000 00da 0a69  ...r....r......i
 00000300: 6e76 6f63 6174 696f 6eda 1170 726f 6365  nvocation..proce
 00000310: 7373 5f64 6563 6f72 6174 6f72 da08 6c61  ss_decorator..la
 00000320: 7374 5f6c 6f67 da0a 6c6f 675f 7265 636f  st_log..log_reco
 00000330: 7264 a900 7221 0000 00fa e42f 636f 6465  rd..r!...../code
 00000340: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000350: 3130 3531 3138 3230 3839 2f73 7263 2f63  1051182089/src/c
+00000350: 3330 3739 3233 3632 3634 2f73 7263 2f63  3079236264/src/c
 00000360: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 00000370: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 00000380: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 00000390: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 000003a0: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 000003b0: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 000003c0: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
```

### Comparing `roboto-0.2.8/src/roboto/cli/invocations/__pycache__/show.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/invocations/__pycache__/show.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 780 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 0c03 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 0c03 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6406 6c05 6d06 5a06 0100 6404 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6408 6500 6a09 6409 6508  m.Z...d.e.j.d.e.
 00000070: 640a 6500 6a0a 640b 6401 6608 640c 640d  d.e.j.d.d.f.d.d.
@@ -25,16 +25,16 @@
 00000180: 0772 0300 0000 da07 6672 6f6d 5f69 64da  .r......from_id.
 00000190: 0d69 6e76 6f63 6174 696f 6e5f 6964 da0b  .invocation_id..
 000001a0: 696e 766f 6361 7469 6f6e 73da 036f 7267  invocations..org
 000001b0: da05 7072 696e 74da 0373 7472 2904 7208  ..print..str).r.
 000001c0: 0000 0072 0900 0000 720a 0000 00da 0a69  ...r....r......i
 000001d0: 6e76 6f63 6174 696f 6ea9 0072 1500 0000  nvocation..r....
 000001e0: fae4 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-000001f0: 7075 742f 7372 6331 3035 3131 3832 3038  put/src105118208
-00000200: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+000001f0: 7075 742f 7372 6333 3037 3932 3336 3236  put/src307923626
+00000200: 342f 7372 632f 636f 6465 7374 6172 2d63  4/src/codestar-c
 00000210: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 00000220: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 00000230: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 00000240: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 00000250: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 00000260: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000270: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto-0.2.8/src/roboto/cli/invocations/__pycache__/status.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/invocations/__pycache__/status.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2025 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 e907 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 e907 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6406 6c08 6d09 5a09 0100 6404  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6408 6500 6a0c  d.l.m.Z...d.e.j.
@@ -39,15 +39,15 @@
 00000260: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
 00000270: 0000 0067 007c 005d 067d 017c 01a0 00a1  ...g.|.].}.|....
 00000280: 0091 0271 0253 00a9 0029 01da 1374 6f5f  ...q.S...)...to_
 00000290: 7072 6573 656e 7461 626c 655f 6469 6374  presentable_dict
 000002a0: a902 da02 2e30 da0d 7374 6174 7573 5f72  .....0..status_r
 000002b0: 6563 6f72 6472 0f00 0000 720f 0000 00fa  ecordr....r.....
 000002c0: e62f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000002d0: 7574 2f73 7263 3130 3531 3138 3230 3839  ut/src1051182089
+000002d0: 7574 2f73 7263 3330 3739 3233 3632 3634  ut/src3079236264
 000002e0: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 000002f0: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000300: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000310: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000320: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000330: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000340: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto-0.2.8/src/roboto/cli/invocations/cancel.py` & `roboto-0.2.9/src/roboto/cli/invocations/cancel.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/invocations/logs.py` & `roboto-0.2.9/src/roboto/cli/invocations/logs.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/invocations/show.py` & `roboto-0.2.9/src/roboto/cli/invocations/show.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/invocations/status.py` & `roboto-0.2.9/src/roboto/cli/invocations/status.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/orgs/__pycache__/commands.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/orgs/__pycache__/commands.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 11296 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 202c 0000  o........Y.e ,..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 202c 0000  o.......2H.e ,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 de02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6404  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 0100 6404  d.l.m.Z.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6407 5a0d 650d  d.l.m.Z...d.Z.e.
@@ -73,16 +73,16 @@
 00000480: 6c6c 2062 6520 7065 7266 6f72 6d65 6420  ll be performed 
 00000490: 696d 706c 6963 6974 6c79 206f 6e20 7468  implicitly on th
 000004a0: 6569 7220 7369 6e67 6c65 206f 7267 2ea9  eir single org..
 000004b0: 02da 0474 7970 65da 0468 656c 70a9 02da  ...type..help...
 000004c0: 0c61 6464 5f61 7267 756d 656e 74da 0373  .add_argument..s
 000004d0: 7472 a902 da06 7061 7273 6572 720b 0000  tr....parserr...
 000004e0: 00a9 0072 1500 0000 fae1 2f63 6f64 6562  ...r....../codeb
-000004f0: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-00000500: 3035 3131 3832 3038 392f 7372 632f 636f  051182089/src/co
+000004f0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+00000500: 3037 3932 3336 3236 342f 7372 632f 636f  079236264/src/co
 00000510: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 00000520: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000530: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000540: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000550: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000560: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000570: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto-0.2.8/src/roboto/cli/orgs/commands.py` & `roboto-0.2.9/src/roboto/cli/orgs/commands.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/tokens/__pycache__/commands.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/tokens/__pycache__/commands.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3269 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 c50c 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 c50c 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6404 6405 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6404 6406 6c08 6d09 5a09 0100 6407  ..d.d.l.m.Z...d.
 00000070: 6509 6408 6500 6a0a 6604 6409 640a 8404  e.d.e.j.f.d.d...
@@ -53,15 +53,15 @@
 00000340: 73da 046a 736f 6eda 0564 756d 7073 da06  s..json..dumps..
 00000350: 7365 6372 6574 da03 7379 73da 0673 7464  secret..sys..std
 00000360: 6572 72da 0577 7269 7465 2905 da04 6172  err..write)...ar
 00000370: 6773 7208 0000 0072 0900 0000 7210 0000  gsr....r....r...
 00000380: 005a 1263 7265 6473 5f65 7861 6d70 6c65  .Z.creds_example
 00000390: 5f6a 736f 6ea9 0072 1a00 0000 fae3 2f63  _json..r....../c
 000003a0: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-000003b0: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+000003b0: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 000003c0: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 000003d0: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 000003e0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 000003f0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 00000400: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 00000410: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 00000420: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/cli/tokens/commands.py` & `roboto-0.2.9/src/roboto/cli/tokens/commands.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/triggers/__pycache__/commands.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/triggers/__pycache__/commands.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 17798 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 8645 0000  o........Y.e.E..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 8645 0000  o.......2H.e.E..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 2002 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6403 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6403 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6403 6406 6c0d  m.Z.m.Z...d.d.l.
@@ -119,15 +119,15 @@
 00000760: 7070 656e 6472 0a00 0000 da08 436f 6e74  ppendr......Cont
 00000770: 6169 6e73 da05 6974 656d 73da 0645 7175  ains..items..Equ
 00000780: 616c 7372 0d00 0000 da03 416e 6429 08da  alsr......And)..
 00000790: 0461 7267 7372 1f00 0000 7220 0000 0072  .argsr....r ...r
 000007a0: 2900 0000 7228 0000 00da 0374 6167 da03  )...r(.....tag..
 000007b0: 6b65 7972 2700 0000 a900 7237 0000 00fa  keyr'.....r7....
 000007c0: e52f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000007d0: 7574 2f73 7263 3130 3531 3138 3230 3839  ut/src1051182089
+000007d0: 7574 2f73 7263 3330 3739 3233 3632 3634  ut/src3079236264
 000007e0: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 000007f0: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000800: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000810: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000820: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000830: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000840: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto-0.2.8/src/roboto/cli/triggers/commands.py` & `roboto-0.2.9/src/roboto/cli/triggers/commands.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/users/__pycache__/commands.cpython-310.pyc` & `roboto-0.2.9/src/roboto/cli/users/__pycache__/commands.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3277 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 cd0c 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 cd0c 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4e01 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6402 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6402 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6406  d.l.m.Z.m.Z...d.
@@ -42,15 +42,15 @@
 00000290: 6672 6f6d 5f69 64da 0269 64da 0575 7365  from_id..id..use
 000002a0: 7273 da07 746f 5f64 6963 74da 0373 7973  rs..to_dict..sys
 000002b0: da06 7374 646f 7574 da05 7772 6974 65da  ..stdout..write.
 000002c0: 046a 736f 6eda 0564 756d 7073 2904 da04  .json..dumps)...
 000002d0: 6172 6773 720b 0000 0072 0c00 0000 da04  argsr....r......
 000002e0: 7573 6572 a900 721d 0000 00fa e22f 636f  user..r....../co
 000002f0: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-00000300: 7263 3130 3531 3138 3230 3839 2f73 7263  rc1051182089/src
+00000300: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
 00000310: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
 00000320: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
 00000330: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
 00000340: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
 00000350: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
 00000360: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
 00000370: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
```

### Comparing `roboto-0.2.8/src/roboto/cli/users/commands.py` & `roboto-0.2.9/src/roboto/cli/users/commands.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/cli/validation.py` & `roboto-0.2.9/src/roboto/cli/validation.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/__pycache__/http_delegates.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/__pycache__/http_delegates.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2677 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 750a 0000  o........Y.eu...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 750a 0000  o.......2H.eu...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6405 6407 6c09 6d0a 5a0a 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6408 6c0b 6d0c 5a0c 0100 6405 6409 6c0d  d.l.m.Z...d.d.l.
@@ -73,15 +73,15 @@
 00000480: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
 00000490: 7210 0000 0072 1200 0000 290c 721e 0000  r....r....).r...
 000004a0: 0072 1f00 0000 7214 0000 0072 1600 0000  .r....r....r....
 000004b0: 7217 0000 0072 1800 0000 7215 0000 0072  r....r....r....r
 000004c0: 1d00 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
 000004d0: 0000 0072 1c00 0000 a900 7222 0000 00fa  ...r......r"....
 000004e0: e52f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000004f0: 7574 2f73 7263 3130 3531 3138 3230 3839  ut/src1051182089
+000004f0: 7574 2f73 7263 3330 3739 3233 3632 3634  ut/src3079236264
 00000500: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 00000510: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000520: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000530: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000540: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000550: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000560: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__init__.py` & `roboto-0.2.9/src/roboto/domain/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2094 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 2e08 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 2e08 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 ec00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6406 6c0e  m.Z.m.Z...d.d.l.
@@ -93,15 +93,15 @@
 000005c0: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
 000005d0: 0000 721f 0000 0072 2000 0000 5a1c 696e  ..r....r ...Z.in
 000005e0: 766f 6361 7469 6f6e 5f72 756e 7469 6d65  vocation_runtime
 000005f0: 5f72 6573 6f75 7263 6573 7221 0000 0072  _resourcesr!...r
 00000600: 2200 0000 da07 5f5f 616c 6c5f 5fa9 0072  ".....__all__..r
 00000610: 2500 0000 7225 0000 00fa e72f 636f 6465  %...r%...../code
 00000620: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000630: 3130 3531 3138 3230 3839 2f73 7263 2f63  1051182089/src/c
+00000630: 3330 3739 3233 3632 3634 2f73 7263 2f63  3079236264/src/c
 00000640: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 00000650: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 00000660: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 00000670: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 00000680: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 00000690: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 000006a0: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/action.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/action.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 9326 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 6e24 0000  o........Y.en$..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 6e24 0000  o.......2H.en$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6403 6404 6c07 6d08 5a08 0100 6403  ..d.d.l.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6403 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6403  m.Z.m.Z.m.Z...d.
@@ -132,16 +132,16 @@
 00000830: 7469 6f6e 2910 da03 636c 7372 1f00 0000  tion)...clsr....
 00000840: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
 00000850: 2300 0000 7224 0000 0072 2500 0000 7226  #...r$...r%...r&
 00000860: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
 00000870: 0000 722a 0000 0072 2b00 0000 722c 0000  ..r*...r+...r,..
 00000880: 00da 0672 6563 6f72 64a9 0072 3400 0000  ...record..r4...
 00000890: fae5 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-000008a0: 7075 742f 7372 6331 3035 3131 3832 3038  put/src105118208
-000008b0: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+000008a0: 7075 742f 7372 6333 3037 3932 3336 3236  put/src307923626
+000008b0: 342f 7372 632f 636f 6465 7374 6172 2d63  4/src/codestar-c
 000008c0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 000008d0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 000008e0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 000008f0: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 00000900: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 00000910: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000920: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/action_container_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/action_container_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3165 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 5d0c 0000  o........Y.e]...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 5d0c 0000  o.......2H.e]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000060: 8400 6404 6502 6a06 8303 5a07 4700 6405  ..d.e.j...Z.G.d.
 00000070: 6406 8400 6406 6504 6a08 8303 5a09 4700  d...d.e.j...Z.G.
@@ -21,15 +21,15 @@
 00000140: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00000150: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00000160: 5f5a 094c 6f67 526f 7574 6572 da07 4d6f  _Z.LogRouter..Mo
 00000170: 6e69 746f 725a 0553 6574 7570 da06 4163  nitorZ.Setup..Ac
 00000180: 7469 6f6e 5a0d 4f75 7470 7574 4861 6e64  tionZ.OutputHand
 00000190: 6c65 72a9 0072 0c00 0000 720c 0000 00fa  ler..r....r.....
 000001a0: f92f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000001b0: 7574 2f73 7263 3130 3531 3138 3230 3839  ut/src1051182089
+000001b0: 7574 2f73 7263 3330 3739 3233 3632 3634  ut/src3079236264
 000001c0: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 000001d0: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 000001e0: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 000001f0: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000200: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000210: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000220: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/action_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/action_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3138 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 420c 0000  o........Y.eB...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 420c 0000  o.......2H.eB...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6403 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6403 6406 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6403 6407 6c0c 6d0d 5a0d 0100 6408  ..d.d.l.m.Z...d.
@@ -78,16 +78,16 @@
 000004d0: 6ea9 01da 134e 6f74 496d 706c 656d 656e  n....NotImplemen
 000004e0: 7465 6445 7272 6f72 290d da04 7365 6c66  tedError)...self
 000004f0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
 00000500: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
 00000510: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
 00000520: 0000 721e 0000 0072 1f00 0000 a900 7226  ..r....r......r&
 00000530: 0000 00fa ee2f 636f 6465 6275 696c 642f  ...../codebuild/
-00000540: 6f75 7470 7574 2f73 7263 3130 3531 3138  output/src105118
-00000550: 3230 3839 2f73 7263 2f63 6f64 6573 7461  2089/src/codesta
+00000540: 6f75 7470 7574 2f73 7263 3330 3739 3233  output/src307923
+00000550: 3632 3634 2f73 7263 2f63 6f64 6573 7461  6264/src/codesta
 00000560: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 00000570: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 00000580: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 00000590: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 000005a0: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 000005b0: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 000005c0: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 8201 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 0920 0000  o........Y.e. ..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 0920 0000  o.......2H.e. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6402 6403 6c04 6d05 5a05 0100 6402  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6402 6405 6c0a 6d0b 5a0b 0100 6402  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6402 6407 6c0e  d.l.m.Z...d.d.l.
@@ -96,15 +96,15 @@
 000005f0: 7400 8300 a001 a100 0100 7c02 7c00 5f02  t.........|.|._.
 00000600: 7c01 7c00 5f03 6400 5300 a901 4e29 04da  |.|._.d.S...N)..
 00000610: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
 00000620: 721e 0000 0072 1f00 0000 2903 da04 7365  r....r....)...se
 00000630: 6c66 7220 0000 0072 2100 0000 a901 da09  lfr ...r!.......
 00000640: 5f5f 636c 6173 735f 5fa9 00fa f32f 636f  __class__..../co
 00000650: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-00000660: 7263 3130 3531 3138 3230 3839 2f73 7263  rc1051182089/src
+00000660: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
 00000670: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
 00000680: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
 00000690: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
 000006a0: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
 000006b0: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
 000006c0: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
 000006d0: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/action_http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/action_http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2302 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 fe08 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 fe08 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 aa00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 5a04 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6404 6406 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6407 6408 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -59,16 +59,16 @@
 000003a0: 64da 046c 6973 7472 1500 0000 7203 0000  d..listr....r...
 000003b0: 0072 0f00 0000 7216 0000 0072 1700 0000  .r....r....r....
 000003c0: 7218 0000 0072 1100 0000 da04 6469 6374  r....r......dict
 000003d0: 7219 0000 0072 0200 0000 721a 0000 0072  r....r....r....r
 000003e0: 1b00 0000 720c 0000 0072 1c00 0000 720d  ....r....r....r.
 000003f0: 0000 0072 1d00 0000 a900 7227 0000 0072  ...r......r'...r
 00000400: 2700 0000 faf4 2f63 6f64 6562 7569 6c64  '...../codebuild
-00000410: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000420: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000410: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000420: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000430: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000440: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000450: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000460: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000470: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000480: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000490: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/action_record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/action_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 5697 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4116 0000  o........Y.eA...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 4116 0000  o.......2H.eA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c07 5a07 6400 6402 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6400 6403 6c0a 6d0b 5a0b 0100 6404  ..d.d.l.m.Z...d.
@@ -39,15 +39,15 @@
 00000260: 696f 6e5f 6875 624e 2906 da08 5f5f 6e61  ion_hubN)...__na
 00000270: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000280: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
 00000290: 5f5f 646f 635f 5fda 0c4f 7267 616e 697a  __doc__..Organiz
 000002a0: 6174 696f 6eda 0941 6374 696f 6e48 7562  ation..ActionHub
 000002b0: a900 7211 0000 0072 1100 0000 faec 2f63  ..r....r....../c
 000002c0: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-000002d0: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+000002d0: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 000002e0: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 000002f0: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 00000300: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 00000310: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 00000320: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 00000330: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 00000340: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 7657 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 e91d 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 e91d 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6403  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6403 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6403 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6407 6408 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
@@ -83,16 +83,16 @@
 00000520: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
 00000530: 7316 0000 007c 02a0 007c 017c 03a1 027d  s....|...|.|...}
 00000540: 047c 007c 047c 0283 0253 00a9 014e 2901  .|.|.|...S...N).
 00000550: da09 6765 745f 6279 5f69 6429 05da 0363  ..get_by_id)...c
 00000560: 6c73 7217 0000 0072 1800 0000 7219 0000  lsr....r....r...
 00000570: 00da 0672 6563 6f72 64a9 0072 1f00 0000  ...record..r....
 00000580: fae9 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-00000590: 7075 742f 7372 6331 3035 3131 3832 3038  put/src105118208
-000005a0: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+00000590: 7075 742f 7372 6333 3037 3932 3336 3236  put/src307923626
+000005a0: 342f 7372 632f 636f 6465 7374 6172 2d63  4/src/codestar-c
 000005b0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 000005c0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 000005d0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 000005e0: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 000005f0: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 00000600: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000610: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2506 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 ca09 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 ca09 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6406 6407 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6406 6408 6c0c 6d0d 5a0d 0100 6406  ..d.d.l.m.Z...d.
@@ -56,16 +56,16 @@
 00000370: 0000 0000 0000 0300 0000 0200 0000 4300  ..............C.
 00000380: 0000 f308 0000 0074 0064 0183 0182 0129  .......t.d.....)
 00000390: 024e da11 6361 6e63 656c 5f69 6e76 6f63  .N..cancel_invoc
 000003a0: 6174 696f 6ea9 01da 134e 6f74 496d 706c  ation....NotImpl
 000003b0: 656d 656e 7465 6445 7272 6f72 a903 da04  ementedError....
 000003c0: 7365 6c66 7212 0000 0072 1300 0000 a900  selfr....r......
 000003d0: 721b 0000 00fa f22f 636f 6465 6275 696c  r....../codebuil
-000003e0: 642f 6f75 7470 7574 2f73 7263 3130 3531  d/output/src1051
-000003f0: 3138 3230 3839 2f73 7263 2f63 6f64 6573  182089/src/codes
+000003e0: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+000003f0: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
 00000400: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 00000410: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 00000420: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 00000430: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 00000440: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 00000450: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 00000460: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 7117 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 cd1b 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 cd1b 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ca00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6403 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6403 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6403 6406 6c0c  m.Z.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 6403 6407 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
@@ -81,16 +81,16 @@
 00000500: 0000 0300 0000 731a 0000 0074 0083 00a0  ......s....t....
 00000510: 01a1 0001 007c 027c 005f 027c 017c 005f  .....|.|._.|.|._
 00000520: 0364 0053 00a9 014e 2904 da05 7375 7065  .d.S...N)...supe
 00000530: 72da 085f 5f69 6e69 745f 5f72 1900 0000  r..__init__r....
 00000540: 721a 0000 0029 03da 0473 656c 6672 1b00  r....)...selfr..
 00000550: 0000 721c 0000 00a9 01da 095f 5f63 6c61  ..r........__cla
 00000560: 7373 5f5f a900 faf7 2f63 6f64 6562 7569  ss__..../codebui
-00000570: 6c64 2f6f 7574 7075 742f 7372 6331 3035  ld/output/src105
-00000580: 3131 3832 3038 392f 7372 632f 636f 6465  1182089/src/code
+00000570: 6c64 2f6f 7574 7075 742f 7372 6333 3037  ld/output/src307
+00000580: 3932 3336 3236 342f 7372 632f 636f 6465  9236264/src/code
 00000590: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 000005a0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 000005b0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 000005c0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 000005d0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 000005e0: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 000005f0: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 827 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 3b03 0000  o........Y.e;...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 3b03 0000  o.......2H.e;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6403 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 4700 6406 6407  m.Z.m.Z...G.d.d.
 00000070: 8400 6407 6503 6a0b 8303 5a0c 4700 6408  ..d.e.j...Z.G.d.
@@ -45,16 +45,16 @@
 000002c0: 0000 7203 0000 00da 0464 6963 74da 0373  ..r......dict..s
 000002d0: 7472 7202 0000 00da 0f5f 5f61 6e6e 6f74  trr......__annot
 000002e0: 6174 696f 6e73 5f5f da04 6c69 7374 720d  ations__..listr.
 000002f0: 0000 0072 0500 0000 720e 0000 0072 0600  ...r....r....r..
 00000300: 0000 7207 0000 0072 0800 0000 7212 0000  ..r....r....r...
 00000310: 0072 1300 0000 a900 721b 0000 0072 1b00  .r......r....r..
 00000320: 0000 faf8 2f63 6f64 6562 7569 6c64 2f6f  ..../codebuild/o
-00000330: 7574 7075 742f 7372 6331 3035 3131 3832  utput/src1051182
-00000340: 3038 392f 7372 632f 636f 6465 7374 6172  089/src/codestar
+00000330: 7574 7075 742f 7372 6333 3037 3932 3336  utput/src3079236
+00000340: 3236 342f 7372 632f 636f 6465 7374 6172  264/src/codestar
 00000350: 2d63 6f6e 6e65 6374 696f 6e73 2e75 732d  -connections.us-
 00000360: 7765 7374 2d32 2e61 6d61 7a6f 6e61 7773  west-2.amazonaws
 00000370: 2e63 6f6d 2f67 6974 2d68 7474 702f 3036  .com/git-http/06
 00000380: 3631 3935 3131 3233 3835 2f75 732d 7765  6195112385/us-we
 00000390: 7374 2d32 2f65 3635 3032 6138 302d 6262  st-2/e6502a80-bb
 000003a0: 3465 2d34 6662 652d 3837 3263 2d35 6434  4e-4fbe-872c-5d4
 000003b0: 3263 3139 3336 3939 642f 726f 626f 746f  2c193699d/roboto
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation_record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 6240 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 6018 0000  o........Y.e`...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 6018 0000  o.......2H.e`...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6404 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
@@ -35,16 +35,16 @@
 00000220: 7220 616e 2041 6374 696f 6e27 7320 496e  r an Action's In
 00000230: 7075 7442 696e 6469 6e67 da07 4461 7461  putBinding..Data
 00000240: 7365 744e 2905 da08 5f5f 6e61 6d65 5f5f  setN)...__name__
 00000250: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 00000260: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
 00000270: 635f 5f72 0a00 0000 a900 720f 0000 0072  c__r......r....r
 00000280: 0f00 0000 faf0 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000290: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-000002a0: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000290: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+000002a0: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 000002b0: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 000002c0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000002d0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000002e0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000002f0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000300: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000310: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/__pycache__/invocation_runtime_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/actions/__pycache__/invocation_runtime_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 990 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 de03 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 de03 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 5a00 6402 5a01 4700 6403 6404  d.l.Z.d.Z.G.d.d.
 00000040: 8400 6404 6502 6500 6a03 8304 5a04 6401  ..d.e.e.j...Z.d.
 00000050: 5300 2905 e900 0000 004e 5a07 524f 424f  S.)......NZ.ROBO
 00000060: 544f 5f63 0000 0000 0000 0000 0000 0000  TO_c............
 00000070: 0000 0000 0200 0000 4000 0000 7376 0000  ........@...sv..
@@ -46,16 +46,16 @@
 000002d0: 6574 6164 6174 6143 6861 6e67 6573 6574  etadataChangeset
 000002e0: 4669 6c65 5a08 496e 7075 7444 6972 5a0c  FileZ.InputDirZ.
 000002f0: 496e 766f 6361 7469 6f6e 4964 5a05 4f72  InvocationIdZ.Or
 00000300: 6749 645a 094f 7574 7075 7444 6972 5a09  gIdZ.OutputDirZ.
 00000310: 526f 626f 746f 456e 765a 1052 6f62 6f74  RobotoEnvZ.Robot
 00000320: 6f53 6572 7669 6365 5572 6ca9 0072 0b00  oServiceUrl..r..
 00000330: 0000 720b 0000 00fa fb2f 636f 6465 6275  ..r....../codebu
-00000340: 696c 642f 6f75 7470 7574 2f73 7263 3130  ild/output/src10
-00000350: 3531 3138 3230 3839 2f73 7263 2f63 6f64  51182089/src/cod
+00000340: 696c 642f 6f75 7470 7574 2f73 7263 3330  ild/output/src30
+00000350: 3739 3233 3632 3634 2f73 7263 2f63 6f64  79236264/src/cod
 00000360: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 00000370: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 00000380: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 00000390: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 000003a0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 000003b0: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 000003c0: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto-0.2.8/src/roboto/domain/actions/action.py` & `roboto-0.2.9/src/roboto/domain/actions/action.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/action_container_resources.py` & `roboto-0.2.9/src/roboto/domain/actions/action_container_resources.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/action_delegate.py` & `roboto-0.2.9/src/roboto/domain/actions/action_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/action_http_delegate.py` & `roboto-0.2.9/src/roboto/domain/actions/action_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/action_http_resources.py` & `roboto-0.2.9/src/roboto/domain/actions/action_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/action_record.py` & `roboto-0.2.9/src/roboto/domain/actions/action_record.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/invocation.py` & `roboto-0.2.9/src/roboto/domain/actions/invocation.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/invocation_delegate.py` & `roboto-0.2.9/src/roboto/domain/actions/invocation_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/invocation_http_delegate.py` & `roboto-0.2.9/src/roboto/domain/actions/invocation_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/invocation_http_resources.py` & `roboto-0.2.9/src/roboto/domain/actions/invocation_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/invocation_record.py` & `roboto-0.2.9/src/roboto/domain/actions/invocation_record.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/actions/invocation_runtime_resources.py` & `roboto-0.2.9/src/roboto/domain/actions/invocation_runtime_resources.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/collections/__init__.py` & `roboto-0.2.9/src/roboto/domain/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/collections/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/collections/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 827 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 3b03 0000  o........Y.e;...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 3b03 0000  o.......2H.e;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
@@ -35,15 +35,15 @@
 00000220: 5f68 7474 705f 7265 736f 7572 6365 7205  _http_resourcer.
 00000230: 0000 0072 0600 0000 5a11 636f 6c6c 6563  ...r....Z.collec
 00000240: 7469 6f6e 5f72 6563 6f72 6472 0700 0000  tion_recordr....
 00000250: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
 00000260: 0b00 0000 720c 0000 00da 075f 5f61 6c6c  ....r......__all
 00000270: 5f5f a900 720f 0000 0072 0f00 0000 faeb  __..r....r......
 00000280: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000290: 742f 7372 6331 3035 3131 3832 3038 392f  t/src1051182089/
+00000290: 742f 7372 6333 3037 3932 3336 3236 342f  t/src3079236264/
 000002a0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 000002b0: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 000002c0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 000002d0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 000002e0: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 000002f0: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000300: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto-0.2.8/src/roboto/domain/collections/__pycache__/collection.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/collections/__pycache__/collection.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 4861 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 fd12 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 fd12 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6400 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6405 6406 6c0a 6d0b 5a0b 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6407 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
@@ -59,15 +59,15 @@
 000003a0: 1a00 0000 7400 8300 a001 a100 0100 7c02  ....t.........|.
 000003b0: 7c00 5f02 7c01 7c00 5f03 6400 5300 a901  |._.|.|._.d.S...
 000003c0: 4e29 04da 0573 7570 6572 da08 5f5f 696e  N)...super..__in
 000003d0: 6974 5f5f 720e 0000 0072 0f00 0000 2903  it__r....r....).
 000003e0: da04 7365 6c66 7210 0000 0072 1100 0000  ..selfr....r....
 000003f0: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
 00000400: ed2f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-00000410: 7574 2f73 7263 3130 3531 3138 3230 3839  ut/src1051182089
+00000410: 7574 2f73 7263 3330 3739 3233 3632 3634  ut/src3079236264
 00000420: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 00000430: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000440: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000450: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000460: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000470: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000480: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto-0.2.8/src/roboto/domain/collections/__pycache__/collection_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/collections/__pycache__/collection_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2679 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 770a 0000  o........Y.ew...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 770a 0000  o.......2H.ew...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 0100 6406  d.l.m.Z.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
@@ -60,16 +60,16 @@
 000003b0: 0000 7400 6401 8301 8201 2902 4eda 1163  ..t.d.....).N..c
 000003c0: 7265 6174 655f 636f 6c6c 6563 7469 6f6e  reate_collection
 000003d0: a901 da13 4e6f 7449 6d70 6c65 6d65 6e74  ....NotImplement
 000003e0: 6564 4572 726f 7229 07da 0473 656c 6672  edError)...selfr
 000003f0: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
 00000400: 0000 0072 1200 0000 7213 0000 00a9 0072  ...r....r......r
 00000410: 1a00 0000 faf6 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000420: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000430: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000420: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000430: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000440: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000450: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000460: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000470: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000480: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000490: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000004a0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/domain/collections/__pycache__/collection_http_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/collections/__pycache__/collection_http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 6721 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 411a 0000  o........Y.eA...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 411a 0000  o.......2H.eA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
@@ -70,16 +70,16 @@
 00000450: 655f 5f68 7474 705f 636c 6965 6e74 da0b  e__http_client..
 00000460: 6874 7470 5f63 6c69 656e 7463 0200 0000  http_clientc....
 00000470: 0000 0000 0000 0000 0200 0000 0200 0000  ................
 00000480: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
 00000490: 0053 00a9 014e 2901 7217 0000 0029 02da  .S...N).r....)..
 000004a0: 0473 656c 6672 1800 0000 a900 721b 0000  .selfr......r...
 000004b0: 00fa fb2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-000004c0: 7470 7574 2f73 7263 3130 3531 3138 3230  tput/src10511820
-000004d0: 3839 2f73 7263 2f63 6f64 6573 7461 722d  89/src/codestar-
+000004c0: 7470 7574 2f73 7263 3330 3739 3233 3632  tput/src30792362
+000004d0: 3634 2f73 7263 2f63 6f64 6573 7461 722d  64/src/codestar-
 000004e0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000004f0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 00000500: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 00000510: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 00000520: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 00000530: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000540: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto-0.2.8/src/roboto/domain/collections/__pycache__/collection_http_resource.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/collections/__pycache__/collection_http_resource.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 971 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 cb03 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 cb03 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6400 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6404 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6405 6406 6c08 6d09 5a09 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6407 6408 8400 6408 6503 6a0a 8303 5a0b  d.d...d.e.j...Z.
@@ -28,16 +28,16 @@
 000001b0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 000001c0: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0a00  .__qualname__r..
 000001d0: 0000 7202 0000 00da 0373 7472 da0f 5f5f  ..r......str..__
 000001e0: 616e 6e6f 7461 7469 6f6e 735f 5f72 0b00  annotations__r..
 000001f0: 0000 720c 0000 00da 046c 6973 7472 0800  ..r......listr..
 00000200: 0000 720d 0000 00a9 0072 1400 0000 7214  ..r......r....r.
 00000210: 0000 00fa fb2f 636f 6465 6275 696c 642f  ...../codebuild/
-00000220: 6f75 7470 7574 2f73 7263 3130 3531 3138  output/src105118
-00000230: 3230 3839 2f73 7263 2f63 6f64 6573 7461  2089/src/codesta
+00000220: 6f75 7470 7574 2f73 7263 3330 3739 3233  output/src307923
+00000230: 3632 3634 2f73 7263 2f63 6f64 6573 7461  6264/src/codesta
 00000240: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 00000250: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 00000260: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 00000270: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 00000280: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 00000290: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 000002a0: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto-0.2.8/src/roboto/domain/collections/__pycache__/collection_record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/collections/__pycache__/collection_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1697 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 a106 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 a106 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6402 6403 8400 6403 6504 6501 6a05 8304  d.d...d.e.e.j...
 00000060: 5a06 4700 6404 6405 8400 6405 6504 6501  Z.G.d.d...d.e.e.
 00000070: 6a05 8304 5a07 4700 6406 6407 8400 6407  j...Z.G.d.d...d.
@@ -17,16 +17,16 @@
 00000100: 436f 6c6c 6563 7469 6f6e 5265 736f 7572  CollectionResour
 00000110: 6365 5479 7065 da07 6461 7461 7365 74da  ceType..dataset.
 00000120: 0466 696c 654e 2905 da08 5f5f 6e61 6d65  .fileN)...__name
 00000130: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
 00000140: 5f5f 7175 616c 6e61 6d65 5f5f da07 4461  __qualname__..Da
 00000150: 7461 7365 74da 0446 696c 65a9 0072 0a00  taset..File..r..
 00000160: 0000 720a 0000 00fa f42f 636f 6465 6275  ..r....../codebu
-00000170: 696c 642f 6f75 7470 7574 2f73 7263 3130  ild/output/src10
-00000180: 3531 3138 3230 3839 2f73 7263 2f63 6f64  51182089/src/cod
+00000170: 696c 642f 6f75 7470 7574 2f73 7263 3330  ild/output/src30
+00000180: 3739 3233 3632 3634 2f73 7263 2f63 6f64  79236264/src/cod
 00000190: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 000001a0: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 000001b0: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 000001c0: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 000001d0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 000001e0: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 000001f0: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto-0.2.8/src/roboto/domain/collections/collection.py` & `roboto-0.2.9/src/roboto/domain/collections/collection.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/collections/collection_delegate.py` & `roboto-0.2.9/src/roboto/domain/collections/collection_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/collections/collection_http_delegate.py` & `roboto-0.2.9/src/roboto/domain/collections/collection_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/collections/collection_http_resource.py` & `roboto-0.2.9/src/roboto/domain/collections/collection_http_resource.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/collections/collection_record.py` & `roboto-0.2.9/src/roboto/domain/collections/collection_record.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/comments/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/comments/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 468 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 d401 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 d401 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6406 5a0c 6407 5300 2908 e901 0000  ..d.Z.d.S.).....
@@ -21,15 +21,15 @@
 00000140: 6572 0300 0000 5a0d 6874 7470 5f64 656c  er....Z.http_del
 00000150: 6567 6174 6572 0400 0000 5a0e 6874 7470  egater....Z.http
 00000160: 5f72 6573 6f75 7263 6573 7205 0000 0072  _resourcesr....r
 00000170: 0600 0000 da06 7265 636f 7264 7207 0000  ......recordr...
 00000180: 0072 0800 0000 da07 5f5f 616c 6c5f 5fa9  .r......__all__.
 00000190: 0072 0d00 0000 720d 0000 00fa e82f 636f  .r....r....../co
 000001a0: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-000001b0: 7263 3130 3531 3138 3230 3839 2f73 7263  rc1051182089/src
+000001b0: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
 000001c0: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
 000001d0: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
 000001e0: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
 000001f0: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
 00000200: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
 00000210: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
 00000220: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
```

### Comparing `roboto-0.2.8/src/roboto/domain/comments/__pycache__/comment.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/comments/__pycache__/comment.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3549 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 dd0d 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 dd0d 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6405  ..d.d.l.m.Z...d.
 00000050: 6406 6c05 6d06 5a06 0100 6405 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 4700 6408 6409  m.Z.m.Z...G.d.d.
 00000070: 8400 6409 8302 5a0a 6401 5300 290a e900  ..d...Z.d.S.)...
@@ -58,16 +58,16 @@
 00000390: 0cda 0363 6c73 720c 0000 0072 0d00 0000  ...clsr....r....
 000003a0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
 000003b0: 1100 0000 da08 6d65 6e74 696f 6e73 da0e  ......mentions..
 000003c0: 6d65 6e74 696f 6e5f 7475 706c 6573 da0c  mention_tuples..
 000003d0: 6469 7370 6c61 795f 6e61 6d65 da07 7573  display_name..us
 000003e0: 6572 5f69 64da 0672 6563 6f72 64a9 0072  er_id..record..r
 000003f0: 1c00 0000 fae7 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000400: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000410: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000400: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000410: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000420: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000430: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000440: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000450: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000460: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000470: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000480: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/domain/comments/__pycache__/delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/comments/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1964 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 ac07 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 ac07 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6405  ..d.d.l.m.Z...d.
 00000050: 6406 6c05 6d06 5a06 6d07 5a07 0100 4700  d.l.m.Z.m.Z...G.
 00000060: 6407 6408 8400 6408 6500 6a08 8303 5a09  d.d...d.e.j...Z.
 00000070: 6401 5300 2909 e900 0000 004e 2901 da08  d.S.)......N)...
@@ -43,16 +43,16 @@
 000002a0: 0000 00f3 0800 0000 7400 6401 8301 8201  ........t.d.....
 000002b0: 2902 4eda 0e63 7265 6174 655f 636f 6d6d  ).N..create_comm
 000002c0: 656e 74a9 01da 134e 6f74 496d 706c 656d  ent....NotImplem
 000002d0: 656e 7465 6445 7272 6f72 2907 da04 7365  entedError)...se
 000002e0: 6c66 7209 0000 0072 0a00 0000 720b 0000  lfr....r....r...
 000002f0: 0072 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
 00000300: a900 7215 0000 00fa e82f 636f 6465 6275  ..r....../codebu
-00000310: 696c 642f 6f75 7470 7574 2f73 7263 3130  ild/output/src10
-00000320: 3531 3138 3230 3839 2f73 7263 2f63 6f64  51182089/src/cod
+00000310: 696c 642f 6f75 7470 7574 2f73 7263 3330  ild/output/src30
+00000320: 3739 3233 3632 3634 2f73 7263 2f63 6f64  79236264/src/cod
 00000330: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 00000340: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 00000350: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 00000360: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 00000370: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 00000380: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 00000390: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto-0.2.8/src/roboto/domain/comments/__pycache__/http_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/comments/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 5153 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 2114 0000  o........Y.e!...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 2114 0000  o.......2H.e!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6402 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6406 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6406 6408 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
@@ -52,15 +52,15 @@
 00000330: 0200 0000 0200 0000 0300 0000 7314 0000  ............s...
 00000340: 0074 0083 00a0 01a1 0001 007c 017c 005f  .t.........|.|._
 00000350: 0264 0053 00a9 014e 2903 da05 7375 7065  .d.S...N)...supe
 00000360: 72da 085f 5f69 6e69 745f 5f72 1000 0000  r..__init__r....
 00000370: 2902 da04 7365 6c66 7211 0000 00a9 01da  )...selfr.......
 00000380: 095f 5f63 6c61 7373 5f5f a900 faed 2f63  .__class__..../c
 00000390: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-000003a0: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+000003a0: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 000003b0: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 000003c0: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 000003d0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 000003e0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 000003f0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 00000400: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 00000410: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/domain/comments/__pycache__/http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/comments/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 239 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 ef00 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 ef00 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6404 6405 8400 6405 6500 6a03  ..G.d.d...d.e.j.
 00000050: 8303 5a04 4700 6406 6407 8400 6407 6500  ..Z.G.d.d...d.e.
 00000060: 6a03 8303 5a05 6401 5300 2908 e900 0000  j...Z.d.S.).....
 00000070: 004e e901 0000 0029 01da 0a45 6e74 6974  .N.....)...Entit
@@ -16,16 +16,16 @@
 000000f0: 656e 7469 7479 5f69 64da 0c63 6f6d 6d65  entity_id..comme
 00000100: 6e74 5f74 6578 744e 2906 da08 5f5f 6e61  nt_textN)...__na
 00000110: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000120: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7203  ..__qualname__r.
 00000130: 0000 00da 0f5f 5f61 6e6e 6f74 6174 696f  .....__annotatio
 00000140: 6e73 5f5f da03 7374 72a9 0072 0d00 0000  ns__..str..r....
 00000150: 720d 0000 00fa ee2f 636f 6465 6275 696c  r....../codebuil
-00000160: 642f 6f75 7470 7574 2f73 7263 3130 3531  d/output/src1051
-00000170: 3138 3230 3839 2f73 7263 2f63 6f64 6573  182089/src/codes
+00000160: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+00000170: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
 00000180: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 00000190: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 000001a0: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 000001b0: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 000001c0: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 000001d0: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 000001e0: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto-0.2.8/src/roboto/domain/comments/__pycache__/record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/comments/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 776 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 0803 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 0803 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000050: 8400 6404 6504 6502 8304 5a05 4700 6405  ..d.e.e...Z.G.d.
 00000060: 6406 8400 6406 6503 6a06 8303 5a07 6401  d...d.e.j...Z.d.
 00000070: 5300 2907 e900 0000 004e 2901 da04 456e  S.)......N)...En
@@ -18,16 +18,16 @@
 00000110: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00000120: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00000130: 5fda 0641 6374 696f 6eda 0a43 6f6c 6c65  _..Action..Colle
 00000140: 6374 696f 6eda 0744 6174 6173 6574 da04  ction..Dataset..
 00000150: 4669 6c65 da0a 496e 766f 6361 7469 6f6e  File..Invocation
 00000160: da07 5472 6967 6765 72a9 0072 1200 0000  ..Trigger..r....
 00000170: 7212 0000 00fa e62f 636f 6465 6275 696c  r....../codebuil
-00000180: 642f 6f75 7470 7574 2f73 7263 3130 3531  d/output/src1051
-00000190: 3138 3230 3839 2f73 7263 2f63 6f64 6573  182089/src/codes
+00000180: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+00000190: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
 000001a0: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 000001b0: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 000001c0: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 000001d0: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 000001e0: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 000001f0: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 00000200: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto-0.2.8/src/roboto/domain/comments/comment.py` & `roboto-0.2.9/src/roboto/domain/comments/comment.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/comments/delegate.py` & `roboto-0.2.9/src/roboto/domain/comments/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/comments/http_delegate.py` & `roboto-0.2.9/src/roboto/domain/comments/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/comments/record.py` & `roboto-0.2.9/src/roboto/domain/comments/record.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/__init__.py` & `roboto-0.2.9/src/roboto/domain/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/datasets/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 678 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 a602 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 a602 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6405 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
@@ -29,16 +29,16 @@
 000001c0: da0d 6874 7470 5f64 656c 6567 6174 6572  ..http_delegater
 000001d0: 0500 0000 da0e 6874 7470 5f72 6573 6f75  ......http_resou
 000001e0: 7263 6573 7206 0000 0072 0700 0000 7208  rcesr....r....r.
 000001f0: 0000 0072 0900 0000 da06 7265 636f 7264  ...r......record
 00000200: 720a 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
 00000210: 075f 5f61 6c6c 5f5f a900 7213 0000 0072  .__all__..r....r
 00000220: 1300 0000 fae8 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000230: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000240: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000230: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000240: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000250: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000260: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000270: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000280: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000290: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000002a0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000002b0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/__pycache__/dataset.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/datasets/__pycache__/dataset.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 21457 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,1055 +1,1104 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 d153 0000  o........Y.e.S..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 b857 0000  o.......2H.e.W..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
+00000020: 0004 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
-00000060: 6402 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
-00000070: 0100 6400 6401 6c0c 5a0c 6403 6404 6c0d  ..d.d.l.Z.d.d.l.
-00000080: 6d0e 5a0e 0100 6403 6405 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
-00000090: 0100 6403 6406 6c11 6d12 5a12 0100 6403  ..d.d.l.m.Z...d.
-000000a0: 6407 6c13 6d14 5a14 0100 6403 6408 6c15  d.l.m.Z...d.d.l.
-000000b0: 6d16 5a16 6d17 5a17 6d18 5a18 0100 6403  m.Z.m.Z.m.Z...d.
-000000c0: 6409 6c19 6d1a 5a1a 6d1b 5a1b 6d1c 5a1c  d.l.m.Z.m.Z.m.Z.
-000000d0: 0100 640a 640b 6c1d 6d1e 5a1e 0100 640a  ..d.d.l.m.Z...d.
-000000e0: 640c 6c1f 6d20 5a20 6d21 5a21 6d22 5a22  d.l.m Z m!Z!m"Z"
-000000f0: 6d23 5a23 6d24 5a24 0100 640a 640d 6c25  m#Z#m$Z$..d.d.l%
-00000100: 6d26 5a26 0100 640e 640f 6c27 6d28 5a28  m&Z&..d.d.l'm(Z(
-00000110: 6d29 5a29 6d2a 5a2a 0100 640e 6410 6c2b  m)Z)m*Z*..d.d.l+
-00000120: 6d2c 5a2c 6d2d 5a2d 0100 6510 8300 5a2e  m,Z,m-Z-..e...Z.
-00000130: 6502 6a2f 4700 6411 6412 8400 6412 8302  e.j/G.d.d...d...
-00000140: 8301 5a30 4700 6413 6414 8400 6414 8302  ..Z0G.d.d...d...
-00000150: 5a31 6401 5300 2915 e900 0000 004e 2903  Z1d.S.)......N).
-00000160: da03 416e 79da 0843 616c 6c61 626c 65da  ..Any..Callable.
-00000170: 084f 7074 696f 6e61 6ce9 0300 0000 2901  .Optional.....).
-00000180: da0b 5065 726d 6973 7369 6f6e 7329 01da  ..Permissions)..
-00000190: 0e64 6566 6175 6c74 5f6c 6f67 6765 7229  .default_logger)
-000001a0: 01da 1251 7565 7279 5370 6563 6966 6963  ...QuerySpecific
-000001b0: 6174 696f 6e29 01da 1670 7964 616e 7469  ation)...pydanti
-000001c0: 635f 6a73 6f6e 6162 6c65 5f64 6963 7429  c_jsonable_dict)
-000001d0: 03da 1554 7261 6e73 6163 7469 6f6e 4d61  ...TransactionMa
-000001e0: 6e61 6765 7241 4243 da11 5472 616e 7361  nagerABC..Transa
-000001f0: 6374 696f 6e52 6563 6f72 64da 0f54 7261  ctionRecord..Tra
-00000200: 6e73 6163 7469 6f6e 5479 7065 2903 da11  nsactionType)...
-00000210: 4d65 7461 6461 7461 4368 616e 6765 7365  MetadataChangese
-00000220: 74da 0b53 7472 5365 7175 656e 6365 da0f  t..StrSequence..
-00000230: 5570 6461 7465 436f 6e64 6974 696f 6ee9  UpdateCondition.
-00000240: 0200 0000 2901 da10 496e 766f 6361 7469  ....)...Invocati
-00000250: 6f6e 456e 7656 6172 2905 da04 4669 6c65  onEnvVar)...File
-00000260: da0c 4669 6c65 4465 6c65 6761 7465 da0a  ..FileDelegate..
-00000270: 4669 6c65 5265 636f 7264 da07 4669 6c65  FileRecord..File
-00000280: 5461 67da 0d53 3343 7265 6465 6e74 6961  Tag..S3Credentia
-00000290: 6c73 2901 da1a 5471 646d 5072 6f67 7265  ls)...TqdmProgre
-000002a0: 7373 4d6f 6e69 746f 7246 6163 746f 7279  ssMonitorFactory
-000002b0: e901 0000 0029 03da 0b43 7265 6465 6e74  .....)...Credent
-000002c0: 6961 6c73 da0f 4461 7461 7365 7444 656c  ials..DatasetDel
-000002d0: 6567 6174 65da 0f53 746f 7261 6765 4c6f  egate..StorageLo
-000002e0: 6361 7469 6f6e 2902 da0d 4164 6d69 6e69  cation)...Admini
-000002f0: 7374 7261 746f 72da 0d44 6174 6173 6574  strator..Dataset
-00000300: 5265 636f 7264 6300 0000 0000 0000 0000  Recordc.........
-00000310: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-00000320: 2600 0000 6500 5a01 6400 5a02 5500 6503  &...e.Z.d.Z.U.e.
-00000330: 6504 6401 3c00 6503 6504 6402 3c00 6503  e.d.<.e.e.d.<.e.
-00000340: 6504 6403 3c00 6404 5300 2905 da0e 4669  e.d.<.d.S.)...Fi
-00000350: 6c65 5570 6c6f 6164 496e 666f da06 6275  leUploadInfo..bu
-00000360: 636b 6574 da03 6b65 79da 0e74 7261 6e73  cket..key..trans
-00000370: 6163 7469 6f6e 5f69 644e 2905 da08 5f5f  action_idN)...__
-00000380: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000390: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000003a0: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
-000003b0: 696f 6e73 5f5f a900 7227 0000 0072 2700  ions__..r'...r'.
-000003c0: 0000 fae7 2f63 6f64 6562 7569 6c64 2f6f  ..../codebuild/o
-000003d0: 7574 7075 742f 7372 6331 3035 3131 3832  utput/src1051182
-000003e0: 3038 392f 7372 632f 636f 6465 7374 6172  089/src/codestar
-000003f0: 2d63 6f6e 6e65 6374 696f 6e73 2e75 732d  -connections.us-
-00000400: 7765 7374 2d32 2e61 6d61 7a6f 6e61 7773  west-2.amazonaws
-00000410: 2e63 6f6d 2f67 6974 2d68 7474 702f 3036  .com/git-http/06
-00000420: 3631 3935 3131 3233 3835 2f75 732d 7765  6195112385/us-we
-00000430: 7374 2d32 2f65 3635 3032 6138 302d 6262  st-2/e6502a80-bb
-00000440: 3465 2d34 6662 652d 3837 3263 2d35 6434  4e-4fbe-872c-5d4
-00000450: 3263 3139 3336 3939 642f 726f 626f 746f  2c193699d/roboto
-00000460: 2d61 692f 726f 626f 746f 2d68 6f73 7465  -ai/roboto-hoste
-00000470: 642d 6170 702f 7061 636b 6167 6573 2f72  d-app/packages/r
-00000480: 6f62 6f74 6f2f 7372 632f 726f 626f 746f  oboto/src/roboto
-00000490: 2f64 6f6d 6169 6e2f 6461 7461 7365 7473  /domain/datasets
-000004a0: 2f64 6174 6173 6574 2e70 7972 1e00 0000  /dataset.pyr....
-000004b0: 2e00 0000 7308 0000 000a 0008 0208 010c  ....s...........
-000004c0: 0172 1e00 0000 6300 0000 0000 0000 0000  .r....c.........
-000004d0: 0000 0000 0000 0018 0000 0040 0000 0073  ...........@...s
-000004e0: 0204 0000 6500 5a01 6400 5a02 5500 6503  ....e.Z.d.Z.U.e.
-000004f0: 6504 6401 3c00 6505 6504 6402 3c00 6506  e.d.<.e.e.d.<.e.
-00000500: 6504 6403 3c00 6404 5a07 6508 6509 1900  e.d.<.d.Z.e.e...
-00000510: 6504 6405 3c00 650a 6504 6406 3c00 650b  e.d.<.e.e.d.<.e.
-00000520: 650c 6a0d 650e 6a0f 6404 6404 6404 6404  e.j.e.j.d.d.d.d.
-00000530: 6404 6607 6407 6503 6408 6505 6409 650a  d.f.d.e.d.e.d.e.
-00000540: 640a 650c 640b 650e 640c 6508 6510 1900  d.e.d.e.d.e.e...
-00000550: 640d 6508 6510 1900 640e 6508 6511 6510  d.e.e...d.e.e.e.
-00000560: 6512 6602 1900 1900 640f 6508 6513 6510  e.f.....d.e.e.e.
-00000570: 1900 1900 6410 6508 6510 1900 6411 6400  ....d.e.e...d.d.
-00000580: 6616 6412 6413 8405 8301 5a14 650b 0904  f.d.d.....Z.e...
-00000590: 645b 6414 6510 6407 6503 6408 6505 6409  d[d.e.d.e.d.e.d.
-000005a0: 650a 640c 6508 6510 1900 6411 6400 660c  e.d.e.e...d.d.f.
-000005b0: 6415 6416 8405 8301 5a15 650b 0904 645b  d.d.....Z.e...d[
-000005c0: 6417 6516 6407 6503 6408 6505 6409 650a  d.e.d.e.d.e.d.e.
-000005d0: 640c 6508 6510 1900 6411 6517 6a18 6a19  d.e.e...d.e.j.j.
-000005e0: 6418 1900 660c 6419 641a 8405 8301 5a1a  d...f.d.d.....Z.
-000005f0: 641b 6506 6407 6503 6408 6505 6409 650a  d.e.d.e.d.e.d.e.
-00000600: 6411 6404 660a 641c 641d 8404 5a1b 651c  d.d.f.d.d...Z.e.
-00000610: 6411 6510 6602 641e 641f 8404 8301 5a1d  d.e.f.d.d.....Z.
-00000620: 651c 6411 6511 6510 6512 6602 1900 6602  e.d.e.e.e.f...f.
-00000630: 6420 6421 8404 8301 5a1e 651c 6411 6506  d d!....Z.e.d.e.
-00000640: 6602 6422 6423 8404 8301 5a1f 651c 6411  f.d"d#....Z.e.d.
-00000650: 6513 6510 1900 6602 6424 6425 8404 8301  e.e...f.d$d%....
-00000660: 5a20 0904 0926 645c 6427 6510 6428 6508  Z ...&d\d'e.d(e.
-00000670: 6510 1900 6429 6521 6411 6404 6608 642a  e...d)e!d.d.f.d*
-00000680: 642b 8405 5a22 645d 642c 642d 8404 5a23  d+..Z"d]d,d-..Z#
-00000690: 0904 0904 645e 642e 6508 6513 6510 1900  ....d^d.e.e.e...
-000006a0: 1900 642f 6508 6513 6510 1900 1900 6411  ..d/e.e.e.....d.
-000006b0: 6404 6606 6430 6431 8405 5a24 0904 0904  d.f.d0d1..Z$....
-000006c0: 645e 6432 6525 6a26 642e 6508 6513 6510  d^d2e%j&d.e.e.e.
-000006d0: 1900 1900 642f 6508 6513 6510 1900 1900  ....d/e.e.e.....
-000006e0: 6411 6404 6608 6433 6434 8405 5a27 6528  d.d.f.d3d4..Z'e(
-000006f0: 6a29 6404 6435 6404 6604 6436 6528 6428  j)d.d5d.f.d6e(d(
-00000700: 6508 6510 1900 6437 652a 6427 6508 6510  e.e...d7e*d'e.e.
-00000710: 1900 6411 6509 660a 6438 6439 8405 5a2b  ..d.e.f.d8d9..Z+
-00000720: 0904 0904 645e 642e 6508 6513 6510 1900  ....d^d.e.e.e...
-00000730: 1900 642f 6508 6513 6510 1900 1900 6411  ..d/e.e.e.....d.
-00000740: 6517 6a18 6a19 652c 6404 6404 6603 1900  e.j.j.e,d.d.f...
-00000750: 6606 643a 643b 8405 5a2d 0904 645b 640e  f.d:d;..Z-..d[d.
-00000760: 6511 6510 6512 6602 1900 643c 6508 6510  e.e.e.f...d<e.e.
-00000770: 1900 6411 6404 6606 643d 643e 8405 5a2e  ..d.d.f.d=d>..Z.
-00000780: 0904 645b 640f 652f 643c 6508 6510 1900  ..d[d.e/d<e.e...
-00000790: 6411 6404 6606 643f 6440 8405 5a30 645d  d.d.f.d?d@..Z0d]
-000007a0: 6441 6442 8404 5a31 0904 645b 640e 652f  dAdB..Z1..d[d.e/
-000007b0: 643c 6508 6510 1900 6411 6404 6606 6443  d<e.e...d.d.f.dC
-000007c0: 6444 8405 5a32 0904 645b 640f 652f 643c  dD..Z2..d[d.e/d<
-000007d0: 6508 6510 1900 6411 6404 6606 6445 6446  e.e...d.d.f.dEdF
-000007e0: 8405 5a33 6411 6511 6510 6512 6602 1900  ..Z3d.e.e.e.f...
-000007f0: 6602 6447 6448 8404 5a34 0904 0926 645c  f.dGdH..Z4...&d\
-00000800: 6449 6525 6a26 642f 6508 6513 6510 1900  dIe%j&d/e.e.e...
-00000810: 1900 6429 6521 6411 6404 6608 644a 644b  ..d)e!d.d.f.dJdK
-00000820: 8405 5a35 0904 0904 645e 644c 6525 6a26  ..Z5....d^dLe%j&
-00000830: 644d 6510 644e 6508 6509 1900 644f 6508  dMe.dNe.e...dOe.
-00000840: 6536 6700 6537 6602 1900 1900 6411 6538  e6g.e7f.....d.e8
-00000850: 660a 6450 6451 8405 5a39 0904 0904 0904  f.dPdQ..Z9......
-00000860: 0904 645f 6452 6508 653a 1900 6453 6508  ..d_dRe.e:..dSe.
-00000870: 6513 653b 1900 1900 6410 6508 6510 1900  e.e;....d.e.e...
-00000880: 643c 6508 6510 1900 6411 6404 660a 6454  d<e.e...d.d.f.dT
-00000890: 6455 8405 5a3c 6456 6521 6411 653d 6604  dU..Z<dVe!d.e=f.
-000008a0: 6457 6458 8404 5a3e 0904 0904 645e 644c  dWdX..Z>....d^dL
-000008b0: 6525 6a26 644d 6510 6427 6510 644e 6508  e%j&dMe.d'e.dNe.
-000008c0: 6509 1900 644f 6508 6536 6700 6537 6602  e...dOe.e6g.e7f.
-000008d0: 1900 1900 6411 6538 660c 6459 645a 8405  ....d.e8f.dYdZ..
-000008e0: 5a3f 6404 5300 2960 da07 4461 7461 7365  Z?d.S.)`..Datase
-000008f0: 74da 1a5f 4461 7461 7365 745f 5f64 6174  t.._Dataset__dat
-00000900: 6173 6574 5f64 656c 6567 6174 65da 175f  aset_delegate.._
-00000910: 4461 7461 7365 745f 5f66 696c 655f 6465  Dataset__file_de
-00000920: 6c65 6761 7465 da10 5f44 6174 6173 6574  legate.._Dataset
-00000930: 5f5f 7265 636f 7264 4eda 1a5f 4461 7461  __recordN.._Data
-00000940: 7365 745f 5f74 656d 705f 6372 6564 656e  set__temp_creden
-00000950: 7469 616c 73da 1d5f 4461 7461 7365 745f  tials.._Dataset_
-00000960: 5f74 7261 6e73 6163 7469 6f6e 5f6d 616e  _transaction_man
-00000970: 6167 6572 da10 6461 7461 7365 745f 6465  ager..dataset_de
-00000980: 6c65 6761 7465 da0d 6669 6c65 5f64 656c  legate..file_del
-00000990: 6567 6174 65da 1374 7261 6e73 6163 7469  egate..transacti
-000009a0: 6f6e 5f6d 616e 6167 6572 da0d 6164 6d69  on_manager..admi
-000009b0: 6e69 7374 7261 746f 72da 1073 746f 7261  nistrator..stora
-000009c0: 6765 5f6c 6f63 6174 696f 6eda 066f 7267  ge_location..org
-000009d0: 5f69 64da 0a63 7265 6174 6564 5f62 79da  _id..created_by.
-000009e0: 086d 6574 6164 6174 61da 0474 6167 73da  .metadata..tags.
-000009f0: 0b64 6573 6372 6970 7469 6f6e da06 7265  .description..re
-00000a00: 7475 726e 630b 0000 0000 0000 0000 0000  turnc...........
-00000a10: 000c 0000 0009 0000 0043 0000 0073 2400  .........C...s$.
-00000a20: 0000 7c01 a000 7c04 7c08 7c05 7c09 7c06  ..|...|.|.|.|.|.
-00000a30: 7c07 7c0a a107 7d0b 7c00 7c0b 7c01 7c02  |.|...}.|.|.|.|.
-00000a40: 7c03 8304 5300 a901 4e29 015a 0e63 7265  |...S...N).Z.cre
-00000a50: 6174 655f 6461 7461 7365 7429 0cda 0363  ate_dataset)...c
-00000a60: 6c73 722f 0000 0072 3000 0000 7231 0000  lsr/...r0...r1..
-00000a70: 0072 3200 0000 7233 0000 0072 3400 0000  .r2...r3...r4...
-00000a80: 7235 0000 0072 3600 0000 7237 0000 0072  r5...r6...r7...r
-00000a90: 3800 0000 da06 7265 636f 7264 7227 0000  8.....recordr'..
-00000aa0: 0072 2700 0000 7228 0000 00da 0663 7265  .r'...r(.....cre
-00000ab0: 6174 653c 0000 0073 1400 0000 040e 0201  ate<...s........
-00000ac0: 0201 0201 0201 0201 0201 0201 04f9 0e09  ................
-00000ad0: 7a0e 4461 7461 7365 742e 6372 6561 7465  z.Dataset.create
-00000ae0: da0a 6461 7461 7365 745f 6964 6306 0000  ..dataset_idc...
-00000af0: 0000 0000 0000 0000 0007 0000 0005 0000  ................
-00000b00: 0043 0000 0073 1a00 0000 7c02 a000 7c01  .C...s....|...|.
-00000b10: 7c05 a102 7d06 7c00 7c06 7c02 7c03 7c04  |...}.|.|.|.|.|.
-00000b20: 8304 5300 723a 0000 0029 01da 1a67 6574  ..S.r:...)...get
-00000b30: 5f64 6174 6173 6574 5f62 795f 7072 696d  _dataset_by_prim
-00000b40: 6172 795f 6b65 7929 0772 3b00 0000 723e  ary_key).r;...r>
-00000b50: 0000 0072 2f00 0000 7230 0000 0072 3100  ...r/...r0...r1.
-00000b60: 0000 7234 0000 0072 3c00 0000 7227 0000  ..r4...r<...r'..
-00000b70: 0072 2700 0000 7228 0000 00da 0766 726f  .r'...r(.....fro
-00000b80: 6d5f 6964 5500 0000 7304 0000 000c 090e  m_idU...s.......
-00000b90: 017a 0f44 6174 6173 6574 2e66 726f 6d5f  .z.Dataset.from_
-00000ba0: 6964 da05 7175 6572 7929 0372 2900 0000  id..query).r)...
-00000bb0: 4e4e 6306 0000 0000 0000 0000 0000 000e  NNc.............
-00000bc0: 0000 0006 0000 0063 0000 0073 d800 0000  .......c...s....
-00000bd0: 8100 7400 7401 6a02 a003 a100 8301 7d06  ..t.t.j.......}.
-00000be0: 7400 8300 7d07 7c01 a004 a100 4400 5d16  t...}.|.....D.].
-00000bf0: 7d08 6401 7c08 7600 7220 7c07 a005 7c08  }.d.|.v.r |...|.
-00000c00: a006 6401 a101 6402 1900 a101 0100 710f  ..d...d.......q.
-00000c10: 7c07 a005 7c08 a101 0100 710f 7c07 7c06  |...|.....q.|.|.
-00000c20: 1800 7d09 7c09 7244 7407 7c09 8301 6403  ..}.|.rDt.|...d.
-00000c30: 6b04 7d0a 7c0a 7236 6404 6e01 6405 7d0b  k.}.|.r6d.n.d.}.
-00000c40: 7408 7c09 9b00 6406 7c0b 9b00 6407 7c06  t.|...d.|...d.|.
-00000c50: 9b00 9d05 8301 8201 7c02 6a09 7c01 7c05  ........|.j.|.|.
-00000c60: 6408 8d02 7d0c 0900 7c0c 6a0a 4400 5d0a  d...}...|.j.D.].
-00000c70: 7d0d 7c00 7c0d 7c02 7c03 7c04 8304 5600  }.|.|.|.|.|...V.
-00000c80: 0100 714f 7c0c 6a0b 7269 7c0c 6a0b 7c01  ..qO|.j.ri|.j.|.
-00000c90: 5f0c 7c02 6a09 7c01 7c05 6408 8d02 7d0c  _.|.j.|.|.d...}.
-00000ca0: 6e02 6400 5300 714c 2909 4eda 012e 7201  n.d.S.qL).N...r.
-00000cb0: 0000 0072 1800 0000 7a23 6172 6520 6e6f  ...r....z#are no
-00000cc0: 7420 6b6e 6f77 6e20 6174 7472 6962 7574  t known attribut
-00000cd0: 6573 206f 6620 4461 7461 7365 747a 2369  es of Datasetz#i
-00000ce0: 7320 6e6f 7420 6120 6b6e 6f77 6e20 6174  s not a known at
-00000cf0: 7472 6962 7574 6520 6f66 2044 6174 6173  tribute of Datas
-00000d00: 6574 da01 207a 142e 204b 6e6f 776e 2061  et.. z.. Known a
-00000d10: 7474 7269 6275 7465 733a 2029 0172 3400  ttributes: ).r4.
-00000d20: 0000 290d da03 7365 7472 1d00 0000 da0c  ..)...setr......
-00000d30: 6d6f 6465 6c5f 6669 656c 6473 da04 6b65  model_fields..ke
-00000d40: 7973 da06 6669 656c 6473 da03 6164 64da  ys..fields..add.
-00000d50: 0573 706c 6974 da03 6c65 6eda 0a56 616c  .split..len..Val
-00000d60: 7565 4572 726f 725a 0e71 7565 7279 5f64  ueErrorZ.query_d
-00000d70: 6174 6173 6574 73da 0569 7465 6d73 da0a  atasets..items..
-00000d80: 6e65 7874 5f74 6f6b 656e da05 6166 7465  next_token..afte
-00000d90: 7229 0e72 3b00 0000 7241 0000 0072 2f00  r).r;...rA...r/.
-00000da0: 0000 7230 0000 0072 3100 0000 7234 0000  ..r0...r1...r4..
-00000db0: 00da 056b 6e6f 776e da06 6163 7475 616c  ...known..actual
-00000dc0: da05 6669 656c 64da 0775 6e6b 6e6f 776e  ..field..unknown
-00000dd0: da06 706c 7572 616c da03 6d73 67da 1170  ..plural..msg..p
-00000de0: 6167 696e 6174 6564 5f72 6573 756c 7473  aginated_results
-00000df0: 723c 0000 0072 2700 0000 7227 0000 0072  r<...r'...r'...r
-00000e00: 2800 0000 7241 0000 0061 0000 0073 3400  (...rA...a...s4.
-00000e10: 0000 0280 0e09 0601 0c01 0803 1601 0c02  ................
-00000e20: 0801 0401 0c01 0203 06ff 0202 02fd 1805  ................
-00000e30: 0e02 0201 0a01 1201 0601 0801 0401 0401  ................
-00000e40: 08ff 0404 02f7 7a0d 4461 7461 7365 742e  ......z.Dataset.
-00000e50: 7175 6572 7972 3c00 0000 6305 0000 0000  queryr<...c.....
-00000e60: 0000 0000 0000 0005 0000 0002 0000 0043  ...............C
-00000e70: 0000 0073 1c00 0000 7c02 7c00 5f00 7c03  ...s....|.|._.|.
-00000e80: 7c00 5f01 7c01 7c00 5f02 7c04 7c00 5f03  |._.|.|._.|.|._.
-00000e90: 6400 5300 723a 0000 0029 0472 2a00 0000  d.S.r:...).r*...
-00000ea0: 722b 0000 0072 2c00 0000 722e 0000 0029  r+...r,...r....)
-00000eb0: 05da 0473 656c 6672 3c00 0000 722f 0000  ...selfr<...r/..
-00000ec0: 0072 3000 0000 7231 0000 0072 2700 0000  .r0...r1...r'...
-00000ed0: 7227 0000 0072 2800 0000 da08 5f5f 696e  r'...r(.....__in
-00000ee0: 6974 5f5f 8900 0000 7308 0000 0006 0706  it__....s.......
-00000ef0: 0106 010a 017a 1044 6174 6173 6574 2e5f  .....z.Dataset._
-00000f00: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00000f10: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000f20: 7308 0000 007c 006a 006a 0153 0072 3a00  s....|.j.j.S.r:.
-00000f30: 0000 2902 722c 0000 0072 3e00 0000 a901  ..).r,...r>.....
-00000f40: 7256 0000 0072 2700 0000 7227 0000 0072  rV...r'...r'...r
-00000f50: 2800 0000 723e 0000 0095 0000 0073 0200  (...r>.......s..
-00000f60: 0000 0802 7a12 4461 7461 7365 742e 6461  ....z.Dataset.da
-00000f70: 7461 7365 745f 6964 6301 0000 0000 0000  taset_idc.......
-00000f80: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00000f90: 00f3 0c00 0000 7c00 6a00 6a01 a002 a100  ......|.j.j.....
-00000fa0: 5300 723a 0000 0029 0372 2c00 0000 7236  S.r:...).r,...r6
-00000fb0: 0000 00da 0463 6f70 7972 5800 0000 7227  .....copyrX...r'
-00000fc0: 0000 0072 2700 0000 7228 0000 0072 3600  ...r'...r(...r6.
-00000fd0: 0000 9900 0000 f302 0000 000c 027a 1044  .............z.D
-00000fe0: 6174 6173 6574 2e6d 6574 6164 6174 6163  ataset.metadatac
-00000ff0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001000: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
-00001010: 0053 0072 3a00 0000 2901 722c 0000 0072  .S.r:...).r,...r
-00001020: 5800 0000 7227 0000 0072 2700 0000 7228  X...r'...r'...r(
-00001030: 0000 0072 3c00 0000 9d00 0000 7302 0000  ...r<.......s...
-00001040: 0006 027a 0e44 6174 6173 6574 2e72 6563  ...z.Dataset.rec
-00001050: 6f72 6463 0100 0000 0000 0000 0000 0000  ordc............
-00001060: 0100 0000 0200 0000 4300 0000 7259 0000  ........C...rY..
-00001070: 0072 3a00 0000 2903 722c 0000 0072 3700  .r:...).r,...r7.
-00001080: 0000 725a 0000 0072 5800 0000 7227 0000  ..rZ...rX...r'..
-00001090: 0072 2700 0000 7228 0000 0072 3700 0000  .r'...r(...r7...
-000010a0: a100 0000 725b 0000 007a 0c44 6174 6173  ....r[...z.Datas
-000010b0: 6574 2e74 6167 73e9 2c01 0000 7221 0000  et.tags.,...r!..
-000010c0: 00da 0663 616c 6c65 72da 0774 696d 656f  ...caller..timeo
-000010d0: 7574 6304 0000 0000 0000 0000 0000 0006  utc.............
-000010e0: 0000 0005 0000 0043 0000 0073 8600 0000  .......C...s....
-000010f0: 7400 a000 a100 7d04 6401 7d05 7c00 6a01  t.....}.d.}.|.j.
-00001100: a002 7c01 7c00 6a03 6a04 a102 7334 7400  ..|.|.j.j...s4t.
-00001110: a000 a100 7c04 1800 7c03 6b04 721b 7405  ....|...|.k.r.t.
-00001120: 6402 8301 8201 7c05 6401 6b04 722b 7400  d.....|.d.k.r+t.
-00001130: a006 7407 6403 7c05 1300 6403 1b00 6404  ..t.d.|...d...d.
-00001140: 8302 a101 0100 7c00 6a01 a002 7c01 7c00  ......|.j...|.|.
-00001150: 6a03 6a04 a102 720f 7c00 6a08 6a09 7c00  j.j...r.|.j.j.|.
-00001160: 6a0a 6a0b 7c01 7c00 6a0a 6a04 6405 8d03  j.j.|.|.j.j.d...
-00001170: 0100 6406 5300 2907 6197 0100 000a 2020  ..d.S.).a.....  
-00001180: 2020 2020 2020 4d61 726b 7320 616e 2075        Marks an u
-00001190: 706c 6f61 6420 6173 2027 636f 6d70 6c65  pload as 'comple
-000011a0: 7465 6427 2c20 7768 6963 6820 616c 6c6f  ted', which allo
-000011b0: 7773 2074 6865 2052 6f62 6f74 6f20 506c  ws the Roboto Pl
-000011c0: 6174 666f 726d 2074 6f20 6576 616c 7561  atform to evalua
-000011d0: 7465 2074 7269 6767 6572 7320 666f 7220  te triggers for 
-000011e0: 6175 746f 6d61 7469 6320 6163 7469 6f6e  automatic action
-000011f0: 206f 6e0a 2020 2020 2020 2020 696e 636f   on.        inco
-00001200: 6d69 6e67 2064 6174 612e 2054 6869 7320  ming data. This 
-00001210: 616c 736f 2061 6964 6573 2072 6570 6f72  also aides repor
-00001220: 7469 6e67 206f 6e20 7061 7274 6961 6c20  ting on partial 
-00001230: 7570 6c6f 6164 2066 6169 6c75 7265 2063  upload failure c
-00001240: 6173 6573 2e0a 0a20 2020 2020 2020 2054  ases...        T
-00001250: 6869 7320 4150 4920 6973 2063 616c 6c65  his API is calle
-00001260: 6420 696d 706c 6963 6974 6c79 2062 7920  d implicitly by 
-00001270: 7468 6520 6075 706c 6f61 645f 6669 6c65  the `upload_file
-00001280: 6020 616e 6420 6075 706c 6f61 645f 6469  ` and `upload_di
-00001290: 7265 6374 6f72 7960 206f 7065 7261 7469  rectory` operati
-000012a0: 6f6e 732c 2061 6e64 2073 686f 756c 6420  ons, and should 
-000012b0: 6f6e 6c79 2062 650a 2020 2020 2020 2020  only be.        
-000012c0: 7573 6564 2065 7870 6c69 6369 746c 7920  used explicitly 
-000012d0: 696e 2070 6f77 6572 2d75 7365 7220 7363  in power-user sc
-000012e0: 656e 6172 696f 732e 0a0a 2020 2020 2020  enarios...      
-000012f0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00001300: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
-00001310: 2020 2020 7201 0000 007a 2954 696d 6564      r....z)Timed
-00001320: 206f 7574 2077 6169 7469 6e67 2066 6f72   out waiting for
-00001330: 2075 706c 6f61 6420 746f 2063 6f6d 706c   upload to compl
-00001340: 6574 652e 7210 0000 00e9 1000 0000 2903  ete.r.........).
-00001350: 723e 0000 0072 2100 0000 7234 0000 004e  r>...r!...r4...N
-00001360: 290c da04 7469 6d65 722e 0000 005a 1769  )...timer....Z.i
-00001370: 735f 7472 616e 7361 6374 696f 6e5f 636f  s_transaction_co
-00001380: 6d70 6c65 7465 723c 0000 0072 3400 0000  mpleter<...r4...
-00001390: da0c 5469 6d65 6f75 7445 7272 6f72 da05  ..TimeoutError..
-000013a0: 736c 6565 70da 036d 696e 722a 0000 00da  sleep..minr*....
-000013b0: 0f63 6f6d 706c 6574 655f 7570 6c6f 6164  .complete_upload
-000013c0: 722c 0000 0072 3e00 0000 2906 7256 0000  r,...r>...).rV..
-000013d0: 0072 2100 0000 725d 0000 0072 5e00 0000  .r!...r]...r^...
-000013e0: da0a 7374 6172 745f 7469 6d65 da09 6974  ..start_time..it
-000013f0: 6572 6174 696f 6e72 2700 0000 7227 0000  erationr'...r'..
-00001400: 0072 2800 0000 7264 0000 00a5 0000 0073  .r(...rd.......s
-00001410: 2200 0000 0810 0401 0601 0801 04ff 1003  "...............
-00001420: 0801 0801 1801 06fa 0801 04ff 0608 0601  ................
-00001430: 0201 0601 0afd 7a17 4461 7461 7365 742e  ......z.Dataset.
-00001440: 636f 6d70 6c65 7465 5f75 706c 6f61 6463  complete_uploadc
-00001450: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001460: 0300 0000 4300 0000 7312 0000 007c 006a  ....C...s....|.j
-00001470: 00a0 017c 006a 02a1 0101 0064 0053 0072  ...|.j.....d.S.r
-00001480: 3a00 0000 2903 722a 0000 00da 0e64 656c  :...).r*.....del
-00001490: 6574 655f 6461 7461 7365 7472 2c00 0000  ete_datasetr,...
-000014a0: 7258 0000 0072 2700 0000 7227 0000 0072  rX...r'...r'...r
-000014b0: 2800 0000 7267 0000 00c5 0000 0073 0200  (...rg.......s..
-000014c0: 0000 1201 7a16 4461 7461 7365 742e 6465  ....z.Dataset.de
-000014d0: 6c65 7465 5f64 6174 6173 6574 da10 696e  lete_dataset..in
-000014e0: 636c 7564 655f 7061 7474 6572 6e73 da10  clude_patterns..
-000014f0: 6578 636c 7564 655f 7061 7474 6572 6e73  exclude_patterns
-00001500: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-00001510: 0004 0000 0043 0000 0073 1e00 0000 7c00  .....C...s....|.
-00001520: a000 7c01 7c02 a102 4400 5d06 7d03 7c03  ..|.|...D.].}.|.
-00001530: a001 a100 0100 7106 6401 5300 2902 61e0  ......q.d.S.).a.
-00001540: 0100 000a 2020 2020 2020 2020 4465 6c65  ....        Dele
-00001550: 7465 2066 696c 6573 2061 7373 6f63 6961  te files associa
-00001560: 7465 6420 7769 7468 2074 6869 7320 6461  ted with this da
-00001570: 7461 7365 742e 0a0a 2020 2020 2020 2020  taset...        
-00001580: 6069 6e63 6c75 6465 5f70 6174 7465 726e  `include_pattern
-00001590: 7360 2061 6e64 2060 6578 636c 7564 655f  s` and `exclude_
-000015a0: 7061 7474 6572 6e73 6020 6172 6520 6c69  patterns` are li
-000015b0: 7374 7320 6f66 2067 6974 6967 6e6f 7265  sts of gitignore
-000015c0: 2d73 7479 6c65 2070 6174 7465 726e 732e  -style patterns.
-000015d0: 0a20 2020 2020 2020 2053 6565 2068 7474  .        See htt
-000015e0: 7073 3a2f 2f67 6974 2d73 636d 2e63 6f6d  ps://git-scm.com
-000015f0: 2f64 6f63 732f 6769 7469 676e 6f72 652e  /docs/gitignore.
-00001600: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-00001610: 653a 0a20 2020 2020 2020 2020 2020 203e  e:.            >
-00001620: 3e3e 2066 726f 6d20 726f 626f 746f 2e64  >> from roboto.d
-00001630: 6f6d 6169 6e20 696d 706f 7274 2064 6174  omain import dat
-00001640: 6173 6574 730a 2020 2020 2020 2020 2020  asets.          
-00001650: 2020 3e3e 3e20 6461 7461 7365 7420 3d20    >>> dataset = 
-00001660: 6461 7461 7365 7473 2e44 6174 6173 6574  datasets.Dataset
-00001670: 282e 2e2e 290a 2020 2020 2020 2020 2020  (...).          
-00001680: 2020 3e3e 3e20 6461 7461 7365 742e 6465    >>> dataset.de
-00001690: 6c65 7465 5f66 696c 6573 280a 2020 2020  lete_files(.    
-000016a0: 2020 2020 2020 2020 2e2e 2e20 2020 2069          ...    i
-000016b0: 6e63 6c75 6465 5f70 6174 7465 726e 733d  nclude_patterns=
-000016c0: 5b22 2a2a 2f2a 2e70 6e67 225d 2c0a 2020  ["**/*.png"],.  
-000016d0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-000016e0: 2065 7863 6c75 6465 5f70 6174 7465 726e   exclude_pattern
-000016f0: 733d 5b22 2a2a 2f62 6163 6b5f 6361 6d65  s=["**/back_came
-00001700: 7261 2f2a 2a22 5d0a 2020 2020 2020 2020  ra/**"].        
-00001710: 2020 2020 2e2e 2e20 290a 0a20 2020 2020      ... )..     
-00001720: 2020 204e 2902 da0a 6c69 7374 5f66 696c     N)...list_fil
-00001730: 6573 da06 6465 6c65 7465 2904 7256 0000  es..delete).rV..
-00001740: 0072 6800 0000 7269 0000 00da 0466 696c  .rh...ri.....fil
-00001750: 6572 2700 0000 7227 0000 0072 2800 0000  er'...r'...r(...
-00001760: da0c 6465 6c65 7465 5f66 696c 6573 c800  ..delete_files..
-00001770: 0000 7306 0000 0010 140a 0104 ff7a 1444  ..s..........z.D
-00001780: 6174 6173 6574 2e64 656c 6574 655f 6669  ataset.delete_fi
-00001790: 6c65 73da 086f 7574 5f70 6174 6863 0400  les..out_pathc..
-000017a0: 0000 0000 0000 0000 0000 0600 0000 0800  ................
-000017b0: 0000 0300 0000 73b2 0000 0088 036a 006a  ......s......j.j
-000017c0: 0174 026a 036b 0373 0e88 036a 006a 0474  .t.j.k.s...j.j.t
-000017d0: 056a 066b 0372 1274 0764 0183 0182 0188  .j.k.r.t.d......
-000017e0: 02a0 08a1 0073 1c88 026a 0964 0264 038d  .....s...j.d.d..
-000017f0: 0101 0087 0366 0164 0464 0584 087d 0464  .....f.d.d...}.d
-00001800: 0674 0a64 0774 0b74 0c74 0d6a 0e66 0219  .t.d.t.t.t.j.f..
-00001810: 0066 0487 0266 0164 0864 0984 0c89 0074  .f...f.d.d.....t
-00001820: 0f88 03a0 107c 027c 03a1 0283 0189 0187  .....|.|........
-00001830: 0087 0166 0264 0a64 0b84 087d 0588 036a  ...f.d.d...}...j
-00001840: 116a 127c 0583 007c 0474 1364 0c88 036a  .j.|...|.t.d...j
-00001850: 006a 1474 1588 0183 0164 0d9c 0264 0e8d  .j.t.....d...d..
-00001860: 0264 0f64 108d 0401 0064 1153 0029 1261  .d.d.....d.S.).a
-00001870: 6702 0000 0a20 2020 2020 2020 2044 6f77  g....        Dow
-00001880: 6e6c 6f61 6420 6669 6c65 7320 6173 736f  nload files asso
-00001890: 6369 6174 6564 2077 6974 6820 7468 6973  ciated with this
-000018a0: 2064 6174 6173 6574 2074 6f20 7468 6520   dataset to the 
-000018b0: 6769 7665 6e20 6469 7265 6374 6f72 792e  given directory.
-000018c0: 0a20 2020 2020 2020 2049 6620 606f 7574  .        If `out
-000018d0: 5f70 6174 6860 2064 6f65 7320 6e6f 7420  _path` does not 
-000018e0: 6578 6973 742c 2069 7420 7769 6c6c 2062  exist, it will b
-000018f0: 6520 6372 6561 7465 642e 0a0a 2020 2020  e created...    
-00001900: 2020 2020 6069 6e63 6c75 6465 5f70 6174      `include_pat
-00001910: 7465 726e 7360 2061 6e64 2060 6578 636c  terns` and `excl
-00001920: 7564 655f 7061 7474 6572 6e73 6020 6172  ude_patterns` ar
-00001930: 6520 6c69 7374 7320 6f66 2067 6974 6967  e lists of gitig
-00001940: 6e6f 7265 2d73 7479 6c65 2070 6174 7465  nore-style patte
-00001950: 726e 732e 0a20 2020 2020 2020 2053 6565  rns..        See
-00001960: 2068 7474 7073 3a2f 2f67 6974 2d73 636d   https://git-scm
-00001970: 2e63 6f6d 2f64 6f63 732f 6769 7469 676e  .com/docs/gitign
-00001980: 6f72 652e 0a0a 2020 2020 2020 2020 4578  ore...        Ex
-00001990: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
-000019a0: 2020 203e 3e3e 2066 726f 6d20 726f 626f     >>> from robo
-000019b0: 746f 2e64 6f6d 6169 6e20 696d 706f 7274  to.domain import
-000019c0: 2064 6174 6173 6574 730a 2020 2020 2020   datasets.      
-000019d0: 2020 2020 2020 3e3e 3e20 6461 7461 7365        >>> datase
-000019e0: 7420 3d20 6461 7461 7365 7473 2e44 6174  t = datasets.Dat
-000019f0: 6173 6574 282e 2e2e 290a 2020 2020 2020  aset(...).      
-00001a00: 2020 2020 2020 3e3e 3e20 6461 7461 7365        >>> datase
-00001a10: 742e 646f 776e 6c6f 6164 5f66 696c 6573  t.download_files
-00001a20: 280a 2020 2020 2020 2020 2020 2020 2e2e  (.            ..
-00001a30: 2e20 2020 2020 7061 7468 6c69 622e 5061  .     pathlib.Pa
-00001a40: 7468 2822 2f74 6d70 2f74 6d70 2e6e 5631  th("/tmp/tmp.nV1
-00001a50: 6764 5735 5748 5622 292c 0a20 2020 2020  gdW5WHV"),.     
-00001a60: 2020 2020 2020 202e 2e2e 2020 2020 2069         ...     i
-00001a70: 6e63 6c75 6465 5f70 6174 7465 726e 733d  nclude_patterns=
-00001a80: 5b22 2a2a 2f2a 2e67 3422 5d2c 0a20 2020  ["**/*.g4"],.   
-00001a90: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
-00001aa0: 2065 7863 6c75 6465 5f70 6174 7465 726e   exclude_pattern
-00001ab0: 733d 5b22 2a2a 2f74 6573 742f 2a2a 225d  s=["**/test/**"]
-00001ac0: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00001ad0: 2029 0a20 2020 2020 2020 20fa 484f 6e6c   ).        .HOnl
-00001ae0: 7920 5333 2d62 6163 6b65 6420 7374 6f72  y S3-backed stor
-00001af0: 6167 6520 6164 6d69 6e69 7374 6572 6564  age administered
-00001b00: 2062 7920 526f 626f 746f 2069 7320 7375   by Roboto is su
-00001b10: 7070 6f72 7465 6420 6174 2074 6869 7320  pported at this 
-00001b20: 7469 6d65 2e54 2901 da07 7061 7265 6e74  time.T)...parent
-00001b30: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00001b40: 0000 0300 0000 1300 0000 7310 0000 0088  ..........s.....
-00001b50: 00a0 0074 016a 02a1 01a0 03a1 0053 0072  ...t.j.......S.r
-00001b60: 3a00 0000 2904 da19 6765 745f 7465 6d70  :...)...get_temp
-00001b70: 6f72 6172 795f 6372 6564 656e 7469 616c  orary_credential
-00001b80: 7372 0600 0000 da08 5265 6164 4f6e 6c79  sr......ReadOnly
-00001b90: da11 746f 5f73 335f 6372 6564 656e 7469  ..to_s3_credenti
-00001ba0: 616c 7372 2700 0000 7258 0000 0072 2700  alsr'...rX...r'.
-00001bb0: 0000 7228 0000 00da 145f 6372 6564 656e  ..r(....._creden
-00001bc0: 7469 616c 5f70 726f 7669 6465 7200 0100  tial_provider...
-00001bd0: 0073 0a00 0000 0401 0401 02ff 0402 02fe  .s..............
-00001be0: 7a34 4461 7461 7365 742e 646f 776e 6c6f  z4Dataset.downlo
-00001bf0: 6164 5f66 696c 6573 2e3c 6c6f 6361 6c73  ad_files.<locals
-00001c00: 3e2e 5f63 7265 6465 6e74 6961 6c5f 7072  >._credential_pr
-00001c10: 6f76 6964 6572 da01 6672 3900 0000 6301  ovider..fr9...c.
-00001c20: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00001c30: 0000 0013 0000 0073 1000 0000 7c00 6a00  .......s....|.j.
-00001c40: 8800 7c00 6a01 1b00 6602 5300 723a 0000  ..|.j...f.S.r:..
-00001c50: 0029 0272 3c00 0000 da0d 7265 6c61 7469  .).r<.....relati
-00001c60: 7665 5f70 6174 6829 0172 7500 0000 2901  ve_path).ru...).
-00001c70: 726e 0000 0072 2700 0000 7228 0000 00da  rn...r'...r(....
-00001c80: 175f 6669 6c65 5f74 6f5f 646f 776e 6c6f  ._file_to_downlo
-00001c90: 6164 5f74 7570 6c65 0501 0000 7302 0000  ad_tuple....s...
-00001ca0: 0010 017a 3744 6174 6173 6574 2e64 6f77  ...z7Dataset.dow
-00001cb0: 6e6c 6f61 645f 6669 6c65 732e 3c6c 6f63  nload_files.<loc
-00001cc0: 616c 733e 2e5f 6669 6c65 5f74 6f5f 646f  als>._file_to_do
-00001cd0: 776e 6c6f 6164 5f74 7570 6c65 6300 0000  wnload_tuplec...
-00001ce0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00001cf0: 0033 0000 0073 1c00 0000 8100 7400 8800  .3...s......t...
-00001d00: 8801 8302 4400 5d05 7d00 7c00 5600 0100  ....D.].}.|.V...
-00001d10: 7106 6400 5300 723a 0000 0029 01da 036d  q.d.S.r:...)...m
-00001d20: 6170 2901 da01 7829 0272 7700 0000 da09  ap)...x).rw.....
-00001d30: 616c 6c5f 6669 6c65 7372 2700 0000 7228  all_filesr'...r(
-00001d40: 0000 00da 0f5f 6669 6c65 5f67 656e 6572  ....._file_gener
-00001d50: 6174 6f72 0a01 0000 730e 0000 0002 8002  ator....s.......
-00001d60: 0102 0102 0108 fe08 0404 fc7a 2f44 6174  ...........z/Dat
-00001d70: 6173 6574 2e64 6f77 6e6c 6f61 645f 6669  aset.download_fi
-00001d80: 6c65 732e 3c6c 6f63 616c 733e 2e5f 6669  les.<locals>._fi
-00001d90: 6c65 5f67 656e 6572 6174 6f72 7218 0000  le_generatorr...
-00001da0: 0029 02da 0962 6173 655f 7061 7468 5a10  .)...base_pathZ.
-00001db0: 746f 7461 6c5f 6669 6c65 5f63 6f75 6e74  total_file_count
-00001dc0: a902 da0b 636f 6e63 7572 7265 6e63 79da  ....concurrency.
-00001dd0: 0363 7478 e908 0000 0029 04da 0e66 696c  .ctx.....)...fil
-00001de0: 655f 6765 6e65 7261 746f 72da 1363 7265  e_generator..cre
-00001df0: 6465 6e74 6961 6c5f 7072 6f76 6964 6572  dential_provider
-00001e00: da18 7072 6f67 7265 7373 5f6d 6f6e 6974  ..progress_monit
-00001e10: 6f72 5f66 6163 746f 7279 da0f 6d61 785f  or_factory..max_
-00001e20: 636f 6e63 7572 7265 6e63 794e 2916 722c  concurrencyN).r,
-00001e30: 0000 0072 3300 0000 721b 0000 00da 0253  ...r3...r......S
-00001e40: 3372 3200 0000 721c 0000 00da 0652 6f62  3r2...r......Rob
-00001e50: 6f74 6fda 134e 6f74 496d 706c 656d 656e  oto..NotImplemen
-00001e60: 7465 6445 7272 6f72 da06 6973 5f64 6972  tedError..is_dir
-00001e70: da05 6d6b 6469 7272 1200 0000 da05 7475  ..mkdirr......tu
-00001e80: 706c 6572 1400 0000 da07 7061 7468 6c69  pler......pathli
-00001e90: 62da 0450 6174 68da 046c 6973 7472 6a00  b..Path..listrj.
-00001ea0: 0000 722b 0000 00da 0e64 6f77 6e6c 6f61  ..r+.....downloa
-00001eb0: 645f 6669 6c65 7372 1700 0000 723e 0000  d_filesr....r>..
-00001ec0: 0072 4a00 0000 2906 7256 0000 0072 6e00  .rJ...).rV...rn.
-00001ed0: 0000 7268 0000 0072 6900 0000 7274 0000  ..rh...ri...rt..
-00001ee0: 0072 7b00 0000 7227 0000 0029 0472 7700  .r{...r'...).rw.
-00001ef0: 0000 727a 0000 0072 6e00 0000 7256 0000  ..rz...rn...rV..
-00001f00: 0072 2800 0000 728e 0000 00df 0000 0073  .r(...r........s
-00001f10: 2c00 0000 0e17 0e01 0202 0201 04ff 0804  ,...............
-00001f20: 0c01 0c02 2005 1003 0e02 0607 0401 0201  .... ...........
-00001f30: 0201 0201 0602 0601 04fe 04fe 0207 0af6  ................
-00001f40: 7a16 4461 7461 7365 742e 646f 776e 6c6f  z.Dataset.downlo
-00001f50: 6164 5f66 696c 6573 46da 0b70 6572 6d69  ad_filesF..permi
-00001f60: 7373 696f 6e73 da0d 666f 7263 655f 7265  ssions..force_re
-00001f70: 6672 6573 6863 0500 0000 0000 0000 0000  freshc..........
-00001f80: 0000 0500 0000 0600 0000 4300 0000 733e  ..........C...s>
-00001f90: 0000 007c 0373 117c 0174 006a 016b 0273  ...|.s.|.t.j.k.s
-00001fa0: 117c 006a 0264 0075 0073 117c 006a 02a0  .|.j.d.u.s.|.j..
-00001fb0: 03a1 0072 1c7c 006a 04a0 057c 006a 067c  ...r.|.j...|.j.|
-00001fc0: 017c 027c 04a1 047c 005f 027c 006a 0253  .|.|...|._.|.j.S
-00001fd0: 0072 3a00 0000 2907 7206 0000 00da 0952  .r:...).r......R
-00001fe0: 6561 6457 7269 7465 722d 0000 00da 0a69  eadWriter-.....i
-00001ff0: 735f 6578 7069 7265 6472 2a00 0000 7271  s_expiredr*...rq
-00002000: 0000 0072 2c00 0000 2905 7256 0000 0072  ...r,...).rV...r
-00002010: 8f00 0000 725d 0000 0072 9000 0000 7221  ....r]...r....r!
-00002020: 0000 0072 2700 0000 7227 0000 0072 2800  ...r'...r'...r(.
-00002030: 0000 7271 0000 001e 0100 0073 1400 0000  ..rq.......s....
-00002040: 0208 02ff 0a02 0a01 0801 02ff 0603 0a01  ................
-00002050: 06ff 0603 7a21 4461 7461 7365 742e 6765  ....z!Dataset.ge
-00002060: 745f 7465 6d70 6f72 6172 795f 6372 6564  t_temporary_cred
-00002070: 656e 7469 616c 7363 0300 0000 0000 0000  entialsc........
-00002080: 0000 0000 0500 0000 0700 0000 6300 0000  ............c...
-00002090: 7368 0000 0081 007c 006a 006a 017c 006a  sh.....|.j.j.|.j
-000020a0: 026a 037c 006a 026a 047c 017c 0264 018d  .j.|.j.j.|.|.d..
-000020b0: 047d 0309 007c 036a 0544 005d 097d 0474  .}...|.j.D.].}.t
-000020c0: 067c 047c 006a 0783 0256 0001 0071 137c  .|.|.j...V...q.|
-000020d0: 036a 0872 317c 006a 006a 017c 006a 026a  .j.r1|.j.j.|.j.j
-000020e0: 037c 006a 026a 047c 036a 087c 017c 0264  .|.j.j.|.j.|.|.d
-000020f0: 018d 057d 036e 0264 0353 0071 1029 0461  ...}.n.d.S.q.).a
-00002100: 1002 0000 0a20 2020 2020 2020 204c 6973  .....        Lis
-00002110: 7420 6669 6c65 7320 6173 736f 6369 6174  t files associat
-00002120: 6564 2077 6974 6820 7468 6973 2064 6174  ed with this dat
-00002130: 6173 6574 2e0a 0a20 2020 2020 2020 2060  aset...        `
-00002140: 696e 636c 7564 655f 7061 7474 6572 6e73  include_patterns
-00002150: 6020 616e 6420 6065 7863 6c75 6465 5f70  ` and `exclude_p
-00002160: 6174 7465 726e 7360 2061 7265 206c 6973  atterns` are lis
-00002170: 7473 206f 6620 6769 7469 676e 6f72 652d  ts of gitignore-
-00002180: 7374 796c 6520 7061 7474 6572 6e73 2e0a  style patterns..
-00002190: 2020 2020 2020 2020 5365 6520 6874 7470          See http
-000021a0: 733a 2f2f 6769 742d 7363 6d2e 636f 6d2f  s://git-scm.com/
-000021b0: 646f 6373 2f67 6974 6967 6e6f 7265 2e0a  docs/gitignore..
-000021c0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-000021d0: 3a0a 2020 2020 2020 2020 2020 2020 3e3e  :.            >>
-000021e0: 3e20 6672 6f6d 2072 6f62 6f74 6f2e 646f  > from roboto.do
-000021f0: 6d61 696e 2069 6d70 6f72 7420 6461 7461  main import data
-00002200: 7365 7473 0a20 2020 2020 2020 2020 2020  sets.           
-00002210: 203e 3e3e 2064 6174 6173 6574 203d 2064   >>> dataset = d
-00002220: 6174 6173 6574 732e 4461 7461 7365 7428  atasets.Dataset(
-00002230: 2e2e 2e29 0a20 2020 2020 2020 2020 2020  ...).           
-00002240: 203e 3e3e 2066 6f72 2066 696c 6520 696e   >>> for file in
-00002250: 2064 6174 6173 6574 2e6c 6973 745f 6669   dataset.list_fi
-00002260: 6c65 7328 0a20 2020 2020 2020 2020 2020  les(.           
-00002270: 202e 2e2e 2020 2020 2069 6e63 6c75 6465   ...     include
-00002280: 5f70 6174 7465 726e 733d 5b22 2a2a 2f2a  _patterns=["**/*
-00002290: 2e67 3422 5d2c 0a20 2020 2020 2020 2020  .g4"],.         
-000022a0: 2020 202e 2e2e 2020 2020 2065 7863 6c75     ...     exclu
-000022b0: 6465 5f70 6174 7465 726e 733d 5b22 2a2a  de_patterns=["**
-000022c0: 2f74 6573 742f 2a2a 225d 0a20 2020 2020  /test/**"].     
-000022d0: 2020 2020 2020 202e 2e2e 2029 3a0a 2020         ... ):.  
-000022e0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-000022f0: 2020 7072 696e 7428 6669 6c65 2e72 656c    print(file.rel
-00002300: 6174 6976 655f 7061 7468 290a 2020 2020  ative_path).    
-00002310: 2020 2020 2902 7268 0000 0072 6900 0000      ).rh...ri...
-00002320: 544e 2909 722a 0000 0072 6a00 0000 722c  TN).r*...rj...r,
-00002330: 0000 0072 3e00 0000 7234 0000 0072 4c00  ...r>...r4...rL.
-00002340: 0000 7212 0000 0072 2b00 0000 724d 0000  ..r....r+...rM..
-00002350: 0029 0572 5600 0000 7268 0000 0072 6900  .).rV...rh...ri.
-00002360: 0000 7255 0000 0072 3c00 0000 7227 0000  ..rU...r<...r'..
-00002370: 0072 2700 0000 7228 0000 0072 6a00 0000  .r'...r(...rj...
-00002380: 3001 0000 7328 0000 0002 8006 1506 0106  0...s(..........
-00002390: 0102 0102 0106 fc02 060a 0110 0106 0106  ................
-000023a0: 0106 0106 0104 0102 0102 0108 fb04 0802  ................
-000023b0: f47a 1244 6174 6173 6574 2e6c 6973 745f  .z.Dataset.list_
-000023c0: 6669 6c65 73da 0a75 7064 6174 6564 5f62  files..updated_b
-000023d0: 7963 0300 0000 0000 0000 0000 0000 0300  yc..............
-000023e0: 0000 0400 0000 4300 0000 f318 0000 007c  ......C........|
-000023f0: 006a 0074 017c 0164 018d 017c 0264 028d  .j.t.|.d...|.d..
-00002400: 0201 0064 0353 0029 0461 c101 0000 0a20  ...d.S.).a..... 
-00002410: 2020 2020 2020 2053 6574 2065 6163 6820         Set each 
-00002420: 606b 6579 603a 2060 7661 6c75 6560 2069  `key`: `value` i
-00002430: 6e20 7468 6973 2064 6963 7420 6173 2064  n this dict as d
-00002440: 6174 6173 6574 206d 6574 6164 6174 6120  ataset metadata 
-00002450: 6966 2069 7420 646f 6573 6e27 7420 6578  if it doesn't ex
-00002460: 6973 742c 2065 6c73 6520 6f76 6572 7772  ist, else overwr
-00002470: 6974 6520 7468 6520 6578 6973 7469 6e67  ite the existing
-00002480: 2076 616c 7565 2e0a 2020 2020 2020 2020   value..        
-00002490: 4b65 7973 206d 7573 7420 6265 2073 7472  Keys must be str
-000024a0: 696e 6773 2e20 446f 7420 6e6f 7461 7469  ings. Dot notati
-000024b0: 6f6e 2069 7320 7375 7070 6f72 7465 6420  on is supported 
-000024c0: 666f 7220 6e65 7374 6564 206b 6579 732e  for nested keys.
-000024d0: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-000024e0: 653a 0a20 2020 2020 2020 2020 2020 203e  e:.            >
-000024f0: 3e3e 2066 726f 6d20 726f 626f 746f 2e64  >> from roboto.d
-00002500: 6f6d 6169 6e20 696d 706f 7274 2064 6174  omain import dat
-00002510: 6173 6574 730a 2020 2020 2020 2020 2020  asets.          
-00002520: 2020 3e3e 3e20 6461 7461 7365 7420 3d20    >>> dataset = 
-00002530: 6461 7461 7365 7473 2e44 6174 6173 6574  datasets.Dataset
-00002540: 282e 2e2e 290a 2020 2020 2020 2020 2020  (...).          
-00002550: 2020 3e3e 3e20 6461 7461 7365 742e 7075    >>> dataset.pu
-00002560: 745f 6d65 7461 6461 7461 287b 0a20 2020  t_metadata({.   
-00002570: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
-00002580: 2022 666f 6f22 3a20 2262 6172 222c 0a20   "foo": "bar",. 
-00002590: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
-000025a0: 2020 2022 6261 7a2e 7175 7822 3a20 3130     "baz.qux": 10
-000025b0: 312c 0a20 2020 2020 2020 2020 2020 202e  1,.            .
-000025c0: 2e2e 207d 290a 0a20 2020 2020 2020 2029  .. })..        )
-000025d0: 01da 0a70 7574 5f66 6965 6c64 73a9 02da  ...put_fields...
-000025e0: 126d 6574 6164 6174 615f 6368 616e 6765  .metadata_change
-000025f0: 7365 7472 9300 0000 4ea9 02da 0675 7064  setr....N....upd
-00002600: 6174 6572 0d00 0000 a903 7256 0000 0072  ater......rV...r
-00002610: 3600 0000 7293 0000 0072 2700 0000 7227  6...r....r'...r'
-00002620: 0000 0072 2800 0000 da0c 7075 745f 6d65  ...r(.....put_me
-00002630: 7461 6461 7461 5901 0000 7308 0000 0004  tadataY...s.....
-00002640: 1208 0102 010a fe7a 1444 6174 6173 6574  .......z.Dataset
-00002650: 2e70 7574 5f6d 6574 6164 6174 6163 0300  .put_metadatac..
-00002660: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00002670: 0000 4300 0000 7294 0000 0029 047a 3141  ..C...r....).z1A
-00002680: 6464 2065 6163 6820 7461 6720 696e 2074  dd each tag in t
-00002690: 6869 7320 7365 7175 656e 6365 2069 6620  his sequence if 
-000026a0: 6974 2064 6f65 736e 2774 2065 7869 7374  it doesn't exist
-000026b0: 2901 da08 7075 745f 7461 6773 7296 0000  )...put_tagsr...
-000026c0: 004e 7298 0000 00a9 0372 5600 0000 7237  .Nr......rV...r7
-000026d0: 0000 0072 9300 0000 7227 0000 0072 2700  ...r....r'...r'.
-000026e0: 0000 7228 0000 0072 9c00 0000 7001 0000  ..r(...r....p...
-000026f0: f308 0000 0004 0608 0102 010a fe7a 1044  .............z.D
-00002700: 6174 6173 6574 2e70 7574 5f74 6167 7363  ataset.put_tagsc
-00002710: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00002720: 0400 0000 4300 0000 731c 0000 007c 006a  ....C...s....|.j
-00002730: 00a0 017c 006a 026a 037c 006a 026a 04a1  ...|.j.j.|.j.j..
-00002740: 027c 005f 0264 0153 0029 027a 4352 6566  .|._.d.S.).zCRef
-00002750: 7265 7368 2074 6865 2075 6e64 6572 6c79  resh the underly
-00002760: 696e 6720 6461 7461 7365 7420 7265 636f  ing dataset reco
-00002770: 7264 2077 6974 6820 7468 6520 6c61 7465  rd with the late
-00002780: 7374 2073 6572 7665 7220 7374 6174 652e  st server state.
-00002790: 4e29 0572 2a00 0000 723f 0000 0072 2c00  N).r*...r?...r,.
-000027a0: 0000 723e 0000 0072 3400 0000 7258 0000  ..r>...r4...rX..
-000027b0: 0072 2700 0000 7227 0000 0072 2800 0000  .r'...r'...r(...
-000027c0: da07 7265 6672 6573 687b 0100 0073 0600  ..refresh{...s..
-000027d0: 0000 0602 0c01 0aff 7a0f 4461 7461 7365  ........z.Datase
-000027e0: 742e 7265 6672 6573 6863 0300 0000 0000  t.refreshc......
-000027f0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00002800: 0000 7294 0000 0029 0461 5001 0000 0a20  ..r....).aP.... 
-00002810: 2020 2020 2020 2052 656d 6f76 6520 6561         Remove ea
-00002820: 6368 206b 6579 2069 6e20 7468 6973 2073  ch key in this s
-00002830: 6571 7565 6e63 6520 6672 6f6d 2064 6174  equence from dat
-00002840: 6173 6574 206d 6574 6164 6174 6120 6966  aset metadata if
-00002850: 2069 7420 6578 6973 7473 2e0a 2020 2020   it exists..    
-00002860: 2020 2020 4b65 7973 206d 7573 7420 6265      Keys must be
-00002870: 2073 7472 696e 6773 2e20 446f 7420 6e6f   strings. Dot no
-00002880: 7461 7469 6f6e 2069 7320 7375 7070 6f72  tation is suppor
-00002890: 7465 6420 666f 7220 6e65 7374 6564 206b  ted for nested k
-000028a0: 6579 732e 0a0a 2020 2020 2020 2020 4578  eys...        Ex
-000028b0: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
-000028c0: 2020 203e 3e3e 2066 726f 6d20 726f 626f     >>> from robo
-000028d0: 746f 2e64 6f6d 6169 6e20 696d 706f 7274  to.domain import
-000028e0: 2064 6174 6173 6574 730a 2020 2020 2020   datasets.      
-000028f0: 2020 2020 2020 3e3e 3e20 6461 7461 7365        >>> datase
-00002900: 7420 3d20 6461 7461 7365 7473 2e44 6174  t = datasets.Dat
-00002910: 6173 6574 282e 2e2e 290a 2020 2020 2020  aset(...).      
-00002920: 2020 2020 2020 3e3e 3e20 6461 7461 7365        >>> datase
-00002930: 742e 7265 6d6f 7665 5f6d 6574 6164 6174  t.remove_metadat
-00002940: 6128 5b22 666f 6f22 2c20 2262 617a 2e71  a(["foo", "baz.q
-00002950: 7578 225d 290a 2020 2020 2020 2020 2901  ux"]).        ).
-00002960: da0d 7265 6d6f 7665 5f66 6965 6c64 7372  ..remove_fieldsr
-00002970: 9600 0000 4e72 9800 0000 729a 0000 0072  ....Nr....r....r
-00002980: 2700 0000 7227 0000 0072 2800 0000 da0f  '...r'...r(.....
-00002990: 7265 6d6f 7665 5f6d 6574 6164 6174 6181  remove_metadata.
-000029a0: 0100 0073 0800 0000 040e 0801 0201 0afe  ...s............
-000029b0: 7a17 4461 7461 7365 742e 7265 6d6f 7665  z.Dataset.remove
-000029c0: 5f6d 6574 6164 6174 6163 0300 0000 0000  _metadatac......
-000029d0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-000029e0: 0000 7294 0000 0029 047a 2d52 656d 6f76  ..r....).z-Remov
-000029f0: 6520 6561 6368 2074 6167 2069 6e20 7468  e each tag in th
-00002a00: 6973 2073 6571 7565 6e63 6520 6966 2069  is sequence if i
-00002a10: 7420 6578 6973 7473 2901 da0b 7265 6d6f  t exists)...remo
-00002a20: 7665 5f74 6167 7372 9600 0000 4e72 9800  ve_tagsr....Nr..
-00002a30: 0000 729d 0000 0072 2700 0000 7227 0000  ..r....r'...r'..
-00002a40: 0072 2800 0000 72a2 0000 0094 0100 0072  .r(...r........r
-00002a50: 9e00 0000 7a13 4461 7461 7365 742e 7265  ....z.Dataset.re
-00002a60: 6d6f 7665 5f74 6167 7363 0100 0000 0000  move_tagsc......
-00002a70: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00002a80: 0000 730a 0000 0074 007c 006a 0183 0153  ..s....t.|.j...S
-00002a90: 0072 3a00 0000 2902 7209 0000 0072 2c00  .r:...).r....r,.
-00002aa0: 0000 7258 0000 0072 2700 0000 7227 0000  ..rX...r'...r'..
-00002ab0: 0072 2800 0000 da07 746f 5f64 6963 749f  .r(.....to_dict.
-00002ac0: 0100 0073 0200 0000 0a01 7a0f 4461 7461  ...s......z.Data
-00002ad0: 7365 742e 746f 5f64 6963 74da 0e64 6972  set.to_dict..dir
-00002ae0: 6563 746f 7279 5f70 6174 6863 0400 0000  ectory_pathc....
-00002af0: 0000 0000 0000 0000 0500 0000 0c00 0000  ................
-00002b00: 0300 0000 7346 0100 007c 01a0 00a1 0073  ....sF...|.....s
-00002b10: 0b74 017c 019b 0064 019d 0283 0182 0164  .t.|...d.......d
-00002b20: 0289 037c 0264 0275 0172 1774 026a 03a0  ...|.d.u.r.t.j..
-00002b30: 047c 02a1 0189 0364 0389 0464 0389 0564  .|.....d...d...d
-00002b40: 0474 056a 0664 0564 0266 0487 0087 0387  .t.j.d.d.f......
-00002b50: 0487 0566 0464 0664 0784 0c89 0088 007c  ...f.d.d.......|
-00002b60: 0183 0101 0088 0464 036b 0272 3974 07a0  .......d.k.r9t..
-00002b70: 0864 08a1 0101 0064 0253 0088 066a 0988  .d.....d.S...j..
-00002b80: 0464 098d 0189 0788 066a 0a74 0b6a 0c88  .d.......j.t.j..
-00002b90: 076a 0d64 0a8d 0289 0287 0687 0766 0264  .j.d.........f.d
-00002ba0: 0b64 0c84 087d 0464 0d74 056a 0664 0e74  .d...}.d.t.j.d.t
-00002bb0: 0e64 0574 0f6a 106a 1174 1274 056a 0674  .d.t.j.j.t.t.j.t
-00002bc0: 0e66 0219 0064 0264 0266 0319 0066 0687  .f...d.d.f...f..
-00002bd0: 0187 0287 0366 0364 0f64 1084 0c89 0188  .....f.d.d......
-00002be0: 066a 136a 1488 026a 1588 017c 0164 1183  .j.j...j...|.d..
-00002bf0: 027c 0474 166a 1788 066a 186a 1974 166a  .|.t.j...j.j.t.j
-00002c00: 1a88 066a 186a 1b74 166a 1c88 026a 1d74  ...j.j.t.j...j.t
-00002c10: 166a 1e88 076a 0d69 0474 1f64 1274 0e7c  .j...j.i.t.d.t.|
-00002c20: 01a0 20a1 0083 0188 0488 0564 139c 0364  .. ........d...d
-00002c30: 148d 0264 1564 168d 0601 0088 066a 2188  ...d.d.......j!.
-00002c40: 076a 0d7c 0364 178d 0201 0064 0253 0029  .j.|.d.....d.S.)
-00002c50: 1861 b502 0000 0a20 2020 2020 2020 2055  .a.....        U
-00002c60: 706c 6f61 6420 6576 6572 7974 6869 6e67  pload everything
-00002c70: 2c20 7265 6375 7273 6976 656c 792c 2069  , recursively, i
-00002c80: 6e20 6469 7265 6374 6f72 792c 2069 676e  n directory, ign
-00002c90: 6f72 696e 6720 6669 6c65 7320 7468 6174  oring files that
-00002ca0: 206d 6174 6368 2061 6e79 206f 6620 7468   match any of th
-00002cb0: 6520 6967 6e6f 7265 2070 6174 7465 726e  e ignore pattern
-00002cc0: 732e 0a0a 2020 2020 2020 2020 6065 7863  s...        `exc
-00002cd0: 6c75 6465 5f70 6174 7465 726e 7360 2069  lude_patterns` i
-00002ce0: 7320 6120 6c69 7374 206f 6620 6769 7469  s a list of giti
-00002cf0: 676e 6f72 652d 7374 796c 6520 7061 7474  gnore-style patt
-00002d00: 6572 6e73 2e0a 2020 2020 2020 2020 5365  erns..        Se
-00002d10: 6520 6874 7470 733a 2f2f 6769 742d 7363  e https://git-sc
-00002d20: 6d2e 636f 6d2f 646f 6373 2f67 6974 6967  m.com/docs/gitig
-00002d30: 6e6f 7265 235f 7061 7474 6572 6e5f 666f  nore#_pattern_fo
-00002d40: 726d 6174 2e0a 0a20 2020 2020 2020 2045  rmat...        E
-00002d50: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
-00002d60: 2020 2020 3e3e 3e20 6672 6f6d 2072 6f62      >>> from rob
-00002d70: 6f74 6f2e 646f 6d61 696e 2069 6d70 6f72  oto.domain impor
-00002d80: 7420 6461 7461 7365 7473 0a20 2020 2020  t datasets.     
-00002d90: 2020 2020 2020 203e 3e3e 2064 6174 6173         >>> datas
-00002da0: 6574 203d 2064 6174 6173 6574 732e 4461  et = datasets.Da
-00002db0: 7461 7365 7428 2e2e 2e29 0a20 2020 2020  taset(...).     
-00002dc0: 2020 2020 2020 203e 3e3e 2064 6174 6173         >>> datas
-00002dd0: 6574 2e75 706c 6f61 645f 6469 7265 6374  et.upload_direct
-00002de0: 6f72 7928 0a20 2020 2020 2020 2020 2020  ory(.           
-00002df0: 202e 2e2e 2020 2020 2070 6174 686c 6962   ...     pathlib
-00002e00: 2e50 6174 6828 222f 7061 7468 2f74 6f2f  .Path("/path/to/
-00002e10: 6469 7265 6374 6f72 7922 292c 0a20 2020  directory"),.   
-00002e20: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
-00002e30: 2065 7863 6c75 6465 5f70 6174 7465 726e   exclude_pattern
-00002e40: 733d 5b0a 2020 2020 2020 2020 2020 2020  s=[.            
-00002e50: 2e2e 2e20 2020 2020 2020 2020 225f 5f70  ...         "__p
-00002e60: 7963 6163 6865 5f5f 2f22 2c0a 2020 2020  ycache__/",.    
-00002e70: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00002e80: 2020 2020 222a 2e70 7963 222c 0a20 2020      "*.pyc",.   
-00002e90: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
-00002ea0: 2020 2020 2022 6e6f 6465 5f6d 6f64 756c       "node_modul
-00002eb0: 6573 2f22 2c0a 2020 2020 2020 2020 2020  es/",.          
-00002ec0: 2020 2e2e 2e20 2020 2020 2020 2020 222a    ...         "*
-00002ed0: 2a2f 2a2e 6c6f 6722 2c0a 2020 2020 2020  */*.log",.      
-00002ee0: 2020 2020 2020 2e2e 2e20 2020 2020 5d2c        ...     ],
-00002ef0: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00002f00: 2029 0a20 2020 2020 2020 207a 1320 6973   ).        z. is
-00002f10: 206e 6f74 2061 2064 6972 6563 746f 7279   not a directory
-00002f20: 4e72 0100 0000 72a4 0000 0072 3900 0000  Nr....r....r9...
-00002f30: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00002f40: 0004 0000 0013 0000 0073 4e00 0000 7c00  .........sN...|.
-00002f50: a000 a100 4400 5d20 7d01 7c01 a001 a100  ....D.] }.|.....
-00002f60: 720f 8800 7c01 8301 0100 7104 8801 6400  r...|.....q...d.
-00002f70: 7501 7219 8801 a002 7c01 a101 7219 7104  u.r.....|...r.q.
-00002f80: 8802 6401 3700 8902 8803 7c01 a003 a100  ..d.7.....|.....
-00002f90: 6a04 3700 8903 7104 6400 5300 2902 4e72  j.7...q.d.S.).Nr
-00002fa0: 1800 0000 2905 da07 6974 6572 6469 7272  ....)...iterdirr
-00002fb0: 8800 0000 da0a 6d61 7463 685f 6669 6c65  ......match_file
-00002fc0: da04 7374 6174 da07 7374 5f73 697a 6529  ..stat..st_size)
-00002fd0: 0272 a400 0000 da04 7061 7468 2904 da10  .r......path)...
-00002fe0: 5f63 6f75 6e74 5f72 6573 6f75 7263 6573  _count_resources
-00002ff0: da0c 6578 636c 7564 655f 7370 6563 da13  ..exclude_spec..
-00003000: 6578 7065 6374 6564 5f66 696c 655f 636f  expected_file_co
-00003010: 756e 74da 1265 7870 6563 7465 645f 6669  unt..expected_fi
-00003020: 6c65 5f73 697a 6572 2700 0000 7228 0000  le_sizer'...r(..
-00003030: 0072 aa00 0000 c701 0000 7310 0000 000c  .r........s.....
-00003040: 0308 010a 0112 0202 0108 0110 0104 f97a  ...............z
-00003050: 3244 6174 6173 6574 2e75 706c 6f61 645f  2Dataset.upload_
-00003060: 6469 7265 6374 6f72 792e 3c6c 6f63 616c  directory.<local
-00003070: 733e 2e5f 636f 756e 745f 7265 736f 7572  s>._count_resour
-00003080: 6365 737a 124e 6f20 6669 6c65 7320 746f  cesz.No files to
-00003090: 2075 706c 6f61 64a9 0172 ac00 0000 a901   upload..r......
-000030a0: 7221 0000 0063 0000 0000 0000 0000 0000  r!...c..........
-000030b0: 0000 0000 0000 0500 0000 1300 0000 7318  ..............s.
-000030c0: 0000 0088 006a 0074 016a 0264 0188 016a  .....j.t.j.d...j
-000030d0: 0364 028d 03a0 04a1 0053 0029 034e 5429  .d.......S.).NT)
-000030e0: 0272 9000 0000 7221 0000 0029 0572 7100  .r....r!...).rq.
-000030f0: 0000 7206 0000 0072 9100 0000 7221 0000  ..r....r....r!..
-00003100: 0072 7300 0000 7227 0000 0029 0272 5600  .rs...r'...).rV.
-00003110: 0000 da0b 7472 616e 7361 6374 696f 6e72  ....transactionr
-00003120: 2700 0000 7228 0000 0072 7400 0000 df01  '...r(...rt.....
-00003130: 0000 730e 0000 0004 0104 0102 0104 0104  ..s.............
-00003140: fd04 0402 fc7a 3644 6174 6173 6574 2e75  .....z6Dataset.u
-00003150: 706c 6f61 645f 6469 7265 6374 6f72 792e  pload_directory.
-00003160: 3c6c 6f63 616c 733e 2e5f 6372 6564 656e  <locals>._creden
-00003170: 7469 616c 5f70 726f 7669 6465 72da 0a69  tial_provider..i
-00003180: 6e6e 6572 5f70 6174 68da 0a6b 6579 5f70  nner_path..key_p
-00003190: 7265 6669 7863 0200 0000 0000 0000 0000  refixc..........
-000031a0: 0000 0400 0000 0700 0000 3300 0000 737a  ..........3...sz
-000031b0: 0000 0081 007c 00a0 00a1 0044 005d 357d  .....|.....D.]5}
-000031c0: 027c 02a0 01a1 0072 1a88 007c 027c 019b  .|.....r...|.|..
-000031d0: 0064 017c 026a 029b 009d 0383 0245 0064  .d.|.j.......E.d
-000031e0: 0048 0001 0071 0588 0264 0075 0172 2488  .H...q...d.u.r$.
-000031f0: 02a0 037c 02a1 0172 2471 057c 019b 0064  ...|...r$q.|...d
-00003200: 017c 026a 029b 009d 037d 037c 0288 016a  .|.j.....}.|...j
-00003210: 049b 0064 017c 03a0 0564 01a1 019b 009d  ...d.|...d......
-00003220: 0366 0256 0001 0071 0564 0053 0029 024e  .f.V...q.d.S.).N
-00003230: da01 2f29 0672 a500 0000 7288 0000 00da  ../).r....r.....
-00003240: 046e 616d 6572 a600 0000 da0f 7265 7175  .namer......requ
-00003250: 6972 6564 5f70 7265 6669 78da 066c 7374  ired_prefix..lst
-00003260: 7269 7029 0472 b100 0000 72b2 0000 0072  rip).r....r....r
-00003270: a900 0000 7220 0000 0029 03da 115f 7570  ....r ...)..._up
-00003280: 6c6f 6164 5f64 6972 6563 746f 7279 da0b  load_directory..
-00003290: 6372 6564 656e 7469 616c 7372 ab00 0000  credentialsr....
-000032a0: 7227 0000 0072 2800 0000 72b7 0000 00e6  r'...r(...r.....
-000032b0: 0100 0073 1200 0000 0280 0c03 0801 1e01  ...s............
-000032c0: 1202 0201 1002 1e01 04f8 7a33 4461 7461  ..........z3Data
-000032d0: 7365 742e 7570 6c6f 6164 5f64 6972 6563  set.upload_direc
-000032e0: 746f 7279 2e3c 6c6f 6361 6c73 3e2e 5f75  tory.<locals>._u
-000032f0: 706c 6f61 645f 6469 7265 6374 6f72 79da  pload_directory.
-00003300: 0072 1800 0000 2903 727c 0000 0072 ac00  .r....).r|...r..
-00003310: 0000 72ad 0000 0072 7d00 0000 7280 0000  ..r....r}...r...
-00003320: 0029 0672 1f00 0000 7281 0000 0072 8200  .).r....r....r..
-00003330: 0000 7237 0000 0072 8300 0000 7284 0000  ..r7...r....r...
-00003340: 0029 0172 5e00 0000 2922 7288 0000 0072  .).r^...)"r....r
-00003350: 4b00 0000 da08 7061 7468 7370 6563 da0d  K.....pathspec..
-00003360: 4769 7449 676e 6f72 6553 7065 63da 0a66  GitIgnoreSpec..f
-00003370: 726f 6d5f 6c69 6e65 7372 8b00 0000 728c  rom_linesr....r.
-00003380: 0000 00da 066c 6f67 6765 72da 0469 6e66  .....logger..inf
-00003390: 6fda 1b5f 4461 7461 7365 745f 5f73 7461  o.._Dataset__sta
-000033a0: 7274 5f74 7261 6e73 6163 7469 6f6e 7271  rt_transactionrq
-000033b0: 0000 0072 0600 0000 7291 0000 0072 2100  ...r....r....r!.
-000033c0: 0000 7225 0000 00da 0b63 6f6c 6c65 6374  ..r%.....collect
-000033d0: 696f 6e73 da03 6162 63da 0947 656e 6572  ions..abc..Gener
-000033e0: 6174 6f72 728a 0000 0072 2b00 0000 5a0c  atorr....r+...Z.
-000033f0: 7570 6c6f 6164 5f66 696c 6573 721f 0000  upload_filesr...
-00003400: 0072 1500 0000 da09 4461 7461 7365 7449  .r......DatasetI
-00003410: 6472 2c00 0000 723e 0000 00da 054f 7267  dr,...r>.....Org
-00003420: 4964 7234 0000 00da 0c43 6f6d 6d6f 6e50  Idr4.....CommonP
-00003430: 7265 6669 7872 b500 0000 da0d 5472 616e  refixr......Tran
-00003440: 7361 6374 696f 6e49 6472 1700 0000 da08  sactionIdr......
-00003450: 6162 736f 6c75 7465 7264 0000 0029 0572  absoluterd...).r
-00003460: 5600 0000 72a4 0000 0072 6900 0000 725e  V...r....ri...r^
-00003470: 0000 0072 7400 0000 7227 0000 0029 0872  ...rt...r'...).r
-00003480: aa00 0000 72b7 0000 0072 b800 0000 72ab  ....r....r....r.
-00003490: 0000 0072 ac00 0000 72ad 0000 0072 5600  ...r....r....rV.
-000034a0: 0000 72b0 0000 0072 2800 0000 da10 7570  ..r....r(.....up
-000034b0: 6c6f 6164 5f64 6972 6563 746f 7279 a201  load_directory..
-000034c0: 0000 735a 0000 0008 190e 0104 0208 0106  ..sZ............
-000034d0: 0102 0104 ff04 0404 011e 0208 0c08 020a  ................
-000034e0: 0104 010c 0204 0208 0106 ff0e 0402 0704  ................
-000034f0: 0102 ff02 0102 ff1a 0212 fe06 0d04 0108  ................
-00003500: 0102 010a 020a 0108 0108 0102 fc02 0602  ................
-00003510: 010a 0202 0102 0104 fd04 fe02 0806 ee14  ................
-00003520: 157a 1844 6174 6173 6574 2e75 706c 6f61  .z.Dataset.uploa
-00003530: 645f 6469 7265 6374 6f72 79da 0f6c 6f63  d_directory..loc
-00003540: 616c 5f66 696c 655f 7061 7468 7220 0000  al_file_pathr ..
-00003550: 0072 b800 0000 7282 0000 0063 0500 0000  .r....r....c....
-00003560: 0000 0000 0000 0000 0700 0000 0700 0000  ................
-00003570: 4300 0000 7330 0000 007c 006a 0064 0164  C...s0...|.j.d.d
-00003580: 028d 017d 057c 00a0 017c 017c 027c 056a  ...}.|...|.|.|.j
-00003590: 027c 037c 04a1 057d 067c 00a0 037c 056a  .|.|...}.|...|.j
-000035a0: 02a1 0101 007c 0653 0029 037a 4a0a 2020  .....|.S.).zJ.  
-000035b0: 2020 2020 2020 5570 6c6f 6164 7320 6120        Uploads a 
-000035c0: 7369 6e67 6c65 2066 696c 6520 746f 2074  single file to t
-000035d0: 6865 2064 6174 6173 6574 2773 2073 746f  he dataset's sto
-000035e0: 7261 6765 206c 6f63 6174 696f 6e2e 0a20  rage location.. 
-000035f0: 2020 2020 2020 2072 1800 0000 72ae 0000         r....r...
-00003600: 0029 0472 bf00 0000 da15 5f44 6174 6173  .).r......_Datas
-00003610: 6574 5f5f 7570 6c6f 6164 5f66 696c 6572  et__upload_filer
-00003620: 2100 0000 7264 0000 0029 0772 5600 0000  !...rd...).rV...
-00003630: 72c9 0000 0072 2000 0000 72b8 0000 0072  r....r ...r....r
-00003640: 8200 0000 72b0 0000 005a 0b75 706c 6f61  ....r....Z.uploa
-00003650: 645f 696e 666f 7227 0000 0072 2700 0000  d_infor'...r'...
-00003660: 7228 0000 00da 0b75 706c 6f61 645f 6669  r(.....upload_fi
-00003670: 6c65 0a02 0000 7314 0000 000c 0a04 0202  le....s.........
-00003680: 0102 0104 0102 0102 0104 fb0c 0804 027a  ...............z
-00003690: 1344 6174 6173 6574 2e75 706c 6f61 645f  .Dataset.upload_
-000036a0: 6669 6c65 7297 0000 00da 0a63 6f6e 6469  filer......condi
-000036b0: 7469 6f6e 7363 0500 0000 0000 0000 0000  tionsc..........
-000036c0: 0000 0600 0000 0700 0000 4300 0000 7322  ..........C...s"
-000036d0: 0000 007c 006a 006a 017c 006a 027c 017c  ...|.j.j.|.j.|.|
-000036e0: 027c 037c 0464 018d 057d 057c 057c 005f  .|.|.d...}.|.|._
-000036f0: 0264 0053 0029 024e 2904 7297 0000 0072  .d.S.).N).r....r
-00003700: cc00 0000 7238 0000 0072 9300 0000 2903  ....r8...r....).
-00003710: 722a 0000 0072 9900 0000 722c 0000 0029  r*...r....r,...)
-00003720: 0672 5600 0000 7297 0000 0072 cc00 0000  .rV...r....r....
-00003730: 7238 0000 0072 9300 0000 da07 7570 6461  r8...r......upda
-00003740: 7465 6472 2700 0000 7227 0000 0072 2800  tedr'...r'...r(.
-00003750: 0000 7299 0000 0022 0200 0073 1000 0000  ..r...."...s....
-00003760: 0607 0401 0201 0201 0201 0201 06fb 0a07  ................
-00003770: 7a0e 4461 7461 7365 742e 7570 6461 7465  z.Dataset.update
-00003780: 72ac 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00003790: 0000 0400 0000 0700 0000 4300 0000 7342  ..........C...sB
-000037a0: 0000 0074 006a 01a0 0264 01a1 017d 0274  ...t.j...d...}.t
-000037b0: 03a0 0474 056a 066a 0764 027c 029b 009d  ...t.j.j.d.|....
-000037c0: 02a1 027d 037c 006a 086a 0974 0a6a 0b7c  ...}.|.j.j.t.j.|
-000037d0: 037c 017c 006a 0c6a 0d7c 006a 0c6a 0d64  .|.|.j.j.|.j.j.d
-000037e0: 038d 0553 0029 044e da06 726f 626f 746f  ...S.).N..roboto
-000037f0: 7a07 726f 626f 746f 2029 055a 1074 7261  z.roboto ).Z.tra
-00003800: 6e73 6163 7469 6f6e 5f74 7970 65da 0b6f  nsaction_type..o
-00003810: 7269 6769 6e61 7469 6f6e 5a17 6578 7065  riginationZ.expe
-00003820: 6374 6564 5f72 6573 6f75 7263 655f 636f  cted_resource_co
-00003830: 756e 7472 3400 0000 da11 7265 736f 7572  untr4.....resour
-00003840: 6365 5f6f 776e 6572 5f69 6429 0eda 0969  ce_owner_id)...i
-00003850: 6d70 6f72 746c 6962 7236 0000 00da 0776  mportlibr6.....v
-00003860: 6572 7369 6f6e da02 6f73 da06 6765 7465  ersion..os..gete
-00003870: 6e76 7211 0000 00da 0952 6f62 6f74 6f45  nvr......RobotoE
-00003880: 6e76 da05 7661 6c75 6572 2e00 0000 5a11  nv..valuer....Z.
-00003890: 6265 6769 6e5f 7472 616e 7361 6374 696f  begin_transactio
-000038a0: 6e72 0c00 0000 5a0a 4669 6c65 5570 6c6f  nr....Z.FileUplo
-000038b0: 6164 722c 0000 0072 3400 0000 2904 7256  adr,...r4...).rV
-000038c0: 0000 0072 ac00 0000 5a0f 7061 636b 6167  ...r....Z.packag
-000038d0: 655f 7665 7273 696f 6e72 cf00 0000 7227  e_versionr....r'
-000038e0: 0000 0072 2700 0000 7228 0000 005a 135f  ...r'...r(...Z._
-000038f0: 5f73 7461 7274 5f74 7261 6e73 6163 7469  _start_transacti
-00003900: 6f6e 3202 0000 7316 0000 000c 0404 010e  on2...s.........
-00003910: 0104 ff06 0304 0102 0102 0106 0106 0106  ................
-00003920: fb7a 1b44 6174 6173 6574 2e5f 5f73 7461  .z.Dataset.__sta
-00003930: 7274 5f74 7261 6e73 6163 7469 6f6e 6306  rt_transactionc.
-00003940: 0000 0000 0000 0000 0000 0007 0000 000d  ................
-00003950: 0000 0003 0000 0073 d800 0000 7c01 a000  .......s....|...
-00003960: a100 730b 7401 7c01 9b00 6401 9d02 8301  ..s.t.|...d.....
-00003970: 8201 8800 6a02 6a03 7404 6a05 6b03 7319  ....j.j.t.j.k.s.
-00003980: 8800 6a02 6a06 7407 6a08 6b03 721d 7409  ..j.j.t.j.k.r.t.
-00003990: 6402 8301 8201 7c04 6403 7501 7223 7c04  d.....|.d.u.r#|.
-000039a0: 6e07 8800 6a0a 740b 6a0c 8801 6404 8d02  n...j.t.j...d...
-000039b0: 7d04 7c05 6403 7500 7238 8700 8701 6602  }.|.d.u.r8....f.
-000039c0: 6405 6406 8408 7d06 7c06 7d05 7c04 6a0d  d.d...}.|.}.|.j.
-000039d0: 9b00 6407 7c02 a00e 6407 a101 9b00 9d03  ..d.|...d.......
-000039e0: 7d02 8800 6a0f 6a10 7c01 7c04 6a11 7c02  }...j.j.|.|.j.|.
-000039f0: 7c05 7412 6a13 8800 6a02 6a14 7412 6a15  |.t.j...j.j.t.j.
-00003a00: 8800 6a02 6a16 7412 6a17 7c04 6a0d 7412  ..j.j.t.j.|.j.t.
-00003a10: 6a18 8801 6904 7419 6408 6409 8d01 640a  j...i.t.d.d...d.
-00003a20: 8d06 0100 741a 7c04 6a11 7c02 8801 640b  ....t.|.j.|...d.
-00003a30: 8d03 5300 290c 7a69 0a20 2020 2020 2020  ..S.).zi.       
-00003a40: 2055 706c 6f61 6473 2061 2066 696c 6520   Uploads a file 
-00003a50: 746f 2074 6865 2064 6174 6173 6574 2773  to the dataset's
-00003a60: 2073 746f 7261 6765 206c 6f63 6174 696f   storage locatio
-00003a70: 6e2e 2044 6f65 7320 6e6f 7420 6d61 726b  n. Does not mark
-00003a80: 2074 6865 2075 706c 6f61 6420 6173 2063   the upload as c
-00003a90: 6f6d 706c 6574 652e 0a20 2020 2020 2020  omplete..       
-00003aa0: 207a 0e20 6973 206e 6f74 2061 2066 696c   z. is not a fil
-00003ab0: 6572 6f00 0000 4e72 af00 0000 6300 0000  ero...Nr....c...
-00003ac0: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00003ad0: 0013 0000 0073 1400 0000 8800 6a00 7401  .....s......j.t.
-00003ae0: 6a02 8801 6401 8d02 a003 a100 5300 2902  j...d.......S.).
-00003af0: 4e72 af00 0000 2904 7271 0000 0072 0600  Nr....).rq...r..
-00003b00: 0000 7291 0000 0072 7300 0000 7227 0000  ..r....rs...r'..
-00003b10: 00a9 0272 5600 0000 7221 0000 0072 2700  ...rV...r!...r'.
-00003b20: 0000 7228 0000 0072 7400 0000 6202 0000  ..r(...rt...b...
-00003b30: 730a 0000 0004 0106 0104 ff04 0202 fe7a  s..............z
-00003b40: 3344 6174 6173 6574 2e5f 5f75 706c 6f61  3Dataset.__uploa
-00003b50: 645f 6669 6c65 2e3c 6c6f 6361 6c73 3e2e  d_file.<locals>.
-00003b60: 5f63 7265 6465 6e74 6961 6c5f 7072 6f76  _credential_prov
-00003b70: 6964 6572 72b3 0000 0072 1800 0000 2901  iderr....r....).
-00003b80: 727e 0000 0029 0272 3700 0000 7283 0000  r~...).r7...r...
-00003b90: 0029 0372 1f00 0000 7220 0000 0072 2100  .).r....r ...r!.
-00003ba0: 0000 291b da07 6973 5f66 696c 6572 4b00  ..)...is_filerK.
-00003bb0: 0000 722c 0000 0072 3300 0000 721b 0000  ..r,...r3...r...
-00003bc0: 0072 8500 0000 7232 0000 0072 1c00 0000  .r....r2...r....
-00003bd0: 7286 0000 0072 8700 0000 7271 0000 0072  r....r....rq...r
-00003be0: 0600 0000 7291 0000 0072 b500 0000 72b6  ....r....r....r.
-00003bf0: 0000 0072 2b00 0000 72cb 0000 0072 1f00  ...r+...r....r..
-00003c00: 0000 7215 0000 0072 c300 0000 723e 0000  ..r....r....r>..
-00003c10: 0072 c400 0000 7234 0000 0072 c500 0000  .r....r4...r....
-00003c20: 72c6 0000 0072 1700 0000 721e 0000 0029  r....r....r....)
-00003c30: 0772 5600 0000 72c9 0000 0072 2000 0000  .rV...r....r ...
-00003c40: 7221 0000 0072 b800 0000 7282 0000 0072  r!...r....r....r
-00003c50: 7400 0000 7227 0000 0072 d700 0000 7228  t...r'...r....r(
-00003c60: 0000 005a 0d5f 5f75 706c 6f61 645f 6669  ...Z.__upload_fi
-00003c70: 6c65 4202 0000 7344 0000 0008 0b0e 010e  leB...sD........
-00003c80: 030e 0102 0202 0104 ff08 0604 ff04 0206  ................
-00003c90: 0104 ff02 fd08 080e 0204 0516 0206 0102  ................
-00003ca0: 0104 0102 0102 010a 020a 0108 0106 0102  ................
-00003cb0: fc08 0606 f502 0e04 0102 0102 0106 fd7a  ...............z
-00003cc0: 1544 6174 6173 6574 2e5f 5f75 706c 6f61  .Dataset.__uploa
-00003cd0: 645f 6669 6c65 723a 0000 0029 024e 725c  d_filer:...).Nr\
-00003ce0: 0000 0029 0272 3900 0000 4e29 024e 4e29  ...).r9...N).NN)
-00003cf0: 044e 4e4e 4e29 4072 2200 0000 7223 0000  .NNNN)@r"...r#..
-00003d00: 0072 2400 0000 721a 0000 0072 2600 0000  .r$...r....r&...
-00003d10: 7213 0000 0072 1d00 0000 722d 0000 0072  r....r....r-...r
-00003d20: 0400 0000 7219 0000 0072 0a00 0000 da0b  ....r....r......
-00003d30: 636c 6173 736d 6574 686f 6472 1c00 0000  classmethodr....
-00003d40: 7286 0000 0072 1b00 0000 7285 0000 0072  r....r....r....r
-00003d50: 2500 0000 da04 6469 6374 7202 0000 0072  %.....dictr....r
-00003d60: 8d00 0000 723d 0000 0072 4000 0000 7208  ....r=...r@...r.
-00003d70: 0000 0072 c000 0000 72c1 0000 0072 c200  ...r....r....r..
-00003d80: 0000 7241 0000 0072 5700 0000 da08 7072  ..rA...rW.....pr
-00003d90: 6f70 6572 7479 723e 0000 0072 3600 0000  opertyr>...r6...
-00003da0: 723c 0000 0072 3700 0000 da03 696e 7472  r<...r7.....intr
-00003db0: 6400 0000 7267 0000 0072 6d00 0000 728b  d...rg...rm...r.
-00003dc0: 0000 0072 8c00 0000 728e 0000 0072 0600  ...r....r....r..
-00003dd0: 0000 7272 0000 00da 0462 6f6f 6c72 7100  ..rr.....boolrq.
-00003de0: 0000 7212 0000 0072 6a00 0000 729b 0000  ..r....rj...r...
-00003df0: 0072 0e00 0000 729c 0000 0072 9f00 0000  .r....r....r....
-00003e00: 72a1 0000 0072 a200 0000 72a3 0000 0072  r....r....r....r
-00003e10: c800 0000 7203 0000 0072 1600 0000 721e  ....r....r....r.
-00003e20: 0000 0072 cb00 0000 720d 0000 0072 0f00  ...r....r....r..
-00003e30: 0000 7299 0000 0072 0b00 0000 72bf 0000  ..r....r....r...
-00003e40: 0072 ca00 0000 7227 0000 0072 2700 0000  .r....r'...r'...
-00003e50: 7227 0000 0072 2800 0000 7229 0000 0035  r'...r(...r)...5
-00003e60: 0000 0073 d601 0000 0a00 0801 0801 0801  ...s............
-00003e70: 1001 0801 0202 0406 0401 0201 0201 0201  ................
-00003e80: 0201 0201 04f5 0202 02fe 0203 02fd 0204  ................
-00003e90: 02fc 0205 02fb 0206 02fa 0607 02f9 0608  ................
-00003ea0: 02f8 0e09 02f7 0a0a 02f6 060b 02f5 020c  ................
-00003eb0: 0cf4 0218 0207 04fa 0202 02fe 0203 02fd  ................
-00003ec0: 0204 02fc 0205 02fb 0606 02fa 0207 0cf9  ................
-00003ed0: 020b 0207 04fa 0202 02fe 0203 02fd 0204  ................
-00003ee0: 02fc 0205 02fb 0606 02fa 0a07 0cf9 0227  ...............'
-00003ef0: 0202 02fe 0203 02fd 0204 02fc 0205 02fb  ................
-00003f00: 0206 0afa 020c 1001 0203 1801 0203 1001  ................
-00003f10: 0203 1401 0206 0201 04fc 0202 02fe 0603  ................
-00003f20: 02fd 0204 02fc 0205 0afb 0a20 0205 0201  ........... ....
-00003f30: 04fd 0a02 02fe 0a03 02fd 0204 0afc 021a  ................
-00003f40: 0201 04fc 0402 02fe 0a03 02fd 0a04 02fc  ................
-00003f50: 0205 0afb 0441 0201 0201 0201 04fb 0202  .....A..........
-00003f60: 02fe 0603 02fd 0204 02fc 0605 02fb 0206  ................
-00003f70: 0afa 0214 0201 04fd 0a02 02fe 0a03 02fd  ................
-00003f80: 1004 0afc 022c 04fd 0a02 02fe 0603 02fd  .....,..........
-00003f90: 0204 0afc 021a 04fd 0202 02fe 0603 02fd  ................
-00003fa0: 0204 0afc 0a0b 0209 04fd 0202 02fe 0603  ................
-00003fb0: 02fd 0204 0afc 0216 04fd 0202 02fe 0603  ................
-00003fc0: 02fd 0204 0afc 160b 0206 0201 04fc 0402  ................
-00003fd0: 02fe 0a03 02fd 0204 02fc 0205 0afb 026c  ...............l
-00003fe0: 0201 04fb 0402 02fe 0203 02fd 0604 02fc  ................
-00003ff0: 0e05 02fb 0206 0afa 021a 0201 0201 0201  ................
-00004000: 04fb 0602 02fe 0a03 02fd 0604 02fc 0605  ................
-00004010: 02fb 0206 0afa 0210 0202 02fe 0203 0afd  ................
-00004020: 0215 0201 04fa 0402 02fe 0203 02fd 0204  ................
-00004030: 02fc 0605 02fb 0e06 02fa 0207 0ef9 7229  ..............r)
-00004040: 0000 0029 32da 0f63 6f6c 6c65 6374 696f  ...)2..collectio
-00004050: 6e73 2e61 6263 72c0 0000 00da 0b64 6174  ns.abcr......dat
-00004060: 6163 6c61 7373 6573 da12 696d 706f 7274  aclasses..import
-00004070: 6c69 622e 6d65 7461 6461 7461 72d1 0000  lib.metadatar...
-00004080: 0072 d300 0000 728b 0000 0072 6000 0000  .r....r....r`...
-00004090: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-000040a0: 0000 7204 0000 0072 ba00 0000 da04 6175  ..r....r......au
-000040b0: 7468 7206 0000 00da 076c 6f67 6769 6e67  thr......logging
-000040c0: 7207 0000 0072 4100 0000 7208 0000 00da  r....rA...r.....
-000040d0: 0573 6572 6465 7209 0000 00da 0c74 7261  .serder......tra
-000040e0: 6e73 6163 7469 6f6e 7372 0a00 0000 720b  nsactionsr....r.
-000040f0: 0000 0072 0c00 0000 da07 7570 6461 7465  ...r......update
-00004100: 7372 0d00 0000 720e 0000 0072 0f00 0000  sr....r....r....
-00004110: da07 6163 7469 6f6e 7372 1100 0000 da05  ..actionsr......
-00004120: 6669 6c65 7372 1200 0000 7213 0000 0072  filesr....r....r
-00004130: 1400 0000 7215 0000 0072 1600 0000 5a0e  ....r....r....Z.
-00004140: 6669 6c65 732e 7072 6f67 7265 7373 7217  files.progressr.
-00004150: 0000 00da 0864 656c 6567 6174 6572 1900  .....delegater..
-00004160: 0000 721a 0000 0072 1b00 0000 723c 0000  ..r....r....r<..
-00004170: 0072 1c00 0000 721d 0000 0072 bd00 0000  .r....r....r....
-00004180: da09 6461 7461 636c 6173 7372 1e00 0000  ..dataclassr....
-00004190: 7229 0000 0072 2700 0000 7227 0000 0072  r)...r'...r'...r
-000041a0: 2700 0000 7228 0000 00da 083c 6d6f 6475  '...r(.....<modu
-000041b0: 6c65 3e01 0000 0073 2e00 0000 0800 0801  le>....s........
-000041c0: 0801 0801 0801 0801 1401 0802 0c02 0c01  ................
-000041d0: 0c01 0c01 1401 1405 0c05 1c01 0c07 1403  ................
-000041e0: 1005 0602 0403 1001 1206                 ..........
+00000060: 6401 6c08 5a08 6400 6401 6c09 5a09 6402  d.l.Z.d.d.l.Z.d.
+00000070: 6403 6c0a 6d0b 5a0b 0100 6402 6404 6c0c  d.l.m.Z...d.d.l.
+00000080: 6d0d 5a0d 6d0e 5a0e 0100 6402 6405 6c0f  m.Z.m.Z...d.d.l.
+00000090: 6d10 5a10 0100 6402 6406 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
+000000a0: 0100 6402 6407 6c13 6d14 5a14 0100 6402  ..d.d.l.m.Z...d.
+000000b0: 6408 6c15 6d16 5a16 6d17 5a17 6d18 5a18  d.l.m.Z.m.Z.m.Z.
+000000c0: 0100 6402 6409 6c19 6d1a 5a1a 6d1b 5a1b  ..d.d.l.m.Z.m.Z.
+000000d0: 6d1c 5a1c 0100 640a 640b 6c1d 6d1e 5a1e  m.Z...d.d.l.m.Z.
+000000e0: 0100 640a 640c 6c1f 6d20 5a20 6d21 5a21  ..d.d.l.m Z m!Z!
+000000f0: 6d22 5a22 6d23 5a23 6d24 5a24 0100 640a  m"Z"m#Z#m$Z$..d.
+00000100: 640d 6c25 6d26 5a26 0100 640e 640f 6c27  d.l%m&Z&..d.d.l'
+00000110: 6d28 5a28 6d29 5a29 6d2a 5a2a 0100 640e  m(Z(m)Z)m*Z*..d.
+00000120: 6410 6c2b 6d2c 5a2c 6d2d 5a2d 0100 6510  d.l+m,Z,m-Z-..e.
+00000130: 8300 5a2e 6502 6a2f 4700 6411 6412 8400  ..Z.e.j/G.d.d...
+00000140: 6412 8302 8301 5a30 4700 6413 6414 8400  d.....Z0G.d.d...
+00000150: 6414 8302 5a31 6401 5300 2915 e900 0000  d...Z1d.S.).....
+00000160: 004e e903 0000 0029 01da 0b50 6572 6d69  .N.....)...Permi
+00000170: 7373 696f 6e73 2902 da1d 526f 626f 746f  ssions)...Roboto
+00000180: 496e 7661 6c69 6452 6571 7565 7374 4578  InvalidRequestEx
+00000190: 6365 7074 696f 6eda 1752 6f62 6f74 6f4e  ception..RobotoN
+000001a0: 6f74 466f 756e 6445 7863 6570 7469 6f6e  otFoundException
+000001b0: 2901 da0e 6465 6661 756c 745f 6c6f 6767  )...default_logg
+000001c0: 6572 2901 da12 5175 6572 7953 7065 6369  er)...QuerySpeci
+000001d0: 6669 6361 7469 6f6e 2901 da16 7079 6461  fication)...pyda
+000001e0: 6e74 6963 5f6a 736f 6e61 626c 655f 6469  ntic_jsonable_di
+000001f0: 6374 2903 da15 5472 616e 7361 6374 696f  ct)...Transactio
+00000200: 6e4d 616e 6167 6572 4142 43da 1154 7261  nManagerABC..Tra
+00000210: 6e73 6163 7469 6f6e 5265 636f 7264 da0f  nsactionRecord..
+00000220: 5472 616e 7361 6374 696f 6e54 7970 6529  TransactionType)
+00000230: 03da 114d 6574 6164 6174 6143 6861 6e67  ...MetadataChang
+00000240: 6573 6574 da0b 5374 7253 6571 7565 6e63  eset..StrSequenc
+00000250: 65da 0f55 7064 6174 6543 6f6e 6469 7469  e..UpdateConditi
+00000260: 6f6e e902 0000 0029 01da 1049 6e76 6f63  on.....)...Invoc
+00000270: 6174 696f 6e45 6e76 5661 7229 05da 0446  ationEnvVar)...F
+00000280: 696c 65da 0c46 696c 6544 656c 6567 6174  ile..FileDelegat
+00000290: 65da 0a46 696c 6552 6563 6f72 64da 0746  e..FileRecord..F
+000002a0: 696c 6554 6167 da0d 5333 4372 6564 656e  ileTag..S3Creden
+000002b0: 7469 616c 7329 01da 1a54 7164 6d50 726f  tials)...TqdmPro
+000002c0: 6772 6573 734d 6f6e 6974 6f72 4661 6374  gressMonitorFact
+000002d0: 6f72 79e9 0100 0000 2903 da0b 4372 6564  ory.....)...Cred
+000002e0: 656e 7469 616c 73da 0f44 6174 6173 6574  entials..Dataset
+000002f0: 4465 6c65 6761 7465 da0f 5374 6f72 6167  Delegate..Storag
+00000300: 654c 6f63 6174 696f 6e29 02da 0d41 646d  eLocation)...Adm
+00000310: 696e 6973 7472 6174 6f72 da0d 4461 7461  inistrator..Data
+00000320: 7365 7452 6563 6f72 6463 0000 0000 0000  setRecordc......
+00000330: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000340: 0000 7326 0000 0065 005a 0164 005a 0255  ..s&...e.Z.d.Z.U
+00000350: 0065 0365 0464 013c 0065 0365 0464 023c  .e.e.d.<.e.e.d.<
+00000360: 0065 0365 0464 033c 0064 0453 0029 05da  .e.e.d.<.d.S.)..
+00000370: 0e46 696c 6555 706c 6f61 6449 6e66 6fda  .FileUploadInfo.
+00000380: 0662 7563 6b65 74da 036b 6579 da0e 7472  .bucket..key..tr
+00000390: 616e 7361 6374 696f 6e5f 6964 4e29 05da  ansaction_idN)..
+000003a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000003b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000003c0: 655f 5fda 0373 7472 da0f 5f5f 616e 6e6f  e__..str..__anno
+000003d0: 7461 7469 6f6e 735f 5fa9 0072 2600 0000  tations__..r&...
+000003e0: 7226 0000 00fa e72f 636f 6465 6275 696c  r&...../codebuil
+000003f0: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+00000400: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
+00000410: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
+00000420: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
+00000430: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
+00000440: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
+00000450: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
+00000460: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
+00000470: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
+00000480: 6f74 6f2d 6169 2f72 6f62 6f74 6f2d 686f  oto-ai/roboto-ho
+00000490: 7374 6564 2d61 7070 2f70 6163 6b61 6765  sted-app/package
+000004a0: 732f 726f 626f 746f 2f73 7263 2f72 6f62  s/roboto/src/rob
+000004b0: 6f74 6f2f 646f 6d61 696e 2f64 6174 6173  oto/domain/datas
+000004c0: 6574 732f 6461 7461 7365 742e 7079 721d  ets/dataset.pyr.
+000004d0: 0000 0032 0000 0073 0800 0000 0a00 0802  ...2...s........
+000004e0: 0801 0c01 721d 0000 0063 0000 0000 0000  ....r....c......
+000004f0: 0000 0000 0000 0000 0000 1800 0000 4000  ..............@.
+00000500: 0000 735a 0400 0065 005a 0164 005a 0255  ..sZ...e.Z.d.Z.U
+00000510: 0065 0365 0464 013c 0065 0565 0464 023c  .e.e.d.<.e.e.d.<
+00000520: 0065 0665 0464 033c 0064 045a 0765 086a  .e.e.d.<.d.Z.e.j
+00000530: 0965 0a19 0065 0464 053c 0065 0b65 0464  .e...e.d.<.e.e.d
+00000540: 063c 0065 0c65 0d6a 0e65 0f6a 1064 0464  .<.e.e.j.e.j.d.d
+00000550: 0464 0464 0464 0466 0764 0765 0364 0865  .d.d.d.f.d.e.d.e
+00000560: 0564 0965 0b64 0a65 0d64 0b65 0f64 0c65  .d.e.d.e.d.e.d.e
+00000570: 086a 0965 1119 0064 0d65 086a 0965 1119  .j.e...d.e.j.e..
+00000580: 0064 0e65 086a 0965 1265 1165 086a 1366  .d.e.j.e.e.e.j.f
+00000590: 0219 0019 0064 0f65 086a 0965 1465 1119  .....d.e.j.e.e..
+000005a0: 0019 0064 1065 086a 0965 1119 0064 1164  ...d.e.j.e...d.d
+000005b0: 0066 1664 1264 1384 0583 015a 1565 0c64  .f.d.d.....Z.e.d
+000005c0: 1465 1164 0765 0364 0865 0564 0965 0b64  .e.d.e.d.e.d.e.d
+000005d0: 1164 0066 0a64 1564 1684 0483 015a 1665  .d.f.d.d.....Z.e
+000005e0: 0c09 0464 5e64 1765 1764 0765 0364 0865  ...d^d.e.d.e.d.e
+000005f0: 0564 0965 0b64 0c65 086a 0965 1119 0064  .d.e.d.e.j.e...d
+00000600: 1165 186a 196a 1a64 1819 0066 0c64 1964  .e.j.j.d...f.d.d
+00000610: 1a84 0583 015a 1b64 1b65 0664 0765 0364  .....Z.d.e.d.e.d
+00000620: 0865 0564 0965 0b64 1164 0466 0a64 1c64  .e.d.e.d.d.f.d.d
+00000630: 1d84 045a 1c65 1d64 1165 1166 0264 1e64  ...Z.e.d.e.f.d.d
+00000640: 1f84 0483 015a 1e65 1d64 1165 1265 1165  .....Z.e.d.e.e.e
+00000650: 086a 1366 0219 0066 0264 2064 2184 0483  .j.f...f.d d!...
+00000660: 015a 1f65 1d64 1165 0666 0264 2264 2384  .Z.e.d.e.f.d"d#.
+00000670: 0483 015a 2065 1d64 1165 1465 1119 0066  ...Z e.d.e.e...f
+00000680: 0264 2464 2584 0483 015a 2109 0409 2664  .d$d%....Z!...&d
+00000690: 5f64 2765 1164 2865 086a 0965 1119 0064  _d'e.d(e.j.e...d
+000006a0: 2965 2264 1164 0466 0864 2a64 2b84 055a  )e"d.d.f.d*d+..Z
+000006b0: 2364 6064 2c64 2d84 045a 2409 0409 0464  #d`d,d-..Z$....d
+000006c0: 6164 2e65 086a 0965 1465 1119 0019 0064  ad.e.j.e.e.....d
+000006d0: 2f65 086a 0965 1465 1119 0019 0064 1164  /e.j.e.e.....d.d
+000006e0: 0466 0664 3064 3184 055a 2509 0409 0464  .f.d0d1..Z%....d
+000006f0: 6164 3265 266a 2764 2e65 086a 0965 1465  ad2e&j'd.e.j.e.e
+00000700: 1119 0019 0064 2f65 086a 0965 1465 1119  .....d/e.j.e.e..
+00000710: 0019 0064 1164 0466 0864 3364 3484 055a  ...d.d.f.d3d4..Z
+00000720: 2864 3565 086a 2965 1165 266a 2766 0219  (d5e.j)e.e&j'f..
+00000730: 0064 1165 2a66 0464 3664 3784 045a 2b65  .d.e*f.d6d7..Z+e
+00000740: 2c6a 2d64 0464 3864 0466 0464 3965 2c64  ,j-d.d8d.f.d9e,d
+00000750: 2865 086a 0965 1119 0064 3a65 2e64 2765  (e.j.e...d:e.d'e
+00000760: 086a 0965 1119 0064 1165 0a66 0a64 3b64  .j.e...d.e.f.d;d
+00000770: 3c84 055a 2f09 0409 0464 6164 2e65 086a  <..Z/....dad.e.j
+00000780: 0965 1465 1119 0019 0064 2f65 086a 0965  .e.e.....d/e.j.e
+00000790: 1465 1119 0019 0064 1165 186a 196a 1a65  .e.....d.e.j.j.e
+000007a0: 2a64 0464 0466 0319 0066 0664 3d64 3e84  *d.d.f...f.d=d>.
+000007b0: 055a 3009 0464 5e64 0e65 1265 1165 086a  .Z0..d^d.e.e.e.j
+000007c0: 1366 0219 0064 3f65 086a 0965 1119 0064  .f...d?e.j.e...d
+000007d0: 1164 0466 0664 4064 4184 055a 3109 0464  .d.f.d@dA..Z1..d
+000007e0: 5e64 0f65 3264 3f65 086a 0965 1119 0064  ^d.e2d?e.j.e...d
+000007f0: 1164 0466 0664 4264 4384 055a 3364 6064  .d.f.dBdC..Z3d`d
+00000800: 4464 4584 045a 3409 0464 5e64 0e65 3264  DdE..Z4..d^d.e2d
+00000810: 3f65 086a 0965 1119 0064 1164 0466 0664  ?e.j.e...d.d.f.d
+00000820: 4664 4784 055a 3509 0464 5e64 0f65 3264  FdG..Z5..d^d.e2d
+00000830: 3f65 086a 0965 1119 0064 1164 0466 0664  ?e.j.e...d.d.f.d
+00000840: 4864 4984 055a 3664 1165 1265 1165 086a  HdI..Z6d.e.e.e.j
+00000850: 1366 0219 0066 0264 4a64 4b84 045a 3709  .f...f.dJdK..Z7.
+00000860: 0409 2664 5f64 4c65 266a 2764 2f65 086a  ..&d_dLe&j'd/e.j
+00000870: 0965 1465 1119 0019 0064 2965 2264 1164  .e.e.....d)e"d.d
+00000880: 0466 0864 4d64 4e84 055a 3809 0409 0464  .f.dMdN..Z8....d
+00000890: 6164 4f65 266a 2764 5065 1164 5165 086a  adOe&j'dPe.dQe.j
+000008a0: 0965 0a19 0064 5265 086a 0965 086a 3967  .e...dRe.j.e.j9g
+000008b0: 0065 3a66 0219 0019 0064 1165 3b66 0a64  .e:f.....d.e;f.d
+000008c0: 5364 5484 055a 3c09 0409 0409 0409 0464  SdT..Z<........d
+000008d0: 6264 5565 086a 0965 3d19 0064 5665 086a  bdUe.j.e=..dVe.j
+000008e0: 0965 1465 3e19 0019 0064 1065 086a 0965  .e.e>....d.e.j.e
+000008f0: 1119 0064 3f65 086a 0965 1119 0064 1164  ...d?e.j.e...d.d
+00000900: 0466 0a64 5764 5884 055a 3f64 5965 2264  .f.dWdX..Z?dYe"d
+00000910: 1165 4066 0464 5a64 5b84 045a 4109 0409  .e@f.dZd[..ZA...
+00000920: 0464 6164 4f65 266a 2764 5065 1164 2765  .dadOe&j'dPe.d'e
+00000930: 1164 5165 086a 0965 0a19 0064 5265 086a  .dQe.j.e...dRe.j
+00000940: 0965 086a 3967 0065 3a66 0219 0019 0064  .e.j9g.e:f.....d
+00000950: 1165 3b66 0c64 5c64 5d84 055a 4264 0453  .e;f.d\d]..ZBd.S
+00000960: 0029 63da 0744 6174 6173 6574 da1a 5f44  .)c..Dataset.._D
+00000970: 6174 6173 6574 5f5f 6461 7461 7365 745f  ataset__dataset_
+00000980: 6465 6c65 6761 7465 da17 5f44 6174 6173  delegate.._Datas
+00000990: 6574 5f5f 6669 6c65 5f64 656c 6567 6174  et__file_delegat
+000009a0: 65da 105f 4461 7461 7365 745f 5f72 6563  e.._Dataset__rec
+000009b0: 6f72 644e da1a 5f44 6174 6173 6574 5f5f  ordN.._Dataset__
+000009c0: 7465 6d70 5f63 7265 6465 6e74 6961 6c73  temp_credentials
+000009d0: da1d 5f44 6174 6173 6574 5f5f 7472 616e  .._Dataset__tran
+000009e0: 7361 6374 696f 6e5f 6d61 6e61 6765 72da  saction_manager.
+000009f0: 1064 6174 6173 6574 5f64 656c 6567 6174  .dataset_delegat
+00000a00: 65da 0d66 696c 655f 6465 6c65 6761 7465  e..file_delegate
+00000a10: da13 7472 616e 7361 6374 696f 6e5f 6d61  ..transaction_ma
+00000a20: 6e61 6765 72da 0d61 646d 696e 6973 7472  nager..administr
+00000a30: 6174 6f72 da10 7374 6f72 6167 655f 6c6f  ator..storage_lo
+00000a40: 6361 7469 6f6e da06 6f72 675f 6964 da0a  cation..org_id..
+00000a50: 6372 6561 7465 645f 6279 da08 6d65 7461  created_by..meta
+00000a60: 6461 7461 da04 7461 6773 da0b 6465 7363  data..tags..desc
+00000a70: 7269 7074 696f 6eda 0672 6574 7572 6e63  ription..returnc
+00000a80: 0b00 0000 0000 0000 0000 0000 0c00 0000  ................
+00000a90: 0900 0000 4300 0000 7324 0000 007c 01a0  ....C...s$...|..
+00000aa0: 007c 047c 087c 057c 097c 067c 077c 0aa1  .|.|.|.|.|.|.|..
+00000ab0: 077d 0b7c 007c 0b7c 017c 027c 0383 0453  .}.|.|.|.|.|...S
+00000ac0: 00a9 014e 2901 5a0e 6372 6561 7465 5f64  ...N).Z.create_d
+00000ad0: 6174 6173 6574 290c da03 636c 7372 2e00  ataset)...clsr..
+00000ae0: 0000 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
+00000af0: 0072 3200 0000 7233 0000 0072 3400 0000  .r2...r3...r4...
+00000b00: 7235 0000 0072 3600 0000 7237 0000 00da  r5...r6...r7....
+00000b10: 0672 6563 6f72 6472 2600 0000 7226 0000  .recordr&...r&..
+00000b20: 0072 2700 0000 da06 6372 6561 7465 4000  .r'.....create@.
+00000b30: 0000 7314 0000 0004 0e02 0102 0102 0102  ..s.............
+00000b40: 0102 0102 0102 0104 f90e 097a 0e44 6174  ...........z.Dat
+00000b50: 6173 6574 2e63 7265 6174 65da 0a64 6174  aset.create..dat
+00000b60: 6173 6574 5f69 6463 0500 0000 0000 0000  aset_idc........
+00000b70: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
+00000b80: 7318 0000 007c 02a0 007c 01a1 017d 057c  s....|...|...}.|
+00000b90: 007c 057c 027c 037c 0483 0453 0072 3900  .|.|.|.|...S.r9.
+00000ba0: 0000 2901 da11 6765 745f 6461 7461 7365  ..)...get_datase
+00000bb0: 745f 6279 5f69 6429 0672 3a00 0000 723d  t_by_id).r:...r=
+00000bc0: 0000 0072 2e00 0000 722f 0000 0072 3000  ...r....r/...r0.
+00000bd0: 0000 723b 0000 0072 2600 0000 7226 0000  ..r;...r&...r&..
+00000be0: 0072 2700 0000 da07 6672 6f6d 5f69 6459  .r'.....from_idY
+00000bf0: 0000 0073 0400 0000 0a08 0e01 7a0f 4461  ...s........z.Da
+00000c00: 7461 7365 742e 6672 6f6d 5f69 64da 0571  taset.from_id..q
+00000c10: 7565 7279 2903 7228 0000 004e 4e63 0600  uery).r(...NNc..
+00000c20: 0000 0000 0000 0000 0000 0e00 0000 0600  ................
+00000c30: 0000 6300 0000 73d8 0000 0081 0074 0074  ..c...s......t.t
+00000c40: 016a 02a0 03a1 0083 017d 0674 0083 007d  .j.......}.t...}
+00000c50: 077c 01a0 04a1 0044 005d 167d 0864 017c  .|.....D.].}.d.|
+00000c60: 0876 0072 207c 07a0 057c 08a0 0664 01a1  .v.r |...|...d..
+00000c70: 0164 0219 00a1 0101 0071 0f7c 07a0 057c  .d.......q.|...|
+00000c80: 08a1 0101 0071 0f7c 077c 0618 007d 097c  .....q.|.|...}.|
+00000c90: 0972 4474 077c 0983 0164 036b 047d 0a7c  .rDt.|...d.k.}.|
+00000ca0: 0a72 3664 046e 0164 057d 0b74 087c 099b  .r6d.n.d.}.t.|..
+00000cb0: 0064 067c 0b9b 0064 077c 069b 009d 0583  .d.|...d.|......
+00000cc0: 0182 017c 026a 097c 017c 0564 088d 027d  ...|.j.|.|.d...}
+00000cd0: 0c09 007c 0c6a 0a44 005d 0a7d 0d7c 007c  ...|.j.D.].}.|.|
+00000ce0: 0d7c 027c 037c 0483 0456 0001 0071 4f7c  .|.|.|...V...qO|
+00000cf0: 0c6a 0b72 697c 0c6a 0b7c 015f 0c7c 026a  .j.ri|.j.|._.|.j
+00000d00: 097c 017c 0564 088d 027d 0c6e 0264 0053  .|.|.d...}.n.d.S
+00000d10: 0071 4c29 094e da01 2e72 0100 0000 7217  .qL).N...r....r.
+00000d20: 0000 007a 2361 7265 206e 6f74 206b 6e6f  ...z#are not kno
+00000d30: 776e 2061 7474 7269 6275 7465 7320 6f66  wn attributes of
+00000d40: 2044 6174 6173 6574 7a23 6973 206e 6f74   Datasetz#is not
+00000d50: 2061 206b 6e6f 776e 2061 7474 7269 6275   a known attribu
+00000d60: 7465 206f 6620 4461 7461 7365 74da 0120  te of Dataset.. 
+00000d70: 7a14 2e20 4b6e 6f77 6e20 6174 7472 6962  z.. Known attrib
+00000d80: 7574 6573 3a20 2901 7233 0000 0029 0dda  utes: ).r3...)..
+00000d90: 0373 6574 721c 0000 00da 0c6d 6f64 656c  .setr......model
+00000da0: 5f66 6965 6c64 73da 046b 6579 73da 0666  _fields..keys..f
+00000db0: 6965 6c64 73da 0361 6464 da05 7370 6c69  ields..add..spli
+00000dc0: 74da 036c 656e da0a 5661 6c75 6545 7272  t..len..ValueErr
+00000dd0: 6f72 5a0e 7175 6572 795f 6461 7461 7365  orZ.query_datase
+00000de0: 7473 da05 6974 656d 73da 0a6e 6578 745f  ts..items..next_
+00000df0: 746f 6b65 6eda 0561 6674 6572 290e 723a  token..after).r:
+00000e00: 0000 0072 4000 0000 722e 0000 0072 2f00  ...r@...r....r/.
+00000e10: 0000 7230 0000 0072 3300 0000 da05 6b6e  ..r0...r3.....kn
+00000e20: 6f77 6eda 0661 6374 7561 6cda 0566 6965  own..actual..fie
+00000e30: 6c64 da07 756e 6b6e 6f77 6eda 0670 6c75  ld..unknown..plu
+00000e40: 7261 6cda 036d 7367 da11 7061 6769 6e61  ral..msg..pagina
+00000e50: 7465 645f 7265 7375 6c74 7372 3b00 0000  ted_resultsr;...
+00000e60: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
+00000e70: 4000 0000 6400 0000 7334 0000 0002 800e  @...d...s4......
+00000e80: 0906 010c 0108 0316 010c 0208 0104 010c  ................
+00000e90: 0102 0306 ff02 0202 fd18 050e 0202 010a  ................
+00000ea0: 0112 0106 0108 0104 0104 0108 ff04 0402  ................
+00000eb0: f77a 0d44 6174 6173 6574 2e71 7565 7279  .z.Dataset.query
+00000ec0: 723b 0000 0063 0500 0000 0000 0000 0000  r;...c..........
+00000ed0: 0000 0500 0000 0200 0000 4300 0000 731c  ..........C...s.
+00000ee0: 0000 007c 027c 005f 007c 037c 005f 017c  ...|.|._.|.|._.|
+00000ef0: 017c 005f 027c 047c 005f 0364 0053 0072  .|._.|.|._.d.S.r
+00000f00: 3900 0000 2904 7229 0000 0072 2a00 0000  9...).r)...r*...
+00000f10: 722b 0000 0072 2d00 0000 2905 da04 7365  r+...r-...)...se
+00000f20: 6c66 723b 0000 0072 2e00 0000 722f 0000  lfr;...r....r/..
+00000f30: 0072 3000 0000 7226 0000 0072 2600 0000  .r0...r&...r&...
+00000f40: 7227 0000 00da 085f 5f69 6e69 745f 5f8c  r'.....__init__.
+00000f50: 0000 0073 0800 0000 0607 0601 0601 0a01  ...s............
+00000f60: 7a10 4461 7461 7365 742e 5f5f 696e 6974  z.Dataset.__init
+00000f70: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+00000f80: 0000 0001 0000 0043 0000 0073 0800 0000  .......C...s....
+00000f90: 7c00 6a00 6a01 5300 7239 0000 0029 0272  |.j.j.S.r9...).r
+00000fa0: 2b00 0000 723d 0000 00a9 0172 5500 0000  +...r=.....rU...
+00000fb0: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
+00000fc0: 3d00 0000 9800 0000 7302 0000 0008 027a  =.......s......z
+00000fd0: 1244 6174 6173 6574 2e64 6174 6173 6574  .Dataset.dataset
+00000fe0: 5f69 6463 0100 0000 0000 0000 0000 0000  _idc............
+00000ff0: 0100 0000 0200 0000 4300 0000 f30c 0000  ........C.......
+00001000: 007c 006a 006a 01a0 02a1 0053 0072 3900  .|.j.j.....S.r9.
+00001010: 0000 2903 722b 0000 0072 3500 0000 da04  ..).r+...r5.....
+00001020: 636f 7079 7257 0000 0072 2600 0000 7226  copyrW...r&...r&
+00001030: 0000 0072 2700 0000 7235 0000 009c 0000  ...r'...r5......
+00001040: 00f3 0200 0000 0c02 7a10 4461 7461 7365  ........z.Datase
+00001050: 742e 6d65 7461 6461 7461 6301 0000 0000  t.metadatac.....
+00001060: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00001070: 0000 0073 0600 0000 7c00 6a00 5300 7239  ...s....|.j.S.r9
+00001080: 0000 0029 0172 2b00 0000 7257 0000 0072  ...).r+...rW...r
+00001090: 2600 0000 7226 0000 0072 2700 0000 723b  &...r&...r'...r;
+000010a0: 0000 00a0 0000 0073 0200 0000 0602 7a0e  .......s......z.
+000010b0: 4461 7461 7365 742e 7265 636f 7264 6301  Dataset.recordc.
+000010c0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+000010d0: 0000 0043 0000 0072 5800 0000 7239 0000  ...C...rX...r9..
+000010e0: 0029 0372 2b00 0000 7236 0000 0072 5900  .).r+...r6...rY.
+000010f0: 0000 7257 0000 0072 2600 0000 7226 0000  ..rW...r&...r&..
+00001100: 0072 2700 0000 7236 0000 00a4 0000 0072  .r'...r6.......r
+00001110: 5a00 0000 7a0c 4461 7461 7365 742e 7461  Z...z.Dataset.ta
+00001120: 6773 e92c 0100 0072 2000 0000 da06 6361  gs.,...r .....ca
+00001130: 6c6c 6572 da07 7469 6d65 6f75 7463 0400  ller..timeoutc..
+00001140: 0000 0000 0000 0000 0000 0600 0000 0500  ................
+00001150: 0000 4300 0000 7380 0000 0074 00a0 00a1  ..C...s....t....
+00001160: 007d 0464 017d 057c 006a 01a0 027c 017c  .}.d.}.|.j...|.|
+00001170: 006a 036a 04a1 0273 3474 00a0 00a1 007c  .j.j...s4t.....|
+00001180: 0418 007c 036b 0472 1b74 0564 0283 0182  ...|.k.r.t.d....
+00001190: 017c 0564 016b 0472 2b74 00a0 0674 0764  .|.d.k.r+t...t.d
+000011a0: 037c 0513 0064 031b 0064 0483 02a1 0101  .|...d...d......
+000011b0: 007c 006a 01a0 027c 017c 006a 036a 04a1  .|.j...|.|.j.j..
+000011c0: 0272 0f7c 006a 086a 097c 006a 0a6a 0b7c  .r.|.j.j.|.j.j.|
+000011d0: 0164 058d 0201 0064 0653 0029 0761 9701  .d.....d.S.).a..
+000011e0: 0000 0a20 2020 2020 2020 204d 6172 6b73  ...        Marks
+000011f0: 2061 6e20 7570 6c6f 6164 2061 7320 2763   an upload as 'c
+00001200: 6f6d 706c 6574 6564 272c 2077 6869 6368  ompleted', which
+00001210: 2061 6c6c 6f77 7320 7468 6520 526f 626f   allows the Robo
+00001220: 746f 2050 6c61 7466 6f72 6d20 746f 2065  to Platform to e
+00001230: 7661 6c75 6174 6520 7472 6967 6765 7273  valuate triggers
+00001240: 2066 6f72 2061 7574 6f6d 6174 6963 2061   for automatic a
+00001250: 6374 696f 6e20 6f6e 0a20 2020 2020 2020  ction on.       
+00001260: 2069 6e63 6f6d 696e 6720 6461 7461 2e20   incoming data. 
+00001270: 5468 6973 2061 6c73 6f20 6169 6465 7320  This also aides 
+00001280: 7265 706f 7274 696e 6720 6f6e 2070 6172  reporting on par
+00001290: 7469 616c 2075 706c 6f61 6420 6661 696c  tial upload fail
+000012a0: 7572 6520 6361 7365 732e 0a0a 2020 2020  ure cases...    
+000012b0: 2020 2020 5468 6973 2041 5049 2069 7320      This API is 
+000012c0: 6361 6c6c 6564 2069 6d70 6c69 6369 746c  called implicitl
+000012d0: 7920 6279 2074 6865 2060 7570 6c6f 6164  y by the `upload
+000012e0: 5f66 696c 6560 2061 6e64 2060 7570 6c6f  _file` and `uplo
+000012f0: 6164 5f64 6972 6563 746f 7279 6020 6f70  ad_directory` op
+00001300: 6572 6174 696f 6e73 2c20 616e 6420 7368  erations, and sh
+00001310: 6f75 6c64 206f 6e6c 7920 6265 0a20 2020  ould only be.   
+00001320: 2020 2020 2075 7365 6420 6578 706c 6963       used explic
+00001330: 6974 6c79 2069 6e20 706f 7765 722d 7573  itly in power-us
+00001340: 6572 2073 6365 6e61 7269 6f73 2e0a 0a20  er scenarios... 
+00001350: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00001360: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
+00001370: 0a20 2020 2020 2020 2072 0100 0000 7a29  .        r....z)
+00001380: 5469 6d65 6420 6f75 7420 7761 6974 696e  Timed out waitin
+00001390: 6720 666f 7220 7570 6c6f 6164 2074 6f20  g for upload to 
+000013a0: 636f 6d70 6c65 7465 2e72 0f00 0000 e910  complete.r......
+000013b0: 0000 0029 0272 3d00 0000 7220 0000 004e  ...).r=...r ...N
+000013c0: 290c da04 7469 6d65 722d 0000 005a 1769  )...timer-...Z.i
+000013d0: 735f 7472 616e 7361 6374 696f 6e5f 636f  s_transaction_co
+000013e0: 6d70 6c65 7465 723b 0000 0072 3300 0000  mpleter;...r3...
+000013f0: da0c 5469 6d65 6f75 7445 7272 6f72 da05  ..TimeoutError..
+00001400: 736c 6565 70da 036d 696e 7229 0000 00da  sleep..minr)....
+00001410: 0f63 6f6d 706c 6574 655f 7570 6c6f 6164  .complete_upload
+00001420: 722b 0000 0072 3d00 0000 2906 7255 0000  r+...r=...).rU..
+00001430: 0072 2000 0000 725c 0000 0072 5d00 0000  .r ...r\...r]...
+00001440: da0a 7374 6172 745f 7469 6d65 da09 6974  ..start_time..it
+00001450: 6572 6174 696f 6e72 2600 0000 7226 0000  erationr&...r&..
+00001460: 0072 2700 0000 7263 0000 00a8 0000 0073  .r'...rc.......s
+00001470: 2000 0000 0810 0401 0601 0801 04ff 1003   ...............
+00001480: 0801 0801 1801 06fa 0801 04ff 0608 0601  ................
+00001490: 0201 0afe 7a17 4461 7461 7365 742e 636f  ....z.Dataset.co
+000014a0: 6d70 6c65 7465 5f75 706c 6f61 6463 0100  mplete_uploadc..
+000014b0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000014c0: 0000 4300 0000 7312 0000 007c 006a 00a0  ..C...s....|.j..
+000014d0: 017c 006a 02a1 0101 0064 0053 0072 3900  .|.j.....d.S.r9.
+000014e0: 0000 2903 7229 0000 00da 0e64 656c 6574  ..).r).....delet
+000014f0: 655f 6461 7461 7365 7472 2b00 0000 7257  e_datasetr+...rW
+00001500: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
+00001510: 0000 7266 0000 00c7 0000 0073 0200 0000  ..rf.......s....
+00001520: 1201 7a16 4461 7461 7365 742e 6465 6c65  ..z.Dataset.dele
+00001530: 7465 5f64 6174 6173 6574 da10 696e 636c  te_dataset..incl
+00001540: 7564 655f 7061 7474 6572 6e73 da10 6578  ude_patterns..ex
+00001550: 636c 7564 655f 7061 7474 6572 6e73 6303  clude_patternsc.
+00001560: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00001570: 0000 0043 0000 0073 1e00 0000 7c00 a000  ...C...s....|...
+00001580: 7c01 7c02 a102 4400 5d06 7d03 7c03 a001  |.|...D.].}.|...
+00001590: a100 0100 7106 6401 5300 2902 61e0 0100  ....q.d.S.).a...
+000015a0: 000a 2020 2020 2020 2020 4465 6c65 7465  ..        Delete
+000015b0: 2066 696c 6573 2061 7373 6f63 6961 7465   files associate
+000015c0: 6420 7769 7468 2074 6869 7320 6461 7461  d with this data
+000015d0: 7365 742e 0a0a 2020 2020 2020 2020 6069  set...        `i
+000015e0: 6e63 6c75 6465 5f70 6174 7465 726e 7360  nclude_patterns`
+000015f0: 2061 6e64 2060 6578 636c 7564 655f 7061   and `exclude_pa
+00001600: 7474 6572 6e73 6020 6172 6520 6c69 7374  tterns` are list
+00001610: 7320 6f66 2067 6974 6967 6e6f 7265 2d73  s of gitignore-s
+00001620: 7479 6c65 2070 6174 7465 726e 732e 0a20  tyle patterns.. 
+00001630: 2020 2020 2020 2053 6565 2068 7474 7073         See https
+00001640: 3a2f 2f67 6974 2d73 636d 2e63 6f6d 2f64  ://git-scm.com/d
+00001650: 6f63 732f 6769 7469 676e 6f72 652e 0a0a  ocs/gitignore...
+00001660: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
+00001670: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00001680: 2066 726f 6d20 726f 626f 746f 2e64 6f6d   from roboto.dom
+00001690: 6169 6e20 696d 706f 7274 2064 6174 6173  ain import datas
+000016a0: 6574 730a 2020 2020 2020 2020 2020 2020  ets.            
+000016b0: 3e3e 3e20 6461 7461 7365 7420 3d20 6461  >>> dataset = da
+000016c0: 7461 7365 7473 2e44 6174 6173 6574 282e  tasets.Dataset(.
+000016d0: 2e2e 290a 2020 2020 2020 2020 2020 2020  ..).            
+000016e0: 3e3e 3e20 6461 7461 7365 742e 6465 6c65  >>> dataset.dele
+000016f0: 7465 5f66 696c 6573 280a 2020 2020 2020  te_files(.      
+00001700: 2020 2020 2020 2e2e 2e20 2020 2069 6e63        ...    inc
+00001710: 6c75 6465 5f70 6174 7465 726e 733d 5b22  lude_patterns=["
+00001720: 2a2a 2f2a 2e70 6e67 225d 2c0a 2020 2020  **/*.png"],.    
+00001730: 2020 2020 2020 2020 2e2e 2e20 2020 2065          ...    e
+00001740: 7863 6c75 6465 5f70 6174 7465 726e 733d  xclude_patterns=
+00001750: 5b22 2a2a 2f62 6163 6b5f 6361 6d65 7261  ["**/back_camera
+00001760: 2f2a 2a22 5d0a 2020 2020 2020 2020 2020  /**"].          
+00001770: 2020 2e2e 2e20 290a 0a20 2020 2020 2020    ... )..       
+00001780: 204e 2902 da0a 6c69 7374 5f66 696c 6573   N)...list_files
+00001790: da06 6465 6c65 7465 2904 7255 0000 0072  ..delete).rU...r
+000017a0: 6700 0000 7268 0000 00da 0466 696c 6572  g...rh.....filer
+000017b0: 2600 0000 7226 0000 0072 2700 0000 da0c  &...r&...r'.....
+000017c0: 6465 6c65 7465 5f66 696c 6573 ca00 0000  delete_files....
+000017d0: 7306 0000 0010 140a 0104 ff7a 1444 6174  s..........z.Dat
+000017e0: 6173 6574 2e64 656c 6574 655f 6669 6c65  aset.delete_file
+000017f0: 73da 086f 7574 5f70 6174 6863 0400 0000  s..out_pathc....
+00001800: 0000 0000 0000 0000 0600 0000 0800 0000  ................
+00001810: 0300 0000 73b2 0000 0088 036a 006a 0174  ....s......j.j.t
+00001820: 026a 036b 0373 0e88 036a 006a 0474 056a  .j.k.s...j.j.t.j
+00001830: 066b 0372 1274 0764 0183 0182 0188 02a0  .k.r.t.d........
+00001840: 08a1 0073 1c88 026a 0964 0264 038d 0101  ...s...j.d.d....
+00001850: 0087 0366 0164 0464 0584 087d 0464 0674  ...f.d.d...}.d.t
+00001860: 0a64 0774 0b74 0c74 0d6a 0e66 0219 0066  .d.t.t.t.j.f...f
+00001870: 0487 0266 0164 0864 0984 0c89 0074 0f88  ...f.d.d.....t..
+00001880: 03a0 107c 027c 03a1 0283 0189 0187 0087  ...|.|..........
+00001890: 0166 0264 0a64 0b84 087d 0588 036a 116a  .f.d.d...}...j.j
+000018a0: 127c 0583 007c 0474 1364 0c88 036a 006a  .|...|.t.d...j.j
+000018b0: 1474 1588 0183 0164 0d9c 0264 0e8d 0264  .t.....d...d...d
+000018c0: 0f64 108d 0401 0064 1153 0029 1261 6702  .d.....d.S.).ag.
+000018d0: 0000 0a20 2020 2020 2020 2044 6f77 6e6c  ...        Downl
+000018e0: 6f61 6420 6669 6c65 7320 6173 736f 6369  oad files associ
+000018f0: 6174 6564 2077 6974 6820 7468 6973 2064  ated with this d
+00001900: 6174 6173 6574 2074 6f20 7468 6520 6769  ataset to the gi
+00001910: 7665 6e20 6469 7265 6374 6f72 792e 0a20  ven directory.. 
+00001920: 2020 2020 2020 2049 6620 606f 7574 5f70         If `out_p
+00001930: 6174 6860 2064 6f65 7320 6e6f 7420 6578  ath` does not ex
+00001940: 6973 742c 2069 7420 7769 6c6c 2062 6520  ist, it will be 
+00001950: 6372 6561 7465 642e 0a0a 2020 2020 2020  created...      
+00001960: 2020 6069 6e63 6c75 6465 5f70 6174 7465    `include_patte
+00001970: 726e 7360 2061 6e64 2060 6578 636c 7564  rns` and `exclud
+00001980: 655f 7061 7474 6572 6e73 6020 6172 6520  e_patterns` are 
+00001990: 6c69 7374 7320 6f66 2067 6974 6967 6e6f  lists of gitigno
+000019a0: 7265 2d73 7479 6c65 2070 6174 7465 726e  re-style pattern
+000019b0: 732e 0a20 2020 2020 2020 2053 6565 2068  s..        See h
+000019c0: 7474 7073 3a2f 2f67 6974 2d73 636d 2e63  ttps://git-scm.c
+000019d0: 6f6d 2f64 6f63 732f 6769 7469 676e 6f72  om/docs/gitignor
+000019e0: 652e 0a0a 2020 2020 2020 2020 4578 616d  e...        Exam
+000019f0: 706c 653a 0a20 2020 2020 2020 2020 2020  ple:.           
+00001a00: 203e 3e3e 2066 726f 6d20 726f 626f 746f   >>> from roboto
+00001a10: 2e64 6f6d 6169 6e20 696d 706f 7274 2064  .domain import d
+00001a20: 6174 6173 6574 730a 2020 2020 2020 2020  atasets.        
+00001a30: 2020 2020 3e3e 3e20 6461 7461 7365 7420      >>> dataset 
+00001a40: 3d20 6461 7461 7365 7473 2e44 6174 6173  = datasets.Datas
+00001a50: 6574 282e 2e2e 290a 2020 2020 2020 2020  et(...).        
+00001a60: 2020 2020 3e3e 3e20 6461 7461 7365 742e      >>> dataset.
+00001a70: 646f 776e 6c6f 6164 5f66 696c 6573 280a  download_files(.
+00001a80: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+00001a90: 2020 2020 7061 7468 6c69 622e 5061 7468      pathlib.Path
+00001aa0: 2822 2f74 6d70 2f74 6d70 2e6e 5631 6764  ("/tmp/tmp.nV1gd
+00001ab0: 5735 5748 5622 292c 0a20 2020 2020 2020  W5WHV"),.       
+00001ac0: 2020 2020 202e 2e2e 2020 2020 2069 6e63       ...     inc
+00001ad0: 6c75 6465 5f70 6174 7465 726e 733d 5b22  lude_patterns=["
+00001ae0: 2a2a 2f2a 2e67 3422 5d2c 0a20 2020 2020  **/*.g4"],.     
+00001af0: 2020 2020 2020 202e 2e2e 2020 2020 2065         ...     e
+00001b00: 7863 6c75 6465 5f70 6174 7465 726e 733d  xclude_patterns=
+00001b10: 5b22 2a2a 2f74 6573 742f 2a2a 225d 0a20  ["**/test/**"]. 
+00001b20: 2020 2020 2020 2020 2020 202e 2e2e 2029             ... )
+00001b30: 0a20 2020 2020 2020 20fa 484f 6e6c 7920  .        .HOnly 
+00001b40: 5333 2d62 6163 6b65 6420 7374 6f72 6167  S3-backed storag
+00001b50: 6520 6164 6d69 6e69 7374 6572 6564 2062  e administered b
+00001b60: 7920 526f 626f 746f 2069 7320 7375 7070  y Roboto is supp
+00001b70: 6f72 7465 6420 6174 2074 6869 7320 7469  orted at this ti
+00001b80: 6d65 2e54 2901 da07 7061 7265 6e74 7363  me.T)...parentsc
+00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ba0: 0300 0000 1300 0000 7310 0000 0088 00a0  ........s.......
+00001bb0: 0074 016a 02a1 01a0 03a1 0053 0072 3900  .t.j.......S.r9.
+00001bc0: 0000 2904 da19 6765 745f 7465 6d70 6f72  ..)...get_tempor
+00001bd0: 6172 795f 6372 6564 656e 7469 616c 7372  ary_credentialsr
+00001be0: 0300 0000 da08 5265 6164 4f6e 6c79 da11  ......ReadOnly..
+00001bf0: 746f 5f73 335f 6372 6564 656e 7469 616c  to_s3_credential
+00001c00: 7372 2600 0000 7257 0000 0072 2600 0000  sr&...rW...r&...
+00001c10: 7227 0000 00da 145f 6372 6564 656e 7469  r'....._credenti
+00001c20: 616c 5f70 726f 7669 6465 7202 0100 0073  al_provider....s
+00001c30: 0a00 0000 0401 0401 02ff 0402 02fe 7a34  ..............z4
+00001c40: 4461 7461 7365 742e 646f 776e 6c6f 6164  Dataset.download
+00001c50: 5f66 696c 6573 2e3c 6c6f 6361 6c73 3e2e  _files.<locals>.
+00001c60: 5f63 7265 6465 6e74 6961 6c5f 7072 6f76  _credential_prov
+00001c70: 6964 6572 da01 6672 3800 0000 6301 0000  ider..fr8...c...
+00001c80: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00001c90: 0013 0000 0073 1000 0000 7c00 6a00 8800  .....s....|.j...
+00001ca0: 7c00 6a01 1b00 6602 5300 7239 0000 0029  |.j...f.S.r9...)
+00001cb0: 0272 3b00 0000 da0d 7265 6c61 7469 7665  .r;.....relative
+00001cc0: 5f70 6174 6829 0172 7400 0000 2901 726d  _path).rt...).rm
+00001cd0: 0000 0072 2600 0000 7227 0000 00da 175f  ...r&...r'....._
+00001ce0: 6669 6c65 5f74 6f5f 646f 776e 6c6f 6164  file_to_download
+00001cf0: 5f74 7570 6c65 0701 0000 7302 0000 0010  _tuple....s.....
+00001d00: 017a 3744 6174 6173 6574 2e64 6f77 6e6c  .z7Dataset.downl
+00001d10: 6f61 645f 6669 6c65 732e 3c6c 6f63 616c  oad_files.<local
+00001d20: 733e 2e5f 6669 6c65 5f74 6f5f 646f 776e  s>._file_to_down
+00001d30: 6c6f 6164 5f74 7570 6c65 6300 0000 0000  load_tuplec.....
+00001d40: 0000 0000 0000 0001 0000 0003 0000 0033  ...............3
+00001d50: 0000 0073 1c00 0000 8100 7400 8800 8801  ...s......t.....
+00001d60: 8302 4400 5d05 7d00 7c00 5600 0100 7106  ..D.].}.|.V...q.
+00001d70: 6400 5300 7239 0000 0029 01da 036d 6170  d.S.r9...)...map
+00001d80: 2901 da01 7829 0272 7600 0000 da09 616c  )...x).rv.....al
+00001d90: 6c5f 6669 6c65 7372 2600 0000 7227 0000  l_filesr&...r'..
+00001da0: 00da 0f5f 6669 6c65 5f67 656e 6572 6174  ..._file_generat
+00001db0: 6f72 0c01 0000 730e 0000 0002 8002 0102  or....s.........
+00001dc0: 0102 0108 fe08 0404 fc7a 2f44 6174 6173  .........z/Datas
+00001dd0: 6574 2e64 6f77 6e6c 6f61 645f 6669 6c65  et.download_file
+00001de0: 732e 3c6c 6f63 616c 733e 2e5f 6669 6c65  s.<locals>._file
+00001df0: 5f67 656e 6572 6174 6f72 7217 0000 0029  _generatorr....)
+00001e00: 02da 0962 6173 655f 7061 7468 5a10 746f  ...base_pathZ.to
+00001e10: 7461 6c5f 6669 6c65 5f63 6f75 6e74 a902  tal_file_count..
+00001e20: da0b 636f 6e63 7572 7265 6e63 79da 0363  ..concurrency..c
+00001e30: 7478 e908 0000 0029 04da 0e66 696c 655f  tx.....)...file_
+00001e40: 6765 6e65 7261 746f 72da 1363 7265 6465  generator..crede
+00001e50: 6e74 6961 6c5f 7072 6f76 6964 6572 da18  ntial_provider..
+00001e60: 7072 6f67 7265 7373 5f6d 6f6e 6974 6f72  progress_monitor
+00001e70: 5f66 6163 746f 7279 da0f 6d61 785f 636f  _factory..max_co
+00001e80: 6e63 7572 7265 6e63 794e 2916 722b 0000  ncurrencyN).r+..
+00001e90: 0072 3200 0000 721a 0000 00da 0253 3372  .r2...r......S3r
+00001ea0: 3100 0000 721b 0000 00da 0652 6f62 6f74  1...r......Robot
+00001eb0: 6fda 134e 6f74 496d 706c 656d 656e 7465  o..NotImplemente
+00001ec0: 6445 7272 6f72 da06 6973 5f64 6972 da05  dError..is_dir..
+00001ed0: 6d6b 6469 7272 1100 0000 da05 7475 706c  mkdirr......tupl
+00001ee0: 6572 1300 0000 da07 7061 7468 6c69 62da  er......pathlib.
+00001ef0: 0450 6174 68da 046c 6973 7472 6900 0000  .Path..listri...
+00001f00: 722a 0000 00da 0e64 6f77 6e6c 6f61 645f  r*.....download_
+00001f10: 6669 6c65 7372 1600 0000 723d 0000 0072  filesr....r=...r
+00001f20: 4900 0000 2906 7255 0000 0072 6d00 0000  I...).rU...rm...
+00001f30: 7267 0000 0072 6800 0000 7273 0000 0072  rg...rh...rs...r
+00001f40: 7a00 0000 7226 0000 0029 0472 7600 0000  z...r&...).rv...
+00001f50: 7279 0000 0072 6d00 0000 7255 0000 0072  ry...rm...rU...r
+00001f60: 2700 0000 728d 0000 00e1 0000 0073 2c00  '...r........s,.
+00001f70: 0000 0e17 0e01 0202 0201 04ff 0804 0c01  ................
+00001f80: 0c02 2005 1003 0e02 0607 0401 0201 0201  .. .............
+00001f90: 0201 0602 0601 04fe 04fe 0207 0af6 7a16  ..............z.
+00001fa0: 4461 7461 7365 742e 646f 776e 6c6f 6164  Dataset.download
+00001fb0: 5f66 696c 6573 7275 0000 0063 0200 0000  _filesru...c....
+00001fc0: 0000 0000 0000 0000 0300 0000 0600 0000  ................
+00001fd0: 4300 0000 735e 0000 0074 007c 006a 0174  C...s^...t.|.j.t
+00001fe0: 027c 0183 0167 0164 018d 0183 017d 027c  .|...g.d.....}.|
+00001ff0: 0273 1974 0364 027c 019b 0064 037c 006a  .s.t.d.|...d.|.j
+00002000: 049b 0064 049d 0583 0182 0174 057c 0283  ...d.......t.|..
+00002010: 0164 056b 0472 2b74 0664 067c 019b 0064  .d.k.r+t.d.|...d
+00002020: 077c 006a 049b 0064 049d 0583 0182 017c  .|.j...d.......|
+00002030: 0264 0819 0053 0029 0961 2d01 0000 0a20  .d...S.).a-.... 
+00002040: 2020 2020 2020 2047 6574 2061 2046 696c         Get a Fil
+00002050: 6520 6f62 6a65 6374 2066 6f72 2074 6865  e object for the
+00002060: 2067 6976 656e 2072 656c 6174 6976 6520   given relative 
+00002070: 7061 7468 2e0a 0a20 2020 2020 2020 2045  path...        E
+00002080: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+00002090: 2020 2020 3e3e 3e20 6672 6f6d 2072 6f62      >>> from rob
+000020a0: 6f74 6f2e 646f 6d61 696e 2069 6d70 6f72  oto.domain impor
+000020b0: 7420 6461 7461 7365 7473 0a20 2020 2020  t datasets.     
+000020c0: 2020 2020 2020 203e 3e3e 2064 6174 6173         >>> datas
+000020d0: 6574 203d 2064 6174 6173 6574 732e 4461  et = datasets.Da
+000020e0: 7461 7365 7428 2e2e 2e29 0a20 2020 2020  taset(...).     
+000020f0: 2020 2020 2020 203e 3e3e 2066 696c 6520         >>> file 
+00002100: 3d20 6461 7461 7365 742e 6765 745f 6669  = dataset.get_fi
+00002110: 6c65 5f69 6e66 6f28 2266 6f6f 2f62 6172  le_info("foo/bar
+00002120: 2e74 7874 2229 0a20 2020 2020 2020 2020  .txt").         
+00002130: 2020 203e 3e3e 2070 7269 6e74 2866 696c     >>> print(fil
+00002140: 652e 6669 6c65 5f69 6429 0a20 2020 2020  e.file_id).     
+00002150: 2020 2020 2020 2066 696c 652d 6162 6331         file-abc1
+00002160: 3233 0a20 2020 2020 2020 2029 0172 6700  23.        ).rg.
+00002170: 0000 7a06 4669 6c65 2027 7a18 2720 6e6f  ..z.File 'z.' no
+00002180: 7420 666f 756e 6420 696e 2064 6174 6173  t found in datas
+00002190: 6574 2027 da01 2772 1700 0000 7a1a 4d75  et '..'r....z.Mu
+000021a0: 6c74 6970 6c65 2066 696c 6573 2066 6f75  ltiple files fou
+000021b0: 6e64 2066 6f72 2027 7a0e 2720 696e 2064  nd for 'z.' in d
+000021c0: 6174 6173 6574 2027 7201 0000 0029 0772  ataset 'r....).r
+000021d0: 8c00 0000 7269 0000 0072 2400 0000 7205  ....ri...r$...r.
+000021e0: 0000 0072 3d00 0000 7249 0000 0072 0400  ...r=...rI...r..
+000021f0: 0000 2903 7255 0000 0072 7500 0000 da08  ..).rU...ru.....
+00002200: 6d61 7463 6869 6e67 7226 0000 0072 2600  matchingr&...r&.
+00002210: 0000 7227 0000 00da 0d67 6574 5f66 696c  ..r'.....get_fil
+00002220: 655f 696e 666f 2001 0000 7314 0000 0016  e_info ...s.....
+00002230: 0e04 0102 0112 0104 ff0c 0402 0112 0104  ................
+00002240: ff08 047a 1544 6174 6173 6574 2e67 6574  ...z.Dataset.get
+00002250: 5f66 696c 655f 696e 666f 46da 0b70 6572  _file_infoF..per
+00002260: 6d69 7373 696f 6e73 da0d 666f 7263 655f  missions..force_
+00002270: 7265 6672 6573 6863 0500 0000 0000 0000  refreshc........
+00002280: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
+00002290: 733e 0000 007c 0373 117c 0174 006a 016b  s>...|.s.|.t.j.k
+000022a0: 0273 117c 006a 0264 0075 0073 117c 006a  .s.|.j.d.u.s.|.j
+000022b0: 02a0 03a1 0072 1c7c 006a 04a0 057c 006a  .....r.|.j...|.j
+000022c0: 067c 017c 027c 04a1 047c 005f 027c 006a  .|.|.|...|._.|.j
+000022d0: 0253 0072 3900 0000 2907 7203 0000 00da  .S.r9...).r.....
+000022e0: 0952 6561 6457 7269 7465 722c 0000 00da  .ReadWriter,....
+000022f0: 0a69 735f 6578 7069 7265 6472 2900 0000  .is_expiredr)...
+00002300: 7270 0000 0072 2b00 0000 2905 7255 0000  rp...r+...).rU..
+00002310: 0072 9100 0000 725c 0000 0072 9200 0000  .r....r\...r....
+00002320: 7220 0000 0072 2600 0000 7226 0000 0072  r ...r&...r&...r
+00002330: 2700 0000 7270 0000 003b 0100 0073 1400  '...rp...;...s..
+00002340: 0000 0208 02ff 0a02 0a01 0801 02ff 0603  ................
+00002350: 0a01 06ff 0603 7a21 4461 7461 7365 742e  ......z!Dataset.
+00002360: 6765 745f 7465 6d70 6f72 6172 795f 6372  get_temporary_cr
+00002370: 6564 656e 7469 616c 7363 0300 0000 0000  edentialsc......
+00002380: 0000 0000 0000 0500 0000 0600 0000 6300  ..............c.
+00002390: 0000 735c 0000 0081 007c 006a 006a 017c  ..s\.....|.j.j.|
+000023a0: 006a 026a 037c 017c 0264 018d 037d 0309  .j.j.|.|.d...}..
+000023b0: 007c 036a 0444 005d 097d 0474 057c 047c  .|.j.D.].}.t.|.|
+000023c0: 006a 0683 0256 0001 0071 107c 036a 0772  .j...V...q.|.j.r
+000023d0: 2b7c 006a 006a 017c 006a 026a 037c 036a  +|.j.j.|.j.j.|.j
+000023e0: 077c 017c 0264 018d 047d 036e 0264 0353  .|.|.d...}.n.d.S
+000023f0: 0071 0d29 0461 1002 0000 0a20 2020 2020  .q.).a.....     
+00002400: 2020 204c 6973 7420 6669 6c65 7320 6173     List files as
+00002410: 736f 6369 6174 6564 2077 6974 6820 7468  sociated with th
+00002420: 6973 2064 6174 6173 6574 2e0a 0a20 2020  is dataset...   
+00002430: 2020 2020 2060 696e 636c 7564 655f 7061       `include_pa
+00002440: 7474 6572 6e73 6020 616e 6420 6065 7863  tterns` and `exc
+00002450: 6c75 6465 5f70 6174 7465 726e 7360 2061  lude_patterns` a
+00002460: 7265 206c 6973 7473 206f 6620 6769 7469  re lists of giti
+00002470: 676e 6f72 652d 7374 796c 6520 7061 7474  gnore-style patt
+00002480: 6572 6e73 2e0a 2020 2020 2020 2020 5365  erns..        Se
+00002490: 6520 6874 7470 733a 2f2f 6769 742d 7363  e https://git-sc
+000024a0: 6d2e 636f 6d2f 646f 6373 2f67 6974 6967  m.com/docs/gitig
+000024b0: 6e6f 7265 2e0a 0a20 2020 2020 2020 2045  nore...        E
+000024c0: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+000024d0: 2020 2020 3e3e 3e20 6672 6f6d 2072 6f62      >>> from rob
+000024e0: 6f74 6f2e 646f 6d61 696e 2069 6d70 6f72  oto.domain impor
+000024f0: 7420 6461 7461 7365 7473 0a20 2020 2020  t datasets.     
+00002500: 2020 2020 2020 203e 3e3e 2064 6174 6173         >>> datas
+00002510: 6574 203d 2064 6174 6173 6574 732e 4461  et = datasets.Da
+00002520: 7461 7365 7428 2e2e 2e29 0a20 2020 2020  taset(...).     
+00002530: 2020 2020 2020 203e 3e3e 2066 6f72 2066         >>> for f
+00002540: 696c 6520 696e 2064 6174 6173 6574 2e6c  ile in dataset.l
+00002550: 6973 745f 6669 6c65 7328 0a20 2020 2020  ist_files(.     
+00002560: 2020 2020 2020 202e 2e2e 2020 2020 2069         ...     i
+00002570: 6e63 6c75 6465 5f70 6174 7465 726e 733d  nclude_patterns=
+00002580: 5b22 2a2a 2f2a 2e67 3422 5d2c 0a20 2020  ["**/*.g4"],.   
+00002590: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
+000025a0: 2065 7863 6c75 6465 5f70 6174 7465 726e   exclude_pattern
+000025b0: 733d 5b22 2a2a 2f74 6573 742f 2a2a 225d  s=["**/test/**"]
+000025c0: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+000025d0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000025e0: 2e2e 2e20 2020 2020 7072 696e 7428 6669  ...     print(fi
+000025f0: 6c65 2e72 656c 6174 6976 655f 7061 7468  le.relative_path
+00002600: 290a 2020 2020 2020 2020 2902 7267 0000  ).        ).rg..
+00002610: 0072 6800 0000 544e 2908 7229 0000 0072  .rh...TN).r)...r
+00002620: 6900 0000 722b 0000 0072 3d00 0000 724b  i...r+...r=...rK
+00002630: 0000 0072 1100 0000 722a 0000 0072 4c00  ...r....r*...rL.
+00002640: 0000 2905 7255 0000 0072 6700 0000 7268  ..).rU...rg...rh
+00002650: 0000 0072 5400 0000 723b 0000 0072 2600  ...rT...r;...r&.
+00002660: 0000 7226 0000 0072 2700 0000 7269 0000  ..r&...r'...ri..
+00002670: 004d 0100 0073 2400 0000 0280 0615 0601  .M...s$.........
+00002680: 0201 0201 06fd 0205 0a01 1001 0601 0601  ................
+00002690: 0601 0401 0201 0201 08fc 0407 02f5 7a12  ..............z.
+000026a0: 4461 7461 7365 742e 6c69 7374 5f66 696c  Dataset.list_fil
+000026b0: 6573 da0a 7570 6461 7465 645f 6279 6303  es..updated_byc.
+000026c0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+000026d0: 0000 0043 0000 00f3 1800 0000 7c00 6a00  ...C........|.j.
+000026e0: 7401 7c01 6401 8d01 7c02 6402 8d02 0100  t.|.d...|.d.....
+000026f0: 6403 5300 2904 61c1 0100 000a 2020 2020  d.S.).a.....    
+00002700: 2020 2020 5365 7420 6561 6368 2060 6b65      Set each `ke
+00002710: 7960 3a20 6076 616c 7565 6020 696e 2074  y`: `value` in t
+00002720: 6869 7320 6469 6374 2061 7320 6461 7461  his dict as data
+00002730: 7365 7420 6d65 7461 6461 7461 2069 6620  set metadata if 
+00002740: 6974 2064 6f65 736e 2774 2065 7869 7374  it doesn't exist
+00002750: 2c20 656c 7365 206f 7665 7277 7269 7465  , else overwrite
+00002760: 2074 6865 2065 7869 7374 696e 6720 7661   the existing va
+00002770: 6c75 652e 0a20 2020 2020 2020 204b 6579  lue..        Key
+00002780: 7320 6d75 7374 2062 6520 7374 7269 6e67  s must be string
+00002790: 732e 2044 6f74 206e 6f74 6174 696f 6e20  s. Dot notation 
+000027a0: 6973 2073 7570 706f 7274 6564 2066 6f72  is supported for
+000027b0: 206e 6573 7465 6420 6b65 7973 2e0a 0a20   nested keys... 
+000027c0: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
+000027d0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+000027e0: 6672 6f6d 2072 6f62 6f74 6f2e 646f 6d61  from roboto.doma
+000027f0: 696e 2069 6d70 6f72 7420 6461 7461 7365  in import datase
+00002800: 7473 0a20 2020 2020 2020 2020 2020 203e  ts.            >
+00002810: 3e3e 2064 6174 6173 6574 203d 2064 6174  >> dataset = dat
+00002820: 6173 6574 732e 4461 7461 7365 7428 2e2e  asets.Dataset(..
+00002830: 2e29 0a20 2020 2020 2020 2020 2020 203e  .).            >
+00002840: 3e3e 2064 6174 6173 6574 2e70 7574 5f6d  >> dataset.put_m
+00002850: 6574 6164 6174 6128 7b0a 2020 2020 2020  etadata({.      
+00002860: 2020 2020 2020 2e2e 2e20 2020 2020 2266        ...     "f
+00002870: 6f6f 223a 2022 6261 7222 2c0a 2020 2020  oo": "bar",.    
+00002880: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+00002890: 2262 617a 2e71 7578 223a 2031 3031 2c0a  "baz.qux": 101,.
+000028a0: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+000028b0: 7d29 0a0a 2020 2020 2020 2020 2901 da0a  })..        )...
+000028c0: 7075 745f 6669 656c 6473 a902 da12 6d65  put_fields....me
+000028d0: 7461 6461 7461 5f63 6861 6e67 6573 6574  tadata_changeset
+000028e0: 7295 0000 004e a902 da06 7570 6461 7465  r....N....update
+000028f0: 720c 0000 00a9 0372 5500 0000 7235 0000  r......rU...r5..
+00002900: 0072 9500 0000 7226 0000 0072 2600 0000  .r....r&...r&...
+00002910: 7227 0000 00da 0c70 7574 5f6d 6574 6164  r'.....put_metad
+00002920: 6174 6174 0100 0073 0800 0000 0412 0801  atat...s........
+00002930: 0201 0afe 7a14 4461 7461 7365 742e 7075  ....z.Dataset.pu
+00002940: 745f 6d65 7461 6461 7461 6303 0000 0000  t_metadatac.....
+00002950: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00002960: 0000 0072 9600 0000 2904 7a31 4164 6420  ...r....).z1Add 
+00002970: 6561 6368 2074 6167 2069 6e20 7468 6973  each tag in this
+00002980: 2073 6571 7565 6e63 6520 6966 2069 7420   sequence if it 
+00002990: 646f 6573 6e27 7420 6578 6973 7429 01da  doesn't exist)..
+000029a0: 0870 7574 5f74 6167 7372 9800 0000 4e72  .put_tagsr....Nr
+000029b0: 9a00 0000 a903 7255 0000 0072 3600 0000  ......rU...r6...
+000029c0: 7295 0000 0072 2600 0000 7226 0000 0072  r....r&...r&...r
+000029d0: 2700 0000 729e 0000 008b 0100 00f3 0800  '...r...........
+000029e0: 0000 0406 0801 0201 0afe 7a10 4461 7461  ..........z.Data
+000029f0: 7365 742e 7075 745f 7461 6773 6301 0000  set.put_tagsc...
+00002a00: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00002a10: 0043 0000 0073 1600 0000 7c00 6a00 a001  .C...s....|.j...
+00002a20: 7c00 6a02 6a03 a101 7c00 5f02 6401 5300  |.j.j...|._.d.S.
+00002a30: 2902 7a43 5265 6672 6573 6820 7468 6520  ).zCRefresh the 
+00002a40: 756e 6465 726c 7969 6e67 2064 6174 6173  underlying datas
+00002a50: 6574 2072 6563 6f72 6420 7769 7468 2074  et record with t
+00002a60: 6865 206c 6174 6573 7420 7365 7276 6572  he latest server
+00002a70: 2073 7461 7465 2e4e 2904 7229 0000 0072   state.N).r)...r
+00002a80: 3e00 0000 722b 0000 0072 3d00 0000 7257  >...r+...r=...rW
+00002a90: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
+00002aa0: 0000 da07 7265 6672 6573 6896 0100 0073  ....refresh....s
+00002ab0: 0600 0000 0602 0601 0aff 7a0f 4461 7461  ..........z.Data
+00002ac0: 7365 742e 7265 6672 6573 6863 0300 0000  set.refreshc....
+00002ad0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00002ae0: 4300 0000 7296 0000 0029 0461 5001 0000  C...r....).aP...
+00002af0: 0a20 2020 2020 2020 2052 656d 6f76 6520  .        Remove 
+00002b00: 6561 6368 206b 6579 2069 6e20 7468 6973  each key in this
+00002b10: 2073 6571 7565 6e63 6520 6672 6f6d 2064   sequence from d
+00002b20: 6174 6173 6574 206d 6574 6164 6174 6120  ataset metadata 
+00002b30: 6966 2069 7420 6578 6973 7473 2e0a 2020  if it exists..  
+00002b40: 2020 2020 2020 4b65 7973 206d 7573 7420        Keys must 
+00002b50: 6265 2073 7472 696e 6773 2e20 446f 7420  be strings. Dot 
+00002b60: 6e6f 7461 7469 6f6e 2069 7320 7375 7070  notation is supp
+00002b70: 6f72 7465 6420 666f 7220 6e65 7374 6564  orted for nested
+00002b80: 206b 6579 732e 0a0a 2020 2020 2020 2020   keys...        
+00002b90: 4578 616d 706c 653a 0a20 2020 2020 2020  Example:.       
+00002ba0: 2020 2020 203e 3e3e 2066 726f 6d20 726f       >>> from ro
+00002bb0: 626f 746f 2e64 6f6d 6169 6e20 696d 706f  boto.domain impo
+00002bc0: 7274 2064 6174 6173 6574 730a 2020 2020  rt datasets.    
+00002bd0: 2020 2020 2020 2020 3e3e 3e20 6461 7461          >>> data
+00002be0: 7365 7420 3d20 6461 7461 7365 7473 2e44  set = datasets.D
+00002bf0: 6174 6173 6574 282e 2e2e 290a 2020 2020  ataset(...).    
+00002c00: 2020 2020 2020 2020 3e3e 3e20 6461 7461          >>> data
+00002c10: 7365 742e 7265 6d6f 7665 5f6d 6574 6164  set.remove_metad
+00002c20: 6174 6128 5b22 666f 6f22 2c20 2262 617a  ata(["foo", "baz
+00002c30: 2e71 7578 225d 290a 2020 2020 2020 2020  .qux"]).        
+00002c40: 2901 da0d 7265 6d6f 7665 5f66 6965 6c64  )...remove_field
+00002c50: 7372 9800 0000 4e72 9a00 0000 729c 0000  sr....Nr....r...
+00002c60: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
+00002c70: da0f 7265 6d6f 7665 5f6d 6574 6164 6174  ..remove_metadat
+00002c80: 619c 0100 0073 0800 0000 040e 0801 0201  a....s..........
+00002c90: 0afe 7a17 4461 7461 7365 742e 7265 6d6f  ..z.Dataset.remo
+00002ca0: 7665 5f6d 6574 6164 6174 6163 0300 0000  ve_metadatac....
+00002cb0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00002cc0: 4300 0000 7296 0000 0029 047a 2d52 656d  C...r....).z-Rem
+00002cd0: 6f76 6520 6561 6368 2074 6167 2069 6e20  ove each tag in 
+00002ce0: 7468 6973 2073 6571 7565 6e63 6520 6966  this sequence if
+00002cf0: 2069 7420 6578 6973 7473 2901 da0b 7265   it exists)...re
+00002d00: 6d6f 7665 5f74 6167 7372 9800 0000 4e72  move_tagsr....Nr
+00002d10: 9a00 0000 729f 0000 0072 2600 0000 7226  ....r....r&...r&
+00002d20: 0000 0072 2700 0000 72a4 0000 00af 0100  ...r'...r.......
+00002d30: 0072 a000 0000 7a13 4461 7461 7365 742e  .r....z.Dataset.
+00002d40: 7265 6d6f 7665 5f74 6167 7363 0100 0000  remove_tagsc....
+00002d50: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00002d60: 4300 0000 730a 0000 0074 007c 006a 0183  C...s....t.|.j..
+00002d70: 0153 0072 3900 0000 2902 7208 0000 0072  .S.r9...).r....r
+00002d80: 2b00 0000 7257 0000 0072 2600 0000 7226  +...rW...r&...r&
+00002d90: 0000 0072 2700 0000 da07 746f 5f64 6963  ...r'.....to_dic
+00002da0: 74ba 0100 0073 0200 0000 0a01 7a0f 4461  t....s......z.Da
+00002db0: 7461 7365 742e 746f 5f64 6963 74da 0e64  taset.to_dict..d
+00002dc0: 6972 6563 746f 7279 5f70 6174 6863 0400  irectory_pathc..
+00002dd0: 0000 0000 0000 0000 0000 0500 0000 0c00  ................
+00002de0: 0000 0300 0000 7346 0100 007c 01a0 00a1  ......sF...|....
+00002df0: 0073 0b74 017c 019b 0064 019d 0283 0182  .s.t.|...d......
+00002e00: 0164 0289 037c 0264 0275 0172 1774 026a  .d...|.d.u.r.t.j
+00002e10: 03a0 047c 02a1 0189 0364 0389 0464 0389  ...|.....d...d..
+00002e20: 0564 0474 056a 0664 0564 0266 0487 0087  .d.t.j.d.d.f....
+00002e30: 0387 0487 0566 0464 0664 0784 0c89 0088  .....f.d.d......
+00002e40: 007c 0183 0101 0088 0464 036b 0272 3974  .|.......d.k.r9t
+00002e50: 07a0 0864 08a1 0101 0064 0253 0088 066a  ...d.....d.S...j
+00002e60: 0988 0464 098d 0189 0788 066a 0a74 0b6a  ...d.......j.t.j
+00002e70: 0c88 076a 0d64 0a8d 0289 0287 0687 0766  ...j.d.........f
+00002e80: 0264 0b64 0c84 087d 0464 0d74 056a 0664  .d.d...}.d.t.j.d
+00002e90: 0e74 0e64 0574 0f6a 106a 1174 1274 056a  .t.d.t.j.j.t.t.j
+00002ea0: 0674 0e66 0219 0064 0264 0266 0319 0066  .t.f...d.d.f...f
+00002eb0: 0687 0187 0287 0366 0364 0f64 1084 0c89  .......f.d.d....
+00002ec0: 0188 066a 136a 1488 026a 1588 017c 0164  ...j.j...j...|.d
+00002ed0: 1183 027c 0474 166a 1788 066a 186a 1974  ...|.t.j...j.j.t
+00002ee0: 166a 1a88 066a 186a 1b74 166a 1c88 026a  .j...j.j.t.j...j
+00002ef0: 1d74 166a 1e88 076a 0d69 0474 1f64 1274  .t.j...j.i.t.d.t
+00002f00: 0e7c 01a0 20a1 0083 0188 0488 0564 139c  .|.. ........d..
+00002f10: 0364 148d 0264 1564 168d 0601 0088 066a  .d...d.d.......j
+00002f20: 2188 076a 0d7c 0364 178d 0201 0064 0253  !..j.|.d.....d.S
+00002f30: 0029 1861 b502 0000 0a20 2020 2020 2020  .).a.....       
+00002f40: 2055 706c 6f61 6420 6576 6572 7974 6869   Upload everythi
+00002f50: 6e67 2c20 7265 6375 7273 6976 656c 792c  ng, recursively,
+00002f60: 2069 6e20 6469 7265 6374 6f72 792c 2069   in directory, i
+00002f70: 676e 6f72 696e 6720 6669 6c65 7320 7468  gnoring files th
+00002f80: 6174 206d 6174 6368 2061 6e79 206f 6620  at match any of 
+00002f90: 7468 6520 6967 6e6f 7265 2070 6174 7465  the ignore patte
+00002fa0: 726e 732e 0a0a 2020 2020 2020 2020 6065  rns...        `e
+00002fb0: 7863 6c75 6465 5f70 6174 7465 726e 7360  xclude_patterns`
+00002fc0: 2069 7320 6120 6c69 7374 206f 6620 6769   is a list of gi
+00002fd0: 7469 676e 6f72 652d 7374 796c 6520 7061  tignore-style pa
+00002fe0: 7474 6572 6e73 2e0a 2020 2020 2020 2020  tterns..        
+00002ff0: 5365 6520 6874 7470 733a 2f2f 6769 742d  See https://git-
+00003000: 7363 6d2e 636f 6d2f 646f 6373 2f67 6974  scm.com/docs/git
+00003010: 6967 6e6f 7265 235f 7061 7474 6572 6e5f  ignore#_pattern_
+00003020: 666f 726d 6174 2e0a 0a20 2020 2020 2020  format...       
+00003030: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
+00003040: 2020 2020 2020 3e3e 3e20 6672 6f6d 2072        >>> from r
+00003050: 6f62 6f74 6f2e 646f 6d61 696e 2069 6d70  oboto.domain imp
+00003060: 6f72 7420 6461 7461 7365 7473 0a20 2020  ort datasets.   
+00003070: 2020 2020 2020 2020 203e 3e3e 2064 6174           >>> dat
+00003080: 6173 6574 203d 2064 6174 6173 6574 732e  aset = datasets.
+00003090: 4461 7461 7365 7428 2e2e 2e29 0a20 2020  Dataset(...).   
+000030a0: 2020 2020 2020 2020 203e 3e3e 2064 6174           >>> dat
+000030b0: 6173 6574 2e75 706c 6f61 645f 6469 7265  aset.upload_dire
+000030c0: 6374 6f72 7928 0a20 2020 2020 2020 2020  ctory(.         
+000030d0: 2020 202e 2e2e 2020 2020 2070 6174 686c     ...     pathl
+000030e0: 6962 2e50 6174 6828 222f 7061 7468 2f74  ib.Path("/path/t
+000030f0: 6f2f 6469 7265 6374 6f72 7922 292c 0a20  o/directory"),. 
+00003100: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+00003110: 2020 2065 7863 6c75 6465 5f70 6174 7465     exclude_patte
+00003120: 726e 733d 5b0a 2020 2020 2020 2020 2020  rns=[.          
+00003130: 2020 2e2e 2e20 2020 2020 2020 2020 225f    ...         "_
+00003140: 5f70 7963 6163 6865 5f5f 2f22 2c0a 2020  _pycache__/",.  
+00003150: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00003160: 2020 2020 2020 222a 2e70 7963 222c 0a20        "*.pyc",. 
+00003170: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+00003180: 2020 2020 2020 2022 6e6f 6465 5f6d 6f64         "node_mod
+00003190: 756c 6573 2f22 2c0a 2020 2020 2020 2020  ules/",.        
+000031a0: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+000031b0: 222a 2a2f 2a2e 6c6f 6722 2c0a 2020 2020  "**/*.log",.    
+000031c0: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+000031d0: 5d2c 0a20 2020 2020 2020 2020 2020 202e  ],.            .
+000031e0: 2e2e 2029 0a20 2020 2020 2020 207a 1320  .. ).        z. 
+000031f0: 6973 206e 6f74 2061 2064 6972 6563 746f  is not a directo
+00003200: 7279 4e72 0100 0000 72a6 0000 0072 3800  ryNr....r....r8.
+00003210: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00003220: 0000 0004 0000 0013 0000 0073 4e00 0000  ...........sN...
+00003230: 7c00 a000 a100 4400 5d20 7d01 7c01 a001  |.....D.] }.|...
+00003240: a100 720f 8800 7c01 8301 0100 7104 8801  ..r...|.....q...
+00003250: 6400 7501 7219 8801 a002 7c01 a101 7219  d.u.r.....|...r.
+00003260: 7104 8802 6401 3700 8902 8803 7c01 a003  q...d.7.....|...
+00003270: a100 6a04 3700 8903 7104 6400 5300 2902  ..j.7...q.d.S.).
+00003280: 4e72 1700 0000 2905 da07 6974 6572 6469  Nr....)...iterdi
+00003290: 7272 8700 0000 da0a 6d61 7463 685f 6669  rr......match_fi
+000032a0: 6c65 da04 7374 6174 da07 7374 5f73 697a  le..stat..st_siz
+000032b0: 6529 0272 a600 0000 da04 7061 7468 2904  e).r......path).
+000032c0: da10 5f63 6f75 6e74 5f72 6573 6f75 7263  .._count_resourc
+000032d0: 6573 da0c 6578 636c 7564 655f 7370 6563  es..exclude_spec
+000032e0: da13 6578 7065 6374 6564 5f66 696c 655f  ..expected_file_
+000032f0: 636f 756e 74da 1265 7870 6563 7465 645f  count..expected_
+00003300: 6669 6c65 5f73 697a 6572 2600 0000 7227  file_sizer&...r'
+00003310: 0000 0072 ac00 0000 e201 0000 7310 0000  ...r........s...
+00003320: 000c 0308 010a 0112 0202 0108 0110 0104  ................
+00003330: f97a 3244 6174 6173 6574 2e75 706c 6f61  .z2Dataset.uploa
+00003340: 645f 6469 7265 6374 6f72 792e 3c6c 6f63  d_directory.<loc
+00003350: 616c 733e 2e5f 636f 756e 745f 7265 736f  als>._count_reso
+00003360: 7572 6365 737a 124e 6f20 6669 6c65 7320  urcesz.No files 
+00003370: 746f 2075 706c 6f61 64a9 0172 ae00 0000  to upload..r....
+00003380: a901 7220 0000 0063 0000 0000 0000 0000  ..r ...c........
+00003390: 0000 0000 0000 0000 0500 0000 1300 0000  ................
+000033a0: 7318 0000 0088 006a 0074 016a 0264 0188  s......j.t.j.d..
+000033b0: 016a 0364 028d 03a0 04a1 0053 0029 034e  .j.d.......S.).N
+000033c0: 5429 0272 9200 0000 7220 0000 0029 0572  T).r....r ...).r
+000033d0: 7000 0000 7203 0000 0072 9300 0000 7220  p...r....r....r 
+000033e0: 0000 0072 7200 0000 7226 0000 0029 0272  ...rr...r&...).r
+000033f0: 5500 0000 da0b 7472 616e 7361 6374 696f  U.....transactio
+00003400: 6e72 2600 0000 7227 0000 0072 7300 0000  nr&...r'...rs...
+00003410: fa01 0000 730e 0000 0004 0104 0102 0104  ....s...........
+00003420: 0104 fd04 0402 fc7a 3644 6174 6173 6574  .......z6Dataset
+00003430: 2e75 706c 6f61 645f 6469 7265 6374 6f72  .upload_director
+00003440: 792e 3c6c 6f63 616c 733e 2e5f 6372 6564  y.<locals>._cred
+00003450: 656e 7469 616c 5f70 726f 7669 6465 72da  ential_provider.
+00003460: 0a69 6e6e 6572 5f70 6174 68da 0a6b 6579  .inner_path..key
+00003470: 5f70 7265 6669 7863 0200 0000 0000 0000  _prefixc........
+00003480: 0000 0000 0400 0000 0700 0000 3300 0000  ............3...
+00003490: 737a 0000 0081 007c 00a0 00a1 0044 005d  sz.....|.....D.]
+000034a0: 357d 027c 02a0 01a1 0072 1a88 007c 027c  5}.|.....r...|.|
+000034b0: 019b 0064 017c 026a 029b 009d 0383 0245  ...d.|.j.......E
+000034c0: 0064 0048 0001 0071 0588 0264 0075 0172  .d.H...q...d.u.r
+000034d0: 2488 02a0 037c 02a1 0172 2471 057c 019b  $....|...r$q.|..
+000034e0: 0064 017c 026a 029b 009d 037d 037c 0288  .d.|.j.....}.|..
+000034f0: 016a 049b 0064 017c 03a0 0564 01a1 019b  .j...d.|...d....
+00003500: 009d 0366 0256 0001 0071 0564 0053 0029  ...f.V...q.d.S.)
+00003510: 024e da01 2f29 0672 a700 0000 7287 0000  .N../).r....r...
+00003520: 00da 046e 616d 6572 a800 0000 da0f 7265  ...namer......re
+00003530: 7175 6972 6564 5f70 7265 6669 78da 066c  quired_prefix..l
+00003540: 7374 7269 7029 0472 b300 0000 72b4 0000  strip).r....r...
+00003550: 0072 ab00 0000 721f 0000 0029 03da 115f  .r....r....)..._
+00003560: 7570 6c6f 6164 5f64 6972 6563 746f 7279  upload_directory
+00003570: da0b 6372 6564 656e 7469 616c 7372 ad00  ..credentialsr..
+00003580: 0000 7226 0000 0072 2700 0000 72b9 0000  ..r&...r'...r...
+00003590: 0001 0200 0073 1200 0000 0280 0c03 0801  .....s..........
+000035a0: 1e01 1202 0201 1002 1e01 04f8 7a33 4461  ............z3Da
+000035b0: 7461 7365 742e 7570 6c6f 6164 5f64 6972  taset.upload_dir
+000035c0: 6563 746f 7279 2e3c 6c6f 6361 6c73 3e2e  ectory.<locals>.
+000035d0: 5f75 706c 6f61 645f 6469 7265 6374 6f72  _upload_director
+000035e0: 79da 0072 1700 0000 2903 727b 0000 0072  y..r....).r{...r
+000035f0: ae00 0000 72af 0000 0072 7c00 0000 727f  ....r....r|...r.
+00003600: 0000 0029 0672 1e00 0000 7280 0000 0072  ...).r....r....r
+00003610: 8100 0000 7236 0000 0072 8200 0000 7283  ....r6...r....r.
+00003620: 0000 0029 0172 5d00 0000 2922 7287 0000  ...).r]...)"r...
+00003630: 0072 4a00 0000 da08 7061 7468 7370 6563  .rJ.....pathspec
+00003640: da0d 4769 7449 676e 6f72 6553 7065 63da  ..GitIgnoreSpec.
+00003650: 0a66 726f 6d5f 6c69 6e65 7372 8a00 0000  .from_linesr....
+00003660: 728b 0000 00da 066c 6f67 6765 72da 0469  r......logger..i
+00003670: 6e66 6fda 1b5f 4461 7461 7365 745f 5f73  nfo.._Dataset__s
+00003680: 7461 7274 5f74 7261 6e73 6163 7469 6f6e  tart_transaction
+00003690: 7270 0000 0072 0300 0000 7293 0000 0072  rp...r....r....r
+000036a0: 2000 0000 7224 0000 00da 0b63 6f6c 6c65   ...r$.....colle
+000036b0: 6374 696f 6e73 da03 6162 63da 0947 656e  ctions..abc..Gen
+000036c0: 6572 6174 6f72 7289 0000 0072 2a00 0000  eratorr....r*...
+000036d0: 5a0c 7570 6c6f 6164 5f66 696c 6573 721e  Z.upload_filesr.
+000036e0: 0000 0072 1400 0000 da09 4461 7461 7365  ...r......Datase
+000036f0: 7449 6472 2b00 0000 723d 0000 00da 054f  tIdr+...r=.....O
+00003700: 7267 4964 7233 0000 00da 0c43 6f6d 6d6f  rgIdr3.....Commo
+00003710: 6e50 7265 6669 7872 b700 0000 da0d 5472  nPrefixr......Tr
+00003720: 616e 7361 6374 696f 6e49 6472 1600 0000  ansactionIdr....
+00003730: da08 6162 736f 6c75 7465 7263 0000 0029  ..absoluterc...)
+00003740: 0572 5500 0000 72a6 0000 0072 6800 0000  .rU...r....rh...
+00003750: 725d 0000 0072 7300 0000 7226 0000 0029  r]...rs...r&...)
+00003760: 0872 ac00 0000 72b9 0000 0072 ba00 0000  .r....r....r....
+00003770: 72ad 0000 0072 ae00 0000 72af 0000 0072  r....r....r....r
+00003780: 5500 0000 72b2 0000 0072 2700 0000 da10  U...r....r'.....
+00003790: 7570 6c6f 6164 5f64 6972 6563 746f 7279  upload_directory
+000037a0: bd01 0000 735a 0000 0008 190e 0104 0208  ....sZ..........
+000037b0: 0106 0102 0104 ff04 0404 011e 0208 0c08  ................
+000037c0: 020a 0104 010c 0204 0208 0106 ff0e 0402  ................
+000037d0: 0704 0102 ff02 0102 ff1a 0212 fe06 0d04  ................
+000037e0: 0108 0102 010a 020a 0108 0108 0102 fc02  ................
+000037f0: 0602 010a 0202 0102 0104 fd04 fe02 0806  ................
+00003800: ee14 157a 1844 6174 6173 6574 2e75 706c  ...z.Dataset.upl
+00003810: 6f61 645f 6469 7265 6374 6f72 79da 0f6c  oad_directory..l
+00003820: 6f63 616c 5f66 696c 655f 7061 7468 721f  ocal_file_pathr.
+00003830: 0000 0072 ba00 0000 7281 0000 0063 0500  ...r....r....c..
+00003840: 0000 0000 0000 0000 0000 0700 0000 0700  ................
+00003850: 0000 4300 0000 7330 0000 007c 006a 0064  ..C...s0...|.j.d
+00003860: 0164 028d 017d 057c 00a0 017c 017c 027c  .d...}.|...|.|.|
+00003870: 056a 027c 037c 04a1 057d 067c 00a0 037c  .j.|.|...}.|...|
+00003880: 056a 02a1 0101 007c 0653 0029 037a 4a0a  .j.....|.S.).zJ.
+00003890: 2020 2020 2020 2020 5570 6c6f 6164 7320          Uploads 
+000038a0: 6120 7369 6e67 6c65 2066 696c 6520 746f  a single file to
+000038b0: 2074 6865 2064 6174 6173 6574 2773 2073   the dataset's s
+000038c0: 746f 7261 6765 206c 6f63 6174 696f 6e2e  torage location.
+000038d0: 0a20 2020 2020 2020 2072 1700 0000 72b0  .        r....r.
+000038e0: 0000 0029 0472 c100 0000 da15 5f44 6174  ...).r......_Dat
+000038f0: 6173 6574 5f5f 7570 6c6f 6164 5f66 696c  aset__upload_fil
+00003900: 6572 2000 0000 7263 0000 0029 0772 5500  er ...rc...).rU.
+00003910: 0000 72cb 0000 0072 1f00 0000 72ba 0000  ..r....r....r...
+00003920: 0072 8100 0000 72b2 0000 005a 0b75 706c  .r....r....Z.upl
+00003930: 6f61 645f 696e 666f 7226 0000 0072 2600  oad_infor&...r&.
+00003940: 0000 7227 0000 00da 0b75 706c 6f61 645f  ..r'.....upload_
+00003950: 6669 6c65 2502 0000 7314 0000 000c 0a04  file%...s.......
+00003960: 0202 0102 0104 0102 0102 0104 fb0c 0804  ................
+00003970: 027a 1344 6174 6173 6574 2e75 706c 6f61  .z.Dataset.uploa
+00003980: 645f 6669 6c65 7299 0000 00da 0a63 6f6e  d_filer......con
+00003990: 6469 7469 6f6e 7363 0500 0000 0000 0000  ditionsc........
+000039a0: 0000 0000 0600 0000 0700 0000 4300 0000  ............C...
+000039b0: 7322 0000 007c 006a 006a 017c 006a 027c  s"...|.j.j.|.j.|
+000039c0: 017c 027c 037c 0464 018d 057d 057c 057c  .|.|.|.d...}.|.|
+000039d0: 005f 0264 0053 0029 024e 2904 7299 0000  ._.d.S.).N).r...
+000039e0: 0072 ce00 0000 7237 0000 0072 9500 0000  .r....r7...r....
+000039f0: 2903 7229 0000 0072 9b00 0000 722b 0000  ).r)...r....r+..
+00003a00: 0029 0672 5500 0000 7299 0000 0072 ce00  .).rU...r....r..
+00003a10: 0000 7237 0000 0072 9500 0000 da07 7570  ..r7...r......up
+00003a20: 6461 7465 6472 2600 0000 7226 0000 0072  datedr&...r&...r
+00003a30: 2700 0000 729b 0000 003d 0200 0073 1000  '...r....=...s..
+00003a40: 0000 0607 0401 0201 0201 0201 0201 06fb  ................
+00003a50: 0a07 7a0e 4461 7461 7365 742e 7570 6461  ..z.Dataset.upda
+00003a60: 7465 72ae 0000 0063 0200 0000 0000 0000  ter....c........
+00003a70: 0000 0000 0400 0000 0700 0000 4300 0000  ............C...
+00003a80: 7342 0000 0074 006a 01a0 0264 01a1 017d  sB...t.j...d...}
+00003a90: 0274 03a0 0474 056a 066a 0764 027c 029b  .t...t.j.j.d.|..
+00003aa0: 009d 02a1 027d 037c 006a 086a 0974 0a6a  .....}.|.j.j.t.j
+00003ab0: 0b7c 037c 017c 006a 0c6a 0d7c 006a 0c6a  .|.|.|.j.j.|.j.j
+00003ac0: 0d64 038d 0553 0029 044e da06 726f 626f  .d...S.).N..robo
+00003ad0: 746f 7a07 726f 626f 746f 2029 055a 1074  toz.roboto ).Z.t
+00003ae0: 7261 6e73 6163 7469 6f6e 5f74 7970 65da  ransaction_type.
+00003af0: 0b6f 7269 6769 6e61 7469 6f6e 5a17 6578  .originationZ.ex
+00003b00: 7065 6374 6564 5f72 6573 6f75 7263 655f  pected_resource_
+00003b10: 636f 756e 7472 3300 0000 da11 7265 736f  countr3.....reso
+00003b20: 7572 6365 5f6f 776e 6572 5f69 6429 0eda  urce_owner_id)..
+00003b30: 0969 6d70 6f72 746c 6962 7235 0000 00da  .importlibr5....
+00003b40: 0776 6572 7369 6f6e da02 6f73 da06 6765  .version..os..ge
+00003b50: 7465 6e76 7210 0000 00da 0952 6f62 6f74  tenvr......Robot
+00003b60: 6f45 6e76 da05 7661 6c75 6572 2d00 0000  oEnv..valuer-...
+00003b70: 5a11 6265 6769 6e5f 7472 616e 7361 6374  Z.begin_transact
+00003b80: 696f 6e72 0b00 0000 5a0a 4669 6c65 5570  ionr....Z.FileUp
+00003b90: 6c6f 6164 722b 0000 0072 3300 0000 2904  loadr+...r3...).
+00003ba0: 7255 0000 0072 ae00 0000 5a0f 7061 636b  rU...r....Z.pack
+00003bb0: 6167 655f 7665 7273 696f 6e72 d100 0000  age_versionr....
+00003bc0: 7226 0000 0072 2600 0000 7227 0000 005a  r&...r&...r'...Z
+00003bd0: 135f 5f73 7461 7274 5f74 7261 6e73 6163  .__start_transac
+00003be0: 7469 6f6e 4d02 0000 7316 0000 000c 0404  tionM...s.......
+00003bf0: 010e 0104 ff06 0304 0102 0102 0106 0106  ................
+00003c00: 0106 fb7a 1b44 6174 6173 6574 2e5f 5f73  ...z.Dataset.__s
+00003c10: 7461 7274 5f74 7261 6e73 6163 7469 6f6e  tart_transaction
+00003c20: 6306 0000 0000 0000 0000 0000 0007 0000  c...............
+00003c30: 000d 0000 0003 0000 0073 d800 0000 7c01  .........s....|.
+00003c40: a000 a100 730b 7401 7c01 9b00 6401 9d02  ....s.t.|...d...
+00003c50: 8301 8201 8800 6a02 6a03 7404 6a05 6b03  ......j.j.t.j.k.
+00003c60: 7319 8800 6a02 6a06 7407 6a08 6b03 721d  s...j.j.t.j.k.r.
+00003c70: 7409 6402 8301 8201 7c04 6403 7501 7223  t.d.....|.d.u.r#
+00003c80: 7c04 6e07 8800 6a0a 740b 6a0c 8801 6404  |.n...j.t.j...d.
+00003c90: 8d02 7d04 7c05 6403 7500 7238 8700 8701  ..}.|.d.u.r8....
+00003ca0: 6602 6405 6406 8408 7d06 7c06 7d05 7c04  f.d.d...}.|.}.|.
+00003cb0: 6a0d 9b00 6407 7c02 a00e 6407 a101 9b00  j...d.|...d.....
+00003cc0: 9d03 7d02 8800 6a0f 6a10 7c01 7c04 6a11  ..}...j.j.|.|.j.
+00003cd0: 7c02 7c05 7412 6a13 8800 6a02 6a14 7412  |.|.t.j...j.j.t.
+00003ce0: 6a15 8800 6a02 6a16 7412 6a17 7c04 6a0d  j...j.j.t.j.|.j.
+00003cf0: 7412 6a18 8801 6904 7419 6408 6409 8d01  t.j...i.t.d.d...
+00003d00: 640a 8d06 0100 741a 7c04 6a11 7c02 8801  d.....t.|.j.|...
+00003d10: 640b 8d03 5300 290c 7a69 0a20 2020 2020  d...S.).zi.     
+00003d20: 2020 2055 706c 6f61 6473 2061 2066 696c     Uploads a fil
+00003d30: 6520 746f 2074 6865 2064 6174 6173 6574  e to the dataset
+00003d40: 2773 2073 746f 7261 6765 206c 6f63 6174  's storage locat
+00003d50: 696f 6e2e 2044 6f65 7320 6e6f 7420 6d61  ion. Does not ma
+00003d60: 726b 2074 6865 2075 706c 6f61 6420 6173  rk the upload as
+00003d70: 2063 6f6d 706c 6574 652e 0a20 2020 2020   complete..     
+00003d80: 2020 207a 0e20 6973 206e 6f74 2061 2066     z. is not a f
+00003d90: 696c 6572 6e00 0000 4e72 b100 0000 6300  ilern...Nr....c.
+00003da0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00003db0: 0000 0013 0000 0073 1400 0000 8800 6a00  .......s......j.
+00003dc0: 7401 6a02 8801 6401 8d02 a003 a100 5300  t.j...d.......S.
+00003dd0: 2902 4e72 b100 0000 2904 7270 0000 0072  ).Nr....).rp...r
+00003de0: 0300 0000 7293 0000 0072 7200 0000 7226  ....r....rr...r&
+00003df0: 0000 00a9 0272 5500 0000 7220 0000 0072  .....rU...r ...r
+00003e00: 2600 0000 7227 0000 0072 7300 0000 7d02  &...r'...rs...}.
+00003e10: 0000 730a 0000 0004 0106 0104 ff04 0202  ..s.............
+00003e20: fe7a 3344 6174 6173 6574 2e5f 5f75 706c  .z3Dataset.__upl
+00003e30: 6f61 645f 6669 6c65 2e3c 6c6f 6361 6c73  oad_file.<locals
+00003e40: 3e2e 5f63 7265 6465 6e74 6961 6c5f 7072  >._credential_pr
+00003e50: 6f76 6964 6572 72b5 0000 0072 1700 0000  oviderr....r....
+00003e60: 2901 727d 0000 0029 0272 3600 0000 7282  ).r}...).r6...r.
+00003e70: 0000 0029 0372 1e00 0000 721f 0000 0072  ...).r....r....r
+00003e80: 2000 0000 291b da07 6973 5f66 696c 6572   ...)...is_filer
+00003e90: 4a00 0000 722b 0000 0072 3200 0000 721a  J...r+...r2...r.
+00003ea0: 0000 0072 8400 0000 7231 0000 0072 1b00  ...r....r1...r..
+00003eb0: 0000 7285 0000 0072 8600 0000 7270 0000  ..r....r....rp..
+00003ec0: 0072 0300 0000 7293 0000 0072 b700 0000  .r....r....r....
+00003ed0: 72b8 0000 0072 2a00 0000 72cd 0000 0072  r....r*...r....r
+00003ee0: 1e00 0000 7214 0000 0072 c500 0000 723d  ....r....r....r=
+00003ef0: 0000 0072 c600 0000 7233 0000 0072 c700  ...r....r3...r..
+00003f00: 0000 72c8 0000 0072 1600 0000 721d 0000  ..r....r....r...
+00003f10: 0029 0772 5500 0000 72cb 0000 0072 1f00  .).rU...r....r..
+00003f20: 0000 7220 0000 0072 ba00 0000 7281 0000  ..r ...r....r...
+00003f30: 0072 7300 0000 7226 0000 0072 d900 0000  .rs...r&...r....
+00003f40: 7227 0000 005a 0d5f 5f75 706c 6f61 645f  r'...Z.__upload_
+00003f50: 6669 6c65 5d02 0000 7344 0000 0008 0b0e  file]...sD......
+00003f60: 010e 030e 0102 0202 0104 ff08 0604 ff04  ................
+00003f70: 0206 0104 ff02 fd08 080e 0204 0516 0206  ................
+00003f80: 0102 0104 0102 0102 010a 020a 0108 0106  ................
+00003f90: 0102 fc08 0606 f502 0e04 0102 0102 0106  ................
+00003fa0: fd7a 1544 6174 6173 6574 2e5f 5f75 706c  .z.Dataset.__upl
+00003fb0: 6f61 645f 6669 6c65 7239 0000 0029 024e  oad_filer9...).N
+00003fc0: 725b 0000 0029 0272 3800 0000 4e29 024e  r[...).r8...N).N
+00003fd0: 4e29 044e 4e4e 4e29 4372 2100 0000 7222  N).NNNN)Cr!...r"
+00003fe0: 0000 0072 2300 0000 7219 0000 0072 2500  ...r#...r....r%.
+00003ff0: 0000 7212 0000 0072 1c00 0000 722c 0000  ..r....r....r,..
+00004000: 00da 0674 7970 696e 67da 084f 7074 696f  ...typing..Optio
+00004010: 6e61 6c72 1800 0000 7209 0000 00da 0b63  nalr....r......c
+00004020: 6c61 7373 6d65 7468 6f64 721b 0000 0072  lassmethodr....r
+00004030: 8500 0000 721a 0000 0072 8400 0000 7224  ....r....r....r$
+00004040: 0000 00da 0464 6963 74da 0341 6e79 728c  .....dict..Anyr.
+00004050: 0000 0072 3c00 0000 723f 0000 0072 0700  ...r<...r?...r..
+00004060: 0000 72c2 0000 0072 c300 0000 72c4 0000  ..r....r....r...
+00004070: 0072 4000 0000 7256 0000 00da 0870 726f  .r@...rV.....pro
+00004080: 7065 7274 7972 3d00 0000 7235 0000 0072  pertyr=...r5...r
+00004090: 3b00 0000 7236 0000 00da 0369 6e74 7263  ;...r6.....intrc
+000040a0: 0000 0072 6600 0000 726c 0000 0072 8a00  ...rf...rl...r..
+000040b0: 0000 728b 0000 0072 8d00 0000 da05 556e  ..r....r......Un
+000040c0: 696f 6e72 1100 0000 7290 0000 0072 0300  ionr....r....r..
+000040d0: 0000 7271 0000 00da 0462 6f6f 6c72 7000  ..rq.....boolrp.
+000040e0: 0000 7269 0000 0072 9d00 0000 720d 0000  ..ri...r....r...
+000040f0: 0072 9e00 0000 72a1 0000 0072 a300 0000  .r....r....r....
+00004100: 72a4 0000 0072 a500 0000 72ca 0000 00da  r....r....r.....
+00004110: 0843 616c 6c61 626c 6572 1500 0000 721d  .Callabler....r.
+00004120: 0000 0072 cd00 0000 720c 0000 0072 0e00  ...r....r....r..
+00004130: 0000 729b 0000 0072 0a00 0000 72c1 0000  ..r....r....r...
+00004140: 0072 cc00 0000 7226 0000 0072 2600 0000  .r....r&...r&...
+00004150: 7226 0000 0072 2700 0000 7228 0000 0039  r&...r'...r(...9
+00004160: 0000 0073 da01 0000 0a00 0801 0801 0801  ...s............
+00004170: 1201 0801 0202 0406 0401 0201 0201 0201  ................
+00004180: 0201 0201 04f5 0202 02fe 0203 02fd 0204  ................
+00004190: 02fc 0205 02fb 0206 02fa 0807 02f9 0808  ................
+000041a0: 02f8 1209 02f7 0c0a 02f6 080b 02f5 020c  ................
+000041b0: 0cf4 0218 0201 0202 02fe 0203 02fd 0204  ................
+000041c0: 02fc 0205 02fb 0206 0cfa 020a 0207 04fa  ................
+000041d0: 0202 02fe 0203 02fd 0204 02fc 0205 02fb  ................
+000041e0: 0806 02fa 0a07 0cf9 0227 0202 02fe 0203  .........'......
+000041f0: 02fd 0204 02fc 0205 02fb 0206 0afa 020c  ................
+00004200: 1001 0203 1a01 0203 1001 0203 1401 0206  ................
+00004210: 0201 04fc 0202 02fe 0803 02fd 0204 02fc  ................
+00004220: 0205 0afb 0a1f 0205 0201 04fd 0c02 02fe  ................
+00004230: 0c03 02fd 0204 0afc 021a 0201 04fc 0402  ................
+00004240: 02fe 0c03 02fd 0c04 02fc 0205 0afb 023f  ...............?
+00004250: 0e02 02fe 0203 0afd 041d 0201 0201 0201  ................
+00004260: 04fb 0202 02fe 0803 02fd 0204 02fc 0805  ................
+00004270: 02fb 0206 0afa 0214 0201 04fd 0c02 02fe  ................
+00004280: 0c03 02fd 1004 0afc 022a 04fd 0c02 02fe  .........*......
+00004290: 0803 02fd 0204 0afc 021a 04fd 0202 02fe  ................
+000042a0: 0803 02fd 0204 0afc 0a0b 0209 04fd 0202  ................
+000042b0: 02fe 0803 02fd 0204 0afc 0216 04fd 0202  ................
+000042c0: 02fe 0803 02fd 0204 0afc 180b 0206 0201  ................
+000042d0: 04fc 0402 02fe 0c03 02fd 0204 02fc 0205  ................
+000042e0: 0afb 026c 0201 04fb 0402 02fe 0203 02fd  ...l............
+000042f0: 0804 02fc 1205 02fb 0206 0afa 021a 0201  ................
+00004300: 0201 0201 04fb 0802 02fe 0c03 02fd 0804  ................
+00004310: 02fc 0805 02fb 0206 0afa 0210 0202 02fe  ................
+00004320: 0203 0afd 0215 0201 04fa 0402 02fe 0203  ................
+00004330: 02fd 0204 02fc 0805 02fb 1206 02fa 0207  ................
+00004340: 0ef9 7228 0000 0029 32da 0f63 6f6c 6c65  ..r(...)2..colle
+00004350: 6374 696f 6e73 2e61 6263 72c2 0000 00da  ctions.abcr.....
+00004360: 0b64 6174 6163 6c61 7373 6573 da12 696d  .dataclasses..im
+00004370: 706f 7274 6c69 622e 6d65 7461 6461 7461  portlib.metadata
+00004380: 72d3 0000 0072 d500 0000 728a 0000 0072  r....r....r....r
+00004390: 5f00 0000 72db 0000 0072 bc00 0000 da04  _...r....r......
+000043a0: 6175 7468 7203 0000 00da 0a65 7863 6570  authr......excep
+000043b0: 7469 6f6e 7372 0400 0000 7205 0000 00da  tionsr....r.....
+000043c0: 076c 6f67 6769 6e67 7206 0000 0072 4000  .loggingr....r@.
+000043d0: 0000 7207 0000 00da 0573 6572 6465 7208  ..r......serder.
+000043e0: 0000 00da 0c74 7261 6e73 6163 7469 6f6e  .....transaction
+000043f0: 7372 0900 0000 720a 0000 0072 0b00 0000  sr....r....r....
+00004400: da07 7570 6461 7465 7372 0c00 0000 720d  ..updatesr....r.
+00004410: 0000 0072 0e00 0000 da07 6163 7469 6f6e  ...r......action
+00004420: 7372 1000 0000 da05 6669 6c65 7372 1100  sr......filesr..
+00004430: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00004440: 0072 1500 0000 5a0e 6669 6c65 732e 7072  .r....Z.files.pr
+00004450: 6f67 7265 7373 7216 0000 00da 0864 656c  ogressr......del
+00004460: 6567 6174 6572 1800 0000 7219 0000 0072  egater....r....r
+00004470: 1a00 0000 723b 0000 0072 1b00 0000 721c  ....r;...r....r.
+00004480: 0000 0072 bf00 0000 da09 6461 7461 636c  ...r......datacl
+00004490: 6173 7372 1d00 0000 7228 0000 0072 2600  assr....r(...r&.
+000044a0: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
+000044b0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000044c0: 3000 0000 0800 0801 0801 0801 0801 0801  0...............
+000044d0: 0801 0802 0c02 1001 0c04 0c01 0c01 1401  ................
+000044e0: 1405 0c05 1c01 0c07 1403 1005 0602 0403  ................
+000044f0: 1001 1206                                ....
```

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/__pycache__/delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/datasets/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3479 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 970d 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 160d 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a05 6403 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6403 6405 6c08 6d09 5a09 0100 6403  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6403 6407 6c0c  d.l.m.Z...d.d.l.
@@ -47,15 +47,15 @@
 000002e0: 6564 5f70 7265 6669 78da 0672 6574 7572  ed_prefix..retur
 000002f0: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
 00000300: 0000 0200 0000 4300 0000 730c 0000 0074  ......C...s....t
 00000310: 0083 007c 006a 016b 0553 00a9 014e 2902  ...|.j.k.S...N).
 00000320: 720a 0000 0072 1700 0000 a901 da04 7365  r....r........se
 00000330: 6c66 a900 7220 0000 00fa e82f 636f 6465  lf..r ...../code
 00000340: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000350: 3130 3531 3138 3230 3839 2f73 7263 2f63  1051182089/src/c
+00000350: 3330 3739 3233 3632 3634 2f73 7263 2f63  3079236264/src/c
 00000360: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 00000370: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 00000380: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 00000390: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 000003a0: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 000003b0: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 000003c0: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
@@ -98,169 +98,165 @@
 00000610: 7222 0000 00da 0464 6963 7472 0200 0000  r".....dictr....
 00000620: 7225 0000 0072 0f00 0000 722b 0000 0072  r%...r....r+...r
 00000630: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
 00000640: 0000 0072 1400 0000 1800 0000 7316 0000  ...r........s...
 00000650: 000a 0008 0108 010a 0108 0108 0108 0108  ................
 00000660: 010e 0216 0312 0372 1400 0000 6300 0000  .......r....c...
 00000670: 0000 0000 0000 0000 0000 0000 0012 0000  ................
-00000680: 0040 0000 0073 c201 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000690: 5a02 6503 6a04 0901 6426 6402 6505 6403  Z.e.j...d&d.e.d.
-000006a0: 6505 6404 6506 6505 1900 6405 6401 6608  e.d.e.e...d.d.f.
-000006b0: 6406 6407 8405 8301 5a07 6503 6a04 6508  d.d.....Z.e.j.e.
-000006c0: 6a09 6401 650a 6a0b 6401 6401 6401 6401  j.d.e.j.d.d.d.d.
-000006d0: 6607 6408 6508 6409 6506 650c 6505 650d  f.d.e.d.e.e.e.e.
-000006e0: 6602 1900 1900 640a 650a 640b 6506 650e  f.....d.e.d.e.e.
-000006f0: 6505 1900 1900 6404 6506 6505 1900 640c  e.....d.e.e...d.
-00000700: 6506 6505 1900 640d 6506 6505 1900 6405  e.e...d.e.e...d.
-00000710: 650f 6610 640e 640f 8405 8301 5a10 6503  e.f.d.d.....Z.e.
-00000720: 6a04 6410 650f 6405 6401 6604 6411 6412  j.d.e.d.d.f.d.d.
-00000730: 8404 8301 5a11 6503 6a04 0901 6426 6402  ....Z.e.j...d&d.
-00000740: 6505 6404 6506 6505 1900 6405 650f 6606  e.d.e.e...d.e.f.
-00000750: 6413 6414 8405 8301 5a12 6503 6a04 0901  d.d.....Z.e.j...
-00000760: 0901 6427 6410 650f 6415 6513 6416 6506  ..d'd.e.d.e.d.e.
-00000770: 6505 1900 6403 6506 6505 1900 6405 6514  e...d.e.e...d.e.
-00000780: 660a 6417 6418 8405 8301 5a15 6503 6a04  f.d.d.....Z.e.j.
-00000790: 0901 0901 0901 0901 6428 6402 6505 6404  ........d(d.e.d.
-000007a0: 6506 6505 1900 6419 6506 6505 1900 641a  e.e...d.e.e...d.
-000007b0: 6506 650e 6505 1900 1900 641b 6506 650e  e.e.e.....d.e.e.
-000007c0: 6505 1900 1900 6405 6516 6517 1900 660c  e.....d.e.e...f.
-000007d0: 641c 641d 8405 8301 5a18 6503 6a04 0901  d.d.....Z.e.j...
-000007e0: 6426 641e 6519 6404 6506 6505 1900 6405  d&d.e.d.e.e...d.
-000007f0: 6516 650f 1900 6606 641f 6420 8405 8301  e.e...f.d.d ....
-00000800: 5a1a 6503 6a04 0901 0901 0901 0901 6428  Z.e.j.........d(
-00000810: 6410 650f 6421 6506 651b 1900 6422 6506  d.e.d!e.e...d"e.
-00000820: 650e 651c 1900 1900 640d 6506 6505 1900  e.e.....d.e.e...
-00000830: 6423 6506 6505 1900 6405 650f 660c 6424  d#e.e...d.e.f.d$
-00000840: 6425 8405 8301 5a1d 6401 5300 2929 da0f  d%....Z.d.S.))..
-00000850: 4461 7461 7365 7444 656c 6567 6174 654e  DatasetDelegateN
-00000860: da0a 6461 7461 7365 745f 6964 da0e 7472  ..dataset_id..tr
-00000870: 616e 7361 6374 696f 6e5f 6964 da06 6f72  ansaction_id..or
-00000880: 675f 6964 721c 0000 0063 0400 0000 0000  g_idr....c......
-00000890: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
-000008a0: 0000 f308 0000 0074 0064 0183 0182 0129  .......t.d.....)
-000008b0: 024e da0f 636f 6d70 6c65 7465 5f75 706c  .N..complete_upl
-000008c0: 6f61 64a9 01da 134e 6f74 496d 706c 656d  oad....NotImplem
-000008d0: 656e 7465 6445 7272 6f72 2904 721f 0000  entedError).r...
-000008e0: 0072 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
-000008f0: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
-00000900: 3900 0000 3200 0000 7302 0000 0008 047a  9...2...s......z
-00000910: 1f44 6174 6173 6574 4465 6c65 6761 7465  .DatasetDelegate
-00000920: 2e63 6f6d 706c 6574 655f 7570 6c6f 6164  .complete_upload
-00000930: da0d 6164 6d69 6e69 7374 7261 746f 72da  ..administrator.
-00000940: 086d 6574 6164 6174 61da 1073 746f 7261  .metadata..stora
-00000950: 6765 5f6c 6f63 6174 696f 6eda 0474 6167  ge_location..tag
-00000960: 73da 0a63 7265 6174 6564 5f62 79da 0b64  s..created_by..d
-00000970: 6573 6372 6970 7469 6f6e 6308 0000 0000  escriptionc.....
-00000980: 0000 0000 0000 0008 0000 0002 0000 0043  ...............C
-00000990: 0000 0072 3800 0000 2902 4eda 0e63 7265  ...r8...).N..cre
-000009a0: 6174 655f 6461 7461 7365 7472 3a00 0000  ate_datasetr:...
-000009b0: 2908 721f 0000 0072 3c00 0000 723d 0000  ).r....r<...r=..
-000009c0: 0072 3e00 0000 723f 0000 0072 3700 0000  .r>...r?...r7...
-000009d0: 7240 0000 0072 4100 0000 7220 0000 0072  r@...rA...r ...r
-000009e0: 2000 0000 7221 0000 0072 4200 0000 3800   ...r!...rB...8.
-000009f0: 0000 7302 0000 0008 0b7a 1e44 6174 6173  ..s......z.Datas
-00000a00: 6574 4465 6c65 6761 7465 2e63 7265 6174  etDelegate.creat
-00000a10: 655f 6461 7461 7365 74da 0672 6563 6f72  e_dataset..recor
-00000a20: 6463 0200 0000 0000 0000 0000 0000 0200  dc..............
-00000a30: 0000 0200 0000 4300 0000 7238 0000 0029  ......C...r8...)
-00000a40: 024e da0e 6465 6c65 7465 5f64 6174 6173  .N..delete_datas
-00000a50: 6574 723a 0000 0029 0272 1f00 0000 7243  etr:...).r....rC
-00000a60: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00000a70: 0000 7244 0000 0045 0000 0073 0200 0000  ..rD...E...s....
-00000a80: 0802 7a1e 4461 7461 7365 7444 656c 6567  ..z.DatasetDeleg
-00000a90: 6174 652e 6465 6c65 7465 5f64 6174 6173  ate.delete_datas
-00000aa0: 6574 6303 0000 0000 0000 0000 0000 0003  etc.............
-00000ab0: 0000 0002 0000 0043 0000 0072 3800 0000  .......C...r8...
-00000ac0: 2902 4eda 1a67 6574 5f64 6174 6173 6574  ).N..get_dataset
-00000ad0: 5f62 795f 7072 696d 6172 795f 6b65 7972  _by_primary_keyr
-00000ae0: 3a00 0000 2903 721f 0000 0072 3500 0000  :...).r....r5...
-00000af0: 7237 0000 0072 2000 0000 7220 0000 0072  r7...r ...r ...r
-00000b00: 2100 0000 7245 0000 0049 0000 00f3 0200  !...rE...I......
-00000b10: 0000 0806 7a2a 4461 7461 7365 7444 656c  ....z*DatasetDel
-00000b20: 6567 6174 652e 6765 745f 6461 7461 7365  egate.get_datase
-00000b30: 745f 6279 5f70 7269 6d61 7279 5f6b 6579  t_by_primary_key
-00000b40: da0b 7065 726d 6973 7369 6f6e 73da 0663  ..permissions..c
-00000b50: 616c 6c65 7263 0500 0000 0000 0000 0000  allerc..........
-00000b60: 0000 0500 0000 0200 0000 4300 0000 7238  ..........C...r8
-00000b70: 0000 0029 024e da19 6765 745f 7465 6d70  ...).N..get_temp
-00000b80: 6f72 6172 795f 6372 6564 656e 7469 616c  orary_credential
-00000b90: 7372 3a00 0000 2905 721f 0000 0072 4300  sr:...).r....rC.
-00000ba0: 0000 7247 0000 0072 4800 0000 7236 0000  ..rG...rH...r6..
-00000bb0: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
-00000bc0: 7249 0000 0051 0000 0073 0200 0000 0808  rI...Q...s......
-00000bd0: 7a29 4461 7461 7365 7444 656c 6567 6174  z)DatasetDelegat
-00000be0: 652e 6765 745f 7465 6d70 6f72 6172 795f  e.get_temporary_
-00000bf0: 6372 6564 656e 7469 616c 73da 0a70 6167  credentials..pag
-00000c00: 655f 746f 6b65 6eda 1069 6e63 6c75 6465  e_token..include
-00000c10: 5f70 6174 7465 726e 73da 1065 7863 6c75  _patterns..exclu
-00000c20: 6465 5f70 6174 7465 726e 7363 0600 0000  de_patternsc....
-00000c30: 0000 0000 0000 0000 0600 0000 0200 0000  ................
-00000c40: 4300 0000 7238 0000 0029 024e da0a 6c69  C...r8...).N..li
-00000c50: 7374 5f66 696c 6573 723a 0000 0029 0672  st_filesr:...).r
-00000c60: 1f00 0000 7235 0000 0072 3700 0000 724a  ....r5...r7...rJ
-00000c70: 0000 0072 4b00 0000 724c 0000 0072 2000  ...rK...rL...r .
-00000c80: 0000 7220 0000 0072 2100 0000 724d 0000  ..r ...r!...rM..
-00000c90: 005b 0000 00f3 0200 0000 0809 7a1a 4461  .[..........z.Da
-00000ca0: 7461 7365 7444 656c 6567 6174 652e 6c69  tasetDelegate.li
-00000cb0: 7374 5f66 696c 6573 da05 7175 6572 7963  st_files..queryc
-00000cc0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000cd0: 0200 0000 4300 0000 7238 0000 0029 024e  ....C...r8...).N
-00000ce0: da0e 7175 6572 795f 6461 7461 7365 7473  ..query_datasets
-00000cf0: 723a 0000 0029 0372 1f00 0000 724f 0000  r:...).r....rO..
-00000d00: 0072 3700 0000 7220 0000 0072 2000 0000  .r7...r ...r ...
-00000d10: 7221 0000 0072 5000 0000 6600 0000 7246  r!...rP...f...rF
-00000d20: 0000 007a 1e44 6174 6173 6574 4465 6c65  ...z.DatasetDele
-00000d30: 6761 7465 2e71 7565 7279 5f64 6174 6173  gate.query_datas
-00000d40: 6574 73da 126d 6574 6164 6174 615f 6368  ets..metadata_ch
-00000d50: 616e 6765 7365 74da 0a63 6f6e 6469 7469  angeset..conditi
-00000d60: 6f6e 73da 0a75 7064 6174 6564 5f62 7963  ons..updated_byc
-00000d70: 0600 0000 0000 0000 0000 0000 0600 0000  ................
-00000d80: 0200 0000 4300 0000 7238 0000 0029 024e  ....C...r8...).N
-00000d90: da06 7570 6461 7465 723a 0000 0029 0672  ..updater:...).r
-00000da0: 1f00 0000 7243 0000 0072 5100 0000 7252  ....rC...rQ...rR
-00000db0: 0000 0072 4100 0000 7253 0000 0072 2000  ...rA...rS...r .
-00000dc0: 0000 7220 0000 0072 2100 0000 7254 0000  ..r ...r!...rT..
-00000dd0: 006e 0000 0072 4e00 0000 7a16 4461 7461  .n...rN...z.Data
-00000de0: 7365 7444 656c 6567 6174 652e 7570 6461  setDelegate.upda
-00000df0: 7465 721d 0000 0029 024e 4e29 044e 4e4e  ter....).NN).NNN
-00000e00: 4e29 1e72 2c00 0000 722d 0000 0072 2e00  N).r,...r-...r..
-00000e10: 0000 da03 6162 63da 0e61 6273 7472 6163  ....abc..abstrac
-00000e20: 746d 6574 686f 6472 2f00 0000 7203 0000  tmethodr/...r...
-00000e30: 0072 3900 0000 7211 0000 00da 0652 6f62  .r9...r......Rob
-00000e40: 6f74 6f72 1300 0000 da02 5333 7233 0000  otor......S3r3..
-00000e50: 0072 0200 0000 da04 6c69 7374 7212 0000  .r......listr...
-00000e60: 0072 4200 0000 7244 0000 0072 4500 0000  .rB...rD...rE...
-00000e70: 7205 0000 0072 1400 0000 7249 0000 0072  r....r....rI...r
-00000e80: 0600 0000 720e 0000 0072 4d00 0000 7207  ....r....rM...r.
-00000e90: 0000 0072 5000 0000 720b 0000 0072 0c00  ...rP...r....r..
-00000ea0: 0000 7254 0000 0072 2000 0000 7220 0000  ..rT...r ...r ..
-00000eb0: 0072 2000 0000 7221 0000 0072 3400 0000  .r ...r!...r4...
-00000ec0: 3100 0000 73d6 0000 0008 0004 0102 0204  1...s...........
-00000ed0: ff02 0102 ff02 0102 ff06 0102 ff02 020c  ................
-00000ee0: fe04 0504 0302 0104 0102 0102 0102 0102  ................
-00000ef0: 0104 f802 0202 fe0e 0302 fd02 0402 fc0a  ................
-00000f00: 0502 fb06 0602 fa06 0702 f906 0802 f802  ................
-00000f10: 090c f704 0c14 0104 0302 0404 fd02 0202  ................
-00000f20: fe06 0302 fd02 040c fc04 0702 0502 0104  ................
-00000f30: fb02 0202 fe02 0302 fd06 0402 fc06 0502  ................
-00000f40: fb02 060c fa04 0902 0402 0102 0102 0104  ................
-00000f50: fa02 0202 fe06 0302 fd06 0402 fc0a 0502  ................
-00000f60: fb0a 0602 fa06 070c f904 0a02 0404 fd02  ................
-00000f70: 0202 fe06 0302 fd06 040c fc04 0702 0402  ................
-00000f80: 0102 0102 0104 fa02 0202 fe06 0302 fd0a  ................
-00000f90: 0402 fc06 0502 fb06 0602 fa02 0710 f972  ...............r
-00000fa0: 3400 0000 291e 7255 0000 0072 3100 0000  4...).rU...r1...
-00000fb0: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-00000fc0: 0000 da08 7079 6461 6e74 6963 da04 6175  ....pydantic..au
-00000fd0: 7468 7205 0000 00da 0468 7474 7072 0600  thr......httpr..
-00000fe0: 0000 724f 0000 0072 0700 0000 da05 7365  ..rO...r......se
-00000ff0: 7264 6572 0900 0000 da04 7469 6d65 720a  rder......timer.
-00001000: 0000 00da 0775 7064 6174 6573 720b 0000  .....updatesr...
-00001010: 0072 0c00 0000 da05 6669 6c65 7372 0e00  .r......filesr..
-00001020: 0000 720f 0000 0072 4300 0000 7211 0000  ..r....rC...r...
-00001030: 0072 1200 0000 7213 0000 00da 0942 6173  .r....r......Bas
-00001040: 654d 6f64 656c 7214 0000 00da 0341 4243  eModelr......ABC
-00001050: 7234 0000 0072 2000 0000 7220 0000 0072  r4...r ...r ...r
-00001060: 2000 0000 7221 0000 00da 083c 6d6f 6475   ...r!.....<modu
-00001070: 6c65 3e01 0000 0073 1c00 0000 0800 0801  le>....s........
-00001080: 1001 0802 0c02 0c01 0c01 0c01 0c01 1001  ................
-00001090: 1004 1401 1207 1619                      ........
+00000680: 0040 0000 0073 a001 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000690: 5a02 6503 6a04 6401 6505 6402 6505 6403  Z.e.j.d.e.d.e.d.
+000006a0: 6404 6606 6405 6406 8404 8301 5a06 6503  d.f.d.d.....Z.e.
+000006b0: 6a04 6507 6a08 6404 6509 6a0a 6404 6404  j.e.j.d.e.j.d.d.
+000006c0: 6404 6404 6607 6407 6507 6408 650b 650c  d.d.f.d.e.d.e.e.
+000006d0: 6505 650d 6602 1900 1900 6409 6509 640a  e.e.f.....d.e.d.
+000006e0: 650b 650e 6505 1900 1900 640b 650b 6505  e.e.e.....d.e.e.
+000006f0: 1900 640c 650b 6505 1900 640d 650b 6505  ..d.e.e...d.e.e.
+00000700: 1900 6403 650f 6610 640e 640f 8405 8301  ..d.e.f.d.d.....
+00000710: 5a10 6503 6a04 6410 650f 6403 6404 6604  Z.e.j.d.e.d.d.f.
+00000720: 6411 6412 8404 8301 5a11 6503 6a04 6401  d.d.....Z.e.j.d.
+00000730: 6505 6403 650f 6604 6413 6414 8404 8301  e.d.e.f.d.d.....
+00000740: 5a12 6503 6a04 0904 0904 6426 6410 650f  Z.e.j.....d&d.e.
+00000750: 6415 6513 6416 650b 6505 1900 6402 650b  d.e.d.e.e...d.e.
+00000760: 6505 1900 6403 6514 660a 6417 6418 8405  e...d.e.f.d.d...
+00000770: 8301 5a15 6503 6a04 0904 0904 0904 6427  ..Z.e.j.......d'
+00000780: 6401 6505 6419 650b 6505 1900 641a 650b  d.e.d.e.e...d.e.
+00000790: 650e 6505 1900 1900 641b 650b 650e 6505  e.e.....d.e.e.e.
+000007a0: 1900 1900 6403 6516 6517 1900 660a 641c  ....d.e.e...f.d.
+000007b0: 641d 8405 8301 5a18 6503 6a04 0904 6428  d.....Z.e.j...d(
+000007c0: 641e 6519 640b 650b 6505 1900 6403 6516  d.e.d.e.e...d.e.
+000007d0: 650f 1900 6606 641f 6420 8405 8301 5a1a  e...f.d.d ....Z.
+000007e0: 6503 6a04 0904 0904 0904 0904 6429 6410  e.j.........d)d.
+000007f0: 650f 6421 650b 651b 1900 6422 650b 650e  e.d!e.e...d"e.e.
+00000800: 651c 1900 1900 640d 650b 6505 1900 6423  e.....d.e.e...d#
+00000810: 650b 6505 1900 6403 650f 660c 6424 6425  e.e...d.e.f.d$d%
+00000820: 8405 8301 5a1d 6404 5300 292a da0f 4461  ....Z.d.S.)*..Da
+00000830: 7461 7365 7444 656c 6567 6174 65da 0a64  tasetDelegate..d
+00000840: 6174 6173 6574 5f69 64da 0e74 7261 6e73  ataset_id..trans
+00000850: 6163 7469 6f6e 5f69 6472 1c00 0000 4e63  action_idr....Nc
+00000860: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000870: 0200 0000 4300 0000 f308 0000 0074 0064  ....C........t.d
+00000880: 0183 0182 0129 024e da0f 636f 6d70 6c65  .....).N..comple
+00000890: 7465 5f75 706c 6f61 64a9 01da 134e 6f74  te_upload....Not
+000008a0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+000008b0: 2903 721f 0000 0072 3500 0000 7236 0000  ).r....r5...r6..
+000008c0: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
+000008d0: 7238 0000 0032 0000 00f3 0200 0000 0802  r8...2..........
+000008e0: 7a1f 4461 7461 7365 7444 656c 6567 6174  z.DatasetDelegat
+000008f0: 652e 636f 6d70 6c65 7465 5f75 706c 6f61  e.complete_uploa
+00000900: 64da 0d61 646d 696e 6973 7472 6174 6f72  d..administrator
+00000910: da08 6d65 7461 6461 7461 da10 7374 6f72  ..metadata..stor
+00000920: 6167 655f 6c6f 6361 7469 6f6e da04 7461  age_location..ta
+00000930: 6773 da06 6f72 675f 6964 da0a 6372 6561  gs..org_id..crea
+00000940: 7465 645f 6279 da0b 6465 7363 7269 7074  ted_by..descript
+00000950: 696f 6e63 0800 0000 0000 0000 0000 0000  ionc............
+00000960: 0800 0000 0200 0000 4300 0000 7237 0000  ........C...r7..
+00000970: 0029 024e da0e 6372 6561 7465 5f64 6174  .).N..create_dat
+00000980: 6173 6574 7239 0000 0029 0872 1f00 0000  asetr9...).r....
+00000990: 723c 0000 0072 3d00 0000 723e 0000 0072  r<...r=...r>...r
+000009a0: 3f00 0000 7240 0000 0072 4100 0000 7242  ?...r@...rA...rB
+000009b0: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+000009c0: 0000 7243 0000 0036 0000 0073 0200 0000  ..rC...6...s....
+000009d0: 080b 7a1e 4461 7461 7365 7444 656c 6567  ..z.DatasetDeleg
+000009e0: 6174 652e 6372 6561 7465 5f64 6174 6173  ate.create_datas
+000009f0: 6574 da06 7265 636f 7264 6302 0000 0000  et..recordc.....
+00000a00: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+00000a10: 0000 0072 3700 0000 2902 4eda 0e64 656c  ...r7...).N..del
+00000a20: 6574 655f 6461 7461 7365 7472 3900 0000  ete_datasetr9...
+00000a30: 2902 721f 0000 0072 4400 0000 7220 0000  ).r....rD...r ..
+00000a40: 0072 2000 0000 7221 0000 0072 4500 0000  .r ...r!...rE...
+00000a50: 4300 0000 723b 0000 007a 1e44 6174 6173  C...r;...z.Datas
+00000a60: 6574 4465 6c65 6761 7465 2e64 656c 6574  etDelegate.delet
+00000a70: 655f 6461 7461 7365 7463 0200 0000 0000  e_datasetc......
+00000a80: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+00000a90: 0000 7237 0000 0029 024e 5a1a 6765 745f  ..r7...).NZ.get_
+00000aa0: 6461 7461 7365 745f 6279 5f70 7269 6d61  dataset_by_prima
+00000ab0: 7279 5f6b 6579 7239 0000 0029 0272 1f00  ry_keyr9...).r..
+00000ac0: 0000 7235 0000 0072 2000 0000 7220 0000  ..r5...r ...r ..
+00000ad0: 0072 2100 0000 da11 6765 745f 6461 7461  .r!.....get_data
+00000ae0: 7365 745f 6279 5f69 6447 0000 0073 0200  set_by_idG...s..
+00000af0: 0000 0805 7a21 4461 7461 7365 7444 656c  ....z!DatasetDel
+00000b00: 6567 6174 652e 6765 745f 6461 7461 7365  egate.get_datase
+00000b10: 745f 6279 5f69 64da 0b70 6572 6d69 7373  t_by_id..permiss
+00000b20: 696f 6e73 da06 6361 6c6c 6572 6305 0000  ions..callerc...
+00000b30: 0000 0000 0000 0000 0005 0000 0002 0000  ................
+00000b40: 0043 0000 0072 3700 0000 2902 4eda 1967  .C...r7...).N..g
+00000b50: 6574 5f74 656d 706f 7261 7279 5f63 7265  et_temporary_cre
+00000b60: 6465 6e74 6961 6c73 7239 0000 0029 0572  dentialsr9...).r
+00000b70: 1f00 0000 7244 0000 0072 4700 0000 7248  ....rD...rG...rH
+00000b80: 0000 0072 3600 0000 7220 0000 0072 2000  ...r6...r ...r .
+00000b90: 0000 7221 0000 0072 4900 0000 4e00 0000  ..r!...rI...N...
+00000ba0: f302 0000 0008 087a 2944 6174 6173 6574  .......z)Dataset
+00000bb0: 4465 6c65 6761 7465 2e67 6574 5f74 656d  Delegate.get_tem
+00000bc0: 706f 7261 7279 5f63 7265 6465 6e74 6961  porary_credentia
+00000bd0: 6c73 da0a 7061 6765 5f74 6f6b 656e da10  ls..page_token..
+00000be0: 696e 636c 7564 655f 7061 7474 6572 6e73  include_patterns
+00000bf0: da10 6578 636c 7564 655f 7061 7474 6572  ..exclude_patter
+00000c00: 6e73 6305 0000 0000 0000 0000 0000 0005  nsc.............
+00000c10: 0000 0002 0000 0043 0000 0072 3700 0000  .......C...r7...
+00000c20: 2902 4eda 0a6c 6973 745f 6669 6c65 7372  ).N..list_filesr
+00000c30: 3900 0000 2905 721f 0000 0072 3500 0000  9...).r....r5...
+00000c40: 724b 0000 0072 4c00 0000 724d 0000 0072  rK...rL...rM...r
+00000c50: 2000 0000 7220 0000 0072 2100 0000 724e   ...r ...r!...rN
+00000c60: 0000 0058 0000 0072 4a00 0000 7a1a 4461  ...X...rJ...z.Da
+00000c70: 7461 7365 7444 656c 6567 6174 652e 6c69  tasetDelegate.li
+00000c80: 7374 5f66 696c 6573 da05 7175 6572 7963  st_files..queryc
+00000c90: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000ca0: 0200 0000 4300 0000 7237 0000 0029 024e  ....C...r7...).N
+00000cb0: da0e 7175 6572 795f 6461 7461 7365 7473  ..query_datasets
+00000cc0: 7239 0000 0029 0372 1f00 0000 724f 0000  r9...).r....rO..
+00000cd0: 0072 4000 0000 7220 0000 0072 2000 0000  .r@...r ...r ...
+00000ce0: 7221 0000 0072 5000 0000 6200 0000 7302  r!...rP...b...s.
+00000cf0: 0000 0008 067a 1e44 6174 6173 6574 4465  .....z.DatasetDe
+00000d00: 6c65 6761 7465 2e71 7565 7279 5f64 6174  legate.query_dat
+00000d10: 6173 6574 73da 126d 6574 6164 6174 615f  asets..metadata_
+00000d20: 6368 616e 6765 7365 74da 0a63 6f6e 6469  changeset..condi
+00000d30: 7469 6f6e 73da 0a75 7064 6174 6564 5f62  tions..updated_b
+00000d40: 7963 0600 0000 0000 0000 0000 0000 0600  yc..............
+00000d50: 0000 0200 0000 4300 0000 7237 0000 0029  ......C...r7...)
+00000d60: 024e da06 7570 6461 7465 7239 0000 0029  .N..updater9...)
+00000d70: 0672 1f00 0000 7244 0000 0072 5100 0000  .r....rD...rQ...
+00000d80: 7252 0000 0072 4200 0000 7253 0000 0072  rR...rB...rS...r
+00000d90: 2000 0000 7220 0000 0072 2100 0000 7254   ...r ...r!...rT
+00000da0: 0000 006a 0000 0073 0200 0000 0809 7a16  ...j...s......z.
+00000db0: 4461 7461 7365 7444 656c 6567 6174 652e  DatasetDelegate.
+00000dc0: 7570 6461 7465 2902 4e4e 2903 4e4e 4e72  update).NN).NNNr
+00000dd0: 1d00 0000 2904 4e4e 4e4e 291e 722c 0000  ....).NNNN).r,..
+00000de0: 0072 2d00 0000 722e 0000 00da 0361 6263  .r-...r......abc
+00000df0: da0e 6162 7374 7261 6374 6d65 7468 6f64  ..abstractmethod
+00000e00: 722f 0000 0072 3800 0000 7211 0000 00da  r/...r8...r.....
+00000e10: 0652 6f62 6f74 6f72 1300 0000 da02 5333  .Robotor......S3
+00000e20: 7203 0000 0072 3300 0000 7202 0000 00da  r....r3...r.....
+00000e30: 046c 6973 7472 1200 0000 7243 0000 0072  .listr....rC...r
+00000e40: 4500 0000 7246 0000 0072 0500 0000 7214  E...rF...r....r.
+00000e50: 0000 0072 4900 0000 7206 0000 0072 0e00  ...rI...r....r..
+00000e60: 0000 724e 0000 0072 0700 0000 7250 0000  ..rN...r....rP..
+00000e70: 0072 0b00 0000 720c 0000 0072 5400 0000  .r....r....rT...
+00000e80: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
+00000e90: 2100 0000 7234 0000 0031 0000 0073 b800  !...r4...1...s..
+00000ea0: 0000 0800 0401 1801 0403 0403 0201 0401  ................
+00000eb0: 0201 0201 0201 0201 04f8 0202 02fe 0e03  ................
+00000ec0: 02fd 0204 02fc 0a05 02fb 0606 02fa 0607  ................
+00000ed0: 02f9 0608 02f8 0209 0cf7 040c 1401 0403  ................
+00000ee0: 0201 0202 02fe 0203 0cfd 0406 0205 0201  ................
+00000ef0: 04fb 0202 02fe 0203 02fd 0604 02fc 0605  ................
+00000f00: 02fb 0206 0cfa 0409 0204 0201 0201 04fb  ................
+00000f10: 0202 02fe 0603 02fd 0a04 02fc 0a05 02fb  ................
+00000f20: 0606 0cfa 0409 0204 04fd 0202 02fe 0603  ................
+00000f30: 02fd 0604 0cfc 0407 0204 0201 0201 0201  ................
+00000f40: 04fa 0202 02fe 0603 02fd 0a04 02fc 0605  ................
+00000f50: 02fb 0606 02fa 0207 10f9 7234 0000 0029  ..........r4...)
+00000f60: 1e72 5500 0000 7231 0000 00da 0674 7970  .rU...r1.....typ
+00000f70: 696e 6772 0200 0000 7203 0000 00da 0870  ingr....r......p
+00000f80: 7964 616e 7469 63da 0461 7574 6872 0500  ydantic..authr..
+00000f90: 0000 da04 6874 7470 7206 0000 0072 4f00  ....httpr....rO.
+00000fa0: 0000 7207 0000 00da 0573 6572 6465 7209  ..r......serder.
+00000fb0: 0000 00da 0474 696d 6572 0a00 0000 da07  .....timer......
+00000fc0: 7570 6461 7465 7372 0b00 0000 720c 0000  updatesr....r...
+00000fd0: 00da 0566 696c 6573 720e 0000 0072 0f00  ...filesr....r..
+00000fe0: 0000 7244 0000 0072 1100 0000 7212 0000  ..rD...r....r...
+00000ff0: 0072 1300 0000 da09 4261 7365 4d6f 6465  .r......BaseMode
+00001000: 6c72 1400 0000 da03 4142 4372 3400 0000  lr......ABCr4...
+00001010: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
+00001020: 2100 0000 da08 3c6d 6f64 756c 653e 0100  !.....<module>..
+00001030: 0000 731c 0000 0008 0008 0110 0108 020c  ..s.............
+00001040: 020c 010c 010c 010c 0110 0110 0414 0112  ................
+00001050: 0716 19                                  ...
```

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/__pycache__/http_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/datasets/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 7970 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 221f 0000  o........Y.e"...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 741e 0000  o.......2H.et...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6403 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6403 6405 6c07 6d08 5a08 0100 6403  ..d.d.l.m.Z...d.
 00000060: 6406 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6403 6407 6c0d 6d0e 5a0e 0100 6403  ..d.d.l.m.Z...d.
@@ -34,424 +34,417 @@
 00000210: 5175 6572 7944 6174 6173 6574 4669 6c65  QueryDatasetFile
 00000220: 7352 6571 7565 7374 da14 5570 6461 7465  sRequest..Update
 00000230: 4461 7461 7365 7452 6571 7565 7374 2903  DatasetRequest).
 00000240: da0d 4164 6d69 6e69 7374 7261 746f 72da  ..Administrator.
 00000250: 0d44 6174 6173 6574 5265 636f 7264 da0f  .DatasetRecord..
 00000260: 5374 6f72 6167 654c 6f63 6174 696f 6e63  StorageLocationc
 00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 1100 0000 0000 0000 73f8 0100 0065 005a  ........s....e.Z
+00000280: 1100 0000 0000 0000 73d6 0100 0065 005a  ........s....e.Z
 00000290: 0164 005a 0255 0065 0365 0464 013c 0065  .d.Z.U.e.e.d.<.e
 000002a0: 0565 0464 023c 0064 0365 0564 0465 0364  .e.d.<.d.e.d.e.d
 000002b0: 0564 0666 0687 0066 0164 0764 0884 0c5a  .d.f...f.d.d...Z
 000002c0: 0609 0609 0609 0664 3064 0965 0765 0519  .......d0d.e.e..
 000002d0: 0064 0a65 0765 0519 0064 0b65 0765 0519  .d.e.e...d.e.e..
 000002e0: 0064 0565 0865 0565 0566 0219 0066 0864  .d.e.e.e.f...f.d
 000002f0: 0c64 0d84 055a 0965 0a6a 0b64 0665 0c6a  .d...Z.e.j.d.e.j
 00000300: 0d64 0664 0664 0664 0666 0764 0e65 0a64  .d.d.d.d.f.d.e.d
 00000310: 0f65 0765 0865 0565 0e66 0219 0019 0064  .e.e.e.e.f.....d
 00000320: 1065 0c64 1165 0765 0f65 0519 0019 0064  .e.d.e.e.e.....d
 00000330: 0965 0765 0519 0064 1265 0765 0519 0064  .e.e...d.e.e...d
 00000340: 1365 0765 0519 0064 0565 1066 1064 1464  .e.e...d.e.f.d.d
 00000350: 1584 055a 1164 1665 1064 0564 0666 0464  ...Z.d.e.d.d.f.d
-00000360: 1764 1884 045a 1209 0664 3164 1965 0564  .d...Z...d1d.e.d
-00000370: 0965 0765 0519 0064 0565 1066 0664 1a64  .e.e...d.e.f.d.d
-00000380: 1b84 055a 1309 0609 0664 3264 1665 1064  ...Z.....d2d.e.d
-00000390: 1c65 1464 1d65 0765 0519 0064 1e65 0765  .e.d.e.e...d.e.e
-000003a0: 0519 0064 0565 1566 0a64 1f64 2084 055a  ...d.e.f.d.d ..Z
-000003b0: 1609 0664 3164 1965 0564 1e65 0564 0965  ...d1d.e.d.e.d.e
-000003c0: 0765 0519 0064 0564 0666 0864 2164 2284  .e...d.d.f.d!d".
-000003d0: 055a 1709 0609 0609 0609 0664 3364 1965  .Z.........d3d.e
-000003e0: 0564 0965 0765 0519 0064 2365 0765 0519  .d.e.e...d#e.e..
-000003f0: 0064 2465 0765 0f65 0519 0019 0064 2565  .d$e.e.e.....d%e
-00000400: 0765 0f65 0519 0019 0064 0565 1865 1919  .e.e.....d.e.e..
-00000410: 0066 0c64 2664 2784 055a 1a09 0664 3164  .f.d&d'..Z...d1d
-00000420: 2865 1b64 0965 0765 0519 0064 0565 1865  (e.d.e.e...d.e.e
-00000430: 1019 0066 0664 2964 2a84 055a 1c09 0609  ...f.d)d*..Z....
-00000440: 0609 0609 0664 3364 1665 1064 2b65 0765  .....d3d.e.d+e.e
-00000450: 1d19 0064 2c65 0765 0f65 1e19 0019 0064  ...d,e.e.e.....d
-00000460: 1365 0765 0519 0064 2d65 0765 0519 0064  .e.e...d-e.e...d
-00000470: 0565 1066 0c64 2e64 2f84 055a 1f87 0004  .e.f.d.d/..Z....
-00000480: 005a 2053 0029 34da 1344 6174 6173 6574  .Z S.)4..Dataset
-00000490: 4874 7470 4465 6c65 6761 7465 da21 5f44  HttpDelegate.!_D
-000004a0: 6174 6173 6574 4874 7470 4465 6c65 6761  atasetHttpDelega
-000004b0: 7465 5f5f 6874 7470 5f63 6c69 656e 74da  te__http_client.
-000004c0: 2d5f 4461 7461 7365 7448 7474 7044 656c  -_DatasetHttpDel
-000004d0: 6567 6174 655f 5f72 6f62 6f74 6f5f 7365  egate__roboto_se
-000004e0: 7276 6963 655f 6261 7365 5f75 726c da17  rvice_base_url..
-000004f0: 726f 626f 746f 5f73 6572 7669 6365 5f62  roboto_service_b
-00000500: 6173 655f 7572 6cda 0b68 7474 705f 636c  ase_url..http_cl
-00000510: 6965 6e74 da06 7265 7475 726e 4e63 0300  ient..returnNc..
-00000520: 0000 0000 0000 0000 0000 0300 0000 0200  ................
-00000530: 0000 0300 0000 731a 0000 0074 0083 00a0  ......s....t....
-00000540: 01a1 0001 007c 027c 005f 027c 017c 005f  .....|.|._.|.|._
-00000550: 0364 0053 00a9 014e 2904 da05 7375 7065  .d.S...N)...supe
-00000560: 72da 085f 5f69 6e69 745f 5f72 1a00 0000  r..__init__r....
-00000570: 721b 0000 0029 03da 0473 656c 6672 1c00  r....)...selfr..
-00000580: 0000 721d 0000 00a9 01da 095f 5f63 6c61  ..r........__cla
-00000590: 7373 5f5f a900 faed 2f63 6f64 6562 7569  ss__..../codebui
-000005a0: 6c64 2f6f 7574 7075 742f 7372 6331 3035  ld/output/src105
-000005b0: 3131 3832 3038 392f 7372 632f 636f 6465  1182089/src/code
-000005c0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
-000005d0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
-000005e0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
-000005f0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
-00000600: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
-00000610: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
-00000620: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
-00000630: 626f 746f 2d61 692f 726f 626f 746f 2d68  boto-ai/roboto-h
-00000640: 6f73 7465 642d 6170 702f 7061 636b 6167  osted-app/packag
-00000650: 6573 2f72 6f62 6f74 6f2f 7372 632f 726f  es/roboto/src/ro
-00000660: 626f 746f 2f64 6f6d 6169 6e2f 6461 7461  boto/domain/data
-00000670: 7365 7473 2f68 7474 705f 6465 6c65 6761  sets/http_delega
-00000680: 7465 2e70 7972 2100 0000 2300 0000 7306  te.pyr!...#...s.
-00000690: 0000 000a 0106 010a 017a 1c44 6174 6173  .........z.Datas
-000006a0: 6574 4874 7470 4465 6c65 6761 7465 2e5f  etHttpDelegate._
-000006b0: 5f69 6e69 745f 5fda 066f 7267 5f69 64da  _init__..org_id.
-000006c0: 0775 7365 725f 6964 da11 7265 736f 7572  .user_id..resour
-000006d0: 6365 5f6f 776e 6572 5f69 6463 0400 0000  ce_owner_idc....
-000006e0: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-000006f0: 4300 0000 7314 0000 0074 007c 017c 027c  C...s....t.|.|.|
-00000700: 0364 0164 0269 0164 038d 0453 0029 044e  .d.d.i.d...S.).N
-00000710: 7a0c 436f 6e74 656e 742d 5479 7065 7a10  z.Content-Typez.
-00000720: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00000730: 2904 7227 0000 0072 2800 0000 7229 0000  ).r'...r(...r)..
-00000740: 00da 1261 6464 6974 696f 6e61 6c5f 6865  ...additional_he
-00000750: 6164 6572 7329 0172 0900 0000 2904 7222  aders).r....).r"
-00000760: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
-00000770: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
-00000780: 00da 0768 6561 6465 7273 2800 0000 730c  ...headers(...s.
-00000790: 0000 0002 0602 0102 0102 0106 0106 fc7a  ...............z
-000007a0: 1b44 6174 6173 6574 4874 7470 4465 6c65  .DatasetHttpDele
-000007b0: 6761 7465 2e68 6561 6465 7273 da0d 6164  gate.headers..ad
-000007c0: 6d69 6e69 7374 7261 746f 72da 086d 6574  ministrator..met
-000007d0: 6164 6174 61da 1073 746f 7261 6765 5f6c  adata..storage_l
-000007e0: 6f63 6174 696f 6eda 0474 6167 73da 0a63  ocation..tags..c
-000007f0: 7265 6174 6564 5f62 79da 0b64 6573 6372  reated_by..descr
-00000800: 6970 7469 6f6e 6308 0000 0000 0000 0000  iptionc.........
-00000810: 0000 000b 0000 0008 0000 0043 0000 0073  ...........C...s
-00000820: 8e00 0000 7c00 6a00 9b00 6401 9d02 7d08  ....|.j...d...}.
-00000830: 7401 7c01 7c02 6402 7501 720e 7c02 6e01  t.|.|.d.u.r.|.n.
-00000840: 6900 7c03 7c07 7c04 6402 7501 7217 7c04  i.|.|.|.d.u.r.|.
-00000850: 6e01 6700 6403 8d05 7d09 7402 8300 8f17  n.g.d...}.t.....
-00000860: 0100 7c00 6a03 6a04 7c08 7405 7c09 8301  ..|.j.j.|.t.|...
-00000870: 7c00 a006 7c05 7c06 a102 6404 8d03 7d0a  |...|.|...d...}.
-00000880: 5700 6402 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
-00000890: 7338 7701 0100 0100 0100 5900 0100 7407  s8w.......Y...t.
-000008a0: a008 7c0a 6a09 6405 6701 6406 8d01 a101  ..|.j.d.g.d.....
-000008b0: 5300 2907 7a27 0a20 2020 2020 2020 2043  S.).z'.        C
-000008c0: 7265 6174 6520 6120 6e65 7720 6461 7461  reate a new data
-000008d0: 7365 742e 0a20 2020 2020 2020 207a 0c2f  set..        z./
-000008e0: 7631 2f64 6174 6173 6574 734e 2905 722c  v1/datasetsN).r,
-000008f0: 0000 0072 2d00 0000 722e 0000 0072 3100  ...r-...r....r1.
-00000900: 0000 722f 0000 00a9 02da 0464 6174 6172  ..r/.......datar
-00000910: 2b00 0000 7233 0000 00a9 01da 096a 736f  +...r3.......jso
-00000920: 6e5f 7061 7468 290a 721b 0000 0072 1300  n_path).r....r..
-00000930: 0000 7206 0000 0072 1a00 0000 da04 706f  ..r....r......po
-00000940: 7374 720b 0000 0072 2b00 0000 7217 0000  str....r+...r...
-00000950: 00da 0e6d 6f64 656c 5f76 616c 6964 6174  ...model_validat
-00000960: 65da 0966 726f 6d5f 6a73 6f6e 290b 7222  e..from_json).r"
-00000970: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
-00000980: 0000 722f 0000 0072 2700 0000 7230 0000  ..r/...r'...r0..
-00000990: 0072 3100 0000 da03 7572 6cda 0c72 6571  .r1.....url..req
-000009a0: 7565 7374 5f62 6f64 79da 0872 6573 706f  uest_body..respo
-000009b0: 6e73 6572 2500 0000 7225 0000 0072 2600  nser%...r%...r&.
-000009c0: 0000 da0e 6372 6561 7465 5f64 6174 6173  ....create_datas
-000009d0: 6574 3500 0000 7320 0000 000c 0d02 0102  et5...s ........
-000009e0: 010e 0102 0102 010e 0106 fb08 0806 0102  ................
-000009f0: 0106 010a 0108 fd1c ff14 077a 2244 6174  ...........z"Dat
-00000a00: 6173 6574 4874 7470 4465 6c65 6761 7465  asetHttpDelegate
-00000a10: 2e63 7265 6174 655f 6461 7461 7365 74da  .create_dataset.
-00000a20: 0672 6563 6f72 6463 0200 0000 0000 0000  .recordc........
-00000a30: 0000 0000 0300 0000 0800 0000 4300 0000  ............C...
-00000a40: 7356 0000 007c 006a 009b 0064 017c 016a  sV...|.j...d.|.j
-00000a50: 019b 009d 037d 0274 0283 008f 1501 007c  .....}.t.......|
-00000a60: 006a 036a 047c 027c 00a0 057c 016a 06a1  .j.j.|.|...|.j..
-00000a70: 0164 028d 0201 0057 0064 0304 0004 0083  .d.....W.d......
-00000a80: 0301 0064 0353 0031 0073 2477 0101 0001  ...d.S.1.s$w....
-00000a90: 0001 0059 0001 0064 0353 0029 047a 230a  ...Y...d.S.).z#.
-00000aa0: 2020 2020 2020 2020 4465 6c65 7465 2061          Delete a
-00000ab0: 2064 6174 6173 6574 2e0a 2020 2020 2020   dataset..      
-00000ac0: 2020 fa0d 2f76 312f 6461 7461 7365 7473    ../v1/datasets
-00000ad0: 2fa9 0172 2b00 0000 4e29 0772 1b00 0000  /..r+...N).r....
-00000ae0: da0a 6461 7461 7365 745f 6964 7206 0000  ..dataset_idr...
-00000af0: 0072 1a00 0000 da06 6465 6c65 7465 722b  .r......deleter+
-00000b00: 0000 0072 2700 0000 2903 7222 0000 0072  ...r'...).r"...r
-00000b10: 3d00 0000 7239 0000 0072 2500 0000 7225  =...r9...r%...r%
-00000b20: 0000 0072 2600 0000 da0e 6465 6c65 7465  ...r&.....delete
-00000b30: 5f64 6174 6173 6574 5400 0000 730e 0000  _datasetT...s...
-00000b40: 0012 0408 0206 0102 010a 0108 fe22 ff7a  .............".z
-00000b50: 2244 6174 6173 6574 4874 7470 4465 6c65  "DatasetHttpDele
-00000b60: 6761 7465 2e64 656c 6574 655f 6461 7461  gate.delete_data
-00000b70: 7365 7472 4000 0000 6303 0000 0000 0000  setr@...c.......
-00000b80: 0000 0000 0005 0000 0008 0000 0043 0000  .............C..
-00000b90: 0073 6000 0000 7c00 6a00 9b00 6401 7c01  .s`...|.j...d.|.
-00000ba0: 9b00 9d03 7d03 7401 8300 8f13 0100 7c00  ....}.t.......|.
-00000bb0: 6a02 6a03 7c03 7c00 a004 7c02 a101 6402  j.j.|.|...|...d.
-00000bc0: 8d02 7d04 5700 6403 0400 0400 8303 0100  ..}.W.d.........
-00000bd0: 6e08 3100 7321 7701 0100 0100 0100 5900  n.1.s!w.......Y.
-00000be0: 0100 7405 a006 7c04 6a07 6404 6701 6405  ..t...|.j.d.g.d.
-00000bf0: 8d01 a101 5300 2906 7a47 0a20 2020 2020  ....S.).zG.     
-00000c00: 2020 2047 6574 2061 2064 6174 6173 6574     Get a dataset
-00000c10: 2062 7920 6974 7320 7072 696d 6172 7920   by its primary 
-00000c20: 6b65 7920 286f 7267 5f69 642c 2064 6174  key (org_id, dat
-00000c30: 6173 6574 5f69 6429 0a20 2020 2020 2020  aset_id).       
-00000c40: 2072 3e00 0000 723f 0000 004e 7233 0000   r>...r?...Nr3..
-00000c50: 0072 3400 0000 2908 721b 0000 0072 0600  .r4...).r....r..
-00000c60: 0000 721a 0000 00da 0367 6574 722b 0000  ..r......getr+..
-00000c70: 0072 1700 0000 7237 0000 0072 3800 0000  .r....r7...r8...
-00000c80: 2905 7222 0000 0072 4000 0000 7227 0000  ).r"...r@...r'..
-00000c90: 0072 3900 0000 723b 0000 0072 2500 0000  .r9...r;...r%...
-00000ca0: 7225 0000 0072 2600 0000 da1a 6765 745f  r%...r&.....get_
-00000cb0: 6461 7461 7365 745f 6279 5f70 7269 6d61  dataset_by_prima
-00000cc0: 7279 5f6b 6579 6000 0000 730a 0000 0010  ry_key`...s.....
-00000cd0: 0808 0218 011c ff14 037a 2e44 6174 6173  .........z.Datas
-00000ce0: 6574 4874 7470 4465 6c65 6761 7465 2e67  etHttpDelegate.g
-00000cf0: 6574 5f64 6174 6173 6574 5f62 795f 7072  et_dataset_by_pr
-00000d00: 696d 6172 795f 6b65 79da 0b70 6572 6d69  imary_key..permi
-00000d10: 7373 696f 6e73 da06 6361 6c6c 6572 da0e  ssions..caller..
-00000d20: 7472 616e 7361 6374 696f 6e5f 6964 6305  transaction_idc.
-00000d30: 0000 0000 0000 0000 0000 0009 0000 0008  ................
-00000d40: 0000 0043 0000 0073 9200 0000 6401 7c02  ...C...s....d.|.
-00000d50: 6a00 6901 7d05 7401 6a02 a003 7c05 a101  j.i.}.t.j...|...
-00000d60: 7d06 7c00 6a04 9b00 6402 7c01 6a05 9b00  }.|.j...d.|.j...
-00000d70: 6403 7c06 9b00 9d05 7d07 7c04 7220 7c07  d.|.....}.|.r |.
-00000d80: 6404 7c04 9b00 9d02 3700 7d07 7406 8300  d.|.....7.}.t...
-00000d90: 8f14 0100 7c00 6a07 a008 7c07 7c00 a009  ....|.j...|.|...
-00000da0: 7c01 6a0a 7c03 a102 a102 7d08 5700 6405  |.j.|.....}.W.d.
-00000db0: 0400 0400 8303 0100 6e08 3100 733a 7701  ........n.1.s:w.
-00000dc0: 0100 0100 0100 5900 0100 740b a00c 7c08  ......Y...t...|.
-00000dd0: 6a0d 6406 6701 6407 8d01 a101 5300 2908  j.d.g.d.....S.).
-00000de0: 7a40 0a20 2020 2020 2020 2047 6574 2074  z@.        Get t
-00000df0: 656d 706f 7261 7279 2063 7265 6465 6e74  emporary credent
-00000e00: 6961 6c73 2074 6f20 6163 6365 7373 2061  ials to access a
-00000e10: 2064 6174 6173 6574 2e0a 2020 2020 2020   dataset..      
-00000e20: 2020 da04 6d6f 6465 723e 0000 007a 0d2f    ..moder>...z./
-00000e30: 6372 6564 656e 7469 616c 733f 7a10 2674  credentials?z.&t
-00000e40: 7261 6e73 6163 7469 6f6e 5f69 643d 4e72  ransaction_id=Nr
-00000e50: 3300 0000 7234 0000 0029 0eda 0576 616c  3...r4...)...val
-00000e60: 7565 da06 7572 6c6c 6962 da05 7061 7273  ue..urllib..pars
-00000e70: 65da 0975 726c 656e 636f 6465 721b 0000  e..urlencoder...
-00000e80: 0072 4000 0000 7206 0000 0072 1a00 0000  .r@...r....r....
-00000e90: 7243 0000 0072 2b00 0000 7227 0000 0072  rC...r+...r'...r
-00000ea0: 1100 0000 7237 0000 0072 3800 0000 2909  ....r7...r8...).
-00000eb0: 7222 0000 0072 3d00 0000 7245 0000 0072  r"...r=...rE...r
-00000ec0: 4600 0000 7247 0000 00da 0c71 7565 7279  F...rG.....query
-00000ed0: 5f70 6172 616d 73da 0a65 6e63 6f64 6564  _params..encoded
-00000ee0: 5f71 7372 3900 0000 723b 0000 0072 2500  _qsr9...r;...r%.
-00000ef0: 0000 7225 0000 0072 2600 0000 da19 6765  ..r%...r&.....ge
-00000f00: 745f 7465 6d70 6f72 6172 795f 6372 6564  t_temporary_cred
-00000f10: 656e 7469 616c 736f 0000 0073 1200 0000  entialso...s....
-00000f20: 0a0a 0c01 1801 0402 0e01 0802 1a01 1cff  ................
-00000f30: 1403 7a2d 4461 7461 7365 7448 7474 7044  ..z-DatasetHttpD
-00000f40: 656c 6567 6174 652e 6765 745f 7465 6d70  elegate.get_temp
-00000f50: 6f72 6172 795f 6372 6564 656e 7469 616c  orary_credential
-00000f60: 7363 0400 0000 0000 0000 0000 0000 0500  sc..............
-00000f70: 0000 0800 0000 4300 0000 735a 0000 007c  ......C...sZ...|
-00000f80: 006a 009b 0064 017c 019b 0064 027c 029b  .j...d.|...d.|..
-00000f90: 0064 039d 067d 0474 0183 008f 1401 007c  .d...}.t.......|
-00000fa0: 006a 026a 037c 047c 00a0 047c 03a1 0164  .j.j.|.|...|...d
-00000fb0: 048d 0201 0057 0064 0504 0004 0083 0301  .....W.d........
-00000fc0: 0064 0553 0031 0073 2677 0101 0001 0001  .d.S.1.s&w......
-00000fd0: 0059 0001 0064 0553 0029 067a d10a 2020  .Y...d.S.).z..  
-00000fe0: 2020 2020 2020 4d61 726b 7320 616e 2075        Marks an u
-00000ff0: 706c 6f61 6420 6173 2027 636f 6d70 6c65  pload as 'comple
-00001000: 7465 6427 2c20 7768 6963 6820 616c 6c6f  ted', which allo
-00001010: 7773 2074 6865 2052 6f62 6f74 6f20 506c  ws the Roboto Pl
-00001020: 6174 666f 726d 2074 6f20 6576 616c 7561  atform to evalua
-00001030: 7465 2074 7269 6767 6572 7320 666f 7220  te triggers for 
-00001040: 6175 746f 6d61 7469 6320 6163 7469 6f6e  automatic action
-00001050: 206f 6e0a 2020 2020 2020 2020 696e 636f   on.        inco
-00001060: 6d69 6e67 2064 6174 612e 2054 6869 7320  ming data. This 
-00001070: 616c 736f 2061 6964 6573 2072 6570 6f72  also aides repor
-00001080: 7469 6e67 206f 6e20 7061 7274 6961 6c20  ting on partial 
-00001090: 7570 6c6f 6164 2066 6169 6c75 7265 2063  upload failure c
-000010a0: 6173 6573 2e0a 2020 2020 2020 2020 723e  ases..        r>
-000010b0: 0000 007a 092f 7570 6c6f 6164 732f 7a09  ...z./uploads/z.
-000010c0: 2f63 6f6d 706c 6574 6529 0272 3900 0000  /complete).r9...
-000010d0: 722b 0000 004e 2905 721b 0000 0072 0600  r+...N).r....r..
-000010e0: 0000 721a 0000 00da 0370 7574 722b 0000  ..r......putr+..
-000010f0: 0029 0572 2200 0000 7240 0000 0072 4700  .).r"...r@...rG.
-00001100: 0000 7227 0000 0072 3900 0000 7225 0000  ..r'...r9...r%..
-00001110: 0072 2500 0000 7226 0000 00da 0f63 6f6d  .r%...r&.....com
-00001120: 706c 6574 655f 7570 6c6f 6164 8500 0000  plete_upload....
-00001130: 7308 0000 0018 0708 0218 0122 ff7a 2344  s..........".z#D
-00001140: 6174 6173 6574 4874 7470 4465 6c65 6761  atasetHttpDelega
-00001150: 7465 2e63 6f6d 706c 6574 655f 7570 6c6f  te.complete_uplo
-00001160: 6164 da0a 7061 6765 5f74 6f6b 656e da10  ad..page_token..
-00001170: 696e 636c 7564 655f 7061 7474 6572 6e73  include_patterns
-00001180: da10 6578 636c 7564 655f 7061 7474 6572  ..exclude_patter
-00001190: 6e73 6306 0000 0000 0000 0000 0000 000b  nsc.............
-000011a0: 0000 0008 0000 0043 0000 0073 ba00 0000  .......C...s....
-000011b0: 7c00 6a00 9b00 6401 7c01 9b00 6402 9d04  |.j...d.|...d...
-000011c0: 7d06 7c03 721c 7401 6a02 a003 6403 7404  }.|.r.t.j...d.t.
-000011d0: 7c03 8301 6901 a101 7d07 7c06 9b00 6404  |...i...}.|...d.
-000011e0: 7c07 9b00 9d03 7d06 7405 7c03 7c04 7c05  |.....}.t.|.|.|.
-000011f0: 6405 8d03 7d08 7406 8300 8f19 0100 7c00  d...}.t.......|.
-00001200: 6a07 6a08 7c06 7409 7c08 6406 6407 8d02  j.j.|.t.|.d.d...
-00001210: 7c00 a00a 7c02 a101 6406 6408 8d04 7d09  |...|...d.d...}.
-00001220: 5700 6409 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
-00001230: 7342 7701 0100 0100 0100 5900 0100 7c09  sBw.......Y...|.
-00001240: 6a0b 640a 6701 640b 8d01 7d0a 740c 640c  j.d.g.d...}.t.d.
-00001250: 640d 8400 7c0a 640e 1900 4400 8301 7c0a  d...|.d...D...|.
-00001260: 640f 1900 6410 8d02 5300 2911 7ae8 0a20  d...d...S.).z.. 
-00001270: 2020 2020 2020 204c 6973 7420 6669 6c65         List file
-00001280: 7320 6173 736f 6369 6174 6564 2077 6974  s associated wit
-00001290: 6820 6461 7461 7365 742e 0a0a 2020 2020  h dataset...    
-000012a0: 2020 2020 4669 6c65 7320 6172 6520 6173      Files are as
-000012b0: 736f 6369 6174 6564 2077 6974 6820 6461  sociated with da
-000012c0: 7461 7365 7473 2069 6e20 616e 2065 7665  tasets in an eve
-000012d0: 6e74 7561 6c6c 792d 636f 6e73 6973 7465  ntually-consiste
-000012e0: 6e74 206d 616e 6e65 722c 0a20 2020 2020  nt manner,.     
-000012f0: 2020 2073 6f20 7468 6572 6520 7769 6c6c     so there will
-00001300: 206c 696b 656c 7920 6265 2064 656c 6179   likely be delay
-00001310: 2062 6574 7765 656e 2061 2066 696c 6520   between a file 
-00001320: 6265 696e 6720 7570 6c6f 6164 6564 2061  being uploaded a
-00001330: 6e64 2069 7420 6170 7065 6172 696e 6720  nd it appearing 
-00001340: 696e 2074 6869 7320 6c69 7374 2e0a 2020  in this list..  
-00001350: 2020 2020 2020 723e 0000 007a 0c2f 6669        r>...z./fi
-00001360: 6c65 732f 7175 6572 7972 5200 0000 da01  les/queryrR.....
-00001370: 3f29 0372 5200 0000 7253 0000 0072 5400  ?).rR...rS...rT.
-00001380: 0000 54a9 01da 0c65 7863 6c75 6465 5f6e  ..T....exclude_n
-00001390: 6f6e 65a9 0372 3300 0000 722b 0000 00da  one..r3...r+....
-000013a0: 0a69 6465 6d70 6f74 656e 744e 7233 0000  .idempotentNr3..
-000013b0: 0072 3400 0000 6301 0000 0000 0000 0000  .r4...c.........
-000013c0: 0000 0002 0000 0005 0000 0053 0000 00f3  ...........S....
-000013d0: 1600 0000 6700 7c00 5d07 7d01 7400 a001  ....g.|.].}.t...
-000013e0: 7c01 a101 9102 7102 5300 7225 0000 0029  |.....q.S.r%...)
-000013f0: 0272 0f00 0000 7237 0000 0029 02da 022e  .r....r7...)....
-00001400: 30da 0466 696c 6572 2500 0000 7225 0000  0..filer%...r%..
-00001410: 0072 2600 0000 da0a 3c6c 6973 7463 6f6d  .r&.....<listcom
-00001420: 703e b300 0000 7302 0000 0016 007a 3244  p>....s......z2D
-00001430: 6174 6173 6574 4874 7470 4465 6c65 6761  atasetHttpDelega
-00001440: 7465 2e6c 6973 745f 6669 6c65 732e 3c6c  te.list_files.<l
-00001450: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00001460: 3eda 0569 7465 6d73 da0a 6e65 7874 5f74  >..items..next_t
-00001470: 6f6b 656e a902 725e 0000 0072 5f00 0000  oken..r^...r_...
-00001480: 290d 721b 0000 0072 4a00 0000 724b 0000  ).r....rJ...rK..
-00001490: 0072 4c00 0000 da03 7374 7272 1400 0000  .rL.....strr....
-000014a0: 7206 0000 0072 1a00 0000 7236 0000 0072  r....r....r6...r
-000014b0: 0b00 0000 722b 0000 0072 3800 0000 7208  ....r+...r8...r.
-000014c0: 0000 0029 0b72 2200 0000 7240 0000 0072  ...).r"...r@...r
-000014d0: 2700 0000 7252 0000 0072 5300 0000 7254  '...rR...rS...rT
-000014e0: 0000 0072 3900 0000 724e 0000 0072 3a00  ...r9...rN...r:.
-000014f0: 0000 723b 0000 00da 0c75 6e6d 6172 7368  ..r;.....unmarsh
-00001500: 616c 6c65 6472 2500 0000 7225 0000 0072  alledr%...r%...r
-00001510: 2600 0000 da0a 6c69 7374 5f66 696c 6573  &.....list_files
-00001520: 9100 0000 732c 0000 0012 0e04 0114 010e  ....s,..........
-00001530: 0102 0202 0102 0102 0106 fd08 0506 0102  ................
-00001540: 010a 0108 0102 0108 fc1c ff0e 0802 0110  ................
-00001550: 0106 0106 fe7a 1e44 6174 6173 6574 4874  .....z.DatasetHt
-00001560: 7470 4465 6c65 6761 7465 2e6c 6973 745f  tpDelegate.list_
-00001570: 6669 6c65 73da 0571 7565 7279 6303 0000  files..queryc...
-00001580: 0000 0000 0000 0000 0007 0000 0008 0000  ................
-00001590: 0043 0000 0073 8600 0000 7c00 6a00 9b00  .C...s....|.j...
-000015a0: 6401 9d02 7d03 7401 7c01 6402 6403 8d02  d...}.t.|.d.d...
-000015b0: 7d04 7402 8300 8f16 0100 7c00 6a03 6a04  }.t.......|.j.j.
-000015c0: 7c03 7c04 7c00 6a05 7c02 6404 8d01 6402  |.|.|.j.|.d...d.
-000015d0: 6405 8d04 7d05 5700 6400 0400 0400 8303  d...}.W.d.......
-000015e0: 0100 6e08 3100 7328 7701 0100 0100 0100  ..n.1.s(w.......
-000015f0: 5900 0100 7c05 6a06 6406 6701 6407 8d01  Y...|.j.d.g.d...
-00001600: 7d06 7407 6408 6409 8400 7c06 640a 1900  }.t.d.d...|.d...
-00001610: 4400 8301 7c06 640b 1900 640c 8d02 5300  D...|.d...d...S.
-00001620: 290d 4e7a 122f 7631 2f64 6174 6173 6574  ).Nz./v1/dataset
-00001630: 732f 7175 6572 7954 7256 0000 0029 0172  s/queryTrV...).r
-00001640: 2900 0000 7258 0000 0072 3300 0000 7234  )...rX...r3...r4
-00001650: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001660: 0200 0000 0500 0000 5300 0000 725a 0000  ........S...rZ..
-00001670: 0072 2500 0000 2902 7217 0000 0072 3700  .r%...).r....r7.
-00001680: 0000 2902 725b 0000 00da 0764 6174 6173  ..).r[.....datas
-00001690: 6574 7225 0000 0072 2500 0000 7226 0000  etr%...r%...r&..
-000016a0: 0072 5d00 0000 c800 0000 7308 0000 0006  .r].......s.....
-000016b0: 0002 0208 ff06 ff7a 3644 6174 6173 6574  .......z6Dataset
-000016c0: 4874 7470 4465 6c65 6761 7465 2e71 7565  HttpDelegate.que
-000016d0: 7279 5f64 6174 6173 6574 732e 3c6c 6f63  ry_datasets.<loc
-000016e0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-000016f0: 5e00 0000 725f 0000 0072 6000 0000 2908  ^...r_...r`...).
-00001700: 721b 0000 0072 0b00 0000 7206 0000 0072  r....r....r....r
-00001710: 1a00 0000 7236 0000 0072 2b00 0000 7238  ....r6...r+...r8
-00001720: 0000 0072 0800 0000 2907 7222 0000 0072  ...r....).r"...r
-00001730: 6400 0000 7227 0000 0072 3900 0000 da09  d...r'...r9.....
-00001740: 706f 7374 5f62 6f64 79da 0372 6573 7262  post_body..resrb
-00001750: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00001760: 0000 da0e 7175 6572 795f 6461 7461 7365  ....query_datase
-00001770: 7473 b700 0000 7322 0000 000c 050c 0108  ts....s"........
-00001780: 0106 0102 0102 010a 0102 0108 fc1c ff0e  ................
-00001790: 0802 0106 0106 0204 fe06 0406 fb7a 2244  .............z"D
-000017a0: 6174 6173 6574 4874 7470 4465 6c65 6761  atasetHttpDelega
-000017b0: 7465 2e71 7565 7279 5f64 6174 6173 6574  te.query_dataset
-000017c0: 73da 126d 6574 6164 6174 615f 6368 616e  s..metadata_chan
-000017d0: 6765 7365 74da 0a63 6f6e 6469 7469 6f6e  geset..condition
-000017e0: 73da 0a75 7064 6174 6564 5f62 7963 0600  s..updated_byc..
-000017f0: 0000 0000 0000 0000 0000 0900 0000 0800  ................
-00001800: 0000 4300 0000 737e 0000 007c 006a 009b  ..C...s~...|.j..
-00001810: 0064 017c 016a 019b 009d 037d 0674 027c  .d.|.j.....}.t.|
-00001820: 027c 047c 0364 028d 037d 0774 0383 008f  .|.|.d...}.t....
-00001830: 1a01 007c 006a 046a 057c 0674 067c 0764  ...|.j.j.|.t.|.d
-00001840: 0364 048d 027c 00a0 077c 016a 087c 05a1  .d...|...|.j.|..
-00001850: 0264 058d 037d 0857 0064 0004 0004 0083  .d...}.W.d......
-00001860: 0301 006e 0831 0073 3077 0101 0001 0001  ...n.1.s0w......
-00001870: 0059 0001 0074 09a0 0a7c 086a 0b64 0667  .Y...t...|.j.d.g
-00001880: 0164 078d 01a1 0153 0029 084e 723e 0000  .d.....S.).Nr>..
-00001890: 0029 0372 6900 0000 7231 0000 0072 6a00  .).ri...r1...rj.
-000018a0: 0000 5472 5600 0000 7232 0000 0072 3300  ..TrV...r2...r3.
-000018b0: 0000 7234 0000 0029 0c72 1b00 0000 7240  ..r4...).r....r@
-000018c0: 0000 0072 1500 0000 7206 0000 0072 1a00  ...r....r....r..
-000018d0: 0000 7250 0000 0072 0b00 0000 722b 0000  ..rP...r....r+..
-000018e0: 0072 2700 0000 7217 0000 0072 3700 0000  .r'...r....r7...
-000018f0: 7238 0000 0029 0972 2200 0000 723d 0000  r8...).r"...r=..
-00001900: 0072 6900 0000 726a 0000 0072 3100 0000  .ri...rj...r1...
-00001910: 726b 0000 0072 3900 0000 da07 7061 796c  rk...r9.....payl
-00001920: 6f61 6472 3b00 0000 7225 0000 0072 2500  oadr;...r%...r%.
-00001930: 0000 7226 0000 00da 0675 7064 6174 65cf  ..r&.....update.
-00001940: 0000 0073 1c00 0000 1208 0201 0201 0201  ...s............
-00001950: 0201 06fd 0805 0601 0201 0a01 0c01 08fd  ................
-00001960: 1cff 1407 7a1a 4461 7461 7365 7448 7474  ....z.DatasetHtt
-00001970: 7044 656c 6567 6174 652e 7570 6461 7465  pDelegate.update
-00001980: 2903 4e4e 4e72 1f00 0000 2902 4e4e 2904  ).NNNr....).NN).
-00001990: 4e4e 4e4e 2921 da08 5f5f 6e61 6d65 5f5f  NNNN)!..__name__
-000019a0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000019b0: 7175 616c 6e61 6d65 5f5f 7207 0000 00da  qualname__r.....
-000019c0: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
-000019d0: 7261 0000 0072 2100 0000 7203 0000 00da  ra...r!...r.....
-000019e0: 0464 6963 7472 2b00 0000 7216 0000 00da  .dictr+...r.....
-000019f0: 0652 6f62 6f74 6f72 1800 0000 da02 5333  .Robotor......S3
-00001a00: 7202 0000 00da 046c 6973 7472 1700 0000  r......listr....
-00001a10: 723c 0000 0072 4200 0000 7244 0000 0072  r<...rB...rD...r
-00001a20: 0500 0000 7211 0000 0072 4f00 0000 7251  ....r....rO...rQ
-00001a30: 0000 0072 0800 0000 720f 0000 0072 6300  ...r....r....rc.
-00001a40: 0000 720a 0000 0072 6800 0000 720c 0000  ..r....rh...r...
-00001a50: 0072 0d00 0000 726d 0000 00da 0d5f 5f63  .r....rm.....__c
-00001a60: 6c61 7373 6365 6c6c 5f5f 7225 0000 0072  lasscell__r%...r
-00001a70: 2500 0000 7223 0000 0072 2600 0000 7219  %...r#...r&...r.
-00001a80: 0000 001f 0000 0073 e400 0000 0a00 0801  .......s........
-00001a90: 0801 1a02 0207 0201 0201 04fc 0602 02fe  ................
-00001aa0: 0603 02fd 0604 02fc 0a05 0afb 040f 0201  ................
-00001ab0: 0401 0201 0201 0201 0201 04f8 0202 02fe  ................
-00001ac0: 0e03 02fd 0204 02fc 0a05 02fb 0606 02fa  ................
-00001ad0: 0607 02f9 0608 02f8 0209 0af7 121f 020f  ................
-00001ae0: 04fd 0202 02fe 0603 02fd 0204 0afc 0213  ................
-00001af0: 0201 04fb 0202 02fe 0203 02fd 0604 02fc  ................
-00001b00: 0605 02fb 0206 0afa 0217 04ff 0201 02ff  ................
-00001b10: 0201 02ff 0601 02ff 0202 0afe 020f 0201  ................
-00001b20: 0201 0201 04fa 0202 02fe 0603 02fd 0604  ................
-00001b30: 02fc 0a05 02fb 0a06 02fa 0607 0af9 0229  ...............)
-00001b40: 04fd 0202 02fe 0603 02fd 0604 0afc 021b  ................
-00001b50: 0201 0201 0201 04fa 0202 02fe 0603 02fd  ................
-00001b60: 0a04 02fc 0605 02fb 0606 02fa 0207 12f9  ................
-00001b70: 7219 0000 0029 22da 0674 7970 696e 6772  r....)"..typingr
-00001b80: 0200 0000 7203 0000 00da 0c75 726c 6c69  ....r......urlli
-00001b90: 622e 7061 7273 6572 4a00 0000 da04 6175  b.parserJ.....au
-00001ba0: 7468 7205 0000 00da 0a65 7863 6570 7469  thr......excepti
-00001bb0: 6f6e 7372 0600 0000 da04 6874 7470 7207  onsr......httpr.
-00001bc0: 0000 0072 0800 0000 7209 0000 0072 6400  ...r....r....rd.
-00001bd0: 0000 720a 0000 00da 0573 6572 6465 720b  ..r......serder.
-00001be0: 0000 00da 0775 7064 6174 6573 720c 0000  .....updatesr...
-00001bf0: 0072 0d00 0000 da05 6669 6c65 7372 0f00  .r......filesr..
-00001c00: 0000 da08 6465 6c65 6761 7465 7211 0000  ....delegater...
-00001c10: 0072 1200 0000 da0e 6874 7470 5f72 6573  .r......http_res
-00001c20: 6f75 7263 6573 7213 0000 0072 1400 0000  ourcesr....r....
-00001c30: 7215 0000 0072 3d00 0000 7216 0000 0072  r....r=...r....r
-00001c40: 1700 0000 7218 0000 0072 1900 0000 7225  ....r....r....r%
-00001c50: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00001c60: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001c70: 731a 0000 0010 0008 010c 020c 0114 010c  s...............
-00001c80: 050c 0110 010c 0410 0114 0114 0514 07    ...............
+00000360: 1764 1884 045a 1264 1965 0564 0565 1066  .d...Z.d.e.d.e.f
+00000370: 0464 1a64 1b84 045a 1309 0609 0664 3164  .d.d...Z.....d1d
+00000380: 1665 1064 1c65 1464 1d65 0765 0519 0064  .e.d.e.d.e.e...d
+00000390: 1e65 0765 0519 0064 0565 1566 0a64 1f64  .e.e...d.e.f.d.d
+000003a0: 2084 055a 1664 1965 0564 1e65 0564 0564   ..Z.d.e.d.e.d.d
+000003b0: 0666 0664 2164 2284 045a 1709 0609 0609  .f.d!d"..Z......
+000003c0: 0664 3064 1965 0564 2365 0765 0519 0064  .d0d.e.d#e.e...d
+000003d0: 2465 0765 0f65 0519 0019 0064 2565 0765  $e.e.e.....d%e.e
+000003e0: 0f65 0519 0019 0064 0565 1865 1919 0066  .e.....d.e.e...f
+000003f0: 0a64 2664 2784 055a 1a09 0664 3264 2865  .d&d'..Z...d2d(e
+00000400: 1b64 0965 0765 0519 0064 0565 1865 1019  .d.e.e...d.e.e..
+00000410: 0066 0664 2964 2a84 055a 1c09 0609 0609  .f.d)d*..Z......
+00000420: 0609 0664 3364 1665 1064 2b65 0765 1d19  ...d3d.e.d+e.e..
+00000430: 0064 2c65 0765 0f65 1e19 0019 0064 1365  .d,e.e.e.....d.e
+00000440: 0765 0519 0064 2d65 0765 0519 0064 0565  .e...d-e.e...d.e
+00000450: 1066 0c64 2e64 2f84 055a 1f87 0004 005a  .f.d.d/..Z.....Z
+00000460: 2053 0029 34da 1344 6174 6173 6574 4874   S.)4..DatasetHt
+00000470: 7470 4465 6c65 6761 7465 da21 5f44 6174  tpDelegate.!_Dat
+00000480: 6173 6574 4874 7470 4465 6c65 6761 7465  asetHttpDelegate
+00000490: 5f5f 6874 7470 5f63 6c69 656e 74da 2d5f  __http_client.-_
+000004a0: 4461 7461 7365 7448 7474 7044 656c 6567  DatasetHttpDeleg
+000004b0: 6174 655f 5f72 6f62 6f74 6f5f 7365 7276  ate__roboto_serv
+000004c0: 6963 655f 6261 7365 5f75 726c da17 726f  ice_base_url..ro
+000004d0: 626f 746f 5f73 6572 7669 6365 5f62 6173  boto_service_bas
+000004e0: 655f 7572 6cda 0b68 7474 705f 636c 6965  e_url..http_clie
+000004f0: 6e74 da06 7265 7475 726e 4e63 0300 0000  nt..returnNc....
+00000500: 0000 0000 0000 0000 0300 0000 0200 0000  ................
+00000510: 0300 0000 731a 0000 0074 0083 00a0 01a1  ....s....t......
+00000520: 0001 007c 027c 005f 027c 017c 005f 0364  ...|.|._.|.|._.d
+00000530: 0053 00a9 014e 2904 da05 7375 7065 72da  .S...N)...super.
+00000540: 085f 5f69 6e69 745f 5f72 1a00 0000 721b  .__init__r....r.
+00000550: 0000 0029 03da 0473 656c 6672 1c00 0000  ...)...selfr....
+00000560: 721d 0000 00a9 01da 095f 5f63 6c61 7373  r........__class
+00000570: 5f5f a900 faed 2f63 6f64 6562 7569 6c64  __..../codebuild
+00000580: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000590: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
+000005a0: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
+000005b0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
+000005c0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
+000005d0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
+000005e0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
+000005f0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
+00000600: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
+00000610: 746f 2d61 692f 726f 626f 746f 2d68 6f73  to-ai/roboto-hos
+00000620: 7465 642d 6170 702f 7061 636b 6167 6573  ted-app/packages
+00000630: 2f72 6f62 6f74 6f2f 7372 632f 726f 626f  /roboto/src/robo
+00000640: 746f 2f64 6f6d 6169 6e2f 6461 7461 7365  to/domain/datase
+00000650: 7473 2f68 7474 705f 6465 6c65 6761 7465  ts/http_delegate
+00000660: 2e70 7972 2100 0000 2300 0000 7306 0000  .pyr!...#...s...
+00000670: 000a 0106 010a 017a 1c44 6174 6173 6574  .......z.Dataset
+00000680: 4874 7470 4465 6c65 6761 7465 2e5f 5f69  HttpDelegate.__i
+00000690: 6e69 745f 5fda 066f 7267 5f69 64da 0775  nit__..org_id..u
+000006a0: 7365 725f 6964 da11 7265 736f 7572 6365  ser_id..resource
+000006b0: 5f6f 776e 6572 5f69 6463 0400 0000 0000  _owner_idc......
+000006c0: 0000 0000 0000 0400 0000 0600 0000 4300  ..............C.
+000006d0: 0000 7314 0000 0074 007c 017c 027c 0364  ..s....t.|.|.|.d
+000006e0: 0164 0269 0164 038d 0453 0029 044e 7a0c  .d.i.d...S.).Nz.
+000006f0: 436f 6e74 656e 742d 5479 7065 7a10 6170  Content-Typez.ap
+00000700: 706c 6963 6174 696f 6e2f 6a73 6f6e 2904  plication/json).
+00000710: 7227 0000 0072 2800 0000 7229 0000 00da  r'...r(...r)....
+00000720: 1261 6464 6974 696f 6e61 6c5f 6865 6164  .additional_head
+00000730: 6572 7329 0172 0900 0000 2904 7222 0000  ers).r....).r"..
+00000740: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
+00000750: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+00000760: 0768 6561 6465 7273 2800 0000 730c 0000  .headers(...s...
+00000770: 0002 0602 0102 0102 0106 0106 fc7a 1b44  .............z.D
+00000780: 6174 6173 6574 4874 7470 4465 6c65 6761  atasetHttpDelega
+00000790: 7465 2e68 6561 6465 7273 da0d 6164 6d69  te.headers..admi
+000007a0: 6e69 7374 7261 746f 72da 086d 6574 6164  nistrator..metad
+000007b0: 6174 61da 1073 746f 7261 6765 5f6c 6f63  ata..storage_loc
+000007c0: 6174 696f 6eda 0474 6167 73da 0a63 7265  ation..tags..cre
+000007d0: 6174 6564 5f62 79da 0b64 6573 6372 6970  ated_by..descrip
+000007e0: 7469 6f6e 6308 0000 0000 0000 0000 0000  tionc...........
+000007f0: 000b 0000 0008 0000 0043 0000 0073 8e00  .........C...s..
+00000800: 0000 7c00 6a00 9b00 6401 9d02 7d08 7401  ..|.j...d...}.t.
+00000810: 7c01 7c02 6402 7501 720e 7c02 6e01 6900  |.|.d.u.r.|.n.i.
+00000820: 7c03 7c07 7c04 6402 7501 7217 7c04 6e01  |.|.|.d.u.r.|.n.
+00000830: 6700 6403 8d05 7d09 7402 8300 8f17 0100  g.d...}.t.......
+00000840: 7c00 6a03 6a04 7c08 7405 7c09 8301 7c00  |.j.j.|.t.|...|.
+00000850: a006 7c05 7c06 a102 6404 8d03 7d0a 5700  ..|.|...d...}.W.
+00000860: 6402 0400 0400 8303 0100 6e08 3100 7338  d.........n.1.s8
+00000870: 7701 0100 0100 0100 5900 0100 7407 a008  w.......Y...t...
+00000880: 7c0a 6a09 6405 6701 6406 8d01 a101 5300  |.j.d.g.d.....S.
+00000890: 2907 7a27 0a20 2020 2020 2020 2043 7265  ).z'.        Cre
+000008a0: 6174 6520 6120 6e65 7720 6461 7461 7365  ate a new datase
+000008b0: 742e 0a20 2020 2020 2020 207a 0c2f 7631  t..        z./v1
+000008c0: 2f64 6174 6173 6574 734e 2905 722c 0000  /datasetsN).r,..
+000008d0: 0072 2d00 0000 722e 0000 0072 3100 0000  .r-...r....r1...
+000008e0: 722f 0000 00a9 02da 0464 6174 6172 2b00  r/.......datar+.
+000008f0: 0000 7233 0000 00a9 01da 096a 736f 6e5f  ..r3.......json_
+00000900: 7061 7468 290a 721b 0000 0072 1300 0000  path).r....r....
+00000910: 7206 0000 0072 1a00 0000 da04 706f 7374  r....r......post
+00000920: 720b 0000 0072 2b00 0000 7217 0000 00da  r....r+...r.....
+00000930: 0e6d 6f64 656c 5f76 616c 6964 6174 65da  .model_validate.
+00000940: 0966 726f 6d5f 6a73 6f6e 290b 7222 0000  .from_json).r"..
+00000950: 0072 2c00 0000 722d 0000 0072 2e00 0000  .r,...r-...r....
+00000960: 722f 0000 0072 2700 0000 7230 0000 0072  r/...r'...r0...r
+00000970: 3100 0000 da03 7572 6cda 0c72 6571 7565  1.....url..reque
+00000980: 7374 5f62 6f64 79da 0872 6573 706f 6e73  st_body..respons
+00000990: 6572 2500 0000 7225 0000 0072 2600 0000  er%...r%...r&...
+000009a0: da0e 6372 6561 7465 5f64 6174 6173 6574  ..create_dataset
+000009b0: 3500 0000 7320 0000 000c 0d02 0102 010e  5...s ..........
+000009c0: 0102 0102 010e 0106 fb08 0806 0102 0106  ................
+000009d0: 010a 0108 fd1c ff14 077a 2244 6174 6173  .........z"Datas
+000009e0: 6574 4874 7470 4465 6c65 6761 7465 2e63  etHttpDelegate.c
+000009f0: 7265 6174 655f 6461 7461 7365 74da 0672  reate_dataset..r
+00000a00: 6563 6f72 6463 0200 0000 0000 0000 0000  ecordc..........
+00000a10: 0000 0300 0000 0800 0000 4300 0000 7352  ..........C...sR
+00000a20: 0000 007c 006a 009b 0064 017c 016a 019b  ...|.j...d.|.j..
+00000a30: 009d 037d 0274 0283 008f 1301 007c 006a  ...}.t.......|.j
+00000a40: 036a 047c 027c 00a0 05a1 0064 028d 0201  .j.|.|.....d....
+00000a50: 0057 0064 0304 0004 0083 0301 0064 0353  .W.d.........d.S
+00000a60: 0031 0073 2277 0101 0001 0001 0059 0001  .1.s"w.......Y..
+00000a70: 0064 0353 0029 047a 230a 2020 2020 2020  .d.S.).z#.      
+00000a80: 2020 4465 6c65 7465 2061 2064 6174 6173    Delete a datas
+00000a90: 6574 2e0a 2020 2020 2020 2020 fa0d 2f76  et..        ../v
+00000aa0: 312f 6461 7461 7365 7473 2fa9 0172 2b00  1/datasets/..r+.
+00000ab0: 0000 4e29 0672 1b00 0000 da0a 6461 7461  ..N).r......data
+00000ac0: 7365 745f 6964 7206 0000 0072 1a00 0000  set_idr....r....
+00000ad0: da06 6465 6c65 7465 722b 0000 0029 0372  ..deleter+...).r
+00000ae0: 2200 0000 723d 0000 0072 3900 0000 7225  "...r=...r9...r%
+00000af0: 0000 0072 2500 0000 7226 0000 00da 0e64  ...r%...r&.....d
+00000b00: 656c 6574 655f 6461 7461 7365 7454 0000  elete_datasetT..
+00000b10: 0073 0e00 0000 1204 0802 0601 0201 0601  .s..............
+00000b20: 08fe 22ff 7a22 4461 7461 7365 7448 7474  ..".z"DatasetHtt
+00000b30: 7044 656c 6567 6174 652e 6465 6c65 7465  pDelegate.delete
+00000b40: 5f64 6174 6173 6574 7240 0000 0063 0200  _datasetr@...c..
+00000b50: 0000 0000 0000 0000 0000 0400 0000 0800  ................
+00000b60: 0000 4300 0000 735e 0000 007c 006a 009b  ..C...s^...|.j..
+00000b70: 0064 017c 019b 009d 037d 0274 0183 008f  .d.|.....}.t....
+00000b80: 1201 007c 006a 026a 037c 027c 00a0 04a1  ...|.j.j.|.|....
+00000b90: 0064 028d 027d 0357 0064 0304 0004 0083  .d...}.W.d......
+00000ba0: 0301 006e 0831 0073 2077 0101 0001 0001  ...n.1.s w......
+00000bb0: 0059 0001 0074 05a0 067c 036a 0764 0467  .Y...t...|.j.d.g
+00000bc0: 0164 058d 01a1 0153 0029 067a 470a 2020  .d.....S.).zG.  
+00000bd0: 2020 2020 2020 4765 7420 6120 6461 7461        Get a data
+00000be0: 7365 7420 6279 2069 7473 2070 7269 6d61  set by its prima
+00000bf0: 7279 206b 6579 2028 6f72 675f 6964 2c20  ry key (org_id, 
+00000c00: 6461 7461 7365 745f 6964 290a 2020 2020  dataset_id).    
+00000c10: 2020 2020 723e 0000 0072 3f00 0000 4e72      r>...r?...Nr
+00000c20: 3300 0000 7234 0000 0029 0872 1b00 0000  3...r4...).r....
+00000c30: 7206 0000 0072 1a00 0000 da03 6765 7472  r....r......getr
+00000c40: 2b00 0000 7217 0000 0072 3700 0000 7238  +...r....r7...r8
+00000c50: 0000 0029 0472 2200 0000 7240 0000 0072  ...).r"...r@...r
+00000c60: 3900 0000 723b 0000 0072 2500 0000 7225  9...r;...r%...r%
+00000c70: 0000 0072 2600 0000 da11 6765 745f 6461  ...r&.....get_da
+00000c80: 7461 7365 745f 6279 5f69 6460 0000 0073  taset_by_id`...s
+00000c90: 0a00 0000 1007 0802 1601 1cff 1403 7a25  ..............z%
+00000ca0: 4461 7461 7365 7448 7474 7044 656c 6567  DatasetHttpDeleg
+00000cb0: 6174 652e 6765 745f 6461 7461 7365 745f  ate.get_dataset_
+00000cc0: 6279 5f69 64da 0b70 6572 6d69 7373 696f  by_id..permissio
+00000cd0: 6e73 da06 6361 6c6c 6572 da0e 7472 616e  ns..caller..tran
+00000ce0: 7361 6374 696f 6e5f 6964 6305 0000 0000  saction_idc.....
+00000cf0: 0000 0000 0000 0009 0000 0008 0000 0043  ...............C
+00000d00: 0000 0073 9000 0000 6401 7c02 6a00 6901  ...s....d.|.j.i.
+00000d10: 7d05 7401 6a02 a003 7c05 a101 7d06 7c00  }.t.j...|...}.|.
+00000d20: 6a04 9b00 6402 7c01 6a05 9b00 6403 7c06  j...d.|.j...d.|.
+00000d30: 9b00 9d05 7d07 7c04 7220 7c07 6404 7c04  ....}.|.r |.d.|.
+00000d40: 9b00 9d02 3700 7d07 7406 8300 8f13 0100  ....7.}.t.......
+00000d50: 7c00 6a07 a008 7c07 7c00 6a09 7c03 6405  |.j...|.|.j.|.d.
+00000d60: 8d01 a102 7d08 5700 6406 0400 0400 8303  ....}.W.d.......
+00000d70: 0100 6e08 3100 7339 7701 0100 0100 0100  ..n.1.s9w.......
+00000d80: 5900 0100 740a a00b 7c08 6a0c 6407 6701  Y...t...|.j.d.g.
+00000d90: 6408 8d01 a101 5300 2909 7a40 0a20 2020  d.....S.).z@.   
+00000da0: 2020 2020 2047 6574 2074 656d 706f 7261       Get tempora
+00000db0: 7279 2063 7265 6465 6e74 6961 6c73 2074  ry credentials t
+00000dc0: 6f20 6163 6365 7373 2061 2064 6174 6173  o access a datas
+00000dd0: 6574 2e0a 2020 2020 2020 2020 da04 6d6f  et..        ..mo
+00000de0: 6465 723e 0000 007a 0d2f 6372 6564 656e  der>...z./creden
+00000df0: 7469 616c 733f 7a10 2674 7261 6e73 6163  tials?z.&transac
+00000e00: 7469 6f6e 5f69 643d a901 7228 0000 004e  tion_id=..r(...N
+00000e10: 7233 0000 0072 3400 0000 290d da05 7661  r3...r4...)...va
+00000e20: 6c75 65da 0675 726c 6c69 62da 0570 6172  lue..urllib..par
+00000e30: 7365 da09 7572 6c65 6e63 6f64 6572 1b00  se..urlencoder..
+00000e40: 0000 7240 0000 0072 0600 0000 721a 0000  ..r@...r....r...
+00000e50: 0072 4300 0000 722b 0000 0072 1100 0000  .rC...r+...r....
+00000e60: 7237 0000 0072 3800 0000 2909 7222 0000  r7...r8...).r"..
+00000e70: 0072 3d00 0000 7245 0000 0072 4600 0000  .r=...rE...rF...
+00000e80: 7247 0000 00da 0c71 7565 7279 5f70 6172  rG.....query_par
+00000e90: 616d 73da 0a65 6e63 6f64 6564 5f71 7372  ams..encoded_qsr
+00000ea0: 3900 0000 723b 0000 0072 2500 0000 7225  9...r;...r%...r%
+00000eb0: 0000 0072 2600 0000 da19 6765 745f 7465  ...r&.....get_te
+00000ec0: 6d70 6f72 6172 795f 6372 6564 656e 7469  mporary_credenti
+00000ed0: 616c 736e 0000 0073 1200 0000 0a0a 0c01  alsn...s........
+00000ee0: 1801 0402 0e01 0802 1801 1cff 1403 7a2d  ..............z-
+00000ef0: 4461 7461 7365 7448 7474 7044 656c 6567  DatasetHttpDeleg
+00000f00: 6174 652e 6765 745f 7465 6d70 6f72 6172  ate.get_temporar
+00000f10: 795f 6372 6564 656e 7469 616c 7363 0300  y_credentialsc..
+00000f20: 0000 0000 0000 0000 0000 0400 0000 0800  ................
+00000f30: 0000 4300 0000 7358 0000 007c 006a 009b  ..C...sX...|.j..
+00000f40: 0064 017c 019b 0064 027c 029b 0064 039d  .d.|...d.|...d..
+00000f50: 067d 0374 0183 008f 1301 007c 006a 026a  .}.t.......|.j.j
+00000f60: 037c 037c 00a0 04a1 0064 048d 0201 0057  .|.|.....d.....W
+00000f70: 0064 0504 0004 0083 0301 0064 0553 0031  .d.........d.S.1
+00000f80: 0073 2577 0101 0001 0001 0059 0001 0064  .s%w.......Y...d
+00000f90: 0553 0029 067a d10a 2020 2020 2020 2020  .S.).z..        
+00000fa0: 4d61 726b 7320 616e 2075 706c 6f61 6420  Marks an upload 
+00000fb0: 6173 2027 636f 6d70 6c65 7465 6427 2c20  as 'completed', 
+00000fc0: 7768 6963 6820 616c 6c6f 7773 2074 6865  which allows the
+00000fd0: 2052 6f62 6f74 6f20 506c 6174 666f 726d   Roboto Platform
+00000fe0: 2074 6f20 6576 616c 7561 7465 2074 7269   to evaluate tri
+00000ff0: 6767 6572 7320 666f 7220 6175 746f 6d61  ggers for automa
+00001000: 7469 6320 6163 7469 6f6e 206f 6e0a 2020  tic action on.  
+00001010: 2020 2020 2020 696e 636f 6d69 6e67 2064        incoming d
+00001020: 6174 612e 2054 6869 7320 616c 736f 2061  ata. This also a
+00001030: 6964 6573 2072 6570 6f72 7469 6e67 206f  ides reporting o
+00001040: 6e20 7061 7274 6961 6c20 7570 6c6f 6164  n partial upload
+00001050: 2066 6169 6c75 7265 2063 6173 6573 2e0a   failure cases..
+00001060: 2020 2020 2020 2020 723e 0000 007a 092f          r>...z./
+00001070: 7570 6c6f 6164 732f 7a09 2f63 6f6d 706c  uploads/z./compl
+00001080: 6574 6529 0272 3900 0000 722b 0000 004e  ete).r9...r+...N
+00001090: 2905 721b 0000 0072 0600 0000 721a 0000  ).r....r....r...
+000010a0: 00da 0370 7574 722b 0000 0029 0472 2200  ...putr+...).r".
+000010b0: 0000 7240 0000 0072 4700 0000 7239 0000  ..r@...rG...r9..
+000010c0: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+000010d0: da0f 636f 6d70 6c65 7465 5f75 706c 6f61  ..complete_uploa
+000010e0: 6484 0000 0073 0800 0000 1805 0802 1601  d....s..........
+000010f0: 22ff 7a23 4461 7461 7365 7448 7474 7044  ".z#DatasetHttpD
+00001100: 656c 6567 6174 652e 636f 6d70 6c65 7465  elegate.complete
+00001110: 5f75 706c 6f61 64da 0a70 6167 655f 746f  _upload..page_to
+00001120: 6b65 6eda 1069 6e63 6c75 6465 5f70 6174  ken..include_pat
+00001130: 7465 726e 73da 1065 7863 6c75 6465 5f70  terns..exclude_p
+00001140: 6174 7465 726e 7363 0500 0000 0000 0000  atternsc........
+00001150: 0000 0000 0a00 0000 0800 0000 4300 0000  ............C...
+00001160: 73b8 0000 007c 006a 009b 0064 017c 019b  s....|.j...d.|..
+00001170: 0064 029d 047d 057c 0272 1c74 016a 02a0  .d...}.|.r.t.j..
+00001180: 0364 0374 047c 0283 0169 01a1 017d 067c  .d.t.|...i...}.|
+00001190: 059b 0064 047c 069b 009d 037d 0574 057c  ...d.|.....}.t.|
+000011a0: 027c 037c 0464 058d 037d 0774 0683 008f  .|.|.d...}.t....
+000011b0: 1801 007c 006a 076a 087c 0574 097c 0764  ...|.j.j.|.t.|.d
+000011c0: 0664 078d 027c 00a0 0aa1 0064 0664 088d  .d...|.....d.d..
+000011d0: 047d 0857 0064 0904 0004 0083 0301 006e  .}.W.d.........n
+000011e0: 0831 0073 4177 0101 0001 0001 0059 0001  .1.sAw.......Y..
+000011f0: 007c 086a 0b64 0a67 0164 0b8d 017d 0974  .|.j.d.g.d...}.t
+00001200: 0c64 0c64 0d84 007c 0964 0e19 0044 0083  .d.d...|.d...D..
+00001210: 017c 0964 0f19 0064 108d 0253 0029 117a  .|.d...d...S.).z
+00001220: e80a 2020 2020 2020 2020 4c69 7374 2066  ..        List f
+00001230: 696c 6573 2061 7373 6f63 6961 7465 6420  iles associated 
+00001240: 7769 7468 2064 6174 6173 6574 2e0a 0a20  with dataset... 
+00001250: 2020 2020 2020 2046 696c 6573 2061 7265         Files are
+00001260: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+00001270: 2064 6174 6173 6574 7320 696e 2061 6e20   datasets in an 
+00001280: 6576 656e 7475 616c 6c79 2d63 6f6e 7369  eventually-consi
+00001290: 7374 656e 7420 6d61 6e6e 6572 2c0a 2020  stent manner,.  
+000012a0: 2020 2020 2020 736f 2074 6865 7265 2077        so there w
+000012b0: 696c 6c20 6c69 6b65 6c79 2062 6520 6465  ill likely be de
+000012c0: 6c61 7920 6265 7477 6565 6e20 6120 6669  lay between a fi
+000012d0: 6c65 2062 6569 6e67 2075 706c 6f61 6465  le being uploade
+000012e0: 6420 616e 6420 6974 2061 7070 6561 7269  d and it appeari
+000012f0: 6e67 2069 6e20 7468 6973 206c 6973 742e  ng in this list.
+00001300: 0a20 2020 2020 2020 2072 3e00 0000 7a0c  .        r>...z.
+00001310: 2f66 696c 6573 2f71 7565 7279 7253 0000  /files/queryrS..
+00001320: 00da 013f 2903 7253 0000 0072 5400 0000  ...?).rS...rT...
+00001330: 7255 0000 0054 a901 da0c 6578 636c 7564  rU...T....exclud
+00001340: 655f 6e6f 6e65 a903 7233 0000 0072 2b00  e_none..r3...r+.
+00001350: 0000 da0a 6964 656d 706f 7465 6e74 4e72  ....idempotentNr
+00001360: 3300 0000 7234 0000 0063 0100 0000 0000  3...r4...c......
+00001370: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
+00001380: 0000 f316 0000 0067 007c 005d 077d 0174  .......g.|.].}.t
+00001390: 00a0 017c 01a1 0191 0271 0253 0072 2500  ...|.....q.S.r%.
+000013a0: 0000 2902 720f 0000 0072 3700 0000 2902  ..).r....r7...).
+000013b0: da02 2e30 da04 6669 6c65 7225 0000 0072  ...0..filer%...r
+000013c0: 2500 0000 7226 0000 00da 0a3c 6c69 7374  %...r&.....<list
+000013d0: 636f 6d70 3eaf 0000 0073 0200 0000 1600  comp>....s......
+000013e0: 7a32 4461 7461 7365 7448 7474 7044 656c  z2DatasetHttpDel
+000013f0: 6567 6174 652e 6c69 7374 5f66 696c 6573  egate.list_files
+00001400: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00001410: 6f6d 703e da05 6974 656d 73da 0a6e 6578  omp>..items..nex
+00001420: 745f 746f 6b65 6ea9 0272 5f00 0000 7260  t_token..r_...r`
+00001430: 0000 0029 0d72 1b00 0000 724b 0000 0072  ...).r....rK...r
+00001440: 4c00 0000 724d 0000 00da 0373 7472 7214  L...rM.....strr.
+00001450: 0000 0072 0600 0000 721a 0000 0072 3600  ...r....r....r6.
+00001460: 0000 720b 0000 0072 2b00 0000 7238 0000  ..r....r+...r8..
+00001470: 0072 0800 0000 290a 7222 0000 0072 4000  .r....).r"...r@.
+00001480: 0000 7253 0000 0072 5400 0000 7255 0000  ..rS...rT...rU..
+00001490: 0072 3900 0000 724f 0000 0072 3a00 0000  .r9...rO...r:...
+000014a0: 723b 0000 00da 0c75 6e6d 6172 7368 616c  r;.....unmarshal
+000014b0: 6c65 6472 2500 0000 7225 0000 0072 2600  ledr%...r%...r&.
+000014c0: 0000 da0a 6c69 7374 5f66 696c 6573 8e00  ....list_files..
+000014d0: 0000 732c 0000 0012 0d04 0114 010e 0102  ..s,............
+000014e0: 0202 0102 0102 0106 fd08 0506 0102 010a  ................
+000014f0: 0106 0102 0108 fc1c ff0e 0802 0110 0106  ................
+00001500: 0106 fe7a 1e44 6174 6173 6574 4874 7470  ...z.DatasetHttp
+00001510: 4465 6c65 6761 7465 2e6c 6973 745f 6669  Delegate.list_fi
+00001520: 6c65 73da 0571 7565 7279 6303 0000 0000  les..queryc.....
+00001530: 0000 0000 0000 0007 0000 0008 0000 0043  ...............C
+00001540: 0000 0073 8600 0000 7c00 6a00 9b00 6401  ...s....|.j...d.
+00001550: 9d02 7d03 7401 7c01 6402 6403 8d02 7d04  ..}.t.|.d.d...}.
+00001560: 7402 8300 8f16 0100 7c00 6a03 6a04 7c03  t.......|.j.j.|.
+00001570: 7c04 7c00 6a05 7c02 6404 8d01 6402 6405  |.|.j.|.d...d.d.
+00001580: 8d04 7d05 5700 6400 0400 0400 8303 0100  ..}.W.d.........
+00001590: 6e08 3100 7328 7701 0100 0100 0100 5900  n.1.s(w.......Y.
+000015a0: 0100 7c05 6a06 6406 6701 6407 8d01 7d06  ..|.j.d.g.d...}.
+000015b0: 7407 6408 6409 8400 7c06 640a 1900 4400  t.d.d...|.d...D.
+000015c0: 8301 7c06 640b 1900 640c 8d02 5300 290d  ..|.d...d...S.).
+000015d0: 4e7a 122f 7631 2f64 6174 6173 6574 732f  Nz./v1/datasets/
+000015e0: 7175 6572 7954 7257 0000 0029 0172 2900  queryTrW...).r).
+000015f0: 0000 7259 0000 0072 3300 0000 7234 0000  ..rY...r3...r4..
+00001600: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001610: 0000 0500 0000 5300 0000 725b 0000 0072  ......S...r[...r
+00001620: 2500 0000 2902 7217 0000 0072 3700 0000  %...).r....r7...
+00001630: 2902 725c 0000 00da 0764 6174 6173 6574  ).r\.....dataset
+00001640: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
+00001650: 5e00 0000 c400 0000 7308 0000 0006 0002  ^.......s.......
+00001660: 0208 ff06 ff7a 3644 6174 6173 6574 4874  .....z6DatasetHt
+00001670: 7470 4465 6c65 6761 7465 2e71 7565 7279  tpDelegate.query
+00001680: 5f64 6174 6173 6574 732e 3c6c 6f63 616c  _datasets.<local
+00001690: 733e 2e3c 6c69 7374 636f 6d70 3e72 5f00  s>.<listcomp>r_.
+000016a0: 0000 7260 0000 0072 6100 0000 2908 721b  ..r`...ra...).r.
+000016b0: 0000 0072 0b00 0000 7206 0000 0072 1a00  ...r....r....r..
+000016c0: 0000 7236 0000 0072 2b00 0000 7238 0000  ..r6...r+...r8..
+000016d0: 0072 0800 0000 2907 7222 0000 0072 6500  .r....).r"...re.
+000016e0: 0000 7227 0000 0072 3900 0000 da09 706f  ..r'...r9.....po
+000016f0: 7374 5f62 6f64 79da 0372 6573 7263 0000  st_body..resrc..
+00001700: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+00001710: da0e 7175 6572 795f 6461 7461 7365 7473  ..query_datasets
+00001720: b300 0000 7322 0000 000c 050c 0108 0106  ....s"..........
+00001730: 0102 0102 010a 0102 0108 fc1c ff0e 0802  ................
+00001740: 0106 0106 0204 fe06 0406 fb7a 2244 6174  ...........z"Dat
+00001750: 6173 6574 4874 7470 4465 6c65 6761 7465  asetHttpDelegate
+00001760: 2e71 7565 7279 5f64 6174 6173 6574 73da  .query_datasets.
+00001770: 126d 6574 6164 6174 615f 6368 616e 6765  .metadata_change
+00001780: 7365 74da 0a63 6f6e 6469 7469 6f6e 73da  set..conditions.
+00001790: 0a75 7064 6174 6564 5f62 7963 0600 0000  .updated_byc....
+000017a0: 0000 0000 0000 0000 0900 0000 0800 0000  ................
+000017b0: 4300 0000 737c 0000 007c 006a 009b 0064  C...s|...|.j...d
+000017c0: 017c 016a 019b 009d 037d 0674 027c 027c  .|.j.....}.t.|.|
+000017d0: 047c 0364 028d 037d 0774 0383 008f 1901  .|.d...}.t......
+000017e0: 007c 006a 046a 057c 0674 067c 0764 0364  .|.j.j.|.t.|.d.d
+000017f0: 048d 027c 006a 077c 0564 058d 0164 068d  ...|.j.|.d...d..
+00001800: 037d 0857 0064 0004 0004 0083 0301 006e  .}.W.d.........n
+00001810: 0831 0073 2f77 0101 0001 0001 0059 0001  .1.s/w.......Y..
+00001820: 0074 08a0 097c 086a 0a64 0767 0164 088d  .t...|.j.d.g.d..
+00001830: 01a1 0153 0029 094e 723e 0000 0029 0372  ...S.).Nr>...).r
+00001840: 6a00 0000 7231 0000 0072 6b00 0000 5472  j...r1...rk...Tr
+00001850: 5700 0000 7249 0000 0072 3200 0000 7233  W...rI...r2...r3
+00001860: 0000 0072 3400 0000 290b 721b 0000 0072  ...r4...).r....r
+00001870: 4000 0000 7215 0000 0072 0600 0000 721a  @...r....r....r.
+00001880: 0000 0072 5100 0000 720b 0000 0072 2b00  ...rQ...r....r+.
+00001890: 0000 7217 0000 0072 3700 0000 7238 0000  ..r....r7...r8..
+000018a0: 0029 0972 2200 0000 723d 0000 0072 6a00  .).r"...r=...rj.
+000018b0: 0000 726b 0000 0072 3100 0000 726c 0000  ..rk...r1...rl..
+000018c0: 0072 3900 0000 da07 7061 796c 6f61 6472  .r9.....payloadr
+000018d0: 3b00 0000 7225 0000 0072 2500 0000 7226  ;...r%...r%...r&
+000018e0: 0000 00da 0675 7064 6174 65cb 0000 0073  .....update....s
+000018f0: 1c00 0000 1208 0201 0201 0201 0201 06fd  ................
+00001900: 0805 0601 0201 0a01 0a01 08fd 1cff 1407  ................
+00001910: 7a1a 4461 7461 7365 7448 7474 7044 656c  z.DatasetHttpDel
+00001920: 6567 6174 652e 7570 6461 7465 2903 4e4e  egate.update).NN
+00001930: 4e29 024e 4e72 1f00 0000 2904 4e4e 4e4e  N).NNr....).NNNN
+00001940: 2921 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )!..__name__..__
+00001950: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00001960: 6e61 6d65 5f5f 7207 0000 00da 0f5f 5f61  name__r......__a
+00001970: 6e6e 6f74 6174 696f 6e73 5f5f 7262 0000  nnotations__rb..
+00001980: 0072 2100 0000 7203 0000 00da 0464 6963  .r!...r......dic
+00001990: 7472 2b00 0000 7216 0000 00da 0652 6f62  tr+...r......Rob
+000019a0: 6f74 6f72 1800 0000 da02 5333 7202 0000  otor......S3r...
+000019b0: 00da 046c 6973 7472 1700 0000 723c 0000  ...listr....r<..
+000019c0: 0072 4200 0000 7244 0000 0072 0500 0000  .rB...rD...r....
+000019d0: 7211 0000 0072 5000 0000 7252 0000 0072  r....rP...rR...r
+000019e0: 0800 0000 720f 0000 0072 6400 0000 720a  ....r....rd...r.
+000019f0: 0000 0072 6900 0000 720c 0000 0072 0d00  ...ri...r....r..
+00001a00: 0000 726e 0000 00da 0d5f 5f63 6c61 7373  ..rn.....__class
+00001a10: 6365 6c6c 5f5f 7225 0000 0072 2500 0000  cell__r%...r%...
+00001a20: 7223 0000 0072 2600 0000 7219 0000 001f  r#...r&...r.....
+00001a30: 0000 0073 c600 0000 0a00 0801 0801 1a02  ...s............
+00001a40: 0207 0201 0201 04fc 0602 02fe 0603 02fd  ................
+00001a50: 0604 02fc 0a05 0afb 040f 0201 0401 0201  ................
+00001a60: 0201 0201 0201 04f8 0202 02fe 0e03 02fd  ................
+00001a70: 0204 02fc 0a05 02fb 0606 02fa 0607 02f9  ................
+00001a80: 0608 02f8 0209 0af7 121f 020c 0202 02fe  ................
+00001a90: 0203 0afd 0212 0201 04fb 0202 02fe 0203  ................
+00001aa0: 02fd 0604 02fc 0605 02fb 0206 0afa 1616  ................
+00001ab0: 020d 0201 0201 04fb 0202 02fe 0603 02fd  ................
+00001ac0: 0a04 02fc 0a05 02fb 0606 0afa 0228 04fd  .............(..
+00001ad0: 0202 02fe 0603 02fd 0604 0afc 021b 0201  ................
+00001ae0: 0201 0201 04fa 0202 02fe 0603 02fd 0a04  ................
+00001af0: 02fc 0605 02fb 0606 02fa 0207 12f9 7219  ..............r.
+00001b00: 0000 0029 22da 0674 7970 696e 6772 0200  ...)"..typingr..
+00001b10: 0000 7203 0000 00da 0c75 726c 6c69 622e  ..r......urllib.
+00001b20: 7061 7273 6572 4b00 0000 da04 6175 7468  parserK.....auth
+00001b30: 7205 0000 00da 0a65 7863 6570 7469 6f6e  r......exception
+00001b40: 7372 0600 0000 da04 6874 7470 7207 0000  sr......httpr...
+00001b50: 0072 0800 0000 7209 0000 0072 6500 0000  .r....r....re...
+00001b60: 720a 0000 00da 0573 6572 6465 720b 0000  r......serder...
+00001b70: 00da 0775 7064 6174 6573 720c 0000 0072  ...updatesr....r
+00001b80: 0d00 0000 da05 6669 6c65 7372 0f00 0000  ......filesr....
+00001b90: da08 6465 6c65 6761 7465 7211 0000 0072  ..delegater....r
+00001ba0: 1200 0000 da0e 6874 7470 5f72 6573 6f75  ......http_resou
+00001bb0: 7263 6573 7213 0000 0072 1400 0000 7215  rcesr....r....r.
+00001bc0: 0000 0072 3d00 0000 7216 0000 0072 1700  ...r=...r....r..
+00001bd0: 0000 7218 0000 0072 1900 0000 7225 0000  ..r....r....r%..
+00001be0: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+00001bf0: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
+00001c00: 0000 0010 0008 010c 020c 0114 010c 050c  ................
+00001c10: 0110 010c 0410 0114 0114 0514 07         .............
```

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/__pycache__/http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/datasets/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1089 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4104 0000  o........Y.eA...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 4104 0000  o.......2H.eA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c01 6d02 5a02 0100 6403 6404 6c03  d.l.m.Z...d.d.l.
 00000050: 6d04 5a04 6d05 5a05 0100 6405 6406 6c06  m.Z.m.Z...d.d.l.
 00000060: 6d07 5a07 6d08 5a08 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
 00000070: 8400 6408 6501 6a09 8303 5a0a 4700 6409  ..d.e.j...Z.G.d.
@@ -37,16 +37,16 @@
 00000240: 6174 696f 6e73 5f5f 7208 0000 0072 0c00  ations__r....r..
 00000250: 0000 da06 7479 7069 6e67 da08 4f70 7469  ....typing..Opti
 00000260: 6f6e 616c da03 7374 72da 0870 7964 616e  onal..str..pydan
 00000270: 7469 63da 0546 6965 6c64 da04 6469 6374  tic..Field..dict
 00000280: 720f 0000 00da 0341 6e79 da04 6c69 7374  r......Any..list
 00000290: 7210 0000 00a9 0072 1d00 0000 721d 0000  r......r....r...
 000002a0: 00fa ee2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-000002b0: 7470 7574 2f73 7263 3130 3531 3138 3230  tput/src10511820
-000002c0: 3839 2f73 7263 2f63 6f64 6573 7461 722d  89/src/codestar-
+000002b0: 7470 7574 2f73 7263 3330 3739 3233 3632  tput/src30792362
+000002c0: 3634 2f73 7263 2f63 6f64 6573 7461 722d  64/src/codestar-
 000002d0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000002e0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000002f0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 00000300: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 00000310: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 00000320: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000330: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/__pycache__/record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/datasets/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1239 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 d704 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 d704 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a05 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000060: 6506 6501 6a07 8304 5a08 4700 6405 6406  e.e.j...Z.G.d.d.
 00000070: 8400 6406 6506 6501 6a07 8304 5a09 4700  ..d.e.e.j...Z.G.
@@ -14,15 +14,15 @@
 000000d0: 005a 0264 015a 0364 0253 0029 03da 0d41  .Z.d.Z.d.S.)...A
 000000e0: 646d 696e 6973 7472 6174 6f72 da06 526f  dministrator..Ro
 000000f0: 626f 746f 4e29 04da 085f 5f6e 616d 655f  botoN)...__name_
 00000100: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000110: 5f71 7561 6c6e 616d 655f 5f72 0600 0000  _qualname__r....
 00000120: a900 720a 0000 0072 0a00 0000 fae6 2f63  ..r....r....../c
 00000130: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000140: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+00000140: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 00000150: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 00000160: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 00000170: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 00000180: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 00000190: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 000001a0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 000001b0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/dataset.py` & `roboto-0.2.9/src/roboto/domain/datasets/dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import collections.abc
 import dataclasses
 import importlib.metadata
 import os
 import pathlib
 import time
-from typing import Any, Callable, Optional
+import typing
 
 import pathspec
 
 from ...auth import Permissions
+from ...exceptions import (
+    RobotoInvalidRequestException,
+    RobotoNotFoundException,
+)
 from ...logging import default_logger
 from ...query import QuerySpecification
 from ...serde import pydantic_jsonable_dict
 from ...transactions import (
     TransactionManagerABC,
     TransactionRecord,
     TransactionType,
@@ -50,30 +54,30 @@
     transaction_id: str
 
 
 class Dataset:
     __dataset_delegate: DatasetDelegate
     __file_delegate: FileDelegate
     __record: DatasetRecord
-    __temp_credentials: Optional[Credentials] = None
+    __temp_credentials: typing.Optional[Credentials] = None
     __transaction_manager: TransactionManagerABC
 
     @classmethod
     def create(
         cls,
         dataset_delegate: DatasetDelegate,
         file_delegate: FileDelegate,
         transaction_manager: TransactionManagerABC,
         administrator: Administrator = Administrator.Roboto,
         storage_location: StorageLocation = StorageLocation.S3,
-        org_id: Optional[str] = None,
-        created_by: Optional[str] = None,
-        metadata: Optional[dict[str, Any]] = None,
-        tags: Optional[list[str]] = None,
-        description: Optional[str] = None,
+        org_id: typing.Optional[str] = None,
+        created_by: typing.Optional[str] = None,
+        metadata: typing.Optional[dict[str, typing.Any]] = None,
+        tags: typing.Optional[list[str]] = None,
+        description: typing.Optional[str] = None,
     ) -> "Dataset":
         record = dataset_delegate.create_dataset(
             administrator,
             metadata,
             storage_location,
             tags,
             org_id,
@@ -85,27 +89,26 @@
     @classmethod
     def from_id(
         cls,
         dataset_id: str,
         dataset_delegate: DatasetDelegate,
         file_delegate: FileDelegate,
         transaction_manager: TransactionManagerABC,
-        org_id: Optional[str] = None,
     ) -> "Dataset":
-        record = dataset_delegate.get_dataset_by_primary_key(dataset_id, org_id)
+        record = dataset_delegate.get_dataset_by_id(dataset_id)
         return cls(record, dataset_delegate, file_delegate, transaction_manager)
 
     @classmethod
     def query(
         cls,
         query: QuerySpecification,
         dataset_delegate: DatasetDelegate,
         file_delegate: FileDelegate,
         transaction_manager: TransactionManagerABC,
-        org_id: Optional[str] = None,
+        org_id: typing.Optional[str] = None,
     ) -> collections.abc.Generator["Dataset", None, None]:
         known = set(DatasetRecord.model_fields.keys())
         actual = set()
         for field in query.fields():
             # Support dot notation for nested fields
             # E.g., "metadata.SoftwareVersion"
             if "." in field:
@@ -147,29 +150,29 @@
         self.__transaction_manager = transaction_manager
 
     @property
     def dataset_id(self) -> str:
         return self.__record.dataset_id
 
     @property
-    def metadata(self) -> dict[str, Any]:
+    def metadata(self) -> dict[str, typing.Any]:
         return self.__record.metadata.copy()
 
     @property
     def record(self) -> DatasetRecord:
         return self.__record
 
     @property
     def tags(self) -> list[str]:
         return self.__record.tags.copy()
 
     def complete_upload(
         self,
         transaction_id: str,
-        caller: Optional[str] = None,  # A Roboto user_id
+        caller: typing.Optional[str] = None,  # A Roboto user_id
         timeout: int = 300,
     ) -> None:
         """
         Marks an upload as 'completed', which allows the Roboto Platform to evaluate triggers for automatic action on
         incoming data. This also aides reporting on partial upload failure cases.
 
         This API is called implicitly by the `upload_file` and `upload_directory` operations, and should only be
@@ -187,24 +190,23 @@
                 raise TimeoutError("Timed out waiting for upload to complete.")
             if iteration > 0:
                 time.sleep(min((2**iteration) / 2, 16))
 
         self.__dataset_delegate.complete_upload(
             dataset_id=self.__record.dataset_id,
             transaction_id=transaction_id,
-            org_id=self.__record.org_id,
         )
 
     def delete_dataset(self) -> None:
         self.__dataset_delegate.delete_dataset(self.__record)
 
     def delete_files(
         self,
-        include_patterns: Optional[list[str]] = None,
-        exclude_patterns: Optional[list[str]] = None,
+        include_patterns: typing.Optional[list[str]] = None,
+        exclude_patterns: typing.Optional[list[str]] = None,
     ) -> None:
         """
         Delete files associated with this dataset.
 
         `include_patterns` and `exclude_patterns` are lists of gitignore-style patterns.
         See https://git-scm.com/docs/gitignore.
 
@@ -219,16 +221,16 @@
         """
         for file in self.list_files(include_patterns, exclude_patterns):
             file.delete()
 
     def download_files(
         self,
         out_path: pathlib.Path,
-        include_patterns: Optional[list[str]] = None,
-        exclude_patterns: Optional[list[str]] = None,
+        include_patterns: typing.Optional[list[str]] = None,
+        exclude_patterns: typing.Optional[list[str]] = None,
     ) -> None:
         """
         Download files associated with this dataset to the given directory.
         If `out_path` does not exist, it will be created.
 
         `include_patterns` and `exclude_patterns` are lists of gitignore-style patterns.
         See https://git-scm.com/docs/gitignore.
@@ -279,36 +281,63 @@
                     "base_path": self.__record.dataset_id,
                     "total_file_count": len(all_files),
                 },
             ),
             max_concurrency=8,
         )
 
+    def get_file_info(
+        self,
+        relative_path: typing.Union[str, pathlib.Path],
+    ) -> File:
+        """
+        Get a File object for the given relative path.
+
+        Example:
+            >>> from roboto.domain import datasets
+            >>> dataset = datasets.Dataset(...)
+            >>> file = dataset.get_file_info("foo/bar.txt")
+            >>> print(file.file_id)
+            file-abc123
+        """
+        matching = list(self.list_files(include_patterns=[str(relative_path)]))
+        if not matching:
+            raise RobotoNotFoundException(
+                f"File '{relative_path}' not found in dataset '{self.dataset_id}'"
+            )
+
+        if len(matching) > 1:
+            raise RobotoInvalidRequestException(
+                f"Multiple files found for '{relative_path}' in dataset '{self.dataset_id}'"
+            )
+
+        return matching[0]
+
     def get_temporary_credentials(
         self,
         permissions: Permissions = Permissions.ReadOnly,
-        caller: Optional[str] = None,  # A Roboto user_id
+        caller: typing.Optional[str] = None,  # A Roboto user_id
         force_refresh: bool = False,
-        transaction_id: Optional[str] = None,
+        transaction_id: typing.Optional[str] = None,
     ) -> Credentials:
         if (
             force_refresh
             or permissions == Permissions.ReadWrite
             or self.__temp_credentials is None
             or self.__temp_credentials.is_expired()
         ):
             self.__temp_credentials = self.__dataset_delegate.get_temporary_credentials(
                 self.__record, permissions, caller, transaction_id
             )
         return self.__temp_credentials
 
     def list_files(
         self,
-        include_patterns: Optional[list[str]] = None,
-        exclude_patterns: Optional[list[str]] = None,
+        include_patterns: typing.Optional[list[str]] = None,
+        exclude_patterns: typing.Optional[list[str]] = None,
     ) -> collections.abc.Generator[File, None, None]:
         """
         List files associated with this dataset.
 
         `include_patterns` and `exclude_patterns` are lists of gitignore-style patterns.
         See https://git-scm.com/docs/gitignore.
 
@@ -320,36 +349,34 @@
             ...     exclude_patterns=["**/test/**"]
             ... ):
             ...     print(file.relative_path)
         """
 
         paginated_results = self.__dataset_delegate.list_files(
             self.__record.dataset_id,
-            self.__record.org_id,
             include_patterns=include_patterns,
             exclude_patterns=exclude_patterns,
         )
         while True:
             for record in paginated_results.items:
                 yield File(record, self.__file_delegate)
             if paginated_results.next_token:
                 paginated_results = self.__dataset_delegate.list_files(
                     self.__record.dataset_id,
-                    self.__record.org_id,
                     paginated_results.next_token,
                     include_patterns=include_patterns,
                     exclude_patterns=exclude_patterns,
                 )
             else:
                 break
 
     def put_metadata(
         self,
-        metadata: dict[str, Any],
-        updated_by: Optional[str] = None,  # A Roboto user_id
+        metadata: dict[str, typing.Any],
+        updated_by: typing.Optional[str] = None,  # A Roboto user_id
     ) -> None:
         """
         Set each `key`: `value` in this dict as dataset metadata if it doesn't exist, else overwrite the existing value.
         Keys must be strings. Dot notation is supported for nested keys.
 
         Example:
             >>> from roboto.domain import datasets
@@ -364,32 +391,32 @@
             metadata_changeset=MetadataChangeset(put_fields=metadata),
             updated_by=updated_by,
         )
 
     def put_tags(
         self,
         tags: StrSequence,
-        updated_by: Optional[str] = None,  # A Roboto user_id
+        updated_by: typing.Optional[str] = None,  # A Roboto user_id
     ) -> None:
         """Add each tag in this sequence if it doesn't exist"""
         self.update(
             metadata_changeset=MetadataChangeset(put_tags=tags),
             updated_by=updated_by,
         )
 
     def refresh(self) -> None:
         """Refresh the underlying dataset record with the latest server state."""
-        self.__record = self.__dataset_delegate.get_dataset_by_primary_key(
-            self.__record.dataset_id, self.__record.org_id
+        self.__record = self.__dataset_delegate.get_dataset_by_id(
+            self.__record.dataset_id
         )
 
     def remove_metadata(
         self,
         metadata: StrSequence,
-        updated_by: Optional[str] = None,  # A Roboto user_id
+        updated_by: typing.Optional[str] = None,  # A Roboto user_id
     ) -> None:
         """
         Remove each key in this sequence from dataset metadata if it exists.
         Keys must be strings. Dot notation is supported for nested keys.
 
         Example:
             >>> from roboto.domain import datasets
@@ -400,29 +427,29 @@
             metadata_changeset=MetadataChangeset(remove_fields=metadata),
             updated_by=updated_by,
         )
 
     def remove_tags(
         self,
         tags: StrSequence,
-        updated_by: Optional[str] = None,  # A Roboto user_id
+        updated_by: typing.Optional[str] = None,  # A Roboto user_id
     ) -> None:
         """Remove each tag in this sequence if it exists"""
         self.update(
             metadata_changeset=MetadataChangeset(remove_tags=tags),
             updated_by=updated_by,
         )
 
-    def to_dict(self) -> dict[str, Any]:
+    def to_dict(self) -> dict[str, typing.Any]:
         return pydantic_jsonable_dict(self.__record)
 
     def upload_directory(
         self,
         directory_path: pathlib.Path,
-        exclude_patterns: Optional[list[str]] = None,
+        exclude_patterns: typing.Optional[list[str]] = None,
         timeout: int = 300,
     ) -> None:
         """
         Upload everything, recursively, in directory, ignoring files that match any of the ignore patterns.
 
         `exclude_patterns` is a list of gitignore-style patterns.
         See https://git-scm.com/docs/gitignore#_pattern_format.
@@ -439,15 +466,15 @@
             ...         "**/*.log",
             ...     ],
             ... )
         """
         if not directory_path.is_dir():
             raise ValueError(f"{directory_path} is not a directory")
 
-        exclude_spec: Optional[pathspec.PathSpec] = None
+        exclude_spec: typing.Optional[pathspec.PathSpec] = None
         if exclude_patterns is not None:
             exclude_spec = pathspec.GitIgnoreSpec.from_lines(
                 exclude_patterns,
             )
 
         expected_file_count = 0
         expected_file_size = 0
@@ -519,16 +546,16 @@
 
         self.complete_upload(transaction.transaction_id, timeout=timeout)
 
     def upload_file(
         self,
         local_file_path: pathlib.Path,
         key: str,
-        credentials: Optional[Credentials] = None,
-        credential_provider: Optional[Callable[[], S3Credentials]] = None,
+        credentials: typing.Optional[Credentials] = None,
+        credential_provider: typing.Optional[typing.Callable[[], S3Credentials]] = None,
     ) -> FileUploadInfo:
         """
         Uploads a single file to the dataset's storage location.
         """
         transaction = self.__start_transaction(expected_file_count=1)
 
         upload_info = self.__upload_file(
@@ -541,18 +568,18 @@
 
         self.complete_upload(transaction.transaction_id)
 
         return upload_info
 
     def update(
         self,
-        metadata_changeset: Optional[MetadataChangeset] = None,
-        conditions: Optional[list[UpdateCondition]] = None,
-        description: Optional[str] = None,
-        updated_by: Optional[str] = None,  # A Roboto user_id
+        metadata_changeset: typing.Optional[MetadataChangeset] = None,
+        conditions: typing.Optional[list[UpdateCondition]] = None,
+        description: typing.Optional[str] = None,
+        updated_by: typing.Optional[str] = None,  # A Roboto user_id
     ) -> None:
         updated = self.__dataset_delegate.update(
             self.__record,
             metadata_changeset=metadata_changeset,
             conditions=conditions,
             description=description,
             updated_by=updated_by,
@@ -576,16 +603,16 @@
         )
 
     def __upload_file(
         self,
         local_file_path: pathlib.Path,
         key: str,
         transaction_id: str,
-        credentials: Optional[Credentials] = None,
-        credential_provider: Optional[Callable[[], S3Credentials]] = None,
+        credentials: typing.Optional[Credentials] = None,
+        credential_provider: typing.Optional[typing.Callable[[], S3Credentials]] = None,
     ) -> FileUploadInfo:
         """
         Uploads a file to the dataset's storage location. Does not mark the upload as complete.
         """
         if not local_file_path.is_file():
             raise ValueError(f"{local_file_path} is not a file")
```

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/delegate.py` & `roboto-0.2.9/src/roboto/domain/datasets/delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,15 @@
             "expiry_time": self.expiration.isoformat(),
             "region": self.region,
         }
 
 
 class DatasetDelegate(abc.ABC):
     @abc.abstractmethod
-    def complete_upload(
-        self, dataset_id: str, transaction_id: str, org_id: Optional[str] = None
-    ) -> None:
+    def complete_upload(self, dataset_id: str, transaction_id: str) -> None:
         raise NotImplementedError("complete_upload")
 
     @abc.abstractmethod
     def create_dataset(
         self,
         administrator: Administrator = Administrator.Roboto,
         metadata: Optional[dict[str, Any]] = None,
@@ -67,18 +65,17 @@
         raise NotImplementedError("create_dataset")
 
     @abc.abstractmethod
     def delete_dataset(self, record: DatasetRecord) -> None:
         raise NotImplementedError("delete_dataset")
 
     @abc.abstractmethod
-    def get_dataset_by_primary_key(
+    def get_dataset_by_id(
         self,
         dataset_id: str,
-        org_id: Optional[str] = None,
     ) -> DatasetRecord:
         raise NotImplementedError("get_dataset_by_primary_key")
 
     @abc.abstractmethod
     def get_temporary_credentials(
         self,
         record: DatasetRecord,
@@ -88,15 +85,14 @@
     ) -> Credentials:
         raise NotImplementedError("get_temporary_credentials")
 
     @abc.abstractmethod
     def list_files(
         self,
         dataset_id: str,
-        org_id: Optional[str] = None,
         page_token: Optional[str] = None,
         include_patterns: Optional[list[str]] = None,
         exclude_patterns: Optional[list[str]] = None,
     ) -> PaginatedList[FileRecord]:
         raise NotImplementedError("list_files")
 
     @abc.abstractmethod
```

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/http_delegate.py` & `roboto-0.2.9/src/roboto/domain/datasets/http_delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,29 +86,28 @@
         Delete a dataset.
         """
         url = f"{self.__roboto_service_base_url}/v1/datasets/{record.dataset_id}"
 
         with RobotoHttpExceptionParse():
             self.__http_client.delete(
                 url,
-                headers=self.headers(record.org_id),
+                headers=self.headers(),
             )
 
-    def get_dataset_by_primary_key(
+    def get_dataset_by_id(
         self,
         dataset_id: str,
-        org_id: Optional[str] = None,
     ) -> DatasetRecord:
         """
         Get a dataset by its primary key (org_id, dataset_id)
         """
         url = f"{self.__roboto_service_base_url}/v1/datasets/{dataset_id}"
 
         with RobotoHttpExceptionParse():
-            response = self.__http_client.get(url, headers=self.headers(org_id))
+            response = self.__http_client.get(url, headers=self.headers())
 
         return DatasetRecord.model_validate(response.from_json(json_path=["data"]))
 
     def get_temporary_credentials(
         self,
         record: DatasetRecord,
         permissions: Permissions,
@@ -122,34 +121,31 @@
         encoded_qs = urllib.parse.urlencode(query_params)
         url = f"{self.__roboto_service_base_url}/v1/datasets/{record.dataset_id}/credentials?{encoded_qs}"
 
         if transaction_id:
             url += f"&transaction_id={transaction_id}"
 
         with RobotoHttpExceptionParse():
-            response = self.__http_client.get(url, self.headers(record.org_id, caller))
+            response = self.__http_client.get(url, self.headers(user_id=caller))
 
         return Credentials.model_validate(response.from_json(json_path=["data"]))
 
-    def complete_upload(
-        self, dataset_id: str, transaction_id: str, org_id: Optional[str] = None
-    ) -> None:
+    def complete_upload(self, dataset_id: str, transaction_id: str) -> None:
         """
         Marks an upload as 'completed', which allows the Roboto Platform to evaluate triggers for automatic action on
         incoming data. This also aides reporting on partial upload failure cases.
         """
         url = f"{self.__roboto_service_base_url}/v1/datasets/{dataset_id}/uploads/{transaction_id}/complete"
 
         with RobotoHttpExceptionParse():
-            self.__http_client.put(url=url, headers=self.headers(org_id))
+            self.__http_client.put(url=url, headers=self.headers())
 
     def list_files(
         self,
         dataset_id: str,
-        org_id: Optional[str] = None,
         page_token: Optional[str] = None,
         include_patterns: Optional[list[str]] = None,
         exclude_patterns: Optional[list[str]] = None,
     ) -> PaginatedList[FileRecord]:
         """
         List files associated with dataset.
 
@@ -166,15 +162,15 @@
             include_patterns=include_patterns,
             exclude_patterns=exclude_patterns,
         )
         with RobotoHttpExceptionParse():
             response = self.__http_client.post(
                 url,
                 data=pydantic_jsonable_dict(request_body, exclude_none=True),
-                headers=self.headers(org_id),
+                headers=self.headers(),
                 idempotent=True,
             )
 
         unmarshalled = response.from_json(json_path=["data"])
         return PaginatedList(
             items=[FileRecord.model_validate(file) for file in unmarshalled["items"]],
             next_token=unmarshalled["next_token"],
@@ -218,11 +214,11 @@
             description=description,
             conditions=conditions,
         )
         with RobotoHttpExceptionParse():
             response = self.__http_client.put(
                 url,
                 data=pydantic_jsonable_dict(payload, exclude_none=True),
-                headers=self.headers(record.org_id, updated_by),
+                headers=self.headers(user_id=updated_by),
             )
 
         return DatasetRecord.model_validate(response.from_json(json_path=["data"]))
```

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/http_resources.py` & `roboto-0.2.9/src/roboto/domain/datasets/http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/datasets/record.py` & `roboto-0.2.9/src/roboto/domain/datasets/record.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/files/__init__.py` & `roboto-0.2.9/src/roboto/domain/files/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/files/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/files/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 943 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 af03 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 af03 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 0100 6400 6405 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
@@ -43,15 +43,15 @@
 000002a0: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
 000002b0: 00da 0870 726f 6772 6573 7372 0c00 0000  ...progressr....
 000002c0: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
 000002d0: 1000 0000 7211 0000 00da 0672 6563 6f72  ....r......recor
 000002e0: 6472 1200 0000 da07 5f5f 616c 6c5f 5fa9  dr......__all__.
 000002f0: 0072 1900 0000 7219 0000 00fa e52f 636f  .r....r....../co
 00000300: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-00000310: 7263 3130 3531 3138 3230 3839 2f73 7263  rc1051182089/src
+00000310: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
 00000320: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
 00000330: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
 00000340: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
 00000350: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
 00000360: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
 00000370: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
 00000380: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
```

### Comparing `roboto-0.2.8/src/roboto/domain/files/__pycache__/client_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/files/__pycache__/client_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 13261 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 cd33 0000  o........Y.e.3..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 aa33 0000  o.......2H.e.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 f000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6401 6c07 5a08 6400 6401 6c09  ..d.d.l.Z.d.d.l.
 00000060: 5a09 6400 6401 6c0a 6d0b 0200 0100 6d0c  Z.d.d.l.m.....m.
 00000070: 5a0d 0100 6400 6401 6c0e 5a0f 6400 6401  Z...d.d.l.Z.d.d.
@@ -62,16 +62,16 @@
 000003d0: 0000 0000 0000 0000 0000 0004 0000 0002  ................
 000003e0: 0000 0043 0000 0073 1600 0000 7c01 7c00  ...C...s....|.|.
 000003f0: 5f00 7c02 7c00 5f01 7c03 7c00 5f02 6400  _.|.|._.|.|._.d.
 00000400: 5300 a901 4e29 0372 1500 0000 7216 0000  S...N).r....r...
 00000410: 0072 1700 0000 2904 da04 7365 6c66 7218  .r....)...selfr.
 00000420: 0000 0072 1900 0000 721a 0000 00a9 0072  ...r....r......r
 00000430: 1d00 0000 faec 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000440: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000450: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000440: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000450: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000460: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000470: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000480: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000490: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000004a0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000004b0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000004c0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
@@ -378,278 +378,278 @@
 00001790: 6c65 73b8 0000 0073 1e00 0000 0809 0401  les....s........
 000017a0: 04ff 0804 0401 0201 0201 0201 0201 08fc  ................
 000017b0: 0c07 0401 0801 06ff 04ff 7a21 4669 6c65  ..........z!File
 000017c0: 436c 6965 6e74 4465 6c65 6761 7465 2e64  ClientDelegate.d
 000017d0: 6f77 6e6c 6f61 645f 6669 6c65 7372 5500  ownload_filesrU.
 000017e0: 0000 7257 0000 0063 0300 0000 0000 0000  ..rW...c........
 000017f0: 0000 0000 0500 0000 0800 0000 4300 0000  ............C...
-00001800: 7366 0000 007c 006a 009b 0064 017c 019b  sf...|.j...d.|..
-00001810: 009d 037d 0374 0183 008f 1601 007c 006a  ...}.t.......|.j
-00001820: 026a 037c 0374 047c 0264 0264 0369 0164  .j.|.t.|.d.d.i.d
-00001830: 048d 0264 058d 027d 0457 0064 0004 0004  ...d...}.W.d....
-00001840: 0083 0301 006e 0831 0073 2477 0101 0001  .....n.1.s$w....
-00001850: 0001 0059 0001 0074 05a0 067c 046a 0764  ...Y...t...|.j.d
-00001860: 0667 0164 078d 01a1 0153 0029 084e 7a11  .g.d.....S.).Nz.
-00001870: 2f76 312f 6669 6c65 732f 7265 636f 7264  /v1/files/record
-00001880: 2f72 4e00 0000 724f 0000 00a9 0272 5700  /rN...rO.....rW.
-00001890: 0000 7252 0000 0072 5300 0000 da04 6461  ..rR...rS.....da
-000018a0: 7461 a901 da09 6a73 6f6e 5f70 6174 6829  ta....json_path)
-000018b0: 0872 2e00 0000 7206 0000 0072 2d00 0000  .r....r....r-...
-000018c0: 7270 0000 0072 0900 0000 7212 0000 00da  rp...r....r.....
-000018d0: 0e6d 6f64 656c 5f76 616c 6964 6174 65da  .model_validate.
-000018e0: 0966 726f 6d5f 6a73 6f6e 2905 721c 0000  .from_json).r...
-000018f0: 0072 5500 0000 7257 0000 0072 5800 0000  .rU...rW...rX...
-00001900: 7276 0000 0072 1d00 0000 721d 0000 0072  rv...r....r....r
-00001910: 1e00 0000 da19 6765 745f 7265 636f 7264  ......get_record
-00001920: 5f62 795f 7072 696d 6172 795f 6b65 79d2  _by_primary_key.
-00001930: 0000 0073 1600 0000 1003 0802 0601 0201  ...s............
-00001940: 0201 0201 0601 04fe 08fe 1cff 1408 7a2c  ..............z,
-00001950: 4669 6c65 436c 6965 6e74 4465 6c65 6761  FileClientDelega
-00001960: 7465 2e67 6574 5f72 6563 6f72 645f 6279  te.get_record_by
-00001970: 5f70 7269 6d61 7279 5f6b 6579 6302 0000  _primary_keyc...
-00001980: 0000 0000 0000 0000 0004 0000 0008 0000  ................
-00001990: 0043 0000 0073 6800 0000 7c00 6a00 9b00  .C...sh...|.j...
-000019a0: 6401 7c01 6a01 9b00 6402 9d04 7d02 7402  d.|.j...d...}.t.
-000019b0: 8300 8f17 0100 7c00 6a03 6a04 7c02 7405  ......|.j.j.|.t.
-000019c0: 7c01 6a06 6403 6404 6901 6405 8d02 6406  |.j.d.d.i.d...d.
-000019d0: 8d02 7d03 5700 6400 0400 0400 8303 0100  ..}.W.d.........
-000019e0: 6e08 3100 7327 7701 0100 0100 0100 5900  n.1.s'w.......Y.
-000019f0: 0100 7c03 6a07 6407 6408 6702 6409 8d01  ..|.j.d.d.g.d...
-00001a00: 5300 290a 4e72 4d00 0000 7a0b 2f73 6967  S.).NrM...z./sig
-00001a10: 6e65 642d 7572 6c72 4e00 0000 724f 0000  ned-urlrN...rO..
-00001a20: 0072 8800 0000 7253 0000 0072 8900 0000  .r....rS...r....
-00001a30: 7258 0000 0072 8a00 0000 2908 722e 0000  rX...r....).r...
-00001a40: 0072 5500 0000 7206 0000 0072 2d00 0000  .rU...r....r-...
-00001a50: 7270 0000 0072 0900 0000 7257 0000 0072  rp...r....rW...r
-00001a60: 8d00 0000 2904 721c 0000 0072 4c00 0000  ....).r....rL...
-00001a70: 7258 0000 0072 7600 0000 721d 0000 0072  rX...rv...r....r
-00001a80: 1d00 0000 721e 0000 00da 0e67 6574 5f73  ....r......get_s
-00001a90: 6967 6e65 645f 7572 6ce1 0000 0073 1600  igned_url....s..
-00001aa0: 0000 1401 0802 0601 0201 0201 0401 0601  ................
-00001ab0: 04fe 08fe 1cff 1008 7a21 4669 6c65 436c  ........z!FileCl
-00001ac0: 6965 6e74 4465 6c65 6761 7465 2e67 6574  ientDelegate.get
-00001ad0: 5f73 6967 6e65 645f 7572 6cda 0571 7565  _signed_url..que
-00001ae0: 7279 6303 0000 0000 0000 0000 0000 0007  ryc.............
-00001af0: 0000 0008 0000 0043 0000 0073 8a00 0000  .......C...s....
-00001b00: 7c00 6a00 9b00 6401 9d02 7d03 7401 7c01  |.j...d...}.t.|.
-00001b10: 6402 6403 8d02 7d04 7402 8300 8f18 0100  d.d...}.t.......
-00001b20: 7c00 6a03 6a04 7c03 7c04 7405 7c02 6404  |.j.j.|.|.t.|.d.
-00001b30: 6405 6901 6406 8d02 6402 6407 8d04 7d05  d.i.d...d.d...}.
-00001b40: 5700 6400 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
-00001b50: 732a 7701 0100 0100 0100 5900 0100 7c05  s*w.......Y...|.
-00001b60: 6a06 6408 6701 6409 8d01 7d06 7407 640a  j.d.g.d...}.t.d.
-00001b70: 640b 8400 7c06 640c 1900 4400 8301 7c06  d...|.d...D...|.
-00001b80: 640d 1900 640e 8d02 5300 290f 4e7a 0f2f  d...d...S.).Nz./
-00001b90: 7631 2f66 696c 6573 2f71 7565 7279 5429  v1/files/queryT)
-00001ba0: 01da 0c65 7863 6c75 6465 5f6e 6f6e 6572  ...exclude_noner
-00001bb0: 4e00 0000 724f 0000 0072 5000 0000 2903  N...rO...rP...).
-00001bc0: 7289 0000 0072 5400 0000 da0a 6964 656d  r....rT.....idem
-00001bd0: 706f 7465 6e74 7289 0000 0072 8a00 0000  potentr....r....
-00001be0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001bf0: 0005 0000 0053 0000 0073 1600 0000 6700  .....S...s....g.
-00001c00: 7c00 5d07 7d01 7400 a001 7c01 a101 9102  |.].}.t...|.....
-00001c10: 7102 5300 721d 0000 0029 0272 1200 0000  q.S.r....).r....
-00001c20: 728c 0000 0029 02da 022e 30da 0764 6174  r....)....0..dat
-00001c30: 6173 6574 721d 0000 0072 1d00 0000 721e  asetr....r....r.
-00001c40: 0000 00da 0a3c 6c69 7374 636f 6d70 3e02  .....<listcomp>.
-00001c50: 0100 0073 0600 0000 0600 0a01 06ff 7a32  ...s..........z2
-00001c60: 4669 6c65 436c 6965 6e74 4465 6c65 6761  FileClientDelega
-00001c70: 7465 2e71 7565 7279 5f66 696c 6573 2e3c  te.query_files.<
-00001c80: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00001c90: 703e da05 6974 656d 73da 0a6e 6578 745f  p>..items..next_
-00001ca0: 746f 6b65 6e29 0272 9600 0000 7297 0000  token).r....r...
-00001cb0: 0029 0872 2e00 0000 720b 0000 0072 0600  .).r....r....r..
-00001cc0: 0000 722d 0000 00da 0470 6f73 7472 0900  ..r-.....postr..
-00001cd0: 0000 728d 0000 0072 0800 0000 2907 721c  ..r....r....).r.
-00001ce0: 0000 0072 9000 0000 7257 0000 0072 5800  ...r....rW...rX.
-00001cf0: 0000 da09 706f 7374 5f62 6f64 7972 7600  ....post_bodyrv.
-00001d00: 0000 da0c 756e 6d61 7273 6861 6c6c 6564  ....unmarshalled
-00001d10: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
-00001d20: 0b71 7565 7279 5f66 696c 6573 ee00 0000  .query_files....
-00001d30: 7328 0000 000c 050c 0108 0106 0102 0102  s(..............
-00001d40: 0102 0102 0106 0104 fe02 0408 f91c ff0e  ................
-00001d50: 0b02 0106 0106 0104 ff06 0306 fc7a 1e46  .............z.F
-00001d60: 696c 6543 6c69 656e 7444 656c 6567 6174  ileClientDelegat
-00001d70: 652e 7175 6572 795f 6669 6c65 7372 6d00  e.query_filesrm.
-00001d80: 0000 726e 0000 00da 0474 6167 7363 0700  ..rn.....tagsc..
-00001d90: 0000 0000 0000 0000 0000 0c00 0000 0800  ................
-00001da0: 0000 4300 0000 73aa 0000 0074 007c 0183  ..C...s....t.|..
-00001db0: 017c 037c 0264 019c 037d 077c 0564 0075  .|.|.d...}.|.d.u
-00001dc0: 0172 2164 0264 0384 007c 05a0 01a1 0044  .r!d.d...|.....D
-00001dd0: 0083 017d 0874 026a 03a0 047c 08a1 017d  ...}.t.j...|...}
-00001de0: 0964 047c 0969 017c 0764 053c 007c 066a  .d.|.i.|.d.<.|.j
-00001df0: 057c 037c 01a0 06a1 006a 0764 068d 027d  .|.|.....j.d...}
-00001e00: 0a7c 0a6a 087c 0764 073c 007a 1a74 09a0  .|.j.|.d.<.z.t..
-00001e10: 0a7c 04a1 017d 0b7c 0b6a 0b64 0869 007c  .|...}.|.j.d.i.|
-00001e20: 07a4 018e 0101 0057 007c 0a64 0075 0172  .......W.|.d.u.r
-00001e30: 497c 0aa0 0ca1 0001 0064 0053 0064 0053  I|.......d.S.d.S
-00001e40: 007c 0a64 0075 0172 547c 0aa0 0ca1 0001  .|.d.u.rT|......
-00001e50: 0077 0077 0029 094e 2903 7269 0000 0072  .w.w.).N).ri...r
-00001e60: 6400 0000 7263 0000 0063 0100 0000 0000  d...rc...c......
-00001e70: 0000 0000 0000 0300 0000 0400 0000 5300  ..............S.
-00001e80: 0000 f318 0000 0069 007c 005d 085c 027d  .......i.|.].\.}
-00001e90: 017d 027c 016a 007c 0293 0271 0253 0072  .}.|.j.|...q.S.r
-00001ea0: 1d00 0000 a901 da05 7661 6c75 65a9 0372  ........value..r
-00001eb0: 9300 0000 da03 7461 6772 9f00 0000 721d  ......tagr....r.
-00001ec0: 0000 0072 1d00 0000 721e 0000 00da 0a3c  ...r....r......<
-00001ed0: 6469 6374 636f 6d70 3e18 0100 00f3 0200  dictcomp>.......
-00001ee0: 0000 1800 7a32 4669 6c65 436c 6965 6e74  ....z2FileClient
-00001ef0: 4465 6c65 6761 7465 2e75 706c 6f61 645f  Delegate.upload_
-00001f00: 6669 6c65 2e3c 6c6f 6361 6c73 3e2e 3c64  file.<locals>.<d
-00001f10: 6963 7463 6f6d 703e da07 5461 6767 696e  ictcomp>..Taggin
-00001f20: 675a 0945 7874 7261 4172 6773 7266 0000  gZ.ExtraArgsrf..
-00001f30: 0072 6a00 0000 721d 0000 0029 0d72 7300  .rj...r....).rs.
-00001f40: 0000 7296 0000 00da 0675 726c 6c69 62da  ..r......urllib.
-00001f50: 0570 6172 7365 da09 7572 6c65 6e63 6f64  .parse..urlencod
-00001f60: 6572 8300 0000 da04 7374 6174 da07 7374  er......stat..st
-00001f70: 5f73 697a 6572 7400 0000 722c 0000 0072  _sizert...r,...r
-00001f80: 4500 0000 da0b 7570 6c6f 6164 5f66 696c  E.....upload_fil
-00001f90: 6572 7500 0000 290c 721c 0000 0072 5e00  eru...).r....r^.
-00001fa0: 0000 726d 0000 0072 6e00 0000 722f 0000  ..rm...rn...r/..
-00001fb0: 0072 9c00 0000 725f 0000 005a 1075 706c  .r....r_...Z.upl
-00001fc0: 6f61 645f 6669 6c65 5f61 7267 73da 1173  oad_file_args..s
-00001fd0: 6572 6961 6c69 7a61 626c 655f 7461 6773  erializable_tags
-00001fe0: da0c 656e 636f 6465 645f 7461 6773 7277  ..encoded_tagsrw
-00001ff0: 0000 0072 5d00 0000 721d 0000 0072 1d00  ...r]...r....r..
-00002000: 0000 721e 0000 0072 aa00 0000 0801 0000  ..r....r........
-00002010: 7328 0000 0006 0a02 0102 0106 fd08 0612  s(..............
-00002020: 010c 010c 0104 020a 0106 ff0a 0302 020a  ................
-00002030: 0112 0108 020c 010c ff0a 0102 ff7a 1e46  .............z.F
-00002040: 696c 6543 6c69 656e 7444 656c 6567 6174  ileClientDelegat
-00002050: 652e 7570 6c6f 6164 5f66 696c 6572 8500  e.upload_filer..
-00002060: 0000 da0a 6578 7472 615f 6172 6773 6307  ....extra_argsc.
-00002070: 0000 0000 0000 0000 0000 000e 0000 0009  ................
-00002080: 0000 0043 0000 0073 a600 0000 7c00 a000  ...C...s....|...
-00002090: 7c03 7c05 a102 7d07 7c04 a001 a100 a002  |.|...}.|.......
-000020a0: 6401 6402 a102 7d08 7c04 a001 a100 a002  d.d...}.|.......
-000020b0: 6403 6402 a102 7d09 7c04 a001 a100 a002  d.d...}.|.......
-000020c0: 6404 6405 a102 7d0a 7c04 6a03 7c09 9b00  d.d...}.|.j.|...
-000020d0: 6406 7c08 9b00 9d03 7c0a 6407 8d02 7d0b  d.|.....|.d...}.
-000020e0: 7a23 7c02 4400 5d15 5c02 7d0c 7d0d 7c07  z#|.D.].\.}.}.|.
-000020f0: 6a04 7405 7c0c 8301 7c01 7c0d 7c06 7406  j.t.|...|.|.|.t.
-00002100: a007 7c0b 6a08 a101 6701 6408 8d05 0100  ..|.j...g.d.....
-00002110: 712d 7c07 a009 a100 0100 5700 7c0b a00a  q-|.......W.|...
-00002120: a100 0100 6400 5300 7c0b a00a a100 0100  ....d.S.|.......
-00002130: 7700 2909 4e72 7a00 0000 727b 0000 00da  w.).Nrz...r{....
-00002140: 1365 7870 6563 7465 645f 6669 6c65 5f63  .expected_file_c
-00002150: 6f75 6e74 da12 6578 7065 6374 6564 5f66  ount..expected_f
-00002160: 696c 655f 7369 7a65 e9ff ffff ff72 7c00  ile_size.....r|.
-00002170: 0000 7266 0000 0029 0272 ad00 0000 7280  ..rf...).r....r.
-00002180: 0000 0029 0b72 8100 0000 7282 0000 0072  ...).r....r....r
-00002190: 7000 0000 7283 0000 005a 0675 706c 6f61  p...r....Z.uploa
-000021a0: 6472 7300 0000 725c 0000 005a 1750 726f  drs...r\...Z.Pro
-000021b0: 6772 6573 7343 616c 6c62 6163 6b49 6e76  gressCallbackInv
-000021c0: 6f6b 6572 7274 0000 00da 0873 6875 7464  okerrt.....shutd
-000021d0: 6f77 6e72 7500 0000 290e 721c 0000 0072  ownru...).r....r
-000021e0: 6d00 0000 7278 0000 0072 2f00 0000 725f  m...rx...r/...r_
-000021f0: 0000 0072 5b00 0000 72ad 0000 0072 8400  ...r[...r....r..
-00002200: 0000 727a 0000 0072 ae00 0000 72af 0000  ..rz...r....r...
-00002210: 0072 7700 0000 da03 7372 6372 6e00 0000  .rw.....srcrn...
-00002220: 721d 0000 0072 1d00 0000 721e 0000 005a  r....r....r....Z
-00002230: 135f 5f75 706c 6f61 645f 6d61 6e79 5f66  .__upload_many_f
-00002240: 696c 6573 2801 0000 7334 0000 0004 0904  iles(...s4......
-00002250: 0104 ff10 0408 0104 0104 ff08 0304 0104  ................
-00002260: ff04 040c 0102 0106 fe02 050c 0104 0106  ................
-00002270: 0102 0102 0102 010a 0202 ff08 fb0a 0a16  ................
-00002280: 027a 2646 696c 6543 6c69 656e 7444 656c  .z&FileClientDel
-00002290: 6567 6174 652e 5f5f 7570 6c6f 6164 5f6d  egate.__upload_m
-000022a0: 616e 795f 6669 6c65 7363 0700 0000 0000  any_filesc......
-000022b0: 0000 0000 0000 0d00 0000 0900 0000 4300  ..............C.
-000022c0: 0000 738c 0000 0064 007d 077c 0464 0075  ..s....d.}.|.d.u
-000022d0: 0172 1964 0164 0284 007c 04a0 00a1 0044  .r.d.d...|.....D
-000022e0: 0083 017d 0874 016a 02a0 037c 08a1 017d  ...}.t.j...|...}
-000022f0: 0964 037c 0969 017d 077c 05a0 04a1 00a0  .d.|.i.}.|......
-00002300: 0564 0464 05a1 027d 0a7c 0a74 066b 0572  .d.d...}.|.t.k.r
-00002310: 327c 006a 077c 017c 027c 037c 057c 067c  2|.j.|.|.|.|.|.|
-00002320: 0764 068d 0601 0064 0053 007c 0244 005d  .d.....d.S.|.D.]
-00002330: 0f5c 027d 0b7d 0c7c 006a 087c 0b7c 017c  .\.}.}.|.j.|.|.|
-00002340: 0c7c 037c 047c 0564 078d 0601 0071 3464  .|.|.|.d.....q4d
-00002350: 0053 0029 084e 6301 0000 0000 0000 0000  .S.).Nc.........
-00002360: 0000 0003 0000 0004 0000 0053 0000 0072  ...........S...r
-00002370: 9d00 0000 721d 0000 0072 9e00 0000 72a0  ....r....r....r.
-00002380: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
-00002390: 0000 72a2 0000 005d 0100 0072 a300 0000  ..r....]...r....
-000023a0: 7a33 4669 6c65 436c 6965 6e74 4465 6c65  z3FileClientDele
-000023b0: 6761 7465 2e75 706c 6f61 645f 6669 6c65  gate.upload_file
-000023c0: 732e 3c6c 6f63 616c 733e 2e3c 6469 6374  s.<locals>.<dict
-000023d0: 636f 6d70 3e72 a400 0000 72ae 0000 0072  comp>r....r....r
-000023e0: 7b00 0000 2906 726d 0000 0072 7800 0000  {...).rm...rx...
-000023f0: 722f 0000 0072 5f00 0000 725b 0000 0072  r/...r_...r[...r
-00002400: ad00 0000 2906 725e 0000 0072 6d00 0000  ....).r^...rm...
-00002410: 726e 0000 0072 2f00 0000 729c 0000 0072  rn...r/...r....r
-00002420: 5f00 0000 2909 7296 0000 0072 a500 0000  _...).r....r....
-00002430: 72a6 0000 0072 a700 0000 7282 0000 0072  r....r....r....r
-00002440: 7000 0000 da0a 4d41 4e59 5f46 494c 4553  p.....MANY_FILES
-00002450: da26 5f46 696c 6543 6c69 656e 7444 656c  .&_FileClientDel
-00002460: 6567 6174 655f 5f75 706c 6f61 645f 6d61  egate__upload_ma
-00002470: 6e79 5f66 696c 6573 72aa 0000 0029 0d72  ny_filesr....).r
-00002480: 1c00 0000 726d 0000 0072 7800 0000 722f  ....rm...rx...r/
-00002490: 0000 0072 9c00 0000 725f 0000 0072 5b00  ...r....r_...r[.
-000024a0: 0000 72ad 0000 0072 ab00 0000 72ac 0000  ..r....r....r...
-000024b0: 0072 ae00 0000 72b2 0000 0072 6e00 0000  .r....r....rn...
-000024c0: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
-000024d0: 0c75 706c 6f61 645f 6669 6c65 7352 0100  .upload_filesR..
-000024e0: 0073 3600 0000 0409 0801 1201 0c01 0801  .s6.............
-000024f0: 0802 0401 04ff 0804 0401 0201 0201 0201  ................
-00002500: 0201 0201 0201 0afa 0c09 0401 0201 0201  ................
-00002510: 0201 0201 0201 0201 08fa 04ff 7a1f 4669  ............z.Fi
-00002520: 6c65 436c 6965 6e74 4465 6c65 6761 7465  leClientDelegate
-00002530: 2e75 706c 6f61 645f 6669 6c65 7329 0154  .upload_files).T
-00002540: 2901 725a 0000 0072 1b00 0000 2927 7228  ).rZ...r....)'r(
-00002550: 0000 0072 2900 0000 722a 0000 0072 0700  ...r)...r*...r..
-00002560: 0000 722b 0000 0072 7300 0000 da0c 7374  ..r+...rs.....st
-00002570: 6174 6963 6d65 7468 6f64 720d 0000 00da  aticmethodr.....
-00002580: 0462 6f6f 6c72 4500 0000 721f 0000 0072  .boolrE...r....r
-00002590: 1200 0000 7259 0000 0072 6f00 0000 7281  ....rY...ro...r.
-000025a0: 0000 0072 1000 0000 da07 7061 7468 6c69  ...r......pathli
-000025b0: 62da 0450 6174 6872 1100 0000 7272 0000  b..Pathr....rr..
-000025c0: 00da 0b63 6f6c 6c65 6374 696f 6e73 da03  ...collections..
-000025d0: 6162 63da 0947 656e 6572 6174 6f72 da05  abc..Generator..
-000025e0: 7475 706c 6572 8600 0000 7287 0000 0072  tupler....r....r
-000025f0: 0400 0000 728e 0000 0072 8f00 0000 720a  ....r....r....r.
-00002600: 0000 0072 0800 0000 729b 0000 00da 0464  ...r....r......d
-00002610: 6963 7472 0f00 0000 72aa 0000 0072 0200  ictr....r....r..
-00002620: 0000 72b4 0000 0072 b500 0000 da0d 5f5f  ..r....r......__
-00002630: 636c 6173 7363 656c 6c5f 5f72 1d00 0000  classcell__r....
-00002640: 721d 0000 0072 4a00 0000 721e 0000 0072  r....rJ...r....r
-00002650: 2c00 0000 3f00 0000 73fe 0000 000a 0008  ,...?...s.......
-00002660: 0108 0102 0202 0204 ff02 0102 ff02 010c  ................
-00002670: ff1a 1412 0502 0c02 0204 ff02 0102 ff02  ................
-00002680: 010c ff04 0e04 fb02 0202 fe04 0302 fd02  ................
-00002690: 0402 fc02 0502 fb02 060a fa04 2202 0104  ............"...
-000026a0: f906 0212 0102 ff02 fe02 0502 fb02 0602  ................
-000026b0: fa02 070a f904 2f02 0104 f906 0212 0102  ....../.........
-000026c0: ff02 fe02 0502 fb02 0602 fa02 0702 f902  ................
-000026d0: 080a f802 1b04 ff02 0102 ff06 0102 ff02  ................
-000026e0: 020a fe12 0f02 1004 fd02 0202 fe06 0302  ................
-000026f0: fd06 040a fc02 2004 0104 f904 0202 fe02  ...... .........
-00002700: 0302 fd02 0402 fc02 0502 fb0e 0602 fa02  ................
-00002710: 0702 f902 080a f804 2502 0102 0104 f902  ........%.......
-00002720: 0202 fe1a 0302 fd02 0402 fc02 0502 fb02  ................
-00002730: 0602 fa0e 070a f902 2f04 0102 0104 f902  ......../.......
-00002740: 0202 fe1a 0302 fd02 0402 fc0e 0502 fb02  ................
-00002750: 0602 fa02 0702 f902 0812 f872 2c00 0000  ...........r,...
-00002760: 2929 da0f 636f 6c6c 6563 7469 6f6e 732e  ))..collections.
-00002770: 6162 6372 ba00 0000 72b8 0000 00da 0674  abcr....r......t
-00002780: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
-00002790: 0400 0000 da0c 7572 6c6c 6962 2e70 6172  ......urllib.par
-000027a0: 7365 72a5 0000 0072 4000 0000 5a11 626f  ser....r@...Z.bo
-000027b0: 746f 332e 7333 2e74 7261 6e73 6665 7272  to3.s3.transferr
-000027c0: 3600 0000 5a08 7472 616e 7366 6572 725c  6...Z.transferr\
-000027d0: 0000 00da 0f62 6f74 6f63 6f72 652e 636f  .....botocore.co
-000027e0: 6e66 6967 7238 0000 00da 1462 6f74 6f63  nfigr8.....botoc
-000027f0: 6f72 652e 6372 6564 656e 7469 616c 73da  ore.credentials.
-00002800: 1062 6f74 6f63 6f72 652e 7365 7373 696f  .botocore.sessio
-00002810: 6eda 0a65 7863 6570 7469 6f6e 7372 0600  n..exceptionsr..
-00002820: 0000 da04 6874 7470 7207 0000 0072 0800  ....httpr....r..
-00002830: 0000 7209 0000 0072 9000 0000 720a 0000  ..r....r....r...
-00002840: 00da 0573 6572 6465 720b 0000 00da 0864  ...serder......d
-00002850: 656c 6567 6174 6572 0d00 0000 720e 0000  elegater....r...
-00002860: 0072 0f00 0000 da08 7072 6f67 7265 7373  .r......progress
-00002870: 7210 0000 0072 1100 0000 724c 0000 0072  r....r....rL...r
-00002880: 1200 0000 72b3 0000 005a 0e42 6173 6553  ....r....Z.BaseS
-00002890: 7562 7363 7269 6265 7272 1400 0000 722c  ubscriberr....r,
-000028a0: 0000 0072 1d00 0000 721d 0000 0072 1d00  ...r....r....r..
-000028b0: 0000 721e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000028c0: 3e01 0000 0073 2600 0000 0800 0801 1401  >....s&.........
-000028d0: 0801 0802 1201 0801 0801 0801 0c02 1401  ................
-000028e0: 0c05 0c01 1401 1005 0c04 0403 1203 141c  ................
+00001800: 7364 0000 007c 006a 009b 0064 017c 019b  sd...|.j...d.|..
+00001810: 009d 037d 0374 0183 008f 1501 007c 006a  ...}.t.......|.j
+00001820: 026a 037c 0374 0464 0264 0369 0164 048d  .j.|.t.d.d.i.d..
+00001830: 0164 058d 027d 0457 0064 0004 0004 0083  .d...}.W.d......
+00001840: 0301 006e 0831 0073 2377 0101 0001 0001  ...n.1.s#w......
+00001850: 0059 0001 0074 05a0 067c 046a 0764 0667  .Y...t...|.j.d.g
+00001860: 0164 078d 01a1 0153 0029 084e 7a11 2f76  .d.....S.).Nz./v
+00001870: 312f 6669 6c65 732f 7265 636f 7264 2f72  1/files/record/r
+00001880: 4e00 0000 724f 0000 0029 0172 5200 0000  N...rO...).rR...
+00001890: 7253 0000 00da 0464 6174 61a9 01da 096a  rS.....data....j
+000018a0: 736f 6e5f 7061 7468 2908 722e 0000 0072  son_path).r....r
+000018b0: 0600 0000 722d 0000 0072 7000 0000 7209  ....r-...rp...r.
+000018c0: 0000 0072 1200 0000 da0e 6d6f 6465 6c5f  ...r......model_
+000018d0: 7661 6c69 6461 7465 da09 6672 6f6d 5f6a  validate..from_j
+000018e0: 736f 6e29 0572 1c00 0000 7255 0000 0072  son).r....rU...r
+000018f0: 5700 0000 7258 0000 0072 7600 0000 721d  W...rX...rv...r.
+00001900: 0000 0072 1d00 0000 721e 0000 00da 1967  ...r....r......g
+00001910: 6574 5f72 6563 6f72 645f 6279 5f70 7269  et_record_by_pri
+00001920: 6d61 7279 5f6b 6579 d200 0000 7314 0000  mary_key....s...
+00001930: 0010 0308 0206 0102 0102 0106 0104 ff08  ................
+00001940: fe1c ff14 077a 2c46 696c 6543 6c69 656e  .....z,FileClien
+00001950: 7444 656c 6567 6174 652e 6765 745f 7265  tDelegate.get_re
+00001960: 636f 7264 5f62 795f 7072 696d 6172 795f  cord_by_primary_
+00001970: 6b65 7963 0200 0000 0000 0000 0000 0000  keyc............
+00001980: 0400 0000 0800 0000 4300 0000 7368 0000  ........C...sh..
+00001990: 007c 006a 009b 0064 017c 016a 019b 0064  .|.j...d.|.j...d
+000019a0: 029d 047d 0274 0283 008f 1701 007c 006a  ...}.t.......|.j
+000019b0: 036a 047c 0274 057c 016a 0664 0364 0469  .j.|.t.|.j.d.d.i
+000019c0: 0164 058d 0264 068d 027d 0357 0064 0004  .d...d...}.W.d..
+000019d0: 0004 0083 0301 006e 0831 0073 2777 0101  .......n.1.s'w..
+000019e0: 0001 0001 0059 0001 007c 036a 0764 0764  .....Y...|.j.d.d
+000019f0: 0867 0264 098d 0153 0029 0a4e 724d 0000  .g.d...S.).NrM..
+00001a00: 007a 0b2f 7369 676e 6564 2d75 726c 724e  .z./signed-urlrN
+00001a10: 0000 0072 4f00 0000 2902 7257 0000 0072  ...rO...).rW...r
+00001a20: 5200 0000 7253 0000 0072 8800 0000 7258  R...rS...r....rX
+00001a30: 0000 0072 8900 0000 2908 722e 0000 0072  ...r....).r....r
+00001a40: 5500 0000 7206 0000 0072 2d00 0000 7270  U...r....r-...rp
+00001a50: 0000 0072 0900 0000 7257 0000 0072 8c00  ...r....rW...r..
+00001a60: 0000 2904 721c 0000 0072 4c00 0000 7258  ..).r....rL...rX
+00001a70: 0000 0072 7600 0000 721d 0000 0072 1d00  ...rv...r....r..
+00001a80: 0000 721e 0000 00da 0e67 6574 5f73 6967  ..r......get_sig
+00001a90: 6e65 645f 7572 6ce0 0000 0073 1600 0000  ned_url....s....
+00001aa0: 1401 0802 0601 0201 0201 0401 0601 04fe  ................
+00001ab0: 08fe 1cff 1008 7a21 4669 6c65 436c 6965  ......z!FileClie
+00001ac0: 6e74 4465 6c65 6761 7465 2e67 6574 5f73  ntDelegate.get_s
+00001ad0: 6967 6e65 645f 7572 6cda 0571 7565 7279  igned_url..query
+00001ae0: 6303 0000 0000 0000 0000 0000 0007 0000  c...............
+00001af0: 0008 0000 0043 0000 0073 8a00 0000 7c00  .....C...s....|.
+00001b00: 6a00 9b00 6401 9d02 7d03 7401 7c01 6402  j...d...}.t.|.d.
+00001b10: 6403 8d02 7d04 7402 8300 8f18 0100 7c00  d...}.t.......|.
+00001b20: 6a03 6a04 7c03 7c04 7405 7c02 6404 6405  j.j.|.|.t.|.d.d.
+00001b30: 6901 6406 8d02 6402 6407 8d04 7d05 5700  i.d...d.d...}.W.
+00001b40: 6400 0400 0400 8303 0100 6e08 3100 732a  d.........n.1.s*
+00001b50: 7701 0100 0100 0100 5900 0100 7c05 6a06  w.......Y...|.j.
+00001b60: 6408 6701 6409 8d01 7d06 7407 640a 640b  d.g.d...}.t.d.d.
+00001b70: 8400 7c06 640c 1900 4400 8301 7c06 640d  ..|.d...D...|.d.
+00001b80: 1900 640e 8d02 5300 290f 4e7a 0f2f 7631  ..d...S.).Nz./v1
+00001b90: 2f66 696c 6573 2f71 7565 7279 5429 01da  /files/queryT)..
+00001ba0: 0c65 7863 6c75 6465 5f6e 6f6e 6572 4e00  .exclude_nonerN.
+00001bb0: 0000 724f 0000 0072 5000 0000 2903 7288  ..rO...rP...).r.
+00001bc0: 0000 0072 5400 0000 da0a 6964 656d 706f  ...rT.....idempo
+00001bd0: 7465 6e74 7288 0000 0072 8900 0000 6301  tentr....r....c.
+00001be0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00001bf0: 0000 0053 0000 0073 1600 0000 6700 7c00  ...S...s....g.|.
+00001c00: 5d07 7d01 7400 a001 7c01 a101 9102 7102  ].}.t...|.....q.
+00001c10: 5300 721d 0000 0029 0272 1200 0000 728b  S.r....).r....r.
+00001c20: 0000 0029 02da 022e 30da 0764 6174 6173  ...)....0..datas
+00001c30: 6574 721d 0000 0072 1d00 0000 721e 0000  etr....r....r...
+00001c40: 00da 0a3c 6c69 7374 636f 6d70 3e01 0100  ...<listcomp>...
+00001c50: 0073 0600 0000 0600 0a01 06ff 7a32 4669  .s..........z2Fi
+00001c60: 6c65 436c 6965 6e74 4465 6c65 6761 7465  leClientDelegate
+00001c70: 2e71 7565 7279 5f66 696c 6573 2e3c 6c6f  .query_files.<lo
+00001c80: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00001c90: da05 6974 656d 73da 0a6e 6578 745f 746f  ..items..next_to
+00001ca0: 6b65 6e29 0272 9500 0000 7296 0000 0029  ken).r....r....)
+00001cb0: 0872 2e00 0000 720b 0000 0072 0600 0000  .r....r....r....
+00001cc0: 722d 0000 00da 0470 6f73 7472 0900 0000  r-.....postr....
+00001cd0: 728c 0000 0072 0800 0000 2907 721c 0000  r....r....).r...
+00001ce0: 0072 8f00 0000 7257 0000 0072 5800 0000  .r....rW...rX...
+00001cf0: da09 706f 7374 5f62 6f64 7972 7600 0000  ..post_bodyrv...
+00001d00: da0c 756e 6d61 7273 6861 6c6c 6564 721d  ..unmarshalledr.
+00001d10: 0000 0072 1d00 0000 721e 0000 00da 0b71  ...r....r......q
+00001d20: 7565 7279 5f66 696c 6573 ed00 0000 7328  uery_files....s(
+00001d30: 0000 000c 050c 0108 0106 0102 0102 0102  ................
+00001d40: 0102 0106 0104 fe02 0408 f91c ff0e 0b02  ................
+00001d50: 0106 0106 0104 ff06 0306 fc7a 1e46 696c  ...........z.Fil
+00001d60: 6543 6c69 656e 7444 656c 6567 6174 652e  eClientDelegate.
+00001d70: 7175 6572 795f 6669 6c65 7372 6d00 0000  query_filesrm...
+00001d80: 726e 0000 00da 0474 6167 7363 0700 0000  rn.....tagsc....
+00001d90: 0000 0000 0000 0000 0c00 0000 0800 0000  ................
+00001da0: 4300 0000 73aa 0000 0074 007c 0183 017c  C...s....t.|...|
+00001db0: 037c 0264 019c 037d 077c 0564 0075 0172  .|.d...}.|.d.u.r
+00001dc0: 2164 0264 0384 007c 05a0 01a1 0044 0083  !d.d...|.....D..
+00001dd0: 017d 0874 026a 03a0 047c 08a1 017d 0964  .}.t.j...|...}.d
+00001de0: 047c 0969 017c 0764 053c 007c 066a 057c  .|.i.|.d.<.|.j.|
+00001df0: 037c 01a0 06a1 006a 0764 068d 027d 0a7c  .|.....j.d...}.|
+00001e00: 0a6a 087c 0764 073c 007a 1a74 09a0 0a7c  .j.|.d.<.z.t...|
+00001e10: 04a1 017d 0b7c 0b6a 0b64 0869 007c 07a4  ...}.|.j.d.i.|..
+00001e20: 018e 0101 0057 007c 0a64 0075 0172 497c  .....W.|.d.u.rI|
+00001e30: 0aa0 0ca1 0001 0064 0053 0064 0053 007c  .......d.S.d.S.|
+00001e40: 0a64 0075 0172 547c 0aa0 0ca1 0001 0077  .d.u.rT|.......w
+00001e50: 0077 0029 094e 2903 7269 0000 0072 6400  .w.).N).ri...rd.
+00001e60: 0000 7263 0000 0063 0100 0000 0000 0000  ..rc...c........
+00001e70: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
+00001e80: f318 0000 0069 007c 005d 085c 027d 017d  .....i.|.].\.}.}
+00001e90: 027c 016a 007c 0293 0271 0253 0072 1d00  .|.j.|...q.S.r..
+00001ea0: 0000 a901 da05 7661 6c75 65a9 0372 9200  ......value..r..
+00001eb0: 0000 da03 7461 6772 9e00 0000 721d 0000  ....tagr....r...
+00001ec0: 0072 1d00 0000 721e 0000 00da 0a3c 6469  .r....r......<di
+00001ed0: 6374 636f 6d70 3e17 0100 00f3 0200 0000  ctcomp>.........
+00001ee0: 1800 7a32 4669 6c65 436c 6965 6e74 4465  ..z2FileClientDe
+00001ef0: 6c65 6761 7465 2e75 706c 6f61 645f 6669  legate.upload_fi
+00001f00: 6c65 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  le.<locals>.<dic
+00001f10: 7463 6f6d 703e da07 5461 6767 696e 675a  tcomp>..TaggingZ
+00001f20: 0945 7874 7261 4172 6773 7266 0000 0072  .ExtraArgsrf...r
+00001f30: 6a00 0000 721d 0000 0029 0d72 7300 0000  j...r....).rs...
+00001f40: 7295 0000 00da 0675 726c 6c69 62da 0570  r......urllib..p
+00001f50: 6172 7365 da09 7572 6c65 6e63 6f64 6572  arse..urlencoder
+00001f60: 8300 0000 da04 7374 6174 da07 7374 5f73  ......stat..st_s
+00001f70: 697a 6572 7400 0000 722c 0000 0072 4500  izert...r,...rE.
+00001f80: 0000 da0b 7570 6c6f 6164 5f66 696c 6572  ....upload_filer
+00001f90: 7500 0000 290c 721c 0000 0072 5e00 0000  u...).r....r^...
+00001fa0: 726d 0000 0072 6e00 0000 722f 0000 0072  rm...rn...r/...r
+00001fb0: 9b00 0000 725f 0000 005a 1075 706c 6f61  ....r_...Z.uploa
+00001fc0: 645f 6669 6c65 5f61 7267 73da 1173 6572  d_file_args..ser
+00001fd0: 6961 6c69 7a61 626c 655f 7461 6773 da0c  ializable_tags..
+00001fe0: 656e 636f 6465 645f 7461 6773 7277 0000  encoded_tagsrw..
+00001ff0: 0072 5d00 0000 721d 0000 0072 1d00 0000  .r]...r....r....
+00002000: 721e 0000 0072 a900 0000 0701 0000 7328  r....r........s(
+00002010: 0000 0006 0a02 0102 0106 fd08 0612 010c  ................
+00002020: 010c 0104 020a 0106 ff0a 0302 020a 0112  ................
+00002030: 0108 020c 010c ff0a 0102 ff7a 1e46 696c  ...........z.Fil
+00002040: 6543 6c69 656e 7444 656c 6567 6174 652e  eClientDelegate.
+00002050: 7570 6c6f 6164 5f66 696c 6572 8500 0000  upload_filer....
+00002060: da0a 6578 7472 615f 6172 6773 6307 0000  ..extra_argsc...
+00002070: 0000 0000 0000 0000 000e 0000 0009 0000  ................
+00002080: 0043 0000 0073 a600 0000 7c00 a000 7c03  .C...s....|...|.
+00002090: 7c05 a102 7d07 7c04 a001 a100 a002 6401  |...}.|.......d.
+000020a0: 6402 a102 7d08 7c04 a001 a100 a002 6403  d...}.|.......d.
+000020b0: 6402 a102 7d09 7c04 a001 a100 a002 6404  d...}.|.......d.
+000020c0: 6405 a102 7d0a 7c04 6a03 7c09 9b00 6406  d...}.|.j.|...d.
+000020d0: 7c08 9b00 9d03 7c0a 6407 8d02 7d0b 7a23  |.....|.d...}.z#
+000020e0: 7c02 4400 5d15 5c02 7d0c 7d0d 7c07 6a04  |.D.].\.}.}.|.j.
+000020f0: 7405 7c0c 8301 7c01 7c0d 7c06 7406 a007  t.|...|.|.|.t...
+00002100: 7c0b 6a08 a101 6701 6408 8d05 0100 712d  |.j...g.d.....q-
+00002110: 7c07 a009 a100 0100 5700 7c0b a00a a100  |.......W.|.....
+00002120: 0100 6400 5300 7c0b a00a a100 0100 7700  ..d.S.|.......w.
+00002130: 2909 4e72 7a00 0000 727b 0000 00da 1365  ).Nrz...r{.....e
+00002140: 7870 6563 7465 645f 6669 6c65 5f63 6f75  xpected_file_cou
+00002150: 6e74 da12 6578 7065 6374 6564 5f66 696c  nt..expected_fil
+00002160: 655f 7369 7a65 e9ff ffff ff72 7c00 0000  e_size.....r|...
+00002170: 7266 0000 0029 0272 ac00 0000 7280 0000  rf...).r....r...
+00002180: 0029 0b72 8100 0000 7282 0000 0072 7000  .).r....r....rp.
+00002190: 0000 7283 0000 005a 0675 706c 6f61 6472  ..r....Z.uploadr
+000021a0: 7300 0000 725c 0000 005a 1750 726f 6772  s...r\...Z.Progr
+000021b0: 6573 7343 616c 6c62 6163 6b49 6e76 6f6b  essCallbackInvok
+000021c0: 6572 7274 0000 00da 0873 6875 7464 6f77  errt.....shutdow
+000021d0: 6e72 7500 0000 290e 721c 0000 0072 6d00  nru...).r....rm.
+000021e0: 0000 7278 0000 0072 2f00 0000 725f 0000  ..rx...r/...r_..
+000021f0: 0072 5b00 0000 72ac 0000 0072 8400 0000  .r[...r....r....
+00002200: 727a 0000 0072 ad00 0000 72ae 0000 0072  rz...r....r....r
+00002210: 7700 0000 da03 7372 6372 6e00 0000 721d  w.....srcrn...r.
+00002220: 0000 0072 1d00 0000 721e 0000 005a 135f  ...r....r....Z._
+00002230: 5f75 706c 6f61 645f 6d61 6e79 5f66 696c  _upload_many_fil
+00002240: 6573 2701 0000 7334 0000 0004 0904 0104  es'...s4........
+00002250: ff10 0408 0104 0104 ff08 0304 0104 ff04  ................
+00002260: 040c 0102 0106 fe02 050c 0104 0106 0102  ................
+00002270: 0102 0102 010a 0202 ff08 fb0a 0a16 027a  ...............z
+00002280: 2646 696c 6543 6c69 656e 7444 656c 6567  &FileClientDeleg
+00002290: 6174 652e 5f5f 7570 6c6f 6164 5f6d 616e  ate.__upload_man
+000022a0: 795f 6669 6c65 7363 0700 0000 0000 0000  y_filesc........
+000022b0: 0000 0000 0d00 0000 0900 0000 4300 0000  ............C...
+000022c0: 738c 0000 0064 007d 077c 0464 0075 0172  s....d.}.|.d.u.r
+000022d0: 1964 0164 0284 007c 04a0 00a1 0044 0083  .d.d...|.....D..
+000022e0: 017d 0874 016a 02a0 037c 08a1 017d 0964  .}.t.j...|...}.d
+000022f0: 037c 0969 017d 077c 05a0 04a1 00a0 0564  .|.i.}.|.......d
+00002300: 0464 05a1 027d 0a7c 0a74 066b 0572 327c  .d...}.|.t.k.r2|
+00002310: 006a 077c 017c 027c 037c 057c 067c 0764  .j.|.|.|.|.|.|.d
+00002320: 068d 0601 0064 0053 007c 0244 005d 0f5c  .....d.S.|.D.].\
+00002330: 027d 0b7d 0c7c 006a 087c 0b7c 017c 0c7c  .}.}.|.j.|.|.|.|
+00002340: 037c 047c 0564 078d 0601 0071 3464 0053  .|.|.d.....q4d.S
+00002350: 0029 084e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00002360: 0003 0000 0004 0000 0053 0000 0072 9c00  .........S...r..
+00002370: 0000 721d 0000 0072 9d00 0000 729f 0000  ..r....r....r...
+00002380: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00002390: 72a1 0000 005c 0100 0072 a200 0000 7a33  r....\...r....z3
+000023a0: 4669 6c65 436c 6965 6e74 4465 6c65 6761  FileClientDelega
+000023b0: 7465 2e75 706c 6f61 645f 6669 6c65 732e  te.upload_files.
+000023c0: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+000023d0: 6d70 3e72 a300 0000 72ad 0000 0072 7b00  mp>r....r....r{.
+000023e0: 0000 2906 726d 0000 0072 7800 0000 722f  ..).rm...rx...r/
+000023f0: 0000 0072 5f00 0000 725b 0000 0072 ac00  ...r_...r[...r..
+00002400: 0000 2906 725e 0000 0072 6d00 0000 726e  ..).r^...rm...rn
+00002410: 0000 0072 2f00 0000 729b 0000 0072 5f00  ...r/...r....r_.
+00002420: 0000 2909 7295 0000 0072 a400 0000 72a5  ..).r....r....r.
+00002430: 0000 0072 a600 0000 7282 0000 0072 7000  ...r....r....rp.
+00002440: 0000 da0a 4d41 4e59 5f46 494c 4553 da26  ....MANY_FILES.&
+00002450: 5f46 696c 6543 6c69 656e 7444 656c 6567  _FileClientDeleg
+00002460: 6174 655f 5f75 706c 6f61 645f 6d61 6e79  ate__upload_many
+00002470: 5f66 696c 6573 72a9 0000 0029 0d72 1c00  _filesr....).r..
+00002480: 0000 726d 0000 0072 7800 0000 722f 0000  ..rm...rx...r/..
+00002490: 0072 9b00 0000 725f 0000 0072 5b00 0000  .r....r_...r[...
+000024a0: 72ac 0000 0072 aa00 0000 72ab 0000 0072  r....r....r....r
+000024b0: ad00 0000 72b1 0000 0072 6e00 0000 721d  ....r....rn...r.
+000024c0: 0000 0072 1d00 0000 721e 0000 00da 0c75  ...r....r......u
+000024d0: 706c 6f61 645f 6669 6c65 7351 0100 0073  pload_filesQ...s
+000024e0: 3600 0000 0409 0801 1201 0c01 0801 0802  6...............
+000024f0: 0401 04ff 0804 0401 0201 0201 0201 0201  ................
+00002500: 0201 0201 0afa 0c09 0401 0201 0201 0201  ................
+00002510: 0201 0201 0201 08fa 04ff 7a1f 4669 6c65  ..........z.File
+00002520: 436c 6965 6e74 4465 6c65 6761 7465 2e75  ClientDelegate.u
+00002530: 706c 6f61 645f 6669 6c65 7329 0154 2901  pload_files).T).
+00002540: 725a 0000 0072 1b00 0000 2927 7228 0000  rZ...r....)'r(..
+00002550: 0072 2900 0000 722a 0000 0072 0700 0000  .r)...r*...r....
+00002560: 722b 0000 0072 7300 0000 da0c 7374 6174  r+...rs.....stat
+00002570: 6963 6d65 7468 6f64 720d 0000 00da 0462  icmethodr......b
+00002580: 6f6f 6c72 4500 0000 721f 0000 0072 1200  oolrE...r....r..
+00002590: 0000 7259 0000 0072 6f00 0000 7281 0000  ..rY...ro...r...
+000025a0: 0072 1000 0000 da07 7061 7468 6c69 62da  .r......pathlib.
+000025b0: 0450 6174 6872 1100 0000 7272 0000 00da  .Pathr....rr....
+000025c0: 0b63 6f6c 6c65 6374 696f 6e73 da03 6162  .collections..ab
+000025d0: 63da 0947 656e 6572 6174 6f72 da05 7475  c..Generator..tu
+000025e0: 706c 6572 8600 0000 7287 0000 0072 0400  pler....r....r..
+000025f0: 0000 728d 0000 0072 8e00 0000 720a 0000  ..r....r....r...
+00002600: 0072 0800 0000 729a 0000 00da 0464 6963  .r....r......dic
+00002610: 7472 0f00 0000 72a9 0000 0072 0200 0000  tr....r....r....
+00002620: 72b3 0000 0072 b400 0000 da0d 5f5f 636c  r....r......__cl
+00002630: 6173 7363 656c 6c5f 5f72 1d00 0000 721d  asscell__r....r.
+00002640: 0000 0072 4a00 0000 721e 0000 0072 2c00  ...rJ...r....r,.
+00002650: 0000 3f00 0000 73fe 0000 000a 0008 0108  ..?...s.........
+00002660: 0102 0202 0204 ff02 0102 ff02 010c ff1a  ................
+00002670: 1412 0502 0c02 0204 ff02 0102 ff02 010c  ................
+00002680: ff04 0e04 fb02 0202 fe04 0302 fd02 0402  ................
+00002690: fc02 0502 fb02 060a fa04 2202 0104 f906  ..........".....
+000026a0: 0212 0102 ff02 fe02 0502 fb02 0602 fa02  ................
+000026b0: 070a f904 2f02 0104 f906 0212 0102 ff02  ..../...........
+000026c0: fe02 0502 fb02 0602 fa02 0702 f902 080a  ................
+000026d0: f802 1b04 ff02 0102 ff06 0102 ff02 020a  ................
+000026e0: fe12 0e02 1004 fd02 0202 fe06 0302 fd06  ................
+000026f0: 040a fc02 2004 0104 f904 0202 fe02 0302  .... ...........
+00002700: fd02 0402 fc02 0502 fb0e 0602 fa02 0702  ................
+00002710: f902 080a f804 2502 0102 0104 f902 0202  ......%.........
+00002720: fe1a 0302 fd02 0402 fc02 0502 fb02 0602  ................
+00002730: fa0e 070a f902 2f04 0102 0104 f902 0202  ....../.........
+00002740: fe1a 0302 fd02 0402 fc0e 0502 fb02 0602  ................
+00002750: fa02 0702 f902 0812 f872 2c00 0000 2929  .........r,...))
+00002760: da0f 636f 6c6c 6563 7469 6f6e 732e 6162  ..collections.ab
+00002770: 6372 b900 0000 72b7 0000 00da 0674 7970  cr....r......typ
+00002780: 696e 6772 0200 0000 7203 0000 0072 0400  ingr....r....r..
+00002790: 0000 da0c 7572 6c6c 6962 2e70 6172 7365  ....urllib.parse
+000027a0: 72a4 0000 0072 4000 0000 5a11 626f 746f  r....r@...Z.boto
+000027b0: 332e 7333 2e74 7261 6e73 6665 7272 3600  3.s3.transferr6.
+000027c0: 0000 5a08 7472 616e 7366 6572 725c 0000  ..Z.transferr\..
+000027d0: 00da 0f62 6f74 6f63 6f72 652e 636f 6e66  ...botocore.conf
+000027e0: 6967 7238 0000 00da 1462 6f74 6f63 6f72  igr8.....botocor
+000027f0: 652e 6372 6564 656e 7469 616c 73da 1062  e.credentials..b
+00002800: 6f74 6f63 6f72 652e 7365 7373 696f 6eda  otocore.session.
+00002810: 0a65 7863 6570 7469 6f6e 7372 0600 0000  .exceptionsr....
+00002820: da04 6874 7470 7207 0000 0072 0800 0000  ..httpr....r....
+00002830: 7209 0000 0072 8f00 0000 720a 0000 00da  r....r....r.....
+00002840: 0573 6572 6465 720b 0000 00da 0864 656c  .serder......del
+00002850: 6567 6174 6572 0d00 0000 720e 0000 0072  egater....r....r
+00002860: 0f00 0000 da08 7072 6f67 7265 7373 7210  ......progressr.
+00002870: 0000 0072 1100 0000 724c 0000 0072 1200  ...r....rL...r..
+00002880: 0000 72b2 0000 005a 0e42 6173 6553 7562  ..r....Z.BaseSub
+00002890: 7363 7269 6265 7272 1400 0000 722c 0000  scriberr....r,..
+000028a0: 0072 1d00 0000 721d 0000 0072 1d00 0000  .r....r....r....
+000028b0: 721e 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+000028c0: 0000 0073 2600 0000 0800 0801 1401 0801  ...s&...........
+000028d0: 0802 1201 0801 0801 0801 0c02 1401 0c05  ................
+000028e0: 0c01 1401 1005 0c04 0403 1203 141c       ..............
```

### Comparing `roboto-0.2.8/src/roboto/domain/files/__pycache__/delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/files/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3294 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 de0c 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 b20c 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 fe00 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a02  d.d.l.Z.d.d.l.Z.
 00000040: 6400 6401 6c03 5a03 6400 6401 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 6d06 5a06 6d07 5a07 6d08  d.d.l.m.Z.m.Z.m.
 00000060: 5a08 0100 7a08 6400 6403 6c05 6d09 5a09  Z...z.d.d.l.m.Z.
 00000070: 0100 5700 6e1b 0400 650a 793e 0100 0100  ..W.n...e.y>....
@@ -38,16 +38,16 @@
 00000250: 2907 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 00000260: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000270: 6e61 6d65 5f5f da09 4461 7461 7365 7449  name__..DatasetI
 00000280: 64da 054f 7267 4964 da0c 436f 6d6d 6f6e  d..OrgId..Common
 00000290: 5072 6566 6978 da0d 5472 616e 7361 6374  Prefix..Transact
 000002a0: 696f 6e49 64a9 0072 1800 0000 7218 0000  ionId..r....r...
 000002b0: 00fa e52f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-000002c0: 7470 7574 2f73 7263 3130 3531 3138 3230  tput/src10511820
-000002d0: 3839 2f73 7263 2f63 6f64 6573 7461 722d  89/src/codestar-
+000002c0: 7470 7574 2f73 7263 3330 3739 3233 3632  tput/src30792362
+000002d0: 3634 2f73 7263 2f63 6f64 6573 7461 722d  64/src/codestar-
 000002e0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000002f0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 00000300: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 00000310: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 00000320: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 00000330: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000340: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
@@ -78,155 +78,153 @@
 000004d0: 6f74 6174 696f 6e73 5f5f 7203 0000 0072  otations__r....r
 000004e0: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
 000004f0: 0000 0072 1a00 0000 2100 0000 730e 0000  ...r....!...s...
 00000500: 000a 0004 0108 0408 0108 0108 0110 0172  ...............r
 00000510: 1a00 0000 da12 4372 6564 656e 7469 616c  ......Credential
 00000520: 5072 6f76 6964 6572 6300 0000 0000 0000  Providerc.......
 00000530: 0000 0000 0000 0000 0010 0000 0040 0000  .............@..
-00000540: 0073 9401 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
+00000540: 0073 8801 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
 00000550: 6a04 6401 6505 6402 6403 6604 6404 6405  j.d.e.d.d.f.d.d.
 00000560: 8404 8301 5a06 6503 6a04 6507 8300 6601  ....Z.e.j.e...f.
 00000570: 6401 6505 6406 6508 6a09 6407 650a 6408  d.e.d.e.j.d.e.d.
 00000580: 650b 6402 6403 660a 6409 640a 8405 8301  e.d.d.f.d.d.....
 00000590: 5a0c 6503 6a04 6507 8300 640b 6602 640c  Z.e.j.e...d.f.d.
 000005a0: 650d 6a03 6a0e 650f 6505 6508 6a09 6602  e.j.j.e.e.e.j.f.
 000005b0: 1900 6403 6403 6603 1900 6407 650a 6408  ..d.d.f...d.e.d.
 000005c0: 650b 640d 6510 6402 6403 660a 640e 640f  e.d.e.d.d.f.d.d.
-000005d0: 8405 8301 5a11 6503 6a04 0903 6421 6410  ....Z.e.j...d!d.
-000005e0: 6512 6411 6513 6512 1900 6402 6505 6606  e.d.e.e...d.e.f.
-000005f0: 6412 6413 8405 8301 5a14 6503 6a04 6401  d.d.....Z.e.j.d.
-00000600: 6505 6402 6512 6604 6414 6415 8404 8301  e.d.e.f.d.d.....
-00000610: 5a15 6503 6a04 0903 6421 6416 6516 6411  Z.e.j...d!d.e.d.
-00000620: 6513 6512 1900 6402 6517 6505 1900 6606  e.e...d.e.e...f.
-00000630: 6417 6418 8405 8301 5a18 6503 6a04 6403  d.d.....Z.e.j.d.
-00000640: 6507 8300 6602 6406 6508 6a09 6419 6512  e...f.d.e.j.d.e.
-00000650: 641a 6512 6407 650a 641b 6513 6519 651a  d.e.d.e.d.e.e.e.
-00000660: 6512 6602 1900 1900 6408 650b 6402 6403  e.f.....d.e.d.d.
-00000670: 660e 641c 641d 8405 8301 5a1b 6503 6a04  f.d.d.....Z.e.j.
-00000680: 6403 6507 8300 641e 6603 6419 6512 640c  d.e...d.f.d.e.d.
-00000690: 650d 6a03 6a0e 650f 6508 6a09 6512 6602  e.j.j.e.e.j.e.f.
-000006a0: 1900 6403 6403 6603 1900 6407 650a 641b  ..d.d.f...d.e.d.
-000006b0: 6513 6519 651a 6512 6602 1900 1900 6408  e.e.e.e.f.....d.
-000006c0: 650b 640d 6510 6402 6403 660e 641f 6420  e.d.e.d.d.f.d.d 
-000006d0: 8405 8301 5a1c 6403 5300 2922 da0c 4669  ....Z.d.S.)"..Fi
-000006e0: 6c65 4465 6c65 6761 7465 da06 7265 636f  leDelegate..reco
-000006f0: 7264 da06 7265 7475 726e 4e63 0200 0000  rd..returnNc....
-00000700: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00000710: 4300 0000 f308 0000 0074 0064 0183 0182  C........t.d....
-00000720: 0129 024e da0b 6465 6c65 7465 5f66 696c  .).N..delete_fil
-00000730: 65a9 01da 134e 6f74 496d 706c 656d 656e  e....NotImplemen
-00000740: 7465 6445 7272 6f72 a902 da04 7365 6c66  tedError....self
-00000750: 7225 0000 0072 1800 0000 7218 0000 0072  r%...r....r....r
-00000760: 1900 0000 7228 0000 0031 0000 00f3 0200  ....r(...1......
-00000770: 0000 0802 7a18 4669 6c65 4465 6c65 6761  ....z.FileDelega
-00000780: 7465 2e64 656c 6574 655f 6669 6c65 da0a  te.delete_file..
-00000790: 6c6f 6361 6c5f 7061 7468 da13 6372 6564  local_path..cred
-000007a0: 656e 7469 616c 5f70 726f 7669 6465 72da  ential_provider.
-000007b0: 1870 726f 6772 6573 735f 6d6f 6e69 746f  .progress_monito
-000007c0: 725f 6661 6374 6f72 7963 0500 0000 0000  r_factoryc......
-000007d0: 0000 0000 0000 0500 0000 0200 0000 4300  ..............C.
-000007e0: 0000 7227 0000 0029 024e da0d 646f 776e  ..r'...).N..down
-000007f0: 6c6f 6164 5f66 696c 6572 2900 0000 2905  load_filer)...).
-00000800: 722c 0000 0072 2500 0000 722e 0000 0072  r,...r%...r....r
-00000810: 2f00 0000 7230 0000 0072 1800 0000 7218  /...r0...r....r.
-00000820: 0000 0072 1900 0000 7231 0000 0035 0000  ...r....r1...5..
-00000830: 0073 0200 0000 0808 7a1a 4669 6c65 4465  .s......z.FileDe
-00000840: 6c65 6761 7465 2e64 6f77 6e6c 6f61 645f  legate.download_
-00000850: 6669 6c65 e914 0000 00da 0e66 696c 655f  file.......file_
-00000860: 6765 6e65 7261 746f 72da 0f6d 6178 5f63  generator..max_c
-00000870: 6f6e 6375 7272 656e 6379 6305 0000 0000  oncurrencyc.....
-00000880: 0000 0000 0000 0005 0000 0002 0000 0043  ...............C
-00000890: 0000 0072 2700 0000 2902 4eda 0e64 6f77  ...r'...).N..dow
-000008a0: 6e6c 6f61 645f 6669 6c65 7372 2900 0000  nload_filesr)...
-000008b0: 2905 722c 0000 0072 3300 0000 722f 0000  ).r,...r3...r/..
-000008c0: 0072 3000 0000 7234 0000 0072 1800 0000  .r0...r4...r....
-000008d0: 7218 0000 0072 1900 0000 7235 0000 003f  r....r....r5...?
-000008e0: 0000 00f3 0200 0000 080a 7a1b 4669 6c65  ..........z.File
-000008f0: 4465 6c65 6761 7465 2e64 6f77 6e6c 6f61  Delegate.downloa
-00000900: 645f 6669 6c65 73da 0766 696c 655f 6964  d_files..file_id
-00000910: 720f 0000 0063 0300 0000 0000 0000 0000  r....c..........
-00000920: 0000 0300 0000 0200 0000 4300 0000 7227  ..........C...r'
-00000930: 0000 0029 024e da19 6765 745f 7265 636f  ...).N..get_reco
-00000940: 7264 5f62 795f 7072 696d 6172 795f 6b65  rd_by_primary_ke
-00000950: 7972 2900 0000 2903 722c 0000 0072 3700  yr)...).r,...r7.
-00000960: 0000 720f 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00000970: 0072 1900 0000 7238 0000 004b 0000 0073  .r....r8...K...s
-00000980: 0200 0000 0804 7a26 4669 6c65 4465 6c65  ......z&FileDele
-00000990: 6761 7465 2e67 6574 5f72 6563 6f72 645f  gate.get_record_
-000009a0: 6279 5f70 7269 6d61 7279 5f6b 6579 6302  by_primary_keyc.
-000009b0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-000009c0: 0000 0043 0000 0072 2700 0000 2902 4eda  ...C...r'...).N.
-000009d0: 0e67 6574 5f73 6967 6e65 645f 7572 6c72  .get_signed_urlr
-000009e0: 2900 0000 722b 0000 0072 1800 0000 7218  )...r+...r....r.
-000009f0: 0000 0072 1900 0000 7239 0000 0051 0000  ...r....r9...Q..
-00000a00: 0072 2d00 0000 7a1b 4669 6c65 4465 6c65  .r-...z.FileDele
-00000a10: 6761 7465 2e67 6574 5f73 6967 6e65 645f  gate.get_signed_
-00000a20: 7572 6cda 0571 7565 7279 6303 0000 0000  url..queryc.....
-00000a30: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
-00000a40: 0000 0072 2700 0000 2902 4eda 0b71 7565  ...r'...).N..que
-00000a50: 7279 5f66 696c 6573 7229 0000 0029 0372  ry_filesr)...).r
-00000a60: 2c00 0000 723a 0000 0072 0f00 0000 7218  ,...r:...r....r.
-00000a70: 0000 0072 1800 0000 7219 0000 0072 3b00  ...r....r....r;.
-00000a80: 0000 5500 0000 7302 0000 0008 067a 1846  ..U...s......z.F
-00000a90: 696c 6544 656c 6567 6174 652e 7175 6572  ileDelegate.quer
-00000aa0: 795f 6669 6c65 73da 0662 7563 6b65 74da  y_files..bucket.
-00000ab0: 036b 6579 da04 7461 6773 6307 0000 0000  .key..tagsc.....
-00000ac0: 0000 0000 0000 0007 0000 0002 0000 0043  ...............C
-00000ad0: 0000 0072 2700 0000 a902 4eda 0b75 706c  ...r'.....N..upl
-00000ae0: 6f61 645f 6669 6c65 7229 0000 0029 0772  oad_filer)...).r
-00000af0: 2c00 0000 722e 0000 0072 3c00 0000 723d  ,...r....r<...r=
-00000b00: 0000 0072 2f00 0000 723e 0000 0072 3000  ...r/...r>...r0.
-00000b10: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000b20: 0072 4000 0000 5d00 0000 7236 0000 007a  .r@...]...r6...z
-00000b30: 1846 696c 6544 656c 6567 6174 652e 7570  .FileDelegate.up
-00000b40: 6c6f 6164 5f66 696c 6572 0900 0000 6307  load_filer....c.
-00000b50: 0000 0000 0000 0000 0000 0007 0000 0002  ................
-00000b60: 0000 0043 0000 0072 2700 0000 723f 0000  ...C...r'...r?..
-00000b70: 0072 2900 0000 2907 722c 0000 0072 3c00  .r)...).r,...r<.
-00000b80: 0000 7233 0000 0072 2f00 0000 723e 0000  ..r3...r/...r>..
-00000b90: 0072 3000 0000 7234 0000 0072 1800 0000  .r0...r4...r....
-00000ba0: 7218 0000 0072 1900 0000 da0c 7570 6c6f  r....r......uplo
-00000bb0: 6164 5f66 696c 6573 6900 0000 7236 0000  ad_filesi...r6..
-00000bc0: 007a 1946 696c 6544 656c 6567 6174 652e  .z.FileDelegate.
-00000bd0: 7570 6c6f 6164 5f66 696c 6573 2901 4e29  upload_files).N)
-00000be0: 1d72 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000bf0: da03 6162 63da 0e61 6273 7472 6163 746d  ..abc..abstractm
-00000c00: 6574 686f 6472 0c00 0000 7228 0000 0072  ethodr....r(...r
-00000c10: 0a00 0000 da07 7061 7468 6c69 62da 0450  ......pathlib..P
-00000c20: 6174 6872 2300 0000 720b 0000 0072 3100  athr#...r....r1.
-00000c30: 0000 da0b 636f 6c6c 6563 7469 6f6e 73da  ....collections.
-00000c40: 0947 656e 6572 6174 6f72 da05 7475 706c  .Generator..tupl
-00000c50: 65da 0369 6e74 7235 0000 0072 2100 0000  e..intr5...r!...
-00000c60: 7203 0000 0072 3800 0000 7239 0000 0072  r....r8...r9...r
-00000c70: 0800 0000 7207 0000 0072 3b00 0000 da04  ....r....r;.....
-00000c80: 6469 6374 720d 0000 0072 4000 0000 7241  dictr....r@...rA
-00000c90: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-00000ca0: 0000 7219 0000 0072 2400 0000 3000 0000  ..r....r$...0...
-00000cb0: 73b2 0000 0008 0004 0114 0104 0304 0604  s...............
-00000cc0: fb02 0202 fe04 0302 fd02 0402 fc02 0502  ................
-00000cd0: fb02 060c fa04 0904 0702 0104 f906 0212  ................
-00000ce0: 0102 ff02 fe02 0502 fb02 0602 fa02 0702  ................
-00000cf0: f902 080c f804 0b02 0204 ff02 0102 ff06  ................
-00000d00: 0102 ff02 020c fe04 0514 0104 0302 0404  ................
-00000d10: fd02 0202 fe06 0302 fd06 040c fc04 0702  ................
-00000d20: 0704 0104 f904 0202 fe02 0302 fd02 0402  ................
-00000d30: fc02 0502 fb0e 0602 fa02 0702 f902 080c  ................
-00000d40: f804 0b02 0604 0102 0104 f902 0202 fe1a  ................
-00000d50: 0302 fd02 0402 fc0e 0502 fb02 0602 fa02  ................
-00000d60: 0702 f902 0810 f872 2400 0000 291c 7242  .......r$...).rB
-00000d70: 0000 00da 0f63 6f6c 6c65 6374 696f 6e73  .....collections
-00000d80: 2e61 6263 7246 0000 00da 0465 6e75 6d72  .abcrF.....enumr
-00000d90: 4400 0000 da06 7479 7069 6e67 7202 0000  D.....typingr...
-00000da0: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
-00000db0: da0b 496d 706f 7274 4572 726f 72da 1174  ..ImportError..t
-00000dc0: 7970 696e 675f 6578 7465 6e73 696f 6e73  yping_extensions
-00000dd0: da04 6874 7470 7207 0000 0072 3a00 0000  ..httpr....r:...
-00000de0: 7208 0000 00da 0870 726f 6772 6573 7372  r......progressr
-00000df0: 0a00 0000 720b 0000 0072 2500 0000 720c  ....r....r%...r.
-00000e00: 0000 00da 0445 6e75 6d72 0d00 0000 721a  .....Enumr....r.
-00000e10: 0000 0072 2300 0000 7222 0000 00da 0341  ...r#...r".....A
-00000e20: 4243 7224 0000 0072 1800 0000 7218 0000  BCr$...r....r...
-00000e30: 0072 1800 0000 7219 0000 00da 083c 6d6f  .r....r......<mo
-00000e40: 6475 6c65 3e01 0000 0073 2e00 0000 0a00  dule>....s......
-00000e50: 0801 0801 0801 1401 0203 1001 0c01 0201  ................
-00000e60: 1001 0c01 0401 02ff 0480 02fd 0c06 0c01  ................
-00000e70: 1001 0c04 1203 1008 140c 1603            ............
+000005d0: 8405 8301 5a11 6503 6a04 6410 6512 6402  ....Z.e.j.d.e.d.
+000005e0: 6505 6604 6411 6412 8404 8301 5a13 6503  e.f.d.d.....Z.e.
+000005f0: 6a04 6401 6505 6402 6512 6604 6413 6414  j.d.e.d.e.f.d.d.
+00000600: 8404 8301 5a14 6503 6a04 0903 6421 6415  ....Z.e.j...d!d.
+00000610: 6515 6416 6516 6512 1900 6402 6517 6505  e.d.e.e...d.e.e.
+00000620: 1900 6606 6417 6418 8405 8301 5a18 6503  ..f.d.d.....Z.e.
+00000630: 6a04 6403 6507 8300 6602 6406 6508 6a09  j.d.e...f.d.e.j.
+00000640: 6419 6512 641a 6512 6407 650a 641b 6516  d.e.d.e.d.e.d.e.
+00000650: 6519 651a 6512 6602 1900 1900 6408 650b  e.e.e.f.....d.e.
+00000660: 6402 6403 660e 641c 641d 8405 8301 5a1b  d.d.f.d.d.....Z.
+00000670: 6503 6a04 6403 6507 8300 641e 6603 6419  e.j.d.e...d.f.d.
+00000680: 6512 640c 650d 6a03 6a0e 650f 6508 6a09  e.d.e.j.j.e.e.j.
+00000690: 6512 6602 1900 6403 6403 6603 1900 6407  e.f...d.d.f...d.
+000006a0: 650a 641b 6516 6519 651a 6512 6602 1900  e.d.e.e.e.e.f...
+000006b0: 1900 6408 650b 640d 6510 6402 6403 660e  ..d.e.d.e.d.d.f.
+000006c0: 641f 6420 8405 8301 5a1c 6403 5300 2922  d.d ....Z.d.S.)"
+000006d0: da0c 4669 6c65 4465 6c65 6761 7465 da06  ..FileDelegate..
+000006e0: 7265 636f 7264 da06 7265 7475 726e 4e63  record..returnNc
+000006f0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000700: 0200 0000 4300 0000 f308 0000 0074 0064  ....C........t.d
+00000710: 0183 0182 0129 024e da0b 6465 6c65 7465  .....).N..delete
+00000720: 5f66 696c 65a9 01da 134e 6f74 496d 706c  _file....NotImpl
+00000730: 656d 656e 7465 6445 7272 6f72 a902 da04  ementedError....
+00000740: 7365 6c66 7225 0000 0072 1800 0000 7218  selfr%...r....r.
+00000750: 0000 0072 1900 0000 7228 0000 0031 0000  ...r....r(...1..
+00000760: 00f3 0200 0000 0802 7a18 4669 6c65 4465  ........z.FileDe
+00000770: 6c65 6761 7465 2e64 656c 6574 655f 6669  legate.delete_fi
+00000780: 6c65 da0a 6c6f 6361 6c5f 7061 7468 da13  le..local_path..
+00000790: 6372 6564 656e 7469 616c 5f70 726f 7669  credential_provi
+000007a0: 6465 72da 1870 726f 6772 6573 735f 6d6f  der..progress_mo
+000007b0: 6e69 746f 725f 6661 6374 6f72 7963 0500  nitor_factoryc..
+000007c0: 0000 0000 0000 0000 0000 0500 0000 0200  ................
+000007d0: 0000 4300 0000 7227 0000 0029 024e da0d  ..C...r'...).N..
+000007e0: 646f 776e 6c6f 6164 5f66 696c 6572 2900  download_filer).
+000007f0: 0000 2905 722c 0000 0072 2500 0000 722e  ..).r,...r%...r.
+00000800: 0000 0072 2f00 0000 7230 0000 0072 1800  ...r/...r0...r..
+00000810: 0000 7218 0000 0072 1900 0000 7231 0000  ..r....r....r1..
+00000820: 0035 0000 0073 0200 0000 0808 7a1a 4669  .5...s......z.Fi
+00000830: 6c65 4465 6c65 6761 7465 2e64 6f77 6e6c  leDelegate.downl
+00000840: 6f61 645f 6669 6c65 e914 0000 00da 0e66  oad_file.......f
+00000850: 696c 655f 6765 6e65 7261 746f 72da 0f6d  ile_generator..m
+00000860: 6178 5f63 6f6e 6375 7272 656e 6379 6305  ax_concurrencyc.
+00000870: 0000 0000 0000 0000 0000 0005 0000 0002  ................
+00000880: 0000 0043 0000 0072 2700 0000 2902 4eda  ...C...r'...).N.
+00000890: 0e64 6f77 6e6c 6f61 645f 6669 6c65 7372  .download_filesr
+000008a0: 2900 0000 2905 722c 0000 0072 3300 0000  )...).r,...r3...
+000008b0: 722f 0000 0072 3000 0000 7234 0000 0072  r/...r0...r4...r
+000008c0: 1800 0000 7218 0000 0072 1900 0000 7235  ....r....r....r5
+000008d0: 0000 003f 0000 00f3 0200 0000 080a 7a1b  ...?..........z.
+000008e0: 4669 6c65 4465 6c65 6761 7465 2e64 6f77  FileDelegate.dow
+000008f0: 6e6c 6f61 645f 6669 6c65 73da 0766 696c  nload_files..fil
+00000900: 655f 6964 6302 0000 0000 0000 0000 0000  e_idc...........
+00000910: 0002 0000 0002 0000 0043 0000 0072 2700  .........C...r'.
+00000920: 0000 2902 4eda 1967 6574 5f72 6563 6f72  ..).N..get_recor
+00000930: 645f 6279 5f70 7269 6d61 7279 5f6b 6579  d_by_primary_key
+00000940: 7229 0000 0029 0272 2c00 0000 7237 0000  r)...).r,...r7..
+00000950: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000960: 7238 0000 004b 0000 0072 2d00 0000 7a26  r8...K...r-...z&
+00000970: 4669 6c65 4465 6c65 6761 7465 2e67 6574  FileDelegate.get
+00000980: 5f72 6563 6f72 645f 6279 5f70 7269 6d61  _record_by_prima
+00000990: 7279 5f6b 6579 6302 0000 0000 0000 0000  ry_keyc.........
+000009a0: 0000 0002 0000 0002 0000 0043 0000 0072  ...........C...r
+000009b0: 2700 0000 2902 4eda 0e67 6574 5f73 6967  '...).N..get_sig
+000009c0: 6e65 645f 7572 6c72 2900 0000 722b 0000  ned_urlr)...r+..
+000009d0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+000009e0: 7239 0000 004f 0000 0072 2d00 0000 7a1b  r9...O...r-...z.
+000009f0: 4669 6c65 4465 6c65 6761 7465 2e67 6574  FileDelegate.get
+00000a00: 5f73 6967 6e65 645f 7572 6cda 0571 7565  _signed_url..que
+00000a10: 7279 720f 0000 0063 0300 0000 0000 0000  ryr....c........
+00000a20: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
+00000a30: 7227 0000 0029 024e da0b 7175 6572 795f  r'...).N..query_
+00000a40: 6669 6c65 7372 2900 0000 2903 722c 0000  filesr)...).r,..
+00000a50: 0072 3a00 0000 720f 0000 0072 1800 0000  .r:...r....r....
+00000a60: 7218 0000 0072 1900 0000 723b 0000 0053  r....r....r;...S
+00000a70: 0000 0073 0200 0000 0806 7a18 4669 6c65  ...s......z.File
+00000a80: 4465 6c65 6761 7465 2e71 7565 7279 5f66  Delegate.query_f
+00000a90: 696c 6573 da06 6275 636b 6574 da03 6b65  iles..bucket..ke
+00000aa0: 79da 0474 6167 7363 0700 0000 0000 0000  y..tagsc........
+00000ab0: 0000 0000 0700 0000 0200 0000 4300 0000  ............C...
+00000ac0: 7227 0000 00a9 024e da0b 7570 6c6f 6164  r'.....N..upload
+00000ad0: 5f66 696c 6572 2900 0000 2907 722c 0000  _filer)...).r,..
+00000ae0: 0072 2e00 0000 723c 0000 0072 3d00 0000  .r....r<...r=...
+00000af0: 722f 0000 0072 3e00 0000 7230 0000 0072  r/...r>...r0...r
+00000b00: 1800 0000 7218 0000 0072 1900 0000 7240  ....r....r....r@
+00000b10: 0000 005b 0000 0072 3600 0000 7a18 4669  ...[...r6...z.Fi
+00000b20: 6c65 4465 6c65 6761 7465 2e75 706c 6f61  leDelegate.uploa
+00000b30: 645f 6669 6c65 7209 0000 0063 0700 0000  d_filer....c....
+00000b40: 0000 0000 0000 0000 0700 0000 0200 0000  ................
+00000b50: 4300 0000 7227 0000 0072 3f00 0000 7229  C...r'...r?...r)
+00000b60: 0000 0029 0772 2c00 0000 723c 0000 0072  ...).r,...r<...r
+00000b70: 3300 0000 722f 0000 0072 3e00 0000 7230  3...r/...r>...r0
+00000b80: 0000 0072 3400 0000 7218 0000 0072 1800  ...r4...r....r..
+00000b90: 0000 7219 0000 00da 0c75 706c 6f61 645f  ..r......upload_
+00000ba0: 6669 6c65 7367 0000 0072 3600 0000 7a19  filesg...r6...z.
+00000bb0: 4669 6c65 4465 6c65 6761 7465 2e75 706c  FileDelegate.upl
+00000bc0: 6f61 645f 6669 6c65 7329 014e 291d 7211  oad_files).N).r.
+00000bd0: 0000 0072 1200 0000 7213 0000 00da 0361  ...r....r......a
+00000be0: 6263 da0e 6162 7374 7261 6374 6d65 7468  bc..abstractmeth
+00000bf0: 6f64 720c 0000 0072 2800 0000 720a 0000  odr....r(...r...
+00000c00: 00da 0770 6174 686c 6962 da04 5061 7468  ...pathlib..Path
+00000c10: 7223 0000 0072 0b00 0000 7231 0000 00da  r#...r....r1....
+00000c20: 0b63 6f6c 6c65 6374 696f 6e73 da09 4765  .collections..Ge
+00000c30: 6e65 7261 746f 72da 0574 7570 6c65 da03  nerator..tuple..
+00000c40: 696e 7472 3500 0000 7221 0000 0072 3800  intr5...r!...r8.
+00000c50: 0000 7239 0000 0072 0800 0000 7203 0000  ..r9...r....r...
+00000c60: 0072 0700 0000 723b 0000 00da 0464 6963  .r....r;.....dic
+00000c70: 7472 0d00 0000 7240 0000 0072 4100 0000  tr....r@...rA...
+00000c80: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+00000c90: 1900 0000 7224 0000 0030 0000 0073 a400  ....r$...0...s..
+00000ca0: 0000 0800 0401 1401 0403 0406 04fb 0202  ................
+00000cb0: 02fe 0403 02fd 0204 02fc 0205 02fb 0206  ................
+00000cc0: 0cfa 0409 0407 0201 04f9 0602 1201 02ff  ................
+00000cd0: 02fe 0205 02fb 0206 02fa 0207 02f9 0208  ................
+00000ce0: 0cf8 040b 1401 0403 1401 0403 0204 04fd  ................
+00000cf0: 0202 02fe 0603 02fd 0604 0cfc 0407 0207  ................
+00000d00: 0401 04f9 0402 02fe 0203 02fd 0204 02fc  ................
+00000d10: 0205 02fb 0e06 02fa 0207 02f9 0208 0cf8  ................
+00000d20: 040b 0206 0401 0201 04f9 0202 02fe 1a03  ................
+00000d30: 02fd 0204 02fc 0e05 02fb 0206 02fa 0207  ................
+00000d40: 02f9 0208 10f8 7224 0000 0029 1c72 4200  ......r$...).rB.
+00000d50: 0000 da0f 636f 6c6c 6563 7469 6f6e 732e  ....collections.
+00000d60: 6162 6372 4600 0000 da04 656e 756d 7244  abcrF.....enumrD
+00000d70: 0000 00da 0674 7970 696e 6772 0200 0000  .....typingr....
+00000d80: 7203 0000 0072 0400 0000 7205 0000 00da  r....r....r.....
+00000d90: 0b49 6d70 6f72 7445 7272 6f72 da11 7479  .ImportError..ty
+00000da0: 7069 6e67 5f65 7874 656e 7369 6f6e 73da  ping_extensions.
+00000db0: 0468 7474 7072 0700 0000 723a 0000 0072  .httpr....r:...r
+00000dc0: 0800 0000 da08 7072 6f67 7265 7373 720a  ......progressr.
+00000dd0: 0000 0072 0b00 0000 7225 0000 0072 0c00  ...r....r%...r..
+00000de0: 0000 da04 456e 756d 720d 0000 0072 1a00  ....Enumr....r..
+00000df0: 0000 7223 0000 0072 2200 0000 da03 4142  ..r#...r".....AB
+00000e00: 4372 2400 0000 7218 0000 0072 1800 0000  Cr$...r....r....
+00000e10: 7218 0000 0072 1900 0000 da08 3c6d 6f64  r....r......<mod
+00000e20: 756c 653e 0100 0000 732e 0000 000a 0008  ule>....s.......
+00000e30: 0108 0108 0114 0102 0310 010c 0102 0110  ................
+00000e40: 010c 0104 0102 ff04 8002 fd0c 060c 0110  ................
+00000e50: 010c 0412 0310 0814 0c16 03              ...........
```

### Comparing `roboto-0.2.8/src/roboto/domain/files/__pycache__/file.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/files/__pycache__/file.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3910 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 460f 0000  o........Y.eF...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 180f 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6403 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6403 6405 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6406  d.l.m.Z.m.Z...d.
@@ -18,266 +18,264 @@
 00000110: 7669 6465 72da 0c46 696c 6544 656c 6567  vider..FileDeleg
 00000120: 6174 6529 02da 1a4e 6f6f 7050 726f 6772  ate)...NoopProgr
 00000130: 6573 734d 6f6e 6974 6f72 4661 6374 6f72  essMonitorFactor
 00000140: 79da 1650 726f 6772 6573 734d 6f6e 6974  y..ProgressMonit
 00000150: 6f72 4661 6374 6f72 7929 01da 0a46 696c  orFactory)...Fil
 00000160: 6552 6563 6f72 6463 0000 0000 0000 0000  eRecordc........
 00000170: 0000 0000 0000 0000 0b00 0000 4000 0000  ............@...
-00000180: 7380 0100 0065 005a 0164 005a 0255 0065  s....e.Z.d.Z.U.e
+00000180: 7374 0100 0065 005a 0164 005a 0255 0065  st...e.Z.d.Z.U.e
 00000190: 0365 0464 013c 0065 0565 0464 023c 0065  .e.d.<.e.e.d.<.e
 000001a0: 0664 0365 0764 0465 0766 0464 0564 0684  .d.e.d.e.f.d.d..
 000001b0: 0483 015a 0865 0664 0765 0764 0865 0764  ...Z.e.d.e.d.e.d
 000001c0: 0465 0766 0664 0964 0a84 0483 015a 0965  .e.f.d.d.....Z.e
 000001d0: 0609 0b64 3064 0765 0764 0865 0764 0c65  ...d0d.e.d.e.d.e
 000001e0: 0a65 0719 0064 0465 0766 0864 0d64 0e84  .e...d.e.f.d.d..
-000001f0: 0583 015a 0b65 0c09 0b64 3064 0f65 0764  ...Z.e...d0d.e.d
-00000200: 1065 0364 1165 0a65 0719 0064 0464 0066  .e.d.e.e...d.d.f
-00000210: 0864 1264 1384 0583 015a 0d65 0c09 0b64  .d.d.....Z.e...d
-00000220: 3064 1465 0e64 1065 0364 1165 0a65 0719  0d.e.d.e.d.e.e..
-00000230: 0064 0465 0f6a 106a 1164 1519 0066 0864  .d.e.j.j.d...f.d
-00000240: 1664 1784 0583 015a 1264 1865 0564 1065  .d.....Z.d.e.d.e
-00000250: 0366 0464 1964 1a84 045a 1365 1464 0465  .f.d.d...Z.e.d.e
-00000260: 0766 0264 1b64 1c84 0483 015a 1565 1464  .f.d.d.....Z.e.d
-00000270: 0465 0766 0264 1d64 1e84 0483 015a 1665  .e.f.d.d.....Z.e
-00000280: 1464 0465 0766 0264 1f64 2084 0483 015a  .d.e.f.d.d ....Z
-00000290: 1765 1464 0465 0566 0264 2164 2284 0483  .e.d.e.f.d!d"...
-000002a0: 015a 1865 1464 0465 0766 0264 2364 2484  .Z.e.d.e.f.d#d$.
-000002b0: 0483 015a 1964 3164 2564 2684 045a 1a65  ...Z.d1d%d&..Z.e
-000002c0: 1b83 0066 0164 2765 1c6a 1d64 2865 1e64  ...f.d'e.j.d(e.d
-000002d0: 2965 1f66 0664 2a64 2b84 055a 2064 0465  )e.f.d*d+..Z d.e
-000002e0: 0766 0264 2c64 2d84 045a 2164 0465 2265  .f.d,d-..Z!d.e"e
-000002f0: 0765 2366 0219 0066 0264 2e64 2f84 045a  .e#f...f.d.d/..Z
-00000300: 2464 0b53 0029 32da 0446 696c 65da 0f5f  $d.S.)2..File.._
-00000310: 4669 6c65 5f5f 6465 6c65 6761 7465 da0d  File__delegate..
-00000320: 5f46 696c 655f 5f72 6563 6f72 64da 0375  _File__record..u
-00000330: 7269 da06 7265 7475 726e 6301 0000 0000  ri..returnc.....
-00000340: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00000350: 0000 0073 1800 0000 7400 6a01 7c00 a002  ...s....t.j.|...
-00000360: 6401 a101 6402 6403 8d02 a003 a100 5300  d...d.d.......S.
-00000370: 2904 7aa3 0a20 2020 2020 2020 2052 6574  ).z..        Ret
-00000380: 7572 6e20 6120 6669 7865 6420 7369 7a65  urn a fixed size
-00000390: 2028 3332 2063 6861 7261 6374 6572 292c   (32 character),
-000003a0: 2075 6e69 7175 6520 4944 2064 6574 6572   unique ID deter
-000003b0: 6d69 6e69 7374 6963 616c 6c79 2066 726f  ministically fro
-000003c0: 6d20 616e 204f 626a 6563 7427 7320 6275  m an Object's bu
-000003d0: 636b 6574 2061 6e64 206b 6579 2e0a 2020  cket and key..  
-000003e0: 2020 2020 2020 5665 7273 696f 6e65 6420        Versioned 
-000003f0: 6f62 6a65 6374 7320 7769 6c6c 2068 6176  objects will hav
-00000400: 6520 7468 6520 7361 6d65 2049 442e 0a20  e the same ID.. 
-00000410: 2020 2020 2020 207a 0575 7466 2d38 e910         z.utf-8..
-00000420: 0000 0029 01da 0b64 6967 6573 745f 7369  ...)...digest_si
-00000430: 7a65 2904 da07 6861 7368 6c69 62da 0762  ze)...hashlib..b
-00000440: 6c61 6b65 3262 da06 656e 636f 6465 da09  lake2b..encode..
-00000450: 6865 7864 6967 6573 7429 0172 1000 0000  hexdigest).r....
-00000460: a900 7218 0000 00fa e12f 636f 6465 6275  ..r....../codebu
-00000470: 696c 642f 6f75 7470 7574 2f73 7263 3130  ild/output/src10
-00000480: 3531 3138 3230 3839 2f73 7263 2f63 6f64  51182089/src/cod
-00000490: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
-000004a0: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
-000004b0: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
-000004c0: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
-000004d0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
-000004e0: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
-000004f0: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
-00000500: 6f62 6f74 6f2d 6169 2f72 6f62 6f74 6f2d  oboto-ai/roboto-
-00000510: 686f 7374 6564 2d61 7070 2f70 6163 6b61  hosted-app/packa
-00000520: 6765 732f 726f 626f 746f 2f73 7263 2f72  ges/roboto/src/r
-00000530: 6f62 6f74 6f2f 646f 6d61 696e 2f66 696c  oboto/domain/fil
-00000540: 6573 2f66 696c 652e 7079 da0f 636f 6d70  es/file.py..comp
-00000550: 7574 655f 6669 6c65 5f69 6417 0000 0073  ute_file_id....s
-00000560: 0200 0000 1806 7a14 4669 6c65 2e63 6f6d  ......z.File.com
-00000570: 7075 7465 5f66 696c 655f 6964 da06 6275  pute_file_id..bu
-00000580: 636b 6574 da03 6b65 7963 0200 0000 0000  cket..keyc......
-00000590: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-000005a0: 0000 7310 0000 0064 017c 009b 0064 027c  ..s....d.|...d.|
-000005b0: 019b 009d 0453 0029 034e 7a0d 6172 6e3a  .....S.).Nz.arn:
-000005c0: 6177 733a 7333 3a3a 3ada 012f 7218 0000  aws:s3:::../r...
-000005d0: 0029 0272 1b00 0000 721c 0000 0072 1800  .).r....r....r..
-000005e0: 0000 7218 0000 0072 1900 0000 da14 636f  ..r....r......co
-000005f0: 6e73 7472 7563 745f 7333 5f6f 626a 5f61  nstruct_s3_obj_a
-00000600: 726e 1f00 0000 7302 0000 0010 027a 1946  rn....s......z.F
-00000610: 696c 652e 636f 6e73 7472 7563 745f 7333  ile.construct_s3
-00000620: 5f6f 626a 5f61 726e 4eda 0776 6572 7369  _obj_arnN..versi
-00000630: 6f6e 6303 0000 0000 0000 0000 0000 0004  onc.............
-00000640: 0000 0004 0000 0043 0000 0073 2600 0000  .......C...s&...
-00000650: 6401 7c00 9b00 6402 7c01 9b00 9d04 7d03  d.|...d.|.....}.
-00000660: 7c02 7211 7c03 6403 7c02 9b00 9d02 3700  |.r.|.d.|.....7.
-00000670: 7d03 7c03 5300 2904 4e7a 0573 333a 2f2f  }.|.S.).Nz.s3://
-00000680: 721d 0000 007a 0b3f 7665 7273 696f 6e49  r....z.?versionI
-00000690: 643d 7218 0000 0029 0472 1b00 0000 721c  d=r....).r....r.
-000006a0: 0000 0072 1f00 0000 5a08 6261 7365 5f75  ...r....Z.base_u
-000006b0: 7269 7218 0000 0072 1800 0000 7219 0000  rir....r....r...
-000006c0: 00da 1463 6f6e 7374 7275 6374 5f73 335f  ...construct_s3_
-000006d0: 6f62 6a5f 7572 6923 0000 0073 0800 0000  obj_uri#...s....
-000006e0: 1004 0401 0e01 0401 7a19 4669 6c65 2e63  ........z.File.c
-000006f0: 6f6e 7374 7275 6374 5f73 335f 6f62 6a5f  onstruct_s3_obj_
-00000700: 7572 69da 0766 696c 655f 6964 da08 6465  uri..file_id..de
-00000710: 6c65 6761 7465 da06 6f72 675f 6964 6304  legate..org_idc.
-00000720: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00000730: 0000 0043 0000 0073 1600 0000 7c02 a000  ...C...s....|...
-00000740: 7c01 7c03 a102 7d04 7c00 7c04 7c02 8302  |.|...}.|.|.|...
-00000750: 5300 a901 4e29 01da 1967 6574 5f72 6563  S...N)...get_rec
-00000760: 6f72 645f 6279 5f70 7269 6d61 7279 5f6b  ord_by_primary_k
-00000770: 6579 2905 da03 636c 7372 2100 0000 7222  ey)...clsr!...r"
-00000780: 0000 0072 2300 0000 da06 7265 636f 7264  ...r#.....record
-00000790: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-000007a0: 0766 726f 6d5f 6964 2c00 0000 7304 0000  .from_id,...s...
-000007b0: 000c 070a 017a 0c46 696c 652e 6672 6f6d  .....z.File.from
-000007c0: 5f69 64da 0571 7565 7279 2903 720d 0000  _id..query).r...
-000007d0: 004e 4e63 0400 0000 0000 0000 0000 0000  .NNc............
-000007e0: 0c00 0000 0600 0000 6300 0000 73d4 0000  ........c...s...
-000007f0: 0081 0074 0074 016a 02a0 03a1 0083 017d  ...t.t.j.......}
-00000800: 0474 0083 007d 057c 01a0 04a1 0044 005d  .t...}.|.....D.]
-00000810: 167d 0664 017c 0676 0072 207c 05a0 057c  .}.d.|.v.r |...|
-00000820: 06a0 0664 01a1 0164 0219 00a1 0101 0071  ...d...d.......q
-00000830: 0f7c 05a0 057c 06a1 0101 0071 0f7c 057c  .|...|.....q.|.|
-00000840: 0418 007d 077c 0772 4474 077c 0783 0164  ...}.|.rDt.|...d
-00000850: 036b 047d 087c 0872 3664 046e 0164 057d  .k.}.|.r6d.n.d.}
-00000860: 0974 087c 079b 0064 067c 099b 0064 077c  .t.|...d.|...d.|
-00000870: 049b 009d 0583 0182 017c 026a 097c 017c  .........|.j.|.|
-00000880: 0364 088d 027d 0a09 007c 0a6a 0a44 005d  .d...}...|.j.D.]
-00000890: 087d 0b7c 007c 0b7c 0283 0256 0001 0071  .}.|.|.|...V...q
-000008a0: 4f7c 0a6a 0b72 677c 0a6a 0b7c 015f 0c7c  O|.j.rg|.j.|._.|
-000008b0: 026a 097c 017c 0364 088d 027d 0a6e 0264  .j.|.|.d...}.n.d
-000008c0: 0053 0071 4c29 094e da01 2e72 0100 0000  .S.qL).N...r....
-000008d0: 7207 0000 007a 2061 7265 206e 6f74 206b  r....z are not k
-000008e0: 6e6f 776e 2061 7474 7269 6275 7465 7320  nown attributes 
-000008f0: 6f66 2046 696c 657a 2069 7320 6e6f 7420  of Filez is not 
-00000900: 6120 6b6e 6f77 6e20 6174 7472 6962 7574  a known attribut
-00000910: 6520 6f66 2046 696c 65da 0120 7a14 2e20  e of File.. z.. 
-00000920: 4b6e 6f77 6e20 6174 7472 6962 7574 6573  Known attributes
-00000930: 3a20 2901 7223 0000 0029 0dda 0373 6574  : ).r#...)...set
-00000940: 720c 0000 00da 0c6d 6f64 656c 5f66 6965  r......model_fie
-00000950: 6c64 73da 046b 6579 73da 0666 6965 6c64  lds..keys..field
-00000960: 73da 0361 6464 da05 7370 6c69 74da 036c  s..add..split..l
-00000970: 656e da0a 5661 6c75 6545 7272 6f72 da0b  en..ValueError..
-00000980: 7175 6572 795f 6669 6c65 73da 0569 7465  query_files..ite
-00000990: 6d73 da0a 6e65 7874 5f74 6f6b 656e da05  ms..next_token..
-000009a0: 6166 7465 7229 0c72 2600 0000 7229 0000  after).r&...r)..
-000009b0: 0072 2200 0000 7223 0000 00da 056b 6e6f  .r"...r#.....kno
-000009c0: 776e da06 6163 7475 616c da05 6669 656c  wn..actual..fiel
-000009d0: 64da 0775 6e6b 6e6f 776e da06 706c 7572  d..unknown..plur
-000009e0: 616c da03 6d73 67da 1170 6167 696e 6174  al..msg..paginat
-000009f0: 6564 5f72 6573 756c 7473 7227 0000 0072  ed_resultsr'...r
-00000a00: 1800 0000 7218 0000 0072 1900 0000 7229  ....r....r....r)
-00000a10: 0000 0036 0000 0073 3000 0000 0280 0e07  ...6...s0.......
-00000a20: 0601 0c01 0803 1601 0c02 0801 0401 0c01  ................
-00000a30: 0203 06ff 0202 02fd 1805 0e02 0201 0a01  ................
-00000a40: 0e01 0601 0801 1001 0402 02f9 7a0a 4669  ............z.Fi
-00000a50: 6c65 2e71 7565 7279 7227 0000 0063 0300  le.queryr'...c..
-00000a60: 0000 0000 0000 0000 0000 0300 0000 0200  ................
-00000a70: 0000 4300 0000 7310 0000 007c 017c 005f  ..C...s....|.|._
-00000a80: 007c 027c 005f 0164 0053 0072 2400 0000  .|.|._.d.S.r$...
-00000a90: 2902 720f 0000 0072 0e00 0000 2903 da04  ).r....r....)...
-00000aa0: 7365 6c66 7227 0000 0072 2200 0000 7218  selfr'...r"...r.
-00000ab0: 0000 0072 1800 0000 7219 0000 00da 085f  ...r....r......_
-00000ac0: 5f69 6e69 745f 5f5a 0000 0073 0400 0000  _init__Z...s....
-00000ad0: 0601 0a01 7a0d 4669 6c65 2e5f 5f69 6e69  ....z.File.__ini
-00000ae0: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-00000af0: 0100 0000 0100 0000 4300 0000 f308 0000  ........C.......
-00000b00: 007c 006a 006a 0153 0072 2400 0000 2902  .|.j.j.S.r$...).
-00000b10: 720f 0000 0072 2100 0000 a901 723f 0000  r....r!.....r?..
-00000b20: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000b30: 7221 0000 005e 0000 00f3 0200 0000 0802  r!...^..........
-00000b40: 7a0c 4669 6c65 2e66 696c 655f 6964 6301  z.File.file_idc.
-00000b50: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000b60: 0000 0043 0000 0072 4100 0000 7224 0000  ...C...rA...r$..
-00000b70: 0029 0272 0f00 0000 7223 0000 0072 4200  .).r....r#...rB.
-00000b80: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000b90: 0072 2300 0000 6200 0000 7243 0000 007a  .r#...b...rC...z
-00000ba0: 0b46 696c 652e 6f72 675f 6964 6301 0000  .File.org_idc...
-00000bb0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00000bc0: 0043 0000 0072 4100 0000 7224 0000 0029  .C...rA...r$...)
-00000bd0: 0272 0f00 0000 7210 0000 0072 4200 0000  .r....r....rB...
-00000be0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00000bf0: 1000 0000 6600 0000 7243 0000 007a 0846  ....f...rC...z.F
-00000c00: 696c 652e 7572 6963 0100 0000 0000 0000  ile.uric........
-00000c10: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000c20: 7306 0000 007c 006a 0053 0072 2400 0000  s....|.j.S.r$...
-00000c30: 2901 720f 0000 0072 4200 0000 7218 0000  ).r....rB...r...
-00000c40: 0072 1800 0000 7219 0000 0072 2700 0000  .r....r....r'...
-00000c50: 6a00 0000 7302 0000 0006 027a 0b46 696c  j...s......z.Fil
-00000c60: 652e 7265 636f 7264 6301 0000 0000 0000  e.recordc.......
-00000c70: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00000c80: 0072 4100 0000 7224 0000 0029 0272 0f00  .rA...r$...).r..
-00000c90: 0000 da0d 7265 6c61 7469 7665 5f70 6174  ....relative_pat
-00000ca0: 6872 4200 0000 7218 0000 0072 1800 0000  hrB...r....r....
-00000cb0: 7219 0000 0072 4400 0000 6e00 0000 7243  r....rD...n...rC
-00000cc0: 0000 007a 1246 696c 652e 7265 6c61 7469  ...z.File.relati
-00000cd0: 7665 5f70 6174 6863 0100 0000 0000 0000  ve_pathc........
-00000ce0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-00000cf0: 7312 0000 007c 006a 00a0 017c 006a 02a1  s....|.j...|.j..
-00000d00: 0101 0064 0053 0072 2400 0000 2903 720e  ...d.S.r$...).r.
-00000d10: 0000 00da 0b64 656c 6574 655f 6669 6c65  .....delete_file
-00000d20: 720f 0000 0072 4200 0000 7218 0000 0072  r....rB...r....r
-00000d30: 1800 0000 7219 0000 00da 0664 656c 6574  ....r......delet
-00000d40: 6572 0000 0073 0200 0000 1201 7a0b 4669  er...s......z.Fi
-00000d50: 6c65 2e64 656c 6574 65da 0a6c 6f63 616c  le.delete..local
-00000d60: 5f70 6174 68da 1363 7265 6465 6e74 6961  _path..credentia
-00000d70: 6c5f 7072 6f76 6964 6572 da18 7072 6f67  l_provider..prog
-00000d80: 7265 7373 5f6d 6f6e 6974 6f72 5f66 6163  ress_monitor_fac
-00000d90: 746f 7279 6304 0000 0000 0000 0000 0000  toryc...........
-00000da0: 0004 0000 0006 0000 0043 0000 0073 1a00  .........C...s..
-00000db0: 0000 7c00 6a00 6a01 7c00 6a02 7c01 7c02  ..|.j.j.|.j.|.|.
-00000dc0: 7c03 6401 8d04 0100 6400 5300 2902 4e29  |.d.....d.S.).N)
-00000dd0: 0172 4900 0000 2903 720e 0000 00da 0d64  .rI...).r......d
-00000de0: 6f77 6e6c 6f61 645f 6669 6c65 720f 0000  ownload_filer...
-00000df0: 0029 0472 3f00 0000 7247 0000 0072 4800  .).r?...rG...rH.
-00000e00: 0000 7249 0000 0072 1800 0000 7218 0000  ..rI...r....r...
-00000e10: 0072 1900 0000 da08 646f 776e 6c6f 6164  .r......download
-00000e20: 7500 0000 730c 0000 0006 0604 0102 0102  u...s...........
-00000e30: 0102 010a fc7a 0d46 696c 652e 646f 776e  .....z.File.down
-00000e40: 6c6f 6164 6301 0000 0000 0000 0000 0000  loadc...........
-00000e50: 0001 0000 0003 0000 0043 0000 0073 0e00  .........C...s..
-00000e60: 0000 7c00 6a00 a001 7c00 6a02 a101 5300  ..|.j...|.j...S.
-00000e70: 7224 0000 0029 0372 0e00 0000 da0e 6765  r$...).r......ge
-00000e80: 745f 7369 676e 6564 5f75 726c 720f 0000  t_signed_urlr...
-00000e90: 0072 4200 0000 7218 0000 0072 1800 0000  .rB...r....r....
-00000ea0: 7219 0000 0072 4c00 0000 8200 0000 7302  r....rL.......s.
-00000eb0: 0000 000e 017a 1346 696c 652e 6765 745f  .....z.File.get_
-00000ec0: 7369 676e 6564 5f75 726c 6301 0000 0000  signed_urlc.....
-00000ed0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000ee0: 0000 0073 0a00 0000 7400 7c00 6a01 8301  ...s....t.|.j...
-00000ef0: 5300 7224 0000 0029 0272 0600 0000 720f  S.r$...).r....r.
-00000f00: 0000 0072 4200 0000 7218 0000 0072 1800  ...rB...r....r..
-00000f10: 0000 7219 0000 00da 0774 6f5f 6469 6374  ..r......to_dict
-00000f20: 8500 0000 7302 0000 000a 017a 0c46 696c  ....s......z.Fil
-00000f30: 652e 746f 5f64 6963 7472 2400 0000 2902  e.to_dictr$...).
-00000f40: 7211 0000 004e 2925 da08 5f5f 6e61 6d65  r....N)%..__name
-00000f50: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000f60: 5f5f 7175 616c 6e61 6d65 5f5f 7209 0000  __qualname__r...
-00000f70: 00da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  ...__annotations
-00000f80: 5f5f 720c 0000 00da 0c73 7461 7469 636d  __r......staticm
-00000f90: 6574 686f 64da 0373 7472 721a 0000 0072  ethod..strr....r
-00000fa0: 1e00 0000 7203 0000 0072 2000 0000 da0b  ....r....r .....
-00000fb0: 636c 6173 736d 6574 686f 6472 2800 0000  classmethodr(...
-00000fc0: 7205 0000 00da 0b63 6f6c 6c65 6374 696f  r......collectio
-00000fd0: 6e73 da03 6162 63da 0947 656e 6572 6174  ns..abc..Generat
-00000fe0: 6f72 7229 0000 0072 4000 0000 da08 7072  orr)...r@.....pr
-00000ff0: 6f70 6572 7479 7221 0000 0072 2300 0000  opertyr!...r#...
-00001000: 7210 0000 0072 2700 0000 7244 0000 0072  r....r'...rD...r
-00001010: 4600 0000 720a 0000 00da 0770 6174 686c  F...r......pathl
-00001020: 6962 da04 5061 7468 7208 0000 0072 0b00  ib..Pathr....r..
-00001030: 0000 724b 0000 0072 4c00 0000 da04 6469  ..rK...rL.....di
-00001040: 6374 7202 0000 0072 4d00 0000 7218 0000  ctr....rM...r...
-00001050: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00001060: 720d 0000 0013 0000 0073 7c00 0000 0a00  r........s|.....
-00001070: 0801 0801 0202 1401 0207 1801 0203 0202  ................
-00001080: 04ff 0201 02ff 0201 02ff 0601 02ff 0202  ................
-00001090: 0cfe 0208 0205 04fc 0202 02fe 0203 02fd  ................
-000010a0: 0604 02fc 0205 0cfb 0209 0205 04fc 0202  ................
-000010b0: 02fe 0203 02fd 0604 02fc 0a05 0cfb 1223  ...............#
-000010c0: 0204 1001 0203 1001 0203 1001 0203 1001  ................
-000010d0: 0203 1001 0a03 0407 04fc 0402 02fe 0203  ................
-000010e0: 02fd 0204 0afc 0e0d 1a03 720d 0000 0029  ..........r....)
-000010f0: 14da 0f63 6f6c 6c65 6374 696f 6e73 2e61  ...collections.a
-00001100: 6263 7255 0000 0072 1400 0000 7259 0000  bcrU...r....rY..
-00001110: 00da 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
-00001120: 0000 0072 2900 0000 7205 0000 00da 0573  ...r)...r......s
-00001130: 6572 6465 7206 0000 0072 2200 0000 7208  erder....r"...r.
-00001140: 0000 0072 0900 0000 da08 7072 6f67 7265  ...r......progre
-00001150: 7373 720a 0000 0072 0b00 0000 7227 0000  ssr....r....r'..
-00001160: 0072 0c00 0000 720d 0000 0072 1800 0000  .r....r....r....
-00001170: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00001180: 083c 6d6f 6475 6c65 3e01 0000 0073 1400  .<module>....s..
-00001190: 0000 0800 0801 0801 1001 0c02 0c01 1001  ................
-000011a0: 1004 0c04 1203                           ......
+000001f0: 0583 015a 0b65 0c64 0f65 0764 1065 0364  ...Z.e.d.e.d.e.d
+00000200: 0464 0066 0664 1164 1284 0483 015a 0d65  .d.f.d.d.....Z.e
+00000210: 0c09 0b64 3064 1365 0e64 1065 0364 1465  ...d0d.e.d.e.d.e
+00000220: 0a65 0719 0064 0465 0f6a 106a 1164 1519  .e...d.e.j.j.d..
+00000230: 0066 0864 1664 1784 0583 015a 1264 1865  .f.d.d.....Z.d.e
+00000240: 0564 1065 0366 0464 1964 1a84 045a 1365  .d.e.f.d.d...Z.e
+00000250: 1464 0465 0766 0264 1b64 1c84 0483 015a  .d.e.f.d.d.....Z
+00000260: 1565 1464 0465 0766 0264 1d64 1e84 0483  .e.d.e.f.d.d....
+00000270: 015a 1665 1464 0465 0766 0264 1f64 2084  .Z.e.d.e.f.d.d .
+00000280: 0483 015a 1765 1464 0465 0566 0264 2164  ...Z.e.d.e.f.d!d
+00000290: 2284 0483 015a 1865 1464 0465 0766 0264  "....Z.e.d.e.f.d
+000002a0: 2364 2484 0483 015a 1964 3164 2564 2684  #d$....Z.d1d%d&.
+000002b0: 045a 1a65 1b83 0066 0164 2765 1c6a 1d64  .Z.e...f.d'e.j.d
+000002c0: 2865 1e64 2965 1f66 0664 2a64 2b84 055a  (e.d)e.f.d*d+..Z
+000002d0: 2064 0465 0766 0264 2c64 2d84 045a 2164   d.e.f.d,d-..Z!d
+000002e0: 0465 2265 0765 2366 0219 0066 0264 2e64  .e"e.e#f...f.d.d
+000002f0: 2f84 045a 2464 0b53 0029 32da 0446 696c  /..Z$d.S.)2..Fil
+00000300: 65da 0f5f 4669 6c65 5f5f 6465 6c65 6761  e.._File__delega
+00000310: 7465 da0d 5f46 696c 655f 5f72 6563 6f72  te.._File__recor
+00000320: 64da 0375 7269 da06 7265 7475 726e 6301  d..uri..returnc.
+00000330: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000340: 0000 0043 0000 0073 1800 0000 7400 6a01  ...C...s....t.j.
+00000350: 7c00 a002 6401 a101 6402 6403 8d02 a003  |...d...d.d.....
+00000360: a100 5300 2904 7aa3 0a20 2020 2020 2020  ..S.).z..       
+00000370: 2052 6574 7572 6e20 6120 6669 7865 6420   Return a fixed 
+00000380: 7369 7a65 2028 3332 2063 6861 7261 6374  size (32 charact
+00000390: 6572 292c 2075 6e69 7175 6520 4944 2064  er), unique ID d
+000003a0: 6574 6572 6d69 6e69 7374 6963 616c 6c79  eterministically
+000003b0: 2066 726f 6d20 616e 204f 626a 6563 7427   from an Object'
+000003c0: 7320 6275 636b 6574 2061 6e64 206b 6579  s bucket and key
+000003d0: 2e0a 2020 2020 2020 2020 5665 7273 696f  ..        Versio
+000003e0: 6e65 6420 6f62 6a65 6374 7320 7769 6c6c  ned objects will
+000003f0: 2068 6176 6520 7468 6520 7361 6d65 2049   have the same I
+00000400: 442e 0a20 2020 2020 2020 207a 0575 7466  D..        z.utf
+00000410: 2d38 e910 0000 0029 01da 0b64 6967 6573  -8.....)...diges
+00000420: 745f 7369 7a65 2904 da07 6861 7368 6c69  t_size)...hashli
+00000430: 62da 0762 6c61 6b65 3262 da06 656e 636f  b..blake2b..enco
+00000440: 6465 da09 6865 7864 6967 6573 7429 0172  de..hexdigest).r
+00000450: 1000 0000 a900 7218 0000 00fa e12f 636f  ......r....../co
+00000460: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
+00000470: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
+00000480: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
+00000490: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
+000004a0: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
+000004b0: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
+000004c0: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
+000004d0: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
+000004e0: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
+000004f0: 3964 2f72 6f62 6f74 6f2d 6169 2f72 6f62  9d/roboto-ai/rob
+00000500: 6f74 6f2d 686f 7374 6564 2d61 7070 2f70  oto-hosted-app/p
+00000510: 6163 6b61 6765 732f 726f 626f 746f 2f73  ackages/roboto/s
+00000520: 7263 2f72 6f62 6f74 6f2f 646f 6d61 696e  rc/roboto/domain
+00000530: 2f66 696c 6573 2f66 696c 652e 7079 da0f  /files/file.py..
+00000540: 636f 6d70 7574 655f 6669 6c65 5f69 6417  compute_file_id.
+00000550: 0000 0073 0200 0000 1806 7a14 4669 6c65  ...s......z.File
+00000560: 2e63 6f6d 7075 7465 5f66 696c 655f 6964  .compute_file_id
+00000570: da06 6275 636b 6574 da03 6b65 7963 0200  ..bucket..keyc..
+00000580: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000590: 0000 4300 0000 7310 0000 0064 017c 009b  ..C...s....d.|..
+000005a0: 0064 027c 019b 009d 0453 0029 034e 7a0d  .d.|.....S.).Nz.
+000005b0: 6172 6e3a 6177 733a 7333 3a3a 3ada 012f  arn:aws:s3:::../
+000005c0: 7218 0000 0029 0272 1b00 0000 721c 0000  r....).r....r...
+000005d0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+000005e0: da14 636f 6e73 7472 7563 745f 7333 5f6f  ..construct_s3_o
+000005f0: 626a 5f61 726e 1f00 0000 7302 0000 0010  bj_arn....s.....
+00000600: 027a 1946 696c 652e 636f 6e73 7472 7563  .z.File.construc
+00000610: 745f 7333 5f6f 626a 5f61 726e 4eda 0776  t_s3_obj_arnN..v
+00000620: 6572 7369 6f6e 6303 0000 0000 0000 0000  ersionc.........
+00000630: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
+00000640: 2600 0000 6401 7c00 9b00 6402 7c01 9b00  &...d.|...d.|...
+00000650: 9d04 7d03 7c02 7211 7c03 6403 7c02 9b00  ..}.|.r.|.d.|...
+00000660: 9d02 3700 7d03 7c03 5300 2904 4e7a 0573  ..7.}.|.S.).Nz.s
+00000670: 333a 2f2f 721d 0000 007a 0b3f 7665 7273  3://r....z.?vers
+00000680: 696f 6e49 643d 7218 0000 0029 0472 1b00  ionId=r....).r..
+00000690: 0000 721c 0000 0072 1f00 0000 5a08 6261  ..r....r....Z.ba
+000006a0: 7365 5f75 7269 7218 0000 0072 1800 0000  se_urir....r....
+000006b0: 7219 0000 00da 1463 6f6e 7374 7275 6374  r......construct
+000006c0: 5f73 335f 6f62 6a5f 7572 6923 0000 0073  _s3_obj_uri#...s
+000006d0: 0800 0000 1004 0401 0e01 0401 7a19 4669  ............z.Fi
+000006e0: 6c65 2e63 6f6e 7374 7275 6374 5f73 335f  le.construct_s3_
+000006f0: 6f62 6a5f 7572 69da 0766 696c 655f 6964  obj_uri..file_id
+00000700: da08 6465 6c65 6761 7465 6303 0000 0000  ..delegatec.....
+00000710: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
+00000720: 0000 0073 1400 0000 7c02 a000 7c01 a101  ...s....|...|...
+00000730: 7d03 7c00 7c03 7c02 8302 5300 a901 4e29  }.|.|.|...S...N)
+00000740: 01da 1967 6574 5f72 6563 6f72 645f 6279  ...get_record_by
+00000750: 5f70 7269 6d61 7279 5f6b 6579 2904 da03  _primary_key)...
+00000760: 636c 7372 2100 0000 7222 0000 00da 0672  clsr!...r".....r
+00000770: 6563 6f72 6472 1800 0000 7218 0000 0072  ecordr....r....r
+00000780: 1900 0000 da07 6672 6f6d 5f69 642c 0000  ......from_id,..
+00000790: 0073 0400 0000 0a06 0a01 7a0c 4669 6c65  .s........z.File
+000007a0: 2e66 726f 6d5f 6964 da05 7175 6572 79da  .from_id..query.
+000007b0: 066f 7267 5f69 6429 0372 0d00 0000 4e4e  .org_id).r....NN
+000007c0: 6304 0000 0000 0000 0000 0000 000c 0000  c...............
+000007d0: 0006 0000 0063 0000 0073 d400 0000 8100  .....c...s......
+000007e0: 7400 7401 6a02 a003 a100 8301 7d04 7400  t.t.j.......}.t.
+000007f0: 8300 7d05 7c01 a004 a100 4400 5d16 7d06  ..}.|.....D.].}.
+00000800: 6401 7c06 7600 7220 7c05 a005 7c06 a006  d.|.v.r |...|...
+00000810: 6401 a101 6402 1900 a101 0100 710f 7c05  d...d.......q.|.
+00000820: a005 7c06 a101 0100 710f 7c05 7c04 1800  ..|.....q.|.|...
+00000830: 7d07 7c07 7244 7407 7c07 8301 6403 6b04  }.|.rDt.|...d.k.
+00000840: 7d08 7c08 7236 6404 6e01 6405 7d09 7408  }.|.r6d.n.d.}.t.
+00000850: 7c07 9b00 6406 7c09 9b00 6407 7c04 9b00  |...d.|...d.|...
+00000860: 9d05 8301 8201 7c02 6a09 7c01 7c03 6408  ......|.j.|.|.d.
+00000870: 8d02 7d0a 0900 7c0a 6a0a 4400 5d08 7d0b  ..}...|.j.D.].}.
+00000880: 7c00 7c0b 7c02 8302 5600 0100 714f 7c0a  |.|.|...V...qO|.
+00000890: 6a0b 7267 7c0a 6a0b 7c01 5f0c 7c02 6a09  j.rg|.j.|._.|.j.
+000008a0: 7c01 7c03 6408 8d02 7d0a 6e02 6400 5300  |.|.d...}.n.d.S.
+000008b0: 714c 2909 4eda 012e 7201 0000 0072 0700  qL).N...r....r..
+000008c0: 0000 7a20 6172 6520 6e6f 7420 6b6e 6f77  ..z are not know
+000008d0: 6e20 6174 7472 6962 7574 6573 206f 6620  n attributes of 
+000008e0: 4669 6c65 7a20 6973 206e 6f74 2061 206b  Filez is not a k
+000008f0: 6e6f 776e 2061 7474 7269 6275 7465 206f  nown attribute o
+00000900: 6620 4669 6c65 da01 207a 142e 204b 6e6f  f File.. z.. Kno
+00000910: 776e 2061 7474 7269 6275 7465 733a 2029  wn attributes: )
+00000920: 0172 2900 0000 290d da03 7365 7472 0c00  .r)...)...setr..
+00000930: 0000 da0c 6d6f 6465 6c5f 6669 656c 6473  ....model_fields
+00000940: da04 6b65 7973 da06 6669 656c 6473 da03  ..keys..fields..
+00000950: 6164 64da 0573 706c 6974 da03 6c65 6eda  add..split..len.
+00000960: 0a56 616c 7565 4572 726f 72da 0b71 7565  .ValueError..que
+00000970: 7279 5f66 696c 6573 da05 6974 656d 73da  ry_files..items.
+00000980: 0a6e 6578 745f 746f 6b65 6eda 0561 6674  .next_token..aft
+00000990: 6572 290c 7225 0000 0072 2800 0000 7222  er).r%...r(...r"
+000009a0: 0000 0072 2900 0000 da05 6b6e 6f77 6eda  ...r).....known.
+000009b0: 0661 6374 7561 6cda 0566 6965 6c64 da07  .actual..field..
+000009c0: 756e 6b6e 6f77 6eda 0670 6c75 7261 6cda  unknown..plural.
+000009d0: 036d 7367 da11 7061 6769 6e61 7465 645f  .msg..paginated_
+000009e0: 7265 7375 6c74 7372 2600 0000 7218 0000  resultsr&...r...
+000009f0: 0072 1800 0000 7219 0000 0072 2800 0000  .r....r....r(...
+00000a00: 3500 0000 7330 0000 0002 800e 0706 010c  5...s0..........
+00000a10: 0108 0316 010c 0208 0104 010c 0102 0306  ................
+00000a20: ff02 0202 fd18 050e 0202 010a 010e 0106  ................
+00000a30: 0108 0110 0104 0202 f97a 0a46 696c 652e  .........z.File.
+00000a40: 7175 6572 7972 2600 0000 6303 0000 0000  queryr&...c.....
+00000a50: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
+00000a60: 0000 0073 1000 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
+00000a70: 7c00 5f01 6400 5300 7223 0000 0029 0272  |._.d.S.r#...).r
+00000a80: 0f00 0000 720e 0000 0029 03da 0473 656c  ....r....)...sel
+00000a90: 6672 2600 0000 7222 0000 0072 1800 0000  fr&...r"...r....
+00000aa0: 7218 0000 0072 1900 0000 da08 5f5f 696e  r....r......__in
+00000ab0: 6974 5f5f 5900 0000 7304 0000 0006 010a  it__Y...s.......
+00000ac0: 017a 0d46 696c 652e 5f5f 696e 6974 5f5f  .z.File.__init__
+00000ad0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000ae0: 0001 0000 0043 0000 00f3 0800 0000 7c00  .....C........|.
+00000af0: 6a00 6a01 5300 7223 0000 0029 0272 0f00  j.j.S.r#...).r..
+00000b00: 0000 7221 0000 00a9 0172 3f00 0000 7218  ..r!.....r?...r.
+00000b10: 0000 0072 1800 0000 7219 0000 0072 2100  ...r....r....r!.
+00000b20: 0000 5d00 0000 f302 0000 0008 027a 0c46  ..]..........z.F
+00000b30: 696c 652e 6669 6c65 5f69 6463 0100 0000  ile.file_idc....
+00000b40: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00000b50: 4300 0000 7241 0000 0072 2300 0000 2902  C...rA...r#...).
+00000b60: 720f 0000 0072 2900 0000 7242 0000 0072  r....r)...rB...r
+00000b70: 1800 0000 7218 0000 0072 1900 0000 7229  ....r....r....r)
+00000b80: 0000 0061 0000 0072 4300 0000 7a0b 4669  ...a...rC...z.Fi
+00000b90: 6c65 2e6f 7267 5f69 6463 0100 0000 0000  le.org_idc......
+00000ba0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000bb0: 0000 7241 0000 0072 2300 0000 2902 720f  ..rA...r#...).r.
+00000bc0: 0000 0072 1000 0000 7242 0000 0072 1800  ...r....rB...r..
+00000bd0: 0000 7218 0000 0072 1900 0000 7210 0000  ..r....r....r...
+00000be0: 0065 0000 0072 4300 0000 7a08 4669 6c65  .e...rC...z.File
+00000bf0: 2e75 7269 6301 0000 0000 0000 0000 0000  .uric...........
+00000c00: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
+00000c10: 0000 7c00 6a00 5300 7223 0000 0029 0172  ..|.j.S.r#...).r
+00000c20: 0f00 0000 7242 0000 0072 1800 0000 7218  ....rB...r....r.
+00000c30: 0000 0072 1900 0000 7226 0000 0069 0000  ...r....r&...i..
+00000c40: 0073 0200 0000 0602 7a0b 4669 6c65 2e72  .s......z.File.r
+00000c50: 6563 6f72 6463 0100 0000 0000 0000 0000  ecordc..........
+00000c60: 0000 0100 0000 0100 0000 4300 0000 7241  ..........C...rA
+00000c70: 0000 0072 2300 0000 2902 720f 0000 00da  ...r#...).r.....
+00000c80: 0d72 656c 6174 6976 655f 7061 7468 7242  .relative_pathrB
+00000c90: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00000ca0: 0000 7244 0000 006d 0000 0072 4300 0000  ..rD...m...rC...
+00000cb0: 7a12 4669 6c65 2e72 656c 6174 6976 655f  z.File.relative_
+00000cc0: 7061 7468 6301 0000 0000 0000 0000 0000  pathc...........
+00000cd0: 0001 0000 0003 0000 0043 0000 0073 1200  .........C...s..
+00000ce0: 0000 7c00 6a00 a001 7c00 6a02 a101 0100  ..|.j...|.j.....
+00000cf0: 6400 5300 7223 0000 0029 0372 0e00 0000  d.S.r#...).r....
+00000d00: da0b 6465 6c65 7465 5f66 696c 6572 0f00  ..delete_filer..
+00000d10: 0000 7242 0000 0072 1800 0000 7218 0000  ..rB...r....r...
+00000d20: 0072 1900 0000 da06 6465 6c65 7465 7100  .r......deleteq.
+00000d30: 0000 7302 0000 0012 017a 0b46 696c 652e  ..s......z.File.
+00000d40: 6465 6c65 7465 da0a 6c6f 6361 6c5f 7061  delete..local_pa
+00000d50: 7468 da13 6372 6564 656e 7469 616c 5f70  th..credential_p
+00000d60: 726f 7669 6465 72da 1870 726f 6772 6573  rovider..progres
+00000d70: 735f 6d6f 6e69 746f 725f 6661 6374 6f72  s_monitor_factor
+00000d80: 7963 0400 0000 0000 0000 0000 0000 0400  yc..............
+00000d90: 0000 0600 0000 4300 0000 731a 0000 007c  ......C...s....|
+00000da0: 006a 006a 017c 006a 027c 017c 027c 0364  .j.j.|.j.|.|.|.d
+00000db0: 018d 0401 0064 0053 0029 024e 2901 7249  .....d.S.).N).rI
+00000dc0: 0000 0029 0372 0e00 0000 da0d 646f 776e  ...).r......down
+00000dd0: 6c6f 6164 5f66 696c 6572 0f00 0000 2904  load_filer....).
+00000de0: 723f 0000 0072 4700 0000 7248 0000 0072  r?...rG...rH...r
+00000df0: 4900 0000 7218 0000 0072 1800 0000 7219  I...r....r....r.
+00000e00: 0000 00da 0864 6f77 6e6c 6f61 6474 0000  .....downloadt..
+00000e10: 0073 0c00 0000 0606 0401 0201 0201 0201  .s..............
+00000e20: 0afc 7a0d 4669 6c65 2e64 6f77 6e6c 6f61  ..z.File.downloa
+00000e30: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
+00000e40: 0000 0300 0000 4300 0000 730e 0000 007c  ......C...s....|
+00000e50: 006a 00a0 017c 006a 02a1 0153 0072 2300  .j...|.j...S.r#.
+00000e60: 0000 2903 720e 0000 00da 0e67 6574 5f73  ..).r......get_s
+00000e70: 6967 6e65 645f 7572 6c72 0f00 0000 7242  igned_urlr....rB
+00000e80: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00000e90: 0000 724c 0000 0081 0000 0073 0200 0000  ..rL.......s....
+00000ea0: 0e01 7a13 4669 6c65 2e67 6574 5f73 6967  ..z.File.get_sig
+00000eb0: 6e65 645f 7572 6c63 0100 0000 0000 0000  ned_urlc........
+00000ec0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00000ed0: 730a 0000 0074 007c 006a 0183 0153 0072  s....t.|.j...S.r
+00000ee0: 2300 0000 2902 7206 0000 0072 0f00 0000  #...).r....r....
+00000ef0: 7242 0000 0072 1800 0000 7218 0000 0072  rB...r....r....r
+00000f00: 1900 0000 da07 746f 5f64 6963 7484 0000  ......to_dict...
+00000f10: 0073 0200 0000 0a01 7a0c 4669 6c65 2e74  .s......z.File.t
+00000f20: 6f5f 6469 6374 7223 0000 0029 0272 1100  o_dictr#...).r..
+00000f30: 0000 4e29 25da 085f 5f6e 616d 655f 5fda  ..N)%..__name__.
+00000f40: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000f50: 7561 6c6e 616d 655f 5f72 0900 0000 da0f  ualname__r......
+00000f60: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
+00000f70: 0c00 0000 da0c 7374 6174 6963 6d65 7468  ......staticmeth
+00000f80: 6f64 da03 7374 7272 1a00 0000 721e 0000  od..strr....r...
+00000f90: 0072 0300 0000 7220 0000 00da 0b63 6c61  .r....r .....cla
+00000fa0: 7373 6d65 7468 6f64 7227 0000 0072 0500  ssmethodr'...r..
+00000fb0: 0000 da0b 636f 6c6c 6563 7469 6f6e 73da  ....collections.
+00000fc0: 0361 6263 da09 4765 6e65 7261 746f 7272  .abc..Generatorr
+00000fd0: 2800 0000 7240 0000 00da 0870 726f 7065  (...r@.....prope
+00000fe0: 7274 7972 2100 0000 7229 0000 0072 1000  rtyr!...r)...r..
+00000ff0: 0000 7226 0000 0072 4400 0000 7246 0000  ..r&...rD...rF..
+00001000: 0072 0a00 0000 da07 7061 7468 6c69 62da  .r......pathlib.
+00001010: 0450 6174 6872 0800 0000 720b 0000 0072  .Pathr....r....r
+00001020: 4b00 0000 724c 0000 00da 0464 6963 7472  K...rL.....dictr
+00001030: 0200 0000 724d 0000 0072 1800 0000 7218  ....rM...r....r.
+00001040: 0000 0072 1800 0000 7219 0000 0072 0d00  ...r....r....r..
+00001050: 0000 1300 0000 7376 0000 000a 0008 0108  ......sv........
+00001060: 0102 0214 0102 0718 0102 0302 0204 ff02  ................
+00001070: 0102 ff02 0102 ff06 0102 ff02 020c fe02  ................
+00001080: 0802 0102 0202 fe02 0302 fd02 040c fc02  ................
+00001090: 0802 0504 fc02 0202 fe02 0302 fd06 0402  ................
+000010a0: fc0a 050c fb12 2302 0410 0102 0310 0102  ......#.........
+000010b0: 0310 0102 0310 0102 0310 010a 0304 0704  ................
+000010c0: fc04 0202 fe02 0302 fd02 040a fc0e 0d1a  ................
+000010d0: 0372 0d00 0000 2914 da0f 636f 6c6c 6563  .r....)...collec
+000010e0: 7469 6f6e 732e 6162 6372 5500 0000 7214  tions.abcrU...r.
+000010f0: 0000 0072 5900 0000 da06 7479 7069 6e67  ...rY.....typing
+00001100: 7202 0000 0072 0300 0000 7228 0000 0072  r....r....r(...r
+00001110: 0500 0000 da05 7365 7264 6572 0600 0000  ......serder....
+00001120: 7222 0000 0072 0800 0000 7209 0000 00da  r"...r....r.....
+00001130: 0870 726f 6772 6573 7372 0a00 0000 720b  .progressr....r.
+00001140: 0000 0072 2600 0000 720c 0000 0072 0d00  ...r&...r....r..
+00001150: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
+00001160: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001170: 0100 0000 7314 0000 0008 0008 0108 0110  ....s...........
+00001180: 010c 020c 0110 0110 040c 0412 03         .............
```

### Comparing `roboto-0.2.8/src/roboto/domain/files/__pycache__/http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/files/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 500 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 f401 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 f401 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c01 6d02 5a02 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6501 6a03 8303 5a04 4700 6405  ..d.e.j...Z.G.d.
 00000060: 6406 8400 6406 6501 6a03 8303 5a05 4700  d...d.e.j...Z.G.
 00000070: 6407 6408 8400 6408 6501 6a03 8303 5a06  d.d...d.e.j...Z.
@@ -22,15 +22,15 @@
 00000150: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00000160: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
 00000170: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
 00000180: 696f 6e73 5f5f 7206 0000 00da 0674 7970  ions__r......typ
 00000190: 696e 67da 084f 7074 696f 6e61 6ca9 0072  ing..Optional..r
 000001a0: 0f00 0000 720f 0000 00fa eb2f 636f 6465  ....r....../code
 000001b0: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-000001c0: 3130 3531 3138 3230 3839 2f73 7263 2f63  1051182089/src/c
+000001c0: 3330 3739 3233 3632 3634 2f73 7263 2f63  3079236264/src/c
 000001d0: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 000001e0: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 000001f0: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 00000200: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 00000210: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 00000220: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 00000230: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
```

### Comparing `roboto-0.2.8/src/roboto/domain/files/__pycache__/progress.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/files/__pycache__/progress.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 4606 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 fe11 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 fe11 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 5a04 4700  m.Z...d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6500 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 4700 6405 6406 8400 6406 6500 6a05 8303  G.d.d...d.e.j...
 00000070: 5a07 4700 6407 6408 8400 6408 6506 8303  Z.G.d.d...d.e...
@@ -21,16 +21,16 @@
 00000140: 6f72 da05 6465 6c74 6163 0200 0000 0000  or..deltac......
 00000150: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
 00000160: 0000 f308 0000 0074 0064 0183 0182 0129  .......t.d.....)
 00000170: 024e da06 7570 6461 7465 a901 da13 4e6f  .N..update....No
 00000180: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
 00000190: 7229 02da 0473 656c 6672 0500 0000 a900  r)...selfr......
 000001a0: 720b 0000 00fa e52f 636f 6465 6275 696c  r....../codebuil
-000001b0: 642f 6f75 7470 7574 2f73 7263 3130 3531  d/output/src1051
-000001c0: 3138 3230 3839 2f73 7263 2f63 6f64 6573  182089/src/codes
+000001b0: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+000001c0: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
 000001d0: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 000001e0: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 000001f0: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 00000200: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 00000210: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 00000220: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 00000230: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto-0.2.8/src/roboto/domain/files/__pycache__/record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/files/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 921 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 9903 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 9903 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000050: 6503 6a04 8303 5a05 6401 5300 2904 e900  e.j...Z.d.S.)...
 00000060: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
 00000070: 0000 0000 0004 0000 0040 0000 0073 9000  .........@...s..
@@ -28,16 +28,16 @@
 000001b0: 0000 0073 1400 0000 7400 6a01 a002 7c00  ...s....t.j...|.
 000001c0: 6a03 a101 7d01 7c01 6a04 5300 2901 4e29  j...}.|.j.S.).N)
 000001d0: 05da 0675 726c 6c69 62da 0570 6172 7365  ...urllib..parse
 000001e0: da08 7572 6c70 6172 7365 7208 0000 00da  ..urlparser.....
 000001f0: 066e 6574 6c6f 63a9 02da 0473 656c 665a  .netloc....selfZ
 00000200: 0a70 6172 7365 645f 7572 69a9 0072 1400  .parsed_uri..r..
 00000210: 0000 fae3 2f63 6f64 6562 7569 6c64 2f6f  ..../codebuild/o
-00000220: 7574 7075 742f 7372 6331 3035 3131 3832  utput/src1051182
-00000230: 3038 392f 7372 632f 636f 6465 7374 6172  089/src/codestar
+00000220: 7574 7075 742f 7372 6333 3037 3932 3336  utput/src3079236
+00000230: 3236 342f 7372 632f 636f 6465 7374 6172  264/src/codestar
 00000240: 2d63 6f6e 6e65 6374 696f 6e73 2e75 732d  -connections.us-
 00000250: 7765 7374 2d32 2e61 6d61 7a6f 6e61 7773  west-2.amazonaws
 00000260: 2e63 6f6d 2f67 6974 2d68 7474 702f 3036  .com/git-http/06
 00000270: 3631 3935 3131 3233 3835 2f75 732d 7765  6195112385/us-we
 00000280: 7374 2d32 2f65 3635 3032 6138 302d 6262  st-2/e6502a80-bb
 00000290: 3465 2d34 6662 652d 3837 3263 2d35 6434  4e-4fbe-872c-5d4
 000002a0: 3263 3139 3336 3939 642f 726f 626f 746f  2c193699d/roboto
```

### Comparing `roboto-0.2.8/src/roboto/domain/files/client_delegate.py` & `roboto-0.2.9/src/roboto/domain/files/client_delegate.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,14 @@
     ) -> FileRecord:
         url = f"{self.__roboto_service_base_url}/v1/files/record/{file_id}"
 
         with RobotoHttpExceptionParse():
             res = self.__http_client.get(
                 url,
                 headers=roboto_headers(
-                    org_id=org_id,
                     additional_headers={"Content-Type": "application/json"},
                 ),
             )
         return FileRecord.model_validate(res.from_json(json_path=["data"]))
 
     def get_signed_url(self, record: FileRecord) -> str:
         url = f"{self.__roboto_service_base_url}/v1/files/{record.file_id}/signed-url"
```

### Comparing `roboto-0.2.8/src/roboto/domain/files/delegate.py` & `roboto-0.2.9/src/roboto/domain/files/delegate.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,17 +69,15 @@
         credential_provider: CredentialProvider,
         progress_monitor_factory: ProgressMonitorFactory = NoopProgressMonitorFactory(),
         max_concurrency: int = 20,
     ) -> None:
         raise NotImplementedError("download_files")
 
     @abc.abstractmethod
-    def get_record_by_primary_key(
-        self, file_id: str, org_id: Optional[str] = None
-    ) -> FileRecord:
+    def get_record_by_primary_key(self, file_id: str) -> FileRecord:
         raise NotImplementedError("get_record_by_primary_key")
 
     @abc.abstractmethod
     def get_signed_url(self, record: FileRecord) -> str:
         raise NotImplementedError("get_signed_url")
 
     @abc.abstractmethod
```

### Comparing `roboto-0.2.8/src/roboto/domain/files/file.py` & `roboto-0.2.9/src/roboto/domain/files/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,16 @@
         return base_uri
 
     @classmethod
     def from_id(
         cls,
         file_id: str,
         delegate: FileDelegate,
-        org_id: Optional[str] = None,
     ) -> "File":
-        record = delegate.get_record_by_primary_key(file_id, org_id)
+        record = delegate.get_record_by_primary_key(file_id)
         return cls(record, delegate)
 
     @classmethod
     def query(
         cls,
         query: QuerySpecification,
         delegate: FileDelegate,
```

### Comparing `roboto-0.2.8/src/roboto/domain/files/progress.py` & `roboto-0.2.9/src/roboto/domain/files/progress.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/files/record.py` & `roboto-0.2.9/src/roboto/domain/files/record.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/http_delegates.py` & `roboto-0.2.9/src/roboto/domain/http_delegates.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/__init__.py` & `roboto-0.2.9/src/roboto/domain/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/orgs/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 902 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 8603 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 8603 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
@@ -41,16 +41,16 @@
 00000280: 6772 0a00 0000 5a0a 6f72 675f 696e 7669  gr....Z.org_invi
 00000290: 7465 720b 0000 005a 086f 7267 5f72 6f6c  ter....Z.org_rol
 000002a0: 6572 0c00 0000 da06 7265 636f 7264 720d  er......recordr.
 000002b0: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
 000002c0: 0000 7211 0000 0072 1200 0000 da07 5f5f  ..r....r......__
 000002d0: 616c 6c5f 5fa9 0072 1900 0000 7219 0000  all__..r....r...
 000002e0: 00fa e42f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-000002f0: 7470 7574 2f73 7263 3130 3531 3138 3230  tput/src10511820
-00000300: 3839 2f73 7263 2f63 6f64 6573 7461 722d  89/src/codestar-
+000002f0: 7470 7574 2f73 7263 3330 3739 3233 3632  tput/src30792362
+00000300: 3634 2f73 7263 2f63 6f64 6573 7461 722d  64/src/codestar-
 00000310: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 00000320: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 00000330: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 00000340: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 00000350: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 00000360: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000370: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/__pycache__/delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/orgs/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3589 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 050e 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 050e 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 4700  m.Z.m.Z.m.Z...G.
 00000060: 6405 6406 8400 6406 6500 6a09 8303 5a0a  d.d...d.e.j...Z.
 00000070: 6401 5300 2907 e900 0000 004e 2902 da03  d.S.)......N)...
@@ -61,16 +61,16 @@
 000003c0: 0000 0000 0004 0000 0002 0000 0043 0000  .............C..
 000003d0: 00f3 0800 0000 7400 6401 8301 8201 2902  ......t.d.....).
 000003e0: 4eda 0a63 7265 6174 655f 6f72 67a9 01da  N..create_org...
 000003f0: 134e 6f74 496d 706c 656d 656e 7465 6445  .NotImplementedE
 00000400: 7272 6f72 2904 da04 7365 6c66 720a 0000  rror)...selfr...
 00000410: 0072 0b00 0000 720c 0000 00a9 0072 1300  .r....r......r..
 00000420: 0000 fae4 2f63 6f64 6562 7569 6c64 2f6f  ..../codebuild/o
-00000430: 7574 7075 742f 7372 6331 3035 3131 3832  utput/src1051182
-00000440: 3038 392f 7372 632f 636f 6465 7374 6172  089/src/codestar
+00000430: 7574 7075 742f 7372 6333 3037 3932 3336  utput/src3079236
+00000440: 3236 342f 7372 632f 636f 6465 7374 6172  264/src/codestar
 00000450: 2d63 6f6e 6e65 6374 696f 6e73 2e75 732d  -connections.us-
 00000460: 7765 7374 2d32 2e61 6d61 7a6f 6e61 7773  west-2.amazonaws
 00000470: 2e63 6f6d 2f67 6974 2d68 7474 702f 3036  .com/git-http/06
 00000480: 3631 3935 3131 3233 3835 2f75 732d 7765  6195112385/us-we
 00000490: 7374 2d32 2f65 3635 3032 6138 302d 6262  st-2/e6502a80-bb
 000004a0: 3465 2d34 6662 652d 3837 3263 2d35 6434  4e-4fbe-872c-5d4
 000004b0: 3263 3139 3336 3939 642f 726f 626f 746f  2c193699d/roboto
```

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/__pycache__/http_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/orgs/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 8997 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 2523 0000  o........Y.e%#..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 2523 0000  o.......2H.e%#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6402 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6402 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6406 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6406 6408 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
@@ -77,15 +77,15 @@
 000004c0: 0200 0000 0200 0000 0300 0000 7314 0000  ............s...
 000004d0: 0074 0083 00a0 01a1 0001 007c 017c 005f  .t.........|.|._
 000004e0: 0264 0053 00a9 014e 2903 da05 7375 7065  .d.S...N)...supe
 000004f0: 72da 085f 5f69 6e69 745f 5f72 1700 0000  r..__init__r....
 00000500: 2902 da04 7365 6c66 7218 0000 00a9 01da  )...selfr.......
 00000510: 095f 5f63 6c61 7373 5f5f a900 fae9 2f63  .__class__..../c
 00000520: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000530: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+00000530: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 00000540: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 00000550: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 00000560: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 00000570: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 00000580: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 00000590: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 000005a0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/__pycache__/http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/orgs/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 740 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 e402 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 e402 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 0100 4700  d.l.m.Z.m.Z...G.
 00000050: 6404 6405 8400 6405 6501 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 4700 6406 6407 8400 6407 6501 6a05 8303  G.d.d...d.e.j...
 00000070: 5a07 4700 6408 6409 8400 6409 6501 6a05  Z.G.d.d...d.e.j.
@@ -23,15 +23,15 @@
 00000160: 6f6d 6169 6e4e 2907 da08 5f5f 6e61 6d65  omainN)...__name
 00000170: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
 00000180: 5f5f 7175 616c 6e61 6d65 5f5f da03 7374  __qualname__..st
 00000190: 72da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  r..__annotations
 000001a0: 5f5f 7207 0000 00da 0462 6f6f 6ca9 0072  __r......bool..r
 000001b0: 0e00 0000 720e 0000 00fa ea2f 636f 6465  ....r....../code
 000001c0: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-000001d0: 3130 3531 3138 3230 3839 2f73 7263 2f63  1051182089/src/c
+000001d0: 3330 3739 3233 3632 3634 2f73 7263 2f63  3079236264/src/c
 000001e0: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 000001f0: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 00000200: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 00000210: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 00000220: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 00000230: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 00000240: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
```

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/__pycache__/org.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/orgs/__pycache__/org.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 4075 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 eb0f 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 eb0f 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
 00000070: 8400 6408 8302 5a0b 6409 5300 290a e900  ..d...Z.d.S.)...
@@ -51,15 +51,15 @@
 00000320: 0029 034e 2903 7211 0000 0072 0e00 0000  .).N).r....r....
 00000330: 7210 0000 00a9 02da 0672 6563 6f72 6472  r........recordr
 00000340: 0f00 0000 2901 da0a 6372 6561 7465 5f6f  ....)...create_o
 00000350: 7267 2906 da03 636c 7372 0e00 0000 720f  rg)...clsr....r.
 00000360: 0000 0072 1000 0000 7211 0000 0072 1300  ...r....r....r..
 00000370: 0000 a900 7216 0000 00fa df2f 636f 6465  ....r....../code
 00000380: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000390: 3130 3531 3138 3230 3839 2f73 7263 2f63  1051182089/src/c
+00000390: 3330 3739 3233 3632 3634 2f73 7263 2f63  3079236264/src/c
 000003a0: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 000003b0: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 000003c0: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 000003d0: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 000003e0: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 000003f0: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 00000400: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
```

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/__pycache__/org_invite.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/orgs/__pycache__/org_invite.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2413 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 6d09 0000  o........Y.em...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 6d09 0000  o.......2H.em...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6407 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6408 6409 8400 6409 8302 5a0b 640a 5300  d.d...d...Z.d.S.
@@ -50,15 +50,15 @@
 00000310: 0000 0072 1100 0000 720f 0000 00a9 02da  ...r....r.......
 00000320: 0672 6563 6f72 6472 1000 0000 2901 da12  .recordr....)...
 00000330: 696e 7669 7465 5f75 7365 725f 746f 5f6f  invite_user_to_o
 00000340: 7267 2906 da03 636c 7372 0e00 0000 720f  rg)...clsr....r.
 00000350: 0000 0072 1000 0000 7211 0000 0072 1400  ...r....r....r..
 00000360: 0000 a900 7217 0000 00fa e62f 636f 6465  ....r....../code
 00000370: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000380: 3130 3531 3138 3230 3839 2f73 7263 2f63  1051182089/src/c
+00000380: 3330 3739 3233 3632 3634 2f73 7263 2f63  3079236264/src/c
 00000390: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 000003a0: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 000003b0: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 000003c0: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 000003d0: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 000003e0: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 000003f0: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
```

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/__pycache__/org_role.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/orgs/__pycache__/org_role.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1921 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 8107 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 8107 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6407 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 4700 6408 6409 8400 6409 8302 5a0c  ..G.d.d...d...Z.
@@ -47,15 +47,15 @@
 000002e0: 0000 0200 0000 0600 0000 1300 0000 f318  ................
 000002f0: 0000 0067 007c 005d 087d 0188 007c 0188  ...g.|.].}...|..
 00000300: 0164 008d 0291 0271 0253 00a9 01a9 02da  .d.....q.S......
 00000310: 0672 6563 6f72 6472 1000 0000 a900 a902  .recordr........
 00000320: da02 2e30 7216 0000 00a9 02da 0363 6c73  ...0r........cls
 00000330: 7210 0000 0072 1700 0000 fae4 2f63 6f64  r....r....../cod
 00000340: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000350: 6331 3035 3131 3832 3038 392f 7372 632f  c1051182089/src/
+00000350: 6333 3037 3932 3336 3236 342f 7372 632f  c3079236264/src/
 00000360: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000370: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000380: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000390: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 000003a0: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 000003b0: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 000003c0: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/__pycache__/record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/orgs/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 775 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 0703 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 0703 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 6504 6500 6a05 8304 5a06 4700  ..d.e.e.j...Z.G.
 00000060: 6406 6407 8400 6407 6504 6500 6a05 8304  d.d...d.e.e.j...
 00000070: 5a07 4700 6408 6409 8400 6409 6501 6a08  Z.G.d.d...d.e.j.
@@ -21,15 +21,15 @@
 00000140: 6f6e 696e 674e 2906 da08 5f5f 6e61 6d65  oningN)...__name
 00000150: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
 00000160: 5f5f 7175 616c 6e61 6d65 5f5f 5a0c 5072  __qualname__Z.Pr
 00000170: 6f76 6973 696f 6e69 6e67 5a06 4163 7469  ovisioningZ.Acti
 00000180: 7665 5a0e 4465 7072 6f76 6973 696f 6e69  veZ.Deprovisioni
 00000190: 6e67 a900 720a 0000 0072 0a00 0000 fae2  ng..r....r......
 000001a0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000001b0: 742f 7372 6331 3035 3131 3832 3038 392f  t/src1051182089/
+000001b0: 742f 7372 6333 3037 3932 3336 3236 342f  t/src3079236264/
 000001c0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 000001d0: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 000001e0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 000001f0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000200: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000210: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000220: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/delegate.py` & `roboto-0.2.9/src/roboto/domain/orgs/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/http_delegate.py` & `roboto-0.2.9/src/roboto/domain/orgs/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/http_resources.py` & `roboto-0.2.9/src/roboto/domain/orgs/http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/org.py` & `roboto-0.2.9/src/roboto/domain/orgs/org.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/org_invite.py` & `roboto-0.2.9/src/roboto/domain/orgs/org_invite.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/org_role.py` & `roboto-0.2.9/src/roboto/domain/orgs/org_role.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/orgs/record.py` & `roboto-0.2.9/src/roboto/domain/orgs/record.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/tokens/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/tokens/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 c401 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 c401 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6700 6406 a201 5a0c 6407 5300 2908  ..g.d...Z.d.S.).
@@ -20,16 +20,16 @@
 00000130: 7202 0000 00da 0d68 7474 705f 6465 6c65  r......http_dele
 00000140: 6761 7465 7203 0000 00da 0e68 7474 705f  gater......http_
 00000150: 7265 736f 7572 6365 7372 0400 0000 7205  resourcesr....r.
 00000160: 0000 00da 0672 6563 6f72 6472 0600 0000  .....recordr....
 00000170: 7207 0000 00da 0574 6f6b 656e 7208 0000  r......tokenr...
 00000180: 00da 075f 5f61 6c6c 5f5f a900 720f 0000  ...__all__..r...
 00000190: 0072 0f00 0000 fae6 2f63 6f64 6562 7569  .r....../codebui
-000001a0: 6c64 2f6f 7574 7075 742f 7372 6331 3035  ld/output/src105
-000001b0: 3131 3832 3038 392f 7372 632f 636f 6465  1182089/src/code
+000001a0: 6c64 2f6f 7574 7075 742f 7372 6333 3037  ld/output/src307
+000001b0: 3932 3336 3236 342f 7372 632f 636f 6465  9236264/src/code
 000001c0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 000001d0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 000001e0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 000001f0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000200: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000210: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000220: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto-0.2.8/src/roboto/domain/tokens/__pycache__/delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/tokens/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 857 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 5903 0000  o........Y.eY...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 5903 0000  o.......2H.eY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 6500 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6401 5300 2907 e900 0000 004e 2901 da08  d.S.)......N)...
 00000070: 4f70 7469 6f6e 616c e901 0000 0029 01da  Optional.....)..
@@ -23,16 +23,16 @@
 00000160: 0000 0000 0000 0000 0000 0200 0000 0200  ................
 00000170: 0000 4300 0000 f308 0000 0074 0064 0183  ..C........t.d..
 00000180: 0182 0129 024e da13 6765 745f 746f 6b65  ...).N..get_toke
 00000190: 6e73 5f66 6f72 5f75 7365 72a9 01da 134e  ns_for_user....N
 000001a0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
 000001b0: 6f72 2902 da04 7365 6c66 7206 0000 00a9  or)...selfr.....
 000001c0: 0072 0d00 0000 fae6 2f63 6f64 6562 7569  .r....../codebui
-000001d0: 6c64 2f6f 7574 7075 742f 7372 6331 3035  ld/output/src105
-000001e0: 3131 3832 3038 392f 7372 632f 636f 6465  1182089/src/code
+000001d0: 6c64 2f6f 7574 7075 742f 7372 6333 3037  ld/output/src307
+000001e0: 3932 3336 3236 342f 7372 632f 636f 6465  9236264/src/code
 000001f0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000200: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000210: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000220: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000230: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000240: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000250: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto-0.2.8/src/roboto/domain/tokens/__pycache__/http_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/tokens/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2226 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 b208 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 b208 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6402 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6406 6407 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6408 6c0b 6d0c 5a0c 0100 6406 6409 6c0d  d.l.m.Z...d.d.l.
@@ -37,16 +37,16 @@
 00000240: 0000 0000 0000 0002 0000 0002 0000 0003  ................
 00000250: 0000 0073 1400 0000 7400 8300 a001 a100  ...s....t.......
 00000260: 0100 7c01 7c00 5f02 6400 5300 a901 4e29  ..|.|._.d.S...N)
 00000270: 03da 0573 7570 6572 da08 5f5f 696e 6974  ...super..__init
 00000280: 5f5f 720d 0000 0029 02da 0473 656c 6672  __r....)...selfr
 00000290: 0e00 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
 000002a0: 5fa9 00fa eb2f 636f 6465 6275 696c 642f  _..../codebuild/
-000002b0: 6f75 7470 7574 2f73 7263 3130 3531 3138  output/src105118
-000002c0: 3230 3839 2f73 7263 2f63 6f64 6573 7461  2089/src/codesta
+000002b0: 6f75 7470 7574 2f73 7263 3330 3739 3233  output/src307923
+000002c0: 3632 3634 2f73 7263 2f63 6f64 6573 7461  6264/src/codesta
 000002d0: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 000002e0: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 000002f0: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 00000300: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 00000310: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 00000320: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 00000330: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto-0.2.8/src/roboto/domain/tokens/__pycache__/http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/tokens/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 283 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 1b01 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 1b01 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 4700 6403 6404 8400 6404 6502 6a03  Z.G.d.d...d.e.j.
 00000050: 8303 5a04 4700 6405 6406 8400 6406 6502  ..Z.G.d.d...d.e.
 00000060: 6a03 8303 5a05 6402 5300 2907 e900 0000  j...Z.d.S.).....
 00000070: 0029 01da 084f 7074 696f 6e61 6c4e 6300  .)...OptionalNc.
@@ -16,16 +16,16 @@
 000000f0: 616d 654e da0b 6465 7363 7269 7074 696f  ameN..descriptio
 00000100: 6e29 08da 085f 5f6e 616d 655f 5fda 0a5f  n)...__name__.._
 00000110: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00000120: 6c6e 616d 655f 5fda 0369 6e74 da0f 5f5f  lname__..int..__
 00000130: 616e 6e6f 7461 7469 6f6e 735f 5fda 0373  annotations__..s
 00000140: 7472 7206 0000 0072 0200 0000 a900 720d  trr....r......r.
 00000150: 0000 0072 0d00 0000 faec 2f63 6f64 6562  ...r....../codeb
-00000160: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-00000170: 3035 3131 3832 3038 392f 7372 632f 636f  051182089/src/co
+00000160: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+00000170: 3037 3932 3336 3236 342f 7372 632f 636f  079236264/src/co
 00000180: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 00000190: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 000001a0: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 000001b0: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 000001c0: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 000001d0: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 000001e0: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto-0.2.8/src/roboto/domain/tokens/__pycache__/record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/tokens/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 455 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 c701 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 c701 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000050: 8400 6404 6503 6a04 8303 5a05 4700 6405  ..d.e.j...Z.G.d.
 00000060: 6406 8400 6406 6503 6a04 8303 5a06 6401  d...d.e.j...Z.d.
 00000070: 5300 2907 e900 0000 004e 2901 da08 4f70  S.)......N)...Op
@@ -20,16 +20,16 @@
 00000130: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 00000140: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000150: 6e61 6d65 5f5f da03 7374 72da 0f5f 5f61  name__..str..__a
 00000160: 6e6e 6f74 6174 696f 6e73 5f5f 7206 0000  nnotations__r...
 00000170: 0072 0200 0000 da08 6461 7465 7469 6d65  .r......datetime
 00000180: 7208 0000 00a9 0072 0f00 0000 720f 0000  r......r....r...
 00000190: 00fa e42f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-000001a0: 7470 7574 2f73 7263 3130 3531 3138 3230  tput/src10511820
-000001b0: 3839 2f73 7263 2f63 6f64 6573 7461 722d  89/src/codestar-
+000001a0: 7470 7574 2f73 7263 3330 3739 3233 3632  tput/src30792362
+000001b0: 3634 2f73 7263 2f63 6f64 6573 7461 722d  64/src/codestar-
 000001c0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000001d0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000001e0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 000001f0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 00000200: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 00000210: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000220: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto-0.2.8/src/roboto/domain/tokens/__pycache__/token.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/tokens/__pycache__/token.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2128 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 5008 0000  o........Y.eP...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 5008 0000  o.......2H.eP...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6407 6408 8400 6408 8302 5a09  ..G.d.d...d...Z.
 00000070: 6409 5300 290a e900 0000 0029 02da 0341  d.S.)......)...A
@@ -41,15 +41,15 @@
 00000280: 017d 037c 007c 037c 0264 028d 0253 0029  .}.|.|.|.d...S.)
 00000290: 034e a901 720c 0000 00a9 02da 0672 6563  .N..r........rec
 000002a0: 6f72 6472 0d00 0000 2901 da15 6765 745f  ordr....)...get_
 000002b0: 746f 6b65 6e5f 6279 5f74 6f6b 656e 5f69  token_by_token_i
 000002c0: 6429 04da 0363 6c73 720c 0000 0072 0d00  d)...clsr....r..
 000002d0: 0000 7211 0000 00a9 0072 1400 0000 fae3  ..r......r......
 000002e0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000002f0: 742f 7372 6331 3035 3131 3832 3038 392f  t/src1051182089/
+000002f0: 742f 7372 6333 3037 3932 3336 3236 342f  t/src3079236264/
 00000300: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000310: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000320: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000330: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000340: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000350: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000360: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto-0.2.8/src/roboto/domain/tokens/delegate.py` & `roboto-0.2.9/src/roboto/domain/tokens/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/tokens/http_delegate.py` & `roboto-0.2.9/src/roboto/domain/tokens/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/tokens/token.py` & `roboto-0.2.9/src/roboto/domain/tokens/token.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/topics/__init__.py` & `roboto-0.2.9/src/roboto/domain/topics/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .topic import Topic
 from .topic_delegate import TopicDelegate
 from .topic_http_delegate import TopicHttpDelegate
 from .topic_record import (
+    CanonicalDataType,
     MessagePathRecord,
     RepresentationContext,
     RepresentationRecord,
     RepresentationStorageFormat,
     TimeseriesPlotContext,
     TopicRecord,
 )
@@ -14,22 +15,23 @@
     AddMessagePathRequest,
     CreateTopicRequest,
     SetDefaultRepresentationRequest,
     UpdateTopicRequest,
 )
 
 __all__ = (
-    "SetDefaultRepresentationRequest",
     "AddMessagePathRequest",
     "AddMessagePathRepresentationRequest",
     "CreateTopicRequest",
+    "CanonicalDataType",
     "MessagePathRecord",
     "RepresentationContext",
     "RepresentationRecord",
     "RepresentationStorageFormat",
+    "SetDefaultRepresentationRequest",
     "TimeseriesPlotContext",
     "Topic",
     "TopicDelegate",
     "TopicHttpDelegate",
     "TopicRecord",
     "UpdateTopicRequest",
 )
```

### Comparing `roboto-0.2.8/src/roboto/domain/topics/topic.py` & `roboto-0.2.9/src/roboto/domain/topics/topic.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,14 +18,34 @@
 
 
 class Topic:
     __record: TopicRecord
     __topic_delegate: TopicDelegate
 
     @classmethod
+    def get_by_association(
+        cls,
+        association: Association,
+        topic_delegate: TopicDelegate,
+        org_id: typing.Optional[str] = None,
+    ) -> collections.abc.Generator["Topic", None, None]:
+        paginated_results = topic_delegate.get_topics_by_association(
+            association, org_id
+        )
+        while True:
+            for topic_record in paginated_results.items:
+                yield cls(topic_record, topic_delegate)
+            if paginated_results.next_token:
+                paginated_results = topic_delegate.get_topics_by_association(
+                    association, org_id, paginated_results.next_token
+                )
+            else:
+                break
+
+    @classmethod
     def create(
         cls,
         request: CreateTopicRequest,
         topic_delegate: TopicDelegate,
     ) -> "Topic":
         topic_record = topic_delegate.create_topic(request)
         return cls(topic_record, topic_delegate)
```

### Comparing `roboto-0.2.8/src/roboto/domain/topics/topic_delegate.py` & `roboto-0.2.9/src/roboto/domain/topics/topic_delegate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import abc
 import collections.abc
 import typing
 
 from ...association import Association
+from ...http import PaginatedList
 from .topic_record import (
     MessagePathRecord,
     RepresentationRecord,
     TopicRecord,
 )
 from .topic_requests import (
     AddMessagePathRepresentationRequest,
@@ -46,14 +47,23 @@
         topic_name: str,
         association: Association,
         org_id: typing.Optional[str] = None,
     ) -> TopicRecord:
         raise NotImplementedError("get_topic_by_name_and_association")
 
     @abc.abstractmethod
+    def get_topics_by_association(
+        self,
+        association: Association,
+        org_id: typing.Optional[str] = None,
+        page_token: typing.Optional[str] = None,
+    ) -> PaginatedList[TopicRecord]:
+        raise NotImplementedError("get_topics_by_association")
+
+    @abc.abstractmethod
     def hard_delete_topic(
         self,
         topic_record: TopicRecord,
     ) -> None:
         raise NotImplementedError("hard_delete_topic")
 
     @abc.abstractmethod
```

### Comparing `roboto-0.2.8/src/roboto/domain/topics/topic_record.py` & `roboto-0.2.9/src/roboto/domain/topics/topic_record.py`

 * *Files 21% similar despite different names*

```diff
@@ -72,29 +72,67 @@
     """Internal identifier for this Representation."""
 
     storage_format: RepresentationStorageFormat
     topic_id: int
     version: int
 
 
+class CanonicalDataType(enum.Enum):
+    """
+    Well-known (and simplified) data types, normalized across frameworks/technologies.
+    Primarily used for UI purposes to determine if a Panel can render a particular MessagePath.
+
+    References:
+        - ROS1 field types: http://wiki.ros.org/msg
+        - ROS2 field types: https://docs.ros.org/en/iron/Concepts/Basic/About-Interfaces.html#field-types
+        - uORB: there is no canonical list of primitive field types, but they appear to be the same as ROS.
+            The documentation states:
+            > Have a look at the existing msg files for supported types.
+            > A message can also be used nested in other messages.
+            From https://docs.px4.io/main/en/middleware/uorb.html#adding-a-new-topic
+
+    Example mappings:
+    - "float32" -> DataType.Number
+    - "uint8[]" -> DataType.Array
+    - "geometry_msgs/Pose" -> DataType.Object
+    - "std_msgs/Header" -> DataType.Object
+    - "string" -> DataType.String
+    - "char" -> DataType.String
+    - "bool" -> DataType.Boolean
+    - "byte" -> DataType.Byte
+
+    """
+
+    Array = "array"  # A sequence of values.
+    Boolean = "boolean"
+    Byte = "byte"
+    Number = "number"
+    Object = "object"  # A struct with attributes.
+    String = "string"
+    Unknown = "unknown"  # This is a fallback and should be used sparingly.
+
+
 class MessagePathRecord(pydantic.BaseModel):
     """
     Path to a typed attribute within individual datum records contained within a Topic.
     """
 
     message_path: str
     """
     Dot-delimited path to the attribute within the datum record.
     """
 
     data_type: str
     """
-    'Native' data type of the attribute at this path. E.g. "float32", "unint8[]", "geometry_msgs/Pose", "string".
+    'Native'/framework-specific data type of the attribute at this path.
+    E.g. "float32", "unint8[]", "geometry_msgs/Pose", "string".
     """
 
+    canonical_data_type: CanonicalDataType
+
     representations: list[RepresentationRecord] = pydantic.Field(default_factory=list)
     """
     Zero to many Representations of this MessagePath.
     """
 
     topic_message_path_id: int
     """Internal identifier for this MessagePath, joined to a particular Topic."""
```

### Comparing `roboto-0.2.8/src/roboto/domain/topics/topic_requests.py` & `roboto-0.2.9/src/roboto/domain/topics/topic_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pydantic
 
 from ...association import Association
 from ...sentinels import NotSet, NotSetType
 from ...updates import MetadataChangeset
 from .topic_record import (
+    CanonicalDataType,
     RepresentationContext,
     RepresentationStorageFormat,
 )
 
 
 class BaseAddRepresentationRequest(pydantic.BaseModel):
     association: Association
@@ -35,14 +36,15 @@
 
 
 class AddMessagePathRequest(pydantic.BaseModel):
     """Associate a MessagePath with a Topic."""
 
     message_path: str
     data_type: str
+    canonical_data_type: CanonicalDataType
 
     model_config = pydantic.ConfigDict(extra="forbid")
 
 
 class CreateTopicRequest(pydantic.BaseModel):
     """Memorialize a topic contained within a source recording file."""
```

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/__init__.py` & `roboto-0.2.9/src/roboto/domain/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/triggers/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 761 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 f902 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 f902 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
@@ -32,16 +32,16 @@
 000001f0: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
 00000200: 0000 00da 0774 7269 6767 6572 7209 0000  .....triggerr...
 00000210: 005a 1074 7269 6767 6572 5f64 656c 6567  .Z.trigger_deleg
 00000220: 6174 6572 0a00 0000 5a0e 7472 6967 6765  ater....Z.trigge
 00000230: 725f 7265 636f 7264 720b 0000 0072 0c00  r_recordr....r..
 00000240: 0000 da07 5f5f 616c 6c5f 5fa9 0072 1100  ....__all__..r..
 00000250: 0000 7211 0000 00fa e82f 636f 6465 6275  ..r....../codebu
-00000260: 696c 642f 6f75 7470 7574 2f73 7263 3130  ild/output/src10
-00000270: 3531 3138 3230 3839 2f73 7263 2f63 6f64  51182089/src/cod
+00000260: 696c 642f 6f75 7470 7574 2f73 7263 3330  ild/output/src30
+00000270: 3739 3233 3632 3634 2f73 7263 2f63 6f64  79236264/src/cod
 00000280: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 00000290: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 000002a0: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 000002b0: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 000002c0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 000002d0: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 000002e0: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/__pycache__/http_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/triggers/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 6389 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 f518 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 f518 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6403 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6403 6405 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
 00000070: 6d0d 5a0d 0100 6403 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
@@ -76,15 +76,15 @@
 000004b0: 0000 0002 0000 0003 0000 0073 1400 0000  ...........s....
 000004c0: 7400 8300 a001 a100 0100 7c01 7c00 5f02  t.........|.|._.
 000004d0: 6400 5300 a901 4e29 03da 0573 7570 6572  d.S...N)...super
 000004e0: da08 5f5f 696e 6974 5f5f 721a 0000 0029  ..__init__r....)
 000004f0: 02da 0473 656c 6672 1b00 0000 a901 da09  ...selfr........
 00000500: 5f5f 636c 6173 735f 5fa9 00fa ed2f 636f  __class__..../co
 00000510: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-00000520: 7263 3130 3531 3138 3230 3839 2f73 7263  rc1051182089/src
+00000520: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
 00000530: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
 00000540: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
 00000550: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
 00000560: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
 00000570: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
 00000580: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
 00000590: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
```

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/__pycache__/http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/triggers/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 4073 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 e90f 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 e90f 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c01 6d02 5a02 6d03 5a03 6d04 5a04  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6401 6c05 5a05 6400 6403 6c05  ..d.d.l.Z.d.d.l.
 00000060: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
@@ -67,15 +67,15 @@
 00000420: 616d 6574 6572 5f76 616c 7565 73da 0576  ameter_values..v
 00000430: 616c 7565 da06 7265 7475 726e 6302 0000  alue..returnc...
 00000440: 0000 0000 0000 0000 0002 0000 0002 0000  ................
 00000450: 0043 0000 0073 0800 0000 7400 7c01 8301  .C...s....t.|...
 00000460: 5300 a901 4e72 0a00 0000 a902 da03 636c  S...Nr........cl
 00000470: 7372 2100 0000 a900 7226 0000 00fa ee2f  sr!.....r&...../
 00000480: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000490: 2f73 7263 3130 3531 3138 3230 3839 2f73  /src1051182089/s
+00000490: 2f73 7263 3330 3739 3233 3632 3634 2f73  /src3079236264/s
 000004a0: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 000004b0: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 000004c0: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 000004d0: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 000004e0: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 000004f0: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000500: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/__pycache__/trigger.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/triggers/__pycache__/trigger.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 10159 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 af27 0000  o........Y.e.'..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 af27 0000  o.......2H.e.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6403 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a07 6d08 5a08 0100 6404 6405 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
@@ -258,15 +258,15 @@
 00001010: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
 00001020: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
 00001030: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
 00001040: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
 00001050: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
 00001060: 722e 0000 00a9 0072 3100 0000 fae7 2f63  r......r1...../c
 00001070: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00001080: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+00001080: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 00001090: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 000010a0: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 000010b0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 000010c0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 000010d0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 000010e0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 000010f0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2837 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 150b 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 150b 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6404 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6407 6408 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -76,16 +76,16 @@
 000004b0: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
 000004c0: 4572 726f 7229 0eda 0473 656c 6672 1200  Error)...selfr..
 000004d0: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
 000004e0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
 000004f0: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
 00000500: 1c00 0000 721d 0000 0072 1e00 0000 a900  ....r....r......
 00000510: 7225 0000 00fa f02f 636f 6465 6275 696c  r%...../codebuil
-00000520: 642f 6f75 7470 7574 2f73 7263 3130 3531  d/output/src1051
-00000530: 3138 3230 3839 2f73 7263 2f63 6f64 6573  182089/src/codes
+00000520: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+00000530: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
 00000540: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 00000550: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 00000560: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 00000570: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 00000580: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 00000590: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 000005a0: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/__pycache__/trigger_record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/triggers/__pycache__/trigger_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1667 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 8306 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 8306 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c03 6d04 5a04 0100 6402 6404 6c05  d.l.m.Z...d.d.l.
 00000060: 6d06 5a06 0100 6405 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000070: 6d09 5a09 6d0a 5a0a 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
@@ -24,16 +24,16 @@
 00000170: 6976 65da 0764 6174 6173 6574 5a0c 6461  ive..datasetZ.da
 00000180: 7461 7365 745f 6669 6c65 4e29 05da 085f  taset_fileN)..._
 00000190: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 000001a0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 000001b0: 5fda 0744 6174 6173 6574 5a0b 4461 7461  _..DatasetZ.Data
 000001c0: 7365 7446 696c 65a9 0072 1000 0000 7210  setFile..r....r.
 000001d0: 0000 00fa ee2f 636f 6465 6275 696c 642f  ...../codebuild/
-000001e0: 6f75 7470 7574 2f73 7263 3130 3531 3138  output/src105118
-000001f0: 3230 3839 2f73 7263 2f63 6f64 6573 7461  2089/src/codesta
+000001e0: 6f75 7470 7574 2f73 7263 3330 3739 3233  output/src307923
+000001f0: 3632 3634 2f73 7263 2f63 6f64 6573 7461  6264/src/codesta
 00000200: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 00000210: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 00000220: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 00000230: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 00000240: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 00000250: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 00000260: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/http_delegate.py` & `roboto-0.2.9/src/roboto/domain/triggers/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/http_resources.py` & `roboto-0.2.9/src/roboto/domain/triggers/http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/trigger.py` & `roboto-0.2.9/src/roboto/domain/triggers/trigger.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/trigger_delegate.py` & `roboto-0.2.9/src/roboto/domain/triggers/trigger_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/triggers/trigger_record.py` & `roboto-0.2.9/src/roboto/domain/triggers/trigger_record.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/users/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/users/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 357 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 6501 0000  o........Y.ee...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 6501 0000  o.......2H.ee...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6700 6406 a201  d.l.m.Z...g.d...
 00000070: 5a0a 6407 5300 2908 e901 0000 0029 01da  Z.d.S.)......)..
@@ -17,15 +17,15 @@
 00000100: 7573 6572 7203 0000 005a 0d75 7365 725f  userr....Z.user_
 00000110: 6465 6c65 6761 7465 7204 0000 005a 1375  delegater....Z.u
 00000120: 7365 725f 6874 7470 5f72 6573 6f75 7263  ser_http_resourc
 00000130: 6573 7205 0000 005a 0b75 7365 725f 7265  esr....Z.user_re
 00000140: 636f 7264 7206 0000 00da 075f 5f61 6c6c  cordr......__all
 00000150: 5f5f a900 720a 0000 0072 0a00 0000 fae5  __..r....r......
 00000160: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000170: 742f 7372 6331 3035 3131 3832 3038 392f  t/src1051182089/
+00000170: 742f 7372 6333 3037 3932 3336 3236 342f  t/src3079236264/
 00000180: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000190: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 000001a0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 000001b0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 000001c0: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 000001d0: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000001e0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto-0.2.8/src/roboto/domain/users/__pycache__/http_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/users/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2308 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 0409 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 0409 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6403 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6403 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6407 6408 6c0c 6d0d 5a0d 0100 6407  ..d.d.l.m.Z...d.
@@ -41,16 +41,16 @@
 00000280: 0000 0000 0000 0000 0000 0002 0000 0002  ................
 00000290: 0000 0003 0000 0073 1400 0000 7400 8300  .......s....t...
 000002a0: a001 a100 0100 7c01 7c00 5f02 6400 5300  ......|.|._.d.S.
 000002b0: a901 4e29 03da 0573 7570 6572 da08 5f5f  ..N)...super..__
 000002c0: 696e 6974 5f5f 720f 0000 0029 02da 0473  init__r....)...s
 000002d0: 656c 6672 1000 0000 a901 da09 5f5f 636c  elfr........__cl
 000002e0: 6173 735f 5fa9 00fa ea2f 636f 6465 6275  ass__..../codebu
-000002f0: 696c 642f 6f75 7470 7574 2f73 7263 3130  ild/output/src10
-00000300: 3531 3138 3230 3839 2f73 7263 2f63 6f64  51182089/src/cod
+000002f0: 696c 642f 6f75 7470 7574 2f73 7263 3330  ild/output/src30
+00000300: 3739 3233 3632 3634 2f73 7263 2f63 6f64  79236264/src/cod
 00000310: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 00000320: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 00000330: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 00000340: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 00000350: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 00000360: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 00000370: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto-0.2.8/src/roboto/domain/users/__pycache__/user.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/users/__pycache__/user.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 2271 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 df08 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 df08 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6403  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6405 6406 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6405 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6408 6409 8400 6409 8302 5a0c  ..G.d.d...d...Z.
@@ -44,16 +44,16 @@
 000002b0: 0000 7318 0000 007c 016a 007c 0264 018d  ..s....|.j.|.d..
 000002c0: 017d 037c 007c 037c 0164 028d 0253 0029  .}.|.|.|.d...S.)
 000002d0: 034e a901 720f 0000 0029 02da 0672 6563  .N..r....)...rec
 000002e0: 6f72 6472 0e00 0000 2901 da0e 6765 745f  ordr....)...get_
 000002f0: 7573 6572 5f62 795f 6964 2904 da03 636c  user_by_id)...cl
 00000300: 7372 0e00 0000 720f 0000 0072 1100 0000  sr....r....r....
 00000310: a900 7214 0000 00fa e12f 636f 6465 6275  ..r....../codebu
-00000320: 696c 642f 6f75 7470 7574 2f73 7263 3130  ild/output/src10
-00000330: 3531 3138 3230 3839 2f73 7263 2f63 6f64  51182089/src/cod
+00000320: 696c 642f 6f75 7470 7574 2f73 7263 3330  ild/output/src30
+00000330: 3739 3233 3632 3634 2f73 7263 2f63 6f64  79236264/src/cod
 00000340: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 00000350: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 00000360: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 00000370: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 00000380: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 00000390: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 000003a0: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto-0.2.8/src/roboto/domain/users/__pycache__/user_delegate.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/users/__pycache__/user_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 935 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 a703 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 a703 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6404 6405 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6406 6407 8400 6407 6500 6a08 8303 5a09  d.d...d.e.j...Z.
 00000070: 6401 5300 2908 e900 0000 004e 2901 da08  d.S.)......N)...
@@ -27,16 +27,16 @@
 000001a0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
 000001b0: 0000 0043 0000 00f3 0800 0000 7400 6401  ...C........t.d.
 000001c0: 8301 8201 2902 4eda 0e67 6574 5f75 7365  ....).N..get_use
 000001d0: 725f 6279 5f69 64a9 01da 134e 6f74 496d  r_by_id....NotIm
 000001e0: 706c 656d 656e 7465 6445 7272 6f72 a902  plementedError..
 000001f0: da04 7365 6c66 7208 0000 00a9 0072 1000  ..selfr......r..
 00000200: 0000 faea 2f63 6f64 6562 7569 6c64 2f6f  ..../codebuild/o
-00000210: 7574 7075 742f 7372 6331 3035 3131 3832  utput/src1051182
-00000220: 3038 392f 7372 632f 636f 6465 7374 6172  089/src/codestar
+00000210: 7574 7075 742f 7372 6333 3037 3932 3336  utput/src3079236
+00000220: 3236 342f 7372 632f 636f 6465 7374 6172  264/src/codestar
 00000230: 2d63 6f6e 6e65 6374 696f 6e73 2e75 732d  -connections.us-
 00000240: 7765 7374 2d32 2e61 6d61 7a6f 6e61 7773  west-2.amazonaws
 00000250: 2e63 6f6d 2f67 6974 2d68 7474 702f 3036  .com/git-http/06
 00000260: 3631 3935 3131 3233 3835 2f75 732d 7765  6195112385/us-we
 00000270: 7374 2d32 2f65 3635 3032 6138 302d 6262  st-2/e6502a80-bb
 00000280: 3465 2d34 6662 652d 3837 3263 2d35 6434  4e-4fbe-872c-5d4
 00000290: 3263 3139 3336 3939 642f 726f 626f 746f  2c193699d/roboto
```

### Comparing `roboto-0.2.8/src/roboto/domain/users/__pycache__/user_http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/users/__pycache__/user_http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 456 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 c801 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 c801 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6502 6a06  ..G.d.d...d.e.j.
 00000060: 8303 5a07 6402 5300 2906 e900 0000 0029  ..Z.d.S.)......)
 00000070: 01da 084f 7074 696f 6e61 6c4e 2902 da13  ...OptionalN)...
@@ -27,15 +27,15 @@
 000001a0: 5f71 7561 6c6e 616d 655f 5f72 0600 0000  _qualname__r....
 000001b0: 7202 0000 00da 0373 7472 da0f 5f5f 616e  r......str..__an
 000001c0: 6e6f 7461 7469 6f6e 735f 5f72 0700 0000  notations__r....
 000001d0: 7208 0000 00da 0464 6963 7472 0300 0000  r......dictr....
 000001e0: da04 626f 6f6c 7209 0000 0072 0400 0000  ..boolr....r....
 000001f0: a900 7211 0000 0072 1100 0000 faf0 2f63  ..r....r....../c
 00000200: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000210: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+00000210: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 00000220: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 00000230: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 00000240: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 00000250: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 00000260: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 00000270: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 00000280: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/domain/users/__pycache__/user_record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/domain/users/__pycache__/user_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 886 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 7603 0000  o........Y.ev...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 7603 0000  o.......2H.ev...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6403 6404 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 4700 6405 6406 8400 6406 6502 6a06  ..G.d.d...d.e.j.
 00000060: 8303 5a07 6402 5300 2907 e900 0000 0029  ..Z.d.S.)......)
 00000070: 01da 084f 7074 696f 6e61 6c4e e903 0000  ...OptionalN....
@@ -32,15 +32,15 @@
 000001f0: 7475 726e 6301 0000 0000 0000 0000 0000  turnc...........
 00000200: 0001 0000 0004 0000 0043 0000 00f3 1000  .........C......
 00000210: 0000 7c00 6a00 a001 7402 6a03 6401 a102  ..|.j...t.j.d...
 00000220: 5300 a902 4e46 2904 720c 0000 00da 0367  S...NF).r......g
 00000230: 6574 7204 0000 00da 0545 6d61 696c a901  etr......Email..
 00000240: da04 7365 6c66 a900 7215 0000 00fa e82f  ..self..r....../
 00000250: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000260: 2f73 7263 3130 3531 3138 3230 3839 2f73  /src1051182089/s
+00000260: 2f73 7263 3330 3739 3233 3632 3634 2f73  /src3079236264/s
 00000270: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000280: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000290: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 000002a0: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 000002b0: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 000002c0: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 000002d0: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto-0.2.8/src/roboto/domain/users/http_delegate.py` & `roboto-0.2.9/src/roboto/domain/users/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/users/user.py` & `roboto-0.2.9/src/roboto/domain/users/user.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/users/user_delegate.py` & `roboto-0.2.9/src/roboto/domain/users/user_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/domain/users/user_record.py` & `roboto-0.2.9/src/roboto/domain/users/user_record.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/exceptions/__init__.py` & `roboto-0.2.9/src/roboto/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/exceptions/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/exceptions/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1101 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4d04 0000  o........Y.eM...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 4d04 0000  o.......2H.eM...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6402 6c0f 6d10 5a10 6d11 5a11 6d12 5a12  d.l.m.Z.m.Z.m.Z.
@@ -45,15 +45,15 @@
 000002c0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
 000002d0: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
 000002e0: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
 000002f0: 0f00 0000 da04 6874 7470 7210 0000 0072  ......httpr....r
 00000300: 1100 0000 7212 0000 00da 075f 5f61 6c6c  ....r......__all
 00000310: 5f5f a900 7216 0000 0072 1600 0000 fae3  __..r....r......
 00000320: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000330: 742f 7372 6331 3035 3131 3832 3038 392f  t/src1051182089/
+00000330: 742f 7372 6333 3037 3932 3336 3236 342f  t/src3079236264/
 00000340: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000350: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000360: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000370: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000380: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000390: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000003a0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto-0.2.8/src/roboto/exceptions/__pycache__/domain.cpython-310.pyc` & `roboto-0.2.9/src/roboto/exceptions/__pycache__/domain.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 8433 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 f120 0000  o........Y.e. ..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 f120 0000  o.......2H.e. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3201 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6401 6c06 5a06 6403 6404 6c07  ..d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 0100 6405 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6501 a00b 6407 a101 5a0c 4700 6408  ..e...d...Z.G.d.
@@ -64,16 +64,16 @@
 000003f0: 018e 0101 007c 017c 005f 027c 027c 005f  .....|.|._.|.|._
 00000400: 0364 0053 00a9 014e 2904 da05 7375 7065  .d.S...N)...supe
 00000410: 72da 085f 5f69 6e69 745f 5f72 0a00 0000  r..__init__r....
 00000420: 720b 0000 0029 05da 0473 656c 6672 0c00  r....)...selfr..
 00000430: 0000 720d 0000 00da 0461 7267 73da 066b  ..r......args..k
 00000440: 7761 7267 73a9 01da 095f 5f63 6c61 7373  wargs....__class
 00000450: 5f5f a900 fae1 2f63 6f64 6562 7569 6c64  __..../codebuild
-00000460: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000470: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000460: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000470: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000480: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000490: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000004a0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000004b0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000004c0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000004d0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000004e0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/exceptions/__pycache__/http.cpython-310.pyc` & `roboto-0.2.9/src/roboto/exceptions/__pycache__/http.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1334 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 3605 0000  o........Y.e6...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 3605 0000  o.......2H.e6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6402 6403 8400 6403 6505 8303 5a06 4700  d.d...d.e...Z.G.
 00000060: 6404 6405 8400 6405 6506 8303 5a07 4700  d.d...d.e...Z.G.
 00000070: 6406 6407 8400 6407 6506 8303 5a08 6401  d.d...d.e...Z.d.
@@ -29,15 +29,15 @@
 000001c0: 0002 0000 0002 0000 0003 0000 0073 1400  .............s..
 000001d0: 0000 7400 8300 a001 a100 0100 7c01 7c00  ..t.........|.|.
 000001e0: 5f02 6400 5300 a901 4e29 03da 0573 7570  _.d.S...N)...sup
 000001f0: 6572 da08 5f5f 696e 6974 5f5f 7203 0000  er..__init__r...
 00000200: 0029 02da 0473 656c 6672 0600 0000 a901  .)...selfr......
 00000210: da09 5f5f 636c 6173 735f 5fa9 00fa df2f  ..__class__..../
 00000220: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000230: 2f73 7263 3130 3531 3138 3230 3839 2f73  /src1051182089/s
+00000230: 2f73 7263 3330 3739 3233 3632 3634 2f73  /src3079236264/s
 00000240: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000250: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000260: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000270: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000280: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000290: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 000002a0: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto-0.2.8/src/roboto/exceptions/domain.py` & `roboto-0.2.9/src/roboto/exceptions/domain.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/exceptions/http.py` & `roboto-0.2.9/src/roboto/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/http/__init__.py` & `roboto-0.2.9/src/roboto/http/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/http/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/http/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1316 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 2405 0000  o........Y.e$...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 2405 0000  o.......2H.e$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a08 0100 6400 6403 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6404 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
@@ -58,15 +58,15 @@
 00000390: 0000 da08 7265 7370 6f6e 7365 7210 0000  ....responser...
 000003a0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
 000003b0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
 000003c0: 1700 0000 5a0c 7465 7374 696e 675f 7574  ....Z.testing_ut
 000003d0: 696c 7218 0000 00da 075f 5f61 6c6c 5f5f  ilr......__all__
 000003e0: a900 721e 0000 0072 1e00 0000 fadd 2f63  ..r....r....../c
 000003f0: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000400: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+00000400: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 00000410: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 00000420: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 00000430: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 00000440: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 00000450: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 00000460: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 00000470: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/http/__pycache__/constants.cpython-310.pyc` & `roboto-0.2.9/src/roboto/http/__pycache__/constants.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 834 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4203 0000  o........Y.eB...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 4203 0000  o.......2H.eB...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 5a00 0900 6401 5a01 0900 6402 5a02 0900  Z...d.Z...d.Z...
 00000040: 6403 5a03 0900 6404 5a04 0900 6405 5a05  d.Z...d.Z...d.Z.
 00000050: 6406 5300 2907 7a1a 582d 526f 626f 746f  d.S.).z.X-Roboto
 00000060: 2d52 6573 6f75 7263 652d 4f77 6e65 722d  -Resource-Owner-
 00000070: 4964 5a15 726f 626f 746f 5265 736f 7572  IdZ.robotoResour
@@ -19,15 +19,15 @@
 00000120: 4144 4552 da18 4f52 475f 4f56 4552 5249  ADER..ORG_OVERRI
 00000130: 4445 5f51 5545 5259 5f50 4152 414d da14  DE_QUERY_PARAM..
 00000140: 5553 4552 5f4f 5645 5252 4944 455f 4845  USER_OVERRIDE_HE
 00000150: 4144 4552 da19 5553 4552 5f4f 5645 5252  ADER..USER_OVERR
 00000160: 4944 455f 5155 4552 595f 5041 5241 4da9  IDE_QUERY_PARAM.
 00000170: 0072 0700 0000 7207 0000 00fa de2f 636f  .r....r....../co
 00000180: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-00000190: 7263 3130 3531 3138 3230 3839 2f73 7263  rc1051182089/src
+00000190: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
 000001a0: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
 000001b0: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
 000001c0: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
 000001d0: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
 000001e0: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
 000001f0: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
 00000200: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
```

### Comparing `roboto-0.2.8/src/roboto/http/__pycache__/headers.cpython-310.pyc` & `roboto-0.2.9/src/roboto/http/__pycache__/headers.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 766 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 fe02 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 fe02 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 0904  m.Z.m.Z.m.Z.....
 00000050: 0904 0904 0904 640b 6405 6501 6506 1900  ......d.d.e.e...
 00000060: 6406 6501 6506 1900 6407 6501 6506 1900  d.e.e...d.e.e...
 00000070: 6408 6501 6507 6506 6506 6602 1900 1900  d.e.e.e.e.f.....
@@ -24,16 +24,16 @@
 00000170: 6400 7501 721a 7c02 7c04 7402 3c00 7c03  d.u.r.|.|.t.<.|.
 00000180: 6400 7501 7223 7c04 a003 7c03 a101 0100  d.u.r#|...|.....
 00000190: 7c04 5300 2901 4e29 0472 0400 0000 7206  |.S.).N).r....r.
 000001a0: 0000 0072 0500 0000 da06 7570 6461 7465  ...r......update
 000001b0: 2905 7207 0000 0072 0800 0000 7209 0000  ).r....r....r...
 000001c0: 0072 0a00 0000 da07 6865 6164 6572 73a9  .r......headers.
 000001d0: 0072 0d00 0000 fadc 2f63 6f64 6562 7569  .r....../codebui
-000001e0: 6c64 2f6f 7574 7075 742f 7372 6331 3035  ld/output/src105
-000001f0: 3131 3832 3038 392f 7372 632f 636f 6465  1182089/src/code
+000001e0: 6c64 2f6f 7574 7075 742f 7372 6333 3037  ld/output/src307
+000001f0: 3932 3336 3236 342f 7372 632f 636f 6465  9236264/src/code
 00000200: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000210: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000220: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000230: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000240: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000250: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000260: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto-0.2.8/src/roboto/http/__pycache__/http_client.cpython-310.pyc` & `roboto-0.2.9/src/roboto/http/__pycache__/http_client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 10563 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4329 0000  o........Y.eC)..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 b32a 0000  o.......2H.e.*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a01 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a08 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c09 5a08 6400 6401 6c0a 5a08 6400  d.l.Z.d.d.l.Z.d.
@@ -36,16 +36,16 @@
 00000230: 679a 9999 9999 99f1 3f69 3075 0000 2904  g.......?i0u..).
 00000240: 5a0e 6174 7465 6d70 745f 6e75 6d62 6572  Z.attempt_number
 00000250: da06 7261 6e64 6f6d da07 756e 6966 6f72  ..random..unifor
 00000260: 6dda 036d 696e 2904 7208 0000 0072 0900  m..min).r....r..
 00000270: 0000 5a10 6578 706f 6e65 6e74 6961 6c5f  ..Z.exponential_
 00000280: 7761 6974 5a08 6a69 7474 6572 6564 a900  waitZ.jittered..
 00000290: 7210 0000 00fa e02f 636f 6465 6275 696c  r....../codebuil
-000002a0: 642f 6f75 7470 7574 2f73 7263 3130 3531  d/output/src1051
-000002b0: 3138 3230 3839 2f73 7263 2f63 6f64 6573  182089/src/codes
+000002a0: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+000002b0: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
 000002c0: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 000002d0: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 000002e0: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 000002f0: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 00000300: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 00000310: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 00000320: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
@@ -324,15 +324,15 @@
 00001430: 4551 5545 5354 5f54 494d 454f 5554 5a15  EQUEST_TIMEOUTZ.
 00001440: 494e 5445 524e 414c 5f53 4552 5645 525f  INTERNAL_SERVER_
 00001450: 4552 524f 525a 0f47 4154 4557 4159 5f54  ERRORZ.GATEWAY_T
 00001460: 494d 454f 5554 5a11 544f 4f5f 4d41 4e59  IMEOUTZ.TOO_MANY
 00001470: 5f52 4551 5545 5354 535a 0b42 4144 5f47  _REQUESTSZ.BAD_G
 00001480: 4154 4557 4159 5a13 5345 5256 4943 455f  ATEWAYZ.SERVICE_
 00001490: 554e 4156 4149 4c41 424c 45da 0a56 616c  UNAVAILABLE..Val
-000014a0: 7565 4572 726f 725a 0855 524c 4572 726f  ueErrorZ.URLErro
+000014a0: 7565 4572 726f 72da 0855 524c 4572 726f  ueError..URLErro
 000014b0: 72da 0672 6561 736f 6eda 074f 5345 7272  r..reason..OSErr
 000014c0: 6f72 da05 6572 726e 6f5a 0a45 434f 4e4e  or..errnoZ.ECONN
 000014d0: 5245 5345 5472 3700 0000 2904 7219 0000  RESETr7...).r...
 000014e0: 0072 5400 0000 7223 0000 005a 1063 6f6e  .rT...r#...Z.con
 000014f0: 6e5f 7265 7365 745f 6572 726f 7272 1000  n_reset_errorr..
 00001500: 0000 7210 0000 0072 1100 0000 da08 5f5f  ..r....r......__
 00001510: 6361 6c6c 5f5f 9800 0000 7346 0000 000e  call__....sF....
@@ -354,15 +354,15 @@
 00001610: 7065 6374 6564 5f74 6f5f 6265 5f74 7261  pected_to_be_tra
 00001620: 6e73 6965 6e74 2e5f 5f72 6571 7565 7374  nsient.__request
 00001630: 5f65 7870 6563 7465 645f 746f 5f62 655f  _expected_to_be_
 00001640: 6964 656d 706f 7465 6e74 4e29 0c72 2f00  idempotentN).r/.
 00001650: 0000 7230 0000 0072 3100 0000 da07 5f5f  ..r0...r1.....__
 00001660: 646f 635f 5f72 3b00 0000 7233 0000 0072  doc__r;...r3...r
 00001670: 1800 0000 7235 0000 0072 3900 0000 7250  ....r5...r9...rP
-00001680: 0000 0072 6000 0000 7258 0000 0072 1000  ...r`...rX...r..
+00001680: 0000 0072 6100 0000 7258 0000 0072 1000  ...ra...rX...r..
 00001690: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
 000016a0: 0072 5100 0000 9000 0000 730c 0000 000a  .rQ.......s.....
 000016b0: 0004 0108 020e 0214 0312 3072 5100 0000  ..........0rQ...
 000016c0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 000016d0: 000b 0000 0040 0000 0073 8001 0000 6500  .....@...s....e.
 000016e0: 5a01 6400 5a02 5500 6503 6504 6504 6602  Z.d.Z.U.e.e.e.f.
 000016f0: 1900 6505 6401 3c00 6506 6a07 6508 1900  ..e.d.<.e.j.e...
@@ -397,17 +397,17 @@
 000018c0: 744e da0c 6261 7365 5f68 6561 6465 7273  tN..base_headers
 000018d0: da10 6465 6661 756c 745f 656e 6470 6f69  ..default_endpoi
 000018e0: 6e74 da0c 6465 6661 756c 745f 6175 7468  nt..default_auth
 000018f0: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
 00001900: 0002 0000 0043 0000 0073 2200 0000 7c01  .....C...s"...|.
 00001910: 6400 7501 7206 7c01 6e01 6900 7c00 5f00  d.u.r.|.n.i.|._.
 00001920: 7c03 7c00 5f01 7c02 7c00 5f02 6400 5300  |.|._.|.|._.d.S.
-00001930: 7216 0000 0029 0372 6300 0000 7264 0000  r....).rc...rd..
-00001940: 0072 6500 0000 2904 7219 0000 0072 6600  .re...).r....rf.
-00001950: 0000 7267 0000 0072 6800 0000 7210 0000  ..rg...rh...r...
+00001930: 7216 0000 0029 0372 6400 0000 7265 0000  r....).rd...re..
+00001940: 0072 6600 0000 2904 7219 0000 0072 6700  .rf...).r....rg.
+00001950: 0000 7268 0000 0072 6900 0000 7210 0000  ..rh...ri...r...
 00001960: 0072 1000 0000 7211 0000 0072 1800 0000  .r....r....r....
 00001970: d100 0000 7306 0000 0012 0606 010a 017a  ....s..........z
 00001980: 1348 7474 7043 6c69 656e 742e 5f5f 696e  .HttpClient.__in
 00001990: 6974 5f5f 5472 3f00 0000 7225 0000 0072  it__Tr?...r%...r
 000019a0: 4000 0000 720a 0000 0063 0500 0000 0000  @...r....c......
 000019b0: 0000 0000 0000 0600 0000 0700 0000 4300  ..............C.
 000019c0: 0000 f31c 0000 0074 007c 0164 017c 027c  .......t.|.d.|.|
@@ -420,58 +420,58 @@
 00001a30: 0000 723f 0000 0072 2500 0000 7240 0000  ..r?...r%...r@..
 00001a40: 0072 5300 0000 7210 0000 0072 1000 0000  .rS...r....r....
 00001a50: 7211 0000 00da 0664 656c 6574 65db 0000  r......delete...
 00001a60: 00f3 0800 0000 0207 0a01 06ff 0a03 7a11  ..............z.
 00001a70: 4874 7470 436c 6965 6e74 2e64 656c 6574  HttpClient.delet
 00001a80: 6572 3c00 0000 723e 0000 0063 0500 0000  er<...r>...c....
 00001a90: 0000 0000 0000 0000 0600 0000 0700 0000  ................
-00001aa0: 4300 0000 7269 0000 0029 034e 7241 0000  C...ri...).NrA..
+00001aa0: 4300 0000 726a 0000 0029 034e 7241 0000  C...rj...).NrA..
 00001ab0: 0029 0572 3c00 0000 723d 0000 0072 2500  .).r<...r=...r%.
-00001ac0: 0000 723e 0000 0072 4000 0000 726b 0000  ..r>...r@...rk..
+00001ac0: 0000 723e 0000 0072 4000 0000 726c 0000  ..r>...r@...rl..
 00001ad0: 0029 0672 1900 0000 723c 0000 0072 2500  .).r....r<...r%.
 00001ae0: 0000 723e 0000 0072 4000 0000 7253 0000  ..r>...r@...rS..
 00001af0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
 00001b00: da03 6765 74e7 0000 0073 1000 0000 0207  ..get....s......
 00001b10: 0201 0201 0201 0201 0201 06fb 0a07 7a0e  ..............z.
 00001b20: 4874 7470 436c 6965 6e74 2e67 6574 4663  HttpClient.getFc
 00001b30: 0500 0000 0000 0000 0000 0000 0600 0000  ................
-00001b40: 0700 0000 4300 0000 7269 0000 0029 034e  ....C...ri...).N
-00001b50: 5a04 504f 5354 726a 0000 0072 6b00 0000  Z.POSTrj...rk...
-00001b60: 726d 0000 0072 1000 0000 7210 0000 0072  rm...r....r....r
-00001b70: 1100 0000 da04 706f 7374 f700 0000 726f  ......post....ro
+00001b40: 0700 0000 4300 0000 726a 0000 0029 034e  ....C...rj...).N
+00001b50: 5a04 504f 5354 726b 0000 0072 6c00 0000  Z.POSTrk...rl...
+00001b60: 726e 0000 0072 1000 0000 7210 0000 0072  rn...r....r....r
+00001b70: 1100 0000 da04 706f 7374 f700 0000 7270  ......post....rp
 00001b80: 0000 007a 0f48 7474 7043 6c69 656e 742e  ...z.HttpClient.
 00001b90: 706f 7374 6305 0000 0000 0000 0000 0000  postc...........
-00001ba0: 0006 0000 0007 0000 0043 0000 0072 6900  .........C...ri.
-00001bb0: 0000 2903 4e5a 0550 4154 4348 726a 0000  ..).NZ.PATCHrj..
-00001bc0: 0072 6b00 0000 726d 0000 0072 1000 0000  .rk...rm...r....
+00001ba0: 0006 0000 0007 0000 0043 0000 0072 6a00  .........C...rj.
+00001bb0: 0000 2903 4e5a 0550 4154 4348 726b 0000  ..).NZ.PATCHrk..
+00001bc0: 0072 6c00 0000 726e 0000 0072 1000 0000  .rl...rn...r....
 00001bd0: 7210 0000 0072 1100 0000 da05 7061 7463  r....r......patc
-00001be0: 6803 0100 0072 6f00 0000 7a10 4874 7470  h....ro...z.Http
+00001be0: 6803 0100 0072 7000 0000 7a10 4874 7470  h....rp...z.Http
 00001bf0: 436c 6965 6e74 2e70 6174 6368 6305 0000  Client.patchc...
 00001c00: 0000 0000 0000 0000 0006 0000 0007 0000  ................
-00001c10: 0043 0000 0072 6900 0000 2903 4e5a 0350  .C...ri...).NZ.P
-00001c20: 5554 726a 0000 0072 6b00 0000 726d 0000  UTrj...rk...rm..
+00001c10: 0043 0000 0072 6a00 0000 2903 4e5a 0350  .C...rj...).NZ.P
+00001c20: 5554 726b 0000 0072 6c00 0000 726e 0000  UTrk...rl...rn..
 00001c30: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00001c40: da03 7075 740f 0100 0072 6f00 0000 7a0e  ..put....ro...z.
+00001c40: da03 7075 740f 0100 0072 7000 0000 7a0e  ..put....rp...z.
 00001c50: 4874 7470 436c 6965 6e74 2e70 7574 da04  HttpClient.put..
 00001c60: 7061 7468 6302 0000 0000 0000 0000 0000  pathc...........
 00001c70: 0002 0000 0003 0000 0043 0000 0073 2200  .........C...s".
 00001c80: 0000 7c00 6a00 6400 7500 7209 7401 6401  ..|.j.d.u.r.t.d.
 00001c90: 8301 8201 7c00 6a00 9b00 6402 7c01 9b00  ....|.j...d.|...
 00001ca0: 9d03 5300 2903 4e7a 3a48 7474 7043 6c69  ..S.).Nz:HttpCli
 00001cb0: 656e 742e 7572 6c20 6361 6c6c 6564 2066  ent.url called f
 00001cc0: 6f72 2063 6c69 656e 7420 7769 7468 206e  or client with n
 00001cd0: 6f20 6465 6661 756c 7420 656e 6470 6f69  o default endpoi
-00001ce0: 6e74 2eda 012f 2902 7265 0000 0072 5c00  nt.../).re...r\.
-00001cf0: 0000 2902 7219 0000 0072 7400 0000 7210  ..).r....rt...r.
+00001ce0: 6e74 2eda 012f 2902 7266 0000 0072 5c00  nt.../).rf...r\.
+00001cf0: 0000 2902 7219 0000 0072 7500 0000 7210  ..).r....ru...r.
 00001d00: 0000 0072 1000 0000 7211 0000 0072 3c00  ...r....r....r<.
 00001d10: 0000 1b01 0000 730a 0000 000a 0102 0102  ......s.........
 00001d20: 0104 ff10 037a 0e48 7474 7043 6c69 656e  .....z.HttpClien
 00001d30: 742e 7572 6cda 0b72 6571 7565 7374 5f63  t.url..request_c
 00001d40: 7478 6302 0000 0000 0000 0000 0000 000a  txc.............
-00001d50: 0000 000a 0000 0043 0000 0073 5e01 0000  .......C...s^...
+00001d50: 0000 000a 0000 0043 0000 0073 a601 0000  .......C...s....
 00001d60: 7c00 6a00 6400 7501 720a 7c00 a000 7c01  |.j.d.u.r.|...|.
 00001d70: a101 7d01 7401 a002 6401 7c01 a102 0100  ..}.t...d.|.....
 00001d80: 7c00 6a03 a004 a100 7d02 7c01 6a05 721e  |.j.....}.|.j.r.
 00001d90: 7c02 a006 7c01 6a05 a101 0100 7a5d 7407  |...|.j.....z]t.
 00001da0: 6a08 7407 a009 740a 7c01 8301 a101 7407  j.t...t.|.....t.
 00001db0: a00b 6402 a101 6403 7c00 a00c 7c01 6a0d  ..d...d.|...|.j.
 00001dc0: a101 6404 8d04 4400 5d42 7d03 7c03 8f36  ..d...D.]B}.|..6
@@ -479,127 +479,138 @@
 00001de0: 6405 8d02 7d04 7c01 6a13 7d05 7c05 6400  d...}.|.j.}.|.d.
 00001df0: 7501 724d 7c05 7c04 5f14 7c02 a015 a100  u.rM|.|._.|.....
 00001e00: 4400 5d0a 5c02 7d06 7d07 7c04 a016 7c06  D.].\.}.}.|...|.
 00001e10: 7c07 a102 0100 7151 7417 740e 6a0f a018  |.....qQt.t.j...
 00001e20: 7c04 a101 8301 5700 0200 6400 0400 0400  |.....W...d.....
 00001e30: 8303 0100 0200 0100 5700 5300 3100 7371  ........W.S.1.sq
 00001e40: 7701 0100 0100 0100 5900 0100 7134 5700  w.......Y...q4W.
-00001e50: 7420 6409 8301 8201 0400 740e 6a19 6a1a  t d.......t.j.j.
+00001e50: 7427 640a 8301 8201 0400 740e 6a19 6a1a  t'd.......t.j.j.
 00001e60: 79a7 0100 7d08 0100 7a1e 7c08 6a1b 7d09  y...}...z.|.j.}.
 00001e70: 7c09 6406 6b04 7295 7c09 6407 6b00 7295  |.d.k.r.|.d.k.r.
 00001e80: 741c 7c08 8301 6400 8202 7c09 6408 6b04  t.|...d...|.d.k.
 00001e90: 729e 741d 7c08 8301 6400 8202 741e 7c08  r.t.|...d...t.|.
 00001ea0: 8301 6400 8202 6400 7d08 7e08 7701 0400  ..d...d.}.~.w...
-00001eb0: 741f 79ae 0100 0100 0100 8200 7700 290a  t.y.........w.).
-00001ec0: 4e7a 0225 73e9 0a00 0000 5429 045a 0572  Nz.%s.....T).Z.r
-00001ed0: 6574 7279 da04 7374 6f70 da07 7265 7261  etry..stop..rera
-00001ee0: 6973 65da 0477 6169 7429 0172 3d00 0000  ise..wait).r=...
-00001ef0: 698f 0100 0072 0b00 0000 69f3 0100 005a  i....r....i....Z
-00001f00: 0b55 6e72 6561 6368 6162 6c65 2921 7264  .Unreachable)!rd
-00001f10: 0000 0072 5600 0000 da05 6465 6275 6772  ...rV.....debugr
-00001f20: 6300 0000 da04 636f 7079 7225 0000 0072  c.....copyr%...r
-00001f30: 4d00 0000 da08 7465 6e61 6369 7479 5a08  M.....tenacityZ.
-00001f40: 5265 7472 7969 6e67 5a12 7265 7472 795f  RetryingZ.retry_
-00001f50: 6966 5f65 7863 6570 7469 6f6e 7251 0000  if_exceptionrQ..
-00001f60: 005a 1273 746f 705f 6166 7465 725f 6174  .Z.stop_after_at
-00001f70: 7465 6d70 74da 055f 7761 6974 723e 0000  tempt.._waitr>..
-00001f80: 0072 3200 0000 7253 0000 005a 0752 6571  .r2...rS...Z.Req
-00001f90: 7565 7374 723c 0000 0072 3d00 0000 7248  uestr<...r=...rH
-00001fa0: 0000 0072 3f00 0000 7226 0000 00da 0a61  ...r?...r&.....a
-00001fb0: 6464 5f68 6561 6465 7272 1300 0000 da07  dd_headerr......
-00001fc0: 7572 6c6f 7065 6e72 5900 0000 725a 0000  urlopenrY...rZ..
-00001fd0: 0072 5b00 0000 7202 0000 0072 0400 0000  .r[...r....r....
-00001fe0: 7203 0000 00da 0945 7863 6570 7469 6f6e  r......Exception
-00001ff0: 721f 0000 0029 0a72 1900 0000 7276 0000  r....).r....rv..
-00002000: 0072 2500 0000 5a07 6174 7465 6d70 7472  .r%...Z.attemptr
-00002010: 5300 0000 5a08 7265 715f 626f 6479 da03  S...Z.req_body..
-00002020: 6b65 79da 0576 616c 7565 7254 0000 0072  key..valuerT...r
-00002030: 2300 0000 7210 0000 0072 1000 0000 7211  #...r....r....r.
-00002040: 0000 005a 095f 5f72 6571 7565 7374 2201  ...Z.__request".
-00002050: 0000 734e 0000 000a 010a 010c 020a 0206  ..sN............
-00002060: 010c 0102 0204 0104 0106 0102 ff08 0302  ................
-00002070: 010a 010a fa06 0806 0108 0106 ff06 0408  ................
-00002080: 0106 0110 020e 010e 0228 f402 f808 2012  .........(.... .
-00002090: f506 0110 010a 0108 010a 010a 0208 800c  ................
-000020a0: 0102 0102 ff7a 1448 7474 7043 6c69 656e  .....z.HttpClien
-000020b0: 742e 5f5f 7265 7175 6573 74da 0677 6169  t.__request..wai
-000020c0: 7465 7263 0200 0000 0000 0000 0000 0000  terc............
-000020d0: 0300 0000 0400 0000 0300 0000 731e 0000  ............s...
-000020e0: 0047 0087 0066 0164 0164 0284 0864 0274  .G...f.d.d...d.t
-000020f0: 006a 016a 0283 037d 027c 0283 0053 0029  .j.j...}.|...S.)
-00002100: 034e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
-00002110: 0000 0004 0000 0000 0000 0073 2400 0000  ...........s$...
-00002120: 6500 5a01 6400 5a02 6401 6503 6a04 6402  e.Z.d.Z.d.e.j.d.
-00002130: 6505 6604 8700 6601 6403 6404 840c 5a06  e.f...f.d.d...Z.
-00002140: 6405 5300 2906 7a20 4874 7470 436c 6965  d.S.).z HttpClie
-00002150: 6e74 2e5f 7761 6974 2e3c 6c6f 6361 6c73  nt._wait.<locals
-00002160: 3e2e 5761 6974 6572 7208 0000 0072 0a00  >.Waiterr....r..
-00002170: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00002180: 0000 0003 0000 0013 0000 0073 0e00 0000  ...........s....
-00002190: 8800 7c01 6400 8302 6401 1b00 5300 2902  ..|.d...d...S.).
-000021a0: 4e69 e803 0000 7210 0000 0029 0272 1900  Ni....r....).r..
-000021b0: 0000 7208 0000 00a9 0172 8400 0000 7210  ..r......r....r.
-000021c0: 0000 0072 1100 0000 7260 0000 0051 0100  ...r....r`...Q..
-000021d0: 0073 0200 0000 0e01 7a29 4874 7470 436c  .s......z)HttpCl
-000021e0: 6965 6e74 2e5f 7761 6974 2e3c 6c6f 6361  ient._wait.<loca
-000021f0: 6c73 3e2e 5761 6974 6572 2e5f 5f63 616c  ls>.Waiter.__cal
-00002200: 6c5f 5f4e 2907 722f 0000 0072 3000 0000  l__N).r/...r0...
-00002210: 7231 0000 0072 7d00 0000 da0e 5265 7472  r1...r}.....Retr
-00002220: 7943 616c 6c53 7461 7465 da05 666c 6f61  yCallState..floa
-00002230: 7472 6000 0000 7210 0000 0072 8500 0000  tr`...r....r....
-00002240: 7210 0000 0072 1100 0000 da06 5761 6974  r....r......Wait
-00002250: 6572 5001 0000 7304 0000 0008 001c 0172  erP...s........r
-00002260: 8800 0000 2903 727d 0000 0072 7a00 0000  ....).r}...rz...
-00002270: da09 7761 6974 5f62 6173 6529 0372 1900  ..wait_base).r..
-00002280: 0000 7284 0000 0072 8800 0000 7210 0000  ..r....r....r...
-00002290: 0072 8500 0000 7211 0000 0072 7e00 0000  .r....r....r~...
-000022a0: 4f01 0000 7304 0000 0018 0106 047a 1048  O...s........z.H
-000022b0: 7474 7043 6c69 656e 742e 5f77 6169 7429  ttpClient._wait)
-000022c0: 034e 4e4e 2903 4e4e 5429 034e 4e46 291b  .NNN).NNT).NNF).
-000022d0: 722f 0000 0072 3000 0000 7231 0000 0072  r/...r0...r1...r
-000022e0: 2400 0000 7237 0000 0072 3300 0000 7235  $...r7...r3...r5
-000022f0: 0000 0072 3600 0000 da14 4874 7470 5265  ...r6.....HttpRe
-00002300: 7175 6573 7444 6563 6f72 6174 6f72 7218  questDecoratorr.
-00002310: 0000 0072 3900 0000 7250 0000 0072 1300  ...r9...rP...r..
-00002320: 0000 726e 0000 0072 1200 0000 724f 0000  ..rn...r....rO..
-00002330: 0072 7000 0000 7271 0000 0072 7200 0000  .rp...rq...rr...
-00002340: 7273 0000 0072 3c00 0000 723b 0000 0072  rs...r<...r;...r
-00002350: 6c00 0000 727d 0000 0072 7a00 0000 7289  l...r}...rz...r.
-00002360: 0000 0072 7e00 0000 7210 0000 0072 1000  ...r~...r....r..
-00002370: 0000 7210 0000 0072 1100 0000 7262 0000  ..r....r....rb..
-00002380: 00cc 0000 0073 9e00 0000 0a00 1001 0e01  .....s..........
-00002390: 0e01 0204 0201 0201 04fc 1002 02fe 0803  ................
-000023a0: 02fd 0804 0afc 020d 0201 0201 04fb 0403  ................
-000023b0: 02fd 0804 02fc 0205 02fb 0206 0afa 020f  ................
-000023c0: 0201 0201 04fb 0202 02fe 0803 02fd 0204  ................
-000023d0: 02fc 0205 02fb 0206 0afa 0213 0201 0201  ................
-000023e0: 04fb 0403 02fd 0804 02fc 0205 02fb 0206  ................
-000023f0: 0afa 020f 0201 0201 04fb 0403 02fd 0804  ................
-00002400: 02fc 0205 02fb 0206 0afa 020f 0201 0201  ................
-00002410: 04fb 0403 02fd 0804 02fc 0205 02fb 0206  ................
-00002420: 0afa 120c 1207 1a2d 7262 0000 0029 2572  .......-rb...)%r
-00002430: 5f00 0000 7220 0000 005a 0b68 7474 702e  _...r ...Z.http.
-00002440: 636c 6965 6e74 7229 0000 00da 076c 6f67  clientr).....log
-00002450: 6769 6e67 720d 0000 0072 3500 0000 5a0c  gingr....r5...Z.
-00002460: 7572 6c6c 6962 2e65 7272 6f72 7232 0000  urllib.errorr2..
-00002470: 00da 0c75 726c 6c69 622e 7061 7273 65da  ...urllib.parse.
-00002480: 0e75 726c 6c69 622e 7265 7175 6573 745a  .urllib.requestZ
-00002490: 0f75 726c 6c69 622e 7265 7370 6f6e 7365  .urllib.response
-000024a0: 727d 0000 005a 0d74 656e 6163 6974 792e  r}...Z.tenacity.
-000024b0: 7761 6974 5a11 726f 626f 746f 2e65 7863  waitZ.roboto.exc
-000024c0: 6570 7469 6f6e 7372 0200 0000 7203 0000  eptionsr....r...
-000024d0: 0072 0400 0000 7206 0000 00da 0573 6572  .r....r......ser
-000024e0: 6465 7207 0000 00da 0967 6574 4c6f 6767  der......getLogg
-000024f0: 6572 7256 0000 00da 066f 626a 6563 745a  errV.....objectZ
-00002500: 0f44 4546 4155 4c54 5f48 4541 4445 5253  .DEFAULT_HEADERS
-00002510: da08 4361 6c6c 6162 6c65 7286 0000 0072  ..Callabler....r
-00002520: 3600 0000 da0d 4261 7365 4578 6365 7074  6.....BaseExcept
-00002530: 696f 6e72 8700 0000 724f 0000 0072 1200  ionr....rO...r..
-00002540: 0000 7213 0000 0072 3b00 0000 728a 0000  ..r....r;...r...
-00002550: 0072 5100 0000 7262 0000 0072 1000 0000  .rQ...rb...r....
-00002560: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00002570: 083c 6d6f 6475 6c65 3e01 0000 0073 4200  .<module>....sB.
-00002580: 0000 0800 0801 0801 0801 0801 0801 0801  ................
-00002590: 0801 0801 0801 0801 0802 0801 1402 0c06  ................
-000025a0: 0c01 0a02 0602 0403 1201 04ff 0205 0401  ................
-000025b0: 02ff 0801 02ff 0202 0afe 0e08 0e23 103f  .............#.?
-000025c0: 0e03 123c                                ...<
+00001eb0: 740e 6a19 6a1f 79cb 0100 7d08 0100 7a17  t.j.j.y...}...z.
+00001ec0: 7420 7c08 6a21 7422 8302 72c6 7c08 6a21  t |.j!t"..r.|.j!
+00001ed0: 6a23 7423 6a24 6b02 72c6 7425 6409 7c01  j#t#j$k.r.t%d.|.
+00001ee0: 6a11 9b00 9d02 8301 6400 8202 8200 6400  j.......d.....d.
+00001ef0: 7d08 7e08 7701 0400 7426 79d2 0100 0100  }.~.w...t&y.....
+00001f00: 0100 8200 7700 290b 4e7a 0225 73e9 0a00  ....w.).Nz.%s...
+00001f10: 0000 5429 045a 0572 6574 7279 da04 7374  ..T).Z.retry..st
+00001f20: 6f70 da07 7265 7261 6973 65da 0477 6169  op..reraise..wai
+00001f30: 7429 0172 3d00 0000 698f 0100 0072 0b00  t).r=...i....r..
+00001f40: 0000 69f3 0100 007a 1d43 6f75 6c64 6e27  ..i....z.Couldn'
+00001f50: 7420 636f 6e6e 6563 7420 746f 2065 6e64  t connect to end
+00001f60: 706f 696e 7420 5a0b 556e 7265 6163 6861  point Z.Unreacha
+00001f70: 626c 6529 2872 6500 0000 7256 0000 00da  ble)(re...rV....
+00001f80: 0564 6562 7567 7264 0000 00da 0463 6f70  .debugrd.....cop
+00001f90: 7972 2500 0000 724d 0000 00da 0874 656e  yr%...rM.....ten
+00001fa0: 6163 6974 795a 0852 6574 7279 696e 675a  acityZ.RetryingZ
+00001fb0: 1272 6574 7279 5f69 665f 6578 6365 7074  .retry_if_except
+00001fc0: 696f 6e72 5100 0000 5a12 7374 6f70 5f61  ionrQ...Z.stop_a
+00001fd0: 6674 6572 5f61 7474 656d 7074 da05 5f77  fter_attempt.._w
+00001fe0: 6169 7472 3e00 0000 7232 0000 0072 5300  aitr>...r2...rS.
+00001ff0: 0000 5a07 5265 7175 6573 7472 3c00 0000  ..Z.Requestr<...
+00002000: 723d 0000 0072 4800 0000 723f 0000 0072  r=...rH...r?...r
+00002010: 2600 0000 da0a 6164 645f 6865 6164 6572  &.....add_header
+00002020: 7213 0000 00da 0775 726c 6f70 656e 7259  r......urlopenrY
+00002030: 0000 0072 5a00 0000 725b 0000 0072 0200  ...rZ...r[...r..
+00002040: 0000 7204 0000 0072 0300 0000 725d 0000  ..r....r....r]..
+00002050: 0072 4400 0000 725e 0000 0072 5f00 0000  .rD...r^...r_...
+00002060: 7260 0000 005a 0c45 434f 4e4e 5245 4655  r`...Z.ECONNREFU
+00002070: 5345 44da 1643 6f6e 6e65 6374 696f 6e52  SED..ConnectionR
+00002080: 6566 7573 6564 4572 726f 72da 0945 7863  efusedError..Exc
+00002090: 6570 7469 6f6e 721f 0000 0029 0a72 1900  eptionr....).r..
+000020a0: 0000 7277 0000 0072 2500 0000 5a07 6174  ..rw...r%...Z.at
+000020b0: 7465 6d70 7472 5300 0000 5a08 7265 715f  temptrS...Z.req_
+000020c0: 626f 6479 da03 6b65 79da 0576 616c 7565  body..key..value
+000020d0: 7254 0000 0072 2300 0000 7210 0000 0072  rT...r#...r....r
+000020e0: 1000 0000 7211 0000 005a 095f 5f72 6571  ....r....Z.__req
+000020f0: 7565 7374 2201 0000 7364 0000 000a 010a  uest"...sd......
+00002100: 010c 020a 0206 010c 0102 0204 0104 0106  ................
+00002110: 0102 ff08 0302 010a 010a fa06 0806 0108  ................
+00002120: 0106 ff06 0408 0106 0110 020e 010e 0228  ...............(
+00002130: f402 f808 2a12 eb06 0110 010a 0108 010a  ....*...........
+00002140: 010a 0208 8012 010a 0202 ff0e 0202 020a  ................
+00002150: 0102 ff02 0202 fe02 0408 800c 0102 0102  ................
+00002160: ff7a 1448 7474 7043 6c69 656e 742e 5f5f  .z.HttpClient.__
+00002170: 7265 7175 6573 74da 0677 6169 7465 7263  request..waiterc
+00002180: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00002190: 0400 0000 0300 0000 731e 0000 0047 0087  ........s....G..
+000021a0: 0066 0164 0164 0284 0864 0274 006a 016a  .f.d.d...d.t.j.j
+000021b0: 0283 037d 027c 0283 0053 0029 034e 6300  ...}.|...S.).Nc.
+000021c0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+000021d0: 0000 0000 0000 0073 2400 0000 6500 5a01  .......s$...e.Z.
+000021e0: 6400 5a02 6401 6503 6a04 6402 6505 6604  d.Z.d.e.j.d.e.f.
+000021f0: 8700 6601 6403 6404 840c 5a06 6405 5300  ..f.d.d...Z.d.S.
+00002200: 2906 7a20 4874 7470 436c 6965 6e74 2e5f  ).z HttpClient._
+00002210: 7761 6974 2e3c 6c6f 6361 6c73 3e2e 5761  wait.<locals>.Wa
+00002220: 6974 6572 7208 0000 0072 0a00 0000 6302  iterr....r....c.
+00002230: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00002240: 0000 0013 0000 0073 0e00 0000 8800 7c01  .......s......|.
+00002250: 6400 8302 6401 1b00 5300 2902 4e69 e803  d...d...S.).Ni..
+00002260: 0000 7210 0000 0029 0272 1900 0000 7208  ..r....).r....r.
+00002270: 0000 00a9 0172 8600 0000 7210 0000 0072  .....r....r....r
+00002280: 1100 0000 7261 0000 005b 0100 0073 0200  ....ra...[...s..
+00002290: 0000 0e01 7a29 4874 7470 436c 6965 6e74  ....z)HttpClient
+000022a0: 2e5f 7761 6974 2e3c 6c6f 6361 6c73 3e2e  ._wait.<locals>.
+000022b0: 5761 6974 6572 2e5f 5f63 616c 6c5f 5f4e  Waiter.__call__N
+000022c0: 2907 722f 0000 0072 3000 0000 7231 0000  ).r/...r0...r1..
+000022d0: 0072 7e00 0000 da0e 5265 7472 7943 616c  .r~.....RetryCal
+000022e0: 6c53 7461 7465 da05 666c 6f61 7472 6100  lState..floatra.
+000022f0: 0000 7210 0000 0072 8700 0000 7210 0000  ..r....r....r...
+00002300: 0072 1100 0000 da06 5761 6974 6572 5a01  .r......WaiterZ.
+00002310: 0000 7304 0000 0008 001c 0172 8a00 0000  ..s........r....
+00002320: 2903 727e 0000 0072 7b00 0000 da09 7761  ).r~...r{.....wa
+00002330: 6974 5f62 6173 6529 0372 1900 0000 7286  it_base).r....r.
+00002340: 0000 0072 8a00 0000 7210 0000 0072 8700  ...r....r....r..
+00002350: 0000 7211 0000 0072 7f00 0000 5901 0000  ..r....r....Y...
+00002360: 7304 0000 0018 0106 047a 1048 7474 7043  s........z.HttpC
+00002370: 6c69 656e 742e 5f77 6169 7429 034e 4e4e  lient._wait).NNN
+00002380: 2903 4e4e 5429 034e 4e46 291b 722f 0000  ).NNT).NNF).r/..
+00002390: 0072 3000 0000 7231 0000 0072 2400 0000  .r0...r1...r$...
+000023a0: 7237 0000 0072 3300 0000 7235 0000 0072  r7...r3...r5...r
+000023b0: 3600 0000 da14 4874 7470 5265 7175 6573  6.....HttpReques
+000023c0: 7444 6563 6f72 6174 6f72 7218 0000 0072  tDecoratorr....r
+000023d0: 3900 0000 7250 0000 0072 1300 0000 726f  9...rP...r....ro
+000023e0: 0000 0072 1200 0000 724f 0000 0072 7100  ...r....rO...rq.
+000023f0: 0000 7272 0000 0072 7300 0000 7274 0000  ..rr...rs...rt..
+00002400: 0072 3c00 0000 723b 0000 0072 6d00 0000  .r<...r;...rm...
+00002410: 727e 0000 0072 7b00 0000 728b 0000 0072  r~...r{...r....r
+00002420: 7f00 0000 7210 0000 0072 1000 0000 7210  ....r....r....r.
+00002430: 0000 0072 1100 0000 7263 0000 00cc 0000  ...r....rc......
+00002440: 0073 9e00 0000 0a00 1001 0e01 0e01 0204  .s..............
+00002450: 0201 0201 04fc 1002 02fe 0803 02fd 0804  ................
+00002460: 0afc 020d 0201 0201 04fb 0403 02fd 0804  ................
+00002470: 02fc 0205 02fb 0206 0afa 020f 0201 0201  ................
+00002480: 04fb 0202 02fe 0803 02fd 0204 02fc 0205  ................
+00002490: 02fb 0206 0afa 0213 0201 0201 04fb 0403  ................
+000024a0: 02fd 0804 02fc 0205 02fb 0206 0afa 020f  ................
+000024b0: 0201 0201 04fb 0403 02fd 0804 02fc 0205  ................
+000024c0: 02fb 0206 0afa 020f 0201 0201 04fb 0403  ................
+000024d0: 02fd 0804 02fc 0205 02fb 0206 0afa 120c  ................
+000024e0: 1207 1a37 7263 0000 0029 2572 6000 0000  ...7rc...)%r`...
+000024f0: 7220 0000 005a 0b68 7474 702e 636c 6965  r ...Z.http.clie
+00002500: 6e74 7229 0000 00da 076c 6f67 6769 6e67  ntr).....logging
+00002510: 720d 0000 0072 3500 0000 5a0c 7572 6c6c  r....r5...Z.urll
+00002520: 6962 2e65 7272 6f72 7232 0000 00da 0c75  ib.errorr2.....u
+00002530: 726c 6c69 622e 7061 7273 65da 0e75 726c  rllib.parse..url
+00002540: 6c69 622e 7265 7175 6573 745a 0f75 726c  lib.requestZ.url
+00002550: 6c69 622e 7265 7370 6f6e 7365 727e 0000  lib.responser~..
+00002560: 005a 0d74 656e 6163 6974 792e 7761 6974  .Z.tenacity.wait
+00002570: 5a11 726f 626f 746f 2e65 7863 6570 7469  Z.roboto.excepti
+00002580: 6f6e 7372 0200 0000 7203 0000 0072 0400  onsr....r....r..
+00002590: 0000 7206 0000 00da 0573 6572 6465 7207  ..r......serder.
+000025a0: 0000 00da 0967 6574 4c6f 6767 6572 7256  .....getLoggerrV
+000025b0: 0000 00da 066f 626a 6563 745a 0f44 4546  .....objectZ.DEF
+000025c0: 4155 4c54 5f48 4541 4445 5253 da08 4361  AULT_HEADERS..Ca
+000025d0: 6c6c 6162 6c65 7288 0000 0072 3600 0000  llabler....r6...
+000025e0: da0d 4261 7365 4578 6365 7074 696f 6e72  ..BaseExceptionr
+000025f0: 8900 0000 724f 0000 0072 1200 0000 7213  ....rO...r....r.
+00002600: 0000 0072 3b00 0000 728c 0000 0072 5100  ...r;...r....rQ.
+00002610: 0000 7263 0000 0072 1000 0000 7210 0000  ..rc...r....r...
+00002620: 0072 1000 0000 7211 0000 00da 083c 6d6f  .r....r......<mo
+00002630: 6475 6c65 3e01 0000 0073 4200 0000 0800  dule>....sB.....
+00002640: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+00002650: 0801 0801 0802 0801 1402 0c06 0c01 0a02  ................
+00002660: 0602 0403 1201 04ff 0205 0401 02ff 0801  ................
+00002670: 02ff 0202 0afe 0e08 0e23 103f 0e03 123c  .........#.?...<
```

### Comparing `roboto-0.2.8/src/roboto/http/__pycache__/request_decorators.cpython-310.pyc` & `roboto-0.2.9/src/roboto/http/__pycache__/request_decorators.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3177 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 690c 0000  o........Y.ei...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 690c 0000  o.......2H.ei...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
@@ -33,16 +33,16 @@
 00000200: 7574 6844 6563 6f72 6174 6f72 5f5f 7573  uthDecorator__us
 00000210: 6572 5f69 64da 0775 7365 725f 6964 6302  er_id..user_idc.
 00000220: 0000 0000 0000 0000 0000 0002 0000 0002  ................
 00000230: 0000 0043 0000 00f3 0a00 0000 7c01 7c00  ...C........|.|.
 00000240: 5f00 6400 5300 a901 4e29 0172 0e00 0000  _.d.S...N).r....
 00000250: 2902 da04 7365 6c66 720f 0000 00a9 0072  )...selfr......r
 00000260: 1300 0000 fae7 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000270: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000280: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000270: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000280: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000290: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 000002a0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000002b0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000002c0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000002d0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000002e0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000002f0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/http/__pycache__/response.cpython-310.pyc` & `roboto-0.2.9/src/roboto/http/__pycache__/response.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 5800 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 a816 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 b116 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6403 6404 6c07 6d08 5a08 0100 6508  ..d.d.l.m.Z...e.
 00000070: 8300 5a09 6503 a00a 6405 a101 5a0b 4700  ..Z.e...d...Z.G.
@@ -28,16 +28,16 @@
 000001b0: 0c42 6174 6368 5265 7175 6573 74da 0872  .BatchRequest..r
 000001c0: 6571 7565 7374 734e 2906 da08 5f5f 6e61  equestsN)...__na
 000001d0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 000001e0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da04  ..__qualname__..
 000001f0: 6c69 7374 7205 0000 00da 0f5f 5f61 6e6e  listr......__ann
 00000200: 6f74 6174 696f 6e73 5f5f a900 720d 0000  otations__..r...
 00000210: 0072 0d00 0000 fadd 2f63 6f64 6562 7569  .r....../codebui
-00000220: 6c64 2f6f 7574 7075 742f 7372 6331 3035  ld/output/src105
-00000230: 3131 3832 3038 392f 7372 632f 636f 6465  1182089/src/code
+00000220: 6c64 2f6f 7574 7075 742f 7372 6333 3037  ld/output/src307
+00000230: 3932 3336 3236 342f 7372 632f 636f 6465  9236264/src/code
 00000240: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000250: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000260: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000270: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000280: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000290: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 000002a0: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
@@ -295,127 +295,127 @@
 00001260: 3634 6465 636f 6465 7242 0000 0072 4400  64decoderB...rD.
 00001270: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
 00001280: 0072 4200 0000 7700 0000 7308 0000 0010  .rB...w...s.....
 00001290: 0308 0110 ff10 027a 1650 6167 696e 6174  .......z.Paginat
 000012a0: 696f 6e54 6f6b 656e 2e64 6563 6f64 65da  ionToken.decode.
 000012b0: 0574 6f6b 656e 6302 0000 0000 0000 0000  .tokenc.........
 000012c0: 0000 0009 0000 000a 0000 0043 0000 0073  ...........C...s
-000012d0: b800 0000 7c01 6400 7500 7208 7400 a001  ....|.d.u.r.t...
+000012d0: be00 0000 7c01 6400 7500 7208 7400 a001  ....|.d.u.r.t...
 000012e0: a100 5300 7a3b 7400 a002 7c01 a101 7d02  ..S.z;t...|...}.
 000012f0: 7c02 a003 7404 6a05 6a06 a101 731f 7407  |...t.j.j...s.t.
 00001300: a008 6401 7c02 a102 0100 7409 6402 8301  ..d.|.....t.d...
 00001310: 8201 7c02 6a0a 6403 6404 6405 8d02 5c03  ..|.j.d.d.d...\.
 00001320: 7d03 7d04 7d05 7404 7c03 8301 7d06 740b  }.}.}.t.|...}.t.
 00001330: 7c04 8301 7d07 7c00 7c06 7c07 7c07 740b  |...}.|.|.|.|.t.
 00001340: 6a0c 6b02 7240 740d a00e 7c05 a101 8303  j.k.r@t...|.....
 00001350: 5700 5300 7c05 8303 5700 5300 0400 740f  W.S.|...W.S...t.
-00001360: 795b 0100 7d08 0100 7a0c 7407 6a08 6406  y[..}...z.t.j.d.
-00001370: 7c08 6407 8d02 0100 7409 6408 8301 6400  |.d.....t.d...d.
-00001380: 8202 6400 7d08 7e08 7701 7700 2909 4e7a  ..d.}.~.w.w.).Nz
-00001390: 2249 6e76 616c 6964 2070 6167 696e 6174  "Invalid paginat
-000013a0: 696f 6e20 746f 6b65 6e20 7363 6865 6d65  ion token scheme
-000013b0: 2025 737a 1f49 6e76 616c 6964 2070 6167   %sz.Invalid pag
-000013c0: 696e 6174 696f 6e20 746f 6b65 6e20 7363  ination token sc
-000013d0: 6865 6d65 fa01 3a72 0300 0000 2901 da08  heme..:r....)...
-000013e0: 6d61 7873 706c 6974 7a18 496e 7661 6c69  maxsplitz.Invali
-000013f0: 6420 7061 6769 6e61 7469 6f6e 2074 6f6b  d pagination tok
-00001400: 656e 2901 da08 6578 635f 696e 666f 7a1f  en)...exc_infoz.
-00001410: 496e 7661 6c69 6420 7061 6769 6e61 7469  Invalid paginati
-00001420: 6f6e 2074 6f6b 656e 2066 6f72 6d61 7429  on token format)
-00001430: 1072 3800 0000 723c 0000 0072 4200 0000  .r8...r<...rB...
-00001440: da0a 7374 6172 7473 7769 7468 7236 0000  ..startswithr6..
-00001450: 0072 3700 0000 7214 0000 00da 066c 6f67  .r7...r......log
-00001460: 6765 7272 1100 0000 da0a 5661 6c75 6545  gerr......ValueE
-00001470: 7272 6f72 da05 7370 6c69 7472 3200 0000  rror..splitr2...
-00001480: 7234 0000 0072 1800 0000 7219 0000 0072  r4...r....r....r
-00001490: 1a00 0000 2909 721b 0000 0072 4800 0000  ....).r....rH...
-000014a0: da07 6465 636f 6465 64da 0673 6368 656d  ..decoded..schem
-000014b0: 65da 0865 6e63 6f64 696e 6772 1000 0000  e..encodingr....
-000014c0: 5a17 7061 6769 6e61 7469 6f6e 5f74 6f6b  Z.pagination_tok
-000014d0: 656e 5f73 6368 656d 655a 1970 6167 696e  en_schemeZ.pagin
-000014e0: 6174 696f 6e5f 746f 6b65 6e5f 656e 636f  ation_token_enco
-000014f0: 6469 6e67 da01 6572 0d00 0000 720d 0000  ding..er....r...
-00001500: 0072 0e00 0000 da0a 6672 6f6d 5f74 6f6b  .r......from_tok
-00001510: 656e 7e00 0000 732e 0000 0008 0208 0102  en~...s.........
-00001520: 010a 010e 010c 0108 0114 0108 0108 0102  ................
-00001530: 0102 0102 010a 0208 ff06 fd02 0506 fb0e  ................
-00001540: 070e 010a 0108 8002 fe7a 1a50 6167 696e  .........z.Pagin
-00001550: 6174 696f 6e54 6f6b 656e 2e66 726f 6d5f  ationToken.from_
-00001560: 746f 6b65 6e72 5100 0000 7252 0000 0063  tokenrQ...rR...c
-00001570: 0400 0000 0000 0000 0000 0000 0400 0000  ................
-00001580: 0200 0000 4300 0000 7316 0000 007c 017c  ....C...s....|.|
-00001590: 005f 007c 027c 005f 017c 037c 005f 0264  ._.|.|._.|.|._.d
-000015a0: 0053 0072 1600 0000 2903 7239 0000 0072  .S.r....).r9...r
-000015b0: 3a00 0000 723b 0000 0029 0472 1f00 0000  :...r;...).r....
-000015c0: 7251 0000 0072 5200 0000 7210 0000 0072  rQ...rR...r....r
-000015d0: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
-000015e0: 5f5f 696e 6974 5f5f 9500 0000 7306 0000  __init__....s...
-000015f0: 0006 0606 010a 017a 1850 6167 696e 6174  .......z.Paginat
-00001600: 696f 6e54 6f6b 656e 2e5f 5f69 6e69 745f  ionToken.__init_
-00001610: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00001620: 0000 0300 0000 4300 0000 7316 0000 007c  ......C...s....|
-00001630: 006a 0072 0974 0174 027c 0083 0183 0153  .j.r.t.t.|.....S
-00001640: 0064 0153 0029 024e 7201 0000 0029 0372  .d.S.).Nr....).r
-00001650: 3b00 0000 7246 0000 0072 2600 0000 a901  ;...rF...r&.....
-00001660: 721f 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00001670: 0e00 0000 da07 5f5f 6c65 6e5f 5f9f 0000  ......__len__...
-00001680: 0073 0200 0000 1601 7a17 5061 6769 6e61  .s......z.Pagina
-00001690: 7469 6f6e 546f 6b65 6e2e 5f5f 6c65 6e5f  tionToken.__len_
-000016a0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-000016b0: 0000 0200 0000 4300 0000 7308 0000 007c  ......C...s....|
-000016c0: 00a0 00a1 0053 0072 1600 0000 2901 da08  .....S.r....)...
-000016d0: 746f 5f74 6f6b 656e 7256 0000 0072 0d00  to_tokenrV...r..
-000016e0: 0000 720d 0000 0072 0e00 0000 da07 5f5f  ..r....r......__
-000016f0: 7374 725f 5fa2 0000 0073 0200 0000 0801  str__....s......
-00001700: 7a17 5061 6769 6e61 7469 6f6e 546f 6b65  z.PaginationToke
-00001710: 6e2e 5f5f 7374 725f 5f63 0100 0000 0000  n.__str__c......
-00001720: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00001730: 0000 7306 0000 007c 006a 0053 0072 1600  ..s....|.j.S.r..
-00001740: 0000 2901 723b 0000 0072 5600 0000 720d  ..).r;...rV...r.
-00001750: 0000 0072 0d00 0000 720e 0000 0072 1000  ...r....r....r..
-00001760: 0000 a500 0000 7302 0000 0006 027a 1450  ......s......z.P
-00001770: 6167 696e 6174 696f 6e54 6f6b 656e 2e64  aginationToken.d
-00001780: 6174 6163 0100 0000 0000 0000 0000 0000  atac............
-00001790: 0200 0000 0700 0000 4300 0000 7340 0000  ........C...s@..
-000017a0: 007c 006a 0074 016a 026b 0272 0c74 03a0  .|.j.t.j.k.r.t..
-000017b0: 047c 006a 05a1 016e 027c 006a 057d 0174  .|.j...n.|.j.}.t
-000017c0: 06a0 077c 006a 086a 099b 0064 017c 006a  ...|.j.j...d.|.j
-000017d0: 006a 099b 0064 017c 019b 009d 05a1 0153  .j...d.|.......S
-000017e0: 0029 024e 7249 0000 0029 0a72 3a00 0000  .).NrI...).r:...
-000017f0: 7232 0000 0072 3400 0000 7218 0000 00da  r2...r4...r.....
-00001800: 0564 756d 7073 723b 0000 0072 3800 0000  .dumpsr;...r8...
-00001810: 7241 0000 0072 3900 0000 7214 0000 0029  rA...r9...r....)
-00001820: 0272 1f00 0000 7210 0000 0072 0d00 0000  .r....r....r....
-00001830: 720d 0000 0072 0e00 0000 7258 0000 00a9  r....r....rX....
-00001840: 0000 0073 0e00 0000 0c03 0cff 0402 02fd  ...s............
-00001850: 0405 1a01 04ff 7a18 5061 6769 6e61 7469  ......z.Paginati
-00001860: 6f6e 546f 6b65 6e2e 746f 5f74 6f6b 656e  onToken.to_token
-00001870: 4e29 0272 1500 0000 7238 0000 0029 1772  N).r....r8...).r
-00001880: 0800 0000 7209 0000 0072 0a00 0000 7221  ....r....r....r!
-00001890: 0000 0072 3600 0000 720c 0000 0072 3200  ...r6...r....r2.
-000018a0: 0000 7222 0000 0072 2a00 0000 da0c 7374  ..r"...r*.....st
-000018b0: 6174 6963 6d65 7468 6f64 723c 0000 0072  aticmethodr<...r
-000018c0: 2600 0000 7241 0000 0072 4200 0000 da0b  &...rA...rB.....
-000018d0: 636c 6173 736d 6574 686f 6472 2300 0000  classmethodr#...
-000018e0: 7254 0000 0072 5500 0000 7257 0000 0072  rT...rU...rW...r
-000018f0: 5900 0000 da08 7072 6f70 6572 7479 7210  Y.....propertyr.
-00001900: 0000 0072 5800 0000 720d 0000 0072 0d00  ...rX...r....r..
-00001910: 0000 720d 0000 0072 0e00 0000 7238 0000  ..r....r....r8..
-00001920: 0060 0000 0073 3200 0000 0a00 0401 0805  .`...s2.........
-00001930: 0801 0a01 0202 0c01 0205 1401 0206 1401  ................
-00001940: 0206 1a01 0216 0202 02fe 0203 02fd 0404  ................
-00001950: 0afc 080a 0803 0203 1201 1203 7238 0000  ............r8..
-00001960: 0029 1772 3f00 0000 da04 656e 756d 7218  .).r?.....enumr.
-00001970: 0000 0072 2200 0000 7224 0000 00da 1172  ...r"...r$.....r
-00001980: 6f62 6f74 6f2e 6578 6365 7074 696f 6e73  oboto.exceptions
-00001990: 7202 0000 00da 076c 6f67 6769 6e67 7204  r......loggingr.
-000019a0: 0000 0072 4d00 0000 da07 5479 7065 5661  ...rM.....TypeVa
-000019b0: 7272 0500 0000 da09 4261 7365 4d6f 6465  rr......BaseMode
-000019c0: 6cda 0747 656e 6572 6963 7206 0000 0072  l..Genericr....r
-000019d0: 0f00 0000 722b 0000 0072 2d00 0000 7230  ....r+...r-...r0
-000019e0: 0000 00da 0445 6e75 6d72 3200 0000 7236  .....Enumr2...r6
-000019f0: 0000 0072 3800 0000 720d 0000 0072 0d00  ...r8...r....r..
-00001a00: 0000 720d 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
-00001a10: 6f64 756c 653e 0100 0000 7322 0000 0008  odule>....s"....
-00001a20: 0008 0108 0108 0108 020c 020c 0406 020a  ................
-00001a30: 021a 031a 041a 1b1a 091a 0c12 1012 0512  ................
-00001a40: 04                                       .
+00001360: 795e 0100 7d08 0100 7a0f 7407 6a08 6406  y^..}...z.t.j.d.
+00001370: 7c01 9b00 9d02 7c08 6407 8d02 0100 7409  |.....|.d.....t.
+00001380: 6408 8301 6400 8202 6400 7d08 7e08 7701  d...d...d.}.~.w.
+00001390: 7700 2909 4e7a 2249 6e76 616c 6964 2070  w.).Nz"Invalid p
+000013a0: 6167 696e 6174 696f 6e20 746f 6b65 6e20  agination token 
+000013b0: 7363 6865 6d65 2025 737a 1f49 6e76 616c  scheme %sz.Inval
+000013c0: 6964 2070 6167 696e 6174 696f 6e20 746f  id pagination to
+000013d0: 6b65 6e20 7363 6865 6d65 fa01 3a72 0300  ken scheme..:r..
+000013e0: 0000 2901 da08 6d61 7873 706c 6974 7a19  ..)...maxsplitz.
+000013f0: 496e 7661 6c69 6420 7061 6769 6e61 7469  Invalid paginati
+00001400: 6f6e 2074 6f6b 656e 2029 01da 0865 7863  on token )...exc
+00001410: 5f69 6e66 6f7a 1f49 6e76 616c 6964 2070  _infoz.Invalid p
+00001420: 6167 696e 6174 696f 6e20 746f 6b65 6e20  agination token 
+00001430: 666f 726d 6174 2910 7238 0000 0072 3c00  format).r8...r<.
+00001440: 0000 7242 0000 00da 0a73 7461 7274 7377  ..rB.....startsw
+00001450: 6974 6872 3600 0000 7237 0000 0072 1400  ithr6...r7...r..
+00001460: 0000 da06 6c6f 6767 6572 7211 0000 00da  ....loggerr.....
+00001470: 0a56 616c 7565 4572 726f 72da 0573 706c  .ValueError..spl
+00001480: 6974 7232 0000 0072 3400 0000 7218 0000  itr2...r4...r...
+00001490: 0072 1900 0000 721a 0000 0029 0972 1b00  .r....r....).r..
+000014a0: 0000 7248 0000 00da 0764 6563 6f64 6564  ..rH.....decoded
+000014b0: da06 7363 6865 6d65 da08 656e 636f 6469  ..scheme..encodi
+000014c0: 6e67 7210 0000 005a 1770 6167 696e 6174  ngr....Z.paginat
+000014d0: 696f 6e5f 746f 6b65 6e5f 7363 6865 6d65  ion_token_scheme
+000014e0: 5a19 7061 6769 6e61 7469 6f6e 5f74 6f6b  Z.pagination_tok
+000014f0: 656e 5f65 6e63 6f64 696e 67da 0165 720d  en_encoding..er.
+00001500: 0000 0072 0d00 0000 720e 0000 00da 0a66  ...r....r......f
+00001510: 726f 6d5f 746f 6b65 6e7e 0000 0073 2e00  rom_token~...s..
+00001520: 0000 0802 0801 0201 0a01 0e01 0c01 0801  ................
+00001530: 1401 0801 0801 0201 0201 0201 0a02 08ff  ................
+00001540: 06fd 0205 06fb 0e07 1401 0a01 0880 02fe  ................
+00001550: 7a1a 5061 6769 6e61 7469 6f6e 546f 6b65  z.PaginationToke
+00001560: 6e2e 6672 6f6d 5f74 6f6b 656e 7251 0000  n.from_tokenrQ..
+00001570: 0072 5200 0000 6304 0000 0000 0000 0000  .rR...c.........
+00001580: 0000 0004 0000 0002 0000 0043 0000 0073  ...........C...s
+00001590: 1600 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
+000015a0: 7c03 7c00 5f02 6400 5300 7216 0000 0029  |.|._.d.S.r....)
+000015b0: 0372 3900 0000 723a 0000 0072 3b00 0000  .r9...r:...r;...
+000015c0: 2904 721f 0000 0072 5100 0000 7252 0000  ).r....rQ...rR..
+000015d0: 0072 1000 0000 720d 0000 0072 0d00 0000  .r....r....r....
+000015e0: 720e 0000 00da 085f 5f69 6e69 745f 5f95  r......__init__.
+000015f0: 0000 0073 0600 0000 0606 0601 0a01 7a18  ...s..........z.
+00001600: 5061 6769 6e61 7469 6f6e 546f 6b65 6e2e  PaginationToken.
+00001610: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00001620: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00001630: 0073 1600 0000 7c00 6a00 7209 7401 7402  .s....|.j.r.t.t.
+00001640: 7c00 8301 8301 5300 6401 5300 2902 4e72  |.....S.d.S.).Nr
+00001650: 0100 0000 2903 723b 0000 0072 4600 0000  ....).r;...rF...
+00001660: 7226 0000 00a9 0172 1f00 0000 720d 0000  r&.....r....r...
+00001670: 0072 0d00 0000 720e 0000 00da 075f 5f6c  .r....r......__l
+00001680: 656e 5f5f 9f00 0000 7302 0000 0016 017a  en__....s......z
+00001690: 1750 6167 696e 6174 696f 6e54 6f6b 656e  .PaginationToken
+000016a0: 2e5f 5f6c 656e 5f5f 6301 0000 0000 0000  .__len__c.......
+000016b0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+000016c0: 0073 0800 0000 7c00 a000 a100 5300 7216  .s....|.....S.r.
+000016d0: 0000 0029 01da 0874 6f5f 746f 6b65 6e72  ...)...to_tokenr
+000016e0: 5600 0000 720d 0000 0072 0d00 0000 720e  V...r....r....r.
+000016f0: 0000 00da 075f 5f73 7472 5f5f a200 0000  .....__str__....
+00001700: 7302 0000 0008 017a 1750 6167 696e 6174  s......z.Paginat
+00001710: 696f 6e54 6f6b 656e 2e5f 5f73 7472 5f5f  ionToken.__str__
+00001720: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001730: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
+00001740: 6a00 5300 7216 0000 0029 0172 3b00 0000  j.S.r....).r;...
+00001750: 7256 0000 0072 0d00 0000 720d 0000 0072  rV...r....r....r
+00001760: 0e00 0000 7210 0000 00a5 0000 0073 0200  ....r........s..
+00001770: 0000 0602 7a14 5061 6769 6e61 7469 6f6e  ....z.Pagination
+00001780: 546f 6b65 6e2e 6461 7461 6301 0000 0000  Token.datac.....
+00001790: 0000 0000 0000 0002 0000 0007 0000 0043  ...............C
+000017a0: 0000 0073 4000 0000 7c00 6a00 7401 6a02  ...s@...|.j.t.j.
+000017b0: 6b02 720c 7403 a004 7c00 6a05 a101 6e02  k.r.t...|.j...n.
+000017c0: 7c00 6a05 7d01 7406 a007 7c00 6a08 6a09  |.j.}.t...|.j.j.
+000017d0: 9b00 6401 7c00 6a00 6a09 9b00 6401 7c01  ..d.|.j.j...d.|.
+000017e0: 9b00 9d05 a101 5300 2902 4e72 4900 0000  ......S.).NrI...
+000017f0: 290a 723a 0000 0072 3200 0000 7234 0000  ).r:...r2...r4..
+00001800: 0072 1800 0000 da05 6475 6d70 7372 3b00  .r......dumpsr;.
+00001810: 0000 7238 0000 0072 4100 0000 7239 0000  ..r8...rA...r9..
+00001820: 0072 1400 0000 2902 721f 0000 0072 1000  .r....).r....r..
+00001830: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00001840: 0072 5800 0000 a900 0000 730e 0000 000c  .rX.......s.....
+00001850: 030c ff04 0202 fd04 051a 0104 ff7a 1850  .............z.P
+00001860: 6167 696e 6174 696f 6e54 6f6b 656e 2e74  aginationToken.t
+00001870: 6f5f 746f 6b65 6e4e 2902 7215 0000 0072  o_tokenN).r....r
+00001880: 3800 0000 2917 7208 0000 0072 0900 0000  8...).r....r....
+00001890: 720a 0000 0072 2100 0000 7236 0000 0072  r....r!...r6...r
+000018a0: 0c00 0000 7232 0000 0072 2200 0000 722a  ....r2...r"...r*
+000018b0: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
+000018c0: 6472 3c00 0000 7226 0000 0072 4100 0000  dr<...r&...rA...
+000018d0: 7242 0000 00da 0b63 6c61 7373 6d65 7468  rB.....classmeth
+000018e0: 6f64 7223 0000 0072 5400 0000 7255 0000  odr#...rT...rU..
+000018f0: 0072 5700 0000 7259 0000 00da 0870 726f  .rW...rY.....pro
+00001900: 7065 7274 7972 1000 0000 7258 0000 0072  pertyr....rX...r
+00001910: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00001920: 0000 0072 3800 0000 6000 0000 7332 0000  ...r8...`...s2..
+00001930: 000a 0004 0108 0508 010a 0102 020c 0102  ................
+00001940: 0514 0102 0614 0102 061a 0102 1602 0202  ................
+00001950: fe02 0302 fd04 040a fc08 0a08 0302 0312  ................
+00001960: 0112 0372 3800 0000 2917 723f 0000 00da  ...r8...).r?....
+00001970: 0465 6e75 6d72 1800 0000 7222 0000 0072  .enumr....r"...r
+00001980: 2400 0000 da11 726f 626f 746f 2e65 7863  $.....roboto.exc
+00001990: 6570 7469 6f6e 7372 0200 0000 da07 6c6f  eptionsr......lo
+000019a0: 6767 696e 6772 0400 0000 724d 0000 00da  ggingr....rM....
+000019b0: 0754 7970 6556 6172 7205 0000 00da 0942  .TypeVarr......B
+000019c0: 6173 654d 6f64 656c da07 4765 6e65 7269  aseModel..Generi
+000019d0: 6372 0600 0000 720f 0000 0072 2b00 0000  cr....r....r+...
+000019e0: 722d 0000 0072 3000 0000 da04 456e 756d  r-...r0.....Enum
+000019f0: 7232 0000 0072 3600 0000 7238 0000 0072  r2...r6...r8...r
+00001a00: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00001a10: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00001a20: 0073 2200 0000 0800 0801 0801 0801 0802  .s".............
+00001a30: 0c02 0c04 0602 0a02 1a03 1a04 1a1b 1a09  ................
+00001a40: 1a0c 1210 1205 1204                      ........
```

### Comparing `roboto-0.2.8/src/roboto/http/__pycache__/testing_util.cpython-310.pyc` & `roboto-0.2.9/src/roboto/http/__pycache__/testing_util.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1819 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 1b07 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 1b07 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a06 6402 6403 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 4700 6404 6405 8400 6405 8302 5a09  ..G.d.d...d...Z.
 00000070: 6401 5300 2906 e900 0000 004e e901 0000  d.S.)......N....
@@ -86,16 +86,16 @@
 00000550: 037c 005f 007c 0470 0774 0183 007c 005f  .|._.|.p.t...|._
 00000560: 027c 027c 005f 037c 017c 005f 0464 0053  .|.|._.|.|._.d.S
 00000570: 00a9 014e 2905 7207 0000 00da 0464 6963  ...N).r......dic
 00000580: 7472 0500 0000 7206 0000 0072 0800 0000  tr....r....r....
 00000590: 2905 da04 7365 6c66 720a 0000 0072 0b00  )...selfr....r..
 000005a0: 0000 720c 0000 0072 0d00 0000 a900 7212  ..r....r......r.
 000005b0: 0000 00fa e12f 636f 6465 6275 696c 642f  ...../codebuild/
-000005c0: 6f75 7470 7574 2f73 7263 3130 3531 3138  output/src105118
-000005d0: 3230 3839 2f73 7263 2f63 6f64 6573 7461  2089/src/codesta
+000005c0: 6f75 7470 7574 2f73 7263 3330 3739 3233  output/src307923
+000005d0: 3632 3634 2f73 7263 2f63 6f64 6573 7461  6264/src/codesta
 000005e0: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 000005f0: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 00000600: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 00000610: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 00000620: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 00000630: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 00000640: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto-0.2.8/src/roboto/http/constants.py` & `roboto-0.2.9/src/roboto/http/constants.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/http/headers.py` & `roboto-0.2.9/src/roboto/http/headers.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/http/http_client.py` & `roboto-0.2.9/src/roboto/http/http_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -323,14 +323,24 @@
             status_code = exc.code
             if status_code > 399 and status_code < 500:
                 raise ClientError(exc) from None
             elif status_code > 499:
                 raise ServerError(exc) from None
             else:
                 raise HttpError(exc) from None
+        except urllib.error.URLError as exc:
+            if (
+                isinstance(exc.reason, OSError)
+                and exc.reason.errno == errno.ECONNREFUSED
+            ):
+                raise ConnectionRefusedError(
+                    f"Couldn't connect to endpoint {request_ctx.url}"
+                ) from None
+            else:
+                raise
         except Exception:
             raise
 
         raise RuntimeError("Unreachable")
 
     def _wait(self, waiter: RetryWaitFn) -> tenacity.wait.wait_base:
         class Waiter(tenacity.wait.wait_base):
```

### Comparing `roboto-0.2.8/src/roboto/http/request_decorators.py` & `roboto-0.2.9/src/roboto/http/request_decorators.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/http/response.py` & `roboto-0.2.9/src/roboto/http/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                 pagination_token_scheme,
                 pagination_token_encoding,
                 json.loads(data)
                 if pagination_token_encoding == PaginationTokenEncoding.Json
                 else data,
             )
         except Exception as e:
-            logger.error("Invalid pagination token", exc_info=e)
+            logger.error(f"Invalid pagination token {token}", exc_info=e)
             raise ValueError("Invalid pagination token format") from None
 
     def __init__(
         self,
         scheme: PaginationTokenScheme,
         encoding: PaginationTokenEncoding,
         data: typing.Any,
```

### Comparing `roboto-0.2.8/src/roboto/http/testing_util.py` & `roboto-0.2.9/src/roboto/http/testing_util.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/image_registry/__init__.py` & `roboto-0.2.9/src/roboto/image_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/image_registry/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/image_registry/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 951 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 b703 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 b703 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6403 6c0e 6d0f 5a0f 6d10 5a10 0100 6404  d.l.m.Z.m.Z...d.
@@ -39,16 +39,16 @@
 00000260: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
 00000270: 0000 00da 0e69 6d61 6765 5f72 6567 6973  .....image_regis
 00000280: 7472 7972 0900 0000 720a 0000 0072 0b00  tryr....r....r..
 00000290: 0000 720c 0000 0072 0d00 0000 da06 7265  ..r....r......re
 000002a0: 636f 7264 720e 0000 0072 0f00 0000 da07  cordr....r......
 000002b0: 5f5f 616c 6c5f 5fa9 0072 1400 0000 7214  __all__..r....r.
 000002c0: 0000 00fa e72f 636f 6465 6275 696c 642f  ...../codebuild/
-000002d0: 6f75 7470 7574 2f73 7263 3130 3531 3138  output/src105118
-000002e0: 3230 3839 2f73 7263 2f63 6f64 6573 7461  2089/src/codesta
+000002d0: 6f75 7470 7574 2f73 7263 3330 3739 3233  output/src307923
+000002e0: 3632 3634 2f73 7263 2f63 6f64 6573 7461  6264/src/codesta
 000002f0: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 00000300: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 00000310: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 00000320: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 00000330: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 00000340: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 00000350: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto-0.2.8/src/roboto/image_registry/__pycache__/http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/image_registry/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 913 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 9103 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 9103 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 4700 6404 6405 8400  e.j...Z.G.d.d...
 00000050: 6405 6500 6a01 8303 5a03 4700 6406 6407  d.e.j...Z.G.d.d.
 00000060: 8400 6407 6500 6a01 8303 5a04 4700 6408  ..d.e.j...Z.G.d.
 00000070: 6409 8400 6409 6500 6a01 8303 5a05 4700  d...d.e.j...Z.G.
@@ -21,16 +21,16 @@
 00000140: 7265 6769 7374 7279 5f75 726c da09 696d  registry_url..im
 00000150: 6167 655f 7572 694e a905 da08 5f5f 6e61  age_uriN....__na
 00000160: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000170: da0c 5f5f 7175 616c 6e61 6d65 5f5f da03  ..__qualname__..
 00000180: 7374 72da 0f5f 5f61 6e6e 6f74 6174 696f  str..__annotatio
 00000190: 6e73 5f5f a900 720c 0000 0072 0c00 0000  ns__..r....r....
 000001a0: faed 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-000001b0: 7075 742f 7372 6331 3035 3131 3832 3038  put/src105118208
-000001c0: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+000001b0: 7075 742f 7372 6333 3037 3932 3336 3236  put/src307923626
+000001c0: 342f 7372 632f 636f 6465 7374 6172 2d63  4/src/codestar-c
 000001d0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 000001e0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 000001f0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 00000200: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 00000210: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 00000220: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000230: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto-0.2.8/src/roboto/image_registry/__pycache__/image_registry.cpython-310.pyc` & `roboto-0.2.9/src/roboto/image_registry/__pycache__/image_registry.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 9136 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 b023 0000  o........Y.e.#..
+00000000: 6f0d 0d0a 0000 0000 3248 a865 b023 0000  o.......2H.e.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ea00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6402 6403 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6402 6404 6c08 6d09 5a09 0100 6402  ..d.d.l.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
@@ -47,15 +47,15 @@
 000002e0: 6578 7069 7261 7469 6f6e da06 7265 7475  expiration..retu
 000002f0: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
 00000300: 0000 0002 0000 0043 0000 0073 0c00 0000  .......C...s....
 00000310: 7400 8300 7c00 6a01 6b05 5300 a901 4e29  t...|.j.k.S...N)
 00000320: 0272 0a00 0000 7215 0000 00a9 01da 0473  .r....r........s
 00000330: 656c 66a9 0072 1a00 0000 faed 2f63 6f64  elf..r....../cod
 00000340: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000350: 6331 3035 3131 3832 3038 392f 7372 632f  c1051182089/src/
+00000350: 6333 3037 3932 3336 3236 342f 7372 632f  c3079236264/src/
 00000360: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000370: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000380: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000390: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 000003a0: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 000003b0: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 000003c0: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto-0.2.8/src/roboto/image_registry/http_resources.py` & `roboto-0.2.9/src/roboto/image_registry/http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/image_registry/image_registry.py` & `roboto-0.2.9/src/roboto/image_registry/image_registry.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/notifications/__pycache__/http_client.cpython-310.pyc` & `roboto-0.2.9/src/roboto/notifications/__pycache__/http_client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1929 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 8907 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 8907 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6406 6407 8400 6407 8302 5a09  ..G.d.d...d...Z.
 00000070: 6408 5300 2909 e900 0000 0029 02da 0341  d.S.)......)...A
@@ -30,15 +30,15 @@
 000001d0: 0000 0200 0000 0200 0000 0300 0000 7314  ..............s.
 000001e0: 0000 0074 0083 00a0 01a1 0001 007c 017c  ...t.........|.|
 000001f0: 005f 0264 0053 0029 014e 2903 da05 7375  ._.d.S.).N)...su
 00000200: 7065 72da 085f 5f69 6e69 745f 5f72 0900  per..__init__r..
 00000210: 0000 2902 da04 7365 6c66 720a 0000 00a9  ..)...selfr.....
 00000220: 01da 095f 5f63 6c61 7373 5f5f a900 fae9  ...__class__....
 00000230: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000240: 742f 7372 6331 3035 3131 3832 3038 392f  t/src1051182089/
+00000240: 742f 7372 6333 3037 3932 3336 3236 342f  t/src3079236264/
 00000250: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000260: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000270: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000280: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000290: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 000002a0: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000002b0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto-0.2.8/src/roboto/notifications/__pycache__/notifications.cpython-310.pyc` & `roboto-0.2.9/src/roboto/notifications/__pycache__/notifications.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 444 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 bc01 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 bc01 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 4700 6404  ..d.e.e...Z.G.d.
 00000050: 6405 8400 6405 6502 6501 8304 5a04 6406  d...d.e.e...Z.d.
 00000060: 5300 2907 e900 0000 0029 01da 0445 6e75  S.)......)...Enu
 00000070: 6d63 0000 0000 0000 0000 0000 0000 0000  mc..............
@@ -11,16 +11,16 @@
 000000a0: 03da 104e 6f74 6966 6963 6174 696f 6e54  ...NotificationT
 000000b0: 7970 655a 0f63 6f6d 6d65 6e74 5f6d 656e  ypeZ.comment_men
 000000c0: 7469 6f6e 4e29 04da 085f 5f6e 616d 655f  tionN)...__name_
 000000d0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 000000e0: 5f71 7561 6c6e 616d 655f 5f5a 0e43 6f6d  _qualname__Z.Com
 000000f0: 6d65 6e74 4d65 6e74 696f 6ea9 0072 0800  mentMention..r..
 00000100: 0000 7208 0000 00fa eb2f 636f 6465 6275  ..r....../codebu
-00000110: 696c 642f 6f75 7470 7574 2f73 7263 3130  ild/output/src10
-00000120: 3531 3138 3230 3839 2f73 7263 2f63 6f64  51182089/src/cod
+00000110: 696c 642f 6f75 7470 7574 2f73 7263 3330  ild/output/src30
+00000120: 3739 3233 3632 3634 2f73 7263 2f63 6f64  79236264/src/cod
 00000130: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 00000140: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 00000150: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 00000160: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 00000170: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 00000180: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 00000190: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto-0.2.8/src/roboto/notifications/http_client.py` & `roboto-0.2.9/src/roboto/notifications/http_client.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/profile/__pycache__/profile.cpython-310.pyc` & `roboto-0.2.9/src/roboto/profile/__pycache__/profile.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3730 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 920e 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 920e 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 6d06 5a06 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6401 6c07 5a07 6403 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6509 8300 5a0a 6405 5a0b 6406 5a0c  ..e...Z.d.Z.d.Z.
@@ -36,16 +36,16 @@
 00000230: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 00000240: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
 00000250: 696f 6e73 5f5f da0d 5052 4f44 5f45 4e44  ions__..PROD_END
 00000260: 504f 494e 5472 0b00 0000 da18 5052 4f44  POINTr......PROD
 00000270: 5f55 5345 525f 504f 4f4c 5f43 4c49 454e  _USER_POOL_CLIEN
 00000280: 545f 4944 720c 0000 00a9 0072 1400 0000  T_IDr......r....
 00000290: 7214 0000 00fa df2f 636f 6465 6275 696c  r....../codebuil
-000002a0: 642f 6f75 7470 7574 2f73 7263 3130 3531  d/output/src1051
-000002b0: 3138 3230 3839 2f73 7263 2f63 6f64 6573  182089/src/codes
+000002a0: 642f 6f75 7470 7574 2f73 7263 3330 3739  d/output/src3079
+000002b0: 3233 3632 3634 2f73 7263 2f63 6f64 6573  236264/src/codes
 000002c0: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 000002d0: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 000002e0: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 000002f0: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 00000300: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 00000310: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 00000320: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto-0.2.8/src/roboto/profile/profile.py` & `roboto-0.2.9/src/roboto/profile/profile.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/pydantic/__pycache__/serializers.cpython-310.pyc` & `roboto-0.2.9/src/roboto/pydantic/__pycache__/serializers.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 524 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 0c02 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 0c02 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6403 6504 6505  d.l.m.Z...d.e.e.
 00000050: 6501 6a06 6602 1900 6404 6503 6604 6405  e.j.f...d.e.f.d.
 00000060: 6406 8404 5a07 6401 5300 2907 e900 0000  d...Z.d.S.).....
 00000070: 004e 2901 da0c 5573 6572 4d65 7461 6461  .N)...UserMetada
@@ -20,16 +20,16 @@
 00000130: 6b65 7920 277a 0927 2c20 2074 7970 6520  key 'z.',  type 
 00000140: 2909 da05 6974 656d 73da 0474 7970 65da  )...items..type.
 00000150: 0462 6f6f 6cda 0369 6e74 da05 666c 6f61  .bool..int..floa
 00000160: 74da 0373 7472 da07 6465 6369 6d61 6cda  t..str..decimal.
 00000170: 0744 6563 696d 616c da0a 5661 6c75 6545  .Decimal..ValueE
 00000180: 7272 6f72 2903 7203 0000 00da 016b da01  rror).r......k..
 00000190: 76a9 0072 1000 0000 fae4 2f63 6f64 6562  v..r....../codeb
-000001a0: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-000001b0: 3035 3131 3832 3038 392f 7372 632f 636f  051182089/src/co
+000001a0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+000001b0: 3037 3932 3336 3236 342f 7372 632f 636f  079236264/src/co
 000001c0: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 000001d0: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 000001e0: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 000001f0: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000200: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000210: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000220: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto-0.2.8/src/roboto/pydantic/__pycache__/validators.cpython-310.pyc` & `roboto-0.2.9/src/roboto/pydantic/__pycache__/validators.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1869 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4d07 0000  o........Y.eM...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 4d07 0000  o.......2H.eM...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6502 6403 6501 6a03 6404 6502 6606 6405  e.d.e.j.d.e.f.d.
 00000050: 6406 8404 5a04 6407 6505 6506 1900 6404  d...Z.d.e.e...d.
 00000060: 6505 6506 1900 6604 6408 6409 8404 5a07  e.e...f.d.d...Z.
 00000070: 6401 5300 290a e900 0000 004e da04 6461  d.S.)......N..da
@@ -73,15 +73,15 @@
 00000480: 6473 da03 6765 74da 0a69 7369 6e73 7461  ds..get..isinsta
 00000490: 6e63 65da 0a61 6e6e 6f74 6174 696f 6eda  nce..annotation.
 000004a0: 0574 7970 6573 da09 556e 696f 6e54 7970  .types..UnionTyp
 000004b0: 65da 0474 7970 65da 085f 5f61 7267 735f  e..type..__args_
 000004c0: 5f29 02da 0a66 6965 6c64 5f6e 616d 65da  _)...field_name.
 000004d0: 0566 6965 6c64 2901 7203 0000 00a9 00fa  .field).r.......
 000004e0: e32f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000004f0: 7574 2f73 7263 3130 3531 3138 3230 3839  ut/src1051182089
+000004f0: 7574 2f73 7263 3330 3739 3233 3632 3634  ut/src3079236264
 00000500: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 00000510: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000520: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000530: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000540: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000550: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000560: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto-0.2.8/src/roboto/pydantic/serializers.py` & `roboto-0.2.9/src/roboto/pydantic/serializers.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/pydantic/validators.py` & `roboto-0.2.9/src/roboto/pydantic/validators.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/query/__init__.py` & `roboto-0.2.9/src/roboto/query/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/query/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/query/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 543 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 1f02 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 1f02 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 6d0d 5a0d 0100 6405 5a0e 6406 5300 2907  m.Z...d.Z.d.S.).
@@ -25,15 +25,15 @@
 00000180: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
 00000190: 0000 5a09 7072 6563 616e 6e65 6472 0700  ..Z.precannedr..
 000001a0: 0000 da05 7175 6572 7972 0800 0000 7209  ....queryr....r.
 000001b0: 0000 00da 0776 6973 6974 6f72 720a 0000  .....visitorr...
 000001c0: 0072 0b00 0000 da07 5f5f 616c 6c5f 5fa9  .r......__all__.
 000001d0: 0072 1000 0000 7210 0000 00fa de2f 636f  .r....r....../co
 000001e0: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-000001f0: 7263 3130 3531 3138 3230 3839 2f73 7263  rc1051182089/src
+000001f0: 7263 3330 3739 3233 3632 3634 2f73 7263  rc3079236264/src
 00000200: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
 00000210: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
 00000220: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
 00000230: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
 00000240: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
 00000250: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
 00000260: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
```

### Comparing `roboto-0.2.8/src/roboto/query/__pycache__/conditions.cpython-310.pyc` & `roboto-0.2.9/src/roboto/query/__pycache__/conditions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 4516 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 a411 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 a411 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6402  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 6d08 5a08 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000070: 8400 6405 6509 6503 6a0a 8304 5a0b 4700  ..d.e.e.j...Z.G.
@@ -46,16 +46,16 @@
 000002d0: da08 436f 6e74 6169 6e73 da0b 4e6f 7443  ..Contains..NotC
 000002e0: 6f6e 7461 696e 73da 0649 734e 756c 6cda  ontains..IsNull.
 000002f0: 0949 734e 6f74 4e75 6c6c da06 4578 6973  .IsNotNull..Exis
 00000300: 7473 da09 4e6f 7445 7869 7374 73da 0a42  ts..NotExists..B
 00000310: 6567 696e 7357 6974 685a 044c 696b 655a  eginsWithZ.LikeZ
 00000320: 074e 6f74 4c69 6b65 a900 7217 0000 0072  .NotLike..r....r
 00000330: 1700 0000 fae0 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000340: 2f6f 7574 7075 742f 7372 6331 3035 3131  /output/src10511
-00000350: 3832 3038 392f 7372 632f 636f 6465 7374  82089/src/codest
+00000340: 2f6f 7574 7075 742f 7372 6333 3037 3932  /output/src30792
+00000350: 3336 3236 342f 7372 632f 636f 6465 7374  36264/src/codest
 00000360: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000370: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000380: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000390: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000003a0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000003b0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000003c0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto-0.2.8/src/roboto/query/__pycache__/precanned.cpython-310.pyc` & `roboto-0.2.9/src/roboto/query/__pycache__/precanned.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1671 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 8706 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 8706 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6404 6508 6405 6508 6604  m.Z...d.e.d.e.f.
 00000060: 6406 6407 8404 5a09 6408 6501 650a 6508  d.d...Z.d.e.e.e.
 00000070: 1900 1900 6409 6501 650a 6508 1900 1900  ....d.e.e.e.....
@@ -18,16 +18,16 @@
 00000110: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
 00000120: 0000 0073 1c00 0000 7c00 a000 6401 6402  ...s....|...d.d.
 00000130: a102 a000 6403 6402 a102 a000 6404 6402  ....d.d.....d.d.
 00000140: a102 5300 2905 4e7a 042a 2a2f 2afa 0125  ..S.).Nz.**/*..%
 00000150: 7a02 2a2a da01 2a29 01da 0772 6570 6c61  z.**..*)...repla
 00000160: 6365 a901 7209 0000 00a9 0072 0f00 0000  ce..r......r....
 00000170: fadf 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-00000180: 7075 742f 7372 6331 3035 3131 3832 3038  put/src105118208
-00000190: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+00000180: 7075 742f 7372 6333 3037 3932 3336 3236  put/src307923626
+00000190: 342f 7372 632f 636f 6465 7374 6172 2d63  4/src/codestar-c
 000001a0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 000001b0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 000001c0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 000001d0: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 000001e0: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 000001f0: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000200: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto-0.2.8/src/roboto/query/__pycache__/query.cpython-310.pyc` & `roboto-0.2.9/src/roboto/query/__pycache__/query.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3861 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 150f 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 150f 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6403 6404 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6507 6500  ..G.d.d...d.e.e.
 00000070: 6a08 8304 5a09 4700 6407 6408 8400 6408  j...Z.G.d.d...d.
@@ -20,16 +20,16 @@
 00000130: 6620 6120 7175 6572 792e da03 4153 435a  f a query...ASCZ
 00000140: 0444 4553 434e 2906 da08 5f5f 6e61 6d65  .DESCN)...__name
 00000150: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
 00000160: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
 00000170: 646f 635f 5f5a 0941 7363 656e 6469 6e67  doc__Z.Ascending
 00000180: 5a0a 4465 7363 656e 6469 6e67 a900 720c  Z.Descending..r.
 00000190: 0000 0072 0c00 0000 fadb 2f63 6f64 6562  ...r....../codeb
-000001a0: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-000001b0: 3035 3131 3832 3038 392f 7372 632f 636f  051182089/src/co
+000001a0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+000001b0: 3037 3932 3336 3236 342f 7372 632f 636f  079236264/src/co
 000001c0: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 000001d0: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 000001e0: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 000001f0: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000200: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000210: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000220: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto-0.2.8/src/roboto/query/__pycache__/visitor.cpython-310.pyc` & `roboto-0.2.9/src/roboto/query/__pycache__/visitor.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1394 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 7205 0000  o........Y.er...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 7205 0000  o.......2H.er...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6500 6a06  ..G.d.d...d.e.j.
 00000060: 8303 5a07 4700 6406 6407 8400 6407 6507  ..Z.G.d.d...d.e.
 00000070: 8303 5a08 6401 5300 2908 e900 0000 004e  ..Z.d.S.)......N
@@ -30,15 +30,15 @@
 000001d0: 616e 6365 7203 0000 00da 0f76 6973 6974  ancer......visit
 000001e0: 5f63 6f6e 6469 7469 6f6e 7204 0000 00da  _conditionr.....
 000001f0: 1576 6973 6974 5f63 6f6e 6469 7469 6f6e  .visit_condition
 00000200: 5f67 726f 7570 da0a 5661 6c75 6545 7272  _group..ValueErr
 00000210: 6f72 da04 7479 7065 2902 da04 7365 6c66  or..type)...self
 00000220: 7207 0000 00a9 0072 0f00 0000 fadd 2f63  r......r....../c
 00000230: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000240: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+00000240: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 00000250: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 00000260: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 00000270: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 00000280: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 00000290: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 000002a0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 000002b0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/query/conditions.py` & `roboto-0.2.9/src/roboto/query/conditions.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/query/precanned.py` & `roboto-0.2.9/src/roboto/query/precanned.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/query/query.py` & `roboto-0.2.9/src/roboto/query/query.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/query/visitor.py` & `roboto-0.2.9/src/roboto/query/visitor.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/sentinels.py` & `roboto-0.2.9/src/roboto/sentinels.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/serde/__init__.py` & `roboto-0.2.9/src/roboto/serde/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/serde/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/serde/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 734 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 de02 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 de02 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6401 6404 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6700 6405 a201  m.Z.m.Z...g.d...
 00000070: 5a0c 6406 5300 2907 7ab3 0a53 6572 4465  Z.d.S.).z..SerDe
@@ -34,15 +34,15 @@
 00000210: da07 5f5f 646f 635f 5f5a 0661 7272 6179  ..__doc__Z.array
 00000220: 7372 0200 0000 da05 6469 6374 7372 0300  sr......dictsr..
 00000230: 0000 7204 0000 0072 0500 0000 7206 0000  ..r....r....r...
 00000240: 0072 0700 0000 da05 7061 7468 7372 0800  .r......pathsr..
 00000250: 0000 7209 0000 00da 075f 5f61 6c6c 5f5f  ..r......__all__
 00000260: a900 720e 0000 0072 0e00 0000 fade 2f63  ..r....r....../c
 00000270: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000280: 7372 6331 3035 3131 3832 3038 392f 7372  src1051182089/sr
+00000280: 7372 6333 3037 3932 3336 3236 342f 7372  src3079236264/sr
 00000290: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 000002a0: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 000002b0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 000002c0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 000002d0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 000002e0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 000002f0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto-0.2.8/src/roboto/serde/__pycache__/dicts.cpython-310.pyc` & `roboto-0.2.9/src/roboto/serde/__pycache__/dicts.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1713 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 b106 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 b106 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 d200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 0902  d.l.Z.d.d.l.Z...
 00000050: 6415 6403 6505 6503 6a06 6503 6a06 6602  d.d.e.e.j.e.j.f.
 00000060: 1900 6404 6507 6503 6a06 1900 6405 6508  ..d.e.e.j...d.e.
 00000070: 6406 6503 6a06 6608 6407 6408 8405 5a09  d.e.j.f.d.d...Z.
@@ -26,15 +26,15 @@
 00000190: 2401 0064 0053 0071 047c 0353 00a9 014e  $..d.S.q.|.S...N
 000001a0: 2904 da04 7479 7065 da04 6469 6374 da14  )...type..dict..
 000001b0: 6361 7365 5f69 6e73 656e 7369 7469 7665  case_insensitive
 000001c0: 5f67 6574 da03 6765 7429 0572 0200 0000  _get..get).r....
 000001d0: 7203 0000 0072 0400 0000 da05 7661 6c75  r....r......valu
 000001e0: 65da 036b 6579 a900 720d 0000 00fa db2f  e..key..r....../
 000001f0: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000200: 2f73 7263 3130 3531 3138 3230 3839 2f73  /src1051182089/s
+00000200: 2f73 7263 3330 3739 3233 3632 3634 2f73  /src3079236264/s
 00000210: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000220: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000230: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000240: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000250: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000260: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000270: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto-0.2.8/src/roboto/serde/__pycache__/paths.cpython-310.pyc` & `roboto-0.2.9/src/roboto/serde/__pycache__/paths.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 801 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 2103 0000  o........Y.e!...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 2103 0000  o.......2H.e!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6403 6503 6504 1900 6404 6502 6a05  Z.d.e.e...d.e.j.
 00000050: 6604 6405 6406 8404 5a06 6407 6501 6503  f.d.d...Z.d.e.e.
 00000060: 6504 1900 1900 6408 6501 6503 6504 1900  e.....d.e.e.e...
 00000070: 1900 6409 6504 6404 6507 6608 640a 640b  ..d.e.d.e.f.d.d.
@@ -14,15 +14,15 @@
 000000d0: 006a 036a 047c 00a1 0253 0029 014e 2905  .j.j.|...S.).N).
 000000e0: da08 7061 7468 7370 6563 da08 5061 7468  ..pathspec..Path
 000000f0: 5370 6563 5a0a 6672 6f6d 5f6c 696e 6573  SpecZ.from_lines
 00000100: da08 7061 7474 6572 6e73 5a13 4769 7457  ..patternsZ.GitW
 00000110: 696c 644d 6174 6368 5061 7474 6572 6e29  ildMatchPattern)
 00000120: 0172 0300 0000 a900 7208 0000 00fa db2f  .r......r....../
 00000130: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000140: 2f73 7263 3130 3531 3138 3230 3839 2f73  /src1051182089/s
+00000140: 2f73 7263 3330 3739 3233 3632 3634 2f73  /src3079236264/s
 00000150: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000160: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000170: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000180: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000190: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 000001a0: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 000001b0: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto-0.2.8/src/roboto/serde/dicts.py` & `roboto-0.2.9/src/roboto/serde/dicts.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/serde/paths.py` & `roboto-0.2.9/src/roboto/serde/paths.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/transactions/__init__.py` & `roboto-0.2.9/src/roboto/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/transactions/__pycache__/__init__.cpython-310.pyc` & `roboto-0.2.9/src/roboto/transactions/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 558 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 2e02 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 2e02 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6405  ..d.d.l.m.Z...d.
 00000070: 5a0c 6406 5300 2907 e901 0000 0029 02da  Z.d.S.)......)..
@@ -24,16 +24,16 @@
 00000170: 7372 0200 0000 7203 0000 005a 0b6d 616e  sr....r....Z.man
 00000180: 6167 6572 5f61 6263 7204 0000 00da 0672  ager_abcr......r
 00000190: 6563 6f72 6472 0500 0000 7206 0000 0072  ecordr....r....r
 000001a0: 0700 0000 7208 0000 00da 1374 7261 6e73  ....r......trans
 000001b0: 6163 7469 6f6e 5f6d 616e 6167 6572 7209  action_managerr.
 000001c0: 0000 00da 075f 5f61 6c6c 5f5f a900 720e  .....__all__..r.
 000001d0: 0000 0072 0e00 0000 fae5 2f63 6f64 6562  ...r....../codeb
-000001e0: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-000001f0: 3035 3131 3832 3038 392f 7372 632f 636f  051182089/src/co
+000001e0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+000001f0: 3037 3932 3336 3236 342f 7372 632f 636f  079236264/src/co
 00000200: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 00000210: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000220: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000230: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000240: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000250: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000260: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto-0.2.8/src/roboto/transactions/__pycache__/http_resources.cpython-310.pyc` & `roboto-0.2.9/src/roboto/transactions/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 318 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 3e01 0000  o........Y.e>...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 3e01 0000  o.......2H.e>...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 6501 6a04 8303 5a05 4700 6406  ..d.e.j...Z.G.d.
 00000060: 6407 8400 6407 6501 6a04 8303 5a06 6401  d...d.e.j...Z.d.
 00000070: 5300 2908 e900 0000 004e e901 0000 0029  S.)......N.....)
@@ -21,15 +21,15 @@
 00000140: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 00000150: 7175 616c 6e61 6d65 5f5f 7203 0000 00da  qualname__r.....
 00000160: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
 00000170: da03 7374 7272 0700 0000 da06 7479 7069  ..strr......typi
 00000180: 6e67 da08 4f70 7469 6f6e 616c da03 696e  ng..Optional..in
 00000190: 74a9 0072 1000 0000 7210 0000 00fa eb2f  t..r....r....../
 000001a0: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-000001b0: 2f73 7263 3130 3531 3138 3230 3839 2f73  /src1051182089/s
+000001b0: 2f73 7263 3330 3739 3233 3632 3634 2f73  /src3079236264/s
 000001c0: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 000001d0: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 000001e0: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 000001f0: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000200: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000210: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000220: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto-0.2.8/src/roboto/transactions/__pycache__/manager_abc.cpython-310.pyc` & `roboto-0.2.9/src/roboto/transactions/__pycache__/manager_abc.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1043 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 1304 0000  o........Y.e....
+00000000: 6f0d 0d0a 0000 0000 3248 a865 1304 0000  o.......2H.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 0100 4700  d.l.m.Z.m.Z...G.
 00000050: 6404 6405 8400 6405 6500 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6401 5300 2906 e900 0000 004e e901 0000  d.S.)......N....
 00000070: 0029 02da 1154 7261 6e73 6163 7469 6f6e  .)...Transaction
@@ -33,15 +33,15 @@
 00000200: 2902 4eda 1162 6567 696e 5f74 7261 6e73  ).N..begin_trans
 00000210: 6163 7469 6f6e a901 da13 4e6f 7449 6d70  action....NotImp
 00000220: 6c65 6d65 6e74 6564 4572 726f 7229 07da  lementedError)..
 00000230: 0473 656c 6672 0600 0000 7207 0000 0072  .selfr....r....r
 00000240: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
 00000250: 0000 00a9 0072 1200 0000 fae8 2f63 6f64  .....r....../cod
 00000260: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000270: 6331 3035 3131 3832 3038 392f 7372 632f  c1051182089/src/
+00000270: 6333 3037 3932 3336 3236 342f 7372 632f  c3079236264/src/
 00000280: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000290: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 000002a0: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 000002b0: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 000002c0: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 000002d0: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 000002e0: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto-0.2.8/src/roboto/transactions/__pycache__/record.cpython-310.pyc` & `roboto-0.2.9/src/roboto/transactions/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 1099 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 4b04 0000  o........Y.eK...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 4b04 0000  o.......2H.eK...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6402 6403 8400 6403 6504 6501 6a05 8304  d.d...d.e.e.j...
 00000060: 5a06 4700 6404 6405 8400 6405 6504 6501  Z.G.d.d...d.e.e.
 00000070: 6a05 8304 5a07 4700 6406 6407 8400 6407  j...Z.G.d.d...d.
@@ -14,16 +14,16 @@
 000000d0: 6402 5300 2903 da0f 5472 616e 7361 6374  d.S.)...Transact
 000000e0: 696f 6e54 7970 655a 0b66 696c 655f 7570  ionTypeZ.file_up
 000000f0: 6c6f 6164 4e29 04da 085f 5f6e 616d 655f  loadN)...__name_
 00000100: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000110: 5f71 7561 6c6e 616d 655f 5fda 0a46 696c  _qualname__..Fil
 00000120: 6555 706c 6f61 64a9 0072 0700 0000 7207  eUpload..r....r.
 00000130: 0000 00fa e32f 636f 6465 6275 696c 642f  ...../codebuild/
-00000140: 6f75 7470 7574 2f73 7263 3130 3531 3138  output/src105118
-00000150: 3230 3839 2f73 7263 2f63 6f64 6573 7461  2089/src/codesta
+00000140: 6f75 7470 7574 2f73 7263 3330 3739 3233  output/src307923
+00000150: 3632 3634 2f73 7263 2f63 6f64 6573 7461  6264/src/codesta
 00000160: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 00000170: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 00000180: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 00000190: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 000001a0: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 000001b0: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 000001c0: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto-0.2.8/src/roboto/transactions/__pycache__/transaction_manager.cpython-310.pyc` & `roboto-0.2.9/src/roboto/transactions/__pycache__/transaction_manager.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jan 11 21:12:42 2024 UTC, .py size: 3198 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ca59 a065 7e0c 0000  o........Y.e~...
+00000000: 6f0d 0d0a 0000 0000 3248 a865 7e0c 0000  o.......2H.e~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6402 6404 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6405 6406 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6405 6407 6c09 6d0a 5a0a 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6408 6c0b 6d0c 5a0c 6d0d 5a0d 0100 4700  d.l.m.Z.m.Z...G.
@@ -45,15 +45,15 @@
 000002c0: 0672 6574 7572 6e4e 6303 0000 0000 0000  .returnNc.......
 000002d0: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
 000002e0: 0073 1000 0000 7c02 7c00 5f00 7c01 7c00  .s....|.|._.|.|.
 000002f0: 5f01 6400 5300 2901 4e29 0272 0d00 0000  _.d.S.).N).r....
 00000300: 720e 0000 0029 03da 0473 656c 6672 0f00  r....)...selfr..
 00000310: 0000 7210 0000 00a9 0072 1300 0000 faf0  ..r......r......
 00000320: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000330: 742f 7372 6331 3035 3131 3832 3038 392f  t/src1051182089/
+00000330: 742f 7372 6333 3037 3932 3336 3236 342f  t/src3079236264/
 00000340: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000350: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000360: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000370: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000380: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000390: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000003a0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto-0.2.8/src/roboto/transactions/manager_abc.py` & `roboto-0.2.9/src/roboto/transactions/manager_abc.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/transactions/record.py` & `roboto-0.2.9/src/roboto/transactions/record.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/transactions/transaction_manager.py` & `roboto-0.2.9/src/roboto/transactions/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/updates.py` & `roboto-0.2.9/src/roboto/updates.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/src/roboto/waiters.py` & `roboto-0.2.9/src/roboto/waiters.py`

 * *Files identical despite different names*

### Comparing `roboto-0.2.8/PKG-INFO` & `roboto-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tools for interacting with roboto.ai
 License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

