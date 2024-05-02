# Comparing `tmp/django-comments-xtd-2.9.8.tar.gz` & `tmp/django-comments-xtd-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-comments-xtd-2.9.8.tar", last modified: Sun Sep 18 10:33:09 2022, max compression
+gzip compressed data, was "django-comments-xtd-2.9.9.tar", last modified: Wed Oct 26 12:44:57 2022, max compression
```

## Comparing `django-comments-xtd-2.9.8.tar` & `django-comments-xtd-2.9.9.tar`

### file list

```diff
@@ -1,422 +1,422 @@
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.117008 django-comments-xtd-2.9.8/
--rw-r--r--   0 danirus    (501) staff       (20)     3989 2020-05-12 19:59:09.000000 django-comments-xtd-2.9.8/.coverage
--rw-r--r--   0 danirus    (501) staff       (20)      290 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/.gitignore
--rw-r--r--   0 danirus    (501) staff       (20)      956 2022-09-18 10:25:38.000000 django-comments-xtd-2.9.8/AUTHORS
--rw-r--r--   0 danirus    (501) staff       (20)    18137 2022-09-18 10:25:38.000000 django-comments-xtd-2.9.8/CHANGELOG.md
--rw-r--r--   0 danirus    (501) staff       (20)     1303 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/LICENSE
--rw-r--r--   0 danirus    (501) staff       (20)      341 2017-07-31 17:55:32.000000 django-comments-xtd-2.9.8/MANIFEST.in
--rw-r--r--   0 danirus    (501) staff       (20)     1112 2022-09-18 10:33:09.116871 django-comments-xtd-2.9.8/PKG-INFO
--rw-r--r--   0 danirus    (501) staff       (20)     1789 2022-09-17 05:14:09.000000 django-comments-xtd-2.9.8/README.rst
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.994413 django-comments-xtd-2.9.8/django_comments_xtd/
--rw-r--r--   0 danirus    (501) staff       (20)      771 2022-09-18 10:25:40.000000 django-comments-xtd-2.9.8/django_comments_xtd/__init__.py
--rw-r--r--   0 danirus    (501) staff       (20)     1729 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/admin.py
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.996371 django-comments-xtd-2.9.8/django_comments_xtd/api/
--rw-r--r--   0 danirus    (501) staff       (20)      285 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/api/__init__.py
--rw-r--r--   0 danirus    (501) staff       (20)     7489 2022-09-17 05:14:38.000000 django-comments-xtd-2.9.8/django_comments_xtd/api/frontend.py
--rw-r--r--   0 danirus    (501) staff       (20)    12552 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/api/serializers.py
--rw-r--r--   0 danirus    (501) staff       (20)      838 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/api/urls.py
--rw-r--r--   0 danirus    (501) staff       (20)     6316 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/api/views.py
--rw-r--r--   0 danirus    (501) staff       (20)      550 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/apps.py
--rw-r--r--   0 danirus    (501) staff       (20)     1178 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/compat.py
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.996720 django-comments-xtd-2.9.8/django_comments_xtd/conf/
--rw-r--r--   0 danirus    (501) staff       (20)      530 2014-01-09 10:13:11.000000 django-comments-xtd-2.9.8/django_comments_xtd/conf/__init__.py
--rw-r--r--   0 danirus    (501) staff       (20)     2337 2022-07-08 07:47:46.000000 django-comments-xtd-2.9.8/django_comments_xtd/conf/defaults.py
--rw-r--r--   0 danirus    (501) staff       (20)     2891 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/forms.py
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.985136 django-comments-xtd-2.9.8/django_comments_xtd/locale/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.984407 django-comments-xtd-2.9.8/django_comments_xtd/locale/de/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.997402 django-comments-xtd-2.9.8/django_comments_xtd/locale/de/LC_MESSAGES/
--rw-r--r--   0 danirus    (501) staff       (20)    10228 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 danirus    (501) staff       (20)    16299 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 danirus    (501) staff       (20)     2635 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 danirus    (501) staff       (20)     4530 2020-09-29 10:03:46.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.984505 django-comments-xtd-2.9.8/django_comments_xtd/locale/es/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.998037 django-comments-xtd-2.9.8/django_comments_xtd/locale/es/LC_MESSAGES/
--rw-r--r--   0 danirus    (501) staff       (20)     6071 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 danirus    (501) staff       (20)    15679 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 danirus    (501) staff       (20)     2497 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 danirus    (501) staff       (20)     4586 2018-01-19 18:27:51.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.984598 django-comments-xtd-2.9.8/django_comments_xtd/locale/fi/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.998750 django-comments-xtd-2.9.8/django_comments_xtd/locale/fi/LC_MESSAGES/
--rw-r--r--   0 danirus    (501) staff       (20)     5872 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 danirus    (501) staff       (20)    15330 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0 danirus    (501) staff       (20)     2445 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/fi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 danirus    (501) staff       (20)     4534 2018-01-19 18:27:51.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/fi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.984692 django-comments-xtd-2.9.8/django_comments_xtd/locale/fr/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.999409 django-comments-xtd-2.9.8/django_comments_xtd/locale/fr/LC_MESSAGES/
--rw-r--r--   0 danirus    (501) staff       (20)     6194 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 danirus    (501) staff       (20)    15795 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 danirus    (501) staff       (20)     2585 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 danirus    (501) staff       (20)     4677 2018-01-19 18:27:51.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.984786 django-comments-xtd-2.9.8/django_comments_xtd/locale/it/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.000074 django-comments-xtd-2.9.8/django_comments_xtd/locale/it/LC_MESSAGES/
--rw-r--r--   0 danirus    (501) staff       (20)     7483 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 danirus    (501) staff       (20)    15315 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 danirus    (501) staff       (20)     2785 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/it/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 danirus    (501) staff       (20)     4769 2021-02-28 10:08:44.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/it/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.984888 django-comments-xtd-2.9.8/django_comments_xtd/locale/nl/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.000798 django-comments-xtd-2.9.8/django_comments_xtd/locale/nl/LC_MESSAGES/
--rw-r--r--   0 danirus    (501) staff       (20)     6857 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 danirus    (501) staff       (20)    14754 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0 danirus    (501) staff       (20)     2563 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 danirus    (501) staff       (20)     4461 2020-09-29 10:03:46.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/nl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.984986 django-comments-xtd-2.9.8/django_comments_xtd/locale/no/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.001472 django-comments-xtd-2.9.8/django_comments_xtd/locale/no/LC_MESSAGES/
--rw-r--r--   0 danirus    (501) staff       (20)     6873 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/no/LC_MESSAGES/django.mo
--rw-r--r--   0 danirus    (501) staff       (20)    14766 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/no/LC_MESSAGES/django.po
--rw-r--r--   0 danirus    (501) staff       (20)     2408 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/no/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 danirus    (501) staff       (20)     4140 2019-12-24 18:20:38.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/no/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.985079 django-comments-xtd-2.9.8/django_comments_xtd/locale/ru/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.002368 django-comments-xtd-2.9.8/django_comments_xtd/locale/ru/LC_MESSAGES/
--rw-r--r--   0 danirus    (501) staff       (20)     8927 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 danirus    (501) staff       (20)    17147 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 danirus    (501) staff       (20)     3463 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 danirus    (501) staff       (20)     5364 2020-09-29 10:03:46.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.985180 django-comments-xtd-2.9.8/django_comments_xtd/locale/zh_Hans/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.002954 django-comments-xtd-2.9.8/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 danirus    (501) staff       (20)     6798 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 danirus    (501) staff       (20)    14408 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 danirus    (501) staff       (20)     2456 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 danirus    (501) staff       (20)     5824 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.003074 django-comments-xtd-2.9.8/django_comments_xtd/management/
--rw-r--r--   0 danirus    (501) staff       (20)        0 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/django_comments_xtd/management/__init__.py
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.003437 django-comments-xtd-2.9.8/django_comments_xtd/management/commands/
--rw-r--r--   0 danirus    (501) staff       (20)        0 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/django_comments_xtd/management/commands/__init__.py
--rw-r--r--   0 danirus    (501) staff       (20)     1642 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/management/commands/initialize_nested_count.py
--rw-r--r--   0 danirus    (501) staff       (20)     1947 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/management/commands/populate_xtdcomments.py
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.004848 django-comments-xtd-2.9.8/django_comments_xtd/migrations/
--rw-r--r--   0 danirus    (501) staff       (20)     1112 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/migrations/0001_initial.py
--rw-r--r--   0 danirus    (501) staff       (20)      685 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/migrations/0002_blacklisteddomain.py
--rw-r--r--   0 danirus    (501) staff       (20)      440 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/migrations/0003_auto_20170220_1333.py
--rw-r--r--   0 danirus    (501) staff       (20)      556 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/migrations/0004_auto_20170221_1510.py
--rw-r--r--   0 danirus    (501) staff       (20)      511 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/migrations/0005_auto_20170920_1247.py
--rw-r--r--   0 danirus    (501) staff       (20)      458 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/migrations/0006_auto_20181204_0948.py
--rw-r--r--   0 danirus    (501) staff       (20)      420 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/migrations/0007_xtdcomment_nested_count.py
--rw-r--r--   0 danirus    (501) staff       (20)      814 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/migrations/0008_auto_20200920_2037.py
--rw-r--r--   0 danirus    (501) staff       (20)        0 2015-04-29 09:19:07.000000 django-comments-xtd-2.9.8/django_comments_xtd/migrations/__init__.py
--rw-r--r--   0 danirus    (501) staff       (20)    12392 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/models.py
--rw-r--r--   0 danirus    (501) staff       (20)     5389 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/moderation.py
--rw-r--r--   0 danirus    (501) staff       (20)      649 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/signals.py
--rw-r--r--   0 danirus    (501) staff       (20)     4604 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/signed.py
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.985537 django-comments-xtd-2.9.8/django_comments_xtd/static/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.985763 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.006116 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/css/
--rw-r--r--   0 danirus    (501) staff       (20)     8886 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/css/_bootswatch.scss
--rwxr-xr-x   0 danirus    (501) staff       (20)     2367 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/css/_variables.scss
--rw-r--r--   0 danirus    (501) staff       (20)   206187 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/css/bootstrap.css
--rw-r--r--   0 danirus    (501) staff       (20)   166873 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/css/bootstrap.min.css
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.008401 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/
--rw-r--r--   0 danirus    (501) staff       (20)    20127 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 danirus    (501) staff       (20)   108738 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 danirus    (501) staff       (20)    45404 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 danirus    (501) staff       (20)    23424 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 danirus    (501) staff       (20)    18028 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.008584 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/img/
--rw-r--r--   0 danirus    (501) staff       (20)      635 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/img/64x64.svg
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.009219 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/
--rw-r--r--   0 danirus    (501) staff       (20)    33106 2022-09-18 10:31:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.8.js
--rw-r--r--   0 danirus    (501) staff       (20)    42069 2022-09-18 10:31:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.8.js.map
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.009995 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/src/
--rw-r--r--   0 danirus    (501) staff       (20)    14198 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/src/comment.jsx
--rw-r--r--   0 danirus    (501) staff       (20)     6295 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/src/commentbox.jsx
--rw-r--r--   0 danirus    (501) staff       (20)    14048 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/src/commentform.jsx
--rw-r--r--   0 danirus    (501) staff       (20)      332 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/src/index.js
--rw-r--r--   0 danirus    (501) staff       (20)      963 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/src/lib.js
--rw-r--r--   0 danirus    (501) staff       (20)    47214 2022-09-18 10:31:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.8.js
--rw-r--r--   0 danirus    (501) staff       (20)    69246 2022-09-18 10:31:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.8.js.map
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.010111 django-comments-xtd-2.9.8/django_comments_xtd/templates/
--rw-r--r--   0 danirus    (501) staff       (20)      304 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/404.html
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.011641 django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/
--rw-r--r--   0 danirus    (501) staff       (20)      274 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/comment_notification_email.txt
--rw-r--r--   0 danirus    (501) staff       (20)     1822 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/delete.html
--rw-r--r--   0 danirus    (501) staff       (20)      502 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/deleted.html
--rw-r--r--   0 danirus    (501) staff       (20)     2138 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/flag.html
--rw-r--r--   0 danirus    (501) staff       (20)      502 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/flagged.html
--rw-r--r--   0 danirus    (501) staff       (20)     2798 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/form.html
--rw-r--r--   0 danirus    (501) staff       (20)     1355 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/list.html
--rw-r--r--   0 danirus    (501) staff       (20)      701 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/posted.html
--rw-r--r--   0 danirus    (501) staff       (20)     1668 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/preview.html
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.014256 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/
--rw-r--r--   0 danirus    (501) staff       (20)       26 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/base.html
--rw-r--r--   0 danirus    (501) staff       (20)     1199 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/comment.html
--rw-r--r--   0 danirus    (501) staff       (20)     1844 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/comment_list.html
--rw-r--r--   0 danirus    (501) staff       (20)     3154 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/comment_tree.html
--rw-r--r--   0 danirus    (501) staff       (20)      286 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/discarded.html
--rw-r--r--   0 danirus    (501) staff       (20)     2812 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/dislike.html
--rw-r--r--   0 danirus    (501) staff       (20)      226 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/disliked.html
--rw-r--r--   0 danirus    (501) staff       (20)      949 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/email_confirmation_request.html
--rw-r--r--   0 danirus    (501) staff       (20)      760 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/email_confirmation_request.txt
--rw-r--r--   0 danirus    (501) staff       (20)      791 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/email_followup_comment.html
--rw-r--r--   0 danirus    (501) staff       (20)      590 2022-09-18 10:25:38.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/email_followup_comment.txt
--rw-r--r--   0 danirus    (501) staff       (20)     2780 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/like.html
--rw-r--r--   0 danirus    (501) staff       (20)      229 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/liked.html
--rw-r--r--   0 danirus    (501) staff       (20)      970 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/moderated.html
--rw-r--r--   0 danirus    (501) staff       (20)      405 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/muted.html
--rw-r--r--   0 danirus    (501) staff       (20)      187 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/only_users_can_post.html
--rw-r--r--   0 danirus    (501) staff       (20)      361 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/removal_notification_email.txt
--rw-r--r--   0 danirus    (501) staff       (20)     1221 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/reply.html
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.986259 django-comments-xtd-2.9.8/django_comments_xtd/templates/includes/
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.014791 django-comments-xtd-2.9.8/django_comments_xtd/templates/includes/django_comments_xtd/
--rw-r--r--   0 danirus    (501) staff       (20)       14 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/includes/django_comments_xtd/comment_content.html
--rw-r--r--   0 danirus    (501) staff       (20)        0 2017-05-18 13:53:04.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/includes/django_comments_xtd/render_comment.html~
--rw-r--r--   0 danirus    (501) staff       (20)      959 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templates/includes/django_comments_xtd/user_feedback.html
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.015021 django-comments-xtd-2.9.8/django_comments_xtd/templatetags/
--rw-r--r--   0 danirus    (501) staff       (20)        0 2014-01-09 10:13:11.000000 django-comments-xtd-2.9.8/django_comments_xtd/templatetags/__init__.py
--rw-r--r--   0 danirus    (501) staff       (20)    21321 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/templatetags/comments_xtd.py
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.018538 django-comments-xtd-2.9.8/django_comments_xtd/tests/
--rw-r--r--   0 danirus    (501) staff       (20)      973 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/__init__.py
--rw-r--r--   0 danirus    (501) staff       (20)      974 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/apiauth.py
--rw-r--r--   0 danirus    (501) staff       (20)      163 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/apps.py
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.019243 django-comments-xtd-2.9.8/django_comments_xtd/tests/migrations/
--rw-r--r--   0 danirus    (501) staff       (20)     2302 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/migrations/0001_initial.py
--rw-r--r--   0 danirus    (501) staff       (20)      530 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/migrations/0002_auto_20170523_1624.py
--rw-r--r--   0 danirus    (501) staff       (20)      678 2022-09-17 05:14:38.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/migrations/0003_uuiddiary.py
--rw-r--r--   0 danirus    (501) staff       (20)        0 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/migrations/__init__.py
--rw-r--r--   0 danirus    (501) staff       (20)     2348 2022-09-17 05:14:38.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/models.py
--rw-r--r--   0 danirus    (501) staff       (20)     3852 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/settings.py
--rw-r--r--   0 danirus    (501) staff       (20)     5028 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/test_api_views.py
--rw-r--r--   0 danirus    (501) staff       (20)     2742 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/test_cmd_initialize_nested_count.py
--rw-r--r--   0 danirus    (501) staff       (20)     2444 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/test_forms.py
--rw-r--r--   0 danirus    (501) staff       (20)     2782 2022-09-17 05:14:38.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/test_frontend.py
--rw-r--r--   0 danirus    (501) staff       (20)      768 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/test_get_version.py
--rw-r--r--   0 danirus    (501) staff       (20)    31297 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/test_models.py
--rw-r--r--   0 danirus    (501) staff       (20)    17289 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/test_moderation.py
--rw-r--r--   0 danirus    (501) staff       (20)    10829 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/test_serializers.py
--rw-r--r--   0 danirus    (501) staff       (20)     7603 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/test_templatetags.py
--rw-r--r--   0 danirus    (501) staff       (20)    21732 2022-09-18 10:25:38.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/test_views.py
--rw-r--r--   0 danirus    (501) staff       (20)      847 2022-07-08 07:47:46.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/urls.py
--rw-r--r--   0 danirus    (501) staff       (20)      449 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/utils.py
--rw-r--r--   0 danirus    (501) staff       (20)      115 2017-02-21 10:57:41.000000 django-comments-xtd-2.9.8/django_comments_xtd/tests/views.py
--rw-r--r--   0 danirus    (501) staff       (20)     1230 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/urls.py
--rw-r--r--   0 danirus    (501) staff       (20)     3996 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/django_comments_xtd/utils.py
--rw-r--r--   0 danirus    (501) staff       (20)    21288 2022-09-18 10:05:01.000000 django-comments-xtd-2.9.8/django_comments_xtd/views.py
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:08.995408 django-comments-xtd-2.9.8/django_comments_xtd.egg-info/
--rw-r--r--   0 danirus    (501) staff       (20)     1112 2022-09-18 10:33:08.000000 django-comments-xtd-2.9.8/django_comments_xtd.egg-info/PKG-INFO
--rw-r--r--   0 danirus    (501) staff       (20)    15977 2022-09-18 10:33:08.000000 django-comments-xtd-2.9.8/django_comments_xtd.egg-info/SOURCES.txt
--rw-r--r--   0 danirus    (501) staff       (20)        1 2022-09-18 10:33:08.000000 django-comments-xtd-2.9.8/django_comments_xtd.egg-info/dependency_links.txt
--rw-r--r--   0 danirus    (501) staff       (20)       92 2022-09-18 10:33:08.000000 django-comments-xtd-2.9.8/django_comments_xtd.egg-info/requires.txt
--rw-r--r--   0 danirus    (501) staff       (20)       20 2022-09-18 10:33:08.000000 django-comments-xtd-2.9.8/django_comments_xtd.egg-info/top_level.txt
--rw-r--r--   0 danirus    (501) staff       (20)        1 2017-08-07 19:36:48.000000 django-comments-xtd-2.9.8/django_comments_xtd.egg-info/zip-safe
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.024207 django-comments-xtd-2.9.8/docs/
--rw-r--r--   0 danirus    (501) staff       (20)     4642 2014-01-09 10:13:11.000000 django-comments-xtd-2.9.8/docs/Makefile
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.024683 django-comments-xtd-2.9.8/docs/__pycache__/
--rw-r--r--   0 danirus    (501) staff       (20)      597 2017-04-05 15:08:05.000000 django-comments-xtd-2.9.8/docs/__pycache__/extensions.cpython-35.pyc
--rw-r--r--   0 danirus    (501) staff       (20)      547 2017-05-17 10:40:57.000000 django-comments-xtd-2.9.8/docs/__pycache__/extensions.cpython-36.pyc
--rw-r--r--   0 danirus    (501) staff       (20)      567 2021-02-28 14:32:10.000000 django-comments-xtd-2.9.8/docs/__pycache__/extensions.cpython-38.pyc
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.024806 django-comments-xtd-2.9.8/docs/_build/
--rw-r--r--   0 danirus    (501) staff       (20)      230 2020-10-11 11:29:49.000000 django-comments-xtd-2.9.8/docs/_build/.buildinfo
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.035994 django-comments-xtd-2.9.8/docs/_build/.doctrees/
--rw-r--r--   0 danirus    (501) staff       (20)  3539313 2020-10-11 11:29:49.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/environment.pickle
--rw-r--r--   0 danirus    (501) staff       (20)    44436 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/example.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    22889 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/extending.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    19183 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/i18n.doctree
--rw-r--r--   0 danirus    (501) staff       (20)   103243 2020-10-11 11:29:49.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/index.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    29170 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/javascript.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    51747 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/logic.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    11764 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/migrating.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    27187 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/quickstart.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    60072 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/settings.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    50287 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/templates.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    59838 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/templatetags.doctree
--rw-r--r--   0 danirus    (501) staff       (20)   194305 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/tutorial.doctree
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.037063 django-comments-xtd-2.9.8/docs/_build/.doctrees/usecases/
--rw-r--r--   0 danirus    (501) staff       (20)    62853 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/usecases/change-user-image-or-avatar.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    39079 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/usecases/only-signed-in-can-comment.doctree
--rw-r--r--   0 danirus    (501) staff       (20)     3377 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/usecases.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    76888 2020-10-11 11:16:51.000000 django-comments-xtd-2.9.8/docs/_build/.doctrees/webapi.doctree
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.046042 django-comments-xtd-2.9.8/docs/_build/doctrees/
--rw-r--r--   0 danirus    (501) staff       (20)  2475254 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 danirus    (501) staff       (20)    40304 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/example.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    22889 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/extending.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    19045 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/i18n.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    16005 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/index.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    28475 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/javascript.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    48493 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/logic.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    11764 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/migrating.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    27187 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/quickstart.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    54490 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/settings.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    50229 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/templates.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    56642 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/templatetags.doctree
--rw-r--r--   0 danirus    (501) staff       (20)   190001 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/tutorial.doctree
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.046537 django-comments-xtd-2.9.8/docs/_build/doctrees/usecases/
--rw-r--r--   0 danirus    (501) staff       (20)     8065 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/usecases/only-signed-in-can-comment.doctree
--rw-r--r--   0 danirus    (501) staff       (20)     3419 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/usecases.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    32780 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.8/docs/_build/doctrees/webapi.doctree
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.051463 django-comments-xtd-2.9.8/docs/_build/html/
--rw-r--r--   0 danirus    (501) staff       (20)      230 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/.buildinfo
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.062837 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/
--rw-r--r--   0 danirus    (501) staff       (20)  3541715 2020-10-11 11:36:25.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/environment.pickle
--rw-r--r--   0 danirus    (501) staff       (20)    44436 2020-10-11 11:35:47.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/example.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    22889 2020-10-11 11:35:47.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/extending.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    19183 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/i18n.doctree
--rw-r--r--   0 danirus    (501) staff       (20)   109616 2020-10-11 11:36:25.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/index.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    29170 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/javascript.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    51747 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/logic.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    11764 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/migrating.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    27187 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/quickstart.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    74148 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/settings.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    50287 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/templates.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    59838 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/templatetags.doctree
--rw-r--r--   0 danirus    (501) staff       (20)   194305 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/tutorial.doctree
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.063924 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/usecases/
--rw-r--r--   0 danirus    (501) staff       (20)    62853 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/usecases/change-user-image-or-avatar.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    39079 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/usecases/only-signed-in-can-comment.doctree
--rw-r--r--   0 danirus    (501) staff       (20)     3377 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/usecases.doctree
--rw-r--r--   0 danirus    (501) staff       (20)    76888 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.8/docs/_build/html/.doctrees/webapi.doctree
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.067613 django-comments-xtd-2.9.8/docs/_build/html/_images/
--rw-r--r--   0 danirus    (501) staff       (20)    80426 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/comments-enabled.png
--rw-r--r--   0 danirus    (501) staff       (20)   183596 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/cover.png
--rw-r--r--   0 danirus    (501) staff       (20)    53244 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/extend-comments-app.png
--rw-r--r--   0 danirus    (501) staff       (20)    32110 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/feedback-buttons.png
--rw-r--r--   0 danirus    (501) staff       (20)    75480 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/feedback-users.png
--rw-r--r--   0 danirus    (501) staff       (20)    44521 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/flag-counter.png
--rw-r--r--   0 danirus    (501) staff       (20)    22281 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/markdown-comment.png
--rw-r--r--   0 danirus    (501) staff       (20)    26498 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/markdown-input.png
--rw-r--r--   0 danirus    (501) staff       (20)    46276 2020-07-05 07:40:16.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/only-users-can-post.png
--rw-r--r--   0 danirus    (501) staff       (20)    73259 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/reply-link.png
--rw-r--r--   0 danirus    (501) staff       (20)    96365 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/_build/html/_images/update-comment-tree.png
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.071130 django-comments-xtd-2.9.8/docs/_build/html/_sources/
--rw-r--r--   0 danirus    (501) staff       (20)     7422 2020-09-29 10:03:46.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/example.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)     5024 2018-08-12 10:16:22.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/extending.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)     3810 2020-06-08 12:15:51.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/i18n.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)    17953 2020-10-11 11:36:25.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)     7538 2020-10-11 11:35:47.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/javascript.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)     9648 2020-07-28 17:33:27.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/logic.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)     2709 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/migrating.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)     4012 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/quickstart.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)    12893 2020-10-11 11:35:47.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/settings.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)     7349 2020-07-28 17:33:27.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/templates.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)     9658 2020-07-05 10:39:13.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/templatetags.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)    44847 2020-10-11 11:35:47.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/tutorial.rst.txt
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.071574 django-comments-xtd-2.9.8/docs/_build/html/_sources/usecases/
--rw-r--r--   0 danirus    (501) staff       (20)    12965 2020-08-08 12:51:49.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/usecases/change-user-image-or-avatar.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)     9043 2020-07-05 07:34:30.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/usecases/only-signed-in-can-comment.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)      238 2020-08-09 07:01:34.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/usecases.rst.txt
--rw-r--r--   0 danirus    (501) staff       (20)    19433 2020-07-28 17:33:27.000000 django-comments-xtd-2.9.8/docs/_build/html/_sources/webapi.rst.txt
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.075516 django-comments-xtd-2.9.8/docs/_build/html/_static/
--rw-r--r--   0 danirus    (501) staff       (20)    12261 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.075795 django-comments-xtd-2.9.8/docs/_build/html/_static/css/
--rw-r--r--   0 danirus    (501) staff       (20)     3391 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/css/badge_only.css
--rw-r--r--   0 danirus    (501) staff       (20)   118340 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 danirus    (501) staff       (20)     9270 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/doctools.js
--rw-r--r--   0 danirus    (501) staff       (20)      329 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 danirus    (501) staff       (20)      286 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/file.png
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.085834 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/
--rw-r--r--   0 danirus    (501) staff       (20)   109948 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Inconsolata-Bold.ttf
--rw-r--r--   0 danirus    (501) staff       (20)    96964 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Inconsolata-Regular.ttf
--rw-r--r--   0 danirus    (501) staff       (20)    63184 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Inconsolata.ttf
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.105616 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/
--rw-r--r--   0 danirus    (501) staff       (20)   256056 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bold.eot
--rw-r--r--   0 danirus    (501) staff       (20)   600856 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bold.ttf
--rw-r--r--   0 danirus    (501) staff       (20)   309728 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bold.woff
--rw-r--r--   0 danirus    (501) staff       (20)   184912 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bold.woff2
--rw-r--r--   0 danirus    (501) staff       (20)   266158 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bolditalic.eot
--rw-r--r--   0 danirus    (501) staff       (20)   622572 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bolditalic.ttf
--rw-r--r--   0 danirus    (501) staff       (20)   323344 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bolditalic.woff
--rw-r--r--   0 danirus    (501) staff       (20)   193308 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bolditalic.woff2
--rw-r--r--   0 danirus    (501) staff       (20)   268604 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-italic.eot
--rw-r--r--   0 danirus    (501) staff       (20)   639388 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-italic.ttf
--rw-r--r--   0 danirus    (501) staff       (20)   328412 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-italic.woff
--rw-r--r--   0 danirus    (501) staff       (20)   195704 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-italic.woff2
--rw-r--r--   0 danirus    (501) staff       (20)   253461 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-regular.eot
--rw-r--r--   0 danirus    (501) staff       (20)   607720 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-regular.ttf
--rw-r--r--   0 danirus    (501) staff       (20)   309192 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-regular.woff
--rw-r--r--   0 danirus    (501) staff       (20)   182708 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-regular.woff2
--rw-r--r--   0 danirus    (501) staff       (20)   656544 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato-Bold.ttf
--rw-r--r--   0 danirus    (501) staff       (20)   656568 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato-Regular.ttf
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.110778 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/
--rw-r--r--   0 danirus    (501) staff       (20)    79520 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
--rw-r--r--   0 danirus    (501) staff       (20)   170616 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
--rw-r--r--   0 danirus    (501) staff       (20)    87624 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
--rw-r--r--   0 danirus    (501) staff       (20)    67312 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
--rw-r--r--   0 danirus    (501) staff       (20)    78331 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
--rw-r--r--   0 danirus    (501) staff       (20)   169064 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
--rw-r--r--   0 danirus    (501) staff       (20)    86288 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
--rw-r--r--   0 danirus    (501) staff       (20)    66444 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
--rw-r--r--   0 danirus    (501) staff       (20)   170616 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab-Bold.ttf
--rw-r--r--   0 danirus    (501) staff       (20)   169064 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab-Regular.ttf
--rw-r--r--   0 danirus    (501) staff       (20)   165742 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 danirus    (501) staff       (20)   444379 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 danirus    (501) staff       (20)   165548 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 danirus    (501) staff       (20)    98024 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 danirus    (501) staff       (20)    77160 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 danirus    (501) staff       (20)   280364 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/jquery-3.4.1.js
--rw-r--r--   0 danirus    (501) staff       (20)    88145 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.111373 django-comments-xtd-2.9.8/docs/_build/html/_static/js/
--rw-r--r--   0 danirus    (501) staff       (20)    15414 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/js/modernizr.min.js
--rw-r--r--   0 danirus    (501) staff       (20)     4414 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 danirus    (501) staff       (20)    10847 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/language_data.js
--rw-r--r--   0 danirus    (501) staff       (20)       90 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/minus.png
--rw-r--r--   0 danirus    (501) staff       (20)       90 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/plus.png
--rw-r--r--   0 danirus    (501) staff       (20)     4395 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/pygments.css
--rw-r--r--   0 danirus    (501) staff       (20)    16029 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 danirus    (501) staff       (20)    35168 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 danirus    (501) staff       (20)    12140 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.8/docs/_build/html/_static/underscore.js
--rw-r--r--   0 danirus    (501) staff       (20)    19720 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/example.html
--rw-r--r--   0 danirus    (501) staff       (20)    22841 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/extending.html
--rw-r--r--   0 danirus    (501) staff       (20)    23005 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/genindex.html
--rw-r--r--   0 danirus    (501) staff       (20)    13945 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/i18n.html
--rw-r--r--   0 danirus    (501) staff       (20)    40911 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/index.html
--rw-r--r--   0 danirus    (501) staff       (20)    19814 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/javascript.html
--rw-r--r--   0 danirus    (501) staff       (20)    25434 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/logic.html
--rw-r--r--   0 danirus    (501) staff       (20)    12353 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/migrating.html
--rw-r--r--   0 danirus    (501) staff       (20)     1253 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/objects.inv
--rw-r--r--   0 danirus    (501) staff       (20)     5772 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/py-modindex.html
--rw-r--r--   0 danirus    (501) staff       (20)    15021 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/quickstart.html
--rw-r--r--   0 danirus    (501) staff       (20)     5602 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/search.html
--rw-r--r--   0 danirus    (501) staff       (20)    30022 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.8/docs/_build/html/searchindex.js
--rw-r--r--   0 danirus    (501) staff       (20)    42775 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/settings.html
--rw-r--r--   0 danirus    (501) staff       (20)    25812 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/templates.html
--rw-r--r--   0 danirus    (501) staff       (20)    37487 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/templatetags.html
--rw-r--r--   0 danirus    (501) staff       (20)   110167 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/tutorial.html
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.112216 django-comments-xtd-2.9.8/docs/_build/html/usecases/
--rw-r--r--   0 danirus    (501) staff       (20)    37849 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/usecases/change-user-image-or-avatar.html
--rw-r--r--   0 danirus    (501) staff       (20)    28677 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/usecases/only-signed-in-can-comment.html
--rw-r--r--   0 danirus    (501) staff       (20)     6828 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/usecases.html
--rw-r--r--   0 danirus    (501) staff       (20)    49376 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.8/docs/_build/html/webapi.html
--rw-r--r--   0 danirus    (501) staff       (20)     7777 2022-09-18 10:25:40.000000 django-comments-xtd-2.9.8/docs/conf.py
--rw-r--r--   0 danirus    (501) staff       (20)     7422 2020-09-29 10:03:46.000000 django-comments-xtd-2.9.8/docs/example.rst
--rw-r--r--   0 danirus    (501) staff       (20)     5022 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/docs/extending.rst
--rw-r--r--   0 danirus    (501) staff       (20)      621 2021-02-28 14:28:58.000000 django-comments-xtd-2.9.8/docs/extensions.py
--rw-r--r--   0 danirus    (501) staff       (20)     3885 2021-02-28 10:08:44.000000 django-comments-xtd-2.9.8/docs/i18n.rst
--rw-r--r--   0 danirus    (501) staff       (20)        0 2017-06-04 11:43:16.000000 django-comments-xtd-2.9.8/docs/i18n.rst~
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.116034 django-comments-xtd-2.9.8/docs/images/
--rw-r--r--   0 danirus    (501) staff       (20)    80426 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/images/comments-enabled.png
--rw-r--r--   0 danirus    (501) staff       (20)   183596 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/images/cover.png
--rw-r--r--   0 danirus    (501) staff       (20)    53244 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/images/extend-comments-app.png
--rw-r--r--   0 danirus    (501) staff       (20)    32110 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/images/feedback-buttons.png
--rw-r--r--   0 danirus    (501) staff       (20)    75480 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/images/feedback-users.png
--rw-r--r--   0 danirus    (501) staff       (20)    44521 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/images/flag-counter.png
--rw-r--r--   0 danirus    (501) staff       (20)    22281 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/images/markdown-comment.png
--rw-r--r--   0 danirus    (501) staff       (20)    26498 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/images/markdown-input.png
--rw-r--r--   0 danirus    (501) staff       (20)    46276 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.8/docs/images/only-users-can-post.png
--rw-r--r--   0 danirus    (501) staff       (20)    97842 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/images/preview-comment.png
--rw-r--r--   0 danirus    (501) staff       (20)    73259 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/images/reply-link.png
--rw-r--r--   0 danirus    (501) staff       (20)    96365 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/images/update-comment-tree.png
--rw-r--r--   0 danirus    (501) staff       (20)    24539 2022-09-18 10:25:40.000000 django-comments-xtd-2.9.8/docs/index.rst
--rw-r--r--   0 danirus    (501) staff       (20)     7538 2022-09-18 10:25:40.000000 django-comments-xtd-2.9.8/docs/javascript.rst
--rw-r--r--   0 danirus    (501) staff       (20)        0 2017-05-19 04:48:08.000000 django-comments-xtd-2.9.8/docs/javascript.rst~
--rw-r--r--   0 danirus    (501) staff       (20)     9648 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.8/docs/logic.rst
--rw-r--r--   0 danirus    (501) staff       (20)     4537 2014-01-09 10:13:11.000000 django-comments-xtd-2.9.8/docs/make.bat
--rw-r--r--   0 danirus    (501) staff       (20)     1218 2021-06-06 15:06:10.000000 django-comments-xtd-2.9.8/docs/management.rst
--rw-r--r--   0 danirus    (501) staff       (20)     2709 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.8/docs/migrating.rst
--rw-r--r--   0 danirus    (501) staff       (20)      459 2017-06-07 05:48:01.000000 django-comments-xtd-2.9.8/docs/migrating.rst~
--rw-r--r--   0 danirus    (501) staff       (20)     4012 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.8/docs/quickstart.rst
--rw-r--r--   0 danirus    (501) staff       (20)       14 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/docs/requirements.txt
--rw-r--r--   0 danirus    (501) staff       (20)    10595 2022-07-08 07:47:46.000000 django-comments-xtd-2.9.8/docs/settings.rst
--rw-r--r--   0 danirus    (501) staff       (20)     7349 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.8/docs/templates.rst
--rw-r--r--   0 danirus    (501) staff       (20)     9658 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.8/docs/templatetags.rst
--rw-r--r--   0 danirus    (501) staff       (20)    45005 2022-09-18 10:25:40.000000 django-comments-xtd-2.9.8/docs/tutorial.rst
-drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-09-18 10:33:09.116580 django-comments-xtd-2.9.8/docs/usecases/
--rw-r--r--   0 danirus    (501) staff       (20)    12965 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.8/docs/usecases/change-user-image-or-avatar.rst
--rw-r--r--   0 danirus    (501) staff       (20)     9043 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.8/docs/usecases/only-signed-in-can-comment.rst
--rw-r--r--   0 danirus    (501) staff       (20)      238 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.8/docs/usecases.rst
--rw-r--r--   0 danirus    (501) staff       (20)    19504 2021-02-16 14:04:32.000000 django-comments-xtd-2.9.8/docs/webapi.rst
--rw-r--r--   0 danirus    (501) staff       (20)        0 2017-05-21 05:59:07.000000 django-comments-xtd-2.9.8/docs/webapi.rst~
--rw-r--r--   0 danirus    (501) staff       (20)      779 2022-09-18 10:25:40.000000 django-comments-xtd-2.9.8/package.json
--rw-r--r--   0 danirus    (501) staff       (20)      645 2022-09-18 10:25:40.000000 django-comments-xtd-2.9.8/pyproject.toml
--rw-r--r--   0 danirus    (501) staff       (20)      131 2022-04-07 09:36:20.000000 django-comments-xtd-2.9.8/requirements.pip
--rw-r--r--   0 danirus    (501) staff       (20)       80 2022-09-18 10:25:40.000000 django-comments-xtd-2.9.8/requirements_tests.pip
--rw-r--r--   0 danirus    (501) staff       (20)       38 2022-09-18 10:33:09.117053 django-comments-xtd-2.9.8/setup.cfg
--rw-r--r--   0 danirus    (501) staff       (20)     1819 2022-09-18 10:25:40.000000 django-comments-xtd-2.9.8/setup.py
--rw-r--r--   0 danirus    (501) staff       (20)     1540 2022-09-18 10:25:38.000000 django-comments-xtd-2.9.8/tox.ini
--rw-r--r--   0 danirus    (501) staff       (20)     1026 2022-09-18 10:25:40.000000 django-comments-xtd-2.9.8/webpack.config.js
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.123957 django-comments-xtd-2.9.9/
+-rw-r--r--   0 danirus    (501) staff       (20)     3989 2020-05-12 19:59:09.000000 django-comments-xtd-2.9.9/.coverage
+-rw-r--r--   0 danirus    (501) staff       (20)      290 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/.gitignore
+-rw-r--r--   0 danirus    (501) staff       (20)      956 2022-09-18 10:25:38.000000 django-comments-xtd-2.9.9/AUTHORS
+-rw-r--r--   0 danirus    (501) staff       (20)    18220 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/CHANGELOG.md
+-rw-r--r--   0 danirus    (501) staff       (20)     1303 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/LICENSE
+-rw-r--r--   0 danirus    (501) staff       (20)      341 2017-07-31 17:55:32.000000 django-comments-xtd-2.9.9/MANIFEST.in
+-rw-r--r--   0 danirus    (501) staff       (20)     1112 2022-10-26 12:44:57.123830 django-comments-xtd-2.9.9/PKG-INFO
+-rw-r--r--   0 danirus    (501) staff       (20)     1796 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/README.rst
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.997861 django-comments-xtd-2.9.9/django_comments_xtd/
+-rw-r--r--   0 danirus    (501) staff       (20)      771 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/django_comments_xtd/__init__.py
+-rw-r--r--   0 danirus    (501) staff       (20)     1729 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/admin.py
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.999807 django-comments-xtd-2.9.9/django_comments_xtd/api/
+-rw-r--r--   0 danirus    (501) staff       (20)      285 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/api/__init__.py
+-rw-r--r--   0 danirus    (501) staff       (20)     7489 2022-09-17 05:14:38.000000 django-comments-xtd-2.9.9/django_comments_xtd/api/frontend.py
+-rw-r--r--   0 danirus    (501) staff       (20)    12552 2022-10-26 12:38:35.000000 django-comments-xtd-2.9.9/django_comments_xtd/api/serializers.py
+-rw-r--r--   0 danirus    (501) staff       (20)      838 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/api/urls.py
+-rw-r--r--   0 danirus    (501) staff       (20)     6316 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/api/views.py
+-rw-r--r--   0 danirus    (501) staff       (20)      550 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/apps.py
+-rw-r--r--   0 danirus    (501) staff       (20)     1178 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/compat.py
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.000195 django-comments-xtd-2.9.9/django_comments_xtd/conf/
+-rw-r--r--   0 danirus    (501) staff       (20)      530 2014-01-09 10:13:11.000000 django-comments-xtd-2.9.9/django_comments_xtd/conf/__init__.py
+-rw-r--r--   0 danirus    (501) staff       (20)     2337 2022-07-08 07:47:46.000000 django-comments-xtd-2.9.9/django_comments_xtd/conf/defaults.py
+-rw-r--r--   0 danirus    (501) staff       (20)     2891 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/forms.py
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.990147 django-comments-xtd-2.9.9/django_comments_xtd/locale/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.989375 django-comments-xtd-2.9.9/django_comments_xtd/locale/de/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.001234 django-comments-xtd-2.9.9/django_comments_xtd/locale/de/LC_MESSAGES/
+-rw-r--r--   0 danirus    (501) staff       (20)    10228 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 danirus    (501) staff       (20)    16299 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 danirus    (501) staff       (20)     2635 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 danirus    (501) staff       (20)     4530 2020-09-29 10:03:46.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.989477 django-comments-xtd-2.9.9/django_comments_xtd/locale/es/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.002114 django-comments-xtd-2.9.9/django_comments_xtd/locale/es/LC_MESSAGES/
+-rw-r--r--   0 danirus    (501) staff       (20)     6071 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 danirus    (501) staff       (20)    15679 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 danirus    (501) staff       (20)     2497 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 danirus    (501) staff       (20)     4586 2018-01-19 18:27:51.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.989576 django-comments-xtd-2.9.9/django_comments_xtd/locale/fi/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.003054 django-comments-xtd-2.9.9/django_comments_xtd/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 danirus    (501) staff       (20)     5872 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 danirus    (501) staff       (20)    15330 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0 danirus    (501) staff       (20)     2445 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/fi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 danirus    (501) staff       (20)     4534 2018-01-19 18:27:51.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/fi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.989681 django-comments-xtd-2.9.9/django_comments_xtd/locale/fr/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.003944 django-comments-xtd-2.9.9/django_comments_xtd/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 danirus    (501) staff       (20)     6194 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 danirus    (501) staff       (20)    15795 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 danirus    (501) staff       (20)     2585 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 danirus    (501) staff       (20)     4677 2018-01-19 18:27:51.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.989778 django-comments-xtd-2.9.9/django_comments_xtd/locale/it/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.004807 django-comments-xtd-2.9.9/django_comments_xtd/locale/it/LC_MESSAGES/
+-rw-r--r--   0 danirus    (501) staff       (20)     7483 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 danirus    (501) staff       (20)    15315 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 danirus    (501) staff       (20)     2785 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/it/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 danirus    (501) staff       (20)     4769 2021-02-28 10:08:44.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/it/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.989885 django-comments-xtd-2.9.9/django_comments_xtd/locale/nl/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.005600 django-comments-xtd-2.9.9/django_comments_xtd/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 danirus    (501) staff       (20)     6857 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 danirus    (501) staff       (20)    14754 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0 danirus    (501) staff       (20)     2563 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 danirus    (501) staff       (20)     4461 2020-09-29 10:03:46.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.989987 django-comments-xtd-2.9.9/django_comments_xtd/locale/no/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.006495 django-comments-xtd-2.9.9/django_comments_xtd/locale/no/LC_MESSAGES/
+-rw-r--r--   0 danirus    (501) staff       (20)     6873 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/no/LC_MESSAGES/django.mo
+-rw-r--r--   0 danirus    (501) staff       (20)    14766 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/no/LC_MESSAGES/django.po
+-rw-r--r--   0 danirus    (501) staff       (20)     2408 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/no/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 danirus    (501) staff       (20)     4140 2019-12-24 18:20:38.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/no/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.990085 django-comments-xtd-2.9.9/django_comments_xtd/locale/ru/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.007428 django-comments-xtd-2.9.9/django_comments_xtd/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 danirus    (501) staff       (20)     8927 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 danirus    (501) staff       (20)    17147 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 danirus    (501) staff       (20)     3463 2021-11-11 16:40:18.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 danirus    (501) staff       (20)     5364 2020-09-29 10:03:46.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.990186 django-comments-xtd-2.9.9/django_comments_xtd/locale/zh_Hans/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.008239 django-comments-xtd-2.9.9/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 danirus    (501) staff       (20)     6798 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 danirus    (501) staff       (20)    14408 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 danirus    (501) staff       (20)     2456 2022-09-18 10:32:49.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 danirus    (501) staff       (20)     5824 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.008382 django-comments-xtd-2.9.9/django_comments_xtd/management/
+-rw-r--r--   0 danirus    (501) staff       (20)        0 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/django_comments_xtd/management/__init__.py
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.008685 django-comments-xtd-2.9.9/django_comments_xtd/management/commands/
+-rw-r--r--   0 danirus    (501) staff       (20)        0 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/django_comments_xtd/management/commands/__init__.py
+-rw-r--r--   0 danirus    (501) staff       (20)     1642 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/management/commands/initialize_nested_count.py
+-rw-r--r--   0 danirus    (501) staff       (20)     1947 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/management/commands/populate_xtdcomments.py
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.010005 django-comments-xtd-2.9.9/django_comments_xtd/migrations/
+-rw-r--r--   0 danirus    (501) staff       (20)     1112 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/migrations/0001_initial.py
+-rw-r--r--   0 danirus    (501) staff       (20)      685 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/migrations/0002_blacklisteddomain.py
+-rw-r--r--   0 danirus    (501) staff       (20)      440 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/migrations/0003_auto_20170220_1333.py
+-rw-r--r--   0 danirus    (501) staff       (20)      556 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/migrations/0004_auto_20170221_1510.py
+-rw-r--r--   0 danirus    (501) staff       (20)      511 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/migrations/0005_auto_20170920_1247.py
+-rw-r--r--   0 danirus    (501) staff       (20)      458 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/migrations/0006_auto_20181204_0948.py
+-rw-r--r--   0 danirus    (501) staff       (20)      420 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/migrations/0007_xtdcomment_nested_count.py
+-rw-r--r--   0 danirus    (501) staff       (20)      814 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/migrations/0008_auto_20200920_2037.py
+-rw-r--r--   0 danirus    (501) staff       (20)        0 2015-04-29 09:19:07.000000 django-comments-xtd-2.9.9/django_comments_xtd/migrations/__init__.py
+-rw-r--r--   0 danirus    (501) staff       (20)    12392 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/models.py
+-rw-r--r--   0 danirus    (501) staff       (20)     5389 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/moderation.py
+-rw-r--r--   0 danirus    (501) staff       (20)      649 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/signals.py
+-rw-r--r--   0 danirus    (501) staff       (20)     4604 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/signed.py
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.990509 django-comments-xtd-2.9.9/django_comments_xtd/static/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.990783 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.011298 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/css/
+-rw-r--r--   0 danirus    (501) staff       (20)     8886 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/css/_bootswatch.scss
+-rwxr-xr-x   0 danirus    (501) staff       (20)     2367 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/css/_variables.scss
+-rw-r--r--   0 danirus    (501) staff       (20)   206187 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/css/bootstrap.css
+-rw-r--r--   0 danirus    (501) staff       (20)   166873 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/css/bootstrap.min.css
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.013448 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/
+-rw-r--r--   0 danirus    (501) staff       (20)    20127 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 danirus    (501) staff       (20)   108738 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 danirus    (501) staff       (20)    45404 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)    23424 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 danirus    (501) staff       (20)    18028 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.013641 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/img/
+-rw-r--r--   0 danirus    (501) staff       (20)      635 2017-04-14 10:49:30.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/img/64x64.svg
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.014320 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/
+-rw-r--r--   0 danirus    (501) staff       (20)    33106 2022-10-26 12:44:30.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.9.js
+-rw-r--r--   0 danirus    (501) staff       (20)    42069 2022-10-26 12:44:30.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.9.js.map
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.014891 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/src/
+-rw-r--r--   0 danirus    (501) staff       (20)    14198 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/src/comment.jsx
+-rw-r--r--   0 danirus    (501) staff       (20)     6295 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/src/commentbox.jsx
+-rw-r--r--   0 danirus    (501) staff       (20)    14048 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/src/commentform.jsx
+-rw-r--r--   0 danirus    (501) staff       (20)      332 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/src/index.js
+-rw-r--r--   0 danirus    (501) staff       (20)      963 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/src/lib.js
+-rw-r--r--   0 danirus    (501) staff       (20)    47214 2022-10-26 12:44:30.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.9.js
+-rw-r--r--   0 danirus    (501) staff       (20)    69246 2022-10-26 12:44:30.000000 django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.9.js.map
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.014992 django-comments-xtd-2.9.9/django_comments_xtd/templates/
+-rw-r--r--   0 danirus    (501) staff       (20)      304 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/404.html
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.016284 django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/
+-rw-r--r--   0 danirus    (501) staff       (20)      274 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/comment_notification_email.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     1822 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/delete.html
+-rw-r--r--   0 danirus    (501) staff       (20)      502 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/deleted.html
+-rw-r--r--   0 danirus    (501) staff       (20)     2138 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/flag.html
+-rw-r--r--   0 danirus    (501) staff       (20)      502 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/flagged.html
+-rw-r--r--   0 danirus    (501) staff       (20)     2798 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/form.html
+-rw-r--r--   0 danirus    (501) staff       (20)     1355 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/list.html
+-rw-r--r--   0 danirus    (501) staff       (20)      701 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/posted.html
+-rw-r--r--   0 danirus    (501) staff       (20)     1668 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/preview.html
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.018876 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/
+-rw-r--r--   0 danirus    (501) staff       (20)       26 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/base.html
+-rw-r--r--   0 danirus    (501) staff       (20)     1199 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/comment.html
+-rw-r--r--   0 danirus    (501) staff       (20)     1844 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/comment_list.html
+-rw-r--r--   0 danirus    (501) staff       (20)     3154 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/comment_tree.html
+-rw-r--r--   0 danirus    (501) staff       (20)      286 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/discarded.html
+-rw-r--r--   0 danirus    (501) staff       (20)     2812 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/dislike.html
+-rw-r--r--   0 danirus    (501) staff       (20)      226 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/disliked.html
+-rw-r--r--   0 danirus    (501) staff       (20)      949 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/email_confirmation_request.html
+-rw-r--r--   0 danirus    (501) staff       (20)      760 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/email_confirmation_request.txt
+-rw-r--r--   0 danirus    (501) staff       (20)      791 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/email_followup_comment.html
+-rw-r--r--   0 danirus    (501) staff       (20)      590 2022-09-18 10:25:38.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/email_followup_comment.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     2780 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/like.html
+-rw-r--r--   0 danirus    (501) staff       (20)      229 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/liked.html
+-rw-r--r--   0 danirus    (501) staff       (20)      970 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/moderated.html
+-rw-r--r--   0 danirus    (501) staff       (20)      405 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/muted.html
+-rw-r--r--   0 danirus    (501) staff       (20)      187 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/only_users_can_post.html
+-rw-r--r--   0 danirus    (501) staff       (20)      361 2022-09-18 09:16:13.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/removal_notification_email.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     1221 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/reply.html
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.991140 django-comments-xtd-2.9.9/django_comments_xtd/templates/includes/
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.019401 django-comments-xtd-2.9.9/django_comments_xtd/templates/includes/django_comments_xtd/
+-rw-r--r--   0 danirus    (501) staff       (20)       14 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/includes/django_comments_xtd/comment_content.html
+-rw-r--r--   0 danirus    (501) staff       (20)        0 2017-05-18 13:53:04.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/includes/django_comments_xtd/render_comment.html~
+-rw-r--r--   0 danirus    (501) staff       (20)      959 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templates/includes/django_comments_xtd/user_feedback.html
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.019644 django-comments-xtd-2.9.9/django_comments_xtd/templatetags/
+-rw-r--r--   0 danirus    (501) staff       (20)        0 2014-01-09 10:13:11.000000 django-comments-xtd-2.9.9/django_comments_xtd/templatetags/__init__.py
+-rw-r--r--   0 danirus    (501) staff       (20)    21321 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/templatetags/comments_xtd.py
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.023047 django-comments-xtd-2.9.9/django_comments_xtd/tests/
+-rw-r--r--   0 danirus    (501) staff       (20)      973 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/__init__.py
+-rw-r--r--   0 danirus    (501) staff       (20)      974 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/apiauth.py
+-rw-r--r--   0 danirus    (501) staff       (20)      163 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/apps.py
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.023698 django-comments-xtd-2.9.9/django_comments_xtd/tests/migrations/
+-rw-r--r--   0 danirus    (501) staff       (20)     2302 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/migrations/0001_initial.py
+-rw-r--r--   0 danirus    (501) staff       (20)      530 2022-01-04 18:27:47.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/migrations/0002_auto_20170523_1624.py
+-rw-r--r--   0 danirus    (501) staff       (20)      678 2022-09-17 05:14:38.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/migrations/0003_uuiddiary.py
+-rw-r--r--   0 danirus    (501) staff       (20)        0 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/migrations/__init__.py
+-rw-r--r--   0 danirus    (501) staff       (20)     2348 2022-09-17 05:14:38.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/models.py
+-rw-r--r--   0 danirus    (501) staff       (20)     3852 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/settings.py
+-rw-r--r--   0 danirus    (501) staff       (20)     5028 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/test_api_views.py
+-rw-r--r--   0 danirus    (501) staff       (20)     2742 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/test_cmd_initialize_nested_count.py
+-rw-r--r--   0 danirus    (501) staff       (20)     2444 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/test_forms.py
+-rw-r--r--   0 danirus    (501) staff       (20)     2782 2022-09-17 05:14:38.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/test_frontend.py
+-rw-r--r--   0 danirus    (501) staff       (20)      768 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/test_get_version.py
+-rw-r--r--   0 danirus    (501) staff       (20)    31297 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/test_models.py
+-rw-r--r--   0 danirus    (501) staff       (20)    17289 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/test_moderation.py
+-rw-r--r--   0 danirus    (501) staff       (20)    10829 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/test_serializers.py
+-rw-r--r--   0 danirus    (501) staff       (20)     7603 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/test_templatetags.py
+-rw-r--r--   0 danirus    (501) staff       (20)    21732 2022-09-18 10:25:38.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/test_views.py
+-rw-r--r--   0 danirus    (501) staff       (20)      847 2022-07-08 07:47:46.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/urls.py
+-rw-r--r--   0 danirus    (501) staff       (20)      449 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/utils.py
+-rw-r--r--   0 danirus    (501) staff       (20)      115 2017-02-21 10:57:41.000000 django-comments-xtd-2.9.9/django_comments_xtd/tests/views.py
+-rw-r--r--   0 danirus    (501) staff       (20)     1230 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/urls.py
+-rw-r--r--   0 danirus    (501) staff       (20)     3996 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/django_comments_xtd/utils.py
+-rw-r--r--   0 danirus    (501) staff       (20)    21288 2022-09-18 10:05:01.000000 django-comments-xtd-2.9.9/django_comments_xtd/views.py
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:56.998810 django-comments-xtd-2.9.9/django_comments_xtd.egg-info/
+-rw-r--r--   0 danirus    (501) staff       (20)     1112 2022-10-26 12:44:56.000000 django-comments-xtd-2.9.9/django_comments_xtd.egg-info/PKG-INFO
+-rw-r--r--   0 danirus    (501) staff       (20)    15977 2022-10-26 12:44:56.000000 django-comments-xtd-2.9.9/django_comments_xtd.egg-info/SOURCES.txt
+-rw-r--r--   0 danirus    (501) staff       (20)        1 2022-10-26 12:44:56.000000 django-comments-xtd-2.9.9/django_comments_xtd.egg-info/dependency_links.txt
+-rw-r--r--   0 danirus    (501) staff       (20)       92 2022-10-26 12:44:56.000000 django-comments-xtd-2.9.9/django_comments_xtd.egg-info/requires.txt
+-rw-r--r--   0 danirus    (501) staff       (20)       20 2022-10-26 12:44:56.000000 django-comments-xtd-2.9.9/django_comments_xtd.egg-info/top_level.txt
+-rw-r--r--   0 danirus    (501) staff       (20)        1 2017-08-07 19:36:48.000000 django-comments-xtd-2.9.9/django_comments_xtd.egg-info/zip-safe
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.028460 django-comments-xtd-2.9.9/docs/
+-rw-r--r--   0 danirus    (501) staff       (20)     4642 2014-01-09 10:13:11.000000 django-comments-xtd-2.9.9/docs/Makefile
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.029047 django-comments-xtd-2.9.9/docs/__pycache__/
+-rw-r--r--   0 danirus    (501) staff       (20)      597 2017-04-05 15:08:05.000000 django-comments-xtd-2.9.9/docs/__pycache__/extensions.cpython-35.pyc
+-rw-r--r--   0 danirus    (501) staff       (20)      547 2017-05-17 10:40:57.000000 django-comments-xtd-2.9.9/docs/__pycache__/extensions.cpython-36.pyc
+-rw-r--r--   0 danirus    (501) staff       (20)      567 2021-02-28 14:32:10.000000 django-comments-xtd-2.9.9/docs/__pycache__/extensions.cpython-38.pyc
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.029186 django-comments-xtd-2.9.9/docs/_build/
+-rw-r--r--   0 danirus    (501) staff       (20)      230 2020-10-11 11:29:49.000000 django-comments-xtd-2.9.9/docs/_build/.buildinfo
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.040062 django-comments-xtd-2.9.9/docs/_build/.doctrees/
+-rw-r--r--   0 danirus    (501) staff       (20)  3539313 2020-10-11 11:29:49.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/environment.pickle
+-rw-r--r--   0 danirus    (501) staff       (20)    44436 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/example.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    22889 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/extending.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    19183 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/i18n.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)   103243 2020-10-11 11:29:49.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/index.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    29170 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/javascript.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    51747 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/logic.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    11764 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/migrating.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    27187 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/quickstart.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    60072 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/settings.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    50287 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/templates.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    59838 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/templatetags.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)   194305 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/tutorial.doctree
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.041094 django-comments-xtd-2.9.9/docs/_build/.doctrees/usecases/
+-rw-r--r--   0 danirus    (501) staff       (20)    62853 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/usecases/change-user-image-or-avatar.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    39079 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/usecases/only-signed-in-can-comment.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)     3377 2020-10-11 11:16:50.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/usecases.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    76888 2020-10-11 11:16:51.000000 django-comments-xtd-2.9.9/docs/_build/.doctrees/webapi.doctree
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.050087 django-comments-xtd-2.9.9/docs/_build/doctrees/
+-rw-r--r--   0 danirus    (501) staff       (20)  2475254 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 danirus    (501) staff       (20)    40304 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/example.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    22889 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/extending.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    19045 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/i18n.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    16005 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    28475 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/javascript.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    48493 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/logic.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    11764 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/migrating.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    27187 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/quickstart.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    54490 2020-06-06 16:11:54.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/settings.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    50229 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/templates.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    56642 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/templatetags.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)   190001 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/tutorial.doctree
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.050587 django-comments-xtd-2.9.9/docs/_build/doctrees/usecases/
+-rw-r--r--   0 danirus    (501) staff       (20)     8065 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/usecases/only-signed-in-can-comment.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)     3419 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/usecases.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    32780 2020-06-06 16:11:55.000000 django-comments-xtd-2.9.9/docs/_build/doctrees/webapi.doctree
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.055688 django-comments-xtd-2.9.9/docs/_build/html/
+-rw-r--r--   0 danirus    (501) staff       (20)      230 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/.buildinfo
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.066771 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/
+-rw-r--r--   0 danirus    (501) staff       (20)  3541715 2020-10-11 11:36:25.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/environment.pickle
+-rw-r--r--   0 danirus    (501) staff       (20)    44436 2020-10-11 11:35:47.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/example.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    22889 2020-10-11 11:35:47.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/extending.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    19183 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/i18n.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)   109616 2020-10-11 11:36:25.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/index.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    29170 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/javascript.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    51747 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/logic.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    11764 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/migrating.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    27187 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/quickstart.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    74148 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/settings.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    50287 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/templates.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    59838 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/templatetags.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)   194305 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/tutorial.doctree
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.067768 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/usecases/
+-rw-r--r--   0 danirus    (501) staff       (20)    62853 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/usecases/change-user-image-or-avatar.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    39079 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/usecases/only-signed-in-can-comment.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)     3377 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/usecases.doctree
+-rw-r--r--   0 danirus    (501) staff       (20)    76888 2020-10-11 11:35:48.000000 django-comments-xtd-2.9.9/docs/_build/html/.doctrees/webapi.doctree
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.071162 django-comments-xtd-2.9.9/docs/_build/html/_images/
+-rw-r--r--   0 danirus    (501) staff       (20)    80426 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/comments-enabled.png
+-rw-r--r--   0 danirus    (501) staff       (20)   183596 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/cover.png
+-rw-r--r--   0 danirus    (501) staff       (20)    53244 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/extend-comments-app.png
+-rw-r--r--   0 danirus    (501) staff       (20)    32110 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/feedback-buttons.png
+-rw-r--r--   0 danirus    (501) staff       (20)    75480 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/feedback-users.png
+-rw-r--r--   0 danirus    (501) staff       (20)    44521 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/flag-counter.png
+-rw-r--r--   0 danirus    (501) staff       (20)    22281 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/markdown-comment.png
+-rw-r--r--   0 danirus    (501) staff       (20)    26498 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/markdown-input.png
+-rw-r--r--   0 danirus    (501) staff       (20)    46276 2020-07-05 07:40:16.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/only-users-can-post.png
+-rw-r--r--   0 danirus    (501) staff       (20)    73259 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/reply-link.png
+-rw-r--r--   0 danirus    (501) staff       (20)    96365 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/_build/html/_images/update-comment-tree.png
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.074820 django-comments-xtd-2.9.9/docs/_build/html/_sources/
+-rw-r--r--   0 danirus    (501) staff       (20)     7422 2020-09-29 10:03:46.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/example.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     5024 2018-08-12 10:16:22.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/extending.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     3810 2020-06-08 12:15:51.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/i18n.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)    17953 2020-10-11 11:36:25.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     7538 2020-10-11 11:35:47.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/javascript.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     9648 2020-07-28 17:33:27.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/logic.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     2709 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/migrating.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     4012 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/quickstart.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)    12893 2020-10-11 11:35:47.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/settings.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     7349 2020-07-28 17:33:27.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/templates.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     9658 2020-07-05 10:39:13.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/templatetags.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)    44847 2020-10-11 11:35:47.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/tutorial.rst.txt
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.075266 django-comments-xtd-2.9.9/docs/_build/html/_sources/usecases/
+-rw-r--r--   0 danirus    (501) staff       (20)    12965 2020-08-08 12:51:49.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/usecases/change-user-image-or-avatar.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)     9043 2020-07-05 07:34:30.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/usecases/only-signed-in-can-comment.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)      238 2020-08-09 07:01:34.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/usecases.rst.txt
+-rw-r--r--   0 danirus    (501) staff       (20)    19433 2020-07-28 17:33:27.000000 django-comments-xtd-2.9.9/docs/_build/html/_sources/webapi.rst.txt
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.078893 django-comments-xtd-2.9.9/docs/_build/html/_static/
+-rw-r--r--   0 danirus    (501) staff       (20)    12261 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.079151 django-comments-xtd-2.9.9/docs/_build/html/_static/css/
+-rw-r--r--   0 danirus    (501) staff       (20)     3391 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/css/badge_only.css
+-rw-r--r--   0 danirus    (501) staff       (20)   118340 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 danirus    (501) staff       (20)     9270 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 danirus    (501) staff       (20)      329 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 danirus    (501) staff       (20)      286 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/file.png
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.089638 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/
+-rw-r--r--   0 danirus    (501) staff       (20)   109948 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Inconsolata-Bold.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)    96964 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Inconsolata-Regular.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)    63184 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Inconsolata.ttf
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.112215 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/
+-rw-r--r--   0 danirus    (501) staff       (20)   256056 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bold.eot
+-rw-r--r--   0 danirus    (501) staff       (20)   600856 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bold.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)   309728 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bold.woff
+-rw-r--r--   0 danirus    (501) staff       (20)   184912 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bold.woff2
+-rw-r--r--   0 danirus    (501) staff       (20)   266158 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bolditalic.eot
+-rw-r--r--   0 danirus    (501) staff       (20)   622572 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bolditalic.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)   323344 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bolditalic.woff
+-rw-r--r--   0 danirus    (501) staff       (20)   193308 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bolditalic.woff2
+-rw-r--r--   0 danirus    (501) staff       (20)   268604 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-italic.eot
+-rw-r--r--   0 danirus    (501) staff       (20)   639388 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-italic.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)   328412 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-italic.woff
+-rw-r--r--   0 danirus    (501) staff       (20)   195704 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-italic.woff2
+-rw-r--r--   0 danirus    (501) staff       (20)   253461 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-regular.eot
+-rw-r--r--   0 danirus    (501) staff       (20)   607720 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-regular.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)   309192 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-regular.woff
+-rw-r--r--   0 danirus    (501) staff       (20)   182708 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-regular.woff2
+-rw-r--r--   0 danirus    (501) staff       (20)   656544 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato-Bold.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)   656568 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato-Regular.ttf
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.116222 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/
+-rw-r--r--   0 danirus    (501) staff       (20)    79520 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
+-rw-r--r--   0 danirus    (501) staff       (20)   170616 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)    87624 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
+-rw-r--r--   0 danirus    (501) staff       (20)    67312 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
+-rw-r--r--   0 danirus    (501) staff       (20)    78331 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
+-rw-r--r--   0 danirus    (501) staff       (20)   169064 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)    86288 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
+-rw-r--r--   0 danirus    (501) staff       (20)    66444 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
+-rw-r--r--   0 danirus    (501) staff       (20)   170616 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab-Bold.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)   169064 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab-Regular.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)   165742 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 danirus    (501) staff       (20)   444379 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 danirus    (501) staff       (20)   165548 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 danirus    (501) staff       (20)    98024 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 danirus    (501) staff       (20)    77160 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 danirus    (501) staff       (20)   280364 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/jquery-3.4.1.js
+-rw-r--r--   0 danirus    (501) staff       (20)    88145 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.117009 django-comments-xtd-2.9.9/docs/_build/html/_static/js/
+-rw-r--r--   0 danirus    (501) staff       (20)    15414 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/js/modernizr.min.js
+-rw-r--r--   0 danirus    (501) staff       (20)     4414 2019-12-25 12:07:15.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 danirus    (501) staff       (20)    10847 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 danirus    (501) staff       (20)       90 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/minus.png
+-rw-r--r--   0 danirus    (501) staff       (20)       90 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/plus.png
+-rw-r--r--   0 danirus    (501) staff       (20)     4395 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 danirus    (501) staff       (20)    16029 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 danirus    (501) staff       (20)    35168 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 danirus    (501) staff       (20)    12140 2019-12-25 12:06:53.000000 django-comments-xtd-2.9.9/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 danirus    (501) staff       (20)    19720 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/example.html
+-rw-r--r--   0 danirus    (501) staff       (20)    22841 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/extending.html
+-rw-r--r--   0 danirus    (501) staff       (20)    23005 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/genindex.html
+-rw-r--r--   0 danirus    (501) staff       (20)    13945 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/i18n.html
+-rw-r--r--   0 danirus    (501) staff       (20)    40911 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/index.html
+-rw-r--r--   0 danirus    (501) staff       (20)    19814 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/javascript.html
+-rw-r--r--   0 danirus    (501) staff       (20)    25434 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/logic.html
+-rw-r--r--   0 danirus    (501) staff       (20)    12353 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/migrating.html
+-rw-r--r--   0 danirus    (501) staff       (20)     1253 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/objects.inv
+-rw-r--r--   0 danirus    (501) staff       (20)     5772 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/py-modindex.html
+-rw-r--r--   0 danirus    (501) staff       (20)    15021 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/quickstart.html
+-rw-r--r--   0 danirus    (501) staff       (20)     5602 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/search.html
+-rw-r--r--   0 danirus    (501) staff       (20)    30022 2020-10-11 11:36:26.000000 django-comments-xtd-2.9.9/docs/_build/html/searchindex.js
+-rw-r--r--   0 danirus    (501) staff       (20)    42775 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/settings.html
+-rw-r--r--   0 danirus    (501) staff       (20)    25812 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/templates.html
+-rw-r--r--   0 danirus    (501) staff       (20)    37487 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/templatetags.html
+-rw-r--r--   0 danirus    (501) staff       (20)   110167 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/tutorial.html
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.117725 django-comments-xtd-2.9.9/docs/_build/html/usecases/
+-rw-r--r--   0 danirus    (501) staff       (20)    37849 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/usecases/change-user-image-or-avatar.html
+-rw-r--r--   0 danirus    (501) staff       (20)    28677 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/usecases/only-signed-in-can-comment.html
+-rw-r--r--   0 danirus    (501) staff       (20)     6828 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/usecases.html
+-rw-r--r--   0 danirus    (501) staff       (20)    49376 2020-10-11 11:35:49.000000 django-comments-xtd-2.9.9/docs/_build/html/webapi.html
+-rw-r--r--   0 danirus    (501) staff       (20)     7777 2022-10-26 12:38:35.000000 django-comments-xtd-2.9.9/docs/conf.py
+-rw-r--r--   0 danirus    (501) staff       (20)     7422 2020-09-29 10:03:46.000000 django-comments-xtd-2.9.9/docs/example.rst
+-rw-r--r--   0 danirus    (501) staff       (20)     5022 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/docs/extending.rst
+-rw-r--r--   0 danirus    (501) staff       (20)      621 2021-02-28 14:28:58.000000 django-comments-xtd-2.9.9/docs/extensions.py
+-rw-r--r--   0 danirus    (501) staff       (20)     3885 2021-02-28 10:08:44.000000 django-comments-xtd-2.9.9/docs/i18n.rst
+-rw-r--r--   0 danirus    (501) staff       (20)        0 2017-06-04 11:43:16.000000 django-comments-xtd-2.9.9/docs/i18n.rst~
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.122950 django-comments-xtd-2.9.9/docs/images/
+-rw-r--r--   0 danirus    (501) staff       (20)    80426 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/images/comments-enabled.png
+-rw-r--r--   0 danirus    (501) staff       (20)   183596 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/images/cover.png
+-rw-r--r--   0 danirus    (501) staff       (20)    53244 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/images/extend-comments-app.png
+-rw-r--r--   0 danirus    (501) staff       (20)    32110 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/images/feedback-buttons.png
+-rw-r--r--   0 danirus    (501) staff       (20)    75480 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/images/feedback-users.png
+-rw-r--r--   0 danirus    (501) staff       (20)    44521 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/images/flag-counter.png
+-rw-r--r--   0 danirus    (501) staff       (20)    22281 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/images/markdown-comment.png
+-rw-r--r--   0 danirus    (501) staff       (20)    26498 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/images/markdown-input.png
+-rw-r--r--   0 danirus    (501) staff       (20)    46276 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.9/docs/images/only-users-can-post.png
+-rw-r--r--   0 danirus    (501) staff       (20)    97842 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/images/preview-comment.png
+-rw-r--r--   0 danirus    (501) staff       (20)    73259 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/images/reply-link.png
+-rw-r--r--   0 danirus    (501) staff       (20)    96365 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/images/update-comment-tree.png
+-rw-r--r--   0 danirus    (501) staff       (20)    24643 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/docs/index.rst
+-rw-r--r--   0 danirus    (501) staff       (20)     7533 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/docs/javascript.rst
+-rw-r--r--   0 danirus    (501) staff       (20)        0 2017-05-19 04:48:08.000000 django-comments-xtd-2.9.9/docs/javascript.rst~
+-rw-r--r--   0 danirus    (501) staff       (20)     9648 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.9/docs/logic.rst
+-rw-r--r--   0 danirus    (501) staff       (20)     4537 2014-01-09 10:13:11.000000 django-comments-xtd-2.9.9/docs/make.bat
+-rw-r--r--   0 danirus    (501) staff       (20)     1218 2021-06-06 15:06:10.000000 django-comments-xtd-2.9.9/docs/management.rst
+-rw-r--r--   0 danirus    (501) staff       (20)     2709 2017-06-09 21:43:55.000000 django-comments-xtd-2.9.9/docs/migrating.rst
+-rw-r--r--   0 danirus    (501) staff       (20)      459 2017-06-07 05:48:01.000000 django-comments-xtd-2.9.9/docs/migrating.rst~
+-rw-r--r--   0 danirus    (501) staff       (20)     4012 2018-11-29 21:42:24.000000 django-comments-xtd-2.9.9/docs/quickstart.rst
+-rw-r--r--   0 danirus    (501) staff       (20)       14 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/docs/requirements.txt
+-rw-r--r--   0 danirus    (501) staff       (20)    10595 2022-07-08 07:47:46.000000 django-comments-xtd-2.9.9/docs/settings.rst
+-rw-r--r--   0 danirus    (501) staff       (20)     7349 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.9/docs/templates.rst
+-rw-r--r--   0 danirus    (501) staff       (20)     9658 2022-01-04 19:18:25.000000 django-comments-xtd-2.9.9/docs/templatetags.rst
+-rw-r--r--   0 danirus    (501) staff       (20)    45005 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/docs/tutorial.rst
+drwxr-xr-x   0 danirus    (501) staff       (20)        0 2022-10-26 12:44:57.123532 django-comments-xtd-2.9.9/docs/usecases/
+-rw-r--r--   0 danirus    (501) staff       (20)    12965 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.9/docs/usecases/change-user-image-or-avatar.rst
+-rw-r--r--   0 danirus    (501) staff       (20)     9043 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.9/docs/usecases/only-signed-in-can-comment.rst
+-rw-r--r--   0 danirus    (501) staff       (20)      238 2020-08-14 16:03:37.000000 django-comments-xtd-2.9.9/docs/usecases.rst
+-rw-r--r--   0 danirus    (501) staff       (20)    19504 2021-02-16 14:04:32.000000 django-comments-xtd-2.9.9/docs/webapi.rst
+-rw-r--r--   0 danirus    (501) staff       (20)        0 2017-05-21 05:59:07.000000 django-comments-xtd-2.9.9/docs/webapi.rst~
+-rw-r--r--   0 danirus    (501) staff       (20)      779 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/package.json
+-rw-r--r--   0 danirus    (501) staff       (20)      178 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/pyproject.toml
+-rw-r--r--   0 danirus    (501) staff       (20)      131 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/requirements.pip
+-rw-r--r--   0 danirus    (501) staff       (20)       80 2022-10-26 12:38:35.000000 django-comments-xtd-2.9.9/requirements_tests.pip
+-rw-r--r--   0 danirus    (501) staff       (20)       38 2022-10-26 12:44:57.124001 django-comments-xtd-2.9.9/setup.cfg
+-rw-r--r--   0 danirus    (501) staff       (20)     1819 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/setup.py
+-rw-r--r--   0 danirus    (501) staff       (20)     1540 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/tox.ini
+-rw-r--r--   0 danirus    (501) staff       (20)     1026 2022-10-26 12:40:38.000000 django-comments-xtd-2.9.9/webpack.config.js
```

### Comparing `django-comments-xtd-2.9.8/.coverage` & `django-comments-xtd-2.9.9/.coverage`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/AUTHORS` & `django-comments-xtd-2.9.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/CHANGELOG.md` & `django-comments-xtd-2.9.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Change Log
 
+## [2.9.9] - 2022-10-26
+
+ * Extends compatibility to django-rest-framework v3.14.
+
 ## [2.9.8] - 2022-09-18
 
  * Fixes [issue 377](https://github.com/danirus/django-comments-xtd/issues/377): content_object is missing in followup notification. View `notify_comment_followers` has been updated to include `content_object` in the context of templates it uses: `email_followup_comment.txt` and `email_followup_comment.html`.
  * Update translation files to the latest strings found in templates. Next step is to include appropriate translations. See [PR #379](https://github.com/danirus/django-comments-xtd/pull/379).
 
 ## [2.9.7] - 2022-07-08
```

