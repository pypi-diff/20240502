# Comparing `tmp/magplan-3.3.1.tar.gz` & `tmp/magplan-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magplan-3.3.1.tar", max compression
+gzip compressed data, was "magplan-3.3.2.tar", max compression
```

## Comparing `magplan-3.3.1.tar` & `magplan-3.3.2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     6010 2023-12-13 19:44:22.000000 magplan-3.3.1/README.md
--rw-r--r--   0        0        0      807 2024-05-01 06:38:38.793659 magplan-3.3.1/pyproject.toml
--rw-r--r--   0        0        0       47 2024-05-01 06:06:18.172458 magplan-3.3.1/src/magplan/__init__.py
--rw-r--r--   0        0        0     2277 2024-05-01 06:14:12.298346 magplan-3.3.1/src/magplan/admin.py
--rw-r--r--   0        0        0      401 2024-05-01 06:14:08.015571 magplan-3.3.1/src/magplan/apps.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/conf/__init__.py
--rw-r--r--   0        0        0     1627 2024-05-01 06:17:13.407396 magplan-3.3.1/src/magplan/conf/settings.py
--rw-r--r--   0        0        0      556 2024-04-15 10:08:49.770398 magplan-3.3.1/src/magplan/context_processors.py
--rw-r--r--   0        0        0     2862 2024-05-01 06:14:08.095870 magplan-3.3.1/src/magplan/dynamic_preferences_registry.py
--rw-r--r--   0        0        0  3415905 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/fixtures/db_test.json
--rw-r--r--   0        0        0    10989 2024-05-01 06:14:08.419960 magplan-3.3.1/src/magplan/forms.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/integrations/__init__.py
--rw-r--r--   0        0        0      732 2024-04-15 10:08:49.769775 magplan-3.3.1/src/magplan/integrations/images.py
--rw-r--r--   0        0        0     4936 2024-05-01 06:14:08.129489 magplan-3.3.1/src/magplan/integrations/posts.py
--rw-r--r--   0        0        0     1823 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39873 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2456 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40385 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/management/commands/__init__.py
--rw-r--r--   0        0        0      352 2024-05-01 06:06:17.521795 magplan-3.3.1/src/magplan/management/commands/render.py
--rw-r--r--   0        0        0      748 2024-05-01 06:14:08.058580 magplan-3.3.1/src/magplan/middleware.py
--rw-r--r--   0        0        0    17534 2024-05-01 06:14:08.624734 magplan-3.3.1/src/magplan/migrations/0001_initial.py
--rw-r--r--   0        0        0    10857 2024-05-01 06:14:08.530027 magplan-3.3.1/src/magplan/migrations/0002_auto_20201115_1140.py
--rw-r--r--   0        0        0      541 2024-04-15 10:08:49.809744 magplan-3.3.1/src/magplan/migrations/0003_auto_20201121_1750.py
--rw-r--r--   0        0        0      611 2024-04-15 10:08:49.820296 magplan-3.3.1/src/magplan/migrations/0004_post_features.py
--rw-r--r--   0        0        0     1424 2024-04-15 10:12:07.568938 magplan-3.3.1/src/magplan/migrations/0005_auto_20210213_1556.py
--rw-r--r--   0        0        0     1005 2024-05-01 06:06:17.394818 magplan-3.3.1/src/magplan/migrations/0006_auto_20210316_1840.py
--rw-r--r--   0        0        0      620 2024-05-01 06:06:17.361434 magplan-3.3.1/src/magplan/migrations/0007_auto_20210316_1900.py
--rw-r--r--   0        0        0     1652 2024-05-01 06:06:17.358361 magplan-3.3.1/src/magplan/migrations/0008_auto_20210318_0108.py
--rw-r--r--   0        0        0      610 2024-04-15 10:12:07.588161 magplan-3.3.1/src/magplan/migrations/0009_auto_20210523_1641.py
--rw-r--r--   0        0        0     2847 2024-05-01 06:06:17.371144 magplan-3.3.1/src/magplan/migrations/0010_auto_20210624_1041.py
--rw-r--r--   0        0        0     1274 2024-04-15 10:12:07.610111 magplan-3.3.1/src/magplan/migrations/0011_auto_20210624_1817.py
--rw-r--r--   0        0        0      984 2024-05-01 06:06:18.388900 magplan-3.3.1/src/magplan/migrations/0012_alter_attachment_meta_alter_comment_meta_and_more.py
--rw-r--r--   0        0        0     1818 2024-05-01 06:14:08.213881 magplan-3.3.1/src/magplan/migrations/0013_sitepreferencemodel.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/migrations/__init__.py
--rw-r--r--   0        0        0    28566 2024-05-01 06:14:12.851359 magplan-3.3.1/src/magplan/models.py
--rw-r--r--   0        0        0      200 2024-05-01 06:06:18.391401 magplan-3.3.1/src/magplan/registries.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/tasks/__init__.py
--rw-r--r--   0        0        0     3873 2024-05-01 06:14:12.297514 magplan-3.3.1/src/magplan/tasks/send_idea_comment_notification.py
--rw-r--r--   0        0        0      468 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/tasks/send_idea_notification.py
--rw-r--r--   0        0        0     4260 2024-05-01 06:14:12.298004 magplan-3.3.1/src/magplan/tasks/send_post_comment_notification.py
--rw-r--r--   0        0        0      542 2024-05-01 06:06:17.480250 magplan-3.3.1/src/magplan/tasks/upload_post_to_wp.py
--rw-r--r--   0        0        0     1790 2024-05-01 06:14:08.227137 magplan-3.3.1/src/magplan/tasks/utils.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-01 06:14:12.276731 magplan-3.3.1/src/magplan/templates/_test_issues.py
--rw-r--r--   0        0        0      758 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/email/_vote_from_email.html
--rw-r--r--   0        0        0      416 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/email/assigned_to_you.html
--rw-r--r--   0        0        0      701 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/email/idea_approved.html
--rw-r--r--   0        0        0      634 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/email/new_comment.html
--rw-r--r--   0        0        0      370 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/email/new_idea.html
--rw-r--r--   0        0        0     8503 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/layout_plan.html
--rw-r--r--   0        0        0      893 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/articles/advert.html
--rw-r--r--   0        0        0      860 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/articles/archived.html
--rw-r--r--   0        0        0      855 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/articles/default.html
--rw-r--r--   0        0        0     3053 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/articles/index.html
--rw-r--r--   0        0        0      911 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/articles/whitelisted.html
--rw-r--r--   0        0        0     4121 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/authors/_form.html
--rw-r--r--   0        0        0      541 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/authors/edit.html
--rw-r--r--   0        0        0      869 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/authors/index.html
--rw-r--r--   0        0        0      480 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/authors/new.html
--rw-r--r--   0        0        0     1077 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/authors/show.html
--rw-r--r--   0        0        0      595 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/ideas/_approve_ideas.html
--rw-r--r--   0        0        0      786 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/ideas/_authors_list.html
--rw-r--r--   0        0        0     2332 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/ideas/_form_base.html
--rw-r--r--   0        0        0     1088 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/ideas/_vote.html
--rw-r--r--   0        0        0     1521 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/ideas/_voting_results.html
--rw-r--r--   0        0        0     3959 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/ideas/index.html
--rw-r--r--   0        0        0     3149 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/ideas/show.html
--rw-r--r--   0        0        0     4404 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/index/index.html
--rw-r--r--   0        0        0     1786 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/issues/_form.html
--rw-r--r--   0        0        0     1202 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/issues/index.html
--rw-r--r--   0        0        0      477 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/issues/new.html
--rw-r--r--   0        0        0      837 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/issues/show.html
--rw-r--r--   0        0        0      573 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/partials/_navbar.sites.html
--rw-r--r--   0        0        0     1395 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/partials/_navbar_header_links.html
--rw-r--r--   0        0        0     2797 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/partials/comments.html
--rw-r--r--   0        0        0     2252 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/partials/navbar.html
--rw-r--r--   0        0        0     3180 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/partials/posts_table.html
--rw-r--r--   0        0        0      956 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/_admin_set_stage.html
--rw-r--r--   0        0        0     6970 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/_attachments.html
--rw-r--r--   0        0        0      768 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/_field_col.html
--rw-r--r--   0        0        0     3389 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/_form_base.html
--rw-r--r--   0        0        0     3359 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/_form_meta.html
--rw-r--r--   0        0        0      286 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/_paywall_alert.html
--rw-r--r--   0        0        0     1063 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/_progress.html
--rw-r--r--   0        0        0      882 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/_schedule.html
--rw-r--r--   0        0        0     2437 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/_stages.html
--rw-r--r--   0        0        0     8559 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/edit.html
--rw-r--r--   0        0        0     9102 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/posts/show.html
--rw-r--r--   0        0        0      345 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/preferences/index.html
--rw-r--r--   0        0        0      804 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/sections/index.html
--rw-r--r--   0        0        0     1607 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templates/magplan/stages/index.html
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/templatetags/__init__.py
--rw-r--r--   0        0        0     6000 2024-05-01 06:06:17.346132 magplan-3.3.1/src/magplan/templatetags/filters.py
--rw-r--r--   0        0        0     2814 2024-05-01 06:14:12.331038 magplan-3.3.1/src/magplan/urls.py
--rw-r--r--   0        0        0     1248 2024-04-15 15:19:59.641866 magplan-3.3.1/src/magplan/utils.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/views/__init__.py
--rw-r--r--   0        0        0      898 2024-04-15 10:12:07.737198 magplan-3.3.1/src/magplan/views/api.py
--rw-r--r--   0        0        0     6338 2024-05-01 06:38:18.611005 magplan-3.3.1/src/magplan/views/articles.py
--rw-r--r--   0        0        0     3041 2024-05-01 06:14:08.519369 magplan-3.3.1/src/magplan/views/authors.py
--rw-r--r--   0        0        0     7950 2024-05-01 06:14:12.432610 magplan-3.3.1/src/magplan/views/ideas.py
--rw-r--r--   0        0        0     3321 2024-05-01 06:14:08.537681 magplan-3.3.1/src/magplan/views/index.py
--rw-r--r--   0        0        0     1859 2024-05-01 06:14:08.558308 magplan-3.3.1/src/magplan/views/issues.py
--rw-r--r--   0        0        0    16990 2024-05-01 06:14:12.645881 magplan-3.3.1/src/magplan/views/posts.py
--rw-r--r--   0        0        0     1134 2024-05-01 06:14:08.564285 magplan-3.3.1/src/magplan/views/preferences.py
--rw-r--r--   0        0        0      337 2024-05-01 06:06:17.714358 magplan-3.3.1/src/magplan/views/sections.py
--rw-r--r--   0        0        0      474 2024-05-01 06:06:17.782732 magplan-3.3.1/src/magplan/views/stages.py
--rw-r--r--   0        0        0      390 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/xmd/README.md
--rw-r--r--   0        0        0       27 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/xmd/__init__.py
--rw-r--r--   0        0        0     2909 2024-05-01 06:14:08.651159 magplan-3.3.1/src/magplan/xmd/lexers.py
--rw-r--r--   0        0        0      874 2024-04-15 10:08:50.159967 magplan-3.3.1/src/magplan/xmd/mappers.py
--rw-r--r--   0        0        0     1397 2024-04-15 10:08:50.169892 magplan-3.3.1/src/magplan/xmd/markdown.py
--rw-r--r--   0        0        0     2561 2024-05-01 06:14:08.666180 magplan-3.3.1/src/magplan/xmd/renderer.py
--rw-r--r--   0        0        0      313 2024-04-15 10:08:50.175035 magplan-3.3.1/src/magplan/xmd/templates.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.1/src/magplan/xmd/tests/__init__.py
--rw-r--r--   0        0        0       72 2024-05-01 06:06:17.586779 magplan-3.3.1/src/magplan/xmd/tests/conftest.py
--rw-r--r--   0        0        0     5168 2024-05-01 06:14:08.736635 magplan-3.3.1/src/magplan/xmd/tests/test_lexer.py
--rw-r--r--   0        0        0     1526 2024-05-01 06:14:08.660016 magplan-3.3.1/src/magplan/xmd/tests/test_renderer.py
--rw-r--r--   0        0        0     1274 2024-05-01 06:06:18.926242 magplan-3.3.1/src/magplan/xmd/tests/test_utils.py
--rw-r--r--   0        0        0      478 2024-04-15 10:08:50.208773 magplan-3.3.1/src/magplan/xmd/utils.py
--rw-r--r--   0        0        0      957 2024-04-15 10:08:50.224860 magplan-3.3.1/src/magplan/xmd/xmd.py
--rw-r--r--   0        0        0     7220 1970-01-01 00:00:00.000000 magplan-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0     6010 2023-12-13 19:44:22.000000 magplan-3.3.2/README.md
+-rw-r--r--   0        0        0      807 2024-05-02 19:57:44.289446 magplan-3.3.2/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-05-01 06:06:18.172458 magplan-3.3.2/src/magplan/__init__.py
+-rw-r--r--   0        0        0     2277 2024-05-01 06:14:12.298346 magplan-3.3.2/src/magplan/admin.py
+-rw-r--r--   0        0        0      401 2024-05-01 06:14:08.015571 magplan-3.3.2/src/magplan/apps.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/conf/__init__.py
+-rw-r--r--   0        0        0     1627 2024-05-01 19:27:23.660995 magplan-3.3.2/src/magplan/conf/settings.py
+-rw-r--r--   0        0        0      556 2024-04-15 10:08:49.770398 magplan-3.3.2/src/magplan/context_processors.py
+-rw-r--r--   0        0        0     3217 2024-05-02 19:41:22.330615 magplan-3.3.2/src/magplan/dynamic_preferences_registry.py
+-rw-r--r--   0        0        0  3415905 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/fixtures/db_test.json
+-rw-r--r--   0        0        0    10989 2024-05-01 06:14:08.419960 magplan-3.3.2/src/magplan/forms.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/integrations/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-15 10:08:49.769775 magplan-3.3.2/src/magplan/integrations/images.py
+-rw-r--r--   0        0        0     4936 2024-05-01 06:14:08.129489 magplan-3.3.2/src/magplan/integrations/posts.py
+-rw-r--r--   0        0        0     1823 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39873 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2456 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40385 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/management/commands/__init__.py
+-rw-r--r--   0        0        0      352 2024-05-01 06:06:17.521795 magplan-3.3.2/src/magplan/management/commands/render.py
+-rw-r--r--   0        0        0      748 2024-05-01 06:14:08.058580 magplan-3.3.2/src/magplan/middleware.py
+-rw-r--r--   0        0        0    17534 2024-05-01 06:14:08.624734 magplan-3.3.2/src/magplan/migrations/0001_initial.py
+-rw-r--r--   0        0        0    10857 2024-05-01 06:14:08.530027 magplan-3.3.2/src/magplan/migrations/0002_auto_20201115_1140.py
+-rw-r--r--   0        0        0      541 2024-04-15 10:08:49.809744 magplan-3.3.2/src/magplan/migrations/0003_auto_20201121_1750.py
+-rw-r--r--   0        0        0      611 2024-04-15 10:08:49.820296 magplan-3.3.2/src/magplan/migrations/0004_post_features.py
+-rw-r--r--   0        0        0     1424 2024-04-15 10:12:07.568938 magplan-3.3.2/src/magplan/migrations/0005_auto_20210213_1556.py
+-rw-r--r--   0        0        0     1005 2024-05-01 06:06:17.394818 magplan-3.3.2/src/magplan/migrations/0006_auto_20210316_1840.py
+-rw-r--r--   0        0        0      620 2024-05-01 06:06:17.361434 magplan-3.3.2/src/magplan/migrations/0007_auto_20210316_1900.py
+-rw-r--r--   0        0        0     1652 2024-05-01 06:06:17.358361 magplan-3.3.2/src/magplan/migrations/0008_auto_20210318_0108.py
+-rw-r--r--   0        0        0      610 2024-04-15 10:12:07.588161 magplan-3.3.2/src/magplan/migrations/0009_auto_20210523_1641.py
+-rw-r--r--   0        0        0     2847 2024-05-01 06:06:17.371144 magplan-3.3.2/src/magplan/migrations/0010_auto_20210624_1041.py
+-rw-r--r--   0        0        0     1274 2024-04-15 10:12:07.610111 magplan-3.3.2/src/magplan/migrations/0011_auto_20210624_1817.py
+-rw-r--r--   0        0        0      984 2024-05-01 19:26:54.597594 magplan-3.3.2/src/magplan/migrations/0012_alter_attachment_meta_alter_comment_meta_and_more.py
+-rw-r--r--   0        0        0     1818 2024-05-01 06:14:08.213881 magplan-3.3.2/src/magplan/migrations/0013_sitepreferencemodel.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/migrations/__init__.py
+-rw-r--r--   0        0        0    28566 2024-05-01 18:57:36.931525 magplan-3.3.2/src/magplan/models.py
+-rw-r--r--   0        0        0      200 2024-05-01 06:06:18.391401 magplan-3.3.2/src/magplan/registries.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/tasks/__init__.py
+-rw-r--r--   0        0        0     3873 2024-05-01 06:14:12.297514 magplan-3.3.2/src/magplan/tasks/send_idea_comment_notification.py
+-rw-r--r--   0        0        0      468 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/tasks/send_idea_notification.py
+-rw-r--r--   0        0        0     4260 2024-05-01 06:14:12.298004 magplan-3.3.2/src/magplan/tasks/send_post_comment_notification.py
+-rw-r--r--   0        0        0      542 2024-05-01 06:06:17.480250 magplan-3.3.2/src/magplan/tasks/upload_post_to_wp.py
+-rw-r--r--   0        0        0     1790 2024-05-01 06:14:08.227137 magplan-3.3.2/src/magplan/tasks/utils.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-01 06:14:12.276731 magplan-3.3.2/src/magplan/templates/_test_issues.py
+-rw-r--r--   0        0        0      758 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/email/_vote_from_email.html
+-rw-r--r--   0        0        0      416 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/email/assigned_to_you.html
+-rw-r--r--   0        0        0      701 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/email/idea_approved.html
+-rw-r--r--   0        0        0      634 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/email/new_comment.html
+-rw-r--r--   0        0        0      370 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/email/new_idea.html
+-rw-r--r--   0        0        0     8503 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/layout_plan.html
+-rw-r--r--   0        0        0      893 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/articles/advert.html
+-rw-r--r--   0        0        0      860 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/articles/archived.html
+-rw-r--r--   0        0        0      855 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/articles/default.html
+-rw-r--r--   0        0        0     3053 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/articles/index.html
+-rw-r--r--   0        0        0      911 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/articles/whitelisted.html
+-rw-r--r--   0        0        0     4121 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/authors/_form.html
+-rw-r--r--   0        0        0      541 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/authors/edit.html
+-rw-r--r--   0        0        0      869 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/authors/index.html
+-rw-r--r--   0        0        0      480 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/authors/new.html
+-rw-r--r--   0        0        0     1077 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/authors/show.html
+-rw-r--r--   0        0        0      595 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/ideas/_approve_ideas.html
+-rw-r--r--   0        0        0      786 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/ideas/_authors_list.html
+-rw-r--r--   0        0        0     2332 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/ideas/_form_base.html
+-rw-r--r--   0        0        0     1088 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/ideas/_vote.html
+-rw-r--r--   0        0        0     1521 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/ideas/_voting_results.html
+-rw-r--r--   0        0        0     3959 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/ideas/index.html
+-rw-r--r--   0        0        0     3149 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/ideas/show.html
+-rw-r--r--   0        0        0     4404 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/index/index.html
+-rw-r--r--   0        0        0     1786 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/issues/_form.html
+-rw-r--r--   0        0        0     1202 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/issues/index.html
+-rw-r--r--   0        0        0      477 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/issues/new.html
+-rw-r--r--   0        0        0      837 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/issues/show.html
+-rw-r--r--   0        0        0      573 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/partials/_navbar.sites.html
+-rw-r--r--   0        0        0     1395 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/partials/_navbar_header_links.html
+-rw-r--r--   0        0        0     2797 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/partials/comments.html
+-rw-r--r--   0        0        0     2252 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/partials/navbar.html
+-rw-r--r--   0        0        0     3180 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/partials/posts_table.html
+-rw-r--r--   0        0        0      956 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/_admin_set_stage.html
+-rw-r--r--   0        0        0     6970 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/_attachments.html
+-rw-r--r--   0        0        0      768 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/_field_col.html
+-rw-r--r--   0        0        0     3389 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/_form_base.html
+-rw-r--r--   0        0        0     3359 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/_form_meta.html
+-rw-r--r--   0        0        0      286 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/_paywall_alert.html
+-rw-r--r--   0        0        0     1063 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/_progress.html
+-rw-r--r--   0        0        0      882 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/_schedule.html
+-rw-r--r--   0        0        0     2437 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/_stages.html
+-rw-r--r--   0        0        0     8559 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/edit.html
+-rw-r--r--   0        0        0     9102 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/posts/show.html
+-rw-r--r--   0        0        0      345 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/preferences/index.html
+-rw-r--r--   0        0        0      804 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/sections/index.html
+-rw-r--r--   0        0        0     1607 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templates/magplan/stages/index.html
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/templatetags/__init__.py
+-rw-r--r--   0        0        0     6000 2024-05-01 06:06:17.346132 magplan-3.3.2/src/magplan/templatetags/filters.py
+-rw-r--r--   0        0        0     2814 2024-05-01 06:14:12.331038 magplan-3.3.2/src/magplan/urls.py
+-rw-r--r--   0        0        0     1248 2024-04-15 15:19:59.641866 magplan-3.3.2/src/magplan/utils.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/views/__init__.py
+-rw-r--r--   0        0        0      898 2024-04-15 10:12:07.737198 magplan-3.3.2/src/magplan/views/api.py
+-rw-r--r--   0        0        0     6338 2024-05-01 06:38:18.611005 magplan-3.3.2/src/magplan/views/articles.py
+-rw-r--r--   0        0        0     3041 2024-05-01 06:14:08.519369 magplan-3.3.2/src/magplan/views/authors.py
+-rw-r--r--   0        0        0     7950 2024-05-01 06:14:12.432610 magplan-3.3.2/src/magplan/views/ideas.py
+-rw-r--r--   0        0        0     3321 2024-05-01 06:14:08.537681 magplan-3.3.2/src/magplan/views/index.py
+-rw-r--r--   0        0        0     1859 2024-05-01 06:14:08.558308 magplan-3.3.2/src/magplan/views/issues.py
+-rw-r--r--   0        0        0    16990 2024-05-01 06:14:12.645881 magplan-3.3.2/src/magplan/views/posts.py
+-rw-r--r--   0        0        0     1134 2024-05-01 06:14:08.564285 magplan-3.3.2/src/magplan/views/preferences.py
+-rw-r--r--   0        0        0      337 2024-05-01 06:06:17.714358 magplan-3.3.2/src/magplan/views/sections.py
+-rw-r--r--   0        0        0      474 2024-05-01 06:06:17.782732 magplan-3.3.2/src/magplan/views/stages.py
+-rw-r--r--   0        0        0      390 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/xmd/README.md
+-rw-r--r--   0        0        0       27 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/xmd/__init__.py
+-rw-r--r--   0        0        0     2909 2024-05-01 06:14:08.651159 magplan-3.3.2/src/magplan/xmd/lexers.py
+-rw-r--r--   0        0        0      874 2024-04-15 10:08:50.159967 magplan-3.3.2/src/magplan/xmd/mappers.py
+-rw-r--r--   0        0        0     1397 2024-04-15 10:08:50.169892 magplan-3.3.2/src/magplan/xmd/markdown.py
+-rw-r--r--   0        0        0     2561 2024-05-01 06:14:08.666180 magplan-3.3.2/src/magplan/xmd/renderer.py
+-rw-r--r--   0        0        0      313 2024-04-15 10:08:50.175035 magplan-3.3.2/src/magplan/xmd/templates.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.2/src/magplan/xmd/tests/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-01 06:06:17.586779 magplan-3.3.2/src/magplan/xmd/tests/conftest.py
+-rw-r--r--   0        0        0     5168 2024-05-01 06:14:08.736635 magplan-3.3.2/src/magplan/xmd/tests/test_lexer.py
+-rw-r--r--   0        0        0     1526 2024-05-01 06:14:08.660016 magplan-3.3.2/src/magplan/xmd/tests/test_renderer.py
+-rw-r--r--   0        0        0     1274 2024-05-01 06:06:18.926242 magplan-3.3.2/src/magplan/xmd/tests/test_utils.py
+-rw-r--r--   0        0        0      478 2024-04-15 10:08:50.208773 magplan-3.3.2/src/magplan/xmd/utils.py
+-rw-r--r--   0        0        0      957 2024-04-15 10:08:50.224860 magplan-3.3.2/src/magplan/xmd/xmd.py
+-rw-r--r--   0        0        0     7220 1970-01-01 00:00:00.000000 magplan-3.3.2/PKG-INFO
```

### Comparing `magplan-3.3.1/README.md` & `magplan-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/pyproject.toml` & `magplan-3.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magplan"
-version = "3.3.1"
+version = "3.3.2"
 description = ""
 authors = ["Ilya Rusanen <ilya@rusanen.co.uk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.34.0"
```

### Comparing `magplan-3.3.1/src/magplan/admin.py` & `magplan-3.3.2/src/magplan/admin.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/conf/settings.py` & `magplan-3.3.2/src/magplan/conf/settings.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/context_processors.py` & `magplan-3.3.2/src/magplan/context_processors.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/dynamic_preferences_registry.py` & `magplan-3.3.2/src/magplan/dynamic_preferences_registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django import forms
+from django.contrib.sites.models import Site
 from dynamic_preferences.preferences import Section
 from dynamic_preferences.types import ChoicePreference, StringPreference
 from dynamic_preferences.users.registries import user_preferences_registry
 
 from magplan.registries import site_preferences_registry
 
 general = Section("general")
@@ -73,8 +74,18 @@
     section = plan
     choices = [
         ("yes", "Да"),
         ("no", "Нет"),
     ]
     default = "yes"
     widget = forms.Select(attrs={"class": "form-control"})
-    verbose_name = "Присылать уведомелния о новых идеях?"
+    verbose_name = "Присылать уведомления о новых идеях?"
+
+
+@user_preferences_registry.register
+class PlanCurrentSite(ChoicePreference):
+    name = "current_site"
+    section = plan
+    choices = [(str(s.id), s.name) for s in Site.objects.all()]
+    default = "1"
+    widget = forms.Select(attrs={"class": "form-control"})
+    verbose_name = "Текущий сайт"
```

### Comparing `magplan-3.3.1/src/magplan/fixtures/db_test.json` & `magplan-3.3.2/src/magplan/fixtures/db_test.json`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/forms.py` & `magplan-3.3.2/src/magplan/forms.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/integrations/images.py` & `magplan-3.3.2/src/magplan/integrations/images.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/integrations/posts.py` & `magplan-3.3.2/src/magplan/integrations/posts.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/locale/en/LC_MESSAGES/django.mo` & `magplan-3.3.2/src/magplan/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/locale/en/LC_MESSAGES/django.po` & `magplan-3.3.2/src/magplan/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/locale/ru/LC_MESSAGES/django.mo` & `magplan-3.3.2/src/magplan/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/locale/ru/LC_MESSAGES/django.po` & `magplan-3.3.2/src/magplan/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/middleware.py` & `magplan-3.3.2/src/magplan/middleware.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0001_initial.py` & `magplan-3.3.2/src/magplan/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0002_auto_20201115_1140.py` & `magplan-3.3.2/src/magplan/migrations/0002_auto_20201115_1140.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0003_auto_20201121_1750.py` & `magplan-3.3.2/src/magplan/migrations/0003_auto_20201121_1750.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0004_post_features.py` & `magplan-3.3.2/src/magplan/migrations/0004_post_features.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0005_auto_20210213_1556.py` & `magplan-3.3.2/src/magplan/migrations/0005_auto_20210213_1556.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0006_auto_20210316_1840.py` & `magplan-3.3.2/src/magplan/migrations/0006_auto_20210316_1840.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0007_auto_20210316_1900.py` & `magplan-3.3.2/src/magplan/migrations/0007_auto_20210316_1900.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0008_auto_20210318_0108.py` & `magplan-3.3.2/src/magplan/migrations/0008_auto_20210318_0108.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0009_auto_20210523_1641.py` & `magplan-3.3.2/src/magplan/migrations/0009_auto_20210523_1641.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0010_auto_20210624_1041.py` & `magplan-3.3.2/src/magplan/migrations/0010_auto_20210624_1041.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0011_auto_20210624_1817.py` & `magplan-3.3.2/src/magplan/migrations/0011_auto_20210624_1817.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0012_alter_attachment_meta_alter_comment_meta_and_more.py` & `magplan-3.3.2/src/magplan/migrations/0012_alter_attachment_meta_alter_comment_meta_and_more.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/migrations/0013_sitepreferencemodel.py` & `magplan-3.3.2/src/magplan/migrations/0013_sitepreferencemodel.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/models.py` & `magplan-3.3.2/src/magplan/models.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/tasks/send_idea_comment_notification.py` & `magplan-3.3.2/src/magplan/tasks/send_idea_comment_notification.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/tasks/send_post_comment_notification.py` & `magplan-3.3.2/src/magplan/tasks/send_post_comment_notification.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/tasks/upload_post_to_wp.py` & `magplan-3.3.2/src/magplan/tasks/upload_post_to_wp.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/tasks/utils.py` & `magplan-3.3.2/src/magplan/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/_test_issues.py` & `magplan-3.3.2/src/magplan/templates/_test_issues.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/email/_vote_from_email.html` & `magplan-3.3.2/src/magplan/templates/email/_vote_from_email.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/email/idea_approved.html` & `magplan-3.3.2/src/magplan/templates/email/idea_approved.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/email/new_comment.html` & `magplan-3.3.2/src/magplan/templates/email/new_comment.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/layout_plan.html` & `magplan-3.3.2/src/magplan/templates/layout_plan.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/articles/advert.html` & `magplan-3.3.2/src/magplan/templates/magplan/articles/advert.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/articles/archived.html` & `magplan-3.3.2/src/magplan/templates/magplan/articles/archived.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/articles/default.html` & `magplan-3.3.2/src/magplan/templates/magplan/articles/default.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/articles/index.html` & `magplan-3.3.2/src/magplan/templates/magplan/articles/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/articles/whitelisted.html` & `magplan-3.3.2/src/magplan/templates/magplan/articles/whitelisted.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/authors/_form.html` & `magplan-3.3.2/src/magplan/templates/magplan/authors/_form.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/authors/edit.html` & `magplan-3.3.2/src/magplan/templates/magplan/authors/edit.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/authors/index.html` & `magplan-3.3.2/src/magplan/templates/magplan/authors/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/authors/show.html` & `magplan-3.3.2/src/magplan/templates/magplan/authors/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/ideas/_approve_ideas.html` & `magplan-3.3.2/src/magplan/templates/magplan/ideas/_approve_ideas.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/ideas/_authors_list.html` & `magplan-3.3.2/src/magplan/templates/magplan/ideas/_authors_list.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/ideas/_form_base.html` & `magplan-3.3.2/src/magplan/templates/magplan/ideas/_form_base.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/ideas/_vote.html` & `magplan-3.3.2/src/magplan/templates/magplan/ideas/_vote.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/ideas/_voting_results.html` & `magplan-3.3.2/src/magplan/templates/magplan/ideas/_voting_results.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/ideas/index.html` & `magplan-3.3.2/src/magplan/templates/magplan/ideas/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/ideas/show.html` & `magplan-3.3.2/src/magplan/templates/magplan/ideas/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/index/index.html` & `magplan-3.3.2/src/magplan/templates/magplan/index/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/issues/_form.html` & `magplan-3.3.2/src/magplan/templates/magplan/issues/_form.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/issues/index.html` & `magplan-3.3.2/src/magplan/templates/magplan/issues/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/issues/show.html` & `magplan-3.3.2/src/magplan/templates/magplan/issues/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/partials/_navbar.sites.html` & `magplan-3.3.2/src/magplan/templates/magplan/partials/_navbar.sites.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/partials/_navbar_header_links.html` & `magplan-3.3.2/src/magplan/templates/magplan/partials/_navbar_header_links.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/partials/comments.html` & `magplan-3.3.2/src/magplan/templates/magplan/partials/comments.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/partials/navbar.html` & `magplan-3.3.2/src/magplan/templates/magplan/partials/navbar.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/partials/posts_table.html` & `magplan-3.3.2/src/magplan/templates/magplan/partials/posts_table.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/posts/_admin_set_stage.html` & `magplan-3.3.2/src/magplan/templates/magplan/posts/_admin_set_stage.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/posts/_attachments.html` & `magplan-3.3.2/src/magplan/templates/magplan/posts/_attachments.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/posts/_field_col.html` & `magplan-3.3.2/src/magplan/templates/magplan/posts/_field_col.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/posts/_form_base.html` & `magplan-3.3.2/src/magplan/templates/magplan/posts/_form_base.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/posts/_form_meta.html` & `magplan-3.3.2/src/magplan/templates/magplan/posts/_form_meta.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/posts/_progress.html` & `magplan-3.3.2/src/magplan/templates/magplan/posts/_progress.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/posts/_schedule.html` & `magplan-3.3.2/src/magplan/templates/magplan/posts/_schedule.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/posts/_stages.html` & `magplan-3.3.2/src/magplan/templates/magplan/posts/_stages.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/posts/edit.html` & `magplan-3.3.2/src/magplan/templates/magplan/posts/edit.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/posts/show.html` & `magplan-3.3.2/src/magplan/templates/magplan/posts/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/sections/index.html` & `magplan-3.3.2/src/magplan/templates/magplan/sections/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templates/magplan/stages/index.html` & `magplan-3.3.2/src/magplan/templates/magplan/stages/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/templatetags/filters.py` & `magplan-3.3.2/src/magplan/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/urls.py` & `magplan-3.3.2/src/magplan/urls.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/utils.py` & `magplan-3.3.2/src/magplan/utils.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/views/api.py` & `magplan-3.3.2/src/magplan/views/api.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/views/articles.py` & `magplan-3.3.2/src/magplan/views/articles.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/views/authors.py` & `magplan-3.3.2/src/magplan/views/authors.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/views/ideas.py` & `magplan-3.3.2/src/magplan/views/ideas.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/views/index.py` & `magplan-3.3.2/src/magplan/views/index.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/views/issues.py` & `magplan-3.3.2/src/magplan/views/issues.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/views/posts.py` & `magplan-3.3.2/src/magplan/views/posts.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/views/preferences.py` & `magplan-3.3.2/src/magplan/views/preferences.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/xmd/lexers.py` & `magplan-3.3.2/src/magplan/xmd/lexers.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/xmd/mappers.py` & `magplan-3.3.2/src/magplan/xmd/mappers.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/xmd/markdown.py` & `magplan-3.3.2/src/magplan/xmd/markdown.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/xmd/renderer.py` & `magplan-3.3.2/src/magplan/xmd/renderer.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/xmd/tests/test_lexer.py` & `magplan-3.3.2/src/magplan/xmd/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/xmd/tests/test_renderer.py` & `magplan-3.3.2/src/magplan/xmd/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/xmd/tests/test_utils.py` & `magplan-3.3.2/src/magplan/xmd/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/src/magplan/xmd/xmd.py` & `magplan-3.3.2/src/magplan/xmd/xmd.py`

 * *Files identical despite different names*

### Comparing `magplan-3.3.1/PKG-INFO` & `magplan-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magplan
-Version: 3.3.1
+Version: 3.3.2
 Summary: 
 Author: Ilya Rusanen
 Author-email: ilya@rusanen.co.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

