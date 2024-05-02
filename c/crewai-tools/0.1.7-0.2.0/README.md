# Comparing `tmp/crewai_tools-0.1.7.tar.gz` & `tmp/crewai_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewai_tools-0.1.7.tar", max compression
+gzip compressed data, was "crewai_tools-0.2.0.tar", max compression
```

## Comparing `crewai_tools-0.1.7.tar` & `crewai_tools-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,56 @@
--rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.1.7/LICENSE
--rw-r--r--   0        0        0     3550 2024-02-26 00:09:39.177886 crewai_tools-0.1.7/README.md
--rw-r--r--   0        0        0      470 2024-03-03 02:54:55.157064 crewai_tools-0.1.7/crewai_tools/__init__.py
--rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.1.7/crewai_tools/adapters/embedchain_adapter.py
--rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.1.7/crewai_tools/adapters/lancedb_adapter.py
--rw-r--r--   0        0        0     1410 2024-03-03 02:54:59.436707 crewai_tools-0.1.7/crewai_tools/tools/__init__.py
--rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.1.7/crewai_tools/tools/base_tool.py
--rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.1.7/crewai_tools/tools/code_docs_search_tool/README.md
--rw-r--r--   0        0        0     1723 2024-04-10 14:50:04.964839 crewai_tools-0.1.7/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
--rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.1.7/crewai_tools/tools/csv_search_tool/README.md
--rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.965121 crewai_tools-0.1.7/crewai_tools/tools/csv_search_tool/csv_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.1.7/crewai_tools/tools/directory_read_tool/README.md
--rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.1.7/crewai_tools/tools/directory_read_tool/directory_read_tool.py
--rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.1.7/crewai_tools/tools/directory_search_tool/README.md
--rw-r--r--   0        0        0     1780 2024-04-10 14:50:04.965389 crewai_tools-0.1.7/crewai_tools/tools/directory_search_tool/directory_search_tool.py
--rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.1.7/crewai_tools/tools/docx_search_tool/README.md
--rw-r--r--   0        0        0     1642 2024-04-10 14:50:04.965572 crewai_tools-0.1.7/crewai_tools/tools/docx_search_tool/docx_search_tool.py
--rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.1.7/crewai_tools/tools/file_read_tool/README.md
--rw-r--r--   0        0        0     1056 2024-02-29 06:10:11.674186 crewai_tools-0.1.7/crewai_tools/tools/file_read_tool/file_read_tool.py
--rw-r--r--   0        0        0     2934 2024-04-10 14:50:04.965947 crewai_tools-0.1.7/crewai_tools/tools/github_search_tool/README.md
--rw-r--r--   0        0        0     2455 2024-04-10 14:50:04.966204 crewai_tools-0.1.7/crewai_tools/tools/github_search_tool/github_search_tool.py
--rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.1.7/crewai_tools/tools/json_search_tool/README.md
--rw-r--r--   0        0        0     1677 2024-04-10 14:50:04.966622 crewai_tools-0.1.7/crewai_tools/tools/json_search_tool/json_search_tool.py
--rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.1.7/crewai_tools/tools/mdx_seach_tool/README.md
--rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.966794 crewai_tools-0.1.7/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
--rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.1.7/crewai_tools/tools/pdf_search_tool/README.md
--rw-r--r--   0        0        0     1462 2024-04-10 14:50:04.967262 crewai_tools-0.1.7/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
--rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.1.7/crewai_tools/tools/pg_seach_tool/README.md
--rw-r--r--   0        0        0     1387 2024-04-04 16:45:56.495555 crewai_tools-0.1.7/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
--rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.1.7/crewai_tools/tools/rag/README.md
--rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.1.7/crewai_tools/tools/rag/__init__.py
--rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.1.7/crewai_tools/tools/rag/rag_tool.py
--rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.1.7/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
--rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.1.7/crewai_tools/tools/scrape_website_tool/README.md
--rw-r--r--   0        0        0     2135 2024-04-07 17:18:28.181398 crewai_tools-0.1.7/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
--rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.1.7/crewai_tools/tools/selenium_scraping_tool/README.md
--rw-r--r--   0        0        0     2558 2024-02-29 06:10:11.665178 crewai_tools-0.1.7/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
--rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.1.7/crewai_tools/tools/serper_dev_tool/README.md
--rw-r--r--   0        0        0     1365 2024-03-03 02:55:52.486790 crewai_tools-0.1.7/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
--rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.1.7/crewai_tools/tools/txt_search_tool/README.md
--rw-r--r--   0        0        0     1627 2024-04-10 14:50:04.967435 crewai_tools-0.1.7/crewai_tools/tools/txt_search_tool/txt_search_tool.py
--rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.1.7/crewai_tools/tools/website_search/README.md
--rw-r--r--   0        0        0     1713 2024-04-10 14:50:04.967608 crewai_tools-0.1.7/crewai_tools/tools/website_search/website_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.1.7/crewai_tools/tools/xml_search_tool/README.md
--rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.967788 crewai_tools-0.1.7/crewai_tools/tools/xml_search_tool/xml_search_tool.py
--rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.1.7/crewai_tools/tools/youtube_channel_search_tool/README.md
--rw-r--r--   0        0        0     2071 2024-04-10 14:50:04.968144 crewai_tools-0.1.7/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
--rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.1.7/crewai_tools/tools/youtube_video_search_tool/README.md
--rw-r--r--   0        0        0     1845 2024-04-10 14:50:04.968320 crewai_tools-0.1.7/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
--rw-r--r--   0        0        0      730 2024-04-10 14:50:15.447576 crewai_tools-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 crewai_tools-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3478 2024-05-02 06:04:48.741505 crewai_tools-0.2.0/README.md
+-rw-r--r--   0        0        0      509 2024-05-02 05:49:21.488653 crewai_tools-0.2.0/crewai_tools/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.2.0/crewai_tools/adapters/embedchain_adapter.py
+-rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.2.0/crewai_tools/adapters/lancedb_adapter.py
+-rw-r--r--   0        0        0     1541 2024-05-02 05:49:42.240076 crewai_tools-0.2.0/crewai_tools/tools/__init__.py
+-rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.2.0/crewai_tools/tools/base_tool.py
+-rw-r--r--   0        0        0      931 2024-05-02 05:36:37.312858 crewai_tools-0.2.0/crewai_tools/tools/browserbase_load_tool/README.md
+-rw-r--r--   0        0        0     1125 2024-05-02 05:36:37.313263 crewai_tools-0.2.0/crewai_tools/tools/browserbase_load_tool/browserbase_load_tool.py
+-rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.2.0/crewai_tools/tools/code_docs_search_tool/README.md
+-rw-r--r--   0        0        0     1723 2024-04-10 14:50:04.964839 crewai_tools-0.2.0/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
+-rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.2.0/crewai_tools/tools/csv_search_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.965121 crewai_tools-0.2.0/crewai_tools/tools/csv_search_tool/csv_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.2.0/crewai_tools/tools/directory_read_tool/README.md
+-rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.2.0/crewai_tools/tools/directory_read_tool/directory_read_tool.py
+-rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.2.0/crewai_tools/tools/directory_search_tool/README.md
+-rw-r--r--   0        0        0     1780 2024-04-10 14:50:04.965389 crewai_tools-0.2.0/crewai_tools/tools/directory_search_tool/directory_search_tool.py
+-rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.2.0/crewai_tools/tools/docx_search_tool/README.md
+-rw-r--r--   0        0        0     1642 2024-04-10 14:50:04.965572 crewai_tools-0.2.0/crewai_tools/tools/docx_search_tool/docx_search_tool.py
+-rw-r--r--   0        0        0     1472 2024-05-02 05:50:40.176058 crewai_tools-0.2.0/crewai_tools/tools/exa_tools/README.md
+-rw-r--r--   0        0        0     1087 2024-05-02 05:40:06.118673 crewai_tools-0.2.0/crewai_tools/tools/exa_tools/exa_base_tool.py
+-rw-r--r--   0        0        0      534 2024-05-02 05:49:03.207184 crewai_tools-0.2.0/crewai_tools/tools/exa_tools/exa_search_tool.py
+-rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.2.0/crewai_tools/tools/file_read_tool/README.md
+-rw-r--r--   0        0        0     1350 2024-05-02 05:36:37.313883 crewai_tools-0.2.0/crewai_tools/tools/file_read_tool/file_read_tool.py
+-rw-r--r--   0        0        0     2934 2024-04-10 14:50:04.965947 crewai_tools-0.2.0/crewai_tools/tools/github_search_tool/README.md
+-rw-r--r--   0        0        0     2455 2024-04-10 14:50:04.966204 crewai_tools-0.2.0/crewai_tools/tools/github_search_tool/github_search_tool.py
+-rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.2.0/crewai_tools/tools/json_search_tool/README.md
+-rw-r--r--   0        0        0     1677 2024-04-10 14:50:04.966622 crewai_tools-0.2.0/crewai_tools/tools/json_search_tool/json_search_tool.py
+-rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.2.0/crewai_tools/tools/mdx_seach_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.966794 crewai_tools-0.2.0/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
+-rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.2.0/crewai_tools/tools/pdf_search_tool/README.md
+-rw-r--r--   0        0        0     1462 2024-04-10 14:50:04.967262 crewai_tools-0.2.0/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
+-rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.2.0/crewai_tools/tools/pg_seach_tool/README.md
+-rw-r--r--   0        0        0     1387 2024-04-04 16:45:56.495555 crewai_tools-0.2.0/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
+-rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.2.0/crewai_tools/tools/rag/README.md
+-rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.2.0/crewai_tools/tools/rag/__init__.py
+-rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.2.0/crewai_tools/tools/rag/rag_tool.py
+-rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.2.0/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
+-rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.2.0/crewai_tools/tools/scrape_website_tool/README.md
+-rw-r--r--   0        0        0     2135 2024-04-07 17:18:28.181398 crewai_tools-0.2.0/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
+-rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.2.0/crewai_tools/tools/selenium_scraping_tool/README.md
+-rw-r--r--   0        0        0     2504 2024-05-02 06:04:48.748764 crewai_tools-0.2.0/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
+-rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.2.0/crewai_tools/tools/serper_dev_tool/README.md
+-rw-r--r--   0        0        0     1447 2024-05-02 05:48:30.482467 crewai_tools-0.2.0/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
+-rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.2.0/crewai_tools/tools/txt_search_tool/README.md
+-rw-r--r--   0        0        0     1627 2024-04-10 14:50:04.967435 crewai_tools-0.2.0/crewai_tools/tools/txt_search_tool/txt_search_tool.py
+-rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.2.0/crewai_tools/tools/website_search/README.md
+-rw-r--r--   0        0        0     1713 2024-04-10 14:50:04.967608 crewai_tools-0.2.0/crewai_tools/tools/website_search/website_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.2.0/crewai_tools/tools/xml_search_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.967788 crewai_tools-0.2.0/crewai_tools/tools/xml_search_tool/xml_search_tool.py
+-rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.2.0/crewai_tools/tools/youtube_channel_search_tool/README.md
+-rw-r--r--   0        0        0     2071 2024-04-10 14:50:04.968144 crewai_tools-0.2.0/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
+-rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.2.0/crewai_tools/tools/youtube_video_search_tool/README.md
+-rw-r--r--   0        0        0     1845 2024-04-10 14:50:04.968320 crewai_tools-0.2.0/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
+-rw-r--r--   0        0        0      730 2024-05-02 06:34:48.376376 crewai_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4541 1970-01-01 00:00:00.000000 crewai_tools-0.2.0/PKG-INFO
```

### Comparing `crewai_tools-0.1.7/LICENSE` & `crewai_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/README.md` & `crewai_tools-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 ## Creating Your Tools
 
 Tools are always expect to return strings, as they are meant to be used by the agents to generate responses.
 
 There are three ways to create tools for crewAI agents:
 - [Subclassing `BaseTool`](#subclassing-basetool)
-- [Creating a tool from a function or lambda](#functional-tool-creation)
 - [Using the `tool` decorator](#utilizing-the-tool-decorator)
 
 ### Subclassing `BaseTool`
 
 ```python
 from crewai_tools import BaseTool
 
@@ -118,8 +117,8 @@
 
 **Local Installation:**
 
 ```bash
 pip install dist/*.tar.gz
 ```
 
-Thank you for your interest in enhancing the capabilities of AI agents through advanced tooling. Your contributions make a significant impact.
+Thank you for your interest in enhancing the capabilities of AI agents through advanced tooling. Your contributions make a significant impact.
```

### Comparing `crewai_tools-0.1.7/crewai_tools/adapters/embedchain_adapter.py` & `crewai_tools-0.2.0/crewai_tools/adapters/embedchain_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/adapters/lancedb_adapter.py` & `crewai_tools-0.2.0/crewai_tools/adapters/lancedb_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/__init__.py` & `crewai_tools-0.2.0/crewai_tools/tools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from .browserbase_load_tool.browserbase_load_tool import BrowserbaseLoadTool
 from .code_docs_search_tool.code_docs_search_tool import CodeDocsSearchTool
 from .csv_search_tool.csv_search_tool import CSVSearchTool
 from .directory_search_tool.directory_search_tool import DirectorySearchTool
 from .directory_read_tool.directory_read_tool import DirectoryReadTool
 from .docx_search_tool.docx_search_tool import DOCXSearchTool
+from .exa_tools.exa_search_tool import EXASearchTool
 from .file_read_tool.file_read_tool import FileReadTool
 from .github_search_tool.github_search_tool import GithubSearchTool
 from .serper_dev_tool.serper_dev_tool import SerperDevTool
 from .txt_search_tool.txt_search_tool import TXTSearchTool
 from .json_search_tool.json_search_tool import JSONSearchTool
 from .mdx_seach_tool.mdx_search_tool import MDXSearchTool
 from .pdf_search_tool.pdf_search_tool import PDFSearchTool
@@ -14,8 +16,8 @@
 from .rag.rag_tool import RagTool
 from .scrape_element_from_website.scrape_element_from_website import ScrapeElementFromWebsiteTool
 from .scrape_website_tool.scrape_website_tool import ScrapeWebsiteTool
 from .selenium_scraping_tool.selenium_scraping_tool import SeleniumScrapingTool
 from .website_search.website_search_tool import WebsiteSearchTool
 from .xml_search_tool.xml_search_tool import XMLSearchTool
 from .youtube_channel_search_tool.youtube_channel_search_tool import YoutubeChannelSearchTool
-from .youtube_video_search_tool.youtube_video_search_tool import YoutubeVideoSearchTool
+from .youtube_video_search_tool.youtube_video_search_tool import YoutubeVideoSearchTool
```

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/base_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/code_docs_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/code_docs_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/csv_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/csv_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/csv_search_tool/csv_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/csv_search_tool/csv_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/directory_read_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/directory_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/directory_read_tool/directory_read_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/directory_read_tool/directory_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/directory_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/directory_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/directory_search_tool/directory_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/directory_search_tool/directory_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/docx_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/docx_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/docx_search_tool/docx_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/docx_search_tool/docx_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/file_read_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/file_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/file_read_tool/file_read_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/file_read_tool/file_read_tool.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 from typing import Optional, Type, Any
 from pydantic.v1 import BaseModel, Field
 from ..base_tool import BaseTool
 
+
 class FixedFileReadToolSchema(BaseModel):
-	"""Input for FileReadTool."""
-	pass
+    """Input for FileReadTool."""
+    pass
+
 
 class FileReadToolSchema(FixedFileReadToolSchema):
-	"""Input for FileReadTool."""
-	file_path: str = Field(..., description="Mandatory file full path to read the file")
+    """Input for FileReadTool."""
+    file_path: str = Field(
+        ...,
+        description="Mandatory file full path to read the file"
+    )
+
 
 class FileReadTool(BaseTool):
-	name: str = "Read a file's content"
-	description: str = "A tool that can be used to read a file's content."
-	args_schema: Type[BaseModel] = FileReadToolSchema
-	file_path: Optional[str] = None
-
-	def __init__(self, file_path: Optional[str] = None, **kwargs):
-		super().__init__(**kwargs)
-		if file_path is not None:
-			self.file_path = file_path
-			self.description = f"A tool that can be used to read {file_path}'s content."
-			self.args_schema = FixedFileReadToolSchema
-			self._generate_description()
-
-	def _run(
-		self,
-		**kwargs: Any,
-	) -> Any:
-		file_path = kwargs.get('file_path', self.file_path)
-		with open(file_path, 'r') as file:
-			return file.read()
+    name: str = "Read a file's content"
+    description: str = "A tool that can be used to read a file's content."
+    args_schema: Type[BaseModel] = FileReadToolSchema
+    file_path: Optional[str] = None
+
+    def __init__(
+        self,
+        file_path: Optional[str] = None,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
+        if file_path is not None:
+            self.file_path = file_path
+            self.description = f"A tool that can be used to read {file_path}'s content."
+            self.args_schema = FixedFileReadToolSchema
+            self._generate_description()
+
+    def _run(
+        self,
+        **kwargs: Any,
+    ) -> Any:
+        try:
+            file_path = kwargs.get('file_path', self.file_path)
+            with open(file_path, 'r') as file:
+                return file.read()
+        except Exception as e:
+            return f"Fail to read the file {file_path}. Error: {e}"
```

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/github_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/github_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/github_search_tool/github_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/github_search_tool/github_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/json_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/json_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/json_search_tool/json_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/json_search_tool/json_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/mdx_seach_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/mdx_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/pdf_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/pdf_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/pg_seach_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/pg_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/pg_seach_tool/pg_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/pg_seach_tool/pg_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/rag/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/rag/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/rag/rag_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/rag/rag_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py` & `crewai_tools-0.2.0/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/scrape_website_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/scrape_website_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/selenium_scraping_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/selenium_scraping_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 		driver = self._create_driver(website_url, self.cookie, self.wait_time)
 
 		content = []
 		if css_element is None or css_element.strip() == "":
 			body_text = driver.find_element(By.TAG_NAME, "body").text
 			content.append(body_text)
 		else:
-			driver.find_elements(By.CSS_SELECTOR, css_element)
 			for element in driver.find_elements(By.CSS_SELECTOR, css_element):
 				content.append(element.text)
 		driver.close()
 		return "\n".join(content)
 
 	def _create_driver(self, url, cookie, wait_time):
 			options = Options()
```

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/serper_dev_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/serper_dev_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,47 +3,50 @@
 import requests
 
 from typing import Type, Any
 from pydantic.v1 import BaseModel, Field
 from crewai_tools.tools.base_tool import BaseTool
 
 class SerperDevToolSchema(BaseModel):
-	"""Input for TXTSearchTool."""
+	"""Input for SerperDevTool."""
 	search_query: str = Field(..., description="Mandatory search query you want to use to search the internet")
 
 class SerperDevTool(BaseTool):
 	name: str = "Search the internet"
-	description: str = "A tool that can be used to semantic search a query from a txt's content."
+	description: str = "A tool that can be used to search the internet with a search_query."
 	args_schema: Type[BaseModel] = SerperDevToolSchema
 	search_url: str = "https://google.serper.dev/search"
-	n_results: int = None
+	n_results: int = 10
 
 	def _run(
 		self,
-		search_query: str,
 		**kwargs: Any,
 	) -> Any:
+		search_query = kwargs.get('search_query')
+		if search_query is None:
+			search_query = kwargs.get('query')
+
 		payload = json.dumps({"q": search_query})
 		headers = {
 				'X-API-KEY': os.environ['SERPER_API_KEY'],
 				'content-type': 'application/json'
 		}
 		response = requests.request("POST", self.search_url, headers=headers, data=payload)
 		results = response.json()
 		if 'organic' in results:
 			results = results['organic']
-			stirng = []
+			string = []
 			for result in results:
 				try:
-					stirng.append('\n'.join([
+					string.append('\n'.join([
 							f"Title: {result['title']}",
 							f"Link: {result['link']}",
 							f"Snippet: {result['snippet']}",
 							"---"
 					]))
 				except KeyError:
 					next
 
-			content = '\n'.join(stirng)
+			content = '\n'.join(string)
 			return f"\nSearch results: {content}\n"
 		else:
 			return results
```

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/txt_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/txt_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/txt_search_tool/txt_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/txt_search_tool/txt_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/website_search/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/website_search/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/website_search/website_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/website_search/website_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/xml_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/xml_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/xml_search_tool/xml_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/xml_search_tool/xml_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/youtube_channel_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/youtube_channel_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/youtube_video_search_tool/README.md` & `crewai_tools-0.2.0/crewai_tools/tools/youtube_video_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py` & `crewai_tools-0.2.0/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.7/pyproject.toml` & `crewai_tools-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crewai-tools"
-version = "0.1.7"
+version = "0.2.0"
 description = "Set of tools for the crewAI framework"
 authors = ["João Moura <joaomdmoura@mgail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.13"
 pydantic = "^2.6.1"
```

### Comparing `crewai_tools-0.1.7/PKG-INFO` & `crewai_tools-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crewai-tools
-Version: 0.1.7
+Version: 0.2.0
 Summary: Set of tools for the crewAI framework
 Author: João Moura
 Author-email: joaomdmoura@mgail.com
 Requires-Python: >=3.10,<=3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -56,15 +56,14 @@
 
 ## Creating Your Tools
 
 Tools are always expect to return strings, as they are meant to be used by the agents to generate responses.
 
 There are three ways to create tools for crewAI agents:
 - [Subclassing `BaseTool`](#subclassing-basetool)
-- [Creating a tool from a function or lambda](#functional-tool-creation)
 - [Using the `tool` decorator](#utilizing-the-tool-decorator)
 
 ### Subclassing `BaseTool`
 
 ```python
 from crewai_tools import BaseTool
 
@@ -146,7 +145,8 @@
 **Local Installation:**
 
 ```bash
 pip install dist/*.tar.gz
 ```
 
 Thank you for your interest in enhancing the capabilities of AI agents through advanced tooling. Your contributions make a significant impact.
+
```

