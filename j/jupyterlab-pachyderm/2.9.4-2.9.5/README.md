# Comparing `tmp/jupyterlab_pachyderm-2.9.4.tar.gz` & `tmp/jupyterlab_pachyderm-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pachyderm-2.9.4.tar", last modified: Wed Apr 10 14:54:37 2024, max compression
+gzip compressed data, was "jupyterlab_pachyderm-2.9.5.tar", last modified: Wed Apr 24 18:14:47 2024, max compression
```

## Comparing `jupyterlab_pachyderm-2.9.4.tar` & `jupyterlab_pachyderm-2.9.5.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.870122 jupyterlab_pachyderm-2.9.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11816 2024-04-10 14:54:37.870122 jupyterlab_pachyderm-2.9.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10416 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/babel.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/cypress.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jest.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.846121 jupyterlab_pachyderm-2.9.4/jupyter-config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.850121 jupyterlab_pachyderm-2.9.4/jupyter-config/nb-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyter-config/nb-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.850121 jupyterlab_pachyderm-2.9.4/jupyter-config/server-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyter-config/server-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.854121 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      922 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/dev_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      725 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28506 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/handlers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.854121 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4410 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.846121 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/schemas/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.854121 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2024-04-10 14:54:26.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-10 14:54:26.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2024-04-10 14:54:26.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2024-04-10 14:54:26.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-04-10 14:54:26.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.858121 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   103733 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/357.1fda421931fafa738e6c.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   157933 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/576.391ef6f4845c9db67e0a.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17631 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/656.c4dc8222482db230e38e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/656.c4dc8222482db230e38e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    51076 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/714.4dee3c5425bce6321038.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/714.4dee3c5425bce6321038.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15715 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/747.e74bd68dc9f322227641.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8625 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/remoteEntry.cbb353a2353963df4b09.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-04-10 14:54:26.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16366 2024-04-10 14:54:35.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/log.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33782 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/pfs_manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11402 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/pps_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.858121 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3201 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.858121 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/data/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/setup_large_repo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4872 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/test_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16897 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/test_integrations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10784 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/test_pps.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.870122 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11816 2024-04-10 14:54:37.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4851 2024-04-10 14:54:37.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-10 14:54:37.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-10 14:54:14.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2024-04-10 14:54:37.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-04-10 14:54:37.000000 jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2024-04-10 14:52:22.000000 jupyterlab_pachyderm-2.9.4/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.858121 jupyterlab_pachyderm-2.9.4/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/schema/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/schema/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/schema/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/schema/telemetry.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2024-04-10 14:54:37.870122 jupyterlab_pachyderm-2.9.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.858121 jupyterlab_pachyderm-2.9.4/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/global.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/handler.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.850121 jupyterlab_pachyderm-2.9.4/src/plugins/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/examples/__test__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/examples/__test__/examples.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/examples/examples.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/examples/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/help/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/help/__tests__/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/help/__tests__/__snapshots__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/help/__tests__/help.test.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/help/help.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/help/help.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/help/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3496 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/__tests__/api.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5759 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/__tests__/mount.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2527 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/api.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.850121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8093 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Config/Config.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Config/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11721 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Config/__tests__/Config.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Config/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4041 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Config/hooks/useConfig.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Datum/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4297 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Datum/Datum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Datum/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6893 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Datum/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7254 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Datum/hooks/useDatum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Explore/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3135 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Explore/Explore.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/FullPageError/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/FullPageError/FullPageError.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.862121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/FullPageError/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      630 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9310 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Pipeline/Pipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Pipeline/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3538 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Pipeline/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5372 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5431 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/customFileBrowser.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6933 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/mount.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15262 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/mount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12612 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/mountDrive.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4313 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/pollMounts.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2862 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/mount/types.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/plugins/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/plugins/telemetry/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/telemetry/__tests__/telemetry.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/telemetry/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/plugins/telemetry/telemetry.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/setupTests.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/utils/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.850121 jupyterlab_pachyderm-2.9.4/src/utils/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/utils/components/Circle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/Circle/Circle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/Circle/circle.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/utils/components/DropdownCombobox/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      506 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/DropdownCombobox/DropdownCombobox.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2335 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/DropdownCombobox/DropdownCombobox.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/utils/components/DropdownCombobox/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4469 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/DropdownCombobox/__tests__/DropdownCombobox.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/utils/components/LoadingDots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/LoadingDots/LoadingDots.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/LoadingDots/loadingDots.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/src/utils/components/Svgs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/Svgs/GenericError.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/Svgs/KubernetesElephant.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/Svgs/PachydermLogo.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/Svgs/StatusWarning.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/components/Svgs/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/icons.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/src/utils/testUtils.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/style/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      595 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/style/base.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.866121 jupyterlab_pachyderm-2.9.4/style/components/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/style/components/button.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/style/components/input.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 14:54:37.870122 jupyterlab_pachyderm-2.9.4/style/icons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/style/icons/file.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/style/icons/info.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/style/icons/mount-logo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/style/icons/repo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/style/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/style/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2024-04-10 14:52:21.000000 jupyterlab_pachyderm-2.9.4/tsconfig.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.601174 jupyterlab_pachyderm-2.9.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11816 2024-04-24 18:14:47.601174 jupyterlab_pachyderm-2.9.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10416 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/babel.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/cypress.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/install.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jest.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.577174 jupyterlab_pachyderm-2.9.5/jupyter-config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.581174 jupyterlab_pachyderm-2.9.5/jupyter-config/nb-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyter-config/nb-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.581174 jupyterlab_pachyderm-2.9.5/jupyter-config/server-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyter-config/server-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.581174 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      922 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/dev_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      725 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28506 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.585174 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4410 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.577174 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/schemas/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.585174 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2024-04-24 18:14:34.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-24 18:14:34.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2024-04-24 18:14:34.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2024-04-24 18:14:34.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-04-24 18:14:34.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.589174 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   103733 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/357.1fda421931fafa738e6c.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   157933 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/576.391ef6f4845c9db67e0a.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17631 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/656.c4dc8222482db230e38e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/656.c4dc8222482db230e38e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    51076 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/714.4dee3c5425bce6321038.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/714.4dee3c5425bce6321038.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15715 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/747.e74bd68dc9f322227641.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8625 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/remoteEntry.38da920ab6234bb8b971.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-04-24 18:14:34.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/style.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16366 2024-04-24 18:14:45.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/log.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33782 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/pfs_manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11402 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/pps_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.589174 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3201 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.589174 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/data/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/setup_large_repo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4872 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16897 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/test_integrations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10784 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/test_pps.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.597174 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11816 2024-04-24 18:14:47.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4851 2024-04-24 18:14:47.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 18:14:47.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 18:14:22.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2024-04-24 18:14:47.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-04-24 18:14:47.000000 jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2024-04-24 18:12:33.000000 jupyterlab_pachyderm-2.9.5/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.589174 jupyterlab_pachyderm-2.9.5/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/schema/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/schema/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/schema/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/schema/telemetry.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2024-04-24 18:14:47.601174 jupyterlab_pachyderm-2.9.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.589174 jupyterlab_pachyderm-2.9.5/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/global.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/handler.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.577174 jupyterlab_pachyderm-2.9.5/src/plugins/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.589174 jupyterlab_pachyderm-2.9.5/src/plugins/examples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.589174 jupyterlab_pachyderm-2.9.5/src/plugins/examples/__test__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/examples/__test__/examples.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/examples/examples.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/examples/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.589174 jupyterlab_pachyderm-2.9.5/src/plugins/help/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.589174 jupyterlab_pachyderm-2.9.5/src/plugins/help/__tests__/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.589174 jupyterlab_pachyderm-2.9.5/src/plugins/help/__tests__/__snapshots__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/help/__tests__/help.test.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/help/help.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/help/help.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/help/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3496 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/__tests__/api.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5759 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/__tests__/mount.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2527 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/api.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.577174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8093 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Config/Config.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Config/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11721 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Config/__tests__/Config.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Config/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4041 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Config/hooks/useConfig.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Datum/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4297 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Datum/Datum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Datum/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6893 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Datum/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7254 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Datum/hooks/useDatum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Explore/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3135 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Explore/Explore.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/FullPageError/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/FullPageError/FullPageError.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/FullPageError/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      630 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9310 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Pipeline/Pipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Pipeline/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3538 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Pipeline/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5372 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5431 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/customFileBrowser.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6933 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/mount.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15262 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/mount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12612 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/mountDrive.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4313 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/pollMounts.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2862 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/mount/types.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/plugins/telemetry/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/telemetry/__tests__/telemetry.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/telemetry/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/plugins/telemetry/telemetry.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/setupTests.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.593174 jupyterlab_pachyderm-2.9.5/src/utils/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.577174 jupyterlab_pachyderm-2.9.5/src/utils/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.597174 jupyterlab_pachyderm-2.9.5/src/utils/components/Circle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/Circle/Circle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/Circle/circle.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.597174 jupyterlab_pachyderm-2.9.5/src/utils/components/DropdownCombobox/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      506 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/DropdownCombobox/DropdownCombobox.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2335 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/DropdownCombobox/DropdownCombobox.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.597174 jupyterlab_pachyderm-2.9.5/src/utils/components/DropdownCombobox/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4469 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/DropdownCombobox/__tests__/DropdownCombobox.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.597174 jupyterlab_pachyderm-2.9.5/src/utils/components/LoadingDots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/LoadingDots/LoadingDots.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/LoadingDots/loadingDots.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.597174 jupyterlab_pachyderm-2.9.5/src/utils/components/Svgs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/Svgs/GenericError.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/Svgs/KubernetesElephant.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/Svgs/PachydermLogo.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/Svgs/StatusWarning.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/components/Svgs/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/icons.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/src/utils/testUtils.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.597174 jupyterlab_pachyderm-2.9.5/style/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      595 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/style/base.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.597174 jupyterlab_pachyderm-2.9.5/style/components/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/style/components/button.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/style/components/input.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 18:14:47.597174 jupyterlab_pachyderm-2.9.5/style/icons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/style/icons/file.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/style/icons/info.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/style/icons/mount-logo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/style/icons/repo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/style/index.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/style/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2024-04-24 18:12:32.000000 jupyterlab_pachyderm-2.9.5/tsconfig.json
```

### Comparing `jupyterlab_pachyderm-2.9.4/LICENSE` & `jupyterlab_pachyderm-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/MANIFEST.in` & `jupyterlab_pachyderm-2.9.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/PKG-INFO` & `jupyterlab_pachyderm-2.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_pachyderm
-Version: 2.9.4
+Version: 2.9.5
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.9.4/README.md` & `jupyterlab_pachyderm-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/__init__.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/_version.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/dev_server.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/dev_server.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/env.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/env.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/handlers.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/package.json` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758597883597885%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.38da920ab6234bb8b971.js'}}",*

 * * "'version'": "'2.9.5'"}*

```diff
@@ -69,15 +69,15 @@
                 "npm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.cbb353a2353963df4b09.js",