### Comparing `django-comments-xtd-2.9.8/LICENSE` & `django-comments-xtd-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/PKG-INFO` & `django-comments-xtd-2.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-comments-xtd
-Version: 2.9.8
+Version: 2.9.9
 Summary: Django Comments Framework extension app with thread support, follow up notifications and email confirmations.
 Home-page: http://pypi.python.org/pypi/django-comments-xtd
 Author: Daniela Rus Morales
 Author-email: danirus@eml.cc
 Maintainer: Daniela Rus Morales
 Maintainer-email: danirus@eml.cc
 License: MIT
```

### Comparing `django-comments-xtd-2.9.8/README.rst` & `django-comments-xtd-2.9.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 #. Registered users can like/dislike comments and can suggest comments removal.
 #. Template tags to list/render the last N comments posted to any given list of app.model pairs.
 #. Emails sent through threads (can be disable to allow other solutions, like a Celery app).
 #. Fully functional JavaScript plugin using ReactJS, jQuery, Bootstrap, Remarkable and MD5.
 
 Example sites and tests work under officially Django `supported versions <https://www.djangoproject.com/download/#supported-versions>`_:
 
-* Django 3.1, 3.0, 2.2
-* Python 3.8, 3.7, 3.6
+* Django 4.1, 4.0, 3.2
+* Python 3.10, 3.9, 3.8
 
 Additional Dependencies:
 
 * django-contrib-comments >=1.8
