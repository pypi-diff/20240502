# Comparing `tmp/python_dev_utils-1.6.0.tar.gz` & `tmp/python_dev_utils-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-1.6.0.tar", last modified: Sat Apr 27 11:39:12 2024, max compression
+gzip compressed data, was "python_dev_utils-1.7.0.tar", last modified: Thu May  2 08:14:58 2024, max compression
```

## Comparing `python_dev_utils-1.6.0.tar` & `python_dev_utils-1.7.0.tar`

### file list

```diff
@@ -1,90 +1,91 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.6.0/LICENCE
--rw-r--r--   0        0        0     5120 2024-04-23 09:09:42.701197 python_dev_utils-1.6.0/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.6.0/dev_utils/__init__.py
--rw-r--r--   0        0        0      407 2024-04-27 11:38:00.638361 python_dev_utils-1.6.0/dev_utils/alembic/__init__.py
--rw-r--r--   0        0        0     1688 2024-04-27 11:26:29.918706 python_dev_utils-1.6.0/dev_utils/alembic/ignore_table.py
--rw-r--r--   0        0        0      921 2024-04-25 13:19:12.947590 python_dev_utils-1.6.0/dev_utils/alembic/migration_numbering.py
--rw-r--r--   0        0        0      892 2024-04-27 09:22:42.892410 python_dev_utils-1.6.0/dev_utils/alembic/utils.py
--rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.6.0/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.6.0/dev_utils/core/abstract.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.6.0/dev_utils/core/exc.py
--rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.6.0/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.6.0/dev_utils/core/logging.py
--rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.6.0/dev_utils/core/results.py
--rw-r--r--   0        0        0      462 2024-04-27 11:37:02.853641 python_dev_utils-1.6.0/dev_utils/core/utils/__init__.py
--rw-r--r--   0        0        0      265 2024-04-26 08:51:43.164520 python_dev_utils-1.6.0/dev_utils/core/utils/datetime.py
--rw-r--r--   0        0        0     1040 2024-04-27 11:36:17.853859 python_dev_utils-1.6.0/dev_utils/core/utils/envs.py
--rw-r--r--   0        0        0      766 2024-04-27 11:36:37.669763 python_dev_utils-1.6.0/dev_utils/core/utils/humanize.py
--rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.6.0/dev_utils/core/utils/inspect.py
--rw-r--r--   0        0        0     1578 2024-04-27 11:36:52.604691 python_dev_utils-1.6.0/dev_utils/core/utils/strings.py
--rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.6.0/dev_utils/fastapi/__init__.py
--rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.6.0/dev_utils/fastapi/middlewares/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.6.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
--rw-r--r--   0        0        0        0 2024-04-22 08:05:13.247824 python_dev_utils-1.6.0/dev_utils/fastapi/openapi/__init__.py
--rw-r--r--   0        0        0     1901 2024-04-23 07:13:12.131657 python_dev_utils-1.6.0/dev_utils/fastapi/openapi/exporter.py
--rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py
--rw-r--r--   0        0        0     3474 2024-04-22 09:15:05.523504 python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/constants.py
--rw-r--r--   0        0        0    12499 2024-04-22 09:09:07.827456 python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/exc.py
--rw-r--r--   0        0        0     3724 2024-04-22 13:05:32.395150 python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py
--rw-r--r--   0        0        0     2184 2024-04-22 12:42:55.028588 python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/openapi_override.py
--rw-r--r--   0        0        0     1265 2024-04-22 09:31:33.905990 python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/utils.py
--rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.6.0/dev_utils/py.typed
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.6.0/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.6.0/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.6.0/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.6.0/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.6.0/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.6.0/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.6.0/dev_utils/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.6.0/dev_utils/sqlalchemy/mixins/audit.py
--rw-r--r--   0        0        0     1187 2024-04-25 09:18:45.437647 python_dev_utils-1.6.0/dev_utils/sqlalchemy/mixins/base.py
--rw-r--r--   0        0        0     6474 2024-04-26 09:53:43.191401 python_dev_utils-1.6.0/dev_utils/sqlalchemy/mixins/general.py
--rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.6.0/dev_utils/sqlalchemy/mixins/ids.py
--rw-r--r--   0        0        0     1005 2024-04-25 11:36:06.219628 python_dev_utils-1.6.0/dev_utils/sqlalchemy/naming_conventions.py
--rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.6.0/dev_utils/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.6.0/dev_utils/sqlalchemy/profiling/containers.py
--rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.6.0/dev_utils/sqlalchemy/profiling/profilers.py
--rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.6.0/dev_utils/sqlalchemy/profiling/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.6.0/dev_utils/sqlalchemy/types/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-16 07:24:43.054226 python_dev_utils-1.6.0/dev_utils/sqlalchemy/types/datetime.py
--rw-r--r--   0        0        0    14281 2024-04-25 13:17:22.836564 python_dev_utils-1.6.0/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0     3263 2024-04-27 11:39:12.764012 python_dev_utils-1.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.6.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 06:25:13.597435 python_dev_utils-1.6.0/tests/alembic/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-27 11:29:42.045776 python_dev_utils-1.6.0/tests/alembic/test_ignore_table.py
--rw-r--r--   0        0        0      772 2024-04-26 09:16:01.643863 python_dev_utils-1.6.0/tests/alembic/test_migration_numbering.py
--rw-r--r--   0        0        0      746 2024-04-27 11:15:08.238156 python_dev_utils-1.6.0/tests/alembic/test_utils.py
--rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.6.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.6.0/tests/core/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.6.0/tests/core/test_abstract.py
--rw-r--r--   0        0        0      393 2024-04-27 09:47:42.911786 python_dev_utils-1.6.0/tests/core/test_datetime_utils.py
--rw-r--r--   0        0        0     3152 2024-04-27 10:11:57.366723 python_dev_utils-1.6.0/tests/core/test_env_utils.py
--rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.6.0/tests/core/test_guards.py
--rw-r--r--   0        0        0     1485 2024-04-27 10:11:40.278820 python_dev_utils-1.6.0/tests/core/test_humanize_utils.py
--rw-r--r--   0        0        0      487 2024-04-27 09:48:27.358654 python_dev_utils-1.6.0/tests/core/test_inspect_utils.py
--rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.6.0/tests/core/test_results.py
--rw-r--r--   0        0        0     1258 2024-04-27 11:01:55.517321 python_dev_utils-1.6.0/tests/core/test_strings_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.6.0/tests/fastapi/__init__.py
--rw-r--r--   0        0        0     1409 2024-04-22 12:43:33.722241 python_dev_utils-1.6.0/tests/fastapi/conftest.py
--rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.6.0/tests/fastapi/test_middlewares.py
--rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.6.0/tests/fastapi/test_verbose_http_exceptions.py
--rw-r--r--   0        0        0     2074 2024-04-22 12:16:38.058690 python_dev_utils-1.6.0/tests/fastapi/test_verbose_http_exceptions_handlers.py
--rw-r--r--   0        0        0     1609 2024-04-22 13:12:15.337384 python_dev_utils-1.6.0/tests/fastapi/test_verbose_http_exceptions_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.6.0/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.6.0/tests/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.6.0/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.6.0/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.6.0/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.6.0/tests/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.6.0/tests/sqlalchemy/mixins/test_audit.py
--rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.6.0/tests/sqlalchemy/mixins/test_base.py
--rw-r--r--   0        0        0     7544 2024-04-26 09:36:52.825485 python_dev_utils-1.6.0/tests/sqlalchemy/mixins/test_general.py
--rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.6.0/tests/sqlalchemy/mixins/test_ids.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.6.0/tests/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.6.0/tests/sqlalchemy/profiling/test_profilers.py
--rw-r--r--   0        0        0      394 2024-04-26 09:26:06.714312 python_dev_utils-1.6.0/tests/sqlalchemy/test_naming_conventions.py
--rw-r--r--   0        0        0     1423 2024-04-22 12:17:27.599234 python_dev_utils-1.6.0/tests/sqlalchemy/test_types.py
--rw-r--r--   0        0        0     9789 2024-04-25 13:18:24.229021 python_dev_utils-1.6.0/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.6.0/tests/types.py
--rw-r--r--   0        0        0     7683 2024-04-25 12:36:46.358159 python_dev_utils-1.6.0/tests/utils.py
--rw-r--r--   0        0        0     5914 1970-01-01 00:00:00.000000 python_dev_utils-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.7.0/LICENCE
+-rw-r--r--   0        0        0     5125 2024-05-02 07:22:44.512284 python_dev_utils-1.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.7.0/dev_utils/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-27 11:38:00.638361 python_dev_utils-1.7.0/dev_utils/alembic/__init__.py
+-rw-r--r--   0        0        0     1688 2024-04-27 11:26:29.918706 python_dev_utils-1.7.0/dev_utils/alembic/ignore_table.py
+-rw-r--r--   0        0        0      921 2024-04-25 13:19:12.947590 python_dev_utils-1.7.0/dev_utils/alembic/migration_numbering.py
+-rw-r--r--   0        0        0      892 2024-04-27 09:22:42.892410 python_dev_utils-1.7.0/dev_utils/alembic/utils.py
+-rw-r--r--   0        0        0        0 2024-05-01 13:16:34.515756 python_dev_utils-1.7.0/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.7.0/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.7.0/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.7.0/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.7.0/dev_utils/core/logging.py
+-rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.7.0/dev_utils/core/results.py
+-rw-r--r--   0        0        0      662 2024-05-01 13:15:58.588972 python_dev_utils-1.7.0/dev_utils/core/utils/__init__.py
+-rw-r--r--   0        0        0      265 2024-04-26 08:51:43.164520 python_dev_utils-1.7.0/dev_utils/core/utils/datetime.py
+-rw-r--r--   0        0        0     1040 2024-04-27 11:36:17.853859 python_dev_utils-1.7.0/dev_utils/core/utils/envs.py
+-rw-r--r--   0        0        0      766 2024-04-27 11:36:37.669763 python_dev_utils-1.7.0/dev_utils/core/utils/humanize.py
+-rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.7.0/dev_utils/core/utils/inspect.py
+-rw-r--r--   0        0        0     1578 2024-04-27 11:36:52.604691 python_dev_utils-1.7.0/dev_utils/core/utils/strings.py
+-rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.7.0/dev_utils/fastapi/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.7.0/dev_utils/fastapi/middlewares/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.7.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
+-rw-r--r--   0        0        0        0 2024-04-22 08:05:13.247824 python_dev_utils-1.7.0/dev_utils/fastapi/openapi/__init__.py
+-rw-r--r--   0        0        0     1901 2024-04-23 07:13:12.131657 python_dev_utils-1.7.0/dev_utils/fastapi/openapi/exporter.py
+-rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py
+-rw-r--r--   0        0        0     3474 2024-04-22 09:15:05.523504 python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/constants.py
+-rw-r--r--   0        0        0    12499 2024-04-22 09:09:07.827456 python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/exc.py
+-rw-r--r--   0        0        0     3724 2024-04-22 13:05:32.395150 python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py
+-rw-r--r--   0        0        0     2184 2024-04-22 12:42:55.028588 python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/openapi_override.py
+-rw-r--r--   0        0        0     1265 2024-04-22 09:31:33.905990 python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.7.0/dev_utils/py.typed
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.7.0/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.7.0/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.7.0/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.7.0/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.7.0/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.7.0/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.7.0/dev_utils/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     4138 2024-05-02 07:47:31.057832 python_dev_utils-1.7.0/dev_utils/sqlalchemy/mixins/audit.py
+-rw-r--r--   0        0        0     1261 2024-04-30 19:40:08.223220 python_dev_utils-1.7.0/dev_utils/sqlalchemy/mixins/base.py
+-rw-r--r--   0        0        0     8096 2024-05-02 07:17:04.053247 python_dev_utils-1.7.0/dev_utils/sqlalchemy/mixins/general.py
+-rw-r--r--   0        0        0     1229 2024-04-30 19:48:16.754203 python_dev_utils-1.7.0/dev_utils/sqlalchemy/mixins/ids.py
+-rw-r--r--   0        0        0     1005 2024-04-25 11:36:06.219628 python_dev_utils-1.7.0/dev_utils/sqlalchemy/naming_conventions.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.7.0/dev_utils/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.7.0/dev_utils/sqlalchemy/profiling/containers.py
+-rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.7.0/dev_utils/sqlalchemy/profiling/profilers.py
+-rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.7.0/dev_utils/sqlalchemy/profiling/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.7.0/dev_utils/sqlalchemy/types/__init__.py
+-rw-r--r--   0        0        0     2457 2024-05-01 11:31:16.251129 python_dev_utils-1.7.0/dev_utils/sqlalchemy/types/datetime.py
+-rw-r--r--   0        0        0     3348 2024-05-02 06:36:14.437004 python_dev_utils-1.7.0/dev_utils/sqlalchemy/types/pydantic.py
+-rw-r--r--   0        0        0    14281 2024-04-25 13:17:22.836564 python_dev_utils-1.7.0/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0     3290 2024-05-02 08:14:58.426977 python_dev_utils-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 06:25:13.597435 python_dev_utils-1.7.0/tests/alembic/__init__.py
+-rw-r--r--   0        0        0     1256 2024-04-27 11:29:42.045776 python_dev_utils-1.7.0/tests/alembic/test_ignore_table.py
+-rw-r--r--   0        0        0      772 2024-04-26 09:16:01.643863 python_dev_utils-1.7.0/tests/alembic/test_migration_numbering.py
+-rw-r--r--   0        0        0      746 2024-04-27 11:15:08.238156 python_dev_utils-1.7.0/tests/alembic/test_utils.py
+-rw-r--r--   0        0        0     9331 2024-05-02 06:38:31.027987 python_dev_utils-1.7.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.7.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.7.0/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      393 2024-04-27 09:47:42.911786 python_dev_utils-1.7.0/tests/core/test_datetime_utils.py
+-rw-r--r--   0        0        0     3152 2024-04-27 10:11:57.366723 python_dev_utils-1.7.0/tests/core/test_env_utils.py
+-rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.7.0/tests/core/test_guards.py
+-rw-r--r--   0        0        0     1485 2024-04-27 10:11:40.278820 python_dev_utils-1.7.0/tests/core/test_humanize_utils.py
+-rw-r--r--   0        0        0      487 2024-04-27 09:48:27.358654 python_dev_utils-1.7.0/tests/core/test_inspect_utils.py
+-rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.7.0/tests/core/test_results.py
+-rw-r--r--   0        0        0     1258 2024-04-27 11:01:55.517321 python_dev_utils-1.7.0/tests/core/test_strings_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.7.0/tests/fastapi/__init__.py
+-rw-r--r--   0        0        0     1409 2024-04-22 12:43:33.722241 python_dev_utils-1.7.0/tests/fastapi/conftest.py
+-rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.7.0/tests/fastapi/test_middlewares.py
+-rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.7.0/tests/fastapi/test_verbose_http_exceptions.py
+-rw-r--r--   0        0        0     2074 2024-04-22 12:16:38.058690 python_dev_utils-1.7.0/tests/fastapi/test_verbose_http_exceptions_handlers.py
+-rw-r--r--   0        0        0     1609 2024-04-22 13:12:15.337384 python_dev_utils-1.7.0/tests/fastapi/test_verbose_http_exceptions_utils.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.7.0/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.7.0/tests/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.7.0/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.7.0/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.7.0/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.7.0/tests/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.7.0/tests/sqlalchemy/mixins/test_audit.py
+-rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.7.0/tests/sqlalchemy/mixins/test_base.py
+-rw-r--r--   0        0        0     8627 2024-05-02 07:18:33.212683 python_dev_utils-1.7.0/tests/sqlalchemy/mixins/test_general.py
+-rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.7.0/tests/sqlalchemy/mixins/test_ids.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.7.0/tests/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.7.0/tests/sqlalchemy/profiling/test_profilers.py
+-rw-r--r--   0        0        0      394 2024-04-26 09:26:06.714312 python_dev_utils-1.7.0/tests/sqlalchemy/test_naming_conventions.py
+-rw-r--r--   0        0        0     4407 2024-05-02 06:53:17.265549 python_dev_utils-1.7.0/tests/sqlalchemy/test_types.py
+-rw-r--r--   0        0        0     9789 2024-04-25 13:18:24.229021 python_dev_utils-1.7.0/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.7.0/tests/types.py
+-rw-r--r--   0        0        0     8004 2024-05-02 06:53:23.154533 python_dev_utils-1.7.0/tests/utils.py
+-rw-r--r--   0        0        0     5919 1970-01-01 00:00:00.000000 python_dev_utils-1.7.0/PKG-INFO
```

### Comparing `python_dev_utils-1.6.0/LICENCE` & `python_dev_utils-1.7.0/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/README.md` & `python_dev_utils-1.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Dev utils
 
 ![coverage](./coverage.svg)
 
 ## For what?
 
 I made this project to avoid copy-pasting with utils in my projects. I was aiming to simplify
