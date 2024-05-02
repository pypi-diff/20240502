# Comparing `tmp/nonecorn-0.16.0.dev3.tar.gz` & `tmp/nonecorn-0.16.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonecorn-0.16.0.dev3.tar", last modified: Mon Jan 15 11:42:10 2024, max compression
+gzip compressed data, was "nonecorn-0.16.0.dev4.tar", last modified: Thu May  2 05:31:32 2024, max compression
```

## Comparing `nonecorn-0.16.0.dev3.tar` & `nonecorn-0.16.0.dev4.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.222128 nonecorn-0.16.0.dev3/
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.087918 nonecorn-0.16.0.dev3/.github/
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.107522 nonecorn-0.16.0.dev3/.github/workflows/
--rw-rw-rw-   0        0        0     3183 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev3/.github/workflows/ci.yml
--rw-rw-rw-   0        0        0      847 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev3/.github/workflows/publish.yml
--rw-rw-rw-   0        0        0      200 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev3/.gitignore
--rw-rw-rw-   0        0        0      215 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev3/.readthedocs.yaml
--rw-rw-rw-   0        0        0    21466 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1072 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/LICENSE
--rw-rw-rw-   0        0        0       30 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/MANIFEST.in
--rw-rw-rw-   0        0        0     4929 2024-01-15 11:42:10.222632 nonecorn-0.16.0.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     3796 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev3/README.rst
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.112046 nonecorn-0.16.0.dev3/artwork/
--rw-rw-rw-   0        0        0      560 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/artwork/LICENSE
--rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/artwork/logo.png
--rw-rw-rw-   0        0        0    19020 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/artwork/logo.svg
--rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/artwork/logo_small.png
--rw-rw-rw-   0        0        0     5947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/artwork/logo_small.svg
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.089426 nonecorn-0.16.0.dev3/compliance/
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.115062 nonecorn-0.16.0.dev3/compliance/autobahn/
--rw-rw-rw-   0        0        0      279 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/compliance/autobahn/fuzzingclient.json
--rw-rw-rw-   0        0        0      782 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/compliance/autobahn/server.py
--rw-rw-rw-   0        0        0      262 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/compliance/autobahn/summarise.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.118078 nonecorn-0.16.0.dev3/compliance/h2spec/
--rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/compliance/h2spec/cert.pem
--rw-rw-rw-   0        0        0     3324 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/compliance/h2spec/key.pem
--rw-rw-rw-   0        0        0      899 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/compliance/h2spec/server.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.122099 nonecorn-0.16.0.dev3/docs/
--rw-rw-rw-   0        0        0      630 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.123607 nonecorn-0.16.0.dev3/docs/_static/
--rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/_static/logo.png
--rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/_static/logo_small.png
--rw-rw-rw-   0        0        0     5624 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/docs/conf.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.131650 nonecorn-0.16.0.dev3/docs/discussion/
--rw-rw-rw-   0        0        0      728 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/discussion/backpressure.rst
--rw-rw-rw-   0        0        0     2116 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/discussion/closing.rst
--rw-rw-rw-   0        0        0      331 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/discussion/design_choices.rst
--rw-rw-rw-   0        0        0     7278 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev3/docs/discussion/dos_mitigations.rst
--rw-rw-rw-   0        0        0     1335 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev3/docs/discussion/flow.rst
--rw-rw-rw-   0        0        0     1479 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/discussion/http2.rst
--rw-rw-rw-   0        0        0      201 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev3/docs/discussion/index.rst
--rw-rw-rw-   0        0        0      705 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/discussion/workers.rst
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.142708 nonecorn-0.16.0.dev3/docs/how_to_guides/
--rw-rw-rw-   0        0        0     3444 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/api_usage.rst
--rw-rw-rw-   0        0        0     1322 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/binds.rst
--rw-rw-rw-   0        0        0    12293 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/configuring.rst
--rw-rw-rw-   0        0        0     1396 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/dispatch_apps.rst
--rw-rw-rw-   0        0        0     1947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/http_https_redirect.rst
--rw-rw-rw-   0        0        0      270 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/index.rst
--rw-rw-rw-   0        0        0     2741 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/logging.rst
--rw-rw-rw-   0        0        0     1347 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/proxy_fix.rst
--rw-rw-rw-   0        0        0      534 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/server_names.rst
--rw-rw-rw-   0        0        0     1274 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/statsd.rst
--rw-rw-rw-   0        0        0     1211 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev3/docs/how_to_guides/wsgi_apps.rst
--rw-rw-rw-   0        0        0     1204 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/index.rst
--rwxrwxrwx   0        0        0      807 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/make.bat
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.144719 nonecorn-0.16.0.dev3/docs/reference/
--rw-rw-rw-   0        0        0      112 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/reference/api.rst
--rw-rw-rw-   0        0        0       80 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/reference/index.rst
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.148740 nonecorn-0.16.0.dev3/docs/tutorials/
--rw-rw-rw-   0        0        0      122 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/tutorials/index.rst
--rw-rw-rw-   0        0        0      231 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev3/docs/tutorials/installation.rst
--rw-rw-rw-   0        0        0      859 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/tutorials/quickstart.rst
--rw-rw-rw-   0        0        0      606 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/docs/tutorials/usage.rst
--rw-rw-rw-   0        0        0     3127 2024-01-07 05:58:04.000000 nonecorn-0.16.0.dev3/pyproject.toml
--rw-rw-rw-   0        0        0      910 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/readme_zh.markdown
--rw-rw-rw-   0        0        0      156 2024-01-15 11:42:10.223134 nonecorn-0.16.0.dev3/setup.cfg
--rw-rw-rw-   0        0        0     2242 2024-01-07 05:58:04.000000 nonecorn-0.16.0.dev3/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.093447 nonecorn-0.16.0.dev3/src/
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.159799 nonecorn-0.16.0.dev3/src/hypercorn/
--rw-rw-rw-   0        0        0       91 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/src/hypercorn/__init__.py
--rw-rw-rw-   0        0        0    11280 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/__main__.py
--rw-rw-rw-   0        0        0     5671 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev3/src/hypercorn/app_wrappers.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.166836 nonecorn-0.16.0.dev3/src/hypercorn/asyncio/
--rw-rw-rw-   0        0        0     1490 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev3/src/hypercorn/asyncio/__init__.py
--rw-rw-rw-   0        0        0     4069 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/src/hypercorn/asyncio/lifespan.py
--rw-rw-rw-   0        0        0     8241 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/asyncio/run.py
--rw-rw-rw-   0        0        0      795 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev3/src/hypercorn/asyncio/statsd.py
--rw-rw-rw-   0        0        0     2305 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev3/src/hypercorn/asyncio/task_group.py
--rw-rw-rw-   0        0        0     6455 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev3/src/hypercorn/asyncio/tcp_server.py
--rw-rw-rw-   0        0        0     3125 2023-12-03 16:27:34.000000 nonecorn-0.16.0.dev3/src/hypercorn/asyncio/udp_server.py
--rw-rw-rw-   0        0        0     1223 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/asyncio/worker_context.py
--rw-rw-rw-   0        0        0    14242 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/config.py
--rw-rw-rw-   0        0        0      557 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/src/hypercorn/events.py
--rw-rw-rw-   0        0        0     7587 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev3/src/hypercorn/logging.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.171360 nonecorn-0.16.0.dev3/src/hypercorn/middleware/
--rw-rw-rw-   0        0        0      415 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev3/src/hypercorn/middleware/__init__.py
--rw-rw-rw-   0        0        0     4414 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/src/hypercorn/middleware/dispatcher.py
--rw-rw-rw-   0        0        0     2686 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/src/hypercorn/middleware/http_to_https.py
--rw-rw-rw-   0        0        0     2772 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev3/src/hypercorn/middleware/proxy_fix.py
--rw-rw-rw-   0        0        0     1538 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/src/hypercorn/middleware/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.178900 nonecorn-0.16.0.dev3/src/hypercorn/protocol/
--rw-rw-rw-   0        0        0     3235 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/src/hypercorn/protocol/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/src/hypercorn/protocol/events.py
--rw-rw-rw-   0        0        0    13933 2024-01-15 10:30:30.000000 nonecorn-0.16.0.dev3/src/hypercorn/protocol/h11.py
--rw-rw-rw-   0        0        0    17131 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/protocol/h2.py
--rw-rw-rw-   0        0        0     6125 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/protocol/h3.py
--rw-rw-rw-   0        0        0    14778 2023-12-06 13:40:08.000000 nonecorn-0.16.0.dev3/src/hypercorn/protocol/http_stream.py
--rw-rw-rw-   0        0        0     5346 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/src/hypercorn/protocol/quic.py
--rw-rw-rw-   0        0        0    19463 2024-01-15 10:31:48.000000 nonecorn-0.16.0.dev3/src/hypercorn/protocol/ws_stream.py
--rw-rw-rw-   0        0        0        8 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/src/hypercorn/py.typed
--rw-rw-rw-   0        0        0     4993 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/run.py
--rw-rw-rw-   0        0        0     3927 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/src/hypercorn/statsd.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.186439 nonecorn-0.16.0.dev3/src/hypercorn/trio/
--rw-rw-rw-   0        0        0     1611 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev3/src/hypercorn/trio/__init__.py
--rw-rw-rw-   0        0        0     3726 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/src/hypercorn/trio/lifespan.py
--rw-rw-rw-   0        0        0     5105 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/trio/run.py
--rw-rw-rw-   0        0        0      509 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/src/hypercorn/trio/statsd.py
--rw-rw-rw-   0        0        0     2503 2023-07-08 16:37:15.000000 nonecorn-0.16.0.dev3/src/hypercorn/trio/task_group.py
--rw-rw-rw-   0        0        0     5326 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/src/hypercorn/trio/tcp_server.py
--rw-rw-rw-   0        0        0     1678 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev3/src/hypercorn/trio/udp_server.py
--rw-rw-rw-   0        0        0     1211 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/trio/worker_context.py
--rw-rw-rw-   0        0        0     8233 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/typing.py
--rw-rw-rw-   0        0        0     9646 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/utils.py
--rw-rw-rw-   0        0        0     6391 2023-12-03 11:38:38.000000 nonecorn-0.16.0.dev3/src/hypercorn/workers.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.191969 nonecorn-0.16.0.dev3/src/nonecorn.egg-info/
--rw-rw-rw-   0        0        0     4929 2024-01-15 11:42:09.000000 nonecorn-0.16.0.dev3/src/nonecorn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3694 2024-01-15 11:42:10.000000 nonecorn-0.16.0.dev3/src/nonecorn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-15 11:42:09.000000 nonecorn-0.16.0.dev3/src/nonecorn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-01-15 11:42:09.000000 nonecorn-0.16.0.dev3/src/nonecorn.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      273 2024-01-15 11:42:09.000000 nonecorn-0.16.0.dev3/src/nonecorn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-15 11:42:09.000000 nonecorn-0.16.0.dev3/src/nonecorn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.200012 nonecorn-0.16.0.dev3/tests/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.204536 nonecorn-0.16.0.dev3/tests/assets/
--rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/assets/cert.pem
--rw-rw-rw-   0        0        0      147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/assets/config.py
--rw-rw-rw-   0        0        0       81 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/assets/config.toml
--rw-rw-rw-   0        0        0      217 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/assets/config_ssl.py
--rw-rw-rw-   0        0        0     3320 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/assets/key.pem
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.210568 nonecorn-0.16.0.dev3/tests/asyncio/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/asyncio/__init__.py
--rw-rw-rw-   0        0        0     1705 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/asyncio/helpers.py
--rw-rw-rw-   0        0        0     4038 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/tests/asyncio/test_keep_alive.py
--rw-rw-rw-   0        0        0     2506 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/asyncio/test_lifespan.py
--rw-rw-rw-   0        0        0     8617 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/tests/asyncio/test_sanity.py
--rw-rw-rw-   0        0        0     1509 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev3/tests/asyncio/test_task_group.py
--rw-rw-rw-   0        0        0     1606 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/tests/asyncio/test_tcp_server.py
--rw-rw-rw-   0        0        0      897 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/conftest.py
--rw-rw-rw-   0        0        0     4396 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev3/tests/helpers.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.214086 nonecorn-0.16.0.dev3/tests/middleware/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/middleware/__init__.py
--rw-rw-rw-   0        0        0     3309 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev3/tests/middleware/test_dispatcher.py
--rw-rw-rw-   0        0        0     4886 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/middleware/test_http_to_https.py
--rw-rw-rw-   0        0        0     2175 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev3/tests/middleware/test_proxy_fix.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.218108 nonecorn-0.16.0.dev3/tests/protocol/
--rw-rw-rw-   0        0        0    15251 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/tests/protocol/test_h11.py
--rw-rw-rw-   0        0        0     3612 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/tests/protocol/test_h2.py
--rw-rw-rw-   0        0        0    10000 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/tests/protocol/test_http_stream.py
--rw-rw-rw-   0        0        0    17458 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/tests/protocol/test_ws_stream.py
--rw-rw-rw-   0        0        0     2983 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/test___main__.py
--rw-rw-rw-   0        0        0     6111 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev3/tests/test_app_wrappers.py
--rw-rw-rw-   0        0        0     5183 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/test_config.py
--rw-rw-rw-   0        0        0     4147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/test_logging.py
--rw-rw-rw-   0        0        0     2223 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-15 11:42:10.221626 nonecorn-0.16.0.dev3/tests/trio/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/trio/__init__.py
--rw-rw-rw-   0        0        0     3980 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/tests/trio/test_keep_alive.py
--rw-rw-rw-   0        0        0     1258 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev3/tests/trio/test_lifespan.py
--rw-rw-rw-   0        0        0     8241 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev3/tests/trio/test_sanity.py
--rw-rw-rw-   0        0        0     1245 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev3/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.310114 nonecorn-0.16.0.dev4/
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.211091 nonecorn-0.16.0.dev4/.github/
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.226095 nonecorn-0.16.0.dev4/.github/workflows/
+-rw-rw-rw-   0        0        0     3183 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/.github/workflows/ci.yml
+-rw-rw-rw-   0        0        0      847 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev4/.github/workflows/publish.yml
+-rw-rw-rw-   0        0        0      200 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev4/.gitignore
+-rw-rw-rw-   0        0        0      215 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev4/.readthedocs.yaml
+-rw-rw-rw-   0        0        0    21466 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1072 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4929 2024-05-02 05:31:32.310114 nonecorn-0.16.0.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     3796 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev4/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.229096 nonecorn-0.16.0.dev4/artwork/
+-rw-rw-rw-   0        0        0      560 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/artwork/LICENSE
+-rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/artwork/logo.png
+-rw-rw-rw-   0        0        0    19020 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/artwork/logo.svg
+-rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/artwork/logo_small.png
+-rw-rw-rw-   0        0        0     5947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/artwork/logo_small.svg
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.212092 nonecorn-0.16.0.dev4/compliance/
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.231096 nonecorn-0.16.0.dev4/compliance/autobahn/
+-rw-rw-rw-   0        0        0      279 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/compliance/autobahn/fuzzingclient.json
+-rw-rw-rw-   0        0        0      782 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/compliance/autobahn/server.py
+-rw-rw-rw-   0        0        0      262 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/compliance/autobahn/summarise.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.233096 nonecorn-0.16.0.dev4/compliance/h2spec/
+-rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/compliance/h2spec/cert.pem
+-rw-rw-rw-   0        0        0     3324 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/compliance/h2spec/key.pem
+-rw-rw-rw-   0        0        0      899 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/compliance/h2spec/server.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.236098 nonecorn-0.16.0.dev4/docs/
+-rw-rw-rw-   0        0        0      630 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.237098 nonecorn-0.16.0.dev4/docs/_static/
+-rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/_static/logo.png
+-rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/_static/logo_small.png
+-rw-rw-rw-   0        0        0     5624 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/docs/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.244099 nonecorn-0.16.0.dev4/docs/discussion/
+-rw-rw-rw-   0        0        0      728 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/discussion/backpressure.rst
+-rw-rw-rw-   0        0        0     2116 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/discussion/closing.rst
+-rw-rw-rw-   0        0        0      331 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/discussion/design_choices.rst
+-rw-rw-rw-   0        0        0     7278 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev4/docs/discussion/dos_mitigations.rst
+-rw-rw-rw-   0        0        0     1335 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev4/docs/discussion/flow.rst
+-rw-rw-rw-   0        0        0     1479 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/discussion/http2.rst
+-rw-rw-rw-   0        0        0      201 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev4/docs/discussion/index.rst
+-rw-rw-rw-   0        0        0      705 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/discussion/workers.rst
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.251101 nonecorn-0.16.0.dev4/docs/how_to_guides/
+-rw-rw-rw-   0        0        0     3444 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/api_usage.rst
+-rw-rw-rw-   0        0        0     1322 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/binds.rst
+-rw-rw-rw-   0        0        0    12293 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/configuring.rst
+-rw-rw-rw-   0        0        0     1396 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/dispatch_apps.rst
+-rw-rw-rw-   0        0        0     1947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/http_https_redirect.rst
+-rw-rw-rw-   0        0        0      270 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/index.rst
+-rw-rw-rw-   0        0        0     2741 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/logging.rst
+-rw-rw-rw-   0        0        0     1347 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/proxy_fix.rst
+-rw-rw-rw-   0        0        0      534 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/server_names.rst
+-rw-rw-rw-   0        0        0     1274 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/statsd.rst
+-rw-rw-rw-   0        0        0     1211 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev4/docs/how_to_guides/wsgi_apps.rst
+-rw-rw-rw-   0        0        0     1204 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/index.rst
+-rwxrwxrwx   0        0        0      807 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/make.bat
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.253101 nonecorn-0.16.0.dev4/docs/reference/
+-rw-rw-rw-   0        0        0      112 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/reference/api.rst
+-rw-rw-rw-   0        0        0       80 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/reference/index.rst
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.255102 nonecorn-0.16.0.dev4/docs/tutorials/
+-rw-rw-rw-   0        0        0      122 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/tutorials/index.rst
+-rw-rw-rw-   0        0        0      231 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev4/docs/tutorials/installation.rst
+-rw-rw-rw-   0        0        0      859 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/tutorials/quickstart.rst
+-rw-rw-rw-   0        0        0      606 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/docs/tutorials/usage.rst
+-rw-rw-rw-   0        0        0     3127 2024-05-02 05:31:29.000000 nonecorn-0.16.0.dev4/pyproject.toml
+-rw-rw-rw-   0        0        0      910 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/readme_zh.markdown
+-rw-rw-rw-   0        0        0      156 2024-05-02 05:31:32.311115 nonecorn-0.16.0.dev4/setup.cfg
+-rw-rw-rw-   0        0        0     2242 2024-05-02 05:31:29.000000 nonecorn-0.16.0.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.216092 nonecorn-0.16.0.dev4/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.263104 nonecorn-0.16.0.dev4/src/hypercorn/
+-rw-rw-rw-   0        0        0       91 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/src/hypercorn/__init__.py
+-rw-rw-rw-   0        0        0    11280 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/__main__.py
+-rw-rw-rw-   0        0        0     5675 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/src/hypercorn/app_wrappers.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.269106 nonecorn-0.16.0.dev4/src/hypercorn/asyncio/
+-rw-rw-rw-   0        0        0     1490 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev4/src/hypercorn/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     4069 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/src/hypercorn/asyncio/lifespan.py
+-rw-rw-rw-   0        0        0     8241 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/asyncio/run.py
+-rw-rw-rw-   0        0        0      795 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev4/src/hypercorn/asyncio/statsd.py
+-rw-rw-rw-   0        0        0     2305 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev4/src/hypercorn/asyncio/task_group.py
+-rw-rw-rw-   0        0        0     6455 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev4/src/hypercorn/asyncio/tcp_server.py
+-rw-rw-rw-   0        0        0     3125 2023-12-03 16:27:34.000000 nonecorn-0.16.0.dev4/src/hypercorn/asyncio/udp_server.py
+-rw-rw-rw-   0        0        0     1223 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/asyncio/worker_context.py
+-rw-rw-rw-   0        0        0    14242 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/config.py
+-rw-rw-rw-   0        0        0      557 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/src/hypercorn/events.py
+-rw-rw-rw-   0        0        0     7587 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev4/src/hypercorn/logging.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.273107 nonecorn-0.16.0.dev4/src/hypercorn/middleware/
+-rw-rw-rw-   0        0        0      415 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev4/src/hypercorn/middleware/__init__.py
+-rw-rw-rw-   0        0        0     4414 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/src/hypercorn/middleware/dispatcher.py
+-rw-rw-rw-   0        0        0     2686 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/src/hypercorn/middleware/http_to_https.py
+-rw-rw-rw-   0        0        0     2772 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev4/src/hypercorn/middleware/proxy_fix.py
+-rw-rw-rw-   0        0        0     1538 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/src/hypercorn/middleware/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.278108 nonecorn-0.16.0.dev4/src/hypercorn/protocol/
+-rw-rw-rw-   0        0        0     3235 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/src/hypercorn/protocol/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/src/hypercorn/protocol/events.py
+-rw-rw-rw-   0        0        0    13933 2024-01-15 10:30:30.000000 nonecorn-0.16.0.dev4/src/hypercorn/protocol/h11.py
+-rw-rw-rw-   0        0        0    17131 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/protocol/h2.py
+-rw-rw-rw-   0        0        0     6125 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/protocol/h3.py
+-rw-rw-rw-   0        0        0    14834 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/src/hypercorn/protocol/http_stream.py
+-rw-rw-rw-   0        0        0     5346 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/src/hypercorn/protocol/quic.py
+-rw-rw-rw-   0        0        0    19463 2024-01-15 10:31:48.000000 nonecorn-0.16.0.dev4/src/hypercorn/protocol/ws_stream.py
+-rw-rw-rw-   0        0        0        8 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/src/hypercorn/py.typed
+-rw-rw-rw-   0        0        0     4993 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/run.py
+-rw-rw-rw-   0        0        0     3927 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/src/hypercorn/statsd.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.284109 nonecorn-0.16.0.dev4/src/hypercorn/trio/
+-rw-rw-rw-   0        0        0     1611 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev4/src/hypercorn/trio/__init__.py
+-rw-rw-rw-   0        0        0     3726 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/src/hypercorn/trio/lifespan.py
+-rw-rw-rw-   0        0        0     5105 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/trio/run.py
+-rw-rw-rw-   0        0        0      509 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/src/hypercorn/trio/statsd.py
+-rw-rw-rw-   0        0        0     2503 2023-07-08 16:37:15.000000 nonecorn-0.16.0.dev4/src/hypercorn/trio/task_group.py
+-rw-rw-rw-   0        0        0     5326 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/src/hypercorn/trio/tcp_server.py
+-rw-rw-rw-   0        0        0     1678 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev4/src/hypercorn/trio/udp_server.py
+-rw-rw-rw-   0        0        0     1211 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/trio/worker_context.py
+-rw-rw-rw-   0        0        0     8256 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/src/hypercorn/typing.py
+-rw-rw-rw-   0        0        0     9646 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/utils.py
+-rw-rw-rw-   0        0        0     6391 2023-12-03 11:38:38.000000 nonecorn-0.16.0.dev4/src/hypercorn/workers.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.288110 nonecorn-0.16.0.dev4/src/nonecorn.egg-info/
+-rw-rw-rw-   0        0        0     4929 2024-05-02 05:31:31.000000 nonecorn-0.16.0.dev4/src/nonecorn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3694 2024-05-02 05:31:32.000000 nonecorn-0.16.0.dev4/src/nonecorn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 05:31:31.000000 nonecorn-0.16.0.dev4/src/nonecorn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-02 05:31:31.000000 nonecorn-0.16.0.dev4/src/nonecorn.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      273 2024-05-02 05:31:31.000000 nonecorn-0.16.0.dev4/src/nonecorn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-02 05:31:31.000000 nonecorn-0.16.0.dev4/src/nonecorn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.293111 nonecorn-0.16.0.dev4/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.297112 nonecorn-0.16.0.dev4/tests/assets/
+-rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/assets/cert.pem
+-rw-rw-rw-   0        0        0      147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/assets/config.py
+-rw-rw-rw-   0        0        0       81 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/assets/config.toml
+-rw-rw-rw-   0        0        0      217 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/assets/config_ssl.py
+-rw-rw-rw-   0        0        0     3320 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/assets/key.pem
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.301113 nonecorn-0.16.0.dev4/tests/asyncio/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     1705 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/asyncio/helpers.py
+-rw-rw-rw-   0        0        0     4075 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/tests/asyncio/test_keep_alive.py
+-rw-rw-rw-   0        0        0     2654 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/tests/asyncio/test_lifespan.py
+-rw-rw-rw-   0        0        0     8765 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/tests/asyncio/test_sanity.py
+-rw-rw-rw-   0        0        0     1571 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/tests/asyncio/test_task_group.py
+-rw-rw-rw-   0        0        0     1680 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/tests/asyncio/test_tcp_server.py
+-rw-rw-rw-   0        0        0      897 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/conftest.py
+-rw-rw-rw-   0        0        0     4396 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev4/tests/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.304113 nonecorn-0.16.0.dev4/tests/middleware/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/middleware/__init__.py
+-rw-rw-rw-   0        0        0     3309 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev4/tests/middleware/test_dispatcher.py
+-rw-rw-rw-   0        0        0     4886 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/middleware/test_http_to_https.py
+-rw-rw-rw-   0        0        0     2175 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev4/tests/middleware/test_proxy_fix.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.307114 nonecorn-0.16.0.dev4/tests/protocol/
+-rw-rw-rw-   0        0        0    15278 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/tests/protocol/test_h11.py
+-rw-rw-rw-   0        0        0     3612 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/tests/protocol/test_h2.py
+-rw-rw-rw-   0        0        0    10000 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/tests/protocol/test_http_stream.py
+-rw-rw-rw-   0        0        0    17493 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/tests/protocol/test_ws_stream.py
+-rw-rw-rw-   0        0        0     2983 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/test___main__.py
+-rw-rw-rw-   0        0        0     6111 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev4/tests/test_app_wrappers.py
+-rw-rw-rw-   0        0        0     5687 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/tests/test_config.py
+-rw-rw-rw-   0        0        0     4147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/test_logging.py
+-rw-rw-rw-   0        0        0     2223 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 05:31:32.309114 nonecorn-0.16.0.dev4/tests/trio/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev4/tests/trio/__init__.py
+-rw-rw-rw-   0        0        0     3980 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/tests/trio/test_keep_alive.py
+-rw-rw-rw-   0        0        0     1661 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev4/tests/trio/test_lifespan.py
+-rw-rw-rw-   0        0        0     8241 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev4/tests/trio/test_sanity.py
+-rw-rw-rw-   0        0        0     1245 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev4/tox.ini
```

### Comparing `nonecorn-0.16.0.dev3/.github/workflows/ci.yml` & `nonecorn-0.16.0.dev4/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
           - {name: '3.8', python: '3.8', tox: py38}
           - {name: 'format', python: '3.12', tox: format}
           - {name: 'mypy', python: '3.12', tox: mypy}
           - {name: 'pep8', python: '3.12', tox: pep8}
           - {name: 'package', python: '3.12', tox: package}
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
 
       - name: update pip
         run: |
           pip install -U wheel
           pip install -U setuptools
