# Comparing `tmp/django-oscar-3.2b0.tar.gz` & `tmp/django-oscar-3.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oscar-3.2b0.tar", last modified: Wed Nov 30 10:39:15 2022, max compression
+gzip compressed data, was "django-oscar-3.2b1.tar", last modified: Tue Dec  6 08:59:33 2022, max compression
```

## Comparing `django-oscar-3.2b0.tar` & `django-oscar-3.2b1.tar`

### file list

```diff
@@ -1,1414 +1,1414 @@
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.522693 django-oscar-3.2b0/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4146 2022-06-24 08:25:41.000000 django-oscar-3.2b0/AUTHORS
--rw-r--r--   0 viggodevries   (501) staff       (20)      120 2019-10-01 13:53:56.000000 django-oscar-3.2b0/CHANGELOG.rst
--rw-r--r--   0 viggodevries   (501) staff       (20)      291 2019-10-01 13:53:56.000000 django-oscar-3.2b0/CONTRIBUTING.rst
--rw-r--r--   0 viggodevries   (501) staff       (20)     1589 2019-10-01 13:53:56.000000 django-oscar-3.2b0/LICENSE
--rw-r--r--   0 viggodevries   (501) staff       (20)      179 2019-10-01 13:53:56.000000 django-oscar-3.2b0/MANIFEST.in
--rw-r--r--   0 viggodevries   (501) staff       (20)    12347 2022-11-30 10:39:15.522833 django-oscar-3.2b0/PKG-INFO
--rw-r--r--   0 viggodevries   (501) staff       (20)    12052 2022-09-27 07:31:46.000000 django-oscar-3.2b0/README.rst
--rw-r--r--   0 viggodevries   (501) staff       (20)      471 2022-11-30 10:39:15.523758 django-oscar-3.2b0/setup.cfg
--rwxr-xr-x   0 viggodevries   (501) staff       (20)     4582 2022-06-24 08:22:10.000000 django-oscar-3.2b0/setup.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.744050 django-oscar-3.2b0/src/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.801175 django-oscar-3.2b0/src/django_oscar.egg-info/
--rw-r--r--   0 viggodevries   (501) staff       (20)    12347 2022-11-30 10:39:14.000000 django-oscar-3.2b0/src/django_oscar.egg-info/PKG-INFO
--rw-r--r--   0 viggodevries   (501) staff       (20)    51547 2022-11-30 10:39:14.000000 django-oscar-3.2b0/src/django_oscar.egg-info/SOURCES.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)        1 2022-11-30 10:39:14.000000 django-oscar-3.2b0/src/django_oscar.egg-info/dependency_links.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)      757 2022-11-30 10:39:14.000000 django-oscar-3.2b0/src/django_oscar.egg-info/requires.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)        6 2022-11-30 10:39:14.000000 django-oscar-3.2b0/src/django_oscar.egg-info/top_level.txt
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.802855 django-oscar-3.2b0/src/oscar/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2645 2022-11-30 10:33:43.000000 django-oscar-3.2b0/src/oscar/__init__.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.803534 django-oscar-3.2b0/src/oscar/apps/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/__init__.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.808709 django-oscar-3.2b0/src/oscar/apps/address/
--rw-r--r--   0 viggodevries   (501) staff       (20)       61 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/address/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    21333 2022-03-29 09:58:26.000000 django-oscar-3.2b0/src/oscar/apps/address/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      638 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/address/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      225 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/address/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1049 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/address/forms.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.813222 django-oscar-3.2b0/src/oscar/apps/address/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4532 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/address/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      647 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/address/migrations/0002_auto_20150927_1547.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      977 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/address/migrations/0003_auto_20150927_1551.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      780 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/address/migrations/0004_auto_20170226_1122.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      825 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/address/migrations/0005_regenerate_user_address_hashes.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      452 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/address/migrations/0006_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/address/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      436 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/address/models.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.817683 django-oscar-3.2b0/src/oscar/apps/analytics/
--rw-r--r--   0 viggodevries   (501) staff       (20)       65 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/analytics/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3711 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/analytics/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      854 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/analytics/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      295 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/analytics/apps.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.820796 django-oscar-3.2b0/src/oscar/apps/analytics/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     3988 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/analytics/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1208 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/analytics/migrations/0002_auto_20140827_1705.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      643 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/analytics/migrations/0003_auto_20200801_0817.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/analytics/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      828 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/analytics/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4057 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/analytics/receivers.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3277 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/analytics/reports.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      755 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/analytics/scores.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.828867 django-oscar-3.2b0/src/oscar/apps/basket/
--rw-r--r--   0 viggodevries   (501) staff       (20)       59 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    32805 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/basket/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1153 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1271 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/basket/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    13333 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/basket/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2152 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/formsets.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      894 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/managers.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     8264 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/middleware.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.837496 django-oscar-3.2b0/src/oscar/apps/basket/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     3081 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1879 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0002_auto_20140827_1705.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      534 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0003_basket_vouchers.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      500 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0004_auto_20141007_2032.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      453 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0005_auto_20150604_1450.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      450 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0006_auto_20160111_1108.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      539 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0007_slugfield_noop.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      437 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0008_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      435 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0009_line_date_updated.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1149 2022-09-30 12:01:09.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0010_convert_to_valid_json.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      493 2022-09-30 11:49:54.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/0011_json_basket_option.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      654 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/basket/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4550 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/basket/reports.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      154 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/basket/signals.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     7166 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/basket/utils.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    22520 2022-06-24 08:22:10.000000 django-oscar-3.2b0/src/oscar/apps/basket/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.846589 django-oscar-3.2b0/src/oscar/apps/catalogue/
--rw-r--r--   0 viggodevries   (501) staff       (20)       65 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    51436 2022-11-24 08:58:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3208 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2036 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1486 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/categories.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      142 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/exceptions.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1331 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/expressions.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4291 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/managers.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.861287 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)    16465 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      535 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0002_auto_20150217_1221.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1457 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0003_data_migration_slugs.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      463 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0004_auto_20150217_1710.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      631 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0005_auto_20150604_1450.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      766 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0006_auto_20150807_1725.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      394 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0007_auto_20151207_1440.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      732 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0008_auto_20160304_1652.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      526 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0009_slugfield_noop.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1447 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0010_auto_20170420_0439.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      413 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0011_auto_20170422_1355.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      997 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0012_auto_20170609_1902.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      734 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0013_auto_20170821_1548.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1098 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0014_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      491 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0015_product_is_public.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1394 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0016_auto_20190327_0757.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      999 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0017_auto_20190816_0938.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1067 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0018_auto_20191220_0920.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1175 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0019_option_required.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      799 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0020_auto_20200801_0817.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1058 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0021_auto_20201005_0844.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      460 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0022_auto_20210210_0539.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      461 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0023_auto_20210824_1414.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     5106 2022-10-25 07:33:45.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0024_remove_duplicate_attributes.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      389 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0025_attribute_code_uniquetogether_constraint.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1825 2022-09-30 11:49:54.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0026_predefined_product_options.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1961 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4526 2022-11-24 08:58:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/product_attributes.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1340 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/receivers.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.867787 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/
--rw-r--r--   0 viggodevries   (501) staff       (20)       80 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     6908 2019-10-25 08:30:30.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      584 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1197 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1623 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      191 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/managers.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.870579 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     3402 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      481 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/migrations/0002_update_email_length.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      658 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/migrations/0003_auto_20160802_1358.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      580 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/migrations/0004_auto_20170429_0941.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      361 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)       64 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/signals.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      288 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/utils.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4848 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/views.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4333 2022-11-24 08:58:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/search_handlers.py
--rw-r--r--   0 viggodevries   (501) staff       (20)       66 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/signals.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     6025 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/utils.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     7732 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/catalogue/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.877634 django-oscar-3.2b0/src/oscar/apps/checkout/
--rw-r--r--   0 viggodevries   (501) staff       (20)       63 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/checkout/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1544 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/checkout/applicator.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2557 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/checkout/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1074 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/checkout/calculators.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      210 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/checkout/context_processors.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      523 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/checkout/exceptions.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3212 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/checkout/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    12631 2022-03-29 09:58:26.000000 django-oscar-3.2b0/src/oscar/apps/checkout/mixins.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/checkout/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    18473 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/checkout/session.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      134 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/checkout/signals.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1887 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/checkout/surcharges.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     8369 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/checkout/utils.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    29119 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/checkout/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.883325 django-oscar-3.2b0/src/oscar/apps/communication/
--rw-r--r--   0 viggodevries   (501) staff       (20)       73 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     7821 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      271 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2857 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/app.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      249 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      301 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/config.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      609 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/managers.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.886675 django-oscar-3.2b0/src/oscar/apps/communication/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4986 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      707 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/migrations/0002_reset_table_names.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      973 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/migrations/0003_remove_notification_category_make_code_uppercase.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      888 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/migrations/0004_auto_20200801_0817.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      591 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/models.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.887695 django-oscar-3.2b0/src/oscar/apps/communication/notifications/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/notifications/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      394 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/notifications/context_processors.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3424 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/notifications/views.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     6183 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/communication/utils.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.893465 django-oscar-3.2b0/src/oscar/apps/customer/
--rw-r--r--   0 viggodevries   (501) staff       (20)       63 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/customer/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     8236 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/abstract_models.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.895330 django-oscar-3.2b0/src/oscar/apps/customer/alerts/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/customer/alerts/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      546 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/alerts/receivers.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4900 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/alerts/utils.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4737 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/alerts/views.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    10953 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2364 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/customer/auth_backends.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    15245 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2279 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/history.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.898872 django-oscar-3.2b0/src/oscar/apps/customer/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     5889 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/customer/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      906 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/customer/migrations/0002_auto_20150807_1725.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      507 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/customer/migrations/0003_update_email_length.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      835 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/customer/migrations/0004_email_save.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      411 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/customer/migrations/0005_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      913 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/migrations/0006_auto_20190430_1736.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      660 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/migrations/0007_auto_20200801_0817.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/customer/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3161 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/mixins.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      282 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      536 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/receivers.py
--rw-r--r--   0 viggodevries   (501) staff       (20)       89 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/signals.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2463 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/utils.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    25756 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/customer/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.899325 django-oscar-3.2b0/src/oscar/apps/customer/wishlists/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/customer/wishlists/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    15194 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/apps/customer/wishlists/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.905354 django-oscar-3.2b0/src/oscar/apps/dashboard/
--rw-r--r--   0 viggodevries   (501) staff       (20)       65 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2608 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/apps.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.911561 django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/
--rw-r--r--   0 viggodevries   (501) staff       (20)       91 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     8509 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    15111 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     6153 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/formsets.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      643 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/mixins.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4557 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/tables.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    37950 2022-06-24 08:22:10.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/views.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      746 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/widgets.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.914311 django-oscar-3.2b0/src/oscar/apps/dashboard/communications/
--rw-r--r--   0 viggodevries   (501) staff       (20)      101 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/communications/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      856 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/communications/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3161 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/communications/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/communications/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2998 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/communications/views.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1921 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/menu.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3276 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/nav.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.917694 django-oscar-3.2b0/src/oscar/apps/dashboard/offers/
--rw-r--r--   0 viggodevries   (501) staff       (20)       78 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/offers/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2260 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/offers/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     8610 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/offers/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/offers/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      969 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/offers/reports.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    15297 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/offers/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.919622 django-oscar-3.2b0/src/oscar/apps/dashboard/orders/
--rw-r--r--   0 viggodevries   (501) staff       (20)       78 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/orders/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2084 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/orders/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     5770 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/orders/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    32430 2022-11-24 08:58:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/orders/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.921636 django-oscar-3.2b0/src/oscar/apps/dashboard/pages/
--rw-r--r--   0 viggodevries   (501) staff       (20)       76 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/pages/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1228 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/pages/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1708 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/pages/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4412 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/pages/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.923034 django-oscar-3.2b0/src/oscar/apps/dashboard/partners/
--rw-r--r--   0 viggodevries   (501) staff       (20)       89 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/partners/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2570 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/partners/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4785 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/partners/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    10483 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/partners/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.924670 django-oscar-3.2b0/src/oscar/apps/dashboard/ranges/
--rw-r--r--   0 viggodevries   (501) staff       (20)       78 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/ranges/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1514 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/ranges/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2953 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/ranges/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/ranges/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     8590 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/ranges/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.927298 django-oscar-3.2b0/src/oscar/apps/dashboard/reports/
--rw-r--r--   0 viggodevries   (501) staff       (20)       87 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reports/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      659 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reports/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1804 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reports/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reports/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3968 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reports/reports.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1232 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reports/utils.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2371 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reports/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.929288 django-oscar-3.2b0/src/oscar/apps/dashboard/reviews/
--rw-r--r--   0 viggodevries   (501) staff       (20)       87 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reviews/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1000 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reviews/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1451 2019-10-25 08:30:30.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reviews/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reviews/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     6634 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/reviews/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.930829 django-oscar-3.2b0/src/oscar/apps/dashboard/shipping/
--rw-r--r--   0 viggodevries   (501) staff       (20)       89 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/shipping/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2546 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/shipping/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      534 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/shipping/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     5069 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/shipping/views.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      596 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/tables.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.932666 django-oscar-3.2b0/src/oscar/apps/dashboard/users/
--rw-r--r--   0 viggodevries   (501) staff       (20)       76 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/users/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1886 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/users/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1405 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/users/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1096 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/users/tables.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     8081 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/users/views.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    11316 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.935088 django-oscar-3.2b0/src/oscar/apps/dashboard/vouchers/
--rw-r--r--   0 viggodevries   (501) staff       (20)       89 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/vouchers/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2580 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/vouchers/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4930 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/vouchers/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    12398 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/vouchers/views.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3127 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/dashboard/widgets.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.943434 django-oscar-3.2b0/src/oscar/apps/offer/
--rw-r--r--   0 viggodevries   (501) staff       (20)       57 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    41948 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/offer/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1188 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3751 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/applicator.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      747 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/offer/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    12252 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/offer/benefits.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    10595 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/offer/conditions.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1849 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/custom.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      835 2019-10-25 08:30:30.000000 django-oscar-3.2b0/src/oscar/apps/offer/managers.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.947831 django-oscar-3.2b0/src/oscar/apps/offer/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)    15415 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      518 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/0002_auto_20151210_1053.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      537 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/0003_auto_20161120_1707.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      509 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/0004_auto_20170415_1518.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      857 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/0005_auto_20170423_1217.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      912 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/0006_auto_20170504_0616.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      561 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/0007_conditionaloffer_exclusive.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      731 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/0008_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      400 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/0009_auto_20200801_0817.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      602 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/0010_conditionaloffer_combinations.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1860 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2778 2022-09-27 07:31:46.000000 django-oscar-3.2b0/src/oscar/apps/offer/queryset.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1064 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/offer/receivers.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2451 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/offer/reports.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     5456 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/results.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1008 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/offer/utils.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2882 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/offer/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.954201 django-oscar-3.2b0/src/oscar/apps/order/
--rw-r--r--   0 viggodevries   (501) staff       (20)       57 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    40614 2022-09-27 07:31:42.000000 django-oscar-3.2b0/src/oscar/apps/order/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3039 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/order/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      217 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      291 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/exceptions.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.961556 django-oscar-3.2b0/src/oscar/apps/order/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)    24133 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      486 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0002_auto_20141007_2032.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      443 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0003_auto_20150113_1629.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      431 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0004_auto_20160111_1108.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      502 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0005_update_email_length.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1225 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0006_orderstatuschange.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1102 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0007_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      577 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0008_auto_20190301_1035.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1263 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0009_surcharge.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      549 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0010_auto_20200724_0909.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      624 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0011_auto_20200801_0817.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1146 2022-09-30 12:01:09.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0012_convert_to_valid_json.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      492 2022-09-30 11:49:54.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/0013_json_option_value.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/order/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      488 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/order/mixins.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2534 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/order/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    10391 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/order/processing.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2042 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/order/reports.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      167 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/order/signals.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    12838 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/order/utils.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.968794 django-oscar-3.2b0/src/oscar/apps/partner/
--rw-r--r--   0 viggodevries   (501) staff       (20)       61 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    11566 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/partner/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      407 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/partner/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      287 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3207 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/availability.py
--rw-r--r--   0 viggodevries   (501) staff       (20)       94 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/exceptions.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4886 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/partner/importers.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.971699 django-oscar-3.2b0/src/oscar/apps/partner/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     6571 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      500 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/migrations/0002_auto_20141007_2032.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      514 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/migrations/0003_auto_20150604_1450.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      528 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/migrations/0004_auto_20160107_1755.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      649 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/migrations/0005_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      842 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/partner/migrations/0006_auto_20200724_0909.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      830 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2372 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/prices.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      920 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/partner/receivers.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    13435 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/partner/strategy.py
--rw-r--r--   0 viggodevries   (501) staff       (20)       26 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/partner/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.974862 django-oscar-3.2b0/src/oscar/apps/payment/
--rw-r--r--   0 viggodevries   (501) staff       (20)       61 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    11260 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/payment/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      676 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      225 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2650 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/bankcards.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1179 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/exceptions.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     9663 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/payment/forms.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.977249 django-oscar-3.2b0/src/oscar/apps/payment/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4917 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      489 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/migrations/0002_auto_20141007_2032.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      492 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/migrations/0003_auto_20160323_1520.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      449 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/migrations/0004_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      797 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/payment/migrations/0005_auto_20200801_0817.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      716 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/payment/models.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.981073 django-oscar-3.2b0/src/oscar/apps/search/
--rw-r--r--   0 viggodevries   (501) staff       (20)       59 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/search/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1195 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/search/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      246 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/search/context_processors.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4932 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/search/facets.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      395 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/search/features.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     5242 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/search/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     8144 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/apps/search/search_handlers.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3760 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/search/search_indexes.py
--rw-r--r--   0 viggodevries   (501) staff       (20)       59 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/search/signals.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2618 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/search/views.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.984318 django-oscar-3.2b0/src/oscar/apps/shipping/
--rw-r--r--   0 viggodevries   (501) staff       (20)       63 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/shipping/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     7877 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/shipping/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      755 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/shipping/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      229 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/shipping/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     5934 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/shipping/methods.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.985779 django-oscar-3.2b0/src/oscar/apps/shipping/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4307 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/shipping/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      671 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/shipping/migrations/0002_auto_20150604_1450.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1130 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/shipping/migrations/0003_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/shipping/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      636 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/shipping/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3688 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/shipping/repository.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1091 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/shipping/scales.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.990009 django-oscar-3.2b0/src/oscar/apps/voucher/
--rw-r--r--   0 viggodevries   (501) staff       (20)       61 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    10115 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/voucher/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1031 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      287 2022-02-09 19:35:31.000000 django-oscar-3.2b0/src/oscar/apps/voucher/apps.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.994425 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     3199 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      634 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0002_auto_20170418_2132.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      497 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0003_auto_20171212_0411.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1877 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0004_auto_20180228_0940.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      602 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0005_auto_20180402_1425.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      486 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0006_auto_20180413_0911.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      623 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0007_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1482 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0008_auto_20200801_0817.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1064 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0009_make_voucher_names_unique.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      810 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0010_auto_20210224_0712.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      634 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      661 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/voucher/receivers.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1448 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/voucher/reports.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1224 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/apps/voucher/utils.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.998092 django-oscar-3.2b0/src/oscar/apps/wishlists/
--rw-r--r--   0 viggodevries   (501) staff       (20)       65 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     5917 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/abstract_models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      327 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/admin.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      602 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/apps.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      817 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/forms.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      719 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/formsets.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.000832 django-oscar-3.2b0/src/oscar/apps/wishlists/migrations/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2782 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/migrations/0001_initial.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      390 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/migrations/0002_auto_20160111_1108.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      448 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/migrations/0003_auto_20181115_1953.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      891 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/migrations/0004_auto_20220328_0939.py
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/migrations/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      571 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1805 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/apps/wishlists/views.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3394 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/config.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.007666 django-oscar-3.2b0/src/oscar/core/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/core/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1254 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/core/ajax.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4972 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/core/application.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4320 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/core/compat.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1130 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/core/context_processors.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     5406 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/core/customisation.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      996 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/core/decorators.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      167 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/core/exceptions.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    10885 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/core/loading.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.008909 django-oscar-3.2b0/src/oscar/core/logging/
--rw-r--r--   0 viggodevries   (501) staff       (20)      467 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/core/logging/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      330 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/core/logging/formatters.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2285 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/core/prices.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2070 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/core/thumbnails.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     7029 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/core/utils.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4249 2019-10-25 08:30:30.000000 django-oscar-3.2b0/src/oscar/core/validators.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     7714 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/defaults.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.011150 django-oscar-3.2b0/src/oscar/forms/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/forms/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1003 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/forms/fields.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4491 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/forms/mixins.py
--rw-r--r--   0 viggodevries   (501) staff       (20)    10101 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/forms/widgets.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.776008 django-oscar-3.2b0/src/oscar/locale/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.750962 django-oscar-3.2b0/src/oscar/locale/am_ET/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.012531 django-oscar-3.2b0/src/oscar/locale/am_ET/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      450 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/am_ET/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263752 2022-11-30 10:24:02.000000 django-oscar-3.2b0/src/oscar/locale/am_ET/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.751175 django-oscar-3.2b0/src/oscar/locale/ar/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.017550 django-oscar-3.2b0/src/oscar/locale/ar/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   123176 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   317447 2022-11-30 10:23:04.000000 django-oscar-3.2b0/src/oscar/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.751384 django-oscar-3.2b0/src/oscar/locale/ar_EG/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.021076 django-oscar-3.2b0/src/oscar/locale/ar_EG/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      529 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/ar_EG/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264715 2022-11-30 10:24:04.000000 django-oscar-3.2b0/src/oscar/locale/ar_EG/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.751592 django-oscar-3.2b0/src/oscar/locale/ar_SA/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.023771 django-oscar-3.2b0/src/oscar/locale/ar_SA/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      538 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/ar_SA/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264724 2022-11-30 10:23:58.000000 django-oscar-3.2b0/src/oscar/locale/ar_SA/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.751805 django-oscar-3.2b0/src/oscar/locale/az/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.026189 django-oscar-3.2b0/src/oscar/locale/az/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2322 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/az/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264417 2022-11-30 10:24:43.000000 django-oscar-3.2b0/src/oscar/locale/az/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.752014 django-oscar-3.2b0/src/oscar/locale/az_AZ/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.028732 django-oscar-3.2b0/src/oscar/locale/az_AZ/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      456 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/az_AZ/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263758 2022-11-30 10:23:34.000000 django-oscar-3.2b0/src/oscar/locale/az_AZ/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.752224 django-oscar-3.2b0/src/oscar/locale/bg/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.031288 django-oscar-3.2b0/src/oscar/locale/bg/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      435 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263737 2022-11-30 10:23:45.000000 django-oscar-3.2b0/src/oscar/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.752450 django-oscar-3.2b0/src/oscar/locale/bg_BG/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.035067 django-oscar-3.2b0/src/oscar/locale/bg_BG/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2075 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/bg_BG/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264443 2022-11-30 10:23:40.000000 django-oscar-3.2b0/src/oscar/locale/bg_BG/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.752665 django-oscar-3.2b0/src/oscar/locale/bn/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.037710 django-oscar-3.2b0/src/oscar/locale/bn/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      433 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/bn/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263735 2022-11-30 10:24:47.000000 django-oscar-3.2b0/src/oscar/locale/bn/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.752888 django-oscar-3.2b0/src/oscar/locale/bn_BD/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.040465 django-oscar-3.2b0/src/oscar/locale/bn_BD/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4913 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/bn_BD/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   265806 2022-11-30 10:23:30.000000 django-oscar-3.2b0/src/oscar/locale/bn_BD/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.753111 django-oscar-3.2b0/src/oscar/locale/ca/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.043534 django-oscar-3.2b0/src/oscar/locale/ca/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    78491 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   292845 2022-11-30 10:23:53.000000 django-oscar-3.2b0/src/oscar/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.753340 django-oscar-3.2b0/src/oscar/locale/ca_ES/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.046113 django-oscar-3.2b0/src/oscar/locale/ca_ES/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      447 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/ca_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263749 2022-11-30 10:24:22.000000 django-oscar-3.2b0/src/oscar/locale/ca_ES/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.753549 django-oscar-3.2b0/src/oscar/locale/cmn/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.048345 django-oscar-3.2b0/src/oscar/locale/cmn/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      439 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/cmn/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263520 2022-11-30 10:23:51.000000 django-oscar-3.2b0/src/oscar/locale/cmn/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.753759 django-oscar-3.2b0/src/oscar/locale/crh/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.051162 django-oscar-3.2b0/src/oscar/locale/crh/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      442 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/crh/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263744 2022-11-30 10:24:30.000000 django-oscar-3.2b0/src/oscar/locale/crh/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.754037 django-oscar-3.2b0/src/oscar/locale/cs/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.054020 django-oscar-3.2b0/src/oscar/locale/cs/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      531 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264323 2022-11-30 10:23:52.000000 django-oscar-3.2b0/src/oscar/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.754363 django-oscar-3.2b0/src/oscar/locale/cs_CZ/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.059021 django-oscar-3.2b0/src/oscar/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   127509 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   312325 2022-11-30 10:23:20.000000 django-oscar-3.2b0/src/oscar/locale/cs_CZ/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.754736 django-oscar-3.2b0/src/oscar/locale/cy/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.062966 django-oscar-3.2b0/src/oscar/locale/cy/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2325 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/cy/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264725 2022-11-30 10:24:01.000000 django-oscar-3.2b0/src/oscar/locale/cy/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.755118 django-oscar-3.2b0/src/oscar/locale/da/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.067527 django-oscar-3.2b0/src/oscar/locale/da/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   124542 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   308000 2022-11-30 10:24:42.000000 django-oscar-3.2b0/src/oscar/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.755514 django-oscar-3.2b0/src/oscar/locale/de/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.071273 django-oscar-3.2b0/src/oscar/locale/de/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   135420 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   316492 2022-11-30 10:23:11.000000 django-oscar-3.2b0/src/oscar/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.755885 django-oscar-3.2b0/src/oscar/locale/el/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.074066 django-oscar-3.2b0/src/oscar/locale/el/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      431 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263733 2022-11-30 10:24:39.000000 django-oscar-3.2b0/src/oscar/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.756284 django-oscar-3.2b0/src/oscar/locale/el_GR/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.077395 django-oscar-3.2b0/src/oscar/locale/el_GR/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    93691 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/el_GR/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   312779 2022-11-30 10:23:56.000000 django-oscar-3.2b0/src/oscar/locale/el_GR/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.756668 django-oscar-3.2b0/src/oscar/locale/en/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.080403 django-oscar-3.2b0/src/oscar/locale/en/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      337 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   254164 2022-11-30 10:06:33.000000 django-oscar-3.2b0/src/oscar/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.757018 django-oscar-3.2b0/src/oscar/locale/en_AU/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.084215 django-oscar-3.2b0/src/oscar/locale/en_AU/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      451 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/en_AU/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263753 2022-11-30 10:24:35.000000 django-oscar-3.2b0/src/oscar/locale/en_AU/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.757350 django-oscar-3.2b0/src/oscar/locale/en_US/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.087677 django-oscar-3.2b0/src/oscar/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   134499 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/en_US/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   311249 2022-11-30 10:23:17.000000 django-oscar-3.2b0/src/oscar/locale/en_US/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.757647 django-oscar-3.2b0/src/oscar/locale/es/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.091260 django-oscar-3.2b0/src/oscar/locale/es/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   134975 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   317218 2022-11-30 10:23:33.000000 django-oscar-3.2b0/src/oscar/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.757916 django-oscar-3.2b0/src/oscar/locale/es_AR/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.093952 django-oscar-3.2b0/src/oscar/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     3682 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   265150 2022-11-30 10:23:13.000000 django-oscar-3.2b0/src/oscar/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.758230 django-oscar-3.2b0/src/oscar/locale/es_CL/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.096440 django-oscar-3.2b0/src/oscar/locale/es_CL/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      744 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/es_CL/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264132 2022-11-30 10:24:16.000000 django-oscar-3.2b0/src/oscar/locale/es_CL/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.758473 django-oscar-3.2b0/src/oscar/locale/es_MX/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.100419 django-oscar-3.2b0/src/oscar/locale/es_MX/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   135463 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/es_MX/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   312361 2022-11-30 10:24:13.000000 django-oscar-3.2b0/src/oscar/locale/es_MX/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.758700 django-oscar-3.2b0/src/oscar/locale/et/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.103666 django-oscar-3.2b0/src/oscar/locale/et/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   138542 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   312233 2022-11-30 10:24:32.000000 django-oscar-3.2b0/src/oscar/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.758928 django-oscar-3.2b0/src/oscar/locale/eu/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.108322 django-oscar-3.2b0/src/oscar/locale/eu/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    62176 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   286152 2022-11-30 10:24:41.000000 django-oscar-3.2b0/src/oscar/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.759220 django-oscar-3.2b0/src/oscar/locale/fa/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.113031 django-oscar-3.2b0/src/oscar/locale/fa/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   160839 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   340182 2022-11-30 10:23:08.000000 django-oscar-3.2b0/src/oscar/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.759678 django-oscar-3.2b0/src/oscar/locale/fa_IR/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.117391 django-oscar-3.2b0/src/oscar/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     6929 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/fa_IR/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   266591 2022-11-30 10:23:10.000000 django-oscar-3.2b0/src/oscar/locale/fa_IR/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.760056 django-oscar-3.2b0/src/oscar/locale/fi/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.121312 django-oscar-3.2b0/src/oscar/locale/fi/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   139572 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   314910 2022-11-30 10:23:03.000000 django-oscar-3.2b0/src/oscar/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.760390 django-oscar-3.2b0/src/oscar/locale/fr/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.125716 django-oscar-3.2b0/src/oscar/locale/fr/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   151694 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   326460 2022-11-30 10:24:31.000000 django-oscar-3.2b0/src/oscar/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.760751 django-oscar-3.2b0/src/oscar/locale/fr_CA/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.128281 django-oscar-3.2b0/src/oscar/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      498 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/fr_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264021 2022-11-30 10:23:07.000000 django-oscar-3.2b0/src/oscar/locale/fr_CA/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.761130 django-oscar-3.2b0/src/oscar/locale/fr_FR/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.130652 django-oscar-3.2b0/src/oscar/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      498 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264021 2022-11-30 10:24:06.000000 django-oscar-3.2b0/src/oscar/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.761464 django-oscar-3.2b0/src/oscar/locale/gu/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.134143 django-oscar-3.2b0/src/oscar/locale/gu/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      434 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/gu/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263736 2022-11-30 10:24:25.000000 django-oscar-3.2b0/src/oscar/locale/gu/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.761803 django-oscar-3.2b0/src/oscar/locale/gu_IN/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.136331 django-oscar-3.2b0/src/oscar/locale/gu_IN/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      448 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/gu_IN/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263750 2022-11-30 10:24:28.000000 django-oscar-3.2b0/src/oscar/locale/gu_IN/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.762219 django-oscar-3.2b0/src/oscar/locale/he/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.139590 django-oscar-3.2b0/src/oscar/locale/he/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   150328 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   329074 2022-11-30 10:24:09.000000 django-oscar-3.2b0/src/oscar/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.762690 django-oscar-3.2b0/src/oscar/locale/hi/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.141981 django-oscar-3.2b0/src/oscar/locale/hi/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    11559 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/hi/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   269389 2022-11-30 10:23:43.000000 django-oscar-3.2b0/src/oscar/locale/hi/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.763100 django-oscar-3.2b0/src/oscar/locale/hi_IN/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.144457 django-oscar-3.2b0/src/oscar/locale/hi_IN/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    31241 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/hi_IN/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   280974 2022-11-30 10:24:46.000000 django-oscar-3.2b0/src/oscar/locale/hi_IN/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.763474 django-oscar-3.2b0/src/oscar/locale/hr/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.147431 django-oscar-3.2b0/src/oscar/locale/hr/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    93479 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   297656 2022-11-30 10:24:08.000000 django-oscar-3.2b0/src/oscar/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.763846 django-oscar-3.2b0/src/oscar/locale/hu/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.150056 django-oscar-3.2b0/src/oscar/locale/hu/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      435 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263737 2022-11-30 10:24:34.000000 django-oscar-3.2b0/src/oscar/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.764277 django-oscar-3.2b0/src/oscar/locale/hu_HU/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.152993 django-oscar-3.2b0/src/oscar/locale/hu_HU/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   107539 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/hu_HU/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   305678 2022-11-30 10:24:44.000000 django-oscar-3.2b0/src/oscar/locale/hu_HU/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.764686 django-oscar-3.2b0/src/oscar/locale/hy/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.156532 django-oscar-3.2b0/src/oscar/locale/hy/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     7072 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/hy/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   266571 2022-11-30 10:23:28.000000 django-oscar-3.2b0/src/oscar/locale/hy/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.765076 django-oscar-3.2b0/src/oscar/locale/hy_AM/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.160190 django-oscar-3.2b0/src/oscar/locale/hy_AM/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      450 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/hy_AM/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263752 2022-11-30 10:24:24.000000 django-oscar-3.2b0/src/oscar/locale/hy_AM/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.765459 django-oscar-3.2b0/src/oscar/locale/id/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.163947 django-oscar-3.2b0/src/oscar/locale/id/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   133492 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   312290 2022-11-30 10:23:50.000000 django-oscar-3.2b0/src/oscar/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.765826 django-oscar-3.2b0/src/oscar/locale/id_ID/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.167388 django-oscar-3.2b0/src/oscar/locale/id_ID/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      447 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/id_ID/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263528 2022-11-30 10:23:15.000000 django-oscar-3.2b0/src/oscar/locale/id_ID/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.766191 django-oscar-3.2b0/src/oscar/locale/is_IS/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.169917 django-oscar-3.2b0/src/oscar/locale/is_IS/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      473 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/is_IS/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263775 2022-11-30 10:24:36.000000 django-oscar-3.2b0/src/oscar/locale/is_IS/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.766521 django-oscar-3.2b0/src/oscar/locale/it/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.174471 django-oscar-3.2b0/src/oscar/locale/it/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   146270 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   322218 2022-11-30 10:24:14.000000 django-oscar-3.2b0/src/oscar/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.766759 django-oscar-3.2b0/src/oscar/locale/ja/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.178431 django-oscar-3.2b0/src/oscar/locale/ja/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   151703 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   327354 2022-11-30 10:24:20.000000 django-oscar-3.2b0/src/oscar/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.766992 django-oscar-3.2b0/src/oscar/locale/ka_GE/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.181673 django-oscar-3.2b0/src/oscar/locale/ka_GE/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    71671 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/ka_GE/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   305689 2022-11-30 10:23:31.000000 django-oscar-3.2b0/src/oscar/locale/ka_GE/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.767219 django-oscar-3.2b0/src/oscar/locale/ko/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.185178 django-oscar-3.2b0/src/oscar/locale/ko/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   135121 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   316766 2022-11-30 10:24:40.000000 django-oscar-3.2b0/src/oscar/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.767450 django-oscar-3.2b0/src/oscar/locale/lt/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.188756 django-oscar-3.2b0/src/oscar/locale/lt/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   130728 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   314773 2022-11-30 10:24:33.000000 django-oscar-3.2b0/src/oscar/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.767665 django-oscar-3.2b0/src/oscar/locale/lv/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.191046 django-oscar-3.2b0/src/oscar/locale/lv/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     3838 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264981 2022-11-30 10:23:21.000000 django-oscar-3.2b0/src/oscar/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.767887 django-oscar-3.2b0/src/oscar/locale/ml/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.193105 django-oscar-3.2b0/src/oscar/locale/ml/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      435 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/ml/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263737 2022-11-30 10:24:45.000000 django-oscar-3.2b0/src/oscar/locale/ml/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.768107 django-oscar-3.2b0/src/oscar/locale/mr/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.195339 django-oscar-3.2b0/src/oscar/locale/mr/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     5262 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/mr/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   266318 2022-11-30 10:23:55.000000 django-oscar-3.2b0/src/oscar/locale/mr/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.768327 django-oscar-3.2b0/src/oscar/locale/ms/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.197263 django-oscar-3.2b0/src/oscar/locale/ms/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      424 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/ms/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263505 2022-11-30 10:23:59.000000 django-oscar-3.2b0/src/oscar/locale/ms/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.768559 django-oscar-3.2b0/src/oscar/locale/nb_NO/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.201205 django-oscar-3.2b0/src/oscar/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    36393 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   276456 2022-11-30 10:24:38.000000 django-oscar-3.2b0/src/oscar/locale/nb_NO/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.768796 django-oscar-3.2b0/src/oscar/locale/nl/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.203939 django-oscar-3.2b0/src/oscar/locale/nl/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   153184 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   323218 2022-11-30 10:24:23.000000 django-oscar-3.2b0/src/oscar/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.769019 django-oscar-3.2b0/src/oscar/locale/pl/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.209037 django-oscar-3.2b0/src/oscar/locale/pl/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   135695 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   316940 2022-11-30 10:23:49.000000 django-oscar-3.2b0/src/oscar/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.769236 django-oscar-3.2b0/src/oscar/locale/pt/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.212366 django-oscar-3.2b0/src/oscar/locale/pt/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      487 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264010 2022-11-30 10:24:15.000000 django-oscar-3.2b0/src/oscar/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.769450 django-oscar-3.2b0/src/oscar/locale/pt_BR/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.216470 django-oscar-3.2b0/src/oscar/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   142706 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   319650 2022-11-30 10:23:24.000000 django-oscar-3.2b0/src/oscar/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.769665 django-oscar-3.2b0/src/oscar/locale/pt_PT/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.220507 django-oscar-3.2b0/src/oscar/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   146645 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   320816 2022-11-30 10:23:26.000000 django-oscar-3.2b0/src/oscar/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.769888 django-oscar-3.2b0/src/oscar/locale/ro_RO/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.224907 django-oscar-3.2b0/src/oscar/locale/ro_RO/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   106322 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/ro_RO/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   302696 2022-11-30 10:24:11.000000 django-oscar-3.2b0/src/oscar/locale/ro_RO/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.770108 django-oscar-3.2b0/src/oscar/locale/ru/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.227177 django-oscar-3.2b0/src/oscar/locale/ru/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    13779 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   270527 2022-11-30 10:23:35.000000 django-oscar-3.2b0/src/oscar/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.770331 django-oscar-3.2b0/src/oscar/locale/ru@petr1708/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.229140 django-oscar-3.2b0/src/oscar/locale/ru@petr1708/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      609 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/ru@petr1708/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264353 2022-11-30 10:23:46.000000 django-oscar-3.2b0/src/oscar/locale/ru@petr1708/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.770551 django-oscar-3.2b0/src/oscar/locale/ru_RU/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.232189 django-oscar-3.2b0/src/oscar/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   179538 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/ru_RU/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   357671 2022-11-30 10:24:29.000000 django-oscar-3.2b0/src/oscar/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.770773 django-oscar-3.2b0/src/oscar/locale/sk/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.236536 django-oscar-3.2b0/src/oscar/locale/sk/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   126358 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   312056 2022-11-30 10:24:10.000000 django-oscar-3.2b0/src/oscar/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.770990 django-oscar-3.2b0/src/oscar/locale/sk_SK/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.239092 django-oscar-3.2b0/src/oscar/locale/sk_SK/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      524 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/sk_SK/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264268 2022-11-30 10:23:18.000000 django-oscar-3.2b0/src/oscar/locale/sk_SK/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.771214 django-oscar-3.2b0/src/oscar/locale/sl_SI/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.241509 django-oscar-3.2b0/src/oscar/locale/sl_SI/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   125966 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/sl_SI/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   309780 2022-11-30 10:23:06.000000 django-oscar-3.2b0/src/oscar/locale/sl_SI/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.771430 django-oscar-3.2b0/src/oscar/locale/sr/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.244264 django-oscar-3.2b0/src/oscar/locale/sr/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   127942 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   310850 2022-11-30 10:23:42.000000 django-oscar-3.2b0/src/oscar/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.771645 django-oscar-3.2b0/src/oscar/locale/sv/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.247407 django-oscar-3.2b0/src/oscar/locale/sv/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    94590 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   297973 2022-11-30 10:23:23.000000 django-oscar-3.2b0/src/oscar/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.771862 django-oscar-3.2b0/src/oscar/locale/sv_SE/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.249681 django-oscar-3.2b0/src/oscar/locale/sv_SE/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      448 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/sv_SE/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263750 2022-11-30 10:23:44.000000 django-oscar-3.2b0/src/oscar/locale/sv_SE/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.772075 django-oscar-3.2b0/src/oscar/locale/sw/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.252339 django-oscar-3.2b0/src/oscar/locale/sw/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      433 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263735 2022-11-30 10:23:37.000000 django-oscar-3.2b0/src/oscar/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.772305 django-oscar-3.2b0/src/oscar/locale/sw_KE/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.255485 django-oscar-3.2b0/src/oscar/locale/sw_KE/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      447 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/sw_KE/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263749 2022-11-30 10:24:26.000000 django-oscar-3.2b0/src/oscar/locale/sw_KE/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.772521 django-oscar-3.2b0/src/oscar/locale/th/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.258726 django-oscar-3.2b0/src/oscar/locale/th/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      423 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263504 2022-11-30 10:24:03.000000 django-oscar-3.2b0/src/oscar/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.772749 django-oscar-3.2b0/src/oscar/locale/th_TH/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.262065 django-oscar-3.2b0/src/oscar/locale/th_TH/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    13390 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/th_TH/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   270546 2022-11-30 10:24:37.000000 django-oscar-3.2b0/src/oscar/locale/th_TH/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.772962 django-oscar-3.2b0/src/oscar/locale/tr/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.266685 django-oscar-3.2b0/src/oscar/locale/tr/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   131714 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   314258 2022-11-30 10:23:12.000000 django-oscar-3.2b0/src/oscar/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.773176 django-oscar-3.2b0/src/oscar/locale/tr_CY/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.269767 django-oscar-3.2b0/src/oscar/locale/tr_CY/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      447 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/tr_CY/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263749 2022-11-30 10:24:21.000000 django-oscar-3.2b0/src/oscar/locale/tr_CY/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.773392 django-oscar-3.2b0/src/oscar/locale/tr_TR/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.273357 django-oscar-3.2b0/src/oscar/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     5440 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   265526 2022-11-30 10:24:17.000000 django-oscar-3.2b0/src/oscar/locale/tr_TR/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.773611 django-oscar-3.2b0/src/oscar/locale/uk/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.278290 django-oscar-3.2b0/src/oscar/locale/uk/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   174600 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   352968 2022-11-30 10:23:14.000000 django-oscar-3.2b0/src/oscar/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.773833 django-oscar-3.2b0/src/oscar/locale/uk_UA/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.281397 django-oscar-3.2b0/src/oscar/locale/uk_UA/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1289 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/uk_UA/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   264763 2022-11-30 10:23:38.000000 django-oscar-3.2b0/src/oscar/locale/uk_UA/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.774049 django-oscar-3.2b0/src/oscar/locale/vi/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.285439 django-oscar-3.2b0/src/oscar/locale/vi/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   139945 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   322890 2022-11-30 10:23:48.000000 django-oscar-3.2b0/src/oscar/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.774720 django-oscar-3.2b0/src/oscar/locale/zh/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.295234 django-oscar-3.2b0/src/oscar/locale/zh/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     7225 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   265431 2022-11-30 10:23:19.000000 django-oscar-3.2b0/src/oscar/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.774272 django-oscar-3.2b0/src/oscar/locale/zh-Hans/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.290246 django-oscar-3.2b0/src/oscar/locale/zh-Hans/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   130881 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/zh-Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   305752 2022-11-30 10:24:18.000000 django-oscar-3.2b0/src/oscar/locale/zh-Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.774511 django-oscar-3.2b0/src/oscar/locale/zh-Hant/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.292878 django-oscar-3.2b0/src/oscar/locale/zh-Hant/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    22350 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/zh-Hant/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   270580 2022-11-30 10:24:05.000000 django-oscar-3.2b0/src/oscar/locale/zh-Hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.775157 django-oscar-3.2b0/src/oscar/locale/zh_CN/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.299755 django-oscar-3.2b0/src/oscar/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1960 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   265285 2022-11-30 10:23:29.000000 django-oscar-3.2b0/src/oscar/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.774942 django-oscar-3.2b0/src/oscar/locale/zh_CN.GB2312/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.297287 django-oscar-3.2b0/src/oscar/locale/zh_CN.GB2312/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      463 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/zh_CN.GB2312/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263544 2022-11-30 10:23:27.000000 django-oscar-3.2b0/src/oscar/locale/zh_CN.GB2312/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.775402 django-oscar-3.2b0/src/oscar/locale/zh_HK/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.302132 django-oscar-3.2b0/src/oscar/locale/zh_HK/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)    10473 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/zh_HK/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   266468 2022-11-30 10:23:39.000000 django-oscar-3.2b0/src/oscar/locale/zh_HK/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.775638 django-oscar-3.2b0/src/oscar/locale/zh_SG/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.304818 django-oscar-3.2b0/src/oscar/locale/zh_SG/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      444 2022-11-30 10:25:17.000000 django-oscar-3.2b0/src/oscar/locale/zh_SG/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263525 2022-11-30 10:23:57.000000 django-oscar-3.2b0/src/oscar/locale/zh_SG/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.776093 django-oscar-3.2b0/src/oscar/locale/zh_TW/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.312416 django-oscar-3.2b0/src/oscar/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)   112036 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   299815 2022-11-30 10:23:25.000000 django-oscar-3.2b0/src/oscar/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.775865 django-oscar-3.2b0/src/oscar/locale/zh_TW.Big5/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.307880 django-oscar-3.2b0/src/oscar/locale/zh_TW.Big5/LC_MESSAGES/
--rw-r--r--   0 viggodevries   (501) staff       (20)      459 2022-11-30 10:25:18.000000 django-oscar-3.2b0/src/oscar/locale/zh_TW.Big5/LC_MESSAGES/django.mo
--rw-r--r--   0 viggodevries   (501) staff       (20)   263540 2022-11-30 10:23:41.000000 django-oscar-3.2b0/src/oscar/locale/zh_TW.Big5/LC_MESSAGES/django.po
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.314961 django-oscar-3.2b0/src/oscar/management/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/management/__init__.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.322593 django-oscar-3.2b0/src/oscar/management/commands/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/management/commands/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      372 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_calculate_scores.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1727 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_cleanup_alerts.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1054 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_find_duplicate_emails.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1123 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_fork_app.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1787 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_fork_statics.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1090 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_generate_email_content.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1413 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_import_catalogue.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      797 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_import_catalogue_images.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2214 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_populate_countries.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      791 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_send_alerts.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      687 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/management/commands/oscar_update_product_ratings.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.323046 django-oscar-3.2b0/src/oscar/models/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/models/__init__.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.324523 django-oscar-3.2b0/src/oscar/models/fields/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4366 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/models/fields/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     7070 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/models/fields/autoslugfield.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      466 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/models/fields/slugfield.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.776900 django-oscar-3.2b0/src/oscar/static/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.325334 django-oscar-3.2b0/src/oscar/static/oscar/
--rw-r--r--   0 viggodevries   (501) staff       (20)      655 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/README.rst
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.328699 django-oscar-3.2b0/src/oscar/static/oscar/css/
--rw-r--r--   0 viggodevries   (501) staff       (20)   295633 2022-11-30 10:38:00.000000 django-oscar-3.2b0/src/oscar/static/oscar/css/dashboard.css
--rw-r--r--   0 viggodevries   (501) staff       (20)   508684 2022-11-30 10:38:00.000000 django-oscar-3.2b0/src/oscar/static/oscar/css/dashboard.css.map
--rw-r--r--   0 viggodevries   (501) staff       (20)    16792 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/css/select2-bootstrap.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)   294186 2022-11-30 10:38:01.000000 django-oscar-3.2b0/src/oscar/static/oscar/css/styles.css
--rw-r--r--   0 viggodevries   (501) staff       (20)   509158 2022-11-30 10:38:01.000000 django-oscar-3.2b0/src/oscar/static/oscar/css/styles.css.map
--rw-r--r--   0 viggodevries   (501) staff       (20)     1150 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/favicon.ico
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.330307 django-oscar-3.2b0/src/oscar/static/oscar/img/
--rw-r--r--   0 viggodevries   (501) staff       (20)     8777 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/glyphicons-halflings-white.png
--rw-r--r--   0 viggodevries   (501) staff       (20)    12799 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/glyphicons-halflings.png
--rw-r--r--   0 viggodevries   (501) staff       (20)     3555 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/image_not_found.jpg
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.334353 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/
--rwxr-xr-x   0 viggodevries   (501) staff       (20)      124 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/black.png
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.335052 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/dashboard/
--rw-r--r--   0 viggodevries   (501) staff       (20)      955 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/dashboard/bg_subtle_dots.png
--rw-r--r--   0 viggodevries   (501) staff       (20)     5469 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/dashboard/logo_oscar.png
--rw-r--r--   0 viggodevries   (501) staff       (20)      331 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon-addlink.svg
--rw-r--r--   0 viggodevries   (501) staff       (20)      380 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon-changelink.svg
--rw-r--r--   0 viggodevries   (501) staff       (20)      392 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon-deletelink.svg
--rw-r--r--   0 viggodevries   (501) staff       (20)     1096 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_arrow_down.png
--rw-r--r--   0 viggodevries   (501) staff       (20)     1109 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_arrow_left.png
--rw-r--r--   0 viggodevries   (501) staff       (20)     2990 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_minus.png
--rw-r--r--   0 viggodevries   (501) staff       (20)     3077 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_plus.png
--rw-r--r--   0 viggodevries   (501) staff       (20)     1224 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_slider_left.png
--rw-r--r--   0 viggodevries   (501) staff       (20)     1218 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_slider_right.png
--rw-r--r--   0 viggodevries   (501) staff       (20)     1306 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/img/ui/nav_sprite.png
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.779038 django-oscar-3.2b0/src/oscar/static/oscar/js/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.335915 django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4/
--rw-r--r--   0 viggodevries   (501) staff       (20)   230599 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4/bootstrap.bundle.js
--rw-r--r--   0 viggodevries   (501) staff       (20)    83376 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4/bootstrap.bundle.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.337697 django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4-datetimepicker/
--rw-r--r--   0 viggodevries   (501) staff       (20)   369018 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4-datetimepicker/moment-with-locales.min.js
--rw-r--r--   0 viggodevries   (501) staff       (20)    11967 2022-11-30 10:37:43.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4-datetimepicker/tempusdominus-bootstrap-4.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)    61593 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4-datetimepicker/tempusdominus-bootstrap-4.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.338169 django-oscar-3.2b0/src/oscar/static/oscar/js/inputmask/
--rw-r--r--   0 viggodevries   (501) staff       (20)    99426 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/inputmask/jquery.inputmask.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.338859 django-oscar-3.2b0/src/oscar/static/oscar/js/jquery/
--rw-r--r--   0 viggodevries   (501) staff       (20)    89501 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/jquery/jquery.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.339623 django-oscar-3.2b0/src/oscar/static/oscar/js/jquery-sortable/
--rw-r--r--   0 viggodevries   (501) staff       (20)     9699 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/jquery-sortable/jquery-sortable-min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.340150 django-oscar-3.2b0/src/oscar/static/oscar/js/mousewheel/
--rw-r--r--   0 viggodevries   (501) staff       (20)     8267 2022-11-30 10:37:43.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/mousewheel/jquery.mousewheel.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.341786 django-oscar-3.2b0/src/oscar/static/oscar/js/oscar/
--rw-r--r--   0 viggodevries   (501) staff       (20)     5427 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/oscar/RelatedObjectLookups.js
--rw-r--r--   0 viggodevries   (501) staff       (20)    19639 2022-10-25 07:33:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/oscar/dashboard.js
--rw-r--r--   0 viggodevries   (501) staff       (20)      582 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/oscar/popup_response.js
--rw-r--r--   0 viggodevries   (501) staff       (20)    12791 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/oscar/ui.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.342693 django-oscar-3.2b0/src/oscar/static/oscar/js/select2/
--rw-r--r--   0 viggodevries   (501) staff       (20)    14966 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/select2/select2.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)    70851 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/select2/select2.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.343632 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.779338 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/icons/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.344707 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/icons/default/
--rw-r--r--   0 viggodevries   (501) staff       (20)    65274 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/icons/default/icons.min.js
--rw-r--r--   0 viggodevries   (501) staff       (20)     6507 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/jquery.tinymce.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.779591 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/models/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.345191 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/models/dom/
--rw-r--r--   0 viggodevries   (501) staff       (20)    95742 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/models/dom/model.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.784620 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.345601 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/advlist/
--rw-r--r--   0 viggodevries   (501) staff       (20)     3376 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/advlist/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.345885 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/anchor/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2537 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/anchor/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.346257 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/autolink/
--rw-r--r--   0 viggodevries   (501) staff       (20)     3060 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/autolink/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.346675 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/autoresize/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2074 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/autoresize/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.346973 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/autosave/
--rw-r--r--   0 viggodevries   (501) staff       (20)     3257 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/autosave/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.347263 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/charmap/
--rw-r--r--   0 viggodevries   (501) staff       (20)    10981 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/charmap/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.347591 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/code/
--rw-r--r--   0 viggodevries   (501) staff       (20)      877 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/code/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.347926 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/codesample/
--rw-r--r--   0 viggodevries   (501) staff       (20)    48043 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/codesample/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.348246 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/directionality/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4360 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/directionality/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.348515 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/emoticons/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.349617 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/emoticons/js/
--rw-r--r--   0 viggodevries   (501) staff       (20)   416095 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/emoticons/js/emojiimages.min.js
--rw-r--r--   0 viggodevries   (501) staff       (20)   192856 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/emoticons/js/emojis.min.js
--rw-r--r--   0 viggodevries   (501) staff       (20)     6325 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/emoticons/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.350155 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/fullscreen/
--rw-r--r--   0 viggodevries   (501) staff       (20)    14630 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/fullscreen/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.350455 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/help/
--rw-r--r--   0 viggodevries   (501) staff       (20)    13080 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/help/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.350731 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/image/
--rw-r--r--   0 viggodevries   (501) staff       (20)    19054 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/image/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.351038 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/importcss/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4036 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/importcss/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.351315 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/insertdatetime/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2911 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/insertdatetime/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.351570 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/link/
--rw-r--r--   0 viggodevries   (501) staff       (20)    15087 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/link/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.351842 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/lists/
--rw-r--r--   0 viggodevries   (501) staff       (20)    22702 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/lists/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.352141 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/media/
--rw-r--r--   0 viggodevries   (501) staff       (20)    16306 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/media/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.352471 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/nonbreaking/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1416 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/nonbreaking/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.352828 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/pagebreak/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1503 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/pagebreak/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.353072 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/preview/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1718 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/preview/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.353318 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/quickbars/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4908 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/quickbars/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.353548 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/save/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1592 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/save/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.353777 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/searchreplace/
--rw-r--r--   0 viggodevries   (501) staff       (20)    13265 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/searchreplace/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.354115 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/table/
--rw-r--r--   0 viggodevries   (501) staff       (20)    46912 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/table/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.354637 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/template/
--rw-r--r--   0 viggodevries   (501) staff       (20)     8103 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/template/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.355072 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/visualblocks/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1230 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/visualblocks/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.355461 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/visualchars/
--rw-r--r--   0 viggodevries   (501) staff       (20)     5172 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/visualchars/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.355950 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/wordcount/
--rw-r--r--   0 viggodevries   (501) staff       (20)    11913 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/wordcount/plugin.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.785867 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.785740 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.356373 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/dark/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1216 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/dark/content.min.css
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.356794 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/default/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1149 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/default/content.min.css
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.357302 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/document/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1248 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/document/content.min.css
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.357772 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1149 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5/content.min.css
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.358195 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5-dark/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1219 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5-dark/content.min.css
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.358625 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/writer/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1170 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/writer/content.min.css
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.786309 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.360653 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/
--rw-r--r--   0 viggodevries   (501) staff       (20)    22753 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/content.inline.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)    22812 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/content.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)    62379 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/skin.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)      508 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/skin.shadowdom.min.css
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.362701 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/
--rw-r--r--   0 viggodevries   (501) staff       (20)    22753 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/content.inline.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)    22423 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/content.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)    62439 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/skin.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)      508 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.364640 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/
--rw-r--r--   0 viggodevries   (501) staff       (20)    22753 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/content.inline.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)    22812 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/content.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)    64589 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/skin.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)      508 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/skin.shadowdom.min.css
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.366581 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/
--rw-r--r--   0 viggodevries   (501) staff       (20)    22753 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/content.inline.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)    22423 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/content.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)    64476 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/skin.min.css
--rw-r--r--   0 viggodevries   (501) staff       (20)      508 2022-11-30 10:37:44.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/skin.shadowdom.min.css
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.786671 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/themes/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.366889 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/themes/silver/
--rw-r--r--   0 viggodevries   (501) staff       (20)   345342 2022-11-30 10:37:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/themes/silver/theme.min.js
--rw-r--r--   0 viggodevries   (501) staff       (20)   396486 2022-11-30 10:37:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/tinymce.min.js
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.368136 django-oscar-3.2b0/src/oscar/static/oscar/scss/
--rw-r--r--   0 viggodevries   (501) staff       (20)      610 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/README.rst
--rw-r--r--   0 viggodevries   (501) staff       (20)      612 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/_alerts.scss
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.370002 django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2599 2022-09-27 09:49:25.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/base.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)      387 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/buttons.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)     1074 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/catalogue.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)      985 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/forms.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)     1934 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/index.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)     1209 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/navbar.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)      825 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/tables.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)      588 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/variables.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)      647 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard.scss
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.372871 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1556 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/checkout.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)      811 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/forms.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)     1260 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/header.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)      367 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/layout.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)     1508 2022-09-27 09:49:25.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/plugins.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)     1243 2022-09-27 09:49:25.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/product_lists.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)     1363 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/product_page.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)     1001 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/reviews.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)      255 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/type.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)      916 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/page/variables.scss
--rw-r--r--   0 viggodevries   (501) staff       (20)      675 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/static/oscar/scss/styles.scss
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.376021 django-oscar-3.2b0/src/oscar/static/oscar/webfonts/
--rw-r--r--   0 viggodevries   (501) staff       (20)   181264 2022-11-30 10:37:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-brands-400.ttf
--rw-r--r--   0 viggodevries   (501) staff       (20)   105112 2022-11-30 10:37:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-brands-400.woff2
--rw-r--r--   0 viggodevries   (501) staff       (20)    60236 2022-11-30 10:37:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-regular-400.ttf
--rw-r--r--   0 viggodevries   (501) staff       (20)    24028 2022-11-30 10:37:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-regular-400.woff2
--rw-r--r--   0 viggodevries   (501) staff       (20)   389948 2022-11-30 10:37:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-solid-900.ttf
--rw-r--r--   0 viggodevries   (501) staff       (20)   154840 2022-11-30 10:37:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-solid-900.woff2
--rw-r--r--   0 viggodevries   (501) staff       (20)    10084 2022-11-30 10:37:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 viggodevries   (501) staff       (20)     4776 2022-11-30 10:37:45.000000 django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.787561 django-oscar-3.2b0/src/oscar/templates/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.376238 django-oscar-3.2b0/src/oscar/templates/flatpages/
--rw-r--r--   0 viggodevries   (501) staff       (20)      916 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/flatpages/default.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.381604 django-oscar-3.2b0/src/oscar/templates/oscar/
--rw-r--r--   0 viggodevries   (501) staff       (20)      345 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/403.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      328 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/404.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      676 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/500.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2151 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/base.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.382530 django-oscar-3.2b0/src/oscar/templates/oscar/basket/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1029 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/basket/basket.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.386213 django-oscar-3.2b0/src/oscar/templates/oscar/basket/messages/
--rw-r--r--   0 viggodevries   (501) staff       (20)      404 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/basket/messages/addition.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      153 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/basket/messages/line_restored.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      142 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/basket/messages/line_saved.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      778 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/basket/messages/new_total.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      145 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/basket/messages/offer_gained.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      150 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/basket/messages/offer_lost.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.388143 django-oscar-3.2b0/src/oscar/templates/oscar/basket/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)    12074 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/basket/partials/basket_content.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2264 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/basket/partials/basket_quick.html
--rw-r--r--   0 viggodevries   (501) staff       (20)    12269 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/basket/partials/basket_totals.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.389358 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/
--rw-r--r--   0 viggodevries   (501) staff       (20)     4234 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/browse.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1596 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/category.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     7848 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/detail.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.392212 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1591 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/add_to_basket_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      639 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/add_to_basket_form_compact.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2812 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/add_to_wishlist.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2468 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/gallery.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1808 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/product.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2624 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/review.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      956 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/stock_record.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.394402 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.395034 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1007 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/partials/review_stars.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1475 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/review_detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2347 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/review_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1828 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/review_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      777 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/review_product.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.399798 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/
--rw-r--r--   0 viggodevries   (501) staff       (20)     6906 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/checkout.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2174 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/gateway.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1607 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/layout.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2684 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/nav.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1358 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/payment_details.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1397 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/preview.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     4613 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/shipping_address.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2616 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/shipping_methods.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     8334 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/thank_you.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1185 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/user_address_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1182 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/checkout/user_address_form.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.789049 django-oscar-3.2b0/src/oscar/templates/oscar/communication/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.400665 django-oscar-3.2b0/src/oscar/templates/oscar/communication/email/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1195 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/email/email_detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      924 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/email/email_list.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.413102 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/
--rw-r--r--   0 viggodevries   (501) staff       (20)     8093 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/base.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      227 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/base.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)      837 2022-03-29 09:58:26.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_email_changed_body.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      550 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_email_changed_body.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)      126 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_email_changed_subject.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)     2686 2022-03-29 09:58:26.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_order_placed_body.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1075 2022-03-29 09:58:26.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_order_placed_body.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)      110 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_order_placed_subject.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)      827 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_password_changed_body.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      481 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_password_changed_body.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)      117 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_password_changed_subject.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)      643 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_password_reset_body.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      434 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_password_reset_body.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)      119 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_password_reset_subject.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)     1129 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_product_alert_body.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      847 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_product_alert_body.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)      832 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_product_alert_confirmation_body.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      590 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_product_alert_confirmation_body.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)       88 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_product_alert_confirmation_subject.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)      120 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_product_alert_subject.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)       62 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_registration_body.html
--rw-r--r--   0 viggodevries   (501) staff       (20)       55 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_registration_body.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_registration_sms.txt
--rw-r--r--   0 viggodevries   (501) staff       (20)       55 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_registration_subject.txt
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.414210 django-oscar-3.2b0/src/oscar/templates/oscar/communication/notifications/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1325 2022-03-29 09:58:26.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/notifications/detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3425 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/communication/notifications/list.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.416501 django-oscar-3.2b0/src/oscar/templates/oscar/customer/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.417938 django-oscar-3.2b0/src/oscar/templates/oscar/customer/address/
--rw-r--r--   0 viggodevries   (501) staff       (20)      740 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/address/address_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      393 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/address/address_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3160 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/address/address_list.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.420414 django-oscar-3.2b0/src/oscar/templates/oscar/customer/alerts/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1774 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/alerts/alert_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)       44 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/alerts/form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      176 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/alerts/message.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      135 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/alerts/message_subject.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     4142 2022-03-29 09:58:26.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/anon_order.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1123 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/baseaccountpage.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.421079 django-oscar-3.2b0/src/oscar/templates/oscar/customer/history/
--rw-r--r--   0 viggodevries   (501) staff       (20)      481 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/history/recently_viewed_products.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1830 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/login_registration.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.422023 django-oscar-3.2b0/src/oscar/templates/oscar/customer/order/
--rw-r--r--   0 viggodevries   (501) staff       (20)     7997 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/order/order_detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2911 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/order/order_list.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.422408 django-oscar-3.2b0/src/oscar/templates/oscar/customer/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1326 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/partials/standard_tabs.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.424249 django-oscar-3.2b0/src/oscar/templates/oscar/customer/profile/
--rw-r--r--   0 viggodevries   (501) staff       (20)      199 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/profile/change_password_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1269 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/profile/profile.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      942 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/profile/profile_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      191 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/profile/profile_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1205 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/registration.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.426814 django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1434 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/wishlists_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1518 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/wishlists_delete_product.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     6262 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/wishlists_detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2300 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/wishlists_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2493 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/wishlists_list.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.429762 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/
--rw-r--r--   0 viggodevries   (501) staff       (20)      250 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/base.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.444074 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2523 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     7698 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1340 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      839 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_row_actions.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      144 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_row_name.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      144 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_row_option_summary.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1629 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/category_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     6099 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/category_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1724 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/category_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1373 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/category_row_actions.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.444463 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/messages/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1472 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/messages/product_saved.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2313 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/option_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     4051 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/option_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1183 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/option_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      791 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/option_row_actions.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      128 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/option_row_name.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1570 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_class_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     8333 2022-11-24 08:58:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_class_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3100 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_class_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2207 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3687 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      897 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_row_actions.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      456 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_row_image.html
--rw-r--r--   0 viggodevries   (501) staff       (20)       89 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_row_stockrecords.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      122 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_row_title.html
--rw-r--r--   0 viggodevries   (501) staff       (20)       91 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_row_variants.html
--rw-r--r--   0 viggodevries   (501) staff       (20)    24812 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_update.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2931 2022-03-29 09:58:26.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/stockalert_list.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.445398 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/comms/
--rw-r--r--   0 viggodevries   (501) staff       (20)     5968 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/comms/detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1926 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/comms/list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     7385 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/index.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     6980 2022-09-27 09:35:08.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/layout.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1359 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/login.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.449945 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1388 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/benefit_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1290 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/condition_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      246 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/metadata_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1348 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/offer_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     7275 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/offer_detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     8432 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/offer_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2078 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/progress.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      450 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/restrictions_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3499 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/step_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2615 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/summary.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.452577 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/
--rw-r--r--   0 viggodevries   (501) staff       (20)     7443 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/line_detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)    42683 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/order_detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     7925 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/order_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1488 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/shippingaddress_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2641 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/statistics.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.453661 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/pages/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1591 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/pages/delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3988 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/pages/index.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.454054 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/pages/messages/
--rw-r--r--   0 viggodevries   (501) staff       (20)      347 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/pages/messages/saved.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1274 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/pages/update.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.459356 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1018 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/advanced_search_modal.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1800 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/alert_messages.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      701 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2607 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/form_field.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      649 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/form_fields.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      604 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/form_fields_inline.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1145 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/pagination.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      982 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/product_images.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      252 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/stock_info.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.463348 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.463807 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/messages/
--rw-r--r--   0 viggodevries   (501) staff       (20)      224 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/messages/user_unlinked.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1366 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      929 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     5739 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2967 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_manage.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1570 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_user_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2764 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_user_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     4011 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_user_select.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.465847 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.466672 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/messages/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1512 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/messages/range_products_saved.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      373 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/messages/range_saved.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1436 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/range_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1854 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/range_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     4592 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/range_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     6882 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/range_product_list.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.467244 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1549 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/index.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.470719 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)      816 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/offer_report.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1510 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/open_basket_report.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1620 2022-03-29 09:58:26.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/order_report.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      780 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/product_report.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1439 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/submitted_basket_report.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1530 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/user_report.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      965 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/voucher_report.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.472280 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reviews/
--rw-r--r--   0 viggodevries   (501) staff       (20)     2374 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reviews/review_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     6653 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reviews/review_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3660 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reviews/review_update.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.474663 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.476800 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/messages/
--rw-r--r--   0 viggodevries   (501) staff       (20)      173 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/messages/band_created.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      162 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/messages/band_deleted.html
--rw-r--r--   0 viggodevries   (501) staff       (20)       58 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/messages/band_updated.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      147 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/messages/method_created.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      153 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/messages/method_deleted.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      153 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/messages/method_updated.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1837 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_band_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1505 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_band_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1369 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_based_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3895 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_based_detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1787 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_based_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2439 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_based_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      984 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/table.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.478721 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.479806 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/alerts/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1673 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/alerts/delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     4027 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/alerts/list.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.480155 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/alerts/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1297 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/alerts/partials/alert.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1653 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/alerts/update.html
--rw-r--r--   0 viggodevries   (501) staff       (20)    10499 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1877 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/index.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1068 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/table.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      122 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/user_row_actions.html
--rw-r--r--   0 viggodevries   (501) staff       (20)       92 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/user_row_checkbox.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.483320 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.484262 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)      845 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1591 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/partials/voucher_set_details_table.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2185 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     5729 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1802 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     9110 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1800 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_delete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     6285 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1799 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3612 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_list.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.485631 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/widgets/
--rw-r--r--   0 viggodevries   (501) staff       (20)      357 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/widgets/popup_response.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      524 2022-03-29 09:58:26.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/widgets/related_multiple_widget_wrapper.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1260 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/widgets/related_widget_wrapper.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      585 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/error.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.793831 django-oscar-3.2b0/src/oscar/templates/oscar/forms/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.486578 django-oscar-3.2b0/src/oscar/templates/oscar/forms/widgets/
--rw-r--r--   0 viggodevries   (501) staff       (20)      543 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/forms/widgets/date_time_picker.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      716 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/forms/widgets/image_input_widget.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2382 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/layout.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1144 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/layout_2_col.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1023 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/layout_3_col.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      173 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/login_forbidden.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.487715 django-oscar-3.2b0/src/oscar/templates/oscar/offer/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1948 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/offer/detail.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1413 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/offer/list.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1253 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/offer/range.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.794227 django-oscar-3.2b0/src/oscar/templates/oscar/order/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.488068 django-oscar-3.2b0/src/oscar/templates/oscar/order/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)     6350 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/order/partials/basket_totals.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.495217 django-oscar-3.2b0/src/oscar/templates/oscar/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1685 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/alert_messages.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      151 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/brand.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      172 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/extrascripts.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      216 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/footer.html
--rw-r--r--   0 viggodevries   (501) staff       (20)       79 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/footer_checkout.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      802 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/form.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     2323 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/form_field.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      595 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/form_fields.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      638 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/form_fields_inline.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      558 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/google_analytics.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      962 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/google_analytics_transaction.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1111 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/mini_basket.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3950 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/nav_accounts.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1187 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/nav_checkout.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3265 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/nav_primary.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1145 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/pagination.html
--rw-r--r--   0 viggodevries   (501) staff       (20)      303 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/partials/search.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.496644 django-oscar-3.2b0/src/oscar/templates/oscar/registration/
--rw-r--r--   0 viggodevries   (501) staff       (20)      929 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/registration/password_reset_complete.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1511 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/registration/password_reset_confirm.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1109 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/registration/password_reset_done.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     1109 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/registration/password_reset_form.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.497076 django-oscar-3.2b0/src/oscar/templates/oscar/search/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:14.795056 django-oscar-3.2b0/src/oscar/templates/oscar/search/indexes/
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.497408 django-oscar-3.2b0/src/oscar/templates/oscar/search/indexes/product/
--rw-r--r--   0 viggodevries   (501) staff       (20)       83 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/search/indexes/product/item_text.txt
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.497733 django-oscar-3.2b0/src/oscar/templates/oscar/search/partials/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1081 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templates/oscar/search/partials/facet.html
--rw-r--r--   0 viggodevries   (501) staff       (20)     3348 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templates/oscar/search/results.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.498210 django-oscar-3.2b0/src/oscar/templates/oscar/wishlists/
--rw-r--r--   0 viggodevries   (501) staff       (20)     1358 2022-06-24 08:22:22.000000 django-oscar-3.2b0/src/oscar/templates/oscar/wishlists/wishlist_detail.html
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.507792 django-oscar-3.2b0/src/oscar/templatetags/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templatetags/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1087 2022-06-24 08:22:10.000000 django-oscar-3.2b0/src/oscar/templatetags/basket_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3916 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templatetags/category_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1100 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templatetags/currency_filters.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      236 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templatetags/dashboard_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      229 2019-10-25 08:30:30.000000 django-oscar-3.2b0/src/oscar/templatetags/datetime_filters.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1383 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templatetags/display_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      578 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templatetags/form_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     2065 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templatetags/history_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4212 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templatetags/image_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1050 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templatetags/product_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      386 2019-10-25 08:30:30.000000 django-oscar-3.2b0/src/oscar/templatetags/purchase_info_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      787 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templatetags/reviews_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      882 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templatetags/shipping_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1657 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templatetags/sorting_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      145 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/templatetags/string_filters.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      283 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templatetags/url_tags.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      188 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/templatetags/wishlist_tags.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.510743 django-oscar-3.2b0/src/oscar/test/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/test/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      979 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/basket.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      767 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/test/contextmanagers.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.519437 django-oscar-3.2b0/src/oscar/test/factories/
--rw-r--r--   0 viggodevries   (501) staff       (20)     8827 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      868 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/address.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      710 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/basket.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3409 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/catalogue.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      627 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/contrib.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      915 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/customer.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      226 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/test/factories/models.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1590 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/offer.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4541 2022-06-02 10:02:25.000000 django-oscar-3.2b0/src/oscar/test/factories/order.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      825 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/partner.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      929 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/payment.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      852 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/urls.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      589 2019-10-25 08:30:30.000000 django-oscar-3.2b0/src/oscar/test/factories/utils.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      241 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/test/factories/views.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     1800 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/voucher.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      273 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/factories/wishlists.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3812 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/test/testcases.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     6205 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/test/utils.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.520935 django-oscar-3.2b0/src/oscar/utils/
--rw-r--r--   0 viggodevries   (501) staff       (20)        0 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/utils/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)       60 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/utils/deprecation.py
--rw-r--r--   0 viggodevries   (501) staff       (20)      215 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/utils/models.py
-drwxr-xr-x   0 viggodevries   (501) staff       (20)        0 2022-11-30 10:39:15.522300 django-oscar-3.2b0/src/oscar/views/
--rw-r--r--   0 viggodevries   (501) staff       (20)      795 2020-02-19 08:48:30.000000 django-oscar-3.2b0/src/oscar/views/__init__.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     3125 2019-10-01 13:53:56.000000 django-oscar-3.2b0/src/oscar/views/decorators.py
--rw-r--r--   0 viggodevries   (501) staff       (20)     4863 2022-02-09 19:38:42.000000 django-oscar-3.2b0/src/oscar/views/generic.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.268782 django-oscar-3.2b1/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4146 2022-03-31 19:33:51.000000 django-oscar-3.2b1/AUTHORS
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      120 2022-03-31 19:33:51.000000 django-oscar-3.2b1/CHANGELOG.rst
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      291 2022-03-31 19:33:51.000000 django-oscar-3.2b1/CONTRIBUTING.rst
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1589 2022-03-31 19:33:51.000000 django-oscar-3.2b1/LICENSE
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      179 2022-03-31 19:33:51.000000 django-oscar-3.2b1/MANIFEST.in
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12345 2022-12-06 08:59:33.268932 django-oscar-3.2b1/PKG-INFO
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12052 2022-10-19 18:33:57.000000 django-oscar-3.2b1/README.rst
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      471 2022-12-06 08:59:33.269668 django-oscar-3.2b1/setup.cfg
+-rwxr-xr-x   0 joeyjurjens   (501) staff       (20)     4582 2022-10-19 18:33:54.000000 django-oscar-3.2b1/setup.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.475244 django-oscar-3.2b1/src/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.542425 django-oscar-3.2b1/src/django_oscar.egg-info/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12345 2022-12-06 08:59:31.000000 django-oscar-3.2b1/src/django_oscar.egg-info/PKG-INFO
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    51547 2022-12-06 08:59:32.000000 django-oscar-3.2b1/src/django_oscar.egg-info/SOURCES.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        1 2022-12-06 08:59:31.000000 django-oscar-3.2b1/src/django_oscar.egg-info/dependency_links.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      757 2022-12-06 08:59:32.000000 django-oscar-3.2b1/src/django_oscar.egg-info/requires.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        6 2022-12-06 08:59:32.000000 django-oscar-3.2b1/src/django_oscar.egg-info/top_level.txt
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.543784 django-oscar-3.2b1/src/oscar/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2648 2022-12-06 08:50:30.000000 django-oscar-3.2b1/src/oscar/__init__.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.544677 django-oscar-3.2b1/src/oscar/apps/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/__init__.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.547782 django-oscar-3.2b1/src/oscar/apps/address/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       61 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    21333 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      638 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      225 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1049 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/forms.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.550802 django-oscar-3.2b1/src/oscar/apps/address/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4532 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      647 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/migrations/0002_auto_20150927_1547.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      977 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/migrations/0003_auto_20150927_1551.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      780 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/migrations/0004_auto_20170226_1122.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      825 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/migrations/0005_regenerate_user_address_hashes.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      452 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/migrations/0006_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      436 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/address/models.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.554174 django-oscar-3.2b1/src/oscar/apps/analytics/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       65 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3711 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      854 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      295 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/apps.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.555893 django-oscar-3.2b1/src/oscar/apps/analytics/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3988 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1208 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/migrations/0002_auto_20140827_1705.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      643 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/migrations/0003_auto_20200801_0817.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      828 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4057 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/receivers.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3277 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/reports.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      755 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/analytics/scores.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.562138 django-oscar-3.2b1/src/oscar/apps/basket/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       59 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    32805 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1153 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1271 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    13333 2022-10-20 08:05:44.000000 django-oscar-3.2b1/src/oscar/apps/basket/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2152 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/formsets.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      894 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/managers.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8264 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/middleware.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.567683 django-oscar-3.2b1/src/oscar/apps/basket/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3081 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1879 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0002_auto_20140827_1705.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      534 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0003_basket_vouchers.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      500 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0004_auto_20141007_2032.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      453 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0005_auto_20150604_1450.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      450 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0006_auto_20160111_1108.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      539 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0007_slugfield_noop.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      437 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0008_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      435 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0009_line_date_updated.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1149 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0010_convert_to_valid_json.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      493 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/0011_json_basket_option.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      654 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4550 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/reports.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      154 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/signals.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7166 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/basket/utils.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22520 2022-06-24 07:48:35.000000 django-oscar-3.2b1/src/oscar/apps/basket/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.576176 django-oscar-3.2b1/src/oscar/apps/catalogue/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       65 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    51436 2022-11-23 09:07:01.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3208 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2036 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1486 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/categories.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      142 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/exceptions.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1331 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/expressions.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4291 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/managers.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.588973 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    16465 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      535 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0002_auto_20150217_1221.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1457 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0003_data_migration_slugs.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      463 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0004_auto_20150217_1710.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      631 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0005_auto_20150604_1450.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      766 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0006_auto_20150807_1725.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      394 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0007_auto_20151207_1440.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      732 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0008_auto_20160304_1652.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      526 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0009_slugfield_noop.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1447 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0010_auto_20170420_0439.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      413 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0011_auto_20170422_1355.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      997 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0012_auto_20170609_1902.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      734 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0013_auto_20170821_1548.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1098 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0014_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      491 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0015_product_is_public.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1394 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0016_auto_20190327_0757.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      999 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0017_auto_20190816_0938.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1067 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0018_auto_20191220_0920.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1175 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0019_option_required.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      799 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0020_auto_20200801_0817.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1058 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0021_auto_20201005_0844.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      460 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0022_auto_20210210_0539.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      461 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0023_auto_20210824_1414.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5106 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0024_remove_duplicate_attributes.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      389 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0025_attribute_code_uniquetogether_constraint.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1825 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0026_predefined_product_options.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1961 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4683 2022-12-06 08:44:32.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/product_attributes.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1340 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/receivers.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.592495 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       80 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6908 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      584 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1197 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1623 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      191 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/managers.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.594756 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3402 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      481 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/migrations/0002_update_email_length.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      658 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/migrations/0003_auto_20160802_1358.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      580 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/migrations/0004_auto_20170429_0941.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      361 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       64 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/signals.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      288 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/utils.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4848 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/views.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4333 2022-11-23 09:07:01.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/search_handlers.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       66 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/signals.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6025 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/utils.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7732 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/catalogue/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.600926 django-oscar-3.2b1/src/oscar/apps/checkout/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       63 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1544 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/applicator.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2557 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1074 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/calculators.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      210 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/context_processors.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      523 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/exceptions.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3212 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12631 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/mixins.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    18473 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/session.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      134 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/signals.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1887 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/surcharges.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8369 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/utils.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    29119 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/checkout/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.605359 django-oscar-3.2b1/src/oscar/apps/communication/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       73 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7821 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      271 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2857 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/app.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      249 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      301 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/config.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      609 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/managers.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.607596 django-oscar-3.2b1/src/oscar/apps/communication/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4986 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      707 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/migrations/0002_reset_table_names.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      973 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/migrations/0003_remove_notification_category_make_code_uppercase.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      888 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/migrations/0004_auto_20200801_0817.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      591 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/models.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.608533 django-oscar-3.2b1/src/oscar/apps/communication/notifications/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/notifications/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      394 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/notifications/context_processors.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3424 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/notifications/views.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6183 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/communication/utils.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.614210 django-oscar-3.2b1/src/oscar/apps/customer/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       63 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8236 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/abstract_models.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.616006 django-oscar-3.2b1/src/oscar/apps/customer/alerts/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/alerts/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      546 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/alerts/receivers.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4900 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/alerts/utils.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4737 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/alerts/views.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10953 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2364 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/auth_backends.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    15245 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2279 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/history.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.619229 django-oscar-3.2b1/src/oscar/apps/customer/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5889 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      906 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/migrations/0002_auto_20150807_1725.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      507 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/migrations/0003_update_email_length.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      835 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/migrations/0004_email_save.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      411 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/migrations/0005_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      913 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/migrations/0006_auto_20190430_1736.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      660 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/migrations/0007_auto_20200801_0817.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3161 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/mixins.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      282 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      536 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/receivers.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       89 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/signals.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2463 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/utils.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    25756 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.619618 django-oscar-3.2b1/src/oscar/apps/customer/wishlists/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/customer/wishlists/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    15194 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/apps/customer/wishlists/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.623851 django-oscar-3.2b1/src/oscar/apps/dashboard/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       65 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2608 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/apps.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.629295 django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       91 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8509 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    15111 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6153 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/formsets.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      643 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/mixins.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4557 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/tables.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    37950 2022-06-24 07:48:38.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/views.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      746 2022-10-19 20:47:39.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/widgets.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.631554 django-oscar-3.2b1/src/oscar/apps/dashboard/communications/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      101 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/communications/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      856 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/communications/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3161 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/communications/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/communications/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2998 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/communications/views.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1921 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/menu.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3276 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/nav.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.633930 django-oscar-3.2b1/src/oscar/apps/dashboard/offers/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       78 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/offers/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2260 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/offers/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8610 2022-06-22 07:04:13.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/offers/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/offers/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      969 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/offers/reports.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    15297 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/offers/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.635994 django-oscar-3.2b1/src/oscar/apps/dashboard/orders/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       78 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/orders/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2084 2022-10-20 14:17:16.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/orders/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5770 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/orders/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    32430 2022-11-01 12:38:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/orders/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.638419 django-oscar-3.2b1/src/oscar/apps/dashboard/pages/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       76 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/pages/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1228 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/pages/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1708 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/pages/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4412 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/pages/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.639999 django-oscar-3.2b1/src/oscar/apps/dashboard/partners/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       89 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/partners/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2570 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/partners/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4785 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/partners/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10483 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/partners/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.642832 django-oscar-3.2b1/src/oscar/apps/dashboard/ranges/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       78 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/ranges/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1514 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/ranges/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2953 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/ranges/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/ranges/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8590 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/ranges/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.646005 django-oscar-3.2b1/src/oscar/apps/dashboard/reports/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       87 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reports/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      659 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reports/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1804 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reports/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reports/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3968 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reports/reports.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1232 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reports/utils.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2371 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reports/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.648399 django-oscar-3.2b1/src/oscar/apps/dashboard/reviews/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       87 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reviews/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1000 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reviews/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1451 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reviews/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reviews/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6634 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/reviews/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.650182 django-oscar-3.2b1/src/oscar/apps/dashboard/shipping/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       89 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/shipping/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2546 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/shipping/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      534 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/shipping/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5069 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/shipping/views.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      596 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/tables.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.652401 django-oscar-3.2b1/src/oscar/apps/dashboard/users/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       76 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/users/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1886 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/users/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1405 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/users/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1096 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/users/tables.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8081 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/users/views.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    11316 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.653959 django-oscar-3.2b1/src/oscar/apps/dashboard/vouchers/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       89 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/vouchers/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2580 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/vouchers/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4930 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/vouchers/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12398 2022-10-19 21:13:59.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/vouchers/views.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3127 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/dashboard/widgets.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.662420 django-oscar-3.2b1/src/oscar/apps/offer/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       57 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    41948 2022-10-19 21:04:04.000000 django-oscar-3.2b1/src/oscar/apps/offer/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1188 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3751 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/applicator.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      747 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12252 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/benefits.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10595 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/conditions.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1849 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/custom.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      835 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/managers.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.666661 django-oscar-3.2b1/src/oscar/apps/offer/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    15415 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      518 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/0002_auto_20151210_1053.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      537 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/0003_auto_20161120_1707.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      509 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/0004_auto_20170415_1518.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      857 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/0005_auto_20170423_1217.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      912 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/0006_auto_20170504_0616.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      561 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/0007_conditionaloffer_exclusive.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      731 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/0008_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      400 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/0009_auto_20200801_0817.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      602 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/0010_conditionaloffer_combinations.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1860 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2778 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/apps/offer/queryset.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1064 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/receivers.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2451 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/reports.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5456 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/results.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1008 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/utils.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2882 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/offer/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.671864 django-oscar-3.2b1/src/oscar/apps/order/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       57 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    40614 2022-10-20 14:17:16.000000 django-oscar-3.2b1/src/oscar/apps/order/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3039 2022-06-22 07:04:09.000000 django-oscar-3.2b1/src/oscar/apps/order/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      217 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      291 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/exceptions.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.677853 django-oscar-3.2b1/src/oscar/apps/order/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    24133 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      486 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0002_auto_20141007_2032.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      443 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0003_auto_20150113_1629.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      431 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0004_auto_20160111_1108.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      502 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0005_update_email_length.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1225 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0006_orderstatuschange.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1102 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0007_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      577 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0008_auto_20190301_1035.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1263 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0009_surcharge.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      549 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0010_auto_20200724_0909.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      624 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0011_auto_20200801_0817.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1146 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0012_convert_to_valid_json.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      492 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/0013_json_option_value.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      488 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/mixins.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2534 2022-10-20 14:17:16.000000 django-oscar-3.2b1/src/oscar/apps/order/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10391 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/processing.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2042 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/reports.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      167 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/signals.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12838 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/order/utils.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.683415 django-oscar-3.2b1/src/oscar/apps/partner/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       61 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    11566 2022-06-22 07:04:13.000000 django-oscar-3.2b1/src/oscar/apps/partner/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      407 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      287 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3207 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/availability.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       94 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/exceptions.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4886 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/importers.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.686700 django-oscar-3.2b1/src/oscar/apps/partner/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6571 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      500 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/migrations/0002_auto_20141007_2032.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      514 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/migrations/0003_auto_20150604_1450.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      528 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/migrations/0004_auto_20160107_1755.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      649 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/migrations/0005_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      842 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/migrations/0006_auto_20200724_0909.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      830 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2372 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/prices.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      920 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/receivers.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    13435 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/strategy.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       26 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/partner/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.689686 django-oscar-3.2b1/src/oscar/apps/payment/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       61 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    11260 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      676 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      225 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2650 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/bankcards.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1179 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/exceptions.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     9663 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/forms.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.692675 django-oscar-3.2b1/src/oscar/apps/payment/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4917 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      489 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/migrations/0002_auto_20141007_2032.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      492 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/migrations/0003_auto_20160323_1520.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      449 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/migrations/0004_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      797 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/migrations/0005_auto_20200801_0817.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      716 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/payment/models.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.697073 django-oscar-3.2b1/src/oscar/apps/search/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       59 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/search/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1195 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/search/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      246 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/search/context_processors.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4932 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/search/facets.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      395 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/search/features.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5242 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/search/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8144 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/search/search_handlers.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3760 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/search/search_indexes.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       59 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/search/signals.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2618 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/search/views.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.700425 django-oscar-3.2b1/src/oscar/apps/shipping/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       63 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7877 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      755 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      229 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5934 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/methods.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.702162 django-oscar-3.2b1/src/oscar/apps/shipping/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4307 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      671 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/migrations/0002_auto_20150604_1450.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1130 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/migrations/0003_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      636 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3688 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/repository.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1091 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/shipping/scales.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.706257 django-oscar-3.2b1/src/oscar/apps/voucher/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       61 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10115 2022-10-20 14:25:31.000000 django-oscar-3.2b1/src/oscar/apps/voucher/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1031 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      287 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/apps.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.710790 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3199 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      634 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0002_auto_20170418_2132.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      497 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0003_auto_20171212_0411.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1877 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0004_auto_20180228_0940.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      602 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0005_auto_20180402_1425.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      486 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0006_auto_20180413_0911.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      623 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0007_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1482 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0008_auto_20200801_0817.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1064 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0009_make_voucher_names_unique.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      810 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0010_auto_20210224_0712.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      634 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      661 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/receivers.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1448 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/reports.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1224 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/voucher/utils.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.714194 django-oscar-3.2b1/src/oscar/apps/wishlists/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       65 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5917 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/abstract_models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      327 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/admin.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      602 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/apps.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      817 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/forms.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      719 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/formsets.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.716162 django-oscar-3.2b1/src/oscar/apps/wishlists/migrations/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2782 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/migrations/0001_initial.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      390 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/migrations/0002_auto_20160111_1108.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      448 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/migrations/0003_auto_20181115_1953.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      891 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/migrations/0004_auto_20220328_0939.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/migrations/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      571 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1805 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/apps/wishlists/views.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3394 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/config.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.721069 django-oscar-3.2b1/src/oscar/core/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1254 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/ajax.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4972 2022-10-20 09:12:44.000000 django-oscar-3.2b1/src/oscar/core/application.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4320 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/compat.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1130 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/context_processors.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5406 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/customisation.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      996 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/decorators.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      167 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/exceptions.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10885 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/loading.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.721776 django-oscar-3.2b1/src/oscar/core/logging/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      467 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/logging/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      330 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/logging/formatters.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2285 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/prices.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2070 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/thumbnails.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7029 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/utils.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4249 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/core/validators.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7714 2022-10-20 14:17:16.000000 django-oscar-3.2b1/src/oscar/defaults.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.723051 django-oscar-3.2b1/src/oscar/forms/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/forms/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1003 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/forms/fields.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4491 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/forms/mixins.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10101 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/forms/widgets.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.515909 django-oscar-3.2b1/src/oscar/locale/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.484909 django-oscar-3.2b1/src/oscar/locale/am_ET/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.723807 django-oscar-3.2b1/src/oscar/locale/am_ET/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      450 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/am_ET/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263752 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/am_ET/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.485183 django-oscar-3.2b1/src/oscar/locale/ar/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.727168 django-oscar-3.2b1/src/oscar/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   123176 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   317447 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.485458 django-oscar-3.2b1/src/oscar/locale/ar_EG/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.729847 django-oscar-3.2b1/src/oscar/locale/ar_EG/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      529 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/ar_EG/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264715 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ar_EG/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.485758 django-oscar-3.2b1/src/oscar/locale/ar_SA/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.732423 django-oscar-3.2b1/src/oscar/locale/ar_SA/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      538 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/ar_SA/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264724 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ar_SA/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.486044 django-oscar-3.2b1/src/oscar/locale/az/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.736349 django-oscar-3.2b1/src/oscar/locale/az/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2322 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/az/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264417 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/az/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.486322 django-oscar-3.2b1/src/oscar/locale/az_AZ/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.739275 django-oscar-3.2b1/src/oscar/locale/az_AZ/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      456 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/az_AZ/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263758 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/az_AZ/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.486624 django-oscar-3.2b1/src/oscar/locale/bg/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.742028 django-oscar-3.2b1/src/oscar/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      435 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263737 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.486896 django-oscar-3.2b1/src/oscar/locale/bg_BG/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.744597 django-oscar-3.2b1/src/oscar/locale/bg_BG/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2075 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/bg_BG/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264443 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/bg_BG/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.487168 django-oscar-3.2b1/src/oscar/locale/bn/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.747542 django-oscar-3.2b1/src/oscar/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      433 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/bn/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263735 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/bn/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.487445 django-oscar-3.2b1/src/oscar/locale/bn_BD/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.751230 django-oscar-3.2b1/src/oscar/locale/bn_BD/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4913 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/bn_BD/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   265806 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/bn_BD/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.487721 django-oscar-3.2b1/src/oscar/locale/ca/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.754747 django-oscar-3.2b1/src/oscar/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    78491 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   292845 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.487994 django-oscar-3.2b1/src/oscar/locale/ca_ES/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.757797 django-oscar-3.2b1/src/oscar/locale/ca_ES/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      447 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/ca_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263749 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ca_ES/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.488269 django-oscar-3.2b1/src/oscar/locale/cmn/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.760711 django-oscar-3.2b1/src/oscar/locale/cmn/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      439 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/cmn/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263520 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/cmn/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.488554 django-oscar-3.2b1/src/oscar/locale/crh/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.763733 django-oscar-3.2b1/src/oscar/locale/crh/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      442 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/crh/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263744 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/crh/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.488837 django-oscar-3.2b1/src/oscar/locale/cs/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.766379 django-oscar-3.2b1/src/oscar/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      531 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264323 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.489117 django-oscar-3.2b1/src/oscar/locale/cs_CZ/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.769710 django-oscar-3.2b1/src/oscar/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   127509 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   312325 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/cs_CZ/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.489395 django-oscar-3.2b1/src/oscar/locale/cy/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.773124 django-oscar-3.2b1/src/oscar/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2325 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/cy/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264725 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/cy/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.489810 django-oscar-3.2b1/src/oscar/locale/da/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.777036 django-oscar-3.2b1/src/oscar/locale/da/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   124542 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   308000 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.490177 django-oscar-3.2b1/src/oscar/locale/de/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.780997 django-oscar-3.2b1/src/oscar/locale/de/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   135420 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   316492 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.490531 django-oscar-3.2b1/src/oscar/locale/el/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.785657 django-oscar-3.2b1/src/oscar/locale/el/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      431 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263733 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.490835 django-oscar-3.2b1/src/oscar/locale/el_GR/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.789052 django-oscar-3.2b1/src/oscar/locale/el_GR/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    93691 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/el_GR/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   312779 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/el_GR/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.491113 django-oscar-3.2b1/src/oscar/locale/en/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.791816 django-oscar-3.2b1/src/oscar/locale/en/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      337 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   254164 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.491392 django-oscar-3.2b1/src/oscar/locale/en_AU/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.795260 django-oscar-3.2b1/src/oscar/locale/en_AU/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      451 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/en_AU/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263753 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/en_AU/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.491668 django-oscar-3.2b1/src/oscar/locale/en_US/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.799729 django-oscar-3.2b1/src/oscar/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   134499 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/en_US/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   311249 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/en_US/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.491951 django-oscar-3.2b1/src/oscar/locale/es/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.803365 django-oscar-3.2b1/src/oscar/locale/es/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   134975 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   317218 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.492223 django-oscar-3.2b1/src/oscar/locale/es_AR/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.806053 django-oscar-3.2b1/src/oscar/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3682 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   265150 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.492493 django-oscar-3.2b1/src/oscar/locale/es_CL/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.808857 django-oscar-3.2b1/src/oscar/locale/es_CL/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      744 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/es_CL/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264132 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/es_CL/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.492772 django-oscar-3.2b1/src/oscar/locale/es_MX/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.812085 django-oscar-3.2b1/src/oscar/locale/es_MX/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   135463 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/es_MX/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   312361 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/es_MX/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.493048 django-oscar-3.2b1/src/oscar/locale/et/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.814836 django-oscar-3.2b1/src/oscar/locale/et/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   138542 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   312233 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.493356 django-oscar-3.2b1/src/oscar/locale/eu/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.818005 django-oscar-3.2b1/src/oscar/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    62176 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   286152 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.493741 django-oscar-3.2b1/src/oscar/locale/fa/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.822326 django-oscar-3.2b1/src/oscar/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   160839 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   340182 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.494029 django-oscar-3.2b1/src/oscar/locale/fa_IR/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.824869 django-oscar-3.2b1/src/oscar/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6929 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   266591 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/fa_IR/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.494319 django-oscar-3.2b1/src/oscar/locale/fi/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.828209 django-oscar-3.2b1/src/oscar/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   139572 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   314910 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.494822 django-oscar-3.2b1/src/oscar/locale/fr/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.831564 django-oscar-3.2b1/src/oscar/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   151694 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   326460 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.495309 django-oscar-3.2b1/src/oscar/locale/fr_CA/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.834440 django-oscar-3.2b1/src/oscar/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      498 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/fr_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264021 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/fr_CA/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.495829 django-oscar-3.2b1/src/oscar/locale/fr_FR/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.837355 django-oscar-3.2b1/src/oscar/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      498 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264021 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.496337 django-oscar-3.2b1/src/oscar/locale/gu/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.839698 django-oscar-3.2b1/src/oscar/locale/gu/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      434 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/gu/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263736 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/gu/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.496900 django-oscar-3.2b1/src/oscar/locale/gu_IN/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.842095 django-oscar-3.2b1/src/oscar/locale/gu_IN/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      448 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/gu_IN/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263750 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/gu_IN/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.497387 django-oscar-3.2b1/src/oscar/locale/he/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.847083 django-oscar-3.2b1/src/oscar/locale/he/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   150328 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   329074 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.497742 django-oscar-3.2b1/src/oscar/locale/hi/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.850460 django-oscar-3.2b1/src/oscar/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    11559 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/hi/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   269389 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hi/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.498042 django-oscar-3.2b1/src/oscar/locale/hi_IN/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.853590 django-oscar-3.2b1/src/oscar/locale/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    31241 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hi_IN/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   280974 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hi_IN/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.498417 django-oscar-3.2b1/src/oscar/locale/hr/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.858499 django-oscar-3.2b1/src/oscar/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    93479 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   297656 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.498853 django-oscar-3.2b1/src/oscar/locale/hu/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.861408 django-oscar-3.2b1/src/oscar/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      435 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263737 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.499208 django-oscar-3.2b1/src/oscar/locale/hu_HU/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.864194 django-oscar-3.2b1/src/oscar/locale/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   107539 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hu_HU/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   305678 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hu_HU/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.499569 django-oscar-3.2b1/src/oscar/locale/hy/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.866713 django-oscar-3.2b1/src/oscar/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7072 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hy/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   266571 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hy/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.499864 django-oscar-3.2b1/src/oscar/locale/hy_AM/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.869047 django-oscar-3.2b1/src/oscar/locale/hy_AM/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      450 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/hy_AM/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263752 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/hy_AM/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.500188 django-oscar-3.2b1/src/oscar/locale/id/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.872499 django-oscar-3.2b1/src/oscar/locale/id/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   133492 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   312290 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.500652 django-oscar-3.2b1/src/oscar/locale/id_ID/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.875114 django-oscar-3.2b1/src/oscar/locale/id_ID/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      447 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/id_ID/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263528 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/id_ID/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.501184 django-oscar-3.2b1/src/oscar/locale/is_IS/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.877689 django-oscar-3.2b1/src/oscar/locale/is_IS/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      473 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/is_IS/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263775 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/is_IS/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.501551 django-oscar-3.2b1/src/oscar/locale/it/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.881529 django-oscar-3.2b1/src/oscar/locale/it/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   146270 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   322218 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.501972 django-oscar-3.2b1/src/oscar/locale/ja/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.885074 django-oscar-3.2b1/src/oscar/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   151703 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   327354 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.502389 django-oscar-3.2b1/src/oscar/locale/ka_GE/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.888716 django-oscar-3.2b1/src/oscar/locale/ka_GE/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    71671 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ka_GE/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   305689 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ka_GE/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.502685 django-oscar-3.2b1/src/oscar/locale/ko/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.893158 django-oscar-3.2b1/src/oscar/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   135121 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   316766 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.502981 django-oscar-3.2b1/src/oscar/locale/lt/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.898229 django-oscar-3.2b1/src/oscar/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   130728 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   314773 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.503278 django-oscar-3.2b1/src/oscar/locale/lv/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.901897 django-oscar-3.2b1/src/oscar/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3838 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264981 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.503643 django-oscar-3.2b1/src/oscar/locale/ml/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.905743 django-oscar-3.2b1/src/oscar/locale/ml/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      435 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/locale/ml/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263737 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ml/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.503939 django-oscar-3.2b1/src/oscar/locale/mr/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.909081 django-oscar-3.2b1/src/oscar/locale/mr/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5262 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/mr/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   266318 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/mr/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.504227 django-oscar-3.2b1/src/oscar/locale/ms/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.911554 django-oscar-3.2b1/src/oscar/locale/ms/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      424 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/ms/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263505 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ms/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.504736 django-oscar-3.2b1/src/oscar/locale/nb_NO/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.914232 django-oscar-3.2b1/src/oscar/locale/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    36393 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   276456 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/nb_NO/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.505032 django-oscar-3.2b1/src/oscar/locale/nl/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.916983 django-oscar-3.2b1/src/oscar/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   153184 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   323218 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.505446 django-oscar-3.2b1/src/oscar/locale/pl/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.920765 django-oscar-3.2b1/src/oscar/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   135695 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   316940 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.505867 django-oscar-3.2b1/src/oscar/locale/pt/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.923494 django-oscar-3.2b1/src/oscar/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      487 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264010 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.506218 django-oscar-3.2b1/src/oscar/locale/pt_BR/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.927042 django-oscar-3.2b1/src/oscar/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   142706 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   319650 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.506550 django-oscar-3.2b1/src/oscar/locale/pt_PT/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.930494 django-oscar-3.2b1/src/oscar/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   146645 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   320816 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.507021 django-oscar-3.2b1/src/oscar/locale/ro_RO/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.933202 django-oscar-3.2b1/src/oscar/locale/ro_RO/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   106322 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ro_RO/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   302696 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ro_RO/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.507440 django-oscar-3.2b1/src/oscar/locale/ru/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.936660 django-oscar-3.2b1/src/oscar/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    13779 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   270527 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.507968 django-oscar-3.2b1/src/oscar/locale/ru@petr1708/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.939463 django-oscar-3.2b1/src/oscar/locale/ru@petr1708/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      609 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/ru@petr1708/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264353 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ru@petr1708/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.508264 django-oscar-3.2b1/src/oscar/locale/ru_RU/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.943276 django-oscar-3.2b1/src/oscar/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   179538 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   357671 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/ru_RU/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.508549 django-oscar-3.2b1/src/oscar/locale/sk/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.947328 django-oscar-3.2b1/src/oscar/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   126358 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   312056 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.508822 django-oscar-3.2b1/src/oscar/locale/sk_SK/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.950181 django-oscar-3.2b1/src/oscar/locale/sk_SK/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      524 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/sk_SK/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264268 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sk_SK/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.509122 django-oscar-3.2b1/src/oscar/locale/sl_SI/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.953760 django-oscar-3.2b1/src/oscar/locale/sl_SI/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   125966 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sl_SI/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   309780 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sl_SI/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.509388 django-oscar-3.2b1/src/oscar/locale/sr/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.958250 django-oscar-3.2b1/src/oscar/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   127942 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   310850 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.509654 django-oscar-3.2b1/src/oscar/locale/sv/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.962295 django-oscar-3.2b1/src/oscar/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    94590 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   297973 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.509923 django-oscar-3.2b1/src/oscar/locale/sv_SE/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.964839 django-oscar-3.2b1/src/oscar/locale/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      448 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/sv_SE/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263750 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sv_SE/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.510194 django-oscar-3.2b1/src/oscar/locale/sw/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.967289 django-oscar-3.2b1/src/oscar/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      433 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263735 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.510476 django-oscar-3.2b1/src/oscar/locale/sw_KE/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.969355 django-oscar-3.2b1/src/oscar/locale/sw_KE/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      447 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/locale/sw_KE/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263749 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/sw_KE/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.510740 django-oscar-3.2b1/src/oscar/locale/th/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.971868 django-oscar-3.2b1/src/oscar/locale/th/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      423 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263504 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.511016 django-oscar-3.2b1/src/oscar/locale/th_TH/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.975257 django-oscar-3.2b1/src/oscar/locale/th_TH/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    13390 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/th_TH/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   270546 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/th_TH/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.511289 django-oscar-3.2b1/src/oscar/locale/tr/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.978032 django-oscar-3.2b1/src/oscar/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   131714 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   314258 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.511555 django-oscar-3.2b1/src/oscar/locale/tr_CY/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.980478 django-oscar-3.2b1/src/oscar/locale/tr_CY/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      447 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/tr_CY/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263749 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/tr_CY/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.511819 django-oscar-3.2b1/src/oscar/locale/tr_TR/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.982965 django-oscar-3.2b1/src/oscar/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5440 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   265526 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/tr_TR/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.512086 django-oscar-3.2b1/src/oscar/locale/uk/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.986122 django-oscar-3.2b1/src/oscar/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   174600 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   352968 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.512362 django-oscar-3.2b1/src/oscar/locale/uk_UA/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.988976 django-oscar-3.2b1/src/oscar/locale/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1289 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/uk_UA/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   264763 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/uk_UA/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.512817 django-oscar-3.2b1/src/oscar/locale/vi/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.992596 django-oscar-3.2b1/src/oscar/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   139945 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   322890 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.513757 django-oscar-3.2b1/src/oscar/locale/zh/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.002653 django-oscar-3.2b1/src/oscar/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7225 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   265431 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.513136 django-oscar-3.2b1/src/oscar/locale/zh-Hans/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.996778 django-oscar-3.2b1/src/oscar/locale/zh-Hans/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   130881 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh-Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   305752 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh-Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.513451 django-oscar-3.2b1/src/oscar/locale/zh-Hant/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.999846 django-oscar-3.2b1/src/oscar/locale/zh-Hant/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22350 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh-Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   270580 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh-Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.514334 django-oscar-3.2b1/src/oscar/locale/zh_CN/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.009702 django-oscar-3.2b1/src/oscar/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1960 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   265285 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.514055 django-oscar-3.2b1/src/oscar/locale/zh_CN.GB2312/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.005719 django-oscar-3.2b1/src/oscar/locale/zh_CN.GB2312/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      463 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/zh_CN.GB2312/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263544 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh_CN.GB2312/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.514619 django-oscar-3.2b1/src/oscar/locale/zh_HK/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.012331 django-oscar-3.2b1/src/oscar/locale/zh_HK/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10473 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/zh_HK/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   266468 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh_HK/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.515198 django-oscar-3.2b1/src/oscar/locale/zh_SG/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.014704 django-oscar-3.2b1/src/oscar/locale/zh_SG/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      444 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/zh_SG/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263525 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh_SG/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.516198 django-oscar-3.2b1/src/oscar/locale/zh_TW/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.020651 django-oscar-3.2b1/src/oscar/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   112036 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   299815 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.515581 django-oscar-3.2b1/src/oscar/locale/zh_TW.Big5/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.017383 django-oscar-3.2b1/src/oscar/locale/zh_TW.Big5/LC_MESSAGES/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      459 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/locale/zh_TW.Big5/LC_MESSAGES/django.mo
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   263540 2022-12-01 08:59:41.000000 django-oscar-3.2b1/src/oscar/locale/zh_TW.Big5/LC_MESSAGES/django.po
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.022498 django-oscar-3.2b1/src/oscar/management/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/__init__.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.027125 django-oscar-3.2b1/src/oscar/management/commands/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      372 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_calculate_scores.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1727 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_cleanup_alerts.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1054 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_find_duplicate_emails.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1123 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_fork_app.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1787 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_fork_statics.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1090 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_generate_email_content.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1413 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_import_catalogue.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      797 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_import_catalogue_images.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2214 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_populate_countries.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      791 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_send_alerts.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      687 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/management/commands/oscar_update_product_ratings.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.027505 django-oscar-3.2b1/src/oscar/models/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/models/__init__.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.028536 django-oscar-3.2b1/src/oscar/models/fields/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4366 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/models/fields/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7070 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/models/fields/autoslugfield.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      466 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/models/fields/slugfield.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.517782 django-oscar-3.2b1/src/oscar/static/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.029082 django-oscar-3.2b1/src/oscar/static/oscar/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      655 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/README.rst
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.031550 django-oscar-3.2b1/src/oscar/static/oscar/css/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   295633 2022-12-06 08:59:10.000000 django-oscar-3.2b1/src/oscar/static/oscar/css/dashboard.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   508684 2022-12-06 08:59:10.000000 django-oscar-3.2b1/src/oscar/static/oscar/css/dashboard.css.map
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    16792 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/css/select2-bootstrap.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   294186 2022-12-06 08:59:13.000000 django-oscar-3.2b1/src/oscar/static/oscar/css/styles.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   509158 2022-12-06 08:59:13.000000 django-oscar-3.2b1/src/oscar/static/oscar/css/styles.css.map
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1150 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/favicon.ico
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.032928 django-oscar-3.2b1/src/oscar/static/oscar/img/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8777 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/glyphicons-halflings-white.png
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12799 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/glyphicons-halflings.png
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3555 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/image_not_found.jpg
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.036256 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/
+-rwxr-xr-x   0 joeyjurjens   (501) staff       (20)      124 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/black.png
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.037015 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/dashboard/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      955 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/dashboard/bg_subtle_dots.png
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5469 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/dashboard/logo_oscar.png
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      331 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon-addlink.svg
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      380 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon-changelink.svg
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      392 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon-deletelink.svg
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1096 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_arrow_down.png
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1109 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_arrow_left.png
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2990 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_minus.png
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3077 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_plus.png
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1224 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_slider_left.png
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1218 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_slider_right.png
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1306 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/img/ui/nav_sprite.png
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.520164 django-oscar-3.2b1/src/oscar/static/oscar/js/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.037998 django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   230599 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4/bootstrap.bundle.js
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    83376 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4/bootstrap.bundle.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.040366 django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4-datetimepicker/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   369018 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4-datetimepicker/moment-with-locales.min.js
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    11967 2022-12-06 08:57:56.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4-datetimepicker/tempusdominus-bootstrap-4.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    61593 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4-datetimepicker/tempusdominus-bootstrap-4.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.041074 django-oscar-3.2b1/src/oscar/static/oscar/js/inputmask/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    99426 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/inputmask/jquery.inputmask.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.041691 django-oscar-3.2b1/src/oscar/static/oscar/js/jquery/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    89501 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/jquery/jquery.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.042239 django-oscar-3.2b1/src/oscar/static/oscar/js/jquery-sortable/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     9699 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/jquery-sortable/jquery-sortable-min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.042582 django-oscar-3.2b1/src/oscar/static/oscar/js/mousewheel/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8267 2022-12-06 08:57:56.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/mousewheel/jquery.mousewheel.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.044035 django-oscar-3.2b1/src/oscar/static/oscar/js/oscar/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5427 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/oscar/RelatedObjectLookups.js
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    19639 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/oscar/dashboard.js
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      582 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/oscar/popup_response.js
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12791 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/oscar/ui.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.044632 django-oscar-3.2b1/src/oscar/static/oscar/js/select2/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    14966 2022-12-06 08:57:56.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/select2/select2.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    70851 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/select2/select2.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.045574 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.520431 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/icons/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.046775 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/icons/default/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    65274 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/icons/default/icons.min.js
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6507 2022-12-06 08:57:56.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/jquery.tinymce.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.520808 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/models/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.047283 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/models/dom/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    95742 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/models/dom/model.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.526245 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.047956 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/advlist/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3376 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/advlist/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.048341 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/anchor/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2537 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/anchor/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.048774 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/autolink/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3060 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/autolink/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.049185 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/autoresize/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2074 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/autoresize/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.049529 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/autosave/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3257 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/autosave/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.049984 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/charmap/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10981 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/charmap/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.050386 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/code/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      877 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/code/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.050901 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/codesample/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    48043 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/codesample/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.051493 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/directionality/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4360 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/directionality/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.052101 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/emoticons/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.053881 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/emoticons/js/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   416095 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/emoticons/js/emojiimages.min.js
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   192856 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/emoticons/js/emojis.min.js
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6325 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/emoticons/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.054820 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/fullscreen/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    14630 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/fullscreen/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.055417 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/help/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    13080 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/help/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.055907 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/image/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    19054 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/image/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.056466 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/importcss/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4036 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/importcss/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.056901 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/insertdatetime/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2911 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/insertdatetime/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.057334 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/link/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    15087 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/link/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.057809 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/lists/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22702 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/lists/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.058330 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/media/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    16306 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/media/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.058786 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/nonbreaking/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1416 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/nonbreaking/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.059320 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/pagebreak/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1503 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/pagebreak/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.059841 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/preview/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1718 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/preview/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.060330 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/quickbars/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4908 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/quickbars/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.061012 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/save/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1592 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/save/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.061501 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/searchreplace/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    13265 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/searchreplace/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.061791 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/table/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    46912 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/table/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.062252 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/template/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8103 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/template/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.062675 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/visualblocks/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1230 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/visualblocks/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.063025 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/visualchars/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5172 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/visualchars/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.063357 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/wordcount/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    11913 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/wordcount/plugin.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.527552 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.527393 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.063701 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/dark/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1216 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/dark/content.min.css
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.064122 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/default/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1149 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/default/content.min.css
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.064375 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/document/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1248 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/document/content.min.css
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.064619 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1149 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5/content.min.css
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.064899 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5-dark/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1219 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5-dark/content.min.css
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.065384 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/writer/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1170 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/writer/content.min.css
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.528118 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.066939 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22753 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/content.inline.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22812 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/content.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    62379 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/skin.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      508 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/skin.shadowdom.min.css
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.068443 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22753 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/content.inline.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22423 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/content.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    62439 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/skin.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      508 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.069853 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22753 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/content.inline.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22812 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/content.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    64589 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/skin.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      508 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/skin.shadowdom.min.css
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.071212 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22753 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/content.inline.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    22423 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/content.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    64476 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/skin.min.css
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      508 2022-12-06 08:57:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/skin.shadowdom.min.css
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.528377 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/themes/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.071472 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/themes/silver/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   345342 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/themes/silver/theme.min.js
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   396486 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/tinymce.min.js
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.073151 django-oscar-3.2b1/src/oscar/static/oscar/scss/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      610 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/README.rst
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      612 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/_alerts.scss
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.076101 django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2599 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/base.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      387 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/buttons.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1074 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/catalogue.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      985 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/forms.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1934 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/index.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1209 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/navbar.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      825 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/tables.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      588 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/variables.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      647 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard.scss
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.078850 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1556 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/checkout.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      811 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/forms.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1260 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/header.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      367 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/layout.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1508 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/plugins.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1243 2022-10-19 18:33:57.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/product_lists.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1363 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/product_page.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1001 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/reviews.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      255 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/type.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      916 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/page/variables.scss
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      675 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/static/oscar/scss/styles.scss
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.082284 django-oscar-3.2b1/src/oscar/static/oscar/webfonts/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   181264 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   105112 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    60236 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    24028 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   389948 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)   154840 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10084 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4776 2022-12-06 08:57:58.000000 django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.529588 django-oscar-3.2b1/src/oscar/templates/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.082542 django-oscar-3.2b1/src/oscar/templates/flatpages/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      916 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/flatpages/default.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.086766 django-oscar-3.2b1/src/oscar/templates/oscar/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      345 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/403.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      328 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/404.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      676 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/500.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2151 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/base.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.087078 django-oscar-3.2b1/src/oscar/templates/oscar/basket/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1029 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/basket/basket.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.089757 django-oscar-3.2b1/src/oscar/templates/oscar/basket/messages/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      404 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/basket/messages/addition.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      153 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/basket/messages/line_restored.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      142 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/basket/messages/line_saved.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      778 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/basket/messages/new_total.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      145 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/basket/messages/offer_gained.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      150 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/basket/messages/offer_lost.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.091807 django-oscar-3.2b1/src/oscar/templates/oscar/basket/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12074 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/basket/partials/basket_content.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2264 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/basket/partials/basket_quick.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    12269 2022-10-27 08:22:58.000000 django-oscar-3.2b1/src/oscar/templates/oscar/basket/partials/basket_totals.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.095467 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4234 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/browse.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1596 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/category.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7848 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/detail.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.101332 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1591 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/add_to_basket_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      639 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/add_to_basket_form_compact.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2812 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/add_to_wishlist.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2468 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/gallery.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1808 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/product.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2624 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/review.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      956 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/stock_record.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.103541 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.104113 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1007 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/partials/review_stars.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1475 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/review_detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2347 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/review_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1828 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/review_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      777 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/review_product.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.110752 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6906 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/checkout.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2174 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/gateway.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1607 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/layout.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2684 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/nav.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1358 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/payment_details.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1397 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/preview.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4613 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/shipping_address.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2616 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/shipping_methods.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8334 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/thank_you.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1185 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/user_address_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1182 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/checkout/user_address_form.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.531416 django-oscar-3.2b1/src/oscar/templates/oscar/communication/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.112059 django-oscar-3.2b1/src/oscar/templates/oscar/communication/email/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1195 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/email/email_detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      924 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/email/email_list.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.122418 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8093 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/base.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      227 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/base.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      837 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_email_changed_body.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      550 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_email_changed_body.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      126 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_email_changed_subject.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2686 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_order_placed_body.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1075 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_order_placed_body.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      110 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_order_placed_subject.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      827 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_password_changed_body.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      481 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_password_changed_body.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      117 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_password_changed_subject.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      643 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_password_reset_body.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      434 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_password_reset_body.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      119 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_password_reset_subject.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1129 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_product_alert_body.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      847 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_product_alert_body.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      832 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_product_alert_confirmation_body.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      590 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_product_alert_confirmation_body.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       88 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_product_alert_confirmation_subject.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      120 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_product_alert_subject.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       62 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_registration_body.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       55 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_registration_body.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_registration_sms.txt
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       55 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_registration_subject.txt
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.123138 django-oscar-3.2b1/src/oscar/templates/oscar/communication/notifications/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1325 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/notifications/detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3425 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/communication/notifications/list.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.124623 django-oscar-3.2b1/src/oscar/templates/oscar/customer/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.125650 django-oscar-3.2b1/src/oscar/templates/oscar/customer/address/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      740 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/address/address_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      393 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/address/address_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3160 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/address/address_list.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.127077 django-oscar-3.2b1/src/oscar/templates/oscar/customer/alerts/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1774 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/alerts/alert_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       44 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/alerts/form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      176 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/alerts/message.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      135 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/alerts/message_subject.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4142 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/anon_order.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1123 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/baseaccountpage.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.127424 django-oscar-3.2b1/src/oscar/templates/oscar/customer/history/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      481 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/history/recently_viewed_products.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1830 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/login_registration.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.128107 django-oscar-3.2b1/src/oscar/templates/oscar/customer/order/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7997 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/order/order_detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2911 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/order/order_list.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.128508 django-oscar-3.2b1/src/oscar/templates/oscar/customer/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1326 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/partials/standard_tabs.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.129981 django-oscar-3.2b1/src/oscar/templates/oscar/customer/profile/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      199 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/profile/change_password_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1269 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/profile/profile.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      942 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/profile/profile_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      191 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/profile/profile_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1205 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/registration.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.132130 django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1434 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/wishlists_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1518 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/wishlists_delete_product.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6262 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/wishlists_detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2300 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/wishlists_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2493 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/wishlists_list.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.134727 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      250 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/base.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.146582 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2523 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7698 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1340 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      839 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_row_actions.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      144 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_row_name.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      144 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_row_option_summary.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1629 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/category_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6099 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/category_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1724 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/category_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1373 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/category_row_actions.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.147323 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/messages/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1472 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/messages/product_saved.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2313 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/option_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4051 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/option_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1183 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/option_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      791 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/option_row_actions.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      128 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/option_row_name.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1570 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_class_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8333 2022-11-01 12:09:57.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_class_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3100 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_class_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2207 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3687 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      897 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_row_actions.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      456 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_row_image.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       89 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_row_stockrecords.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      122 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_row_title.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       91 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_row_variants.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    24812 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_update.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2931 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/stockalert_list.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.148740 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/comms/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5968 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/comms/detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1926 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/comms/list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7385 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/index.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6980 2022-06-22 07:04:09.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/layout.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1359 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/login.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.154275 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1388 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/benefit_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1290 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/condition_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      246 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/metadata_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1348 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/offer_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7275 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/offer_detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8432 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/offer_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2078 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/progress.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      450 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/restrictions_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3499 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/step_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2615 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/summary.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.157748 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7443 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/line_detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    42683 2022-10-20 14:17:16.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/order_detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     7925 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/order_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1488 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/shippingaddress_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2641 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/statistics.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.159448 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/pages/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1591 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/pages/delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3988 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/pages/index.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.159949 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/pages/messages/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      347 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/pages/messages/saved.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1274 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/pages/update.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.164768 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1018 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/advanced_search_modal.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1800 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/alert_messages.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      701 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2607 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/form_field.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      649 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/form_fields.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      604 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/form_fields_inline.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1145 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/pagination.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      982 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/product_images.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      252 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/stock_info.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.167892 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.168220 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/messages/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      224 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/messages/user_unlinked.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1366 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      929 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5739 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2967 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_manage.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1570 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_user_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2764 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_user_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4011 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_user_select.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.170112 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.171131 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/messages/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1512 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/messages/range_products_saved.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      373 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/messages/range_saved.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1436 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/range_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1854 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/range_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4592 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/range_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6882 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/range_product_list.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.171643 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1549 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/index.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.174568 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      816 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/offer_report.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1510 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/open_basket_report.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1620 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/order_report.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      780 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/product_report.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1439 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/submitted_basket_report.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1530 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/user_report.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      965 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/voucher_report.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.175716 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reviews/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2374 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reviews/review_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6653 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reviews/review_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3660 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reviews/review_update.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.178440 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.181716 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/messages/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      173 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/messages/band_created.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      162 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/messages/band_deleted.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       58 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/messages/band_updated.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      147 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/messages/method_created.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      153 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/messages/method_deleted.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      153 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/messages/method_updated.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1837 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_band_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1505 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_band_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1369 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_based_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3895 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_based_detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1787 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_based_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2439 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_based_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      984 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/table.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.183878 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.185130 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/alerts/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1673 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/alerts/delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4027 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/alerts/list.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.185525 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/alerts/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1297 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/alerts/partials/alert.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1653 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/alerts/update.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)    10499 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1877 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/index.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1068 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/table.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      122 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/user_row_actions.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       92 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/user_row_checkbox.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.188727 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.189673 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      845 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1591 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/partials/voucher_set_details_table.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2185 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     5729 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1802 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     9110 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1800 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_delete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6285 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1799 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3612 2022-10-19 21:07:02.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_list.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.190817 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/widgets/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      357 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/widgets/popup_response.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      524 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/widgets/related_multiple_widget_wrapper.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1260 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/widgets/related_widget_wrapper.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      585 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/error.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.536070 django-oscar-3.2b1/src/oscar/templates/oscar/forms/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.191498 django-oscar-3.2b1/src/oscar/templates/oscar/forms/widgets/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      543 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/forms/widgets/date_time_picker.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      716 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/forms/widgets/image_input_widget.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2382 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/layout.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1144 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/layout_2_col.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1023 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/layout_3_col.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      173 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/login_forbidden.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.192672 django-oscar-3.2b1/src/oscar/templates/oscar/offer/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1948 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/offer/detail.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1413 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/offer/list.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1253 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/offer/range.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.536449 django-oscar-3.2b1/src/oscar/templates/oscar/order/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.193054 django-oscar-3.2b1/src/oscar/templates/oscar/order/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6350 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/order/partials/basket_totals.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.204194 django-oscar-3.2b1/src/oscar/templates/oscar/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1685 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/alert_messages.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      151 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/brand.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      172 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/extrascripts.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      216 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/footer.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       79 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/footer_checkout.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      802 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/form.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2323 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/form_field.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      595 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/form_fields.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      638 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/form_fields_inline.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      558 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/google_analytics.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      962 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/google_analytics_transaction.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1111 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/mini_basket.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3950 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/nav_accounts.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1187 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/nav_checkout.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3265 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/nav_primary.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1145 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/pagination.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      303 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/partials/search.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.211073 django-oscar-3.2b1/src/oscar/templates/oscar/registration/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      929 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/registration/password_reset_complete.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1511 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/registration/password_reset_confirm.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1109 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/registration/password_reset_done.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1109 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/registration/password_reset_form.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.211831 django-oscar-3.2b1/src/oscar/templates/oscar/search/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:32.537098 django-oscar-3.2b1/src/oscar/templates/oscar/search/indexes/
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.212544 django-oscar-3.2b1/src/oscar/templates/oscar/search/indexes/product/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       83 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/search/indexes/product/item_text.txt
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.244399 django-oscar-3.2b1/src/oscar/templates/oscar/search/partials/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1081 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/search/partials/facet.html
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3348 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templates/oscar/search/results.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.245205 django-oscar-3.2b1/src/oscar/templates/oscar/wishlists/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1358 2022-06-24 14:35:55.000000 django-oscar-3.2b1/src/oscar/templates/oscar/wishlists/wishlist_detail.html
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.254231 django-oscar-3.2b1/src/oscar/templatetags/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1087 2022-06-24 07:48:35.000000 django-oscar-3.2b1/src/oscar/templatetags/basket_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3916 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/category_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1100 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/currency_filters.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      236 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/dashboard_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      229 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/datetime_filters.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1383 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/display_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      578 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/form_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     2065 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/history_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4212 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/image_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1050 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/product_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      386 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/purchase_info_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      787 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/reviews_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      882 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/shipping_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1657 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/sorting_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      145 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/string_filters.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      283 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/url_tags.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      188 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/templatetags/wishlist_tags.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.256513 django-oscar-3.2b1/src/oscar/test/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      979 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/basket.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      767 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/contextmanagers.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.265371 django-oscar-3.2b1/src/oscar/test/factories/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     8827 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      868 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/address.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      710 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/basket.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3409 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/catalogue.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      627 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/contrib.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      915 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/customer.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      226 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/models.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1590 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/offer.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4541 2022-06-22 07:04:09.000000 django-oscar-3.2b1/src/oscar/test/factories/order.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      825 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/partner.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      929 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/payment.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      852 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/urls.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      589 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/utils.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      241 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/views.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     1800 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/voucher.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      273 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/factories/wishlists.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3812 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/testcases.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     6205 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/test/utils.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.266689 django-oscar-3.2b1/src/oscar/utils/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)        0 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/utils/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)       60 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/utils/deprecation.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      215 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/utils/models.py
+drwxr-xr-x   0 joeyjurjens   (501) staff       (20)        0 2022-12-06 08:59:33.268278 django-oscar-3.2b1/src/oscar/views/
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)      795 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/views/__init__.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     3125 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/views/decorators.py
+-rw-r--r--   0 joeyjurjens   (501) staff       (20)     4863 2022-03-31 19:33:51.000000 django-oscar-3.2b1/src/oscar/views/generic.py
```

### Comparing `django-oscar-3.2b0/AUTHORS` & `django-oscar-3.2b1/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/LICENSE` & `django-oscar-3.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/PKG-INFO` & `django-oscar-3.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar
-Version: 3.2b0
+Version: 3.2b1
 Summary: A domain-driven e-commerce framework for Django
 Home-page: https://github.com/django-oscar/django-oscar
 Author: David Winterbottom
 Author-email: david.winterbottom@gmail.com
 License: BSD
 Keywords: E-commerce,Django,domain-driven
 Platform: linux