-working with sqlalchemy, FastAPI and other libs.
+working with sqlalchemy, FastAPI and other libraries.
 
 ## Install
 
 Package has optional dependencies, so if you use it in some specific cases, install only needed
 dependencies.
 
 For profiling:
```

### Comparing `python_dev_utils-1.6.0/dev_utils/alembic/ignore_table.py` & `python_dev_utils-1.7.0/dev_utils/alembic/ignore_table.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/alembic/migration_numbering.py` & `python_dev_utils-1.7.0/dev_utils/alembic/migration_numbering.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/alembic/utils.py` & `python_dev_utils-1.7.0/dev_utils/alembic/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/core/abstract.py` & `python_dev_utils-1.7.0/dev_utils/core/abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/core/exc.py` & `python_dev_utils-1.7.0/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/core/guards.py` & `python_dev_utils-1.7.0/dev_utils/core/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/core/logging.py` & `python_dev_utils-1.7.0/dev_utils/core/logging.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/core/results.py` & `python_dev_utils-1.7.0/dev_utils/core/results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/core/utils/envs.py` & `python_dev_utils-1.7.0/dev_utils/core/utils/envs.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/core/utils/humanize.py` & `python_dev_utils-1.7.0/dev_utils/core/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/core/utils/inspect.py` & `python_dev_utils-1.7.0/dev_utils/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/core/utils/strings.py` & `python_dev_utils-1.7.0/dev_utils/core/utils/strings.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/fastapi/__init__.py` & `python_dev_utils-1.7.0/dev_utils/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py` & `python_dev_utils-1.7.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/fastapi/openapi/exporter.py` & `python_dev_utils-1.7.0/dev_utils/fastapi/openapi/exporter.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py` & `python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/constants.py` & `python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/constants.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/exc.py` & `python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py` & `python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/openapi_override.py` & `python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/openapi_override.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/fastapi/verbose_http_exceptions/utils.py` & `python_dev_utils-1.7.0/dev_utils/fastapi/verbose_http_exceptions/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/filters/converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/filters/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/filters/operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/filters/types.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/filters/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/mixins/base.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/mixins/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, TypeGuard
 