@@ -48,17 +48,17 @@
       fail-fast: false
       matrix:
         include:
           - {name: 'asyncio', worker: 'asyncio'}
           - {name: 'trio', worker: 'trio'}
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.12"
 
       - name: update pip
         run: |
           pip install -U wheel
           pip install -U setuptools
@@ -84,17 +84,17 @@
       fail-fast: false
       matrix:
         include:
           - {name: 'asyncio', worker: 'asyncio'}
           - {name: 'trio', worker: 'trio'}
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.10"
 
       - name: update pip
         run: |
           pip install -U wheel
           pip install -U setuptools
```

### Comparing `nonecorn-0.16.0.dev3/.github/workflows/publish.yml` & `nonecorn-0.16.0.dev4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/CHANGELOG.rst` & `nonecorn-0.16.0.dev4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/LICENSE` & `nonecorn-0.16.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/PKG-INFO` & `nonecorn-0.16.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonecorn
-Version: 0.16.0.dev3
+Version: 0.16.0.dev4
 Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
 Home-page: https://gitlab.com/pgjones/hypercorn/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nonecorn-0.16.0.dev3/README.rst` & `nonecorn-0.16.0.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/artwork/LICENSE` & `nonecorn-0.16.0.dev4/artwork/LICENSE`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/artwork/logo.png` & `nonecorn-0.16.0.dev4/artwork/logo.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/artwork/logo.svg` & `nonecorn-0.16.0.dev4/artwork/logo.svg`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/artwork/logo_small.png` & `nonecorn-0.16.0.dev4/artwork/logo_small.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/artwork/logo_small.svg` & `nonecorn-0.16.0.dev4/artwork/logo_small.svg`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/compliance/autobahn/server.py` & `nonecorn-0.16.0.dev4/compliance/autobahn/server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/compliance/h2spec/cert.pem` & `nonecorn-0.16.0.dev4/compliance/h2spec/cert.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/compliance/h2spec/key.pem` & `nonecorn-0.16.0.dev4/compliance/h2spec/key.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/compliance/h2spec/server.py` & `nonecorn-0.16.0.dev4/compliance/h2spec/server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/Makefile` & `nonecorn-0.16.0.dev4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/_static/logo.png` & `nonecorn-0.16.0.dev4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/_static/logo_small.png` & `nonecorn-0.16.0.dev4/docs/_static/logo_small.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/conf.py` & `nonecorn-0.16.0.dev4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/discussion/backpressure.rst` & `nonecorn-0.16.0.dev4/docs/discussion/backpressure.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/discussion/closing.rst` & `nonecorn-0.16.0.dev4/docs/discussion/closing.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/discussion/dos_mitigations.rst` & `nonecorn-0.16.0.dev4/docs/discussion/dos_mitigations.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/discussion/flow.rst` & `nonecorn-0.16.0.dev4/docs/discussion/flow.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/discussion/http2.rst` & `nonecorn-0.16.0.dev4/docs/discussion/http2.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/discussion/workers.rst` & `nonecorn-0.16.0.dev4/docs/discussion/workers.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/how_to_guides/api_usage.rst` & `nonecorn-0.16.0.dev4/docs/how_to_guides/api_usage.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/how_to_guides/binds.rst` & `nonecorn-0.16.0.dev4/docs/how_to_guides/binds.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/how_to_guides/configuring.rst` & `nonecorn-0.16.0.dev4/docs/how_to_guides/configuring.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/how_to_guides/dispatch_apps.rst` & `nonecorn-0.16.0.dev4/docs/how_to_guides/dispatch_apps.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/how_to_guides/http_https_redirect.rst` & `nonecorn-0.16.0.dev4/docs/how_to_guides/http_https_redirect.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/how_to_guides/logging.rst` & `nonecorn-0.16.0.dev4/docs/how_to_guides/logging.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/how_to_guides/proxy_fix.rst` & `nonecorn-0.16.0.dev4/docs/how_to_guides/proxy_fix.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/how_to_guides/server_names.rst` & `nonecorn-0.16.0.dev4/docs/how_to_guides/server_names.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/how_to_guides/statsd.rst` & `nonecorn-0.16.0.dev4/docs/how_to_guides/statsd.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/how_to_guides/wsgi_apps.rst` & `nonecorn-0.16.0.dev4/docs/how_to_guides/wsgi_apps.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/index.rst` & `nonecorn-0.16.0.dev4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/make.bat` & `nonecorn-0.16.0.dev4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/tutorials/quickstart.rst` & `nonecorn-0.16.0.dev4/docs/tutorials/quickstart.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/docs/tutorials/usage.rst` & `nonecorn-0.16.0.dev4/docs/tutorials/usage.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/pyproject.toml` & `nonecorn-0.16.0.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonecorn"
