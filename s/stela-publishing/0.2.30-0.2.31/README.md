# Comparing `tmp/stela_publishing-0.2.30.tar.gz` & `tmp/stela_publishing-0.2.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stela_publishing-0.2.30.tar", last modified: Tue Apr 23 18:09:20 2024, max compression
+gzip compressed data, was "stela_publishing-0.2.31.tar", last modified: Thu May  2 18:23:15 2024, max compression
```

## Comparing `stela_publishing-0.2.30.tar` & `stela_publishing-0.2.31.tar`

### file list

```diff
@@ -1,423 +1,423 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:20.625573 stela_publishing-0.2.30/
--rw-rw-rw-   0        0        0    35803 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/LICENSE
--rw-rw-rw-   0        0        0      133 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/MANIFEST.in
--rw-rw-rw-   0        0        0     3241 2024-04-23 18:09:20.581601 stela_publishing-0.2.30/PKG-INFO
--rw-rw-rw-   0        0        0     2058 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.338956 stela_publishing-0.2.30/accounts/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/accounts/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/accounts/admin.py
--rw-rw-rw-   0        0        0      154 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/accounts/apps.py
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/accounts/forms.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.343953 stela_publishing-0.2.30/accounts/migrations/
--rw-rw-rw-   0        0        0     4062 2024-01-29 16:48:12.000000 stela_publishing-0.2.30/accounts/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-29 16:48:12.000000 stela_publishing-0.2.30/accounts/migrations/__init__.py
--rw-rw-rw-   0        0        0     4733 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/accounts/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/accounts/tests.py
--rw-rw-rw-   0        0        0      370 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/accounts/token.py
--rw-rw-rw-   0        0        0     1836 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/accounts/urls.py
--rw-rw-rw-   0        0        0    10979 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/accounts/views.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.364012 stela_publishing-0.2.30/cloud/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/cloud/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/cloud/admin.py
--rw-rw-rw-   0        0        0      148 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/cloud/apps.py
--rw-rw-rw-   0        0        0     3456 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/cloud/cart.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.369005 stela_publishing-0.2.30/cloud/migrations/
--rw-rw-rw-   0        0        0     5564 2024-01-29 16:48:24.000000 stela_publishing-0.2.30/cloud/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-29 16:48:24.000000 stela_publishing-0.2.30/cloud/migrations/__init__.py
--rw-rw-rw-   0        0        0     3508 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/cloud/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/cloud/tests.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/cloud/views.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.385996 stela_publishing-0.2.30/geolocation/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/geolocation/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/geolocation/admin.py
--rw-rw-rw-   0        0        0      160 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/geolocation/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.390992 stela_publishing-0.2.30/geolocation/migrations/
--rw-rw-rw-   0        0        0     6403 2024-01-29 16:48:36.000000 stela_publishing-0.2.30/geolocation/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-29 16:48:36.000000 stela_publishing-0.2.30/geolocation/migrations/__init__.py
--rw-rw-rw-   0        0        0      582 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/geolocation/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/geolocation/tests.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.30/geolocation/views.py
--rw-rw-rw-   0        0        0       42 2024-04-23 18:09:20.625573 stela_publishing-0.2.30/setup.cfg
--rw-rw-rw-   0        0        0     1394 2024-04-23 18:07:30.000000 stela_publishing-0.2.30/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.495170 stela_publishing-0.2.30/stela_control/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/__init__.py
--rw-rw-rw-   0        0        0       34 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/admin.py
--rw-rw-rw-   0        0        0      163 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/apps.py
--rw-rw-rw-   0        0        0     7541 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/cart.py
--rw-rw-rw-   0        0        0      164 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/context_processors.py
--rw-rw-rw-   0        0        0      316 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/cron.py
--rw-rw-rw-   0        0        0    74884 2024-04-23 18:00:07.000000 stela_publishing-0.2.30/stela_control/forms.py
--rw-rw-rw-   0        0        0      181 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.134338 stela_publishing-0.2.30/stela_control/locale/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.134338 stela_publishing-0.2.30/stela_control/locale/es/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.506165 stela_publishing-0.2.30/stela_control/locale/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0    59691 2024-02-12 17:42:58.000000 stela_publishing-0.2.30/stela_control/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0   376901 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/locale/es/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.644570 stela_publishing-0.2.30/stela_control/migrations/
--rw-rw-rw-   0        0        0    85798 2024-01-29 16:48:50.000000 stela_publishing-0.2.30/stela_control/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     7914 2024-02-07 18:48:34.000000 stela_publishing-0.2.30/stela_control/migrations/0002_rename_response_chatsupport_content_and_more.py
--rw-rw-rw-   0        0        0     7300 2024-02-10 15:04:52.000000 stela_publishing-0.2.30/stela_control/migrations/0003_rename_logo_company_alter_logo_and_more.py
--rw-rw-rw-   0        0        0     6916 2024-02-10 16:34:10.000000 stela_publishing-0.2.30/stela_control/migrations/0004_content_video_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     5651 2024-02-10 16:49:33.000000 stela_publishing-0.2.30/stela_control/migrations/0005_rename_description_team_content_and_more.py
--rw-rw-rw-   0        0        0     6881 2024-02-13 00:43:29.000000 stela_publishing-0.2.30/stela_control/migrations/0006_content_cover_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     6174 2024-02-13 00:46:55.000000 stela_publishing-0.2.30/stela_control/migrations/0007_content_fecade_url_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     6925 2024-02-20 21:45:50.000000 stela_publishing-0.2.30/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6664 2024-02-26 16:53:17.000000 stela_publishing-0.2.30/stela_control/migrations/0009_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5955 2024-02-28 16:33:58.000000 stela_publishing-0.2.30/stela_control/migrations/0010_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6006 2024-02-28 16:39:48.000000 stela_publishing-0.2.30/stela_control/migrations/0011_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6714 2024-02-28 16:47:02.000000 stela_publishing-0.2.30/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6809 2024-02-28 16:55:43.000000 stela_publishing-0.2.30/stela_control/migrations/0013_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5972 2024-02-28 17:37:52.000000 stela_publishing-0.2.30/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6686 2024-02-28 19:01:16.000000 stela_publishing-0.2.30/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5617 2024-02-28 19:16:55.000000 stela_publishing-0.2.30/stela_control/migrations/0016_remove_sociallinks_url_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     6432 2024-02-28 19:17:57.000000 stela_publishing-0.2.30/stela_control/migrations/0017_sociallinks_social_url_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     7209 2024-04-23 16:47:22.000000 stela_publishing-0.2.30/stela_control/migrations/0018_inventory_condition_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     6726 2024-04-23 17:33:11.000000 stela_publishing-0.2.30/stela_control/migrations/0019_inventory_amazon_published_date_and_more.py
--rw-rw-rw-   0        0        0     6283 2024-04-23 18:01:51.000000 stela_publishing-0.2.30/stela_control/migrations/0020_remove_inventory_amazon_published_date_and_more.py
--rw-rw-rw-   0        0        0     5941 2024-04-23 18:02:34.000000 stela_publishing-0.2.30/stela_control/migrations/0021_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0        0 2024-01-29 16:48:50.000000 stela_publishing-0.2.30/stela_control/migrations/__init__.py
--rw-rw-rw-   0        0        0    68389 2024-04-23 18:02:23.000000 stela_publishing-0.2.30/stela_control/models.py
--rw-rw-rw-   0        0        0     2943 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/routers.py
--rw-rw-rw-   0        0        0   144613 2024-04-20 17:01:45.000000 stela_publishing-0.2.30/stela_control/superfunctions.py
--rw-rw-rw-   0        0        0      410 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/tasks.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.136337 stela_publishing-0.2.30/stela_control/templates/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.743595 stela_publishing-0.2.30/stela_control/templates/stela_control/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.761582 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/
--rw-rw-rw-   0        0        0      497 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/base.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.799558 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/registration/
--rw-rw-rw-   0        0        0      227 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/registration/account_activation_email.html
--rw-rw-rw-   0        0        0       21 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/registration/activation_invalid.html
--rw-rw-rw-   0        0        0     1373 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/registration/confirmation_email.html
--rw-rw-rw-   0        0        0     3071 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/registration/register.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.875512 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/
--rw-rw-rw-   0        0        0     1364 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/delete_user.html
--rw-rw-rw-   0        0        0     2813 2024-02-04 17:29:27.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/login.html
--rw-rw-rw-   0        0        0     2692 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html
--rw-rw-rw-   0        0        0     2043 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/password_reset_done.html
--rw-rw-rw-   0        0        0      629 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/password_reset_email.html
--rw-rw-rw-   0        0        0     2424 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/password_reset_form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.893001 stela_publishing-0.2.30/stela_control/templates/stela_control/analytics/
--rw-rw-rw-   0        0        0      757 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/analytics/analytics.html
--rw-rw-rw-   0        0        0      527 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/analytics/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.903997 stela_publishing-0.2.30/stela_control/templates/stela_control/api/
--rw-rw-rw-   0        0        0     5932 2024-01-15 04:03:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/api/main.html
--rw-rw-rw-   0        0        0     2817 2024-02-13 00:06:24.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/base.html
--rw-rw-rw-   0        0        0     4402 2024-02-07 14:19:14.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/base_content.html
--rw-rw-rw-   0        0        0     6768 2024-02-07 14:19:37.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/base_list.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.915989 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/
--rw-rw-rw-   0        0        0   240584 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/homebrew.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.172832 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/
--rw-rw-rw-   0        0        0     2186 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/bill-data-customer.html
--rw-rw-rw-   0        0        0    30854 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/checkout.html
--rw-rw-rw-   0        0        0      906 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/data-customer.html
--rw-rw-rw-   0        0        0    56802 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/invoice-copy.html
--rw-rw-rw-   0        0        0    56693 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/invoice.html
--rw-rw-rw-   0        0        0     2875 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/order-placed.html
--rw-rw-rw-   0        0        0    48008 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/preview-recipt.html
--rw-rw-rw-   0        0        0     2750 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html
--rw-rw-rw-   0        0        0     3336 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/recipt-detail.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.186823 stela_publishing-0.2.30/stela_control/templates/stela_control/chatstela/
--rw-rw-rw-   0        0        0    30842 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/chatstela/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.256441 stela_publishing-0.2.30/stela_control/templates/stela_control/content/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.298417 stela_publishing-0.2.30/stela_control/templates/stela_control/content/comments/
--rw-rw-rw-   0        0        0     7574 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/content/comments/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.321400 stela_publishing-0.2.30/stela_control/templates/stela_control/content/docs/
--rw-rw-rw-   0        0        0    15755 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/content/docs/main.html
--rw-rw-rw-   0        0        0     7448 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/content/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.339390 stela_publishing-0.2.30/stela_control/templates/stela_control/content/main/
--rw-rw-rw-   0        0        0     1003 2024-02-28 11:49:02.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/content/main/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.352380 stela_publishing-0.2.30/stela_control/templates/stela_control/content/staff/
--rw-rw-rw-   0        0        0     7608 2024-02-10 16:45:07.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/content/staff/index.html
--rw-rw-rw-   0        0        0    26830 2024-02-23 18:59:08.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/content/stelastory.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.368370 stela_publishing-0.2.30/stela_control/templates/stela_control/developer/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.426957 stela_publishing-0.2.30/stela_control/templates/stela_control/developer/data-update/
--rw-rw-rw-   0        0        0      933 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/developer/data-update/modal1.html
--rw-rw-rw-   0        0        0      898 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/developer/data-update/modal2.html
--rw-rw-rw-   0        0        0      900 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/developer/data-update/modal3.html
--rw-rw-rw-   0        0        0      875 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/developer/data-update/modal4.html
--rw-rw-rw-   0        0        0    46793 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/developer/home.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.192519 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.438949 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/accounts/
--rw-rw-rw-   0        0        0      413 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/accounts/password_reset_email.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.461936 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/billing/
--rw-rw-rw-   0        0        0    21938 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html
--rw-rw-rw-   0        0        0    21903 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/billing/invoice.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.516901 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/contact/
--rw-rw-rw-   0        0        0    20096 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/contact/message_notification.html
--rw-rw-rw-   0        0        0    29872 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/contact/message_response.html
--rw-rw-rw-   0        0        0     8454 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/contact/support_notification.html
--rw-rw-rw-   0        0        0    21428 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/contact/update_support.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.528894 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/marketing/
--rw-rw-rw-   0        0        0    60992 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.556877 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/newsletter/
--rw-rw-rw-   0        0        0    21461 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html
--rw-rw-rw-   0        0        0    21883 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/newsletter/success.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.650818 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/
--rw-rw-rw-   0        0        0    10226 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html
--rw-rw-rw-   0        0        0    10337 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_express_placed.html
--rw-rw-rw-   0        0        0    57366 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_order_placed.html
--rw-rw-rw-   0        0        0    57419 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_order_placed2.html
--rw-rw-rw-   0        0        0    57320 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves.html
--rw-rw-rw-   0        0        0    57419 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves2.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.739763 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/
--rw-rw-rw-   0        0        0    27770 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/billing_payment.html
--rw-rw-rw-   0        0        0     6930 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/charges.html
--rw-rw-rw-   0        0        0    20151 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/payment_notification.html
--rw-rw-rw-   0        0        0    20151 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/sale_notification.html
--rw-rw-rw-   0        0        0     7266 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html
--rw-rw-rw-   0        0        0     7166 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/withdrawals.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.772743 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/support/
--rw-rw-rw-   0        0        0    20072 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/support/support_notification.html
--rw-rw-rw-   0        0        0    20096 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/support/support_response.html
--rw-rw-rw-   0        0        0    22210 2024-02-23 18:58:52.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/home.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.791734 stela_publishing-0.2.30/stela_control/templates/stela_control/inbox/
--rw-rw-rw-   0        0        0     7530 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/inbox/index.html
--rw-rw-rw-   0        0        0     8900 2024-02-10 15:38:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.199514 stela_publishing-0.2.30/stela_control/templates/stela_control/inventory/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:16.810721 stela_publishing-0.2.30/stela_control/templates/stela_control/inventory/journals/
--rw-rw-rw-   0        0        0     6289 2024-02-08 17:58:31.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/inventory/journals/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.141516 stela_publishing-0.2.30/stela_control/templates/stela_control/inventory/publishing/
--rw-rw-rw-   0        0        0     6897 2024-02-26 22:43:48.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/inventory/publishing/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.600052 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.610045 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/aboutemmerut/
--rw-rw-rw-   0        0        0     1694 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.623036 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/aboutsecondary/
--rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.634031 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/aboutstela/
--rw-rw-rw-   0        0        0     1381 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/aboutstela/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.644025 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/appstela/
--rw-rw-rw-   0        0        0     1806 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/appstela/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.207509 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/auth/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.663012 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/auth/pw_reset/
--rw-rw-rw-   0        0        0       45 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/auth/pw_reset/form_errors.html
--rw-rw-rw-   0        0        0      171 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/auth/pw_reset/password_reset_form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.679002 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/auth/signup/
--rw-rw-rw-   0        0        0      794 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html
--rw-rw-rw-   0        0        0      269 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/auth/signup/success_register.html
--rw-rw-rw-   0        0        0     3005 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/blog-feed.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.684998 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/categories/
--rw-rw-rw-   0        0        0      834 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/categories/modal4.html
--rw-rw-rw-   0        0        0      826 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/chatbox.html
--rw-rw-rw-   0        0        0      925 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/chatbox2.html
--rw-rw-rw-   0        0        0      143 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/city_data.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.695992 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/colors/
--rw-rw-rw-   0        0        0      857 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/colors/modal2.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.706985 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/contact/
--rw-rw-rw-   0        0        0     1606 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/contact/modal.html
--rw-rw-rw-   0        0        0     1638 2024-01-22 20:05:28.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/dynamic-formset.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.718978 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/emmerutfooter/
--rw-rw-rw-   0        0        0     2233 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.753957 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/emmerutservices/
--rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html
--rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html
--rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html
--rw-rw-rw-   0        0        0      841 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/form-base.html
--rw-rw-rw-   0        0        0       64 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/form-errors.html
--rw-rw-rw-   0        0        0       45 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/form.html
--rw-rw-rw-   0        0        0      924 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/formset-base-services.html
--rw-rw-rw-   0        0        0     1790 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/formset-base.html
--rw-rw-rw-   0        0        0      816 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/formset.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.213504 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/handlers/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.796931 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/handlers/blog/
--rw-rw-rw-   0        0        0     1488 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages.html
--rw-rw-rw-   0        0        0      128 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/handlers/blog/empty-blog.html
--rw-rw-rw-   0        0        0      265 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/handlers/blog/empy-blog.html
--rw-rw-rw-   0        0        0      103 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/hashtags.html
--rw-rw-rw-   0        0        0      587 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/instagram-alert.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.830909 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/inventory/
--rw-rw-rw-   0        0        0     2029 2024-02-27 00:20:27.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html
--rw-rw-rw-   0        0        0      777 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/inventory/simple-form.html
--rw-rw-rw-   0        0        0     1578 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/inventory/simple-formset.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.841902 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/job-application/
--rw-rw-rw-   0        0        0       45 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/job-application/error-form-v1.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:17.846899 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/linkzoneupdates/
--rw-rw-rw-   0        0        0      848 2024-01-15 04:03:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.220549 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.023790 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/
--rw-rw-rw-   0        0        0     1067 2024-02-23 15:58:42.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html
--rw-rw-rw-   0        0        0     1467 2024-02-23 16:29:50.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html
--rw-rw-rw-   0        0        0     1650 2024-02-23 18:05:44.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     2732 2024-02-23 18:06:01.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     2477 2024-02-23 18:05:57.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html
--rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:06.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html
--rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:10.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     2887 2024-02-23 18:06:18.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2593 2024-02-23 18:06:24.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2296 2024-02-23 18:06:30.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1639 2024-02-23 18:06:35.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2803 2024-02-23 18:06:42.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.188688 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/
--rw-rw-rw-   0        0        0     1614 2024-02-23 18:04:43.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     3292 2024-02-23 18:04:45.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     3051 2024-02-23 18:04:50.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html
--rw-rw-rw-   0        0        0     1936 2024-02-23 18:04:55.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html
--rw-rw-rw-   0        0        0     2198 2024-02-23 18:05:01.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     2866 2024-02-23 18:05:07.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2737 2024-02-23 18:05:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2418 2024-02-23 18:05:17.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1412 2024-02-23 18:07:47.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2803 2024-02-23 18:05:27.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html
--rw-rw-rw-   0        0        0     1297 2024-02-23 15:56:06.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html
--rw-rw-rw-   0        0        0     1778 2024-02-23 16:29:34.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.392278 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/
--rw-rw-rw-   0        0        0     1069 2024-02-23 15:58:34.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html
--rw-rw-rw-   0        0        0     1464 2024-02-23 16:29:44.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html
--rw-rw-rw-   0        0        0     1962 2024-02-23 18:06:50.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     3022 2024-02-23 18:06:54.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     2815 2024-02-23 18:07:00.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html
--rw-rw-rw-   0        0        0     1740 2024-02-23 18:07:07.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html
--rw-rw-rw-   0        0        0     2080 2024-02-23 18:07:11.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     3148 2024-02-23 18:07:16.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2631 2024-02-23 18:07:22.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2489 2024-02-23 18:07:28.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1929 2024-02-23 18:07:33.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2803 2024-02-23 18:07:38.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.437001 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.455989 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/community/
--rw-rw-rw-   0        0        0      818 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/community/formdata.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.461986 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/content-pro-media/
--rw-rw-rw-   0        0        0     3209 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.485972 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/content-pro-update/
--rw-rw-rw-   0        0        0       83 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/content-pro-update/content.html
--rw-rw-rw-   0        0        0       84 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/content-pro-update/schedule.html
--rw-rw-rw-   0        0        0      986 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.503960 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ic-update/
--rw-rw-rw-   0        0        0      469 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ic-update/content.html
--rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.569920 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/
--rw-rw-rw-   0        0        0    25077 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html
--rw-rw-rw-   0        0        0     1667 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html
--rw-rw-rw-   0        0        0     1530 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html
--rw-rw-rw-   0        0        0     1849 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html
--rw-rw-rw-   0        0        0     1774 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html
--rw-rw-rw-   0        0        0     4485 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html
--rw-rw-rw-   0        0        0     5787 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.584910 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/meta-assets/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page-alert.html
--rw-rw-rw-   0        0        0      628 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.620888 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/page-analythics/
--rw-rw-rw-   0        0        0     1755 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html
--rw-rw-rw-   0        0        0     1960 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html
--rw-rw-rw-   0        0        0     1428 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.637877 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/smart-boost/
--rw-rw-rw-   0        0        0     2129 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.648871 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/stela-sight/
--rw-rw-rw-   0        0        0      268 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/stela-sight/data.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.654867 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/newcomer/
--rw-rw-rw-   0        0        0     3796 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/newcomer/form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.671857 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/post/
--rw-rw-rw-   0        0        0      846 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/post/list-modal.html
--rw-rw-rw-   0        0        0      850 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/post/main-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.701839 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/
--rw-rw-rw-   0        0        0     1824 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/catalog-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.773794 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/
--rw-rw-rw-   0        0        0      933 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/catalog-form.html
--rw-rw-rw-   0        0        0      872 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/category-form.html
--rw-rw-rw-   0        0        0      888 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/color-form.html
--rw-rw-rw-   0        0        0     1024 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/product-form.html
--rw-rw-rw-   0        0        0      855 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/size-form.html
--rw-rw-rw-   0        0        0      115 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/variant-form.html
--rw-rw-rw-   0        0        0      805 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/product-modal.html
--rw-rw-rw-   0        0        0      848 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/size-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.851746 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/update/
--rw-rw-rw-   0        0        0      234 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/update/catalog-form.html
--rw-rw-rw-   0        0        0      287 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/update/category-form.html
--rw-rw-rw-   0        0        0      230 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/update/color-form.html
--rw-rw-rw-   0        0        0     1008 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/update/product-form.html
--rw-rw-rw-   0        0        0      228 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/update/size-form.html
--rw-rw-rw-   0        0        0      234 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/update/variant-form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.906713 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/profile/
--rw-rw-rw-   0        0        0     1306 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/profile/dynamic-form.html
--rw-rw-rw-   0        0        0      200 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/profile/single-form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.916706 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/projects/
--rw-rw-rw-   0        0        0     1698 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/projects/modal.html
--rw-rw-rw-   0        0        0      260 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/remove-complete.html
--rw-rw-rw-   0        0        0      212 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/single-form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.282672 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.940691 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/
--rw-rw-rw-   0        0        0     1099 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.965676 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/error_forms/
--rw-rw-rw-   0        0        0     1099 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:18.998654 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/forms/
--rw-rw-rw-   0        0        0     1269 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html
--rw-rw-rw-   0        0        0     1097 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.023640 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/update_forms/
--rw-rw-rw-   0        0        0     1156 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html
--rw-rw-rw-   0        0        0     1320 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.037631 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/staff/
--rw-rw-rw-   0        0        0     1947 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/staff/form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.067613 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stela_story/
--rw-rw-rw-   0        0        0     3404 2024-02-21 12:50:07.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stela_story/feed-item.html
--rw-rw-rw-   0        0        0     2001 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.081605 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stelafooter/
--rw-rw-rw-   0        0        0     2176 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stelafooter/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.102592 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stelamedia/
--rw-rw-rw-   0        0        0     1695 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stelamedia/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.120580 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stelapath/
--rw-rw-rw-   0        0        0     1337 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stelapath/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.136571 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/youtube/
--rw-rw-rw-   0        0        0      157 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/youtube/video-preview.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.289940 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.240042 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/email-marketing/
--rw-rw-rw-   0        0        0     2345 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/email-marketing/email_list.html
--rw-rw-rw-   0        0        0     1774 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/email-marketing/emails_list.html
--rw-rw-rw-   0        0        0     1917 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/email-marketing/new_email.html
--rw-rw-rw-   0        0        0      976 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/email-marketing/update_email.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.254034 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/
--rw-rw-rw-   0        0        0    10789 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:15.291939 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/instagram/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.687051 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/
--rw-rw-rw-   0        0        0    13445 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.711038 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/
--rw-rw-rw-   0        0        0    23333 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.748149 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/
--rw-rw-rw-   0        0        0    34272 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.816107 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.829100 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/community/
--rw-rw-rw-   0        0        0    14156 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.918046 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/
--rw-rw-rw-   0        0        0    30243 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html
--rw-rw-rw-   0        0        0      248 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/update.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.928040 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/
--rw-rw-rw-   0        0        0     3162 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html
--rw-rw-rw-   0        0        0    12633 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html
--rw-rw-rw-   0        0        0    17640 2024-02-12 17:40:18.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/newcomer.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:19.975011 stela_publishing-0.2.30/stela_control/templates/stela_control/orders/
--rw-rw-rw-   0        0        0     6171 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/orders/list_view.html
--rw-rw-rw-   0        0        0     8860 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/orders/order_update.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:20.097934 stela_publishing-0.2.30/stela_control/templates/stela_control/payments/
--rw-rw-rw-   0        0        0    43167 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/payments/homebrew.html
--rw-rw-rw-   0        0        0     2687 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/payments/register-wallet.html
--rw-rw-rw-   0        0        0     4322 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/payments/wallet-list.html
--rw-rw-rw-   0        0        0     2831 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/payments/withdraw.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:20.110925 stela_publishing-0.2.30/stela_control/templates/stela_control/prostela/
--rw-rw-rw-   0        0        0      153 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/prostela/chatbox.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:20.122919 stela_publishing-0.2.30/stela_control/templates/stela_control/prostela-expert/
--rw-rw-rw-   0        0        0    34014 2024-01-15 04:03:12.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/prostela-expert/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:20.205867 stela_publishing-0.2.30/stela_control/templates/stela_control/reviews/
--rw-rw-rw-   0        0        0     3170 2024-01-15 04:03:13.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/reviews/reviews_list.html
--rw-rw-rw-   0        0        0     1325 2024-01-15 04:03:13.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/reviews/update_review.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:20.231227 stela_publishing-0.2.30/stela_control/templates/stela_control/support/
--rw-rw-rw-   0        0        0     2061 2024-01-15 04:03:13.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/support/list.html
--rw-rw-rw-   0        0        0     7093 2024-01-15 04:03:13.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/support/update.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:20.500651 stela_publishing-0.2.30/stela_control/templates/stela_control/users/
--rw-rw-rw-   0        0        0      339 2024-01-18 10:28:40.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/users/generic-user-handler.html
--rw-rw-rw-   0        0        0    11181 2024-01-22 21:22:30.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/users/profile.html
--rw-rw-rw-   0        0        0    12343 2024-02-06 16:52:33.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/users/users-control.html
--rw-rw-rw-   0        0        0     6472 2024-02-06 15:00:39.000000 stela_publishing-0.2.30/stela_control/templates/stela_control/users/users.html
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:20.519639 stela_publishing-0.2.30/stela_control/templatetags/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:13.000000 stela_publishing-0.2.30/stela_control/templatetags/__init__.py
--rw-rw-rw-   0        0        0     1277 2024-01-19 05:09:17.000000 stela_publishing-0.2.30/stela_control/templatetags/stelatags.py
--rw-rw-rw-   0        0        0      507 2024-01-15 04:03:13.000000 stela_publishing-0.2.30/stela_control/tests.py
--rw-rw-rw-   0        0        0     1131 2024-01-15 04:03:13.000000 stela_publishing-0.2.30/stela_control/tokenize.py
--rw-rw-rw-   0        0        0     5281 2024-02-20 00:45:02.000000 stela_publishing-0.2.30/stela_control/urls.py
--rw-rw-rw-   0        0        0   211317 2024-02-20 00:48:27.000000 stela_publishing-0.2.30/stela_control/views.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:09:20.563611 stela_publishing-0.2.30/stela_publishing.egg-info/
--rw-rw-rw-   0        0        0     3241 2024-04-23 18:09:14.000000 stela_publishing-0.2.30/stela_publishing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    20966 2024-04-23 18:09:15.000000 stela_publishing-0.2.30/stela_publishing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:09:14.000000 stela_publishing-0.2.30/stela_publishing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      355 2024-04-23 18:09:14.000000 stela_publishing-0.2.30/stela_publishing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2024-04-23 18:09:14.000000 stela_publishing-0.2.30/stela_publishing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:15.444083 stela_publishing-0.2.31/
+-rw-rw-rw-   0        0        0    35803 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/LICENSE
+-rw-rw-rw-   0        0        0      133 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/MANIFEST.in
+-rw-rw-rw-   0        0        0     3241 2024-05-02 18:23:15.441085 stela_publishing-0.2.31/PKG-INFO
+-rw-rw-rw-   0        0        0     2058 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.163198 stela_publishing-0.2.31/accounts/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/accounts/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/accounts/admin.py
+-rw-rw-rw-   0        0        0      154 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/accounts/apps.py
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/accounts/forms.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.168195 stela_publishing-0.2.31/accounts/migrations/
+-rw-rw-rw-   0        0        0     4062 2024-01-29 16:48:12.000000 stela_publishing-0.2.31/accounts/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-29 16:48:12.000000 stela_publishing-0.2.31/accounts/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4733 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/accounts/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/accounts/tests.py
+-rw-rw-rw-   0        0        0      370 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/accounts/token.py
+-rw-rw-rw-   0        0        0     1836 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/accounts/urls.py
+-rw-rw-rw-   0        0        0    10979 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/accounts/views.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.190181 stela_publishing-0.2.31/cloud/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/cloud/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/cloud/admin.py
+-rw-rw-rw-   0        0        0      148 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/cloud/apps.py
+-rw-rw-rw-   0        0        0     3456 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/cloud/cart.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.197177 stela_publishing-0.2.31/cloud/migrations/
+-rw-rw-rw-   0        0        0     5564 2024-01-29 16:48:24.000000 stela_publishing-0.2.31/cloud/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-29 16:48:24.000000 stela_publishing-0.2.31/cloud/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3508 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/cloud/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/cloud/tests.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/cloud/views.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.214167 stela_publishing-0.2.31/geolocation/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/geolocation/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/geolocation/admin.py
+-rw-rw-rw-   0        0        0      160 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/geolocation/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.220164 stela_publishing-0.2.31/geolocation/migrations/
+-rw-rw-rw-   0        0        0     6403 2024-01-29 16:48:36.000000 stela_publishing-0.2.31/geolocation/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-29 16:48:36.000000 stela_publishing-0.2.31/geolocation/migrations/__init__.py
+-rw-rw-rw-   0        0        0      582 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/geolocation/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/geolocation/tests.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.31/geolocation/views.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 18:23:15.445083 stela_publishing-0.2.31/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2024-05-02 18:22:57.000000 stela_publishing-0.2.31/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.272131 stela_publishing-0.2.31/stela_control/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/__init__.py
+-rw-rw-rw-   0        0        0       34 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/admin.py
+-rw-rw-rw-   0        0        0      163 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/apps.py
+-rw-rw-rw-   0        0        0     7541 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/cart.py
+-rw-rw-rw-   0        0        0      164 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/context_processors.py
+-rw-rw-rw-   0        0        0      316 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/cron.py
+-rw-rw-rw-   0        0        0    74895 2024-05-02 18:17:25.000000 stela_publishing-0.2.31/stela_control/forms.py
+-rw-rw-rw-   0        0        0      181 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.004297 stela_publishing-0.2.31/stela_control/locale/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.005296 stela_publishing-0.2.31/stela_control/locale/es/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.306167 stela_publishing-0.2.31/stela_control/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    59691 2024-02-12 17:42:58.000000 stela_publishing-0.2.31/stela_control/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0   376901 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/locale/es/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.407106 stela_publishing-0.2.31/stela_control/migrations/
+-rw-rw-rw-   0        0        0    85798 2024-01-29 16:48:50.000000 stela_publishing-0.2.31/stela_control/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     7914 2024-02-07 18:48:34.000000 stela_publishing-0.2.31/stela_control/migrations/0002_rename_response_chatsupport_content_and_more.py
+-rw-rw-rw-   0        0        0     7300 2024-02-10 15:04:52.000000 stela_publishing-0.2.31/stela_control/migrations/0003_rename_logo_company_alter_logo_and_more.py
+-rw-rw-rw-   0        0        0     6916 2024-02-10 16:34:10.000000 stela_publishing-0.2.31/stela_control/migrations/0004_content_video_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     5651 2024-02-10 16:49:33.000000 stela_publishing-0.2.31/stela_control/migrations/0005_rename_description_team_content_and_more.py
+-rw-rw-rw-   0        0        0     6881 2024-02-13 00:43:29.000000 stela_publishing-0.2.31/stela_control/migrations/0006_content_cover_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     6174 2024-02-13 00:46:55.000000 stela_publishing-0.2.31/stela_control/migrations/0007_content_fecade_url_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     6925 2024-02-20 21:45:50.000000 stela_publishing-0.2.31/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6664 2024-02-26 16:53:17.000000 stela_publishing-0.2.31/stela_control/migrations/0009_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5955 2024-02-28 16:33:58.000000 stela_publishing-0.2.31/stela_control/migrations/0010_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6006 2024-02-28 16:39:48.000000 stela_publishing-0.2.31/stela_control/migrations/0011_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6714 2024-02-28 16:47:02.000000 stela_publishing-0.2.31/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6809 2024-02-28 16:55:43.000000 stela_publishing-0.2.31/stela_control/migrations/0013_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5972 2024-02-28 17:37:52.000000 stela_publishing-0.2.31/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6686 2024-02-28 19:01:16.000000 stela_publishing-0.2.31/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5617 2024-02-28 19:16:55.000000 stela_publishing-0.2.31/stela_control/migrations/0016_remove_sociallinks_url_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     6432 2024-02-28 19:17:57.000000 stela_publishing-0.2.31/stela_control/migrations/0017_sociallinks_social_url_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     7209 2024-04-23 16:47:22.000000 stela_publishing-0.2.31/stela_control/migrations/0018_inventory_condition_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     6726 2024-04-23 17:33:11.000000 stela_publishing-0.2.31/stela_control/migrations/0019_inventory_amazon_published_date_and_more.py
+-rw-rw-rw-   0        0        0     6283 2024-04-23 18:01:51.000000 stela_publishing-0.2.31/stela_control/migrations/0020_remove_inventory_amazon_published_date_and_more.py
+-rw-rw-rw-   0        0        0     5941 2024-04-23 18:02:34.000000 stela_publishing-0.2.31/stela_control/migrations/0021_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0        0 2024-01-29 16:48:50.000000 stela_publishing-0.2.31/stela_control/migrations/__init__.py
+-rw-rw-rw-   0        0        0    68445 2024-05-02 18:17:10.000000 stela_publishing-0.2.31/stela_control/models.py
+-rw-rw-rw-   0        0        0     2943 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/routers.py
+-rw-rw-rw-   0        0        0   144613 2024-04-20 17:01:45.000000 stela_publishing-0.2.31/stela_control/superfunctions.py
+-rw-rw-rw-   0        0        0      410 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/tasks.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.009293 stela_publishing-0.2.31/stela_control/templates/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.711504 stela_publishing-0.2.31/stela_control/templates/stela_control/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.739485 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/
+-rw-rw-rw-   0        0        0      497 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/base.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.829431 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/registration/
+-rw-rw-rw-   0        0        0      227 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/registration/account_activation_email.html
+-rw-rw-rw-   0        0        0       21 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/registration/activation_invalid.html
+-rw-rw-rw-   0        0        0     1373 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/registration/confirmation_email.html
+-rw-rw-rw-   0        0        0     3071 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/registration/register.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:05.155231 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/
+-rw-rw-rw-   0        0        0     1364 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/delete_user.html
+-rw-rw-rw-   0        0        0     2813 2024-02-04 17:29:27.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/login.html
+-rw-rw-rw-   0        0        0     2692 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html
+-rw-rw-rw-   0        0        0     2043 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/password_reset_done.html
+-rw-rw-rw-   0        0        0      629 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/password_reset_email.html
+-rw-rw-rw-   0        0        0     2424 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/password_reset_form.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:05.198204 stela_publishing-0.2.31/stela_control/templates/stela_control/analytics/
+-rw-rw-rw-   0        0        0      757 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/analytics/analytics.html
+-rw-rw-rw-   0        0        0      527 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/analytics/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:05.262164 stela_publishing-0.2.31/stela_control/templates/stela_control/api/
+-rw-rw-rw-   0        0        0     5932 2024-01-15 04:03:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/api/main.html
+-rw-rw-rw-   0        0        0     2817 2024-02-13 00:06:24.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/base.html
+-rw-rw-rw-   0        0        0     4402 2024-02-07 14:19:14.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/base_content.html
+-rw-rw-rw-   0        0        0     6768 2024-02-07 14:19:37.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/base_list.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:05.430062 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/
+-rw-rw-rw-   0        0        0   240584 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/homebrew.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:05.922313 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/
+-rw-rw-rw-   0        0        0     2186 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/bill-data-customer.html
+-rw-rw-rw-   0        0        0    30854 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/checkout.html
+-rw-rw-rw-   0        0        0      906 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/data-customer.html
+-rw-rw-rw-   0        0        0    56802 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/invoice-copy.html
+-rw-rw-rw-   0        0        0    56693 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/invoice.html
+-rw-rw-rw-   0        0        0     2875 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/order-placed.html
+-rw-rw-rw-   0        0        0    48008 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/preview-recipt.html
+-rw-rw-rw-   0        0        0     2750 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html
+-rw-rw-rw-   0        0        0     3336 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/recipt-detail.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:05.982275 stela_publishing-0.2.31/stela_control/templates/stela_control/chatstela/
+-rw-rw-rw-   0        0        0    30842 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/chatstela/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:06.093207 stela_publishing-0.2.31/stela_control/templates/stela_control/content/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:06.157170 stela_publishing-0.2.31/stela_control/templates/stela_control/content/comments/
+-rw-rw-rw-   0        0        0     7574 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/content/comments/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:06.206138 stela_publishing-0.2.31/stela_control/templates/stela_control/content/docs/
+-rw-rw-rw-   0        0        0    15755 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/content/docs/main.html
+-rw-rw-rw-   0        0        0     7448 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/content/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:06.280094 stela_publishing-0.2.31/stela_control/templates/stela_control/content/main/
+-rw-rw-rw-   0        0        0     1003 2024-02-28 11:49:02.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/content/main/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:06.586481 stela_publishing-0.2.31/stela_control/templates/stela_control/content/staff/
+-rw-rw-rw-   0        0        0     7608 2024-02-10 16:45:07.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/content/staff/index.html
+-rw-rw-rw-   0        0        0    26830 2024-02-23 18:59:08.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/content/stelastory.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:06.700419 stela_publishing-0.2.31/stela_control/templates/stela_control/developer/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:06.823334 stela_publishing-0.2.31/stela_control/templates/stela_control/developer/data-update/
+-rw-rw-rw-   0        0        0      933 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/developer/data-update/modal1.html
+-rw-rw-rw-   0        0        0      898 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/developer/data-update/modal2.html
+-rw-rw-rw-   0        0        0      900 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/developer/data-update/modal3.html
+-rw-rw-rw-   0        0        0      875 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/developer/data-update/modal4.html
+-rw-rw-rw-   0        0        0    46793 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/developer/home.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.035277 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:06.847318 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/accounts/
+-rw-rw-rw-   0        0        0      413 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/accounts/password_reset_email.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:06.960250 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/billing/
+-rw-rw-rw-   0        0        0    21938 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html
+-rw-rw-rw-   0        0        0    21903 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/billing/invoice.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:07.125149 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/contact/
+-rw-rw-rw-   0        0        0    20096 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/contact/message_notification.html
+-rw-rw-rw-   0        0        0    29872 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/contact/message_response.html
+-rw-rw-rw-   0        0        0     8454 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/contact/support_notification.html
+-rw-rw-rw-   0        0        0    21428 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/contact/update_support.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:07.183113 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/marketing/
+-rw-rw-rw-   0        0        0    60992 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:07.246075 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/newsletter/
+-rw-rw-rw-   0        0        0    21461 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html
+-rw-rw-rw-   0        0        0    21883 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/newsletter/success.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:07.574425 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/
+-rw-rw-rw-   0        0        0    10226 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html
+-rw-rw-rw-   0        0        0    10337 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_express_placed.html
+-rw-rw-rw-   0        0        0    57366 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_order_placed.html
+-rw-rw-rw-   0        0        0    57419 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_order_placed2.html
+-rw-rw-rw-   0        0        0    57320 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves.html
+-rw-rw-rw-   0        0        0    57419 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves2.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:07.849255 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/
+-rw-rw-rw-   0        0        0    27770 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/billing_payment.html
+-rw-rw-rw-   0        0        0     6930 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/charges.html
+-rw-rw-rw-   0        0        0    20151 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/payment_notification.html
+-rw-rw-rw-   0        0        0    20151 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/sale_notification.html
+-rw-rw-rw-   0        0        0     7266 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html
+-rw-rw-rw-   0        0        0     7166 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/withdrawals.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:07.923211 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/support/
+-rw-rw-rw-   0        0        0    20072 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/support/support_notification.html
+-rw-rw-rw-   0        0        0    20096 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/support/support_response.html
+-rw-rw-rw-   0        0        0    22210 2024-02-23 18:58:52.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/home.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:07.961187 stela_publishing-0.2.31/stela_control/templates/stela_control/inbox/
+-rw-rw-rw-   0        0        0     7530 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/inbox/index.html
+-rw-rw-rw-   0        0        0     8900 2024-02-10 15:38:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.038274 stela_publishing-0.2.31/stela_control/templates/stela_control/inventory/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:08.229023 stela_publishing-0.2.31/stela_control/templates/stela_control/inventory/journals/
+-rw-rw-rw-   0        0        0     6289 2024-02-08 17:58:31.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/inventory/journals/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:08.693322 stela_publishing-0.2.31/stela_control/templates/stela_control/inventory/publishing/
+-rw-rw-rw-   0        0        0     6897 2024-02-26 22:43:48.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/inventory/publishing/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.271966 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.324932 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/aboutemmerut/
+-rw-rw-rw-   0        0        0     1694 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.354913 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/aboutsecondary/
+-rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.386893 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/aboutstela/
+-rw-rw-rw-   0        0        0     1381 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/aboutstela/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.415877 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/appstela/
+-rw-rw-rw-   0        0        0     1806 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/appstela/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.046270 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/auth/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.492233 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/auth/pw_reset/
+-rw-rw-rw-   0        0        0       45 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/auth/pw_reset/form_errors.html
+-rw-rw-rw-   0        0        0      171 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/auth/pw_reset/password_reset_form.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.521213 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/auth/signup/
+-rw-rw-rw-   0        0        0      794 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html
+-rw-rw-rw-   0        0        0      269 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/auth/signup/success_register.html
+-rw-rw-rw-   0        0        0     3005 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/blog-feed.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.535205 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/categories/
+-rw-rw-rw-   0        0        0      834 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/categories/modal4.html
+-rw-rw-rw-   0        0        0      826 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/chatbox.html
+-rw-rw-rw-   0        0        0      925 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/chatbox2.html
+-rw-rw-rw-   0        0        0      143 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/city_data.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.560190 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/colors/
+-rw-rw-rw-   0        0        0      857 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/colors/modal2.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.584175 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/contact/
+-rw-rw-rw-   0        0        0     1606 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/contact/modal.html
+-rw-rw-rw-   0        0        0     1638 2024-01-22 20:05:28.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/dynamic-formset.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.609161 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/emmerutfooter/
+-rw-rw-rw-   0        0        0     2233 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.685112 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/emmerutservices/
+-rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html
+-rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html
+-rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html
+-rw-rw-rw-   0        0        0      841 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/form-base.html
+-rw-rw-rw-   0        0        0       64 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/form-errors.html
+-rw-rw-rw-   0        0        0       45 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/form.html
+-rw-rw-rw-   0        0        0      924 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/formset-base-services.html
+-rw-rw-rw-   0        0        0     1790 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/formset-base.html
+-rw-rw-rw-   0        0        0      816 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/formset.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.052266 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/handlers/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.783053 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/handlers/blog/
+-rw-rw-rw-   0        0        0     1488 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages.html
+-rw-rw-rw-   0        0        0      128 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/handlers/blog/empty-blog.html
+-rw-rw-rw-   0        0        0      265 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/handlers/blog/empy-blog.html
+-rw-rw-rw-   0        0        0      103 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/hashtags.html
+-rw-rw-rw-   0        0        0      587 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/instagram-alert.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.926966 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/inventory/
+-rw-rw-rw-   0        0        0     2029 2024-02-27 00:20:27.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html
+-rw-rw-rw-   0        0        0      777 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/inventory/simple-form.html
+-rw-rw-rw-   0        0        0     1578 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/inventory/simple-formset.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.944954 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/job-application/
+-rw-rw-rw-   0        0        0       45 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/job-application/error-form-v1.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:09.958944 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/linkzoneupdates/
+-rw-rw-rw-   0        0        0      848 2024-01-15 04:03:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.059263 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:10.319723 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/
+-rw-rw-rw-   0        0        0     1067 2024-02-23 15:58:42.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html
+-rw-rw-rw-   0        0        0     1467 2024-02-23 16:29:50.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html
+-rw-rw-rw-   0        0        0     1650 2024-02-23 18:05:44.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     2732 2024-02-23 18:06:01.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     2477 2024-02-23 18:05:57.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:06.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:10.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     2887 2024-02-23 18:06:18.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2593 2024-02-23 18:06:24.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2296 2024-02-23 18:06:30.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1639 2024-02-23 18:06:35.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2803 2024-02-23 18:06:42.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:10.518247 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/
+-rw-rw-rw-   0        0        0     1614 2024-02-23 18:04:43.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     3292 2024-02-23 18:04:45.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     3051 2024-02-23 18:04:50.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1936 2024-02-23 18:04:55.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     2198 2024-02-23 18:05:01.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     2866 2024-02-23 18:05:07.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2971 2024-05-02 18:22:00.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2418 2024-02-23 18:05:17.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1412 2024-02-23 18:07:47.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2803 2024-02-23 18:05:27.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html
+-rw-rw-rw-   0        0        0     1297 2024-02-23 15:56:06.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html
+-rw-rw-rw-   0        0        0     1778 2024-02-23 16:29:34.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:10.950979 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/
+-rw-rw-rw-   0        0        0     1069 2024-02-23 15:58:34.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html
+-rw-rw-rw-   0        0        0     1464 2024-02-23 16:29:44.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html
+-rw-rw-rw-   0        0        0     1962 2024-02-23 18:06:50.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     3022 2024-02-23 18:06:54.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     2815 2024-02-23 18:07:00.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1740 2024-02-23 18:07:07.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     2080 2024-02-23 18:07:11.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     3148 2024-02-23 18:07:16.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2631 2024-02-23 18:07:22.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2489 2024-02-23 18:07:28.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1929 2024-02-23 18:07:33.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2803 2024-02-23 18:07:38.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.050917 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.068908 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/community/
+-rw-rw-rw-   0        0        0      818 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/community/formdata.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.084897 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/content-pro-media/
+-rw-rw-rw-   0        0        0     3209 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.126872 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/content-pro-update/
+-rw-rw-rw-   0        0        0       83 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/content-pro-update/content.html
+-rw-rw-rw-   0        0        0       84 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/content-pro-update/schedule.html
+-rw-rw-rw-   0        0        0      986 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.155855 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ic-update/
+-rw-rw-rw-   0        0        0      469 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ic-update/content.html
+-rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.292770 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/
+-rw-rw-rw-   0        0        0    25077 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html
+-rw-rw-rw-   0        0        0     1667 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html
+-rw-rw-rw-   0        0        0     1530 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html
+-rw-rw-rw-   0        0        0     1849 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html
+-rw-rw-rw-   0        0        0     1774 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html
+-rw-rw-rw-   0        0        0     4485 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html
+-rw-rw-rw-   0        0        0     5787 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.317754 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/meta-assets/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page-alert.html
+-rw-rw-rw-   0        0        0      628 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.387712 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/page-analythics/
+-rw-rw-rw-   0        0        0     1755 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html
+-rw-rw-rw-   0        0        0     1960 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html
+-rw-rw-rw-   0        0        0     1428 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.408697 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/smart-boost/
+-rw-rw-rw-   0        0        0     2129 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.427686 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/stela-sight/
+-rw-rw-rw-   0        0        0      268 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/stela-sight/data.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.460214 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/newcomer/
+-rw-rw-rw-   0        0        0     3796 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/newcomer/form.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.540169 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/post/
+-rw-rw-rw-   0        0        0      846 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/post/list-modal.html
+-rw-rw-rw-   0        0        0      850 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/post/main-modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.624117 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/
+-rw-rw-rw-   0        0        0     1824 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/catalog-modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:11.836987 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/
+-rw-rw-rw-   0        0        0      933 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/catalog-form.html
+-rw-rw-rw-   0        0        0      872 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/category-form.html
+-rw-rw-rw-   0        0        0      888 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/color-form.html
+-rw-rw-rw-   0        0        0     1024 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/product-form.html
+-rw-rw-rw-   0        0        0      855 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/size-form.html
+-rw-rw-rw-   0        0        0      115 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/variant-form.html
+-rw-rw-rw-   0        0        0      805 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/product-modal.html
+-rw-rw-rw-   0        0        0      848 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/size-modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.069845 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/update/
+-rw-rw-rw-   0        0        0      234 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/update/catalog-form.html
+-rw-rw-rw-   0        0        0      287 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/update/category-form.html
+-rw-rw-rw-   0        0        0      230 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/update/color-form.html
+-rw-rw-rw-   0        0        0     1008 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/update/product-form.html
+-rw-rw-rw-   0        0        0      228 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/update/size-form.html
+-rw-rw-rw-   0        0        0      234 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/update/variant-form.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.113816 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/profile/
+-rw-rw-rw-   0        0        0     1306 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/profile/dynamic-form.html
+-rw-rw-rw-   0        0        0      200 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/profile/single-form.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.136803 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/projects/
+-rw-rw-rw-   0        0        0     1698 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/projects/modal.html
+-rw-rw-rw-   0        0        0      260 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/remove-complete.html
+-rw-rw-rw-   0        0        0      212 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/single-form.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.080248 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.192768 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/
+-rw-rw-rw-   0        0        0     1099 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.245734 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/error_forms/
+-rw-rw-rw-   0        0        0     1099 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.327685 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/forms/
+-rw-rw-rw-   0        0        0     1269 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html
+-rw-rw-rw-   0        0        0     1097 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.387648 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/update_forms/
+-rw-rw-rw-   0        0        0     1156 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1320 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.435619 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/staff/
+-rw-rw-rw-   0        0        0     1947 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/staff/form.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.505164 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stela_story/
+-rw-rw-rw-   0        0        0     3404 2024-02-21 12:50:07.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stela_story/feed-item.html
+-rw-rw-rw-   0        0        0     2001 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.531147 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stelafooter/
+-rw-rw-rw-   0        0        0     2176 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stelafooter/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.566125 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stelamedia/
+-rw-rw-rw-   0        0        0     1695 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stelamedia/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.591110 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stelapath/
+-rw-rw-rw-   0        0        0     1337 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stelapath/modal.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.609098 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/youtube/
+-rw-rw-rw-   0        0        0      157 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/youtube/video-preview.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.088245 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:12.717032 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/email-marketing/
+-rw-rw-rw-   0        0        0     2345 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/email-marketing/email_list.html
+-rw-rw-rw-   0        0        0     1774 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/email-marketing/emails_list.html
+-rw-rw-rw-   0        0        0     1917 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/email-marketing/new_email.html
+-rw-rw-rw-   0        0        0      976 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/email-marketing/update_email.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:13.186284 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/
+-rw-rw-rw-   0        0        0    10789 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:04.092243 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/instagram/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:13.863458 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/
+-rw-rw-rw-   0        0        0    13445 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:13.921422 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/
+-rw-rw-rw-   0        0        0    23333 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:13.981386 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/
+-rw-rw-rw-   0        0        0    34272 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:14.040349 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:14.099313 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/community/
+-rw-rw-rw-   0        0        0    14156 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:14.204247 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/
+-rw-rw-rw-   0        0        0    30243 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html
+-rw-rw-rw-   0        0        0      248 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/update.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:14.244223 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/
+-rw-rw-rw-   0        0        0     3162 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html
+-rw-rw-rw-   0        0        0    12633 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html
+-rw-rw-rw-   0        0        0    17640 2024-02-12 17:40:18.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/newcomer.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:14.348160 stela_publishing-0.2.31/stela_control/templates/stela_control/orders/
+-rw-rw-rw-   0        0        0     6171 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/orders/list_view.html
+-rw-rw-rw-   0        0        0     8860 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/orders/order_update.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:14.578618 stela_publishing-0.2.31/stela_control/templates/stela_control/payments/
+-rw-rw-rw-   0        0        0    43167 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/payments/homebrew.html
+-rw-rw-rw-   0        0        0     2687 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/payments/register-wallet.html
+-rw-rw-rw-   0        0        0     4322 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/payments/wallet-list.html
+-rw-rw-rw-   0        0        0     2831 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/payments/withdraw.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:14.597605 stela_publishing-0.2.31/stela_control/templates/stela_control/prostela/
+-rw-rw-rw-   0        0        0      153 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/prostela/chatbox.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:14.681553 stela_publishing-0.2.31/stela_control/templates/stela_control/prostela-expert/
+-rw-rw-rw-   0        0        0    34014 2024-01-15 04:03:12.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/prostela-expert/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:14.757507 stela_publishing-0.2.31/stela_control/templates/stela_control/reviews/
+-rw-rw-rw-   0        0        0     3170 2024-01-15 04:03:13.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/reviews/reviews_list.html
+-rw-rw-rw-   0        0        0     1325 2024-01-15 04:03:13.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/reviews/update_review.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:14.827463 stela_publishing-0.2.31/stela_control/templates/stela_control/support/
+-rw-rw-rw-   0        0        0     2061 2024-01-15 04:03:13.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/support/list.html
+-rw-rw-rw-   0        0        0     7093 2024-01-15 04:03:13.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/support/update.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:15.398114 stela_publishing-0.2.31/stela_control/templates/stela_control/users/
+-rw-rw-rw-   0        0        0      339 2024-01-18 10:28:40.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/users/generic-user-handler.html
+-rw-rw-rw-   0        0        0    11181 2024-01-22 21:22:30.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/users/profile.html
+-rw-rw-rw-   0        0        0    12343 2024-02-06 16:52:33.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/users/users-control.html
+-rw-rw-rw-   0        0        0     6472 2024-02-06 15:00:39.000000 stela_publishing-0.2.31/stela_control/templates/stela_control/users/users.html
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:15.414102 stela_publishing-0.2.31/stela_control/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:13.000000 stela_publishing-0.2.31/stela_control/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1277 2024-01-19 05:09:17.000000 stela_publishing-0.2.31/stela_control/templatetags/stelatags.py
+-rw-rw-rw-   0        0        0      507 2024-01-15 04:03:13.000000 stela_publishing-0.2.31/stela_control/tests.py
+-rw-rw-rw-   0        0        0     1131 2024-01-15 04:03:13.000000 stela_publishing-0.2.31/stela_control/tokenize.py
+-rw-rw-rw-   0        0        0     5281 2024-02-20 00:45:02.000000 stela_publishing-0.2.31/stela_control/urls.py
+-rw-rw-rw-   0        0        0   211317 2024-02-20 00:48:27.000000 stela_publishing-0.2.31/stela_control/views.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:23:15.437088 stela_publishing-0.2.31/stela_publishing.egg-info/
+-rw-rw-rw-   0        0        0     3241 2024-05-02 18:23:02.000000 stela_publishing-0.2.31/stela_publishing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    20966 2024-05-02 18:23:03.000000 stela_publishing-0.2.31/stela_publishing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 18:23:02.000000 stela_publishing-0.2.31/stela_publishing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      355 2024-05-02 18:23:02.000000 stela_publishing-0.2.31/stela_publishing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2024-05-02 18:23:02.000000 stela_publishing-0.2.31/stela_publishing.egg-info/top_level.txt
```

### Comparing `stela_publishing-0.2.30/LICENSE` & `stela_publishing-0.2.31/LICENSE`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/PKG-INFO` & `stela_publishing-0.2.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stela_publishing
-Version: 0.2.30
+Version: 0.2.31
 Summary: All apps in one for business.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `stela_publishing-0.2.30/README.md` & `stela_publishing-0.2.31/README.md`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/accounts/migrations/0001_initial.py` & `stela_publishing-0.2.31/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/accounts/models.py` & `stela_publishing-0.2.31/accounts/models.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/accounts/urls.py` & `stela_publishing-0.2.31/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/accounts/views.py` & `stela_publishing-0.2.31/accounts/views.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/cloud/cart.py` & `stela_publishing-0.2.31/cloud/cart.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/cloud/migrations/0001_initial.py` & `stela_publishing-0.2.31/cloud/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/cloud/models.py` & `stela_publishing-0.2.31/cloud/models.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/geolocation/migrations/0001_initial.py` & `stela_publishing-0.2.31/geolocation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/geolocation/models.py` & `stela_publishing-0.2.31/geolocation/models.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/setup.py` & `stela_publishing-0.2.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 excluded_packages = [
     'core', 'core.*', 
     'linkzone', 'linkzone.*', 
 ]
 setup(
     name='stela_publishing',
-    version='0.2.30',
+    version='0.2.31',
     packages=find_packages(exclude=excluded_packages),
     include_package_data=True,
     license='MIT',
     description='All apps in one for business.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

### Comparing `stela_publishing-0.2.30/stela_control/cart.py` & `stela_publishing-0.2.31/stela_control/cart.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/forms.py` & `stela_publishing-0.2.31/stela_control/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1231,15 +1231,15 @@
 
         return subtitle
 
 class SimpleContentForm(forms.ModelForm):
 
     class Meta:
         model = Content