-* djangorestframework >=3.12
+* djangorestframework >=3.12,<3.15
 
 Checkout the Docker image `danirus/django-comments-xtd-demo <https://hub.docker.com/r/danirus/django-comments-xtd-demo/>`_.
 
 `Read The Docs <http://readthedocs.org/docs/django-comments-xtd/>`_.
```

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/__init__.py` & `django-comments-xtd-2.9.9/django_comments_xtd/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def get_form():
     from django_comments_xtd.conf import settings
     return import_string(settings.COMMENTS_XTD_FORM_CLASS)
 
 
-VERSION = (2, 9, 8, 'f', 0)  # following PEP 440
+VERSION = (2, 9, 9, 'f', 0)  # following PEP 440
 
 
 def get_version():
     version = '%s.%s.%s' % (VERSION[0], VERSION[1], VERSION[2])
     if VERSION[3] != 'f':
         version = '%s%s%s' % (version, VERSION[3], VERSION[4])
     return version
```

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/admin.py` & `django-comments-xtd-2.9.9/django_comments_xtd/admin.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/api/frontend.py` & `django-comments-xtd-2.9.9/django_comments_xtd/api/frontend.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/api/serializers.py` & `django-comments-xtd-2.9.9/django_comments_xtd/api/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,22 +87,22 @@
         if ctype is None or object_pk is None:
             return serializers.ValidationError("Missing content_type or "
                                                "object_pk field.")
         try:
             model = apps.get_model(*ctype.split(".", 1))
             target = model._default_manager.get(pk=object_pk)
             whocan = get_app_model_options(content_type=ctype)['who_can_post']
