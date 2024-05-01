# Comparing `tmp/qai_scraper-0.5.tar.gz` & `tmp/qai_scraper-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_scraper-0.5.tar", max compression
+gzip compressed data, was "qai_scraper-0.5.1.tar", max compression
```

## Comparing `qai_scraper-0.5.tar` & `qai_scraper-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      314 2024-03-20 14:35:12.016070 qai_scraper-0.5/README.md
--rw-r--r--   0        0        0     1093 2024-05-01 22:26:05.245336 qai_scraper-0.5/pyproject.toml
--rw-r--r--   0        0        0      559 2024-03-22 05:00:53.167580 qai_scraper-0.5/src/qai/scraper/__init__.py
--rw-r--r--   0        0        0      120 2024-02-10 19:13:04.898933 qai_scraper-0.5/src/qai/scraper/definitions.py
--rw-r--r--   0        0        0    11491 2024-03-22 15:47:18.141931 qai_scraper-0.5/src/qai/scraper/filters/filter.py
--rw-r--r--   0        0        0      420 2024-02-26 02:13:14.624053 qai_scraper-0.5/src/qai/scraper/filters/meta.py
--rw-r--r--   0        0        0     1909 2024-03-22 21:59:22.960761 qai_scraper-0.5/src/qai/scraper/processors/div_table.py
--rw-r--r--   0        0        0     4007 2024-02-17 12:04:23.372421 qai_scraper-0.5/src/qai/scraper/processors/html_simplifier.py
--rw-r--r--   0        0        0      852 2024-03-22 23:23:34.994288 qai_scraper-0.5/src/qai/scraper/processors/html_writer.py
--rw-r--r--   0        0        0     1301 2024-02-22 15:49:44.518109 qai_scraper-0.5/src/qai/scraper/processors/markdown_writer.py
--rw-r--r--   0        0        0     1748 2024-02-26 02:05:06.080876 qai_scraper-0.5/src/qai/scraper/processors/one_deep_merger.py
--rw-r--r--   0        0        0     2425 2024-03-22 04:58:42.159671 qai_scraper-0.5/src/qai/scraper/processors/processor_factory.py
--rw-r--r--   0        0        0     1316 2024-02-10 19:14:41.681445 qai_scraper-0.5/src/qai/scraper/processors/processors.py
--rw-r--r--   0        0        0     1242 2024-02-10 18:29:46.395073 qai_scraper-0.5/src/qai/scraper/processors/tag_denester.py
--rw-r--r--   0        0        0     3642 2024-02-10 18:29:46.395363 qai_scraper-0.5/src/qai/scraper/processors/tag_keeper.py
--rw-r--r--   0        0        0     2731 2024-02-10 18:29:46.395675 qai_scraper-0.5/src/qai/scraper/processors/tag_remover.py
--rw-r--r--   0        0        0     1242 2024-02-10 18:29:46.395956 qai_scraper-0.5/src/qai/scraper/processors/tag_to_static.py
--rw-r--r--   0        0        0     1003 2024-02-16 00:18:14.303956 qai_scraper-0.5/src/qai/scraper/processors/text_writer.py
--rw-r--r--   0        0        0      889 2024-02-10 18:41:35.480070 qai_scraper-0.5/src/qai/scraper/processors/value_converter.py
--rw-r--r--   0        0        0     1734 2024-02-26 03:22:02.344850 qai_scraper-0.5/src/qai/scraper/processors/writer.py
--rw-r--r--   0        0        0      758 2024-02-25 19:07:13.133531 qai_scraper-0.5/src/qai/scraper/scrapers/meta.py
--rw-r--r--   0        0        0    11276 2024-03-22 05:53:36.865669 qai_scraper-0.5/src/qai/scraper/scrapers/scraper.py
--rw-r--r--   0        0        0      387 2024-02-29 15:44:12.259730 qai_scraper-0.5/src/qai/scraper/scrapers/scraper_factory.py
--rw-r--r--   0        0        0     3772 2024-02-13 23:10:17.438395 qai_scraper-0.5/src/qai/scraper/scrapers/stealthscraper.py
--rw-r--r--   0        0        0        0 2024-02-10 18:44:59.533302 qai_scraper-0.5/src/qai/scraper/utils/__init__.py
--rw-r--r--   0        0        0     5476 2024-03-22 16:02:38.975249 qai_scraper-0.5/src/qai/scraper/utils/bs_utils.py
--rw-r--r--   0        0        0     2133 2024-02-10 19:13:15.495694 qai_scraper-0.5/src/qai/scraper/utils/scrape_utils.py
--rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 qai_scraper-0.5/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-05-01 22:26:51.495059 qai_scraper-0.5.1/README.md
+-rw-r--r--   0        0        0     1095 2024-05-01 22:27:45.122577 qai_scraper-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      559 2024-03-22 05:00:53.167580 qai_scraper-0.5.1/src/qai/scraper/__init__.py
+-rw-r--r--   0        0        0      120 2024-02-10 19:13:04.898933 qai_scraper-0.5.1/src/qai/scraper/definitions.py
+-rw-r--r--   0        0        0    11491 2024-03-22 15:47:18.141931 qai_scraper-0.5.1/src/qai/scraper/filters/filter.py
+-rw-r--r--   0        0        0      420 2024-02-26 02:13:14.624053 qai_scraper-0.5.1/src/qai/scraper/filters/meta.py
+-rw-r--r--   0        0        0     1909 2024-03-22 21:59:22.960761 qai_scraper-0.5.1/src/qai/scraper/processors/div_table.py
+-rw-r--r--   0        0        0     4007 2024-02-17 12:04:23.372421 qai_scraper-0.5.1/src/qai/scraper/processors/html_simplifier.py
+-rw-r--r--   0        0        0      852 2024-03-22 23:23:34.994288 qai_scraper-0.5.1/src/qai/scraper/processors/html_writer.py
+-rw-r--r--   0        0        0     1301 2024-02-22 15:49:44.518109 qai_scraper-0.5.1/src/qai/scraper/processors/markdown_writer.py
+-rw-r--r--   0        0        0     1748 2024-02-26 02:05:06.080876 qai_scraper-0.5.1/src/qai/scraper/processors/one_deep_merger.py
+-rw-r--r--   0        0        0     2425 2024-03-22 04:58:42.159671 qai_scraper-0.5.1/src/qai/scraper/processors/processor_factory.py
+-rw-r--r--   0        0        0     1316 2024-02-10 19:14:41.681445 qai_scraper-0.5.1/src/qai/scraper/processors/processors.py
+-rw-r--r--   0        0        0     1242 2024-02-10 18:29:46.395073 qai_scraper-0.5.1/src/qai/scraper/processors/tag_denester.py
+-rw-r--r--   0        0        0     3642 2024-02-10 18:29:46.395363 qai_scraper-0.5.1/src/qai/scraper/processors/tag_keeper.py
+-rw-r--r--   0        0        0     2731 2024-02-10 18:29:46.395675 qai_scraper-0.5.1/src/qai/scraper/processors/tag_remover.py
+-rw-r--r--   0        0        0     1242 2024-02-10 18:29:46.395956 qai_scraper-0.5.1/src/qai/scraper/processors/tag_to_static.py
+-rw-r--r--   0        0        0     1003 2024-02-16 00:18:14.303956 qai_scraper-0.5.1/src/qai/scraper/processors/text_writer.py
+-rw-r--r--   0        0        0      889 2024-02-10 18:41:35.480070 qai_scraper-0.5.1/src/qai/scraper/processors/value_converter.py
+-rw-r--r--   0        0        0     1734 2024-02-26 03:22:02.344850 qai_scraper-0.5.1/src/qai/scraper/processors/writer.py
+-rw-r--r--   0        0        0      758 2024-02-25 19:07:13.133531 qai_scraper-0.5.1/src/qai/scraper/scrapers/meta.py
+-rw-r--r--   0        0        0    11276 2024-03-22 05:53:36.865669 qai_scraper-0.5.1/src/qai/scraper/scrapers/scraper.py
+-rw-r--r--   0        0        0      387 2024-02-29 15:44:12.259730 qai_scraper-0.5.1/src/qai/scraper/scrapers/scraper_factory.py
+-rw-r--r--   0        0        0     3772 2024-02-13 23:10:17.438395 qai_scraper-0.5.1/src/qai/scraper/scrapers/stealthscraper.py
+-rw-r--r--   0        0        0        0 2024-02-10 18:44:59.533302 qai_scraper-0.5.1/src/qai/scraper/utils/__init__.py
+-rw-r--r--   0        0        0     5476 2024-03-22 16:02:38.975249 qai_scraper-0.5.1/src/qai/scraper/utils/bs_utils.py
+-rw-r--r--   0        0        0     2133 2024-02-10 19:13:15.495694 qai_scraper-0.5.1/src/qai/scraper/utils/scrape_utils.py
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 qai_scraper-0.5.1/PKG-INFO
```

### Comparing `qai_scraper-0.5/pyproject.toml` & `qai_scraper-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
 description = ""
 name = "qai-scraper"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5"
