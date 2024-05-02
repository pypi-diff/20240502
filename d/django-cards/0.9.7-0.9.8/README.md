# Comparing `tmp/django-cards-0.9.7.tar.gz` & `tmp/django-cards-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cards-0.9.7.tar", last modified: Tue Dec  5 11:46:04 2023, max compression
+gzip compressed data, was "django-cards-0.9.8.tar", last modified: Tue Dec  5 15:43:28 2023, max compression
```

## Comparing `django-cards-0.9.7.tar` & `django-cards-0.9.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.513489 django-cards-0.9.7/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-08-02 21:08:42.000000 django-cards-0.9.7/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       55 2023-08-02 21:08:42.000000 django-cards-0.9.7/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      551 2023-12-05 11:46:04.513352 django-cards-0.9.7/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      130 2023-08-02 21:08:42.000000 django-cards-0.9.7/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.505720 django-cards-0.9.7/cards/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      166 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/apps.py
--rw-r--r--   0 tom        (501) staff       (20)    26980 2023-12-05 11:41:56.000000 django-cards-0.9.7/cards/base.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.506168 django-cards-0.9.7/cards/card_list/
--rw-r--r--   0 tom        (501) staff       (20)      115 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/card_list/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     5753 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/card_list/base.py
--rw-r--r--   0 tom        (501) staff       (20)     3952 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/card_list/main.py
--rw-r--r--   0 tom        (501) staff       (20)     2468 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/card_list/tree.py
--rw-r--r--   0 tom        (501) staff       (20)      714 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/includes.py
--rw-r--r--   0 tom        (501) staff       (20)     5498 2023-12-05 11:31:51.000000 django-cards-0.9.7/cards/standard.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.503514 django-cards-0.9.7/cards/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.503568 django-cards-0.9.7/cards/static/cards/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.504080 django-cards-0.9.7/cards/static/cards/jstree/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.503677 django-cards-0.9.7/cards/static/cards/jstree/css/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.503878 django-cards-0.9.7/cards/static/cards/jstree/css/themes/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.507110 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/
--rw-r--r--   0 tom        (501) staff       (20)     5660 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/32px.png
--rw-r--r--   0 tom        (501) staff       (20)     2215 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/40px.png
--rw-r--r--   0 tom        (501) staff       (20)    31722 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/style.css
--rw-r--r--   0 tom        (501) staff       (20)    27353 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1464 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.507857 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/
--rw-r--r--   0 tom        (501) staff       (20)     1525 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/32px.png
--rw-r--r--   0 tom        (501) staff       (20)     6526 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/40px.png
--rw-r--r--   0 tom        (501) staff       (20)    34459 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/style.css
--rw-r--r--   0 tom        (501) staff       (20)    29959 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1464 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.508578 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/
--rw-r--r--   0 tom        (501) staff       (20)     6423 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/30px.png
--rw-r--r--   0 tom        (501) staff       (20)     3333 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/32px.png
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.504008 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.510662 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/
--rw-r--r--   0 tom        (501) staff       (20)    24108 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   134830 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    49936 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    27344 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    24056 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   140377 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    50224 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    27108 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    25059 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   150837 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    50788 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    28152 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    32574 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/style.css
--rw-r--r--   0 tom        (501) staff       (20)    27752 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1720 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.511084 django-cards-0.9.7/cards/static/cards/jstree/js/
--rw-r--r--   0 tom        (501) staff       (20)   307794 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/js/jstree.js
--rw-r--r--   0 tom        (501) staff       (20)   141222 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/static/cards/jstree/js/jstree.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.504203 django-cards-0.9.7/cards/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.504327 django-cards-0.9.7/cards/templates/cards/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.511279 django-cards-0.9.7/cards/templates/cards/groups/
--rw-r--r--   0 tom        (501) staff       (20)      206 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/groups/groups.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.512537 django-cards-0.9.7/cards/templates/cards/standard/
--rw-r--r--   0 tom        (501) staff       (20)       69 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/standard/blank.html
--rw-r--r--   0 tom        (501) staff       (20)     1588 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/standard/card_group.html
--rw-r--r--   0 tom        (501) staff       (20)     2212 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/standard/datatable.html
--rw-r--r--   0 tom        (501) staff       (20)      778 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/standard/default.html
--rw-r--r--   0 tom        (501) staff       (20)     1747 2023-12-05 11:31:51.000000 django-cards-0.9.7/cards/templates/cards/standard/default_body.html
--rw-r--r--   0 tom        (501) staff       (20)     1079 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/standard/html.html
--rw-r--r--   0 tom        (501) staff       (20)     2606 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/standard/list_selection.html
--rw-r--r--   0 tom        (501) staff       (20)      576 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/standard/message.html
--rw-r--r--   0 tom        (501) staff       (20)      859 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/standard/table.html
--rw-r--r--   0 tom        (501) staff       (20)     1547 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/standard/table_body.html
--rw-r--r--   0 tom        (501) staff       (20)     2198 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templates/cards/standard/tree_selection.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.512738 django-cards-0.9.7/cards/templatetags/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templatetags/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      362 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/templatetags/django_cards_tags.py
--rw-r--r--   0 tom        (501) staff       (20)      115 2023-08-02 21:08:42.000000 django-cards-0.9.7/cards/url_converters.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 11:46:04.513188 django-cards-0.9.7/django_cards.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      551 2023-12-05 11:46:04.000000 django-cards-0.9.7/django_cards.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     3065 2023-12-05 11:46:04.000000 django-cards-0.9.7/django_cards.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-12-05 11:46:04.000000 django-cards-0.9.7/django_cards.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-12-05 11:46:04.000000 django-cards-0.9.7/django_cards.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-12-05 11:46:04.513535 django-cards-0.9.7/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      645 2023-12-05 11:41:56.000000 django-cards-0.9.7/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.073981 django-cards-0.9.8/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-08-02 21:08:42.000000 django-cards-0.9.8/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       55 2023-08-02 21:08:42.000000 django-cards-0.9.8/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      551 2023-12-05 15:43:28.073853 django-cards-0.9.8/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      130 2023-08-02 21:08:42.000000 django-cards-0.9.8/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.066304 django-cards-0.9.8/cards/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      166 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)    26980 2023-12-05 11:41:56.000000 django-cards-0.9.8/cards/base.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.066749 django-cards-0.9.8/cards/card_list/
+-rw-r--r--   0 tom        (501) staff       (20)      115 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/card_list/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     5753 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/card_list/base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3952 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/card_list/main.py
+-rw-r--r--   0 tom        (501) staff       (20)     2468 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/card_list/tree.py
+-rw-r--r--   0 tom        (501) staff       (20)      714 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/includes.py
+-rw-r--r--   0 tom        (501) staff       (20)     5498 2023-12-05 11:31:51.000000 django-cards-0.9.8/cards/standard.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.064159 django-cards-0.9.8/cards/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.064212 django-cards-0.9.8/cards/static/cards/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.064715 django-cards-0.9.8/cards/static/cards/jstree/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.064322 django-cards-0.9.8/cards/static/cards/jstree/css/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.064516 django-cards-0.9.8/cards/static/cards/jstree/css/themes/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.067638 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/
+-rw-r--r--   0 tom        (501) staff       (20)     5660 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/32px.png
+-rw-r--r--   0 tom        (501) staff       (20)     2215 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/40px.png
+-rw-r--r--   0 tom        (501) staff       (20)    31722 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    27353 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1464 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.068401 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/
+-rw-r--r--   0 tom        (501) staff       (20)     1525 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/32px.png
+-rw-r--r--   0 tom        (501) staff       (20)     6526 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/40px.png
+-rw-r--r--   0 tom        (501) staff       (20)    34459 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    29959 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1464 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.069152 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/
+-rw-r--r--   0 tom        (501) staff       (20)     6423 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/30px.png
+-rw-r--r--   0 tom        (501) staff       (20)     3333 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/32px.png
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.064642 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.071229 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/
+-rw-r--r--   0 tom        (501) staff       (20)    24108 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   134830 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    49936 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    27344 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    24056 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   140377 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    50224 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    27108 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    25059 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   150837 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    50788 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    28152 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    32574 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    27752 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1720 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.071655 django-cards-0.9.8/cards/static/cards/jstree/js/
+-rw-r--r--   0 tom        (501) staff       (20)   307794 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/js/jstree.js
+-rw-r--r--   0 tom        (501) staff       (20)   141222 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/static/cards/jstree/js/jstree.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.064844 django-cards-0.9.8/cards/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.064969 django-cards-0.9.8/cards/templates/cards/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.071851 django-cards-0.9.8/cards/templates/cards/groups/
+-rw-r--r--   0 tom        (501) staff       (20)      206 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templates/cards/groups/groups.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.073057 django-cards-0.9.8/cards/templates/cards/standard/
+-rw-r--r--   0 tom        (501) staff       (20)       69 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templates/cards/standard/blank.html
+-rw-r--r--   0 tom        (501) staff       (20)     1588 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templates/cards/standard/card_group.html
+-rw-r--r--   0 tom        (501) staff       (20)     2212 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templates/cards/standard/datatable.html
+-rw-r--r--   0 tom        (501) staff       (20)      778 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templates/cards/standard/default.html
+-rw-r--r--   0 tom        (501) staff       (20)     1747 2023-12-05 11:31:51.000000 django-cards-0.9.8/cards/templates/cards/standard/default_body.html
+-rw-r--r--   0 tom        (501) staff       (20)     1079 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templates/cards/standard/html.html
+-rw-r--r--   0 tom        (501) staff       (20)     3088 2023-12-05 15:13:54.000000 django-cards-0.9.8/cards/templates/cards/standard/list_selection.html
+-rw-r--r--   0 tom        (501) staff       (20)      576 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templates/cards/standard/message.html
+-rw-r--r--   0 tom        (501) staff       (20)      859 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templates/cards/standard/table.html
+-rw-r--r--   0 tom        (501) staff       (20)     1547 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templates/cards/standard/table_body.html
+-rw-r--r--   0 tom        (501) staff       (20)     2198 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templates/cards/standard/tree_selection.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.073258 django-cards-0.9.8/cards/templatetags/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templatetags/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      362 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/templatetags/django_cards_tags.py
+-rw-r--r--   0 tom        (501) staff       (20)      115 2023-08-02 21:08:42.000000 django-cards-0.9.8/cards/url_converters.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-12-05 15:43:28.073700 django-cards-0.9.8/django_cards.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      551 2023-12-05 15:43:28.000000 django-cards-0.9.8/django_cards.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     3065 2023-12-05 15:43:28.000000 django-cards-0.9.8/django_cards.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-12-05 15:43:28.000000 django-cards-0.9.8/django_cards.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-12-05 15:43:28.000000 django-cards-0.9.8/django_cards.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-12-05 15:43:28.074025 django-cards-0.9.8/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      645 2023-12-05 15:42:07.000000 django-cards-0.9.8/setup.py
```

### Comparing `django-cards-0.9.7/LICENSE` & `django-cards-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/PKG-INFO` & `django-cards-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cards
-Version: 0.9.7
+Version: 0.9.8
 Summary: Django app that allows you make cards
 Home-page: https://github.com/django-advance-utils/django-cards
 Author: Thomas Turner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `django-cards-0.9.7/cards/base.py` & `django-cards-0.9.8/cards/base.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/card_list/base.py` & `django-cards-0.9.8/cards/card_list/base.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/card_list/main.py` & `django-cards-0.9.8/cards/card_list/main.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/card_list/tree.py` & `django-cards-0.9.8/cards/card_list/tree.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/includes.py` & `django-cards-0.9.8/cards/includes.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/standard.py` & `django-cards-0.9.8/cards/standard.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/32px.png` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/40px.png` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/40px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/style.css` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/style.min.css` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/default/throbber.gif` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/32px.png` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/40px.png` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/40px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/style.css` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/style.min.css` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/default-dark/throbber.gif` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/default-dark/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/30px.png` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/30px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/32px.png` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/style.css` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/style.min.css` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/css/themes/proton/throbber.gif` & `django-cards-0.9.8/cards/static/cards/jstree/css/themes/proton/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/js/jstree.js` & `django-cards-0.9.8/cards/static/cards/jstree/js/jstree.js`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/static/cards/jstree/js/jstree.min.js` & `django-cards-0.9.8/cards/static/cards/jstree/js/jstree.min.js`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/templates/cards/standard/card_group.html` & `django-cards-0.9.8/cards/templates/cards/standard/card_group.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/templates/cards/standard/datatable.html` & `django-cards-0.9.8/cards/templates/cards/standard/datatable.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/templates/cards/standard/default.html` & `django-cards-0.9.8/cards/templates/cards/standard/default.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/templates/cards/standard/default_body.html` & `django-cards-0.9.8/cards/templates/cards/standard/default_body.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/templates/cards/standard/html.html` & `django-cards-0.9.8/cards/templates/cards/standard/html.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/templates/cards/standard/message.html` & `django-cards-0.9.8/cards/templates/cards/standard/message.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/templates/cards/standard/table.html` & `django-cards-0.9.8/cards/templates/cards/standard/table.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/templates/cards/standard/table_body.html` & `django-cards-0.9.8/cards/templates/cards/standard/table_body.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/cards/templates/cards/standard/tree_selection.html` & `django-cards-0.9.8/cards/templates/cards/standard/tree_selection.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/django_cards.egg-info/PKG-INFO` & `django-cards-0.9.8/django_cards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cards
-Version: 0.9.7
+Version: 0.9.8
 Summary: Django app that allows you make cards
 Home-page: https://github.com/django-advance-utils/django-cards
 Author: Thomas Turner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `django-cards-0.9.7/django_cards.egg-info/SOURCES.txt` & `django-cards-0.9.8/django_cards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.7/setup.py` & `django-cards-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-cards",
-    version="0.9.7",
+    version="0.9.8",
     author="Thomas Turner",
     description="Django app that allows you make cards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-cards",
     include_package_data=True,
     packages=['cards'],
```

