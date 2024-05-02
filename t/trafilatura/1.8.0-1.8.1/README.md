# Comparing `tmp/trafilatura-1.8.0.tar.gz` & `tmp/trafilatura-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trafilatura-1.8.0.tar", last modified: Wed Mar 20 15:19:58 2024, max compression
+gzip compressed data, was "trafilatura-1.8.1.tar", last modified: Wed Apr  3 11:42:46 2024, max compression
```

## Comparing `trafilatura-1.8.0.tar` & `trafilatura-1.8.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-03-20 15:19:58.928766 trafilatura-1.8.0/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      796 2021-11-18 18:20:49.000000 trafilatura-1.8.0/CITATION.cff
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     2129 2024-01-08 12:50:38.000000 trafilatura-1.8.0/CONTRIBUTING.md
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    12926 2024-03-20 15:18:39.000000 trafilatura-1.8.0/HISTORY.md
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    10173 2024-03-20 15:18:48.000000 trafilatura-1.8.0/LICENSE
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      489 2022-03-07 11:15:49.000000 trafilatura-1.8.0/MANIFEST.in
--rw-r--r--   0 adbar     (1001) adbar     (1005)    14943 2024-03-20 15:19:58.928766 trafilatura-1.8.0/PKG-INFO
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    11790 2024-03-20 15:18:48.000000 trafilatura-1.8.0/README.rst
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-03-20 15:19:58.904766 trafilatura-1.8.0/docs/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      634 2019-12-24 15:36:05.000000 trafilatura-1.8.0/docs/Makefile
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-03-20 15:19:58.896766 trafilatura-1.8.0/docs/_build/
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-03-20 15:19:58.912766 trafilatura-1.8.0/docs/_build/_images/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)   140162 2020-06-17 16:47:44.000000 trafilatura-1.8.0/docs/_build/_images/dwds-count-exportieren.jpg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)   108871 2020-06-17 16:47:44.000000 trafilatura-1.8.0/docs/_build/_images/dwds-exportieren.jpg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)   171519 2020-06-17 16:47:44.000000 trafilatura-1.8.0/docs/_build/_images/dwds-treffer-exportieren.jpg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    75098 2021-01-08 16:52:37.000000 trafilatura-1.8.0/docs/_build/_images/gui-screenshot.png
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    96837 2021-09-16 16:27:51.000000 trafilatura-1.8.0/docs/_build/_images/software-ecosystem.png
--rw-rw-r--   0 adbar     (1001) adbar     (1005)   816558 2020-01-17 15:42:23.000000 trafilatura-1.8.0/docs/_build/_images/trafilatura-demo.gif
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-03-20 15:19:58.916766 trafilatura-1.8.0/docs/_build/_static/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      286 2023-11-29 13:26:25.000000 trafilatura-1.8.0/docs/_build/_static/file.png
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       90 2023-11-29 13:26:25.000000 trafilatura-1.8.0/docs/_build/_static/minus.png
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       90 2023-11-29 13:26:25.000000 trafilatura-1.8.0/docs/_build/_static/plus.png
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    23420 2022-01-25 15:28:24.000000 trafilatura-1.8.0/docs/_build/_static/trafilatura-logo.png
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      285 2022-01-28 19:17:06.000000 trafilatura-1.8.0/docs/background.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    24721 2023-04-13 12:18:08.000000 trafilatura-1.8.0/docs/compendium.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     4385 2024-01-08 14:28:11.000000 trafilatura-1.8.0/docs/conf.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     1822 2024-01-25 12:45:59.000000 trafilatura-1.8.0/docs/corefunctions.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     3407 2022-01-13 18:52:09.000000 trafilatura-1.8.0/docs/corpus-data.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     8180 2024-01-08 12:50:38.000000 trafilatura-1.8.0/docs/crawls.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    10317 2024-01-25 12:45:59.000000 trafilatura-1.8.0/docs/downloads.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)   140162 2020-06-17 16:47:44.000000 trafilatura-1.8.0/docs/dwds-count-exportieren.jpg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)   108871 2020-06-17 16:47:44.000000 trafilatura-1.8.0/docs/dwds-exportieren.jpg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)   171519 2020-06-17 16:47:44.000000 trafilatura-1.8.0/docs/dwds-treffer-exportieren.jpg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    16498 2024-02-27 12:25:00.000000 trafilatura-1.8.0/docs/evaluation.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    75098 2021-01-08 16:52:37.000000 trafilatura-1.8.0/docs/gui-screenshot.png
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     9504 2024-03-20 15:18:48.000000 trafilatura-1.8.0/docs/index.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     2740 2021-11-29 16:07:30.000000 trafilatura-1.8.0/docs/installation-gui.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     5972 2024-01-08 12:50:38.000000 trafilatura-1.8.0/docs/installation.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      795 2019-12-24 15:36:05.000000 trafilatura-1.8.0/docs/make.bat
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     2608 2024-01-08 12:50:38.000000 trafilatura-1.8.0/docs/quickstart.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      139 2024-01-25 12:45:59.000000 trafilatura-1.8.0/docs/requirements.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     5735 2024-01-08 12:50:38.000000 trafilatura-1.8.0/docs/settings.rst
--rw-------   0 adbar     (1001) adbar     (1005)    96837 2021-09-16 16:27:51.000000 trafilatura-1.8.0/docs/software-ecosystem.png
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    10299 2024-02-27 12:25:00.000000 trafilatura-1.8.0/docs/sources.rst
--rw-r--r--   0 adbar     (1001) adbar     (1005)   816558 2020-01-17 15:42:23.000000 trafilatura-1.8.0/docs/trafilatura-demo.gif
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    23420 2022-01-25 15:28:24.000000 trafilatura-1.8.0/docs/trafilatura-logo.png
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     5033 2024-03-14 16:03:48.000000 trafilatura-1.8.0/docs/troubleshooting.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     7978 2023-11-08 15:59:34.000000 trafilatura-1.8.0/docs/tutorial-dwds.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     5416 2024-02-27 12:25:00.000000 trafilatura-1.8.0/docs/tutorial-epsilla.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    10881 2023-11-08 15:59:34.000000 trafilatura-1.8.0/docs/tutorial0.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     4662 2023-11-08 15:59:34.000000 trafilatura-1.8.0/docs/tutorial1.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     1447 2023-04-13 12:18:08.000000 trafilatura-1.8.0/docs/tutorial2.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     2668 2024-02-27 12:25:00.000000 trafilatura-1.8.0/docs/tutorials.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     3782 2023-11-03 16:02:12.000000 trafilatura-1.8.0/docs/url-management.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     2031 2024-02-27 12:25:00.000000 trafilatura-1.8.0/docs/usage-api.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    15049 2024-02-27 12:25:00.000000 trafilatura-1.8.0/docs/usage-cli.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      835 2024-02-27 12:25:00.000000 trafilatura-1.8.0/docs/usage-gui.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    14853 2024-02-27 12:25:00.000000 trafilatura-1.8.0/docs/usage-python.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     5697 2024-02-27 12:25:00.000000 trafilatura-1.8.0/docs/usage-r.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      196 2024-01-25 12:45:59.000000 trafilatura-1.8.0/docs/usage.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    16864 2024-02-27 12:25:00.000000 trafilatura-1.8.0/docs/used-by.rst
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       40 2021-11-15 14:02:12.000000 trafilatura-1.8.0/pytest.ini
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       38 2024-03-20 15:19:58.928766 trafilatura-1.8.0/setup.cfg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     4718 2024-03-20 15:18:48.000000 trafilatura-1.8.0/setup.py
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-03-20 15:19:58.920766 trafilatura-1.8.0/tests/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       84 2023-08-18 16:12:07.000000 trafilatura-1.8.0/tests/__init__.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    20146 2024-01-24 17:14:34.000000 trafilatura-1.8.0/tests/cli_tests.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     9187 2024-02-27 12:25:00.000000 trafilatura-1.8.0/tests/downloads_tests.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     9699 2023-12-15 15:05:15.000000 trafilatura-1.8.0/tests/feeds_tests.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     9834 2023-10-04 12:59:20.000000 trafilatura-1.8.0/tests/filters_tests.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     1925 2023-08-18 16:12:07.000000 trafilatura-1.8.0/tests/hashing_tests.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    70093 2023-08-18 16:12:07.000000 trafilatura-1.8.0/tests/json_metadata_tests.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    24025 2023-11-28 12:44:32.000000 trafilatura-1.8.0/tests/metadata_tests.py
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-03-20 15:19:58.920766 trafilatura-1.8.0/tests/resources/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     7490 2021-11-08 11:56:03.000000 trafilatura-1.8.0/tests/resources/apache.html
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      416 2019-12-24 15:36:05.000000 trafilatura-1.8.0/tests/resources/exotic_tags.html
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      444 2019-12-24 15:36:05.000000 trafilatura-1.8.0/tests/resources/exotic_tags_tei.html
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    34299 2021-10-29 16:43:41.000000 trafilatura-1.8.0/tests/resources/feed.json
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      823 2020-12-22 14:28:05.000000 trafilatura-1.8.0/tests/resources/feed1.atom
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      668 2021-01-21 13:30:47.000000 trafilatura-1.8.0/tests/resources/feed2.rss
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     4148 2023-01-04 17:43:29.000000 trafilatura-1.8.0/tests/resources/http_sample.html
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     3741 2019-12-24 15:36:05.000000 trafilatura-1.8.0/tests/resources/httpbin_sample.html
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       93 2023-05-11 19:41:09.000000 trafilatura-1.8.0/tests/resources/list-discard.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       94 2023-05-11 19:41:09.000000 trafilatura-1.8.0/tests/resources/list-process.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      741 2023-10-24 14:50:14.000000 trafilatura-1.8.0/tests/resources/newsettings.cfg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      154 2021-10-27 16:32:31.000000 trafilatura-1.8.0/tests/resources/redundant-urls.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    38705 2021-12-08 16:43:57.000000 trafilatura-1.8.0/tests/resources/scam.html
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     2056 2020-12-22 16:53:15.000000 trafilatura-1.8.0/tests/resources/sitemap-hreflang.xml
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     8622 2020-09-25 15:03:42.000000 trafilatura-1.8.0/tests/resources/sitemap.xml
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      494 2020-11-27 17:14:37.000000 trafilatura-1.8.0/tests/resources/sitemap.xml.gz
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      397 2021-01-21 13:31:13.000000 trafilatura-1.8.0/tests/resources/sitemap2.xml
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    14388 2023-05-11 19:41:09.000000 trafilatura-1.8.0/tests/resources/utf8.html
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    23220 2021-10-27 11:17:58.000000 trafilatura-1.8.0/tests/resources/webpage.html.gz
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      725 2024-01-24 17:14:34.000000 trafilatura-1.8.0/tests/resources/zerolength.cfg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     8437 2024-02-27 12:25:00.000000 trafilatura-1.8.0/tests/sitemaps_tests.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     7725 2023-12-13 12:15:25.000000 trafilatura-1.8.0/tests/spider_tests.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    66606 2024-03-07 16:12:21.000000 trafilatura-1.8.0/tests/unit_tests.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    20324 2024-01-24 17:14:34.000000 trafilatura-1.8.0/tests/xml_tei_tests.py
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-03-20 15:19:58.924766 trafilatura-1.8.0/trafilatura/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      608 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/__init__.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    13288 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/cli.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    16486 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/cli_utils.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    49989 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/core.py
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-03-20 15:19:58.928766 trafilatura-1.8.0/trafilatura/data/
--rw-rw-r--   0 adbar     (1001) adbar     (1005)   851312 2022-08-02 16:32:41.000000 trafilatura-1.8.0/trafilatura/data/jt-stopwords-pickle.lzma
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    80692 2022-08-02 16:32:41.000000 trafilatura-1.8.0/trafilatura/data/tei-schema-pickle.lzma
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    14538 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/downloads.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     5014 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/external.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     9664 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/feeds.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     4917 2024-01-22 11:54:58.000000 trafilatura-1.8.0/trafilatura/filters.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     8103 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/gui.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     4876 2023-08-18 16:12:07.000000 trafilatura-1.8.0/trafilatura/hashing.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    13349 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/htmlprocessing.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     9844 2023-08-18 16:12:07.000000 trafilatura-1.8.0/trafilatura/json_metadata.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     3671 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/lru.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      951 2023-08-18 16:12:07.000000 trafilatura-1.8.0/trafilatura/meta.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    21929 2024-02-27 12:25:00.000000 trafilatura-1.8.0/trafilatura/metadata.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     4359 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/metaxpaths.py
--rwxrwxr-x   0 adbar     (1001) adbar     (1005)    17877 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/readability_lxml.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      739 2024-02-05 15:30:45.000000 trafilatura-1.8.0/trafilatura/settings.cfg
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     3130 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/settings.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     9766 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/sitemaps.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     9013 2023-08-18 16:12:07.000000 trafilatura-1.8.0/trafilatura/spider.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    15998 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/utils.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    21430 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/xml.py
--rw-rw-r--   0 adbar     (1001) adbar     (1005)    11564 2024-03-20 15:18:48.000000 trafilatura-1.8.0/trafilatura/xpaths.py
-drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-03-20 15:19:58.928766 trafilatura-1.8.0/trafilatura.egg-info/
--rw-r--r--   0 adbar     (1001) adbar     (1005)    14943 2024-03-20 15:19:58.000000 trafilatura-1.8.0/trafilatura.egg-info/PKG-INFO
--rw-rw-r--   0 adbar     (1001) adbar     (1005)     3075 2024-03-20 15:19:58.000000 trafilatura-1.8.0/trafilatura.egg-info/SOURCES.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)        1 2024-03-20 15:19:58.000000 trafilatura-1.8.0/trafilatura.egg-info/dependency_links.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       92 2024-03-20 15:19:58.000000 trafilatura-1.8.0/trafilatura.egg-info/entry_points.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)        1 2023-10-04 13:27:10.000000 trafilatura-1.8.0/trafilatura.egg-info/not-zip-safe
--rw-rw-r--   0 adbar     (1001) adbar     (1005)      577 2024-03-20 15:19:58.000000 trafilatura-1.8.0/trafilatura.egg-info/requires.txt
--rw-rw-r--   0 adbar     (1001) adbar     (1005)       12 2024-03-20 15:19:58.000000 trafilatura-1.8.0/trafilatura.egg-info/top_level.txt
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.360365 trafilatura-1.8.1/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      796 2021-11-18 18:20:49.000000 trafilatura-1.8.1/CITATION.cff
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2129 2024-01-08 12:50:38.000000 trafilatura-1.8.1/CONTRIBUTING.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    13253 2024-04-03 11:38:12.000000 trafilatura-1.8.1/HISTORY.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    10173 2024-03-20 15:18:48.000000 trafilatura-1.8.1/LICENSE
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      489 2022-03-07 11:15:49.000000 trafilatura-1.8.1/MANIFEST.in
+-rw-r--r--   0 adbar     (1000) adbar     (1000)    14947 2024-04-03 11:42:46.360365 trafilatura-1.8.1/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    11790 2024-03-20 15:18:48.000000 trafilatura-1.8.1/README.rst
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.352360 trafilatura-1.8.1/docs/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      634 2019-12-24 15:36:05.000000 trafilatura-1.8.1/docs/Makefile
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.348357 trafilatura-1.8.1/docs/_build/
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.352360 trafilatura-1.8.1/docs/_build/_images/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   140162 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/_build/_images/dwds-count-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   108871 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/_build/_images/dwds-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   171519 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/_build/_images/dwds-treffer-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    75098 2021-01-08 16:52:37.000000 trafilatura-1.8.1/docs/_build/_images/gui-screenshot.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    96837 2021-09-16 16:27:51.000000 trafilatura-1.8.1/docs/_build/_images/software-ecosystem.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   816558 2020-01-17 15:42:23.000000 trafilatura-1.8.1/docs/_build/_images/trafilatura-demo.gif
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.352360 trafilatura-1.8.1/docs/_build/_static/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      286 2023-11-29 13:26:25.000000 trafilatura-1.8.1/docs/_build/_static/file.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       90 2023-11-29 13:26:25.000000 trafilatura-1.8.1/docs/_build/_static/minus.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       90 2023-11-29 13:26:25.000000 trafilatura-1.8.1/docs/_build/_static/plus.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    23420 2022-01-25 15:28:24.000000 trafilatura-1.8.1/docs/_build/_static/trafilatura-logo.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      285 2022-01-28 19:17:06.000000 trafilatura-1.8.1/docs/background.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    24721 2023-04-13 12:18:08.000000 trafilatura-1.8.1/docs/compendium.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4385 2024-01-08 14:28:11.000000 trafilatura-1.8.1/docs/conf.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1822 2024-01-25 12:45:59.000000 trafilatura-1.8.1/docs/corefunctions.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3407 2022-01-13 18:52:09.000000 trafilatura-1.8.1/docs/corpus-data.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8180 2024-01-08 12:50:38.000000 trafilatura-1.8.1/docs/crawls.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    10317 2024-01-25 12:45:59.000000 trafilatura-1.8.1/docs/downloads.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   140162 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/dwds-count-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   108871 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/dwds-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   171519 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/dwds-treffer-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16498 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/evaluation.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    75098 2021-01-08 16:52:37.000000 trafilatura-1.8.1/docs/gui-screenshot.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9504 2024-03-20 15:18:48.000000 trafilatura-1.8.1/docs/index.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2740 2021-11-29 16:07:30.000000 trafilatura-1.8.1/docs/installation-gui.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5972 2024-01-08 12:50:38.000000 trafilatura-1.8.1/docs/installation.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      795 2019-12-24 15:36:05.000000 trafilatura-1.8.1/docs/make.bat
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2608 2024-01-08 12:50:38.000000 trafilatura-1.8.1/docs/quickstart.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      139 2024-01-25 12:45:59.000000 trafilatura-1.8.1/docs/requirements.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5735 2024-01-08 12:50:38.000000 trafilatura-1.8.1/docs/settings.rst
+-rw-------   0 adbar     (1000) adbar     (1000)    96837 2021-09-16 16:27:51.000000 trafilatura-1.8.1/docs/software-ecosystem.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    10299 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/sources.rst
+-rw-r--r--   0 adbar     (1000) adbar     (1000)   816558 2020-01-17 15:42:23.000000 trafilatura-1.8.1/docs/trafilatura-demo.gif
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    23420 2022-01-25 15:28:24.000000 trafilatura-1.8.1/docs/trafilatura-logo.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4975 2024-03-25 12:40:36.000000 trafilatura-1.8.1/docs/troubleshooting.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7978 2023-11-08 15:59:34.000000 trafilatura-1.8.1/docs/tutorial-dwds.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5416 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/tutorial-epsilla.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    10881 2023-11-08 15:59:34.000000 trafilatura-1.8.1/docs/tutorial0.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4662 2023-11-08 15:59:34.000000 trafilatura-1.8.1/docs/tutorial1.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1447 2023-04-13 12:18:08.000000 trafilatura-1.8.1/docs/tutorial2.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2668 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/tutorials.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3782 2023-11-03 16:02:12.000000 trafilatura-1.8.1/docs/url-management.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2031 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/usage-api.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    15049 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/usage-cli.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      835 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/usage-gui.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    14853 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/usage-python.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5697 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/usage-r.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      196 2024-01-25 12:45:59.000000 trafilatura-1.8.1/docs/usage.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16864 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/used-by.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-11-15 14:02:12.000000 trafilatura-1.8.1/pytest.ini
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2024-04-03 11:42:46.360365 trafilatura-1.8.1/setup.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4722 2024-04-02 17:40:04.000000 trafilatura-1.8.1/setup.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.352360 trafilatura-1.8.1/tests/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       84 2023-08-18 16:12:07.000000 trafilatura-1.8.1/tests/__init__.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    20146 2024-01-24 17:14:34.000000 trafilatura-1.8.1/tests/cli_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9187 2024-02-27 12:25:00.000000 trafilatura-1.8.1/tests/downloads_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9699 2023-12-15 15:05:15.000000 trafilatura-1.8.1/tests/feeds_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9834 2023-10-04 12:59:20.000000 trafilatura-1.8.1/tests/filters_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1925 2023-08-18 16:12:07.000000 trafilatura-1.8.1/tests/hashing_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    70093 2023-08-18 16:12:07.000000 trafilatura-1.8.1/tests/json_metadata_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    24025 2023-11-28 12:44:32.000000 trafilatura-1.8.1/tests/metadata_tests.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.356362 trafilatura-1.8.1/tests/resources/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7490 2021-11-08 11:56:03.000000 trafilatura-1.8.1/tests/resources/apache.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      416 2019-12-24 15:36:05.000000 trafilatura-1.8.1/tests/resources/exotic_tags.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      444 2019-12-24 15:36:05.000000 trafilatura-1.8.1/tests/resources/exotic_tags_tei.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    34299 2021-10-29 16:43:41.000000 trafilatura-1.8.1/tests/resources/feed.json
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      823 2020-12-22 14:28:05.000000 trafilatura-1.8.1/tests/resources/feed1.atom
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      668 2021-01-21 13:30:47.000000 trafilatura-1.8.1/tests/resources/feed2.rss
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4148 2023-01-04 17:43:29.000000 trafilatura-1.8.1/tests/resources/http_sample.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3741 2019-12-24 15:36:05.000000 trafilatura-1.8.1/tests/resources/httpbin_sample.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       93 2023-05-11 19:41:09.000000 trafilatura-1.8.1/tests/resources/list-discard.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       94 2023-05-11 19:41:09.000000 trafilatura-1.8.1/tests/resources/list-process.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      741 2023-10-24 14:50:14.000000 trafilatura-1.8.1/tests/resources/newsettings.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      154 2021-10-27 16:32:31.000000 trafilatura-1.8.1/tests/resources/redundant-urls.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    38705 2021-12-08 16:43:57.000000 trafilatura-1.8.1/tests/resources/scam.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2056 2020-12-22 16:53:15.000000 trafilatura-1.8.1/tests/resources/sitemap-hreflang.xml
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8622 2020-09-25 15:03:42.000000 trafilatura-1.8.1/tests/resources/sitemap.xml
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      494 2020-11-27 17:14:37.000000 trafilatura-1.8.1/tests/resources/sitemap.xml.gz
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      397 2021-01-21 13:31:13.000000 trafilatura-1.8.1/tests/resources/sitemap2.xml
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    14388 2023-05-11 19:41:09.000000 trafilatura-1.8.1/tests/resources/utf8.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    23220 2021-10-27 11:17:58.000000 trafilatura-1.8.1/tests/resources/webpage.html.gz
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      725 2024-01-24 17:14:34.000000 trafilatura-1.8.1/tests/resources/zerolength.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8437 2024-02-27 12:25:00.000000 trafilatura-1.8.1/tests/sitemaps_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7725 2023-12-13 12:15:25.000000 trafilatura-1.8.1/tests/spider_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    67941 2024-04-02 17:40:04.000000 trafilatura-1.8.1/tests/unit_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    20324 2024-01-24 17:14:34.000000 trafilatura-1.8.1/tests/xml_tei_tests.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.356362 trafilatura-1.8.1/trafilatura/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      608 2024-04-03 11:38:59.000000 trafilatura-1.8.1/trafilatura/__init__.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    13288 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/cli.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16486 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/cli_utils.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    50196 2024-04-02 17:55:15.000000 trafilatura-1.8.1/trafilatura/core.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.360365 trafilatura-1.8.1/trafilatura/data/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   851312 2022-08-02 16:32:41.000000 trafilatura-1.8.1/trafilatura/data/jt-stopwords-pickle.lzma
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    80692 2022-08-02 16:32:41.000000 trafilatura-1.8.1/trafilatura/data/tei-schema-pickle.lzma
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    14538 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/downloads.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4943 2024-04-03 06:16:54.000000 trafilatura-1.8.1/trafilatura/external.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9664 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/feeds.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4917 2024-01-22 11:54:58.000000 trafilatura-1.8.1/trafilatura/filters.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8103 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/gui.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4876 2023-08-18 16:12:07.000000 trafilatura-1.8.1/trafilatura/hashing.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    13435 2024-04-02 17:40:04.000000 trafilatura-1.8.1/trafilatura/htmlprocessing.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9844 2023-08-18 16:12:07.000000 trafilatura-1.8.1/trafilatura/json_metadata.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3671 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/lru.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      951 2023-08-18 16:12:07.000000 trafilatura-1.8.1/trafilatura/meta.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    21929 2024-02-27 12:25:00.000000 trafilatura-1.8.1/trafilatura/metadata.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4359 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/metaxpaths.py
+-rwxrwxr-x   0 adbar     (1000) adbar     (1000)    17877 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/readability_lxml.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      739 2024-02-05 15:30:45.000000 trafilatura-1.8.1/trafilatura/settings.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3130 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/settings.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9766 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/sitemaps.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9013 2023-08-18 16:12:07.000000 trafilatura-1.8.1/trafilatura/spider.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16004 2024-03-28 17:14:38.000000 trafilatura-1.8.1/trafilatura/utils.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    21940 2024-03-28 17:14:38.000000 trafilatura-1.8.1/trafilatura/xml.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    11775 2024-04-03 11:34:41.000000 trafilatura-1.8.1/trafilatura/xpaths.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.360365 trafilatura-1.8.1/trafilatura.egg-info/
+-rw-r--r--   0 adbar     (1000) adbar     (1000)    14947 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3075 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/SOURCES.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/dependency_links.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       92 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/entry_points.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/not-zip-safe
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      581 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/requires.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       12 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/top_level.txt
```

### Comparing `trafilatura-1.8.0/CITATION.cff` & `trafilatura-1.8.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/CONTRIBUTING.md` & `trafilatura-1.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/HISTORY.md` & `trafilatura-1.8.1/HISTORY.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 ## History / Changelog
 
 
+### 1.8.1
+
+Maintenance:
+- Pin LXML to prevent broken dependency (#535)
+
+Extraction:
+- Improve extraction accuracy for major news outlets (#530)
+- Fix formatting by correcting order of element generation and space handling with @dlwh (#528)
+- Fix: prevent tail insertion before children in nested elements by @knit-bee (#536)
+
+
 ### 1.8.0
 
 Extraction:
 - Better precision by @felipehertzer (#509, #520)
 - Code formatting in TXT/Markdown output added (#498)
 - Improved CSV output (#496)
 - LXML: compile XPath expressions (#504)
```

### Comparing `trafilatura-1.8.0/LICENSE` & `trafilatura-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/PKG-INFO` & `trafilatura-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trafilatura
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python package and command-line tool designed to gather text on the Web, includes all necessary discovery and text processing components to perform web crawling, downloads, scraping, and extraction of main texts, metadata and comments.
 Home-page: https://trafilatura.readthedocs.io
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: Apache-2.0
 Project-URL: Documentation, https://trafilatura.readthedocs.io
 Project-URL: Source, https://github.com/adbar/trafilatura
@@ -44,15 +44,15 @@
 Requires-Dist: charset_normalizer>=3.0.1; python_version < "3.7"
 Requires-Dist: charset_normalizer>=3.2.0; python_version >= "3.7"
 Requires-Dist: courlan>=1.0.0
 Requires-Dist: htmldate>=1.8.0
 Requires-Dist: importlib_metadata; python_version < "3.8"
 Requires-Dist: justext>=3.0.0
 Requires-Dist: lxml==4.9.2; platform_system == "Darwin" and python_version <= "3.8"
-Requires-Dist: lxml<6,>=4.9.4; platform_system != "Darwin" or python_version > "3.8"
+Requires-Dist: lxml<5.2.0,>=4.9.4; platform_system != "Darwin" or python_version > "3.8"
 Requires-Dist: urllib3<2,>=1.26; python_version < "3.7"
 Requires-Dist: urllib3<3,>=1.26; python_version >= "3.7"
 Provides-Extra: all
 Requires-Dist: brotli; extra == "all"
 Requires-Dist: cchardet>=2.1.7; python_version < "3.11" and extra == "all"
 Requires-Dist: faust-cchardet>=2.1.19; python_version >= "3.11" and extra == "all"
 Requires-Dist: htmldate[speed]>=1.8.0; extra == "all"
```

### Comparing `trafilatura-1.8.0/README.rst` & `trafilatura-1.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/Makefile` & `trafilatura-1.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/_build/_images/dwds-count-exportieren.jpg` & `trafilatura-1.8.1/docs/_build/_images/dwds-count-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/_build/_images/dwds-exportieren.jpg` & `trafilatura-1.8.1/docs/_build/_images/dwds-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/_build/_images/dwds-treffer-exportieren.jpg` & `trafilatura-1.8.1/docs/_build/_images/dwds-treffer-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/_build/_images/gui-screenshot.png` & `trafilatura-1.8.1/docs/_build/_images/gui-screenshot.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/_build/_images/software-ecosystem.png` & `trafilatura-1.8.1/docs/_build/_images/software-ecosystem.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/_build/_images/trafilatura-demo.gif` & `trafilatura-1.8.1/docs/_build/_images/trafilatura-demo.gif`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/_build/_static/trafilatura-logo.png` & `trafilatura-1.8.1/docs/_build/_static/trafilatura-logo.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/compendium.rst` & `trafilatura-1.8.1/docs/compendium.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/conf.py` & `trafilatura-1.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/corefunctions.rst` & `trafilatura-1.8.1/docs/corefunctions.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/corpus-data.rst` & `trafilatura-1.8.1/docs/corpus-data.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/crawls.rst` & `trafilatura-1.8.1/docs/crawls.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/downloads.rst` & `trafilatura-1.8.1/docs/downloads.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/dwds-count-exportieren.jpg` & `trafilatura-1.8.1/docs/dwds-count-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/dwds-exportieren.jpg` & `trafilatura-1.8.1/docs/dwds-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/dwds-treffer-exportieren.jpg` & `trafilatura-1.8.1/docs/dwds-treffer-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/evaluation.rst` & `trafilatura-1.8.1/docs/evaluation.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/gui-screenshot.png` & `trafilatura-1.8.1/docs/gui-screenshot.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/index.rst` & `trafilatura-1.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/installation-gui.rst` & `trafilatura-1.8.1/docs/installation-gui.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/installation.rst` & `trafilatura-1.8.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/make.bat` & `trafilatura-1.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/quickstart.rst` & `trafilatura-1.8.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/settings.rst` & `trafilatura-1.8.1/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/software-ecosystem.png` & `trafilatura-1.8.1/docs/software-ecosystem.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/sources.rst` & `trafilatura-1.8.1/docs/sources.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/trafilatura-demo.gif` & `trafilatura-1.8.1/docs/trafilatura-demo.gif`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/trafilatura-logo.png` & `trafilatura-1.8.1/docs/trafilatura-logo.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/troubleshooting.rst` & `trafilatura-1.8.1/docs/troubleshooting.rst`

 * *Files 5% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 
 The extractor uses several fallbacks to make sure enough text is returned. Content extraction is a tradeoff between precision and recall, that is between desired and undesirable content. Being ready to accept more unwanted text makes it easier to gather more of the relevant text in the output. Here are ways to tackle the issue:
 
 - Opting for ``favor_recall`` (Python) or ``--recall`` (CLI)
 - Changing the minimum acceptable length in the settings
 - Using the more basic `baseline <corefunctions.html#baseline>`_ or `html2txt <corefunctions.html#html2txt>`_ functions instead (which is also faster)
 
-(see also `reported issues with The New Yorker <https://github.com/adbar/trafilatura/issues?q=is%3Aissue+newyorker>`_)
-
 
 Beyond raw HTML
 ^^^^^^^^^^^^^^^
 
 While downloading and processing raw HTML documents is much faster, it can be necessary to fully render the web page before further processing, e.g. because a page makes exhaustive use of JavaScript or because content is injected from multiple sources.
 
 In such cases the way to go is to use a browser automation library like `Playwright <https://playwright.dev/python/>`_. For available alternatives see this `list of headless browsers <https://github.com/dhamaniasad/HeadlessBrowsers>`_.
 
-For more refined masking and automation methods, see the `nodriver package <https://github.com/ultrafunkamsterdam/nodriver>`_.
+For more refined masking and automation methods, see the `nodriver <https://github.com/ultrafunkamsterdam/nodriver>`_ and `browserforge <https://github.com/daijro/browserforge>`_ packages.
 
 
 
 Bypassing paywalls
 ^^^^^^^^^^^^^^^^^^
 
 A browser automation library can also be useful to bypass issues related to cookies and paywalls as it can be combined with a corresponding browser extension, e.g. `iamdamdev's bypass-paywalls-chrome <https://github.com/iamadamdev/bypass-paywalls-chrome>`_ or `this alternative by magnolia1234 <https://gitlab.com/magnolia1234/bypass-paywalls-chrome-clean>`_.
```

### Comparing `trafilatura-1.8.0/docs/tutorial-dwds.rst` & `trafilatura-1.8.1/docs/tutorial-dwds.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/tutorial-epsilla.rst` & `trafilatura-1.8.1/docs/tutorial-epsilla.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/tutorial0.rst` & `trafilatura-1.8.1/docs/tutorial0.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/tutorial1.rst` & `trafilatura-1.8.1/docs/tutorial1.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/tutorial2.rst` & `trafilatura-1.8.1/docs/tutorial2.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/tutorials.rst` & `trafilatura-1.8.1/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/url-management.rst` & `trafilatura-1.8.1/docs/url-management.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/usage-api.rst` & `trafilatura-1.8.1/docs/usage-api.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/usage-cli.rst` & `trafilatura-1.8.1/docs/usage-cli.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/usage-gui.rst` & `trafilatura-1.8.1/docs/usage-gui.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/usage-python.rst` & `trafilatura-1.8.1/docs/usage-python.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/usage-r.rst` & `trafilatura-1.8.1/docs/usage-r.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/docs/used-by.rst` & `trafilatura-1.8.1/docs/used-by.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/setup.py` & `trafilatura-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         "charset_normalizer >= 3.2.0; python_version >= '3.7'",
         "courlan >= 1.0.0",
         "htmldate >= 1.8.0",
         "importlib_metadata; python_version < '3.8'",
         "justext >= 3.0.0",
         # see tests on Github Actions
         "lxml == 4.9.2 ; platform_system == 'Darwin' and python_version <= '3.8'",
-        "lxml >= 4.9.4, < 6; platform_system != 'Darwin' or python_version > '3.8'",
+        "lxml >= 4.9.4, < 5.2.0; platform_system != 'Darwin' or python_version > '3.8'",
         "urllib3 >= 1.26, < 2; python_version < '3.7'",
         "urllib3 >= 1.26, < 3; python_version >= '3.7'",
     ],
     extras_require=extras,
     entry_points={
         "console_scripts": [
             "trafilatura=trafilatura.cli:main",
```

### Comparing `trafilatura-1.8.0/tests/cli_tests.py` & `trafilatura-1.8.1/tests/cli_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/downloads_tests.py` & `trafilatura-1.8.1/tests/downloads_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/feeds_tests.py` & `trafilatura-1.8.1/tests/feeds_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/filters_tests.py` & `trafilatura-1.8.1/tests/filters_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/hashing_tests.py` & `trafilatura-1.8.1/tests/hashing_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/json_metadata_tests.py` & `trafilatura-1.8.1/tests/json_metadata_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/metadata_tests.py` & `trafilatura-1.8.1/tests/metadata_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/apache.html` & `trafilatura-1.8.1/tests/resources/apache.html`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/feed.json` & `trafilatura-1.8.1/tests/resources/feed.json`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/feed1.atom` & `trafilatura-1.8.1/tests/resources/feed1.atom`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/feed2.rss` & `trafilatura-1.8.1/tests/resources/feed2.rss`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/http_sample.html` & `trafilatura-1.8.1/tests/resources/http_sample.html`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/httpbin_sample.html` & `trafilatura-1.8.1/tests/resources/httpbin_sample.html`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/newsettings.cfg` & `trafilatura-1.8.1/tests/resources/newsettings.cfg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/scam.html` & `trafilatura-1.8.1/tests/resources/scam.html`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/sitemap-hreflang.xml` & `trafilatura-1.8.1/tests/resources/sitemap-hreflang.xml`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/sitemap.xml` & `trafilatura-1.8.1/tests/resources/sitemap.xml`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/utf8.html` & `trafilatura-1.8.1/tests/resources/utf8.html`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/webpage.html.gz` & `trafilatura-1.8.1/tests/resources/webpage.html.gz`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/resources/zerolength.cfg` & `trafilatura-1.8.1/tests/resources/zerolength.cfg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/sitemaps_tests.py` & `trafilatura-1.8.1/tests/sitemaps_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/spider_tests.py` & `trafilatura-1.8.1/tests/spider_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/tests/unit_tests.py` & `trafilatura-1.8.1/tests/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,16 +349,21 @@
     my_document = html.fromstring('<html><body><article><ul><li>Number 1</li><li>Number <a href="test.html">2</a></li><li>Number 3</li><p>Test</p></article></body></html>')
     my_result = extract(my_document, output_format='xml', include_links=True, config=ZERO_CONFIG)
     assert '<item>Number <ref target="test.html">2</ref></item>' in my_result
 
     # XML and Markdown formatting within <p>-tag
     my_document = html.fromstring('<html><body><p><b>bold</b>, <i>italics</i>, <tt>tt</tt>, <strike>deleted</strike>, <u>underlined</u>, <a href="test.html">link</a> and additional text to bypass detection.</p></body></html>')
     my_result = extract(copy(my_document), no_fallback=True, include_formatting=False, config=ZERO_CONFIG)
-    # TXT: newline problem here
-    assert my_result == 'bold, italics, tt,\ndeleted, underlined, link and additional text to bypass detection.'
+    assert my_result == 'bold, italics, tt, deleted, underlined, link and additional text to bypass detection.'
+
+    my_result = extract(copy(my_document), no_fallback=True, include_formatting=True, config=ZERO_CONFIG)
+    assert my_result == '**bold**, *italics*, `tt`, ~~deleted~~, __underlined__, link and additional text to bypass detection.'
+
+    my_result = extract(copy(my_document), no_fallback=True, include_links=True, include_formatting=True, config=ZERO_CONFIG)
+    assert my_result == '**bold**, *italics*, `tt`, ~~deleted~~, __underlined__, [link](test.html) and additional text to bypass detection.'
 
     my_result = extract(copy(my_document), output_format='xml', no_fallback=True, include_formatting=True, config=ZERO_CONFIG)
     assert '<p><hi rend="#b">bold</hi>, <hi rend="#i">italics</hi>, <hi rend="#t">tt</hi>, <del>deleted</del>, <hi rend="#u">underlined</hi>, link and additional text to bypass detection.</p>' in my_result
     assert 'rend="#b"' in my_result and 'rend="#i"' in my_result and 'rend="#t"' in my_result and 'rend="#u"' in my_result and '<del>' in my_result
 
     my_result = extract(copy(my_document), output_format='xml', include_formatting=True, include_links=True, no_fallback=True, config=ZERO_CONFIG)
     assert '<p><hi rend="#b">bold</hi>, <hi rend="#i">italics</hi>, <hi rend="#t">tt</hi>, <del>deleted</del>, <hi rend="#u">underlined</hi>, <ref target="test.html">link</ref> and additional text to bypass detection.</p>' in my_result
@@ -753,14 +758,27 @@
     trafilatura.htmlprocessing.process_node(line_break, options)
     assert line_break.text is None
     assert line_break.tail == "tail"
     node = etree.fromstring("<div><p>some text</p>tail</div>")[0]
     trafilatura.htmlprocessing.process_node(node, options)
     assert node.text == "some text"
     assert node.tail == "tail"
+    node = etree.fromstring("<p><ref target='url'><hi rend='#b'>bold</hi>inner</ref>outer</p>")[0]
+    processed = trafilatura.htmlprocessing.handle_textnode(node, options)
+    assert processed.tail == "outer"
+    node = etree.fromstring("<p><ref target='url'>text</ref>tail</p>")[0]
+    processed = trafilatura.htmlprocessing.handle_textnode(node, options)
+    assert processed.tail == "tail" and processed.text == "text"
+    node = etree.fromstring("<p><ref target='url'></ref>tail</p>")[0]
+    processed = trafilatura.htmlprocessing.handle_textnode(node, options)
+    assert processed.tail == "" and processed.text == "tail"
+    node = etree.fromstring("<p><ref target='url'>text<hi rend='#b'>bold</hi></ref>tail</p>")[0]
+    processed = trafilatura.htmlprocessing.handle_textnode(node, options)
+    assert processed.tail == "tail" and processed.text == "text"
+
 
 
 def test_extraction_options():
     '''Test the different parameters available in extract() and bare_extraction()'''
     my_html = '<html><head><meta http-equiv="content-language" content="EN"/></head><body><div="article-body"><p>Text.<!-- comment --></p></div></body></html>'
     with pytest.raises(NameError) as err:
         extract(my_html, json_output=True)
```

### Comparing `trafilatura-1.8.0/tests/xml_tei_tests.py` & `trafilatura-1.8.1/tests/xml_tei_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/__init__.py` & `trafilatura-1.8.1/trafilatura/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 
 __title__ = 'trafilatura'
 __author__ = 'Adrien Barbaresi and contributors'
 __license__ = "Apache-2.0"
 __copyright__ = 'Copyright 2019-2024, Adrien Barbaresi'
-__version__ = '1.8.0'
+__version__ = '1.8.1'
 
 
 import logging
 
 from .core import bare_extraction, baseline, extract, html2txt, process_record
 from .downloads import fetch_response, fetch_url
 from .metadata import extract_metadata
```

### Comparing `trafilatura-1.8.0/trafilatura/cli.py` & `trafilatura-1.8.1/trafilatura/cli.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/cli_utils.py` & `trafilatura-1.8.1/trafilatura/cli_utils.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/core.py` & `trafilatura-1.8.1/trafilatura/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import logging
 import re  # import regex as re
 import warnings
 from copy import deepcopy
 
-from lxml.etree import Element, SubElement, XPath, strip_elements, strip_tags
+from lxml.etree import Element, SubElement, XPath, strip_elements, strip_tags, tostring
 from lxml.html import tostring
 
 # own
 from .external import (SANITIZED_XPATH, justext_rescue, sanitize_tree,
                        try_readability)
 from .filters import (LANGID_FLAG, check_html_lang, duplicate_test,
                       language_filter, text_chars_test)
@@ -252,15 +252,15 @@
     if element.tag not in potential_tags:
         if element.tag != 'done':
             LOGGER.debug('discarding element: %s %s', element.tag, element.text)
         return None
     if element.tag == 'div':
         # make a copy and prune it in case it contains sub-elements handled on their own?
         # divcopy = deepcopy(element)
-        processed_element = handle_textnode(element, options, comments_fix=False)
+        processed_element = handle_textnode(element, options, comments_fix=False, preserve_spaces=True)
         if processed_element is not None and text_chars_test(processed_element.text) is True:
             processed_element.attrib.clear()
             # small div-correction # could be moved elsewhere
             if processed_element.tag == 'div':
                 processed_element.tag = 'p'
             # insert
             return processed_element
@@ -1015,14 +1015,17 @@
         return None
 
     # special case: python variables
     if output_format == 'python':
         document.text = xmltotxt(postbody, include_formatting)
         if include_comments is True:
             document.comments = xmltotxt(commentsbody, include_formatting)
+            document.commentsbody = commentsbody
+        document.raw_text = document.text
+        document.body = postbody
     else:
         document.raw_text, document.body, document.commentsbody = temp_text, postbody, commentsbody
     if as_dict is True:
         document = {slot: getattr(document, slot, None) for slot in document.__slots__}
     return document
 
 
@@ -1119,15 +1122,16 @@
     # post-processing
     if document is None:
         return None
     if output_format != 'txt':
         # add record ID to metadata
         document.id = record_id
         # calculate fingerprint
-        document.fingerprint = content_fingerprint(str(document.title) + " " + document.raw_text)
+        if document.raw_text is not None:
+            document.fingerprint = content_fingerprint(str(document.title) + " " + str(document.raw_text))
 
     # return
     return determine_returnstring(document, output_format, include_formatting, tei_validation)
 
 
 # for legacy and backwards compatibility
 def process_record(filecontent, url=None, record_id=None, no_fallback=False,
```

### Comparing `trafilatura-1.8.0/trafilatura/data/jt-stopwords-pickle.lzma` & `trafilatura-1.8.1/trafilatura/data/jt-stopwords-pickle.lzma`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/data/tei-schema-pickle.lzma` & `trafilatura-1.8.1/trafilatura/data/tei-schema-pickle.lzma`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/downloads.py` & `trafilatura-1.8.1/trafilatura/downloads.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/external.py` & `trafilatura-1.8.1/trafilatura/external.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import logging
 import lzma
 from pathlib import Path
 from pickle import load as load_pickle
 
 # third-party
-from justext.core import (ParagraphMaker, classify_paragraphs, preprocessor,
+from justext.core import (ParagraphMaker, classify_paragraphs,
                           revise_paragraph_classification)
 from justext.utils import get_stoplist  # , get_stoplists
 from lxml.etree import Element, strip_tags
 
 # own
 from .htmlprocessing import convert_tags, prune_unwanted_nodes, tree_cleaning
 from .readability_lxml import Document as ReadabilityDocument  # fork
@@ -52,16 +52,15 @@
     #     stoplist.update(get_stoplist(language))
     # JT_STOPLIST = tuple(stoplist)
     return JT_STOPLIST
 
 
 def custom_justext(tree, stoplist):
     'Customized version of JusText processing'
-    dom = preprocessor(tree)  # tree_cleaning(tree, True)
-    paragraphs = ParagraphMaker.make_paragraphs(dom)
+    paragraphs = ParagraphMaker.make_paragraphs(tree)
     classify_paragraphs(paragraphs, stoplist, 50, 200, 0.1, 0.2, 0.2, True)
     revise_paragraph_classification(paragraphs, 200)
     return paragraphs
 
 
 def try_justext(tree, url, target_language):
     '''Second safety net: try with the generic algorithm justext'''
```

### Comparing `trafilatura-1.8.0/trafilatura/feeds.py` & `trafilatura-1.8.1/trafilatura/feeds.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/filters.py` & `trafilatura-1.8.1/trafilatura/filters.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/gui.py` & `trafilatura-1.8.1/trafilatura/gui.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/hashing.py` & `trafilatura-1.8.1/trafilatura/hashing.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/htmlprocessing.py` & `trafilatura-1.8.1/trafilatura/htmlprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -304,38 +304,39 @@
         for elem in tree.iter('img'):
             elem.tag = 'graphic'
     return tree
 
 
 def handle_textnode(element, options, comments_fix=True, preserve_spaces=False):
     '''Convert, format, and probe potential text elements'''
-    if element.text is None and element.tail is None:
+    if element.text is None and element.tail is None and len(element) == 0:
         return None
     # lb bypass
     if comments_fix is False and element.tag == 'lb':
-        element.tail = trim(element.tail)
+        if preserve_spaces is False:
+            element.tail = trim(element.tail)
         # if textfilter(element) is True:
         #     return None
         # duplicate_test(subelement)?
         return element
-    if element.text is None:
+    if element.text is None and len(element) == 0:
         # try the tail
         # LOGGER.debug('using tail for element %s', element.tag)
         element.text, element.tail = element.tail, ''
         # handle differently for br/lb
         if comments_fix and element.tag == 'lb':
             element.tag = 'p'
     # trim
     if preserve_spaces is False:
         element.text = trim(element.text)
         if element.tail:
             element.tail = trim(element.tail)
     # filter content
     # or not re.search(r'\w', element.text):  # text_content()?
-    if not element.text or textfilter(element) is True:
+    if not element.text and textfilter(element) is True:
         return None
     if options.dedup and duplicate_test(element, options.config) is True:
         return None
     return element
 
 
 def process_node(element, options):
```

### Comparing `trafilatura-1.8.0/trafilatura/json_metadata.py` & `trafilatura-1.8.1/trafilatura/json_metadata.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/lru.py` & `trafilatura-1.8.1/trafilatura/lru.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/meta.py` & `trafilatura-1.8.1/trafilatura/meta.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/metadata.py` & `trafilatura-1.8.1/trafilatura/metadata.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/metaxpaths.py` & `trafilatura-1.8.1/trafilatura/metaxpaths.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/readability_lxml.py` & `trafilatura-1.8.1/trafilatura/readability_lxml.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/settings.cfg` & `trafilatura-1.8.1/trafilatura/settings.cfg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/settings.py` & `trafilatura-1.8.1/trafilatura/settings.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/sitemaps.py` & `trafilatura-1.8.1/trafilatura/sitemaps.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/spider.py` & `trafilatura-1.8.1/trafilatura/spider.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura/utils.py` & `trafilatura-1.8.1/trafilatura/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,16 +264,16 @@
         # remove newlines that are not related to punctuation or markup
         # remove non-printable chars and normalize space characters (including Unicode spaces)
         new_line = trim(LINES_TRIMMING.sub(r" ", new_line))
         # prune empty lines
         if all(map(str.isspace, new_line)):
             new_line = None
         elif trailing_space:
-            space_before = " " if line[0] == " " else ""
-            space_after = " " if line[-1] == " " else ""
+            space_before = " " if line[0].isspace() else ""
+            space_after = " " if line[-1].isspace() else ""
             new_line = "".join([space_before, new_line, space_after])
     return new_line
 
 
 def sanitize(text, preserve_space=False, trailing_space=False):
     '''Convert text and discard incompatible and invalid characters'''
     # consider all text as a single line
```

### Comparing `trafilatura-1.8.0/trafilatura/xml.py` & `trafilatura-1.8.1/trafilatura/xml.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 CONTROL_PARSER = XMLParser(remove_blank_text=True)
 
 NEWLINE_ELEMS = {
     'cell': '|',
     'item': '\n- ',
     **{tag: '\n' for tag in ['code', 'graphic', 'head', 'lb', 'list', 'p', 'quote', 'row', 'table']}
 }
-SPECIAL_FORMATTING = {'del', 'head', 'hi'}
+SPECIAL_FORMATTING = {'del', 'head', 'hi', 'ref'}
 WITH_ATTRIBUTES = {'cell', 'del', 'graphic', 'head', 'hi', 'item', 'list', 'ref'}
 
 NESTING_WHITELIST = {"cell", "figure", "item", "note", "quote"}
 
 META_ATTRIBUTES = [
     'sitename', 'title', 'author', 'date', 'url', 'hostname',
     'description', 'categories', 'tags', 'license', 'id',
@@ -207,57 +207,60 @@
     result = TEI_RELAXNG.validate(xmldoc)
     if result is False:
         LOGGER.warning('not a valid TEI document: %s', TEI_RELAXNG.error_log.last_error)
     return result
 
 
 def replace_element_text(element, include_formatting):
-    '''Determine element text based on text and tail'''
+    '''Determine element text based on **just the text** of the element. You must deal with the tail separately.'''
+    elem_text = element.text
     # handle formatting: convert to markdown
     if include_formatting is True and element.text is not None:
         if element.tag in ('del', 'head'):
             if element.tag == 'head':
                 try:
                     number = int(element.get('rend')[1])
                 except (TypeError, ValueError):
                     number = 2
-                element.text = f'{"#" * number} {element.text}'
+                elem_text = f'{"#" * number} {elem_text}'
             elif element.tag == 'del':
-                element.text = f'~~{element.text}~~'
+                elem_text = f'~~{elem_text}~~'
         elif element.tag == 'hi':
             rend = element.get('rend')
             if rend in HI_FORMATTING:
-                element.text = f'{HI_FORMATTING[rend]}{element.text}{HI_FORMATTING[rend]}'
+                elem_text = f'{HI_FORMATTING[rend]}{elem_text}{HI_FORMATTING[rend]}'
         elif element.tag == 'code':
             if '\n' in element.text:
-                element.text = f'```\n{element.text}\n```'
+                elem_text = f'```\n{elem_text}\n```'
             else:
-                element.text = f'`{element.text}`'
+                elem_text = f'`{elem_text}`'
     # handle links
     if element.tag == 'ref':
-        if element.text is not None:
-            link_text = f'[{element.text}]'
+        if elem_text is not None:
+            link_text = f'[{elem_text}]'
             if element.get('target') is not None:
-                element.text = f"{link_text}({element.get('target')})"
+                elem_text = f"{link_text}({element.get('target')})"
             else:
-                LOGGER.warning('missing link attribute: %s %s', element.text, element.attrib)
-                element.text = link_text
+                LOGGER.warning('missing link attribute: %s %s', elem_text, element.attrib)
+                elem_text = link_text
         else:
-            LOGGER.warning('empty link: %s %s', element.text, element.attrib)
+            LOGGER.warning('empty link: %s %s', elem_text, element.attrib)
     # handle text
-    return (element.text or '') + (element.tail or '')
+    return (elem_text or '')
 
 
 def merge_with_parent(element, include_formatting=False):
     '''Merge element with its parent and convert formatting to markdown.'''
     parent = element.getparent()
     if parent is None:
         return
 
     full_text = replace_element_text(element, include_formatting)
+    if element.tail is not None:
+        full_text = f'{full_text}{element.tail}'
 
     previous = element.getprevious()
     if previous is not None:
         # There is a previous node, append text to its tail
         if previous.tail is not None:
             previous.tail = f'{previous.tail} {full_text}'
         else:
@@ -265,40 +268,57 @@
     elif parent.text is not None:
         parent.text = f'{parent.text} {full_text}'
     else:
         parent.text = full_text
     parent.remove(element)
 
 
+def process_element(element, returnlist, include_formatting):
+    # Process children recursively
+    if element.text is not None:
+        # this is the text that comes before the first child
+        textelement = replace_element_text(element, include_formatting)
+        returnlist.append(textelement)
+
+    for child in element:
+        process_element(child, returnlist, include_formatting)
+
+    if element.text is None and element.tail is None:
+        if element.tag == 'graphic':
+            # add source, default to ''
+            text = f'{element.get("title", "")} {element.get("alt", "")}'
+            returnlist.extend(['![', text.strip(), ']', '(', element.get('src', ''), ')'])
+        # newlines for textless elements
+        if element.tag in ('graphic', 'row', 'table'):
+            returnlist.append('\n')
+        return  # Nothing more to do with textless elements
+
+    # Process text
+
+    # Common elements (Now processes end-tag logic correctly)
+    if element.tag in NEWLINE_ELEMS:
+        returnlist.extend([NEWLINE_ELEMS[element.tag], '\n'])
+    elif element.tag == 'comments':
+        returnlist.append('\n\n')
+    else:
+        if element.tag not in SPECIAL_FORMATTING:
+            LOGGER.debug('unprocessed element in output: %s', element.tag)
+            returnlist.extend([' '])
+
+    # this is text that comes after the closing tag, so it should be after any NEWLINE_ELEMS
+    if element.tail is not None:
+        returnlist.append(element.tail)
+
+
 def xmltotxt(xmloutput, include_formatting):
     '''Convert to plain text format and optionally preserve formatting as markdown.'''
     returnlist = []
-    # strip_tags(xmloutput, 'div', 'main', 'span')
-    # iterate and convert to list of strings
-    for element in xmloutput.iter('*'):
-        if element.text is None and element.tail is None:
-            if element.tag == 'graphic':
-                # add source, default to ''
-                text = f'{element.get("title", "")} {element.get("alt", "")}'
-                returnlist.extend(['![', text.strip(), ']', '(', element.get('src', ''), ')'])
-            # newlines for textless elements
-            if element.tag in ('graphic', 'row', 'table'):
-                returnlist.append('\n')
-            continue
-        # process text
-        textelement = replace_element_text(element, include_formatting)
-        # common elements
-        if element.tag in NEWLINE_ELEMS:
-            returnlist.extend([NEWLINE_ELEMS[element.tag], textelement, '\n'])
-        elif element.tag == 'comments':
-            returnlist.append('\n\n')
-        else:
-            if element.tag not in SPECIAL_FORMATTING:
-                LOGGER.debug('unprocessed element in output: %s', element.tag)
-            returnlist.extend([textelement, ' '])
+
+    process_element(xmloutput, returnlist, include_formatting)
+
     return unescape(sanitize(''.join(returnlist)))
 
 
 def xmltocsv(document, include_formatting, *, delim="\t", null="null"):
     "Convert the internal XML document representation to a CSV string."
     # preprocessing
     posttext = xmltotxt(document.body, include_formatting)
```

### Comparing `trafilatura-1.8.0/trafilatura/xpaths.py` & `trafilatura-1.8.1/trafilatura/xpaths.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,66 +109,69 @@
     contains(translate(@id, "S", "s"), "share") or
     contains(@id, "social") or contains(@class, "social") or contains(@class, "sociable") or
     contains(@id, "syndication") or contains(@class, "syndication") or
     starts-with(@id, "jp-") or starts-with(@id, "dpsp-content") or
     contains(@class, "embedded") or contains(@class, "embed")
     or contains(@id, "newsletter") or contains(@class, "newsletter")
     or contains(@class, "subnav") or
-    contains(@id, "cookie") or contains(@class, "cookie") or contains(@id, "tags")
-    or contains(@class, "tags")  or contains(@id, "sidebar") or
-    contains(@class, "sidebar") or contains(@id, "banner") or contains(@class, "banner")
-    or contains(@class, "meta") or
-    contains(@id, "menu") or contains(@class, "menu") or
+    contains(@id, "cookie") or contains(@class, "cookie") or
+    contains(@id, "tags") or contains(@class, "tags")  or contains(@class, "tag-list") or
+    contains(@id, "sidebar") or contains(@class, "sidebar") or
+    contains(@id, "banner") or contains(@class, "banner") or contains(@class, "bar") or
+    contains(@class, "meta") or contains(@id, "menu") or contains(@class, "menu") or
     contains(translate(@id, "N", "n"), "nav") or contains(translate(@role, "N", "n"), "nav")
     or starts-with(@class, "nav") or contains(translate(@class, "N", "n"), "navigation") or
     contains(@class, "navbar") or contains(@class, "navbox") or starts-with(@class, "post-nav")
     or contains(@id, "breadcrumb") or contains(@class, "breadcrumb") or
     contains(@id, "bread-crumb") or contains(@class, "bread-crumb") or
     contains(@id, "author") or contains(@class, "author") or
     contains(@id, "button") or contains(@class, "button")
     or contains(translate(@class, "B", "b"), "byline")
-    or contains(@class, "rating") or starts-with(@class, "widget") or
+    or contains(@class, "rating") or contains(@class, "widget") or
     contains(@class, "attachment") or contains(@class, "timestamp") or
     contains(@class, "user-info") or contains(@class, "user-profile") or
     contains(@class, "-ad-") or contains(@class, "-icon")
     or contains(@class, "article-infos") or
     contains(translate(@class, "I", "i"), "infoline")
     or contains(@data-component, "MostPopularStories")
     or contains(@class, "outbrain") or contains(@class, "taboola")
-    or contains(@class, "criteo") or contains(@class, "options")
+    or contains(@class, "criteo") or contains(@class, "options") or contains(@class, "expand")
     or contains(@class, "consent") or contains(@class, "modal-content")
     or contains(@class, "paid-content") or contains(@class, "paidcontent")
     or contains(@id, "premium-") or contains(@id, "paywall")
     or contains(@class, "obfuscated") or contains(@class, "blurred")
     or contains(@class, " ad ")
-    or contains(@class, "next-post") or contains(@class, "side-stories")
+    or contains(@class, "next-") or contains(@class, "side-stories")
     or contains(@class, "related-stories") or contains(@class, "most-popular")
     or contains(@class, "mol-factbox") or starts-with(@class, "ZendeskForm")
     or contains(@class, "message-container") or contains(@id, "message_container")
     or contains(@class, "yin") or contains(@class, "zlylin") or
-    contains(@class, "xg1") or contains(@id, "bmdh")
-    or @data-lp-replacement-content or @data-testid]''',
+    contains(@class, "xg1") or contains(@id, "bmdh") or
+    contains(@class, "slide") or contains(@class, "viewport") or
+    @data-lp-replacement-content or @data-testid]''',
 
     # comment debris + hidden parts
     '''.//*[@class="comments-title" or contains(@class, "comments-title") or
     contains(@class, "nocomments") or starts-with(@id, "reply-") or starts-with(@class, "reply-") or
     contains(@class, "-reply-") or contains(@class, "message") or contains(@id, "reader-comments")
     or contains(@id, "akismet") or contains(@class, "akismet") or contains(@class, "suggest-links") or
-    starts-with(@class, "hide-") or contains(@class, "hide-print") or contains(@id, "hidden")
-    or contains(@style, "hidden") or contains(@hidden, "hidden") or contains(@class, "noprint")
-    or contains(@style, "display:none") or contains(@style, "display: none") or contains(@class, " hidden") or @aria-hidden="true"
-    or contains(@class, "notloaded")]''',
+    starts-with(@class, "hide-") or contains(@class, "-hide-") or contains(@class, "hide-print") or
+    contains(@id, "hidden") or contains(@style, "hidden") or contains(@class, " hidden") or
+    contains(@class, "noprint") or contains(@style, "display:none") or contains(@style, "display: none")
+    or @aria-hidden="true" or contains(@class, "notloaded")]''',
 )]
 # conflicts:
 # contains(@id, "header") or contains(@class, "header") or
 # class contains "cats" (categories, also tags?)
 # or contains(@class, "hidden ")  or contains(@class, "-hide")
 # or contains(@class, "paywall")
 # contains(@class, "content-info") or contains(@class, "content-title")
 # contains(translate(@class, "N", "n"), "nav") or
+# contains(@class, "panel") or
+# or starts-with(@id, "comment-")
 
 
 # the following conditions focus on extraction precision
 TEASER_DISCARD_XPATH = [XPath(
     '''.//*[(self::div or self::item or self::list
              or self::p or self::section or self::span)][
         contains(translate(@id, "T", "t"), "teaser") or contains(translate(@class, "T", "t"), "teaser")
```

### Comparing `trafilatura-1.8.0/trafilatura.egg-info/PKG-INFO` & `trafilatura-1.8.1/trafilatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trafilatura
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python package and command-line tool designed to gather text on the Web, includes all necessary discovery and text processing components to perform web crawling, downloads, scraping, and extraction of main texts, metadata and comments.
 Home-page: https://trafilatura.readthedocs.io
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: Apache-2.0
 Project-URL: Documentation, https://trafilatura.readthedocs.io
 Project-URL: Source, https://github.com/adbar/trafilatura
@@ -44,15 +44,15 @@
 Requires-Dist: charset_normalizer>=3.0.1; python_version < "3.7"
 Requires-Dist: charset_normalizer>=3.2.0; python_version >= "3.7"
 Requires-Dist: courlan>=1.0.0
 Requires-Dist: htmldate>=1.8.0
 Requires-Dist: importlib_metadata; python_version < "3.8"
 Requires-Dist: justext>=3.0.0
 Requires-Dist: lxml==4.9.2; platform_system == "Darwin" and python_version <= "3.8"
-Requires-Dist: lxml<6,>=4.9.4; platform_system != "Darwin" or python_version > "3.8"
+Requires-Dist: lxml<5.2.0,>=4.9.4; platform_system != "Darwin" or python_version > "3.8"
 Requires-Dist: urllib3<2,>=1.26; python_version < "3.7"
 Requires-Dist: urllib3<3,>=1.26; python_version >= "3.7"
 Provides-Extra: all
 Requires-Dist: brotli; extra == "all"
 Requires-Dist: cchardet>=2.1.7; python_version < "3.11" and extra == "all"
 Requires-Dist: faust-cchardet>=2.1.19; python_version >= "3.11" and extra == "all"
 Requires-Dist: htmldate[speed]>=1.8.0; extra == "all"
```

### Comparing `trafilatura-1.8.0/trafilatura.egg-info/SOURCES.txt` & `trafilatura-1.8.1/trafilatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.0/trafilatura.egg-info/requires.txt` & `trafilatura-1.8.1/trafilatura.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 certifi
 courlan>=1.0.0
 htmldate>=1.8.0
 justext>=3.0.0
 
 [:platform_system != "Darwin" or python_version > "3.8"]
-lxml<6,>=4.9.4
+lxml<5.2.0,>=4.9.4
 
 [:platform_system == "Darwin" and python_version <= "3.8"]
 lxml==4.9.2
 
 [:python_version < "3.7"]
 charset_normalizer>=3.0.1
 urllib3<2,>=1.26
```

