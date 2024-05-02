# Comparing `tmp/authx-1.1.1.tar.gz` & `tmp/authx-1.1.2.tar.gz`

## Comparing `authx-1.1.1.tar` & `authx-1.1.2.tar`

### file list

```diff
@@ -1,114 +1,115 @@
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 authx-1.1.1/.all-contributorsrc
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 authx-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 authx-1.1.1/mkdocs.yml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 authx-1.1.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 authx-1.1.1/.github/SECURITY.md
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 authx-1.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 authx-1.1.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 authx-1.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 authx-1.1.1/authx/__init__.py
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 authx-1.1.1/authx/config.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 authx-1.1.1/authx/core.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 authx-1.1.1/authx/dependencies.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 authx-1.1.1/authx/exceptions.py
--rw-r--r--   0        0        0    25599 2020-02-02 00:00:00.000000 authx-1.1.1/authx/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.1/authx/py.typed
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 authx-1.1.1/authx/schema.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 authx-1.1.1/authx/token.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 authx-1.1.1/authx/types.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 authx-1.1.1/authx/_internal/__init__.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 authx-1.1.1/authx/_internal/_callback.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 authx-1.1.1/authx/_internal/_error.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 authx-1.1.1/authx/_internal/_logger.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 authx-1.1.1/authx/_internal/_memory.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 authx-1.1.1/authx/_internal/_signature.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 authx-1.1.1/authx/_internal/_utils.py
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 authx-1.1.1/docs/index.md
--rw-r--r--   0        0        0    50523 2020-02-02 00:00:00.000000 authx-1.1.1/docs/release.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/config.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/dependencies.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/exceptions.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/main.md
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/reference.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/request.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/token.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/extra/cache.md
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/extra/metrics.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/extra/oauth2.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/extra/profiler.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/extra/session.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/internal/callback.md
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/internal/errors.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/internal/memory.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 authx-1.1.1/docs/api/internal/signature.md
--rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 authx-1.1.1/docs/callbacks/token.md
--rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 authx-1.1.1/docs/callbacks/user.md
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 authx-1.1.1/docs/css/custom.css
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 authx-1.1.1/docs/css/termynal.css
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 authx-1.1.1/docs/dependencies/aliases.md
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 authx-1.1.1/docs/dependencies/bundle.md
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 authx-1.1.1/docs/dependencies/dependencies.md
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 authx-1.1.1/docs/dependencies/injection.md
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 authx-1.1.1/docs/development/contributing.md
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 authx-1.1.1/docs/extra/Cache.md
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 authx-1.1.1/docs/extra/Metrics.md
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 authx-1.1.1/docs/extra/OAuth2.md
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 authx-1.1.1/docs/extra/Sessions.md
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 authx-1.1.1/docs/extra/profiler.md
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 authx-1.1.1/docs/faq/code_of_conduct.md
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 authx-1.1.1/docs/faq/faq.md
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 authx-1.1.1/docs/faq/help.md
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 authx-1.1.1/docs/faq/license.md
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 authx-1.1.1/docs/get-started/basic-usage.md
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 authx-1.1.1/docs/get-started/installation.md
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 authx-1.1.1/docs/get-started/location.md
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 authx-1.1.1/docs/get-started/payload.md
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 authx-1.1.1/docs/get-started/refresh.md
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 authx-1.1.1/docs/get-started/token.md
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 authx-1.1.1/docs/img/header.svg
--rw-r--r--   0        0        0   335246 2020-02-02 00:00:00.000000 authx-1.1.1/docs/img/icon.ico
--rw-r--r--   0        0        0   112430 2020-02-02 00:00:00.000000 authx-1.1.1/docs/img/logo.png
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 authx-1.1.1/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 authx-1.1.1/docs/js/termynal.js
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 authx-1.1.1/requirements/all.txt
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.1.1/requirements/docs.in
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 authx-1.1.1/requirements/docs.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authx-1.1.1/requirements/linting.in
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 authx-1.1.1/requirements/linting.txt
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 authx-1.1.1/requirements/pyproject.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 authx-1.1.1/requirements/testing.in
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 authx-1.1.1/requirements/testing.txt
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 authx-1.1.1/scripts/clean.sh
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 authx-1.1.1/scripts/docs_build.sh
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 authx-1.1.1/scripts/docs_serve.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx-1.1.1/scripts/format.sh
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 authx-1.1.1/scripts/mypy.sh
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 authx-1.1.1/scripts/requirements.sh
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 authx-1.1.1/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 authx-1.1.1/tests/test_authx.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 authx-1.1.1/tests/test_callback.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 authx-1.1.1/tests/test_config.py
--rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 authx-1.1.1/tests/test_core.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 authx-1.1.1/tests/test_dependencies.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 authx-1.1.1/tests/test_errors.py
--rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 authx-1.1.1/tests/test_schema.py
--rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 authx-1.1.1/tests/test_token.py
--rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 authx-1.1.1/tests/utils.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 authx-1.1.1/tests/app/conftest.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 authx-1.1.1/tests/app/test_access_location.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 authx-1.1.1/tests/app/test_blocklist_token.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 authx-1.1.1/tests/app/test_fresh_token.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 authx-1.1.1/tests/app/test_get_subject.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 authx-1.1.1/tests/app/test_token_protected_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.1/tests/internal/__init__.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 authx-1.1.1/tests/internal/test_logger.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 authx-1.1.1/tests/internal/test_memory.py
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 authx-1.1.1/tests/internal/test_signature.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 authx-1.1.1/tests/internal/test_utils.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 authx-1.1.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx-1.1.1/LICENSE
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 authx-1.1.1/README.md
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 authx-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 authx-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 authx-1.1.2/.all-contributorsrc
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 authx-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 authx-1.1.2/mkdocs.yml
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 authx-1.1.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 authx-1.1.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 authx-1.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 authx-1.1.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 authx-1.1.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 authx-1.1.2/authx/__init__.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 authx-1.1.2/authx/config.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 authx-1.1.2/authx/core.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 authx-1.1.2/authx/dependencies.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 authx-1.1.2/authx/exceptions.py
+-rw-r--r--   0        0        0    25599 2020-02-02 00:00:00.000000 authx-1.1.2/authx/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.2/authx/py.typed
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 authx-1.1.2/authx/schema.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 authx-1.1.2/authx/token.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 authx-1.1.2/authx/types.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/__init__.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_callback.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_error.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_logger.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_memory.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_signature.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_utils.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 authx-1.1.2/docs/index.md
+-rw-r--r--   0        0        0    51615 2020-02-02 00:00:00.000000 authx-1.1.2/docs/release.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/config.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/dependencies.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/exceptions.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/main.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/reference.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/request.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/token.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/extra/cache.md
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/extra/metrics.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/extra/oauth2.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/extra/profiler.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/extra/session.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/internal/callback.md
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/internal/errors.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/internal/memory.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/internal/signature.md
+-rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 authx-1.1.2/docs/callbacks/token.md
+-rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 authx-1.1.2/docs/callbacks/user.md
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 authx-1.1.2/docs/css/custom.css
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 authx-1.1.2/docs/css/termynal.css
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 authx-1.1.2/docs/dependencies/aliases.md
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 authx-1.1.2/docs/dependencies/bundle.md
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 authx-1.1.2/docs/dependencies/dependencies.md
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 authx-1.1.2/docs/dependencies/injection.md
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 authx-1.1.2/docs/development/contributing.md
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 authx-1.1.2/docs/extra/Cache.md
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 authx-1.1.2/docs/extra/Metrics.md
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 authx-1.1.2/docs/extra/OAuth2.md
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 authx-1.1.2/docs/extra/Sessions.md
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 authx-1.1.2/docs/extra/profiler.md
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 authx-1.1.2/docs/faq/code_of_conduct.md
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 authx-1.1.2/docs/faq/faq.md
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 authx-1.1.2/docs/faq/help.md
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 authx-1.1.2/docs/faq/license.md
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/basic-usage.md
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/installation.md
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/location.md
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/payload.md
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/refresh.md
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/token.md
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 authx-1.1.2/docs/img/header.svg
+-rw-r--r--   0        0        0   335246 2020-02-02 00:00:00.000000 authx-1.1.2/docs/img/icon.ico
+-rw-r--r--   0        0        0   112430 2020-02-02 00:00:00.000000 authx-1.1.2/docs/img/logo.png
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 authx-1.1.2/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 authx-1.1.2/docs/js/termynal.js
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/all.txt
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/docs.in
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/docs.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/linting.in
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/linting.txt
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/pyproject.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/testing.in
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/testing.txt
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/clean.sh
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/docs_build.sh
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/docs_serve.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/format.sh
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/mypy.sh
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/requirements.sh
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/test.sh
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/test_extra.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_authx.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_callback.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_config.py
+-rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_core.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_dependencies.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_errors.py
+-rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_schema.py
+-rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_token.py
+-rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 authx-1.1.2/tests/utils.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/conftest.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/test_access_location.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/test_blocklist_token.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/test_fresh_token.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/test_get_subject.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/test_token_protected_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.2/tests/internal/__init__.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 authx-1.1.2/tests/internal/test_logger.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 authx-1.1.2/tests/internal/test_memory.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 authx-1.1.2/tests/internal/test_signature.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 authx-1.1.2/tests/internal/test_utils.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 authx-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx-1.1.2/LICENSE
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 authx-1.1.2/README.md
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 authx-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    12133 2020-02-02 00:00:00.000000 authx-1.1.2/PKG-INFO
```

### Comparing `authx-1.1.1/.all-contributorsrc` & `authx-1.1.2/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/mkdocs.yml` & `authx-1.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/.github/workflows/ci.yml` & `authx-1.1.2/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -3,40 +3,14 @@
 on:
   push:
     branches:
       - main
   pull_request: {}
 
 jobs:
-  lint:
-    runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python-version: ["3.11"]
-      fail-fast: false
-
-    steps:
-      - uses: actions/checkout@v4
-      - name: Set up Python
-        uses: actions/setup-python@v5
-        with:
-          python-version: ${{ matrix.python-version }}
-
-      - name: setup uv
-        uses: yezz123/setup-uv@v4
-        with:
-          uv-version: "0.1.17"
-          uv-venv: ".venv"
-
-      - name: Install Dependencies
-        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/linting.txt
-
-      - name: Run Pre-commit
-        run: bash scripts/format.sh
-
   tests:
 
     name: test py${{ matrix.python-version }} on ${{ matrix.os }}
 
     runs-on: ${{ matrix.os }}-latest
 
 
@@ -55,15 +29,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: setup UV
         uses: yezz123/setup-uv@v4
         with:
-          uv-version: "0.1.17"
+          uv-version: "0.1.39"
           uv-venv: ".venv"
 
       - name: Install Dependencies
         run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/testing.txt
 
       - name: Freeze Dependencies
         run: uv pip freeze
@@ -75,17 +49,62 @@
 
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v4
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           file: ./coverage.xml
 
+  test-extra:
+
+    name: test py${{ matrix.python-version }} on ${{ matrix.os }} with extra
+
+    runs-on: ${{ matrix.os }}-latest
+
+    services:
+      redis:
+        image: redis
+        ports:
+          - 6379:6379
+        options: >-
+          --health-cmd "redis-cli ping"
+          --health-interval 10s
+          --health-timeout 5s
+          --health-retries 5
+
+    strategy:
+
+      matrix:
+
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+
+        os: [ubuntu]
+
+    steps:
+      - uses: actions/checkout@v4
+
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Clone authx extra
+        run: git clone https://github.com/yezz123/authx-extra.git --single-branch
+
+      - name: Update pip
+        run: python -m pip install --upgrade pip
+
+      - name: Test Suite - ${{ matrix.os }} - py${{ matrix.python-version }}
+        run: bash scripts/test_extra.sh
+        env:
+          ENV: test
+          REDIS_URL: "redis://0.0.0.0:6379"
+
   # https://github.com/marketplace/actions/alls-green#why used for branch protection checks
   check:
     if: always()
-    needs: [lint, tests]
+    needs: [tests, test-extra]
     runs-on: ubuntu-latest
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
           jobs: ${{ toJSON(needs) }}
```

### Comparing `authx-1.1.1/.github/workflows/latest-changes.yml` & `authx-1.1.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/.github/workflows/release.yml` & `authx-1.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/config.py` & `authx-1.1.2/authx/config.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/core.py` & `authx-1.1.2/authx/core.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/dependencies.py` & `authx-1.1.2/authx/dependencies.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/exceptions.py` & `authx-1.1.2/authx/exceptions.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/main.py` & `authx-1.1.2/authx/main.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/schema.py` & `authx-1.1.2/authx/schema.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/token.py` & `authx-1.1.2/authx/token.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/types.py` & `authx-1.1.2/authx/types.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/_internal/__init__.py` & `authx-1.1.2/authx/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/_internal/_callback.py` & `authx-1.1.2/authx/_internal/_callback.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/_internal/_error.py` & `authx-1.1.2/authx/_internal/_error.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/_internal/_logger.py` & `authx-1.1.2/authx/_internal/_logger.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/_internal/_memory.py` & `authx-1.1.2/authx/_internal/_memory.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/_internal/_signature.py` & `authx-1.1.2/authx/_internal/_signature.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/authx/_internal/_utils.py` & `authx-1.1.2/authx/_internal/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 
 def IST_time() -> datetime:
     return datetime.now().astimezone(utc)
 
 
 def tz_now(tz: BaseTzInfo = utc) -> datetime:
-    dt = datetime.utcnow()
+    dt = datetime.now(tz=tz)
     return dt.replace(tzinfo=tz)
 
 
 def tz_from_iso(
     dt: str, to_tz: BaseTzInfo = utc, format: str = "%Y-%m-%dT%H:%M:%S.%f%z"
 ) -> datetime:
     date_time = datetime.strptime(dt, format)
```

### Comparing `authx-1.1.1/docs/index.md` & `authx-1.1.2/docs/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,26 +10,32 @@
 <p align="center">
     <em>Ready-to-use and customizable Authentications and Oauth2 management for FastAPI ⚡</em>
 </p>
 <p align="center">
 <a href="https://github.com/yezz123/authx/actions/workflows/ci.yml" target="_blank">
     <img src="https://github.com/yezz123/authx/actions/workflows/ci.yml/badge.svg" alt="lint">
 </a>
+<a href="https://results.pre-commit.ci/latest/github/yezz123/authx/main" target="_blank">
+    <img src="https://results.pre-commit.ci/badge/github/yezz123/authx/main.svg" alt="pre-commit.ci status">
+</a>
 <a href="https://pypi.org/project/authx" target="_blank">
     <img src="https://img.shields.io/pypi/v/authx?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://codecov.io/gh/yezz123/authx">
     <img src="https://codecov.io/gh/yezz123/authx/branch/main/graph/badge.svg"/>
 </a>
 <a href="https://pepy.tech/project/authx" target="_blank">
     <img src="https://static.pepy.tech/badge/authx" alt="Total Downloads">
 </a>
 <a href="https://pydantic.dev" target="_blank">
     <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json" alt="Pydantic Version 2">
 </a>
+<a href="https://github.com/astral-sh/ruff" target="_blank">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" alt="Ruff">
+</a>
 </p>
 </p>
 
 ---
 
 **Source Code**: <https://github.com/yezz123/authx>
```

### Comparing `authx-1.1.1/docs/release.md` & `authx-1.1.2/docs/release.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,32 @@
   - navigation
 ---
 
 # Release Notes
 
 ## Latest Changes
 
