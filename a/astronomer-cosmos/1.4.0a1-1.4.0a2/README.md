# Comparing `tmp/astronomer_cosmos-1.4.0a1.tar.gz` & `tmp/astronomer_cosmos-1.4.0a2.tar.gz`

## Comparing `astronomer_cosmos-1.4.0a1.tar` & `astronomer_cosmos-1.4.0a2.tar`

### file list

```diff
@@ -1,72 +1,74 @@
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/__init__.py
--rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/config.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/constants.py
--rw-r--r--   0        0        0    12655 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/converter.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/exceptions.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/airflow/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/airflow/dag.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/airflow/graph.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/airflow/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/core/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/dbt/executable.py
--rw-r--r--   0        0        0    17773 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/dbt/graph.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/dbt/project.py
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/dbt/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/operators/azure_container_instance.py
--rw-r--r--   0        0        0    14758 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/operators/base.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/operators/docker.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/operators/local.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/plugin/__init__.py
--rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/plugin/static/iframeResizer.contentWindow.min.js
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/plugin/static/iframeResizer.min.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/plugin/templates/dbt_docs.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/plugin/templates/dbt_docs_not_set_up.html
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/__init__.py
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/base.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/athena/__init__.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/athena/access_key.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/bigquery/oauth.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/bigquery/service_account_keyfile_dict.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/snowflake/user_privatekey.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/vertica/__init__.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/cosmos/profiles/vertica/user_pass.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/LICENSE
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/README.rst
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/pyproject.toml
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/cache.py
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/config.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/constants.py
+-rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/converter.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/exceptions.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/log.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0    18527 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/project.py
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/azure_container_instance.py
+-rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/base.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    32029 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/local.py
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/plugin/__init__.py
+-rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/plugin/static/iframeResizer.contentWindow.min.js
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/plugin/static/iframeResizer.min.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/plugin/templates/dbt_docs.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/plugin/templates/dbt_docs_not_set_up.html
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/__init__.py
+-rwxr-xr-x   0        0        0    11351 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/athena/__init__.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/athena/access_key.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/oauth.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/vertica/__init__.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/vertica/user_pass.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/LICENSE
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/README.rst
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/pyproject.toml
+-rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/PKG-INFO
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/__init__.py` & `astronomer_cosmos-1.4.0a2/cosmos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore # ignores "Cannot assign to a type" MyPy error
 
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
-__version__ = "1.4.0a1"
+__version__ = "1.4.0a2"
 
 
 from cosmos.airflow.dag import DbtDag
 from cosmos.airflow.task_group import DbtTaskGroup
 from cosmos.config import (
     ExecutionConfig,
     ProfileConfig,
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/config.py` & `astronomer_cosmos-1.4.0a2/cosmos/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,30 +50,31 @@
     :param selector: Name of a dbt YAML selector to use for parsing. Only supported when using ``load_method=LoadMode.DBT_LS``.
     :param dbt_deps: Configure to run dbt deps when using dbt ls for dag parsing
     :param node_converters: a dictionary mapping a ``DbtResourceType`` into a callable. Users can control how to render dbt nodes in Airflow. Only supported when using ``load_method=LoadMode.DBT_MANIFEST`` or ``LoadMode.DBT_LS``.
     :param dbt_executable_path: The path to the dbt executable for dag generation. Defaults to dbt if available on the path.
     :param env_vars: (Deprecated since Cosmos 1.3 use ProjectConfig.env_vars) A dictionary of environment variables for rendering. Only supported when using ``LoadMode.DBT_LS``.
     :param dbt_project_path: Configures the DBT project location accessible on the airflow controller for DAG rendering. Mutually Exclusive with ProjectConfig.dbt_project_path. Required when using ``load_method=LoadMode.DBT_LS`` or ``load_method=LoadMode.CUSTOM``.
     :param dbt_ls_path: Configures the location of an output of ``dbt ls``. Required when using ``load_method=LoadMode.DBT_LS_FILE``.
+    :param enable_mock_profile: Allows to enable/disable mocking profile. Enabled by default. Mock profiles are useful for parsing Cosmos DAGs in the CI, but should be disabled to benefit from partial parsing (since Cosmos 1.4).
     """
 
     emit_datasets: bool = True
     test_behavior: TestBehavior = TestBehavior.AFTER_EACH
     load_method: LoadMode = LoadMode.AUTOMATIC
     select: list[str] = field(default_factory=list)
     exclude: list[str] = field(default_factory=list)
     selector: str | None = None
     dbt_deps: bool = True
     node_converters: dict[DbtResourceType, Callable[..., Any]] | None = None
     dbt_executable_path: str | Path = get_system_dbt()
     env_vars: dict[str, str] | None = None
     dbt_project_path: InitVar[str | Path | None] = None
     dbt_ls_path: Path | None = None
-
     project_path: Path | None = field(init=False)
+    enable_mock_profile: bool = True
 
     def __post_init__(self, dbt_project_path: str | Path | None) -> None:
         if self.env_vars:
             warnings.warn(
                 "RenderConfig.env_vars is deprecated since Cosmos 1.3 and will be removed in Cosmos 2.0. Use ProjectConfig.env_vars instead.",
                 DeprecationWarning,
             )
@@ -284,15 +285,16 @@
                 # write profile_contents to desired_profile_path using yaml library
                 desired_profile_path.write_text(profile_contents)
                 yield desired_profile_path, env_vars
             else:
                 with tempfile.TemporaryDirectory() as temp_dir:
                     temp_file = Path(temp_dir) / DEFAULT_PROFILES_FILE_NAME
                     logger.info(
-                        "Creating temporary profiles.yml at %s with the following contents:\n%s",
+                        "Creating temporary profiles.yml with use_mock_values=%s at %s with the following contents:\n%s",
+                        use_mock_values,
                         temp_file,
                         profile_contents,
                     )
                     temp_file.write_text(profile_contents)
                     yield temp_file, env_vars
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/constants.py` & `astronomer_cosmos-1.4.0a2/cosmos/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 from pathlib import Path
 
 import aenum
 
 DBT_PROFILE_PATH = Path(os.path.expanduser("~")).joinpath(".dbt/profiles.yml")
 DEFAULT_DBT_PROFILE_NAME = "cosmos_profile"
 DEFAULT_DBT_TARGET_NAME = "cosmos_target"
+DEFAULT_COSMOS_CACHE_DIR_NAME = "cosmos"
 DBT_LOG_PATH_ENVVAR = "DBT_LOG_PATH"
 DBT_LOG_DIR_NAME = "logs"
 DBT_TARGET_PATH_ENVVAR = "DBT_TARGET_PATH"
 DBT_TARGET_DIR_NAME = "target"
 DBT_PARTIAL_PARSE_FILE_NAME = "partial_parse.msgpack"
+DBT_MANIFEST_FILE_NAME = "manifest.json"
 DBT_LOG_FILENAME = "dbt.log"
 DBT_BINARY_NAME = "dbt"
 
 DEFAULT_OPENLINEAGE_NAMESPACE = "cosmos"
 OPENLINEAGE_PRODUCER = "https://github.com/astronomer/astronomer-cosmos/"
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/converter.py` & `astronomer_cosmos-1.4.0a2/cosmos/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import inspect
 from typing import Any, Callable
 from warnings import warn
 
 from airflow.models.dag import DAG
 from airflow.utils.task_group import TaskGroup
 
+from cosmos import cache, settings
 from cosmos.airflow.graph import build_airflow_graph
 from cosmos.config import ExecutionConfig, ProfileConfig, ProjectConfig, RenderConfig
 from cosmos.constants import ExecutionMode
 from cosmos.dbt.graph import DbtGraph
 from cosmos.dbt.selector import retrieve_by_label
 from cosmos.exceptions import CosmosValueError
 from cosmos.log import get_logger
@@ -53,15 +54,15 @@
     Extract kwargs specific to the Airflow DAG or TaskGroup class initialization method.
 
     :param kwargs: kwargs which can contain Airflow DAG or TaskGroup and cosmos.converter.DbtToAirflowConverter kwargs.
     """
     new_kwargs = {}
     non_airflow_kwargs = specific_kwargs(**kwargs)
     for arg_key, arg_value in kwargs.items():
-        if arg_key not in non_airflow_kwargs:
+        if arg_key not in non_airflow_kwargs or arg_key == "dag":
             new_kwargs[arg_key] = arg_value
     return new_kwargs
 
 
 def validate_arguments(
     select: list[str],
     exclude: list[str],
@@ -210,51 +211,45 @@
 
         execution_config = execution_config or ExecutionConfig()
         render_config = render_config or RenderConfig()
         operator_args = operator_args or {}
 
         validate_initial_user_config(execution_config, profile_config, project_config, render_config, operator_args)
 
-        # If we are using the old interface, we should migrate it to the new interface
-        # This is safe to do now since we have validated which config interface we're using
         if project_config.dbt_project_path:
             execution_config, render_config = migrate_to_new_interface(execution_config, project_config, render_config)
 
         validate_adapted_user_config(execution_config, project_config, render_config)
 
         env_vars = project_config.env_vars or operator_args.get("env")
         dbt_vars = project_config.dbt_vars or operator_args.get("vars")
 
-        # Previously, we were creating a cosmos.dbt.project.DbtProject
-        # DbtProject has now been replaced with ProjectConfig directly
-        #   since the interface of the two classes were effectively the same
-        # Under this previous implementation, we were passing:
-        #  - name, root dir, models dir, snapshots dir and manifest path
-        # Internally in the dbtProject class, we were defaulting the profile_path
-        #   To be root dir/profiles.yml
-        # To keep this logic working, if converter is given no ProfileConfig,
-        #   we can create a default retaining this value to preserve this functionality.
-        # We may want to consider defaulting this value in our actual ProjceConfig class?
-        dbt_graph = DbtGraph(
+        cache_dir = None
+        if settings.enable_cache:
+            cache_dir = cache._obtain_cache_dir_path(cache_identifier=cache._create_cache_identifier(dag, task_group))
+
+        self.dbt_graph = DbtGraph(
             project=project_config,
             render_config=render_config,
             execution_config=execution_config,
             profile_config=profile_config,
+            cache_dir=cache_dir,
             dbt_vars=dbt_vars,
         )
-        dbt_graph.load(method=render_config.load_method, execution_mode=execution_config.execution_mode)
+        self.dbt_graph.load(method=render_config.load_method, execution_mode=execution_config.execution_mode)
 
         task_args = {
             **operator_args,
             "project_dir": execution_config.project_path,
             "partial_parse": project_config.partial_parse,
             "profile_config": profile_config,
             "emit_datasets": render_config.emit_datasets,
             "env": env_vars,
             "vars": dbt_vars,
+            "cache_dir": cache_dir,
         }
         if execution_config.dbt_executable_path:
             task_args["dbt_executable_path"] = execution_config.dbt_executable_path
         if execution_config.invocation_mode:
             task_args["invocation_mode"] = execution_config.invocation_mode
 
         validate_arguments(
@@ -262,15 +257,15 @@
             render_config.exclude,
             profile_config,
             task_args,
             execution_mode=execution_config.execution_mode,
         )
 
         build_airflow_graph(
-            nodes=dbt_graph.filtered_nodes,
+            nodes=self.dbt_graph.filtered_nodes,
             dag=dag or (task_group and task_group.dag),
             task_group=task_group,
             execution_mode=execution_config.execution_mode,
             task_args=task_args,
             test_indirect_selection=execution_config.test_indirect_selection,
             dbt_project_name=project_config.project_name,
             on_warning_callback=on_warning_callback,
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/log.py` & `astronomer_cosmos-1.4.0a2/cosmos/log.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/airflow/dag.py` & `astronomer_cosmos-1.4.0a2/cosmos/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/airflow/graph.py` & `astronomer_cosmos-1.4.0a2/cosmos/airflow/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/airflow/task_group.py` & `astronomer_cosmos-1.4.0a2/cosmos/airflow/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/core/airflow.py` & `astronomer_cosmos-1.4.0a2/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.4.0a2/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/dbt/graph.py` & `astronomer_cosmos-1.4.0a2/cosmos/dbt/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from subprocess import PIPE, Popen
 from typing import Any
 
 import yaml
 
+from cosmos import cache
 from cosmos.config import ExecutionConfig, ProfileConfig, ProjectConfig, RenderConfig
 from cosmos.constants import (
     DBT_LOG_DIR_NAME,
     DBT_LOG_FILENAME,
     DBT_LOG_PATH_ENVVAR,
     DBT_TARGET_DIR_NAME,
     DBT_TARGET_PATH_ENVVAR,
     DbtResourceType,
     ExecutionMode,
     LoadMode,
 )
 from cosmos.dbt.parser.project import LegacyDbtProject
-from cosmos.dbt.project import copy_msgpack_for_partial_parse, create_symlinks, environ
+from cosmos.dbt.project import create_symlinks, environ, get_partial_parse_path
 from cosmos.dbt.selector import select_nodes
 from cosmos.log import get_logger
 
 logger = get_logger(__name__)
 
 
 class CosmosLoadDbtException(Exception):
@@ -69,15 +70,15 @@
         """
         return self.resource_name.replace(".", "_")
 
 
 def run_command(command: list[str], tmp_dir: Path, env_vars: dict[str, str]) -> str:
     """Run a command in a subprocess, returning the stdout."""
     logger.info("Running command: `%s`", " ".join(command))
-    logger.info("Environment variable keys: %s", env_vars.keys())
+    logger.debug("Environment variable keys: %s", env_vars.keys())
     process = Popen(
         command,
         stdout=PIPE,
         stderr=PIPE,
         cwd=tmp_dir,
         universal_newlines=True,
         env=env_vars,
@@ -132,21 +133,23 @@
 
     def __init__(
         self,
         project: ProjectConfig,
         render_config: RenderConfig = RenderConfig(),
         execution_config: ExecutionConfig = ExecutionConfig(),
         profile_config: ProfileConfig | None = None,
+        cache_dir: Path | None = None,
         # dbt_vars only supported for LegacyDbtProject
         dbt_vars: dict[str, str] | None = None,
     ):
         self.project = project
         self.render_config = render_config
         self.profile_config = profile_config
         self.execution_config = execution_config
+        self.cache_dir = cache_dir
         self.dbt_vars = dbt_vars or {}
 
     def load(
         self,
         method: LoadMode = LoadMode.AUTOMATIC,
         execution_mode: ExecutionMode = ExecutionMode.LOCAL,
     ) -> None:
@@ -246,22 +249,27 @@
             raise CosmosLoadDbtException("Unable to load project via dbt ls without a profile config.")
 
         with tempfile.TemporaryDirectory() as tmpdir:
             logger.info(
                 f"Content of the dbt project dir {self.render_config.project_path}: `{os.listdir(self.render_config.project_path)}`"
             )
             tmpdir_path = Path(tmpdir)
-            create_symlinks(self.render_config.project_path, tmpdir_path, self.render_config.dbt_deps)
 
-            if self.project.partial_parse:
-                copy_msgpack_for_partial_parse(self.render_config.project_path, tmpdir_path)
+            abs_project_path = self.render_config.project_path.absolute()
+            create_symlinks(abs_project_path, tmpdir_path, self.render_config.dbt_deps)
 
-            with self.profile_config.ensure_profile(use_mock_values=True) as profile_values, environ(
-                self.project.env_vars or self.render_config.env_vars or {}
-            ):
+            if self.project.partial_parse and self.cache_dir:
+                latest_partial_parse = cache._get_latest_partial_parse(abs_project_path, self.cache_dir)
+                logger.info("Partial parse is enabled and the latest partial parse file is %s", latest_partial_parse)
+                if latest_partial_parse is not None:
+                    cache._copy_partial_parse_to_project(latest_partial_parse, tmpdir_path)
+
+            with self.profile_config.ensure_profile(
+                use_mock_values=self.render_config.enable_mock_profile
+            ) as profile_values, environ(self.project.env_vars or self.render_config.env_vars or {}):
                 (profile_path, env_vars) = profile_values
                 env = os.environ.copy()
                 env.update(env_vars)
 
                 self.local_flags = [
                     "--project-dir",
                     str(tmpdir),
@@ -284,14 +292,19 @@
                     logger.debug("dbt deps output: %s", stdout)
 
                 nodes = self.run_dbt_ls(dbt_cmd, self.execution_config.project_path, tmpdir_path, env)
 
                 self.nodes = nodes
                 self.filtered_nodes = nodes
 
+            if self.project.partial_parse and self.cache_dir:
+                partial_parse_file = get_partial_parse_path(tmpdir_path)
+                if partial_parse_file.exists():
+                    cache._update_partial_parse_cache(partial_parse_file, self.cache_dir)
+
     def load_via_dbt_ls_file(self) -> None:
         """
         This is between dbt ls and full manifest. It allows to use the output (needs to be json output) of the dbt ls as a
         file stored in the image you run Cosmos on. The advantage is that you can use the parser from LoadMode.DBT_LS without
         actually running dbt ls every time. BUT you will need one dbt ls file for each separate group.
 
         This technically should increase performance and also removes the necessity to have your whole dbt project copied
@@ -418,15 +431,15 @@
                 nodes=nodes,
                 select=self.render_config.select,
                 exclude=self.render_config.exclude,
             )
 
     def update_node_dependency(self) -> None:
         """
-        This will update the property `has_text` if node has `dbt` test
+        This will update the property `has_test` if node has `dbt` test
 
         Updates in-place:
         * self.filtered_nodes
         """
         for _, node in self.filtered_nodes.items():
             if node.resource_type == DbtResourceType.TEST:
                 for node_id in node.depends_on:
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/dbt/project.py` & `astronomer_cosmos-1.4.0a2/cosmos/dbt/project.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,19 @@
         # this is linked to dbt deps so if dbt deps is true then ignore existing dbt_packages folder
         ignore_paths.append("dbt_packages")
     for child_name in os.listdir(project_path):
         if child_name not in ignore_paths:
             os.symlink(project_path / child_name, tmp_dir / child_name)
 
 
-def copy_msgpack_for_partial_parse(project_path: Path, tmp_dir: Path) -> None:
-    partial_parse_file = Path(project_path) / DBT_TARGET_DIR_NAME / DBT_PARTIAL_PARSE_FILE_NAME
-
-    if partial_parse_file.exists():
-        tmp_target_dir = tmp_dir / DBT_TARGET_DIR_NAME
-        tmp_target_dir.mkdir(exist_ok=True)
-
-        shutil.copy(str(partial_parse_file), str(tmp_target_dir / DBT_PARTIAL_PARSE_FILE_NAME))
+def get_partial_parse_path(project_dir_path: Path) -> Path:
+    """
+    Return the partial parse (partial_parse.msgpack) path for a given dbt project directory.
+    """
+    return project_dir_path / DBT_TARGET_DIR_NAME / DBT_PARTIAL_PARSE_FILE_NAME
 
 
 @contextmanager
 def environ(env_vars: dict[str, str]) -> Generator[None, None, None]:
     """Temporarily set environment variables inside the context manager and restore
     when exiting.
     """
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/dbt/selector.py` & `astronomer_cosmos-1.4.0a2/cosmos/dbt/selector.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.4.0a2/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/dbt/parser/project.py` & `astronomer_cosmos-1.4.0a2/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.4.0a2/cosmos/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/operators/__init__.py` & `astronomer_cosmos-1.4.0a2/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/operators/azure_container_instance.py` & `astronomer_cosmos-1.4.0a2/cosmos/operators/azure_container_instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 except ImportError:
     raise ImportError(
         "Could not import AzureContainerInstancesOperator. Ensure you've installed the Microsoft Azure provider "
         "separately or with `pip install astronomer-cosmos[...,azure-container-instance]`."
     )
 
 
-class DbtAzureContainerInstanceBaseOperator(AzureContainerInstancesOperator, AbstractDbtBaseOperator):  # type: ignore
+class DbtAzureContainerInstanceBaseOperator(AbstractDbtBaseOperator, AzureContainerInstancesOperator):  # type: ignore
     """
     Executes a dbt core cli command in an Azure Container Instance
     """
 
     template_fields: Sequence[str] = tuple(
         list(AbstractDbtBaseOperator.template_fields) + list(AzureContainerInstancesOperator.template_fields)
     )
@@ -62,70 +62,70 @@
             registry_conn_id=registry_conn_id,
             **kwargs,
         )
 
     def build_and_run_cmd(self, context: Context, cmd_flags: list[str] | None = None) -> None:
         self.build_command(context, cmd_flags)
         self.log.info(f"Running command: {self.command}")
-        result = super().execute(context)
+        result = AzureContainerInstancesOperator.execute(self, context)
         logger.info(result)
 
     def build_command(self, context: Context, cmd_flags: list[str] | None = None) -> None:
         # For the first round, we're going to assume that the command is dbt
         # This means that we don't have openlineage support, but we will create a ticket
         # to add that in the future
         self.dbt_executable_path = "dbt"
         dbt_cmd, env_vars = self.build_cmd(context=context, cmd_flags=cmd_flags)
         self.environment_variables: dict[str, Any] = {**env_vars, **self.environment_variables}
         self.command: list[str] = dbt_cmd
 
 
-class DbtLSAzureContainerInstanceOperator(DbtLSMixin, DbtAzureContainerInstanceBaseOperator):
+class DbtLSAzureContainerInstanceOperator(DbtLSMixin, DbtAzureContainerInstanceBaseOperator):  # type: ignore
     """
     Executes a dbt core ls command.
     """
 
 
-class DbtSeedAzureContainerInstanceOperator(DbtSeedMixin, DbtAzureContainerInstanceBaseOperator):
+class DbtSeedAzureContainerInstanceOperator(DbtSeedMixin, DbtAzureContainerInstanceBaseOperator):  # type: ignore
     """
     Executes a dbt core seed command.
 
     :param full_refresh: dbt optional arg - dbt will treat incremental models as table models
     """
 
     template_fields: Sequence[str] = DbtAzureContainerInstanceBaseOperator.template_fields + DbtRunMixin.template_fields  # type: ignore[operator]
 
 
-class DbtSnapshotAzureContainerInstanceOperator(DbtSnapshotMixin, DbtAzureContainerInstanceBaseOperator):
+class DbtSnapshotAzureContainerInstanceOperator(DbtSnapshotMixin, DbtAzureContainerInstanceBaseOperator):  # type: ignore
     """
     Executes a dbt core snapshot command.
 
     """
 
 
-class DbtRunAzureContainerInstanceOperator(DbtRunMixin, DbtAzureContainerInstanceBaseOperator):
+class DbtRunAzureContainerInstanceOperator(DbtRunMixin, DbtAzureContainerInstanceBaseOperator):  # type: ignore
     """
     Executes a dbt core run command.
     """
 
     template_fields: Sequence[str] = DbtAzureContainerInstanceBaseOperator.template_fields + DbtRunMixin.template_fields  # type: ignore[operator]
 
 
-class DbtTestAzureContainerInstanceOperator(DbtTestMixin, DbtAzureContainerInstanceBaseOperator):
+class DbtTestAzureContainerInstanceOperator(DbtTestMixin, DbtAzureContainerInstanceBaseOperator):  # type: ignore
     """
     Executes a dbt core test command.
     """
 
     def __init__(self, on_warning_callback: Callable[..., Any] | None = None, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         # as of now, on_warning_callback in azure container instance executor does nothing
         self.on_warning_callback = on_warning_callback
 
 
-class DbtRunOperationAzureContainerInstanceOperator(DbtRunOperationMixin, DbtAzureContainerInstanceBaseOperator):
+class DbtRunOperationAzureContainerInstanceOperator(DbtRunOperationMixin, DbtAzureContainerInstanceBaseOperator):  # type: ignore
     """
     Executes a dbt core run-operation command.
 
     :param macro_name: name of macro to execute
     :param args: Supply arguments to the macro. This dictionary will be mapped to the keyword arguments defined in the
         selected macro.
     """
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/operators/base.py` & `astronomer_cosmos-1.4.0a2/cosmos/operators/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 import os
 from abc import ABCMeta, abstractmethod
+from functools import cached_property
+from pathlib import Path
 from typing import Any, Sequence, Tuple
 
 import yaml
 from airflow.models.baseoperator import BaseOperator
 from airflow.utils.context import Context
 from airflow.utils.operator_helpers import context_to_airflow_vars
 from airflow.utils.strings import to_boolean
 
+from cosmos import cache
 from cosmos.dbt.executable import get_system_dbt
 from cosmos.log import get_logger
 
 logger = get_logger(__name__)
 
 
 class AbstractDbtBaseOperator(BaseOperator, metaclass=ABCMeta):
@@ -39,31 +42,33 @@
     :param warn_error: dbt optional argument to convert dbt warnings into errors
     :param db_name: override the target db instead of the one supplied in the airflow connection
     :param schema: override the target schema instead of the one supplied in the airflow connection
     :param env: If env is not None, it must be a dict that defines the
         environment variables for the new process; these are used instead
         of inheriting the current process environment, which is the default
         behavior. (templated)
-    :param append_env: If False(default) uses the environment variables passed in env params
-        and does not inherit the current process environment. If True, inherits the environment variables
+    :param append_env: . If True (default), inherits the environment variables
         from current passes and then environment variable passed by the user will either update the existing
-        inherited environment variables or the new variables gets appended to it
+        inherited environment variables or the new variables gets appended to it.
+        If False, only uses the environment variables passed in env params
+        and does not inherit the current process environment.
     :param output_encoding: Output encoding of bash command
     :param skip_exit_code: If task exits with this exit code, leave the task
         in ``skipped`` state (default: 99). If set to ``None``, any non-zero
         exit code will be treated as a failure.
     :param partial_parse: If True (default), then the operator will use the
         ``partial_parse.msgpack`` during execution if it exists. If False, then
         a flag will be explicitly set to turn off partial parsing.
     :param cancel_query_on_kill: If true, then cancel any running queries when the task's on_kill() is executed.
         Otherwise, the query will keep running when the task is killed.
     :param dbt_executable_path: Path to dbt executable can be used with venv
         (i.e. /home/astro/.pyenv/versions/dbt_venv/bin/dbt)
     :param dbt_cmd_flags: List of flags to pass to dbt command
     :param dbt_cmd_global_flags: List of dbt global flags to be passed to the dbt command
+    :param cache_dir: Directory used to cache Cosmos/dbt artifacts in Airflow worker nodes
     """
 
     template_fields: Sequence[str] = ("env", "select", "exclude", "selector", "vars", "models")
     global_flags = (
         "project_dir",
         "select",
         "exclude",
@@ -95,22 +100,23 @@
         no_version_check: bool = False,
         fail_fast: bool = False,
         quiet: bool = False,
         warn_error: bool = False,
         db_name: str | None = None,
         schema: str | None = None,
         env: dict[str, Any] | None = None,
-        append_env: bool = False,
+        append_env: bool = True,
         output_encoding: str = "utf-8",
         skip_exit_code: int = 99,
         partial_parse: bool = True,
         cancel_query_on_kill: bool = True,
         dbt_executable_path: str = get_system_dbt(),
         dbt_cmd_flags: list[str] | None = None,
         dbt_cmd_global_flags: list[str] | None = None,
+        cache_dir: Path | None = None,
         **kwargs: Any,
     ) -> None:
         self.project_dir = project_dir
         self.conn_id = conn_id
         self.select = select
         self.exclude = exclude
         self.selector = selector
@@ -130,14 +136,15 @@
         self.output_encoding = output_encoding
         self.skip_exit_code = skip_exit_code
         self.partial_parse = partial_parse
         self.cancel_query_on_kill = cancel_query_on_kill
         self.dbt_executable_path = dbt_executable_path
         self.dbt_cmd_flags = dbt_cmd_flags
         self.dbt_cmd_global_flags = dbt_cmd_global_flags or []
+        self.cache_dir = cache_dir
         super().__init__(**kwargs)
 
     def get_env(self, context: Context) -> dict[str, str | bytes | os.PathLike[Any]]:
         """
         Builds the set of environment variables to be exposed for the bash command.
 
         The order of determination is:
@@ -190,25 +197,36 @@
         for global_flag in self.global_flags:
             # for now, skip the project_dir flag
             if global_flag == "project_dir":
                 continue
 
             dbt_name = f"--{global_flag.replace('_', '-')}"
             global_flag_value = self.__getattribute__(global_flag)
-            if global_flag_value is not None:
-                if isinstance(global_flag_value, dict):
-                    yaml_string = yaml.dump(global_flag_value)
-                    flags.extend([dbt_name, yaml_string])
-                else:
-                    flags.extend([dbt_name, str(global_flag_value)])
+            flags.extend(self._process_global_flag(dbt_name, global_flag_value))
+
         for global_boolean_flag in self.global_boolean_flags:
             if self.__getattribute__(global_boolean_flag):
                 flags.append(f"--{global_boolean_flag.replace('_', '-')}")
         return flags
 
+    @staticmethod
+    def _process_global_flag(flag_name: str, flag_value: Any) -> list[str]:
+        """Helper method to process global flags and reduce complexity."""
+        if flag_value is None:
+            return []
+        elif isinstance(flag_value, dict):
+            yaml_string = yaml.dump(flag_value)
+            return [flag_name, yaml_string]
+        elif isinstance(flag_value, list) and flag_value:
+            return [flag_name, " ".join(flag_value)]
+        elif isinstance(flag_value, list):
+            return []
+        else:
+            return [flag_name, str(flag_value)]
+
     def add_cmd_flags(self) -> list[str]:
         """Allows subclasses to override to add flags for their dbt command"""
         return []
 
     def build_cmd(
         self,
         context: Context,
@@ -368,26 +386,14 @@
         **kwargs: Any,
     ) -> None:
         self.select = select
         self.exclude = exclude
         self.selector = selector
         super().__init__(exclude=exclude, select=select, selector=selector, **kwargs)  # type: ignore
 
-    def add_cmd_flags(self) -> list[str]:
-        flags = []
-        if self.exclude:
-            flags.extend(["--exclude", *self.exclude])
-
-        if self.select:
-            flags.extend(["--select", *self.select])
-
-        if self.selector:
-            flags.extend(["--selector", self.selector])
-        return flags
-
 
 class DbtRunOperationMixin:
     """
     Mixin for dbt run operation command.
 
     :param macro_name: name of macro to execute
     :param args: Supply arguments to the macro. This dictionary will be mapped to the keyword arguments defined in the
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/operators/docker.py` & `astronomer_cosmos-1.4.0a2/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.4.0a2/cosmos/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/operators/local.py` & `astronomer_cosmos-1.4.0a2/cosmos/operators/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowSkipException
 from airflow.models.taskinstance import TaskInstance
 from airflow.utils.context import Context
 from airflow.utils.session import NEW_SESSION, create_session, provide_session
 from attr import define
 
+from cosmos import cache
 from cosmos.constants import InvocationMode
+from cosmos.dbt.project import get_partial_parse_path
 
 try:
     from airflow.datasets import Dataset
     from openlineage.common.provider.dbt.local import DbtLocalArtifactProcessor
 except ModuleNotFoundError:
     is_openlineage_available = False
     DbtLocalArtifactProcessor = None
@@ -45,15 +47,15 @@
 )
 from cosmos.dbt.parser.output import (
     extract_dbt_runner_issues,
     extract_log_issues,
     parse_number_of_warnings_dbt_runner,
     parse_number_of_warnings_subprocess,
 )
-from cosmos.dbt.project import change_working_directory, copy_msgpack_for_partial_parse, create_symlinks, environ
+from cosmos.dbt.project import change_working_directory, create_symlinks, environ
 from cosmos.hooks.subprocess import (
     FullOutputSubprocessHook,
     FullOutputSubprocessResult,
 )
 from cosmos.log import get_logger
 from cosmos.operators.base import (
     AbstractDbtBaseOperator,
@@ -257,15 +259,14 @@
             )
 
         if self._dbt_runner is None:
             self._dbt_runner = dbtRunner()
 
         # Exclude the dbt executable path from the command
         cli_args = command[1:]
-
         logger.info("Trying to run dbtRunner with:\n %s\n in %s", cli_args, cwd)
 
         with change_working_directory(cwd), environ(env):
             result = self._dbt_runner.invoke(cli_args)
 
         return result
 
@@ -278,30 +279,37 @@
         """
         Copies the dbt project to a temporary directory and runs the command.
         """
         if not self.invocation_mode:
             self._discover_invocation_mode()
 
         with tempfile.TemporaryDirectory() as tmp_project_dir:
+
             logger.info(
                 "Cloning project to writable temp directory %s from %s",
                 tmp_project_dir,
                 self.project_dir,
             )
+            tmp_dir_path = Path(tmp_project_dir)
             env = {k: str(v) for k, v in env.items()}
-            create_symlinks(Path(self.project_dir), Path(tmp_project_dir), self.install_deps)
+            create_symlinks(Path(self.project_dir), tmp_dir_path, self.install_deps)
 
-            if self.partial_parse:
-                copy_msgpack_for_partial_parse(Path(self.project_dir), Path(tmp_project_dir))
+            if self.partial_parse and self.cache_dir is not None:
+                latest_partial_parse = cache._get_latest_partial_parse(Path(self.project_dir), self.cache_dir)
+                logger.info("Partial parse is enabled and the latest partial parse file is %s", latest_partial_parse)
+                if latest_partial_parse is not None:
+                    cache._copy_partial_parse_to_project(latest_partial_parse, tmp_dir_path)
 
             with self.profile_config.ensure_profile() as profile_values:
                 (profile_path, env_vars) = profile_values
                 env.update(env_vars)
 
                 flags = [
+                    "--project-dir",
+                    str(tmp_project_dir),
                     "--profiles-dir",
                     str(profile_path.parent),
                     "--profile",
                     self.profile_config.profile_name,
                     "--target",
                     self.profile_config.target_name,
                 ]
@@ -313,33 +321,39 @@
                         command=deps_command,
                         env=env,
                         cwd=tmp_project_dir,
                     )
 
                 full_cmd = cmd + flags
 
-                logger.info("Using environment variables keys: %s", env.keys())
+                logger.debug("Using environment variables keys: %s", env.keys())
+
                 result = self.invoke_dbt(
                     command=full_cmd,
                     env=env,
                     cwd=tmp_project_dir,
                 )
                 if is_openlineage_available:
-                    self.calculate_openlineage_events_completes(env, Path(tmp_project_dir))
+                    self.calculate_openlineage_events_completes(env, tmp_dir_path)
                     context[
                         "task_instance"
                     ].openlineage_events_completes = self.openlineage_events_completes  # type: ignore
 
                 if self.emit_datasets:
                     inlets = self.get_datasets("inputs")
                     outlets = self.get_datasets("outputs")
                     logger.info("Inlets: %s", inlets)
                     logger.info("Outlets: %s", outlets)
                     self.register_dataset(inlets, outlets)
 
+                if self.partial_parse and self.cache_dir:
+                    partial_parse_file = get_partial_parse_path(tmp_dir_path)
+                    if partial_parse_file.exists():
+                        cache._update_partial_parse_cache(partial_parse_file, self.cache_dir)
+
                 self.store_compiled_sql(tmp_project_dir, context)
                 self.handle_exception(result)
                 if self.callback:
                     self.callback(tmp_project_dir)
 
                 return result
 
@@ -564,27 +578,29 @@
 class DbtDocsLocalOperator(DbtLocalBaseOperator):
     """
     Executes `dbt docs generate` command.
     Use the `callback` parameter to specify a callback function to run after the command completes.
     """
 
     ui_color = "#8194E0"
-    required_files = ["index.html", "manifest.json", "graph.gpickle", "catalog.json"]
+    required_files = ["index.html", "manifest.json", "catalog.json"]
     base_cmd = ["docs", "generate"]
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self.check_static_flag()
 
     def check_static_flag(self) -> None:
-        flag = "--static"
         if self.dbt_cmd_flags:
-            if flag in self.dbt_cmd_flags:
+            if "--static" in self.dbt_cmd_flags:
                 # For the --static flag we only upload the generated static_index.html file
                 self.required_files = ["static_index.html"]
+        if self.dbt_cmd_global_flags:
+            if "--no-write-json" in self.dbt_cmd_global_flags and "graph.gpickle" in self.required_files:
+                self.required_files.remove("graph.gpickle")
 
 
 class DbtDocsCloudLocalOperator(DbtDocsLocalOperator, ABC):
     """
     Abstract class for operators that upload the generated documentation to cloud storage.
     """
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.4.0a2/cosmos/operators/virtualenv.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,49 +33,53 @@
 class DbtVirtualenvBaseOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core cli command within a Python Virtual Environment, that is created before running the dbt command
     and deleted at the end of the operator execution.
 
     :param py_requirements: If defined, creates a virtual environment with the specified dependencies. Example:
            ["dbt-postgres==1.5.0"]
+    :param pip_install_options: Pip options to use when installing Python dependencies. Example: ["--upgrade", "--no-cache-dir"]
     :param py_system_site_packages: Whether or not all the Python packages from the Airflow instance will be accessible
            within the virtual environment (if py_requirements argument is specified).
            Avoid using unless the dbt job requires it.
     """
 
     def __init__(
         self,
         py_requirements: list[str] | None = None,
+        pip_install_options: list[str] | None = None,
         py_system_site_packages: bool = False,
         **kwargs: Any,
     ) -> None:
         self.py_requirements = py_requirements or []
+        self.pip_install_options = pip_install_options or []
         self.py_system_site_packages = py_system_site_packages
         super().__init__(**kwargs)
         self._venv_tmp_dir: None | TemporaryDirectory[str] = None
 
     @cached_property
     def venv_dbt_path(
         self,
     ) -> str:
         """
         Path to the dbt binary within a Python virtualenv.
 
         The first time this property is called, it creates a virtualenv and installs the dependencies based on the
-        self.py_requirements and self.py_system_site_packages. This value is cached for future calls.
+        self.py_requirements, self.pip_install_options, and self.py_system_site_packages. This value is cached for future calls.
         """
         # We are reusing the virtualenv directory for all subprocess calls within this task/operator.
         # For this reason, we are not using contexts at this point.
         # The deletion of this directory is done explicitly at the end of the `execute` method.
         self._venv_tmp_dir = TemporaryDirectory(prefix="cosmos-venv")
         py_interpreter = prepare_virtualenv(
             venv_directory=self._venv_tmp_dir.name,
             python_bin=PY_INTERPRETER,
             system_site_packages=self.py_system_site_packages,
             requirements=self.py_requirements,
+            pip_install_options=self.pip_install_options,
         )
         dbt_binary = Path(py_interpreter).parent / "dbt"
         cmd_output = self.subprocess_hook.run_command(
             [
                 py_interpreter,
                 "-c",
                 "from importlib.metadata import version; print(version('dbt-core'))",
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/plugin/__init__.py` & `astronomer_cosmos-1.4.0a2/cosmos/plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     heightCalculationMethod: function getHeight() {
       return Math.max(
         // Overview page
         getMaxElement('bottom', 'div.panel.panel-default') + 50,
         // Model page
         getMaxElement('bottom', 'section.section') + 75,
         // Search page
-        getMaxElement('bottom', 'div.result-body') + 110
+        getMaxElement('bottom', 'div.result-body') + 125
       )
     }
   }
 </script>
 """
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/plugin/static/iframeResizer.contentWindow.min.js` & `astronomer_cosmos-1.4.0a2/cosmos/plugin/static/iframeResizer.contentWindow.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/plugin/static/iframeResizer.min.js` & `astronomer_cosmos-1.4.0a2/cosmos/plugin/static/iframeResizer.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/__init__.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/base.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,26 @@
             profile_contents["config"] = self.dbt_config_vars.as_dict()
 
         if self.disable_event_tracking:
             profile_contents["config"] = {"send_anonymous_usage_stats": False}
 
         return str(yaml.dump(profile_contents, indent=4))
 
+    def _get_airflow_conn_field(self, airflow_field: str) -> Any:
+        # make sure there's no "extra." prefix
+        if airflow_field.startswith("extra."):
+            airflow_field = airflow_field.replace("extra.", "", 1)
+            value = self.conn.extra_dejson.get(airflow_field)
+        elif airflow_field.startswith("extra__"):
+            value = self.conn.extra_dejson.get(airflow_field)
+        else:
+            value = getattr(self.conn, airflow_field, None)
+
+        return value
+
     def get_dbt_value(self, name: str) -> Any:
         """
         Gets values for the dbt profile based on the required_by_dbt and required_in_profile_args lists.
         Precedence is:
         1. profile_args
         2. conn
         """
@@ -256,24 +268,17 @@
         if name in self.airflow_param_mapping:
             airflow_fields = self.airflow_param_mapping[name]
 
             if isinstance(airflow_fields, str):
                 airflow_fields = [airflow_fields]
 
             for airflow_field in airflow_fields:
-                # make sure there's no "extra." prefix
-                if airflow_field.startswith("extra."):
-                    airflow_field = airflow_field.replace("extra.", "", 1)
-                    value = self.conn.extra_dejson.get(airflow_field)
-                else:
-                    value = getattr(self.conn, airflow_field, None)
-
+                value = self._get_airflow_conn_field(airflow_field)
                 if not value:
                     continue
-
                 # if there's a transform method, use it
                 if hasattr(self, f"transform_{name}"):
                     return getattr(self, f"transform_{name}")(value)
 
                 return value
 
         # otherwise, we don't have it - return None
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/athena/access_key.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/athena/access_key.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/bigquery/oauth.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/oauth.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/bigquery/service_account_keyfile_dict.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/service_account_keyfile_dict.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/snowflake/__init__.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/snowflake/user_privatekey.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_privatekey.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,24 +9,27 @@
 class TrinoBaseProfileMapping(BaseProfileMapping):
     "Maps common fields for Airflow Trino connections to dbt profiles."
 
     airflow_connection_type: str = "trino"
     dbt_profile_type: str = "trino"
     is_community: bool = True
 
-    required_fields = [
+    base_fields = [
         "host",
         "database",
         "schema",
         "port",
     ]
 
+    required_fields = base_fields + ["user"]
+
     airflow_param_mapping = {
         "host": "host",
         "port": "port",
+        "user": "login",
         "session_properties": "extra.session_properties",
     }
 
     @property
     def profile(self) -> dict[str, Any]:
         "Gets profile."
         profile_vars = {
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/certificate.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Maps Airflow Trino connections to Certificate Trino dbt profiles.
     https://docs.getdbt.com/reference/warehouse-setups/trino-setup#certificate
     https://airflow.apache.org/docs/apache-airflow-providers-trino/stable/connections.html
     """
 
     dbt_profile_method: str = "certificate"
 
-    required_fields = TrinoBaseProfileMapping.required_fields + [
+    required_fields = TrinoBaseProfileMapping.base_fields + [
         "client_certificate",
         "client_private_key",
     ]
 
     airflow_param_mapping = {
         "client_certificate": "extra.certs__client_cert_path",
         "client_private_key": "extra.certs__client_key_path",
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/jwt.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     https://docs.getdbt.com/reference/warehouse-setups/trino-setup#jwt
     https://airflow.apache.org/docs/apache-airflow-providers-trino/stable/connections.html
     """
 
     dbt_profile_method: str = "jwt"
 
-    required_fields = TrinoBaseProfileMapping.required_fields + [
+    required_fields = TrinoBaseProfileMapping.base_fields + [
         "jwt_token",
     ]
     secret_fields = [
         "jwt_token",
     ]
     airflow_param_mapping = {
         "jwt_token": "extra.jwt__token",
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/ldap.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     https://docs.getdbt.com/reference/warehouse-setups/trino-setup#ldap
     https://airflow.apache.org/docs/apache-airflow-providers-trino/stable/connections.html
     """
 
     dbt_profile_method: str = "ldap"
 
-    required_fields = TrinoBaseProfileMapping.required_fields + [
+    required_fields = TrinoBaseProfileMapping.base_fields + [
         "user",
         "password",
     ]
     secret_fields = [
         "password",
     ]
     airflow_param_mapping = {
```