-        except (AttributeError, TypeError, LookupError):
+        except (AttributeError, TypeError, LookupError, ValueError):
             raise serializers.ValidationError("Invalid content_type value: %r"
                                               % escape(ctype))
         except model.DoesNotExist:
             raise serializers.ValidationError(
                 "No object matching content-type %r and object PK %r exists."
                 % (escape(ctype), escape(object_pk)))
-        except (ValueError, serializers.ValidationError) as e:
+        except (serializers.ValidationError) as e:
             raise serializers.ValidationError(
                 "Attempting to get content-type %r and object PK %r exists "
                 "raised %s" % (escape(ctype), escape(object_pk),
                                e.__class__.__name__))
         else:
             if whocan == "users" and not self.request.user.is_authenticated:
                 raise serializers.ValidationError("User not authenticated")
```

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/api/urls.py` & `django-comments-xtd-2.9.9/django_comments_xtd/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/api/views.py` & `django-comments-xtd-2.9.9/django_comments_xtd/api/views.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/apps.py` & `django-comments-xtd-2.9.9/django_comments_xtd/apps.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/compat.py` & `django-comments-xtd-2.9.9/django_comments_xtd/compat.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/conf/__init__.py` & `django-comments-xtd-2.9.9/django_comments_xtd/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/conf/defaults.py` & `django-comments-xtd-2.9.9/django_comments_xtd/conf/defaults.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/forms.py` & `django-comments-xtd-2.9.9/django_comments_xtd/forms.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/de/LC_MESSAGES/django.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/de/LC_MESSAGES/django.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/de/LC_MESSAGES/djangojs.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/de/LC_MESSAGES/djangojs.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/es/LC_MESSAGES/django.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/es/LC_MESSAGES/django.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/es/LC_MESSAGES/djangojs.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/es/LC_MESSAGES/djangojs.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/fi/LC_MESSAGES/django.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/fi/LC_MESSAGES/django.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/fi/LC_MESSAGES/djangojs.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/fi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/fi/LC_MESSAGES/djangojs.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/fi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/fr/LC_MESSAGES/django.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/fr/LC_MESSAGES/django.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/fr/LC_MESSAGES/djangojs.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/fr/LC_MESSAGES/djangojs.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/it/LC_MESSAGES/django.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/it/LC_MESSAGES/django.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/it/LC_MESSAGES/djangojs.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/it/LC_MESSAGES/djangojs.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/nl/LC_MESSAGES/django.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/nl/LC_MESSAGES/django.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/nl/LC_MESSAGES/djangojs.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/nl/LC_MESSAGES/djangojs.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/no/LC_MESSAGES/django.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/no/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/no/LC_MESSAGES/django.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/no/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/no/LC_MESSAGES/djangojs.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/no/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/no/LC_MESSAGES/djangojs.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/no/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/ru/LC_MESSAGES/django.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/ru/LC_MESSAGES/django.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/ru/LC_MESSAGES/djangojs.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/ru/LC_MESSAGES/djangojs.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/django.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/djangojs.mo` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `django-comments-xtd-2.9.9/django_comments_xtd/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/management/commands/initialize_nested_count.py` & `django-comments-xtd-2.9.9/django_comments_xtd/management/commands/initialize_nested_count.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/management/commands/populate_xtdcomments.py` & `django-comments-xtd-2.9.9/django_comments_xtd/management/commands/populate_xtdcomments.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/migrations/0001_initial.py` & `django-comments-xtd-2.9.9/django_comments_xtd/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/migrations/0002_blacklisteddomain.py` & `django-comments-xtd-2.9.9/django_comments_xtd/migrations/0002_blacklisteddomain.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/migrations/0004_auto_20170221_1510.py` & `django-comments-xtd-2.9.9/django_comments_xtd/migrations/0004_auto_20170221_1510.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/migrations/0008_auto_20200920_2037.py` & `django-comments-xtd-2.9.9/django_comments_xtd/migrations/0008_auto_20200920_2037.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/models.py` & `django-comments-xtd-2.9.9/django_comments_xtd/models.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/moderation.py` & `django-comments-xtd-2.9.9/django_comments_xtd/moderation.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/signals.py` & `django-comments-xtd-2.9.9/django_comments_xtd/signals.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/signed.py` & `django-comments-xtd-2.9.9/django_comments_xtd/signed.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/css/_bootswatch.scss` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/css/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/css/_variables.scss` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/css/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/css/bootstrap.css` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/css/bootstrap.min.css` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.eot` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.svg` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.ttf` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.woff` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.woff2` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/img/64x64.svg` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/img/64x64.svg`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.8.js` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1496,8 +1496,8 @@
                     className: "media-list"
                 }, i)))
             }
         }]) && H(t.prototype, r), n && H(t, n), s
     }(a.a.Component);
     s.a.render(a.a.createElement($, Object.assign(window.comments_props, window.comments_props_override)), document.getElementById("comments"))
 }]);
-//# sourceMappingURL=plugin-2.9.8.js.map
+//# sourceMappingURL=plugin-2.9.9.js.map
```

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.8.js.map` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.9.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'file'": "'plugin-2.9.9.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "plugin-2.9.8.js",
+    "file": "plugin-2.9.9.js",
     "mappings": "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",
     "names": [
         "modules",
         "webpackJsonpCallback",
         "data",
         "moduleId",
         "chunkId",
```

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/src/comment.jsx` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/src/comment.jsx`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/src/commentbox.jsx` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/src/commentbox.jsx`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/src/commentform.jsx` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/src/commentform.jsx`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/src/lib.js` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/src/lib.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.8.js` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1636,8 +1636,8 @@
                 return n.inlineMode = !0, this.core.process(n), n.tokens
             }, Me.prototype.renderInline = function(e, t) {
                 return t = t || {}, this.renderer.render(this.parseInline(e, t), this.options, t)
             }
         }
     }
 ]);