-        fields = ['status','title','subtitle','media',]
+        fields = ['category','status','title','subtitle','media',]
         
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
     
         for field in self.fields.values():
             field.widget.attrs['placeholder'] = field.label
             field.label = False
```

### Comparing `stela_publishing-0.2.30/stela_control/locale/es/LC_MESSAGES/django.mo` & `stela_publishing-0.2.31/stela_control/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/locale/es/LC_MESSAGES/django.po` & `stela_publishing-0.2.31/stela_control/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0001_initial.py` & `stela_publishing-0.2.31/stela_control/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0002_rename_response_chatsupport_content_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0002_rename_response_chatsupport_content_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0003_rename_logo_company_alter_logo_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0003_rename_logo_company_alter_logo_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0004_content_video_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0004_content_video_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0005_rename_description_team_content_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0005_rename_description_team_content_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0006_content_cover_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0006_content_cover_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0007_content_fecade_url_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0007_content_fecade_url_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0009_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0009_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0010_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0010_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0011_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0011_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0013_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0013_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0016_remove_sociallinks_url_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0016_remove_sociallinks_url_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0017_sociallinks_social_url_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0017_sociallinks_social_url_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0018_inventory_condition_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0018_inventory_condition_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0019_inventory_amazon_published_date_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0019_inventory_amazon_published_date_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0020_remove_inventory_amazon_published_date_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0020_remove_inventory_amazon_published_date_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/migrations/0021_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.31/stela_control/migrations/0021_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/models.py` & `stela_publishing-0.2.31/stela_control/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -785,14 +785,16 @@
     }
     CATEGORY = {
         (_('News'),_('News')),
         (_('Reviews'),_('Reviews')),
         (_('Events'),_('Events')),
         (_('Stories'),_('Stories')),
         (_('Honors'),_('Honors')),
+        (_('Family Tree'),_('Family Tree')),
+        
     }
     category = models.CharField(max_length=100, choices=CATEGORY, blank=True, default=_('News'))
     card = models.CharField(max_length=50, null=True, choices=CARD_OPTION, verbose_name=_('Color Card'), blank=True)
     about = models.CharField(max_length=60, choices=ABOUT, verbose_name=_('Title'), null=True, blank=True, default='Mission')
     author = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, related_name="author", null=True)
     section = models.CharField(max_length=200, verbose_name=_('Section'), default="No section")
     path = models.CharField(max_length=60, choices=CHOICESPATH, verbose_name=_('Path Title'), null=True)