+from sqlalchemy.orm.decl_api import declarative_mixin
+
 from dev_utils.core.exc import NoDeclarativeModelError
 from dev_utils.core.utils import get_object_class_absolute_name
 from dev_utils.sqlalchemy.utils import is_declarative
 
 if TYPE_CHECKING:
     from sqlalchemy.orm.decl_api import DeclarativeBase
     from sqlalchemy.orm.mapper import Mapper
 
 
+@declarative_mixin
 class BaseModelMixin:
     """Base model mixin."""
 
     @cached_property
     def _is_mixin_in_declarative_model(self) -> "TypeGuard[Mapper[Any]]":  # type: ignore
         return any(is_declarative(class_) for class_ in self.__class__.mro())
```

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/mixins/general.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/mixins/general.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import re
 from typing import TYPE_CHECKING, Any, ClassVar, TypeAlias
 
+from sqlalchemy.orm.decl_api import declarative_mixin, declared_attr
+
 from dev_utils.core.logging import logger
 from dev_utils.core.utils.inspect import get_object_class_absolute_name
 from dev_utils.sqlalchemy.mixins.base import BaseModelMixin
 from dev_utils.sqlalchemy.utils import (
     get_model_instance_data_as_dict,
     get_unloaded_fields,
     get_valid_field_names,
@@ -11,14 +14,15 @@
 
 if TYPE_CHECKING:
     from sqlalchemy.orm.decl_api import DeclarativeBase
 
     DictStrAny: TypeAlias = dict[str, Any]
 
 
+@declarative_mixin
 class DictConverterMixin(BaseModelMixin):
     """Mixin for converting models to dict."""
 
     def _replace(
         self,
         item: dict[str, Any],
         **replace: str,
@@ -45,14 +49,15 @@
         available_fields = valid_fields - exclude_fields
         item: dict[str, Any] = {field: self._get_instance_attr(field) for field in available_fields}
         replace = {key: value for key, value in replace.items() if key in item}
         self._replace(item, **replace)
         return item
 
 
+@declarative_mixin
 class DifferenceMixin(BaseModelMixin):
     """Mixin for checking difference between instance and other objects.
 
     It will not override double underscore methods like __eq__ or other to avoid Incorrect behavior.
     """
 
     safe_difference_flag: ClassVar[bool] = False
@@ -134,14 +139,15 @@
             return self._is_model_different_from(item, exclude)
         if self.safe_difference_flag:
             return True
         msg = f"Incorrect item. Ожидались: Dict, {self.__class__.__name__}. Got: {type(item)}."
         raise TypeError(msg)
 
 
+@declarative_mixin
 class BetterReprMixin(BaseModelMixin):
     """Mixin with better __repr__ method for SQLAlchemy model instances."""
 
     use_full_class_path: ClassVar[bool] = False
     max_repr_elements: ClassVar[int | None] = None
     repr_include_fields: ClassVar[set[str] | None] = None
 
@@ -165,7 +171,49 @@
         class_name = (
             get_object_class_absolute_name(self)
             if self.use_full_class_path
             else self.__class__.__name__
         )
         values_pairs = ", ".join(values_pairs_list)
         return f"{class_name}({values_pairs})"
+
+
+@declarative_mixin
+class TableNameMixin(BaseModelMixin):
+    """Mixin for auto-creation of model table name (__tablename__).
+
+    You may pass class-level attribute ``__join_application_prefix__`` to make mixin create
+    table names with application prefix. For example, if your model class ``User`` with
+    TableNameMixin is located in ``application/models/users.py`` file, your tablename will be
+    ``users_user``.
+    """
+
+    __join_application_prefix__: ClassVar[bool] = False
+
+    @classmethod
+    def _get_model_application_name(cls) -> str:
+        """Parse current model file and package context to get app name.
+
+        Analog of django table naming: ``app``_``model``.
+        """
+        if cls.__module__ == "__main__":
+            return ''
+        path_parts = cls.__module__.split('.')
+        for ele in path_parts[::-1]:
+            if ele == "models":
+                continue
+            return ele
+        return ''
+
+    @declared_attr.directive
+    @classmethod
+    def __tablename__(cls) -> str:
+        """Infer table name from class name."""
+        name = cls.__name__
+        name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
+        name = re.sub('__([A-Z])', r'_\1', name)
+        name = re.sub('([a-z0-9])([A-Z])', r'\1_\2', name)
+        if cls.__join_application_prefix__ and (
+            (application_name := cls._get_model_application_name()) != ""
+        ):
+            return f'{application_name}_{name.lower()}'
+        return name.lower()
```

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/mixins/ids.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/mixins/ids.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 import uuid
 
 from sqlalchemy import UUID, BigInteger, Integer
