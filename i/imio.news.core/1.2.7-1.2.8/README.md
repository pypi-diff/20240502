# Comparing `tmp/imio.news.core-1.2.7.tar.gz` & `tmp/imio.news.core-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.news.core-1.2.7.tar", last modified: Thu Apr  4 15:57:26 2024, max compression
+gzip compressed data, was "dist/imio.news.core-1.2.8.tar", last modified: Thu May  2 10:47:53 2024, max compression
```

## Comparing `imio.news.core-1.2.7.tar` & `imio.news.core-1.2.8.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3423 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      665 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      106 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6701 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2209 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/README.rst
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7986 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       65 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/requirements.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/setup.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2328 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/setup.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.784553 imio.news.core-1.2.7/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      259 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/browser/bring_news_into_news_folders/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/bring_news_into_news_folders/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      392 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/bring_news_into_news_folders/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3557 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      595 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/overrides/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/browser/static/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      791 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/contents/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      226 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/contents/entity/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/entity/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/entity/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1742 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/entity/content.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/contents/folder/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/folder/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/folder/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/folder/content.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio/news/core/contents/newsfolder/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsfolder/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsfolder/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1236 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsfolder/content.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      690 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5073 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5483 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/serializer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5608 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2415 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/converters.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.784553 imio.news.core-1.2.7/src/imio/news/core/faceted/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6592 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/faceted/config/news.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4126 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/indexers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1543 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/indexers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      199 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      347 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/overrides.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      762 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.784553 imio.news.core-1.2.7/src/imio/news/core/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      167 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2007 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2843 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/contentrules.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/diff_tool.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      449 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      743 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/repositorytool.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      980 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      295 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/Plone_Site.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1613 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1372 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1432 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1554 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      361 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/default/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      124 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      876 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/profiles.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/serializer/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/serializer/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      175 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/serializer/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      579 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/serializer/newsitem.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      663 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/setuphandlers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6032 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/subscribers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1342 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1805 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/testing.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/tests/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/resources/plone.png
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1987 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2801 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_bring_news_into_news_folders.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1598 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3380 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_entity.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3550 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_indexer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2222 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_local_roles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8040 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_multilingual.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9084 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_newsfolder.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14046 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_newsitem.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      929 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1950 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3490 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5134 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/test_vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/tests/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/upgrades/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4744 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.784553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1003_to_1004/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.792553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2843 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/diff_tool.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/repositorytool.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      282 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/types/imio.news.NewsItem.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1007_to_1008/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      743 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.784553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      305 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      305 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      309 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsFolder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      307 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsItem.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1009_to_1010/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      218 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1009_to_1010/rolemap.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2185 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1660 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/viewlets/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/viewlets/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      519 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/viewlets/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.796553 imio.news.core-1.2.7/src/imio/news/core/viewlets/news/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      357 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/viewlets/news/button_to_bring_news.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1121 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/viewlets/news.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4363 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1003 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio/news/core/vocabularies.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-04 15:57:26.788553 imio.news.core-1.2.7/src/imio.news.core.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6701 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4992 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       15 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      278 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2024-04-04 15:57:26.000000 imio.news.core-1.2.7/src/imio.news.core.egg-info/top_level.txt
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/
+-rw-r--r--   0 laurent    (501) staff       (20)     3564 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/CHANGES.rst
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/CONTRIBUTORS.rst
+-rw-r--r--   0 laurent    (501) staff       (20)      522 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/DEVELOP.rst
+-rw-r--r--   0 laurent    (501) staff       (20)    18092 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/LICENSE.GPL
+-rw-r--r--   0 laurent    (501) staff       (20)      665 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/LICENSE.rst
+-rw-r--r--   0 laurent    (501) staff       (20)      106 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/MANIFEST.in
+-rw-r--r--   0 laurent    (501) staff       (20)     6862 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     2209 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/README.rst
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     7986 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/docs/conf.py
+-rw-r--r--   0 laurent    (501) staff       (20)       65 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/docs/index.rst
+-rw-r--r--   0 laurent    (501) staff       (20)       64 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/requirements.txt
+-rw-r--r--   0 laurent    (501) staff       (20)      518 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/setup.cfg
+-rw-r--r--   0 laurent    (501) staff       (20)     2328 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/setup.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/
+-rw-r--r--   0 laurent    (501) staff       (20)      259 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/browser/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/browser/bring_news_into_news_folders/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/bring_news_into_news_folders/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      392 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/bring_news_into_news_folders/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     3557 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py
+-rw-r--r--   0 laurent    (501) staff       (20)      595 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/browser/overrides/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/overrides/.gitkeep
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/browser/static/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/browser/static/.gitkeep
+-rw-r--r--   0 laurent    (501) staff       (20)      791 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/contents/
+-rw-r--r--   0 laurent    (501) staff       (20)      226 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      205 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/contents/entity/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/entity/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)       70 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/entity/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     1742 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/entity/content.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/contents/folder/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/folder/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)       70 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/folder/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      314 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/folder/content.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsfolder/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsfolder/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)       70 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsfolder/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     1236 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsfolder/content.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      690 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     5073 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/content.py
+-rw-r--r--   0 laurent    (501) staff       (20)     5483 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/serializer.py
+-rw-r--r--   0 laurent    (501) staff       (20)     5608 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/view.pt
+-rw-r--r--   0 laurent    (501) staff       (20)     2415 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/views.py
+-rw-r--r--   0 laurent    (501) staff       (20)      487 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/converters.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/faceted/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/faceted/config/
+-rw-r--r--   0 laurent    (501) staff       (20)     6592 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/faceted/config/news.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     4199 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/indexers.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1543 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/indexers.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      199 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/interfaces.py
+-rw-r--r--   0 laurent    (501) staff       (20)      347 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/overrides.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      762 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/permissions.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/
+-rw-r--r--   0 laurent    (501) staff       (20)      167 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/browserlayer.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     2007 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/catalog.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     2843 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/contentrules.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      205 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/diff_tool.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      449 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/metadata.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      743 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/registry.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      252 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/repositorytool.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      980 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/rolemap.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      295 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1613 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.Entity.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1372 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.Folder.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1432 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1554 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      361 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/default/types.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/uninstall/
+-rw-r--r--   0 laurent    (501) staff       (20)      124 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      876 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/profiles.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/serializer/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/serializer/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      175 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/serializer/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      579 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/serializer/newsitem.py
+-rw-r--r--   0 laurent    (501) staff       (20)      663 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/setuphandlers.py
+-rw-r--r--   0 laurent    (501) staff       (20)     6032 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/subscribers.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1342 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/subscribers.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     1805 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/testing.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/tests/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/tests/resources/
+-rw-r--r--   0 laurent    (501) staff       (20)    24753 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/resources/plone.png
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/tests/robot/
+-rw-r--r--   0 laurent    (501) staff       (20)     1987 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/robot/test_example.robot
+-rw-r--r--   0 laurent    (501) staff       (20)     2801 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_bring_news_into_news_folders.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1598 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_cropping.py
+-rw-r--r--   0 laurent    (501) staff       (20)     3380 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_entity.py
+-rw-r--r--   0 laurent    (501) staff       (20)     3550 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_indexer.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2222 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_local_roles.py
+-rw-r--r--   0 laurent    (501) staff       (20)     8040 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_multilingual.py
+-rw-r--r--   0 laurent    (501) staff       (20)     9084 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_newsfolder.py
+-rw-r--r--   0 laurent    (501) staff       (20)    14324 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_newsitem.py
+-rw-r--r--   0 laurent    (501) staff       (20)      929 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_robot.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1950 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_setup.py
+-rw-r--r--   0 laurent    (501) staff       (20)     3490 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_utils.py
+-rw-r--r--   0 laurent    (501) staff       (20)     5134 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/test_vocabularies.py
+-rw-r--r--   0 laurent    (501) staff       (20)      273 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/tests/utils.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)     5055 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1003_to_1004/
+-rw-r--r--   0 laurent    (501) staff       (20)     1066 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/
+-rw-r--r--   0 laurent    (501) staff       (20)     2843 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      205 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/diff_tool.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      252 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/repositorytool.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      282 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/types/imio.news.NewsItem.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1007_to_1008/
+-rw-r--r--   0 laurent    (501) staff       (20)      743 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      305 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Entity.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      305 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.Folder.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      309 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsFolder.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      307 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1008_to_1009/types/imio.news.NewsItem.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1009_to_1010/
+-rw-r--r--   0 laurent    (501) staff       (20)      218 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1009_to_1010/rolemap.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     2185 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/upgrades/upgrades.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1660 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/utils.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      519 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/news/
+-rw-r--r--   0 laurent    (501) staff       (20)      357 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/news/button_to_bring_news.pt
+-rw-r--r--   0 laurent    (501) staff       (20)     1069 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/viewlets/news.py
+-rw-r--r--   0 laurent    (501) staff       (20)     4363 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/vocabularies.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1003 2024-05-02 10:47:52.000000 imio.news.core-1.2.8/src/imio/news/core/vocabularies.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/
+-rw-r--r--   0 laurent    (501) staff       (20)     6862 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     4992 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/SOURCES.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/dependency_links.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       15 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/not-zip-safe
+-rw-r--r--   0 laurent    (501) staff       (20)      278 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/requires.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        5 2024-05-02 10:47:53.000000 imio.news.core-1.2.8/src/imio.news.core.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `imio.news.core-1.2.7/CHANGES.rst` & `imio.news.core-1.2.8/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.2.8 (2024-05-02)
+------------------
+
+- WEB-4101 : Use local category (if any) instead of category in `category_title` indexer
+  [laulaz]
+
+
 1.2.7 (2024-04-04)
 ------------------
 
 - Fix : serializer and message "At least one of these parameters must be supplied: path, UID"
   [boulch]
```

