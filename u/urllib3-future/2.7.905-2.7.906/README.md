# Comparing `tmp/urllib3_future-2.7.905.tar.gz` & `tmp/urllib3_future-2.7.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Apr 28 11:52:11 2024, max compression
+gzip compressed data, last modified: Thu May  2 06:05:36 2024, max compression
```

## Comparing `urllib3_future-2.7.905.tar` & `urllib3_future-2.7.906.tar`

### file list

```diff
@@ -1,312 +1,312 @@
--rw-r--r--   0        0        0    86587 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/CHANGES.rst
--rw-r--r--   0        0        0      490 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dev-requirements.txt
--rw-r--r--   0        0        0     4602 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/Makefile
--rw-r--r--   0        0        0    54247 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/advanced-usage.rst
--rw-r--r--   0        0        0     4297 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/async.rst
--rw-r--r--   0        0        0       59 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/changelog.rst
--rw-r--r--   0        0        0     5787 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/conf.py
--rw-r--r--   0        0        0     6749 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/contributing.rst
--rw-r--r--   0        0        0     1939 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/index.rst
--rw-r--r--   0        0        0     4513 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/make.bat
--rw-r--r--   0        0        0       92 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/requirements.txt
--rw-r--r--   0        0        0    17426 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/user-guide.rst
--rw-r--r--   0        0        0    15195 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/v2-migration-guide.rst
--rw-r--r--   0        0        0     1770 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/_static/banner.svg
--rw-r--r--   0        0        0     3999 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/_static/banner_github.svg
--rw-r--r--   0        0        0     1818 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/_static/dark-logo.svg
--rw-r--r--   0        0        0   307934 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/_static/logo.png
--rw-r--r--   0        0        0     7872 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/images/demo-button.png
--rw-r--r--   0        0        0      714 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/images/favicon.png
--rw-r--r--   0        0        0     6226 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/images/learn-more-button.png
--rw-r--r--   0        0        0     2165 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/images/logo.png
--rw-r--r--   0        0        0      516 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/images/logo.svg
--rw-r--r--   0        0        0      245 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/index.rst
--rw-r--r--   0        0        0      457 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/urllib3.backend.rst
--rw-r--r--   0        0        0      349 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/urllib3.connection.rst
--rw-r--r--   0        0        0      712 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/urllib3.connectionpool.rst
--rw-r--r--   0        0        0      185 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/urllib3.exceptions.rst
--rw-r--r--   0        0        0      350 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/urllib3.fields.rst
--rw-r--r--   0        0        0      559 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/urllib3.poolmanager.rst
--rw-r--r--   0        0        0       71 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/urllib3.request.rst
--rw-r--r--   0        0        0      905 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/urllib3.response.rst
--rw-r--r--   0        0        0      385 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/urllib3.util.rst
--rw-r--r--   0        0        0      206 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/contrib/index.rst
--rw-r--r--   0        0        0      231 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/contrib/resolver.rst
--rw-r--r--   0        0        0      124 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/contrib/socks.rst
--rw-r--r--   0        0        0      142 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/docs/reference/contrib/ssa.rst
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/__init__.py
--rw-r--r--   0        0        0    13408 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/handlers.py
--rwxr-xr-x   0        0        0     1198 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/https_proxy.py
--rwxr-xr-x   0        0        0     4582 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/proxy.py
--rwxr-xr-x   0        0        0     9813 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/server.py
--rw-r--r--   0        0        0    11213 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/testcase.py
--rw-r--r--   0        0        0      511 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/certs/README.rst
--rw-r--r--   0        0        0     1679 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/certs/cacert.key
--rw-r--r--   0        0        0     1273 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/certs/cacert.pem
--rw-r--r--   0        0        0     1265 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/certs/server.crt
--rw-r--r--   0        0        0     1679 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/dummyserver/certs/server.key
--rw-r--r--   0        0        0     6090 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/__init__.py
--rw-r--r--   0        0        0    15956 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/_collections.py
--rw-r--r--   0        0        0     8092 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/_constant.py
--rw-r--r--   0        0        0    21727 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/_request_methods.py
--rw-r--r--   0        0        0     2655 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/_typing.py
--rw-r--r--   0        0        0      100 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/_version.py
--rw-r--r--   0        0        0    38148 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/connection.py
--rw-r--r--   0        0        0    75605 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9988 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/exceptions.py
--rw-r--r--   0        0        0     9151 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/fields.py
--rw-r--r--   0        0        0     2202 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/filepost.py
--rw-r--r--   0        0        0    36048 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/py.typed
--rw-r--r--   0        0        0    35459 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/response.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/_async/__init__.py
--rw-r--r--   0        0        0    36236 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/_async/connection.py
--rw-r--r--   0        0        0    77458 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/_async/connectionpool.py
--rw-r--r--   0        0        0    32214 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/_async/poolmanager.py
--rw-r--r--   0        0        0    17222 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/_async/response.py
--rw-r--r--   0        0        0      390 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/backend/__init__.py
--rw-r--r--   0        0        0    16031 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/backend/_base.py
--rw-r--r--   0        0        0    44491 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/backend/hface.py
--rw-r--r--   0        0        0      225 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/backend/_async/__init__.py
--rw-r--r--   0        0        0     6002 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/backend/_async/_base.py
--rw-r--r--   0        0        0    42615 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/backend/_async/hface.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0     4930 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/_socks_override.py
--rw-r--r--   0        0        0      724 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    13565 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/socks.py
--rw-r--r--   0        0        0     1109 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/__init__.py
--rw-r--r--   0        0        0     1699 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/_configuration.py
--rw-r--r--   0        0        0     1207 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/_error_codes.py
--rw-r--r--   0        0        0     3729 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/_stream_matrix.py
--rw-r--r--   0        0        0      801 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/_typing.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/py.typed
--rw-r--r--   0        0        0     1085 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/events/__init__.py
--rw-r--r--   0        0        0     4421 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/events/_events.py
--rw-r--r--   0        0        0     1003 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/__init__.py
--rw-r--r--   0        0        0     4327 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/_factories.py
--rw-r--r--   0        0        0     9935 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/_protocols.py
--rw-r--r--   0        0        0      705 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0    10446 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http1/_h11.py
--rw-r--r--   0        0        0      704 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     8859 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http2/_h2.py
--rw-r--r--   0        0        0      709 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0    17220 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http3/_qh3.py
--rw-r--r--   0        0        0     3314 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/imcc/__init__.py
--rw-r--r--   0        0        0      293 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/__init__.py
--rw-r--r--   0        0        0     8415 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/factories.py
--rw-r--r--   0        0        0    18961 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/protocols.py
--rw-r--r--   0        0        0     4290 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/utils.py
--rw-r--r--   0        0        0      291 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/__init__.py
--rw-r--r--   0        0        0     7871 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/factories.py
--rw-r--r--   0        0        0    10621 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/protocols.py
--rw-r--r--   0        0        0      381 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/doh/__init__.py
--rw-r--r--   0        0        0    22371 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/doq/__init__.py
--rw-r--r--   0        0        0    15402 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/dot/__init__.py
--rw-r--r--   0        0        0     5951 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/dou/__init__.py
--rw-r--r--   0        0        0    11140 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/in_memory/__init__.py
--rw-r--r--   0        0        0     5299 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/in_memory/_dict.py
--rw-r--r--   0        0        0     2643 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/null/__init__.py
--rw-r--r--   0        0        0      103 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/system/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/system/_socket.py
--rw-r--r--   0        0        0      381 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/doh/__init__.py
--rw-r--r--   0        0        0    22180 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/doq/__init__.py
--rw-r--r--   0        0        0    14846 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/dot/__init__.py
--rw-r--r--   0        0        0     4493 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/dou/__init__.py
--rw-r--r--   0        0        0    10836 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/in_memory/__init__.py
--rw-r--r--   0        0        0     5425 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/in_memory/_dict.py
--rw-r--r--   0        0        0     2539 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/null/__init__.py
--rw-r--r--   0        0        0      103 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/system/__init__.py
--rw-r--r--   0        0        0     1626 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/resolver/system/_socket.py
--rw-r--r--   0        0        0    12158 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/contrib/ssa/__init__.py
--rw-r--r--   0        0        0      999 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/__init__.py
--rw-r--r--   0        0        0     3884 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/connection.py
--rw-r--r--   0        0        0     1145 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8886 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/request.py
--rw-r--r--   0        0        0     1329 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/response.py
--rw-r--r--   0        0        0    19245 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/retry.py
--rw-r--r--   0        0        0    24783 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5816 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     7226 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10684 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/timeout.py
--rw-r--r--   0        0        0    21933 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/traffic_police.py
--rw-r--r--   0        0        0    15270 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/wait.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/_async/__init__.py
--rw-r--r--   0        0        0     5492 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/_async/ssl_.py
--rw-r--r--   0        0        0    22050 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3/util/_async/traffic_police.py
--rw-r--r--   0        0        0     6090 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/__init__.py
--rw-r--r--   0        0        0    15956 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/_collections.py
--rw-r--r--   0        0        0     8092 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/_constant.py
--rw-r--r--   0        0        0    21727 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/_request_methods.py
--rw-r--r--   0        0        0     2655 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/_typing.py
--rw-r--r--   0        0        0      100 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/_version.py
--rw-r--r--   0        0        0    38148 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/connection.py
--rw-r--r--   0        0        0    75605 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/connectionpool.py
--rw-r--r--   0        0        0     9988 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/exceptions.py
--rw-r--r--   0        0        0     9151 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/fields.py
--rw-r--r--   0        0        0     2202 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/filepost.py
--rw-r--r--   0        0        0    36048 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/poolmanager.py
--rw-r--r--   0        0        0       93 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/py.typed
--rw-r--r--   0        0        0    35459 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/response.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/_async/__init__.py
--rw-r--r--   0        0        0    36236 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/_async/connection.py
--rw-r--r--   0        0        0    77458 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/_async/connectionpool.py
--rw-r--r--   0        0        0    32214 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/_async/poolmanager.py
--rw-r--r--   0        0        0    17222 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/_async/response.py
--rw-r--r--   0        0        0      390 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/backend/__init__.py
--rw-r--r--   0        0        0    16031 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/backend/_base.py
--rw-r--r--   0        0        0    44491 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/backend/hface.py
--rw-r--r--   0        0        0      225 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/backend/_async/__init__.py
--rw-r--r--   0        0        0     6002 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/backend/_async/_base.py
--rw-r--r--   0        0        0    42615 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/backend/_async/hface.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/__init__.py
--rw-r--r--   0        0        0     4930 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/_socks_override.py
--rw-r--r--   0        0        0      724 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/pyopenssl.py
--rw-r--r--   0        0        0    13565 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/socks.py
--rw-r--r--   0        0        0     1109 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/__init__.py
--rw-r--r--   0        0        0     1699 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/_configuration.py
--rw-r--r--   0        0        0     1207 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/_error_codes.py
--rw-r--r--   0        0        0     3729 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/_stream_matrix.py
--rw-r--r--   0        0        0      801 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/_typing.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/py.typed
--rw-r--r--   0        0        0     1085 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/events/__init__.py
--rw-r--r--   0        0        0     4421 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/events/_events.py
--rw-r--r--   0        0        0     1003 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/__init__.py
--rw-r--r--   0        0        0     4327 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/_factories.py
--rw-r--r--   0        0        0     9935 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/_protocols.py
--rw-r--r--   0        0        0      705 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0    10446 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http1/_h11.py
--rw-r--r--   0        0        0      704 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     8859 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http2/_h2.py
--rw-r--r--   0        0        0      709 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0    17220 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py
--rw-r--r--   0        0        0     3314 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/imcc/__init__.py
--rw-r--r--   0        0        0      293 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/__init__.py
--rw-r--r--   0        0        0     8415 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/factories.py
--rw-r--r--   0        0        0    18961 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/protocols.py
--rw-r--r--   0        0        0     4290 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/utils.py
--rw-r--r--   0        0        0      291 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/__init__.py
--rw-r--r--   0        0        0     7871 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/factories.py
--rw-r--r--   0        0        0    10621 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/protocols.py
--rw-r--r--   0        0        0      381 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/doh/__init__.py
--rw-r--r--   0        0        0    22371 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/doq/__init__.py
--rw-r--r--   0        0        0    15402 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/dot/__init__.py
--rw-r--r--   0        0        0     5951 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/dou/__init__.py
--rw-r--r--   0        0        0    11140 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/in_memory/__init__.py
--rw-r--r--   0        0        0     5299 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py
--rw-r--r--   0        0        0     2643 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/null/__init__.py
--rw-r--r--   0        0        0      103 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/system/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/system/_socket.py
--rw-r--r--   0        0        0      381 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/doh/__init__.py
--rw-r--r--   0        0        0    22180 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/doq/__init__.py
--rw-r--r--   0        0        0    14846 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/dot/__init__.py
--rw-r--r--   0        0        0     4493 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/dou/__init__.py
--rw-r--r--   0        0        0    10836 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/in_memory/__init__.py
--rw-r--r--   0        0        0     5425 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/in_memory/_dict.py
--rw-r--r--   0        0        0     2539 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/null/__init__.py
--rw-r--r--   0        0        0      103 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/system/__init__.py
--rw-r--r--   0        0        0     1626 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/system/_socket.py
--rw-r--r--   0        0        0    12158 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/contrib/ssa/__init__.py
--rw-r--r--   0        0        0      999 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/__init__.py
--rw-r--r--   0        0        0     3884 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/connection.py
--rw-r--r--   0        0        0     1145 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/proxy.py
--rw-r--r--   0        0        0     8886 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/request.py
--rw-r--r--   0        0        0     1329 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/response.py
--rw-r--r--   0        0        0    19245 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/retry.py
--rw-r--r--   0        0        0    24783 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/ssl_.py
--rw-r--r--   0        0        0     5816 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     7226 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/ssltransport.py
--rw-r--r--   0        0        0    10684 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/timeout.py
--rw-r--r--   0        0        0    21933 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/traffic_police.py
--rw-r--r--   0        0        0    15270 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/url.py
--rw-r--r--   0        0        0     1146 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/util.py
--rw-r--r--   0        0        0     4423 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/wait.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/_async/__init__.py
--rw-r--r--   0        0        0     5492 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/_async/ssl_.py
--rw-r--r--   0        0        0    22050 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/src/urllib3_future/util/_async/traffic_police.py
--rw-r--r--   0        0        0     9646 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/__init__.py
--rw-r--r--   0        0        0    11926 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/conftest.py
--rw-r--r--   0        0        0     6222 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/port_helpers.py
--rw-r--r--   0        0        0    12638 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_collections.py
--rw-r--r--   0        0        0      692 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_compatibility.py
--rw-r--r--   0        0        0    10288 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_connection.py
--rw-r--r--   0        0        0    22649 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_connectionpool.py
--rw-r--r--   0        0        0     1531 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_exceptions.py
--rw-r--r--   0        0        0     3882 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_fields.py
--rw-r--r--   0        0        0     3778 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_filepost.py
--rw-r--r--   0        0        0      978 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_no_ssl.py
--rw-r--r--   0        0        0    17951 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_poolmanager.py
--rw-r--r--   0        0        0     3657 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_proxymanager.py
--rw-r--r--   0        0        0    38863 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_response.py
--rw-r--r--   0        0        0    16640 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_retry.py
--rw-r--r--   0        0        0     6554 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_ssl.py
--rw-r--r--   0        0        0    16917 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_ssltransport.py
--rw-r--r--   0        0        0    43037 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_util.py
--rw-r--r--   0        0        0     5999 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/test_wait.py
--rw-r--r--   0        0        0     1187 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/tz_stub.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/contrib/__init__.py
--rw-r--r--   0        0        0     1257 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/contrib/duplicate_san.pem
--rw-r--r--   0        0        0    21281 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/contrib/test_resolver.py
--rw-r--r--   0        0        0    25922 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/contrib/test_socks.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/contrib/asynchronous/__init__.py
--rw-r--r--   0        0        0    21291 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/contrib/asynchronous/test_resolver.py
--rw-r--r--   0        0        0    21728 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/contrib/asynchronous/test_socks.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/contrib/hface/__init__.py
--rw-r--r--   0        0        0     3717 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/contrib/hface/test_stream_matrix.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/__init__.py
--rw-r--r--   0        0        0     9840 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/test_chunked_transfer.py
--rw-r--r--   0        0        0     3702 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/test_connection.py
--rw-r--r--   0        0        0    56059 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/test_connectionpool.py
--rw-r--r--   0        0        0     7756 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/test_happy_eyeballs.py
--rw-r--r--   0        0        0    43193 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/test_https.py
--rw-r--r--   0        0        0     1104 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/test_no_ssl.py
--rw-r--r--   0        0        0    23853 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/test_poolmanager.py
--rw-r--r--   0        0        0    32501 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/test_proxy_poolmanager.py
--rw-r--r--   0        0        0    88179 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/test_socketlevel.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/asynchronous/__init__.py
--rw-r--r--   0        0        0    59408 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/asynchronous/test_connectionpool.py
--rw-r--r--   0        0        0     7329 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/asynchronous/test_happy_eyeballs.py
--rw-r--r--   0        0        0    19562 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_dummyserver/asynchronous/test_poolmanager.py
--rw-r--r--   0        0        0     2837 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/__init__.py
--rw-r--r--   0        0        0     3069 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/test_conn_info.py
--rw-r--r--   0        0        0     3764 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/test_connection.py
--rw-r--r--   0        0        0     2821 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/test_connection_multiplexed.py
--rw-r--r--   0        0        0     5912 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/test_connectionpool_multiplexed.py
--rw-r--r--   0        0        0     1924 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/test_protolevel.py
--rw-r--r--   0        0        0     3209 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/test_proxy.py
--rw-r--r--   0        0        0     5658 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/test_send_data.py
--rw-r--r--   0        0        0     1864 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/test_stream.py
--rw-r--r--   0        0        0     6683 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/test_svn.py
--rw-r--r--   0        0        0        0 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/asynchronous/__init__.py
--rw-r--r--   0        0        0     2217 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/asynchronous/test_conn_info.py
--rw-r--r--   0        0        0     4035 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/asynchronous/test_connection.py
--rw-r--r--   0        0        0     3122 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/asynchronous/test_connection_multiplexed.py
--rw-r--r--   0        0        0     6143 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py
--rw-r--r--   0        0        0     2003 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/asynchronous/test_protolevel.py
--rw-r--r--   0        0        0     3274 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/asynchronous/test_proxy.py
--rw-r--r--   0        0        0     5880 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/asynchronous/test_send_data.py
--rw-r--r--   0        0        0     1967 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/asynchronous/test_stream.py
--rw-r--r--   0        0        0     7217 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/test/with_traefik/asynchronous/test_svn.py
--rw-r--r--   0        0        0       85 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/.gitignore
--rw-r--r--   0        0        0     1093 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/LICENSE.txt
--rw-r--r--   0        0        0     4277 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/README.md
--rw-r--r--   0        0        0     1342 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/hatch_build.py
--rw-r--r--   0        0        0     5594 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/pyproject.toml
--rw-r--r--   0        0        0     7012 2024-04-28 11:52:11.000000 urllib3_future-2.7.905/PKG-INFO
+-rw-r--r--   0        0        0    86709 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/CHANGES.rst
+-rw-r--r--   0        0        0      490 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dev-requirements.txt
+-rw-r--r--   0        0        0     4602 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/Makefile
+-rw-r--r--   0        0        0    54247 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/advanced-usage.rst
+-rw-r--r--   0        0        0     4297 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/async.rst
+-rw-r--r--   0        0        0       59 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/changelog.rst
+-rw-r--r--   0        0        0     5787 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/conf.py
+-rw-r--r--   0        0        0     6749 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/contributing.rst
+-rw-r--r--   0        0        0     1939 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/index.rst
+-rw-r--r--   0        0        0     4513 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/make.bat
+-rw-r--r--   0        0        0       92 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/requirements.txt
+-rw-r--r--   0        0        0    17426 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/user-guide.rst
+-rw-r--r--   0        0        0    15195 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/v2-migration-guide.rst
+-rw-r--r--   0        0        0     1770 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/_static/banner.svg
+-rw-r--r--   0        0        0     3999 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/_static/banner_github.svg
+-rw-r--r--   0        0        0     1818 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/_static/dark-logo.svg
+-rw-r--r--   0        0        0   307934 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/_static/logo.png
+-rw-r--r--   0        0        0     7872 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/images/demo-button.png
+-rw-r--r--   0        0        0      714 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/images/favicon.png
+-rw-r--r--   0        0        0     6226 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/images/learn-more-button.png
+-rw-r--r--   0        0        0     2165 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/images/logo.png
+-rw-r--r--   0        0        0      516 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/images/logo.svg
+-rw-r--r--   0        0        0      245 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/index.rst
+-rw-r--r--   0        0        0      457 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/urllib3.backend.rst
+-rw-r--r--   0        0        0      349 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/urllib3.connection.rst
+-rw-r--r--   0        0        0      712 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/urllib3.connectionpool.rst
+-rw-r--r--   0        0        0      185 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/urllib3.exceptions.rst
+-rw-r--r--   0        0        0      350 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/urllib3.fields.rst
+-rw-r--r--   0        0        0      559 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/urllib3.poolmanager.rst
+-rw-r--r--   0        0        0       71 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/urllib3.request.rst
+-rw-r--r--   0        0        0      905 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/urllib3.response.rst
+-rw-r--r--   0        0        0      385 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/urllib3.util.rst
+-rw-r--r--   0        0        0      206 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/contrib/index.rst
+-rw-r--r--   0        0        0      231 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/contrib/resolver.rst
+-rw-r--r--   0        0        0      124 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/contrib/socks.rst
+-rw-r--r--   0        0        0      142 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/docs/reference/contrib/ssa.rst
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/__init__.py
+-rw-r--r--   0        0        0    13408 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/handlers.py
+-rwxr-xr-x   0        0        0     1198 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/https_proxy.py
+-rwxr-xr-x   0        0        0     4582 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/proxy.py
+-rwxr-xr-x   0        0        0     9813 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/server.py
+-rw-r--r--   0        0        0    11213 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/testcase.py
+-rw-r--r--   0        0        0      511 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/certs/README.rst
+-rw-r--r--   0        0        0     1679 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/certs/cacert.key
+-rw-r--r--   0        0        0     1273 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/certs/cacert.pem
+-rw-r--r--   0        0        0     1265 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/certs/server.crt
+-rw-r--r--   0        0        0     1679 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/dummyserver/certs/server.key
+-rw-r--r--   0        0        0     6090 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/__init__.py
+-rw-r--r--   0        0        0    15956 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/_collections.py
+-rw-r--r--   0        0        0     8092 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/_constant.py
+-rw-r--r--   0        0        0    21727 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/_request_methods.py
+-rw-r--r--   0        0        0     2655 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/_typing.py
+-rw-r--r--   0        0        0      100 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/_version.py
+-rw-r--r--   0        0        0    38148 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/connection.py
+-rw-r--r--   0        0        0    75605 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9988 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/exceptions.py
+-rw-r--r--   0        0        0     9151 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/fields.py
+-rw-r--r--   0        0        0     2202 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/filepost.py
+-rw-r--r--   0        0        0    36048 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/py.typed
+-rw-r--r--   0        0        0    35459 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/response.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/_async/__init__.py
+-rw-r--r--   0        0        0    36236 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/_async/connection.py
+-rw-r--r--   0        0        0    77458 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/_async/connectionpool.py
+-rw-r--r--   0        0        0    32214 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/_async/poolmanager.py
+-rw-r--r--   0        0        0    17222 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/_async/response.py
+-rw-r--r--   0        0        0      390 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/backend/__init__.py
+-rw-r--r--   0        0        0    16166 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/backend/_base.py
+-rw-r--r--   0        0        0    44522 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/backend/hface.py
+-rw-r--r--   0        0        0      225 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/backend/_async/__init__.py
+-rw-r--r--   0        0        0     5987 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/backend/_async/_base.py
+-rw-r--r--   0        0        0    42646 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/backend/_async/hface.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0     4930 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/_socks_override.py
+-rw-r--r--   0        0        0      724 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    13565 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0     1109 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/__init__.py
+-rw-r--r--   0        0        0     1699 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/_error_codes.py
+-rw-r--r--   0        0        0     3729 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/_stream_matrix.py
+-rw-r--r--   0        0        0      801 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/_typing.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/py.typed
+-rw-r--r--   0        0        0     1085 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/events/__init__.py
+-rw-r--r--   0        0        0     4421 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/events/_events.py
+-rw-r--r--   0        0        0     1003 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/__init__.py
+-rw-r--r--   0        0        0     4327 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/_factories.py
+-rw-r--r--   0        0        0     9935 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      705 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    10446 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0      704 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     9084 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      709 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0    16782 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http3/_qh3.py
+-rw-r--r--   0        0        0     3314 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/imcc/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/__init__.py
+-rw-r--r--   0        0        0     8415 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/factories.py
+-rw-r--r--   0        0        0    18961 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/protocols.py
+-rw-r--r--   0        0        0     4290 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/utils.py
+-rw-r--r--   0        0        0      291 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/__init__.py
+-rw-r--r--   0        0        0     7871 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/factories.py
+-rw-r--r--   0        0        0    10621 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/protocols.py
+-rw-r--r--   0        0        0      381 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/doh/__init__.py
+-rw-r--r--   0        0        0    22371 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/doq/__init__.py
+-rw-r--r--   0        0        0    15402 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/dot/__init__.py
+-rw-r--r--   0        0        0     5951 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/dou/__init__.py
+-rw-r--r--   0        0        0    11140 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/in_memory/__init__.py
+-rw-r--r--   0        0        0     5299 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/in_memory/_dict.py
+-rw-r--r--   0        0        0     2643 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/system/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/system/_socket.py
+-rw-r--r--   0        0        0      381 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/doh/__init__.py
+-rw-r--r--   0        0        0    22180 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/doq/__init__.py
+-rw-r--r--   0        0        0    14846 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/dot/__init__.py
+-rw-r--r--   0        0        0     4493 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/dou/__init__.py
+-rw-r--r--   0        0        0    10836 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/in_memory/__init__.py
+-rw-r--r--   0        0        0     5425 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/in_memory/_dict.py
+-rw-r--r--   0        0        0     2539 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/system/__init__.py
+-rw-r--r--   0        0        0     1626 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/resolver/system/_socket.py
+-rw-r--r--   0        0        0    12158 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/contrib/ssa/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     3884 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1145 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8886 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/request.py
+-rw-r--r--   0        0        0     1329 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/response.py
+-rw-r--r--   0        0        0    19245 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/retry.py
+-rw-r--r--   0        0        0    24783 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5816 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     7226 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10684 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    21933 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/traffic_police.py
+-rw-r--r--   0        0        0    15295 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/wait.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/_async/__init__.py
+-rw-r--r--   0        0        0     5492 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/_async/ssl_.py
+-rw-r--r--   0        0        0    22050 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3/util/_async/traffic_police.py
+-rw-r--r--   0        0        0     6090 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/__init__.py
+-rw-r--r--   0        0        0    15956 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/_collections.py
+-rw-r--r--   0        0        0     8092 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/_constant.py
+-rw-r--r--   0        0        0    21727 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/_request_methods.py
+-rw-r--r--   0        0        0     2655 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/_typing.py
+-rw-r--r--   0        0        0      100 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/_version.py
+-rw-r--r--   0        0        0    38148 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/connection.py
+-rw-r--r--   0        0        0    75605 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/connectionpool.py
+-rw-r--r--   0        0        0     9988 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/exceptions.py
+-rw-r--r--   0        0        0     9151 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/fields.py
+-rw-r--r--   0        0        0     2202 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/filepost.py
+-rw-r--r--   0        0        0    36048 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/poolmanager.py
+-rw-r--r--   0        0        0       93 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/py.typed
+-rw-r--r--   0        0        0    35459 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/response.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/_async/__init__.py
+-rw-r--r--   0        0        0    36236 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/_async/connection.py
+-rw-r--r--   0        0        0    77458 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/_async/connectionpool.py
+-rw-r--r--   0        0        0    32214 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/_async/poolmanager.py
+-rw-r--r--   0        0        0    17222 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/_async/response.py
+-rw-r--r--   0        0        0      390 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/backend/__init__.py
+-rw-r--r--   0        0        0    16166 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/backend/_base.py
+-rw-r--r--   0        0        0    44522 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/backend/hface.py
+-rw-r--r--   0        0        0      225 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/backend/_async/__init__.py
+-rw-r--r--   0        0        0     5987 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/backend/_async/_base.py
+-rw-r--r--   0        0        0    42646 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/backend/_async/hface.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/__init__.py
+-rw-r--r--   0        0        0     4930 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/_socks_override.py
+-rw-r--r--   0        0        0      724 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    13565 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/socks.py
+-rw-r--r--   0        0        0     1109 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/__init__.py
+-rw-r--r--   0        0        0     1699 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/_error_codes.py
+-rw-r--r--   0        0        0     3729 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/_stream_matrix.py
+-rw-r--r--   0        0        0      801 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/_typing.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/py.typed
+-rw-r--r--   0        0        0     1085 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/events/__init__.py
+-rw-r--r--   0        0        0     4421 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/events/_events.py
+-rw-r--r--   0        0        0     1003 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/__init__.py
+-rw-r--r--   0        0        0     4327 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/_factories.py
+-rw-r--r--   0        0        0     9935 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      705 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    10446 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0      704 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     9084 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      709 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0    16782 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py
+-rw-r--r--   0        0        0     3314 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/imcc/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/__init__.py
+-rw-r--r--   0        0        0     8415 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/factories.py
+-rw-r--r--   0        0        0    18961 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/protocols.py
+-rw-r--r--   0        0        0     4290 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/utils.py
+-rw-r--r--   0        0        0      291 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/__init__.py
+-rw-r--r--   0        0        0     7871 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/factories.py
+-rw-r--r--   0        0        0    10621 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/protocols.py
+-rw-r--r--   0        0        0      381 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/doh/__init__.py
+-rw-r--r--   0        0        0    22371 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/doq/__init__.py
+-rw-r--r--   0        0        0    15402 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/dot/__init__.py
+-rw-r--r--   0        0        0     5951 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/dou/__init__.py
+-rw-r--r--   0        0        0    11140 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/in_memory/__init__.py
+-rw-r--r--   0        0        0     5299 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py
+-rw-r--r--   0        0        0     2643 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/system/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/system/_socket.py
+-rw-r--r--   0        0        0      381 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/doh/__init__.py
+-rw-r--r--   0        0        0    22180 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/doq/__init__.py
+-rw-r--r--   0        0        0    14846 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/dot/__init__.py
+-rw-r--r--   0        0        0     4493 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/dou/__init__.py
+-rw-r--r--   0        0        0    10836 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/in_memory/__init__.py
+-rw-r--r--   0        0        0     5425 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/in_memory/_dict.py
+-rw-r--r--   0        0        0     2539 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/system/__init__.py
+-rw-r--r--   0        0        0     1626 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/system/_socket.py
+-rw-r--r--   0        0        0    12158 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/contrib/ssa/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/__init__.py
+-rw-r--r--   0        0        0     3884 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/connection.py
+-rw-r--r--   0        0        0     1145 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/proxy.py
+-rw-r--r--   0        0        0     8886 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/request.py
+-rw-r--r--   0        0        0     1329 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/response.py
+-rw-r--r--   0        0        0    19245 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/retry.py
+-rw-r--r--   0        0        0    24783 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/ssl_.py
+-rw-r--r--   0        0        0     5816 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     7226 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/ssltransport.py
+-rw-r--r--   0        0        0    10684 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/timeout.py
+-rw-r--r--   0        0        0    21933 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/traffic_police.py
+-rw-r--r--   0        0        0    15295 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/url.py
+-rw-r--r--   0        0        0     1146 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/util.py
+-rw-r--r--   0        0        0     4423 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/wait.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/_async/__init__.py
+-rw-r--r--   0        0        0     5492 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/_async/ssl_.py
+-rw-r--r--   0        0        0    22050 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/src/urllib3_future/util/_async/traffic_police.py
+-rw-r--r--   0        0        0     9646 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/__init__.py
+-rw-r--r--   0        0        0    11926 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/conftest.py
+-rw-r--r--   0        0        0     6222 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/port_helpers.py
+-rw-r--r--   0        0        0    12638 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_collections.py
+-rw-r--r--   0        0        0      692 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_compatibility.py
+-rw-r--r--   0        0        0    10288 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_connection.py
+-rw-r--r--   0        0        0    22649 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_connectionpool.py
+-rw-r--r--   0        0        0     1531 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_exceptions.py
+-rw-r--r--   0        0        0     3882 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_fields.py
+-rw-r--r--   0        0        0     3778 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_filepost.py
+-rw-r--r--   0        0        0      978 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_no_ssl.py
+-rw-r--r--   0        0        0    17951 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_poolmanager.py
+-rw-r--r--   0        0        0     3657 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_proxymanager.py
+-rw-r--r--   0        0        0    38863 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_response.py
+-rw-r--r--   0        0        0    16640 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_retry.py
+-rw-r--r--   0        0        0     6554 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_ssl.py
+-rw-r--r--   0        0        0    16917 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_ssltransport.py
+-rw-r--r--   0        0        0    43037 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_util.py
+-rw-r--r--   0        0        0     5999 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/test_wait.py
+-rw-r--r--   0        0        0     1187 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/tz_stub.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/contrib/__init__.py
+-rw-r--r--   0        0        0     1257 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/contrib/duplicate_san.pem
+-rw-r--r--   0        0        0    21281 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/contrib/test_resolver.py
+-rw-r--r--   0        0        0    25922 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/contrib/test_socks.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/contrib/asynchronous/__init__.py
+-rw-r--r--   0        0        0    21291 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/contrib/asynchronous/test_resolver.py
+-rw-r--r--   0        0        0    21728 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/contrib/asynchronous/test_socks.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/contrib/hface/__init__.py
+-rw-r--r--   0        0        0     3717 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/contrib/hface/test_stream_matrix.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/__init__.py
+-rw-r--r--   0        0        0     9840 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/test_chunked_transfer.py
+-rw-r--r--   0        0        0     3702 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/test_connection.py
+-rw-r--r--   0        0        0    56059 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/test_connectionpool.py
+-rw-r--r--   0        0        0     7756 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/test_happy_eyeballs.py
+-rw-r--r--   0        0        0    43193 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/test_https.py
+-rw-r--r--   0        0        0     1104 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/test_no_ssl.py
+-rw-r--r--   0        0        0    23853 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/test_poolmanager.py
+-rw-r--r--   0        0        0    32501 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/test_proxy_poolmanager.py
+-rw-r--r--   0        0        0    88179 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/test_socketlevel.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/asynchronous/__init__.py
+-rw-r--r--   0        0        0    59408 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/asynchronous/test_connectionpool.py
+-rw-r--r--   0        0        0     7329 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/asynchronous/test_happy_eyeballs.py
+-rw-r--r--   0        0        0    19562 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_dummyserver/asynchronous/test_poolmanager.py
+-rw-r--r--   0        0        0     2837 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/__init__.py
+-rw-r--r--   0        0        0     3069 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/test_conn_info.py
+-rw-r--r--   0        0        0     3764 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/test_connection.py
+-rw-r--r--   0        0        0     2821 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/test_connection_multiplexed.py
+-rw-r--r--   0        0        0     5912 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/test_connectionpool_multiplexed.py
+-rw-r--r--   0        0        0     1924 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/test_protolevel.py
+-rw-r--r--   0        0        0     3209 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/test_proxy.py
+-rw-r--r--   0        0        0     5658 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/test_send_data.py
+-rw-r--r--   0        0        0     1864 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/test_stream.py
+-rw-r--r--   0        0        0     6683 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/test_svn.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/asynchronous/__init__.py
+-rw-r--r--   0        0        0     2217 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/asynchronous/test_conn_info.py
+-rw-r--r--   0        0        0     4035 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/asynchronous/test_connection.py
+-rw-r--r--   0        0        0     3122 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/asynchronous/test_connection_multiplexed.py
+-rw-r--r--   0        0        0     6143 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py
+-rw-r--r--   0        0        0     2003 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/asynchronous/test_protolevel.py
+-rw-r--r--   0        0        0     3274 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/asynchronous/test_proxy.py
+-rw-r--r--   0        0        0     5880 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/asynchronous/test_send_data.py
+-rw-r--r--   0        0        0     1967 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/asynchronous/test_stream.py
+-rw-r--r--   0        0        0     7217 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/test/with_traefik/asynchronous/test_svn.py
+-rw-r--r--   0        0        0       85 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/.gitignore
+-rw-r--r--   0        0        0     1093 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/LICENSE.txt
+-rw-r--r--   0        0        0     4277 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/README.md
+-rw-r--r--   0        0        0     1342 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/hatch_build.py
+-rw-r--r--   0        0        0     5594 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/pyproject.toml
+-rw-r--r--   0        0        0     7012 2024-05-02 06:05:36.000000 urllib3_future-2.7.906/PKG-INFO
```

### Comparing `urllib3_future-2.7.905/CHANGES.rst` & `urllib3_future-2.7.906/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2.7.906 (2024-05-02)
+====================
+
+- Overall performance improvement with HTTP/2 in a highly concurrent context.
+
 2.7.905 (2024-04-28)
 ====================
 
 - Added support for ``jh2>=5,<6`` instead of ``h2~=4.0`` as a drop-in replacement.
   Expect a significant performance improvement with HTTP/2. We successfully reduced our dependency footprint to the minimum.
 
 2.7.904 (2024-04-20)