-from sqlalchemy.orm import Mapped, declared_attr, mapped_column
+from sqlalchemy.orm import Mapped, mapped_column, synonym
+from sqlalchemy.orm.decl_api import declarative_mixin, declared_attr
 
 from dev_utils.sqlalchemy.mixins.base import BaseModelMixin
 
 
+@declarative_mixin
 class IntegerIDMixin(BaseModelMixin):
     """Integer primary key field (id) mixin."""
 
     @declared_attr
     def id(cls) -> Mapped[int]:
         """Id field."""
         return mapped_column(
             BigInteger().with_variant(Integer, "sqlite"),
             nullable=False,
             unique=True,
             primary_key=True,
             autoincrement=True,
         )
 
+    @declared_attr
+    def pk(cls) -> Mapped[int]:
+        """Synonym for id field."""
+        return synonym("id")
+
 
+@declarative_mixin
 class UUIDMixin(BaseModelMixin):
     """UUID primary key field (id) mixin."""
 
     @declared_attr
     def id(cls) -> Mapped[uuid.UUID]:
         """Id field."""
         return mapped_column(
             UUID(as_uuid=True),
             nullable=False,
             primary_key=True,
             default=uuid.uuid4,
         )
+
+    @declared_attr
+    def pk(cls) -> Mapped[uuid.UUID]:
+        """Synonym for id field."""
+        return synonym("id")
```

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/naming_conventions.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/profiling/containers.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/profiling/containers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/profiling/profilers.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/profiling/profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/profiling/utils.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/profiling/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/types/datetime.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/types/datetime.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,26 +35,34 @@
         return datetime.datetime
 
     def process_result_value(  # noqa: D102
         self: "UTCDateTime",
         value: "datetime.datetime | None",
         dialect: "Dialect",  # noqa
     ) -> "datetime.datetime | None":
-        if isinstance(value, datetime.datetime) and value.tzinfo is None:
-            return value.replace(tzinfo=UTC)
+        if value is None:
+            return value
+        if value.tzinfo is None:
+            return value.replace(tzinfo=datetime.UTC)
         return value
 
     def process_bind_param(  # noqa: D102
         self: "UTCDateTime",
         value: "datetime.datetime | None",
         dialect: "Dialect",  # noqa
     ) -> "datetime.datetime | None":
-        if isinstance(value, datetime.datetime) and value.tzinfo is None:
-            return value.replace(tzinfo=UTC)
-        return value
+        if value is None:
+            return value
+        if value.tzinfo is None:
+            msg = (
+                f'UTCDateTime type requires the tzinfo param to be set in datetime field. '
+                f'{type(value)} was passed.'
+            )
+            raise TypeError(msg)
+        return value.astimezone(datetime.UTC)
 
 
 @compiles(Utcnow, "postgresql")
 def pg_utcnow(type_: Any, compiler: Any, **kwargs: Any) -> str:  # noqa
     """Mapping for Utcnow on postgresql current time func with timezone."""  # noqa: D401
     return "TIMEZONE('utc', CURRENT_TIMESTAMP)"
```