-//# sourceMappingURL=vendor~plugin-2.9.8.js.map
+//# sourceMappingURL=vendor~plugin-2.9.9.js.map
```

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.8.js.map` & `django-comments-xtd-2.9.9/django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.9.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'file'": "'vendor~plugin-2.9.9.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "vendor~plugin-2.9.8.js",
+    "file": "vendor~plugin-2.9.9.js",
     "mappings": "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IAAM,EAEnDZ,EAAMgB,GAAOL,EAAM1E,IAAI/D,WAAW8H,KAASc,GAAUd,IAqB5D,OApBIA,GAAOgB,IAAOyN,GAAW,IAC7B/H,EAAQ1G,EAAMY,IAED,EAEX6N,EAAWC,GAAY,GAKN,MAHjBF,EAAWxO,EAAMgB,EAAML,EAAM1E,IAAI/D,WAAW8H,IAAQ,IAGd,KAAbwO,IAAqBC,GAAW,GACxC,KAAbF,GAAkC,KAAbA,IAAqBG,GAAY,GAE3C,KAAX5N,IAEEuN,GAAWE,KAAaE,GAAW,GACnCJ,GAAWG,KAAaE,GAAY,KAIrC,CACLD,SAAUA,EACVC,UAAWA,EACXC,OAAQjI,GA3XZ,qCACGvM,MAAM,IAAIvD,SAAQ,SAASmC,GAAMqV,GAAQrV,EAAGb,WAAW,IAAM,KAqehE,IAAI0W,GAAc,8CAyDlB,IAAIC,GAAgB,8CA2UpB,IAAIC,GAAc,CAChB,OACA,MACA,aACA,MACA,OACA,QACA,OACA,MACA,MACA,OACA,OACA,MACA,OACA,MACA,OACA,MACA,MACA,KACA,SACA,OACA,OACA,QACA,MACA,OACA,KACA,OACA,OACA,MACA,OACA,YACA,WACA,YACA,WACA,OACA,SACA,MACA,OACA,QACA,OACA,UACA,OACA,MACA,KACA,MACA,OACA,kBACA,MACA,OACA,OACA,UACA,UACA,QACA,QACA,MACA,OACA,MACA,OACA,YACA,aACA,MACA,MACA,SACA,OACA,cACA,SACA,MACA,KACA,MACA,QACA,KACA,MACA,OACA,cACA,cACA,eACA,OACA,UACA,UACA,YACA,MACA,MACA,MACA,MACA,aACA,KACA,UACA,UACA,OACA,SACA,SACA,mBACA,0BACA,UACA,MACA,kBACA,qBACA,MACA,MACA,OACA,WACA,OACA,SACA,OACA,KACA,MACA,eACA,QACA,MACA,OACA,MACA,MACA,OACA,OACA,OACA,MACA,MACA,UACA,SACA,QACA,SACA,OACA,SACA,UACA,MACA,UACA,QACA,SACA,MACA,QACA,MACA,OACA,YACA,WACA,QACA,OACA,QACA,MACA,WACA,MACA,QACA,OACA,a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",
     "names": [
         "window",
         "push",
         "3",
         "module",
         "__webpack_exports__",
```

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/delete.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/delete.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/flag.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/flag.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/form.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/form.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/list.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/list.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/posted.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/posted.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/comments/preview.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/comments/preview.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/comment.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/comment.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/comment_list.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/comment_list.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/comment_tree.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/comment_tree.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/dislike.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/dislike.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/email_confirmation_request.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/email_confirmation_request.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/email_confirmation_request.txt` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/email_confirmation_request.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/email_followup_comment.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/email_followup_comment.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/email_followup_comment.txt` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/email_followup_comment.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/like.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/like.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/moderated.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/moderated.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/django_comments_xtd/reply.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/django_comments_xtd/reply.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templates/includes/django_comments_xtd/user_feedback.html` & `django-comments-xtd-2.9.9/django_comments_xtd/templates/includes/django_comments_xtd/user_feedback.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/templatetags/comments_xtd.py` & `django-comments-xtd-2.9.9/django_comments_xtd/templatetags/comments_xtd.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/__init__.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/apiauth.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/apiauth.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/migrations/0001_initial.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/migrations/0002_auto_20170523_1624.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/migrations/0002_auto_20170523_1624.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/migrations/0003_uuiddiary.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/migrations/0003_uuiddiary.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/models.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/settings.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/test_api_views.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/test_api_views.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/test_cmd_initialize_nested_count.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/test_cmd_initialize_nested_count.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/test_forms.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/test_frontend.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/test_frontend.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/test_get_version.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/test_get_version.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/test_models.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/test_moderation.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/test_moderation.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/test_serializers.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/test_templatetags.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/test_views.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/tests/urls.py` & `django-comments-xtd-2.9.9/django_comments_xtd/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/urls.py` & `django-comments-xtd-2.9.9/django_comments_xtd/urls.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/utils.py` & `django-comments-xtd-2.9.9/django_comments_xtd/utils.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd/views.py` & `django-comments-xtd-2.9.9/django_comments_xtd/views.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd.egg-info/PKG-INFO` & `django-comments-xtd-2.9.9/django_comments_xtd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-comments-xtd
-Version: 2.9.8
+Version: 2.9.9
 Summary: Django Comments Framework extension app with thread support, follow up notifications and email confirmations.
 Home-page: http://pypi.python.org/pypi/django-comments-xtd
 Author: Daniela Rus Morales
 Author-email: danirus@eml.cc
 Maintainer: Daniela Rus Morales
 Maintainer-email: danirus@eml.cc
 License: MIT