+version = "0.5.1"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 beautifulsoup4 = "^4.12.2"
 bs4 = "^0.0.2"
 chromadb = "^0.4.22"
 flask = "^3.0.0"
```

### Comparing `qai_scraper-0.5/src/qai/scraper/__init__.py` & `qai_scraper-0.5.1/src/qai/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/filters/filter.py` & `qai_scraper-0.5.1/src/qai/scraper/filters/filter.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/div_table.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/div_table.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/html_simplifier.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/html_simplifier.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/html_writer.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/html_writer.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/markdown_writer.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/markdown_writer.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/one_deep_merger.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/one_deep_merger.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/processor_factory.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/processor_factory.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/processors.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/processors.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/tag_denester.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/tag_denester.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/tag_keeper.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/tag_keeper.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/tag_remover.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/tag_remover.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/tag_to_static.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/tag_to_static.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/text_writer.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/text_writer.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/value_converter.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/value_converter.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/processors/writer.py` & `qai_scraper-0.5.1/src/qai/scraper/processors/writer.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/scrapers/meta.py` & `qai_scraper-0.5.1/src/qai/scraper/scrapers/meta.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/scrapers/scraper.py` & `qai_scraper-0.5.1/src/qai/scraper/scrapers/scraper.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/scrapers/stealthscraper.py` & `qai_scraper-0.5.1/src/qai/scraper/scrapers/stealthscraper.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/utils/bs_utils.py` & `qai_scraper-0.5.1/src/qai/scraper/utils/bs_utils.py`

 * *Files identical despite different names*

### Comparing `qai_scraper-0.5/src/qai/scraper/utils/scrape_utils.py` & `qai_scraper-0.5.1/src/qai/scraper/utils/scrape_utils.py`

 * *Files identical despite different names*

