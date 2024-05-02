# Comparing `tmp/packg-0.9.2.tar.gz` & `tmp/packg-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.9.2.tar", last modified: Sat Jan 27 12:11:05 2024, max compression
+gzip compressed data, was "packg-0.9.3.tar", last modified: Sat Jan 27 12:29:53 2024, max compression
```

## Comparing `packg-0.9.2.tar` & `packg-0.9.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:11:05.286025 packg-0.9.2/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11339 2024-01-22 09:09:11.000000 packg-0.9.2/LICENSE
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3803 2024-01-27 12:11:05.282025 packg-0.9.2/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)     2687 2024-01-27 12:10:49.000000 packg-0.9.2/README.md
--rw-------   0 gings    (14999) lmb-mit   (1061)     2631 2024-01-22 09:09:11.000000 packg-0.9.2/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)      120 2024-01-27 12:10:49.000000 packg-0.9.2/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2024-01-27 12:11:05.286025 packg-0.9.2/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:11:05.086021 packg-0.9.2/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:11:05.150022 packg-0.9.2/src/packg/
--rw-------   0 gings    (14999) lmb-mit   (1061)      128 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      120 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/__main__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3132 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/caching.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5819 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/constclass.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1055 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/debugging.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2551 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/dtime.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:11:05.218024 packg-0.9.2/src/packg/iotools/
--rw-------   0 gings    (14999) lmb-mit   (1061)     1645 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4260 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/compressed.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5423 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/file_indexer.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3332 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/file_reader.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1231 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/git_root_finder.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3457 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/git_status_checker.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6849 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/jsonext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    11571 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/jsonext_encoder.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1090 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1056 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/numpyext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5108 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/pathspec_matcher.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      971 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/tomlext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4863 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/iotools/yamlext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     7136 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/log.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1231 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/magic.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      644 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/maths.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1386 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/misc.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:11:05.226024 packg-0.9.2/src/packg/multiproc/
--rw-------   0 gings    (14999) lmb-mit   (1061)      441 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/multiproc/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     7524 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/multiproc/multiproc_fn.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    14843 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/multiproc/multiproc_producer_consumer.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     7152 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/packaging.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3700 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/paths.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:11:05.242024 packg-0.9.2/src/packg/run/
--rw-------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/run/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2213 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/run/cleanup.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1374 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/run/create_autocomplete.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      148 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/run/print_paths.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      148 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/run/show_env.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1771 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/stats.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:11:05.254024 packg-0.9.2/src/packg/strings/
--rw-------   0 gings    (14999) lmb-mit   (1061)      343 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/strings/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4842 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/strings/abbreviations.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2460 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/strings/base64tools.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      790 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/strings/hasher.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      639 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/strings/quote_urlparse.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:11:05.262024 packg-0.9.2/src/packg/system/
--rw-------   0 gings    (14999) lmb-mit   (1061)      174 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/system/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2070 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/system/systemcall.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:11:05.274025 packg-0.9.2/src/packg/testing/
--rw-------   0 gings    (14999) lmb-mit   (1061)       88 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/testing/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1190 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/testing/fixture_webserver.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     8371 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/testing/import_from_source.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2203 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/testing/setup_tests.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      956 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/tqdmext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      643 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/typext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3446 2024-01-27 12:10:49.000000 packg-0.9.2/src/packg/web.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:11:05.278025 packg-0.9.2/src/packg.egg-info/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3803 2024-01-27 12:11:05.000000 packg-0.9.2/src/packg.egg-info/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1614 2024-01-27 12:11:05.000000 packg-0.9.2/src/packg.egg-info/SOURCES.txt
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)        1 2024-01-27 12:11:05.000000 packg-0.9.2/src/packg.egg-info/dependency_links.txt
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      120 2024-01-27 12:11:05.000000 packg-0.9.2/src/packg.egg-info/requires.txt
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)        6 2024-01-27 12:11:05.000000 packg-0.9.2/src/packg.egg-info/top_level.txt
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)        1 2023-06-25 20:37:56.000000 packg-0.9.2/src/packg.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:53.236946 packg-0.9.3/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11339 2024-01-22 09:09:11.000000 packg-0.9.3/LICENSE
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3803 2024-01-27 12:29:53.232946 packg-0.9.3/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2687 2024-01-27 12:29:37.000000 packg-0.9.3/README.md
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2631 2024-01-22 09:09:11.000000 packg-0.9.3/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)      120 2024-01-27 12:29:37.000000 packg-0.9.3/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2024-01-27 12:29:53.236946 packg-0.9.3/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:53.024942 packg-0.9.3/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:53.088943 packg-0.9.3/src/packg/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      128 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      120 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/__main__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3132 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/caching.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5819 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/constclass.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1055 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/debugging.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2551 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/dtime.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:53.152945 packg-0.9.3/src/packg/iotools/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1645 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4260 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/compressed.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5423 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/file_indexer.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3332 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/file_reader.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1231 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/git_root_finder.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3457 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/git_status_checker.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6849 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/jsonext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11571 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/jsonext_encoder.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1090 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1056 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/numpyext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5108 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/pathspec_matcher.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      971 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/tomlext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4863 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/iotools/yamlext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     7237 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/log.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1231 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/magic.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      644 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/maths.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1386 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/misc.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:53.160945 packg-0.9.3/src/packg/multiproc/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      441 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/multiproc/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     7524 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/multiproc/multiproc_fn.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    14843 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/multiproc/multiproc_producer_consumer.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     7152 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/packaging.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3700 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/paths.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:53.180945 packg-0.9.3/src/packg/run/
+-rw-------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/run/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2213 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/run/cleanup.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1374 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/run/create_autocomplete.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      148 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/run/print_paths.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      148 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/run/show_env.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1771 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/stats.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:53.200945 packg-0.9.3/src/packg/strings/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      343 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/strings/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4842 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/strings/abbreviations.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2460 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/strings/base64tools.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      790 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/strings/hasher.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      639 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/strings/quote_urlparse.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:53.204946 packg-0.9.3/src/packg/system/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      174 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/system/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2070 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/system/systemcall.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:53.220946 packg-0.9.3/src/packg/testing/
+-rw-------   0 gings    (14999) lmb-mit   (1061)       88 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/testing/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1190 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/testing/fixture_webserver.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     8371 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/testing/import_from_source.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2203 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/testing/setup_tests.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      956 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/tqdmext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      643 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/typext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3446 2024-01-27 12:29:37.000000 packg-0.9.3/src/packg/web.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-27 12:29:53.224946 packg-0.9.3/src/packg.egg-info/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3803 2024-01-27 12:29:52.000000 packg-0.9.3/src/packg.egg-info/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1614 2024-01-27 12:29:52.000000 packg-0.9.3/src/packg.egg-info/SOURCES.txt
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)        1 2024-01-27 12:29:52.000000 packg-0.9.3/src/packg.egg-info/dependency_links.txt
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      120 2024-01-27 12:29:52.000000 packg-0.9.3/src/packg.egg-info/requires.txt
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)        6 2024-01-27 12:29:52.000000 packg-0.9.3/src/packg.egg-info/top_level.txt
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)        1 2023-06-25 20:37:56.000000 packg-0.9.3/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.9.2/LICENSE` & `packg-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/PKG-INFO` & `packg-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.9.2
+Version: 0.9.3
 Summary: Collection of utilities used in other python projects.
 Author: simonging
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/simonging/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.9.2 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.9.3 Summary: Collection of
 utilities used in other python projects. Author: simonging License: Apache-2.0
 Project-URL: Project-URL, https://github.com/simonging/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.9.2/README.md` & `packg-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/pyproject.toml` & `packg-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/caching.py` & `packg-0.9.3/src/packg/caching.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/constclass.py` & `packg-0.9.3/src/packg/constclass.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/debugging.py` & `packg-0.9.3/src/packg/debugging.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/dtime.py` & `packg-0.9.3/src/packg/dtime.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/__init__.py` & `packg-0.9.3/src/packg/iotools/__init__.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/compressed.py` & `packg-0.9.3/src/packg/iotools/compressed.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/file_indexer.py` & `packg-0.9.3/src/packg/iotools/file_indexer.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/file_reader.py` & `packg-0.9.3/src/packg/iotools/file_reader.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/git_root_finder.py` & `packg-0.9.3/src/packg/iotools/git_root_finder.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/git_status_checker.py` & `packg-0.9.3/src/packg/iotools/git_status_checker.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/jsonext.py` & `packg-0.9.3/src/packg/iotools/jsonext.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/jsonext_encoder.py` & `packg-0.9.3/src/packg/iotools/jsonext_encoder.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/misc.py` & `packg-0.9.3/src/packg/iotools/misc.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/numpyext.py` & `packg-0.9.3/src/packg/iotools/numpyext.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/pathspec_matcher.py` & `packg-0.9.3/src/packg/iotools/pathspec_matcher.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/tomlext.py` & `packg-0.9.3/src/packg/iotools/tomlext.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/iotools/yamlext.py` & `packg-0.9.3/src/packg/iotools/yamlext.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/log.py` & `packg-0.9.3/src/packg/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 from __future__ import annotations
 
 import logging
 import os
 import sys
 from copy import deepcopy
 from logging import getLevelName
