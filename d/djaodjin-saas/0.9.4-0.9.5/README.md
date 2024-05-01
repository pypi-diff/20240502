# Comparing `tmp/djaodjin-saas-0.9.4.tar.gz` & `tmp/djaodjin-saas-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djaodjin-saas-0.9.4.tar", last modified: Thu Mar 25 18:03:12 2021, max compression
+gzip compressed data, was "dist/djaodjin-saas-0.9.5.tar", last modified: Tue Apr 27 05:39:36 2021, max compression
```

## Comparing `djaodjin-saas-0.9.4.tar` & `djaodjin-saas-0.9.5.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/
--rw-r--r--   0 smirolo    (502) staff       (20)     4956 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/PKG-INFO
--rw-r--r--   0 smirolo    (502) staff       (20)     3773 2021-03-25 18:01:15.000000 djaodjin-saas-0.9.4/README.md
--rw-r--r--   0 smirolo    (502) staff       (20)      252 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/requirements.txt
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/
--rw-r--r--   0 smirolo    (502) staff       (20)     1433 2021-03-25 18:01:55.000000 djaodjin-saas-0.9.4/saas/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1962 2020-05-25 20:56:38.000000 djaodjin-saas-0.9.4/saas/admin.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/api/
--rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/api/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)    10114 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/api/accounts.py
--rw-r--r--   0 smirolo    (502) staff       (20)     6268 2021-03-24 20:20:21.000000 djaodjin-saas-0.9.4/saas/api/backend.py
--rw-r--r--   0 smirolo    (502) staff       (20)     9728 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.4/saas/api/balances.py
--rw-r--r--   0 smirolo    (502) staff       (20)    21023 2021-03-23 20:53:08.000000 djaodjin-saas-0.9.4/saas/api/billing.py
--rw-r--r--   0 smirolo    (502) staff       (20)    11676 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/api/charges.py
--rw-r--r--   0 smirolo    (502) staff       (20)     8334 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/api/coupons.py
--rw-r--r--   0 smirolo    (502) staff       (20)    27323 2021-02-22 15:57:14.000000 djaodjin-saas-0.9.4/saas/api/metrics.py
--rw-r--r--   0 smirolo    (502) staff       (20)    17170 2021-03-24 20:00:11.000000 djaodjin-saas-0.9.4/saas/api/organizations.py
--rw-r--r--   0 smirolo    (502) staff       (20)    12119 2021-03-24 17:11:48.000000 djaodjin-saas-0.9.4/saas/api/plans.py
--rw-r--r--   0 smirolo    (502) staff       (20)    49575 2021-03-24 17:41:27.000000 djaodjin-saas-0.9.4/saas/api/roles.py
--rw-r--r--   0 smirolo    (502) staff       (20)    37085 2021-03-24 20:01:57.000000 djaodjin-saas-0.9.4/saas/api/serializers.py
--rw-r--r--   0 smirolo    (502) staff       (20)    27821 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/api/subscriptions.py
--rw-r--r--   0 smirolo    (502) staff       (20)    20011 2020-06-06 05:34:17.000000 djaodjin-saas-0.9.4/saas/api/transactions.py
--rw-r--r--   0 smirolo    (502) staff       (20)     5593 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/api/users.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/backends/
--rw-r--r--   0 smirolo    (502) staff       (20)     4404 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/backends/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     5437 2021-03-23 21:05:27.000000 djaodjin-saas-0.9.4/saas/backends/fake_processor.py
--rw-r--r--   0 smirolo    (502) staff       (20)     6787 2021-03-23 21:05:07.000000 djaodjin-saas-0.9.4/saas/backends/razorpay_processor.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/backends/stripe_processor/
--rw-r--r--   0 smirolo    (502) staff       (20)       32 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/backends/stripe_processor/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)    47123 2021-03-23 17:51:22.000000 djaodjin-saas-0.9.4/saas/backends/stripe_processor/base.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/backends/stripe_processor/urls/
--rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/backends/stripe_processor/urls/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1578 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/backends/stripe_processor/urls/api.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1628 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/backends/stripe_processor/urls/views.py
--rw-r--r--   0 smirolo    (502) staff       (20)     5089 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/backends/stripe_processor/views.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/backends/urls/
--rw-r--r--   0 smirolo    (502) staff       (20)     1562 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/backends/urls/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1523 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/backends/urls/api.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1525 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/backends/urls/views.py
--rw-r--r--   0 smirolo    (502) staff       (20)    11579 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/cart.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3766 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/compat.py
--rw-r--r--   0 smirolo    (502) staff       (20)    40398 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/decorators.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2316 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/docs.py
--rw-r--r--   0 smirolo    (502) staff       (20)     9332 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/extras.py
--rw-r--r--   0 smirolo    (502) staff       (20)    13607 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/filters.py
--rw-r--r--   0 smirolo    (502) staff       (20)    16178 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/forms.py
--rw-r--r--   0 smirolo    (502) staff       (20)    13091 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/humanize.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3596 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/ledger.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/management/
--rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/management/__init__.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/management/commands/
--rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/management/commands/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2308 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/management/commands/compile_stats.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1935 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/management/commands/delete_organization.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2265 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/management/commands/delete_processor_customers.py
--rw-r--r--   0 smirolo    (502) staff       (20)    10249 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/management/commands/ledger.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3456 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/management/commands/reconcile_with_processor.py
--rw-r--r--   0 smirolo    (502) staff       (20)     4527 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/management/commands/renewals.py
--rw-r--r--   0 smirolo    (502) staff       (20)     8934 2021-02-22 15:56:26.000000 djaodjin-saas-0.9.4/saas/management/commands/report_weekly_revenue.py
--rw-r--r--   0 smirolo    (502) staff       (20)     7877 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/management/commands/send_invites.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/metrics/
--rw-r--r--   0 smirolo    (502) staff       (20)        0 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.4/saas/metrics/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)    15845 2021-02-22 15:50:19.000000 djaodjin-saas-0.9.4/saas/metrics/base.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2886 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.4/saas/metrics/subscriptions.py
--rw-r--r--   0 smirolo    (502) staff       (20)     8330 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/metrics/transactions.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/migrations/
--rw-r--r--   0 smirolo    (502) staff       (20)    18901 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/migrations/0001_initial.py
--rw-r--r--   0 smirolo    (502) staff       (20)      419 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/migrations/0002_auto_20161126_2248.py
--rw-r--r--   0 smirolo    (502) staff       (20)      459 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/migrations/0003_balanceline_is_positive.py
--rw-r--r--   0 smirolo    (502) staff       (20)      845 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/migrations/0004_auto_20161221_1944.py
--rw-r--r--   0 smirolo    (502) staff       (20)      438 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/migrations/0005_role_extra.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3426 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/migrations/0006_0_3_0.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3397 2019-12-11 05:35:09.000000 djaodjin-saas-0.9.4/saas/migrations/0007_0_3_3.py
--rw-r--r--   0 smirolo    (502) staff       (20)    14688 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/migrations/0008_0_3_4.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1260 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/migrations/0009_0_3_5.py
--rw-r--r--   0 smirolo    (502) staff       (20)      313 2019-12-11 05:36:57.000000 djaodjin-saas-0.9.4/saas/migrations/0010_0_4_0.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1219 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/migrations/0011_0_7_0.py
--rw-r--r--   0 smirolo    (502) staff       (20)      652 2020-01-20 17:05:17.000000 djaodjin-saas-0.9.4/saas/migrations/0012_0_8_3.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1508 2020-05-25 20:56:38.000000 djaodjin-saas-0.9.4/saas/migrations/0013_0_9_0.py
--rw-r--r--   0 smirolo    (502) staff       (20)      508 2021-02-22 18:42:09.000000 djaodjin-saas-0.9.4/saas/migrations/0014_v0_9_3.py
--rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/migrations/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)    46736 2021-03-23 20:32:25.000000 djaodjin-saas-0.9.4/saas/mixins.py
--rw-r--r--   0 smirolo    (502) staff       (20)   195199 2021-03-24 20:08:53.000000 djaodjin-saas-0.9.4/saas/models.py
--rw-r--r--   0 smirolo    (502) staff       (20)     4135 2019-12-17 22:27:55.000000 djaodjin-saas-0.9.4/saas/pagination.py
--rw-r--r--   0 smirolo    (502) staff       (20)    19503 2021-02-26 18:16:49.000000 djaodjin-saas-0.9.4/saas/renewals.py
--rw-r--r--   0 smirolo    (502) staff       (20)     8432 2021-02-22 16:15:00.000000 djaodjin-saas-0.9.4/saas/settings.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3244 2021-02-22 17:55:24.000000 djaodjin-saas-0.9.4/saas/signals.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/static/
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/static/js/
--rw-r--r--   0 smirolo    (502) staff       (20)     3909 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/static/js/djaodjin-postal.js
--rw-r--r--   0 smirolo    (502) staff       (20)    33930 2020-06-04 18:09:32.000000 djaodjin-saas-0.9.4/saas/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (502) staff       (20)     4881 2021-03-24 17:40:51.000000 djaodjin-saas-0.9.4/saas/static/js/djaodjin-resources.js
--rw-r--r--   0 smirolo    (502) staff       (20)    49507 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/static/js/djaodjin-saas-angular.js
--rw-r--r--   0 smirolo    (502) staff       (20)    82540 2021-03-24 20:11:15.000000 djaodjin-saas-0.9.4/saas/static/js/djaodjin-saas-vue.js
--rw-r--r--   0 smirolo    (502) staff       (20)    29265 2020-10-14 04:29:25.000000 djaodjin-saas-0.9.4/saas/static/js/djaodjin-saas.js
--rw-r--r--   0 smirolo    (502) staff       (20)    21828 2021-03-24 20:15:25.000000 djaodjin-saas-0.9.4/saas/static/js/djaodjin-stripe.js
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/templates/
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/templates/saas/
--rw-r--r--   0 smirolo    (502) staff       (20)     1569 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/_bank_use.html
--rw-r--r--   0 smirolo    (502) staff       (20)     3008 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/templates/saas/_card_use.html
--rw-r--r--   0 smirolo    (502) staff       (20)     1247 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/_charges.html
--rw-r--r--   0 smirolo    (502) staff       (20)      338 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/_filter.html
--rw-r--r--   0 smirolo    (502) staff       (20)     3332 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/templates/saas/_invoiceables.html
--rw-r--r--   0 smirolo    (502) staff       (20)      666 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/_paginator.html
--rw-r--r--   0 smirolo    (502) staff       (20)      565 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/_razorpay_checkout.html
--rw-r--r--   0 smirolo    (502) staff       (20)     1883 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/_sidebar.html
--rw-r--r--   0 smirolo    (502) staff       (20)     1421 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/_transactions.html
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/templates/saas/agreements/
--rw-r--r--   0 smirolo    (502) staff       (20)     1894 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/agreements/security.md
--rw-r--r--   0 smirolo    (502) staff       (20)     5165 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/agreements/terms-of-use.md
--rw-r--r--   0 smirolo    (502) staff       (20)     2213 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/templates/saas/base.html
--rw-r--r--   0 smirolo    (502) staff       (20)     3590 2020-10-14 04:36:54.000000 djaodjin-saas-0.9.4/saas/templates/saas/base_dashboard.html
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/
--rw-r--r--   0 smirolo    (502) staff       (20)     1027 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/balance.html
--rw-r--r--   0 smirolo    (502) staff       (20)     2443 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/bank.html
--rw-r--r--   0 smirolo    (502) staff       (20)      924 2021-03-23 22:20:24.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/card.html
--rw-r--r--   0 smirolo    (502) staff       (20)      216 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/cart-periods.html
--rw-r--r--   0 smirolo    (502) staff       (20)      230 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/cart-seats.html
--rw-r--r--   0 smirolo    (502) staff       (20)     2474 2021-03-23 22:13:46.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/cart.html
--rw-r--r--   0 smirolo    (502) staff       (20)      225 2019-10-25 21:14:24.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/charges.html
--rw-r--r--   0 smirolo    (502) staff       (20)     6322 2020-06-07 20:42:36.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/checkout.html
--rw-r--r--   0 smirolo    (502) staff       (20)     5945 2020-05-25 20:56:38.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/coupons.html
--rw-r--r--   0 smirolo    (502) staff       (20)     1556 2019-10-25 20:55:23.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/import.html
--rw-r--r--   0 smirolo    (502) staff       (20)     2491 2019-12-17 22:28:33.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/index.html
--rw-r--r--   0 smirolo    (502) staff       (20)     3083 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/receipt.html
--rw-r--r--   0 smirolo    (502) staff       (20)     2909 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/transactions.html
--rw-r--r--   0 smirolo    (502) staff       (20)     1119 2019-10-25 22:04:46.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/transfers.html
--rw-r--r--   0 smirolo    (502) staff       (20)      639 2020-03-05 16:50:40.000000 djaodjin-saas-0.9.4/saas/templates/saas/billing/withdraw.html
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/templates/saas/legal/
--rw-r--r--   0 smirolo    (502) staff       (20)      140 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/legal/agreement.html
--rw-r--r--   0 smirolo    (502) staff       (20)     1047 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/legal/index.html
--rw-r--r--   0 smirolo    (502) staff       (20)      424 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/legal/sign.html
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/templates/saas/metrics/
--rw-r--r--   0 smirolo    (502) staff       (20)     3040 2019-10-25 21:30:37.000000 djaodjin-saas-0.9.4/saas/templates/saas/metrics/balances.html
--rw-r--r--   0 smirolo    (502) staff       (20)     2918 2019-10-30 22:12:01.000000 djaodjin-saas-0.9.4/saas/templates/saas/metrics/base.html
--rw-r--r--   0 smirolo    (502) staff       (20)     2244 2019-12-19 18:02:41.000000 djaodjin-saas-0.9.4/saas/templates/saas/metrics/coupons.html
--rw-r--r--   0 smirolo    (502) staff       (20)     3859 2019-10-25 20:36:53.000000 djaodjin-saas-0.9.4/saas/templates/saas/metrics/dashboard.html
--rw-r--r--   0 smirolo    (502) staff       (20)      227 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/metrics/plans.html
--rw-r--r--   0 smirolo    (502) staff       (20)       86 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/metrics/revenue.html
--rw-r--r--   0 smirolo    (502) staff       (20)      333 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/organization_redirects.html
--rw-r--r--   0 smirolo    (502) staff       (20)     1100 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/pricing.html
--rw-r--r--   0 smirolo    (502) staff       (20)     3375 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/printable_charge_receipt.html
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/templates/saas/profile/
--rw-r--r--   0 smirolo    (502) staff       (20)     1365 2019-10-25 23:51:54.000000 djaodjin-saas-0.9.4/saas/templates/saas/profile/index.html
--rw-r--r--   0 smirolo    (502) staff       (20)      317 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/profile/new.html
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/templates/saas/profile/roles/
--rw-r--r--   0 smirolo    (502) staff       (20)     1590 2019-10-25 21:15:19.000000 djaodjin-saas-0.9.4/saas/templates/saas/profile/roles/index.html
--rw-r--r--   0 smirolo    (502) staff       (20)     3243 2020-05-25 20:57:15.000000 djaodjin-saas-0.9.4/saas/templates/saas/profile/roles/role.html
--rw-r--r--   0 smirolo    (502) staff       (20)     6096 2019-10-25 22:49:44.000000 djaodjin-saas-0.9.4/saas/templates/saas/profile/subscribers.html
--rw-r--r--   0 smirolo    (502) staff       (20)     5108 2019-10-26 01:32:07.000000 djaodjin-saas-0.9.4/saas/templates/saas/profile/subscriptions.html
--rw-r--r--   0 smirolo    (502) staff       (20)      330 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templates/saas/redeem.html
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/templates/saas/users/
--rw-r--r--   0 smirolo    (502) staff       (20)     3922 2020-01-22 06:19:25.000000 djaodjin-saas-0.9.4/saas/templates/saas/users/roles.html
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/templatetags/
--rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/templatetags/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     7339 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/templatetags/saas_tags.py
--rw-r--r--   0 smirolo    (502) staff       (20)     4761 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.4/saas/tests.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/urls/
--rw-r--r--   0 smirolo    (502) staff       (20)     1627 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/urls/__init__.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/urls/api/
--rw-r--r--   0 smirolo    (502) staff       (20)     1736 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/urls/api/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2682 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/broker.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2008 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/cart.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1666 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/legal.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/urls/api/provider/
--rw-r--r--   0 smirolo    (502) staff       (20)     1846 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/provider/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2603 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/provider/billing.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1829 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/provider/charges.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2887 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.4/saas/urls/api/provider/metrics.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1828 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/provider/plans.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1940 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/provider/roles.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2522 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/provider/subscribers.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1868 2019-11-19 21:42:27.000000 djaodjin-saas-0.9.4/saas/urls/api/search.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/urls/api/subscriber/
--rw-r--r--   0 smirolo    (502) staff       (20)     1701 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/urls/api/subscriber/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2204 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/subscriber/billing.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1957 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/subscriber/charges.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2381 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/subscriber/profile.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2119 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/subscriber/roles.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2585 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/api/users.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2775 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/broker.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1945 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/noauth.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/urls/provider/
--rw-r--r--   0 smirolo    (502) staff       (20)     1607 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/urls/provider/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2670 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/provider/billing.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2921 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.4/saas/urls/provider/metrics.py
--rw-r--r--   0 smirolo    (502) staff       (20)     3161 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/provider/profile.py
--rw-r--r--   0 smirolo    (502) staff       (20)     5887 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/redirects.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2069 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/request.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/urls/subscriber/
--rw-r--r--   0 smirolo    (502) staff       (20)     1599 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/urls/subscriber/__init__.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/urls/subscriber/billing/
--rw-r--r--   0 smirolo    (502) staff       (20)     1565 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/urls/subscriber/billing/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2430 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/subscriber/billing/info.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2636 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/subscriber/billing/payment.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2419 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/subscriber/profile.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1645 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/urls/users.py
--rw-r--r--   0 smirolo    (502) staff       (20)    13825 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/utils.py
-drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-03-25 18:03:12.000000 djaodjin-saas-0.9.4/saas/views/
--rw-r--r--   0 smirolo    (502) staff       (20)     1504 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/views/__init__.py
--rw-r--r--   0 smirolo    (502) staff       (20)    45333 2021-03-23 20:55:55.000000 djaodjin-saas-0.9.4/saas/views/billing.py
--rw-r--r--   0 smirolo    (502) staff       (20)    13047 2021-02-23 16:11:41.000000 djaodjin-saas-0.9.4/saas/views/download.py
--rw-r--r--   0 smirolo    (502) staff       (20)     1715 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/saas/views/extra.py
--rw-r--r--   0 smirolo    (502) staff       (20)     6537 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/views/legal.py
--rw-r--r--   0 smirolo    (502) staff       (20)     9743 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/views/metrics.py
--rw-r--r--   0 smirolo    (502) staff       (20)     7137 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/views/optins.py
--rw-r--r--   0 smirolo    (502) staff       (20)     9542 2020-12-01 21:54:48.000000 djaodjin-saas-0.9.4/saas/views/plans.py
--rw-r--r--   0 smirolo    (502) staff       (20)    16671 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/views/profile.py
--rw-r--r--   0 smirolo    (502) staff       (20)    14100 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/views/redirects.py
--rw-r--r--   0 smirolo    (502) staff       (20)     9490 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/saas/views/roles.py
--rw-r--r--   0 smirolo    (502) staff       (20)     2773 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.4/saas/views/users.py
--rw-r--r--   0 smirolo    (502) staff       (20)       39 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.4/setup.cfg
--rw-r--r--   0 smirolo    (502) staff       (20)     3425 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.4/setup.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/
+-rw-r--r--   0 smirolo    (502) staff       (20)     5220 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/PKG-INFO
+-rw-r--r--   0 smirolo    (502) staff       (20)     4013 2021-04-27 05:38:14.000000 djaodjin-saas-0.9.5/README.md
+-rw-r--r--   0 smirolo    (502) staff       (20)      252 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/requirements.txt
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1433 2021-04-27 05:31:58.000000 djaodjin-saas-0.9.5/saas/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1962 2020-05-25 20:56:38.000000 djaodjin-saas-0.9.5/saas/admin.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/api/
+-rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/api/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    10114 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/api/accounts.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     6878 2021-03-26 06:55:12.000000 djaodjin-saas-0.9.5/saas/api/backend.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     9728 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.5/saas/api/balances.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    21105 2021-04-26 23:32:06.000000 djaodjin-saas-0.9.5/saas/api/billing.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    11676 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/api/charges.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     8334 2021-04-17 02:56:38.000000 djaodjin-saas-0.9.5/saas/api/coupons.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    27323 2021-02-22 15:57:14.000000 djaodjin-saas-0.9.5/saas/api/metrics.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    17170 2021-03-24 20:00:11.000000 djaodjin-saas-0.9.5/saas/api/organizations.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    12119 2021-03-24 17:11:48.000000 djaodjin-saas-0.9.5/saas/api/plans.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    49575 2021-04-27 03:19:52.000000 djaodjin-saas-0.9.5/saas/api/roles.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    37494 2021-04-15 18:11:14.000000 djaodjin-saas-0.9.5/saas/api/serializers.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    27821 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/api/subscriptions.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    20011 2020-06-06 05:34:17.000000 djaodjin-saas-0.9.5/saas/api/transactions.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     5593 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/api/users.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/backends/
+-rw-r--r--   0 smirolo    (502) staff       (20)     4404 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/backends/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     5437 2021-03-23 21:05:27.000000 djaodjin-saas-0.9.5/saas/backends/fake_processor.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     6787 2021-03-23 21:05:07.000000 djaodjin-saas-0.9.5/saas/backends/razorpay_processor.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/backends/stripe_processor/
+-rw-r--r--   0 smirolo    (502) staff       (20)       32 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/backends/stripe_processor/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    47579 2021-04-15 17:52:13.000000 djaodjin-saas-0.9.5/saas/backends/stripe_processor/base.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/backends/stripe_processor/urls/
+-rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/backends/stripe_processor/urls/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1578 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/backends/stripe_processor/urls/api.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1628 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/backends/stripe_processor/urls/views.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     5089 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/backends/stripe_processor/views.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/backends/urls/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1562 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/backends/urls/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1523 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/backends/urls/api.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1525 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/backends/urls/views.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    11579 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/cart.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3766 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/compat.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    40398 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/decorators.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2507 2021-04-07 18:09:08.000000 djaodjin-saas-0.9.5/saas/docs.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     9332 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/extras.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    13607 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/filters.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    16178 2021-04-26 15:29:47.000000 djaodjin-saas-0.9.5/saas/forms.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    13091 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/humanize.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3596 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/ledger.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/management/
+-rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/management/__init__.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/management/commands/
+-rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/management/commands/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2308 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/management/commands/compile_stats.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1935 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/management/commands/delete_organization.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2265 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/management/commands/delete_processor_customers.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    10249 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/management/commands/ledger.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3456 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/management/commands/reconcile_with_processor.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     4527 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/management/commands/renewals.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     8934 2021-02-22 15:56:26.000000 djaodjin-saas-0.9.5/saas/management/commands/report_weekly_revenue.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     7877 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/management/commands/send_invites.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/metrics/
+-rw-r--r--   0 smirolo    (502) staff       (20)        0 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.5/saas/metrics/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    15845 2021-02-22 15:50:19.000000 djaodjin-saas-0.9.5/saas/metrics/base.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2886 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.5/saas/metrics/subscriptions.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     8330 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/metrics/transactions.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/migrations/
+-rw-r--r--   0 smirolo    (502) staff       (20)    18901 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/migrations/0001_initial.py
+-rw-r--r--   0 smirolo    (502) staff       (20)      419 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/migrations/0002_auto_20161126_2248.py
+-rw-r--r--   0 smirolo    (502) staff       (20)      459 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/migrations/0003_balanceline_is_positive.py
+-rw-r--r--   0 smirolo    (502) staff       (20)      845 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/migrations/0004_auto_20161221_1944.py
+-rw-r--r--   0 smirolo    (502) staff       (20)      438 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/migrations/0005_role_extra.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3426 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/migrations/0006_0_3_0.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3397 2019-12-11 05:35:09.000000 djaodjin-saas-0.9.5/saas/migrations/0007_0_3_3.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    14688 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/migrations/0008_0_3_4.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1260 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/migrations/0009_0_3_5.py
+-rw-r--r--   0 smirolo    (502) staff       (20)      313 2019-12-11 05:36:57.000000 djaodjin-saas-0.9.5/saas/migrations/0010_0_4_0.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1219 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/migrations/0011_0_7_0.py
+-rw-r--r--   0 smirolo    (502) staff       (20)      652 2020-01-20 17:05:17.000000 djaodjin-saas-0.9.5/saas/migrations/0012_0_8_3.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1508 2020-05-25 20:56:38.000000 djaodjin-saas-0.9.5/saas/migrations/0013_0_9_0.py
+-rw-r--r--   0 smirolo    (502) staff       (20)      508 2021-02-22 18:42:09.000000 djaodjin-saas-0.9.5/saas/migrations/0014_v0_9_3.py
+-rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/migrations/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    47309 2021-04-25 15:44:53.000000 djaodjin-saas-0.9.5/saas/mixins.py
+-rw-r--r--   0 smirolo    (502) staff       (20)   194895 2021-04-17 04:06:15.000000 djaodjin-saas-0.9.5/saas/models.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     4135 2019-12-17 22:27:55.000000 djaodjin-saas-0.9.5/saas/pagination.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    19503 2021-02-26 18:16:49.000000 djaodjin-saas-0.9.5/saas/renewals.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     8432 2021-02-22 16:15:00.000000 djaodjin-saas-0.9.5/saas/settings.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3244 2021-02-22 17:55:24.000000 djaodjin-saas-0.9.5/saas/signals.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/static/
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/static/js/
+-rw-r--r--   0 smirolo    (502) staff       (20)     3909 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/static/js/djaodjin-postal.js
+-rw-r--r--   0 smirolo    (502) staff       (20)    33930 2020-06-04 18:09:32.000000 djaodjin-saas-0.9.5/saas/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (502) staff       (20)     4881 2021-03-24 17:40:51.000000 djaodjin-saas-0.9.5/saas/static/js/djaodjin-resources.js
+-rw-r--r--   0 smirolo    (502) staff       (20)    49507 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/static/js/djaodjin-saas-angular.js
+-rw-r--r--   0 smirolo    (502) staff       (20)    84063 2021-04-27 03:20:08.000000 djaodjin-saas-0.9.5/saas/static/js/djaodjin-saas-vue.js
+-rw-r--r--   0 smirolo    (502) staff       (20)    29265 2020-10-14 04:29:25.000000 djaodjin-saas-0.9.5/saas/static/js/djaodjin-saas.js
+-rw-r--r--   0 smirolo    (502) staff       (20)    21998 2021-04-26 23:52:25.000000 djaodjin-saas-0.9.5/saas/static/js/djaodjin-stripe.js
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/templates/
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/templates/saas/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1569 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/_bank_use.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     3008 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/templates/saas/_card_use.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     1247 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/_charges.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      338 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/_filter.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     3332 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/templates/saas/_invoiceables.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      666 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/_paginator.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      565 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/_razorpay_checkout.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     1883 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/_sidebar.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     1421 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/_transactions.html
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/templates/saas/agreements/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1894 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/agreements/security.md
+-rw-r--r--   0 smirolo    (502) staff       (20)     5165 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/agreements/terms-of-use.md
+-rw-r--r--   0 smirolo    (502) staff       (20)     2213 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/templates/saas/base.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     3590 2020-10-14 04:36:54.000000 djaodjin-saas-0.9.5/saas/templates/saas/base_dashboard.html
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1027 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/balance.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     2443 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/bank.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     1013 2021-04-15 18:19:56.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/card.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      216 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/cart-periods.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      230 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/cart-seats.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     2569 2021-04-15 18:23:45.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/cart.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      225 2019-10-25 21:14:24.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/charges.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     6322 2020-06-07 20:42:36.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/checkout.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     5945 2020-05-25 20:56:38.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/coupons.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     1556 2019-10-25 20:55:23.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/import.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     2491 2019-12-17 22:28:33.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/index.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     3069 2021-04-22 06:48:01.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/receipt.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     2909 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/transactions.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     1119 2019-10-25 22:04:46.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/transfers.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      639 2020-03-05 16:50:40.000000 djaodjin-saas-0.9.5/saas/templates/saas/billing/withdraw.html
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/templates/saas/legal/
+-rw-r--r--   0 smirolo    (502) staff       (20)      140 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/legal/agreement.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     1047 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/legal/index.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      424 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/legal/sign.html
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/templates/saas/metrics/
+-rw-r--r--   0 smirolo    (502) staff       (20)     3040 2019-10-25 21:30:37.000000 djaodjin-saas-0.9.5/saas/templates/saas/metrics/balances.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     2918 2019-10-30 22:12:01.000000 djaodjin-saas-0.9.5/saas/templates/saas/metrics/base.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     2244 2019-12-19 18:02:41.000000 djaodjin-saas-0.9.5/saas/templates/saas/metrics/coupons.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     3859 2019-10-25 20:36:53.000000 djaodjin-saas-0.9.5/saas/templates/saas/metrics/dashboard.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      227 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/metrics/plans.html
+-rw-r--r--   0 smirolo    (502) staff       (20)       86 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/metrics/revenue.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      333 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/organization_redirects.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     1100 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/pricing.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     3361 2021-04-22 06:50:33.000000 djaodjin-saas-0.9.5/saas/templates/saas/printable_charge_receipt.html
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/templates/saas/profile/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1365 2019-10-25 23:51:54.000000 djaodjin-saas-0.9.5/saas/templates/saas/profile/index.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      317 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/profile/new.html
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/templates/saas/profile/roles/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1590 2019-10-25 21:15:19.000000 djaodjin-saas-0.9.5/saas/templates/saas/profile/roles/index.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     3195 2021-04-27 02:38:33.000000 djaodjin-saas-0.9.5/saas/templates/saas/profile/roles/role.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     6096 2019-10-25 22:49:44.000000 djaodjin-saas-0.9.5/saas/templates/saas/profile/subscribers.html
+-rw-r--r--   0 smirolo    (502) staff       (20)     5108 2019-10-26 01:32:07.000000 djaodjin-saas-0.9.5/saas/templates/saas/profile/subscriptions.html
+-rw-r--r--   0 smirolo    (502) staff       (20)      330 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templates/saas/redeem.html
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/templates/saas/users/
+-rw-r--r--   0 smirolo    (502) staff       (20)     3871 2021-04-27 03:19:08.000000 djaodjin-saas-0.9.5/saas/templates/saas/users/roles.html
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/templatetags/
+-rw-r--r--   0 smirolo    (502) staff       (20)        0 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     7339 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/templatetags/saas_tags.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     4761 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.5/saas/tests.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/urls/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1627 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/urls/__init__.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/urls/api/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1736 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2682 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/broker.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2008 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/cart.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1666 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/legal.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/urls/api/provider/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1846 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/provider/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2603 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/provider/billing.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1829 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/provider/charges.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2887 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.5/saas/urls/api/provider/metrics.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1828 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/provider/plans.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1940 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/provider/roles.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2522 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/provider/subscribers.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1868 2019-11-19 21:42:27.000000 djaodjin-saas-0.9.5/saas/urls/api/search.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/urls/api/subscriber/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1701 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/urls/api/subscriber/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2204 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/subscriber/billing.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1957 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/subscriber/charges.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2381 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/subscriber/profile.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2119 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/subscriber/roles.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2585 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/api/users.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2775 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/broker.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1945 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/noauth.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/urls/provider/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1607 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/urls/provider/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2670 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/provider/billing.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2921 2020-12-01 21:56:22.000000 djaodjin-saas-0.9.5/saas/urls/provider/metrics.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     3161 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/provider/profile.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     5887 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/redirects.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2069 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/request.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/urls/subscriber/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1599 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/urls/subscriber/__init__.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/urls/subscriber/billing/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1565 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/urls/subscriber/billing/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2430 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/subscriber/billing/info.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2636 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/subscriber/billing/payment.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2419 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/subscriber/profile.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1645 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/urls/users.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    13825 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/utils.py
+drwxr-xr-x   0 smirolo    (502) staff       (20)        0 2021-04-27 05:39:36.000000 djaodjin-saas-0.9.5/saas/views/
+-rw-r--r--   0 smirolo    (502) staff       (20)     1504 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/views/__init__.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    45333 2021-03-23 20:55:55.000000 djaodjin-saas-0.9.5/saas/views/billing.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    13047 2021-02-23 16:11:41.000000 djaodjin-saas-0.9.5/saas/views/download.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     1715 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/saas/views/extra.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     6537 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/views/legal.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     9743 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/views/metrics.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     7137 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/views/optins.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     9542 2020-12-01 21:54:48.000000 djaodjin-saas-0.9.5/saas/views/plans.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    17143 2021-04-26 20:36:40.000000 djaodjin-saas-0.9.5/saas/views/profile.py
+-rw-r--r--   0 smirolo    (502) staff       (20)    14307 2021-04-07 18:58:00.000000 djaodjin-saas-0.9.5/saas/views/redirects.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     9490 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/saas/views/roles.py
+-rw-r--r--   0 smirolo    (502) staff       (20)     2773 2020-09-01 22:36:15.000000 djaodjin-saas-0.9.5/saas/views/users.py
+-rw-r--r--   0 smirolo    (502) staff       (20)       39 2019-10-11 18:54:49.000000 djaodjin-saas-0.9.5/setup.cfg
+-rw-r--r--   0 smirolo    (502) staff       (20)     3425 2021-02-22 15:42:35.000000 djaodjin-saas-0.9.5/setup.py
```

### Comparing `djaodjin-saas-0.9.4/PKG-INFO` & `djaodjin-saas-0.9.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 1.1
 Name: djaodjin-saas
