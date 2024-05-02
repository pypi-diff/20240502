# Comparing `tmp/djangorestframework-jsonapi-6.1.0.tar.gz` & `tmp/djangorestframework-jsonapi-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-jsonapi-6.1.0.tar", last modified: Fri Aug 25 13:53:37 2023, max compression
+gzip compressed data, was "djangorestframework-jsonapi-7.0.0.tar", last modified: Thu May  2 19:40:57 2024, max compression
```

## Comparing `djangorestframework-jsonapi-6.1.0.tar` & `djangorestframework-jsonapi-7.0.0.tar`

### file list

```diff
@@ -1,161 +1,163 @@
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.991946 djangorestframework-jsonapi-6.1.0/.github/
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.991946 djangorestframework-jsonapi-6.1.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 sao       (1000) sao       (1000)      381 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-6.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 sao       (1000) sao       (1000)      479 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-6.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.991946 djangorestframework-jsonapi-6.1.0/.github/workflows/
--rw-rw-r--   0 sao       (1000) sao       (1000)     2777 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/.github/workflows/codeql-analysis.yml
--rw-rw-r--   0 sao       (1000) sao       (1000)     1457 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/.github/workflows/tests.yml
--rw-r--r--   0 sao       (1000) sao       (1000)      517 2019-01-14 20:37:09.000000 djangorestframework-jsonapi-6.1.0/.gitignore
--rw-rw-r--   0 sao       (1000) sao       (1000)      436 2020-12-11 17:31:52.000000 djangorestframework-jsonapi-6.1.0/.pre-commit-config.yaml
--rw-r--r--   0 sao       (1000) sao       (1000)      453 2020-01-23 17:40:39.000000 djangorestframework-jsonapi-6.1.0/.pyup.yml
--rw-rw-r--   0 sao       (1000) sao       (1000)     1983 2023-06-13 18:48:34.000000 djangorestframework-jsonapi-6.1.0/AUTHORS
--rw-rw-r--   0 sao       (1000) sao       (1000)    20750 2023-08-25 13:53:12.000000 djangorestframework-jsonapi-6.1.0/CHANGELOG.md
--rw-r--r--   0 sao       (1000) sao       (1000)     1331 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-6.1.0/LICENSE
--rw-rw-r--   0 sao       (1000) sao       (1000)      157 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-6.1.0/MANIFEST.in
--rw-rw-r--   0 sao       (1000) sao       (1000)     7690 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/PKG-INFO
--rw-rw-r--   0 sao       (1000) sao       (1000)     6437 2023-06-13 12:55:47.000000 djangorestframework-jsonapi-6.1.0/README.rst
--rw-rw-r--   0 sao       (1000) sao       (1000)      481 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/SECURITY.md
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.991946 djangorestframework-jsonapi-6.1.0/djangorestframework_jsonapi.egg-info/
--rw-r--r--   0 sao       (1000) sao       (1000)     7690 2023-08-25 13:53:36.000000 djangorestframework-jsonapi-6.1.0/djangorestframework_jsonapi.egg-info/PKG-INFO
--rw-r--r--   0 sao       (1000) sao       (1000)     4324 2023-08-25 13:53:36.000000 djangorestframework-jsonapi-6.1.0/djangorestframework_jsonapi.egg-info/SOURCES.txt
--rw-r--r--   0 sao       (1000) sao       (1000)        1 2023-08-25 13:53:36.000000 djangorestframework-jsonapi-6.1.0/djangorestframework_jsonapi.egg-info/dependency_links.txt
--rw-r--r--   0 sao       (1000) sao       (1000)        1 2019-01-14 20:37:33.000000 djangorestframework-jsonapi-6.1.0/djangorestframework_jsonapi.egg-info/not-zip-safe
--rw-r--r--   0 sao       (1000) sao       (1000)      180 2023-08-25 13:53:36.000000 djangorestframework-jsonapi-6.1.0/djangorestframework_jsonapi.egg-info/requires.txt
--rw-r--r--   0 sao       (1000) sao       (1000)       95 2023-08-25 13:53:36.000000 djangorestframework-jsonapi-6.1.0/djangorestframework_jsonapi.egg-info/top_level.txt
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/docs/
--rw-r--r--   0 sao       (1000) sao       (1000)       14 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-6.1.0/docs/.gitignore
--rw-rw-r--   0 sao       (1000) sao       (1000)     2064 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/docs/CONTRIBUTING.md
--rw-rw-r--   0 sao       (1000) sao       (1000)     7490 2021-10-07 17:51:19.000000 djangorestframework-jsonapi-6.1.0/docs/Makefile
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/docs/_static/
--rw-r--r--   0 sao       (1000) sao       (1000)        0 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-6.1.0/docs/_static/.gitkeep
--rw-r--r--   0 sao       (1000) sao       (1000)      187 2019-10-09 11:21:11.000000 djangorestframework-jsonapi-6.1.0/docs/api.rst
--rw-rw-r--   0 sao       (1000) sao       (1000)    10381 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/docs/conf.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     3317 2023-06-13 12:55:47.000000 djangorestframework-jsonapi-6.1.0/docs/getting-started.md
--rw-rw-r--   0 sao       (1000) sao       (1000)      510 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-6.1.0/docs/index.rst
--rw-rw-r--   0 sao       (1000) sao       (1000)     7285 2021-10-07 17:51:19.000000 djangorestframework-jsonapi-6.1.0/docs/make.bat
--rw-rw-r--   0 sao       (1000) sao       (1000)    41454 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-6.1.0/docs/usage.md
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/
--rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-6.1.0/example/__init__.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/api/
--rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-6.1.0/example/api/__init__.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/api/resources/
--rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-6.1.0/example/api/resources/__init__.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     2002 2021-11-30 19:09:29.000000 djangorestframework-jsonapi-6.1.0/example/api/resources/identity.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/api/serializers/
--rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-6.1.0/example/api/serializers/__init__.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1086 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/api/serializers/identity.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      178 2020-11-22 20:50:00.000000 djangorestframework-jsonapi-6.1.0/example/api/serializers/post.py
--rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-6.1.0/example/api/urls.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     3812 2022-01-03 16:22:32.000000 djangorestframework-jsonapi-6.1.0/example/factories.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/fixtures/
--rw-rw-r--   0 sao       (1000) sao       (1000)     6129 2022-01-03 16:22:32.000000 djangorestframework-jsonapi-6.1.0/example/fixtures/blogentry.json
--rw-rw-r--   0 sao       (1000) sao       (1000)     2855 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/example/fixtures/drf_example.json
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/migrations/
--rw-rw-r--   0 sao       (1000) sao       (1000)     5131 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0001_initial.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1248 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0002_taggeditem.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     3839 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0003_polymorphics.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     2076 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0004_auto_20171011_0631.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1638 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0005_auto_20180922_1508.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1582 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0006_auto_20181228_0752.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      404 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0007_artproject_description.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1086 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0008_labresults.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      610 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0009_labresults_author.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      346 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0010_auto_20210714_0809.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      869 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0011_rename_type_author_author_type_and_more.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      453 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/migrations/0012_author_full_name.py
--rw-r--r--   0 sao       (1000) sao       (1000)        0 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-6.1.0/example/migrations/__init__.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     4449 2022-09-06 21:02:11.000000 djangorestframework-jsonapi-6.1.0/example/models.py
--rw-r--r--   0 sao       (1000) sao       (1000)      190 2019-10-02 10:38:51.000000 djangorestframework-jsonapi-6.1.0/example/requirements.txt
--rw-rw-r--   0 sao       (1000) sao       (1000)    12248 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/serializers.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/settings/
--rw-r--r--   0 sao       (1000) sao       (1000)       27 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-6.1.0/example/settings/__init__.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     3157 2023-06-13 12:55:47.000000 djangorestframework-jsonapi-6.1.0/example/settings/dev.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      372 2020-12-28 17:44:42.000000 djangorestframework-jsonapi-6.1.0/example/settings/test.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/templates/
--rw-rw-r--   0 sao       (1000) sao       (1000)      835 2020-10-30 18:13:47.000000 djangorestframework-jsonapi-6.1.0/example/templates/swagger-ui.html
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/tests/
--rw-rw-r--   0 sao       (1000) sao       (1000)     1069 2021-10-22 16:46:01.000000 djangorestframework-jsonapi-6.1.0/example/tests/__init__.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/tests/__snapshots__/
--rw-rw-r--   0 sao       (1000) sao       (1000)     4565 2022-09-06 20:02:55.000000 djangorestframework-jsonapi-6.1.0/example/tests/__snapshots__/test_errors.ambr
--rw-rw-r--   0 sao       (1000) sao       (1000)    37683 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-6.1.0/example/tests/__snapshots__/test_openapi.ambr
--rw-rw-r--   0 sao       (1000) sao       (1000)     1890 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/tests/conftest.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/tests/integration/
--rw-rw-r--   0 sao       (1000) sao       (1000)     1231 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-6.1.0/example/tests/integration/test_browsable_api.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     9297 2023-02-21 06:14:59.000000 djangorestframework-jsonapi-6.1.0/example/tests/integration/test_includes.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1562 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/tests/integration/test_meta.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     7836 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/tests/integration/test_model_resource_name.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     5690 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-6.1.0/example/tests/integration/test_non_paginated_responses.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     3406 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-6.1.0/example/tests/integration/test_pagination.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     9797 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/example/tests/integration/test_polymorphism.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1294 2020-11-22 20:50:00.000000 djangorestframework-jsonapi-6.1.0/example/tests/integration/test_sparse_fieldsets.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     7505 2022-09-06 20:02:55.000000 djangorestframework-jsonapi-6.1.0/example/tests/test_errors.py
--rw-rw-r--   0 sao       (1000) sao       (1000)    26316 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-6.1.0/example/tests/test_filters.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      844 2021-10-22 16:46:01.000000 djangorestframework-jsonapi-6.1.0/example/tests/test_generic_validation.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     4940 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/tests/test_generic_viewset.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     7621 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/example/tests/test_model_viewsets.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     6379 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-6.1.0/example/tests/test_openapi.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     4273 2021-10-10 18:12:54.000000 djangorestframework-jsonapi-6.1.0/example/tests/test_performance.py
--rw-rw-r--   0 sao       (1000) sao       (1000)    10146 2021-12-14 16:42:40.000000 djangorestframework-jsonapi-6.1.0/example/tests/test_serializers.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      723 2020-11-22 20:50:00.000000 djangorestframework-jsonapi-6.1.0/example/tests/test_sideload_resources.py
--rw-rw-r--   0 sao       (1000) sao       (1000)    22292 2023-04-25 15:58:23.000000 djangorestframework-jsonapi-6.1.0/example/tests/test_views.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/example/tests/unit/
--rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-6.1.0/example/tests/unit/__init__.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     5575 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/example/tests/unit/test_default_drf_serializers.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     3428 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/example/tests/unit/test_filter_schema_params.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     4425 2021-10-22 16:46:01.000000 djangorestframework-jsonapi-6.1.0/example/tests/unit/test_renderer_class_methods.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     6444 2022-09-06 20:02:55.000000 djangorestframework-jsonapi-6.1.0/example/tests/unit/test_renderers.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1063 2021-10-22 16:46:01.000000 djangorestframework-jsonapi-6.1.0/example/tests/unit/test_serializer_method_field.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     3211 2022-09-06 20:02:55.000000 djangorestframework-jsonapi-6.1.0/example/urls.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     3427 2023-04-25 15:58:23.000000 djangorestframework-jsonapi-6.1.0/example/urls_test.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      717 2020-11-22 20:50:00.000000 djangorestframework-jsonapi-6.1.0/example/utils.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     7985 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/example/views.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/requirements/
--rw-rw-r--   0 sao       (1000) sao       (1000)       86 2023-06-13 12:55:47.000000 djangorestframework-jsonapi-6.1.0/requirements/requirements-codestyle.txt
--rw-rw-r--   0 sao       (1000) sao       (1000)       58 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/requirements/requirements-documentation.txt
--rw-rw-r--   0 sao       (1000) sao       (1000)       77 2023-06-13 12:55:47.000000 djangorestframework-jsonapi-6.1.0/requirements/requirements-optionals.txt
--rw-rw-r--   0 sao       (1000) sao       (1000)       13 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/requirements/requirements-packaging.txt
--rw-rw-r--   0 sao       (1000) sao       (1000)      125 2023-06-13 12:55:47.000000 djangorestframework-jsonapi-6.1.0/requirements/requirements-testing.txt
--rw-rw-r--   0 sao       (1000) sao       (1000)      614 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-6.1.0/requirements.txt
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/
--rw-rw-r--   0 sao       (1000) sao       (1000)      160 2023-08-25 13:53:12.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/__init__.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      562 2022-09-24 17:22:57.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/compat.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/django_filters/
--rw-r--r--   0 sao       (1000) sao       (1000)       56 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/django_filters/__init__.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     5966 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/django_filters/backends.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1747 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/exceptions.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     4589 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/filters.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     6068 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/metadata.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     3218 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/pagination.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     6645 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/parsers.py
--rw-rw-r--   0 sao       (1000) sao       (1000)    14828 2023-06-13 18:48:34.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/relations.py
--rw-rw-r--   0 sao       (1000) sao       (1000)    26345 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/renderers.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/schemas/
--rw-rw-r--   0 sao       (1000) sao       (1000)        0 2020-10-30 18:13:47.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/schemas/__init__.py
--rw-rw-r--   0 sao       (1000) sao       (1000)    36003 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/schemas/openapi.py
--rw-rw-r--   0 sao       (1000) sao       (1000)    17807 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/serializers.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1600 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/settings.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.991946 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/templates/
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/templates/rest_framework_json_api/
--rw-rw-r--   0 sao       (1000) sao       (1000)      550 2020-11-09 20:27:29.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/templates/rest_framework_json_api/api.html
--rw-rw-r--   0 sao       (1000) sao       (1000)     1503 2020-11-09 20:27:29.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/templates/rest_framework_json_api/includes.html
--rw-rw-r--   0 sao       (1000) sao       (1000)    17436 2023-06-13 18:48:34.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/utils.py
--rw-rw-r--   0 sao       (1000) sao       (1000)    16313 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/rest_framework_json_api/views.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1059 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/setup.cfg
--rwxrwxr-x   0 sao       (1000) sao       (1000)     3412 2023-06-13 12:55:47.000000 djangorestframework-jsonapi-6.1.0/setup.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/tests/
--rw-rw-r--   0 sao       (1000) sao       (1000)        0 2020-11-09 20:15:41.000000 djangorestframework-jsonapi-6.1.0/tests/__init__.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1476 2022-12-19 17:57:16.000000 djangorestframework-jsonapi-6.1.0/tests/conftest.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1357 2022-09-24 17:22:57.000000 djangorestframework-jsonapi-6.1.0/tests/models.py
-drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2023-08-25 13:53:36.995947 djangorestframework-jsonapi-6.1.0/tests/schemas/
--rw-rw-r--   0 sao       (1000) sao       (1000)      409 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-6.1.0/tests/schemas/test_openapi.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1333 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-6.1.0/tests/serializers.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1421 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-6.1.0/tests/test_pagination.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     4172 2022-01-03 16:22:32.000000 djangorestframework-jsonapi-6.1.0/tests/test_parsers.py
--rw-rw-r--   0 sao       (1000) sao       (1000)    10462 2023-06-13 18:48:34.000000 djangorestframework-jsonapi-6.1.0/tests/test_relations.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1825 2023-02-21 06:14:59.000000 djangorestframework-jsonapi-6.1.0/tests/test_serializers.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      437 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-6.1.0/tests/test_settings.py
--rw-rw-r--   0 sao       (1000) sao       (1000)    13027 2023-06-13 18:48:34.000000 djangorestframework-jsonapi-6.1.0/tests/test_utils.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     9209 2023-06-13 18:48:34.000000 djangorestframework-jsonapi-6.1.0/tests/test_views.py
--rw-rw-r--   0 sao       (1000) sao       (1000)      267 2022-09-06 20:02:55.000000 djangorestframework-jsonapi-6.1.0/tests/views.py
--rw-rw-r--   0 sao       (1000) sao       (1000)     1663 2023-06-13 12:55:47.000000 djangorestframework-jsonapi-6.1.0/tox.ini
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.233449 djangorestframework-jsonapi-7.0.0/
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.213448 djangorestframework-jsonapi-7.0.0/.github/
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.213448 djangorestframework-jsonapi-7.0.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 sao       (1000) sao       (1000)      381 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-7.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 sao       (1000) sao       (1000)      479 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-7.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.213448 djangorestframework-jsonapi-7.0.0/.github/workflows/
+-rw-rw-r--   0 sao       (1000) sao       (1000)     2777 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-7.0.0/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1504 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 sao       (1000) sao       (1000)      517 2019-01-14 20:37:09.000000 djangorestframework-jsonapi-7.0.0/.gitignore
+-rw-rw-r--   0 sao       (1000) sao       (1000)      436 2020-12-11 17:31:52.000000 djangorestframework-jsonapi-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 sao       (1000) sao       (1000)      453 2020-01-23 17:40:39.000000 djangorestframework-jsonapi-7.0.0/.pyup.yml
+-rw-rw-r--   0 sao       (1000) sao       (1000)     2026 2023-10-19 11:02:58.000000 djangorestframework-jsonapi-7.0.0/AUTHORS
+-rw-rw-r--   0 sao       (1000) sao       (1000)    21839 2024-05-02 19:40:15.000000 djangorestframework-jsonapi-7.0.0/CHANGELOG.md
+-rw-r--r--   0 sao       (1000) sao       (1000)     1331 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-7.0.0/LICENSE
+-rw-rw-r--   0 sao       (1000) sao       (1000)      157 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-7.0.0/MANIFEST.in
+-rw-rw-r--   0 sao       (1000) sao       (1000)     8061 2024-05-02 19:40:57.233449 djangorestframework-jsonapi-7.0.0/PKG-INFO
+-rw-rw-r--   0 sao       (1000) sao       (1000)     6428 2024-04-18 19:02:48.000000 djangorestframework-jsonapi-7.0.0/README.rst
+-rw-rw-r--   0 sao       (1000) sao       (1000)      481 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-7.0.0/SECURITY.md
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.213448 djangorestframework-jsonapi-7.0.0/djangorestframework_jsonapi.egg-info/
+-rw-r--r--   0 sao       (1000) sao       (1000)     8061 2024-05-02 19:40:57.000000 djangorestframework-jsonapi-7.0.0/djangorestframework_jsonapi.egg-info/PKG-INFO
+-rw-r--r--   0 sao       (1000) sao       (1000)     4415 2024-05-02 19:40:57.000000 djangorestframework-jsonapi-7.0.0/djangorestframework_jsonapi.egg-info/SOURCES.txt
+-rw-r--r--   0 sao       (1000) sao       (1000)        1 2024-05-02 19:40:57.000000 djangorestframework-jsonapi-7.0.0/djangorestframework_jsonapi.egg-info/dependency_links.txt
+-rw-r--r--   0 sao       (1000) sao       (1000)        1 2019-01-14 20:37:33.000000 djangorestframework-jsonapi-7.0.0/djangorestframework_jsonapi.egg-info/not-zip-safe
+-rw-r--r--   0 sao       (1000) sao       (1000)      180 2024-05-02 19:40:57.000000 djangorestframework-jsonapi-7.0.0/djangorestframework_jsonapi.egg-info/requires.txt
+-rw-r--r--   0 sao       (1000) sao       (1000)       95 2024-05-02 19:40:57.000000 djangorestframework-jsonapi-7.0.0/djangorestframework_jsonapi.egg-info/top_level.txt
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.217448 djangorestframework-jsonapi-7.0.0/docs/
+-rw-r--r--   0 sao       (1000) sao       (1000)       14 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-7.0.0/docs/.gitignore
+-rw-rw-r--   0 sao       (1000) sao       (1000)     2064 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-7.0.0/docs/CONTRIBUTING.md
+-rw-rw-r--   0 sao       (1000) sao       (1000)     7490 2021-10-07 17:51:19.000000 djangorestframework-jsonapi-7.0.0/docs/Makefile
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.217448 djangorestframework-jsonapi-7.0.0/docs/_static/
+-rw-r--r--   0 sao       (1000) sao       (1000)        0 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-7.0.0/docs/_static/.gitkeep
+-rw-r--r--   0 sao       (1000) sao       (1000)      187 2019-10-09 11:21:11.000000 djangorestframework-jsonapi-7.0.0/docs/api.rst
+-rw-rw-r--   0 sao       (1000) sao       (1000)    10146 2024-03-20 16:52:18.000000 djangorestframework-jsonapi-7.0.0/docs/conf.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     3308 2024-04-18 19:02:48.000000 djangorestframework-jsonapi-7.0.0/docs/getting-started.md
+-rw-rw-r--   0 sao       (1000) sao       (1000)      510 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-7.0.0/docs/index.rst
+-rw-rw-r--   0 sao       (1000) sao       (1000)     7285 2021-10-07 17:51:19.000000 djangorestframework-jsonapi-7.0.0/docs/make.bat
+-rw-rw-r--   0 sao       (1000) sao       (1000)    41454 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-7.0.0/docs/usage.md
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.217448 djangorestframework-jsonapi-7.0.0/example/
+-rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-7.0.0/example/__init__.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.217448 djangorestframework-jsonapi-7.0.0/example/api/
+-rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-7.0.0/example/api/__init__.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.217448 djangorestframework-jsonapi-7.0.0/example/api/resources/
+-rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-7.0.0/example/api/resources/__init__.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     2002 2021-11-30 19:09:29.000000 djangorestframework-jsonapi-7.0.0/example/api/resources/identity.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.217448 djangorestframework-jsonapi-7.0.0/example/api/serializers/
+-rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-7.0.0/example/api/serializers/__init__.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1086 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/api/serializers/identity.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      178 2020-11-22 20:50:00.000000 djangorestframework-jsonapi-7.0.0/example/api/serializers/post.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-7.0.0/example/api/urls.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     4512 2023-09-22 06:24:47.000000 djangorestframework-jsonapi-7.0.0/example/factories.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.217448 djangorestframework-jsonapi-7.0.0/example/fixtures/
+-rw-rw-r--   0 sao       (1000) sao       (1000)     6129 2022-01-03 16:22:32.000000 djangorestframework-jsonapi-7.0.0/example/fixtures/blogentry.json
+-rw-rw-r--   0 sao       (1000) sao       (1000)     2855 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-7.0.0/example/fixtures/drf_example.json
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.221449 djangorestframework-jsonapi-7.0.0/example/migrations/
+-rw-rw-r--   0 sao       (1000) sao       (1000)     5131 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0001_initial.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1248 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0002_taggeditem.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     3839 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0003_polymorphics.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     2076 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0004_auto_20171011_0631.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1638 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0005_auto_20180922_1508.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1582 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0006_auto_20181228_0752.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      404 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0007_artproject_description.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1086 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0008_labresults.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      610 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0009_labresults_author.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      346 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0010_auto_20210714_0809.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      869 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0011_rename_type_author_author_type_and_more.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      453 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0012_author_full_name.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      747 2023-09-19 05:52:27.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0013_questionnaire.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      420 2023-09-19 05:52:27.000000 djangorestframework-jsonapi-7.0.0/example/migrations/0014_questionnaire_metadata.py
+-rw-r--r--   0 sao       (1000) sao       (1000)        0 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-7.0.0/example/migrations/__init__.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     4599 2023-09-19 05:52:27.000000 djangorestframework-jsonapi-7.0.0/example/models.py
+-rw-r--r--   0 sao       (1000) sao       (1000)      190 2019-10-02 10:38:51.000000 djangorestframework-jsonapi-7.0.0/example/requirements.txt
+-rw-rw-r--   0 sao       (1000) sao       (1000)    12837 2024-04-19 21:45:30.000000 djangorestframework-jsonapi-7.0.0/example/serializers.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.221449 djangorestframework-jsonapi-7.0.0/example/settings/
+-rw-r--r--   0 sao       (1000) sao       (1000)       27 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-7.0.0/example/settings/__init__.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     3157 2023-06-13 12:55:47.000000 djangorestframework-jsonapi-7.0.0/example/settings/dev.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      372 2020-12-28 17:44:42.000000 djangorestframework-jsonapi-7.0.0/example/settings/test.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.221449 djangorestframework-jsonapi-7.0.0/example/templates/
+-rw-rw-r--   0 sao       (1000) sao       (1000)      835 2020-10-30 18:13:47.000000 djangorestframework-jsonapi-7.0.0/example/templates/swagger-ui.html
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.225449 djangorestframework-jsonapi-7.0.0/example/tests/
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1069 2021-10-22 16:46:01.000000 djangorestframework-jsonapi-7.0.0/example/tests/__init__.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.225449 djangorestframework-jsonapi-7.0.0/example/tests/__snapshots__/
+-rw-rw-r--   0 sao       (1000) sao       (1000)     4589 2023-09-22 06:24:47.000000 djangorestframework-jsonapi-7.0.0/example/tests/__snapshots__/test_errors.ambr
+-rw-rw-r--   0 sao       (1000) sao       (1000)    37707 2023-09-22 06:24:47.000000 djangorestframework-jsonapi-7.0.0/example/tests/__snapshots__/test_openapi.ambr
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1947 2023-09-19 05:52:27.000000 djangorestframework-jsonapi-7.0.0/example/tests/conftest.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.225449 djangorestframework-jsonapi-7.0.0/example/tests/integration/
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1231 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-7.0.0/example/tests/integration/test_browsable_api.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     7099 2024-04-19 21:39:16.000000 djangorestframework-jsonapi-7.0.0/example/tests/integration/test_includes.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1562 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/tests/integration/test_meta.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     7836 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/tests/integration/test_model_resource_name.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     5694 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/example/tests/integration/test_non_paginated_responses.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     3408 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/example/tests/integration/test_pagination.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     9774 2023-09-22 06:24:47.000000 djangorestframework-jsonapi-7.0.0/example/tests/integration/test_polymorphism.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1325 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/example/tests/integration/test_sparse_fieldsets.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     7505 2022-09-06 20:02:55.000000 djangorestframework-jsonapi-7.0.0/example/tests/test_errors.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    26318 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/example/tests/test_filters.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      844 2021-10-22 16:46:01.000000 djangorestframework-jsonapi-7.0.0/example/tests/test_generic_validation.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     4940 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/tests/test_generic_viewset.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     7621 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-7.0.0/example/tests/test_model_viewsets.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     7697 2023-09-19 05:52:27.000000 djangorestframework-jsonapi-7.0.0/example/tests/test_openapi.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     4273 2024-04-19 21:39:34.000000 djangorestframework-jsonapi-7.0.0/example/tests/test_performance.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    11332 2023-09-19 05:52:27.000000 djangorestframework-jsonapi-7.0.0/example/tests/test_serializers.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      724 2024-03-18 17:34:31.000000 djangorestframework-jsonapi-7.0.0/example/tests/test_sideload_resources.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    22292 2023-04-25 15:58:23.000000 djangorestframework-jsonapi-7.0.0/example/tests/test_views.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.229449 djangorestframework-jsonapi-7.0.0/example/tests/unit/
+-rw-rw-r--   0 sao       (1000) sao       (1000)        0 2017-05-30 08:48:17.000000 djangorestframework-jsonapi-7.0.0/example/tests/unit/__init__.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     5575 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/example/tests/unit/test_default_drf_serializers.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     3428 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-7.0.0/example/tests/unit/test_filter_schema_params.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     4397 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/example/tests/unit/test_renderer_class_methods.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     6556 2024-03-05 06:06:09.000000 djangorestframework-jsonapi-7.0.0/example/tests/unit/test_renderers.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1063 2021-10-22 16:46:01.000000 djangorestframework-jsonapi-7.0.0/example/tests/unit/test_serializer_method_field.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     3294 2023-09-19 05:52:27.000000 djangorestframework-jsonapi-7.0.0/example/urls.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     3508 2024-04-18 19:02:48.000000 djangorestframework-jsonapi-7.0.0/example/urls_test.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      717 2020-11-22 20:50:00.000000 djangorestframework-jsonapi-7.0.0/example/utils.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     8328 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/example/views.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.229449 djangorestframework-jsonapi-7.0.0/requirements/
+-rw-rw-r--   0 sao       (1000) sao       (1000)       85 2024-04-18 19:02:48.000000 djangorestframework-jsonapi-7.0.0/requirements/requirements-codestyle.txt
+-rw-rw-r--   0 sao       (1000) sao       (1000)       58 2023-12-22 11:26:43.000000 djangorestframework-jsonapi-7.0.0/requirements/requirements-documentation.txt
+-rw-rw-r--   0 sao       (1000) sao       (1000)      320 2024-04-18 19:02:48.000000 djangorestframework-jsonapi-7.0.0/requirements/requirements-optionals.txt
+-rw-rw-r--   0 sao       (1000) sao       (1000)       13 2024-03-18 17:34:31.000000 djangorestframework-jsonapi-7.0.0/requirements/requirements-packaging.txt
+-rw-rw-r--   0 sao       (1000) sao       (1000)      125 2024-04-18 19:02:48.000000 djangorestframework-jsonapi-7.0.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 sao       (1000) sao       (1000)      614 2021-09-23 17:13:33.000000 djangorestframework-jsonapi-7.0.0/requirements.txt
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.229449 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/
+-rw-rw-r--   0 sao       (1000) sao       (1000)      160 2024-05-02 19:40:15.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/__init__.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)        0 2024-03-20 16:52:18.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/compat.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.229449 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/django_filters/
+-rw-r--r--   0 sao       (1000) sao       (1000)       56 2018-12-31 08:26:06.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/django_filters/__init__.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     5966 2023-09-19 05:52:13.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/django_filters/backends.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1747 2024-04-18 19:32:05.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/exceptions.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     4589 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/filters.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     5967 2024-03-20 16:52:18.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/metadata.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     3218 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/pagination.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     6646 2024-03-18 17:34:31.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/parsers.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    14836 2024-04-30 18:29:15.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/relations.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    26907 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/renderers.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.229449 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/schemas/
+-rw-rw-r--   0 sao       (1000) sao       (1000)        0 2020-10-30 18:13:47.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/schemas/__init__.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    36280 2024-03-20 16:52:18.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/schemas/openapi.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    17506 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/serializers.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1600 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/settings.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.213448 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/templates/
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.233449 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/templates/rest_framework_json_api/
+-rw-rw-r--   0 sao       (1000) sao       (1000)      550 2020-11-09 20:27:29.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/templates/rest_framework_json_api/api.html
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1503 2020-11-09 20:27:29.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/templates/rest_framework_json_api/includes.html
+-rw-rw-r--   0 sao       (1000) sao       (1000)    17474 2024-04-19 18:05:34.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/utils.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    16313 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/rest_framework_json_api/views.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      963 2024-05-02 19:40:57.233449 djangorestframework-jsonapi-7.0.0/setup.cfg
+-rwxrwxr-x   0 sao       (1000) sao       (1000)     3857 2024-04-18 19:02:48.000000 djangorestframework-jsonapi-7.0.0/setup.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.233449 djangorestframework-jsonapi-7.0.0/tests/
+-rw-rw-r--   0 sao       (1000) sao       (1000)        0 2020-11-09 20:15:41.000000 djangorestframework-jsonapi-7.0.0/tests/__init__.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     2391 2024-04-18 19:40:01.000000 djangorestframework-jsonapi-7.0.0/tests/conftest.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1359 2024-04-18 19:02:48.000000 djangorestframework-jsonapi-7.0.0/tests/models.py
+drwxrwxr-x   0 sao       (1000) sao       (1000)        0 2024-05-02 19:40:57.233449 djangorestframework-jsonapi-7.0.0/tests/schemas/
+-rw-rw-r--   0 sao       (1000) sao       (1000)      409 2023-08-23 12:27:19.000000 djangorestframework-jsonapi-7.0.0/tests/schemas/test_openapi.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1871 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/tests/serializers.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1421 2023-04-25 16:40:02.000000 djangorestframework-jsonapi-7.0.0/tests/test_pagination.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     4172 2022-01-03 16:22:32.000000 djangorestframework-jsonapi-7.0.0/tests/test_parsers.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    10601 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/tests/test_relations.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     2842 2023-10-19 11:02:58.000000 djangorestframework-jsonapi-7.0.0/tests/test_serializers.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      437 2023-02-21 08:29:06.000000 djangorestframework-jsonapi-7.0.0/tests/test_settings.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    13026 2024-04-18 19:02:48.000000 djangorestframework-jsonapi-7.0.0/tests/test_utils.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)    15864 2024-05-02 18:52:42.000000 djangorestframework-jsonapi-7.0.0/tests/test_views.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)      985 2024-04-19 19:44:00.000000 djangorestframework-jsonapi-7.0.0/tests/views.py
+-rw-rw-r--   0 sao       (1000) sao       (1000)     1379 2024-04-18 19:02:48.000000 djangorestframework-jsonapi-7.0.0/tox.ini
```

### Comparing `djangorestframework-jsonapi-6.1.0/.github/workflows/codeql-analysis.yml` & `djangorestframework-jsonapi-7.0.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/.github/workflows/tests.yml` & `djangorestframework-jsonapi-7.0.0/.github/workflows/tests.yml`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 jobs:
   test:
     name: Run test
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     env:
       PYTHON: ${{ matrix.python-version }}
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
@@ -26,30 +26,31 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - name: Run tox targets for ${{ matrix.python-version }}
         run: tox run -f py$(echo ${{ matrix.python-version }} | tr -d .)
       - name: Upload coverage report
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v4
         with:
+          token: ${{ secrets.CODECOV_TOKEN }}
           env_vars: PYTHON
   check:
     name: Run check
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         tox-env: ["black", "lint", "docs"]
     steps:
       - uses: actions/checkout@v2
-      - name: Set up Python 3.8
+      - name: Set up Python 3.9
         uses: actions/setup-python@v2
         with:
-          python-version: 3.8
+          python-version: 3.9
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - name: Run lint
         run: tox
         env:
```