+            "load": "static/remoteEntry.38da920ab6234bb8b971.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
@@ -135,9 +135,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.9.4"
+    "version": "2.9.5"
 }
```

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.9.5'"}*

```diff
@@ -130,9 +130,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.9.4"
+    "version": "2.9.5"
 }
```

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/357.1fda421931fafa738e6c.js` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/357.1fda421931fafa738e6c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/576.391ef6f4845c9db67e0a.js` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/576.391ef6f4845c9db67e0a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/656.c4dc8222482db230e38e.js` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/656.c4dc8222482db230e38e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/714.4dee3c5425bce6321038.js` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/714.4dee3c5425bce6321038.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/747.e74bd68dc9f322227641.js` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/747.e74bd68dc9f322227641.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/remoteEntry.cbb353a2353963df4b09.js` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/remoteEntry.38da920ab6234bb8b971.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -120,15 +120,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (i("downshift", "8.3.2", (() => Promise.all([j.e(714), j.e(271)]).then((() => () => j(714))))), i("jupyterlab-pachyderm", "2.9.4", (() => Promise.all([j.e(656), j.e(271), j.e(576)]).then((() => () => j(1777))))), i("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), i("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), i("yaml", "0", (() => j.e(357).then((() => () => j(357)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("downshift", "8.3.2", (() => Promise.all([j.e(714), j.e(271)]).then((() => () => j(714))))), i("jupyterlab-pachyderm", "2.9.5", (() => Promise.all([j.e(656), j.e(271), j.e(576)]).then((() => () => j(1777))))), i("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), i("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), i("yaml", "0", (() => j.e(357).then((() => () => j(357)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/labextension/static/third-party-licenses.json` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/pfs_manager.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/pfs_manager.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/pps_client.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/pps_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/conftest.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/setup_large_repo.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/setup_large_repo.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/test_config.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/test_integrations.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm/tests/test_pps.py` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm/tests/test_pps.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm.egg-info/PKG-INFO` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_pachyderm
-Version: 2.9.4
+Version: 2.9.5
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.9.4/jupyterlab_pachyderm.egg-info/SOURCES.txt` & `jupyterlab_pachyderm-2.9.5/jupyterlab_pachyderm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 jupyterlab_pachyderm/labextension/static/576.391ef6f4845c9db67e0a.js
 jupyterlab_pachyderm/labextension/static/656.c4dc8222482db230e38e.js
 jupyterlab_pachyderm/labextension/static/656.c4dc8222482db230e38e.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
 jupyterlab_pachyderm/labextension/static/714.4dee3c5425bce6321038.js
 jupyterlab_pachyderm/labextension/static/714.4dee3c5425bce6321038.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/747.e74bd68dc9f322227641.js