```

### Comparing `django-comments-xtd-2.9.8/django_comments_xtd.egg-info/SOURCES.txt` & `django-comments-xtd-2.9.9/django_comments_xtd.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -92,18 +92,18 @@
 django_comments_xtd/static/django_comments_xtd/css/bootstrap.min.css
 django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.eot
 django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.svg
 django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.ttf
 django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.woff
 django_comments_xtd/static/django_comments_xtd/fonts/glyphicons-halflings-regular.woff2
 django_comments_xtd/static/django_comments_xtd/img/64x64.svg
-django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.8.js
-django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.8.js.map
-django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.8.js
-django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.8.js.map
+django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.9.js
+django_comments_xtd/static/django_comments_xtd/js/plugin-2.9.9.js.map
+django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.9.js
+django_comments_xtd/static/django_comments_xtd/js/vendor~plugin-2.9.9.js.map
 django_comments_xtd/static/django_comments_xtd/js/src/comment.jsx
 django_comments_xtd/static/django_comments_xtd/js/src/commentbox.jsx
 django_comments_xtd/static/django_comments_xtd/js/src/commentform.jsx
 django_comments_xtd/static/django_comments_xtd/js/src/index.js
 django_comments_xtd/static/django_comments_xtd/js/src/lib.js
 django_comments_xtd/templates/404.html
 django_comments_xtd/templates/comments/comment_notification_email.txt
