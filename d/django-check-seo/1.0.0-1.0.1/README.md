# Comparing `tmp/django-check-seo-1.0.0.tar.gz` & `tmp/django_check_seo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-check-seo-1.0.0.tar", last modified: Thu Jan 25 12:57:58 2024, max compression
+gzip compressed data, was "django_check_seo-1.0.1.tar", last modified: Thu May  2 11:14:40 2024, max compression
```

## Comparing `django-check-seo-1.0.0.tar` & `django_check_seo-1.0.1.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.691319 django-check-seo-1.0.0/
--rw-r--r--   0 kapt      (1000) kapt      (1000)       93 2024-01-25 12:57:38.000000 django-check-seo-1.0.0/.bumpversion.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)      365 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/.coveragerc
--rw-r--r--   0 kapt      (1000) kapt      (1000)       74 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/.flake8
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.679319 django-check-seo-1.0.0/.github/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.683319 django-check-seo-1.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      834 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)      595 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)      130 2021-09-09 16:31:58.000000 django-check-seo-1.0.0/.gitignore
--rw-r--r--   0 kapt      (1000) kapt      (1000)      113 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/.isort.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)      870 2023-12-18 16:46:38.000000 django-check-seo-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 kapt      (1000) kapt      (1000)       78 2021-09-09 16:31:58.000000 django-check-seo-1.0.0/AUTHORS.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)    18244 2024-01-25 12:57:42.000000 django-check-seo-1.0.0/CHANGELOG.rst
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1554 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)    35149 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/LICENSE
--rw-r--r--   0 kapt      (1000) kapt      (1000)      220 2022-06-14 08:10:41.000000 django-check-seo-1.0.0/MANIFEST.in
--rw-r--r--   0 kapt      (1000) kapt      (1000)     7529 2024-01-25 12:57:58.691319 django-check-seo-1.0.0/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6311 2024-01-25 12:57:06.000000 django-check-seo-1.0.0/README.md
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.683319 django-check-seo-1.0.0/django_check_seo/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      112 2023-12-18 16:45:41.000000 django-check-seo-1.0.0/django_check_seo/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      181 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/apps.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.687319 django-check-seo-1.0.0/django_check_seo/checks/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/checks/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      320 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/checks/custom_list.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1778 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/checks/site.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.687319 django-check-seo-1.0.0/django_check_seo/checks_list/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      418 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/checks_list/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     7826 2023-03-03 15:45:59.000000 django-check-seo-1.0.0/django_check_seo/checks_list/check_description.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4001 2022-06-14 09:17:55.000000 django-check-seo-1.0.0/django_check_seo/checks_list/check_h1.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3793 2022-06-14 09:17:55.000000 django-check-seo-1.0.0/django_check_seo/checks_list/check_h2.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2914 2022-06-14 09:27:26.000000 django-check-seo-1.0.0/django_check_seo/checks_list/check_images.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3931 2022-06-14 09:17:55.000000 django-check-seo-1.0.0/django_check_seo/checks_list/check_keyword_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1928 2023-04-19 13:25:13.000000 django-check-seo-1.0.0/django_check_seo/checks_list/check_keywords.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4092 2022-06-14 09:17:55.000000 django-check-seo-1.0.0/django_check_seo/checks_list/check_links.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5709 2022-06-14 09:17:55.000000 django-check-seo-1.0.0/django_check_seo/checks_list/check_title.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3367 2022-06-14 09:17:55.000000 django-check-seo-1.0.0/django_check_seo/checks_list/check_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2018 2022-06-14 09:17:55.000000 django-check-seo-1.0.0/django_check_seo/checks_list/content_words_number.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2453 2022-06-14 09:17:55.000000 django-check-seo-1.0.0/django_check_seo/checks_list/keyword_present_first_paragraph.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2052 2022-09-21 15:03:12.000000 django-check-seo-1.0.0/django_check_seo/checks_list/launch_checks.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      668 2023-03-03 15:45:59.000000 django-check-seo-1.0.0/django_check_seo/cms_toolbars.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.687319 django-check-seo-1.0.0/django_check_seo/conf/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/conf/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      815 2022-06-14 08:53:12.000000 django-check-seo-1.0.0/django_check_seo/conf/settings.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.679319 django-check-seo-1.0.0/django_check_seo/locale/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.679319 django-check-seo-1.0.0/django_check_seo/locale/fr/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.687319 django-check-seo-1.0.0/django_check_seo/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    16533 2022-06-14 09:38:51.000000 django-check-seo-1.0.0/django_check_seo/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt      (1000) kapt      (1000)    24514 2022-06-14 09:38:24.000000 django-check-seo-1.0.0/django_check_seo/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.687319 django-check-seo-1.0.0/django_check_seo/migrations/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      976 2024-01-25 12:49:58.000000 django-check-seo-1.0.0/django_check_seo/migrations/0001_initial.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/migrations/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      532 2024-01-25 12:49:58.000000 django-check-seo-1.0.0/django_check_seo/models.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.679319 django-check-seo-1.0.0/django_check_seo/static/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.687319 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4734 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/design.css
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.691319 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    11358 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/LICENCE
--rw-r--r--   0 kapt      (1000) kapt      (1000)      139 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/NOTICE
--rw-r--r--   0 kapt      (1000) kapt      (1000)   164936 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   163448 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   162636 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   158604 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   122512 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)    15388 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/logo-small.png
--rw-r--r--   0 kapt      (1000) kapt      (1000)   137074 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/django_check_seo/static/django-check-seo/logo.png
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.679319 django-check-seo-1.0.0/django_check_seo/templates/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.691319 django-check-seo-1.0.0/django_check_seo/templates/django_check_seo/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3439 2024-01-25 12:27:47.000000 django-check-seo-1.0.0/django_check_seo/templates/django_check_seo/default.html
--rw-r--r--   0 kapt      (1000) kapt      (1000)      705 2024-01-25 12:33:00.000000 django-check-seo-1.0.0/django_check_seo/templates/django_check_seo/element.html
--rw-r--r--   0 kapt      (1000) kapt      (1000)      603 2024-01-25 12:41:13.000000 django-check-seo-1.0.0/django_check_seo/urls.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3110 2024-01-25 12:49:59.000000 django-check-seo-1.0.0/django_check_seo/views.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.691319 django-check-seo-1.0.0/django_check_seo.egg-info/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     7529 2024-01-25 12:57:58.000000 django-check-seo-1.0.0/django_check_seo.egg-info/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2595 2024-01-25 12:57:58.000000 django-check-seo-1.0.0/django_check_seo.egg-info/SOURCES.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2024-01-25 12:57:58.000000 django-check-seo-1.0.0/django_check_seo.egg-info/dependency_links.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       59 2024-01-25 12:57:58.000000 django-check-seo-1.0.0/django_check_seo.egg-info/requires.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       17 2024-01-25 12:57:58.000000 django-check-seo-1.0.0/django_check_seo.egg-info/top_level.txt
--rwxr-xr-x   0 kapt      (1000) kapt      (1000)     4701 2022-09-21 15:17:31.000000 django-check-seo-1.0.0/launch_tests.sh
--rw-r--r--   0 kapt      (1000) kapt      (1000)       94 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/pytest.ini
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1099 2024-01-25 12:57:58.691319 django-check-seo-1.0.0/setup.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)       52 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/setup.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-01-25 12:57:58.691319 django-check-seo-1.0.0/tests/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    16223 2021-09-09 16:31:52.000000 django-check-seo-1.0.0/tests/test_content_words_number.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     9522 2021-09-09 16:31:52.000000 django-check-seo-1.0.0/tests/test_description.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6045 2021-09-09 16:31:52.000000 django-check-seo-1.0.0/tests/test_h1.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6469 2021-09-09 16:31:52.000000 django-check-seo-1.0.0/tests/test_h2.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4439 2021-09-09 16:31:52.000000 django-check-seo-1.0.0/tests/test_images.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5135 2021-09-09 16:31:52.000000 django-check-seo-1.0.0/tests/test_keyword_present_first_paragraph.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5989 2021-09-09 16:31:58.000000 django-check-seo-1.0.0/tests/test_keyword_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2476 2021-09-09 16:31:52.000000 django-check-seo-1.0.0/tests/test_keywords.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6480 2021-09-09 16:31:52.000000 django-check-seo-1.0.0/tests/test_links.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     7288 2021-09-09 16:31:52.000000 django-check-seo-1.0.0/tests/test_title.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3672 2021-09-09 16:31:52.000000 django-check-seo-1.0.0/tests/test_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      618 2021-09-08 08:29:05.000000 django-check-seo-1.0.0/tests_settings.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.116728 django_check_seo-1.0.1/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       93 2024-05-02 11:14:11.000000 django_check_seo-1.0.1/.bumpversion.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      365 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/.coveragerc
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       74 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/.flake8
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    10273 2024-02-01 09:04:43.000000 django_check_seo-1.0.1/.gitchangelog.rc
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.084727 django_check_seo-1.0.1/.github/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.096727 django_check_seo-1.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      834 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      595 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      130 2021-09-09 16:31:58.000000 django_check_seo-1.0.1/.gitignore
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      113 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/.isort.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      870 2024-02-02 15:24:28.000000 django_check_seo-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       78 2021-09-09 16:31:58.000000 django_check_seo-1.0.1/AUTHORS.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    18702 2024-05-02 11:14:15.000000 django_check_seo-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1554 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    35149 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/LICENSE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      220 2022-06-14 08:10:41.000000 django_check_seo-1.0.1/MANIFEST.in
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     7416 2024-05-02 11:14:40.116728 django_check_seo-1.0.1/PKG-INFO
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6276 2024-02-02 15:26:44.000000 django_check_seo-1.0.1/README.md
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.096727 django_check_seo-1.0.1/django_check_seo/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      112 2024-02-02 15:24:28.000000 django_check_seo-1.0.1/django_check_seo/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      181 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/apps.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.100727 django_check_seo-1.0.1/django_check_seo/checks/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/checks/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      320 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/checks/custom_list.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1778 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/checks/site.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.104728 django_check_seo-1.0.1/django_check_seo/checks_list/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      418 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/checks_list/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     7823 2024-05-02 11:13:44.000000 django_check_seo-1.0.1/django_check_seo/checks_list/check_description.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4003 2024-05-02 11:09:19.000000 django_check_seo-1.0.1/django_check_seo/checks_list/check_h1.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3795 2024-05-02 11:09:26.000000 django_check_seo-1.0.1/django_check_seo/checks_list/check_h2.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2914 2022-06-14 09:27:26.000000 django_check_seo-1.0.1/django_check_seo/checks_list/check_images.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3935 2024-05-02 11:09:33.000000 django_check_seo-1.0.1/django_check_seo/checks_list/check_keyword_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1928 2024-02-02 15:24:28.000000 django_check_seo-1.0.1/django_check_seo/checks_list/check_keywords.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4092 2022-06-14 09:17:55.000000 django_check_seo-1.0.1/django_check_seo/checks_list/check_links.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5711 2024-05-02 11:09:40.000000 django_check_seo-1.0.1/django_check_seo/checks_list/check_title.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3367 2022-06-14 09:17:55.000000 django_check_seo-1.0.1/django_check_seo/checks_list/check_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2018 2022-06-14 09:17:55.000000 django_check_seo-1.0.1/django_check_seo/checks_list/content_words_number.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2455 2024-05-02 11:09:43.000000 django_check_seo-1.0.1/django_check_seo/checks_list/keyword_present_first_paragraph.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2052 2022-09-21 15:03:12.000000 django_check_seo-1.0.1/django_check_seo/checks_list/launch_checks.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      668 2024-02-02 15:24:28.000000 django_check_seo-1.0.1/django_check_seo/cms_toolbars.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.104728 django_check_seo-1.0.1/django_check_seo/conf/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/conf/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      815 2022-06-14 08:53:12.000000 django_check_seo-1.0.1/django_check_seo/conf/settings.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.088727 django_check_seo-1.0.1/django_check_seo/locale/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.088727 django_check_seo-1.0.1/django_check_seo/locale/fr/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.104728 django_check_seo-1.0.1/django_check_seo/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    16533 2022-06-14 09:38:51.000000 django_check_seo-1.0.1/django_check_seo/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    24514 2022-06-14 09:38:24.000000 django_check_seo-1.0.1/django_check_seo/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.104728 django_check_seo-1.0.1/django_check_seo/migrations/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      976 2024-02-02 15:24:28.000000 django_check_seo-1.0.1/django_check_seo/migrations/0001_initial.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/migrations/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      532 2024-02-02 15:24:28.000000 django_check_seo-1.0.1/django_check_seo/models.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.088727 django_check_seo-1.0.1/django_check_seo/static/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.104728 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4734 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/design.css
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.112728 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    11358 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/LICENCE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      139 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/NOTICE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   164936 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   163448 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   162636 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   158604 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   122512 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    15388 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/logo-small.png
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   137074 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/django_check_seo/static/django-check-seo/logo.png
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.088727 django_check_seo-1.0.1/django_check_seo/templates/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.112728 django_check_seo-1.0.1/django_check_seo/templates/django_check_seo/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3439 2024-02-02 15:24:28.000000 django_check_seo-1.0.1/django_check_seo/templates/django_check_seo/default.html
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      705 2024-02-02 15:24:28.000000 django_check_seo-1.0.1/django_check_seo/templates/django_check_seo/element.html
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      603 2024-01-25 12:41:13.000000 django_check_seo-1.0.1/django_check_seo/urls.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3110 2024-02-02 15:24:28.000000 django_check_seo-1.0.1/django_check_seo/views.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.116728 django_check_seo-1.0.1/django_check_seo.egg-info/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     7416 2024-05-02 11:14:40.000000 django_check_seo-1.0.1/django_check_seo.egg-info/PKG-INFO
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2612 2024-05-02 11:14:40.000000 django_check_seo-1.0.1/django_check_seo.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2024-05-02 11:14:40.000000 django_check_seo-1.0.1/django_check_seo.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       59 2024-05-02 11:14:40.000000 django_check_seo-1.0.1/django_check_seo.egg-info/requires.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       17 2024-05-02 11:14:40.000000 django_check_seo-1.0.1/django_check_seo.egg-info/top_level.txt
+-rwxr-xr-x   0 kapt      (1000) kapt      (1000)     4701 2022-09-21 15:17:31.000000 django_check_seo-1.0.1/launch_tests.sh
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       94 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/pytest.ini
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1043 2024-05-02 11:14:40.116728 django_check_seo-1.0.1/setup.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       52 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/setup.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2024-05-02 11:14:40.116728 django_check_seo-1.0.1/tests/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    16223 2021-09-09 16:31:52.000000 django_check_seo-1.0.1/tests/test_content_words_number.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     9522 2021-09-09 16:31:52.000000 django_check_seo-1.0.1/tests/test_description.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6045 2021-09-09 16:31:52.000000 django_check_seo-1.0.1/tests/test_h1.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6469 2021-09-09 16:31:52.000000 django_check_seo-1.0.1/tests/test_h2.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4439 2021-09-09 16:31:52.000000 django_check_seo-1.0.1/tests/test_images.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5135 2021-09-09 16:31:52.000000 django_check_seo-1.0.1/tests/test_keyword_present_first_paragraph.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5989 2021-09-09 16:31:58.000000 django_check_seo-1.0.1/tests/test_keyword_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2476 2021-09-09 16:31:52.000000 django_check_seo-1.0.1/tests/test_keywords.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6480 2021-09-09 16:31:52.000000 django_check_seo-1.0.1/tests/test_links.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     7288 2021-09-09 16:31:52.000000 django_check_seo-1.0.1/tests/test_title.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3672 2021-09-09 16:31:52.000000 django_check_seo-1.0.1/tests/test_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      618 2021-09-08 08:29:05.000000 django_check_seo-1.0.1/tests_settings.py
```

### Comparing `django-check-seo-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `django_check_seo-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `django_check_seo-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/.pre-commit-config.yaml` & `django_check_seo-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/CHANGELOG.rst` & `django_check_seo-1.0.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 Changelog
 =========
 
 