```

### Comparing `urllib3_future-2.7.905/docs/Makefile` & `urllib3_future-2.7.906/docs/Makefile`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/advanced-usage.rst` & `urllib3_future-2.7.906/docs/advanced-usage.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/async.rst` & `urllib3_future-2.7.906/docs/async.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/conf.py` & `urllib3_future-2.7.906/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/contributing.rst` & `urllib3_future-2.7.906/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/index.rst` & `urllib3_future-2.7.906/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/make.bat` & `urllib3_future-2.7.906/docs/make.bat`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/user-guide.rst` & `urllib3_future-2.7.906/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/v2-migration-guide.rst` & `urllib3_future-2.7.906/docs/v2-migration-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/_static/banner.svg` & `urllib3_future-2.7.906/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/_static/banner_github.svg` & `urllib3_future-2.7.906/docs/_static/banner_github.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/_static/dark-logo.svg` & `urllib3_future-2.7.906/docs/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/_static/logo.png` & `urllib3_future-2.7.906/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/images/demo-button.png` & `urllib3_future-2.7.906/docs/images/demo-button.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/images/favicon.png` & `urllib3_future-2.7.906/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/images/learn-more-button.png` & `urllib3_future-2.7.906/docs/images/learn-more-button.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/images/logo.png` & `urllib3_future-2.7.906/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/images/logo.svg` & `urllib3_future-2.7.906/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/reference/urllib3.connectionpool.rst` & `urllib3_future-2.7.906/docs/reference/urllib3.connectionpool.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/reference/urllib3.poolmanager.rst` & `urllib3_future-2.7.906/docs/reference/urllib3.poolmanager.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/docs/reference/urllib3.response.rst` & `urllib3_future-2.7.906/docs/reference/urllib3.response.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/dummyserver/handlers.py` & `urllib3_future-2.7.906/dummyserver/handlers.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/dummyserver/https_proxy.py` & `urllib3_future-2.7.906/dummyserver/https_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/dummyserver/proxy.py` & `urllib3_future-2.7.906/dummyserver/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/dummyserver/server.py` & `urllib3_future-2.7.906/dummyserver/server.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/dummyserver/testcase.py` & `urllib3_future-2.7.906/dummyserver/testcase.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/dummyserver/certs/cacert.key` & `urllib3_future-2.7.906/dummyserver/certs/cacert.key`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/dummyserver/certs/cacert.pem` & `urllib3_future-2.7.906/dummyserver/certs/cacert.pem`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/dummyserver/certs/server.crt` & `urllib3_future-2.7.906/dummyserver/certs/server.crt`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/dummyserver/certs/server.key` & `urllib3_future-2.7.906/dummyserver/certs/server.key`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/__init__.py` & `urllib3_future-2.7.906/src/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/_collections.py` & `urllib3_future-2.7.906/src/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/_constant.py` & `urllib3_future-2.7.906/src/urllib3/_constant.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/_request_methods.py` & `urllib3_future-2.7.906/src/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/_typing.py` & `urllib3_future-2.7.906/src/urllib3/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/connection.py` & `urllib3_future-2.7.906/src/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/connectionpool.py` & `urllib3_future-2.7.906/src/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/exceptions.py` & `urllib3_future-2.7.906/src/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/fields.py` & `urllib3_future-2.7.906/src/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/filepost.py` & `urllib3_future-2.7.906/src/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/poolmanager.py` & `urllib3_future-2.7.906/src/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/response.py` & `urllib3_future-2.7.906/src/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/_async/connection.py` & `urllib3_future-2.7.906/src/urllib3/_async/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/_async/connectionpool.py` & `urllib3_future-2.7.906/src/urllib3/_async/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/_async/poolmanager.py` & `urllib3_future-2.7.906/src/urllib3/_async/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/_async/response.py` & `urllib3_future-2.7.906/src/urllib3/_async/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/backend/_base.py` & `urllib3_future-2.7.906/src/urllib3/backend/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,19 @@
         self.status = status
         self.version = version
         self.reason = reason
         self.msg = headers
         self._method = method
 
         self.__internal_read_st = body