```

### Comparing `django-comments-xtd-2.9.8/docs/Makefile` & `django-comments-xtd-2.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/__pycache__/extensions.cpython-35.pyc` & `django-comments-xtd-2.9.9/docs/__pycache__/extensions.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/__pycache__/extensions.cpython-36.pyc` & `django-comments-xtd-2.9.9/docs/__pycache__/extensions.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/__pycache__/extensions.cpython-38.pyc` & `django-comments-xtd-2.9.9/docs/__pycache__/extensions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/environment.pickle` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/example.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/example.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/extending.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/extending.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/i18n.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/i18n.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/index.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/javascript.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/javascript.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/logic.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/logic.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/migrating.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/migrating.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/quickstart.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/quickstart.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/settings.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/settings.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/templates.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/templates.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/templatetags.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/templatetags.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/tutorial.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/tutorial.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/usecases/change-user-image-or-avatar.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/usecases/change-user-image-or-avatar.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/usecases/only-signed-in-can-comment.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/usecases/only-signed-in-can-comment.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/usecases.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/usecases.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/.doctrees/webapi.doctree` & `django-comments-xtd-2.9.9/docs/_build/.doctrees/webapi.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/environment.pickle` & `django-comments-xtd-2.9.9/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/example.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/example.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/extending.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/extending.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/i18n.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/i18n.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/index.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/javascript.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/javascript.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/logic.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/logic.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/migrating.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/migrating.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/quickstart.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/quickstart.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/settings.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/settings.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/templates.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/templates.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/templatetags.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/templatetags.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/tutorial.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/tutorial.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/usecases/only-signed-in-can-comment.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/usecases/only-signed-in-can-comment.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/usecases.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/usecases.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/doctrees/webapi.doctree` & `django-comments-xtd-2.9.9/docs/_build/doctrees/webapi.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/environment.pickle` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/example.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/example.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/extending.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/extending.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/i18n.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/i18n.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/index.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/javascript.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/javascript.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/logic.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/logic.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/migrating.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/migrating.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/quickstart.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/quickstart.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/settings.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/settings.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/templates.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/templates.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/templatetags.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/templatetags.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/tutorial.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/tutorial.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/usecases/change-user-image-or-avatar.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/usecases/change-user-image-or-avatar.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/usecases/only-signed-in-can-comment.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/usecases/only-signed-in-can-comment.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/usecases.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/usecases.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/.doctrees/webapi.doctree` & `django-comments-xtd-2.9.9/docs/_build/html/.doctrees/webapi.doctree`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/comments-enabled.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/comments-enabled.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/cover.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/cover.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/extend-comments-app.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/extend-comments-app.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/feedback-buttons.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/feedback-buttons.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/feedback-users.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/feedback-users.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/flag-counter.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/flag-counter.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/markdown-comment.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/markdown-comment.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/markdown-input.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/markdown-input.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/only-users-can-post.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/only-users-can-post.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/reply-link.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/reply-link.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_images/update-comment-tree.png` & `django-comments-xtd-2.9.9/docs/_build/html/_images/update-comment-tree.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/example.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/example.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/extending.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/extending.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/i18n.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/i18n.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/index.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/javascript.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/javascript.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/logic.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/logic.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/migrating.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/migrating.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/quickstart.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/quickstart.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/settings.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/settings.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/templates.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/templates.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/templatetags.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/templatetags.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/tutorial.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/tutorial.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/usecases/change-user-image-or-avatar.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/usecases/change-user-image-or-avatar.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/usecases/only-signed-in-can-comment.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/usecases/only-signed-in-can-comment.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_sources/webapi.rst.txt` & `django-comments-xtd-2.9.9/docs/_build/html/_sources/webapi.rst.txt`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/basic.css` & `django-comments-xtd-2.9.9/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/css/badge_only.css` & `django-comments-xtd-2.9.9/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/css/theme.css` & `django-comments-xtd-2.9.9/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/doctools.js` & `django-comments-xtd-2.9.9/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Inconsolata-Bold.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Inconsolata-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Inconsolata-Regular.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Inconsolata.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Inconsolata.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bold.eot` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bold.eot`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bold.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bold.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bold.woff` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bold.woff2` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bolditalic.eot` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bolditalic.eot`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bolditalic.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bolditalic.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bolditalic.woff` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bolditalic.woff`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-bolditalic.woff2` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-bolditalic.woff2`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-italic.eot` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-italic.eot`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-italic.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-italic.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-italic.woff` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-italic.woff`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-italic.woff2` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-italic.woff2`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-regular.eot` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-regular.eot`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-regular.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-regular.woff` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-regular.woff`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato/lato-regular.woff2` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato/lato-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato-Bold.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/Lato-Regular.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab-Bold.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/RobotoSlab-Regular.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/RobotoSlab-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/fontawesome-webfont.eot` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/fontawesome-webfont.svg` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/fontawesome-webfont.ttf` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/fontawesome-webfont.woff` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/fonts/fontawesome-webfont.woff2` & `django-comments-xtd-2.9.9/docs/_build/html/_static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/jquery-3.4.1.js` & `django-comments-xtd-2.9.9/docs/_build/html/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/jquery.js` & `django-comments-xtd-2.9.9/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/js/modernizr.min.js` & `django-comments-xtd-2.9.9/docs/_build/html/_static/js/modernizr.min.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/js/theme.js` & `django-comments-xtd-2.9.9/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/language_data.js` & `django-comments-xtd-2.9.9/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/pygments.css` & `django-comments-xtd-2.9.9/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/searchtools.js` & `django-comments-xtd-2.9.9/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/underscore-1.3.1.js` & `django-comments-xtd-2.9.9/docs/_build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/_static/underscore.js` & `django-comments-xtd-2.9.9/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/example.html` & `django-comments-xtd-2.9.9/docs/_build/html/example.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/extending.html` & `django-comments-xtd-2.9.9/docs/_build/html/extending.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/genindex.html` & `django-comments-xtd-2.9.9/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/i18n.html` & `django-comments-xtd-2.9.9/docs/_build/html/i18n.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/index.html` & `django-comments-xtd-2.9.9/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/javascript.html` & `django-comments-xtd-2.9.9/docs/_build/html/javascript.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/logic.html` & `django-comments-xtd-2.9.9/docs/_build/html/logic.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/migrating.html` & `django-comments-xtd-2.9.9/docs/_build/html/migrating.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/objects.inv` & `django-comments-xtd-2.9.9/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/py-modindex.html` & `django-comments-xtd-2.9.9/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/quickstart.html` & `django-comments-xtd-2.9.9/docs/_build/html/quickstart.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/search.html` & `django-comments-xtd-2.9.9/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/searchindex.js` & `django-comments-xtd-2.9.9/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/settings.html` & `django-comments-xtd-2.9.9/docs/_build/html/settings.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/templates.html` & `django-comments-xtd-2.9.9/docs/_build/html/templates.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/templatetags.html` & `django-comments-xtd-2.9.9/docs/_build/html/templatetags.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/tutorial.html` & `django-comments-xtd-2.9.9/docs/_build/html/tutorial.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/usecases/change-user-image-or-avatar.html` & `django-comments-xtd-2.9.9/docs/_build/html/usecases/change-user-image-or-avatar.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/usecases/only-signed-in-can-comment.html` & `django-comments-xtd-2.9.9/docs/_build/html/usecases/only-signed-in-can-comment.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/usecases.html` & `django-comments-xtd-2.9.9/docs/_build/html/usecases.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/_build/html/webapi.html` & `django-comments-xtd-2.9.9/docs/_build/html/webapi.html`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/conf.py` & `django-comments-xtd-2.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/example.rst` & `django-comments-xtd-2.9.9/docs/example.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/extending.rst` & `django-comments-xtd-2.9.9/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/extensions.py` & `django-comments-xtd-2.9.9/docs/extensions.py`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/i18n.rst` & `django-comments-xtd-2.9.9/docs/i18n.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/comments-enabled.png` & `django-comments-xtd-2.9.9/docs/images/comments-enabled.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/cover.png` & `django-comments-xtd-2.9.9/docs/images/cover.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/extend-comments-app.png` & `django-comments-xtd-2.9.9/docs/images/extend-comments-app.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/feedback-buttons.png` & `django-comments-xtd-2.9.9/docs/images/feedback-buttons.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/feedback-users.png` & `django-comments-xtd-2.9.9/docs/images/feedback-users.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/flag-counter.png` & `django-comments-xtd-2.9.9/docs/images/flag-counter.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/markdown-comment.png` & `django-comments-xtd-2.9.9/docs/images/markdown-comment.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/markdown-input.png` & `django-comments-xtd-2.9.9/docs/images/markdown-input.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/only-users-can-post.png` & `django-comments-xtd-2.9.9/docs/images/only-users-can-post.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/preview-comment.png` & `django-comments-xtd-2.9.9/docs/images/preview-comment.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/reply-link.png` & `django-comments-xtd-2.9.9/docs/images/reply-link.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/images/update-comment-tree.png` & `django-comments-xtd-2.9.9/docs/images/update-comment-tree.png`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/index.rst` & `django-comments-xtd-2.9.9/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 A Django pluggable application that adds comments to your project. It extends
 the once official `Django Comments Framework
 <https://pypi.python.org/pypi/django-contrib-comments>`_.
 
 
 .. note::
 