-Version: 0.9.4
+Version: 0.9.5
 Summary: Django application for subscription businesses
 Home-page: https://github.com/djaodjin/djaodjin-saas/
 Author: The DjaoDjin Team
 Author-email: support@djaodjin.com
 License: BSD
-Download-URL: https://github.com/djaodjin/djaodjin-saas/tarball/0.9.4
+Download-URL: https://github.com/djaodjin/djaodjin-saas/tarball/0.9.5
 Description: djaodjin-saas is a Django application that implements the logic to support
         subscription-based Software-as-a-Service businesses.
         
         Major Features:
         
         - Separate billing profiles and authenticated users
         - Double entry book keeping ledger
         - Flexible security framework
         
         Tested with
         
-        - **Python:** 3.6, **Django:** 2.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.11
-        - **Python:** 3.6, **Django:** 3.0 (latest), **Django Rest Framework:** 3.11
-        - **Python:** 2.7 (end-of-life), **Django:** 1.11, **Django Rest Framework:** 3.9.4
+        - **Python:** 3.6, **Django:** 2.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
+        - **Python:** 3.6, **Django:** 3.0 (latest), **Django Rest Framework:** 3.12
+        - **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
         
         This project contains bare bone templates which are compatible with Django
         and Jinja2 template engines. To see djaodjin-saas in action as part
         of a full-fledged subscription-based session proxy, take a look
         at [djaoapp](https://github.com/djaodjin/djaoapp/).
         
         Full documentation for the project is available at
@@ -101,16 +101,19 @@
         Django project. We provide sample e-mail templates here in the
         saas/templates/notification/ directory.
         
         
         Release Notes
         =============
         
-        0.9.4
+        0.9.5
         
-          * adds processor in checkout and card APIs
-          * fixes computed balance due when subscription is free
-          * re-raises all StripeError as ProcessorError
+          * keeps user model fields in sync with personal billing profile
+          * prints last4 as exactly 4 digits on receipts
+          * fixes index error in the presence of 100% discount and advance payments
+          * fixes statement balances in the presence of GroupBuy
+          * fixes PaymentIntent not found while using StripeConnect accounts
+          * redirects to login page on redirects-to-profile if user not authenticated
         
         [previous release notes](changelog)
         
 Platform: UNKNOWN
```

### Comparing `djaodjin-saas-0.9.4/README.md` & `djaodjin-saas-0.9.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 - Separate billing profiles and authenticated users
 - Double entry book keeping ledger
 - Flexible security framework
 
 Tested with
 
-- **Python:** 3.6, **Django:** 2.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.11
-- **Python:** 3.6, **Django:** 3.0 (latest), **Django Rest Framework:** 3.11
-- **Python:** 2.7 (end-of-life), **Django:** 1.11, **Django Rest Framework:** 3.9.4
+- **Python:** 3.6, **Django:** 2.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
+- **Python:** 3.6, **Django:** 3.0 (latest), **Django Rest Framework:** 3.12
+- **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
 
 This project contains bare bone templates which are compatible with Django
 and Jinja2 template engines. To see djaodjin-saas in action as part
 of a full-fledged subscription-based session proxy, take a look
 at [djaoapp](https://github.com/djaodjin/djaoapp/).
 
 Full documentation for the project is available at
@@ -92,14 +92,17 @@
 Django project. We provide sample e-mail templates here in the
 saas/templates/notification/ directory.
 
 
 Release Notes
 =============
 
-0.9.4
+0.9.5
 
-  * adds processor in checkout and card APIs
-  * fixes computed balance due when subscription is free
-  * re-raises all StripeError as ProcessorError
+  * keeps user model fields in sync with personal billing profile
+  * prints last4 as exactly 4 digits on receipts
+  * fixes index error in the presence of 100% discount and advance payments
+  * fixes statement balances in the presence of GroupBuy
+  * fixes PaymentIntent not found while using StripeConnect accounts
+  * redirects to login page on redirects-to-profile if user not authenticated
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-saas-0.9.4/saas/__init__.py` & `djaodjin-saas-0.9.5/saas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the saas django app.
 """
 
-__version__ = '0.9.4'
+__version__ = '0.9.5'
```

### Comparing `djaodjin-saas-0.9.4/saas/admin.py` & `djaodjin-saas-0.9.5/saas/admin.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/accounts.py` & `djaodjin-saas-0.9.5/saas/api/accounts.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/backend.py` & `djaodjin-saas-0.9.5/saas/api/backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from rest_framework import status
 from rest_framework.exceptions import ValidationError
 from rest_framework.generics import (RetrieveAPIView,
     RetrieveUpdateDestroyAPIView)
 from rest_framework.response import Response
 
 from ..backends import ProcessorError
-from ..docs import swagger_auto_schema
+from ..docs import swagger_auto_schema, Parameter, IN_PATH
 from ..mixins import OrganizationMixin
 from ..models import get_broker
 from .serializers import (BankSerializer, CardSerializer,
     CardTokenSerializer)
 
 #pylint: disable=no-init
 
@@ -83,14 +83,20 @@
                                  RetrieveUpdateDestroyAPIView):
     """
     Retrieves a payment method
 
     Pass through to the processor to retrieve some details about
     the payment method (ex: credit card) associated to a subscriber.
 
+    When you wish to update the payment method on file through
+    a Strong Customer Authentication (SCA) workflow, the payment processor
+    will require a token generated by the server. That token can be retrieved
+    in the processor.STRIPE_INTENT_SECRET field when the API is called
+    with `?update=1` query parameters.
+
     **Tags**: billing
 
     **Examples**
 
     .. code-block:: http
 
         GET /api/billing/cowork/card/ HTTP/1.1
@@ -120,14 +126,22 @@
         .. code-block:: http
 
             DELETE /api/billing/cowork/card/ HTTP/1.1
         """
         return super(PaymentMethodDetailAPIView, self).delete(
             request, *args, **kwargs)
 
+    @swagger_auto_schema(
+        manual_parameters=[
+            Parameter('update', IN_PATH, type='bool')
+        ])
+    def get(self, request, *args, **kwargs):
+        return super(PaymentMethodDetailAPIView, self).get(
+            request, *args, **kwargs)
+
     @swagger_auto_schema(request_body=CardTokenSerializer)
     def put(self, request, *args, **kwargs):
         """
         Updates a payment method
 
         Pass through to the processor to update some details about
         the payment method (ex: credit card) associated to a subscriber.
```

### Comparing `djaodjin-saas-0.9.4/saas/api/balances.py` & `djaodjin-saas-0.9.5/saas/api/balances.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/billing.py` & `djaodjin-saas-0.9.5/saas/api/billing.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,17 +180,18 @@
         for item in items:
             cart_item, created = self.insert_item(request, **item)
             if created:
                 status_code = status.HTTP_201_CREATED
             # insert_item will either return a dict or a CartItem instance
             # (which cannot be directly serialized).
             if isinstance(cart_item, CartItem):
-                cart_items += [serializer.to_representation(cart_item)]
-            else:
-                cart_items += [cart_item]
+                cart_item = serializer.to_representation(cart_item)
+            if cart_item.get('sync_on'):
+                cart_item.update({'detail': _("User was added.")})
+            cart_items += [cart_item]
         if len(items) > 1:
             headers = self.get_success_headers(cart_items)
             return Response(cart_items, status=status_code, headers=headers)
         headers = self.get_success_headers(cart_items[0])
         return Response(cart_items[0], status=status_code, headers=headers)
 
     @staticmethod
```

### Comparing `djaodjin-saas-0.9.4/saas/api/charges.py` & `djaodjin-saas-0.9.5/saas/api/charges.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/coupons.py` & `djaodjin-saas-0.9.5/saas/api/coupons.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/metrics.py` & `djaodjin-saas-0.9.5/saas/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/organizations.py` & `djaodjin-saas-0.9.5/saas/api/organizations.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/plans.py` & `djaodjin-saas-0.9.5/saas/api/plans.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/roles.py` & `djaodjin-saas-0.9.5/saas/api/roles.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/serializers.py` & `djaodjin-saas-0.9.5/saas/api/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,19 @@
     balance_unit = serializers.CharField(
         help_text=_("Three-letter ISO 4217 code for currency unit (ex: usd)"))
 
 
 class ProcessorAuthSerializer(NoModelSerializer):
 
     STRIPE_PUB_KEY = serializers.CharField(required=False,
-        help_text=_("Stripe processor public key"))
+        help_text=_("Processor public key (Stripe)"))
     STRIPE_INTENT_SECRET = serializers.CharField(required=False,
-        help_text=_("intent secret for SCA (Stripe)"))
+        help_text=_("PaymentIntent or SetupIntent secret for SCA (Stripe)"))
+    STRIPE_ACCOUNT = serializers.CharField(required=False,
+        help_text=_("Connected account identifier (Stripe)"))
 
 
 class CardSerializer(NoModelSerializer):
     """
     Information to verify a credit card
     """
     processor = ProcessorAuthSerializer(required=False,
@@ -233,25 +235,29 @@
 
     state = serializers.CharField(source='get_state_display',
         help_text=_("Current state (i.e. created, done, failed, disputed)"))
     readable_amount = serializers.SerializerMethodField(
         help_text=_("Amount and unit in a commonly accepted readable format"))
     detail = serializers.CharField(read_only=True, required=False,
         help_text=_("Feedback for the user in plain text"))
+    last4 = serializers.CharField(source='get_last4_display', read_only=True,
+        help_text=_("Last 4 digits of the credit card used"))
 
     @staticmethod
     def get_readable_amount(charge):
         return as_money(charge.amount, charge.unit)
 
     class Meta:
         model = Charge
         fields = ('created_at', 'amount', 'unit', 'readable_amount',
-                  'description', 'last4', 'exp_date', 'processor_key', 'state',
-                  'detail')
-        read_only_fields = ('detail',)
+            'description', 'last4', 'exp_date', 'processor_key', 'state',
+            'detail')
+        read_only_fields = ('created_at', 'amount', 'unit', 'readable_amount',
+            'description', 'last4', 'exp_date', 'processor_key', 'state',
+            'detail')
 
 
 class CouponCreateSerializer(serializers.ModelSerializer):
     """
     Serializer to create a coupon, including the `code`.
     """
     discount_type = EnumField(choices=Coupon.DISCOUNT_CHOICES,
```

### Comparing `djaodjin-saas-0.9.4/saas/api/subscriptions.py` & `djaodjin-saas-0.9.5/saas/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/transactions.py` & `djaodjin-saas-0.9.5/saas/api/transactions.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/api/users.py` & `djaodjin-saas-0.9.5/saas/api/users.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/backends/__init__.py` & `djaodjin-saas-0.9.5/saas/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/backends/fake_processor.py` & `djaodjin-saas-0.9.5/saas/backends/fake_processor.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/backends/razorpay_processor.py` & `djaodjin-saas-0.9.5/saas/backends/razorpay_processor.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/backends/stripe_processor/base.py` & `djaodjin-saas-0.9.5/saas/backends/stripe_processor/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,16 @@
         kwargs = self._prepare_request()
         if self.mode == self.REMOTE and not self._is_platform(broker):
             # We generate Stripe data into the StripeConnect account.
             if not broker.processor_deposit_key:
                 raise ProcessorSetupError(
                     _("%(organization)s is not connected to a Stripe account."
                     ) % {'organization': broker}, broker)
+            # https://stripe.com/docs/connect/enable-payment-acceptance-guide?\
+            #platform=web#create-a-payment-intent
             kwargs.update({'stripe_account': broker.processor_deposit_key})
         return kwargs
 
     def _prepare_transfer_request(self, provider):
         kwargs = self._prepare_request()
         if (self.mode in (self.FORWARD, self.REMOTE)
             and  not self._is_platform(provider)):
@@ -736,28 +738,34 @@
                 # We are updating a card for later payments.
                 setup_intent = stripe.SetupIntent.create(**kwargs)
                 LOGGER.debug("stripe.PaymentIntent.create("\
                     "amount=%d, currency=%s, kwargs=%s) =>\n%s",
                     amount, unit, kwargs, str(setup_intent))
                 context.update({
                     'STRIPE_INTENT_SECRET': setup_intent.client_secret})
+                if 'stripe_account' in kwargs:
+                    context.update({
+                        'STRIPE_ACCOUNT': kwargs.get('stripe_account')})
 
             elif amount > 0:
                 if broker_fee_amount:
                     kwargs.update({'application_fee_amount': broker_fee_amount})
                 try:
                     payment_intent = stripe.PaymentIntent.create(
                         amount=amount, currency=unit,
                         setup_future_usage='off_session',
                         **kwargs)
                     LOGGER.debug("stripe.PaymentIntent.create("\
                         "amount=%d, currency=%s, kwargs=%s) =>\n%s",
                         amount, unit, kwargs, str(payment_intent))
                     context.update({
                         'STRIPE_INTENT_SECRET': payment_intent.client_secret})
+                    if 'stripe_account' in kwargs:
+                        context.update({
+                            'STRIPE_ACCOUNT': kwargs.get('stripe_account')})
 
                 except stripe.error.CardError as err:
                     # If the card is declined, Stripe will record a failed
                     # ``Charge`` and raise an exception here. Unfortunately only
                     # the Charge id is present in the CardError exception.
                     # So instead of generating
                     # an HTTP retrieve and recording a failed charge in our
```

### Comparing `djaodjin-saas-0.9.4/saas/backends/stripe_processor/urls/api.py` & `djaodjin-saas-0.9.5/saas/backends/stripe_processor/urls/api.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/backends/stripe_processor/urls/views.py` & `djaodjin-saas-0.9.5/saas/backends/stripe_processor/urls/views.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/backends/stripe_processor/views.py` & `djaodjin-saas-0.9.5/saas/backends/stripe_processor/views.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/backends/urls/__init__.py` & `djaodjin-saas-0.9.5/saas/backends/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/backends/urls/api.py` & `djaodjin-saas-0.9.5/saas/backends/urls/api.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/backends/urls/views.py` & `djaodjin-saas-0.9.5/saas/backends/urls/views.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/cart.py` & `djaodjin-saas-0.9.5/saas/cart.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/compat.py` & `djaodjin-saas-0.9.5/saas/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/decorators.py` & `djaodjin-saas-0.9.5/saas/decorators.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/docs.py` & `djaodjin-saas-0.9.5/saas/docs.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,20 +21,22 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 #pylint:disable=unused-argument,unused-import
 
 try:
-    from drf_yasg.openapi import Response as OpenAPIResponse
+    from drf_yasg.openapi import Response as OpenAPIResponse, Parameter, IN_PATH
     from drf_yasg.utils import no_body, swagger_auto_schema
 except ImportError:
     from functools import wraps
     from .compat import available_attrs
 
+    IN_PATH = 0
+
     class no_body(object):#pylint:disable=invalid-name
         pass
 
     def swagger_auto_schema(function=None, **kwargs):
         """
         Dummy decorator when drf_yasg is not present.
         """
@@ -50,7 +52,14 @@
 
     class OpenAPIResponse(object):
         """
         Dummy response object to document API.
         """
         def __init__(self, *args, **kwargs):
             pass
+
+    class Parameter(object):
+        """
+        Dummy object to document API.
+        """
+        def __init__(self, *args, **kwargs):
+            pass
```

### Comparing `djaodjin-saas-0.9.4/saas/extras.py` & `djaodjin-saas-0.9.5/saas/extras.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/filters.py` & `djaodjin-saas-0.9.5/saas/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/forms.py` & `djaodjin-saas-0.9.5/saas/forms.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/humanize.py` & `djaodjin-saas-0.9.5/saas/humanize.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/ledger.py` & `djaodjin-saas-0.9.5/saas/ledger.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/management/commands/compile_stats.py` & `djaodjin-saas-0.9.5/saas/management/commands/compile_stats.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/management/commands/delete_organization.py` & `djaodjin-saas-0.9.5/saas/management/commands/delete_organization.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/management/commands/delete_processor_customers.py` & `djaodjin-saas-0.9.5/saas/management/commands/delete_processor_customers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/management/commands/ledger.py` & `djaodjin-saas-0.9.5/saas/management/commands/ledger.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/management/commands/reconcile_with_processor.py` & `djaodjin-saas-0.9.5/saas/management/commands/reconcile_with_processor.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/management/commands/renewals.py` & `djaodjin-saas-0.9.5/saas/management/commands/renewals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/management/commands/report_weekly_revenue.py` & `djaodjin-saas-0.9.5/saas/management/commands/report_weekly_revenue.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/management/commands/send_invites.py` & `djaodjin-saas-0.9.5/saas/management/commands/send_invites.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/metrics/base.py` & `djaodjin-saas-0.9.5/saas/metrics/base.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/metrics/subscriptions.py` & `djaodjin-saas-0.9.5/saas/metrics/subscriptions.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/metrics/transactions.py` & `djaodjin-saas-0.9.5/saas/metrics/transactions.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/migrations/0001_initial.py` & `djaodjin-saas-0.9.5/saas/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/migrations/0004_auto_20161221_1944.py` & `djaodjin-saas-0.9.5/saas/migrations/0004_auto_20161221_1944.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/migrations/0006_0_3_0.py` & `djaodjin-saas-0.9.5/saas/migrations/0006_0_3_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/migrations/0007_0_3_3.py` & `djaodjin-saas-0.9.5/saas/migrations/0007_0_3_3.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/migrations/0008_0_3_4.py` & `djaodjin-saas-0.9.5/saas/migrations/0008_0_3_4.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/migrations/0009_0_3_5.py` & `djaodjin-saas-0.9.5/saas/migrations/0009_0_3_5.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/migrations/0011_0_7_0.py` & `djaodjin-saas-0.9.5/saas/migrations/0011_0_7_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/migrations/0012_0_8_3.py` & `djaodjin-saas-0.9.5/saas/migrations/0012_0_8_3.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/migrations/0013_0_9_0.py` & `djaodjin-saas-0.9.5/saas/migrations/0013_0_9_0.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/mixins.py` & `djaodjin-saas-0.9.5/saas/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 #pylint:disable=too-many-lines
 from __future__ import unicode_literals
 
-import re
+import logging, re
 
 from django.contrib.auth import REDIRECT_FIELD_NAME, get_user_model
 from django.contrib.auth.hashers import UNUSABLE_PASSWORD_PREFIX
 from django.db.models import Q, F
 from django.http import Http404
 from django.template.defaultfilters import slugify
 from django.utils.translation import ugettext_lazy as _
@@ -44,14 +44,16 @@
     RoleDescription, Subscription, Transaction, get_broker, is_broker,
     sum_orig_amount)
 from .utils import (build_absolute_uri, datetime_or_now,
     get_organization_model, get_role_model, update_context_urls,
     validate_redirect_url)
 from .extras import OrganizationMixinBase
 