+from typing import Union
 
 from loguru import logger
 from pathspec import PathSpec
 
 from packg.iotools.pathspec_matcher import make_pathspec
+from typedparser import VerboseQuietArgs
 
-LevelType = str | int  # either "DEBUG" or 10
+LevelType = Union[str, int]  # either "DEBUG" or 10
 DEFAULT_LOGURU_FORMAT = (
     "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}</level> | "
     "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - "
     "<level>{message}</level>"
 )
 SHORTER_FORMAT = (
     "<green>{time:YYYYMMDD HH:mm:ss}</green> <level>{level: <4.4}</level> "
@@ -51,16 +53,16 @@
 
 
 def configure_logger(
     level: LevelType = "DEBUG",
     sink=sys.stderr,
     format=SHORTEST_FORMAT,  # noqa # pylint: disable=redefined-builtin
     colorize=True,
-    add_sinks: list[any] | list[dict[str, any]] | None = None,
-    kwargs_handler: dict[str, any] | None = None,
+    add_sinks: Union[list[any], list[dict[str, any]], None] = None,
+    kwargs_handler: Union[dict[str, any], None] = None,
     **kwargs: any,
 ) -> dict[str, any]:
     """
     Configure the loguru logger. For more complex usages, use logger.configure() directly.
 
     Args:
         level: minimum level to log
@@ -165,15 +167,15 @@
 def get_level_as_int(level: LevelType):
     if isinstance(level, int):
         return level
     level_int = int(getLevelName(level.upper()))
     return level_int
 
 
-def get_logger_level_from_args(args) -> str:
+def get_logger_level_from_args(args: VerboseQuietArgs) -> str:
     if args.verbose:
         return "DEBUG"
     if args.quiet:
         return "WARNING"
     return "INFO"
```

### Comparing `packg-0.9.2/src/packg/magic.py` & `packg-0.9.3/src/packg/magic.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/maths.py` & `packg-0.9.3/src/packg/maths.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/misc.py` & `packg-0.9.3/src/packg/misc.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/multiproc/multiproc_fn.py` & `packg-0.9.3/src/packg/multiproc/multiproc_fn.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/multiproc/multiproc_producer_consumer.py` & `packg-0.9.3/src/packg/multiproc/multiproc_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/packaging.py` & `packg-0.9.3/src/packg/packaging.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/paths.py` & `packg-0.9.3/src/packg/paths.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/run/cleanup.py` & `packg-0.9.3/src/packg/run/cleanup.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/run/create_autocomplete.py` & `packg-0.9.3/src/packg/run/create_autocomplete.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/stats.py` & `packg-0.9.3/src/packg/stats.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/strings/abbreviations.py` & `packg-0.9.3/src/packg/strings/abbreviations.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/strings/base64tools.py` & `packg-0.9.3/src/packg/strings/base64tools.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/strings/hasher.py` & `packg-0.9.3/src/packg/strings/hasher.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/strings/quote_urlparse.py` & `packg-0.9.3/src/packg/strings/quote_urlparse.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/system/systemcall.py` & `packg-0.9.3/src/packg/system/systemcall.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/testing/fixture_webserver.py` & `packg-0.9.3/src/packg/testing/fixture_webserver.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/testing/import_from_source.py` & `packg-0.9.3/src/packg/testing/import_from_source.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/testing/setup_tests.py` & `packg-0.9.3/src/packg/testing/setup_tests.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/tqdmext.py` & `packg-0.9.3/src/packg/tqdmext.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/typext.py` & `packg-0.9.3/src/packg/typext.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg/web.py` & `packg-0.9.3/src/packg/web.py`

 * *Files identical despite different names*

### Comparing `packg-0.9.2/src/packg.egg-info/PKG-INFO` & `packg-0.9.3/src/packg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.9.2
+Version: 0.9.3
 Summary: Collection of utilities used in other python projects.
 Author: simonging
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/simonging/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.9.2 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.9.3 Summary: Collection of
 utilities used in other python projects. Author: simonging License: Apache-2.0
 Project-URL: Project-URL, https://github.com/simonging/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.9.2/src/packg.egg-info/SOURCES.txt` & `packg-0.9.3/src/packg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

