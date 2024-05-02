# Comparing `tmp/dj-whisperer-0.3.0.tar.gz` & `tmp/dj-whisperer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-whisperer-0.3.0.tar", last modified: Tue Mar 26 08:19:56 2024, max compression
+gzip compressed data, was "dist/dj-whisperer-0.3.1.tar", last modified: Thu May  2 14:46:11 2024, max compression
```

## Comparing `dj-whisperer-0.3.0.tar` & `dj-whisperer-0.3.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1050 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     1446 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4636 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3334 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2735 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/dj_whisperer.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4636 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/dj_whisperer.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1574 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/dj_whisperer.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/dj_whisperer.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/dj_whisperer.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       10 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/dj_whisperer.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4589 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/docs/advanced.rst
--rw-rw-rw-   0 root         (0) root         (0)     2077 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      806 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/docs/introduction.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     2658 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      322 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      461 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/runtests.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2103 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/tox.ini
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/whisperer/
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/client.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/codes.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1887 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/countdown.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/events.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/whisperer/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2750 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/migrations/0002_webhook_additional_headers.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/migrations/0003_auto_20200505_0853.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/migrations/0004_webhook_retry_count.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/migrations/0005_webhook_config.py
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/migrations/0006_auto_20200925_1710.py
--rw-rw-rw-   0 root         (0) root         (0)     2658 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/migrations/0007_event_queue.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/migrations/0008_ayto_20240323_2301.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3775 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/models.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/whisperer/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/resources/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/resources/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/resources/views.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/services.py
--rw-rw-rw-   0 root         (0) root         (0)    10262 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tasks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 08:19:56.000000 dj-whisperer-0.3.0/whisperer/tests/
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tests/celery.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tests/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tests/test_serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tests/test_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2571 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3718 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)    31247 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tests/tests.py
--rw-rw-rw-   0 root         (0) root         (0)     2112 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/tests/webhooks.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2654 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2024-03-26 08:19:35.000000 dj-whisperer-0.3.0/whisperer/validators.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1502 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4792 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2791 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/dj_whisperer.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4792 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/dj_whisperer.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/dj_whisperer.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/dj_whisperer.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/dj_whisperer.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       10 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/dj_whisperer.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4589 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/docs/advanced.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      806 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/docs/introduction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     2658 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/runtests.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/whisperer/
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1887 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/countdown.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/whisperer/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/migrations/0002_webhook_additional_headers.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/migrations/0003_auto_20200505_0853.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/migrations/0004_webhook_retry_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/migrations/0005_webhook_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/migrations/0006_auto_20200925_1710.py
+-rw-rw-rw-   0 root         (0) root         (0)     2658 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/migrations/0007_event_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/migrations/0008_ayto_20240323_2301.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3775 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/models.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/whisperer/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/resources/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/resources/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/resources/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/services.py
+-rw-rw-rw-   0 root         (0) root         (0)    10262 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tasks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-02 14:46:11.000000 dj-whisperer-0.3.1/whisperer/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tests/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tests/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tests/test_serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      750 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tests/test_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2571 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tests/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)    31273 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tests/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     2112 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/tests/webhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2024-05-02 14:45:52.000000 dj-whisperer-0.3.1/whisperer/validators.py
```

### Comparing `dj-whisperer-0.3.0/.gitignore` & `dj-whisperer-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/LICENSE.txt` & `dj-whisperer-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/Makefile` & `dj-whisperer-0.3.1/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Generate all combinations of Python and Django versions
 COMBINATIONS := py27-django110 py27-django111 \
                 py34-django110 py34-django111 py34-django20 \
                 py35-django110 py35-django111 py35-django20 py35-django21 py35-django22 \
                 py36-django111 py36-django20 py36-django21 py36-django22 py36-django30 py36-django31 \
                 py37-django111 py37-django20 py37-django21 py37-django22 py37-django30 py37-django31 \