+LOGGER = logging.getLogger(__name__)
+
 
 class BalanceDueMixin(object):
     """
     Mixin to retrieve a profile's balance due as line items
     for a checkout workflow.
     """
     @staticmethod
@@ -70,14 +72,19 @@
     def as_invoicables(self, user, customer, at_time=None):
         #pylint: disable=too-many-locals,unused-argument,no-self-use
         invoicables = []
         at_time = datetime_or_now(at_time)
         balances = Transaction.objects.get_statement_balances(
             customer, until=at_time)
         for event_id, amount_by_units in six.iteritems(balances):
+            if not event_id.startswith('sub_'):
+                # XXX Not showing balance due on group buy events.
+                LOGGER.error("Looking at a balance %s on event_id '%s'",
+                    amount_by_units, event_id)
+                continue
             subscription = Subscription.objects.get_by_event_id(event_id)
             last_unpaid_orders = customer.last_unpaid_orders(
                 subscription=subscription, at_time=at_time)
             order_balances = sum_orig_amount(last_unpaid_orders)
             lines = []
             for order_balance in order_balances:
                 order_amount = order_balance.get('amount')
@@ -324,15 +331,18 @@
             else:
                 options = self.get_cart_options(subscription,
                     created_at=created_at, prorate_to=prorate_to,
                     cart_item=cart_item)
                 # option is selected
                 if len(options) == 1:
                     # We only have one option.
