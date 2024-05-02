# Comparing `tmp/mat3ra-utils-2024.4.6.post0.tar.gz` & `tmp/mat3ra_utils-2024.5.2.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra-utils-2024.4.6.post0.tar", last modified: Sat Apr  6 02:16:48 2024, max compression
+gzip compressed data, was "mat3ra_utils-2024.5.2.post0.tar", last modified: Thu May  2 03:14:23 2024, max compression
```

## Comparing `mat3ra-utils-2024.4.6.post0.tar` & `mat3ra_utils-2024.5.2.post0.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.010671 mat3ra-utils-2024.4.6.post0/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.eslintignore
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.eslintrc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:47.990671 mat3ra-utils-2024.4.6.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:47.998671 mat3ra-utils-2024.4.6.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:47.998671 mat3ra-utils-2024.4.6.post0/.husky/
--rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.nycrc
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-06 02:16:48.010671 mat3ra-utils-2024.4.6.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   314260 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:16:48.010671 mat3ra-utils-2024.4.6.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:47.994670 mat3ra-utils-2024.4.6.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:47.998671 mat3ra-utils-2024.4.6.post0/src/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:47.994670 mat3ra-utils-2024.4.6.post0/src/js/browser/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:47.998671 mat3ra-utils-2024.4.6.post0/src/js/browser/specific/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/browser/specific/codemirror.ts
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/index_browser.ts
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/index_server.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:47.998671 mat3ra-utils-2024.4.6.post0/src/js/server/
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/server/file.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.002671 mat3ra-utils-2024.4.6.post0/src/js/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/array.js
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/class.js
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/clone.js
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/constants.js
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/hash.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/math.ts
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/object.ts
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.002671 mat3ra-utils-2024.4.6.post0/src/js/shared/specific/
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/specific/filter.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/specific/github.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/specific/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/specific/timestampable.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/str.js
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/tree.js
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/url.js
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/js/shared/uuid.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.002671 mat3ra-utils-2024.4.6.post0/src/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.002671 mat3ra-utils-2024.4.6.post0/src/py/mat3ra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.002671 mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.010671 mat3ra-utils-2024.4.6.post0/src/py/mat3ra_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-06 02:16:47.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-06 02:16:47.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:16:47.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-06 02:16:47.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 02:16:47.000000 mat3ra-utils-2024.4.6.post0/src/py/mat3ra_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:47.994670 mat3ra-utils-2024.4.6.post0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.006671 mat3ra-utils-2024.4.6.post0/tests/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/js/class.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/js/clone.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/js/file.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/js/filter.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/js/object.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/js/str.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/js/tree.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/js/url.tests.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:47.994670 mat3ra-utils-2024.4.6.post0/tests/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.006671 mat3ra-utils-2024.4.6.post0/tests/py/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.006671 mat3ra-utils-2024.4.6.post0/tests/py/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:48.010671 mat3ra-utils-2024.4.6.post0/tests/py/unit/fixtures/factory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/fixtures/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/fixtures/factory/factory_object_1.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/fixtures/factory/factory_object_2.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/fixtures/file_with_content.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/test_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tests/py/unit/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tsconfig-transpile.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-06 02:16:31.000000 mat3ra-utils-2024.4.6.post0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.eslintrc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.165434 mat3ra_utils-2024.5.2.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.169433 mat3ra_utils-2024.5.2.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.169433 mat3ra_utils-2024.5.2.post0/.husky/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.nycrc
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   314260 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.165434 mat3ra_utils-2024.5.2.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.169433 mat3ra_utils-2024.5.2.post0/src/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.165434 mat3ra_utils-2024.5.2.post0/src/js/browser/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.169433 mat3ra_utils-2024.5.2.post0/src/js/browser/specific/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/browser/specific/codemirror.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/index_browser.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/index_server.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.169433 mat3ra_utils-2024.5.2.post0/src/js/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/server/file.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.173433 mat3ra_utils-2024.5.2.post0/src/js/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/array.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/class.js
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/clone.js
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/constants.js
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/hash.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/math.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/object.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/selector.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.173433 mat3ra_utils-2024.5.2.post0/src/js/shared/specific/
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/specific/filter.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/specific/github.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/specific/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/specific/timestampable.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/str.js
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/tree.js
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/url.js
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/js/shared/uuid.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.173433 mat3ra_utils-2024.5.2.post0/src/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.173433 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.177433 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-02 03:14:23.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-02 03:14:23.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:14:23.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 03:14:23.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 03:14:23.000000 mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.165434 mat3ra_utils-2024.5.2.post0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.177433 mat3ra_utils-2024.5.2.post0/tests/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/class.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/clone.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/file.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/filter.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/object.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/str.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/tree.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/js/url.tests.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.165434 mat3ra_utils-2024.5.2.post0/tests/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/tests/py/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:23.181433 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/factory/factory_object_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/factory/factory_object_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/fixtures/file_with_content.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tests/py/unit/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tsconfig-transpile.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 03:14:03.000000 mat3ra_utils-2024.5.2.post0/tsconfig.json
```

### Comparing `mat3ra-utils-2024.4.6.post0/.github/workflows/cicd.yml` & `mat3ra_utils-2024.5.2.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/.gitignore` & `mat3ra_utils-2024.5.2.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/LICENSE.md` & `mat3ra_utils-2024.5.2.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/PKG-INFO` & `mat3ra_utils-2024.5.2.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-utils
-Version: 2024.4.6.post0
+Version: 2024.5.2.post0
 Summary: Utils.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2024 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `mat3ra-utils-2024.4.6.post0/package-lock.json` & `mat3ra_utils-2024.5.2.post0/package-lock.json`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/package.json` & `mat3ra_utils-2024.5.2.post0/package.json`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/pyproject.toml` & `mat3ra_utils-2024.5.2.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/index.ts` & `mat3ra_utils-2024.5.2.post0/src/js/index.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/server/file.js` & `mat3ra_utils-2024.5.2.post0/src/js/server/file.js`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/array.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/array.js`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/class.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/class.js`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/constants.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/constants.js`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/hash.ts` & `mat3ra_utils-2024.5.2.post0/src/js/shared/hash.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/math.ts` & `mat3ra_utils-2024.5.2.post0/src/js/shared/math.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/object.ts` & `mat3ra_utils-2024.5.2.post0/src/js/shared/object.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/selector.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/selector.js`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/specific/filter.ts` & `mat3ra_utils-2024.5.2.post0/src/js/shared/specific/filter.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/specific/github.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/specific/github.js`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/str.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/str.js`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/js/shared/tree.js` & `mat3ra_utils-2024.5.2.post0/src/js/shared/tree.js`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/factory.py` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/factory.py`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/object.py` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/object.py`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/regex.py` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/regex.py`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/py/mat3ra/utils/string.py` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra/utils/string.py`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/src/py/mat3ra_utils.egg-info/PKG-INFO` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-utils