### Comparing `djangorestframework-jsonapi-6.1.0/.gitignore` & `djangorestframework-jsonapi-7.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/AUTHORS` & `djangorestframework-jsonapi-7.0.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Adam Wróbel <https://adamwrobel.com>
 Adam Ziolkowski <adam@adsized.com>
 Alan Crosswell <alan@columbia.edu>
 Alex Seidmann <alex@leanpnt.de>
+Antoine Auger <https://antoineauger.fr/en>
 Anton Shutik <shutikanton@gmail.com>
 Arttu Perälä <arttu@perala.me>
 Ashley Loewen <github@ashleycodes.tech>
 Asif Saif Uddin <auvipy@gmail.com>
 Beni Keller <beni@matraxi.ch>
 Boris Pleshakov <koordinator.kun@gmail.com>
 Charlie Allatson <charles.allatson@gmail.com>
```

### Comparing `djangorestframework-jsonapi-6.1.0/CHANGELOG.md` & `djangorestframework-jsonapi-7.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,45 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Note that in line with [Django REST framework policy](https://www.django-rest-framework.org/topics/release-notes/),
 any parts of the framework not mentioned in the documentation should generally be considered private API, and may be subject to change.
 
+## [7.0.0] - 2024-05-02
+
+### Added
+
+* Added support for Python 3.12
+* Added support for Django 5.0
+* Added support for Django REST framework 3.15
+
+### Fixed
+
+* Fixed OpenAPI schema generation for `Serializer` when used inside another `Serializer` or as a child of `ListField`.
+* `ModelSerializer` fields are now returned in the same order than DRF
+* Avoided that an empty attributes dict is rendered in case serializer does not
+  provide any attribute fields.
+* Avoided shadowing of exception when rendering errors (regression since 4.3.0).
+* Ensured that sparse fields only applies when rendering, not when parsing.
+* Adjusted that sparse fields properly removes meta fields when not defined.
+
+### Removed
+
+* Removed support for Python 3.7.
+* Removed support for Django 3.2.
+* Removed support for Django 4.0.
+* Removed support for Django 4.1.
+* Removed support for Django REST framework 3.13.
+* Removed obsolete compat `NullBooleanField` and `get_reference` definitions.
+
 ## [6.1.0] - 2023-08-25
 
+This is the last release supporting Python 3.7, Django 3.2, Django 4.0, Django 4.1 and Django REST framework 3.13.
+
 ### Added
 
 * Added support for Python 3.11.
 * Added support for Django 4.2.
 * Added `400 Bad Request` as a possible error response in the OpenAPI schema.
 
 ### Changed
```

### Comparing `djangorestframework-jsonapi-6.1.0/LICENSE` & `djangorestframework-jsonapi-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/PKG-INFO` & `djangorestframework-jsonapi-7.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: djangorestframework-jsonapi
-Version: 6.1.0
+Version: 7.0.0
 Summary: A Django REST framework API adapter for the JSON:API spec.
 Home-page: https://github.com/django-json-api/django-rest-framework-json-api
 Author: Jerel Unruh
 Author-email: 
 License: BSD
+Project-URL: Documentation, https://django-rest-framework-json-api.readthedocs.org/
+Project-URL: Changelog, https://github.com/django-json-api/django-rest-framework-json-api/blob/main/CHANGELOG.md
+Project-URL: Source, https://github.com/django-json-api/django-rest-framework-json-api
+Project-URL: Tracker, https://github.com/django-json-api/django-rest-framework-json-api/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: django-filter
 Provides-Extra: django-polymorphic
 Provides-Extra: openapi
 License-File: LICENSE
 License-File: AUTHORS
 
 ==================================
@@ -120,17 +124,17 @@
 .. _JSON:API: https://jsonapi.org
 .. _Django REST framework: https://www.django-rest-framework.org/
 
 ------------
 Requirements
 ------------
 
-1. Python (3.7, 3.8, 3.9, 3.10, 3.11)
-2. Django (3.2, 4.0, 4.1, 4.2)
-3. Django REST framework (3.13, 3.14)
+1. Python (3.8, 3.9, 3.10, 3.11, 3.12)
+2. Django (4.2, 5.0)
+3. Django REST framework (3.14, 3.15)
 
 We **highly** recommend and only officially support the latest patch release of each Python, Django and REST framework series.
 
 Generally Python and Django series are supported till the official end of life. For Django REST framework the last two series are supported.
 
 For optional dependencies such as Django Filter only the latest release is officially supported even though lower versions should work as well.
```

### Comparing `djangorestframework-jsonapi-6.1.0/README.rst` & `djangorestframework-jsonapi-7.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,17 @@
 .. _JSON:API: https://jsonapi.org
 .. _Django REST framework: https://www.django-rest-framework.org/
 
 ------------
 Requirements
 ------------
 
-1. Python (3.7, 3.8, 3.9, 3.10, 3.11)
-2. Django (3.2, 4.0, 4.1, 4.2)
-3. Django REST framework (3.13, 3.14)
+1. Python (3.8, 3.9, 3.10, 3.11, 3.12)
+2. Django (4.2, 5.0)
+3. Django REST framework (3.14, 3.15)
 
 We **highly** recommend and only officially support the latest patch release of each Python, Django and REST framework series.
 
 Generally Python and Django series are supported till the official end of life. For Django REST framework the last two series are supported.
 
 For optional dependencies such as Django Filter only the latest release is officially supported even though lower versions should work as well.
```

### Comparing `djangorestframework-jsonapi-6.1.0/djangorestframework_jsonapi.egg-info/PKG-INFO` & `djangorestframework-jsonapi-7.0.0/djangorestframework_jsonapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: djangorestframework-jsonapi
-Version: 6.1.0
+Version: 7.0.0
 Summary: A Django REST framework API adapter for the JSON:API spec.
 Home-page: https://github.com/django-json-api/django-rest-framework-json-api
 Author: Jerel Unruh
 Author-email: 
 License: BSD
+Project-URL: Documentation, https://django-rest-framework-json-api.readthedocs.org/
+Project-URL: Changelog, https://github.com/django-json-api/django-rest-framework-json-api/blob/main/CHANGELOG.md
+Project-URL: Source, https://github.com/django-json-api/django-rest-framework-json-api
+Project-URL: Tracker, https://github.com/django-json-api/django-rest-framework-json-api/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: django-filter
 Provides-Extra: django-polymorphic
 Provides-Extra: openapi
 License-File: LICENSE
 License-File: AUTHORS
 
 ==================================
@@ -120,17 +124,17 @@
 .. _JSON:API: https://jsonapi.org
 .. _Django REST framework: https://www.django-rest-framework.org/
 
 ------------
 Requirements
 ------------
 
-1. Python (3.7, 3.8, 3.9, 3.10, 3.11)
-2. Django (3.2, 4.0, 4.1, 4.2)
-3. Django REST framework (3.13, 3.14)
+1. Python (3.8, 3.9, 3.10, 3.11, 3.12)
+2. Django (4.2, 5.0)
+3. Django REST framework (3.14, 3.15)
 
 We **highly** recommend and only officially support the latest patch release of each Python, Django and REST framework series.
 
 Generally Python and Django series are supported till the official end of life. For Django REST framework the last two series are supported.
 
 For optional dependencies such as Django Filter only the latest release is officially supported even though lower versions should work as well.
```

### Comparing `djangorestframework-jsonapi-6.1.0/djangorestframework_jsonapi.egg-info/SOURCES.txt` & `djangorestframework-jsonapi-7.0.0/djangorestframework_jsonapi.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 example/migrations/0006_auto_20181228_0752.py
 example/migrations/0007_artproject_description.py
 example/migrations/0008_labresults.py
 example/migrations/0009_labresults_author.py
 example/migrations/0010_auto_20210714_0809.py
 example/migrations/0011_rename_type_author_author_type_and_more.py
 example/migrations/0012_author_full_name.py
+example/migrations/0013_questionnaire.py
+example/migrations/0014_questionnaire_metadata.py
 example/migrations/__init__.py
 example/settings/__init__.py
 example/settings/dev.py
 example/settings/test.py
 example/templates/swagger-ui.html
 example/tests/__init__.py
 example/tests/conftest.py
```

### Comparing `djangorestframework-jsonapi-6.1.0/docs/CONTRIBUTING.md` & `djangorestframework-jsonapi-7.0.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/docs/Makefile` & `djangorestframework-jsonapi-7.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/docs/conf.py` & `djangorestframework-jsonapi-7.0.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ["sphinx.ext.autodoc", "recommonmark"]
+extensions = ["sphinx.ext.autodoc", "recommonmark", "sphinx_rtd_theme"]
 autodoc_member_order = "bysource"
 autodoc_inherit_docstrings = False
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
@@ -118,23 +118,15 @@
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "default"
-
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
-
-if not on_rtd:  # only import and set the theme if we're building docs locally
-    import sphinx_rtd_theme
-
-    html_theme = "sphinx_rtd_theme"
-    html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 # html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
```

### Comparing `djangorestframework-jsonapi-6.1.0/docs/getting-started.md` & `djangorestframework-jsonapi-7.0.0/docs/getting-started.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,17 @@
     }
 }
 ```
 
 
 ## Requirements
 
-1. Python (3.7, 3.8, 3.9, 3.10, 3.11)
-2. Django (3.2, 4.0, 4.1, 4.2)
-3. Django REST framework (3.13, 3.14)
+1. Python (3.8, 3.9, 3.10, 3.11, 3.12)
+2. Django (4.2, 5.0)
+3. Django REST framework (3.14, 3.15)
 
 We **highly** recommend and only officially support the latest patch release of each Python, Django and REST framework series.
 
 Generally Python and Django series are supported till the official end of life. For Django REST framework the last two series are supported.
 
 For optional dependencies such as Django Filter only the latest release is officially supported even though lower versions should work as well.
```

