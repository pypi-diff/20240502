# Comparing `tmp/pydantic_forms-1.0.2.tar.gz` & `tmp/pydantic_forms-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_forms-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pydantic_forms-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pydantic_forms-1.0.2.tar` & `pydantic_forms-1.0.3.tar`

### file list

```diff
@@ -1,66 +1,69 @@
--rw-r--r--   0        0        0      345 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/.bumpversion.cfg
--rw-r--r--   0        0        0       24 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/.coveragerc
--rw-r--r--   0        0        0      502 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/.github/workflows/dependabot.yml
--rw-r--r--   0        0        0      550 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/.github/workflows/publish-release.yaml
--rw-r--r--   0        0        0      385 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1101 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     1464 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1782 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/.gitignore
--rw-r--r--   0        0        0     1581 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1283 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/.stignore
--rw-r--r--   0        0        0     3141 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/README.md
--rw-r--r--   0        0        0      636 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/__init__.py
--rw-r--r--   0        0        0      896 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/core/__init__.py
--rw-r--r--   0        0        0     4943 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/core/asynchronous.py
--rw-r--r--   0        0        0     2372 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/core/shared.py
--rw-r--r--   0        0        0     4774 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/core/sync.py
--rw-r--r--   0        0        0        0 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/exception_handlers/__init__.py
--rw-r--r--   0        0        0     2367 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/exception_handlers/fastapi.py
--rw-r--r--   0        0        0     3236 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/py.typed
--rw-r--r--   0        0        0     1914 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/types.py
--rw-r--r--   0        0        0        0 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/utils/__init__.py
--rw-r--r--   0        0        0     8835 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/utils/json.py
--rw-r--r--   0        0        0     1679 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/validators/__init__.py
--rw-r--r--   0        0        0        0 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/validators/components/__init__.py
--rw-r--r--   0        0        0     2059 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/validators/components/accept.py
--rw-r--r--   0        0        0     2495 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/validators/components/choice.py
--rw-r--r--   0        0        0     1579 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/validators/components/choice_list.py
--rw-r--r--   0        0        0      845 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/validators/components/contact_person.py
--rw-r--r--   0        0        0     1844 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/validators/components/contact_person_list.py
--rw-r--r--   0        0        0      882 2024-02-19 12:24:10.829145 pydantic_forms-1.0.2/pydantic_forms/validators/components/display_subscription.py
--rw-r--r--   0        0        0      759 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/components/divider.py
--rw-r--r--   0        0        0      755 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/components/label.py
--rw-r--r--   0        0        0      772 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/components/list_of_one.py
--rw-r--r--   0        0        0      904 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/components/list_of_two.py
--rw-r--r--   0        0        0      700 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/components/long_text.py
--rw-r--r--   0        0        0     1707 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/components/migration_summary.py
--rw-r--r--   0        0        0      816 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/components/organisation_id.py
--rw-r--r--   0        0        0     2839 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/components/read_only_field.py
--rw-r--r--   0        0        0     1402 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/components/timestamp.py
--rw-r--r--   0        0        0     1382 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/components/unique_constrained_list.py
--rw-r--r--   0        0        0      481 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pydantic_forms/validators/helpers.py
--rw-r--r--   0        0        0     3641 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1744 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/setup.cfg
--rw-r--r--   0        0        0      660 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/setup.py
--rw-r--r--   0        0        0        0 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/exception_handlers/__init__.py
--rw-r--r--   0        0        0     1648 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/exception_handlers/test_fastapi.py
--rw-r--r--   0        0        0     2640 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_accept.py
--rw-r--r--   0        0        0     3339 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_choice.py
--rw-r--r--   0        0        0     4518 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_choice_list.py
--rw-r--r--   0        0        0     4635 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_constrained_list.py
--rw-r--r--   0        0        0     1095 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_contact_person.py
--rw-r--r--   0        0        0     4572 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_contact_person_list.py
--rw-r--r--   0        0        0     6944 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_core.py
--rw-r--r--   0        0        0     6467 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_core_async.py
--rw-r--r--   0        0        0     1742 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_display_subscription.py
--rw-r--r--   0        0        0      338 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_divider.py
--rw-r--r--   0        0        0      338 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_label.py
--rw-r--r--   0        0        0     1223 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_list_of_one.py
--rw-r--r--   0        0        0     2217 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_list_of_two.py
--rw-r--r--   0        0        0      471 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_long_text.py
--rw-r--r--   0        0        0     1285 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_migration_summary.py
--rw-r--r--   0        0        0      572 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_organisation_id.py
--rw-r--r--   0        0        0     5605 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_read_only_field.py
--rw-r--r--   0        0        0     1427 2024-02-19 12:24:10.833145 pydantic_forms-1.0.2/tests/unit_tests/test_timestamp.py
--rw-r--r--   0        0        0     6519 1970-01-01 00:00:00.000000 pydantic_forms-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      345 2024-05-02 11:24:08.396393 pydantic_forms-1.0.3/.bumpversion.cfg
+-rw-r--r--   0        0        0       44 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/.coveragerc
+-rw-r--r--   0        0        0      502 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      550 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/.github/workflows/publish-release.yaml
+-rw-r--r--   0        0        0      384 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1107 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     1612 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1782 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1581 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1283 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/.stignore
+-rw-r--r--   0        0        0     3427 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/README.md
+-rw-r--r--   0        0        0       19 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/codecov.yml
+-rw-r--r--   0        0        0      624 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/__init__.py
+-rw-r--r--   0        0        0      896 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/core/__init__.py
+-rw-r--r--   0        0        0     5010 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/core/asynchronous.py
+-rw-r--r--   0        0        0     2372 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/core/shared.py
+-rw-r--r--   0        0        0     4825 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/core/sync.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/exception_handlers/__init__.py
+-rw-r--r--   0        0        0     2419 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/exception_handlers/fastapi.py
+-rw-r--r--   0        0        0     3328 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/py.typed
+-rw-r--r--   0        0        0     1914 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/types.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/utils/__init__.py
+-rw-r--r--   0        0        0     8943 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/utils/json.py
+-rw-r--r--   0        0        0     1713 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/__init__.py
+-rw-r--r--   0        0        0     2062 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/accept.py
+-rw-r--r--   0        0        0     2495 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/choice.py
+-rw-r--r--   0        0        0     1579 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/choice_list.py
+-rw-r--r--   0        0        0      845 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/contact_person.py
+-rw-r--r--   0        0        0     1844 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/contact_person_list.py
+-rw-r--r--   0        0        0      882 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/display_subscription.py
+-rw-r--r--   0        0        0      759 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/divider.py
+-rw-r--r--   0        0        0      755 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/label.py
+-rw-r--r--   0        0        0      772 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/list_of_one.py
+-rw-r--r--   0        0        0      904 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/list_of_two.py
+-rw-r--r--   0        0        0      700 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/long_text.py
+-rw-r--r--   0        0        0     1707 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/migration_summary.py
+-rw-r--r--   0        0        0      816 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/organisation_id.py
+-rw-r--r--   0        0        0     2839 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/read_only_field.py
+-rw-r--r--   0        0        0     1402 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/timestamp.py
+-rw-r--r--   0        0        0     1382 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/components/unique_constrained_list.py
+-rw-r--r--   0        0        0      494 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pydantic_forms/validators/helpers.py
+-rw-r--r--   0        0        0     3685 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1744 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/setup.cfg
+-rw-r--r--   0        0        0      660 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/setup.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/tests/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/tests/unit_tests/exception_handlers/__init__.py
+-rw-r--r--   0        0        0     1648 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/tests/unit_tests/exception_handlers/test_fastapi.py
+-rw-r--r--   0        0        0     2617 2024-05-02 11:24:08.400393 pydantic_forms-1.0.3/tests/unit_tests/test_accept.py
+-rw-r--r--   0        0        0     3339 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_choice.py
+-rw-r--r--   0        0        0     4518 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_choice_list.py
+-rw-r--r--   0        0        0     4635 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_constrained_list.py
+-rw-r--r--   0        0        0     1095 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_contact_person.py
+-rw-r--r--   0        0        0     4572 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_contact_person_list.py
+-rw-r--r--   0        0        0     6944 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_core.py
+-rw-r--r--   0        0        0     6467 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_core_async.py
+-rw-r--r--   0        0        0     1742 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_display_subscription.py
+-rw-r--r--   0        0        0      338 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_divider.py
+-rw-r--r--   0        0        0      338 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_label.py
+-rw-r--r--   0        0        0     1223 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_list_of_one.py
+-rw-r--r--   0        0        0     2217 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_list_of_two.py
+-rw-r--r--   0        0        0      471 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_long_text.py
+-rw-r--r--   0        0        0     1285 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_migration_summary.py
+-rw-r--r--   0        0        0      572 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_organisation_id.py
+-rw-r--r--   0        0        0     5605 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_read_only_field.py
+-rw-r--r--   0        0        0     1427 2024-05-02 11:24:08.404393 pydantic_forms-1.0.3/tests/unit_tests/test_timestamp.py
+-rw-r--r--   0        0        0     6824 1970-01-01 00:00:00.000000 pydantic_forms-1.0.3/PKG-INFO
```