-    This documentation represents the current version, v2.9.8, of
+    This documentation represents the current version, v2.9.9, of
     django-comments-xtd. For old versions of the documentation:
 
     * v2.8.5: https://django-comments-xtd.readthedocs.io/en/2.8.5/
     * v2.7.2: https://django-comments-xtd.readthedocs.io/en/2.7.2/
     * v2.6.2: https://django-comments-xtd.readthedocs.io/en/2.6.2/
     * v2.5.1: https://django-comments-xtd.readthedocs.io/en/2.5.1/
     * v2.4.3: https://django-comments-xtd.readthedocs.io/en/2.4.3/
@@ -92,20 +92,24 @@
    settings
    templates
    usecases
 
 Change Log
 ==========
 
+[2.9.9] - 2022-10-26
+--------------------
+
+   * Extends compatibility to django-rest-framework v3.14.
 
 [2.9.8] - 2022-09-18
 --------------------
 
    * Fixes `issue 377 <https://github.com/danirus/django-comments-xtd/issues/377>`_: content_object is missing in followup notification. View `notify_comment_followers` has been updated to include `content_object` in the context of templates it uses: `email_followup_comment.txt` and `email_followup_comment.html`.
- * Update translation files to the latest strings found in templates. Next step is to include appropriate translations. See `PR #379 <https://github.com/danirus/django-comments-xtd/pull/379>`_.
+   * Update translation files to the latest strings found in templates. Next step is to include appropriate translations. See `PR #379 <https://github.com/danirus/django-comments-xtd/pull/379>`_.
 
 [2.9.7] - 2022-07-08
 --------------------
 
    * Allows to customize the json object returned by the `get_commentbox_props` template tag. Define the new setting `COMMENTS_XTD_COMMENTBOX_CLASS` as the string path to the class that will return the JSON object. It defaults to the class `django_comments_xtd.api.frontend.CommentBoxDriver`.
 
 [2.9.5] - 2021-12-14
```

### Comparing `django-comments-xtd-2.9.8/docs/javascript.rst` & `django-comments-xtd-2.9.9/docs/javascript.rst`

 * *Files 2% similar despite different names*

```diff
@@ -129,16 +129,16 @@
 Webpack will put the bundles in the static directory of django-comments-xtd and
 Django will fetch them from there when rendering the article's detail page:
 
    .. code-block:: html+django
 
        {% block extra-js %}
        [...]
-       <script src="{% static 'django_comments_xtd/js/vendor~plugin-2.9.8.js' %}"></script>
-       <script src="{% static 'django_comments_xtd/js/plugin-2.9.8.js' %}"></script>
+       <script src="{% static 'django_comments_xtd/js/vendor~plugin-2.9.9.js' %}"></script>
+       <script src="{% static 'django_comments_xtd/js/plugin-2.9.9.js' %}"></script>
        {% endblock extra-js %}
 
 
 Code structure
 ==============
 
 Plugin sources live inside the **static** directory of django-comments-xtd:
@@ -146,21 +146,21 @@
    .. code-block:: shell
 
        $ cd ~/src/django-comments-xtd
        $ tree django_comments_xtd/static/django_comments_xtd/js
 
        django_comments_xtd/static/django_comments_xtd/js
        ├── src
-       │   ├── comment.jsx
-       │   ├── commentbox.jsx
-       │   ├── commentform.jsx
-       │   ├── index.js
-       │   └── lib.js
-       ├── vendor~plugin-2.9.8.js
-       └── plugin-2.9.8.js
+       │   ├── comment.jsx
+       │   ├── commentbox.jsx
+       │   ├── commentform.jsx
+       │   ├── index.js
+       │   └── lib.js
+       ├── vendor~plugin-2.9.9.js
+       └── plugin-2.9.9.js
 
        1 directory, 7 files
 
 The intial development was inspired by the `ReactJS Comment Box tutorial
 <https://github.com/facebook/react/blob/v15.3.2/docs/docs/tutorial.md>`_.
 Component names reflect those of the ReactJS tutorial.
```

### Comparing `django-comments-xtd-2.9.8/docs/logic.rst` & `django-comments-xtd-2.9.9/docs/logic.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/make.bat` & `django-comments-xtd-2.9.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/management.rst` & `django-comments-xtd-2.9.9/docs/management.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/migrating.rst` & `django-comments-xtd-2.9.9/docs/migrating.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/quickstart.rst` & `django-comments-xtd-2.9.9/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/settings.rst` & `django-comments-xtd-2.9.9/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/templates.rst` & `django-comments-xtd-2.9.9/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/templatetags.rst` & `django-comments-xtd-2.9.9/docs/templatetags.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/tutorial.rst` & `django-comments-xtd-2.9.9/docs/tutorial.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1132,16 +1132,16 @@
     <script
       src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"
       integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy"
       crossorigin="anonymous"></script>
     <script
       type="text/javascript"
       src="{% url 'javascript-catalog' %}"></script>
-    <script src="{% static 'django_comments_xtd/js/vendor~plugin-2.9.8.js' %}"></script>
-    <script src="{% static 'django_comments_xtd/js/plugin-2.9.8.js' %}"></script>
+    <script src="{% static 'django_comments_xtd/js/vendor~plugin-2.9.9.js' %}"></script>
+    <script src="{% static 'django_comments_xtd/js/plugin-2.9.9.js' %}"></script>
     <script>
     $(function() {
       $('[data-toggle="tooltip"]').tooltip({html: true});
     });
     </script>
     {% endblock %}
```

### Comparing `django-comments-xtd-2.9.8/docs/usecases/change-user-image-or-avatar.rst` & `django-comments-xtd-2.9.9/docs/usecases/change-user-image-or-avatar.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/usecases/only-signed-in-can-comment.rst` & `django-comments-xtd-2.9.9/docs/usecases/only-signed-in-can-comment.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/docs/webapi.rst` & `django-comments-xtd-2.9.9/docs/webapi.rst`

 * *Files identical despite different names*

### Comparing `django-comments-xtd-2.9.8/package.json` & `django-comments-xtd-2.9.9/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'2.9.9'"}*

```diff
@@ -23,9 +23,9 @@
     "main": "app.js",
     "name": "django-comments-xtd-plugins",
     "scripts": {
         "build": "webpack --mode production",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch"
     },
-    "version": "2.9.8"
+    "version": "2.9.9"
 }
```

### Comparing `django-comments-xtd-2.9.8/setup.py` & `django-comments-xtd-2.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 test.run_tests = run_tests
 
 
 setup(
     name="django-comments-xtd",
-    version="2.9.8",
+    version="2.9.9",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description=("Django Comments Framework extension app with thread "
                  "support, follow up notifications and email "
                  "confirmations."),
     long_description=("A reusable Django app that extends django-contrib-"
@@ -33,15 +33,15 @@
     author_email="danirus@eml.cc",
     maintainer="Daniela Rus Morales",
     maintainer_email="danirus@eml.cc",
     url="http://pypi.python.org/pypi/django-comments-xtd",
     install_requires=[
         'Django>=3,<5',
         'django-contrib-comments>=2.2,<2.3',
-        'djangorestframework>=3.12,<3.14',
+        'djangorestframework>=3.12,<3.15',
         'docutils',
         'six',
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
```

### Comparing `django-comments-xtd-2.9.8/tox.ini` & `django-comments-xtd-2.9.9/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     pytest
     pytest-cov
     pytest-django
     selenium
     py-3.10-django-3.2: django>=3.2,<3.3
     py-3.10-django-4.0: django>=4.0,<4.1
     py-3.10-django-4.1: django>=4.1,<4.2
-    py-3.10-django-{3.2,4.0,4.1}: djangorestframework>=3.12,<3.13
+    py-3.10-django-{3.2,4.0,4.1}: djangorestframework>=3.12,<3.15
     py-3.10-django-{3.2,4.0,4.1}: django-contrib-comments>=2.1,<2.2
     py-3.10-django-{4.0,4.1}: pytz
 setenv =
     PYTHONPATH = {toxinidir}:{toxinidir}
     DJANGO_SETTINGS_MODULE=django_comments_xtd.tests.settings
 
 [testenv:pep8]
```

### Comparing `django-comments-xtd-2.9.8/webpack.config.js` & `django-comments-xtd-2.9.9/webpack.config.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
 module.exports = {
     mode: "production",
     devtool: 'source-map',
     entry: {
         plugin: path.resolve(SOURCE_DIR, 'index.js')
     },
     output: {
-        filename: '[name]-2.9.8.js',
+        filename: '[name]-2.9.9.js',
         path: STATIC_DIR
     },
     optimization: {
         splitChunks: {
             cacheGroups: {
                 default: false,
                 vendors: false,
```

