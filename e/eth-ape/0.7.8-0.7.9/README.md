# Comparing `tmp/eth-ape-0.7.8.tar.gz` & `tmp/eth-ape-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-ape-0.7.8.tar", last modified: Mon Feb 12 16:58:29 2024, max compression
+gzip compressed data, was "eth-ape-0.7.9.tar", last modified: Fri Feb 16 18:36:13 2024, max compression
```

## Comparing `eth-ape-0.7.8.tar` & `eth-ape-0.7.9.tar`

### file list

```diff
@@ -1,505 +1,505 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.019879 eth-ape-0.7.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.023879 eth-ape-0.7.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.023879 eth-ape-0.7.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-12 16:57:30.000000 eth-ape-0.7.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-02-12 16:57:30.000000 eth-ape-0.7.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-02-12 16:57:30.000000 eth-ape-0.7.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-02-12 16:57:30.000000 eth-ape-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-02-12 16:58:29.087879 eth-ape-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-02-12 16:57:30.000000 eth-ape-0.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-02-12 16:57:30.000000 eth-ape-0.7.8/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-12 16:57:30.000000 eth-ape-0.7.8/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-12 16:57:30.000000 eth-ape-0.7.8/codeql-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-12 16:57:30.000000 eth-ape-0.7.8/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.023879 eth-ape-0.7.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.023879 eth-ape-0.7.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.023879 eth-ape-0.7.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.023879 eth-ape-0.7.8/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/commands/accounts.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/commands/compile.rst
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/commands/console.rst
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/commands/init.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/commands/networks.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/commands/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/commands/pm.rst
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/commands/test.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.027879 eth-ape-0.7.8/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/methoddocs/ape.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/methoddocs/ape_accounts.md
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/methoddocs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/methoddocs/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/methoddocs/contracts.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/methoddocs/managers.md
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/methoddocs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/methoddocs/types.md
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.031879 eth-ape-0.7.8/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/accounts.md
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/clis.md
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/compile.md
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/config.md
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/console.md
--rw-r--r--   0 runner    (1001) docker     (127)    15143 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/contracts.md
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/data.md
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/dependencies.md
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/developing_plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/forking_networks.md
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/installing_plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-02-12 16:57:30.000000 eth-ape-0.7.8/docs/userguides/logging.md
--rw-r--r--   0 runner    (1001) docker     (127)    21467 2024-02-12 16:57:31.000000 eth-ape-0.7.8/docs/userguides/networks.md
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-02-12 16:57:31.000000 eth-ape-0.7.8/docs/userguides/projects.md
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-02-12 16:57:31.000000 eth-ape-0.7.8/docs/userguides/proxy.md
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-02-12 16:57:31.000000 eth-ape-0.7.8/docs/userguides/publishing.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-12 16:57:31.000000 eth-ape-0.7.8/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-02-12 16:57:31.000000 eth-ape-0.7.8/docs/userguides/scripts.md
--rw-r--r--   0 runner    (1001) docker     (127)    24402 2024-02-12 16:57:31.000000 eth-ape-0.7.8/docs/userguides/testing.md
--rw-r--r--   0 runner    (1001) docker     (127)    20438 2024-02-12 16:57:31.000000 eth-ape-0.7.8/docs/userguides/transactions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-02-12 16:57:31.000000 eth-ape-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-12 16:57:31.000000 eth-ape-0.7.8/recommended-plugins.txt
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-12 16:58:29.087879 eth-ape-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-02-12 16:57:31.000000 eth-ape-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.011879 eth-ape-0.7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.031879 eth-ape-0.7.8/src/ape/
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/__modules__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.031879 eth-ape-0.7.8/src/ape/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21114 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/explorers.py
--rw-r--r--   0 runner    (1001) docker     (127)    42700 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    24000 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    37100 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/api/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.035879 eth-ape-0.7.8/src/ape/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    14037 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/cli/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    15315 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/cli/paramtype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.035879 eth-ape-0.7.8/src/ape/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54839 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/contracts/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24678 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/harambe.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.035879 eth-ape-0.7.8/src/ape/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13084 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    60131 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/compilers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    24833 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.035879 eth-ape-0.7.8/src/ape/managers/project/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/project/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)    30887 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/project/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/project/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/managers/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.039879 eth-ape-0.7.8/src/ape/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21574 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/plugins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/plugins/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/plugins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/plugins/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/plugins/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/plugins/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/plugins/pluggy_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/plugins/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/plugins/query.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.039879 eth-ape-0.7.8/src/ape/pytest/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/pytest/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/pytest/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/pytest/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/pytest/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/pytest/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/pytest/gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/pytest/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/pytest/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.039879 eth-ape-0.7.8/src/ape/types/
--rw-r--r--   0 runner    (1001) docker     (127)    15819 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/types/address.py
--rw-r--r--   0 runner    (1001) docker     (127)    36424 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/types/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/types/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)    23239 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/types/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.043879 eth-ape-0.7.8/src/ape/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/utils/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/utils/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/utils/github.py
--rw-r--r--   0 runner    (1001) docker     (127)    15158 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/utils/os.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-12 16:58:28.000000 eth-ape-0.7.8/src/ape/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.043879 eth-ape-0.7.8/src/ape_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_accounts/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_accounts/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.043879 eth-ape-0.7.8/src/ape_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_cache/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_cache/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    17961 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_cache/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.043879 eth-ape-0.7.8/src/ape_compile/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_compile/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_compile/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.043879 eth-ape-0.7.8/src/ape_console/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_console/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_console/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_console/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.047879 eth-ape-0.7.8/src/ape_ethereum/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    44155 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/ecosystem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.047879 eth-ape-0.7.8/src/ape_ethereum/multicall/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/multicall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/multicall/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/multicall/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/multicall/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    53190 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15268 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_ethereum/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.047879 eth-ape-0.7.8/src/ape_geth/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_geth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_geth/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_geth/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_geth/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.047879 eth-ape-0.7.8/src/ape_init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_init/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.047879 eth-ape-0.7.8/src/ape_networks/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_networks/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.047879 eth-ape-0.7.8/src/ape_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_plugins/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_plugins/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.047879 eth-ape-0.7.8/src/ape_pm/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_pm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_pm/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_pm/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_pm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.047879 eth-ape-0.7.8/src/ape_run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_run/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_run/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.051879 eth-ape-0.7.8/src/ape_test/
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_test/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_test/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_test/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/src/ape_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.051879 eth-ape-0.7.8/src/eth_ape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-02-12 16:58:28.000000 eth-ape-0.7.8/src/eth_ape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-02-12 16:58:28.000000 eth-ape-0.7.8/src/eth_ape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 16:58:28.000000 eth-ape-0.7.8/src/eth_ape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-12 16:58:28.000000 eth-ape-0.7.8/src/eth_ape.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 16:58:28.000000 eth-ape-0.7.8/src/eth_ape.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-02-12 16:58:28.000000 eth-ape-0.7.8/src/eth_ape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-12 16:58:28.000000 eth-ape-0.7.8/src/eth_ape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.051879 eth-ape-0.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.059879 eth-ape-0.7.8/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26353 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.059879 eth-ape-0.7.8/tests/functional/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/conversion/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/conversion/test_encode_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/conversion/test_ether.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/conversion/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/conversion/test_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.059879 eth-ape-0.7.8/tests/functional/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.011879 eth-ape-0.7.8/tests/functional/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.011879 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.059879 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/abi/
--rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/abi/contract_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.063879 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (127)    26703 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/BeaconProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    77599 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/ContractA.json
--rw-r--r--   0 runner    (1001) docker     (127)    75147 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/ContractB.json
--rw-r--r--   0 runner    (1001) docker     (127)    32313 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/ContractC.json
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/DsNoteTest.json
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/HasError.json
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/Interface.json
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json
--rw-r--r--   0 runner    (1001) docker     (127)    46986 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/RevertsContract.json
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/SolFallbackAndReceive.json
--rw-r--r--   0 runner    (1001) docker     (127)   240439 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/SubReverts.json
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/VyDefault.json
--rw-r--r--   0 runner    (1001) docker     (127)   251475 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/VyperContract.json
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/VyperFactory.json
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/beacon.json
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/eip1967.json
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/proxy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.011879 eth-ape-0.7.8/tests/functional/data/manifests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.011879 eth-ape-0.7.8/tests/functional/data/manifests/OpenZeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.063879 eth-ape-0.7.8/tests/functional/data/manifests/OpenZeppelin/v3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)  1689272 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/manifests/OpenZeppelin/v3.1.0/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.067879 eth-ape-0.7.8/tests/functional/data/manifests/OpenZeppelin/v4.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)  3230874 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/manifests/OpenZeppelin/v4.4.2/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.015879 eth-ape-0.7.8/tests/functional/data/projects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.071879 eth-ape-0.7.8/tests/functional/data/projects/ApeProject/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/projects/ApeProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.071879 eth-ape-0.7.8/tests/functional/data/projects/ApeProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/projects/ApeProject/contracts/ApeContract0.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/projects/ApeProject/contracts/ApeContract1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/projects/ApeProject/contracts/Contract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.071879 eth-ape-0.7.8/tests/functional/data/projects/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/projects/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.071879 eth-ape-0.7.8/tests/functional/data/projects/BrownieProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/projects/BrownieProject/contracts/brownie.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.015879 eth-ape-0.7.8/tests/functional/data/projects/LongContractsFolder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.015879 eth-ape-0.7.8/tests/functional/data/projects/LongContractsFolder/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.071879 eth-ape-0.7.8/tests/functional/data/projects/LongContractsFolder/source/v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/projects/LongContractsFolder/source/v0.1/long_contracts_folder.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.071879 eth-ape-0.7.8/tests/functional/data/python/
--rw-r--r--   0 runner    (1001) docker     (127)    37472 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.075879 eth-ape-0.7.8/tests/functional/data/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/ContractA.sol
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/ContractB.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/ContractC.sol
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/Proxy.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/RevertsContract.vy
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/SolFallbackAndReceive.sol
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/SolidityContract.sol
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/SubRevertsVy.vy
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/VyDefault.vy
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/VyperContract.vy
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/VyperFactory.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.075879 eth-ape-0.7.8/tests/functional/data/sources/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/data/sources/interfaces/ISubReverts.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.075879 eth-ape-0.7.8/tests/functional/geth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/geth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/geth/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/geth/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/geth/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/geth/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/geth/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/geth/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/geth/text_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    31931 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_block_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    22203 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_compilers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_contract_call_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_contract_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_contract_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    33167 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_contract_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_contract_method_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_contracts_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_default_sender_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    54312 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_network_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_network_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    23943 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_receipt_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_reverts_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.075879 eth-ape-0.7.8/tests/functional/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/utils/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/utils/test_basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/utils/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/utils/test_os.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/functional/utils/test_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.075879 eth-ape-0.7.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.015879 eth-ape-0.7.8/tests/integration/cli/projects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.015879 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/contracts/Contract.test
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/contracts/Contract2.foo
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/contracts/doc.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/contracts/file_without_ext
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/contracts/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/contracts/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/contracts/subdir/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/contracts/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/bad-contracts/contracts/tests/TestContract.foobar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/projects/empty-config/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/empty-config/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/projects/geth/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/geth/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/projects/geth/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/geth/contracts/TokenA.json
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/geth/contracts/TokenB.json
--rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/geth/contracts/VyperContract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/projects/geth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/geth/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/geth/tests/test_using_local_geth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.015879 eth-ape-0.7.8/tests/integration/cli/projects/multiple-interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/projects/multiple-interfaces/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/multiple-interfaces/contracts/Interface-with-hyphens.json
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.exclude.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/multiple-interfaces/contracts/InterfaceWithNumber123.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/multiple-interfaces/contracts/Interface_with_underscores.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/projects/no-config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/no-config/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.079879 eth-ape-0.7.8/tests/integration/cli/projects/only-dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/only-dependencies/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.083879 eth-ape-0.7.8/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/importme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.083879 eth-ape-0.7.8/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/DependencyInProjectOnly.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.015879 eth-ape-0.7.8/tests/integration/cli/projects/only-script-subdirs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.015879 eth-ape-0.7.8/tests/integration/cli/projects/only-script-subdirs/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.083879 eth-ape-0.7.8/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_click_print.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_main_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.015879 eth-ape-0.7.8/tests/integration/cli/projects/script/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.083879 eth-ape-0.7.8/tests/integration/cli/projects/script/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/contracts/VyperContract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.083879 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/click.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/error_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/error_forgot_click.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/error_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/error_no_def.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/output_contract_view_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.083879 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_click_print.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_main_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.083879 eth-ape-0.7.8/tests/integration/cli/projects/test/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/test/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.083879 eth-ape-0.7.8/tests/integration/cli/projects/test/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/test/tests/test_fixture_isolation.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/test/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/test/tests/test_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.083879 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/ContractA.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/Exclude.json
--rw-r--r--   0 runner    (1001) docker     (127)    41634 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json
--rw-r--r--   0 runner    (1001) docker     (127)    64327 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/exclude_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/exclude_dir/UnwantedContract.json
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/hyphen-Contract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.015879 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/dep/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/dep/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)    64326 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/dep/contracts/RawVyperOutputDep.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/scripts/txerr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/containing_sub_dependencies.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.019879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/sub-dependency.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/contracts/Other.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/contracts/Project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.019879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/default/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/default/contracts/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/default/contracts/hyphen-DependencyContract.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/manifest_dependency.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.019879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.019879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.019879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/renamed_complex_contracts_folder.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.019879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/renamed_contracts_folder.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 16:58:29.087879 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/renamed_contracts_folder_specified_in_config.json
--rw-r--r--   0 runner    (1001) docker     (127)    12564 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_pm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/test_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-02-12 16:57:31.000000 eth-ape-0.7.8/tests/integration/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.702334 eth-ape-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.634333 eth-ape-0.7.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.638333 eth-ape-0.7.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.638333 eth-ape-0.7.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-16 18:35:07.000000 eth-ape-0.7.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-02-16 18:35:07.000000 eth-ape-0.7.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-02-16 18:35:07.000000 eth-ape-0.7.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-02-16 18:35:07.000000 eth-ape-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-02-16 18:36:13.702334 eth-ape-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-02-16 18:35:07.000000 eth-ape-0.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-02-16 18:35:07.000000 eth-ape-0.7.9/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-16 18:35:07.000000 eth-ape-0.7.9/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-16 18:35:07.000000 eth-ape-0.7.9/codeql-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-16 18:35:07.000000 eth-ape-0.7.9/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.638333 eth-ape-0.7.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.638333 eth-ape-0.7.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.638333 eth-ape-0.7.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.638333 eth-ape-0.7.9/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/commands/accounts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/commands/compile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/commands/console.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/commands/init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/commands/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/commands/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/commands/pm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/commands/test.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.642333 eth-ape-0.7.9/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/methoddocs/ape.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/methoddocs/ape_accounts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/methoddocs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/methoddocs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/methoddocs/contracts.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/methoddocs/managers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/methoddocs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/methoddocs/types.md
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.642333 eth-ape-0.7.9/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/accounts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/clis.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/compile.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/console.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15143 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/contracts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/data.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/dependencies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/developing_plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/forking_networks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/installing_plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/logging.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21467 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/networks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/projects.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/proxy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/publishing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/scripts.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24402 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/testing.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20438 2024-02-16 18:35:07.000000 eth-ape-0.7.9/docs/userguides/transactions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-02-16 18:35:07.000000 eth-ape-0.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-16 18:35:07.000000 eth-ape-0.7.9/recommended-plugins.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-16 18:36:13.702334 eth-ape-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-02-16 18:35:07.000000 eth-ape-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.626333 eth-ape-0.7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.646334 eth-ape-0.7.9/src/ape/
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/__modules__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.646334 eth-ape-0.7.9/src/ape/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21114 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/explorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42700 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24000 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37100 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/api/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.646334 eth-ape-0.7.9/src/ape/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14037 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/cli/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15315 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/cli/paramtype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.650334 eth-ape-0.7.9/src/ape/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54839 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/contracts/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24678 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/harambe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.650334 eth-ape-0.7.9/src/ape/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13084 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60131 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/compilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24833 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.650334 eth-ape-0.7.9/src/ape/managers/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/project/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30887 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/project/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/project/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/managers/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.650334 eth-ape-0.7.9/src/ape/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21574 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/plugins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/plugins/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/plugins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/plugins/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/plugins/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/plugins/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/plugins/pluggy_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/plugins/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/plugins/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.654333 eth-ape-0.7.9/src/ape/pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/pytest/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/pytest/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/pytest/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/pytest/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/pytest/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/pytest/gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/pytest/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/pytest/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.654333 eth-ape-0.7.9/src/ape/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    15819 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36424 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/types/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/types/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23239 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/types/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.654333 eth-ape-0.7.9/src/ape/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/utils/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/utils/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/utils/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15158 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/utils/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-16 18:36:13.000000 eth-ape-0.7.9/src/ape/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.654333 eth-ape-0.7.9/src/ape_accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_accounts/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_accounts/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.658334 eth-ape-0.7.9/src/ape_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_cache/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_cache/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17961 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_cache/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.658334 eth-ape-0.7.9/src/ape_compile/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_compile/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_compile/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.658334 eth-ape-0.7.9/src/ape_console/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_console/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_console/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_console/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.658334 eth-ape-0.7.9/src/ape_ethereum/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45099 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/ecosystem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.658334 eth-ape-0.7.9/src/ape_ethereum/multicall/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/multicall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/multicall/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/multicall/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/multicall/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53222 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16208 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_ethereum/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.658334 eth-ape-0.7.9/src/ape_geth/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_geth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_geth/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_geth/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_geth/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.658334 eth-ape-0.7.9/src/ape_init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_init/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.662334 eth-ape-0.7.9/src/ape_networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_networks/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.662334 eth-ape-0.7.9/src/ape_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_plugins/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_plugins/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.662334 eth-ape-0.7.9/src/ape_pm/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_pm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_pm/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_pm/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_pm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.662334 eth-ape-0.7.9/src/ape_run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_run/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_run/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.662334 eth-ape-0.7.9/src/ape_test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_test/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_test/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_test/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/src/ape_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.662334 eth-ape-0.7.9/src/eth_ape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-02-16 18:36:13.000000 eth-ape-0.7.9/src/eth_ape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-02-16 18:36:13.000000 eth-ape-0.7.9/src/eth_ape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 18:36:13.000000 eth-ape-0.7.9/src/eth_ape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-16 18:36:13.000000 eth-ape-0.7.9/src/eth_ape.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 18:36:13.000000 eth-ape-0.7.9/src/eth_ape.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-02-16 18:36:13.000000 eth-ape-0.7.9/src/eth_ape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-16 18:36:13.000000 eth-ape-0.7.9/src/eth_ape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.662334 eth-ape-0.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.670334 eth-ape-0.7.9/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26353 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.670334 eth-ape-0.7.9/tests/functional/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/conversion/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/conversion/test_encode_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/conversion/test_ether.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/conversion/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/conversion/test_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.670334 eth-ape-0.7.9/tests/functional/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.626333 eth-ape-0.7.9/tests/functional/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.626333 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.670334 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/abi/
+-rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/abi/contract_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.674334 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (127)    26703 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/BeaconProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    77599 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/ContractA.json
+-rw-r--r--   0 runner    (1001) docker     (127)    75147 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/ContractB.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32313 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/ContractC.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/DsNoteTest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/HasError.json
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/Interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46986 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/RevertsContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/SolFallbackAndReceive.json
+-rw-r--r--   0 runner    (1001) docker     (127)   240439 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/SubReverts.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/VyDefault.json
+-rw-r--r--   0 runner    (1001) docker     (127)   251475 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/VyperContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/VyperFactory.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/beacon.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/eip1967.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/proxy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.626333 eth-ape-0.7.9/tests/functional/data/manifests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.626333 eth-ape-0.7.9/tests/functional/data/manifests/OpenZeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.674334 eth-ape-0.7.9/tests/functional/data/manifests/OpenZeppelin/v3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)  1689272 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/manifests/OpenZeppelin/v3.1.0/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.678334 eth-ape-0.7.9/tests/functional/data/manifests/OpenZeppelin/v4.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)  3230874 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/manifests/OpenZeppelin/v4.4.2/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.630333 eth-ape-0.7.9/tests/functional/data/projects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.682334 eth-ape-0.7.9/tests/functional/data/projects/ApeProject/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/projects/ApeProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.682334 eth-ape-0.7.9/tests/functional/data/projects/ApeProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/projects/ApeProject/contracts/ApeContract0.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/projects/ApeProject/contracts/ApeContract1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/projects/ApeProject/contracts/Contract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.682334 eth-ape-0.7.9/tests/functional/data/projects/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/projects/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.682334 eth-ape-0.7.9/tests/functional/data/projects/BrownieProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/projects/BrownieProject/contracts/brownie.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.630333 eth-ape-0.7.9/tests/functional/data/projects/LongContractsFolder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.630333 eth-ape-0.7.9/tests/functional/data/projects/LongContractsFolder/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.682334 eth-ape-0.7.9/tests/functional/data/projects/LongContractsFolder/source/v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/projects/LongContractsFolder/source/v0.1/long_contracts_folder.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.682334 eth-ape-0.7.9/tests/functional/data/python/
+-rw-r--r--   0 runner    (1001) docker     (127)    37472 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.686334 eth-ape-0.7.9/tests/functional/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/ContractA.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/ContractB.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/ContractC.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/Proxy.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/RevertsContract.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/SolFallbackAndReceive.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/SolidityContract.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/SubRevertsVy.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/VyDefault.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/VyperContract.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/VyperFactory.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.686334 eth-ape-0.7.9/tests/functional/data/sources/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/data/sources/interfaces/ISubReverts.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.686334 eth-ape-0.7.9/tests/functional/geth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/geth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/geth/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/geth/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/geth/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/geth/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/geth/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/geth/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/geth/text_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31931 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_block_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22203 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_compilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_contract_call_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_contract_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_contract_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33167 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_contract_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_contract_method_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_contracts_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_default_sender_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57926 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_network_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23943 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_receipt_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_reverts_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.686334 eth-ape-0.7.9/tests/functional/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/utils/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/utils/test_basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/utils/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/utils/test_os.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/functional/utils/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.686334 eth-ape-0.7.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.690334 eth-ape-0.7.9/tests/integration/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.634333 eth-ape-0.7.9/tests/integration/cli/projects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.630333 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.690334 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/contracts/Contract.test
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/contracts/Contract2.foo
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/contracts/doc.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/contracts/file_without_ext
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/contracts/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.690334 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/contracts/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/contracts/subdir/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.690334 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/contracts/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/bad-contracts/contracts/tests/TestContract.foobar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.690334 eth-ape-0.7.9/tests/integration/cli/projects/empty-config/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/empty-config/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.690334 eth-ape-0.7.9/tests/integration/cli/projects/geth/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/geth/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.690334 eth-ape-0.7.9/tests/integration/cli/projects/geth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/geth/contracts/TokenA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/geth/contracts/TokenB.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/geth/contracts/VyperContract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.690334 eth-ape-0.7.9/tests/integration/cli/projects/geth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/geth/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/geth/tests/test_using_local_geth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.630333 eth-ape-0.7.9/tests/integration/cli/projects/multiple-interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.694334 eth-ape-0.7.9/tests/integration/cli/projects/multiple-interfaces/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/multiple-interfaces/contracts/Interface-with-hyphens.json
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.exclude.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/multiple-interfaces/contracts/InterfaceWithNumber123.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/multiple-interfaces/contracts/Interface_with_underscores.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.694334 eth-ape-0.7.9/tests/integration/cli/projects/no-config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/no-config/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.694334 eth-ape-0.7.9/tests/integration/cli/projects/only-dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/only-dependencies/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.694334 eth-ape-0.7.9/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/importme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.694334 eth-ape-0.7.9/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/DependencyInProjectOnly.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.630333 eth-ape-0.7.9/tests/integration/cli/projects/only-script-subdirs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.630333 eth-ape-0.7.9/tests/integration/cli/projects/only-script-subdirs/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.694334 eth-ape-0.7.9/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_click_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_main_print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.630333 eth-ape-0.7.9/tests/integration/cli/projects/script/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.694334 eth-ape-0.7.9/tests/integration/cli/projects/script/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/contracts/VyperContract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.694334 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/error_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/error_forgot_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/error_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/error_no_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/output_contract_view_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.694334 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_click_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_main_print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.694334 eth-ape-0.7.9/tests/integration/cli/projects/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/test/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/test/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/test/tests/test_fixture_isolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/test/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/test/tests/test_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/ContractA.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/Exclude.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41634 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json
+-rw-r--r--   0 runner    (1001) docker     (127)    64327 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/exclude_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/exclude_dir/UnwantedContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/hyphen-Contract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.630333 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/dep/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/dep/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)    64326 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/dep/contracts/RawVyperOutputDep.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/scripts/txerr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/containing_sub_dependencies.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.634333 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/sub-dependency.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/contracts/Other.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/contracts/Project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.634333 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/default/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/default/contracts/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/default/contracts/hyphen-DependencyContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/manifest_dependency.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.634333 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.634333 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.634333 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/renamed_complex_contracts_folder.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.634333 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.698334 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/renamed_contracts_folder.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.702334 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:13.702334 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/renamed_contracts_folder_specified_in_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12564 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_pm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-02-16 18:35:07.000000 eth-ape-0.7.9/tests/integration/cli/utils.py
```

### Comparing `eth-ape-0.7.8/.github/ISSUE_TEMPLATE/bug.md` & `eth-ape-0.7.9/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/ISSUE_TEMPLATE/feature.md` & `eth-ape-0.7.9/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/ISSUE_TEMPLATE/work-item.md` & `eth-ape-0.7.9/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/PULL_REQUEST_TEMPLATE.md` & `eth-ape-0.7.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/release-drafter.yml` & `eth-ape-0.7.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/workflows/codeql.yml` & `eth-ape-0.7.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/workflows/commitlint.yaml` & `eth-ape-0.7.9/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/workflows/docs.yaml` & `eth-ape-0.7.9/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/workflows/prtitle.yaml` & `eth-ape-0.7.9/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/workflows/publish.yaml` & `eth-ape-0.7.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/workflows/stale-prs.yml` & `eth-ape-0.7.9/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.github/workflows/test.yaml` & `eth-ape-0.7.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.gitignore` & `eth-ape-0.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/.pre-commit-config.yaml` & `eth-ape-0.7.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/CONTRIBUTING.md` & `eth-ape-0.7.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/Dockerfile` & `eth-ape-0.7.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/LICENSE` & `eth-ape-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/PKG-INFO` & `eth-ape-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-ape
-Version: 0.7.8
+Version: 0.7.9
 Summary: Ape Ethereum Framework
 Home-page: https://apeworx.io
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Project-URL: Documentation, https://docs.apeworx.io/ape/
 Project-URL: Funding, https://gitcoin.co/grants/5958/ape-maintenance-fund
