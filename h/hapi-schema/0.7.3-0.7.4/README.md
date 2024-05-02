# Comparing `tmp/hapi_schema-0.7.3.tar.gz` & `tmp/hapi_schema-0.7.4.tar.gz`

## Comparing `hapi_schema-0.7.3.tar` & `hapi_schema-0.7.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/changelog.md
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/contributing.md
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/.config/coveragerc
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/.config/pytest.ini
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/.config/ruff.toml
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/_version.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_admin1.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_admin2.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_age_range.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_dataset.py
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_food_security.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_gender.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_humanitarian_needs.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_ipc_phase.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_ipc_type.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_location.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_national_risk.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_operational_presence.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_org.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_org_type.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_patch.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_population.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_population_group.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_population_status.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_resource.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/db_sector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/utils/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/utils/base.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/src/hapi_schema/utils/view_params.py
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/conftest.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_admin1.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_admin2.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_age_range.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_dataset.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_food_security.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_gender.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_humanitarian_needs.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_ipc_phase.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_ipc_type.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_location.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_national_risk.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_operational_presence.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_org.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_org_type.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_patch.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_population.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_population_group.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_population_status.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_resource.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/test_sector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/__init__.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_admin1.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_admin2.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_age_range.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_dataset.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_food_security.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_gender.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_humanitarian_needs.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_ipc_phase.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_ipc_type.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_location.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_national_risk.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_operational_presence.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_org.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_org_type.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_patch.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_population.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_population_group.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_population_status.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_resource.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/tests/sample_data/data_sector.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/README.md
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hapi_schema-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/changelog.md
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/contributing.md
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.config/coveragerc
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.config/pytest.ini
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.config/ruff.toml
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/_version.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_admin1.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_admin2.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_age_range.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_dataset.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_food_security.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_gender.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_humanitarian_needs.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_ipc_phase.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_ipc_type.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_location.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_national_risk.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_operational_presence.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_org.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_org_type.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_patch.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_population.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_population_group.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_population_status.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_resource.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_sector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/utils/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/utils/base.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/utils/view_params.py
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/conftest.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_admin1.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_admin2.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_age_range.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_dataset.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_food_security.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_gender.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_humanitarian_needs.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_ipc_phase.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_ipc_type.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_location.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_national_risk.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_operational_presence.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_org.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_org_type.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_patch.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_population.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_population_group.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_population_status.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_resource.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_sector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/__init__.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_admin1.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_admin2.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_age_range.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_dataset.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_food_security.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_gender.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_humanitarian_needs.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_ipc_phase.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_ipc_type.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_location.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_national_risk.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_operational_presence.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_org.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_org_type.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_patch.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_population.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_population_group.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_population_status.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_resource.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_sector.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/README.md
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/PKG-INFO
```

### Comparing `hapi_schema-0.7.3/changelog.md` & `hapi_schema-0.7.4/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-# [0.7.3]
+## [0.7.4]
+
+### Changed
+
+- Added columns to the patches table
+
+
+## [0.7.3]
 
 ### Fixed
 
 - Incorrect constraint quotes in IPC type
 - Clashing unique constraint names in admins
 
 ## [0.7.2]
@@ -25,14 +32,16 @@
 - Removed constraint from food security
 
 ### Added
 - Missing constraints
 - Tests on the constraints
 - `hapi_updated_date` and `hapi_replaced_date` fields
 
+## [0.7.0]
+
 ### Changed
 
 - Small changes to other dates for HAPI v2
 
 ## [0.6.2]
 
 ### Changed