-        self.closed = True if self.__internal_read_st is None else False
-        self._eot = True if self.__internal_read_st is None else False
+
+        has_body = self.__internal_read_st is not None
+
+        self.closed = has_body is False
+        self._eot = self.closed
 
         # is kept to determine if we can upgrade conn
         self.authority = authority
         self.port = port
 
         self._stream_id = stream_id
 
@@ -320,14 +323,16 @@
         self._promises_per_stream: dict[int, ResponsePromise] = {}
         self._pending_responses: dict[
             int, LowLevelResponse | AsyncLowLevelResponse
         ] = {}
 
         self._start_last_request: datetime | None = None
 
+        self._cached_http_vsn: int | None = None
+
     def __contains__(self, item: ResponsePromise) -> bool:
         return item.uid in self._promises
 
     @property
     def disabled_svn(self) -> set[HttpVersion]:
         return self._disabled_svn
 
@@ -337,15 +342,17 @@
         assert self._svn is not None
         return self._svn.value
 
     @property
     def _http_vsn(self) -> int:
         """Reimplemented for backward compatibility purposes."""
         assert self._svn is not None
-        return int(self._svn.value.split("/")[-1].replace(".", ""))
+        if self._cached_http_vsn is None:
+            self._cached_http_vsn = int(self._svn.value.split("/")[-1].replace(".", ""))
+        return self._cached_http_vsn
 
     @property
     def is_saturated(self) -> bool:
         raise NotImplementedError
 
     @property
     def is_idle(self) -> bool:
```

### Comparing `urllib3_future-2.7.905/src/urllib3/backend/hface.py` & `urllib3_future-2.7.906/src/urllib3/backend/hface.py`

 * *Files 1% similar despite different names*

```diff
@@ -950,16 +950,16 @@
         ).pop()
 
         headers = HTTPHeaderDict()
         status: int | None = None
 
         for raw_header, raw_value in head_event.headers:
             # special headers that represent (usually) the HTTP response status, version and reason.
-            if raw_header.startswith(b":"):
-                if status is None and raw_header == b":status":
+            if status is None and raw_header[0] == 0x3A:
+                if raw_header == b":status":
                     status = int(raw_value)
             else:
                 headers.add(raw_header.decode("ascii"), raw_value.decode("iso-8859-1"))
 
         if promise is None:
             try:
                 promise = self._promises_per_stream.pop(head_event.stream_id)
@@ -1148,7 +1148,8 @@
         self._promises_per_stream = {}
         self._pending_responses = {}
         self.__custom_tls_settings = None
         self.conn_info = None
         self.__expected_body_length = None
         self.__remaining_body_length = None
         self._start_last_request = None
+        self._cached_http_vsn = None
```

### Comparing `urllib3_future-2.7.905/src/urllib3/backend/_async/_base.py` & `urllib3_future-2.7.906/src/urllib3/backend/_async/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,19 @@
         self.status = status
         self.version = version
         self.reason = reason
         self.msg = headers
         self._method = method
 
         self.__internal_read_st = body