### Comparing `djangorestframework-jsonapi-6.1.0/docs/make.bat` & `djangorestframework-jsonapi-7.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/docs/usage.md` & `djangorestframework-jsonapi-7.0.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/api/resources/identity.py` & `djangorestframework-jsonapi-7.0.0/example/api/resources/identity.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/api/serializers/identity.py` & `djangorestframework-jsonapi-7.0.0/example/api/serializers/identity.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/factories.py` & `djangorestframework-jsonapi-7.0.0/example/factories.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     AuthorBioMetadata,
     AuthorType,
     Blog,
     Comment,
     Company,
     Entry,
     ProjectType,
+    Questionnaire,
     ResearchProject,
     TaggedItem,
 )
 
 faker = FakerFactory.create()
 faker.seed(983843)
 
@@ -32,26 +33,28 @@
         model = AuthorType
 
     name = factory.LazyAttribute(lambda x: faker.name())
 
 
 class AuthorFactory(factory.django.DjangoModelFactory):
     class Meta:
+        skip_postgeneration_save = True
         model = Author
 
     name = factory.LazyAttribute(lambda x: faker.name())
     email = factory.LazyAttribute(lambda x: faker.email())
 
     bio = factory.RelatedFactory("example.factories.AuthorBioFactory", "author")
     author_type = factory.SubFactory(AuthorTypeFactory)
 
 
 class AuthorBioFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = AuthorBio