### Comparing `python_dev_utils-1.6.0/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-1.7.0/dev_utils/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/pyproject.toml` & `python_dev_utils-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -167,19 +167,20 @@
     "mimesis>=15.1.0",
     "ipython>=8.22.2",
     "sqlalchemy-utils>=0.41.2",
     "psycopg2-binary>=2.9.9",
     "asyncpg>=0.29.0",
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
+    "pytest-mock>=3.14.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "1.6.0"
+version = "1.7.0"
 description = "My project utils package, that I use in my projects."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
```

### Comparing `python_dev_utils-1.6.0/tests/alembic/test_ignore_table.py` & `python_dev_utils-1.7.0/tests/alembic/test_ignore_table.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/alembic/test_migration_numbering.py` & `python_dev_utils-1.7.0/tests/alembic/test_migration_numbering.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/alembic/test_utils.py` & `python_dev_utils-1.7.0/tests/alembic/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/conftest.py` & `python_dev_utils-1.7.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from sqlalchemy.ext.asyncio import async_scoped_session, async_sessionmaker, create_async_engine
 from sqlalchemy.orm import scoped_session, sessionmaker
 
 from dev_utils.fastapi.middlewares.sqlalchemy_profiling import (
     add_query_counter_middleware,
     add_query_profiling_middleware,
 )
