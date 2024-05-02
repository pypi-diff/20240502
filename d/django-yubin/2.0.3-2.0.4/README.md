# Comparing `tmp/django-yubin-2.0.3.tar.gz` & `tmp/django_yubin-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-yubin-2.0.3.tar", last modified: Tue Jan  9 16:04:12 2024, max compression
+gzip compressed data, was "django_yubin-2.0.4.tar", last modified: Thu May  2 16:32:42 2024, max compression
```

## Comparing `django-yubin-2.0.3.tar` & `django_yubin-2.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.961586 django-yubin-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-01-09 16:04:05.000000 django-yubin-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-09 16:04:05.000000 django-yubin-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-01-09 16:04:12.961586 django-yubin-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-01-09 16:04:05.000000 django-yubin-2.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.957586 django-yubin-2.0.3/django_yubin/
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/mailparser_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.957586 django-yubin-2.0.3/django_yubin/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.957586 django-yubin-2.0.3/django_yubin/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/management/commands/create_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/management/commands/db2file.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/management/commands/file2db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/management/commands/sample.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/management/commands/send_test_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)    18647 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/message_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.961586 django-yubin-2.0.3/django_yubin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0002_auto_20170405_1635.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0003_auto_20171201_1506.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0004_message_date_sent.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0005_auto_20181128_0407.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0006_auto_20200319_1120.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0007_auto_20200319_1158.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0008_auto_20200320_0407.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0009_auto_20221122_1605.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0010_message_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/0011_message_bcc_address_message_cc_address_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11308 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/storage_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.953586 django-yubin-2.0.3/django_yubin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.953586 django-yubin-2.0.3/django_yubin/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.953586 django-yubin-2.0.3/django_yubin/templates/admin/django_yubin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.961586 django-yubin-2.0.3/django_yubin/templates/admin/django_yubin/message/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/templates/admin/django_yubin/message/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.961586 django-yubin-2.0.3/django_yubin/templates/django_yubin/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/templates/django_yubin/html_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/templates/django_yubin/message_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-01-09 16:04:05.000000 django-yubin-2.0.3/django_yubin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.961586 django-yubin-2.0.3/django_yubin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-01-09 16:04:12.000000 django-yubin-2.0.3/django_yubin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-01-09 16:04:12.000000 django-yubin-2.0.3/django_yubin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 16:04:12.000000 django-yubin-2.0.3/django_yubin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-09 16:04:12.000000 django-yubin-2.0.3/django_yubin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-09 16:04:12.000000 django-yubin-2.0.3/django_yubin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:04:12.961586 django-yubin-2.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-01-09 16:04:05.000000 django-yubin-2.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-01-09 16:04:05.000000 django-yubin-2.0.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-01-09 16:04:05.000000 django-yubin-2.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-01-09 16:04:05.000000 django-yubin-2.0.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-01-09 16:04:05.000000 django-yubin-2.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-01-09 16:04:05.000000 django-yubin-2.0.3/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-01-09 16:04:05.000000 django-yubin-2.0.3/docs/mailviews.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-01-09 16:04:05.000000 django-yubin-2.0.3/docs/queue.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-01-09 16:04:05.000000 django-yubin-2.0.3/docs/settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-01-09 16:04:05.000000 django-yubin-2.0.3/docs/storages.rst
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-09 16:04:12.965586 django-yubin-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-01-09 16:04:05.000000 django-yubin-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.762867 django_yubin-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-05-02 16:32:39.000000 django_yubin-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-02 16:32:39.000000 django_yubin-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-02 16:32:42.762867 django_yubin-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-02 16:32:39.000000 django_yubin-2.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.758866 django_yubin-2.0.4/django_yubin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/mailparser_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.758866 django_yubin-2.0.4/django_yubin/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.758866 django_yubin-2.0.4/django_yubin/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/management/commands/create_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/management/commands/db2file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/management/commands/file2db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/management/commands/sample.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/management/commands/send_test_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18647 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/message_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.762867 django_yubin-2.0.4/django_yubin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0002_auto_20170405_1635.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0003_auto_20171201_1506.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0004_message_date_sent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0005_auto_20181128_0407.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0006_auto_20200319_1120.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0007_auto_20200319_1158.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0008_auto_20200320_0407.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0009_auto_20221122_1605.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0010_message_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/0011_message_bcc_address_message_cc_address_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11308 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/storage_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.754866 django_yubin-2.0.4/django_yubin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.754866 django_yubin-2.0.4/django_yubin/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.754866 django_yubin-2.0.4/django_yubin/templates/admin/django_yubin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.762867 django_yubin-2.0.4/django_yubin/templates/admin/django_yubin/message/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/templates/admin/django_yubin/message/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.762867 django_yubin-2.0.4/django_yubin/templates/django_yubin/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/templates/django_yubin/html_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/templates/django_yubin/message_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-02 16:32:39.000000 django_yubin-2.0.4/django_yubin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.762867 django_yubin-2.0.4/django_yubin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-02 16:32:42.000000 django_yubin-2.0.4/django_yubin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-02 16:32:42.000000 django_yubin-2.0.4/django_yubin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:32:42.000000 django_yubin-2.0.4/django_yubin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 16:32:42.000000 django_yubin-2.0.4/django_yubin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 16:32:42.000000 django_yubin-2.0.4/django_yubin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:32:42.762867 django_yubin-2.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-02 16:32:39.000000 django_yubin-2.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-02 16:32:39.000000 django_yubin-2.0.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-02 16:32:39.000000 django_yubin-2.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-02 16:32:39.000000 django_yubin-2.0.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-02 16:32:39.000000 django_yubin-2.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-02 16:32:39.000000 django_yubin-2.0.4/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-02 16:32:39.000000 django_yubin-2.0.4/docs/mailviews.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-02 16:32:39.000000 django_yubin-2.0.4/docs/queue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-02 16:32:39.000000 django_yubin-2.0.4/docs/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-02 16:32:39.000000 django_yubin-2.0.4/docs/storages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 16:32:42.762867 django_yubin-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-02 16:32:39.000000 django_yubin-2.0.4/setup.py
```

### Comparing `django-yubin-2.0.3/LICENSE` & `django_yubin-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/PKG-INFO` & `django_yubin-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-yubin
-Version: 2.0.3
+Version: 2.0.4
 Summary: A reusable Django app for composing and queueing emails django-mailviews + Celery + others
 Home-page: http://github.com/APSL/django-yubin
 Author: Antoni Aloy
 Author-email: aaloy@apsl.net
 Maintainer: APSL
 Maintainer-email: info@apsl.net
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
-Requires-Dist: celery<5.3,>=5.0
+Requires-Dist: celery<6,>=5.0
 Requires-Dist: mail-parser
 Requires-Dist: pytz
 
 django-yubin
 ============
 
 .. image:: https://github.com/APSL/django-yubin/actions/workflows/ci-cd.yml/badge.svg