### Comparing `astronomer_cosmos-1.4.0a1/cosmos/profiles/vertica/user_pass.py` & `astronomer_cosmos-1.4.0a2/cosmos/profiles/vertica/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/.gitignore` & `astronomer_cosmos-1.4.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/LICENSE` & `astronomer_cosmos-1.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/README.rst` & `astronomer_cosmos-1.4.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a1/pyproject.toml` & `astronomer_cosmos-1.4.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -195,11 +195,11 @@
 no_warn_unused_ignores = true
 
 [tool.ruff]
 line-length = 120
 [tool.ruff.lint]
 select = ["C901", "I"]
 [tool.ruff.lint.mccabe]
-max-complexity = 8
+max-complexity = 10
 
 [tool.distutils.bdist_wheel]
 universal = true
```

### Comparing `astronomer_cosmos-1.4.0a1/PKG-INFO` & `astronomer_cosmos-1.4.0a2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: astronomer-cosmos
-Version: 1.4.0a1
+Version: 1.4.0a2
 Summary: Orchestrate your dbt projects in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://astronomer.github.io/astronomer-cosmos
 Project-URL: Source code, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -27,16 +27,25 @@
 Requires-Dist: apache-airflow>=2.3.0
 Requires-Dist: attrs
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: virtualenv
 Provides-Extra: all