```

### Comparing `eth-ape-0.7.8/README.md` & `eth-ape-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/SECURITY.md` & `eth-ape-0.7.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/build_docs.py` & `eth-ape-0.7.9/build_docs.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/_static/custom.css` & `eth-ape-0.7.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/_static/custom.js` & `eth-ape-0.7.9/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/_templates/layout.html` & `eth-ape-0.7.9/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/conf.py` & `eth-ape-0.7.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/favicon.ico` & `eth-ape-0.7.9/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/index.md` & `eth-ape-0.7.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/logo.gif` & `eth-ape-0.7.9/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/methoddocs/api.md` & `eth-ape-0.7.9/docs/methoddocs/api.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/methoddocs/cli.md` & `eth-ape-0.7.9/docs/methoddocs/cli.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/methoddocs/contracts.md` & `eth-ape-0.7.9/docs/methoddocs/contracts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/methoddocs/managers.md` & `eth-ape-0.7.9/docs/methoddocs/managers.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/methoddocs/plugins.md` & `eth-ape-0.7.9/docs/methoddocs/plugins.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/methoddocs/types.md` & `eth-ape-0.7.9/docs/methoddocs/types.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/accounts.md` & `eth-ape-0.7.9/docs/userguides/accounts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/clis.md` & `eth-ape-0.7.9/docs/userguides/clis.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/compile.md` & `eth-ape-0.7.9/docs/userguides/compile.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/config.md` & `eth-ape-0.7.9/docs/userguides/config.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/console.md` & `eth-ape-0.7.9/docs/userguides/console.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/contracts.md` & `eth-ape-0.7.9/docs/userguides/contracts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/data.md` & `eth-ape-0.7.9/docs/userguides/data.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/dependencies.md` & `eth-ape-0.7.9/docs/userguides/dependencies.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/developing_plugins.md` & `eth-ape-0.7.9/docs/userguides/developing_plugins.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/forking_networks.md` & `eth-ape-0.7.9/docs/userguides/forking_networks.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/installing_plugins.md` & `eth-ape-0.7.9/docs/userguides/installing_plugins.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/logging.md` & `eth-ape-0.7.9/docs/userguides/logging.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/networks.md` & `eth-ape-0.7.9/docs/userguides/networks.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/projects.md` & `eth-ape-0.7.9/docs/userguides/projects.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/proxy.md` & `eth-ape-0.7.9/docs/userguides/proxy.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/publishing.md` & `eth-ape-0.7.9/docs/userguides/publishing.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/scripts.md` & `eth-ape-0.7.9/docs/userguides/scripts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/testing.md` & `eth-ape-0.7.9/docs/userguides/testing.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/docs/userguides/transactions.md` & `eth-ape-0.7.9/docs/userguides/transactions.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/pyproject.toml` & `eth-ape-0.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/setup.py` & `eth-ape-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/__init__.py` & `eth-ape-0.7.9/src/ape/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/_cli.py` & `eth-ape-0.7.9/src/ape/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/__init__.py` & `eth-ape-0.7.9/src/ape/api/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/accounts.py` & `eth-ape-0.7.9/src/ape/api/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/address.py` & `eth-ape-0.7.9/src/ape/api/address.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/compiler.py` & `eth-ape-0.7.9/src/ape/api/compiler.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/config.py` & `eth-ape-0.7.9/src/ape/api/config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/convert.py` & `eth-ape-0.7.9/src/ape/api/convert.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/explorers.py` & `eth-ape-0.7.9/src/ape/api/explorers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/networks.py` & `eth-ape-0.7.9/src/ape/api/networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/projects.py` & `eth-ape-0.7.9/src/ape/api/projects.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/providers.py` & `eth-ape-0.7.9/src/ape/api/providers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/query.py` & `eth-ape-0.7.9/src/ape/api/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/api/transactions.py` & `eth-ape-0.7.9/src/ape/api/transactions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/cli/__init__.py` & `eth-ape-0.7.9/src/ape/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/cli/arguments.py` & `eth-ape-0.7.9/src/ape/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/cli/choices.py` & `eth-ape-0.7.9/src/ape/cli/choices.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/cli/commands.py` & `eth-ape-0.7.9/src/ape/cli/commands.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/cli/options.py` & `eth-ape-0.7.9/src/ape/cli/options.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/cli/paramtype.py` & `eth-ape-0.7.9/src/ape/cli/paramtype.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/contracts/base.py` & `eth-ape-0.7.9/src/ape/contracts/base.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/exceptions.py` & `eth-ape-0.7.9/src/ape/exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/logging.py` & `eth-ape-0.7.9/src/ape/logging.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/__init__.py` & `eth-ape-0.7.9/src/ape/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/accounts.py` & `eth-ape-0.7.9/src/ape/managers/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/base.py` & `eth-ape-0.7.9/src/ape/managers/base.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/chain.py` & `eth-ape-0.7.9/src/ape/managers/chain.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/compilers.py` & `eth-ape-0.7.9/src/ape/managers/compilers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/config.py` & `eth-ape-0.7.9/src/ape/managers/config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/converters.py` & `eth-ape-0.7.9/src/ape/managers/converters.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/networks.py` & `eth-ape-0.7.9/src/ape/managers/networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/project/dependency.py` & `eth-ape-0.7.9/src/ape/managers/project/dependency.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/project/manager.py` & `eth-ape-0.7.9/src/ape/managers/project/manager.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/project/types.py` & `eth-ape-0.7.9/src/ape/managers/project/types.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/managers/query.py` & `eth-ape-0.7.9/src/ape/managers/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/plugins/__init__.py` & `eth-ape-0.7.9/src/ape/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/plugins/_utils.py` & `eth-ape-0.7.9/src/ape/plugins/_utils.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/plugins/account.py` & `eth-ape-0.7.9/src/ape/plugins/account.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/plugins/compiler.py` & `eth-ape-0.7.9/src/ape/plugins/compiler.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/plugins/config.py` & `eth-ape-0.7.9/src/ape/plugins/config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/plugins/converter.py` & `eth-ape-0.7.9/src/ape/plugins/converter.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/plugins/network.py` & `eth-ape-0.7.9/src/ape/plugins/network.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/plugins/pluggy_patch.py` & `eth-ape-0.7.9/src/ape/plugins/pluggy_patch.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/plugins/project.py` & `eth-ape-0.7.9/src/ape/plugins/project.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/plugins/query.py` & `eth-ape-0.7.9/src/ape/plugins/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/pytest/README.md` & `eth-ape-0.7.9/src/ape/pytest/README.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/pytest/config.py` & `eth-ape-0.7.9/src/ape/pytest/config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/pytest/contextmanagers.py` & `eth-ape-0.7.9/src/ape/pytest/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/pytest/coverage.py` & `eth-ape-0.7.9/src/ape/pytest/coverage.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/pytest/fixtures.py` & `eth-ape-0.7.9/src/ape/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/pytest/gas.py` & `eth-ape-0.7.9/src/ape/pytest/gas.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/pytest/plugin.py` & `eth-ape-0.7.9/src/ape/pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/pytest/runners.py` & `eth-ape-0.7.9/src/ape/pytest/runners.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/types/__init__.py` & `eth-ape-0.7.9/src/ape/types/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/types/address.py` & `eth-ape-0.7.9/src/ape/types/address.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/types/coverage.py` & `eth-ape-0.7.9/src/ape/types/coverage.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/types/signatures.py` & `eth-ape-0.7.9/src/ape/types/signatures.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/types/trace.py` & `eth-ape-0.7.9/src/ape/types/trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/utils/__init__.py` & `eth-ape-0.7.9/src/ape/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/utils/abi.py` & `eth-ape-0.7.9/src/ape/utils/abi.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/utils/basemodel.py` & `eth-ape-0.7.9/src/ape/utils/basemodel.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/utils/github.py` & `eth-ape-0.7.9/src/ape/utils/github.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/utils/misc.py` & `eth-ape-0.7.9/src/ape/utils/misc.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/utils/os.py` & `eth-ape-0.7.9/src/ape/utils/os.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/utils/process.py` & `eth-ape-0.7.9/src/ape/utils/process.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/utils/testing.py` & `eth-ape-0.7.9/src/ape/utils/testing.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/utils/trace.py` & `eth-ape-0.7.9/src/ape/utils/trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape/utils/validators.py` & `eth-ape-0.7.9/src/ape/utils/validators.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_accounts/_cli.py` & `eth-ape-0.7.9/src/ape_accounts/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_accounts/accounts.py` & `eth-ape-0.7.9/src/ape_accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_cache/_cli.py` & `eth-ape-0.7.9/src/ape_cache/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_cache/models.py` & `eth-ape-0.7.9/src/ape_cache/models.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_cache/query.py` & `eth-ape-0.7.9/src/ape_cache/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_compile/__init__.py` & `eth-ape-0.7.9/src/ape_compile/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_compile/_cli.py` & `eth-ape-0.7.9/src/ape_compile/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_console/_cli.py` & `eth-ape-0.7.9/src/ape_console/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_console/plugin.py` & `eth-ape-0.7.9/src/ape_console/plugin.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_ethereum/__init__.py` & `eth-ape-0.7.9/src/ape_ethereum/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_ethereum/_converters.py` & `eth-ape-0.7.9/src/ape_ethereum/_converters.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_ethereum/ecosystem.py` & `eth-ape-0.7.9/src/ape_ethereum/ecosystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     ProxyType,
 )
 from ape_ethereum.transactions import (
     AccessListTransaction,
     BaseTransaction,
     DynamicFeeTransaction,
     Receipt,
+    SharedBlobReceipt,
+    SharedBlobTransaction,
     StaticFeeTransaction,
     TransactionStatusEnum,
     TransactionType,
 )
 
 NETWORKS = {
     # chain_id, network_id
@@ -476,15 +478,15 @@
             except (ApeException, ValueError):
                 pass
 
         return None
 
     def decode_receipt(self, data: Dict) -> ReceiptAPI:
         status = data.get("status")
-        if status:
+        if status is not None:
             status = self.conversion_manager.convert(status, int)
             status = TransactionStatusEnum(status)
 
         txn_hash = None
         hash_key_choices = ("hash", "txHash", "txnHash", "transactionHash", "transaction_hash")
         for choice in hash_key_choices:
             if choice in data:
@@ -501,26 +503,38 @@
         elif "input" in data and isinstance(data["input"], str):
             data["input"] = HexBytes(data["input"])
 
         block_number = data.get("block_number", data.get("blockNumber"))
         if block_number is None:
             raise ValueError("Missing block number.")
 
-        receipt = Receipt(
+        receipt_kwargs = dict(
             block_number=block_number,
             contract_address=data.get("contract_address") or data.get("contractAddress"),
             gas_limit=data.get("gas", data.get("gas_limit", data.get("gasLimit"))) or 0,
             gas_price=data.get("gas_price", data.get("gasPrice")) or 0,
             gas_used=data.get("gas_used", data.get("gasUsed")) or 0,
             logs=data.get("logs", []),
             status=status,
             txn_hash=txn_hash,
             transaction=self.create_transaction(**data),
         )
-        return receipt
+
+        receipt_cls: Type[Receipt]
+        if any(
+            x in data
+            for x in ("blobGasPrice", "blobGasUsed", "blobVersionedHashes", "maxFeePerBlobGas")
+        ):
+            receipt_cls = SharedBlobReceipt
+            receipt_kwargs["blob_gas_price"] = data.get("blob_gas_price", data.get("blobGasPrice"))
+            receipt_kwargs["blob_gas_used"] = data.get("blob_gas_used", data.get("blobGasUsed"))
+        else:
+            receipt_cls = Receipt
+
+        return receipt_cls.model_validate(receipt_kwargs)
 
     def decode_block(self, data: Dict) -> BlockAPI:
         data["hash"] = HexBytes(data["hash"]) if data.get("hash") else None
         if "gas_limit" in data:
             data["gasLimit"] = data.pop("gas_limit")
         if "gas_used" in data:
             data["gasUsed"] = data.pop("gas_used")
@@ -764,29 +778,32 @@
         tx_data = _correct_key("gas", tx_data, ("gas_limit", "gasLimit"))
         tx_data = _correct_key("gas_price", tx_data, ("gasPrice",))
         tx_data = _correct_key(
             "type",
             tx_data,
             ("txType", "tx_type", "txnType", "txn_type", "transactionType", "transaction_type"),
         )
+        tx_data = _correct_key("maxFeePerBlobGas", tx_data, ("max_fee_per_blob_gas",))
+        tx_data = _correct_key("blobVersionedHashes", tx_data, ("blob_versioned_hashes",))
 
         # Handle unique value specifications, such as "1 ether".
         if "value" in tx_data and not isinstance(tx_data["value"], int):
             value = tx_data["value"] or 0  # Convert None to 0.
             tx_data["value"] = self.conversion_manager.convert(value, int)
 
         # None is not allowed, the user likely means `b""`.
         if "data" in tx_data and tx_data["data"] is None:
             tx_data["data"] = b""
 
         # Deduce the transaction type.
         transaction_types: Dict[TransactionType, Type[TransactionAPI]] = {
             TransactionType.STATIC: StaticFeeTransaction,
-            TransactionType.DYNAMIC: DynamicFeeTransaction,
             TransactionType.ACCESS_LIST: AccessListTransaction,
+            TransactionType.DYNAMIC: DynamicFeeTransaction,
+            TransactionType.SHARED_BLOB: SharedBlobTransaction,
         }
         if "type" in tx_data:
             # May be None in data.
             if tx_data["type"] is None:
                 # Explicit `None` means used default.
                 version = self.default_transaction_type
             elif isinstance(tx_data["type"], TransactionType):
@@ -799,14 +816,16 @@
 
         elif "gas_price" in tx_data:
             version = TransactionType.STATIC
         elif "max_fee" in tx_data or "max_priority_fee" in tx_data:
             version = TransactionType.DYNAMIC
         elif "access_list" in tx_data or "accessList" in tx_data:
             version = TransactionType.ACCESS_LIST
+        elif "maxFeePerBlobGas" in tx_data or "blobVersionedHashes" in tx_data:
+            version = TransactionType.SHARED_BLOB
         else:
             version = self.default_transaction_type
 
         tx_data["type"] = version.value
 
         # This causes problems in pydantic for some reason.
         # NOTE: This must happen after deducing the tx type!
```

### Comparing `eth-ape-0.7.8/src/ape_ethereum/multicall/constants.py` & `eth-ape-0.7.9/src/ape_ethereum/multicall/constants.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_ethereum/multicall/exceptions.py` & `eth-ape-0.7.9/src/ape_ethereum/multicall/exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_ethereum/multicall/handlers.py` & `eth-ape-0.7.9/src/ape_ethereum/multicall/handlers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_ethereum/provider.py` & `eth-ape-0.7.9/src/ape_ethereum/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -826,15 +826,16 @@
         txn_type = TransactionType(txn.type)
         if (
             txn_type in (TransactionType.STATIC, TransactionType.ACCESS_LIST)
             and isinstance(txn, StaticFeeTransaction)
             and txn.gas_price is None
         ):
             txn.gas_price = self.gas_price
-        elif txn_type is TransactionType.DYNAMIC:
+
+        elif txn_type in (TransactionType.DYNAMIC, TransactionType.SHARED_BLOB):
             if txn.max_priority_fee is None:
                 txn.max_priority_fee = self.priority_fee
 
             if txn.max_fee is None:
                 multiplier = self.network.base_fee_multiplier
                 txn.max_fee = int(self.base_fee * multiplier + txn.max_priority_fee)
```

### Comparing `eth-ape-0.7.8/src/ape_ethereum/proxies.py` & `eth-ape-0.7.9/src/ape_ethereum/proxies.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_ethereum/transactions.py` & `eth-ape-0.7.9/src/ape_ethereum/transactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     Transaction enumerable type constants defined by
     `EIP-2718 <https://eips.ethereum.org/EIPS/eip-2718>`__.
     """
 
     STATIC = 0
     ACCESS_LIST = 1  # EIP-2930
     DYNAMIC = 2  # EIP-1559
+    SHARED_BLOB = 3  # EIP-4844
 
 
 class AccessList(BaseModel):
     address: AddressType
     storage_keys: List[HexBytes] = Field(default_factory=list, alias="storageKeys")
 
 
@@ -124,14 +125,30 @@
         # NOTE: Work-around, Pydantic doesn't handle calculated fields well.
         values["max_fee"] = cls.conversion_manager.convert(
             values.get("gas_limit", 0), int
         ) * cls.conversion_manager.convert(values.get("gas_price", 0), int)
         return values
 
 
+class AccessListTransaction(StaticFeeTransaction):
+    """
+    `EIP-2930 <https://eips.ethereum.org/EIPS/eip-2930>`__
+    transactions are similar to legacy transaction with an added access list functionality.
+    """
+
+    gas_price: Optional[int] = Field(None, alias="gasPrice")
+    type: int = Field(TransactionType.ACCESS_LIST.value)
+    access_list: List[AccessList] = Field(default_factory=list, alias="accessList")
+
+    @field_validator("type")
+    @classmethod
+    def check_type(cls, value):
+        return value.value if isinstance(value, TransactionType) else value
+
+
 class DynamicFeeTransaction(BaseTransaction):
     """
     Transactions that are post-EIP-1559 and use the ``maxFeePerGas``
     and ``maxPriorityFeePerGas`` fields.
     """
 
     max_priority_fee: Optional[int] = Field(None, alias="maxPriorityFeePerGas")  # type: ignore
@@ -141,28 +158,31 @@
 
     @field_validator("type")
     @classmethod
     def check_type(cls, value):
         return value.value if isinstance(value, TransactionType) else value
 
 
-class AccessListTransaction(StaticFeeTransaction):
+class SharedBlobTransaction(DynamicFeeTransaction):
     """
-    `EIP-2930 <https://eips.ethereum.org/EIPS/eip-2930>`__
-    transactions are similar to legacy transaction with an added access list functionality.
+    `EIP-4844 <https://eips.ethereum.org/EIPS/eip-4844>`__ transactions.
     """
 
-    gas_price: Optional[int] = Field(None, alias="gasPrice")
-    type: int = Field(TransactionType.ACCESS_LIST.value)
-    access_list: List[AccessList] = Field(default_factory=list, alias="accessList")
+    max_fee_per_blob_gas: int = Field(0, alias="maxFeePerBlobGas")
+    blob_versioned_hashes: List[HexBytes] = Field([], alias="blobVersionedHashes")
 
-    @field_validator("type")
+    """
+    Overridden because EIP-4844 states it cannot be nil.
+    """
+    receiver: AddressType = Field(ZERO_ADDRESS, alias="to")
+
+    @field_validator("max_fee_per_blob_gas", mode="before")
     @classmethod
-    def check_type(cls, value):
-        return value.value if isinstance(value, TransactionType) else value
+    def hex_to_int(cls, value):
+        return value if isinstance(value, int) else int(HexBytes(value).hex(), 16)
 
 
 class Receipt(ReceiptAPI):
     gas_limit: int
     gas_price: int
     gas_used: int
 
@@ -400,7 +420,17 @@
             contract_address=address,
             event_arguments={i.name: value for i, value in zip(method_abi.inputs, values)},
             event_name=method_abi.name,
             log_index=log["logIndex"],
             transaction_hash=log["transactionHash"],
             transaction_index=log["transactionIndex"],
         )
+
+
+class SharedBlobReceipt(Receipt):
+    blob_gas_used: int
+    blob_gas_price: int
+
+    @field_validator("blob_gas_used", "blob_gas_price", mode="before")
+    @classmethod
+    def hex_to_int(cls, value):
+        return value if isinstance(value, int) else int(HexBytes(value).hex(), 16)
```

### Comparing `eth-ape-0.7.8/src/ape_geth/__init__.py` & `eth-ape-0.7.9/src/ape_geth/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_geth/provider.py` & `eth-ape-0.7.9/src/ape_geth/provider.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_geth/query.py` & `eth-ape-0.7.9/src/ape_geth/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_init/_cli.py` & `eth-ape-0.7.9/src/ape_init/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_networks/__init__.py` & `eth-ape-0.7.9/src/ape_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_networks/_cli.py` & `eth-ape-0.7.9/src/ape_networks/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_plugins/_cli.py` & `eth-ape-0.7.9/src/ape_plugins/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_plugins/exceptions.py` & `eth-ape-0.7.9/src/ape_plugins/exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_pm/_cli.py` & `eth-ape-0.7.9/src/ape_pm/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_pm/compiler.py` & `eth-ape-0.7.9/src/ape_pm/compiler.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_run/_cli.py` & `eth-ape-0.7.9/src/ape_run/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_test/__init__.py` & `eth-ape-0.7.9/src/ape_test/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_test/_cli.py` & `eth-ape-0.7.9/src/ape_test/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_test/accounts.py` & `eth-ape-0.7.9/src/ape_test/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/ape_test/provider.py` & `eth-ape-0.7.9/src/ape_test/provider.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/eth_ape.egg-info/PKG-INFO` & `eth-ape-0.7.9/src/eth_ape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-ape
-Version: 0.7.8
+Version: 0.7.9
 Summary: Ape Ethereum Framework
 Home-page: https://apeworx.io
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Project-URL: Documentation, https://docs.apeworx.io/ape/
 Project-URL: Funding, https://gitcoin.co/grants/5958/ape-maintenance-fund
```

### Comparing `eth-ape-0.7.8/src/eth_ape.egg-info/SOURCES.txt` & `eth-ape-0.7.9/src/eth_ape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/src/eth_ape.egg-info/requires.txt` & `eth-ape-0.7.9/src/eth_ape.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/README.md` & `eth-ape-0.7.9/tests/README.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/conftest.py` & `eth-ape-0.7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/conftest.py` & `eth-ape-0.7.9/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/conversion/test_address.py` & `eth-ape-0.7.9/tests/functional/conversion/test_address.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/conversion/test_encode_structs.py` & `eth-ape-0.7.9/tests/functional/conversion/test_encode_structs.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/conversion/test_ether.py` & `eth-ape-0.7.9/tests/functional/conversion/test_ether.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/conversion/test_hex.py` & `eth-ape-0.7.9/tests/functional/conversion/test_hex.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/conversion/test_timestamp.py` & `eth-ape-0.7.9/tests/functional/conversion/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/abi/contract_abi.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/abi/contract_abi.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/BeaconProxy.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/BeaconProxy.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/ContractA.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/ContractA.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/ContractB.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/ContractB.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/ContractC.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/ContractC.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/DsNoteTest.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/DsNoteTest.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/HasError.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/HasError.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/RevertsContract.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/RevertsContract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/SolFallbackAndReceive.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/SolFallbackAndReceive.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/SolidityContract.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/SolidityContract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/SubReverts.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/SubReverts.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/VyDefault.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/VyDefault.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/VyperContract.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/VyperContract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/VyperFactory.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/VyperFactory.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/beacon.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/beacon.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/eip1967.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/eip1967.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/contracts/ethereum/local/proxy.json` & `eth-ape-0.7.9/tests/functional/data/contracts/ethereum/local/proxy.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/manifests/OpenZeppelin/v3.1.0/OpenZeppelin.json` & `eth-ape-0.7.9/tests/functional/data/manifests/OpenZeppelin/v3.1.0/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/manifests/OpenZeppelin/v4.4.2/OpenZeppelin.json` & `eth-ape-0.7.9/tests/functional/data/manifests/OpenZeppelin/v4.4.2/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/projects/ApeProject/contracts/Contract.json` & `eth-ape-0.7.9/tests/functional/data/projects/ApeProject/contracts/Contract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/python/__init__.py` & `eth-ape-0.7.9/tests/functional/data/python/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/sources/ContractA.sol` & `eth-ape-0.7.9/tests/functional/data/sources/ContractA.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/sources/ContractB.sol` & `eth-ape-0.7.9/tests/functional/data/sources/ContractB.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/sources/ContractC.sol` & `eth-ape-0.7.9/tests/functional/data/sources/ContractC.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/sources/HasError.sol` & `eth-ape-0.7.9/tests/functional/data/sources/HasError.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/sources/RevertsContract.vy` & `eth-ape-0.7.9/tests/functional/data/sources/RevertsContract.vy`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/sources/SolidityContract.sol` & `eth-ape-0.7.9/tests/functional/data/sources/SolidityContract.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/data/sources/VyperContract.vy` & `eth-ape-0.7.9/tests/functional/data/sources/VyperContract.vy`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/geth/conftest.py` & `eth-ape-0.7.9/tests/functional/geth/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/geth/test_contract.py` & `eth-ape-0.7.9/tests/functional/geth/test_contract.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/geth/test_provider.py` & `eth-ape-0.7.9/tests/functional/geth/test_provider.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/geth/test_query.py` & `eth-ape-0.7.9/tests/functional/geth/test_query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/geth/test_trace.py` & `eth-ape-0.7.9/tests/functional/geth/test_trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/geth/text_proxy.py` & `eth-ape-0.7.9/tests/functional/geth/text_proxy.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_accounts.py` & `eth-ape-0.7.9/tests/functional/test_accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_address.py` & `eth-ape-0.7.9/tests/functional/test_address.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_block.py` & `eth-ape-0.7.9/tests/functional/test_block.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_block_container.py` & `eth-ape-0.7.9/tests/functional/test_block_container.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_chain.py` & `eth-ape-0.7.9/tests/functional/test_chain.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_cli.py` & `eth-ape-0.7.9/tests/functional/test_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_compilers.py` & `eth-ape-0.7.9/tests/functional/test_compilers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_config.py` & `eth-ape-0.7.9/tests/functional/test_config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_console.py` & `eth-ape-0.7.9/tests/functional/test_console.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_contract.py` & `eth-ape-0.7.9/tests/functional/test_contract.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_contract_container.py` & `eth-ape-0.7.9/tests/functional/test_contract_container.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_contract_event.py` & `eth-ape-0.7.9/tests/functional/test_contract_event.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_contract_instance.py` & `eth-ape-0.7.9/tests/functional/test_contract_instance.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_contract_method_handler.py` & `eth-ape-0.7.9/tests/functional/test_contract_method_handler.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_contracts_cache.py` & `eth-ape-0.7.9/tests/functional/test_contracts_cache.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_coverage.py` & `eth-ape-0.7.9/tests/functional/test_coverage.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_default_sender_context_manager.py` & `eth-ape-0.7.9/tests/functional/test_default_sender_context_manager.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_dependencies.py` & `eth-ape-0.7.9/tests/functional/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_ecosystem.py` & `eth-ape-0.7.9/tests/functional/test_ecosystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,22 @@
 from ethpm_types.abi import ABIType, EventABI, MethodABI
 
 from ape.api.networks import LOCAL_NETWORK_NAME, NetworkAPI
 from ape.exceptions import DecodingError, NetworkError, NetworkNotFoundError
 from ape.types import AddressType
 from ape.utils import DEFAULT_LOCAL_TRANSACTION_ACCEPTANCE_TIMEOUT
 from ape_ethereum.ecosystem import BLUEPRINT_HEADER, BaseEthereumConfig, Block
-from ape_ethereum.transactions import DynamicFeeTransaction, StaticFeeTransaction, TransactionType
+from ape_ethereum.transactions import (
+    DynamicFeeTransaction,
+    Receipt,
+    SharedBlobReceipt,
+    SharedBlobTransaction,
+    StaticFeeTransaction,
+    TransactionType,
+)
 
 LOG = {
     "removed": False,
     "logIndex": "0x0",
     "transactionIndex": "0x0",
     "transactionHash": "0x74dd040dfa06f0af9af8ca95d7aae409978400151c746f55ecce19e7356cfc5a",
     "blockHash": "0x2c99950b07accf3e442512a3352a11e6fed37b2331de5f71b7743b357d96e4e8",
@@ -403,22 +410,23 @@
         "logsBloom": HexBytes(
             "0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000"  # noqa: E501
         ),
         "status": 1,
         "effectiveGasPrice": 0,
     }
     receipt = ethereum.decode_receipt(receipt_data)
+    assert type(receipt) is Receipt  # NOTE: Purposely not using isinstance()
 
     # Tests against bug where input data would come back improperly
     assert receipt.data == HexBytes(
         "0x3461169d573360005560016005556000600655600261040655600061040755600161040855600361080755600061080855600161080955600261080a55610c08546103ff811161169d5760018101610c0855610c038102610c09016005548082558060051b60018301600082601f0160051c610400811161169d57801561009657905b806006015481840155600101818118610082575b505050505061040654806104018301558060051b6001610401840101600082601f0160051c610400811161169d5780156100e157905b806104070154818401556001018181186100cc575b505050505061080754806108028301558060051b6001610802840101600082601f0160051c610400811161169d57801561012c57905b80610808015481840155600101818118610117575b5050505050505062301809546103ff811161169d57600181016230180955610c0381026230180a016005548082558060051b60018301600082601f0160051c610400811161169d57801561019057905b80600601548184015560010181811861017c575b505050505061040654806104018301558060051b6001610401840101600082601f0160051c610400811161169d5780156101db57905b806104070154818401556001018181186101c6575b505050505061080754806108028301558060051b6001610802840101600082601f0160051c610400811161169d57801561022657905b80610808015481840155600101818118610211575b5050505050505062301809546103ff811161169d57600181016230180955610c0381026230180a016005548082558060051b60018301600082601f0160051c610400811161169d57801561028a57905b806006015481840155600101818118610276575b505050505061040654806104018301558060051b6001610401840101600082601f0160051c610400811161169d5780156102d557905b806104070154818401556001018181186102c0575b505050505061080754806108028301558060051b6001610802840101600082601f0160051c610400811161169d57801561032057905b8061080801548184015560010181811861030b575b5050505050505061136361033961000039611363610000f36003361161000c5761134b565b60003560e01c3461135157632beb1711811861007c57600436186113515760007f1a7c56fae0af54ebae73bc4699b9de9835e7bb86b050dff7e80695b633f17abd60006040a260017fe5299d63f5ecdd1740024ea0902bd82cc8dc6b51d69078e007096f907615ced560006040a2005b633fb5c1cb81186101e95760243618611351576000543318156100f657600b6040527f21617574686f72697a656400000000000000000000000000000000000000000060605260405060405180606001601f826000031636823750506308c379a06000526020602052601f19601f6040510116604401601cfd5b6005600435146113515760015460025560043560015560076080527f44796e616d69630000000000000000000000000000000000000000000000000060a05260808051602082012090506004357fa84473122c11e32cd505595f246a28418b8ecd6cf819f4e3915363fad1b8f9686060600143034060c05260025460e052806101005260076040527f44796e616d69630000000000000000000000000000000000000000000000000060605260408160c00181518082526020830160208301815181525050508051806020830101601f82600003163682375050601f19601f82516020010116905090508101905060c0a3005b63e30081a081186102445760243618611351576004358060a01c611351576040526040516003556040517f7ff7bacc6cd661809ed1ddce28d4ad2c5b37779b61b9e3235f8262be529101a960006060a2607b60605260206060f35b63e30443bc811861028d5760443618611351576004358060a01c611351576040526004604051602052600052604060002080546024358082018281106113515790509050815550005b6309b1b3f281186102b257600436186113515733604052600143034060605260406040f35b6302f487d681186102dc576004361861135157336040526001430340606052600160805260606040f35b63a420b5a58118610306576004361861135157600260405233606052600143034060805260606040f35b63e9f7fd1481186103355760043618611351573360405260014303406060526001608052600160a05260806040f35b63a2fbee5381186103645760043618611351576002604052600260605233608052600143034060a05260806040f35b6342ce1ec6811861039f57600436186113515760016040523360605260014303406080523360a052600143034060c052600260e05260c06040f35b63052f3e76811861040257600436186113515760208060405280604001600060008252600060006000600181116113515780156103ef57905b60008160051b6020870101526001018181186103d8575b5050810160200190509050810190506040f35b63b345ad96811861047d576004361861135157602080604052806040016000600160a052600160c052600060a0518084528060051b6000826001811161135157801561046757905b8060051b60c001518160051b60208901015260010181811861044a575b5050820160200191505090509050810190506040f35b6335417bf48118610506576004361861135157602080604052806040016000600360e052600161010052600261012052600361014052600060e0518084528060051b600082600381116113515780156104f057905b8060051b61010001518160051b6020890101526001018181186104d2575b5050820160200191505090509050810190506040f35b63a5b0930d8118610585576004361861135157602080604052806040016000600260c0523360e0523361010052600060c0518084528060051b6000826002811161135157801561056f57905b8060051b60e001518160051b602089010152600101818118610552575b5050820160200191505090509050810190506040f35b639bfb2ad8811861063e576004361861135157602080604052806040016000600261014052336101605260014303406101805260016101a052336101c05260014303406101e052600261020052600061014051808452606081026000826002811161135157801561062857905b606081026020880101606082026101600180518252602081015160208301526040810151604083015250506001018181186105f2575b5050820160200191505090509050810190506040f35b633ce80e9481186106795760043618611351576001604052336060526001430340608052600260a0523360c052600143034060e05260c06040f35b6343790b64811861069a576004361861135157610280366040376102806040f35b63d4d64b3581186106bb576004361861135157610500366040376105006040f35b63650543a381186106df576004361861135157607b60405261014160605260406040f35b63243e096381186106fe57600436186113515760403660403760406040f35b638ba6052d81186107c657600436186113515761028036604037336040526040516102c0526060516102e0526080516103005260a0516103205260c0516103405260e051610360526101005161038052610120516103a052610140516103c052610160516103e05261018051610400526101a051610420526101c051610440526101e051610460526102005161048052610220516104a052610240516104c052610260516104e05261028051610500526102a0516105205261028036610540376105006102c0f35b63ccd62aa481186107fd576004361861135157600160405260026060526003608052600460a052600560c052600660e05260c06040f35b636126c87f81186108b2576004361861135157602080604052806040016000600362010080526001620100a0526002620100c0526003620100e052600462010100526005620101205260066201014052600062010080518084528060061b600082610400811161135157801561089c57905b8060061b60208801018160061b620100a0018051825260208101516020830152505060010181811861086f575b5050820160200191505090509050810190506040f35b6394a66fc981186109d557600436186113515760208060405280604001606080825280820160006005548083528060051b600082610400811161135157801561091157905b80600601548160051b6020880101526001018181186108f7575b505082016020019150509050810190508060208301528082016000610406548083528060051b600082610400811161135157801561096657905b8061040701548160051b60208801015260010181811861094b575b505082016020019150509050810190508060408301528082016000610807548083528060051b60008261040081116113515780156109bb57905b8061080801548160051b6020880101526001018181186109a0575b505082016020019150509050810190509050810190506040f35b63abeb202281186111335760043618611351576020806040528060400160a08082528082016000610c08548083528060051b6000826104008111611351578015610b5157905b828160051b602088010152610c038102610c09018360208801016060808252808201600084548083528060051b6000826104008111611351578015610a7857905b8060018a0101548160051b602088010152600101818118610a5c575b505082016020019150509050810190508060208301526104018301818301600082548083528060051b6000826104008111611351578015610ad157905b806001880101548160051b602088010152600101818118610ab5575b5050820160200191505090509050810190508060408301526108028301818301600082548083528060051b6000826104008111611351578015610b2c57905b806001880101548160051b602088010152600101818118610b10575b5050820160200191505090509050810190509050905083019250600101818118610a1b575b50508201602001915050905081019050806020830152808201600062301809548083528060051b6000826104008111611351578015610cc357905b828160051b602088010152610c0381026230180a018360208801016060808252808201600084548083528060051b6000826104008111611351578015610bea57905b8060018a0101548160051b602088010152600101818118610bce575b505082016020019150509050810190508060208301526104018301818301600082548083528060051b6000826104008111611351578015610c4357905b806001880101548160051b602088010152600101818118610c27575b5050820160200191505090509050810190508060408301526108028301818301600082548083528060051b6000826104008111611351578015610c9e57905b806001880101548160051b602088010152600101818118610c82575b5050820160200191505090509050810190509050905083019250600101818118610b8c575b5050820160200191505090508101905080604083015280820160006260240a548083528060051b6000826104008111611351578015610e3557905b828160051b602088010152610c0381026260240b018360208801016060808252808201600084548083528060051b6000826104008111611351578015610d5c57905b8060018a0101548160051b602088010152600101818118610d40575b505082016020019150509050810190508060208301526104018301818301600082548083528060051b6000826104008111611351578015610db557905b806001880101548160051b602088010152600101818118610d99575b5050820160200191505090509050810190508060408301526108028301818301600082548083528060051b6000826104008111611351578015610e1057905b806001880101548160051b602088010152600101818118610df4575b5050820160200191505090509050810190509050905083019250600101818118610cfe575b5050820160200191505090508101905080606083015280820160006290300b548083528060051b6000826104008111611351578015610fa757905b828160051b602088010152610c0381026290300c018360208801016060808252808201600084548083528060051b6000826104008111611351578015610ece57905b8060018a0101548160051b602088010152600101818118610eb2575b505082016020019150509050810190508060208301526104018301818301600082548083528060051b6000826104008111611351578015610f2757905b806001880101548160051b602088010152600101818118610f0b575b5050820160200191505090509050810190508060408301526108028301818301600082548083528060051b6000826104008111611351578015610f8257905b806001880101548160051b602088010152600101818118610f66575b5050820160200191505090509050810190509050905083019250600101818118610e70575b50508201602001915050905081019050806080830152808201600062c03c0c548083528060051b600082610400811161135157801561111957905b828160051b602088010152610c03810262c03c0d018360208801016060808252808201600084548083528060051b600082610400811161135157801561104057905b8060018a0101548160051b602088010152600101818118611024575b505082016020019150509050810190508060208301526104018301818301600082548083528060051b600082610400811161135157801561109957905b806001880101548160051b60208801015260010181811861107d575b5050820160200191505090509050810190508060408301526108028301818301600082548083528060051b60008261040081116113515780156110f457905b806001880101548160051b6020880101526001018181186110d8575b5050820160200191505090509050810190509050905083019250600101818118610fe2575b505082016020019150509050810190509050810190506040f35b6399e74a4c81186111e25760043618611351576020806040528060400160006002620180805233620180a05233620180c05233620180e0526060366201810037600062018080518084526060810260008261040081116113515780156111cc57905b60608102602088010160608202620180a0018051825260208101516020830152604081015160408301525050600101818118611195575b5050820160200191505090509050810190506040f35b638da5cb5b811861120157600436186113515760005460405260206040f35b6323fd0e40811861122057600436186113515760015460405260206040f35b634825cf6f811861123f57600436186113515760025460405260206040f35b636cbceeec811861125e57600436186113515760035460405260206040f35b6327e235e381186112995760243618611351576004358060a01c61135157604052600460405160205260005260406000205460605260206060f35b63d3aaff6d81186112db576044361861135157610401600435600281116113515702600501602435815481101561135157600182010190505460405260206040f35b63ae8ef2cb811861134957608436186113515762300c01600435600481116113515702610c0801610c03602435825481101561135157026001820101905061040160443560028111611351570281019050606435815481101561135157600182010190505460405260206040f35b505b60006000fd5b600080fda165767970657283000306000b005b600080fd"  # noqa: E501
     )
 
 
-def test_decode_etherscan_receipt(eth_tester_provider, ethereum):
+def test_decode_receipt_from_etherscan(eth_tester_provider, ethereum):
     receipt = ethereum.decode_receipt(
         {
             "blockNumber": "11291970",
             "timeStamp": "1661846925",
             "hash": "0x5780b43d819035ed1fa079171bdce7f0bbeaa6b01f201f8985d279a66cfc6844",
             "nonce": "0",
             "blockHash": "0x3175f953c1da4bf3d15b853dae4a150ae44e2e71380936463e89142c12961968",
@@ -436,19 +444,69 @@
             "methodId": "0xf926657e",
             "functionName": "setup(address _reputationOracle, address _recordingOracle, uint256 _reputationOracleStake, uint256 _recordingOracleStake, string _url, string _hash)",  # noqa: E501
             "required_confirmations": "13703",
             "status": "1",
             "chainId": 1,
         }
     )
+    assert type(receipt) is Receipt  # NOTE: Purposely not using isinstance()
     assert receipt.type == 0
     assert receipt.max_fee == 0
     assert receipt.gas_price == 1499999989
 
 
+def test_decode_receipt_shared_blob(ethereum):
+    blob_gas_price = "0x4d137e31b"
+    blob_gas_used = "0x20000"
+
+    data = {
+        "required_confirmations": 0,
+        "blockHash": HexBytes("0x051fb508617fcbe0034538b7ee54c1dedbbbaa6f8d0aeb776edf81bafbc883bd"),
+        "blockNumber": 10526428,
+        "from": "0x194E22F49BC3f58903866d55488E1e9e8d69b517",
+        "gas": 5500000,
+        "gasPrice": 1000000008,
+        "maxFeePerGas": 150000000000,
+        "maxPriorityFeePerGas": 1000000000,
+        "maxFeePerBlobGas": "0x22ecb25c00",
+        "hash": HexBytes("0xd2882bae0d79a6c8e0fbf0089bbcb4b2eef3a1365471ad9f779b06a41ba47d3c"),
+        "input": HexBytes("0xb72d42a1000000000000000000000000000000000000000000"),  # Note: abridged
+        "nonce": 329925,
+        "to": "0xd5c325D183C592C94998000C5e0EED9e6655c020",
+        "transactionIndex": 48,
+        "value": 0,
+        "type": 3,
+        "accessList": [],
+        "chainId": 5,
+        "blobVersionedHashes": [
+            "0x015405d502a27897ad38ffcb80566d1559fa53764befc6d90731082837c2d19e"
+        ],
+        "v": 0,
+        "r": HexBytes("0x4e5bdcbba31548cb8f9806491c5ced7b0f1eac78c7dc0677616c23ee0e469f74"),
+        "s": HexBytes("0x31c98ea044c97225d83b9a3f0fa719e2299b9fbc6436e4b3eb096ea528de03ff"),
+        "yParity": 0,
+        "blobGasPrice": blob_gas_price,
+        "blobGasUsed": blob_gas_used,
+        "contractAddress": None,
+        "cumulativeGasUsed": 23085827,
+        "effectiveGasPrice": 1000000008,
+        "gasUsed": 219756,
+        "logs": [],
+        "logsBloom": HexBytes("0x00000000010002"),
+        "status": 1,
+        "transactionHash": HexBytes(
+            "0xd2882bae0d79a6c8e0fbf0089bbcb4b2eef3a1365471ad9f779b06a41ba47d3c"
+        ),
+    }
+    actual = ethereum.decode_receipt(data)
+    assert isinstance(actual, SharedBlobReceipt)
+    assert actual.blob_gas_used == int(blob_gas_used, 16)
+    assert actual.blob_gas_price == int(blob_gas_price, 16)
+
+
 def test_default_transaction_type_not_connected_used_default_network(
     temp_config, ethereum, networks
 ):
     value = TransactionType.STATIC.value
     config_dict = {"ethereum": {"mainnet_fork": {"default_transaction_type": value}}}
     assert ethereum.default_transaction_type == TransactionType.DYNAMIC
 
@@ -656,14 +714,51 @@
 @pytest.mark.parametrize("kwarg_name", ("max_fee", "max_fee_per_gas", "maxFee", "maxFeePerGas"))
 def test_create_transaction_max_fee_per_gas(kwarg_name, ethereum):
     fee = 1_000_000_000
     tx = ethereum.create_transaction(**{kwarg_name: fee})
     assert tx.max_fee == fee
 
 
+@pytest.mark.parametrize("kwarg_name", ("gas_price", "gasPrice"))
+def test_create_transaction_with_gas_price(kwarg_name, ethereum):
+    price = 123
+    tx = ethereum.create_transaction(**{kwarg_name: price})
+    assert tx.gas_price == price
+
+
+@pytest.mark.parametrize(
+    "tx_kwargs",
+    [{"type": 3}, {"max_fee_per_blob_gas": 123}, {"blob_versioned_hashes": [HexBytes(123)]}],
+)
+def test_create_transaction_shared_blob(tx_kwargs, ethereum):
+    tx = ethereum.create_transaction(**tx_kwargs)
+    assert isinstance(tx, SharedBlobTransaction)
+    assert tx.type == TransactionType.SHARED_BLOB.value
+
+
+@pytest.mark.parametrize(
+    "kwarg_name,value", [("max_fee_per_blob_gas", 345), ("maxFeePerBlobGas", "0x2343")]
+)
+def test_create_transaction_max_fee_per_blob_gas(kwarg_name, value, ethereum):
+    tx = ethereum.create_transaction(**{kwarg_name: value})
+    assert isinstance(tx, SharedBlobTransaction)
+    expected = value if isinstance(value, int) else int(HexBytes(value).hex(), 16)
+    assert tx.max_fee_per_blob_gas == expected
+
+
+@pytest.mark.parametrize(
+    "kwarg_name,value",
+    [("blob_versioned_hashes", "0x123"), ("blobVersionedHashes", HexBytes("0x123"))],
+)
+def test_create_transaction_blob_versioned_hashed(kwarg_name, value, ethereum):
+    tx = ethereum.create_transaction(**{kwarg_name: [value]})
+    assert isinstance(tx, SharedBlobTransaction)
+    assert tx.blob_versioned_hashes == [HexBytes(value)]
+
+
 @pytest.mark.parametrize("tx_type", TransactionType)
 def test_encode_transaction(tx_type, ethereum, vyper_contract_instance, owner, eth_tester_provider):
     abi = vyper_contract_instance.contract_type.methods[0]
     actual = ethereum.encode_transaction(
         vyper_contract_instance.address, abi, sender=owner.address, type=tx_type.value
     )
     assert actual.gas_limit == eth_tester_provider.max_gas
```

### Comparing `eth-ape-0.7.8/tests/functional/test_exceptions.py` & `eth-ape-0.7.9/tests/functional/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_fixtures.py` & `eth-ape-0.7.9/tests/functional/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_history.py` & `eth-ape-0.7.9/tests/functional/test_history.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_logging.py` & `eth-ape-0.7.9/tests/functional/test_logging.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_multicall.py` & `eth-ape-0.7.9/tests/functional/test_multicall.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_network_api.py` & `eth-ape-0.7.9/tests/functional/test_network_api.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_network_manager.py` & `eth-ape-0.7.9/tests/functional/test_network_manager.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_plugins.py` & `eth-ape-0.7.9/tests/functional/test_plugins.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_project.py` & `eth-ape-0.7.9/tests/functional/test_project.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_provider.py` & `eth-ape-0.7.9/tests/functional/test_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,14 +274,15 @@
 def test_prepare_transaction_with_max_gas(tx_type, eth_tester_provider, ethereum, owner):
     tx = ethereum.create_transaction(type=tx_type.value, sender=owner.address)
     tx.gas_limit = None  # Undo set from validator
     assert tx.gas_limit is None, "Test setup failed - couldn't clear tx gas limit."
 
     actual = eth_tester_provider.prepare_transaction(tx)
     assert actual.gas_limit == eth_tester_provider.max_gas
+    assert actual.max_fee is not None
 
 
 def test_no_comma_in_rpc_url():
     test_url = "URI: http://127.0.0.1:8545,"
     sanitised_url = _sanitize_web3_url(test_url)
 
     assert "," not in sanitised_url
```

### Comparing `eth-ape-0.7.8/tests/functional/test_query.py` & `eth-ape-0.7.9/tests/functional/test_query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_receipt.py` & `eth-ape-0.7.9/tests/functional/test_receipt.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_reverts_context_manager.py` & `eth-ape-0.7.9/tests/functional/test_reverts_context_manager.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/test_transaction.py` & `eth-ape-0.7.9/tests/functional/test_transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,73 +123,83 @@
 
 @pytest.fixture
 def access_list():
     return ACCESS_LIST
 
 
 @pytest.mark.parametrize("type_kwarg", (0, "0x0", b"\x00", "0", HexBytes("0x0"), HexBytes("0x00")))
-def test_create_static_fee_transaction(ethereum, type_kwarg):
+def test_type_0_transactions(ethereum, type_kwarg):
     txn = ethereum.create_transaction(type=type_kwarg)
     assert txn.type == TransactionType.STATIC.value
 
 
 @pytest.mark.parametrize("type_kwarg", (1, "0x01", b"\x01", "1", "01", HexBytes("0x01")))
-def test_create_access_list_transaction(ethereum, type_kwarg):
+def test_type_1_transactions(ethereum, type_kwarg):
     txn = ethereum.create_transaction(type=type_kwarg)
     assert txn.type == TransactionType.ACCESS_LIST.value
 
 
 @pytest.mark.parametrize("type_kwarg", (None, 2, "0x02", b"\x02", "2", "02", HexBytes("0x02")))
-def test_create_dynamic_fee_transaction(ethereum, type_kwarg):
+def test_type_2_transactions(ethereum, type_kwarg):
     txn = ethereum.create_transaction(type=type_kwarg)
     assert txn.type == TransactionType.DYNAMIC.value
 
 
 @pytest.mark.parametrize("key", ("accessList", "access_list"))
-def test_transaction_with_access_lists(ethereum, access_list, key):
+def test_type_1_transactions_using_access_list(ethereum, access_list, key):
     """
     If not given type and only given accessList, the assumed type is 1,
     an "access-list" transaction.
     """
     data = {key: access_list}
     txn = ethereum.create_transaction(**data)
     assert txn.type == 1
 
 
 @pytest.mark.parametrize("key", ("accessList", "access_list"))
-def test_transaction_with_access_lists_and_max_fee(ethereum, access_list, key):
+def test_type_2_transactions_with_max_fee_and_access_list(ethereum, access_list, key):
     """
     Dynamic-fee txns also support access lists, so the presence of max_fee
     with access_list implies a type 2 txn.
     """
     data = {"max_fee": 1000000000, key: access_list}
     txn = ethereum.create_transaction(**data)
     assert txn.type == 2
+    assert txn.max_fee == 1000000000
 
 
-def test_create_dynamic_fee_transaction_with_access_lists(ethereum, access_list):
+def test_type_2_transactions_with_access_list(ethereum, access_list):
     txn = ethereum.create_transaction(type=2, accessList=access_list)
     assert txn.type == TransactionType.DYNAMIC.value
     assert txn.access_list == [AccessList.model_validate(x) for x in access_list]
 
 
 @pytest.mark.parametrize(
+    "tx_kwargs",
+    [{"type": 3}, {"max_fee_per_blob_gas": 123}, {"blob_versioned_hashes": [HexBytes(123)]}],
+)
+def test_type_3_transactions(ethereum, tx_kwargs):
+    txn = ethereum.create_transaction(**tx_kwargs)
+    assert txn.type == 3
+
+
+@pytest.mark.parametrize(
     "fee_kwargs",
     (
         {"max_fee": "100 gwei"},
         {"max_fee": int(100e9)},
         {"max_priority_fee": "1 gwei"},
         {"max_priority_fee": int(1e9)},
         {"max_priority_fee": "1 gwei", "max_fee": "100 gwei"},
         {"max_priority_fee": int(1e9), "max_fee": "100 gwei"},
         {"max_priority_fee": "1 gwei", "max_fee": int(100e9)},
         {"max_priority_fee": int(1e9), "max_fee": int(100e9)},
     ),
 )
-def test_create_dynamic_fee_kwargs(ethereum, fee_kwargs):
+def test_type_2_transactions_using_fee_kwargs(ethereum, fee_kwargs):
     txn = ethereum.create_transaction(**fee_kwargs)
     assert isinstance(txn, DynamicFeeTransaction)
     if "max_priority_fee" in fee_kwargs:
         assert txn.max_priority_fee == int(1e9)
     if "max_fee" in fee_kwargs:
         assert txn.max_fee == int(100e9)
```

### Comparing `eth-ape-0.7.8/tests/functional/test_types.py` & `eth-ape-0.7.9/tests/functional/test_types.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/utils/test_abi.py` & `eth-ape-0.7.9/tests/functional/utils/test_abi.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/utils/test_basemodel.py` & `eth-ape-0.7.9/tests/functional/utils/test_basemodel.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/utils/test_github.py` & `eth-ape-0.7.9/tests/functional/utils/test_github.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/utils/test_misc.py` & `eth-ape-0.7.9/tests/functional/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/utils/test_os.py` & `eth-ape-0.7.9/tests/functional/utils/test_os.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/functional/utils/test_trace.py` & `eth-ape-0.7.9/tests/functional/utils/test_trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/conftest.py` & `eth-ape-0.7.9/tests/integration/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/geth/ape-config.yaml` & `eth-ape-0.7.9/tests/integration/cli/projects/geth/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/geth/contracts/TokenA.json` & `eth-ape-0.7.9/tests/integration/cli/projects/geth/contracts/TokenA.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/geth/contracts/TokenB.json` & `eth-ape-0.7.9/tests/integration/cli/projects/geth/contracts/TokenB.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/geth/contracts/VyperContract.json` & `eth-ape-0.7.9/tests/integration/cli/projects/geth/contracts/VyperContract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/geth/tests/test_using_local_geth.py` & `eth-ape-0.7.9/tests/integration/cli/projects/geth/tests/test_using_local_geth.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/script/contracts/VyperContract.json` & `eth-ape-0.7.9/tests/integration/cli/projects/script/contracts/VyperContract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/test/tests/test_fixture_isolation.py` & `eth-ape-0.7.9/tests/integration/cli/projects/test/tests/test_fixture_isolation.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/test/tests/test_fixtures.py` & `eth-ape-0.7.9/tests/integration/cli/projects/test/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/test/tests/test_networks.py` & `eth-ape-0.7.9/tests/integration/cli/projects/test/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/ContractA.json` & `eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/ContractA.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json` & `eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json` & `eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/dep/contracts/RawVyperOutputDep.json` & `eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/dep/contracts/RawVyperOutputDep.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/with-contracts/tests/test_contract.py` & `eth-ape-0.7.9/tests/integration/cli/projects/with-contracts/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/projects/with-dependencies/ape-config.yaml` & `eth-ape-0.7.9/tests/integration/cli/projects/with-dependencies/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/test_accounts.py` & `eth-ape-0.7.9/tests/integration/cli/test_accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/test_compile.py` & `eth-ape-0.7.9/tests/integration/cli/test_compile.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/test_console.py` & `eth-ape-0.7.9/tests/integration/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/test_init.py` & `eth-ape-0.7.9/tests/integration/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/test_misc.py` & `eth-ape-0.7.9/tests/integration/cli/test_misc.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/test_networks.py` & `eth-ape-0.7.9/tests/integration/cli/test_networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/test_plugins.py` & `eth-ape-0.7.9/tests/integration/cli/test_plugins.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/test_pm.py` & `eth-ape-0.7.9/tests/integration/cli/test_pm.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/test_run.py` & `eth-ape-0.7.9/tests/integration/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/test_test.py` & `eth-ape-0.7.9/tests/integration/cli/test_test.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.7.8/tests/integration/cli/utils.py` & `eth-ape-0.7.9/tests/integration/cli/utils.py`

 * *Files identical despite different names*