### Comparing `imio.news.core-1.2.7/DEVELOP.rst` & `imio.news.core-1.2.8/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/LICENSE.GPL` & `imio.news.core-1.2.8/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/LICENSE.rst` & `imio.news.core-1.2.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/PKG-INFO` & `imio.news.core-1.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: imio.news.core
-Version: 1.2.7
+Version: 1.2.8
 Summary: Core product for iMio news website
 Home-page: https://github.com/collective/imio.news.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.news.core
 Project-URL: Source, https://github.com/imio/imio.news.core
 Project-URL: Tracker, https://github.com/imio/imio.news.core/issues
 Keywords: Python Plone CMS
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -128,14 +129,21 @@
 - Christophe Boulanger, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.8 (2024-05-02)
+------------------
+
+- WEB-4101 : Use local category (if any) instead of category in `category_title` indexer
+  [laulaz]
+
+
 1.2.7 (2024-04-04)
 ------------------
 
 - Fix : serializer and message "At least one of these parameters must be supplied: path, UID"
   [boulch]
 
 
@@ -305,7 +313,9 @@
 
 
 1.0a1 (2022-01-25)
 ------------------
 
 - Initial release.
   [boulch]
+
+
```

### Comparing `imio.news.core-1.2.7/README.rst` & `imio.news.core-1.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/docs/conf.py` & `imio.news.core-1.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/setup.cfg` & `imio.news.core-1.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/setup.py` & `imio.news.core-1.2.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.news.core",
-    version="1.2.7",
+    version="1.2.8",
     description="Core product for iMio news website",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imio.news.core-1.2.7/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py` & `imio.news.core-1.2.8/src/imio/news/core/browser/bring_news_into_news_folders/news_folders.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/browser/configure.zcml` & `imio.news.core-1.2.8/src/imio/news/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/configure.zcml` & `imio.news.core-1.2.8/src/imio/news/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/contents/entity/content.py` & `imio.news.core-1.2.8/src/imio/news/core/contents/entity/content.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/contents/newsfolder/content.py` & `imio.news.core-1.2.8/src/imio/news/core/contents/newsfolder/content.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/configure.zcml` & `imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/content.py` & `imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/content.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/serializer.py` & `imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/serializer.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/view.pt` & `imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/view.pt`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/contents/newsitem/views.py` & `imio.news.core-1.2.8/src/imio/news/core/contents/newsitem/views.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/faceted/config/news.xml` & `imio.news.core-1.2.8/src/imio/news/core/faceted/config/news.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/indexers.py` & `imio.news.core-1.2.8/src/imio/news/core/indexers.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 @indexer(INewsItem)
 def translated_in_en(obj):
     return bool(obj.title_en)
 
 
 @indexer(INewsItem)
 def category_title(obj):
+    if obj.local_category is not None:
+        return obj.local_category
     if obj.category is not None:
         return translate_vocabulary_term(
             "imio.news.vocabulary.NewsCategories", obj.category
         )
 
 
 @indexer(INewsItem)
```