-                    line = options[cart_item.option - 1]
+                    # It could happen when we use a 100% discount coupon
+                    # with advance discounts; in which case the advance
+                    # discounts would be cancelled. nothing is totally free.
+                    line = options[0]
                     lines += [line]
                     options = []
                 elif (cart_item.option > 0 and
                     (cart_item.option - 1) < len(options)):
                     # The number of periods was already selected so we generate
                     # a line instead.
                     line = options[cart_item.option - 1]
@@ -1206,19 +1216,22 @@
         active_links=active_links)
 
 
 def get_charge_context(charge):
     """
     Return a dictionnary useful to populate charge receipt templates.
     """
-    context = {'charge': charge,
-               'refunded': charge.refunded.exists(),
-               'charge_items': charge.line_items,
-               'organization': charge.customer,
-               'provider': charge.broker, # XXX update templates
+    context = {
+        'last4': charge.get_last4_display(),
+        'exp_date': charge.exp_date,
+        'charge': charge,
+        'refunded': charge.refunded.exists(),
+        'charge_items': charge.line_items,
+        'organization': charge.customer,
+        'provider': charge.broker, # XXX update templates
     }
     return context
 
 
 def product_url(provider, subscriber=None, request=None):
     """
     We cannot use a basic ``reverse('product_default_start')`` here because
```

### Comparing `djaodjin-saas-0.9.4/saas/models.py` & `djaodjin-saas-0.9.5/saas/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1362,20 +1362,23 @@
     def create_charge(self, customer, transactions, amount, unit,
                       processor, processor_charge_id, receipt_info,
                       user=None, descr=None, created_at=None):
         #pylint: disable=too-many-arguments
         assert amount > 0
         created_at = datetime_or_now(created_at)
         with transaction.atomic():
+            last4 = receipt_info.get('last4')
+            if last4:
+                last4 = int(last4)
             charge = self.create(
                 processor=processor, processor_key=processor_charge_id,
                 amount=amount, unit=unit, customer=customer,
                 created_at=created_at, created_by=user,
                 description=descr,
-                last4=receipt_info.get('last4'),
+                last4=last4,
                 exp_date=receipt_info.get('exp_date'),
                 card_name=receipt_info.get('card_name', ""))
             for invoiced in transactions:
                 # XXX Here we need to associate the (invoice_key, sync_on)
                 # to the ChargeItem.
                 ChargeItem.objects.create(invoiced=invoiced, charge=charge,
                     invoice_key=getattr(invoiced, 'invoice_key', None),
@@ -1574,14 +1577,17 @@
 
     # XXX unique together paid and invoiced.
     # customer and invoiced_items account payble should match.
 
     def __str__(self):
         return str(self.processor_key)
 
+    def get_last4_display(self):
+        return '%04d' % self.last4
+
     @property
     def broker_fee_amount(self):
         if not hasattr(self, '_broker_fee_amount'):
             self._broker_fee_amount = 0
             for charge_item in self.charge_items.all():
                 invoiced_item = charge_item.invoiced
                 if invoiced_item.subscription:
@@ -1792,22 +1798,22 @@
         self.state = self.DONE
         signals.charge_updated.send(sender=__name__, charge=self, user=None)
 
     def failed(self, receipt_info=None):
         assert self.state == self.CREATED
         kwargs = {}
         if receipt_info:
-            kwargs.update({
-                'last4': receipt_info.get('last4'),
-                'exp_date': receipt_info.get('exp_date'),
-                'card_name': receipt_info.get('card_name', "")
-            })
-            self.last4 = receipt_info.get('last4')
+            self.last4 = int(receipt_info.get('last4'))
             self.exp_date = receipt_info.get('exp_date')
             self.card_name = receipt_info.get('card_name', "")
+            kwargs.update({
+                'last4': self.last4,
+                'exp_date': self.exp_date,
+                'card_name': self.card_name
+            })
         with transaction.atomic():
             updated = Charge.objects.select_for_update(nowait=True).filter(
                 pk=self.pk, state=self.CREATED).update(
                     state=self.FAILED, **kwargs)
             if not updated:
                 raise DatabaseError(
                     "Charge is currently being updated by another transaction")
@@ -1887,22 +1893,22 @@
                 cowork:Funds                          $156.78
                 stripe:Funds
         """
         #pylint: disable=too-many-locals,too-many-statements
         assert self.state == self.CREATED
         kwargs = {}
         if receipt_info:
-            kwargs.update({
-                'last4': receipt_info.get('last4'),
-                'exp_date': receipt_info.get('exp_date'),
-                'card_name': receipt_info.get('card_name', "")
-            })
-            self.last4 = receipt_info.get('last4')
+            self.last4 = int(receipt_info.get('last4'))
             self.exp_date = receipt_info.get('exp_date')
             self.card_name = receipt_info.get('card_name', "")
+            kwargs.update({
+                'last4': self.last4,
+                'exp_date': self.exp_date,
+                'card_name': self.card_name
+            })
         with transaction.atomic():
             # up at the top of this method so that we bail out quickly, before
             # we start to mistakenly enter the charge and distributions a second
             # time on two rapid fire `Charge.retrieve()` calls.
             updated = Charge.objects.select_for_update(nowait=True).filter(
                 pk=self.pk, state=self.CREATED).update(
                     state=self.DONE, **kwargs)
@@ -3427,23 +3433,16 @@
                 orig_balance=Sum('dest_amount'),
                 last_activity_at=Max('created_at')).order_by(
                     'last_activity_at', '-event_id')
         for orig_balance in orig_balances:
             orig_amount = orig_balance['orig_balance']
             orig_unit = orig_balance['dest_unit']
             event_id = orig_balance['event_id']