```

### Comparing `stela_publishing-0.2.30/stela_control/routers.py` & `stela_publishing-0.2.31/stela_control/routers.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/superfunctions.py` & `stela_publishing-0.2.31/stela_control/superfunctions.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/registration/confirmation_email.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/registration/confirmation_email.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/registration/register.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/registration/register.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/delete_user.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/delete_user.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/login.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/login.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/password_reset_done.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/password_reset_email.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/accounts/user/password_reset_form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/accounts/user/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/analytics/analytics.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/analytics/analytics.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/analytics/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/analytics/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/api/main.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/api/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/base.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/base.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/base_content.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/base_content.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/base_list.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/base_list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/billing/homebrew.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/billing/homebrew.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/bill-data-customer.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/bill-data-customer.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/checkout.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/checkout.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/data-customer.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/data-customer.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/invoice-copy.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/invoice-copy.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/invoice.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/invoice.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/order-placed.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/order-placed.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/preview-recipt.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/preview-recipt.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/billing/sections/recipt-detail.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/billing/sections/recipt-detail.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/chatstela/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/chatstela/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/content/comments/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/content/comments/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/content/docs/main.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/content/docs/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/content/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/content/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/content/main/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/content/main/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/content/staff/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/content/staff/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/content/stelastory.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/content/stelastory.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/developer/data-update/modal1.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/developer/data-update/modal1.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/developer/data-update/modal2.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/developer/data-update/modal2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/developer/data-update/modal3.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/developer/data-update/modal3.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/developer/data-update/modal4.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/developer/data-update/modal4.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/developer/home.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/developer/home.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/billing/invoice.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/billing/invoice.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/contact/message_notification.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/contact/message_notification.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/contact/message_response.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/contact/message_response.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/contact/support_notification.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/contact/support_notification.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/contact/update_support.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/contact/update_support.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/newsletter/success.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/newsletter/success.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_express_placed.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_express_placed.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_order_placed.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_order_placed.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_order_placed2.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_order_placed2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves2.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/billing_payment.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/billing_payment.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/charges.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/charges.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/payment_notification.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/payment_notification.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/sale_notification.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/sale_notification.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/payments/withdrawals.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/payments/withdrawals.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/support/support_notification.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/support/support_notification.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/emails-template/support/support_response.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/emails-template/support/support_response.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/home.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/home.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/inbox/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/inbox/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/inventory/journals/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/inventory/journals/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/inventory/publishing/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/inventory/publishing/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/aboutstela/modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/aboutstela/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/appstela/modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/appstela/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/blog-feed.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/blog-feed.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/categories/modal4.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/categories/modal4.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/chatbox.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/chatbox.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/chatbox2.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/chatbox2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/colors/modal2.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/colors/modal2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/contact/modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/contact/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/dynamic-formset.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/dynamic-formset.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/form-base.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/form-base.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/formset-base-services.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/formset-base-services.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/formset-base.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/formset-base.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/formset.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/formset.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/instagram-alert.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/instagram-alert.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/inventory/simple-form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/inventory/simple-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/inventory/simple-formset.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/inventory/simple-formset.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,60 +4,54 @@
     <div id="formset">
         {{ formset.management_form }}
         {% for form in formset %}
         <div id="form-0" class="formset pt-2">
             <div class="row">
                 <div class="col-12">
                     <div class="input-group mb-3">