### Comparing `imio.news.core-1.2.7/src/imio/news/core/indexers.zcml` & `imio.news.core-1.2.8/src/imio/news/core/indexers.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/permissions.zcml` & `imio.news.core-1.2.8/src/imio/news/core/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/profiles/default/catalog.xml` & `imio.news.core-1.2.8/src/imio/news/core/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/profiles/default/contentrules.xml` & `imio.news.core-1.2.8/src/imio/news/core/profiles/default/contentrules.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/profiles/default/registry.xml` & `imio.news.core-1.2.8/src/imio/news/core/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/profiles/default/rolemap.xml` & `imio.news.core-1.2.8/src/imio/news/core/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.Entity.xml` & `imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.Entity.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.Folder.xml` & `imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml` & `imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.NewsFolder.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml` & `imio.news.core-1.2.8/src/imio/news/core/profiles/default/types/imio.news.NewsItem.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/profiles.zcml` & `imio.news.core-1.2.8/src/imio/news/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/serializer/newsitem.py` & `imio.news.core-1.2.8/src/imio/news/core/serializer/newsitem.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/setuphandlers.py` & `imio.news.core-1.2.8/src/imio/news/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/subscribers.py` & `imio.news.core-1.2.8/src/imio/news/core/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/subscribers.zcml` & `imio.news.core-1.2.8/src/imio/news/core/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/testing.py` & `imio.news.core-1.2.8/src/imio/news/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/resources/plone.png` & `imio.news.core-1.2.8/src/imio/news/core/tests/resources/plone.png`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/robot/test_example.robot` & `imio.news.core-1.2.8/src/imio/news/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_bring_news_into_news_folders.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_bring_news_into_news_folders.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_cropping.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_entity.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_indexer.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_local_roles.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_multilingual.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_multilingual.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_newsfolder.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_newsfolder.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_newsitem.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_newsitem.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,19 @@
         )
         news_item.category = "works"
         news_item.reindexObject()
         catalog = api.portal.get_tool("portal_catalog")
         brain = api.content.find(UID=news_item.UID())[0]
         indexes = catalog.getIndexDataForRID(brain.getRID())
         self.assertEqual(indexes.get("category_title"), "Travaux")
