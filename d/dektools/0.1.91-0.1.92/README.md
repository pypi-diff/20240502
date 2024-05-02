# Comparing `tmp/dektools-0.1.91.tar.gz` & `tmp/dektools-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dektools-0.1.91.tar", last modified: Thu May  2 06:50:16 2024, max compression
+gzip compressed data, was "dektools-0.1.92.tar", last modified: Thu May  2 07:13:57 2024, max compression
```

## Comparing `dektools-0.1.91.tar` & `dektools-0.1.92.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0        0 2024-05-02 06:50:15.425673 dektools-0.1.91/README.md
--rw-r--r--   0        0        0        0 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/__init__.py
--rw-r--r--   0        0        0     2923 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/attr.py
--rw-r--r--   0        0        0        0 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/cache/__init__.py
--rw-r--r--   0        0        0      257 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/cache/base/__init__.py
--rw-r--r--   0        0        0     2359 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/cache/disk.py
--rw-r--r--   0        0        0     2202 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/cfg.py
--rw-r--r--   0        0        0      835 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/__entry__.py
--rw-r--r--   0        0        0       56 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/__init__.py
--rw-r--r--   0        0        0      426 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/cfg.py
--rw-r--r--   0        0        0      631 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/cmd.py
--rw-r--r--   0        0        0     2181 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/file.py
--rw-r--r--   0        0        0      632 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/hash.py
--rw-r--r--   0        0        0      278 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/net.py
--rw-r--r--   0        0        0     1080 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/print.py
--rw-r--r--   0        0        0      213 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/url.py
--rw-r--r--   0        0        0      134 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/utils.py
--rw-r--r--   0        0        0      241 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/click/version.py
--rw-r--r--   0        0        0      384 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/common.py
--rw-r--r--   0        0        0        0 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/crypto/__init__.py
--rw-r--r--   0        0        0      616 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/crypto/aes.py
--rw-r--r--   0        0        0     1713 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/derive.py
--rw-r--r--   0        0        0       91 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/dict/__init__.py
--rw-r--r--   0        0        0     1186 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/dict/chain.py
--rw-r--r--   0        0        0     3607 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/dict/configurable.py
--rw-r--r--   0        0        0     1070 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/dict/flat.py
--rw-r--r--   0        0        0     3657 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/dict/simple.py
--rw-r--r--   0        0        0     1319 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/download.py
--rw-r--r--   0        0        0        0 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/encode/__init__.py
--rw-r--r--   0        0        0     1479 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/encode/b62.py
--rw-r--r--   0        0        0      964 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/expression.py
--rw-r--r--   0        0        0     3379 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/__init__.py
--rw-r--r--   0        0        0     3547 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/filter/__init__.py
--rw-r--r--   0        0        0       42 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/filter/utils/__init__.py
--rw-r--r--   0        0        0      740 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/filter/utils/attr.py
--rw-r--r--   0        0        0      514 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/filter/utils/method.py
--rw-r--r--   0        0        0      759 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/__init__.py
--rw-r--r--   0        0        0      434 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/base/__init__.py
--rw-r--r--   0        0        0      224 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/chain.py
--rw-r--r--   0        0        0      528 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/data.py
--rw-r--r--   0        0        0      193 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/filter.py
--rw-r--r--   0        0        0     1341 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/if_.py
--rw-r--r--   0        0        0      269 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/key.py
--rw-r--r--   0        0        0      325 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/keyvar.py
--rw-r--r--   0        0        0      598 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/list.py
--rw-r--r--   0        0        0      302 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/storageflush.py
--rw-r--r--   0        0        0      431 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/instruction/var.py
--rw-r--r--   0        0        0       23 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/produce/__init__.py
--rw-r--r--   0        0        0      571 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/produce/base/__init__.py
--rw-r--r--   0        0        0       76 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/produce/default.py
--rw-r--r--   0        0        0      456 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/storage.py
--rw-r--r--   0        0        0      986 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/value.py
--rw-r--r--   0        0        0     1024 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/extraction/variables.py
--rw-r--r--   0        0        0       64 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/file/__init__.py
--rw-r--r--   0        0        0     4023 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/file/hit.py
--rw-r--r--   0        0        0     6883 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/file/operation.py
--rw-r--r--   0        0        0      474 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/file/path.py
--rw-r--r--   0        0        0     1565 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/format.py
--rw-r--r--   0        0        0     1299 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/func.py
--rw-r--r--   0        0        0      469 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/hash.py
--rw-r--r--   0        0        0     1366 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/module.py
--rw-r--r--   0        0        0     1887 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/net.py
--rw-r--r--   0        0        0      741 2024-05-02 06:50:15.425673 dektools-0.1.91/dektools/output.py
--rw-r--r--   0        0        0      494 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/package/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/package/lock/__init__.py
--rw-r--r--   0        0        0      277 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/package/lock/base/__init__.py
--rw-r--r--   0        0        0      208 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/package/lock/pdm.py
--rw-r--r--   0        0        0       88 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/py.py
--rw-r--r--   0        0        0      419 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/re.py
--rw-r--r--   0        0        0      263 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/reactive.py
--rw-r--r--   0        0        0     1129 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/repr.py
--rw-r--r--   0        0        0     5814 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/shell.py
--rw-r--r--   0        0        0      742 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/snowflake.py
--rw-r--r--   0        0        0     1388 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/sort.py
--rw-r--r--   0        0        0     5729 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/str.py
--rw-r--r--   0        0        0     2818 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/sync.py
--rw-r--r--   0        0        0     1473 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/sys.py
--rw-r--r--   0        0        0     1306 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/task.py
--rw-r--r--   0        0        0     2709 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/time.py
--rw-r--r--   0        0        0     3979 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/typer/__init__.py
--rw-r--r--   0        0        0      930 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/typer/annotation.py
--rw-r--r--   0        0        0     1751 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/url.py
--rw-r--r--   0        0        0      651 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/variables.py
--rw-r--r--   0        0        0      940 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/version.py
--rw-r--r--   0        0        0     3138 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/yaml/__init__.py
--rw-r--r--   0        0        0       19 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/yaml/tags/__init__.py
--rw-r--r--   0        0        0     1450 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/yaml/tags/base/__init__.py
--rw-r--r--   0        0        0      179 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/yaml/tags/repr.py
--rw-r--r--   0        0        0      174 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/yaml/tags/str.py
--rw-r--r--   0        0        0     2517 2024-05-02 06:50:15.429673 dektools-0.1.91/dektools/zip.py
--rw-r--r--   0        0        0      756 2024-05-02 06:50:16.705664 dektools-0.1.91/pyproject.toml
--rw-r--r--   0        0        0       89 2024-05-02 06:50:15.429673 dektools-0.1.91/tests/__init__.py
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 dektools-0.1.91/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-02 07:13:55.743665 dektools-0.1.92/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/__init__.py
+-rw-r--r--   0        0        0     2923 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/attr.py
+-rw-r--r--   0        0        0        0 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/cache/__init__.py
+-rw-r--r--   0        0        0      257 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/cache/base/__init__.py
+-rw-r--r--   0        0        0     2359 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/cache/disk.py
+-rw-r--r--   0        0        0     2202 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/cfg.py
+-rw-r--r--   0        0        0      835 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/__entry__.py
+-rw-r--r--   0        0        0       56 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/cfg.py
+-rw-r--r--   0        0        0      631 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/cmd.py
+-rw-r--r--   0        0        0     2181 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/file.py
+-rw-r--r--   0        0        0      632 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/hash.py
+-rw-r--r--   0        0        0      278 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/net.py
+-rw-r--r--   0        0        0     1080 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/print.py
+-rw-r--r--   0        0        0      213 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/url.py
+-rw-r--r--   0        0        0      134 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/utils.py
+-rw-r--r--   0        0        0      241 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/click/version.py
+-rw-r--r--   0        0        0      384 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/common.py
+-rw-r--r--   0        0        0        0 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/crypto/__init__.py
+-rw-r--r--   0        0        0     1085 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/crypto/aes.py
+-rw-r--r--   0        0        0     1713 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/derive.py
+-rw-r--r--   0        0        0       91 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/dict/__init__.py
+-rw-r--r--   0        0        0     1186 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/dict/chain.py
+-rw-r--r--   0        0        0     3607 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/dict/configurable.py
+-rw-r--r--   0        0        0     1070 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/dict/flat.py
+-rw-r--r--   0        0        0     3657 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/dict/simple.py
+-rw-r--r--   0        0        0     1319 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/download.py
+-rw-r--r--   0        0        0        0 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/encode/__init__.py
+-rw-r--r--   0        0        0     1479 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/encode/b62.py
+-rw-r--r--   0        0        0      964 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/expression.py
+-rw-r--r--   0        0        0     3379 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/__init__.py
+-rw-r--r--   0        0        0     3547 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/filter/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/filter/utils/__init__.py
+-rw-r--r--   0        0        0      740 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/filter/utils/attr.py
+-rw-r--r--   0        0        0      514 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/filter/utils/method.py
+-rw-r--r--   0        0        0      759 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/__init__.py
+-rw-r--r--   0        0        0      434 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/base/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/chain.py
+-rw-r--r--   0        0        0      528 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/data.py
+-rw-r--r--   0        0        0      193 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/filter.py
+-rw-r--r--   0        0        0     1341 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/if_.py
+-rw-r--r--   0        0        0      269 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/key.py
+-rw-r--r--   0        0        0      325 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/keyvar.py
+-rw-r--r--   0        0        0      598 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/list.py
+-rw-r--r--   0        0        0      302 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/storageflush.py
+-rw-r--r--   0        0        0      431 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/instruction/var.py
+-rw-r--r--   0        0        0       23 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/produce/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/produce/base/__init__.py
+-rw-r--r--   0        0        0       76 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/produce/default.py
+-rw-r--r--   0        0        0      456 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/storage.py
+-rw-r--r--   0        0        0      986 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/value.py
+-rw-r--r--   0        0        0     1024 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/extraction/variables.py
+-rw-r--r--   0        0        0       64 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/file/__init__.py
+-rw-r--r--   0        0        0     4023 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/file/hit.py
+-rw-r--r--   0        0        0     6883 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/file/operation.py
+-rw-r--r--   0        0        0      474 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/file/path.py
+-rw-r--r--   0        0        0     1565 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/format.py
+-rw-r--r--   0        0        0     1299 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/func.py
+-rw-r--r--   0        0        0      469 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/hash.py
+-rw-r--r--   0        0        0     1366 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/module.py
+-rw-r--r--   0        0        0     1887 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/net.py
+-rw-r--r--   0        0        0      741 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/output.py
+-rw-r--r--   0        0        0      494 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/package/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/package/lock/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/package/lock/base/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/package/lock/pdm.py
+-rw-r--r--   0        0        0       88 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/py.py
+-rw-r--r--   0        0        0      419 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/re.py
+-rw-r--r--   0        0        0      263 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/reactive.py
+-rw-r--r--   0        0        0     1129 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/repr.py
+-rw-r--r--   0        0        0     5814 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/shell.py
+-rw-r--r--   0        0        0      742 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/snowflake.py
+-rw-r--r--   0        0        0     1388 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/sort.py
+-rw-r--r--   0        0        0     5729 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/str.py
+-rw-r--r--   0        0        0     2818 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/sync.py
+-rw-r--r--   0        0        0     1473 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/sys.py
+-rw-r--r--   0        0        0     1306 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/task.py
+-rw-r--r--   0        0        0     2709 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/time.py
+-rw-r--r--   0        0        0     3979 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/typer/__init__.py
+-rw-r--r--   0        0        0      930 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/typer/annotation.py
+-rw-r--r--   0        0        0     1751 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/url.py
+-rw-r--r--   0        0        0      651 2024-05-02 07:13:55.743665 dektools-0.1.92/dektools/variables.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:13:55.747666 dektools-0.1.92/dektools/version.py
+-rw-r--r--   0        0        0     3138 2024-05-02 07:13:55.747666 dektools-0.1.92/dektools/yaml/__init__.py
+-rw-r--r--   0        0        0       19 2024-05-02 07:13:55.747666 dektools-0.1.92/dektools/yaml/tags/__init__.py
+-rw-r--r--   0        0        0     1450 2024-05-02 07:13:55.747666 dektools-0.1.92/dektools/yaml/tags/base/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-02 07:13:55.747666 dektools-0.1.92/dektools/yaml/tags/repr.py
+-rw-r--r--   0        0        0      174 2024-05-02 07:13:55.747666 dektools-0.1.92/dektools/yaml/tags/str.py
+-rw-r--r--   0        0        0     2517 2024-05-02 07:13:55.747666 dektools-0.1.92/dektools/zip.py
+-rw-r--r--   0        0        0      756 2024-05-02 07:13:57.055659 dektools-0.1.92/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-05-02 07:13:55.747666 dektools-0.1.92/tests/__init__.py
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 dektools-0.1.92/PKG-INFO
```

### Comparing `dektools-0.1.91/dektools/attr.py` & `dektools-0.1.92/dektools/attr.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/cache/disk.py` & `dektools-0.1.92/dektools/cache/disk.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/cfg.py` & `dektools-0.1.92/dektools/cfg.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/click/__entry__.py` & `dektools-0.1.92/dektools/click/__entry__.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/click/cmd.py` & `dektools-0.1.92/dektools/click/cmd.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/click/file.py` & `dektools-0.1.92/dektools/click/file.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/click/hash.py` & `dektools-0.1.92/dektools/click/hash.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/click/print.py` & `dektools-0.1.92/dektools/click/print.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/derive.py` & `dektools-0.1.92/dektools/derive.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/dict/chain.py` & `dektools-0.1.92/dektools/dict/chain.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/dict/configurable.py` & `dektools-0.1.92/dektools/dict/configurable.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/dict/flat.py` & `dektools-0.1.92/dektools/dict/flat.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/dict/simple.py` & `dektools-0.1.92/dektools/dict/simple.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/download.py` & `dektools-0.1.92/dektools/download.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/encode/b62.py` & `dektools-0.1.92/dektools/encode/b62.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/expression.py` & `dektools-0.1.92/dektools/expression.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/__init__.py` & `dektools-0.1.92/dektools/extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/filter/__init__.py` & `dektools-0.1.92/dektools/extraction/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/filter/utils/attr.py` & `dektools-0.1.92/dektools/extraction/filter/utils/attr.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/filter/utils/method.py` & `dektools-0.1.92/dektools/extraction/filter/utils/method.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/instruction/__init__.py` & `dektools-0.1.92/dektools/extraction/instruction/__init__.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/instruction/data.py` & `dektools-0.1.92/dektools/extraction/instruction/data.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/instruction/if_.py` & `dektools-0.1.92/dektools/extraction/instruction/if_.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/instruction/list.py` & `dektools-0.1.92/dektools/extraction/instruction/list.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/produce/base/__init__.py` & `dektools-0.1.92/dektools/extraction/produce/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/value.py` & `dektools-0.1.92/dektools/extraction/value.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/extraction/variables.py` & `dektools-0.1.92/dektools/extraction/variables.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/file/hit.py` & `dektools-0.1.92/dektools/file/hit.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/file/operation.py` & `dektools-0.1.92/dektools/file/operation.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/format.py` & `dektools-0.1.92/dektools/format.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/func.py` & `dektools-0.1.92/dektools/func.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/module.py` & `dektools-0.1.92/dektools/module.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/net.py` & `dektools-0.1.92/dektools/net.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/output.py` & `dektools-0.1.92/dektools/output.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/repr.py` & `dektools-0.1.92/dektools/repr.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/shell.py` & `dektools-0.1.92/dektools/shell.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/snowflake.py` & `dektools-0.1.92/dektools/snowflake.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/sort.py` & `dektools-0.1.92/dektools/sort.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/str.py` & `dektools-0.1.92/dektools/str.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/sync.py` & `dektools-0.1.92/dektools/sync.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/sys.py` & `dektools-0.1.92/dektools/sys.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/task.py` & `dektools-0.1.92/dektools/task.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/time.py` & `dektools-0.1.92/dektools/time.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/typer/__init__.py` & `dektools-0.1.92/dektools/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/typer/annotation.py` & `dektools-0.1.92/dektools/typer/annotation.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/url.py` & `dektools-0.1.92/dektools/url.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/variables.py` & `dektools-0.1.92/dektools/variables.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/version.py` & `dektools-0.1.92/dektools/version.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/yaml/__init__.py` & `dektools-0.1.92/dektools/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/yaml/tags/base/__init__.py` & `dektools-0.1.92/dektools/yaml/tags/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/dektools/zip.py` & `dektools-0.1.92/dektools/zip.py`

 * *Files identical despite different names*

### Comparing `dektools-0.1.91/pyproject.toml` & `dektools-0.1.92/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dektools"
-version = "0.1.91"
+version = "0.1.92"
 description = ""
 authors = [
     { name = "sanzenwin", email = "sanzenwin@gmail.com" },
 ]
 dependencies = [
     "igittigitt<=2.0.4",
     "pyyaml<=6.0.1",
```

### Comparing `dektools-0.1.91/PKG-INFO` & `dektools-0.1.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dektools
-Version: 0.1.91
+Version: 0.1.92
 Author-Email: sanzenwin <sanzenwin@gmail.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: igittigitt<=2.0.4
 Requires-Dist: pyyaml<=6.0.1
 Requires-Dist: yamlloader<=1.3.2
 Requires-Dist: pybase62<=1.0.0
```