-        self.closed = True if self.__internal_read_st is None else False
-        self._eot = True if self.__internal_read_st is None else False
+
+        has_body = self.__internal_read_st is not None
+
+        self.closed = has_body is False
+        self._eot = self.closed
 
         # is kept to determine if we can upgrade conn
         self.authority = authority
         self.port = port
 
         self._stream_id = stream_id
```

### Comparing `urllib3_future-2.7.905/src/urllib3/backend/_async/hface.py` & `urllib3_future-2.7.906/src/urllib3/backend/_async/hface.py`

 * *Files 1% similar despite different names*

```diff
@@ -903,16 +903,16 @@
                 respect_end_stream_signal=False,
                 stream_id=promise.stream_id if promise else None,
             )
         ).pop()
 
         for raw_header, raw_value in head_event.headers:
             # special headers that represent (usually) the HTTP response status, version and reason.
-            if raw_header.startswith(b":"):
-                if status is None and raw_header == b":status":
+            if status is None and raw_header[0] == 0x3A:
+                if raw_header == b":status":
                     status = int(raw_value)
             else:
                 headers.add(raw_header.decode("ascii"), raw_value.decode("iso-8859-1"))
 
         if promise is None:
             try:
                 promise = self._promises_per_stream.pop(head_event.stream_id)
@@ -1101,7 +1101,8 @@
         self._promises_per_stream = {}
         self._pending_responses = {}
         self.__custom_tls_settings = None
         self.conn_info = None
         self.__expected_body_length = None
         self.__remaining_body_length = None
         self._start_last_request = None