-jupyterlab_pachyderm/labextension/static/remoteEntry.cbb353a2353963df4b09.js
+jupyterlab_pachyderm/labextension/static/remoteEntry.38da920ab6234bb8b971.js
 jupyterlab_pachyderm/labextension/static/style.js
 jupyterlab_pachyderm/labextension/static/third-party-licenses.json
 jupyterlab_pachyderm/tests/__init__.py
 jupyterlab_pachyderm/tests/conftest.py
 jupyterlab_pachyderm/tests/setup_large_repo.py
 jupyterlab_pachyderm/tests/test_config.py
 jupyterlab_pachyderm/tests/test_integrations.py
```

### Comparing `jupyterlab_pachyderm-2.9.4/package.json` & `jupyterlab_pachyderm-2.9.5/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.9.5'"}*

```diff
@@ -130,9 +130,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.9.4"
+    "version": "2.9.5"
 }
```

### Comparing `jupyterlab_pachyderm-2.9.4/pyproject.toml` & `jupyterlab_pachyderm-2.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/setup.cfg` & `jupyterlab_pachyderm-2.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/setup.py` & `jupyterlab_pachyderm-2.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/handler.ts` & `jupyterlab_pachyderm-2.9.5/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/examples/__test__/examples.test.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/examples/__test__/examples.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/examples/examples.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/examples/examples.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap` & `jupyterlab_pachyderm-2.9.5/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/help/__tests__/help.test.ts` & `jupyterlab_pachyderm-2.9.5/src/plugins/help/__tests__/help.test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/help/help.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/help/help.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/__tests__/api.test.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/__tests__/api.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/__tests__/mount.test.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/__tests__/mount.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/api.ts` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/api.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Config/Config.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Config/Config.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Config/__tests__/Config.test.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Config/__tests__/Config.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Config/hooks/useConfig.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Config/hooks/useConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Datum/Datum.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Datum/Datum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Datum/hooks/useDatum.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Datum/hooks/useDatum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Explore/Explore.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Explore/Explore.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/FullPageError/FullPageError.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/FullPageError/FullPageError.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Pipeline/Pipeline.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Pipeline/Pipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/customFileBrowser.ts` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/customFileBrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/index.ts` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/mount.css` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/mount.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/mount.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/mount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/mountDrive.ts` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/mountDrive.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/pollMounts.ts` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/pollMounts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/mount/types.ts` & `jupyterlab_pachyderm-2.9.5/src/plugins/mount/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/telemetry/__tests__/telemetry.test.tsx` & `jupyterlab_pachyderm-2.9.5/src/plugins/telemetry/__tests__/telemetry.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/plugins/telemetry/telemetry.ts` & `jupyterlab_pachyderm-2.9.5/src/plugins/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/utils/components/Circle/Circle.tsx` & `jupyterlab_pachyderm-2.9.5/src/utils/components/Circle/Circle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/utils/components/DropdownCombobox/DropdownCombobox.tsx` & `jupyterlab_pachyderm-2.9.5/src/utils/components/DropdownCombobox/DropdownCombobox.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/utils/components/DropdownCombobox/__tests__/DropdownCombobox.test.tsx` & `jupyterlab_pachyderm-2.9.5/src/utils/components/DropdownCombobox/__tests__/DropdownCombobox.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/utils/components/LoadingDots/loadingDots.css` & `jupyterlab_pachyderm-2.9.5/src/utils/components/LoadingDots/loadingDots.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/utils/components/Svgs/GenericError.js` & `jupyterlab_pachyderm-2.9.5/src/utils/components/Svgs/GenericError.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/utils/components/Svgs/KubernetesElephant.js` & `jupyterlab_pachyderm-2.9.5/src/utils/components/Svgs/KubernetesElephant.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/utils/components/Svgs/PachydermLogo.js` & `jupyterlab_pachyderm-2.9.5/src/utils/components/Svgs/PachydermLogo.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/utils/components/Svgs/StatusWarning.js` & `jupyterlab_pachyderm-2.9.5/src/utils/components/Svgs/StatusWarning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/src/utils/icons.ts` & `jupyterlab_pachyderm-2.9.5/src/utils/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/style/base.css` & `jupyterlab_pachyderm-2.9.5/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/style/components/button.css` & `jupyterlab_pachyderm-2.9.5/style/components/button.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/style/icons/file.svg` & `jupyterlab_pachyderm-2.9.5/style/icons/file.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/style/icons/info.svg` & `jupyterlab_pachyderm-2.9.5/style/icons/info.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/style/icons/mount-logo.svg` & `jupyterlab_pachyderm-2.9.5/style/icons/mount-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.9.4/style/icons/repo.svg` & `jupyterlab_pachyderm-2.9.5/style/icons/repo.svg`

 * *Files identical despite different names*