-                        <div class="input-group-prepend">
-                            <span class="input-group-text">{% trans "Slider Image" %}</span>
-                        </div>
-                        <div class="custom-file {% if form.image.errors %}has-danger{% endif %}">
-                            {{form.media}}
-                        </div>
+                      <div class="input-group-prepend">
+                        <span class="input-group-text">{% trans "App Image" %}</span>
+                      </div>
+                      <div class="custom-file">
+                          {{form.media}}
+                      </div>
                     </div>
                 </div>
                 <div class="col-12">
                     {{form.status|as_crispy_field}}
                 </div>
                 <div class="col-12">
-                    {{form.title|as_crispy_field}}
-                </div>
-                <div class="col-12">
-                    {{form.subtitle|as_crispy_field}}
+                    {{form.url|as_crispy_field}}
                 </div>
             </div>
         </div>
         {% endfor %}
         <div id="empty-form" class="d-none">
             <div class="row">
                 <div class="col-12">
                     <div class="input-group mb-3">
                         <div class="input-group-prepend">
-                            <span class="input-group-text">{% trans "Slider Image" %}</span>
+                            <span class="input-group-text">{% trans "App Image" %}</span>
                         </div>
                         <div class="custom-file">
                             {{formset.empty_form.media}}
                         </div>
                     </div>
                 </div>
                 <div class="col-12">
                     {{formset.empty_form.status|as_crispy_field}}
                 </div>
                 <div class="col-12">