+        news_item.local_category = "Local category"
+        news_item.reindexObject()
+        brain = api.content.find(UID=news_item.UID())[0]
+        indexes = catalog.getIndexDataForRID(brain.getRID())
+        self.assertEqual(indexes.get("category_title"), "Local category")
 
     def test_referrer_newsfolders(self):
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         intids = getUtility(IIntIds)
         entity2 = api.content.create(
             container=self.portal,
             type="imio.news.Entity",
```

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_robot.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_setup.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_utils.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/tests/test_vocabularies.py` & `imio.news.core-1.2.8/src/imio/news/core/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/upgrades/configure.zcml` & `imio.news.core-1.2.8/src/imio/news/core/upgrades/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -138,8 +138,18 @@
       profile="imio.news.core:default">
     <genericsetup:upgradeDepends
         title="Add new permission to manager : imio.news.core.BringNewsIntoPersonnalNewsFolder"
         import_profile="imio.news.core.upgrades:upgrade_1009_to_1010"
         />
   </genericsetup:upgradeSteps>
 
+  <genericsetup:upgradeSteps
+      source="1010"
+      destination="1011"
+      profile="imio.news.core:default">
+    <genericsetup:upgradeStep
+        title="Reindex catalog for category_title (local category OR category)"
+        handler=".upgrades.reindex_catalog"
+        />
+  </genericsetup:upgradeSteps>
+
 </configure>
```

### Comparing `imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml` & `imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1003_to_1004/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml` & `imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1006_to_1007/contentrules.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml` & `imio.news.core-1.2.8/src/imio/news/core/upgrades/profiles/1007_to_1008/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/upgrades/upgrades.py` & `imio.news.core-1.2.8/src/imio/news/core/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/utils.py` & `imio.news.core-1.2.8/src/imio/news/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/viewlets/configure.zcml` & `imio.news.core-1.2.8/src/imio/news/core/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/viewlets/news.py` & `imio.news.core-1.2.8/src/imio/news/core/viewlets/news.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 
 from imio.news.core.contents import IEntity
-from imio.news.core.utils import get_entity_for_obj
 from plone import api
 from plone.app.layout.viewlets import common
 
 
 class BringNewsIntoNewsFoldersViewlet(common.ViewletBase):
 
     def available(self):
@@ -23,13 +22,13 @@
         return False
     has_permission = False
     brains = api.content.find(object_provides=IEntity.__identifier__)
     for brain in brains:
         entity = brain.getObject()
         if (
             api.user.get_permissions(user=user, obj=entity).get("Modify portal content")
-            == True
+            is True
         ):
             if entity.authorize_to_bring_news_anywhere:
                 has_permission = True
                 break
     return has_permission
```

### Comparing `imio.news.core-1.2.7/src/imio/news/core/vocabularies.py` & `imio.news.core-1.2.8/src/imio/news/core/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio/news/core/vocabularies.zcml` & `imio.news.core-1.2.8/src/imio/news/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.news.core-1.2.7/src/imio.news.core.egg-info/PKG-INFO` & `imio.news.core-1.2.8/src/imio.news.core.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: imio.news.core
-Version: 1.2.7
+Version: 1.2.8
 Summary: Core product for iMio news website
 Home-page: https://github.com/collective/imio.news.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.news.core
 Project-URL: Source, https://github.com/imio/imio.news.core
 Project-URL: Tracker, https://github.com/imio/imio.news.core/issues
 Keywords: Python Plone CMS
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -128,14 +129,21 @@
 - Christophe Boulanger, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.8 (2024-05-02)
+------------------
+
+- WEB-4101 : Use local category (if any) instead of category in `category_title` indexer
+  [laulaz]
+
+
 1.2.7 (2024-04-04)
 ------------------
 
 - Fix : serializer and message "At least one of these parameters must be supplied: path, UID"
   [boulch]
 
 
@@ -305,7 +313,9 @@
 
 
 1.0a1 (2022-01-25)
 ------------------
 
 - Initial release.
   [boulch]
+
+
```

### Comparing `imio.news.core-1.2.7/src/imio.news.core.egg-info/SOURCES.txt` & `imio.news.core-1.2.8/src/imio.news.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