-version = "0.16.0dev3"
+version = "0.16.0dev4"
 description = "A ASGI Server based on Hyper libraries and inspired by Gunicorn"
 authors = ["pgjones <philip.graham.jones@googlemail.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `nonecorn-0.16.0.dev3/readme_zh.markdown` & `nonecorn-0.16.0.dev4/readme_zh.markdown`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/setup.py` & `nonecorn-0.16.0.dev4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "pytest-cov",
     "pytest-trio",
     "trio",
 ]
 
 setup(
     name="nonecorn",
-    version="0.16.0dev3",
+    version="0.16.0dev4",
     python_requires=">=3.7",
     description="A ASGI Server forked from hypercorn with more extra feature beyond ASGI",
     long_description=long_description,
     url="https://gitlab.com/pgjones/hypercorn/",
     author="P G Jones",
     author_email="philip.graham.jones@googlemail.com",
     license="MIT",
```

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/__main__.py` & `nonecorn-0.16.0.dev4/src/hypercorn/__main__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/app_wrappers.py` & `nonecorn-0.16.0.dev4/src/hypercorn/app_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             exc_info: Optional[Exception] = None,
         ) -> None:
             nonlocal headers, response_started, status_code
 
             raw, _ = status.split(" ", 1)
             status_code = int(raw)
             headers = [
-                (name.lower().encode("ascii"), value.encode("ascii"))
+                (name.lower().encode("latin-1"), value.encode("latin-1"))
                 for name, value in response_headers
             ]
             response_started = True
 
         response_body = self.app(environ, start_response)
 
         if not response_started:
```

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/asyncio/__init__.py` & `nonecorn-0.16.0.dev4/src/hypercorn/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/asyncio/lifespan.py` & `nonecorn-0.16.0.dev4/src/hypercorn/asyncio/lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/asyncio/run.py` & `nonecorn-0.16.0.dev4/src/hypercorn/asyncio/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/asyncio/statsd.py` & `nonecorn-0.16.0.dev4/src/hypercorn/asyncio/statsd.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/asyncio/task_group.py` & `nonecorn-0.16.0.dev4/src/hypercorn/asyncio/task_group.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/asyncio/tcp_server.py` & `nonecorn-0.16.0.dev4/src/hypercorn/asyncio/tcp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/asyncio/udp_server.py` & `nonecorn-0.16.0.dev4/src/hypercorn/asyncio/udp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/asyncio/worker_context.py` & `nonecorn-0.16.0.dev4/src/hypercorn/asyncio/worker_context.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/config.py` & `nonecorn-0.16.0.dev4/src/hypercorn/config.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/events.py` & `nonecorn-0.16.0.dev4/src/hypercorn/events.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/logging.py` & `nonecorn-0.16.0.dev4/src/hypercorn/logging.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/middleware/dispatcher.py` & `nonecorn-0.16.0.dev4/src/hypercorn/middleware/dispatcher.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/middleware/http_to_https.py` & `nonecorn-0.16.0.dev4/src/hypercorn/middleware/http_to_https.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/middleware/proxy_fix.py` & `nonecorn-0.16.0.dev4/src/hypercorn/middleware/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/middleware/wsgi.py` & `nonecorn-0.16.0.dev4/src/hypercorn/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/protocol/__init__.py` & `nonecorn-0.16.0.dev4/src/hypercorn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/protocol/events.py` & `nonecorn-0.16.0.dev4/src/hypercorn/protocol/events.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/protocol/h11.py` & `nonecorn-0.16.0.dev4/src/hypercorn/protocol/h11.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/protocol/h2.py` & `nonecorn-0.16.0.dev4/src/hypercorn/protocol/h2.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/protocol/h3.py` & `nonecorn-0.16.0.dev4/src/hypercorn/protocol/h3.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/protocol/http_stream.py` & `nonecorn-0.16.0.dev4/src/hypercorn/protocol/http_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,16 @@
             await self.app_put(
                 {"type": "http.request", "body": bytes(event.data), "more_body": True}
             )
         elif isinstance(event, EndBody):
             await self.app_put({"type": "http.request", "body": b"", "more_body": False})
         elif isinstance(event, StreamClosed):
             self.closed = True
-            await self.config.log.access(self.scope, None, time() - self.start_time)
+            if self.state != ASGIHTTPState.CLOSED:
+                await self.config.log.access(self.scope, None, time() - self.start_time)
             if self.app_put is not None:
                 await self.app_put({"type": "http.disconnect"})
 
     async def app_send(self, message: Optional[ASGISendEvent]) -> None:
         if message is None:  # ASGI App has finished sending messages
             if not self.closed:
                 # Cleanup if required
```

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/protocol/quic.py` & `nonecorn-0.16.0.dev4/src/hypercorn/protocol/quic.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/protocol/ws_stream.py` & `nonecorn-0.16.0.dev4/src/hypercorn/protocol/ws_stream.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/run.py` & `nonecorn-0.16.0.dev4/src/hypercorn/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/statsd.py` & `nonecorn-0.16.0.dev4/src/hypercorn/statsd.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/trio/__init__.py` & `nonecorn-0.16.0.dev4/src/hypercorn/trio/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/trio/lifespan.py` & `nonecorn-0.16.0.dev4/src/hypercorn/trio/lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/trio/run.py` & `nonecorn-0.16.0.dev4/src/hypercorn/trio/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/trio/task_group.py` & `nonecorn-0.16.0.dev4/src/hypercorn/trio/task_group.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/trio/tcp_server.py` & `nonecorn-0.16.0.dev4/src/hypercorn/trio/tcp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/trio/udp_server.py` & `nonecorn-0.16.0.dev4/src/hypercorn/trio/udp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/trio/worker_context.py` & `nonecorn-0.16.0.dev4/src/hypercorn/trio/worker_context.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/typing.py` & `nonecorn-0.16.0.dev4/src/hypercorn/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -244,112 +244,112 @@
 Framework = Union[ASGIFramework, WSGIFramework]
 
 
 class H2SyncStream(Protocol):
     scope: dict
 
     def data_received(self, data: bytes) -> None:
-        ...
+        pass
 
     def ended(self) -> None:
-        ...
+        pass
 
     def reset(self) -> None:
-        ...
+        pass
 
     def close(self) -> None:
-        ...
+        pass
 
     async def handle_request(
         self,
         event: h2.events.RequestReceived,
         scheme: str,
         client: Tuple[str, int],
         server: Tuple[str, int],
     ) -> None:
-        ...
+        pass
 
 
 class H2AsyncStream(Protocol):
     scope: dict
 
     async def data_received(self, data: bytes) -> None:
-        ...
+        pass
 
     async def ended(self) -> None:
-        ...
+        pass
 
     async def reset(self) -> None:
-        ...
+        pass
 
     async def close(self) -> None:
-        ...
+        pass
 
     async def handle_request(
         self,
         event: h2.events.RequestReceived,
         scheme: str,
         client: Tuple[str, int],
         server: Tuple[str, int],
     ) -> None:
-        ...
+        pass
 
 
 class Event(Protocol):
     def __init__(self) -> None:
-        ...
+        pass
 
     async def clear(self) -> None:
-        ...
+        pass
 
     async def set(self) -> None:
-        ...
+        pass
 
     async def wait(self) -> None:
-        ...
+        pass
 
     def is_set(self) -> bool:
-        ...
+        pass
 
 
 class WorkerContext(Protocol):
     event_class: Type[Event]
     terminate: Event
     terminated: Event
 
     async def mark_request(self) -> None:
-        ...
+        pass
 
     @staticmethod
     async def sleep(wait: Union[float, int]) -> None:
-        ...
+        pass
 
     @staticmethod
     def time() -> float:
-        ...
+        pass
 
 
 class TaskGroup(Protocol):
     async def spawn_app(
         self,
         app: AppWrapper,
         config: Config,
         scope: Scope,
         send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
     ) -> Callable[[ASGIReceiveEvent], Awaitable[None]]:
-        ...
+        pass
 
     def spawn(self, func: Callable, *args: Any) -> None:
-        ...
+        pass
 
     async def __aenter__(self) -> TaskGroup:
-        ...
+        pass
 
     async def __aexit__(self, exc_type: type, exc_value: BaseException, tb: TracebackType) -> None:
-        ...
+        pass
 
 
 class ResponseSummary(TypedDict):
     status: int
     headers: Iterable[Tuple[bytes, bytes]]
 
 
@@ -358,8 +358,8 @@
         self,
         scope: Scope,
         receive: ASGIReceiveCallable,
         send: ASGISendCallable,
         sync_spawn: Callable,
         call_soon: Callable,
     ) -> None:
-        ...
+        pass
```

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/utils.py` & `nonecorn-0.16.0.dev4/src/hypercorn/utils.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/hypercorn/workers.py` & `nonecorn-0.16.0.dev4/src/hypercorn/workers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/src/nonecorn.egg-info/PKG-INFO` & `nonecorn-0.16.0.dev4/src/nonecorn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonecorn
-Version: 0.16.0.dev3
+Version: 0.16.0.dev4
 Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
 Home-page: https://gitlab.com/pgjones/hypercorn/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nonecorn-0.16.0.dev3/src/nonecorn.egg-info/SOURCES.txt` & `nonecorn-0.16.0.dev4/src/nonecorn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/assets/cert.pem` & `nonecorn-0.16.0.dev4/tests/assets/cert.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/assets/key.pem` & `nonecorn-0.16.0.dev4/tests/assets/key.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/asyncio/helpers.py` & `nonecorn-0.16.0.dev4/tests/asyncio/helpers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/asyncio/test_keep_alive.py` & `nonecorn-0.16.0.dev4/tests/asyncio/test_keep_alive.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,17 @@
                 }
             )
             await send({"type": "http.response.body", "body": b"", "more_body": False})
             break
 
 
 @pytest_asyncio.fixture(name="server", scope="function")  # type: ignore[misc]