+## 1.1.2
+
+### Docs
+
+* 📝 Update badges and links in README. PR [#583](https://github.com/yezz123/authx/pull/583) by [@yezz123](https://github.com/yezz123).
+* 📝  Refactor route decorators to use `@app.get` instead of `@app.route`. PR [#576](https://github.com/yezz123/authx/pull/576) by [@yezz123](https://github.com/yezz123).
+
+### Internal
+
+* 🔧 remove linting step from CI. PR [#578](https://github.com/yezz123/authx/pull/578) by [@yezz123](https://github.com/yezz123).
+* :recycle: refactor `datetime` function. PR [#580](https://github.com/yezz123/authx/pull/580) by [@yezz123](https://github.com/yezz123).
+* 👷 Add extra job to run additional tests with Redis service. PR [#581](https://github.com/yezz123/authx/pull/581) by [@yezz123](https://github.com/yezz123).
+
+### Dependencies
+
+* ⬆️ Update `uv` version in CI. PR [#582](https://github.com/yezz123/authx/pull/582) by [@pinchXOXO](https://github.com/pinchXOXO).
+* [pre-commit.ci] pre-commit autoupdate. PR [#579](https://github.com/yezz123/authx/pull/579) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
+
 ## 1.1.1
 
 ### Internal
 
 * ✅ Fix skipped tests & Add coverage pragmas. PR [#571](https://github.com/yezz123/authx/pull/571) by [@yezz123](https://github.com/yezz123).
 * 🔧 drop The action `hynek/build-and-inspect-python-package`. PR [#570](https://github.com/yezz123/authx/pull/570) by [@yezz123](https://github.com/yezz123).
```

### Comparing `authx-1.1.1/docs/api/exceptions.md` & `authx-1.1.2/docs/api/exceptions.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/callbacks/token.md` & `authx-1.1.2/docs/callbacks/token.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/callbacks/user.md` & `authx-1.1.2/docs/callbacks/user.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/css/termynal.css` & `authx-1.1.2/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/dependencies/aliases.md` & `authx-1.1.2/docs/dependencies/aliases.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,30 +12,30 @@
     from fastapi import FastAPI, Depends
     from authx import AuthX
 
     app = FastAPI()
     security = AuthX()
     security.handle_errors(app)
 
-    @app.route('/', dependencies=[Depends(security.access_token_required)])
+    @app.get('/', dependencies=[Depends(security.access_token_required)])
     def root(subject = Depends(security.get_current_subject), token = Depends(security.get_token_from_request)):
         ...
     ```
 
 === "With aliases"
 
     ```py
     from fastapi import FastAPI
     from authx import AuthX
 
     app = FastAPI()
     security = AuthX()
     security.handle_errors(app)
 
-    @app.route('/', dependencies=[security.ACCESS_REQUIRED])
+    @app.get('/', dependencies=[security.ACCESS_REQUIRED])
     def root(subject = security.CURRENT_SUBJECT, token = security.RAW_ACCESS_TOKEN):
         ...
     ```
 
 ## Aliases
 
 ### `ACCESS_REQUIRED`
@@ -49,15 +49,15 @@
 ```py
 from fastapi import FastAPI
 from authx import AuthX
 
 app = FastAPI()
 security = AuthX()
 
-@app.route('/protected')
+@app.get('/protected')
 def protected(payload = security.ACCESS_REQUIRED):
     return f"Your Access Token Payload is {payload}"
 ```
 
 ### `ACCESS_TOKEN`
 
 - [`RequestToken`](../api/request.md)
@@ -70,15 +70,15 @@
 from fastapi import FastAPI
 from authx import AuthX
 
 app = FastAPI()
 security = AuthX()
 
 # Use route dependency to enforce validation in conjunction with ACCESS_TOKEN
-@app.route('/protected', dependencies=[security.ACCESS_REQUIRED])
+@app.get('/protected', dependencies=[security.ACCESS_REQUIRED])
 def protected(token = security.ACCESS_TOKEN):
     return f"Your Access Token is {token}"
 ```
 
 ### `REFRESH_REQUIRED`
 
 - [`TokenPayload`](../api/token.md)
@@ -90,15 +90,15 @@
 ```py
 from fastapi import FastAPI
 from authx import AuthX
 
 app = FastAPI()
 security = AuthX()
 
-@app.route('/refresh')
+@app.get('/refresh')
 def refresh(payload = security.REFRESH_REQUIRED):
     return f"Your Refresh Token Payload is {payload}"
 ```
 
 ### `REFRESH_TOKEN`
 
 - [`RequestToken`](../api/request.md)
@@ -111,15 +111,15 @@
 from fastapi import FastAPI
 from authx import AuthX
 
 app = FastAPI()
 security = AuthX()
 
 # Use route dependency to enforce validation in conjunction with REFRESH_TOKEN
-@app.route('/refresh', dependencies=[security.REFRESH_REQUIRED])
+@app.get('/refresh', dependencies=[security.REFRESH_REQUIRED])
 def refresh(token = security.REFRESH_TOKEN):
     return f"Your Refresh Token is {token}"
 ```
 
 ### `FRESH_REQUIRED`
 
 - [`TokenPayload`](../api/token.md)
@@ -131,15 +131,15 @@
 ```py
 from fastapi import FastAPI
 from authx import AuthX
 
 app = FastAPI()
 security = AuthX()
 
-@app.route('/protected', dependencies=[security.FRESH_REQUIRED])
+@app.get('/protected', dependencies=[security.FRESH_REQUIRED])
 def protected():
     return "Congratulations! Your have a fresh and valid access token."
 ```
 
 ### `CURRENT_SUBJECT`
 
 - `Any`
@@ -154,15 +154,15 @@
 ```py
 from fastapi import FastAPI
 from authx import AuthX
 
 app = FastAPI()
 security = AuthX()
 
-@app.route('/whoami')
+@app.get('/whoami')
 def whoami(subject = security.CURRENT_SUBJECT):
     return f"You are: {subject}"
 ```
 
 ### `BUNDLE` / `DEPENDENCY`
 
 - [`AuthXDependency`](../api/dependencies.md)
@@ -174,13 +174,13 @@
 ```py
 from fastapi import FastAPI
 from authx import AuthX
 
 app = FastAPI()
 security = AuthX()
 
-@app.route('/create_token')
+@app.get('/create_token')
 def create_token(auth = security.BUNDLE):
     token = auth.create_access_token(uid="test")
     auth.set_access_cookie(token)
     return "OK"
 ```
```

### Comparing `authx-1.1.1/docs/dependencies/bundle.md` & `authx-1.1.2/docs/dependencies/bundle.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/dependencies/dependencies.md` & `authx-1.1.2/docs/dependencies/dependencies.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/dependencies/injection.md` & `authx-1.1.2/docs/dependencies/injection.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/development/contributing.md` & `authx-1.1.2/docs/development/contributing.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/extra/Cache.md` & `authx-1.1.2/docs/extra/Cache.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/extra/Metrics.md` & `authx-1.1.2/docs/extra/Metrics.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/extra/OAuth2.md` & `authx-1.1.2/docs/extra/OAuth2.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/extra/Sessions.md` & `authx-1.1.2/docs/extra/Sessions.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/extra/profiler.md` & `authx-1.1.2/docs/extra/profiler.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/faq/code_of_conduct.md` & `authx-1.1.2/docs/faq/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/faq/faq.md` & `authx-1.1.2/docs/faq/faq.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/faq/help.md` & `authx-1.1.2/docs/faq/help.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/faq/license.md` & `authx-1.1.2/docs/faq/license.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/get-started/basic-usage.md` & `authx-1.1.2/docs/get-started/basic-usage.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/get-started/installation.md` & `authx-1.1.2/docs/get-started/installation.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/get-started/location.md` & `authx-1.1.2/docs/get-started/location.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/get-started/payload.md` & `authx-1.1.2/docs/get-started/payload.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/get-started/refresh.md` & `authx-1.1.2/docs/get-started/refresh.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/get-started/token.md` & `authx-1.1.2/docs/get-started/token.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/img/header.svg` & `authx-1.1.2/docs/img/header.svg`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/img/icon.ico` & `authx-1.1.2/docs/img/icon.ico`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/img/logo.png` & `authx-1.1.2/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/js/custom.js` & `authx-1.1.2/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/docs/js/termynal.js` & `authx-1.1.2/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/requirements/docs.txt` & `authx-1.1.2/requirements/docs.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,64 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile requirements/docs.in -o requirements/docs.txt
+annotated-types==0.6.0
+    # via pydantic
 anyio==4.3.0
-    # via httpx
+    # via
+    #   httpx
+    #   starlette
 async-timeout==4.0.3
     # via redis
-authx-extra @ git+https://github.com/yezz123/authx-extra.git@aac2f826b330ce2569659c961d682e5c2f0693a1
+authx==1.1.1
+    # via authx-extra
+authx-extra @ git+https://github.com/yezz123/authx-extra.git@9364049513e122f511e43a7bbd8ba0702b8d9fb8
 babel==2.14.0
     # via mkdocs-material
 beautifulsoup4==4.12.3
     # via mkdocs-mermaid2-plugin
-cairocffi==1.6.1
+cairocffi==1.7.0
     # via cairosvg
 cairosvg==2.7.1
 certifi==2024.2.2
     # via
     #   httpcore
     #   httpx
     #   requests
 cffi==1.16.0
-    # via cairocffi
+    # via
+    #   cairocffi
+    #   cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   mkdocs
     #   mkdocstrings
     #   typer
 colorama==0.4.6
     # via
     #   griffe
     #   mkdocs-material
+cryptography==42.0.5
+    # via pyjwt
 cssselect2==0.7.0
     # via cairosvg
 cyclic==1.0.0
     # via mdx-include
 defusedxml==0.7.1
     # via cairosvg
+ecdsa==0.19.0
+    # via python-jose
 editorconfig==0.12.4
     # via jsbeautifier
+fastapi==0.110.3
+    # via authx
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.42.1
+griffe==0.44.0
     # via
     #   griffe-typingdoc
     #   mkdocstrings-python
 griffe-typingdoc==0.2.5
 h11==0.14.0
     # via httpcore
 httpcore==1.0.5
@@ -80,106 +94,142 @@
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocstrings
 mdurl==0.1.2
     # via markdown-it-py
 mdx-include==1.4.2
 mergedeep==1.3.4
-    # via mkdocs
-mkdocs==1.5.3
+    # via
+    #   mkdocs
+    #   mkdocs-get-deps
+mkdocs==1.6.0
     # via
     #   mkdocs-autorefs
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-mermaid2-plugin
     #   mkdocstrings
 mkdocs-autorefs==1.0.1
     # via mkdocstrings
+mkdocs-get-deps==0.2.0
+    # via mkdocs
 mkdocs-markdownextradata-plugin==0.2.5
-mkdocs-material==9.5.17
+mkdocs-material==9.5.20
 mkdocs-material-extensions==1.3.1
     # via mkdocs-material
 mkdocs-mermaid2-plugin==1.1.1
-mkdocstrings==0.24.3
+mkdocstrings==0.25.0
     # via mkdocstrings-python
-mkdocstrings-python==1.9.2
+mkdocstrings-python==1.10.0
     # via mkdocstrings
 packaging==24.0
     # via mkdocs
 paginate==0.5.6
     # via mkdocs-material
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via cairosvg
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
-    #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocstrings
 prometheus-client==0.20.0
     # via authx-extra
+pyasn1==0.6.0
+    # via
+    #   python-jose
+    #   rsa
 pycparser==2.22
     # via cffi
+pydantic==2.7.1
+    # via
+    #   authx
+    #   fastapi
+    #   pydantic-settings
+pydantic-core==2.18.2
+    # via pydantic
+pydantic-settings==2.2.1
+    # via authx
 pygments==2.17.2
     # via
     #   mkdocs-material
     #   rich
 pyinstrument==4.6.2
     # via authx-extra
-pymdown-extensions==10.7.1
+pyjwt==2.8.0
+    # via authx
+pymdown-extensions==10.8.1
     # via
     #   mkdocs-material
     #   mkdocs-mermaid2-plugin
     #   mkdocstrings
 python-dateutil==2.9.0.post0
-    # via ghp-import
+    # via
+    #   authx
+    #   ghp-import
+python-dotenv==1.0.1
+    # via pydantic-settings
+python-jose==3.3.0
+    # via authx
+pytz==2024.1
+    # via authx
 pyyaml==6.0.1
     # via
     #   mkdocs
+    #   mkdocs-get-deps
     #   mkdocs-markdownextradata-plugin
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 rcslice==1.1.0
     # via mdx-include
-redis==5.0.3
+redis==5.0.4
     # via authx-extra
-regex==2023.12.25
+regex==2024.4.28
     # via mkdocs-material
 requests==2.31.0
     # via
     #   mkdocs-material
     #   mkdocs-mermaid2-plugin
 rich==13.7.1
     # via typer
+rsa==4.9
+    # via python-jose
 setuptools==69.5.1
     # via mkdocs-mermaid2-plugin
 shellingham==1.5.4
     # via typer
 six==1.16.0
     # via
+    #   ecdsa
     #   jsbeautifier
     #   python-dateutil
 sniffio==1.3.1
     # via
     #   anyio
     #   httpx
 soupsieve==2.5
     # via beautifulsoup4
-tinycss2==1.2.1
+starlette==0.37.2
+    # via fastapi
+tinycss2==1.3.0
     # via
     #   cairosvg
     #   cssselect2
 typer==0.12.3
     # via typer-cli
 typer-cli==0.12.3
 typing-extensions==4.11.0
     # via
+    #   fastapi
     #   griffe-typingdoc
+    #   pydantic
+    #   pydantic-core
     #   typer
 urllib3==2.2.1
     # via requests
 watchdog==4.0.0
     # via mkdocs
 webencodings==0.5.1
     # via
```

### Comparing `authx-1.1.1/requirements/linting.txt` & `authx-1.1.2/requirements/linting.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile requirements/linting.in -o requirements/linting.txt
-black==24.4.0
+black==24.4.2
 cfgv==3.4.0
     # via pre-commit
 click==8.1.7
     # via black
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.4
+filelock==3.14.0
     # via virtualenv
-identify==2.5.35
+identify==2.5.36
     # via pre-commit
-mypy==1.9.0
+mypy==1.10.0
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 nodeenv==1.8.0
     # via pre-commit
 packaging==24.0
     # via black
 pathspec==0.12.1
     # via black
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   black
     #   virtualenv
 pre-commit==3.7.0
 pyupgrade==3.15.2
 pyyaml==6.0.1
     # via pre-commit
-ruff==0.3.7
+ruff==0.4.2
 setuptools==69.5.1
     # via nodeenv
 tokenize-rt==5.2.0
     # via pyupgrade
 typing-extensions==4.11.0
     # via mypy
-virtualenv==20.25.1
+virtualenv==20.26.1
     # via pre-commit
```

### Comparing `authx-1.1.1/requirements/pyproject.txt` & `authx-1.1.2/requirements/pyproject.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
     # via starlette
 cffi==1.16.0
     # via cryptography
 cryptography==42.0.5
     # via pyjwt
 ecdsa==0.19.0
     # via python-jose
-fastapi==0.110.1
+fastapi==0.110.3
 idna==3.7
     # via anyio
 pyasn1==0.6.0
     # via
     #   python-jose
     #   rsa
 pycparser==2.22
     # via cffi
-pydantic==2.7.0
+pydantic==2.7.1
     # via
     #   fastapi
     #   pydantic-settings
-pydantic-core==2.18.1
+pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
 pyjwt==2.8.0
 python-dateutil==2.9.0.post0
 python-dotenv==1.0.1
     # via pydantic-settings
 python-jose==3.3.0
```

### Comparing `authx-1.1.1/requirements/testing.txt` & `authx-1.1.2/requirements/testing.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 certifi==2024.2.2
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.3.2
     # via requests
-coverage==7.4.4
+coverage==7.5.0
     # via pytest-cov
-freezegun==1.4.0
+freezegun==1.5.0
 h11==0.14.0
     # via httpcore
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
 idna==3.7
     # via
     #   anyio
     #   httpx
     #   requests
 iniconfig==2.0.0
     # via pytest
-itsdangerous==2.1.2
+itsdangerous==2.2.0
 packaging==24.0
     # via pytest
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   pytest-asyncio
     #   pytest-cov
 pytest-asyncio==0.23.6
 pytest-cov==5.0.0
 python-dateutil==2.9.0.post0
     # via freezegun
```

### Comparing `authx-1.1.1/scripts/clean.sh` & `authx-1.1.2/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/test_authx.py` & `authx-1.1.2/tests/test_authx.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/test_callback.py` & `authx-1.1.2/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/test_config.py` & `authx-1.1.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/test_core.py` & `authx-1.1.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/test_dependencies.py` & `authx-1.1.2/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/test_errors.py` & `authx-1.1.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/test_schema.py` & `authx-1.1.2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/test_token.py` & `authx-1.1.2/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/utils.py` & `authx-1.1.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/app/conftest.py` & `authx-1.1.2/tests/app/conftest.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/app/test_access_location.py` & `authx-1.1.2/tests/app/test_access_location.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/app/test_blocklist_token.py` & `authx-1.1.2/tests/app/test_blocklist_token.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/app/test_fresh_token.py` & `authx-1.1.2/tests/app/test_fresh_token.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/app/test_get_subject.py` & `authx-1.1.2/tests/app/test_get_subject.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/app/test_token_protected_access.py` & `authx-1.1.2/tests/app/test_token_protected_access.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/internal/test_logger.py` & `authx-1.1.2/tests/internal/test_logger.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/internal/test_memory.py` & `authx-1.1.2/tests/internal/test_memory.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/tests/internal/test_signature.py` & `authx-1.1.2/tests/internal/test_signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     dict_obj = {"session_id": 1}
     token = serializer.encode(dict_obj)
     time.sleep(2)
     data, err = serializer.decode(token)
     assert data is None and err == "SignatureExpired"
 
 
+@unittest.skip("Skipping test for now")
 def test_decode_with_invalid_signature():
     serializer = SignatureSerializer("MY_SECRET_KEY", expired_in=1)
     dict_obj = {"session_id": 1}
     token = serializer.encode(dict_obj)
     tampered_token = f"{token[:-1]}a"
     data, err = serializer.decode(tampered_token)
     assert data is None and err == "InvalidSignature"
```

### Comparing `authx-1.1.1/tests/internal/test_utils.py` & `authx-1.1.2/tests/internal/test_utils.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/.gitignore` & `authx-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/LICENSE` & `authx-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/README.md` & `authx-1.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,541 +14,636 @@
 000000d0: 2f61 3e0a 3c70 2061 6c69 676e 3d22 6365  /a>.<p align="ce
 000000e0: 6e74 6572 223e 0a20 2020 203c 656d 3e52  nter">.    <em>R
 000000f0: 6561 6479 2d74 6f2d 7573 6520 616e 6420  eady-to-use and 
 00000100: 6375 7374 6f6d 697a 6162 6c65 2041 7574  customizable Aut
 00000110: 6865 6e74 6963 6174 696f 6e73 2061 6e64  hentications and
 00000120: 204f 6175 7468 3220 6d61 6e61 6765 6d65   Oauth2 manageme
 00000130: 6e74 2066 6f72 2046 6173 7441 5049 20e2  nt for FastAPI .
-00000140: 9aa1 3c2f 656d 3e0a 3c2f 703e 0a3c 7020  ..</em>.</p>.<p 
-00000150: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000160: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000170: 2f67 6974 6875 622e 636f 6d2f 7965 7a7a  /github.com/yezz
-00000180: 3132 332f 6175 7468 782f 6163 7469 6f6e  123/authx/action
-00000190: 732f 776f 726b 666c 6f77 732f 6369 2e79  s/workflows/ci.y
-000001a0: 6d6c 2220 7461 7267 6574 3d22 5f62 6c61  ml" target="_bla
-000001b0: 6e6b 223e 0a20 2020 203c 696d 6720 7372  nk">.    <img sr
-000001c0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
-000001d0: 622e 636f 6d2f 7965 7a7a 3132 332f 6175  b.com/yezz123/au
-000001e0: 7468 782f 6163 7469 6f6e 732f 776f 726b  thx/actions/work
-000001f0: 666c 6f77 732f 6369 2e79 6d6c 2f62 6164  flows/ci.yml/bad
-00000200: 6765 2e73 7667 2220 616c 743d 226c 696e  ge.svg" alt="lin
-00000210: 7422 3e0a 3c2f 613e 0a3c 6120 6872 6566  t">.</a>.<a href
-00000220: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
-00000230: 7267 2f70 726f 6a65 6374 2f61 7574 6878  rg/project/authx
-00000240: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00000250: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
-00000260: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000270: 656c 6473 2e69 6f2f 7079 7069 2f76 2f61  elds.io/pypi/v/a
-00000280: 7574 6878 3f63 6f6c 6f72 3d25 3233 3334  uthx?color=%2334
-00000290: 4430 3538 266c 6162 656c 3d70 7970 6925  D058&label=pypi%
-000002a0: 3230 7061 636b 6167 6522 2061 6c74 3d22  20package" alt="
-000002b0: 5061 636b 6167 6520 7665 7273 696f 6e22  Package version"
-000002c0: 3e0a 3c2f 613e 0a3c 6120 6872 6566 3d22  >.</a>.<a href="
-000002d0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
-000002e0: 696f 2f67 682f 7965 7a7a 3132 332f 6175  io/gh/yezz123/au
-000002f0: 7468 7822 3e0a 2020 2020 3c69 6d67 2073  thx">.    <img s
-00000300: 7263 3d22 6874 7470 733a 2f2f 636f 6465  rc="https://code
-00000310: 636f 762e 696f 2f67 682f 7965 7a7a 3132  cov.io/gh/yezz12
-00000320: 332f 6175 7468 782f 6272 616e 6368 2f6d  3/authx/branch/m
-00000330: 6169 6e2f 6772 6170 682f 6261 6467 652e  ain/graph/badge.
-00000340: 7376 6722 2f3e 0a3c 2f61 3e0a 3c61 2068  svg"/>.</a>.<a h
-00000350: 7265 663d 2268 7474 7073 3a2f 2f70 6570  ref="https://pep
-00000360: 792e 7465 6368 2f70 726f 6a65 6374 2f61  y.tech/project/a
-00000370: 7574 6878 2220 7461 7267 6574 3d22 5f62  uthx" target="_b
-00000380: 6c61 6e6b 223e 0a20 2020 203c 696d 6720  lank">.    <img 
-00000390: 7372 633d 2268 7474 7073 3a2f 2f73 7461  src="https://sta
-000003a0: 7469 632e 7065 7079 2e74 6563 682f 6261  tic.pepy.tech/ba
-000003b0: 6467 652f 6175 7468 7822 2061 6c74 3d22  dge/authx" alt="
-000003c0: 5465 7374 223e 0a3c 2f61 3e0a 3c61 2068  Test">.</a>.<a h
-000003d0: 7265 663d 2268 7474 7073 3a2f 2f70 7964  ref="https://pyd
-000003e0: 616e 7469 632e 6465 7622 2074 6172 6765  antic.dev" targe
-000003f0: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
-00000400: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000410: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000420: 2f65 6e64 706f 696e 743f 7572 6c3d 6874  /endpoint?url=ht
-00000430: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000440: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000450: 7079 6461 6e74 6963 2f70 7964 616e 7469  pydantic/pydanti
-00000460: 632f 6d61 696e 2f64 6f63 732f 6261 6467  c/main/docs/badg
-00000470: 652f 7632 2e6a 736f 6e22 2061 6c74 3d22  e/v2.json" alt="
-00000480: 5079 6461 6e74 6963 2056 6572 7369 6f6e  Pydantic Version
-00000490: 2032 223e 0a3c 2f61 3e0a 3c2f 703e 0a3c   2">.</a>.</p>.<
-000004a0: 2f70 3e0a 0a2d 2d2d 0a0a 2a2a 536f 7572  /p>..---..**Sour
-000004b0: 6365 2043 6f64 652a 2a3a 203c 6874 7470  ce Code**: <http
-000004c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
-000004d0: 657a 7a31 3233 2f61 7574 6878 3e0a 0a2a  ezz123/authx>..*
-000004e0: 2a44 6f63 756d 656e 7461 7469 6f6e 2a2a  *Documentation**
-000004f0: 3a20 3c68 7474 7073 3a2f 2f61 7574 6878  : <https://authx
-00000500: 2e79 657a 7a2e 6d65 2f3e 0a0a 2d2d 2d0a  .yezz.me/>..---.
-00000510: 0a41 6464 2061 2046 756c 6c79 2072 6567  .Add a Fully reg
-00000520: 6973 7472 6174 696f 6e20 616e 6420 6175  istration and au
-00000530: 7468 656e 7469 6361 7469 6f6e 206f 7220  thentication or 
-00000540: 6175 7468 6f72 697a 6174 696f 6e20 7379  authorization sy
-00000550: 7374 656d 2074 6f20 796f 7572 0a5b 4661  stem to your.[Fa
-00000560: 7374 4150 495d 2868 7474 7073 3a2f 2f66  stAPI](https://f
-00000570: 6173 7461 7069 2e74 6961 6e67 6f6c 6f2e  astapi.tiangolo.
-00000580: 636f 6d2f 2920 7072 6f6a 6563 742e 202a  com/) project. *
-00000590: 2a41 7574 6858 2a2a 2069 7320 6465 7369  *AuthX** is desi
-000005a0: 676e 6564 2074 6f20 6265 2061 730a 6375  gned to be as.cu
-000005b0: 7374 6f6d 697a 6162 6c65 2061 6e64 2061  stomizable and a
-000005c0: 6461 7074 6162 6c65 2061 7320 706f 7373  daptable as poss
-000005d0: 6962 6c65 2e0a 0a23 2320 4665 6174 7572  ible...## Featur
-000005e0: 6573 0a0a 2d20 5b78 5d20 5375 7070 6f72  es..- [x] Suppor
-000005f0: 7420 5079 7468 6f6e 2033 2e38 2b20 2620  t Python 3.8+ & 
-00000600: 5079 6461 6e74 6963 2032 2e30 2b2e 0a2d  Pydantic 2.0+..-
-00000610: 205b 785d 204d 756c 7469 706c 6520 6375   [x] Multiple cu
-00000620: 7374 6f6d 697a 6162 6c65 2061 7574 6865  stomizable authe
-00000630: 6e74 6963 6174 696f 6e20 6261 636b 656e  ntication backen
-00000640: 643a 0a20 202d 205b 785d 204a 5754 2061  d:.  - [x] JWT a
-00000650: 7574 6865 6e74 6963 6174 696f 6e20 6261  uthentication ba
-00000660: 636b 656e 6420 696e 636c 7564 6564 0a20  ckend included. 
-00000670: 2020 202d 205b 785d 204a 5754 2065 6e63     - [x] JWT enc
-00000680: 6f64 696e 672f 6465 636f 6469 6e67 2066  oding/decoding f
-00000690: 6f72 2061 7070 6c69 6361 7469 6f6e 2061  or application a
-000006a0: 7574 6865 6e74 6963 6174 696f 6e0a 2020  uthentication.  
-000006b0: 2020 2d20 5b78 5d20 4175 746f 6d61 7469    - [x] Automati
-000006c0: 6320 6465 7465 6374 696f 6e20 6f66 204a  c detection of J
-000006d0: 5754 7320 696e 2072 6571 7565 7374 733a  WTs in requests:
-000006e0: 0a20 2020 2020 202d 205b 785d 204a 5754  .      - [x] JWT
-000006f0: 7320 696e 2068 6561 6465 7273 0a20 2020  s in headers.   
-00000700: 2020 202d 205b 785d 204a 5754 7320 696e     - [x] JWTs in
-00000710: 2063 6f6f 6b69 6573 0a20 2020 2020 202d   cookies.      -
-00000720: 205b 785d 204a 5754 7320 696e 2071 7565   [x] JWTs in que
-00000730: 7279 2070 6172 616d 6574 6572 730a 2020  ry parameters.  
-00000740: 2020 2020 2d20 5b78 5d20 4a57 5473 2069      - [x] JWTs i
-00000750: 6e20 7265 7175 6573 7420 626f 6469 6573  n request bodies
-00000760: 0a20 202d 205b 785d 2043 6f6f 6b69 6520  .  - [x] Cookie 
-00000770: 6175 7468 656e 7469 6361 7469 6f6e 2062  authentication b
-00000780: 6163 6b65 6e64 2069 6e63 6c75 6465 640a  ackend included.
-00000790: 2d20 5b78 5d20 4d69 6464 6c65 7761 7265  - [x] Middleware
-000007a0: 2066 6f72 2061 7574 6865 6e74 6963 6174   for authenticat
-000007b0: 696f 6e20 616e 6420 6175 7468 6f72 697a  ion and authoriz
-000007c0: 6174 696f 6e20 7468 726f 7567 6820 4a57  ation through JW
-000007d0: 542e 0a2d 205b 785d 2045 7874 656e 7369  T..- [x] Extensi
-000007e0: 626c 6520 4572 726f 7220 4861 6e64 6c69  ble Error Handli
-000007f0: 6e67 2053 7973 7465 6d2e 0a0a 2323 2320  ng System...### 
-00000800: 4578 7472 6120 4665 6174 7572 6573 0a0a  Extra Features..
-00000810: 4175 7468 5820 6973 2064 6573 6967 6e65  AuthX is designe
-00000820: 6420 746f 2062 6520 6173 2063 7573 746f  d to be as custo
-00000830: 6d69 7a61 626c 6520 616e 6420 6164 6170  mizable and adap
-00000840: 7461 626c 6520 6173 2070 6f73 7369 626c  table as possibl
-00000850: 652e 0a0a 536f 2079 6f75 206e 6565 6420  e...So you need 
-00000860: 746f 2069 6e73 7461 6c6c 205b 6061 7574  to install [`aut
-00000870: 6878 2d65 7874 7261 605d 2868 7474 7073  hx-extra`](https
-00000880: 3a2f 2f67 6974 6875 622e 636f 6d2f 7965  ://github.com/ye
-00000890: 7a7a 3132 332f 6175 7468 782d 6578 7472  zz123/authx-extr
-000008a0: 6129 2074 6f20 6765 7420 6578 7472 6120  a) to get extra 
-000008b0: 6665 6174 7572 6573 2e0a 0a2d 205b 785d  features...- [x]
-000008c0: 2055 7369 6e67 2052 6564 6973 2061 7320   Using Redis as 
-000008d0: 6120 7365 7373 696f 6e20 7374 6f72 6520  a session store 
-000008e0: 2620 6361 6368 652e 0a2d 205b 785d 2053  & cache..- [x] S
-000008f0: 7570 706f 7274 2048 5454 5043 6163 6865  upport HTTPCache
-00000900: 2e0a 2d20 5b78 5d20 5375 7070 6f72 7420  ..- [x] Support 
-00000910: 5365 7373 696f 6e73 2061 6e64 2050 7265  Sessions and Pre
-00000920: 2d62 7569 6c74 2043 5255 4420 6675 6e63  -built CRUD func
-00000930: 7469 6f6e 7320 616e 6420 496e 7374 616e  tions and Instan
-00000940: 6365 2074 6f20 6c61 756e 6368 2052 6564  ce to launch Red
-00000950: 6973 2e0a 2d20 5b78 5d20 5375 7070 6f72  is..- [x] Suppor
-00000960: 7420 4d69 6464 6c65 7761 7265 206f 6620  t Middleware of 
-00000970: 5b70 7969 6e73 7472 756d 656e 745d 2868  [pyinstrument](h
-00000980: 7474 7073 3a2f 2f70 7969 6e73 7472 756d  ttps://pyinstrum
-00000990: 656e 742e 7265 6164 7468 6564 6f63 732e  ent.readthedocs.
-000009a0: 696f 2f29 2074 6f20 6368 6563 6b20 796f  io/) to check yo
-000009b0: 7572 2073 6572 7669 6365 2070 6572 666f  ur service perfo
-000009c0: 726d 616e 6365 2e0a 2d20 5b78 5d20 5375  rmance..- [x] Su
-000009d0: 7070 6f72 7420 4d69 6464 6c65 7761 7265  pport Middleware
-000009e0: 2066 6f72 2063 6f6c 6c65 6374 696e 6720   for collecting 
-000009f0: 616e 6420 6578 706f 7369 6e67 205b 5072  and exposing [Pr
-00000a00: 6f6d 6574 6865 7573 5d28 6874 7470 733a  ometheus](https:
-00000a10: 2f2f 7072 6f6d 6574 6865 7573 2e69 6f2f  //prometheus.io/
-00000a20: 2920 6d65 7472 6963 732e 0a0a 2a2a 4e6f  ) metrics...**No
-00000a30: 7465 3a2a 2a20 4368 6563 6b20 5b52 656c  te:** Check [Rel
-00000a40: 6561 7365 204e 6f74 6573 5d28 6874 7470  ease Notes](http
-00000a50: 733a 2f2f 6175 7468 782e 7965 7a7a 2e6d  s://authx.yezz.m
-00000a60: 652f 7265 6c65 6173 652f 292e 0a0a 2323  e/release/)...##
-00000a70: 2050 726f 6a65 6374 2075 7369 6e67 0a0a   Project using..
-00000a80: 4865 7265 2069 7320 6120 7369 6d70 6c65  Here is a simple
-00000a90: 2077 6179 2074 6f20 6b69 636b 7374 6172   way to kickstar
-00000aa0: 7420 796f 7572 2070 726f 6a65 6374 2077  t your project w
-00000ab0: 6974 6820 4175 7468 583a 0a0a 6060 6070  ith AuthX:..```p
-00000ac0: 7974 686f 6e0a 6672 6f6d 2066 6173 7461  ython.from fasta
-00000ad0: 7069 2069 6d70 6f72 7420 4661 7374 4150  pi import FastAP
-00000ae0: 492c 2044 6570 656e 6473 2c20 4854 5450  I, Depends, HTTP
-00000af0: 4578 6365 7074 696f 6e0a 6672 6f6d 2061  Exception.from a
-00000b00: 7574 6878 2069 6d70 6f72 7420 4175 7468  uthx import Auth
-00000b10: 582c 2041 7574 6858 436f 6e66 6967 2c20  X, AuthXConfig, 
-00000b20: 5265 7175 6573 7454 6f6b 656e 0a0a 6170  RequestToken..ap
-00000b30: 7020 3d20 4661 7374 4150 4928 290a 0a63  p = FastAPI()..c
-00000b40: 6f6e 6669 6720 3d20 4175 7468 5843 6f6e  onfig = AuthXCon
-00000b50: 6669 6728 0a20 2020 2020 4a57 545f 414c  fig(.     JWT_AL
-00000b60: 474f 5249 5448 4d20 3d20 2248 5332 3536  GORITHM = "HS256
-00000b70: 222c 0a20 2020 2020 4a57 545f 5345 4352  ",.     JWT_SECR
-00000b80: 4554 5f4b 4559 203d 2022 5345 4352 4554  ET_KEY = "SECRET
-00000b90: 5f4b 4559 222c 0a20 2020 2020 4a57 545f  _KEY",.     JWT_
-00000ba0: 544f 4b45 4e5f 4c4f 4341 5449 4f4e 203d  TOKEN_LOCATION =
-00000bb0: 205b 2268 6561 6465 7273 225d 2c0a 290a   ["headers"],.).
-00000bc0: 0a61 7574 6820 3d20 4175 7468 5828 636f  .auth = AuthX(co
-00000bd0: 6e66 6967 3d63 6f6e 6669 6729 0a61 7574  nfig=config).aut
-00000be0: 682e 6861 6e64 6c65 5f65 7272 6f72 7328  h.handle_errors(
-00000bf0: 6170 7029 0a0a 4061 7070 2e67 6574 2827  app)..@app.get('
-00000c00: 2f6c 6f67 696e 2729 0a64 6566 206c 6f67  /login').def log
-00000c10: 696e 2875 7365 726e 616d 653a 2073 7472  in(username: str
-00000c20: 2c20 7061 7373 776f 7264 3a20 7374 7229  , password: str)
-00000c30: 3a0a 2020 2020 2069 6620 7573 6572 6e61  :.     if userna
-00000c40: 6d65 203d 3d20 2278 797a 2220 616e 6420  me == "xyz" and 
-00000c50: 7061 7373 776f 7264 203d 3d20 2278 797a  password == "xyz
-00000c60: 223a 0a20 2020 2020 2020 2020 2074 6f6b  ":.          tok
-00000c70: 656e 203d 2061 7574 682e 6372 6561 7465  en = auth.create
-00000c80: 5f61 6363 6573 735f 746f 6b65 6e28 7569  _access_token(ui
-00000c90: 643d 7573 6572 6e61 6d65 290a 2020 2020  d=username).    
-00000ca0: 2020 2020 2020 7265 7475 726e 207b 2261        return {"a
-00000cb0: 6363 6573 735f 746f 6b65 6e22 3a20 746f  ccess_token": to
-00000cc0: 6b65 6e7d 0a20 2020 2020 7261 6973 6520  ken}.     raise 
-00000cd0: 4854 5450 4578 6365 7074 696f 6e28 3430  HTTPException(40
-00000ce0: 312c 2064 6574 6169 6c3d 7b22 6d65 7373  1, detail={"mess
-00000cf0: 6167 6522 3a20 2249 6e76 616c 6964 2063  age": "Invalid c
-00000d00: 7265 6465 6e74 6961 6c73 227d 290a 0a40  redentials"})..@
-00000d10: 6170 702e 6765 7428 222f 7072 6f74 6563  app.get("/protec
-00000d20: 7465 6422 2c20 6465 7065 6e64 656e 6369  ted", dependenci
-00000d30: 6573 3d5b 4465 7065 6e64 7328 6175 7468  es=[Depends(auth
-00000d40: 2e67 6574 5f74 6f6b 656e 5f66 726f 6d5f  .get_token_from_
-00000d50: 7265 7175 6573 7429 5d29 0a64 6566 2067  request)]).def g
-00000d60: 6574 5f70 726f 7465 6374 6564 2874 6f6b  et_protected(tok
-00000d70: 656e 3a20 5265 7175 6573 7454 6f6b 656e  en: RequestToken
-00000d80: 203d 2044 6570 656e 6473 2829 293a 0a20   = Depends()):. 
-00000d90: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00000da0: 2020 2061 7574 682e 7665 7269 6679 5f74     auth.verify_t
-00000db0: 6f6b 656e 2874 6f6b 656e 3d74 6f6b 656e  oken(token=token
-00000dc0: 290a 2020 2020 2020 2020 2020 7265 7475  ).          retu
-00000dd0: 726e 207b 226d 6573 7361 6765 223a 2022  rn {"message": "
-00000de0: 4865 6c6c 6f20 776f 726c 6420 2122 7d0a  Hello world !"}.
-00000df0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00000e00: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
-00000e10: 2020 2020 2020 7261 6973 6520 4854 5450        raise HTTP
-00000e20: 4578 6365 7074 696f 6e28 3430 312c 2064  Exception(401, d
-00000e30: 6574 6169 6c3d 7b22 6d65 7373 6167 6522  etail={"message"
-00000e40: 3a20 7374 7228 6529 7d29 2066 726f 6d20  : str(e)}) from 
-00000e50: 650a 6060 600a 0a23 2320 436f 6e74 7269  e.```..## Contri
-00000e60: 6275 746f 7273 2061 6e64 2073 706f 6e73  butors and spons
-00000e70: 6f72 730a 0a3c 212d 2d20 414c 4c2d 434f  ors..<!-- ALL-CO
-00000e80: 4e54 5249 4255 544f 5253 2d42 4144 4745  NTRIBUTORS-BADGE
-00000e90: 3a53 5441 5254 202d 2044 6f20 6e6f 7420  :START - Do not 
-00000ea0: 7265 6d6f 7665 206f 7220 6d6f 6469 6679  remove or modify
-00000eb0: 2074 6869 7320 7365 6374 696f 6e20 2d2d   this section --
-00000ec0: 3e0a 5b21 5b41 6c6c 2043 6f6e 7472 6962  >.[![All Contrib
-00000ed0: 7574 6f72 735d 2868 7474 7073 3a2f 2f69  utors](https://i
-00000ee0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000ef0: 6467 652f 616c 6c5f 636f 6e74 7269 6275  dge/all_contribu
-00000f00: 746f 7273 2d31 302d 6f72 616e 6765 2e73  tors-10-orange.s
-00000f10: 7667 3f73 7479 6c65 3d66 6c61 742d 7371  vg?style=flat-sq
-00000f20: 7561 7265 295d 2823 636f 6e74 7269 6275  uare)](#contribu
-00000f30: 746f 7273 2d29 0a3c 212d 2d20 414c 4c2d  tors-).<!-- ALL-
-00000f40: 434f 4e54 5249 4255 544f 5253 2d42 4144  CONTRIBUTORS-BAD
-00000f50: 4745 3a45 4e44 202d 2d3e 0a0a 5468 616e  GE:END -->..Than
-00000f60: 6b73 2067 6f65 7320 746f 2074 6865 7365  ks goes to these
-00000f70: 2077 6f6e 6465 7266 756c 2070 656f 706c   wonderful peopl
-00000f80: 650a 285b 656d 6f6a 6920 6b65 795d 2868  e.([emoji key](h
-00000f90: 7474 7073 3a2f 2f61 6c6c 636f 6e74 7269  ttps://allcontri
-00000fa0: 6275 746f 7273 2e6f 7267 2f64 6f63 732f  butors.org/docs/
-00000fb0: 656e 2f65 6d6f 6a69 2d6b 6579 2929 3a0a  en/emoji-key)):.
-00000fc0: 0a3c 212d 2d20 414c 4c2d 434f 4e54 5249  .<!-- ALL-CONTRI
-00000fd0: 4255 544f 5253 2d4c 4953 543a 5354 4152  BUTORS-LIST:STAR
-00000fe0: 5420 2d20 446f 206e 6f74 2072 656d 6f76  T - Do not remov
-00000ff0: 6520 6f72 206d 6f64 6966 7920 7468 6973  e or modify this
-00001000: 2073 6563 7469 6f6e 202d 2d3e 0a3c 212d   section -->.<!-
-00001010: 2d20 7072 6574 7469 6572 2d69 676e 6f72  - prettier-ignor
-00001020: 652d 7374 6172 7420 2d2d 3e0a 3c21 2d2d  e-start -->.<!--
-00001030: 206d 6172 6b64 6f77 6e6c 696e 742d 6469   markdownlint-di
-00001040: 7361 626c 6520 2d2d 3e0a 3c74 6162 6c65  sable -->.<table
-00001050: 3e0a 2020 3c74 626f 6479 3e0a 2020 2020  >.  <tbody>.    
-00001060: 3c74 723e 0a20 2020 2020 203c 7464 2061  <tr>.      <td a
-00001070: 6c69 676e 3d22 6365 6e74 6572 2220 7661  lign="center" va
-00001080: 6c69 676e 3d22 746f 7022 2077 6964 7468  lign="top" width
-00001090: 3d22 3134 2e32 3825 223e 3c61 2068 7265  ="14.28%"><a hre
-000010a0: 663d 2268 7474 703a 2f2f 7965 7a7a 2e6d  f="http://yezz.m
-000010b0: 6522 3e3c 696d 6720 7372 633d 2268 7474  e"><img src="htt
-000010c0: 7073 3a2f 2f61 7661 7461 7273 2e67 6974  ps://avatars.git
-000010d0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-000010e0: 6f6d 2f75 2f35 3237 3136 3230 333f 763d  om/u/52716203?v=
-000010f0: 343f 733d 3130 3022 2077 6964 7468 3d22  4?s=100" width="
-00001100: 3130 3070 783b 2220 616c 743d 2259 6173  100px;" alt="Yas
-00001110: 7365 7220 5461 6869 7269 222f 3e3c 6272  ser Tahiri"/><br
-00001120: 202f 3e3c 7375 623e 3c62 3e59 6173 7365   /><sub><b>Yasse
-00001130: 7220 5461 6869 7269 3c2f 623e 3c2f 7375  r Tahiri</b></su
-00001140: 623e 3c2f 613e 3c62 7220 2f3e 3c61 2068  b></a><br /><a h
-00001150: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00001160: 6875 622e 636f 6d2f 7965 7a7a 3132 332f  hub.com/yezz123/
-00001170: 6175 7468 782f 636f 6d6d 6974 733f 6175  authx/commits?au
-00001180: 7468 6f72 3d79 657a 7a31 3233 2220 7469  thor=yezz123" ti
-00001190: 746c 653d 2243 6f64 6522 3ef0 9f92 bb3c  tle="Code">....<
-000011a0: 2f61 3e20 3c61 2068 7265 663d 2268 7474  /a> <a href="htt
-000011b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000011c0: 7965 7a7a 3132 332f 6175 7468 782f 636f  yezz123/authx/co
-000011d0: 6d6d 6974 733f 6175 7468 6f72 3d79 657a  mmits?author=yez
-000011e0: 7a31 3233 2220 7469 746c 653d 2244 6f63  z123" title="Doc
-000011f0: 756d 656e 7461 7469 6f6e 223e f09f 9396  umentation">....
-00001200: 3c2f 613e 203c 6120 6872 6566 3d22 236d  </a> <a href="#m
-00001210: 6169 6e74 656e 616e 6365 2d79 657a 7a31  aintenance-yezz1
-00001220: 3233 2220 7469 746c 653d 224d 6169 6e74  23" title="Maint
-00001230: 656e 616e 6365 223e f09f 9aa7 3c2f 613e  enance">....</a>
-00001240: 203c 6120 6872 6566 3d22 2369 6e66 7261   <a href="#infra
-00001250: 2d79 657a 7a31 3233 2220 7469 746c 653d  -yezz123" title=
-00001260: 2249 6e66 7261 7374 7275 6374 7572 6520  "Infrastructure 
-00001270: 2848 6f73 7469 6e67 2c20 4275 696c 642d  (Hosting, Build-
-00001280: 546f 6f6c 732c 2065 7463 2922 3ef0 9f9a  Tools, etc)">...
-00001290: 873c 2f61 3e3c 2f74 643e 0a20 2020 2020  .</a></td>.     
-000012a0: 203c 7464 2061 6c69 676e 3d22 6365 6e74   <td align="cent
-000012b0: 6572 2220 7661 6c69 676e 3d22 746f 7022  er" valign="top"
-000012c0: 2077 6964 7468 3d22 3134 2e32 3825 223e   width="14.28%">
-000012d0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000012e0: 2f73 6f75 6261 692e 6d65 223e 3c69 6d67  /soubai.me"><img
-000012f0: 2073 7263 3d22 6874 7470 733a 2f2f 6176   src="https://av
-00001300: 6174 6172 732e 6769 7468 7562 7573 6572  atars.githubuser
-00001310: 636f 6e74 656e 742e 636f 6d2f 752f 3131  content.com/u/11
-00001320: 3532 3337 3931 3f76 3d34 3f73 3d31 3030  523791?v=4?s=100
-00001330: 2220 7769 6474 683d 2231 3030 7078 3b22  " width="100px;"
-00001340: 2061 6c74 3d22 4162 6465 7272 6168 696d   alt="Abderrahim
-00001350: 2053 4f55 4241 492d 454c 4944 5249 5349   SOUBAI-ELIDRISI
-00001360: 222f 3e3c 6272 202f 3e3c 7375 623e 3c62  "/><br /><sub><b
-00001370: 3e41 6264 6572 7261 6869 6d20 534f 5542  >Abderrahim SOUB
-00001380: 4149 2d45 4c49 4452 4953 493c 2f62 3e3c  AI-ELIDRISI</b><
-00001390: 2f73 7562 3e3c 2f61 3e3c 6272 202f 3e3c  /sub></a><br /><
-000013a0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000013b0: 6769 7468 7562 2e63 6f6d 2f79 657a 7a31  github.com/yezz1
-000013c0: 3233 2f61 7574 6878 2f70 756c 6c73 3f71  23/authx/pulls?q
-000013d0: 3d69 7325 3341 7072 2b72 6576 6965 7765  =is%3Apr+reviewe
-000013e0: 642d 6279 2533 4141 6264 6572 7261 6869  d-by%3AAbderrahi
-000013f0: 6d53 6f75 6261 6945 6c69 6472 6973 7369  mSoubaiElidrissi
-00001400: 2220 7469 746c 653d 2252 6576 6965 7765  " title="Reviewe
-00001410: 6420 5075 6c6c 2052 6571 7565 7374 7322  d Pull Requests"
-00001420: 3ef0 9f91 803c 2f61 3e20 3c61 2068 7265  >....</a> <a hre
-00001430: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00001440: 622e 636f 6d2f 7965 7a7a 3132 332f 6175  b.com/yezz123/au
-00001450: 7468 782f 636f 6d6d 6974 733f 6175 7468  thx/commits?auth
-00001460: 6f72 3d41 6264 6572 7261 6869 6d53 6f75  or=AbderrahimSou
-00001470: 6261 6945 6c69 6472 6973 7369 2220 7469  baiElidrissi" ti
-00001480: 746c 653d 2244 6f63 756d 656e 7461 7469  tle="Documentati
-00001490: 6f6e 223e f09f 9396 3c2f 613e 3c2f 7464  on">....</a></td
-000014a0: 3e0a 2020 2020 2020 3c74 6420 616c 6967  >.      <td alig
-000014b0: 6e3d 2263 656e 7465 7222 2076 616c 6967  n="center" valig
-000014c0: 6e3d 2274 6f70 2220 7769 6474 683d 2231  n="top" width="1
-000014d0: 342e 3238 2522 3e3c 6120 6872 6566 3d22  4.28%"><a href="
-000014e0: 6874 7470 733a 2f2f 736d 616b 6f73 682e  https://smakosh.
-000014f0: 636f 6d22 3e3c 696d 6720 7372 633d 2268  com"><img src="h
-00001500: 7474 7073 3a2f 2f61 7661 7461 7273 2e67  ttps://avatars.g
-00001510: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00001520: 2e63 6f6d 2f75 2f32 3030 3832 3134 313f  .com/u/20082141?
-00001530: 763d 343f 733d 3130 3022 2077 6964 7468  v=4?s=100" width
-00001540: 3d22 3130 3070 783b 2220 616c 743d 2249  ="100px;" alt="I
-00001550: 736d 6169 6c20 4768 616c 6c6f 7520 222f  smail Ghallou "/
-00001560: 3e3c 6272 202f 3e3c 7375 623e 3c62 3e49  ><br /><sub><b>I
-00001570: 736d 6169 6c20 4768 616c 6c6f 7520 3c2f  smail Ghallou </
-00001580: 623e 3c2f 7375 623e 3c2f 613e 3c62 7220  b></sub></a><br 
-00001590: 2f3e 3c61 2068 7265 663d 2268 7474 7073  /><a href="https
-000015a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7965  ://github.com/ye
-000015b0: 7a7a 3132 332f 6175 7468 782f 636f 6d6d  zz123/authx/comm
-000015c0: 6974 733f 6175 7468 6f72 3d73 6d61 6b6f  its?author=smako
-000015d0: 7368 2220 7469 746c 653d 2243 6f64 6522  sh" title="Code"
-000015e0: 3ef0 9f92 bb3c 2f61 3e20 3c61 2068 7265  >....</a> <a hre
-000015f0: 663d 2223 7365 6375 7269 7479 2d73 6d61  f="#security-sma
-00001600: 6b6f 7368 2220 7469 746c 653d 2253 6563  kosh" title="Sec
-00001610: 7572 6974 7922 3ef0 9f9b a1ef b88f 3c2f  urity">.......</
-00001620: 613e 3c2f 7464 3e0a 2020 2020 2020 3c74  a></td>.      <t
-00001630: 6420 616c 6967 6e3d 2263 656e 7465 7222  d align="center"
-00001640: 2076 616c 6967 6e3d 2274 6f70 2220 7769   valign="top" wi
-00001650: 6474 683d 2231 342e 3238 2522 3e3c 6120  dth="14.28%"><a 
-00001660: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001670: 7468 7562 2e63 6f6d 2f4d 6f6a 6978 436f  thub.com/MojixCo
-00001680: 6465 7222 3e3c 696d 6720 7372 633d 2268  der"><img src="h
-00001690: 7474 7073 3a2f 2f61 7661 7461 7273 2e67  ttps://avatars.g
-000016a0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-000016b0: 2e63 6f6d 2f75 2f37 3636 3730 3330 393f  .com/u/76670309?
-000016c0: 763d 343f 733d 3130 3022 2077 6964 7468  v=4?s=100" width
-000016d0: 3d22 3130 3070 783b 2220 616c 743d 224d  ="100px;" alt="M
-000016e0: 6f6a 6978 436f 6465 7222 2f3e 3c62 7220  ojixCoder"/><br 
-000016f0: 2f3e 3c73 7562 3e3c 623e 4d6f 6a69 7843  /><sub><b>MojixC
-00001700: 6f64 6572 3c2f 623e 3c2f 7375 623e 3c2f  oder</b></sub></
-00001710: 613e 3c62 7220 2f3e 3c61 2068 7265 663d  a><br /><a href=
-00001720: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001730: 636f 6d2f 7965 7a7a 3132 332f 6175 7468  com/yezz123/auth
-00001740: 782f 636f 6d6d 6974 733f 6175 7468 6f72  x/commits?author
-00001750: 3d4d 6f6a 6978 436f 6465 7222 2074 6974  =MojixCoder" tit
-00001760: 6c65 3d22 436f 6465 223e f09f 92bb 3c2f  le="Code">....</
-00001770: 613e 203c 6120 6872 6566 3d22 6874 7470  a> <a href="http
-00001780: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
-00001790: 657a 7a31 3233 2f61 7574 6878 2f69 7373  ezz123/authx/iss
-000017a0: 7565 733f 713d 6175 7468 6f72 2533 414d  ues?q=author%3AM
-000017b0: 6f6a 6978 436f 6465 7222 2074 6974 6c65  ojixCoder" title
-000017c0: 3d22 4275 6720 7265 706f 7274 7322 3ef0  ="Bug reports">.
-000017d0: 9f90 9b3c 2f61 3e3c 2f74 643e 0a20 2020  ...</a></td>.   
-000017e0: 2020 203c 7464 2061 6c69 676e 3d22 6365     <td align="ce
-000017f0: 6e74 6572 2220 7661 6c69 676e 3d22 746f  nter" valign="to
-00001800: 7022 2077 6964 7468 3d22 3134 2e32 3825  p" width="14.28%
-00001810: 223e 3c61 2068 7265 663d 2268 7474 703a  "><a href="http:
-00001820: 2f2f 7372 616c 6162 2e63 6f6d 223e 3c69  //sralab.com"><i
-00001830: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001840: 6176 6174 6172 732e 6769 7468 7562 7573  avatars.githubus
-00001850: 6572 636f 6e74 656e 742e 636f 6d2f 752f  ercontent.com/u/
-00001860: 3138 3135 3f76 3d34 3f73 3d31 3030 2220  1815?v=4?s=100" 
-00001870: 7769 6474 683d 2231 3030 7078 3b22 2061  width="100px;" a
-00001880: 6c74 3d22 5374 c3a9 7068 616e 6520 5261  lt="St..phane Ra
-00001890: 696d 6261 756c 7422 2f3e 3c62 7220 2f3e  imbault"/><br />
-000018a0: 3c73 7562 3e3c 623e 5374 c3a9 7068 616e  <sub><b>St..phan
-000018b0: 6520 5261 696d 6261 756c 743c 2f62 3e3c  e Raimbault</b><
-000018c0: 2f73 7562 3e3c 2f61 3e3c 6272 202f 3e3c  /sub></a><br /><
-000018d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000018e0: 6769 7468 7562 2e63 6f6d 2f79 657a 7a31  github.com/yezz1
-000018f0: 3233 2f61 7574 6878 2f63 6f6d 6d69 7473  23/authx/commits
-00001900: 3f61 7574 686f 723d 7374 6570 6861 6e65  ?author=stephane
-00001910: 2220 7469 746c 653d 2243 6f64 6522 3ef0  " title="Code">.
-00001920: 9f92 bb3c 2f61 3e20 3c61 2068 7265 663d  ...</a> <a href=
-00001930: 2223 706c 7567 696e 2d73 7465 7068 616e  "#plugin-stephan
-00001940: 6522 2074 6974 6c65 3d22 506c 7567 696e  e" title="Plugin
-00001950: 2f75 7469 6c69 7479 206c 6962 7261 7269  /utility librari
-00001960: 6573 223e f09f 948c 3c2f 613e 3c2f 7464  es">....</a></td
-00001970: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
-00001980: 3c74 723e 0a20 2020 2020 203c 7464 2061  <tr>.      <td a
-00001990: 6c69 676e 3d22 6365 6e74 6572 2220 7661  lign="center" va
-000019a0: 6c69 676e 3d22 746f 7022 2077 6964 7468  lign="top" width
-000019b0: 3d22 3134 2e32 3825 223e 3c61 2068 7265  ="14.28%"><a hre
-000019c0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-000019d0: 622e 636f 6d2f 7468 656f 6f68 6f68 6f22  b.com/theoohoho"
-000019e0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-000019f0: 3a2f 2f61 7661 7461 7273 2e67 6974 6875  ://avatars.githu
-00001a00: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00001a10: 2f75 2f33 3135 3337 3436 363f 763d 343f  /u/31537466?v=4?
-00001a20: 733d 3130 3022 2077 6964 7468 3d22 3130  s=100" width="10
-00001a30: 3070 783b 2220 616c 743d 2274 6865 6f6f  0px;" alt="theoo
-00001a40: 686f 686f 222f 3e3c 6272 202f 3e3c 7375  hoho"/><br /><su
-00001a50: 623e 3c62 3e74 6865 6f6f 686f 686f 3c2f  b><b>theoohoho</
-00001a60: 623e 3c2f 7375 623e 3c2f 613e 3c62 7220  b></sub></a><br 
-00001a70: 2f3e 3c61 2068 7265 663d 2268 7474 7073  /><a href="https
-00001a80: 3a2f 2f67 6974 6875 622e 636f 6d2f 7965  ://github.com/ye
-00001a90: 7a7a 3132 332f 6175 7468 782f 636f 6d6d  zz123/authx/comm
-00001aa0: 6974 733f 6175 7468 6f72 3d74 6865 6f6f  its?author=theoo
-00001ab0: 686f 686f 2220 7469 746c 653d 2244 6f63  hoho" title="Doc
-00001ac0: 756d 656e 7461 7469 6f6e 223e f09f 9396  umentation">....
-00001ad0: 3c2f 613e 3c2f 7464 3e0a 2020 2020 2020  </a></td>.      
-00001ae0: 3c74 6420 616c 6967 6e3d 2263 656e 7465  <td align="cente
-00001af0: 7222 2076 616c 6967 6e3d 2274 6f70 2220  r" valign="top" 
-00001b00: 7769 6474 683d 2231 342e 3238 2522 3e3c  width="14.28%"><
-00001b10: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001b20: 796f 6765 7368 7570 6164 6879 6179 2e6e  yogeshupadhyay.n
-00001b30: 6574 6c69 6679 2e61 7070 2f22 3e3c 696d  etlify.app/"><im
-00001b40: 6720 7372 633d 2268 7474 7073 3a2f 2f61  g src="https://a
-00001b50: 7661 7461 7273 2e67 6974 6875 6275 7365  vatars.githubuse
-00001b60: 7263 6f6e 7465 6e74 2e63 6f6d 2f75 2f35  rcontent.com/u/5
-00001b70: 3339 3932 3136 383f 763d 343f 733d 3130  3992168?v=4?s=10
-00001b80: 3022 2077 6964 7468 3d22 3130 3070 783b  0" width="100px;
-00001b90: 2220 616c 743d 2259 6f67 6573 6820 5570  " alt="Yogesh Up
-00001ba0: 6164 6879 6179 222f 3e3c 6272 202f 3e3c  adhyay"/><br /><
-00001bb0: 7375 623e 3c62 3e59 6f67 6573 6820 5570  sub><b>Yogesh Up
-00001bc0: 6164 6879 6179 3c2f 623e 3c2f 7375 623e  adhyay</b></sub>
-00001bd0: 3c2f 613e 3c62 7220 2f3e 3c61 2068 7265  </a><br /><a hre
-00001be0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00001bf0: 622e 636f 6d2f 7965 7a7a 3132 332f 6175  b.com/yezz123/au
-00001c00: 7468 782f 6973 7375 6573 3f71 3d61 7574  thx/issues?q=aut
-00001c10: 686f 7225 3341 596f 6765 7368 5570 6468  hor%3AYogeshUpdh
-00001c20: 7961 7922 2074 6974 6c65 3d22 4275 6720  yay" title="Bug 
-00001c30: 7265 706f 7274 7322 3ef0 9f90 9b3c 2f61  reports">....</a
-00001c40: 3e3c 2f74 643e 0a20 2020 2020 203c 7464  ></td>.      <td
-00001c50: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
-00001c60: 7661 6c69 676e 3d22 746f 7022 2077 6964  valign="top" wid
-00001c70: 7468 3d22 3134 2e32 3825 223e 3c61 2068  th="14.28%"><a h
-00001c80: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00001c90: 6875 622e 636f 6d2f 6966 7465 6e65 7422  hub.com/iftenet"
-00001ca0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00001cb0: 3a2f 2f61 7661 7461 7273 2e67 6974 6875  ://avatars.githu
-00001cc0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00001cd0: 2f75 2f31 3339 3738 3830 3f76 3d34 3f73  /u/1397880?v=4?s
-00001ce0: 3d31 3030 2220 7769 6474 683d 2231 3030  =100" width="100
-00001cf0: 7078 3b22 2061 6c74 3d22 526f 6d61 6e22  px;" alt="Roman"
-00001d00: 2f3e 3c62 7220 2f3e 3c73 7562 3e3c 623e  /><br /><sub><b>
-00001d10: 526f 6d61 6e3c 2f62 3e3c 2f73 7562 3e3c  Roman</b></sub><
-00001d20: 2f61 3e3c 6272 202f 3e3c 6120 6872 6566  /a><br /><a href
-00001d30: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00001d40: 2e63 6f6d 2f79 657a 7a31 3233 2f61 7574  .com/yezz123/aut
-00001d50: 6878 2f69 7373 7565 733f 713d 6175 7468  hx/issues?q=auth
-00001d60: 6f72 2533 4169 6674 656e 6574 2220 7469  or%3Aiftenet" ti
-00001d70: 746c 653d 2242 7567 2072 6570 6f72 7473  tle="Bug reports
-00001d80: 223e f09f 909b 3c2f 613e 3c2f 7464 3e0a  ">....</a></td>.
-00001d90: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
-00001da0: 2263 656e 7465 7222 2076 616c 6967 6e3d  "center" valign=
-00001db0: 2274 6f70 2220 7769 6474 683d 2231 342e  "top" width="14.
-00001dc0: 3238 2522 3e3c 6120 6872 6566 3d22 6874  28%"><a href="ht
-00001dd0: 7470 733a 2f2f 7777 772e 6c69 6e6b 6564  tps://www.linked
-00001de0: 696e 2e63 6f6d 2f74 6f64 6179 2f61 7574  in.com/today/aut
-00001df0: 686f 722f 616c 6f62 6273 223e 3c69 6d67  hor/alobbs"><img
-00001e00: 2073 7263 3d22 6874 7470 733a 2f2f 6176   src="https://av
-00001e10: 6174 6172 732e 6769 7468 7562 7573 6572  atars.githubuser
-00001e20: 636f 6e74 656e 742e 636f 6d2f 752f 3137  content.com/u/17
-00001e30: 3035 3539 3f76 3d34 3f73 3d31 3030 2220  0559?v=4?s=100" 
-00001e40: 7769 6474 683d 2231 3030 7078 3b22 2061  width="100px;" a
-00001e50: 6c74 3d22 416c 7661 726f 204c 6f70 657a  lt="Alvaro Lopez
-00001e60: 204f 7274 6567 6122 2f3e 3c62 7220 2f3e   Ortega"/><br />
-00001e70: 3c73 7562 3e3c 623e 416c 7661 726f 204c  <sub><b>Alvaro L
-00001e80: 6f70 657a 204f 7274 6567 613c 2f62 3e3c  opez Ortega</b><
-00001e90: 2f73 7562 3e3c 2f61 3e3c 6272 202f 3e3c  /sub></a><br /><
-00001ea0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001eb0: 6769 7468 7562 2e63 6f6d 2f79 657a 7a31  github.com/yezz1
-00001ec0: 3233 2f61 7574 6878 2f63 6f6d 6d69 7473  23/authx/commits
-00001ed0: 3f61 7574 686f 723d 616c 6f62 6273 2220  ?author=alobbs" 
-00001ee0: 7469 746c 653d 2244 6f63 756d 656e 7461  title="Documenta
-00001ef0: 7469 6f6e 223e f09f 9396 3c2f 613e 3c2f  tion">....</a></
-00001f00: 7464 3e0a 2020 2020 2020 3c74 6420 616c  td>.      <td al
-00001f10: 6967 6e3d 2263 656e 7465 7222 2076 616c  ign="center" val
-00001f20: 6967 6e3d 2274 6f70 2220 7769 6474 683d  ign="top" width=
-00001f30: 2231 342e 3238 2522 3e3c 6120 6872 6566  "14.28%"><a href
-00001f40: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00001f50: 2e63 6f6d 2f70 696e 6368 584f 584f 223e  .com/pinchXOXO">
-00001f60: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001f70: 2f2f 6176 6174 6172 732e 6769 7468 7562  //avatars.github
-00001f80: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00001f90: 752f 3638 3530 3137 3939 3f76 3d34 3f73  u/68501799?v=4?s
-00001fa0: 3d31 3030 2220 7769 6474 683d 2231 3030  =100" width="100
-00001fb0: 7078 3b22 2061 6c74 3d22 4465 7679 2053  px;" alt="Devy S
-00001fc0: 616e 746f 222f 3e3c 6272 202f 3e3c 7375  anto"/><br /><su
-00001fd0: 623e 3c62 3e44 6576 7920 5361 6e74 6f3c  b><b>Devy Santo<
-00001fe0: 2f62 3e3c 2f73 7562 3e3c 2f61 3e3c 6272  /b></sub></a><br
-00001ff0: 202f 3e3c 6120 6872 6566 3d22 2369 6e66   /><a href="#inf
-00002000: 7261 2d70 696e 6368 584f 584f 2220 7469  ra-pinchXOXO" ti
-00002010: 746c 653d 2249 6e66 7261 7374 7275 6374  tle="Infrastruct
-00002020: 7572 6520 2848 6f73 7469 6e67 2c20 4275  ure (Hosting, Bu
-00002030: 696c 642d 546f 6f6c 732c 2065 7463 2922  ild-Tools, etc)"
-00002040: 3ef0 9f9a 873c 2f61 3e3c 2f74 643e 0a20  >....</a></td>. 
-00002050: 2020 203c 2f74 723e 0a20 203c 2f74 626f     </tr>.  </tbo
-00002060: 6479 3e0a 3c2f 7461 626c 653e 0a0a 3c21  dy>.</table>..<!
-00002070: 2d2d 206d 6172 6b64 6f77 6e6c 696e 742d  -- markdownlint-
-00002080: 7265 7374 6f72 6520 2d2d 3e0a 3c21 2d2d  restore -->.<!--
-00002090: 2070 7265 7474 6965 722d 6967 6e6f 7265   prettier-ignore
-000020a0: 2d65 6e64 202d 2d3e 0a0a 3c21 2d2d 2041  -end -->..<!-- A
-000020b0: 4c4c 2d43 4f4e 5452 4942 5554 4f52 532d  LL-CONTRIBUTORS-
-000020c0: 4c49 5354 3a45 4e44 202d 2d3e 0a0a 3c21  LIST:END -->..<!
-000020d0: 2d2d 2041 4c4c 2d43 4f4e 5452 4942 5554  -- ALL-CONTRIBUT
-000020e0: 4f52 532d 4c49 5354 3a53 5441 5254 202d  ORS-LIST:START -
-000020f0: 2044 6f20 6e6f 7420 7265 6d6f 7665 206f   Do not remove o
-00002100: 7220 6d6f 6469 6679 2074 6869 7320 7365  r modify this se
-00002110: 6374 696f 6e20 2d2d 3e0a 3c21 2d2d 2070  ction -->.<!-- p
-00002120: 7265 7474 6965 722d 6967 6e6f 7265 2d73  rettier-ignore-s
-00002130: 7461 7274 202d 2d3e 0a3c 212d 2d20 6d61  tart -->.<!-- ma
-00002140: 726b 646f 776e 6c69 6e74 2d64 6973 6162  rkdownlint-disab
-00002150: 6c65 202d 2d3e 0a0a 3c21 2d2d 206d 6172  le -->..<!-- mar
-00002160: 6b64 6f77 6e6c 696e 742d 7265 7374 6f72  kdownlint-restor
-00002170: 6520 2d2d 3e0a 3c21 2d2d 2070 7265 7474  e -->.<!-- prett
-00002180: 6965 722d 6967 6e6f 7265 2d65 6e64 202d  ier-ignore-end -
-00002190: 2d3e 0a0a 3c21 2d2d 2041 4c4c 2d43 4f4e  ->..<!-- ALL-CON
-000021a0: 5452 4942 5554 4f52 532d 4c49 5354 3a45  TRIBUTORS-LIST:E
-000021b0: 4e44 202d 2d3e 0a0a 5468 6973 2070 726f  ND -->..This pro
-000021c0: 6a65 6374 2066 6f6c 6c6f 7773 2074 6865  ject follows the
-000021d0: 0a5b 616c 6c2d 636f 6e74 7269 6275 746f  .[all-contributo
-000021e0: 7273 5d28 6874 7470 733a 2f2f 6769 7468  rs](https://gith
-000021f0: 7562 2e63 6f6d 2f61 6c6c 2d63 6f6e 7472  ub.com/all-contr
-00002200: 6962 7574 6f72 732f 616c 6c2d 636f 6e74  ibutors/all-cont
-00002210: 7269 6275 746f 7273 290a 7370 6563 6966  ributors).specif
-00002220: 6963 6174 696f 6e2e 2043 6f6e 7472 6962  ication. Contrib
-00002230: 7574 696f 6e73 206f 6620 616e 7920 6b69  utions of any ki
-00002240: 6e64 2077 656c 636f 6d65 210a 0a23 2320  nd welcome!..## 
-00002250: 4c69 6365 6e73 650a 0a54 6869 7320 7072  License..This pr
-00002260: 6f6a 6563 7420 6973 206c 6963 656e 7365  oject is license
-00002270: 6420 756e 6465 7220 7468 6520 7465 726d  d under the term
-00002280: 7320 6f66 2074 6865 204d 4954 204c 6963  s of the MIT Lic
-00002290: 656e 7365 2e0a                           ense..
+00000140: 9aa1 3c2f 656d 3e0a 3c2f 703e 0a3c 2f70  ..</em>.</p>.</p
+00000150: 3e0a 0a2d 2d2d 0a0a 7c20 5072 6f6a 6563  >..---..| Projec
+00000160: 7420 7c20 5374 6174 7573 2020 2020 2020  t | Status      
+00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003a0: 2020 2020 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d      |.|---------
+000003b0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+000003c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000003d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000003e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000003f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000004f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000005a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000005b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000005c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000005d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000005e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000005f0: 2d2d 7c0a 7c20 4349 2020 2020 2020 7c20  --|.| CI      | 
+00000600: 5b20 215b 2043 4920 5d28 2068 7474 7073  [ ![ CI ]( https
+00000610: 3a2f 2f67 6974 6875 622e 636f 6d2f 7965  ://github.com/ye
+00000620: 7a7a 3132 332f 6175 7468 782f 6163 7469  zz123/authx/acti
+00000630: 6f6e 732f 776f 726b 666c 6f77 732f 6369  ons/workflows/ci
+00000640: 2e79 6d6c 2f62 6164 6765 2e73 7667 2029  .yml/badge.svg )
+00000650: 205d 2820 6874 7470 733a 2f2f 6769 7468   ]( https://gith
+00000660: 7562 2e63 6f6d 2f79 657a 7a31 3233 2f61  ub.com/yezz123/a
+00000670: 7574 6878 2f61 6374 696f 6e73 2f77 6f72  uthx/actions/wor
+00000680: 6b66 6c6f 7773 2f63 692e 796d 6c20 2920  kflows/ci.yml ) 
+00000690: 205b 2021 5b20 7072 652d 636f 6d6d 6974   [ ![ pre-commit
+000006a0: 2e63 6920 7374 6174 7573 205d 2820 6874  .ci status ]( ht
+000006b0: 7470 733a 2f2f 7265 7375 6c74 732e 7072  tps://results.pr
+000006c0: 652d 636f 6d6d 6974 2e63 692f 6261 6467  e-commit.ci/badg
+000006d0: 652f 6769 7468 7562 2f79 657a 7a31 3233  e/github/yezz123
+000006e0: 2f61 7574 6878 2f6d 6169 6e2e 7376 6720  /authx/main.svg 
+000006f0: 2920 2020 5d28 2068 7474 7073 3a2f 2f72  )   ]( https://r
+00000700: 6573 756c 7473 2e70 7265 2d63 6f6d 6d69  esults.pre-commi
+00000710: 742e 6369 2f6c 6174 6573 742f 6769 7468  t.ci/latest/gith
+00000720: 7562 2f79 657a 7a31 3233 2f61 7574 6878  ub/yezz123/authx
+00000730: 2f6d 6169 6e20 2920 205b 2021 5b20 436f  /main )  [ ![ Co
+00000740: 6465 636f 7620 5d28 2068 7474 7073 3a2f  decov ]( https:/
+00000750: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f79  /codecov.io/gh/y
+00000760: 657a 7a31 3233 2f61 7574 6878 2f62 7261  ezz123/authx/bra
+00000770: 6e63 682f 6d61 696e 2f67 7261 7068 2f62  nch/main/graph/b
+00000780: 6164 6765 2e73 7667 2029 2020 205d 2820  adge.svg )   ]( 
+00000790: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+000007a0: 696f 2f67 682f 7965 7a7a 3132 332f 6175  io/gh/yezz123/au
+000007b0: 7468 7820 2920 7c0a 7c20 4d65 7461 2020  thx ) |.| Meta  
+000007c0: 2020 7c20 5b20 215b 2050 6163 6b61 6765    | [ ![ Package
+000007d0: 2076 6572 7369 6f6e 205d 2820 6874 7470   version ]( http
+000007e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000007f0: 696f 2f70 7970 692f 762f 6175 7468 783f  io/pypi/v/authx?
+00000800: 636f 6c6f 723d 2532 3333 3444 3035 3826  color=%2334D058&
+00000810: 6c61 6265 6c3d 7079 7069 2532 3070 6163  label=pypi%20pac
+00000820: 6b61 6765 2029 2020 205d 2820 6874 7470  kage )   ]( http
+00000830: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000840: 6a65 6374 2f61 7574 6878 2029 2020 5b20  ject/authx )  [ 
+00000850: 215b 2044 6f77 6e6c 6f61 6473 205d 2820  ![ Downloads ]( 
+00000860: 6874 7470 733a 2f2f 7374 6174 6963 2e70  https://static.p
+00000870: 6570 792e 7465 6368 2f62 6164 6765 2f61  epy.tech/badge/a
+00000880: 7574 6878 2029 2020 205d 2820 6874 7470  uthx )   ]( http
+00000890: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+000008a0: 6f6a 6563 742f 6175 7468 7820 2920 205b  oject/authx )  [
+000008b0: 2021 5b20 5079 6461 6e74 6963 2056 6572   ![ Pydantic Ver
+000008c0: 7369 6f6e 2032 205d 2820 6874 7470 733a  sion 2 ]( https:
+000008d0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000008e0: 2f65 6e64 706f 696e 743f 7572 6c3d 6874  /endpoint?url=ht
+000008f0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000900: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000910: 7079 6461 6e74 6963 2f70 7964 616e 7469  pydantic/pydanti
+00000920: 632f 6d61 696e 2f64 6f63 732f 6261 6467  c/main/docs/badg
+00000930: 652f 7632 2e6a 736f 6e20 2920 2020 5d28  e/v2.json )   ](
+00000940: 2068 7474 7073 3a2f 2f70 7964 616e 7469   https://pydanti
+00000950: 632e 6465 7620 2920 205b 2021 5b20 5275  c.dev )  [ ![ Ru
+00000960: 6666 205d 2820 6874 7470 733a 2f2f 696d  ff ]( https://im
+00000970: 672e 7368 6965 6c64 732e 696f 2f65 6e64  g.shields.io/end
+00000980: 706f 696e 743f 7572 6c3d 6874 7470 733a  point?url=https:
+00000990: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+000009a0: 636f 6e74 656e 742e 636f 6d2f 6173 7472  content.com/astr
+000009b0: 616c 2d73 682f 7275 6666 2f6d 6169 6e2f  al-sh/ruff/main/
+000009c0: 6173 7365 7473 2f62 6164 6765 2f76 322e  assets/badge/v2.
+000009d0: 6a73 6f6e 2029 205d 2820 6874 7470 733a  json ) ]( https:
+000009e0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7374  //github.com/ast
+000009f0: 7261 6c2d 7368 2f72 7566 6620 2920 2020  ral-sh/ruff )   
+00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a80: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00000a90: 0a2d 2d2d 0a0a 2a2a 536f 7572 6365 2043  .---..**Source C
+00000aa0: 6f64 652a 2a3a 203c 6874 7470 733a 2f2f  ode**: <https://
+00000ab0: 6769 7468 7562 2e63 6f6d 2f79 657a 7a31  github.com/yezz1
+00000ac0: 3233 2f61 7574 6878 3e0a 0a2a 2a44 6f63  23/authx>..**Doc
+00000ad0: 756d 656e 7461 7469 6f6e 2a2a 3a20 3c68  umentation**: <h
+00000ae0: 7474 7073 3a2f 2f61 7574 6878 2e79 657a  ttps://authx.yez
+00000af0: 7a2e 6d65 2f3e 0a0a 2d2d 2d0a 0a41 6464  z.me/>..---..Add
+00000b00: 2061 2046 756c 6c79 2072 6567 6973 7472   a Fully registr
+00000b10: 6174 696f 6e20 616e 6420 6175 7468 656e  ation and authen
+00000b20: 7469 6361 7469 6f6e 206f 7220 6175 7468  tication or auth
+00000b30: 6f72 697a 6174 696f 6e20 7379 7374 656d  orization system
+00000b40: 2074 6f20 796f 7572 0a5b 4661 7374 4150   to your.[FastAP
+00000b50: 495d 2868 7474 7073 3a2f 2f66 6173 7461  I](https://fasta
+00000b60: 7069 2e74 6961 6e67 6f6c 6f2e 636f 6d2f  pi.tiangolo.com/
+00000b70: 2920 7072 6f6a 6563 742e 202a 2a41 7574  ) project. **Aut
+00000b80: 6858 2a2a 2069 7320 6465 7369 676e 6564  hX** is designed
+00000b90: 2074 6f20 6265 2061 730a 6375 7374 6f6d   to be as.custom
+00000ba0: 697a 6162 6c65 2061 6e64 2061 6461 7074  izable and adapt
+00000bb0: 6162 6c65 2061 7320 706f 7373 6962 6c65  able as possible
+00000bc0: 2e0a 0a23 2320 4665 6174 7572 6573 0a0a  ...## Features..
+00000bd0: 2d20 5b78 5d20 5375 7070 6f72 7420 5079  - [x] Support Py
+00000be0: 7468 6f6e 2033 2e38 2b20 2620 5079 6461  thon 3.8+ & Pyda
+00000bf0: 6e74 6963 2032 2e30 2b2e 0a2d 205b 785d  ntic 2.0+..- [x]
+00000c00: 204d 756c 7469 706c 6520 6375 7374 6f6d   Multiple custom
+00000c10: 697a 6162 6c65 2061 7574 6865 6e74 6963  izable authentic
+00000c20: 6174 696f 6e20 6261 636b 656e 643a 0a20  ation backend:. 
+00000c30: 202d 205b 785d 204a 5754 2061 7574 6865   - [x] JWT authe
+00000c40: 6e74 6963 6174 696f 6e20 6261 636b 656e  ntication backen
+00000c50: 6420 696e 636c 7564 6564 0a20 2020 202d  d included.    -
+00000c60: 205b 785d 204a 5754 2065 6e63 6f64 696e   [x] JWT encodin
+00000c70: 672f 6465 636f 6469 6e67 2066 6f72 2061  g/decoding for a
+00000c80: 7070 6c69 6361 7469 6f6e 2061 7574 6865  pplication authe
+00000c90: 6e74 6963 6174 696f 6e0a 2020 2020 2d20  ntication.    - 
+00000ca0: 5b78 5d20 4175 746f 6d61 7469 6320 6465  [x] Automatic de
+00000cb0: 7465 6374 696f 6e20 6f66 204a 5754 7320  tection of JWTs 
+00000cc0: 696e 2072 6571 7565 7374 733a 0a20 2020  in requests:.   
+00000cd0: 2020 202d 205b 785d 204a 5754 7320 696e     - [x] JWTs in
+00000ce0: 2068 6561 6465 7273 0a20 2020 2020 202d   headers.      -
+00000cf0: 205b 785d 204a 5754 7320 696e 2063 6f6f   [x] JWTs in coo
+00000d00: 6b69 6573 0a20 2020 2020 202d 205b 785d  kies.      - [x]
+00000d10: 204a 5754 7320 696e 2071 7565 7279 2070   JWTs in query p
+00000d20: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00000d30: 2d20 5b78 5d20 4a57 5473 2069 6e20 7265  - [x] JWTs in re
+00000d40: 7175 6573 7420 626f 6469 6573 0a20 202d  quest bodies.  -
+00000d50: 205b 785d 2043 6f6f 6b69 6520 6175 7468   [x] Cookie auth
+00000d60: 656e 7469 6361 7469 6f6e 2062 6163 6b65  entication backe
+00000d70: 6e64 2069 6e63 6c75 6465 640a 2d20 5b78  nd included.- [x
+00000d80: 5d20 4d69 6464 6c65 7761 7265 2066 6f72  ] Middleware for
+00000d90: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
+00000da0: 616e 6420 6175 7468 6f72 697a 6174 696f  and authorizatio
+00000db0: 6e20 7468 726f 7567 6820 4a57 542e 0a2d  n through JWT..-
+00000dc0: 205b 785d 2045 7874 656e 7369 626c 6520   [x] Extensible 
+00000dd0: 4572 726f 7220 4861 6e64 6c69 6e67 2053  Error Handling S
+00000de0: 7973 7465 6d2e 0a0a 2323 2320 4578 7472  ystem...### Extr
+00000df0: 6120 4665 6174 7572 6573 0a0a 4175 7468  a Features..Auth
+00000e00: 5820 6973 2064 6573 6967 6e65 6420 746f  X is designed to
+00000e10: 2062 6520 6173 2063 7573 746f 6d69 7a61   be as customiza
+00000e20: 626c 6520 616e 6420 6164 6170 7461 626c  ble and adaptabl
+00000e30: 6520 6173 2070 6f73 7369 626c 652e 0a0a  e as possible...
+00000e40: 536f 2079 6f75 206e 6565 6420 746f 2069  So you need to i
+00000e50: 6e73 7461 6c6c 205b 6061 7574 6878 2d65  nstall [`authx-e
+00000e60: 7874 7261 605d 2868 7474 7073 3a2f 2f67  xtra`](https://g
+00000e70: 6974 6875 622e 636f 6d2f 7965 7a7a 3132  ithub.com/yezz12
+00000e80: 332f 6175 7468 782d 6578 7472 6129 2074  3/authx-extra) t
+00000e90: 6f20 6765 7420 6578 7472 6120 6665 6174  o get extra feat
+00000ea0: 7572 6573 2e0a 0a2d 205b 785d 2055 7369  ures...- [x] Usi
+00000eb0: 6e67 2052 6564 6973 2061 7320 6120 7365  ng Redis as a se
+00000ec0: 7373 696f 6e20 7374 6f72 6520 2620 6361  ssion store & ca
+00000ed0: 6368 652e 0a2d 205b 785d 2053 7570 706f  che..- [x] Suppo
+00000ee0: 7274 2048 5454 5043 6163 6865 2e0a 2d20  rt HTTPCache..- 
+00000ef0: 5b78 5d20 5375 7070 6f72 7420 5365 7373  [x] Support Sess
+00000f00: 696f 6e73 2061 6e64 2050 7265 2d62 7569  ions and Pre-bui
+00000f10: 6c74 2043 5255 4420 6675 6e63 7469 6f6e  lt CRUD function
+00000f20: 7320 616e 6420 496e 7374 616e 6365 2074  s and Instance t
+00000f30: 6f20 6c61 756e 6368 2052 6564 6973 2e0a  o launch Redis..
+00000f40: 2d20 5b78 5d20 5375 7070 6f72 7420 4d69  - [x] Support Mi
+00000f50: 6464 6c65 7761 7265 206f 6620 5b70 7969  ddleware of [pyi
+00000f60: 6e73 7472 756d 656e 745d 2868 7474 7073  nstrument](https
+00000f70: 3a2f 2f70 7969 6e73 7472 756d 656e 742e  ://pyinstrument.
+00000f80: 7265 6164 7468 6564 6f63 732e 696f 2f29  readthedocs.io/)
+00000f90: 2074 6f20 6368 6563 6b20 796f 7572 2073   to check your s
+00000fa0: 6572 7669 6365 2070 6572 666f 726d 616e  ervice performan
+00000fb0: 6365 2e0a 2d20 5b78 5d20 5375 7070 6f72  ce..- [x] Suppor
+00000fc0: 7420 4d69 6464 6c65 7761 7265 2066 6f72  t Middleware for
+00000fd0: 2063 6f6c 6c65 6374 696e 6720 616e 6420   collecting and 
+00000fe0: 6578 706f 7369 6e67 205b 5072 6f6d 6574  exposing [Promet
+00000ff0: 6865 7573 5d28 6874 7470 733a 2f2f 7072  heus](https://pr
+00001000: 6f6d 6574 6865 7573 2e69 6f2f 2920 6d65  ometheus.io/) me
+00001010: 7472 6963 732e 0a0a 2a2a 4e6f 7465 3a2a  trics...**Note:*
+00001020: 2a20 4368 6563 6b20 5b52 656c 6561 7365  * Check [Release
+00001030: 204e 6f74 6573 5d28 6874 7470 733a 2f2f   Notes](https://
+00001040: 6175 7468 782e 7965 7a7a 2e6d 652f 7265  authx.yezz.me/re
+00001050: 6c65 6173 652f 292e 0a0a 2323 2050 726f  lease/)...## Pro
+00001060: 6a65 6374 2075 7369 6e67 0a0a 4865 7265  ject using..Here
+00001070: 2069 7320 6120 7369 6d70 6c65 2077 6179   is a simple way
+00001080: 2074 6f20 6b69 636b 7374 6172 7420 796f   to kickstart yo
+00001090: 7572 2070 726f 6a65 6374 2077 6974 6820  ur project with 
+000010a0: 4175 7468 583a 0a0a 6060 6070 7974 686f  AuthX:..```pytho
+000010b0: 6e0a 6672 6f6d 2066 6173 7461 7069 2069  n.from fastapi i
+000010c0: 6d70 6f72 7420 4661 7374 4150 492c 2044  mport FastAPI, D
+000010d0: 6570 656e 6473 2c20 4854 5450 4578 6365  epends, HTTPExce
+000010e0: 7074 696f 6e0a 6672 6f6d 2061 7574 6878  ption.from authx
+000010f0: 2069 6d70 6f72 7420 4175 7468 582c 2041   import AuthX, A
+00001100: 7574 6858 436f 6e66 6967 2c20 5265 7175  uthXConfig, Requ
+00001110: 6573 7454 6f6b 656e 0a0a 6170 7020 3d20  estToken..app = 
+00001120: 4661 7374 4150 4928 290a 0a63 6f6e 6669  FastAPI()..confi
+00001130: 6720 3d20 4175 7468 5843 6f6e 6669 6728  g = AuthXConfig(
+00001140: 0a20 2020 2020 4a57 545f 414c 474f 5249  .     JWT_ALGORI
+00001150: 5448 4d20 3d20 2248 5332 3536 222c 0a20  THM = "HS256",. 
+00001160: 2020 2020 4a57 545f 5345 4352 4554 5f4b      JWT_SECRET_K
+00001170: 4559 203d 2022 5345 4352 4554 5f4b 4559  EY = "SECRET_KEY
+00001180: 222c 0a20 2020 2020 4a57 545f 544f 4b45  ",.     JWT_TOKE
+00001190: 4e5f 4c4f 4341 5449 4f4e 203d 205b 2268  N_LOCATION = ["h
+000011a0: 6561 6465 7273 225d 2c0a 290a 0a61 7574  eaders"],.)..aut
+000011b0: 6820 3d20 4175 7468 5828 636f 6e66 6967  h = AuthX(config
+000011c0: 3d63 6f6e 6669 6729 0a61 7574 682e 6861  =config).auth.ha
+000011d0: 6e64 6c65 5f65 7272 6f72 7328 6170 7029  ndle_errors(app)
+000011e0: 0a0a 4061 7070 2e67 6574 2827 2f6c 6f67  ..@app.get('/log
+000011f0: 696e 2729 0a64 6566 206c 6f67 696e 2875  in').def login(u
+00001200: 7365 726e 616d 653a 2073 7472 2c20 7061  sername: str, pa
+00001210: 7373 776f 7264 3a20 7374 7229 3a0a 2020  ssword: str):.  
+00001220: 2020 2069 6620 7573 6572 6e61 6d65 203d     if username =
+00001230: 3d20 2278 797a 2220 616e 6420 7061 7373  = "xyz" and pass
+00001240: 776f 7264 203d 3d20 2278 797a 223a 0a20  word == "xyz":. 
+00001250: 2020 2020 2020 2020 2074 6f6b 656e 203d           token =
+00001260: 2061 7574 682e 6372 6561 7465 5f61 6363   auth.create_acc
+00001270: 6573 735f 746f 6b65 6e28 7569 643d 7573  ess_token(uid=us
+00001280: 6572 6e61 6d65 290a 2020 2020 2020 2020  ername).        
+00001290: 2020 7265 7475 726e 207b 2261 6363 6573    return {"acces
+000012a0: 735f 746f 6b65 6e22 3a20 746f 6b65 6e7d  s_token": token}
+000012b0: 0a20 2020 2020 7261 6973 6520 4854 5450  .     raise HTTP
+000012c0: 4578 6365 7074 696f 6e28 3430 312c 2064  Exception(401, d
+000012d0: 6574 6169 6c3d 7b22 6d65 7373 6167 6522  etail={"message"
+000012e0: 3a20 2249 6e76 616c 6964 2063 7265 6465  : "Invalid crede
+000012f0: 6e74 6961 6c73 227d 290a 0a40 6170 702e  ntials"})..@app.
+00001300: 6765 7428 222f 7072 6f74 6563 7465 6422  get("/protected"
+00001310: 2c20 6465 7065 6e64 656e 6369 6573 3d5b  , dependencies=[
+00001320: 4465 7065 6e64 7328 6175 7468 2e67 6574  Depends(auth.get
+00001330: 5f74 6f6b 656e 5f66 726f 6d5f 7265 7175  _token_from_requ
+00001340: 6573 7429 5d29 0a64 6566 2067 6574 5f70  est)]).def get_p
+00001350: 726f 7465 6374 6564 2874 6f6b 656e 3a20  rotected(token: 
+00001360: 5265 7175 6573 7454 6f6b 656e 203d 2044  RequestToken = D
+00001370: 6570 656e 6473 2829 293a 0a20 2020 2020  epends()):.     
+00001380: 7472 793a 0a20 2020 2020 2020 2020 2061  try:.          a
+00001390: 7574 682e 7665 7269 6679 5f74 6f6b 656e  uth.verify_token
+000013a0: 2874 6f6b 656e 3d74 6f6b 656e 290a 2020  (token=token).  
+000013b0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+000013c0: 226d 6573 7361 6765 223a 2022 4865 6c6c  "message": "Hell
+000013d0: 6f20 776f 726c 6420 2122 7d0a 2020 2020  o world !"}.    
+000013e0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000013f0: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+00001400: 2020 7261 6973 6520 4854 5450 4578 6365    raise HTTPExce
+00001410: 7074 696f 6e28 3430 312c 2064 6574 6169  ption(401, detai
+00001420: 6c3d 7b22 6d65 7373 6167 6522 3a20 7374  l={"message": st
+00001430: 7228 6529 7d29 2066 726f 6d20 650a 6060  r(e)}) from e.``
+00001440: 600a 0a23 2320 436f 6e74 7269 6275 746f  `..## Contributo
+00001450: 7273 2061 6e64 2073 706f 6e73 6f72 730a  rs and sponsors.
+00001460: 0a3c 212d 2d20 414c 4c2d 434f 4e54 5249  .<!-- ALL-CONTRI
+00001470: 4255 544f 5253 2d42 4144 4745 3a53 5441  BUTORS-BADGE:STA
+00001480: 5254 202d 2044 6f20 6e6f 7420 7265 6d6f  RT - Do not remo
+00001490: 7665 206f 7220 6d6f 6469 6679 2074 6869  ve or modify thi
+000014a0: 7320 7365 6374 696f 6e20 2d2d 3e0a 5b21  s section -->.[!
+000014b0: 5b41 6c6c 2043 6f6e 7472 6962 7574 6f72  [All Contributor
+000014c0: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
+000014d0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000014e0: 616c 6c5f 636f 6e74 7269 6275 746f 7273  all_contributors
+000014f0: 2d31 302d 6f72 616e 6765 2e73 7667 3f73  -10-orange.svg?s
+00001500: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+00001510: 295d 2823 636f 6e74 7269 6275 746f 7273  )](#contributors
+00001520: 2d29 0a3c 212d 2d20 414c 4c2d 434f 4e54  -).<!-- ALL-CONT
+00001530: 5249 4255 544f 5253 2d42 4144 4745 3a45  RIBUTORS-BADGE:E
+00001540: 4e44 202d 2d3e 0a0a 5468 616e 6b73 2067  ND -->..Thanks g
+00001550: 6f65 7320 746f 2074 6865 7365 2077 6f6e  oes to these won
+00001560: 6465 7266 756c 2070 656f 706c 650a 285b  derful people.([
+00001570: 656d 6f6a 6920 6b65 795d 2868 7474 7073  emoji key](https
+00001580: 3a2f 2f61 6c6c 636f 6e74 7269 6275 746f  ://allcontributo
+00001590: 7273 2e6f 7267 2f64 6f63 732f 656e 2f65  rs.org/docs/en/e
+000015a0: 6d6f 6a69 2d6b 6579 2929 3a0a 0a3c 212d  moji-key)):..<!-
+000015b0: 2d20 414c 4c2d 434f 4e54 5249 4255 544f  - ALL-CONTRIBUTO
+000015c0: 5253 2d4c 4953 543a 5354 4152 5420 2d20  RS-LIST:START - 
+000015d0: 446f 206e 6f74 2072 656d 6f76 6520 6f72  Do not remove or
+000015e0: 206d 6f64 6966 7920 7468 6973 2073 6563   modify this sec
+000015f0: 7469 6f6e 202d 2d3e 0a3c 212d 2d20 7072  tion -->.<!-- pr
+00001600: 6574 7469 6572 2d69 676e 6f72 652d 7374  ettier-ignore-st
+00001610: 6172 7420 2d2d 3e0a 3c21 2d2d 206d 6172  art -->.<!-- mar
+00001620: 6b64 6f77 6e6c 696e 742d 6469 7361 626c  kdownlint-disabl
+00001630: 6520 2d2d 3e0a 3c74 6162 6c65 3e0a 2020  e -->.<table>.  
+00001640: 3c74 626f 6479 3e0a 2020 2020 3c74 723e  <tbody>.    <tr>
+00001650: 0a20 2020 2020 203c 7464 2061 6c69 676e  .      <td align
+00001660: 3d22 6365 6e74 6572 2220 7661 6c69 676e  ="center" valign
+00001670: 3d22 746f 7022 2077 6964 7468 3d22 3134  ="top" width="14
+00001680: 2e32 3825 223e 3c61 2068 7265 663d 2268  .28%"><a href="h
+00001690: 7474 703a 2f2f 7965 7a7a 2e6d 6522 3e3c  ttp://yezz.me"><
+000016a0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000016b0: 2f61 7661 7461 7273 2e67 6974 6875 6275  /avatars.githubu
+000016c0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f75  sercontent.com/u
+000016d0: 2f35 3237 3136 3230 333f 763d 343f 733d  /52716203?v=4?s=
+000016e0: 3130 3022 2077 6964 7468 3d22 3130 3070  100" width="100p
+000016f0: 783b 2220 616c 743d 2259 6173 7365 7220  x;" alt="Yasser 
+00001700: 5461 6869 7269 222f 3e3c 6272 202f 3e3c  Tahiri"/><br /><
+00001710: 7375 623e 3c62 3e59 6173 7365 7220 5461  sub><b>Yasser Ta
+00001720: 6869 7269 3c2f 623e 3c2f 7375 623e 3c2f  hiri</b></sub></
+00001730: 613e 3c62 7220 2f3e 3c61 2068 7265 663d  a><br /><a href=
+00001740: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00001750: 636f 6d2f 7965 7a7a 3132 332f 6175 7468  com/yezz123/auth
+00001760: 782f 636f 6d6d 6974 733f 6175 7468 6f72  x/commits?author
+00001770: 3d79 657a 7a31 3233 2220 7469 746c 653d  =yezz123" title=
+00001780: 2243 6f64 6522 3ef0 9f92 bb3c 2f61 3e20  "Code">....</a> 
+00001790: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000017a0: 2f67 6974 6875 622e 636f 6d2f 7965 7a7a  /github.com/yezz
+000017b0: 3132 332f 6175 7468 782f 636f 6d6d 6974  123/authx/commit
+000017c0: 733f 6175 7468 6f72 3d79 657a 7a31 3233  s?author=yezz123
+000017d0: 2220 7469 746c 653d 2244 6f63 756d 656e  " title="Documen
+000017e0: 7461 7469 6f6e 223e f09f 9396 3c2f 613e  tation">....</a>
+000017f0: 203c 6120 6872 6566 3d22 236d 6169 6e74   <a href="#maint
+00001800: 656e 616e 6365 2d79 657a 7a31 3233 2220  enance-yezz123" 
+00001810: 7469 746c 653d 224d 6169 6e74 656e 616e  title="Maintenan
+00001820: 6365 223e f09f 9aa7 3c2f 613e 203c 6120  ce">....</a> <a 
+00001830: 6872 6566 3d22 2369 6e66 7261 2d79 657a  href="#infra-yez
+00001840: 7a31 3233 2220 7469 746c 653d 2249 6e66  z123" title="Inf
+00001850: 7261 7374 7275 6374 7572 6520 2848 6f73  rastructure (Hos
+00001860: 7469 6e67 2c20 4275 696c 642d 546f 6f6c  ting, Build-Tool
+00001870: 732c 2065 7463 2922 3ef0 9f9a 873c 2f61  s, etc)">....</a
+00001880: 3e3c 2f74 643e 0a20 2020 2020 203c 7464  ></td>.      <td
+00001890: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
+000018a0: 7661 6c69 676e 3d22 746f 7022 2077 6964  valign="top" wid
+000018b0: 7468 3d22 3134 2e32 3825 223e 3c61 2068  th="14.28%"><a h
+000018c0: 7265 663d 2268 7474 7073 3a2f 2f73 6f75  ref="https://sou
+000018d0: 6261 692e 6d65 223e 3c69 6d67 2073 7263  bai.me"><img src
+000018e0: 3d22 6874 7470 733a 2f2f 6176 6174 6172  ="https://avatar
+000018f0: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
+00001900: 656e 742e 636f 6d2f 752f 3131 3532 3337  ent.com/u/115237
+00001910: 3931 3f76 3d34 3f73 3d31 3030 2220 7769  91?v=4?s=100" wi
+00001920: 6474 683d 2231 3030 7078 3b22 2061 6c74  dth="100px;" alt
+00001930: 3d22 4162 6465 7272 6168 696d 2053 4f55  ="Abderrahim SOU
+00001940: 4241 492d 454c 4944 5249 5349 222f 3e3c  BAI-ELIDRISI"/><
+00001950: 6272 202f 3e3c 7375 623e 3c62 3e41 6264  br /><sub><b>Abd
+00001960: 6572 7261 6869 6d20 534f 5542 4149 2d45  errahim SOUBAI-E
+00001970: 4c49 4452 4953 493c 2f62 3e3c 2f73 7562  LIDRISI</b></sub
+00001980: 3e3c 2f61 3e3c 6272 202f 3e3c 6120 6872  ></a><br /><a hr
+00001990: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000019a0: 7562 2e63 6f6d 2f79 657a 7a31 3233 2f61  ub.com/yezz123/a
+000019b0: 7574 6878 2f70 756c 6c73 3f71 3d69 7325  uthx/pulls?q=is%
+000019c0: 3341 7072 2b72 6576 6965 7765 642d 6279  3Apr+reviewed-by
+000019d0: 2533 4141 6264 6572 7261 6869 6d53 6f75  %3AAbderrahimSou
+000019e0: 6261 6945 6c69 6472 6973 7369 2220 7469  baiElidrissi" ti
+000019f0: 746c 653d 2252 6576 6965 7765 6420 5075  tle="Reviewed Pu
+00001a00: 6c6c 2052 6571 7565 7374 7322 3ef0 9f91  ll Requests">...
+00001a10: 803c 2f61 3e20 3c61 2068 7265 663d 2268  .</a> <a href="h
+00001a20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001a30: 6d2f 7965 7a7a 3132 332f 6175 7468 782f  m/yezz123/authx/
+00001a40: 636f 6d6d 6974 733f 6175 7468 6f72 3d41  commits?author=A
+00001a50: 6264 6572 7261 6869 6d53 6f75 6261 6945  bderrahimSoubaiE
+00001a60: 6c69 6472 6973 7369 2220 7469 746c 653d  lidrissi" title=
+00001a70: 2244 6f63 756d 656e 7461 7469 6f6e 223e  "Documentation">
+00001a80: f09f 9396 3c2f 613e 3c2f 7464 3e0a 2020  ....</a></td>.  
+00001a90: 2020 2020 3c74 6420 616c 6967 6e3d 2263      <td align="c
+00001aa0: 656e 7465 7222 2076 616c 6967 6e3d 2274  enter" valign="t
+00001ab0: 6f70 2220 7769 6474 683d 2231 342e 3238  op" width="14.28
+00001ac0: 2522 3e3c 6120 6872 6566 3d22 6874 7470  %"><a href="http
+00001ad0: 733a 2f2f 736d 616b 6f73 682e 636f 6d22  s://smakosh.com"
+00001ae0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00001af0: 3a2f 2f61 7661 7461 7273 2e67 6974 6875  ://avatars.githu
+00001b00: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00001b10: 2f75 2f32 3030 3832 3134 313f 763d 343f  /u/20082141?v=4?
+00001b20: 733d 3130 3022 2077 6964 7468 3d22 3130  s=100" width="10
+00001b30: 3070 783b 2220 616c 743d 2249 736d 6169  0px;" alt="Ismai
+00001b40: 6c20 4768 616c 6c6f 7520 222f 3e3c 6272  l Ghallou "/><br
+00001b50: 202f 3e3c 7375 623e 3c62 3e49 736d 6169   /><sub><b>Ismai
+00001b60: 6c20 4768 616c 6c6f 7520 3c2f 623e 3c2f  l Ghallou </b></
+00001b70: 7375 623e 3c2f 613e 3c62 7220 2f3e 3c61  sub></a><br /><a
+00001b80: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00001b90: 6974 6875 622e 636f 6d2f 7965 7a7a 3132  ithub.com/yezz12
+00001ba0: 332f 6175 7468 782f 636f 6d6d 6974 733f  3/authx/commits?
+00001bb0: 6175 7468 6f72 3d73 6d61 6b6f 7368 2220  author=smakosh" 
+00001bc0: 7469 746c 653d 2243 6f64 6522 3ef0 9f92  title="Code">...
+00001bd0: bb3c 2f61 3e20 3c61 2068 7265 663d 2223  .</a> <a href="#
+00001be0: 7365 6375 7269 7479 2d73 6d61 6b6f 7368  security-smakosh
+00001bf0: 2220 7469 746c 653d 2253 6563 7572 6974  " title="Securit
+00001c00: 7922 3ef0 9f9b a1ef b88f 3c2f 613e 3c2f  y">.......</a></
+00001c10: 7464 3e0a 2020 2020 2020 3c74 6420 616c  td>.      <td al
+00001c20: 6967 6e3d 2263 656e 7465 7222 2076 616c  ign="center" val
+00001c30: 6967 6e3d 2274 6f70 2220 7769 6474 683d  ign="top" width=
+00001c40: 2231 342e 3238 2522 3e3c 6120 6872 6566  "14.28%"><a href
+00001c50: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00001c60: 2e63 6f6d 2f4d 6f6a 6978 436f 6465 7222  .com/MojixCoder"
+00001c70: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00001c80: 3a2f 2f61 7661 7461 7273 2e67 6974 6875  ://avatars.githu
+00001c90: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00001ca0: 2f75 2f37 3636 3730 3330 393f 763d 343f  /u/76670309?v=4?
+00001cb0: 733d 3130 3022 2077 6964 7468 3d22 3130  s=100" width="10
+00001cc0: 3070 783b 2220 616c 743d 224d 6f6a 6978  0px;" alt="Mojix
+00001cd0: 436f 6465 7222 2f3e 3c62 7220 2f3e 3c73  Coder"/><br /><s
+00001ce0: 7562 3e3c 623e 4d6f 6a69 7843 6f64 6572  ub><b>MojixCoder
+00001cf0: 3c2f 623e 3c2f 7375 623e 3c2f 613e 3c62  </b></sub></a><b
+00001d00: 7220 2f3e 3c61 2068 7265 663d 2268 7474  r /><a href="htt
+00001d10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001d20: 7965 7a7a 3132 332f 6175 7468 782f 636f  yezz123/authx/co
+00001d30: 6d6d 6974 733f 6175 7468 6f72 3d4d 6f6a  mmits?author=Moj
+00001d40: 6978 436f 6465 7222 2074 6974 6c65 3d22  ixCoder" title="
+00001d50: 436f 6465 223e f09f 92bb 3c2f 613e 203c  Code">....</a> <
+00001d60: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001d70: 6769 7468 7562 2e63 6f6d 2f79 657a 7a31  github.com/yezz1
+00001d80: 3233 2f61 7574 6878 2f69 7373 7565 733f  23/authx/issues?
+00001d90: 713d 6175 7468 6f72 2533 414d 6f6a 6978  q=author%3AMojix
+00001da0: 436f 6465 7222 2074 6974 6c65 3d22 4275  Coder" title="Bu
+00001db0: 6720 7265 706f 7274 7322 3ef0 9f90 9b3c  g reports">....<
+00001dc0: 2f61 3e3c 2f74 643e 0a20 2020 2020 203c  /a></td>.      <
+00001dd0: 7464 2061 6c69 676e 3d22 6365 6e74 6572  td align="center
+00001de0: 2220 7661 6c69 676e 3d22 746f 7022 2077  " valign="top" w
+00001df0: 6964 7468 3d22 3134 2e32 3825 223e 3c61  idth="14.28%"><a
+00001e00: 2068 7265 663d 2268 7474 703a 2f2f 7372   href="http://sr
+00001e10: 616c 6162 2e63 6f6d 223e 3c69 6d67 2073  alab.com"><img s
+00001e20: 7263 3d22 6874 7470 733a 2f2f 6176 6174  rc="https://avat
+00001e30: 6172 732e 6769 7468 7562 7573 6572 636f  ars.githubuserco
+00001e40: 6e74 656e 742e 636f 6d2f 752f 3138 3135  ntent.com/u/1815
+00001e50: 3f76 3d34 3f73 3d31 3030 2220 7769 6474  ?v=4?s=100" widt
+00001e60: 683d 2231 3030 7078 3b22 2061 6c74 3d22  h="100px;" alt="
+00001e70: 5374 c3a9 7068 616e 6520 5261 696d 6261  St..phane Raimba
+00001e80: 756c 7422 2f3e 3c62 7220 2f3e 3c73 7562  ult"/><br /><sub
+00001e90: 3e3c 623e 5374 c3a9 7068 616e 6520 5261  ><b>St..phane Ra
+00001ea0: 696d 6261 756c 743c 2f62 3e3c 2f73 7562  imbault</b></sub
+00001eb0: 3e3c 2f61 3e3c 6272 202f 3e3c 6120 6872  ></a><br /><a hr
+00001ec0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00001ed0: 7562 2e63 6f6d 2f79 657a 7a31 3233 2f61  ub.com/yezz123/a
+00001ee0: 7574 6878 2f63 6f6d 6d69 7473 3f61 7574  uthx/commits?aut
+00001ef0: 686f 723d 7374 6570 6861 6e65 2220 7469  hor=stephane" ti
+00001f00: 746c 653d 2243 6f64 6522 3ef0 9f92 bb3c  tle="Code">....<
+00001f10: 2f61 3e20 3c61 2068 7265 663d 2223 706c  /a> <a href="#pl
+00001f20: 7567 696e 2d73 7465 7068 616e 6522 2074  ugin-stephane" t
+00001f30: 6974 6c65 3d22 506c 7567 696e 2f75 7469  itle="Plugin/uti
+00001f40: 6c69 7479 206c 6962 7261 7269 6573 223e  lity libraries">
+00001f50: f09f 948c 3c2f 613e 3c2f 7464 3e0a 2020  ....</a></td>.  
+00001f60: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
+00001f70: 0a20 2020 2020 203c 7464 2061 6c69 676e  .      <td align
+00001f80: 3d22 6365 6e74 6572 2220 7661 6c69 676e  ="center" valign
+00001f90: 3d22 746f 7022 2077 6964 7468 3d22 3134  ="top" width="14
+00001fa0: 2e32 3825 223e 3c61 2068 7265 663d 2268  .28%"><a href="h
+00001fb0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001fc0: 6d2f 7468 656f 6f68 6f68 6f22 3e3c 696d  m/theoohoho"><im
+00001fd0: 6720 7372 633d 2268 7474 7073 3a2f 2f61  g src="https://a
+00001fe0: 7661 7461 7273 2e67 6974 6875 6275 7365  vatars.githubuse
+00001ff0: 7263 6f6e 7465 6e74 2e63 6f6d 2f75 2f33  rcontent.com/u/3
+00002000: 3135 3337 3436 363f 763d 343f 733d 3130  1537466?v=4?s=10
+00002010: 3022 2077 6964 7468 3d22 3130 3070 783b  0" width="100px;
+00002020: 2220 616c 743d 2274 6865 6f6f 686f 686f  " alt="theoohoho
+00002030: 222f 3e3c 6272 202f 3e3c 7375 623e 3c62  "/><br /><sub><b
+00002040: 3e74 6865 6f6f 686f 686f 3c2f 623e 3c2f  >theoohoho</b></
+00002050: 7375 623e 3c2f 613e 3c62 7220 2f3e 3c61  sub></a><br /><a
+00002060: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00002070: 6974 6875 622e 636f 6d2f 7965 7a7a 3132  ithub.com/yezz12
+00002080: 332f 6175 7468 782f 636f 6d6d 6974 733f  3/authx/commits?
+00002090: 6175 7468 6f72 3d74 6865 6f6f 686f 686f  author=theoohoho
+000020a0: 2220 7469 746c 653d 2244 6f63 756d 656e  " title="Documen
+000020b0: 7461 7469 6f6e 223e f09f 9396 3c2f 613e  tation">....</a>
+000020c0: 3c2f 7464 3e0a 2020 2020 2020 3c74 6420  </td>.      <td 
+000020d0: 616c 6967 6e3d 2263 656e 7465 7222 2076  align="center" v
+000020e0: 616c 6967 6e3d 2274 6f70 2220 7769 6474  align="top" widt
+000020f0: 683d 2231 342e 3238 2522 3e3c 6120 6872  h="14.28%"><a hr
+00002100: 6566 3d22 6874 7470 733a 2f2f 796f 6765  ef="https://yoge
+00002110: 7368 7570 6164 6879 6179 2e6e 6574 6c69  shupadhyay.netli
+00002120: 6679 2e61 7070 2f22 3e3c 696d 6720 7372  fy.app/"><img sr
+00002130: 633d 2268 7474 7073 3a2f 2f61 7661 7461  c="https://avata
+00002140: 7273 2e67 6974 6875 6275 7365 7263 6f6e  rs.githubusercon
+00002150: 7465 6e74 2e63 6f6d 2f75 2f35 3339 3932  tent.com/u/53992
+00002160: 3136 383f 763d 343f 733d 3130 3022 2077  168?v=4?s=100" w
+00002170: 6964 7468 3d22 3130 3070 783b 2220 616c  idth="100px;" al
+00002180: 743d 2259 6f67 6573 6820 5570 6164 6879  t="Yogesh Upadhy
+00002190: 6179 222f 3e3c 6272 202f 3e3c 7375 623e  ay"/><br /><sub>
+000021a0: 3c62 3e59 6f67 6573 6820 5570 6164 6879  <b>Yogesh Upadhy
+000021b0: 6179 3c2f 623e 3c2f 7375 623e 3c2f 613e  ay</b></sub></a>
+000021c0: 3c62 7220 2f3e 3c61 2068 7265 663d 2268  <br /><a href="h
+000021d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000021e0: 6d2f 7965 7a7a 3132 332f 6175 7468 782f  m/yezz123/authx/
+000021f0: 6973 7375 6573 3f71 3d61 7574 686f 7225  issues?q=author%
+00002200: 3341 596f 6765 7368 5570 6468 7961 7922  3AYogeshUpdhyay"
+00002210: 2074 6974 6c65 3d22 4275 6720 7265 706f   title="Bug repo
+00002220: 7274 7322 3ef0 9f90 9b3c 2f61 3e3c 2f74  rts">....</a></t
+00002230: 643e 0a20 2020 2020 203c 7464 2061 6c69  d>.      <td ali
+00002240: 676e 3d22 6365 6e74 6572 2220 7661 6c69  gn="center" vali
+00002250: 676e 3d22 746f 7022 2077 6964 7468 3d22  gn="top" width="
+00002260: 3134 2e32 3825 223e 3c61 2068 7265 663d  14.28%"><a href=
+00002270: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00002280: 636f 6d2f 6966 7465 6e65 7422 3e3c 696d  com/iftenet"><im
+00002290: 6720 7372 633d 2268 7474 7073 3a2f 2f61  g src="https://a
+000022a0: 7661 7461 7273 2e67 6974 6875 6275 7365  vatars.githubuse
+000022b0: 7263 6f6e 7465 6e74 2e63 6f6d 2f75 2f31  rcontent.com/u/1
+000022c0: 3339 3738 3830 3f76 3d34 3f73 3d31 3030  397880?v=4?s=100
+000022d0: 2220 7769 6474 683d 2231 3030 7078 3b22  " width="100px;"
+000022e0: 2061 6c74 3d22 526f 6d61 6e22 2f3e 3c62   alt="Roman"/><b
+000022f0: 7220 2f3e 3c73 7562 3e3c 623e 526f 6d61  r /><sub><b>Roma
+00002300: 6e3c 2f62 3e3c 2f73 7562 3e3c 2f61 3e3c  n</b></sub></a><
+00002310: 6272 202f 3e3c 6120 6872 6566 3d22 6874  br /><a href="ht
+00002320: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002330: 2f79 657a 7a31 3233 2f61 7574 6878 2f69  /yezz123/authx/i
+00002340: 7373 7565 733f 713d 6175 7468 6f72 2533  ssues?q=author%3
+00002350: 4169 6674 656e 6574 2220 7469 746c 653d  Aiftenet" title=
+00002360: 2242 7567 2072 6570 6f72 7473 223e f09f  "Bug reports">..
+00002370: 909b 3c2f 613e 3c2f 7464 3e0a 2020 2020  ..</a></td>.    
+00002380: 2020 3c74 6420 616c 6967 6e3d 2263 656e    <td align="cen
+00002390: 7465 7222 2076 616c 6967 6e3d 2274 6f70  ter" valign="top
+000023a0: 2220 7769 6474 683d 2231 342e 3238 2522  " width="14.28%"
+000023b0: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+000023c0: 2f2f 7777 772e 6c69 6e6b 6564 696e 2e63  //www.linkedin.c
+000023d0: 6f6d 2f74 6f64 6179 2f61 7574 686f 722f  om/today/author/
+000023e0: 616c 6f62 6273 223e 3c69 6d67 2073 7263  alobbs"><img src
+000023f0: 3d22 6874 7470 733a 2f2f 6176 6174 6172  ="https://avatar
+00002400: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
+00002410: 656e 742e 636f 6d2f 752f 3137 3035 3539  ent.com/u/170559
+00002420: 3f76 3d34 3f73 3d31 3030 2220 7769 6474  ?v=4?s=100" widt
+00002430: 683d 2231 3030 7078 3b22 2061 6c74 3d22  h="100px;" alt="
+00002440: 416c 7661 726f 204c 6f70 657a 204f 7274  Alvaro Lopez Ort
+00002450: 6567 6122 2f3e 3c62 7220 2f3e 3c73 7562  ega"/><br /><sub
+00002460: 3e3c 623e 416c 7661 726f 204c 6f70 657a  ><b>Alvaro Lopez
+00002470: 204f 7274 6567 613c 2f62 3e3c 2f73 7562   Ortega</b></sub
+00002480: 3e3c 2f61 3e3c 6272 202f 3e3c 6120 6872  ></a><br /><a hr
+00002490: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000024a0: 7562 2e63 6f6d 2f79 657a 7a31 3233 2f61  ub.com/yezz123/a
+000024b0: 7574 6878 2f63 6f6d 6d69 7473 3f61 7574  uthx/commits?aut
+000024c0: 686f 723d 616c 6f62 6273 2220 7469 746c  hor=alobbs" titl
+000024d0: 653d 2244 6f63 756d 656e 7461 7469 6f6e  e="Documentation
+000024e0: 223e f09f 9396 3c2f 613e 3c2f 7464 3e0a  ">....</a></td>.
+000024f0: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
+00002500: 2263 656e 7465 7222 2076 616c 6967 6e3d  "center" valign=
+00002510: 2274 6f70 2220 7769 6474 683d 2231 342e  "top" width="14.
+00002520: 3238 2522 3e3c 6120 6872 6566 3d22 6874  28%"><a href="ht
+00002530: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002540: 2f70 696e 6368 584f 584f 223e 3c69 6d67  /pinchXOXO"><img
+00002550: 2073 7263 3d22 6874 7470 733a 2f2f 6176   src="https://av
+00002560: 6174 6172 732e 6769 7468 7562 7573 6572  atars.githubuser
+00002570: 636f 6e74 656e 742e 636f 6d2f 752f 3638  content.com/u/68
+00002580: 3530 3137 3939 3f76 3d34 3f73 3d31 3030  501799?v=4?s=100
+00002590: 2220 7769 6474 683d 2231 3030 7078 3b22  " width="100px;"
+000025a0: 2061 6c74 3d22 4465 7679 2053 616e 746f   alt="Devy Santo
+000025b0: 222f 3e3c 6272 202f 3e3c 7375 623e 3c62  "/><br /><sub><b
+000025c0: 3e44 6576 7920 5361 6e74 6f3c 2f62 3e3c  >Devy Santo</b><
+000025d0: 2f73 7562 3e3c 2f61 3e3c 6272 202f 3e3c  /sub></a><br /><
+000025e0: 6120 6872 6566 3d22 2369 6e66 7261 2d70  a href="#infra-p
+000025f0: 696e 6368 584f 584f 2220 7469 746c 653d  inchXOXO" title=
+00002600: 2249 6e66 7261 7374 7275 6374 7572 6520  "Infrastructure 
+00002610: 2848 6f73 7469 6e67 2c20 4275 696c 642d  (Hosting, Build-
+00002620: 546f 6f6c 732c 2065 7463 2922 3ef0 9f9a  Tools, etc)">...
+00002630: 873c 2f61 3e3c 2f74 643e 0a20 2020 203c  .</a></td>.    <
+00002640: 2f74 723e 0a20 203c 2f74 626f 6479 3e0a  /tr>.  </tbody>.
+00002650: 3c2f 7461 626c 653e 0a0a 3c21 2d2d 206d  </table>..<!-- m
+00002660: 6172 6b64 6f77 6e6c 696e 742d 7265 7374  arkdownlint-rest
+00002670: 6f72 6520 2d2d 3e0a 3c21 2d2d 2070 7265  ore -->.<!-- pre
+00002680: 7474 6965 722d 6967 6e6f 7265 2d65 6e64  ttier-ignore-end
+00002690: 202d 2d3e 0a0a 3c21 2d2d 2041 4c4c 2d43   -->..<!-- ALL-C
+000026a0: 4f4e 5452 4942 5554 4f52 532d 4c49 5354  ONTRIBUTORS-LIST
+000026b0: 3a45 4e44 202d 2d3e 0a0a 3c21 2d2d 2041  :END -->..<!-- A
+000026c0: 4c4c 2d43 4f4e 5452 4942 5554 4f52 532d  LL-CONTRIBUTORS-
+000026d0: 4c49 5354 3a53 5441 5254 202d 2044 6f20  LIST:START - Do 
+000026e0: 6e6f 7420 7265 6d6f 7665 206f 7220 6d6f  not remove or mo
+000026f0: 6469 6679 2074 6869 7320 7365 6374 696f  dify this sectio
+00002700: 6e20 2d2d 3e0a 3c21 2d2d 2070 7265 7474  n -->.<!-- prett
+00002710: 6965 722d 6967 6e6f 7265 2d73 7461 7274  ier-ignore-start
+00002720: 202d 2d3e 0a3c 212d 2d20 6d61 726b 646f   -->.<!-- markdo
+00002730: 776e 6c69 6e74 2d64 6973 6162 6c65 202d  wnlint-disable -
+00002740: 2d3e 0a0a 3c21 2d2d 206d 6172 6b64 6f77  ->..<!-- markdow
+00002750: 6e6c 696e 742d 7265 7374 6f72 6520 2d2d  nlint-restore --
+00002760: 3e0a 3c21 2d2d 2070 7265 7474 6965 722d  >.<!-- prettier-
+00002770: 6967 6e6f 7265 2d65 6e64 202d 2d3e 0a0a  ignore-end -->..
+00002780: 3c21 2d2d 2041 4c4c 2d43 4f4e 5452 4942  <!-- ALL-CONTRIB
+00002790: 5554 4f52 532d 4c49 5354 3a45 4e44 202d  UTORS-LIST:END -
+000027a0: 2d3e 0a0a 5468 6973 2070 726f 6a65 6374  ->..This project
+000027b0: 2066 6f6c 6c6f 7773 2074 6865 0a5b 616c   follows the.[al
+000027c0: 6c2d 636f 6e74 7269 6275 746f 7273 5d28  l-contributors](
+000027d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000027e0: 6f6d 2f61 6c6c 2d63 6f6e 7472 6962 7574  om/all-contribut
+000027f0: 6f72 732f 616c 6c2d 636f 6e74 7269 6275  ors/all-contribu
+00002800: 746f 7273 290a 7370 6563 6966 6963 6174  tors).specificat
+00002810: 696f 6e2e 2043 6f6e 7472 6962 7574 696f  ion. Contributio
+00002820: 6e73 206f 6620 616e 7920 6b69 6e64 2077  ns of any kind w
+00002830: 656c 636f 6d65 210a 0a23 2320 4c69 6365  elcome!..## Lice
+00002840: 6e73 650a 0a54 6869 7320 7072 6f6a 6563  nse..This projec
+00002850: 7420 6973 206c 6963 656e 7365 6420 756e  t is licensed un
+00002860: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
+00002870: 2074 6865 204d 4954 204c 6963 656e 7365   the MIT License
+00002880: 2e0a                                     ..
```

### Comparing `authx-1.1.1/pyproject.toml` & `authx-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `authx-1.1.1/PKG-INFO` & `authx-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: authx
-Version: 1.1.1
+Version: 1.1.2
 Summary: Ready to use and customizable Authentications and Oauth2 management for FastAPI
 Project-URL: Homepage, https://github.com/yezz123/authx
 Project-URL: Documentation, https://authx.yezz.me/
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
@@ -45,35 +45,25 @@
 <p align="center">
 <a href="https://authx.yezz.me" target="_blank">
     <img src="https://user-images.githubusercontent.com/52716203/136962014-280d82b0-0640-4ee5-9a11-b451b338f6d8.png" alt="AuthX">
 </a>
 <p align="center">
     <em>Ready-to-use and customizable Authentications and Oauth2 management for FastAPI ⚡</em>
 </p>
-<p align="center">
-<a href="https://github.com/yezz123/authx/actions/workflows/ci.yml" target="_blank">
-    <img src="https://github.com/yezz123/authx/actions/workflows/ci.yml/badge.svg" alt="lint">
-</a>
-<a href="https://pypi.org/project/authx" target="_blank">
-    <img src="https://img.shields.io/pypi/v/authx?color=%2334D058&label=pypi%20package" alt="Package version">
-</a>
-<a href="https://codecov.io/gh/yezz123/authx">
-    <img src="https://codecov.io/gh/yezz123/authx/branch/main/graph/badge.svg"/>
-</a>
-<a href="https://pepy.tech/project/authx" target="_blank">
-    <img src="https://static.pepy.tech/badge/authx" alt="Test">
-</a>
-<a href="https://pydantic.dev" target="_blank">
-    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json" alt="Pydantic Version 2">
-</a>
-</p>
 </p>
 
 ---
 
+| Project | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+|---------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CI      | [ ![ CI ]( https://github.com/yezz123/authx/actions/workflows/ci.yml/badge.svg ) ]( https://github.com/yezz123/authx/actions/workflows/ci.yml )  [ ![ pre-commit.ci status ]( https://results.pre-commit.ci/badge/github/yezz123/authx/main.svg )   ]( https://results.pre-commit.ci/latest/github/yezz123/authx/main )  [ ![ Codecov ]( https://codecov.io/gh/yezz123/authx/branch/main/graph/badge.svg )   ]( https://codecov.io/gh/yezz123/authx ) |
+| Meta    | [ ![ Package version ]( https://img.shields.io/pypi/v/authx?color=%2334D058&label=pypi%20package )   ]( https://pypi.org/project/authx )  [ ![ Downloads ]( https://static.pepy.tech/badge/authx )   ]( https://pepy.tech/project/authx )  [ ![ Pydantic Version 2 ]( https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json )   ]( https://pydantic.dev )  [ ![ Ruff ]( https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json ) ]( https://github.com/astral-sh/ruff )                                                                                                                                                 |
+
+---
+
 **Source Code**: <https://github.com/yezz123/authx>
 
 **Documentation**: <https://authx.yezz.me/>
 
 ---
 
 Add a Fully registration and authentication or authorization system to your
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: authx Version: 1.1.1 Summary: Ready to use and
+Metadata-Version: 2.3 Name: authx Version: 1.1.2 Summary: Ready to use and
 customizable Authentications and Oauth2 management for FastAPI Project-URL:
 Homepage, https://github.com/yezz123/authx Project-URL: Documentation, https://
 authx.yezz.me/ Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri
 yezz.me> License-Expression: MIT License-File: LICENSE Keywords:
 Authentication,Cookie,FastAPI,JWT,Oauth2,Pydantic Classifier: Development
 Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier: Framework ::
@@ -22,17 +22,36 @@
 Dist: pydantic<3.0.0,>=2.0.0 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.6.0
 Requires-Dist: python-dateutil<3.0.0,>=2.8 Requires-Dist: python-
 jose<4.0.0,>=3.3.0 Requires-Dist: pytz<2025.0,>=2023.3 Description-Content-
 Type: text/markdown # Authx
                                     _[_A_u_t_h_X_]
 RReeaaddyy--ttoo--uussee aanndd ccuussttoommiizzaabbllee AAuutthheennttiiccaattiioonnss aanndd OOaauutthh22 mmaannaaggeemmeenntt ffoorr FFaassttAAPPII
                                       ?â??¡
-_[_l_i_n_t_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_y_e_z_z_1_2_3_/_a_u_t_h_x_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
-                     _b_a_d_g_e_._s_v_g_]_[_T_e_s_t_]_[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _2_]
---- **Source Code**:
+--- | Project | Status | |---------|-------------------------------------------
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+------------------------------------------------------------| | CI | [ ![ CI ]
+( https://github.com/yezz123/authx/actions/workflows/ci.yml/badge.svg ) ]
+( https://github.com/yezz123/authx/actions/workflows/ci.yml ) [ ![ pre-
+commit.ci status ]( https://results.pre-commit.ci/badge/github/yezz123/authx/
+main.svg ) ]( https://results.pre-commit.ci/latest/github/yezz123/authx/main )
+[ ![ Codecov ]( https://codecov.io/gh/yezz123/authx/branch/main/graph/badge.svg
+) ]( https://codecov.io/gh/yezz123/authx ) | | Meta | [ ![ Package version ]
+( https://img.shields.io/pypi/v/authx?color=%2334D058&label=pypi%20package ) ]
+( https://pypi.org/project/authx ) [ ![ Downloads ]( https://static.pepy.tech/
+badge/authx ) ]( https://pepy.tech/project/authx ) [ ![ Pydantic Version 2 ]
+( https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/
+pydantic/pydantic/main/docs/badge/v2.json ) ]( https://pydantic.dev ) [ ![ Ruff
+]( https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/
+astral-sh/ruff/main/assets/badge/v2.json ) ]( https://github.com/astral-sh/ruff
+) | --- **Source Code**:
 github.com/yezz123/authx> **Documentation**:
 authx.yezz.me/> --- Add a Fully registration and authentication or
 authorization system to your [FastAPI](https://fastapi.tiangolo.com/) project.
 **AuthX** is designed to be as customizable and adaptable as possible. ##
 Features - [x] Support Python 3.8+ & Pydantic 2.0+. - [x] Multiple customizable
 authentication backend: - [x] JWT authentication backend included - [x] JWT
 encoding/decoding for application authentication - [x] Automatic detection of
```