@@ -288,9 +288,7 @@
 Looking for commercial support?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 If you are interested in having an Oscar project built for you, or for
 development of an existing Oscar site then please get in touch via `info@oscarcommerce.com`_.
 
 .. _`info@oscarcommerce.com`: mailto:info@oscarcommerce.com
-
-
```

### Comparing `django-oscar-3.2b0/README.rst` & `django-oscar-3.2b1/README.rst`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/setup.py` & `django-oscar-3.2b1/setup.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/django_oscar.egg-info/PKG-INFO` & `django-oscar-3.2b1/src/django_oscar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar
-Version: 3.2b0
+Version: 3.2b1
 Summary: A domain-driven e-commerce framework for Django
 Home-page: https://github.com/django-oscar/django-oscar
 Author: David Winterbottom
 Author-email: david.winterbottom@gmail.com
 License: BSD
 Keywords: E-commerce,Django,domain-driven
 Platform: linux
@@ -288,9 +288,7 @@
 Looking for commercial support?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 If you are interested in having an Oscar project built for you, or for
 development of an existing Oscar site then please get in touch via `info@oscarcommerce.com`_.
 
 .. _`info@oscarcommerce.com`: mailto:info@oscarcommerce.com
-
-
```

### Comparing `django-oscar-3.2b0/src/django_oscar.egg-info/SOURCES.txt` & `django-oscar-3.2b1/src/django_oscar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/django_oscar.egg-info/requires.txt` & `django-oscar-3.2b1/src/django_oscar.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/__init__.py` & `django-oscar-3.2b1/src/oscar/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Use 'alpha', 'beta', 'rc' or 'final' as the 4th element to indicate release type.
-VERSION = (3, 2, 0, 'beta')
+VERSION = (3, 2, 0, 'beta', 1)
 
 
 def get_short_version():
     return '%s.%s' % (VERSION[0], VERSION[1])
 
 
 def get_version():