+        self._cached_http_vsn = None
```

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/_socks_override.py` & `urllib3_future-2.7.906/src/urllib3/contrib/_socks_override.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/pyopenssl.py` & `urllib3_future-2.7.906/src/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/socks.py` & `urllib3_future-2.7.906/src/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/__init__.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/_configuration.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/_error_codes.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/_stream_matrix.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/_stream_matrix.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/_typing.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/events/__init__.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/events/_events.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/__init__.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/_factories.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/_protocols.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http1/__init__.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http1/_h11.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http1/_h11.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http2/__init__.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http2/_h2.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http2/_h2.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,24 +78,24 @@
             observable_impl=self,
         )
         self._open_stream_count: int = 0
         self._connection.initiate_connection()
         self._events: StreamMatrix = StreamMatrix()
         self._terminated: bool = False
         self._goaway_to_honor: bool = False
+        self._max_stream_count = self._connection.remote_settings.max_concurrent_streams
 
     @staticmethod
     def exceptions() -> tuple[type[BaseException], ...]:
         return jh2.exceptions.ProtocolError, jh2.exceptions.H2Error
 
     def is_available(self) -> bool:
-        if self._goaway_to_honor:
+        if self._terminated or self._goaway_to_honor:
             return False
-        max_streams = self._connection.remote_settings.max_concurrent_streams
-        return self._terminated is False and max_streams > self._open_stream_count
+        return self._max_stream_count > self._open_stream_count  # type: ignore[no-any-return]
 
     def is_idle(self) -> bool:
         return self._terminated is False and self._open_stream_count == 0
 
     def has_expired(self) -> bool:
         return self._terminated or self._goaway_to_honor
 
@@ -192,14 +192,19 @@
         try:
             h2_events = self._connection.receive_data(data)
         except jh2.exceptions.ProtocolError as e:
             self._connection_terminated(e.error_code, str(e))
         else:
             self._events.extend(self._map_events(h2_events))
 
+        if self._connection.remote_settings.has_update:
+            self._max_stream_count = (
+                self._connection.remote_settings.max_concurrent_streams
+            )
+
     def bytes_to_send(self) -> bytes:
         return self._connection.data_to_send()  # type: ignore[no-any-return]
 
     def _connection_terminated(
         self, error_code: int = 0, message: str | None = None
     ) -> None:
         if self._terminated:
```

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http3/__init__.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/hface/protocols/http3/_qh3.py` & `urllib3_future-2.7.906/src/urllib3/contrib/hface/protocols/http3/_qh3.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,24 +215,14 @@
             for h3_event in self._http.handle_event(quic_event):
                 self._events.extend(self._map_h3_event(h3_event))
 
         if hasattr(self._quic, "_close_event") and self._quic._close_event is not None:
             self._events.extend(self._map_quic_event(self._quic._close_event))
 
     def _map_quic_event(self, quic_event: quic_events.QuicEvent) -> Iterable[Event]:
-        if isinstance(quic_event, quic_events.ConnectionIdIssued):
-            self._connection_ids.add(quic_event.connection_id)
-        elif isinstance(quic_event, quic_events.ConnectionIdRetired):
-            try:
-                self._connection_ids.remove(quic_event.connection_id)
-            except (
-                KeyError
-            ):  # it is surprising, learn more about this with aioquic maintainer.
-                pass
-
         if isinstance(quic_event, quic_events.HandshakeCompleted):
             yield _HandshakeCompleted(quic_event.alpn_protocol)
         elif isinstance(quic_event, quic_events.ConnectionTerminated):
             self._terminated = True
             yield ConnectionTerminated(quic_event.error_code, quic_event.reason_phrase)
         elif isinstance(quic_event, quic_events.StreamReset):
             self._open_stream_count -= 1
```

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/imcc/__init__.py` & `urllib3_future-2.7.906/src/urllib3/contrib/imcc/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/factories.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/protocols.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/utils.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/factories.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/protocols.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/doh/_urllib3.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/doq/_qh3.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/dot/_ssl.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/dou/_socket.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/in_memory/_dict.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/null/__init__.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/_async/system/_socket.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/_async/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/doh/_urllib3.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/doq/_qh3.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/dot/_ssl.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/dou/_socket.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/in_memory/_dict.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/null/__init__.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/resolver/system/_socket.py` & `urllib3_future-2.7.906/src/urllib3/contrib/resolver/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/contrib/ssa/__init__.py` & `urllib3_future-2.7.906/src/urllib3/contrib/ssa/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/__init__.py` & `urllib3_future-2.7.906/src/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/connection.py` & `urllib3_future-2.7.906/src/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/proxy.py` & `urllib3_future-2.7.906/src/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/request.py` & `urllib3_future-2.7.906/src/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/response.py` & `urllib3_future-2.7.906/src/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/retry.py` & `urllib3_future-2.7.906/src/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/ssl_.py` & `urllib3_future-2.7.906/src/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/ssl_match_hostname.py` & `urllib3_future-2.7.906/src/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/ssltransport.py` & `urllib3_future-2.7.906/src/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/timeout.py` & `urllib3_future-2.7.906/src/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/traffic_police.py` & `urllib3_future-2.7.906/src/urllib3/util/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/url.py` & `urllib3_future-2.7.906/src/urllib3/util/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,14 +345,15 @@
             raise LocationParseError(
                 f"Name '{name}' is not a valid IDNA label"
             ) from None
 
     return name.lower().encode("ascii")
 
 
+@lru_cache(maxsize=1024)
 def _encode_target(target: str) -> str:
     """Percent-encodes a request target so that there are no invalid characters
 
     Pre-condition for this function is that 'target' must start with '/'.
     If that is the case then _TARGET_RE will always produce a match.
     """
     match = _TARGET_RE.match(target)
```

### Comparing `urllib3_future-2.7.905/src/urllib3/util/util.py` & `urllib3_future-2.7.906/src/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/wait.py` & `urllib3_future-2.7.906/src/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/_async/ssl_.py` & `urllib3_future-2.7.906/src/urllib3/util/_async/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3/util/_async/traffic_police.py` & `urllib3_future-2.7.906/src/urllib3/util/_async/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/_collections.py` & `urllib3_future-2.7.906/src/urllib3_future/_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/_constant.py` & `urllib3_future-2.7.906/src/urllib3_future/_constant.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/_request_methods.py` & `urllib3_future-2.7.906/src/urllib3_future/_request_methods.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/_typing.py` & `urllib3_future-2.7.906/src/urllib3_future/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/connection.py` & `urllib3_future-2.7.906/src/urllib3_future/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/connectionpool.py` & `urllib3_future-2.7.906/src/urllib3_future/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/exceptions.py` & `urllib3_future-2.7.906/src/urllib3_future/exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/fields.py` & `urllib3_future-2.7.906/src/urllib3_future/fields.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/filepost.py` & `urllib3_future-2.7.906/src/urllib3_future/filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/poolmanager.py` & `urllib3_future-2.7.906/src/urllib3_future/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/response.py` & `urllib3_future-2.7.906/src/urllib3_future/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/_async/connection.py` & `urllib3_future-2.7.906/src/urllib3_future/_async/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/_async/connectionpool.py` & `urllib3_future-2.7.906/src/urllib3_future/_async/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/_async/poolmanager.py` & `urllib3_future-2.7.906/src/urllib3_future/_async/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/_async/response.py` & `urllib3_future-2.7.906/src/urllib3_future/_async/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/backend/_base.py` & `urllib3_future-2.7.906/src/urllib3_future/backend/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,19 @@
         self.status = status
         self.version = version
         self.reason = reason
         self.msg = headers
         self._method = method
 
         self.__internal_read_st = body
-        self.closed = True if self.__internal_read_st is None else False
-        self._eot = True if self.__internal_read_st is None else False
+
+        has_body = self.__internal_read_st is not None
+
+        self.closed = has_body is False
+        self._eot = self.closed
 
         # is kept to determine if we can upgrade conn
         self.authority = authority
         self.port = port
 
         self._stream_id = stream_id
 
@@ -320,14 +323,16 @@
         self._promises_per_stream: dict[int, ResponsePromise] = {}
         self._pending_responses: dict[
             int, LowLevelResponse | AsyncLowLevelResponse
         ] = {}
 
         self._start_last_request: datetime | None = None
 
+        self._cached_http_vsn: int | None = None
+
     def __contains__(self, item: ResponsePromise) -> bool:
         return item.uid in self._promises
 
     @property
     def disabled_svn(self) -> set[HttpVersion]:
         return self._disabled_svn
 
@@ -337,15 +342,17 @@
         assert self._svn is not None
         return self._svn.value
 
     @property
     def _http_vsn(self) -> int:
         """Reimplemented for backward compatibility purposes."""
         assert self._svn is not None
-        return int(self._svn.value.split("/")[-1].replace(".", ""))
+        if self._cached_http_vsn is None:
+            self._cached_http_vsn = int(self._svn.value.split("/")[-1].replace(".", ""))
+        return self._cached_http_vsn
 
     @property
     def is_saturated(self) -> bool:
         raise NotImplementedError
 
     @property
     def is_idle(self) -> bool:
```

### Comparing `urllib3_future-2.7.905/src/urllib3_future/backend/hface.py` & `urllib3_future-2.7.906/src/urllib3_future/backend/hface.py`

 * *Files 1% similar despite different names*

```diff
@@ -950,16 +950,16 @@
         ).pop()
 
         headers = HTTPHeaderDict()
         status: int | None = None
 
         for raw_header, raw_value in head_event.headers:
             # special headers that represent (usually) the HTTP response status, version and reason.
-            if raw_header.startswith(b":"):
-                if status is None and raw_header == b":status":
+            if status is None and raw_header[0] == 0x3A:
+                if raw_header == b":status":
                     status = int(raw_value)
             else:
                 headers.add(raw_header.decode("ascii"), raw_value.decode("iso-8859-1"))
 
         if promise is None:
             try:
                 promise = self._promises_per_stream.pop(head_event.stream_id)
@@ -1148,7 +1148,8 @@
         self._promises_per_stream = {}
         self._pending_responses = {}
         self.__custom_tls_settings = None
         self.conn_info = None
         self.__expected_body_length = None
         self.__remaining_body_length = None
         self._start_last_request = None
+        self._cached_http_vsn = None
```

### Comparing `urllib3_future-2.7.905/src/urllib3_future/backend/_async/_base.py` & `urllib3_future-2.7.906/src/urllib3_future/backend/_async/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,19 @@
         self.status = status
         self.version = version
         self.reason = reason
         self.msg = headers
         self._method = method
 
         self.__internal_read_st = body
-        self.closed = True if self.__internal_read_st is None else False
-        self._eot = True if self.__internal_read_st is None else False
+
+        has_body = self.__internal_read_st is not None
+
+        self.closed = has_body is False
+        self._eot = self.closed
 
         # is kept to determine if we can upgrade conn
         self.authority = authority
         self.port = port
 
         self._stream_id = stream_id
```

### Comparing `urllib3_future-2.7.905/src/urllib3_future/backend/_async/hface.py` & `urllib3_future-2.7.906/src/urllib3_future/backend/_async/hface.py`

 * *Files 1% similar despite different names*

```diff
@@ -903,16 +903,16 @@
                 respect_end_stream_signal=False,
                 stream_id=promise.stream_id if promise else None,
             )
         ).pop()
 
         for raw_header, raw_value in head_event.headers:
             # special headers that represent (usually) the HTTP response status, version and reason.
-            if raw_header.startswith(b":"):
-                if status is None and raw_header == b":status":
+            if status is None and raw_header[0] == 0x3A:
+                if raw_header == b":status":
                     status = int(raw_value)
             else:
                 headers.add(raw_header.decode("ascii"), raw_value.decode("iso-8859-1"))
 
         if promise is None:
             try:
                 promise = self._promises_per_stream.pop(head_event.stream_id)
@@ -1101,7 +1101,8 @@
         self._promises_per_stream = {}
         self._pending_responses = {}
         self.__custom_tls_settings = None
         self.conn_info = None
         self.__expected_body_length = None
         self.__remaining_body_length = None
         self._start_last_request = None
+        self._cached_http_vsn = None
```

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/_socks_override.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/_socks_override.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/pyopenssl.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/socks.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/_configuration.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/_error_codes.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/_stream_matrix.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/_stream_matrix.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/_typing.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/events/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/events/_events.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/_factories.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/_protocols.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http1/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http1/_h11.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http1/_h11.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http2/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http2/_h2.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http2/_h2.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,24 +78,24 @@
             observable_impl=self,
         )
         self._open_stream_count: int = 0
         self._connection.initiate_connection()
         self._events: StreamMatrix = StreamMatrix()
         self._terminated: bool = False
         self._goaway_to_honor: bool = False
+        self._max_stream_count = self._connection.remote_settings.max_concurrent_streams
 
     @staticmethod
     def exceptions() -> tuple[type[BaseException], ...]:
         return jh2.exceptions.ProtocolError, jh2.exceptions.H2Error
 
     def is_available(self) -> bool:
-        if self._goaway_to_honor:
+        if self._terminated or self._goaway_to_honor:
             return False
-        max_streams = self._connection.remote_settings.max_concurrent_streams
-        return self._terminated is False and max_streams > self._open_stream_count
+        return self._max_stream_count > self._open_stream_count  # type: ignore[no-any-return]
 
     def is_idle(self) -> bool:
         return self._terminated is False and self._open_stream_count == 0
 
     def has_expired(self) -> bool:
         return self._terminated or self._goaway_to_honor
 
@@ -192,14 +192,19 @@
         try:
             h2_events = self._connection.receive_data(data)
         except jh2.exceptions.ProtocolError as e:
             self._connection_terminated(e.error_code, str(e))
         else:
             self._events.extend(self._map_events(h2_events))
 
+        if self._connection.remote_settings.has_update:
+            self._max_stream_count = (
+                self._connection.remote_settings.max_concurrent_streams
+            )
+
     def bytes_to_send(self) -> bytes:
         return self._connection.data_to_send()  # type: ignore[no-any-return]
 
     def _connection_terminated(
         self, error_code: int = 0, message: str | None = None
     ) -> None:
         if self._terminated:
```

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http3/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,24 +215,14 @@
             for h3_event in self._http.handle_event(quic_event):
                 self._events.extend(self._map_h3_event(h3_event))
 
         if hasattr(self._quic, "_close_event") and self._quic._close_event is not None:
             self._events.extend(self._map_quic_event(self._quic._close_event))
 
     def _map_quic_event(self, quic_event: quic_events.QuicEvent) -> Iterable[Event]:
-        if isinstance(quic_event, quic_events.ConnectionIdIssued):
-            self._connection_ids.add(quic_event.connection_id)
-        elif isinstance(quic_event, quic_events.ConnectionIdRetired):
-            try:
-                self._connection_ids.remove(quic_event.connection_id)
-            except (
-                KeyError
-            ):  # it is surprising, learn more about this with aioquic maintainer.
-                pass
-
         if isinstance(quic_event, quic_events.HandshakeCompleted):
             yield _HandshakeCompleted(quic_event.alpn_protocol)
         elif isinstance(quic_event, quic_events.ConnectionTerminated):
             self._terminated = True
             yield ConnectionTerminated(quic_event.error_code, quic_event.reason_phrase)
         elif isinstance(quic_event, quic_events.StreamReset):
             self._open_stream_count -= 1