### Comparing `pydantic_forms-1.0.2/.github/workflows/publish-release.yaml` & `pydantic_forms-1.0.3/.github/workflows/publish-release.yaml`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/.github/workflows/run-linting-tests.yml` & `pydantic_forms-1.0.3/.github/workflows/run-linting-tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,11 +30,11 @@
           pip install flit
           flit install --deps develop --extras fastapi
       - name: Check formatting
         run: |
           python -V | grep 10 || black --check .
       - name: Lint with ruff
         run: |
-          ruff .
+          ruff check .
       - name: Check with mypy
         run: |
           mypy pydantic_forms
```

### Comparing `pydantic_forms-1.0.2/.github/workflows/run-unit-tests.yml` & `pydantic_forms-1.0.3/.github/workflows/run-unit-tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 jobs:
   container_job:
     name: Unit tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ['3.9', '3.10', '3.11', '3.12']
-        pydantic-version: ['2.5.2', 'lockfile']
+        pydantic-version: ['lockfile']
         fastapi-version: ['0.103.2', 'lockfile']
       fail-fast: false
     container: python:${{ matrix.python-version }}-slim
     steps:
       # Downloads a copy of the code in your repository before running CI tests
       - name: Check out repository code
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: Install dependencies
         run: |
           apt update
           apt install curl git build-essential libpq-dev libffi-dev -y
           python -m pip install --upgrade pip
           pip install flit
           flit install --deps develop