-            if event_id.startswith('cpn_'):
-                # XXX group buy events should certainly be re-written as sub_.
-                continue
-            if not event_id.startswith('sub_'):
-                LOGGER.error("event_id '%s' does not start with 'sub_'"\
-                    " in get_statement_balances", event_id)
-            assert event_id.startswith('sub_')
-            # We should always have subscription events in orig_balances
-            # by the definition of the SQL query.
+            # We could have subscription or group-buy (coupon codes) events
+            # in both dest_balances and orig_balances.
             balance_by_units = dest_balance_per_events.get(event_id, {})
             if orig_unit in balance_by_units:
                 balance_by_units.update({
                     orig_unit: balance_by_units[orig_unit] - orig_amount})
 
         balances = {}
         for event_id, balance in six.iteritems(dest_balance_per_events):
```

### Comparing `djaodjin-saas-0.9.4/saas/pagination.py` & `djaodjin-saas-0.9.5/saas/pagination.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/renewals.py` & `djaodjin-saas-0.9.5/saas/renewals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/settings.py` & `djaodjin-saas-0.9.5/saas/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/signals.py` & `djaodjin-saas-0.9.5/saas/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/static/js/djaodjin-postal.js` & `djaodjin-saas-0.9.5/saas/static/js/djaodjin-postal.js`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/static/js/djaodjin-resources-vue.js` & `djaodjin-saas-0.9.5/saas/static/js/djaodjin-resources-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/static/js/djaodjin-resources.js` & `djaodjin-saas-0.9.5/saas/static/js/djaodjin-resources.js`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/static/js/djaodjin-saas-angular.js` & `djaodjin-saas-0.9.5/saas/static/js/djaodjin-saas-angular.js`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/static/js/djaodjin-saas-vue.js` & `djaodjin-saas-0.9.5/saas/static/js/djaodjin-saas-vue.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020, DjaoDjin inc.
+// Copyright (c) 2021, DjaoDjin inc.
 // All rights reserved.
 // BSD 2-Clause license
 
 /*global Vue jQuery moment interpolate gettext showMessages showErrorMessages Stripe updateBarChart updateChart getUrlParameter $ */
 
 
 Vue.filter('formatDate', function(value, format) {
@@ -438,14 +438,15 @@
     ],
     data: function() {
         return $.extend({ // XXX jQuery
             api_card_url: this.$urls.organization.api_card,
             api_profile_url: this.$urls.organization.api_base,
             processor_pub_key: null,
             stripe_intent_secret: null,
+            stripe_account: null,
             stripe: null,
             cardNumber: '',
             cardCvc: '',
             cardExpMonth: '',
             cardExpYear: '',
             card_name: '',
             card_address_line1: '',
@@ -471,23 +472,25 @@
                 'card_address_line1',
                 'card_city',
                 'card_address_zip',
                 'country',
                 'region',
             ],
             labels: {
-                cardNumberLabel: gettext("Card Number"),
-                securityCodeLabel: gettext("Security Code"),
-                expirationLabel: gettext("Expiration"),
-                cardHolderLabel: gettext("Card Holder"),
-                streetAddressLabel: gettext("Street address"),
-                localityLabel: gettext("City/Town"),
-                regionLabel: gettext("State/Province/County"),
-                postalCodeLabel: gettext("Zip/Postal code"),
-                countryLabel: gettext("Country")
+                cardNumberLabel: (this.$labels && this.$labels.cardNumberLabel) || "Card Number",
+                securityCodeLabel: (this.$labels && this.$labels.securityCodeLabel) || "Security Code",
+                expirationLabel: (this.$labels && this.$labels.expirationLabel) || "Expiration",
+                cardHolderLabel: (this.$labels && this.$labels.cardHolderLabel) || "Card Holder",
+                streetAddressLabel: (this.$labels && this.$labels.streetAddressLabel) || "Street address",
+                localityLabel: (this.$labels && this.$labels.localityLabel) || "City/Town",
+                regionLabel: (this.$labels && this.$labels.regionLabel) || "State/Province/County",
+                postalCodeLabel: (this.$labels && this.$labels.postalCodeLabel) || "Zip/Postal code",
+                countryLabel: (this.$labels && this.$labels.countryLabel) || "Country",
+                fieldShoundNotBeEmptyError: (this.$labels && this.$labels.fieldShoundNotBeEmptyError) || "This field shouldn't be empty",
+                fieldsCannotBeEmptyError: (this.$labels && this.$labels.fieldsCannotBeEmptyError) || " field(s) cannot be empty."
             }
         }, this.getCardFormData());
     },
     methods: {
         getCardFormData: function() {
             var vm = this;
             var data = {};
@@ -561,16 +564,25 @@
                     }
                     if (resp.processor && resp.processor.STRIPE_PUB_KEY) {
                         vm.processor_pub_key = resp.processor.STRIPE_PUB_KEY;
                     }
                     if (resp.processor && resp.processor.STRIPE_INTENT_SECRET) {
                         vm.stripe_intent_secret = resp.processor.STRIPE_INTENT_SECRET;
                     }
+                    if (resp.processor && resp.processor.STRIPE_ACCOUNT) {
+                        vm.stripe_account = resp.processor.STRIPE_ACCOUNT;
+                    }
                     if (vm.processor_pub_key) {
-                        vm.stripe = Stripe(vm.processor_pub_key);
+                        if (vm.stripe_account) {
+                            vm.stripe = Stripe(vm.processor_pub_key, {
+                                stripeAccount: vm.stripe_account
+                            });
+                        } else {
+                            vm.stripe = Stripe(vm.processor_pub_key);
+                        }
                         if (vm.stripe_intent_secret) {
                             var elements = vm.stripe.elements();
                             vm.cardElement = elements.create("card", {
                                 hidePostalCode: true
                             });
                             vm.cardElement.mount("#card-element");
                         }
@@ -578,17 +590,15 @@
                 });
         },
         getCardToken: function(cb) {
             var vm = this;
             // this identifies your website in the createToken call below
             if (vm.stripe_intent_secret) {
                 if (!vm.stripe) {
-                    showMessages([
-                        gettext("You haven't set a valid Stripe public key")
-                    ], "error");
+                    showErrorMessages("You haven't set a valid Stripe public key");
                     return;
                 }
                 if (vm.stripe_intent_secret.substring(0, 3) === 'pi_') {
                     vm.stripe.confirmCardPayment(
                         vm.stripe_intent_secret, {
                             payment_method: {
                                 type: "card",
@@ -700,15 +710,15 @@
             var errorMessages = "";
             vm.validate.forEach(function(field) {
                 if (vm[field] === '') {
                     vm[field] = vm.getInitValue($(vm.$el), field); //XXX jQuery
                 }
                 if (vm[field] === '') {
                     valid = false;
-                    errors[field] = [gettext("This field shouldn't be empty")];
+                    errors[field] = [vm.labels.fieldShoundNotBeEmptyError];
                 }
             });
             vm.errors = errors;
             if (Object.keys(vm.errors).length > 0) {
                 if (vm.errors['cardNumber']) {
                     if (errorMessages) {
                         errorMessages += ", ";
@@ -761,16 +771,15 @@
                 if (vm.errors['region']) {
                     if (errorMessages) {
                         errorMessages += ", ";
                     }
                     errorMessages += vm.labels.postalCodeLabel;
                 }
                 if (errorMessages) {
-                    errorMessages = interpolate(
-                        gettext("%s field(s) cannot be empty."), [errorMessages]);
+                    errorMessages = errorMessages + vm.labels.fieldsCannotBeEmptyError;
                 }
                 showErrorMessages(errorMessages);
             }
             return valid;
         },
     },
     computed: {
@@ -788,16 +797,23 @@
         elements = vm.$el.querySelectorAll('[data-exp-date]');
         if (elements.length > 0) {
             vm.savedCard.exp_date = elements[0].getAttribute('data-exp-date');
         }
         vm.processor_pub_key = vm.$el.getAttribute('data-processor-pub-key');
         vm.stripe_intent_secret = vm.$el.getAttribute(
             'data-stripe-intent-secret');
+        vm.stripe_account = vm.$el.getAttribute('data-stripe-account');
         if (vm.processor_pub_key) {
-            vm.stripe = Stripe(vm.processor_pub_key);
+            if (vm.stripe_account) {
+                vm.stripe = Stripe(vm.processor_pub_key, {
+                    stripeAccount: vm.stripe_account
+                });
+            } else {
+                vm.stripe = Stripe(vm.processor_pub_key);
+            }
             if (vm.stripe_intent_secret) {
                 var elements = vm.stripe.elements();
                 vm.cardElement = elements.create("card", {
                     hidePostalCode: true
                 });
                 vm.cardElement.mount("#card-element");
             }
@@ -1930,16 +1946,16 @@
         cardMixin,
         itemListMixin,
     ],
     data: function() {
         var res = {
             url: this.$urls.organization.api_transactions,
             api_cancel_balance_url: this.$urls.organization.api_cancel_balance_due,
-            last4: gettext("N/A"),
-            exp_date: gettext("N/A"),
+            last4: (this.$labels && this.$labels.notAvailableLabel) || "N/A",
+            exp_date: (this.$labels && this.$labels.notAvailableLabel) || "N/A",
             cardLoaded: false
         }
         return res;
     },
     methods: {
         getCard: function() {
             var vm = this;
@@ -1988,17 +2004,17 @@
         itemListMixin,
     ],
     data: function() {
         return {
             url: this.$urls.organization.api_transactions,
             api_balance_url: this.$urls.provider.api_bank,
             balanceLoaded: false,
-            last4: gettext("N/A"),
-            bank_name: gettext("N/A"),
-            balance_amount: gettext("N/A"),
+            last4: (this.$labels && this.$labels.notAvailableLabel) || "N/A",
+            bank_name: (this.$labels && this.$labels.notAvailableLabel) || "N/A",
+            balance_amount: (this.$labels && this.$labels.notAvailableLabel) || "N/A",
             balance_unit: '',
         }
     },
     methods: {
         getBalance: function() {
             var vm = this;
             vm.reqGet(vm.api_balance_url,
@@ -2326,16 +2342,18 @@
                 sync_on: user.email
             }
             var option = vm.plansOption[plan];
             if (option) {
                 data.option = option
             }
             vm.reqPost(vm.api_cart_url, data,
-                function() {
-                    showMessages([gettext("User was added.")], "success");
+                function(resp) {
+                    if (resp.detail) {
+                        showMessages([resp.detail], "success");
+                    }
                     vm.init = false;
                     vm.$set(vm.plansUser, plan, {
                         fullName: '',
                         email: ''
                     });
                     vm.get();
                 });
```