```

### Comparing `django-yubin-2.0.3/README.rst` & `django_yubin-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/__init__.py` & `django_yubin-2.0.4/django_yubin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/admin.py` & `django_yubin-2.0.4/django_yubin/admin.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/backends.py` & `django_yubin-2.0.4/django_yubin/backends.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/constants.py` & `django_yubin-2.0.4/django_yubin/constants.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/engine.py` & `django_yubin-2.0.4/django_yubin/engine.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/mailparser_utils.py` & `django_yubin-2.0.4/django_yubin/mailparser_utils.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/management/commands/create_mail.py` & `django_yubin-2.0.4/django_yubin/management/commands/create_mail.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/management/commands/file2db.py` & `django_yubin-2.0.4/django_yubin/management/commands/file2db.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/management/commands/sample.pdf` & `django_yubin-2.0.4/django_yubin/management/commands/sample.pdf`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/management/commands/send_test_mail.py` & `django_yubin-2.0.4/django_yubin/management/commands/send_test_mail.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/message_views.py` & `django_yubin-2.0.4/django_yubin/message_views.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/migrations/0001_initial.py` & `django_yubin-2.0.4/django_yubin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/migrations/0002_auto_20170405_1635.py` & `django_yubin-2.0.4/django_yubin/migrations/0002_auto_20170405_1635.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/migrations/0003_auto_20171201_1506.py` & `django_yubin-2.0.4/django_yubin/migrations/0003_auto_20171201_1506.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/migrations/0006_auto_20200319_1120.py` & `django_yubin-2.0.4/django_yubin/migrations/0006_auto_20200319_1120.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/migrations/0007_auto_20200319_1158.py` & `django_yubin-2.0.4/django_yubin/migrations/0007_auto_20200319_1158.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/migrations/0009_auto_20221122_1605.py` & `django_yubin-2.0.4/django_yubin/migrations/0009_auto_20221122_1605.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/migrations/0011_message_bcc_address_message_cc_address_and_more.py` & `django_yubin-2.0.4/django_yubin/migrations/0011_message_bcc_address_message_cc_address_and_more.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/models.py` & `django_yubin-2.0.4/django_yubin/models.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/settings.py` & `django_yubin-2.0.4/django_yubin/settings.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/signals.py` & `django_yubin-2.0.4/django_yubin/signals.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/storage_backends.py` & `django_yubin-2.0.4/django_yubin/storage_backends.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/tasks.py` & `django_yubin-2.0.4/django_yubin/tasks.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/templates/django_yubin/message_detail.html` & `django_yubin-2.0.4/django_yubin/templates/django_yubin/message_detail.html`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin/views.py` & `django_yubin-2.0.4/django_yubin/views.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/django_yubin.egg-info/PKG-INFO` & `django_yubin-2.0.4/django_yubin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-yubin
-Version: 2.0.3
+Version: 2.0.4
 Summary: A reusable Django app for composing and queueing emails django-mailviews + Celery + others
 Home-page: http://github.com/APSL/django-yubin
 Author: Antoni Aloy
 Author-email: aaloy@apsl.net
 Maintainer: APSL
 Maintainer-email: info@apsl.net
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
-Requires-Dist: celery<5.3,>=5.0
+Requires-Dist: celery<6,>=5.0
 Requires-Dist: mail-parser
 Requires-Dist: pytz
 
 django-yubin
 ============
 
 .. image:: https://github.com/APSL/django-yubin/actions/workflows/ci-cd.yml/badge.svg