+from dev_utils.sqlalchemy.types.pydantic import json_serializer
 from tests.utils import (
     Base,
     MyModel,
     OtherModel,
     coin_flip,
     create_db,
     create_db_item_async,
@@ -99,27 +100,37 @@
 
 
 @pytest.fixture(scope="session")
 def db_sync_engine(db_sync_url: str) -> "Generator[Engine, None, None]":
     """SQLAlchemy engine session-based fixture."""
     with suppress(SQLAlchemyError):
         create_db(db_sync_url)
-    engine = create_engine(db_sync_url, echo=False, pool_pre_ping=True)
+    engine = create_engine(
+        db_sync_url,
+        echo=False,
+        pool_pre_ping=True,
+        json_serializer=json_serializer,
+    )
     try:
         yield engine
     finally:
         engine.dispose()
     with suppress(SQLAlchemyError):
         destroy_db(db_sync_url)
 
 
 @pytest_asyncio.fixture(scope="session")  # type: ignore
 async def db_async_engine(db_async_url: str) -> "AsyncGenerator[AsyncEngine, None]":  # type: ignore
     """SQLAlchemy engine session-based fixture."""
-    engine = create_async_engine(db_async_url, echo=True, pool_pre_ping=True)
+    engine = create_async_engine(
+        db_async_url,
+        echo=True,
+        pool_pre_ping=True,
+        json_serializer=json_serializer,
+    )
     try:
         yield engine
     finally:
         await engine.dispose()
 
 
 @pytest.fixture(scope="session")
```

### Comparing `python_dev_utils-1.6.0/tests/core/test_abstract.py` & `python_dev_utils-1.7.0/tests/core/test_abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/core/test_env_utils.py` & `python_dev_utils-1.7.0/tests/core/test_env_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/core/test_guards.py` & `python_dev_utils-1.7.0/tests/core/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/core/test_humanize_utils.py` & `python_dev_utils-1.7.0/tests/core/test_humanize_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/core/test_results.py` & `python_dev_utils-1.7.0/tests/core/test_results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/core/test_strings_utils.py` & `python_dev_utils-1.7.0/tests/core/test_strings_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/fastapi/conftest.py` & `python_dev_utils-1.7.0/tests/fastapi/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/fastapi/test_verbose_http_exceptions.py` & `python_dev_utils-1.7.0/tests/fastapi/test_verbose_http_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/fastapi/test_verbose_http_exceptions_handlers.py` & `python_dev_utils-1.7.0/tests/fastapi/test_verbose_http_exceptions_handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/fastapi/test_verbose_http_exceptions_utils.py` & `python_dev_utils-1.7.0/tests/fastapi/test_verbose_http_exceptions_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-1.7.0/tests/sqlalchemy/filters/test_converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/sqlalchemy/filters/test_guards.py` & `python_dev_utils-1.7.0/tests/sqlalchemy/filters/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-1.7.0/tests/sqlalchemy/filters/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/sqlalchemy/mixins/test_audit.py` & `python_dev_utils-1.7.0/tests/sqlalchemy/mixins/test_audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/sqlalchemy/mixins/test_base.py` & `python_dev_utils-1.7.0/tests/sqlalchemy/mixins/test_base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/sqlalchemy/mixins/test_general.py` & `python_dev_utils-1.7.0/tests/sqlalchemy/mixins/test_general.py`

 * *Files 8% similar despite different names*

```diff
@@ -215,7 +215,36 @@
     MyModel.safe_difference_flag = True
     selected_with_unload = await db_async_session.scalar(
         select(MyModel).options(load_only(MyModel.id)),
     )
     assert selected_with_unload, "MyModel instance not found (but it must be in DB)"
     selected_with_unload_repr = repr(selected_with_unload)
     assert "<Not loaded>" in selected_with_unload_repr
+
+
+def test_table_name_auto() -> None:
+    class TableNameModel(
+        general_mixins.TableNameMixin,
+        ids_mixins.IntegerIDMixin,
+        Base,
+    ):  # noqa: D101
+        some_other_attr: Mapped[str]
+
+    assert TableNameModel.__tablename__ == "table_name_model"
+
+
+def test_table_name_with_app_name_auto() -> None:
+    class TableNameWithAppNameModel(
+        general_mixins.TableNameMixin,
+        ids_mixins.IntegerIDMixin,
+        Base,
+    ):  # noqa: D101
+        __join_application_prefix__ = True
+        some_other_attr: Mapped[str]
+
+    assert TableNameWithAppNameModel.__tablename__ == "test_general_table_name_with_app_name_model"
+    TableNameWithAppNameModel.__module__ = '__main__'
+    assert TableNameWithAppNameModel.__tablename__ == "table_name_with_app_name_model"
+    TableNameWithAppNameModel.__module__ = 'models'
+    assert TableNameWithAppNameModel.__tablename__ == "table_name_with_app_name_model"
+    TableNameWithAppNameModel.__module__ = 'users.models'
+    assert TableNameWithAppNameModel.__tablename__ == "users_table_name_with_app_name_model"
```

### Comparing `python_dev_utils-1.6.0/tests/sqlalchemy/profiling/test_profilers.py` & `python_dev_utils-1.7.0/tests/sqlalchemy/profiling/test_profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/sqlalchemy/test_utils.py` & `python_dev_utils-1.7.0/tests/sqlalchemy/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/types.py` & `python_dev_utils-1.7.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.6.0/tests/utils.py` & `python_dev_utils-1.7.0/tests/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.ext.hybrid import hybrid_method, hybrid_property
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column, relationship
 from sqlalchemy_utils import create_database, database_exists, drop_database  # type: ignore
 
 from dev_utils.sqlalchemy.mixins.general import BetterReprMixin, DifferenceMixin
 from dev_utils.sqlalchemy.types.datetime import UTCDateTime
+from dev_utils.sqlalchemy.types.pydantic import PydanticType
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Session
 
@@ -235,8 +236,14 @@
         return self.name + "" + self.other_name
 
 
 class TableWithUTCDT(Base):  # noqa: D101
     __tablename__ = "table_with_UTC_dt"
 
     id: Mapped[int] = mapped_column(primary_key=True)  # noqa
-    dt_field: Mapped[datetime.datetime] = mapped_column(UTCDateTime)
+    dt_field: Mapped[datetime.datetime | None] = mapped_column(UTCDateTime)
+    pydantic_type: Mapped[PydanticTestSchema | None] = mapped_column(
+        PydanticType(PydanticTestSchema),
+    )
+    pydantic_list_type: Mapped[list[PydanticTestSchema] | None] = mapped_column(
+        PydanticType(list[PydanticTestSchema]),
+    )
```

### Comparing `python_dev_utils-1.6.0/PKG-INFO` & `python_dev_utils-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_dev_utils
-Version: 1.6.0
+Version: 1.7.0
 Summary: My project utils package, that I use in my projects.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: fastapi-exceptions
 Provides-Extra: profiling
 Provides-Extra: sqlalchemy-filters
@@ -23,15 +23,15 @@
 # Dev utils
 
 ![coverage](./coverage.svg)
 
 ## For what?
 
 I made this project to avoid copy-pasting with utils in my projects. I was aiming to simplify
-working with sqlalchemy, FastAPI and other libs.
+working with sqlalchemy, FastAPI and other libraries.
 
 ## Install
 
 Package has optional dependencies, so if you use it in some specific cases, install only needed
 dependencies.
 
 For profiling:
```