### Comparing `djaodjin-saas-0.9.4/saas/static/js/djaodjin-saas.js` & `djaodjin-saas-0.9.5/saas/static/js/djaodjin-saas.js`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/static/js/djaodjin-stripe.js` & `djaodjin-saas-0.9.5/saas/static/js/djaodjin-stripe.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -101,16 +101,15 @@
                 }
                 errorMessages += self.options.routingNumberLabel;
                 routingNumberElement.parents(
                     ".form-group").addClass("has-error");
                 valid = false;
             }
             if (errorMessages) {
-                errorMessages = interpolate(
-                    self.options.fieldsCannotBeEmptyError, [errorMessages]);
+                errorMessages = errorMessages + self.options.fieldsCannotBeEmptyError;
             }
             if (valid) {
                 // this identifies your website in the createToken call below
                 Stripe.setPublishableKey(self.options.stripePubKey);
                 Stripe.bankAccount.createToken({
                     country: country,
                     routingNumber: routingNumber,
@@ -133,15 +132,15 @@
     };
 
     $.fn.bank.defaults = {
         stripePubKey: null,
         countryLabel: "Country",
         accountNumberLabel: "Account Number",
         routingNumberLabel: "Routing Number",
-        fieldsCannotBeEmptyError: gettext("%s field(s) cannot be empty.")
+        fieldsCannotBeEmptyError: " field(s) cannot be empty."
     };
 
     /** Augment a <form> to request a token from a credit card, then submit
         the form with that token.
 
         usage:
             $("#payment-form").card({stripePubKey: *YourStripePublicKey*});
@@ -198,16 +197,21 @@
             var self = this;
         },
     };
 
     Card.prototype = {
         init: function() {
             var self = this;
-
-            self.stripe = Stripe(self.options.stripePubKey);
+            if (self.options.stripeAccount) {
+                self.stripe = Stripe(self.options.stripePubKey, {
+                    stripeAccount: self.options.stripeAccount
+                });
+            } else {
+                self.stripe = Stripe(self.options.stripePubKey);
+            }
             if (self.options.stripeIntentSecret) {
                 var elements = self.stripe.elements();
                 self.cardElement = elements.create("card", {
                     hidePostalCode: true
                 });
                 self.cardElement.mount("#card-element");
             }
@@ -423,16 +427,15 @@
                 }
                 errorMessages += self.options.countryLabel;
                 addressCountryElement.parents(
                     ".form-group").addClass("has-error");
                 valid = false;
             }
             if (errorMessages) {
-                errorMessages = interpolate(
-                    self.options.fieldsCannotBeEmptyError, [errorMessages]);
+                errorMessages = errorMessages + self.options.fieldsCannotBeEmptyError;
             }
             if (valid) {
                 // this identifies your website in the createToken call below
                 if (self.options.stripeIntentSecret) {
                     if (self.options.stripeIntentSecret.substring(0, 3) === 'pi_') {
                         self.stripe.confirmCardPayment(
                             self.options.stripeIntentSecret, {
@@ -509,22 +512,23 @@
         var opts = $.extend({}, $.fn.card.defaults, options);
         return new Card($(this), opts);
     };
 
     $.fn.card.defaults = {
         stripePubKey: null,
         stripeIntentSecret: null,
+        stripeAccount: null,
         saas_api_card: null,
         cardNumberLabel: "Card Number",
         securityCodeLabel: "Security Code",
         expirationLabel: "Expiration",
         cardHolderLabel: "Card Holder",
         streetAddressLabel: "Street address",
         localityLabel: "City/Town",
         regionLabel: "State/Province/County",
         postalCodeLabel: "Zip/Postal code",
         countryLabel: "Country",
-        fieldsCannotBeEmptyError: gettext("%s field(s) cannot be empty.")
+        fieldsCannotBeEmptyError: " field(s) cannot be empty."
     };
 
 
 })(jQuery);
```

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/_bank_use.html` & `djaodjin-saas-0.9.5/saas/templates/saas/_bank_use.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/_card_use.html` & `djaodjin-saas-0.9.5/saas/templates/saas/_card_use.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/_charges.html` & `djaodjin-saas-0.9.5/saas/templates/saas/_charges.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/_invoiceables.html` & `djaodjin-saas-0.9.5/saas/templates/saas/_invoiceables.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/_paginator.html` & `djaodjin-saas-0.9.5/saas/templates/saas/_paginator.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/_razorpay_checkout.html` & `djaodjin-saas-0.9.5/saas/templates/saas/_razorpay_checkout.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/_sidebar.html` & `djaodjin-saas-0.9.5/saas/templates/saas/_sidebar.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/_transactions.html` & `djaodjin-saas-0.9.5/saas/templates/saas/_transactions.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/agreements/security.md` & `djaodjin-saas-0.9.5/saas/templates/saas/agreements/security.md`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/agreements/terms-of-use.md` & `djaodjin-saas-0.9.5/saas/templates/saas/agreements/terms-of-use.md`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/base.html` & `djaodjin-saas-0.9.5/saas/templates/saas/base.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/base_dashboard.html` & `djaodjin-saas-0.9.5/saas/templates/saas/base_dashboard.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/balance.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/balance.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/bank.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/bank.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/card.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/card.html`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 {% block saas_content %}
 <card-update inline-template id="update-card-container"
     data-processor-pub-key="{{STRIPE_PUB_KEY}}"
     {% if STRIPE_INTENT_SECRET %}
     data-stripe-intent-secret="{{STRIPE_INTENT_SECRET}}"
     {% endif %}
+    {% if STRIPE_ACCOUNT %}
+    data-stripe-account="{{STRIPE_ACCOUNT}}"
+    {% endif %}
   >
   <div>
     <h1>Update Card for {{ organization }}</h1>
     <form id="update-card" method="post"
         action=".{% if next %}/?next={{next}}{% endif %}"
         v-on:submit.prevent="save">
         <input type="hidden" name="csrfmiddlewaretoken" value="{{csrf_token}}">
```

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/cart.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/cart.html`

 * *Files 3% similar despite different names*

```diff
@@ -62,13 +62,14 @@
              saas_api_cart: "{{ urls.api_cart }}" });
     }
 {% endif %}
 {% if STRIPE_PUB_KEY %}
     cardForm.card({
         stripePubKey: "{{ STRIPE_PUB_KEY }}",
         stripeIntentSecret: {% if STRIPE_INTENT_SECRET %}"{{ STRIPE_INTENT_SECRET }}"{% else %}null{% endif %},
+        stripeAccount: {% if STRIPE_ACCOUNT %}"{{ STRIPE_ACCOUNT }}"{% else %}null{% endif %},
         saas_api_card: "{{ urls.organization.api_card }}"
     });
 {% endif %}
 });
 </script>
 {% endblock %}
```

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/checkout.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/checkout.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/coupons.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/coupons.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/import.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/import.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/index.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/receipt.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/receipt.html`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,19 @@
     </dl>
     <dl>
       <dt>amount</dt>
       <dd id="amount-info">{{charge.price|humanize_money}}</dd>
     </dl>
     <dl>
       <dt>card</dt>
-      <dd>**** - {{charge.last4}}</dd>
+      <dd>**** - {{last4}}</dd>
     </dl>
     <dl>
       <dt>expires</dt>
-      <dd>{{charge.exp_date}}</dd>
+      <dd>{{exp_date}}</dd>
     </dl>
   </section>
   <section id="invoiced_items">
     <table>
       <thead>
         <tr>
           <th>Amount</th>
```

#### html2text {}

```diff
@@ -7,17 +7,17 @@
 charge failed. {% elif charge.is_disputed %} The charge was disputed. {% elif
 charge.is_progress %} The charge is in progress... {% endif %}
   REFERENCE
       #{{ charge.processor_key }}
   amount
       {{charge.price|humanize_money}}
   card
-      **** - {{charge.last4}}
+      **** - {{last4}}
   expires
-      {{charge.exp_date}}
+      {{exp_date}}
 AAmmoouunntt                                     DDeessccrriippttiioonn
                                                                      {% if
                                                                      line.refundable
 {                                          {                         and
 {line.invoiced.dest_price|humanize_money}} {line.invoiced|describe}} charge.state ==
                                                                      charge.DONE %}
                                                                      Refund {% endif
```

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/transactions.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/transactions.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/transfers.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/transfers.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/billing/withdraw.html` & `djaodjin-saas-0.9.5/saas/templates/saas/billing/withdraw.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/legal/index.html` & `djaodjin-saas-0.9.5/saas/templates/saas/legal/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/metrics/balances.html` & `djaodjin-saas-0.9.5/saas/templates/saas/metrics/balances.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/metrics/base.html` & `djaodjin-saas-0.9.5/saas/templates/saas/metrics/base.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/metrics/coupons.html` & `djaodjin-saas-0.9.5/saas/templates/saas/metrics/coupons.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/metrics/dashboard.html` & `djaodjin-saas-0.9.5/saas/templates/saas/metrics/dashboard.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/pricing.html` & `djaodjin-saas-0.9.5/saas/templates/saas/pricing.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/printable_charge_receipt.html` & `djaodjin-saas-0.9.5/saas/templates/saas/printable_charge_receipt.html`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,19 @@
       </tr>
       <tr>
         <th class="info-row-header">AMOUNT&nbsp;&nbsp;</th>
         <td>{{charge.price|humanize_money}}</td>
       </tr>
       <tr>
         <th class="info-row-header">CARD&nbsp;&nbsp;</th>
-        <td>**** - {{charge.last4}}</td>
+        <td>**** - {{last4}}</td>
       </tr>
       <tr>
         <th class="info-row-header">EXPIRES&nbsp;&nbsp;</th>
-        <td>{{charge.exp_date}}</td>
+        <td>{{exp_date}}</td>
       </tr>
     </tbody>
   </table>
 </div>
 <hr>
 <div id="invoiced_items">
     <table>
```

#### html2text {}

```diff
@@ -17,16 +17,16 @@
 {charge.price|humanize_money}}. The charge was disputed.
 {% elif charge.is_progress %}
 On {{charge.created_at}}, we attempted to charge your card for {
 {charge.price|humanize_money}}. The charge is in progress...
 {% endif %}
 RREEFFEERREENNCCEE? ?  #{{charge.processor_key}}
 AAMMOOUUNNTT? ?     {{charge.price|humanize_money}}
-CCAARRDD? ?       **** - {{charge.last4}}
-EEXXPPIIRREESS? ?    {{charge.exp_date}}
+CCAARRDD? ?       **** - {{last4}}
+EEXXPPIIRREESS? ?    {{exp_date}}
 ===============================================================================
 AAmmoouunntt                                      DDeessccrriippttiioonn
 {{line.invoiced.dest_price|humanize_money}} {{line.invoiced|describe}}
 -{{refund.orig_price|humanize_money}}       {{refund|describe}}
 ===============================================================================
 Thank you for your continued business. If you have any questions or comments,
 email us at _{_{_p_r_o_v_i_d_e_r_._e_m_a_i_l_}_}.
```

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/profile/index.html` & `djaodjin-saas-0.9.5/saas/templates/saas/profile/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/profile/roles/index.html` & `djaodjin-saas-0.9.5/saas/templates/saas/profile/roles/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/profile/roles/role.html` & `djaodjin-saas-0.9.5/saas/templates/saas/profile/roles/role.html`

 * *Files 3% similar despite different names*

```diff
@@ -43,21 +43,19 @@
       </tbody>
     </table>
     <!-- modal -->
     <hr />
     <div>
       <h2>Invite user to have a role '{{role_descr.title}}' on {{organization.printable_name}}</h2>
       <form id="add-user" ng-submit="save($event)"
-            @submit.prevent="submit">
+           @submit.prevent="submit">
         <input type="hidden" name="csrfmiddlewaretoken" value="{{csrf_token}}">
         <input type="text" name="user" placeholder="Username or e-mail"
                ng-model="unregistered.slug" v-model="unregistered.slug" />
-        <div class="add-role-modal"
-            ng-click="create($event)"
-            @submit.prevent="submit">
+        <div class="add-role-modal" v-show="profileRequestDone">
           <p>
 If the user couldn't be found in the system, it is a great occasion to invite
 them.
           </p>
           <div>
             <label>To</label>
             <input type="text" max-length="150"
```

#### html2text {}

```diff
@@ -11,16 +11,15 @@
                                        click="sendInvite(item.user.slug)" v-
 [[item.user.slug]]  [                  if="item.grant_key">Re-send            click="remove
                     [item.user.email]] click="save(item.user)" v-             (index)">Remove
                                        if="item.accept_request_api_url">Grant
 ===============================================================================
 ********** IInnvviittee uusseerr ttoo hhaavvee aa rroollee ''{{{{rroollee__ddeessccrr..ttiittllee}}}}'' oonn {{
 {{oorrggaanniizzaattiioonn..pprriinnttaabbllee__nnaammee}}}} **********
-submit.prevent="submit"> [user                ]
-submit.prevent="submit">
+submit.prevent="submit">[user                ]
 If the user couldn't be found in the system, it is a great occasion to invite
 them.
 To[email               ]
 The following invite message will be sent along
 Hello, I am adding you as a {{role_descr.title}} to {
 {organization.printable_name}}. Thank you, - {{request.user.first_name}}
 Submit
```

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/profile/subscribers.html` & `djaodjin-saas-0.9.5/saas/templates/saas/profile/subscribers.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/profile/subscriptions.html` & `djaodjin-saas-0.9.5/saas/templates/saas/profile/subscriptions.html`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/templates/saas/users/roles.html` & `djaodjin-saas-0.9.5/saas/templates/saas/users/roles.html`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,15 @@
                autocomplete="off"
                ng-model="unregistered.slug"
                v-model="unregistered.slug"
                uib-typeahead="item.slug for item in getCandidates($viewValue)"
                uib-typeahead-loading="loadingOrganizations"
                uib-typeahead-template-url="customTemplate.html" />
         <button type="submit" name="submit">Add</button>
-      </form>
-      <div>
-        <form id="add-profile" @submit.prevent="submit" ng-submit="create($event)">
+        <div id="add-profile" v-show="profileRequestDone">
           <p ng-model="unregistered">
 [[unregistered.full_name]] was not found. This is an opportunity to invite
 a manager for [[unregistered.full_name]] to join {{organization.printable_name}}.
           </p>
           <label>To</label>
           <input id="new-request-email" name="email"
                  type="text" max-length="150"
@@ -76,14 +74,14 @@
 
 I would like to request access to [[unregistered.full_name]].
 
 Thank you,
 - {{request.user.first_name}}
           </textarea>
           <button type="submit">Request access</button>
-        </form>
-      </div>
+        </div>
+      </form>
     </div>
     <!-- end of modal dialog -->
   </div>
 </role-profile-list>
 {% endblock %}
```

#### html2text {}

```diff
@@ -11,13 +11,12 @@
                                      [[entry.request_key ? "requested" :
 [                                    entry.role_description.title]]         click="remove
 [entry.organization.printable_name]] click="acceptGrant(entry)" v-          (index)">remove
                                      if="entry.accept_grant_api_url">accept
 {% include "saas/_paginator.html" %}
 ****** RReeqquueesstt aacccceessss ...... ******
 submit.prevent="submit" ng-submit="save($event)"> [organization        ]Add
-submit.prevent="submit" ng-submit="create($event)">
 [[unregistered.full_name]] was not found. This is an opportunity to invite a
 manager for [[unregistered.full_name]] to join {{organization.printable_name}}.
 
 Request access
 {% endblock %}
```

### Comparing `djaodjin-saas-0.9.4/saas/templatetags/saas_tags.py` & `djaodjin-saas-0.9.5/saas/templatetags/saas_tags.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/tests.py` & `djaodjin-saas-0.9.5/saas/tests.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/__init__.py` & `djaodjin-saas-0.9.5/saas/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/__init__.py` & `djaodjin-saas-0.9.5/saas/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/broker.py` & `djaodjin-saas-0.9.5/saas/urls/api/broker.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/cart.py` & `djaodjin-saas-0.9.5/saas/urls/api/cart.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/legal.py` & `djaodjin-saas-0.9.5/saas/urls/api/legal.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/provider/__init__.py` & `djaodjin-saas-0.9.5/saas/urls/api/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/provider/billing.py` & `djaodjin-saas-0.9.5/saas/urls/api/provider/billing.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/provider/charges.py` & `djaodjin-saas-0.9.5/saas/urls/api/provider/charges.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/provider/metrics.py` & `djaodjin-saas-0.9.5/saas/urls/api/provider/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/provider/plans.py` & `djaodjin-saas-0.9.5/saas/urls/api/provider/plans.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/provider/roles.py` & `djaodjin-saas-0.9.5/saas/urls/api/provider/roles.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/provider/subscribers.py` & `djaodjin-saas-0.9.5/saas/urls/api/provider/subscribers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/search.py` & `djaodjin-saas-0.9.5/saas/urls/api/search.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/subscriber/__init__.py` & `djaodjin-saas-0.9.5/saas/urls/api/subscriber/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/subscriber/billing.py` & `djaodjin-saas-0.9.5/saas/urls/api/subscriber/billing.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/subscriber/charges.py` & `djaodjin-saas-0.9.5/saas/urls/api/subscriber/charges.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/subscriber/profile.py` & `djaodjin-saas-0.9.5/saas/urls/api/subscriber/profile.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/subscriber/roles.py` & `djaodjin-saas-0.9.5/saas/urls/api/subscriber/roles.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/api/users.py` & `djaodjin-saas-0.9.5/saas/urls/api/users.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/broker.py` & `djaodjin-saas-0.9.5/saas/urls/broker.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/noauth.py` & `djaodjin-saas-0.9.5/saas/urls/noauth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/provider/__init__.py` & `djaodjin-saas-0.9.5/saas/urls/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/provider/billing.py` & `djaodjin-saas-0.9.5/saas/urls/provider/billing.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/provider/metrics.py` & `djaodjin-saas-0.9.5/saas/urls/provider/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/provider/profile.py` & `djaodjin-saas-0.9.5/saas/urls/provider/profile.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/redirects.py` & `djaodjin-saas-0.9.5/saas/urls/redirects.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/request.py` & `djaodjin-saas-0.9.5/saas/urls/request.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/subscriber/__init__.py` & `djaodjin-saas-0.9.5/saas/urls/subscriber/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/subscriber/billing/__init__.py` & `djaodjin-saas-0.9.5/saas/urls/subscriber/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/subscriber/billing/info.py` & `djaodjin-saas-0.9.5/saas/urls/subscriber/billing/info.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/subscriber/billing/payment.py` & `djaodjin-saas-0.9.5/saas/urls/subscriber/billing/payment.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/subscriber/profile.py` & `djaodjin-saas-0.9.5/saas/urls/subscriber/profile.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/urls/users.py` & `djaodjin-saas-0.9.5/saas/urls/users.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/utils.py` & `djaodjin-saas-0.9.5/saas/utils.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/views/__init__.py` & `djaodjin-saas-0.9.5/saas/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/views/billing.py` & `djaodjin-saas-0.9.5/saas/views/billing.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/views/download.py` & `djaodjin-saas-0.9.5/saas/views/download.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/views/extra.py` & `djaodjin-saas-0.9.5/saas/views/extra.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/views/legal.py` & `djaodjin-saas-0.9.5/saas/views/legal.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/views/metrics.py` & `djaodjin-saas-0.9.5/saas/views/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/views/optins.py` & `djaodjin-saas-0.9.5/saas/views/optins.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/views/plans.py` & `djaodjin-saas-0.9.5/saas/views/plans.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/views/profile.py` & `djaodjin-saas-0.9.5/saas/views/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 Manage Profile information
 """
 import logging
 
 from django import http
 from django.contrib import messages
 from django.contrib.auth import REDIRECT_FIELD_NAME
+from django.core.exceptions import ValidationError
 from django.db import IntegrityError, transaction
 from django.views.generic import (CreateView, DetailView, ListView,
     TemplateView, UpdateView)
-from django.utils.decorators import method_decorator
 
 from . import RedirectFormMixin
 from .. import settings, signals
 from ..compat import reverse, NoReverseMatch
 from ..decorators import _valid_manager
 from ..forms import (OrganizationForm, OrganizationCreateForm,
     ManagerAndOrganizationForm)
@@ -54,15 +54,15 @@
     """
     List of users with a specific role for an organization.
 
     Template:
 
     To edit the layout of this page, create a local \
     ``saas/profile/roles/role.html`` (`example <https://github.com/djaodjin\
-/djaodjin-saas/tree/master/saas/templates/saas/profile/roles.html>`__).
+/djaodjin-saas/tree/master/saas/templates/saas/profile/roles/role.html>`__).
     You should insure the page will call back the
     :ref:`/api/profile/:organization/roles/:role/ <api_role>`
     API end point to fetch the set of users with the specified role.
 
     Template context:
       - ``role_descr`` Description of the role that defines
         the permissions of users on an organization
@@ -364,56 +364,68 @@
     Template context:
       - ``urls.organization.password_chage`` URL to update user password.
       - ``organization`` The organization object
       - ``request`` The HTTP request object
     """
 
     model = get_organization_model()
+    form_class = OrganizationForm
     slug_field = 'slug'
     slug_url_kwarg = 'organization'
     template_name = "saas/profile/index.html"
 
-    @method_decorator(transaction.atomic)
+    def update_attached_user(self, form):
+        validated_data = form.cleaned_data
+        user = self.object.attached_user()
+        if user:
+            user.username = validated_data.get('slug', user.username)
+            user.email = validated_data.get('email', user.email)
+            if update_db_row(user, form):
+                raise ValidationError("update_attached_user")
+        return user
+
     def form_valid(self, form):
         validated_data = form.cleaned_data
         # Calls `get_object()` such that we get the actual values present
         # in the database. `self.object` will contain the updated values
         # at this point.
         changes = self.get_object().get_changes(validated_data)
-        user = self.object.attached_user()
-        if user:
-            user.username = validated_data.get('slug', user.username)
         self.object.slug = validated_data.get('slug', self.object.slug)
         self.object.full_name = validated_data['full_name']
         self.object.email = validated_data['email']
         if 'is_bulk_buyer' in validated_data:
             self.object.is_bulk_buyer = validated_data['is_bulk_buyer']
         else:
             self.object.is_bulk_buyer = False
         if 'extra' in validated_data:
             self.object.extra = validated_data['extra']
         is_provider = self.object.is_provider
         if _valid_manager(self.request, [get_broker()]):
             self.object.is_provider = validated_data.get(
                 'is_provider', is_provider)
 
-        form.save(commit=False)
-        if update_db_row(self.object, form):
+        try:
+            with transaction.atomic():
+                self.update_attached_user(form)
+                if update_db_row(self.object, form):
+                    raise ValidationError("form_valid")
+        except ValidationError:
             return self.form_invalid(form)
+
         signals.organization_updated.send(sender=__name__,
                 organization=self.object, changes=changes,
                 user=self.request.user)
         return http.HttpResponseRedirect(self.get_success_url())
 
     def get_form_class(self):
         if self.object.attached_user():
             # There is only one user so we will add the User fields
             # to the form so they can be updated at the same time.
             return ManagerAndOrganizationForm
-        return OrganizationForm
+        return super(OrganizationProfileView, self).get_form_class()
 
     def get_initial(self):
         kwargs = super(OrganizationProfileView, self).get_initial()
         if Plan.objects.exists():
             # Do not display the bulk buying option if there are no plans.
             kwargs.update({'is_bulk_buyer': self.object.is_bulk_buyer})
         if _valid_manager(self.request, [get_broker()]):
```

### Comparing `djaodjin-saas-0.9.4/saas/views/redirects.py` & `djaodjin-saas-0.9.5/saas/views/redirects.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from django.utils.translation import ugettext_lazy as _
 from django.views.generic import RedirectView
 from django.views.generic.base import ContextMixin, TemplateResponseMixin
 from django.views.generic.edit import FormMixin
 
 from .. import settings
 from ..cart import session_cart_to_database
-from ..compat import reverse, NoReverseMatch
+from ..compat import is_authenticated, reverse, NoReverseMatch
 from ..decorators import fail_direct
 from ..models import RoleDescription, get_broker
 from ..utils import (get_organization_model, get_role_model,
     update_context_urls, validate_redirect_url as validate_redirect_url_base)
 
 
 LOGGER = logging.getLogger(__name__)
@@ -166,14 +166,18 @@
             organization = self.organization_model.objects.filter(
                 email__endswith=domain).get()
         return user, organization
 
     def get(self, request, *args, **kwargs):
         #pylint:disable=too-many-locals,too-many-statements
         #pylint:disable=too-many-nested-blocks,too-many-return-statements
+        if not is_authenticated(request):
+            # If we got here and the user is not authenticated, it is pointless.
+            return http.HttpResponseRedirect(settings.LOGIN_URL)
+
         session_cart_to_database(request)
 
         redirect_to = reverse('saas_user_product_list', args=(request.user,))
         next_url = self.request.GET.get(REDIRECT_FIELD_NAME, None)
         if next_url:
             redirect_to += '?%s=%s' % (REDIRECT_FIELD_NAME, next_url)
```

### Comparing `djaodjin-saas-0.9.4/saas/views/roles.py` & `djaodjin-saas-0.9.5/saas/views/roles.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/saas/views/users.py` & `djaodjin-saas-0.9.5/saas/views/users.py`

 * *Files identical despite different names*

### Comparing `djaodjin-saas-0.9.4/setup.py` & `djaodjin-saas-0.9.5/setup.py`

 * *Files identical despite different names*