```

### Comparing `django-yubin-2.0.3/django_yubin.egg-info/SOURCES.txt` & `django_yubin-2.0.4/django_yubin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/docs/Makefile` & `django_yubin-2.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/docs/changelog.rst` & `django_yubin-2.0.4/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 Changelog
 =========
 
 This project adheres to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
 Starting from version 2.0.0, the format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_.
 
+[2.0.4] - 2024-05-02
+--------------------
+
+Changed
+^^^^^^^
+* <6 upper bound to celery dependency.
+
 [2.0.3] - 2024-01-09
 --------------------
 
 Fixed
 ^^^^^
 * Fix race condition between Celery and database transactions (https://github.com/APSL/django-yubin/pull/74)
```

### Comparing `django-yubin-2.0.3/docs/conf.py` & `django_yubin-2.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/docs/contributing.rst` & `django_yubin-2.0.4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/docs/index.rst` & `django_yubin-2.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/docs/install.rst` & `django_yubin-2.0.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/docs/mailviews.rst` & `django_yubin-2.0.4/docs/mailviews.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/docs/queue.rst` & `django_yubin-2.0.4/docs/queue.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/docs/settings.rst` & `django_yubin-2.0.4/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/docs/storages.rst` & `django_yubin-2.0.4/docs/storages.rst`

 * *Files identical despite different names*

### Comparing `django-yubin-2.0.3/setup.py` & `django_yubin-2.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from setuptools import setup
 
 
 INSTALL_REQUIRES = [
-    'celery>=5.0,<5.3',
+    'celery>=5.0,<6',
     'mail-parser',
     'pytz',
 ]
 
 
 with open('README.rst') as docs_index:
     long_description = docs_index.read()
```