```

### Comparing `hapi_schema-0.7.3/contributing.md` & `hapi_schema-0.7.4/contributing.md`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/requirements.txt` & `hapi_schema-0.7.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/.config/pre-commit-config.yaml` & `hapi_schema-0.7.4/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/.github/workflows/publish.yaml` & `hapi_schema-0.7.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/.github/workflows/run-python-tests.yaml` & `hapi_schema-0.7.4/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_admin1.py` & `hapi_schema-0.7.4/src/hapi_schema/db_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_admin2.py` & `hapi_schema-0.7.4/src/hapi_schema/db_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_age_range.py` & `hapi_schema-0.7.4/src/hapi_schema/db_age_range.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_dataset.py` & `hapi_schema-0.7.4/src/hapi_schema/db_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """Dataset table and view."""
 
-from sqlalchemy import Integer, String, select
+from sqlalchemy import String, select
 from sqlalchemy.orm import Mapped, mapped_column
 
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBDataset(Base):
     __tablename__ = "dataset"
 
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    hdx_id: Mapped[str] = mapped_column(
-        String(36), unique=True, nullable=False
-    )
+    hdx_id: Mapped[str] = mapped_column(String(36), primary_key=True)
     hdx_stub: Mapped[str] = mapped_column(
         String(128), unique=True, nullable=False
     )
     title = mapped_column(String(1024), nullable=False)
     hdx_provider_stub: Mapped[str] = mapped_column(
         String(128), nullable=False, index=True
     )
```

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_food_security.py` & `hapi_schema-0.7.4/src/hapi_schema/db_food_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         CheckConstraint(
             "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
             name="reference_period",
         ),
     )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    resource_ref: Mapped[int] = mapped_column(
-        ForeignKey("resource.id", onupdate="CASCADE", ondelete="CASCADE"),
+    resource_hdx_id: Mapped[int] = mapped_column(
+        ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"), nullable=False
     )
     ipc_phase_code: Mapped[str] = mapped_column(
         ForeignKey("ipc_phase.code", onupdate="CASCADE"), nullable=False
@@ -75,15 +75,14 @@
         *DBFoodSecurity.__table__.columns,
         DBDataset.hdx_id.label("dataset_hdx_id"),
         DBDataset.hdx_stub.label("dataset_hdx_stub"),
         DBDataset.title.label("dataset_title"),
         DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
         DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
         DBIpcPhase.name.label("ipc_phase_name"),
-        DBResource.hdx_id.label("resource_hdx_id"),
         DBResource.name.label("resource_name"),
         DBResource.update_date.label("resource_update_date"),
         DBResource.hapi_updated_date.label("hapi_updated_date"),
         DBResource.hapi_replaced_date.label("hapi_replaced_date"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
@@ -110,20 +109,20 @@
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
         # Join pop to resource to dataset
         .join(
             DBResource.__table__,
-            DBFoodSecurity.resource_ref == DBResource.id,
+            DBFoodSecurity.resource_hdx_id == DBResource.hdx_id,
             isouter=True,
         )
         .join(
             DBDataset.__table__,
-            DBResource.dataset_ref == DBDataset.id,
+            DBResource.dataset_hdx_id == DBDataset.hdx_id,
             isouter=True,
         )
         # Join to ipc phase
         .join(
             DBIpcPhase.__table__,
             DBFoodSecurity.ipc_phase_code == DBIpcPhase.code,
             isouter=True,
```

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_gender.py` & `hapi_schema-0.7.4/src/hapi_schema/db_gender.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_humanitarian_needs.py` & `hapi_schema-0.7.4/src/hapi_schema/db_humanitarian_needs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         CheckConstraint(
             "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
             name="reference_period",
         ),
     )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    resource_ref: Mapped[int] = mapped_column(
-        ForeignKey("resource.id", onupdate="CASCADE", ondelete="CASCADE"),
+    resource_hdx_id: Mapped[int] = mapped_column(
+        ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"), nullable=False
     )
     population_status_code: Mapped[str] = mapped_column(
         ForeignKey("population_status.code", onupdate="CASCADE"),
@@ -87,15 +87,14 @@
     selectable=select(
         *DBHumanitarianNeeds.__table__.columns,
         DBDataset.hdx_id.label("dataset_hdx_id"),
         DBDataset.hdx_stub.label("dataset_hdx_stub"),
         DBDataset.title.label("dataset_title"),
         DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
         DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
-        DBResource.hdx_id.label("resource_hdx_id"),
         DBResource.name.label("resource_name"),
         DBResource.update_date.label("resource_update_date"),
         DBResource.hapi_updated_date.label("hapi_updated_date"),
         DBResource.hapi_replaced_date.label("hapi_replaced_date"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
@@ -123,20 +122,20 @@
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
         # Join needs to resource to dataset
         .join(
             DBResource.__table__,
-            DBHumanitarianNeeds.resource_ref == DBResource.id,
+            DBHumanitarianNeeds.resource_hdx_id == DBResource.hdx_id,
             isouter=True,
         )
         .join(
             DBDataset.__table__,
-            DBResource.dataset_ref == DBDataset.id,
+            DBResource.dataset_hdx_id == DBDataset.hdx_id,
             isouter=True,
         )
         # Join needs to sector
         .join(
             DBSector.__table__,
             DBHumanitarianNeeds.sector_code == DBSector.code,
             isouter=True,
```

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_ipc_phase.py` & `hapi_schema-0.7.4/src/hapi_schema/db_ipc_phase.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_ipc_type.py` & `hapi_schema-0.7.4/src/hapi_schema/db_ipc_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_location.py` & `hapi_schema-0.7.4/src/hapi_schema/db_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_national_risk.py` & `hapi_schema-0.7.4/src/hapi_schema/db_national_risk.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         CheckConstraint(
             "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
             name="reference_period",
         ),
     )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    resource_ref: Mapped[int] = mapped_column(
-        ForeignKey("resource.id", onupdate="CASCADE", ondelete="CASCADE"),
+    resource_hdx_id: Mapped[int] = mapped_column(
+        ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"), nullable=False
     )
     risk_class: Mapped[int] = mapped_column(Integer, nullable=False)
     global_rank: Mapped[int] = mapped_column(Integer, nullable=False)
@@ -74,15 +74,14 @@
     selectable=select(
         *DBNationalRisk.__table__.columns,
         DBDataset.hdx_id.label("dataset_hdx_id"),
         DBDataset.hdx_stub.label("dataset_hdx_stub"),
         DBDataset.title.label("dataset_title"),
         DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
         DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
-        DBResource.hdx_id.label("resource_hdx_id"),
         DBResource.name.label("resource_name"),
         DBResource.update_date.label("resource_update_date"),
         DBResource.hapi_updated_date.label("hapi_updated_date"),
         DBResource.hapi_replaced_date.label("hapi_replaced_date"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
@@ -107,17 +106,17 @@
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
         # Join risk to resource to dataset
         .join(
             DBResource.__table__,
-            DBNationalRisk.resource_ref == DBResource.id,
+            DBNationalRisk.resource_hdx_id == DBResource.hdx_id,
             isouter=True,
         )
         .join(
             DBDataset.__table__,
-            DBResource.dataset_ref == DBDataset.id,
+            DBResource.dataset_hdx_id == DBDataset.hdx_id,
             isouter=True,
         )
     ),
 )
```

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_operational_presence.py` & `hapi_schema-0.7.4/src/hapi_schema/db_operational_presence.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         CheckConstraint(
             "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
             name="reference_period",
         ),
     )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    resource_ref = mapped_column(
-        ForeignKey("resource.id", onupdate="CASCADE", ondelete="CASCADE"),
+    resource_hdx_id = mapped_column(
+        ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"), nullable=False
     )
     org_ref: Mapped[str] = mapped_column(
         ForeignKey("org.id", onupdate="CASCADE"), nullable=False
@@ -68,15 +68,14 @@
     selectable=select(
         *DBOperationalPresence.__table__.columns,
         DBDataset.hdx_id.label("dataset_hdx_id"),
         DBDataset.hdx_stub.label("dataset_hdx_stub"),
         DBDataset.title.label("dataset_title"),
         DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
         DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
-        DBResource.hdx_id.label("resource_hdx_id"),
         DBResource.name.label("resource_name"),
         DBResource.update_date.label("resource_update_date"),
         DBResource.hapi_updated_date.label("hapi_updated_date"),
         DBResource.hapi_replaced_date.label("hapi_replaced_date"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
@@ -108,20 +107,20 @@
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
         # Join op to resource to dataset
         .join(
             DBResource.__table__,
-            DBOperationalPresence.resource_ref == DBResource.id,
+            DBOperationalPresence.resource_hdx_id == DBResource.hdx_id,
             isouter=True,
         )
         .join(
             DBDataset.__table__,
-            DBResource.dataset_ref == DBDataset.id,
+            DBResource.dataset_hdx_id == DBDataset.hdx_id,
             isouter=True,
         )
         # Join op to org to org type
         .join(
             DBOrg.__table__,
             DBOperationalPresence.org_ref == DBOrg.id,
             isouter=True,
```

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_org.py` & `hapi_schema-0.7.4/src/hapi_schema/db_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_org_type.py` & `hapi_schema-0.7.4/src/hapi_schema/db_org_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_population.py` & `hapi_schema-0.7.4/src/hapi_schema/db_population.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         CheckConstraint(
             "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
             name="reference_period",
         ),
     )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    resource_ref: Mapped[int] = mapped_column(
-        ForeignKey("resource.id", onupdate="CASCADE", ondelete="CASCADE"),
+    resource_hdx_id: Mapped[int] = mapped_column(
+        ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"), nullable=False
     )
     gender_code: Mapped[str] = mapped_column(
         ForeignKey("gender.code", onupdate="CASCADE"), nullable=True
@@ -69,15 +69,14 @@
     selectable=select(
         *DBPopulation.__table__.columns,
         DBDataset.hdx_id.label("dataset_hdx_id"),
         DBDataset.hdx_stub.label("dataset_hdx_stub"),
         DBDataset.title.label("dataset_title"),
         DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
         DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
-        DBResource.hdx_id.label("resource_hdx_id"),
         DBResource.name.label("resource_name"),
         DBResource.update_date.label("resource_update_date"),
         DBResource.hapi_updated_date.label("hapi_updated_date"),
         DBResource.hapi_replaced_date.label("hapi_replaced_date"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
@@ -104,17 +103,17 @@
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
         # Join pop to resource to dataset
         .join(
             DBResource.__table__,
-            DBPopulation.resource_ref == DBResource.id,
+            DBPopulation.resource_hdx_id == DBResource.hdx_id,
             isouter=True,
         )
         .join(
             DBDataset.__table__,
-            DBResource.dataset_ref == DBDataset.id,
+            DBResource.dataset_hdx_id == DBDataset.hdx_id,
             isouter=True,
         )
     ),
 )
```

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_population_group.py` & `hapi_schema-0.7.4/src/hapi_schema/db_population_group.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_population_status.py` & `hapi_schema-0.7.4/src/hapi_schema/db_population_status.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_resource.py` & `hapi_schema-0.7.4/src/hapi_schema/db_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from datetime import datetime
 
 from sqlalchemy import (
     Boolean,
     CheckConstraint,
     DateTime,
     ForeignKey,
-    Integer,
     String,
     select,
     text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_dataset import DBDataset
@@ -24,22 +23,19 @@
     __table_args__ = (
         CheckConstraint(
             "(hapi_replaced_date IS NULL) OR (hapi_replaced_date >= hapi_updated_date)",
             name="hapi_dates",
         ),
     )
 
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    dataset_ref: Mapped[int] = mapped_column(
-        ForeignKey("dataset.id", onupdate="CASCADE", ondelete="CASCADE"),
+    hdx_id: Mapped[str] = mapped_column(String(36), primary_key=True)
+    dataset_hdx_id: Mapped[int] = mapped_column(
+        ForeignKey("dataset.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
-    hdx_id: Mapped[str] = mapped_column(
-        String(36), unique=True, nullable=False
-    )
     name: Mapped[str] = mapped_column(String(256), nullable=False)
     format: Mapped[str] = mapped_column(String(32), nullable=False)
     update_date = mapped_column(DateTime, nullable=False, index=True)
     download_url: Mapped[str] = mapped_column(
         String(1024), nullable=False, unique=True
     )
     is_hxl: Mapped[bool] = mapped_column(Boolean, nullable=False, index=True)
@@ -51,20 +47,19 @@
 
 
 view_params_resource = ViewParams(
     name="resource_view",
     metadata=Base.metadata,
     selectable=select(
         *DBResource.__table__.columns,
-        DBDataset.hdx_id.label("dataset_hdx_id"),
         DBDataset.hdx_stub.label("dataset_hdx_stub"),
         DBDataset.title.label("dataset_title"),
         DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
         DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
     ).select_from(
         DBResource.__table__.join(
             DBDataset.__table__,
-            DBResource.dataset_ref == DBDataset.id,
+            DBResource.dataset_hdx_id == DBDataset.hdx_id,
             isouter=True,
         )
     ),
 )
```

### Comparing `hapi_schema-0.7.3/src/hapi_schema/db_sector.py` & `hapi_schema-0.7.4/src/hapi_schema/db_sector.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/conftest.py` & `hapi_schema-0.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/test_admin1.py` & `hapi_schema-0.7.4/tests/test_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/test_admin2.py` & `hapi_schema-0.7.4/tests/test_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/test_dataset.py` & `hapi_schema-0.7.4/tests/test_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 
 def test_dataset_view(run_view_test):
     """Check that dataset view has most columns."""
     view_dataset = build_view(view_params_dataset.__dict__)
     run_view_test(
         view=view_dataset,
         whereclause=(
-            view_dataset.c.id == 1,
+            view_dataset.c.hdx_id == "c3f001fa-b45b-464c-9460-1ca79fd39b40",
             view_dataset.c.hdx_stub == "dataset01",
             view_dataset.c.title == "Dataset #1",
             view_dataset.c.hdx_provider_stub == "provider01",
             view_dataset.c.hdx_provider_name == "Provider #1",
         ),
     )
```

### Comparing `hapi_schema-0.7.3/tests/test_food_security.py` & `hapi_schema-0.7.4/tests/test_food_security.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,29 @@
         view=view_food_security,
         whereclause=(
             view_food_security.c.id == 3,
             view_food_security.c.dataset_hdx_id
             == "7cf3cec8-dbbc-4c96-9762-1464cd0bff75",
             view_food_security.c.resource_hdx_id
             == "62ad6e55-5f5d-4494-854c-4110687e9e25",
+            view_food_security.c.resource_name == "resource-03.csv",
             view_food_security.c.ipc_phase_name == "Phase 3: Crisis",
             view_food_security.c.admin2_code == "FOO-001-A",
             view_food_security.c.admin1_code == "FOO-001",
             view_food_security.c.location_code == "FOO",
         ),
     )
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
             DBFoodSecurity(
-                resource_ref=3,
+                resource_hdx_id="62ad6e55-5f5d-4494-854c-4110687e9e25",
                 admin2_ref=4,
                 ipc_phase_code="1",
                 ipc_type_code="current",
                 population_in_phase=1_000,
                 population_fraction_in_phase=1,
                 reference_period_start=datetime(2023, 2, 1),
                 reference_period_end=datetime(2023, 1, 1),
```

### Comparing `hapi_schema-0.7.3/tests/test_humanitarian_needs.py` & `hapi_schema-0.7.4/tests/test_humanitarian_needs.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         view=view_humanitarian_needs,
         whereclause=(
             view_humanitarian_needs.c.id == 3,
             view_humanitarian_needs.c.dataset_hdx_id
             == "c3f001fa-b45b-464c-9460-1ca79fd39b40",
             view_humanitarian_needs.c.resource_hdx_id
             == "90deb235-1bf5-4bae-b231-3393222c2d01",
+            view_humanitarian_needs.c.resource_name == "resource-01.csv",
             view_humanitarian_needs.c.admin2_code == "FOO-001-XXX",
             view_humanitarian_needs.c.admin1_code == "FOO-001",
             view_humanitarian_needs.c.location_code == "FOO",
             view_humanitarian_needs.c.population_status_code == "inneed",
             view_humanitarian_needs.c.population_group_code == "idps",
             view_humanitarian_needs.c.sector_name
             == "Water Sanitation Hygiene",
@@ -35,15 +36,15 @@
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
             DBHumanitarianNeeds(
-                resource_ref=1,
+                resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
                 admin2_ref=1,
                 gender_code=None,
                 age_range_code=None,
                 disabled_marker=None,
                 sector_code=None,
                 population_group_code=None,
                 population_status_code="affected",
```

### Comparing `hapi_schema-0.7.3/tests/test_ipc_phase.py` & `hapi_schema-0.7.4/tests/test_ipc_phase.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/test_ipc_type.py` & `hapi_schema-0.7.4/tests/test_ipc_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/test_location.py` & `hapi_schema-0.7.4/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/test_national_risk.py` & `hapi_schema-0.7.4/tests/test_national_risk.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,27 +15,28 @@
         view=view_national_risk,
         whereclause=(
             view_national_risk.c.id == 1,
             view_national_risk.c.dataset_hdx_id
             == "c3f001fa-b45b-464c-9460-1ca79fd39b40",
             view_national_risk.c.resource_hdx_id
             == "90deb235-1bf5-4bae-b231-3393222c2d01",
+            view_national_risk.c.resource_name == "resource-01.csv",
             view_national_risk.c.admin2_code == "FOO-XXX-XXX",
             view_national_risk.c.admin1_code == "FOO-XXX",
             view_national_risk.c.location_code == "FOO",
         ),
     )
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
             DBNationalRisk(
-                resource_ref=1,
+                resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
                 admin2_ref=1,
                 risk_class=5,
                 global_rank=4,
                 overall_risk=8.1,
                 hazard_exposure_risk=8.7,
                 vulnerability_risk=8.5,
                 coping_capacity_risk=7.1,
@@ -51,15 +52,15 @@
 
 
 def test_meta_avg_recentness_constraint(run_constraints_test):
     """Check that meta_avg_recentness_years is >= 0"""
     run_constraints_test(
         new_rows=[
             DBNationalRisk(
-                resource_ref=1,
+                resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
                 admin2_ref=1,
                 risk_class=5,
                 global_rank=4,
                 overall_risk=8.1,
                 hazard_exposure_risk=8.7,
                 vulnerability_risk=8.5,
                 coping_capacity_risk=7.1,
```

### Comparing `hapi_schema-0.7.3/tests/test_operational_presence.py` & `hapi_schema-0.7.4/tests/test_operational_presence.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         view=view_operational_presence,
         whereclause=(
             view_operational_presence.c.id == 5,
             view_operational_presence.c.dataset_hdx_id
             == "c3f001fa-b45b-464c-9460-1ca79fd39b40",
             view_operational_presence.c.resource_hdx_id
             == "90deb235-1bf5-4bae-b231-3393222c2d01",
+            view_operational_presence.c.resource_name == "resource-01.csv",
             view_operational_presence.c.admin2_code == "FOO-XXX-XXX",
             view_operational_presence.c.admin1_code == "FOO-XXX",
             view_operational_presence.c.location_code == "FOO",
             view_operational_presence.c.org_type_description
             == "International NGO",
             view_operational_presence.c.org_acronym == "ORG02",
             view_operational_presence.c.sector_name
@@ -34,15 +35,15 @@
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
             DBOperationalPresence(
-                resource_ref=1,
+                resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
                 admin2_ref=2,
                 org_ref=1,
                 sector_code="SHL",
                 reference_period_start=datetime(2023, 1, 2),
                 reference_period_end=datetime(2023, 1, 1),
                 source_data="DATA,DATA,DATA",
             )
```

### Comparing `hapi_schema-0.7.3/tests/test_org.py` & `hapi_schema-0.7.4/tests/test_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/test_patch.py` & `hapi_schema-0.7.4/tests/test_patch.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,20 +10,24 @@
     Base.metadata.create_all(engine)
 
     sql_table_creation_code = """CREATE TABLE patch (
         id INTEGER NOT NULL,
         patch_sequence_number INTEGER NOT NULL,
         commit_hash VARCHAR(48) NOT NULL,
         commit_date DATETIME NOT NULL,
-        patch_path VARCHAR(128) NOT NULL,
-        permanent_download_url VARCHAR(1024) NOT NULL,
+        patch_path VARCHAR(512) NOT NULL,
+        patch_permalink_url VARCHAR(1024) NOT NULL,
+        patch_target VARCHAR(128) NOT NULL,
+        patch_hash VARCHAR(48) NOT NULL,
         state VARCHAR(10) NOT NULL,
+        execution_date DATETIME,
         PRIMARY KEY (id),
         UNIQUE (commit_hash),
-        UNIQUE (permanent_download_url)
+        UNIQUE (patch_permalink_url),
+        UNIQUE (patch_hash)
 )
 """
     sql_patch_sequence_number_index_creation = """
     CREATE INDEX ix_patch_patch_sequence_number ON patch (patch_sequence_number)
     """
     sql_state_index_creation = (
         """CREATE INDEX ix_patch_state ON patch (state)"""
```

### Comparing `hapi_schema-0.7.3/tests/test_population.py` & `hapi_schema-0.7.4/tests/test_population.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,28 +12,29 @@
         view=view_population,
         whereclause=(
             view_population.c.id == 3,
             view_population.c.dataset_hdx_id
             == "c3f001fa-b45b-464c-9460-1ca79fd39b40",
             view_population.c.resource_hdx_id
             == "90deb235-1bf5-4bae-b231-3393222c2d01",
+            view_population.c.resource_name == "resource-01.csv",
             view_population.c.admin2_code == "FOO-001-XXX",
             view_population.c.admin1_code == "FOO-001",
             view_population.c.location_code == "FOO",
             view_population.c.gender_code == "f",
         ),
     )
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
             DBPopulation(
-                resource_ref=1,
+                resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
                 admin2_ref=1,
                 gender_code=None,
                 age_range_code=None,
                 population=1_000_000,
                 reference_period_start=datetime(2023, 1, 2),
                 reference_period_end=datetime(2023, 1, 1),
                 source_data="DATA,DATA,DATA",
@@ -44,15 +45,15 @@
 
 
 def test_population_positive(run_constraints_test):
     """Check that the population value is positive"""
     run_constraints_test(
         new_rows=[
             DBPopulation(
-                resource_ref=1,
+                resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
                 admin2_ref=1,
                 gender_code=None,
                 age_range_code=None,
                 population=-1,
                 reference_period_start=None,
                 reference_period_end=None,
                 source_data="DATA,DATA,DATA",
```

### Comparing `hapi_schema-0.7.3/tests/test_population_group.py` & `hapi_schema-0.7.4/tests/test_population_group.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/test_population_status.py` & `hapi_schema-0.7.4/tests/test_population_status.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/test_resource.py` & `hapi_schema-0.7.4/tests/test_resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,44 +7,43 @@
 
 def test_resource_view(run_view_test):
     """Check that resource references dataset."""
     view_resource = build_view(view_params_resource.__dict__)
     run_view_test(
         view=view_resource,
         whereclause=(
-            view_resource.c.id == 1,
-            view_resource.c.dataset_hdx_id
-            == "c3f001fa-b45b-464c-9460-1ca79fd39b40",
+            view_resource.c.hdx_id == "90deb235-1bf5-4bae-b231-3393222c2d01",
+            view_resource.c.dataset_hdx_stub == "dataset01",
         ),
     )
 
 
 def test_hapi_date_constraint(run_constraints_test):
     """Check that hapi_replaced_date cannot be less than hapi_updated_date"""
     run_constraints_test(
         new_rows=[
             DBResource(
-                dataset_ref=2,
                 hdx_id="9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f",
+                dataset_hdx_id="7cf3cec8-dbbc-4c96-9762-1464cd0bff75",
                 name="resource-04.csv",
                 format="csv",
                 update_date=datetime(2023, 1, 1),
                 download_url="https://data.humdata.org/dataset/7cf3cec8-dbbc-4c96-9762-1464cd0bff75/resource/9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f/download/resource-04.csv",
                 is_hxl=True,
                 hapi_updated_date=datetime(2023, 1, 2),
                 hapi_replaced_date=datetime(2023, 1, 1),
             )
         ],
         expected_constraint="hapi_dates",
     )
 
     (
         dict(
-            dataset_ref=2,
             hdx_id="9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f",
+            dataset_hdx_id="7cf3cec8-dbbc-4c96-9762-1464cd0bff75",
             name="resource-04.csv",
             format="csv",
             update_date=datetime(2023, 1, 1),
             download_url="https://data.humdata.org/dataset/7cf3cec8-dbbc-4c96-9762-1464cd0bff75/resource/9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f/download/resource-04.csv",
             is_hxl=True,
             hapi_updated_date=datetime(2023, 8, 1),
             hapi_replaced_date=None,
```

### Comparing `hapi_schema-0.7.3/tests/sample_data/data_admin1.py` & `hapi_schema-0.7.4/tests/sample_data/data_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/sample_data/data_admin2.py` & `hapi_schema-0.7.4/tests/sample_data/data_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/sample_data/data_ipc_phase.py` & `hapi_schema-0.7.4/tests/sample_data/data_ipc_phase.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/sample_data/data_national_risk.py` & `hapi_schema-0.7.4/tests/sample_data/data_national_risk.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 data_national_risk = [
     dict(
         id=1,
-        resource_ref=1,
+        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         admin2_ref=1,
         risk_class=5,
         global_rank=4,
         overall_risk=8.1,
         hazard_exposure_risk=8.7,
         vulnerability_risk=8.5,
         coping_capacity_risk=7.1,
```

### Comparing `hapi_schema-0.7.3/tests/sample_data/data_org.py` & `hapi_schema-0.7.4/tests/sample_data/data_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/tests/sample_data/data_patch.py` & `hapi_schema-0.7.4/tests/sample_data/data_patch.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,30 +2,39 @@
 
 data_patch = [
     dict(
         id=1,
         patch_sequence_number=1,
         commit_hash="66e7e589a1224a1832ba7360817dda7a7d9313cf",
         commit_date=datetime(2023, 1, 1),
-        patch_path="2024/01",
-        permanent_download_url="https://github.com/OCHA-DAP/hapi-patch-repo/blob/66e7e589a1224a1832ba7360817dda7a7d9313cf/2024/01/hapi_patch_10_hno.json",
+        patch_path="/2024/01/hapi_patch_1_hno.json",
+        patch_target="humanitarian_needs",
+        patch_hash="66e7e589a1224a1832ba7360817dda7a7d9313dg",
+        patch_permalink_url="https://github.com/OCHA-DAP/hapi-patch-repo/blob/66e7e589a1224a1832ba7360817dda7a7d9313cf/2024/01/hapi_patch_1_hno.json",
         state="executed",
+        execution_date=datetime(2023, 1, 2),
     ),
     dict(
         id=2,
         patch_sequence_number=2,
         commit_hash="554f18a92cf6a23a14e0f29356a6dec150f651ff",
         commit_date=datetime(2023, 1, 2),
-        patch_path="2024/01",
-        permanent_download_url="https://github.com/OCHA-DAP/hapi-patch-repo/blob/554f18a92cf6a23a14e0f29356a6dec150f651ff/2024/01/hapi_patch_10_hno.json",
+        patch_path="2024/01/hapi_patch_2_hno.json",
+        patch_target="humanitarian_needs",
+        patch_hash="554f18a92cf6a23a14e0f29356a6dec150f651gg",
+        patch_permalink_url="https://github.com/OCHA-DAP/hapi-patch-repo/blob/554f18a92cf6a23a14e0f29356a6dec150f651ff/2024/01/hapi_patch_2_hno.json",
         state="failed",
+        execution_date=datetime(2023, 1, 3),
     ),
     dict(
         id=3,
         patch_sequence_number=3,
         commit_hash="35ea27da009e5add8d8d227e02fd2c4bbcc84b76",
         commit_date=datetime(2023, 1, 3),
-        patch_path="2024/01",
-        permanent_download_url="https://github.com/OCHA-DAP/hapi-patch-repo/blob/35ea27da009e5add8d8d227e02fd2c4bbcc84b76/2024/01/hapi_patch_10_hno.json",
+        patch_path="2024/01/hapi_patch_3_hno.json",
+        patch_target="humanitarian_needs",
+        patch_hash="554f18a92cf6a23a14e0f29356a6dec150f65187",
+        patch_permalink_url="https://github.com/OCHA-DAP/hapi-patch-repo/blob/35ea27da009e5add8d8d227e02fd2c4bbcc84b76/2024/01/hapi_patch_3_hno.json",
         state="discovered",
+        execution_date=None,
     ),
 ]
```

### Comparing `hapi_schema-0.7.3/tests/sample_data/data_population.py` & `hapi_schema-0.7.4/tests/sample_data/data_operational_presence.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 from datetime import datetime
 
-data_population = [
-    # total national
+data_operational_presence = [
     dict(
         id=1,
-        resource_ref=1,
-        admin2_ref=1,
-        gender_code=None,
-        age_range_code=None,
-        population=1_000_000,
+        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
+        admin2_ref=2,
+        org_ref=1,
+        sector_code="SHL",
         reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=datetime(2023, 6, 30),
+        reference_period_end=None,
         source_data="DATA,DATA,DATA",
     ),
-    # national f, all ages
     dict(
         id=2,
-        resource_ref=1,
-        admin2_ref=1,
-        gender_code="f",
-        age_range_code=None,
-        population=500_000,
+        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
+        admin2_ref=4,
+        org_ref=2,
+        sector_code="FSC",
         reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=datetime(2023, 6, 30),
+        reference_period_end=None,
         source_data="DATA,DATA,DATA",
     ),
-    # admin1 f, age 0-4
     dict(
         id=3,
-        resource_ref=1,
-        admin2_ref=2,
-        gender_code="f",
-        age_range_code="0-4",
-        population=5_000,
+        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
+        admin2_ref=4,
+        org_ref=3,
+        sector_code="WSH",
         reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=datetime(2023, 6, 30),
+        reference_period_end=None,
         source_data="DATA,DATA,DATA",
     ),
-    # admin2 ages 80+
     dict(
         id=4,
-        resource_ref=1,
-        admin2_ref=4,
-        gender_code=None,
-        age_range_code="80+",
-        population=500,
+        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
+        admin2_ref=6,
+        org_ref=3,
+        sector_code="HEA",
+        reference_period_start=datetime(2023, 1, 1),
+        reference_period_end=None,
+        source_data="DATA,DATA,DATA",
+    ),
+    dict(
+        id=5,
+        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
+        admin2_ref=1,
+        org_ref=2,
+        sector_code="WSH",
         reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=datetime(2023, 6, 30),
+        reference_period_end=None,
         source_data="DATA,DATA,DATA",
     ),
 ]
```

### Comparing `hapi_schema-0.7.3/.gitignore` & `hapi_schema-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/LICENSE` & `hapi_schema-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/pyproject.toml` & `hapi_schema-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.3/PKG-INFO` & `hapi_schema-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hapi-schema
-Version: 0.7.3
+Version: 0.7.4
 Summary: HAPI database schema specified in SQLAlchemy
 Project-URL: Homepage, https://github.com/OCHA-DAP/hapi-schemas
 Author-email: Simon Johnson <simon.johnson@un.org>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,hapi,schema
 Classifier: Intended Audience :: Developers
```

