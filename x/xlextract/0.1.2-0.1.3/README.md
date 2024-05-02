# Comparing `tmp/xlextract-0.1.2.tar.gz` & `tmp/xlextract-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlextract-0.1.2.tar", max compression
+gzip compressed data, was "xlextract-0.1.3.tar", max compression
```

## Comparing `xlextract-0.1.2.tar` & `xlextract-0.1.3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0      859 2024-05-01 19:03:49.374335 xlextract-0.1.2/README.md
--rw-r--r--   0        0        0      392 2024-05-01 19:04:15.564566 xlextract-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       34 2024-05-01 18:05:47.773922 xlextract-0.1.2/xlextract/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2024-05-01 18:06:56.104470 xlextract-0.1.2/xlextract/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180414 2024-05-01 18:05:47.673921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1647 2024-05-01 18:05:47.673921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    57974 2024-05-01 18:05:47.663921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1686 2024-05-01 18:05:47.663921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    24760 2024-05-01 18:05:47.663921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1643 2024-05-01 18:05:47.663921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0   113635 2024-05-01 18:05:47.663921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1711 2024-05-01 18:05:47.663921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    28418 2024-05-01 18:05:47.653921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1653 2024-05-01 18:05:47.653921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0  1711103 2024-05-01 18:05:47.743922 xlextract-0.1.2/xlextract/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1724 2024-05-01 18:05:47.743922 xlextract-0.1.2/xlextract/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   131375 2024-05-01 18:05:47.653921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1673 2024-05-01 18:05:47.653921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   801174 2024-05-01 18:05:47.653921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1713 2024-05-01 18:05:47.653921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3736 2024-05-01 18:05:47.623921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1624 2024-05-01 18:05:47.623921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   129375 2024-05-01 18:05:47.623921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1686 2024-05-01 18:05:47.623921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    83381 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1691 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0     7812 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1701 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    26274 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/_policybase.data.json
--rw-r--r--   0        0        0     1722 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/_policybase.meta.json
--rw-r--r--   0        0        0    16650 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1653 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7512 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1666 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25164 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1638 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9460 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1651 2024-05-01 18:05:47.613921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0   123702 2024-05-01 18:05:47.603921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1798 2024-05-01 18:05:47.603921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    12130 2024-05-01 18:05:47.603921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1702 2024-05-01 18:05:47.603921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0   116099 2024-05-01 18:05:47.603921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1667 2024-05-01 18:05:47.603921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    30801 2024-05-01 18:05:47.593921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1677 2024-05-01 18:05:47.593921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     6457 2024-05-01 18:05:47.593921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1703 2024-05-01 18:05:47.593921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0     5392 2024-05-01 18:05:47.593921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/_abc.data.json
--rw-r--r--   0        0        0     1666 2024-05-01 18:05:47.593921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/_abc.meta.json
--rw-r--r--   0        0        0    58770 2024-05-01 18:05:47.593921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1763 2024-05-01 18:05:47.593921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    77929 2024-05-01 18:05:47.593921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1808 2024-05-01 18:05:47.593921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0   117718 2024-05-01 18:05:47.583921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1833 2024-05-01 18:05:47.583921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    19857 2024-05-01 18:05:47.583921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1683 2024-05-01 18:05:47.583921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    22958 2024-05-01 18:05:47.583921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/readers.data.json
--rw-r--r--   0        0        0     1843 2024-05-01 18:05:47.583921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/readers.meta.json
--rw-r--r--   0        0        0    10874 2024-05-01 18:05:47.573921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/resources/__init__.data.json
--rw-r--r--   0        0        0     1767 2024-05-01 18:05:47.583921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/resources/__init__.meta.json
--rw-r--r--   0        0        0     1809 2024-05-01 18:05:47.573921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/resources/abc.data.json
--rw-r--r--   0        0        0     1666 2024-05-01 18:05:47.573921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/resources/abc.meta.json
--rw-r--r--   0        0        0   108464 2024-05-01 18:05:47.573921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1686 2024-05-01 18:05:47.573921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   405124 2024-05-01 18:05:47.573921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1755 2024-05-01 18:05:47.573921 xlextract-0.1.2/xlextract/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4913 2024-05-01 18:05:47.553920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1613 2024-05-01 18:05:47.553920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0   104515 2024-05-01 18:05:47.543920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1695 2024-05-01 18:05:47.543920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0   125881 2024-05-01 18:05:47.543920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1693 2024-05-01 18:05:47.543920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   246513 2024-05-01 18:05:47.543920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1714 2024-05-01 18:05:47.543920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    45119 2024-05-01 18:05:47.533920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/resource.data.json
--rw-r--r--   0        0        0     1628 2024-05-01 18:05:47.533920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/resource.meta.json
--rw-r--r--   0        0        0    14507 2024-05-01 18:05:47.533920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1638 2024-05-01 18:05:47.533920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28949 2024-05-01 18:05:47.533920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1663 2024-05-01 18:05:47.533920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    52302 2024-05-01 18:05:47.533920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1706 2024-05-01 18:05:47.533920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   224781 2024-05-01 18:05:47.523920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1688 2024-05-01 18:05:47.523920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   157649 2024-05-01 18:05:47.513920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/sys/__init__.data.json
--rw-r--r--   0        0        0     1735 2024-05-01 18:05:47.513920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/sys/__init__.meta.json
--rw-r--r--   0        0        0   310173 2024-05-01 18:05:47.513920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1704 2024-05-01 18:05:47.513920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   600170 2024-05-01 18:05:47.503920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1706 2024-05-01 18:05:47.503920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0   121173 2024-05-01 18:05:47.473920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1670 2024-05-01 18:05:47.473920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0     9572 2024-05-01 18:06:56.104470 xlextract-0.1.2/xlextract/.mypy_cache/3.11/xlextract/__init__.data.json
--rw-r--r--   0        0        0     1525 2024-05-01 18:06:56.104470 xlextract-0.1.2/xlextract/.mypy_cache/3.11/xlextract/__init__.meta.json
--rw-r--r--   0        0        0    12521 2024-05-01 18:06:19.624179 xlextract-0.1.2/xlextract/.mypy_cache/3.11/xlextract/xlextract.data.json
--rw-r--r--   0        0        0     1570 2024-05-01 18:06:19.624179 xlextract-0.1.2/xlextract/.mypy_cache/3.11/xlextract/xlextract.meta.json
--rw-r--r--   0        0        0    98226 2024-05-01 18:05:47.473920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/zipfile/__init__.data.json
--rw-r--r--   0        0        0     1699 2024-05-01 18:05:47.473920 xlextract-0.1.2/xlextract/.mypy_cache/3.11/zipfile/__init__.meta.json
--rw-r--r--   0        0        0      190 2024-05-01 18:05:47.773922 xlextract-0.1.2/xlextract/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     4310 2024-05-01 18:33:10.266838 xlextract-0.1.2/xlextract/__init__.py
--rw-r--r--   0        0        0     1884 2024-05-01 18:06:16.984157 xlextract-0.1.2/xlextract/classes.py
--rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 xlextract-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      768 2024-05-01 23:28:00.803700 xlextract-0.1.3/README.md
+-rw-r--r--   0        0        0      392 2024-05-01 23:27:54.723653 xlextract-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-05-01 18:05:47.773922 xlextract-0.1.3/xlextract/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0        2 2024-05-01 18:06:56.104470 xlextract-0.1.3/xlextract/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180414 2024-05-01 18:05:47.673921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1647 2024-05-01 18:05:47.673921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    57974 2024-05-01 18:05:47.663921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1686 2024-05-01 18:05:47.663921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    24760 2024-05-01 18:05:47.663921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1643 2024-05-01 18:05:47.663921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0   113635 2024-05-01 18:05:47.663921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1711 2024-05-01 18:05:47.663921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    28418 2024-05-01 18:05:47.653921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1653 2024-05-01 18:05:47.653921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0  1711103 2024-05-01 18:05:47.743922 xlextract-0.1.3/xlextract/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1724 2024-05-01 18:05:47.743922 xlextract-0.1.3/xlextract/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   131375 2024-05-01 18:05:47.653921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1673 2024-05-01 18:05:47.653921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   801174 2024-05-01 18:05:47.653921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1713 2024-05-01 18:05:47.653921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3736 2024-05-01 18:05:47.623921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1624 2024-05-01 18:05:47.623921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   129375 2024-05-01 18:05:47.623921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1686 2024-05-01 18:05:47.623921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    83381 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1691 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0     7812 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1701 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    26274 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/_policybase.data.json
+-rw-r--r--   0        0        0     1722 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/_policybase.meta.json
+-rw-r--r--   0        0        0    16650 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1653 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7512 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1666 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25164 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1638 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9460 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1651 2024-05-01 18:05:47.613921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0   123702 2024-05-01 18:05:47.603921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1798 2024-05-01 18:05:47.603921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    12130 2024-05-01 18:05:47.603921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1702 2024-05-01 18:05:47.603921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0   116099 2024-05-01 18:05:47.603921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1667 2024-05-01 18:05:47.603921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    30801 2024-05-01 18:05:47.593921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1677 2024-05-01 18:05:47.593921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     6457 2024-05-01 18:05:47.593921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1703 2024-05-01 18:05:47.593921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0     5392 2024-05-01 18:05:47.593921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/_abc.data.json
+-rw-r--r--   0        0        0     1666 2024-05-01 18:05:47.593921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/_abc.meta.json
+-rw-r--r--   0        0        0    58770 2024-05-01 18:05:47.593921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1763 2024-05-01 18:05:47.593921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    77929 2024-05-01 18:05:47.593921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1808 2024-05-01 18:05:47.593921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0   117718 2024-05-01 18:05:47.583921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1833 2024-05-01 18:05:47.583921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    19857 2024-05-01 18:05:47.583921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1683 2024-05-01 18:05:47.583921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    22958 2024-05-01 18:05:47.583921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/readers.data.json
+-rw-r--r--   0        0        0     1843 2024-05-01 18:05:47.583921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/readers.meta.json
+-rw-r--r--   0        0        0    10874 2024-05-01 18:05:47.573921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/resources/__init__.data.json
+-rw-r--r--   0        0        0     1767 2024-05-01 18:05:47.583921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/resources/__init__.meta.json
+-rw-r--r--   0        0        0     1809 2024-05-01 18:05:47.573921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/resources/abc.data.json
+-rw-r--r--   0        0        0     1666 2024-05-01 18:05:47.573921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/resources/abc.meta.json
+-rw-r--r--   0        0        0   108464 2024-05-01 18:05:47.573921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1686 2024-05-01 18:05:47.573921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   405124 2024-05-01 18:05:47.573921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1755 2024-05-01 18:05:47.573921 xlextract-0.1.3/xlextract/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4913 2024-05-01 18:05:47.553920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1613 2024-05-01 18:05:47.553920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0   104515 2024-05-01 18:05:47.543920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1695 2024-05-01 18:05:47.543920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0   125881 2024-05-01 18:05:47.543920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1693 2024-05-01 18:05:47.543920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   246513 2024-05-01 18:05:47.543920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1714 2024-05-01 18:05:47.543920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    45119 2024-05-01 18:05:47.533920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/resource.data.json
+-rw-r--r--   0        0        0     1628 2024-05-01 18:05:47.533920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/resource.meta.json
+-rw-r--r--   0        0        0    14507 2024-05-01 18:05:47.533920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1638 2024-05-01 18:05:47.533920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28949 2024-05-01 18:05:47.533920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1663 2024-05-01 18:05:47.533920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    52302 2024-05-01 18:05:47.533920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1706 2024-05-01 18:05:47.533920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   224781 2024-05-01 18:05:47.523920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1688 2024-05-01 18:05:47.523920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   157649 2024-05-01 18:05:47.513920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/sys/__init__.data.json
+-rw-r--r--   0        0        0     1735 2024-05-01 18:05:47.513920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/sys/__init__.meta.json
+-rw-r--r--   0        0        0   310173 2024-05-01 18:05:47.513920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1704 2024-05-01 18:05:47.513920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   600170 2024-05-01 18:05:47.503920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1706 2024-05-01 18:05:47.503920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0   121173 2024-05-01 18:05:47.473920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1670 2024-05-01 18:05:47.473920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0     9572 2024-05-01 18:06:56.104470 xlextract-0.1.3/xlextract/.mypy_cache/3.11/xlextract/__init__.data.json
+-rw-r--r--   0        0        0     1525 2024-05-01 18:06:56.104470 xlextract-0.1.3/xlextract/.mypy_cache/3.11/xlextract/__init__.meta.json
+-rw-r--r--   0        0        0    12521 2024-05-01 18:06:19.624179 xlextract-0.1.3/xlextract/.mypy_cache/3.11/xlextract/xlextract.data.json
+-rw-r--r--   0        0        0     1570 2024-05-01 18:06:19.624179 xlextract-0.1.3/xlextract/.mypy_cache/3.11/xlextract/xlextract.meta.json
+-rw-r--r--   0        0        0    98226 2024-05-01 18:05:47.473920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/zipfile/__init__.data.json
+-rw-r--r--   0        0        0     1699 2024-05-01 18:05:47.473920 xlextract-0.1.3/xlextract/.mypy_cache/3.11/zipfile/__init__.meta.json
+-rw-r--r--   0        0        0      190 2024-05-01 18:05:47.773922 xlextract-0.1.3/xlextract/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     4310 2024-05-01 18:33:10.266838 xlextract-0.1.3/xlextract/__init__.py
+-rw-r--r--   0        0        0     1884 2024-05-01 18:06:16.984157 xlextract-0.1.3/xlextract/classes.py
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 xlextract-0.1.3/PKG-INFO
```

### Comparing `xlextract-0.1.2/README.md` & `xlextract-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xlextract.svg)](https://img.shields.io/pypi/pyversions/xlextract)
 [![PyPI](https://img.shields.io/pypi/v/xlextract.svg)](https://pypi.python.org/pypi/xlextract)
-[![Downloads](https://static.pepy.tech/badge/xlextract)](https://static.pepy.tech/badge/xlextract)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 XLExtract
 =========
 
 An abstraction layer for quickly pulling data out of Microsoft Excel Spreadsheets.
 
 The project is currently powered by the [openpyxl](https://pypi.org/project/openpyxl/) library but you don't need to know anything about the underlying library and it could change in the future.
 
 ## Installation
-xlextract can be installed via poetry with: 'poetry add xlextract'  
-or via pip with: 'pip install xlextract'
+xlextract can be installed via poetry with: ```poetry add xlextract```  
+or via pip with: ```pip install xlextract```
```

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/_ast.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/_ast.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/_codecs.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/_codecs.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/_collections_abc.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/_collections_abc.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/_typeshed/__init__.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/abc.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/abc.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/builtins.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/builtins.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/codecs.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/codecs.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/collections/__init__.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/collections/__init__.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/collections/abc.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/collections/abc.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/contextlib.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/contextlib.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/dataclasses.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/dataclasses.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/__init__.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/__init__.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/_policybase.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/_policybase.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/_policybase.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/_policybase.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/charset.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/charset.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/contentmanager.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/contentmanager.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/errors.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/errors.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/header.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/header.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/message.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/message.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/policy.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/email/policy.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/enum.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/enum.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/genericpath.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/genericpath.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/__init__.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/__init__.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/_abc.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/_abc.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/_abc.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/_abc.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/abc.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/abc.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/machinery.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/machinery.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/readers.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/readers.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/readers.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/readers.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/resources/__init__.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/resources/__init__.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/resources/__init__.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/resources/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/resources/abc.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/resources/abc.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/importlib/resources/abc.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/importlib/resources/abc.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/io.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/io.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/os/__init__.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/os/__init__.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/os/path.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/os/path.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/pathlib.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/pathlib.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/posixpath.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/posixpath.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/re.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/re.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/resource.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/resource.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/resource.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/resource.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_compile.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_compile.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_constants.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_constants.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_parse.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/sre_parse.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/subprocess.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/subprocess.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/sys/__init__.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/sys/__init__.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/sys/__init__.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/sys/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/types.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/types.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/typing.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/typing.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/typing_extensions.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/typing_extensions.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/xlextract/__init__.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/xlextract/__init__.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/xlextract/__init__.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/xlextract/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/xlextract/xlextract.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/xlextract/xlextract.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/xlextract/xlextract.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/xlextract/xlextract.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/zipfile/__init__.data.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/zipfile/__init__.data.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/.mypy_cache/3.11/zipfile/__init__.meta.json` & `xlextract-0.1.3/xlextract/.mypy_cache/3.11/zipfile/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/__init__.py` & `xlextract-0.1.3/xlextract/__init__.py`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/xlextract/classes.py` & `xlextract-0.1.3/xlextract/classes.py`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.2/PKG-INFO` & `xlextract-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: xlextract
-Version: 0.1.2
+Version: 0.1.3
 Summary: Extract data from Excel files
 Author: AJ Cruz
 Author-email: aj.cruz@computacenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xlextract.svg)](https://img.shields.io/pypi/pyversions/xlextract)
 [![PyPI](https://img.shields.io/pypi/v/xlextract.svg)](https://pypi.python.org/pypi/xlextract)
-[![Downloads](https://static.pepy.tech/badge/xlextract)](https://static.pepy.tech/badge/xlextract)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 XLExtract
 =========
 
 An abstraction layer for quickly pulling data out of Microsoft Excel Spreadsheets.
 
 The project is currently powered by the [openpyxl](https://pypi.org/project/openpyxl/) library but you don't need to know anything about the underlying library and it could change in the future.
 
 ## Installation
-xlextract can be installed via poetry with: 'poetry add xlextract'  
-or via pip with: 'pip install xlextract'
+xlextract can be installed via poetry with: ```poetry add xlextract```  
+or via pip with: ```pip install xlextract```
```