@@ -32,13 +32,16 @@
             pip install fastapi~=${{ matrix.fastapi-version }}
           else
             flit install --extras fastapi
           fi
         env:
           FLIT_ROOT_INSTALL: 1
       - name: Run Unit tests
-        run: pytest --cov-branch --cov=pydantic_forms --cov-report=xml
-#      - name: "Upload coverage to Codecov"
-#        uses: codecov/codecov-action@v2
-#        with:
-#          fail_ci_if_error: true
-#          files: ./coverage.xml
+        run: pytest tests/unit_tests --cov-branch --cov=pydantic_forms --ignore=tests --cov-report=xml
+        env:
+          COVERAGE_FILE: reports/.coverage.${{ matrix.python-version }}
+      - name: "Upload coverage to Codecov"
+        uses: codecov/codecov-action@v3
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          fail_ci_if_error: true
+          files: ./coverage.xml
```

### Comparing `pydantic_forms-1.0.2/.gitignore` & `pydantic_forms-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/.pre-commit-config.yaml` & `pydantic_forms-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/.stignore` & `pydantic_forms-1.0.3/.stignore`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/README.md` & `pydantic_forms-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Pydantic forms
 
 [![pypi_version](https://img.shields.io/pypi/v/pydantic-forms?color=%2334D058&label=pypi%20package)](https://pypi.org/project/pydantic-forms)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/pydantic-forms.svg?color=%2334D058)](https://pypi.org/project/pydantic-forms)
+[![Downloads](https://static.pepy.tech/badge/pydantic-forms/month)](https://pepy.tech/project/pydantic-forms)
+[![codecov](https://codecov.io/gh/workfloworchestrator/pydantic-forms/branch/main/graph/badge.svg?token=AJMOSWPHQX)](https://codecov.io/gh/workfloworchestrator/pydantic-forms)
 
 A Python package that lets you add smart forms to [FastAPI](https://fastapi.tiangolo.com/)
 and [Flask](https://palletsprojects.com/p/flask/). Forms will respond with a JSON scheme that
 contains all info needed in a React frontend with uniforms to render the forms and handle all validation tasks.
 
 Forms can also consist out of a wizard, so you can create complex form flows consisting out of multiple
 consecutive forms. The forms and the validation logic are defined by
```