-async def _server(event_loop: asyncio.AbstractEventLoop) -> AsyncGenerator[TCPServer, None]:
+async def _server() -> AsyncGenerator[TCPServer, None]:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     config = Config()
     config.keep_alive_timeout = KEEP_ALIVE_TIMEOUT
     server = TCPServer(
         ASGIWrapper(slow_framework),
         event_loop,
         config,
         WorkerContext(None),
```

### Comparing `nonecorn-0.16.0.dev3/tests/asyncio/test_lifespan.py` & `nonecorn-0.16.0.dev4/tests/asyncio/test_lifespan.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,51 +16,59 @@
 
 async def no_lifespan_app(scope: Scope, receive: Callable, send: Callable) -> None:
     sleep(0.1)  # Block purposefully
     raise Exception()
 
 
 @pytest.mark.asyncio
-async def test_ensure_no_race_condition(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_ensure_no_race_condition() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     config = Config()
     config.startup_timeout = 0.2
     lifespan = Lifespan(ASGIWrapper(no_lifespan_app), config, event_loop)
     task = event_loop.create_task(lifespan.handle_lifespan())
     await lifespan.wait_for_startup()  # Raises if there is a race condition
     await task
 
 
 @pytest.mark.asyncio
-async def test_startup_timeout_error(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_startup_timeout_error() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     config = Config()
     config.startup_timeout = 0.01
     lifespan = Lifespan(ASGIWrapper(SlowLifespanFramework(0.02, asyncio.sleep)), config, event_loop)
     task = event_loop.create_task(lifespan.handle_lifespan())
     with pytest.raises(LifespanTimeoutError) as exc_info:
         await lifespan.wait_for_startup()
     assert str(exc_info.value).startswith("Timeout whilst awaiting startup")
     await task
 
 
 @pytest.mark.asyncio
-async def test_startup_failure(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_startup_failure() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     lifespan = Lifespan(ASGIWrapper(lifespan_failure), Config(), event_loop)
     lifespan_task = event_loop.create_task(lifespan.handle_lifespan())
     await lifespan.wait_for_startup()
     assert lifespan_task.done()
     exception = lifespan_task.exception()
     assert isinstance(exception, LifespanFailureError)
     assert str(exception) == "Lifespan failure in startup. 'Failure'"
 
 
 async def return_app(scope: Scope, receive: Callable, send: Callable) -> None:
     return
 
 
 @pytest.mark.asyncio
-async def test_lifespan_return(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_lifespan_return() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     lifespan = Lifespan(ASGIWrapper(return_app), Config(), event_loop)
     lifespan_task = event_loop.create_task(lifespan.handle_lifespan())
     await lifespan.wait_for_startup()
     await lifespan.wait_for_shutdown()
     # Should complete (not hang)
     assert lifespan_task.done()
```

### Comparing `nonecorn-0.16.0.dev3/tests/asyncio/test_sanity.py` & `nonecorn-0.16.0.dev4/tests/asyncio/test_sanity.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 from hypercorn.asyncio.worker_context import WorkerContext
 from hypercorn.config import Config
 from .helpers import MemoryReader, MemoryWriter
 from ..helpers import SANITY_BODY, sanity_framework
 
 
 @pytest.mark.asyncio
-async def test_http1_request(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_http1_request() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     server = TCPServer(
         ASGIWrapper(sanity_framework),
         event_loop,
         Config(),
         WorkerContext(None),
         MemoryReader(),  # type: ignore
         MemoryWriter(),  # type: ignore
@@ -69,15 +71,17 @@
         h11.EndOfMessage(headers=[]),
     ]
     server.reader.close()  # type: ignore
     await task
 
 
 @pytest.mark.asyncio
-async def test_http1_websocket(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_http1_websocket() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     server = TCPServer(
         ASGIWrapper(sanity_framework),
         event_loop,
         Config(),
         WorkerContext(None),
         MemoryReader(),  # type: ignore
         MemoryWriter(),  # type: ignore
@@ -106,15 +110,17 @@
     assert list(client.events()) == [wsproto.events.CloseConnection(code=1000, reason="")]
     assert server.writer.is_closed  # type: ignore
     server.reader.close()  # type: ignore
     await task
 
 
 @pytest.mark.asyncio
-async def test_http2_request(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_http2_request() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     server = TCPServer(
         ASGIWrapper(sanity_framework),
         event_loop,
         Config(),
         WorkerContext(None),
         MemoryReader(),  # type: ignore
         MemoryWriter(http2=True),  # type: ignore
@@ -169,15 +175,17 @@
     await server.writer.receive()  # type: ignore
     assert server.writer.is_closed  # type: ignore
     server.reader.close()  # type: ignore
     await task
 
 
 @pytest.mark.asyncio
-async def test_http2_websocket(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_http2_websocket() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     server = TCPServer(
         ASGIWrapper(sanity_framework),
         event_loop,
         Config(),
         WorkerContext(None),
         MemoryReader(),  # type: ignore
         MemoryWriter(http2=True),  # type: ignore
```

### Comparing `nonecorn-0.16.0.dev3/tests/asyncio/test_task_group.py` & `nonecorn-0.16.0.dev4/tests/asyncio/test_task_group.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from hypercorn.app_wrappers import ASGIWrapper
 from hypercorn.asyncio.task_group import TaskGroup
 from hypercorn.config import Config
 from hypercorn.typing import HTTPScope, Scope
 
 
 @pytest.mark.asyncio
-async def test_spawn_app(event_loop: asyncio.AbstractEventLoop, http_scope: HTTPScope) -> None:
+async def test_spawn_app(http_scope: HTTPScope) -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     async def _echo_app(scope: Scope, receive: Callable, send: Callable) -> None:
         while True:
             message = await receive()
             if message is None:
                 return
             await send(message)
 
@@ -27,17 +29,17 @@
         )
         await put({"type": "http.disconnect"})
         assert (await app_queue.get()) == {"type": "http.disconnect"}
         await put(None)
 
 
 @pytest.mark.asyncio
-async def test_spawn_app_error(
-    event_loop: asyncio.AbstractEventLoop, http_scope: HTTPScope
-) -> None:
+async def test_spawn_app_error(http_scope: HTTPScope) -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     async def _error_app(scope: Scope, receive: Callable, send: Callable) -> None:
         raise Exception()
 
     app_queue: asyncio.Queue = asyncio.Queue()
     async with TaskGroup(event_loop) as task_group:
         await task_group.spawn_app(ASGIWrapper(_error_app), Config(), http_scope, app_queue.put)
     assert (await app_queue.get()) is None
```

### Comparing `nonecorn-0.16.0.dev3/tests/asyncio/test_tcp_server.py` & `nonecorn-0.16.0.dev4/tests/asyncio/test_tcp_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from hypercorn.asyncio.worker_context import WorkerContext
 from hypercorn.config import Config
 from .helpers import MemoryReader, MemoryWriter
 from ..helpers import echo_framework
 
 
 @pytest.mark.asyncio
-async def test_completes_on_closed(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_completes_on_closed() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     server = TCPServer(
         ASGIWrapper(echo_framework),
         event_loop,
         Config(),
         WorkerContext(None),
         MemoryReader(),  # type: ignore
         MemoryWriter(),  # type: ignore
@@ -25,15 +27,17 @@
     server.reader.close()  # type: ignore
     await server.run()
     # Key is that this line is reached, rather than the above line
     # hanging.
 
 
 @pytest.mark.asyncio
-async def test_complets_on_half_close(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_complets_on_half_close() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     server = TCPServer(
         ASGIWrapper(echo_framework),
         event_loop,
         Config(),
         WorkerContext(None),
         MemoryReader(),  # type: ignore
         MemoryWriter(),  # type: ignore
```

### Comparing `nonecorn-0.16.0.dev3/tests/conftest.py` & `nonecorn-0.16.0.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/helpers.py` & `nonecorn-0.16.0.dev4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/middleware/test_dispatcher.py` & `nonecorn-0.16.0.dev4/tests/middleware/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/middleware/test_http_to_https.py` & `nonecorn-0.16.0.dev4/tests/middleware/test_http_to_https.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/middleware/test_proxy_fix.py` & `nonecorn-0.16.0.dev4/tests/middleware/test_proxy_fix.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/protocol/test_h11.py` & `nonecorn-0.16.0.dev4/tests/protocol/test_h11.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,17 +132,17 @@
     await protocol.stream_send(EndBody(stream_id=1))
     await protocol.stream_send(StreamClosed(stream_id=1))
     protocol.send.assert_called()  # type: ignore
     assert protocol.send.call_args_list[3] == call(expected)  # type: ignore
 
 
 @pytest.mark.asyncio
-async def test_protocol_instant_recycle(
-    protocol: H11Protocol, event_loop: asyncio.AbstractEventLoop
-) -> None:
+async def test_protocol_instant_recycle(protocol: H11Protocol) -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     # This test task acts as the asgi app, spawned tasks act as the
     # server.
     data = b"GET / HTTP/1.1\r\nHost: hypercorn\r\n\r\n"
     # This test requires a real event as the handling should pause on
     # the instant receipt
     protocol.can_read = EventWrapper()
     task = event_loop.create_task(protocol.handle(RawData(data=data)))
```

### Comparing `nonecorn-0.16.0.dev3/tests/protocol/test_h2.py` & `nonecorn-0.16.0.dev4/tests/protocol/test_h2.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     from unittest.mock import AsyncMock
 except ImportError:
     # Python < 3.8
     from mock import AsyncMock  # type: ignore
 
 
 @pytest.mark.asyncio
-async def test_stream_buffer_push_and_pop(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_stream_buffer_push_and_pop() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     stream_buffer = StreamBuffer(EventWrapper)
 
     async def _push_over_limit() -> bool:
         await stream_buffer.push(b"a" * (BUFFER_HIGH_WATER + 1))
         return True
 
     task = event_loop.create_task(_push_over_limit())
@@ -32,41 +34,43 @@
     await stream_buffer.pop(BUFFER_HIGH_WATER // 4)
     assert not task.done()  # Blocked as over low water
     await stream_buffer.pop(BUFFER_HIGH_WATER // 4)
     assert (await task) is True
 
 
 @pytest.mark.asyncio
-async def test_stream_buffer_drain(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_stream_buffer_drain() -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     stream_buffer = StreamBuffer(EventWrapper)
     await stream_buffer.push(b"a" * 10)
 
     async def _drain() -> bool:
         await stream_buffer.drain()
         return True
 
     task = event_loop.create_task(_drain())
     assert not task.done()  # Blocked
     await stream_buffer.pop(20)
     assert (await task) is True
 
 
 @pytest.mark.asyncio
-async def test_stream_buffer_closed(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_stream_buffer_closed() -> None:
     stream_buffer = StreamBuffer(EventWrapper)
     await stream_buffer.close()
     await stream_buffer._is_empty.wait()
     await stream_buffer._paused.wait()
     assert True
     with pytest.raises(BufferCompleteError):
         await stream_buffer.push(b"a")
 
 
 @pytest.mark.asyncio
-async def test_stream_buffer_complete(event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_stream_buffer_complete() -> None:
     stream_buffer = StreamBuffer(EventWrapper)
     await stream_buffer.push(b"a" * 10)
     assert not stream_buffer.complete
     stream_buffer.set_complete()
     assert not stream_buffer.complete
     await stream_buffer.pop(20)
     assert stream_buffer.complete
```

### Comparing `nonecorn-0.16.0.dev3/tests/protocol/test_http_stream.py` & `nonecorn-0.16.0.dev4/tests/protocol/test_http_stream.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/protocol/test_ws_stream.py` & `nonecorn-0.16.0.dev4/tests/protocol/test_ws_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,17 @@
         call(Data(stream_id=1, data=b"\x81\x05hello")),
         call(Data(stream_id=1, data=b"\x88\x02\x03\xe8")),
         call(EndData(stream_id=1)),
     ]
 
 
 @pytest.mark.asyncio
-async def test_pings(stream: WSStream, event_loop: asyncio.AbstractEventLoop) -> None:
+async def test_pings(stream: WSStream) -> None:
+    event_loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+
     stream.config.websocket_ping_interval = 0.1
     await stream.handle(
         Request(
             stream_id=1,
             http_version="2",
             headers=[(b"sec-websocket-version", b"13")],
             raw_path=b"/?a=b",
```

### Comparing `nonecorn-0.16.0.dev3/tests/test___main__.py` & `nonecorn-0.16.0.dev4/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/test_app_wrappers.py` & `nonecorn-0.16.0.dev4/tests/test_app_wrappers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/test_config.py` & `nonecorn-0.16.0.dev4/tests/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,20 +49,31 @@
     _check_standard_config(config)
 
 
 def test_create_ssl_context() -> None:
     path = os.path.join(os.path.dirname(__file__), "assets/config_ssl.py")
     config = Config.from_pyfile(path)
     context = config.create_ssl_context()
-    assert context.options & (
-        ssl.OP_NO_SSLv2
-        | ssl.OP_NO_SSLv3
-        | ssl.OP_NO_TLSv1
-        | ssl.OP_NO_TLSv1_1
-        | ssl.OP_NO_COMPRESSION
+
+    # NOTE: In earlier versions of python context.options is equal to <Options.OP_NO_COMPRESSION: 0>
+    #       hence the ANDing context.options with the specified ssl options results in
+    #       "<Options.OP_NO_COMPRESSION: 0>", which as a Boolean value, is False.
+    #
+    #       To overcome this, instead of checking that the result in True, we will check that it is
+    #        equal to "context.options".
+    assert (
+        context.options
+        & (
+            ssl.OP_NO_SSLv2
+            | ssl.OP_NO_SSLv3
+            | ssl.OP_NO_TLSv1
+            | ssl.OP_NO_TLSv1_1
+            | ssl.OP_NO_COMPRESSION
+        )
+        == context.options
     )
 
 
 @pytest.mark.parametrize(
     "bind, expected_family, expected_binding",
     [
         ("127.0.0.1:5000", socket.AF_INET, ("127.0.0.1", 5000)),
```

### Comparing `nonecorn-0.16.0.dev3/tests/test_logging.py` & `nonecorn-0.16.0.dev4/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/test_utils.py` & `nonecorn-0.16.0.dev4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/trio/test_keep_alive.py` & `nonecorn-0.16.0.dev4/tests/trio/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tests/trio/test_lifespan.py` & `nonecorn-0.16.0.dev4/tests/trio/test_lifespan.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 from __future__ import annotations
 
+import sys
+
+if sys.version_info < (3, 11):
+    from exceptiongroup import ExceptionGroup
+
 import pytest
 import trio
 
 from hypercorn.app_wrappers import ASGIWrapper
 from hypercorn.config import Config
 from hypercorn.trio.lifespan import Lifespan
 from hypercorn.utils import LifespanFailureError, LifespanTimeoutError
@@ -20,13 +25,21 @@
         await lifespan.wait_for_startup()
     assert str(exc_info.value).startswith("Timeout whilst awaiting startup")
 
 
 @pytest.mark.trio
 async def test_startup_failure() -> None:
     lifespan = Lifespan(ASGIWrapper(lifespan_failure), Config())
+
     with pytest.raises(LifespanFailureError) as exc_info:
-        async with trio.open_nursery() as lifespan_nursery:
-            await lifespan_nursery.start(lifespan.handle_lifespan)
-            await lifespan.wait_for_startup()
+        try:
+            async with trio.open_nursery() as lifespan_nursery:
+                await lifespan_nursery.start(lifespan.handle_lifespan)
+                await lifespan.wait_for_startup()
+        except ExceptionGroup as exception:
+            target_exception = exception
+            if len(exception.exceptions) == 1:
+                target_exception = exception.exceptions[0]
+
+            raise target_exception.with_traceback(target_exception.__traceback__)
 
     assert str(exc_info.value) == "Lifespan failure in startup. 'Failure'"
```

### Comparing `nonecorn-0.16.0.dev3/tests/trio/test_sanity.py` & `nonecorn-0.16.0.dev4/tests/trio/test_sanity.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev3/tox.ini` & `nonecorn-0.16.0.dev4/tox.ini`

 * *Files identical despite different names*