```

### Comparing `django-oscar-3.2b0/src/oscar/apps/address/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/address/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/address/admin.py` & `django-oscar-3.2b1/src/oscar/apps/address/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/address/forms.py` & `django-oscar-3.2b1/src/oscar/apps/address/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/address/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/address/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/address/migrations/0002_auto_20150927_1547.py` & `django-oscar-3.2b1/src/oscar/apps/address/migrations/0002_auto_20150927_1547.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/address/migrations/0003_auto_20150927_1551.py` & `django-oscar-3.2b1/src/oscar/apps/address/migrations/0003_auto_20150927_1551.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/address/migrations/0004_auto_20170226_1122.py` & `django-oscar-3.2b1/src/oscar/apps/address/migrations/0004_auto_20170226_1122.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/address/migrations/0005_regenerate_user_address_hashes.py` & `django-oscar-3.2b1/src/oscar/apps/address/migrations/0005_regenerate_user_address_hashes.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/analytics/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/analytics/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/analytics/admin.py` & `django-oscar-3.2b1/src/oscar/apps/analytics/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/analytics/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/analytics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/analytics/migrations/0002_auto_20140827_1705.py` & `django-oscar-3.2b1/src/oscar/apps/analytics/migrations/0002_auto_20140827_1705.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/analytics/migrations/0003_auto_20200801_0817.py` & `django-oscar-3.2b1/src/oscar/apps/analytics/migrations/0003_auto_20200801_0817.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/analytics/models.py` & `django-oscar-3.2b1/src/oscar/apps/analytics/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/analytics/receivers.py` & `django-oscar-3.2b1/src/oscar/apps/analytics/receivers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/analytics/reports.py` & `django-oscar-3.2b1/src/oscar/apps/analytics/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/analytics/scores.py` & `django-oscar-3.2b1/src/oscar/apps/analytics/scores.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/basket/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/admin.py` & `django-oscar-3.2b1/src/oscar/apps/basket/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/apps.py` & `django-oscar-3.2b1/src/oscar/apps/basket/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/forms.py` & `django-oscar-3.2b1/src/oscar/apps/basket/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/formsets.py` & `django-oscar-3.2b1/src/oscar/apps/basket/formsets.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/managers.py` & `django-oscar-3.2b1/src/oscar/apps/basket/managers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/middleware.py` & `django-oscar-3.2b1/src/oscar/apps/basket/middleware.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/basket/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/migrations/0002_auto_20140827_1705.py` & `django-oscar-3.2b1/src/oscar/apps/basket/migrations/0002_auto_20140827_1705.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/migrations/0003_basket_vouchers.py` & `django-oscar-3.2b1/src/oscar/apps/basket/migrations/0003_basket_vouchers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/migrations/0007_slugfield_noop.py` & `django-oscar-3.2b1/src/oscar/apps/basket/migrations/0007_slugfield_noop.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/migrations/0010_convert_to_valid_json.py` & `django-oscar-3.2b1/src/oscar/apps/basket/migrations/0010_convert_to_valid_json.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/models.py` & `django-oscar-3.2b1/src/oscar/apps/basket/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/reports.py` & `django-oscar-3.2b1/src/oscar/apps/basket/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/utils.py` & `django-oscar-3.2b1/src/oscar/apps/basket/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/basket/views.py` & `django-oscar-3.2b1/src/oscar/apps/basket/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/admin.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/apps.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/categories.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/categories.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/expressions.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/expressions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/managers.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/managers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0002_auto_20150217_1221.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0002_auto_20150217_1221.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0003_data_migration_slugs.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0003_data_migration_slugs.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0005_auto_20150604_1450.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0005_auto_20150604_1450.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0006_auto_20150807_1725.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0006_auto_20150807_1725.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0008_auto_20160304_1652.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0008_auto_20160304_1652.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0009_slugfield_noop.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0009_slugfield_noop.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0010_auto_20170420_0439.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0010_auto_20170420_0439.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0012_auto_20170609_1902.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0012_auto_20170609_1902.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0013_auto_20170821_1548.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0013_auto_20170821_1548.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0014_auto_20181115_1953.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0014_auto_20181115_1953.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0016_auto_20190327_0757.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0016_auto_20190327_0757.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0017_auto_20190816_0938.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0017_auto_20190816_0938.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0018_auto_20191220_0920.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0018_auto_20191220_0920.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0019_option_required.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0019_option_required.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0020_auto_20200801_0817.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0020_auto_20200801_0817.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0021_auto_20201005_0844.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0021_auto_20201005_0844.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0024_remove_duplicate_attributes.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0024_remove_duplicate_attributes.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/migrations/0026_predefined_product_options.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/migrations/0026_predefined_product_options.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/models.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/product_attributes.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/product_attributes.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
     To refetch the attribute values from the database:
 
         product.attr.refresh()
     """
 
     def __setstate__(self, state):
+        self.__dict__.setdefault("_product", None)
+        self.__dict__.setdefault("_initialized", False)
+        self.__dict__.setdefault("_dirty", set())
         self.__dict__ = state
 
     def __init__(self, product):
         # use __dict__ directly to avoid triggering __setattr__, which would
         # cause a recursion error on _initialized.
         self.__dict__.update(
             {"_product": product, "_initialized": False, "_dirty": set()}
```

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/receivers.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/receivers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/admin.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/apps.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/forms.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/migrations/0003_auto_20160802_1358.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/migrations/0003_auto_20160802_1358.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/migrations/0004_auto_20170429_0941.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/migrations/0004_auto_20170429_0941.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/reviews/views.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/reviews/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/search_handlers.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/search_handlers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/utils.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/catalogue/views.py` & `django-oscar-3.2b1/src/oscar/apps/catalogue/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/checkout/applicator.py` & `django-oscar-3.2b1/src/oscar/apps/checkout/applicator.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/checkout/apps.py` & `django-oscar-3.2b1/src/oscar/apps/checkout/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/checkout/calculators.py` & `django-oscar-3.2b1/src/oscar/apps/checkout/calculators.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/checkout/exceptions.py` & `django-oscar-3.2b1/src/oscar/apps/checkout/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/checkout/forms.py` & `django-oscar-3.2b1/src/oscar/apps/checkout/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/checkout/mixins.py` & `django-oscar-3.2b1/src/oscar/apps/checkout/mixins.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/checkout/session.py` & `django-oscar-3.2b1/src/oscar/apps/checkout/session.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/checkout/surcharges.py` & `django-oscar-3.2b1/src/oscar/apps/checkout/surcharges.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/checkout/utils.py` & `django-oscar-3.2b1/src/oscar/apps/checkout/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/checkout/views.py` & `django-oscar-3.2b1/src/oscar/apps/checkout/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/communication/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/communication/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/communication/app.py` & `django-oscar-3.2b1/src/oscar/apps/communication/app.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/communication/managers.py` & `django-oscar-3.2b1/src/oscar/apps/communication/managers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/communication/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/communication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/communication/migrations/0002_reset_table_names.py` & `django-oscar-3.2b1/src/oscar/apps/communication/migrations/0002_reset_table_names.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/communication/migrations/0003_remove_notification_category_make_code_uppercase.py` & `django-oscar-3.2b1/src/oscar/apps/communication/migrations/0003_remove_notification_category_make_code_uppercase.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/communication/migrations/0004_auto_20200801_0817.py` & `django-oscar-3.2b1/src/oscar/apps/communication/migrations/0004_auto_20200801_0817.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/communication/models.py` & `django-oscar-3.2b1/src/oscar/apps/communication/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/communication/notifications/views.py` & `django-oscar-3.2b1/src/oscar/apps/communication/notifications/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/communication/utils.py` & `django-oscar-3.2b1/src/oscar/apps/communication/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/customer/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/alerts/receivers.py` & `django-oscar-3.2b1/src/oscar/apps/customer/alerts/receivers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/alerts/utils.py` & `django-oscar-3.2b1/src/oscar/apps/customer/alerts/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/alerts/views.py` & `django-oscar-3.2b1/src/oscar/apps/customer/alerts/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/apps.py` & `django-oscar-3.2b1/src/oscar/apps/customer/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/auth_backends.py` & `django-oscar-3.2b1/src/oscar/apps/customer/auth_backends.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/forms.py` & `django-oscar-3.2b1/src/oscar/apps/customer/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/history.py` & `django-oscar-3.2b1/src/oscar/apps/customer/history.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/customer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/migrations/0002_auto_20150807_1725.py` & `django-oscar-3.2b1/src/oscar/apps/customer/migrations/0002_auto_20150807_1725.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/migrations/0004_email_save.py` & `django-oscar-3.2b1/src/oscar/apps/customer/migrations/0004_email_save.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/migrations/0006_auto_20190430_1736.py` & `django-oscar-3.2b1/src/oscar/apps/customer/migrations/0006_auto_20190430_1736.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/migrations/0007_auto_20200801_0817.py` & `django-oscar-3.2b1/src/oscar/apps/customer/migrations/0007_auto_20200801_0817.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/mixins.py` & `django-oscar-3.2b1/src/oscar/apps/customer/mixins.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/receivers.py` & `django-oscar-3.2b1/src/oscar/apps/customer/receivers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/utils.py` & `django-oscar-3.2b1/src/oscar/apps/customer/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/views.py` & `django-oscar-3.2b1/src/oscar/apps/customer/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/customer/wishlists/views.py` & `django-oscar-3.2b1/src/oscar/apps/customer/wishlists/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/formsets.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/formsets.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/mixins.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/mixins.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/tables.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/tables.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/catalogue/widgets.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/catalogue/widgets.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/communications/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/communications/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/communications/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/communications/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/communications/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/communications/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/menu.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/menu.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/nav.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/nav.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/offers/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/offers/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/offers/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/offers/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/offers/reports.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/offers/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/offers/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/offers/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/orders/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/orders/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/orders/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/orders/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/orders/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/orders/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/pages/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/pages/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/pages/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/pages/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/pages/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/pages/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/partners/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/partners/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/partners/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/partners/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/partners/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/partners/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/ranges/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/ranges/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/ranges/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/ranges/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/ranges/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/ranges/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/reports/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/reports/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/reports/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/reports/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/reports/reports.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/reports/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/reports/utils.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/reports/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/reports/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/reports/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/reviews/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/reviews/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/reviews/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/reviews/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/reviews/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/reviews/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/shipping/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/shipping/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/shipping/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/shipping/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/shipping/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/shipping/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/tables.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/tables.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/users/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/users/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/users/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/users/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/users/tables.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/users/tables.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/users/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/users/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/vouchers/apps.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/vouchers/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/vouchers/forms.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/vouchers/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/vouchers/views.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/vouchers/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/dashboard/widgets.py` & `django-oscar-3.2b1/src/oscar/apps/dashboard/widgets.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/offer/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/admin.py` & `django-oscar-3.2b1/src/oscar/apps/offer/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/applicator.py` & `django-oscar-3.2b1/src/oscar/apps/offer/applicator.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/apps.py` & `django-oscar-3.2b1/src/oscar/apps/offer/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/benefits.py` & `django-oscar-3.2b1/src/oscar/apps/offer/benefits.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/conditions.py` & `django-oscar-3.2b1/src/oscar/apps/offer/conditions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/custom.py` & `django-oscar-3.2b1/src/oscar/apps/offer/custom.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/managers.py` & `django-oscar-3.2b1/src/oscar/apps/offer/managers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/offer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/migrations/0002_auto_20151210_1053.py` & `django-oscar-3.2b1/src/oscar/apps/offer/migrations/0002_auto_20151210_1053.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/migrations/0003_auto_20161120_1707.py` & `django-oscar-3.2b1/src/oscar/apps/offer/migrations/0003_auto_20161120_1707.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/migrations/0005_auto_20170423_1217.py` & `django-oscar-3.2b1/src/oscar/apps/offer/migrations/0005_auto_20170423_1217.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/migrations/0006_auto_20170504_0616.py` & `django-oscar-3.2b1/src/oscar/apps/offer/migrations/0006_auto_20170504_0616.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/migrations/0007_conditionaloffer_exclusive.py` & `django-oscar-3.2b1/src/oscar/apps/offer/migrations/0007_conditionaloffer_exclusive.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/migrations/0008_auto_20181115_1953.py` & `django-oscar-3.2b1/src/oscar/apps/offer/migrations/0008_auto_20181115_1953.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/migrations/0010_conditionaloffer_combinations.py` & `django-oscar-3.2b1/src/oscar/apps/offer/migrations/0010_conditionaloffer_combinations.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/models.py` & `django-oscar-3.2b1/src/oscar/apps/offer/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/queryset.py` & `django-oscar-3.2b1/src/oscar/apps/offer/queryset.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/receivers.py` & `django-oscar-3.2b1/src/oscar/apps/offer/receivers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/reports.py` & `django-oscar-3.2b1/src/oscar/apps/offer/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/results.py` & `django-oscar-3.2b1/src/oscar/apps/offer/results.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/utils.py` & `django-oscar-3.2b1/src/oscar/apps/offer/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/offer/views.py` & `django-oscar-3.2b1/src/oscar/apps/offer/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/order/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/admin.py` & `django-oscar-3.2b1/src/oscar/apps/order/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/order/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/migrations/0006_orderstatuschange.py` & `django-oscar-3.2b1/src/oscar/apps/order/migrations/0006_orderstatuschange.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/migrations/0007_auto_20181115_1953.py` & `django-oscar-3.2b1/src/oscar/apps/order/migrations/0007_auto_20181115_1953.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/migrations/0008_auto_20190301_1035.py` & `django-oscar-3.2b1/src/oscar/apps/order/migrations/0008_auto_20190301_1035.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/migrations/0009_surcharge.py` & `django-oscar-3.2b1/src/oscar/apps/order/migrations/0009_surcharge.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/migrations/0010_auto_20200724_0909.py` & `django-oscar-3.2b1/src/oscar/apps/order/migrations/0010_auto_20200724_0909.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/migrations/0011_auto_20200801_0817.py` & `django-oscar-3.2b1/src/oscar/apps/order/migrations/0011_auto_20200801_0817.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/migrations/0012_convert_to_valid_json.py` & `django-oscar-3.2b1/src/oscar/apps/order/migrations/0012_convert_to_valid_json.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/models.py` & `django-oscar-3.2b1/src/oscar/apps/order/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/processing.py` & `django-oscar-3.2b1/src/oscar/apps/order/processing.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/reports.py` & `django-oscar-3.2b1/src/oscar/apps/order/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/order/utils.py` & `django-oscar-3.2b1/src/oscar/apps/order/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/partner/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/availability.py` & `django-oscar-3.2b1/src/oscar/apps/partner/availability.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/importers.py` & `django-oscar-3.2b1/src/oscar/apps/partner/importers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/partner/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/migrations/0003_auto_20150604_1450.py` & `django-oscar-3.2b1/src/oscar/apps/partner/migrations/0003_auto_20150604_1450.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/migrations/0004_auto_20160107_1755.py` & `django-oscar-3.2b1/src/oscar/apps/partner/migrations/0004_auto_20160107_1755.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/migrations/0005_auto_20181115_1953.py` & `django-oscar-3.2b1/src/oscar/apps/partner/migrations/0005_auto_20181115_1953.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/migrations/0006_auto_20200724_0909.py` & `django-oscar-3.2b1/src/oscar/apps/partner/migrations/0006_auto_20200724_0909.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/models.py` & `django-oscar-3.2b1/src/oscar/apps/partner/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/prices.py` & `django-oscar-3.2b1/src/oscar/apps/partner/prices.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/receivers.py` & `django-oscar-3.2b1/src/oscar/apps/partner/receivers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/partner/strategy.py` & `django-oscar-3.2b1/src/oscar/apps/partner/strategy.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/payment/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/payment/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/payment/admin.py` & `django-oscar-3.2b1/src/oscar/apps/payment/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/payment/bankcards.py` & `django-oscar-3.2b1/src/oscar/apps/payment/bankcards.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/payment/exceptions.py` & `django-oscar-3.2b1/src/oscar/apps/payment/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/payment/forms.py` & `django-oscar-3.2b1/src/oscar/apps/payment/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/payment/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/payment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/payment/migrations/0005_auto_20200801_0817.py` & `django-oscar-3.2b1/src/oscar/apps/payment/migrations/0005_auto_20200801_0817.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/payment/models.py` & `django-oscar-3.2b1/src/oscar/apps/payment/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/search/apps.py` & `django-oscar-3.2b1/src/oscar/apps/search/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/search/facets.py` & `django-oscar-3.2b1/src/oscar/apps/search/facets.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/search/forms.py` & `django-oscar-3.2b1/src/oscar/apps/search/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/search/search_handlers.py` & `django-oscar-3.2b1/src/oscar/apps/search/search_handlers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/search/search_indexes.py` & `django-oscar-3.2b1/src/oscar/apps/search/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/search/views.py` & `django-oscar-3.2b1/src/oscar/apps/search/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/shipping/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/shipping/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/shipping/admin.py` & `django-oscar-3.2b1/src/oscar/apps/shipping/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/shipping/methods.py` & `django-oscar-3.2b1/src/oscar/apps/shipping/methods.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/shipping/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/shipping/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/shipping/migrations/0002_auto_20150604_1450.py` & `django-oscar-3.2b1/src/oscar/apps/shipping/migrations/0002_auto_20150604_1450.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/shipping/migrations/0003_auto_20181115_1953.py` & `django-oscar-3.2b1/src/oscar/apps/shipping/migrations/0003_auto_20181115_1953.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/shipping/models.py` & `django-oscar-3.2b1/src/oscar/apps/shipping/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/shipping/repository.py` & `django-oscar-3.2b1/src/oscar/apps/shipping/repository.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/shipping/scales.py` & `django-oscar-3.2b1/src/oscar/apps/shipping/scales.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/admin.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0002_auto_20170418_2132.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0002_auto_20170418_2132.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0004_auto_20180228_0940.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0004_auto_20180228_0940.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0005_auto_20180402_1425.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0005_auto_20180402_1425.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0007_auto_20181115_1953.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0007_auto_20181115_1953.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0008_auto_20200801_0817.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0008_auto_20200801_0817.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0009_make_voucher_names_unique.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0009_make_voucher_names_unique.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/migrations/0010_auto_20210224_0712.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/migrations/0010_auto_20210224_0712.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/models.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/receivers.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/receivers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/reports.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/voucher/utils.py` & `django-oscar-3.2b1/src/oscar/apps/voucher/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/wishlists/abstract_models.py` & `django-oscar-3.2b1/src/oscar/apps/wishlists/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/wishlists/apps.py` & `django-oscar-3.2b1/src/oscar/apps/wishlists/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/wishlists/forms.py` & `django-oscar-3.2b1/src/oscar/apps/wishlists/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/wishlists/formsets.py` & `django-oscar-3.2b1/src/oscar/apps/wishlists/formsets.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/wishlists/migrations/0001_initial.py` & `django-oscar-3.2b1/src/oscar/apps/wishlists/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/wishlists/migrations/0004_auto_20220328_0939.py` & `django-oscar-3.2b1/src/oscar/apps/wishlists/migrations/0004_auto_20220328_0939.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/wishlists/models.py` & `django-oscar-3.2b1/src/oscar/apps/wishlists/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/apps/wishlists/views.py` & `django-oscar-3.2b1/src/oscar/apps/wishlists/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/config.py` & `django-oscar-3.2b1/src/oscar/config.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/ajax.py` & `django-oscar-3.2b1/src/oscar/core/ajax.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/application.py` & `django-oscar-3.2b1/src/oscar/core/application.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/compat.py` & `django-oscar-3.2b1/src/oscar/core/compat.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/context_processors.py` & `django-oscar-3.2b1/src/oscar/core/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/customisation.py` & `django-oscar-3.2b1/src/oscar/core/customisation.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/decorators.py` & `django-oscar-3.2b1/src/oscar/core/decorators.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/loading.py` & `django-oscar-3.2b1/src/oscar/core/loading.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/prices.py` & `django-oscar-3.2b1/src/oscar/core/prices.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/thumbnails.py` & `django-oscar-3.2b1/src/oscar/core/thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/utils.py` & `django-oscar-3.2b1/src/oscar/core/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/core/validators.py` & `django-oscar-3.2b1/src/oscar/core/validators.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/defaults.py` & `django-oscar-3.2b1/src/oscar/defaults.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/forms/fields.py` & `django-oscar-3.2b1/src/oscar/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/forms/mixins.py` & `django-oscar-3.2b1/src/oscar/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/forms/widgets.py` & `django-oscar-3.2b1/src/oscar/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/am_ET/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/am_ET/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ar/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ar/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ar_EG/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ar_EG/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ar_EG/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ar_EG/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ar_SA/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ar_SA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ar_SA/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ar_SA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/az/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/az/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/az/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/az/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/az_AZ/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/az_AZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/bg/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/bg_BG/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/bg_BG/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/bg_BG/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/bg_BG/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/bn/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/bn_BD/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/bn_BD/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/bn_BD/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/bn_BD/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ca/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ca/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ca_ES/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ca_ES/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/cmn/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/cmn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/crh/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/crh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/cs/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/cs/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/cs_CZ/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/cs_CZ/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/cy/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/cy/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/cy/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/cy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/da/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/da/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/de/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/de/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/el/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/el_GR/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/el_GR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/el_GR/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/el_GR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/en/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/en_AU/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/en_AU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/en_US/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/en_US/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/en_US/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/en_US/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/es/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/es/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/es_AR/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/es_AR/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/es_CL/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/es_CL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/es_CL/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/es_CL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/es_MX/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/es_MX/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/es_MX/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/es_MX/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/et/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/et/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/eu/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/eu/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/fa/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/fa/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/fa_IR/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/fa_IR/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/fi/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/fi/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/fr/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/fr/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/fr_CA/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/fr_CA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/fr_FR/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/gu/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/gu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/gu_IN/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/gu_IN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/he/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/he/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hi/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/hi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hi/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hi_IN/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/hi_IN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hi_IN/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/hi_IN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hr/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hr/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hu/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hu_HU/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/hu_HU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hu_HU/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/hu_HU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hy/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/hy/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hy/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/hy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/hy_AM/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/hy_AM/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/id/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/id/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/id_ID/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/id_ID/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/is_IS/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/is_IS/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/it/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/it/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ja/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ja/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ka_GE/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ka_GE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ka_GE/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ka_GE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ko/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ko/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/lt/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/lt/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/lv/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/lv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/lv/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ml/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ml/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/mr/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/mr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/mr/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/mr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ms/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ms/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/nb_NO/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/nb_NO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/nb_NO/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/nl/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/nl/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/pl/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/pl/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/pt/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/pt_BR/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/pt_BR/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/pt_PT/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/pt_PT/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ro_RO/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ro_RO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ro_RO/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ro_RO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ru/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ru/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ru@petr1708/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ru@petr1708/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ru@petr1708/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ru@petr1708/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ru_RU/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/ru_RU/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sk/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sk/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sk_SK/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/sk_SK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sk_SK/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/sk_SK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sl_SI/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/sl_SI/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sl_SI/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/sl_SI/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sr/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/sr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sr/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sv/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sv/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sv_SE/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/sv_SE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sw/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/sw_KE/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/sw_KE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/th/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/th_TH/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/th_TH/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/th_TH/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/tr/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/tr/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/tr_CY/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/tr_CY/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/tr_TR/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/tr_TR/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/uk/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/uk/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/uk_UA/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/uk_UA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/uk_UA/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/uk_UA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/vi/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/vi/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh-Hans/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/zh-Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh-Hans/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/zh-Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh-Hant/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/zh-Hant/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh-Hant/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/zh-Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh_CN/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh_CN/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh_CN.GB2312/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/zh_CN.GB2312/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh_HK/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/zh_HK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh_HK/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/zh_HK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh_SG/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/zh_SG/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh_TW/LC_MESSAGES/django.mo` & `django-oscar-3.2b1/src/oscar/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh_TW/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/locale/zh_TW.Big5/LC_MESSAGES/django.po` & `django-oscar-3.2b1/src/oscar/locale/zh_TW.Big5/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/management/commands/oscar_cleanup_alerts.py` & `django-oscar-3.2b1/src/oscar/management/commands/oscar_cleanup_alerts.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/management/commands/oscar_find_duplicate_emails.py` & `django-oscar-3.2b1/src/oscar/management/commands/oscar_find_duplicate_emails.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/management/commands/oscar_fork_app.py` & `django-oscar-3.2b1/src/oscar/management/commands/oscar_fork_app.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/management/commands/oscar_fork_statics.py` & `django-oscar-3.2b1/src/oscar/management/commands/oscar_fork_statics.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/management/commands/oscar_generate_email_content.py` & `django-oscar-3.2b1/src/oscar/management/commands/oscar_generate_email_content.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/management/commands/oscar_import_catalogue.py` & `django-oscar-3.2b1/src/oscar/management/commands/oscar_import_catalogue.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/management/commands/oscar_import_catalogue_images.py` & `django-oscar-3.2b1/src/oscar/management/commands/oscar_import_catalogue_images.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/management/commands/oscar_populate_countries.py` & `django-oscar-3.2b1/src/oscar/management/commands/oscar_populate_countries.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/management/commands/oscar_send_alerts.py` & `django-oscar-3.2b1/src/oscar/management/commands/oscar_send_alerts.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/management/commands/oscar_update_product_ratings.py` & `django-oscar-3.2b1/src/oscar/management/commands/oscar_update_product_ratings.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/models/fields/__init__.py` & `django-oscar-3.2b1/src/oscar/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/models/fields/autoslugfield.py` & `django-oscar-3.2b1/src/oscar/models/fields/autoslugfield.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/README.rst` & `django-oscar-3.2b1/src/oscar/static/oscar/README.rst`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/css/dashboard.css` & `django-oscar-3.2b1/src/oscar/static/oscar/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/css/dashboard.css.map` & `django-oscar-3.2b1/src/oscar/static/oscar/css/dashboard.css.map`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/css/select2-bootstrap.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/css/select2-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/css/styles.css` & `django-oscar-3.2b1/src/oscar/static/oscar/css/styles.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/css/styles.css.map` & `django-oscar-3.2b1/src/oscar/static/oscar/css/styles.css.map`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/favicon.ico` & `django-oscar-3.2b1/src/oscar/static/oscar/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/glyphicons-halflings-white.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/glyphicons-halflings.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/image_not_found.jpg` & `django-oscar-3.2b1/src/oscar/static/oscar/img/image_not_found.jpg`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/ui/dashboard/bg_subtle_dots.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/ui/dashboard/bg_subtle_dots.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/ui/dashboard/logo_oscar.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/ui/dashboard/logo_oscar.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_arrow_down.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_arrow_down.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_arrow_left.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_arrow_left.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_minus.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_minus.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_plus.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_plus.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_slider_left.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_slider_left.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/ui/icon_slider_right.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/ui/icon_slider_right.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/img/ui/nav_sprite.png` & `django-oscar-3.2b1/src/oscar/static/oscar/img/ui/nav_sprite.png`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4/bootstrap.bundle.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4/bootstrap.bundle.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4-datetimepicker/moment-with-locales.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4-datetimepicker/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4-datetimepicker/tempusdominus-bootstrap-4.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4-datetimepicker/tempusdominus-bootstrap-4.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/bootstrap4-datetimepicker/tempusdominus-bootstrap-4.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/bootstrap4-datetimepicker/tempusdominus-bootstrap-4.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/inputmask/jquery.inputmask.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/inputmask/jquery.inputmask.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/jquery/jquery.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/jquery-sortable/jquery-sortable-min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/jquery-sortable/jquery-sortable-min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/mousewheel/jquery.mousewheel.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/mousewheel/jquery.mousewheel.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/oscar/RelatedObjectLookups.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/oscar/RelatedObjectLookups.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/oscar/dashboard.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/oscar/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/oscar/popup_response.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/oscar/popup_response.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/oscar/ui.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/oscar/ui.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/select2/select2.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/select2/select2.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/icons/default/icons.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/icons/default/icons.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/jquery.tinymce.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/jquery.tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/models/dom/model.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/models/dom/model.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/advlist/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/advlist/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/anchor/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/anchor/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/autolink/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/autolink/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/autoresize/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/autoresize/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/autosave/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/autosave/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/charmap/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/charmap/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/code/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/code/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/codesample/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/codesample/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/directionality/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/directionality/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/emoticons/js/emojiimages.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/emoticons/js/emojiimages.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/emoticons/js/emojis.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/emoticons/js/emojis.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/emoticons/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/emoticons/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/fullscreen/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/fullscreen/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/help/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/help/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/image/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/image/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/importcss/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/importcss/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/insertdatetime/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/insertdatetime/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/link/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/link/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/lists/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/lists/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/media/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/media/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/nonbreaking/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/nonbreaking/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/pagebreak/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/pagebreak/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/preview/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/preview/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/quickbars/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/quickbars/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/save/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/save/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/searchreplace/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/searchreplace/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/table/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/table/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/template/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/template/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/visualblocks/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/visualblocks/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/visualchars/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/visualchars/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/plugins/wordcount/plugin.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/plugins/wordcount/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/dark/content.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/dark/content.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/default/content.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/default/content.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/document/content.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/document/content.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5/content.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5/content.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5-dark/content.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/tinymce-5-dark/content.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/content/writer/content.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/content/writer/content.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/content.inline.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/content.inline.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/content.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/content.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/skin.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/content.inline.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/content.inline.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/content.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/content.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/skin.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/oxide-dark/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/content.inline.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/content.inline.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/content.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/content.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/skin.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/content.inline.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/content.inline.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/content.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/content.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/skin.min.css` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/skins/ui/tinymce-5-dark/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/themes/silver/theme.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/themes/silver/theme.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/js/tinymce/tinymce.min.js` & `django-oscar-3.2b1/src/oscar/static/oscar/js/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/README.rst` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/README.rst`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/_alerts.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/_alerts.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/base.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/base.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/catalogue.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/catalogue.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/forms.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/forms.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/index.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/index.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/navbar.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/navbar.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/tables.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/tables.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard/variables.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard/variables.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/dashboard.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/dashboard.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/page/checkout.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/page/checkout.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/page/forms.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/page/forms.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/page/header.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/page/header.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/page/plugins.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/page/plugins.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/page/product_lists.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/page/product_lists.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/page/product_page.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/page/product_page.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/page/reviews.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/page/reviews.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/page/variables.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/page/variables.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/scss/styles.scss` & `django-oscar-3.2b1/src/oscar/static/oscar/scss/styles.scss`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-brands-400.ttf` & `django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-brands-400.woff2` & `django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-regular-400.ttf` & `django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-regular-400.woff2` & `django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-solid-900.ttf` & `django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-solid-900.woff2` & `django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-v4compatibility.ttf` & `django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/static/oscar/webfonts/fa-v4compatibility.woff2` & `django-oscar-3.2b1/src/oscar/static/oscar/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/flatpages/default.html` & `django-oscar-3.2b1/src/oscar/templates/flatpages/default.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/500.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/500.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/base.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/base.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/basket/basket.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/basket/basket.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/basket/messages/new_total.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/basket/messages/new_total.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/basket/partials/basket_content.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/basket/partials/basket_content.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/basket/partials/basket_quick.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/basket/partials/basket_quick.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/basket/partials/basket_totals.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/basket/partials/basket_totals.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/browse.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/browse.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/category.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/category.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/add_to_basket_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/add_to_basket_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/add_to_basket_form_compact.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/add_to_basket_form_compact.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/add_to_wishlist.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/add_to_wishlist.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/gallery.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/gallery.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/product.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/product.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/review.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/review.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/partials/stock_record.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/partials/stock_record.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/partials/review_stars.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/partials/review_stars.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/review_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/review_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/review_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/review_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/review_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/review_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/catalogue/reviews/review_product.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/catalogue/reviews/review_product.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/checkout.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/checkout.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/gateway.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/gateway.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/layout.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/layout.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/nav.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/nav.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/payment_details.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/payment_details.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/preview.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/preview.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/shipping_address.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/shipping_address.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/shipping_methods.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/shipping_methods.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/thank_you.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/thank_you.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/user_address_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/user_address_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/checkout/user_address_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/checkout/user_address_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/email/email_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/email/email_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/email/email_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/email/email_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/base.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/base.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_email_changed_body.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_email_changed_body.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_email_changed_body.txt` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_email_changed_body.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_order_placed_body.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_order_placed_body.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_order_placed_body.txt` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_order_placed_body.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_password_changed_body.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_password_changed_body.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_password_reset_body.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_password_reset_body.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_product_alert_body.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_product_alert_body.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_product_alert_body.txt` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_product_alert_body.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_product_alert_confirmation_body.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_product_alert_confirmation_body.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/emails/commtype_product_alert_confirmation_body.txt` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/emails/commtype_product_alert_confirmation_body.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/notifications/detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/notifications/detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/communication/notifications/list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/communication/notifications/list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/address/address_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/address/address_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/address/address_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/address/address_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/alerts/alert_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/alerts/alert_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/anon_order.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/anon_order.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/baseaccountpage.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/baseaccountpage.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/login_registration.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/login_registration.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/order/order_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/order/order_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/order/order_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/order/order_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/partials/standard_tabs.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/partials/standard_tabs.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/profile/profile.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/profile/profile.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/profile/profile_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/profile/profile_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/registration.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/registration.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/wishlists_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/wishlists_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/wishlists_delete_product.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/wishlists_delete_product.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/wishlists_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/wishlists_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/wishlists_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/wishlists_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/customer/wishlists/wishlists_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/customer/wishlists/wishlists_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_row_actions.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/attribute_option_group_row_actions.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/category_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/category_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/category_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/category_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/category_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/category_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/category_row_actions.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/category_row_actions.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/messages/product_saved.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/messages/product_saved.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/option_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/option_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/option_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/option_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/option_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/option_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/option_row_actions.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/option_row_actions.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_class_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_class_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_class_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_class_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_class_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_class_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_row_actions.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_row_actions.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/product_update.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/product_update.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/catalogue/stockalert_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/catalogue/stockalert_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/comms/detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/comms/detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/comms/list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/comms/list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/index.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/layout.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/layout.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/login.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/login.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/benefit_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/benefit_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/condition_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/condition_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/offer_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/offer_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/offer_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/offer_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/offer_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/offer_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/progress.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/progress.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/step_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/step_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/offers/summary.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/offers/summary.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/line_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/line_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/order_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/order_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/order_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/order_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/shippingaddress_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/shippingaddress_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/orders/statistics.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/orders/statistics.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/pages/delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/pages/delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/pages/index.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/pages/index.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/pages/update.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/pages/update.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/advanced_search_modal.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/advanced_search_modal.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/alert_messages.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/alert_messages.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/form_field.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/form_field.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/form_fields.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/form_fields.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/form_fields_inline.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/form_fields_inline.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/pagination.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/pagination.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partials/product_images.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partials/product_images.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_manage.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_manage.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_user_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_user_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_user_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_user_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/partners/partner_user_select.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/partners/partner_user_select.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/messages/range_products_saved.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/messages/range_products_saved.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/range_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/range_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/range_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/range_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/range_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/range_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/ranges/range_product_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/ranges/range_product_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/index.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/index.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/offer_report.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/offer_report.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/open_basket_report.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/open_basket_report.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/order_report.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/order_report.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/product_report.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/product_report.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/submitted_basket_report.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/submitted_basket_report.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/user_report.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/user_report.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reports/partials/voucher_report.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reports/partials/voucher_report.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reviews/review_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reviews/review_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reviews/review_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reviews/review_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/reviews/review_update.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/reviews/review_update.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_band_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_band_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_band_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_band_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_based_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_based_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_based_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_based_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_based_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_based_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/shipping/weight_based_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/shipping/weight_based_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/table.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/table.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/alerts/delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/alerts/delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/alerts/list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/alerts/list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/alerts/partials/alert.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/alerts/partials/alert.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/alerts/update.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/alerts/update.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/index.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/index.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/users/table.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/users/table.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/partials/voucher_set_details_table.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/partials/voucher_set_details_table.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_delete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/vouchers/voucher_set_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/widgets/related_multiple_widget_wrapper.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/widgets/related_multiple_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/dashboard/widgets/related_widget_wrapper.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/dashboard/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/error.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/error.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/forms/widgets/date_time_picker.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/forms/widgets/date_time_picker.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/forms/widgets/image_input_widget.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/forms/widgets/image_input_widget.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/layout.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/layout.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/layout_2_col.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/layout_2_col.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/layout_3_col.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/layout_3_col.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/offer/detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/offer/detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/offer/list.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/offer/list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/offer/range.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/offer/range.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/order/partials/basket_totals.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/order/partials/basket_totals.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/alert_messages.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/alert_messages.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/form_field.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/form_field.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/form_fields.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/form_fields.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/form_fields_inline.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/form_fields_inline.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/google_analytics.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/google_analytics.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/google_analytics_transaction.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/google_analytics_transaction.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/mini_basket.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/mini_basket.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/nav_accounts.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/nav_accounts.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/nav_checkout.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/nav_checkout.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/nav_primary.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/nav_primary.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/partials/pagination.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/partials/pagination.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/registration/password_reset_complete.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/registration/password_reset_confirm.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/registration/password_reset_done.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/registration/password_reset_form.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/search/partials/facet.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/search/partials/facet.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/search/results.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/search/results.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templates/oscar/wishlists/wishlist_detail.html` & `django-oscar-3.2b1/src/oscar/templates/oscar/wishlists/wishlist_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/basket_tags.py` & `django-oscar-3.2b1/src/oscar/templatetags/basket_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/category_tags.py` & `django-oscar-3.2b1/src/oscar/templatetags/category_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/currency_filters.py` & `django-oscar-3.2b1/src/oscar/templatetags/currency_filters.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/display_tags.py` & `django-oscar-3.2b1/src/oscar/templatetags/display_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/form_tags.py` & `django-oscar-3.2b1/src/oscar/templatetags/form_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/history_tags.py` & `django-oscar-3.2b1/src/oscar/templatetags/history_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/image_tags.py` & `django-oscar-3.2b1/src/oscar/templatetags/image_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/product_tags.py` & `django-oscar-3.2b1/src/oscar/templatetags/product_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/reviews_tags.py` & `django-oscar-3.2b1/src/oscar/templatetags/reviews_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/shipping_tags.py` & `django-oscar-3.2b1/src/oscar/templatetags/shipping_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/templatetags/sorting_tags.py` & `django-oscar-3.2b1/src/oscar/templatetags/sorting_tags.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/basket.py` & `django-oscar-3.2b1/src/oscar/test/basket.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/contextmanagers.py` & `django-oscar-3.2b1/src/oscar/test/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/__init__.py` & `django-oscar-3.2b1/src/oscar/test/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/address.py` & `django-oscar-3.2b1/src/oscar/test/factories/address.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/basket.py` & `django-oscar-3.2b1/src/oscar/test/factories/basket.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/catalogue.py` & `django-oscar-3.2b1/src/oscar/test/factories/catalogue.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/contrib.py` & `django-oscar-3.2b1/src/oscar/test/factories/contrib.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/customer.py` & `django-oscar-3.2b1/src/oscar/test/factories/customer.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/offer.py` & `django-oscar-3.2b1/src/oscar/test/factories/offer.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/order.py` & `django-oscar-3.2b1/src/oscar/test/factories/order.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/partner.py` & `django-oscar-3.2b1/src/oscar/test/factories/partner.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/payment.py` & `django-oscar-3.2b1/src/oscar/test/factories/payment.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/urls.py` & `django-oscar-3.2b1/src/oscar/test/factories/urls.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/utils.py` & `django-oscar-3.2b1/src/oscar/test/factories/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/factories/voucher.py` & `django-oscar-3.2b1/src/oscar/test/factories/voucher.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/testcases.py` & `django-oscar-3.2b1/src/oscar/test/testcases.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/test/utils.py` & `django-oscar-3.2b1/src/oscar/test/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/views/__init__.py` & `django-oscar-3.2b1/src/oscar/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/views/decorators.py` & `django-oscar-3.2b1/src/oscar/views/decorators.py`

 * *Files identical despite different names*

### Comparing `django-oscar-3.2b0/src/oscar/views/generic.py` & `django-oscar-3.2b1/src/oscar/views/generic.py`

 * *Files identical despite different names*