-                    {{formset.empty_form.title|as_crispy_field}}
-                </div>
-                <div class="col-12">
-                    {{formset.empty_form.subtitle|as_crispy_field}}
+                    {{formset.empty_form.url|as_crispy_field}}
                 </div>
             </div>
         </div>
     </div>
     <div class="d-flex justify-content-between my-3">
         <button class="btn-clear" onclick="addFormset()" type="button"><i class="fa-solid fa-plus"></i> {% trans "Add" %}</button>
         <button class="btn-clear remove-formset" onclick="clearFormset()" type="button"><i class="fa-solid fa-minus"></i> {% trans "Remove" %}</button>
     </div> 
 </div>
 <p class="response-footer text-link fw-bold oxanium"></p>
 <input type="hidden" name="form-id" value={{form_name}}>
-<input type="hidden" name="section" value={{section}}>
+<input type="hidden" name="section" value={{section}}> 
 <input type="hidden" name="form-url" value="/validations/content/">
```

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html`

 * *Files 10% similar despite different names*

```diff
@@ -4,54 +4,66 @@
     <div id="formset">
         {{ formset.management_form }}
         {% for form in formset %}
         <div id="form-0" class="formset pt-2">
             <div class="row">
                 <div class="col-12">
                     <div class="input-group mb-3">
-                      <div class="input-group-prepend">
-                        <span class="input-group-text">{% trans "App Image" %}</span>
-                      </div>
-                      <div class="custom-file">
-                          {{form.media}}
-                      </div>
+                        <div class="input-group-prepend">
+                            <span class="input-group-text">{% trans "Slider Image" %}</span>
+                        </div>
+                        <div class="custom-file {% if form.image.errors %}has-danger{% endif %}">
+                            {{form.media}}
+                        </div>
                     </div>
                 </div>
                 <div class="col-12">
                     {{form.status|as_crispy_field}}
                 </div>
                 <div class="col-12">
-                    {{form.url|as_crispy_field}}
+                    {{form.category|as_crispy_field}}
+                </div>
+                <div class="col-12">
+                    {{form.title|as_crispy_field}}
+                </div>
+                <div class="col-12">
+                    {{form.subtitle|as_crispy_field}}
                 </div>
             </div>
         </div>
         {% endfor %}
         <div id="empty-form" class="d-none">
             <div class="row">
                 <div class="col-12">
                     <div class="input-group mb-3">
                         <div class="input-group-prepend">
-                            <span class="input-group-text">{% trans "App Image" %}</span>
+                            <span class="input-group-text">{% trans "Slider Image" %}</span>
                         </div>
                         <div class="custom-file">
                             {{formset.empty_form.media}}
                         </div>
                     </div>
                 </div>
                 <div class="col-12">
                     {{formset.empty_form.status|as_crispy_field}}
                 </div>
                 <div class="col-12">
-                    {{formset.empty_form.url|as_crispy_field}}
+                    {{form.category|as_crispy_field}}
+                </div>
+                <div class="col-12">
+                    {{formset.empty_form.title|as_crispy_field}}
+                </div>
+                <div class="col-12">
+                    {{formset.empty_form.subtitle|as_crispy_field}}
                 </div>
             </div>
         </div>
     </div>
     <div class="d-flex justify-content-between my-3">
         <button class="btn-clear" onclick="addFormset()" type="button"><i class="fa-solid fa-plus"></i> {% trans "Add" %}</button>
         <button class="btn-clear remove-formset" onclick="clearFormset()" type="button"><i class="fa-solid fa-minus"></i> {% trans "Remove" %}</button>
     </div> 
 </div>
 <p class="response-footer text-link fw-bold oxanium"></p>
 <input type="hidden" name="form-id" value={{form_name}}>
-<input type="hidden" name="section" value={{section}}> 
+<input type="hidden" name="section" value={{section}}>
 <input type="hidden" name="form-url" value="/validations/content/">
```

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/community/formdata.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/community/formdata.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/newcomer/form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/newcomer/form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/post/list-modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/post/list-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/post/main-modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/post/main-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/catalog-modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/catalog-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/catalog-form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/catalog-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/category-form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/category-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/color-form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/color-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/product-form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/product-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/new/size-form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/new/size-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/product-modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/product-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/size-modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/size-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/products/update/product-form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/products/update/product-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/profile/dynamic-form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/profile/dynamic-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/projects/modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/projects/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/staff/form.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/staff/form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stela_story/feed-item.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stela_story/feed-item.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stelafooter/modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stelafooter/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stelamedia/modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stelamedia/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/load-data/stelapath/modal.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/load-data/stelapath/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/email-marketing/email_list.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/email-marketing/email_list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/email-marketing/emails_list.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/email-marketing/emails_list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/email-marketing/new_email.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/email-marketing/new_email.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/email-marketing/update_email.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/email-marketing/update_email.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/newcomer.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/newcomer.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/orders/list_view.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/orders/list_view.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/orders/order_update.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/orders/order_update.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/payments/homebrew.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/payments/homebrew.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/payments/register-wallet.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/payments/register-wallet.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/payments/wallet-list.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/payments/wallet-list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/payments/withdraw.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/payments/withdraw.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/prostela-expert/index.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/prostela-expert/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/reviews/reviews_list.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/reviews/reviews_list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/reviews/update_review.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/reviews/update_review.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/support/list.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/support/list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/support/update.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/support/update.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/users/profile.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/users/profile.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/users/users-control.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/users/users-control.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templates/stela_control/users/users.html` & `stela_publishing-0.2.31/stela_control/templates/stela_control/users/users.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/templatetags/stelatags.py` & `stela_publishing-0.2.31/stela_control/templatetags/stelatags.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/tokenize.py` & `stela_publishing-0.2.31/stela_control/tokenize.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/urls.py` & `stela_publishing-0.2.31/stela_control/urls.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_control/views.py` & `stela_publishing-0.2.31/stela_control/views.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.30/stela_publishing.egg-info/PKG-INFO` & `stela_publishing-0.2.31/stela_publishing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stela_publishing
-Version: 0.2.30
+Version: 0.2.31
 Summary: All apps in one for business.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `stela_publishing-0.2.30/stela_publishing.egg-info/SOURCES.txt` & `stela_publishing-0.2.31/stela_publishing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