-Version: 2024.4.6.post0
+Version: 2024.5.2.post0
 Summary: Utils.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2024 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `mat3ra-utils-2024.4.6.post0/src/py/mat3ra_utils.egg-info/SOURCES.txt` & `mat3ra_utils-2024.5.2.post0/src/py/mat3ra_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 src/js/shared/specific/filter.ts
 src/js/shared/specific/github.js
 src/js/shared/specific/index.ts
 src/js/shared/specific/timestampable.ts
 src/py/__init__.py
 src/py/mat3ra/__init__.py
 src/py/mat3ra/utils/__init__.py
+src/py/mat3ra/utils/array.py
 src/py/mat3ra/utils/factory.py
 src/py/mat3ra/utils/file.py
 src/py/mat3ra/utils/mixins.py
 src/py/mat3ra/utils/object.py
 src/py/mat3ra/utils/regex.py
 src/py/mat3ra/utils/string.py
 src/py/mat3ra_utils.egg-info/PKG-INFO
@@ -56,14 +57,15 @@
 tests/js/file.tests.ts
 tests/js/filter.tests.ts
 tests/js/object.tests.ts
 tests/js/str.tests.ts
 tests/js/tree.tests.ts
 tests/js/url.tests.ts
 tests/py/unit/__init__.py
+tests/py/unit/test_array.py
 tests/py/unit/test_factory.py
 tests/py/unit/test_file.py
 tests/py/unit/test_mixins.py
 tests/py/unit/test_object.py
 tests/py/unit/test_string.py
 tests/py/unit/fixtures/__init__.py
 tests/py/unit/fixtures/file_with_content.txt
```

### Comparing `mat3ra-utils-2024.4.6.post0/tests/js/class.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/class.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/tests/js/clone.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/clone.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/tests/js/filter.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/filter.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/tests/js/object.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/object.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/tests/js/str.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/str.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/tests/js/tree.tests.ts` & `mat3ra_utils-2024.5.2.post0/tests/js/tree.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/tests/py/unit/test_mixins.py` & `mat3ra_utils-2024.5.2.post0/tests/py/unit/test_mixins.py`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/tests/py/unit/test_object.py` & `mat3ra_utils-2024.5.2.post0/tests/py/unit/test_object.py`

 * *Files identical despite different names*

### Comparing `mat3ra-utils-2024.4.6.post0/tests/py/unit/test_string.py` & `mat3ra_utils-2024.5.2.post0/tests/py/unit/test_string.py`

 * *Files identical despite different names*