+        skip_postgeneration_save = True
 
     author = factory.SubFactory(AuthorFactory)
     body = factory.LazyAttribute(lambda x: faker.text())
 
     metadata = factory.RelatedFactory(
         "example.factories.AuthorBioMetadataFactory", "bio"
     )
@@ -64,14 +67,15 @@
     bio = factory.SubFactory(AuthorBioFactory)
     body = factory.LazyAttribute(lambda x: faker.text())
 
 
 class EntryFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = Entry
+        skip_postgeneration_save = True
 
     headline = factory.LazyAttribute(lambda x: faker.sentence(nb_words=4))
     body_text = factory.LazyAttribute(lambda x: faker.text())
 
     blog = factory.SubFactory(BlogFactory)
 
     @factory.post_generation
@@ -125,18 +129,40 @@
     supervisor = factory.LazyAttribute(lambda x: faker.name())
     project_type = factory.SubFactory(ProjectTypeFactory)
 
 
 class CompanyFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = Company
+        skip_postgeneration_save = True
 
     name = factory.LazyAttribute(lambda x: faker.company())
     current_project = factory.SubFactory(ArtProjectFactory)
 
     @factory.post_generation
     def future_projects(self, create, extracted, **kwargs):
         if not create:  # pragma: no cover
             return
         if extracted:
             for project in extracted:
                 self.future_projects.add(project)
+
+
+class QuestionnaireFactory(factory.django.DjangoModelFactory):
+    class Meta:
+        model = Questionnaire
+
+    name = factory.LazyAttribute(lambda x: faker.text())
+    questions = [
+        {
+            "text": "What is your name?",
+            "required": True,
+        },
+        {
+            "text": "What is your quest?",
+            "required": False,
+        },
+        {
+            "text": "What is the air-speed velocity of an unladen swallow?",
+        },
+    ]
+    metadata = {"author": "Bridgekeeper"}
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/fixtures/blogentry.json` & `djangorestframework-jsonapi-7.0.0/example/fixtures/blogentry.json`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/fixtures/drf_example.json` & `djangorestframework-jsonapi-7.0.0/example/fixtures/drf_example.json`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/migrations/0001_initial.py` & `djangorestframework-jsonapi-7.0.0/example/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/migrations/0002_taggeditem.py` & `djangorestframework-jsonapi-7.0.0/example/migrations/0002_taggeditem.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/migrations/0003_polymorphics.py` & `djangorestframework-jsonapi-7.0.0/example/migrations/0003_polymorphics.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/migrations/0004_auto_20171011_0631.py` & `djangorestframework-jsonapi-7.0.0/example/migrations/0004_auto_20171011_0631.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/migrations/0005_auto_20180922_1508.py` & `djangorestframework-jsonapi-7.0.0/example/migrations/0005_auto_20180922_1508.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/migrations/0006_auto_20181228_0752.py` & `djangorestframework-jsonapi-7.0.0/example/migrations/0006_auto_20181228_0752.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/migrations/0008_labresults.py` & `djangorestframework-jsonapi-7.0.0/example/migrations/0008_labresults.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/migrations/0009_labresults_author.py` & `djangorestframework-jsonapi-7.0.0/example/migrations/0009_labresults_author.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/migrations/0011_rename_type_author_author_type_and_more.py` & `djangorestframework-jsonapi-7.0.0/example/migrations/0011_rename_type_author_author_type_and_more.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/models.py` & `djangorestframework-jsonapi-7.0.0/example/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,7 +176,13 @@
     current_project = models.ForeignKey(
         Project, related_name="companies", on_delete=models.CASCADE
     )
     future_projects = models.ManyToManyField(Project)
 
     def __str__(self):
         return self.name
+
+
+class Questionnaire(models.Model):
+    name = models.CharField(max_length=100)
+    questions = models.JSONField()
+    metadata = models.JSONField()
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/serializers.py` & `djangorestframework-jsonapi-7.0.0/example/serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Blog,
     Comment,
     Company,
     Entry,
     LabResults,
     Project,
     ProjectType,
+    Questionnaire,
     ResearchProject,
     TaggedItem,
 )
 
 
 class TaggedItemSerializer(serializers.ModelSerializer):
     class Meta:
@@ -417,7 +418,26 @@
         "current_art_project": ProjectSerializer,
         "current_research_project": ProjectSerializer,
     }
 
     class Meta:
         model = Company
         fields = "__all__"