```

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/imcc/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/imcc/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/factories.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/protocols.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/utils.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/factories.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/protocols.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/dou/_socket.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/null/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/_async/system/_socket.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/_async/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/doh/_urllib3.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/doq/_qh3.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/dot/_ssl.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/dou/_socket.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/in_memory/_dict.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/null/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/resolver/system/_socket.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/resolver/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/contrib/ssa/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/contrib/ssa/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/__init__.py` & `urllib3_future-2.7.906/src/urllib3_future/util/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/connection.py` & `urllib3_future-2.7.906/src/urllib3_future/util/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/proxy.py` & `urllib3_future-2.7.906/src/urllib3_future/util/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/request.py` & `urllib3_future-2.7.906/src/urllib3_future/util/request.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/response.py` & `urllib3_future-2.7.906/src/urllib3_future/util/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/retry.py` & `urllib3_future-2.7.906/src/urllib3_future/util/retry.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/ssl_.py` & `urllib3_future-2.7.906/src/urllib3_future/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/ssl_match_hostname.py` & `urllib3_future-2.7.906/src/urllib3_future/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/ssltransport.py` & `urllib3_future-2.7.906/src/urllib3_future/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/timeout.py` & `urllib3_future-2.7.906/src/urllib3_future/util/timeout.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/traffic_police.py` & `urllib3_future-2.7.906/src/urllib3_future/util/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/url.py` & `urllib3_future-2.7.906/src/urllib3_future/util/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,14 +345,15 @@
             raise LocationParseError(
                 f"Name '{name}' is not a valid IDNA label"
             ) from None
 
     return name.lower().encode("ascii")
 
 
+@lru_cache(maxsize=1024)
 def _encode_target(target: str) -> str:
     """Percent-encodes a request target so that there are no invalid characters
 
     Pre-condition for this function is that 'target' must start with '/'.
     If that is the case then _TARGET_RE will always produce a match.
     """
     match = _TARGET_RE.match(target)
```

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/util.py` & `urllib3_future-2.7.906/src/urllib3_future/util/util.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/wait.py` & `urllib3_future-2.7.906/src/urllib3_future/util/wait.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/_async/ssl_.py` & `urllib3_future-2.7.906/src/urllib3_future/util/_async/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/src/urllib3_future/util/_async/traffic_police.py` & `urllib3_future-2.7.906/src/urllib3_future/util/_async/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/__init__.py` & `urllib3_future-2.7.906/test/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/conftest.py` & `urllib3_future-2.7.906/test/conftest.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/port_helpers.py` & `urllib3_future-2.7.906/test/port_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_collections.py` & `urllib3_future-2.7.906/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_compatibility.py` & `urllib3_future-2.7.906/test/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_connection.py` & `urllib3_future-2.7.906/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_connectionpool.py` & `urllib3_future-2.7.906/test/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_exceptions.py` & `urllib3_future-2.7.906/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_fields.py` & `urllib3_future-2.7.906/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_filepost.py` & `urllib3_future-2.7.906/test/test_filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_no_ssl.py` & `urllib3_future-2.7.906/test/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_poolmanager.py` & `urllib3_future-2.7.906/test/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_proxymanager.py` & `urllib3_future-2.7.906/test/test_proxymanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_response.py` & `urllib3_future-2.7.906/test/test_response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_retry.py` & `urllib3_future-2.7.906/test/test_retry.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_ssl.py` & `urllib3_future-2.7.906/test/test_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_ssltransport.py` & `urllib3_future-2.7.906/test/test_ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_util.py` & `urllib3_future-2.7.906/test/test_util.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/test_wait.py` & `urllib3_future-2.7.906/test/test_wait.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/tz_stub.py` & `urllib3_future-2.7.906/test/tz_stub.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/contrib/duplicate_san.pem` & `urllib3_future-2.7.906/test/contrib/duplicate_san.pem`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/contrib/test_resolver.py` & `urllib3_future-2.7.906/test/contrib/test_resolver.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/contrib/test_socks.py` & `urllib3_future-2.7.906/test/contrib/test_socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/contrib/asynchronous/test_resolver.py` & `urllib3_future-2.7.906/test/contrib/asynchronous/test_resolver.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/contrib/asynchronous/test_socks.py` & `urllib3_future-2.7.906/test/contrib/asynchronous/test_socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/contrib/hface/test_stream_matrix.py` & `urllib3_future-2.7.906/test/contrib/hface/test_stream_matrix.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/test_chunked_transfer.py` & `urllib3_future-2.7.906/test/with_dummyserver/test_chunked_transfer.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/test_connection.py` & `urllib3_future-2.7.906/test/with_dummyserver/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/test_connectionpool.py` & `urllib3_future-2.7.906/test/with_dummyserver/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/test_happy_eyeballs.py` & `urllib3_future-2.7.906/test/with_dummyserver/test_happy_eyeballs.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/test_https.py` & `urllib3_future-2.7.906/test/with_dummyserver/test_https.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/test_no_ssl.py` & `urllib3_future-2.7.906/test/with_dummyserver/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/test_poolmanager.py` & `urllib3_future-2.7.906/test/with_dummyserver/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/test_proxy_poolmanager.py` & `urllib3_future-2.7.906/test/with_dummyserver/test_proxy_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/test_socketlevel.py` & `urllib3_future-2.7.906/test/with_dummyserver/test_socketlevel.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/asynchronous/test_connectionpool.py` & `urllib3_future-2.7.906/test/with_dummyserver/asynchronous/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/asynchronous/test_happy_eyeballs.py` & `urllib3_future-2.7.906/test/with_dummyserver/asynchronous/test_happy_eyeballs.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_dummyserver/asynchronous/test_poolmanager.py` & `urllib3_future-2.7.906/test/with_dummyserver/asynchronous/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/__init__.py` & `urllib3_future-2.7.906/test/with_traefik/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/test_conn_info.py` & `urllib3_future-2.7.906/test/with_traefik/test_conn_info.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/test_connection.py` & `urllib3_future-2.7.906/test/with_traefik/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/test_connection_multiplexed.py` & `urllib3_future-2.7.906/test/with_traefik/test_connection_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/test_connectionpool_multiplexed.py` & `urllib3_future-2.7.906/test/with_traefik/test_connectionpool_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/test_protolevel.py` & `urllib3_future-2.7.906/test/with_traefik/test_protolevel.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/test_proxy.py` & `urllib3_future-2.7.906/test/with_traefik/test_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/test_send_data.py` & `urllib3_future-2.7.906/test/with_traefik/test_send_data.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/test_stream.py` & `urllib3_future-2.7.906/test/with_traefik/test_stream.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/test_svn.py` & `urllib3_future-2.7.906/test/with_traefik/test_svn.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/asynchronous/test_conn_info.py` & `urllib3_future-2.7.906/test/with_traefik/asynchronous/test_conn_info.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/asynchronous/test_connection.py` & `urllib3_future-2.7.906/test/with_traefik/asynchronous/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/asynchronous/test_connection_multiplexed.py` & `urllib3_future-2.7.906/test/with_traefik/asynchronous/test_connection_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py` & `urllib3_future-2.7.906/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/asynchronous/test_protolevel.py` & `urllib3_future-2.7.906/test/with_traefik/asynchronous/test_protolevel.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/asynchronous/test_proxy.py` & `urllib3_future-2.7.906/test/with_traefik/asynchronous/test_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/asynchronous/test_send_data.py` & `urllib3_future-2.7.906/test/with_traefik/asynchronous/test_send_data.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/asynchronous/test_stream.py` & `urllib3_future-2.7.906/test/with_traefik/asynchronous/test_stream.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/test/with_traefik/asynchronous/test_svn.py` & `urllib3_future-2.7.906/test/with_traefik/asynchronous/test_svn.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/LICENSE.txt` & `urllib3_future-2.7.906/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/README.md` & `urllib3_future-2.7.906/README.md`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/hatch_build.py` & `urllib3_future-2.7.906/hatch_build.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.905/pyproject.toml` & `urllib3_future-2.7.906/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
   "qh3>=1.0.3,<2.0.0; (platform_system == 'Darwin' or platform_system == 'Windows' or platform_system == 'Linux') and (platform_machine == 'x86_64' or platform_machine == 's390x' or platform_machine == 'aarch64' or platform_machine == 'armv7l' or platform_machine == 'ppc64le' or platform_machine == 'ppc64' or platform_machine == 'AMD64' or platform_machine == 'arm64') and (platform_python_implementation == 'CPython' or (platform_python_implementation == 'PyPy' and python_version < '3.11'))",
   "h11>=0.11.0,<1.0.0",
-  "jh2>=5.0.0,<6.0.0",
+  "jh2>=5.0.3,<6.0.0",
 ]
 
 [project.optional-dependencies]
 brotli = [
   "brotli>=1.0.9; platform_python_implementation == 'CPython'",
   "brotlicffi>=0.8.0; platform_python_implementation != 'CPython'"
 ]
```

### Comparing `urllib3_future-2.7.905/PKG-INFO` & `urllib3_future-2.7.906/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: urllib3-future
-Version: 2.7.905
+Version: 2.7.906
 Summary: urllib3.future is a powerful HTTP 1.1, 2, and 3 client with both sync and async interfaces
 Project-URL: Changelog, https://github.com/jawah/urllib3.future/blob/main/CHANGES.rst
 Project-URL: Documentation, https://urllib3future.readthedocs.io
 Project-URL: Code, https://github.com/jawah/urllib3.future
 Project-URL: Issue tracker, https://github.com/jawah/urllib3.future/issues
 Author-email: Andrey Petrov <andrey.petrov@shazow.net>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Requires-Dist: h11<1.0.0,>=0.11.0
-Requires-Dist: jh2<6.0.0,>=5.0.0
+Requires-Dist: jh2<6.0.0,>=5.0.3
 Requires-Dist: qh3<2.0.0,>=1.0.3; (platform_system == 'Darwin' or platform_system == 'Windows' or platform_system == 'Linux') and (platform_machine == 'x86_64' or platform_machine == 's390x' or platform_machine == 'aarch64' or platform_machine == 'armv7l' or platform_machine == 'ppc64le' or platform_machine == 'ppc64' or platform_machine == 'AMD64' or platform_machine == 'arm64') and (platform_python_implementation == 'CPython' or (platform_python_implementation == 'PyPy' and python_version < '3.11'))
 Provides-Extra: brotli
 Requires-Dist: brotli>=1.0.9; (platform_python_implementation == 'CPython') and extra == 'brotli'
 Requires-Dist: brotlicffi>=0.8.0; (platform_python_implementation != 'CPython') and extra == 'brotli'
 Provides-Extra: qh3
 Requires-Dist: qh3<2.0.0,>=1.0.3; extra == 'qh3'
 Provides-Extra: secure
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: urllib3-future Version: 2.7.905 Summary:
+Metadata-Version: 2.3 Name: urllib3-future Version: 2.7.906 Summary:
 urllib3.future is a powerful HTTP 1.1, 2, and 3 client with both sync and async
 interfaces Project-URL: Changelog, https://github.com/jawah/urllib3.future/
 blob/main/CHANGES.rst Project-URL: Documentation, https://
 urllib3future.readthedocs.io Project-URL: Code, https://github.com/jawah/
 urllib3.future Project-URL: Issue tracker, https://github.com/jawah/
 urllib3.future/issues Author-email: Andrey Petrov
 shazow.net> Maintainer-email: "Ahmed R. TAHRI"
@@ -17,15 +17,15 @@
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Classifier: Topic :: Internet :: WWW/HTTP Classifier:
 Topic :: Software Development :: Libraries Requires-Python: >=3.7 Requires-
-Dist: h11<1.0.0,>=0.11.0 Requires-Dist: jh2<6.0.0,>=5.0.0 Requires-Dist:
+Dist: h11<1.0.0,>=0.11.0 Requires-Dist: jh2<6.0.0,>=5.0.3 Requires-Dist:
 qh3<2.0.0,>=1.0.3; (platform_system == 'Darwin' or platform_system == 'Windows'
 or platform_system == 'Linux') and (platform_machine == 'x86_64' or
 platform_machine == 's390x' or platform_machine == 'aarch64' or
 platform_machine == 'armv7l' or platform_machine == 'ppc64le' or
 platform_machine == 'ppc64' or platform_machine == 'AMD64' or platform_machine
 == 'arm64') and (platform_python_implementation == 'CPython' or
 (platform_python_implementation == 'PyPy' and python_version < '3.11'))
```