+v1.0.1 (2024-05-02)
+-------------------
+
+Bug fixes
+~~~~~~~~~
+- Handle plural form in content [Corentin Bettiol]
+
+  When searching for a keyword in the document (meta description, h1, h2, early content), handle plural of keyword too.
+
+  For example, if the keyword is "destination", the checks will accept "destinations".
+  Work at least for fr/en/es/pt
+
+
+Documentation
+~~~~~~~~~~~~~
+- Update README [Corentin Bettiol]
+- Update changelog [Corentin Bettiol]
+
+
 v1.0.0 (2024-01-25)
 -------------------
 
 Features
 ~~~~~~~~
 - Add permission "use_django_check_seo" [Corentin Bettiol]
```

### Comparing `django-check-seo-1.0.0/CONTRIBUTING.md` & `django_check_seo-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/LICENSE` & `django_check_seo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/PKG-INFO` & `django_check_seo-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,22 @@
-Metadata-Version: 2.1
-Name: django-check-seo
-Version: 1.0.0
-Summary: Django Check SEO will check the SEO aspects of your site for you, and will provide advice in case of problems.
-Home-page: https://github.com/kapt-labs/django-check-seo
-Author: Dev Kapt
-Author-email: dev@kapt.mobi
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.8
-Classifier: Framework :: Django :: 2.2
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-Requires-Dist: djangocms-page-meta
-Requires-Dist: requests
-Requires-Dist: beautifulsoup4
-Requires-Dist: lxml
-Requires-Dist: unidecode
-
 ![Django Check SEO](https://user-images.githubusercontent.com/45763865/114545606-72178380-9c5c-11eb-99dd-1088bb2a0bd9.png)
 
 *Replacing some features of Yoast or SEMrush for Django & Django-CMS users.*
 
 In other words, django-check-seo will tell you if you have problems concerning a broad range of SEO aspects of your pages.
 
 ----
 
 [![PyPI](https://img.shields.io/pypi/v/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![GitHub last commit](https://img.shields.io/github/last-commit/kapt-labs/django-check-seo)](https://github.com/kapt-labs/django-check-seo)
 
 ----
 
 # Install
 
-*(compatible with django >= 1.8.15 & python >= 2.7)*
+*Only for django >= 2.2 & python >= 3.7, see [here](https://github.com/kapt-labs/django-check-seo/tree/python2) for a python2/django 1.8-1.11 version (tl;dr: install version <0.6).*
 
 1. Install the module from [PyPI](https://pypi.org/project/django-check-seo/):
     ```
     python3 -m pip install django-check-seo
     ```
 
 2. Add it in your `INSTALLED_APPS`:
@@ -55,19 +24,14 @@
         "django_check_seo",
     ```
 
 3. Add this in your `urls.py` *(if you're using django-cms, put it before the `cms.urls` line or it will not work)*:
     ```
         path("django-check-seo/", include("django_check_seo.urls")),
     ```
-    * *Or add this if you're still using `url` (you shouldn't):*
-        ```
-            url(r"^django-check-seo/", include("django_check_seo.urls")),
-        ```
-
 4. Update your Django [Site](https://i.imgur.com/pNRsKs7.png) object parameters with a working url (here's an [example](https://i.imgur.com/IedF3xE.png) for dev environment).
 
 5. Add `testserver` (and maybe `www.testserver`) to your `ALLOWED_HOSTS` list in your settings.py (django-check-seo uses the Test Framework in order to get content, instead of doing an HTTP request).
 
 6. ![**new in 1.0.0**](https://img.shields.io/badge/new_in-1.0.0-green) Add the permission (`use_django_check_seo`) to the users/groups you want to give access to.
 
 7. *(optional) Configure the settings (see [config](#config)).*
```

### Comparing `django-check-seo-1.0.0/README.md` & `django_check_seo-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,51 @@
+Metadata-Version: 2.1
+Name: django-check-seo
+Version: 1.0.1
+Summary: Django Check SEO will check the SEO aspects of your site for you, and will provide advice in case of problems.
+Home-page: https://github.com/kapt-labs/django-check-seo
+Author: Dev Kapt
+Author-email: dev@kapt.mobi
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: djangocms-page-meta
+Requires-Dist: requests
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
+Requires-Dist: unidecode
+
 ![Django Check SEO](https://user-images.githubusercontent.com/45763865/114545606-72178380-9c5c-11eb-99dd-1088bb2a0bd9.png)
 
 *Replacing some features of Yoast or SEMrush for Django & Django-CMS users.*
 
 In other words, django-check-seo will tell you if you have problems concerning a broad range of SEO aspects of your pages.
 
 ----
 
 [![PyPI](https://img.shields.io/pypi/v/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![GitHub last commit](https://img.shields.io/github/last-commit/kapt-labs/django-check-seo)](https://github.com/kapt-labs/django-check-seo)
 
 ----
 
 # Install
 
-*(compatible with django >= 1.8.15 & python >= 2.7)*
+*Only for django >= 2.2 & python >= 3.7, see [here](https://github.com/kapt-labs/django-check-seo/tree/python2) for a python2/django 1.8-1.11 version (tl;dr: install version <0.6).*
 
 1. Install the module from [PyPI](https://pypi.org/project/django-check-seo/):
     ```
     python3 -m pip install django-check-seo
     ```
 
 2. Add it in your `INSTALLED_APPS`:
@@ -24,19 +53,14 @@
         "django_check_seo",
     ```
 
 3. Add this in your `urls.py` *(if you're using django-cms, put it before the `cms.urls` line or it will not work)*:
     ```
         path("django-check-seo/", include("django_check_seo.urls")),
     ```
-    * *Or add this if you're still using `url` (you shouldn't):*
-        ```
-            url(r"^django-check-seo/", include("django_check_seo.urls")),
-        ```
-
 4. Update your Django [Site](https://i.imgur.com/pNRsKs7.png) object parameters with a working url (here's an [example](https://i.imgur.com/IedF3xE.png) for dev environment).
 
 5. Add `testserver` (and maybe `www.testserver`) to your `ALLOWED_HOSTS` list in your settings.py (django-check-seo uses the Test Framework in order to get content, instead of doing an HTTP request).
 
 6. ![**new in 1.0.0**](https://img.shields.io/badge/new_in-1.0.0-green) Add the permission (`use_django_check_seo`) to the users/groups you want to give access to.
 
 7. *(optional) Configure the settings (see [config](#config)).*
```

### Comparing `django-check-seo-1.0.0/django_check_seo/checks/site.py` & `django_check_seo-1.0.1/django_check_seo/checks/site.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/check_description.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/check_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,27 +119,25 @@
             length = len(tag.attrs["content"])
 
             # too short
             if (
                 length
                 < site.settings.DJANGO_CHECK_SEO_SETTINGS["meta_description_length"][0]
             ):
-
                 length_short.found = ngettext(
                     "%(words)d char", "%(words)d chars", length
                 ) % {"words": length}
                 length_short.searched_in = meta_description
                 site.problems.append(length_short)
 
             # too long
             elif (
                 length
                 > site.settings.DJANGO_CHECK_SEO_SETTINGS["meta_description_length"][1]
             ):
-
                 length_long.found = str(length)
                 length_long.searched_in = [
                     tag.attrs["content"][
                         : site.settings.DJANGO_CHECK_SEO_SETTINGS[
                             "meta_description_length"
                         ][1]
                     ]
@@ -151,15 +149,14 @@
                     ]
                     + "</b>"
                 ]
                 site.problems.append(length_long)
 
             # perfect
             else:
-
                 length_success.found = str(length)
                 length_success.searched_in = meta_description
                 site.success.append(length_success)
 
             occurrence = []
             keywords_good.found = ""
             for keyword in site.keywords:
@@ -167,15 +164,15 @@
 
                 # standardize apostrophes
                 keyword_lower = keyword_lower.replace("'", "’")
                 content_lower = tag.attrs["content"].lower().replace("'", "’")
 
                 nb_occurrences = len(
                     re.findall(
-                        r"(^| |\n|,|\.|!|\?)" + keyword_lower + r"($| |\n|,|\.|!|\?)",
+                        r"(^| |\n|,|\.|!|\?)" + keyword_lower + r"s?($| |\n|,|\.|!|\?)",
                         content_lower,
                     )
                 )
                 occurrence.append(nb_occurrences)
                 # edit current meta description
                 meta_description_kw[number_meta_description - 1] = meta_description_kw[
                     number_meta_description - 1
@@ -185,27 +182,25 @@
                 if nb_occurrences > 0:
                     if keywords_good.found != "":
                         keywords_good.found += ", "
                     keywords_good.found += keyword
 
             # if no keyword is found in description
             if not any(i > 0 for i in occurrence):
-
                 keywords_bad.found = 0
                 keywords_bad.searched_in = meta_description
                 site.warnings.append(keywords_bad)
 
             # perfect
             else:
                 keywords_good.searched_in = meta_description_kw
                 site.success.append(keywords_good)
 
     # too many meta description
     if number_meta_description > 1:
-
         too_much_meta.found = number_meta_description
         too_much_meta.searched_in = meta_description
         site.warnings.append(too_much_meta)
     # perfect
     elif number_meta_description == 1:
         meta_description_only_one.searched_in = meta_description
         site.success.append(meta_description_only_one)
```

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/check_h1.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/check_h1.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             # standardize apostrophes
             keyword = keyword.replace("'", "’")
             h1_text = h1_text.replace("'", "’")
 
             # ugly regex ? see example at https://github.com/kapt-labs/django-check-seo/issues/38#issuecomment-603108275
             nb_occurrences = len(
                 re.findall(
-                    r"(^| |\n|,|\.|!|\?)" + keyword + r"($| |\n|,|\.|!|\?)",
+                    r"(^| |\n|,|\.|!|\?)" + keyword + r"s?($| |\n|,|\.|!|\?)",
                     h1_text,
                 )
             )
             occurrence.append(nb_occurrences)
 
             if nb_occurrences > 0:
                 h1_text = h1_text.replace(
```

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/check_h2.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/check_h2.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                 keyword_lower = keyword_lower.replace("'", "’")
                 single_h2 = single_h2.replace("'", "’")
 
                 nb_occurrences = len(
                     re.findall(
                         r"(^| |\n|,|\.|!|\?)"
                         + keyword_lower.lower()
-                        + r"($| |\n|,|\.|!|\?)",
+                        + r"s?($| |\n|,|\.|!|\?)",
                         single_h2,
                     )
                 )
                 occurrence.append(nb_occurrences)
 
                 # add kw in found
                 if nb_occurrences > 0:
```

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/check_images.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/check_images.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/check_keyword_url.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/check_keyword_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,25 +77,25 @@
         # remove apostrophes as they are generally removed from URLs
         keyword = keyword.replace("'", "").replace("’", "")
 
         keyword_unnaccented = unidecode.unidecode(keyword)  # pragma: no cover
 
         nb_occurrences = len(
             re.findall(
-                r"(^| |\n|,|\.|!|\?|/|-)" + keyword + r"($| |\n|,|\.|!|\?|/|-)",
+                r"(^| |\n|,|\.|!|\?|/|-)" + keyword + r"s?($| |\n|,|\.|!|\?|/|-)",
                 full_url,
             )
         )
         if nb_occurrences == 0:
             # retry with unnaccented kw
             accented_occurrences = len(
                 re.findall(
                     r"(^| |\n|,|\.|!|\?|/|-)"
                     + keyword_unnaccented
-                    + r"($| |\n|,|\.|!|\?|/|-)",
+                    + r"s?($| |\n|,|\.|!|\?|/|-)",
                     full_url,
                 )
             )
         occurrence.append(nb_occurrences + accented_occurrences)
 
         if nb_occurrences > 0:
             full_url = full_url.replace(keyword, '<b class="good">' + keyword + "</b>")
```

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/check_keywords.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/check_keywords.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/check_links.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/check_links.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/check_title.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/check_title.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     title_text = titles[0].text.lower()
     title_text_kw = []
 
     for kw in site.keywords:
         kw = kw.lower()
         nb_occurrences = len(
             re.findall(
-                r"(^| |\n|,|\.|!|\?)" + kw + r"($| |\n|,|\.|!|\?)",
+                r"(^| |\n|,|\.|!|\?)" + kw + r"s?($| |\n|,|\.|!|\?)",
                 title_text,
             )
         )
         occurrence.append(nb_occurrences)
 
         if nb_occurrences > 0:
             title_text = title_text.replace(
```

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/check_url.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/check_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/content_words_number.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/content_words_number.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/keyword_present_first_paragraph.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/keyword_present_first_paragraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     occurrence = []
     first_words_kw = []
 
     for keyword in site.keywords:
         keyword = keyword.lower()
         nb_occurrences = len(
             re.findall(
-                r"(^| |\n|,|\.|!|\?)" + keyword + r"($| |\n|,|\.|!|\?)",
+                r"(^| |\n|,|\.|!|\?)" + keyword + r"s?($| |\n|,|\.|!|\?)",
                 first_words,
             )
         )
         occurrence.append(nb_occurrences)
 
         if nb_occurrences > 0:
             first_words_text = first_words_text.replace(
```

### Comparing `django-check-seo-1.0.0/django_check_seo/checks_list/launch_checks.py` & `django_check_seo-1.0.1/django_check_seo/checks_list/launch_checks.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/cms_toolbars.py` & `django_check_seo-1.0.1/django_check_seo/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/conf/settings.py` & `django_check_seo-1.0.1/django_check_seo/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/locale/fr/LC_MESSAGES/django.mo` & `django_check_seo-1.0.1/django_check_seo/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/locale/fr/LC_MESSAGES/django.po` & `django_check_seo-1.0.1/django_check_seo/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/migrations/0001_initial.py` & `django_check_seo-1.0.1/django_check_seo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/models.py` & `django_check_seo-1.0.1/django_check_seo/models.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/static/django-check-seo/design.css` & `django_check_seo-1.0.1/django_check_seo/static/django-check-seo/design.css`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/LICENCE` & `django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/LICENCE`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf` & `django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf` & `django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf` & `django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf` & `django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf` & `django_check_seo-1.0.1/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/static/django-check-seo/logo-small.png` & `django_check_seo-1.0.1/django_check_seo/static/django-check-seo/logo-small.png`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/static/django-check-seo/logo.png` & `django_check_seo-1.0.1/django_check_seo/static/django-check-seo/logo.png`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/templates/django_check_seo/default.html` & `django_check_seo-1.0.1/django_check_seo/templates/django_check_seo/default.html`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/templates/django_check_seo/element.html` & `django_check_seo-1.0.1/django_check_seo/templates/django_check_seo/element.html`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/urls.py` & `django_check_seo-1.0.1/django_check_seo/urls.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo/views.py` & `django_check_seo-1.0.1/django_check_seo/views.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/django_check_seo.egg-info/PKG-INFO` & `django_check_seo-1.0.1/django_check_seo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: django-check-seo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django Check SEO will check the SEO aspects of your site for you, and will provide advice in case of problems.
 Home-page: https://github.com/kapt-labs/django-check-seo
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.8
-Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +37,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![GitHub last commit](https://img.shields.io/github/last-commit/kapt-labs/django-check-seo)](https://github.com/kapt-labs/django-check-seo)
 
 ----
 
 # Install
 
-*(compatible with django >= 1.8.15 & python >= 2.7)*
+*Only for django >= 2.2 & python >= 3.7, see [here](https://github.com/kapt-labs/django-check-seo/tree/python2) for a python2/django 1.8-1.11 version (tl;dr: install version <0.6).*
 
 1. Install the module from [PyPI](https://pypi.org/project/django-check-seo/):
     ```
     python3 -m pip install django-check-seo
     ```
 
 2. Add it in your `INSTALLED_APPS`:
@@ -55,19 +53,14 @@
         "django_check_seo",
     ```
 
 3. Add this in your `urls.py` *(if you're using django-cms, put it before the `cms.urls` line or it will not work)*:
     ```
         path("django-check-seo/", include("django_check_seo.urls")),
     ```
-    * *Or add this if you're still using `url` (you shouldn't):*
-        ```
-            url(r"^django-check-seo/", include("django_check_seo.urls")),
-        ```
-
 4. Update your Django [Site](https://i.imgur.com/pNRsKs7.png) object parameters with a working url (here's an [example](https://i.imgur.com/IedF3xE.png) for dev environment).
 
 5. Add `testserver` (and maybe `www.testserver`) to your `ALLOWED_HOSTS` list in your settings.py (django-check-seo uses the Test Framework in order to get content, instead of doing an HTTP request).
 
 6. ![**new in 1.0.0**](https://img.shields.io/badge/new_in-1.0.0-green) Add the permission (`use_django_check_seo`) to the users/groups you want to give access to.
 
 7. *(optional) Configure the settings (see [config](#config)).*
```

### Comparing `django-check-seo-1.0.0/django_check_seo.egg-info/SOURCES.txt` & `django_check_seo-1.0.1/django_check_seo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .bumpversion.cfg
 .coveragerc
 .flake8
+.gitchangelog.rc
 .gitignore
 .isort.cfg
 .pre-commit-config.yaml
 AUTHORS.md
 CHANGELOG.rst
 CONTRIBUTING.md
 LICENSE
```

### Comparing `django-check-seo-1.0.0/launch_tests.sh` & `django_check_seo-1.0.1/launch_tests.sh`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/setup.cfg` & `django_check_seo-1.0.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [metadata]
 name = django-check-seo
-version = 1.0.0
+version = 1.0.1
 description = Django Check SEO will check the SEO aspects of your site for you, and will provide advice in case of problems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kapt-labs/django-check-seo
 author = Dev Kapt
 author_email = dev@kapt.mobi
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 1.8
-	Framework :: Django :: 2.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python
 	Programming Language :: Python :: 2
 	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3
```

### Comparing `django-check-seo-1.0.0/tests/test_content_words_number.py` & `django_check_seo-1.0.1/tests/test_content_words_number.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests/test_description.py` & `django_check_seo-1.0.1/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests/test_h1.py` & `django_check_seo-1.0.1/tests/test_h1.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests/test_h2.py` & `django_check_seo-1.0.1/tests/test_h2.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests/test_images.py` & `django_check_seo-1.0.1/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests/test_keyword_present_first_paragraph.py` & `django_check_seo-1.0.1/tests/test_keyword_present_first_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests/test_keyword_url.py` & `django_check_seo-1.0.1/tests/test_keyword_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests/test_keywords.py` & `django_check_seo-1.0.1/tests/test_keywords.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests/test_links.py` & `django_check_seo-1.0.1/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests/test_title.py` & `django_check_seo-1.0.1/tests/test_title.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests/test_url.py` & `django_check_seo-1.0.1/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-1.0.0/tests_settings.py` & `django_check_seo-1.0.1/tests_settings.py`

 * *Files identical despite different names*