+
+
+class QuestionSerializer(serializers.Serializer):
+    text = serializers.CharField()
+    required = serializers.BooleanField(default=False)
+
+
+class QuestionnaireMetadataSerializer(serializers.Serializer):
+    author = serializers.CharField()
+    producer = serializers.CharField(default=None)
+
+
+class QuestionnaireSerializer(serializers.ModelSerializer):
+    questions = serializers.ListField(child=QuestionSerializer())
+    metadata = QuestionnaireMetadataSerializer()
+
+    class Meta:
+        model = Questionnaire
+        fields = ("name", "questions", "metadata")
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/settings/dev.py` & `djangorestframework-jsonapi-7.0.0/example/settings/dev.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/templates/swagger-ui.html` & `djangorestframework-jsonapi-7.0.0/example/templates/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/__init__.py` & `djangorestframework-jsonapi-7.0.0/example/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/__snapshots__/test_errors.ambr` & `djangorestframework-jsonapi-7.0.0/example/tests/__snapshots__/test_errors.ambr`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# serializer version: 1
 # name: test_first_level_attribute_error
   dict({
     'errors': list([
       dict({
         'code': 'required',
         'detail': 'This field is required.',
         'source': dict({
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/__snapshots__/test_openapi.ambr` & `djangorestframework-jsonapi-7.0.0/example/tests/__snapshots__/test_openapi.ambr`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# serializer version: 1
 # name: test_delete_request
   '''
   {
     "description": "",
     "operationId": "destroy/authors/{id}",
     "parameters": [
       {
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/conftest.py` & `djangorestframework-jsonapi-7.0.0/example/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     AuthorBioMetadataFactory,
     AuthorFactory,
     AuthorTypeFactory,
     BlogFactory,
     CommentFactory,
     CompanyFactory,
     EntryFactory,
+    QuestionnaireFactory,
     ResearchProjectFactory,
     TaggedItemFactory,
 )
 
 register(BlogFactory)
 register(AuthorFactory)
 register(AuthorBioFactory)
@@ -23,14 +24,15 @@
 register(AuthorTypeFactory)
 register(EntryFactory)
 register(CommentFactory)
 register(TaggedItemFactory)
 register(ArtProjectFactory)
 register(ResearchProjectFactory)
 register(CompanyFactory)
+register(QuestionnaireFactory)
 
 
 @pytest.fixture
 def single_entry(blog, author, entry_factory, comment_factory, tagged_item_factory):
     entry = entry_factory(blog=blog, authors=(author,))
     comment_factory(entry=entry)
     tagged_item_factory(content_object=entry)
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/integration/test_browsable_api.py` & `djangorestframework-jsonapi-7.0.0/example/tests/integration/test_browsable_api.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/integration/test_includes.py` & `djangorestframework-jsonapi-7.0.0/example/tests/integration/test_includes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,13 @@
 import pytest
 from django.urls import reverse
 
 pytestmark = pytest.mark.django_db
 
 
-def test_included_data_on_list(multiple_entries, client):
-    response = client.get(
-        reverse("entry-list"), data={"include": "comments", "page[size]": 5}
-    )
-    included = response.json().get("included")
-
-    assert len(response.json()["data"]) == len(
-        multiple_entries
-    ), "Incorrect entry count"
-    assert [x.get("type") for x in included] == [
-        "comments",
-        "comments",
-    ], "List included types are incorrect"
-
-    comment_count = len(
-        [resource for resource in included if resource["type"] == "comments"]
-    )
-    expected_comment_count = sum(entry.comments.count() for entry in multiple_entries)
-    assert comment_count == expected_comment_count, "List comment count is incorrect"
-
-
-def test_included_data_on_list_with_one_to_one_relations(multiple_entries, client):
-    response = client.get(
-        reverse("entry-list"), data={"include": "authors.bio.metadata", "page[size]": 5}
-    )
-    included = response.json().get("included")
-
-    assert len(response.json()["data"]) == len(
-        multiple_entries
-    ), "Incorrect entry count"
-    expected_include_types = [
-        "authorBioMetadata",
-        "authorBioMetadata",
-        "authorBios",
-        "authorBios",
-        "authors",
-        "authors",
-    ]
-    include_types = [x.get("type") for x in included]
-    assert include_types == expected_include_types, "List included types are incorrect"
-
-
-def test_default_included_data_on_detail(single_entry, client):
-    return test_included_data_on_detail(
-        single_entry=single_entry, client=client, query=""
-    )
-
-
-def test_included_data_on_detail(single_entry, client, query="?include=comments"):
-    response = client.get(
-        reverse("entry-detail", kwargs={"pk": single_entry.pk}) + query
-    )
-    included = response.json().get("included")
-
-    assert [x.get("type") for x in included] == [
-        "comments"
-    ], "Detail included types are incorrect"
-
-    comment_count = len(
-        [resource for resource in included if resource["type"] == "comments"]
-    )
-    expected_comment_count = single_entry.comments.count()
-    assert comment_count == expected_comment_count, "Detail comment count is incorrect"
-
-
 def test_dynamic_related_data_is_included(single_entry, entry_factory, client):
     entry_factory()
     response = client.get(
         reverse("entry-detail", kwargs={"pk": single_entry.pk}) + "?include=featured"
     )
     included = response.json().get("included")
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/integration/test_meta.py` & `djangorestframework-jsonapi-7.0.0/example/tests/integration/test_meta.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/integration/test_model_resource_name.py` & `djangorestframework-jsonapi-7.0.0/example/tests/integration/test_model_resource_name.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/integration/test_non_paginated_responses.py` & `djangorestframework-jsonapi-7.0.0/example/tests/integration/test_non_paginated_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "rest_framework_json_api.utils" ".get_default_included_resources_from_serializer",
     new=lambda s: [],
 )
 def test_multiple_entries_no_pagination(multiple_entries, client):
     expected = {
         "data": [
             {
-                "type": "posts",
+                "type": "entries",
                 "id": "1",
                 "attributes": {
                     "headline": multiple_entries[0].headline,
                     "bodyText": multiple_entries[0].body_text,
                     "pubDate": None,
                     "modDate": None,
                 },
@@ -66,15 +66,15 @@
                             "self": "http://testserver/entries/1/relationships/featured_hyperlinked",  # noqa: B950
                         }
                     },
                     "tags": {"data": [], "meta": {"count": 0}},
                 },
             },
             {
-                "type": "posts",
+                "type": "entries",
                 "id": "2",
                 "attributes": {
                     "headline": multiple_entries[1].headline,
                     "bodyText": multiple_entries[1].body_text,
                     "pubDate": None,
                     "modDate": None,
                 },
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/integration/test_pagination.py` & `djangorestframework-jsonapi-7.0.0/example/tests/integration/test_pagination.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "rest_framework_json_api.utils" ".get_default_included_resources_from_serializer",
     new=lambda s: [],
 )
 def test_pagination_with_single_entry(single_entry, client):
     expected = {
         "data": [
             {
-                "type": "posts",
+                "type": "entries",
                 "id": "1",
                 "attributes": {
                     "headline": single_entry.headline,
                     "bodyText": single_entry.body_text,
                     "pubDate": None,
                     "modDate": None,
                 },
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/integration/test_polymorphism.py` & `djangorestframework-jsonapi-7.0.0/example/tests/integration/test_polymorphism.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     assert content["data"]["relationships"]["currentResearchProject"]["data"] is None
     assert {
         rel["type"]
         for rel in content["data"]["relationships"]["futureProjects"]["data"]
     } == {"researchProjects", "artProjects"}
     assert {x.get("type") for x in content.get("included")} == {
         "artProjects",
-        "artProjects",
         "researchProjects",
     }, "Detail included types are incorrect"
     # Ensure that the child fields are present.
     assert content.get("included")[0].get("attributes").get("artist") is not None
     assert content.get("included")[1].get("attributes").get("artist") is not None
     assert content.get("included")[2].get("attributes").get("supervisor") is not None
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/integration/test_sparse_fieldsets.py` & `djangorestframework-jsonapi-7.0.0/example/tests/integration/test_sparse_fieldsets.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     assert response.status_code == status.HTTP_200_OK
     data = response.json()["data"]
 
     assert len(data) == 1
     entry = data[0]
     assert entry["attributes"].keys() == {"headline"}
     assert entry["relationships"].keys() == {"blog"}
+    assert "meta" not in entry
 
 
 @pytest.mark.parametrize(
     "fields_param", ["invalidfields[entries]", "fieldsinvalid[entries"]
 )
 def test_sparse_fieldset_invalid_fields_parameter(client, entry, fields_param):
     """
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/test_errors.py` & `djangorestframework-jsonapi-7.0.0/example/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/test_filters.py` & `djangorestframework-jsonapi-7.0.0/example/tests/test_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -466,15 +466,15 @@
         """
         response = self.client.get(
             self.url, data={"filter[search]": "barnard field research"}
         )
         expected_result = {
             "data": [
                 {
-                    "type": "posts",
+                    "type": "entries",
                     "id": "7",
                     "attributes": {
                         "headline": "ANTH3868X",
                         "bodyText": "ETHNOGRAPHIC FIELD RESEARCH IN NYC",
                         "pubDate": None,
                         "modDate": None,
                     },
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/test_generic_validation.py` & `djangorestframework-jsonapi-7.0.0/example/tests/test_generic_validation.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/test_generic_viewset.py` & `djangorestframework-jsonapi-7.0.0/example/tests/test_generic_viewset.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/test_model_viewsets.py` & `djangorestframework-jsonapi-7.0.0/example/tests/test_model_viewsets.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/test_openapi.py` & `djangorestframework-jsonapi-7.0.0/example/tests/test_openapi.py`

 * *Files 11% similar despite different names*

```diff
@@ -121,14 +121,54 @@
     schema = generator.get_schema(request=request)
 
     company_properties = schema["components"]["schemas"]["Company"]["properties"]
     assert company_properties["id"] == {"$ref": "#/components/schemas/id"}
     assert "id" not in company_properties["attributes"]["properties"]
 
 
+def test_schema_subserializers():
+    """Schema for child Serializers reflects the actual response structure."""
+    patterns = [
+        re_path(
+            "^questionnaires/?$", views.QuestionnaireViewset.as_view({"get": "list"})
+        ),
+    ]
+    generator = SchemaGenerator(patterns=patterns)
+
+    request = create_request("/")
+    schema = generator.get_schema(request=request)
+
+    assert {
+        "type": "object",
+        "properties": {
+            "metadata": {
+                "type": "object",
+                "properties": {
+                    "author": {"type": "string"},
+                    "producer": {"type": "string"},
+                },
+                "required": ["author"],
+            },
+            "questions": {
+                "type": "array",
+                "items": {
+                    "type": "object",
+                    "properties": {
+                        "text": {"type": "string"},
+                        "required": {"type": "boolean", "default": False},
+                    },
+                    "required": ["text"],
+                },
+            },
+            "name": {"type": "string", "maxLength": 100},
+        },
+        "required": ["name", "questions", "metadata"],
+    } == schema["components"]["schemas"]["Questionnaire"]["properties"]["attributes"]
+
+
 def test_schema_parameters_include():
     """Include paramater is only used when serializer defines included_serializers."""
     patterns = [
         re_path("^authors/?$", views.AuthorViewSet.as_view({"get": "list"})),
         re_path("^project-types/?$", views.ProjectTypeViewset.as_view({"get": "list"})),
     ]
     generator = SchemaGenerator(patterns=patterns)
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/test_performance.py` & `djangorestframework-jsonapi-7.0.0/example/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/test_serializers.py` & `djangorestframework-jsonapi-7.0.0/example/tests/test_serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,14 +220,47 @@
         }
 
         response = client.get(reverse("comment-detail", kwargs={"pk": comment.pk}))
 
         assert response.status_code == 200
         assert expected == response.json()
 
+    def test_model_serializer_with_subserializers(self, questionnaire, client):
+        expected = {
+            "data": {
+                "type": "questionnaires",
+                "id": str(questionnaire.pk),
+                "attributes": {
+                    "name": questionnaire.name,
+                    "questions": [
+                        {
+                            "text": "What is your name?",
+                            "required": True,
+                        },
+                        {
+                            "text": "What is your quest?",
+                            "required": False,
+                        },
+                        {
+                            "text": "What is the air-speed velocity of an unladen swallow?",
+                            "required": False,
+                        },
+                    ],
+                    "metadata": {"author": "Bridgekeeper", "producer": None},
+                },
+            },
+        }
+
+        response = client.get(
+            reverse("questionnaire-detail", kwargs={"pk": questionnaire.pk})
+        )
+
+        assert response.status_code == 200
+        assert expected == response.json()
+
 
 class TestPolymorphicModelSerializer(TestCase):
     def setUp(self):
         self.project = ArtProjectFactory.create()
         self.child_init_args = {}
 
         # Override `__init__` with our own method
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/test_sideload_resources.py` & `djangorestframework-jsonapi-7.0.0/example/tests/test_sideload_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test sideloading resources
 """
+
 import json
 
 from django.urls import reverse
 from django.utils import encoding
 
 from example.tests import TestBase
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/test_views.py` & `djangorestframework-jsonapi-7.0.0/example/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/unit/test_default_drf_serializers.py` & `djangorestframework-jsonapi-7.0.0/example/tests/unit/test_default_drf_serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/unit/test_filter_schema_params.py` & `djangorestframework-jsonapi-7.0.0/example/tests/unit/test_filter_schema_params.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/unit/test_renderer_class_methods.py` & `djangorestframework-jsonapi-7.0.0/example/tests/unit/test_renderer_class_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,16 +98,16 @@
         "deleted": serializers.ReadOnlyField(),
     }
     resource = {"id": 1, "deleted": None, "username": "jerel"}
     expected = {"username": "jerel", "deleted": None}
     assert sorted(JSONRenderer.extract_attributes(fields, resource)) == sorted(
         expected
     ), "Regular fields should be extracted"
-    assert sorted(JSONRenderer.extract_attributes(fields, {})) == sorted(
-        {"username": ""}
+    assert (
+        JSONRenderer.extract_attributes(fields, {}) == {}
     ), "Should not extract read_only fields on empty serializer"
 
 
 def test_extract_meta():
     serializer = ResourceSerializer(data={"username": "jerel", "version": "1.0.0"})
     serializer.is_valid()
     expected = {
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/unit/test_renderers.py` & `djangorestframework-jsonapi-7.0.0/example/tests/unit/test_renderers.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,24 +122,25 @@
             many=True, write_only=True, queryset=Comment.objects.all()
         )
 
         rating = serializers.IntegerField(write_only=True)
 
         class Meta:
             model = Entry
-            fields = ("comments", "rating")
+            fields = ("headline", "comments", "rating")
 
     class WriteOnlyDummyTestViewSet(views.ReadOnlyModelViewSet):
         queryset = Entry.objects.all()
         serializer_class = WriteonlyTestSerializer
 
     rendered = render_dummy_test_serialized_view(WriteOnlyDummyTestViewSet, Entry())
     result = json.loads(rendered.decode())
 
     assert "rating" not in result["data"]["attributes"]
+    assert "headline" in result["data"]["attributes"]
     assert "relationships" not in result["data"]
 
 
 def test_render_empty_relationship_reverse_lookup():
     """Test that empty relationships are rendered as None."""
 
     class EmptyRelationshipSerializer(serializers.ModelSerializer):
@@ -149,14 +150,15 @@
 
     class EmptyRelationshipViewSet(views.ReadOnlyModelViewSet):
         queryset = Author.objects.all()
         serializer_class = EmptyRelationshipSerializer
 
     rendered = render_dummy_test_serialized_view(EmptyRelationshipViewSet, Author())
     result = json.loads(rendered.decode())
+    assert "attributes" not in result["data"]
     assert "relationships" in result["data"]
     assert "bio" in result["data"]["relationships"]
     assert result["data"]["relationships"]["bio"] == {"data": None}
 
 
 @pytest.mark.django_db
 def test_extract_relation_instance(comment):
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/tests/unit/test_serializer_method_field.py` & `djangorestframework-jsonapi-7.0.0/example/tests/unit/test_serializer_method_field.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/urls.py` & `djangorestframework-jsonapi-7.0.0/example/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,27 +15,29 @@
     CompanyViewset,
     EntryRelationshipView,
     EntryViewSet,
     LabResultViewSet,
     NonPaginatedEntryViewSet,
     ProjectTypeViewset,
     ProjectViewset,
+    QuestionnaireViewset,
 )
 
 router = routers.DefaultRouter(trailing_slash=False)
 
 router.register(r"blogs", BlogViewSet)
 router.register(r"entries", EntryViewSet)
 router.register(r"nopage-entries", NonPaginatedEntryViewSet, "nopage-entry")
 router.register(r"authors", AuthorViewSet)
 router.register(r"comments", CommentViewSet)
 router.register(r"companies", CompanyViewset)
 router.register(r"projects", ProjectViewset)
 router.register(r"project-types", ProjectTypeViewset)
 router.register(r"lab-results", LabResultViewSet)
+router.register(r"questionnaires", QuestionnaireViewset)
 
 urlpatterns = [
     path("", include(router.urls)),
     re_path(
         r"^entries/(?P<entry_pk>[^/.]+)/suggested/$",
         EntryViewSet.as_view({"get": "list"}),
         name="entry-suggested",
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/urls_test.py` & `djangorestframework-jsonapi-7.0.0/example/urls_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.urls import re_path
+from django.urls import path, re_path
 from rest_framework import routers
 
 from .api.resources.identity import GenericIdentity, Identity
 from example.views import (
     AuthorRelationshipView,
     AuthorViewSet,
     BlogRelationshipView,
@@ -16,14 +16,15 @@
     EntryViewSet,
     FiltersetEntryViewSet,
     LabResultViewSet,
     NoFiltersetEntryViewSet,
     NonPaginatedEntryViewSet,
     ProjectTypeViewset,
     ProjectViewset,
+    QuestionnaireViewset,
 )
 
 router = routers.DefaultRouter(trailing_slash=False)
 
 router.register(r"blogs", BlogViewSet)
 # router to test default DRF blog functionalities
 router.register(r"drf-blogs", DRFBlogViewSet, "drf-entry-blog")
@@ -34,22 +35,23 @@
 router.register(r"nofilterset-entries", NoFiltersetEntryViewSet, "nofilterset-entry")
 router.register(r"authors", AuthorViewSet)
 router.register(r"comments", CommentViewSet)
 router.register(r"companies", CompanyViewset)
 router.register(r"projects", ProjectViewset)
 router.register(r"project-types", ProjectTypeViewset)
 router.register(r"lab-results", LabResultViewSet)
+router.register(r"questionnaires", QuestionnaireViewset)
 
 # for the old tests
 router.register(r"identities", Identity)
 
 urlpatterns = [
     # old tests
-    re_path(
-        r"identities/default/(?P<pk>\d+)$",
+    path(
+        "identities/default/<int:pk>",
         GenericIdentity.as_view(),
         name="user-default",
     ),
     re_path(
         r"^entries/(?P<entry_pk>[^/.]+)/blog$",
         BlogViewSet.as_view({"get": "retrieve"}),
         name="entry-blog",
```

### Comparing `djangorestframework-jsonapi-6.1.0/example/utils.py` & `djangorestframework-jsonapi-7.0.0/example/utils.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/example/views.py` & `djangorestframework-jsonapi-7.0.0/example/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,28 +25,30 @@
     Blog,
     Comment,
     Company,
     Entry,
     LabResults,
     Project,
     ProjectType,
+    Questionnaire,
 )
 from example.serializers import (
     AuthorDetailSerializer,
     AuthorListSerializer,
     AuthorSerializer,
     BlogDRFSerializer,
     BlogSerializer,
     CommentSerializer,
     CompanySerializer,
     EntryDRFSerializers,
     EntrySerializer,
     LabResultsSerializer,
     ProjectSerializer,
     ProjectTypeSerializer,
+    QuestionnaireSerializer,
 )
 
 HTTP_422_UNPROCESSABLE_ENTITY = 422
 
 
 class BlogViewSet(ModelViewSet):
     queryset = Blog.objects.all()
@@ -106,15 +108,18 @@
 class BlogCustomViewSet(JsonApiViewSet):
     queryset = Blog.objects.all()
     serializer_class = BlogSerializer
 
 
 class EntryViewSet(ModelViewSet):
     queryset = Entry.objects.all()
-    resource_name = "posts"
+    # TODO it should not be supported to overwrite resource name
+    # of endpoints with serializers as includes and sparse fields
+    # cannot be aware of it
+    # resource_name = "posts"
 
     def get_serializer_class(self):
         return EntrySerializer
 
     def get_object(self):
         # Handle featured
         entry_pk = self.kwargs.get("entry_pk", None)
@@ -288,7 +293,12 @@
 class LabResultViewSet(ReadOnlyModelViewSet):
     queryset = LabResults.objects.all()
     serializer_class = LabResultsSerializer
     prefetch_for_includes = {
         "__all__": [],
         "author": ["author__bio", "author__entries"],
     }
+
+
+class QuestionnaireViewset(ModelViewSet):
+    queryset = Questionnaire.objects.all()
+    serializer_class = QuestionnaireSerializer
```

### Comparing `djangorestframework-jsonapi-6.1.0/requirements.txt` & `djangorestframework-jsonapi-7.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/django_filters/backends.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/django_filters/backends.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/exceptions.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/filters.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/filters.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/metadata.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django.db.models.fields import related
 from django.utils.encoding import force_str
 from rest_framework import serializers
 from rest_framework.metadata import SimpleMetadata
 from rest_framework.settings import api_settings
 from rest_framework.utils.field_mapping import ClassLookupDict
 
-from rest_framework_json_api.compat import NullBooleanField
 from rest_framework_json_api.utils import format_field_name, get_related_resource_type
 
 
 class JSONAPIMetadata(SimpleMetadata):
     """
     This is the JSON:API metadata implementation.
     It returns an ad-hoc set of information about the view.
@@ -18,15 +17,14 @@
     """
 
     type_lookup = ClassLookupDict(
         {
             serializers.Field: "GenericField",
             serializers.RelatedField: "Relationship",
             serializers.BooleanField: "Boolean",
-            NullBooleanField: "Boolean",
             serializers.CharField: "String",
             serializers.URLField: "URL",
             serializers.EmailField: "Email",
             serializers.RegexField: "Regex",
             serializers.SlugField: "Slug",
             serializers.IntegerField: "Integer",
             serializers.FloatField: "Float",
```

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/pagination.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/pagination.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/parsers.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Parsers
 """
+
 from rest_framework import parsers
 from rest_framework.exceptions import ParseError
 
 from rest_framework_json_api import exceptions, renderers
 from rest_framework_json_api.utils import get_resource_name, undo_format_field_names
```

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/relations.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,17 +102,17 @@
 
     def get_links(self, obj=None, lookup_field="pk"):
         request = self.context.get("request", None)
         view = self.context.get("view", None)
         return_data = {}
 
         kwargs = {
-            lookup_field: getattr(obj, lookup_field)
-            if obj
-            else view.kwargs[lookup_field]
+            lookup_field: (
+                getattr(obj, lookup_field) if obj else view.kwargs[lookup_field]
+            )
         }
 
         field_name = self.field_name if self.field_name else self.parent.field_name
 
         self_kwargs = kwargs.copy()
         self_kwargs.update({"related_field": format_link_segment(field_name)})
         self_link = self.get_url("self", self.self_link_view_name, self_kwargs, request)
```

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/renderers.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/renderers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Renderers
 """
+
 import copy
 from collections import defaultdict
 from collections.abc import Iterable
 
 import inflection
 from django.db.models import Manager
 from django.template import loader
@@ -12,21 +13,34 @@
 from rest_framework import relations, renderers
 from rest_framework.fields import SkipField, get_attribute
 from rest_framework.relations import PKOnlyObject
 from rest_framework.serializers import ListSerializer, Serializer
 from rest_framework.settings import api_settings
 
 import rest_framework_json_api
-from rest_framework_json_api import utils
 from rest_framework_json_api.relations import (
     HyperlinkedMixin,
     ManySerializerMethodResourceRelatedField,
     ResourceRelatedField,
     SkipDataMixin,
 )
+from rest_framework_json_api.utils import (
+    format_errors,
+    format_field_name,
+    format_field_names,
+    get_included_resources,
+    get_related_resource_type,
+    get_relation_instance,
+    get_resource_id,
+    get_resource_name,
+    get_resource_type_from_instance,
+    get_resource_type_from_serializer,
+    get_serializer_fields,
+    is_relationship_field,
+)
 
 
 class JSONRenderer(renderers.JSONRenderer):
     """
     The `JSONRenderer` exposes a number of methods that you may override if you need highly
     custom rendering control.
 
@@ -52,39 +66,28 @@
     media_type = "application/vnd.api+json"
     format = "vnd.api+json"
 
     @classmethod
     def extract_attributes(cls, fields, resource):
         """
         Builds the `attributes` object of the JSON:API resource object.
-        """
-        data = {}
-        for field_name, field in iter(fields.items()):
-            # ID is always provided in the root of JSON:API so remove it from attributes
-            if field_name == "id":
-                continue
-            # don't output a key for write only fields
-            if fields[field_name].write_only:
-                continue
-            # Skip fields with relations
-            if utils.is_relationship_field(field):
-                continue
 
-            # Skip read_only attribute fields when `resource` is an empty
-            # serializer. Prevents the "Raw Data" form of the browsable API
-            # from rendering `"foo": null` for read only fields
-            try:
-                resource[field_name]
-            except KeyError:
-                if fields[field_name].read_only:
-                    continue
+        Ensures that ID which is always provided in a JSON:API resource object
+        and relationships are not returned.
+        """
 
-            data.update({field_name: resource.get(field_name)})
+        invalid_fields = {"id", api_settings.URL_FIELD_NAME}
 
-        return utils.format_field_names(data)
+        return {
+            format_field_name(field_name): value
+            for field_name, value in resource.items()
+            if field_name in fields
+            and field_name not in invalid_fields
+            and not is_relationship_field(fields[field_name])
+        }
 
     @classmethod
     def extract_relationships(cls, fields, resource, resource_instance):
         """
         Builds the relationships top level object based on related serializers.
         """
         # Avoid circular deps
@@ -102,22 +105,22 @@
                 continue
 
             # don't output a key for write only fields
             if fields[field_name].write_only:
                 continue
 
             # Skip fields without relations
-            if not utils.is_relationship_field(field):
+            if not is_relationship_field(field):
                 continue
 
             source = field.source
-            relation_type = utils.get_related_resource_type(field)
+            relation_type = get_related_resource_type(field)
 
             if isinstance(field, relations.HyperlinkedIdentityField):
-                resolved, relation_instance = utils.get_relation_instance(
+                resolved, relation_instance = get_relation_instance(
                     resource_instance, source, field.parent
                 )
                 if not resolved:
                     continue
                 # special case for HyperlinkedIdentityField
                 relation_data = list()
 
@@ -161,15 +164,15 @@
                 data.update({field_name: relation_data})
                 continue
 
             if isinstance(
                 field,
                 (relations.PrimaryKeyRelatedField, relations.HyperlinkedRelatedField),
             ):
-                resolved, relation = utils.get_relation_instance(
+                resolved, relation = get_relation_instance(
                     resource_instance, f"{source}_id", field.parent
                 )
                 if not resolved:
                     continue
                 relation_id = relation if resource.get(field_name) else None
                 relation_data = {"data": None}
                 if relation_id is not None:
@@ -184,15 +187,15 @@
                     relation_data.update(
                         {"links": {"related": resource.get(field_name)}}
                     )
                 data.update({field_name: relation_data})
                 continue
 
             if isinstance(field, relations.ManyRelatedField):
-                resolved, relation_instance = utils.get_relation_instance(
+                resolved, relation_instance = get_relation_instance(
                     resource_instance, source, field.parent
                 )
                 if not resolved:
                     continue
 
                 relation_data = {}
 
@@ -217,17 +220,15 @@
                     data.update({field_name: relation_data})
                     continue
 
                 relation_data = list()
                 for nested_resource_instance in relation_instance:
                     nested_resource_instance_type = (
                         relation_type
-                        or utils.get_resource_type_from_instance(
-                            nested_resource_instance
-                        )
+                        or get_resource_type_from_instance(nested_resource_instance)
                     )
 
                     relation_data.append(
                         {
                             "type": nested_resource_instance_type,
                             "id": force_str(nested_resource_instance.pk),
                         }
@@ -238,15 +239,15 @@
                             "data": relation_data,
                             "meta": {"count": len(relation_data)},
                         }
                     }
                 )
                 continue
 
-        return utils.format_field_names(data)
+        return format_field_names(data)
 
     @classmethod
     def extract_relation_instance(cls, field, resource_instance):
         """
         Determines what instance represents given relation and extracts it.
 
         Relation instance is determined exactly same way as it determined
@@ -284,15 +285,15 @@
 
         for field_name, field in iter(fields.items()):
             # Skip URL field
             if field_name == api_settings.URL_FIELD_NAME:
                 continue
 
             # Skip fields without relations
-            if not utils.is_relationship_field(field):
+            if not is_relationship_field(field):
                 continue
 
             try:
                 included_resources.remove(field_name)
             except ValueError:
                 # Skip fields not in requested included resources
                 # If no child field, directly continue with the next field
@@ -336,28 +337,26 @@
                 key.replace(f"{field_name}.", "", 1)
                 for key in included_resources
                 if field_name == key.split(".")[0]
             ]
 
             if isinstance(field, ListSerializer):
                 serializer = field.child
-                relation_type = utils.get_resource_type_from_serializer(serializer)
+                relation_type = get_resource_type_from_serializer(serializer)
                 relation_queryset = list(relation_instance)
 
                 if serializer_data:
                     for position in range(len(serializer_data)):
                         serializer_resource = serializer_data[position]
                         nested_resource_instance = relation_queryset[position]
                         resource_type = (
                             relation_type
-                            or utils.get_resource_type_from_instance(
-                                nested_resource_instance
-                            )
+                            or get_resource_type_from_instance(nested_resource_instance)
                         )
-                        serializer_fields = utils.get_serializer_fields(
+                        serializer_fields = get_serializer_fields(
                             serializer.__class__(
                                 nested_resource_instance, context=serializer.context
                             )
                         )
                         new_item = cls.build_json_resource_obj(
                             serializer_fields,
                             serializer_resource,
@@ -373,18 +372,18 @@
                             serializer_resource,
                             nested_resource_instance,
                             new_included_resources,
                             included_cache,
                         )
 
             if isinstance(field, Serializer):
-                relation_type = utils.get_resource_type_from_serializer(field)
+                relation_type = get_resource_type_from_serializer(field)
 
                 # Get the serializer fields
-                serializer_fields = utils.get_serializer_fields(field)
+                serializer_fields = get_serializer_fields(field)
                 if serializer_data:
                     new_item = cls.build_json_resource_obj(
                         serializer_fields,
                         serializer_data,
                         relation_instance,
                         relation_type,
                         field,
@@ -409,15 +408,16 @@
         if hasattr(serializer, "child"):
             meta = getattr(serializer.child, "Meta", None)
         else:
             meta = getattr(serializer, "Meta", None)
         meta_fields = getattr(meta, "meta_fields", [])
         data = {}
         for field_name in meta_fields:
-            data.update({field_name: resource.get(field_name)})
+            if field_name in resource:
+                data.update({field_name: resource[field_name]})
         return data
 
     @classmethod
     def extract_root_meta(cls, serializer, resource):
         """
         Calls a `get_root_meta` function on a serializer, if it exists.
         """
@@ -430,73 +430,97 @@
         if getattr(serializer, "get_root_meta", None):
             json_api_meta = serializer.get_root_meta(resource, many)
             assert isinstance(json_api_meta, dict), "get_root_meta must return a dict"
             data.update(json_api_meta)
         return data
 
     @classmethod
+    def _filter_sparse_fields(cls, serializer, fields, resource_name):
+        request = serializer.context.get("request")
+        if request:
+            sparse_fieldset_query_param = f"fields[{resource_name}]"
+            sparse_fieldset_value = request.query_params.get(
+                sparse_fieldset_query_param
+            )
+            if sparse_fieldset_value:
+                sparse_fields = sparse_fieldset_value.split(",")
+                return {
+                    field_name: field
+                    for field_name, field, in fields.items()
+                    if field_name in sparse_fields
+                }
+
+        return fields
+
+    @classmethod
     def build_json_resource_obj(
         cls,
         fields,
         resource,
         resource_instance,
         resource_name,
         serializer,
         force_type_resolution=False,
     ):
         """
         Builds the resource object (type, id, attributes) and extracts relationships.
         """
         # Determine type from the instance if the underlying model is polymorphic
         if force_type_resolution:
-            resource_name = utils.get_resource_type_from_instance(resource_instance)
+            resource_name = get_resource_type_from_instance(resource_instance)
         resource_data = {
             "type": resource_name,
-            "id": utils.get_resource_id(resource_instance, resource),
-            "attributes": cls.extract_attributes(fields, resource),
+            "id": get_resource_id(resource_instance, resource),
         }
+
+        # TODO remove this filter by rewriting extract_relationships
+        # so it uses the serialized data as a basis
+        fields = cls._filter_sparse_fields(serializer, fields, resource_name)
+        attributes = cls.extract_attributes(fields, resource)
+        if attributes:
+            resource_data["attributes"] = attributes
         relationships = cls.extract_relationships(fields, resource, resource_instance)
         if relationships:
             resource_data["relationships"] = relationships
         # Add 'self' link if field is present and valid
         if api_settings.URL_FIELD_NAME in resource and isinstance(
             fields[api_settings.URL_FIELD_NAME], relations.RelatedField
         ):
             resource_data["links"] = {"self": resource[api_settings.URL_FIELD_NAME]}
 
         meta = cls.extract_meta(serializer, resource)
         if meta:
-            resource_data["meta"] = utils.format_field_names(meta)
+            resource_data["meta"] = format_field_names(meta)
 
         return resource_data
 
     def render_relationship_view(
         self, data, accepted_media_type=None, renderer_context=None
     ):
         # Special case for RelationshipView
         view = renderer_context.get("view", None)
         render_data = {"data": data}
         links = view.get_links()
         if links:
-            render_data.update({"links": links}),
+            render_data["links"] = links
         return super().render(render_data, accepted_media_type, renderer_context)
 
     def render_errors(self, data, accepted_media_type=None, renderer_context=None):
         return super().render(
-            utils.format_errors(data), accepted_media_type, renderer_context
+            format_errors(data), accepted_media_type, renderer_context
         )
 
     def render(self, data, accepted_media_type=None, renderer_context=None):
         renderer_context = renderer_context or {}
 
         view = renderer_context.get("view", None)
         request = renderer_context.get("request", None)
 
         # Get the resource name.
-        resource_name = utils.get_resource_name(renderer_context)
+        resource_name = get_resource_name(renderer_context)
 
         # If this is an error response, skip the rest.
         if resource_name == "errors":
             return self.render_errors(data, accepted_media_type, renderer_context)
 
         # if response.status_code is 204 then the data to be rendered must
         # be None
@@ -524,15 +548,15 @@
         if data and "results" in data:
             serializer_data = data["results"]
         else:
             serializer_data = data
 
         serializer = getattr(serializer_data, "serializer", None)
 
-        included_resources = utils.get_included_resources(request, serializer)
+        included_resources = get_included_resources(request, serializer)
 
         if serializer is not None:
             # Extract root meta for any type of serializer
             json_api_meta.update(self.extract_root_meta(serializer, serializer_data))
 
             if getattr(serializer, "many", False):
                 json_api_data = list()
@@ -551,15 +575,15 @@
                             serializer.child.get_polymorphic_serializer_for_instance(
                                 resource_instance
                             )(context=serializer.child.context)
                         )
                     else:
                         resource_serializer_class = serializer.child
 
-                    fields = utils.get_serializer_fields(resource_serializer_class)
+                    fields = get_serializer_fields(resource_serializer_class)
                     force_type_resolution = getattr(
                         resource_serializer_class, "_poly_force_type_resolution", False
                     )
 
                     json_resource_obj = self.build_json_resource_obj(
                         fields,
                         resource,
@@ -574,15 +598,15 @@
                         fields,
                         resource,
                         resource_instance,
                         included_resources,
                         included_cache,
                     )
             else:
-                fields = utils.get_serializer_fields(serializer)
+                fields = get_serializer_fields(serializer)
                 force_type_resolution = getattr(
                     serializer, "_poly_force_type_resolution", False
                 )
 
                 resource_instance = serializer.instance
                 json_api_data = self.build_json_resource_obj(
                     fields,
@@ -633,15 +657,15 @@
             for included_type in sorted(included_cache.keys()):
                 for included_id in sorted(included_cache[included_type].keys()):
                     render_data["included"].append(
                         included_cache[included_type][included_id]
                     )
 
         if json_api_meta:
-            render_data["meta"] = utils.format_field_names(json_api_meta)
+            render_data["meta"] = format_field_names(json_api_meta)
 
         return super().render(render_data, accepted_media_type, renderer_context)
 
 
 class BrowsableAPIRenderer(renderers.BrowsableAPIRenderer):
     template = "rest_framework_json_api/api.html"
     includes_template = "rest_framework_json_api/includes.html"
@@ -683,14 +707,13 @@
         try:
             if "related_field" in view.kwargs:
                 serializer_class = view.get_related_serializer_class()
             else:
                 serializer_class = view.get_serializer_class()
         except AttributeError:
             return
-
         if not hasattr(serializer_class, "included_serializers"):
             return
 
         template = loader.get_template(self.includes_template)
         context = {"elements": self._get_included_serializers(serializer_class)}
         return template.render(context)
```

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/schemas/openapi.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/schemas/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from rest_framework.fields import empty
 from rest_framework.relations import ManyRelatedField
 from rest_framework.schemas import openapi as drf_openapi
 from rest_framework.schemas.utils import is_list_view
 
 from rest_framework_json_api import serializers, views
-from rest_framework_json_api.compat import get_reference
 from rest_framework_json_api.relations import ManySerializerMethodResourceRelatedField
 from rest_framework_json_api.utils import format_field_name
 
 
 class SchemaGenerator(drf_openapi.SchemaGenerator):
     """
     Extend DRF's SchemaGenerator to implement JSON:API flavored generateschema command.
@@ -529,20 +528,18 @@
         :param collection: True for collections; False for individual items.
 
         Uses a $ref to the components.schemas.<Name> component definition.
         """
         if collection:
             data = {
                 "type": "array",
-                "items": get_reference(
-                    self, self.get_response_serializer(path, method)
-                ),
+                "items": self.get_reference(self.get_response_serializer(path, method)),
             }
         else:
-            data = get_reference(self, self.get_response_serializer(path, method))
+            data = self.get_reference(self.get_response_serializer(path, method))
 
         return {
             "description": operation["operationId"],
             "content": {
                 "application/vnd.api+json": {
                     "schema": {
                         "type": "object",
@@ -677,14 +674,22 @@
         """
         Custom map_serializer that serializes the schema using the JSON:API spec.
 
         Non-attributes like related and identity fields, are moved to 'relationships'
         and 'links'.
         """
         # TODO: remove attributes, etc. for relationshipView??
+        if isinstance(
+            serializer.parent, (serializers.ListField, serializers.BaseSerializer)
+        ):
+            # Return plain non-JSON:API serializer schema for serializers nested inside
+            # a Serializer or a ListField, as those don't use the full JSON:API
+            # serializer schemas.
+            return super().map_serializer(serializer)
+
         required = []
         attributes = {}
         relationships_required = []
         relationships = {}
 
         for field in serializer.fields.values():
             if isinstance(field, serializers.HyperlinkedIdentityField):
```

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/serializers.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,43 +71,40 @@
 class SparseFieldsetsMixin:
     """
     A serializer mixin that adds support for sparse fieldsets through `fields` query parameter.
 
     Specification: https://jsonapi.org/format/#fetching-sparse-fieldsets
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        context = kwargs.get("context")
-        request = context.get("request") if context else None
+    @property
+    def _readable_fields(self):
+        request = self.context.get("request") if self.context else None
+        readable_fields = super()._readable_fields
 
         if request:
-            sparse_fieldset_query_param = "fields[{}]".format(
-                get_resource_type_from_serializer(self)
-            )
             try:
-                param_name = next(
-                    key
-                    for key in request.query_params
-                    if sparse_fieldset_query_param == key
+                resource_type = get_resource_type_from_serializer(self)
+                sparse_fieldset_query_param = f"fields[{resource_type}]"
+
+                sparse_fieldset_value = request.query_params.get(
+                    sparse_fieldset_query_param
                 )
-            except StopIteration:
+                if sparse_fieldset_value:
+                    sparse_fields = sparse_fieldset_value.split(",")
+                    return (
+                        field
+                        for field in readable_fields
+                        if field.field_name in sparse_fields
+                        or field.field_name == api_settings.URL_FIELD_NAME
+                    )
+            except AttributeError:
+                # no type on serializer, must be used only as only nested
                 pass
-            else:
-                fieldset = request.query_params.get(param_name).split(",")
-                # iterate over a *copy* of self.fields' underlying dict, because we may
-                # modify the original during the iteration.
-                # self.fields is a `rest_framework.utils.serializer_helpers.BindingDict`
-                for field_name, _field in self.fields.fields.copy().items():
-                    if (
-                        field_name == api_settings.URL_FIELD_NAME
-                    ):  # leave self link there
-                        continue
-                    if field_name not in fieldset:
-                        self.fields.pop(field_name)
+
+        return readable_fields
 
 
 class IncludedResourcesValidationMixin:
     """
     A serializer mixin that adds validation of `include` query parameter to
     support compound documents.
 
@@ -305,19 +302,19 @@
     def get_field_names(self, declared_fields, info):
         """
         We override the parent to omit explicity defined meta fields (such
         as SerializerMethodFields) from the list of declared fields
         """
         meta_fields = getattr(self.Meta, "meta_fields", [])
 
-        declared = {}
-        for field_name in set(declared_fields.keys()):
-            field = declared_fields[field_name]
-            if field_name not in meta_fields:
-                declared[field_name] = field
+        declared = {
+            field_name: field
+            for field_name, field in declared_fields.items()
+            if field_name not in meta_fields
+        }
         fields = super().get_field_names(declared, info)
         return list(fields) + list(getattr(self.Meta, "meta_fields", list()))
 
 
 class PolymorphicSerializerMetaclass(SerializerMetaclass):
     """
     This metaclass ensures that the `polymorphic_serializers` is correctly defined on a
```

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/settings.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/templates/rest_framework_json_api/api.html` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/templates/rest_framework_json_api/api.html`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/templates/rest_framework_json_api/includes.html` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/templates/rest_framework_json_api/includes.html`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/utils.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,35 +377,36 @@
     errors = []
     # handle generic errors. ValidationError('test') in a view for example
     if isinstance(response.data, list):
         for message in response.data:
             errors.extend(format_error_object(message, "/data", response))
     # handle all errors thrown from serializers
     else:
-        # Avoid circular deps
-        from rest_framework import generics
-
-        has_serializer = isinstance(context["view"], generics.GenericAPIView)
-        if has_serializer:
+        try:
             serializer = context["view"].get_serializer()
             fields = get_serializer_fields(serializer) or dict()
             relationship_fields = [
                 format_field_name(name)
                 for name, field in fields.items()
                 if is_relationship_field(field)
             ]
+        except Exception:
+            # ignore potential errors when retrieving serializer
+            # as it might shadow error which is currently being
+            # formatted
+            serializer = None
 
         for field, error in response.data.items():
             non_field_error = field == api_settings.NON_FIELD_ERRORS_KEY
             field = format_field_name(field)
             pointer = None
             if non_field_error:
                 # Serializer error does not refer to a specific field.
                 pointer = "/data"
-            elif has_serializer:
+            elif serializer:
                 # pointer can be determined only if there's a serializer.
                 rel = "relationships" if field in relationship_fields else "attributes"
                 pointer = f"/data/{rel}/{field}"
             if isinstance(exc, Http404) and isinstance(error, str):
                 # 404 errors don't have a pointer
                 errors.extend(format_error_object(error, None, response))
             elif isinstance(error, str):
```

### Comparing `djangorestframework-jsonapi-6.1.0/rest_framework_json_api/views.py` & `djangorestframework-jsonapi-7.0.0/rest_framework_json_api/views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/setup.cfg` & `djangorestframework-jsonapi-7.0.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -54,17 +54,15 @@
 	def __repr__
 
 [tool:pytest]
 DJANGO_SETTINGS_MODULE = example.settings.test
 filterwarnings = 
 	error::DeprecationWarning
 	error::PendingDeprecationWarning
-	ignore:The django.utils.timezone.utc alias is deprecated.
-	ignore:pkg_resources is deprecated as an API
-	ignore:Deprecated call to `pkg_resource
+	ignore:Built-in schema generation is deprecated.
 testpaths = 
 	example
 	tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `djangorestframework-jsonapi-6.1.0/setup.py` & `djangorestframework-jsonapi-7.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -82,30 +82,39 @@
         "Environment :: Web Environment",
         "Framework :: Django",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
+    project_urls={
+        "Documentation": "https://django-rest-framework-json-api.readthedocs.org/",
+        "Changelog": (
+            "https://github.com/django-json-api/django-rest-framework-json-api/"
+            "blob/main/CHANGELOG.md"
+        ),
+        "Source": "https://github.com/django-json-api/django-rest-framework-json-api",
+        "Tracker": "https://github.com/django-json-api/django-rest-framework-json-api/issues",
+    },
     install_requires=[
         "inflection>=0.5.0",
-        "djangorestframework>=3.13",
-        "django>=3.2",
+        "djangorestframework>=3.14",
+        "django>=4.2",
     ],
     extras_require={
         "django-polymorphic": ["django-polymorphic>=3.0"],
         "django-filter": ["django-filter>=2.4"],
         "openapi": ["pyyaml>=5.4", "uritemplate>=3.0.1"],
     },
     setup_requires=wheel,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     zip_safe=False,
 )
```

### Comparing `djangorestframework-jsonapi-6.1.0/tests/conftest.py` & `djangorestframework-jsonapi-7.0.0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import pytest
 from rest_framework.test import APIClient
 
 from tests.models import (
     BasicModel,
+    ForeignKeySource,
     ForeignKeyTarget,
     ManyToManySource,
     ManyToManyTarget,
+    NestedRelatedSource,
 )
 
 
 @pytest.fixture(autouse=True)
 def use_rest_framework_json_api_defaults(settings):
     """
     Enfroce default settings for tests modules.
@@ -36,14 +38,19 @@
 
 @pytest.fixture
 def foreign_key_target(db):
     return ForeignKeyTarget.objects.create(name="Target")
 
 
 @pytest.fixture
+def foreign_key_source(db, foreign_key_target):
+    return ForeignKeySource.objects.create(name="Source", target=foreign_key_target)
+
+
+@pytest.fixture
 def many_to_many_source(db, many_to_many_targets):
     source = ManyToManySource.objects.create(name="Source")
     source.targets.add(*many_to_many_targets)
     return source
 
 
 @pytest.fixture
@@ -51,9 +58,37 @@
     return [
         ManyToManyTarget.objects.create(name="Target1"),
         ManyToManyTarget.objects.create(name="Target2"),
     ]
 
 
 @pytest.fixture
+def many_to_many_sources(db, many_to_many_targets):
+    source1 = ManyToManySource.objects.create(name="Source1")
+    source2 = ManyToManySource.objects.create(name="Source2")
+
+    source1.targets.add(*many_to_many_targets)
+    source2.targets.add(*many_to_many_targets)
+
+    return [source1, source2]
+
+
+@pytest.fixture
+def nested_related_source(
+    db,
+    foreign_key_source,
+    foreign_key_target,
+    many_to_many_targets,
+    many_to_many_sources,
+):
+    source = NestedRelatedSource.objects.create(
+        fk_source=foreign_key_source, fk_target=foreign_key_target
+    )
+    source.m2m_targets.add(*many_to_many_targets)
+    source.m2m_sources.add(*many_to_many_sources)
+
+    return source
+
+
+@pytest.fixture
 def client():
     return APIClient()
```

### Comparing `djangorestframework-jsonapi-6.1.0/tests/models.py` & `djangorestframework-jsonapi-7.0.0/tests/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     name = models.CharField(max_length=100)
     target = models.ForeignKey(
         ForeignKeyTarget, related_name="sources", on_delete=models.CASCADE
     )
 
 
 class NestedRelatedSource(DJAModel):
-    m2m_source = models.ManyToManyField(ManyToManySource, related_name="nested_source")
+    m2m_sources = models.ManyToManyField(ManyToManySource, related_name="nested_source")
     fk_source = models.ForeignKey(
         ForeignKeySource, related_name="nested_source", on_delete=models.CASCADE
     )
-    m2m_target = models.ManyToManyField(ManyToManySource, related_name="nested_target")
+    m2m_targets = models.ManyToManyField(ManyToManyTarget, related_name="nested_target")
     fk_target = models.ForeignKey(
-        ForeignKeySource, related_name="nested_target", on_delete=models.CASCADE
+        ForeignKeyTarget, related_name="nested_target", on_delete=models.CASCADE
     )
```

### Comparing `djangorestframework-jsonapi-6.1.0/tests/serializers.py` & `djangorestframework-jsonapi-7.0.0/tests/serializers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,72 @@
 from rest_framework_json_api import serializers
-from rest_framework_json_api.relations import ResourceRelatedField
 from tests.models import (
     BasicModel,
     ForeignKeySource,
     ForeignKeyTarget,
     ManyToManySource,
     ManyToManyTarget,
+    NestedRelatedSource,
 )
 
 
 class BasicModelSerializer(serializers.ModelSerializer):
     class Meta:
         fields = ("text",)
         model = BasicModel
 
 
+class ForeignKeyTargetSerializer(serializers.ModelSerializer):
+    class Meta:
+        fields = ("name",)
+        model = ForeignKeyTarget
+
+
 class ForeignKeySourceSerializer(serializers.ModelSerializer):
-    target = ResourceRelatedField(queryset=ForeignKeyTarget.objects)
+    included_serializers = {"target": ForeignKeyTargetSerializer}
 
     class Meta:
         model = ForeignKeySource
-        fields = ("target",)
+        fields = (
+            "name",
+            "target",
+        )
+
+
+class ManyToManyTargetSerializer(serializers.ModelSerializer):
+    class Meta:
+        fields = ("name",)
+        model = ManyToManyTarget
 
 
 class ManyToManySourceSerializer(serializers.ModelSerializer):
-    targets = ResourceRelatedField(many=True, queryset=ManyToManyTarget.objects)
+    included_serializers = {"targets": "tests.serializers.ManyToManyTargetSerializer"}
 
     class Meta:
         model = ManyToManySource
         fields = ("targets",)
 
 
-class ManyToManyTargetSerializer(serializers.ModelSerializer):
+class ManyToManySourceReadOnlySerializer(serializers.ModelSerializer):
     class Meta:
-        model = ManyToManyTarget
+        model = ManyToManySource
+        fields = ("targets",)
 
 
-class ManyToManySourceReadOnlySerializer(serializers.ModelSerializer):
-    targets = ResourceRelatedField(many=True, read_only=True)
+class NestedRelatedSourceSerializer(serializers.ModelSerializer):
+    included_serializers = {
+        "m2m_sources": ManyToManySourceSerializer,
+        "fk_source": ForeignKeySourceSerializer,
+        "m2m_targets": ManyToManyTargetSerializer,
+        "fk_target": ForeignKeyTargetSerializer,
+    }
 
     class Meta:
-        model = ManyToManySource
-        fields = ("targets",)
+        model = NestedRelatedSource
+        fields = ("m2m_sources", "fk_source", "m2m_targets", "fk_target")
 
 
 class CallableDefaultSerializer(serializers.Serializer):
     field = serializers.CharField(default=serializers.CreateOnlyDefault("default"))
 
     class Meta:
         fields = ("field",)
```

### Comparing `djangorestframework-jsonapi-6.1.0/tests/test_pagination.py` & `djangorestframework-jsonapi-7.0.0/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/tests/test_parsers.py` & `djangorestframework-jsonapi-7.0.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-jsonapi-6.1.0/tests/test_relations.py` & `djangorestframework-jsonapi-7.0.0/tests/test_relations.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     )
     def test_serialize(
         self, format_type, pluralize_type, resource_type, foreign_key_target, settings
     ):
         settings.JSON_API_FORMAT_TYPES = format_type
         settings.JSON_API_PLURALIZE_TYPES = pluralize_type
 
-        serializer = ForeignKeySourceSerializer(instance={"target": foreign_key_target})
+        serializer = ForeignKeySourceSerializer(
+            instance={"target": foreign_key_target, "name": "Test"}
+        )
         expected = {
             "type": resource_type,
             "id": str(foreign_key_target.pk),
         }
 
         assert serializer.data["target"] == expected
 
@@ -81,15 +83,18 @@
     def test_deserialize(
         self, format_type, pluralize_type, resource_type, foreign_key_target, settings
     ):
         settings.JSON_API_FORMAT_TYPES = format_type
         settings.JSON_API_PLURALIZE_TYPES = pluralize_type
 
         serializer = ForeignKeySourceSerializer(
-            data={"target": {"type": resource_type, "id": str(foreign_key_target.pk)}}
+            data={
+                "target": {"type": resource_type, "id": str(foreign_key_target.pk)},
+                "name": "Test",
+            }
         )
 
         assert serializer.is_valid()
         assert serializer.validated_data["target"] == foreign_key_target
 
     @pytest.mark.parametrize(
         "format_type,pluralize_type,resource_type",
@@ -187,15 +192,17 @@
             (
                 {"id": "1234"},
                 "Invalid resource identifier object: missing 'type' attribute",
             ),
         ],
     )
     def test_invalid_resource_id_object(self, resource_identifier, error):
-        serializer = ForeignKeySourceSerializer(data={"target": resource_identifier})
+        serializer = ForeignKeySourceSerializer(
+            data={"target": resource_identifier, "name": "Test"}
+        )
         assert not serializer.is_valid()
         assert serializer.errors == {"target": [error]}
 
 
 class TestHyperlinkedRelatedField:
     @pytest.fixture
     def instance(self):
```

### Comparing `djangorestframework-jsonapi-6.1.0/tests/test_utils.py` & `djangorestframework-jsonapi-7.0.0/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
     [
         (
             "m2m_source.targets",
             "ManyToManyTarget",
             {"many": True, "queryset": ManyToManyTarget.objects.all()},
         ),
         (
-            "m2m_target.sources.",
+            "m2m_target.sources",
             "ManyToManySource",
             {"many": True, "queryset": ManyToManySource.objects.all()},
         ),
         (
             "fk_source.target",
             "ForeignKeyTarget",
             {"many": True, "queryset": ForeignKeyTarget.objects.all()},
```