-Requires-Dist: astronomer-cosmos[dbt-all]; extra == 'all'
-Requires-Dist: astronomer-cosmos[openlineage]; extra == 'all'
+Requires-Dist: dbt-athena; extra == 'all'
+Requires-Dist: dbt-bigquery; extra == 'all'
+Requires-Dist: dbt-databricks; extra == 'all'
+Requires-Dist: dbt-exasol; extra == 'all'
+Requires-Dist: dbt-postgres; extra == 'all'
+Requires-Dist: dbt-redshift; extra == 'all'
+Requires-Dist: dbt-snowflake; extra == 'all'
+Requires-Dist: dbt-spark; extra == 'all'
+Requires-Dist: dbt-vertica; extra == 'all'
+Requires-Dist: openlineage-airflow; extra == 'all'
+Requires-Dist: openlineage-integration-common; extra == 'all'
 Provides-Extra: azure-container-instance
 Requires-Dist: apache-airflow-providers-microsoft-azure>=8.4.0; extra == 'azure-container-instance'
 Provides-Extra: dbt-all
 Requires-Dist: dbt-athena; extra == 'dbt-all'
 Requires-Dist: dbt-bigquery; extra == 'dbt-all'
 Requires-Dist: dbt-databricks; extra == 'dbt-all'
 Requires-Dist: dbt-exasol; extra == 'dbt-all'
```