### Comparing `pydantic_forms-1.0.2/pydantic_forms/__init__.py` & `pydantic_forms-1.0.3/pydantic_forms/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""This is the pydantic-forms engine."""
+"""Pydantic-forms engine."""
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
```

### Comparing `pydantic_forms-1.0.2/pydantic_forms/core/__init__.py` & `pydantic_forms-1.0.3/pydantic_forms/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/core/asynchronous.py` & `pydantic_forms-1.0.3/pydantic_forms/core/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     if isinstance(generated_form, dict):
         # Check whether the result was yielded. (AsyncGenerator can only yield, not return)
         # This is a downside of using AsyncGenerator; we cannot enforce the last returned item
         # to be of `State`
         return generated_form
 
     # Form is not completely filled raise next form
-    raise FormNotCompleteError(generated_form.model_json_schema())
+    raise FormNotCompleteError(generated_form.model_json_schema(), meta=getattr(generated_form, "meta__", None))
 
 
 def _get_form(key: str) -> StateInputFormGeneratorAsync:
     if not (func := FORMS.get(key)):
         raise FormException(f"Form {key} does not exist.")
 
     if not isasyncgenfunction(func):
@@ -103,20 +103,22 @@
     user_inputs: Union[list[State], None] = None,
     user: str = "Just a user",  # Todo: check if we need users inside form logic?
     **extra_state: Any,
 ) -> State:
     """Handle the logic for the endpoint that the frontend uses to render a form with or without prefilled input.
 
     Args:
+    ----
         form_key: name of form in the FORM dict
         user_inputs: List of form inputs from frontend
         user: User who starts this form
         extra_state: Optional initial state variables
 
     Returns:
+    -------
         The data that the user entered into the form
 
     """
     if user_inputs is None:
         # Ensure the first FormNotComplete is raised from Swagger when a POST is done without user_inputs:
         user_inputs = []
```

### Comparing `pydantic_forms-1.0.2/pydantic_forms/core/shared.py` & `pydantic_forms-1.0.3/pydantic_forms/core/shared.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/core/sync.py` & `pydantic_forms-1.0.3/pydantic_forms/core/sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,24 +61,24 @@
         # Loop through user inputs and for each input validate and update current state and validation results
         while user_inputs:
             user_input = user_inputs.pop(0)
             # Validate
             try:
                 form_validated_data = generated_form(**user_input)
             except ValidationError as e:
-                raise FormValidationError(generated_form.__name__, e) from e  # type: ignore
+                raise FormValidationError(generated_form.__name__, e) from e
 
             # Update state with validated_data
             current_state.update(form_validated_data.model_dump())
 
             # Make next form or trigger StopIteration
             generated_form = generator.send(form_validated_data)
 
         # Form is not completely filled; raise next form
-        raise FormNotCompleteError(generated_form.model_json_schema())
+        raise FormNotCompleteError(generated_form.model_json_schema(), meta=getattr(generated_form, "meta__", None))
     except StopIteration as e:
         if user_inputs:
             raise FormOverflowError(f"Did not process all user_inputs ({len(user_inputs)} remaining)")
 
         # Form is completely filled, so we can return the last of the data and
         return e.value
 
@@ -98,20 +98,22 @@
     user_inputs: Union[list[State], None] = None,
     user: str = "Just a user",  # Todo: check if we need users inside form logic?
     **extra_state: dict[str, Any],
 ) -> State:
     """Handle the logic for the endpoint that the frontend uses to render a form with or without prefilled input.
 
     Args:
+    ----
         form_key: name of form in the FORM dict
         user_inputs: List of form inputs from frontend
         user: User who starts this form
         extra_state: Optional initial state variables
 
     Returns:
+    -------
         The data that the user entered into the form
 
     """
     if user_inputs is None:
         # Ensure the first FormNotComplete is raised from Swagger when a POST is done without user_inputs:
         user_inputs = []
```

### Comparing `pydantic_forms-1.0.2/pydantic_forms/exception_handlers/fastapi.py` & `pydantic_forms-1.0.3/pydantic_forms/exception_handlers/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
                 "type": type(exc).__name__,
                 "detail": str(exc),
                 "traceback": show_ex(exc),
                 # We need to make sure the is nothing the default json.dumps cannot handle
                 "form": json_loads(json_dumps(exc.form)),
                 "title": "Form not complete",
                 "status": HTTPStatus.NOT_EXTENDED,