-                py38-django22 py38-django30 py38-django31
+                py38-django22 py38-django30 py38-django31 py38-django32 py38-django40 py38-django41 py38-django42
 
 # ANSI color codes
 YELLOW := \033[33m
 WHITE := \033[97m
 RESET := \033[0m
 
 # Define commands
```

### Comparing `dj-whisperer-0.3.0/PKG-INFO` & `dj-whisperer-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-whisperer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-whisperer
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -26,14 +26,18 @@
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Django Whisperer
 
 [![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/dj-whisperer)](https://bitbucket.org/akinonteam/dj-whisperer/addon/pipelines/home)
 [![Documentation status](https://readthedocs.org/projects/dj-whisperer/badge/?version=latest)](https://dj-whisperer.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `dj-whisperer-0.3.0/README.md` & `dj-whisperer-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/bitbucket-pipelines.yml` & `dj-whisperer-0.3.1/bitbucket-pipelines.yml`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             - redis
       - step:
           name: py38
           image: python:3.8-alpine
           script:
             - apk add postgresql-dev gcc git python3-dev musl-dev
             - pip install tox
-            - tox -e py38-django22,py38-django30,py38-django31
+            - tox -e py38-django22,py38-django30,py38-django31,py38-django32,py38-django40,py38-django41,py38-django42
           services:
             - postgres
             - redis
   tags:
     '*':
       - step:
           name: Publish to PyPI
```

### Comparing `dj-whisperer-0.3.0/dj_whisperer.egg-info/PKG-INFO` & `dj-whisperer-0.3.1/dj_whisperer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-whisperer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-whisperer
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -26,14 +26,18 @@
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Django Whisperer
 
 [![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/dj-whisperer)](https://bitbucket.org/akinonteam/dj-whisperer/addon/pipelines/home)
 [![Documentation status](https://readthedocs.org/projects/dj-whisperer/badge/?version=latest)](https://dj-whisperer.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `dj-whisperer-0.3.0/dj_whisperer.egg-info/SOURCES.txt` & `dj-whisperer-0.3.1/dj_whisperer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/docs/Makefile` & `dj-whisperer-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/docs/advanced.rst` & `dj-whisperer-0.3.1/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/docs/conf.py` & `dj-whisperer-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/docs/index.rst` & `dj-whisperer-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/docs/introduction.rst` & `dj-whisperer-0.3.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/docs/make.bat` & `dj-whisperer-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/docs/quickstart.rst` & `dj-whisperer-0.3.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/setup.py` & `dj-whisperer-0.3.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -61,9 +61,13 @@
         "Framework :: Django :: 1.10",
         "Framework :: Django :: 1.11",
         "Framework :: Django :: 2.0",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
+        "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
     ],
 )
```

### Comparing `dj-whisperer-0.3.0/tox.ini` & `dj-whisperer-0.3.1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -6,46 +6,51 @@
 [tox]
 isolated_build = True
 skip_missing_interpreters = True
 envlist = py27-{django110,django111}
           py34-{django110,django111,django20}
           py35-{django110,django111,django20,django21,django22}
           {py36,py37}-{django111,django20,django21,django22,django30,django31}
-          py38-{django22,django30,django31}
+          py38-{django22,django30,django31,django32,django40,django41,django42}
           linting
 
 [testenv]
 deps = django110: Django>=1.10,<1.11
        django110: celery==4.1.0
        django111: Django>=1.11.7,<2.0
        django{110,111}: django-filter==1.1.0
        django{110,111}: djangorestframework-filters==0.11.1
        django20: Django>=2.0,<2.1
        django21: Django>=2.1,<2.2
        django22: Django>=2.2.8,<3.0
        django{20,21,22}: django-filter==2.1.0
        django30: Django>=3.0,<3.1
        django31: Django>=3.1,<3.2
-       django{30,31}: django-filter==2.4.0
-       django{111,20,21,22,30,31}: celery
-       djangorestframework<3.12
+       django32: Django>=3.2,<4.0
+       django40: Django>=4.0,<4.1
+       django41: Django>=4.1,<4.2
+       django42: Django>=4.2,<5.0
+       django{30,31,32}: django-filter==2.4.0
+       django{40,41,42}: django-filter==21.1
+       django{111,20,21,22,30,31,32,40,41,42}: celery
+       djangorestframework<3.15
        django-redis>=4.6.0
        psycopg2-binary
        requests
        mock
        model-mommy==1.6.0
        requests_mock==1.6.0
        importlib-metadata>=1.4.0,<5.0; python_version == '3.7'
 commands = python runtests.py
 
 [testenv:linting]
 deps = black==21.5b1
        isort==5.0.4
-       Django>=2.2.8,<3.2
-       djangorestframework<3.12
+       Django>=2.2.8,<5.0
+       djangorestframework<3.15
        djangorestframework-filters<0.12
        requests
        celery
        mock
        model-mommy==1.6.0
        requests_mock==1.6.0
        click==7.1.2
```

### Comparing `dj-whisperer-0.3.0/whisperer/client.py` & `dj-whisperer-0.3.1/whisperer/client.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/codes.py` & `dj-whisperer-0.3.1/whisperer/codes.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/countdown.py` & `dj-whisperer-0.3.1/whisperer/countdown.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/events.py` & `dj-whisperer-0.3.1/whisperer/events.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/exceptions.py` & `dj-whisperer-0.3.1/whisperer/exceptions.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/migrations/0001_initial.py` & `dj-whisperer-0.3.1/whisperer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/migrations/0003_auto_20200505_0853.py` & `dj-whisperer-0.3.1/whisperer/migrations/0003_auto_20200505_0853.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/migrations/0004_webhook_retry_count.py` & `dj-whisperer-0.3.1/whisperer/migrations/0004_webhook_retry_count.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/migrations/0005_webhook_config.py` & `dj-whisperer-0.3.1/whisperer/migrations/0005_webhook_config.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/migrations/0006_auto_20200925_1710.py` & `dj-whisperer-0.3.1/whisperer/migrations/0006_auto_20200925_1710.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/migrations/0007_event_queue.py` & `dj-whisperer-0.3.1/whisperer/migrations/0007_event_queue.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/migrations/0008_ayto_20240323_2301.py` & `dj-whisperer-0.3.1/whisperer/migrations/0008_ayto_20240323_2301.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/models.py` & `dj-whisperer-0.3.1/whisperer/models.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/resources/filters.py` & `dj-whisperer-0.3.1/whisperer/resources/filters.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/resources/serializers.py` & `dj-whisperer-0.3.1/whisperer/resources/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/resources/views.py` & `dj-whisperer-0.3.1/whisperer/resources/views.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/services.py` & `dj-whisperer-0.3.1/whisperer/services.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/tasks.py` & `dj-whisperer-0.3.1/whisperer/tasks.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/tests/models.py` & `dj-whisperer-0.3.1/whisperer/tests/models.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/tests/test_serializers.py` & `dj-whisperer-0.3.1/whisperer/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/tests/test_settings.py` & `dj-whisperer-0.3.1/whisperer/tests/test_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'whisperer.tests',
     'whisperer',
 ]
 
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
+
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.postgresql',
         'NAME': 'postgres',
         'USER': 'postgres',
         'PASSWORD': 'postgres',
         'HOST': 'localhost',
```

### Comparing `dj-whisperer-0.3.0/whisperer/tests/test_utils.py` & `dj-whisperer-0.3.1/whisperer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/tests/test_views.py` & `dj-whisperer-0.3.1/whisperer/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/tests/tests.py` & `dj-whisperer-0.3.1/whisperer/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,15 @@
             modified_date=timezone.now(),
             created_date=timezone.now(),
             request_payload={},
             retry_count=TASK_RETRY_COUNT,
             delivered=False,
             webhook=self.webhook,
         )
+        self.order.save()
         with requests_mock.Mocker() as mock:
             mock.register_uri(
                 "POST", self.webhook.target_url, text="Order Created", status_code=200
             )
             deliver_event(
                 self.order, "order-created", async_=False, event_uuid=webhookevent.uuid
             )
```

### Comparing `dj-whisperer-0.3.0/whisperer/tests/webhooks.py` & `dj-whisperer-0.3.1/whisperer/tests/webhooks.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/urls.py` & `dj-whisperer-0.3.1/whisperer/urls.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/utils.py` & `dj-whisperer-0.3.1/whisperer/utils.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.3.0/whisperer/validators.py` & `dj-whisperer-0.3.1/whisperer/validators.py`

 * *Files identical despite different names*

