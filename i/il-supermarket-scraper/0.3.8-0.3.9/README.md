# Comparing `tmp/il_supermarket_scraper-0.3.8.tar.gz` & `tmp/il_supermarket_scraper-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "il_supermarket_scraper-0.3.8.tar", last modified: Thu Apr 18 10:08:10 2024, max compression
+gzip compressed data, was "il_supermarket_scraper-0.3.9.tar", last modified: Thu May  2 05:41:55 2024, max compression
```

## Comparing `il_supermarket_scraper-0.3.8.tar` & `il_supermarket_scraper-0.3.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.064190 il_supermarket_scraper-0.3.8/il_supermarket_scarper/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.068189 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/apsx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/bina.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/cerberus.py
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/multipage_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/publishprice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/web.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrapper_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.072189 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/bareket.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/bitan.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/cofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/doralon.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/good_pharm.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/hazihinam.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/het_cohen.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/keshet.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/king_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/maayan2000.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/machsani_ashuk.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/mega.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/nativ_hashed.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/osherad.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/polizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/quik.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/ramilevy.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/salachdabach.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/shefa_barcart_ashem.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/shufersal.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/shuk_ahir.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/stop_market.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/super_pharm.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/super_sapir.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/super_yuda.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/superdosh.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/tivtaam.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/victory.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/yellow.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/yohananof.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/zolvebegadol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/gzip_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/marking.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/retrey.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-18 10:08:10.000000 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-18 10:08:10.000000 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:08:10.000000 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 10:08:10.000000 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 10:08:10.000000 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:41:55.725089 il_supermarket_scraper-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-02 05:41:55.725089 il_supermarket_scraper-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:41:55.717089 il_supermarket_scraper-0.3.9/il_supermarket_scarper/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:41:55.717089 il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/apsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/bina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/cerberus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/multipage_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/publishprice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrapper_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:41:55.721089 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/bareket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/bitan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/cofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/doralon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/good_pharm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/hazihinam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/het_cohen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/keshet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/king_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/maayan2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/machsani_ashuk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/mega.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/nativ_hashed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/osherad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/polizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/quik.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/ramilevy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/salachdabach.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/shefa_barcart_ashem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/shufersal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/shuk_ahir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/stop_market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/super_pharm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/super_sapir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/super_yuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/superdosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/tivtaam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/victory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/yellow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/yohananof.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/zolvebegadol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:41:55.725089 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/gzip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/marking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/retrey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:41:55.725089 il_supermarket_scraper-0.3.9/il_supermarket_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-02 05:41:55.000000 il_supermarket_scraper-0.3.9/il_supermarket_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-02 05:41:55.000000 il_supermarket_scraper-0.3.9/il_supermarket_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 05:41:55.000000 il_supermarket_scraper-0.3.9/il_supermarket_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 05:41:55.000000 il_supermarket_scraper-0.3.9/il_supermarket_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 05:41:55.000000 il_supermarket_scraper-0.3.9/il_supermarket_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 05:41:55.729089 il_supermarket_scraper-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:41:55.725089 il_supermarket_scraper-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-02 05:41:51.000000 il_supermarket_scraper-0.3.9/tests/test_main.py
```

### Comparing `il_supermarket_scraper-0.3.8/LICENSE.txt` & `il_supermarket_scraper-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/PKG-INFO` & `il_supermarket_scraper-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: il-supermarket-scraper
-Version: 0.3.8
+Version: 0.3.9
 Summary: python package that implement a scraping for israeli supermarket data
 Home-page: https://github.com/jladan/package_demo
 Author: Sefi Erlich
 Author-email: erlichsefi@gmail.com
 License: MIT
 Keywords: israel,israeli,scraper,supermarket
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: retry==0.9.2
 Requires-Dist: mock==4.0.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: lxml==5.2.1
 Requires-Dist: beautifulsoup4==4.10.0
-Requires-Dist: pymongo==4.2.0
+Requires-Dist: pymongo==4.6.3
 Requires-Dist: pytz==2022.4
 Requires-Dist: holidays==0.16
 Requires-Dist: cachetools==5.2.0
 Requires-Dist: pytest-playwright==0.4.4
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `il_supermarket_scraper-0.3.8/README.md` & `il_supermarket_scraper-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/apsx.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/apsx.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/bina.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/bina.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/cerberus.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/cerberus.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/engine.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/engine.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/matrix.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/matrix.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/multipage_web.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/multipage_web.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/publishprice.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/publishprice.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/web.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/engines/web.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/main.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/main.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrapper_runner.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrapper_runner.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/__init__.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/bareket.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/bareket.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/cofix.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/cofix.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/nativ_hashed.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/nativ_hashed.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/polizer.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/polizer.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/super_pharm.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/super_pharm.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/tivtaam.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers/tivtaam.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers_factory.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/scrappers_factory.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/__init__.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/connection.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/connection.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/file_types.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/gzip_utils.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/gzip_utils.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/logger.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/loop.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/loop.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/marking.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/marking.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/mongo.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/mongo.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/retrey.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/retrey.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/status.py` & `il_supermarket_scraper-0.3.9/il_supermarket_scarper/utils/status.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/PKG-INFO` & `il_supermarket_scraper-0.3.9/il_supermarket_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: il-supermarket-scraper
-Version: 0.3.8
+Version: 0.3.9
 Summary: python package that implement a scraping for israeli supermarket data
 Home-page: https://github.com/jladan/package_demo
 Author: Sefi Erlich
 Author-email: erlichsefi@gmail.com
 License: MIT
 Keywords: israel,israeli,scraper,supermarket
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: retry==0.9.2
 Requires-Dist: mock==4.0.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: lxml==5.2.1
 Requires-Dist: beautifulsoup4==4.10.0
-Requires-Dist: pymongo==4.2.0
+Requires-Dist: pymongo==4.6.3
 Requires-Dist: pytz==2022.4
 Requires-Dist: holidays==0.16
 Requires-Dist: cachetools==5.2.0
 Requires-Dist: pytest-playwright==0.4.4
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/SOURCES.txt` & `il_supermarket_scraper-0.3.9/il_supermarket_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/setup.py` & `il_supermarket_scraper-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         "il_supermarket_scarper.utils",
     ],
     # Needed for dependencies
     install_requires=required,
     tests_require=dev_required,
     extras_require={"test": ["pytest"]},
     # *strongly* suggested for sharing
-    version="0.3.8",
+    version="0.3.9",
     # The license can be anything you like
     license="MIT",
     description="python package that implement a scraping for israeli supermarket data",
     # We will also need a readme eventually (there will be a warning)
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["israel", "israeli", "scraper", "supermarket"],
```

### Comparing `il_supermarket_scraper-0.3.8/tests/test_integration.py` & `il_supermarket_scraper-0.3.9/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `il_supermarket_scraper-0.3.8/tests/test_main.py` & `il_supermarket_scraper-0.3.9/tests/test_main.py`

 * *Files identical despite different names*