+                "meta": getattr(exc, "meta", None),
             },
             status_code=HTTPStatus.NOT_EXTENDED,
         )
 
     return JSONResponse(
         {
             "detail": str(exc),
```

### Comparing `pydantic_forms-1.0.2/pydantic_forms/exceptions.py` & `pydantic_forms-1.0.3/pydantic_forms/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import traceback
-from typing import Any, Iterable, TypedDict, Union, cast
+from typing import Any, Iterable, Optional, TypedDict, Union, cast
 
 from more_itertools import side_effect
 from pydantic import ValidationError
 from pydantic_core import ErrorDetails
 
 from pydantic_forms.types import JSON
 
@@ -15,18 +15,20 @@
 class FormNotCompleteError(FormException):
     """Raised when fewer inputs are provided than the form can process.
 
     This exception is part of the normal forms workflow.
     """
 
     form: JSON
+    meta: Optional[JSON]
 
-    def __init__(self, form: JSON):
+    def __init__(self, form: JSON, *, meta: Optional[JSON] = None):
         super().__init__(form)
         self.form = form
+        self.meta = meta
 
 
 class FormOverflowError(FormException):
     """Raised when more inputs are provided than the form can process."""
 
 
 def convert_errors(validation_error: ValidationError) -> Iterable[ErrorDetails]:
```

### Comparing `pydantic_forms-1.0.2/pydantic_forms/types.py` & `pydantic_forms-1.0.3/pydantic_forms/types.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/utils/json.py` & `pydantic_forms-1.0.3/pydantic_forms/utils/json.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,20 +102,23 @@
 logger = structlog.get_logger(__name__)
 
 
 def to_serializable(o: Any) -> Any:
     """Convert an object into an object that the JSON encode can serialize.
 
     Args:
+    ----
         o: Object to convert.
 
     Returns:
+    -------
         Serializable object.
 
     Raises:
+    ------
         TypeError: in case no conversion was possible.
 
     """
     if isinstance(o, UUID):
         return str(o)
     if (
         isinstance(o, IPv4Address)
@@ -146,17 +149,19 @@
 UUID_PATTERN = re.compile(r"^[\da-f]{8}-([\da-f]{4}-){3}[\da-f]{12}$", re.IGNORECASE)
 
 
 def from_serializable(dct: dict[str, Any]) -> dict[str, Any]:
     """Convert a serializable object into a more specific, custom, Python data type.
 
     Args:
+    ----
         dct: Serializable object.
 
     Returns:
+    -------
         Either the serializable object itself or a more specific data type if a conversion was possible.
 
     """
     for k, v in dct.items():
         # We don't want to try converting each string we come across to a `datetime` object, hence we employ a simple
         # and reasonably specific heuristic that identifies likely ISO formatted string candidates
         if isinstance(v, str) and len(v) == ISO_FORMAT_STR_LEN and v[10] == "T":
@@ -194,32 +199,37 @@
 
 def non_none_dict(dikt: Sequence[tuple[str, Any]]) -> dict[Any, Any]:
     """Return no `None` values in a Dict.
 
     This function may be used in the `asdict()` method as dictionary factory.
 
     Args:
+    ----
         dikt: Tuple of values where
 
     Returns:
+    -------
         dict of the keys and values if value is not None
 
     Examples:
+    --------
         >>> non_none_dict({"a": 0, "b": None, "c": ""}.items())
         {'a': 0, 'c': ''}
 
     """
     return {k: v for k, v in dikt if v is not None}
 
 
 def isoformat(dt: datetime) -> str:
     """ISO format datetime object with max precision limited to seconds.
 
     Args:
+    ----
         dt: datatime object to be formatted
 
     Returns:
+    -------
         ISO 8601 formatted string
 
     """
     # IMPORTANT should the format be ever changed, be sure to update TIMESTAMP_REGEX as well!
     return dt.isoformat(timespec="seconds")
```

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/__init__.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pydantic_forms.validators.components.accept import Accept
+from pydantic_forms.validators.components.accept import Accept, AcceptValues
 from pydantic_forms.validators.components.choice import Choice
 from pydantic_forms.validators.components.choice_list import choice_list
 from pydantic_forms.validators.components.contact_person import ContactPerson, ContactPersonName
 from pydantic_forms.validators.components.contact_person_list import contact_person_list
 from pydantic_forms.validators.components.display_subscription import DisplaySubscription
 from pydantic_forms.validators.components.divider import Divider
 from pydantic_forms.validators.components.label import Label
@@ -13,14 +13,15 @@
 from pydantic_forms.validators.components.organisation_id import OrganisationId
 from pydantic_forms.validators.components.read_only_field import ReadOnlyField
 from pydantic_forms.validators.components.timestamp import Timestamp, timestamp
 from pydantic_forms.validators.components.unique_constrained_list import unique_conlist, validate_unique_list
 
 __all__ = (
     "Accept",
+    "AcceptValues",
     "Choice",
     "choice_list",
     "contact_person_list",
     "ContactPerson",
     "ContactPersonName",
     "DisplaySubscription",
     "Divider",
```

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/accept.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/accept.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 
 from pydantic import GetCoreSchemaHandler, GetJsonSchemaHandler, TypeAdapter
 from pydantic_core import CoreSchema, core_schema
 
 from pydantic_forms.types import AcceptData, strEnum
 
 
+class AcceptValues(strEnum):
+    ACCEPTED = "ACCEPTED"
+    INCOMPLETE = "INCOMPLETE"
+
+
 class Accept(str):
     data: ClassVar[Optional[AcceptData]] = None
 
-    class Values(strEnum):
-        ACCEPTED = "ACCEPTED"
-        INCOMPLETE = "INCOMPLETE"
-
-    _enum_adapter = TypeAdapter(Values)
+    _enum_adapter = TypeAdapter(AcceptValues)
 
     @classmethod
     def __get_pydantic_json_schema__(cls, core_schema: CoreSchema, handler: GetJsonSchemaHandler) -> dict[str, Any]:
         json_schema = handler.resolve_ref_schema(core_schema["schema"])
         return (
             json_schema
-            | {"format": "accept", "type": "string", "enum": list(cls.Values)}
+            | {"format": "accept", "type": "string", "enum": list(AcceptValues)}
             | ({"data": cls.data} if cls.data else {})
         )
 
     @classmethod
     def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
         return core_schema.no_info_after_validator_function(cls._validate, handler(str))
```

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/choice.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/choice.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/choice_list.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/choice_list.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/contact_person.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/contact_person.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/contact_person_list.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/contact_person_list.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/display_subscription.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/display_subscription.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/divider.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/divider.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/label.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/label.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/list_of_one.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/list_of_one.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/list_of_two.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/list_of_two.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/long_text.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/long_text.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/migration_summary.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/migration_summary.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/organisation_id.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/organisation_id.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/read_only_field.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/read_only_field.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/timestamp.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/timestamp.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pydantic_forms/validators/components/unique_constrained_list.py` & `pydantic_forms-1.0.3/pydantic_forms/validators/components/unique_constrained_list.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/pyproject.toml` & `pydantic_forms-1.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 requires = [
     "more-itertools",
-    "pydantic[email] >= 2.5.1",
+    "pydantic[email] ~= 2.5.1",
+    "pydantic~=2.5.1"
 ]
 description-file = "README.md"
 requires-python = ">=3.9,<=3.13"
 
 [tool.flit.metadata.urls]
 Documentation = "https://github.com/workfloworchestrator/pydantic-forms/blob/main/README.md"
 
@@ -122,16 +123,17 @@
     ".eggs",
     "__pycache__",
     "dist",
     "src",
     "venv",
     ".venv",
     "docs",
+    "tests"
 ]
-ignore = [
+lint.ignore = [
     "C417",
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
     "D105",
@@ -145,21 +147,21 @@
     "B904",
     "N803",
     "N801",
     "N815",
     "N802",
 ]
 line-length = 120
-select = ["B", "C", "D", "E", "F", "I", "N", "RET", "S", "T", "W"]
+lint.select = ["B", "C", "D", "E", "F", "I", "N", "RET", "S", "T", "W"]
 target-version = "py39"
 
-[tool.ruff.flake8-tidy-imports]
+[tool.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.lint.per-file-ignores]
 "tests/*" = ["S101", "B033", "N816", "N802"]
 
-[tool.ruff.pydocstyle]
+[tool.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.isort]
+[tool.lint.isort]
 known-third-party = ["pydantic"]
```

### Comparing `pydantic_forms-1.0.2/setup.cfg` & `pydantic_forms-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/setup.py` & `pydantic_forms-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/exception_handlers/test_fastapi.py` & `pydantic_forms-1.0.3/tests/unit_tests/exception_handlers/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_accept.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_accept.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from unittest.mock import ANY
+
 from pydantic_core import ValidationError
 from pytest import raises
 
 from pydantic_forms.core import FormPage
 from pydantic_forms.utils.json import json_loads
-from pydantic_forms.validators import Accept
+from pydantic_forms.validators import Accept, AcceptValues
 
 
 def test_accept_ok():
     class Form(FormPage):
         accept: Accept
 
     validated_data = Form(accept="ACCEPTED").model_dump_json()
@@ -20,25 +22,26 @@
     class Form(FormPage):
         accept: Accept
 
     expected = {
         "additionalProperties": False,
         "properties": {
             "accept": {
-                "enum": ["ACCEPTED", "INCOMPLETE"],
+                "enum": [AcceptValues.ACCEPTED, AcceptValues.INCOMPLETE],
                 "format": "accept",
-                "metadata": {"pydantic.internal.needs_apply_discriminated_union": False},
                 "type": "string",
                 "title": "Accept",
+                "metadata": ANY,
             }
         },
         "required": ["accept"],
         "title": "unknown",
         "type": "object",
     }
+
     assert Form.model_json_schema(mode="serialization") == expected
 
 
 def test_accept_schema_with_data():
     class SpecialAccept(Accept):
         data = [("field", "label")]
 
@@ -46,25 +49,26 @@
         accept: SpecialAccept
 
     expected = {
         "additionalProperties": False,
         "properties": {
             "accept": {
                 "data": [("field", "label")],
-                "enum": ["ACCEPTED", "INCOMPLETE"],
+                "enum": [AcceptValues.ACCEPTED, AcceptValues.INCOMPLETE],
                 "format": "accept",
-                "metadata": {"pydantic.internal.needs_apply_discriminated_union": False},
                 "type": "string",
                 "title": "Accept",
+                "metadata": ANY,
             }
         },
         "required": ["accept"],
         "title": "unknown",
         "type": "object",
     }
+
     assert Form.model_json_schema() == expected
 
 
 def test_accept_nok_incomplete():
     class Form(FormPage):
         accept: Accept
```

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_choice.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_choice_list.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_choice_list.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_constrained_list.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_constrained_list.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_contact_person.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_contact_person.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_contact_person_list.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_contact_person_list.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_core.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_core_async.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_core_async.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_display_subscription.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_display_subscription.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_list_of_one.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_list_of_one.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_list_of_two.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_list_of_two.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_migration_summary.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_migration_summary.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_organisation_id.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_organisation_id.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_read_only_field.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_read_only_field.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/tests/unit_tests/test_timestamp.py` & `pydantic_forms-1.0.3/tests/unit_tests/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `pydantic_forms-1.0.2/PKG-INFO` & `pydantic_forms-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pydantic-forms
-Version: 1.0.2
-Summary: This is the pydantic-forms engine.
+Version: 1.0.3
+Summary: Pydantic-forms engine.
 Home-page: https://github.com/workfloworchestrator/pydantic-forms
 Author: SURF
 Author-email: automation-beheer@surf.nl
 Requires-Python: >=3.9,<=3.13
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -31,15 +31,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: more-itertools
-Requires-Dist: pydantic[email] >= 2.5.1
+Requires-Dist: pydantic[email] ~= 2.5.1
+Requires-Dist: pydantic~=2.5.1
 Requires-Dist: toml ; extra == "dev"
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: mypy_extensions ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pydocstyle ; extra == "dev"
 Requires-Dist: python-dotenv ; extra == "dev"
 Requires-Dist: watchdog ; extra == "dev"
@@ -75,14 +76,16 @@
 Provides-Extra: orjson
 Provides-Extra: test
 
 # Pydantic forms
 
 [![pypi_version](https://img.shields.io/pypi/v/pydantic-forms?color=%2334D058&label=pypi%20package)](https://pypi.org/project/pydantic-forms)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/pydantic-forms.svg?color=%2334D058)](https://pypi.org/project/pydantic-forms)
+[![Downloads](https://static.pepy.tech/badge/pydantic-forms/month)](https://pepy.tech/project/pydantic-forms)
+[![codecov](https://codecov.io/gh/workfloworchestrator/pydantic-forms/branch/main/graph/badge.svg?token=AJMOSWPHQX)](https://codecov.io/gh/workfloworchestrator/pydantic-forms)
 
 A Python package that lets you add smart forms to [FastAPI](https://fastapi.tiangolo.com/)
 and [Flask](https://palletsprojects.com/p/flask/). Forms will respond with a JSON scheme that
 contains all info needed in a React frontend with uniforms to render the forms and handle all validation tasks.
 
 Forms can also consist out of a wizard, so you can create complex form flows consisting out of multiple
 consecutive forms. The forms and the validation logic are defined by
```

